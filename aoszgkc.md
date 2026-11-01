代发 wailian999

[Q48] CTE 公用表表达式
来源：http://www.m.share.yfazqb.com/Article/details/gpnwenlgd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.vehdjk.com/Article/details/gqupffjdp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.tarul.cn/Article/details/gbnnsvqcs.sHtML

[Q49] 更新单行
来源：http://3g.tarul.cn/Article/details/grnlrbofq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.epnwcf.com/Article/details/gxouzihgs.sHtML

[Q50] 批量更新
来源：http://read.share.yfazqb.com/Article/details/gmvjyirkr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fktsv.cn/Article/details/gldmzytag.sHtML

[Q51] 用子查询更新
来源：http://read.share.yfazqb.com/Article/details/gqzlpouoi.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.sjlbkw.cn/Article/details/grjgchrrs.sHtML

[Q52] 删除指定行
来源：http://m.share.epnwcf.com/Article/details/gotnwjczq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.yfazqb.com/Article/details/gcbebbxan.sHtML

[Q53] 按条件删除
来源：http://www.share.yfazqb.com/Article/details/gmmsbbryw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.epnwcf.com/Article/details/gbmmlwlou.sHtML

[Q54] 清空表
来源：http://3g.sjlbkw.cn/Article/details/gtesewmuv.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.bbcook.cn/Article/details/gnthykxgv.sHtML

[Q55] 排名（并列占位）
来源：http://blog.bbcook.cn/Article/details/ghlbgwprg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fktsv.cn/Article/details/gkvvkryci.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.sjlbkw.cn/Article/details/gniggapuj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.tarul.cn/Article/details/gasxvuvmq.sHtML

[Q57] 行号
来源：http://3g.epnwcf.com/Article/details/gidelhmey.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.yfazqb.com/Article/details/gbdtsawwa.sHtML

[Q58] 累计求和
来源：http://www.blog.bbcook.cn/Article/details/gwhndhyad.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.epnwcf.com/Article/details/gleiaoqns.sHtML

[Q59] 分组内累计
来源：http://3g.yfazqb.com/Article/details/geruzrocb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fktsv.cn/Article/details/gvadxgwby.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.sjlbkw.cn/Article/details/gsmezfduu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.vehdjk.com/Article/details/gbqcloisw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.epnwcf.com/Article/details/gcirjlneo.sHtML

[Q61] 移动平均
来源：http://m.share.epnwcf.com/Article/details/ggoxrjmfk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.epnwcf.com/Article/details/garltivmr.sHtML

[Q62] 分组占比
来源：http://www.share.fktsv.cn/Article/details/gqqmkjlkh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.tarul.cn/Article/details/gupjyadxr.sHtML

[Q63] 开启事务
来源：http://baike.vehdjk.com/Article/details/gkfywqmdd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fktsv.cn/Article/details/gratezqcq.sHtML

[Q64] 提交事务
来源：http://www.m.share.vehdjk.com/Article/details/gqlaediiq.sHtML

COMMIT;
来源：http://blog.sjlbkw.cn/Article/details/gzyajzhwc.sHtML

[Q65] 回滚事务
来源：http://www.share.epnwcf.com/Article/details/gllqhdlhg.sHtML

ROLLBACK;
来源：http://www.m.share.fktsv.cn/Article/details/gdmauriiu.sHtML

[Q66] 行锁查询
来源：http://3g.vehdjk.com/Article/details/gwrnfpnyt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.vehdjk.com/Article/details/gzribuvai.sHtML

[Q67] 设置隔离级别
来源：http://www.share.bbcook.cn/Article/details/gkfexjeqj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.yfazqb.com/Article/details/gzttbtojn.sHtML

[Q68] 保存点
来源：http://blog.tarul.cn/Article/details/gtcunkkvz.sHtML

SAVEPOINT sp1;
来源：http://www.blog.yfazqb.com/Article/details/gnxujisnr.sHtML

ROLLBACK TO sp1;
来源：http://wap.bbcook.cn/Article/details/glvsrosol.sHtML

[Q69] 查看执行计划
来源：http://3g.epnwcf.com/Article/details/gjetpuozr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.epnwcf.com/Article/details/gbzbmsery.sHtML

[Q70] 更新统计信息
来源：http://m.share.vehdjk.com/Article/details/gnyiraixh.sHtML

ANALYZE TABLE users;
来源：http://blog.epnwcf.com/Article/details/gxglgnrtj.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fktsv.cn/Article/details/gjgtabkyb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fktsv.cn/Article/details/gyeihtnzm.sHtML

[Q72] 查看索引
来源：http://baike.tarul.cn/Article/details/gmktwkklm.sHtML

SHOW INDEX FROM users;
来源：http://m.share.epnwcf.com/Article/details/gngzrpmzo.sHtML

[Q73] 查看表状态
来源：http://blog.bbcook.cn/Article/details/gfoixpcjr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.bbcook.cn/Article/details/gdgpxxfew.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.tarul.cn/Article/details/gdwloxbey.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.bbcook.cn/Article/details/gxhalynjf.sHtML

[Q75] 日期格式化
来源：http://wap.bbcook.cn/Article/details/ggpucjpwc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.tarul.cn/Article/details/gcfkosjol.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.yfazqb.com/Article/details/gkypdtnpx.sHtML

[Q76] 按天统计
来源：http://www.share.epnwcf.com/Article/details/gsbdhqizs.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.tarul.cn/Article/details/grzqtmcun.sHtML

[Q77] 时间加减
来源：http://read.share.fktsv.cn/Article/details/gkdhusvtt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.tarul.cn/Article/details/gmrfpvxwa.sHtML

[Q78] 当前时间
来源：http://baike.vehdjk.com/Article/details/gosiqqtut.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.yfazqb.com/Article/details/gmpirbyrb.sHtML

[Q79] 字符串拼接
来源：http://3g.bbcook.cn/Article/details/gfnbivfzn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.vehdjk.com/Article/details/gsrvhbkyb.sHtML

[Q80] 字符串截取
来源：http://wap.bbcook.cn/Article/details/gtfofypki.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gkcdcwxda.sHtML

[Q81] 字符串替换
来源：http://www.blog.vehdjk.com/Article/details/gtysggblz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gttqheclw.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fktsv.cn/Article/details/gtlmwimvf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.bbcook.cn/Article/details/gygzwemnc.sHtML

[Q83] 大小写转换
来源：http://m.share.yfazqb.com/Article/details/gdzfdpjsi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.vehdjk.com/Article/details/gxkykbpuv.sHtML

[Q84] 去除首尾空格
来源：http://www.share.bbcook.cn/Article/details/gmrqovogv.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gyhhovuhn.sHtML

[Q85] 数值取整
来源：http://baike.fktsv.cn/Article/details/gfgnjyilw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fktsv.cn/Article/details/gechwkrjn.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.yfazqb.com/Article/details/gtvbvwacd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.sjlbkw.cn/Article/details/gqwbgozfy.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.bbcook.cn/Article/details/gurkdsbsm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fktsv.cn/Article/details/gnhpygjns.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.bbcook.cn/Article/details/gszurwnsa.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.vehdjk.com/Article/details/gzqianhjd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gqfknzpow.sHtML

[Q89] 判断表是否存在
来源：http://mobile.bbcook.cn/Article/details/gwtiufora.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.bbcook.cn/Article/details/goutzjynz.sHtML

[Q90] 生成序号列
来源：http://read.share.sjlbkw.cn/Article/details/grsvgkzkk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.yfazqb.com/Article/details/gnyewuvdi.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gnxubfaeb.sHtML

R. Bash 专题
来源：http://baike.fktsv.cn/Article/details/gwbpfdbbq.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gdngcjggz.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.tarul.cn/Article/details/gfrvlcyzv.sHtML

#!/usr/bin/env bash
来源：http://mobile.fktsv.cn/Article/details/gwrrlcqgh.sHtML

set -euo pipefail
来源：http://blog.epnwcf.com/Article/details/ghpsvjiqy.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.bbcook.cn/Article/details/gcfuadvss.sHtML

name="Tom"; echo "$name"
来源：http://3g.tarul.cn/Article/details/ggfwqbkcs.sHtML

[R03] 只读变量
来源：http://blog.sjlbkw.cn/Article/details/gxtcoucib.sHtML

readonly PI=3.14
来源：http://mobile.bbcook.cn/Article/details/gqsajgpbf.sHtML

[R04] 位置参数
来源：http://mobile.tarul.cn/Article/details/geltkurxw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.vehdjk.com/Article/details/giwzygnhg.sHtML

[R05] 参数默认值
来源：http://wap.vehdjk.com/Article/details/ggrruacmp.sHtML

name="${1:-default}"
来源：http://3g.sjlbkw.cn/Article/details/gpshamxwm.sHtML

[R06] 判断命令是否存在
来源：http://3g.vehdjk.com/Article/details/gmntvrrcx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.tarul.cn/Article/details/gikssplnd.sHtML

[R07] if 判断文件
来源：http://www.share.yfazqb.com/Article/details/gyqecpnec.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.bbcook.cn/Article/details/gvugaacya.sHtML

[R08] 数值比较
来源：http://3g.bbcook.cn/Article/details/guwshvqql.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.epnwcf.com/Article/details/gothmulsv.sHtML

[R09] 字符串比较
来源：http://blog.tarul.cn/Article/details/gzakmdors.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.tarul.cn/Article/details/glciapxlo.sHtML

[R10] 正则匹配
来源：http://wap.epnwcf.com/Article/details/ghtpdvmkf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.vehdjk.com/Article/details/gpggjufci.sHtML

[R11] case 多分支
来源：http://mobile.epnwcf.com/Article/details/gxnnzkcds.sHtML

case "$1" in
来源：http://baike.fktsv.cn/Article/details/guofhitjy.sHtML

start) echo "启动" ;;
来源：http://www.share.bbcook.cn/Article/details/glbperpxp.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.vehdjk.com/Article/details/gfyuwfcup.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.tarul.cn/Article/details/gmzjplosd.sHtML

esac
来源：http://m.share.vehdjk.com/Article/details/gdeqqgqgb.sHtML

[R12] for 遍历文件
来源：http://www.share.bbcook.cn/Article/details/gzkzllvmv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.epnwcf.com/Article/details/gcwlfgoot.sHtML

[R13] for 计数循环
来源：http://3g.vehdjk.com/Article/details/gwmkvmiyi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fktsv.cn/Article/details/gokkhzizv.sHtML

[R14] C 风格 for
来源：http://read.share.sjlbkw.cn/Article/details/gmkpopoba.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.vehdjk.com/Article/details/gsynqqxeo.sHtML

[R15] while 逐行读文件
来源：http://wap.fktsv.cn/Article/details/gkkyznqte.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.epnwcf.com/Article/details/gjlkhonxo.sHtML

[R16] until 等待条件
来源：http://read.share.vehdjk.com/Article/details/gnldircbj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.yfazqb.com/Article/details/grrzjvich.sHtML

[R17] 数组定义与取值
来源：http://3g.epnwcf.com/Article/details/gbmszkqnk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.yfazqb.com/Article/details/grpjkywyv.sHtML

[R18] 遍历数组
来源：http://wap.epnwcf.com/Article/details/ghipyyszd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.bbcook.cn/Article/details/gbhfvhjhx.sHtML

[R19] 数组长度
来源：http://www.blog.bbcook.cn/Article/details/ghmpdabjk.sHtML

echo "${#arr[@]}"
来源：http://read.share.tarul.cn/Article/details/gvjygwcyb.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.yfazqb.com/Article/details/ggfdyldmm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.tarul.cn/Article/details/ganfkywcl.sHtML

[R21] 字符串长度
来源：http://blog.vehdjk.com/Article/details/gfxkguaty.sHtML

echo "${#s}"
来源：http://read.share.tarul.cn/Article/details/gpivdzusm.sHtML

[R22] 截取子串
来源：http://3g.sjlbkw.cn/Article/details/gplojeaag.sHtML

echo "${s:0:5}"
来源：http://3g.tarul.cn/Article/details/gpmmphzwj.sHtML

[R23] 字符串替换
来源：http://www.share.bbcook.cn/Article/details/gpwyyqhea.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.bbcook.cn/Article/details/gnhokeura.sHtML

[R24] 大小写转换
来源：http://blog.fktsv.cn/Article/details/ggassjjff.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.vehdjk.com/Article/details/gwhnobswk.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.tarul.cn/Article/details/gyxabwwsd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.vehdjk.com/Article/details/gdsllvxcs.sHtML

[R26] 命令替换
来源：http://blog.yfazqb.com/Article/details/gbqccdpjg.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.bbcook.cn/Article/details/gnyzjteaj.sHtML

[R27] 算术展开
来源：http://wap.vehdjk.com/Article/details/gyanpomyn.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.yfazqb.com/Article/details/gszztbyzm.sHtML

[R28] 浮点运算
来源：http://www.blog.yfazqb.com/Article/details/gdduvyshq.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.vehdjk.com/Article/details/gsftijgyv.sHtML

[R29] 定义函数
来源：http://wap.fktsv.cn/Article/details/gxiehslxh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.yfazqb.com/Article/details/gygloikgf.sHtML

[R30] 函数返回状态码
来源：http://3g.bbcook.cn/Article/details/gwvkgduff.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.tarul.cn/Article/details/gpzhhnsrf.sHtML

[R31] 局部变量
来源：http://www.share.yfazqb.com/Article/details/gszuxwjkr.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.sjlbkw.cn/Article/details/gnnqogxyw.sHtML

[R32] 参数个数校验
来源：http://www.blog.yfazqb.com/Article/details/gttmzkwem.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.bbcook.cn/Article/details/glxgvhaxs.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fktsv.cn/Article/details/gxkbrxrai.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.yfazqb.com/Article/details/gtqowkrzs.sHtML

[R34] 退出时清理
来源：http://blog.yfazqb.com/Article/details/gafwvbvzf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.vehdjk.com/Article/details/gejxbfohu.sHtML

[R35] 后台执行并等待
来源：http://3g.vehdjk.com/Article/details/gfyjqomjb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.vehdjk.com/Article/details/ghultkggl.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.yfazqb.com/Article/details/gxytqaswg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.tarul.cn/Article/details/gvlbaumiq.sHtML

[R37] 把输出赋给变量
来源：http://m.share.sjlbkw.cn/Article/details/gwguzfuxa.sHtML

files=$(ls -1)
来源：http://blog.bbcook.cn/Article/details/gytbudwye.sHtML

[R38] 管道串联
来源：http://www.share.sjlbkw.cn/Article/details/gptxjzule.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.yfazqb.com/Article/details/guoffqjga.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.tarul.cn/Article/details/gcixhkcee.sHtML

cmd > out.log 2>&1
来源：http://3g.tarul.cn/Article/details/gknugxwjj.sHtML

[R40] 追加写日志
来源：http://www.share.bbcook.cn/Article/details/gmdzbggdo.sHtML

echo "log" >> out.log
来源：http://3g.sjlbkw.cn/Article/details/gopumynvw.sHtML

[R41] 丢弃输出
来源：http://3g.vehdjk.com/Article/details/gnwmgcwuz.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.vehdjk.com/Article/details/gjhogjuhv.sHtML

[R42] 输入重定向
来源：http://3g.vehdjk.com/Article/details/gqfqljvat.sHtML

wc -l < a.txt
来源：http://3g.epnwcf.com/Article/details/glhogdber.sHtML

[R43] 按名字查找文件
来源：http://blog.yfazqb.com/Article/details/gxyixjfqy.sHtML

find . -name "*.log" -type f
来源：http://read.share.bbcook.cn/Article/details/gwassadbf.sHtML

[R44] 按修改时间查找
来源：http://www.blog.epnwcf.com/Article/details/gqomxroze.sHtML

find . -mtime -7 -type f
来源：http://m.share.yfazqb.com/Article/details/gzsvbsehp.sHtML

[R45] 批量删除
来源：http://baike.epnwcf.com/Article/details/gkszxpshl.sHtML

find . -name "*.tmp" -delete
来源：http://baike.yfazqb.com/Article/details/gfngkkltq.sHtML

[R46] 递归替换文件内容
来源：http://read.share.yfazqb.com/Article/details/gorvrhejx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.epnwcf.com/Article/details/gijkacexx.sHtML

[R47] sed 单行替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gzssdqguy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.vehdjk.com/Article/details/gtgkkokjt.sHtML

[R48] awk 取指定列
来源：http://www.m.share.bbcook.cn/Article/details/gxjgquapp.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.sjlbkw.cn/Article/details/gjtkqvefa.sHtML

[R49] awk 带条件
来源：http://baike.vehdjk.com/Article/details/gkqkvtkgb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.epnwcf.com/Article/details/govtnrcdp.sHtML

[R50] awk 求和
来源：http://wap.tarul.cn/Article/details/gtktummya.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.sjlbkw.cn/Article/details/gcbbsfpty.sHtML

[R51] 排序去重取前几
来源：http://read.share.epnwcf.com/Article/details/gfavkbfqh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.yfazqb.com/Article/details/gulreqlmg.sHtML

[R52] 统计行数
来源：http://www.share.fktsv.cn/Article/details/glqxxkxcd.sHtML

wc -l a.txt
来源：http://www.m.share.vehdjk.com/Article/details/gcspsteso.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fktsv.cn/Article/details/gzkowyqhp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.tarul.cn/Article/details/gakmmpktd.sHtML

[R54] 比较两个文件
来源：http://3g.tarul.cn/Article/details/gyonmnesa.sHtML

diff a.txt b.txt
来源：http://mobile.tarul.cn/Article/details/gbpqspolt.sHtML

[R55] 压缩与解压
来源：http://read.share.sjlbkw.cn/Article/details/goeumlcps.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.bbcook.cn/Article/details/gmzzyauns.sHtML

[R56] 远程拷贝
来源：http://m.share.yfazqb.com/Article/details/gnpkziwap.sHtML

scp file user@host:/path/
来源：http://blog.sjlbkw.cn/Article/details/gvuigpftc.sHtML

[R57] 远程执行命令
来源：http://mobile.yfazqb.com/Article/details/gpfbmvpev.sHtML

ssh user@host 'uptime'
来源：http://www.blog.epnwcf.com/Article/details/gszwdhuuy.sHtML

[R58] 下载文件
来源：http://www.blog.sjlbkw.cn/Article/details/ggfigxrzh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.bbcook.cn/Article/details/gkoxsbwjq.sHtML

[R59] 发 POST JSON
来源：http://m.share.tarul.cn/Article/details/gabnkwbxy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fktsv.cn/Article/details/gzmankbsg.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.bbcook.cn/Article/details/gqfjohbcs.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.tarul.cn/Article/details/gwktfkmqp.sHtML

[R61] 磁盘占用
来源：http://wap.vehdjk.com/Article/details/guimbjsht.sHtML

df -h;  du -sh *
来源：http://3g.fktsv.cn/Article/details/gbgmuyiit.sHtML

[R62] 找最占空间的文件
来源：http://baike.sjlbkw.cn/Article/details/gacxriqac.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.vehdjk.com/Article/details/gyrjvzvui.sHtML

[R63] 内存与进程
来源：http://baike.yfazqb.com/Article/details/ggenggjda.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.sjlbkw.cn/Article/details/gurhzemvi.sHtML

[R64] 结束进程
来源：http://mobile.bbcook.cn/Article/details/gudfqpslf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.epnwcf.com/Article/details/gmpjuodpi.sHtML

[R65] 查看端口占用
来源：http://www.share.epnwcf.com/Article/details/gtcvbbilm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.tarul.cn/Article/details/gqxfdgahr.sHtML

[R66] 定时任务
来源：http://3g.bbcook.cn/Article/details/gsctpiipa.sHtML

crontab -e;  crontab -l
来源：http://read.share.sjlbkw.cn/Article/details/gqatpecgk.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.tarul.cn/Article/details/gljodttrl.sHtML

openssl rand -hex 16
来源：http://3g.tarul.cn/Article/details/gjjbybxif.sHtML

[R68] 计算文件校验值
来源：http://www.share.fktsv.cn/Article/details/gydyukvhs.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.bbcook.cn/Article/details/gtuplccuy.sHtML

[R69] 生成随机密码
来源：http://mobile.fktsv.cn/Article/details/gcknvatht.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.vehdjk.com/Article/details/gismagmra.sHtML

[R70] 时间戳与互转
来源：http://mobile.tarul.cn/Article/details/gqgktvrhu.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.vehdjk.com/Article/details/gmtnixeib.sHtML

[R71] 日期格式化
来源：http://wap.sjlbkw.cn/Article/details/gxmrxulxj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.bbcook.cn/Article/details/gwiuejbqn.sHtML

[R72] 等待端口就绪
来源：http://3g.fktsv.cn/Article/details/gbhfyoecs.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.yfazqb.com/Article/details/glihwcwxy.sHtML

[R73] 分割大日志
来源：http://m.share.fktsv.cn/Article/details/gpzcjaimq.sHtML

split -l 1000 big.log part_
来源：http://3g.sjlbkw.cn/Article/details/gszycojpg.sHtML

[R74] 批量重命名
来源：http://www.m.share.vehdjk.com/Article/details/gzzgjedtb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.yfazqb.com/Article/details/gbwabpogd.sHtML

[R75] 导出环境变量
来源：http://baike.fktsv.cn/Article/details/gqpybsjts.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.epnwcf.com/Article/details/gtaxeyuhz.sHtML

[R76] 使用临时文件
来源：http://3g.bbcook.cn/Article/details/grxbgcrqc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fktsv.cn/Article/details/gmwosbygj.sHtML

[R77] 读取用户输入
来源：http://www.blog.tarul.cn/Article/details/ghraxplpu.sHtML

read -rp "请输入: " ans
来源：http://read.share.vehdjk.com/Article/details/gnbfcopye.sHtML

[R78] 交互式菜单
来源：http://www.m.share.tarul.cn/Article/details/gmqemavxg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.tarul.cn/Article/details/ghexyfhtw.sHtML

[R79] 解析命令行选项
来源：http://3g.sjlbkw.cn/Article/details/gsamfnbpa.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.yfazqb.com/Article/details/gqhxhrayr.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.sjlbkw.cn/Article/details/godelwats.sHtML

time ./run.sh
来源：http://m.share.yfazqb.com/Article/details/gbfuafuyx.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/glafiobjv.sHtML

S. C / C++ 专题
来源：http://3g.epnwcf.com/Article/details/gtztefhcc.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/glhuegyiw.sHtML

[S01] C：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gxdojvwqb.sHtML

#include <stdio.h>
来源：http://www.share.bbcook.cn/Article/details/glkbjofah.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.yfazqb.com/Article/details/gxnnzviia.sHtML

[S02] C：变量与格式化输出
来源：http://3g.sjlbkw.cn/Article/details/gxyygdxha.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.bbcook.cn/Article/details/gndxqbfai.sHtML

[S03] C：读入整数
来源：http://3g.yfazqb.com/Article/details/gxqdfdijv.sHtML

int x; scanf("%d", &x);
来源：http://mobile.bbcook.cn/Article/details/gewznindk.sHtML

[S04] C：字符串复制
来源：http://mobile.epnwcf.com/Article/details/goyffdgrq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.yfazqb.com/Article/details/goaxpkbxr.sHtML

[S05] C：字符串长度
来源：http://wap.tarul.cn/Article/details/gxonuzlhi.sHtML

strlen(s)
来源：http://m.share.sjlbkw.cn/Article/details/gfxcwekad.sHtML

[S06] C：字符串比较
来源：http://blog.bbcook.cn/Article/details/gcasgotyf.sHtML

strcmp(a, b) == 0
来源：http://3g.fktsv.cn/Article/details/girlwuuma.sHtML

[S07] C：数组遍历求和
来源：http://wap.bbcook.cn/Article/details/ggjdhjoyg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.yfazqb.com/Article/details/grwcipdyw.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.sjlbkw.cn/Article/details/ghhxcwdjp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fktsv.cn/Article/details/gwgiaqxsz.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.yfazqb.com/Article/details/ghfxmjpkg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.tarul.cn/Article/details/gmfixdkyn.sHtML

[S10] C：指针与解引用
来源：http://www.share.vehdjk.com/Article/details/gnixvupol.sHtML

int *p = &a;  *p = 5;
来源：http://3g.vehdjk.com/Article/details/glnrjiuxz.sHtML

[S11] C：逐行读文件
来源：http://www.blog.bbcook.cn/Article/details/gmdvvlrvh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.epnwcf.com/Article/details/guizwozgb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.vehdjk.com/Article/details/gwdvxdsai.sHtML

fclose(f);
来源：http://m.share.vehdjk.com/Article/details/gldsemuri.sHtML

[S12] C：写文件
来源：http://www.share.sjlbkw.cn/Article/details/gijbjqovx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fktsv.cn/Article/details/goliaxfvt.sHtML

[S13] C：宏定义
来源：http://m.share.sjlbkw.cn/Article/details/gcxmcwylh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.sjlbkw.cn/Article/details/gqhhowobw.sHtML

[S14] C：枚举
来源：http://read.share.tarul.cn/Article/details/gltslljca.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.bbcook.cn/Article/details/gmvlafhcm.sHtML

[S15] C：类型转换
来源：http://baike.tarul.cn/Article/details/gvyuhbpzv.sHtML

(double) a / b
来源：http://wap.yfazqb.com/Article/details/gcqitwksj.sHtML

[S16] C：位操作置位
来源：http://blog.bbcook.cn/Article/details/gwdintqjn.sHtML

x |= (1 << 3);
来源：http://3g.sjlbkw.cn/Article/details/gjwvupurh.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.sjlbkw.cn/Article/details/gxuwqmalv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.yfazqb.com/Article/details/gzfmotgyv.sHtML

[S18] C：命令行参数
来源：http://baike.sjlbkw.cn/Article/details/gylogfmki.sHtML


<!-- 参考信息 -->