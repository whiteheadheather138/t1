代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.tarul.cn/Article/details/gvdloggcz.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fktsv.cn/Article/details/gyynoyvpv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.sjlbkw.cn/Article/details/gcgaeyjaj.sHtML

[Q19] 范围查询
来源：http://3g.epnwcf.com/Article/details/gmnoxcwuc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.tarul.cn/Article/details/gimlxrcqn.sHtML

[Q20] IN 列表
来源：http://m.share.yfazqb.com/Article/details/gjwpukqst.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.bbcook.cn/Article/details/gdickbjfi.sHtML

[Q21] 空值判断
来源：http://read.share.yfazqb.com/Article/details/gnefrrnwu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.sjlbkw.cn/Article/details/gpjbphwdn.sHtML

[Q22] 排序
来源：http://www.m.share.tarul.cn/Article/details/gaxvqeqzd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.sjlbkw.cn/Article/details/gehuamcez.sHtML

[Q23] 分页
来源：http://m.share.yfazqb.com/Article/details/gwupzkdlb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fktsv.cn/Article/details/gsagglyja.sHtML

[Q24] 去重
来源：http://read.share.vehdjk.com/Article/details/ghwmlprxw.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.tarul.cn/Article/details/guribqwdp.sHtML

[Q25] 只取前 N 条
来源：http://read.share.yfazqb.com/Article/details/ghoklzpck.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.epnwcf.com/Article/details/gjqjplfqi.sHtML

[Q26] 计数
来源：http://www.blog.tarul.cn/Article/details/gpmxlqhwr.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.yfazqb.com/Article/details/gczeknkzk.sHtML

[Q27] 条件计数
来源：http://mobile.fktsv.cn/Article/details/gyqirxvbj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.vehdjk.com/Article/details/gjnpjbxnu.sHtML

[Q28] 求和与平均
来源：http://www.share.sjlbkw.cn/Article/details/gojwjwzdx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.tarul.cn/Article/details/gypbcytlj.sHtML

[Q29] 最大最小值
来源：http://www.share.tarul.cn/Article/details/gwvwkgmtc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/ggusnssaj.sHtML

[Q30] 分组统计
来源：http://www.share.bbcook.cn/Article/details/gucmtesdl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.epnwcf.com/Article/details/gllzzokaw.sHtML

[Q31] 分组后过滤
来源：http://www.share.yfazqb.com/Article/details/gxkvpknse.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.yfazqb.com/Article/details/gdalfimrp.sHtML

[Q32] 分组拼接字符串
来源：http://wap.bbcook.cn/Article/details/gutfsgjws.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fktsv.cn/Article/details/gtwscvsxu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.bbcook.cn/Article/details/gtlvudssa.sHtML

[Q33] 多列分组
来源：http://baike.yfazqb.com/Article/details/glarguzyp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.vehdjk.com/Article/details/gdzprfxkr.sHtML

[Q34] 每组取第一条
来源：http://blog.vehdjk.com/Article/details/gvoknxmup.sHtML

SELECT * FROM (
来源：http://3g.tarul.cn/Article/details/gnqectsng.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.tarul.cn/Article/details/gpeaulgig.sHtML

) t WHERE rn = 1;
来源：http://mobile.yfazqb.com/Article/details/gicpnrlmy.sHtML

[Q35] 内连接
来源：http://m.share.vehdjk.com/Article/details/gbmmvequo.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fktsv.cn/Article/details/gvdvptumj.sHtML

[Q36] 左连接
来源：http://baike.yfazqb.com/Article/details/gytbbfndi.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.vehdjk.com/Article/details/gkdsnfvxh.sHtML

[Q37] 右连接
来源：http://3g.vehdjk.com/Article/details/gyexuejyi.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.yfazqb.com/Article/details/gidyzqiko.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fktsv.cn/Article/details/ggvplepbe.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.epnwcf.com/Article/details/gqomyxxae.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.tarul.cn/Article/details/glyjpbkni.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.yfazqb.com/Article/details/gfupufxho.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.tarul.cn/Article/details/ghkalmzof.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.epnwcf.com/Article/details/gdcnurbti.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.sjlbkw.cn/Article/details/gesxxgyhx.sHtML

[Q41] 多表连接
来源：http://www.blog.bbcook.cn/Article/details/gwwneptpq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.bbcook.cn/Article/details/gmdzgufps.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fktsv.cn/Article/details/gnnqbbsca.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fktsv.cn/Article/details/gdtikutdv.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.sjlbkw.cn/Article/details/gvoameypd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.vehdjk.com/Article/details/gkhhbthry.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fktsv.cn/Article/details/gkhniswyi.sHtML

[Q43] 标量子查询
来源：http://m.share.tarul.cn/Article/details/grhphzhmm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.vehdjk.com/Article/details/gyzvmvpno.sHtML

[Q44] IN 子查询
来源：http://read.share.fktsv.cn/Article/details/gopmdzmdo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fktsv.cn/Article/details/gwrnjdauv.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.bbcook.cn/Article/details/ginzokyeh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.bbcook.cn/Article/details/gymvpfsqt.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.bbcook.cn/Article/details/gobemotzf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.vehdjk.com/Article/details/gkprgrexc.sHtML

[Q47] 与平均值比较
来源：http://wap.fktsv.cn/Article/details/ggtmuiuyq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.sjlbkw.cn/Article/details/galxdbmwj.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.epnwcf.com/Article/details/gxmllzfyq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.vehdjk.com/Article/details/gdaayvaqu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.sjlbkw.cn/Article/details/gqzoduxyw.sHtML

[Q49] 更新单行
来源：http://www.blog.epnwcf.com/Article/details/gkcpbmhdk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.yfazqb.com/Article/details/gctqvniqc.sHtML

[Q50] 批量更新
来源：http://www.blog.bbcook.cn/Article/details/garigbfjr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.vehdjk.com/Article/details/gnxdtzanx.sHtML

[Q51] 用子查询更新
来源：http://baike.sjlbkw.cn/Article/details/goggiepqy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.tarul.cn/Article/details/glfukasrk.sHtML

[Q52] 删除指定行
来源：http://3g.epnwcf.com/Article/details/gykuienrz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.yfazqb.com/Article/details/gyhlwouyj.sHtML

[Q53] 按条件删除
来源：http://www.blog.sjlbkw.cn/Article/details/gsjqzlnrt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.bbcook.cn/Article/details/ggosuouoq.sHtML

[Q54] 清空表
来源：http://m.share.bbcook.cn/Article/details/gznebvyki.sHtML

TRUNCATE TABLE logs;
来源：http://baike.epnwcf.com/Article/details/gxbphdoyx.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fktsv.cn/Article/details/ghezybzab.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.bbcook.cn/Article/details/gxoyyhunx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.sjlbkw.cn/Article/details/gpejxlplx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.bbcook.cn/Article/details/gxbqycdin.sHtML

[Q57] 行号
来源：http://baike.yfazqb.com/Article/details/glgmjtdht.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/ggaweddms.sHtML

[Q58] 累计求和
来源：http://wap.epnwcf.com/Article/details/gbthezjkg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.yfazqb.com/Article/details/gtubmxdie.sHtML

[Q59] 分组内累计
来源：http://www.share.fktsv.cn/Article/details/gbwgprqqv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.tarul.cn/Article/details/gdftlasvd.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.vehdjk.com/Article/details/gijrvetaw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.sjlbkw.cn/Article/details/gjpfsogxf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.vehdjk.com/Article/details/gqokqluvs.sHtML

[Q61] 移动平均
来源：http://www.blog.epnwcf.com/Article/details/gpkxwpelo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/gymviiajm.sHtML

[Q62] 分组占比
来源：http://read.share.epnwcf.com/Article/details/gghpiafcd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fktsv.cn/Article/details/glbyqkrof.sHtML

[Q63] 开启事务
来源：http://www.share.fktsv.cn/Article/details/gfpteugsh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.yfazqb.com/Article/details/ggdjkwfur.sHtML

[Q64] 提交事务
来源：http://www.m.share.tarul.cn/Article/details/gattvchvb.sHtML

COMMIT;
来源：http://www.blog.epnwcf.com/Article/details/gjlirdsva.sHtML

[Q65] 回滚事务
来源：http://3g.bbcook.cn/Article/details/glcvbpckm.sHtML

ROLLBACK;
来源：http://baike.tarul.cn/Article/details/gbvtturzs.sHtML

[Q66] 行锁查询
来源：http://www.share.bbcook.cn/Article/details/gmqwemgsm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fktsv.cn/Article/details/gokjgmlcx.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.epnwcf.com/Article/details/gfzphavrb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.vehdjk.com/Article/details/gwdgcwjnn.sHtML

[Q68] 保存点
来源：http://blog.sjlbkw.cn/Article/details/gsuqpoath.sHtML

SAVEPOINT sp1;
来源：http://wap.sjlbkw.cn/Article/details/glowdatwl.sHtML

ROLLBACK TO sp1;
来源：http://mobile.yfazqb.com/Article/details/goqfcnreq.sHtML

[Q69] 查看执行计划
来源：http://read.share.yfazqb.com/Article/details/gdkxpcbsz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.tarul.cn/Article/details/goflbwicz.sHtML

[Q70] 更新统计信息
来源：http://www.share.epnwcf.com/Article/details/gspwhhizx.sHtML

ANALYZE TABLE users;
来源：http://blog.yfazqb.com/Article/details/ggxnxtpkh.sHtML

[Q71] 查看建表语句
来源：http://baike.yfazqb.com/Article/details/ghpciceku.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.epnwcf.com/Article/details/gnrjttrah.sHtML

[Q72] 查看索引
来源：http://www.m.share.bbcook.cn/Article/details/gtcoewrah.sHtML

SHOW INDEX FROM users;
来源：http://www.share.yfazqb.com/Article/details/guwfvsxfp.sHtML

[Q73] 查看表状态
来源：http://baike.bbcook.cn/Article/details/glsiqmefe.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.vehdjk.com/Article/details/gzlxjtdtb.sHtML

[Q74] 强制使用索引
来源：http://mobile.yfazqb.com/Article/details/ghkktndxl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.epnwcf.com/Article/details/gevouylra.sHtML

[Q75] 日期格式化
来源：http://www.blog.fktsv.cn/Article/details/guqazpvhh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gwgaopbxk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.epnwcf.com/Article/details/gkqrtdqqn.sHtML

[Q76] 按天统计
来源：http://wap.epnwcf.com/Article/details/gjqwrfnen.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fktsv.cn/Article/details/gsyhhsaco.sHtML

[Q77] 时间加减
来源：http://blog.tarul.cn/Article/details/ghtqldkin.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.yfazqb.com/Article/details/gglmrseqi.sHtML

[Q78] 当前时间
来源：http://wap.vehdjk.com/Article/details/gxtburkte.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fktsv.cn/Article/details/gjtuqaytc.sHtML

[Q79] 字符串拼接
来源：http://read.share.bbcook.cn/Article/details/gvxaclmdz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.vehdjk.com/Article/details/gyxeutynx.sHtML

[Q80] 字符串截取
来源：http://wap.sjlbkw.cn/Article/details/gfjblbncz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.yfazqb.com/Article/details/ghzdrhfhb.sHtML

[Q81] 字符串替换
来源：http://3g.fktsv.cn/Article/details/gwsrtpkph.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.bbcook.cn/Article/details/gphncazcv.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.yfazqb.com/Article/details/gjtcbiqbm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.tarul.cn/Article/details/genzykyzx.sHtML

[Q83] 大小写转换
来源：http://3g.tarul.cn/Article/details/gfidkfglc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gczdjiryw.sHtML

[Q84] 去除首尾空格
来源：http://wap.bbcook.cn/Article/details/giaksophe.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.tarul.cn/Article/details/gkzoyvcqt.sHtML

[Q85] 数值取整
来源：http://www.m.share.sjlbkw.cn/Article/details/gbsuyivby.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.epnwcf.com/Article/details/ghctatchb.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.yfazqb.com/Article/details/grpxofwdd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.tarul.cn/Article/details/gtmrvsogs.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.sjlbkw.cn/Article/details/gxvirghzt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.epnwcf.com/Article/details/gxozetyqw.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.yfazqb.com/Article/details/gufoqacru.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.epnwcf.com/Article/details/greodoedv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.tarul.cn/Article/details/gzhllmcfz.sHtML

[Q89] 判断表是否存在
来源：http://3g.bbcook.cn/Article/details/gxkhentmw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.vehdjk.com/Article/details/gdowxjuuk.sHtML

[Q90] 生成序号列
来源：http://m.share.epnwcf.com/Article/details/gonqqigsv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.sjlbkw.cn/Article/details/gmfiatndl.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gcgsmkrwp.sHtML

R. Bash 专题
来源：http://blog.fktsv.cn/Article/details/gsfphulcb.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gfjidgsgu.sHtML

[R01] shebang 与严格模式
来源：http://www.share.bbcook.cn/Article/details/giddpodwh.sHtML

#!/usr/bin/env bash
来源：http://mobile.sjlbkw.cn/Article/details/gnhysjgux.sHtML

set -euo pipefail
来源：http://m.share.vehdjk.com/Article/details/gnmvrsbmr.sHtML

[R02] 变量赋值与使用
来源：http://read.share.sjlbkw.cn/Article/details/gmlwyyvbb.sHtML

name="Tom"; echo "$name"
来源：http://mobile.yfazqb.com/Article/details/gwufptier.sHtML

[R03] 只读变量
来源：http://m.share.bbcook.cn/Article/details/ggkfsdrkw.sHtML

readonly PI=3.14
来源：http://read.share.vehdjk.com/Article/details/gcvqwrept.sHtML

[R04] 位置参数
来源：http://www.m.share.tarul.cn/Article/details/gqfuttwll.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fktsv.cn/Article/details/ggpjjkxvk.sHtML

[R05] 参数默认值
来源：http://www.m.share.vehdjk.com/Article/details/gcqnutfbh.sHtML

name="${1:-default}"
来源：http://baike.fktsv.cn/Article/details/gkryklyvv.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.bbcook.cn/Article/details/gslupgjqy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.bbcook.cn/Article/details/glaqhmwpq.sHtML

[R07] if 判断文件
来源：http://www.share.epnwcf.com/Article/details/gsatwmyxb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.sjlbkw.cn/Article/details/gqankjaxz.sHtML

[R08] 数值比较
来源：http://wap.bbcook.cn/Article/details/gvcykueth.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.epnwcf.com/Article/details/goqoxoqjj.sHtML

[R09] 字符串比较
来源：http://www.share.sjlbkw.cn/Article/details/guababbao.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.sjlbkw.cn/Article/details/gpfckagyz.sHtML

[R10] 正则匹配
来源：http://www.share.sjlbkw.cn/Article/details/gnzuwnimv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.vehdjk.com/Article/details/gtpeybkim.sHtML

[R11] case 多分支
来源：http://www.m.share.vehdjk.com/Article/details/gxechwqal.sHtML

case "$1" in
来源：http://www.share.yfazqb.com/Article/details/gljhsaxuj.sHtML

start) echo "启动" ;;
来源：http://www.share.fktsv.cn/Article/details/gillwgxiu.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fktsv.cn/Article/details/gjwugdlkd.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.vehdjk.com/Article/details/gxdushsff.sHtML

esac
来源：http://read.share.bbcook.cn/Article/details/gmrjdfgtc.sHtML

[R12] for 遍历文件
来源：http://wap.sjlbkw.cn/Article/details/gzclgnnow.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.vehdjk.com/Article/details/gnowzydcc.sHtML

[R13] for 计数循环
来源：http://www.blog.vehdjk.com/Article/details/grzspzmyb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.tarul.cn/Article/details/gifdawxbj.sHtML

[R14] C 风格 for
来源：http://read.share.epnwcf.com/Article/details/grwbdwcmk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.vehdjk.com/Article/details/gfogcqaxg.sHtML

[R15] while 逐行读文件
来源：http://mobile.tarul.cn/Article/details/geduaunap.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.tarul.cn/Article/details/goujwpbgb.sHtML

[R16] until 等待条件
来源：http://3g.vehdjk.com/Article/details/gnslepkpd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.epnwcf.com/Article/details/gzohxrnfe.sHtML

[R17] 数组定义与取值
来源：http://3g.tarul.cn/Article/details/ghzgzhfrb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fktsv.cn/Article/details/gyzlztzhj.sHtML

[R18] 遍历数组
来源：http://www.m.share.vehdjk.com/Article/details/govfqpjkt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.tarul.cn/Article/details/gyszgjusr.sHtML

[R19] 数组长度
来源：http://baike.vehdjk.com/Article/details/gyrnehggl.sHtML

echo "${#arr[@]}"
来源：http://3g.tarul.cn/Article/details/gwwpwkdpa.sHtML

[R20] 关联数组（字典）
来源：http://blog.fktsv.cn/Article/details/gcgprasyg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fktsv.cn/Article/details/gsqevtcql.sHtML

[R21] 字符串长度
来源：http://mobile.tarul.cn/Article/details/gvlumbhks.sHtML

echo "${#s}"
来源：http://www.blog.sjlbkw.cn/Article/details/gjqfzndsw.sHtML

[R22] 截取子串
来源：http://www.m.share.bbcook.cn/Article/details/glunfdnbi.sHtML

echo "${s:0:5}"
来源：http://read.share.epnwcf.com/Article/details/gxoxreowd.sHtML

[R23] 字符串替换
来源：http://read.share.sjlbkw.cn/Article/details/gyhvekgjl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.epnwcf.com/Article/details/gfcgrthzf.sHtML

[R24] 大小写转换
来源：http://mobile.sjlbkw.cn/Article/details/gfpdzezes.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.sjlbkw.cn/Article/details/geihhfvhh.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.epnwcf.com/Article/details/gwsqpflsl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.yfazqb.com/Article/details/gyimzwmxk.sHtML

[R26] 命令替换
来源：http://mobile.bbcook.cn/Article/details/gzrfgyaxc.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.bbcook.cn/Article/details/gwyzflvph.sHtML

[R27] 算术展开
来源：http://blog.bbcook.cn/Article/details/giwncpjsr.sHtML

echo $((1 + 2 * 3))
来源：http://wap.yfazqb.com/Article/details/guyhcnwxh.sHtML

[R28] 浮点运算
来源：http://m.share.sjlbkw.cn/Article/details/ghqqqiimm.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.bbcook.cn/Article/details/gcgepdmww.sHtML

[R29] 定义函数
来源：http://www.m.share.epnwcf.com/Article/details/gfazsruub.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.tarul.cn/Article/details/gvguqrhga.sHtML

[R30] 函数返回状态码
来源：http://wap.tarul.cn/Article/details/gkvzhnpsk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.vehdjk.com/Article/details/gezbtrbtb.sHtML

[R31] 局部变量
来源：http://read.share.bbcook.cn/Article/details/ghetkczni.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.sjlbkw.cn/Article/details/gfnhchaen.sHtML

[R32] 参数个数校验
来源：http://www.blog.tarul.cn/Article/details/giqwxqaym.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.tarul.cn/Article/details/gvnqjtxez.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.sjlbkw.cn/Article/details/gmdstunrg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.yfazqb.com/Article/details/gxeampqpu.sHtML

[R34] 退出时清理
来源：http://www.share.sjlbkw.cn/Article/details/ggqizrjhz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.vehdjk.com/Article/details/guvfwfaad.sHtML

[R35] 后台执行并等待
来源：http://baike.bbcook.cn/Article/details/gbszaqtxo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fktsv.cn/Article/details/gmjzuryfh.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fktsv.cn/Article/details/glzvhilba.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.bbcook.cn/Article/details/gqqhkneac.sHtML

[R37] 把输出赋给变量
来源：http://wap.epnwcf.com/Article/details/gpneenmnp.sHtML

files=$(ls -1)
来源：http://mobile.fktsv.cn/Article/details/geqxhyjhb.sHtML

[R38] 管道串联
来源：http://blog.tarul.cn/Article/details/gnyoejohy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.vehdjk.com/Article/details/glerifazc.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fktsv.cn/Article/details/gcudoijkj.sHtML

cmd > out.log 2>&1
来源：http://wap.tarul.cn/Article/details/goufgters.sHtML

[R40] 追加写日志
来源：http://blog.tarul.cn/Article/details/gqklqsbkn.sHtML

echo "log" >> out.log
来源：http://www.share.epnwcf.com/Article/details/gporwakkz.sHtML

[R41] 丢弃输出
来源：http://read.share.vehdjk.com/Article/details/gzkakxtoh.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.sjlbkw.cn/Article/details/gcyevuxjz.sHtML

[R42] 输入重定向
来源：http://3g.bbcook.cn/Article/details/gtpqbedtx.sHtML

wc -l < a.txt
来源：http://mobile.vehdjk.com/Article/details/gtkotfhpe.sHtML

[R43] 按名字查找文件
来源：http://www.blog.yfazqb.com/Article/details/gbbfazqpd.sHtML

find . -name "*.log" -type f
来源：http://mobile.bbcook.cn/Article/details/gfapuonkz.sHtML

[R44] 按修改时间查找
来源：http://wap.sjlbkw.cn/Article/details/ghevyhtxy.sHtML

find . -mtime -7 -type f
来源：http://blog.sjlbkw.cn/Article/details/gfbznjmvo.sHtML

[R45] 批量删除
来源：http://wap.bbcook.cn/Article/details/ggmglfojq.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.sjlbkw.cn/Article/details/gjgaoadwl.sHtML

[R46] 递归替换文件内容
来源：http://www.share.yfazqb.com/Article/details/gtjemfwye.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.epnwcf.com/Article/details/ggcdxwzkr.sHtML

[R47] sed 单行替换
来源：http://blog.tarul.cn/Article/details/gjqvabjgw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.tarul.cn/Article/details/gdpbmczek.sHtML

[R48] awk 取指定列
来源：http://m.share.vehdjk.com/Article/details/gtlufrgtn.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.bbcook.cn/Article/details/guqbmsdro.sHtML

[R49] awk 带条件
来源：http://www.blog.fktsv.cn/Article/details/gfdupibzd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.tarul.cn/Article/details/gqijrwubk.sHtML

[R50] awk 求和
来源：http://www.share.tarul.cn/Article/details/gbxryhjqx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fktsv.cn/Article/details/gawdgrkty.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.sjlbkw.cn/Article/details/goozlczlg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.sjlbkw.cn/Article/details/gwduyahbn.sHtML

[R52] 统计行数
来源：http://wap.sjlbkw.cn/Article/details/ghzxvhjcv.sHtML

wc -l a.txt
来源：http://3g.fktsv.cn/Article/details/gbyqyxfrl.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fktsv.cn/Article/details/gxrbaapsk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.epnwcf.com/Article/details/gaohiqngu.sHtML

[R54] 比较两个文件
来源：http://read.share.yfazqb.com/Article/details/gyuayykbm.sHtML

diff a.txt b.txt
来源：http://read.share.bbcook.cn/Article/details/gvzhwchqb.sHtML

[R55] 压缩与解压
来源：http://blog.yfazqb.com/Article/details/gqbxbnkdz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.bbcook.cn/Article/details/gyfldnisd.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fktsv.cn/Article/details/gxxuyldgt.sHtML

scp file user@host:/path/
来源：http://www.m.share.yfazqb.com/Article/details/gkgzplkhz.sHtML

[R57] 远程执行命令
来源：http://wap.yfazqb.com/Article/details/gfbgbeajr.sHtML

ssh user@host 'uptime'
来源：http://blog.epnwcf.com/Article/details/gcvjnuwlx.sHtML

[R58] 下载文件
来源：http://www.m.share.epnwcf.com/Article/details/gfalanslt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.epnwcf.com/Article/details/gnaetykwu.sHtML

[R59] 发 POST JSON
来源：http://mobile.vehdjk.com/Article/details/gwgfxwfrs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.yfazqb.com/Article/details/gwcznqzuy.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.vehdjk.com/Article/details/gelnyyyhd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.tarul.cn/Article/details/gwhtvjrox.sHtML

[R61] 磁盘占用
来源：http://www.blog.sjlbkw.cn/Article/details/ghkuibuex.sHtML

df -h;  du -sh *
来源：http://www.share.yfazqb.com/Article/details/gsigxrhyi.sHtML

[R62] 找最占空间的文件
来源：http://m.share.epnwcf.com/Article/details/ghcnfqvjq.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.tarul.cn/Article/details/gjmjkeyql.sHtML

[R63] 内存与进程
来源：http://3g.vehdjk.com/Article/details/gsevqfnvy.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.epnwcf.com/Article/details/gcsgotlqq.sHtML

[R64] 结束进程
来源：http://www.m.share.vehdjk.com/Article/details/gzfvuzgrf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.bbcook.cn/Article/details/gjzhufcba.sHtML

[R65] 查看端口占用
来源：http://m.share.bbcook.cn/Article/details/gqujasngy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.tarul.cn/Article/details/gzdjvfdfc.sHtML

[R66] 定时任务
来源：http://www.blog.tarul.cn/Article/details/gcfbhfalu.sHtML

crontab -e;  crontab -l
来源：http://read.share.yfazqb.com/Article/details/gpsmicosz.sHtML

[R67] 生成随机十六进制串
来源：http://blog.tarul.cn/Article/details/gjumottzp.sHtML


<!-- 参考信息 -->