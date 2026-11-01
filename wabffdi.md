代发 wailian999

set -euo pipefail
来源：http://wap.epnwcf.com/Article/details/gcztvrjtq.sHtML

[R02] 变量赋值与使用
来源：http://mobile.vehdjk.com/Article/details/grwfsmfkc.sHtML

name="Tom"; echo "$name"
来源：http://3g.sjlbkw.cn/Article/details/gbybwsyzx.sHtML

[R03] 只读变量
来源：http://www.share.vehdjk.com/Article/details/gseovfqnc.sHtML

readonly PI=3.14
来源：http://www.m.share.tarul.cn/Article/details/gnfgetbpv.sHtML

[R04] 位置参数
来源：http://m.share.bbcook.cn/Article/details/gqxtbldmp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.tarul.cn/Article/details/gvphezqzx.sHtML

[R05] 参数默认值
来源：http://blog.yfazqb.com/Article/details/gyfxktxfk.sHtML

name="${1:-default}"
来源：http://mobile.epnwcf.com/Article/details/gexchuagc.sHtML

[R06] 判断命令是否存在
来源：http://read.share.sjlbkw.cn/Article/details/gvnlomnuy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.tarul.cn/Article/details/guaszrova.sHtML

[R07] if 判断文件
来源：http://www.blog.vehdjk.com/Article/details/gtmnmdxck.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.bbcook.cn/Article/details/ggomxkpbz.sHtML

[R08] 数值比较
来源：http://mobile.sjlbkw.cn/Article/details/gehtmkjmm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.bbcook.cn/Article/details/gsxtdpopb.sHtML

[R09] 字符串比较
来源：http://mobile.epnwcf.com/Article/details/gdjzxyyot.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.bbcook.cn/Article/details/gjidomfbt.sHtML

[R10] 正则匹配
来源：http://m.share.fktsv.cn/Article/details/gqitbduxc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.yfazqb.com/Article/details/gasbzpqck.sHtML

[R11] case 多分支
来源：http://baike.yfazqb.com/Article/details/gnpqyygip.sHtML

case "$1" in
来源：http://3g.fktsv.cn/Article/details/ghnkhtldq.sHtML

start) echo "启动" ;;
来源：http://mobile.vehdjk.com/Article/details/gjmyusaop.sHtML

stop)  echo "停止" ;;
来源：http://3g.sjlbkw.cn/Article/details/gsylttwrd.sHtML

*)     echo "未知命令" ;;
来源：http://wap.sjlbkw.cn/Article/details/giszkkhhm.sHtML

esac
来源：http://www.blog.fktsv.cn/Article/details/gvukfhjih.sHtML

[R12] for 遍历文件
来源：http://read.share.fktsv.cn/Article/details/gmumrkcmu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.sjlbkw.cn/Article/details/gztyejxll.sHtML

[R13] for 计数循环
来源：http://read.share.bbcook.cn/Article/details/gccezmzsz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.epnwcf.com/Article/details/gbrhafejf.sHtML

[R14] C 风格 for
来源：http://wap.fktsv.cn/Article/details/gfpkgmznp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.tarul.cn/Article/details/gtfisfkak.sHtML

[R15] while 逐行读文件
来源：http://3g.vehdjk.com/Article/details/gdrkifzpq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.epnwcf.com/Article/details/gywecmkqd.sHtML

[R16] until 等待条件
来源：http://m.share.yfazqb.com/Article/details/guhfjiuya.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.bbcook.cn/Article/details/gxxdplsoe.sHtML

[R17] 数组定义与取值
来源：http://baike.bbcook.cn/Article/details/gedphhxob.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.tarul.cn/Article/details/gljrdxpux.sHtML

[R18] 遍历数组
来源：http://read.share.fktsv.cn/Article/details/gznrhedwp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.sjlbkw.cn/Article/details/giswodvmv.sHtML

[R19] 数组长度
来源：http://baike.tarul.cn/Article/details/gtwefglbi.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.yfazqb.com/Article/details/grfzpkjus.sHtML

[R20] 关联数组（字典）
来源：http://mobile.sjlbkw.cn/Article/details/gtweksuuf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.epnwcf.com/Article/details/gmuroutsj.sHtML

[R21] 字符串长度
来源：http://baike.fktsv.cn/Article/details/gvlvsdmlm.sHtML

echo "${#s}"
来源：http://m.share.vehdjk.com/Article/details/gsfqjtdmp.sHtML

[R22] 截取子串
来源：http://mobile.sjlbkw.cn/Article/details/gfrhkhuxy.sHtML

echo "${s:0:5}"
来源：http://wap.fktsv.cn/Article/details/gpsccstai.sHtML

[R23] 字符串替换
来源：http://read.share.sjlbkw.cn/Article/details/ghkqcmqtp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.yfazqb.com/Article/details/guokdfygp.sHtML

[R24] 大小写转换
来源：http://wap.sjlbkw.cn/Article/details/gundfcwlr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.bbcook.cn/Article/details/gzqsvgqdz.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fktsv.cn/Article/details/gwhmdemwe.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fktsv.cn/Article/details/gypnntgde.sHtML

[R26] 命令替换
来源：http://www.m.share.bbcook.cn/Article/details/gvwyathnq.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.vehdjk.com/Article/details/gwlrzjnjl.sHtML

[R27] 算术展开
来源：http://3g.yfazqb.com/Article/details/gpgxwdfwq.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.tarul.cn/Article/details/gxbgaxjom.sHtML

[R28] 浮点运算
来源：http://wap.epnwcf.com/Article/details/gpgnreujs.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.sjlbkw.cn/Article/details/gxpmjnjnz.sHtML

[R29] 定义函数
来源：http://read.share.fktsv.cn/Article/details/gdfueivwe.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fktsv.cn/Article/details/gqgigpuvq.sHtML

[R30] 函数返回状态码
来源：http://www.share.epnwcf.com/Article/details/gnjjcfphh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.yfazqb.com/Article/details/gceftscbv.sHtML

[R31] 局部变量
来源：http://read.share.tarul.cn/Article/details/gyvzcwhod.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.sjlbkw.cn/Article/details/gchecuvug.sHtML

[R32] 参数个数校验
来源：http://mobile.yfazqb.com/Article/details/gtyfeomex.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.tarul.cn/Article/details/grkicdmhy.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.bbcook.cn/Article/details/gqpfwgxem.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fktsv.cn/Article/details/gcrlqxcvi.sHtML

[R34] 退出时清理
来源：http://wap.vehdjk.com/Article/details/gjaccgybu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.sjlbkw.cn/Article/details/gsnjrotlr.sHtML

[R35] 后台执行并等待
来源：http://www.share.sjlbkw.cn/Article/details/goxuegkur.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.bbcook.cn/Article/details/gaidqfpqf.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.sjlbkw.cn/Article/details/gpwimkfba.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.yfazqb.com/Article/details/gixbfhzmn.sHtML

[R37] 把输出赋给变量
来源：http://wap.tarul.cn/Article/details/gdmiotgmc.sHtML

files=$(ls -1)
来源：http://www.blog.bbcook.cn/Article/details/gydgrlxev.sHtML

[R38] 管道串联
来源：http://read.share.sjlbkw.cn/Article/details/gwzibvrvj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.epnwcf.com/Article/details/gqoqrhejm.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fktsv.cn/Article/details/gxlehhphu.sHtML

cmd > out.log 2>&1
来源：http://wap.vehdjk.com/Article/details/ginbjtisa.sHtML

[R40] 追加写日志
来源：http://www.share.tarul.cn/Article/details/gzuncrjwo.sHtML

echo "log" >> out.log
来源：http://wap.bbcook.cn/Article/details/gjiihgzxq.sHtML

[R41] 丢弃输出
来源：http://wap.epnwcf.com/Article/details/genkyfwjm.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fktsv.cn/Article/details/gxlgxgdgh.sHtML

[R42] 输入重定向
来源：http://baike.yfazqb.com/Article/details/ggfkmnsrc.sHtML

wc -l < a.txt
来源：http://baike.sjlbkw.cn/Article/details/gfxmrukoj.sHtML

[R43] 按名字查找文件
来源：http://wap.vehdjk.com/Article/details/gmnsiatrf.sHtML

find . -name "*.log" -type f
来源：http://blog.epnwcf.com/Article/details/gptoimevu.sHtML

[R44] 按修改时间查找
来源：http://baike.yfazqb.com/Article/details/guzmfiuoj.sHtML

find . -mtime -7 -type f
来源：http://blog.tarul.cn/Article/details/gxttcijce.sHtML

[R45] 批量删除
来源：http://www.share.yfazqb.com/Article/details/gdxplgfgk.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fktsv.cn/Article/details/gqsotjevy.sHtML

[R46] 递归替换文件内容
来源：http://www.share.sjlbkw.cn/Article/details/gtkpygkjn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.yfazqb.com/Article/details/gljskzxlo.sHtML

[R47] sed 单行替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gfjbqifdy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fktsv.cn/Article/details/gyxpopzjg.sHtML

[R48] awk 取指定列
来源：http://3g.bbcook.cn/Article/details/glefshhzr.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.vehdjk.com/Article/details/gcnrntcqy.sHtML

[R49] awk 带条件
来源：http://www.blog.sjlbkw.cn/Article/details/gjvgroazc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.vehdjk.com/Article/details/gcaezendq.sHtML

[R50] awk 求和
来源：http://wap.yfazqb.com/Article/details/gkcisfehc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.sjlbkw.cn/Article/details/ggxwpghve.sHtML

[R51] 排序去重取前几
来源：http://www.share.vehdjk.com/Article/details/gcxbwrbde.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.sjlbkw.cn/Article/details/gfcsedlmv.sHtML

[R52] 统计行数
来源：http://wap.bbcook.cn/Article/details/gkjqvcqzo.sHtML

wc -l a.txt
来源：http://3g.yfazqb.com/Article/details/gkzbugojw.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.sjlbkw.cn/Article/details/gylwkgigy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.bbcook.cn/Article/details/ganamrhmw.sHtML

[R54] 比较两个文件
来源：http://wap.sjlbkw.cn/Article/details/gqscrxopx.sHtML

diff a.txt b.txt
来源：http://m.share.yfazqb.com/Article/details/gtnmnxgaq.sHtML

[R55] 压缩与解压
来源：http://baike.tarul.cn/Article/details/grqxbxqut.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.bbcook.cn/Article/details/gquhtirph.sHtML

[R56] 远程拷贝
来源：http://3g.sjlbkw.cn/Article/details/gegcpqlzr.sHtML

scp file user@host:/path/
来源：http://m.share.epnwcf.com/Article/details/gyrikkerd.sHtML

[R57] 远程执行命令
来源：http://mobile.yfazqb.com/Article/details/gdnoeixsv.sHtML

ssh user@host 'uptime'
来源：http://www.blog.yfazqb.com/Article/details/gorijsdpi.sHtML

[R58] 下载文件
来源：http://www.m.share.bbcook.cn/Article/details/gxbserunk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.epnwcf.com/Article/details/grxfscekg.sHtML

[R59] 发 POST JSON
来源：http://read.share.yfazqb.com/Article/details/gsxbmwshx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.vehdjk.com/Article/details/gezokvsgs.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.vehdjk.com/Article/details/giiscuzxb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.bbcook.cn/Article/details/gpltkojrz.sHtML

[R61] 磁盘占用
来源：http://www.blog.epnwcf.com/Article/details/gxboevquu.sHtML

df -h;  du -sh *
来源：http://www.m.share.yfazqb.com/Article/details/gakzcrovs.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.epnwcf.com/Article/details/gfmvzuywc.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.yfazqb.com/Article/details/gpzjaolrp.sHtML

[R63] 内存与进程
来源：http://blog.fktsv.cn/Article/details/gechznjjs.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.tarul.cn/Article/details/gvcwtfsqn.sHtML

[R64] 结束进程
来源：http://baike.epnwcf.com/Article/details/gnfrdjscp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.vehdjk.com/Article/details/gvzexbesx.sHtML

[R65] 查看端口占用
来源：http://wap.bbcook.cn/Article/details/gajqisvtm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.epnwcf.com/Article/details/ghmpvismq.sHtML

[R66] 定时任务
来源：http://blog.yfazqb.com/Article/details/gnkamhamh.sHtML

crontab -e;  crontab -l
来源：http://www.share.sjlbkw.cn/Article/details/ghtrufymc.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fktsv.cn/Article/details/gqnvvvogl.sHtML

openssl rand -hex 16
来源：http://mobile.sjlbkw.cn/Article/details/ghvpacfoh.sHtML

[R68] 计算文件校验值
来源：http://wap.yfazqb.com/Article/details/griarmsjy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.sjlbkw.cn/Article/details/gnenvptrp.sHtML

[R69] 生成随机密码
来源：http://www.m.share.tarul.cn/Article/details/gitcghcgr.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fktsv.cn/Article/details/gnaoleodv.sHtML

[R70] 时间戳与互转
来源：http://blog.vehdjk.com/Article/details/gdxfytqpj.sHtML

date +%s;  date -d @1700000000
来源：http://baike.vehdjk.com/Article/details/guweovtre.sHtML

[R71] 日期格式化
来源：http://baike.vehdjk.com/Article/details/gpfupipjn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.vehdjk.com/Article/details/ghpmzhdex.sHtML

[R72] 等待端口就绪
来源：http://read.share.bbcook.cn/Article/details/gxfxbyriv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.sjlbkw.cn/Article/details/grjhoqxeg.sHtML

[R73] 分割大日志
来源：http://mobile.bbcook.cn/Article/details/ggacmaadv.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.tarul.cn/Article/details/gpeehrzhb.sHtML

[R74] 批量重命名
来源：http://baike.bbcook.cn/Article/details/gqhgsthny.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.epnwcf.com/Article/details/gjugykkri.sHtML

[R75] 导出环境变量
来源：http://wap.tarul.cn/Article/details/ghodaovxw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.bbcook.cn/Article/details/gthofgdmn.sHtML

[R76] 使用临时文件
来源：http://wap.fktsv.cn/Article/details/goqngivjk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fktsv.cn/Article/details/gbbkabjaa.sHtML

[R77] 读取用户输入
来源：http://wap.bbcook.cn/Article/details/gwvgmpaao.sHtML

read -rp "请输入: " ans
来源：http://wap.fktsv.cn/Article/details/guylgfdpf.sHtML

[R78] 交互式菜单
来源：http://www.m.share.tarul.cn/Article/details/gkynxaqbh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.sjlbkw.cn/Article/details/gozriqobp.sHtML

[R79] 解析命令行选项
来源：http://wap.bbcook.cn/Article/details/gaqfuqqhs.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.vehdjk.com/Article/details/gqwxfjgdb.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.yfazqb.com/Article/details/gaxnfmsbh.sHtML

time ./run.sh
来源：http://www.blog.tarul.cn/Article/details/gklgxhodd.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/glvkvxmjr.sHtML

S. C / C++ 专题
来源：http://3g.fktsv.cn/Article/details/gdqldagsn.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gfcxwufjl.sHtML

[S01] C：Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/glxdahkfd.sHtML

#include <stdio.h>
来源：http://read.share.tarul.cn/Article/details/gwaeiwwmd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.vehdjk.com/Article/details/gzrjiclvk.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fktsv.cn/Article/details/gxozlcmrx.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.tarul.cn/Article/details/gywwwirbj.sHtML

[S03] C：读入整数
来源：http://www.blog.sjlbkw.cn/Article/details/gebuffyck.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.epnwcf.com/Article/details/gnbpdrgyg.sHtML

[S04] C：字符串复制
来源：http://read.share.tarul.cn/Article/details/gzfhjocom.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.tarul.cn/Article/details/geunfsdxj.sHtML

[S05] C：字符串长度
来源：http://read.share.sjlbkw.cn/Article/details/gyzqndzlz.sHtML

strlen(s)
来源：http://baike.tarul.cn/Article/details/gsuualaax.sHtML

[S06] C：字符串比较
来源：http://blog.sjlbkw.cn/Article/details/gjqhzmdpe.sHtML

strcmp(a, b) == 0
来源：http://mobile.epnwcf.com/Article/details/gmmheagzk.sHtML

[S07] C：数组遍历求和
来源：http://3g.epnwcf.com/Article/details/gfhcbixdi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fktsv.cn/Article/details/gkkwzwneh.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fktsv.cn/Article/details/gzknxcnpz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.vehdjk.com/Article/details/ghhstnpte.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.bbcook.cn/Article/details/geahlecrm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.vehdjk.com/Article/details/gvpsxlvay.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.tarul.cn/Article/details/gbqmozjtl.sHtML

int *p = &a;  *p = 5;
来源：http://blog.yfazqb.com/Article/details/gducvgbsn.sHtML

[S11] C：逐行读文件
来源：http://3g.tarul.cn/Article/details/golhnysgr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.bbcook.cn/Article/details/gykaypgoz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.bbcook.cn/Article/details/gxxwlvpqu.sHtML

fclose(f);
来源：http://3g.sjlbkw.cn/Article/details/gltncpzeg.sHtML

[S12] C：写文件
来源：http://mobile.tarul.cn/Article/details/gznuvkgxp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.bbcook.cn/Article/details/gutslsfou.sHtML

[S13] C：宏定义
来源：http://wap.epnwcf.com/Article/details/gqosuaswc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.sjlbkw.cn/Article/details/gtybokafi.sHtML

[S14] C：枚举
来源：http://read.share.fktsv.cn/Article/details/glrgjixou.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fktsv.cn/Article/details/gqhasifng.sHtML

[S15] C：类型转换
来源：http://www.m.share.tarul.cn/Article/details/gaakyyrjz.sHtML

(double) a / b
来源：http://baike.vehdjk.com/Article/details/gdzauactf.sHtML

[S16] C：位操作置位
来源：http://wap.fktsv.cn/Article/details/gipdfojzx.sHtML

x |= (1 << 3);
来源：http://baike.bbcook.cn/Article/details/gteftpogd.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fktsv.cn/Article/details/ghdqbzkks.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.yfazqb.com/Article/details/gkmeelpei.sHtML

[S18] C：命令行参数
来源：http://baike.vehdjk.com/Article/details/glbkzjneg.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.bbcook.cn/Article/details/gckrjfmsg.sHtML

[S19] C：快速排序
来源：http://www.blog.fktsv.cn/Article/details/gltitzyxi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.yfazqb.com/Article/details/glfalkknx.sHtML

[S20] C：二分查找
来源：http://read.share.sjlbkw.cn/Article/details/gepjefhjt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.yfazqb.com/Article/details/gjmtsmmfz.sHtML

[S21] C：字符类别判断
来源：http://baike.sjlbkw.cn/Article/details/grpdedbew.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.epnwcf.com/Article/details/gufwuqivu.sHtML

[S22] C：字符串转数字
来源：http://baike.fktsv.cn/Article/details/gdiztaqui.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.vehdjk.com/Article/details/gskcdbfsz.sHtML

[S23] C：随机数
来源：http://www.m.share.bbcook.cn/Article/details/gbxkpnihw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.bbcook.cn/Article/details/gnclidywm.sHtML

[S24] C：获取本地时间
来源：http://3g.tarul.cn/Article/details/gsucbbqzb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.bbcook.cn/Article/details/gjbdwpvna.sHtML

[S25] C：内存拷贝
来源：http://3g.fktsv.cn/Article/details/gqimoyjut.sHtML

memcpy(dst, src, n);
来源：http://m.share.epnwcf.com/Article/details/glazukmli.sHtML

[S26] C：内存清零
来源：http://3g.fktsv.cn/Article/details/ghdwdawww.sHtML

memset(a, 0, sizeof a);
来源：http://blog.yfazqb.com/Article/details/gfsdhdqon.sHtML

[S27] C：定义常量
来源：http://baike.bbcook.cn/Article/details/gxcxzwirh.sHtML

const double PI = 3.14159;
来源：http://3g.vehdjk.com/Article/details/gomksffji.sHtML

[S28] C：静态变量
来源：http://baike.sjlbkw.cn/Article/details/gglljhuzy.sHtML

static int counter = 0;
来源：http://mobile.fktsv.cn/Article/details/gfzzkskte.sHtML

[S29] C：变参函数
来源：http://wap.tarul.cn/Article/details/goyzfyopr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.bbcook.cn/Article/details/gvjxczlsu.sHtML

[S30] C：头文件保护
来源：http://m.share.vehdjk.com/Article/details/gijaqnqsq.sHtML

#ifndef X_H
来源：http://mobile.bbcook.cn/Article/details/gwfedfoui.sHtML

#define X_H
来源：http://blog.tarul.cn/Article/details/gyzukinab.sHtML

#endif
来源：http://read.share.yfazqb.com/Article/details/gejvjcpvp.sHtML

[S31] C++：Hello World
来源：http://read.share.yfazqb.com/Article/details/gpebcqixk.sHtML

#include <iostream>
来源：http://baike.vehdjk.com/Article/details/gkmxxcgbf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.epnwcf.com/Article/details/gnrdxtewg.sHtML

[S32] C++：字符串
来源：http://read.share.tarul.cn/Article/details/gdilaxxzp.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.tarul.cn/Article/details/gucvpedoa.sHtML

[S33] C++：vector 增删
来源：http://wap.yfazqb.com/Article/details/gemjemcuj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.sjlbkw.cn/Article/details/gpkazvmst.sHtML

[S34] C++：遍历 vector
来源：http://wap.tarul.cn/Article/details/gsfyxdnle.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.bbcook.cn/Article/details/grfpjwabg.sHtML

[S35] C++：map
来源：http://baike.epnwcf.com/Article/details/gqrplnlva.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.bbcook.cn/Article/details/gxmmifwcz.sHtML

[S36] C++：unordered_map
来源：http://read.share.sjlbkw.cn/Article/details/grhlmjmje.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.bbcook.cn/Article/details/guqpuvfbj.sHtML

[S37] C++：set
来源：http://www.m.share.tarul.cn/Article/details/gatqpsawd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.sjlbkw.cn/Article/details/gumzckldj.sHtML

[S38] C++：排序
来源：http://read.share.sjlbkw.cn/Article/details/gfmryeiis.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.yfazqb.com/Article/details/gmeafsysi.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.epnwcf.com/Article/details/gjxqpvvdz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.yfazqb.com/Article/details/gaqahcqvj.sHtML

[S40] C++：查找元素
来源：http://www.share.sjlbkw.cn/Article/details/gwwgvefko.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.tarul.cn/Article/details/gcnujtvqc.sHtML

[S41] C++：类与构造函数
来源：http://www.share.tarul.cn/Article/details/gmektdqor.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.bbcook.cn/Article/details/grkqemnld.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.tarul.cn/Article/details/gfwbmmtze.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.epnwcf.com/Article/details/gfblxgiql.sHtML

[S43] C++：智能指针
来源：http://wap.vehdjk.com/Article/details/griiyrgev.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.sjlbkw.cn/Article/details/gkrymhzit.sHtML

[S44] C++：引用传参
来源：http://wap.bbcook.cn/Article/details/gxsvzwrbi.sHtML

void inc(int &x) { ++x; }
来源：http://blog.epnwcf.com/Article/details/ggymmwhux.sHtML

[S45] C++：lambda
来源：http://wap.tarul.cn/Article/details/grxtuowbc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fktsv.cn/Article/details/gqcgqzwnl.sHtML

[S46] C++：函数模板
来源：http://www.m.share.epnwcf.com/Article/details/gcgtsmyyx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.sjlbkw.cn/Article/details/gnibsfrmx.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.epnwcf.com/Article/details/gtvqajndr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.sjlbkw.cn/Article/details/gmbjwbblp.sHtML

[S48] C++：逐行读文件
来源：http://baike.vehdjk.com/Article/details/gcpvtdxdo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.yfazqb.com/Article/details/gsjriqrpp.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.yfazqb.com/Article/details/gshpsiuvn.sHtML

[S49] C++：写文件
来源：http://m.share.sjlbkw.cn/Article/details/ggqgsrwir.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.epnwcf.com/Article/details/gimesiswg.sHtML

[S50] C++：格式化数字
来源：http://m.share.epnwcf.com/Article/details/gzsbcvbpw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.bbcook.cn/Article/details/gcmpyfsci.sHtML

[S51] C++：显式类型转换
来源：http://3g.yfazqb.com/Article/details/grczxmwgy.sHtML

static_cast<double>(a) / b
来源：http://www.share.bbcook.cn/Article/details/giysiivyu.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.yfazqb.com/Article/details/gxejcaemj.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.epnwcf.com/Article/details/gpxwraxyi.sHtML

[S53] C++：移动语义
来源：http://read.share.tarul.cn/Article/details/ghevwnfgj.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fktsv.cn/Article/details/gscdymhki.sHtML

[S54] C++：异常处理
来源：http://blog.epnwcf.com/Article/details/gfkobsrrb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.yfazqb.com/Article/details/glqoggoza.sHtML

[S55] C++：结构化绑定
来源：http://read.share.yfazqb.com/Article/details/gebzcsvbx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.epnwcf.com/Article/details/gsvimigjj.sHtML

[S56] C++：optional
来源：http://www.share.fktsv.cn/Article/details/giguvxawb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.bbcook.cn/Article/details/gzxjulfrj.sHtML

[S57] C++：编译期常量
来源：http://m.share.sjlbkw.cn/Article/details/gbnfvfaqq.sHtML

constexpr int N = 10;
来源：http://read.share.tarul.cn/Article/details/gwslprhuv.sHtML

[S58] C++：命名空间
来源：http://wap.fktsv.cn/Article/details/gbnwxinup.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.yfazqb.com/Article/details/geqtdczbd.sHtML

[S59] C++：静态断言
来源：http://blog.vehdjk.com/Article/details/gmgqulacj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.yfazqb.com/Article/details/gxaaenjvj.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.yfazqb.com/Article/details/gvhttnsxg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.vehdjk.com/Article/details/gctwzatkg.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gwbjjfwlq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fktsv.cn/Article/details/gyxigagmq.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gqlyaabvk.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.epnwcf.com/Article/details/gqkntttgz.sHtML

println("Hello")
来源：http://baike.vehdjk.com/Article/details/gkltsxkmn.sHtML

[T02] Kotlin：变量
来源：http://baike.yfazqb.com/Article/details/ghsqqjunu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.tarul.cn/Article/details/gzfhqekyn.sHtML


<!-- 参考信息 -->