# Juice Rescue ⚡🔌🚗

Do you own a Juicebox charger? Has your organization, power company, or government energy board developed arrangements with consumers that rely on the JuiceBox? Are you frustrated and worried that [Enel X Way shut down its North American operations](https://www.juiceboxnorthamerica.com/), including key software the chargers rely on?

**Update August 24, 2025**: From October 2024 - August 2025, the Juice Rescue community brought together hundreds of owners of Juiceboxes to organize to keep our vehicles charged.

You can read the full story of this group here: [Escaping the chains of tethered products: the Juice Rescue project ](https://natematias.com/portfolio/2025-08-22-unchaining-from-broken-software-tethers/).

This page is now an archive of those efforts. Since the last update, we:

* Organized [a Discord channel](https://discord.gg/JcZr6RSKE3) (still available, though with less activity) to coordinate
* Supported many people to get data out of their Juiceboxes, with the [Juicepassproxy software](https://github.com/JuiceRescue/juicepassproxy)
* Surveyed people and collaborated to get people access to software fixes, as well as supported a successful open hardware effort by OpenEVSE. If you still need to fix your Juicebox, your best option is to replace the board with one from OpenEVSE, available here:
 * [Juicebox V2 replacement board](https://store.openevse.com/products/replacement-electronics-for-juicebox-v2-plastic-grey-and-white?srsltid=AfmBOopa1qkZpI3o8O6fTkRLA9b2WhkBtwWRB51iKcAUMNWw9MzYKbpS)
 * [Juicebox V1 replacement board](https://store.openevse.com/products/replacement-electronics-for-juicebox-v1-metal-black-and-orange?srsltid=AfmBOopOxw8iy3Nij97i6MbjodzHQBIhe5625OUXm3x0lghd4hE9-oxt)
* Developed an entity that could take on donations and pay for this, though this turned out not to be needed (thanks everyone!)

<div align="center"><hr style="width:50%"/></div>

**Update Oct 9 2024**: We have compiled a [short PDF guide on Preparing for Enel X Way's Abandonment of JuiceBox EV Charging Software](documents/2024-10-09-preparing-for-enel-x-juicebox-software-abandonment.pdf)

**Update Oct 10 2024**: Contributors to Juice Rescue have worked with Consumer Reports to send a letter to the U.S. Federal Trade Commission urging. Here are two quotes from the longer [letter asking the FTC to investigate the behavior of Enel X](documents/2024-10-10-Juicebox-letter-to-FTC.pdf). And here's 
* "The decision to stop supporting the app that thousands of consumers use to control the charger and the complete loss of functionality for the commercial EV chargers represents an egregious example of how companies are controlling the functionality of a product even after the consumer has purchased the device."
* Here's the story on the CR site: [Consumer Reports, U.S. PIRG, and 60 self-reported owners of JuiceBox EV chargers call on the FTC to investigate Enel X after abruptly discontinuing sales and support of its EV chargers](https://advocacy.consumerreports.org/research/consumer-reports-u-s-pirg-and-60-self-reported-owners-of-juicebox-ev-chargers-call-on-the-ftc-to-investigate-enel-x-after-abruptly-discontinuing-sales-and-support-of-its-ev-chargers/). We are deeply grateful for everyone at the CR team for working with us so quickly to establish the facts collaborate on a productive path with federal regulators.

## How we're keeping JuiceBoxes running

Now that Enel X is shutting down key infrastructure for these devices, Juice Rescue is organizing a collective effort aimed at keeping JuiceBoxes running with full functionality:

* Educating people about how to safely keep charging with your JuiceBox charger
* Organizing technology development on projects like [Juicepassproxy](https://github.com/JuiceRescue/juicepassproxy) that can replace some of the functionality that will be lost once Enel X shuts down
* Coordinating efforts across customers and clients of Enel X to:
  * Advocate that Enel X release JuiceBox-related intellectual property and source code, allowing customers to keep the chargers' full functionality
  * Direct public pressure, policy, and legal strategies that could help Enel X meet its promises to customers/clients, and its obligations under the law, including [right to repair](https://en.wikipedia.org/wiki/Right_to_repair) laws

## JuiceBox FAQ

**Will my JuiceBox shut down on October 11?** *Residential JuiceBoxes will continue to charge fine, even after Enel X shuts down their infrastructure.* However, after this day, users won't be able to change the settings, monitor charging, schedule or initiate charging, because these functions are dependent on Enel X's network and app. Commercial users and those with special deals with power companies, on the other hand, may not be able to charge at all; they should contact their commercial operator or power company with questions.

**Will my JuiceBox become a fire hazard?** Probably not. But if your circuit breaker and wiring are not properly matched (i.e., sized too low) to the output of your JuiceBox, then you should make sure to configure the charger and lower the maximum output before October 11. Otherwise the charger may draw more amps than your system can provide, which could either trip your breaker or become a fire hazard. efforts like [Juicepassproxy](https://github.com/JuiceRescue/juicepassproxy) should eventually make it easier for users to modify these settings even after Enel X shuts down.

**Can I connect my JuiceBox to other systems like Home Assistant?** Yes. The [Juicepassproxy](https://github.com/JuiceRescue/juicepassproxy) project allows someone with technical skills to get data out of the JuiceBox. We are working to make this software more functional and easier to set up with Home Assistant and other systems.

## About us
Juice Rescue is organized by a group of people who own JuiceBoxes or whose organizations rely on them. If you have questions about the group, please [join the Discord server](https://discord.gg/rBgbGZsA) and ask. The Discord conversation includes:

* Residential JuiceBox owners who want to continue to monitor and manage their EV chargers over the network
* A co-op in upstate New York that has 43 chargers
* Internet of Things developers with experience working with EV charging systems
* Organizers with experience in relevant intellectual property issues and federal/state regulations

<!-- - Dr. [J. Nathan Matias](https://natematias.com/), on the tech team at the Ithaca Ecovillage, a community that uses 43 JuiceBox chargers   
- (other organizers add your name and/or username here) -->
