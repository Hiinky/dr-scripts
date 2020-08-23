## dr-lich options list

long, but not complete

### bare bones
No matter if only use lich for go2 travel magic or have customized every possible option, these fields are universally helpful.
script | yaml_field | explanation
------------ | ------------ | -------------
many | hometown | Some possible options: Crossing, Leth Deriel, Riverhaven, Therenborough, Rossman's Landing, Langenfirth, Throne City, Shard, Hibarnhvidar, Boar Clan, Ain Ghazal, Fang Cove, Ratha, Aesry, Mer'Kresh, Muspar'i, Hara'jaal
many | safe_room | A room number of your choosing. Best practice is a quiet room outside justice and _never_ a public room where people try to socialize.  It is extremely annoying to watch and bad manners to spam.
go2/bescort | footwear | If defined, go2 will remove shoes before wearing ice skates when traveling the Forfedhar ice road.  Skates are available at the pond in Crossing during Winter or from players during the other seasons.  Highly recommended for saving time and your character's life.
go2/bescort | bescort_fare_handling | Defaults to false.  If true, will attempt to pull money from the nearest bank if you have no money for fares.  Can snag if you still have no funds at that bank but very useful if you remember to deposit a few plat in the usual places like Lang, Haven, or Leth.
go2/bescort | bescort_hide | Defaults to true.  If false, your character will not hide when on the ferries and suchlike.
go2/bescort | shard_thief_password | Optional field only useful to thieves in Shard who know their password.


### universal magic settings
Magic is sprinkled in many places through the lich dependency set of scripts and the majority use these common fields.
yaml_field | explanation
------------ | -------------
cambrinth | The exact adjective and noun of your cambrinth item.
cambrinth_cap | Numerical value your cambrinth holds such as 16.  It is important to get this number exact so the system can use while worn when applicable.  Formula to use cambrinth while worn is `(capacity * 2) + 100` so an incorrect cap can cause trouble.
stored_cambrinth | Defaults to false.  Should your cambrinth be worn or stored?
cambrinth_items:
- name:
  cap:
  stored: |
