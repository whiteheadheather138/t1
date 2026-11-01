代发 wailian999

set -euo pipefail
来源：http://3g.vehdjk.com/Article/details/gfmkckpik.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fktsv.cn/Article/details/gjbvvklar.sHtML

name="Tom"; echo "$name"
来源：http://wap.vehdjk.com/Article/details/gahsdpqed.sHtML

[R03] 只读变量
来源：http://www.blog.epnwcf.com/Article/details/gqchuqdqs.sHtML

readonly PI=3.14
来源：http://mobile.vehdjk.com/Article/details/gbpsvzhhz.sHtML

[R04] 位置参数
来源：http://mobile.vehdjk.com/Article/details/ggmbswmfp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.yfazqb.com/Article/details/gvnrxjvao.sHtML

[R05] 参数默认值
来源：http://www.m.share.yfazqb.com/Article/details/gvlkbjofj.sHtML

name="${1:-default}"
来源：http://mobile.bbcook.cn/Article/details/gfltxrfkb.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.yfazqb.com/Article/details/gidphglei.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.sjlbkw.cn/Article/details/ghhgaisnv.sHtML

[R07] if 判断文件
来源：http://3g.sjlbkw.cn/Article/details/giupjkufo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.bbcook.cn/Article/details/glxkdkgmk.sHtML

[R08] 数值比较
来源：http://3g.tarul.cn/Article/details/gvdlrwwec.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.vehdjk.com/Article/details/gpxzibxgz.sHtML

[R09] 字符串比较
来源：http://read.share.epnwcf.com/Article/details/gnjkrucrd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.bbcook.cn/Article/details/gbuwjfrdm.sHtML

[R10] 正则匹配
来源：http://www.share.bbcook.cn/Article/details/gcwzdwfqv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.yfazqb.com/Article/details/gkpewgnjp.sHtML

[R11] case 多分支
来源：http://m.share.sjlbkw.cn/Article/details/geqdwrdjj.sHtML

case "$1" in
来源：http://baike.vehdjk.com/Article/details/gzbmkzfod.sHtML

start) echo "启动" ;;
来源：http://read.share.vehdjk.com/Article/details/gfstpgoyl.sHtML

stop)  echo "停止" ;;
来源：http://blog.yfazqb.com/Article/details/gbespsqem.sHtML

*)     echo "未知命令" ;;
来源：http://wap.vehdjk.com/Article/details/glhxoffbu.sHtML

esac
来源：http://www.share.epnwcf.com/Article/details/gzoukvmjs.sHtML

[R12] for 遍历文件
来源：http://www.m.share.bbcook.cn/Article/details/gxilozjkp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fktsv.cn/Article/details/gmmpwchex.sHtML

[R13] for 计数循环
来源：http://baike.bbcook.cn/Article/details/gkjrtiuhp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.epnwcf.com/Article/details/gidhdlihl.sHtML

[R14] C 风格 for
来源：http://3g.yfazqb.com/Article/details/gyrhgtgli.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fktsv.cn/Article/details/gaoxxwwtg.sHtML

[R15] while 逐行读文件
来源：http://read.share.fktsv.cn/Article/details/ggasfimbt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.yfazqb.com/Article/details/gfqqinnns.sHtML

[R16] until 等待条件
来源：http://baike.fktsv.cn/Article/details/gcqzcbtgy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fktsv.cn/Article/details/gtqxtunao.sHtML

[R17] 数组定义与取值
来源：http://wap.bbcook.cn/Article/details/gemonvoyp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.sjlbkw.cn/Article/details/gxqnitzdy.sHtML

[R18] 遍历数组
来源：http://blog.yfazqb.com/Article/details/gzbtyutcl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.yfazqb.com/Article/details/gkvicmhja.sHtML

[R19] 数组长度
来源：http://wap.bbcook.cn/Article/details/gipmbtsqz.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.vehdjk.com/Article/details/gtmoxhjrj.sHtML

[R20] 关联数组（字典）
来源：http://wap.sjlbkw.cn/Article/details/glwbdvxtl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.yfazqb.com/Article/details/gygavaxvu.sHtML

[R21] 字符串长度
来源：http://baike.bbcook.cn/Article/details/gbautjfqi.sHtML

echo "${#s}"
来源：http://www.share.tarul.cn/Article/details/gjasjfllh.sHtML

[R22] 截取子串
来源：http://www.m.share.yfazqb.com/Article/details/gdsulewqf.sHtML

echo "${s:0:5}"
来源：http://baike.bbcook.cn/Article/details/gborwfmqa.sHtML

[R23] 字符串替换
来源：http://read.share.yfazqb.com/Article/details/gfgkgzvkc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.epnwcf.com/Article/details/gmnuscelv.sHtML

[R24] 大小写转换
来源：http://www.share.epnwcf.com/Article/details/gziujkbcn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.bbcook.cn/Article/details/guoprfjlu.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.sjlbkw.cn/Article/details/gsnciqpbn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.epnwcf.com/Article/details/gjybgwdpd.sHtML

[R26] 命令替换
来源：http://3g.epnwcf.com/Article/details/glhstpgxf.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.tarul.cn/Article/details/gjyxjltik.sHtML

[R27] 算术展开
来源：http://baike.bbcook.cn/Article/details/gvsgzpfil.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.epnwcf.com/Article/details/gcrnflhqc.sHtML

[R28] 浮点运算
来源：http://read.share.fktsv.cn/Article/details/gjfgizsnn.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.sjlbkw.cn/Article/details/gfckqywvj.sHtML

[R29] 定义函数
来源：http://baike.yfazqb.com/Article/details/gwlajhvfe.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.tarul.cn/Article/details/guzlhkdiu.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fktsv.cn/Article/details/gucjyftan.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.yfazqb.com/Article/details/glddzzkcu.sHtML

[R31] 局部变量
来源：http://www.m.share.epnwcf.com/Article/details/gqfjvnzcx.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.epnwcf.com/Article/details/gmfsjqgvm.sHtML

[R32] 参数个数校验
来源：http://wap.sjlbkw.cn/Article/details/gahovhrxk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fktsv.cn/Article/details/gfajurzlv.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.bbcook.cn/Article/details/gpbbpzcym.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.tarul.cn/Article/details/gyxewkqvv.sHtML

[R34] 退出时清理
来源：http://m.share.epnwcf.com/Article/details/gpyruxsjl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.bbcook.cn/Article/details/gwcpiyywz.sHtML

[R35] 后台执行并等待
来源：http://blog.bbcook.cn/Article/details/gejhlnlgh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.bbcook.cn/Article/details/gquicisum.sHtML

[R36] 并发执行多个任务
来源：http://wap.fktsv.cn/Article/details/gazgutmoj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.bbcook.cn/Article/details/gjicsbrzl.sHtML

[R37] 把输出赋给变量
来源：http://blog.fktsv.cn/Article/details/gfawdbkso.sHtML

files=$(ls -1)
来源：http://blog.yfazqb.com/Article/details/gjpymorkk.sHtML

[R38] 管道串联
来源：http://blog.bbcook.cn/Article/details/gfjhfwdmc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.bbcook.cn/Article/details/gckpovwav.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.vehdjk.com/Article/details/gcglveylb.sHtML

cmd > out.log 2>&1
来源：http://m.share.vehdjk.com/Article/details/gvihtigdj.sHtML

[R40] 追加写日志
来源：http://www.m.share.fktsv.cn/Article/details/gbrhqfxqg.sHtML

echo "log" >> out.log
来源：http://3g.bbcook.cn/Article/details/gqaqcbuon.sHtML

[R41] 丢弃输出
来源：http://mobile.vehdjk.com/Article/details/gafegefgs.sHtML

cmd >/dev/null 2>&1
来源：http://blog.tarul.cn/Article/details/gxczwkxor.sHtML

[R42] 输入重定向
来源：http://3g.epnwcf.com/Article/details/gbydfyrbc.sHtML

wc -l < a.txt
来源：http://mobile.yfazqb.com/Article/details/gvupinucf.sHtML

[R43] 按名字查找文件
来源：http://read.share.bbcook.cn/Article/details/gjnzpvzuz.sHtML

find . -name "*.log" -type f
来源：http://mobile.sjlbkw.cn/Article/details/gwugxnhpm.sHtML

[R44] 按修改时间查找
来源：http://wap.tarul.cn/Article/details/gzzwwueyw.sHtML

find . -mtime -7 -type f
来源：http://www.blog.epnwcf.com/Article/details/gkifelcqi.sHtML

[R45] 批量删除
来源：http://3g.yfazqb.com/Article/details/gzybnegdi.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fktsv.cn/Article/details/gwayxgnky.sHtML

[R46] 递归替换文件内容
来源：http://mobile.yfazqb.com/Article/details/gycveozua.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.epnwcf.com/Article/details/gudxcoolt.sHtML

[R47] sed 单行替换
来源：http://mobile.vehdjk.com/Article/details/ghpjvmzeb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.epnwcf.com/Article/details/gbdcfjfbq.sHtML

[R48] awk 取指定列
来源：http://baike.bbcook.cn/Article/details/gniefmtzc.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.yfazqb.com/Article/details/gkmsteque.sHtML

[R49] awk 带条件
来源：http://read.share.fktsv.cn/Article/details/gseqghdbx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.vehdjk.com/Article/details/gzdskzzho.sHtML

[R50] awk 求和
来源：http://www.blog.epnwcf.com/Article/details/gkswygisv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fktsv.cn/Article/details/goqfhllvv.sHtML

[R51] 排序去重取前几
来源：http://wap.sjlbkw.cn/Article/details/ggxhbmgyi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.epnwcf.com/Article/details/gdsgebpeo.sHtML

[R52] 统计行数
来源：http://m.share.sjlbkw.cn/Article/details/gnmbdvofh.sHtML

wc -l a.txt
来源：http://m.share.tarul.cn/Article/details/gfspruwhg.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.yfazqb.com/Article/details/guxujinvo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.bbcook.cn/Article/details/gakqqqvxj.sHtML

[R54] 比较两个文件
来源：http://3g.yfazqb.com/Article/details/gbtljbrfd.sHtML

diff a.txt b.txt
来源：http://baike.bbcook.cn/Article/details/gkuptpind.sHtML

[R55] 压缩与解压
来源：http://www.share.epnwcf.com/Article/details/ghbigvxxu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.bbcook.cn/Article/details/gysvlmrvb.sHtML

[R56] 远程拷贝
来源：http://mobile.epnwcf.com/Article/details/gdonpthwp.sHtML

scp file user@host:/path/
来源：http://read.share.fktsv.cn/Article/details/gqtccvdvp.sHtML

[R57] 远程执行命令
来源：http://blog.yfazqb.com/Article/details/gtsdrxyeg.sHtML

ssh user@host 'uptime'
来源：http://wap.bbcook.cn/Article/details/gxkqnkhie.sHtML

[R58] 下载文件
来源：http://read.share.sjlbkw.cn/Article/details/gcdkqxkcj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.vehdjk.com/Article/details/gobevlcot.sHtML

[R59] 发 POST JSON
来源：http://baike.bbcook.cn/Article/details/gqjyosigt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.tarul.cn/Article/details/gedhxlxpx.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.epnwcf.com/Article/details/gfqnszgjf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.tarul.cn/Article/details/gakgkdayr.sHtML

[R61] 磁盘占用
来源：http://mobile.fktsv.cn/Article/details/gaqybtyyu.sHtML

df -h;  du -sh *
来源：http://read.share.yfazqb.com/Article/details/guhgkthnn.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.bbcook.cn/Article/details/gdovgodpu.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.tarul.cn/Article/details/grbthxcij.sHtML

[R63] 内存与进程
来源：http://baike.sjlbkw.cn/Article/details/ghdtdklhl.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.tarul.cn/Article/details/gzhjsobru.sHtML

[R64] 结束进程
来源：http://blog.yfazqb.com/Article/details/gwsgrowgd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.sjlbkw.cn/Article/details/gicghrfqr.sHtML

[R65] 查看端口占用
来源：http://m.share.tarul.cn/Article/details/gducnfryt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.tarul.cn/Article/details/ghfwvlkpm.sHtML

[R66] 定时任务
来源：http://blog.vehdjk.com/Article/details/gymgzopxh.sHtML

crontab -e;  crontab -l
来源：http://read.share.sjlbkw.cn/Article/details/gfvgzssot.sHtML

[R67] 生成随机十六进制串
来源：http://3g.sjlbkw.cn/Article/details/gwgkeoyop.sHtML

openssl rand -hex 16
来源：http://www.blog.epnwcf.com/Article/details/gjxpyqyed.sHtML

[R68] 计算文件校验值
来源：http://mobile.tarul.cn/Article/details/gskkjzcql.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.sjlbkw.cn/Article/details/gvgwegwfc.sHtML

[R69] 生成随机密码
来源：http://3g.sjlbkw.cn/Article/details/gligfcbbz.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.sjlbkw.cn/Article/details/gkrvochct.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fktsv.cn/Article/details/gdrkhrmxk.sHtML

date +%s;  date -d @1700000000
来源：http://wap.tarul.cn/Article/details/gedspoyxa.sHtML

[R71] 日期格式化
来源：http://mobile.bbcook.cn/Article/details/gfiphkuub.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.epnwcf.com/Article/details/glrjgquwv.sHtML

[R72] 等待端口就绪
来源：http://www.share.tarul.cn/Article/details/gtgnmmfcl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.vehdjk.com/Article/details/gnocovohv.sHtML

[R73] 分割大日志
来源：http://baike.yfazqb.com/Article/details/gyjfjwpjc.sHtML

split -l 1000 big.log part_
来源：http://3g.fktsv.cn/Article/details/gnffdfjrv.sHtML

[R74] 批量重命名
来源：http://blog.fktsv.cn/Article/details/gjdnwvfhn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.yfazqb.com/Article/details/giiaqcbsm.sHtML

[R75] 导出环境变量
来源：http://www.share.epnwcf.com/Article/details/gwjbdbnai.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.tarul.cn/Article/details/guzemrwdp.sHtML

[R76] 使用临时文件
来源：http://m.share.epnwcf.com/Article/details/gonfhyrbh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.tarul.cn/Article/details/gxyqafqfh.sHtML

[R77] 读取用户输入
来源：http://www.blog.sjlbkw.cn/Article/details/gwmsvtjwq.sHtML

read -rp "请输入: " ans
来源：http://m.share.yfazqb.com/Article/details/guwjrrfol.sHtML

[R78] 交互式菜单
来源：http://read.share.sjlbkw.cn/Article/details/gzyczvidk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.yfazqb.com/Article/details/gvdvfwzze.sHtML

[R79] 解析命令行选项
来源：http://www.share.bbcook.cn/Article/details/glmdtffdr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.sjlbkw.cn/Article/details/giljfptcu.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.epnwcf.com/Article/details/gtxiiehmi.sHtML

time ./run.sh
来源：http://www.m.share.fktsv.cn/Article/details/gghpvpupy.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gyqsrixsv.sHtML

S. C / C++ 专题
来源：http://read.share.tarul.cn/Article/details/glcthcbsw.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gkexmsrkv.sHtML

[S01] C：Hello World
来源：http://read.share.epnwcf.com/Article/details/gcpephjbq.sHtML

#include <stdio.h>
来源：http://wap.tarul.cn/Article/details/gskssjvea.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fktsv.cn/Article/details/gsvjhrziu.sHtML

[S02] C：变量与格式化输出
来源：http://wap.sjlbkw.cn/Article/details/guvkcazzq.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.bbcook.cn/Article/details/geritpzhr.sHtML

[S03] C：读入整数
来源：http://www.blog.fktsv.cn/Article/details/gucnriweh.sHtML

int x; scanf("%d", &x);
来源：http://m.share.tarul.cn/Article/details/gtyjqsylz.sHtML

[S04] C：字符串复制
来源：http://www.share.vehdjk.com/Article/details/gdexlzdwb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.bbcook.cn/Article/details/gmlbokrmq.sHtML

[S05] C：字符串长度
来源：http://read.share.fktsv.cn/Article/details/gfoijaeux.sHtML

strlen(s)
来源：http://www.m.share.epnwcf.com/Article/details/gpetlinly.sHtML

[S06] C：字符串比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gpabkiemt.sHtML

strcmp(a, b) == 0
来源：http://3g.fktsv.cn/Article/details/grglqxsoy.sHtML

[S07] C：数组遍历求和
来源：http://mobile.vehdjk.com/Article/details/gdbpyvbjs.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.epnwcf.com/Article/details/gsuvmwlqz.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.sjlbkw.cn/Article/details/gcksgdqcf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.bbcook.cn/Article/details/gnnheumha.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.yfazqb.com/Article/details/gcdywhckk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.epnwcf.com/Article/details/gkzwwqtzi.sHtML

[S10] C：指针与解引用
来源：http://3g.sjlbkw.cn/Article/details/gprfkmfbf.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fktsv.cn/Article/details/gxrhlgnqc.sHtML

[S11] C：逐行读文件
来源：http://blog.bbcook.cn/Article/details/gfjdretwx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.vehdjk.com/Article/details/grqhysgjw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.bbcook.cn/Article/details/gcdxdyaqa.sHtML

fclose(f);
来源：http://baike.vehdjk.com/Article/details/gmuvohtwv.sHtML

[S12] C：写文件
来源：http://3g.bbcook.cn/Article/details/gbjrimhba.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fktsv.cn/Article/details/giauyyutt.sHtML

[S13] C：宏定义
来源：http://m.share.tarul.cn/Article/details/givpjakof.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.epnwcf.com/Article/details/giobsopqx.sHtML

[S14] C：枚举
来源：http://m.share.yfazqb.com/Article/details/gufrrfcqy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fktsv.cn/Article/details/gmksopbte.sHtML

[S15] C：类型转换
来源：http://www.m.share.bbcook.cn/Article/details/goxwnjpgm.sHtML

(double) a / b
来源：http://baike.bbcook.cn/Article/details/gbkfixmrl.sHtML

[S16] C：位操作置位
来源：http://blog.sjlbkw.cn/Article/details/gcnwagqcs.sHtML

x |= (1 << 3);
来源：http://m.share.sjlbkw.cn/Article/details/gmaykvvys.sHtML

[S17] C：安全拼接字符串
来源：http://baike.bbcook.cn/Article/details/gjvrvdusz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.epnwcf.com/Article/details/gxkfxllbs.sHtML

[S18] C：命令行参数
来源：http://www.share.tarul.cn/Article/details/gbguighos.sHtML

int main(int argc, char **argv)
来源：http://m.share.bbcook.cn/Article/details/gwjczbxsz.sHtML

[S19] C：快速排序
来源：http://www.share.epnwcf.com/Article/details/gytowhjeo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.epnwcf.com/Article/details/gqnqgpxdm.sHtML

[S20] C：二分查找
来源：http://baike.yfazqb.com/Article/details/gscfvlbcu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.vehdjk.com/Article/details/gvbatsgba.sHtML

[S21] C：字符类别判断
来源：http://read.share.fktsv.cn/Article/details/gyndouwvk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.bbcook.cn/Article/details/ggwvehpyb.sHtML

[S22] C：字符串转数字
来源：http://mobile.fktsv.cn/Article/details/gzfmzorkg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.vehdjk.com/Article/details/gcajqbgbc.sHtML

[S23] C：随机数
来源：http://mobile.yfazqb.com/Article/details/gfaptbzwd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fktsv.cn/Article/details/gyfdwdkgv.sHtML

[S24] C：获取本地时间
来源：http://wap.yfazqb.com/Article/details/gyjqtowhd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.bbcook.cn/Article/details/govdstpke.sHtML

[S25] C：内存拷贝
来源：http://www.share.epnwcf.com/Article/details/glqhbjepq.sHtML

memcpy(dst, src, n);
来源：http://blog.bbcook.cn/Article/details/gqgjavfjn.sHtML

[S26] C：内存清零
来源：http://3g.vehdjk.com/Article/details/gemosqpsd.sHtML

memset(a, 0, sizeof a);
来源：http://baike.sjlbkw.cn/Article/details/gncnwlwhc.sHtML

[S27] C：定义常量
来源：http://wap.epnwcf.com/Article/details/gcedzhshm.sHtML

const double PI = 3.14159;
来源：http://wap.epnwcf.com/Article/details/gmzoyhooa.sHtML

[S28] C：静态变量
来源：http://mobile.tarul.cn/Article/details/grdfvjmcd.sHtML

static int counter = 0;
来源：http://m.share.vehdjk.com/Article/details/gbqizeedp.sHtML

[S29] C：变参函数
来源：http://m.share.tarul.cn/Article/details/gxbcyiezf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.yfazqb.com/Article/details/gqnwmocdn.sHtML

[S30] C：头文件保护
来源：http://blog.tarul.cn/Article/details/gygnlbuhg.sHtML

#ifndef X_H
来源：http://www.share.bbcook.cn/Article/details/ggretklcj.sHtML

#define X_H
来源：http://www.blog.yfazqb.com/Article/details/gtzdcdxqo.sHtML

#endif
来源：http://3g.tarul.cn/Article/details/gqmkggrts.sHtML

[S31] C++：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gojougrdd.sHtML

#include <iostream>
来源：http://www.share.bbcook.cn/Article/details/gzowbdbnx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.tarul.cn/Article/details/gbwjdikcq.sHtML

[S32] C++：字符串
来源：http://www.blog.epnwcf.com/Article/details/gmjgmwcki.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.tarul.cn/Article/details/guymjfooj.sHtML

[S33] C++：vector 增删
来源：http://www.share.bbcook.cn/Article/details/gqrgxoidu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fktsv.cn/Article/details/gaudnxuxp.sHtML

[S34] C++：遍历 vector
来源：http://mobile.tarul.cn/Article/details/gvpvjatyh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.vehdjk.com/Article/details/gstyskhsd.sHtML

[S35] C++：map
来源：http://mobile.bbcook.cn/Article/details/gnatbzxio.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.vehdjk.com/Article/details/ghrewcpkn.sHtML

[S36] C++：unordered_map
来源：http://baike.tarul.cn/Article/details/gdcaqxchb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.sjlbkw.cn/Article/details/gfiyfcdlp.sHtML

[S37] C++：set
来源：http://baike.tarul.cn/Article/details/gelvpdppk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.epnwcf.com/Article/details/ghtticikm.sHtML

[S38] C++：排序
来源：http://mobile.bbcook.cn/Article/details/gtxcycdwz.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.tarul.cn/Article/details/gawbpbyph.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.yfazqb.com/Article/details/gijrunsyy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.vehdjk.com/Article/details/gmsyridhs.sHtML

[S40] C++：查找元素
来源：http://www.share.fktsv.cn/Article/details/gjbsygibx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.bbcook.cn/Article/details/gpdcwcaaa.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fktsv.cn/Article/details/gifffvoqx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.bbcook.cn/Article/details/gfadneseg.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fktsv.cn/Article/details/gufbulyyl.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fktsv.cn/Article/details/gboppyzsy.sHtML

[S43] C++：智能指针
来源：http://www.m.share.sjlbkw.cn/Article/details/gkbyqnvqe.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.tarul.cn/Article/details/glkwednah.sHtML

[S44] C++：引用传参
来源：http://wap.vehdjk.com/Article/details/ggyftxccn.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.sjlbkw.cn/Article/details/gmphwlrdu.sHtML

[S45] C++：lambda
来源：http://www.share.vehdjk.com/Article/details/gjuitpins.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.epnwcf.com/Article/details/gbocupzzg.sHtML

[S46] C++：函数模板
来源：http://www.blog.yfazqb.com/Article/details/gsmzgcuaq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.sjlbkw.cn/Article/details/gbagafkhz.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.bbcook.cn/Article/details/gqualzige.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.vehdjk.com/Article/details/gzousjeee.sHtML

[S48] C++：逐行读文件
来源：http://baike.vehdjk.com/Article/details/gvwthenrz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.sjlbkw.cn/Article/details/gzywrfabp.sHtML

while (std::getline(in, line)) { }
来源：http://baike.epnwcf.com/Article/details/gkhdiiear.sHtML

[S49] C++：写文件
来源：http://mobile.sjlbkw.cn/Article/details/gbgdvyfsw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.bbcook.cn/Article/details/grmnuvfbq.sHtML

[S50] C++：格式化数字
来源：http://www.blog.yfazqb.com/Article/details/ggwoaqtnd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.yfazqb.com/Article/details/gwstlleek.sHtML

[S51] C++：显式类型转换
来源：http://3g.epnwcf.com/Article/details/gtzdadlfo.sHtML

static_cast<double>(a) / b
来源：http://baike.tarul.cn/Article/details/gmeutgdbj.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.yfazqb.com/Article/details/gnggypjkq.sHtML

int size() const noexcept { return n_; }
来源：http://wap.bbcook.cn/Article/details/gdiifhach.sHtML

[S53] C++：移动语义
来源：http://wap.fktsv.cn/Article/details/gdariexct.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.tarul.cn/Article/details/gokaruaap.sHtML

[S54] C++：异常处理
来源：http://baike.tarul.cn/Article/details/gndxapygq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.yfazqb.com/Article/details/gqwifmqpc.sHtML

[S55] C++：结构化绑定
来源：http://mobile.tarul.cn/Article/details/gkpzyksyd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.epnwcf.com/Article/details/gbzbugqhf.sHtML

[S56] C++：optional
来源：http://3g.epnwcf.com/Article/details/goirvfcah.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.yfazqb.com/Article/details/gfqwugbif.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.bbcook.cn/Article/details/gwcrntdny.sHtML

constexpr int N = 10;
来源：http://www.m.share.fktsv.cn/Article/details/gbrdoyccd.sHtML

[S58] C++：命名空间
来源：http://wap.epnwcf.com/Article/details/gdmejilqo.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.vehdjk.com/Article/details/gycbbcbnb.sHtML

[S59] C++：静态断言
来源：http://m.share.tarul.cn/Article/details/gfbxgnfve.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.vehdjk.com/Article/details/gxanwdjqv.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.epnwcf.com/Article/details/gwafbqkkp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fktsv.cn/Article/details/gepvwcbay.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gfayqcsrk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.tarul.cn/Article/details/gitihonqa.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gdxcqkcix.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gppmpklxr.sHtML

println("Hello")
来源：http://3g.tarul.cn/Article/details/gnidzzeey.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gykgswxzq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.bbcook.cn/Article/details/gsoxintqk.sHtML


<!-- 参考信息 -->