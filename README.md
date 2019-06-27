# Lab6 Poker
This is the completed lab for Lab #5.  This lab has the PokerHub handing the HubPokerTable object.

In this lab, I want you to start the new game.  
*	The Start button in PokerTable.fxml will fire method btnStart_Click().  This method will create an Action instance of GamePlay, figure out the rule that’s selected in the menu and request a game to be started.  All of this is done for you.
*	The Action is sent from the controller to the mainApp and to the hub.  All of this is done for you.
*	The Action is being received by the hub, and the code is set for you to work.  Check out **** case StartGame: **** in PokerHub.  You’re going to have to set the HubGamePlay to a new instance of GamePlay(), set the deck, pick the dealer and then…  
*	Deal the first set of cards.  Notice I’m using switch/case, but NOT breaking after the Start.  This means the code will fall through from Start to Deal.  I want the first cards drawn based on the game’s ruleset.
*	Draw the cards to the right player(s) and/or the community hand.  Finally, make sure you set eDrawCountLast so the client knows which card to paint in JavaFX
*	Send back the HubGamePlay to the client.
*	This client will execute method: Handle_GameState
*	Code method Handle_GameState to push the right cards to the right player, making sure to keep track of which card is face up, which is face down.
