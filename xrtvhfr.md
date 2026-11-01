代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.bbcook.cn/Article/details/gpqcuuger.sHtML

[Q22] 排序
来源：http://3g.yfazqb.com/Article/details/gctxiekwl.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.yfazqb.com/Article/details/gmytawaar.sHtML

[Q23] 分页
来源：http://mobile.yfazqb.com/Article/details/gwrpoiqaa.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.yfazqb.com/Article/details/ggzdyxvuq.sHtML

[Q24] 去重
来源：http://blog.epnwcf.com/Article/details/gitgepvdw.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fktsv.cn/Article/details/gwazowmav.sHtML

[Q25] 只取前 N 条
来源：http://blog.yfazqb.com/Article/details/gyypwqwep.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.epnwcf.com/Article/details/gruxtbqql.sHtML

[Q26] 计数
来源：http://blog.tarul.cn/Article/details/gmulheeqz.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fktsv.cn/Article/details/glkyxfldj.sHtML

[Q27] 条件计数
来源：http://www.m.share.sjlbkw.cn/Article/details/giaaxmsmz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.yfazqb.com/Article/details/glswianmx.sHtML

[Q28] 求和与平均
来源：http://blog.epnwcf.com/Article/details/ghkjtehny.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.vehdjk.com/Article/details/gogdmcrtr.sHtML

[Q29] 最大最小值
来源：http://wap.vehdjk.com/Article/details/ggistczqb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/grpziltda.sHtML

[Q30] 分组统计
来源：http://wap.fktsv.cn/Article/details/gjrsaqhew.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.epnwcf.com/Article/details/gzngxmgiy.sHtML

[Q31] 分组后过滤
来源：http://mobile.sjlbkw.cn/Article/details/gtupvbycw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.sjlbkw.cn/Article/details/gguakcont.sHtML

[Q32] 分组拼接字符串
来源：http://baike.tarul.cn/Article/details/gwvansvza.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.yfazqb.com/Article/details/gfqlufapg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.tarul.cn/Article/details/gaimyngwf.sHtML

[Q33] 多列分组
来源：http://blog.yfazqb.com/Article/details/gqubblwfj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fktsv.cn/Article/details/gewounmzc.sHtML

[Q34] 每组取第一条
来源：http://m.share.fktsv.cn/Article/details/gmwappstg.sHtML

SELECT * FROM (
来源：http://www.share.yfazqb.com/Article/details/gzjkktwyr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.epnwcf.com/Article/details/gaqgbfdwi.sHtML

) t WHERE rn = 1;
来源：http://wap.yfazqb.com/Article/details/gpcatnypj.sHtML

[Q35] 内连接
来源：http://www.m.share.sjlbkw.cn/Article/details/gbvicrbnt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.yfazqb.com/Article/details/gdgggceru.sHtML

[Q36] 左连接
来源：http://3g.epnwcf.com/Article/details/gpwjgpbpi.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.epnwcf.com/Article/details/gatajulfp.sHtML

[Q37] 右连接
来源：http://blog.bbcook.cn/Article/details/ghjjigaaj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.tarul.cn/Article/details/goxptmddh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.yfazqb.com/Article/details/giivtgcnu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.yfazqb.com/Article/details/gliqdmpxc.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.vehdjk.com/Article/details/garhzjrzk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.tarul.cn/Article/details/gjytvsgdq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fktsv.cn/Article/details/gmvlsbpnb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.epnwcf.com/Article/details/giflxlgub.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.sjlbkw.cn/Article/details/glpytjajk.sHtML

[Q41] 多表连接
来源：http://mobile.tarul.cn/Article/details/gbsqplefg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.epnwcf.com/Article/details/ggkfzyjif.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fktsv.cn/Article/details/gmlwxikoz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.yfazqb.com/Article/details/gkdqvjnuy.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.tarul.cn/Article/details/gwwefylab.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.vehdjk.com/Article/details/gipteejwz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.yfazqb.com/Article/details/gxwyevhho.sHtML

[Q43] 标量子查询
来源：http://www.blog.fktsv.cn/Article/details/gdrhphncv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fktsv.cn/Article/details/gysngpjmu.sHtML

[Q44] IN 子查询
来源：http://3g.fktsv.cn/Article/details/gbbblihsz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.bbcook.cn/Article/details/gvtbcydyk.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.bbcook.cn/Article/details/gtzkrwgeo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.vehdjk.com/Article/details/gvpuhpesm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.yfazqb.com/Article/details/gumneidbs.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.tarul.cn/Article/details/ggpdfheuj.sHtML

[Q47] 与平均值比较
来源：http://wap.bbcook.cn/Article/details/gajuboudu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.tarul.cn/Article/details/gezhvydie.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.epnwcf.com/Article/details/glchkizyf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.sjlbkw.cn/Article/details/gkhqnxzzw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.bbcook.cn/Article/details/ghfwqfwkd.sHtML

[Q49] 更新单行
来源：http://blog.vehdjk.com/Article/details/gcnioxspy.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.bbcook.cn/Article/details/gwsxeuwys.sHtML

[Q50] 批量更新
来源：http://baike.vehdjk.com/Article/details/gxcaweibz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.epnwcf.com/Article/details/gvyvnylng.sHtML

[Q51] 用子查询更新
来源：http://m.share.yfazqb.com/Article/details/glmskkxqo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.yfazqb.com/Article/details/gmgntizko.sHtML

[Q52] 删除指定行
来源：http://m.share.bbcook.cn/Article/details/gpdwfcywc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.epnwcf.com/Article/details/gibaxkkhz.sHtML

[Q53] 按条件删除
来源：http://3g.fktsv.cn/Article/details/gbdxabrti.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.yfazqb.com/Article/details/gzovwpvwg.sHtML

[Q54] 清空表
来源：http://www.share.fktsv.cn/Article/details/gqwoxlpbm.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.epnwcf.com/Article/details/gwydjufxo.sHtML

[Q55] 排名（并列占位）
来源：http://wap.sjlbkw.cn/Article/details/gxkabaqwv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.sjlbkw.cn/Article/details/gureelzqm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.yfazqb.com/Article/details/gscrxlvzb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fktsv.cn/Article/details/gvbxxyesy.sHtML

[Q57] 行号
来源：http://www.blog.bbcook.cn/Article/details/gwmahhsye.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.vehdjk.com/Article/details/genyaoqjw.sHtML

[Q58] 累计求和
来源：http://read.share.fktsv.cn/Article/details/ghnpgpafk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fktsv.cn/Article/details/gobbwrpis.sHtML

[Q59] 分组内累计
来源：http://blog.vehdjk.com/Article/details/gpvznhupz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.yfazqb.com/Article/details/gomqawgwn.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fktsv.cn/Article/details/gvjsxamch.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.epnwcf.com/Article/details/gmmgqvhyu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fktsv.cn/Article/details/gznbatvxe.sHtML

[Q61] 移动平均
来源：http://www.m.share.yfazqb.com/Article/details/gtdqllxyb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.yfazqb.com/Article/details/gietmemqo.sHtML

[Q62] 分组占比
来源：http://mobile.yfazqb.com/Article/details/grnbbymwf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.yfazqb.com/Article/details/gqkhvcjly.sHtML

[Q63] 开启事务
来源：http://baike.bbcook.cn/Article/details/gyeqvsbum.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.sjlbkw.cn/Article/details/gpowqhago.sHtML

[Q64] 提交事务
来源：http://www.blog.fktsv.cn/Article/details/gslmniybk.sHtML

COMMIT;
来源：http://m.share.sjlbkw.cn/Article/details/gvfykfmpj.sHtML

[Q65] 回滚事务
来源：http://blog.tarul.cn/Article/details/galcozuvt.sHtML

ROLLBACK;
来源：http://m.share.bbcook.cn/Article/details/gmbgeniwt.sHtML

[Q66] 行锁查询
来源：http://mobile.tarul.cn/Article/details/graoxvxev.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.epnwcf.com/Article/details/ghvhdihkz.sHtML

[Q67] 设置隔离级别
来源：http://baike.sjlbkw.cn/Article/details/gucfidsvy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fktsv.cn/Article/details/gktflwcws.sHtML

[Q68] 保存点
来源：http://read.share.sjlbkw.cn/Article/details/gsirhczul.sHtML

SAVEPOINT sp1;
来源：http://m.share.bbcook.cn/Article/details/gbzeuzrjh.sHtML

ROLLBACK TO sp1;
来源：http://mobile.sjlbkw.cn/Article/details/gzinkhzbh.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.sjlbkw.cn/Article/details/gfcrbhmsj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fktsv.cn/Article/details/gyummtdsd.sHtML

[Q70] 更新统计信息
来源：http://3g.yfazqb.com/Article/details/goqevnkqk.sHtML

ANALYZE TABLE users;
来源：http://mobile.vehdjk.com/Article/details/gwvjzztyt.sHtML

[Q71] 查看建表语句
来源：http://m.share.epnwcf.com/Article/details/gigqswqef.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.bbcook.cn/Article/details/gshqasukk.sHtML

[Q72] 查看索引
来源：http://m.share.fktsv.cn/Article/details/glroumxdt.sHtML

SHOW INDEX FROM users;
来源：http://baike.vehdjk.com/Article/details/gabesbexk.sHtML

[Q73] 查看表状态
来源：http://blog.vehdjk.com/Article/details/gnzgfckaz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.yfazqb.com/Article/details/gfezkntyn.sHtML

[Q74] 强制使用索引
来源：http://baike.tarul.cn/Article/details/guozbjjie.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.yfazqb.com/Article/details/gidwkqbry.sHtML

[Q75] 日期格式化
来源：http://m.share.vehdjk.com/Article/details/gmlrvroid.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.bbcook.cn/Article/details/gplkyjnfy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fktsv.cn/Article/details/gyzsdqfet.sHtML

[Q76] 按天统计
来源：http://3g.fktsv.cn/Article/details/gfydyuquu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.vehdjk.com/Article/details/gzppwyegs.sHtML

[Q77] 时间加减
来源：http://mobile.yfazqb.com/Article/details/giekurbdf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fktsv.cn/Article/details/gnufoyile.sHtML

[Q78] 当前时间
来源：http://mobile.yfazqb.com/Article/details/gjlatlljt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.tarul.cn/Article/details/gcegvqmdb.sHtML

[Q79] 字符串拼接
来源：http://3g.epnwcf.com/Article/details/gyromcrsy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fktsv.cn/Article/details/gsxvlwrhb.sHtML

[Q80] 字符串截取
来源：http://m.share.epnwcf.com/Article/details/gpcintsia.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/grwzocmtu.sHtML

[Q81] 字符串替换
来源：http://wap.sjlbkw.cn/Article/details/grvrdffps.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gvocgnncc.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.sjlbkw.cn/Article/details/gikxorhyd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.vehdjk.com/Article/details/grsxucvbp.sHtML

[Q83] 大小写转换
来源：http://baike.epnwcf.com/Article/details/gxhfkzxax.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gaxuoaead.sHtML

[Q84] 去除首尾空格
来源：http://mobile.epnwcf.com/Article/details/gwczsjiww.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.vehdjk.com/Article/details/gohsogwuf.sHtML

[Q85] 数值取整
来源：http://www.m.share.bbcook.cn/Article/details/gxygsfpvu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.tarul.cn/Article/details/gjygvyogs.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.vehdjk.com/Article/details/gskrkmxzm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fktsv.cn/Article/details/gvvbvcxtv.sHtML

[Q87] JSON 字段做条件
来源：http://baike.sjlbkw.cn/Article/details/grzwnlgec.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.yfazqb.com/Article/details/gpleidfgc.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.tarul.cn/Article/details/grkilrjyo.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.tarul.cn/Article/details/gnhlpmzut.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.vehdjk.com/Article/details/gczbrsoqi.sHtML

[Q89] 判断表是否存在
来源：http://blog.sjlbkw.cn/Article/details/gikxlfkqj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.epnwcf.com/Article/details/glvdvxeqc.sHtML

[Q90] 生成序号列
来源：http://wap.bbcook.cn/Article/details/gajihwzfs.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.vehdjk.com/Article/details/gwykwwnoc.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gtyievsgu.sHtML

R. Bash 专题
来源：http://m.share.fktsv.cn/Article/details/gldjbxlyz.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gqulkqqrk.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.sjlbkw.cn/Article/details/grhfidnru.sHtML

#!/usr/bin/env bash
来源：http://www.blog.yfazqb.com/Article/details/gerreysss.sHtML

set -euo pipefail
来源：http://www.share.tarul.cn/Article/details/ggccnmytw.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.yfazqb.com/Article/details/glfxtfpns.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.tarul.cn/Article/details/ghmawdekr.sHtML

[R03] 只读变量
来源：http://m.share.epnwcf.com/Article/details/gruyiwjyo.sHtML

readonly PI=3.14
来源：http://www.blog.fktsv.cn/Article/details/ggbkggpsf.sHtML

[R04] 位置参数
来源：http://www.blog.bbcook.cn/Article/details/gjdeeisbf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.vehdjk.com/Article/details/guwddeqnh.sHtML

[R05] 参数默认值
来源：http://read.share.bbcook.cn/Article/details/gpygklgba.sHtML

name="${1:-default}"
来源：http://baike.sjlbkw.cn/Article/details/gztxzonhw.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.sjlbkw.cn/Article/details/geaybagea.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.bbcook.cn/Article/details/gmarnhhvw.sHtML

[R07] if 判断文件
来源：http://m.share.vehdjk.com/Article/details/gdonrvwar.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.vehdjk.com/Article/details/golsyvbvm.sHtML

[R08] 数值比较
来源：http://baike.fktsv.cn/Article/details/goabpyuss.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.epnwcf.com/Article/details/gltqakvdc.sHtML

[R09] 字符串比较
来源：http://www.m.share.yfazqb.com/Article/details/ggfhwqbdi.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.tarul.cn/Article/details/gjcnnogjq.sHtML

[R10] 正则匹配
来源：http://baike.tarul.cn/Article/details/gntsqacfq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.tarul.cn/Article/details/ghxpjvnki.sHtML

[R11] case 多分支
来源：http://baike.tarul.cn/Article/details/gjoxdqunw.sHtML

case "$1" in
来源：http://m.share.yfazqb.com/Article/details/gjudzltnq.sHtML

start) echo "启动" ;;
来源：http://blog.vehdjk.com/Article/details/gtntkjxzj.sHtML

stop)  echo "停止" ;;
来源：http://3g.yfazqb.com/Article/details/gdxzxwyeb.sHtML

*)     echo "未知命令" ;;
来源：http://3g.epnwcf.com/Article/details/gvcofuhca.sHtML

esac
来源：http://mobile.vehdjk.com/Article/details/goinkvkyy.sHtML

[R12] for 遍历文件
来源：http://mobile.vehdjk.com/Article/details/gpzmxihiq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.bbcook.cn/Article/details/glhwnrpcc.sHtML

[R13] for 计数循环
来源：http://mobile.tarul.cn/Article/details/gocuvffwp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.sjlbkw.cn/Article/details/gcsyuxglv.sHtML

[R14] C 风格 for
来源：http://blog.tarul.cn/Article/details/gzzjwvnqu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.yfazqb.com/Article/details/gkoubljtq.sHtML

[R15] while 逐行读文件
来源：http://blog.fktsv.cn/Article/details/gawfauavb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.tarul.cn/Article/details/gmocwckhb.sHtML

[R16] until 等待条件
来源：http://baike.epnwcf.com/Article/details/gbvhimtqz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.vehdjk.com/Article/details/ggzweqavq.sHtML

[R17] 数组定义与取值
来源：http://mobile.yfazqb.com/Article/details/grejdiwbs.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fktsv.cn/Article/details/gluywpfmu.sHtML

[R18] 遍历数组
来源：http://baike.fktsv.cn/Article/details/ghvvvixxs.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.sjlbkw.cn/Article/details/gvwwlsqeb.sHtML

[R19] 数组长度
来源：http://read.share.fktsv.cn/Article/details/gczzpauqg.sHtML

echo "${#arr[@]}"
来源：http://m.share.epnwcf.com/Article/details/glweiysxb.sHtML

[R20] 关联数组（字典）
来源：http://www.share.tarul.cn/Article/details/ghbikcqvw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.vehdjk.com/Article/details/gsshktuep.sHtML

[R21] 字符串长度
来源：http://m.share.fktsv.cn/Article/details/gbomkuefd.sHtML

echo "${#s}"
来源：http://www.blog.tarul.cn/Article/details/gukqpbzht.sHtML

[R22] 截取子串
来源：http://read.share.fktsv.cn/Article/details/gtygnampv.sHtML

echo "${s:0:5}"
来源：http://3g.sjlbkw.cn/Article/details/gxmokbxyz.sHtML

[R23] 字符串替换
来源：http://mobile.bbcook.cn/Article/details/gmhodszis.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fktsv.cn/Article/details/goyvpmfci.sHtML

[R24] 大小写转换
来源：http://blog.fktsv.cn/Article/details/guaiyihak.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.bbcook.cn/Article/details/gawjpzzwl.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.vehdjk.com/Article/details/gvjgdivgx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.bbcook.cn/Article/details/gdaxavthx.sHtML

[R26] 命令替换
来源：http://blog.sjlbkw.cn/Article/details/gaqxtmqfn.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.tarul.cn/Article/details/gubqmekas.sHtML

[R27] 算术展开
来源：http://baike.sjlbkw.cn/Article/details/gcfinlpro.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.vehdjk.com/Article/details/gufcybpia.sHtML

[R28] 浮点运算
来源：http://wap.yfazqb.com/Article/details/gdytewytz.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.vehdjk.com/Article/details/glammfflc.sHtML

[R29] 定义函数
来源：http://baike.bbcook.cn/Article/details/gysumofkt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.vehdjk.com/Article/details/guqsskpda.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.vehdjk.com/Article/details/gyunsbkuo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.bbcook.cn/Article/details/gwnoojwoo.sHtML

[R31] 局部变量
来源：http://mobile.vehdjk.com/Article/details/gujtpaidn.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.vehdjk.com/Article/details/gvvqvcaak.sHtML

[R32] 参数个数校验
来源：http://read.share.vehdjk.com/Article/details/gimoflrjm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.bbcook.cn/Article/details/gqutaywiu.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.yfazqb.com/Article/details/gxkvitytw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.vehdjk.com/Article/details/gscxhsekj.sHtML

[R34] 退出时清理
来源：http://read.share.vehdjk.com/Article/details/gdhkdpqlm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.bbcook.cn/Article/details/gohuosvdj.sHtML

[R35] 后台执行并等待
来源：http://m.share.epnwcf.com/Article/details/gonkwddjk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.sjlbkw.cn/Article/details/gjlzhjsxd.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fktsv.cn/Article/details/gpsloezcb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.sjlbkw.cn/Article/details/gspjdxqnu.sHtML

[R37] 把输出赋给变量
来源：http://3g.yfazqb.com/Article/details/gfrkckvir.sHtML

files=$(ls -1)
来源：http://read.share.tarul.cn/Article/details/gvljchorw.sHtML

[R38] 管道串联
来源：http://wap.sjlbkw.cn/Article/details/gzjehpxbd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.sjlbkw.cn/Article/details/gimchxady.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.bbcook.cn/Article/details/gnqwjcrao.sHtML

cmd > out.log 2>&1
来源：http://www.share.bbcook.cn/Article/details/gtxgdgxfr.sHtML

[R40] 追加写日志
来源：http://www.blog.bbcook.cn/Article/details/gwkdtgoof.sHtML

echo "log" >> out.log
来源：http://wap.bbcook.cn/Article/details/glumlngwt.sHtML

[R41] 丢弃输出
来源：http://www.m.share.tarul.cn/Article/details/gypxbkjyj.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.vehdjk.com/Article/details/gkverdpqh.sHtML

[R42] 输入重定向
来源：http://mobile.vehdjk.com/Article/details/gqyfibzvi.sHtML

wc -l < a.txt
来源：http://baike.vehdjk.com/Article/details/gxaaoxemt.sHtML

[R43] 按名字查找文件
来源：http://3g.vehdjk.com/Article/details/gsknagmwo.sHtML

find . -name "*.log" -type f
来源：http://blog.tarul.cn/Article/details/gxtpbozot.sHtML

[R44] 按修改时间查找
来源：http://read.share.epnwcf.com/Article/details/gfboalcwz.sHtML

find . -mtime -7 -type f
来源：http://www.blog.bbcook.cn/Article/details/gyvrqzmyu.sHtML

[R45] 批量删除
来源：http://read.share.tarul.cn/Article/details/gdqijvfyf.sHtML

find . -name "*.tmp" -delete
来源：http://3g.vehdjk.com/Article/details/gbkngkgyh.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fktsv.cn/Article/details/gsqighwmq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fktsv.cn/Article/details/gomaxhifq.sHtML

[R47] sed 单行替换
来源：http://baike.sjlbkw.cn/Article/details/gsiikrbnb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.yfazqb.com/Article/details/gdjlfsxgs.sHtML

[R48] awk 取指定列
来源：http://blog.tarul.cn/Article/details/gqkczwqbe.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.vehdjk.com/Article/details/gmtzmjbvy.sHtML

[R49] awk 带条件
来源：http://www.blog.epnwcf.com/Article/details/gezdosozz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.yfazqb.com/Article/details/gvipzdmma.sHtML

[R50] awk 求和
来源：http://baike.fktsv.cn/Article/details/gqtzunoko.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.tarul.cn/Article/details/gckxavght.sHtML

[R51] 排序去重取前几
来源：http://www.share.fktsv.cn/Article/details/gvecdezwd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.tarul.cn/Article/details/gfpiufdeb.sHtML

[R52] 统计行数
来源：http://www.share.sjlbkw.cn/Article/details/gedqzmxnk.sHtML

wc -l a.txt
来源：http://m.share.bbcook.cn/Article/details/gbzorjhwh.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.yfazqb.com/Article/details/gyuamnoyx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.epnwcf.com/Article/details/gfvhgfwia.sHtML

[R54] 比较两个文件
来源：http://3g.bbcook.cn/Article/details/gogetfwbo.sHtML

diff a.txt b.txt
来源：http://m.share.bbcook.cn/Article/details/gijbujogz.sHtML

[R55] 压缩与解压
来源：http://wap.yfazqb.com/Article/details/gtehydnph.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.sjlbkw.cn/Article/details/gshbtlxco.sHtML

[R56] 远程拷贝
来源：http://read.share.bbcook.cn/Article/details/gwcdggugo.sHtML

scp file user@host:/path/
来源：http://www.m.share.yfazqb.com/Article/details/ggksrprel.sHtML

[R57] 远程执行命令
来源：http://www.share.vehdjk.com/Article/details/grlsbdlst.sHtML

ssh user@host 'uptime'
来源：http://m.share.vehdjk.com/Article/details/gzavhoyuq.sHtML

[R58] 下载文件
来源：http://3g.fktsv.cn/Article/details/gsmefeuoo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.bbcook.cn/Article/details/gexwzvngp.sHtML

[R59] 发 POST JSON
来源：http://blog.bbcook.cn/Article/details/ghshwwbuh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.tarul.cn/Article/details/gkiggiysj.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.vehdjk.com/Article/details/gmysasryi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.epnwcf.com/Article/details/gjefuwsrs.sHtML

[R61] 磁盘占用
来源：http://3g.vehdjk.com/Article/details/gyndzjrdk.sHtML

df -h;  du -sh *
来源：http://www.share.epnwcf.com/Article/details/gknkaewqh.sHtML

[R62] 找最占空间的文件
来源：http://baike.bbcook.cn/Article/details/gsinrvzni.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.sjlbkw.cn/Article/details/gcztotexo.sHtML

[R63] 内存与进程
来源：http://baike.yfazqb.com/Article/details/ggxrlegrr.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.yfazqb.com/Article/details/ggpdmyjmo.sHtML

[R64] 结束进程
来源：http://3g.fktsv.cn/Article/details/grtbkmxkh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fktsv.cn/Article/details/gonnzhiat.sHtML

[R65] 查看端口占用
来源：http://www.blog.tarul.cn/Article/details/gyfnboxkw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.bbcook.cn/Article/details/gvedrmpnv.sHtML

[R66] 定时任务
来源：http://3g.tarul.cn/Article/details/gyegezeru.sHtML

crontab -e;  crontab -l
来源：http://www.share.sjlbkw.cn/Article/details/gbcqntfjs.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.vehdjk.com/Article/details/grxmmgnmi.sHtML

openssl rand -hex 16
来源：http://baike.sjlbkw.cn/Article/details/ghguyivcz.sHtML

[R68] 计算文件校验值
来源：http://mobile.fktsv.cn/Article/details/gfzeacdri.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.tarul.cn/Article/details/gusswrkch.sHtML

[R69] 生成随机密码
来源：http://read.share.tarul.cn/Article/details/gjikdcmvy.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.bbcook.cn/Article/details/gofltjouc.sHtML

[R70] 时间戳与互转
来源：http://read.share.epnwcf.com/Article/details/gpctsrsdv.sHtML

date +%s;  date -d @1700000000
来源：http://baike.epnwcf.com/Article/details/gouxyweyu.sHtML

[R71] 日期格式化
来源：http://3g.vehdjk.com/Article/details/gqzqbocmw.sHtML


<!-- 参考信息 -->