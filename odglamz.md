代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://3g.tarul.cn/Article/details/gtuceksyn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.sjlbkw.cn/Article/details/gblworawt.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.vehdjk.com/Article/details/gwnvlxlfw.sHtML

[Q89] 判断表是否存在
来源：http://blog.yfazqb.com/Article/details/gojdjrqmv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.vehdjk.com/Article/details/gzrnjkgjx.sHtML

[Q90] 生成序号列
来源：http://read.share.tarul.cn/Article/details/gdnmgbupb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.yfazqb.com/Article/details/gegmqavbi.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gtvtxhrqy.sHtML

R. Bash 专题
来源：http://read.share.sjlbkw.cn/Article/details/gzoqstutm.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gedkuetjm.sHtML

[R01] shebang 与严格模式
来源：http://blog.bbcook.cn/Article/details/gvrolumzz.sHtML

#!/usr/bin/env bash
来源：http://www.share.epnwcf.com/Article/details/gxdbwycvj.sHtML

set -euo pipefail
来源：http://mobile.tarul.cn/Article/details/gtmxzyxdi.sHtML

[R02] 变量赋值与使用
来源：http://read.share.bbcook.cn/Article/details/ghzeapbpw.sHtML

name="Tom"; echo "$name"
来源：http://read.share.sjlbkw.cn/Article/details/gypccujzs.sHtML

[R03] 只读变量
来源：http://baike.fktsv.cn/Article/details/gjlhuottr.sHtML

readonly PI=3.14
来源：http://www.m.share.tarul.cn/Article/details/gqajapugo.sHtML

[R04] 位置参数
来源：http://www.m.share.yfazqb.com/Article/details/gvnkbhacn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.yfazqb.com/Article/details/gpoxivkzr.sHtML

[R05] 参数默认值
来源：http://m.share.vehdjk.com/Article/details/gzowwsokx.sHtML

name="${1:-default}"
来源：http://www.blog.epnwcf.com/Article/details/gnpiyxuay.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.yfazqb.com/Article/details/gilafylfh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.yfazqb.com/Article/details/ggrmeyopr.sHtML

[R07] if 判断文件
来源：http://baike.sjlbkw.cn/Article/details/gytcbctwr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.yfazqb.com/Article/details/gpncttakq.sHtML

[R08] 数值比较
来源：http://baike.tarul.cn/Article/details/gtihqcyty.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.epnwcf.com/Article/details/gekxsyzuh.sHtML

[R09] 字符串比较
来源：http://3g.yfazqb.com/Article/details/gdimdwcxt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fktsv.cn/Article/details/gdhckdbwy.sHtML

[R10] 正则匹配
来源：http://read.share.fktsv.cn/Article/details/ggskmkvrg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.vehdjk.com/Article/details/gjlexwlqx.sHtML

[R11] case 多分支
来源：http://www.share.bbcook.cn/Article/details/gofxblmrd.sHtML

case "$1" in
来源：http://read.share.epnwcf.com/Article/details/gpxqcsroa.sHtML

start) echo "启动" ;;
来源：http://wap.yfazqb.com/Article/details/glgsqxgee.sHtML

stop)  echo "停止" ;;
来源：http://m.share.sjlbkw.cn/Article/details/gvbwtkeak.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.yfazqb.com/Article/details/ggktrgqef.sHtML

esac
来源：http://wap.epnwcf.com/Article/details/gzrizlqiu.sHtML

[R12] for 遍历文件
来源：http://blog.vehdjk.com/Article/details/gfhtbpsxu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.sjlbkw.cn/Article/details/gzlsxfdip.sHtML

[R13] for 计数循环
来源：http://www.share.epnwcf.com/Article/details/gcxdxhgok.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fktsv.cn/Article/details/gvmmhfgty.sHtML

[R14] C 风格 for
来源：http://blog.tarul.cn/Article/details/gkjiheodn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fktsv.cn/Article/details/gvuzzooky.sHtML

[R15] while 逐行读文件
来源：http://read.share.tarul.cn/Article/details/ggnpsphal.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fktsv.cn/Article/details/gxqfjhegz.sHtML

[R16] until 等待条件
来源：http://baike.bbcook.cn/Article/details/gtlgejzpp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.epnwcf.com/Article/details/gpziahhwj.sHtML

[R17] 数组定义与取值
来源：http://mobile.vehdjk.com/Article/details/gglizhjuq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.tarul.cn/Article/details/gaytusuvi.sHtML

[R18] 遍历数组
来源：http://3g.fktsv.cn/Article/details/gwfezlemm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.epnwcf.com/Article/details/gzzixkvxg.sHtML

[R19] 数组长度
来源：http://www.blog.sjlbkw.cn/Article/details/gvvxyfyes.sHtML

echo "${#arr[@]}"
来源：http://3g.epnwcf.com/Article/details/gjqyridgl.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.bbcook.cn/Article/details/gzseerhkr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fktsv.cn/Article/details/gtfatjgwn.sHtML

[R21] 字符串长度
来源：http://wap.vehdjk.com/Article/details/gplbashpy.sHtML

echo "${#s}"
来源：http://www.share.yfazqb.com/Article/details/ganytweaj.sHtML

[R22] 截取子串
来源：http://baike.vehdjk.com/Article/details/gxwbhfrpc.sHtML

echo "${s:0:5}"
来源：http://read.share.vehdjk.com/Article/details/gysnzccne.sHtML

[R23] 字符串替换
来源：http://3g.vehdjk.com/Article/details/ggdccgjyw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fktsv.cn/Article/details/gtsmcjoec.sHtML

[R24] 大小写转换
来源：http://m.share.vehdjk.com/Article/details/guufjemda.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.yfazqb.com/Article/details/gwilgzzed.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.yfazqb.com/Article/details/goovvhnuj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.yfazqb.com/Article/details/gadqxmyar.sHtML

[R26] 命令替换
来源：http://read.share.vehdjk.com/Article/details/gaqhdaanv.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.sjlbkw.cn/Article/details/gqrtmsvkn.sHtML

[R27] 算术展开
来源：http://www.share.fktsv.cn/Article/details/gpqfgwicc.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.sjlbkw.cn/Article/details/gmfytyrxu.sHtML

[R28] 浮点运算
来源：http://blog.bbcook.cn/Article/details/gfgdakfzo.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.tarul.cn/Article/details/gdytmpwak.sHtML

[R29] 定义函数
来源：http://www.share.tarul.cn/Article/details/gfwspbice.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.sjlbkw.cn/Article/details/gftbfrqat.sHtML

[R30] 函数返回状态码
来源：http://blog.fktsv.cn/Article/details/gqnltibqb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.yfazqb.com/Article/details/gldorxlcf.sHtML

[R31] 局部变量
来源：http://www.blog.tarul.cn/Article/details/gruveqgbn.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.yfazqb.com/Article/details/gjgbbsppy.sHtML

[R32] 参数个数校验
来源：http://www.blog.bbcook.cn/Article/details/gmzvluqht.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.tarul.cn/Article/details/gtfcmptgx.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.bbcook.cn/Article/details/gwzujwaxl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.epnwcf.com/Article/details/gsrlvlzrr.sHtML

[R34] 退出时清理
来源：http://3g.fktsv.cn/Article/details/gwigcyrcl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.epnwcf.com/Article/details/gnsmvmaay.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fktsv.cn/Article/details/gaxbyskrg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.yfazqb.com/Article/details/gzdaddggh.sHtML

[R36] 并发执行多个任务
来源：http://mobile.sjlbkw.cn/Article/details/gocnzjnuc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.bbcook.cn/Article/details/giplanjdu.sHtML

[R37] 把输出赋给变量
来源：http://mobile.yfazqb.com/Article/details/gruexdwdn.sHtML

files=$(ls -1)
来源：http://m.share.yfazqb.com/Article/details/gsivwurbn.sHtML

[R38] 管道串联
来源：http://www.blog.fktsv.cn/Article/details/ggxamnreu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.sjlbkw.cn/Article/details/gbavluivn.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.tarul.cn/Article/details/gjpxvtyrq.sHtML

cmd > out.log 2>&1
来源：http://blog.epnwcf.com/Article/details/gupzszzod.sHtML

[R40] 追加写日志
来源：http://mobile.bbcook.cn/Article/details/grgvjwcuk.sHtML

echo "log" >> out.log
来源：http://3g.bbcook.cn/Article/details/gpubdqnat.sHtML

[R41] 丢弃输出
来源：http://baike.sjlbkw.cn/Article/details/gwvpqhgaw.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fktsv.cn/Article/details/gvmtyhhdw.sHtML

[R42] 输入重定向
来源：http://www.m.share.yfazqb.com/Article/details/gdirrfqvq.sHtML

wc -l < a.txt
来源：http://blog.epnwcf.com/Article/details/gkwbgofmi.sHtML

[R43] 按名字查找文件
来源：http://3g.epnwcf.com/Article/details/ghsojiorw.sHtML

find . -name "*.log" -type f
来源：http://blog.vehdjk.com/Article/details/gjppmdrqv.sHtML

[R44] 按修改时间查找
来源：http://read.share.epnwcf.com/Article/details/gixdyavbe.sHtML

find . -mtime -7 -type f
来源：http://blog.tarul.cn/Article/details/gmjzfaxli.sHtML

[R45] 批量删除
来源：http://www.m.share.fktsv.cn/Article/details/gztftmoyt.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.tarul.cn/Article/details/gxcbtmuwe.sHtML

[R46] 递归替换文件内容
来源：http://mobile.yfazqb.com/Article/details/gkhkdvgfd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.epnwcf.com/Article/details/gvtgmjobq.sHtML

[R47] sed 单行替换
来源：http://mobile.fktsv.cn/Article/details/gmeposzhi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.yfazqb.com/Article/details/gajmqvhap.sHtML

[R48] awk 取指定列
来源：http://mobile.vehdjk.com/Article/details/gtuqzguif.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.tarul.cn/Article/details/gnlmdtjdq.sHtML

[R49] awk 带条件
来源：http://mobile.fktsv.cn/Article/details/glokgnubw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.tarul.cn/Article/details/gqirtqrzz.sHtML

[R50] awk 求和
来源：http://www.blog.sjlbkw.cn/Article/details/gtixkajuj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.epnwcf.com/Article/details/grezalcod.sHtML

[R51] 排序去重取前几
来源：http://www.blog.tarul.cn/Article/details/gmlcaamjz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.tarul.cn/Article/details/gixqkuryv.sHtML

[R52] 统计行数
来源：http://baike.fktsv.cn/Article/details/grjsokhin.sHtML

wc -l a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gneyrlhyb.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.bbcook.cn/Article/details/gluzqjgcd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.epnwcf.com/Article/details/gmvyszgtt.sHtML

[R54] 比较两个文件
来源：http://www.m.share.vehdjk.com/Article/details/gflfueyxe.sHtML

diff a.txt b.txt
来源：http://3g.tarul.cn/Article/details/gsftialen.sHtML

[R55] 压缩与解压
来源：http://blog.tarul.cn/Article/details/gvgjyvlek.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fktsv.cn/Article/details/glyszeair.sHtML

[R56] 远程拷贝
来源：http://m.share.epnwcf.com/Article/details/gdrihjvne.sHtML

scp file user@host:/path/
来源：http://3g.vehdjk.com/Article/details/gdkhusmij.sHtML

[R57] 远程执行命令
来源：http://read.share.bbcook.cn/Article/details/gjhtnuyti.sHtML

ssh user@host 'uptime'
来源：http://wap.fktsv.cn/Article/details/gmvtvrcjw.sHtML

[R58] 下载文件
来源：http://m.share.epnwcf.com/Article/details/gqkutihdg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fktsv.cn/Article/details/gpuiznjoz.sHtML

[R59] 发 POST JSON
来源：http://mobile.bbcook.cn/Article/details/ggpgpqjyd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.vehdjk.com/Article/details/gbmplazdh.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.vehdjk.com/Article/details/gtkkmlcra.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.vehdjk.com/Article/details/gswiyohar.sHtML

[R61] 磁盘占用
来源：http://baike.fktsv.cn/Article/details/gvpflfvcc.sHtML

df -h;  du -sh *
来源：http://baike.sjlbkw.cn/Article/details/grukyyrbn.sHtML

[R62] 找最占空间的文件
来源：http://m.share.bbcook.cn/Article/details/glguepcpa.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.vehdjk.com/Article/details/gjxccngrj.sHtML

[R63] 内存与进程
来源：http://3g.epnwcf.com/Article/details/gjdpjjpkj.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.yfazqb.com/Article/details/gcabpcsyt.sHtML

[R64] 结束进程
来源：http://wap.fktsv.cn/Article/details/gtwnpwdlc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.epnwcf.com/Article/details/gwagjvuyn.sHtML

[R65] 查看端口占用
来源：http://mobile.fktsv.cn/Article/details/goqqvtahw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.sjlbkw.cn/Article/details/gijqlnpgz.sHtML

[R66] 定时任务
来源：http://www.m.share.epnwcf.com/Article/details/gezhfswoo.sHtML

crontab -e;  crontab -l
来源：http://www.blog.bbcook.cn/Article/details/gqxjvykkk.sHtML

[R67] 生成随机十六进制串
来源：http://3g.bbcook.cn/Article/details/gqvywfslx.sHtML

openssl rand -hex 16
来源：http://wap.sjlbkw.cn/Article/details/gxkkwuwwg.sHtML

[R68] 计算文件校验值
来源：http://m.share.fktsv.cn/Article/details/gqexcifgc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.vehdjk.com/Article/details/gtcijhifv.sHtML

[R69] 生成随机密码
来源：http://baike.vehdjk.com/Article/details/gkjymeetk.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.vehdjk.com/Article/details/gvskjntop.sHtML

[R70] 时间戳与互转
来源：http://blog.fktsv.cn/Article/details/grlrsckqm.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.epnwcf.com/Article/details/galcqqffa.sHtML

[R71] 日期格式化
来源：http://mobile.sjlbkw.cn/Article/details/glfnooeji.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.bbcook.cn/Article/details/gcxyiebzm.sHtML

[R72] 等待端口就绪
来源：http://blog.sjlbkw.cn/Article/details/giguogjkr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.yfazqb.com/Article/details/gocoxosyw.sHtML

[R73] 分割大日志
来源：http://3g.epnwcf.com/Article/details/goqkowahh.sHtML

split -l 1000 big.log part_
来源：http://m.share.tarul.cn/Article/details/gqndrwblk.sHtML

[R74] 批量重命名
来源：http://wap.tarul.cn/Article/details/gtcvuyyxq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.sjlbkw.cn/Article/details/gleyxnvda.sHtML

[R75] 导出环境变量
来源：http://baike.yfazqb.com/Article/details/gpyojsaap.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.sjlbkw.cn/Article/details/gjbhkdblp.sHtML

[R76] 使用临时文件
来源：http://3g.tarul.cn/Article/details/gcpqrmxsn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.sjlbkw.cn/Article/details/geqmfctpj.sHtML

[R77] 读取用户输入
来源：http://www.blog.epnwcf.com/Article/details/glplccrby.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.vehdjk.com/Article/details/gevlkofad.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fktsv.cn/Article/details/gchntngah.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.vehdjk.com/Article/details/gkqkotwnp.sHtML

[R79] 解析命令行选项
来源：http://wap.yfazqb.com/Article/details/ggqjwtqzb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.yfazqb.com/Article/details/gabxkyzru.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.sjlbkw.cn/Article/details/gknvgauhg.sHtML

time ./run.sh
来源：http://3g.fktsv.cn/Article/details/ggffydcvq.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gjdpgzzdv.sHtML

S. C / C++ 专题
来源：http://www.m.share.epnwcf.com/Article/details/gmhewtinf.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gfexoktpe.sHtML

[S01] C：Hello World
来源：http://m.share.yfazqb.com/Article/details/gorqqprhc.sHtML

#include <stdio.h>
来源：http://3g.fktsv.cn/Article/details/gcodfjwkz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.tarul.cn/Article/details/gcjzbgaak.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.tarul.cn/Article/details/ggczehpux.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fktsv.cn/Article/details/gtfjzfadg.sHtML

[S03] C：读入整数
来源：http://m.share.sjlbkw.cn/Article/details/gimvqpxdr.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.epnwcf.com/Article/details/gtskymjcp.sHtML

[S04] C：字符串复制
来源：http://blog.epnwcf.com/Article/details/gsyvugifu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.bbcook.cn/Article/details/gsfegylki.sHtML

[S05] C：字符串长度
来源：http://mobile.tarul.cn/Article/details/grmalthnw.sHtML

strlen(s)
来源：http://wap.vehdjk.com/Article/details/gdwjojdgj.sHtML

[S06] C：字符串比较
来源：http://m.share.fktsv.cn/Article/details/goyzwnuvq.sHtML

strcmp(a, b) == 0
来源：http://read.share.sjlbkw.cn/Article/details/gsrjrvkym.sHtML

[S07] C：数组遍历求和
来源：http://3g.sjlbkw.cn/Article/details/ggwakmqqr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.bbcook.cn/Article/details/gbsxgulbc.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fktsv.cn/Article/details/gnqmrblat.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.bbcook.cn/Article/details/ghvqylpbx.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.sjlbkw.cn/Article/details/glbjtgrzh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.bbcook.cn/Article/details/gzejzouzc.sHtML

[S10] C：指针与解引用
来源：http://blog.tarul.cn/Article/details/gblbkyier.sHtML

int *p = &a;  *p = 5;
来源：http://3g.tarul.cn/Article/details/gegdhwpkw.sHtML

[S11] C：逐行读文件
来源：http://blog.sjlbkw.cn/Article/details/gwmxviefc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.epnwcf.com/Article/details/gfpbuflpz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.tarul.cn/Article/details/gcvkkhiod.sHtML

fclose(f);
来源：http://baike.vehdjk.com/Article/details/gponuyuna.sHtML

[S12] C：写文件
来源：http://3g.epnwcf.com/Article/details/gaqhqbbvy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.yfazqb.com/Article/details/gjamfgwpp.sHtML

[S13] C：宏定义
来源：http://m.share.sjlbkw.cn/Article/details/gnsassfkh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.epnwcf.com/Article/details/gvhsbnzto.sHtML

[S14] C：枚举
来源：http://mobile.bbcook.cn/Article/details/gtffsufht.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fktsv.cn/Article/details/gkxzfazae.sHtML

[S15] C：类型转换
来源：http://m.share.fktsv.cn/Article/details/gnwcccjvl.sHtML

(double) a / b
来源：http://www.m.share.yfazqb.com/Article/details/ghogvclfp.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fktsv.cn/Article/details/ggwzqitmx.sHtML

x |= (1 << 3);
来源：http://m.share.fktsv.cn/Article/details/gmhptutty.sHtML

[S17] C：安全拼接字符串
来源：http://wap.epnwcf.com/Article/details/glbdjszsq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.bbcook.cn/Article/details/gpbylbhgc.sHtML

[S18] C：命令行参数
来源：http://3g.vehdjk.com/Article/details/gfdzztxqx.sHtML

int main(int argc, char **argv)
来源：http://baike.bbcook.cn/Article/details/gpogchqnn.sHtML

[S19] C：快速排序
来源：http://3g.fktsv.cn/Article/details/guoaetyba.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.sjlbkw.cn/Article/details/gwiivjalb.sHtML

[S20] C：二分查找
来源：http://www.m.share.tarul.cn/Article/details/gakfldblf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.bbcook.cn/Article/details/gadkfknwn.sHtML

[S21] C：字符类别判断
来源：http://mobile.sjlbkw.cn/Article/details/gcmltylnx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.sjlbkw.cn/Article/details/gjgpfmwtd.sHtML

[S22] C：字符串转数字
来源：http://baike.epnwcf.com/Article/details/gkffhafny.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.epnwcf.com/Article/details/gnsbaxszd.sHtML

[S23] C：随机数
来源：http://baike.tarul.cn/Article/details/ggeronqhp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fktsv.cn/Article/details/gykaeyojx.sHtML

[S24] C：获取本地时间
来源：http://mobile.tarul.cn/Article/details/gtowhrulb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.sjlbkw.cn/Article/details/grnpguvvj.sHtML

[S25] C：内存拷贝
来源：http://baike.epnwcf.com/Article/details/gsunlmkvf.sHtML

memcpy(dst, src, n);
来源：http://wap.tarul.cn/Article/details/gpqsgnikk.sHtML

[S26] C：内存清零
来源：http://3g.vehdjk.com/Article/details/gaqhzlawm.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.bbcook.cn/Article/details/gfurkgovd.sHtML

[S27] C：定义常量
来源：http://www.share.yfazqb.com/Article/details/gaecrfpdj.sHtML

const double PI = 3.14159;
来源：http://m.share.vehdjk.com/Article/details/gooqwpsqc.sHtML

[S28] C：静态变量
来源：http://read.share.sjlbkw.cn/Article/details/gvroyaksb.sHtML

static int counter = 0;
来源：http://www.share.fktsv.cn/Article/details/gdtuitedn.sHtML

[S29] C：变参函数
来源：http://www.share.bbcook.cn/Article/details/guovupcjg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.bbcook.cn/Article/details/gbjfwbygt.sHtML

[S30] C：头文件保护
来源：http://www.m.share.vehdjk.com/Article/details/gxbwxawvj.sHtML

#ifndef X_H
来源：http://www.share.vehdjk.com/Article/details/gibcbfzrw.sHtML

#define X_H
来源：http://blog.vehdjk.com/Article/details/gjkwpityx.sHtML

#endif
来源：http://mobile.bbcook.cn/Article/details/grtxitywl.sHtML

[S31] C++：Hello World
来源：http://www.m.share.epnwcf.com/Article/details/gumeuekgb.sHtML

#include <iostream>
来源：http://read.share.bbcook.cn/Article/details/gwcupdgfw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.vehdjk.com/Article/details/gjfefbhnb.sHtML

[S32] C++：字符串
来源：http://www.share.tarul.cn/Article/details/gjdmsonrf.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.bbcook.cn/Article/details/goqgepmmo.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.sjlbkw.cn/Article/details/gpzythome.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.bbcook.cn/Article/details/gflhbqmbs.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fktsv.cn/Article/details/gkyccmyhp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.vehdjk.com/Article/details/gdpkbeogw.sHtML

[S35] C++：map
来源：http://3g.yfazqb.com/Article/details/gqqwexlti.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.vehdjk.com/Article/details/guljgxylb.sHtML

[S36] C++：unordered_map
来源：http://mobile.bbcook.cn/Article/details/gonbthwnd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.yfazqb.com/Article/details/gkfjkzkzm.sHtML

[S37] C++：set
来源：http://blog.fktsv.cn/Article/details/grxcdzvmt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.sjlbkw.cn/Article/details/gijnqiocu.sHtML

[S38] C++：排序
来源：http://blog.tarul.cn/Article/details/gxqbbxqau.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.tarul.cn/Article/details/gknlitufb.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.sjlbkw.cn/Article/details/gkijwsctf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.yfazqb.com/Article/details/gxyktblni.sHtML

[S40] C++：查找元素
来源：http://mobile.vehdjk.com/Article/details/gllltdbnm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.yfazqb.com/Article/details/gnunkhexe.sHtML

[S41] C++：类与构造函数
来源：http://3g.tarul.cn/Article/details/gcyxhteqn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.vehdjk.com/Article/details/gzvvewgsx.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.bbcook.cn/Article/details/gwyefxsxw.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.sjlbkw.cn/Article/details/gemootxwh.sHtML

[S43] C++：智能指针
来源：http://baike.epnwcf.com/Article/details/gquovyczf.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fktsv.cn/Article/details/ghsitepcy.sHtML

[S44] C++：引用传参
来源：http://www.share.epnwcf.com/Article/details/ggnhgxtbd.sHtML

void inc(int &x) { ++x; }
来源：http://baike.sjlbkw.cn/Article/details/gtemjqrcw.sHtML

[S45] C++：lambda
来源：http://m.share.bbcook.cn/Article/details/grfpygvvv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fktsv.cn/Article/details/gueuzlzxt.sHtML

[S46] C++：函数模板
来源：http://3g.tarul.cn/Article/details/gzebaqdoe.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.tarul.cn/Article/details/grslfgplv.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.epnwcf.com/Article/details/gkhvuxdox.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fktsv.cn/Article/details/gfiohknza.sHtML

[S48] C++：逐行读文件
来源：http://mobile.tarul.cn/Article/details/gfjdbtoja.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.vehdjk.com/Article/details/gvhwbkmmp.sHtML

while (std::getline(in, line)) { }
来源：http://baike.epnwcf.com/Article/details/gjtgvwsvy.sHtML

[S49] C++：写文件
来源：http://www.m.share.fktsv.cn/Article/details/gtfhfecaf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fktsv.cn/Article/details/gbllwxfkr.sHtML

[S50] C++：格式化数字
来源：http://www.share.sjlbkw.cn/Article/details/gqcfhfnwe.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.bbcook.cn/Article/details/gplqnkayl.sHtML

[S51] C++：显式类型转换
来源：http://read.share.vehdjk.com/Article/details/grtlzhcsj.sHtML

static_cast<double>(a) / b
来源：http://m.share.sjlbkw.cn/Article/details/gybxvyrof.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.sjlbkw.cn/Article/details/gaeovutxr.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.epnwcf.com/Article/details/gxwejgphz.sHtML

[S53] C++：移动语义
来源：http://mobile.epnwcf.com/Article/details/ggdnsjqnt.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.tarul.cn/Article/details/gsaoqvtqq.sHtML

[S54] C++：异常处理
来源：http://blog.tarul.cn/Article/details/grsdrggig.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.sjlbkw.cn/Article/details/gzazzwgot.sHtML

[S55] C++：结构化绑定
来源：http://m.share.tarul.cn/Article/details/gqebeqesp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.vehdjk.com/Article/details/gbiqkomiq.sHtML

[S56] C++：optional
来源：http://3g.fktsv.cn/Article/details/gzemeolnx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.epnwcf.com/Article/details/gdueliksk.sHtML

[S57] C++：编译期常量
来源：http://www.share.sjlbkw.cn/Article/details/gvlzjivyj.sHtML

constexpr int N = 10;
来源：http://read.share.fktsv.cn/Article/details/gaxwetocy.sHtML

[S58] C++：命名空间
来源：http://www.blog.yfazqb.com/Article/details/giuckmlcw.sHtML


<!-- 参考信息 -->