# dc4bc-conference-call

This repository is used by dc4bc participants to communicate with each other in order to start DKG rounds. The procedure is as follows:

1. Somebody creates a new file `dc4bc-conference-call-22-10-2020` with the following structure:
```
{
  "SigningThreshold": 1,
  "Participants": [
    {
    "Addr": "addr1",
    "PubKey": "Otwt+xeI7Po3aNIcLWugnMIHxWcoTPnI3kylUkIFq80=",
    "DkgPubKey": "icmEgjz+F/W6qC347pIvu317GOZA7vj4cthe/+6+GtTvh4hng0C6yx40f7RTKcNuCe+xUATI2dNEciyx7ntUaAzBOuuzRuYmOIYjBTFmt8Zms/9K1EVMhXm0zGFb5rfP"
    }
  ]
}
```
2. Other participants open pull-requests with their data, appending to the list of `Participants`;
3. When everything is ready, the contents of this file are used as input for the StartDKG procedure by one of the participants.

*N.B.: for more information about getting the data for this procedure please visit https://github.com/depools/dc4bc/blob/master/HowTo.md*
