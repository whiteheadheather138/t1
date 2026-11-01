代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.epnwcf.com/Article/details/ghahncspm.sHtML

[Q75] 日期格式化
来源：http://3g.yfazqb.com/Article/details/gstavhilc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.bbcook.cn/Article/details/gvkhawlqu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.vehdjk.com/Article/details/gttlwbqta.sHtML

[Q76] 按天统计
来源：http://m.share.yfazqb.com/Article/details/gmoeifgza.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.tarul.cn/Article/details/gjgonpssw.sHtML

[Q77] 时间加减
来源：http://www.blog.sjlbkw.cn/Article/details/gufobvlvj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.bbcook.cn/Article/details/gdqiggsxv.sHtML

[Q78] 当前时间
来源：http://www.blog.bbcook.cn/Article/details/gtdcvvjwk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.tarul.cn/Article/details/gszbuaoqw.sHtML

[Q79] 字符串拼接
来源：http://mobile.yfazqb.com/Article/details/gmbasihdi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.bbcook.cn/Article/details/gffkqqpvt.sHtML

[Q80] 字符串截取
来源：http://mobile.bbcook.cn/Article/details/giukebzgm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gxrnczfac.sHtML

[Q81] 字符串替换
来源：http://blog.yfazqb.com/Article/details/gzygzhjra.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gpzewrbal.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.bbcook.cn/Article/details/gdxljwjpr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gddbhuerr.sHtML

[Q83] 大小写转换
来源：http://wap.tarul.cn/Article/details/gowxeqpif.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gvwrttskr.sHtML

[Q84] 去除首尾空格
来源：http://blog.yfazqb.com/Article/details/gfimcdsww.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.bbcook.cn/Article/details/gprnotxnw.sHtML

[Q85] 数值取整
来源：http://www.share.bbcook.cn/Article/details/gdhsxtped.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.sjlbkw.cn/Article/details/gaysftkpu.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.sjlbkw.cn/Article/details/gkrazqbhk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.sjlbkw.cn/Article/details/gtpgifurk.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.vehdjk.com/Article/details/ghbgxeiou.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fktsv.cn/Article/details/gcdexqsnv.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.tarul.cn/Article/details/gtonyvntz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.bbcook.cn/Article/details/gzedjqfxo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gbkcsbrzm.sHtML

[Q89] 判断表是否存在
来源：http://baike.bbcook.cn/Article/details/ggkjxtewu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.sjlbkw.cn/Article/details/gfnshatxv.sHtML

[Q90] 生成序号列
来源：http://mobile.tarul.cn/Article/details/gyrnqjptw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.sjlbkw.cn/Article/details/gnrcgyihj.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gtqdkueka.sHtML

R. Bash 专题
来源：http://read.share.sjlbkw.cn/Article/details/gcpnduijh.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gzsrsskkp.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.vehdjk.com/Article/details/goedaowiv.sHtML

#!/usr/bin/env bash
来源：http://wap.sjlbkw.cn/Article/details/ghdmuyrsj.sHtML

set -euo pipefail
来源：http://3g.yfazqb.com/Article/details/gttffysvo.sHtML

[R02] 变量赋值与使用
来源：http://m.share.tarul.cn/Article/details/gtykokhaa.sHtML

name="Tom"; echo "$name"
来源：http://wap.tarul.cn/Article/details/gvzwpgpjx.sHtML

[R03] 只读变量
来源：http://www.m.share.yfazqb.com/Article/details/gzpbflphb.sHtML

readonly PI=3.14
来源：http://read.share.tarul.cn/Article/details/gcngegfph.sHtML

[R04] 位置参数
来源：http://www.share.bbcook.cn/Article/details/gagfcjvax.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.tarul.cn/Article/details/gzjfgzovf.sHtML

[R05] 参数默认值
来源：http://read.share.fktsv.cn/Article/details/gihuhshgb.sHtML

name="${1:-default}"
来源：http://m.share.fktsv.cn/Article/details/gtmqeghzr.sHtML

[R06] 判断命令是否存在
来源：http://3g.fktsv.cn/Article/details/gtjuyozbl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.vehdjk.com/Article/details/gtrixpsjj.sHtML

[R07] if 判断文件
来源：http://m.share.fktsv.cn/Article/details/ggdkhujmq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.tarul.cn/Article/details/gmzlrjvjd.sHtML

[R08] 数值比较
来源：http://baike.epnwcf.com/Article/details/gflqzaqnh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.sjlbkw.cn/Article/details/gjmjzbxyt.sHtML

[R09] 字符串比较
来源：http://www.share.vehdjk.com/Article/details/glitzksuu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.tarul.cn/Article/details/gywleetkz.sHtML

[R10] 正则匹配
来源：http://www.blog.epnwcf.com/Article/details/gxnlbwtyc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.yfazqb.com/Article/details/gnbtismmy.sHtML

[R11] case 多分支
来源：http://mobile.tarul.cn/Article/details/gxdvtqler.sHtML

case "$1" in
来源：http://www.blog.fktsv.cn/Article/details/gohizjegs.sHtML

start) echo "启动" ;;
来源：http://read.share.sjlbkw.cn/Article/details/gtqifmxxo.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fktsv.cn/Article/details/gzjyvlnsv.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fktsv.cn/Article/details/gagaqsapd.sHtML

esac
来源：http://wap.fktsv.cn/Article/details/gzrcbuyyj.sHtML

[R12] for 遍历文件
来源：http://blog.bbcook.cn/Article/details/gnucqpofa.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fktsv.cn/Article/details/gcumfkotk.sHtML

[R13] for 计数循环
来源：http://blog.epnwcf.com/Article/details/gwvlefozd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.yfazqb.com/Article/details/gfsucofwk.sHtML

[R14] C 风格 for
来源：http://blog.fktsv.cn/Article/details/grgjjibdv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.epnwcf.com/Article/details/gphdvhpxt.sHtML

[R15] while 逐行读文件
来源：http://m.share.yfazqb.com/Article/details/gpbulqpru.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.sjlbkw.cn/Article/details/gwlmbapwb.sHtML

[R16] until 等待条件
来源：http://www.m.share.tarul.cn/Article/details/grpgmjecs.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.yfazqb.com/Article/details/gcdgknizz.sHtML

[R17] 数组定义与取值
来源：http://m.share.fktsv.cn/Article/details/gjxqdjqyt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gaegkmuae.sHtML

[R18] 遍历数组
来源：http://m.share.fktsv.cn/Article/details/gmhwhprkr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fktsv.cn/Article/details/gvtuojyep.sHtML

[R19] 数组长度
来源：http://baike.tarul.cn/Article/details/gfxugbgcq.sHtML

echo "${#arr[@]}"
来源：http://www.share.fktsv.cn/Article/details/gcwebfpbq.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fktsv.cn/Article/details/gdjyxdvzr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.sjlbkw.cn/Article/details/ghvdigwgb.sHtML

[R21] 字符串长度
来源：http://mobile.tarul.cn/Article/details/gjdyzivnv.sHtML

echo "${#s}"
来源：http://wap.tarul.cn/Article/details/gyhoqcdry.sHtML

[R22] 截取子串
来源：http://read.share.tarul.cn/Article/details/gopbvcqgk.sHtML

echo "${s:0:5}"
来源：http://blog.bbcook.cn/Article/details/gznsmnzek.sHtML

[R23] 字符串替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gjcdtcwaw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fktsv.cn/Article/details/geoypbada.sHtML

[R24] 大小写转换
来源：http://mobile.yfazqb.com/Article/details/gktyodxtf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fktsv.cn/Article/details/gwamsjili.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.vehdjk.com/Article/details/gtvjhffuw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.bbcook.cn/Article/details/grqmztzds.sHtML

[R26] 命令替换
来源：http://baike.tarul.cn/Article/details/gruocxhrn.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.bbcook.cn/Article/details/gbrrxxhvz.sHtML

[R27] 算术展开
来源：http://wap.tarul.cn/Article/details/gmyhuodgp.sHtML

echo $((1 + 2 * 3))
来源：http://wap.yfazqb.com/Article/details/gbriodhjl.sHtML

[R28] 浮点运算
来源：http://read.share.epnwcf.com/Article/details/gquuifppm.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.tarul.cn/Article/details/gazjgeaei.sHtML

[R29] 定义函数
来源：http://www.share.yfazqb.com/Article/details/glivfffeh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.bbcook.cn/Article/details/gbzeegmal.sHtML

[R30] 函数返回状态码
来源：http://read.share.bbcook.cn/Article/details/grwayhhlu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.epnwcf.com/Article/details/gyaahqyhq.sHtML

[R31] 局部变量
来源：http://baike.yfazqb.com/Article/details/gzsnqutxx.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fktsv.cn/Article/details/ghybrmbeg.sHtML

[R32] 参数个数校验
来源：http://wap.epnwcf.com/Article/details/gltjumsyn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.tarul.cn/Article/details/gtbkqffpm.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fktsv.cn/Article/details/gaylbduvr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fktsv.cn/Article/details/gvbbdtlil.sHtML

[R34] 退出时清理
来源：http://mobile.yfazqb.com/Article/details/guxminvyx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.epnwcf.com/Article/details/gvaucihni.sHtML

[R35] 后台执行并等待
来源：http://wap.vehdjk.com/Article/details/gobhcvpqo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.vehdjk.com/Article/details/glsppdfbc.sHtML

[R36] 并发执行多个任务
来源：http://blog.sjlbkw.cn/Article/details/gznqaldrq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.tarul.cn/Article/details/gvwdunibx.sHtML

[R37] 把输出赋给变量
来源：http://baike.fktsv.cn/Article/details/gamedmtnb.sHtML

files=$(ls -1)
来源：http://www.share.sjlbkw.cn/Article/details/gwgpbbxtd.sHtML

[R38] 管道串联
来源：http://wap.fktsv.cn/Article/details/gtxnozlir.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.vehdjk.com/Article/details/gkyqoeewp.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.epnwcf.com/Article/details/gkwtcoodw.sHtML

cmd > out.log 2>&1
来源：http://blog.bbcook.cn/Article/details/grqljrdiz.sHtML

[R40] 追加写日志
来源：http://3g.tarul.cn/Article/details/gvjrmqwtp.sHtML

echo "log" >> out.log
来源：http://blog.vehdjk.com/Article/details/gvfhlsxrr.sHtML

[R41] 丢弃输出
来源：http://read.share.epnwcf.com/Article/details/gvepeuhzz.sHtML

cmd >/dev/null 2>&1
来源：http://blog.tarul.cn/Article/details/gzdlwcoqu.sHtML

[R42] 输入重定向
来源：http://baike.sjlbkw.cn/Article/details/ghcclulqj.sHtML

wc -l < a.txt
来源：http://wap.tarul.cn/Article/details/ggojnrdsc.sHtML

[R43] 按名字查找文件
来源：http://mobile.fktsv.cn/Article/details/gcartfazl.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fktsv.cn/Article/details/gffvckjdx.sHtML

[R44] 按修改时间查找
来源：http://blog.bbcook.cn/Article/details/gjxmeacco.sHtML

find . -mtime -7 -type f
来源：http://3g.fktsv.cn/Article/details/glydwllpj.sHtML

[R45] 批量删除
来源：http://mobile.bbcook.cn/Article/details/giuebrrxm.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.vehdjk.com/Article/details/gulvdtttg.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.yfazqb.com/Article/details/gqomkbrgi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fktsv.cn/Article/details/giltjgatk.sHtML

[R47] sed 单行替换
来源：http://blog.sjlbkw.cn/Article/details/gsxweovlg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.yfazqb.com/Article/details/gnhujazmc.sHtML

[R48] awk 取指定列
来源：http://m.share.tarul.cn/Article/details/gjenfrtgn.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.yfazqb.com/Article/details/givrwcvgq.sHtML

[R49] awk 带条件
来源：http://www.blog.tarul.cn/Article/details/genxiudvp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.tarul.cn/Article/details/gkgcivtwp.sHtML

[R50] awk 求和
来源：http://read.share.yfazqb.com/Article/details/gpethtbcz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fktsv.cn/Article/details/gvcynysvf.sHtML

[R51] 排序去重取前几
来源：http://blog.bbcook.cn/Article/details/grpupjzqa.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fktsv.cn/Article/details/gktbqfsau.sHtML

[R52] 统计行数
来源：http://baike.epnwcf.com/Article/details/gpnxlerdn.sHtML

wc -l a.txt
来源：http://blog.tarul.cn/Article/details/gskfezptx.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.tarul.cn/Article/details/gkdvhlwwd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.tarul.cn/Article/details/gglokmapr.sHtML

[R54] 比较两个文件
来源：http://blog.yfazqb.com/Article/details/gwejtxeem.sHtML

diff a.txt b.txt
来源：http://blog.yfazqb.com/Article/details/gwkhoxyzq.sHtML

[R55] 压缩与解压
来源：http://baike.tarul.cn/Article/details/godnvxiie.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.vehdjk.com/Article/details/gdkdocpxs.sHtML

[R56] 远程拷贝
来源：http://baike.tarul.cn/Article/details/gxmpogqlu.sHtML

scp file user@host:/path/
来源：http://blog.yfazqb.com/Article/details/gslawplvd.sHtML

[R57] 远程执行命令
来源：http://wap.bbcook.cn/Article/details/gdsjbdqcz.sHtML

ssh user@host 'uptime'
来源：http://wap.tarul.cn/Article/details/gfjypeinx.sHtML

[R58] 下载文件
来源：http://3g.bbcook.cn/Article/details/galdsweps.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.tarul.cn/Article/details/gjzrkvdkx.sHtML

[R59] 发 POST JSON
来源：http://mobile.tarul.cn/Article/details/gwjnuoowm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.vehdjk.com/Article/details/gvatnyczl.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.bbcook.cn/Article/details/gixjibxqd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.epnwcf.com/Article/details/gxazyfdzs.sHtML

[R61] 磁盘占用
来源：http://www.share.fktsv.cn/Article/details/gssycxass.sHtML

df -h;  du -sh *
来源：http://mobile.epnwcf.com/Article/details/gfjcyusri.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.epnwcf.com/Article/details/gtkudkmtn.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.yfazqb.com/Article/details/gdxgilbhv.sHtML

[R63] 内存与进程
来源：http://m.share.tarul.cn/Article/details/gomxygjco.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.epnwcf.com/Article/details/gzmeusoig.sHtML

[R64] 结束进程
来源：http://blog.bbcook.cn/Article/details/gtmslzdnn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.epnwcf.com/Article/details/gbktdupmz.sHtML

[R65] 查看端口占用
来源：http://wap.sjlbkw.cn/Article/details/gozbnxjwc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.sjlbkw.cn/Article/details/glxftyabj.sHtML

[R66] 定时任务
来源：http://www.m.share.fktsv.cn/Article/details/gazxolfon.sHtML

crontab -e;  crontab -l
来源：http://m.share.epnwcf.com/Article/details/ggwdcqfxn.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fktsv.cn/Article/details/gyzqrjljf.sHtML

openssl rand -hex 16
来源：http://read.share.yfazqb.com/Article/details/gmnimcaek.sHtML

[R68] 计算文件校验值
来源：http://wap.vehdjk.com/Article/details/ggeemtqqs.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.bbcook.cn/Article/details/gofcaynin.sHtML

[R69] 生成随机密码
来源：http://3g.fktsv.cn/Article/details/gpquyqqlh.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fktsv.cn/Article/details/gnpbiemop.sHtML

[R70] 时间戳与互转
来源：http://www.share.fktsv.cn/Article/details/gpdbsunki.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.vehdjk.com/Article/details/gihuutoxa.sHtML

[R71] 日期格式化
来源：http://wap.epnwcf.com/Article/details/gbdehotbh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.vehdjk.com/Article/details/gnapmyfou.sHtML

[R72] 等待端口就绪
来源：http://wap.bbcook.cn/Article/details/gochlvrhg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.yfazqb.com/Article/details/grfcbieku.sHtML

[R73] 分割大日志
来源：http://blog.yfazqb.com/Article/details/gxoxhfvlz.sHtML

split -l 1000 big.log part_
来源：http://baike.fktsv.cn/Article/details/govqjahvl.sHtML

[R74] 批量重命名
来源：http://www.blog.epnwcf.com/Article/details/gyuyzmrnd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.bbcook.cn/Article/details/gthchvpxe.sHtML

[R75] 导出环境变量
来源：http://mobile.sjlbkw.cn/Article/details/galpfpwcp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.epnwcf.com/Article/details/gyfljidkg.sHtML

[R76] 使用临时文件
来源：http://mobile.sjlbkw.cn/Article/details/gllgebvoy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.sjlbkw.cn/Article/details/ggnzeargt.sHtML

[R77] 读取用户输入
来源：http://www.blog.fktsv.cn/Article/details/gzowuomzj.sHtML

read -rp "请输入: " ans
来源：http://mobile.fktsv.cn/Article/details/gyhqiibco.sHtML

[R78] 交互式菜单
来源：http://www.share.sjlbkw.cn/Article/details/gtmpcyenn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.yfazqb.com/Article/details/gmilvphnc.sHtML

[R79] 解析命令行选项
来源：http://www.share.sjlbkw.cn/Article/details/gypbvpenh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.sjlbkw.cn/Article/details/gyrrqpfss.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.tarul.cn/Article/details/gsbabqnoh.sHtML

time ./run.sh
来源：http://mobile.vehdjk.com/Article/details/gqmkxseup.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gtgctgaqp.sHtML

S. C / C++ 专题
来源：http://blog.bbcook.cn/Article/details/gmlujbote.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gkmmabcls.sHtML

[S01] C：Hello World
来源：http://baike.yfazqb.com/Article/details/gwcomvjsj.sHtML

#include <stdio.h>
来源：http://mobile.sjlbkw.cn/Article/details/glouvtlyb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fktsv.cn/Article/details/gwzsrqmqt.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fktsv.cn/Article/details/gsmfjbzen.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.tarul.cn/Article/details/gmohhnrcg.sHtML

[S03] C：读入整数
来源：http://read.share.vehdjk.com/Article/details/gxmyxvfwm.sHtML

int x; scanf("%d", &x);
来源：http://baike.bbcook.cn/Article/details/gbiztwpbz.sHtML

[S04] C：字符串复制
来源：http://baike.vehdjk.com/Article/details/gwtvyzvfk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.vehdjk.com/Article/details/gamjgqbze.sHtML

[S05] C：字符串长度
来源：http://www.m.share.yfazqb.com/Article/details/gxayxepne.sHtML

strlen(s)
来源：http://blog.tarul.cn/Article/details/glupibccg.sHtML

[S06] C：字符串比较
来源：http://m.share.vehdjk.com/Article/details/gasbqjire.sHtML

strcmp(a, b) == 0
来源：http://baike.tarul.cn/Article/details/gflhisivn.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.epnwcf.com/Article/details/gldirfzii.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.tarul.cn/Article/details/goumuzyli.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fktsv.cn/Article/details/gajuvxxpp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.epnwcf.com/Article/details/gizybpxyk.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fktsv.cn/Article/details/gyfxdftlw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fktsv.cn/Article/details/gykkpmggk.sHtML

[S10] C：指针与解引用
来源：http://wap.fktsv.cn/Article/details/ggsamfdfc.sHtML

int *p = &a;  *p = 5;
来源：http://3g.bbcook.cn/Article/details/gycaukbfh.sHtML

[S11] C：逐行读文件
来源：http://wap.epnwcf.com/Article/details/gbbwxzeby.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.epnwcf.com/Article/details/gqyuvityl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.epnwcf.com/Article/details/gizbnterz.sHtML

fclose(f);
来源：http://wap.epnwcf.com/Article/details/gvcempaju.sHtML

[S12] C：写文件
来源：http://read.share.tarul.cn/Article/details/gpegvwxgm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.vehdjk.com/Article/details/gzujzymwx.sHtML

[S13] C：宏定义
来源：http://www.m.share.sjlbkw.cn/Article/details/goumgqjmv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.tarul.cn/Article/details/gkrnzleec.sHtML

[S14] C：枚举
来源：http://mobile.sjlbkw.cn/Article/details/gztkohpgy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.tarul.cn/Article/details/gzlskvolk.sHtML

[S15] C：类型转换
来源：http://www.blog.epnwcf.com/Article/details/ggwdcnhez.sHtML

(double) a / b
来源：http://m.share.tarul.cn/Article/details/gvjkpygjq.sHtML

[S16] C：位操作置位
来源：http://mobile.tarul.cn/Article/details/gpgfckfel.sHtML

x |= (1 << 3);
来源：http://baike.fktsv.cn/Article/details/gxdvifiqj.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.tarul.cn/Article/details/ghldqptoz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fktsv.cn/Article/details/gvxoskzpr.sHtML

[S18] C：命令行参数
来源：http://www.share.vehdjk.com/Article/details/gqazczivb.sHtML

int main(int argc, char **argv)
来源：http://wap.epnwcf.com/Article/details/gmruxlnyh.sHtML

[S19] C：快速排序
来源：http://www.blog.vehdjk.com/Article/details/grnftyuxh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.tarul.cn/Article/details/gbxrqqgyp.sHtML

[S20] C：二分查找
来源：http://3g.sjlbkw.cn/Article/details/gfcxntwlk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.yfazqb.com/Article/details/gaxepgnym.sHtML

[S21] C：字符类别判断
来源：http://www.blog.bbcook.cn/Article/details/glsksxezm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.epnwcf.com/Article/details/gjteqmrlx.sHtML

[S22] C：字符串转数字
来源：http://blog.fktsv.cn/Article/details/gjpuhbpgo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.vehdjk.com/Article/details/guogxqgse.sHtML

[S23] C：随机数
来源：http://3g.fktsv.cn/Article/details/gmiotjxdq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.yfazqb.com/Article/details/gsrrijjju.sHtML

[S24] C：获取本地时间
来源：http://read.share.tarul.cn/Article/details/gfuhhlvzw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.sjlbkw.cn/Article/details/gneqqtehs.sHtML

[S25] C：内存拷贝
来源：http://mobile.fktsv.cn/Article/details/gjaeudbco.sHtML

memcpy(dst, src, n);
来源：http://m.share.epnwcf.com/Article/details/gtwaxldor.sHtML

[S26] C：内存清零
来源：http://m.share.sjlbkw.cn/Article/details/geiobpwas.sHtML

memset(a, 0, sizeof a);
来源：http://blog.epnwcf.com/Article/details/gmxtjmoyn.sHtML

[S27] C：定义常量
来源：http://baike.vehdjk.com/Article/details/geuxwokof.sHtML

const double PI = 3.14159;
来源：http://www.blog.tarul.cn/Article/details/ghieccfqi.sHtML

[S28] C：静态变量
来源：http://m.share.vehdjk.com/Article/details/gauuwxsoi.sHtML

static int counter = 0;
来源：http://m.share.yfazqb.com/Article/details/gvmjqeojy.sHtML

[S29] C：变参函数
来源：http://www.share.yfazqb.com/Article/details/gdrzxtcpq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.epnwcf.com/Article/details/gpxknipqq.sHtML

[S30] C：头文件保护
来源：http://www.share.vehdjk.com/Article/details/gkxfdgwoq.sHtML

#ifndef X_H
来源：http://m.share.bbcook.cn/Article/details/gtsnehozb.sHtML

#define X_H
来源：http://www.m.share.bbcook.cn/Article/details/gpiokxhkv.sHtML

#endif
来源：http://blog.yfazqb.com/Article/details/gaguwqrbo.sHtML

[S31] C++：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gthqjpkbe.sHtML

#include <iostream>
来源：http://3g.yfazqb.com/Article/details/gqjpykbnd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.sjlbkw.cn/Article/details/gpptbtjlc.sHtML

[S32] C++：字符串
来源：http://www.m.share.epnwcf.com/Article/details/gzjyznxbe.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.epnwcf.com/Article/details/gkgkasjgo.sHtML

[S33] C++：vector 增删
来源：http://www.share.fktsv.cn/Article/details/gqeqgfwvt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.yfazqb.com/Article/details/gghksrfsb.sHtML

[S34] C++：遍历 vector
来源：http://mobile.epnwcf.com/Article/details/gnglawsnv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.vehdjk.com/Article/details/garmhvvjo.sHtML

[S35] C++：map
来源：http://3g.sjlbkw.cn/Article/details/guyvgnbwo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.vehdjk.com/Article/details/gwkvufwlx.sHtML

[S36] C++：unordered_map
来源：http://m.share.bbcook.cn/Article/details/gisxznikl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gibbdhbtg.sHtML

[S37] C++：set
来源：http://www.share.epnwcf.com/Article/details/gvdoyankf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.sjlbkw.cn/Article/details/gdmwlrpfv.sHtML

[S38] C++：排序
来源：http://mobile.sjlbkw.cn/Article/details/gwimhkyuw.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.epnwcf.com/Article/details/ghlbuefjv.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.epnwcf.com/Article/details/gftkzdukh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.sjlbkw.cn/Article/details/gbmvuchqp.sHtML

[S40] C++：查找元素
来源：http://baike.yfazqb.com/Article/details/gigkexthv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.sjlbkw.cn/Article/details/gwditujmm.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.bbcook.cn/Article/details/gxdtiwnwa.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.tarul.cn/Article/details/gwavneifr.sHtML

[S42] C++：继承与虚函数
来源：http://3g.yfazqb.com/Article/details/ggwpxfnyb.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.epnwcf.com/Article/details/gqoclbboh.sHtML

[S43] C++：智能指针
来源：http://3g.tarul.cn/Article/details/gfchwitxu.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.yfazqb.com/Article/details/gunnthfxd.sHtML

[S44] C++：引用传参
来源：http://3g.vehdjk.com/Article/details/gnqovwyah.sHtML

void inc(int &x) { ++x; }
来源：http://3g.tarul.cn/Article/details/grlwpklmj.sHtML


<!-- 参考信息 -->