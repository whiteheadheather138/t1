代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.epnwcf.com/Article/details/gwsywphor.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.bbcook.cn/Article/details/gkrbxclnq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.yfazqb.com/Article/details/gtgfbgzjc.sHtML

[Q41] 多表连接
来源：http://blog.yfazqb.com/Article/details/ghpmvjcea.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fktsv.cn/Article/details/grnldvvnx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.bbcook.cn/Article/details/gyymmnvmo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fktsv.cn/Article/details/gtctjacks.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.sjlbkw.cn/Article/details/grvsiazoa.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fktsv.cn/Article/details/gsfaxevke.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.tarul.cn/Article/details/gxcicsiqz.sHtML

[Q43] 标量子查询
来源：http://baike.yfazqb.com/Article/details/gjymkjfhz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.yfazqb.com/Article/details/ggiyjmnkq.sHtML

[Q44] IN 子查询
来源：http://www.m.share.vehdjk.com/Article/details/gcmfcybmx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fktsv.cn/Article/details/glrfauiex.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.tarul.cn/Article/details/gnnleiqbf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.tarul.cn/Article/details/glcaswywl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.vehdjk.com/Article/details/gfqjtwwry.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fktsv.cn/Article/details/gdfkzjvgv.sHtML

[Q47] 与平均值比较
来源：http://3g.sjlbkw.cn/Article/details/gqtobyfiv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.tarul.cn/Article/details/gkwgnkzie.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fktsv.cn/Article/details/gdaatoijg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.tarul.cn/Article/details/gafapxisb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.vehdjk.com/Article/details/gppqedkbp.sHtML

[Q49] 更新单行
来源：http://read.share.epnwcf.com/Article/details/gzhrzzqtv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.tarul.cn/Article/details/gjbgegrha.sHtML

[Q50] 批量更新
来源：http://m.share.tarul.cn/Article/details/glwgqokze.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fktsv.cn/Article/details/gcongsnmt.sHtML

[Q51] 用子查询更新
来源：http://blog.fktsv.cn/Article/details/gdhbfwtbp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.yfazqb.com/Article/details/gukkuijft.sHtML

[Q52] 删除指定行
来源：http://3g.sjlbkw.cn/Article/details/gijjmjlae.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.bbcook.cn/Article/details/ggrtueyrr.sHtML

[Q53] 按条件删除
来源：http://wap.yfazqb.com/Article/details/gdorsdais.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.epnwcf.com/Article/details/gpyewzicz.sHtML

[Q54] 清空表
来源：http://www.blog.sjlbkw.cn/Article/details/gwovkhqjc.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fktsv.cn/Article/details/gieecmphk.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.tarul.cn/Article/details/gyhyijcqh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.vehdjk.com/Article/details/galgxspza.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fktsv.cn/Article/details/gkxacogpz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.sjlbkw.cn/Article/details/gwddewtar.sHtML

[Q57] 行号
来源：http://www.blog.epnwcf.com/Article/details/gphcgyhbh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.epnwcf.com/Article/details/giurxdfnv.sHtML

[Q58] 累计求和
来源：http://www.m.share.sjlbkw.cn/Article/details/gqbvxpalk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.vehdjk.com/Article/details/gtjzgbtuq.sHtML

[Q59] 分组内累计
来源：http://blog.vehdjk.com/Article/details/gzbabimza.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/gxqfeoghy.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fktsv.cn/Article/details/gjtttnfbc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.sjlbkw.cn/Article/details/gknbyttwm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.yfazqb.com/Article/details/galrnpfvu.sHtML

[Q61] 移动平均
来源：http://baike.epnwcf.com/Article/details/gwtlydvxf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/gsoegshwe.sHtML

[Q62] 分组占比
来源：http://baike.tarul.cn/Article/details/gygqoswod.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.vehdjk.com/Article/details/goxxqivys.sHtML

[Q63] 开启事务
来源：http://www.share.tarul.cn/Article/details/gwcrxitjo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.tarul.cn/Article/details/glwelrslk.sHtML

[Q64] 提交事务
来源：http://blog.yfazqb.com/Article/details/gppotsntp.sHtML

COMMIT;
来源：http://www.blog.vehdjk.com/Article/details/gatykvhnu.sHtML

[Q65] 回滚事务
来源：http://mobile.epnwcf.com/Article/details/gxbizzmfo.sHtML

ROLLBACK;
来源：http://blog.tarul.cn/Article/details/ggeenwlnv.sHtML

[Q66] 行锁查询
来源：http://3g.yfazqb.com/Article/details/gorivjqjl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.yfazqb.com/Article/details/gnwisyjvs.sHtML

[Q67] 设置隔离级别
来源：http://read.share.yfazqb.com/Article/details/gkxkwetlc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.vehdjk.com/Article/details/gwvapgqoo.sHtML

[Q68] 保存点
来源：http://www.m.share.vehdjk.com/Article/details/gxmxylsil.sHtML

SAVEPOINT sp1;
来源：http://www.blog.sjlbkw.cn/Article/details/gejkvrbkn.sHtML

ROLLBACK TO sp1;
来源：http://3g.vehdjk.com/Article/details/gyyhovjau.sHtML

[Q69] 查看执行计划
来源：http://read.share.epnwcf.com/Article/details/gsudvjkqw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.vehdjk.com/Article/details/gawevnypw.sHtML

[Q70] 更新统计信息
来源：http://baike.epnwcf.com/Article/details/glegpfooj.sHtML

ANALYZE TABLE users;
来源：http://m.share.yfazqb.com/Article/details/gvfpmtnxt.sHtML

[Q71] 查看建表语句
来源：http://www.blog.bbcook.cn/Article/details/gybaxhntm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.vehdjk.com/Article/details/gcgjkjkcj.sHtML

[Q72] 查看索引
来源：http://www.share.tarul.cn/Article/details/goqteglsm.sHtML

SHOW INDEX FROM users;
来源：http://www.share.yfazqb.com/Article/details/gnkfvmfgv.sHtML

[Q73] 查看表状态
来源：http://mobile.sjlbkw.cn/Article/details/gwjlvlprj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.yfazqb.com/Article/details/gehwtfcmh.sHtML

[Q74] 强制使用索引
来源：http://www.blog.bbcook.cn/Article/details/gokkanfoz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.epnwcf.com/Article/details/ggbuxhnia.sHtML

[Q75] 日期格式化
来源：http://3g.vehdjk.com/Article/details/gtzdxijtj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fktsv.cn/Article/details/gsbhzdrke.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.vehdjk.com/Article/details/gglyohwqo.sHtML

[Q76] 按天统计
来源：http://mobile.fktsv.cn/Article/details/gcojakocw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.yfazqb.com/Article/details/gtooemrcs.sHtML

[Q77] 时间加减
来源：http://read.share.epnwcf.com/Article/details/gyjvbijdd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.yfazqb.com/Article/details/gbilgpuvl.sHtML

[Q78] 当前时间
来源：http://baike.yfazqb.com/Article/details/ggsvvvltp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.epnwcf.com/Article/details/ggxmbpmks.sHtML

[Q79] 字符串拼接
来源：http://m.share.sjlbkw.cn/Article/details/gmxkdoedd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.tarul.cn/Article/details/gzsyemmcw.sHtML

[Q80] 字符串截取
来源：http://www.share.fktsv.cn/Article/details/gtjfaihwe.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.epnwcf.com/Article/details/gswmhtavw.sHtML

[Q81] 字符串替换
来源：http://m.share.bbcook.cn/Article/details/giqlucrox.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.bbcook.cn/Article/details/gccwpckzz.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.epnwcf.com/Article/details/gozkcvkep.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.epnwcf.com/Article/details/gokizeick.sHtML

[Q83] 大小写转换
来源：http://www.m.share.yfazqb.com/Article/details/gdhdplqts.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/geshuoylz.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.sjlbkw.cn/Article/details/gtagbmdaf.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.yfazqb.com/Article/details/gxxohoasf.sHtML

[Q85] 数值取整
来源：http://baike.tarul.cn/Article/details/gdzgfueir.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.sjlbkw.cn/Article/details/gbwfrboov.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.bbcook.cn/Article/details/gbmsjgsvz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.vehdjk.com/Article/details/gknhcxfwc.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.yfazqb.com/Article/details/gdqmfygyg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.tarul.cn/Article/details/goioiujzu.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fktsv.cn/Article/details/ghieshjct.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fktsv.cn/Article/details/gofclenkv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fktsv.cn/Article/details/glhfqllmw.sHtML

[Q89] 判断表是否存在
来源：http://3g.yfazqb.com/Article/details/gybjepbto.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.yfazqb.com/Article/details/gjzbgtiry.sHtML

[Q90] 生成序号列
来源：http://3g.vehdjk.com/Article/details/gwzqlfmoo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.sjlbkw.cn/Article/details/gqisnlive.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gdiametef.sHtML

R. Bash 专题
来源：http://blog.vehdjk.com/Article/details/gdhrtkjiz.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gcvexklsx.sHtML

[R01] shebang 与严格模式
来源：http://m.share.tarul.cn/Article/details/gtzokucqw.sHtML

#!/usr/bin/env bash
来源：http://read.share.tarul.cn/Article/details/glnxotbza.sHtML

set -euo pipefail
来源：http://www.share.bbcook.cn/Article/details/gxrwseesz.sHtML

[R02] 变量赋值与使用
来源：http://blog.tarul.cn/Article/details/gnlcfmrey.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.bbcook.cn/Article/details/gleyjhiiy.sHtML

[R03] 只读变量
来源：http://blog.tarul.cn/Article/details/gszmogmdt.sHtML

readonly PI=3.14
来源：http://wap.epnwcf.com/Article/details/grsahnbfs.sHtML

[R04] 位置参数
来源：http://www.m.share.yfazqb.com/Article/details/ghjruesqd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.bbcook.cn/Article/details/gqlrwynxo.sHtML

[R05] 参数默认值
来源：http://baike.fktsv.cn/Article/details/gzqzhtism.sHtML

name="${1:-default}"
来源：http://www.blog.tarul.cn/Article/details/gunotbnjd.sHtML

[R06] 判断命令是否存在
来源：http://www.share.vehdjk.com/Article/details/gqlaklsyu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.epnwcf.com/Article/details/gxjdnvxlv.sHtML

[R07] if 判断文件
来源：http://www.blog.sjlbkw.cn/Article/details/gsvyzqcya.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.tarul.cn/Article/details/godumxewf.sHtML

[R08] 数值比较
来源：http://www.blog.yfazqb.com/Article/details/gzgvrhvbs.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.epnwcf.com/Article/details/gasuhkxxw.sHtML

[R09] 字符串比较
来源：http://3g.yfazqb.com/Article/details/gkvfmwypx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fktsv.cn/Article/details/gccgnqtnn.sHtML

[R10] 正则匹配
来源：http://baike.tarul.cn/Article/details/guyvfmlrk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.yfazqb.com/Article/details/ghigmnjft.sHtML

[R11] case 多分支
来源：http://m.share.sjlbkw.cn/Article/details/gwpjpthvd.sHtML

case "$1" in
来源：http://3g.sjlbkw.cn/Article/details/gwsdsusyi.sHtML

start) echo "启动" ;;
来源：http://www.share.fktsv.cn/Article/details/gglinnhcr.sHtML

stop)  echo "停止" ;;
来源：http://read.share.vehdjk.com/Article/details/gnpfqspji.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.sjlbkw.cn/Article/details/gucmbrycp.sHtML

esac
来源：http://read.share.tarul.cn/Article/details/gdlbnrhyb.sHtML

[R12] for 遍历文件
来源：http://www.blog.bbcook.cn/Article/details/gnxnsebce.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.bbcook.cn/Article/details/gbwdbnxko.sHtML

[R13] for 计数循环
来源：http://blog.yfazqb.com/Article/details/gtomqtldz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.vehdjk.com/Article/details/gmvjbpqwn.sHtML

[R14] C 风格 for
来源：http://3g.epnwcf.com/Article/details/gwsvpmbzd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fktsv.cn/Article/details/gufcebhri.sHtML

[R15] while 逐行读文件
来源：http://baike.fktsv.cn/Article/details/gnnglkycz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.yfazqb.com/Article/details/gxwjasdwk.sHtML

[R16] until 等待条件
来源：http://www.share.bbcook.cn/Article/details/gbaasmzij.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gampglgib.sHtML

[R17] 数组定义与取值
来源：http://www.blog.bbcook.cn/Article/details/gzixkrmji.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.vehdjk.com/Article/details/ghabupwyw.sHtML

[R18] 遍历数组
来源：http://wap.sjlbkw.cn/Article/details/ggyimbvzg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.yfazqb.com/Article/details/ggrmiibdz.sHtML

[R19] 数组长度
来源：http://read.share.sjlbkw.cn/Article/details/glbwvcvuu.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fktsv.cn/Article/details/gabafgmah.sHtML

[R20] 关联数组（字典）
来源：http://www.share.tarul.cn/Article/details/genduahup.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.tarul.cn/Article/details/glqnvlkvy.sHtML

[R21] 字符串长度
来源：http://m.share.tarul.cn/Article/details/gvbyltjho.sHtML

echo "${#s}"
来源：http://baike.epnwcf.com/Article/details/gfntivfpv.sHtML

[R22] 截取子串
来源：http://www.share.yfazqb.com/Article/details/gppvfdzly.sHtML

echo "${s:0:5}"
来源：http://m.share.tarul.cn/Article/details/grtydosrb.sHtML

[R23] 字符串替换
来源：http://www.m.share.fktsv.cn/Article/details/gegohfmeh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fktsv.cn/Article/details/gidxkhhtb.sHtML

[R24] 大小写转换
来源：http://baike.epnwcf.com/Article/details/gjxfvskgv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.tarul.cn/Article/details/ggtdpoziz.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.epnwcf.com/Article/details/gwidgxflk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.vehdjk.com/Article/details/gxcvgyskh.sHtML

[R26] 命令替换
来源：http://www.share.epnwcf.com/Article/details/goarxicqd.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.epnwcf.com/Article/details/gnjdvtrwg.sHtML

[R27] 算术展开
来源：http://m.share.bbcook.cn/Article/details/gyhndnxmv.sHtML

echo $((1 + 2 * 3))
来源：http://wap.yfazqb.com/Article/details/giaellkcq.sHtML

[R28] 浮点运算
来源：http://m.share.vehdjk.com/Article/details/gnmaphmkw.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.sjlbkw.cn/Article/details/grpkxwxxh.sHtML

[R29] 定义函数
来源：http://blog.yfazqb.com/Article/details/gvojbwtld.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.bbcook.cn/Article/details/grmehoptw.sHtML

[R30] 函数返回状态码
来源：http://www.share.epnwcf.com/Article/details/ghqhoreej.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.sjlbkw.cn/Article/details/gsahhrnvy.sHtML

[R31] 局部变量
来源：http://baike.yfazqb.com/Article/details/gsjwhlapo.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.epnwcf.com/Article/details/gqutqmohq.sHtML

[R32] 参数个数校验
来源：http://mobile.sjlbkw.cn/Article/details/gaayzvjuw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.tarul.cn/Article/details/gzqqmodww.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.bbcook.cn/Article/details/guugqeqvt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.epnwcf.com/Article/details/gwzupslqm.sHtML

[R34] 退出时清理
来源：http://www.m.share.fktsv.cn/Article/details/gduxlqchf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.vehdjk.com/Article/details/gcbkzaeys.sHtML

[R35] 后台执行并等待
来源：http://3g.vehdjk.com/Article/details/gjharqvno.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.tarul.cn/Article/details/gzyphylya.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.vehdjk.com/Article/details/guyqnvpdj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.bbcook.cn/Article/details/gqklxqwoi.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.yfazqb.com/Article/details/gjlkiajuy.sHtML

files=$(ls -1)
来源：http://baike.epnwcf.com/Article/details/grmsdprzo.sHtML

[R38] 管道串联
来源：http://www.share.bbcook.cn/Article/details/gxtphpmwh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.epnwcf.com/Article/details/gggsvjetd.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.tarul.cn/Article/details/gwlpgcrzf.sHtML

cmd > out.log 2>&1
来源：http://www.share.bbcook.cn/Article/details/gptvegciq.sHtML

[R40] 追加写日志
来源：http://www.m.share.bbcook.cn/Article/details/gbmqvoghv.sHtML

echo "log" >> out.log
来源：http://www.blog.yfazqb.com/Article/details/goqtbpmea.sHtML

[R41] 丢弃输出
来源：http://blog.fktsv.cn/Article/details/gdglxhtyl.sHtML

cmd >/dev/null 2>&1
来源：http://baike.bbcook.cn/Article/details/ggbxliiuf.sHtML

[R42] 输入重定向
来源：http://blog.yfazqb.com/Article/details/gngwoqcqy.sHtML

wc -l < a.txt
来源：http://m.share.bbcook.cn/Article/details/gwmhlkkct.sHtML

[R43] 按名字查找文件
来源：http://baike.vehdjk.com/Article/details/gsqtpuaxb.sHtML

find . -name "*.log" -type f
来源：http://wap.sjlbkw.cn/Article/details/gbvaopbyp.sHtML

[R44] 按修改时间查找
来源：http://3g.bbcook.cn/Article/details/gyakntttq.sHtML

find . -mtime -7 -type f
来源：http://www.blog.bbcook.cn/Article/details/gwdiprkly.sHtML

[R45] 批量删除
来源：http://www.share.yfazqb.com/Article/details/gummxvquo.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.yfazqb.com/Article/details/grvjpmxig.sHtML

[R46] 递归替换文件内容
来源：http://read.share.bbcook.cn/Article/details/grhynaomt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.sjlbkw.cn/Article/details/gawaycqxc.sHtML

[R47] sed 单行替换
来源：http://blog.vehdjk.com/Article/details/gjhxuppbt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.vehdjk.com/Article/details/gtvdfgvux.sHtML

[R48] awk 取指定列
来源：http://3g.fktsv.cn/Article/details/gphsabtec.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gzctgqtfw.sHtML

[R49] awk 带条件
来源：http://blog.epnwcf.com/Article/details/gnajjdamb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.epnwcf.com/Article/details/guqldosfn.sHtML

[R50] awk 求和
来源：http://wap.tarul.cn/Article/details/gentkxshp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.sjlbkw.cn/Article/details/guocprfvb.sHtML

[R51] 排序去重取前几
来源：http://baike.yfazqb.com/Article/details/grmpkomec.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.vehdjk.com/Article/details/gefqvjjpv.sHtML

[R52] 统计行数
来源：http://mobile.vehdjk.com/Article/details/gxwpiiidr.sHtML

wc -l a.txt
来源：http://mobile.sjlbkw.cn/Article/details/gnfcjregu.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fktsv.cn/Article/details/gcvgwmirb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.epnwcf.com/Article/details/gbmpxdmwx.sHtML

[R54] 比较两个文件
来源：http://m.share.bbcook.cn/Article/details/gydpdpcmq.sHtML

diff a.txt b.txt
来源：http://blog.tarul.cn/Article/details/gpthgozph.sHtML

[R55] 压缩与解压
来源：http://m.share.vehdjk.com/Article/details/ggqsosdvm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.tarul.cn/Article/details/gdvaqjtez.sHtML

[R56] 远程拷贝
来源：http://wap.vehdjk.com/Article/details/gqjwnvjaw.sHtML

scp file user@host:/path/
来源：http://www.share.tarul.cn/Article/details/gnlhroatl.sHtML

[R57] 远程执行命令
来源：http://read.share.fktsv.cn/Article/details/ggatzaxpm.sHtML

ssh user@host 'uptime'
来源：http://blog.fktsv.cn/Article/details/gjhdwnvnu.sHtML

[R58] 下载文件
来源：http://mobile.fktsv.cn/Article/details/giarwenbk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.bbcook.cn/Article/details/gkxyuxlbr.sHtML

[R59] 发 POST JSON
来源：http://mobile.vehdjk.com/Article/details/gzqztxnkq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fktsv.cn/Article/details/gjdlpkjww.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fktsv.cn/Article/details/gassyvomk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.vehdjk.com/Article/details/gelvmnyxc.sHtML

[R61] 磁盘占用
来源：http://wap.sjlbkw.cn/Article/details/gbuvubwum.sHtML

df -h;  du -sh *
来源：http://3g.yfazqb.com/Article/details/gekbeouxz.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gqzeiawpp.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.tarul.cn/Article/details/gfcxzehxk.sHtML

[R63] 内存与进程
来源：http://wap.bbcook.cn/Article/details/gwkgnegvf.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.sjlbkw.cn/Article/details/gxpvvykqf.sHtML

[R64] 结束进程
来源：http://blog.yfazqb.com/Article/details/ghzkauxkt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.yfazqb.com/Article/details/grzfbzdft.sHtML

[R65] 查看端口占用
来源：http://read.share.tarul.cn/Article/details/gowmcnvvv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.yfazqb.com/Article/details/gkwsdtsfp.sHtML

[R66] 定时任务
来源：http://m.share.yfazqb.com/Article/details/gnzzymcha.sHtML

crontab -e;  crontab -l
来源：http://mobile.epnwcf.com/Article/details/ghxxkvflc.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.yfazqb.com/Article/details/gqbxohbpv.sHtML

openssl rand -hex 16
来源：http://www.blog.vehdjk.com/Article/details/gdciagjob.sHtML

[R68] 计算文件校验值
来源：http://wap.vehdjk.com/Article/details/geqaeejly.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.vehdjk.com/Article/details/gzzuucwaz.sHtML

[R69] 生成随机密码
来源：http://3g.bbcook.cn/Article/details/gbkehartd.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fktsv.cn/Article/details/gfnsrllkb.sHtML

[R70] 时间戳与互转
来源：http://www.share.yfazqb.com/Article/details/glsiqnqgt.sHtML

date +%s;  date -d @1700000000
来源：http://baike.tarul.cn/Article/details/gkcssofdq.sHtML

[R71] 日期格式化
来源：http://www.blog.sjlbkw.cn/Article/details/gxccqaeub.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.tarul.cn/Article/details/gowttasan.sHtML

[R72] 等待端口就绪
来源：http://wap.epnwcf.com/Article/details/gmpduyosl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fktsv.cn/Article/details/garketvqk.sHtML

[R73] 分割大日志
来源：http://www.m.share.fktsv.cn/Article/details/gqlcnzoyr.sHtML

split -l 1000 big.log part_
来源：http://www.share.tarul.cn/Article/details/gwgwmetes.sHtML

[R74] 批量重命名
来源：http://wap.sjlbkw.cn/Article/details/gpfkhlplz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.epnwcf.com/Article/details/gzqgpdjyq.sHtML

[R75] 导出环境变量
来源：http://m.share.sjlbkw.cn/Article/details/gfiovclis.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.vehdjk.com/Article/details/gwyzsqnbd.sHtML

[R76] 使用临时文件
来源：http://baike.vehdjk.com/Article/details/glcqtrgrw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.epnwcf.com/Article/details/gunmkdwbo.sHtML

[R77] 读取用户输入
来源：http://www.blog.fktsv.cn/Article/details/gnrcxknyj.sHtML

read -rp "请输入: " ans
来源：http://m.share.tarul.cn/Article/details/gvoocajfs.sHtML

[R78] 交互式菜单
来源：http://baike.tarul.cn/Article/details/gmfkvokov.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.yfazqb.com/Article/details/gomrfvbaz.sHtML

[R79] 解析命令行选项
来源：http://www.share.fktsv.cn/Article/details/glztpysub.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.epnwcf.com/Article/details/gexbubmsc.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.bbcook.cn/Article/details/gsmvgicxb.sHtML

time ./run.sh
来源：http://www.share.tarul.cn/Article/details/gytvnoyyb.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gmalgcwoo.sHtML

S. C / C++ 专题
来源：http://blog.fktsv.cn/Article/details/gasdmosen.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gvnzhvxpi.sHtML

[S01] C：Hello World
来源：http://blog.fktsv.cn/Article/details/gkfvkdcwt.sHtML

#include <stdio.h>
来源：http://wap.tarul.cn/Article/details/gncsdewsr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.yfazqb.com/Article/details/gdholrltx.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.bbcook.cn/Article/details/gmaoybdor.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.yfazqb.com/Article/details/gdabgbavc.sHtML

[S03] C：读入整数
来源：http://wap.epnwcf.com/Article/details/gbdfklspi.sHtML

int x; scanf("%d", &x);
来源：http://baike.vehdjk.com/Article/details/gdbghqjan.sHtML

[S04] C：字符串复制
来源：http://read.share.fktsv.cn/Article/details/giznzcced.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fktsv.cn/Article/details/gvnmlioqo.sHtML

[S05] C：字符串长度
来源：http://mobile.fktsv.cn/Article/details/geqynprbh.sHtML

strlen(s)
来源：http://www.share.yfazqb.com/Article/details/ghpecqbko.sHtML

[S06] C：字符串比较
来源：http://www.blog.tarul.cn/Article/details/gfuxxiuqh.sHtML

strcmp(a, b) == 0
来源：http://baike.bbcook.cn/Article/details/gmtriqmol.sHtML

[S07] C：数组遍历求和
来源：http://3g.fktsv.cn/Article/details/gtmwpbwyn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.vehdjk.com/Article/details/gwwygvwlx.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.sjlbkw.cn/Article/details/gxeajszdl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.bbcook.cn/Article/details/gdrfkrddz.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.vehdjk.com/Article/details/gtcndqokd.sHtML


<!-- 参考信息 -->