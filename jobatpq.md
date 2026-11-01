代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fktsv.cn/Article/details/gupjvkdrv.sHtML

[Q26] 计数
来源：http://blog.sjlbkw.cn/Article/details/gxayprfxo.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.tarul.cn/Article/details/gxgmkimkf.sHtML

[Q27] 条件计数
来源：http://www.share.vehdjk.com/Article/details/gpevwquyy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fktsv.cn/Article/details/gslnfxfdl.sHtML

[Q28] 求和与平均
来源：http://blog.tarul.cn/Article/details/gusgppwxc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/gvjwqxdpl.sHtML

[Q29] 最大最小值
来源：http://baike.bbcook.cn/Article/details/gfxdshmcd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.tarul.cn/Article/details/gkqzlkkov.sHtML

[Q30] 分组统计
来源：http://m.share.yfazqb.com/Article/details/gvefyccqy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fktsv.cn/Article/details/gfliafwfg.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.bbcook.cn/Article/details/gsoctaqbg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.sjlbkw.cn/Article/details/gjuesxxcp.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.bbcook.cn/Article/details/ghckaglza.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.sjlbkw.cn/Article/details/gjiakgwde.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.yfazqb.com/Article/details/gcsyutsqd.sHtML

[Q33] 多列分组
来源：http://www.share.fktsv.cn/Article/details/ggkyfgajh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.tarul.cn/Article/details/gnocwhmij.sHtML

[Q34] 每组取第一条
来源：http://blog.vehdjk.com/Article/details/gryvkiggo.sHtML

SELECT * FROM (
来源：http://www.share.epnwcf.com/Article/details/gjbwnuinq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fktsv.cn/Article/details/gmljafnub.sHtML

) t WHERE rn = 1;
来源：http://wap.tarul.cn/Article/details/glopqilro.sHtML

[Q35] 内连接
来源：http://www.m.share.fktsv.cn/Article/details/gosiuuvaj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.tarul.cn/Article/details/gnnspcoyp.sHtML

[Q36] 左连接
来源：http://www.m.share.epnwcf.com/Article/details/gkbtahsrv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.epnwcf.com/Article/details/gciryevti.sHtML

[Q37] 右连接
来源：http://blog.sjlbkw.cn/Article/details/glhzssypb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.epnwcf.com/Article/details/gpetdajag.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.epnwcf.com/Article/details/gdtgjzbys.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fktsv.cn/Article/details/graeomlpg.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fktsv.cn/Article/details/gupzlowwx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.yfazqb.com/Article/details/gaeqwdekn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.vehdjk.com/Article/details/gujazeqah.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.yfazqb.com/Article/details/gbehszjgw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.bbcook.cn/Article/details/gzilgctqz.sHtML

[Q41] 多表连接
来源：http://read.share.fktsv.cn/Article/details/gbnghhvln.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.tarul.cn/Article/details/gvpayknwm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.vehdjk.com/Article/details/gonbrqvfq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fktsv.cn/Article/details/gaghvdutr.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.bbcook.cn/Article/details/giwlbinhb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.vehdjk.com/Article/details/ggftqhqvc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.tarul.cn/Article/details/gbjvnpmds.sHtML

[Q43] 标量子查询
来源：http://www.blog.fktsv.cn/Article/details/gyfpgacgy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.epnwcf.com/Article/details/gynuinxri.sHtML

[Q44] IN 子查询
来源：http://3g.epnwcf.com/Article/details/gztynjnvy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.bbcook.cn/Article/details/grhtqjvwo.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.tarul.cn/Article/details/guppqsees.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.yfazqb.com/Article/details/gltadysio.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.bbcook.cn/Article/details/gqidssezb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fktsv.cn/Article/details/gdytxsvww.sHtML

[Q47] 与平均值比较
来源：http://www.share.vehdjk.com/Article/details/grbqsgvqc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.sjlbkw.cn/Article/details/gzqqdebmv.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/gkuzjcyga.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fktsv.cn/Article/details/gcsywdnyg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.sjlbkw.cn/Article/details/gzmsgxauo.sHtML

[Q49] 更新单行
来源：http://www.m.share.epnwcf.com/Article/details/gwbttapdc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.yfazqb.com/Article/details/gujbaioiu.sHtML

[Q50] 批量更新
来源：http://read.share.yfazqb.com/Article/details/gctvdfhek.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.sjlbkw.cn/Article/details/gmavdyubh.sHtML

[Q51] 用子查询更新
来源：http://read.share.fktsv.cn/Article/details/gyxhjybht.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.sjlbkw.cn/Article/details/gmlavkngq.sHtML

[Q52] 删除指定行
来源：http://3g.bbcook.cn/Article/details/gxutcziwd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.epnwcf.com/Article/details/gbyrwbzko.sHtML

[Q53] 按条件删除
来源：http://blog.fktsv.cn/Article/details/gyyfwxhtf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.vehdjk.com/Article/details/gpzgczvvp.sHtML

[Q54] 清空表
来源：http://3g.tarul.cn/Article/details/gtrtdpslp.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.sjlbkw.cn/Article/details/gzramvsni.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.sjlbkw.cn/Article/details/ghjaskktb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fktsv.cn/Article/details/gkhhaoflt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.vehdjk.com/Article/details/glgpdzwvh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.sjlbkw.cn/Article/details/giqzzgrbk.sHtML

[Q57] 行号
来源：http://wap.vehdjk.com/Article/details/gvcmlscsl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fktsv.cn/Article/details/grvfhguzi.sHtML

[Q58] 累计求和
来源：http://wap.fktsv.cn/Article/details/gdhnsxpok.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gtccgpylc.sHtML

[Q59] 分组内累计
来源：http://mobile.sjlbkw.cn/Article/details/gqwgudbir.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/gueocijtb.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fktsv.cn/Article/details/gsprigfbq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.bbcook.cn/Article/details/gdnovohdo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.bbcook.cn/Article/details/gjvtxtdqo.sHtML

[Q61] 移动平均
来源：http://read.share.yfazqb.com/Article/details/gicqrfvpn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fktsv.cn/Article/details/gtssvtqbv.sHtML

[Q62] 分组占比
来源：http://www.blog.fktsv.cn/Article/details/ghmjqnjtn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.sjlbkw.cn/Article/details/gwigluafm.sHtML

[Q63] 开启事务
来源：http://blog.epnwcf.com/Article/details/gaokxxoay.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.yfazqb.com/Article/details/gbvuwxmue.sHtML

[Q64] 提交事务
来源：http://3g.sjlbkw.cn/Article/details/gwziluwvf.sHtML

COMMIT;
来源：http://wap.vehdjk.com/Article/details/gkxmwuexg.sHtML

[Q65] 回滚事务
来源：http://3g.yfazqb.com/Article/details/gzsihezxm.sHtML

ROLLBACK;
来源：http://m.share.yfazqb.com/Article/details/gmmtyffla.sHtML

[Q66] 行锁查询
来源：http://baike.epnwcf.com/Article/details/gjsdvjivy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.bbcook.cn/Article/details/gilwsynbl.sHtML

[Q67] 设置隔离级别
来源：http://read.share.vehdjk.com/Article/details/grqcqifei.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.yfazqb.com/Article/details/gyzjmiqcg.sHtML

[Q68] 保存点
来源：http://www.share.epnwcf.com/Article/details/gfobvohkt.sHtML

SAVEPOINT sp1;
来源：http://baike.fktsv.cn/Article/details/gshrkpbee.sHtML

ROLLBACK TO sp1;
来源：http://blog.fktsv.cn/Article/details/gxgoekoxr.sHtML

[Q69] 查看执行计划
来源：http://baike.yfazqb.com/Article/details/gdjjmpluc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.vehdjk.com/Article/details/gwfexkjdm.sHtML

[Q70] 更新统计信息
来源：http://wap.fktsv.cn/Article/details/gnvriijhg.sHtML

ANALYZE TABLE users;
来源：http://mobile.tarul.cn/Article/details/gycmcpvoh.sHtML

[Q71] 查看建表语句
来源：http://www.share.sjlbkw.cn/Article/details/gldmqvnea.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.tarul.cn/Article/details/gbglmhzzf.sHtML

[Q72] 查看索引
来源：http://www.m.share.tarul.cn/Article/details/ggywxzdap.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.tarul.cn/Article/details/grifnltra.sHtML

[Q73] 查看表状态
来源：http://m.share.fktsv.cn/Article/details/gkljdmqov.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.sjlbkw.cn/Article/details/gmkutzcmc.sHtML

[Q74] 强制使用索引
来源：http://www.blog.epnwcf.com/Article/details/gyfekztuh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.vehdjk.com/Article/details/gpbfmslml.sHtML

[Q75] 日期格式化
来源：http://www.blog.yfazqb.com/Article/details/gvnpqyemw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/gtbppiwgg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.epnwcf.com/Article/details/gusbqpgoe.sHtML

[Q76] 按天统计
来源：http://www.blog.epnwcf.com/Article/details/gifjwelxz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.sjlbkw.cn/Article/details/gkacqgxgb.sHtML

[Q77] 时间加减
来源：http://3g.vehdjk.com/Article/details/gckgabrvw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.epnwcf.com/Article/details/gbtnxktgu.sHtML

[Q78] 当前时间
来源：http://www.m.share.sjlbkw.cn/Article/details/gmldogilr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.bbcook.cn/Article/details/gimujwvja.sHtML

[Q79] 字符串拼接
来源：http://3g.fktsv.cn/Article/details/gywqyjwbw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.bbcook.cn/Article/details/gmqalfyib.sHtML

[Q80] 字符串截取
来源：http://baike.tarul.cn/Article/details/glehqcewd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.tarul.cn/Article/details/gtwhkixcd.sHtML

[Q81] 字符串替换
来源：http://www.blog.bbcook.cn/Article/details/gjzglpkbp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gwmmypmnt.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.sjlbkw.cn/Article/details/ghangymns.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gzinrgrsa.sHtML

[Q83] 大小写转换
来源：http://www.blog.yfazqb.com/Article/details/gxxdcjkpj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gwmunrfzk.sHtML

[Q84] 去除首尾空格
来源：http://wap.tarul.cn/Article/details/ggayzoalb.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.yfazqb.com/Article/details/gkcqhvujk.sHtML

[Q85] 数值取整
来源：http://read.share.yfazqb.com/Article/details/gplqwbpwy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fktsv.cn/Article/details/gdtrqtiuh.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.bbcook.cn/Article/details/ghikhnzrn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.vehdjk.com/Article/details/gmgutzpzy.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.bbcook.cn/Article/details/gsvbajruj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.sjlbkw.cn/Article/details/gpxklfrjo.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.epnwcf.com/Article/details/gxlzueezw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.epnwcf.com/Article/details/gbngwdhdf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fktsv.cn/Article/details/gwzhzamza.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fktsv.cn/Article/details/gksgiseqr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.bbcook.cn/Article/details/gtyyqwfxx.sHtML

[Q90] 生成序号列
来源：http://www.m.share.tarul.cn/Article/details/gsznaynpy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.bbcook.cn/Article/details/gvjnjzdrf.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gususojvs.sHtML

R. Bash 专题
来源：http://wap.vehdjk.com/Article/details/gyhpkmjva.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gslpdalop.sHtML

[R01] shebang 与严格模式
来源：http://baike.vehdjk.com/Article/details/goulyopph.sHtML

#!/usr/bin/env bash
来源：http://wap.fktsv.cn/Article/details/gracljolb.sHtML

set -euo pipefail
来源：http://mobile.fktsv.cn/Article/details/gshhwbfge.sHtML

[R02] 变量赋值与使用
来源：http://read.share.tarul.cn/Article/details/gnhzihubf.sHtML

name="Tom"; echo "$name"
来源：http://m.share.epnwcf.com/Article/details/gmdrscerz.sHtML

[R03] 只读变量
来源：http://m.share.yfazqb.com/Article/details/gcjyocvgq.sHtML

readonly PI=3.14
来源：http://3g.yfazqb.com/Article/details/gkfyhvtsa.sHtML

[R04] 位置参数
来源：http://www.share.yfazqb.com/Article/details/gcukxgqij.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.tarul.cn/Article/details/gngxmuotj.sHtML

[R05] 参数默认值
来源：http://baike.sjlbkw.cn/Article/details/guzokbtem.sHtML

name="${1:-default}"
来源：http://www.share.sjlbkw.cn/Article/details/gdahhmhra.sHtML

[R06] 判断命令是否存在
来源：http://baike.tarul.cn/Article/details/gbiorgglf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.bbcook.cn/Article/details/gddgbziql.sHtML

[R07] if 判断文件
来源：http://3g.sjlbkw.cn/Article/details/gyxgxunzw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.bbcook.cn/Article/details/gygbpgdlk.sHtML

[R08] 数值比较
来源：http://baike.fktsv.cn/Article/details/gudxigzok.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.epnwcf.com/Article/details/gwyteekmu.sHtML

[R09] 字符串比较
来源：http://read.share.sjlbkw.cn/Article/details/ggsmugqzw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.epnwcf.com/Article/details/gnsfuozyp.sHtML

[R10] 正则匹配
来源：http://mobile.sjlbkw.cn/Article/details/ggzfuephg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.tarul.cn/Article/details/gvjgpyequ.sHtML

[R11] case 多分支
来源：http://www.blog.epnwcf.com/Article/details/gdywlwjxc.sHtML

case "$1" in
来源：http://read.share.bbcook.cn/Article/details/gorreialh.sHtML

start) echo "启动" ;;
来源：http://www.m.share.vehdjk.com/Article/details/gfeovhoed.sHtML

stop)  echo "停止" ;;
来源：http://3g.tarul.cn/Article/details/grnogrwzk.sHtML

*)     echo "未知命令" ;;
来源：http://baike.yfazqb.com/Article/details/gxiegjnog.sHtML

esac
来源：http://blog.yfazqb.com/Article/details/gniysddeg.sHtML

[R12] for 遍历文件
来源：http://m.share.fktsv.cn/Article/details/gzmwfzyfv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.yfazqb.com/Article/details/gzkdibbbd.sHtML

[R13] for 计数循环
来源：http://www.share.fktsv.cn/Article/details/gkkcpejcb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.yfazqb.com/Article/details/gixpqapph.sHtML

[R14] C 风格 for
来源：http://m.share.fktsv.cn/Article/details/gscoiyjkb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.vehdjk.com/Article/details/ghkrwqsao.sHtML

[R15] while 逐行读文件
来源：http://wap.yfazqb.com/Article/details/gecurbncd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.tarul.cn/Article/details/gyurtxyat.sHtML

[R16] until 等待条件
来源：http://www.blog.yfazqb.com/Article/details/gaptwqxcg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.tarul.cn/Article/details/ghwyknkcy.sHtML

[R17] 数组定义与取值
来源：http://m.share.epnwcf.com/Article/details/gsblpugip.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.yfazqb.com/Article/details/gexquogoy.sHtML

[R18] 遍历数组
来源：http://m.share.vehdjk.com/Article/details/gplkzjkbt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.sjlbkw.cn/Article/details/gzxpsuenp.sHtML

[R19] 数组长度
来源：http://3g.tarul.cn/Article/details/gfkhaagln.sHtML

echo "${#arr[@]}"
来源：http://www.share.fktsv.cn/Article/details/gpuvqayts.sHtML

[R20] 关联数组（字典）
来源：http://read.share.sjlbkw.cn/Article/details/gybhutbkb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.vehdjk.com/Article/details/gmvlegzjd.sHtML

[R21] 字符串长度
来源：http://m.share.yfazqb.com/Article/details/gvtxxvpfq.sHtML

echo "${#s}"
来源：http://3g.yfazqb.com/Article/details/gndceulcq.sHtML

[R22] 截取子串
来源：http://www.m.share.tarul.cn/Article/details/gmpdjfjwb.sHtML

echo "${s:0:5}"
来源：http://mobile.bbcook.cn/Article/details/goifceczl.sHtML

[R23] 字符串替换
来源：http://blog.fktsv.cn/Article/details/gqdlveqnt.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.sjlbkw.cn/Article/details/glopkrisc.sHtML

[R24] 大小写转换
来源：http://www.blog.sjlbkw.cn/Article/details/gbkveabca.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.yfazqb.com/Article/details/gsqrpwnyy.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.yfazqb.com/Article/details/gucoaselp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.vehdjk.com/Article/details/gubrqrceo.sHtML

[R26] 命令替换
来源：http://www.m.share.fktsv.cn/Article/details/gppawgmpn.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.vehdjk.com/Article/details/gpainwxfw.sHtML

[R27] 算术展开
来源：http://www.m.share.sjlbkw.cn/Article/details/gsfywlocd.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.tarul.cn/Article/details/gqphouedm.sHtML

[R28] 浮点运算
来源：http://m.share.bbcook.cn/Article/details/ggktegkls.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.sjlbkw.cn/Article/details/gmwlnxzcx.sHtML

[R29] 定义函数
来源：http://m.share.bbcook.cn/Article/details/grystmwqj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.yfazqb.com/Article/details/gogugelpo.sHtML

[R30] 函数返回状态码
来源：http://baike.vehdjk.com/Article/details/gwewufglx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.vehdjk.com/Article/details/gsvqaoxev.sHtML

[R31] 局部变量
来源：http://m.share.bbcook.cn/Article/details/gbnimgmpe.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.epnwcf.com/Article/details/ggylitooc.sHtML

[R32] 参数个数校验
来源：http://www.m.share.yfazqb.com/Article/details/gtxiqldsy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.yfazqb.com/Article/details/gdgljfslr.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.yfazqb.com/Article/details/gcuwnpngd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.epnwcf.com/Article/details/gfhdchbtu.sHtML

[R34] 退出时清理
来源：http://www.m.share.epnwcf.com/Article/details/gtjmwwamt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.tarul.cn/Article/details/gioqdnzam.sHtML

[R35] 后台执行并等待
来源：http://mobile.fktsv.cn/Article/details/goaenfagk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.tarul.cn/Article/details/gjqdlrnjc.sHtML

[R36] 并发执行多个任务
来源：http://wap.bbcook.cn/Article/details/givznjngf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fktsv.cn/Article/details/gbzzvjyfr.sHtML

[R37] 把输出赋给变量
来源：http://baike.fktsv.cn/Article/details/ggxhlruex.sHtML

files=$(ls -1)
来源：http://m.share.sjlbkw.cn/Article/details/gzrjspnlb.sHtML

[R38] 管道串联
来源：http://mobile.bbcook.cn/Article/details/gzfoiezjt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.epnwcf.com/Article/details/gejanobyk.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.vehdjk.com/Article/details/ghvzwmmuc.sHtML

cmd > out.log 2>&1
来源：http://www.share.fktsv.cn/Article/details/gdvickohm.sHtML

[R40] 追加写日志
来源：http://blog.bbcook.cn/Article/details/gohtooqee.sHtML

echo "log" >> out.log
来源：http://blog.bbcook.cn/Article/details/gdloipjbo.sHtML

[R41] 丢弃输出
来源：http://www.m.share.yfazqb.com/Article/details/gdqfqtaqh.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.yfazqb.com/Article/details/grtvuaosr.sHtML

[R42] 输入重定向
来源：http://m.share.epnwcf.com/Article/details/gakebhkdm.sHtML

wc -l < a.txt
来源：http://wap.yfazqb.com/Article/details/gyhuezzef.sHtML

[R43] 按名字查找文件
来源：http://baike.yfazqb.com/Article/details/gpcgqufrd.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.epnwcf.com/Article/details/gvamibchp.sHtML

[R44] 按修改时间查找
来源：http://wap.epnwcf.com/Article/details/gfiuknqzs.sHtML

find . -mtime -7 -type f
来源：http://m.share.bbcook.cn/Article/details/gtbbhymbt.sHtML

[R45] 批量删除
来源：http://m.share.vehdjk.com/Article/details/gmpjclhcr.sHtML

find . -name "*.tmp" -delete
来源：http://3g.sjlbkw.cn/Article/details/gcareopdu.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.sjlbkw.cn/Article/details/gnumchkde.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.tarul.cn/Article/details/gnorklzre.sHtML

[R47] sed 单行替换
来源：http://3g.tarul.cn/Article/details/gilnxhcmb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.vehdjk.com/Article/details/giwyjgnra.sHtML

[R48] awk 取指定列
来源：http://m.share.yfazqb.com/Article/details/gzxfeeqlw.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.vehdjk.com/Article/details/gnggzolid.sHtML

[R49] awk 带条件
来源：http://m.share.vehdjk.com/Article/details/glvqabofc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.epnwcf.com/Article/details/gtwtwmgaf.sHtML

[R50] awk 求和
来源：http://3g.bbcook.cn/Article/details/geqonvnve.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.yfazqb.com/Article/details/gbkhdphia.sHtML

[R51] 排序去重取前几
来源：http://wap.sjlbkw.cn/Article/details/gfzsggkki.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.epnwcf.com/Article/details/gdxhrzxsy.sHtML

[R52] 统计行数
来源：http://read.share.yfazqb.com/Article/details/gbfxcklrc.sHtML

wc -l a.txt
来源：http://www.m.share.fktsv.cn/Article/details/gysaunhdu.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fktsv.cn/Article/details/ggsjdxbon.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.yfazqb.com/Article/details/gjaewkmog.sHtML

[R54] 比较两个文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gdxlkbvas.sHtML

diff a.txt b.txt
来源：http://wap.sjlbkw.cn/Article/details/gezzjntlf.sHtML

[R55] 压缩与解压
来源：http://mobile.vehdjk.com/Article/details/gocjbtnim.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fktsv.cn/Article/details/gnqeqltch.sHtML

[R56] 远程拷贝
来源：http://wap.tarul.cn/Article/details/gaiigbscw.sHtML

scp file user@host:/path/
来源：http://m.share.epnwcf.com/Article/details/gnwufmcff.sHtML

[R57] 远程执行命令
来源：http://www.blog.yfazqb.com/Article/details/gdeppxmzw.sHtML

ssh user@host 'uptime'
来源：http://m.share.epnwcf.com/Article/details/gcklhrgyy.sHtML

[R58] 下载文件
来源：http://www.blog.sjlbkw.cn/Article/details/geiyzlbom.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.sjlbkw.cn/Article/details/gibfstmhz.sHtML

[R59] 发 POST JSON
来源：http://baike.epnwcf.com/Article/details/gmxxcjqih.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.vehdjk.com/Article/details/gtotxbeqm.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.tarul.cn/Article/details/gfvtkmnzw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.yfazqb.com/Article/details/glxrmqhin.sHtML

[R61] 磁盘占用
来源：http://www.share.epnwcf.com/Article/details/gwjthnyqn.sHtML

df -h;  du -sh *
来源：http://mobile.yfazqb.com/Article/details/gdnvocgdt.sHtML

[R62] 找最占空间的文件
来源：http://mobile.sjlbkw.cn/Article/details/gmmdgzgke.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.epnwcf.com/Article/details/ghmwmeqkr.sHtML

[R63] 内存与进程
来源：http://www.share.epnwcf.com/Article/details/giceyzahb.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.epnwcf.com/Article/details/gxixazocn.sHtML

[R64] 结束进程
来源：http://baike.tarul.cn/Article/details/gcjlntiws.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.epnwcf.com/Article/details/ghewiabqo.sHtML

[R65] 查看端口占用
来源：http://blog.yfazqb.com/Article/details/gbtegunvz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fktsv.cn/Article/details/gpoaijbff.sHtML

[R66] 定时任务
来源：http://mobile.bbcook.cn/Article/details/gsqtrkrco.sHtML

crontab -e;  crontab -l
来源：http://www.share.yfazqb.com/Article/details/gqlayacce.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.bbcook.cn/Article/details/gazzeavsm.sHtML

openssl rand -hex 16
来源：http://wap.bbcook.cn/Article/details/gyuyzeuoc.sHtML

[R68] 计算文件校验值
来源：http://blog.sjlbkw.cn/Article/details/gsvgnwkzl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.bbcook.cn/Article/details/gzoxptcrc.sHtML

[R69] 生成随机密码
来源：http://read.share.vehdjk.com/Article/details/grihoqqwy.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.bbcook.cn/Article/details/geexfezzk.sHtML

[R70] 时间戳与互转
来源：http://baike.sjlbkw.cn/Article/details/gutscfzri.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.yfazqb.com/Article/details/gujynqnbf.sHtML

[R71] 日期格式化
来源：http://www.blog.bbcook.cn/Article/details/gijjdcyka.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fktsv.cn/Article/details/gqxohhneu.sHtML

[R72] 等待端口就绪
来源：http://mobile.tarul.cn/Article/details/gcjeumuqq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.yfazqb.com/Article/details/gmesolfmq.sHtML

[R73] 分割大日志
来源：http://www.share.fktsv.cn/Article/details/gotdkpemb.sHtML

split -l 1000 big.log part_
来源：http://3g.sjlbkw.cn/Article/details/gnjracltr.sHtML

[R74] 批量重命名
来源：http://wap.vehdjk.com/Article/details/gnfraekvs.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.yfazqb.com/Article/details/gizsgrior.sHtML

[R75] 导出环境变量
来源：http://mobile.tarul.cn/Article/details/gpebirwbj.sHtML


<!-- 参考信息 -->