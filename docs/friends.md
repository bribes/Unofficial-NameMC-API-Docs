# NameMC Friends API docs
NameMC has their own system for caching capes.

This API's purpose is to get all capes a user owns according to NameMC.

### `GET https://api.namemc.com/profile/UUID_Here/friends`
This is the only endpoint for this API.

Parameters are as follows:
- **`UUID_Here`** - the UUID of the account

### Possible responses

The API will almost always return HTTP status code `200 OK` and set its `Content-Type` header to `application/json`.

If the user you provide doesn't exist, the API will return HTTP status code `404 Not Found`, and the `Content-Type` header will remain `application/json`.

Here are the different responses that can be returned:

**Returns the Users Friends / HTTP `200`:**
```json
[
  {
    "uuid": "a909a57d-feff-4801-accd-f09e19a05d28",
    "name": "000000000000000h"
  },
  {
    "uuid": "f438f9dd-268d-49f4-9b5c-6af88c1613f0",
    "name": "000000000000000_"
  },
  {
    "uuid": "66b49ddd-bf8c-474f-b561-ed07f1058949",
    "name": "000Blaser"
  },
  {
    "uuid": "0d02b245-e4e9-4b3f-b900-7f7ba7747664",
    "name": "000x0a0n0a0x000"
  },
  {
    "uuid": "1718289f-9156-442f-9fc4-a10ee76e8158",
    "name": "0ffExplicita"
  },
  {
    "uuid": "88223b94-e347-4261-b80e-d0650a54f316",
    "name": "0h69"
  },
  {
    "uuid": "de30afae-442c-4ad8-a7bd-eef50faf1dc8",
    "name": "0hDxddy"
  },
  {
    "uuid": "51d2d573-797d-4db4-b36b-676236c3ed5d",
    "name": "0hZhaping"
  },
  {
    "uuid": "9f184bd4-9a2f-4918-aa11-698063fd5310",
    "name": "0KAYAMA"
  },
  {
    "uuid": "d9a78c9c-18a1-48fe-8287-2bb2a296905f",
    "name": "0nlyAquaa"
  },
  {
    "uuid": "7a724c60-773c-4667-b77c-84cecdcf31f9",
    "name": "0UTLOVE"
  },
  {
    "uuid": "2f82b125-fe56-4481-9446-132b585844c3",
    "name": "0YJ"
  },
  {
    "uuid": "171b2907-f8b1-4eac-b870-d3d287f24945",
    "name": "0zb"
  },
  {
    "uuid": "687ad06c-0bf1-4aa4-af9e-49d97f4104b7",
    "name": "123"
  },
  {
    "uuid": "2fb7c8ff-f698-4f60-b1ee-7f7c580b8ff9",
    "name": "123123"
  },
  {
    "uuid": "c0ddfccf-4ade-4e7a-8e47-226b89b2cfe9",
    "name": "15Z"
  },
  {
    "uuid": "b43b7e5e-5990-41e8-ab48-b50de8859119",
    "name": "162"
  },
  {
    "uuid": "09fd634e-6c55-42ef-95c7-646f3e853d52",
    "name": "1z1"
  },
  {
    "uuid": "7efcb353-05a0-4c00-ab8e-a067cb153e41",
    "name": "1____3____3____7"
  },
  {
    "uuid": "87bb7f82-d948-4b30-a76a-10ee48e182bd",
    "name": "2ehz"
  },
  {
    "uuid": "94618e23-0fdf-4904-b4a8-b11b63643cdd",
    "name": "3lu"
  },
  {
    "uuid": "1766206e-a906-4300-91e9-ce4f01eb94a4",
    "name": "3MFrench"
  },
  {
    "uuid": "3b4d5283-42c8-42a9-bd65-5cc16183780d",
    "name": "3rst"
  },
  {
    "uuid": "fb6737d1-46af-4891-b189-18d189546876",
    "name": "420Sadica"
  },
  {
    "uuid": "ef594374-d957-41ac-a605-dde936bc2da4",
    "name": "450"
  },
  {
    "uuid": "befac8a2-f41c-4155-be29-91ea670c6025",
    "name": "4saken"
  },
  {
    "uuid": "c186d379-929c-4f68-b654-7b7e01fc4bbc",
    "name": "5nt"
  },
  {
    "uuid": "c985d41c-6cc8-4648-8746-f14eb8da9a28",
    "name": "5ny"
  },
  {
    "uuid": "96d79830-450d-453a-9126-2b8384e3da4e",
    "name": "6ha"
  },
  {
    "uuid": "6a55de7e-300b-4919-a4e1-abbcdf8fe4fe",
    "name": "8394"
  },
  {
    "uuid": "514d7cb8-4836-4650-840a-01318deb02de",
    "name": "9w4"
  },
  {
    "uuid": "9bd5fcba-8fb1-484c-89ef-9d9133139954",
    "name": "ADASTRAA"
  },
  {
    "uuid": "65de51aa-b4d5-48d3-91f0-770bd4264347",
    "name": "Addiction"
  },
  {
    "uuid": "17cc54dc-1987-4162-9aa3-59e3b0a2531a",
    "name": "AdminSeries"
  },
  {
    "uuid": "8e153bdc-dd60-47dc-add4-a264c3fb810b",
    "name": "Adult"
  },
  {
    "uuid": "8bb6cf92-4997-4f12-946e-10b8c936256d",
    "name": "Adventure"
  },
  {
    "uuid": "3712fe8c-e768-4b8a-8dd9-c340996faae7",
    "name": "Aedine"
  },
  {
    "uuid": "e4d551e2-c06a-4654-9e04-117e942160c4",
    "name": "Aering"
  },
  {
    "uuid": "dc34e39a-98ee-442a-8c58-4b3e3ce0d7ce",
    "name": "Afford"
  },
  {
    "uuid": "1f095c8a-5bb0-4d56-ba51-61b31cc1b058",
    "name": "AHHHHHHHHHH"
  },
  {
    "uuid": "ef333548-0fc0-413e-a555-4ef5e64afec4",
    "name": "Aimina"
  },
  {
    "uuid": "77966ca3-ac85-44b2-bcb0-b7c5f9342e86",
    "name": "Akhali"
  },
  {
    "uuid": "da4b4851-7d76-4c87-ab74-495239c7a984",
    "name": "Altaria"
  },
  {
    "uuid": "041c251e-9894-43f1-b8b9-83f02180b3af",
    "name": "Amigo"
  },
  {
    "uuid": "2d4742ef-8193-454e-8b57-8cd2e85e7a4c",
    "name": "angehlic"
  },
  {
    "uuid": "ad0eba26-e002-493b-8bbd-cc09f6adfae1",
    "name": "Annual"
  },
  {
    "uuid": "dc66cd17-b299-4e6c-8001-8a8662d0b353",
    "name": "Antagonised"
  },
  {
    "uuid": "d6c6f1a6-5f34-4a0d-9fa7-26c31471b715",
    "name": "antcine"
  },
  {
    "uuid": "0f996d51-a75a-424e-b87d-54a2a78c93f3",
    "name": "areumadlol"
  },
  {
    "uuid": "901878ed-2690-420d-811c-93983dd10e76",
    "name": "Arson"
  },
  {
    "uuid": "4456ab5f-9042-4c5a-95ef-63e0c669b802",
    "name": "Aseia"
  },
  {
    "uuid": "f669b484-cc85-455f-8ca9-8f3bc51056c8",
    "name": "Asiel"
  },
  {
    "uuid": "cc8093a2-4f14-4030-8c21-644eae7f25ce",
    "name": "Asira"
  },
  {
    "uuid": "b143b358-e068-4dfa-b292-0b417d01b2db",
    "name": "Ask"
  },
  {
    "uuid": "630aa72a-9bd4-4f86-9c9e-dc095a9d1afe",
    "name": "auctioneers"
  },
  {
    "uuid": "c4f90dd1-a7ef-4d45-ba0d-3fc02f524e91",
    "name": "Autvmn"
  },
  {
    "uuid": "17bede05-00ab-41a2-a672-1aa016202a8a",
    "name": "AveryDE"
  },
  {
    "uuid": "a9ffd2dc-8f52-4aa9-bc7f-83fdef5665b4",
    "name": "Ayear"
  },
  {
    "uuid": "6a55170b-1568-45ac-aea1-9e7f2750822f",
    "name": "Ayk"
  },
  {
    "uuid": "ad2f8c98-fa5e-4345-9e1d-3e69b7f2f3b3",
    "name": "B4FFY"
  },
  {
    "uuid": "a1bad206-ed9d-4422-b660-18ee317a0ddb",
    "name": "baaddies"
  },
  {
    "uuid": "8a753f2b-77fa-4e34-9f6f-4c2697661151",
    "name": "Bag"
  },
  {
    "uuid": "107cd08e-0933-443a-841d-ad474c1dd0c7",
    "name": "baiIey"
  },
  {
    "uuid": "14f19f50-50cb-44cd-9f0b-be906ad59753",
    "name": "Bar"
  },
  {
    "uuid": "ded481bd-27d3-4af6-a38e-c013fa2f9750",
    "name": "Bay"
  },
  {
    "uuid": "fbc2dc18-43cb-438a-b4e6-66dbad0e9e8c",
    "name": "bb"
  },
  {
    "uuid": "025c8cd1-685d-4407-bd4d-41d4184af6dd",
    "name": "bctch"
  },
  {
    "uuid": "2504768b-04f6-4f49-a269-caef6e9c9063",
    "name": "BedLost"
  },
  {
    "uuid": "82356da7-cf5e-481c-a7f4-f3d32aae18de",
    "name": "Begins"
  },
  {
    "uuid": "c25f4eef-82ef-426c-b54a-ba412fc695fc",
    "name": "benscn"
  },
  {
    "uuid": "9610a584-ac44-40b3-be3f-8d5a561ecc6e",
    "name": "bestpp7"
  },
  {
    "uuid": "dd71195f-9b72-4205-8ead-675992b9702b",
    "name": "BestSellings"
  },
  {
    "uuid": "a91063a3-56c1-46be-bbe7-c3f5412d1c57",
    "name": "BetaTests"
  },
  {
    "uuid": "861e3cb8-0e2e-4f53-a50f-fbd5356fa8c0",
    "name": "billyK_"
  },
  {
    "uuid": "d031dd67-7d8b-451a-b820-e447b983e1ae",
    "name": "bixo"
  },
  {
    "uuid": "818d58ea-b064-4c4d-8528-f4da546c2613",
    "name": "Boludin"
  },
  {
    "uuid": "37e82686-a1e9-4a48-9301-c2d21d55c8ff",
    "name": "Bozo"
  },
  {
    "uuid": "e1afe168-24fe-4ea1-bcf3-24913ce80d36",
    "name": "Brancher"
  },
  {
    "uuid": "d61efec3-4fe8-4fbb-8de3-e139f8deebcf",
    "name": "Brutal"
  },
  {
    "uuid": "95d847c3-33a2-450b-8891-581529afd373",
    "name": "Bundel"
  },
  {
    "uuid": "e4bc0fc7-d40b-435e-8c5d-68500db2f1e0",
    "name": "Burrito"
  },
  {
    "uuid": "7c9cfa0a-6787-45f8-aba4-b8cb68e5199b",
    "name": "Bvnger"
  },
  {
    "uuid": "693872e6-6383-4f1a-a2c7-4dd6f5cf7a73",
    "name": "bvx"
  },
  {
    "uuid": "bb05f42f-d57c-4a93-8ed8-e69cc718069b",
    "name": "calnoob"
  },
  {
    "uuid": "338fd4e5-aba2-469d-949b-0536710a425a",
    "name": "Cam"
  },
  {
    "uuid": "a1172f36-6412-4af5-9f31-a11120ee3b80",
    "name": "Carly"
  },
  {
    "uuid": "35f02248-8ad9-492b-89e2-9a648fc3fe52",
    "name": "Cashier"
  },
  {
    "uuid": "0f5a3ec3-32c4-4f51-b2a5-0e34f1556080",
    "name": "Caspre"
  },
  {
    "uuid": "580dab7b-e3cb-43a9-9bd0-4a8c043c87a1",
    "name": "CBD"
  },
  {
    "uuid": "c648f3fe-0bc1-4d9f-9ea4-b110290dda31",
    "name": "ceck"
  },
  {
    "uuid": "b12897cf-5562-4b04-99d6-3a5d323b680a",
    "name": "Chelsea"
  },
  {
    "uuid": "78682288-9dea-45d1-ae6e-c551f11d03c8",
    "name": "Christene"
  },
  {
    "uuid": "e4be5581-276d-459b-b5d9-ac5835f06cc6",
    "name": "Chucky"
  },
  {
    "uuid": "ce180cd6-20dc-420e-8eff-62e45c52464a",
    "name": "Cite"
  },
  {
    "uuid": "5230b07b-aead-44a9-89be-01c89ff2e59d",
    "name": "Clearon"
  },
  {
    "uuid": "aab39f9d-1cdc-454f-a18d-e2644807bad1",
    "name": "Cloak"
  },
  {
    "uuid": "c741d4a0-6369-48e0-9de2-9808d477624b",
    "name": "clors"
  },
  {
    "uuid": "97875ed0-5649-4048-8a49-72fcf8dd5df9",
    "name": "clout"
  },
  {
    "uuid": "5b084570-c33b-4e98-9e88-986dd5eb98eb",
    "name": "Clxne"
  },
  {
    "uuid": "8e5f2750-16e6-4dda-9886-223a11954c09",
    "name": "cocopuffs"
  },
  {
    "uuid": "403e6cb7-a6ca-440a-8041-7fb1e579b5a5",
    "name": "CoderTim"
  },
  {
    "uuid": "b6682564-b60f-46b3-94d7-5fa7a7d51a58",
    "name": "collage"
  },
  {
    "uuid": "900f95b5-d182-4e5e-9685-de639b82be5f",
    "name": "Collector"
  },
  {
    "uuid": "f52aca18-b3c4-4c02-9f67-6a274dffe7ce",
    "name": "Colossi"
  },
  {
    "uuid": "72d28075-961b-4925-a6d6-c777dc9207fb",
    "name": "Common"
  },
  {
    "uuid": "ccb4dd6e-ed12-4d99-af00-63b2b5dab102",
    "name": "CONCIDE"
  },
  {
    "uuid": "07e7e8a9-7ee8-4c74-8ee7-77f13e5ed55f",
    "name": "Core"
  },
  {
    "uuid": "338d6286-bd7b-4994-8012-9f9a176dc289",
    "name": "corel"
  },
  {
    "uuid": "10de5acf-3656-4944-a2fc-34ae0e1a2713",
    "name": "Cottagecore"
  },
  {
    "uuid": "4a924015-92c7-48bc-921a-2281df23d40a",
    "name": "Couple"
  },
  {
    "uuid": "d9a73c68-5d7c-4826-bc2f-ce8aa6a2aff5",
    "name": "cowtails"
  },
  {
    "uuid": "9e7755df-8dc9-44ad-acea-d58d1d1a7a02",
    "name": "Crumples"
  },
  {
    "uuid": "cd10e76c-1cdf-48c1-9aab-e43d29069797",
    "name": "crycries"
  },
  {
    "uuid": "6ddc48c2-f9bb-492c-93a4-52599b2d5e03",
    "name": "Cut"
  },
  {
    "uuid": "ec03c256-b51f-4867-84b1-0441068503bb",
    "name": "DADDYSGlRL"
  },
  {
    "uuid": "4aaf8ca3-864c-4679-b2b6-43769306434b",
    "name": "daisychu"
  },
  {
    "uuid": "2a70ca0f-f7e9-4a4f-a0e7-494f73b8e0fd",
    "name": "Danni1"
  },
  {
    "uuid": "bf412996-c1e4-424b-880d-1d5788628e95",
    "name": "dayfruits"
  },
  {
    "uuid": "f98d1b05-7ef5-4edd-8237-042bfd69b11b",
    "name": "Defeat"
  },
  {
    "uuid": "620142bc-93f9-447e-bb9b-42e147453340",
    "name": "Dehu"
  },
  {
    "uuid": "7606e50b-89a8-403f-b9de-f634c44d1e2d",
    "name": "Demisexuality"
  },
  {
    "uuid": "2d0190df-4f65-467b-99d7-c666b5a89c30",
    "name": "Derby"
  },
  {
    "uuid": "fc4be483-73b0-456d-9a9d-855ec4ddb26c",
    "name": "destroys"
  },
  {
    "uuid": "2cee80d4-a8a5-4220-91f6-87f7483fcf3d",
    "name": "Detect"
  },
  {
    "uuid": "16eda423-daad-4ef8-9f20-5652f205b581",
    "name": "Discontinue"
  },
  {
    "uuid": "1aa769f2-bd92-4e95-87d3-f4c1124c532d",
    "name": "Divorse"
  },
  {
    "uuid": "cc0f1328-b950-41e9-8f1e-411423781377",
    "name": "djs"
  },
  {
    "uuid": "ae0fda0d-7bb3-4532-841c-903190d7fc65",
    "name": "Dolida"
  },
  {
    "uuid": "1396b4ef-64b6-4601-a683-8c6f753e8121",
    "name": "Door"
  },
  {
    "uuid": "8d1ee56a-f6d0-4298-9949-697bc638d588",
    "name": "Dork"
  },
  {
    "uuid": "63cb7fdb-e6f5-4cb9-b6fd-8b20182d3b08",
    "name": "Douglass"
  },
  {
    "uuid": "a2851f52-7fe2-4cde-96e8-530df3065acf",
    "name": "Download"
  },
  {
    "uuid": "e69295b6-cdfa-4116-82ec-6d35b3945616",
    "name": "Doxxer"
  },
  {
    "uuid": "7dc7778a-086b-487c-9d71-609d3a4a738c",
    "name": "Dqrknesss"
  },
  {
    "uuid": "5663b605-daf1-498b-9b86-e129048b8358",
    "name": "Due"
  },
  {
    "uuid": "a120e1ef-7b80-4554-a045-f68e97323176",
    "name": "Duplexes"
  },
  {
    "uuid": "8af29653-3b68-44d0-8593-2742dca689c9",
    "name": "Dusks"
  },
  {
    "uuid": "3a60d516-b8d2-4f52-8e3d-689793580de4",
    "name": "Dwalm"
  },
  {
    "uuid": "f2e6011a-d245-4fa4-a58d-d677f3ba7fdd",
    "name": "Edge"
  },
  {
    "uuid": "207dd757-a084-41da-bb67-806d42f56fae",
    "name": "Ediscn"
  },
  {
    "uuid": "a16d8c3b-8c36-449f-99d8-e3cd4110744e",
    "name": "egirlausi"
  },
  {
    "uuid": "d5a64b26-15ea-46c4-8319-f9c83e82a1fa",
    "name": "Eliminate"
  },
  {
    "uuid": "2df2c9a3-572c-4cda-afdf-3655ff14541d",
    "name": "Envy"
  },
  {
    "uuid": "2666c044-013c-4bbe-ad84-89450ce39d18",
    "name": "EPICGAMERMJ"
  },
  {
    "uuid": "4ead7f17-17df-4723-b70a-32b273ad6131",
    "name": "euforic"
  },
  {
    "uuid": "558d5964-9325-4f9d-8ff5-f93dc7216e4a",
    "name": "F5"
  },
  {
    "uuid": "ac4a465f-2000-4952-812a-41506d6f4349",
    "name": "Fabb"
  },
  {
    "uuid": "735659d6-c847-4fe0-8816-d3b4688469fb",
    "name": "Fabulous"
  },
  {
    "uuid": "a86c2ba6-2226-432c-9d50-836a2c34c262",
    "name": "Factorising"
  },
  {
    "uuid": "7d81c2eb-f703-4f56-b602-7f7b1e929942",
    "name": "Famous"
  },
  {
    "uuid": "151eae30-2635-4162-be1d-cec2ac58c3e7",
    "name": "fangirl"
  },
  {
    "uuid": "ab0add4e-505c-4822-81bd-fffa9ff1dce3",
    "name": "FEATIES"
  },
  {
    "uuid": "a21b6ae5-b04e-4efb-8649-fb60d8a8fcae",
    "name": "fembu"
  },
  {
    "uuid": "bda65331-d305-40c8-a496-1830e5b9aeab",
    "name": "Ferment"
  },
  {
    "uuid": "70296d53-9fc3-4e53-97eb-269e97f14aad",
    "name": "Fisk"
  },
  {
    "uuid": "572a76a1-7eb4-486a-9cb9-102ca3785ff2",
    "name": "Floras"
  },
  {
    "uuid": "a3318c83-79e0-4247-b8bf-93cc06ea8cfa",
    "name": "FOODCHAIN"
  },
  {
    "uuid": "36fff839-5cb3-4d44-bd25-4c2a24b4ea18",
    "name": "Fortress"
  },
  {
    "uuid": "41ecdbcf-7d6c-4b29-8a5b-5b8a32d8e55d",
    "name": "Foxi"
  },
  {
    "uuid": "24fb0217-9925-4ff8-b822-756e710e2a91",
    "name": "fraaanmatos"
  },
  {
    "uuid": "f3911dbe-78f5-4dab-9b97-dee8f4db8a10",
    "name": "Fracturing"
  },
  {
    "uuid": "efcfc8b6-e5ce-4c77-975d-705c453f5106",
    "name": "fraid"
  },
  {
    "uuid": "198a87b0-5806-47c1-adef-b2f6540166c2",
    "name": "frxnek"
  },
  {
    "uuid": "b50c8925-2346-451f-91e0-ce7c0b1b7256",
    "name": "Fungi"
  },
  {
    "uuid": "9570163a-dd49-4ce0-b48c-06bfb3efb1b6",
    "name": "Gazes"
  },
  {
    "uuid": "f3360bad-40fa-4b2c-8bd3-bbff98e54156",
    "name": "Geqrge"
  },
  {
    "uuid": "5b52582a-4a3f-4d59-8fb5-1eaa7c8ebc92",
    "name": "Gestic"
  },
  {
    "uuid": "2a577637-77f0-4838-a2c0-f95ccfc3b62d",
    "name": "gtg"
  },
  {
    "uuid": "cc49fe89-79d6-484b-8072-9ea8a3ac2b80",
    "name": "GUSDAPPY"
  },
  {
    "uuid": "8153155b-a6ba-4ff0-a352-b7ac7eb8a139",
    "name": "Hair"
  },
  {
    "uuid": "4303d2b6-7b00-484e-a9ea-918642eb8e6e",
    "name": "Hangouts"
  },
  {
    "uuid": "5237b4b7-5eed-421d-a43f-0e4968e69207",
    "name": "hannahxxrose"
  },
  {
    "uuid": "3e0183f5-6634-416c-8d96-1ffa08d1345d",
    "name": "hellguy"
  },
  {
    "uuid": "ddbebefc-9427-4140-8d41-f36e4da6919b",
    "name": "Honduras"
  },
  {
    "uuid": "8a8bf31f-ed10-4626-8d00-439b300b870f",
    "name": "HP3"
  },
  {
    "uuid": "dcc16a1e-5fea-48f2-890b-a36bd7a4ae84",
    "name": "i4w"
  },
  {
    "uuid": "2484d432-2f4b-49df-9558-3de00e5eb4aa",
    "name": "I8I"
  },
  {
    "uuid": "b59b0915-7f9f-46b7-ac9f-618ae8174e9f",
    "name": "IceShqrk"
  },
  {
    "uuid": "60935030-23e4-4d9e-bcd1-1105254ce674",
    "name": "idec"
  },
  {
    "uuid": "0d43ff2b-80cc-461e-ad12-14b7cbebb021",
    "name": "III"
  },
  {
    "uuid": "ba93601d-e751-49ab-a24c-88ea256b763a",
    "name": "IlyRudi"
  },
  {
    "uuid": "2361ca08-44dc-4541-8fb1-4f02f3f9f222",
    "name": "iPhone"
  },
  {
    "uuid": "c23e5ef9-0e69-483d-a3e9-247196eddbaa",
    "name": "Itashi"
  },
  {
    "uuid": "84e2b7e9-7443-4cce-8a65-6b5e4dbd9a37",
    "name": "jaivie"
  },
  {
    "uuid": "d005d622-f796-4682-ae1c-dc27e15ef857",
    "name": "Jaleel"
  },
  {
    "uuid": "0fe6c20f-fa45-4348-8f65-067f906c4c30",
    "name": "Jarlin"
  },
  {
    "uuid": "ef07f569-83c4-40fc-aa78-1454b829ad9a",
    "name": "Jecy"
  },
  {
    "uuid": "1ccef50b-f6ae-4542-b1a9-d434384a5b25",
    "name": "Jeff"
  },
  {
    "uuid": "ad291843-fcf4-40e0-8620-34fd7d4b9c77",
    "name": "Jerk"
  },
  {
    "uuid": "f5e247ad-8bcc-49e7-8da8-ff960d6a3766",
    "name": "Jim"
  },
  {
    "uuid": "14906aa5-7c38-4ac2-989b-3bb4c9f83069",
    "name": "JoeBiden"
  },
  {
    "uuid": "2c50e6ed-678b-4a89-891a-e3bc987fb760",
    "name": "Joi"
  },
  {
    "uuid": "85736c50-3c7e-472c-a63a-a3551a77631e",
    "name": "jonah_"
  },
  {
    "uuid": "68568ef4-b340-42b7-955e-4d8c2bb16f60",
    "name": "Jozeeh"
  },
  {
    "uuid": "304a3ba2-1d15-42f5-b86b-087f36d8721a",
    "name": "JuiceWorId"
  },
  {
    "uuid": "69282c00-93dc-4805-999a-5877e228c50f",
    "name": "kanc"
  },
  {
    "uuid": "b293b72c-6c1a-41fb-bf71-089bce200d97",
    "name": "Keep"
  },
  {
    "uuid": "dcf2910c-04f9-4f8f-aa99-296cb4c24de1",
    "name": "Keshi"
  },
  {
    "uuid": "eddb9845-68ae-4d6d-bd50-05d4f530c112",
    "name": "Keshia"
  },
  {
    "uuid": "486914ec-9da2-42f5-aa2c-540950ddb364",
    "name": "kitty"
  },
  {
    "uuid": "711de4f9-4c94-4904-a858-8c680de8c8c9",
    "name": "kitwojownik"
  },
  {
    "uuid": "be4725d2-643b-4d94-872d-8cd407cb1b88",
    "name": "kwch"
  },
  {
    "uuid": "4df28717-dcac-4145-a3e9-b82b21c56387",
    "name": "Lars"
  },
  {
    "uuid": "30354c4d-4489-4eee-85c4-6e166709ee5a",
    "name": "LEGITPLAYERBRE"
  },
  {
    "uuid": "a90c39ac-bbb5-4e40-bb99-8bbd3e58b3a5",
    "name": "Lende123"
  },
  {
    "uuid": "f26ad2bb-5a63-4759-ac9e-42f7f3ff43fd",
    "name": "Lickii"
  },
  {
    "uuid": "37293217-656e-4f6d-96f4-6a5658c8d520",
    "name": "Lim"
  },
  {
    "uuid": "93bf0feb-2ed9-42ab-be2f-a4a585f8dd35",
    "name": "Liyfii"
  },
  {
    "uuid": "b4769eac-1010-405a-b668-04a07b2f20f3",
    "name": "lolitsalex"
  },
  {
    "uuid": "73ab5780-cfb5-46b9-8efb-56d2f40deb93",
    "name": "Lookout"
  },
  {
    "uuid": "866574bb-5b53-402c-a53d-168903fe0143",
    "name": "LooneyTunes"
  },
  {
    "uuid": "f011e170-0130-4c41-b284-e1171035f536",
    "name": "Lost"
  },
  {
    "uuid": "e90c93b7-249f-4eef-82c8-00097aa7d28c",
    "name": "Louis"
  },
  {
    "uuid": "2e4a7c28-b4d4-46f9-af89-0e0fd6e1e8e6",
    "name": "Lovino"
  },
  {
    "uuid": "b28a9123-abf0-442e-8821-0f86d672c695",
    "name": "Luv"
  },
  {
    "uuid": "69954857-ee31-4a76-b9bf-fa43a922ee4c",
    "name": "Lux"
  },
  {
    "uuid": "e7650391-4e8f-468d-aeb0-81dbfed0c7f6",
    "name": "Luxury"
  },
  {
    "uuid": "55ccf198-12d3-480b-814a-aed79b93601a",
    "name": "LynnPlays_"
  },
  {
    "uuid": "4a66d3d8-7eed-42e6-a479-e4139e9041ee",
    "name": "M6yo"
  },
  {
    "uuid": "8de5c872-4d30-40d9-9d9a-473ab626567a",
    "name": "Magepunk"
  },
  {
    "uuid": "fe15273a-c660-4a6f-95da-ee3f9458eeba",
    "name": "Manhal_IQ_"
  },
  {
    "uuid": "7a3c3291-08aa-4a4a-866c-112aabdbda96",
    "name": "MCBYT"
  },
  {
    "uuid": "d7961a28-fd8d-43d8-96fa-bb6d4bffaa30",
    "name": "Measurer"
  },
  {
    "uuid": "fae14fed-b1b9-4938-8b6c-250e7db818a1",
    "name": "MeeZoid"
  },
  {
    "uuid": "40d812f9-be8b-45fb-9251-c082a451008d",
    "name": "Megan"
  },
  {
    "uuid": "0e0468f5-9bb4-4c09-a1a3-5c24e0c6f837",
    "name": "mercum"
  },
  {
    "uuid": "8f265384-c73c-40d2-b79d-fea376e4b5e6",
    "name": "Mew"
  },
  {
    "uuid": "ed4c04db-09aa-40ce-8186-337fb40ae51b",
    "name": "Minight"
  },
  {
    "uuid": "d95afc28-94c0-4b2b-b5a9-0058d0fed51b",
    "name": "Miynh"
  },
  {
    "uuid": "631f163b-6702-4cd2-b1d1-b104464cd60e",
    "name": "Mlnion2"
  },
  {
    "uuid": "ca46c64f-3378-44df-8e6f-2fb4a8a9106a",
    "name": "Moo"
  },
  {
    "uuid": "3367543e-08af-4caf-a2dc-d5e4ab13fdc5",
    "name": "mph"
  },
  {
    "uuid": "9328e5d5-0215-4ebb-9519-24e5968d0cc7",
    "name": "MrNames"
  },
  {
    "uuid": "24854322-50a2-444d-b6db-8c6f04fa6474",
    "name": "mtrani"
  },
  {
    "uuid": "17494e1c-7037-450f-bb6f-4c3de615acb1",
    "name": "Multi"
  },
  {
    "uuid": "8dbd88e4-0079-4353-865f-c7c97d585a48",
    "name": "Music"
  },
  {
    "uuid": "88895145-e7b5-4dc2-bf54-13637c640e55",
    "name": "Mutant"
  },
  {
    "uuid": "b3dcaa03-ff26-46f7-b4cf-729fa0f39d0d",
    "name": "Naxxoo"
  },
  {
    "uuid": "de6cf9c4-2c11-473c-9794-0e9aa76e7d96",
    "name": "Neo"
  },
  {
    "uuid": "fe40b828-852c-47bf-a36a-1713784fbf50",
    "name": "newsmen"
  },
  {
    "uuid": "bcf3490f-e174-4820-9d6a-5e4b671fb03a",
    "name": "Nicoooh"
  },
  {
    "uuid": "9c62e1ac-16bb-41fe-8b7e-b4692864b2c2",
    "name": "Ninja"
  },
  {
    "uuid": "6e21a329-586d-476e-a30b-2a0d85e421a5",
    "name": "NiqhtViaa_x3"
  },
  {
    "uuid": "eabac01b-0bdf-4763-b57b-0502511610ad",
    "name": "Nixe"
  },
  {
    "uuid": "0fad361a-1830-44c4-9793-38b7de7ca8b4",
    "name": "njet"
  },
  {
    "uuid": "f0d02567-ea80-491c-8dab-b210a872cbe0",
    "name": "nominating"
  },
  {
    "uuid": "91d8cbb7-4753-471f-af93-75bae55ac8ce",
    "name": "NotNico"
  },
  {
    "uuid": "af587d2e-9c61-4ea1-b8b1-c504947f0784",
    "name": "Nurvi"
  },
  {
    "uuid": "aa482d0e-a51f-428d-a990-d951650d4e89",
    "name": "oAnxiety"
  },
  {
    "uuid": "567b1761-2811-4a10-9ef2-3b7d0c3f87fa",
    "name": "onlyvibe"
  },
  {
    "uuid": "c8413156-6ea2-43ae-88b3-8b45865184bc",
    "name": "Optifine"
  },
  {
    "uuid": "f8cd5f56-31c3-475b-ae9e-f2ad677ce2ed",
    "name": "oVincent"
  },
  {
    "uuid": "83d045c6-f6de-4c6f-a0f9-7c0b86b4c0a3",
    "name": "owem"
  },
  {
    "uuid": "109c98e8-732a-4e23-815a-25914aeeed34",
    "name": "pacxx"
  },
  {
    "uuid": "246dfa75-237a-4007-b104-b405ef58198f",
    "name": "PayPal"
  },
  {
    "uuid": "acd3f5df-187f-4c7d-8aba-e5fd19db3699",
    "name": "Phobia"
  },
  {
    "uuid": "5beb911e-e586-42dc-b157-94f569f59005",
    "name": "Phycology"
  },
  {
    "uuid": "75671ef0-fd85-4875-bdf4-891dbf17ae58",
    "name": "Pibi"
  },
  {
    "uuid": "d1d06b5b-26a7-40a3-9da7-d6f2ed2b50cb",
    "name": "Pillar"
  },
  {
    "uuid": "5f4672e5-b5e0-47d8-84c9-e35470fe4857",
    "name": "Pillars"
  },
  {
    "uuid": "d506e55b-b901-4f26-a3d6-6f5dc21cfd35",
    "name": "piricompas"
  },
  {
    "uuid": "d0324c08-8c94-49ec-8d5d-5c83d82c8c50",
    "name": "Planner"
  },
  {
    "uuid": "0a3fce62-34fa-4efd-a50d-c1149be08dca",
    "name": "Poise"
  },
  {
    "uuid": "43bf7504-792c-4ad5-ac6d-37d8e3e18421",
    "name": "pokiu"
  },
  {
    "uuid": "b88e35dd-4b22-4a6d-bbcd-344aec6b78c3",
    "name": "poster"
  },
  {
    "uuid": "814381c0-069e-46de-b5dd-83d1a4b1c1aa",
    "name": "PRAXYY"
  },
  {
    "uuid": "2fa9e4e9-90d5-4e1d-b6e5-98b45f9bb274",
    "name": "Prepare"
  },
  {
    "uuid": "30a47ba7-dffc-4b5a-a43e-97455be51896",
    "name": "Produce"
  },
  {
    "uuid": "79eb74f2-4ffa-463c-9afd-5239722e18fc",
    "name": "Protest"
  },
  {
    "uuid": "f180dbdb-5655-403a-a143-956cd75f0d51",
    "name": "PS1"
  },
  {
    "uuid": "aa601ca8-2dd5-47fe-91eb-a6726431dc53",
    "name": "Python"
  },
  {
    "uuid": "b70aa28a-e7f6-44d5-a47e-687d35f113d9",
    "name": "qMad"
  },
  {
    "uuid": "8d49bfa0-6bd4-45d2-9a6b-1ec8c6ce65e6",
    "name": "Quality"
  },
  {
    "uuid": "daafa3b9-6b6e-4ad9-9fab-dc3329413a35",
    "name": "Ramsy"
  },
  {
    "uuid": "61f84cda-c894-4273-aa5d-30508654fb9a",
    "name": "Rare"
  },
  {
    "uuid": "0852b458-16e7-41f5-a57c-b7eda17e5e04",
    "name": "Rassistonaut"
  },
  {
    "uuid": "93dda80c-65f1-4cac-ad85-24a01b1d9e05",
    "name": "Reecce"
  },
  {
    "uuid": "9c43a472-575a-4c9a-9b47-8ad756450a10",
    "name": "Remote"
  },
  {
    "uuid": "aa274553-deb8-4546-910a-ccf58b2b7141",
    "name": "Reseals"
  },
  {
    "uuid": "09b76a85-1e5a-4e65-aadf-d7430beb1729",
    "name": "Restart"
  },
  {
    "uuid": "505c9160-2a59-4ae1-9d40-7e1e67da08aa",
    "name": "Room"
  },
  {
    "uuid": "11da6c98-22f6-4e88-b289-ff15fd433091",
    "name": "Rotto"
  },
  {
    "uuid": "226add32-23b2-4521-8443-8e7516459bf3",
    "name": "Sailboater"
  },
  {
    "uuid": "fb71c0fc-6dba-4a18-a397-f2cce59f28d7",
    "name": "Sam"
  },
  {
    "uuid": "c3c86c84-7b09-4d00-8247-119bf214e039",
    "name": "Sandal"
  },
  {
    "uuid": "92a220c3-5e6c-42bf-a585-6534f4c6a290",
    "name": "Saox"
  },
  {
    "uuid": "b072182e-0084-4e3e-abfe-b440fb7742ac",
    "name": "Scorn"
  },
  {
    "uuid": "e0564f41-7d38-4f3c-9bfd-f250cd001982",
    "name": "Scott"
  },
  {
    "uuid": "f0079842-385f-4835-bd5a-03fddf58aeb6",
    "name": "Scrosen"
  },
  {
    "uuid": "cc1e48c5-0752-42fb-8773-f6ea05c5026c",
    "name": "selfabort"
  },
  {
    "uuid": "29c6a931-6a31-46d9-8f5b-77a89f34468e",
    "name": "Shane"
  },
  {
    "uuid": "a39a4475-dc18-4574-a83f-aa14a39cba0b",
    "name": "shimato_420"
  },
  {
    "uuid": "dfe75173-ce89-4074-9bdc-4da4ba2c80b1",
    "name": "Shortcut"
  },
  {
    "uuid": "63aadfdf-7394-4956-874b-c3e0a02c99bc",
    "name": "Shrieked"
  },
  {
    "uuid": "ed6daf33-575b-460b-a2f3-e208a1004c10",
    "name": "Siri"
  },
  {
    "uuid": "ac425634-a3b0-4902-94cd-4f7dac6f1571",
    "name": "Skies"
  },
  {
    "uuid": "22b933e5-bbfb-4b31-aae3-91bfacf20f54",
    "name": "Skiving"
  },
  {
    "uuid": "34cf9372-b51d-4629-8ae3-2eabe31c6170",
    "name": "Sleveris"
  },
  {
    "uuid": "c4fdfed8-b1fe-47cd-8225-006fdd196d33",
    "name": "slevsbunny"
  },
  {
    "uuid": "2ee7ca88-31bd-4f71-85f5-4e32c56653c0",
    "name": "Snape"
  },
  {
    "uuid": "aba44cdd-0396-46e3-9c27-d063587145e3",
    "name": "sncww"
  },
  {
    "uuid": "46f89c4d-cde5-49e7-9920-c7b61b784335",
    "name": "Snuz"
  },
  {
    "uuid": "0666fffd-732d-428b-ae17-2992d4527ede",
    "name": "Solitude"
  },
  {
    "uuid": "68797299-f02f-4ecd-a451-e3275c5cf49d",
    "name": "sometimes"
  },
  {
    "uuid": "63819adf-3fa4-4ad7-b8a2-82c4e5ba523f",
    "name": "soundwave507"
  },
  {
    "uuid": "b1dca070-854c-43af-a189-3af0713adafd",
    "name": "spit"
  },
  {
    "uuid": "c4c72feb-a07d-410b-bfa3-c549fa75bdff",
    "name": "Splash"
  },
  {
    "uuid": "dbf5fd47-8b2d-48ba-9847-4a75cce86411",
    "name": "Splinter"
  },
  {
    "uuid": "991171ca-6653-4f7f-aa18-a81510179265",
    "name": "splutchy26"
  },
  {
    "uuid": "0a94cf3e-a410-432f-9d18-6a067dd0e86b",
    "name": "Stay"
  },
  {
    "uuid": "79923036-b581-466a-853f-c15d96ed473d",
    "name": "Straight"
  },
  {
    "uuid": "d0c41f9f-70e3-446e-8937-8fd5034081a3",
    "name": "Successfull"
  },
  {
    "uuid": "8d5951a3-907b-49c1-96b4-04adcb59f58c",
    "name": "sus"
  },
  {
    "uuid": "f2d0dc02-1726-4846-9ca8-9573a4cadb47",
    "name": "Sw1j"
  },
  {
    "uuid": "6d02334e-cf92-403b-b31e-20c1cc3bbcde",
    "name": "swirled"
  },
  {
    "uuid": "db4a1d18-e4a1-482a-8fa7-163d0a00e276",
    "name": "Talya"
  },
  {
    "uuid": "de83b5a7-0391-4dbb-ad43-e87cf65fa620",
    "name": "Taste"
  },
  {
    "uuid": "10f70f56-9b38-45b1-8e66-6338d7f36bf2",
    "name": "teayuh"
  },
  {
    "uuid": "95630945-a97e-4dfd-a9e1-2d941a642ad4",
    "name": "Telepathy"
  },
  {
    "uuid": "f30ba35a-6bc4-45e5-a93c-0b07cfc1a17c",
    "name": "tenfeet"
  },
  {
    "uuid": "d512ba7a-b97c-49cb-8ab1-1227b5bb0f53",
    "name": "Terrible"
  },
  {
    "uuid": "5746c9f9-182f-4c76-a5ac-a48ba5eb2adc",
    "name": "Theyll"
  },
  {
    "uuid": "608fee54-cd81-42e8-8bee-27216ca82857",
    "name": "Thunderbolt"
  },
  {
    "uuid": "0e371352-2c0f-4b63-a20e-2474724ae761",
    "name": "Tight"
  },
  {
    "uuid": "896c1c65-08f1-4d10-9dc9-4ff45cd3dfd6",
    "name": "Tossed"
  },
  {
    "uuid": "dc78a37b-7b8c-4b75-8602-2258bef3b96f",
    "name": "Totem"
  },
  {
    "uuid": "ecd27fd8-5b86-4683-98b4-f3e59dbda7de",
    "name": "toxci"
  },
  {
    "uuid": "0cff6af7-8f77-4f3e-87ab-e8eac13589fa",
    "name": "tri"
  },
  {
    "uuid": "0e582c99-97e1-44a6-960b-79965c9cb355",
    "name": "unhappyy"
  },
  {
    "uuid": "0d2ae6f5-0b82-4380-a8ed-8135e0449b20",
    "name": "unhindered"
  },
  {
    "uuid": "a487ace7-c257-4df0-befb-b3735114553a",
    "name": "unslow"
  },
  {
    "uuid": "713259d4-d3d2-491c-b95e-b6300a9d14e0",
    "name": "Usher"
  },
  {
    "uuid": "f0127719-394f-4acb-bf92-b68fca790289",
    "name": "uue"
  },
  {
    "uuid": "c2d15748-2971-40ae-9890-0237be07b318",
    "name": "Valkys"
  },
  {
    "uuid": "8ae44825-c3bc-4f91-ae51-82b625b62110",
    "name": "Vedusa"
  },
  {
    "uuid": "c3fac957-fe49-48d3-8700-716912ede69a",
    "name": "Velh"
  },
  {
    "uuid": "c846a925-7f66-49fc-ade1-d8cb204d18db",
    "name": "vesn"
  },
  {
    "uuid": "ef259a0e-5b05-4911-8d87-06b19ac95f23",
    "name": "victories"
  },
  {
    "uuid": "8aadb7cc-a98f-414a-8433-fe65617a3eaf",
    "name": "VirtualTea"
  },
  {
    "uuid": "eb0be566-7850-4c94-8357-7cbf8041814b",
    "name": "vitaax"
  },
  {
    "uuid": "2f65e89b-a5b3-4586-b0dd-d312a6ca0e15",
    "name": "W0RRIES"
  },
  {
    "uuid": "52baf8e4-9d07-4c42-8cea-ac5a231cc89c",
    "name": "Wack_Attack"
  },
  {
    "uuid": "89225796-7f7b-4d8e-bfbf-705951794346",
    "name": "Waitresses"
  },
  {
    "uuid": "8e17e70c-1918-4c01-a13b-7dd32eae79cf",
    "name": "Warning"
  },
  {
    "uuid": "51685f17-e03a-4346-9a30-504dbd1953be",
    "name": "Wholesome"
  },
  {
    "uuid": "83d79c89-b718-4bab-a687-6764671f4aab",
    "name": "wqzes"
  },
  {
    "uuid": "6b831421-b03b-45d6-bbee-c660c1ef3abf",
    "name": "wtf"
  },
  {
    "uuid": "9d996931-373a-4e03-8b0c-d5ae2bd966a6",
    "name": "wtfben"
  },
  {
    "uuid": "9a774e18-6273-4a53-878f-f303b53775bc",
    "name": "Wxhy"
  },
  {
    "uuid": "969b1e6b-82da-4f46-8027-b1c0b9aef559",
    "name": "wydbbg"
  },
  {
    "uuid": "f9822147-244d-4c74-a3f4-79baef43f3bf",
    "name": "xcnax"
  },
  {
    "uuid": "e44f9ee7-3d0d-4add-bd58-3c099291a509",
    "name": "xDreamGer_"
  },
  {
    "uuid": "935e160c-0a9d-49e5-a1ef-2ccd1d54ff7d",
    "name": "xinabox"
  },
  {
    "uuid": "ed66a35c-00f3-4218-9540-0e72c8e96cb2",
    "name": "xk"
  },
  {
    "uuid": "74f563de-d0ba-4358-bf32-bd16901897d7",
    "name": "xn5"
  },
  {
    "uuid": "1cbc5eb6-e95a-4325-a660-c3b7e83b95e0",
    "name": "x_x"
  },
  {
    "uuid": "20877605-064d-42a9-a058-250fb187171d",
    "name": "X__"
  },
  {
    "uuid": "6b8d8d68-fdd0-4566-9274-6759f8890a82",
    "name": "Yanny"
  },
  {
    "uuid": "4b6e77dc-3067-4043-ac5a-1f43fdacc1a4",
    "name": "Yeezys"
  },
  {
    "uuid": "23a93fac-93e3-4f5c-98b1-b179b347f310",
    "name": "yogrt"
  },
  {
    "uuid": "44fb33df-c394-4355-82fc-286b21962923",
    "name": "Yohaacraft"
  },
  {
    "uuid": "abef2ad5-a941-49f5-a84f-7656924e8c97",
    "name": "YourLocalStalker"
  },
  {
    "uuid": "b86d814c-fb09-420d-9435-9c589edea731",
    "name": "Yuck"
  },
  {
    "uuid": "dfed3752-88a2-43e3-8492-9e9486be8bcd",
    "name": "zareexd"
  },
  {
    "uuid": "28ab4d97-c8ed-47c0-a701-c7d8819bc9a4",
    "name": "ZegaMC"
  },
  {
    "uuid": "929cacd2-3e69-4641-9c8c-60444a11c366",
    "name": "Zelistic"
  },
  {
    "uuid": "1c9d1be4-0347-44f3-8270-decebf7f2672",
    "name": "ZeroLogic"
  },
  {
    "uuid": "04f0b5ea-bfab-4191-9797-e45b06aea06e",
    "name": "zKevsh"
  },
  {
    "uuid": "0754b578-8495-4048-bd91-933dbbd61dee",
    "name": "Zorkai"
  },
  {
    "uuid": "7e609b1a-aaaa-4157-a777-988427a289eb",
    "name": "zqw"
  },
  {
    "uuid": "f815dd0c-e2f1-4ff7-a554-86dc87ddbf9c",
    "name": "_Waylon"
  }
]
```

**No Friends / HTTP `200`:**
```json
[]
```

**Invalid UUID / HTTP `400`:**
```
Bad Request
```

**You Didn't Provide The Username Parameter / HTTP `404`:**
```json
{"error":"You didn't supply an account to get a skin hash from! Add the parameter ?username=IGN_HERE."}
```
