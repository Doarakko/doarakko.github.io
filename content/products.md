# Products

## [iyashi](https://github.com/Doarakko/iyashi)

"iyashi" is a slack bot that randomly returns the pictures of animals you posted.

When you post a picture of an animal, it will be automatically classified and registered.

[![iyashi sample](/img/iyashi-sample.gif)](https://github.com/Doarakko/iyashi)

## [go-yugioh](https://github.com/Doarakko/go-yugioh)

Go library for accessing the [Yu-Gi-Oh! API by YGOPRODeck](https://db.ygoprodeck.com/api-guide/).

[![go yugioh github](/img/go-yugioh-github.png)](https://github.com/Doarakko/go-yugioh)

```go
import (
	"fmt"

	"github.com/Doarakko/go-yugioh/yugioh"
)

func main() {
	client := yugioh.NewClient()
	cards, _, _ := client.Cards.List(
		&yugioh.CardsListOptions{
			KeyWord: "dragon", Type: "Fusion Monster", Attribute: "light"})

	for _, card := range cards {
		fmt.Printf("Name: %v\nType: %v\nRace: %v\nDescription:\n%v\n\n",
			card.Name, card.Type, card.Race, card.Description)
	}
}
```

```
Name: A-to-Z-Dragon Buster Cannon
Type: Fusion Monster
Race: Machine
Description:
"ABC-Dragon Buster" + "XYZ-Dragon Cannon"
Must be Special Summoned (from your Extra Deck) by banishing cards you control with the above original names, and cannot be Special Summoned by other ways. (You do not use "Polymerization".) During either player's turn, when your opponent activates a Spell/Trap Card, or monster effect: You can discard 1 card; negate the activation, and if you do, destroy that card. During either player's turn: You can banish this card, then target 1 each of your banished "ABC-Dragon Buster", and "XYZ-Dragon Cannon"; Special Summon them.

Name: ABC-Dragon Buster
Type: Fusion Monster
Race: Machine
Description:
"A-Assault Core" + "B-Buster Drake" + "C-Crush Wyvern"
Must first be Special Summoned (from your Extra Deck) by banishing the above cards you control and/or from your Graveyard. (You do not use "Polymerization".) Once per turn, during either player's turn: You can discard 1 card, then target 1 card on the field; banish it. During your opponent's turn: You can Tribute this card, then target 3 of your banished LIGHT Machine-Type Union monsters with different names; Special Summon them (this is a Quick Effect).
...
```

## [draw](https://github.com/Doarakko/draw)

Draw Yu-Gi-Oh! Card.

[![draw sample](/img/draw-sample.gif)](https://github.com/Doarakko/draw)

## [Otoko Banzuke](https://otoko-banzuke.herokuapp.com)

Search Otoko from YouTube comments, and make banzuke based on comment like count.

[![Otoko Banzuke sample](/img/otoko-banzuke-sample.jpg)](https://otoko-banzuke.herokuapp.com)

## [bigburger](https://github.com/Doarakko/bigburger)

bigburger is command line tool displayed big burger with toppings.

[![bigburger sample](/img/bigburger-sample.gif)](https://github.com/Doarakko/bigburger)

## [Kagoole](https://kagoole.herokuapp.com)

Search [Kaggle](https://kaggle.com) competitions and solutions based on data and predict type, evaluation metric, etc.

[![Kagoole sample](/img/kagoole-sample.jpg)](https://kagoole.herokuapp.com)

## [Kaggle Calendar](https://kaggle-calendar.herokuapp.com)

[Kaggle](https://kaggle.com) google calendar by data type.

[![Kaggle Calendar sample](/img/kaggle-calendar-sample.jpg)](https://kaggle-calendar.herokuapp.com)

## [Kaggle Kernel Notification](https://github.com/Doarakko/kaggle-kernel-notification)

Notify new [Kaggle](https://kaggle.com) kernels to Slack or LINE without coding.

[![Kaggle Kernel Notification sample](/img/kaggle-kernel-notification-sample.jpg)](<(https://github.com/Doarakko/kaggle-kernel-notification)>)

## [Kaggle Competition Notification](https://github.com/Doarakko/kaggle-competition-notification)

Notify new [Kaggle](https://kaggle.com) competition to Slack or LINE without coding.

[![Kaggle Competition Notification sample](/img/kaggle-competition-notification-sample.jpg)](https://github.com/Doarakko/kaggle-competition-notification)
