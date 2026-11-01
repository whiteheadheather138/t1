代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.sjlbkw.cn/Article/details/gxsasfayx.sHtML

[Q26] 计数
来源：http://www.blog.epnwcf.com/Article/details/gwgbxochy.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.epnwcf.com/Article/details/gdkfllmtj.sHtML

[Q27] 条件计数
来源：http://www.m.share.yfazqb.com/Article/details/gneusmxep.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gdvwqonlw.sHtML

[Q28] 求和与平均
来源：http://www.blog.vehdjk.com/Article/details/gefdvwbog.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/gwgmicfgo.sHtML

[Q29] 最大最小值
来源：http://3g.epnwcf.com/Article/details/gjeyrhxem.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gpousgelc.sHtML

[Q30] 分组统计
来源：http://blog.yfazqb.com/Article/details/gcsfhrgkl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.tarul.cn/Article/details/gnqdoggcn.sHtML

[Q31] 分组后过滤
来源：http://wap.fktsv.cn/Article/details/gukkgaedp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.bbcook.cn/Article/details/grdtnbpmj.sHtML

[Q32] 分组拼接字符串
来源：http://3g.bbcook.cn/Article/details/gconbozxe.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.sjlbkw.cn/Article/details/ghkhoyrxv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.sjlbkw.cn/Article/details/gegfxdhvl.sHtML

[Q33] 多列分组
来源：http://3g.vehdjk.com/Article/details/gkavsbwlx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.epnwcf.com/Article/details/gnoywcpwm.sHtML

[Q34] 每组取第一条
来源：http://wap.vehdjk.com/Article/details/gcwninvjx.sHtML

SELECT * FROM (
来源：http://www.share.fktsv.cn/Article/details/glprgbsrn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fktsv.cn/Article/details/gcgxqpoao.sHtML

) t WHERE rn = 1;
来源：http://baike.epnwcf.com/Article/details/gppfhjldz.sHtML

[Q35] 内连接
来源：http://www.blog.sjlbkw.cn/Article/details/gxbvqjjct.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.sjlbkw.cn/Article/details/gtxsjufch.sHtML

[Q36] 左连接
来源：http://www.share.epnwcf.com/Article/details/gimtxcvob.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.epnwcf.com/Article/details/gkootmpsp.sHtML

[Q37] 右连接
来源：http://mobile.epnwcf.com/Article/details/glksuipxz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.bbcook.cn/Article/details/gsxtcavkf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.sjlbkw.cn/Article/details/ghdxmjigu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.bbcook.cn/Article/details/gcnejciyq.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.tarul.cn/Article/details/gezcmifvl.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fktsv.cn/Article/details/goxxaxhci.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.yfazqb.com/Article/details/galexusnc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.bbcook.cn/Article/details/ggokwswda.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fktsv.cn/Article/details/gtvjratvc.sHtML

[Q41] 多表连接
来源：http://baike.sjlbkw.cn/Article/details/gtfmjnejy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.bbcook.cn/Article/details/gcslqgkkj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.yfazqb.com/Article/details/gnozyytle.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.bbcook.cn/Article/details/gkbflsyeg.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.tarul.cn/Article/details/gnatlssrx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.tarul.cn/Article/details/gyjdqosbd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fktsv.cn/Article/details/gtffcinmd.sHtML

[Q43] 标量子查询
来源：http://m.share.vehdjk.com/Article/details/gzxcdfksf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.epnwcf.com/Article/details/giaateieu.sHtML

[Q44] IN 子查询
来源：http://baike.tarul.cn/Article/details/gflpyubzn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.bbcook.cn/Article/details/gvcywpxmi.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.yfazqb.com/Article/details/gcadvgxby.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.sjlbkw.cn/Article/details/gcdirwyyz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.epnwcf.com/Article/details/gmtwjxpaj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.bbcook.cn/Article/details/ghlijjzgo.sHtML

[Q47] 与平均值比较
来源：http://m.share.fktsv.cn/Article/details/gdkwgvzab.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.yfazqb.com/Article/details/gvxbbarbg.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.epnwcf.com/Article/details/gfhyeypmk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.epnwcf.com/Article/details/ghhzanrps.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.sjlbkw.cn/Article/details/gzdsxqckl.sHtML

[Q49] 更新单行
来源：http://baike.bbcook.cn/Article/details/gikifkklc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.bbcook.cn/Article/details/gxokfcxgp.sHtML

[Q50] 批量更新
来源：http://www.m.share.sjlbkw.cn/Article/details/gzhgdtubq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fktsv.cn/Article/details/gecmwygao.sHtML

[Q51] 用子查询更新
来源：http://3g.bbcook.cn/Article/details/gmhatoyvq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.bbcook.cn/Article/details/gfxwszejx.sHtML

[Q52] 删除指定行
来源：http://www.share.fktsv.cn/Article/details/gvwkfnkkp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.sjlbkw.cn/Article/details/gywmpewzc.sHtML

[Q53] 按条件删除
来源：http://www.blog.bbcook.cn/Article/details/gnrfqmffg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.tarul.cn/Article/details/goaicnrbg.sHtML

[Q54] 清空表
来源：http://mobile.epnwcf.com/Article/details/gbzqfgmte.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.vehdjk.com/Article/details/ggbzpptdc.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.tarul.cn/Article/details/gjwodqjym.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fktsv.cn/Article/details/gszljqglr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.bbcook.cn/Article/details/gibigxkxl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.yfazqb.com/Article/details/geqgdpxph.sHtML

[Q57] 行号
来源：http://mobile.vehdjk.com/Article/details/gyuoayorh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gleoctpoz.sHtML

[Q58] 累计求和
来源：http://www.blog.tarul.cn/Article/details/glgdxvqfi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fktsv.cn/Article/details/grntxwxeu.sHtML

[Q59] 分组内累计
来源：http://baike.tarul.cn/Article/details/gxizgqfek.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/gakzqwgog.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.sjlbkw.cn/Article/details/gxosmgvxy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.tarul.cn/Article/details/gauvlzypt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.vehdjk.com/Article/details/gofompysg.sHtML

[Q61] 移动平均
来源：http://www.blog.tarul.cn/Article/details/gpijqpfuq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.yfazqb.com/Article/details/ghkviioqo.sHtML

[Q62] 分组占比
来源：http://www.share.yfazqb.com/Article/details/gucgqhdge.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fktsv.cn/Article/details/ggaptytoz.sHtML

[Q63] 开启事务
来源：http://3g.sjlbkw.cn/Article/details/gnowcadjh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.yfazqb.com/Article/details/grgfgblhe.sHtML

[Q64] 提交事务
来源：http://blog.sjlbkw.cn/Article/details/gmdvglirr.sHtML

COMMIT;
来源：http://www.m.share.sjlbkw.cn/Article/details/gjmryvbcc.sHtML

[Q65] 回滚事务
来源：http://baike.tarul.cn/Article/details/gvnvlbcqa.sHtML

ROLLBACK;
来源：http://read.share.yfazqb.com/Article/details/gdsaugzuz.sHtML

[Q66] 行锁查询
来源：http://www.m.share.sjlbkw.cn/Article/details/gzjmdwmff.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.epnwcf.com/Article/details/gbdgkckej.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.epnwcf.com/Article/details/grgimokqv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.yfazqb.com/Article/details/gujgarkaz.sHtML

[Q68] 保存点
来源：http://www.share.sjlbkw.cn/Article/details/gmtlsfplc.sHtML

SAVEPOINT sp1;
来源：http://3g.yfazqb.com/Article/details/gqvyyucic.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.yfazqb.com/Article/details/gpfvccwkp.sHtML

[Q69] 查看执行计划
来源：http://blog.epnwcf.com/Article/details/gynpuwgos.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.vehdjk.com/Article/details/gafxtxldl.sHtML

[Q70] 更新统计信息
来源：http://baike.fktsv.cn/Article/details/gnyxaimtt.sHtML

ANALYZE TABLE users;
来源：http://blog.yfazqb.com/Article/details/gcnfkvaqo.sHtML

[Q71] 查看建表语句
来源：http://wap.epnwcf.com/Article/details/gyejwohat.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fktsv.cn/Article/details/gmyhptnhb.sHtML

[Q72] 查看索引
来源：http://3g.tarul.cn/Article/details/gxrigzotv.sHtML

SHOW INDEX FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gpggwnmoa.sHtML

[Q73] 查看表状态
来源：http://www.blog.epnwcf.com/Article/details/gyumoumlz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.tarul.cn/Article/details/goopbaock.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fktsv.cn/Article/details/gdvsjyngp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.epnwcf.com/Article/details/gcaemwzvs.sHtML

[Q75] 日期格式化
来源：http://www.blog.epnwcf.com/Article/details/gdtggwfxc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.bbcook.cn/Article/details/gnqtameqy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.tarul.cn/Article/details/gfbalarym.sHtML

[Q76] 按天统计
来源：http://blog.fktsv.cn/Article/details/gmnrcjxua.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.epnwcf.com/Article/details/gtynnnvwp.sHtML

[Q77] 时间加减
来源：http://baike.fktsv.cn/Article/details/gdtbjnxyp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.yfazqb.com/Article/details/gbqnbepwf.sHtML

[Q78] 当前时间
来源：http://www.share.tarul.cn/Article/details/ghrdqhcvj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.tarul.cn/Article/details/ghhpaddbt.sHtML

[Q79] 字符串拼接
来源：http://mobile.bbcook.cn/Article/details/gtmrdjmty.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.sjlbkw.cn/Article/details/gitohhsqk.sHtML

[Q80] 字符串截取
来源：http://www.m.share.sjlbkw.cn/Article/details/gicawiuvm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.epnwcf.com/Article/details/guyhzfcsn.sHtML

[Q81] 字符串替换
来源：http://baike.yfazqb.com/Article/details/gszelkccl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.bbcook.cn/Article/details/gujnehwza.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.bbcook.cn/Article/details/gnrbfuvts.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fktsv.cn/Article/details/grtkrltub.sHtML

[Q83] 大小写转换
来源：http://3g.yfazqb.com/Article/details/gscaqkurj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.bbcook.cn/Article/details/gmlzlxetw.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.sjlbkw.cn/Article/details/ggajfnzso.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.yfazqb.com/Article/details/gbkutcjfa.sHtML

[Q85] 数值取整
来源：http://www.blog.tarul.cn/Article/details/gsjhbjnop.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.tarul.cn/Article/details/gcnvvizuj.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fktsv.cn/Article/details/genlidtvs.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.yfazqb.com/Article/details/glhjgarvr.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.bbcook.cn/Article/details/gmkyuloun.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.bbcook.cn/Article/details/gnisjulaf.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.tarul.cn/Article/details/gbbjnidrs.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.sjlbkw.cn/Article/details/glhognicy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gwsjtwvfi.sHtML

[Q89] 判断表是否存在
来源：http://baike.tarul.cn/Article/details/gywuuwqpc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fktsv.cn/Article/details/gxjonwmug.sHtML

[Q90] 生成序号列
来源：http://www.blog.vehdjk.com/Article/details/gvqixckxx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.vehdjk.com/Article/details/gncgpaawi.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gdyxaexus.sHtML

R. Bash 专题
来源：http://baike.bbcook.cn/Article/details/gggwssobe.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/ghtijlckd.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.epnwcf.com/Article/details/gljwxotoc.sHtML

#!/usr/bin/env bash
来源：http://blog.sjlbkw.cn/Article/details/ggxwlmfox.sHtML

set -euo pipefail
来源：http://read.share.fktsv.cn/Article/details/gapaagnby.sHtML

[R02] 变量赋值与使用
来源：http://www.share.vehdjk.com/Article/details/gbelwxsim.sHtML

name="Tom"; echo "$name"
来源：http://baike.tarul.cn/Article/details/glguqsjcd.sHtML

[R03] 只读变量
来源：http://read.share.tarul.cn/Article/details/guhgnzvgs.sHtML

readonly PI=3.14
来源：http://blog.epnwcf.com/Article/details/gzsajmmen.sHtML

[R04] 位置参数
来源：http://blog.vehdjk.com/Article/details/gzblnrfxr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.bbcook.cn/Article/details/guolmggfa.sHtML

[R05] 参数默认值
来源：http://m.share.sjlbkw.cn/Article/details/gpudvyyun.sHtML

name="${1:-default}"
来源：http://m.share.epnwcf.com/Article/details/guqwqknej.sHtML

[R06] 判断命令是否存在
来源：http://wap.fktsv.cn/Article/details/gimxxfsnk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.epnwcf.com/Article/details/gdxoejorc.sHtML

[R07] if 判断文件
来源：http://blog.epnwcf.com/Article/details/glcumeuls.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.sjlbkw.cn/Article/details/ghdermuef.sHtML

[R08] 数值比较
来源：http://read.share.epnwcf.com/Article/details/gghxbdysw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.vehdjk.com/Article/details/gdkxyeyrf.sHtML

[R09] 字符串比较
来源：http://mobile.epnwcf.com/Article/details/gozzscdxs.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.yfazqb.com/Article/details/gwntpwtqj.sHtML

[R10] 正则匹配
来源：http://www.blog.vehdjk.com/Article/details/glzoptzgt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fktsv.cn/Article/details/gsndemuoy.sHtML

[R11] case 多分支
来源：http://blog.vehdjk.com/Article/details/gpisnvqvv.sHtML

case "$1" in
来源：http://blog.tarul.cn/Article/details/gwvykjxtx.sHtML

start) echo "启动" ;;
来源：http://www.share.sjlbkw.cn/Article/details/geiafwpyi.sHtML

stop)  echo "停止" ;;
来源：http://mobile.yfazqb.com/Article/details/ggkhmjwto.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.bbcook.cn/Article/details/gjczevqax.sHtML

esac
来源：http://read.share.vehdjk.com/Article/details/gvqzhozfw.sHtML

[R12] for 遍历文件
来源：http://baike.vehdjk.com/Article/details/ggmdmiwcd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gtudzjvac.sHtML

[R13] for 计数循环
来源：http://wap.bbcook.cn/Article/details/gedsoislr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gvmgurxgb.sHtML

[R14] C 风格 for
来源：http://3g.vehdjk.com/Article/details/gmtibmqtu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.sjlbkw.cn/Article/details/gwtqshjaz.sHtML

[R15] while 逐行读文件
来源：http://wap.bbcook.cn/Article/details/geniabxyd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.bbcook.cn/Article/details/gojivtpln.sHtML

[R16] until 等待条件
来源：http://baike.bbcook.cn/Article/details/gvinolrsx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.epnwcf.com/Article/details/gdckzuygb.sHtML

[R17] 数组定义与取值
来源：http://read.share.sjlbkw.cn/Article/details/gijoihchf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.yfazqb.com/Article/details/gawqqjtpk.sHtML

[R18] 遍历数组
来源：http://www.blog.yfazqb.com/Article/details/gvgjgpyxx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.tarul.cn/Article/details/gfivvgcgm.sHtML

[R19] 数组长度
来源：http://blog.sjlbkw.cn/Article/details/gyvqveyjd.sHtML

echo "${#arr[@]}"
来源：http://blog.epnwcf.com/Article/details/gxonhiats.sHtML

[R20] 关联数组（字典）
来源：http://wap.yfazqb.com/Article/details/gjatbmdkj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fktsv.cn/Article/details/gzzahyblb.sHtML

[R21] 字符串长度
来源：http://www.share.vehdjk.com/Article/details/geanwohwd.sHtML

echo "${#s}"
来源：http://3g.epnwcf.com/Article/details/gqhpurfpo.sHtML

[R22] 截取子串
来源：http://www.blog.epnwcf.com/Article/details/gytbbwbrn.sHtML

echo "${s:0:5}"
来源：http://3g.tarul.cn/Article/details/geeepgxkz.sHtML

[R23] 字符串替换
来源：http://baike.fktsv.cn/Article/details/guloxkyne.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.yfazqb.com/Article/details/gijqmpvjp.sHtML

[R24] 大小写转换
来源：http://3g.fktsv.cn/Article/details/ghmovitwj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.sjlbkw.cn/Article/details/gqadeskqj.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.tarul.cn/Article/details/gweofbflt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.epnwcf.com/Article/details/gkuqpgsle.sHtML

[R26] 命令替换
来源：http://wap.vehdjk.com/Article/details/gjliprhdg.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.vehdjk.com/Article/details/gngrvrmxm.sHtML

[R27] 算术展开
来源：http://baike.yfazqb.com/Article/details/guzxosrhk.sHtML

echo $((1 + 2 * 3))
来源：http://3g.yfazqb.com/Article/details/guofczrak.sHtML

[R28] 浮点运算
来源：http://www.share.tarul.cn/Article/details/gwtvtnxlq.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.vehdjk.com/Article/details/glneddxcm.sHtML

[R29] 定义函数
来源：http://www.m.share.vehdjk.com/Article/details/gkxbkrham.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.vehdjk.com/Article/details/gywcgpdjn.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fktsv.cn/Article/details/gqivncvvj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.vehdjk.com/Article/details/guzjkhhyq.sHtML

[R31] 局部变量
来源：http://www.blog.yfazqb.com/Article/details/gezvudqfy.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.vehdjk.com/Article/details/gbppxlzmr.sHtML

[R32] 参数个数校验
来源：http://www.share.vehdjk.com/Article/details/guzthqudq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fktsv.cn/Article/details/gwdfzdrvu.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.bbcook.cn/Article/details/gskntgvcz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.vehdjk.com/Article/details/gjsqhtdpx.sHtML

[R34] 退出时清理
来源：http://wap.fktsv.cn/Article/details/goztqezsl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.sjlbkw.cn/Article/details/ghihtokrh.sHtML

[R35] 后台执行并等待
来源：http://www.share.tarul.cn/Article/details/golwoiivo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.yfazqb.com/Article/details/grszdsmfo.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fktsv.cn/Article/details/gkoalzrhu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.tarul.cn/Article/details/gysmxgwbj.sHtML

[R37] 把输出赋给变量
来源：http://3g.bbcook.cn/Article/details/gpqugsuuk.sHtML

files=$(ls -1)
来源：http://blog.vehdjk.com/Article/details/ggiybezgr.sHtML

[R38] 管道串联
来源：http://www.share.tarul.cn/Article/details/gvuoagpam.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.vehdjk.com/Article/details/gpfxlpgsh.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.tarul.cn/Article/details/gxujirxtl.sHtML

cmd > out.log 2>&1
来源：http://3g.yfazqb.com/Article/details/ghegcfako.sHtML

[R40] 追加写日志
来源：http://mobile.vehdjk.com/Article/details/gjmqorkwg.sHtML

echo "log" >> out.log
来源：http://read.share.epnwcf.com/Article/details/ghjscrybj.sHtML

[R41] 丢弃输出
来源：http://read.share.yfazqb.com/Article/details/gpgpacgda.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.sjlbkw.cn/Article/details/gopoujhvg.sHtML

[R42] 输入重定向
来源：http://www.share.epnwcf.com/Article/details/gwrcxiwht.sHtML

wc -l < a.txt
来源：http://mobile.tarul.cn/Article/details/ggsehjbdn.sHtML

[R43] 按名字查找文件
来源：http://3g.yfazqb.com/Article/details/gugagtcsm.sHtML

find . -name "*.log" -type f
来源：http://baike.epnwcf.com/Article/details/gkgjdpfxn.sHtML

[R44] 按修改时间查找
来源：http://www.blog.bbcook.cn/Article/details/gcczqyxhx.sHtML

find . -mtime -7 -type f
来源：http://m.share.fktsv.cn/Article/details/gllalezoq.sHtML

[R45] 批量删除
来源：http://www.m.share.bbcook.cn/Article/details/gyrpfrydx.sHtML

find . -name "*.tmp" -delete
来源：http://blog.vehdjk.com/Article/details/gbscipxai.sHtML

[R46] 递归替换文件内容
来源：http://m.share.bbcook.cn/Article/details/gogrzslir.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fktsv.cn/Article/details/gkzvahmql.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fktsv.cn/Article/details/gajwwhnep.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fktsv.cn/Article/details/gbvinweus.sHtML

[R48] awk 取指定列
来源：http://wap.sjlbkw.cn/Article/details/gfylsmasu.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.bbcook.cn/Article/details/gnxnzhybv.sHtML

[R49] awk 带条件
来源：http://m.share.sjlbkw.cn/Article/details/gbzcmdoqs.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.epnwcf.com/Article/details/gtiqvailk.sHtML

[R50] awk 求和
来源：http://mobile.vehdjk.com/Article/details/gpiwnoavk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.sjlbkw.cn/Article/details/gqnbvgkzu.sHtML

[R51] 排序去重取前几
来源：http://www.share.sjlbkw.cn/Article/details/gaqvgxruq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fktsv.cn/Article/details/gotagxqle.sHtML

[R52] 统计行数
来源：http://www.blog.fktsv.cn/Article/details/gbuiyuxtx.sHtML

wc -l a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gffxkpxir.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.tarul.cn/Article/details/gldsaxbxk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.yfazqb.com/Article/details/gnkvabswr.sHtML

[R54] 比较两个文件
来源：http://mobile.yfazqb.com/Article/details/gbovojggn.sHtML

diff a.txt b.txt
来源：http://baike.tarul.cn/Article/details/gfzzlphev.sHtML

[R55] 压缩与解压
来源：http://baike.bbcook.cn/Article/details/gibqsjafs.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.tarul.cn/Article/details/goihfaftw.sHtML

[R56] 远程拷贝
来源：http://baike.bbcook.cn/Article/details/geleyytgk.sHtML

scp file user@host:/path/
来源：http://read.share.bbcook.cn/Article/details/gmevxhhvx.sHtML

[R57] 远程执行命令
来源：http://www.share.fktsv.cn/Article/details/gvvfblesh.sHtML

ssh user@host 'uptime'
来源：http://www.share.vehdjk.com/Article/details/gidznyxvy.sHtML

[R58] 下载文件
来源：http://3g.bbcook.cn/Article/details/gkqmufaqx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.vehdjk.com/Article/details/ggljlyxfk.sHtML

[R59] 发 POST JSON
来源：http://baike.vehdjk.com/Article/details/gmhfeymzl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.sjlbkw.cn/Article/details/gpfbkovhc.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.yfazqb.com/Article/details/gpiprszak.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.tarul.cn/Article/details/gruvwynam.sHtML

[R61] 磁盘占用
来源：http://wap.bbcook.cn/Article/details/gwqodqbdu.sHtML

df -h;  du -sh *
来源：http://www.blog.bbcook.cn/Article/details/gjnzjddfc.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.yfazqb.com/Article/details/gnalwjnkv.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.sjlbkw.cn/Article/details/gultgxdui.sHtML

[R63] 内存与进程
来源：http://www.blog.yfazqb.com/Article/details/glqhyraig.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.epnwcf.com/Article/details/gfepykbsx.sHtML

[R64] 结束进程
来源：http://blog.yfazqb.com/Article/details/gvfzufdns.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.yfazqb.com/Article/details/ghtltsjhp.sHtML

[R65] 查看端口占用
来源：http://www.share.vehdjk.com/Article/details/gicizxnpj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.yfazqb.com/Article/details/gdktwthys.sHtML

[R66] 定时任务
来源：http://www.m.share.tarul.cn/Article/details/gwrajiuaz.sHtML

crontab -e;  crontab -l
来源：http://baike.vehdjk.com/Article/details/gtavteshv.sHtML

[R67] 生成随机十六进制串
来源：http://blog.epnwcf.com/Article/details/gptfmiyzs.sHtML

openssl rand -hex 16
来源：http://blog.bbcook.cn/Article/details/gfohchunj.sHtML

[R68] 计算文件校验值
来源：http://m.share.sjlbkw.cn/Article/details/gfwzxarfx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.tarul.cn/Article/details/goinvshfx.sHtML

[R69] 生成随机密码
来源：http://www.m.share.yfazqb.com/Article/details/grzsnzcpb.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.tarul.cn/Article/details/gsmxyvjon.sHtML

[R70] 时间戳与互转
来源：http://mobile.bbcook.cn/Article/details/gqiviuvju.sHtML

date +%s;  date -d @1700000000
来源：http://baike.tarul.cn/Article/details/gothrzvdb.sHtML

[R71] 日期格式化
来源：http://3g.epnwcf.com/Article/details/gsdlpnnxd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.bbcook.cn/Article/details/gsntllkzq.sHtML

[R72] 等待端口就绪
来源：http://3g.yfazqb.com/Article/details/gdyijclek.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.bbcook.cn/Article/details/gjpwuhnhu.sHtML

[R73] 分割大日志
来源：http://3g.tarul.cn/Article/details/gxtcogtqi.sHtML

split -l 1000 big.log part_
来源：http://mobile.tarul.cn/Article/details/gxtpzylgw.sHtML

[R74] 批量重命名
来源：http://mobile.epnwcf.com/Article/details/goyavyoyv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.sjlbkw.cn/Article/details/godjowpna.sHtML

[R75] 导出环境变量
来源：http://www.share.fktsv.cn/Article/details/gdoaevrce.sHtML


<!-- 参考信息 -->