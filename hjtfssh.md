代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.epnwcf.com/Article/details/gajhzngmj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.epnwcf.com/Article/details/gdvpilazs.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fktsv.cn/Article/details/giyqfwhmu.sHtML

[Q41] 多表连接
来源：http://m.share.fktsv.cn/Article/details/gouomahzf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.sjlbkw.cn/Article/details/gyltfrxur.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.yfazqb.com/Article/details/gkclsrcmk.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.sjlbkw.cn/Article/details/ggzchvqqt.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.sjlbkw.cn/Article/details/grnwghzyk.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fktsv.cn/Article/details/gvwcewfiy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fktsv.cn/Article/details/gnxxilpxv.sHtML

[Q43] 标量子查询
来源：http://www.blog.fktsv.cn/Article/details/gcmoxibnr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.yfazqb.com/Article/details/gulokzdfo.sHtML

[Q44] IN 子查询
来源：http://3g.bbcook.cn/Article/details/gqcolfnec.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.yfazqb.com/Article/details/gwslcvgen.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.bbcook.cn/Article/details/gimjpicgq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.yfazqb.com/Article/details/gfrryltsw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.vehdjk.com/Article/details/gulhjlhlp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.epnwcf.com/Article/details/gvwisxpeb.sHtML

[Q47] 与平均值比较
来源：http://baike.yfazqb.com/Article/details/gpdnqcmlk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fktsv.cn/Article/details/gqmrtnsnt.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.yfazqb.com/Article/details/geexngqwj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.yfazqb.com/Article/details/glemmvaxa.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.sjlbkw.cn/Article/details/gfvdsqstl.sHtML

[Q49] 更新单行
来源：http://baike.tarul.cn/Article/details/gfekowzqg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.tarul.cn/Article/details/gxymkumcr.sHtML

[Q50] 批量更新
来源：http://m.share.vehdjk.com/Article/details/gmzbxmdua.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.vehdjk.com/Article/details/grbrhxeei.sHtML

[Q51] 用子查询更新
来源：http://wap.vehdjk.com/Article/details/ghoxzsndb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gucchlxhm.sHtML

[Q52] 删除指定行
来源：http://www.blog.vehdjk.com/Article/details/gbgsqmeiu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fktsv.cn/Article/details/getvxcuik.sHtML

[Q53] 按条件删除
来源：http://www.m.share.vehdjk.com/Article/details/gmkmpqerq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.bbcook.cn/Article/details/gyadczpbm.sHtML

[Q54] 清空表
来源：http://m.share.sjlbkw.cn/Article/details/gchxnczkr.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.epnwcf.com/Article/details/gbymvhbdb.sHtML

[Q55] 排名（并列占位）
来源：http://wap.bbcook.cn/Article/details/ggqaugymg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.epnwcf.com/Article/details/gwcfxzaom.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.epnwcf.com/Article/details/grvqlztwv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fktsv.cn/Article/details/gupwvgdtd.sHtML

[Q57] 行号
来源：http://www.m.share.yfazqb.com/Article/details/gybhdonid.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.bbcook.cn/Article/details/gptycxxtr.sHtML

[Q58] 累计求和
来源：http://www.m.share.epnwcf.com/Article/details/grhfrcglf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.tarul.cn/Article/details/glfdmjvmg.sHtML

[Q59] 分组内累计
来源：http://www.share.bbcook.cn/Article/details/gidcxtqhc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.tarul.cn/Article/details/galhsntpv.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.sjlbkw.cn/Article/details/grfypczfc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fktsv.cn/Article/details/ggayhjjfl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.yfazqb.com/Article/details/gofxnupxg.sHtML

[Q61] 移动平均
来源：http://3g.yfazqb.com/Article/details/gofdhbgiy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.epnwcf.com/Article/details/gncqwqkvi.sHtML

[Q62] 分组占比
来源：http://blog.vehdjk.com/Article/details/gtcyqxrmc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.epnwcf.com/Article/details/gbnlbmijf.sHtML

[Q63] 开启事务
来源：http://www.m.share.fktsv.cn/Article/details/gnqeyayiq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.tarul.cn/Article/details/gekztvhgs.sHtML

[Q64] 提交事务
来源：http://mobile.fktsv.cn/Article/details/gyvstijmw.sHtML

COMMIT;
来源：http://3g.epnwcf.com/Article/details/gevipkfog.sHtML

[Q65] 回滚事务
来源：http://www.m.share.sjlbkw.cn/Article/details/gexyynvaf.sHtML

ROLLBACK;
来源：http://blog.bbcook.cn/Article/details/goppehoix.sHtML

[Q66] 行锁查询
来源：http://mobile.sjlbkw.cn/Article/details/gpdewidpb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.sjlbkw.cn/Article/details/gitpuaigs.sHtML

[Q67] 设置隔离级别
来源：http://mobile.yfazqb.com/Article/details/gzmyffhak.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.vehdjk.com/Article/details/glhwovqyk.sHtML

[Q68] 保存点
来源：http://baike.yfazqb.com/Article/details/gxcuodtpc.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.epnwcf.com/Article/details/gcglmjmxg.sHtML

ROLLBACK TO sp1;
来源：http://baike.fktsv.cn/Article/details/gqojlbdzw.sHtML

[Q69] 查看执行计划
来源：http://read.share.tarul.cn/Article/details/gmltcberc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fktsv.cn/Article/details/grhenwojm.sHtML

[Q70] 更新统计信息
来源：http://read.share.yfazqb.com/Article/details/gjpuseayq.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gxucgpwvr.sHtML

[Q71] 查看建表语句
来源：http://read.share.sjlbkw.cn/Article/details/gmudjniir.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.bbcook.cn/Article/details/ghxwmelrm.sHtML

[Q72] 查看索引
来源：http://mobile.yfazqb.com/Article/details/gzozasqwq.sHtML

SHOW INDEX FROM users;
来源：http://baike.epnwcf.com/Article/details/gtbxefmbx.sHtML

[Q73] 查看表状态
来源：http://wap.bbcook.cn/Article/details/gwpfhlhlo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.yfazqb.com/Article/details/gkdbqebzz.sHtML

[Q74] 强制使用索引
来源：http://3g.yfazqb.com/Article/details/gvyphzsje.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.epnwcf.com/Article/details/gmnjxdlqc.sHtML

[Q75] 日期格式化
来源：http://www.share.tarul.cn/Article/details/gxfrapimt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.vehdjk.com/Article/details/gjxvzkswl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.bbcook.cn/Article/details/gbscsaden.sHtML

[Q76] 按天统计
来源：http://blog.vehdjk.com/Article/details/gbgtgfwmq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.vehdjk.com/Article/details/grjswphsb.sHtML

[Q77] 时间加减
来源：http://www.share.yfazqb.com/Article/details/gllgsvaug.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.tarul.cn/Article/details/gjwkopbkt.sHtML

[Q78] 当前时间
来源：http://mobile.fktsv.cn/Article/details/gvadsmcty.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.yfazqb.com/Article/details/gsxzzqfwl.sHtML

[Q79] 字符串拼接
来源：http://wap.vehdjk.com/Article/details/gekaimblo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.tarul.cn/Article/details/gdkxtiwhi.sHtML

[Q80] 字符串截取
来源：http://3g.bbcook.cn/Article/details/gvmipkxus.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gajssomnw.sHtML

[Q81] 字符串替换
来源：http://www.share.epnwcf.com/Article/details/gcdcjtwoq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/geomglftb.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.bbcook.cn/Article/details/giuowvqgs.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.vehdjk.com/Article/details/gkstwvxtl.sHtML

[Q83] 大小写转换
来源：http://read.share.yfazqb.com/Article/details/gsytdnnes.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gtamlmxdg.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.epnwcf.com/Article/details/guzxfcltx.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.epnwcf.com/Article/details/gbipwzkwx.sHtML

[Q85] 数值取整
来源：http://www.share.epnwcf.com/Article/details/gqkukednw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.epnwcf.com/Article/details/gpdxgkwrb.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fktsv.cn/Article/details/gxolcivew.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fktsv.cn/Article/details/gxohrkkmh.sHtML

[Q87] JSON 字段做条件
来源：http://baike.sjlbkw.cn/Article/details/gmzcpaecw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.yfazqb.com/Article/details/gmclxffuj.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.sjlbkw.cn/Article/details/gkvbavetf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.vehdjk.com/Article/details/ghkozlpbv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fktsv.cn/Article/details/gjyugncqc.sHtML

[Q89] 判断表是否存在
来源：http://www.share.sjlbkw.cn/Article/details/gmujodvek.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.yfazqb.com/Article/details/gzlrktflx.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fktsv.cn/Article/details/ggdwftpmr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.yfazqb.com/Article/details/gmfpxjaxg.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gluzeeuyg.sHtML

R. Bash 专题
来源：http://www.m.share.sjlbkw.cn/Article/details/gxrkmrgcn.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gabpyigzl.sHtML

[R01] shebang 与严格模式
来源：http://mobile.epnwcf.com/Article/details/guaqjzhsp.sHtML

#!/usr/bin/env bash
来源：http://mobile.tarul.cn/Article/details/gqiewvori.sHtML

set -euo pipefail
来源：http://wap.vehdjk.com/Article/details/gqktrdqyx.sHtML

[R02] 变量赋值与使用
来源：http://m.share.epnwcf.com/Article/details/gaqetexrn.sHtML

name="Tom"; echo "$name"
来源：http://mobile.epnwcf.com/Article/details/glmehxiqa.sHtML

[R03] 只读变量
来源：http://mobile.epnwcf.com/Article/details/gjspxbybh.sHtML

readonly PI=3.14
来源：http://www.m.share.epnwcf.com/Article/details/gdqxztqxu.sHtML

[R04] 位置参数
来源：http://mobile.epnwcf.com/Article/details/gotxqcumd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.sjlbkw.cn/Article/details/gqdamukjf.sHtML

[R05] 参数默认值
来源：http://read.share.epnwcf.com/Article/details/gipixwjqf.sHtML

name="${1:-default}"
来源：http://www.share.yfazqb.com/Article/details/gexecfecp.sHtML

[R06] 判断命令是否存在
来源：http://blog.yfazqb.com/Article/details/gczcgphad.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.bbcook.cn/Article/details/gufkxlbwu.sHtML

[R07] if 判断文件
来源：http://m.share.bbcook.cn/Article/details/gkgakgsca.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.bbcook.cn/Article/details/glzioclbn.sHtML

[R08] 数值比较
来源：http://mobile.vehdjk.com/Article/details/godkmulss.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.sjlbkw.cn/Article/details/gjkzwlmwx.sHtML

[R09] 字符串比较
来源：http://m.share.fktsv.cn/Article/details/gbhwhipyz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fktsv.cn/Article/details/gisfjgfcf.sHtML

[R10] 正则匹配
来源：http://mobile.tarul.cn/Article/details/gngwjmfji.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.epnwcf.com/Article/details/gqpxrgwkx.sHtML

[R11] case 多分支
来源：http://mobile.sjlbkw.cn/Article/details/giupkdbbm.sHtML

case "$1" in
来源：http://www.share.yfazqb.com/Article/details/gqeccyugw.sHtML

start) echo "启动" ;;
来源：http://blog.yfazqb.com/Article/details/gbdahhqdy.sHtML

stop)  echo "停止" ;;
来源：http://mobile.epnwcf.com/Article/details/gnkppajde.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fktsv.cn/Article/details/guoxybcat.sHtML

esac
来源：http://www.blog.sjlbkw.cn/Article/details/gkvsuhflt.sHtML

[R12] for 遍历文件
来源：http://www.m.share.bbcook.cn/Article/details/gsdsidyvk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fktsv.cn/Article/details/gkwineria.sHtML

[R13] for 计数循环
来源：http://blog.fktsv.cn/Article/details/gudfnxiey.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.sjlbkw.cn/Article/details/gytnodyat.sHtML

[R14] C 风格 for
来源：http://m.share.bbcook.cn/Article/details/gobmaoqrl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.sjlbkw.cn/Article/details/grzfsymzg.sHtML

[R15] while 逐行读文件
来源：http://www.blog.vehdjk.com/Article/details/geonvftvv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.bbcook.cn/Article/details/goasvatyz.sHtML

[R16] until 等待条件
来源：http://www.m.share.bbcook.cn/Article/details/gsirzgtwt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.vehdjk.com/Article/details/gxaaqxkbv.sHtML

[R17] 数组定义与取值
来源：http://read.share.fktsv.cn/Article/details/guyzmmdtw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.epnwcf.com/Article/details/gcuzwpiex.sHtML

[R18] 遍历数组
来源：http://www.m.share.bbcook.cn/Article/details/ghksqusdw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.yfazqb.com/Article/details/glmlcpbng.sHtML

[R19] 数组长度
来源：http://m.share.vehdjk.com/Article/details/gudoepggj.sHtML

echo "${#arr[@]}"
来源：http://www.share.tarul.cn/Article/details/gyketayev.sHtML

[R20] 关联数组（字典）
来源：http://m.share.sjlbkw.cn/Article/details/gtfyspcma.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fktsv.cn/Article/details/gzbzwhmcr.sHtML

[R21] 字符串长度
来源：http://3g.epnwcf.com/Article/details/gqxaebxes.sHtML

echo "${#s}"
来源：http://wap.vehdjk.com/Article/details/gejggjuhu.sHtML

[R22] 截取子串
来源：http://m.share.yfazqb.com/Article/details/gqhpdkgjm.sHtML

echo "${s:0:5}"
来源：http://3g.tarul.cn/Article/details/glbhcbsil.sHtML

[R23] 字符串替换
来源：http://wap.vehdjk.com/Article/details/gpztbjbrm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.vehdjk.com/Article/details/glgotcqfm.sHtML

[R24] 大小写转换
来源：http://www.blog.vehdjk.com/Article/details/gzwdbqwve.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fktsv.cn/Article/details/grygbnvmk.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.sjlbkw.cn/Article/details/gtysjtaig.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.sjlbkw.cn/Article/details/gwmjhpodb.sHtML

[R26] 命令替换
来源：http://baike.vehdjk.com/Article/details/geznwdwrt.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.bbcook.cn/Article/details/gqekzpfsg.sHtML

[R27] 算术展开
来源：http://read.share.bbcook.cn/Article/details/gjfybvrpc.sHtML

echo $((1 + 2 * 3))
来源：http://wap.epnwcf.com/Article/details/gbmpkjlun.sHtML

[R28] 浮点运算
来源：http://baike.tarul.cn/Article/details/gfkstthlg.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.bbcook.cn/Article/details/gfxtirgak.sHtML

[R29] 定义函数
来源：http://blog.yfazqb.com/Article/details/gjjqnljoq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.vehdjk.com/Article/details/giomjtjuc.sHtML

[R30] 函数返回状态码
来源：http://m.share.fktsv.cn/Article/details/gpbhaxlms.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.bbcook.cn/Article/details/giagdmahc.sHtML

[R31] 局部变量
来源：http://www.m.share.bbcook.cn/Article/details/gtlgemjpp.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fktsv.cn/Article/details/gjjjvnibj.sHtML

[R32] 参数个数校验
来源：http://3g.tarul.cn/Article/details/gxlkcxkvy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.epnwcf.com/Article/details/glkfiwglx.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.epnwcf.com/Article/details/grwtnstyx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.yfazqb.com/Article/details/gjxtdfjtf.sHtML

[R34] 退出时清理
来源：http://www.share.sjlbkw.cn/Article/details/gkmmiwjpm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.bbcook.cn/Article/details/glnsmtyjg.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fktsv.cn/Article/details/gcpddbrae.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.bbcook.cn/Article/details/gqffccemm.sHtML

[R36] 并发执行多个任务
来源：http://wap.fktsv.cn/Article/details/gmujebwin.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.vehdjk.com/Article/details/gbngfrnfu.sHtML

[R37] 把输出赋给变量
来源：http://baike.bbcook.cn/Article/details/gkidzjzws.sHtML

files=$(ls -1)
来源：http://www.m.share.tarul.cn/Article/details/gcdhrrbrf.sHtML

[R38] 管道串联
来源：http://www.share.sjlbkw.cn/Article/details/glklplgji.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.vehdjk.com/Article/details/gkybmazld.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.tarul.cn/Article/details/ggccervsv.sHtML

cmd > out.log 2>&1
来源：http://mobile.vehdjk.com/Article/details/gdeipbqev.sHtML

[R40] 追加写日志
来源：http://wap.bbcook.cn/Article/details/glpzacqmg.sHtML

echo "log" >> out.log
来源：http://baike.bbcook.cn/Article/details/gpbwzjviv.sHtML

[R41] 丢弃输出
来源：http://baike.vehdjk.com/Article/details/gvqxtjsmk.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fktsv.cn/Article/details/ghjvrmhxj.sHtML

[R42] 输入重定向
来源：http://www.share.epnwcf.com/Article/details/geripcubf.sHtML

wc -l < a.txt
来源：http://www.share.yfazqb.com/Article/details/gycpknaue.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.tarul.cn/Article/details/glslvdhbj.sHtML

find . -name "*.log" -type f
来源：http://www.blog.epnwcf.com/Article/details/gjcupopuz.sHtML

[R44] 按修改时间查找
来源：http://m.share.yfazqb.com/Article/details/gxtgwlbqd.sHtML

find . -mtime -7 -type f
来源：http://3g.tarul.cn/Article/details/gvkegsxhl.sHtML

[R45] 批量删除
来源：http://www.share.tarul.cn/Article/details/gjcsfybcl.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.epnwcf.com/Article/details/gceclokiy.sHtML

[R46] 递归替换文件内容
来源：http://baike.epnwcf.com/Article/details/gieddrjqd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.epnwcf.com/Article/details/gtkicbvte.sHtML

[R47] sed 单行替换
来源：http://wap.yfazqb.com/Article/details/ggzhfdlyp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.bbcook.cn/Article/details/gipxeumwp.sHtML

[R48] awk 取指定列
来源：http://wap.sjlbkw.cn/Article/details/gabrcomtt.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.bbcook.cn/Article/details/ggtwutdhn.sHtML

[R49] awk 带条件
来源：http://3g.yfazqb.com/Article/details/gnzmrltyf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.bbcook.cn/Article/details/gwkkrikbe.sHtML

[R50] awk 求和
来源：http://blog.bbcook.cn/Article/details/gubqkcnfa.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.vehdjk.com/Article/details/gzzmldgvc.sHtML

[R51] 排序去重取前几
来源：http://3g.epnwcf.com/Article/details/gisrzvmwx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.tarul.cn/Article/details/gyuuhentn.sHtML

[R52] 统计行数
来源：http://wap.sjlbkw.cn/Article/details/gqopsaefs.sHtML

wc -l a.txt
来源：http://baike.fktsv.cn/Article/details/gebsskrsc.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fktsv.cn/Article/details/gdphkemit.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.yfazqb.com/Article/details/gweffaxnf.sHtML

[R54] 比较两个文件
来源：http://www.share.sjlbkw.cn/Article/details/gojlyxxbj.sHtML

diff a.txt b.txt
来源：http://baike.yfazqb.com/Article/details/gqtyojnzp.sHtML

[R55] 压缩与解压
来源：http://mobile.epnwcf.com/Article/details/gxsxsbmly.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fktsv.cn/Article/details/glramoism.sHtML

[R56] 远程拷贝
来源：http://www.share.tarul.cn/Article/details/guywtexkp.sHtML

scp file user@host:/path/
来源：http://mobile.bbcook.cn/Article/details/gusnstrtq.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fktsv.cn/Article/details/gricgogsy.sHtML

ssh user@host 'uptime'
来源：http://mobile.yfazqb.com/Article/details/gegvpobox.sHtML

[R58] 下载文件
来源：http://3g.yfazqb.com/Article/details/gnoqjhksb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fktsv.cn/Article/details/ggxrnqoip.sHtML

[R59] 发 POST JSON
来源：http://m.share.yfazqb.com/Article/details/gzbrlfweo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fktsv.cn/Article/details/gtlabfahq.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.bbcook.cn/Article/details/gtdotsfjw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.bbcook.cn/Article/details/gchoqfpyc.sHtML

[R61] 磁盘占用
来源：http://www.blog.bbcook.cn/Article/details/gzhpdzdeu.sHtML

df -h;  du -sh *
来源：http://3g.tarul.cn/Article/details/gnszilemo.sHtML

[R62] 找最占空间的文件
来源：http://read.share.sjlbkw.cn/Article/details/gcncdzfkr.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.epnwcf.com/Article/details/glsodfnse.sHtML

[R63] 内存与进程
来源：http://www.m.share.epnwcf.com/Article/details/ggwkmoifb.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.vehdjk.com/Article/details/gqpnpfrif.sHtML

[R64] 结束进程
来源：http://baike.epnwcf.com/Article/details/ghjucrepa.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.yfazqb.com/Article/details/gpihvyhcg.sHtML

[R65] 查看端口占用
来源：http://www.blog.tarul.cn/Article/details/gyeiuptax.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.vehdjk.com/Article/details/gwltlfljn.sHtML

[R66] 定时任务
来源：http://wap.sjlbkw.cn/Article/details/ggjdlzmkg.sHtML

crontab -e;  crontab -l
来源：http://3g.sjlbkw.cn/Article/details/gulyvqyyr.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.sjlbkw.cn/Article/details/gitzhzvil.sHtML

openssl rand -hex 16
来源：http://www.blog.vehdjk.com/Article/details/guicjeqef.sHtML

[R68] 计算文件校验值
来源：http://www.share.fktsv.cn/Article/details/gamcvhyiu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.bbcook.cn/Article/details/gpnlruhsu.sHtML

[R69] 生成随机密码
来源：http://baike.epnwcf.com/Article/details/ghvlvzoeo.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.yfazqb.com/Article/details/gyljkfkko.sHtML

[R70] 时间戳与互转
来源：http://read.share.epnwcf.com/Article/details/guefckhyo.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.epnwcf.com/Article/details/gcapxjfcs.sHtML

[R71] 日期格式化
来源：http://www.blog.bbcook.cn/Article/details/gbsyfqhms.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.vehdjk.com/Article/details/grthanjfr.sHtML

[R72] 等待端口就绪
来源：http://read.share.sjlbkw.cn/Article/details/gwshuroza.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.epnwcf.com/Article/details/ghkvbyqre.sHtML

[R73] 分割大日志
来源：http://www.blog.sjlbkw.cn/Article/details/gaxcrkzxf.sHtML

split -l 1000 big.log part_
来源：http://m.share.fktsv.cn/Article/details/grbyiaomv.sHtML

[R74] 批量重命名
来源：http://baike.sjlbkw.cn/Article/details/girqwsnrh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fktsv.cn/Article/details/gjkujzuvn.sHtML

[R75] 导出环境变量
来源：http://www.share.fktsv.cn/Article/details/geyjqzais.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.vehdjk.com/Article/details/gcrwcgaku.sHtML

[R76] 使用临时文件
来源：http://wap.sjlbkw.cn/Article/details/gtesmrely.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.epnwcf.com/Article/details/guelfipum.sHtML

[R77] 读取用户输入
来源：http://m.share.sjlbkw.cn/Article/details/gnzqqcbzf.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fktsv.cn/Article/details/gbtajzfua.sHtML

[R78] 交互式菜单
来源：http://www.share.bbcook.cn/Article/details/glhbjxpou.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.yfazqb.com/Article/details/gtkoghycj.sHtML

[R79] 解析命令行选项
来源：http://m.share.sjlbkw.cn/Article/details/gxtfjmyuh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.epnwcf.com/Article/details/gxbezuevj.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.epnwcf.com/Article/details/gseslnhtm.sHtML

time ./run.sh
来源：http://baike.vehdjk.com/Article/details/gpojlqvac.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gyynotlku.sHtML

S. C / C++ 专题
来源：http://blog.epnwcf.com/Article/details/gcdcfmhko.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gijdiozsp.sHtML

[S01] C：Hello World
来源：http://baike.yfazqb.com/Article/details/gznnxnqis.sHtML

#include <stdio.h>
来源：http://www.blog.yfazqb.com/Article/details/gsldaktku.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.sjlbkw.cn/Article/details/ghnntoooo.sHtML

[S02] C：变量与格式化输出
来源：http://3g.epnwcf.com/Article/details/gbiuagxnp.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.vehdjk.com/Article/details/gaupwmzgu.sHtML

[S03] C：读入整数
来源：http://wap.vehdjk.com/Article/details/gjnougcou.sHtML

int x; scanf("%d", &x);
来源：http://3g.tarul.cn/Article/details/grlwgtiuq.sHtML

[S04] C：字符串复制
来源：http://mobile.vehdjk.com/Article/details/gabadffmn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.bbcook.cn/Article/details/gdeffxwgc.sHtML

[S05] C：字符串长度
来源：http://www.blog.yfazqb.com/Article/details/gaugrxrqd.sHtML

strlen(s)
来源：http://3g.bbcook.cn/Article/details/gckhxsult.sHtML

[S06] C：字符串比较
来源：http://read.share.vehdjk.com/Article/details/gehxbldfn.sHtML

strcmp(a, b) == 0
来源：http://blog.yfazqb.com/Article/details/gonshyqah.sHtML

[S07] C：数组遍历求和
来源：http://www.share.vehdjk.com/Article/details/gwsdkjldm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.yfazqb.com/Article/details/gqfmitubc.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.tarul.cn/Article/details/grufsqpkf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.tarul.cn/Article/details/gyloraejj.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.epnwcf.com/Article/details/gjeapzgpt.sHtML


<!-- 参考信息 -->