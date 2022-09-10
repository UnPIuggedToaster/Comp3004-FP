# COMP3004Final

Author: 
Hassan Allam 


Submission Structure:

COMP3004Final-main -> 

    team35 -> 

        -- A collection of png's used for the GUI 
        icon -> 
            icons_off 
            icons_on
        progress 

        -- Database class that holds the session history as a QVector of QStringLists
        db.cpp 
        db.h 

        images_resource.qrc

        -- QT C++ generated main class
        main.cpp
        main.h

        -- QT C++ mainwindow function, bulk of the code logic is based in mainwindow.cpp
        mainwindow.ui 
        mainwindow.h
        mainwindow.cpp

        team35.pro 

    .gitignore 

    -- sequence diagram pdf 
    sequenceDiagram.pdf 

    -- pdf containing the traceability matrix, state diagram, acitivity diagram, and use cases 
    Traceability-state-activity-useCase_diagram.pdf 

    -- the UML diagram 
    umlDiagram.pdf

Tested Scenarios

Scenario's that passed

    - User trying to turn on the batter at 0 % 
    - User removing ear connection and/or ces connection during session selection/sessions
    - Battery running out during session time 
    - Interuptting soft off resets the timer 
    - User changing intensity during session 
    - Changing intensity during session time while recording saves the last intensity set 
    - User cannot connect CES module or Ear clips while device is powered on
    - User can power off the machine during a session
    - Machine powers off after 30 seconds if the user fails to confirm a session time/session length 

Scenario's that failed

    - User cannot select a session from their history if there is only 1 session to select from 
