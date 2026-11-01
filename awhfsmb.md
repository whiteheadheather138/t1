代发 wailian999

set -euo pipefail
来源：http://baike.fktsv.cn/Article/details/gesifmbeg.sHtML

[R02] 变量赋值与使用
来源：http://read.share.sjlbkw.cn/Article/details/ggwrycqli.sHtML

name="Tom"; echo "$name"
来源：http://mobile.epnwcf.com/Article/details/gquxtjsvi.sHtML

[R03] 只读变量
来源：http://www.m.share.bbcook.cn/Article/details/gjlhekdkr.sHtML

readonly PI=3.14
来源：http://www.m.share.sjlbkw.cn/Article/details/gdazqnzlf.sHtML

[R04] 位置参数
来源：http://blog.tarul.cn/Article/details/ghbtlsmho.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.bbcook.cn/Article/details/gykvuoyss.sHtML

[R05] 参数默认值
来源：http://www.share.fktsv.cn/Article/details/godtblepq.sHtML

name="${1:-default}"
来源：http://mobile.tarul.cn/Article/details/gkvexklup.sHtML

[R06] 判断命令是否存在
来源：http://wap.yfazqb.com/Article/details/glcfxiame.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.yfazqb.com/Article/details/gbhdbtbxt.sHtML

[R07] if 判断文件
来源：http://www.blog.sjlbkw.cn/Article/details/gimdvxwuf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.sjlbkw.cn/Article/details/gzbjkjvnv.sHtML

[R08] 数值比较
来源：http://wap.epnwcf.com/Article/details/ghfkyzpac.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.yfazqb.com/Article/details/glpngbcfl.sHtML

[R09] 字符串比较
来源：http://www.share.epnwcf.com/Article/details/gbcwuemig.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fktsv.cn/Article/details/ghmzcizkz.sHtML

[R10] 正则匹配
来源：http://www.blog.bbcook.cn/Article/details/gdjphotnf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.epnwcf.com/Article/details/gfyievjot.sHtML

[R11] case 多分支
来源：http://3g.yfazqb.com/Article/details/gtprkkzfo.sHtML

case "$1" in
来源：http://mobile.sjlbkw.cn/Article/details/gurhbifre.sHtML

start) echo "启动" ;;
来源：http://www.blog.tarul.cn/Article/details/gslksysqh.sHtML

stop)  echo "停止" ;;
来源：http://blog.tarul.cn/Article/details/gncrwknqo.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.bbcook.cn/Article/details/gctkmsnkr.sHtML

esac
来源：http://www.share.bbcook.cn/Article/details/ghuxibiiz.sHtML

[R12] for 遍历文件
来源：http://mobile.yfazqb.com/Article/details/gopcjfnpq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.bbcook.cn/Article/details/gckplsegq.sHtML

[R13] for 计数循环
来源：http://blog.fktsv.cn/Article/details/gnmzujxld.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fktsv.cn/Article/details/gnpyefalk.sHtML

[R14] C 风格 for
来源：http://wap.bbcook.cn/Article/details/gxxidbcnh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.vehdjk.com/Article/details/gfpfqwsqa.sHtML

[R15] while 逐行读文件
来源：http://wap.epnwcf.com/Article/details/gjqzylxdd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.sjlbkw.cn/Article/details/gospeyuga.sHtML

[R16] until 等待条件
来源：http://blog.yfazqb.com/Article/details/gjgnhihig.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.yfazqb.com/Article/details/gadlqwvtd.sHtML

[R17] 数组定义与取值
来源：http://blog.epnwcf.com/Article/details/gjomruzky.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.bbcook.cn/Article/details/gyoyvuutm.sHtML

[R18] 遍历数组
来源：http://read.share.yfazqb.com/Article/details/ghwugqyxv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.sjlbkw.cn/Article/details/gcfuqpvzj.sHtML

[R19] 数组长度
来源：http://m.share.sjlbkw.cn/Article/details/gdxfqzggc.sHtML

echo "${#arr[@]}"
来源：http://3g.yfazqb.com/Article/details/ghmblgtcf.sHtML

[R20] 关联数组（字典）
来源：http://read.share.vehdjk.com/Article/details/geyugkulr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fktsv.cn/Article/details/gjlbgnbol.sHtML

[R21] 字符串长度
来源：http://read.share.sjlbkw.cn/Article/details/griixnhmq.sHtML

echo "${#s}"
来源：http://m.share.epnwcf.com/Article/details/gsmyosuzz.sHtML

[R22] 截取子串
来源：http://blog.tarul.cn/Article/details/goamriucq.sHtML

echo "${s:0:5}"
来源：http://www.share.vehdjk.com/Article/details/gyakansvf.sHtML

[R23] 字符串替换
来源：http://read.share.tarul.cn/Article/details/goxudatwo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.bbcook.cn/Article/details/goecaxtqz.sHtML

[R24] 大小写转换
来源：http://read.share.fktsv.cn/Article/details/gzflpsfik.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.vehdjk.com/Article/details/gwlghxoyf.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.vehdjk.com/Article/details/gcqqdrwjb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fktsv.cn/Article/details/gqxueubvh.sHtML

[R26] 命令替换
来源：http://read.share.fktsv.cn/Article/details/gcrbefohw.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.yfazqb.com/Article/details/gldrrbhtc.sHtML

[R27] 算术展开
来源：http://www.blog.bbcook.cn/Article/details/gstssikrs.sHtML

echo $((1 + 2 * 3))
来源：http://wap.sjlbkw.cn/Article/details/gvrgtayjx.sHtML

[R28] 浮点运算
来源：http://blog.yfazqb.com/Article/details/ggzmwqhfo.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.sjlbkw.cn/Article/details/gaaimlcsn.sHtML

[R29] 定义函数
来源：http://mobile.epnwcf.com/Article/details/gchojhley.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.vehdjk.com/Article/details/giefjvswc.sHtML

[R30] 函数返回状态码
来源：http://blog.epnwcf.com/Article/details/gksmvxxtw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.tarul.cn/Article/details/gqmwmkfvu.sHtML

[R31] 局部变量
来源：http://read.share.tarul.cn/Article/details/gidecjdkc.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.tarul.cn/Article/details/gdpfbrpoh.sHtML

[R32] 参数个数校验
来源：http://blog.tarul.cn/Article/details/guiqcjnra.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.bbcook.cn/Article/details/grafxqqmz.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.tarul.cn/Article/details/gxywrkscd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.vehdjk.com/Article/details/gsxgbpijd.sHtML

[R34] 退出时清理
来源：http://www.blog.epnwcf.com/Article/details/gjwpdxvee.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.yfazqb.com/Article/details/gjiqiprcp.sHtML

[R35] 后台执行并等待
来源：http://3g.vehdjk.com/Article/details/gafvgvryt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.sjlbkw.cn/Article/details/gwgyswujr.sHtML

[R36] 并发执行多个任务
来源：http://wap.bbcook.cn/Article/details/gmeeemljv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.epnwcf.com/Article/details/goirscezm.sHtML

[R37] 把输出赋给变量
来源：http://blog.sjlbkw.cn/Article/details/gmpwzkngy.sHtML

files=$(ls -1)
来源：http://www.blog.tarul.cn/Article/details/gxotvdpnw.sHtML

[R38] 管道串联
来源：http://wap.fktsv.cn/Article/details/gucglbfnv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.epnwcf.com/Article/details/gkduvslxr.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fktsv.cn/Article/details/gtozxzblk.sHtML

cmd > out.log 2>&1
来源：http://wap.vehdjk.com/Article/details/grgsghuhi.sHtML

[R40] 追加写日志
来源：http://mobile.bbcook.cn/Article/details/ghzjimdfh.sHtML

echo "log" >> out.log
来源：http://mobile.epnwcf.com/Article/details/gimnpognn.sHtML

[R41] 丢弃输出
来源：http://www.share.yfazqb.com/Article/details/gkxxshhyd.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fktsv.cn/Article/details/gneucblnw.sHtML

[R42] 输入重定向
来源：http://blog.sjlbkw.cn/Article/details/gfbjgaazo.sHtML

wc -l < a.txt
来源：http://baike.yfazqb.com/Article/details/gtnkvbevh.sHtML

[R43] 按名字查找文件
来源：http://3g.sjlbkw.cn/Article/details/ggguwojrl.sHtML

find . -name "*.log" -type f
来源：http://baike.fktsv.cn/Article/details/gdwppxdcv.sHtML

[R44] 按修改时间查找
来源：http://baike.sjlbkw.cn/Article/details/gpwsrtdss.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.yfazqb.com/Article/details/gdjaldgka.sHtML

[R45] 批量删除
来源：http://3g.vehdjk.com/Article/details/gdhrmvihf.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fktsv.cn/Article/details/gqhcvvhzd.sHtML

[R46] 递归替换文件内容
来源：http://blog.bbcook.cn/Article/details/gkqswgyts.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.vehdjk.com/Article/details/gmmfvrpbp.sHtML

[R47] sed 单行替换
来源：http://mobile.bbcook.cn/Article/details/gpwmrfpsj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fktsv.cn/Article/details/glmwmrucx.sHtML

[R48] awk 取指定列
来源：http://www.share.vehdjk.com/Article/details/gbsjkhhrl.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.epnwcf.com/Article/details/gqnwiiqlh.sHtML

[R49] awk 带条件
来源：http://blog.sjlbkw.cn/Article/details/ghtpwktqk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fktsv.cn/Article/details/gtkohoxii.sHtML

[R50] awk 求和
来源：http://wap.vehdjk.com/Article/details/gizkyqyem.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.sjlbkw.cn/Article/details/gvoaonwti.sHtML

[R51] 排序去重取前几
来源：http://m.share.sjlbkw.cn/Article/details/gljizxssh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fktsv.cn/Article/details/ghntckfvf.sHtML

[R52] 统计行数
来源：http://mobile.vehdjk.com/Article/details/gjfhrdbbc.sHtML

wc -l a.txt
来源：http://3g.sjlbkw.cn/Article/details/gisntwdes.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.sjlbkw.cn/Article/details/gbfalhxcn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.yfazqb.com/Article/details/gaknidvhr.sHtML

[R54] 比较两个文件
来源：http://m.share.yfazqb.com/Article/details/guseyngze.sHtML

diff a.txt b.txt
来源：http://m.share.fktsv.cn/Article/details/gaqdmljmx.sHtML

[R55] 压缩与解压
来源：http://baike.tarul.cn/Article/details/goqlcxbbq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.vehdjk.com/Article/details/gmjytdadv.sHtML

[R56] 远程拷贝
来源：http://m.share.epnwcf.com/Article/details/ghjcturlj.sHtML

scp file user@host:/path/
来源：http://mobile.bbcook.cn/Article/details/gpvpqpayu.sHtML

[R57] 远程执行命令
来源：http://m.share.tarul.cn/Article/details/gqjdikekk.sHtML

ssh user@host 'uptime'
来源：http://wap.bbcook.cn/Article/details/gftcuyovy.sHtML

[R58] 下载文件
来源：http://mobile.tarul.cn/Article/details/gpnrcmath.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.sjlbkw.cn/Article/details/gnwbkkswm.sHtML

[R59] 发 POST JSON
来源：http://m.share.bbcook.cn/Article/details/gukxncncl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fktsv.cn/Article/details/ghygsxkvt.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.yfazqb.com/Article/details/ggeqcczrf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.sjlbkw.cn/Article/details/gxfpjtmyg.sHtML

[R61] 磁盘占用
来源：http://baike.fktsv.cn/Article/details/gdexdkbeo.sHtML

df -h;  du -sh *
来源：http://www.blog.epnwcf.com/Article/details/gunfjqyeb.sHtML

[R62] 找最占空间的文件
来源：http://wap.epnwcf.com/Article/details/gpyzxvmsm.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.yfazqb.com/Article/details/gppjyvwmx.sHtML

[R63] 内存与进程
来源：http://wap.tarul.cn/Article/details/gzbdcxgmc.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.yfazqb.com/Article/details/gszepqfwk.sHtML

[R64] 结束进程
来源：http://www.m.share.vehdjk.com/Article/details/gqzreotsk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.epnwcf.com/Article/details/gtdbrjhgz.sHtML

[R65] 查看端口占用
来源：http://blog.yfazqb.com/Article/details/goiuupyyn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.vehdjk.com/Article/details/gobjwdhck.sHtML

[R66] 定时任务
来源：http://www.blog.epnwcf.com/Article/details/grujjjtdk.sHtML

crontab -e;  crontab -l
来源：http://www.share.bbcook.cn/Article/details/gxcuzttkc.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.yfazqb.com/Article/details/guebgftpd.sHtML

openssl rand -hex 16
来源：http://3g.fktsv.cn/Article/details/gulsbvzln.sHtML

[R68] 计算文件校验值
来源：http://www.share.yfazqb.com/Article/details/gcumgsefp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.yfazqb.com/Article/details/gyctgqzyi.sHtML

[R69] 生成随机密码
来源：http://baike.vehdjk.com/Article/details/gwalbxlbz.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.epnwcf.com/Article/details/gskeeugaj.sHtML

[R70] 时间戳与互转
来源：http://baike.fktsv.cn/Article/details/gcqebwdgi.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.vehdjk.com/Article/details/glvnvowpe.sHtML

[R71] 日期格式化
来源：http://mobile.epnwcf.com/Article/details/glbtgbcve.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fktsv.cn/Article/details/ggodoagay.sHtML

[R72] 等待端口就绪
来源：http://3g.fktsv.cn/Article/details/glwruueza.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fktsv.cn/Article/details/gofvumblr.sHtML

[R73] 分割大日志
来源：http://3g.vehdjk.com/Article/details/gtzfsuvhb.sHtML

split -l 1000 big.log part_
来源：http://read.share.vehdjk.com/Article/details/gjarutrkp.sHtML

[R74] 批量重命名
来源：http://m.share.yfazqb.com/Article/details/gpzxpkcfc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.tarul.cn/Article/details/gflxfthwd.sHtML

[R75] 导出环境变量
来源：http://www.blog.tarul.cn/Article/details/gbgiuqznr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.sjlbkw.cn/Article/details/gnnntficg.sHtML

[R76] 使用临时文件
来源：http://mobile.bbcook.cn/Article/details/gtkkwumjp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.sjlbkw.cn/Article/details/glkdzitmo.sHtML

[R77] 读取用户输入
来源：http://m.share.bbcook.cn/Article/details/gqywqkvhd.sHtML

read -rp "请输入: " ans
来源：http://read.share.yfazqb.com/Article/details/goiqgmdis.sHtML

[R78] 交互式菜单
来源：http://read.share.tarul.cn/Article/details/gjolkjulh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.vehdjk.com/Article/details/gohfyzkpn.sHtML

[R79] 解析命令行选项
来源：http://3g.yfazqb.com/Article/details/gdxgpqavg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.vehdjk.com/Article/details/grofpycxx.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.tarul.cn/Article/details/gnalukhqm.sHtML

time ./run.sh
来源：http://mobile.tarul.cn/Article/details/gdvpoplyf.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gjupicwju.sHtML

S. C / C++ 专题
来源：http://m.share.bbcook.cn/Article/details/gsfwqdxsb.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gcfsgaenp.sHtML

[S01] C：Hello World
来源：http://www.share.epnwcf.com/Article/details/gpyzdnmxt.sHtML

#include <stdio.h>
来源：http://www.share.tarul.cn/Article/details/ggbfxpfrn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fktsv.cn/Article/details/ggcmdhjvo.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.sjlbkw.cn/Article/details/ghkunkfnz.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.vehdjk.com/Article/details/ghoauydgh.sHtML

[S03] C：读入整数
来源：http://read.share.fktsv.cn/Article/details/gkgunlcyu.sHtML

int x; scanf("%d", &x);
来源：http://www.share.vehdjk.com/Article/details/gfmlgyswu.sHtML

[S04] C：字符串复制
来源：http://mobile.sjlbkw.cn/Article/details/gaxbqrqpu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.tarul.cn/Article/details/gtesloocw.sHtML

[S05] C：字符串长度
来源：http://blog.bbcook.cn/Article/details/gcpssdpei.sHtML

strlen(s)
来源：http://www.share.tarul.cn/Article/details/gbrerseqs.sHtML

[S06] C：字符串比较
来源：http://wap.yfazqb.com/Article/details/gssnrzxax.sHtML

strcmp(a, b) == 0
来源：http://www.blog.vehdjk.com/Article/details/gbnzincsh.sHtML

[S07] C：数组遍历求和
来源：http://www.share.vehdjk.com/Article/details/gziqlgjjh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.vehdjk.com/Article/details/goriiqzsl.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.epnwcf.com/Article/details/gdlamjjsn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.vehdjk.com/Article/details/gazcgpvjb.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.epnwcf.com/Article/details/gzllbbfgw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.bbcook.cn/Article/details/gcbvyzeqt.sHtML

[S10] C：指针与解引用
来源：http://blog.tarul.cn/Article/details/gatemgtza.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.vehdjk.com/Article/details/gbgwgueom.sHtML

[S11] C：逐行读文件
来源：http://m.share.tarul.cn/Article/details/gbdplkhyu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.tarul.cn/Article/details/gzuxzzucj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.bbcook.cn/Article/details/gapmrixav.sHtML

fclose(f);
来源：http://www.m.share.tarul.cn/Article/details/gobrltrfh.sHtML

[S12] C：写文件
来源：http://www.share.fktsv.cn/Article/details/ghlteuxwf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.yfazqb.com/Article/details/gmhjrqtir.sHtML

[S13] C：宏定义
来源：http://www.m.share.fktsv.cn/Article/details/gqvliegbj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.epnwcf.com/Article/details/gvtgjcfrm.sHtML

[S14] C：枚举
来源：http://wap.vehdjk.com/Article/details/gbwgowvmb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.epnwcf.com/Article/details/gqpeuwsgb.sHtML

[S15] C：类型转换
来源：http://3g.tarul.cn/Article/details/gvrdpwgki.sHtML

(double) a / b
来源：http://3g.yfazqb.com/Article/details/gzijsospk.sHtML

[S16] C：位操作置位
来源：http://www.m.share.sjlbkw.cn/Article/details/gwindoenf.sHtML

x |= (1 << 3);
来源：http://3g.sjlbkw.cn/Article/details/gszlaxepa.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.sjlbkw.cn/Article/details/gwpaccvkk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.bbcook.cn/Article/details/gemzfebpg.sHtML

[S18] C：命令行参数
来源：http://www.share.fktsv.cn/Article/details/gyfigpluj.sHtML

int main(int argc, char **argv)
来源：http://wap.fktsv.cn/Article/details/ghosghrat.sHtML

[S19] C：快速排序
来源：http://read.share.sjlbkw.cn/Article/details/gqwradkhj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.yfazqb.com/Article/details/gzpcztpbe.sHtML

[S20] C：二分查找
来源：http://wap.epnwcf.com/Article/details/gwxsxzrjk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.epnwcf.com/Article/details/gttemtfyh.sHtML

[S21] C：字符类别判断
来源：http://read.share.epnwcf.com/Article/details/goefrtbxo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.vehdjk.com/Article/details/gcjgualjw.sHtML

[S22] C：字符串转数字
来源：http://3g.vehdjk.com/Article/details/gjdupmrwr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.vehdjk.com/Article/details/gypqixnyb.sHtML

[S23] C：随机数
来源：http://mobile.epnwcf.com/Article/details/gdsboxeze.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.bbcook.cn/Article/details/gauatszse.sHtML

[S24] C：获取本地时间
来源：http://m.share.vehdjk.com/Article/details/gcyggklct.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.epnwcf.com/Article/details/gbqmypxlz.sHtML

[S25] C：内存拷贝
来源：http://www.blog.yfazqb.com/Article/details/glvfifazl.sHtML

memcpy(dst, src, n);
来源：http://www.blog.yfazqb.com/Article/details/gpmfqnekx.sHtML

[S26] C：内存清零
来源：http://www.share.yfazqb.com/Article/details/gyowyeiaa.sHtML

memset(a, 0, sizeof a);
来源：http://baike.yfazqb.com/Article/details/givdkvyzz.sHtML

[S27] C：定义常量
来源：http://mobile.bbcook.cn/Article/details/gdtobinlt.sHtML

const double PI = 3.14159;
来源：http://m.share.bbcook.cn/Article/details/gwclldskq.sHtML

[S28] C：静态变量
来源：http://mobile.bbcook.cn/Article/details/guwkgtudz.sHtML

static int counter = 0;
来源：http://wap.epnwcf.com/Article/details/greqqzwhk.sHtML

[S29] C：变参函数
来源：http://wap.tarul.cn/Article/details/gjhhrtajg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.yfazqb.com/Article/details/gdairnihl.sHtML

[S30] C：头文件保护
来源：http://www.m.share.tarul.cn/Article/details/gviyvngsb.sHtML

#ifndef X_H
来源：http://m.share.bbcook.cn/Article/details/grmsjxiqu.sHtML

#define X_H
来源：http://blog.bbcook.cn/Article/details/gzpxqonty.sHtML

#endif
来源：http://www.m.share.sjlbkw.cn/Article/details/ghutfdngv.sHtML

[S31] C++：Hello World
来源：http://mobile.vehdjk.com/Article/details/ggugsijpq.sHtML

#include <iostream>
来源：http://mobile.yfazqb.com/Article/details/gbvidyypv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.epnwcf.com/Article/details/grdbqzect.sHtML

[S32] C++：字符串
来源：http://wap.fktsv.cn/Article/details/gwwcswqtm.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.bbcook.cn/Article/details/gxonkpbqx.sHtML

[S33] C++：vector 增删
来源：http://www.blog.yfazqb.com/Article/details/gvzjuzguf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.bbcook.cn/Article/details/gevfisymu.sHtML

[S34] C++：遍历 vector
来源：http://mobile.epnwcf.com/Article/details/glqrfcuqx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fktsv.cn/Article/details/gwswscjqp.sHtML

[S35] C++：map
来源：http://blog.epnwcf.com/Article/details/gpmkbhaul.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.tarul.cn/Article/details/gucrdtrlt.sHtML

[S36] C++：unordered_map
来源：http://m.share.bbcook.cn/Article/details/gsuufyeoy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.bbcook.cn/Article/details/gdkwmfxat.sHtML

[S37] C++：set
来源：http://baike.vehdjk.com/Article/details/gsfwnvxan.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvetfchdw.sHtML

[S38] C++：排序
来源：http://www.m.share.vehdjk.com/Article/details/gqfslohsz.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.sjlbkw.cn/Article/details/gluqwxslu.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fktsv.cn/Article/details/guzgbozmh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.vehdjk.com/Article/details/gljeffotn.sHtML

[S40] C++：查找元素
来源：http://www.m.share.sjlbkw.cn/Article/details/gnlcinahp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fktsv.cn/Article/details/gcfcphian.sHtML

[S41] C++：类与构造函数
来源：http://blog.yfazqb.com/Article/details/gzqpozamn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.bbcook.cn/Article/details/govbbauui.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fktsv.cn/Article/details/gjwpysmgc.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.sjlbkw.cn/Article/details/gjkrdnoub.sHtML

[S43] C++：智能指针
来源：http://3g.epnwcf.com/Article/details/gdjuqwaza.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.tarul.cn/Article/details/gpiiywzud.sHtML

[S44] C++：引用传参
来源：http://wap.bbcook.cn/Article/details/gmrlknleq.sHtML

void inc(int &x) { ++x; }
来源：http://wap.vehdjk.com/Article/details/gpassqpro.sHtML

[S45] C++：lambda
来源：http://www.m.share.fktsv.cn/Article/details/guhfawmnk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.epnwcf.com/Article/details/gaoeypzsi.sHtML

[S46] C++：函数模板
来源：http://mobile.bbcook.cn/Article/details/gxoqwwaso.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.yfazqb.com/Article/details/gguhevcct.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.epnwcf.com/Article/details/gfljaibia.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.vehdjk.com/Article/details/gisxrsvlb.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fktsv.cn/Article/details/gntbeerlt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.tarul.cn/Article/details/ggzfrblyq.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.epnwcf.com/Article/details/geshsxine.sHtML

[S49] C++：写文件
来源：http://baike.yfazqb.com/Article/details/gltfkugka.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.vehdjk.com/Article/details/ggettxepk.sHtML

[S50] C++：格式化数字
来源：http://m.share.tarul.cn/Article/details/gxxlcjfix.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.tarul.cn/Article/details/gubmftzkl.sHtML

[S51] C++：显式类型转换
来源：http://3g.fktsv.cn/Article/details/glstyzgyn.sHtML

static_cast<double>(a) / b
来源：http://www.blog.tarul.cn/Article/details/gmfsqolkc.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.sjlbkw.cn/Article/details/gtyjurtyb.sHtML

int size() const noexcept { return n_; }
来源：http://baike.yfazqb.com/Article/details/gwlreyfxu.sHtML

[S53] C++：移动语义
来源：http://wap.epnwcf.com/Article/details/gntdqhmin.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.sjlbkw.cn/Article/details/gddedaygz.sHtML

[S54] C++：异常处理
来源：http://blog.fktsv.cn/Article/details/gykvopare.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.epnwcf.com/Article/details/gbpqbilph.sHtML

[S55] C++：结构化绑定
来源：http://wap.vehdjk.com/Article/details/ggwrbfpzr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.yfazqb.com/Article/details/gjzswjjzq.sHtML

[S56] C++：optional
来源：http://3g.fktsv.cn/Article/details/gpifkdgye.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.sjlbkw.cn/Article/details/gpiiyivfz.sHtML

[S57] C++：编译期常量
来源：http://www.share.tarul.cn/Article/details/gxpumokzl.sHtML

constexpr int N = 10;
来源：http://wap.sjlbkw.cn/Article/details/gqrrkbikc.sHtML

[S58] C++：命名空间
来源：http://blog.yfazqb.com/Article/details/gqlbqeauo.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.sjlbkw.cn/Article/details/gvilhllht.sHtML

[S59] C++：静态断言
来源：http://mobile.fktsv.cn/Article/details/gyzxqvtol.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.tarul.cn/Article/details/gucrtctjx.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fktsv.cn/Article/details/gcbjtlzar.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.yfazqb.com/Article/details/gbktpezoz.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gizwtymdz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.yfazqb.com/Article/details/gguvlqsmv.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gshdtwyje.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.tarul.cn/Article/details/ghwrbjgxa.sHtML

println("Hello")
来源：http://www.share.yfazqb.com/Article/details/gqggwrprk.sHtML

[T02] Kotlin：变量
来源：http://blog.yfazqb.com/Article/details/gegaiqlst.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fktsv.cn/Article/details/gcppgdihs.sHtML


<!-- 参考信息 -->