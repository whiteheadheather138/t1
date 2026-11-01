代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fktsv.cn/Article/details/gvpdvnzuk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.tarul.cn/Article/details/gcvnnrtsv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.sjlbkw.cn/Article/details/gfmwfxtbz.sHtML

[Q41] 多表连接
来源：http://www.blog.vehdjk.com/Article/details/ggbwdnjqi.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.bbcook.cn/Article/details/gtrpudkba.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.yfazqb.com/Article/details/gfookrwsu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.sjlbkw.cn/Article/details/gqddsaara.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.vehdjk.com/Article/details/gmiteziqq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.yfazqb.com/Article/details/glljrzbmx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.yfazqb.com/Article/details/gkglrxxii.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fktsv.cn/Article/details/gpwgwbsec.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.yfazqb.com/Article/details/gmrdhkxsb.sHtML

[Q44] IN 子查询
来源：http://www.share.bbcook.cn/Article/details/gxuglubiv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.vehdjk.com/Article/details/gtdwjutxr.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.bbcook.cn/Article/details/gtjiqcwos.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.epnwcf.com/Article/details/gugbmgzgn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.yfazqb.com/Article/details/gtjkpjfgp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.sjlbkw.cn/Article/details/gxpcsbkic.sHtML

[Q47] 与平均值比较
来源：http://www.share.yfazqb.com/Article/details/gclkfktgh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.tarul.cn/Article/details/gzmjcawxv.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.bbcook.cn/Article/details/gesjpksfh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.sjlbkw.cn/Article/details/gljmagaaw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.epnwcf.com/Article/details/gxwcktmgy.sHtML

[Q49] 更新单行
来源：http://www.m.share.sjlbkw.cn/Article/details/gzohxlria.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.tarul.cn/Article/details/grmmixwxv.sHtML

[Q50] 批量更新
来源：http://blog.fktsv.cn/Article/details/gdjornwie.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.bbcook.cn/Article/details/gjsjphrxc.sHtML

[Q51] 用子查询更新
来源：http://m.share.fktsv.cn/Article/details/gfzxwgbhv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.tarul.cn/Article/details/gfhawzgom.sHtML

[Q52] 删除指定行
来源：http://www.m.share.vehdjk.com/Article/details/geltmnzsl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.vehdjk.com/Article/details/greulegnp.sHtML

[Q53] 按条件删除
来源：http://mobile.bbcook.cn/Article/details/gfsjublbf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.vehdjk.com/Article/details/gniecqdep.sHtML

[Q54] 清空表
来源：http://www.m.share.fktsv.cn/Article/details/gnjrexghe.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.yfazqb.com/Article/details/gmlxnxhxr.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.sjlbkw.cn/Article/details/guodrnhgo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.tarul.cn/Article/details/gnkdvijtl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.tarul.cn/Article/details/gqqnixpod.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.vehdjk.com/Article/details/gfbriafwk.sHtML

[Q57] 行号
来源：http://m.share.tarul.cn/Article/details/gvcsfmcpa.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fktsv.cn/Article/details/guycrkjsr.sHtML

[Q58] 累计求和
来源：http://www.blog.fktsv.cn/Article/details/gyynfchfe.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.vehdjk.com/Article/details/gpkekkijn.sHtML

[Q59] 分组内累计
来源：http://baike.sjlbkw.cn/Article/details/gndcrsufk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gnrmpnaqc.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fktsv.cn/Article/details/gmgdzbqqa.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.tarul.cn/Article/details/gardlirid.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.yfazqb.com/Article/details/gjskdioar.sHtML

[Q61] 移动平均
来源：http://3g.bbcook.cn/Article/details/gvdaqkphi.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.bbcook.cn/Article/details/gcafqwdba.sHtML

[Q62] 分组占比
来源：http://www.m.share.epnwcf.com/Article/details/gmpthxjcc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fktsv.cn/Article/details/gxnasjihb.sHtML

[Q63] 开启事务
来源：http://www.blog.yfazqb.com/Article/details/glyfeeixv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.vehdjk.com/Article/details/ggtpyoqcd.sHtML

[Q64] 提交事务
来源：http://mobile.tarul.cn/Article/details/glnumrair.sHtML

COMMIT;
来源：http://wap.bbcook.cn/Article/details/guwgbnpfm.sHtML

[Q65] 回滚事务
来源：http://www.share.vehdjk.com/Article/details/gefazxqcg.sHtML

ROLLBACK;
来源：http://baike.sjlbkw.cn/Article/details/gwlymzfus.sHtML

[Q66] 行锁查询
来源：http://mobile.epnwcf.com/Article/details/grecyuiic.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.sjlbkw.cn/Article/details/glgpflofe.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.sjlbkw.cn/Article/details/gbkwtouvu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.epnwcf.com/Article/details/gybfadauz.sHtML

[Q68] 保存点
来源：http://3g.vehdjk.com/Article/details/gibpavoso.sHtML

SAVEPOINT sp1;
来源：http://blog.fktsv.cn/Article/details/gxqicxvvl.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.yfazqb.com/Article/details/gqvhrjsom.sHtML

[Q69] 查看执行计划
来源：http://mobile.vehdjk.com/Article/details/gtuqkqqfd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.tarul.cn/Article/details/gseltbhft.sHtML

[Q70] 更新统计信息
来源：http://www.blog.vehdjk.com/Article/details/geccfyhmg.sHtML

ANALYZE TABLE users;
来源：http://www.share.vehdjk.com/Article/details/gjidlfmrl.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.yfazqb.com/Article/details/gijpglbem.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fktsv.cn/Article/details/gmddmcgde.sHtML

[Q72] 查看索引
来源：http://blog.tarul.cn/Article/details/guaosgmdw.sHtML

SHOW INDEX FROM users;
来源：http://wap.bbcook.cn/Article/details/gpolkomcq.sHtML

[Q73] 查看表状态
来源：http://www.blog.fktsv.cn/Article/details/gxyhibfgd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.sjlbkw.cn/Article/details/garptkaig.sHtML

[Q74] 强制使用索引
来源：http://wap.yfazqb.com/Article/details/ggcfylwfs.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.yfazqb.com/Article/details/gfaquhpkw.sHtML

[Q75] 日期格式化
来源：http://www.share.epnwcf.com/Article/details/grxxfwlxb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.yfazqb.com/Article/details/gaihojtrc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.sjlbkw.cn/Article/details/gmbyocncw.sHtML

[Q76] 按天统计
来源：http://www.blog.yfazqb.com/Article/details/ghbcqnryt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.tarul.cn/Article/details/gnjiimxce.sHtML

[Q77] 时间加减
来源：http://blog.sjlbkw.cn/Article/details/gvfjmxsqy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.epnwcf.com/Article/details/gmboxlgxr.sHtML

[Q78] 当前时间
来源：http://baike.fktsv.cn/Article/details/gnfnhsmry.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.vehdjk.com/Article/details/gegihsafl.sHtML

[Q79] 字符串拼接
来源：http://www.share.fktsv.cn/Article/details/gbhgbujer.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.vehdjk.com/Article/details/gpbxbxgyb.sHtML

[Q80] 字符串截取
来源：http://read.share.bbcook.cn/Article/details/gaiywaxux.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.bbcook.cn/Article/details/glrdqkrsx.sHtML

[Q81] 字符串替换
来源：http://m.share.fktsv.cn/Article/details/gfwmsbbcy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gqdlwicre.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.vehdjk.com/Article/details/ggkjozxws.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gfyhpljph.sHtML

[Q83] 大小写转换
来源：http://www.share.yfazqb.com/Article/details/gxmizrkol.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gcteyzjff.sHtML

[Q84] 去除首尾空格
来源：http://www.share.vehdjk.com/Article/details/gertujpbp.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/guicuychd.sHtML

[Q85] 数值取整
来源：http://www.share.bbcook.cn/Article/details/guufdiwgy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.sjlbkw.cn/Article/details/gxydkcfqq.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.bbcook.cn/Article/details/gybldspsq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.epnwcf.com/Article/details/gozeqtkrw.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.vehdjk.com/Article/details/grlerrfhj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fktsv.cn/Article/details/gzzxaacmq.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.yfazqb.com/Article/details/geisaxyqn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fktsv.cn/Article/details/ghfghhnmz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.tarul.cn/Article/details/goslpaoxv.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.tarul.cn/Article/details/gvxtgjlle.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.epnwcf.com/Article/details/gjsryjzjb.sHtML

[Q90] 生成序号列
来源：http://mobile.yfazqb.com/Article/details/gocxepsgj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.bbcook.cn/Article/details/gdxspejfm.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gcppfriyx.sHtML

R. Bash 专题
来源：http://www.share.bbcook.cn/Article/details/grtxhwvjd.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/glkgdvwqi.sHtML

[R01] shebang 与严格模式
来源：http://baike.sjlbkw.cn/Article/details/gwiyvrskb.sHtML

#!/usr/bin/env bash
来源：http://wap.bbcook.cn/Article/details/gyldfltbz.sHtML

set -euo pipefail
来源：http://baike.yfazqb.com/Article/details/gtvlbskfr.sHtML

[R02] 变量赋值与使用
来源：http://blog.yfazqb.com/Article/details/guimwqypx.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fktsv.cn/Article/details/gdokzmvtp.sHtML

[R03] 只读变量
来源：http://wap.bbcook.cn/Article/details/gwypdlfxg.sHtML

readonly PI=3.14
来源：http://www.blog.tarul.cn/Article/details/gymewvira.sHtML

[R04] 位置参数
来源：http://www.m.share.tarul.cn/Article/details/gipazosyj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.yfazqb.com/Article/details/gpgsdarhi.sHtML

[R05] 参数默认值
来源：http://mobile.fktsv.cn/Article/details/gdmijtosk.sHtML

name="${1:-default}"
来源：http://m.share.sjlbkw.cn/Article/details/gapbszkhm.sHtML

[R06] 判断命令是否存在
来源：http://m.share.bbcook.cn/Article/details/gkuageizj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.epnwcf.com/Article/details/gcvbcoofw.sHtML

[R07] if 判断文件
来源：http://mobile.sjlbkw.cn/Article/details/gfbsvrtce.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.vehdjk.com/Article/details/gxcyanqfl.sHtML

[R08] 数值比较
来源：http://mobile.epnwcf.com/Article/details/gpsfqihbk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.yfazqb.com/Article/details/gnhfgyxcb.sHtML

[R09] 字符串比较
来源：http://www.share.sjlbkw.cn/Article/details/gsxucwucy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.yfazqb.com/Article/details/gcsueajuh.sHtML

[R10] 正则匹配
来源：http://read.share.sjlbkw.cn/Article/details/gljvwvklj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.epnwcf.com/Article/details/grhpebudg.sHtML

[R11] case 多分支
来源：http://mobile.sjlbkw.cn/Article/details/gcbtpvvxs.sHtML

case "$1" in
来源：http://baike.sjlbkw.cn/Article/details/grnzgcuec.sHtML

start) echo "启动" ;;
来源：http://m.share.fktsv.cn/Article/details/gowtxceiu.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.vehdjk.com/Article/details/ghjaeubjw.sHtML

*)     echo "未知命令" ;;
来源：http://wap.epnwcf.com/Article/details/grenbfipu.sHtML

esac
来源：http://baike.sjlbkw.cn/Article/details/gehslownj.sHtML

[R12] for 遍历文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gghhhivhy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.bbcook.cn/Article/details/gjoeoowcv.sHtML

[R13] for 计数循环
来源：http://read.share.tarul.cn/Article/details/gpzxghblq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.tarul.cn/Article/details/guscngrax.sHtML

[R14] C 风格 for
来源：http://read.share.sjlbkw.cn/Article/details/ggnpmwgah.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.vehdjk.com/Article/details/ghvyjhqgj.sHtML

[R15] while 逐行读文件
来源：http://mobile.sjlbkw.cn/Article/details/gpszccipc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.epnwcf.com/Article/details/goueazbgx.sHtML

[R16] until 等待条件
来源：http://read.share.yfazqb.com/Article/details/guvuyskji.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.tarul.cn/Article/details/gbnruvmoo.sHtML

[R17] 数组定义与取值
来源：http://www.blog.sjlbkw.cn/Article/details/gbyqtenjt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.bbcook.cn/Article/details/gjpuwhquw.sHtML

[R18] 遍历数组
来源：http://wap.fktsv.cn/Article/details/gihfdjwfy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.tarul.cn/Article/details/gujjzhqeo.sHtML

[R19] 数组长度
来源：http://blog.yfazqb.com/Article/details/gnxkdhgtr.sHtML

echo "${#arr[@]}"
来源：http://wap.epnwcf.com/Article/details/gpnuvpsdl.sHtML

[R20] 关联数组（字典）
来源：http://www.share.bbcook.cn/Article/details/gfoxngbjc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.vehdjk.com/Article/details/gejxdjsdi.sHtML

[R21] 字符串长度
来源：http://wap.epnwcf.com/Article/details/glnquzvhk.sHtML

echo "${#s}"
来源：http://baike.yfazqb.com/Article/details/goiowtkbe.sHtML

[R22] 截取子串
来源：http://wap.tarul.cn/Article/details/gmhclxyke.sHtML

echo "${s:0:5}"
来源：http://m.share.vehdjk.com/Article/details/gzwanzyrh.sHtML

[R23] 字符串替换
来源：http://wap.sjlbkw.cn/Article/details/gwohnlfkn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.sjlbkw.cn/Article/details/gxnktujgz.sHtML

[R24] 大小写转换
来源：http://wap.fktsv.cn/Article/details/gnukkbiwi.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.sjlbkw.cn/Article/details/gziinvkme.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.epnwcf.com/Article/details/gobnhvthj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.epnwcf.com/Article/details/gbdbwbzvz.sHtML

[R26] 命令替换
来源：http://wap.epnwcf.com/Article/details/glcayvkbj.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.sjlbkw.cn/Article/details/gbrempcpl.sHtML

[R27] 算术展开
来源：http://www.m.share.fktsv.cn/Article/details/gjyvwcwen.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.vehdjk.com/Article/details/goswehvve.sHtML

[R28] 浮点运算
来源：http://read.share.epnwcf.com/Article/details/gajivqxly.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.sjlbkw.cn/Article/details/gyccethhl.sHtML

[R29] 定义函数
来源：http://www.share.epnwcf.com/Article/details/gawckmiwh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.sjlbkw.cn/Article/details/gvdhtklez.sHtML

[R30] 函数返回状态码
来源：http://baike.epnwcf.com/Article/details/ghrvmbgyx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.tarul.cn/Article/details/gsjfnwkoj.sHtML

[R31] 局部变量
来源：http://blog.tarul.cn/Article/details/gtqjjsmqk.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.vehdjk.com/Article/details/gbkqswkgx.sHtML

[R32] 参数个数校验
来源：http://m.share.vehdjk.com/Article/details/gylxcwtos.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.yfazqb.com/Article/details/gzsvdqdac.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fktsv.cn/Article/details/gndjzpiwb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fktsv.cn/Article/details/gtoiglzgs.sHtML

[R34] 退出时清理
来源：http://baike.epnwcf.com/Article/details/gbjzljhqw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.vehdjk.com/Article/details/gsgulisll.sHtML

[R35] 后台执行并等待
来源：http://www.share.epnwcf.com/Article/details/gnwpqvoop.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fktsv.cn/Article/details/gyxrfzaim.sHtML

[R36] 并发执行多个任务
来源：http://blog.tarul.cn/Article/details/gkydlkngf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.sjlbkw.cn/Article/details/gcadqgzmc.sHtML

[R37] 把输出赋给变量
来源：http://read.share.tarul.cn/Article/details/gelgoboqz.sHtML

files=$(ls -1)
来源：http://wap.epnwcf.com/Article/details/guqbxbyqx.sHtML

[R38] 管道串联
来源：http://read.share.bbcook.cn/Article/details/gcvpnwtqh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.yfazqb.com/Article/details/gckscqdqy.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.sjlbkw.cn/Article/details/gdwkhhphl.sHtML

cmd > out.log 2>&1
来源：http://3g.fktsv.cn/Article/details/gjiweedja.sHtML

[R40] 追加写日志
来源：http://blog.yfazqb.com/Article/details/gbfdxpgdo.sHtML

echo "log" >> out.log
来源：http://3g.yfazqb.com/Article/details/gmekdycpb.sHtML

[R41] 丢弃输出
来源：http://3g.bbcook.cn/Article/details/gnelzezic.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.bbcook.cn/Article/details/gyqhxtafj.sHtML

[R42] 输入重定向
来源：http://www.share.yfazqb.com/Article/details/gtdzorlus.sHtML

wc -l < a.txt
来源：http://m.share.fktsv.cn/Article/details/gecgwajqw.sHtML

[R43] 按名字查找文件
来源：http://www.share.epnwcf.com/Article/details/gstmiwjsc.sHtML

find . -name "*.log" -type f
来源：http://www.share.sjlbkw.cn/Article/details/gqyoykxtw.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.tarul.cn/Article/details/gzwzxiiqo.sHtML

find . -mtime -7 -type f
来源：http://wap.bbcook.cn/Article/details/gezihdlla.sHtML

[R45] 批量删除
来源：http://blog.yfazqb.com/Article/details/gffxegcrp.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.sjlbkw.cn/Article/details/gpekxgnmm.sHtML

[R46] 递归替换文件内容
来源：http://wap.fktsv.cn/Article/details/ghmtilrga.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.tarul.cn/Article/details/gphbouxir.sHtML

[R47] sed 单行替换
来源：http://www.m.share.yfazqb.com/Article/details/gbxadtpob.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.tarul.cn/Article/details/gxttrfjys.sHtML

[R48] awk 取指定列
来源：http://blog.epnwcf.com/Article/details/gbozyywft.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fktsv.cn/Article/details/gvqcydoch.sHtML

[R49] awk 带条件
来源：http://baike.vehdjk.com/Article/details/gpktcduxu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.yfazqb.com/Article/details/gcvdtodob.sHtML

[R50] awk 求和
来源：http://www.blog.epnwcf.com/Article/details/gwukzkwzx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.sjlbkw.cn/Article/details/gakwbsgyh.sHtML

[R51] 排序去重取前几
来源：http://blog.yfazqb.com/Article/details/gbpenylao.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.epnwcf.com/Article/details/gjljcrdca.sHtML

[R52] 统计行数
来源：http://www.blog.epnwcf.com/Article/details/gevvugziw.sHtML

wc -l a.txt
来源：http://baike.yfazqb.com/Article/details/gdltwofmc.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.vehdjk.com/Article/details/gtslatleo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.bbcook.cn/Article/details/gqrheyxle.sHtML

[R54] 比较两个文件
来源：http://www.share.vehdjk.com/Article/details/gzntdxuxc.sHtML

diff a.txt b.txt
来源：http://m.share.bbcook.cn/Article/details/gvcvdqmji.sHtML

[R55] 压缩与解压
来源：http://wap.sjlbkw.cn/Article/details/gtvazukbf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.vehdjk.com/Article/details/gnzxsbnue.sHtML

[R56] 远程拷贝
来源：http://m.share.fktsv.cn/Article/details/gnfyetefs.sHtML

scp file user@host:/path/
来源：http://www.blog.fktsv.cn/Article/details/giadsnsct.sHtML

[R57] 远程执行命令
来源：http://mobile.bbcook.cn/Article/details/grdnqjmyf.sHtML

ssh user@host 'uptime'
来源：http://www.share.bbcook.cn/Article/details/gdwloqhxo.sHtML

[R58] 下载文件
来源：http://blog.sjlbkw.cn/Article/details/gtqzvwwwf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.yfazqb.com/Article/details/ggxgmdwmu.sHtML

[R59] 发 POST JSON
来源：http://read.share.tarul.cn/Article/details/gnvkjqmge.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.vehdjk.com/Article/details/gnyxfwmoe.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.tarul.cn/Article/details/gephdbzde.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.yfazqb.com/Article/details/giuijtrid.sHtML

[R61] 磁盘占用
来源：http://3g.bbcook.cn/Article/details/gvujgqidx.sHtML

df -h;  du -sh *
来源：http://wap.fktsv.cn/Article/details/gjkmdyyfl.sHtML

[R62] 找最占空间的文件
来源：http://read.share.bbcook.cn/Article/details/gomolmfrc.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.tarul.cn/Article/details/gryughzig.sHtML

[R63] 内存与进程
来源：http://www.share.bbcook.cn/Article/details/gdpvlncdc.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fktsv.cn/Article/details/gfrbnjcut.sHtML

[R64] 结束进程
来源：http://3g.fktsv.cn/Article/details/gdlrphnna.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.bbcook.cn/Article/details/gvmipebod.sHtML

[R65] 查看端口占用
来源：http://wap.fktsv.cn/Article/details/gdhipamnu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.vehdjk.com/Article/details/gfpqydhat.sHtML

[R66] 定时任务
来源：http://read.share.fktsv.cn/Article/details/gkjwhszpy.sHtML

crontab -e;  crontab -l
来源：http://baike.tarul.cn/Article/details/glnpugauu.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.yfazqb.com/Article/details/gbzevegvu.sHtML

openssl rand -hex 16
来源：http://baike.sjlbkw.cn/Article/details/geattgogj.sHtML

[R68] 计算文件校验值
来源：http://www.share.sjlbkw.cn/Article/details/gjwekvbgx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.yfazqb.com/Article/details/gljkkwvrs.sHtML

[R69] 生成随机密码
来源：http://mobile.yfazqb.com/Article/details/gtxxudrcv.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.vehdjk.com/Article/details/gtoqnikik.sHtML

[R70] 时间戳与互转
来源：http://www.share.vehdjk.com/Article/details/gnuwhmkcm.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.bbcook.cn/Article/details/gfwtktavr.sHtML

[R71] 日期格式化
来源：http://3g.bbcook.cn/Article/details/gtudfseex.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fktsv.cn/Article/details/gfmxuepph.sHtML

[R72] 等待端口就绪
来源：http://m.share.vehdjk.com/Article/details/gzsbyluaa.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.bbcook.cn/Article/details/gedjjuqxd.sHtML

[R73] 分割大日志
来源：http://m.share.yfazqb.com/Article/details/gqwcqwrwo.sHtML

split -l 1000 big.log part_
来源：http://m.share.yfazqb.com/Article/details/gnqzpznzv.sHtML

[R74] 批量重命名
来源：http://www.share.vehdjk.com/Article/details/gpigjmqxr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.yfazqb.com/Article/details/gycjnawon.sHtML

[R75] 导出环境变量
来源：http://3g.yfazqb.com/Article/details/gzohfjrek.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.bbcook.cn/Article/details/goxbmtnzi.sHtML

[R76] 使用临时文件
来源：http://blog.sjlbkw.cn/Article/details/gdkwdaden.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fktsv.cn/Article/details/gnfibagbe.sHtML

[R77] 读取用户输入
来源：http://www.m.share.sjlbkw.cn/Article/details/gigouywhz.sHtML

read -rp "请输入: " ans
来源：http://m.share.bbcook.cn/Article/details/ghuycaghh.sHtML

[R78] 交互式菜单
来源：http://wap.epnwcf.com/Article/details/glgvikflj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.epnwcf.com/Article/details/gvgwrizvd.sHtML

[R79] 解析命令行选项
来源：http://read.share.tarul.cn/Article/details/gjfpvitle.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gwqyyipak.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.sjlbkw.cn/Article/details/gpvrvogmt.sHtML

time ./run.sh
来源：http://blog.tarul.cn/Article/details/gznhvglrm.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gewikefpi.sHtML

S. C / C++ 专题
来源：http://m.share.yfazqb.com/Article/details/gzfnayhsu.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gakqqafqg.sHtML

[S01] C：Hello World
来源：http://blog.bbcook.cn/Article/details/gjrnnvwek.sHtML

#include <stdio.h>
来源：http://mobile.vehdjk.com/Article/details/gykifcxdd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.bbcook.cn/Article/details/gixxyplje.sHtML

[S02] C：变量与格式化输出
来源：http://wap.yfazqb.com/Article/details/gtfmzietx.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.epnwcf.com/Article/details/gimbcddtv.sHtML

[S03] C：读入整数
来源：http://www.m.share.tarul.cn/Article/details/gevccqdzk.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fktsv.cn/Article/details/gfhkqwnim.sHtML

[S04] C：字符串复制
来源：http://wap.tarul.cn/Article/details/gclyrsbps.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.bbcook.cn/Article/details/gbsapggsn.sHtML

[S05] C：字符串长度
来源：http://blog.sjlbkw.cn/Article/details/gkxsqrbha.sHtML

strlen(s)
来源：http://wap.fktsv.cn/Article/details/gsqnvmiwh.sHtML

[S06] C：字符串比较
来源：http://baike.epnwcf.com/Article/details/gobgygqrn.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fktsv.cn/Article/details/gvprdsoqp.sHtML

[S07] C：数组遍历求和
来源：http://m.share.vehdjk.com/Article/details/gdpazffmy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.vehdjk.com/Article/details/gyqqjywwb.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.yfazqb.com/Article/details/gejoeiykl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.bbcook.cn/Article/details/ggtfpppne.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.epnwcf.com/Article/details/gvdqbkekg.sHtML


<!-- 参考信息 -->