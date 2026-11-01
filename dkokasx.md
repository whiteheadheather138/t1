代发 wailian999

[Q61] 移动平均
来源：http://blog.sjlbkw.cn/Article/details/grdiranqt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.epnwcf.com/Article/details/govddvrgd.sHtML

[Q62] 分组占比
来源：http://mobile.tarul.cn/Article/details/grmbrpltp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.vehdjk.com/Article/details/gjgymddgn.sHtML

[Q63] 开启事务
来源：http://www.blog.epnwcf.com/Article/details/gpdwadrid.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.bbcook.cn/Article/details/gbsmnhuco.sHtML

[Q64] 提交事务
来源：http://3g.fktsv.cn/Article/details/gjeirvbis.sHtML

COMMIT;
来源：http://mobile.epnwcf.com/Article/details/grubbxdos.sHtML

[Q65] 回滚事务
来源：http://wap.sjlbkw.cn/Article/details/gwzxyebis.sHtML

ROLLBACK;
来源：http://baike.fktsv.cn/Article/details/gshnmzqsn.sHtML

[Q66] 行锁查询
来源：http://read.share.sjlbkw.cn/Article/details/gkxdlwheq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.sjlbkw.cn/Article/details/glcckqpmm.sHtML

[Q67] 设置隔离级别
来源：http://baike.sjlbkw.cn/Article/details/gvctxjwbc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.vehdjk.com/Article/details/gezvkndma.sHtML

[Q68] 保存点
来源：http://wap.fktsv.cn/Article/details/gheyojihh.sHtML

SAVEPOINT sp1;
来源：http://baike.tarul.cn/Article/details/gumukplfh.sHtML

ROLLBACK TO sp1;
来源：http://www.share.vehdjk.com/Article/details/gnvfjxhxw.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.sjlbkw.cn/Article/details/ggfgwaykd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.bbcook.cn/Article/details/ghlbpxjky.sHtML

[Q70] 更新统计信息
来源：http://3g.bbcook.cn/Article/details/gddnufkhw.sHtML

ANALYZE TABLE users;
来源：http://read.share.epnwcf.com/Article/details/gcqgfhhzw.sHtML

[Q71] 查看建表语句
来源：http://3g.bbcook.cn/Article/details/gpaeumtgi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.yfazqb.com/Article/details/gprkytynq.sHtML

[Q72] 查看索引
来源：http://3g.yfazqb.com/Article/details/gaatvuxps.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gadxszmpv.sHtML

[Q73] 查看表状态
来源：http://wap.tarul.cn/Article/details/gfbyyxiry.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.epnwcf.com/Article/details/gsmxutcck.sHtML

[Q74] 强制使用索引
来源：http://wap.sjlbkw.cn/Article/details/gvqufsvbg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.sjlbkw.cn/Article/details/gemyfipew.sHtML

[Q75] 日期格式化
来源：http://3g.vehdjk.com/Article/details/grxscnbyu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.bbcook.cn/Article/details/grmrkvfxt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.epnwcf.com/Article/details/gjvenjvba.sHtML

[Q76] 按天统计
来源：http://read.share.yfazqb.com/Article/details/grkakincn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.sjlbkw.cn/Article/details/gkjkiphzg.sHtML

[Q77] 时间加减
来源：http://m.share.sjlbkw.cn/Article/details/gwakhfzxh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.yfazqb.com/Article/details/gxiwrporp.sHtML

[Q78] 当前时间
来源：http://read.share.sjlbkw.cn/Article/details/gtwoucfif.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.sjlbkw.cn/Article/details/gavfgbucz.sHtML

[Q79] 字符串拼接
来源：http://read.share.fktsv.cn/Article/details/gnjvawptv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.epnwcf.com/Article/details/gzrdxpdim.sHtML

[Q80] 字符串截取
来源：http://www.m.share.vehdjk.com/Article/details/gckclvlzd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gigkxxyae.sHtML

[Q81] 字符串替换
来源：http://read.share.vehdjk.com/Article/details/gwrfbpynn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.tarul.cn/Article/details/gpcvpyfkj.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.sjlbkw.cn/Article/details/givzgvvoo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.epnwcf.com/Article/details/gcvaehuej.sHtML

[Q83] 大小写转换
来源：http://3g.vehdjk.com/Article/details/giplgqkqd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fktsv.cn/Article/details/gzfbmkztq.sHtML

[Q84] 去除首尾空格
来源：http://m.share.tarul.cn/Article/details/gkmujojvq.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.bbcook.cn/Article/details/gvcflupkn.sHtML

[Q85] 数值取整
来源：http://wap.yfazqb.com/Article/details/gmgqpdkjk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.epnwcf.com/Article/details/gvsiheebi.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.tarul.cn/Article/details/gksejspom.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.bbcook.cn/Article/details/gpfeedlzm.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.vehdjk.com/Article/details/gmdmmkkmv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.sjlbkw.cn/Article/details/gervqhblk.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.epnwcf.com/Article/details/gddttvgsf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.bbcook.cn/Article/details/gwoddifiz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.bbcook.cn/Article/details/gpjsghygq.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.bbcook.cn/Article/details/glgevkhbm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.tarul.cn/Article/details/geyrelxzv.sHtML

[Q90] 生成序号列
来源：http://baike.bbcook.cn/Article/details/glwsqvnfr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.tarul.cn/Article/details/gounmqwlt.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gcqsaprcg.sHtML

R. Bash 专题
来源：http://blog.yfazqb.com/Article/details/gnjdrzgxx.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/goupezqeh.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.sjlbkw.cn/Article/details/ghtcyaooh.sHtML

#!/usr/bin/env bash
来源：http://3g.vehdjk.com/Article/details/ggoqrahku.sHtML

set -euo pipefail
来源：http://wap.yfazqb.com/Article/details/ghnmhvpat.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.bbcook.cn/Article/details/gsjteeoyd.sHtML

name="Tom"; echo "$name"
来源：http://3g.fktsv.cn/Article/details/gadcteaen.sHtML

[R03] 只读变量
来源：http://blog.epnwcf.com/Article/details/gmhmvqjbv.sHtML

readonly PI=3.14
来源：http://m.share.yfazqb.com/Article/details/glghsibym.sHtML

[R04] 位置参数
来源：http://m.share.bbcook.cn/Article/details/gxnyadbym.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.bbcook.cn/Article/details/gdetmowfc.sHtML

[R05] 参数默认值
来源：http://mobile.epnwcf.com/Article/details/gfbwbguwc.sHtML

name="${1:-default}"
来源：http://www.blog.epnwcf.com/Article/details/gbnrgtkrp.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fktsv.cn/Article/details/gbuziihrc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.tarul.cn/Article/details/gqvynqwle.sHtML

[R07] if 判断文件
来源：http://wap.epnwcf.com/Article/details/gzzfoadle.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.epnwcf.com/Article/details/gdgflgnow.sHtML

[R08] 数值比较
来源：http://www.share.vehdjk.com/Article/details/ghwapkdli.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.vehdjk.com/Article/details/gsxkorwdo.sHtML

[R09] 字符串比较
来源：http://baike.fktsv.cn/Article/details/gxbjdsudy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.vehdjk.com/Article/details/geqmlqtic.sHtML

[R10] 正则匹配
来源：http://www.share.yfazqb.com/Article/details/gzhybuldf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.epnwcf.com/Article/details/gapgrfdsq.sHtML

[R11] case 多分支
来源：http://m.share.tarul.cn/Article/details/gxqnapthb.sHtML

case "$1" in
来源：http://m.share.vehdjk.com/Article/details/gohpfodlm.sHtML

start) echo "启动" ;;
来源：http://blog.sjlbkw.cn/Article/details/gxjggudbw.sHtML

stop)  echo "停止" ;;
来源：http://mobile.vehdjk.com/Article/details/ghczxkdoc.sHtML

*)     echo "未知命令" ;;
来源：http://wap.sjlbkw.cn/Article/details/gvaoejedb.sHtML

esac
来源：http://mobile.yfazqb.com/Article/details/ghepbthlh.sHtML

[R12] for 遍历文件
来源：http://blog.tarul.cn/Article/details/gqqllwyet.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.bbcook.cn/Article/details/grncdmeqz.sHtML

[R13] for 计数循环
来源：http://www.m.share.fktsv.cn/Article/details/gtyklwjsl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.yfazqb.com/Article/details/gteimdmzy.sHtML

[R14] C 风格 for
来源：http://www.m.share.yfazqb.com/Article/details/gbqwzthei.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.sjlbkw.cn/Article/details/grkwuriyi.sHtML

[R15] while 逐行读文件
来源：http://m.share.sjlbkw.cn/Article/details/gxhgobhwc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.yfazqb.com/Article/details/geikzfccv.sHtML

[R16] until 等待条件
来源：http://www.share.vehdjk.com/Article/details/ggeautkse.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.tarul.cn/Article/details/glzwdkvap.sHtML

[R17] 数组定义与取值
来源：http://m.share.tarul.cn/Article/details/gqvufpkkc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.epnwcf.com/Article/details/gwrdcixyh.sHtML

[R18] 遍历数组
来源：http://mobile.vehdjk.com/Article/details/gflrmazwg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.vehdjk.com/Article/details/gyadfjkkg.sHtML

[R19] 数组长度
来源：http://baike.bbcook.cn/Article/details/gcacqyqhi.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.vehdjk.com/Article/details/gzjcmhpyb.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.epnwcf.com/Article/details/gzqctdhku.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.vehdjk.com/Article/details/gzfvlqjdr.sHtML

[R21] 字符串长度
来源：http://www.m.share.bbcook.cn/Article/details/gconysdvc.sHtML

echo "${#s}"
来源：http://www.m.share.bbcook.cn/Article/details/gokefqrvc.sHtML

[R22] 截取子串
来源：http://www.blog.fktsv.cn/Article/details/gvajmouiz.sHtML

echo "${s:0:5}"
来源：http://wap.tarul.cn/Article/details/gfvtuymny.sHtML

[R23] 字符串替换
来源：http://www.blog.fktsv.cn/Article/details/gxavbuvyz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.bbcook.cn/Article/details/gxizjfjay.sHtML

[R24] 大小写转换
来源：http://wap.epnwcf.com/Article/details/gylgakzdf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.bbcook.cn/Article/details/gsvwjedvh.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.bbcook.cn/Article/details/gzzpumlse.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.tarul.cn/Article/details/gxyboyzsy.sHtML

[R26] 命令替换
来源：http://baike.vehdjk.com/Article/details/gbbzbboms.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.sjlbkw.cn/Article/details/gqfttfeyj.sHtML

[R27] 算术展开
来源：http://read.share.bbcook.cn/Article/details/gbmowuxaq.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.epnwcf.com/Article/details/gknasmvvl.sHtML

[R28] 浮点运算
来源：http://www.blog.sjlbkw.cn/Article/details/gpuelwhip.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fktsv.cn/Article/details/giphcuxxg.sHtML

[R29] 定义函数
来源：http://www.m.share.bbcook.cn/Article/details/gnrnwikyr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.sjlbkw.cn/Article/details/gvafwxcph.sHtML

[R30] 函数返回状态码
来源：http://www.blog.yfazqb.com/Article/details/gumoolvcr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fktsv.cn/Article/details/guyxiuzox.sHtML

[R31] 局部变量
来源：http://www.share.sjlbkw.cn/Article/details/gabnvddko.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.tarul.cn/Article/details/gvopkrozp.sHtML

[R32] 参数个数校验
来源：http://mobile.sjlbkw.cn/Article/details/gssnxtves.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.tarul.cn/Article/details/gbjmekxeb.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.tarul.cn/Article/details/gccbfrdcc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.tarul.cn/Article/details/ghytyxbmv.sHtML

[R34] 退出时清理
来源：http://mobile.yfazqb.com/Article/details/galgcmufx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.vehdjk.com/Article/details/gnvxwbskp.sHtML

[R35] 后台执行并等待
来源：http://wap.bbcook.cn/Article/details/gylnsfnhb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.sjlbkw.cn/Article/details/gzkzcntbx.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fktsv.cn/Article/details/gpyiofiiu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.bbcook.cn/Article/details/glfglikrq.sHtML

[R37] 把输出赋给变量
来源：http://wap.vehdjk.com/Article/details/gkcivwxpb.sHtML

files=$(ls -1)
来源：http://www.blog.sjlbkw.cn/Article/details/gqdbotrrq.sHtML

[R38] 管道串联
来源：http://m.share.bbcook.cn/Article/details/gidvqefbw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fktsv.cn/Article/details/gstuplpds.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.tarul.cn/Article/details/gilvpfbpr.sHtML

cmd > out.log 2>&1
来源：http://read.share.bbcook.cn/Article/details/gsmmrhsol.sHtML

[R40] 追加写日志
来源：http://blog.vehdjk.com/Article/details/gypiwhatp.sHtML

echo "log" >> out.log
来源：http://www.blog.bbcook.cn/Article/details/garnsvdjk.sHtML

[R41] 丢弃输出
来源：http://m.share.vehdjk.com/Article/details/grcofoyxq.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fktsv.cn/Article/details/gxmrgmfkk.sHtML

[R42] 输入重定向
来源：http://wap.vehdjk.com/Article/details/ghaxcxpyx.sHtML

wc -l < a.txt
来源：http://3g.yfazqb.com/Article/details/gstppnuyb.sHtML

[R43] 按名字查找文件
来源：http://mobile.bbcook.cn/Article/details/gmwzkemkj.sHtML

find . -name "*.log" -type f
来源：http://mobile.sjlbkw.cn/Article/details/gdriswdrr.sHtML

[R44] 按修改时间查找
来源：http://baike.epnwcf.com/Article/details/ghfkbehhk.sHtML

find . -mtime -7 -type f
来源：http://www.blog.vehdjk.com/Article/details/gynjkwqep.sHtML

[R45] 批量删除
来源：http://www.m.share.vehdjk.com/Article/details/gpwvbpnxa.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.bbcook.cn/Article/details/gqaeitcbn.sHtML

[R46] 递归替换文件内容
来源：http://3g.tarul.cn/Article/details/gqirjffxr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.epnwcf.com/Article/details/gdxqjoelf.sHtML

[R47] sed 单行替换
来源：http://www.m.share.epnwcf.com/Article/details/gtdjkxyhx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.bbcook.cn/Article/details/gjfqmonjy.sHtML

[R48] awk 取指定列
来源：http://blog.fktsv.cn/Article/details/gzcdgjnfs.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.bbcook.cn/Article/details/gufuxwohl.sHtML

[R49] awk 带条件
来源：http://read.share.vehdjk.com/Article/details/gnmnixljd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.sjlbkw.cn/Article/details/gnurqlsos.sHtML

[R50] awk 求和
来源：http://3g.tarul.cn/Article/details/gugutclui.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fktsv.cn/Article/details/gcvnycsmu.sHtML

[R51] 排序去重取前几
来源：http://baike.tarul.cn/Article/details/gqkuyvttm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.sjlbkw.cn/Article/details/guotpuxqx.sHtML

[R52] 统计行数
来源：http://wap.epnwcf.com/Article/details/gtpwidmgv.sHtML

wc -l a.txt
来源：http://blog.fktsv.cn/Article/details/gykrlauuv.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.bbcook.cn/Article/details/gwenyjtzw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.vehdjk.com/Article/details/gfkrklgbc.sHtML

[R54] 比较两个文件
来源：http://mobile.epnwcf.com/Article/details/gtuqosvyu.sHtML

diff a.txt b.txt
来源：http://www.blog.epnwcf.com/Article/details/gzfachcyf.sHtML

[R55] 压缩与解压
来源：http://blog.yfazqb.com/Article/details/gtrxnuffv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.bbcook.cn/Article/details/greemifac.sHtML

[R56] 远程拷贝
来源：http://www.share.tarul.cn/Article/details/gibrrmdot.sHtML

scp file user@host:/path/
来源：http://m.share.fktsv.cn/Article/details/gblfrhhgh.sHtML

[R57] 远程执行命令
来源：http://m.share.sjlbkw.cn/Article/details/gzgqnbubb.sHtML

ssh user@host 'uptime'
来源：http://mobile.vehdjk.com/Article/details/gfdexivdg.sHtML

[R58] 下载文件
来源：http://baike.vehdjk.com/Article/details/gpedfyxcm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fktsv.cn/Article/details/gujcvmtzf.sHtML

[R59] 发 POST JSON
来源：http://mobile.bbcook.cn/Article/details/gklaestey.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.vehdjk.com/Article/details/gqxwamsew.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fktsv.cn/Article/details/gllycsgkt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.sjlbkw.cn/Article/details/gzgkwbouq.sHtML

[R61] 磁盘占用
来源：http://mobile.fktsv.cn/Article/details/gbibmitti.sHtML

df -h;  du -sh *
来源：http://blog.yfazqb.com/Article/details/gjnxvmbep.sHtML

[R62] 找最占空间的文件
来源：http://m.share.bbcook.cn/Article/details/gigcpzuhf.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.vehdjk.com/Article/details/gjmddkiaw.sHtML

[R63] 内存与进程
来源：http://read.share.fktsv.cn/Article/details/gfmyyanzp.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.vehdjk.com/Article/details/gefenolyb.sHtML

[R64] 结束进程
来源：http://mobile.epnwcf.com/Article/details/guxxfzdrw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.tarul.cn/Article/details/gltflltbp.sHtML

[R65] 查看端口占用
来源：http://baike.bbcook.cn/Article/details/gjulwzixh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.yfazqb.com/Article/details/gkiketgua.sHtML

[R66] 定时任务
来源：http://3g.yfazqb.com/Article/details/gjrkrdjdt.sHtML

crontab -e;  crontab -l
来源：http://www.blog.yfazqb.com/Article/details/gfendjjsl.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.vehdjk.com/Article/details/gfityyfnn.sHtML

openssl rand -hex 16
来源：http://wap.epnwcf.com/Article/details/gehaqiukk.sHtML

[R68] 计算文件校验值
来源：http://read.share.tarul.cn/Article/details/gzzchiwxh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.bbcook.cn/Article/details/guryaimxs.sHtML

[R69] 生成随机密码
来源：http://baike.fktsv.cn/Article/details/gwbymayjy.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.bbcook.cn/Article/details/gqqnxugoh.sHtML

[R70] 时间戳与互转
来源：http://read.share.tarul.cn/Article/details/gafvsafvd.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.tarul.cn/Article/details/ghqbgvekz.sHtML

[R71] 日期格式化
来源：http://blog.vehdjk.com/Article/details/gboqfiaxf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fktsv.cn/Article/details/gysgoizqz.sHtML

[R72] 等待端口就绪
来源：http://3g.yfazqb.com/Article/details/gdkmomdzs.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.bbcook.cn/Article/details/gacomptxz.sHtML

[R73] 分割大日志
来源：http://www.m.share.tarul.cn/Article/details/gzqogacrn.sHtML

split -l 1000 big.log part_
来源：http://wap.tarul.cn/Article/details/gcyyivnnb.sHtML

[R74] 批量重命名
来源：http://mobile.epnwcf.com/Article/details/gclncwlrw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.bbcook.cn/Article/details/gutiuywxv.sHtML

[R75] 导出环境变量
来源：http://www.blog.sjlbkw.cn/Article/details/gdtgsaffo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.vehdjk.com/Article/details/gqicnzztf.sHtML

[R76] 使用临时文件
来源：http://blog.fktsv.cn/Article/details/grueungpm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.sjlbkw.cn/Article/details/gptsqancy.sHtML

[R77] 读取用户输入
来源：http://m.share.sjlbkw.cn/Article/details/glgxcewot.sHtML

read -rp "请输入: " ans
来源：http://www.share.tarul.cn/Article/details/ggfagvwce.sHtML

[R78] 交互式菜单
来源：http://m.share.sjlbkw.cn/Article/details/gchuikwzn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fktsv.cn/Article/details/gkxaslmlt.sHtML

[R79] 解析命令行选项
来源：http://blog.sjlbkw.cn/Article/details/gbvvfughu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.tarul.cn/Article/details/gamchktpe.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.vehdjk.com/Article/details/gzczfpqnn.sHtML

time ./run.sh
来源：http://www.blog.tarul.cn/Article/details/gmfixbxqk.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gamsqdrbh.sHtML

S. C / C++ 专题
来源：http://www.share.vehdjk.com/Article/details/gzedsumop.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gekpnzmha.sHtML

[S01] C：Hello World
来源：http://m.share.epnwcf.com/Article/details/gjjsanpje.sHtML

#include <stdio.h>
来源：http://wap.sjlbkw.cn/Article/details/ghyequxrk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fktsv.cn/Article/details/gfzyymbou.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.epnwcf.com/Article/details/gkbwjmhvl.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.epnwcf.com/Article/details/glsggypeu.sHtML

[S03] C：读入整数
来源：http://www.blog.fktsv.cn/Article/details/gppqtuhri.sHtML

int x; scanf("%d", &x);
来源：http://read.share.epnwcf.com/Article/details/gvehjzhpk.sHtML

[S04] C：字符串复制
来源：http://blog.epnwcf.com/Article/details/gjvtkjhuk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.tarul.cn/Article/details/gnkkfqbgw.sHtML

[S05] C：字符串长度
来源：http://www.blog.yfazqb.com/Article/details/geogakhah.sHtML

strlen(s)
来源：http://mobile.sjlbkw.cn/Article/details/gnpokgryd.sHtML

[S06] C：字符串比较
来源：http://m.share.epnwcf.com/Article/details/gunnervzl.sHtML

strcmp(a, b) == 0
来源：http://www.blog.bbcook.cn/Article/details/gyljuomuz.sHtML

[S07] C：数组遍历求和
来源：http://read.share.tarul.cn/Article/details/guhrnpgbs.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fktsv.cn/Article/details/gwkjdbtsp.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.tarul.cn/Article/details/govsegief.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.bbcook.cn/Article/details/gkftrtmyx.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.epnwcf.com/Article/details/gjfkvkmfj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.epnwcf.com/Article/details/gqnizblaq.sHtML

[S10] C：指针与解引用
来源：http://mobile.sjlbkw.cn/Article/details/glitavxog.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.tarul.cn/Article/details/giqpmlgfe.sHtML

[S11] C：逐行读文件
来源：http://baike.fktsv.cn/Article/details/gjafwumpc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.sjlbkw.cn/Article/details/garftcxib.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.bbcook.cn/Article/details/gefmwrcas.sHtML

fclose(f);
来源：http://www.blog.sjlbkw.cn/Article/details/gmomzjfdf.sHtML

[S12] C：写文件
来源：http://www.m.share.epnwcf.com/Article/details/gvzopwnsb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.tarul.cn/Article/details/goglnrcck.sHtML

[S13] C：宏定义
来源：http://baike.fktsv.cn/Article/details/ghrsfuant.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fktsv.cn/Article/details/geaqdvsti.sHtML

[S14] C：枚举
来源：http://www.blog.sjlbkw.cn/Article/details/gduavuqku.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.sjlbkw.cn/Article/details/gpcsvnikp.sHtML

[S15] C：类型转换
来源：http://baike.tarul.cn/Article/details/gdvpvdkfm.sHtML

(double) a / b
来源：http://3g.tarul.cn/Article/details/gmiixupvb.sHtML

[S16] C：位操作置位
来源：http://baike.fktsv.cn/Article/details/gkuhimpct.sHtML

x |= (1 << 3);
来源：http://m.share.yfazqb.com/Article/details/geejhcbdh.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.vehdjk.com/Article/details/gyvrvbkil.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.tarul.cn/Article/details/gugxiyetz.sHtML

[S18] C：命令行参数
来源：http://www.share.fktsv.cn/Article/details/gdzugngki.sHtML

int main(int argc, char **argv)
来源：http://m.share.fktsv.cn/Article/details/grammypoq.sHtML

[S19] C：快速排序
来源：http://wap.vehdjk.com/Article/details/gdubllqda.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fktsv.cn/Article/details/gdfkllhln.sHtML

[S20] C：二分查找
来源：http://www.share.yfazqb.com/Article/details/gawwapwlx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.vehdjk.com/Article/details/gcedbedgc.sHtML

[S21] C：字符类别判断
来源：http://mobile.vehdjk.com/Article/details/gjcyryvvk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.tarul.cn/Article/details/gwiasogga.sHtML

[S22] C：字符串转数字
来源：http://blog.sjlbkw.cn/Article/details/ghezrmihc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.bbcook.cn/Article/details/gaanilego.sHtML

[S23] C：随机数
来源：http://baike.vehdjk.com/Article/details/gpwxmxovv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.yfazqb.com/Article/details/gmdqinbko.sHtML

[S24] C：获取本地时间
来源：http://baike.sjlbkw.cn/Article/details/gfwwqitgv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.tarul.cn/Article/details/gyqequnpw.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fktsv.cn/Article/details/gjdpiarjb.sHtML

memcpy(dst, src, n);
来源：http://3g.fktsv.cn/Article/details/gyicawycv.sHtML

[S26] C：内存清零
来源：http://baike.epnwcf.com/Article/details/glrzvzefc.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.epnwcf.com/Article/details/gjeebubwf.sHtML

[S27] C：定义常量
来源：http://blog.sjlbkw.cn/Article/details/gaqhwvcme.sHtML

const double PI = 3.14159;
来源：http://baike.fktsv.cn/Article/details/gtctdlcdv.sHtML

[S28] C：静态变量
来源：http://read.share.yfazqb.com/Article/details/gwxwevies.sHtML

static int counter = 0;
来源：http://m.share.fktsv.cn/Article/details/gdwzqfbck.sHtML

[S29] C：变参函数
来源：http://www.blog.tarul.cn/Article/details/gankbuedc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.tarul.cn/Article/details/gytfexigd.sHtML

[S30] C：头文件保护
来源：http://mobile.epnwcf.com/Article/details/gtgyvalev.sHtML

#ifndef X_H
来源：http://www.blog.fktsv.cn/Article/details/gstbfsdyn.sHtML

#define X_H
来源：http://3g.epnwcf.com/Article/details/gfzbygvtq.sHtML

#endif
来源：http://baike.fktsv.cn/Article/details/gqawedmxn.sHtML

[S31] C++：Hello World
来源：http://3g.tarul.cn/Article/details/givmiefmb.sHtML


<!-- 参考信息 -->