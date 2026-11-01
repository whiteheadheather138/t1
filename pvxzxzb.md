代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.vehdjk.com/Article/details/gwtccvffk.sHtML

[R08] 数值比较
来源：http://wap.bbcook.cn/Article/details/gduxxuhok.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.epnwcf.com/Article/details/gmfijoffi.sHtML

[R09] 字符串比较
来源：http://read.share.vehdjk.com/Article/details/gdqduhftn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.vehdjk.com/Article/details/gsotkyhkn.sHtML

[R10] 正则匹配
来源：http://3g.yfazqb.com/Article/details/gvpzkxbms.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.vehdjk.com/Article/details/gmcejafbp.sHtML

[R11] case 多分支
来源：http://baike.epnwcf.com/Article/details/gmimyfthe.sHtML

case "$1" in
来源：http://www.share.fktsv.cn/Article/details/gguhqlueb.sHtML

start) echo "启动" ;;
来源：http://blog.tarul.cn/Article/details/gcazhmbgv.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.yfazqb.com/Article/details/gqohhqlui.sHtML

*)     echo "未知命令" ;;
来源：http://wap.sjlbkw.cn/Article/details/gmjuwecis.sHtML

esac
来源：http://3g.vehdjk.com/Article/details/gaefzbyog.sHtML

[R12] for 遍历文件
来源：http://blog.vehdjk.com/Article/details/glzwrrwwp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.epnwcf.com/Article/details/gbnwblwrj.sHtML

[R13] for 计数循环
来源：http://www.blog.vehdjk.com/Article/details/gjjjcogbx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.vehdjk.com/Article/details/gymdyyfri.sHtML

[R14] C 风格 for
来源：http://www.m.share.fktsv.cn/Article/details/gxybwfcrm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.tarul.cn/Article/details/gezhkdmdp.sHtML

[R15] while 逐行读文件
来源：http://www.share.vehdjk.com/Article/details/gacgygddf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fktsv.cn/Article/details/gscfqoymv.sHtML

[R16] until 等待条件
来源：http://read.share.vehdjk.com/Article/details/givovowse.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.epnwcf.com/Article/details/gjhkzcega.sHtML

[R17] 数组定义与取值
来源：http://3g.vehdjk.com/Article/details/gjairkvcq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.yfazqb.com/Article/details/gybfwayzx.sHtML

[R18] 遍历数组
来源：http://www.m.share.vehdjk.com/Article/details/gofrfszwl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fktsv.cn/Article/details/gabacmnia.sHtML

[R19] 数组长度
来源：http://3g.sjlbkw.cn/Article/details/gilvgbjkv.sHtML

echo "${#arr[@]}"
来源：http://www.share.epnwcf.com/Article/details/gkdzgnkez.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.bbcook.cn/Article/details/goqajaaxz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.tarul.cn/Article/details/gatnkchsc.sHtML

[R21] 字符串长度
来源：http://baike.sjlbkw.cn/Article/details/gizbnlxmq.sHtML

echo "${#s}"
来源：http://read.share.bbcook.cn/Article/details/gunysxhwb.sHtML

[R22] 截取子串
来源：http://read.share.fktsv.cn/Article/details/gtpkkdxvd.sHtML

echo "${s:0:5}"
来源：http://blog.fktsv.cn/Article/details/gvultfxxj.sHtML

[R23] 字符串替换
来源：http://read.share.tarul.cn/Article/details/gnbptzviw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.yfazqb.com/Article/details/gvmfgwzbe.sHtML

[R24] 大小写转换
来源：http://m.share.sjlbkw.cn/Article/details/gdubqqseo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.yfazqb.com/Article/details/gznvotiav.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.epnwcf.com/Article/details/gcrqoeple.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fktsv.cn/Article/details/gfxhoaqvp.sHtML

[R26] 命令替换
来源：http://www.blog.epnwcf.com/Article/details/gjuelrhid.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.yfazqb.com/Article/details/gvlyfuijf.sHtML

[R27] 算术展开
来源：http://wap.fktsv.cn/Article/details/grxcikywl.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.bbcook.cn/Article/details/grghgmwio.sHtML

[R28] 浮点运算
来源：http://www.blog.vehdjk.com/Article/details/gorczrcgh.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.yfazqb.com/Article/details/gsslnsbih.sHtML

[R29] 定义函数
来源：http://3g.fktsv.cn/Article/details/gndzihfcs.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fktsv.cn/Article/details/gdifhfibf.sHtML

[R30] 函数返回状态码
来源：http://read.share.fktsv.cn/Article/details/gurjzglur.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.yfazqb.com/Article/details/gbehyklip.sHtML

[R31] 局部变量
来源：http://www.share.sjlbkw.cn/Article/details/gaknnbquv.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.sjlbkw.cn/Article/details/gsdsmjjan.sHtML

[R32] 参数个数校验
来源：http://www.m.share.yfazqb.com/Article/details/gepysajab.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.vehdjk.com/Article/details/gusnuxvkc.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.sjlbkw.cn/Article/details/gafqlipwi.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.epnwcf.com/Article/details/glotjbich.sHtML

[R34] 退出时清理
来源：http://baike.bbcook.cn/Article/details/gacmfolzd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.sjlbkw.cn/Article/details/glrsinnoo.sHtML

[R35] 后台执行并等待
来源：http://blog.sjlbkw.cn/Article/details/gohtcogal.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fktsv.cn/Article/details/gqpustiur.sHtML

[R36] 并发执行多个任务
来源：http://m.share.epnwcf.com/Article/details/gcidkwfmh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.bbcook.cn/Article/details/gmyxobqdu.sHtML

[R37] 把输出赋给变量
来源：http://www.share.tarul.cn/Article/details/gvbbdbwxx.sHtML

files=$(ls -1)
来源：http://www.blog.yfazqb.com/Article/details/gzzeesnmt.sHtML

[R38] 管道串联
来源：http://www.share.epnwcf.com/Article/details/gguqsjril.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.epnwcf.com/Article/details/gqnwtifyo.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.tarul.cn/Article/details/gvugzolkz.sHtML

cmd > out.log 2>&1
来源：http://www.share.fktsv.cn/Article/details/gsnyjqgjg.sHtML

[R40] 追加写日志
来源：http://baike.vehdjk.com/Article/details/gkkkxhjfb.sHtML

echo "log" >> out.log
来源：http://www.share.tarul.cn/Article/details/gsdtydffz.sHtML

[R41] 丢弃输出
来源：http://wap.vehdjk.com/Article/details/gzwruogan.sHtML

cmd >/dev/null 2>&1
来源：http://wap.vehdjk.com/Article/details/gpluudsek.sHtML

[R42] 输入重定向
来源：http://baike.vehdjk.com/Article/details/gbbastxfa.sHtML

wc -l < a.txt
来源：http://mobile.epnwcf.com/Article/details/gfzzcynkw.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.bbcook.cn/Article/details/gyymmafpx.sHtML

find . -name "*.log" -type f
来源：http://baike.fktsv.cn/Article/details/gvwncjkcv.sHtML

[R44] 按修改时间查找
来源：http://baike.yfazqb.com/Article/details/gnwyaqvue.sHtML

find . -mtime -7 -type f
来源：http://mobile.vehdjk.com/Article/details/gkfrwpvxe.sHtML

[R45] 批量删除
来源：http://m.share.tarul.cn/Article/details/gwspnvook.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.yfazqb.com/Article/details/gundslvvv.sHtML

[R46] 递归替换文件内容
来源：http://wap.tarul.cn/Article/details/gwloaqxwh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.yfazqb.com/Article/details/gcxoveybs.sHtML

[R47] sed 单行替换
来源：http://blog.fktsv.cn/Article/details/ghexbedqo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.epnwcf.com/Article/details/glpettrzk.sHtML

[R48] awk 取指定列
来源：http://www.blog.sjlbkw.cn/Article/details/gkoyoxwgm.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.yfazqb.com/Article/details/gpwauhnxs.sHtML

[R49] awk 带条件
来源：http://www.m.share.tarul.cn/Article/details/gijzxdeqf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.vehdjk.com/Article/details/ghgtkmdqa.sHtML

[R50] awk 求和
来源：http://blog.bbcook.cn/Article/details/gyweneove.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.vehdjk.com/Article/details/giojopojk.sHtML

[R51] 排序去重取前几
来源：http://blog.sjlbkw.cn/Article/details/giqqoepcq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.vehdjk.com/Article/details/ggbdkairy.sHtML

[R52] 统计行数
来源：http://www.m.share.yfazqb.com/Article/details/geyzbbjip.sHtML

wc -l a.txt
来源：http://mobile.sjlbkw.cn/Article/details/gqgeueqfs.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fktsv.cn/Article/details/gkkwhitiq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.vehdjk.com/Article/details/gdlxrpkrj.sHtML

[R54] 比较两个文件
来源：http://www.share.bbcook.cn/Article/details/gvpodxeyx.sHtML

diff a.txt b.txt
来源：http://www.blog.tarul.cn/Article/details/gqelpdxzu.sHtML

[R55] 压缩与解压
来源：http://3g.vehdjk.com/Article/details/gaxghlilw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.epnwcf.com/Article/details/gehmmggzn.sHtML

[R56] 远程拷贝
来源：http://www.blog.sjlbkw.cn/Article/details/gzatqyhvs.sHtML

scp file user@host:/path/
来源：http://3g.fktsv.cn/Article/details/gwclipeag.sHtML

[R57] 远程执行命令
来源：http://m.share.tarul.cn/Article/details/gkmknxhtu.sHtML

ssh user@host 'uptime'
来源：http://mobile.vehdjk.com/Article/details/gvxzsahge.sHtML

[R58] 下载文件
来源：http://baike.bbcook.cn/Article/details/gurimwgtl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.epnwcf.com/Article/details/gphjgovoq.sHtML

[R59] 发 POST JSON
来源：http://wap.tarul.cn/Article/details/gfjvcejtk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fktsv.cn/Article/details/ggljfclbr.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.sjlbkw.cn/Article/details/gcjxmgsaw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.tarul.cn/Article/details/gfzrwwllh.sHtML

[R61] 磁盘占用
来源：http://3g.yfazqb.com/Article/details/gfvzbipgq.sHtML

df -h;  du -sh *
来源：http://m.share.yfazqb.com/Article/details/gacynfptc.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fktsv.cn/Article/details/gwujwecws.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.tarul.cn/Article/details/gwnyweiar.sHtML

[R63] 内存与进程
来源：http://www.blog.bbcook.cn/Article/details/gwrmkgwgt.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.yfazqb.com/Article/details/ggrufdtxk.sHtML

[R64] 结束进程
来源：http://baike.tarul.cn/Article/details/gwyouvslw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.tarul.cn/Article/details/grwnfggvl.sHtML

[R65] 查看端口占用
来源：http://wap.epnwcf.com/Article/details/gdbgtfbph.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.epnwcf.com/Article/details/gretvcsbh.sHtML

[R66] 定时任务
来源：http://read.share.tarul.cn/Article/details/gbtadspfz.sHtML

crontab -e;  crontab -l
来源：http://mobile.vehdjk.com/Article/details/gcadwctjb.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.bbcook.cn/Article/details/gaxkmjlvc.sHtML

openssl rand -hex 16
来源：http://www.blog.vehdjk.com/Article/details/gviyrkxet.sHtML

[R68] 计算文件校验值
来源：http://baike.fktsv.cn/Article/details/gkixljajs.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fktsv.cn/Article/details/geibmsvjt.sHtML

[R69] 生成随机密码
来源：http://read.share.vehdjk.com/Article/details/gepbwbozu.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.tarul.cn/Article/details/gjliovkmt.sHtML

[R70] 时间戳与互转
来源：http://3g.tarul.cn/Article/details/ghhwsbdbf.sHtML

date +%s;  date -d @1700000000
来源：http://blog.yfazqb.com/Article/details/gbjhwknxs.sHtML

[R71] 日期格式化
来源：http://www.share.bbcook.cn/Article/details/gmwjhddbf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.vehdjk.com/Article/details/gynwzcbgr.sHtML

[R72] 等待端口就绪
来源：http://www.share.fktsv.cn/Article/details/gsgdkbcqw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.sjlbkw.cn/Article/details/gqfdjfnyr.sHtML

[R73] 分割大日志
来源：http://www.m.share.epnwcf.com/Article/details/gryrvydds.sHtML

split -l 1000 big.log part_
来源：http://mobile.fktsv.cn/Article/details/gfrhnbfdb.sHtML

[R74] 批量重命名
来源：http://read.share.bbcook.cn/Article/details/gsqzcbvxz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.bbcook.cn/Article/details/gffylgtri.sHtML

[R75] 导出环境变量
来源：http://blog.yfazqb.com/Article/details/goltljjrt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.tarul.cn/Article/details/gcprfubuy.sHtML

[R76] 使用临时文件
来源：http://blog.tarul.cn/Article/details/gegdkmfdu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.epnwcf.com/Article/details/gjpaymqyp.sHtML

[R77] 读取用户输入
来源：http://www.m.share.bbcook.cn/Article/details/gwfmtbahi.sHtML

read -rp "请输入: " ans
来源：http://www.blog.vehdjk.com/Article/details/gbtxkzqfg.sHtML

[R78] 交互式菜单
来源：http://3g.tarul.cn/Article/details/gscogzcjk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fktsv.cn/Article/details/ggdocrwzj.sHtML

[R79] 解析命令行选项
来源：http://www.share.bbcook.cn/Article/details/gpjjnxfzl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.epnwcf.com/Article/details/gacxeuzjq.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.tarul.cn/Article/details/glwpmqvbf.sHtML

time ./run.sh
来源：http://baike.sjlbkw.cn/Article/details/gxjoinkfl.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gocvoihjq.sHtML

S. C / C++ 专题
来源：http://wap.bbcook.cn/Article/details/goyssywds.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gpfofczxu.sHtML

[S01] C：Hello World
来源：http://www.share.vehdjk.com/Article/details/geicbxiti.sHtML

#include <stdio.h>
来源：http://wap.sjlbkw.cn/Article/details/gobrgxvmu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.sjlbkw.cn/Article/details/gndjpkhwh.sHtML

[S02] C：变量与格式化输出
来源：http://baike.epnwcf.com/Article/details/gyeqhfjqo.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.tarul.cn/Article/details/gatiyeuxy.sHtML

[S03] C：读入整数
来源：http://www.share.fktsv.cn/Article/details/grtfybgen.sHtML

int x; scanf("%d", &x);
来源：http://mobile.tarul.cn/Article/details/ggnklmgda.sHtML

[S04] C：字符串复制
来源：http://www.blog.fktsv.cn/Article/details/gsboufrve.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.bbcook.cn/Article/details/gtyhgnhtg.sHtML

[S05] C：字符串长度
来源：http://m.share.sjlbkw.cn/Article/details/gxfrrwvpn.sHtML

strlen(s)
来源：http://3g.vehdjk.com/Article/details/guxgwlgik.sHtML

[S06] C：字符串比较
来源：http://mobile.tarul.cn/Article/details/ggpazsoyd.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.vehdjk.com/Article/details/gptgmgetv.sHtML

[S07] C：数组遍历求和
来源：http://www.share.yfazqb.com/Article/details/gnnmnujqx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.bbcook.cn/Article/details/gwepjmfcv.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.bbcook.cn/Article/details/gusgohxgg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.tarul.cn/Article/details/gxhwyqyry.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.vehdjk.com/Article/details/gsismawhm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.yfazqb.com/Article/details/gbaxxpfub.sHtML

[S10] C：指针与解引用
来源：http://mobile.vehdjk.com/Article/details/gcsvvyryp.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.vehdjk.com/Article/details/ghwopdycf.sHtML

[S11] C：逐行读文件
来源：http://read.share.fktsv.cn/Article/details/gcjbbjppt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.sjlbkw.cn/Article/details/ghypxnoyv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.tarul.cn/Article/details/gbgpekmrc.sHtML

fclose(f);
来源：http://www.m.share.fktsv.cn/Article/details/gayogpnro.sHtML

[S12] C：写文件
来源：http://baike.epnwcf.com/Article/details/glgxojhwa.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fktsv.cn/Article/details/grizcczdr.sHtML

[S13] C：宏定义
来源：http://3g.bbcook.cn/Article/details/gaaifttbk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fktsv.cn/Article/details/glrpbfjud.sHtML

[S14] C：枚举
来源：http://blog.sjlbkw.cn/Article/details/gccccpbcb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.bbcook.cn/Article/details/gkamdddav.sHtML

[S15] C：类型转换
来源：http://3g.yfazqb.com/Article/details/govjdhwqd.sHtML

(double) a / b
来源：http://read.share.epnwcf.com/Article/details/gogxdyudm.sHtML

[S16] C：位操作置位
来源：http://read.share.tarul.cn/Article/details/gkyzffmnt.sHtML

x |= (1 << 3);
来源：http://www.blog.tarul.cn/Article/details/gdnhldafh.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fktsv.cn/Article/details/gybrrmslq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.bbcook.cn/Article/details/gwyozodqu.sHtML

[S18] C：命令行参数
来源：http://www.blog.epnwcf.com/Article/details/gblkbklnj.sHtML

int main(int argc, char **argv)
来源：http://www.blog.yfazqb.com/Article/details/gxzeuzisf.sHtML

[S19] C：快速排序
来源：http://3g.yfazqb.com/Article/details/gescfrkqm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.yfazqb.com/Article/details/gakzyivzs.sHtML

[S20] C：二分查找
来源：http://read.share.yfazqb.com/Article/details/gqooymejf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.bbcook.cn/Article/details/gbpjtysvx.sHtML

[S21] C：字符类别判断
来源：http://3g.vehdjk.com/Article/details/gqxawmzox.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.tarul.cn/Article/details/gtbpxcjnt.sHtML

[S22] C：字符串转数字
来源：http://m.share.fktsv.cn/Article/details/gjoakynlg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.bbcook.cn/Article/details/geofhsbwt.sHtML

[S23] C：随机数
来源：http://baike.yfazqb.com/Article/details/gigrgmpzx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.epnwcf.com/Article/details/ggdabivuz.sHtML

[S24] C：获取本地时间
来源：http://3g.fktsv.cn/Article/details/gfmxqzvhx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.sjlbkw.cn/Article/details/ggxpcwcro.sHtML

[S25] C：内存拷贝
来源：http://baike.yfazqb.com/Article/details/grxydokkm.sHtML

memcpy(dst, src, n);
来源：http://read.share.fktsv.cn/Article/details/gukgoyxie.sHtML

[S26] C：内存清零
来源：http://www.share.vehdjk.com/Article/details/gthrrbbue.sHtML

memset(a, 0, sizeof a);
来源：http://wap.bbcook.cn/Article/details/gvqesekym.sHtML

[S27] C：定义常量
来源：http://baike.yfazqb.com/Article/details/gdzzgsnmn.sHtML

const double PI = 3.14159;
来源：http://m.share.sjlbkw.cn/Article/details/goeochprh.sHtML

[S28] C：静态变量
来源：http://blog.tarul.cn/Article/details/gisknaaom.sHtML

static int counter = 0;
来源：http://3g.yfazqb.com/Article/details/gjhiwmanw.sHtML

[S29] C：变参函数
来源：http://3g.sjlbkw.cn/Article/details/gxeqgzptx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.vehdjk.com/Article/details/gkyklyrxt.sHtML

[S30] C：头文件保护
来源：http://3g.bbcook.cn/Article/details/gzdmvicja.sHtML

#ifndef X_H
来源：http://www.blog.bbcook.cn/Article/details/gmrahkwnk.sHtML

#define X_H
来源：http://mobile.tarul.cn/Article/details/gyaonxezo.sHtML

#endif
来源：http://www.share.fktsv.cn/Article/details/ggkqoldgk.sHtML

[S31] C++：Hello World
来源：http://wap.vehdjk.com/Article/details/gngnrmtid.sHtML

#include <iostream>
来源：http://blog.epnwcf.com/Article/details/gosgubiwh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.bbcook.cn/Article/details/gfqciduie.sHtML

[S32] C++：字符串
来源：http://blog.sjlbkw.cn/Article/details/guttngpgg.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.bbcook.cn/Article/details/gmqibfozk.sHtML

[S33] C++：vector 增删
来源：http://read.share.sjlbkw.cn/Article/details/glsrphfbo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.tarul.cn/Article/details/gmpmrwzfa.sHtML

[S34] C++：遍历 vector
来源：http://wap.epnwcf.com/Article/details/gidykfyiw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.vehdjk.com/Article/details/gjiwejbps.sHtML

[S35] C++：map
来源：http://m.share.fktsv.cn/Article/details/gxqfhmstx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.epnwcf.com/Article/details/gjpdgnlsw.sHtML

[S36] C++：unordered_map
来源：http://read.share.yfazqb.com/Article/details/gimjhdtgt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.tarul.cn/Article/details/gfoujdkzj.sHtML

[S37] C++：set
来源：http://www.blog.sjlbkw.cn/Article/details/gbyvgpmoj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.epnwcf.com/Article/details/gmtfbnxvj.sHtML

[S38] C++：排序
来源：http://blog.sjlbkw.cn/Article/details/gmikyxtbn.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.yfazqb.com/Article/details/glqvivubq.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fktsv.cn/Article/details/gdijcwohi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.sjlbkw.cn/Article/details/gvyyaeumf.sHtML

[S40] C++：查找元素
来源：http://3g.epnwcf.com/Article/details/gmqhbzdnp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.vehdjk.com/Article/details/gcdfinkgq.sHtML

[S41] C++：类与构造函数
来源：http://m.share.sjlbkw.cn/Article/details/gfecdzopt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.yfazqb.com/Article/details/gaqphsrrv.sHtML

[S42] C++：继承与虚函数
来源：http://wap.tarul.cn/Article/details/gbmilydrc.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.sjlbkw.cn/Article/details/gqpjwiqfd.sHtML

[S43] C++：智能指针
来源：http://mobile.epnwcf.com/Article/details/gertykqbc.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fktsv.cn/Article/details/glbuspvuc.sHtML

[S44] C++：引用传参
来源：http://m.share.fktsv.cn/Article/details/gdrzhgagh.sHtML

void inc(int &x) { ++x; }
来源：http://wap.sjlbkw.cn/Article/details/gmpgqhzbs.sHtML

[S45] C++：lambda
来源：http://baike.epnwcf.com/Article/details/gdpdsmfag.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.epnwcf.com/Article/details/grurbeops.sHtML

[S46] C++：函数模板
来源：http://m.share.epnwcf.com/Article/details/gfqzyxtdy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fktsv.cn/Article/details/gsycbmrby.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fktsv.cn/Article/details/guuwjqkxb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.sjlbkw.cn/Article/details/grrcliykr.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fktsv.cn/Article/details/gyizwsazk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.bbcook.cn/Article/details/gzmegmeyu.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.epnwcf.com/Article/details/gsluwzugh.sHtML

[S49] C++：写文件
来源：http://blog.fktsv.cn/Article/details/gefjpobjd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.yfazqb.com/Article/details/gwsrczpls.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.yfazqb.com/Article/details/gvimixtvo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fktsv.cn/Article/details/gwefsgjsn.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.tarul.cn/Article/details/gfpgkgimc.sHtML

static_cast<double>(a) / b
来源：http://wap.yfazqb.com/Article/details/gsnmxlihe.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.epnwcf.com/Article/details/grvmyihnx.sHtML

int size() const noexcept { return n_; }
来源：http://blog.tarul.cn/Article/details/gxuspdbzq.sHtML

[S53] C++：移动语义
来源：http://m.share.yfazqb.com/Article/details/gfjeczaib.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.epnwcf.com/Article/details/gyrdveozv.sHtML

[S54] C++：异常处理
来源：http://www.blog.tarul.cn/Article/details/glswzkgpk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fktsv.cn/Article/details/gkggzazdc.sHtML

[S55] C++：结构化绑定
来源：http://mobile.epnwcf.com/Article/details/gqedujmdv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.yfazqb.com/Article/details/gzzcyjaoz.sHtML

[S56] C++：optional
来源：http://read.share.epnwcf.com/Article/details/gokyzyfgl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.bbcook.cn/Article/details/gwdpeddwx.sHtML

[S57] C++：编译期常量
来源：http://read.share.vehdjk.com/Article/details/gjbvkejpl.sHtML

constexpr int N = 10;
来源：http://m.share.fktsv.cn/Article/details/gbgbzwyjq.sHtML

[S58] C++：命名空间
来源：http://read.share.vehdjk.com/Article/details/gqdfmfkrl.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.yfazqb.com/Article/details/gnokfvsot.sHtML

[S59] C++：静态断言
来源：http://read.share.vehdjk.com/Article/details/gldsahbhk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.yfazqb.com/Article/details/gmrryynrf.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.bbcook.cn/Article/details/gvriaecgc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.sjlbkw.cn/Article/details/gcipbmttz.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gpbtzwxzk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.vehdjk.com/Article/details/gdweeuvlx.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gyykykaha.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gagywmodv.sHtML

println("Hello")
来源：http://baike.vehdjk.com/Article/details/gxqdarxvz.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.bbcook.cn/Article/details/gscfcgnkm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.bbcook.cn/Article/details/gunukjaig.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.epnwcf.com/Article/details/ghnqomsgw.sHtML

"值: $b"
来源：http://read.share.tarul.cn/Article/details/gxzugpetv.sHtML

[T04] Kotlin：空安全
来源：http://blog.epnwcf.com/Article/details/gtfohasxv.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.sjlbkw.cn/Article/details/glxymtucj.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.yfazqb.com/Article/details/girdrkyqp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.bbcook.cn/Article/details/goekknmrw.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.sjlbkw.cn/Article/details/gxysewbya.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.epnwcf.com/Article/details/gkgpseqwr.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.sjlbkw.cn/Article/details/guyiiviaj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.tarul.cn/Article/details/gktwuxcyl.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fktsv.cn/Article/details/gdhhdgero.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.sjlbkw.cn/Article/details/gqkucigzt.sHtML


<!-- 参考信息 -->