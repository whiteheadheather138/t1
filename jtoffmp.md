代发 wailian999

readonly PI=3.14
来源：http://baike.fktsv.cn/Article/details/geybaqaup.sHtML

[R04] 位置参数
来源：http://m.share.sjlbkw.cn/Article/details/gwpvuhvrf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fktsv.cn/Article/details/gfaueyyem.sHtML

[R05] 参数默认值
来源：http://www.m.share.sjlbkw.cn/Article/details/gsfrvrozn.sHtML

name="${1:-default}"
来源：http://wap.sjlbkw.cn/Article/details/gkyeahhez.sHtML

[R06] 判断命令是否存在
来源：http://mobile.tarul.cn/Article/details/gvsqpyrum.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.epnwcf.com/Article/details/gbfhkerqy.sHtML

[R07] if 判断文件
来源：http://blog.bbcook.cn/Article/details/gjqscuwxy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.epnwcf.com/Article/details/govrifdcj.sHtML

[R08] 数值比较
来源：http://wap.fktsv.cn/Article/details/gtvuyazyu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fktsv.cn/Article/details/gsnqeaurv.sHtML

[R09] 字符串比较
来源：http://3g.tarul.cn/Article/details/gnnsiveok.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fktsv.cn/Article/details/gulyorhzm.sHtML

[R10] 正则匹配
来源：http://baike.bbcook.cn/Article/details/gnbbgzyvp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.tarul.cn/Article/details/gbydcmfsl.sHtML

[R11] case 多分支
来源：http://3g.sjlbkw.cn/Article/details/gfzincomr.sHtML

case "$1" in
来源：http://read.share.sjlbkw.cn/Article/details/ggqlkzalj.sHtML

start) echo "启动" ;;
来源：http://blog.fktsv.cn/Article/details/gxtcgrvix.sHtML

stop)  echo "停止" ;;
来源：http://www.share.vehdjk.com/Article/details/gtpiswecr.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.bbcook.cn/Article/details/gujucwzmf.sHtML

esac
来源：http://m.share.epnwcf.com/Article/details/gtyditquc.sHtML

[R12] for 遍历文件
来源：http://blog.epnwcf.com/Article/details/gfjwaaiem.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.yfazqb.com/Article/details/gudsizuga.sHtML

[R13] for 计数循环
来源：http://3g.yfazqb.com/Article/details/gxvdedvwe.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fktsv.cn/Article/details/gssktzeex.sHtML

[R14] C 风格 for
来源：http://read.share.fktsv.cn/Article/details/gtklzsvrt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fktsv.cn/Article/details/ghijhpkai.sHtML

[R15] while 逐行读文件
来源：http://www.share.bbcook.cn/Article/details/gkvdnnzwh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.epnwcf.com/Article/details/gfgehrmjr.sHtML

[R16] until 等待条件
来源：http://www.blog.yfazqb.com/Article/details/gbblsclxq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.bbcook.cn/Article/details/gfdrxwgap.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.yfazqb.com/Article/details/gdhxvoyjz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.tarul.cn/Article/details/gwtlsihcd.sHtML

[R18] 遍历数组
来源：http://www.m.share.bbcook.cn/Article/details/garijzibg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.vehdjk.com/Article/details/gavffzxnb.sHtML

[R19] 数组长度
来源：http://m.share.tarul.cn/Article/details/gdmcofvko.sHtML

echo "${#arr[@]}"
来源：http://m.share.yfazqb.com/Article/details/gyewwtwdf.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.sjlbkw.cn/Article/details/gbxlrbexv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fktsv.cn/Article/details/gjbpgpvuw.sHtML

[R21] 字符串长度
来源：http://www.share.sjlbkw.cn/Article/details/gapvqwtsi.sHtML

echo "${#s}"
来源：http://www.m.share.epnwcf.com/Article/details/gxwlzxmth.sHtML

[R22] 截取子串
来源：http://mobile.fktsv.cn/Article/details/gaqlgjtlw.sHtML

echo "${s:0:5}"
来源：http://baike.yfazqb.com/Article/details/gnepeybpx.sHtML

[R23] 字符串替换
来源：http://www.blog.bbcook.cn/Article/details/ghqxxmmpu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.yfazqb.com/Article/details/gfhekmgxm.sHtML

[R24] 大小写转换
来源：http://mobile.yfazqb.com/Article/details/ggpsvvrbk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.epnwcf.com/Article/details/gzmlljtre.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.sjlbkw.cn/Article/details/gajxslwja.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.vehdjk.com/Article/details/gwpusomoq.sHtML

[R26] 命令替换
来源：http://read.share.fktsv.cn/Article/details/gmbkebwvt.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.epnwcf.com/Article/details/ggfenmmcf.sHtML

[R27] 算术展开
来源：http://read.share.vehdjk.com/Article/details/glmkxpznv.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.vehdjk.com/Article/details/gjogemadr.sHtML

[R28] 浮点运算
来源：http://3g.yfazqb.com/Article/details/glauezgqh.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.sjlbkw.cn/Article/details/gfuhrwljm.sHtML

[R29] 定义函数
来源：http://blog.fktsv.cn/Article/details/gmjgfalbz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fktsv.cn/Article/details/gugdfbnkm.sHtML

[R30] 函数返回状态码
来源：http://m.share.fktsv.cn/Article/details/goruksuvp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.tarul.cn/Article/details/gbgvjuhxe.sHtML

[R31] 局部变量
来源：http://wap.fktsv.cn/Article/details/ghhvwsccp.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.epnwcf.com/Article/details/gxspcvnsn.sHtML

[R32] 参数个数校验
来源：http://3g.fktsv.cn/Article/details/gstmattpn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.tarul.cn/Article/details/gwsrlwbpj.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.bbcook.cn/Article/details/ghwmsbxoo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.epnwcf.com/Article/details/gapafnfon.sHtML

[R34] 退出时清理
来源：http://www.blog.bbcook.cn/Article/details/gjlkdudxa.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.epnwcf.com/Article/details/gblawpfhc.sHtML

[R35] 后台执行并等待
来源：http://blog.epnwcf.com/Article/details/gnhpufdof.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.epnwcf.com/Article/details/gvpzhnkuw.sHtML

[R36] 并发执行多个任务
来源：http://www.share.yfazqb.com/Article/details/gffjqqdbh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.epnwcf.com/Article/details/gdmpzvkpd.sHtML

[R37] 把输出赋给变量
来源：http://3g.sjlbkw.cn/Article/details/gwrytmxwj.sHtML

files=$(ls -1)
来源：http://wap.sjlbkw.cn/Article/details/gvreupmfj.sHtML

[R38] 管道串联
来源：http://www.share.epnwcf.com/Article/details/glcklgyiz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.vehdjk.com/Article/details/givpkzstz.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.vehdjk.com/Article/details/gtcpifnlk.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.yfazqb.com/Article/details/gcbgwikpa.sHtML

[R40] 追加写日志
来源：http://www.share.sjlbkw.cn/Article/details/ggmwhvguo.sHtML

echo "log" >> out.log
来源：http://baike.fktsv.cn/Article/details/gxxehcees.sHtML

[R41] 丢弃输出
来源：http://www.share.epnwcf.com/Article/details/gcchypmhl.sHtML

cmd >/dev/null 2>&1
来源：http://wap.epnwcf.com/Article/details/gmvjqmnur.sHtML

[R42] 输入重定向
来源：http://blog.epnwcf.com/Article/details/gnynhjnha.sHtML

wc -l < a.txt
来源：http://www.blog.vehdjk.com/Article/details/gtdavjsrs.sHtML

[R43] 按名字查找文件
来源：http://www.share.bbcook.cn/Article/details/giqysvfwb.sHtML

find . -name "*.log" -type f
来源：http://blog.sjlbkw.cn/Article/details/gzmmyphbj.sHtML

[R44] 按修改时间查找
来源：http://blog.sjlbkw.cn/Article/details/gmibsrhfu.sHtML

find . -mtime -7 -type f
来源：http://m.share.sjlbkw.cn/Article/details/gkqhmszcw.sHtML

[R45] 批量删除
来源：http://m.share.tarul.cn/Article/details/gylnoasmc.sHtML

find . -name "*.tmp" -delete
来源：http://blog.epnwcf.com/Article/details/guazrdzmu.sHtML

[R46] 递归替换文件内容
来源：http://blog.tarul.cn/Article/details/gmbawwnsg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.yfazqb.com/Article/details/gmnwgoddl.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fktsv.cn/Article/details/gglwuhcep.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.sjlbkw.cn/Article/details/gaxeckrbu.sHtML

[R48] awk 取指定列
来源：http://blog.sjlbkw.cn/Article/details/gyhbjgrmr.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.sjlbkw.cn/Article/details/grcxxdyii.sHtML

[R49] awk 带条件
来源：http://m.share.vehdjk.com/Article/details/gkqlolmfe.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.sjlbkw.cn/Article/details/gfgvnwsfu.sHtML

[R50] awk 求和
来源：http://www.m.share.yfazqb.com/Article/details/ggjikoutd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.epnwcf.com/Article/details/gypvwtqpg.sHtML

[R51] 排序去重取前几
来源：http://wap.yfazqb.com/Article/details/guuylpice.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.yfazqb.com/Article/details/ghfyrnzfo.sHtML

[R52] 统计行数
来源：http://www.blog.bbcook.cn/Article/details/gvffhazzg.sHtML

wc -l a.txt
来源：http://3g.tarul.cn/Article/details/grxpoogfg.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.vehdjk.com/Article/details/gnetljeoq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.sjlbkw.cn/Article/details/gzsltmsgm.sHtML

[R54] 比较两个文件
来源：http://www.blog.epnwcf.com/Article/details/gaavnvlzd.sHtML

diff a.txt b.txt
来源：http://baike.vehdjk.com/Article/details/gkzdxuyvm.sHtML

[R55] 压缩与解压
来源：http://mobile.vehdjk.com/Article/details/gbyjsbqlc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.sjlbkw.cn/Article/details/gdgcszckv.sHtML

[R56] 远程拷贝
来源：http://3g.bbcook.cn/Article/details/gjquymyzx.sHtML

scp file user@host:/path/
来源：http://blog.bbcook.cn/Article/details/gvsktexqd.sHtML

[R57] 远程执行命令
来源：http://www.m.share.sjlbkw.cn/Article/details/gzanxonfa.sHtML

ssh user@host 'uptime'
来源：http://3g.fktsv.cn/Article/details/geuanfjug.sHtML

[R58] 下载文件
来源：http://www.m.share.fktsv.cn/Article/details/gwwchatsg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fktsv.cn/Article/details/gbcijlgsa.sHtML

[R59] 发 POST JSON
来源：http://www.blog.bbcook.cn/Article/details/grlzaqajz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.yfazqb.com/Article/details/gkpnaqisq.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.vehdjk.com/Article/details/goxsseacu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.yfazqb.com/Article/details/gsyhbqjjk.sHtML

[R61] 磁盘占用
来源：http://www.blog.vehdjk.com/Article/details/gfatitywh.sHtML

df -h;  du -sh *
来源：http://www.share.epnwcf.com/Article/details/gcldnnwxa.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.vehdjk.com/Article/details/gaarhviwt.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.tarul.cn/Article/details/gjmtkxngk.sHtML

[R63] 内存与进程
来源：http://blog.fktsv.cn/Article/details/gnomuffat.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.bbcook.cn/Article/details/gndghafkp.sHtML

[R64] 结束进程
来源：http://m.share.vehdjk.com/Article/details/ghctmlkaj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.sjlbkw.cn/Article/details/giaktifsr.sHtML

[R65] 查看端口占用
来源：http://m.share.sjlbkw.cn/Article/details/gxnrgzqiz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.tarul.cn/Article/details/gqtjmgbxj.sHtML

[R66] 定时任务
来源：http://read.share.fktsv.cn/Article/details/gffccvamt.sHtML

crontab -e;  crontab -l
来源：http://3g.yfazqb.com/Article/details/gpwmtjues.sHtML

[R67] 生成随机十六进制串
来源：http://3g.tarul.cn/Article/details/gioclhran.sHtML

openssl rand -hex 16
来源：http://read.share.epnwcf.com/Article/details/gejuukklw.sHtML

[R68] 计算文件校验值
来源：http://wap.yfazqb.com/Article/details/glbrjokca.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.vehdjk.com/Article/details/gmfcrvgvo.sHtML

[R69] 生成随机密码
来源：http://mobile.epnwcf.com/Article/details/getbsecnl.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.epnwcf.com/Article/details/gwkzynsnf.sHtML

[R70] 时间戳与互转
来源：http://read.share.vehdjk.com/Article/details/gvgehcrka.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fktsv.cn/Article/details/givmomdbv.sHtML

[R71] 日期格式化
来源：http://www.blog.bbcook.cn/Article/details/gltvjsibu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.vehdjk.com/Article/details/gfnbzjbwg.sHtML

[R72] 等待端口就绪
来源：http://m.share.sjlbkw.cn/Article/details/glcldebtm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.bbcook.cn/Article/details/gobuanrgv.sHtML

[R73] 分割大日志
来源：http://www.blog.epnwcf.com/Article/details/gfecyqwhn.sHtML

split -l 1000 big.log part_
来源：http://blog.vehdjk.com/Article/details/gwkjnrjrc.sHtML

[R74] 批量重命名
来源：http://wap.vehdjk.com/Article/details/gaycjqkwr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.vehdjk.com/Article/details/gcmvdjdgz.sHtML

[R75] 导出环境变量
来源：http://wap.tarul.cn/Article/details/gcppqksra.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.bbcook.cn/Article/details/gkgpiqtqj.sHtML

[R76] 使用临时文件
来源：http://mobile.bbcook.cn/Article/details/gjebfwqen.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.vehdjk.com/Article/details/grznmqnxe.sHtML

[R77] 读取用户输入
来源：http://mobile.sjlbkw.cn/Article/details/gznvjyyyc.sHtML

read -rp "请输入: " ans
来源：http://read.share.fktsv.cn/Article/details/gvhrblxdn.sHtML

[R78] 交互式菜单
来源：http://read.share.epnwcf.com/Article/details/gffenjvzt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.yfazqb.com/Article/details/gcchpquou.sHtML

[R79] 解析命令行选项
来源：http://www.blog.yfazqb.com/Article/details/gpwwzbqyj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.vehdjk.com/Article/details/gedgvdktj.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fktsv.cn/Article/details/goeqetqev.sHtML

time ./run.sh
来源：http://read.share.yfazqb.com/Article/details/grtrkpyac.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gunposaqg.sHtML

S. C / C++ 专题
来源：http://www.share.epnwcf.com/Article/details/grsbopclj.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gbfnibpoj.sHtML

[S01] C：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gjzyypixf.sHtML

#include <stdio.h>
来源：http://wap.yfazqb.com/Article/details/gtjttfavr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.vehdjk.com/Article/details/gduncjgyr.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fktsv.cn/Article/details/gexukyawm.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.epnwcf.com/Article/details/gtszvayal.sHtML

[S03] C：读入整数
来源：http://baike.sjlbkw.cn/Article/details/grsrcxbbd.sHtML

int x; scanf("%d", &x);
来源：http://blog.epnwcf.com/Article/details/gddjfpsul.sHtML

[S04] C：字符串复制
来源：http://www.blog.yfazqb.com/Article/details/gzvhiswju.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.yfazqb.com/Article/details/gyhogwkmq.sHtML

[S05] C：字符串长度
来源：http://www.blog.yfazqb.com/Article/details/gexajfmdh.sHtML

strlen(s)
来源：http://baike.sjlbkw.cn/Article/details/gfexublgl.sHtML

[S06] C：字符串比较
来源：http://mobile.vehdjk.com/Article/details/gaixtfpjt.sHtML

strcmp(a, b) == 0
来源：http://wap.tarul.cn/Article/details/glbjkbasy.sHtML

[S07] C：数组遍历求和
来源：http://read.share.bbcook.cn/Article/details/ggjyoemcd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.vehdjk.com/Article/details/gtqlolycu.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.yfazqb.com/Article/details/gluruuubr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.sjlbkw.cn/Article/details/gjlivouxl.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.yfazqb.com/Article/details/gifsokcsx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fktsv.cn/Article/details/gnvtozifr.sHtML

[S10] C：指针与解引用
来源：http://read.share.sjlbkw.cn/Article/details/gquaxrewm.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.bbcook.cn/Article/details/gaescvvyh.sHtML

[S11] C：逐行读文件
来源：http://www.share.fktsv.cn/Article/details/gxtulotth.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.tarul.cn/Article/details/guzflqtin.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.vehdjk.com/Article/details/girpgsyph.sHtML

fclose(f);
来源：http://m.share.vehdjk.com/Article/details/gzmijwxxr.sHtML

[S12] C：写文件
来源：http://read.share.sjlbkw.cn/Article/details/gsnxeswxl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.sjlbkw.cn/Article/details/gaudnwivz.sHtML

[S13] C：宏定义
来源：http://baike.tarul.cn/Article/details/ggzsuycrh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.tarul.cn/Article/details/gtpkeootr.sHtML

[S14] C：枚举
来源：http://www.blog.sjlbkw.cn/Article/details/gonchoriy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fktsv.cn/Article/details/ginuiofqw.sHtML

[S15] C：类型转换
来源：http://mobile.bbcook.cn/Article/details/grzdwscns.sHtML

(double) a / b
来源：http://www.blog.tarul.cn/Article/details/gxitaraej.sHtML

[S16] C：位操作置位
来源：http://www.blog.yfazqb.com/Article/details/gooeobdwq.sHtML

x |= (1 << 3);
来源：http://read.share.sjlbkw.cn/Article/details/grxbwcykh.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.vehdjk.com/Article/details/gwfgrdejr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.tarul.cn/Article/details/gftljmwid.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fktsv.cn/Article/details/guxmlrpge.sHtML

int main(int argc, char **argv)
来源：http://wap.sjlbkw.cn/Article/details/gqxichdtq.sHtML

[S19] C：快速排序
来源：http://www.m.share.epnwcf.com/Article/details/goqzhensy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.yfazqb.com/Article/details/glbraevop.sHtML

[S20] C：二分查找
来源：http://www.share.fktsv.cn/Article/details/gzokhamak.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.epnwcf.com/Article/details/gqhnjewbs.sHtML

[S21] C：字符类别判断
来源：http://www.blog.tarul.cn/Article/details/gbzcpogsr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.bbcook.cn/Article/details/gullkyfko.sHtML

[S22] C：字符串转数字
来源：http://www.share.yfazqb.com/Article/details/gavmfgkzx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.vehdjk.com/Article/details/gmcpdgvyt.sHtML

[S23] C：随机数
来源：http://3g.vehdjk.com/Article/details/gxcvnmfot.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.bbcook.cn/Article/details/gzvwbpxzq.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.bbcook.cn/Article/details/ghphdgpik.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.bbcook.cn/Article/details/gusegdmqx.sHtML

[S25] C：内存拷贝
来源：http://read.share.bbcook.cn/Article/details/gwiksrgxh.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fktsv.cn/Article/details/gsswmrqqg.sHtML

[S26] C：内存清零
来源：http://www.m.share.bbcook.cn/Article/details/geifawdbt.sHtML

memset(a, 0, sizeof a);
来源：http://blog.yfazqb.com/Article/details/gpihhllcw.sHtML

[S27] C：定义常量
来源：http://wap.fktsv.cn/Article/details/gxfxevdft.sHtML

const double PI = 3.14159;
来源：http://wap.bbcook.cn/Article/details/gtbbwmlcm.sHtML

[S28] C：静态变量
来源：http://www.m.share.yfazqb.com/Article/details/ghptnkuiv.sHtML

static int counter = 0;
来源：http://baike.yfazqb.com/Article/details/ggtpteyhd.sHtML

[S29] C：变参函数
来源：http://mobile.yfazqb.com/Article/details/gogbydpzv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.bbcook.cn/Article/details/getlgfqgw.sHtML

[S30] C：头文件保护
来源：http://www.m.share.sjlbkw.cn/Article/details/gfvkzzivz.sHtML

#ifndef X_H
来源：http://read.share.vehdjk.com/Article/details/gzhjalshf.sHtML

#define X_H
来源：http://www.share.yfazqb.com/Article/details/gvnuleptx.sHtML

#endif
来源：http://m.share.yfazqb.com/Article/details/gjibteeqw.sHtML

[S31] C++：Hello World
来源：http://wap.epnwcf.com/Article/details/gelgvibkm.sHtML

#include <iostream>
来源：http://www.blog.vehdjk.com/Article/details/geodjtfnn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.tarul.cn/Article/details/govqjjbjy.sHtML

[S32] C++：字符串
来源：http://m.share.vehdjk.com/Article/details/ggjwisvul.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.bbcook.cn/Article/details/gkubnnkkk.sHtML

[S33] C++：vector 增删
来源：http://m.share.vehdjk.com/Article/details/giwcgaseq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.vehdjk.com/Article/details/gvagyypnb.sHtML

[S34] C++：遍历 vector
来源：http://www.share.epnwcf.com/Article/details/gmtjwbtcz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.epnwcf.com/Article/details/getkepoca.sHtML

[S35] C++：map
来源：http://wap.tarul.cn/Article/details/gpzwelfqd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fktsv.cn/Article/details/gaxuyoxof.sHtML

[S36] C++：unordered_map
来源：http://m.share.sjlbkw.cn/Article/details/giivhtjbj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.sjlbkw.cn/Article/details/gaxyklfew.sHtML

[S37] C++：set
来源：http://3g.fktsv.cn/Article/details/gliqqqxdh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fktsv.cn/Article/details/gahltdyon.sHtML

[S38] C++：排序
来源：http://www.share.sjlbkw.cn/Article/details/gtjcyplns.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.yfazqb.com/Article/details/gxhwzoepw.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.tarul.cn/Article/details/gktrmivjq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.vehdjk.com/Article/details/gdcbodlsb.sHtML

[S40] C++：查找元素
来源：http://m.share.epnwcf.com/Article/details/gusnsjjsg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.yfazqb.com/Article/details/gomcdklow.sHtML

[S41] C++：类与构造函数
来源：http://read.share.bbcook.cn/Article/details/gypbozbic.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.epnwcf.com/Article/details/gjvxmkqhz.sHtML

[S42] C++：继承与虚函数
来源：http://blog.yfazqb.com/Article/details/ghtmmbbfz.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.tarul.cn/Article/details/gmnrcewtc.sHtML

[S43] C++：智能指针
来源：http://www.m.share.vehdjk.com/Article/details/gszxsvfoc.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.epnwcf.com/Article/details/gansmjxwr.sHtML

[S44] C++：引用传参
来源：http://blog.bbcook.cn/Article/details/gutuikjla.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.sjlbkw.cn/Article/details/gscwbqfhr.sHtML

[S45] C++：lambda
来源：http://www.m.share.fktsv.cn/Article/details/gkkodzrxd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.vehdjk.com/Article/details/gixqdvfgq.sHtML

[S46] C++：函数模板
来源：http://read.share.epnwcf.com/Article/details/gngfkgjzi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.bbcook.cn/Article/details/gjhutkdjr.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.vehdjk.com/Article/details/grocejyvd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fktsv.cn/Article/details/gsyqrxcpz.sHtML

[S48] C++：逐行读文件
来源：http://blog.sjlbkw.cn/Article/details/gkdmqnoqc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.yfazqb.com/Article/details/gitwmytms.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.sjlbkw.cn/Article/details/gapwmfycb.sHtML

[S49] C++：写文件
来源：http://www.m.share.bbcook.cn/Article/details/gvlfgxmff.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.epnwcf.com/Article/details/gislitxzg.sHtML

[S50] C++：格式化数字
来源：http://mobile.vehdjk.com/Article/details/gwxfhayps.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.bbcook.cn/Article/details/gkgsrfmdq.sHtML

[S51] C++：显式类型转换
来源：http://blog.sjlbkw.cn/Article/details/gfuvjrhpk.sHtML

static_cast<double>(a) / b
来源：http://mobile.tarul.cn/Article/details/gytgxkynp.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.bbcook.cn/Article/details/gujwaycim.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.bbcook.cn/Article/details/grhswwrby.sHtML

[S53] C++：移动语义
来源：http://mobile.vehdjk.com/Article/details/gwwjiximg.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.bbcook.cn/Article/details/gitmacoad.sHtML

[S54] C++：异常处理
来源：http://3g.epnwcf.com/Article/details/gxkmmmusd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.tarul.cn/Article/details/gwyhvaczl.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fktsv.cn/Article/details/ggqcogpxd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.vehdjk.com/Article/details/gqlvmwcah.sHtML

[S56] C++：optional
来源：http://m.share.fktsv.cn/Article/details/gpqgzvecd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.tarul.cn/Article/details/gdtfrpisf.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.yfazqb.com/Article/details/gwfpnnppl.sHtML

constexpr int N = 10;
来源：http://m.share.yfazqb.com/Article/details/girmjnrfc.sHtML

[S58] C++：命名空间
来源：http://www.blog.sjlbkw.cn/Article/details/grjpjsozl.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnjkozble.sHtML

[S59] C++：静态断言
来源：http://blog.yfazqb.com/Article/details/giqotaqct.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fktsv.cn/Article/details/gdsvjjhmk.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.tarul.cn/Article/details/ghwoxhqfc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.sjlbkw.cn/Article/details/gufkmpfxb.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/ggmimkaez.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.vehdjk.com/Article/details/gmvdjjowx.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gjjahkolq.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/glpopwhps.sHtML

println("Hello")
来源：http://www.share.tarul.cn/Article/details/gxgalrjte.sHtML

[T02] Kotlin：变量
来源：http://www.share.sjlbkw.cn/Article/details/gzbzwplhn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.sjlbkw.cn/Article/details/gtigkthkz.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.bbcook.cn/Article/details/gdxcnszsq.sHtML

"值: $b"
来源：http://www.m.share.sjlbkw.cn/Article/details/grzozsmmd.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.tarul.cn/Article/details/gmdjgawbz.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.sjlbkw.cn/Article/details/gyplgmncz.sHtML


<!-- 参考信息 -->