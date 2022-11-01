CAFE POS 프로그램입니다.

메뉴를 선택후 옵션을 선택하면  메뉴정보와 옵션정보 가격이 뜹니다.

결제시  주문이 됩니다.

주문정보가 DB에 저장되어 판매보기에서 오늘의 판매량과 메뉴별 
판매량을 확인할수있습니다.

재고관리에서 재료재고를 확인할수있고. 재료를 추가 주문가능.


(메뉴를 주문시 메뉴의 재료가 줄어듬)

선택취소시 메뉴와 옵션정보가 취소 됩니다.

이슈 - 메뉴를 주문하거나 재료를 주문시 버튼을 다시 눌러줘야 값이 바뀜


해결책- 수정하려고 했지만 해결책을 찾지 못했다.


DB

drop table coffee;
create table coffee(
coffeename varchar2(20),
coffeesize varchar2(10),
shot varchar2(10),
coffeetemp varchar2(10),
price number 
);
	

col coffeename for a20;
col coffeesize for a10;
col shot for a14;
col coffeetemp for a10;
col price for 99999;

commit;
select * from coffee;





drop table stock;
create table stock(
wondu number,
milk number,
sirup number,
berry number,
mango number,
green number,
black number,
choco number
);

col wondu for 999;
col milk for 999;
col sirup for 999;
col berry for 999;
col green for 999;
col black for 999;
col choco for 999;
col mango for 999;

insert into stock(wondu,milk,sirup,berry,mango,green,black,choco)
values(30,30,30,10,10,10,10,10);


commit;
select * from stock;
