## How Can Juice Rescue Save Your EV Charger? \- A Survey

*January 4, 2025*

Two months after the [Juice Rescue](https://juice-rescue.org/) project formed to support people faced with the end of their JuiceBox chargers, our community of over 200 has already helped people understand the situation, keep their chargers running, and [advocate for change in partnership with Consumer Reports](https://advocacy.consumerreports.org/press_release/ftc-software-tethering/). **THANK YOU\!**

In response to the pressure, Enel X way has kept the app running (for now) and has sold the company to another business, who haven't yet announced any plans. Furthermore, the maker of the JuiceBox's underlying chip has promised not to offer any more security updates after a [security vulnerability was released](https://vicone.com/blog/from-pwn2own-automotive-a-stack-based-buffer-overflow-vulnerability-in-juicebox-40-smart-ev-charging-station).

So Juice Rescue is deciding what to take on next. We have a fiscal sponsor who can process donations, volunteers who are excited to work with code and/or documentation, and many people who have offered to test out solutions.

Our goal is to keep running and keep out of the landfill as many of the [120,000+ North American JuiceBoxes](https://www.consumerreports.org/cars/hybrids-evs/enel-x-way-closing-what-to-do-if-you-own-a-juicebox-charger-a1912800096/) as possible, while also taking steps that would be useful to people in other countries should Enel X Way abandon you too.

Before agreeing on our next steps or taking any donations, we want to choose a direction that works for the greatest number of people. So we have three possible directions that we want your feedback on:

* Helping people **replace the internal (insecure) controller board** with a $99 open hardware [OpenEVSE board](https://www.openevse.com/about-us.html) ([JuiceBox v1](https://openevse.dozuki.com/Guide/Replace+Controller+in+Juicebox+v1/52)) ([JuiceBox v2](https://openevse.dozuki.com/Guide/Replace+Controller+in+Juicebox+v2/53)). OpenEVSE already have prototype boards sent out to community members for testing and expect to have replacements in Q1. With OpenEVSE, people can [log into the charger from the web](https://openevse.stoplight.io/docs/openevse-wifi-v4/3e38d9ead39fc-user-guide) or use other software like Home Assistant.
  * This path would focus on collective organizing to help each other actually replace the controllers, and improvements to existing management software.  
* **Improving the [Juicepassproxy](https://github.com/JuiceRescue/juicepassproxy) software** and supporting people to keep their JuiceBoxes running on the existing software/hardware.
  * This path would require some rewriting of the current code, as well as substantial work to create documentation and setup guides for the many different versions of the Juicebox hardware and software.  
* Organizing an **exchange network** or guide for anyone who just wants to **redistribute** or **recycle** the charger they have (in concert with the above options)

Please [**Complete the Survey here by January 10th**](https://docs.google.com/forms/d/e/1FAIpQLSebxh9e52KvGheKCdoS5xvhGZG3nvG90iy_DJqezTTkjlV2WQ/viewform?usp=dialog) so we can review the results and follow up.

---

To provide more detail on the options, here's a comparison. It's important to note Juicepassproxy relies on third-party software such as Home Assistant to make these features visible and usable. OpenEVSE offers more options, including a built-in web interface, a [Home Assistant](https://www.home-assistant.io/) instance running on your home network, or a third-party backend using the [OCPP protocol](https://openchargealliance.org/protocols/open-charge-point-protocol/) (for multiple chargers).

|  | Original JuiceNet App | Enel X Way App | OpenEVSE Controller | Juicepass proxy |
| :---- | ----- | ----- | ----- | ----- |
| Home Assistant Compatible | ✅ | ⛔ | ✅ | ✅ |
| Record usage data | ✅ | ✅ | ✅ (slightly less accurately) | ✅ |
| Control power levels | ✅ | ✅ | ✅ | ✅ |
| Control charging schedules | ✅ | ✅ | ✅ | ✅ |
| Off-peak charging | (unsure) | ✅ | ✅ (with the scheduler or third party data) | ✅ |
| Managing multiple chargers in one interface | ✅ | ✅ | (it depends on the software you use) | ⛔ |
| Load balancing multiple chargers | ✅ | ⛔ | 🟡 (with third party software like Home Assistant or Node-Red) | ⛔ (could be added) |

## Comparing OpenEVSE and JuicepassProxy

Here is a comparison of the OpenEVSE and Juicepassproxy options :

|  | OpenEVSE | Juicepassproxy |
| :---- | ----- | ----- |
| **Installation** | 1\. Open the box &  replace the controller. The board uses the same  connectors as the original board 2.Connect to WiFi and other services as needed ([Install Guides](https://openevse.dozuki.com/c/JuiceBox)) | 1\. Re-configure your home network 2\. Set up the Docker system on an always-on computer, which may be the same computer as a pre-existing Home Assistant server 3\. Install and configure Juicepassproxy 4\. Connect to Home Assistant |
| **Cost** | $99. | No cost. |
| **Usability and ease of setup** | Once the new controller is in place, working with the software is simple and straightforward. You do need to be willing to open the box, able to use a screwdriver, and plug cables into the new controller. | No need to open the box. You need to be willing to learn how your network works, re-configure the DNS system, and do occasional diagnosis/adjustments. You also need to be able to install and run Python code on an always-on computer and do occasional diagnostics.  |
| **Universality** | Most JuiceBoxes should be covered with the two controlled boards that have been prototyped without any modification. | Many different versions of the firmware and hardware make it difficult to provide reliable, universally-workable steps without a broad effort at shared documentation. |
| **Longevity** | Firmware and security updates provided across the OpenEVSE ecosystem. All design files and source code have been published. | The network configuration could require ongoing tweaks at unexpected times No future firmware or security updates available from Enel X Wa.y |
| **UL**  | Voids UL certification | Voids UL certification |
| **Ongoing support** | A strong [OpenEVSE Support network](https://openev.freshdesk.com/support/home). Open source board [design files](https://github.com/OpenEVSE/JuiceRescueController) Firmware for [the Controller](https://github.com/OpenEVSE/open_evse) and [WiFi](https://github.com/OpenEVSE/openevse_esp32_firmware) is unmodified from standard OpenEVSE & published on Github. | If enough people in the Juice Rescue community is interested in providing support, we can organize it. |

Thanks everyone\!

\-- Juice Rescue Team
