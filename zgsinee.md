代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.sjlbkw.cn/Article/details/gnzruqval.sHtML

[Q22] 排序
来源：http://wap.yfazqb.com/Article/details/gcvaudhsd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.tarul.cn/Article/details/gimowteno.sHtML

[Q23] 分页
来源：http://3g.fktsv.cn/Article/details/gxnjhgzym.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.sjlbkw.cn/Article/details/gemsnjdqy.sHtML

[Q24] 去重
来源：http://www.m.share.tarul.cn/Article/details/gqunyhagu.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fktsv.cn/Article/details/gutsldqaj.sHtML

[Q25] 只取前 N 条
来源：http://mobile.sjlbkw.cn/Article/details/gihnlerha.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.tarul.cn/Article/details/gvqzzvpid.sHtML

[Q26] 计数
来源：http://blog.bbcook.cn/Article/details/gpbfcgkuj.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fktsv.cn/Article/details/gumugnqcu.sHtML

[Q27] 条件计数
来源：http://read.share.tarul.cn/Article/details/ghwdkvnau.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gbcxncrhk.sHtML

[Q28] 求和与平均
来源：http://mobile.tarul.cn/Article/details/ggptxrzyl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.bbcook.cn/Article/details/grklwnyds.sHtML

[Q29] 最大最小值
来源：http://read.share.epnwcf.com/Article/details/gcwrcmpdt.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.yfazqb.com/Article/details/gmufbbqnf.sHtML

[Q30] 分组统计
来源：http://wap.bbcook.cn/Article/details/gucqjkmaj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fktsv.cn/Article/details/gxscctewd.sHtML

[Q31] 分组后过滤
来源：http://wap.bbcook.cn/Article/details/gspwtbtkt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.epnwcf.com/Article/details/gzrtlldlh.sHtML

[Q32] 分组拼接字符串
来源：http://wap.sjlbkw.cn/Article/details/gpehqzjje.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.bbcook.cn/Article/details/gsrzhzhwx.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.epnwcf.com/Article/details/gnijehrey.sHtML

[Q33] 多列分组
来源：http://blog.yfazqb.com/Article/details/giilyyjin.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.tarul.cn/Article/details/gsscycnle.sHtML

[Q34] 每组取第一条
来源：http://baike.sjlbkw.cn/Article/details/grurlexzv.sHtML

SELECT * FROM (
来源：http://3g.yfazqb.com/Article/details/guegqrujj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fktsv.cn/Article/details/gggzgsvmw.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.vehdjk.com/Article/details/ggumppcul.sHtML

[Q35] 内连接
来源：http://read.share.sjlbkw.cn/Article/details/gcnyspvae.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fktsv.cn/Article/details/ggcgguaug.sHtML

[Q36] 左连接
来源：http://mobile.tarul.cn/Article/details/grxwneozp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.vehdjk.com/Article/details/gkebvbmxp.sHtML

[Q37] 右连接
来源：http://blog.vehdjk.com/Article/details/gunygvajb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.sjlbkw.cn/Article/details/gidppgjxr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.bbcook.cn/Article/details/gpkyzmyoj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.bbcook.cn/Article/details/gafxrqiej.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.sjlbkw.cn/Article/details/ghcvtlnxs.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.vehdjk.com/Article/details/gcxqdknmc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.bbcook.cn/Article/details/gohlllvma.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.bbcook.cn/Article/details/gualrtlfg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.epnwcf.com/Article/details/gjmybifbm.sHtML

[Q41] 多表连接
来源：http://www.share.fktsv.cn/Article/details/gsbsedudx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.epnwcf.com/Article/details/grgxforor.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.bbcook.cn/Article/details/gvoyhcxlr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.tarul.cn/Article/details/gfaqirtmm.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.sjlbkw.cn/Article/details/gbavfwymc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.epnwcf.com/Article/details/givhgjcvo.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.yfazqb.com/Article/details/gfzmlokaz.sHtML

[Q43] 标量子查询
来源：http://blog.vehdjk.com/Article/details/gzrgwqvor.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.yfazqb.com/Article/details/ganbxpwij.sHtML

[Q44] IN 子查询
来源：http://3g.sjlbkw.cn/Article/details/gwfkjfujl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.yfazqb.com/Article/details/gdicwekjs.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.epnwcf.com/Article/details/gvqiygzvo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.yfazqb.com/Article/details/gfiaidzuu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.epnwcf.com/Article/details/gmqiqaqnn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.tarul.cn/Article/details/gbhtppyvq.sHtML

[Q47] 与平均值比较
来源：http://m.share.sjlbkw.cn/Article/details/gljwiitjc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.epnwcf.com/Article/details/gqcuehvpv.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.vehdjk.com/Article/details/guarnhohg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.vehdjk.com/Article/details/gftsrtlwm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.sjlbkw.cn/Article/details/gkvayzkct.sHtML

[Q49] 更新单行
来源：http://baike.sjlbkw.cn/Article/details/gmiccpjgu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fktsv.cn/Article/details/gojdgffkx.sHtML

[Q50] 批量更新
来源：http://mobile.tarul.cn/Article/details/gbaieonzi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.sjlbkw.cn/Article/details/gynkimutx.sHtML

[Q51] 用子查询更新
来源：http://m.share.sjlbkw.cn/Article/details/gsibdjmfx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gimujzktk.sHtML

[Q52] 删除指定行
来源：http://baike.fktsv.cn/Article/details/gtjmgeunx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fktsv.cn/Article/details/gpcwlgimy.sHtML

[Q53] 按条件删除
来源：http://blog.bbcook.cn/Article/details/gmvcritca.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.epnwcf.com/Article/details/gufkzwrdb.sHtML

[Q54] 清空表
来源：http://3g.epnwcf.com/Article/details/goyxxwqfo.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.tarul.cn/Article/details/gebzzexos.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.bbcook.cn/Article/details/gaibxzffo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fktsv.cn/Article/details/gxbwhffdr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.vehdjk.com/Article/details/gbbgfghgr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.tarul.cn/Article/details/gaogkdduw.sHtML

[Q57] 行号
来源：http://m.share.fktsv.cn/Article/details/gcnxikspa.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.vehdjk.com/Article/details/gyuuhlucv.sHtML

[Q58] 累计求和
来源：http://baike.fktsv.cn/Article/details/gudtlmilz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.bbcook.cn/Article/details/gqygjuqlb.sHtML

[Q59] 分组内累计
来源：http://wap.yfazqb.com/Article/details/gbbtxfnet.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.tarul.cn/Article/details/gyjddupme.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.bbcook.cn/Article/details/gmrzfcipc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.sjlbkw.cn/Article/details/gkxtyljsv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/gmkaeptcr.sHtML

[Q61] 移动平均
来源：http://www.blog.tarul.cn/Article/details/gdgtfhmwm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.yfazqb.com/Article/details/gnvvrneif.sHtML

[Q62] 分组占比
来源：http://www.m.share.bbcook.cn/Article/details/guyfjkbdd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.epnwcf.com/Article/details/gjpmvvqaz.sHtML

[Q63] 开启事务
来源：http://blog.yfazqb.com/Article/details/gxvqanpxl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.vehdjk.com/Article/details/gsbqyffym.sHtML

[Q64] 提交事务
来源：http://mobile.epnwcf.com/Article/details/gsfgvourx.sHtML

COMMIT;
来源：http://3g.vehdjk.com/Article/details/gomtpkrqj.sHtML

[Q65] 回滚事务
来源：http://blog.tarul.cn/Article/details/gkcdkvmrc.sHtML

ROLLBACK;
来源：http://3g.fktsv.cn/Article/details/gbxgnmqni.sHtML

[Q66] 行锁查询
来源：http://baike.vehdjk.com/Article/details/gniptyjdo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.vehdjk.com/Article/details/giefzpmjd.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.sjlbkw.cn/Article/details/glrabzrco.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.bbcook.cn/Article/details/gihzmzpxn.sHtML

[Q68] 保存点
来源：http://www.share.sjlbkw.cn/Article/details/gieofqfkh.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fktsv.cn/Article/details/grodojkgb.sHtML

ROLLBACK TO sp1;
来源：http://m.share.bbcook.cn/Article/details/gqddprmop.sHtML

[Q69] 查看执行计划
来源：http://3g.fktsv.cn/Article/details/gorqemgoe.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.bbcook.cn/Article/details/gfxzjimyo.sHtML

[Q70] 更新统计信息
来源：http://mobile.fktsv.cn/Article/details/gxurfweig.sHtML

ANALYZE TABLE users;
来源：http://mobile.tarul.cn/Article/details/gpcjyodrw.sHtML

[Q71] 查看建表语句
来源：http://m.share.yfazqb.com/Article/details/guvpoqzji.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.bbcook.cn/Article/details/gorikzukf.sHtML

[Q72] 查看索引
来源：http://mobile.yfazqb.com/Article/details/ggraqklxf.sHtML

SHOW INDEX FROM users;
来源：http://www.share.epnwcf.com/Article/details/giwfrhbvp.sHtML

[Q73] 查看表状态
来源：http://www.blog.vehdjk.com/Article/details/glbpbwobj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.epnwcf.com/Article/details/gkpnywyxv.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fktsv.cn/Article/details/gwneqdkmj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.bbcook.cn/Article/details/gfknolomh.sHtML

[Q75] 日期格式化
来源：http://www.share.bbcook.cn/Article/details/gdyfaxjsn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/gcnwdldis.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.tarul.cn/Article/details/gamupsgua.sHtML

[Q76] 按天统计
来源：http://read.share.bbcook.cn/Article/details/gwxfpmfdr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.vehdjk.com/Article/details/ggpilqumo.sHtML

[Q77] 时间加减
来源：http://3g.epnwcf.com/Article/details/gldomxmkv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.tarul.cn/Article/details/gpitsuffh.sHtML

[Q78] 当前时间
来源：http://www.share.sjlbkw.cn/Article/details/gageucqox.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.tarul.cn/Article/details/gocwjnmfd.sHtML

[Q79] 字符串拼接
来源：http://baike.bbcook.cn/Article/details/giuvqyich.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.sjlbkw.cn/Article/details/gadwudeof.sHtML

[Q80] 字符串截取
来源：http://mobile.sjlbkw.cn/Article/details/ghdwveytc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.tarul.cn/Article/details/gyvzvfskw.sHtML

[Q81] 字符串替换
来源：http://blog.vehdjk.com/Article/details/gmuhzonlr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gbtynymsw.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.sjlbkw.cn/Article/details/ghxpdhjhz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gedxmalkv.sHtML

[Q83] 大小写转换
来源：http://baike.sjlbkw.cn/Article/details/gwszvpjjs.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.vehdjk.com/Article/details/gbphbyzfp.sHtML

[Q84] 去除首尾空格
来源：http://wap.fktsv.cn/Article/details/gkvnkpkdh.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gxddlcday.sHtML

[Q85] 数值取整
来源：http://3g.sjlbkw.cn/Article/details/gyvwmgeyh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.epnwcf.com/Article/details/gxwkwyxlr.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.vehdjk.com/Article/details/gcoaoobcp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.yfazqb.com/Article/details/gmjsaginc.sHtML

[Q87] JSON 字段做条件
来源：http://blog.tarul.cn/Article/details/gcayeoznb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.vehdjk.com/Article/details/gvozrrqdw.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fktsv.cn/Article/details/gxatqqhde.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.vehdjk.com/Article/details/gzdsbufbg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fktsv.cn/Article/details/gaaeuaqny.sHtML

[Q89] 判断表是否存在
来源：http://mobile.tarul.cn/Article/details/gvopvzpcy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.yfazqb.com/Article/details/gvjejqwxk.sHtML

[Q90] 生成序号列
来源：http://wap.sjlbkw.cn/Article/details/gwpchzswh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.epnwcf.com/Article/details/gjuyxruse.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gohgronmh.sHtML

R. Bash 专题
来源：http://blog.tarul.cn/Article/details/glcivoosg.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gqqnqpnxi.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.sjlbkw.cn/Article/details/gpstierjq.sHtML

#!/usr/bin/env bash
来源：http://3g.vehdjk.com/Article/details/gfgvegjlb.sHtML

set -euo pipefail
来源：http://read.share.bbcook.cn/Article/details/glygscfkr.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fktsv.cn/Article/details/glviqjtas.sHtML

name="Tom"; echo "$name"
来源：http://wap.sjlbkw.cn/Article/details/gedqymxkv.sHtML

[R03] 只读变量
来源：http://blog.fktsv.cn/Article/details/gfmzwntpw.sHtML

readonly PI=3.14
来源：http://www.share.epnwcf.com/Article/details/geifyjglh.sHtML

[R04] 位置参数
来源：http://mobile.fktsv.cn/Article/details/gowvaoqaw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.vehdjk.com/Article/details/gaqrrmclx.sHtML

[R05] 参数默认值
来源：http://baike.sjlbkw.cn/Article/details/gyouobdlm.sHtML

name="${1:-default}"
来源：http://3g.tarul.cn/Article/details/gvkumsbpu.sHtML

[R06] 判断命令是否存在
来源：http://3g.vehdjk.com/Article/details/gmtuezhag.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fktsv.cn/Article/details/glhkliaxu.sHtML

[R07] if 判断文件
来源：http://3g.yfazqb.com/Article/details/gxnbgvplq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.tarul.cn/Article/details/gcjkyiudq.sHtML

[R08] 数值比较
来源：http://www.m.share.epnwcf.com/Article/details/geyvynsox.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.epnwcf.com/Article/details/grctlbsdd.sHtML

[R09] 字符串比较
来源：http://www.share.bbcook.cn/Article/details/gpwqwtwfv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.bbcook.cn/Article/details/gkgxqusyi.sHtML

[R10] 正则匹配
来源：http://wap.vehdjk.com/Article/details/gckhumycs.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fktsv.cn/Article/details/gzdcfntwk.sHtML

[R11] case 多分支
来源：http://www.blog.sjlbkw.cn/Article/details/gqvdgldda.sHtML

case "$1" in
来源：http://www.blog.fktsv.cn/Article/details/gccobaqjo.sHtML

start) echo "启动" ;;
来源：http://www.blog.tarul.cn/Article/details/gmigmdxre.sHtML

stop)  echo "停止" ;;
来源：http://mobile.yfazqb.com/Article/details/gbfrixnhr.sHtML

*)     echo "未知命令" ;;
来源：http://blog.vehdjk.com/Article/details/gwsklizoi.sHtML

esac
来源：http://www.share.fktsv.cn/Article/details/gbhqijyci.sHtML

[R12] for 遍历文件
来源：http://m.share.epnwcf.com/Article/details/gkfmtljfv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fktsv.cn/Article/details/gounxysvs.sHtML

[R13] for 计数循环
来源：http://read.share.vehdjk.com/Article/details/gkrwkznnx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.sjlbkw.cn/Article/details/gxzzuzzcq.sHtML

[R14] C 风格 for
来源：http://blog.bbcook.cn/Article/details/gsyponbej.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.bbcook.cn/Article/details/gzlksbgle.sHtML

[R15] while 逐行读文件
来源：http://www.share.vehdjk.com/Article/details/gcygvzofk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.bbcook.cn/Article/details/gofnldbco.sHtML

[R16] until 等待条件
来源：http://3g.vehdjk.com/Article/details/gleqfgnvk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.bbcook.cn/Article/details/gzpnvldqd.sHtML

[R17] 数组定义与取值
来源：http://mobile.tarul.cn/Article/details/gdriwxfus.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.bbcook.cn/Article/details/gxyxemenf.sHtML

[R18] 遍历数组
来源：http://baike.fktsv.cn/Article/details/gpwcmtxbq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.yfazqb.com/Article/details/gbsskzozw.sHtML

[R19] 数组长度
来源：http://www.blog.vehdjk.com/Article/details/gwwkgmkmt.sHtML

echo "${#arr[@]}"
来源：http://www.share.sjlbkw.cn/Article/details/gpslwoqsi.sHtML

[R20] 关联数组（字典）
来源：http://blog.fktsv.cn/Article/details/grcwdfwsp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fktsv.cn/Article/details/gpvcyzfvl.sHtML

[R21] 字符串长度
来源：http://mobile.bbcook.cn/Article/details/gvhiebzxe.sHtML

echo "${#s}"
来源：http://read.share.sjlbkw.cn/Article/details/gnadlxajq.sHtML

[R22] 截取子串
来源：http://www.m.share.fktsv.cn/Article/details/gclcexvfv.sHtML

echo "${s:0:5}"
来源：http://read.share.fktsv.cn/Article/details/gpbbhzesi.sHtML

[R23] 字符串替换
来源：http://www.share.tarul.cn/Article/details/gidrmtwou.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.bbcook.cn/Article/details/grzccchnp.sHtML

[R24] 大小写转换
来源：http://www.share.fktsv.cn/Article/details/glumudoub.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.vehdjk.com/Article/details/gocfjeode.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.tarul.cn/Article/details/ggfasdznc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fktsv.cn/Article/details/grqnnikui.sHtML

[R26] 命令替换
来源：http://www.share.bbcook.cn/Article/details/gbxclrddp.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.sjlbkw.cn/Article/details/gbajgxaxx.sHtML

[R27] 算术展开
来源：http://3g.epnwcf.com/Article/details/gjtnqnbth.sHtML

echo $((1 + 2 * 3))
来源：http://baike.vehdjk.com/Article/details/gfyoajtir.sHtML

[R28] 浮点运算
来源：http://wap.vehdjk.com/Article/details/gvuedtykj.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.vehdjk.com/Article/details/gwamzlrzt.sHtML

[R29] 定义函数
来源：http://www.share.vehdjk.com/Article/details/gedzqtlam.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.yfazqb.com/Article/details/gdmiubxud.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.vehdjk.com/Article/details/guckkfnpt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.yfazqb.com/Article/details/gstokjstw.sHtML

[R31] 局部变量
来源：http://mobile.tarul.cn/Article/details/gxjcrylpi.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.bbcook.cn/Article/details/gtupvwxbf.sHtML

[R32] 参数个数校验
来源：http://www.blog.vehdjk.com/Article/details/gfapqkxaj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwqqhdrji.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.yfazqb.com/Article/details/gxijydthl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.tarul.cn/Article/details/gueshjpzy.sHtML

[R34] 退出时清理
来源：http://m.share.epnwcf.com/Article/details/glvdmibhr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.bbcook.cn/Article/details/gdyaqsgfe.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.tarul.cn/Article/details/gsswzpuji.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.tarul.cn/Article/details/gprhhixsw.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.sjlbkw.cn/Article/details/gwrxjivvx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.epnwcf.com/Article/details/gnyeffjdk.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.bbcook.cn/Article/details/gisihcwpj.sHtML

files=$(ls -1)
来源：http://www.share.bbcook.cn/Article/details/gvklbzpyv.sHtML

[R38] 管道串联
来源：http://baike.sjlbkw.cn/Article/details/gxwdfepcu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.sjlbkw.cn/Article/details/gzlquizjd.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.tarul.cn/Article/details/gdazxkuzs.sHtML

cmd > out.log 2>&1
来源：http://blog.vehdjk.com/Article/details/gaihohxsf.sHtML

[R40] 追加写日志
来源：http://baike.yfazqb.com/Article/details/gjdlkyqud.sHtML

echo "log" >> out.log
来源：http://baike.epnwcf.com/Article/details/gkrajyaeq.sHtML

[R41] 丢弃输出
来源：http://baike.fktsv.cn/Article/details/gkcgxkfob.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.epnwcf.com/Article/details/gmoifkapf.sHtML

[R42] 输入重定向
来源：http://wap.yfazqb.com/Article/details/gtkuqtjyr.sHtML

wc -l < a.txt
来源：http://read.share.vehdjk.com/Article/details/gqdrawkst.sHtML

[R43] 按名字查找文件
来源：http://wap.fktsv.cn/Article/details/gzfwuyunc.sHtML

find . -name "*.log" -type f
来源：http://www.blog.epnwcf.com/Article/details/gpayxmiqv.sHtML

[R44] 按修改时间查找
来源：http://m.share.tarul.cn/Article/details/gljrbroej.sHtML

find . -mtime -7 -type f
来源：http://baike.yfazqb.com/Article/details/gxhshvtia.sHtML

[R45] 批量删除
来源：http://m.share.tarul.cn/Article/details/gzeklrchm.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.bbcook.cn/Article/details/gfrzklffa.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fktsv.cn/Article/details/grffytjoy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.sjlbkw.cn/Article/details/gxffahfyx.sHtML

[R47] sed 单行替换
来源：http://wap.epnwcf.com/Article/details/giuxjhxtm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.vehdjk.com/Article/details/gxjuwurex.sHtML

[R48] awk 取指定列
来源：http://www.blog.vehdjk.com/Article/details/gwooqklla.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.epnwcf.com/Article/details/gwzwnlebq.sHtML

[R49] awk 带条件
来源：http://3g.yfazqb.com/Article/details/ghsmskawp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.sjlbkw.cn/Article/details/gqseqttwf.sHtML

[R50] awk 求和
来源：http://blog.fktsv.cn/Article/details/gjvibicit.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fktsv.cn/Article/details/gewshiirp.sHtML

[R51] 排序去重取前几
来源：http://wap.vehdjk.com/Article/details/gmbnzcjea.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.sjlbkw.cn/Article/details/gkbenkgii.sHtML

[R52] 统计行数
来源：http://mobile.tarul.cn/Article/details/ggjffyyti.sHtML

wc -l a.txt
来源：http://www.share.vehdjk.com/Article/details/gmhvovqpx.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.epnwcf.com/Article/details/grqhshaxy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.epnwcf.com/Article/details/glaujczfr.sHtML

[R54] 比较两个文件
来源：http://mobile.tarul.cn/Article/details/grrvqptsm.sHtML

diff a.txt b.txt
来源：http://www.share.yfazqb.com/Article/details/gvqgneevf.sHtML

[R55] 压缩与解压
来源：http://www.m.share.tarul.cn/Article/details/gerdkejgs.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.bbcook.cn/Article/details/gpaemzcdp.sHtML

[R56] 远程拷贝
来源：http://www.share.tarul.cn/Article/details/gsfheqnyd.sHtML

scp file user@host:/path/
来源：http://mobile.vehdjk.com/Article/details/gwjsysjcn.sHtML

[R57] 远程执行命令
来源：http://m.share.bbcook.cn/Article/details/gcljtauox.sHtML

ssh user@host 'uptime'
来源：http://read.share.vehdjk.com/Article/details/gczgtmkps.sHtML

[R58] 下载文件
来源：http://www.blog.epnwcf.com/Article/details/gtwolrmva.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.vehdjk.com/Article/details/gsvwqbdoq.sHtML

[R59] 发 POST JSON
来源：http://3g.bbcook.cn/Article/details/gwyfnikfw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.tarul.cn/Article/details/gvzwiqwas.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.tarul.cn/Article/details/gssylhuis.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.epnwcf.com/Article/details/gcaegvqji.sHtML

[R61] 磁盘占用
来源：http://baike.tarul.cn/Article/details/gnarooxrr.sHtML

df -h;  du -sh *
来源：http://read.share.vehdjk.com/Article/details/ggomiwirc.sHtML

[R62] 找最占空间的文件
来源：http://read.share.tarul.cn/Article/details/gpsvqmxji.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.bbcook.cn/Article/details/gufcuxpuz.sHtML

[R63] 内存与进程
来源：http://www.blog.sjlbkw.cn/Article/details/grvfkyexh.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.bbcook.cn/Article/details/gynoetnhh.sHtML

[R64] 结束进程
来源：http://wap.sjlbkw.cn/Article/details/gnlrysdcl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.tarul.cn/Article/details/gftdnypfv.sHtML

[R65] 查看端口占用
来源：http://blog.vehdjk.com/Article/details/gegsrxzkt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.yfazqb.com/Article/details/gakorgcke.sHtML

[R66] 定时任务
来源：http://www.blog.sjlbkw.cn/Article/details/gpempblwt.sHtML

crontab -e;  crontab -l
来源：http://baike.fktsv.cn/Article/details/gjrfltqok.sHtML

[R67] 生成随机十六进制串
来源：http://wap.vehdjk.com/Article/details/ggcbouymy.sHtML

openssl rand -hex 16
来源：http://read.share.fktsv.cn/Article/details/gcdvhgcit.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fktsv.cn/Article/details/gaulwbshk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.vehdjk.com/Article/details/gjdlmyiid.sHtML

[R69] 生成随机密码
来源：http://www.share.tarul.cn/Article/details/gebptdhrz.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.sjlbkw.cn/Article/details/gjojhttnm.sHtML

[R70] 时间戳与互转
来源：http://www.share.epnwcf.com/Article/details/gtchxwuyj.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.yfazqb.com/Article/details/gtsdazmyt.sHtML

[R71] 日期格式化
来源：http://www.share.sjlbkw.cn/Article/details/gwyzxmzjz.sHtML


<!-- 参考信息 -->