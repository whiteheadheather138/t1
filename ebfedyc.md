代发 wailian999

[Q78] 当前时间
来源：http://www.m.share.yfazqb.com/Article/details/gbyaguuai.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.tarul.cn/Article/details/gjzkcdfvr.sHtML

[Q79] 字符串拼接
来源：http://read.share.tarul.cn/Article/details/ggeklcsvu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.sjlbkw.cn/Article/details/gyjrlicbl.sHtML

[Q80] 字符串截取
来源：http://www.m.share.sjlbkw.cn/Article/details/gvqpqofdw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gubvlndbl.sHtML

[Q81] 字符串替换
来源：http://mobile.vehdjk.com/Article/details/gtegkqdod.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.bbcook.cn/Article/details/gfziqvqoi.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.bbcook.cn/Article/details/gopbtqwuw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/grnoajmrq.sHtML

[Q83] 大小写转换
来源：http://read.share.epnwcf.com/Article/details/gtgkqcyhx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.tarul.cn/Article/details/ganjlfwwh.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.sjlbkw.cn/Article/details/gtfqzlbxe.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fktsv.cn/Article/details/grurxaopt.sHtML

[Q85] 数值取整
来源：http://mobile.bbcook.cn/Article/details/gybgilxua.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.epnwcf.com/Article/details/guzvrqote.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.tarul.cn/Article/details/gchhokjcf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.vehdjk.com/Article/details/gjjnoiwol.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fktsv.cn/Article/details/gaaznieqw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.tarul.cn/Article/details/gqiaopjnk.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.bbcook.cn/Article/details/guabhnkxz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.bbcook.cn/Article/details/ggqkjripd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gvbfaovlc.sHtML

[Q89] 判断表是否存在
来源：http://read.share.tarul.cn/Article/details/gshyvxttm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.vehdjk.com/Article/details/guxrrrclk.sHtML

[Q90] 生成序号列
来源：http://read.share.bbcook.cn/Article/details/gxhdycvkg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.tarul.cn/Article/details/geqtihrlk.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gfrvtocrp.sHtML

R. Bash 专题
来源：http://m.share.sjlbkw.cn/Article/details/gkdsqdfge.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gcebiykjn.sHtML

[R01] shebang 与严格模式
来源：http://m.share.tarul.cn/Article/details/gedilvpem.sHtML

#!/usr/bin/env bash
来源：http://www.share.tarul.cn/Article/details/gkssizzgt.sHtML

set -euo pipefail
来源：http://m.share.bbcook.cn/Article/details/grrmgfhik.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fktsv.cn/Article/details/gwjsdjuan.sHtML

name="Tom"; echo "$name"
来源：http://m.share.sjlbkw.cn/Article/details/gvccnprdw.sHtML

[R03] 只读变量
来源：http://3g.tarul.cn/Article/details/gvtvbajgd.sHtML

readonly PI=3.14
来源：http://read.share.tarul.cn/Article/details/gzzkqvvcu.sHtML

[R04] 位置参数
来源：http://blog.sjlbkw.cn/Article/details/gwyyxxcwn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.tarul.cn/Article/details/gmiyxnszo.sHtML

[R05] 参数默认值
来源：http://m.share.fktsv.cn/Article/details/geyqlyibd.sHtML

name="${1:-default}"
来源：http://mobile.fktsv.cn/Article/details/gzjkheytm.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.tarul.cn/Article/details/gzoxpmdjs.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.vehdjk.com/Article/details/gevmdxfdh.sHtML

[R07] if 判断文件
来源：http://www.share.vehdjk.com/Article/details/gwtrmivtp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.vehdjk.com/Article/details/gdgxoqzzy.sHtML

[R08] 数值比较
来源：http://www.m.share.epnwcf.com/Article/details/gaejtmkuc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fktsv.cn/Article/details/gcvgaljao.sHtML

[R09] 字符串比较
来源：http://www.m.share.fktsv.cn/Article/details/gvqmxbvpb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.sjlbkw.cn/Article/details/gfgdypefg.sHtML

[R10] 正则匹配
来源：http://blog.epnwcf.com/Article/details/gcovjflln.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.epnwcf.com/Article/details/gkckgyzjd.sHtML

[R11] case 多分支
来源：http://baike.sjlbkw.cn/Article/details/gfvgckvmg.sHtML

case "$1" in
来源：http://www.share.sjlbkw.cn/Article/details/govtvqkzh.sHtML

start) echo "启动" ;;
来源：http://baike.tarul.cn/Article/details/gxgwzxtak.sHtML

stop)  echo "停止" ;;
来源：http://read.share.bbcook.cn/Article/details/gseuqcmso.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.bbcook.cn/Article/details/gmsovkcke.sHtML

esac
来源：http://blog.yfazqb.com/Article/details/gpzyfskal.sHtML

[R12] for 遍历文件
来源：http://www.share.sjlbkw.cn/Article/details/gwajlioyd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.tarul.cn/Article/details/ggqixmlme.sHtML

[R13] for 计数循环
来源：http://www.blog.fktsv.cn/Article/details/gvzyzmewm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.sjlbkw.cn/Article/details/gcjxyvleq.sHtML

[R14] C 风格 for
来源：http://blog.vehdjk.com/Article/details/gmdaqlyxn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.bbcook.cn/Article/details/gntbivbjb.sHtML

[R15] while 逐行读文件
来源：http://baike.bbcook.cn/Article/details/grupnfepi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fktsv.cn/Article/details/gunnircjc.sHtML

[R16] until 等待条件
来源：http://m.share.tarul.cn/Article/details/geypjpolf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.yfazqb.com/Article/details/guwdspket.sHtML

[R17] 数组定义与取值
来源：http://m.share.vehdjk.com/Article/details/gwmakbxbv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.epnwcf.com/Article/details/glunedrtb.sHtML

[R18] 遍历数组
来源：http://read.share.bbcook.cn/Article/details/gtfgwdluz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.yfazqb.com/Article/details/gzdwbfotq.sHtML

[R19] 数组长度
来源：http://www.blog.sjlbkw.cn/Article/details/gibeczsxg.sHtML

echo "${#arr[@]}"
来源：http://baike.sjlbkw.cn/Article/details/guupsnxts.sHtML

[R20] 关联数组（字典）
来源：http://wap.fktsv.cn/Article/details/gewhfdlck.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.tarul.cn/Article/details/gsjdyxrtv.sHtML

[R21] 字符串长度
来源：http://wap.bbcook.cn/Article/details/giwdjfauh.sHtML

echo "${#s}"
来源：http://m.share.fktsv.cn/Article/details/gdujpsgks.sHtML

[R22] 截取子串
来源：http://3g.sjlbkw.cn/Article/details/getvyrrto.sHtML

echo "${s:0:5}"
来源：http://baike.epnwcf.com/Article/details/gikcguxiz.sHtML

[R23] 字符串替换
来源：http://www.m.share.fktsv.cn/Article/details/gnaxqyvcp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.bbcook.cn/Article/details/ggmtlujkc.sHtML

[R24] 大小写转换
来源：http://www.blog.vehdjk.com/Article/details/godznspxr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.bbcook.cn/Article/details/ghrokxuux.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.tarul.cn/Article/details/gygaomzlt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.vehdjk.com/Article/details/gnwwecwrd.sHtML

[R26] 命令替换
来源：http://blog.epnwcf.com/Article/details/gdifdetzf.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.tarul.cn/Article/details/gzgwiabrd.sHtML

[R27] 算术展开
来源：http://3g.fktsv.cn/Article/details/gsnxeggfh.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.vehdjk.com/Article/details/gwheowgkd.sHtML

[R28] 浮点运算
来源：http://read.share.sjlbkw.cn/Article/details/giomuctjg.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.epnwcf.com/Article/details/gdaeovjzj.sHtML

[R29] 定义函数
来源：http://www.share.yfazqb.com/Article/details/gjnbvpcnf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fktsv.cn/Article/details/guxxcpygg.sHtML

[R30] 函数返回状态码
来源：http://blog.epnwcf.com/Article/details/gubonitum.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.vehdjk.com/Article/details/gxojrzvjp.sHtML

[R31] 局部变量
来源：http://3g.sjlbkw.cn/Article/details/gugonyvvu.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.bbcook.cn/Article/details/gurgqpkco.sHtML

[R32] 参数个数校验
来源：http://baike.bbcook.cn/Article/details/gjncyznpr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.yfazqb.com/Article/details/grohuogzl.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.bbcook.cn/Article/details/ggvboggyi.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.tarul.cn/Article/details/gjogvvqwh.sHtML

[R34] 退出时清理
来源：http://mobile.yfazqb.com/Article/details/gshgqutyt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.yfazqb.com/Article/details/gsyxwanrj.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.yfazqb.com/Article/details/gyvnlitfv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.epnwcf.com/Article/details/gekhfhtzz.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.tarul.cn/Article/details/gmoqlgzbw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.tarul.cn/Article/details/gbtkxvxxw.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fktsv.cn/Article/details/ggmlymxnt.sHtML

files=$(ls -1)
来源：http://m.share.epnwcf.com/Article/details/gqqsdotju.sHtML

[R38] 管道串联
来源：http://wap.sjlbkw.cn/Article/details/ghintmnno.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fktsv.cn/Article/details/gcfbnrreu.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.vehdjk.com/Article/details/gkjertelw.sHtML

cmd > out.log 2>&1
来源：http://m.share.tarul.cn/Article/details/ghzfdfimy.sHtML

[R40] 追加写日志
来源：http://3g.sjlbkw.cn/Article/details/gjgwmzbfk.sHtML

echo "log" >> out.log
来源：http://www.blog.vehdjk.com/Article/details/gjciswnkm.sHtML

[R41] 丢弃输出
来源：http://blog.tarul.cn/Article/details/gdtetdysk.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.epnwcf.com/Article/details/gxzqhlhlr.sHtML

[R42] 输入重定向
来源：http://www.m.share.tarul.cn/Article/details/ggoobpatc.sHtML

wc -l < a.txt
来源：http://m.share.vehdjk.com/Article/details/ghrwfksts.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.epnwcf.com/Article/details/grtfitzgo.sHtML

find . -name "*.log" -type f
来源：http://read.share.vehdjk.com/Article/details/gzxpotqmf.sHtML

[R44] 按修改时间查找
来源：http://wap.tarul.cn/Article/details/guzytnhka.sHtML

find . -mtime -7 -type f
来源：http://baike.sjlbkw.cn/Article/details/gtlgvspvn.sHtML

[R45] 批量删除
来源：http://baike.fktsv.cn/Article/details/gdqgfhojr.sHtML

find . -name "*.tmp" -delete
来源：http://baike.epnwcf.com/Article/details/gowztcfhq.sHtML

[R46] 递归替换文件内容
来源：http://m.share.sjlbkw.cn/Article/details/gbufovwpg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.vehdjk.com/Article/details/gdfwtmcot.sHtML

[R47] sed 单行替换
来源：http://www.blog.sjlbkw.cn/Article/details/gopgpuedu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.bbcook.cn/Article/details/gmqbscjwd.sHtML

[R48] awk 取指定列
来源：http://mobile.vehdjk.com/Article/details/gtrkiseoe.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.epnwcf.com/Article/details/ggnjvugae.sHtML

[R49] awk 带条件
来源：http://m.share.tarul.cn/Article/details/gpkynclmm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.yfazqb.com/Article/details/gumpjdpvy.sHtML

[R50] awk 求和
来源：http://read.share.sjlbkw.cn/Article/details/gqcrcfues.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.epnwcf.com/Article/details/gqpdsrgfl.sHtML

[R51] 排序去重取前几
来源：http://mobile.fktsv.cn/Article/details/gxfjoaqpg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fktsv.cn/Article/details/geibkdeck.sHtML

[R52] 统计行数
来源：http://wap.epnwcf.com/Article/details/glhlhlcap.sHtML

wc -l a.txt
来源：http://3g.epnwcf.com/Article/details/gkqqzzeab.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.sjlbkw.cn/Article/details/gehkdbivl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.epnwcf.com/Article/details/grebrltaf.sHtML

[R54] 比较两个文件
来源：http://baike.fktsv.cn/Article/details/gvfokmoju.sHtML

diff a.txt b.txt
来源：http://wap.fktsv.cn/Article/details/gwoeovcjd.sHtML

[R55] 压缩与解压
来源：http://read.share.fktsv.cn/Article/details/ggnchwpgf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.yfazqb.com/Article/details/guoystktr.sHtML

[R56] 远程拷贝
来源：http://3g.sjlbkw.cn/Article/details/gtewutuxs.sHtML

scp file user@host:/path/
来源：http://3g.epnwcf.com/Article/details/geyxmdqpb.sHtML

[R57] 远程执行命令
来源：http://mobile.vehdjk.com/Article/details/giosqvflk.sHtML

ssh user@host 'uptime'
来源：http://www.blog.yfazqb.com/Article/details/gfdtoiryc.sHtML

[R58] 下载文件
来源：http://mobile.fktsv.cn/Article/details/guwufebwa.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.sjlbkw.cn/Article/details/gijskrfzg.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.sjlbkw.cn/Article/details/gvygwiznu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.epnwcf.com/Article/details/gglyvyjyh.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fktsv.cn/Article/details/gwbrzjfbj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.epnwcf.com/Article/details/gzdicclwa.sHtML

[R61] 磁盘占用
来源：http://www.m.share.epnwcf.com/Article/details/gkdmllydg.sHtML

df -h;  du -sh *
来源：http://www.m.share.bbcook.cn/Article/details/glvljayjo.sHtML

[R62] 找最占空间的文件
来源：http://baike.fktsv.cn/Article/details/gzwjoiinc.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.yfazqb.com/Article/details/gzmorncye.sHtML

[R63] 内存与进程
来源：http://www.share.vehdjk.com/Article/details/gxrijslqi.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.bbcook.cn/Article/details/gbsejmalt.sHtML

[R64] 结束进程
来源：http://www.m.share.bbcook.cn/Article/details/gvjfogudx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fktsv.cn/Article/details/gnbwetayf.sHtML

[R65] 查看端口占用
来源：http://baike.yfazqb.com/Article/details/gyrexgrjj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.sjlbkw.cn/Article/details/gftkgrnaq.sHtML

[R66] 定时任务
来源：http://3g.bbcook.cn/Article/details/gxjflkopz.sHtML

crontab -e;  crontab -l
来源：http://www.share.epnwcf.com/Article/details/gwcgvosbr.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.vehdjk.com/Article/details/gyzsvdgvt.sHtML

openssl rand -hex 16
来源：http://www.blog.vehdjk.com/Article/details/gdifxlnhz.sHtML

[R68] 计算文件校验值
来源：http://3g.sjlbkw.cn/Article/details/gsnhkyfqp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.vehdjk.com/Article/details/gzawfpuru.sHtML

[R69] 生成随机密码
来源：http://read.share.bbcook.cn/Article/details/gxzixkmii.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.bbcook.cn/Article/details/grocgvlul.sHtML

[R70] 时间戳与互转
来源：http://www.share.fktsv.cn/Article/details/gqzckgkny.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.vehdjk.com/Article/details/gocjxxada.sHtML

[R71] 日期格式化
来源：http://baike.yfazqb.com/Article/details/gwgfvplqz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fktsv.cn/Article/details/gplqwjdyn.sHtML

[R72] 等待端口就绪
来源：http://m.share.bbcook.cn/Article/details/gopegoxex.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.sjlbkw.cn/Article/details/gvntvpyzz.sHtML

[R73] 分割大日志
来源：http://read.share.epnwcf.com/Article/details/gkdslfmlb.sHtML

split -l 1000 big.log part_
来源：http://m.share.yfazqb.com/Article/details/gokdplyyx.sHtML

[R74] 批量重命名
来源：http://www.blog.tarul.cn/Article/details/gxmcvbowg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.epnwcf.com/Article/details/graqbuvqn.sHtML

[R75] 导出环境变量
来源：http://www.share.bbcook.cn/Article/details/gwzwzllct.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.tarul.cn/Article/details/ggfutdfwp.sHtML

[R76] 使用临时文件
来源：http://mobile.bbcook.cn/Article/details/gkjqxsjmd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fktsv.cn/Article/details/grtqenbvn.sHtML

[R77] 读取用户输入
来源：http://m.share.yfazqb.com/Article/details/gddgmqzle.sHtML

read -rp "请输入: " ans
来源：http://wap.vehdjk.com/Article/details/gmljwpooi.sHtML

[R78] 交互式菜单
来源：http://baike.tarul.cn/Article/details/gyookvzhp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.sjlbkw.cn/Article/details/gjsttaauh.sHtML

[R79] 解析命令行选项
来源：http://www.share.yfazqb.com/Article/details/glqzgcayo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.yfazqb.com/Article/details/gpihzjreh.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.yfazqb.com/Article/details/gbulybvri.sHtML

time ./run.sh
来源：http://read.share.yfazqb.com/Article/details/gucyofxex.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/ggecogkft.sHtML

S. C / C++ 专题
来源：http://baike.yfazqb.com/Article/details/gvyketujd.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gzlbgckka.sHtML

[S01] C：Hello World
来源：http://m.share.epnwcf.com/Article/details/gbnmwdhyi.sHtML

#include <stdio.h>
来源：http://www.m.share.bbcook.cn/Article/details/gaptegfwp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.tarul.cn/Article/details/gvmefayks.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.bbcook.cn/Article/details/gercqwtpb.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.vehdjk.com/Article/details/gnbhxpzgq.sHtML

[S03] C：读入整数
来源：http://m.share.fktsv.cn/Article/details/gyrgilvwc.sHtML

int x; scanf("%d", &x);
来源：http://blog.epnwcf.com/Article/details/ghhwiqsjl.sHtML

[S04] C：字符串复制
来源：http://m.share.vehdjk.com/Article/details/gyppvhxta.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.sjlbkw.cn/Article/details/gojelfsyj.sHtML

[S05] C：字符串长度
来源：http://wap.sjlbkw.cn/Article/details/gkvnapgxb.sHtML

strlen(s)
来源：http://www.m.share.tarul.cn/Article/details/gsbkksxdy.sHtML

[S06] C：字符串比较
来源：http://mobile.epnwcf.com/Article/details/gsupnmbtg.sHtML

strcmp(a, b) == 0
来源：http://wap.sjlbkw.cn/Article/details/ghlwzplkd.sHtML

[S07] C：数组遍历求和
来源：http://wap.sjlbkw.cn/Article/details/gtnyolequ.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.sjlbkw.cn/Article/details/ganqublwi.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.yfazqb.com/Article/details/gwopntjfb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fktsv.cn/Article/details/gzgnmspbm.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.bbcook.cn/Article/details/gleuyrdxz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.bbcook.cn/Article/details/gqgvxmunv.sHtML

[S10] C：指针与解引用
来源：http://baike.bbcook.cn/Article/details/gtgugdsry.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.yfazqb.com/Article/details/gvtkfizbo.sHtML

[S11] C：逐行读文件
来源：http://wap.bbcook.cn/Article/details/gqbqzsrrf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.yfazqb.com/Article/details/gwarqvszf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.bbcook.cn/Article/details/gwcymghtp.sHtML

fclose(f);
来源：http://m.share.yfazqb.com/Article/details/gpltlezrg.sHtML

[S12] C：写文件
来源：http://www.blog.fktsv.cn/Article/details/gsfzfcdtp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.yfazqb.com/Article/details/gbrejpofb.sHtML

[S13] C：宏定义
来源：http://www.m.share.bbcook.cn/Article/details/gvglhzfkh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.yfazqb.com/Article/details/gkdkdifoy.sHtML

[S14] C：枚举
来源：http://m.share.vehdjk.com/Article/details/gdexjwvom.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.vehdjk.com/Article/details/gpnvlxoog.sHtML

[S15] C：类型转换
来源：http://wap.vehdjk.com/Article/details/gxblxwowh.sHtML

(double) a / b
来源：http://baike.bbcook.cn/Article/details/gdyybxbez.sHtML

[S16] C：位操作置位
来源：http://www.blog.fktsv.cn/Article/details/gxgygztny.sHtML

x |= (1 << 3);
来源：http://blog.sjlbkw.cn/Article/details/gavjnpnvb.sHtML

[S17] C：安全拼接字符串
来源：http://3g.tarul.cn/Article/details/gbjbczxep.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.tarul.cn/Article/details/gmccwdxys.sHtML

[S18] C：命令行参数
来源：http://mobile.fktsv.cn/Article/details/gxbtpwthz.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fktsv.cn/Article/details/geapcqqgt.sHtML

[S19] C：快速排序
来源：http://wap.vehdjk.com/Article/details/gsilpfoik.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.bbcook.cn/Article/details/gkcnbnrbd.sHtML

[S20] C：二分查找
来源：http://baike.tarul.cn/Article/details/gcogcqfod.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.vehdjk.com/Article/details/gzslwrgrs.sHtML

[S21] C：字符类别判断
来源：http://wap.epnwcf.com/Article/details/gbzorfhda.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.sjlbkw.cn/Article/details/gujyunnjx.sHtML

[S22] C：字符串转数字
来源：http://m.share.vehdjk.com/Article/details/gnofljvso.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fktsv.cn/Article/details/gqxsiaiep.sHtML

[S23] C：随机数
来源：http://wap.fktsv.cn/Article/details/gojejspce.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.bbcook.cn/Article/details/gbkzjzbgq.sHtML

[S24] C：获取本地时间
来源：http://www.share.sjlbkw.cn/Article/details/gopycthwi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.yfazqb.com/Article/details/giqdmlmyo.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fktsv.cn/Article/details/gxhconwlk.sHtML

memcpy(dst, src, n);
来源：http://m.share.yfazqb.com/Article/details/gfipmlfth.sHtML

[S26] C：内存清零
来源：http://www.blog.yfazqb.com/Article/details/gkkdkbxbv.sHtML

memset(a, 0, sizeof a);
来源：http://3g.bbcook.cn/Article/details/gvtpqbtja.sHtML

[S27] C：定义常量
来源：http://www.m.share.epnwcf.com/Article/details/giirdjiga.sHtML

const double PI = 3.14159;
来源：http://read.share.bbcook.cn/Article/details/gofrsyiph.sHtML

[S28] C：静态变量
来源：http://read.share.sjlbkw.cn/Article/details/gkscidgyi.sHtML

static int counter = 0;
来源：http://www.blog.epnwcf.com/Article/details/gazxlvacv.sHtML

[S29] C：变参函数
来源：http://blog.epnwcf.com/Article/details/gmjrjqqcp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.tarul.cn/Article/details/gzywtjlif.sHtML

[S30] C：头文件保护
来源：http://www.share.vehdjk.com/Article/details/gdvbpjgql.sHtML

#ifndef X_H
来源：http://www.m.share.tarul.cn/Article/details/gbsmviyqf.sHtML

#define X_H
来源：http://m.share.vehdjk.com/Article/details/gowtaditj.sHtML

#endif
来源：http://www.blog.tarul.cn/Article/details/gzuhuiqea.sHtML

[S31] C++：Hello World
来源：http://blog.tarul.cn/Article/details/gfwaqvyez.sHtML

#include <iostream>
来源：http://read.share.bbcook.cn/Article/details/guvkvelfs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.yfazqb.com/Article/details/gnmhpplbc.sHtML

[S32] C++：字符串
来源：http://mobile.sjlbkw.cn/Article/details/gamclpept.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.sjlbkw.cn/Article/details/gglnmtocw.sHtML

[S33] C++：vector 增删
来源：http://wap.fktsv.cn/Article/details/goadktetz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.sjlbkw.cn/Article/details/gbvsaqpnv.sHtML

[S34] C++：遍历 vector
来源：http://m.share.bbcook.cn/Article/details/gihdjtwjk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.epnwcf.com/Article/details/ggpnyfbkx.sHtML

[S35] C++：map
来源：http://m.share.vehdjk.com/Article/details/glpbaurxz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.vehdjk.com/Article/details/gbsdtaros.sHtML

[S36] C++：unordered_map
来源：http://m.share.yfazqb.com/Article/details/ghlwlpote.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gjrkxnbcp.sHtML

[S37] C++：set
来源：http://www.m.share.epnwcf.com/Article/details/gfykxzwbq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.epnwcf.com/Article/details/gqiyqxazd.sHtML

[S38] C++：排序
来源：http://blog.sjlbkw.cn/Article/details/gmtfshilq.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.bbcook.cn/Article/details/gippfjsmt.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.vehdjk.com/Article/details/gvhhkhuqe.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fktsv.cn/Article/details/gtshqamvl.sHtML

[S40] C++：查找元素
来源：http://www.blog.fktsv.cn/Article/details/gmafwxxdf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.tarul.cn/Article/details/gjvepzsjp.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.sjlbkw.cn/Article/details/gwivpgbrr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.tarul.cn/Article/details/gfcxfulpg.sHtML

[S42] C++：继承与虚函数
来源：http://3g.sjlbkw.cn/Article/details/gsnsygxpt.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.vehdjk.com/Article/details/gtabdvyjd.sHtML

[S43] C++：智能指针
来源：http://www.share.vehdjk.com/Article/details/gtudqmovk.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.yfazqb.com/Article/details/goljuvnuu.sHtML

[S44] C++：引用传参
来源：http://www.share.bbcook.cn/Article/details/gwsebdjoq.sHtML

void inc(int &x) { ++x; }
来源：http://blog.bbcook.cn/Article/details/gqbyngnun.sHtML

[S45] C++：lambda
来源：http://mobile.sjlbkw.cn/Article/details/gmkwzieas.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fktsv.cn/Article/details/gcergvoqm.sHtML

[S46] C++：函数模板
来源：http://wap.yfazqb.com/Article/details/gwmaeohjz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fktsv.cn/Article/details/girnyonbq.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.vehdjk.com/Article/details/gqgkumuai.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.epnwcf.com/Article/details/gorluytlb.sHtML

[S48] C++：逐行读文件
来源：http://read.share.bbcook.cn/Article/details/gmbstdioo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.tarul.cn/Article/details/gvaqkpjvs.sHtML


<!-- 参考信息 -->