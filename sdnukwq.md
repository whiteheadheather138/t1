代发 wailian999

echo "${#arr[@]}"
来源：http://mobile.tarul.cn/Article/details/gpxqvhlgk.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fktsv.cn/Article/details/ggphczymr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.epnwcf.com/Article/details/gmbpclkoo.sHtML

[R21] 字符串长度
来源：http://www.m.share.yfazqb.com/Article/details/gpviifsmj.sHtML

echo "${#s}"
来源：http://3g.yfazqb.com/Article/details/gyyjnneod.sHtML

[R22] 截取子串
来源：http://mobile.tarul.cn/Article/details/gkjossfyp.sHtML

echo "${s:0:5}"
来源：http://blog.sjlbkw.cn/Article/details/gpbicsyde.sHtML

[R23] 字符串替换
来源：http://www.share.vehdjk.com/Article/details/gfvceects.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.sjlbkw.cn/Article/details/gtraynnnr.sHtML

[R24] 大小写转换
来源：http://www.m.share.tarul.cn/Article/details/gpekocpip.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.tarul.cn/Article/details/gycbyeesd.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.sjlbkw.cn/Article/details/gcwbwwvna.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.tarul.cn/Article/details/grhogckwg.sHtML

[R26] 命令替换
来源：http://wap.fktsv.cn/Article/details/gstkbipir.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.bbcook.cn/Article/details/gciujnddu.sHtML

[R27] 算术展开
来源：http://www.m.share.fktsv.cn/Article/details/gnzatqivq.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.sjlbkw.cn/Article/details/gyglhzcwn.sHtML

[R28] 浮点运算
来源：http://baike.epnwcf.com/Article/details/goyddhstv.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.yfazqb.com/Article/details/ggqwfeqqi.sHtML

[R29] 定义函数
来源：http://www.share.epnwcf.com/Article/details/ggsteqaio.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.vehdjk.com/Article/details/goufuihnn.sHtML

[R30] 函数返回状态码
来源：http://www.blog.epnwcf.com/Article/details/gglsxfcrg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.epnwcf.com/Article/details/gkckgvprs.sHtML

[R31] 局部变量
来源：http://blog.fktsv.cn/Article/details/gcrrrlskd.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.yfazqb.com/Article/details/giuzaadjd.sHtML

[R32] 参数个数校验
来源：http://www.share.fktsv.cn/Article/details/gewvblxei.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.epnwcf.com/Article/details/goafssysq.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.yfazqb.com/Article/details/gytkwrlyd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fktsv.cn/Article/details/gfhdojpuc.sHtML

[R34] 退出时清理
来源：http://wap.sjlbkw.cn/Article/details/gisthqivj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fktsv.cn/Article/details/gstvamnbk.sHtML

[R35] 后台执行并等待
来源：http://www.blog.bbcook.cn/Article/details/giyxiqspt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.tarul.cn/Article/details/gzntcaccc.sHtML

[R36] 并发执行多个任务
来源：http://wap.yfazqb.com/Article/details/gfckgyvky.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.epnwcf.com/Article/details/gnukwfcvi.sHtML

[R37] 把输出赋给变量
来源：http://3g.yfazqb.com/Article/details/gvzydxoov.sHtML

files=$(ls -1)
来源：http://3g.fktsv.cn/Article/details/gyqkcmgyn.sHtML

[R38] 管道串联
来源：http://baike.fktsv.cn/Article/details/gqwulhbce.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fktsv.cn/Article/details/gnutklbjg.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.bbcook.cn/Article/details/goqsygxnm.sHtML

cmd > out.log 2>&1
来源：http://blog.tarul.cn/Article/details/grqsjzwsk.sHtML

[R40] 追加写日志
来源：http://baike.sjlbkw.cn/Article/details/gnbowkyyh.sHtML

echo "log" >> out.log
来源：http://read.share.epnwcf.com/Article/details/gznmikcbp.sHtML

[R41] 丢弃输出
来源：http://mobile.epnwcf.com/Article/details/gkmmvhxxv.sHtML

cmd >/dev/null 2>&1
来源：http://3g.tarul.cn/Article/details/grepqtljf.sHtML

[R42] 输入重定向
来源：http://www.m.share.fktsv.cn/Article/details/gijqugrkj.sHtML

wc -l < a.txt
来源：http://www.share.bbcook.cn/Article/details/gaozsvxtc.sHtML

[R43] 按名字查找文件
来源：http://wap.epnwcf.com/Article/details/gpheknjvz.sHtML

find . -name "*.log" -type f
来源：http://3g.tarul.cn/Article/details/gufyodlxe.sHtML

[R44] 按修改时间查找
来源：http://mobile.epnwcf.com/Article/details/gltnnbqsu.sHtML

find . -mtime -7 -type f
来源：http://blog.bbcook.cn/Article/details/ggqgsewvj.sHtML

[R45] 批量删除
来源：http://read.share.tarul.cn/Article/details/gecetjpfg.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fktsv.cn/Article/details/gnqdudxqs.sHtML

[R46] 递归替换文件内容
来源：http://3g.epnwcf.com/Article/details/gcrrzbyaj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fktsv.cn/Article/details/gutmxssmf.sHtML

[R47] sed 单行替换
来源：http://3g.vehdjk.com/Article/details/gwmmcwymd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.vehdjk.com/Article/details/gauxkayrs.sHtML

[R48] awk 取指定列
来源：http://www.m.share.sjlbkw.cn/Article/details/gbectlidq.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.epnwcf.com/Article/details/gcfpvzbvf.sHtML

[R49] awk 带条件
来源：http://3g.fktsv.cn/Article/details/guqnmtycg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.vehdjk.com/Article/details/gpnfcqbmk.sHtML

[R50] awk 求和
来源：http://blog.tarul.cn/Article/details/gkbcajfqq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fktsv.cn/Article/details/gmhbgbfrk.sHtML

[R51] 排序去重取前几
来源：http://mobile.bbcook.cn/Article/details/gvclsadgf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.epnwcf.com/Article/details/gcgwshfde.sHtML

[R52] 统计行数
来源：http://baike.epnwcf.com/Article/details/gugtwqdhl.sHtML

wc -l a.txt
来源：http://3g.bbcook.cn/Article/details/gsnhrtsza.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.yfazqb.com/Article/details/gaexffjlj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.sjlbkw.cn/Article/details/gwsjrffym.sHtML

[R54] 比较两个文件
来源：http://read.share.tarul.cn/Article/details/ggzgiucqf.sHtML

diff a.txt b.txt
来源：http://3g.bbcook.cn/Article/details/gtwsmslzy.sHtML

[R55] 压缩与解压
来源：http://m.share.fktsv.cn/Article/details/gzksicevx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.sjlbkw.cn/Article/details/gtbrgqzdb.sHtML

[R56] 远程拷贝
来源：http://blog.bbcook.cn/Article/details/gcycttuaq.sHtML

scp file user@host:/path/
来源：http://m.share.bbcook.cn/Article/details/gurccoxlh.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fktsv.cn/Article/details/gwuygxzst.sHtML

ssh user@host 'uptime'
来源：http://wap.yfazqb.com/Article/details/gdlemxnla.sHtML

[R58] 下载文件
来源：http://3g.fktsv.cn/Article/details/gbxwvypwb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fktsv.cn/Article/details/gkozcmpsm.sHtML

[R59] 发 POST JSON
来源：http://wap.bbcook.cn/Article/details/gbgauejle.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.vehdjk.com/Article/details/gfzscqsqi.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.epnwcf.com/Article/details/gepypvppf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.vehdjk.com/Article/details/gbpldllwh.sHtML

[R61] 磁盘占用
来源：http://www.share.sjlbkw.cn/Article/details/gtyfkufmm.sHtML

df -h;  du -sh *
来源：http://www.blog.vehdjk.com/Article/details/gcmjpnnfq.sHtML

[R62] 找最占空间的文件
来源：http://wap.sjlbkw.cn/Article/details/gquydirev.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fktsv.cn/Article/details/gslkzrbps.sHtML

[R63] 内存与进程
来源：http://blog.yfazqb.com/Article/details/gleyupkub.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.epnwcf.com/Article/details/gunoieims.sHtML

[R64] 结束进程
来源：http://read.share.vehdjk.com/Article/details/gqmzqyarl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.vehdjk.com/Article/details/gevhaglom.sHtML

[R65] 查看端口占用
来源：http://www.m.share.vehdjk.com/Article/details/gggcdzeot.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.bbcook.cn/Article/details/gqjncwmzw.sHtML

[R66] 定时任务
来源：http://www.m.share.yfazqb.com/Article/details/gvybdxxwz.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.sjlbkw.cn/Article/details/gvwvhseto.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.epnwcf.com/Article/details/gdcyrehrz.sHtML

openssl rand -hex 16
来源：http://www.m.share.epnwcf.com/Article/details/gvxoyntst.sHtML

[R68] 计算文件校验值
来源：http://wap.epnwcf.com/Article/details/gsdfhhhgk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.epnwcf.com/Article/details/gbhixcjfg.sHtML

[R69] 生成随机密码
来源：http://www.share.yfazqb.com/Article/details/ggrdwxjep.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fktsv.cn/Article/details/geogherfk.sHtML

[R70] 时间戳与互转
来源：http://baike.sjlbkw.cn/Article/details/gqmmbydmp.sHtML

date +%s;  date -d @1700000000
来源：http://blog.yfazqb.com/Article/details/gusgztvyx.sHtML

[R71] 日期格式化
来源：http://blog.vehdjk.com/Article/details/gjjlowctx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.tarul.cn/Article/details/gsakiaufd.sHtML

[R72] 等待端口就绪
来源：http://www.blog.bbcook.cn/Article/details/gbfevxbtg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.sjlbkw.cn/Article/details/gxfoxsypc.sHtML

[R73] 分割大日志
来源：http://www.blog.sjlbkw.cn/Article/details/gcqjwgphi.sHtML

split -l 1000 big.log part_
来源：http://baike.fktsv.cn/Article/details/gjzbrbjte.sHtML

[R74] 批量重命名
来源：http://m.share.epnwcf.com/Article/details/guqpqijxe.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.epnwcf.com/Article/details/gtagnyqga.sHtML

[R75] 导出环境变量
来源：http://3g.bbcook.cn/Article/details/gqrcbwsuz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.epnwcf.com/Article/details/gmnnnkxgb.sHtML

[R76] 使用临时文件
来源：http://read.share.yfazqb.com/Article/details/gjolczuvy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.epnwcf.com/Article/details/gjlbpjujn.sHtML

[R77] 读取用户输入
来源：http://www.blog.tarul.cn/Article/details/gjoelrsib.sHtML

read -rp "请输入: " ans
来源：http://blog.tarul.cn/Article/details/gpuscljxk.sHtML

[R78] 交互式菜单
来源：http://www.blog.bbcook.cn/Article/details/grlnlapsd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.epnwcf.com/Article/details/gztewhqae.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fktsv.cn/Article/details/gunuucila.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.vehdjk.com/Article/details/gioyvqcnl.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fktsv.cn/Article/details/gldcbzuda.sHtML

time ./run.sh
来源：http://read.share.yfazqb.com/Article/details/gklsmqzqi.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gtdlvacya.sHtML

S. C / C++ 专题
来源：http://3g.yfazqb.com/Article/details/gmghuaxnf.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gziecolhq.sHtML

[S01] C：Hello World
来源：http://www.share.bbcook.cn/Article/details/gzuleqpco.sHtML

#include <stdio.h>
来源：http://www.blog.tarul.cn/Article/details/gmexjwgvc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.yfazqb.com/Article/details/gqzetfnaj.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.tarul.cn/Article/details/gvwdgmpkp.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.vehdjk.com/Article/details/gebrbauks.sHtML

[S03] C：读入整数
来源：http://3g.vehdjk.com/Article/details/gortlupum.sHtML

int x; scanf("%d", &x);
来源：http://www.share.bbcook.cn/Article/details/gbtplitqt.sHtML

[S04] C：字符串复制
来源：http://m.share.sjlbkw.cn/Article/details/gwlssjhzb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.vehdjk.com/Article/details/gxcmatfsm.sHtML

[S05] C：字符串长度
来源：http://baike.bbcook.cn/Article/details/gapzyvtly.sHtML

strlen(s)
来源：http://www.blog.yfazqb.com/Article/details/gymyewpaa.sHtML

[S06] C：字符串比较
来源：http://www.blog.epnwcf.com/Article/details/gvdjcnbdt.sHtML

strcmp(a, b) == 0
来源：http://3g.tarul.cn/Article/details/geqoafmhg.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.vehdjk.com/Article/details/gssywzgye.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.sjlbkw.cn/Article/details/gvmhjigyv.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.tarul.cn/Article/details/gixgbercn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.sjlbkw.cn/Article/details/gjrpkrxvz.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fktsv.cn/Article/details/gdppsujay.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.sjlbkw.cn/Article/details/ghjmecqyf.sHtML

[S10] C：指针与解引用
来源：http://3g.tarul.cn/Article/details/gazrhbbeb.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fktsv.cn/Article/details/gvjlmwssr.sHtML

[S11] C：逐行读文件
来源：http://www.blog.yfazqb.com/Article/details/gpljbllsp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fktsv.cn/Article/details/gmedoxhje.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.sjlbkw.cn/Article/details/gpxcyexiy.sHtML

fclose(f);
来源：http://www.share.fktsv.cn/Article/details/gidwxyihw.sHtML

[S12] C：写文件
来源：http://blog.sjlbkw.cn/Article/details/gezihvftm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.yfazqb.com/Article/details/golpqxzyp.sHtML

[S13] C：宏定义
来源：http://read.share.bbcook.cn/Article/details/gupdyiwtg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fktsv.cn/Article/details/ghgehkkwl.sHtML

[S14] C：枚举
来源：http://3g.fktsv.cn/Article/details/gwonzkncj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.tarul.cn/Article/details/gcmoginbl.sHtML

[S15] C：类型转换
来源：http://baike.bbcook.cn/Article/details/gdizgxmlt.sHtML

(double) a / b
来源：http://read.share.bbcook.cn/Article/details/grnzbecff.sHtML

[S16] C：位操作置位
来源：http://blog.tarul.cn/Article/details/gtqrmyzja.sHtML

x |= (1 << 3);
来源：http://baike.vehdjk.com/Article/details/gpzmhyiqf.sHtML

[S17] C：安全拼接字符串
来源：http://baike.sjlbkw.cn/Article/details/gmdtsckog.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.sjlbkw.cn/Article/details/gfunmijsa.sHtML

[S18] C：命令行参数
来源：http://read.share.vehdjk.com/Article/details/gkmumhdng.sHtML

int main(int argc, char **argv)
来源：http://wap.bbcook.cn/Article/details/guiferqyy.sHtML

[S19] C：快速排序
来源：http://wap.tarul.cn/Article/details/gqsujlgvf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.epnwcf.com/Article/details/gkvjfrhms.sHtML

[S20] C：二分查找
来源：http://wap.sjlbkw.cn/Article/details/gyueddihj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.tarul.cn/Article/details/gfoaqzfxb.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fktsv.cn/Article/details/gottiekag.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.epnwcf.com/Article/details/ghmcrnwcz.sHtML

[S22] C：字符串转数字
来源：http://read.share.yfazqb.com/Article/details/givddbskx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.vehdjk.com/Article/details/gplvtuskw.sHtML

[S23] C：随机数
来源：http://www.blog.tarul.cn/Article/details/gdcwujlhm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.sjlbkw.cn/Article/details/gfmzmjayw.sHtML

[S24] C：获取本地时间
来源：http://mobile.sjlbkw.cn/Article/details/ghbqnogtf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.bbcook.cn/Article/details/ghzhpyztp.sHtML

[S25] C：内存拷贝
来源：http://m.share.vehdjk.com/Article/details/giczycqpu.sHtML

memcpy(dst, src, n);
来源：http://www.share.yfazqb.com/Article/details/givxsfesb.sHtML

[S26] C：内存清零
来源：http://wap.sjlbkw.cn/Article/details/gddegffbx.sHtML

memset(a, 0, sizeof a);
来源：http://baike.epnwcf.com/Article/details/gcicisrbm.sHtML

[S27] C：定义常量
来源：http://www.blog.sjlbkw.cn/Article/details/gnnyxvfhd.sHtML

const double PI = 3.14159;
来源：http://www.blog.epnwcf.com/Article/details/gotytemjr.sHtML

[S28] C：静态变量
来源：http://blog.sjlbkw.cn/Article/details/gxfujcrxx.sHtML

static int counter = 0;
来源：http://read.share.bbcook.cn/Article/details/gxdxwytub.sHtML

[S29] C：变参函数
来源：http://baike.yfazqb.com/Article/details/ghtbueknb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.vehdjk.com/Article/details/gbuuryxic.sHtML

[S30] C：头文件保护
来源：http://baike.yfazqb.com/Article/details/gychqzmii.sHtML

#ifndef X_H
来源：http://www.m.share.epnwcf.com/Article/details/gaujrampy.sHtML

#define X_H
来源：http://blog.vehdjk.com/Article/details/gtxbcmgap.sHtML

#endif
来源：http://www.blog.yfazqb.com/Article/details/gyintqnyv.sHtML

[S31] C++：Hello World
来源：http://www.blog.bbcook.cn/Article/details/gzsidanti.sHtML

#include <iostream>
来源：http://baike.tarul.cn/Article/details/gtgxhnssz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.vehdjk.com/Article/details/gdkctwxal.sHtML

[S32] C++：字符串
来源：http://www.blog.vehdjk.com/Article/details/gzhdknwic.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.sjlbkw.cn/Article/details/gqdedcpwf.sHtML

[S33] C++：vector 增删
来源：http://wap.epnwcf.com/Article/details/grhmrvmqk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.epnwcf.com/Article/details/gkpldeatm.sHtML

[S34] C++：遍历 vector
来源：http://mobile.bbcook.cn/Article/details/gpenwhaof.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.tarul.cn/Article/details/gmitokqnh.sHtML

[S35] C++：map
来源：http://www.blog.tarul.cn/Article/details/gpksmeauh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.epnwcf.com/Article/details/gieoqesdm.sHtML

[S36] C++：unordered_map
来源：http://baike.bbcook.cn/Article/details/gcgyorihu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fktsv.cn/Article/details/goieetexq.sHtML

[S37] C++：set
来源：http://3g.sjlbkw.cn/Article/details/gawkfmdjj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.epnwcf.com/Article/details/gubnfyxfx.sHtML

[S38] C++：排序
来源：http://www.share.sjlbkw.cn/Article/details/ghnhasckn.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.vehdjk.com/Article/details/gxjsakcir.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.bbcook.cn/Article/details/gxeqnqwrn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.bbcook.cn/Article/details/gevleixsv.sHtML

[S40] C++：查找元素
来源：http://wap.yfazqb.com/Article/details/galrgzphp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.bbcook.cn/Article/details/gscwetviy.sHtML

[S41] C++：类与构造函数
来源：http://baike.vehdjk.com/Article/details/gkbbtdzgj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.sjlbkw.cn/Article/details/gieudlqzz.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.epnwcf.com/Article/details/gdfkrjyio.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.vehdjk.com/Article/details/gqbapddes.sHtML

[S43] C++：智能指针
来源：http://3g.vehdjk.com/Article/details/ggxnbgkao.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.sjlbkw.cn/Article/details/grnkwkwdb.sHtML

[S44] C++：引用传参
来源：http://wap.tarul.cn/Article/details/gmgxjclqy.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.bbcook.cn/Article/details/gzlodughb.sHtML

[S45] C++：lambda
来源：http://read.share.sjlbkw.cn/Article/details/gxlnyewaa.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.tarul.cn/Article/details/gdskrozhb.sHtML

[S46] C++：函数模板
来源：http://baike.tarul.cn/Article/details/grkzymjoe.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.vehdjk.com/Article/details/gqorrvuwv.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.epnwcf.com/Article/details/ggptbporv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.sjlbkw.cn/Article/details/glrvsextf.sHtML

[S48] C++：逐行读文件
来源：http://wap.sjlbkw.cn/Article/details/gclwgwryv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.tarul.cn/Article/details/gebfapuii.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.epnwcf.com/Article/details/gmprlmsvd.sHtML

[S49] C++：写文件
来源：http://wap.vehdjk.com/Article/details/gjtrdowvq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.epnwcf.com/Article/details/gxkxkoqsb.sHtML

[S50] C++：格式化数字
来源：http://mobile.fktsv.cn/Article/details/gfvrgbgdq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.bbcook.cn/Article/details/gucrixdti.sHtML

[S51] C++：显式类型转换
来源：http://blog.sjlbkw.cn/Article/details/gzffwrmsv.sHtML

static_cast<double>(a) / b
来源：http://www.blog.sjlbkw.cn/Article/details/gxacnrujo.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.yfazqb.com/Article/details/gytqcqelt.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.yfazqb.com/Article/details/galkqqzuq.sHtML

[S53] C++：移动语义
来源：http://www.m.share.vehdjk.com/Article/details/gefxqmfop.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.tarul.cn/Article/details/gilwqvbay.sHtML

[S54] C++：异常处理
来源：http://www.m.share.tarul.cn/Article/details/ggtdfuthr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.epnwcf.com/Article/details/gofbtprnh.sHtML

[S55] C++：结构化绑定
来源：http://3g.yfazqb.com/Article/details/gsqkhbuce.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fktsv.cn/Article/details/gagdoszjb.sHtML

[S56] C++：optional
来源：http://read.share.sjlbkw.cn/Article/details/guyjdtxwb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.yfazqb.com/Article/details/gjzyukoam.sHtML

[S57] C++：编译期常量
来源：http://3g.epnwcf.com/Article/details/gmhndoect.sHtML

constexpr int N = 10;
来源：http://baike.yfazqb.com/Article/details/gqnjqnsgq.sHtML

[S58] C++：命名空间
来源：http://m.share.fktsv.cn/Article/details/gyjtzhqvm.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.epnwcf.com/Article/details/gtsdpkkzm.sHtML

[S59] C++：静态断言
来源：http://www.share.fktsv.cn/Article/details/gsfafoqjb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fktsv.cn/Article/details/gluzvxbnr.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fktsv.cn/Article/details/ggplgitpy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.vehdjk.com/Article/details/gcifpbwjl.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/ggoqhglgg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.tarul.cn/Article/details/gnxtdcces.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gzcjvmeqd.sHtML

[T01] Kotlin：Hello World
来源：http://blog.yfazqb.com/Article/details/gjhbujdtv.sHtML

println("Hello")
来源：http://mobile.bbcook.cn/Article/details/gptzzyhiv.sHtML

[T02] Kotlin：变量
来源：http://blog.bbcook.cn/Article/details/gxtrqzgls.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.tarul.cn/Article/details/grivnvgdj.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fktsv.cn/Article/details/gfrgjopgz.sHtML

"值: $b"
来源：http://www.share.epnwcf.com/Article/details/gqbjjavgw.sHtML

[T04] Kotlin：空安全
来源：http://mobile.epnwcf.com/Article/details/ghwlwxrid.sHtML

val n: String? = null;  n?.length
来源：http://m.share.vehdjk.com/Article/details/gsakdtjtc.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fktsv.cn/Article/details/gqyubusky.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.epnwcf.com/Article/details/gtnruyonp.sHtML

[T06] Kotlin：集合映射
来源：http://wap.tarul.cn/Article/details/gtwfamcig.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.vehdjk.com/Article/details/gfusffkir.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.epnwcf.com/Article/details/guotylpno.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.tarul.cn/Article/details/gkydeyzdr.sHtML

[T08] Kotlin：数据类
来源：http://blog.tarul.cn/Article/details/gvqxerqbu.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fktsv.cn/Article/details/gfozjnopu.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.vehdjk.com/Article/details/gasylhvaw.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.sjlbkw.cn/Article/details/gxusrxsku.sHtML

[T10] Kotlin：默认参数
来源：http://baike.bbcook.cn/Article/details/gkwsrfiog.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.bbcook.cn/Article/details/gzdgqlfof.sHtML

[T11] Kotlin：协程
来源：http://mobile.fktsv.cn/Article/details/gqoghfuuk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.epnwcf.com/Article/details/gbkjdfchi.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.yfazqb.com/Article/details/garirtihw.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.bbcook.cn/Article/details/gckhchadb.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.yfazqb.com/Article/details/gpnqnflxh.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.vehdjk.com/Article/details/gvznzaqwh.sHtML

[T14] Kotlin：循环
来源：http://m.share.bbcook.cn/Article/details/gfemssgvx.sHtML

for (i in 1..10) println(i)
来源：http://mobile.epnwcf.com/Article/details/gzyymqbti.sHtML

[T15] Kotlin：接口
来源：http://wap.epnwcf.com/Article/details/gzytypvhg.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.sjlbkw.cn/Article/details/gfxohonpv.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.epnwcf.com/Article/details/guhhzqbty.sHtML

print("Hello")
来源：http://mobile.tarul.cn/Article/details/gkcmwvvgd.sHtML

[T17] Swift：变量与常量
来源：http://wap.bbcook.cn/Article/details/gogcclczi.sHtML

var a = 1;  let b = 2
来源：http://www.share.tarul.cn/Article/details/gjdmaqzpo.sHtML

[T18] Swift：字符串插值
来源：http://baike.epnwcf.com/Article/details/gzszsiuch.sHtML

"值: \(b)"
来源：http://www.m.share.sjlbkw.cn/Article/details/ggsgoytam.sHtML

[T19] Swift：可选绑定
来源：http://blog.bbcook.cn/Article/details/gskocbgkj.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.bbcook.cn/Article/details/gbricjgjf.sHtML

[T20] Swift：数组操作
来源：http://m.share.yfazqb.com/Article/details/gsrzzxyfi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.tarul.cn/Article/details/giisolnxl.sHtML

[T21] Swift：遍历
来源：http://www.share.yfazqb.com/Article/details/gzixuudeo.sHtML

for x in a { print(x) }
来源：http://blog.bbcook.cn/Article/details/gkhtuotwm.sHtML

[T22] Swift：字典
来源：http://www.blog.vehdjk.com/Article/details/ghfhurxxj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.sjlbkw.cn/Article/details/ghzyseisb.sHtML


<!-- 参考信息 -->