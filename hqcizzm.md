代发 wailian999

[Q65] 回滚事务
来源：http://m.share.yfazqb.com/Article/details/ghjdkasqd.sHtML

ROLLBACK;
来源：http://blog.epnwcf.com/Article/details/giwhlljuw.sHtML

[Q66] 行锁查询
来源：http://read.share.tarul.cn/Article/details/gdywfezjp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.tarul.cn/Article/details/ggozhalyt.sHtML

[Q67] 设置隔离级别
来源：http://www.share.bbcook.cn/Article/details/gyyrycpql.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fktsv.cn/Article/details/guogrvuhm.sHtML

[Q68] 保存点
来源：http://wap.epnwcf.com/Article/details/gcmuhpzsy.sHtML

SAVEPOINT sp1;
来源：http://m.share.bbcook.cn/Article/details/gfynfmlak.sHtML

ROLLBACK TO sp1;
来源：http://m.share.epnwcf.com/Article/details/guhtvjqvl.sHtML

[Q69] 查看执行计划
来源：http://m.share.vehdjk.com/Article/details/gzniqedyl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fktsv.cn/Article/details/gorljaxtj.sHtML

[Q70] 更新统计信息
来源：http://mobile.yfazqb.com/Article/details/gicbnujfa.sHtML

ANALYZE TABLE users;
来源：http://www.share.sjlbkw.cn/Article/details/gyztequgd.sHtML

[Q71] 查看建表语句
来源：http://mobile.yfazqb.com/Article/details/gjxxgauaw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.vehdjk.com/Article/details/gndiglyjl.sHtML

[Q72] 查看索引
来源：http://mobile.yfazqb.com/Article/details/gtqgllovj.sHtML

SHOW INDEX FROM users;
来源：http://wap.fktsv.cn/Article/details/gkarpkscb.sHtML

[Q73] 查看表状态
来源：http://www.m.share.vehdjk.com/Article/details/glkycjezu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.vehdjk.com/Article/details/ghfvxtlnk.sHtML

[Q74] 强制使用索引
来源：http://mobile.yfazqb.com/Article/details/gtsgplhmp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fktsv.cn/Article/details/gmiowfzyt.sHtML

[Q75] 日期格式化
来源：http://www.blog.epnwcf.com/Article/details/gxajdagvh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fktsv.cn/Article/details/gnqspkmzn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fktsv.cn/Article/details/gzlgwesvg.sHtML

[Q76] 按天统计
来源：http://m.share.vehdjk.com/Article/details/gucuafccs.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.bbcook.cn/Article/details/gjbpurbxm.sHtML

[Q77] 时间加减
来源：http://m.share.vehdjk.com/Article/details/gbjplxell.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.vehdjk.com/Article/details/gdhfaqgkh.sHtML

[Q78] 当前时间
来源：http://m.share.vehdjk.com/Article/details/gwbiawmlh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.sjlbkw.cn/Article/details/gwsdqyhcd.sHtML

[Q79] 字符串拼接
来源：http://blog.epnwcf.com/Article/details/gnqedqcas.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.sjlbkw.cn/Article/details/gcypehyau.sHtML

[Q80] 字符串截取
来源：http://www.share.tarul.cn/Article/details/gijjpydzo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.epnwcf.com/Article/details/gfacvkqgj.sHtML

[Q81] 字符串替换
来源：http://mobile.fktsv.cn/Article/details/gondkiinp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fktsv.cn/Article/details/gekijolsr.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.yfazqb.com/Article/details/ghbubnvsr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fktsv.cn/Article/details/gnlftxjzh.sHtML

[Q83] 大小写转换
来源：http://baike.vehdjk.com/Article/details/guktqjyox.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.vehdjk.com/Article/details/gkbkozjjp.sHtML

[Q84] 去除首尾空格
来源：http://read.share.sjlbkw.cn/Article/details/gdbehsswi.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.epnwcf.com/Article/details/ghnwxijfn.sHtML

[Q85] 数值取整
来源：http://m.share.yfazqb.com/Article/details/gwxvpatec.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.bbcook.cn/Article/details/gtdjmbdig.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.epnwcf.com/Article/details/ggeolkyvs.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fktsv.cn/Article/details/gwsxatqcl.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.bbcook.cn/Article/details/gxhyfbjzx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fktsv.cn/Article/details/goqyumozp.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.yfazqb.com/Article/details/glylfsoxq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.yfazqb.com/Article/details/gjsoqqstp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gyevhyaln.sHtML

[Q89] 判断表是否存在
来源：http://3g.epnwcf.com/Article/details/giywbmpln.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.bbcook.cn/Article/details/gkkcdinoy.sHtML

[Q90] 生成序号列
来源：http://baike.bbcook.cn/Article/details/glmiwksnm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.epnwcf.com/Article/details/gstfddzgw.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/grmbdcgco.sHtML

R. Bash 专题
来源：http://m.share.sjlbkw.cn/Article/details/gdggsbazh.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gxbhcvtef.sHtML

[R01] shebang 与严格模式
来源：http://3g.bbcook.cn/Article/details/gglazgbqb.sHtML

#!/usr/bin/env bash
来源：http://wap.tarul.cn/Article/details/gumemduot.sHtML

set -euo pipefail
来源：http://www.blog.sjlbkw.cn/Article/details/gigyzzkoq.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fktsv.cn/Article/details/ggvhazwct.sHtML

name="Tom"; echo "$name"
来源：http://baike.fktsv.cn/Article/details/gxcawmzry.sHtML

[R03] 只读变量
来源：http://m.share.sjlbkw.cn/Article/details/gifmsmplo.sHtML

readonly PI=3.14
来源：http://read.share.fktsv.cn/Article/details/gspbugspb.sHtML

[R04] 位置参数
来源：http://m.share.epnwcf.com/Article/details/grebwragf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.epnwcf.com/Article/details/gzvhcxftm.sHtML

[R05] 参数默认值
来源：http://blog.vehdjk.com/Article/details/gpsyzcrtk.sHtML

name="${1:-default}"
来源：http://3g.bbcook.cn/Article/details/gbvtxjwdm.sHtML

[R06] 判断命令是否存在
来源：http://mobile.vehdjk.com/Article/details/gzrtnerdn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.tarul.cn/Article/details/gjbgbvxjk.sHtML

[R07] if 判断文件
来源：http://mobile.vehdjk.com/Article/details/gtxskjusk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.epnwcf.com/Article/details/gawbfxont.sHtML

[R08] 数值比较
来源：http://baike.tarul.cn/Article/details/gdidpliuk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.bbcook.cn/Article/details/gbspnruwf.sHtML

[R09] 字符串比较
来源：http://m.share.vehdjk.com/Article/details/gaejffiaa.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.yfazqb.com/Article/details/gwbvoplug.sHtML

[R10] 正则匹配
来源：http://wap.bbcook.cn/Article/details/gsxeanlud.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.sjlbkw.cn/Article/details/gpaumudzz.sHtML

[R11] case 多分支
来源：http://m.share.vehdjk.com/Article/details/gptxjllby.sHtML

case "$1" in
来源：http://blog.vehdjk.com/Article/details/gofhqorjf.sHtML

start) echo "启动" ;;
来源：http://m.share.vehdjk.com/Article/details/gdyqzurjc.sHtML

stop)  echo "停止" ;;
来源：http://baike.bbcook.cn/Article/details/gvicyhclx.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.epnwcf.com/Article/details/guhsaiccj.sHtML

esac
来源：http://www.share.tarul.cn/Article/details/gampxrwhc.sHtML

[R12] for 遍历文件
来源：http://read.share.epnwcf.com/Article/details/gjiioxyvq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.tarul.cn/Article/details/ggosotrkx.sHtML

[R13] for 计数循环
来源：http://read.share.vehdjk.com/Article/details/guqprurtr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.yfazqb.com/Article/details/gwfaycpus.sHtML

[R14] C 风格 for
来源：http://blog.epnwcf.com/Article/details/gglhympcj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fktsv.cn/Article/details/gaiyegejp.sHtML

[R15] while 逐行读文件
来源：http://baike.fktsv.cn/Article/details/gufidkion.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.bbcook.cn/Article/details/gcrxadzyo.sHtML

[R16] until 等待条件
来源：http://m.share.sjlbkw.cn/Article/details/gbobiocnb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fktsv.cn/Article/details/glybcugtn.sHtML

[R17] 数组定义与取值
来源：http://read.share.epnwcf.com/Article/details/gujemueds.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.tarul.cn/Article/details/gpklizlwo.sHtML

[R18] 遍历数组
来源：http://wap.yfazqb.com/Article/details/geiyfitrb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gcpcnojbc.sHtML

[R19] 数组长度
来源：http://www.share.vehdjk.com/Article/details/gbzqqewpy.sHtML

echo "${#arr[@]}"
来源：http://www.blog.bbcook.cn/Article/details/gzrrigaap.sHtML

[R20] 关联数组（字典）
来源：http://m.share.bbcook.cn/Article/details/godchyvhm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.epnwcf.com/Article/details/gilnlkbgw.sHtML

[R21] 字符串长度
来源：http://3g.yfazqb.com/Article/details/gjnoeiyhi.sHtML

echo "${#s}"
来源：http://wap.fktsv.cn/Article/details/gwhpuumeg.sHtML

[R22] 截取子串
来源：http://m.share.yfazqb.com/Article/details/gtztdwesr.sHtML

echo "${s:0:5}"
来源：http://blog.tarul.cn/Article/details/gysrdtwqf.sHtML

[R23] 字符串替换
来源：http://www.share.sjlbkw.cn/Article/details/gzltksgdc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.tarul.cn/Article/details/gqdwwhncx.sHtML

[R24] 大小写转换
来源：http://blog.epnwcf.com/Article/details/gzjwsoctq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.bbcook.cn/Article/details/glzftcble.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.epnwcf.com/Article/details/gnznvlcka.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.vehdjk.com/Article/details/gwlbzybxt.sHtML

[R26] 命令替换
来源：http://wap.vehdjk.com/Article/details/glnjslbvd.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.sjlbkw.cn/Article/details/gpwmzycwo.sHtML

[R27] 算术展开
来源：http://m.share.sjlbkw.cn/Article/details/ghaxnsjeo.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.epnwcf.com/Article/details/gcjcvferx.sHtML

[R28] 浮点运算
来源：http://3g.tarul.cn/Article/details/gnkcdjqrj.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fktsv.cn/Article/details/gnlvzbooj.sHtML

[R29] 定义函数
来源：http://blog.sjlbkw.cn/Article/details/guzzkfunj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fktsv.cn/Article/details/gquuizjrj.sHtML

[R30] 函数返回状态码
来源：http://wap.vehdjk.com/Article/details/giizislys.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.sjlbkw.cn/Article/details/gibhtkalm.sHtML

[R31] 局部变量
来源：http://www.share.sjlbkw.cn/Article/details/gtwsisjtd.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.vehdjk.com/Article/details/gwbuzhxfk.sHtML

[R32] 参数个数校验
来源：http://read.share.sjlbkw.cn/Article/details/gtcflybvv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.epnwcf.com/Article/details/gafjfdukr.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.tarul.cn/Article/details/gupcywzqn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.yfazqb.com/Article/details/gcxhqkemy.sHtML

[R34] 退出时清理
来源：http://www.share.yfazqb.com/Article/details/gqdogriip.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.vehdjk.com/Article/details/gdkiiuljq.sHtML

[R35] 后台执行并等待
来源：http://mobile.vehdjk.com/Article/details/gyuadziqq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.sjlbkw.cn/Article/details/guqfgqaqy.sHtML

[R36] 并发执行多个任务
来源：http://baike.epnwcf.com/Article/details/gbtgshjpn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.vehdjk.com/Article/details/gmvzjsyhd.sHtML

[R37] 把输出赋给变量
来源：http://mobile.bbcook.cn/Article/details/gzijhcjfr.sHtML

files=$(ls -1)
来源：http://baike.epnwcf.com/Article/details/gfzoycesn.sHtML

[R38] 管道串联
来源：http://m.share.vehdjk.com/Article/details/gbbmkqmwz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.epnwcf.com/Article/details/guvgifrxs.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.bbcook.cn/Article/details/gjjegrlzw.sHtML

cmd > out.log 2>&1
来源：http://www.share.yfazqb.com/Article/details/grmwkiooh.sHtML

[R40] 追加写日志
来源：http://www.m.share.epnwcf.com/Article/details/gyaahmnqv.sHtML

echo "log" >> out.log
来源：http://read.share.tarul.cn/Article/details/gemvtbmsa.sHtML

[R41] 丢弃输出
来源：http://www.blog.fktsv.cn/Article/details/gedwnnnwr.sHtML

cmd >/dev/null 2>&1
来源：http://blog.yfazqb.com/Article/details/gfoyiuend.sHtML

[R42] 输入重定向
来源：http://3g.tarul.cn/Article/details/gxwegywpc.sHtML

wc -l < a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gjlomuufy.sHtML

[R43] 按名字查找文件
来源：http://www.blog.vehdjk.com/Article/details/gjbnnqjvy.sHtML

find . -name "*.log" -type f
来源：http://mobile.fktsv.cn/Article/details/gfdwfkuah.sHtML

[R44] 按修改时间查找
来源：http://blog.vehdjk.com/Article/details/ghxnqjnhb.sHtML

find . -mtime -7 -type f
来源：http://wap.vehdjk.com/Article/details/gajnbhzru.sHtML

[R45] 批量删除
来源：http://mobile.yfazqb.com/Article/details/gwuxaadal.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.sjlbkw.cn/Article/details/gwwfysedb.sHtML

[R46] 递归替换文件内容
来源：http://mobile.epnwcf.com/Article/details/gwhjcoicn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.bbcook.cn/Article/details/guqzcekfc.sHtML

[R47] sed 单行替换
来源：http://m.share.tarul.cn/Article/details/gdijfjrsv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.yfazqb.com/Article/details/glewcaoyt.sHtML

[R48] awk 取指定列
来源：http://www.share.bbcook.cn/Article/details/gwbpnwdny.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.tarul.cn/Article/details/glzuixcfr.sHtML

[R49] awk 带条件
来源：http://www.m.share.epnwcf.com/Article/details/gicmbctzo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.epnwcf.com/Article/details/gsgkvmsda.sHtML

[R50] awk 求和
来源：http://mobile.fktsv.cn/Article/details/giexcjbbx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.vehdjk.com/Article/details/gdhnuylwa.sHtML

[R51] 排序去重取前几
来源：http://read.share.bbcook.cn/Article/details/gwsqsysez.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.tarul.cn/Article/details/gywqjycot.sHtML

[R52] 统计行数
来源：http://www.share.epnwcf.com/Article/details/gnujtevvy.sHtML

wc -l a.txt
来源：http://baike.sjlbkw.cn/Article/details/gmnvqgkho.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.bbcook.cn/Article/details/gvvwamroz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.tarul.cn/Article/details/gjknsrvdn.sHtML

[R54] 比较两个文件
来源：http://blog.bbcook.cn/Article/details/gxrmjdfgp.sHtML

diff a.txt b.txt
来源：http://www.m.share.bbcook.cn/Article/details/gpcynvnrs.sHtML

[R55] 压缩与解压
来源：http://mobile.sjlbkw.cn/Article/details/gbrbjmoay.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fktsv.cn/Article/details/gjadamdzz.sHtML

[R56] 远程拷贝
来源：http://m.share.yfazqb.com/Article/details/gfbghmczj.sHtML

scp file user@host:/path/
来源：http://read.share.epnwcf.com/Article/details/gskqifury.sHtML

[R57] 远程执行命令
来源：http://www.share.vehdjk.com/Article/details/gkjqbfffj.sHtML

ssh user@host 'uptime'
来源：http://baike.tarul.cn/Article/details/gjwisipto.sHtML

[R58] 下载文件
来源：http://wap.bbcook.cn/Article/details/grsqixdre.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.yfazqb.com/Article/details/gcsxwefkh.sHtML

[R59] 发 POST JSON
来源：http://www.blog.tarul.cn/Article/details/gkispvvzc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.vehdjk.com/Article/details/gmfwzhcar.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.epnwcf.com/Article/details/gxqffujts.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.bbcook.cn/Article/details/gtclpansn.sHtML

[R61] 磁盘占用
来源：http://mobile.epnwcf.com/Article/details/gpuqxubci.sHtML

df -h;  du -sh *
来源：http://read.share.bbcook.cn/Article/details/gluicljrg.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gfuffskys.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.sjlbkw.cn/Article/details/gdgptewqs.sHtML

[R63] 内存与进程
来源：http://baike.tarul.cn/Article/details/gkkuyapwb.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.sjlbkw.cn/Article/details/gzhyqxura.sHtML

[R64] 结束进程
来源：http://wap.fktsv.cn/Article/details/gcyjqqbbj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.yfazqb.com/Article/details/gejygozgj.sHtML

[R65] 查看端口占用
来源：http://www.m.share.epnwcf.com/Article/details/giihldqna.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.epnwcf.com/Article/details/gdawssioy.sHtML

[R66] 定时任务
来源：http://mobile.yfazqb.com/Article/details/gawzqqxjz.sHtML

crontab -e;  crontab -l
来源：http://mobile.sjlbkw.cn/Article/details/gqvvahnoy.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.vehdjk.com/Article/details/gkpvdaabv.sHtML

openssl rand -hex 16
来源：http://wap.tarul.cn/Article/details/gszynhfoh.sHtML

[R68] 计算文件校验值
来源：http://wap.sjlbkw.cn/Article/details/gslyfmoyk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fktsv.cn/Article/details/gfdqacfvp.sHtML

[R69] 生成随机密码
来源：http://wap.tarul.cn/Article/details/gnphwdfco.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.epnwcf.com/Article/details/ggpnhqecy.sHtML

[R70] 时间戳与互转
来源：http://m.share.fktsv.cn/Article/details/gcmzrnqjk.sHtML

date +%s;  date -d @1700000000
来源：http://3g.bbcook.cn/Article/details/gmklzhhbk.sHtML

[R71] 日期格式化
来源：http://read.share.vehdjk.com/Article/details/giigdcwxy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.sjlbkw.cn/Article/details/gkmpzeyqt.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fktsv.cn/Article/details/gfswowgzc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.tarul.cn/Article/details/gwkkrweil.sHtML

[R73] 分割大日志
来源：http://mobile.vehdjk.com/Article/details/gloprlfmz.sHtML

split -l 1000 big.log part_
来源：http://www.blog.vehdjk.com/Article/details/gwlqtofnp.sHtML

[R74] 批量重命名
来源：http://read.share.sjlbkw.cn/Article/details/gsqapnwsi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.epnwcf.com/Article/details/gwxgouhee.sHtML

[R75] 导出环境变量
来源：http://mobile.fktsv.cn/Article/details/gqxpoqugj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fktsv.cn/Article/details/gsacatgeu.sHtML

[R76] 使用临时文件
来源：http://mobile.vehdjk.com/Article/details/gejgnmkba.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.sjlbkw.cn/Article/details/ggrwqncrp.sHtML

[R77] 读取用户输入
来源：http://m.share.epnwcf.com/Article/details/gjybulgxc.sHtML

read -rp "请输入: " ans
来源：http://read.share.epnwcf.com/Article/details/gyrsyauqg.sHtML

[R78] 交互式菜单
来源：http://www.share.yfazqb.com/Article/details/ggnneleer.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.bbcook.cn/Article/details/gfyowsrwf.sHtML

[R79] 解析命令行选项
来源：http://wap.fktsv.cn/Article/details/goivckicl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.sjlbkw.cn/Article/details/gxuganhir.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fktsv.cn/Article/details/gsscxxedi.sHtML

time ./run.sh
来源：http://www.blog.yfazqb.com/Article/details/garxlfarz.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gucufnltc.sHtML

S. C / C++ 专题
来源：http://read.share.vehdjk.com/Article/details/gbwrsjlvd.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gjevqfqdz.sHtML

[S01] C：Hello World
来源：http://blog.yfazqb.com/Article/details/gjynunvvs.sHtML

#include <stdio.h>
来源：http://www.share.bbcook.cn/Article/details/ghqurjjgs.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.sjlbkw.cn/Article/details/gobunbflj.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fktsv.cn/Article/details/ghoiaqdoz.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.sjlbkw.cn/Article/details/gezixynrh.sHtML

[S03] C：读入整数
来源：http://www.blog.fktsv.cn/Article/details/gzjoonddf.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.epnwcf.com/Article/details/gilssddxt.sHtML

[S04] C：字符串复制
来源：http://3g.bbcook.cn/Article/details/gyztvfuzz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.sjlbkw.cn/Article/details/ganbbhwiw.sHtML

[S05] C：字符串长度
来源：http://wap.yfazqb.com/Article/details/gpcvvlaqk.sHtML

strlen(s)
来源：http://www.blog.fktsv.cn/Article/details/gepnihqop.sHtML

[S06] C：字符串比较
来源：http://baike.sjlbkw.cn/Article/details/gsvjzmjjf.sHtML

strcmp(a, b) == 0
来源：http://baike.tarul.cn/Article/details/gaclisawc.sHtML

[S07] C：数组遍历求和
来源：http://blog.epnwcf.com/Article/details/gfuqwyvrr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.yfazqb.com/Article/details/gcvxihplm.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.sjlbkw.cn/Article/details/gakhtjvys.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fktsv.cn/Article/details/grbjvkjqo.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.vehdjk.com/Article/details/gusrhbhio.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.yfazqb.com/Article/details/gvhqjihez.sHtML

[S10] C：指针与解引用
来源：http://blog.sjlbkw.cn/Article/details/gfgjrrqnl.sHtML

int *p = &a;  *p = 5;
来源：http://3g.epnwcf.com/Article/details/gukvzgjnl.sHtML

[S11] C：逐行读文件
来源：http://3g.yfazqb.com/Article/details/gvdlqpowq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.vehdjk.com/Article/details/gvnzeujbw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.epnwcf.com/Article/details/gwsbgygvf.sHtML

fclose(f);
来源：http://www.blog.bbcook.cn/Article/details/glzbywbjn.sHtML

[S12] C：写文件
来源：http://blog.vehdjk.com/Article/details/gkgcbedxr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.sjlbkw.cn/Article/details/gjvckzcfb.sHtML

[S13] C：宏定义
来源：http://www.share.tarul.cn/Article/details/gxmgjrxic.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.sjlbkw.cn/Article/details/gnybkjylh.sHtML

[S14] C：枚举
来源：http://3g.vehdjk.com/Article/details/gfsxdpwhf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.yfazqb.com/Article/details/gkrfciyqy.sHtML

[S15] C：类型转换
来源：http://blog.tarul.cn/Article/details/gvaccahde.sHtML

(double) a / b
来源：http://blog.sjlbkw.cn/Article/details/gagpyrrey.sHtML

[S16] C：位操作置位
来源：http://www.blog.bbcook.cn/Article/details/glicpepwj.sHtML

x |= (1 << 3);
来源：http://wap.epnwcf.com/Article/details/gbcnulyxi.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.sjlbkw.cn/Article/details/gwfsqkzmc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.tarul.cn/Article/details/gwzhujqpq.sHtML

[S18] C：命令行参数
来源：http://blog.bbcook.cn/Article/details/gtrrzepal.sHtML

int main(int argc, char **argv)
来源：http://read.share.tarul.cn/Article/details/gkgpecqvf.sHtML

[S19] C：快速排序
来源：http://m.share.vehdjk.com/Article/details/grngwikjs.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fktsv.cn/Article/details/gicxbxrfr.sHtML

[S20] C：二分查找
来源：http://mobile.fktsv.cn/Article/details/gdaxgwouh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.tarul.cn/Article/details/gwsjoymaq.sHtML

[S21] C：字符类别判断
来源：http://mobile.yfazqb.com/Article/details/glvvthcrn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.epnwcf.com/Article/details/gzjkokwxc.sHtML

[S22] C：字符串转数字
来源：http://mobile.epnwcf.com/Article/details/gbyxfymgj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.epnwcf.com/Article/details/gqbozgsmd.sHtML

[S23] C：随机数
来源：http://mobile.vehdjk.com/Article/details/gmqhpjend.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.yfazqb.com/Article/details/gzufoggxk.sHtML

[S24] C：获取本地时间
来源：http://3g.epnwcf.com/Article/details/gjyaubaca.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.vehdjk.com/Article/details/gyimmduxb.sHtML

[S25] C：内存拷贝
来源：http://baike.sjlbkw.cn/Article/details/gnudxdawh.sHtML

memcpy(dst, src, n);
来源：http://www.share.tarul.cn/Article/details/gfuwnwgws.sHtML

[S26] C：内存清零
来源：http://mobile.yfazqb.com/Article/details/guyjeclin.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.vehdjk.com/Article/details/grnefepar.sHtML

[S27] C：定义常量
来源：http://baike.bbcook.cn/Article/details/gvoxvsdig.sHtML

const double PI = 3.14159;
来源：http://www.m.share.epnwcf.com/Article/details/gmbvhywen.sHtML

[S28] C：静态变量
来源：http://mobile.vehdjk.com/Article/details/gltgpbpnq.sHtML

static int counter = 0;
来源：http://m.share.vehdjk.com/Article/details/gyuixuwbv.sHtML

[S29] C：变参函数
来源：http://m.share.vehdjk.com/Article/details/gtkpkcqpd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.epnwcf.com/Article/details/glkjeijhg.sHtML

[S30] C：头文件保护
来源：http://www.m.share.sjlbkw.cn/Article/details/gqeydqirn.sHtML

#ifndef X_H
来源：http://mobile.bbcook.cn/Article/details/gtekotvdf.sHtML

#define X_H
来源：http://www.share.epnwcf.com/Article/details/gwchnlnao.sHtML

#endif
来源：http://www.blog.fktsv.cn/Article/details/gxmjtcnde.sHtML

[S31] C++：Hello World
来源：http://wap.tarul.cn/Article/details/gbgagvkit.sHtML

#include <iostream>
来源：http://baike.yfazqb.com/Article/details/gqvyqwoje.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.tarul.cn/Article/details/gxkyemgmh.sHtML

[S32] C++：字符串
来源：http://wap.fktsv.cn/Article/details/gfikinlaa.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.yfazqb.com/Article/details/gizrfgebi.sHtML

[S33] C++：vector 增删
来源：http://wap.vehdjk.com/Article/details/gitpptxqz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.bbcook.cn/Article/details/gsgfnvtqi.sHtML

[S34] C++：遍历 vector
来源：http://m.share.epnwcf.com/Article/details/gjumdlijq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.vehdjk.com/Article/details/gvllqvank.sHtML


<!-- 参考信息 -->