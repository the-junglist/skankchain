# skankchain

The TallyWhacker™ Powered by SkankChain™
Introducing The TallyWhacker™
Powered by SkankChain™

A digital tab reckoner and bullshit interceptor for hospitality outposts.

What is it?
A hybrid POS subsystem that logs, flags, and settles transactions with the precision of Yai Ooan’s biro and the cold indifference of terminal code.

Whether it’s a half-paid incense-for-smoothie exchange or a beer lifted from the fridge during a spiritual monologue, TallyWhacker sees all.

Features:
Real-Time Skank Scanning
ts
Copy
Edit
if (customer.vibe === "Yogi Begger" && payment.intent === "mystic") {
  TallyWhacker.warn("Skank Risk Level: HIGH");
}
Tab Drift Tracker
Visualizes unpaid items over time

Highlights ghost items Dave swears he never ordered

ts
Copy
Edit
tab.add({ item: "Banana Smoothie", price: 65, delivery: "Beach Drop" });
tab.trackDrift("smoothie", +3); // suspicious
Karmic Credit Limit™
A floating max tab threshold calculated by behavior, last payment, and the "Did they do the dishes?" factor.

ts
Copy
Edit
karmicCredit.calculate({
  partialPayments: [60],
  fridgeRaids: 2,
  unsolicitedGuitarSolos: true,
});
Terminal-Style Receipt Generator
Sample Output:

yaml
Copy
Edit
┌──────── TallyWhacker™ Receipt ────────┐
│ Customer: dave_vagabond               │
│ Items:                                │
│ - Mung Thing ................. ฿90     │
│ - Leo Beer (visual theft) .... ฿50     │
│ - Smoothie (beach drop) ...... ฿65     │
│ Extras:                               │
│ - Motorbike (7d) ............. ฿1400   │
│ - Scratch Fee ................. ฿500   │
│ Partial Payment .............. -฿60    │
│ 🧾 Total Due: .................. ฿2045  │
└───────────────────────────────────────┘
Optional Modules:
SkankChain Watchdog™: AI flagging for repeat freeloaders, spiritually evasive language, and tab split trickery.

FridgeCam Integration: Auto-log unauthorized grabs via motion trigger. Dave: “I was blessing the Leo!”

Lore Mode: Animate Dave’s crimes in comic cutscene format, suitable for staff training or vibe control.

Tagline:
The TallyWhacker™ –
“Every tab told. Every skank logged.”

[01:25, 15/07/2025] Nathan: 🎭 BOB POS: DaveWatch™ – Episode I
“The Unslippery Ledger of Yai Ooan”
Powered by SkankChain™

🛖 Scene:
A breezy bamboo guesthouse-café on a Thai island. Sand. Motorbikes. Hammocks.
Enter: Slippery Dave — skin sun-worn, eyes enlightened, wallet suspiciously light.

📍1. Arrival
[Yai Ooan, hunched over her ledger with a biro and a seventh sense for BS, senses a disturbance. Dave enters through the open front.]

Yai Ooan (internal log, in Thai):

“ไอ้เหี้ยมาอีกละ... Wanker.”
(Translation: The f**kwit returns.)

[OrderSession logs: visitTimestamp, customerID: dave_vagabond, sessionStart: now()]

📍2. His Glorious Return from Argentina
Dave:

“Yai! I’m back! Argentina was epic. Stayed with some friends, taught them how to live more freely. Gave them some ideas, you know?”

Yai Ooan (deadpan):

“Very generous of you.”

[Note added: dave.selfReported: unpaid_stay += 1]

📍3. The Order Begins
Dave:

“Can I get a Coke? And... you got that mung bean curry still?”

[SkankChain logs:
orderSession.items.push({ item: "Coca-Cola", price: 25 })
orderSession.items.push({ item: "Crusty Vegan Mung Thing", price: 90 })]

📍4. Side Deal with the Gardener
[Dave makes eye contact with the gardener, nods knowingly]

Dave (low voice):

“Oi, can you... y’know, add a lil’ green to my tab?”

[SkankChain logs:
orderSession.items.push({ item: "Herbal Supplement", price: 150, source: "gardener" })]

📍5. Beach Banana Smoothie Flex
[Dave walks by the waitress, doesn't break stride]

Dave:

“Smoothie banana, yeah? Just bring it down to the driftwood bench.”

[SkankChain logs:
orderSession.items.push({ item: "Banana Smoothie", price: 65, delivery: "Beach Drop" })]

📍6. Fridge Grab Stealth Attempt
[Dave casually opens the drinks fridge, grabs a Leo, gives a lazy “I got this” wave to Ooan while she’s talking to Germans about rice portions.]

Yai Ooan (still facing away, eyes squinted):

“One beer. Logged.”

[SkankChain logs:
orderSession.items.push({ item: "Leo Beer (Self-Service)", price: 50, method: "Visual Theft Intercept" })]

📍7. Tab Negotiations
Yai Ooan:

“Want a tally? Can settle at the end of the week.”

Dave:

“Err, yeah, no, not yet... Western Union’s being weird. I’ve got... here—”

[Dave pulls out 60 Baht in coins and a half-used incense stick.]

Yai Ooan (logging silently):

tabPartialPayment: 60

📍8. The Reckoning
[Dave finally requests his tab after a week of skanking.]

Dave (squinting at the paper):

“Wait, I don’t remember ordering that many smoothies... oh wait, yeah... yeah, no that was me.”

Yai Ooan (without looking up):

“Also: bike rental, 200 per day. Seven days.
500 Baht scratch fine. Gardener saw.”

[SkankChain logs:
session.extras.push({ item: "Motorbike Rental (7 days)", total: 1400 })
session.extras.push({ item: "Scratch Fee", price: 500, witness: "gardener" })]

📍9. Final Total:
json
Copy
Edit
{
  "customer": "dave_vagabond",
  "items": [
    { "item": "Coca-Cola", "price": 25 },
    { "item": "Crusty Vegan Mung Thing", "price": 90 },
    { "item": "Herbal Supplement", "price": 150 },
    { "item": "Banana Smoothie", "price": 65 },
    { "item": "Leo Beer", "price": 50 }
  ],
  "extras": [
    { "item": "Motorbike Rental (7 days)", "price": 1400 },
    { "item": "Scratch Fee", "price": 500 }
  ],
  "partialPayments": [60],
  "totalDue": 2220,
  "status": "Pending Payment"
}
[01:39, 15/07/2025] Nathan: SkankChain™ Lore Entry:
ts
Copy
Edit
export const skankDuo = {
  groupName: "Yogi Begger & Poo Poo",
  knownCrimes: [
    "Buffet loitering",
    "Incense-for-smoothie bartering",
    "Borrowed towel never returned",
    "Spiritual mansplaining"
  ],
  tabBehavior: {
    method: "Drift and Deny",
    maxTabBeforeEviction: 235,
    currentBalance: 187.5,
    notes: "Last seen near the hammock tree, quoting Rumi incorrectly"
  },
  quotes: [
    "You can't put a price on energy.",
    "Money is an illusion. But do you validate Western Union?",
    "Poo Poo doesn't eat the food... he blesses it."
  ]
}
