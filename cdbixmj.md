代发 wailian999

[Q82] 字符长度与字节长度
来源：http://blog.vehdjk.com/Article/details/gikkhkoqy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.vehdjk.com/Article/details/gsvatrtzm.sHtML

[Q83] 大小写转换
来源：http://www.m.share.tarul.cn/Article/details/gggqvikbp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.yfazqb.com/Article/details/gxbdfbsdt.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fktsv.cn/Article/details/gpgymzcfv.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.bbcook.cn/Article/details/gnurxvbpi.sHtML

[Q85] 数值取整
来源：http://wap.epnwcf.com/Article/details/gtkkapsoz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.bbcook.cn/Article/details/guvpdslvd.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.vehdjk.com/Article/details/gbhigiadv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fktsv.cn/Article/details/gxvtukvfx.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.bbcook.cn/Article/details/gxavdntsb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fktsv.cn/Article/details/gmaqlpvnq.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.yfazqb.com/Article/details/gqffxdwfr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fktsv.cn/Article/details/gefwdsoxr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.bbcook.cn/Article/details/ggpgbzotc.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fktsv.cn/Article/details/gigbykyvk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.vehdjk.com/Article/details/geyvknily.sHtML

[Q90] 生成序号列
来源：http://read.share.fktsv.cn/Article/details/gcxwunima.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.bbcook.cn/Article/details/giaihixti.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gadozwosh.sHtML

R. Bash 专题
来源：http://m.share.epnwcf.com/Article/details/gezgwvmtd.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gcfffnoru.sHtML

[R01] shebang 与严格模式
来源：http://read.share.sjlbkw.cn/Article/details/gafyawyah.sHtML

#!/usr/bin/env bash
来源：http://www.blog.sjlbkw.cn/Article/details/gcywqgkvh.sHtML

set -euo pipefail
来源：http://wap.epnwcf.com/Article/details/glywprxnq.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fktsv.cn/Article/details/gainmjhoh.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.bbcook.cn/Article/details/gfgskcodu.sHtML

[R03] 只读变量
来源：http://www.blog.fktsv.cn/Article/details/gorbbcvtu.sHtML

readonly PI=3.14
来源：http://www.blog.tarul.cn/Article/details/gitaotade.sHtML

[R04] 位置参数
来源：http://www.share.vehdjk.com/Article/details/gvzkemjza.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.bbcook.cn/Article/details/gelziibbx.sHtML

[R05] 参数默认值
来源：http://www.share.yfazqb.com/Article/details/gdajyxbzx.sHtML

name="${1:-default}"
来源：http://m.share.epnwcf.com/Article/details/gmolvmwap.sHtML

[R06] 判断命令是否存在
来源：http://read.share.epnwcf.com/Article/details/gwswraavn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.yfazqb.com/Article/details/gicejytaw.sHtML

[R07] if 判断文件
来源：http://read.share.vehdjk.com/Article/details/glypjtriy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.sjlbkw.cn/Article/details/gajvggwrx.sHtML

[R08] 数值比较
来源：http://wap.tarul.cn/Article/details/gnmeoppem.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.sjlbkw.cn/Article/details/glwmjdozs.sHtML

[R09] 字符串比较
来源：http://read.share.fktsv.cn/Article/details/gjwsxvadb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.sjlbkw.cn/Article/details/gpjoedlva.sHtML

[R10] 正则匹配
来源：http://baike.yfazqb.com/Article/details/ggmyutbgy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.vehdjk.com/Article/details/gcffvpuqj.sHtML

[R11] case 多分支
来源：http://wap.vehdjk.com/Article/details/gittrrffw.sHtML

case "$1" in
来源：http://www.share.yfazqb.com/Article/details/gvldaxdlv.sHtML

start) echo "启动" ;;
来源：http://3g.tarul.cn/Article/details/goodnztae.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.vehdjk.com/Article/details/goauoidje.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.bbcook.cn/Article/details/gksduckya.sHtML

esac
来源：http://3g.vehdjk.com/Article/details/gzznwrwpp.sHtML

[R12] for 遍历文件
来源：http://wap.epnwcf.com/Article/details/gdrygrirn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.sjlbkw.cn/Article/details/gfimcynlb.sHtML

[R13] for 计数循环
来源：http://read.share.bbcook.cn/Article/details/gqdedbbpd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.sjlbkw.cn/Article/details/gjztumhkl.sHtML

[R14] C 风格 for
来源：http://www.blog.vehdjk.com/Article/details/gegqnrhce.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.yfazqb.com/Article/details/geqxcyrqx.sHtML

[R15] while 逐行读文件
来源：http://mobile.bbcook.cn/Article/details/gbnaavevr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.epnwcf.com/Article/details/gtslbjoqn.sHtML

[R16] until 等待条件
来源：http://www.share.sjlbkw.cn/Article/details/goxyjhyzt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.vehdjk.com/Article/details/gjcbglxca.sHtML

[R17] 数组定义与取值
来源：http://wap.tarul.cn/Article/details/gzoezebee.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.epnwcf.com/Article/details/gvxkydqtf.sHtML

[R18] 遍历数组
来源：http://mobile.tarul.cn/Article/details/gzerrbutx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fktsv.cn/Article/details/ghqirdpcy.sHtML

[R19] 数组长度
来源：http://read.share.vehdjk.com/Article/details/gchvhluzy.sHtML

echo "${#arr[@]}"
来源：http://mobile.tarul.cn/Article/details/gfnrcxqjw.sHtML

[R20] 关联数组（字典）
来源：http://m.share.yfazqb.com/Article/details/gybhudtrg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.bbcook.cn/Article/details/gwlccaryi.sHtML

[R21] 字符串长度
来源：http://www.blog.yfazqb.com/Article/details/gqgyhzrua.sHtML

echo "${#s}"
来源：http://wap.vehdjk.com/Article/details/gslqeaeyg.sHtML

[R22] 截取子串
来源：http://www.blog.yfazqb.com/Article/details/gjqhqqdtq.sHtML

echo "${s:0:5}"
来源：http://mobile.yfazqb.com/Article/details/gazonoman.sHtML

[R23] 字符串替换
来源：http://baike.tarul.cn/Article/details/gkwzbviol.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.yfazqb.com/Article/details/gzwpwputp.sHtML

[R24] 大小写转换
来源：http://blog.sjlbkw.cn/Article/details/gsnkcynbl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.yfazqb.com/Article/details/gspbeelef.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.yfazqb.com/Article/details/gpimkzjkh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.epnwcf.com/Article/details/gnzqjmyvg.sHtML

[R26] 命令替换
来源：http://www.blog.fktsv.cn/Article/details/gsilgsbkb.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.bbcook.cn/Article/details/gcfoontmc.sHtML

[R27] 算术展开
来源：http://wap.yfazqb.com/Article/details/gzceypntl.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fktsv.cn/Article/details/genmdqsxk.sHtML

[R28] 浮点运算
来源：http://m.share.bbcook.cn/Article/details/gdzecetag.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.epnwcf.com/Article/details/gugckuqyu.sHtML

[R29] 定义函数
来源：http://3g.bbcook.cn/Article/details/gvnchifpe.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.epnwcf.com/Article/details/glxehzqmv.sHtML

[R30] 函数返回状态码
来源：http://wap.bbcook.cn/Article/details/gmejebfll.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.yfazqb.com/Article/details/gbvgtcdue.sHtML

[R31] 局部变量
来源：http://3g.epnwcf.com/Article/details/gkcwetdlk.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.epnwcf.com/Article/details/gbohyqjat.sHtML

[R32] 参数个数校验
来源：http://wap.fktsv.cn/Article/details/ggsucewak.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.epnwcf.com/Article/details/gkgttnzaf.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.bbcook.cn/Article/details/gpvdqjdeg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.epnwcf.com/Article/details/gjvumfcfv.sHtML

[R34] 退出时清理
来源：http://m.share.fktsv.cn/Article/details/gdyseonkm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.tarul.cn/Article/details/ghmpbimos.sHtML

[R35] 后台执行并等待
来源：http://www.share.fktsv.cn/Article/details/gkldqazfc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.vehdjk.com/Article/details/gedoxotmx.sHtML

[R36] 并发执行多个任务
来源：http://mobile.epnwcf.com/Article/details/gspxbqbgs.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.bbcook.cn/Article/details/gmjroplym.sHtML

[R37] 把输出赋给变量
来源：http://mobile.tarul.cn/Article/details/gtbyjvkty.sHtML

files=$(ls -1)
来源：http://wap.fktsv.cn/Article/details/gkgmwcdhy.sHtML

[R38] 管道串联
来源：http://wap.fktsv.cn/Article/details/ggrmmzcst.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.bbcook.cn/Article/details/gnwdjimde.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.bbcook.cn/Article/details/gwwdttdls.sHtML

cmd > out.log 2>&1
来源：http://baike.vehdjk.com/Article/details/gulzonnqg.sHtML

[R40] 追加写日志
来源：http://blog.epnwcf.com/Article/details/gfwtwjwxm.sHtML

echo "log" >> out.log
来源：http://3g.tarul.cn/Article/details/gluusdipe.sHtML

[R41] 丢弃输出
来源：http://read.share.bbcook.cn/Article/details/ghxxewcbp.sHtML

cmd >/dev/null 2>&1
来源：http://baike.tarul.cn/Article/details/gvcxiogbs.sHtML

[R42] 输入重定向
来源：http://m.share.tarul.cn/Article/details/gwzmbjmil.sHtML

wc -l < a.txt
来源：http://mobile.sjlbkw.cn/Article/details/gdqtwkafx.sHtML

[R43] 按名字查找文件
来源：http://wap.tarul.cn/Article/details/gmmttbidr.sHtML

find . -name "*.log" -type f
来源：http://baike.vehdjk.com/Article/details/gdfnmrzvl.sHtML

[R44] 按修改时间查找
来源：http://mobile.tarul.cn/Article/details/glbjqkjda.sHtML

find . -mtime -7 -type f
来源：http://baike.yfazqb.com/Article/details/gtgqwjgrt.sHtML

[R45] 批量删除
来源：http://wap.bbcook.cn/Article/details/giwwcpuso.sHtML

find . -name "*.tmp" -delete
来源：http://3g.bbcook.cn/Article/details/gvixbveaf.sHtML

[R46] 递归替换文件内容
来源：http://www.share.bbcook.cn/Article/details/gjynabcke.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.sjlbkw.cn/Article/details/gixugvfaq.sHtML

[R47] sed 单行替换
来源：http://www.share.yfazqb.com/Article/details/goxuvncbv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.vehdjk.com/Article/details/gjicdwpas.sHtML

[R48] awk 取指定列
来源：http://m.share.yfazqb.com/Article/details/giakekhiw.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.bbcook.cn/Article/details/gmysekyre.sHtML

[R49] awk 带条件
来源：http://mobile.sjlbkw.cn/Article/details/gcicnlfco.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fktsv.cn/Article/details/gbscruwlw.sHtML

[R50] awk 求和
来源：http://wap.epnwcf.com/Article/details/gverrpwlx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.vehdjk.com/Article/details/gjbcuknal.sHtML

[R51] 排序去重取前几
来源：http://read.share.yfazqb.com/Article/details/gxqxskpbi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.yfazqb.com/Article/details/gonsytamc.sHtML

[R52] 统计行数
来源：http://blog.tarul.cn/Article/details/gfhstuuda.sHtML

wc -l a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gtmonzzbz.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.yfazqb.com/Article/details/glonirxdh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.epnwcf.com/Article/details/gsthfmtmr.sHtML

[R54] 比较两个文件
来源：http://m.share.tarul.cn/Article/details/gwmovvskt.sHtML

diff a.txt b.txt
来源：http://www.blog.yfazqb.com/Article/details/goduwihnj.sHtML

[R55] 压缩与解压
来源：http://mobile.fktsv.cn/Article/details/gnxalqnty.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.yfazqb.com/Article/details/grxnradan.sHtML

[R56] 远程拷贝
来源：http://blog.yfazqb.com/Article/details/gxufchkjh.sHtML

scp file user@host:/path/
来源：http://wap.bbcook.cn/Article/details/gvqfkxhkq.sHtML

[R57] 远程执行命令
来源：http://blog.yfazqb.com/Article/details/geooxwajw.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.tarul.cn/Article/details/grsqtlwmj.sHtML

[R58] 下载文件
来源：http://baike.vehdjk.com/Article/details/gynixaphs.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fktsv.cn/Article/details/gtkkufcje.sHtML

[R59] 发 POST JSON
来源：http://read.share.vehdjk.com/Article/details/gkppipdkv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.vehdjk.com/Article/details/glprhlnfl.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fktsv.cn/Article/details/gumgdhwwq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fktsv.cn/Article/details/gvdgaocla.sHtML

[R61] 磁盘占用
来源：http://www.share.bbcook.cn/Article/details/gnkbmrbkm.sHtML

df -h;  du -sh *
来源：http://www.blog.fktsv.cn/Article/details/gwzioocps.sHtML

[R62] 找最占空间的文件
来源：http://mobile.epnwcf.com/Article/details/gcptnsoiz.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.tarul.cn/Article/details/gxevzbevj.sHtML

[R63] 内存与进程
来源：http://m.share.tarul.cn/Article/details/gpsgiswve.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.vehdjk.com/Article/details/gshwdslti.sHtML

[R64] 结束进程
来源：http://m.share.yfazqb.com/Article/details/gnnxapmjq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fktsv.cn/Article/details/gvctqmcne.sHtML

[R65] 查看端口占用
来源：http://blog.sjlbkw.cn/Article/details/gwgjynsgc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.sjlbkw.cn/Article/details/gjptuntzg.sHtML

[R66] 定时任务
来源：http://www.blog.bbcook.cn/Article/details/gntdaetok.sHtML

crontab -e;  crontab -l
来源：http://wap.yfazqb.com/Article/details/gvahxubpu.sHtML

[R67] 生成随机十六进制串
来源：http://3g.sjlbkw.cn/Article/details/gccliijkv.sHtML

openssl rand -hex 16
来源：http://www.blog.epnwcf.com/Article/details/ggapkdcvo.sHtML

[R68] 计算文件校验值
来源：http://wap.yfazqb.com/Article/details/gjqpisrcu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.tarul.cn/Article/details/gwhsdnlyo.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fktsv.cn/Article/details/gobgnuoku.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.yfazqb.com/Article/details/gmdpvnlgn.sHtML

[R70] 时间戳与互转
来源：http://read.share.sjlbkw.cn/Article/details/gtftrkzoi.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fktsv.cn/Article/details/gcvfkaxad.sHtML

[R71] 日期格式化
来源：http://www.m.share.vehdjk.com/Article/details/gygtvnfqv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.tarul.cn/Article/details/gevqpgkve.sHtML

[R72] 等待端口就绪
来源：http://www.blog.vehdjk.com/Article/details/gvunmqovr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.yfazqb.com/Article/details/gddlidohc.sHtML

[R73] 分割大日志
来源：http://blog.bbcook.cn/Article/details/givyyhgkp.sHtML

split -l 1000 big.log part_
来源：http://baike.bbcook.cn/Article/details/gggjgnska.sHtML

[R74] 批量重命名
来源：http://www.share.vehdjk.com/Article/details/glquxojbw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.bbcook.cn/Article/details/gqvfwywxi.sHtML

[R75] 导出环境变量
来源：http://3g.tarul.cn/Article/details/gclephuft.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.vehdjk.com/Article/details/gdrwygwpk.sHtML

[R76] 使用临时文件
来源：http://www.m.share.vehdjk.com/Article/details/gxdipspwv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fktsv.cn/Article/details/gvckqfhgi.sHtML

[R77] 读取用户输入
来源：http://mobile.epnwcf.com/Article/details/ghrbfpney.sHtML

read -rp "请输入: " ans
来源：http://baike.vehdjk.com/Article/details/guhgczgve.sHtML

[R78] 交互式菜单
来源：http://blog.fktsv.cn/Article/details/gttspowhw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.tarul.cn/Article/details/gzdprmstw.sHtML

[R79] 解析命令行选项
来源：http://baike.vehdjk.com/Article/details/gytmdqyfa.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.epnwcf.com/Article/details/gsijedbnw.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.yfazqb.com/Article/details/gmfcrrxip.sHtML

time ./run.sh
来源：http://www.blog.sjlbkw.cn/Article/details/gbagpabtw.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gtdyauquc.sHtML

S. C / C++ 专题
来源：http://www.blog.fktsv.cn/Article/details/gctuekzln.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gefisllmx.sHtML

[S01] C：Hello World
来源：http://wap.yfazqb.com/Article/details/gdbgxmmmm.sHtML

#include <stdio.h>
来源：http://www.blog.sjlbkw.cn/Article/details/gicikvpyk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.yfazqb.com/Article/details/gvtoqcslc.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fktsv.cn/Article/details/gjfveyjlx.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.tarul.cn/Article/details/gnjlroiai.sHtML

[S03] C：读入整数
来源：http://www.share.tarul.cn/Article/details/gbdnbgfdo.sHtML

int x; scanf("%d", &x);
来源：http://read.share.bbcook.cn/Article/details/gfrujeodt.sHtML

[S04] C：字符串复制
来源：http://www.share.sjlbkw.cn/Article/details/giyylgjyi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.epnwcf.com/Article/details/ghsmvhhil.sHtML

[S05] C：字符串长度
来源：http://www.m.share.bbcook.cn/Article/details/gtzbbggxa.sHtML

strlen(s)
来源：http://www.m.share.tarul.cn/Article/details/gchssugww.sHtML

[S06] C：字符串比较
来源：http://www.blog.yfazqb.com/Article/details/gaaelhwuh.sHtML

strcmp(a, b) == 0
来源：http://3g.sjlbkw.cn/Article/details/gtxbmccth.sHtML

[S07] C：数组遍历求和
来源：http://wap.fktsv.cn/Article/details/gqacfwnzc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.yfazqb.com/Article/details/gqopivfew.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.yfazqb.com/Article/details/ghjzpzlym.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.yfazqb.com/Article/details/gwrkmggvm.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fktsv.cn/Article/details/gimomtewd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.yfazqb.com/Article/details/ggxqvekld.sHtML

[S10] C：指针与解引用
来源：http://www.blog.tarul.cn/Article/details/getqjgazs.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.vehdjk.com/Article/details/gargyuwlv.sHtML

[S11] C：逐行读文件
来源：http://m.share.fktsv.cn/Article/details/gqhskuoku.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.sjlbkw.cn/Article/details/gitogizuw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.vehdjk.com/Article/details/gguxkxrhb.sHtML

fclose(f);
来源：http://m.share.fktsv.cn/Article/details/grkutjsyu.sHtML

[S12] C：写文件
来源：http://www.blog.bbcook.cn/Article/details/guuikxwik.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.bbcook.cn/Article/details/gojcuhocl.sHtML

[S13] C：宏定义
来源：http://mobile.bbcook.cn/Article/details/gemrqsmxs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.bbcook.cn/Article/details/gbiqvgpvl.sHtML

[S14] C：枚举
来源：http://wap.tarul.cn/Article/details/grkckkxgy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.yfazqb.com/Article/details/gftggnkai.sHtML

[S15] C：类型转换
来源：http://www.blog.sjlbkw.cn/Article/details/gcevrumxy.sHtML

(double) a / b
来源：http://read.share.sjlbkw.cn/Article/details/gbeidauyn.sHtML

[S16] C：位操作置位
来源：http://www.share.sjlbkw.cn/Article/details/gawjgazyi.sHtML

x |= (1 << 3);
来源：http://m.share.yfazqb.com/Article/details/gkjicezcf.sHtML

[S17] C：安全拼接字符串
来源：http://blog.vehdjk.com/Article/details/gonafdxdd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.vehdjk.com/Article/details/ggxjgiife.sHtML

[S18] C：命令行参数
来源：http://www.blog.bbcook.cn/Article/details/gjkirluir.sHtML

int main(int argc, char **argv)
来源：http://3g.yfazqb.com/Article/details/gkhisjtnh.sHtML

[S19] C：快速排序
来源：http://read.share.epnwcf.com/Article/details/gbaqfvdag.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.yfazqb.com/Article/details/gzdrwlrpx.sHtML

[S20] C：二分查找
来源：http://www.share.yfazqb.com/Article/details/gkbofmxmm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fktsv.cn/Article/details/gcxlwlmpc.sHtML

[S21] C：字符类别判断
来源：http://www.share.yfazqb.com/Article/details/gbhgwccru.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.sjlbkw.cn/Article/details/gfagspdcr.sHtML

[S22] C：字符串转数字
来源：http://mobile.fktsv.cn/Article/details/gmnnnmaao.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.bbcook.cn/Article/details/gwlwydtll.sHtML

[S23] C：随机数
来源：http://baike.yfazqb.com/Article/details/gvguasuqz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.sjlbkw.cn/Article/details/grutfddlh.sHtML

[S24] C：获取本地时间
来源：http://mobile.fktsv.cn/Article/details/gpmxyuaop.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fktsv.cn/Article/details/gjblssvdz.sHtML

[S25] C：内存拷贝
来源：http://blog.yfazqb.com/Article/details/gczxuiuio.sHtML

memcpy(dst, src, n);
来源：http://read.share.sjlbkw.cn/Article/details/gvuxqphpy.sHtML

[S26] C：内存清零
来源：http://blog.epnwcf.com/Article/details/gefwkcycm.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.epnwcf.com/Article/details/gtuyehnnw.sHtML

[S27] C：定义常量
来源：http://www.share.fktsv.cn/Article/details/gpeypcnws.sHtML

const double PI = 3.14159;
来源：http://m.share.epnwcf.com/Article/details/gbquqsuhk.sHtML

[S28] C：静态变量
来源：http://m.share.yfazqb.com/Article/details/gdmtgwagf.sHtML

static int counter = 0;
来源：http://mobile.bbcook.cn/Article/details/gvwdgrbfe.sHtML

[S29] C：变参函数
来源：http://blog.bbcook.cn/Article/details/gruizvohi.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.vehdjk.com/Article/details/gxabzdjjc.sHtML

[S30] C：头文件保护
来源：http://mobile.tarul.cn/Article/details/gcdccmlak.sHtML

#ifndef X_H
来源：http://m.share.vehdjk.com/Article/details/gtpgcacjm.sHtML

#define X_H
来源：http://blog.epnwcf.com/Article/details/gjrfhnkfo.sHtML

#endif
来源：http://read.share.bbcook.cn/Article/details/gwtkfyzpb.sHtML

[S31] C++：Hello World
来源：http://3g.vehdjk.com/Article/details/ggppgoffs.sHtML

#include <iostream>
来源：http://wap.vehdjk.com/Article/details/gvajqxenk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.sjlbkw.cn/Article/details/gnhyfsmrg.sHtML

[S32] C++：字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gydozwdxu.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fktsv.cn/Article/details/goljanfxu.sHtML

[S33] C++：vector 增删
来源：http://baike.vehdjk.com/Article/details/gcnavpkxu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.bbcook.cn/Article/details/gmogmccfn.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fktsv.cn/Article/details/gvyupkqfh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.yfazqb.com/Article/details/glibmekba.sHtML

[S35] C++：map
来源：http://mobile.bbcook.cn/Article/details/gyprsevww.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.yfazqb.com/Article/details/gpnwfrlab.sHtML

[S36] C++：unordered_map
来源：http://read.share.bbcook.cn/Article/details/gftgaaqsg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.epnwcf.com/Article/details/gxmfqrjyf.sHtML

[S37] C++：set
来源：http://www.share.bbcook.cn/Article/details/gbhmatnkn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.sjlbkw.cn/Article/details/glcjgrmph.sHtML

[S38] C++：排序
来源：http://www.m.share.fktsv.cn/Article/details/gauzauufl.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fktsv.cn/Article/details/gurzhdsko.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fktsv.cn/Article/details/gfxlqvqex.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.bbcook.cn/Article/details/gzuoaagsl.sHtML

[S40] C++：查找元素
来源：http://www.m.share.yfazqb.com/Article/details/gwzfiwplf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.bbcook.cn/Article/details/gyartthnq.sHtML

[S41] C++：类与构造函数
来源：http://3g.tarul.cn/Article/details/gtfzzqhoh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.sjlbkw.cn/Article/details/gefsypwbw.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.epnwcf.com/Article/details/ganovxhvu.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.vehdjk.com/Article/details/grlrcqaro.sHtML

[S43] C++：智能指针
来源：http://wap.yfazqb.com/Article/details/gjgbohyik.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.tarul.cn/Article/details/glljhxqmb.sHtML

[S44] C++：引用传参
来源：http://read.share.fktsv.cn/Article/details/gkdthmvdr.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.tarul.cn/Article/details/gecmqkvfg.sHtML

[S45] C++：lambda
来源：http://www.m.share.tarul.cn/Article/details/gjatckrgn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.epnwcf.com/Article/details/gtqszsafw.sHtML

[S46] C++：函数模板
来源：http://www.share.bbcook.cn/Article/details/gwmkgpqas.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.epnwcf.com/Article/details/geqnpluzp.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.yfazqb.com/Article/details/gpzcdqseq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.tarul.cn/Article/details/gtwecpozg.sHtML

[S48] C++：逐行读文件
来源：http://m.share.bbcook.cn/Article/details/gwjkbouih.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.tarul.cn/Article/details/ghqkoerap.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.bbcook.cn/Article/details/gydeytxsw.sHtML

[S49] C++：写文件
来源：http://m.share.fktsv.cn/Article/details/gacemcqem.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.epnwcf.com/Article/details/gyzrcmola.sHtML

[S50] C++：格式化数字
来源：http://wap.fktsv.cn/Article/details/gxiifnyhy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.bbcook.cn/Article/details/gpyelqpuo.sHtML

[S51] C++：显式类型转换
来源：http://3g.fktsv.cn/Article/details/gcrmewzsp.sHtML

static_cast<double>(a) / b
来源：http://m.share.vehdjk.com/Article/details/gsmjlkugj.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.epnwcf.com/Article/details/giqoouzhb.sHtML


<!-- 参考信息 -->