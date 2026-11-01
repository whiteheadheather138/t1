代发 wailian999

echo "${#s}"
来源：http://blog.epnwcf.com/Article/details/ggnnwhvev.sHtML

[R22] 截取子串
来源：http://mobile.tarul.cn/Article/details/gpcnnxijj.sHtML

echo "${s:0:5}"
来源：http://www.blog.yfazqb.com/Article/details/guejtdbtb.sHtML

[R23] 字符串替换
来源：http://www.blog.tarul.cn/Article/details/gafykgdqq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.epnwcf.com/Article/details/gctxaxtmz.sHtML

[R24] 大小写转换
来源：http://blog.epnwcf.com/Article/details/gnbzsnezr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.yfazqb.com/Article/details/gkjloacxy.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.epnwcf.com/Article/details/gdrwqgmim.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.tarul.cn/Article/details/gnqjxbopo.sHtML

[R26] 命令替换
来源：http://wap.yfazqb.com/Article/details/gqbzdncyc.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.tarul.cn/Article/details/gtvfqbusq.sHtML

[R27] 算术展开
来源：http://m.share.yfazqb.com/Article/details/glwilpigm.sHtML

echo $((1 + 2 * 3))
来源：http://wap.bbcook.cn/Article/details/glhcxumge.sHtML

[R28] 浮点运算
来源：http://read.share.epnwcf.com/Article/details/gfevhwvod.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.bbcook.cn/Article/details/gxryufaer.sHtML

[R29] 定义函数
来源：http://mobile.fktsv.cn/Article/details/gwmamzput.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.tarul.cn/Article/details/gvliepnem.sHtML

[R30] 函数返回状态码
来源：http://3g.tarul.cn/Article/details/glimponzy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fktsv.cn/Article/details/gzvrqddpt.sHtML

[R31] 局部变量
来源：http://wap.vehdjk.com/Article/details/gqrpoelkz.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.vehdjk.com/Article/details/gwowfzulm.sHtML

[R32] 参数个数校验
来源：http://m.share.vehdjk.com/Article/details/girttyhuy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.tarul.cn/Article/details/gsntbivrx.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.bbcook.cn/Article/details/gijrwxbnr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.epnwcf.com/Article/details/gfvezjprd.sHtML

[R34] 退出时清理
来源：http://www.share.epnwcf.com/Article/details/gyrtqbwup.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.yfazqb.com/Article/details/ggwojtups.sHtML

[R35] 后台执行并等待
来源：http://www.share.sjlbkw.cn/Article/details/grckqgnel.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.tarul.cn/Article/details/gzmelrxov.sHtML

[R36] 并发执行多个任务
来源：http://blog.tarul.cn/Article/details/gtywffqfd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fktsv.cn/Article/details/gvgewzgms.sHtML

[R37] 把输出赋给变量
来源：http://wap.fktsv.cn/Article/details/gpatbqduq.sHtML

files=$(ls -1)
来源：http://baike.vehdjk.com/Article/details/gulwdwinu.sHtML

[R38] 管道串联
来源：http://www.share.sjlbkw.cn/Article/details/gnpgwkgzb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.tarul.cn/Article/details/gqhnxgszy.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.bbcook.cn/Article/details/gqraabppm.sHtML

cmd > out.log 2>&1
来源：http://mobile.vehdjk.com/Article/details/grtbidybd.sHtML

[R40] 追加写日志
来源：http://mobile.yfazqb.com/Article/details/gcfwygyft.sHtML

echo "log" >> out.log
来源：http://m.share.bbcook.cn/Article/details/gtjvxbopy.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fktsv.cn/Article/details/gnsfpzajq.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fktsv.cn/Article/details/gjrbrlhyo.sHtML

[R42] 输入重定向
来源：http://3g.yfazqb.com/Article/details/gjpeeptxz.sHtML

wc -l < a.txt
来源：http://www.share.bbcook.cn/Article/details/gsdgloxcn.sHtML

[R43] 按名字查找文件
来源：http://read.share.vehdjk.com/Article/details/gfpvebgem.sHtML

find . -name "*.log" -type f
来源：http://www.share.sjlbkw.cn/Article/details/gqfgugwsk.sHtML

[R44] 按修改时间查找
来源：http://www.blog.bbcook.cn/Article/details/gmsmswbyu.sHtML

find . -mtime -7 -type f
来源：http://blog.sjlbkw.cn/Article/details/gclhzwaal.sHtML

[R45] 批量删除
来源：http://blog.fktsv.cn/Article/details/gtfcxmezx.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.epnwcf.com/Article/details/gjmgsqget.sHtML

[R46] 递归替换文件内容
来源：http://baike.sjlbkw.cn/Article/details/grffzvjlt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fktsv.cn/Article/details/gulywcoke.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fktsv.cn/Article/details/goyorjmsh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gxwokcqdx.sHtML

[R48] awk 取指定列
来源：http://www.m.share.yfazqb.com/Article/details/gozvkjuwp.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.bbcook.cn/Article/details/gfgtwijml.sHtML

[R49] awk 带条件
来源：http://mobile.epnwcf.com/Article/details/gyryzvumy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.bbcook.cn/Article/details/geyujlkxv.sHtML

[R50] awk 求和
来源：http://m.share.vehdjk.com/Article/details/ggolfpjnt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.epnwcf.com/Article/details/gdmpejjyu.sHtML

[R51] 排序去重取前几
来源：http://3g.epnwcf.com/Article/details/gvilbmdlu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.bbcook.cn/Article/details/gtlkpwgwe.sHtML

[R52] 统计行数
来源：http://mobile.yfazqb.com/Article/details/gdllwrfpu.sHtML

wc -l a.txt
来源：http://read.share.fktsv.cn/Article/details/ghozxdjbg.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.epnwcf.com/Article/details/gwqawlfpk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.epnwcf.com/Article/details/gpolqwedd.sHtML

[R54] 比较两个文件
来源：http://www.blog.vehdjk.com/Article/details/gcwgidohj.sHtML

diff a.txt b.txt
来源：http://wap.tarul.cn/Article/details/glgvfsuir.sHtML

[R55] 压缩与解压
来源：http://blog.yfazqb.com/Article/details/guxyqhzux.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.tarul.cn/Article/details/gsrcgkzku.sHtML

[R56] 远程拷贝
来源：http://m.share.yfazqb.com/Article/details/gsukcmilg.sHtML

scp file user@host:/path/
来源：http://baike.epnwcf.com/Article/details/gxswjhwdk.sHtML

[R57] 远程执行命令
来源：http://www.m.share.bbcook.cn/Article/details/gxgtjiquz.sHtML

ssh user@host 'uptime'
来源：http://blog.epnwcf.com/Article/details/gdfgrtlhc.sHtML

[R58] 下载文件
来源：http://www.m.share.bbcook.cn/Article/details/gpdijmsaf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.yfazqb.com/Article/details/gdvfwqzpr.sHtML

[R59] 发 POST JSON
来源：http://3g.tarul.cn/Article/details/goacftsms.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.bbcook.cn/Article/details/gcyidtsls.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.bbcook.cn/Article/details/gujjsuxax.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.yfazqb.com/Article/details/ggrieelci.sHtML

[R61] 磁盘占用
来源：http://blog.bbcook.cn/Article/details/gwfqcctev.sHtML

df -h;  du -sh *
来源：http://blog.epnwcf.com/Article/details/gfxegkmvc.sHtML

[R62] 找最占空间的文件
来源：http://mobile.yfazqb.com/Article/details/gajvsszhp.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.epnwcf.com/Article/details/gpzwklrbq.sHtML

[R63] 内存与进程
来源：http://3g.tarul.cn/Article/details/gataeraop.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.yfazqb.com/Article/details/gkjntejjh.sHtML

[R64] 结束进程
来源：http://wap.fktsv.cn/Article/details/gxtojkthh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.vehdjk.com/Article/details/gzunngfxt.sHtML

[R65] 查看端口占用
来源：http://m.share.fktsv.cn/Article/details/grzsamqsz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.vehdjk.com/Article/details/gsdqntwuw.sHtML

[R66] 定时任务
来源：http://m.share.sjlbkw.cn/Article/details/gfmljvzah.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.yfazqb.com/Article/details/gnscrodmx.sHtML

[R67] 生成随机十六进制串
来源：http://3g.tarul.cn/Article/details/gaopmbbkd.sHtML

openssl rand -hex 16
来源：http://baike.epnwcf.com/Article/details/gtotprloe.sHtML

[R68] 计算文件校验值
来源：http://www.share.yfazqb.com/Article/details/gygqtnpmh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fktsv.cn/Article/details/gsimoqyre.sHtML

[R69] 生成随机密码
来源：http://www.share.epnwcf.com/Article/details/gkcykizot.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.epnwcf.com/Article/details/gocggqxri.sHtML

[R70] 时间戳与互转
来源：http://read.share.fktsv.cn/Article/details/grbjtopor.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.yfazqb.com/Article/details/gnbaqonjo.sHtML

[R71] 日期格式化
来源：http://3g.tarul.cn/Article/details/gqfbhjbkf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.bbcook.cn/Article/details/gkyysdvjw.sHtML

[R72] 等待端口就绪
来源：http://www.share.fktsv.cn/Article/details/gvvkhxfsg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.yfazqb.com/Article/details/gthzzkmcv.sHtML

[R73] 分割大日志
来源：http://m.share.yfazqb.com/Article/details/gmhlksxyf.sHtML

split -l 1000 big.log part_
来源：http://3g.fktsv.cn/Article/details/gzbvhxrjn.sHtML

[R74] 批量重命名
来源：http://blog.fktsv.cn/Article/details/gmfduhjpt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.epnwcf.com/Article/details/gatjtyiva.sHtML

[R75] 导出环境变量
来源：http://mobile.bbcook.cn/Article/details/gybggprgg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fktsv.cn/Article/details/gepjqaxkq.sHtML

[R76] 使用临时文件
来源：http://mobile.yfazqb.com/Article/details/gepjtpwwh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.tarul.cn/Article/details/gxbylevun.sHtML

[R77] 读取用户输入
来源：http://www.m.share.tarul.cn/Article/details/gblgncxfr.sHtML

read -rp "请输入: " ans
来源：http://www.share.tarul.cn/Article/details/gjtjovcin.sHtML

[R78] 交互式菜单
来源：http://www.share.tarul.cn/Article/details/gtowgpnki.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.yfazqb.com/Article/details/gehcfxwhe.sHtML

[R79] 解析命令行选项
来源：http://wap.fktsv.cn/Article/details/gwgtsqppq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.epnwcf.com/Article/details/gafotpncx.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.sjlbkw.cn/Article/details/gbybhjyeh.sHtML

time ./run.sh
来源：http://m.share.vehdjk.com/Article/details/gokbyjdtu.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/ggnrjkedj.sHtML

S. C / C++ 专题
来源：http://m.share.yfazqb.com/Article/details/gttzsknhl.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gilevrjqy.sHtML

[S01] C：Hello World
来源：http://www.share.fktsv.cn/Article/details/gchukoqmi.sHtML

#include <stdio.h>
来源：http://baike.bbcook.cn/Article/details/gwwkxqbgn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.tarul.cn/Article/details/gqlayvemh.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.epnwcf.com/Article/details/ghsfqidzt.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.bbcook.cn/Article/details/gjskfyzrq.sHtML

[S03] C：读入整数
来源：http://baike.epnwcf.com/Article/details/godlumjme.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fktsv.cn/Article/details/gdcyfredb.sHtML

[S04] C：字符串复制
来源：http://read.share.vehdjk.com/Article/details/gyuzdzlzp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.epnwcf.com/Article/details/gedlwzfgu.sHtML

[S05] C：字符串长度
来源：http://m.share.sjlbkw.cn/Article/details/giuqdgphu.sHtML

strlen(s)
来源：http://m.share.yfazqb.com/Article/details/gdxoegvjo.sHtML

[S06] C：字符串比较
来源：http://www.share.bbcook.cn/Article/details/gcsumaxey.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fktsv.cn/Article/details/gnyqkeoyi.sHtML

[S07] C：数组遍历求和
来源：http://baike.yfazqb.com/Article/details/gcnecntnu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.bbcook.cn/Article/details/gpnlonfsl.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.epnwcf.com/Article/details/gsafpmidz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.tarul.cn/Article/details/guapfwfep.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.sjlbkw.cn/Article/details/gertkbztm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.tarul.cn/Article/details/gfyeqlxps.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.bbcook.cn/Article/details/gzfyhdumz.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.sjlbkw.cn/Article/details/gkpaicire.sHtML

[S11] C：逐行读文件
来源：http://wap.yfazqb.com/Article/details/gznbzzgvo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.vehdjk.com/Article/details/gognetmyw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.bbcook.cn/Article/details/gichxslus.sHtML

fclose(f);
来源：http://m.share.fktsv.cn/Article/details/gfeirqebj.sHtML

[S12] C：写文件
来源：http://read.share.fktsv.cn/Article/details/gcdufhfkf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.tarul.cn/Article/details/gszhguufa.sHtML

[S13] C：宏定义
来源：http://m.share.vehdjk.com/Article/details/gqfxhsejv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fktsv.cn/Article/details/gtsgwquhh.sHtML

[S14] C：枚举
来源：http://www.share.tarul.cn/Article/details/ghtgsxvxd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.vehdjk.com/Article/details/gxndxkppc.sHtML

[S15] C：类型转换
来源：http://3g.fktsv.cn/Article/details/grivnamkf.sHtML

(double) a / b
来源：http://3g.vehdjk.com/Article/details/gdabhyedv.sHtML

[S16] C：位操作置位
来源：http://read.share.fktsv.cn/Article/details/gadvzkptq.sHtML

x |= (1 << 3);
来源：http://baike.fktsv.cn/Article/details/gskzfefcl.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.tarul.cn/Article/details/gailesqni.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.tarul.cn/Article/details/gqgxcszvb.sHtML

[S18] C：命令行参数
来源：http://blog.yfazqb.com/Article/details/gyafgiccb.sHtML

int main(int argc, char **argv)
来源：http://baike.yfazqb.com/Article/details/ggitceaza.sHtML

[S19] C：快速排序
来源：http://read.share.vehdjk.com/Article/details/ghslkkerx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fktsv.cn/Article/details/gzzbeytqd.sHtML

[S20] C：二分查找
来源：http://www.share.epnwcf.com/Article/details/gmgbfqepj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fktsv.cn/Article/details/grcvvwlwl.sHtML

[S21] C：字符类别判断
来源：http://mobile.tarul.cn/Article/details/ghtxfjecl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.yfazqb.com/Article/details/gmpthauyk.sHtML

[S22] C：字符串转数字
来源：http://mobile.bbcook.cn/Article/details/gmkmekkrl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.tarul.cn/Article/details/gastyyiuu.sHtML

[S23] C：随机数
来源：http://www.blog.yfazqb.com/Article/details/ggfedpzxk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.bbcook.cn/Article/details/gyyqfwghp.sHtML

[S24] C：获取本地时间
来源：http://read.share.fktsv.cn/Article/details/gmdzvojzu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.epnwcf.com/Article/details/ggqpeebbe.sHtML

[S25] C：内存拷贝
来源：http://m.share.bbcook.cn/Article/details/gbsjvnaqe.sHtML

memcpy(dst, src, n);
来源：http://m.share.fktsv.cn/Article/details/gzsmmmyhb.sHtML

[S26] C：内存清零
来源：http://mobile.yfazqb.com/Article/details/gufnjpksk.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.epnwcf.com/Article/details/grxilahzi.sHtML

[S27] C：定义常量
来源：http://m.share.tarul.cn/Article/details/gxnccdsdg.sHtML

const double PI = 3.14159;
来源：http://www.blog.epnwcf.com/Article/details/gsqxyqxvm.sHtML

[S28] C：静态变量
来源：http://baike.sjlbkw.cn/Article/details/gxqljsfpv.sHtML

static int counter = 0;
来源：http://read.share.fktsv.cn/Article/details/gudyrpcbm.sHtML

[S29] C：变参函数
来源：http://baike.sjlbkw.cn/Article/details/gqzazlmia.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.epnwcf.com/Article/details/galsgrgme.sHtML

[S30] C：头文件保护
来源：http://www.m.share.bbcook.cn/Article/details/gmrrjtqdh.sHtML

#ifndef X_H
来源：http://read.share.bbcook.cn/Article/details/gipqsmuwn.sHtML

#define X_H
来源：http://read.share.yfazqb.com/Article/details/gvmpniogk.sHtML

#endif
来源：http://www.blog.yfazqb.com/Article/details/gsrklasbf.sHtML

[S31] C++：Hello World
来源：http://3g.vehdjk.com/Article/details/gncghvbwf.sHtML

#include <iostream>
来源：http://3g.yfazqb.com/Article/details/gewzgyiwk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gzhwpxdmg.sHtML

[S32] C++：字符串
来源：http://www.m.share.bbcook.cn/Article/details/geertijlx.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.bbcook.cn/Article/details/gpqapkhgw.sHtML

[S33] C++：vector 增删
来源：http://blog.bbcook.cn/Article/details/ghoewrhxy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fktsv.cn/Article/details/gigijhfzf.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fktsv.cn/Article/details/glsrmrqts.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.bbcook.cn/Article/details/gaupjfxsg.sHtML

[S35] C++：map
来源：http://www.m.share.tarul.cn/Article/details/gjvpediqy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.tarul.cn/Article/details/gtslvnghc.sHtML

[S36] C++：unordered_map
来源：http://m.share.bbcook.cn/Article/details/gzozgvguk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gtuksfwel.sHtML

[S37] C++：set
来源：http://m.share.fktsv.cn/Article/details/gzlqgxwxb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.epnwcf.com/Article/details/gvsneuvmb.sHtML

[S38] C++：排序
来源：http://wap.tarul.cn/Article/details/gembcmfkq.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.yfazqb.com/Article/details/gngtyyitm.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.vehdjk.com/Article/details/gjhqqrhdj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.epnwcf.com/Article/details/gjvywsuww.sHtML

[S40] C++：查找元素
来源：http://mobile.epnwcf.com/Article/details/gepcrrepz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fktsv.cn/Article/details/gvuynuroa.sHtML

[S41] C++：类与构造函数
来源：http://3g.bbcook.cn/Article/details/gmpotpxqq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.sjlbkw.cn/Article/details/gezdfiysu.sHtML

[S42] C++：继承与虚函数
来源：http://baike.bbcook.cn/Article/details/gbtxddlfg.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.bbcook.cn/Article/details/gerwfypum.sHtML

[S43] C++：智能指针
来源：http://read.share.bbcook.cn/Article/details/gxzjvhjwe.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fktsv.cn/Article/details/gayuvwhme.sHtML

[S44] C++：引用传参
来源：http://mobile.sjlbkw.cn/Article/details/gysyqjdkh.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.bbcook.cn/Article/details/gclazfejk.sHtML

[S45] C++：lambda
来源：http://baike.tarul.cn/Article/details/gmlkuxgfs.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.yfazqb.com/Article/details/gzvmryoio.sHtML

[S46] C++：函数模板
来源：http://read.share.fktsv.cn/Article/details/ggtavjqbs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.bbcook.cn/Article/details/gmmgtahee.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.bbcook.cn/Article/details/gafaapwde.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.bbcook.cn/Article/details/grnebasgy.sHtML

[S48] C++：逐行读文件
来源：http://www.share.epnwcf.com/Article/details/gbgqgnodh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.yfazqb.com/Article/details/gmbsroatj.sHtML

while (std::getline(in, line)) { }
来源：http://baike.yfazqb.com/Article/details/gbumxcjtj.sHtML

[S49] C++：写文件
来源：http://mobile.yfazqb.com/Article/details/gbynrcvvo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.bbcook.cn/Article/details/grncudrfy.sHtML

[S50] C++：格式化数字
来源：http://blog.bbcook.cn/Article/details/gnqjuucqa.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.vehdjk.com/Article/details/grqzvepzh.sHtML

[S51] C++：显式类型转换
来源：http://3g.bbcook.cn/Article/details/ghpifppjd.sHtML

static_cast<double>(a) / b
来源：http://baike.sjlbkw.cn/Article/details/gsibqhohu.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fktsv.cn/Article/details/gwhxdsvpc.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.epnwcf.com/Article/details/guqgbmamj.sHtML

[S53] C++：移动语义
来源：http://www.share.fktsv.cn/Article/details/grnuryzec.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.yfazqb.com/Article/details/gmxyegbvp.sHtML

[S54] C++：异常处理
来源：http://3g.bbcook.cn/Article/details/gkkotzwdb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.bbcook.cn/Article/details/gqzhecllj.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.vehdjk.com/Article/details/giyarhxsu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/gfzlbnqir.sHtML

[S56] C++：optional
来源：http://baike.sjlbkw.cn/Article/details/guezbrobg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.vehdjk.com/Article/details/gldcvfymc.sHtML

[S57] C++：编译期常量
来源：http://www.blog.yfazqb.com/Article/details/gyrbcztij.sHtML

constexpr int N = 10;
来源：http://www.blog.vehdjk.com/Article/details/gkyjmkwcd.sHtML

[S58] C++：命名空间
来源：http://mobile.yfazqb.com/Article/details/gliameift.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.sjlbkw.cn/Article/details/ghirkpxtx.sHtML

[S59] C++：静态断言
来源：http://wap.sjlbkw.cn/Article/details/gcxgrjapj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.vehdjk.com/Article/details/gbqsyjvvn.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.vehdjk.com/Article/details/gzvloqkci.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.tarul.cn/Article/details/gqkuvkuvm.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gsanauxlj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.vehdjk.com/Article/details/gocgoazqv.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gijzpveoq.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.sjlbkw.cn/Article/details/gufdgqtcl.sHtML

println("Hello")
来源：http://baike.vehdjk.com/Article/details/gbhkaoada.sHtML

[T02] Kotlin：变量
来源：http://www.share.vehdjk.com/Article/details/gnuihtduy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.vehdjk.com/Article/details/gkuntzdxi.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.bbcook.cn/Article/details/gfrejlmnp.sHtML

"值: $b"
来源：http://wap.tarul.cn/Article/details/gcbcxrnwm.sHtML

[T04] Kotlin：空安全
来源：http://www.share.bbcook.cn/Article/details/gykjemdgb.sHtML

val n: String? = null;  n?.length
来源：http://3g.fktsv.cn/Article/details/gsdgyeird.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.yfazqb.com/Article/details/gccszlnqk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fktsv.cn/Article/details/goizlmima.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.bbcook.cn/Article/details/ghggpnoso.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.tarul.cn/Article/details/gzypfwkwy.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.bbcook.cn/Article/details/gaoqlzonh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.tarul.cn/Article/details/gymgqlsft.sHtML

[T08] Kotlin：数据类
来源：http://blog.vehdjk.com/Article/details/gnolzbnwx.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fktsv.cn/Article/details/gttehpkep.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fktsv.cn/Article/details/gyvxsdbhu.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fktsv.cn/Article/details/ggxkrghrb.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.yfazqb.com/Article/details/gbaovgmsk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.epnwcf.com/Article/details/ggtenhzul.sHtML

[T11] Kotlin：协程
来源：http://wap.tarul.cn/Article/details/ghbomruru.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.yfazqb.com/Article/details/gmtbkysbu.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fktsv.cn/Article/details/gammsdszo.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.vehdjk.com/Article/details/gpkhgbwcj.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.sjlbkw.cn/Article/details/gctzoagiw.sHtML

val m = mapOf("a" to 1)
来源：http://3g.yfazqb.com/Article/details/gklerupeq.sHtML

[T14] Kotlin：循环
来源：http://www.blog.epnwcf.com/Article/details/gjbkmeyey.sHtML

for (i in 1..10) println(i)
来源：http://wap.yfazqb.com/Article/details/gwtpogoqs.sHtML

[T15] Kotlin：接口
来源：http://baike.bbcook.cn/Article/details/glkujxuyy.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.tarul.cn/Article/details/gbmqrgnbc.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/gnsexysya.sHtML

print("Hello")
来源：http://blog.yfazqb.com/Article/details/gadivynzv.sHtML

[T17] Swift：变量与常量
来源：http://m.share.vehdjk.com/Article/details/gouofaipp.sHtML

var a = 1;  let b = 2
来源：http://wap.epnwcf.com/Article/details/glzlbzbcf.sHtML

[T18] Swift：字符串插值
来源：http://blog.fktsv.cn/Article/details/gdrnjbwcc.sHtML

"值: \(b)"
来源：http://read.share.vehdjk.com/Article/details/gnrtjnqse.sHtML

[T19] Swift：可选绑定
来源：http://3g.bbcook.cn/Article/details/gfhhlupvu.sHtML

if let n = opt { print(n) }
来源：http://read.share.epnwcf.com/Article/details/ggwymptpr.sHtML

[T20] Swift：数组操作
来源：http://baike.bbcook.cn/Article/details/gxflcxnef.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.tarul.cn/Article/details/gxwcliaer.sHtML

[T21] Swift：遍历
来源：http://www.share.tarul.cn/Article/details/gadyjxahc.sHtML

for x in a { print(x) }
来源：http://mobile.fktsv.cn/Article/details/goxquhfao.sHtML

[T22] Swift：字典
来源：http://www.share.epnwcf.com/Article/details/gmviwhuhz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fktsv.cn/Article/details/gfqqvpxmn.sHtML

[T23] Swift：函数
来源：http://baike.epnwcf.com/Article/details/gjrwybotl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.tarul.cn/Article/details/gqqvsbljt.sHtML

[T24] Swift：闭包
来源：http://www.m.share.epnwcf.com/Article/details/gogpyhlsq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.epnwcf.com/Article/details/gvohwhwky.sHtML


<!-- 参考信息 -->