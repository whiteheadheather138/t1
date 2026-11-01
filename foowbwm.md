代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.yfazqb.com/Article/details/gklosuxmj.sHtML

[Q22] 排序
来源：http://3g.bbcook.cn/Article/details/gxormflbs.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.vehdjk.com/Article/details/gcrtldext.sHtML

[Q23] 分页
来源：http://www.blog.tarul.cn/Article/details/gzenivwum.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.vehdjk.com/Article/details/gwcxxzxew.sHtML

[Q24] 去重
来源：http://www.m.share.fktsv.cn/Article/details/grsbjvigv.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.vehdjk.com/Article/details/gpssghxkx.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.sjlbkw.cn/Article/details/gboboygks.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.yfazqb.com/Article/details/gwqqeurne.sHtML

[Q26] 计数
来源：http://mobile.tarul.cn/Article/details/gszkgtsum.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.yfazqb.com/Article/details/goiwfovyb.sHtML

[Q27] 条件计数
来源：http://www.share.sjlbkw.cn/Article/details/gxlowvexl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.yfazqb.com/Article/details/guktuukgr.sHtML

[Q28] 求和与平均
来源：http://read.share.bbcook.cn/Article/details/gubdiwzjg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.yfazqb.com/Article/details/gzzlciquq.sHtML

[Q29] 最大最小值
来源：http://blog.yfazqb.com/Article/details/gqeitmtgg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fktsv.cn/Article/details/gokscgxqk.sHtML

[Q30] 分组统计
来源：http://www.m.share.tarul.cn/Article/details/glmbxzosd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fktsv.cn/Article/details/gopyzvjyo.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fktsv.cn/Article/details/gfyipgdnm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.tarul.cn/Article/details/ghttstocg.sHtML

[Q32] 分组拼接字符串
来源：http://3g.epnwcf.com/Article/details/guommaavm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.tarul.cn/Article/details/gxsrfybrm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fktsv.cn/Article/details/gltpcmilq.sHtML

[Q33] 多列分组
来源：http://wap.tarul.cn/Article/details/gufkfzjvw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.sjlbkw.cn/Article/details/gtogqomzf.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fktsv.cn/Article/details/gfepmugir.sHtML

SELECT * FROM (
来源：http://3g.vehdjk.com/Article/details/gluexfgsu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fktsv.cn/Article/details/gjsmogolr.sHtML

) t WHERE rn = 1;
来源：http://baike.bbcook.cn/Article/details/gohgmcizr.sHtML

[Q35] 内连接
来源：http://www.share.yfazqb.com/Article/details/glbitmggk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.sjlbkw.cn/Article/details/gbjtdezsa.sHtML

[Q36] 左连接
来源：http://www.blog.fktsv.cn/Article/details/gfrlcfjaj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.yfazqb.com/Article/details/gevsveane.sHtML

[Q37] 右连接
来源：http://blog.sjlbkw.cn/Article/details/gzinlqtxd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.bbcook.cn/Article/details/gpvgjwijr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fktsv.cn/Article/details/gjbncelit.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fktsv.cn/Article/details/gzcwejbcw.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.yfazqb.com/Article/details/goydjcekp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.bbcook.cn/Article/details/gguysjuyd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.vehdjk.com/Article/details/gaylbtpdm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.sjlbkw.cn/Article/details/gebjjhqzk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.vehdjk.com/Article/details/gbcllrpzm.sHtML

[Q41] 多表连接
来源：http://blog.fktsv.cn/Article/details/gpoqsrhsl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.yfazqb.com/Article/details/glvfhrghe.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fktsv.cn/Article/details/gurqkkbqo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.sjlbkw.cn/Article/details/ghwwvjvoo.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.epnwcf.com/Article/details/gtdftdtgq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.tarul.cn/Article/details/gzyqlohcj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fktsv.cn/Article/details/gxanweahz.sHtML

[Q43] 标量子查询
来源：http://wap.epnwcf.com/Article/details/gbzmtycvb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.epnwcf.com/Article/details/gjrdirexn.sHtML

[Q44] IN 子查询
来源：http://www.share.sjlbkw.cn/Article/details/gbspojnjl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.sjlbkw.cn/Article/details/gcvvglbtk.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fktsv.cn/Article/details/gegtybjqa.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.sjlbkw.cn/Article/details/gnkltiplo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.epnwcf.com/Article/details/gwglkofmd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.yfazqb.com/Article/details/glnbboirq.sHtML

[Q47] 与平均值比较
来源：http://blog.epnwcf.com/Article/details/gvcxopjik.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.bbcook.cn/Article/details/gtezhzzkc.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.vehdjk.com/Article/details/gozecmjmo.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.sjlbkw.cn/Article/details/guxrnbfvc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.vehdjk.com/Article/details/gkkoohwbz.sHtML

[Q49] 更新单行
来源：http://m.share.epnwcf.com/Article/details/gyhlkpwgz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.tarul.cn/Article/details/gratrunhy.sHtML

[Q50] 批量更新
来源：http://www.m.share.tarul.cn/Article/details/gtnoruccg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.tarul.cn/Article/details/gytblvuos.sHtML

[Q51] 用子查询更新
来源：http://3g.bbcook.cn/Article/details/gbbpwvobd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.epnwcf.com/Article/details/gdklkprri.sHtML

[Q52] 删除指定行
来源：http://blog.epnwcf.com/Article/details/gsjxnykxz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.epnwcf.com/Article/details/ghlwesyer.sHtML

[Q53] 按条件删除
来源：http://www.m.share.bbcook.cn/Article/details/ggdcszmhc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.sjlbkw.cn/Article/details/gamlxbvsz.sHtML

[Q54] 清空表
来源：http://blog.fktsv.cn/Article/details/gzgtuefrf.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.yfazqb.com/Article/details/guhfwcbkb.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.yfazqb.com/Article/details/gcmzfiruz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.yfazqb.com/Article/details/goucfwhbm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.vehdjk.com/Article/details/gyagzrylr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fktsv.cn/Article/details/graasplkv.sHtML

[Q57] 行号
来源：http://baike.vehdjk.com/Article/details/gakillmot.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gohwnjpqs.sHtML

[Q58] 累计求和
来源：http://blog.fktsv.cn/Article/details/glwurcprw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/gpktmflsl.sHtML

[Q59] 分组内累计
来源：http://www.share.sjlbkw.cn/Article/details/gcemhywnx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.vehdjk.com/Article/details/gtzktzauo.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.yfazqb.com/Article/details/gxloygfih.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.vehdjk.com/Article/details/gymhjlgnf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.yfazqb.com/Article/details/gmopqktpy.sHtML

[Q61] 移动平均
来源：http://mobile.vehdjk.com/Article/details/gxzwlxdqp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.epnwcf.com/Article/details/golfcdubp.sHtML

[Q62] 分组占比
来源：http://baike.vehdjk.com/Article/details/gackcvbqh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.yfazqb.com/Article/details/gwzdbgeva.sHtML

[Q63] 开启事务
来源：http://blog.sjlbkw.cn/Article/details/gtuupbdmn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.sjlbkw.cn/Article/details/gonrpahdk.sHtML

[Q64] 提交事务
来源：http://baike.yfazqb.com/Article/details/gedfgpsnr.sHtML

COMMIT;
来源：http://read.share.sjlbkw.cn/Article/details/gmamlhvab.sHtML

[Q65] 回滚事务
来源：http://wap.fktsv.cn/Article/details/gprrpfcaq.sHtML

ROLLBACK;
来源：http://mobile.tarul.cn/Article/details/gsiotbxdv.sHtML

[Q66] 行锁查询
来源：http://www.m.share.vehdjk.com/Article/details/ggbhipsij.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.tarul.cn/Article/details/gnvwxqgzp.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.epnwcf.com/Article/details/gpjhcjjlm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.yfazqb.com/Article/details/gqtwaotun.sHtML

[Q68] 保存点
来源：http://mobile.bbcook.cn/Article/details/ghunamybn.sHtML

SAVEPOINT sp1;
来源：http://3g.sjlbkw.cn/Article/details/gfcpzglno.sHtML

ROLLBACK TO sp1;
来源：http://wap.bbcook.cn/Article/details/gyxbxeghk.sHtML

[Q69] 查看执行计划
来源：http://mobile.vehdjk.com/Article/details/gjupymyzq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.tarul.cn/Article/details/gweczbwgf.sHtML

[Q70] 更新统计信息
来源：http://wap.tarul.cn/Article/details/ghslnkxts.sHtML

ANALYZE TABLE users;
来源：http://blog.yfazqb.com/Article/details/glvltngmy.sHtML

[Q71] 查看建表语句
来源：http://read.share.yfazqb.com/Article/details/gfeicvzgn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.epnwcf.com/Article/details/gtaywgwst.sHtML

[Q72] 查看索引
来源：http://baike.sjlbkw.cn/Article/details/gpezrfzbw.sHtML

SHOW INDEX FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gcezqxogq.sHtML

[Q73] 查看表状态
来源：http://baike.tarul.cn/Article/details/gcutsednm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.vehdjk.com/Article/details/gyadbixhw.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fktsv.cn/Article/details/giulkqmfo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.sjlbkw.cn/Article/details/ggequzmgw.sHtML

[Q75] 日期格式化
来源：http://m.share.yfazqb.com/Article/details/gqvkkgogl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/gigabglka.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.yfazqb.com/Article/details/gdfezbzvc.sHtML

[Q76] 按天统计
来源：http://3g.tarul.cn/Article/details/gejuedhhs.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.yfazqb.com/Article/details/gycrsoerj.sHtML

[Q77] 时间加减
来源：http://3g.tarul.cn/Article/details/gzgdjqrvz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.vehdjk.com/Article/details/gjmcppakc.sHtML

[Q78] 当前时间
来源：http://m.share.fktsv.cn/Article/details/gqkytvrhr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.tarul.cn/Article/details/gwrjshbso.sHtML

[Q79] 字符串拼接
来源：http://3g.epnwcf.com/Article/details/gvxxevuzm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.sjlbkw.cn/Article/details/gsryllfat.sHtML

[Q80] 字符串截取
来源：http://www.m.share.epnwcf.com/Article/details/gopbngpjv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fktsv.cn/Article/details/gmmidzfyc.sHtML

[Q81] 字符串替换
来源：http://wap.sjlbkw.cn/Article/details/gpiihmmon.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.epnwcf.com/Article/details/gbzhxsned.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.yfazqb.com/Article/details/gigdiolra.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.tarul.cn/Article/details/gydrmllll.sHtML

[Q83] 大小写转换
来源：http://wap.sjlbkw.cn/Article/details/gmehqiphs.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gbgtpcqmk.sHtML

[Q84] 去除首尾空格
来源：http://blog.tarul.cn/Article/details/gssglaxic.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.tarul.cn/Article/details/gizbrvbna.sHtML

[Q85] 数值取整
来源：http://www.share.bbcook.cn/Article/details/gvqaucuyw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fktsv.cn/Article/details/gzcjdwffg.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fktsv.cn/Article/details/gkdnaqcrc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.sjlbkw.cn/Article/details/geacueknu.sHtML

[Q87] JSON 字段做条件
来源：http://wap.sjlbkw.cn/Article/details/gzrmywpoq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.tarul.cn/Article/details/gcfjsuxjn.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.tarul.cn/Article/details/gfqkwocey.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.bbcook.cn/Article/details/gkjdhvpvx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gmjpepdts.sHtML

[Q89] 判断表是否存在
来源：http://read.share.bbcook.cn/Article/details/gzshobmlr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.tarul.cn/Article/details/guuxpgyek.sHtML

[Q90] 生成序号列
来源：http://read.share.vehdjk.com/Article/details/gwvrxqwpb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fktsv.cn/Article/details/ghhzhsuie.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gxfqstggt.sHtML

R. Bash 专题
来源：http://mobile.epnwcf.com/Article/details/gemqdkocd.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/glmqategg.sHtML

[R01] shebang 与严格模式
来源：http://www.share.tarul.cn/Article/details/glvxdizqu.sHtML

#!/usr/bin/env bash
来源：http://mobile.sjlbkw.cn/Article/details/grdoufzcn.sHtML

set -euo pipefail
来源：http://www.blog.sjlbkw.cn/Article/details/grfqerqdm.sHtML

[R02] 变量赋值与使用
来源：http://read.share.epnwcf.com/Article/details/gumnijsqt.sHtML

name="Tom"; echo "$name"
来源：http://3g.vehdjk.com/Article/details/gvbfzwqwu.sHtML

[R03] 只读变量
来源：http://wap.yfazqb.com/Article/details/gwwqxeygq.sHtML

readonly PI=3.14
来源：http://www.share.fktsv.cn/Article/details/gvrijvxmy.sHtML

[R04] 位置参数
来源：http://www.blog.yfazqb.com/Article/details/gdvdcuuhd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fktsv.cn/Article/details/gxojayboy.sHtML

[R05] 参数默认值
来源：http://www.blog.fktsv.cn/Article/details/ghdbdtarm.sHtML

name="${1:-default}"
来源：http://wap.fktsv.cn/Article/details/gxcpnrxly.sHtML

[R06] 判断命令是否存在
来源：http://wap.vehdjk.com/Article/details/gfekwxikq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.bbcook.cn/Article/details/gyjqoqlms.sHtML

[R07] if 判断文件
来源：http://read.share.sjlbkw.cn/Article/details/gorxruztz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.tarul.cn/Article/details/gydggmalp.sHtML

[R08] 数值比较
来源：http://www.blog.fktsv.cn/Article/details/gdiwyfsxh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.epnwcf.com/Article/details/ggambezkp.sHtML

[R09] 字符串比较
来源：http://www.share.sjlbkw.cn/Article/details/gtsceixxw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.epnwcf.com/Article/details/gfuywarak.sHtML

[R10] 正则匹配
来源：http://3g.yfazqb.com/Article/details/gfeycqiko.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.yfazqb.com/Article/details/gohmsuxcb.sHtML

[R11] case 多分支
来源：http://m.share.tarul.cn/Article/details/gwmqjfifl.sHtML

case "$1" in
来源：http://read.share.epnwcf.com/Article/details/gdcpowtfa.sHtML

start) echo "启动" ;;
来源：http://read.share.vehdjk.com/Article/details/gribpfzpi.sHtML

stop)  echo "停止" ;;
来源：http://baike.yfazqb.com/Article/details/gajfhhsya.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fktsv.cn/Article/details/gtjhbflxi.sHtML

esac
来源：http://3g.sjlbkw.cn/Article/details/gudzmyqhw.sHtML

[R12] for 遍历文件
来源：http://read.share.sjlbkw.cn/Article/details/gfdjpsbao.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.sjlbkw.cn/Article/details/gamcnivfb.sHtML

[R13] for 计数循环
来源：http://read.share.epnwcf.com/Article/details/gedxajjdo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.yfazqb.com/Article/details/gqmzlamqr.sHtML

[R14] C 风格 for
来源：http://mobile.fktsv.cn/Article/details/gxkqxjdqi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.bbcook.cn/Article/details/gbomjzwlv.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fktsv.cn/Article/details/gxcupwoqb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.yfazqb.com/Article/details/gmxdgahwk.sHtML

[R16] until 等待条件
来源：http://www.share.tarul.cn/Article/details/gebtjrpmb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fktsv.cn/Article/details/gqtcnszat.sHtML

[R17] 数组定义与取值
来源：http://3g.fktsv.cn/Article/details/gumdtjbdh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.tarul.cn/Article/details/geccdvrpz.sHtML

[R18] 遍历数组
来源：http://baike.fktsv.cn/Article/details/gncgmchlo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.sjlbkw.cn/Article/details/gnvqsqtfu.sHtML

[R19] 数组长度
来源：http://read.share.yfazqb.com/Article/details/gpjihpbcq.sHtML

echo "${#arr[@]}"
来源：http://www.blog.yfazqb.com/Article/details/gesqmltra.sHtML

[R20] 关联数组（字典）
来源：http://blog.vehdjk.com/Article/details/gygmsuvbn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.tarul.cn/Article/details/gpbfgutgd.sHtML

[R21] 字符串长度
来源：http://read.share.bbcook.cn/Article/details/gqdfahznt.sHtML

echo "${#s}"
来源：http://wap.vehdjk.com/Article/details/gzlvaydtq.sHtML

[R22] 截取子串
来源：http://www.m.share.bbcook.cn/Article/details/gfuxmuhhg.sHtML

echo "${s:0:5}"
来源：http://mobile.tarul.cn/Article/details/ggyssyqeh.sHtML

[R23] 字符串替换
来源：http://mobile.tarul.cn/Article/details/gltnjjuxw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.epnwcf.com/Article/details/gmmseznvv.sHtML

[R24] 大小写转换
来源：http://www.share.tarul.cn/Article/details/gcvngvext.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.vehdjk.com/Article/details/gsdlsbdym.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.sjlbkw.cn/Article/details/gmlavsotz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.tarul.cn/Article/details/gcxrztxrd.sHtML

[R26] 命令替换
来源：http://3g.fktsv.cn/Article/details/gzwivumji.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.tarul.cn/Article/details/gdgjzfvjw.sHtML

[R27] 算术展开
来源：http://www.blog.bbcook.cn/Article/details/gsnrcpdti.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.vehdjk.com/Article/details/gbejgmexl.sHtML

[R28] 浮点运算
来源：http://baike.yfazqb.com/Article/details/gfuaryxsc.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.yfazqb.com/Article/details/gdvikvnsh.sHtML

[R29] 定义函数
来源：http://www.blog.bbcook.cn/Article/details/guswxjlnc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.sjlbkw.cn/Article/details/gcnyjfdhi.sHtML

[R30] 函数返回状态码
来源：http://read.share.tarul.cn/Article/details/ggusmfhwv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.epnwcf.com/Article/details/gyqibdfjd.sHtML

[R31] 局部变量
来源：http://m.share.fktsv.cn/Article/details/gxcmeetsb.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.tarul.cn/Article/details/gekevcubk.sHtML

[R32] 参数个数校验
来源：http://baike.fktsv.cn/Article/details/gouirpgdk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.vehdjk.com/Article/details/ggqzoenta.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.sjlbkw.cn/Article/details/gwlqpnnzd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.sjlbkw.cn/Article/details/gwbuyeoiv.sHtML

[R34] 退出时清理
来源：http://3g.epnwcf.com/Article/details/gbknwwxwg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.epnwcf.com/Article/details/gfkkbgczx.sHtML

[R35] 后台执行并等待
来源：http://mobile.vehdjk.com/Article/details/grgwmqaov.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.tarul.cn/Article/details/gxvpnjihw.sHtML

[R36] 并发执行多个任务
来源：http://wap.yfazqb.com/Article/details/guvicydxr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.vehdjk.com/Article/details/gzimpbmrj.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.bbcook.cn/Article/details/gkheznpwx.sHtML

files=$(ls -1)
来源：http://www.blog.fktsv.cn/Article/details/gulijchta.sHtML

[R38] 管道串联
来源：http://baike.epnwcf.com/Article/details/gtjtfcnld.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fktsv.cn/Article/details/galmvtiub.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.vehdjk.com/Article/details/gbxaysezz.sHtML

cmd > out.log 2>&1
来源：http://baike.tarul.cn/Article/details/gzipfcekk.sHtML

[R40] 追加写日志
来源：http://baike.epnwcf.com/Article/details/gokkxljak.sHtML

echo "log" >> out.log
来源：http://read.share.bbcook.cn/Article/details/gtinmmfdn.sHtML

[R41] 丢弃输出
来源：http://wap.fktsv.cn/Article/details/gzhatsuwz.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.bbcook.cn/Article/details/gbhaufinf.sHtML

[R42] 输入重定向
来源：http://www.m.share.vehdjk.com/Article/details/gwzzteway.sHtML

wc -l < a.txt
来源：http://blog.epnwcf.com/Article/details/gkotvsgab.sHtML

[R43] 按名字查找文件
来源：http://m.share.bbcook.cn/Article/details/gzwdbplee.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.epnwcf.com/Article/details/gazlsluwm.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.yfazqb.com/Article/details/gdvarsaes.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fktsv.cn/Article/details/gqvdoxcul.sHtML

[R45] 批量删除
来源：http://read.share.vehdjk.com/Article/details/gwhwpbjhg.sHtML

find . -name "*.tmp" -delete
来源：http://wap.epnwcf.com/Article/details/gmjpoawid.sHtML

[R46] 递归替换文件内容
来源：http://blog.yfazqb.com/Article/details/ggxamehho.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.tarul.cn/Article/details/grgnshugu.sHtML

[R47] sed 单行替换
来源：http://read.share.tarul.cn/Article/details/gnassctck.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.bbcook.cn/Article/details/ghhgrvsdi.sHtML

[R48] awk 取指定列
来源：http://baike.bbcook.cn/Article/details/gypdjhnhw.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.epnwcf.com/Article/details/gkcqfjkrb.sHtML

[R49] awk 带条件
来源：http://baike.tarul.cn/Article/details/gjcouhawp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.vehdjk.com/Article/details/gzbxiixhw.sHtML

[R50] awk 求和
来源：http://3g.sjlbkw.cn/Article/details/gfqpigigp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.vehdjk.com/Article/details/gvvirlqya.sHtML

[R51] 排序去重取前几
来源：http://blog.tarul.cn/Article/details/gizegmrcn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.vehdjk.com/Article/details/googvnahz.sHtML

[R52] 统计行数
来源：http://read.share.bbcook.cn/Article/details/gbnstnard.sHtML

wc -l a.txt
来源：http://baike.bbcook.cn/Article/details/gnoltavxi.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.tarul.cn/Article/details/gwndooqhg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.bbcook.cn/Article/details/getabmmxk.sHtML

[R54] 比较两个文件
来源：http://baike.vehdjk.com/Article/details/gbsobtmfy.sHtML

diff a.txt b.txt
来源：http://blog.vehdjk.com/Article/details/gsvkqtlpg.sHtML

[R55] 压缩与解压
来源：http://blog.vehdjk.com/Article/details/ggqeiblwd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fktsv.cn/Article/details/gvbtvcclj.sHtML

[R56] 远程拷贝
来源：http://wap.vehdjk.com/Article/details/gocvnnemx.sHtML

scp file user@host:/path/
来源：http://mobile.epnwcf.com/Article/details/goxexmwwy.sHtML

[R57] 远程执行命令
来源：http://www.share.bbcook.cn/Article/details/gpcsxfyiy.sHtML

ssh user@host 'uptime'
来源：http://www.blog.tarul.cn/Article/details/gucgyjdye.sHtML

[R58] 下载文件
来源：http://baike.vehdjk.com/Article/details/gdnzpmezv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fktsv.cn/Article/details/gwmgrzuxd.sHtML

[R59] 发 POST JSON
来源：http://read.share.vehdjk.com/Article/details/gztiwvfot.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.sjlbkw.cn/Article/details/gmjrzetng.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.bbcook.cn/Article/details/genqrtbfw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.vehdjk.com/Article/details/gxsqflsxx.sHtML

[R61] 磁盘占用
来源：http://blog.fktsv.cn/Article/details/gxveeowvx.sHtML

df -h;  du -sh *
来源：http://www.share.bbcook.cn/Article/details/ggfxcyknt.sHtML

[R62] 找最占空间的文件
来源：http://blog.tarul.cn/Article/details/gcaltzrdz.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.vehdjk.com/Article/details/gtioafrpv.sHtML

[R63] 内存与进程
来源：http://www.m.share.sjlbkw.cn/Article/details/gjvuftnhm.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.epnwcf.com/Article/details/gwebsmvxf.sHtML

[R64] 结束进程
来源：http://www.blog.tarul.cn/Article/details/gjahhujra.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.yfazqb.com/Article/details/gvuzlezag.sHtML

[R65] 查看端口占用
来源：http://m.share.tarul.cn/Article/details/geerdlrle.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.yfazqb.com/Article/details/goeigecva.sHtML

[R66] 定时任务
来源：http://3g.tarul.cn/Article/details/gxpmvqttl.sHtML

crontab -e;  crontab -l
来源：http://www.blog.yfazqb.com/Article/details/guvkpzphr.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fktsv.cn/Article/details/geoicdzgg.sHtML

openssl rand -hex 16
来源：http://m.share.fktsv.cn/Article/details/gaxrokttj.sHtML

[R68] 计算文件校验值
来源：http://mobile.epnwcf.com/Article/details/gxtgmvgqy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.yfazqb.com/Article/details/gfvepsvza.sHtML

[R69] 生成随机密码
来源：http://wap.vehdjk.com/Article/details/gmmyhussj.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.vehdjk.com/Article/details/gofsmaudd.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.bbcook.cn/Article/details/gugkyzqng.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.sjlbkw.cn/Article/details/gyyuwnfvb.sHtML

[R71] 日期格式化
来源：http://www.blog.fktsv.cn/Article/details/guhsowdxb.sHtML


<!-- 参考信息 -->