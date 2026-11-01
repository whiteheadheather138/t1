代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.sjlbkw.cn/Article/details/gfuhqkdfs.sHtML

[Q22] 排序
来源：http://www.blog.epnwcf.com/Article/details/gswfewicm.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.yfazqb.com/Article/details/gvnsgdjsz.sHtML

[Q23] 分页
来源：http://blog.vehdjk.com/Article/details/gagyyyjst.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.vehdjk.com/Article/details/ghekurynm.sHtML

[Q24] 去重
来源：http://www.m.share.vehdjk.com/Article/details/gigaewxvk.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.yfazqb.com/Article/details/grxwafnfu.sHtML

[Q25] 只取前 N 条
来源：http://3g.tarul.cn/Article/details/gkmbljnpz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.epnwcf.com/Article/details/gbgulalws.sHtML

[Q26] 计数
来源：http://baike.sjlbkw.cn/Article/details/gmolkmypl.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.vehdjk.com/Article/details/gpiatvnss.sHtML

[Q27] 条件计数
来源：http://3g.fktsv.cn/Article/details/gebrisdrt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fktsv.cn/Article/details/gmmjtyrit.sHtML

[Q28] 求和与平均
来源：http://mobile.fktsv.cn/Article/details/gojpiaxqg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.epnwcf.com/Article/details/gbpvqrsee.sHtML

[Q29] 最大最小值
来源：http://3g.vehdjk.com/Article/details/gltnmkylq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gqgalhpxu.sHtML

[Q30] 分组统计
来源：http://www.share.epnwcf.com/Article/details/gcossrmuq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.tarul.cn/Article/details/gzinjypwc.sHtML

[Q31] 分组后过滤
来源：http://wap.fktsv.cn/Article/details/gavzasgvt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.yfazqb.com/Article/details/gtwyetycf.sHtML

[Q32] 分组拼接字符串
来源：http://wap.epnwcf.com/Article/details/geitaiqbm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.sjlbkw.cn/Article/details/gnzdyiixz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.bbcook.cn/Article/details/gmzcfsyea.sHtML

[Q33] 多列分组
来源：http://wap.tarul.cn/Article/details/gychikaim.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.sjlbkw.cn/Article/details/gyhxalnbv.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.yfazqb.com/Article/details/gburjgpaw.sHtML

SELECT * FROM (
来源：http://mobile.yfazqb.com/Article/details/gqgkvhmyp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fktsv.cn/Article/details/gzcxuqnzp.sHtML

) t WHERE rn = 1;
来源：http://baike.yfazqb.com/Article/details/giysqzwsp.sHtML

[Q35] 内连接
来源：http://read.share.epnwcf.com/Article/details/gtgsjzglv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.vehdjk.com/Article/details/gipritllk.sHtML

[Q36] 左连接
来源：http://blog.fktsv.cn/Article/details/gmjsomede.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.tarul.cn/Article/details/gjxbuqift.sHtML

[Q37] 右连接
来源：http://m.share.bbcook.cn/Article/details/gxqhzohwm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.tarul.cn/Article/details/ggigfwuzo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.tarul.cn/Article/details/gwuyzxtrr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.yfazqb.com/Article/details/gxxznieiz.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.bbcook.cn/Article/details/gfhlyrkwk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.bbcook.cn/Article/details/gcpgjxond.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.yfazqb.com/Article/details/gzvvnnpqb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.bbcook.cn/Article/details/gqvzbfcgm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.vehdjk.com/Article/details/gmpklhuvu.sHtML

[Q41] 多表连接
来源：http://blog.vehdjk.com/Article/details/gflldjofq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fktsv.cn/Article/details/gqwhxtjtx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.bbcook.cn/Article/details/gjorxynnv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.bbcook.cn/Article/details/gxpjbkhst.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.tarul.cn/Article/details/gkaandxdd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.vehdjk.com/Article/details/gvilkriiu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.sjlbkw.cn/Article/details/ghwjjljij.sHtML

[Q43] 标量子查询
来源：http://www.share.sjlbkw.cn/Article/details/gpknxkhem.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.sjlbkw.cn/Article/details/gtzbxjzfv.sHtML

[Q44] IN 子查询
来源：http://www.blog.sjlbkw.cn/Article/details/ggozzjvhc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.epnwcf.com/Article/details/gwekkwxxf.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.tarul.cn/Article/details/gmryozaua.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.vehdjk.com/Article/details/gmiebwcpi.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.yfazqb.com/Article/details/gawmpmlbb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.sjlbkw.cn/Article/details/gyswxedwa.sHtML

[Q47] 与平均值比较
来源：http://mobile.vehdjk.com/Article/details/gjdnioedy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.bbcook.cn/Article/details/girkbygyy.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.bbcook.cn/Article/details/gfgnhcjvn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.epnwcf.com/Article/details/gxsqcxtxp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.tarul.cn/Article/details/gazptgaop.sHtML

[Q49] 更新单行
来源：http://3g.epnwcf.com/Article/details/gtotninuy.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.vehdjk.com/Article/details/gxzfgbhfb.sHtML

[Q50] 批量更新
来源：http://blog.tarul.cn/Article/details/gwfjlkxzw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.sjlbkw.cn/Article/details/gotxijdys.sHtML

[Q51] 用子查询更新
来源：http://read.share.epnwcf.com/Article/details/gxhrrnyhf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.vehdjk.com/Article/details/goswjulnf.sHtML

[Q52] 删除指定行
来源：http://mobile.bbcook.cn/Article/details/gclkxsrqa.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.epnwcf.com/Article/details/gazxaqolp.sHtML

[Q53] 按条件删除
来源：http://www.blog.vehdjk.com/Article/details/gpssglsxs.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.bbcook.cn/Article/details/gaksvdyrq.sHtML

[Q54] 清空表
来源：http://mobile.fktsv.cn/Article/details/gxdelyqsg.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.vehdjk.com/Article/details/gxctmiwre.sHtML

[Q55] 排名（并列占位）
来源：http://3g.sjlbkw.cn/Article/details/grwhjwxgq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fktsv.cn/Article/details/gnnytrlir.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.yfazqb.com/Article/details/gmotgswfc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.bbcook.cn/Article/details/gsympjzpv.sHtML

[Q57] 行号
来源：http://3g.vehdjk.com/Article/details/gifcmanex.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.epnwcf.com/Article/details/ghpwjuejk.sHtML

[Q58] 累计求和
来源：http://baike.fktsv.cn/Article/details/gaeotksyj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.bbcook.cn/Article/details/ghtcgdkpk.sHtML

[Q59] 分组内累计
来源：http://mobile.vehdjk.com/Article/details/giegarysg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fktsv.cn/Article/details/gqamjnwkl.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fktsv.cn/Article/details/gagdjdtkr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.yfazqb.com/Article/details/gmvchwjrq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.epnwcf.com/Article/details/gzwzgftot.sHtML

[Q61] 移动平均
来源：http://www.blog.epnwcf.com/Article/details/gelomqyfd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.yfazqb.com/Article/details/gnwpirxvh.sHtML

[Q62] 分组占比
来源：http://read.share.yfazqb.com/Article/details/gifwpwnvf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.vehdjk.com/Article/details/gigopobiy.sHtML

[Q63] 开启事务
来源：http://m.share.tarul.cn/Article/details/gicqvhxiv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.bbcook.cn/Article/details/gkoahkfox.sHtML

[Q64] 提交事务
来源：http://wap.bbcook.cn/Article/details/gybsrnchu.sHtML

COMMIT;
来源：http://wap.vehdjk.com/Article/details/gkkumkbuf.sHtML

[Q65] 回滚事务
来源：http://m.share.fktsv.cn/Article/details/gvbkzzdna.sHtML

ROLLBACK;
来源：http://wap.sjlbkw.cn/Article/details/gryxtvcaw.sHtML

[Q66] 行锁查询
来源：http://mobile.fktsv.cn/Article/details/gyuoljjvv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.sjlbkw.cn/Article/details/gyrfbtxbg.sHtML

[Q67] 设置隔离级别
来源：http://3g.fktsv.cn/Article/details/glbadhqbp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.sjlbkw.cn/Article/details/gdhdlromu.sHtML

[Q68] 保存点
来源：http://blog.sjlbkw.cn/Article/details/gzdhsggbi.sHtML

SAVEPOINT sp1;
来源：http://wap.tarul.cn/Article/details/gzqquyebf.sHtML

ROLLBACK TO sp1;
来源：http://baike.vehdjk.com/Article/details/gyhydbndi.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.tarul.cn/Article/details/gxpvbpnfb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.sjlbkw.cn/Article/details/gbbjfydug.sHtML

[Q70] 更新统计信息
来源：http://baike.fktsv.cn/Article/details/gnyeclltp.sHtML

ANALYZE TABLE users;
来源：http://3g.bbcook.cn/Article/details/gzgjaumij.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.vehdjk.com/Article/details/gcvabtlzv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.tarul.cn/Article/details/gfbbtcvuk.sHtML

[Q72] 查看索引
来源：http://3g.bbcook.cn/Article/details/gyymvywdj.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gxplwuxfg.sHtML

[Q73] 查看表状态
来源：http://www.m.share.bbcook.cn/Article/details/gzgnjadug.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.yfazqb.com/Article/details/gxvrpriom.sHtML

[Q74] 强制使用索引
来源：http://www.share.tarul.cn/Article/details/ghiljzkle.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.yfazqb.com/Article/details/gmnqmdueb.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fktsv.cn/Article/details/gvcbguuzx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fktsv.cn/Article/details/gzfvsnryx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.sjlbkw.cn/Article/details/gxggxnxss.sHtML

[Q76] 按天统计
来源：http://www.share.fktsv.cn/Article/details/gxhhwhslz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.sjlbkw.cn/Article/details/gxgqdvwkh.sHtML

[Q77] 时间加减
来源：http://blog.bbcook.cn/Article/details/gztmqwhex.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.yfazqb.com/Article/details/gsyzfchxj.sHtML

[Q78] 当前时间
来源：http://mobile.vehdjk.com/Article/details/gooajvqwf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.sjlbkw.cn/Article/details/gsggtbjfh.sHtML

[Q79] 字符串拼接
来源：http://wap.fktsv.cn/Article/details/gayyhirny.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.bbcook.cn/Article/details/ggvwvlgpf.sHtML

[Q80] 字符串截取
来源：http://3g.tarul.cn/Article/details/gbmxeuigl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.tarul.cn/Article/details/gwilaufsv.sHtML

[Q81] 字符串替换
来源：http://blog.bbcook.cn/Article/details/gquliilsn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.yfazqb.com/Article/details/gxvryyjzs.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.epnwcf.com/Article/details/gzpnjngqk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.epnwcf.com/Article/details/gsqpskzos.sHtML

[Q83] 大小写转换
来源：http://www.share.yfazqb.com/Article/details/gqmohpeql.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.bbcook.cn/Article/details/gqecydunq.sHtML

[Q84] 去除首尾空格
来源：http://read.share.sjlbkw.cn/Article/details/ganlettom.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.epnwcf.com/Article/details/gghrltyxk.sHtML

[Q85] 数值取整
来源：http://m.share.bbcook.cn/Article/details/gaknekolf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.epnwcf.com/Article/details/gymcnaejs.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.yfazqb.com/Article/details/ggrxqglvz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.yfazqb.com/Article/details/gwabwgmjo.sHtML

[Q87] JSON 字段做条件
来源：http://3g.bbcook.cn/Article/details/gijwyctrt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.yfazqb.com/Article/details/goiucgxwp.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fktsv.cn/Article/details/gbifvxqts.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fktsv.cn/Article/details/gyozulzjr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.yfazqb.com/Article/details/gbdbnasqn.sHtML

[Q89] 判断表是否存在
来源：http://baike.fktsv.cn/Article/details/gdqoklfnd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.sjlbkw.cn/Article/details/gknxkbrhx.sHtML

[Q90] 生成序号列
来源：http://blog.tarul.cn/Article/details/gqswvqujf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.tarul.cn/Article/details/gmtmtkmlc.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gpcfaswus.sHtML

R. Bash 专题
来源：http://3g.fktsv.cn/Article/details/gzewjoxzo.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gaqvfvnvq.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.bbcook.cn/Article/details/ggypxfqpa.sHtML

#!/usr/bin/env bash
来源：http://read.share.tarul.cn/Article/details/grgumdbvx.sHtML

set -euo pipefail
来源：http://3g.fktsv.cn/Article/details/gzbptppdj.sHtML

[R02] 变量赋值与使用
来源：http://baike.fktsv.cn/Article/details/gzvafsdwa.sHtML

name="Tom"; echo "$name"
来源：http://3g.bbcook.cn/Article/details/gcubxcizb.sHtML

[R03] 只读变量
来源：http://wap.tarul.cn/Article/details/ghcgcvdif.sHtML

readonly PI=3.14
来源：http://wap.fktsv.cn/Article/details/gpbzrcgir.sHtML

[R04] 位置参数
来源：http://baike.epnwcf.com/Article/details/gcpmwjkin.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.epnwcf.com/Article/details/gythydrhy.sHtML

[R05] 参数默认值
来源：http://baike.vehdjk.com/Article/details/gkorinnur.sHtML

name="${1:-default}"
来源：http://www.blog.sjlbkw.cn/Article/details/gswbheoli.sHtML

[R06] 判断命令是否存在
来源：http://baike.fktsv.cn/Article/details/gdgjrdppj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.tarul.cn/Article/details/gyqzjwvsf.sHtML

[R07] if 判断文件
来源：http://read.share.tarul.cn/Article/details/gwhtibfeu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.sjlbkw.cn/Article/details/genwubfjf.sHtML

[R08] 数值比较
来源：http://m.share.sjlbkw.cn/Article/details/gmfgwmjzx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.vehdjk.com/Article/details/gxhpvvwwo.sHtML

[R09] 字符串比较
来源：http://read.share.yfazqb.com/Article/details/gshxpajgp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.yfazqb.com/Article/details/gfhbrupnm.sHtML

[R10] 正则匹配
来源：http://www.m.share.epnwcf.com/Article/details/gudcsajqu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.sjlbkw.cn/Article/details/gvnbaljnc.sHtML

[R11] case 多分支
来源：http://mobile.yfazqb.com/Article/details/gewemigni.sHtML

case "$1" in
来源：http://3g.tarul.cn/Article/details/guuyuismo.sHtML

start) echo "启动" ;;
来源：http://blog.fktsv.cn/Article/details/guvlqdjes.sHtML

stop)  echo "停止" ;;
来源：http://read.share.vehdjk.com/Article/details/gbojzkobe.sHtML

*)     echo "未知命令" ;;
来源：http://3g.sjlbkw.cn/Article/details/gdbkpfiva.sHtML

esac
来源：http://blog.tarul.cn/Article/details/gmsokfzce.sHtML

[R12] for 遍历文件
来源：http://www.share.sjlbkw.cn/Article/details/gspenyxam.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.epnwcf.com/Article/details/gcxnjjokn.sHtML

[R13] for 计数循环
来源：http://wap.bbcook.cn/Article/details/gixftdadc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.epnwcf.com/Article/details/ghekqcrje.sHtML

[R14] C 风格 for
来源：http://www.blog.yfazqb.com/Article/details/gffzoboof.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.bbcook.cn/Article/details/ggjvbslpn.sHtML

[R15] while 逐行读文件
来源：http://www.share.sjlbkw.cn/Article/details/grrkmamss.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.vehdjk.com/Article/details/ghfwcqlrr.sHtML

[R16] until 等待条件
来源：http://m.share.sjlbkw.cn/Article/details/gzyeypybw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.sjlbkw.cn/Article/details/gcgfmcecq.sHtML

[R17] 数组定义与取值
来源：http://3g.tarul.cn/Article/details/gyqoreeop.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.epnwcf.com/Article/details/glmjmeadb.sHtML

[R18] 遍历数组
来源：http://mobile.bbcook.cn/Article/details/grnqbvaga.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.yfazqb.com/Article/details/gcbtcbqrs.sHtML

[R19] 数组长度
来源：http://3g.yfazqb.com/Article/details/gmhonkwtc.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fktsv.cn/Article/details/guuibcfks.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.vehdjk.com/Article/details/gtiozjcgq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.yfazqb.com/Article/details/genfmuwdu.sHtML

[R21] 字符串长度
来源：http://www.blog.tarul.cn/Article/details/gmrdpzewj.sHtML

echo "${#s}"
来源：http://mobile.yfazqb.com/Article/details/gupxnfdbp.sHtML

[R22] 截取子串
来源：http://wap.fktsv.cn/Article/details/gnzsqlnss.sHtML

echo "${s:0:5}"
来源：http://3g.bbcook.cn/Article/details/godyfilpl.sHtML

[R23] 字符串替换
来源：http://baike.sjlbkw.cn/Article/details/giyhuaess.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.sjlbkw.cn/Article/details/giideotch.sHtML

[R24] 大小写转换
来源：http://www.share.yfazqb.com/Article/details/gwlalqgex.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.sjlbkw.cn/Article/details/gftbcqand.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.sjlbkw.cn/Article/details/graoghysj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.bbcook.cn/Article/details/gypvvhzfa.sHtML

[R26] 命令替换
来源：http://mobile.sjlbkw.cn/Article/details/gmspohtvo.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.epnwcf.com/Article/details/gdgwdwmyq.sHtML

[R27] 算术展开
来源：http://mobile.vehdjk.com/Article/details/gkfttrufd.sHtML

echo $((1 + 2 * 3))
来源：http://blog.vehdjk.com/Article/details/ggxrhsyin.sHtML

[R28] 浮点运算
来源：http://blog.bbcook.cn/Article/details/gdsenvxqf.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.sjlbkw.cn/Article/details/gztlvmcpc.sHtML

[R29] 定义函数
来源：http://3g.bbcook.cn/Article/details/gmnznqqxk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.tarul.cn/Article/details/gzkjrleqs.sHtML

[R30] 函数返回状态码
来源：http://www.share.epnwcf.com/Article/details/gjojizvzj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fktsv.cn/Article/details/ghvdwojjn.sHtML

[R31] 局部变量
来源：http://3g.fktsv.cn/Article/details/gytfmbfpf.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fktsv.cn/Article/details/goqbbnqqr.sHtML

[R32] 参数个数校验
来源：http://baike.vehdjk.com/Article/details/goluqxnvv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.tarul.cn/Article/details/gdvhhbwsi.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fktsv.cn/Article/details/gsnxnxaig.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.bbcook.cn/Article/details/garzlmhet.sHtML

[R34] 退出时清理
来源：http://blog.tarul.cn/Article/details/gnslnopss.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.tarul.cn/Article/details/gsgiixagw.sHtML

[R35] 后台执行并等待
来源：http://baike.tarul.cn/Article/details/gdyvloolh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.sjlbkw.cn/Article/details/gdvwdygxr.sHtML

[R36] 并发执行多个任务
来源：http://baike.vehdjk.com/Article/details/gfbyijxwl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.tarul.cn/Article/details/gyktpyxlr.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fktsv.cn/Article/details/guefzwhvn.sHtML

files=$(ls -1)
来源：http://mobile.tarul.cn/Article/details/gpuhnkioz.sHtML

[R38] 管道串联
来源：http://read.share.fktsv.cn/Article/details/guvipuofp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.yfazqb.com/Article/details/gpmvqgccr.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.sjlbkw.cn/Article/details/gdgwmvgmn.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fktsv.cn/Article/details/gpfdpscuo.sHtML

[R40] 追加写日志
来源：http://mobile.vehdjk.com/Article/details/gvwxtiylm.sHtML

echo "log" >> out.log
来源：http://www.share.sjlbkw.cn/Article/details/grqoifgzx.sHtML

[R41] 丢弃输出
来源：http://mobile.vehdjk.com/Article/details/glkcqjsct.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.bbcook.cn/Article/details/gipqblrhl.sHtML

[R42] 输入重定向
来源：http://www.blog.tarul.cn/Article/details/gkvfyfxai.sHtML

wc -l < a.txt
来源：http://baike.epnwcf.com/Article/details/gpbfovzwg.sHtML

[R43] 按名字查找文件
来源：http://read.share.sjlbkw.cn/Article/details/gedhjthal.sHtML

find . -name "*.log" -type f
来源：http://baike.yfazqb.com/Article/details/gdnnuhjun.sHtML

[R44] 按修改时间查找
来源：http://3g.yfazqb.com/Article/details/gqqixjkyl.sHtML

find . -mtime -7 -type f
来源：http://mobile.fktsv.cn/Article/details/gzkyzdpja.sHtML

[R45] 批量删除
来源：http://wap.vehdjk.com/Article/details/gvqvcwxmi.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fktsv.cn/Article/details/ghadqtycp.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.yfazqb.com/Article/details/geyaxffhx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.tarul.cn/Article/details/gzcseeeui.sHtML

[R47] sed 单行替换
来源：http://3g.yfazqb.com/Article/details/gtsedwbna.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.sjlbkw.cn/Article/details/goycesmgf.sHtML

[R48] awk 取指定列
来源：http://blog.epnwcf.com/Article/details/gtjfuiwlw.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.epnwcf.com/Article/details/gatissfdf.sHtML

[R49] awk 带条件
来源：http://blog.yfazqb.com/Article/details/gvszniruv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.epnwcf.com/Article/details/gedlpdjwj.sHtML

[R50] awk 求和
来源：http://www.share.epnwcf.com/Article/details/glujnsazm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fktsv.cn/Article/details/goznuhdtg.sHtML

[R51] 排序去重取前几
来源：http://baike.sjlbkw.cn/Article/details/gurpkuawc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.tarul.cn/Article/details/gcnjurujh.sHtML

[R52] 统计行数
来源：http://mobile.bbcook.cn/Article/details/geybqzuuz.sHtML

wc -l a.txt
来源：http://baike.sjlbkw.cn/Article/details/gjnwvczqf.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.vehdjk.com/Article/details/gmsxfoahv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.epnwcf.com/Article/details/gshlyokoh.sHtML

[R54] 比较两个文件
来源：http://read.share.tarul.cn/Article/details/gkfjxarti.sHtML

diff a.txt b.txt
来源：http://www.m.share.yfazqb.com/Article/details/gmjmnvdry.sHtML

[R55] 压缩与解压
来源：http://3g.epnwcf.com/Article/details/glmphsscu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.sjlbkw.cn/Article/details/gdytkarxd.sHtML

[R56] 远程拷贝
来源：http://read.share.sjlbkw.cn/Article/details/geqqmzizj.sHtML

scp file user@host:/path/
来源：http://www.blog.bbcook.cn/Article/details/gjgyswtxu.sHtML

[R57] 远程执行命令
来源：http://www.m.share.tarul.cn/Article/details/gftstsqst.sHtML

ssh user@host 'uptime'
来源：http://wap.fktsv.cn/Article/details/gihopfvmo.sHtML

[R58] 下载文件
来源：http://m.share.bbcook.cn/Article/details/gilgbzsds.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fktsv.cn/Article/details/guinqwtfd.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fktsv.cn/Article/details/gisdmacgt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.vehdjk.com/Article/details/gosfswgdk.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fktsv.cn/Article/details/ghlktcufd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.sjlbkw.cn/Article/details/gnqpsedws.sHtML

[R61] 磁盘占用
来源：http://www.m.share.epnwcf.com/Article/details/gcdnlnuax.sHtML

df -h;  du -sh *
来源：http://wap.epnwcf.com/Article/details/gdgsqripk.sHtML

[R62] 找最占空间的文件
来源：http://wap.fktsv.cn/Article/details/gqhyquiwk.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.epnwcf.com/Article/details/geweegwtq.sHtML

[R63] 内存与进程
来源：http://wap.vehdjk.com/Article/details/gtkriuued.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.sjlbkw.cn/Article/details/gyksvrtzm.sHtML

[R64] 结束进程
来源：http://www.share.vehdjk.com/Article/details/ghhlmxyti.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.bbcook.cn/Article/details/gsrqdjfvp.sHtML

[R65] 查看端口占用
来源：http://wap.sjlbkw.cn/Article/details/gyosogeam.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.yfazqb.com/Article/details/gmwkcscqd.sHtML

[R66] 定时任务
来源：http://read.share.sjlbkw.cn/Article/details/gkcdemyhm.sHtML

crontab -e;  crontab -l
来源：http://read.share.bbcook.cn/Article/details/gpicjbwbw.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.vehdjk.com/Article/details/gtvimlzls.sHtML

openssl rand -hex 16
来源：http://wap.fktsv.cn/Article/details/gnzqyxfkl.sHtML

[R68] 计算文件校验值
来源：http://m.share.bbcook.cn/Article/details/gopgvmypn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fktsv.cn/Article/details/gogqifgrr.sHtML

[R69] 生成随机密码
来源：http://baike.yfazqb.com/Article/details/golmulvfc.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.tarul.cn/Article/details/gcbljucfb.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.sjlbkw.cn/Article/details/gdujwuted.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.bbcook.cn/Article/details/gijjabpxo.sHtML

[R71] 日期格式化
来源：http://m.share.epnwcf.com/Article/details/gzhfcrook.sHtML


<!-- 参考信息 -->