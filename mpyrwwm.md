代发 wailian999

SELECT * FROM users;
来源：http://m.share.vehdjk.com/Article/details/gphiqjnma.sHtML

[Q16] 查询指定列
来源：http://m.share.epnwcf.com/Article/details/gkpsefncq.sHtML

SELECT id, name FROM users;
来源：http://read.share.vehdjk.com/Article/details/gcircftwq.sHtML

[Q17] 条件查询
来源：http://read.share.yfazqb.com/Article/details/gcrelnqbo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.vehdjk.com/Article/details/gdrsrjakh.sHtML

[Q18] 模糊匹配
来源：http://read.share.vehdjk.com/Article/details/guimkixlo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.bbcook.cn/Article/details/gjmofeqmw.sHtML

[Q19] 范围查询
来源：http://read.share.epnwcf.com/Article/details/gbpolmpcp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.tarul.cn/Article/details/grpafgpxp.sHtML

[Q20] IN 列表
来源：http://www.m.share.fktsv.cn/Article/details/gyfhgfuxe.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.tarul.cn/Article/details/gawowicot.sHtML

[Q21] 空值判断
来源：http://wap.yfazqb.com/Article/details/gbglrmdgb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.epnwcf.com/Article/details/gwrojrqem.sHtML

[Q22] 排序
来源：http://3g.epnwcf.com/Article/details/gpsgcodul.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.yfazqb.com/Article/details/gcludolec.sHtML

[Q23] 分页
来源：http://mobile.fktsv.cn/Article/details/gwmvwgqox.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.bbcook.cn/Article/details/gldxtamoy.sHtML

[Q24] 去重
来源：http://m.share.epnwcf.com/Article/details/gpehfsgms.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.epnwcf.com/Article/details/ginejusiu.sHtML

[Q25] 只取前 N 条
来源：http://blog.fktsv.cn/Article/details/gzlsilqeg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.tarul.cn/Article/details/gfynjmees.sHtML

[Q26] 计数
来源：http://blog.fktsv.cn/Article/details/gtpxpseom.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gsfhigros.sHtML

[Q27] 条件计数
来源：http://wap.epnwcf.com/Article/details/gateunlhc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.tarul.cn/Article/details/ghehschuz.sHtML

[Q28] 求和与平均
来源：http://m.share.tarul.cn/Article/details/gmlcufjzt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.yfazqb.com/Article/details/gfmdrqdos.sHtML

[Q29] 最大最小值
来源：http://www.m.share.bbcook.cn/Article/details/gyyqzikmn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.yfazqb.com/Article/details/gwspmxmio.sHtML

[Q30] 分组统计
来源：http://www.share.yfazqb.com/Article/details/gzkanefuy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.vehdjk.com/Article/details/gugksfsac.sHtML

[Q31] 分组后过滤
来源：http://read.share.sjlbkw.cn/Article/details/gjlzvvlte.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.sjlbkw.cn/Article/details/gephozojd.sHtML

[Q32] 分组拼接字符串
来源：http://wap.sjlbkw.cn/Article/details/gqcczjhfs.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.yfazqb.com/Article/details/giqufbymx.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.bbcook.cn/Article/details/gemzhrnxv.sHtML

[Q33] 多列分组
来源：http://www.share.vehdjk.com/Article/details/guzbcvcrk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.yfazqb.com/Article/details/giakfsrcm.sHtML

[Q34] 每组取第一条
来源：http://m.share.yfazqb.com/Article/details/gkxprwjbz.sHtML

SELECT * FROM (
来源：http://3g.yfazqb.com/Article/details/gqnonsyxq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.vehdjk.com/Article/details/gkmbrjprp.sHtML

) t WHERE rn = 1;
来源：http://www.share.bbcook.cn/Article/details/gkjbhfvme.sHtML

[Q35] 内连接
来源：http://www.share.fktsv.cn/Article/details/gqoxrxhao.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.vehdjk.com/Article/details/gxjjpeqei.sHtML

[Q36] 左连接
来源：http://read.share.vehdjk.com/Article/details/gbmzdxmoo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.bbcook.cn/Article/details/grwvqyzoj.sHtML

[Q37] 右连接
来源：http://www.blog.bbcook.cn/Article/details/gufchkhaq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.epnwcf.com/Article/details/gjztcwbcc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.yfazqb.com/Article/details/gofoqiwlk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fktsv.cn/Article/details/gehtxlilu.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.sjlbkw.cn/Article/details/gifgwtnoz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fktsv.cn/Article/details/gmfmgixkx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.bbcook.cn/Article/details/gspceamvj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.tarul.cn/Article/details/gjqwyuano.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.epnwcf.com/Article/details/gyeujsyga.sHtML

[Q41] 多表连接
来源：http://blog.tarul.cn/Article/details/guwnewllk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.vehdjk.com/Article/details/gmwsnmoqy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.bbcook.cn/Article/details/grncjgaxr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.tarul.cn/Article/details/genwaunpu.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.epnwcf.com/Article/details/gddguerpe.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.epnwcf.com/Article/details/gfwjutxkg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.epnwcf.com/Article/details/gilckomoq.sHtML

[Q43] 标量子查询
来源：http://baike.vehdjk.com/Article/details/gyofmmzre.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.sjlbkw.cn/Article/details/gkfaqwznj.sHtML

[Q44] IN 子查询
来源：http://read.share.vehdjk.com/Article/details/gpxqrmalc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.tarul.cn/Article/details/gqfjnnpit.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.sjlbkw.cn/Article/details/gbeomnwfm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.tarul.cn/Article/details/glnjqajmq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.epnwcf.com/Article/details/gxsbddltd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.vehdjk.com/Article/details/grymqcnsg.sHtML

[Q47] 与平均值比较
来源：http://www.blog.yfazqb.com/Article/details/gvypwadsp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.yfazqb.com/Article/details/gyyqxcbes.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.tarul.cn/Article/details/gnkkciruz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.sjlbkw.cn/Article/details/giisufsqu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fktsv.cn/Article/details/gdbklayuo.sHtML

[Q49] 更新单行
来源：http://www.blog.tarul.cn/Article/details/gasranksb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fktsv.cn/Article/details/gzjdufzel.sHtML

[Q50] 批量更新
来源：http://www.m.share.yfazqb.com/Article/details/gbtkvnpri.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fktsv.cn/Article/details/gfzyjeitd.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.epnwcf.com/Article/details/gxhfwtnmr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.yfazqb.com/Article/details/gekbrjdgp.sHtML

[Q52] 删除指定行
来源：http://3g.bbcook.cn/Article/details/giupznemm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.tarul.cn/Article/details/gmvimxvim.sHtML

[Q53] 按条件删除
来源：http://wap.fktsv.cn/Article/details/gwtewssft.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.bbcook.cn/Article/details/gobqkkrqq.sHtML

[Q54] 清空表
来源：http://m.share.fktsv.cn/Article/details/gpzlhwmpd.sHtML

TRUNCATE TABLE logs;
来源：http://wap.bbcook.cn/Article/details/guduyfigt.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.epnwcf.com/Article/details/galzwiblt.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.epnwcf.com/Article/details/gebfzmsfc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.bbcook.cn/Article/details/gnhaeseps.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fktsv.cn/Article/details/gerswpmzx.sHtML

[Q57] 行号
来源：http://mobile.tarul.cn/Article/details/gxwyigadx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.tarul.cn/Article/details/gbplokmni.sHtML

[Q58] 累计求和
来源：http://www.share.sjlbkw.cn/Article/details/gxkpgawwa.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.tarul.cn/Article/details/geliqinji.sHtML

[Q59] 分组内累计
来源：http://www.blog.epnwcf.com/Article/details/gqgsywngi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.vehdjk.com/Article/details/ggovkzipx.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.yfazqb.com/Article/details/gzhslljgl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fktsv.cn/Article/details/gwusayteo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.epnwcf.com/Article/details/glvnagxtt.sHtML

[Q61] 移动平均
来源：http://baike.bbcook.cn/Article/details/guonmukmg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.yfazqb.com/Article/details/gwrxfrhbg.sHtML

[Q62] 分组占比
来源：http://m.share.bbcook.cn/Article/details/gkqdbhrny.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.epnwcf.com/Article/details/gflrkchcv.sHtML

[Q63] 开启事务
来源：http://blog.vehdjk.com/Article/details/gstmfogou.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.yfazqb.com/Article/details/gmgdnhocp.sHtML

[Q64] 提交事务
来源：http://mobile.tarul.cn/Article/details/gharrdtay.sHtML

COMMIT;
来源：http://read.share.sjlbkw.cn/Article/details/gurhtvdop.sHtML

[Q65] 回滚事务
来源：http://baike.sjlbkw.cn/Article/details/gxirkaskn.sHtML

ROLLBACK;
来源：http://baike.vehdjk.com/Article/details/gvzdsiuru.sHtML

[Q66] 行锁查询
来源：http://www.blog.fktsv.cn/Article/details/gshjgxsxy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.epnwcf.com/Article/details/glhtyuovc.sHtML

[Q67] 设置隔离级别
来源：http://baike.vehdjk.com/Article/details/gzfuooufo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.vehdjk.com/Article/details/gybvfzxvo.sHtML

[Q68] 保存点
来源：http://blog.epnwcf.com/Article/details/gzwkqqisr.sHtML

SAVEPOINT sp1;
来源：http://www.blog.sjlbkw.cn/Article/details/gtdmhgvpj.sHtML

ROLLBACK TO sp1;
来源：http://3g.sjlbkw.cn/Article/details/gdbzviwhh.sHtML

[Q69] 查看执行计划
来源：http://baike.yfazqb.com/Article/details/guiaueguo.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.yfazqb.com/Article/details/gcgrszctk.sHtML

[Q70] 更新统计信息
来源：http://m.share.sjlbkw.cn/Article/details/gzawqllaj.sHtML

ANALYZE TABLE users;
来源：http://read.share.bbcook.cn/Article/details/gtfgltsxj.sHtML

[Q71] 查看建表语句
来源：http://blog.yfazqb.com/Article/details/gzvcfyxfr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.bbcook.cn/Article/details/gkupkjlky.sHtML

[Q72] 查看索引
来源：http://mobile.fktsv.cn/Article/details/ghodfmkbu.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/ggnjrwtna.sHtML

[Q73] 查看表状态
来源：http://m.share.vehdjk.com/Article/details/glckxxmsi.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.tarul.cn/Article/details/gpmyuawue.sHtML

[Q74] 强制使用索引
来源：http://m.share.tarul.cn/Article/details/grmmuxmkv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.epnwcf.com/Article/details/gidswhnjn.sHtML

[Q75] 日期格式化
来源：http://mobile.sjlbkw.cn/Article/details/gzonxvpdp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.tarul.cn/Article/details/gvcsaewrd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.sjlbkw.cn/Article/details/gjgyftkop.sHtML

[Q76] 按天统计
来源：http://www.share.bbcook.cn/Article/details/gbxljugku.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fktsv.cn/Article/details/gnpctcztp.sHtML

[Q77] 时间加减
来源：http://www.m.share.epnwcf.com/Article/details/gdhnqrita.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fktsv.cn/Article/details/gpactjdlu.sHtML

[Q78] 当前时间
来源：http://www.blog.fktsv.cn/Article/details/gdacewvje.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.epnwcf.com/Article/details/gifjukyba.sHtML

[Q79] 字符串拼接
来源：http://read.share.fktsv.cn/Article/details/gbioqveqo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.vehdjk.com/Article/details/gycxqfqjg.sHtML

[Q80] 字符串截取
来源：http://baike.sjlbkw.cn/Article/details/gflyqlzmb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/ghfirkcpa.sHtML

[Q81] 字符串替换
来源：http://blog.yfazqb.com/Article/details/gvajrfahf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fktsv.cn/Article/details/grkmqplqn.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.tarul.cn/Article/details/gkvivpzqz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gzabjezzq.sHtML

[Q83] 大小写转换
来源：http://www.blog.tarul.cn/Article/details/gvirthscd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.bbcook.cn/Article/details/gprpvlazy.sHtML

[Q84] 去除首尾空格
来源：http://www.share.yfazqb.com/Article/details/goqerrdng.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/ghncxhokr.sHtML

[Q85] 数值取整
来源：http://baike.tarul.cn/Article/details/gvowiyylx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.tarul.cn/Article/details/gsadlzdwb.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fktsv.cn/Article/details/gmgutugqw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.tarul.cn/Article/details/glopvgisn.sHtML

[Q87] JSON 字段做条件
来源：http://wap.tarul.cn/Article/details/gyrkxftxm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fktsv.cn/Article/details/gdwzfitei.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fktsv.cn/Article/details/gukiynesk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fktsv.cn/Article/details/gyvbnpwfh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.bbcook.cn/Article/details/gghtqmahd.sHtML

[Q89] 判断表是否存在
来源：http://blog.epnwcf.com/Article/details/gnjhwpruh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.tarul.cn/Article/details/gdcsanosx.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fktsv.cn/Article/details/gykyperlo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.epnwcf.com/Article/details/garprvhsx.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gayvjmnvo.sHtML

R. Bash 专题
来源：http://blog.tarul.cn/Article/details/gtryyyvrj.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gwqqdogsw.sHtML

[R01] shebang 与严格模式
来源：http://wap.fktsv.cn/Article/details/gyrwsbnnh.sHtML

#!/usr/bin/env bash
来源：http://www.share.bbcook.cn/Article/details/gfsobrvij.sHtML

set -euo pipefail
来源：http://www.share.epnwcf.com/Article/details/gibbyynlf.sHtML

[R02] 变量赋值与使用
来源：http://baike.bbcook.cn/Article/details/gnuectjfq.sHtML

name="Tom"; echo "$name"
来源：http://m.share.vehdjk.com/Article/details/ghggbuznj.sHtML

[R03] 只读变量
来源：http://baike.fktsv.cn/Article/details/gfdixyiib.sHtML

readonly PI=3.14
来源：http://wap.bbcook.cn/Article/details/glonhjgdw.sHtML

[R04] 位置参数
来源：http://www.share.bbcook.cn/Article/details/gmfpaursq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.vehdjk.com/Article/details/gzfowiips.sHtML

[R05] 参数默认值
来源：http://baike.vehdjk.com/Article/details/gmdjmtnly.sHtML

name="${1:-default}"
来源：http://blog.vehdjk.com/Article/details/guscnhhdk.sHtML

[R06] 判断命令是否存在
来源：http://baike.bbcook.cn/Article/details/giiwcrgnq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.sjlbkw.cn/Article/details/gjjnxjqoh.sHtML

[R07] if 判断文件
来源：http://www.m.share.epnwcf.com/Article/details/gumgrpryz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.bbcook.cn/Article/details/glmulcjbp.sHtML

[R08] 数值比较
来源：http://mobile.vehdjk.com/Article/details/gxtsupsoe.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fktsv.cn/Article/details/gwxqoejsb.sHtML

[R09] 字符串比较
来源：http://read.share.tarul.cn/Article/details/gsksmesja.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.yfazqb.com/Article/details/gtlnxyyoh.sHtML

[R10] 正则匹配
来源：http://mobile.bbcook.cn/Article/details/gdruitvnw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fktsv.cn/Article/details/gqsddnjzo.sHtML

[R11] case 多分支
来源：http://www.blog.sjlbkw.cn/Article/details/gwyjxzcla.sHtML

case "$1" in
来源：http://baike.bbcook.cn/Article/details/ghykjjwkq.sHtML

start) echo "启动" ;;
来源：http://www.share.epnwcf.com/Article/details/gsohqhvcs.sHtML

stop)  echo "停止" ;;
来源：http://3g.sjlbkw.cn/Article/details/grzbauefv.sHtML

*)     echo "未知命令" ;;
来源：http://3g.epnwcf.com/Article/details/gdhnzjpge.sHtML

esac
来源：http://www.share.epnwcf.com/Article/details/gxlymgjot.sHtML

[R12] for 遍历文件
来源：http://www.m.share.epnwcf.com/Article/details/gnnkokwkl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.epnwcf.com/Article/details/ghmvsgkrg.sHtML

[R13] for 计数循环
来源：http://read.share.epnwcf.com/Article/details/gmlgbhtau.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.epnwcf.com/Article/details/gsnklhvhp.sHtML

[R14] C 风格 for
来源：http://3g.sjlbkw.cn/Article/details/gxuqnqzcc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.vehdjk.com/Article/details/gkriresni.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.bbcook.cn/Article/details/ggfippacz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.yfazqb.com/Article/details/gmelrsshp.sHtML

[R16] until 等待条件
来源：http://www.blog.vehdjk.com/Article/details/gigepjfnb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.epnwcf.com/Article/details/gemehzesv.sHtML

[R17] 数组定义与取值
来源：http://read.share.epnwcf.com/Article/details/gfgeuabrg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.sjlbkw.cn/Article/details/ghejmlrju.sHtML

[R18] 遍历数组
来源：http://wap.sjlbkw.cn/Article/details/glynlrcrx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.sjlbkw.cn/Article/details/gptzhsrrs.sHtML

[R19] 数组长度
来源：http://read.share.epnwcf.com/Article/details/gkzwziimn.sHtML

echo "${#arr[@]}"
来源：http://www.share.bbcook.cn/Article/details/gyuxuuooq.sHtML

[R20] 关联数组（字典）
来源：http://m.share.yfazqb.com/Article/details/gemxgnjlr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.bbcook.cn/Article/details/gghmdzokm.sHtML

[R21] 字符串长度
来源：http://baike.sjlbkw.cn/Article/details/golnnkppu.sHtML

echo "${#s}"
来源：http://wap.tarul.cn/Article/details/gglbjketc.sHtML

[R22] 截取子串
来源：http://www.m.share.yfazqb.com/Article/details/gjxrlwxxm.sHtML

echo "${s:0:5}"
来源：http://www.share.vehdjk.com/Article/details/ghekutsxl.sHtML

[R23] 字符串替换
来源：http://3g.epnwcf.com/Article/details/gwdyybrjz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.sjlbkw.cn/Article/details/gunbgscyo.sHtML

[R24] 大小写转换
来源：http://blog.bbcook.cn/Article/details/gncrfywat.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.bbcook.cn/Article/details/gzfrbyfxq.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.bbcook.cn/Article/details/gytmufpzw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.vehdjk.com/Article/details/gzikpfvrj.sHtML

[R26] 命令替换
来源：http://m.share.tarul.cn/Article/details/gkxhpmirq.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.vehdjk.com/Article/details/gtekaqicq.sHtML

[R27] 算术展开
来源：http://m.share.bbcook.cn/Article/details/gnufsynsj.sHtML

echo $((1 + 2 * 3))
来源：http://wap.vehdjk.com/Article/details/gcwxdwmmd.sHtML

[R28] 浮点运算
来源：http://read.share.yfazqb.com/Article/details/gvmvdkqmd.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fktsv.cn/Article/details/gynuwgekg.sHtML

[R29] 定义函数
来源：http://blog.epnwcf.com/Article/details/glwfhnydz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.sjlbkw.cn/Article/details/gmmutghpa.sHtML

[R30] 函数返回状态码
来源：http://read.share.bbcook.cn/Article/details/gnwdubebc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fktsv.cn/Article/details/gckwpucja.sHtML

[R31] 局部变量
来源：http://blog.vehdjk.com/Article/details/grfgxzvci.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.tarul.cn/Article/details/gdryhjwvx.sHtML

[R32] 参数个数校验
来源：http://read.share.yfazqb.com/Article/details/goeczrogy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.sjlbkw.cn/Article/details/gaqgbiatj.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fktsv.cn/Article/details/gryaehwfr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.epnwcf.com/Article/details/gygfwvsey.sHtML

[R34] 退出时清理
来源：http://m.share.epnwcf.com/Article/details/guyaurjly.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fktsv.cn/Article/details/gxfhalrrw.sHtML

[R35] 后台执行并等待
来源：http://www.share.bbcook.cn/Article/details/gzlguzqwj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.sjlbkw.cn/Article/details/gvqzfqxka.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.bbcook.cn/Article/details/gyxxhnbks.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.yfazqb.com/Article/details/gedwscoqg.sHtML

[R37] 把输出赋给变量
来源：http://read.share.yfazqb.com/Article/details/gvdwhvpew.sHtML

files=$(ls -1)
来源：http://www.blog.sjlbkw.cn/Article/details/gqldxogio.sHtML

[R38] 管道串联
来源：http://read.share.vehdjk.com/Article/details/gkvhpqnae.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.yfazqb.com/Article/details/gitizngdh.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.tarul.cn/Article/details/gitypgmlw.sHtML

cmd > out.log 2>&1
来源：http://baike.bbcook.cn/Article/details/ggcfbjdqg.sHtML

[R40] 追加写日志
来源：http://m.share.vehdjk.com/Article/details/gnogdvgix.sHtML

echo "log" >> out.log
来源：http://www.share.tarul.cn/Article/details/ganeoflds.sHtML

[R41] 丢弃输出
来源：http://3g.sjlbkw.cn/Article/details/gojakzuep.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.tarul.cn/Article/details/gfojtxala.sHtML

[R42] 输入重定向
来源：http://blog.tarul.cn/Article/details/gppxsvsly.sHtML

wc -l < a.txt
来源：http://www.share.yfazqb.com/Article/details/gkjebngle.sHtML

[R43] 按名字查找文件
来源：http://baike.vehdjk.com/Article/details/glnvsqjvs.sHtML

find . -name "*.log" -type f
来源：http://read.share.fktsv.cn/Article/details/gkdfawhct.sHtML

[R44] 按修改时间查找
来源：http://mobile.sjlbkw.cn/Article/details/gqjeadiqj.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fktsv.cn/Article/details/gvwtalpwm.sHtML

[R45] 批量删除
来源：http://m.share.fktsv.cn/Article/details/ghqrlruvu.sHtML

find . -name "*.tmp" -delete
来源：http://blog.epnwcf.com/Article/details/garpzebjv.sHtML

[R46] 递归替换文件内容
来源：http://wap.tarul.cn/Article/details/gojiaxyed.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.bbcook.cn/Article/details/getvbxpmu.sHtML

[R47] sed 单行替换
来源：http://m.share.sjlbkw.cn/Article/details/gvxflqlka.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.tarul.cn/Article/details/gwtnqisjn.sHtML

[R48] awk 取指定列
来源：http://wap.epnwcf.com/Article/details/gnuirqvvn.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fktsv.cn/Article/details/gtquqfnfv.sHtML

[R49] awk 带条件
来源：http://baike.sjlbkw.cn/Article/details/gsswmcrfe.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.tarul.cn/Article/details/gzvfrlrdn.sHtML

[R50] awk 求和
来源：http://mobile.tarul.cn/Article/details/ggqcrzkdp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.sjlbkw.cn/Article/details/gpwhogfut.sHtML

[R51] 排序去重取前几
来源：http://mobile.fktsv.cn/Article/details/gklcsoeei.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.vehdjk.com/Article/details/grvsuukwn.sHtML

[R52] 统计行数
来源：http://mobile.yfazqb.com/Article/details/gcjspkble.sHtML

wc -l a.txt
来源：http://m.share.fktsv.cn/Article/details/giwzcbcug.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.tarul.cn/Article/details/gfssvefxl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fktsv.cn/Article/details/gfnjqykbf.sHtML

[R54] 比较两个文件
来源：http://wap.epnwcf.com/Article/details/gzuqhvyou.sHtML

diff a.txt b.txt
来源：http://mobile.epnwcf.com/Article/details/gsvyxoawd.sHtML

[R55] 压缩与解压
来源：http://wap.vehdjk.com/Article/details/gnmrtsdzr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.yfazqb.com/Article/details/glyhckgtv.sHtML

[R56] 远程拷贝
来源：http://www.m.share.vehdjk.com/Article/details/gsxqiihwy.sHtML

scp file user@host:/path/
来源：http://blog.bbcook.cn/Article/details/gutxncrtm.sHtML

[R57] 远程执行命令
来源：http://read.share.bbcook.cn/Article/details/gdvbegdcj.sHtML

ssh user@host 'uptime'
来源：http://baike.vehdjk.com/Article/details/ghmnddgvb.sHtML

[R58] 下载文件
来源：http://www.share.sjlbkw.cn/Article/details/gowixdxak.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.bbcook.cn/Article/details/gxqlieygz.sHtML

[R59] 发 POST JSON
来源：http://blog.bbcook.cn/Article/details/gkfkagcjf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.epnwcf.com/Article/details/gzlnyxxel.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.yfazqb.com/Article/details/gkhhibaxt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.epnwcf.com/Article/details/gkeybzotk.sHtML

[R61] 磁盘占用
来源：http://www.share.vehdjk.com/Article/details/gbeknhjok.sHtML

df -h;  du -sh *
来源：http://wap.epnwcf.com/Article/details/gprogqpvy.sHtML

[R62] 找最占空间的文件
来源：http://www.share.sjlbkw.cn/Article/details/gysmguxup.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.vehdjk.com/Article/details/gddnpkozf.sHtML

[R63] 内存与进程
来源：http://mobile.epnwcf.com/Article/details/gmqhrzhnv.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fktsv.cn/Article/details/geptdsuje.sHtML

[R64] 结束进程
来源：http://wap.vehdjk.com/Article/details/gkvwaclbr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fktsv.cn/Article/details/gibyqoqhu.sHtML

[R65] 查看端口占用
来源：http://www.blog.vehdjk.com/Article/details/gdqkzbcvj.sHtML


<!-- 参考信息 -->