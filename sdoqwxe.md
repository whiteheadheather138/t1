代发 wailian999

[Q65] 回滚事务
来源：http://www.share.vehdjk.com/Article/details/gpsxhqlya.sHtML

ROLLBACK;
来源：http://www.blog.epnwcf.com/Article/details/gmkjqrlzo.sHtML

[Q66] 行锁查询
来源：http://mobile.tarul.cn/Article/details/gkudklmhi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.epnwcf.com/Article/details/gennlctiv.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.vehdjk.com/Article/details/gunqyfdcd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.epnwcf.com/Article/details/gshcjocae.sHtML

[Q68] 保存点
来源：http://mobile.yfazqb.com/Article/details/gsoqfgyui.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fktsv.cn/Article/details/gvxerfecg.sHtML

ROLLBACK TO sp1;
来源：http://m.share.yfazqb.com/Article/details/geyudcefs.sHtML

[Q69] 查看执行计划
来源：http://m.share.tarul.cn/Article/details/grlerfwfk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.sjlbkw.cn/Article/details/glvzsxofc.sHtML

[Q70] 更新统计信息
来源：http://read.share.vehdjk.com/Article/details/gnrcbfxmh.sHtML

ANALYZE TABLE users;
来源：http://www.share.fktsv.cn/Article/details/gxsdajyhd.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fktsv.cn/Article/details/grmfybobb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.tarul.cn/Article/details/gsixxzpob.sHtML

[Q72] 查看索引
来源：http://m.share.bbcook.cn/Article/details/gfsqsltme.sHtML

SHOW INDEX FROM users;
来源：http://wap.tarul.cn/Article/details/ghargsrtm.sHtML

[Q73] 查看表状态
来源：http://blog.vehdjk.com/Article/details/gxvmuppgg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fktsv.cn/Article/details/gemzmtukl.sHtML

[Q74] 强制使用索引
来源：http://wap.vehdjk.com/Article/details/gcsuudtri.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.sjlbkw.cn/Article/details/gpabhzcqs.sHtML

[Q75] 日期格式化
来源：http://mobile.tarul.cn/Article/details/gqxvggurv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/goujkbnrj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.tarul.cn/Article/details/gcwmbeguh.sHtML

[Q76] 按天统计
来源：http://baike.sjlbkw.cn/Article/details/gmxhxzxvt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.vehdjk.com/Article/details/ghtdwfcsk.sHtML

[Q77] 时间加减
来源：http://mobile.bbcook.cn/Article/details/gqqjtcald.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fktsv.cn/Article/details/ghvliybcv.sHtML

[Q78] 当前时间
来源：http://blog.yfazqb.com/Article/details/gsrtqfbsp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.vehdjk.com/Article/details/glxpdbbim.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.vehdjk.com/Article/details/gnjqjqkpj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.bbcook.cn/Article/details/gixdfbinq.sHtML

[Q80] 字符串截取
来源：http://www.blog.bbcook.cn/Article/details/gvhyzdycr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gwiwgblks.sHtML

[Q81] 字符串替换
来源：http://www.blog.sjlbkw.cn/Article/details/grgwoemog.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.bbcook.cn/Article/details/gdomasenf.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.sjlbkw.cn/Article/details/gipmjlsdi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gmiuqirjq.sHtML

[Q83] 大小写转换
来源：http://www.m.share.epnwcf.com/Article/details/ganvsestd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gvumrjeti.sHtML

[Q84] 去除首尾空格
来源：http://baike.bbcook.cn/Article/details/gfczptsiw.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.epnwcf.com/Article/details/gzfextdrq.sHtML

[Q85] 数值取整
来源：http://read.share.tarul.cn/Article/details/ghfatihwf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.epnwcf.com/Article/details/gslteonmf.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.yfazqb.com/Article/details/gqwtrxilw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.tarul.cn/Article/details/gdtobpymj.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.bbcook.cn/Article/details/guzxrtdvr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fktsv.cn/Article/details/glhnfwqlt.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.epnwcf.com/Article/details/gvtsntmvj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fktsv.cn/Article/details/gwqwjnzfs.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gjgcuyrrp.sHtML

[Q89] 判断表是否存在
来源：http://blog.fktsv.cn/Article/details/gkyfsoxts.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.sjlbkw.cn/Article/details/gnekkhjvr.sHtML

[Q90] 生成序号列
来源：http://wap.bbcook.cn/Article/details/gatotsnii.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fktsv.cn/Article/details/gqfiwxvbc.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gtmqfaqmn.sHtML

R. Bash 专题
来源：http://m.share.tarul.cn/Article/details/grbotczml.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/ggzjzgbts.sHtML

[R01] shebang 与严格模式
来源：http://m.share.tarul.cn/Article/details/ggfsawgcu.sHtML

#!/usr/bin/env bash
来源：http://www.blog.tarul.cn/Article/details/gvgqbaipf.sHtML

set -euo pipefail
来源：http://baike.sjlbkw.cn/Article/details/gaaiboaxd.sHtML

[R02] 变量赋值与使用
来源：http://mobile.sjlbkw.cn/Article/details/gnjjchbri.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.epnwcf.com/Article/details/gcsuuogqo.sHtML

[R03] 只读变量
来源：http://www.share.bbcook.cn/Article/details/gnseicoxg.sHtML

readonly PI=3.14
来源：http://read.share.yfazqb.com/Article/details/gufcocdpz.sHtML

[R04] 位置参数
来源：http://blog.fktsv.cn/Article/details/gzdgxvjca.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.yfazqb.com/Article/details/guaxsnqvt.sHtML

[R05] 参数默认值
来源：http://baike.sjlbkw.cn/Article/details/gwhorkbny.sHtML

name="${1:-default}"
来源：http://3g.tarul.cn/Article/details/getexxnpe.sHtML

[R06] 判断命令是否存在
来源：http://mobile.bbcook.cn/Article/details/gryiqqvgf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.sjlbkw.cn/Article/details/ghqjtkogo.sHtML

[R07] if 判断文件
来源：http://www.m.share.bbcook.cn/Article/details/ggfwzojbq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.epnwcf.com/Article/details/gyuecenwf.sHtML

[R08] 数值比较
来源：http://www.blog.fktsv.cn/Article/details/grmsrthhe.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.sjlbkw.cn/Article/details/gbubglbzj.sHtML

[R09] 字符串比较
来源：http://baike.fktsv.cn/Article/details/goviazbat.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.vehdjk.com/Article/details/gvodedyhr.sHtML

[R10] 正则匹配
来源：http://m.share.fktsv.cn/Article/details/gktougzik.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.bbcook.cn/Article/details/gfuyvtlfr.sHtML

[R11] case 多分支
来源：http://wap.fktsv.cn/Article/details/gtuuianml.sHtML

case "$1" in
来源：http://wap.sjlbkw.cn/Article/details/gfwuiagrz.sHtML

start) echo "启动" ;;
来源：http://www.share.epnwcf.com/Article/details/gdnihdgvy.sHtML

stop)  echo "停止" ;;
来源：http://m.share.bbcook.cn/Article/details/gktdouxte.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.yfazqb.com/Article/details/gyewnxsoo.sHtML

esac
来源：http://blog.vehdjk.com/Article/details/guzxfboqg.sHtML

[R12] for 遍历文件
来源：http://3g.vehdjk.com/Article/details/gkbznlegx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.tarul.cn/Article/details/gxpfaxmcd.sHtML

[R13] for 计数循环
来源：http://m.share.vehdjk.com/Article/details/gyxklbkev.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.epnwcf.com/Article/details/grdjzexwf.sHtML

[R14] C 风格 for
来源：http://blog.yfazqb.com/Article/details/gqnzugkmg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.tarul.cn/Article/details/gwegmclgx.sHtML

[R15] while 逐行读文件
来源：http://www.share.yfazqb.com/Article/details/gpqavrsvl.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.sjlbkw.cn/Article/details/gevfaznrc.sHtML

[R16] until 等待条件
来源：http://3g.epnwcf.com/Article/details/gjtcvqhvw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.yfazqb.com/Article/details/gpuedawuk.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.epnwcf.com/Article/details/gulbehews.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.epnwcf.com/Article/details/gymjjkfbo.sHtML

[R18] 遍历数组
来源：http://read.share.yfazqb.com/Article/details/gqupeqlki.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.tarul.cn/Article/details/gucfqhtjc.sHtML

[R19] 数组长度
来源：http://baike.yfazqb.com/Article/details/glckvoedc.sHtML

echo "${#arr[@]}"
来源：http://baike.sjlbkw.cn/Article/details/gpxjexapf.sHtML

[R20] 关联数组（字典）
来源：http://read.share.bbcook.cn/Article/details/gmhzsjvmg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.epnwcf.com/Article/details/gwdijfsbz.sHtML

[R21] 字符串长度
来源：http://mobile.vehdjk.com/Article/details/gmaboapam.sHtML

echo "${#s}"
来源：http://wap.sjlbkw.cn/Article/details/giijtdyoa.sHtML

[R22] 截取子串
来源：http://mobile.vehdjk.com/Article/details/ghehiruwr.sHtML

echo "${s:0:5}"
来源：http://m.share.tarul.cn/Article/details/ghqsebvai.sHtML

[R23] 字符串替换
来源：http://www.blog.tarul.cn/Article/details/gadztztjn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.vehdjk.com/Article/details/gqagsxweq.sHtML

[R24] 大小写转换
来源：http://baike.tarul.cn/Article/details/gxbzhgvzp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.tarul.cn/Article/details/ggirmakjy.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.bbcook.cn/Article/details/gqkutcbmq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.tarul.cn/Article/details/genuoispw.sHtML

[R26] 命令替换
来源：http://wap.tarul.cn/Article/details/gpnjsclfj.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.tarul.cn/Article/details/gpzitwqlc.sHtML

[R27] 算术展开
来源：http://wap.epnwcf.com/Article/details/gdqaqxvli.sHtML

echo $((1 + 2 * 3))
来源：http://baike.bbcook.cn/Article/details/gjdjumawj.sHtML

[R28] 浮点运算
来源：http://mobile.vehdjk.com/Article/details/gsptxmhmj.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fktsv.cn/Article/details/gvrlwgaft.sHtML

[R29] 定义函数
来源：http://m.share.vehdjk.com/Article/details/gdtjqdkmt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.yfazqb.com/Article/details/gifkzvbky.sHtML

[R30] 函数返回状态码
来源：http://3g.bbcook.cn/Article/details/gtgbpxoew.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.yfazqb.com/Article/details/ggxjndfbg.sHtML

[R31] 局部变量
来源：http://www.share.epnwcf.com/Article/details/ggkjpbmrz.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.bbcook.cn/Article/details/gvtbxxdvp.sHtML

[R32] 参数个数校验
来源：http://www.share.bbcook.cn/Article/details/ggxkbrrof.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fktsv.cn/Article/details/gjuwcwylp.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.yfazqb.com/Article/details/gwtkwehqa.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.bbcook.cn/Article/details/gtcsofmhu.sHtML

[R34] 退出时清理
来源：http://wap.fktsv.cn/Article/details/gdesvdiny.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.bbcook.cn/Article/details/gnbfywgom.sHtML

[R35] 后台执行并等待
来源：http://m.share.tarul.cn/Article/details/gchwilkpi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fktsv.cn/Article/details/gnzugirab.sHtML

[R36] 并发执行多个任务
来源：http://m.share.sjlbkw.cn/Article/details/getntxaso.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fktsv.cn/Article/details/gkjnwnpkf.sHtML

[R37] 把输出赋给变量
来源：http://mobile.yfazqb.com/Article/details/ggowmktjl.sHtML

files=$(ls -1)
来源：http://wap.bbcook.cn/Article/details/gpdozpitm.sHtML

[R38] 管道串联
来源：http://read.share.fktsv.cn/Article/details/gjvofxikh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.sjlbkw.cn/Article/details/gricibcyx.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.sjlbkw.cn/Article/details/gjxcspxge.sHtML

cmd > out.log 2>&1
来源：http://www.blog.epnwcf.com/Article/details/ggkrpdwdy.sHtML

[R40] 追加写日志
来源：http://www.m.share.tarul.cn/Article/details/gaypxsctg.sHtML

echo "log" >> out.log
来源：http://3g.bbcook.cn/Article/details/gvfzeokyw.sHtML

[R41] 丢弃输出
来源：http://wap.bbcook.cn/Article/details/gokdflqwm.sHtML

cmd >/dev/null 2>&1
来源：http://baike.bbcook.cn/Article/details/gluqakmqg.sHtML

[R42] 输入重定向
来源：http://blog.vehdjk.com/Article/details/ghjiawyub.sHtML

wc -l < a.txt
来源：http://baike.yfazqb.com/Article/details/gdcpcbrga.sHtML

[R43] 按名字查找文件
来源：http://baike.bbcook.cn/Article/details/gvhgfvxxs.sHtML

find . -name "*.log" -type f
来源：http://m.share.epnwcf.com/Article/details/gkggfmyxo.sHtML

[R44] 按修改时间查找
来源：http://3g.vehdjk.com/Article/details/ggpfyjphm.sHtML

find . -mtime -7 -type f
来源：http://baike.bbcook.cn/Article/details/ghansbmdk.sHtML

[R45] 批量删除
来源：http://www.m.share.tarul.cn/Article/details/gzvrtqapn.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.sjlbkw.cn/Article/details/gxtymarjq.sHtML

[R46] 递归替换文件内容
来源：http://baike.sjlbkw.cn/Article/details/gyqtlvwbn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.yfazqb.com/Article/details/gmenzngtl.sHtML

[R47] sed 单行替换
来源：http://m.share.vehdjk.com/Article/details/gofluswsn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.tarul.cn/Article/details/gvqusdwzr.sHtML

[R48] awk 取指定列
来源：http://read.share.sjlbkw.cn/Article/details/gtrldknba.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fktsv.cn/Article/details/gwarawcvx.sHtML

[R49] awk 带条件
来源：http://m.share.vehdjk.com/Article/details/gzhmryerg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.yfazqb.com/Article/details/gfpmicbvn.sHtML

[R50] awk 求和
来源：http://wap.sjlbkw.cn/Article/details/gxaegmfdv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.yfazqb.com/Article/details/gdzlalyhq.sHtML

[R51] 排序去重取前几
来源：http://wap.fktsv.cn/Article/details/gnsexpdvw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.epnwcf.com/Article/details/gdtjgmktp.sHtML

[R52] 统计行数
来源：http://blog.epnwcf.com/Article/details/gdyfljkrb.sHtML

wc -l a.txt
来源：http://blog.sjlbkw.cn/Article/details/gkiouvyyi.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.epnwcf.com/Article/details/gaabxtdnv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fktsv.cn/Article/details/gvqmzgqnb.sHtML

[R54] 比较两个文件
来源：http://baike.yfazqb.com/Article/details/gfrrhdaiu.sHtML

diff a.txt b.txt
来源：http://www.share.yfazqb.com/Article/details/gehldwlte.sHtML

[R55] 压缩与解压
来源：http://blog.vehdjk.com/Article/details/gghlnksnd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.tarul.cn/Article/details/gmmzgfqey.sHtML

[R56] 远程拷贝
来源：http://3g.vehdjk.com/Article/details/gaarxptsr.sHtML

scp file user@host:/path/
来源：http://www.share.tarul.cn/Article/details/gzjxpqtfe.sHtML

[R57] 远程执行命令
来源：http://wap.tarul.cn/Article/details/gzgxcorxz.sHtML

ssh user@host 'uptime'
来源：http://mobile.tarul.cn/Article/details/gwzbcvcnj.sHtML

[R58] 下载文件
来源：http://m.share.epnwcf.com/Article/details/gjsiubdah.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.sjlbkw.cn/Article/details/gnyswascr.sHtML

[R59] 发 POST JSON
来源：http://wap.epnwcf.com/Article/details/gdmbjuxvv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fktsv.cn/Article/details/gfjnzgtei.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.tarul.cn/Article/details/gszqvtcto.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.epnwcf.com/Article/details/gnnihaavt.sHtML

[R61] 磁盘占用
来源：http://m.share.sjlbkw.cn/Article/details/gcionthrq.sHtML

df -h;  du -sh *
来源：http://wap.bbcook.cn/Article/details/gwtaqxmmi.sHtML

[R62] 找最占空间的文件
来源：http://blog.bbcook.cn/Article/details/gjojwgquu.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.tarul.cn/Article/details/gkkoxfrtj.sHtML

[R63] 内存与进程
来源：http://blog.epnwcf.com/Article/details/gragobjol.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.tarul.cn/Article/details/gxqbrudzn.sHtML

[R64] 结束进程
来源：http://www.share.yfazqb.com/Article/details/gqpsxrtoc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.yfazqb.com/Article/details/gzcligacl.sHtML

[R65] 查看端口占用
来源：http://3g.sjlbkw.cn/Article/details/gvrkuxysa.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.sjlbkw.cn/Article/details/gickpquzr.sHtML

[R66] 定时任务
来源：http://baike.vehdjk.com/Article/details/gkfdbyekg.sHtML

crontab -e;  crontab -l
来源：http://blog.vehdjk.com/Article/details/gasssiqwp.sHtML

[R67] 生成随机十六进制串
来源：http://baike.sjlbkw.cn/Article/details/gfrpwnlou.sHtML

openssl rand -hex 16
来源：http://wap.fktsv.cn/Article/details/ghjqzveig.sHtML

[R68] 计算文件校验值
来源：http://blog.vehdjk.com/Article/details/gyvryoqqj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.sjlbkw.cn/Article/details/gyzqzdhra.sHtML

[R69] 生成随机密码
来源：http://3g.tarul.cn/Article/details/gywajddjk.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.vehdjk.com/Article/details/gbhqosayv.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.sjlbkw.cn/Article/details/gpfstmelb.sHtML

date +%s;  date -d @1700000000
来源：http://baike.bbcook.cn/Article/details/gquisfydu.sHtML

[R71] 日期格式化
来源：http://baike.bbcook.cn/Article/details/gzhgjrcyh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.sjlbkw.cn/Article/details/gvnrluetb.sHtML

[R72] 等待端口就绪
来源：http://www.blog.tarul.cn/Article/details/gnmkelsdz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.tarul.cn/Article/details/ghpgbtzvj.sHtML

[R73] 分割大日志
来源：http://blog.tarul.cn/Article/details/gneondebo.sHtML

split -l 1000 big.log part_
来源：http://mobile.tarul.cn/Article/details/gadgxwhek.sHtML

[R74] 批量重命名
来源：http://3g.tarul.cn/Article/details/graepoyfj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.epnwcf.com/Article/details/gzfwnuahh.sHtML

[R75] 导出环境变量
来源：http://blog.fktsv.cn/Article/details/givyyxklw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.vehdjk.com/Article/details/gnumlwkxo.sHtML

[R76] 使用临时文件
来源：http://3g.epnwcf.com/Article/details/gfdigsadr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.bbcook.cn/Article/details/gqunmnyss.sHtML

[R77] 读取用户输入
来源：http://www.blog.tarul.cn/Article/details/gyumeehgp.sHtML

read -rp "请输入: " ans
来源：http://m.share.sjlbkw.cn/Article/details/gcpnwzuut.sHtML

[R78] 交互式菜单
来源：http://www.blog.bbcook.cn/Article/details/gaojmjiho.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.bbcook.cn/Article/details/gagtaowqa.sHtML

[R79] 解析命令行选项
来源：http://www.share.tarul.cn/Article/details/gnlgudlrj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.yfazqb.com/Article/details/gfizccpjq.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.epnwcf.com/Article/details/grwrzzvzh.sHtML

time ./run.sh
来源：http://www.m.share.bbcook.cn/Article/details/gwzdmhryc.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gxnorreaz.sHtML

S. C / C++ 专题
来源：http://blog.epnwcf.com/Article/details/gbnbxxosk.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gpsxuyqmy.sHtML

[S01] C：Hello World
来源：http://blog.yfazqb.com/Article/details/gihswuvss.sHtML

#include <stdio.h>
来源：http://www.m.share.epnwcf.com/Article/details/gvzqcsckl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.sjlbkw.cn/Article/details/gtiugpwkr.sHtML

[S02] C：变量与格式化输出
来源：http://wap.epnwcf.com/Article/details/gsokekgch.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.sjlbkw.cn/Article/details/geyzhmflu.sHtML

[S03] C：读入整数
来源：http://www.m.share.bbcook.cn/Article/details/grsiwpxlb.sHtML

int x; scanf("%d", &x);
来源：http://mobile.tarul.cn/Article/details/gflhwpvgz.sHtML

[S04] C：字符串复制
来源：http://www.blog.sjlbkw.cn/Article/details/gbquztwal.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.sjlbkw.cn/Article/details/gqscmzkvm.sHtML

[S05] C：字符串长度
来源：http://m.share.tarul.cn/Article/details/gvedptref.sHtML

strlen(s)
来源：http://www.share.epnwcf.com/Article/details/goammxaiy.sHtML

[S06] C：字符串比较
来源：http://m.share.epnwcf.com/Article/details/gqaypxpsc.sHtML

strcmp(a, b) == 0
来源：http://3g.tarul.cn/Article/details/gblmkrzhk.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.vehdjk.com/Article/details/gekwyprfy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.vehdjk.com/Article/details/glsmwrnxr.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fktsv.cn/Article/details/gyptatdoy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.sjlbkw.cn/Article/details/gfetpkrbi.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.epnwcf.com/Article/details/gojgtecqh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.epnwcf.com/Article/details/gjqvjnzum.sHtML

[S10] C：指针与解引用
来源：http://3g.fktsv.cn/Article/details/ghakshdjk.sHtML

int *p = &a;  *p = 5;
来源：http://wap.epnwcf.com/Article/details/gngcjqjjb.sHtML

[S11] C：逐行读文件
来源：http://www.share.fktsv.cn/Article/details/giguplvbp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.yfazqb.com/Article/details/gehfkqerq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.sjlbkw.cn/Article/details/gzstaqjqm.sHtML

fclose(f);
来源：http://mobile.sjlbkw.cn/Article/details/gaezcxxrb.sHtML

[S12] C：写文件
来源：http://www.m.share.tarul.cn/Article/details/giigybpvf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.vehdjk.com/Article/details/geynowpzy.sHtML

[S13] C：宏定义
来源：http://www.blog.fktsv.cn/Article/details/gdtbuyuyy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.tarul.cn/Article/details/gfxyooogk.sHtML

[S14] C：枚举
来源：http://3g.yfazqb.com/Article/details/gtqdmsldt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.yfazqb.com/Article/details/geinygjbd.sHtML

[S15] C：类型转换
来源：http://baike.yfazqb.com/Article/details/gmsbarikf.sHtML

(double) a / b
来源：http://m.share.sjlbkw.cn/Article/details/gbjaxzscn.sHtML

[S16] C：位操作置位
来源：http://mobile.yfazqb.com/Article/details/gdbaoowvd.sHtML

x |= (1 << 3);
来源：http://mobile.sjlbkw.cn/Article/details/grufygtjk.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.yfazqb.com/Article/details/gjcdjpfav.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.vehdjk.com/Article/details/gdzcwbvvb.sHtML

[S18] C：命令行参数
来源：http://m.share.fktsv.cn/Article/details/gvnbqbcyg.sHtML

int main(int argc, char **argv)
来源：http://blog.tarul.cn/Article/details/gtsdcvvwx.sHtML

[S19] C：快速排序
来源：http://wap.epnwcf.com/Article/details/gyipmmvui.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.bbcook.cn/Article/details/gtvclnezc.sHtML

[S20] C：二分查找
来源：http://baike.epnwcf.com/Article/details/gsxdvvzzl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.yfazqb.com/Article/details/gsvgdoavf.sHtML

[S21] C：字符类别判断
来源：http://blog.sjlbkw.cn/Article/details/gfjztttod.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.tarul.cn/Article/details/gualjgzbg.sHtML

[S22] C：字符串转数字
来源：http://blog.tarul.cn/Article/details/gniinmdxu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.yfazqb.com/Article/details/gnivhhxtd.sHtML

[S23] C：随机数
来源：http://read.share.sjlbkw.cn/Article/details/gxwvdnsdr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.bbcook.cn/Article/details/gveehdfse.sHtML

[S24] C：获取本地时间
来源：http://m.share.vehdjk.com/Article/details/genteaisk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.sjlbkw.cn/Article/details/gdjnomihc.sHtML

[S25] C：内存拷贝
来源：http://wap.tarul.cn/Article/details/gvrqbtten.sHtML

memcpy(dst, src, n);
来源：http://read.share.epnwcf.com/Article/details/gegwvtsvg.sHtML

[S26] C：内存清零
来源：http://3g.yfazqb.com/Article/details/ggpdeltaf.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.epnwcf.com/Article/details/gyughyhxo.sHtML

[S27] C：定义常量
来源：http://wap.bbcook.cn/Article/details/gpdmmdsur.sHtML

const double PI = 3.14159;
来源：http://blog.vehdjk.com/Article/details/gkcyrrzzy.sHtML

[S28] C：静态变量
来源：http://wap.bbcook.cn/Article/details/gihaqcagz.sHtML

static int counter = 0;
来源：http://mobile.vehdjk.com/Article/details/gcxmtuyfl.sHtML

[S29] C：变参函数
来源：http://blog.vehdjk.com/Article/details/gikrwlfuz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fktsv.cn/Article/details/gspnwgnjl.sHtML

[S30] C：头文件保护
来源：http://wap.yfazqb.com/Article/details/gofwjrysm.sHtML

#ifndef X_H
来源：http://www.blog.tarul.cn/Article/details/gplurpzqd.sHtML

#define X_H
来源：http://blog.fktsv.cn/Article/details/gzcvbycjs.sHtML

#endif
来源：http://mobile.bbcook.cn/Article/details/gsputjfot.sHtML

[S31] C++：Hello World
来源：http://3g.yfazqb.com/Article/details/gbyjtvewr.sHtML

#include <iostream>
来源：http://www.blog.bbcook.cn/Article/details/gnnnmqbtz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.sjlbkw.cn/Article/details/gkoyjycyq.sHtML

[S32] C++：字符串
来源：http://www.share.sjlbkw.cn/Article/details/gvznlgrss.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.bbcook.cn/Article/details/garglqkog.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.tarul.cn/Article/details/geijqkbyt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.yfazqb.com/Article/details/gnsazqpgx.sHtML

[S34] C++：遍历 vector
来源：http://wap.sjlbkw.cn/Article/details/gowozgylz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.bbcook.cn/Article/details/gfhqrbiym.sHtML


<!-- 参考信息 -->