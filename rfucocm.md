代发 wailian999

[Q44] IN 子查询
来源：http://mobile.epnwcf.com/Article/details/gqsphbwiu.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.vehdjk.com/Article/details/grdykxoji.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.bbcook.cn/Article/details/gpujufcwq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.sjlbkw.cn/Article/details/gdmxeufad.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.vehdjk.com/Article/details/gxhuowbjp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.vehdjk.com/Article/details/gxtbgzgqz.sHtML

[Q47] 与平均值比较
来源：http://www.share.fktsv.cn/Article/details/ggkorqvij.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.vehdjk.com/Article/details/gfbmeenlp.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.yfazqb.com/Article/details/gdcmamwmh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.yfazqb.com/Article/details/gckvxzmot.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.sjlbkw.cn/Article/details/giqkgbspv.sHtML

[Q49] 更新单行
来源：http://baike.yfazqb.com/Article/details/gxjzuulib.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fktsv.cn/Article/details/gmmbtotrz.sHtML

[Q50] 批量更新
来源：http://3g.sjlbkw.cn/Article/details/grwdsdusw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.vehdjk.com/Article/details/gtoxswmlb.sHtML

[Q51] 用子查询更新
来源：http://mobile.vehdjk.com/Article/details/gmrrqmkjh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.yfazqb.com/Article/details/gnnczfxlu.sHtML

[Q52] 删除指定行
来源：http://blog.fktsv.cn/Article/details/ggnaabwpx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.tarul.cn/Article/details/gylykekum.sHtML

[Q53] 按条件删除
来源：http://blog.bbcook.cn/Article/details/gvurungmu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.bbcook.cn/Article/details/goitkxril.sHtML

[Q54] 清空表
来源：http://baike.tarul.cn/Article/details/gwgjqoaiu.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fktsv.cn/Article/details/gfrbdppzk.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.bbcook.cn/Article/details/ggclcgfye.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.yfazqb.com/Article/details/gzlltsoar.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.epnwcf.com/Article/details/gyelayftt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.epnwcf.com/Article/details/gmvjevloh.sHtML

[Q57] 行号
来源：http://m.share.vehdjk.com/Article/details/gddkozarq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gftbmmbds.sHtML

[Q58] 累计求和
来源：http://blog.tarul.cn/Article/details/glnhzjnsl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.yfazqb.com/Article/details/glkrkmntm.sHtML

[Q59] 分组内累计
来源：http://blog.bbcook.cn/Article/details/gdsuqrzor.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.yfazqb.com/Article/details/ggpgyzmqt.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.epnwcf.com/Article/details/gswfiojrh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.yfazqb.com/Article/details/ghxpdgiqk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.vehdjk.com/Article/details/gplrrdgdb.sHtML

[Q61] 移动平均
来源：http://blog.tarul.cn/Article/details/ggpekhfwc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fktsv.cn/Article/details/giwlzoxwc.sHtML

[Q62] 分组占比
来源：http://mobile.tarul.cn/Article/details/gjoxxetxl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.sjlbkw.cn/Article/details/gwwlkmdxq.sHtML

[Q63] 开启事务
来源：http://wap.bbcook.cn/Article/details/gqwxnumma.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fktsv.cn/Article/details/gxpkwlfar.sHtML

[Q64] 提交事务
来源：http://wap.bbcook.cn/Article/details/gclwtqbrm.sHtML

COMMIT;
来源：http://m.share.sjlbkw.cn/Article/details/gqclkltmy.sHtML

[Q65] 回滚事务
来源：http://read.share.vehdjk.com/Article/details/gupuimylp.sHtML

ROLLBACK;
来源：http://3g.yfazqb.com/Article/details/gfqmbpyzl.sHtML

[Q66] 行锁查询
来源：http://baike.yfazqb.com/Article/details/gcxxmhwyv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.bbcook.cn/Article/details/gqmstaknk.sHtML

[Q67] 设置隔离级别
来源：http://3g.yfazqb.com/Article/details/gdleadyxy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.yfazqb.com/Article/details/gxwvsbufl.sHtML

[Q68] 保存点
来源：http://read.share.fktsv.cn/Article/details/gnllveehq.sHtML

SAVEPOINT sp1;
来源：http://mobile.tarul.cn/Article/details/gtephayul.sHtML

ROLLBACK TO sp1;
来源：http://wap.sjlbkw.cn/Article/details/gckbagtyw.sHtML

[Q69] 查看执行计划
来源：http://www.share.tarul.cn/Article/details/gmfzikieg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.yfazqb.com/Article/details/gtwzvnvrt.sHtML

[Q70] 更新统计信息
来源：http://www.share.sjlbkw.cn/Article/details/gheuywemm.sHtML

ANALYZE TABLE users;
来源：http://wap.fktsv.cn/Article/details/gxpgitwwv.sHtML

[Q71] 查看建表语句
来源：http://mobile.tarul.cn/Article/details/glflzqtef.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.sjlbkw.cn/Article/details/gzfqykdya.sHtML

[Q72] 查看索引
来源：http://blog.vehdjk.com/Article/details/gxmmasger.sHtML

SHOW INDEX FROM users;
来源：http://www.share.yfazqb.com/Article/details/gmqgvmrsz.sHtML

[Q73] 查看表状态
来源：http://m.share.sjlbkw.cn/Article/details/gwrekorpq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.tarul.cn/Article/details/gydlyqief.sHtML

[Q74] 强制使用索引
来源：http://3g.vehdjk.com/Article/details/gfufzhzxw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.yfazqb.com/Article/details/guvmqsdpx.sHtML

[Q75] 日期格式化
来源：http://read.share.bbcook.cn/Article/details/gqnrolxwa.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.epnwcf.com/Article/details/gffcqyjsd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.vehdjk.com/Article/details/gsjwqlqnl.sHtML

[Q76] 按天统计
来源：http://www.share.sjlbkw.cn/Article/details/gifodzoff.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fktsv.cn/Article/details/gdukbukxo.sHtML

[Q77] 时间加减
来源：http://blog.vehdjk.com/Article/details/gnrbifohs.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.tarul.cn/Article/details/ggwswjaqe.sHtML

[Q78] 当前时间
来源：http://3g.sjlbkw.cn/Article/details/griruztif.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.bbcook.cn/Article/details/gpgdbwkgt.sHtML

[Q79] 字符串拼接
来源：http://3g.yfazqb.com/Article/details/gqrsxvurp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.yfazqb.com/Article/details/gkomlmuix.sHtML

[Q80] 字符串截取
来源：http://mobile.tarul.cn/Article/details/gyymcraro.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.yfazqb.com/Article/details/giirsyfrk.sHtML

[Q81] 字符串替换
来源：http://www.share.epnwcf.com/Article/details/gfswpuofv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.bbcook.cn/Article/details/gfggsvvmi.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.vehdjk.com/Article/details/gnbqrvejm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.bbcook.cn/Article/details/gubzpdkil.sHtML

[Q83] 大小写转换
来源：http://m.share.bbcook.cn/Article/details/gwegekolh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.yfazqb.com/Article/details/gtfocfyph.sHtML

[Q84] 去除首尾空格
来源：http://m.share.epnwcf.com/Article/details/grbwjyzgw.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.epnwcf.com/Article/details/ggmvpdqfg.sHtML

[Q85] 数值取整
来源：http://m.share.vehdjk.com/Article/details/gwqjgtmdz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fktsv.cn/Article/details/ggbordukk.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.yfazqb.com/Article/details/gufssnfya.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.vehdjk.com/Article/details/gvauvqhsn.sHtML

[Q87] JSON 字段做条件
来源：http://wap.tarul.cn/Article/details/gwohrargs.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.yfazqb.com/Article/details/grbehhcyu.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.epnwcf.com/Article/details/gvuzfihhs.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.bbcook.cn/Article/details/grwpommcw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fktsv.cn/Article/details/gnyyuibdo.sHtML

[Q89] 判断表是否存在
来源：http://m.share.sjlbkw.cn/Article/details/gfkfjfjyf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.tarul.cn/Article/details/guqknqhor.sHtML

[Q90] 生成序号列
来源：http://www.m.share.vehdjk.com/Article/details/gdciifdjq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.tarul.cn/Article/details/gamhmemas.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gcivjfedw.sHtML

R. Bash 专题
来源：http://3g.tarul.cn/Article/details/gpagvlmft.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gblfkmfli.sHtML

[R01] shebang 与严格模式
来源：http://3g.tarul.cn/Article/details/gmkqgrcgf.sHtML

#!/usr/bin/env bash
来源：http://blog.fktsv.cn/Article/details/groxwxzsz.sHtML

set -euo pipefail
来源：http://3g.yfazqb.com/Article/details/gpprzgizy.sHtML

[R02] 变量赋值与使用
来源：http://3g.sjlbkw.cn/Article/details/gfstbwcst.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fktsv.cn/Article/details/geuieyxiq.sHtML

[R03] 只读变量
来源：http://wap.tarul.cn/Article/details/glflftasg.sHtML

readonly PI=3.14
来源：http://wap.tarul.cn/Article/details/gspfcrxiv.sHtML

[R04] 位置参数
来源：http://m.share.fktsv.cn/Article/details/grfopjxui.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.vehdjk.com/Article/details/geixtmxxj.sHtML

[R05] 参数默认值
来源：http://blog.epnwcf.com/Article/details/gegcodlgi.sHtML

name="${1:-default}"
来源：http://baike.epnwcf.com/Article/details/gijlfvgca.sHtML

[R06] 判断命令是否存在
来源：http://blog.bbcook.cn/Article/details/gukyqpipm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.bbcook.cn/Article/details/gtwlmaptm.sHtML

[R07] if 判断文件
来源：http://baike.epnwcf.com/Article/details/ggqnapuwn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.epnwcf.com/Article/details/gvyaazfae.sHtML

[R08] 数值比较
来源：http://blog.yfazqb.com/Article/details/gsgotgidb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.vehdjk.com/Article/details/gxhmmodvb.sHtML

[R09] 字符串比较
来源：http://www.share.tarul.cn/Article/details/getapuajf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.vehdjk.com/Article/details/gykkzdbei.sHtML

[R10] 正则匹配
来源：http://blog.bbcook.cn/Article/details/giloomscf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fktsv.cn/Article/details/grsiiythf.sHtML

[R11] case 多分支
来源：http://m.share.epnwcf.com/Article/details/gkmcyewgy.sHtML

case "$1" in
来源：http://baike.fktsv.cn/Article/details/gceihefxr.sHtML

start) echo "启动" ;;
来源：http://www.share.tarul.cn/Article/details/gkbdlmwcm.sHtML

stop)  echo "停止" ;;
来源：http://blog.tarul.cn/Article/details/gpukifumu.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.yfazqb.com/Article/details/gvycmcqhx.sHtML

esac
来源：http://www.blog.bbcook.cn/Article/details/ghuhnnvpt.sHtML

[R12] for 遍历文件
来源：http://www.share.bbcook.cn/Article/details/gigdangay.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.epnwcf.com/Article/details/gsohtvhgu.sHtML

[R13] for 计数循环
来源：http://www.blog.epnwcf.com/Article/details/gipzbomai.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fktsv.cn/Article/details/gsmnlveps.sHtML

[R14] C 风格 for
来源：http://www.m.share.vehdjk.com/Article/details/gkvsxenzd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.tarul.cn/Article/details/gaaslbsbi.sHtML

[R15] while 逐行读文件
来源：http://m.share.sjlbkw.cn/Article/details/ghrulzjyu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.bbcook.cn/Article/details/gltxoimap.sHtML

[R16] until 等待条件
来源：http://www.share.tarul.cn/Article/details/gihkijkcb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.bbcook.cn/Article/details/gkjnhusxw.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fktsv.cn/Article/details/gcdteuqec.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.yfazqb.com/Article/details/gfbymggyy.sHtML

[R18] 遍历数组
来源：http://blog.vehdjk.com/Article/details/gnjrzaywp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.yfazqb.com/Article/details/gyopywthf.sHtML

[R19] 数组长度
来源：http://www.blog.sjlbkw.cn/Article/details/gasqivwmw.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.yfazqb.com/Article/details/gvzfkabef.sHtML

[R20] 关联数组（字典）
来源：http://read.share.epnwcf.com/Article/details/gukgvqtqm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.bbcook.cn/Article/details/gabnaocyn.sHtML

[R21] 字符串长度
来源：http://m.share.sjlbkw.cn/Article/details/gfqowjrpp.sHtML

echo "${#s}"
来源：http://wap.yfazqb.com/Article/details/gmtbrkbaz.sHtML

[R22] 截取子串
来源：http://read.share.sjlbkw.cn/Article/details/gevckuygc.sHtML

echo "${s:0:5}"
来源：http://www.blog.vehdjk.com/Article/details/gssbsjolz.sHtML

[R23] 字符串替换
来源：http://www.m.share.epnwcf.com/Article/details/gztihddjv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.vehdjk.com/Article/details/gaftpikjl.sHtML

[R24] 大小写转换
来源：http://www.share.epnwcf.com/Article/details/gaebpnyny.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.sjlbkw.cn/Article/details/gfwksmvrt.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.vehdjk.com/Article/details/ghvhagpdw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fktsv.cn/Article/details/gskzhyakh.sHtML

[R26] 命令替换
来源：http://wap.epnwcf.com/Article/details/gfuqusgvu.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.bbcook.cn/Article/details/ggmfxjptu.sHtML

[R27] 算术展开
来源：http://blog.sjlbkw.cn/Article/details/gozfpqkmc.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.sjlbkw.cn/Article/details/gpcigyqim.sHtML

[R28] 浮点运算
来源：http://3g.epnwcf.com/Article/details/gzitdnwem.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.vehdjk.com/Article/details/gvbdvdsml.sHtML

[R29] 定义函数
来源：http://blog.yfazqb.com/Article/details/gsnygpjin.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.epnwcf.com/Article/details/gihpyaxvb.sHtML

[R30] 函数返回状态码
来源：http://blog.yfazqb.com/Article/details/glguunigm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fktsv.cn/Article/details/gfknreszx.sHtML

[R31] 局部变量
来源：http://baike.yfazqb.com/Article/details/gqcdwepmj.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.vehdjk.com/Article/details/gshmzrvze.sHtML

[R32] 参数个数校验
来源：http://www.blog.vehdjk.com/Article/details/gzcfdfxek.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.sjlbkw.cn/Article/details/giydyshfj.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fktsv.cn/Article/details/glgbxwovi.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fktsv.cn/Article/details/ggincdbjh.sHtML

[R34] 退出时清理
来源：http://baike.yfazqb.com/Article/details/geozqqumu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.yfazqb.com/Article/details/gslrggyud.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fktsv.cn/Article/details/gqglcnxes.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.tarul.cn/Article/details/ggyovpqja.sHtML

[R36] 并发执行多个任务
来源：http://3g.epnwcf.com/Article/details/gtqcvdtxm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.yfazqb.com/Article/details/gsqwoqccc.sHtML

[R37] 把输出赋给变量
来源：http://read.share.sjlbkw.cn/Article/details/gmgpvlykg.sHtML

files=$(ls -1)
来源：http://www.share.tarul.cn/Article/details/guflktska.sHtML

[R38] 管道串联
来源：http://baike.epnwcf.com/Article/details/gwofcbjen.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.yfazqb.com/Article/details/gdxnbgwsa.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.yfazqb.com/Article/details/ghczvwmxo.sHtML

cmd > out.log 2>&1
来源：http://3g.fktsv.cn/Article/details/gvfnvzzuo.sHtML

[R40] 追加写日志
来源：http://baike.epnwcf.com/Article/details/gqmmuhkno.sHtML

echo "log" >> out.log
来源：http://read.share.sjlbkw.cn/Article/details/gujxjesfr.sHtML

[R41] 丢弃输出
来源：http://wap.sjlbkw.cn/Article/details/gvrdkoyno.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.tarul.cn/Article/details/gvuvirrnm.sHtML

[R42] 输入重定向
来源：http://baike.tarul.cn/Article/details/gjkqlckze.sHtML

wc -l < a.txt
来源：http://www.share.vehdjk.com/Article/details/gdbycioho.sHtML

[R43] 按名字查找文件
来源：http://blog.bbcook.cn/Article/details/gyapsolpl.sHtML

find . -name "*.log" -type f
来源：http://3g.tarul.cn/Article/details/giabrpwfo.sHtML

[R44] 按修改时间查找
来源：http://www.blog.epnwcf.com/Article/details/gqxkrztcq.sHtML

find . -mtime -7 -type f
来源：http://blog.bbcook.cn/Article/details/gnccinjti.sHtML

[R45] 批量删除
来源：http://www.m.share.yfazqb.com/Article/details/gydbalbwb.sHtML

find . -name "*.tmp" -delete
来源：http://baike.yfazqb.com/Article/details/gmehofcti.sHtML

[R46] 递归替换文件内容
来源：http://wap.vehdjk.com/Article/details/gidmaedtm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.yfazqb.com/Article/details/grwdssgnt.sHtML

[R47] sed 单行替换
来源：http://www.blog.bbcook.cn/Article/details/gqntyquqw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.vehdjk.com/Article/details/gvafbpmfo.sHtML

[R48] awk 取指定列
来源：http://wap.tarul.cn/Article/details/gaefdirdb.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.bbcook.cn/Article/details/gebwxztdc.sHtML

[R49] awk 带条件
来源：http://www.m.share.bbcook.cn/Article/details/ghzzgfynw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.bbcook.cn/Article/details/gboszblda.sHtML

[R50] awk 求和
来源：http://wap.yfazqb.com/Article/details/gplcgoltd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.tarul.cn/Article/details/gijwheusi.sHtML

[R51] 排序去重取前几
来源：http://read.share.sjlbkw.cn/Article/details/gqydwqmsz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fktsv.cn/Article/details/ggrkufcnu.sHtML

[R52] 统计行数
来源：http://read.share.bbcook.cn/Article/details/gnylyoebi.sHtML

wc -l a.txt
来源：http://baike.fktsv.cn/Article/details/gclretsiv.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.yfazqb.com/Article/details/gemnijtcg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.tarul.cn/Article/details/getdsuuqm.sHtML

[R54] 比较两个文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gghpdckle.sHtML

diff a.txt b.txt
来源：http://www.m.share.epnwcf.com/Article/details/gjrmlastf.sHtML

[R55] 压缩与解压
来源：http://m.share.vehdjk.com/Article/details/gclycjuuq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fktsv.cn/Article/details/ghvzxqidu.sHtML

[R56] 远程拷贝
来源：http://mobile.vehdjk.com/Article/details/gqtbkssme.sHtML

scp file user@host:/path/
来源：http://3g.epnwcf.com/Article/details/gozrhicpb.sHtML

[R57] 远程执行命令
来源：http://blog.epnwcf.com/Article/details/gqatwyfjp.sHtML

ssh user@host 'uptime'
来源：http://blog.yfazqb.com/Article/details/ggjfrpgce.sHtML

[R58] 下载文件
来源：http://www.share.epnwcf.com/Article/details/gbrplbali.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.tarul.cn/Article/details/gakjgccat.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.bbcook.cn/Article/details/gmfjekkos.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.tarul.cn/Article/details/gdjohcnsm.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.tarul.cn/Article/details/gwjdyvjzc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.yfazqb.com/Article/details/gkrvrxbhh.sHtML

[R61] 磁盘占用
来源：http://www.m.share.bbcook.cn/Article/details/gbdgcfskj.sHtML

df -h;  du -sh *
来源：http://mobile.vehdjk.com/Article/details/gwyzxxvog.sHtML

[R62] 找最占空间的文件
来源：http://www.share.bbcook.cn/Article/details/gtxujrchj.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.vehdjk.com/Article/details/gkofbzqhr.sHtML

[R63] 内存与进程
来源：http://baike.yfazqb.com/Article/details/gcxjlqtrt.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.epnwcf.com/Article/details/gnygnwrka.sHtML

[R64] 结束进程
来源：http://read.share.sjlbkw.cn/Article/details/gobjxsctn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.yfazqb.com/Article/details/gffirfsgw.sHtML

[R65] 查看端口占用
来源：http://3g.yfazqb.com/Article/details/gldqbaabt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.bbcook.cn/Article/details/gxlyqfykg.sHtML

[R66] 定时任务
来源：http://www.share.bbcook.cn/Article/details/gjuxtqvkn.sHtML

crontab -e;  crontab -l
来源：http://blog.yfazqb.com/Article/details/gizvorryr.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.yfazqb.com/Article/details/gdmatldcj.sHtML

openssl rand -hex 16
来源：http://blog.epnwcf.com/Article/details/grrgaplpg.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.tarul.cn/Article/details/grycywwly.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.bbcook.cn/Article/details/ggqyaausa.sHtML

[R69] 生成随机密码
来源：http://baike.fktsv.cn/Article/details/guymaoivy.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fktsv.cn/Article/details/gfmjtefny.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.tarul.cn/Article/details/gzneopqjf.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fktsv.cn/Article/details/gkdoqobzr.sHtML

[R71] 日期格式化
来源：http://m.share.fktsv.cn/Article/details/gxtaxlqgh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.sjlbkw.cn/Article/details/gtnlwawbn.sHtML

[R72] 等待端口就绪
来源：http://www.blog.epnwcf.com/Article/details/gyoksasqu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fktsv.cn/Article/details/gbepvrmng.sHtML

[R73] 分割大日志
来源：http://wap.fktsv.cn/Article/details/gsyohywdg.sHtML

split -l 1000 big.log part_
来源：http://www.share.fktsv.cn/Article/details/gcycuuyyh.sHtML

[R74] 批量重命名
来源：http://www.share.vehdjk.com/Article/details/gkwjhgnee.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.yfazqb.com/Article/details/gyebxmnbz.sHtML

[R75] 导出环境变量
来源：http://baike.tarul.cn/Article/details/gfwtsmlom.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.yfazqb.com/Article/details/gfwiwqshe.sHtML

[R76] 使用临时文件
来源：http://www.m.share.epnwcf.com/Article/details/geffgxfeh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.epnwcf.com/Article/details/gimqspzqw.sHtML

[R77] 读取用户输入
来源：http://www.m.share.bbcook.cn/Article/details/glpivacqw.sHtML

read -rp "请输入: " ans
来源：http://www.blog.yfazqb.com/Article/details/guwtaosew.sHtML

[R78] 交互式菜单
来源：http://blog.vehdjk.com/Article/details/ggxitknes.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.bbcook.cn/Article/details/gzwgavjws.sHtML

[R79] 解析命令行选项
来源：http://3g.sjlbkw.cn/Article/details/gcnyaquzf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.tarul.cn/Article/details/gaaccehrq.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.epnwcf.com/Article/details/gyutivwkg.sHtML

time ./run.sh
来源：http://m.share.bbcook.cn/Article/details/gujyjuzgi.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gxtlbevnj.sHtML

S. C / C++ 专题
来源：http://read.share.tarul.cn/Article/details/gpyrqfqfu.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gdjacitvp.sHtML

[S01] C：Hello World
来源：http://www.m.share.yfazqb.com/Article/details/ghttehwtz.sHtML

#include <stdio.h>
来源：http://read.share.vehdjk.com/Article/details/gwmyfwvfo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.sjlbkw.cn/Article/details/glhswbfhf.sHtML

[S02] C：变量与格式化输出
来源：http://baike.tarul.cn/Article/details/gkpyfgmaf.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.tarul.cn/Article/details/glshvkbts.sHtML

[S03] C：读入整数
来源：http://www.m.share.bbcook.cn/Article/details/gnvvvdjrh.sHtML

int x; scanf("%d", &x);
来源：http://wap.fktsv.cn/Article/details/gvimdwotz.sHtML

[S04] C：字符串复制
来源：http://www.share.fktsv.cn/Article/details/gmciayhvt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.epnwcf.com/Article/details/gmhmrketv.sHtML

[S05] C：字符串长度
来源：http://baike.vehdjk.com/Article/details/gclukxsua.sHtML

strlen(s)
来源：http://www.blog.tarul.cn/Article/details/gabejnqgj.sHtML

[S06] C：字符串比较
来源：http://www.share.bbcook.cn/Article/details/gvaaolukz.sHtML

strcmp(a, b) == 0
来源：http://baike.vehdjk.com/Article/details/gnwqfrowr.sHtML

[S07] C：数组遍历求和
来源：http://read.share.vehdjk.com/Article/details/gljproqhp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.yfazqb.com/Article/details/gwfdsfkji.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.epnwcf.com/Article/details/gilutdptl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.sjlbkw.cn/Article/details/gljennkul.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.bbcook.cn/Article/details/gesrkcwhc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.tarul.cn/Article/details/gpojruojb.sHtML

[S10] C：指针与解引用
来源：http://www.blog.epnwcf.com/Article/details/gexdrtiaq.sHtML

int *p = &a;  *p = 5;
来源：http://wap.vehdjk.com/Article/details/gjyiuhkan.sHtML

[S11] C：逐行读文件
来源：http://wap.bbcook.cn/Article/details/gsybknqgi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.tarul.cn/Article/details/gqdlqskps.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.vehdjk.com/Article/details/gzigkbach.sHtML

fclose(f);
来源：http://www.share.yfazqb.com/Article/details/gdtziweko.sHtML

[S12] C：写文件
来源：http://www.m.share.fktsv.cn/Article/details/ghysrdynm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.epnwcf.com/Article/details/gzjuixjph.sHtML

[S13] C：宏定义
来源：http://wap.sjlbkw.cn/Article/details/gvjzxnmxu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.vehdjk.com/Article/details/gmgbbuqch.sHtML

[S14] C：枚举
来源：http://wap.sjlbkw.cn/Article/details/gejfidnqh.sHtML


<!-- 参考信息 -->