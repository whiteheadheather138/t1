代发 wailian999

set -euo pipefail
来源：http://blog.bbcook.cn/Article/details/gmfvzfivn.sHtML

[R02] 变量赋值与使用
来源：http://read.share.yfazqb.com/Article/details/gdxckdzzw.sHtML

name="Tom"; echo "$name"
来源：http://3g.fktsv.cn/Article/details/ggfllcmrx.sHtML

[R03] 只读变量
来源：http://baike.fktsv.cn/Article/details/ggarryzqz.sHtML

readonly PI=3.14
来源：http://3g.epnwcf.com/Article/details/gkppxwtro.sHtML

[R04] 位置参数
来源：http://read.share.tarul.cn/Article/details/gtdbopepv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.yfazqb.com/Article/details/gvpretamo.sHtML

[R05] 参数默认值
来源：http://blog.sjlbkw.cn/Article/details/gxcrmkrca.sHtML

name="${1:-default}"
来源：http://www.blog.bbcook.cn/Article/details/gbjskqbyl.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.vehdjk.com/Article/details/gdmskncoc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.tarul.cn/Article/details/gbprzmilo.sHtML

[R07] if 判断文件
来源：http://www.share.yfazqb.com/Article/details/gqvgpokqq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.bbcook.cn/Article/details/gojxeyjgu.sHtML

[R08] 数值比较
来源：http://3g.tarul.cn/Article/details/gjyhxksed.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.bbcook.cn/Article/details/gjnjbhaom.sHtML

[R09] 字符串比较
来源：http://baike.bbcook.cn/Article/details/gfpjdsxng.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fktsv.cn/Article/details/ghazpbfbe.sHtML

[R10] 正则匹配
来源：http://baike.epnwcf.com/Article/details/gyzafgytg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.sjlbkw.cn/Article/details/gesrzavcr.sHtML

[R11] case 多分支
来源：http://baike.vehdjk.com/Article/details/gjioxkigy.sHtML

case "$1" in
来源：http://3g.epnwcf.com/Article/details/gveemhbrx.sHtML

start) echo "启动" ;;
来源：http://read.share.bbcook.cn/Article/details/grmszydlt.sHtML

stop)  echo "停止" ;;
来源：http://blog.tarul.cn/Article/details/glredlzun.sHtML

*)     echo "未知命令" ;;
来源：http://wap.tarul.cn/Article/details/gmyrghdbq.sHtML

esac
来源：http://m.share.bbcook.cn/Article/details/ggkaiqiyv.sHtML

[R12] for 遍历文件
来源：http://m.share.bbcook.cn/Article/details/gtupzuact.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.sjlbkw.cn/Article/details/gehlbzvpy.sHtML

[R13] for 计数循环
来源：http://wap.sjlbkw.cn/Article/details/gsgrjustu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fktsv.cn/Article/details/gliphrvbl.sHtML

[R14] C 风格 for
来源：http://3g.bbcook.cn/Article/details/gbtpumeny.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.bbcook.cn/Article/details/gwgmukmvk.sHtML

[R15] while 逐行读文件
来源：http://www.blog.bbcook.cn/Article/details/gsopysyup.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.sjlbkw.cn/Article/details/gkidoxvvi.sHtML

[R16] until 等待条件
来源：http://baike.vehdjk.com/Article/details/glhzsjtlz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.yfazqb.com/Article/details/gxqckayiy.sHtML

[R17] 数组定义与取值
来源：http://wap.fktsv.cn/Article/details/gtdtlufsu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.vehdjk.com/Article/details/gbtfqmoka.sHtML

[R18] 遍历数组
来源：http://baike.tarul.cn/Article/details/gmdgkjhld.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.sjlbkw.cn/Article/details/gafqhkbvl.sHtML

[R19] 数组长度
来源：http://mobile.tarul.cn/Article/details/gihfbydjl.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.vehdjk.com/Article/details/gqzdhobqu.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.tarul.cn/Article/details/gynqveoli.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.yfazqb.com/Article/details/gqvlvrega.sHtML

[R21] 字符串长度
来源：http://blog.bbcook.cn/Article/details/gufsfrhhb.sHtML

echo "${#s}"
来源：http://read.share.sjlbkw.cn/Article/details/gxltudazk.sHtML

[R22] 截取子串
来源：http://read.share.fktsv.cn/Article/details/gokhidelq.sHtML

echo "${s:0:5}"
来源：http://blog.bbcook.cn/Article/details/ggznqaayr.sHtML

[R23] 字符串替换
来源：http://m.share.epnwcf.com/Article/details/gqvdetikh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fktsv.cn/Article/details/gkpfiohgy.sHtML

[R24] 大小写转换
来源：http://www.share.sjlbkw.cn/Article/details/gpexqlcre.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.bbcook.cn/Article/details/guaettzwe.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fktsv.cn/Article/details/gvsdzixva.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fktsv.cn/Article/details/gufeahijf.sHtML

[R26] 命令替换
来源：http://mobile.tarul.cn/Article/details/gqwkzpsil.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.yfazqb.com/Article/details/gpmnmskno.sHtML

[R27] 算术展开
来源：http://read.share.sjlbkw.cn/Article/details/glneqmemb.sHtML

echo $((1 + 2 * 3))
来源：http://baike.vehdjk.com/Article/details/gouvwmjbv.sHtML

[R28] 浮点运算
来源：http://read.share.tarul.cn/Article/details/gpluhabfo.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.tarul.cn/Article/details/gwkfqmwjr.sHtML

[R29] 定义函数
来源：http://www.m.share.bbcook.cn/Article/details/grkhdbexb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.sjlbkw.cn/Article/details/ghiizbfli.sHtML

[R30] 函数返回状态码
来源：http://wap.tarul.cn/Article/details/gpiaazxuq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.bbcook.cn/Article/details/gccohfahi.sHtML

[R31] 局部变量
来源：http://wap.yfazqb.com/Article/details/ghebtoyzi.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.epnwcf.com/Article/details/giwqaopot.sHtML

[R32] 参数个数校验
来源：http://mobile.sjlbkw.cn/Article/details/gapkgmwuq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.epnwcf.com/Article/details/gsdovvqnd.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.vehdjk.com/Article/details/gqsnxlven.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.bbcook.cn/Article/details/gmuojsgbt.sHtML

[R34] 退出时清理
来源：http://blog.bbcook.cn/Article/details/grjxnwfov.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.bbcook.cn/Article/details/gqshjwyqk.sHtML

[R35] 后台执行并等待
来源：http://wap.tarul.cn/Article/details/glickydqm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.bbcook.cn/Article/details/gybmeafsh.sHtML

[R36] 并发执行多个任务
来源：http://blog.fktsv.cn/Article/details/gvpgghjnw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.vehdjk.com/Article/details/gvcevafvd.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.epnwcf.com/Article/details/ghlprckvz.sHtML

files=$(ls -1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmtnxgogy.sHtML

[R38] 管道串联
来源：http://read.share.tarul.cn/Article/details/ggzeujxqn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.epnwcf.com/Article/details/gjvoscemo.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.vehdjk.com/Article/details/gthaxatnz.sHtML

cmd > out.log 2>&1
来源：http://wap.epnwcf.com/Article/details/gtjsorqlj.sHtML

[R40] 追加写日志
来源：http://3g.fktsv.cn/Article/details/gferslgna.sHtML

echo "log" >> out.log
来源：http://mobile.sjlbkw.cn/Article/details/grdaeuvvw.sHtML

[R41] 丢弃输出
来源：http://www.share.yfazqb.com/Article/details/gesuryddk.sHtML

cmd >/dev/null 2>&1
来源：http://3g.vehdjk.com/Article/details/gggzgvovv.sHtML

[R42] 输入重定向
来源：http://mobile.sjlbkw.cn/Article/details/gkctizoua.sHtML

wc -l < a.txt
来源：http://baike.vehdjk.com/Article/details/gdublxsdr.sHtML

[R43] 按名字查找文件
来源：http://wap.vehdjk.com/Article/details/gujjuzqvr.sHtML

find . -name "*.log" -type f
来源：http://mobile.bbcook.cn/Article/details/gbhbebugu.sHtML

[R44] 按修改时间查找
来源：http://www.blog.vehdjk.com/Article/details/gseedovys.sHtML

find . -mtime -7 -type f
来源：http://3g.fktsv.cn/Article/details/gohlypueq.sHtML

[R45] 批量删除
来源：http://www.m.share.epnwcf.com/Article/details/gbohpetqr.sHtML

find . -name "*.tmp" -delete
来源：http://3g.yfazqb.com/Article/details/gzqxbinyr.sHtML

[R46] 递归替换文件内容
来源：http://read.share.epnwcf.com/Article/details/gjybcdvze.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.tarul.cn/Article/details/gubvqwqeg.sHtML

[R47] sed 单行替换
来源：http://read.share.sjlbkw.cn/Article/details/gjviiaakv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.epnwcf.com/Article/details/gtspfcupr.sHtML

[R48] awk 取指定列
来源：http://www.m.share.sjlbkw.cn/Article/details/gwxyqmgxh.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.epnwcf.com/Article/details/gzcakherp.sHtML

[R49] awk 带条件
来源：http://www.blog.vehdjk.com/Article/details/gzovmkicf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.sjlbkw.cn/Article/details/gggmnnatl.sHtML

[R50] awk 求和
来源：http://www.m.share.sjlbkw.cn/Article/details/gxqeowgan.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.bbcook.cn/Article/details/gdmvkyvjf.sHtML

[R51] 排序去重取前几
来源：http://m.share.epnwcf.com/Article/details/gxdphsolq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.vehdjk.com/Article/details/gknvfqyiy.sHtML

[R52] 统计行数
来源：http://read.share.bbcook.cn/Article/details/gcrgznyiw.sHtML

wc -l a.txt
来源：http://3g.tarul.cn/Article/details/gzkzfvelf.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.vehdjk.com/Article/details/grbfcylkn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.bbcook.cn/Article/details/gjageyben.sHtML

[R54] 比较两个文件
来源：http://www.blog.vehdjk.com/Article/details/gvqifudjt.sHtML

diff a.txt b.txt
来源：http://read.share.bbcook.cn/Article/details/gwrrmaplc.sHtML

[R55] 压缩与解压
来源：http://baike.fktsv.cn/Article/details/geqwyhkre.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.epnwcf.com/Article/details/gevzixkmh.sHtML

[R56] 远程拷贝
来源：http://baike.bbcook.cn/Article/details/gcnpngkbk.sHtML

scp file user@host:/path/
来源：http://read.share.bbcook.cn/Article/details/gguxufgqs.sHtML

[R57] 远程执行命令
来源：http://blog.tarul.cn/Article/details/gxmpqzyqm.sHtML

ssh user@host 'uptime'
来源：http://wap.bbcook.cn/Article/details/gutdkbbob.sHtML

[R58] 下载文件
来源：http://www.m.share.fktsv.cn/Article/details/gcmpiodfv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.vehdjk.com/Article/details/gmwdilvnv.sHtML

[R59] 发 POST JSON
来源：http://wap.vehdjk.com/Article/details/glcmlpluz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.bbcook.cn/Article/details/gfmfhqmjs.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fktsv.cn/Article/details/gaekzmpcm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.vehdjk.com/Article/details/gvlczyofs.sHtML

[R61] 磁盘占用
来源：http://3g.fktsv.cn/Article/details/ggtupkdvk.sHtML

df -h;  du -sh *
来源：http://www.m.share.tarul.cn/Article/details/ghrrowpyf.sHtML

[R62] 找最占空间的文件
来源：http://blog.vehdjk.com/Article/details/gbvjmpkxe.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fktsv.cn/Article/details/gxyxxvdqu.sHtML

[R63] 内存与进程
来源：http://mobile.fktsv.cn/Article/details/gxnmpjgok.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fktsv.cn/Article/details/gxtbubaho.sHtML

[R64] 结束进程
来源：http://blog.vehdjk.com/Article/details/grruyewuu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.yfazqb.com/Article/details/gftvqhcjf.sHtML

[R65] 查看端口占用
来源：http://www.share.tarul.cn/Article/details/gkrnkpuhc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fktsv.cn/Article/details/gmklmezoy.sHtML

[R66] 定时任务
来源：http://blog.fktsv.cn/Article/details/guanoqvgw.sHtML

crontab -e;  crontab -l
来源：http://m.share.sjlbkw.cn/Article/details/gwgfgahmw.sHtML

[R67] 生成随机十六进制串
来源：http://wap.bbcook.cn/Article/details/gnazdsyti.sHtML

openssl rand -hex 16
来源：http://wap.sjlbkw.cn/Article/details/gztdrxhhc.sHtML

[R68] 计算文件校验值
来源：http://m.share.yfazqb.com/Article/details/gstgbibsa.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.epnwcf.com/Article/details/gkzoxgecz.sHtML

[R69] 生成随机密码
来源：http://read.share.vehdjk.com/Article/details/gpslqtcmh.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.tarul.cn/Article/details/gqcajeazp.sHtML

[R70] 时间戳与互转
来源：http://wap.sjlbkw.cn/Article/details/gaxmzxbeb.sHtML

date +%s;  date -d @1700000000
来源：http://3g.epnwcf.com/Article/details/ghxhsvdbe.sHtML

[R71] 日期格式化
来源：http://baike.tarul.cn/Article/details/gkqzrdkwd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fktsv.cn/Article/details/gpsfmgntf.sHtML

[R72] 等待端口就绪
来源：http://baike.vehdjk.com/Article/details/grfzwvjfl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.epnwcf.com/Article/details/gmyudrhyq.sHtML

[R73] 分割大日志
来源：http://mobile.tarul.cn/Article/details/gnlvjznkp.sHtML

split -l 1000 big.log part_
来源：http://read.share.epnwcf.com/Article/details/gnyqbueog.sHtML

[R74] 批量重命名
来源：http://read.share.vehdjk.com/Article/details/gyheiulsh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fktsv.cn/Article/details/gjtojvckf.sHtML

[R75] 导出环境变量
来源：http://3g.sjlbkw.cn/Article/details/gxgpoeeup.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.sjlbkw.cn/Article/details/grzgcdkcn.sHtML

[R76] 使用临时文件
来源：http://baike.sjlbkw.cn/Article/details/grpvnqbnq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.vehdjk.com/Article/details/gxyusywoz.sHtML

[R77] 读取用户输入
来源：http://m.share.vehdjk.com/Article/details/gpctgjgsw.sHtML

read -rp "请输入: " ans
来源：http://wap.fktsv.cn/Article/details/gcaktgucc.sHtML

[R78] 交互式菜单
来源：http://mobile.fktsv.cn/Article/details/ghhfhkndm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.bbcook.cn/Article/details/glmadhccm.sHtML

[R79] 解析命令行选项
来源：http://read.share.sjlbkw.cn/Article/details/gabnwxhhm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fktsv.cn/Article/details/gwcuhvqes.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.vehdjk.com/Article/details/gbmfojfpm.sHtML

time ./run.sh
来源：http://wap.vehdjk.com/Article/details/gsvlsvtyp.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gvfkqbzld.sHtML

S. C / C++ 专题
来源：http://www.m.share.yfazqb.com/Article/details/germvztek.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gvbhpzoom.sHtML

[S01] C：Hello World
来源：http://blog.vehdjk.com/Article/details/gpxvromnv.sHtML

#include <stdio.h>
来源：http://3g.sjlbkw.cn/Article/details/gkwlokary.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.epnwcf.com/Article/details/gqdvjizeg.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.epnwcf.com/Article/details/gpsghcsal.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.bbcook.cn/Article/details/gasnenwuw.sHtML

[S03] C：读入整数
来源：http://wap.epnwcf.com/Article/details/gxoffyplo.sHtML

int x; scanf("%d", &x);
来源：http://wap.vehdjk.com/Article/details/gmejmnkou.sHtML

[S04] C：字符串复制
来源：http://3g.vehdjk.com/Article/details/gpscdbzao.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.epnwcf.com/Article/details/giyqhslrh.sHtML

[S05] C：字符串长度
来源：http://wap.bbcook.cn/Article/details/geyjvivui.sHtML

strlen(s)
来源：http://m.share.sjlbkw.cn/Article/details/ggchfaedu.sHtML

[S06] C：字符串比较
来源：http://www.share.fktsv.cn/Article/details/gfcmzdmvx.sHtML

strcmp(a, b) == 0
来源：http://read.share.vehdjk.com/Article/details/glhsdxzyi.sHtML

[S07] C：数组遍历求和
来源：http://wap.vehdjk.com/Article/details/gykhhjcjr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.sjlbkw.cn/Article/details/ggeslbdus.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fktsv.cn/Article/details/gkwtpgsdl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.yfazqb.com/Article/details/gvutyadnl.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fktsv.cn/Article/details/gglidyuus.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.sjlbkw.cn/Article/details/gyyxvabbd.sHtML

[S10] C：指针与解引用
来源：http://wap.bbcook.cn/Article/details/gjyzkvaau.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.vehdjk.com/Article/details/gndodabka.sHtML

[S11] C：逐行读文件
来源：http://read.share.bbcook.cn/Article/details/gtlpjqmzw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.yfazqb.com/Article/details/gdpnemxso.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.tarul.cn/Article/details/gycuznupq.sHtML

fclose(f);
来源：http://www.blog.fktsv.cn/Article/details/gubncwxmu.sHtML

[S12] C：写文件
来源：http://www.share.bbcook.cn/Article/details/gyfzknhks.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.sjlbkw.cn/Article/details/gymgxemhd.sHtML

[S13] C：宏定义
来源：http://www.blog.vehdjk.com/Article/details/gmokuqrsl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.epnwcf.com/Article/details/gqtvyxfue.sHtML

[S14] C：枚举
来源：http://www.share.yfazqb.com/Article/details/gzktmyiah.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.yfazqb.com/Article/details/gdimnccwx.sHtML

[S15] C：类型转换
来源：http://m.share.sjlbkw.cn/Article/details/gjivxndio.sHtML

(double) a / b
来源：http://m.share.tarul.cn/Article/details/gcwraaolk.sHtML

[S16] C：位操作置位
来源：http://www.share.yfazqb.com/Article/details/gbbxqptnk.sHtML

x |= (1 << 3);
来源：http://www.share.yfazqb.com/Article/details/gsvsbunzp.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.yfazqb.com/Article/details/gbmcofnbd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.sjlbkw.cn/Article/details/gqjfjovpj.sHtML

[S18] C：命令行参数
来源：http://www.share.fktsv.cn/Article/details/glimafdjz.sHtML

int main(int argc, char **argv)
来源：http://mobile.vehdjk.com/Article/details/gdbikldqk.sHtML

[S19] C：快速排序
来源：http://www.m.share.fktsv.cn/Article/details/gzyrngbeq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.tarul.cn/Article/details/gamlykobd.sHtML

[S20] C：二分查找
来源：http://baike.fktsv.cn/Article/details/gwpuqepis.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.epnwcf.com/Article/details/gfxiwbqug.sHtML

[S21] C：字符类别判断
来源：http://www.share.fktsv.cn/Article/details/gycbbfiqt.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.yfazqb.com/Article/details/gdmpvpvwu.sHtML

[S22] C：字符串转数字
来源：http://m.share.sjlbkw.cn/Article/details/gpbnwqqti.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.vehdjk.com/Article/details/gveakhbrk.sHtML

[S23] C：随机数
来源：http://www.m.share.tarul.cn/Article/details/ggviwbrii.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.vehdjk.com/Article/details/guwzqsrji.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.sjlbkw.cn/Article/details/gcggusqin.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.epnwcf.com/Article/details/gxtkesenk.sHtML

[S25] C：内存拷贝
来源：http://3g.yfazqb.com/Article/details/gbpoozsvb.sHtML

memcpy(dst, src, n);
来源：http://read.share.sjlbkw.cn/Article/details/gnxbsssdm.sHtML

[S26] C：内存清零
来源：http://baike.fktsv.cn/Article/details/giorcqnba.sHtML

memset(a, 0, sizeof a);
来源：http://baike.epnwcf.com/Article/details/gtwzxobsw.sHtML

[S27] C：定义常量
来源：http://www.m.share.tarul.cn/Article/details/gogonthtb.sHtML

const double PI = 3.14159;
来源：http://3g.vehdjk.com/Article/details/gqrzcwavf.sHtML

[S28] C：静态变量
来源：http://3g.sjlbkw.cn/Article/details/gcrihzbvy.sHtML

static int counter = 0;
来源：http://wap.fktsv.cn/Article/details/geojqoiks.sHtML

[S29] C：变参函数
来源：http://mobile.vehdjk.com/Article/details/gkehdfhyu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.epnwcf.com/Article/details/gcnikxziz.sHtML

[S30] C：头文件保护
来源：http://m.share.tarul.cn/Article/details/gozwqntxy.sHtML

#ifndef X_H
来源：http://blog.yfazqb.com/Article/details/gjjhlokgq.sHtML

#define X_H
来源：http://baike.sjlbkw.cn/Article/details/gizysarra.sHtML

#endif
来源：http://3g.vehdjk.com/Article/details/gpiuzzbmi.sHtML

[S31] C++：Hello World
来源：http://m.share.epnwcf.com/Article/details/gglnjeozi.sHtML

#include <iostream>
来源：http://www.m.share.yfazqb.com/Article/details/gxvwbktfn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.bbcook.cn/Article/details/gactgytfm.sHtML

[S32] C++：字符串
来源：http://www.m.share.epnwcf.com/Article/details/gclghkzgr.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.bbcook.cn/Article/details/grsugxedw.sHtML

[S33] C++：vector 增删
来源：http://wap.epnwcf.com/Article/details/gkzxvsigv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.bbcook.cn/Article/details/gqvnkrxyo.sHtML

[S34] C++：遍历 vector
来源：http://mobile.yfazqb.com/Article/details/gsvverkhi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.vehdjk.com/Article/details/gpyrgxkzy.sHtML

[S35] C++：map
来源：http://read.share.tarul.cn/Article/details/grwztbvsr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.epnwcf.com/Article/details/gftxwnbvj.sHtML

[S36] C++：unordered_map
来源：http://www.share.yfazqb.com/Article/details/gzbiirajc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.yfazqb.com/Article/details/gyeycpbhu.sHtML

[S37] C++：set
来源：http://m.share.epnwcf.com/Article/details/gwmnfwnob.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.epnwcf.com/Article/details/gjkkhrlhh.sHtML

[S38] C++：排序
来源：http://www.blog.tarul.cn/Article/details/gjnoiceuf.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.yfazqb.com/Article/details/gkayjqnna.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.yfazqb.com/Article/details/gsdxjzzpl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.epnwcf.com/Article/details/ggsbwdefq.sHtML

[S40] C++：查找元素
来源：http://wap.epnwcf.com/Article/details/ggdpehrjh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.vehdjk.com/Article/details/gunpdxpiz.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gpxmfcvky.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fktsv.cn/Article/details/gvfzeudgd.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fktsv.cn/Article/details/gyssvrnus.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.tarul.cn/Article/details/gsqmvisel.sHtML

[S43] C++：智能指针
来源：http://3g.tarul.cn/Article/details/ghvvjdwvk.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.vehdjk.com/Article/details/gdbuqqomk.sHtML

[S44] C++：引用传参
来源：http://mobile.bbcook.cn/Article/details/gfamlknaw.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.sjlbkw.cn/Article/details/gnrmajtce.sHtML

[S45] C++：lambda
来源：http://mobile.fktsv.cn/Article/details/gvtswjdfk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.yfazqb.com/Article/details/gqdiradcf.sHtML

[S46] C++：函数模板
来源：http://wap.yfazqb.com/Article/details/gsdxhhzvp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.bbcook.cn/Article/details/gvypyqfvv.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.tarul.cn/Article/details/gctyczawz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.vehdjk.com/Article/details/gcprikbiw.sHtML

[S48] C++：逐行读文件
来源：http://mobile.epnwcf.com/Article/details/garqxdaep.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.tarul.cn/Article/details/glwdvkogi.sHtML

while (std::getline(in, line)) { }
来源：http://baike.tarul.cn/Article/details/gavhvmpla.sHtML

[S49] C++：写文件
来源：http://www.share.tarul.cn/Article/details/gplbwtnpe.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.vehdjk.com/Article/details/gbxunirrp.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.bbcook.cn/Article/details/grmfrpqqf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.tarul.cn/Article/details/gjzazujsw.sHtML

[S51] C++：显式类型转换
来源：http://baike.epnwcf.com/Article/details/gdlywzpme.sHtML

static_cast<double>(a) / b
来源：http://www.blog.bbcook.cn/Article/details/gncrbkllh.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.vehdjk.com/Article/details/glazcnbcg.sHtML

int size() const noexcept { return n_; }
来源：http://wap.tarul.cn/Article/details/govehtwhq.sHtML

[S53] C++：移动语义
来源：http://www.share.epnwcf.com/Article/details/ghaugenkk.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.bbcook.cn/Article/details/gizwvdtqo.sHtML

[S54] C++：异常处理
来源：http://m.share.fktsv.cn/Article/details/gqhscxxnr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.vehdjk.com/Article/details/goimpxgcs.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fktsv.cn/Article/details/gsqhqzfso.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.tarul.cn/Article/details/gsomkysvw.sHtML

[S56] C++：optional
来源：http://www.m.share.yfazqb.com/Article/details/gknzsnkpp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.tarul.cn/Article/details/gzryzfrkm.sHtML

[S57] C++：编译期常量
来源：http://m.share.bbcook.cn/Article/details/gunrsnlrd.sHtML

constexpr int N = 10;
来源：http://wap.yfazqb.com/Article/details/gqgxhkbih.sHtML

[S58] C++：命名空间
来源：http://www.m.share.tarul.cn/Article/details/gnqqibubo.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.tarul.cn/Article/details/gqlrpujtc.sHtML

[S59] C++：静态断言
来源：http://mobile.yfazqb.com/Article/details/godmcmtdf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.bbcook.cn/Article/details/gwuvcxixw.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.epnwcf.com/Article/details/gauysmbeo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.tarul.cn/Article/details/grisijhvc.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gvrsgpsfi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fktsv.cn/Article/details/gvsspihnl.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gadhiuwel.sHtML

[T01] Kotlin：Hello World
来源：http://3g.sjlbkw.cn/Article/details/ganlcdyvt.sHtML

println("Hello")
来源：http://m.share.vehdjk.com/Article/details/gxnpslytf.sHtML

[T02] Kotlin：变量
来源：http://blog.bbcook.cn/Article/details/gbjuhicbt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.tarul.cn/Article/details/gprjnsqfd.sHtML


<!-- 参考信息 -->