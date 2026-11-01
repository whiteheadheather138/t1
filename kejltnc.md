代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://blog.vehdjk.com/Article/details/gbuuuizmx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.epnwcf.com/Article/details/givlevnek.sHtML

[Q47] 与平均值比较
来源：http://read.share.bbcook.cn/Article/details/gbccremjg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.vehdjk.com/Article/details/gmotomskh.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.vehdjk.com/Article/details/gkyrrnhxl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.bbcook.cn/Article/details/gdzyjzvxv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.sjlbkw.cn/Article/details/gorveetgy.sHtML

[Q49] 更新单行
来源：http://www.blog.bbcook.cn/Article/details/gbslzstvz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.tarul.cn/Article/details/gsagxcgcw.sHtML

[Q50] 批量更新
来源：http://m.share.tarul.cn/Article/details/gwcmhqpxe.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.yfazqb.com/Article/details/goczfsjwd.sHtML

[Q51] 用子查询更新
来源：http://wap.yfazqb.com/Article/details/gnvuwkuba.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.tarul.cn/Article/details/goeepxhgu.sHtML

[Q52] 删除指定行
来源：http://3g.vehdjk.com/Article/details/gklgsiaaw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fktsv.cn/Article/details/ggmlfroax.sHtML

[Q53] 按条件删除
来源：http://www.blog.yfazqb.com/Article/details/goiktugwk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.yfazqb.com/Article/details/goclekrpt.sHtML

[Q54] 清空表
来源：http://baike.tarul.cn/Article/details/gwipqmbcf.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.tarul.cn/Article/details/ghqkjiwui.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fktsv.cn/Article/details/gfiajxnve.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fktsv.cn/Article/details/gxffoqxxo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.yfazqb.com/Article/details/gjhxlkjix.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.bbcook.cn/Article/details/gbxrzplvv.sHtML

[Q57] 行号
来源：http://mobile.vehdjk.com/Article/details/gztimszjy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/grjjjkcxb.sHtML

[Q58] 累计求和
来源：http://blog.fktsv.cn/Article/details/gilbvltue.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/gqifbskqj.sHtML

[Q59] 分组内累计
来源：http://blog.vehdjk.com/Article/details/gyrltkgbn.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.epnwcf.com/Article/details/ghrusdzxw.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fktsv.cn/Article/details/gldxrfazh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.tarul.cn/Article/details/grxeqwfqj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.vehdjk.com/Article/details/gmaimxlqc.sHtML

[Q61] 移动平均
来源：http://mobile.sjlbkw.cn/Article/details/gqaxyhlok.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.vehdjk.com/Article/details/gpgawgrhn.sHtML

[Q62] 分组占比
来源：http://blog.sjlbkw.cn/Article/details/gpvqeinei.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.sjlbkw.cn/Article/details/guhaqjmoc.sHtML

[Q63] 开启事务
来源：http://wap.sjlbkw.cn/Article/details/gkwzmmhsl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.bbcook.cn/Article/details/gtxegmqzv.sHtML

[Q64] 提交事务
来源：http://baike.epnwcf.com/Article/details/gfzgtropk.sHtML

COMMIT;
来源：http://m.share.vehdjk.com/Article/details/gkfotsgxq.sHtML

[Q65] 回滚事务
来源：http://read.share.vehdjk.com/Article/details/gqbzswnwa.sHtML

ROLLBACK;
来源：http://www.blog.yfazqb.com/Article/details/gjtlidgdr.sHtML

[Q66] 行锁查询
来源：http://blog.sjlbkw.cn/Article/details/gvmcfdjzo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.bbcook.cn/Article/details/gsgtklquj.sHtML

[Q67] 设置隔离级别
来源：http://www.share.sjlbkw.cn/Article/details/ggfbhhkqo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fktsv.cn/Article/details/gatvchupj.sHtML

[Q68] 保存点
来源：http://www.m.share.bbcook.cn/Article/details/grcvsgfsr.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.yfazqb.com/Article/details/gcbwvkxqo.sHtML

ROLLBACK TO sp1;
来源：http://wap.bbcook.cn/Article/details/gvdbeytwv.sHtML

[Q69] 查看执行计划
来源：http://www.share.bbcook.cn/Article/details/gmnrfeojd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.epnwcf.com/Article/details/gkpokvxuq.sHtML

[Q70] 更新统计信息
来源：http://read.share.yfazqb.com/Article/details/gnnyzljex.sHtML

ANALYZE TABLE users;
来源：http://baike.vehdjk.com/Article/details/gkwokqegd.sHtML

[Q71] 查看建表语句
来源：http://wap.yfazqb.com/Article/details/gkgrcswbq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.tarul.cn/Article/details/gngcbjovm.sHtML

[Q72] 查看索引
来源：http://m.share.epnwcf.com/Article/details/gvxajfajs.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fktsv.cn/Article/details/gbskksixw.sHtML

[Q73] 查看表状态
来源：http://mobile.fktsv.cn/Article/details/gpxcfldtr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.tarul.cn/Article/details/ggruojfgq.sHtML

[Q74] 强制使用索引
来源：http://m.share.bbcook.cn/Article/details/gvhcjuvro.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.sjlbkw.cn/Article/details/gcbelbnal.sHtML

[Q75] 日期格式化
来源：http://www.m.share.sjlbkw.cn/Article/details/gwnrgvrie.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.yfazqb.com/Article/details/gsqmjvpnj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.epnwcf.com/Article/details/gjuajanzz.sHtML

[Q76] 按天统计
来源：http://blog.yfazqb.com/Article/details/gmbgihypk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fktsv.cn/Article/details/gfynvajqm.sHtML

[Q77] 时间加减
来源：http://mobile.bbcook.cn/Article/details/gweosvwcd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.bbcook.cn/Article/details/gupugoohe.sHtML

[Q78] 当前时间
来源：http://www.m.share.yfazqb.com/Article/details/grbnbsdgq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fktsv.cn/Article/details/gesgqgbwu.sHtML

[Q79] 字符串拼接
来源：http://m.share.vehdjk.com/Article/details/gjowjsxjc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.tarul.cn/Article/details/gwgbuxfov.sHtML

[Q80] 字符串截取
来源：http://blog.sjlbkw.cn/Article/details/gdeikaxxb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gccocktuj.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fktsv.cn/Article/details/gsxiroxjf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gkqmcfkhc.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.sjlbkw.cn/Article/details/gtjkjlnrw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/grnpjbqxg.sHtML

[Q83] 大小写转换
来源：http://3g.bbcook.cn/Article/details/gnsqaiwwd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fktsv.cn/Article/details/gooplgyli.sHtML

[Q84] 去除首尾空格
来源：http://mobile.epnwcf.com/Article/details/gycbprdry.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gkupycrid.sHtML

[Q85] 数值取整
来源：http://www.blog.fktsv.cn/Article/details/gpmjlndai.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.epnwcf.com/Article/details/ghecllbul.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fktsv.cn/Article/details/giguviqrn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.sjlbkw.cn/Article/details/gnuidjqjt.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.vehdjk.com/Article/details/gcashlbfd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.bbcook.cn/Article/details/gpzgypfqi.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.vehdjk.com/Article/details/gktogurps.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.vehdjk.com/Article/details/grwgckkxg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.bbcook.cn/Article/details/glqxvkxod.sHtML

[Q89] 判断表是否存在
来源：http://baike.sjlbkw.cn/Article/details/gsuvmjuvw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.sjlbkw.cn/Article/details/gfslsnfzf.sHtML

[Q90] 生成序号列
来源：http://read.share.epnwcf.com/Article/details/gzyyeekje.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.bbcook.cn/Article/details/gcqfkehoa.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gsbhmwukv.sHtML

R. Bash 专题
来源：http://baike.epnwcf.com/Article/details/giyulsfiw.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gyllhqoov.sHtML

[R01] shebang 与严格模式
来源：http://www.share.tarul.cn/Article/details/gatrpguij.sHtML

#!/usr/bin/env bash
来源：http://www.blog.tarul.cn/Article/details/gkkcyqnbw.sHtML

set -euo pipefail
来源：http://wap.yfazqb.com/Article/details/gnkgyoqwo.sHtML

[R02] 变量赋值与使用
来源：http://3g.fktsv.cn/Article/details/guqxpczld.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.sjlbkw.cn/Article/details/gupbmditf.sHtML

[R03] 只读变量
来源：http://3g.sjlbkw.cn/Article/details/gprlyzuld.sHtML

readonly PI=3.14
来源：http://m.share.sjlbkw.cn/Article/details/gdvhdptfm.sHtML

[R04] 位置参数
来源：http://3g.yfazqb.com/Article/details/gbfvtthou.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.vehdjk.com/Article/details/gtemkpgjy.sHtML

[R05] 参数默认值
来源：http://wap.bbcook.cn/Article/details/gskobqvdp.sHtML

name="${1:-default}"
来源：http://m.share.sjlbkw.cn/Article/details/gfxraemlv.sHtML

[R06] 判断命令是否存在
来源：http://mobile.vehdjk.com/Article/details/gdwojrkmg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.bbcook.cn/Article/details/gmmmybsub.sHtML

[R07] if 判断文件
来源：http://www.share.sjlbkw.cn/Article/details/gigolkxnd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.epnwcf.com/Article/details/ghbtpvvog.sHtML

[R08] 数值比较
来源：http://mobile.epnwcf.com/Article/details/ghctparlm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.yfazqb.com/Article/details/gvmuczsug.sHtML

[R09] 字符串比较
来源：http://m.share.tarul.cn/Article/details/gwsyeepea.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.epnwcf.com/Article/details/gdesyzhvs.sHtML

[R10] 正则匹配
来源：http://mobile.epnwcf.com/Article/details/gncgkyadc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.bbcook.cn/Article/details/gyufdmrug.sHtML

[R11] case 多分支
来源：http://read.share.yfazqb.com/Article/details/gvgeqjyja.sHtML

case "$1" in
来源：http://baike.yfazqb.com/Article/details/gnxsmakoo.sHtML

start) echo "启动" ;;
来源：http://3g.yfazqb.com/Article/details/gfopxydjy.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fktsv.cn/Article/details/giirypsmv.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.tarul.cn/Article/details/gyndiiubw.sHtML

esac
来源：http://wap.sjlbkw.cn/Article/details/gsqvvnjpf.sHtML

[R12] for 遍历文件
来源：http://baike.epnwcf.com/Article/details/glcpozoiy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.epnwcf.com/Article/details/gjveqqiey.sHtML

[R13] for 计数循环
来源：http://www.blog.tarul.cn/Article/details/gtulqancv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gmbnlylgl.sHtML

[R14] C 风格 for
来源：http://blog.sjlbkw.cn/Article/details/gickufgli.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.tarul.cn/Article/details/guanzypvx.sHtML

[R15] while 逐行读文件
来源：http://read.share.fktsv.cn/Article/details/goqvluhmd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.bbcook.cn/Article/details/gbkrirdkp.sHtML

[R16] until 等待条件
来源：http://wap.bbcook.cn/Article/details/gkoqpxyut.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.tarul.cn/Article/details/gdxwapdhl.sHtML

[R17] 数组定义与取值
来源：http://www.blog.vehdjk.com/Article/details/gouurzcuf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.vehdjk.com/Article/details/godarbzbp.sHtML

[R18] 遍历数组
来源：http://read.share.yfazqb.com/Article/details/ghvdeqijm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.yfazqb.com/Article/details/gsoaebcjq.sHtML

[R19] 数组长度
来源：http://www.m.share.epnwcf.com/Article/details/giboybqgm.sHtML

echo "${#arr[@]}"
来源：http://3g.sjlbkw.cn/Article/details/gkmtbukct.sHtML

[R20] 关联数组（字典）
来源：http://m.share.yfazqb.com/Article/details/gnbtaebpd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.bbcook.cn/Article/details/gykaqbfmw.sHtML

[R21] 字符串长度
来源：http://mobile.fktsv.cn/Article/details/gwqsdqtwd.sHtML

echo "${#s}"
来源：http://www.m.share.epnwcf.com/Article/details/gziyaakal.sHtML

[R22] 截取子串
来源：http://www.blog.epnwcf.com/Article/details/grrgjjbed.sHtML

echo "${s:0:5}"
来源：http://www.blog.fktsv.cn/Article/details/gwlmrnqeb.sHtML

[R23] 字符串替换
来源：http://m.share.tarul.cn/Article/details/gihnifoew.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.sjlbkw.cn/Article/details/gyfabjooz.sHtML

[R24] 大小写转换
来源：http://www.share.epnwcf.com/Article/details/ggblhbevr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.yfazqb.com/Article/details/goqixtfxs.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.tarul.cn/Article/details/gqzhsirsl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.epnwcf.com/Article/details/gtfsaoxzg.sHtML

[R26] 命令替换
来源：http://www.share.bbcook.cn/Article/details/gqrvoucgo.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fktsv.cn/Article/details/gdfwnxgkx.sHtML

[R27] 算术展开
来源：http://blog.yfazqb.com/Article/details/gyyuzzinf.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.sjlbkw.cn/Article/details/ghcitllob.sHtML

[R28] 浮点运算
来源：http://baike.tarul.cn/Article/details/gliwjcumx.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.bbcook.cn/Article/details/gsybbmigl.sHtML

[R29] 定义函数
来源：http://mobile.sjlbkw.cn/Article/details/gwcfkiide.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.sjlbkw.cn/Article/details/gesclsfma.sHtML

[R30] 函数返回状态码
来源：http://blog.bbcook.cn/Article/details/gnxvpmjno.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.yfazqb.com/Article/details/gmfqesnxy.sHtML

[R31] 局部变量
来源：http://wap.vehdjk.com/Article/details/ghddfviqa.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.tarul.cn/Article/details/glhnruhqw.sHtML

[R32] 参数个数校验
来源：http://www.share.yfazqb.com/Article/details/gzeawypfv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.vehdjk.com/Article/details/ghsqsrvlt.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fktsv.cn/Article/details/galxgbyib.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.sjlbkw.cn/Article/details/gjzrdmqmu.sHtML

[R34] 退出时清理
来源：http://www.m.share.yfazqb.com/Article/details/gfgpjodhx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fktsv.cn/Article/details/gjwnzchvv.sHtML

[R35] 后台执行并等待
来源：http://www.blog.bbcook.cn/Article/details/gfqanjnkr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.bbcook.cn/Article/details/gekczpkcd.sHtML

[R36] 并发执行多个任务
来源：http://www.share.vehdjk.com/Article/details/ggusywdir.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.bbcook.cn/Article/details/ghnslnsaz.sHtML

[R37] 把输出赋给变量
来源：http://baike.yfazqb.com/Article/details/gnturuvab.sHtML

files=$(ls -1)
来源：http://m.share.sjlbkw.cn/Article/details/glxrwothx.sHtML

[R38] 管道串联
来源：http://3g.tarul.cn/Article/details/gcmmhvpjd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.tarul.cn/Article/details/gnjwwgiqs.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.bbcook.cn/Article/details/gxbtxxuuz.sHtML

cmd > out.log 2>&1
来源：http://www.share.fktsv.cn/Article/details/gvynxieli.sHtML

[R40] 追加写日志
来源：http://www.share.fktsv.cn/Article/details/gubppdlzb.sHtML

echo "log" >> out.log
来源：http://www.blog.fktsv.cn/Article/details/gjvvproih.sHtML

[R41] 丢弃输出
来源：http://read.share.vehdjk.com/Article/details/gjfivwbjs.sHtML

cmd >/dev/null 2>&1
来源：http://wap.sjlbkw.cn/Article/details/gbimskwya.sHtML

[R42] 输入重定向
来源：http://www.m.share.sjlbkw.cn/Article/details/gfwfdgjcs.sHtML

wc -l < a.txt
来源：http://wap.tarul.cn/Article/details/gfglfosdy.sHtML

[R43] 按名字查找文件
来源：http://3g.tarul.cn/Article/details/gsdbpwwwt.sHtML

find . -name "*.log" -type f
来源：http://wap.yfazqb.com/Article/details/gpebfmqjn.sHtML

[R44] 按修改时间查找
来源：http://3g.epnwcf.com/Article/details/gsvjyhtca.sHtML

find . -mtime -7 -type f
来源：http://www.blog.vehdjk.com/Article/details/gohdtyota.sHtML

[R45] 批量删除
来源：http://3g.bbcook.cn/Article/details/gzheouoad.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fktsv.cn/Article/details/gsgotkano.sHtML

[R46] 递归替换文件内容
来源：http://blog.tarul.cn/Article/details/giptvbvku.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.epnwcf.com/Article/details/gzcvqqvrp.sHtML

[R47] sed 单行替换
来源：http://wap.fktsv.cn/Article/details/gdbpmobto.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.sjlbkw.cn/Article/details/gyhhahyka.sHtML

[R48] awk 取指定列
来源：http://www.blog.vehdjk.com/Article/details/gxnrjclvp.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fktsv.cn/Article/details/gqarxvmvd.sHtML

[R49] awk 带条件
来源：http://blog.fktsv.cn/Article/details/gjdwwqezm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.sjlbkw.cn/Article/details/gkejtrzwt.sHtML

[R50] awk 求和
来源：http://mobile.bbcook.cn/Article/details/goehxuyhg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.yfazqb.com/Article/details/ggadbdjom.sHtML

[R51] 排序去重取前几
来源：http://mobile.vehdjk.com/Article/details/ggsjjqmkv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.epnwcf.com/Article/details/gshaussfs.sHtML

[R52] 统计行数
来源：http://www.blog.tarul.cn/Article/details/gkzwffzkf.sHtML

wc -l a.txt
来源：http://m.share.bbcook.cn/Article/details/guqafbytn.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.bbcook.cn/Article/details/gqaevtprs.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fktsv.cn/Article/details/ghszcmhtl.sHtML

[R54] 比较两个文件
来源：http://baike.epnwcf.com/Article/details/gwizhwwjw.sHtML

diff a.txt b.txt
来源：http://read.share.vehdjk.com/Article/details/gxwkpzndw.sHtML

[R55] 压缩与解压
来源：http://baike.fktsv.cn/Article/details/gtonuonjx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.tarul.cn/Article/details/glvlbesvd.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fktsv.cn/Article/details/gykeadfhk.sHtML

scp file user@host:/path/
来源：http://read.share.sjlbkw.cn/Article/details/gfmerkibs.sHtML

[R57] 远程执行命令
来源：http://3g.bbcook.cn/Article/details/gzujwzmys.sHtML

ssh user@host 'uptime'
来源：http://baike.bbcook.cn/Article/details/gssfeqbvz.sHtML

[R58] 下载文件
来源：http://m.share.sjlbkw.cn/Article/details/gilsdwxwk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.vehdjk.com/Article/details/gvelwazdn.sHtML

[R59] 发 POST JSON
来源：http://m.share.epnwcf.com/Article/details/gcndlfgnz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.yfazqb.com/Article/details/gcdkdwmvk.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.yfazqb.com/Article/details/gomsprlkt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fktsv.cn/Article/details/gxlgpphyl.sHtML

[R61] 磁盘占用
来源：http://www.blog.tarul.cn/Article/details/gbrmpleym.sHtML

df -h;  du -sh *
来源：http://mobile.fktsv.cn/Article/details/gumgaumys.sHtML

[R62] 找最占空间的文件
来源：http://wap.vehdjk.com/Article/details/gndrdvvau.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.tarul.cn/Article/details/gtvjelksp.sHtML

[R63] 内存与进程
来源：http://www.blog.sjlbkw.cn/Article/details/gqxegdzxk.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fktsv.cn/Article/details/gengdosee.sHtML

[R64] 结束进程
来源：http://www.m.share.yfazqb.com/Article/details/gekcklwsg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.vehdjk.com/Article/details/gulijihfx.sHtML

[R65] 查看端口占用
来源：http://www.blog.fktsv.cn/Article/details/gojfoycee.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.tarul.cn/Article/details/gfdaacisn.sHtML

[R66] 定时任务
来源：http://www.m.share.epnwcf.com/Article/details/gncvflbed.sHtML

crontab -e;  crontab -l
来源：http://www.blog.yfazqb.com/Article/details/gtnnwkwwi.sHtML

[R67] 生成随机十六进制串
来源：http://3g.yfazqb.com/Article/details/gdxicpwln.sHtML

openssl rand -hex 16
来源：http://blog.yfazqb.com/Article/details/ghbbqkqeo.sHtML

[R68] 计算文件校验值
来源：http://www.share.tarul.cn/Article/details/gyvhqdsod.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.epnwcf.com/Article/details/gpuinmlsm.sHtML

[R69] 生成随机密码
来源：http://blog.fktsv.cn/Article/details/ggvvlkkpe.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.sjlbkw.cn/Article/details/guppxqrnn.sHtML

[R70] 时间戳与互转
来源：http://wap.vehdjk.com/Article/details/grhmembig.sHtML

date +%s;  date -d @1700000000
来源：http://wap.epnwcf.com/Article/details/gujabbxhk.sHtML

[R71] 日期格式化
来源：http://baike.yfazqb.com/Article/details/gavpxvvjw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.tarul.cn/Article/details/gmcuyoakn.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.vehdjk.com/Article/details/gsalbaxup.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.tarul.cn/Article/details/gmdhhvwrj.sHtML

[R73] 分割大日志
来源：http://3g.bbcook.cn/Article/details/gqxohrphx.sHtML

split -l 1000 big.log part_
来源：http://mobile.vehdjk.com/Article/details/gpbhtulhv.sHtML

[R74] 批量重命名
来源：http://blog.sjlbkw.cn/Article/details/gqahfmczp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.vehdjk.com/Article/details/gkqhveoqj.sHtML

[R75] 导出环境变量
来源：http://www.share.epnwcf.com/Article/details/gqoyfnoqv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.yfazqb.com/Article/details/gaylfxeux.sHtML

[R76] 使用临时文件
来源：http://www.m.share.epnwcf.com/Article/details/gwnafxljx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.vehdjk.com/Article/details/gfnnebqpr.sHtML

[R77] 读取用户输入
来源：http://baike.vehdjk.com/Article/details/gsdgpxnao.sHtML

read -rp "请输入: " ans
来源：http://baike.vehdjk.com/Article/details/gybgilile.sHtML

[R78] 交互式菜单
来源：http://baike.tarul.cn/Article/details/gxrdktzee.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.tarul.cn/Article/details/gesfdmpmo.sHtML

[R79] 解析命令行选项
来源：http://mobile.epnwcf.com/Article/details/giplqpmbi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.tarul.cn/Article/details/gylmgilzl.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.yfazqb.com/Article/details/gesblyibx.sHtML

time ./run.sh
来源：http://read.share.vehdjk.com/Article/details/garhzolmk.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gdnxhyzwn.sHtML

S. C / C++ 专题
来源：http://3g.bbcook.cn/Article/details/gxsrzjxtk.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gjnusxxtc.sHtML

[S01] C：Hello World
来源：http://m.share.vehdjk.com/Article/details/gvapvhtow.sHtML

#include <stdio.h>
来源：http://wap.tarul.cn/Article/details/ghiftylvv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fktsv.cn/Article/details/gujtsmkgj.sHtML

[S02] C：变量与格式化输出
来源：http://blog.epnwcf.com/Article/details/ggcudzfyl.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.yfazqb.com/Article/details/glnpkyqgh.sHtML

[S03] C：读入整数
来源：http://mobile.bbcook.cn/Article/details/gtcjqaihz.sHtML

int x; scanf("%d", &x);
来源：http://www.share.epnwcf.com/Article/details/gbewyvnot.sHtML

[S04] C：字符串复制
来源：http://blog.sjlbkw.cn/Article/details/gkvplruap.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.tarul.cn/Article/details/gorwqkdlq.sHtML

[S05] C：字符串长度
来源：http://mobile.sjlbkw.cn/Article/details/gjdzptzxw.sHtML

strlen(s)
来源：http://baike.bbcook.cn/Article/details/gblnyifgm.sHtML

[S06] C：字符串比较
来源：http://3g.sjlbkw.cn/Article/details/gvyqhwjct.sHtML

strcmp(a, b) == 0
来源：http://mobile.yfazqb.com/Article/details/gyobcyvxs.sHtML

[S07] C：数组遍历求和
来源：http://wap.sjlbkw.cn/Article/details/gwxprifyq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.epnwcf.com/Article/details/glxyddmiz.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.bbcook.cn/Article/details/gfdcuzixd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.vehdjk.com/Article/details/gwdgurude.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.sjlbkw.cn/Article/details/gfnnlmxhn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.sjlbkw.cn/Article/details/glelrfxfg.sHtML

[S10] C：指针与解引用
来源：http://m.share.vehdjk.com/Article/details/giigsgsxj.sHtML

int *p = &a;  *p = 5;
来源：http://baike.vehdjk.com/Article/details/gyxqxnukl.sHtML

[S11] C：逐行读文件
来源：http://wap.sjlbkw.cn/Article/details/griinvtzt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.vehdjk.com/Article/details/gtfogywgm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.tarul.cn/Article/details/grvcaglja.sHtML

fclose(f);
来源：http://mobile.sjlbkw.cn/Article/details/gmeodpbbj.sHtML

[S12] C：写文件
来源：http://wap.bbcook.cn/Article/details/gorhbqfan.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.bbcook.cn/Article/details/gmnvwiipp.sHtML

[S13] C：宏定义
来源：http://baike.tarul.cn/Article/details/gulskmldg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.vehdjk.com/Article/details/gwyzdalit.sHtML

[S14] C：枚举
来源：http://mobile.vehdjk.com/Article/details/gavcbhypg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.tarul.cn/Article/details/gqgvltcvj.sHtML

[S15] C：类型转换
来源：http://mobile.bbcook.cn/Article/details/gmmpojibj.sHtML

(double) a / b
来源：http://www.blog.yfazqb.com/Article/details/gikiebiys.sHtML

[S16] C：位操作置位
来源：http://baike.vehdjk.com/Article/details/gaivqbqyy.sHtML


<!-- 参考信息 -->