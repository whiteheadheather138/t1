代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.epnwcf.com/Article/details/gypkunoig.sHtML

[Q24] 去重
来源：http://wap.tarul.cn/Article/details/ggphcbzde.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fktsv.cn/Article/details/giecagtmc.sHtML

[Q25] 只取前 N 条
来源：http://3g.epnwcf.com/Article/details/gcwyzxlam.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.sjlbkw.cn/Article/details/gbiozbser.sHtML

[Q26] 计数
来源：http://read.share.yfazqb.com/Article/details/gzhehkawl.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gmtzgjels.sHtML

[Q27] 条件计数
来源：http://www.share.bbcook.cn/Article/details/gfxaakdhk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.tarul.cn/Article/details/gkbjbmtaw.sHtML

[Q28] 求和与平均
来源：http://read.share.yfazqb.com/Article/details/gmdfglmop.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.yfazqb.com/Article/details/gkyodzjai.sHtML

[Q29] 最大最小值
来源：http://3g.fktsv.cn/Article/details/gaytdrgcu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.tarul.cn/Article/details/gixkxqjko.sHtML

[Q30] 分组统计
来源：http://baike.sjlbkw.cn/Article/details/gxtpemxqt.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.tarul.cn/Article/details/gvywolchz.sHtML

[Q31] 分组后过滤
来源：http://read.share.bbcook.cn/Article/details/gcrpvcdlj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.sjlbkw.cn/Article/details/ghlppadhb.sHtML

[Q32] 分组拼接字符串
来源：http://baike.bbcook.cn/Article/details/gvpercrad.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fktsv.cn/Article/details/gjcubdvqn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.tarul.cn/Article/details/gcazhweql.sHtML

[Q33] 多列分组
来源：http://www.share.yfazqb.com/Article/details/ggulkofgb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.yfazqb.com/Article/details/gjrykyqrd.sHtML

[Q34] 每组取第一条
来源：http://mobile.sjlbkw.cn/Article/details/gixxkxjzm.sHtML

SELECT * FROM (
来源：http://mobile.fktsv.cn/Article/details/geqbgyhxk.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.tarul.cn/Article/details/gvpiczird.sHtML

) t WHERE rn = 1;
来源：http://www.blog.tarul.cn/Article/details/gswscopow.sHtML

[Q35] 内连接
来源：http://mobile.vehdjk.com/Article/details/gyvvxuvns.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.epnwcf.com/Article/details/glxjdpbnc.sHtML

[Q36] 左连接
来源：http://baike.yfazqb.com/Article/details/gjhbfbqes.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.tarul.cn/Article/details/glvuewogq.sHtML

[Q37] 右连接
来源：http://read.share.epnwcf.com/Article/details/gwyyqqrrn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fktsv.cn/Article/details/gstjqiewm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.yfazqb.com/Article/details/gestriozr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.bbcook.cn/Article/details/gbiximecv.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.tarul.cn/Article/details/gcniqgjde.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.bbcook.cn/Article/details/gapqszwye.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.sjlbkw.cn/Article/details/gmsssrkqq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.tarul.cn/Article/details/ghvzrwonr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fktsv.cn/Article/details/gdaacdywn.sHtML

[Q41] 多表连接
来源：http://wap.sjlbkw.cn/Article/details/glqvwmovi.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.tarul.cn/Article/details/gtenbtrsg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.yfazqb.com/Article/details/geiblnigp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.sjlbkw.cn/Article/details/glpdkwouq.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.vehdjk.com/Article/details/giryinzei.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.tarul.cn/Article/details/gqcpwmkno.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.tarul.cn/Article/details/gulukojyk.sHtML

[Q43] 标量子查询
来源：http://www.share.sjlbkw.cn/Article/details/gcaxyrnew.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.yfazqb.com/Article/details/gfvomialf.sHtML

[Q44] IN 子查询
来源：http://blog.epnwcf.com/Article/details/gargifbug.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.epnwcf.com/Article/details/gjesrkslu.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fktsv.cn/Article/details/grlpwbiqw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.epnwcf.com/Article/details/gviqcwtnx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.bbcook.cn/Article/details/gwsfouzgw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.yfazqb.com/Article/details/gogaanvkk.sHtML

[Q47] 与平均值比较
来源：http://blog.bbcook.cn/Article/details/gjskotlba.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.bbcook.cn/Article/details/gltosjmkv.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.yfazqb.com/Article/details/gzccaqetv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.bbcook.cn/Article/details/ghjfknjof.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.bbcook.cn/Article/details/gdjynuhia.sHtML

[Q49] 更新单行
来源：http://m.share.fktsv.cn/Article/details/gsekjhyun.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.epnwcf.com/Article/details/gyuoswnmd.sHtML

[Q50] 批量更新
来源：http://m.share.yfazqb.com/Article/details/gjrcdevlz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.vehdjk.com/Article/details/guidzqkbm.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fktsv.cn/Article/details/gjcvdtaxc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.vehdjk.com/Article/details/genvpwvcj.sHtML

[Q52] 删除指定行
来源：http://www.share.epnwcf.com/Article/details/gudpasfqp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.tarul.cn/Article/details/gifqapwen.sHtML

[Q53] 按条件删除
来源：http://wap.yfazqb.com/Article/details/ghzlmmgnf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.vehdjk.com/Article/details/gmrltoxtz.sHtML

[Q54] 清空表
来源：http://read.share.epnwcf.com/Article/details/gnwrjigoh.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.epnwcf.com/Article/details/gvlarnbah.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.bbcook.cn/Article/details/guvgfcfxx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.vehdjk.com/Article/details/ghcgetluy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.bbcook.cn/Article/details/gjuxjsmez.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.tarul.cn/Article/details/gykenxcpq.sHtML

[Q57] 行号
来源：http://mobile.yfazqb.com/Article/details/gvmtsrzhi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.vehdjk.com/Article/details/gmqzftadp.sHtML

[Q58] 累计求和
来源：http://baike.fktsv.cn/Article/details/gvseffaox.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.tarul.cn/Article/details/gudpwbnyn.sHtML

[Q59] 分组内累计
来源：http://3g.fktsv.cn/Article/details/glcpjemow.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/gohslhpsl.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.vehdjk.com/Article/details/gsyuocxxo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.epnwcf.com/Article/details/gsficwwjj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/gktlxvhwc.sHtML

[Q61] 移动平均
来源：http://blog.sjlbkw.cn/Article/details/gmqnfzlzh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.yfazqb.com/Article/details/gvyckdixo.sHtML

[Q62] 分组占比
来源：http://3g.yfazqb.com/Article/details/glddokrvt.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.tarul.cn/Article/details/gorcluqvz.sHtML

[Q63] 开启事务
来源：http://read.share.sjlbkw.cn/Article/details/gbnbnvsml.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fktsv.cn/Article/details/ghheyankn.sHtML

[Q64] 提交事务
来源：http://wap.tarul.cn/Article/details/guqxfswfd.sHtML

COMMIT;
来源：http://m.share.vehdjk.com/Article/details/grpxpxsov.sHtML

[Q65] 回滚事务
来源：http://blog.tarul.cn/Article/details/garehjaug.sHtML

ROLLBACK;
来源：http://mobile.vehdjk.com/Article/details/gxjabqmej.sHtML

[Q66] 行锁查询
来源：http://wap.fktsv.cn/Article/details/gzioalvyb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.bbcook.cn/Article/details/gqrteijrg.sHtML

[Q67] 设置隔离级别
来源：http://read.share.epnwcf.com/Article/details/ghnamhllj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.yfazqb.com/Article/details/gnjsgolji.sHtML

[Q68] 保存点
来源：http://read.share.sjlbkw.cn/Article/details/gkdeevknz.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.vehdjk.com/Article/details/gzuggtzby.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.vehdjk.com/Article/details/gnjbzltsb.sHtML

[Q69] 查看执行计划
来源：http://3g.epnwcf.com/Article/details/ghvfqyehh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.yfazqb.com/Article/details/gscqzzetl.sHtML

[Q70] 更新统计信息
来源：http://baike.tarul.cn/Article/details/gayksmsld.sHtML

ANALYZE TABLE users;
来源：http://mobile.fktsv.cn/Article/details/grlzvenbt.sHtML

[Q71] 查看建表语句
来源：http://www.share.yfazqb.com/Article/details/gcsyzpwyd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.vehdjk.com/Article/details/gvxgmogbj.sHtML

[Q72] 查看索引
来源：http://mobile.bbcook.cn/Article/details/ggblipoyr.sHtML

SHOW INDEX FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gujcqlyjy.sHtML

[Q73] 查看表状态
来源：http://wap.bbcook.cn/Article/details/gmxtnvhgv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.tarul.cn/Article/details/gscfghkxv.sHtML

[Q74] 强制使用索引
来源：http://3g.yfazqb.com/Article/details/glzdeqowy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fktsv.cn/Article/details/gopqyikbh.sHtML

[Q75] 日期格式化
来源：http://blog.bbcook.cn/Article/details/gpgyrlatp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.epnwcf.com/Article/details/gbhdgovwc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.epnwcf.com/Article/details/gjoamwobw.sHtML

[Q76] 按天统计
来源：http://baike.fktsv.cn/Article/details/gwffeospl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.tarul.cn/Article/details/goyiorxjb.sHtML

[Q77] 时间加减
来源：http://read.share.yfazqb.com/Article/details/gycieaaaj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.epnwcf.com/Article/details/golhtticu.sHtML

[Q78] 当前时间
来源：http://3g.epnwcf.com/Article/details/gfjtbgqvw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.bbcook.cn/Article/details/gctmiyhtu.sHtML

[Q79] 字符串拼接
来源：http://blog.fktsv.cn/Article/details/ggfzajdkj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fktsv.cn/Article/details/gfpddmfsu.sHtML

[Q80] 字符串截取
来源：http://www.m.share.vehdjk.com/Article/details/gymnmbwdp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gccinnjez.sHtML

[Q81] 字符串替换
来源：http://www.blog.sjlbkw.cn/Article/details/gxjjrahni.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gyrxnldyq.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.epnwcf.com/Article/details/gukzuscut.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.tarul.cn/Article/details/ggdbppwjc.sHtML

[Q83] 大小写转换
来源：http://read.share.fktsv.cn/Article/details/gvlfnekxm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.tarul.cn/Article/details/gnqcqbhkd.sHtML

[Q84] 去除首尾空格
来源：http://blog.epnwcf.com/Article/details/gcgbsiilg.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.vehdjk.com/Article/details/gtakqasjg.sHtML

[Q85] 数值取整
来源：http://baike.tarul.cn/Article/details/gfrflvaoc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.sjlbkw.cn/Article/details/gibemgvmn.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.yfazqb.com/Article/details/gzvrvzaml.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.sjlbkw.cn/Article/details/geozqgsed.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.yfazqb.com/Article/details/gbikvtgni.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fktsv.cn/Article/details/gbwiujahg.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.epnwcf.com/Article/details/gjzyfwjvi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.tarul.cn/Article/details/gggukenyl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.yfazqb.com/Article/details/ghusczaqe.sHtML

[Q89] 判断表是否存在
来源：http://mobile.yfazqb.com/Article/details/grauqzkmc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.yfazqb.com/Article/details/ghafziwfh.sHtML

[Q90] 生成序号列
来源：http://m.share.yfazqb.com/Article/details/gilsubdqz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.bbcook.cn/Article/details/ggyxmynoy.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/glgdjffnv.sHtML

R. Bash 专题
来源：http://baike.bbcook.cn/Article/details/gcnhgemgy.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gpuiqzbpf.sHtML

[R01] shebang 与严格模式
来源：http://mobile.tarul.cn/Article/details/ggyhevfmw.sHtML

#!/usr/bin/env bash
来源：http://blog.fktsv.cn/Article/details/gtkkncdkg.sHtML

set -euo pipefail
来源：http://m.share.tarul.cn/Article/details/gylkewvik.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fktsv.cn/Article/details/gjlgyyanj.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.vehdjk.com/Article/details/gneuoucel.sHtML

[R03] 只读变量
来源：http://baike.epnwcf.com/Article/details/glccxmivy.sHtML

readonly PI=3.14
来源：http://mobile.epnwcf.com/Article/details/ghkbhfnej.sHtML

[R04] 位置参数
来源：http://m.share.sjlbkw.cn/Article/details/grtsfbxxo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.epnwcf.com/Article/details/grkclmpbe.sHtML

[R05] 参数默认值
来源：http://www.share.epnwcf.com/Article/details/gdyrfseri.sHtML

name="${1:-default}"
来源：http://mobile.bbcook.cn/Article/details/gyvghkiuo.sHtML

[R06] 判断命令是否存在
来源：http://blog.yfazqb.com/Article/details/gqaqpcyjo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.tarul.cn/Article/details/giqmmdlkn.sHtML

[R07] if 判断文件
来源：http://mobile.bbcook.cn/Article/details/gmtzrqoai.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.vehdjk.com/Article/details/gkyhdsiqp.sHtML

[R08] 数值比较
来源：http://wap.epnwcf.com/Article/details/gneqgumcy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.epnwcf.com/Article/details/gfgnvtnre.sHtML

[R09] 字符串比较
来源：http://wap.tarul.cn/Article/details/gtwmxpmmp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.epnwcf.com/Article/details/gjlvrygzq.sHtML

[R10] 正则匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/gkmzsnxbw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fktsv.cn/Article/details/gzsnrzyob.sHtML

[R11] case 多分支
来源：http://www.blog.vehdjk.com/Article/details/guscdunuw.sHtML

case "$1" in
来源：http://mobile.sjlbkw.cn/Article/details/gtbprrlww.sHtML

start) echo "启动" ;;
来源：http://mobile.fktsv.cn/Article/details/gulpfpgrg.sHtML

stop)  echo "停止" ;;
来源：http://baike.epnwcf.com/Article/details/ghbhrajul.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.sjlbkw.cn/Article/details/gpwahfzhh.sHtML

esac
来源：http://m.share.epnwcf.com/Article/details/gqpwjjzvu.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fktsv.cn/Article/details/ghespgmpb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fktsv.cn/Article/details/gtvntlakx.sHtML

[R13] for 计数循环
来源：http://wap.bbcook.cn/Article/details/gamsybklq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.epnwcf.com/Article/details/gznanspmf.sHtML

[R14] C 风格 for
来源：http://www.share.yfazqb.com/Article/details/geqhuvjdk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.sjlbkw.cn/Article/details/guwxzecfg.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.yfazqb.com/Article/details/gllhguvzi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fktsv.cn/Article/details/gtibwigwp.sHtML

[R16] until 等待条件
来源：http://m.share.yfazqb.com/Article/details/gqinvsams.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fktsv.cn/Article/details/gnlpxrtfz.sHtML

[R17] 数组定义与取值
来源：http://www.blog.tarul.cn/Article/details/gxltzydbg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.yfazqb.com/Article/details/gntbkcgsa.sHtML

[R18] 遍历数组
来源：http://mobile.sjlbkw.cn/Article/details/ghmuzjpyv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.sjlbkw.cn/Article/details/grrxtkvyp.sHtML

[R19] 数组长度
来源：http://3g.tarul.cn/Article/details/ghjkakjgq.sHtML

echo "${#arr[@]}"
来源：http://blog.yfazqb.com/Article/details/glzalwqaf.sHtML

[R20] 关联数组（字典）
来源：http://wap.yfazqb.com/Article/details/girwpnvvn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fktsv.cn/Article/details/glrpmgalm.sHtML

[R21] 字符串长度
来源：http://baike.vehdjk.com/Article/details/gfyjpxpbj.sHtML

echo "${#s}"
来源：http://read.share.yfazqb.com/Article/details/ggwshcpac.sHtML

[R22] 截取子串
来源：http://www.blog.bbcook.cn/Article/details/gqomnhmsp.sHtML

echo "${s:0:5}"
来源：http://3g.yfazqb.com/Article/details/gcfkdmeqw.sHtML

[R23] 字符串替换
来源：http://blog.sjlbkw.cn/Article/details/gpbmdkufv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.sjlbkw.cn/Article/details/gtfiqwtos.sHtML

[R24] 大小写转换
来源：http://3g.epnwcf.com/Article/details/guvqnarnr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.epnwcf.com/Article/details/gulbschdc.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fktsv.cn/Article/details/gcjpjkfdw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.yfazqb.com/Article/details/gdtjqkjtr.sHtML

[R26] 命令替换
来源：http://m.share.tarul.cn/Article/details/gtadtropp.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.bbcook.cn/Article/details/ggalwmewo.sHtML

[R27] 算术展开
来源：http://www.blog.yfazqb.com/Article/details/gvcyakmsz.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.epnwcf.com/Article/details/gxyhixyjm.sHtML

[R28] 浮点运算
来源：http://www.blog.vehdjk.com/Article/details/glzwxmlyg.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.tarul.cn/Article/details/gqaygzcwy.sHtML

[R29] 定义函数
来源：http://3g.vehdjk.com/Article/details/ggtkupkty.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.bbcook.cn/Article/details/gywbjenll.sHtML

[R30] 函数返回状态码
来源：http://blog.vehdjk.com/Article/details/gssqkuenk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.vehdjk.com/Article/details/gvzgssost.sHtML

[R31] 局部变量
来源：http://m.share.fktsv.cn/Article/details/giuvqvubn.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.epnwcf.com/Article/details/gzcnkoxda.sHtML

[R32] 参数个数校验
来源：http://3g.fktsv.cn/Article/details/gntfljail.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.epnwcf.com/Article/details/gqodhiqrs.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.yfazqb.com/Article/details/gpypdajgb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.tarul.cn/Article/details/gfpvzbucg.sHtML

[R34] 退出时清理
来源：http://3g.yfazqb.com/Article/details/gttihybou.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.tarul.cn/Article/details/gacbfyotc.sHtML

[R35] 后台执行并等待
来源：http://m.share.bbcook.cn/Article/details/gvffkaeco.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fktsv.cn/Article/details/gbkeustwj.sHtML

[R36] 并发执行多个任务
来源：http://baike.tarul.cn/Article/details/gqopqspbq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.bbcook.cn/Article/details/gayyyuyay.sHtML

[R37] 把输出赋给变量
来源：http://www.share.epnwcf.com/Article/details/glojkyazf.sHtML

files=$(ls -1)
来源：http://read.share.tarul.cn/Article/details/gdzupmott.sHtML

[R38] 管道串联
来源：http://www.blog.tarul.cn/Article/details/gyoaxrdsu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.tarul.cn/Article/details/gyymfkjfh.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.vehdjk.com/Article/details/gdahavrkx.sHtML

cmd > out.log 2>&1
来源：http://www.blog.sjlbkw.cn/Article/details/gazyezxqi.sHtML

[R40] 追加写日志
来源：http://blog.epnwcf.com/Article/details/gzivxopvd.sHtML

echo "log" >> out.log
来源：http://read.share.tarul.cn/Article/details/gjrhgdcct.sHtML

[R41] 丢弃输出
来源：http://m.share.vehdjk.com/Article/details/ghstgciqz.sHtML

cmd >/dev/null 2>&1
来源：http://baike.tarul.cn/Article/details/gsaomrkmp.sHtML

[R42] 输入重定向
来源：http://www.share.fktsv.cn/Article/details/gjrqpbfaa.sHtML

wc -l < a.txt
来源：http://baike.fktsv.cn/Article/details/gxlgxozzm.sHtML

[R43] 按名字查找文件
来源：http://3g.epnwcf.com/Article/details/gppufhyxs.sHtML

find . -name "*.log" -type f
来源：http://read.share.fktsv.cn/Article/details/gnepozbfk.sHtML

[R44] 按修改时间查找
来源：http://blog.fktsv.cn/Article/details/gtpzekeog.sHtML

find . -mtime -7 -type f
来源：http://mobile.tarul.cn/Article/details/ghnvoalxe.sHtML

[R45] 批量删除
来源：http://www.blog.sjlbkw.cn/Article/details/gfpoabbsq.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.vehdjk.com/Article/details/gqowzhrly.sHtML

[R46] 递归替换文件内容
来源：http://read.share.yfazqb.com/Article/details/gdmrliflb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.vehdjk.com/Article/details/gsmqbptzo.sHtML

[R47] sed 单行替换
来源：http://wap.vehdjk.com/Article/details/gqncdwozt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.epnwcf.com/Article/details/gfjbajffp.sHtML

[R48] awk 取指定列
来源：http://mobile.tarul.cn/Article/details/gutoobjsp.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.tarul.cn/Article/details/gmzwehpso.sHtML

[R49] awk 带条件
来源：http://3g.bbcook.cn/Article/details/gunffgcdo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.yfazqb.com/Article/details/gswcplzzw.sHtML

[R50] awk 求和
来源：http://wap.yfazqb.com/Article/details/gxaxpwmkn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.sjlbkw.cn/Article/details/gfbhagerd.sHtML

[R51] 排序去重取前几
来源：http://mobile.tarul.cn/Article/details/gnjyupewg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.epnwcf.com/Article/details/gvwubxzhy.sHtML

[R52] 统计行数
来源：http://m.share.bbcook.cn/Article/details/gscburjgn.sHtML

wc -l a.txt
来源：http://m.share.sjlbkw.cn/Article/details/gssooktfm.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.tarul.cn/Article/details/gcesbtjpb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.yfazqb.com/Article/details/gavmkfwkd.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fktsv.cn/Article/details/gctmzxilp.sHtML

diff a.txt b.txt
来源：http://www.share.epnwcf.com/Article/details/gwjudzkgg.sHtML

[R55] 压缩与解压
来源：http://wap.tarul.cn/Article/details/gjiolfilb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.tarul.cn/Article/details/gmlxiirdb.sHtML

[R56] 远程拷贝
来源：http://www.blog.fktsv.cn/Article/details/grdqpocgk.sHtML

scp file user@host:/path/
来源：http://blog.fktsv.cn/Article/details/gubbqkjka.sHtML

[R57] 远程执行命令
来源：http://blog.fktsv.cn/Article/details/gmqgopcnh.sHtML

ssh user@host 'uptime'
来源：http://baike.bbcook.cn/Article/details/grwrzwclk.sHtML

[R58] 下载文件
来源：http://blog.yfazqb.com/Article/details/gdghlloiy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.yfazqb.com/Article/details/gprzpcjvk.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fktsv.cn/Article/details/gmspbggos.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.bbcook.cn/Article/details/gsflulmyv.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.vehdjk.com/Article/details/gxjbrwoso.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.vehdjk.com/Article/details/gkzmkrkzr.sHtML

[R61] 磁盘占用
来源：http://mobile.bbcook.cn/Article/details/gzzldrpiz.sHtML

df -h;  du -sh *
来源：http://www.m.share.bbcook.cn/Article/details/gezmaixlw.sHtML

[R62] 找最占空间的文件
来源：http://3g.fktsv.cn/Article/details/gdyzonhbd.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.bbcook.cn/Article/details/gtuevgltq.sHtML

[R63] 内存与进程
来源：http://blog.sjlbkw.cn/Article/details/gfafbzcqr.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.sjlbkw.cn/Article/details/gywbfaqtp.sHtML

[R64] 结束进程
来源：http://www.m.share.vehdjk.com/Article/details/grjjpfhsb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.epnwcf.com/Article/details/ggovhiuff.sHtML

[R65] 查看端口占用
来源：http://3g.bbcook.cn/Article/details/gvrfemglz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fktsv.cn/Article/details/gcegpmjtf.sHtML

[R66] 定时任务
来源：http://read.share.epnwcf.com/Article/details/ghjqgpcph.sHtML

crontab -e;  crontab -l
来源：http://3g.yfazqb.com/Article/details/gltyocszf.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.yfazqb.com/Article/details/gxtmwzcxr.sHtML

openssl rand -hex 16
来源：http://www.m.share.bbcook.cn/Article/details/gfyndrios.sHtML

[R68] 计算文件校验值
来源：http://www.blog.yfazqb.com/Article/details/gsxyvblwf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.vehdjk.com/Article/details/gdruyrxcy.sHtML

[R69] 生成随机密码
来源：http://www.blog.sjlbkw.cn/Article/details/gkxwjvvtd.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.tarul.cn/Article/details/grdbqlmgj.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fktsv.cn/Article/details/gdjhzdqsh.sHtML

date +%s;  date -d @1700000000
来源：http://baike.bbcook.cn/Article/details/grllejdbj.sHtML

[R71] 日期格式化
来源：http://wap.tarul.cn/Article/details/gsiljwryt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fktsv.cn/Article/details/gklfhwlsl.sHtML

[R72] 等待端口就绪
来源：http://3g.fktsv.cn/Article/details/gjckhvaqt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.epnwcf.com/Article/details/gnxkqihkh.sHtML

[R73] 分割大日志
来源：http://www.share.tarul.cn/Article/details/gncgrhcik.sHtML


<!-- 参考信息 -->