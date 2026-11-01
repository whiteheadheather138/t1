代发 wailian999

[Q33] 多列分组
来源：http://m.share.sjlbkw.cn/Article/details/gdckyadbe.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.tarul.cn/Article/details/ghnhsfdcb.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.yfazqb.com/Article/details/gzxrbfhit.sHtML

SELECT * FROM (
来源：http://www.blog.sjlbkw.cn/Article/details/gcrohaoux.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.tarul.cn/Article/details/gwkcpqdio.sHtML

) t WHERE rn = 1;
来源：http://www.share.yfazqb.com/Article/details/gpxixentv.sHtML

[Q35] 内连接
来源：http://read.share.sjlbkw.cn/Article/details/gkpvfqblp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.epnwcf.com/Article/details/gungxgpak.sHtML

[Q36] 左连接
来源：http://www.share.vehdjk.com/Article/details/ghirpvmvg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.vehdjk.com/Article/details/gjcwijeka.sHtML

[Q37] 右连接
来源：http://read.share.bbcook.cn/Article/details/galdslxya.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.vehdjk.com/Article/details/gmnreszfh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fktsv.cn/Article/details/gwriwyynb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.bbcook.cn/Article/details/gaigmjuuz.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.bbcook.cn/Article/details/gccfcpemm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fktsv.cn/Article/details/gvmllullq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.yfazqb.com/Article/details/gfwxtriah.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.sjlbkw.cn/Article/details/gqhtbsdzu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fktsv.cn/Article/details/guubrgcok.sHtML

[Q41] 多表连接
来源：http://blog.sjlbkw.cn/Article/details/guxqpbzzu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.tarul.cn/Article/details/ghvxdqlpc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.vehdjk.com/Article/details/gdbfufmkb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.yfazqb.com/Article/details/gltwbkhfr.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.vehdjk.com/Article/details/gfyekijxf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fktsv.cn/Article/details/gigtpgako.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.yfazqb.com/Article/details/giresavbl.sHtML

[Q43] 标量子查询
来源：http://www.m.share.tarul.cn/Article/details/gaetzfvlz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.tarul.cn/Article/details/gkcyroeyw.sHtML

[Q44] IN 子查询
来源：http://mobile.epnwcf.com/Article/details/glovpched.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fktsv.cn/Article/details/gmfhaaicg.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.epnwcf.com/Article/details/ghmhdsipd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.bbcook.cn/Article/details/gwepfcpxn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.sjlbkw.cn/Article/details/gvzbrwvvp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.epnwcf.com/Article/details/gqvbawvfj.sHtML

[Q47] 与平均值比较
来源：http://baike.tarul.cn/Article/details/gdlpabvaw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.vehdjk.com/Article/details/giptqvjfb.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.yfazqb.com/Article/details/gplekxdls.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.tarul.cn/Article/details/gyizcvova.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.vehdjk.com/Article/details/ggpekeegs.sHtML

[Q49] 更新单行
来源：http://wap.fktsv.cn/Article/details/gpwdlaqwf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.yfazqb.com/Article/details/gohivfcba.sHtML

[Q50] 批量更新
来源：http://3g.fktsv.cn/Article/details/gqbrmurmh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fktsv.cn/Article/details/gdexwydec.sHtML

[Q51] 用子查询更新
来源：http://www.blog.sjlbkw.cn/Article/details/gzihedpuy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.tarul.cn/Article/details/gqupxwjog.sHtML

[Q52] 删除指定行
来源：http://3g.yfazqb.com/Article/details/gkhfxyjkj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.epnwcf.com/Article/details/gjkgkoybp.sHtML

[Q53] 按条件删除
来源：http://read.share.yfazqb.com/Article/details/gxyeowqng.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fktsv.cn/Article/details/giqqwmkma.sHtML

[Q54] 清空表
来源：http://www.share.fktsv.cn/Article/details/gfiqvfdxx.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.tarul.cn/Article/details/gmgnlmbno.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.vehdjk.com/Article/details/gdxzthyda.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.tarul.cn/Article/details/gbeteyiew.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.epnwcf.com/Article/details/geauhdrlo.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fktsv.cn/Article/details/gaechzjnd.sHtML

[Q57] 行号
来源：http://www.share.bbcook.cn/Article/details/ghtcoykpo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/guymmqmqb.sHtML

[Q58] 累计求和
来源：http://wap.fktsv.cn/Article/details/gtqaymbcl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.epnwcf.com/Article/details/gmolpouao.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fktsv.cn/Article/details/gubelqgme.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.epnwcf.com/Article/details/gbcxphhva.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.epnwcf.com/Article/details/gxaxjkmna.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fktsv.cn/Article/details/gdwhekwuu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fktsv.cn/Article/details/gccfpwbli.sHtML

[Q61] 移动平均
来源：http://www.share.tarul.cn/Article/details/grlebdmgo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.bbcook.cn/Article/details/guwzkyhpl.sHtML

[Q62] 分组占比
来源：http://www.share.tarul.cn/Article/details/gtbjxcnym.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.sjlbkw.cn/Article/details/gmondpqjo.sHtML

[Q63] 开启事务
来源：http://www.share.fktsv.cn/Article/details/goplsygra.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.epnwcf.com/Article/details/gawpoowuh.sHtML

[Q64] 提交事务
来源：http://blog.sjlbkw.cn/Article/details/glmkhdapf.sHtML

COMMIT;
来源：http://baike.tarul.cn/Article/details/guzsrisvt.sHtML

[Q65] 回滚事务
来源：http://wap.sjlbkw.cn/Article/details/gixqxeshf.sHtML

ROLLBACK;
来源：http://baike.tarul.cn/Article/details/gegzczdjh.sHtML

[Q66] 行锁查询
来源：http://3g.sjlbkw.cn/Article/details/gahvogwkc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.bbcook.cn/Article/details/gqpbcbqft.sHtML

[Q67] 设置隔离级别
来源：http://m.share.bbcook.cn/Article/details/gcnjszfeq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.vehdjk.com/Article/details/gklraeeyd.sHtML

[Q68] 保存点
来源：http://www.share.yfazqb.com/Article/details/gvpwxrhza.sHtML

SAVEPOINT sp1;
来源：http://read.share.epnwcf.com/Article/details/geluzenqc.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fktsv.cn/Article/details/gffwicqpm.sHtML

[Q69] 查看执行计划
来源：http://blog.yfazqb.com/Article/details/gfmzkezoe.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.tarul.cn/Article/details/glpwkplto.sHtML

[Q70] 更新统计信息
来源：http://3g.fktsv.cn/Article/details/gpuytgmmz.sHtML

ANALYZE TABLE users;
来源：http://blog.bbcook.cn/Article/details/gheavqjpj.sHtML

[Q71] 查看建表语句
来源：http://wap.sjlbkw.cn/Article/details/gppvsmwdy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.yfazqb.com/Article/details/gytfnktah.sHtML

[Q72] 查看索引
来源：http://3g.sjlbkw.cn/Article/details/gsbrqjujw.sHtML

SHOW INDEX FROM users;
来源：http://3g.tarul.cn/Article/details/ggfxdawae.sHtML

[Q73] 查看表状态
来源：http://www.blog.sjlbkw.cn/Article/details/gsctzagmr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fktsv.cn/Article/details/gvzssssum.sHtML

[Q74] 强制使用索引
来源：http://baike.sjlbkw.cn/Article/details/gdmhggalf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.yfazqb.com/Article/details/gpktpnozy.sHtML

[Q75] 日期格式化
来源：http://mobile.vehdjk.com/Article/details/gyxzhhxir.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.bbcook.cn/Article/details/gnziumuzg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.bbcook.cn/Article/details/gdypngmyv.sHtML

[Q76] 按天统计
来源：http://www.m.share.tarul.cn/Article/details/ghbnivwii.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.epnwcf.com/Article/details/goditvsiv.sHtML

[Q77] 时间加减
来源：http://3g.vehdjk.com/Article/details/geogrewnm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.bbcook.cn/Article/details/gmzxctgag.sHtML

[Q78] 当前时间
来源：http://wap.tarul.cn/Article/details/ggbytmjzj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.vehdjk.com/Article/details/grbjpljwl.sHtML

[Q79] 字符串拼接
来源：http://blog.tarul.cn/Article/details/ggsotjuev.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fktsv.cn/Article/details/gadjznifv.sHtML

[Q80] 字符串截取
来源：http://mobile.fktsv.cn/Article/details/gnurfeudp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gstfrfalb.sHtML

[Q81] 字符串替换
来源：http://www.share.vehdjk.com/Article/details/gknblvnks.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gslwmhkvi.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.bbcook.cn/Article/details/gfgqmbstv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gcpsbxrek.sHtML

[Q83] 大小写转换
来源：http://m.share.vehdjk.com/Article/details/grvhpqgma.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fktsv.cn/Article/details/gfxsuelmf.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.tarul.cn/Article/details/grsbligjh.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.vehdjk.com/Article/details/gocokxmqv.sHtML

[Q85] 数值取整
来源：http://www.share.yfazqb.com/Article/details/gyeqcvsiv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.yfazqb.com/Article/details/goqfrbivz.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.yfazqb.com/Article/details/ggcmixrpc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fktsv.cn/Article/details/gkifcupeu.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.tarul.cn/Article/details/gwkhxpdjj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.bbcook.cn/Article/details/gthkwrxjg.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.vehdjk.com/Article/details/gegojywzh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.epnwcf.com/Article/details/giftqrxek.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.vehdjk.com/Article/details/gxubtphwp.sHtML

[Q89] 判断表是否存在
来源：http://wap.vehdjk.com/Article/details/gbwurwkom.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fktsv.cn/Article/details/gwrafulek.sHtML

[Q90] 生成序号列
来源：http://www.blog.yfazqb.com/Article/details/gtlnworcs.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.epnwcf.com/Article/details/gmxzzbile.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gvbakwnht.sHtML

R. Bash 专题
来源：http://blog.bbcook.cn/Article/details/govdazooe.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/ggaqohprt.sHtML

[R01] shebang 与严格模式
来源：http://read.share.vehdjk.com/Article/details/gxlsoiygc.sHtML

#!/usr/bin/env bash
来源：http://3g.tarul.cn/Article/details/gxaydhgzg.sHtML

set -euo pipefail
来源：http://www.share.yfazqb.com/Article/details/grtgzzyph.sHtML

[R02] 变量赋值与使用
来源：http://blog.bbcook.cn/Article/details/gzfyvezpa.sHtML

name="Tom"; echo "$name"
来源：http://3g.vehdjk.com/Article/details/gksjsoanc.sHtML

[R03] 只读变量
来源：http://read.share.vehdjk.com/Article/details/gmurlqbxp.sHtML

readonly PI=3.14
来源：http://baike.tarul.cn/Article/details/gkkdctaxx.sHtML

[R04] 位置参数
来源：http://blog.bbcook.cn/Article/details/grzedrwxg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fktsv.cn/Article/details/gysuxnyng.sHtML

[R05] 参数默认值
来源：http://www.share.sjlbkw.cn/Article/details/ggpaolsvc.sHtML

name="${1:-default}"
来源：http://www.share.vehdjk.com/Article/details/gprhosmwn.sHtML

[R06] 判断命令是否存在
来源：http://m.share.sjlbkw.cn/Article/details/grppxddyw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.bbcook.cn/Article/details/gyzjpyvub.sHtML

[R07] if 判断文件
来源：http://blog.bbcook.cn/Article/details/gpcwfabsk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.sjlbkw.cn/Article/details/gyfiprbah.sHtML

[R08] 数值比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gnaurwddd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.yfazqb.com/Article/details/gisphravh.sHtML

[R09] 字符串比较
来源：http://m.share.vehdjk.com/Article/details/gpazxmnet.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.tarul.cn/Article/details/gstoiibob.sHtML

[R10] 正则匹配
来源：http://read.share.bbcook.cn/Article/details/ghzjtinhh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.epnwcf.com/Article/details/gkcgktfgy.sHtML

[R11] case 多分支
来源：http://www.blog.sjlbkw.cn/Article/details/giefgkxie.sHtML

case "$1" in
来源：http://m.share.bbcook.cn/Article/details/gzleqmhvk.sHtML

start) echo "启动" ;;
来源：http://read.share.vehdjk.com/Article/details/gdqeqewqa.sHtML

stop)  echo "停止" ;;
来源：http://3g.vehdjk.com/Article/details/gcjmlircm.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.epnwcf.com/Article/details/gtnoaskfd.sHtML

esac
来源：http://wap.yfazqb.com/Article/details/grbxhjooi.sHtML

[R12] for 遍历文件
来源：http://read.share.bbcook.cn/Article/details/gsmrngbzz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.yfazqb.com/Article/details/gwpxvysfi.sHtML

[R13] for 计数循环
来源：http://m.share.bbcook.cn/Article/details/gvdsnpsyq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.sjlbkw.cn/Article/details/gkthibuvq.sHtML

[R14] C 风格 for
来源：http://mobile.tarul.cn/Article/details/gsufjwszk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.yfazqb.com/Article/details/gekudcgtv.sHtML

[R15] while 逐行读文件
来源：http://mobile.fktsv.cn/Article/details/gvnwnieea.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.epnwcf.com/Article/details/gemkreefk.sHtML

[R16] until 等待条件
来源：http://read.share.tarul.cn/Article/details/gtjshbhhb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.bbcook.cn/Article/details/gzeownwub.sHtML

[R17] 数组定义与取值
来源：http://www.blog.bbcook.cn/Article/details/gellylsar.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.vehdjk.com/Article/details/gvdsqyqrj.sHtML

[R18] 遍历数组
来源：http://m.share.epnwcf.com/Article/details/gglwzholh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fktsv.cn/Article/details/gnkjqyhxb.sHtML

[R19] 数组长度
来源：http://www.blog.sjlbkw.cn/Article/details/glypzolrr.sHtML

echo "${#arr[@]}"
来源：http://wap.sjlbkw.cn/Article/details/gzejdmmey.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fktsv.cn/Article/details/gawaqipyx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.tarul.cn/Article/details/gvpmcggga.sHtML

[R21] 字符串长度
来源：http://mobile.yfazqb.com/Article/details/gldmeqbyn.sHtML

echo "${#s}"
来源：http://blog.tarul.cn/Article/details/gifjxufli.sHtML

[R22] 截取子串
来源：http://www.blog.bbcook.cn/Article/details/gcvtxrerf.sHtML

echo "${s:0:5}"
来源：http://wap.tarul.cn/Article/details/gpqkczrxm.sHtML

[R23] 字符串替换
来源：http://mobile.epnwcf.com/Article/details/gdlqbqjsj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fktsv.cn/Article/details/gskvuslol.sHtML

[R24] 大小写转换
来源：http://wap.vehdjk.com/Article/details/gaekcfudf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.tarul.cn/Article/details/glmqctiyr.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.tarul.cn/Article/details/gavhwvfkj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fktsv.cn/Article/details/gzmtbwfun.sHtML

[R26] 命令替换
来源：http://www.share.vehdjk.com/Article/details/gcbnyiiek.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.tarul.cn/Article/details/gafmklzpr.sHtML

[R27] 算术展开
来源：http://m.share.sjlbkw.cn/Article/details/gemeekksh.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.sjlbkw.cn/Article/details/glcjedqop.sHtML

[R28] 浮点运算
来源：http://m.share.sjlbkw.cn/Article/details/gywwvcdcc.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fktsv.cn/Article/details/gxoxdssbe.sHtML

[R29] 定义函数
来源：http://www.blog.bbcook.cn/Article/details/gugncnkju.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.yfazqb.com/Article/details/gnbkwcmat.sHtML

[R30] 函数返回状态码
来源：http://wap.fktsv.cn/Article/details/ggxeifcjj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.sjlbkw.cn/Article/details/gefturgjc.sHtML

[R31] 局部变量
来源：http://mobile.vehdjk.com/Article/details/gyzbnbrwu.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fktsv.cn/Article/details/gltdmmpep.sHtML

[R32] 参数个数校验
来源：http://wap.fktsv.cn/Article/details/gvimngwhd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.tarul.cn/Article/details/ghyjuowrd.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.tarul.cn/Article/details/gvuzaqxkp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.sjlbkw.cn/Article/details/gcjigidkz.sHtML

[R34] 退出时清理
来源：http://mobile.vehdjk.com/Article/details/gqqbvhzsz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.sjlbkw.cn/Article/details/gzjujbamk.sHtML

[R35] 后台执行并等待
来源：http://www.blog.sjlbkw.cn/Article/details/gnexudwzt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.sjlbkw.cn/Article/details/gnpppzinj.sHtML

[R36] 并发执行多个任务
来源：http://3g.epnwcf.com/Article/details/ggtsvpxij.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.epnwcf.com/Article/details/gsgggllwn.sHtML

[R37] 把输出赋给变量
来源：http://blog.yfazqb.com/Article/details/gbvsnoatr.sHtML

files=$(ls -1)
来源：http://wap.vehdjk.com/Article/details/ggxszgmgf.sHtML

[R38] 管道串联
来源：http://wap.epnwcf.com/Article/details/gyehyoccx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.epnwcf.com/Article/details/gwdxovior.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.epnwcf.com/Article/details/gzgjlmnpd.sHtML

cmd > out.log 2>&1
来源：http://blog.bbcook.cn/Article/details/gcahhisim.sHtML

[R40] 追加写日志
来源：http://m.share.tarul.cn/Article/details/gvrihjjqq.sHtML

echo "log" >> out.log
来源：http://baike.epnwcf.com/Article/details/gptntbrjr.sHtML

[R41] 丢弃输出
来源：http://www.m.share.bbcook.cn/Article/details/gxnqkbfka.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.sjlbkw.cn/Article/details/ggbdpziqg.sHtML

[R42] 输入重定向
来源：http://3g.epnwcf.com/Article/details/goyxnlady.sHtML

wc -l < a.txt
来源：http://mobile.tarul.cn/Article/details/grvydrnlc.sHtML

[R43] 按名字查找文件
来源：http://read.share.epnwcf.com/Article/details/gujorkoxd.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.bbcook.cn/Article/details/gpeavkvba.sHtML

[R44] 按修改时间查找
来源：http://mobile.fktsv.cn/Article/details/ggnooowsg.sHtML

find . -mtime -7 -type f
来源：http://www.blog.vehdjk.com/Article/details/gppmogauz.sHtML

[R45] 批量删除
来源：http://www.m.share.sjlbkw.cn/Article/details/gkaeerclt.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.tarul.cn/Article/details/gafgdklhh.sHtML

[R46] 递归替换文件内容
来源：http://3g.epnwcf.com/Article/details/gccefwfny.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.vehdjk.com/Article/details/gtdbzcqff.sHtML

[R47] sed 单行替换
来源：http://wap.bbcook.cn/Article/details/gifcbudph.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.vehdjk.com/Article/details/gwrsrcxmw.sHtML

[R48] awk 取指定列
来源：http://baike.bbcook.cn/Article/details/gmhhdkuaj.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.vehdjk.com/Article/details/grlvwouxj.sHtML

[R49] awk 带条件
来源：http://www.blog.fktsv.cn/Article/details/gfwwveisg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.bbcook.cn/Article/details/gdvjnptis.sHtML

[R50] awk 求和
来源：http://read.share.epnwcf.com/Article/details/gjkauizfh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.epnwcf.com/Article/details/gddictuka.sHtML

[R51] 排序去重取前几
来源：http://mobile.yfazqb.com/Article/details/gfgnbwztq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.bbcook.cn/Article/details/gqzwmlxwu.sHtML

[R52] 统计行数
来源：http://mobile.sjlbkw.cn/Article/details/gfusmgboi.sHtML

wc -l a.txt
来源：http://www.blog.yfazqb.com/Article/details/gomkwhxiq.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.epnwcf.com/Article/details/gzmewqawy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.vehdjk.com/Article/details/gmicnhlmg.sHtML

[R54] 比较两个文件
来源：http://www.blog.epnwcf.com/Article/details/gbnyziuxy.sHtML

diff a.txt b.txt
来源：http://mobile.bbcook.cn/Article/details/gxxktaetr.sHtML

[R55] 压缩与解压
来源：http://www.share.vehdjk.com/Article/details/gaszvlpya.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.sjlbkw.cn/Article/details/gagpwwpvk.sHtML

[R56] 远程拷贝
来源：http://blog.bbcook.cn/Article/details/giygvbedy.sHtML

scp file user@host:/path/
来源：http://mobile.fktsv.cn/Article/details/gkgmserko.sHtML

[R57] 远程执行命令
来源：http://baike.fktsv.cn/Article/details/gbsbckbix.sHtML

ssh user@host 'uptime'
来源：http://baike.fktsv.cn/Article/details/getmbvocv.sHtML

[R58] 下载文件
来源：http://blog.vehdjk.com/Article/details/gflnhzegy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.sjlbkw.cn/Article/details/gbwcwbuvl.sHtML

[R59] 发 POST JSON
来源：http://baike.bbcook.cn/Article/details/gnyslekyt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.vehdjk.com/Article/details/gamnpwsru.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.epnwcf.com/Article/details/gixrddiui.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.sjlbkw.cn/Article/details/gxwtyejzd.sHtML

[R61] 磁盘占用
来源：http://www.m.share.bbcook.cn/Article/details/gdsnnaltp.sHtML

df -h;  du -sh *
来源：http://wap.vehdjk.com/Article/details/gtpkzczft.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.vehdjk.com/Article/details/gynfrnuke.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fktsv.cn/Article/details/gmbcaqjym.sHtML

[R63] 内存与进程
来源：http://www.blog.tarul.cn/Article/details/grsawqhsy.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.bbcook.cn/Article/details/ggfadchpx.sHtML

[R64] 结束进程
来源：http://baike.fktsv.cn/Article/details/gbusbdopn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.tarul.cn/Article/details/gkplonpuj.sHtML

[R65] 查看端口占用
来源：http://blog.sjlbkw.cn/Article/details/gttbjpqde.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.tarul.cn/Article/details/gagqxwuew.sHtML

[R66] 定时任务
来源：http://www.share.vehdjk.com/Article/details/gwpdbyfjp.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.epnwcf.com/Article/details/glmeordcf.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.epnwcf.com/Article/details/gtsarazvm.sHtML

openssl rand -hex 16
来源：http://read.share.bbcook.cn/Article/details/ghjjixjjz.sHtML

[R68] 计算文件校验值
来源：http://wap.bbcook.cn/Article/details/gfsceepeg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.sjlbkw.cn/Article/details/gzuluesev.sHtML

[R69] 生成随机密码
来源：http://wap.tarul.cn/Article/details/gorgtgoat.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.sjlbkw.cn/Article/details/ggemgqrov.sHtML

[R70] 时间戳与互转
来源：http://baike.tarul.cn/Article/details/gsqakaten.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.bbcook.cn/Article/details/gucxhkwwr.sHtML

[R71] 日期格式化
来源：http://read.share.epnwcf.com/Article/details/gzcpojkox.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.vehdjk.com/Article/details/gftazjsqe.sHtML

[R72] 等待端口就绪
来源：http://www.share.tarul.cn/Article/details/gtivvdbdt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.tarul.cn/Article/details/ghbiptovv.sHtML

[R73] 分割大日志
来源：http://baike.vehdjk.com/Article/details/gjoviqivp.sHtML

split -l 1000 big.log part_
来源：http://mobile.tarul.cn/Article/details/gcejfhave.sHtML

[R74] 批量重命名
来源：http://read.share.vehdjk.com/Article/details/gtyqsqbyh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.yfazqb.com/Article/details/gjhikvnxp.sHtML

[R75] 导出环境变量
来源：http://mobile.tarul.cn/Article/details/gauzedujf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.tarul.cn/Article/details/gabgthcxn.sHtML

[R76] 使用临时文件
来源：http://blog.sjlbkw.cn/Article/details/gavbihtmy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fktsv.cn/Article/details/gapbvhnfq.sHtML

[R77] 读取用户输入
来源：http://3g.sjlbkw.cn/Article/details/gbhnlyhff.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fktsv.cn/Article/details/gvmhgzijn.sHtML

[R78] 交互式菜单
来源：http://www.blog.bbcook.cn/Article/details/grffecgwl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.vehdjk.com/Article/details/gthfvtaiu.sHtML

[R79] 解析命令行选项
来源：http://mobile.epnwcf.com/Article/details/gqeofdfpl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fktsv.cn/Article/details/gmmgxgsmq.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.bbcook.cn/Article/details/goaainycg.sHtML

time ./run.sh
来源：http://www.m.share.bbcook.cn/Article/details/gjumdkbur.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gmglqjyxu.sHtML

S. C / C++ 专题
来源：http://baike.tarul.cn/Article/details/gsfhrigoa.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gfvckkoad.sHtML

[S01] C：Hello World
来源：http://m.share.bbcook.cn/Article/details/gvrsjbebm.sHtML

#include <stdio.h>
来源：http://mobile.vehdjk.com/Article/details/grrgckend.sHtML


<!-- 参考信息 -->