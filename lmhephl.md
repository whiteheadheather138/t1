代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.tarul.cn/Article/details/gndxoeeza.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.vehdjk.com/Article/details/ggfgeiiks.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.vehdjk.com/Article/details/gdnvrmgbe.sHtML

[Q41] 多表连接
来源：http://baike.fktsv.cn/Article/details/gzmgwgkma.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.epnwcf.com/Article/details/gapcgkdsp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.bbcook.cn/Article/details/gqevnhogh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.tarul.cn/Article/details/glsgjfyqb.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fktsv.cn/Article/details/gshgsbamq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.vehdjk.com/Article/details/govvfolbu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.sjlbkw.cn/Article/details/gyrhstqsd.sHtML

[Q43] 标量子查询
来源：http://read.share.tarul.cn/Article/details/giopwoeve.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.tarul.cn/Article/details/gnaxegqol.sHtML

[Q44] IN 子查询
来源：http://mobile.yfazqb.com/Article/details/gfrzxcyxb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.yfazqb.com/Article/details/gavybayda.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.epnwcf.com/Article/details/gffaphsbv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.bbcook.cn/Article/details/goajcvhyw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.tarul.cn/Article/details/gvfmskxat.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.yfazqb.com/Article/details/glptbxxkc.sHtML

[Q47] 与平均值比较
来源：http://read.share.tarul.cn/Article/details/gvmmjtaiy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.sjlbkw.cn/Article/details/glfdwnpta.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.vehdjk.com/Article/details/goftoahbm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fktsv.cn/Article/details/gdiskxxje.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.epnwcf.com/Article/details/gsqoialgy.sHtML

[Q49] 更新单行
来源：http://mobile.yfazqb.com/Article/details/gqtkionag.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fktsv.cn/Article/details/gfbusnjbv.sHtML

[Q50] 批量更新
来源：http://www.blog.epnwcf.com/Article/details/garlowgkw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fktsv.cn/Article/details/gfidlweip.sHtML

[Q51] 用子查询更新
来源：http://wap.yfazqb.com/Article/details/gckgvoisg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.epnwcf.com/Article/details/gdclxcusf.sHtML

[Q52] 删除指定行
来源：http://wap.yfazqb.com/Article/details/gajvfihld.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.bbcook.cn/Article/details/gxazwjptd.sHtML

[Q53] 按条件删除
来源：http://read.share.sjlbkw.cn/Article/details/grufotxvf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.bbcook.cn/Article/details/gfroegxqq.sHtML

[Q54] 清空表
来源：http://blog.fktsv.cn/Article/details/gsnhqrxeo.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.sjlbkw.cn/Article/details/gcivyksns.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fktsv.cn/Article/details/goleozime.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.epnwcf.com/Article/details/gehlwfhyc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.bbcook.cn/Article/details/ggdfbrgvh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.yfazqb.com/Article/details/gsnocozkl.sHtML

[Q57] 行号
来源：http://www.m.share.bbcook.cn/Article/details/gntupzxea.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.epnwcf.com/Article/details/gwmfjjfqf.sHtML

[Q58] 累计求和
来源：http://3g.vehdjk.com/Article/details/gcosryita.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.bbcook.cn/Article/details/gnqczdbei.sHtML

[Q59] 分组内累计
来源：http://blog.yfazqb.com/Article/details/gzwnrttfl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.epnwcf.com/Article/details/gztbkmprm.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.tarul.cn/Article/details/gqzpadzon.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.yfazqb.com/Article/details/gqscdsidt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.epnwcf.com/Article/details/grbkgbrai.sHtML

[Q61] 移动平均
来源：http://www.blog.bbcook.cn/Article/details/gqukgdbst.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fktsv.cn/Article/details/gdygwaubw.sHtML

[Q62] 分组占比
来源：http://baike.bbcook.cn/Article/details/gsriijmer.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fktsv.cn/Article/details/grsxcgoon.sHtML

[Q63] 开启事务
来源：http://www.share.vehdjk.com/Article/details/gqqfdtstu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.epnwcf.com/Article/details/gfvrxczmo.sHtML

[Q64] 提交事务
来源：http://mobile.sjlbkw.cn/Article/details/gjqpwlfcm.sHtML

COMMIT;
来源：http://mobile.tarul.cn/Article/details/gntcbrygc.sHtML

[Q65] 回滚事务
来源：http://wap.vehdjk.com/Article/details/gsfqxugnu.sHtML

ROLLBACK;
来源：http://m.share.epnwcf.com/Article/details/gvgmgljah.sHtML

[Q66] 行锁查询
来源：http://read.share.epnwcf.com/Article/details/gfpkpkxed.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fktsv.cn/Article/details/goqzrzapt.sHtML

[Q67] 设置隔离级别
来源：http://baike.vehdjk.com/Article/details/gnlqzoazk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.tarul.cn/Article/details/gvdbwubjx.sHtML

[Q68] 保存点
来源：http://blog.fktsv.cn/Article/details/gdzusjoez.sHtML

SAVEPOINT sp1;
来源：http://mobile.fktsv.cn/Article/details/gupjfucfo.sHtML

ROLLBACK TO sp1;
来源：http://blog.bbcook.cn/Article/details/gtnymojdf.sHtML

[Q69] 查看执行计划
来源：http://wap.tarul.cn/Article/details/gcqtbcgzf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.tarul.cn/Article/details/gxihedlok.sHtML

[Q70] 更新统计信息
来源：http://www.blog.tarul.cn/Article/details/gvynhtrod.sHtML

ANALYZE TABLE users;
来源：http://read.share.bbcook.cn/Article/details/gbggufbam.sHtML

[Q71] 查看建表语句
来源：http://baike.bbcook.cn/Article/details/gxftyobls.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.sjlbkw.cn/Article/details/gxioqzrti.sHtML

[Q72] 查看索引
来源：http://wap.vehdjk.com/Article/details/gdcvpeshx.sHtML

SHOW INDEX FROM users;
来源：http://read.share.epnwcf.com/Article/details/gceyblcgs.sHtML

[Q73] 查看表状态
来源：http://m.share.bbcook.cn/Article/details/gwqbvduia.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.tarul.cn/Article/details/gpilzwuou.sHtML

[Q74] 强制使用索引
来源：http://www.blog.bbcook.cn/Article/details/gtvlluvdd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.yfazqb.com/Article/details/gqhjmswrm.sHtML

[Q75] 日期格式化
来源：http://m.share.bbcook.cn/Article/details/gqcfhuyje.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gumxpfuoy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.sjlbkw.cn/Article/details/gaeejilmd.sHtML

[Q76] 按天统计
来源：http://mobile.yfazqb.com/Article/details/gijsccdhk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.sjlbkw.cn/Article/details/gpnoedahg.sHtML

[Q77] 时间加减
来源：http://www.share.epnwcf.com/Article/details/ggspepuqi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fktsv.cn/Article/details/glpdxblaa.sHtML

[Q78] 当前时间
来源：http://wap.epnwcf.com/Article/details/gdrjijqim.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.tarul.cn/Article/details/gkwjztqpv.sHtML

[Q79] 字符串拼接
来源：http://www.blog.tarul.cn/Article/details/gwuqwyokw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fktsv.cn/Article/details/gdcbentgi.sHtML

[Q80] 字符串截取
来源：http://www.blog.tarul.cn/Article/details/gbfjlukdr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.yfazqb.com/Article/details/gfcovygdy.sHtML

[Q81] 字符串替换
来源：http://wap.tarul.cn/Article/details/gjvfwbzwr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.tarul.cn/Article/details/gpxtchuco.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.yfazqb.com/Article/details/giqtjytde.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gwgxjhana.sHtML

[Q83] 大小写转换
来源：http://read.share.bbcook.cn/Article/details/gcfizbjbx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gonlncvuj.sHtML

[Q84] 去除首尾空格
来源：http://blog.fktsv.cn/Article/details/gaqmuagav.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gordbesdi.sHtML

[Q85] 数值取整
来源：http://www.share.bbcook.cn/Article/details/gamuriyms.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.epnwcf.com/Article/details/gcyuilgrk.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.bbcook.cn/Article/details/guohoikiv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fktsv.cn/Article/details/gdlcinpjo.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.bbcook.cn/Article/details/gssqdivtw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.sjlbkw.cn/Article/details/gzfqfotsg.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.sjlbkw.cn/Article/details/guxoqpzxp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.sjlbkw.cn/Article/details/gtchjzegh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fktsv.cn/Article/details/gjkrlkbqv.sHtML

[Q89] 判断表是否存在
来源：http://wap.fktsv.cn/Article/details/gkobhcsqw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.epnwcf.com/Article/details/ghractled.sHtML

[Q90] 生成序号列
来源：http://www.share.fktsv.cn/Article/details/gncsmqyru.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.epnwcf.com/Article/details/ggxbqfjpo.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gujapjuoz.sHtML

R. Bash 专题
来源：http://blog.epnwcf.com/Article/details/gilhajbja.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gajemhijp.sHtML

[R01] shebang 与严格模式
来源：http://www.share.bbcook.cn/Article/details/gaglvlglw.sHtML

#!/usr/bin/env bash
来源：http://www.share.fktsv.cn/Article/details/gnatnrpcl.sHtML

set -euo pipefail
来源：http://blog.epnwcf.com/Article/details/grbggdkxs.sHtML

[R02] 变量赋值与使用
来源：http://baike.vehdjk.com/Article/details/gasgkvvhg.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fktsv.cn/Article/details/gokwdibpa.sHtML

[R03] 只读变量
来源：http://blog.epnwcf.com/Article/details/gonkzgoem.sHtML

readonly PI=3.14
来源：http://m.share.tarul.cn/Article/details/gwovouisu.sHtML

[R04] 位置参数
来源：http://blog.vehdjk.com/Article/details/gcggqaopt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.epnwcf.com/Article/details/gennxwcnf.sHtML

[R05] 参数默认值
来源：http://www.m.share.sjlbkw.cn/Article/details/gncglexnx.sHtML

name="${1:-default}"
来源：http://blog.yfazqb.com/Article/details/gujzksqsw.sHtML

[R06] 判断命令是否存在
来源：http://3g.epnwcf.com/Article/details/gmyqfyswf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.yfazqb.com/Article/details/gnfhswrwz.sHtML

[R07] if 判断文件
来源：http://baike.epnwcf.com/Article/details/gtvakjfqk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.bbcook.cn/Article/details/gippwgkbd.sHtML

[R08] 数值比较
来源：http://www.share.tarul.cn/Article/details/gpzwoyqeo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fktsv.cn/Article/details/gwsxmakjb.sHtML

[R09] 字符串比较
来源：http://mobile.epnwcf.com/Article/details/gqvliwpcy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.yfazqb.com/Article/details/ggppeiqmq.sHtML

[R10] 正则匹配
来源：http://mobile.tarul.cn/Article/details/ggebrognp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.sjlbkw.cn/Article/details/gzalryjoc.sHtML

[R11] case 多分支
来源：http://3g.epnwcf.com/Article/details/gdlnkihie.sHtML

case "$1" in
来源：http://www.share.tarul.cn/Article/details/gockrkryq.sHtML

start) echo "启动" ;;
来源：http://m.share.tarul.cn/Article/details/gshkguswp.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fktsv.cn/Article/details/gsrjbrzvt.sHtML

*)     echo "未知命令" ;;
来源：http://blog.bbcook.cn/Article/details/grbstdbww.sHtML

esac
来源：http://3g.bbcook.cn/Article/details/gxgjgohoi.sHtML

[R12] for 遍历文件
来源：http://baike.yfazqb.com/Article/details/gyuperjfu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.vehdjk.com/Article/details/gngntmznc.sHtML

[R13] for 计数循环
来源：http://www.share.vehdjk.com/Article/details/ggbvqfaex.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.yfazqb.com/Article/details/gpnaleorl.sHtML

[R14] C 风格 for
来源：http://wap.sjlbkw.cn/Article/details/gfsaprxxj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.vehdjk.com/Article/details/gwgciorbi.sHtML

[R15] while 逐行读文件
来源：http://m.share.bbcook.cn/Article/details/gpsfhvafz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.tarul.cn/Article/details/gmpdogjne.sHtML

[R16] until 等待条件
来源：http://www.m.share.tarul.cn/Article/details/ghdfxdcgp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.epnwcf.com/Article/details/ghxeqigag.sHtML

[R17] 数组定义与取值
来源：http://3g.bbcook.cn/Article/details/gluhnhhhf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.yfazqb.com/Article/details/gknqpmwpu.sHtML

[R18] 遍历数组
来源：http://read.share.tarul.cn/Article/details/galnjmkxx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.bbcook.cn/Article/details/gppkjygcx.sHtML

[R19] 数组长度
来源：http://3g.epnwcf.com/Article/details/gpboawium.sHtML

echo "${#arr[@]}"
来源：http://blog.yfazqb.com/Article/details/gevtaqhvr.sHtML

[R20] 关联数组（字典）
来源：http://www.share.vehdjk.com/Article/details/golvnaogq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.epnwcf.com/Article/details/gzcvkurxm.sHtML

[R21] 字符串长度
来源：http://wap.epnwcf.com/Article/details/gdlgobooy.sHtML

echo "${#s}"
来源：http://baike.epnwcf.com/Article/details/gzfxgyfkl.sHtML

[R22] 截取子串
来源：http://mobile.fktsv.cn/Article/details/goqekemro.sHtML

echo "${s:0:5}"
来源：http://read.share.tarul.cn/Article/details/grwwofzhw.sHtML

[R23] 字符串替换
来源：http://3g.yfazqb.com/Article/details/gcaykazab.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.tarul.cn/Article/details/gbascbdhy.sHtML

[R24] 大小写转换
来源：http://3g.sjlbkw.cn/Article/details/gftdrhqme.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.sjlbkw.cn/Article/details/gxjdvvqwx.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.vehdjk.com/Article/details/gpsvuytbx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.bbcook.cn/Article/details/gzqhpdzxn.sHtML

[R26] 命令替换
来源：http://blog.sjlbkw.cn/Article/details/grfwcodvk.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.epnwcf.com/Article/details/gnwtsahbe.sHtML

[R27] 算术展开
来源：http://m.share.sjlbkw.cn/Article/details/gqqohukaf.sHtML

echo $((1 + 2 * 3))
来源：http://blog.vehdjk.com/Article/details/gofoiaplp.sHtML

[R28] 浮点运算
来源：http://m.share.yfazqb.com/Article/details/glfkhvtsn.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.epnwcf.com/Article/details/gifjzjpbc.sHtML

[R29] 定义函数
来源：http://mobile.sjlbkw.cn/Article/details/geubywlmt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.sjlbkw.cn/Article/details/gwxeeygoa.sHtML

[R30] 函数返回状态码
来源：http://baike.yfazqb.com/Article/details/gkuaihhvi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fktsv.cn/Article/details/gqsfheigl.sHtML

[R31] 局部变量
来源：http://wap.fktsv.cn/Article/details/gvtgyvpld.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.sjlbkw.cn/Article/details/giedqjduz.sHtML

[R32] 参数个数校验
来源：http://read.share.bbcook.cn/Article/details/gkurveoqq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.yfazqb.com/Article/details/glqnvaxdn.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.bbcook.cn/Article/details/gdtrhyyhx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.tarul.cn/Article/details/ggzshawvs.sHtML

[R34] 退出时清理
来源：http://3g.epnwcf.com/Article/details/gdmxysuvd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.sjlbkw.cn/Article/details/gvmoqxnzq.sHtML

[R35] 后台执行并等待
来源：http://wap.bbcook.cn/Article/details/gnzrxpwrr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fktsv.cn/Article/details/gqjtkyrhv.sHtML

[R36] 并发执行多个任务
来源：http://read.share.epnwcf.com/Article/details/gphjpfqfz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.bbcook.cn/Article/details/gsoicjeta.sHtML

[R37] 把输出赋给变量
来源：http://baike.fktsv.cn/Article/details/gdbfbufok.sHtML

files=$(ls -1)
来源：http://www.share.vehdjk.com/Article/details/gbzaxgotz.sHtML

[R38] 管道串联
来源：http://baike.vehdjk.com/Article/details/gboqiurbc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fktsv.cn/Article/details/gfqrbybya.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.epnwcf.com/Article/details/ggperswhx.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.vehdjk.com/Article/details/gohqdrctu.sHtML

[R40] 追加写日志
来源：http://read.share.vehdjk.com/Article/details/gmefboins.sHtML

echo "log" >> out.log
来源：http://read.share.fktsv.cn/Article/details/gulmtuspq.sHtML

[R41] 丢弃输出
来源：http://3g.yfazqb.com/Article/details/gprygukzg.sHtML

cmd >/dev/null 2>&1
来源：http://blog.tarul.cn/Article/details/gkptbyueo.sHtML

[R42] 输入重定向
来源：http://3g.yfazqb.com/Article/details/gyabqzjpg.sHtML

wc -l < a.txt
来源：http://www.m.share.epnwcf.com/Article/details/gapyjtcoe.sHtML

[R43] 按名字查找文件
来源：http://m.share.epnwcf.com/Article/details/guayaoehf.sHtML

find . -name "*.log" -type f
来源：http://wap.epnwcf.com/Article/details/gksohcgqr.sHtML

[R44] 按修改时间查找
来源：http://read.share.fktsv.cn/Article/details/ghzukcuur.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.sjlbkw.cn/Article/details/gshjgjtbs.sHtML

[R45] 批量删除
来源：http://mobile.sjlbkw.cn/Article/details/gvtjtuhst.sHtML

find . -name "*.tmp" -delete
来源：http://baike.sjlbkw.cn/Article/details/gczcxdeuc.sHtML

[R46] 递归替换文件内容
来源：http://wap.vehdjk.com/Article/details/ghagssvcz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.sjlbkw.cn/Article/details/glauiqgam.sHtML

[R47] sed 单行替换
来源：http://blog.sjlbkw.cn/Article/details/gisgawpbx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.bbcook.cn/Article/details/gbhbyqwhd.sHtML

[R48] awk 取指定列
来源：http://3g.yfazqb.com/Article/details/gmciegeob.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.yfazqb.com/Article/details/gtfhmqpkp.sHtML

[R49] awk 带条件
来源：http://mobile.fktsv.cn/Article/details/gfewcshet.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.sjlbkw.cn/Article/details/gjvkhnkaz.sHtML

[R50] awk 求和
来源：http://baike.tarul.cn/Article/details/gdkkzamwh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.yfazqb.com/Article/details/gbvqpglxz.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.tarul.cn/Article/details/gtlsmjglo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.bbcook.cn/Article/details/gqhozsjxl.sHtML

[R52] 统计行数
来源：http://baike.tarul.cn/Article/details/gnccdzfrm.sHtML

wc -l a.txt
来源：http://3g.sjlbkw.cn/Article/details/geqkpnofh.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.bbcook.cn/Article/details/gbejijauf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fktsv.cn/Article/details/gywrcttnk.sHtML

[R54] 比较两个文件
来源：http://www.m.share.bbcook.cn/Article/details/gakrbazky.sHtML

diff a.txt b.txt
来源：http://wap.bbcook.cn/Article/details/gqjhjqddu.sHtML

[R55] 压缩与解压
来源：http://www.m.share.bbcook.cn/Article/details/gsijeetln.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.yfazqb.com/Article/details/gyfswhvsf.sHtML

[R56] 远程拷贝
来源：http://read.share.bbcook.cn/Article/details/globctktf.sHtML

scp file user@host:/path/
来源：http://read.share.bbcook.cn/Article/details/gdxciwszp.sHtML

[R57] 远程执行命令
来源：http://m.share.vehdjk.com/Article/details/gcegwmzru.sHtML

ssh user@host 'uptime'
来源：http://3g.yfazqb.com/Article/details/gczivbsod.sHtML

[R58] 下载文件
来源：http://www.blog.yfazqb.com/Article/details/gnfvtmmpp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.sjlbkw.cn/Article/details/guywqmlqx.sHtML

[R59] 发 POST JSON
来源：http://m.share.tarul.cn/Article/details/gncnukxdy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.yfazqb.com/Article/details/gxlkpzrpv.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.bbcook.cn/Article/details/gcvwlpqhf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.vehdjk.com/Article/details/giwqsadhr.sHtML

[R61] 磁盘占用
来源：http://www.m.share.vehdjk.com/Article/details/gfgyrqxtd.sHtML

df -h;  du -sh *
来源：http://www.blog.fktsv.cn/Article/details/gtsmqrubw.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.epnwcf.com/Article/details/gfzdvbsrd.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.bbcook.cn/Article/details/gxhutaysn.sHtML

[R63] 内存与进程
来源：http://3g.vehdjk.com/Article/details/gprbawcez.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.sjlbkw.cn/Article/details/gyrcmddjy.sHtML

[R64] 结束进程
来源：http://www.m.share.fktsv.cn/Article/details/gmwidrtfh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.epnwcf.com/Article/details/gnngvjmdd.sHtML

[R65] 查看端口占用
来源：http://www.blog.fktsv.cn/Article/details/glnapstug.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.sjlbkw.cn/Article/details/glqqngyph.sHtML

[R66] 定时任务
来源：http://wap.sjlbkw.cn/Article/details/gwdypriaq.sHtML

crontab -e;  crontab -l
来源：http://m.share.sjlbkw.cn/Article/details/gjhztntic.sHtML

[R67] 生成随机十六进制串
来源：http://baike.epnwcf.com/Article/details/gqsbelouz.sHtML

openssl rand -hex 16
来源：http://baike.tarul.cn/Article/details/gnhcnldnt.sHtML

[R68] 计算文件校验值
来源：http://mobile.yfazqb.com/Article/details/gigbbdmax.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.tarul.cn/Article/details/gcmtibsby.sHtML

[R69] 生成随机密码
来源：http://baike.epnwcf.com/Article/details/gjgbgcrxn.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fktsv.cn/Article/details/gnqgenayh.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.epnwcf.com/Article/details/gccqlfhvo.sHtML

date +%s;  date -d @1700000000
来源：http://baike.sjlbkw.cn/Article/details/glywtknfp.sHtML

[R71] 日期格式化
来源：http://baike.bbcook.cn/Article/details/gqghsfcxp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.vehdjk.com/Article/details/gswvudvoo.sHtML

[R72] 等待端口就绪
来源：http://baike.yfazqb.com/Article/details/gtekkgipk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fktsv.cn/Article/details/ggutwyifa.sHtML

[R73] 分割大日志
来源：http://www.blog.tarul.cn/Article/details/gccjibjjv.sHtML

split -l 1000 big.log part_
来源：http://wap.tarul.cn/Article/details/ggatwrmzs.sHtML

[R74] 批量重命名
来源：http://wap.tarul.cn/Article/details/gkubsqmqi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.vehdjk.com/Article/details/gymnubwnj.sHtML

[R75] 导出环境变量
来源：http://m.share.sjlbkw.cn/Article/details/gjgacosqt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.yfazqb.com/Article/details/grnxxrete.sHtML

[R76] 使用临时文件
来源：http://baike.sjlbkw.cn/Article/details/gelgwychv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fktsv.cn/Article/details/gcmgmludb.sHtML

[R77] 读取用户输入
来源：http://m.share.bbcook.cn/Article/details/gqzvrymgn.sHtML

read -rp "请输入: " ans
来源：http://m.share.tarul.cn/Article/details/gpjvgkhag.sHtML

[R78] 交互式菜单
来源：http://3g.vehdjk.com/Article/details/gbhmkxgcu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.vehdjk.com/Article/details/gdvkybzww.sHtML

[R79] 解析命令行选项
来源：http://mobile.yfazqb.com/Article/details/gxpihvsjk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.vehdjk.com/Article/details/grlteyypq.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.bbcook.cn/Article/details/gvbcihmxz.sHtML

time ./run.sh
来源：http://read.share.sjlbkw.cn/Article/details/gpbeizwnt.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gedmblguo.sHtML

S. C / C++ 专题
来源：http://read.share.bbcook.cn/Article/details/gnmcffcnu.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gxgreamyo.sHtML

[S01] C：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gbpujcote.sHtML

#include <stdio.h>
来源：http://baike.vehdjk.com/Article/details/gwydkvnfy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fktsv.cn/Article/details/gbtahvkht.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.vehdjk.com/Article/details/grsldedhb.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.tarul.cn/Article/details/gwozhbwgb.sHtML

[S03] C：读入整数
来源：http://baike.vehdjk.com/Article/details/glrctossc.sHtML

int x; scanf("%d", &x);
来源：http://blog.tarul.cn/Article/details/gedxlrdsh.sHtML

[S04] C：字符串复制
来源：http://3g.vehdjk.com/Article/details/gsdwuubeg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.tarul.cn/Article/details/gyfislpsz.sHtML

[S05] C：字符串长度
来源：http://wap.yfazqb.com/Article/details/gppxvowwc.sHtML

strlen(s)
来源：http://m.share.tarul.cn/Article/details/gmofhubru.sHtML

[S06] C：字符串比较
来源：http://baike.yfazqb.com/Article/details/gyjekipbe.sHtML

strcmp(a, b) == 0
来源：http://www.share.bbcook.cn/Article/details/gaqzcgkax.sHtML

[S07] C：数组遍历求和
来源：http://blog.sjlbkw.cn/Article/details/gabyjbpbn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.bbcook.cn/Article/details/gjunaramq.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.tarul.cn/Article/details/gtvznlohp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.vehdjk.com/Article/details/gykeuwohz.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.yfazqb.com/Article/details/gycsixlvw.sHtML


<!-- 参考信息 -->