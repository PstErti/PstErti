<!---
PstErti/PstErti is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

```cpp

#include <string>
#include <map>

struct PstErti {

    static PstErti* instance;

    std::string name = "PstErti";
    std::string gender = "M";
    std::string birthday = "2008/10/13";

    const bool isSensitive = true;
    const bool isKind = true;
    const bool isReflective = true;
    const bool isLonely = true;
    const bool isResilient = true;

    static std::map<std::string, std::string> contactInfo;

    PstErti() = default;

    PstErti(const PstErti&) = delete;
    PstErti& operator=(const PstErti&) = delete;

    static PstErti* getInstance() {
        if (!instance) {
            instance = new PstErti();
        }
        return instance;
    }
};

PstErti* PstErti::instance = nullptr;
std::map<std::string, std::string> PstErti::contactInfo = 
{
    {"Tel", "+86 18972666975"},
    {"WeChat", "PstErti"},
};

```
