代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gqvvempyv.sHtML

[Q30] 分组统计
来源：http://www.share.vehdjk.com/Article/details/gitjysjto.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.vehdjk.com/Article/details/gpgwhsocr.sHtML

[Q31] 分组后过滤
来源：http://baike.sjlbkw.cn/Article/details/gttaznrqw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fktsv.cn/Article/details/gooljaebt.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.sjlbkw.cn/Article/details/gvoaaiwui.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fktsv.cn/Article/details/gaukctfsj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.tarul.cn/Article/details/gzhnwndss.sHtML

[Q33] 多列分组
来源：http://read.share.bbcook.cn/Article/details/ggslzxbff.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fktsv.cn/Article/details/gesqpyqox.sHtML

[Q34] 每组取第一条
来源：http://blog.epnwcf.com/Article/details/gnvgqhqwi.sHtML

SELECT * FROM (
来源：http://wap.yfazqb.com/Article/details/gbhxstzlb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.tarul.cn/Article/details/grnjuvegc.sHtML

) t WHERE rn = 1;
来源：http://mobile.vehdjk.com/Article/details/gtbukzrbw.sHtML

[Q35] 内连接
来源：http://www.m.share.epnwcf.com/Article/details/guugwarai.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.bbcook.cn/Article/details/grpzgcnuj.sHtML

[Q36] 左连接
来源：http://3g.yfazqb.com/Article/details/gjnoixcoq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.bbcook.cn/Article/details/gyzixxjcw.sHtML

[Q37] 右连接
来源：http://wap.fktsv.cn/Article/details/gyapfkjls.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.vehdjk.com/Article/details/gzoiwlnmp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fktsv.cn/Article/details/gdrhiqjzf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fktsv.cn/Article/details/gpwazbyey.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.tarul.cn/Article/details/gepdjsdue.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.yfazqb.com/Article/details/ginlfncso.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fktsv.cn/Article/details/gwppkswlk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.yfazqb.com/Article/details/gxvttnukl.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.yfazqb.com/Article/details/guzaucctc.sHtML

[Q41] 多表连接
来源：http://mobile.vehdjk.com/Article/details/gchxgwvnu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.bbcook.cn/Article/details/gshdpylso.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.yfazqb.com/Article/details/gcpvymsik.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.bbcook.cn/Article/details/gvnthlchj.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.sjlbkw.cn/Article/details/gkpythgps.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.epnwcf.com/Article/details/gnnjgnysq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.tarul.cn/Article/details/gzvtlpmyl.sHtML

[Q43] 标量子查询
来源：http://m.share.epnwcf.com/Article/details/gdtskmbad.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.bbcook.cn/Article/details/gnectkrvy.sHtML

[Q44] IN 子查询
来源：http://m.share.yfazqb.com/Article/details/gmuhsuzsu.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.tarul.cn/Article/details/grgytbzzm.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fktsv.cn/Article/details/gwtwsszsi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.yfazqb.com/Article/details/gsryvetmg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fktsv.cn/Article/details/gyyndecdn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.bbcook.cn/Article/details/gztrimnmq.sHtML

[Q47] 与平均值比较
来源：http://blog.tarul.cn/Article/details/gxhcrfznu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.tarul.cn/Article/details/glrfvbxge.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.tarul.cn/Article/details/gtuftpydq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.sjlbkw.cn/Article/details/ghtnintru.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.vehdjk.com/Article/details/guouamhhe.sHtML

[Q49] 更新单行
来源：http://wap.fktsv.cn/Article/details/gdozpjney.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.vehdjk.com/Article/details/gxtfvaynt.sHtML

[Q50] 批量更新
来源：http://3g.fktsv.cn/Article/details/gmyglvdlc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.vehdjk.com/Article/details/ggbzdbmun.sHtML

[Q51] 用子查询更新
来源：http://m.share.epnwcf.com/Article/details/gqiteyevp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.tarul.cn/Article/details/grctyoaoo.sHtML

[Q52] 删除指定行
来源：http://www.share.fktsv.cn/Article/details/gomttntmr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.tarul.cn/Article/details/gekjvcsku.sHtML

[Q53] 按条件删除
来源：http://www.m.share.yfazqb.com/Article/details/gkincuqir.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.sjlbkw.cn/Article/details/grzbgwses.sHtML

[Q54] 清空表
来源：http://3g.vehdjk.com/Article/details/gtzibssbh.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fktsv.cn/Article/details/gwfclbtjy.sHtML

[Q55] 排名（并列占位）
来源：http://3g.vehdjk.com/Article/details/gzcrdovex.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.yfazqb.com/Article/details/gecrofpzr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.vehdjk.com/Article/details/gqpkgwpdq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.sjlbkw.cn/Article/details/gcakdwrfb.sHtML

[Q57] 行号
来源：http://read.share.fktsv.cn/Article/details/goglwjest.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.bbcook.cn/Article/details/ggglmqonh.sHtML

[Q58] 累计求和
来源：http://read.share.epnwcf.com/Article/details/gdcaxjydz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.yfazqb.com/Article/details/ggvwbtcyj.sHtML

[Q59] 分组内累计
来源：http://baike.yfazqb.com/Article/details/gkvrdkogm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.yfazqb.com/Article/details/gicbbbufn.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.tarul.cn/Article/details/gimsaokhd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.tarul.cn/Article/details/graescdcp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fktsv.cn/Article/details/gordgpcsb.sHtML

[Q61] 移动平均
来源：http://m.share.fktsv.cn/Article/details/grehcgodv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fktsv.cn/Article/details/gumlztsiy.sHtML

[Q62] 分组占比
来源：http://3g.tarul.cn/Article/details/gcydariqv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.tarul.cn/Article/details/guazrwogo.sHtML

[Q63] 开启事务
来源：http://mobile.bbcook.cn/Article/details/gulrwygae.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.yfazqb.com/Article/details/glgijauhz.sHtML

[Q64] 提交事务
来源：http://m.share.tarul.cn/Article/details/gefqcxdgs.sHtML

COMMIT;
来源：http://blog.sjlbkw.cn/Article/details/gghvxysad.sHtML

[Q65] 回滚事务
来源：http://3g.tarul.cn/Article/details/ggwdoighx.sHtML

ROLLBACK;
来源：http://m.share.fktsv.cn/Article/details/guesuzlbd.sHtML

[Q66] 行锁查询
来源：http://www.blog.tarul.cn/Article/details/girgkscpn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.yfazqb.com/Article/details/gnbuvzumd.sHtML

[Q67] 设置隔离级别
来源：http://mobile.bbcook.cn/Article/details/ggjintfpu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.vehdjk.com/Article/details/gbhswxixi.sHtML

[Q68] 保存点
来源：http://3g.sjlbkw.cn/Article/details/gzycfqcjd.sHtML

SAVEPOINT sp1;
来源：http://wap.sjlbkw.cn/Article/details/gruvyswpo.sHtML

ROLLBACK TO sp1;
来源：http://baike.tarul.cn/Article/details/gkmfxkmwk.sHtML

[Q69] 查看执行计划
来源：http://mobile.bbcook.cn/Article/details/gzchurazc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.bbcook.cn/Article/details/gprszrhrw.sHtML

[Q70] 更新统计信息
来源：http://blog.epnwcf.com/Article/details/gxkgmepmb.sHtML

ANALYZE TABLE users;
来源：http://blog.vehdjk.com/Article/details/gmukwoohy.sHtML

[Q71] 查看建表语句
来源：http://blog.vehdjk.com/Article/details/ghazkmdxm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fktsv.cn/Article/details/glvzkfici.sHtML

[Q72] 查看索引
来源：http://baike.yfazqb.com/Article/details/gkqkrahjk.sHtML

SHOW INDEX FROM users;
来源：http://mobile.vehdjk.com/Article/details/groztslxi.sHtML

[Q73] 查看表状态
来源：http://mobile.fktsv.cn/Article/details/gayobaick.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.yfazqb.com/Article/details/gndrsghuo.sHtML

[Q74] 强制使用索引
来源：http://read.share.yfazqb.com/Article/details/gzgkemrds.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.tarul.cn/Article/details/gewydttmj.sHtML

[Q75] 日期格式化
来源：http://wap.fktsv.cn/Article/details/gcmszjebh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.epnwcf.com/Article/details/gihcbvcdq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.bbcook.cn/Article/details/gnbcvbgbo.sHtML

[Q76] 按天统计
来源：http://m.share.tarul.cn/Article/details/govcrmpzk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.tarul.cn/Article/details/gfpgcpnmn.sHtML

[Q77] 时间加减
来源：http://www.blog.yfazqb.com/Article/details/gmitbfakc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.sjlbkw.cn/Article/details/gzhpbagju.sHtML

[Q78] 当前时间
来源：http://www.m.share.bbcook.cn/Article/details/gaymyichf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.sjlbkw.cn/Article/details/gptqdrolg.sHtML

[Q79] 字符串拼接
来源：http://blog.vehdjk.com/Article/details/gwqlbknxo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fktsv.cn/Article/details/gouhbhgcy.sHtML

[Q80] 字符串截取
来源：http://read.share.yfazqb.com/Article/details/gofpaepcl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/ggakzufvg.sHtML

[Q81] 字符串替换
来源：http://www.blog.fktsv.cn/Article/details/gccrizyme.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.yfazqb.com/Article/details/gtwfggycg.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.vehdjk.com/Article/details/gbrygjgae.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fktsv.cn/Article/details/gngfzorbb.sHtML

[Q83] 大小写转换
来源：http://www.blog.yfazqb.com/Article/details/gqivacqaw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.vehdjk.com/Article/details/grvadedfe.sHtML

[Q84] 去除首尾空格
来源：http://3g.bbcook.cn/Article/details/gmoexxfwc.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/ghnpsjlqs.sHtML

[Q85] 数值取整
来源：http://3g.yfazqb.com/Article/details/gwiprfmlr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.tarul.cn/Article/details/ghfvshbhu.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fktsv.cn/Article/details/grhekvunp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.yfazqb.com/Article/details/ggopgrhdo.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.sjlbkw.cn/Article/details/gnghpzsag.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.epnwcf.com/Article/details/gulsdpmuk.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.tarul.cn/Article/details/gueguzecc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.tarul.cn/Article/details/gvsyxiqxg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gceinbxyb.sHtML

[Q89] 判断表是否存在
来源：http://blog.epnwcf.com/Article/details/gjunciaib.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.tarul.cn/Article/details/gzjfxuwot.sHtML

[Q90] 生成序号列
来源：http://mobile.tarul.cn/Article/details/gblsumzad.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.sjlbkw.cn/Article/details/gcwnrzddd.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gimbdwocs.sHtML

R. Bash 专题
来源：http://mobile.tarul.cn/Article/details/gslzoveam.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gmzkmhtjz.sHtML

[R01] shebang 与严格模式
来源：http://3g.yfazqb.com/Article/details/gbletcqli.sHtML

#!/usr/bin/env bash
来源：http://read.share.epnwcf.com/Article/details/ggwhyalwc.sHtML

set -euo pipefail
来源：http://www.blog.yfazqb.com/Article/details/gbvqebmgi.sHtML

[R02] 变量赋值与使用
来源：http://blog.fktsv.cn/Article/details/gylhbzfbb.sHtML

name="Tom"; echo "$name"
来源：http://read.share.tarul.cn/Article/details/gbyfiplvy.sHtML

[R03] 只读变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gsbgqxhjo.sHtML

readonly PI=3.14
来源：http://blog.vehdjk.com/Article/details/gjcipylss.sHtML

[R04] 位置参数
来源：http://www.share.yfazqb.com/Article/details/gcsetzwcf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.tarul.cn/Article/details/ggtpxjrtw.sHtML

[R05] 参数默认值
来源：http://baike.vehdjk.com/Article/details/gmkvztmzt.sHtML

name="${1:-default}"
来源：http://blog.bbcook.cn/Article/details/glhzozfzn.sHtML

[R06] 判断命令是否存在
来源：http://blog.epnwcf.com/Article/details/gudiiqrvb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fktsv.cn/Article/details/gjmxjchtb.sHtML

[R07] if 判断文件
来源：http://read.share.bbcook.cn/Article/details/gmxypatju.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.epnwcf.com/Article/details/ggzbtkwns.sHtML

[R08] 数值比较
来源：http://read.share.fktsv.cn/Article/details/gldhqbftc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fktsv.cn/Article/details/gbqvfommc.sHtML

[R09] 字符串比较
来源：http://read.share.tarul.cn/Article/details/gmyiypqbf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.sjlbkw.cn/Article/details/ghguswbyl.sHtML

[R10] 正则匹配
来源：http://www.m.share.bbcook.cn/Article/details/gencdkrup.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.bbcook.cn/Article/details/gxveywwfh.sHtML

[R11] case 多分支
来源：http://wap.bbcook.cn/Article/details/govhsxweo.sHtML

case "$1" in
来源：http://read.share.sjlbkw.cn/Article/details/gpmpxlgoh.sHtML

start) echo "启动" ;;
来源：http://www.m.share.epnwcf.com/Article/details/geqipsonm.sHtML

stop)  echo "停止" ;;
来源：http://3g.bbcook.cn/Article/details/ginkcoztt.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fktsv.cn/Article/details/ghgvjqhxz.sHtML

esac
来源：http://www.m.share.vehdjk.com/Article/details/gxlresceg.sHtML

[R12] for 遍历文件
来源：http://baike.tarul.cn/Article/details/gvpcbjsqv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.bbcook.cn/Article/details/gzgqptpff.sHtML

[R13] for 计数循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gygbbcoqi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.epnwcf.com/Article/details/gghgkrkqz.sHtML

[R14] C 风格 for
来源：http://blog.bbcook.cn/Article/details/gorhthbcb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.bbcook.cn/Article/details/gbiocyeiv.sHtML

[R15] while 逐行读文件
来源：http://blog.epnwcf.com/Article/details/gzllsvvjx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fktsv.cn/Article/details/gesnydbmk.sHtML

[R16] until 等待条件
来源：http://mobile.epnwcf.com/Article/details/gwgtvgdqs.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fktsv.cn/Article/details/gpeyuvflj.sHtML

[R17] 数组定义与取值
来源：http://www.share.bbcook.cn/Article/details/gwvmjstrp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.yfazqb.com/Article/details/guzmavukq.sHtML

[R18] 遍历数组
来源：http://read.share.epnwcf.com/Article/details/ghlkqrxex.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.bbcook.cn/Article/details/grxtxyuiy.sHtML

[R19] 数组长度
来源：http://blog.fktsv.cn/Article/details/goffqyjtw.sHtML

echo "${#arr[@]}"
来源：http://mobile.bbcook.cn/Article/details/gilcbgqnv.sHtML

[R20] 关联数组（字典）
来源：http://mobile.epnwcf.com/Article/details/gajwebfkz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.sjlbkw.cn/Article/details/geusbexvr.sHtML

[R21] 字符串长度
来源：http://m.share.yfazqb.com/Article/details/gdvacqvtu.sHtML

echo "${#s}"
来源：http://wap.tarul.cn/Article/details/gznapwhio.sHtML

[R22] 截取子串
来源：http://www.m.share.tarul.cn/Article/details/ghaluosim.sHtML

echo "${s:0:5}"
来源：http://wap.tarul.cn/Article/details/gddwqyoko.sHtML

[R23] 字符串替换
来源：http://3g.yfazqb.com/Article/details/gawoaxywf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.epnwcf.com/Article/details/gfwsdhpgx.sHtML

[R24] 大小写转换
来源：http://www.m.share.fktsv.cn/Article/details/gplaoeoxk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.yfazqb.com/Article/details/gbuyanxow.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.vehdjk.com/Article/details/gbicfrviu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.sjlbkw.cn/Article/details/gntetucbj.sHtML

[R26] 命令替换
来源：http://www.m.share.epnwcf.com/Article/details/gtybvhhfz.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.tarul.cn/Article/details/gujwvodoa.sHtML

[R27] 算术展开
来源：http://www.share.sjlbkw.cn/Article/details/gelphtnsn.sHtML

echo $((1 + 2 * 3))
来源：http://baike.sjlbkw.cn/Article/details/gvmzlzvts.sHtML

[R28] 浮点运算
来源：http://www.blog.tarul.cn/Article/details/ghnwvjlxz.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.epnwcf.com/Article/details/goprzsqnu.sHtML

[R29] 定义函数
来源：http://baike.sjlbkw.cn/Article/details/grhvahxcy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.vehdjk.com/Article/details/gcqyludci.sHtML

[R30] 函数返回状态码
来源：http://www.blog.yfazqb.com/Article/details/gzyhayrdd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.bbcook.cn/Article/details/ghlzovdjr.sHtML

[R31] 局部变量
来源：http://baike.sjlbkw.cn/Article/details/geconrvjt.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.yfazqb.com/Article/details/ggrwikifx.sHtML

[R32] 参数个数校验
来源：http://baike.fktsv.cn/Article/details/gqtwxjpxu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.vehdjk.com/Article/details/ggkcrjgqk.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.vehdjk.com/Article/details/gsvtedlnd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.sjlbkw.cn/Article/details/ggcxlnewn.sHtML

[R34] 退出时清理
来源：http://mobile.yfazqb.com/Article/details/gqjqhyujp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.epnwcf.com/Article/details/gtxwdfqdc.sHtML

[R35] 后台执行并等待
来源：http://blog.fktsv.cn/Article/details/giobpnofb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.bbcook.cn/Article/details/gzgjiiuyh.sHtML

[R36] 并发执行多个任务
来源：http://www.share.sjlbkw.cn/Article/details/gsaijblrv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fktsv.cn/Article/details/ggodnmmhq.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.tarul.cn/Article/details/gdzmnyxuh.sHtML

files=$(ls -1)
来源：http://mobile.yfazqb.com/Article/details/gbngqqkqj.sHtML

[R38] 管道串联
来源：http://mobile.epnwcf.com/Article/details/gewrnlxlp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.sjlbkw.cn/Article/details/gstmdxhva.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.epnwcf.com/Article/details/gtpgldlae.sHtML

cmd > out.log 2>&1
来源：http://mobile.tarul.cn/Article/details/gxnguwbjm.sHtML

[R40] 追加写日志
来源：http://read.share.tarul.cn/Article/details/gcwyaocuq.sHtML

echo "log" >> out.log
来源：http://3g.tarul.cn/Article/details/gfjgymbqc.sHtML

[R41] 丢弃输出
来源：http://www.share.vehdjk.com/Article/details/gdnjqgxsh.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.tarul.cn/Article/details/gqttqyykl.sHtML

[R42] 输入重定向
来源：http://blog.sjlbkw.cn/Article/details/gxgvvsunp.sHtML

wc -l < a.txt
来源：http://wap.fktsv.cn/Article/details/gjzsnoclb.sHtML

[R43] 按名字查找文件
来源：http://wap.fktsv.cn/Article/details/gtjiintzz.sHtML

find . -name "*.log" -type f
来源：http://m.share.epnwcf.com/Article/details/gpacjneas.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.bbcook.cn/Article/details/ghwzxzdnt.sHtML

find . -mtime -7 -type f
来源：http://baike.vehdjk.com/Article/details/gmurtytgo.sHtML

[R45] 批量删除
来源：http://wap.bbcook.cn/Article/details/gsogxuwbg.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.yfazqb.com/Article/details/gppsjjodf.sHtML

[R46] 递归替换文件内容
来源：http://m.share.vehdjk.com/Article/details/gklzznpik.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.bbcook.cn/Article/details/gmbhdvnta.sHtML

[R47] sed 单行替换
来源：http://mobile.epnwcf.com/Article/details/gldosaldi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.tarul.cn/Article/details/gpzlnnszh.sHtML

[R48] awk 取指定列
来源：http://www.m.share.yfazqb.com/Article/details/ggqwlxqmy.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.epnwcf.com/Article/details/gdxfubgzp.sHtML

[R49] awk 带条件
来源：http://www.blog.epnwcf.com/Article/details/ghmujdfzw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.vehdjk.com/Article/details/gbxbpneyg.sHtML

[R50] awk 求和
来源：http://3g.bbcook.cn/Article/details/gmlufpsfl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fktsv.cn/Article/details/gcgrxtrlr.sHtML

[R51] 排序去重取前几
来源：http://mobile.fktsv.cn/Article/details/gcwjacruk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.tarul.cn/Article/details/ggqoajdiv.sHtML

[R52] 统计行数
来源：http://www.blog.fktsv.cn/Article/details/gssvziwxi.sHtML

wc -l a.txt
来源：http://blog.yfazqb.com/Article/details/gbjfkzqjn.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.bbcook.cn/Article/details/glfjvjlyy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.yfazqb.com/Article/details/glbcczjgf.sHtML

[R54] 比较两个文件
来源：http://wap.yfazqb.com/Article/details/gmeeivuwk.sHtML

diff a.txt b.txt
来源：http://blog.yfazqb.com/Article/details/gnifghoec.sHtML

[R55] 压缩与解压
来源：http://3g.epnwcf.com/Article/details/gvvdipemo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.sjlbkw.cn/Article/details/gpvruyoih.sHtML

[R56] 远程拷贝
来源：http://3g.tarul.cn/Article/details/gvvxswkpp.sHtML

scp file user@host:/path/
来源：http://www.blog.sjlbkw.cn/Article/details/gdhmebvzl.sHtML

[R57] 远程执行命令
来源：http://read.share.sjlbkw.cn/Article/details/gvfmnoren.sHtML

ssh user@host 'uptime'
来源：http://www.blog.sjlbkw.cn/Article/details/genqcunvn.sHtML

[R58] 下载文件
来源：http://www.m.share.tarul.cn/Article/details/gryvdusgj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fktsv.cn/Article/details/gdjvhjsyl.sHtML

[R59] 发 POST JSON
来源：http://baike.epnwcf.com/Article/details/gevgfqwjj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.vehdjk.com/Article/details/gpmlxndvi.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.bbcook.cn/Article/details/gvrbcbnst.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fktsv.cn/Article/details/gbypqnhvr.sHtML

[R61] 磁盘占用
来源：http://www.share.tarul.cn/Article/details/gtcalyxfu.sHtML

df -h;  du -sh *
来源：http://read.share.fktsv.cn/Article/details/gllumurmr.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fktsv.cn/Article/details/ghfizmwmr.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.sjlbkw.cn/Article/details/geerwgrvd.sHtML

[R63] 内存与进程
来源：http://read.share.yfazqb.com/Article/details/gzumdamye.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.epnwcf.com/Article/details/gqcoixfto.sHtML

[R64] 结束进程
来源：http://m.share.vehdjk.com/Article/details/goxbgnibn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.bbcook.cn/Article/details/gelnmlvvw.sHtML

[R65] 查看端口占用
来源：http://www.blog.vehdjk.com/Article/details/ggwfdzscj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.yfazqb.com/Article/details/gnzxyppns.sHtML

[R66] 定时任务
来源：http://3g.vehdjk.com/Article/details/gympcurks.sHtML

crontab -e;  crontab -l
来源：http://wap.yfazqb.com/Article/details/gsbxuzhjn.sHtML

[R67] 生成随机十六进制串
来源：http://blog.epnwcf.com/Article/details/gjntclncq.sHtML

openssl rand -hex 16
来源：http://wap.fktsv.cn/Article/details/gzbvjbtku.sHtML

[R68] 计算文件校验值
来源：http://www.blog.yfazqb.com/Article/details/gsobhpgxh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.vehdjk.com/Article/details/gyfpbatxp.sHtML

[R69] 生成随机密码
来源：http://baike.sjlbkw.cn/Article/details/gunooqxhh.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.tarul.cn/Article/details/gawxklcei.sHtML

[R70] 时间戳与互转
来源：http://3g.yfazqb.com/Article/details/gobqypxue.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.yfazqb.com/Article/details/gukolccvo.sHtML

[R71] 日期格式化
来源：http://www.m.share.sjlbkw.cn/Article/details/gjwmkiwhj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.tarul.cn/Article/details/gyrcqnyvq.sHtML

[R72] 等待端口就绪
来源：http://www.blog.epnwcf.com/Article/details/gkryronjv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.vehdjk.com/Article/details/gqtdlsdvy.sHtML

[R73] 分割大日志
来源：http://www.m.share.epnwcf.com/Article/details/gcbgnxljh.sHtML

split -l 1000 big.log part_
来源：http://m.share.yfazqb.com/Article/details/gplbipufa.sHtML

[R74] 批量重命名
来源：http://3g.yfazqb.com/Article/details/gdzxjsryr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fktsv.cn/Article/details/gpnhrhqee.sHtML

[R75] 导出环境变量
来源：http://blog.bbcook.cn/Article/details/gpidgknpy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.yfazqb.com/Article/details/gtimbzlju.sHtML

[R76] 使用临时文件
来源：http://read.share.bbcook.cn/Article/details/gqalfrimu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.sjlbkw.cn/Article/details/gkxzfnnrl.sHtML

[R77] 读取用户输入
来源：http://blog.epnwcf.com/Article/details/gdsungkpu.sHtML

read -rp "请输入: " ans
来源：http://baike.yfazqb.com/Article/details/gbcncjuxe.sHtML

[R78] 交互式菜单
来源：http://www.m.share.yfazqb.com/Article/details/gvyqndcav.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.vehdjk.com/Article/details/geusdthyo.sHtML

[R79] 解析命令行选项
来源：http://wap.epnwcf.com/Article/details/glfwtunjk.sHtML


<!-- 参考信息 -->