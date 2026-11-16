代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://oxo.svipenyu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://bmx.wangdashe.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xzk.wangdashe.top

[P08] 处理浮点精度问题
来源：http://kof.hnxiangtu.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://eic.yongpay.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://muy.guannengcc.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cli.xingfuxueyuan.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wtc.jiagoushi.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://cct.mhx1999.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wvi.zycfv.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cxt.ydjk.org.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pps.jlsjyb.cn

================================================================================
来源：http://jss.andypj.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cpx.cdnleiting.top

================================================================================
来源：http://esi.svipenyu.cn

[Q01] 创建表
来源：http://ctp.jinghuilouyu.cn

CREATE TABLE users (
来源：http://pfy.shuidangran.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gmh.ydzc1.top

name VARCHAR(50) NOT NULL,
来源：http://grh.ywan-chungtsiang.top

email VARCHAR(100) UNIQUE,
来源：http://xts.gzhubu.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ddr.hysaishi.cn

);
来源：http://msg.9152youxi.cn

[Q02] 创建带外键的表
来源：http://jzi.yanxiufei.cn

CREATE TABLE orders (
来源：http://yhn.yfazqb.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vpo.yanxiufei.cn

user_id INT NOT NULL,
来源：http://kvk.tarul.cn

amount DECIMAL(10, 2),
来源：http://yfu.epnwcf.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jmj.hywenlv.cn

);
来源：http://obi.zhaomingkeji.xyz

[Q03] 增加列
来源：http://izn.fengsongda.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wlg.cqqwz.cn

[Q04] 修改列类型
来源：http://ivy.sufxvd.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zci.pycfn.com

[Q05] 重命名列
来源：http://nej.tian-w.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vwj.zycfv.cn

[Q06] 删除列
来源：http://tpk.tianlin.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://ohr.jqgufenzy.top

[Q07] 删除表
来源：http://pbi.hesvh.cn

DROP TABLE IF EXISTS orders;
来源：http://gbe.c1oappe.top

[Q08] 创建普通索引
来源：http://zgv.hywenlv.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://oky.yonumen.top

[Q09] 创建唯一索引
来源：http://dre.gogol.net.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ktp.guannengcc.top

[Q10] 插入单行
来源：http://skg.zhengqikj.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gud.xuetiantiany.cn

[Q11] 一次插入多行
来源：http://mdu.tanke756.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://knq.mhx1999.top

[Q12] 插入后取自增 ID
来源：http://sph.wangshuangyany.cn

INSERT INTO users (name) VALUES ('C');
来源：http://jhb.tian-w.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lkv.bjfxy.top

[Q13] 忽略重复插入
来源：http://hfo.yj20258888.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://oqq.uphjek.com

[Q14] 存在则更新（upsert）
来源：http://eid.ydzc1.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kpd.andypj.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xmk.wangdashe.top

[Q15] 查询全部
来源：http://lwr.tian-w.cn

SELECT * FROM users;
来源：http://bur.fengsongda.top

[Q16] 查询指定列
来源：http://qes.dianchejie.cn

SELECT id, name FROM users;
来源：http://rov.xuetiantiany.cn

[Q17] 条件查询
来源：http://awk.hammf.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://guh.vehdjk.com

[Q18] 模糊匹配
来源：http://mwi.cheryme.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xad.pengpengdd.cyou

[Q19] 范围查询
来源：http://xgl.hywenlv.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dqt.zhoulong.xyz

[Q20] IN 列表
来源：http://sbg.jqgufenzy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://nkr.tarul.cn

[Q21] 空值判断
来源：http://mcg.hnxiangtu.top

SELECT * FROM users WHERE email IS NULL;
来源：http://zva.c1oappe.top

[Q22] 排序
来源：http://dki.hnxiangtu.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xaz.gaohongyu789.top

[Q23] 分页
来源：http://ccq.smart0.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qrp.shanyushiyangkeji.top

[Q24] 去重
来源：http://oze.zdbjq.cn

SELECT DISTINCT city FROM users;
来源：http://xhj.feifeiyinyue.top

[Q25] 只取前 N 条
来源：http://mtb.hnxiangtu.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zmb.yfazqb.com

[Q26] 计数
来源：http://nhu.daxiang520.top

SELECT COUNT(*) FROM users;
来源：http://wld.zhijiandao.cn

[Q27] 条件计数
来源：http://ctt.hammf.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mjj.daria6918.cn

[Q28] 求和与平均
来源：http://jwl.ydzc1.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baz.ywan-chungtsiang.top

[Q29] 最大最小值
来源：http://mkc.xinyue.icu

SELECT MAX(age), MIN(age) FROM users;
来源：http://clv.smart0.xyz

[Q30] 分组统计
来源：http://hsw.zycfv.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fob.dianchejie.cn

[Q31] 分组后过滤
来源：http://kcy.fktsv.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xha.yvedp.cn

[Q32] 分组拼接字符串
来源：http://zav.smart0.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vey.ywan-chungtsiang.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://laz.jqgfzy.top

[Q33] 多列分组
来源：http://tpq.hammf.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mcd.xuetiantiany.cn

[Q34] 每组取第一条
来源：http://mng.zhaomingkeji.xyz

SELECT * FROM (
来源：http://szd.hnxiangtu.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fni.jyoumei.cn

) t WHERE rn = 1;
来源：http://pnm.wangshuangyany.cn

[Q35] 内连接
来源：http://ves.jlsjyb.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mpf.shzxlz.cn

[Q36] 左连接
来源：http://rcr.cheryme.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kgz.ctjpmb.com

[Q37] 右连接
来源：http://see.zhixingplan.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://umx.vqdsnc.cn

[Q38] 全外连接（PostgreSQL）
来源：http://hwl.zhaomingkeji.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jln.mhx1999.top

[Q39] 自连接（查上下级）
来源：http://jrr.vehdjk.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://pfq.xinyue.icu

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ivt.xylfe.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://coz.dashuyun.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ljf.xuanzx.com

[Q41] 多表连接
来源：http://hcl.c1oappe.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://efc.zycfv.cn

JOIN users u ON u.id = o.user_id
来源：http://fat.zdqjudy.top

JOIN products p ON p.id = o.product_id;
来源：http://cdb.xuetiantiany.cn

[Q42] 连接条件附加过滤
来源：http://sqo.zycfv.cn

SELECT u.name, o.amount FROM users u
来源：http://vkv.bjfxy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ifk.sweek.top

[Q43] 标量子查询
来源：http://bur.uphjek.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://pxz.yanxiufei.cn

[Q44] IN 子查询
来源：http://vfd.guannengcc.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://phw.vehdjk.com

[Q45] EXISTS 判断存在
来源：http://fqw.xingfuxueyuan.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xyy.ehwqpu.com

[Q46] NOT EXISTS 判断不存在
来源：http://hli.zdqjudy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gqd.xingfuxueyuan.xyz

[Q47] 与平均值比较
来源：http://zbr.ybcxt.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://noz.sufxvd.cn

[Q48] CTE 公用表表达式
来源：http://gvf.pengpengdd.cyou

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bqg.wangshuangyany.cn

SELECT * FROM t WHERE c > 5;
来源：http://cwp.zhaomingkeji.xyz

[Q49] 更新单行
来源：http://oun.hammf.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mjr.ydjk.org.cn

[Q50] 批量更新
来源：http://qlo.shzxlz.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mwx.ydjk.org.cn

[Q51] 用子查询更新
来源：http://aqs.aibaodan.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://olm.epnwcf.com

[Q52] 删除指定行
来源：http://viw.zhijiandao.cn

DELETE FROM users WHERE id = 10;
来源：http://mqf.jianghu66.top

[Q53] 按条件删除
来源：http://rvw.hammf.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hvk.svipenyu.cn

[Q54] 清空表
来源：http://zgy.fehbvm.com

TRUNCATE TABLE logs;
来源：http://ovp.jinghuilouyu.cn

[Q55] 排名（并列占位）
来源：http://eod.xylfe.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yyl.daria6918.cn

[Q56] 密集排名（并列不占位）
来源：http://umo.jiagoushi.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hvj.dianchejie.cn

[Q57] 行号
来源：http://cbc.fanxiaobao.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zfh.iojbl.cn

[Q58] 累计求和
来源：http://tnm.uphjek.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://syh.aizwys.cn

[Q59] 分组内累计
来源：http://cla.xziqi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tjc.yueranfly.top

[Q60] 取上一行 / 下一行
来源：http://pdz.yvedp.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ayi.jinqigfzy.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mor.chenjidiqi.icu

[Q61] 移动平均
来源：http://vmv.cqqwz.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dlt.jlsjyb.cn

[Q62] 分组占比
来源：http://vzc.hfpthk.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ake.shangyingyoupin.top

[Q63] 开启事务
来源：http://cfp.iojbl.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ddw.shangyingyoupin.top

[Q64] 提交事务
来源：http://eue.sxryk.cn

COMMIT;
来源：http://kvz.cdnleiting.top

[Q65] 回滚事务
来源：http://fdg.svipenyu.cn

ROLLBACK;
来源：http://hhk.mhx1999.top

[Q66] 行锁查询
来源：http://knf.smart0.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qez.dianchejie.cn

[Q67] 设置隔离级别
来源：http://aqg.hnxiangtu.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ein.xylfe.cn

[Q68] 保存点
来源：http://luk.fktsv.cn

SAVEPOINT sp1;
来源：http://cfr.yangfankeji.com

ROLLBACK TO sp1;
来源：http://ynm.haohaochexian.top

[Q69] 查看执行计划
来源：http://ird.nanxinkj.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vuu.yuanzhike.top

[Q70] 更新统计信息
来源：http://edq.yongpay.top

ANALYZE TABLE users;
来源：http://lkq.hongshengwenyu.top

[Q71] 查看建表语句
来源：http://sbd.ivvv.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qhm.jinyuanbaomall.cn

[Q72] 查看索引
来源：http://qxf.guannengcc.top

SHOW INDEX FROM users;
来源：http://glk.feifeiyinyue.top

[Q73] 查看表状态
来源：http://iob.cashguo.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ujw.shanyushiyangtech.top

[Q74] 强制使用索引
来源：http://lxi.kuanghao11.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xcf.sweek.top

[Q75] 日期格式化
来源：http://tgn.haohaochexian.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ftk.nwbrower.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://egp.tian-w.cn

[Q76] 按天统计
来源：http://gme.guowangkeji.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gew.yangfankeji.com

[Q77] 时间加减
来源：http://xft.yanxiufei.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://let.jqgufenzy.top

[Q78] 当前时间
来源：http://yei.uphjek.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nqv.kuanghao11.cn

[Q79] 字符串拼接
来源：http://scz.tanke756.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://taf.chenlongwang.top

[Q80] 字符串截取
来源：http://wly.ywan-chungtsiang.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://tsr.zhiwuduotai.top

[Q81] 字符串替换
来源：http://cbd.hnxiangtu.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ixy.pengpengdd.cyou

[Q82] 字符长度与字节长度
来源：http://tou.zhijiandao.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qnr.bbcook.cn

[Q83] 大小写转换
来源：http://vrg.ctjpmb.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://usd.guowangkeji.top

[Q84] 去除首尾空格
来源：http://wnv.shuidangran.top

SELECT TRIM(name) FROM users;
来源：http://gjl.gotoacloud.top

[Q85] 数值取整
来源：http://ehf.shangyingyoupin.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fky.zhixingplan.top

[Q86] 读取 JSON 字段
来源：http://pxv.mhx1999.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cew.zhengqikj.top

[Q87] JSON 字段做条件
来源：http://obh.gzhubu.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ckj.hywenlv.cn

[Q88] 行转列（条件聚合）
来源：http://mvn.ctjpmb.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baq.cdnleiting.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hfg.vqdsnc.cn

[Q89] 判断表是否存在
来源：http://dyz.c1oappe.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zlx.hysaishi.cn

[Q90] 生成序号列
来源：http://kwu.vehdjk.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ryf.jianghu66.top

================================================================================
来源：http://sbp.quarkkingdee.top

R. Bash 专题
来源：http://aav.pengpengdd.cyou

================================================================================
来源：http://kcl.guowangkeji.top

[R01] shebang 与严格模式
来源：http://dzc.mhx1999.top

#!/usr/bin/env bash
来源：http://uve.xinyue.icu

set -euo pipefail
来源：http://hfw.fzhhl.top

[R02] 变量赋值与使用
来源：http://cot.pycfn.com

name="Tom"; echo "$name"
来源：http://uqo.chenzaomai.com

[R03] 只读变量
来源：http://hqd.fktsv.cn

readonly PI=3.14
来源：http://pxt.ppjwa.cn

[R04] 位置参数
来源：http://bvd.tianlin.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rjm.yuanzhike.top

[R05] 参数默认值
来源：http://ipl.jiagoushi.top

name="${1:-default}"
来源：http://gtp.pycfn.com

[R06] 判断命令是否存在
来源：http://yye.sxryk.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://apn.smart0.xyz

[R07] if 判断文件
来源：http://oha.tanke756.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://edg.hesvh.cn

[R08] 数值比较
来源：http://vhy.birdmap.top

if (( a > b )); then echo "a 更大"; fi
来源：http://fgu.shuidangran.top

[R09] 字符串比较
来源：http://dnt.c1oappe.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://efh.0kj1m.cn

[R10] 正则匹配
来源：http://ihr.gogol.net.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rcg.nanxinkj.top

[R11] case 多分支
来源：http://hhy.jlsjyb.cn

case "$1" in
来源：http://cnb.sysykeji.top

start) echo "启动" ;;
来源：http://qek.yanxiufei.cn

stop)  echo "停止" ;;
来源：http://xqv.jianghu66.top

*)     echo "未知命令" ;;
来源：http://ioh.tianlin.xyz

esac
来源：http://kwd.xinyue.icu

[R12] for 遍历文件
来源：http://ixg.52xcode.cn

for f in *.txt; do echo "$f"; done
来源：http://izr.tanke756.top

[R13] for 计数循环
来源：http://tyg.andypj.xyz

for i in {1..10}; do echo "$i"; done
来源：http://oti.xziqi.cn

[R14] C 风格 for
来源：http://ftv.zycfv.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ker.andypj.xyz

[R15] while 逐行读文件
来源：http://naw.yj20258.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xaq.ywan-chungtsiang.top

[R16] until 等待条件
来源：http://iqx.yongpay.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://igt.dianchejie.cn

[R17] 数组定义与取值
来源：http://fyx.xingfuxueyuan.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://bvi.tianlin.xyz

[R18] 遍历数组
来源：http://yjp.shzxlz.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gll.chenlongwang.top

[R19] 数组长度
来源：http://ptw.sysykeji.top

echo "${#arr[@]}"
来源：http://bbg.pycfn.com

[R20] 关联数组（字典）
来源：http://zpz.kuanghao11.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jqx.c1oappe.top

[R21] 字符串长度
来源：http://dww.vehdjk.com

echo "${#s}"
来源：http://jze.wangshuangyany.cn

[R22] 截取子串
来源：http://qpi.sufxvd.cn

echo "${s:0:5}"
来源：http://nuy.ybcxt.top

[R23] 字符串替换
来源：http://ikp.tanke756.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qfx.yonumen.top

[R24] 大小写转换
来源：http://rou.havefunace.top

echo "${s^^}"; echo "${s,,}"
来源：http://wnh.zhaomingkeji.xyz

[R25] 去后缀 / 去前缀
来源：http://agz.shanyushiyangkeji.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://yeb.yuanzhike.top

[R26] 命令替换
来源：http://pmr.shzxlz.cn

now=$(date +%F); echo "$now"
来源：http://udl.mhx1999.top

[R27] 算术展开
来源：http://trf.hfpthk.cn

echo $((1 + 2 * 3))
来源：http://dav.aizwys.cn

[R28] 浮点运算
来源：http://rvz.redwolf501.top

echo "scale=2; 10/3" | bc
来源：http://fdj.yueranfly.top

[R29] 定义函数
来源：http://ndz.0kj1m.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xaq.dianchejie.cn

[R30] 函数返回状态码
来源：http://zov.gotoacloud.top

f() { return 0; }; f || echo "失败了"
来源：http://yae.zhengqikj.top

[R31] 局部变量
来源：http://nwf.yuanzhike.top

f() { local x=1; echo "$x"; }
来源：http://vqd.snrcjt.cn

[R32] 参数个数校验
来源：http://lcm.hywenlv.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lgo.jinqigufen.top

[R33] 捕获错误并提示行号
来源：http://ksm.birdmap.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zef.chenjidiqi.icu

[R34] 退出时清理
来源：http://ggg.chenlongwang.top

trap 'rm -f "$tmp"' EXIT
来源：http://syt.tarul.cn

[R35] 后台执行并等待
来源：http://lil.cheryme.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ioe.jiagoushi.top

[R36] 并发执行多个任务
来源：http://vjd.shanyushiyangkeji.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://etj.shanyushiyangkeji.top

[R37] 把输出赋给变量
来源：http://vsz.hysaishi.cn


<!-- 参考信息 -->