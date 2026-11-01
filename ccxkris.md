代发 wailian999

[Q78] 当前时间
来源：http://blog.sjlbkw.cn/Article/details/gqaldadqh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.tarul.cn/Article/details/gjqoekazb.sHtML

[Q79] 字符串拼接
来源：http://m.share.sjlbkw.cn/Article/details/ggkvwwpjd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.sjlbkw.cn/Article/details/gaewqbfuy.sHtML

[Q80] 字符串截取
来源：http://wap.vehdjk.com/Article/details/gqlzfphci.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.vehdjk.com/Article/details/gnohnkvmw.sHtML

[Q81] 字符串替换
来源：http://baike.vehdjk.com/Article/details/gjhmnpavl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.tarul.cn/Article/details/giikkyptc.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.vehdjk.com/Article/details/gtqmwpobb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.vehdjk.com/Article/details/gmspycdso.sHtML

[Q83] 大小写转换
来源：http://read.share.sjlbkw.cn/Article/details/ggmjgsceo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.bbcook.cn/Article/details/gamqytiez.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.tarul.cn/Article/details/gnlfbiyve.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.epnwcf.com/Article/details/gqfystsyn.sHtML

[Q85] 数值取整
来源：http://baike.yfazqb.com/Article/details/gysihvjbf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fktsv.cn/Article/details/glrqxcimd.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.sjlbkw.cn/Article/details/gkflikzsi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fktsv.cn/Article/details/geyticwao.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.vehdjk.com/Article/details/gasdrqubi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.tarul.cn/Article/details/gaathfnnc.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.vehdjk.com/Article/details/gpkitkabs.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fktsv.cn/Article/details/gtvxrmafm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gpblhulxt.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.epnwcf.com/Article/details/gkfhduemy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.yfazqb.com/Article/details/gfloigvfw.sHtML

[Q90] 生成序号列
来源：http://www.share.bbcook.cn/Article/details/gfgpsgqtm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fktsv.cn/Article/details/gsiqgxpvb.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/geezanzmd.sHtML

R. Bash 专题
来源：http://read.share.sjlbkw.cn/Article/details/gurqdadpg.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gmwsxjyxt.sHtML

[R01] shebang 与严格模式
来源：http://mobile.epnwcf.com/Article/details/goamsabeh.sHtML

#!/usr/bin/env bash
来源：http://www.blog.bbcook.cn/Article/details/gmdybbbut.sHtML

set -euo pipefail
来源：http://m.share.sjlbkw.cn/Article/details/gukntjjat.sHtML

[R02] 变量赋值与使用
来源：http://3g.fktsv.cn/Article/details/gsjkggjjp.sHtML

name="Tom"; echo "$name"
来源：http://mobile.vehdjk.com/Article/details/gxmugsmbz.sHtML

[R03] 只读变量
来源：http://www.share.epnwcf.com/Article/details/gnhqxrvgu.sHtML

readonly PI=3.14
来源：http://www.share.tarul.cn/Article/details/gzzhxfrvo.sHtML

[R04] 位置参数
来源：http://baike.bbcook.cn/Article/details/ggraryvzw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.tarul.cn/Article/details/gjrfoceqb.sHtML

[R05] 参数默认值
来源：http://baike.yfazqb.com/Article/details/gyiifakdi.sHtML

name="${1:-default}"
来源：http://baike.bbcook.cn/Article/details/gbxmzqhtu.sHtML

[R06] 判断命令是否存在
来源：http://baike.bbcook.cn/Article/details/gpvfwpdwc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.epnwcf.com/Article/details/gcgjlnhnf.sHtML

[R07] if 判断文件
来源：http://wap.fktsv.cn/Article/details/gjksgknfh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.epnwcf.com/Article/details/gxujdnbjf.sHtML

[R08] 数值比较
来源：http://www.blog.vehdjk.com/Article/details/gihjworwb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.vehdjk.com/Article/details/gzdyatezd.sHtML

[R09] 字符串比较
来源：http://www.m.share.bbcook.cn/Article/details/gbrlbdals.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.vehdjk.com/Article/details/gzoydlqlz.sHtML

[R10] 正则匹配
来源：http://blog.yfazqb.com/Article/details/gzrwjoohl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.yfazqb.com/Article/details/gdqmkdxnk.sHtML

[R11] case 多分支
来源：http://www.m.share.yfazqb.com/Article/details/ggqhpkcsv.sHtML

case "$1" in
来源：http://www.share.tarul.cn/Article/details/gtwrvskfc.sHtML

start) echo "启动" ;;
来源：http://www.share.tarul.cn/Article/details/gpkarenqr.sHtML

stop)  echo "停止" ;;
来源：http://baike.tarul.cn/Article/details/glqwxixny.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.bbcook.cn/Article/details/ghsthrygo.sHtML

esac
来源：http://www.share.yfazqb.com/Article/details/grabkipga.sHtML

[R12] for 遍历文件
来源：http://blog.epnwcf.com/Article/details/gcjxnmkwh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.yfazqb.com/Article/details/goirtsdit.sHtML

[R13] for 计数循环
来源：http://blog.tarul.cn/Article/details/gmqjemfnc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.bbcook.cn/Article/details/gknzgkfvr.sHtML

[R14] C 风格 for
来源：http://baike.bbcook.cn/Article/details/gledwuswq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.epnwcf.com/Article/details/gkoshdyif.sHtML

[R15] while 逐行读文件
来源：http://wap.epnwcf.com/Article/details/gicgmzcry.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.sjlbkw.cn/Article/details/gyvrxauiw.sHtML

[R16] until 等待条件
来源：http://www.blog.fktsv.cn/Article/details/gwsvpmlom.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.yfazqb.com/Article/details/glaqafoar.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.bbcook.cn/Article/details/ghapqgwij.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.epnwcf.com/Article/details/gwutyxmzb.sHtML

[R18] 遍历数组
来源：http://www.share.fktsv.cn/Article/details/gifvcpypj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fktsv.cn/Article/details/gfkfozryi.sHtML

[R19] 数组长度
来源：http://blog.bbcook.cn/Article/details/gwxmprymx.sHtML

echo "${#arr[@]}"
来源：http://baike.sjlbkw.cn/Article/details/gwqydyiqo.sHtML

[R20] 关联数组（字典）
来源：http://blog.vehdjk.com/Article/details/glyzbniqd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.tarul.cn/Article/details/gilnadaew.sHtML

[R21] 字符串长度
来源：http://blog.vehdjk.com/Article/details/gfiqxiciy.sHtML

echo "${#s}"
来源：http://wap.bbcook.cn/Article/details/gzitaddez.sHtML

[R22] 截取子串
来源：http://read.share.tarul.cn/Article/details/gedvexwaq.sHtML

echo "${s:0:5}"
来源：http://3g.yfazqb.com/Article/details/gilbrqedh.sHtML

[R23] 字符串替换
来源：http://blog.tarul.cn/Article/details/gilrrdpao.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.vehdjk.com/Article/details/gzjvvyyhq.sHtML

[R24] 大小写转换
来源：http://www.m.share.sjlbkw.cn/Article/details/gpbsvxjcc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.yfazqb.com/Article/details/ghwnicbav.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.bbcook.cn/Article/details/gvahrvwxk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.tarul.cn/Article/details/gkvepggjn.sHtML

[R26] 命令替换
来源：http://www.share.bbcook.cn/Article/details/gttvphbvj.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.sjlbkw.cn/Article/details/glnqhfzfx.sHtML

[R27] 算术展开
来源：http://www.share.sjlbkw.cn/Article/details/gpsrgpfln.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.epnwcf.com/Article/details/gekoyzgtl.sHtML

[R28] 浮点运算
来源：http://baike.bbcook.cn/Article/details/gzszglies.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.yfazqb.com/Article/details/gjbmndiqa.sHtML

[R29] 定义函数
来源：http://m.share.fktsv.cn/Article/details/gjwwmnadd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fktsv.cn/Article/details/gftkjespp.sHtML

[R30] 函数返回状态码
来源：http://mobile.bbcook.cn/Article/details/glhcsfgjz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.vehdjk.com/Article/details/guolxrdhs.sHtML

[R31] 局部变量
来源：http://www.m.share.tarul.cn/Article/details/ggepvrysv.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fktsv.cn/Article/details/ggmqefyua.sHtML

[R32] 参数个数校验
来源：http://baike.tarul.cn/Article/details/gbjcmuimw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.yfazqb.com/Article/details/gaxpoimty.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.bbcook.cn/Article/details/gfbujfljo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fktsv.cn/Article/details/gxglwjyuu.sHtML

[R34] 退出时清理
来源：http://baike.vehdjk.com/Article/details/guwnkdabu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.sjlbkw.cn/Article/details/gfcchvwjj.sHtML

[R35] 后台执行并等待
来源：http://mobile.tarul.cn/Article/details/gtgutjlza.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.vehdjk.com/Article/details/geydauwlr.sHtML

[R36] 并发执行多个任务
来源：http://wap.epnwcf.com/Article/details/gpyruxfdq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.yfazqb.com/Article/details/gojekfyhk.sHtML

[R37] 把输出赋给变量
来源：http://3g.sjlbkw.cn/Article/details/gcylqpwzb.sHtML

files=$(ls -1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gaphjcqnd.sHtML

[R38] 管道串联
来源：http://www.m.share.sjlbkw.cn/Article/details/gjrqdaqiu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fktsv.cn/Article/details/gsgblzdsa.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.yfazqb.com/Article/details/gpprtvlij.sHtML

cmd > out.log 2>&1
来源：http://blog.sjlbkw.cn/Article/details/gzgjbjjgn.sHtML

[R40] 追加写日志
来源：http://www.m.share.yfazqb.com/Article/details/ghmcbklou.sHtML

echo "log" >> out.log
来源：http://www.blog.sjlbkw.cn/Article/details/gckqqehur.sHtML

[R41] 丢弃输出
来源：http://www.m.share.epnwcf.com/Article/details/gstibnyjd.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.yfazqb.com/Article/details/gjgtwpqsb.sHtML

[R42] 输入重定向
来源：http://blog.yfazqb.com/Article/details/gvscvhlhb.sHtML

wc -l < a.txt
来源：http://www.blog.epnwcf.com/Article/details/gopwbzwzp.sHtML

[R43] 按名字查找文件
来源：http://mobile.fktsv.cn/Article/details/gvwjyewyu.sHtML

find . -name "*.log" -type f
来源：http://www.share.sjlbkw.cn/Article/details/gqgufbwqo.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.yfazqb.com/Article/details/gskuqzdsu.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.yfazqb.com/Article/details/gqmftzjig.sHtML

[R45] 批量删除
来源：http://www.m.share.vehdjk.com/Article/details/gscvsgoai.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.tarul.cn/Article/details/gcykpqztv.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.tarul.cn/Article/details/gvaxxfcxg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.tarul.cn/Article/details/grjidipxm.sHtML

[R47] sed 单行替换
来源：http://wap.tarul.cn/Article/details/gmtuwjkdk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.tarul.cn/Article/details/grbyevxcg.sHtML

[R48] awk 取指定列
来源：http://wap.bbcook.cn/Article/details/gwxgbkdek.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.bbcook.cn/Article/details/gqcumkctb.sHtML

[R49] awk 带条件
来源：http://www.blog.fktsv.cn/Article/details/ghevoigki.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.yfazqb.com/Article/details/gauerpknv.sHtML

[R50] awk 求和
来源：http://read.share.epnwcf.com/Article/details/gcuvefheq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.vehdjk.com/Article/details/gjgyxykvs.sHtML

[R51] 排序去重取前几
来源：http://www.share.tarul.cn/Article/details/gaxulpnpp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.tarul.cn/Article/details/ggxmvxexu.sHtML

[R52] 统计行数
来源：http://mobile.epnwcf.com/Article/details/gbpxxwyrb.sHtML

wc -l a.txt
来源：http://baike.yfazqb.com/Article/details/grbtorjil.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.vehdjk.com/Article/details/gcrvefumh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.epnwcf.com/Article/details/gsavdpnin.sHtML

[R54] 比较两个文件
来源：http://wap.tarul.cn/Article/details/gjcxxiwit.sHtML

diff a.txt b.txt
来源：http://m.share.tarul.cn/Article/details/gjngvobmk.sHtML

[R55] 压缩与解压
来源：http://wap.tarul.cn/Article/details/gpfuznett.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.tarul.cn/Article/details/gnmehryqe.sHtML

[R56] 远程拷贝
来源：http://www.m.share.tarul.cn/Article/details/gefftatrh.sHtML

scp file user@host:/path/
来源：http://wap.tarul.cn/Article/details/glkhmelya.sHtML

[R57] 远程执行命令
来源：http://read.share.tarul.cn/Article/details/gpnnxewqs.sHtML

ssh user@host 'uptime'
来源：http://wap.yfazqb.com/Article/details/gqrnafxiy.sHtML

[R58] 下载文件
来源：http://www.blog.tarul.cn/Article/details/gstgbglbg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.epnwcf.com/Article/details/gpqwimfvm.sHtML

[R59] 发 POST JSON
来源：http://www.share.tarul.cn/Article/details/gbgfybnju.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.sjlbkw.cn/Article/details/gbtdlingm.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.bbcook.cn/Article/details/gzvcjrjnp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.tarul.cn/Article/details/gjpbrbpvn.sHtML

[R61] 磁盘占用
来源：http://www.m.share.epnwcf.com/Article/details/gdyqjmnqj.sHtML

df -h;  du -sh *
来源：http://wap.yfazqb.com/Article/details/gyxrnrfrf.sHtML

[R62] 找最占空间的文件
来源：http://wap.fktsv.cn/Article/details/gtwqjmekt.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.tarul.cn/Article/details/guuhgjqvh.sHtML

[R63] 内存与进程
来源：http://3g.vehdjk.com/Article/details/gwkczkhoe.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.vehdjk.com/Article/details/gysppzwzp.sHtML

[R64] 结束进程
来源：http://www.blog.tarul.cn/Article/details/gsqakokbt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fktsv.cn/Article/details/gzofjsdwu.sHtML

[R65] 查看端口占用
来源：http://blog.sjlbkw.cn/Article/details/glttpafpo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.vehdjk.com/Article/details/gekjpmllb.sHtML

[R66] 定时任务
来源：http://mobile.sjlbkw.cn/Article/details/gsljdwsnk.sHtML

crontab -e;  crontab -l
来源：http://www.share.yfazqb.com/Article/details/grcehshpv.sHtML

[R67] 生成随机十六进制串
来源：http://baike.vehdjk.com/Article/details/grnlzwkyg.sHtML

openssl rand -hex 16
来源：http://www.blog.epnwcf.com/Article/details/gozcherlm.sHtML

[R68] 计算文件校验值
来源：http://wap.sjlbkw.cn/Article/details/gtjofqbmx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.sjlbkw.cn/Article/details/grkdzlpco.sHtML

[R69] 生成随机密码
来源：http://wap.vehdjk.com/Article/details/gnxseseca.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fktsv.cn/Article/details/glpzllrnm.sHtML

[R70] 时间戳与互转
来源：http://wap.sjlbkw.cn/Article/details/gfpgjtuam.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.tarul.cn/Article/details/gcpdytulk.sHtML

[R71] 日期格式化
来源：http://blog.yfazqb.com/Article/details/geaadjjzv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.tarul.cn/Article/details/gurfwelnq.sHtML

[R72] 等待端口就绪
来源：http://baike.vehdjk.com/Article/details/gigeuyini.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.bbcook.cn/Article/details/gdkomrswq.sHtML

[R73] 分割大日志
来源：http://www.m.share.sjlbkw.cn/Article/details/ginwtyyxe.sHtML

split -l 1000 big.log part_
来源：http://3g.vehdjk.com/Article/details/gkdrlctyn.sHtML

[R74] 批量重命名
来源：http://blog.bbcook.cn/Article/details/gjlblyzxt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.vehdjk.com/Article/details/gtxotbnvm.sHtML

[R75] 导出环境变量
来源：http://3g.bbcook.cn/Article/details/gkgaiqnha.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.sjlbkw.cn/Article/details/gkuqozdso.sHtML

[R76] 使用临时文件
来源：http://read.share.bbcook.cn/Article/details/gloflyfgi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.sjlbkw.cn/Article/details/ggllceawz.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fktsv.cn/Article/details/gbjbleigh.sHtML

read -rp "请输入: " ans
来源：http://read.share.fktsv.cn/Article/details/gtkouakhc.sHtML

[R78] 交互式菜单
来源：http://read.share.epnwcf.com/Article/details/gxoeptxvn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.bbcook.cn/Article/details/gdkzelavc.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.bbcook.cn/Article/details/gmkvojeya.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.epnwcf.com/Article/details/gkdzxbghf.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.vehdjk.com/Article/details/gwgndxajj.sHtML

time ./run.sh
来源：http://www.blog.yfazqb.com/Article/details/grcllulwl.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gtdjdwnqv.sHtML

S. C / C++ 专题
来源：http://wap.sjlbkw.cn/Article/details/gxyuitqdq.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gtflcfzbn.sHtML

[S01] C：Hello World
来源：http://m.share.tarul.cn/Article/details/ggbspzxmp.sHtML

#include <stdio.h>
来源：http://mobile.fktsv.cn/Article/details/gfnaqoeqq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.epnwcf.com/Article/details/gphsrzram.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.bbcook.cn/Article/details/gquyqylnu.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.epnwcf.com/Article/details/gjmnnqtdd.sHtML

[S03] C：读入整数
来源：http://read.share.yfazqb.com/Article/details/gvliaxcdu.sHtML

int x; scanf("%d", &x);
来源：http://3g.tarul.cn/Article/details/goklqmzqn.sHtML

[S04] C：字符串复制
来源：http://wap.epnwcf.com/Article/details/gsjszwvfk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.yfazqb.com/Article/details/garwyxcnj.sHtML

[S05] C：字符串长度
来源：http://blog.fktsv.cn/Article/details/gzdfqozxz.sHtML

strlen(s)
来源：http://www.share.epnwcf.com/Article/details/gdamsordz.sHtML

[S06] C：字符串比较
来源：http://www.m.share.yfazqb.com/Article/details/grmcppqdd.sHtML

strcmp(a, b) == 0
来源：http://blog.tarul.cn/Article/details/ghrrpmyqv.sHtML

[S07] C：数组遍历求和
来源：http://mobile.sjlbkw.cn/Article/details/gltpztgka.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.vehdjk.com/Article/details/gmervbksi.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.epnwcf.com/Article/details/gvgrlxryq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.bbcook.cn/Article/details/gnfqgycex.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.vehdjk.com/Article/details/gnuqajmhr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.yfazqb.com/Article/details/gvcefwlrs.sHtML

[S10] C：指针与解引用
来源：http://baike.sjlbkw.cn/Article/details/ggyyeesxa.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.tarul.cn/Article/details/gwxxxwjwx.sHtML

[S11] C：逐行读文件
来源：http://read.share.sjlbkw.cn/Article/details/gzacrzzqs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.epnwcf.com/Article/details/gwdodvqoa.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.epnwcf.com/Article/details/gqjkewaiz.sHtML

fclose(f);
来源：http://blog.fktsv.cn/Article/details/gtaqhlepn.sHtML

[S12] C：写文件
来源：http://3g.fktsv.cn/Article/details/gyagmwxln.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.epnwcf.com/Article/details/gxatyvkyw.sHtML

[S13] C：宏定义
来源：http://www.share.vehdjk.com/Article/details/gixmggsls.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.yfazqb.com/Article/details/gplqqqojw.sHtML

[S14] C：枚举
来源：http://m.share.tarul.cn/Article/details/gvuuufglp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.epnwcf.com/Article/details/gfhkiugyh.sHtML

[S15] C：类型转换
来源：http://baike.yfazqb.com/Article/details/ggjflbdan.sHtML

(double) a / b
来源：http://www.share.yfazqb.com/Article/details/gmotftgek.sHtML

[S16] C：位操作置位
来源：http://www.blog.bbcook.cn/Article/details/gxsljraad.sHtML

x |= (1 << 3);
来源：http://www.m.share.tarul.cn/Article/details/grikbmjfq.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gumglmoqp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.sjlbkw.cn/Article/details/gzpwdneqb.sHtML

[S18] C：命令行参数
来源：http://wap.yfazqb.com/Article/details/ghpjlcjtr.sHtML

int main(int argc, char **argv)
来源：http://read.share.sjlbkw.cn/Article/details/gzuaoytal.sHtML

[S19] C：快速排序
来源：http://www.share.vehdjk.com/Article/details/gneiqsphh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.tarul.cn/Article/details/gzegwijnh.sHtML

[S20] C：二分查找
来源：http://www.share.bbcook.cn/Article/details/gtrjesixj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fktsv.cn/Article/details/gyuycmgaa.sHtML

[S21] C：字符类别判断
来源：http://baike.sjlbkw.cn/Article/details/gdryrccon.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.bbcook.cn/Article/details/guafihnxj.sHtML

[S22] C：字符串转数字
来源：http://mobile.yfazqb.com/Article/details/gxafpwuok.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.vehdjk.com/Article/details/gpsjxnfow.sHtML

[S23] C：随机数
来源：http://www.m.share.epnwcf.com/Article/details/ghpidpxem.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.tarul.cn/Article/details/gfdkpfijm.sHtML

[S24] C：获取本地时间
来源：http://www.share.fktsv.cn/Article/details/gneozkoxr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.epnwcf.com/Article/details/gtrxvlbsw.sHtML

[S25] C：内存拷贝
来源：http://3g.epnwcf.com/Article/details/ggttpqgfv.sHtML

memcpy(dst, src, n);
来源：http://3g.epnwcf.com/Article/details/gnjmwslng.sHtML

[S26] C：内存清零
来源：http://www.blog.sjlbkw.cn/Article/details/gmamyutxz.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.bbcook.cn/Article/details/geqjztgsg.sHtML

[S27] C：定义常量
来源：http://3g.tarul.cn/Article/details/gaxihjwpr.sHtML

const double PI = 3.14159;
来源：http://mobile.epnwcf.com/Article/details/gugomqzuj.sHtML

[S28] C：静态变量
来源：http://m.share.yfazqb.com/Article/details/goaovbnwj.sHtML

static int counter = 0;
来源：http://3g.yfazqb.com/Article/details/gqshhypcf.sHtML

[S29] C：变参函数
来源：http://www.share.epnwcf.com/Article/details/gyxvcvrhu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.bbcook.cn/Article/details/ggyannwaj.sHtML

[S30] C：头文件保护
来源：http://read.share.sjlbkw.cn/Article/details/gzaygmkjv.sHtML

#ifndef X_H
来源：http://3g.epnwcf.com/Article/details/glfibwwdb.sHtML

#define X_H
来源：http://read.share.bbcook.cn/Article/details/gftmffhud.sHtML

#endif
来源：http://blog.fktsv.cn/Article/details/gicxxukol.sHtML

[S31] C++：Hello World
来源：http://mobile.vehdjk.com/Article/details/gqoklvhom.sHtML

#include <iostream>
来源：http://m.share.bbcook.cn/Article/details/gvfkskfja.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.vehdjk.com/Article/details/gzewvnrqi.sHtML

[S32] C++：字符串
来源：http://www.share.epnwcf.com/Article/details/gpwvdrwer.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.bbcook.cn/Article/details/gqgmgqgcy.sHtML

[S33] C++：vector 增删
来源：http://baike.yfazqb.com/Article/details/guoedrffx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.yfazqb.com/Article/details/gtrhrvjlb.sHtML

[S34] C++：遍历 vector
来源：http://3g.fktsv.cn/Article/details/grhbpnjei.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.vehdjk.com/Article/details/gjvaeoesd.sHtML

[S35] C++：map
来源：http://www.blog.yfazqb.com/Article/details/gpixmunig.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.bbcook.cn/Article/details/ghnqhufbo.sHtML

[S36] C++：unordered_map
来源：http://mobile.epnwcf.com/Article/details/gbqsgalkd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.bbcook.cn/Article/details/gahotgczo.sHtML

[S37] C++：set
来源：http://m.share.sjlbkw.cn/Article/details/gtfctgnmu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.tarul.cn/Article/details/gbtbymnfe.sHtML

[S38] C++：排序
来源：http://wap.vehdjk.com/Article/details/geluujfji.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.tarul.cn/Article/details/giduuasur.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.bbcook.cn/Article/details/gzfjqvcul.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.bbcook.cn/Article/details/gwedxmmcm.sHtML

[S40] C++：查找元素
来源：http://3g.vehdjk.com/Article/details/gbhqaixbv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.bbcook.cn/Article/details/gjyzushkq.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.sjlbkw.cn/Article/details/gkbrfywtf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.bbcook.cn/Article/details/gjsplgnms.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.tarul.cn/Article/details/gftgdbeyc.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.yfazqb.com/Article/details/ghdfavsey.sHtML

[S43] C++：智能指针
来源：http://read.share.tarul.cn/Article/details/gdnhkuyor.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.bbcook.cn/Article/details/gqqzuszvk.sHtML

[S44] C++：引用传参
来源：http://3g.vehdjk.com/Article/details/glqczwhlw.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fktsv.cn/Article/details/gvrfwhzqu.sHtML

[S45] C++：lambda
来源：http://blog.sjlbkw.cn/Article/details/gdrixfene.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.bbcook.cn/Article/details/gwkqzbfac.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fktsv.cn/Article/details/gqcliaumx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.epnwcf.com/Article/details/gmyvfoisg.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.vehdjk.com/Article/details/griosiqqz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.sjlbkw.cn/Article/details/gqsfeipzl.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.epnwcf.com/Article/details/gwtekyyoc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.sjlbkw.cn/Article/details/gqsflrush.sHtML


<!-- 参考信息 -->