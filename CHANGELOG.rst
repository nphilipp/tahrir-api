Changelog
=========

0.4.0
-----

- Watch out for the other 'person' in the scope. `de8efd36f <https://github.com/fedora-infra/tahrir-api/commit/de8efd36f3140417030a0e6733c5815562bdf764>`_
- Preserve order here. `306da8eec <https://github.com/fedora-infra/tahrir-api/commit/306da8eec0139f8ba003709172ef0069c43a0147>`_
- Merge pull request #20 from fedora-infra/feature/person-scope `0c023d474 <https://github.com/fedora-infra/tahrir-api/commit/0c023d474161938ee4aec371334b5750e94f2bbc>`_
- Pull in the ordereddict on py2.6. `4700ef8af <https://github.com/fedora-infra/tahrir-api/commit/4700ef8af2e338147cdcf27aecabaf8ca66999ed>`_
- Merge pull request #21 from fedora-infra/feature/preserve_leaderboard_order `abc5299ff <https://github.com/fedora-infra/tahrir-api/commit/abc5299ff400e7b3b51b7dcf37e2037abdb5bb61>`_
- Add a last_login field for persons. `0e08f1501 <https://github.com/fedora-infra/tahrir-api/commit/0e08f150112a86a239aca5cd6bdc5ccd162021a0>`_
- Add API interface for last-login modifications. `6fef6f7ba <https://github.com/fedora-infra/tahrir-api/commit/6fef6f7badc67e73d366831ebc3bd09c3b1d7351>`_
- Make the note_login signature symmetric with get_person. `fb6f2b6c8 <https://github.com/fedora-infra/tahrir-api/commit/fb6f2b6c8eb68aa1c8a35dfe54f52c0cf44f3209>`_
- Merge pull request #22 from fedora-infra/feature/add-last-login `3798a82d7 <https://github.com/fedora-infra/tahrir-api/commit/3798a82d798688c663ed39239a22ed47e013118a>`_

0.3.0
-----

- Clean up readme. `79fca2522 <https://github.com/fedora-infra/tahrir-api/commit/79fca2522d324a80b827df69d845d8cd327662d1>`_
- Harsher slugification. `0f35df3a3 <https://github.com/fedora-infra/tahrir-api/commit/0f35df3a33552092c9271ec9ec81b19d058d8da0>`_
- Add a new column to the persons model to keep track of rank. `7fa90759f <https://github.com/fedora-infra/tahrir-api/commit/7fa90759fdcfc8a96b48331ac9d43aba100db419>`_
- Add failing test for cached ranking. `e3a19392c <https://github.com/fedora-infra/tahrir-api/commit/e3a19392c2d00699995733acbcd15adcc3a5e648>`_
- Isolate those tests a little more. `e0c702ed4 <https://github.com/fedora-infra/tahrir-api/commit/e0c702ed425cd1fa17ca53720d593aa9b79c6d41>`_
- Add a __repr__ to make debugging tests easier. `be0ffc229 <https://github.com/fedora-infra/tahrir-api/commit/be0ffc2297674a599c674cb1340b53de7899c067>`_
- Recalculate and cache rank each time a new assertion is awarded. `f36fc6cdb <https://github.com/fedora-infra/tahrir-api/commit/f36fc6cdb1419912995697216635bbd6ae27b0b2>`_
- Expose a Person's rank in __json__. `c948f722c <https://github.com/fedora-infra/tahrir-api/commit/c948f722c13d3d6427dddcb36bb13d2945c2dfc7>`_
- Accept a notification callback and invoke it when rank changes. `a1ba93054 <https://github.com/fedora-infra/tahrir-api/commit/a1ba93054dc25604511eca42416cd79099eccf06>`_
- Remove spurious backslash. `9e30a3e81 <https://github.com/fedora-infra/tahrir-api/commit/9e30a3e81e8188442d1e07e4bf7c476947a251e9>`_
- Simplify that adjust_ranks call. `c899188d6 <https://github.com/fedora-infra/tahrir-api/commit/c899188d6ef8b7e34d4ed22ec1c5de86aba144cc>`_
- Add a test for pre-existing users with no cached rank. `4d5db0f95 <https://github.com/fedora-infra/tahrir-api/commit/4d5db0f95a9e780b7e0ee232fb0dd9e25c34f569>`_
- Additionally, send the badge award message too.  Because that just makes sense. `0e6d5b22c <https://github.com/fedora-infra/tahrir-api/commit/0e6d5b22cece05f541d0162c3480401686b7b122>`_
- Introduce timelimits to the leaderboard maker. `31d67a598 <https://github.com/fedora-infra/tahrir-api/commit/31d67a5989fca0688682152896719700eb931ed5>`_
- Also.. watch out for these. `46c9e7389 <https://github.com/fedora-infra/tahrir-api/commit/46c9e7389d92ec4abf04ff96d026ad01de501202>`_
- Revert "Also.. watch out for these." `7d1dd0d62 <https://github.com/fedora-infra/tahrir-api/commit/7d1dd0d62c16b1949631a3361e442e3a2d6e6a62>`_
- Change that fedmsg topic from "update" to "advance" (since it will always be advancing, and we never emit messages for rank slipping). `8b6be130e <https://github.com/fedora-infra/tahrir-api/commit/8b6be130e66c8780439b0c081f1353ec8b01f713>`_
- Add a comment on the meaning of the 'start' and 'stop' parameters. `0dd45b85a <https://github.com/fedora-infra/tahrir-api/commit/0dd45b85a8fc6d71bcf29a323239b9bfd0649a84>`_
- Add a docstring for _adjust_ranks. `2bc1d8eda <https://github.com/fedora-infra/tahrir-api/commit/2bc1d8edad98f21c1acc430c43f1ddb235b4d711>`_
- Explicitly label the sq.func('count') interface. `bf2994d8c <https://github.com/fedora-infra/tahrir-api/commit/bf2994d8c6b057e06e3bba0fcba5980f67b13cf1>`_
- Nuke unicode_literals. `4bdbe3e98 <https://github.com/fedora-infra/tahrir-api/commit/4bdbe3e98ae3f08d04e4d545e71feb9c71bd8ac6>`_
- Make ranking-tie test a little more forgiving since database ordering is undefined. `8bb7db1fd <https://github.com/fedora-infra/tahrir-api/commit/8bb7db1fd6220543669b5e43667baa29be5c59ef>`_
- Add a note to the comment about null rank. `899564420 <https://github.com/fedora-infra/tahrir-api/commit/899564420f88fd5f1bd6f1734e2b9e89c38f63fa>`_
- assert_in fails on py2.6, so roll our own. `f296da1ec <https://github.com/fedora-infra/tahrir-api/commit/f296da1ecd79fcb19d3eaef9fc0b7a79c5a0a46a>`_
- Merge pull request #19 from fedora-infra/feature/ranking `b23db318c <https://github.com/fedora-infra/tahrir-api/commit/b23db318c4dfbd289cef93549b81901be1038b57>`_

0.2.8
-----

- Unfinished get_badges_from_tags code from yesterday. `94bd55030 <https://github.com/fedora-infra/tahrir-api/commit/94bd550300a752d135e19151d0bee7afe6a17282>`_
- Merge branch 'develop' into feature/badges-from-tags `e82b15a8f <https://github.com/fedora-infra/tahrir-api/commit/e82b15a8f024f287ce60066b1ee7866337447190>`_
- More progress on badges_from_tags, just gotta figure out this last part... `d1d020dbf <https://github.com/fedora-infra/tahrir-api/commit/d1d020dbf616eee8070bf777d6eacd880142f478>`_
- Woo, get_badges_from_tags method is working! `7589178a1 <https://github.com/fedora-infra/tahrir-api/commit/7589178a1b70d1697eef29860d1eaa093842f840>`_
- Merge branch 'feature/badges-from-tags' into develop `d87ea66ae <https://github.com/fedora-infra/tahrir-api/commit/d87ea66ae36fcf8cd943180a4b679bb3de148500>`_
- Misplaced paren. `b3478f916 <https://github.com/fedora-infra/tahrir-api/commit/b3478f916ab42de15376405a768005dbc9fd4d19>`_
- Fix bug where duplicate badges were returned by get_badges_from_tags. `df64ba362 <https://github.com/fedora-infra/tahrir-api/commit/df64ba3626e791f19acddfeb17122c9f64c8669a>`_
- Update dbapi.py `286a57dd2 <https://github.com/fedora-infra/tahrir-api/commit/286a57dd26cce4a9a40f5567f319de88c04527ad>`_
- Implement Threebean's idea for match_all, with a few tweaks. Tests will still not pass, because we need to make "contains" look for whole words, and not just parts. `0c4a50abe <https://github.com/fedora-infra/tahrir-api/commit/0c4a50abe327db0a03703e240856f0f480077d9b>`_
- Add a query for opt-out to the api. `455499e48 <https://github.com/fedora-infra/tahrir-api/commit/455499e48b8ffd56b7072d79775c98b9e592f335>`_
- Remove q debugging from tags test and enable it. Will still fail. `a25fdc0f0 <https://github.com/fedora-infra/tahrir-api/commit/a25fdc0f0b1d1fe0d86cb8ecb7624d3ecc1bedc9>`_
- Make sure tags string has a trailing comma when adding a badge. `c802d8000 <https://github.com/fedora-infra/tahrir-api/commit/c802d80009830c92ac9774cfa842773612cedd5f>`_
- Make sure tags actually exists before running .endswith() on it. `775ab1dc0 <https://github.com/fedora-infra/tahrir-api/commit/775ab1dc0359aa4a247a195a440af614fc085433>`_
- Complete get_badges_from_tags, and all tests are passing! :D `41f16bb0d <https://github.com/fedora-infra/tahrir-api/commit/41f16bb0d57b320eb1cf15f5f8586b0047c42441>`_
- Merge pull request #18 from Qalthos/patch-1 `9f187462c <https://github.com/fedora-infra/tahrir-api/commit/9f187462c542ebbd0a51f822b55900ed3aaf415c>`_

0.2.7
-----

- Datetime objects are not JSON serializable. `a9ccdc8c6 <https://github.com/fedora-infra/tahrir-api/commit/a9ccdc8c6f847c197f5ae01b7dc953ec73e22009>`_
- Add get_invitation method to get an invite by its unique ID. `585b39e98 <https://github.com/fedora-infra/tahrir-api/commit/585b39e985b8eb61a9b4e1de6fe87347f14b8a0b>`_
- Fix comical bug. `6000d623a <https://github.com/fedora-infra/tahrir-api/commit/6000d623adb7eec7451faa96868caa7fdb17e048>`_
- Make add_badge always return a smart id. `78e13b4da <https://github.com/fedora-infra/tahrir-api/commit/78e13b4da9efe0537c47fafa501d1cc5780e66f3>`_
- Actually use that badge_id. `a90203a67 <https://github.com/fedora-infra/tahrir-api/commit/a90203a6776166353743bc474718420744dc087e>`_

0.2.6
-----

- Allow our caller to pass in an already created session object. `2620f7bb9 <https://github.com/fedora-infra/tahrir-api/commit/2620f7bb951f56fb11dd57d598a0bb657cf11c51>`_
- Be less odd. `d710209d8 <https://github.com/fedora-infra/tahrir-api/commit/d710209d8b98f52030caee1e09cc8e6dba49dc37>`_
- Autocommit after certain method calls, but only when configured to do so. `257ec1b5e <https://github.com/fedora-infra/tahrir-api/commit/257ec1b5ede62c8ee3597f7ac3b540bff2773f38>`_
- Make get person/badge and badge/person exists methods case-insensitive. `90a82a97f <https://github.com/fedora-infra/tahrir-api/commit/90a82a97fec6678e53bd503a5bd8940f2daaa8bf>`_
- Make get_assertions_by_badge case-insensitive. `e07af017c <https://github.com/fedora-infra/tahrir-api/commit/e07af017c35e056af372ec9e017cc5576ef07347>`_
- PEP 8. `88f89f839 <https://github.com/fedora-infra/tahrir-api/commit/88f89f839ea652e9521606828312692da3fec2fe>`_
- Add method to get invitations by issuer ID. `8160010c4 <https://github.com/fedora-infra/tahrir-api/commit/8160010c41b99787e5d6cdaec74f041dbba30624>`_
- Invitations have persons as issuers, not Issuers. `7de2e7b3c <https://github.com/fedora-infra/tahrir-api/commit/7de2e7b3c9adca9129abf85c6b01484cda020f58>`_

0.2.5
-----

- Make users' nicknames unique. `fa310e8bb <https://github.com/fedora-infra/tahrir-api/commit/fa310e8bb584239f6596cb2962ded4aaf9086811>`_
- 0.2.5 `981b97558 <https://github.com/fedora-infra/tahrir-api/commit/981b97558e1bcce8c4e032ae83dc684836da38ac>`_

0.2.4
-----

- Add get_all methods for models that didn't have them. `936eb3516 <https://github.com/fedora-infra/tahrir-api/commit/936eb3516854e996ba8f64efb0e0cea0924cdf6c>`_
- Uniform test names (where possible). `f8d37261e <https://github.com/fedora-infra/tahrir-api/commit/f8d37261e30c180aa17cb011d39d459871474c24>`_
- Add get_assertions_by_badge. `a11358bc4 <https://github.com/fedora-infra/tahrir-api/commit/a11358bc4a57ba1b363e734db0311187e03595a9>`_
- Adjust some indentation. `bc0eb0cc4 <https://github.com/fedora-infra/tahrir-api/commit/bc0eb0cc4e960e0f6b3a914b150b4b1082832481>`_
- PEP 8. `1d9adc3f3 <https://github.com/fedora-infra/tahrir-api/commit/1d9adc3f3f7dc915ce3531f6416b00613c9a7647>`_
- Fix a mistake in that function I just added. `284fc4f2e <https://github.com/fedora-infra/tahrir-api/commit/284fc4f2e6e7db330b3ad7c0c6ccdc19877ceda7>`_

0.2.3
-----

- Fix syntax error in alembic script. `3634d46c1 <https://github.com/fedora-infra/tahrir-api/commit/3634d46c1676db977eb5c695def6c1e9af54c338>`_
- persons.id is actually an integer, so this foreign key must match. `99088b584 <https://github.com/fedora-infra/tahrir-api/commit/99088b58404b2432a394b7afd49ab6bef1bde6ab>`_
- Alembic upgrade script to fix foreign key mismatch. `d19a0a9a5 <https://github.com/fedora-infra/tahrir-api/commit/d19a0a9a5416cc9ad174fb474c09430e1e9ce5bc>`_
- Patch to allow creating a Person with a website and a bio, as well. `19311fd8d <https://github.com/fedora-infra/tahrir-api/commit/19311fd8ddd376cfb1a54bb173c493b18305c362>`_
- Allow add_badge to take tags. `57b32e6dd <https://github.com/fedora-infra/tahrir-api/commit/57b32e6dd54567621516e7055a2159115a5cdc64>`_
- Add two new columns for Person we will need. `43bce48cf <https://github.com/fedora-infra/tahrir-api/commit/43bce48cf261b849db9207e24f87fe864cdd2b55>`_
- Alembic script for the last DB upgrade. `b048918b4 <https://github.com/fedora-infra/tahrir-api/commit/b048918b4939f533bb539eb25faeeb7d8a9d943b>`_
- Merge pull request #17 from fedora-infra/feature/person.created_on `b572ea3e7 <https://github.com/fedora-infra/tahrir-api/commit/b572ea3e76c6dd21f89f37b21570ebb26c600212>`_
- Merge pull request #16 from fedora-infra/feature/foreign-key-mismatch `58b10f435 <https://github.com/fedora-infra/tahrir-api/commit/58b10f435c63cc7794b70985635820050a93aa61>`_
- Put things in a straight line. `b8b008178 <https://github.com/fedora-infra/tahrir-api/commit/b8b008178779481c8e192b0269ddc61a468c2287>`_

0.2.2
-----

- Include alembic stuff and tests when we do a release to pypi. `5f7a6e23a <https://github.com/fedora-infra/tahrir-api/commit/5f7a6e23aae4dd5e923a1a427f1dc41108fd19c7>`_

0.2.1
-----

- Allow add_person to set the nickname. `0a6daea03 <https://github.com/fedora-infra/tahrir-api/commit/0a6daea03df16937a7fd1cafdcf46ec5a420c123>`_
- person_exists should accept other arguments. `0f53c9154 <https://github.com/fedora-infra/tahrir-api/commit/0f53c91545456c9d026e6298f4c5cde9fc6a5ccb>`_
- Merge pull request #12 from fedora-infra/feature/nickname-setting `09ad98118 <https://github.com/fedora-infra/tahrir-api/commit/09ad981182aa63e37623df2da989d69cecb600eb>`_
- Allow getting a user by id and nickname. `be32cb9c2 <https://github.com/fedora-infra/tahrir-api/commit/be32cb9c2cedccd015478f01e9fbb4c862b5ab08>`_
- Merge pull request #13 from fedora-infra/feature/nickname-getting `cda6a4611 <https://github.com/fedora-infra/tahrir-api/commit/cda6a4611d646e09f2f9f0e580b9a11bda2b5f5b>`_
- Fix typo. `c7c369750 <https://github.com/fedora-infra/tahrir-api/commit/c7c3697502044751d8e24ff1ee59b602eb9029f3>`_
- Update link to Tahrir in readme. `344fdbc11 <https://github.com/fedora-infra/tahrir-api/commit/344fdbc1147d9c09e86120630d40c7d2731708ed>`_
- Stop leaking sqlalchemy sessions.  Fixes #14. `ab1de52e7 <https://github.com/fedora-infra/tahrir-api/commit/ab1de52e7ce7d8f36e43d95c9fc2bc7013f79364>`_
- Merge pull request #15 from fedora-infra/feature/stop-session-leak `63dc66811 <https://github.com/fedora-infra/tahrir-api/commit/63dc66811981de3d39ea6d37d23b7df985b8380d>`_
- PEP8. `71c7cb91d <https://github.com/fedora-infra/tahrir-api/commit/71c7cb91d893c9b752553b758b4e3538539b2236>`_

0.2.0
-----

- Remove the need for a "tahrir.salt" config value. `3d44dc91f <https://github.com/fedora-infra/tahrir-api/commit/3d44dc91f61fdbc49b57714eb951bee52289cd86>`_
- Remove an old print statement. `bb5ecf9f0 <https://github.com/fedora-infra/tahrir-api/commit/bb5ecf9f043b1d0f2f114e73e52c094fe0a482c7>`_
- Merge pull request #10 from fedora-infra/feature/simple-salts `9a1e415c7 <https://github.com/fedora-infra/tahrir-api/commit/9a1e415c7d551da69f266b799c9aaa8bb3cae9ac>`_
- add initial alembic files, point at tahrir.db, and basic readme `e434673c7 <https://github.com/fedora-infra/tahrir-api/commit/e434673c7622156d014296cb6da827a62c786eb5>`_
- Add swap file extensions to .gitignore `1d6579c73 <https://github.com/fedora-infra/tahrir-api/commit/1d6579c738ba306f5e33c9fe50c8b9c186cd30ee>`_
- Make Alembic run migrations as a transaction, rolling back on OperationError. Also add a migration script to add a column. `f661a7c62 <https://github.com/fedora-infra/tahrir-api/commit/f661a7c6280d7d359aa58ed921ca16d73126e364>`_
- Print repr() of OperationalError. `5ae3e40e2 <https://github.com/fedora-infra/tahrir-api/commit/5ae3e40e26c48be1cf584276ebce74347740dd0c>`_
- Add 3 more Alembic scripts to complete Tahrir model changes for now. `46a4b2f59 <https://github.com/fedora-infra/tahrir-api/commit/46a4b2f5972c67668cf5f42e8983d680a2672b66>`_
- Merge branch 'feature/alembic' into develop `d33a96a31 <https://github.com/fedora-infra/tahrir-api/commit/d33a96a3169b3a8b2679527975361bb0308bcefa>`_
- Update models to match Alembic changes. `ab28f4c14 <https://github.com/fedora-infra/tahrir-api/commit/ab28f4c14782605f571f8451f4db0a4135682af2>`_
- Make created_on default values be the current datetime. `987aa7bcc <https://github.com/fedora-infra/tahrir-api/commit/987aa7bccfe8c11ff57566860b34484c0ce6286e>`_
- Alembic script to add created_by to invitations table. `d51427e9e <https://github.com/fedora-infra/tahrir-api/commit/d51427e9e11165cc01d2981725a7f560550ab2f5>`_
- Add invitations table created_by field to model. Fixes Tahrir #58. `55d8803d9 <https://github.com/fedora-infra/tahrir-api/commit/55d8803d9c3296b085f136f29a0e132fc1075aff>`_
- Merge branch 'feature/issue-58' into develop `6842648e4 <https://github.com/fedora-infra/tahrir-api/commit/6842648e44c38cb781825cbd64babddb6f90aba0>`_
- Make Alembic scripts properly include nullable args. (Thanks, @puiterwijk!) `47c14055a <https://github.com/fedora-infra/tahrir-api/commit/47c14055aab1970d0abd8b003cfe811b1c796794>`_
- Make issued_on in assertions table not nullable and set default to datetime.now. `57b03be29 <https://github.com/fedora-infra/tahrir-api/commit/57b03be29f7e68490d4ead4bc29b497c8cb8485b>`_
- Fix failing test (was failing on add_invitation). `1015377cd <https://github.com/fedora-infra/tahrir-api/commit/1015377cd5e16d390c89d0b19cd8fcbe6eaab758>`_
- Fix unicode warning thrown in tests (thanks @Qalthos!) `ee3b008bd <https://github.com/fedora-infra/tahrir-api/commit/ee3b008bd773d8472b60ecf213298c5f6c59e8a1>`_
- Add get_all_assertions and get_all_persons methods. `5a1e07ae2 <https://github.com/fedora-infra/tahrir-api/commit/5a1e07ae26d148fd90c54ab26e68068523555aa8>`_
- Fix get_assertions_by_email so it actually functions. `42fe14005 <https://github.com/fedora-infra/tahrir-api/commit/42fe14005c059f557d582c39c02db2463b0388b2>`_
- Add get_person_email and make person_exists take an email OR id. `f056f26d7 <https://github.com/fedora-infra/tahrir-api/commit/f056f26d7cb039855862b925d9c9d06d60b461e3>`_
- Merge pull request #11 from fedora-infra/feature/TahrirDatabase-improvements `e2b485c9e <https://github.com/fedora-infra/tahrir-api/commit/e2b485c9e5e14d15bd51625a2617178823de03c3>`_
