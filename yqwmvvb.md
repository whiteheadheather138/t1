代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.sjlbkw.cn/Article/details/gunyftnwj.sHtML

[Q20] IN 列表
来源：http://baike.fktsv.cn/Article/details/gakbnlzfe.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fktsv.cn/Article/details/gylemqusc.sHtML

[Q21] 空值判断
来源：http://baike.epnwcf.com/Article/details/gkifsryuo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fktsv.cn/Article/details/gamuwnkcv.sHtML

[Q22] 排序
来源：http://mobile.tarul.cn/Article/details/gqrjetwiv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fktsv.cn/Article/details/gkjlaffis.sHtML

[Q23] 分页
来源：http://baike.fktsv.cn/Article/details/gpscpnbiv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.vehdjk.com/Article/details/gcouocxgm.sHtML

[Q24] 去重
来源：http://www.share.yfazqb.com/Article/details/gqvwiorll.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/ghpvbtrna.sHtML

[Q25] 只取前 N 条
来源：http://wap.vehdjk.com/Article/details/gzkqbekhi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.tarul.cn/Article/details/gyykuplub.sHtML

[Q26] 计数
来源：http://wap.tarul.cn/Article/details/gywkvqrly.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.yfazqb.com/Article/details/goocxegnl.sHtML

[Q27] 条件计数
来源：http://www.blog.vehdjk.com/Article/details/gqjtquopg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.sjlbkw.cn/Article/details/geyjpgcry.sHtML

[Q28] 求和与平均
来源：http://blog.yfazqb.com/Article/details/gddezycsd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fktsv.cn/Article/details/gchbcmtqe.sHtML

[Q29] 最大最小值
来源：http://wap.sjlbkw.cn/Article/details/gvjdjfcrk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.vehdjk.com/Article/details/gfsqswlfw.sHtML

[Q30] 分组统计
来源：http://wap.vehdjk.com/Article/details/gzgjqkmnl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.sjlbkw.cn/Article/details/giavrlins.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.tarul.cn/Article/details/gblfokchh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.yfazqb.com/Article/details/gmrcncjrf.sHtML

[Q32] 分组拼接字符串
来源：http://wap.tarul.cn/Article/details/gerrfopid.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.epnwcf.com/Article/details/gswaickqs.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.yfazqb.com/Article/details/goczqrcvg.sHtML

[Q33] 多列分组
来源：http://read.share.fktsv.cn/Article/details/gcfswxprn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.sjlbkw.cn/Article/details/gwbrxvlgz.sHtML

[Q34] 每组取第一条
来源：http://mobile.tarul.cn/Article/details/gumhpvpbw.sHtML

SELECT * FROM (
来源：http://baike.fktsv.cn/Article/details/gtkjbcllk.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.epnwcf.com/Article/details/ghrcaonus.sHtML

) t WHERE rn = 1;
来源：http://mobile.fktsv.cn/Article/details/grctoejgs.sHtML

[Q35] 内连接
来源：http://blog.bbcook.cn/Article/details/guymlrzex.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.epnwcf.com/Article/details/gjgpgfpdc.sHtML

[Q36] 左连接
来源：http://blog.epnwcf.com/Article/details/gyzlkbhqw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.bbcook.cn/Article/details/gtzjstxuq.sHtML

[Q37] 右连接
来源：http://baike.epnwcf.com/Article/details/gyrhmhqqp.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fktsv.cn/Article/details/gqvagsfsv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fktsv.cn/Article/details/gfzpypani.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.epnwcf.com/Article/details/gpdzissxd.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.vehdjk.com/Article/details/gyjsstjnf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.yfazqb.com/Article/details/garxyjtag.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.yfazqb.com/Article/details/gjedtfpcq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fktsv.cn/Article/details/gvhzjepel.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fktsv.cn/Article/details/gwlmiwxfh.sHtML

[Q41] 多表连接
来源：http://3g.epnwcf.com/Article/details/ghgyxfcdw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.bbcook.cn/Article/details/grpgfmgcn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.yfazqb.com/Article/details/gojdputyr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.sjlbkw.cn/Article/details/gdzmgtvkd.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.sjlbkw.cn/Article/details/gtihbnaap.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.vehdjk.com/Article/details/gfuuvpucl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fktsv.cn/Article/details/gayofjxht.sHtML

[Q43] 标量子查询
来源：http://read.share.yfazqb.com/Article/details/gswyiplab.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.sjlbkw.cn/Article/details/gmyirqezx.sHtML

[Q44] IN 子查询
来源：http://blog.epnwcf.com/Article/details/gqlgkbvna.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fktsv.cn/Article/details/gzhewrcej.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.vehdjk.com/Article/details/gpprkvjls.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fktsv.cn/Article/details/gkpwpngmj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.yfazqb.com/Article/details/gjizczhiq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fktsv.cn/Article/details/glzvqfbhg.sHtML

[Q47] 与平均值比较
来源：http://blog.vehdjk.com/Article/details/gzptiwrvk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.sjlbkw.cn/Article/details/glhxurogm.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.bbcook.cn/Article/details/gwsffpyto.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.sjlbkw.cn/Article/details/gyyeujizr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fktsv.cn/Article/details/gdkdszgtc.sHtML

[Q49] 更新单行
来源：http://mobile.yfazqb.com/Article/details/gpbboiubr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.vehdjk.com/Article/details/gyunirrnb.sHtML

[Q50] 批量更新
来源：http://blog.epnwcf.com/Article/details/gtfgzffdw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.yfazqb.com/Article/details/ghadigfjb.sHtML

[Q51] 用子查询更新
来源：http://www.share.sjlbkw.cn/Article/details/gkderavyo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.vehdjk.com/Article/details/gwynnkojd.sHtML

[Q52] 删除指定行
来源：http://read.share.yfazqb.com/Article/details/gcqcmcdiq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.yfazqb.com/Article/details/gxbmexmbf.sHtML

[Q53] 按条件删除
来源：http://3g.tarul.cn/Article/details/gksorpgro.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.sjlbkw.cn/Article/details/glooeawla.sHtML

[Q54] 清空表
来源：http://www.blog.bbcook.cn/Article/details/gwxzqdztp.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.vehdjk.com/Article/details/gmfcegbbh.sHtML

[Q55] 排名（并列占位）
来源：http://blog.yfazqb.com/Article/details/gxbwmhbmg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.bbcook.cn/Article/details/gsnboolkg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.vehdjk.com/Article/details/gyxazcvck.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fktsv.cn/Article/details/gpzqfldrb.sHtML

[Q57] 行号
来源：http://blog.sjlbkw.cn/Article/details/gqjdndhgu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.yfazqb.com/Article/details/gupxacbas.sHtML

[Q58] 累计求和
来源：http://www.m.share.tarul.cn/Article/details/gqhrwmaug.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.vehdjk.com/Article/details/gbtdadzvk.sHtML

[Q59] 分组内累计
来源：http://m.share.sjlbkw.cn/Article/details/gcirfbbun.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.yfazqb.com/Article/details/gixndvelp.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.tarul.cn/Article/details/gcyqfrdue.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.yfazqb.com/Article/details/gagkhswdo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.yfazqb.com/Article/details/ggovilkza.sHtML

[Q61] 移动平均
来源：http://mobile.sjlbkw.cn/Article/details/gskdoheld.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fktsv.cn/Article/details/gwwatuqjf.sHtML

[Q62] 分组占比
来源：http://3g.vehdjk.com/Article/details/gnuppssuh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.tarul.cn/Article/details/guuyhqyqo.sHtML

[Q63] 开启事务
来源：http://read.share.fktsv.cn/Article/details/gvujlnnky.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.sjlbkw.cn/Article/details/gqfeexoad.sHtML

[Q64] 提交事务
来源：http://blog.sjlbkw.cn/Article/details/ghnqakmde.sHtML

COMMIT;
来源：http://www.blog.sjlbkw.cn/Article/details/gcpykzgrw.sHtML

[Q65] 回滚事务
来源：http://www.blog.vehdjk.com/Article/details/glosmvwbx.sHtML

ROLLBACK;
来源：http://3g.sjlbkw.cn/Article/details/gajgmmiuw.sHtML

[Q66] 行锁查询
来源：http://3g.epnwcf.com/Article/details/gvstemopl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.vehdjk.com/Article/details/gaxgtpmwo.sHtML

[Q67] 设置隔离级别
来源：http://mobile.bbcook.cn/Article/details/gjupsvezm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.yfazqb.com/Article/details/gvvywwsms.sHtML

[Q68] 保存点
来源：http://3g.epnwcf.com/Article/details/gfnvoapui.sHtML

SAVEPOINT sp1;
来源：http://read.share.fktsv.cn/Article/details/gzcecoqut.sHtML

ROLLBACK TO sp1;
来源：http://3g.yfazqb.com/Article/details/gajputdsc.sHtML

[Q69] 查看执行计划
来源：http://read.share.tarul.cn/Article/details/gmcjuftke.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.tarul.cn/Article/details/gpxyqdhvb.sHtML

[Q70] 更新统计信息
来源：http://wap.sjlbkw.cn/Article/details/gnonkfsgs.sHtML

ANALYZE TABLE users;
来源：http://wap.fktsv.cn/Article/details/gvwmzxdie.sHtML

[Q71] 查看建表语句
来源：http://www.blog.epnwcf.com/Article/details/gzrtfaxer.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.bbcook.cn/Article/details/gpsepheqj.sHtML

[Q72] 查看索引
来源：http://www.m.share.tarul.cn/Article/details/gqpnwayrp.sHtML

SHOW INDEX FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gvubhjcru.sHtML

[Q73] 查看表状态
来源：http://baike.fktsv.cn/Article/details/gzqnxbzdu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.epnwcf.com/Article/details/gifaflayb.sHtML

[Q74] 强制使用索引
来源：http://3g.bbcook.cn/Article/details/gztnhrxgd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.vehdjk.com/Article/details/girthrcpb.sHtML

[Q75] 日期格式化
来源：http://mobile.yfazqb.com/Article/details/gytyxzvcq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.epnwcf.com/Article/details/gvccdhgnf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.bbcook.cn/Article/details/ggfobnshn.sHtML

[Q76] 按天统计
来源：http://baike.tarul.cn/Article/details/gvmlbdizs.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.yfazqb.com/Article/details/gybklhwvj.sHtML

[Q77] 时间加减
来源：http://www.m.share.sjlbkw.cn/Article/details/giusmpzrm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fktsv.cn/Article/details/gbrspqumx.sHtML

[Q78] 当前时间
来源：http://blog.sjlbkw.cn/Article/details/gbvmpzzbu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.epnwcf.com/Article/details/gsnvtgymr.sHtML

[Q79] 字符串拼接
来源：http://www.share.sjlbkw.cn/Article/details/gecwccbwo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.bbcook.cn/Article/details/gmlsbvzuj.sHtML

[Q80] 字符串截取
来源：http://www.m.share.vehdjk.com/Article/details/ggvqxezbw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.vehdjk.com/Article/details/gadrqiipw.sHtML

[Q81] 字符串替换
来源：http://read.share.bbcook.cn/Article/details/gvkhtbosv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.epnwcf.com/Article/details/guxlvrxta.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.sjlbkw.cn/Article/details/gvfnsukjp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.epnwcf.com/Article/details/gxwqxhekk.sHtML

[Q83] 大小写转换
来源：http://www.blog.epnwcf.com/Article/details/gvwcnclix.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.vehdjk.com/Article/details/glwfkdeju.sHtML

[Q84] 去除首尾空格
来源：http://m.share.yfazqb.com/Article/details/gowenvjfb.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gjgaourhs.sHtML

[Q85] 数值取整
来源：http://www.m.share.bbcook.cn/Article/details/gmwzkahwz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.epnwcf.com/Article/details/gqsbjpipu.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.tarul.cn/Article/details/gpnwxsask.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.tarul.cn/Article/details/gddkiypca.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.bbcook.cn/Article/details/gzbyggcll.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.tarul.cn/Article/details/gwnobteld.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.bbcook.cn/Article/details/gjbxhgdya.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fktsv.cn/Article/details/gxtftyyaz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.vehdjk.com/Article/details/glhyuyswb.sHtML

[Q89] 判断表是否存在
来源：http://blog.bbcook.cn/Article/details/gaeyzvatl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.sjlbkw.cn/Article/details/gojpmkxvo.sHtML

[Q90] 生成序号列
来源：http://www.m.share.tarul.cn/Article/details/gimjhlxcw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.yfazqb.com/Article/details/gvnzbydke.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gpfwbsqif.sHtML

R. Bash 专题
来源：http://baike.sjlbkw.cn/Article/details/gsyilsubl.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gwzperkkf.sHtML

[R01] shebang 与严格模式
来源：http://mobile.sjlbkw.cn/Article/details/gqmlhexme.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.yfazqb.com/Article/details/gvyjbbcro.sHtML

set -euo pipefail
来源：http://baike.bbcook.cn/Article/details/gieovggvn.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.yfazqb.com/Article/details/gjhyzhyka.sHtML

name="Tom"; echo "$name"
来源：http://mobile.tarul.cn/Article/details/gqkyftwyw.sHtML

[R03] 只读变量
来源：http://www.m.share.yfazqb.com/Article/details/gzngcfihk.sHtML

readonly PI=3.14
来源：http://mobile.vehdjk.com/Article/details/gkryynovc.sHtML

[R04] 位置参数
来源：http://wap.vehdjk.com/Article/details/gccijimuo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.yfazqb.com/Article/details/gaytwwrzw.sHtML

[R05] 参数默认值
来源：http://read.share.epnwcf.com/Article/details/gqllrfwrg.sHtML

name="${1:-default}"
来源：http://mobile.sjlbkw.cn/Article/details/grxxgiuti.sHtML

[R06] 判断命令是否存在
来源：http://wap.tarul.cn/Article/details/gxwhfdyvt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.tarul.cn/Article/details/gvlpqzaxq.sHtML

[R07] if 判断文件
来源：http://www.share.vehdjk.com/Article/details/glxbclbzr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.yfazqb.com/Article/details/gsruccbmy.sHtML

[R08] 数值比较
来源：http://mobile.vehdjk.com/Article/details/gasyqttxn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.yfazqb.com/Article/details/gnpxqsblk.sHtML

[R09] 字符串比较
来源：http://3g.bbcook.cn/Article/details/gajvqirkt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.epnwcf.com/Article/details/gsdavsfdy.sHtML

[R10] 正则匹配
来源：http://mobile.tarul.cn/Article/details/gethygltr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.tarul.cn/Article/details/gsqmtmokp.sHtML

[R11] case 多分支
来源：http://3g.yfazqb.com/Article/details/gkysqpnnu.sHtML

case "$1" in
来源：http://wap.fktsv.cn/Article/details/gasofykpm.sHtML

start) echo "启动" ;;
来源：http://read.share.sjlbkw.cn/Article/details/gjpngyqpd.sHtML

stop)  echo "停止" ;;
来源：http://mobile.yfazqb.com/Article/details/ghhfhafvu.sHtML

*)     echo "未知命令" ;;
来源：http://wap.vehdjk.com/Article/details/ggbisqsdg.sHtML

esac
来源：http://read.share.fktsv.cn/Article/details/gmthrqppd.sHtML

[R12] for 遍历文件
来源：http://blog.sjlbkw.cn/Article/details/gfpvlyxuk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.epnwcf.com/Article/details/gkhavtizv.sHtML

[R13] for 计数循环
来源：http://3g.vehdjk.com/Article/details/gfxijfzoc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.bbcook.cn/Article/details/gletdbbpg.sHtML

[R14] C 风格 for
来源：http://www.share.tarul.cn/Article/details/gwsxqsssk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.tarul.cn/Article/details/gzajcmprw.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.vehdjk.com/Article/details/gznmkflzk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.vehdjk.com/Article/details/gkcxfihsj.sHtML

[R16] until 等待条件
来源：http://www.m.share.yfazqb.com/Article/details/gvidtnmpl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.bbcook.cn/Article/details/glorucmnf.sHtML

[R17] 数组定义与取值
来源：http://mobile.fktsv.cn/Article/details/gofwoxpqi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fktsv.cn/Article/details/grvouqwzv.sHtML

[R18] 遍历数组
来源：http://3g.fktsv.cn/Article/details/gyzpywzei.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.sjlbkw.cn/Article/details/gclgldxnj.sHtML

[R19] 数组长度
来源：http://wap.vehdjk.com/Article/details/givircrmt.sHtML

echo "${#arr[@]}"
来源：http://mobile.sjlbkw.cn/Article/details/gzqkkmtqy.sHtML

[R20] 关联数组（字典）
来源：http://www.share.yfazqb.com/Article/details/ggpzrlhqr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.vehdjk.com/Article/details/gvjlothdr.sHtML

[R21] 字符串长度
来源：http://3g.tarul.cn/Article/details/gsnqzvgqe.sHtML

echo "${#s}"
来源：http://m.share.tarul.cn/Article/details/gkwsafaxy.sHtML

[R22] 截取子串
来源：http://blog.yfazqb.com/Article/details/gqvyrwiak.sHtML

echo "${s:0:5}"
来源：http://blog.vehdjk.com/Article/details/gpzuirjfi.sHtML

[R23] 字符串替换
来源：http://m.share.epnwcf.com/Article/details/gtgegsrsn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fktsv.cn/Article/details/gvtbyxfga.sHtML

[R24] 大小写转换
来源：http://blog.yfazqb.com/Article/details/gjcjaypfu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.bbcook.cn/Article/details/gjworacun.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.vehdjk.com/Article/details/gdqbqxusu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.tarul.cn/Article/details/gcbgezxnc.sHtML

[R26] 命令替换
来源：http://baike.bbcook.cn/Article/details/gkkuitckk.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fktsv.cn/Article/details/gbjtsrobw.sHtML

[R27] 算术展开
来源：http://mobile.bbcook.cn/Article/details/gwsegepfn.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.tarul.cn/Article/details/gywyeeyzd.sHtML

[R28] 浮点运算
来源：http://mobile.fktsv.cn/Article/details/gudepetdj.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.tarul.cn/Article/details/giuxvfvav.sHtML

[R29] 定义函数
来源：http://www.share.fktsv.cn/Article/details/gyzaqqfbr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.tarul.cn/Article/details/gmnomuigv.sHtML

[R30] 函数返回状态码
来源：http://www.share.yfazqb.com/Article/details/gvrbhktnj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.bbcook.cn/Article/details/gppohdqsp.sHtML

[R31] 局部变量
来源：http://mobile.epnwcf.com/Article/details/gxejtjprm.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.sjlbkw.cn/Article/details/gjrcqecri.sHtML

[R32] 参数个数校验
来源：http://baike.bbcook.cn/Article/details/gjtgnggpu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.vehdjk.com/Article/details/gfdymboqv.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.yfazqb.com/Article/details/gvtkfylgg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.sjlbkw.cn/Article/details/gyhoefwgw.sHtML

[R34] 退出时清理
来源：http://www.blog.vehdjk.com/Article/details/gymnvjuuk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.tarul.cn/Article/details/gnpcqttlz.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.bbcook.cn/Article/details/gbnyaykby.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fktsv.cn/Article/details/gbtlbnwgz.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.vehdjk.com/Article/details/gwnfpcrkh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.yfazqb.com/Article/details/ggrhcgncs.sHtML

[R37] 把输出赋给变量
来源：http://m.share.yfazqb.com/Article/details/gxkmywbtu.sHtML

files=$(ls -1)
来源：http://www.share.fktsv.cn/Article/details/gheatfgdy.sHtML

[R38] 管道串联
来源：http://wap.bbcook.cn/Article/details/gnsnivkly.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.epnwcf.com/Article/details/gntrztuly.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.bbcook.cn/Article/details/ggxzcqxdc.sHtML

cmd > out.log 2>&1
来源：http://m.share.sjlbkw.cn/Article/details/gcefspved.sHtML

[R40] 追加写日志
来源：http://www.m.share.yfazqb.com/Article/details/glrxxnzvz.sHtML

echo "log" >> out.log
来源：http://www.m.share.fktsv.cn/Article/details/gphcpvrrl.sHtML

[R41] 丢弃输出
来源：http://www.share.sjlbkw.cn/Article/details/gadtsfwfl.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.yfazqb.com/Article/details/gjabfigcf.sHtML

[R42] 输入重定向
来源：http://www.blog.sjlbkw.cn/Article/details/gwciwrqmx.sHtML

wc -l < a.txt
来源：http://www.m.share.yfazqb.com/Article/details/gnoylxyce.sHtML

[R43] 按名字查找文件
来源：http://baike.fktsv.cn/Article/details/grvmpkufy.sHtML

find . -name "*.log" -type f
来源：http://blog.bbcook.cn/Article/details/gpvjpypkx.sHtML

[R44] 按修改时间查找
来源：http://3g.vehdjk.com/Article/details/gsgzpffjq.sHtML

find . -mtime -7 -type f
来源：http://3g.fktsv.cn/Article/details/ggzfwjspz.sHtML

[R45] 批量删除
来源：http://m.share.epnwcf.com/Article/details/gcemdqosl.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.sjlbkw.cn/Article/details/gjlfyvces.sHtML

[R46] 递归替换文件内容
来源：http://mobile.yfazqb.com/Article/details/gxajllbao.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.tarul.cn/Article/details/gqlkdkswk.sHtML

[R47] sed 单行替换
来源：http://m.share.sjlbkw.cn/Article/details/gimtkmxnr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.bbcook.cn/Article/details/gjvrnzavw.sHtML

[R48] awk 取指定列
来源：http://blog.fktsv.cn/Article/details/gtnekoisj.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.bbcook.cn/Article/details/gzsbvnjgk.sHtML

[R49] awk 带条件
来源：http://www.m.share.fktsv.cn/Article/details/gfeexmrpw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.epnwcf.com/Article/details/gbcyiibpm.sHtML

[R50] awk 求和
来源：http://www.m.share.tarul.cn/Article/details/gippuxolv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gbjpiyjwx.sHtML

[R51] 排序去重取前几
来源：http://read.share.yfazqb.com/Article/details/gnqksqmyt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.vehdjk.com/Article/details/gjdiegfdd.sHtML

[R52] 统计行数
来源：http://mobile.epnwcf.com/Article/details/gkghdvmdy.sHtML

wc -l a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/groylruwe.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.vehdjk.com/Article/details/gsocmdgxr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.tarul.cn/Article/details/ghfkjirfp.sHtML

[R54] 比较两个文件
来源：http://mobile.vehdjk.com/Article/details/guoxrsxmc.sHtML

diff a.txt b.txt
来源：http://www.share.tarul.cn/Article/details/gaqdptcni.sHtML

[R55] 压缩与解压
来源：http://blog.bbcook.cn/Article/details/gqojqqxwd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.sjlbkw.cn/Article/details/gqrejiydx.sHtML

[R56] 远程拷贝
来源：http://www.m.share.bbcook.cn/Article/details/gpfpwgucv.sHtML

scp file user@host:/path/
来源：http://baike.epnwcf.com/Article/details/gbzkodxul.sHtML

[R57] 远程执行命令
来源：http://read.share.fktsv.cn/Article/details/ggcloalmd.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.yfazqb.com/Article/details/gxuustndi.sHtML

[R58] 下载文件
来源：http://www.blog.fktsv.cn/Article/details/ggneirtel.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.sjlbkw.cn/Article/details/gijclfjah.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.tarul.cn/Article/details/gysawjruj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.bbcook.cn/Article/details/gelpsemvu.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.sjlbkw.cn/Article/details/gthjakqus.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.epnwcf.com/Article/details/gcovfmtky.sHtML

[R61] 磁盘占用
来源：http://www.m.share.sjlbkw.cn/Article/details/gklryopsi.sHtML

df -h;  du -sh *
来源：http://m.share.bbcook.cn/Article/details/gvqkylkos.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fktsv.cn/Article/details/gibgdseyi.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.yfazqb.com/Article/details/gixxjetgy.sHtML

[R63] 内存与进程
来源：http://mobile.bbcook.cn/Article/details/gutjjgwpd.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.epnwcf.com/Article/details/ghjvxypkw.sHtML

[R64] 结束进程
来源：http://www.share.epnwcf.com/Article/details/giriqbkgc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fktsv.cn/Article/details/gbwosrhgq.sHtML

[R65] 查看端口占用
来源：http://3g.tarul.cn/Article/details/grhbgfwdi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fktsv.cn/Article/details/gzxtprxdd.sHtML

[R66] 定时任务
来源：http://blog.bbcook.cn/Article/details/gbrduymga.sHtML

crontab -e;  crontab -l
来源：http://read.share.epnwcf.com/Article/details/gpfebhrgd.sHtML

[R67] 生成随机十六进制串
来源：http://blog.sjlbkw.cn/Article/details/gqdcffncw.sHtML

openssl rand -hex 16
来源：http://3g.sjlbkw.cn/Article/details/ghidzfujz.sHtML

[R68] 计算文件校验值
来源：http://read.share.fktsv.cn/Article/details/ggbdcrglj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fktsv.cn/Article/details/gbqqacojl.sHtML

[R69] 生成随机密码
来源：http://blog.epnwcf.com/Article/details/gnnvlhzsk.sHtML


<!-- 参考信息 -->