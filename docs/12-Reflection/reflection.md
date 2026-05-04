---
title: Reflection
---

## Review of Module's Sucess

The Gyroscope module was largely successful. The basic requirements for the project and concept were met where the PCB was built with primarily surface mount components, the microcontroller can execute code, it can read and send sensor data to the correct recipients, and the module can be powered both individually and in connection with the other boards. The one goal that I was unable to fulfill with this module was being able to accurately read speed from the accelerometer data. I had intended to implement a Kalman Filter to offset the gravity readings but was unable to within the project's time constraints. Aside from this, however, the module fulfills its primary function and is able to accurately read data, quickly send its data to the other boards, and correctly act upon the messages that it receives.

## Module Startup Tips

There were mutliple parts of the project I struggled with but was able to overcome: 

- One issue that I had was that many of the course's setup and coding guides for the ESP32-S3 were outdated, so I had to work around that through researching and working with my group. If you are using the ESP32 over the PIC, I recommend using the guides available on the internet instead.
- I also had to switch groups early on in the project due to being burdened with a larger share of the work, so trying to catch up to my new group made it difficult to take the time to flesh out the concept for my module, though it did work out in the end. I would recommend paying extra attention when picking a group for this semester.
- Micropython in Pymakr caused many issues for my group members and myself, so, if using the ESP32, I would also recommend switching over to C in the Arduino IDE for the project given that the ESP32 is primarily designed to be used with this software.
- There are many other niche issues that I experienced throughout the project, such as having to enable the USB CDC setting in Arduino to see my serial monitor but then having to disable it for the code to work dependent of the IDE, a quirk I have never experienced with the IDE despite having used it several times before. This project is likely new territory for most students, so, again, be sure to research solutions and don't give up. 

## Lessons Learned

1. Do not rush through reviewing datasheets of components, you may make a mistake in designing your PCB layout.
2. Start testing full code as soon as possible to ensure all aspects of the module are in order.
3. Test with other modules as soon as possible to ensure all aspects of communication and message structure are in order.
4. Start planning out and building the housing for the project as soon as possible, there will not be enough time to make a proper one if it is left for last.
5. Thoroughly document all successful tests for the project, it will help in case something stops working.
6. Order extra parts not only for the individual module but for the whole team in case components break, go missing, or there isn't enough for everyone.
7. Review and re-review assignments and deliverables, it is easy to miss something and get points off because there is so much to do.
8. Meet with the team outside of class, this allows for longer and more thorough testing sessions between the modules.
9. 
10. 

## Recommendations for Future Students

1. Do your research, your project will end up better if you are thorough when choosing the project concept and which major components to use.
2. In order to prepare for capstone, challenge yourself and do not settle for the bare minimum because it likely will not be enough for next year.
3. Talk to the professor or TAs when you need help, their experience will likely guide you to better solutions and help you fix your problems faster. 
4. Choose your group wisely, otherwise you may be building a project you don't want to build or doing a large amount of the work.
5. Do not be afraid to rely on your group, their help and feedback may help make the project and your module better than if you had done it solo.
