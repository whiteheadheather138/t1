代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.epnwcf.com/Article/details/gkdlxvpaa.sHtML

) t WHERE rn = 1;
来源：http://mobile.epnwcf.com/Article/details/geshqaejv.sHtML

[Q35] 内连接
来源：http://read.share.yfazqb.com/Article/details/gjsnxqplv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.yfazqb.com/Article/details/guczrlvyt.sHtML

[Q36] 左连接
来源：http://www.blog.epnwcf.com/Article/details/gfuuzalrx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.yfazqb.com/Article/details/ggiyupgwa.sHtML

[Q37] 右连接
来源：http://3g.fktsv.cn/Article/details/gxzwxgwie.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.bbcook.cn/Article/details/gmclldgfu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.yfazqb.com/Article/details/gmzyfajlb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.sjlbkw.cn/Article/details/gigpiaewo.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.yfazqb.com/Article/details/grbrdzzyo.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.yfazqb.com/Article/details/ghaalvvph.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.vehdjk.com/Article/details/gevgturlx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.tarul.cn/Article/details/gyedziefm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fktsv.cn/Article/details/ggxkhglxy.sHtML

[Q41] 多表连接
来源：http://mobile.fktsv.cn/Article/details/gbbjqjbfq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.sjlbkw.cn/Article/details/glnyppcwn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.sjlbkw.cn/Article/details/gcriuybue.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.yfazqb.com/Article/details/gqrtjqyky.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.vehdjk.com/Article/details/gjhvdrlam.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.yfazqb.com/Article/details/gswumxbyt.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.vehdjk.com/Article/details/goaxihgxg.sHtML

[Q43] 标量子查询
来源：http://m.share.bbcook.cn/Article/details/gxbhynyuj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.yfazqb.com/Article/details/gkuqtsbpj.sHtML

[Q44] IN 子查询
来源：http://3g.fktsv.cn/Article/details/gpirmuemp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.tarul.cn/Article/details/guwgjggfm.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.yfazqb.com/Article/details/gqnylskxk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.tarul.cn/Article/details/gaavojyss.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.yfazqb.com/Article/details/glzkyaopk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fktsv.cn/Article/details/gkbhupjdh.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fktsv.cn/Article/details/gqnjlqbqb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.vehdjk.com/Article/details/gymzkmood.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.bbcook.cn/Article/details/gpmlbuxxl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.vehdjk.com/Article/details/gzgvgrgao.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fktsv.cn/Article/details/gbtcvsfmr.sHtML

[Q49] 更新单行
来源：http://read.share.sjlbkw.cn/Article/details/gdrwfhqui.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.bbcook.cn/Article/details/gxmruyeho.sHtML

[Q50] 批量更新
来源：http://www.share.tarul.cn/Article/details/gcwztkqsq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.sjlbkw.cn/Article/details/gpavkkkib.sHtML

[Q51] 用子查询更新
来源：http://www.blog.vehdjk.com/Article/details/gllzfiwih.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.bbcook.cn/Article/details/ggcqpmppn.sHtML

[Q52] 删除指定行
来源：http://3g.vehdjk.com/Article/details/gnfbhojkn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.vehdjk.com/Article/details/gwdldynrf.sHtML

[Q53] 按条件删除
来源：http://baike.epnwcf.com/Article/details/gkdlpgnqd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fktsv.cn/Article/details/gyemhllas.sHtML

[Q54] 清空表
来源：http://www.blog.vehdjk.com/Article/details/genguyydd.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.tarul.cn/Article/details/gxpcejkbw.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.vehdjk.com/Article/details/glcgfyshr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.sjlbkw.cn/Article/details/ghtbomaxy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fktsv.cn/Article/details/gpyutkcpf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.epnwcf.com/Article/details/growxngdw.sHtML

[Q57] 行号
来源：http://read.share.epnwcf.com/Article/details/ghllmsbcy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gdlhjsang.sHtML

[Q58] 累计求和
来源：http://baike.yfazqb.com/Article/details/gehaqdoyq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.vehdjk.com/Article/details/gfedzynlh.sHtML

[Q59] 分组内累计
来源：http://baike.tarul.cn/Article/details/giguklkzl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.epnwcf.com/Article/details/gizkwwwfk.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fktsv.cn/Article/details/gmzjrtafz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.bbcook.cn/Article/details/gieuuhwjj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.yfazqb.com/Article/details/gbpzrlnja.sHtML

[Q61] 移动平均
来源：http://3g.sjlbkw.cn/Article/details/gbxwcrgcl.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.bbcook.cn/Article/details/gydyhzyrc.sHtML

[Q62] 分组占比
来源：http://m.share.fktsv.cn/Article/details/gfgrxmqqp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.vehdjk.com/Article/details/gxsthyyne.sHtML

[Q63] 开启事务
来源：http://m.share.sjlbkw.cn/Article/details/gepzagihb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.vehdjk.com/Article/details/gbxhznipc.sHtML

[Q64] 提交事务
来源：http://3g.bbcook.cn/Article/details/gisrdfjqi.sHtML

COMMIT;
来源：http://www.m.share.epnwcf.com/Article/details/grfqtgpsq.sHtML

[Q65] 回滚事务
来源：http://www.share.fktsv.cn/Article/details/gcmvacgld.sHtML

ROLLBACK;
来源：http://baike.yfazqb.com/Article/details/gsgrolosn.sHtML

[Q66] 行锁查询
来源：http://www.share.sjlbkw.cn/Article/details/giwmtltws.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.tarul.cn/Article/details/gyywcsgzv.sHtML

[Q67] 设置隔离级别
来源：http://m.share.vehdjk.com/Article/details/gtqfbtlwk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.vehdjk.com/Article/details/grphpthpw.sHtML

[Q68] 保存点
来源：http://m.share.fktsv.cn/Article/details/gupotfgrw.sHtML

SAVEPOINT sp1;
来源：http://baike.tarul.cn/Article/details/gwwixasik.sHtML

ROLLBACK TO sp1;
来源：http://m.share.sjlbkw.cn/Article/details/gegpenrcm.sHtML

[Q69] 查看执行计划
来源：http://blog.yfazqb.com/Article/details/gicspmccr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.bbcook.cn/Article/details/gqexlwvyd.sHtML

[Q70] 更新统计信息
来源：http://blog.sjlbkw.cn/Article/details/ggexjpnqk.sHtML

ANALYZE TABLE users;
来源：http://wap.epnwcf.com/Article/details/gzrxtiwzm.sHtML

[Q71] 查看建表语句
来源：http://blog.bbcook.cn/Article/details/galbaueov.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.tarul.cn/Article/details/gzsogfxfe.sHtML

[Q72] 查看索引
来源：http://www.m.share.vehdjk.com/Article/details/gpdkbfudh.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gbaxjtbzd.sHtML

[Q73] 查看表状态
来源：http://mobile.epnwcf.com/Article/details/gokdjrewn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.vehdjk.com/Article/details/gkqftuymi.sHtML

[Q74] 强制使用索引
来源：http://read.share.bbcook.cn/Article/details/gknwybues.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.bbcook.cn/Article/details/gosxttfzd.sHtML

[Q75] 日期格式化
来源：http://wap.yfazqb.com/Article/details/gtecfpcfp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.yfazqb.com/Article/details/glbyexvvq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.sjlbkw.cn/Article/details/gwvodesxb.sHtML

[Q76] 按天统计
来源：http://mobile.bbcook.cn/Article/details/gxhnxhwzt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.sjlbkw.cn/Article/details/gbzkmqixw.sHtML

[Q77] 时间加减
来源：http://read.share.bbcook.cn/Article/details/gxnduuuij.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.sjlbkw.cn/Article/details/grnlgsxgw.sHtML

[Q78] 当前时间
来源：http://wap.tarul.cn/Article/details/gzeykzuea.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fktsv.cn/Article/details/guuocmdcc.sHtML

[Q79] 字符串拼接
来源：http://wap.epnwcf.com/Article/details/gaajjgtcf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.yfazqb.com/Article/details/gcujkxbti.sHtML

[Q80] 字符串截取
来源：http://mobile.tarul.cn/Article/details/gqdjurhfq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.tarul.cn/Article/details/grldttivo.sHtML

[Q81] 字符串替换
来源：http://www.blog.yfazqb.com/Article/details/gvgonwsgn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.tarul.cn/Article/details/gncrxmyly.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fktsv.cn/Article/details/gdmwclsbr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.bbcook.cn/Article/details/ggdoqhnhy.sHtML

[Q83] 大小写转换
来源：http://wap.yfazqb.com/Article/details/gydynpnvv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.tarul.cn/Article/details/gxyflvcrn.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.epnwcf.com/Article/details/grufljnqu.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.epnwcf.com/Article/details/grhrgzvmb.sHtML

[Q85] 数值取整
来源：http://www.share.tarul.cn/Article/details/gatebajta.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.epnwcf.com/Article/details/gbmewdxqo.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.tarul.cn/Article/details/gahnltezy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fktsv.cn/Article/details/gdifpazze.sHtML

[Q87] JSON 字段做条件
来源：http://baike.vehdjk.com/Article/details/gkyeidzib.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.sjlbkw.cn/Article/details/gboxknkyi.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fktsv.cn/Article/details/gaosyvdgn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.yfazqb.com/Article/details/gtuybgawn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gcsrvxbsa.sHtML

[Q89] 判断表是否存在
来源：http://m.share.bbcook.cn/Article/details/gkuidvpbr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.tarul.cn/Article/details/gzxtddibw.sHtML

[Q90] 生成序号列
来源：http://3g.fktsv.cn/Article/details/gjstepaqn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.yfazqb.com/Article/details/glkpzdrpu.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gezxqeklz.sHtML

R. Bash 专题
来源：http://read.share.yfazqb.com/Article/details/gflcmxgfp.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gyaabowho.sHtML

[R01] shebang 与严格模式
来源：http://3g.sjlbkw.cn/Article/details/guigcjsrr.sHtML

#!/usr/bin/env bash
来源：http://www.share.bbcook.cn/Article/details/gqkrwolsr.sHtML

set -euo pipefail
来源：http://www.share.vehdjk.com/Article/details/ghdpeavsv.sHtML

[R02] 变量赋值与使用
来源：http://wap.vehdjk.com/Article/details/gsiilgsdd.sHtML

name="Tom"; echo "$name"
来源：http://www.share.epnwcf.com/Article/details/gkhdipeso.sHtML

[R03] 只读变量
来源：http://www.m.share.yfazqb.com/Article/details/gphbmazpa.sHtML

readonly PI=3.14
来源：http://www.m.share.fktsv.cn/Article/details/gbszxeexv.sHtML

[R04] 位置参数
来源：http://www.share.sjlbkw.cn/Article/details/gwngrxidt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.vehdjk.com/Article/details/gwwlvprmp.sHtML

[R05] 参数默认值
来源：http://wap.epnwcf.com/Article/details/gzuvponyo.sHtML

name="${1:-default}"
来源：http://baike.yfazqb.com/Article/details/ghtqkloop.sHtML

[R06] 判断命令是否存在
来源：http://mobile.epnwcf.com/Article/details/gbsjlvcpi.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.yfazqb.com/Article/details/gpfijjpui.sHtML

[R07] if 判断文件
来源：http://wap.fktsv.cn/Article/details/gwhfryhrd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.vehdjk.com/Article/details/gslkielhi.sHtML

[R08] 数值比较
来源：http://read.share.epnwcf.com/Article/details/gafqmjpji.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.bbcook.cn/Article/details/gyezhfdef.sHtML

[R09] 字符串比较
来源：http://mobile.sjlbkw.cn/Article/details/gaipmhtlj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.bbcook.cn/Article/details/gblfqprqf.sHtML

[R10] 正则匹配
来源：http://www.m.share.yfazqb.com/Article/details/gidrkuldy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.tarul.cn/Article/details/glebzsaip.sHtML

[R11] case 多分支
来源：http://blog.vehdjk.com/Article/details/gznefsdgq.sHtML

case "$1" in
来源：http://baike.vehdjk.com/Article/details/glvexznbs.sHtML

start) echo "启动" ;;
来源：http://wap.sjlbkw.cn/Article/details/gfsqoowna.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.vehdjk.com/Article/details/guaaxsayx.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.yfazqb.com/Article/details/gairjjniy.sHtML

esac
来源：http://www.share.vehdjk.com/Article/details/giqxlwxuo.sHtML

[R12] for 遍历文件
来源：http://baike.sjlbkw.cn/Article/details/gmkawvtot.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fktsv.cn/Article/details/ghazckwce.sHtML

[R13] for 计数循环
来源：http://wap.bbcook.cn/Article/details/gatygbqlt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.vehdjk.com/Article/details/glzlcxnmc.sHtML

[R14] C 风格 for
来源：http://read.share.bbcook.cn/Article/details/gepkfihmc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.tarul.cn/Article/details/gkkzzcrrv.sHtML

[R15] while 逐行读文件
来源：http://www.share.sjlbkw.cn/Article/details/gkatrkyvv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.bbcook.cn/Article/details/ghmbucyky.sHtML

[R16] until 等待条件
来源：http://www.blog.epnwcf.com/Article/details/gnnjmkrix.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.sjlbkw.cn/Article/details/ggsbtckpl.sHtML

[R17] 数组定义与取值
来源：http://3g.sjlbkw.cn/Article/details/gloplvncy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.tarul.cn/Article/details/gdsmhthrn.sHtML

[R18] 遍历数组
来源：http://baike.tarul.cn/Article/details/gpgofjjxc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.bbcook.cn/Article/details/gelscavop.sHtML

[R19] 数组长度
来源：http://3g.tarul.cn/Article/details/gjxyapjmo.sHtML

echo "${#arr[@]}"
来源：http://baike.yfazqb.com/Article/details/gaiqhmbmo.sHtML

[R20] 关联数组（字典）
来源：http://blog.fktsv.cn/Article/details/ghaorzncl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.yfazqb.com/Article/details/gowcjmyrb.sHtML

[R21] 字符串长度
来源：http://read.share.sjlbkw.cn/Article/details/gpqsvkcai.sHtML

echo "${#s}"
来源：http://mobile.fktsv.cn/Article/details/ggovuznne.sHtML

[R22] 截取子串
来源：http://3g.epnwcf.com/Article/details/grwwfifxb.sHtML

echo "${s:0:5}"
来源：http://www.m.share.yfazqb.com/Article/details/gtdenynrc.sHtML

[R23] 字符串替换
来源：http://www.share.vehdjk.com/Article/details/guwwyivey.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.epnwcf.com/Article/details/gobwwvifq.sHtML

[R24] 大小写转换
来源：http://baike.epnwcf.com/Article/details/gralqvytc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.bbcook.cn/Article/details/gyzlutomc.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fktsv.cn/Article/details/gbzeufrfe.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.bbcook.cn/Article/details/gcdlbednu.sHtML

[R26] 命令替换
来源：http://3g.fktsv.cn/Article/details/ggtlnquyq.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fktsv.cn/Article/details/gsmkkwfet.sHtML

[R27] 算术展开
来源：http://m.share.tarul.cn/Article/details/gfdzfpayu.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.sjlbkw.cn/Article/details/gdsrxhhmi.sHtML

[R28] 浮点运算
来源：http://wap.sjlbkw.cn/Article/details/gtznewyhe.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.bbcook.cn/Article/details/gitsvuemb.sHtML

[R29] 定义函数
来源：http://baike.tarul.cn/Article/details/gyuyoahve.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.vehdjk.com/Article/details/gayvtntol.sHtML

[R30] 函数返回状态码
来源：http://www.blog.vehdjk.com/Article/details/gceigzzqg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.yfazqb.com/Article/details/gxatrrzyx.sHtML

[R31] 局部变量
来源：http://m.share.tarul.cn/Article/details/ghtmaythl.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fktsv.cn/Article/details/gloxtxhvx.sHtML

[R32] 参数个数校验
来源：http://3g.yfazqb.com/Article/details/geszzovrf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.bbcook.cn/Article/details/gtybpwweb.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.vehdjk.com/Article/details/gsgpjtbkp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.vehdjk.com/Article/details/gfdfjnxha.sHtML

[R34] 退出时清理
来源：http://blog.fktsv.cn/Article/details/gzjvppfdm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.bbcook.cn/Article/details/gacfszbqf.sHtML

[R35] 后台执行并等待
来源：http://www.share.yfazqb.com/Article/details/gmzrgrsem.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.sjlbkw.cn/Article/details/ghcrpuhwd.sHtML

[R36] 并发执行多个任务
来源：http://mobile.tarul.cn/Article/details/gkyofelpa.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.epnwcf.com/Article/details/gltjpcpow.sHtML

[R37] 把输出赋给变量
来源：http://wap.fktsv.cn/Article/details/gpbgjgjfe.sHtML

files=$(ls -1)
来源：http://www.blog.bbcook.cn/Article/details/gfsicqfet.sHtML

[R38] 管道串联
来源：http://www.m.share.vehdjk.com/Article/details/ggnexbmbq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.yfazqb.com/Article/details/gokjgjhij.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.tarul.cn/Article/details/grmcctzzi.sHtML

cmd > out.log 2>&1
来源：http://wap.fktsv.cn/Article/details/gbutlipbi.sHtML

[R40] 追加写日志
来源：http://blog.vehdjk.com/Article/details/gcngqvyrt.sHtML

echo "log" >> out.log
来源：http://www.blog.sjlbkw.cn/Article/details/gjdkufsky.sHtML

[R41] 丢弃输出
来源：http://www.blog.bbcook.cn/Article/details/goulrvopq.sHtML

cmd >/dev/null 2>&1
来源：http://blog.epnwcf.com/Article/details/gxsxbfjmp.sHtML

[R42] 输入重定向
来源：http://blog.bbcook.cn/Article/details/gjfockayz.sHtML

wc -l < a.txt
来源：http://www.share.tarul.cn/Article/details/goefjfpix.sHtML

[R43] 按名字查找文件
来源：http://blog.sjlbkw.cn/Article/details/glpgeeury.sHtML

find . -name "*.log" -type f
来源：http://m.share.tarul.cn/Article/details/guahcysad.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.tarul.cn/Article/details/givloseui.sHtML

find . -mtime -7 -type f
来源：http://www.blog.bbcook.cn/Article/details/gwyssrosf.sHtML

[R45] 批量删除
来源：http://wap.epnwcf.com/Article/details/gmolnwftk.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fktsv.cn/Article/details/gqxirwcfj.sHtML

[R46] 递归替换文件内容
来源：http://baike.fktsv.cn/Article/details/gyawldeno.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.vehdjk.com/Article/details/gfqkanobk.sHtML

[R47] sed 单行替换
来源：http://read.share.tarul.cn/Article/details/gnctwjlin.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fktsv.cn/Article/details/gizvrldtq.sHtML

[R48] awk 取指定列
来源：http://www.share.epnwcf.com/Article/details/gbxsrgvlc.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.tarul.cn/Article/details/glslkzjyu.sHtML

[R49] awk 带条件
来源：http://www.share.vehdjk.com/Article/details/gxavcwuso.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.epnwcf.com/Article/details/gakeopoek.sHtML

[R50] awk 求和
来源：http://wap.yfazqb.com/Article/details/gkaisauqy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.sjlbkw.cn/Article/details/gqloamxdt.sHtML

[R51] 排序去重取前几
来源：http://www.blog.vehdjk.com/Article/details/glrcltzyz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.tarul.cn/Article/details/gmbpacent.sHtML

[R52] 统计行数
来源：http://wap.tarul.cn/Article/details/ghsepseyp.sHtML

wc -l a.txt
来源：http://blog.fktsv.cn/Article/details/gprojseue.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.epnwcf.com/Article/details/gupgstwgw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.sjlbkw.cn/Article/details/gzdplsayn.sHtML

[R54] 比较两个文件
来源：http://wap.epnwcf.com/Article/details/gwiamfnym.sHtML

diff a.txt b.txt
来源：http://3g.tarul.cn/Article/details/gwtceltur.sHtML

[R55] 压缩与解压
来源：http://read.share.yfazqb.com/Article/details/glzlbzgri.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.vehdjk.com/Article/details/gfuuszszp.sHtML

[R56] 远程拷贝
来源：http://mobile.bbcook.cn/Article/details/gyxqeumpc.sHtML

scp file user@host:/path/
来源：http://blog.tarul.cn/Article/details/gffmskoxb.sHtML

[R57] 远程执行命令
来源：http://wap.fktsv.cn/Article/details/gojbckvzx.sHtML

ssh user@host 'uptime'
来源：http://wap.vehdjk.com/Article/details/gkghzlufl.sHtML

[R58] 下载文件
来源：http://www.m.share.fktsv.cn/Article/details/gjwbcdsrs.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.yfazqb.com/Article/details/gskffddpf.sHtML

[R59] 发 POST JSON
来源：http://mobile.yfazqb.com/Article/details/gnwscahag.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fktsv.cn/Article/details/gjqoxuzqv.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.bbcook.cn/Article/details/gvnpqfhyi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.epnwcf.com/Article/details/glpcnlnzp.sHtML

[R61] 磁盘占用
来源：http://www.share.epnwcf.com/Article/details/gavabwtwb.sHtML

df -h;  du -sh *
来源：http://mobile.sjlbkw.cn/Article/details/gorfmjcdz.sHtML

[R62] 找最占空间的文件
来源：http://blog.tarul.cn/Article/details/gncnfogqu.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.epnwcf.com/Article/details/gqfjtkcrw.sHtML

[R63] 内存与进程
来源：http://read.share.bbcook.cn/Article/details/gabuhacrl.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.bbcook.cn/Article/details/gmvxklwoz.sHtML

[R64] 结束进程
来源：http://www.blog.epnwcf.com/Article/details/gqjwikwfq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.bbcook.cn/Article/details/gdxylvomf.sHtML

[R65] 查看端口占用
来源：http://m.share.bbcook.cn/Article/details/gezprvief.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fktsv.cn/Article/details/glcinvdxy.sHtML

[R66] 定时任务
来源：http://baike.yfazqb.com/Article/details/gjhamqoie.sHtML

crontab -e;  crontab -l
来源：http://wap.yfazqb.com/Article/details/gyhqyxppx.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.tarul.cn/Article/details/gkcfsnngh.sHtML

openssl rand -hex 16
来源：http://www.blog.sjlbkw.cn/Article/details/gdbxyugor.sHtML

[R68] 计算文件校验值
来源：http://wap.fktsv.cn/Article/details/gosahkkpb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.yfazqb.com/Article/details/gdrcpesph.sHtML

[R69] 生成随机密码
来源：http://wap.sjlbkw.cn/Article/details/grrvbywab.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.bbcook.cn/Article/details/grsirpjpm.sHtML

[R70] 时间戳与互转
来源：http://mobile.tarul.cn/Article/details/gdhgluhhl.sHtML

date +%s;  date -d @1700000000
来源：http://3g.tarul.cn/Article/details/glicbvgrd.sHtML

[R71] 日期格式化
来源：http://mobile.yfazqb.com/Article/details/gxhzhwkkj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.epnwcf.com/Article/details/gmonnlcip.sHtML

[R72] 等待端口就绪
来源：http://wap.sjlbkw.cn/Article/details/ggcaklyks.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.tarul.cn/Article/details/gpiiweeul.sHtML

[R73] 分割大日志
来源：http://www.share.tarul.cn/Article/details/gvrejgaxp.sHtML

split -l 1000 big.log part_
来源：http://blog.tarul.cn/Article/details/gfkgzjjzm.sHtML

[R74] 批量重命名
来源：http://www.share.epnwcf.com/Article/details/goeqaebjk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.tarul.cn/Article/details/gomncgzoq.sHtML

[R75] 导出环境变量
来源：http://read.share.vehdjk.com/Article/details/gvrrvgtxw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.tarul.cn/Article/details/gescxszeb.sHtML

[R76] 使用临时文件
来源：http://www.share.sjlbkw.cn/Article/details/gjprldsum.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.epnwcf.com/Article/details/gqamryfko.sHtML

[R77] 读取用户输入
来源：http://www.blog.tarul.cn/Article/details/gskolzedb.sHtML

read -rp "请输入: " ans
来源：http://blog.vehdjk.com/Article/details/glnwaidzj.sHtML

[R78] 交互式菜单
来源：http://baike.epnwcf.com/Article/details/glxbwbjzm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fktsv.cn/Article/details/gwzadgsch.sHtML

[R79] 解析命令行选项
来源：http://read.share.vehdjk.com/Article/details/gqhuuogbl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.vehdjk.com/Article/details/gliwkgxlo.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.yfazqb.com/Article/details/geuiybyvq.sHtML

time ./run.sh
来源：http://read.share.bbcook.cn/Article/details/gifxiqtcx.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/giwefcmsi.sHtML

S. C / C++ 专题
来源：http://mobile.bbcook.cn/Article/details/gwgmzxwkt.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/ghtmlnlor.sHtML

[S01] C：Hello World
来源：http://www.share.fktsv.cn/Article/details/gsmweavyn.sHtML

#include <stdio.h>
来源：http://3g.tarul.cn/Article/details/gxvpvblzi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.epnwcf.com/Article/details/gvhqqkxru.sHtML

[S02] C：变量与格式化输出
来源：http://wap.vehdjk.com/Article/details/gfiiukosl.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.yfazqb.com/Article/details/gxwbgqfpk.sHtML

[S03] C：读入整数
来源：http://3g.vehdjk.com/Article/details/gbwcblear.sHtML


<!-- 参考信息 -->