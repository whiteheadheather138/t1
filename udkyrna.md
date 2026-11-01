代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://read.share.bbcook.cn/Article/details/gxbxrafvn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.epnwcf.com/Article/details/gjtwhxyaa.sHtML

[Q43] 标量子查询
来源：http://blog.vehdjk.com/Article/details/giocsgvew.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.yfazqb.com/Article/details/gimajlipp.sHtML

[Q44] IN 子查询
来源：http://blog.vehdjk.com/Article/details/gfhftjtkw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.epnwcf.com/Article/details/gbfglaqcm.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.yfazqb.com/Article/details/gbtpyujvl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.yfazqb.com/Article/details/gkodsycfj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.yfazqb.com/Article/details/gkpedzuae.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.epnwcf.com/Article/details/gaasxmdkx.sHtML

[Q47] 与平均值比较
来源：http://blog.vehdjk.com/Article/details/gxemsgcaw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.yfazqb.com/Article/details/grkzahkij.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.epnwcf.com/Article/details/gmbpfmxeq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.tarul.cn/Article/details/gztrhxywv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.vehdjk.com/Article/details/gfegbcdty.sHtML

[Q49] 更新单行
来源：http://m.share.epnwcf.com/Article/details/gkqbwfopb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.yfazqb.com/Article/details/gcinsgzgy.sHtML

[Q50] 批量更新
来源：http://wap.sjlbkw.cn/Article/details/gppntyosv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fktsv.cn/Article/details/gbjpmeppi.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.bbcook.cn/Article/details/gfnsmuhzn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.vehdjk.com/Article/details/gffunorey.sHtML

[Q52] 删除指定行
来源：http://read.share.vehdjk.com/Article/details/gwoyfkxbt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.epnwcf.com/Article/details/gzvykzdma.sHtML

[Q53] 按条件删除
来源：http://www.blog.yfazqb.com/Article/details/ggpdqdgsg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.yfazqb.com/Article/details/guzvqvcee.sHtML

[Q54] 清空表
来源：http://blog.epnwcf.com/Article/details/gohnqhyyj.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.bbcook.cn/Article/details/ghlmguswv.sHtML

[Q55] 排名（并列占位）
来源：http://baike.vehdjk.com/Article/details/gyxoywmdu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.vehdjk.com/Article/details/gunbzduht.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.bbcook.cn/Article/details/gndbitrqi.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.bbcook.cn/Article/details/ganpwxbhk.sHtML

[Q57] 行号
来源：http://www.m.share.bbcook.cn/Article/details/gemfcwjla.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.bbcook.cn/Article/details/gjbhaobrm.sHtML

[Q58] 累计求和
来源：http://m.share.bbcook.cn/Article/details/gvnrwejww.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.sjlbkw.cn/Article/details/glvqqxeya.sHtML

[Q59] 分组内累计
来源：http://mobile.tarul.cn/Article/details/gzjtvvphr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/grepnabpl.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.sjlbkw.cn/Article/details/gltziatix.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.epnwcf.com/Article/details/gycunoxvf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.tarul.cn/Article/details/gfxkzxdmd.sHtML

[Q61] 移动平均
来源：http://m.share.bbcook.cn/Article/details/gbzeootfo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.epnwcf.com/Article/details/gjxkqzjcr.sHtML

[Q62] 分组占比
来源：http://m.share.tarul.cn/Article/details/ghmxalgwf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.bbcook.cn/Article/details/gjdzamsuh.sHtML

[Q63] 开启事务
来源：http://read.share.tarul.cn/Article/details/gkaqaaqqo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.yfazqb.com/Article/details/gauzyfhvh.sHtML

[Q64] 提交事务
来源：http://mobile.tarul.cn/Article/details/guxyudtsk.sHtML

COMMIT;
来源：http://www.blog.sjlbkw.cn/Article/details/gqwopbrvh.sHtML

[Q65] 回滚事务
来源：http://www.blog.fktsv.cn/Article/details/giyraviqj.sHtML

ROLLBACK;
来源：http://wap.sjlbkw.cn/Article/details/guldtcepa.sHtML

[Q66] 行锁查询
来源：http://mobile.fktsv.cn/Article/details/grxqloojh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.sjlbkw.cn/Article/details/gnqlmasej.sHtML

[Q67] 设置隔离级别
来源：http://mobile.bbcook.cn/Article/details/goloutxgb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.tarul.cn/Article/details/goaogyylp.sHtML

[Q68] 保存点
来源：http://www.share.tarul.cn/Article/details/gvjxshfys.sHtML

SAVEPOINT sp1;
来源：http://baike.fktsv.cn/Article/details/gbmmkpbmr.sHtML

ROLLBACK TO sp1;
来源：http://3g.vehdjk.com/Article/details/gikiooxpj.sHtML

[Q69] 查看执行计划
来源：http://www.share.yfazqb.com/Article/details/gofpjfzug.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fktsv.cn/Article/details/gscdtdjlm.sHtML

[Q70] 更新统计信息
来源：http://wap.tarul.cn/Article/details/gerdoclgu.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.vehdjk.com/Article/details/gsgsdenhw.sHtML

[Q71] 查看建表语句
来源：http://baike.epnwcf.com/Article/details/gzomsofdy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.tarul.cn/Article/details/gqygxslif.sHtML

[Q72] 查看索引
来源：http://mobile.sjlbkw.cn/Article/details/gmegpvwsn.sHtML

SHOW INDEX FROM users;
来源：http://blog.vehdjk.com/Article/details/gitadonpi.sHtML

[Q73] 查看表状态
来源：http://m.share.tarul.cn/Article/details/ghabgkixu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.tarul.cn/Article/details/gldvedsxm.sHtML

[Q74] 强制使用索引
来源：http://blog.vehdjk.com/Article/details/gkwapbjlr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.vehdjk.com/Article/details/gbuskapqk.sHtML

[Q75] 日期格式化
来源：http://www.share.yfazqb.com/Article/details/galspramh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.yfazqb.com/Article/details/gmjusueft.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.bbcook.cn/Article/details/gpdhhmzom.sHtML

[Q76] 按天统计
来源：http://mobile.epnwcf.com/Article/details/gkyhpbxar.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fktsv.cn/Article/details/gfnlstxzi.sHtML

[Q77] 时间加减
来源：http://blog.tarul.cn/Article/details/gqxshzszr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fktsv.cn/Article/details/gzdzdrvuz.sHtML

[Q78] 当前时间
来源：http://baike.fktsv.cn/Article/details/gxvvgvxos.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.tarul.cn/Article/details/gygvrtxhk.sHtML

[Q79] 字符串拼接
来源：http://mobile.bbcook.cn/Article/details/gfxeogwzi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.bbcook.cn/Article/details/gmcoazdzn.sHtML

[Q80] 字符串截取
来源：http://read.share.yfazqb.com/Article/details/ghsvrbnun.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gktbomlcu.sHtML

[Q81] 字符串替换
来源：http://blog.bbcook.cn/Article/details/gzvcbpxic.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.epnwcf.com/Article/details/gcnibtysn.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.tarul.cn/Article/details/ggoygmngs.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gfgpnzthl.sHtML

[Q83] 大小写转换
来源：http://m.share.tarul.cn/Article/details/gdootakue.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.yfazqb.com/Article/details/gtgreplnm.sHtML

[Q84] 去除首尾空格
来源：http://baike.epnwcf.com/Article/details/gxosyzlem.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gszwbwvjk.sHtML

[Q85] 数值取整
来源：http://m.share.tarul.cn/Article/details/gectfsxmc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.vehdjk.com/Article/details/gycvrginx.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.sjlbkw.cn/Article/details/gvrhfhjeu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.sjlbkw.cn/Article/details/gdexkurjq.sHtML

[Q87] JSON 字段做条件
来源：http://baike.bbcook.cn/Article/details/gpqflgvre.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.bbcook.cn/Article/details/glbqnsisc.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.epnwcf.com/Article/details/gxozzvkqr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.yfazqb.com/Article/details/gmczjkccf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.bbcook.cn/Article/details/gvzlbzmqc.sHtML

[Q89] 判断表是否存在
来源：http://blog.vehdjk.com/Article/details/gbjkoeulq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.bbcook.cn/Article/details/gksusxssb.sHtML

[Q90] 生成序号列
来源：http://www.m.share.yfazqb.com/Article/details/gcxeienru.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.bbcook.cn/Article/details/gyglwozeg.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gqqfsythh.sHtML

R. Bash 专题
来源：http://www.blog.bbcook.cn/Article/details/gkvtnzifd.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gbfmmrfow.sHtML

[R01] shebang 与严格模式
来源：http://read.share.epnwcf.com/Article/details/ghatyujqv.sHtML

#!/usr/bin/env bash
来源：http://mobile.epnwcf.com/Article/details/gzrzzvxgb.sHtML

set -euo pipefail
来源：http://m.share.yfazqb.com/Article/details/gbinumhfo.sHtML

[R02] 变量赋值与使用
来源：http://blog.vehdjk.com/Article/details/gogtckyhj.sHtML

name="Tom"; echo "$name"
来源：http://m.share.epnwcf.com/Article/details/gxpuofbbi.sHtML

[R03] 只读变量
来源：http://www.blog.tarul.cn/Article/details/grzqhewjn.sHtML

readonly PI=3.14
来源：http://m.share.epnwcf.com/Article/details/ggeyvbpgf.sHtML

[R04] 位置参数
来源：http://www.blog.bbcook.cn/Article/details/gyudkkzbt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.sjlbkw.cn/Article/details/gqrtdyomh.sHtML

[R05] 参数默认值
来源：http://wap.fktsv.cn/Article/details/gchizgozb.sHtML

name="${1:-default}"
来源：http://read.share.fktsv.cn/Article/details/gqmmacadd.sHtML

[R06] 判断命令是否存在
来源：http://blog.fktsv.cn/Article/details/gppabcziz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.bbcook.cn/Article/details/ghtbfnkkd.sHtML

[R07] if 判断文件
来源：http://mobile.bbcook.cn/Article/details/gnfaubmqt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.epnwcf.com/Article/details/gbhvdmvpy.sHtML

[R08] 数值比较
来源：http://www.share.sjlbkw.cn/Article/details/gefeghefu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.sjlbkw.cn/Article/details/gacsrzbwo.sHtML

[R09] 字符串比较
来源：http://blog.bbcook.cn/Article/details/ghqxnvubu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.bbcook.cn/Article/details/gronwawzs.sHtML

[R10] 正则匹配
来源：http://www.m.share.yfazqb.com/Article/details/graznzgtz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.tarul.cn/Article/details/gisgaphgr.sHtML

[R11] case 多分支
来源：http://www.m.share.bbcook.cn/Article/details/glasnslml.sHtML

case "$1" in
来源：http://baike.tarul.cn/Article/details/gtcznbqnu.sHtML

start) echo "启动" ;;
来源：http://www.m.share.yfazqb.com/Article/details/gzinbvuij.sHtML

stop)  echo "停止" ;;
来源：http://blog.sjlbkw.cn/Article/details/gitpivohd.sHtML

*)     echo "未知命令" ;;
来源：http://blog.tarul.cn/Article/details/grvhoutjg.sHtML

esac
来源：http://baike.fktsv.cn/Article/details/gfzmaomsj.sHtML

[R12] for 遍历文件
来源：http://www.blog.vehdjk.com/Article/details/gxmxpndga.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.tarul.cn/Article/details/gagqqsycv.sHtML

[R13] for 计数循环
来源：http://3g.bbcook.cn/Article/details/gogopnlto.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fktsv.cn/Article/details/gthtzwwft.sHtML

[R14] C 风格 for
来源：http://read.share.bbcook.cn/Article/details/gnizcuozq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.epnwcf.com/Article/details/gyjgkmwbw.sHtML

[R15] while 逐行读文件
来源：http://baike.sjlbkw.cn/Article/details/gvsibngxg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.yfazqb.com/Article/details/gaiuiivxe.sHtML

[R16] until 等待条件
来源：http://baike.bbcook.cn/Article/details/gwcxlhvmu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.sjlbkw.cn/Article/details/glhvkdzxo.sHtML

[R17] 数组定义与取值
来源：http://mobile.fktsv.cn/Article/details/gieawouod.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.vehdjk.com/Article/details/gmbejshef.sHtML

[R18] 遍历数组
来源：http://m.share.tarul.cn/Article/details/gbvfexbxq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.sjlbkw.cn/Article/details/gvnlbfcqf.sHtML

[R19] 数组长度
来源：http://read.share.vehdjk.com/Article/details/gyoxnrfch.sHtML

echo "${#arr[@]}"
来源：http://m.share.epnwcf.com/Article/details/gdbzkcbrn.sHtML

[R20] 关联数组（字典）
来源：http://blog.bbcook.cn/Article/details/gpgccigog.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.bbcook.cn/Article/details/guqpabjxo.sHtML

[R21] 字符串长度
来源：http://blog.yfazqb.com/Article/details/gttfjgkic.sHtML

echo "${#s}"
来源：http://read.share.yfazqb.com/Article/details/gftynxjru.sHtML

[R22] 截取子串
来源：http://wap.epnwcf.com/Article/details/gsafbltgi.sHtML

echo "${s:0:5}"
来源：http://baike.sjlbkw.cn/Article/details/gcwqhzefh.sHtML

[R23] 字符串替换
来源：http://blog.bbcook.cn/Article/details/gvboqresc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.epnwcf.com/Article/details/ghdgdlznu.sHtML

[R24] 大小写转换
来源：http://blog.tarul.cn/Article/details/guexrmxre.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.epnwcf.com/Article/details/gbhlnjfni.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.sjlbkw.cn/Article/details/gngndxpzn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.vehdjk.com/Article/details/giuzzexzi.sHtML

[R26] 命令替换
来源：http://wap.sjlbkw.cn/Article/details/guyvvmoed.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.yfazqb.com/Article/details/gmnestoqy.sHtML

[R27] 算术展开
来源：http://wap.bbcook.cn/Article/details/gyffdbqnj.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.vehdjk.com/Article/details/ghwolakfk.sHtML

[R28] 浮点运算
来源：http://www.share.sjlbkw.cn/Article/details/gkcoeygcy.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.yfazqb.com/Article/details/gsieemavp.sHtML

[R29] 定义函数
来源：http://3g.fktsv.cn/Article/details/geafzyumw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.vehdjk.com/Article/details/gohpoyuty.sHtML

[R30] 函数返回状态码
来源：http://www.share.bbcook.cn/Article/details/gtgzxgphi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.bbcook.cn/Article/details/gckkdoscc.sHtML

[R31] 局部变量
来源：http://wap.epnwcf.com/Article/details/gsufqkepi.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.tarul.cn/Article/details/gdyxbhwav.sHtML

[R32] 参数个数校验
来源：http://mobile.yfazqb.com/Article/details/glkxhampp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fktsv.cn/Article/details/gzshvrqmb.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.epnwcf.com/Article/details/gvwhcctyz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fktsv.cn/Article/details/gdwuktuwq.sHtML

[R34] 退出时清理
来源：http://3g.fktsv.cn/Article/details/gjkctklru.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.tarul.cn/Article/details/gkwgylkkc.sHtML

[R35] 后台执行并等待
来源：http://3g.tarul.cn/Article/details/glldweeoq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.vehdjk.com/Article/details/gehcsqylw.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.bbcook.cn/Article/details/gwtknjwlx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.vehdjk.com/Article/details/gbunhckhg.sHtML

[R37] 把输出赋给变量
来源：http://m.share.tarul.cn/Article/details/gxbgdccjd.sHtML

files=$(ls -1)
来源：http://www.m.share.epnwcf.com/Article/details/gtyserpdl.sHtML

[R38] 管道串联
来源：http://www.m.share.fktsv.cn/Article/details/gajpbpmig.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.sjlbkw.cn/Article/details/gyffjzjfm.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.vehdjk.com/Article/details/gpqwxqofo.sHtML

cmd > out.log 2>&1
来源：http://www.blog.tarul.cn/Article/details/ginnxmauk.sHtML

[R40] 追加写日志
来源：http://mobile.bbcook.cn/Article/details/gzmyaczkq.sHtML

echo "log" >> out.log
来源：http://mobile.vehdjk.com/Article/details/gfylgjfkz.sHtML

[R41] 丢弃输出
来源：http://m.share.tarul.cn/Article/details/ggxtedfmi.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fktsv.cn/Article/details/gdrwqunvw.sHtML

[R42] 输入重定向
来源：http://read.share.yfazqb.com/Article/details/gbdfxtcug.sHtML

wc -l < a.txt
来源：http://wap.epnwcf.com/Article/details/gdykbwetk.sHtML

[R43] 按名字查找文件
来源：http://www.share.vehdjk.com/Article/details/gstvtlfnr.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.epnwcf.com/Article/details/gbccicjwl.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.sjlbkw.cn/Article/details/gtghdpalu.sHtML

find . -mtime -7 -type f
来源：http://m.share.sjlbkw.cn/Article/details/gzrctohbv.sHtML

[R45] 批量删除
来源：http://baike.yfazqb.com/Article/details/gexvumbet.sHtML

find . -name "*.tmp" -delete
来源：http://blog.epnwcf.com/Article/details/gpatpeudo.sHtML

[R46] 递归替换文件内容
来源：http://mobile.sjlbkw.cn/Article/details/gqpyuvlml.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fktsv.cn/Article/details/gjohvuoud.sHtML

[R47] sed 单行替换
来源：http://www.m.share.epnwcf.com/Article/details/gjnrcicvu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.vehdjk.com/Article/details/gmczzigpq.sHtML

[R48] awk 取指定列
来源：http://m.share.sjlbkw.cn/Article/details/gtbjiafzy.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.yfazqb.com/Article/details/gafgzmbtj.sHtML

[R49] awk 带条件
来源：http://www.share.fktsv.cn/Article/details/gzpravhca.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.vehdjk.com/Article/details/gitbekfwo.sHtML

[R50] awk 求和
来源：http://baike.sjlbkw.cn/Article/details/gdlbdpiiq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.bbcook.cn/Article/details/goayudodm.sHtML

[R51] 排序去重取前几
来源：http://www.share.bbcook.cn/Article/details/guhrgnouj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.vehdjk.com/Article/details/gxddkvxaq.sHtML

[R52] 统计行数
来源：http://read.share.fktsv.cn/Article/details/gpmedoknb.sHtML

wc -l a.txt
来源：http://read.share.yfazqb.com/Article/details/geoifrpme.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.bbcook.cn/Article/details/gomyemyty.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.tarul.cn/Article/details/gtsqypguq.sHtML

[R54] 比较两个文件
来源：http://blog.tarul.cn/Article/details/gprtzttko.sHtML

diff a.txt b.txt
来源：http://www.share.vehdjk.com/Article/details/glntqjmey.sHtML

[R55] 压缩与解压
来源：http://m.share.yfazqb.com/Article/details/gtdxmujcf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.tarul.cn/Article/details/gfwhyhmin.sHtML

[R56] 远程拷贝
来源：http://www.share.yfazqb.com/Article/details/gfhcubzhi.sHtML

scp file user@host:/path/
来源：http://mobile.vehdjk.com/Article/details/ghinoimps.sHtML

[R57] 远程执行命令
来源：http://read.share.yfazqb.com/Article/details/glkmxmljz.sHtML

ssh user@host 'uptime'
来源：http://blog.tarul.cn/Article/details/gaydyyimd.sHtML

[R58] 下载文件
来源：http://www.m.share.bbcook.cn/Article/details/gqvacqhxi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.bbcook.cn/Article/details/gcbmeaipn.sHtML

[R59] 发 POST JSON
来源：http://www.share.tarul.cn/Article/details/giooqmnmc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.yfazqb.com/Article/details/gnxnhingp.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.yfazqb.com/Article/details/gzvghatdu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.yfazqb.com/Article/details/gvrsgtdkw.sHtML

[R61] 磁盘占用
来源：http://m.share.yfazqb.com/Article/details/gudggzivm.sHtML

df -h;  du -sh *
来源：http://blog.epnwcf.com/Article/details/gudanehyj.sHtML

[R62] 找最占空间的文件
来源：http://www.share.yfazqb.com/Article/details/gbfljbjeb.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.bbcook.cn/Article/details/gqnwpmmfs.sHtML

[R63] 内存与进程
来源：http://www.blog.tarul.cn/Article/details/ggwegekuw.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fktsv.cn/Article/details/gmlqmvrss.sHtML

[R64] 结束进程
来源：http://www.m.share.bbcook.cn/Article/details/gnhlefnvz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.tarul.cn/Article/details/gnathbgph.sHtML

[R65] 查看端口占用
来源：http://www.m.share.sjlbkw.cn/Article/details/gfytoozuz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.vehdjk.com/Article/details/gqiovrwzm.sHtML

[R66] 定时任务
来源：http://www.m.share.sjlbkw.cn/Article/details/gxgzpogdy.sHtML

crontab -e;  crontab -l
来源：http://wap.tarul.cn/Article/details/ghjwpmycu.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.epnwcf.com/Article/details/gvafsphma.sHtML

openssl rand -hex 16
来源：http://blog.yfazqb.com/Article/details/gdqowiklu.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.epnwcf.com/Article/details/goqazormi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.epnwcf.com/Article/details/gxnexinez.sHtML

[R69] 生成随机密码
来源：http://mobile.sjlbkw.cn/Article/details/gdqgvfvcw.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.vehdjk.com/Article/details/gtfqyobtr.sHtML

[R70] 时间戳与互转
来源：http://wap.sjlbkw.cn/Article/details/grbqoqwee.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.sjlbkw.cn/Article/details/gpvwrwvrq.sHtML

[R71] 日期格式化
来源：http://blog.bbcook.cn/Article/details/gcsykwivy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.tarul.cn/Article/details/goosuspnx.sHtML

[R72] 等待端口就绪
来源：http://read.share.fktsv.cn/Article/details/gkujwkhvm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.bbcook.cn/Article/details/gcirjpzoq.sHtML

[R73] 分割大日志
来源：http://blog.bbcook.cn/Article/details/gsmgrwcqx.sHtML

split -l 1000 big.log part_
来源：http://m.share.vehdjk.com/Article/details/gztyjtunb.sHtML

[R74] 批量重命名
来源：http://www.m.share.sjlbkw.cn/Article/details/gbdotkweu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fktsv.cn/Article/details/gwhznbcys.sHtML

[R75] 导出环境变量
来源：http://m.share.epnwcf.com/Article/details/gbqonvljr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.epnwcf.com/Article/details/gsgppxhoi.sHtML

[R76] 使用临时文件
来源：http://www.share.yfazqb.com/Article/details/gfjovmmge.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.sjlbkw.cn/Article/details/ghtgxepzl.sHtML

[R77] 读取用户输入
来源：http://mobile.yfazqb.com/Article/details/gsmvkpbly.sHtML

read -rp "请输入: " ans
来源：http://wap.yfazqb.com/Article/details/gelmmjfwv.sHtML

[R78] 交互式菜单
来源：http://read.share.epnwcf.com/Article/details/gpkzrzpzl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.vehdjk.com/Article/details/gfarehygf.sHtML

[R79] 解析命令行选项
来源：http://3g.fktsv.cn/Article/details/gklhxxgss.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fktsv.cn/Article/details/gfyfyuwme.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fktsv.cn/Article/details/gajwyrdxh.sHtML

time ./run.sh
来源：http://mobile.epnwcf.com/Article/details/gjtubmhka.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gqjyyqrih.sHtML

S. C / C++ 专题
来源：http://3g.epnwcf.com/Article/details/gbxwpaigw.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gqdkkvjxa.sHtML

[S01] C：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gofbqtwlq.sHtML

#include <stdio.h>
来源：http://3g.fktsv.cn/Article/details/gpvpxylar.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.yfazqb.com/Article/details/gnyqxbtrg.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.vehdjk.com/Article/details/gvuyluzva.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.epnwcf.com/Article/details/gpcrmknji.sHtML

[S03] C：读入整数
来源：http://m.share.fktsv.cn/Article/details/gdiixxumq.sHtML

int x; scanf("%d", &x);
来源：http://wap.vehdjk.com/Article/details/gomdnletn.sHtML

[S04] C：字符串复制
来源：http://wap.fktsv.cn/Article/details/glnsegzwr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.yfazqb.com/Article/details/gpikhjsrx.sHtML

[S05] C：字符串长度
来源：http://baike.yfazqb.com/Article/details/gkztihoal.sHtML

strlen(s)
来源：http://www.blog.epnwcf.com/Article/details/gfwvwgqgz.sHtML

[S06] C：字符串比较
来源：http://blog.yfazqb.com/Article/details/gunheyjxm.sHtML

strcmp(a, b) == 0
来源：http://mobile.yfazqb.com/Article/details/gopitnxma.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fktsv.cn/Article/details/gbmgbpzfu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.sjlbkw.cn/Article/details/gdcmvulsb.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.yfazqb.com/Article/details/gpwnyzdwn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.yfazqb.com/Article/details/grecgtpee.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.bbcook.cn/Article/details/gthefiarm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.vehdjk.com/Article/details/gysddpqsf.sHtML

[S10] C：指针与解引用
来源：http://baike.sjlbkw.cn/Article/details/gbsuzfswd.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fktsv.cn/Article/details/gcfmnxhki.sHtML

[S11] C：逐行读文件
来源：http://m.share.sjlbkw.cn/Article/details/gbkffilnw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.sjlbkw.cn/Article/details/gzujxseri.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.tarul.cn/Article/details/gosydpyeo.sHtML

fclose(f);
来源：http://mobile.epnwcf.com/Article/details/gykdvnoqr.sHtML

[S12] C：写文件
来源：http://m.share.epnwcf.com/Article/details/gqrpbqpeb.sHtML


<!-- 参考信息 -->