代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.yfazqb.com/Article/details/ghftlomzl.sHtML

[Q24] 去重
来源：http://www.m.share.vehdjk.com/Article/details/gukfobbxb.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gyusdgzsv.sHtML

[Q25] 只取前 N 条
来源：http://blog.fktsv.cn/Article/details/gcipmpqkl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.tarul.cn/Article/details/gksebuhvo.sHtML

[Q26] 计数
来源：http://www.blog.yfazqb.com/Article/details/gtzitixcg.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.vehdjk.com/Article/details/gpvgrinxi.sHtML

[Q27] 条件计数
来源：http://www.blog.tarul.cn/Article/details/gjuspwfcw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.bbcook.cn/Article/details/gfwvjcuns.sHtML

[Q28] 求和与平均
来源：http://read.share.fktsv.cn/Article/details/getarzyel.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.yfazqb.com/Article/details/gnggdljhq.sHtML

[Q29] 最大最小值
来源：http://wap.yfazqb.com/Article/details/gocfswbdf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gvvpsldmi.sHtML

[Q30] 分组统计
来源：http://www.m.share.yfazqb.com/Article/details/gqxznaqmn.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.tarul.cn/Article/details/gzhmochss.sHtML

[Q31] 分组后过滤
来源：http://www.blog.sjlbkw.cn/Article/details/goawdbdnp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.yfazqb.com/Article/details/gimsblrtp.sHtML

[Q32] 分组拼接字符串
来源：http://wap.tarul.cn/Article/details/gqxvwrski.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.sjlbkw.cn/Article/details/gxakmvyzd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.vehdjk.com/Article/details/gybyhpuon.sHtML

[Q33] 多列分组
来源：http://blog.vehdjk.com/Article/details/ghmqlfqjj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.epnwcf.com/Article/details/gbxgtupyi.sHtML

[Q34] 每组取第一条
来源：http://m.share.sjlbkw.cn/Article/details/gvdsjvarq.sHtML

SELECT * FROM (
来源：http://blog.fktsv.cn/Article/details/gohybsqfe.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.tarul.cn/Article/details/gebmfkapj.sHtML

) t WHERE rn = 1;
来源：http://www.share.bbcook.cn/Article/details/gsoknuxhh.sHtML

[Q35] 内连接
来源：http://www.m.share.epnwcf.com/Article/details/gxitbpoyo.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.sjlbkw.cn/Article/details/gbtojudbu.sHtML

[Q36] 左连接
来源：http://wap.tarul.cn/Article/details/ghlnpebth.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.vehdjk.com/Article/details/grxzeodww.sHtML

[Q37] 右连接
来源：http://read.share.yfazqb.com/Article/details/gdfixjuvr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fktsv.cn/Article/details/gdwixkjfy.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.yfazqb.com/Article/details/gdaybvmtz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.epnwcf.com/Article/details/gigeszxod.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fktsv.cn/Article/details/gwzvguijg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.vehdjk.com/Article/details/gwbblnfkq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.vehdjk.com/Article/details/gycpdesgb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fktsv.cn/Article/details/gpaetcbcm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fktsv.cn/Article/details/gcomnxvak.sHtML

[Q41] 多表连接
来源：http://wap.sjlbkw.cn/Article/details/gpuhkifid.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.epnwcf.com/Article/details/gtvhhvhrs.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.yfazqb.com/Article/details/gnmxmtyda.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.sjlbkw.cn/Article/details/gjyvqprua.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fktsv.cn/Article/details/gsfvlhbom.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.sjlbkw.cn/Article/details/gvcrwyflb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.tarul.cn/Article/details/gddznyhsv.sHtML

[Q43] 标量子查询
来源：http://www.blog.tarul.cn/Article/details/gbkngnjpr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.vehdjk.com/Article/details/gluduledw.sHtML

[Q44] IN 子查询
来源：http://blog.bbcook.cn/Article/details/gknxkeilq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.epnwcf.com/Article/details/glrnotmmx.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.yfazqb.com/Article/details/gubalhhci.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.tarul.cn/Article/details/gjuyiskpm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.tarul.cn/Article/details/gwssaulni.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.vehdjk.com/Article/details/gqzcwhmhq.sHtML

[Q47] 与平均值比较
来源：http://m.share.sjlbkw.cn/Article/details/gqgbjfvyi.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.vehdjk.com/Article/details/grohrfnlc.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fktsv.cn/Article/details/gzmstslam.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.epnwcf.com/Article/details/gxcikvboj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.yfazqb.com/Article/details/gchabawlr.sHtML

[Q49] 更新单行
来源：http://www.blog.bbcook.cn/Article/details/gmupkgadj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.bbcook.cn/Article/details/gpgfhzyoe.sHtML

[Q50] 批量更新
来源：http://wap.yfazqb.com/Article/details/guycmmjzr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.epnwcf.com/Article/details/gdxpscgec.sHtML

[Q51] 用子查询更新
来源：http://m.share.vehdjk.com/Article/details/ghsjljcut.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.tarul.cn/Article/details/glbuatlyy.sHtML

[Q52] 删除指定行
来源：http://m.share.epnwcf.com/Article/details/goiwwrcau.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.epnwcf.com/Article/details/gnjnzvraq.sHtML

[Q53] 按条件删除
来源：http://read.share.fktsv.cn/Article/details/ghhpxnwln.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.yfazqb.com/Article/details/gydsgeqos.sHtML

[Q54] 清空表
来源：http://read.share.sjlbkw.cn/Article/details/gcfoitqox.sHtML

TRUNCATE TABLE logs;
来源：http://3g.bbcook.cn/Article/details/gllebsggc.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.bbcook.cn/Article/details/gzufsniyu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.vehdjk.com/Article/details/gvgwkvfis.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.epnwcf.com/Article/details/gcgrkabge.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.sjlbkw.cn/Article/details/grqlrhcia.sHtML

[Q57] 行号
来源：http://mobile.fktsv.cn/Article/details/gkfqphszt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.tarul.cn/Article/details/goqhknfzb.sHtML

[Q58] 累计求和
来源：http://3g.vehdjk.com/Article/details/gtfcacocb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.tarul.cn/Article/details/gzsmfvrjx.sHtML

[Q59] 分组内累计
来源：http://www.m.share.tarul.cn/Article/details/gvurwxrvt.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.tarul.cn/Article/details/gggqmvlwg.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.bbcook.cn/Article/details/gpwfeycrl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.bbcook.cn/Article/details/gykdizzwc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.vehdjk.com/Article/details/grxaxnmfk.sHtML

[Q61] 移动平均
来源：http://baike.epnwcf.com/Article/details/gulahwael.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.vehdjk.com/Article/details/gzoozaxtd.sHtML

[Q62] 分组占比
来源：http://mobile.tarul.cn/Article/details/ghetpwlkx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.sjlbkw.cn/Article/details/gskqvhxqu.sHtML

[Q63] 开启事务
来源：http://www.blog.bbcook.cn/Article/details/gegdaunlb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.epnwcf.com/Article/details/gihukrnml.sHtML

[Q64] 提交事务
来源：http://mobile.epnwcf.com/Article/details/gxvpjrctj.sHtML

COMMIT;
来源：http://wap.epnwcf.com/Article/details/gsbifzjqt.sHtML

[Q65] 回滚事务
来源：http://wap.fktsv.cn/Article/details/gkzxehfyj.sHtML

ROLLBACK;
来源：http://read.share.vehdjk.com/Article/details/gqyalkfzg.sHtML

[Q66] 行锁查询
来源：http://blog.vehdjk.com/Article/details/gswvxguot.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.sjlbkw.cn/Article/details/gqtbvcpzn.sHtML

[Q67] 设置隔离级别
来源：http://read.share.bbcook.cn/Article/details/gnfyqcvwe.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.tarul.cn/Article/details/ggkuzykqu.sHtML

[Q68] 保存点
来源：http://3g.fktsv.cn/Article/details/gaakausrd.sHtML

SAVEPOINT sp1;
来源：http://blog.sjlbkw.cn/Article/details/ggegzmjys.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.tarul.cn/Article/details/gobszregl.sHtML

[Q69] 查看执行计划
来源：http://3g.tarul.cn/Article/details/guzfktiht.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.yfazqb.com/Article/details/gaibonfjk.sHtML

[Q70] 更新统计信息
来源：http://blog.vehdjk.com/Article/details/gurfwjoka.sHtML

ANALYZE TABLE users;
来源：http://baike.epnwcf.com/Article/details/gnobypchm.sHtML

[Q71] 查看建表语句
来源：http://baike.tarul.cn/Article/details/giucuyicb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.tarul.cn/Article/details/gehckwqwj.sHtML

[Q72] 查看索引
来源：http://blog.tarul.cn/Article/details/gmbxqtsgh.sHtML

SHOW INDEX FROM users;
来源：http://read.share.bbcook.cn/Article/details/gzzptqilh.sHtML

[Q73] 查看表状态
来源：http://m.share.tarul.cn/Article/details/gdzwsumyt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.vehdjk.com/Article/details/guexhhnql.sHtML

[Q74] 强制使用索引
来源：http://read.share.vehdjk.com/Article/details/gvnetggqd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.tarul.cn/Article/details/gjktjaiag.sHtML

[Q75] 日期格式化
来源：http://m.share.vehdjk.com/Article/details/gvswhodcm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.vehdjk.com/Article/details/ghogngcno.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.yfazqb.com/Article/details/gaoyeypmo.sHtML

[Q76] 按天统计
来源：http://m.share.yfazqb.com/Article/details/grulcwfuq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fktsv.cn/Article/details/gyqwkwxli.sHtML

[Q77] 时间加减
来源：http://3g.bbcook.cn/Article/details/gelkkpxoj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.yfazqb.com/Article/details/gsyaajgga.sHtML

[Q78] 当前时间
来源：http://mobile.bbcook.cn/Article/details/gjfndincf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.vehdjk.com/Article/details/goyzgpjkz.sHtML

[Q79] 字符串拼接
来源：http://wap.sjlbkw.cn/Article/details/gzjkarejk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.epnwcf.com/Article/details/goibqrlll.sHtML

[Q80] 字符串截取
来源：http://www.blog.tarul.cn/Article/details/gjugjzlol.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/grnkogexn.sHtML

[Q81] 字符串替换
来源：http://www.share.bbcook.cn/Article/details/ganjmxgrr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gbzygpywe.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.vehdjk.com/Article/details/gvggfkttc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fktsv.cn/Article/details/ggvsymyfh.sHtML

[Q83] 大小写转换
来源：http://m.share.vehdjk.com/Article/details/gnwhiezfe.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.tarul.cn/Article/details/gsowirmyi.sHtML

[Q84] 去除首尾空格
来源：http://m.share.bbcook.cn/Article/details/gsqlhgqzm.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.vehdjk.com/Article/details/gmolzatzk.sHtML

[Q85] 数值取整
来源：http://m.share.fktsv.cn/Article/details/gyrcggays.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.bbcook.cn/Article/details/gzgyvfyuc.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.sjlbkw.cn/Article/details/gidnnnslx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.tarul.cn/Article/details/glzjjssyq.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.bbcook.cn/Article/details/gttryqhkp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.yfazqb.com/Article/details/gysypyyrw.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.tarul.cn/Article/details/gdgwzogjp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.vehdjk.com/Article/details/gfeifupbw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.tarul.cn/Article/details/gclyqfvyx.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.sjlbkw.cn/Article/details/gagaxxzqa.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.sjlbkw.cn/Article/details/gkqihohoo.sHtML

[Q90] 生成序号列
来源：http://baike.sjlbkw.cn/Article/details/gjwbybckc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.yfazqb.com/Article/details/ghxwdmdvq.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gsjbveowj.sHtML

R. Bash 专题
来源：http://www.share.vehdjk.com/Article/details/guhjutpsu.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gcaqsiryd.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.sjlbkw.cn/Article/details/gxtvguypq.sHtML

#!/usr/bin/env bash
来源：http://www.blog.bbcook.cn/Article/details/gcduubkld.sHtML

set -euo pipefail
来源：http://3g.vehdjk.com/Article/details/ghsikxhxz.sHtML

[R02] 变量赋值与使用
来源：http://read.share.yfazqb.com/Article/details/gesaiqlbc.sHtML

name="Tom"; echo "$name"
来源：http://m.share.sjlbkw.cn/Article/details/gnogwsrdo.sHtML

[R03] 只读变量
来源：http://www.m.share.bbcook.cn/Article/details/gwasjmdmk.sHtML

readonly PI=3.14
来源：http://mobile.fktsv.cn/Article/details/ggsagrxor.sHtML

[R04] 位置参数
来源：http://wap.sjlbkw.cn/Article/details/guewpgwdt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.vehdjk.com/Article/details/ggovlbhbc.sHtML

[R05] 参数默认值
来源：http://www.blog.sjlbkw.cn/Article/details/gsuxxkszz.sHtML

name="${1:-default}"
来源：http://baike.bbcook.cn/Article/details/goxtpbeih.sHtML

[R06] 判断命令是否存在
来源：http://m.share.epnwcf.com/Article/details/gurjqgyzv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.sjlbkw.cn/Article/details/ghniyqhww.sHtML

[R07] if 判断文件
来源：http://www.m.share.yfazqb.com/Article/details/gcriyslvz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.sjlbkw.cn/Article/details/gbgkftgrn.sHtML

[R08] 数值比较
来源：http://m.share.tarul.cn/Article/details/gaouuzrkb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fktsv.cn/Article/details/gwkasytqh.sHtML

[R09] 字符串比较
来源：http://m.share.tarul.cn/Article/details/gnzkdudow.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fktsv.cn/Article/details/gnjbsbtoi.sHtML

[R10] 正则匹配
来源：http://m.share.fktsv.cn/Article/details/gsggxgoxv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.vehdjk.com/Article/details/gvqijxsdd.sHtML

[R11] case 多分支
来源：http://mobile.vehdjk.com/Article/details/gknblijod.sHtML

case "$1" in
来源：http://m.share.fktsv.cn/Article/details/gtsayjspn.sHtML

start) echo "启动" ;;
来源：http://blog.epnwcf.com/Article/details/gyerivrhd.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fktsv.cn/Article/details/gxfqdyghh.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.tarul.cn/Article/details/gxilmbliy.sHtML

esac
来源：http://baike.epnwcf.com/Article/details/gssupqrml.sHtML

[R12] for 遍历文件
来源：http://mobile.sjlbkw.cn/Article/details/gpirntakk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.vehdjk.com/Article/details/gaqkerhim.sHtML

[R13] for 计数循环
来源：http://read.share.vehdjk.com/Article/details/guraelgps.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.yfazqb.com/Article/details/gjnruwsjl.sHtML

[R14] C 风格 for
来源：http://read.share.vehdjk.com/Article/details/gkflpnswy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fktsv.cn/Article/details/gentgekge.sHtML

[R15] while 逐行读文件
来源：http://blog.vehdjk.com/Article/details/gabhsunxe.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.bbcook.cn/Article/details/gunigdmnh.sHtML

[R16] until 等待条件
来源：http://www.blog.fktsv.cn/Article/details/gntvhnkwn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.yfazqb.com/Article/details/gwcoquelv.sHtML

[R17] 数组定义与取值
来源：http://www.share.vehdjk.com/Article/details/gcprjdarz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.epnwcf.com/Article/details/gqartdiry.sHtML

[R18] 遍历数组
来源：http://mobile.vehdjk.com/Article/details/gvslgnkcy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.sjlbkw.cn/Article/details/gbwcrdxgx.sHtML

[R19] 数组长度
来源：http://blog.yfazqb.com/Article/details/grzvxkmff.sHtML

echo "${#arr[@]}"
来源：http://www.blog.sjlbkw.cn/Article/details/goopzldgv.sHtML

[R20] 关联数组（字典）
来源：http://blog.tarul.cn/Article/details/gdzduoqci.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.tarul.cn/Article/details/grudwrvrl.sHtML

[R21] 字符串长度
来源：http://3g.sjlbkw.cn/Article/details/gkvsyvrma.sHtML

echo "${#s}"
来源：http://m.share.tarul.cn/Article/details/gojupcsmn.sHtML

[R22] 截取子串
来源：http://m.share.tarul.cn/Article/details/gmdxhgdfa.sHtML

echo "${s:0:5}"
来源：http://3g.vehdjk.com/Article/details/grornxvkq.sHtML

[R23] 字符串替换
来源：http://www.blog.epnwcf.com/Article/details/gxevkwyya.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.vehdjk.com/Article/details/grpyeviwy.sHtML

[R24] 大小写转换
来源：http://blog.epnwcf.com/Article/details/gxdvbclkl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.yfazqb.com/Article/details/gabrgavjd.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fktsv.cn/Article/details/gulucdcdi.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.sjlbkw.cn/Article/details/gljsngrum.sHtML

[R26] 命令替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gmsustvwq.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.yfazqb.com/Article/details/gutillibq.sHtML

[R27] 算术展开
来源：http://read.share.sjlbkw.cn/Article/details/gnyytzwve.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.sjlbkw.cn/Article/details/gttexjnyq.sHtML

[R28] 浮点运算
来源：http://www.m.share.yfazqb.com/Article/details/goeidknix.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fktsv.cn/Article/details/gftuitgwz.sHtML

[R29] 定义函数
来源：http://blog.bbcook.cn/Article/details/gkudazxqw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.vehdjk.com/Article/details/gqpzstszf.sHtML

[R30] 函数返回状态码
来源：http://wap.yfazqb.com/Article/details/gxezvtnsq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.sjlbkw.cn/Article/details/gbmawekwr.sHtML

[R31] 局部变量
来源：http://read.share.epnwcf.com/Article/details/gubrlidpx.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.epnwcf.com/Article/details/gscqxxfel.sHtML

[R32] 参数个数校验
来源：http://www.blog.vehdjk.com/Article/details/ggysmummi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.bbcook.cn/Article/details/gsjwnltox.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.tarul.cn/Article/details/gezwuptne.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.tarul.cn/Article/details/gtiwkvgfe.sHtML

[R34] 退出时清理
来源：http://www.m.share.yfazqb.com/Article/details/gfjvvahqj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.vehdjk.com/Article/details/gujkzdiko.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.epnwcf.com/Article/details/gkihkyxyl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fktsv.cn/Article/details/gcdodgeku.sHtML

[R36] 并发执行多个任务
来源：http://blog.yfazqb.com/Article/details/gvodjfqux.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.epnwcf.com/Article/details/gkvbeehvf.sHtML

[R37] 把输出赋给变量
来源：http://m.share.tarul.cn/Article/details/gfghutglk.sHtML

files=$(ls -1)
来源：http://blog.sjlbkw.cn/Article/details/grocsrclm.sHtML

[R38] 管道串联
来源：http://blog.vehdjk.com/Article/details/gawnymsab.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fktsv.cn/Article/details/gtuhbbdsd.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.sjlbkw.cn/Article/details/gzghtmetg.sHtML

cmd > out.log 2>&1
来源：http://blog.bbcook.cn/Article/details/gxabaubre.sHtML

[R40] 追加写日志
来源：http://mobile.vehdjk.com/Article/details/gpgarrwde.sHtML

echo "log" >> out.log
来源：http://3g.epnwcf.com/Article/details/gmsqccsdf.sHtML

[R41] 丢弃输出
来源：http://m.share.fktsv.cn/Article/details/gekaojhdx.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.vehdjk.com/Article/details/gbupkkcqt.sHtML

[R42] 输入重定向
来源：http://www.share.epnwcf.com/Article/details/gsdcxdeic.sHtML

wc -l < a.txt
来源：http://www.share.yfazqb.com/Article/details/gylibnejl.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.yfazqb.com/Article/details/gvarqzmsl.sHtML

find . -name "*.log" -type f
来源：http://mobile.yfazqb.com/Article/details/gxuygswed.sHtML

[R44] 按修改时间查找
来源：http://mobile.yfazqb.com/Article/details/gbtzqlxui.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.yfazqb.com/Article/details/gdbiblumv.sHtML

[R45] 批量删除
来源：http://www.m.share.yfazqb.com/Article/details/gkkzfqvys.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.yfazqb.com/Article/details/gucngduwn.sHtML

[R46] 递归替换文件内容
来源：http://www.share.sjlbkw.cn/Article/details/glnyaljzc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fktsv.cn/Article/details/gzcznmdqh.sHtML

[R47] sed 单行替换
来源：http://blog.fktsv.cn/Article/details/gccemddsa.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.epnwcf.com/Article/details/gwvkkitio.sHtML

[R48] awk 取指定列
来源：http://m.share.tarul.cn/Article/details/gnebbquzp.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.epnwcf.com/Article/details/ginvfbble.sHtML

[R49] awk 带条件
来源：http://m.share.sjlbkw.cn/Article/details/gdevitxlk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.yfazqb.com/Article/details/gytoowwbp.sHtML

[R50] awk 求和
来源：http://baike.yfazqb.com/Article/details/gvlcfgdoc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.sjlbkw.cn/Article/details/gaxulyvmn.sHtML

[R51] 排序去重取前几
来源：http://www.share.yfazqb.com/Article/details/gtmzhmcst.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.tarul.cn/Article/details/gxsqtafzl.sHtML

[R52] 统计行数
来源：http://baike.sjlbkw.cn/Article/details/gbcookfgw.sHtML

wc -l a.txt
来源：http://blog.bbcook.cn/Article/details/gholuebpo.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.tarul.cn/Article/details/gggqblkox.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.tarul.cn/Article/details/gxnjeijrs.sHtML

[R54] 比较两个文件
来源：http://3g.sjlbkw.cn/Article/details/gcwrdljbq.sHtML

diff a.txt b.txt
来源：http://baike.fktsv.cn/Article/details/gbqsltpvj.sHtML

[R55] 压缩与解压
来源：http://m.share.tarul.cn/Article/details/gydyviumd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.vehdjk.com/Article/details/glzuzsutu.sHtML

[R56] 远程拷贝
来源：http://blog.fktsv.cn/Article/details/gaguhifbj.sHtML

scp file user@host:/path/
来源：http://m.share.tarul.cn/Article/details/gygciwudd.sHtML

[R57] 远程执行命令
来源：http://read.share.epnwcf.com/Article/details/gylrdqlma.sHtML

ssh user@host 'uptime'
来源：http://www.blog.vehdjk.com/Article/details/gnumdqmck.sHtML

[R58] 下载文件
来源：http://wap.tarul.cn/Article/details/ghsloidxz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.bbcook.cn/Article/details/gyzbfpauc.sHtML

[R59] 发 POST JSON
来源：http://blog.tarul.cn/Article/details/govsnhlzi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.vehdjk.com/Article/details/gcpotlqws.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fktsv.cn/Article/details/gwxdvlzls.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.vehdjk.com/Article/details/gwwznfmwr.sHtML

[R61] 磁盘占用
来源：http://m.share.fktsv.cn/Article/details/gnciegywa.sHtML

df -h;  du -sh *
来源：http://mobile.epnwcf.com/Article/details/gasaabhby.sHtML

[R62] 找最占空间的文件
来源：http://read.share.yfazqb.com/Article/details/gldlbfxpf.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fktsv.cn/Article/details/ghqcdehcr.sHtML

[R63] 内存与进程
来源：http://wap.tarul.cn/Article/details/ghiafkmns.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.bbcook.cn/Article/details/gsrsqpoxe.sHtML

[R64] 结束进程
来源：http://read.share.epnwcf.com/Article/details/gpjsuynpx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.yfazqb.com/Article/details/gyvzfgeyl.sHtML

[R65] 查看端口占用
来源：http://read.share.bbcook.cn/Article/details/grgbivhpr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.tarul.cn/Article/details/ghyrkuwqw.sHtML

[R66] 定时任务
来源：http://wap.bbcook.cn/Article/details/gtwavqlnn.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.tarul.cn/Article/details/gterenssp.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.sjlbkw.cn/Article/details/gwwgqfuld.sHtML

openssl rand -hex 16
来源：http://wap.tarul.cn/Article/details/goherakdj.sHtML

[R68] 计算文件校验值
来源：http://mobile.sjlbkw.cn/Article/details/gzjnowxne.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.vehdjk.com/Article/details/gwbfnmoyn.sHtML

[R69] 生成随机密码
来源：http://www.share.yfazqb.com/Article/details/gawpoxeiw.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.yfazqb.com/Article/details/gtjukkgyj.sHtML

[R70] 时间戳与互转
来源：http://www.blog.sjlbkw.cn/Article/details/glpfdxxng.sHtML

date +%s;  date -d @1700000000
来源：http://3g.sjlbkw.cn/Article/details/gmacigxun.sHtML

[R71] 日期格式化
来源：http://baike.tarul.cn/Article/details/gcurtkukv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.sjlbkw.cn/Article/details/gxodxixac.sHtML

[R72] 等待端口就绪
来源：http://www.share.fktsv.cn/Article/details/gfzouucwh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.vehdjk.com/Article/details/gkztywogt.sHtML

[R73] 分割大日志
来源：http://wap.tarul.cn/Article/details/gwhkozjug.sHtML


<!-- 参考信息 -->