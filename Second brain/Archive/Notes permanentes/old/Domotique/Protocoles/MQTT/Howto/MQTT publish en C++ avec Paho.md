---
alias:
metadata: 02
author: AUGST-MERELLE Alexandra
type: howto
status: ready
keywords: cpp, paho, mqtt
creation: 2021-06-27
modification: 2021-06-27
---
 | 
------------ | ------------
MOC | [[DOMOTIQUE]] [[DEV]]
Project | [[Domotique (Projet)]] [[Polaris (Projet)]] [[cpp (Projet)]]
Template | [[Archive/Notes permanentes]]
Source | [[www.eclipse.org]]
# [[MQTT]] [[publish]] en [[Dev (index)]] avec [[Paho]]
MQTT publish en C++ avec Paho

Here is a simple example of publishing with the C++ client [[synchronous]] API:

```cpp
int main(int argc, char* argv[])
{
    const std::string TOPIC { "hello" };
    const std::string PAYLOAD1 { "Hello World!" };

    const char* PAYLOAD2 = "Hi there!";

    // Create a client

    mqtt::client cli(ADDRESS, CLIENT_ID);

    mqtt::connect_options connOpts;
    connOpts.set_keep_alive_interval(20);
    connOpts.set_clean_session(true);

    try {
        // Connect to the client

        cli.connect(connOpts);

        // Publish using a message pointer.

        auto msg = mqtt::make_message(TOPIC, PAYLOAD1);
        msg->set_qos(QOS);

        cli.publish(msg);

        // Now try with itemized publish.

        cli.publish(TOPIC, PAYLOAD2, strlen(PAYLOAD2), 0, false);

        // Disconnect

        cli.disconnect();
    }
    catch (const mqtt::exception& exc) {
        std::cerr << "Error: " << exc.what() << " ["
            << exc.get_reason_code() << "]" << std::endl;
        return 1;
    }

    return 0;
}
```
## Référence
[www.eclipse.org](https://www.eclipse.org/paho/index.php?page=clients/cpp/index.php)
## Liens
[[code]] [[cpp]]