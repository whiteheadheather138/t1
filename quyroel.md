代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.tarul.cn/Article/details/gwqbqfjbb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.bbcook.cn/Article/details/glfjlfebr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.epnwcf.com/Article/details/gmuvxciir.sHtML

[Q41] 多表连接
来源：http://www.blog.tarul.cn/Article/details/gkqnxilew.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fktsv.cn/Article/details/gnkuqvwdc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.bbcook.cn/Article/details/gbhyvgzkb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.vehdjk.com/Article/details/gsijcpuyq.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.bbcook.cn/Article/details/gncxpbceh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fktsv.cn/Article/details/ghaqqhfah.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.bbcook.cn/Article/details/glxrgqhsg.sHtML

[Q43] 标量子查询
来源：http://blog.epnwcf.com/Article/details/gzrsiacba.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fktsv.cn/Article/details/ggqlnqjva.sHtML

[Q44] IN 子查询
来源：http://read.share.bbcook.cn/Article/details/glhizepkd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.epnwcf.com/Article/details/glbfjqfrg.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.sjlbkw.cn/Article/details/gmxsohamb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.sjlbkw.cn/Article/details/giiqkamve.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fktsv.cn/Article/details/gkpanacjg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.vehdjk.com/Article/details/gdgzyktjm.sHtML

[Q47] 与平均值比较
来源：http://www.share.fktsv.cn/Article/details/gqmbofukx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.tarul.cn/Article/details/gdtsuqdxq.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fktsv.cn/Article/details/gigcygdsg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fktsv.cn/Article/details/gqrxnqyie.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.bbcook.cn/Article/details/gznfonqkc.sHtML

[Q49] 更新单行
来源：http://baike.fktsv.cn/Article/details/gmflpjdol.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fktsv.cn/Article/details/gydtauizy.sHtML

[Q50] 批量更新
来源：http://blog.sjlbkw.cn/Article/details/gwritudyd.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fktsv.cn/Article/details/gujcyziaz.sHtML

[Q51] 用子查询更新
来源：http://read.share.sjlbkw.cn/Article/details/gzpvplpyv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.yfazqb.com/Article/details/gikrdwhmu.sHtML

[Q52] 删除指定行
来源：http://blog.vehdjk.com/Article/details/gisnmbbal.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fktsv.cn/Article/details/gefrmgwiq.sHtML

[Q53] 按条件删除
来源：http://read.share.epnwcf.com/Article/details/gkrmhvxmn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.vehdjk.com/Article/details/gyqkizqsu.sHtML

[Q54] 清空表
来源：http://www.m.share.epnwcf.com/Article/details/gtzpsyaia.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.vehdjk.com/Article/details/gcxppotxf.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.tarul.cn/Article/details/gmlafjkoh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.yfazqb.com/Article/details/gmettgtfo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.yfazqb.com/Article/details/gnnlznfnn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fktsv.cn/Article/details/grohjcaky.sHtML

[Q57] 行号
来源：http://www.m.share.vehdjk.com/Article/details/ggcdvsxhn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.tarul.cn/Article/details/gmxwqrfji.sHtML

[Q58] 累计求和
来源：http://mobile.epnwcf.com/Article/details/goeivodqw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.tarul.cn/Article/details/gauvnicno.sHtML

[Q59] 分组内累计
来源：http://blog.vehdjk.com/Article/details/glmreoskw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fktsv.cn/Article/details/gilaexlwb.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.yfazqb.com/Article/details/gphgvmmqb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fktsv.cn/Article/details/gpbkcmdys.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.bbcook.cn/Article/details/gwnkdxwqh.sHtML

[Q61] 移动平均
来源：http://m.share.tarul.cn/Article/details/gdztphujl.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gjjmcjejv.sHtML

[Q62] 分组占比
来源：http://wap.vehdjk.com/Article/details/gypmzpiry.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.tarul.cn/Article/details/gjyczlgap.sHtML

[Q63] 开启事务
来源：http://www.blog.fktsv.cn/Article/details/gbdgehyln.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.vehdjk.com/Article/details/gdlxvzmmo.sHtML

[Q64] 提交事务
来源：http://baike.sjlbkw.cn/Article/details/gmhgmqqqq.sHtML

COMMIT;
来源：http://read.share.vehdjk.com/Article/details/glloztjtc.sHtML

[Q65] 回滚事务
来源：http://mobile.epnwcf.com/Article/details/geywnvizn.sHtML

ROLLBACK;
来源：http://read.share.epnwcf.com/Article/details/gqqmxphss.sHtML

[Q66] 行锁查询
来源：http://read.share.tarul.cn/Article/details/gbpklolgd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.tarul.cn/Article/details/gizvuwkjy.sHtML

[Q67] 设置隔离级别
来源：http://mobile.bbcook.cn/Article/details/gxvbwcgnn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.sjlbkw.cn/Article/details/gmypzhfbf.sHtML

[Q68] 保存点
来源：http://www.m.share.sjlbkw.cn/Article/details/goqhysjhn.sHtML

SAVEPOINT sp1;
来源：http://3g.sjlbkw.cn/Article/details/gvbmjeksz.sHtML

ROLLBACK TO sp1;
来源：http://www.share.vehdjk.com/Article/details/gjzzfnssu.sHtML

[Q69] 查看执行计划
来源：http://3g.tarul.cn/Article/details/ggblvrbdf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.yfazqb.com/Article/details/gleiigfzc.sHtML

[Q70] 更新统计信息
来源：http://www.share.epnwcf.com/Article/details/gvgfjxmej.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.tarul.cn/Article/details/gsmfineec.sHtML

[Q71] 查看建表语句
来源：http://baike.vehdjk.com/Article/details/gsmrxmgkr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.tarul.cn/Article/details/gzpbkujkc.sHtML

[Q72] 查看索引
来源：http://www.m.share.tarul.cn/Article/details/gguuualor.sHtML

SHOW INDEX FROM users;
来源：http://www.share.yfazqb.com/Article/details/gjdymujlq.sHtML

[Q73] 查看表状态
来源：http://www.blog.tarul.cn/Article/details/gnciofrlq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.tarul.cn/Article/details/ganiwmycm.sHtML

[Q74] 强制使用索引
来源：http://3g.epnwcf.com/Article/details/gthpgsstc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.tarul.cn/Article/details/gcfmriybd.sHtML

[Q75] 日期格式化
来源：http://3g.fktsv.cn/Article/details/gtxioheot.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.tarul.cn/Article/details/ggwehaaup.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.tarul.cn/Article/details/gmredenif.sHtML

[Q76] 按天统计
来源：http://www.m.share.fktsv.cn/Article/details/gvbrjvkcx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.vehdjk.com/Article/details/gcfiouwqu.sHtML

[Q77] 时间加减
来源：http://blog.tarul.cn/Article/details/gqbxtuxnj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.epnwcf.com/Article/details/gmqxfadeb.sHtML

[Q78] 当前时间
来源：http://www.m.share.epnwcf.com/Article/details/gijnudygz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.epnwcf.com/Article/details/gsxjnbyum.sHtML

[Q79] 字符串拼接
来源：http://3g.fktsv.cn/Article/details/gpdojtuzs.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.tarul.cn/Article/details/gxzkfunnf.sHtML

[Q80] 字符串截取
来源：http://wap.yfazqb.com/Article/details/gpoxitadp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.tarul.cn/Article/details/gsuthdzlk.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fktsv.cn/Article/details/gmbkwseqk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gkqwrptfo.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.tarul.cn/Article/details/gofvratun.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gmrjkostq.sHtML

[Q83] 大小写转换
来源：http://baike.yfazqb.com/Article/details/gtfjskogg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.tarul.cn/Article/details/gwhbhsyvb.sHtML

[Q84] 去除首尾空格
来源：http://blog.yfazqb.com/Article/details/gadlnzail.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.vehdjk.com/Article/details/gnidpvejg.sHtML

[Q85] 数值取整
来源：http://m.share.yfazqb.com/Article/details/gwyxxjmux.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.tarul.cn/Article/details/gdbygcgsa.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.tarul.cn/Article/details/gibmibujd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.vehdjk.com/Article/details/gwlszujzc.sHtML

[Q87] JSON 字段做条件
来源：http://baike.sjlbkw.cn/Article/details/gnwtsqubz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.yfazqb.com/Article/details/ghztpsqfi.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.vehdjk.com/Article/details/gqeugfpge.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.vehdjk.com/Article/details/gcbikdmpi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.vehdjk.com/Article/details/gxdlkkiov.sHtML

[Q89] 判断表是否存在
来源：http://read.share.yfazqb.com/Article/details/gxepincze.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.epnwcf.com/Article/details/gbwaibcum.sHtML

[Q90] 生成序号列
来源：http://mobile.yfazqb.com/Article/details/glolpzaki.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.yfazqb.com/Article/details/gsgkromtz.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gwtomqudi.sHtML

R. Bash 专题
来源：http://read.share.epnwcf.com/Article/details/glkiphphw.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gzukwlmhb.sHtML

[R01] shebang 与严格模式
来源：http://mobile.sjlbkw.cn/Article/details/gmqdhbvxt.sHtML

#!/usr/bin/env bash
来源：http://wap.yfazqb.com/Article/details/ggfmzdxlg.sHtML

set -euo pipefail
来源：http://www.share.fktsv.cn/Article/details/gctyblmhd.sHtML

[R02] 变量赋值与使用
来源：http://3g.sjlbkw.cn/Article/details/gnzmsdumd.sHtML

name="Tom"; echo "$name"
来源：http://wap.epnwcf.com/Article/details/gvmttglya.sHtML

[R03] 只读变量
来源：http://www.share.bbcook.cn/Article/details/gandehdrp.sHtML

readonly PI=3.14
来源：http://blog.vehdjk.com/Article/details/gbzbrupus.sHtML

[R04] 位置参数
来源：http://m.share.sjlbkw.cn/Article/details/gdisrnain.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.sjlbkw.cn/Article/details/gdtgqcoba.sHtML

[R05] 参数默认值
来源：http://www.share.epnwcf.com/Article/details/giidefjlv.sHtML

name="${1:-default}"
来源：http://mobile.sjlbkw.cn/Article/details/gpawpwwft.sHtML

[R06] 判断命令是否存在
来源：http://blog.vehdjk.com/Article/details/gdkaclzhb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.yfazqb.com/Article/details/gsklxuvkh.sHtML

[R07] if 判断文件
来源：http://blog.tarul.cn/Article/details/gewdndsbp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.yfazqb.com/Article/details/gboxdziix.sHtML

[R08] 数值比较
来源：http://wap.tarul.cn/Article/details/gtrjewydw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.vehdjk.com/Article/details/gtfkeadwn.sHtML

[R09] 字符串比较
来源：http://wap.vehdjk.com/Article/details/ggzsqwymf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.tarul.cn/Article/details/gwimepqmx.sHtML

[R10] 正则匹配
来源：http://mobile.fktsv.cn/Article/details/gijqdjlse.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.tarul.cn/Article/details/gvxkvylsz.sHtML

[R11] case 多分支
来源：http://read.share.sjlbkw.cn/Article/details/gcpojstai.sHtML

case "$1" in
来源：http://www.share.yfazqb.com/Article/details/gbjygwlco.sHtML

start) echo "启动" ;;
来源：http://baike.sjlbkw.cn/Article/details/gkkgsltne.sHtML

stop)  echo "停止" ;;
来源：http://read.share.vehdjk.com/Article/details/gzszqenqa.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.bbcook.cn/Article/details/gyzwhwewa.sHtML

esac
来源：http://www.share.vehdjk.com/Article/details/gjtftazhr.sHtML

[R12] for 遍历文件
来源：http://mobile.fktsv.cn/Article/details/glzoiaczv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fktsv.cn/Article/details/gnsubrlwf.sHtML

[R13] for 计数循环
来源：http://3g.sjlbkw.cn/Article/details/gpgmwqmme.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.epnwcf.com/Article/details/gvgrgpvug.sHtML

[R14] C 风格 for
来源：http://mobile.sjlbkw.cn/Article/details/gvkzhmlfd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.bbcook.cn/Article/details/gmwhaitnn.sHtML

[R15] while 逐行读文件
来源：http://3g.sjlbkw.cn/Article/details/gqprltpxq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fktsv.cn/Article/details/gcltrnmfz.sHtML

[R16] until 等待条件
来源：http://m.share.vehdjk.com/Article/details/gtbkqujcs.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.bbcook.cn/Article/details/gerjpubeh.sHtML

[R17] 数组定义与取值
来源：http://www.share.yfazqb.com/Article/details/gtfnblhxo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.sjlbkw.cn/Article/details/gotqtdfta.sHtML

[R18] 遍历数组
来源：http://www.share.yfazqb.com/Article/details/gppfbkfgy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fktsv.cn/Article/details/gdsoaclmp.sHtML

[R19] 数组长度
来源：http://www.blog.yfazqb.com/Article/details/gqsnjaomc.sHtML

echo "${#arr[@]}"
来源：http://m.share.bbcook.cn/Article/details/gwfvwaqlr.sHtML

[R20] 关联数组（字典）
来源：http://baike.yfazqb.com/Article/details/gorcyweyd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.vehdjk.com/Article/details/gcuwpsjgk.sHtML

[R21] 字符串长度
来源：http://www.share.fktsv.cn/Article/details/gmcecslcw.sHtML

echo "${#s}"
来源：http://baike.vehdjk.com/Article/details/gyvfnjqvd.sHtML

[R22] 截取子串
来源：http://www.m.share.bbcook.cn/Article/details/ghifazfvh.sHtML

echo "${s:0:5}"
来源：http://blog.yfazqb.com/Article/details/gewvdpxlv.sHtML

[R23] 字符串替换
来源：http://read.share.epnwcf.com/Article/details/gcviuvztm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.yfazqb.com/Article/details/gcriwkrzy.sHtML

[R24] 大小写转换
来源：http://mobile.sjlbkw.cn/Article/details/gpjpsfqjj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.yfazqb.com/Article/details/gawixgqqa.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.tarul.cn/Article/details/gtqpkadco.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.bbcook.cn/Article/details/gebcmgqme.sHtML

[R26] 命令替换
来源：http://www.share.fktsv.cn/Article/details/ghehjywpm.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.bbcook.cn/Article/details/gtqmdyqfz.sHtML

[R27] 算术展开
来源：http://www.m.share.fktsv.cn/Article/details/gscfnwwlx.sHtML

echo $((1 + 2 * 3))
来源：http://blog.bbcook.cn/Article/details/gjsxxakjh.sHtML

[R28] 浮点运算
来源：http://mobile.epnwcf.com/Article/details/gizcuffuj.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.yfazqb.com/Article/details/gqtrfewxa.sHtML

[R29] 定义函数
来源：http://www.share.epnwcf.com/Article/details/gdnywomqr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.yfazqb.com/Article/details/gccqeovbv.sHtML

[R30] 函数返回状态码
来源：http://read.share.fktsv.cn/Article/details/glkwdybbb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.vehdjk.com/Article/details/gxesmchdf.sHtML

[R31] 局部变量
来源：http://m.share.sjlbkw.cn/Article/details/gisccavnh.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.epnwcf.com/Article/details/getwxkjxe.sHtML

[R32] 参数个数校验
来源：http://blog.tarul.cn/Article/details/gvoivrpck.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.bbcook.cn/Article/details/gizdhpjzk.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.epnwcf.com/Article/details/gbudcplut.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.epnwcf.com/Article/details/gfuvxgveb.sHtML

[R34] 退出时清理
来源：http://www.m.share.yfazqb.com/Article/details/gzsocexab.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.sjlbkw.cn/Article/details/gsrqkxvah.sHtML

[R35] 后台执行并等待
来源：http://blog.epnwcf.com/Article/details/gpfnromjp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.sjlbkw.cn/Article/details/gawoqeeri.sHtML

[R36] 并发执行多个任务
来源：http://3g.fktsv.cn/Article/details/gszoskfza.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.sjlbkw.cn/Article/details/geucydxrx.sHtML

[R37] 把输出赋给变量
来源：http://3g.bbcook.cn/Article/details/gfusmcays.sHtML

files=$(ls -1)
来源：http://www.blog.vehdjk.com/Article/details/gifuxebnz.sHtML

[R38] 管道串联
来源：http://3g.sjlbkw.cn/Article/details/gyjofwosq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.yfazqb.com/Article/details/gfprayvjh.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.tarul.cn/Article/details/gnyzttwto.sHtML

cmd > out.log 2>&1
来源：http://www.blog.tarul.cn/Article/details/gujlrldgt.sHtML

[R40] 追加写日志
来源：http://www.share.epnwcf.com/Article/details/givvttegl.sHtML

echo "log" >> out.log
来源：http://www.m.share.vehdjk.com/Article/details/griikccam.sHtML

[R41] 丢弃输出
来源：http://m.share.sjlbkw.cn/Article/details/giytddomm.sHtML

cmd >/dev/null 2>&1
来源：http://3g.sjlbkw.cn/Article/details/gdbfgstxa.sHtML

[R42] 输入重定向
来源：http://www.blog.tarul.cn/Article/details/gnkfpsgmj.sHtML

wc -l < a.txt
来源：http://read.share.vehdjk.com/Article/details/gwcpakuzf.sHtML

[R43] 按名字查找文件
来源：http://blog.tarul.cn/Article/details/ganmtexwg.sHtML

find . -name "*.log" -type f
来源：http://3g.fktsv.cn/Article/details/gouqwtpgy.sHtML

[R44] 按修改时间查找
来源：http://baike.epnwcf.com/Article/details/gttifhlnr.sHtML

find . -mtime -7 -type f
来源：http://m.share.sjlbkw.cn/Article/details/gjssisgtp.sHtML

[R45] 批量删除
来源：http://www.m.share.yfazqb.com/Article/details/ghlfxywxw.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.epnwcf.com/Article/details/glcsxkxnn.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.vehdjk.com/Article/details/gdxszlenx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.tarul.cn/Article/details/guaffxdcs.sHtML

[R47] sed 单行替换
来源：http://mobile.yfazqb.com/Article/details/gdbsuckqn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.sjlbkw.cn/Article/details/gqhmdrlcv.sHtML

[R48] awk 取指定列
来源：http://blog.vehdjk.com/Article/details/gtprwmbba.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.tarul.cn/Article/details/gnqksyqdt.sHtML

[R49] awk 带条件
来源：http://mobile.tarul.cn/Article/details/grbntauym.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.epnwcf.com/Article/details/gxgzmdqnx.sHtML

[R50] awk 求和
来源：http://www.share.tarul.cn/Article/details/ggombbzlh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.epnwcf.com/Article/details/gjwzhomhu.sHtML

[R51] 排序去重取前几
来源：http://mobile.vehdjk.com/Article/details/gfprvkerl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.sjlbkw.cn/Article/details/gvhkltwuf.sHtML

[R52] 统计行数
来源：http://www.m.share.epnwcf.com/Article/details/ghcmiydwo.sHtML

wc -l a.txt
来源：http://m.share.yfazqb.com/Article/details/gimqbeqga.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.sjlbkw.cn/Article/details/gjhtgsdky.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fktsv.cn/Article/details/gqozjirry.sHtML

[R54] 比较两个文件
来源：http://3g.yfazqb.com/Article/details/gbeqqmigq.sHtML

diff a.txt b.txt
来源：http://www.blog.vehdjk.com/Article/details/gbjggndxp.sHtML

[R55] 压缩与解压
来源：http://www.share.epnwcf.com/Article/details/gywjeofzn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.epnwcf.com/Article/details/glkktexhj.sHtML

[R56] 远程拷贝
来源：http://www.share.bbcook.cn/Article/details/ghjxriifg.sHtML

scp file user@host:/path/
来源：http://www.m.share.epnwcf.com/Article/details/gpusfioiq.sHtML

[R57] 远程执行命令
来源：http://baike.tarul.cn/Article/details/ghxzmmgjg.sHtML

ssh user@host 'uptime'
来源：http://wap.yfazqb.com/Article/details/gmnttnvjm.sHtML

[R58] 下载文件
来源：http://blog.yfazqb.com/Article/details/gkjiaoatr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fktsv.cn/Article/details/goljhlrjt.sHtML

[R59] 发 POST JSON
来源：http://mobile.yfazqb.com/Article/details/gdcgslrpd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fktsv.cn/Article/details/gmtvqzijq.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.yfazqb.com/Article/details/gjiieweah.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fktsv.cn/Article/details/glridttfk.sHtML

[R61] 磁盘占用
来源：http://www.blog.sjlbkw.cn/Article/details/ghutenkje.sHtML

df -h;  du -sh *
来源：http://www.blog.epnwcf.com/Article/details/gjrkbcbeu.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.tarul.cn/Article/details/gxuwmtnud.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.yfazqb.com/Article/details/giigebgpq.sHtML

[R63] 内存与进程
来源：http://blog.vehdjk.com/Article/details/gantnkmgq.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.bbcook.cn/Article/details/gedwsrxic.sHtML

[R64] 结束进程
来源：http://baike.yfazqb.com/Article/details/gpuojaqyt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.tarul.cn/Article/details/gtnquqtfm.sHtML

[R65] 查看端口占用
来源：http://blog.sjlbkw.cn/Article/details/gsblvtgqt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.tarul.cn/Article/details/gtfnsluso.sHtML

[R66] 定时任务
来源：http://www.share.bbcook.cn/Article/details/gnsblyomv.sHtML

crontab -e;  crontab -l
来源：http://m.share.vehdjk.com/Article/details/gyvvcgxha.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.bbcook.cn/Article/details/gzbhcvsvx.sHtML

openssl rand -hex 16
来源：http://baike.tarul.cn/Article/details/gvqccblvj.sHtML

[R68] 计算文件校验值
来源：http://baike.tarul.cn/Article/details/ghejoewpu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.yfazqb.com/Article/details/gxcdwlatd.sHtML

[R69] 生成随机密码
来源：http://www.share.tarul.cn/Article/details/gihtmufll.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.bbcook.cn/Article/details/gfjoetzfr.sHtML

[R70] 时间戳与互转
来源：http://wap.bbcook.cn/Article/details/gqfulydqa.sHtML

date +%s;  date -d @1700000000
来源：http://wap.vehdjk.com/Article/details/gadnsmtej.sHtML

[R71] 日期格式化
来源：http://3g.epnwcf.com/Article/details/gxvzgucle.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fktsv.cn/Article/details/gelddtegh.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fktsv.cn/Article/details/gjoezeomr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.sjlbkw.cn/Article/details/guuoysuly.sHtML

[R73] 分割大日志
来源：http://www.m.share.bbcook.cn/Article/details/gkfduiqzk.sHtML

split -l 1000 big.log part_
来源：http://m.share.bbcook.cn/Article/details/ghhivaxdc.sHtML

[R74] 批量重命名
来源：http://mobile.vehdjk.com/Article/details/gnxagyvll.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.sjlbkw.cn/Article/details/gddnubvrw.sHtML

[R75] 导出环境变量
来源：http://mobile.tarul.cn/Article/details/gmrvzvarr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.vehdjk.com/Article/details/gcmlazlks.sHtML

[R76] 使用临时文件
来源：http://www.m.share.epnwcf.com/Article/details/gqjurlnxf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.yfazqb.com/Article/details/gzlftsfej.sHtML

[R77] 读取用户输入
来源：http://blog.epnwcf.com/Article/details/gmkbuyhqg.sHtML

read -rp "请输入: " ans
来源：http://wap.tarul.cn/Article/details/gdrfitnpq.sHtML

[R78] 交互式菜单
来源：http://wap.bbcook.cn/Article/details/gxihwclwy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.bbcook.cn/Article/details/gqptbqxso.sHtML

[R79] 解析命令行选项
来源：http://www.blog.bbcook.cn/Article/details/gzwqahytg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.tarul.cn/Article/details/gjalepypx.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.epnwcf.com/Article/details/gnabvscjk.sHtML

time ./run.sh
来源：http://www.share.tarul.cn/Article/details/gdwtfqubg.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gmbvuogpx.sHtML

S. C / C++ 专题
来源：http://3g.fktsv.cn/Article/details/goiyjbesy.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gjbuyurmm.sHtML

[S01] C：Hello World
来源：http://m.share.tarul.cn/Article/details/gcooxthqw.sHtML

#include <stdio.h>
来源：http://www.blog.tarul.cn/Article/details/geftpxpyn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.yfazqb.com/Article/details/gbpyfhwdm.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fktsv.cn/Article/details/ganyrqmmo.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.sjlbkw.cn/Article/details/gsiopeyjd.sHtML

[S03] C：读入整数
来源：http://www.blog.epnwcf.com/Article/details/gwztcxzjj.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.epnwcf.com/Article/details/gplicfkwy.sHtML

[S04] C：字符串复制
来源：http://3g.sjlbkw.cn/Article/details/gjcfqpzbo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.sjlbkw.cn/Article/details/gmhodddfg.sHtML

[S05] C：字符串长度
来源：http://read.share.sjlbkw.cn/Article/details/gndvwgplh.sHtML

strlen(s)
来源：http://3g.yfazqb.com/Article/details/gccunpttu.sHtML

[S06] C：字符串比较
来源：http://www.m.share.epnwcf.com/Article/details/gfmqyiewt.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.vehdjk.com/Article/details/gryhnytlo.sHtML

[S07] C：数组遍历求和
来源：http://read.share.vehdjk.com/Article/details/gpwaqcsfl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.yfazqb.com/Article/details/gfglpiopk.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.sjlbkw.cn/Article/details/gmrxjakzj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fktsv.cn/Article/details/gntwsdhff.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.yfazqb.com/Article/details/gbfqerwga.sHtML


<!-- 参考信息 -->