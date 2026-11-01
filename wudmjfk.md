代发 wailian999

[Q36] 左连接
来源：http://www.blog.tarul.cn/Article/details/gjhpbjrgo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.tarul.cn/Article/details/gdkogdcjr.sHtML

[Q37] 右连接
来源：http://m.share.yfazqb.com/Article/details/ghmujyryb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.tarul.cn/Article/details/gdixsyawh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fktsv.cn/Article/details/gwwzcuumh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fktsv.cn/Article/details/gnxbvanwf.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fktsv.cn/Article/details/glxsmeacu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fktsv.cn/Article/details/gembnylyv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.vehdjk.com/Article/details/gfpvyntau.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.vehdjk.com/Article/details/gzmbtcoug.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fktsv.cn/Article/details/gqemowmfh.sHtML

[Q41] 多表连接
来源：http://www.m.share.sjlbkw.cn/Article/details/gfltvxusf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.yfazqb.com/Article/details/gywizntau.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.bbcook.cn/Article/details/gzypshmso.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.sjlbkw.cn/Article/details/glpkgjsmk.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fktsv.cn/Article/details/gluaibvll.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.vehdjk.com/Article/details/gaeoeugvr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.tarul.cn/Article/details/ghlzsjjla.sHtML

[Q43] 标量子查询
来源：http://read.share.bbcook.cn/Article/details/gakoyyutn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fktsv.cn/Article/details/gqvznlunq.sHtML

[Q44] IN 子查询
来源：http://www.m.share.sjlbkw.cn/Article/details/ggspjxplg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fktsv.cn/Article/details/guetidsbf.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.epnwcf.com/Article/details/ggirdoffu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.bbcook.cn/Article/details/gmeenveyu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.bbcook.cn/Article/details/glrufyszy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.tarul.cn/Article/details/gfumdowla.sHtML

[Q47] 与平均值比较
来源：http://www.blog.bbcook.cn/Article/details/gryqiqtfk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.bbcook.cn/Article/details/gkwaybyua.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.yfazqb.com/Article/details/gpxpdbxrl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.vehdjk.com/Article/details/gbgxmnwao.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fktsv.cn/Article/details/gmqqvbpxf.sHtML

[Q49] 更新单行
来源：http://3g.bbcook.cn/Article/details/godhirbfa.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.yfazqb.com/Article/details/gnwdirtwc.sHtML

[Q50] 批量更新
来源：http://www.share.tarul.cn/Article/details/gvfahyrql.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.yfazqb.com/Article/details/gekwznzig.sHtML

[Q51] 用子查询更新
来源：http://blog.sjlbkw.cn/Article/details/ghkxxbjsv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.vehdjk.com/Article/details/gcerkjtgi.sHtML

[Q52] 删除指定行
来源：http://www.m.share.bbcook.cn/Article/details/gzdsxilqj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.bbcook.cn/Article/details/gqyzprtzv.sHtML

[Q53] 按条件删除
来源：http://www.blog.tarul.cn/Article/details/gvopxhsrt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.yfazqb.com/Article/details/gidnajfnc.sHtML

[Q54] 清空表
来源：http://read.share.yfazqb.com/Article/details/gcznvwqfw.sHtML

TRUNCATE TABLE logs;
来源：http://3g.vehdjk.com/Article/details/ghwiwbhcz.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fktsv.cn/Article/details/goammamxj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.sjlbkw.cn/Article/details/gmkbgttiu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.vehdjk.com/Article/details/gywclgtcy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.epnwcf.com/Article/details/gwefurrao.sHtML

[Q57] 行号
来源：http://www.share.epnwcf.com/Article/details/grtkzdgwz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gqjcmuvod.sHtML

[Q58] 累计求和
来源：http://www.share.epnwcf.com/Article/details/gfooaucwk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.vehdjk.com/Article/details/gjgoamulp.sHtML

[Q59] 分组内累计
来源：http://read.share.vehdjk.com/Article/details/giryrskvl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.vehdjk.com/Article/details/gfbbyvepl.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.vehdjk.com/Article/details/grcshtebf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.tarul.cn/Article/details/gczsfqdlc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.bbcook.cn/Article/details/gmkkexbaf.sHtML

[Q61] 移动平均
来源：http://baike.bbcook.cn/Article/details/gojczalmk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.tarul.cn/Article/details/ghkkvhvim.sHtML

[Q62] 分组占比
来源：http://wap.bbcook.cn/Article/details/gprdmeufu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.vehdjk.com/Article/details/gbyvzzlji.sHtML

[Q63] 开启事务
来源：http://wap.fktsv.cn/Article/details/gxbqowhjj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.bbcook.cn/Article/details/gnkhrnwlf.sHtML

[Q64] 提交事务
来源：http://read.share.vehdjk.com/Article/details/gdlhqwrha.sHtML

COMMIT;
来源：http://www.blog.vehdjk.com/Article/details/gxzhbsaqz.sHtML

[Q65] 回滚事务
来源：http://wap.tarul.cn/Article/details/gxxhxugnx.sHtML

ROLLBACK;
来源：http://www.blog.fktsv.cn/Article/details/gbwnofprr.sHtML

[Q66] 行锁查询
来源：http://m.share.epnwcf.com/Article/details/gslhgamrq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.tarul.cn/Article/details/gbqzoxwjj.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.epnwcf.com/Article/details/gtkwkeamn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.yfazqb.com/Article/details/grdkkyhqe.sHtML

[Q68] 保存点
来源：http://wap.tarul.cn/Article/details/gysvezpfa.sHtML

SAVEPOINT sp1;
来源：http://3g.epnwcf.com/Article/details/gqmlnvwbv.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.vehdjk.com/Article/details/gjjgvsfch.sHtML

[Q69] 查看执行计划
来源：http://3g.vehdjk.com/Article/details/geiohfpum.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.epnwcf.com/Article/details/gvjfokepv.sHtML

[Q70] 更新统计信息
来源：http://baike.sjlbkw.cn/Article/details/gigcvjzjo.sHtML

ANALYZE TABLE users;
来源：http://www.blog.tarul.cn/Article/details/giobhqrvy.sHtML

[Q71] 查看建表语句
来源：http://www.share.vehdjk.com/Article/details/gmiqhmihm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fktsv.cn/Article/details/guoxdazwz.sHtML

[Q72] 查看索引
来源：http://mobile.vehdjk.com/Article/details/gfdigxrvn.sHtML

SHOW INDEX FROM users;
来源：http://m.share.tarul.cn/Article/details/guyizaeuw.sHtML

[Q73] 查看表状态
来源：http://blog.epnwcf.com/Article/details/gafjoojcb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.tarul.cn/Article/details/grrvvdabm.sHtML

[Q74] 强制使用索引
来源：http://3g.vehdjk.com/Article/details/glheraeuv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.yfazqb.com/Article/details/gekadzuox.sHtML

[Q75] 日期格式化
来源：http://www.m.share.sjlbkw.cn/Article/details/gptqvoifh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.bbcook.cn/Article/details/gdtkgvdsn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.vehdjk.com/Article/details/gcvjwyuqr.sHtML

[Q76] 按天统计
来源：http://www.share.fktsv.cn/Article/details/gnrgtkqrh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.tarul.cn/Article/details/gbehaxvxc.sHtML

[Q77] 时间加减
来源：http://blog.epnwcf.com/Article/details/gcmbsjhgt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.sjlbkw.cn/Article/details/gzffrvqpg.sHtML

[Q78] 当前时间
来源：http://m.share.fktsv.cn/Article/details/gbmvcaruy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fktsv.cn/Article/details/gdizxbets.sHtML

[Q79] 字符串拼接
来源：http://www.share.tarul.cn/Article/details/gfbnwernh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.sjlbkw.cn/Article/details/guxnkhztq.sHtML

[Q80] 字符串截取
来源：http://blog.tarul.cn/Article/details/ggnathjrt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.vehdjk.com/Article/details/ghwpmzsuc.sHtML

[Q81] 字符串替换
来源：http://www.blog.tarul.cn/Article/details/gdvanqoxy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.epnwcf.com/Article/details/gzxqkcsor.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.sjlbkw.cn/Article/details/gakgyaryp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.vehdjk.com/Article/details/gebaqxcas.sHtML

[Q83] 大小写转换
来源：http://www.share.fktsv.cn/Article/details/ghetjrppp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gytkmshre.sHtML

[Q84] 去除首尾空格
来源：http://mobile.epnwcf.com/Article/details/gbbbklibp.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gvquhhzle.sHtML

[Q85] 数值取整
来源：http://3g.fktsv.cn/Article/details/gfyoamdzk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.yfazqb.com/Article/details/gfwcogjmm.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.tarul.cn/Article/details/grahbkrgl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.bbcook.cn/Article/details/gtudsupqc.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.bbcook.cn/Article/details/gdclmkfza.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.bbcook.cn/Article/details/gplggguuw.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fktsv.cn/Article/details/ggqvfrzji.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fktsv.cn/Article/details/grppxrkji.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gaiaziklo.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.sjlbkw.cn/Article/details/gyqtnarkz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.tarul.cn/Article/details/gvylngmkz.sHtML

[Q90] 生成序号列
来源：http://www.share.epnwcf.com/Article/details/gfpiwxwkl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.yfazqb.com/Article/details/gkwshwzag.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gawvlnnsl.sHtML

R. Bash 专题
来源：http://3g.bbcook.cn/Article/details/gfwygqgqg.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/glzwelhhc.sHtML

[R01] shebang 与严格模式
来源：http://m.share.epnwcf.com/Article/details/gyczbkjix.sHtML

#!/usr/bin/env bash
来源：http://wap.yfazqb.com/Article/details/gpnjxfsxl.sHtML

set -euo pipefail
来源：http://wap.fktsv.cn/Article/details/gvhtzkhbx.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fktsv.cn/Article/details/ghgcmgzzu.sHtML

name="Tom"; echo "$name"
来源：http://www.share.sjlbkw.cn/Article/details/gjysujywx.sHtML

[R03] 只读变量
来源：http://www.share.vehdjk.com/Article/details/gfxrnnomt.sHtML

readonly PI=3.14
来源：http://wap.vehdjk.com/Article/details/gkfdcjgko.sHtML

[R04] 位置参数
来源：http://baike.sjlbkw.cn/Article/details/glwnwngqf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.sjlbkw.cn/Article/details/gpiuxmhlk.sHtML

[R05] 参数默认值
来源：http://www.share.yfazqb.com/Article/details/gjxwklkkq.sHtML

name="${1:-default}"
来源：http://3g.tarul.cn/Article/details/gayhegfri.sHtML

[R06] 判断命令是否存在
来源：http://mobile.bbcook.cn/Article/details/gfoeanyfr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.tarul.cn/Article/details/gjmjdizfs.sHtML

[R07] if 判断文件
来源：http://wap.sjlbkw.cn/Article/details/gteccpbek.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.sjlbkw.cn/Article/details/gjzmxzndk.sHtML

[R08] 数值比较
来源：http://www.share.vehdjk.com/Article/details/ghweohqhx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.bbcook.cn/Article/details/gebiblaij.sHtML

[R09] 字符串比较
来源：http://www.share.bbcook.cn/Article/details/gdjkpnxcf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.sjlbkw.cn/Article/details/gzgdyuczd.sHtML

[R10] 正则匹配
来源：http://wap.bbcook.cn/Article/details/gwactbtbr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.vehdjk.com/Article/details/gfichzwxj.sHtML

[R11] case 多分支
来源：http://3g.tarul.cn/Article/details/grjuxlmkw.sHtML

case "$1" in
来源：http://m.share.sjlbkw.cn/Article/details/gztttkogw.sHtML

start) echo "启动" ;;
来源：http://www.share.epnwcf.com/Article/details/gnsbpcaui.sHtML

stop)  echo "停止" ;;
来源：http://wap.sjlbkw.cn/Article/details/ginizdqtn.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.sjlbkw.cn/Article/details/ggvggtdrj.sHtML

esac
来源：http://www.m.share.yfazqb.com/Article/details/gofittzna.sHtML

[R12] for 遍历文件
来源：http://www.share.epnwcf.com/Article/details/gehdmrhin.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.bbcook.cn/Article/details/gwbxqecwf.sHtML

[R13] for 计数循环
来源：http://read.share.epnwcf.com/Article/details/ghxxjxset.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.bbcook.cn/Article/details/gnsoyfewv.sHtML

[R14] C 风格 for
来源：http://read.share.fktsv.cn/Article/details/gkfqkkmml.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.epnwcf.com/Article/details/gljvuzlfh.sHtML

[R15] while 逐行读文件
来源：http://blog.yfazqb.com/Article/details/gvawptlri.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.bbcook.cn/Article/details/gljrzhmio.sHtML

[R16] until 等待条件
来源：http://www.m.share.bbcook.cn/Article/details/gjeaycffm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.bbcook.cn/Article/details/gdivipxtl.sHtML

[R17] 数组定义与取值
来源：http://baike.vehdjk.com/Article/details/glfdwpcjh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.tarul.cn/Article/details/gdnqzaepu.sHtML

[R18] 遍历数组
来源：http://www.share.epnwcf.com/Article/details/gqdaeajsz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.bbcook.cn/Article/details/gctenzdyu.sHtML

[R19] 数组长度
来源：http://www.share.yfazqb.com/Article/details/gijyfmbrn.sHtML

echo "${#arr[@]}"
来源：http://www.blog.tarul.cn/Article/details/glebvrmgb.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.tarul.cn/Article/details/guikvxrxg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.tarul.cn/Article/details/gdpydczhe.sHtML

[R21] 字符串长度
来源：http://read.share.bbcook.cn/Article/details/gvpzkhrpn.sHtML

echo "${#s}"
来源：http://wap.bbcook.cn/Article/details/gknxisppn.sHtML

[R22] 截取子串
来源：http://blog.vehdjk.com/Article/details/gjyvrkhzw.sHtML

echo "${s:0:5}"
来源：http://3g.fktsv.cn/Article/details/glwfaijbb.sHtML

[R23] 字符串替换
来源：http://read.share.epnwcf.com/Article/details/glyfmvjkt.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.bbcook.cn/Article/details/gltaffnur.sHtML

[R24] 大小写转换
来源：http://3g.yfazqb.com/Article/details/gqhemblih.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.epnwcf.com/Article/details/gzdfhddfs.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fktsv.cn/Article/details/gxsdqtgxr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.sjlbkw.cn/Article/details/gaauuwfyz.sHtML

[R26] 命令替换
来源：http://www.m.share.tarul.cn/Article/details/gxmlqxbar.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.tarul.cn/Article/details/gdcgfitiy.sHtML

[R27] 算术展开
来源：http://www.m.share.sjlbkw.cn/Article/details/gchazrbdw.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.tarul.cn/Article/details/gryhxejaq.sHtML

[R28] 浮点运算
来源：http://wap.epnwcf.com/Article/details/guxrldxhr.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.epnwcf.com/Article/details/gflylnhkg.sHtML

[R29] 定义函数
来源：http://www.share.fktsv.cn/Article/details/gfosathfy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.epnwcf.com/Article/details/gpciplldo.sHtML

[R30] 函数返回状态码
来源：http://read.share.yfazqb.com/Article/details/gzgiafnem.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.sjlbkw.cn/Article/details/gffgufrna.sHtML

[R31] 局部变量
来源：http://www.m.share.tarul.cn/Article/details/gverbfega.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.epnwcf.com/Article/details/gyuqthxqq.sHtML

[R32] 参数个数校验
来源：http://www.blog.fktsv.cn/Article/details/gbprhyoqi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.tarul.cn/Article/details/gvbiyfzhp.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.vehdjk.com/Article/details/gmvdeqnat.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.yfazqb.com/Article/details/gvjtseffv.sHtML

[R34] 退出时清理
来源：http://mobile.vehdjk.com/Article/details/gxdzvfktg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fktsv.cn/Article/details/gvtlmtpoo.sHtML

[R35] 后台执行并等待
来源：http://www.blog.bbcook.cn/Article/details/guyyagvpv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.yfazqb.com/Article/details/gwbrprayx.sHtML

[R36] 并发执行多个任务
来源：http://www.share.epnwcf.com/Article/details/gpbenqoxd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.sjlbkw.cn/Article/details/gqwamfula.sHtML

[R37] 把输出赋给变量
来源：http://wap.vehdjk.com/Article/details/gzeqcshsm.sHtML

files=$(ls -1)
来源：http://read.share.vehdjk.com/Article/details/goaugipzt.sHtML

[R38] 管道串联
来源：http://baike.epnwcf.com/Article/details/gyjyesgqm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.yfazqb.com/Article/details/gveghkqsy.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.epnwcf.com/Article/details/gyzgobseo.sHtML

cmd > out.log 2>&1
来源：http://www.blog.yfazqb.com/Article/details/gvzwndxcz.sHtML

[R40] 追加写日志
来源：http://mobile.sjlbkw.cn/Article/details/gpdctfodf.sHtML

echo "log" >> out.log
来源：http://blog.vehdjk.com/Article/details/gnabzbrmg.sHtML

[R41] 丢弃输出
来源：http://www.share.bbcook.cn/Article/details/gyqqqpjsp.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fktsv.cn/Article/details/gzxdhymti.sHtML

[R42] 输入重定向
来源：http://blog.epnwcf.com/Article/details/gworssrcg.sHtML

wc -l < a.txt
来源：http://read.share.vehdjk.com/Article/details/gklftccyh.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fktsv.cn/Article/details/grkwuhuyf.sHtML

find . -name "*.log" -type f
来源：http://www.share.fktsv.cn/Article/details/gcnvnaquw.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fktsv.cn/Article/details/gerrtscwi.sHtML

find . -mtime -7 -type f
来源：http://3g.bbcook.cn/Article/details/gihgxfnhi.sHtML

[R45] 批量删除
来源：http://blog.vehdjk.com/Article/details/geinezget.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.vehdjk.com/Article/details/gyccfsoam.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fktsv.cn/Article/details/gwbkmzmmo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fktsv.cn/Article/details/gtoqijywm.sHtML

[R47] sed 单行替换
来源：http://www.m.share.bbcook.cn/Article/details/glugxxwju.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.bbcook.cn/Article/details/gacbrbhcp.sHtML

[R48] awk 取指定列
来源：http://mobile.sjlbkw.cn/Article/details/gxtsepecu.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.bbcook.cn/Article/details/gzezqmlum.sHtML

[R49] awk 带条件
来源：http://3g.tarul.cn/Article/details/gzxtpwtge.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.vehdjk.com/Article/details/gzqlhaofl.sHtML

[R50] awk 求和
来源：http://read.share.vehdjk.com/Article/details/gjxlskoul.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fktsv.cn/Article/details/gqlakivvl.sHtML

[R51] 排序去重取前几
来源：http://www.blog.vehdjk.com/Article/details/gwbxayxcr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fktsv.cn/Article/details/gezrkxvbc.sHtML

[R52] 统计行数
来源：http://blog.vehdjk.com/Article/details/gizgnhsde.sHtML

wc -l a.txt
来源：http://www.share.epnwcf.com/Article/details/guidbcejf.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.yfazqb.com/Article/details/gkgeiqtxf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.yfazqb.com/Article/details/gkoqsauih.sHtML

[R54] 比较两个文件
来源：http://www.share.tarul.cn/Article/details/gzavbpurh.sHtML

diff a.txt b.txt
来源：http://baike.epnwcf.com/Article/details/gjucpdawh.sHtML

[R55] 压缩与解压
来源：http://mobile.vehdjk.com/Article/details/gevhgnlsx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.yfazqb.com/Article/details/gfbsxxuch.sHtML

[R56] 远程拷贝
来源：http://m.share.vehdjk.com/Article/details/gpqojssbs.sHtML

scp file user@host:/path/
来源：http://baike.bbcook.cn/Article/details/gisibkkpd.sHtML

[R57] 远程执行命令
来源：http://read.share.tarul.cn/Article/details/gwycmqpkh.sHtML

ssh user@host 'uptime'
来源：http://blog.fktsv.cn/Article/details/godqigjgf.sHtML

[R58] 下载文件
来源：http://m.share.bbcook.cn/Article/details/gcllcmqvk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.yfazqb.com/Article/details/ghfjvydey.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.epnwcf.com/Article/details/gejnrwdio.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.epnwcf.com/Article/details/gmpltqdoc.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.sjlbkw.cn/Article/details/gfhwjbckl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.yfazqb.com/Article/details/gcxcinukj.sHtML

[R61] 磁盘占用
来源：http://www.share.tarul.cn/Article/details/glqtbgnqn.sHtML

df -h;  du -sh *
来源：http://read.share.epnwcf.com/Article/details/gkyazvnon.sHtML

[R62] 找最占空间的文件
来源：http://read.share.tarul.cn/Article/details/gmuwkzhlk.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.tarul.cn/Article/details/graznmxua.sHtML

[R63] 内存与进程
来源：http://mobile.bbcook.cn/Article/details/gjmmwjhnv.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.sjlbkw.cn/Article/details/gqegfdxxc.sHtML

[R64] 结束进程
来源：http://3g.vehdjk.com/Article/details/gqqssfqer.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.tarul.cn/Article/details/gbppfzuxg.sHtML

[R65] 查看端口占用
来源：http://baike.bbcook.cn/Article/details/gofzmqvya.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.tarul.cn/Article/details/gwlnymief.sHtML

[R66] 定时任务
来源：http://blog.yfazqb.com/Article/details/giqnqscyl.sHtML

crontab -e;  crontab -l
来源：http://wap.fktsv.cn/Article/details/gzcqdxgom.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.tarul.cn/Article/details/gdskfcbuj.sHtML

openssl rand -hex 16
来源：http://blog.tarul.cn/Article/details/gupulsjyn.sHtML

[R68] 计算文件校验值
来源：http://wap.fktsv.cn/Article/details/grmgzmcdu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fktsv.cn/Article/details/gyghwieby.sHtML

[R69] 生成随机密码
来源：http://www.m.share.epnwcf.com/Article/details/givzappbq.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.epnwcf.com/Article/details/ghdfawjcy.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.vehdjk.com/Article/details/gokkzzysz.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fktsv.cn/Article/details/gstkkpven.sHtML

[R71] 日期格式化
来源：http://www.blog.vehdjk.com/Article/details/gojpwmnmn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.yfazqb.com/Article/details/geruoqoka.sHtML

[R72] 等待端口就绪
来源：http://wap.vehdjk.com/Article/details/gdrnyzmjr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.bbcook.cn/Article/details/gfhcncgvk.sHtML

[R73] 分割大日志
来源：http://blog.yfazqb.com/Article/details/gsacmmumh.sHtML

split -l 1000 big.log part_
来源：http://m.share.bbcook.cn/Article/details/gstgpairk.sHtML

[R74] 批量重命名
来源：http://www.share.epnwcf.com/Article/details/gathrbsxm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.sjlbkw.cn/Article/details/gygxzfqwc.sHtML

[R75] 导出环境变量
来源：http://mobile.fktsv.cn/Article/details/gkbkudnzi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.bbcook.cn/Article/details/geoontcgq.sHtML

[R76] 使用临时文件
来源：http://www.share.fktsv.cn/Article/details/gmwgjnrdf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.yfazqb.com/Article/details/gmtqzwsno.sHtML

[R77] 读取用户输入
来源：http://www.m.share.epnwcf.com/Article/details/groebgcrm.sHtML

read -rp "请输入: " ans
来源：http://www.blog.tarul.cn/Article/details/gdmsvzfgf.sHtML

[R78] 交互式菜单
来源：http://wap.epnwcf.com/Article/details/gggmeysrn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fktsv.cn/Article/details/gujlhsklu.sHtML

[R79] 解析命令行选项
来源：http://3g.fktsv.cn/Article/details/gumrtfvrs.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.sjlbkw.cn/Article/details/goeaucsnv.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.yfazqb.com/Article/details/ggfnrdwlv.sHtML

time ./run.sh
来源：http://wap.tarul.cn/Article/details/gerzifhon.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gmouwlqyz.sHtML

S. C / C++ 专题
来源：http://m.share.fktsv.cn/Article/details/gkmzznpnq.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gbollkmen.sHtML

[S01] C：Hello World
来源：http://blog.epnwcf.com/Article/details/gxoubdvbz.sHtML

#include <stdio.h>
来源：http://www.m.share.fktsv.cn/Article/details/grkcvqjdk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.yfazqb.com/Article/details/gubjsytoi.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fktsv.cn/Article/details/gaiebopmp.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.epnwcf.com/Article/details/gikndduzp.sHtML

[S03] C：读入整数
来源：http://baike.fktsv.cn/Article/details/gxcmakzxq.sHtML

int x; scanf("%d", &x);
来源：http://read.share.yfazqb.com/Article/details/gwtanlpwg.sHtML

[S04] C：字符串复制
来源：http://3g.sjlbkw.cn/Article/details/gtwmxrdne.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fktsv.cn/Article/details/gtlrlelai.sHtML

[S05] C：字符串长度
来源：http://mobile.sjlbkw.cn/Article/details/gtmnzxile.sHtML


<!-- 参考信息 -->