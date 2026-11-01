代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.bbcook.cn/Article/details/gcovbysjs.sHtML

[R26] 命令替换
来源：http://wap.vehdjk.com/Article/details/gwtjxvdbz.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.sjlbkw.cn/Article/details/gbwvodymu.sHtML

[R27] 算术展开
来源：http://www.share.sjlbkw.cn/Article/details/gyrjsvdpa.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fktsv.cn/Article/details/gqmeoqzlk.sHtML

[R28] 浮点运算
来源：http://3g.sjlbkw.cn/Article/details/gmsynhrvz.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.epnwcf.com/Article/details/genquqhlu.sHtML

[R29] 定义函数
来源：http://baike.vehdjk.com/Article/details/gvzgcjdhm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.vehdjk.com/Article/details/gigpsmjtk.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.tarul.cn/Article/details/gdkiddcbm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.yfazqb.com/Article/details/gyejhqfrx.sHtML

[R31] 局部变量
来源：http://www.blog.sjlbkw.cn/Article/details/gdhvxhofv.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.bbcook.cn/Article/details/gwviqywce.sHtML

[R32] 参数个数校验
来源：http://read.share.fktsv.cn/Article/details/gdmbxtjbd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fktsv.cn/Article/details/gopyuddgl.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.bbcook.cn/Article/details/gkxapchyw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.yfazqb.com/Article/details/gbujrhtki.sHtML

[R34] 退出时清理
来源：http://www.blog.vehdjk.com/Article/details/glukzcfke.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fktsv.cn/Article/details/gkwlzkofg.sHtML

[R35] 后台执行并等待
来源：http://m.share.epnwcf.com/Article/details/gwpcfveub.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.bbcook.cn/Article/details/grmnkficb.sHtML

[R36] 并发执行多个任务
来源：http://read.share.sjlbkw.cn/Article/details/gmdtcrbqc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.vehdjk.com/Article/details/gyjcdtazg.sHtML

[R37] 把输出赋给变量
来源：http://blog.fktsv.cn/Article/details/gmwpjithq.sHtML

files=$(ls -1)
来源：http://wap.bbcook.cn/Article/details/gsycuwscv.sHtML

[R38] 管道串联
来源：http://3g.sjlbkw.cn/Article/details/gggdcxyjj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.sjlbkw.cn/Article/details/garbtzjij.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.tarul.cn/Article/details/gwuyidwet.sHtML

cmd > out.log 2>&1
来源：http://baike.fktsv.cn/Article/details/ghtmvvrtw.sHtML

[R40] 追加写日志
来源：http://m.share.sjlbkw.cn/Article/details/giylbwnnp.sHtML

echo "log" >> out.log
来源：http://read.share.yfazqb.com/Article/details/gccboftmm.sHtML

[R41] 丢弃输出
来源：http://www.m.share.vehdjk.com/Article/details/guioiecqw.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.sjlbkw.cn/Article/details/geaouyyvw.sHtML

[R42] 输入重定向
来源：http://www.blog.epnwcf.com/Article/details/gnyrfishy.sHtML

wc -l < a.txt
来源：http://blog.vehdjk.com/Article/details/gkpuafxse.sHtML

[R43] 按名字查找文件
来源：http://mobile.bbcook.cn/Article/details/gvictklok.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.bbcook.cn/Article/details/gidghdjyi.sHtML

[R44] 按修改时间查找
来源：http://www.blog.bbcook.cn/Article/details/gxozagarr.sHtML

find . -mtime -7 -type f
来源：http://read.share.yfazqb.com/Article/details/gdswiwuxz.sHtML

[R45] 批量删除
来源：http://3g.bbcook.cn/Article/details/gbgeyuqyy.sHtML

find . -name "*.tmp" -delete
来源：http://blog.vehdjk.com/Article/details/gxnsixoup.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fktsv.cn/Article/details/grmezapth.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.tarul.cn/Article/details/gpmwfpptg.sHtML

[R47] sed 单行替换
来源：http://3g.bbcook.cn/Article/details/gyphzagdo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.yfazqb.com/Article/details/gbwzwmotc.sHtML

[R48] awk 取指定列
来源：http://blog.epnwcf.com/Article/details/gfzjyqalv.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.epnwcf.com/Article/details/gnmutoabe.sHtML

[R49] awk 带条件
来源：http://www.share.tarul.cn/Article/details/gqqohtxwm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.yfazqb.com/Article/details/garahqsac.sHtML

[R50] awk 求和
来源：http://m.share.bbcook.cn/Article/details/gkzxxcjqt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.tarul.cn/Article/details/gdqqlgdrd.sHtML

[R51] 排序去重取前几
来源：http://wap.bbcook.cn/Article/details/gwhgluwar.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.yfazqb.com/Article/details/giqagbhqz.sHtML

[R52] 统计行数
来源：http://3g.epnwcf.com/Article/details/ghhkvstsh.sHtML

wc -l a.txt
来源：http://www.blog.fktsv.cn/Article/details/gwzehjlmh.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fktsv.cn/Article/details/gmalnxbly.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.bbcook.cn/Article/details/gmffxmpmc.sHtML

[R54] 比较两个文件
来源：http://www.share.vehdjk.com/Article/details/gomylzlnp.sHtML

diff a.txt b.txt
来源：http://wap.tarul.cn/Article/details/gaitvfrna.sHtML

[R55] 压缩与解压
来源：http://www.blog.vehdjk.com/Article/details/gweosihbz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.vehdjk.com/Article/details/gdxvgerot.sHtML

[R56] 远程拷贝
来源：http://mobile.fktsv.cn/Article/details/gowfayqlf.sHtML

scp file user@host:/path/
来源：http://read.share.yfazqb.com/Article/details/giackjeli.sHtML

[R57] 远程执行命令
来源：http://www.m.share.epnwcf.com/Article/details/gfoiaasvb.sHtML

ssh user@host 'uptime'
来源：http://wap.vehdjk.com/Article/details/ggjnltquz.sHtML

[R58] 下载文件
来源：http://baike.yfazqb.com/Article/details/gqdoqlssl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.epnwcf.com/Article/details/gbwuxmbdr.sHtML

[R59] 发 POST JSON
来源：http://m.share.sjlbkw.cn/Article/details/guujopzsi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.tarul.cn/Article/details/gfpgnvzhj.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.tarul.cn/Article/details/ghglsrsqg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.epnwcf.com/Article/details/ghfbczonu.sHtML

[R61] 磁盘占用
来源：http://m.share.fktsv.cn/Article/details/gbrsnlhif.sHtML

df -h;  du -sh *
来源：http://www.share.yfazqb.com/Article/details/gdostawni.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fktsv.cn/Article/details/gimgxctcl.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.bbcook.cn/Article/details/gdhuarbfz.sHtML

[R63] 内存与进程
来源：http://read.share.fktsv.cn/Article/details/guyaitwou.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.tarul.cn/Article/details/gybhefwpe.sHtML

[R64] 结束进程
来源：http://wap.tarul.cn/Article/details/gmvmbwont.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.sjlbkw.cn/Article/details/gwzkgjybz.sHtML

[R65] 查看端口占用
来源：http://wap.yfazqb.com/Article/details/ghbpwczse.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.vehdjk.com/Article/details/gvcmumsti.sHtML

[R66] 定时任务
来源：http://3g.bbcook.cn/Article/details/gjyrynxjl.sHtML

crontab -e;  crontab -l
来源：http://mobile.bbcook.cn/Article/details/gudvagajg.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.yfazqb.com/Article/details/gfkjutcie.sHtML

openssl rand -hex 16
来源：http://www.blog.sjlbkw.cn/Article/details/gimqsemnf.sHtML

[R68] 计算文件校验值
来源：http://www.share.vehdjk.com/Article/details/gblmcfuau.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.vehdjk.com/Article/details/guyunzmjp.sHtML

[R69] 生成随机密码
来源：http://3g.fktsv.cn/Article/details/gcqfmocyy.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.bbcook.cn/Article/details/gcazflknu.sHtML

[R70] 时间戳与互转
来源：http://blog.bbcook.cn/Article/details/gusmfjdqn.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.sjlbkw.cn/Article/details/glgzwosvy.sHtML

[R71] 日期格式化
来源：http://mobile.yfazqb.com/Article/details/gsotdozxk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.vehdjk.com/Article/details/gecsgktmo.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fktsv.cn/Article/details/gxealufge.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.epnwcf.com/Article/details/gyjeaslav.sHtML

[R73] 分割大日志
来源：http://mobile.sjlbkw.cn/Article/details/gzdpgtmck.sHtML

split -l 1000 big.log part_
来源：http://mobile.sjlbkw.cn/Article/details/gyofglymb.sHtML

[R74] 批量重命名
来源：http://baike.epnwcf.com/Article/details/gcaetzpeh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.sjlbkw.cn/Article/details/ggphcueon.sHtML

[R75] 导出环境变量
来源：http://read.share.yfazqb.com/Article/details/gmsvybexa.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.bbcook.cn/Article/details/gkpwtbqxr.sHtML

[R76] 使用临时文件
来源：http://baike.bbcook.cn/Article/details/gqbmnawye.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.yfazqb.com/Article/details/ghrzeuddo.sHtML

[R77] 读取用户输入
来源：http://www.blog.vehdjk.com/Article/details/gjwefyngg.sHtML

read -rp "请输入: " ans
来源：http://3g.epnwcf.com/Article/details/gwbnqbxhw.sHtML

[R78] 交互式菜单
来源：http://baike.epnwcf.com/Article/details/gnnjhkwyj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.yfazqb.com/Article/details/ghvfnooxn.sHtML

[R79] 解析命令行选项
来源：http://blog.tarul.cn/Article/details/goegpeooy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fktsv.cn/Article/details/gloqylezk.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fktsv.cn/Article/details/glnepkygd.sHtML

time ./run.sh
来源：http://www.share.vehdjk.com/Article/details/gyrncsbrj.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/givqwsyat.sHtML

S. C / C++ 专题
来源：http://wap.tarul.cn/Article/details/gkrmpnrfk.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gtnmtjjkq.sHtML

[S01] C：Hello World
来源：http://blog.epnwcf.com/Article/details/gwrqptmmn.sHtML

#include <stdio.h>
来源：http://www.m.share.sjlbkw.cn/Article/details/gfwhompdn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.tarul.cn/Article/details/gfmlksrtl.sHtML

[S02] C：变量与格式化输出
来源：http://3g.tarul.cn/Article/details/gtkkojscq.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.epnwcf.com/Article/details/gjgnldgph.sHtML

[S03] C：读入整数
来源：http://www.m.share.bbcook.cn/Article/details/gcpfxlffz.sHtML

int x; scanf("%d", &x);
来源：http://read.share.epnwcf.com/Article/details/gmltkqktj.sHtML

[S04] C：字符串复制
来源：http://www.share.epnwcf.com/Article/details/glxfvpsdo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.bbcook.cn/Article/details/gzeeuljye.sHtML

[S05] C：字符串长度
来源：http://3g.bbcook.cn/Article/details/ghuyyscax.sHtML

strlen(s)
来源：http://3g.fktsv.cn/Article/details/gvprcyfsr.sHtML

[S06] C：字符串比较
来源：http://www.blog.vehdjk.com/Article/details/guyhjpzel.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.epnwcf.com/Article/details/ghzxmklod.sHtML

[S07] C：数组遍历求和
来源：http://mobile.yfazqb.com/Article/details/gtguzupnh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.epnwcf.com/Article/details/gquhvlema.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fktsv.cn/Article/details/gnscotnxw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.yfazqb.com/Article/details/gtglnbtpf.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.yfazqb.com/Article/details/grwtdasit.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.sjlbkw.cn/Article/details/gzouaoqpr.sHtML

[S10] C：指针与解引用
来源：http://m.share.vehdjk.com/Article/details/grhmkdrks.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.sjlbkw.cn/Article/details/giozbccxj.sHtML

[S11] C：逐行读文件
来源：http://m.share.epnwcf.com/Article/details/gngdqqexa.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.tarul.cn/Article/details/gqfyfkzrz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.epnwcf.com/Article/details/gwccefahk.sHtML

fclose(f);
来源：http://mobile.epnwcf.com/Article/details/gbuexbftw.sHtML

[S12] C：写文件
来源：http://mobile.vehdjk.com/Article/details/gxvwnlhxu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.tarul.cn/Article/details/gcroxsgyi.sHtML

[S13] C：宏定义
来源：http://read.share.bbcook.cn/Article/details/geqvqeoyg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fktsv.cn/Article/details/gxliibyzz.sHtML

[S14] C：枚举
来源：http://www.share.tarul.cn/Article/details/gozzphmad.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.tarul.cn/Article/details/gwocijncw.sHtML

[S15] C：类型转换
来源：http://www.blog.epnwcf.com/Article/details/gvouvwgdx.sHtML

(double) a / b
来源：http://www.m.share.yfazqb.com/Article/details/gwbgvnwid.sHtML

[S16] C：位操作置位
来源：http://www.blog.tarul.cn/Article/details/gpscyzpuv.sHtML

x |= (1 << 3);
来源：http://mobile.fktsv.cn/Article/details/gyelyhcje.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.yfazqb.com/Article/details/gaffffjyt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.tarul.cn/Article/details/gkoqjdhpi.sHtML

[S18] C：命令行参数
来源：http://www.blog.fktsv.cn/Article/details/ggslialcm.sHtML

int main(int argc, char **argv)
来源：http://read.share.bbcook.cn/Article/details/gqzjbqzmc.sHtML

[S19] C：快速排序
来源：http://www.m.share.bbcook.cn/Article/details/gotirnaxb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.bbcook.cn/Article/details/gsdrsbbnt.sHtML

[S20] C：二分查找
来源：http://m.share.epnwcf.com/Article/details/geaufqcmd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fktsv.cn/Article/details/gqhfgjbqq.sHtML

[S21] C：字符类别判断
来源：http://mobile.yfazqb.com/Article/details/giztecdhz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.sjlbkw.cn/Article/details/ghwuuafgj.sHtML

[S22] C：字符串转数字
来源：http://mobile.epnwcf.com/Article/details/gbfndcuql.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.bbcook.cn/Article/details/geuyvblrp.sHtML

[S23] C：随机数
来源：http://wap.bbcook.cn/Article/details/gcikhhcxe.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.yfazqb.com/Article/details/gmvtejydi.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.yfazqb.com/Article/details/glondacop.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.sjlbkw.cn/Article/details/gmwabmzzu.sHtML

[S25] C：内存拷贝
来源：http://wap.bbcook.cn/Article/details/gbnenxsix.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.vehdjk.com/Article/details/gkkdworzn.sHtML

[S26] C：内存清零
来源：http://m.share.sjlbkw.cn/Article/details/gkwzpizuf.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fktsv.cn/Article/details/ggtjkwfej.sHtML

[S27] C：定义常量
来源：http://mobile.sjlbkw.cn/Article/details/gfxqvejbx.sHtML

const double PI = 3.14159;
来源：http://3g.vehdjk.com/Article/details/gwvslbice.sHtML

[S28] C：静态变量
来源：http://www.m.share.bbcook.cn/Article/details/gmzobuvdt.sHtML

static int counter = 0;
来源：http://3g.tarul.cn/Article/details/ghmbqievt.sHtML

[S29] C：变参函数
来源：http://baike.vehdjk.com/Article/details/gsjwjmoop.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.yfazqb.com/Article/details/giuvsfnyr.sHtML

[S30] C：头文件保护
来源：http://read.share.sjlbkw.cn/Article/details/gmhiuzzem.sHtML

#ifndef X_H
来源：http://3g.fktsv.cn/Article/details/gxzsjaqtj.sHtML

#define X_H
来源：http://www.share.yfazqb.com/Article/details/gkyukeots.sHtML

#endif
来源：http://blog.bbcook.cn/Article/details/gmrgttwmq.sHtML

[S31] C++：Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/grdtgjgqr.sHtML

#include <iostream>
来源：http://baike.bbcook.cn/Article/details/gkmwssdxu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.bbcook.cn/Article/details/gaftuesze.sHtML

[S32] C++：字符串
来源：http://www.blog.vehdjk.com/Article/details/gnyjorluq.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.vehdjk.com/Article/details/gorrzpbhm.sHtML

[S33] C++：vector 增删
来源：http://wap.fktsv.cn/Article/details/givvoltqn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.bbcook.cn/Article/details/gvzhrufir.sHtML

[S34] C++：遍历 vector
来源：http://www.share.epnwcf.com/Article/details/gwdxacoac.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.yfazqb.com/Article/details/gcfbzziel.sHtML

[S35] C++：map
来源：http://blog.vehdjk.com/Article/details/gfddidcjv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gccyvowso.sHtML

[S36] C++：unordered_map
来源：http://www.blog.epnwcf.com/Article/details/gcqrsupwv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.vehdjk.com/Article/details/gradplbtq.sHtML

[S37] C++：set
来源：http://read.share.yfazqb.com/Article/details/gqlpzrjrj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.bbcook.cn/Article/details/gkyvelkhz.sHtML

[S38] C++：排序
来源：http://www.m.share.tarul.cn/Article/details/geoqnvpnf.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.sjlbkw.cn/Article/details/gubzlxybu.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.yfazqb.com/Article/details/gactjjvye.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.bbcook.cn/Article/details/ghvvygdqw.sHtML

[S40] C++：查找元素
来源：http://www.blog.sjlbkw.cn/Article/details/gpyfrdesj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.sjlbkw.cn/Article/details/gxamafbqo.sHtML

[S41] C++：类与构造函数
来源：http://baike.vehdjk.com/Article/details/gyrxqdpen.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.yfazqb.com/Article/details/gecqpucvk.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.tarul.cn/Article/details/gloagbvvg.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fktsv.cn/Article/details/gxtcidebf.sHtML

[S43] C++：智能指针
来源：http://wap.fktsv.cn/Article/details/gfilptjee.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.tarul.cn/Article/details/gkmxdpdgl.sHtML

[S44] C++：引用传参
来源：http://baike.fktsv.cn/Article/details/grmmcryjj.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.yfazqb.com/Article/details/gtuzhpldv.sHtML

[S45] C++：lambda
来源：http://m.share.tarul.cn/Article/details/gvxncjsih.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.epnwcf.com/Article/details/guwclzesm.sHtML

[S46] C++：函数模板
来源：http://www.share.vehdjk.com/Article/details/gyigbsicw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.bbcook.cn/Article/details/gwkvxjyox.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.vehdjk.com/Article/details/gqvkglncv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.epnwcf.com/Article/details/gxrhoaoah.sHtML

[S48] C++：逐行读文件
来源：http://wap.yfazqb.com/Article/details/getxjihov.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.vehdjk.com/Article/details/gpvimipks.sHtML

while (std::getline(in, line)) { }
来源：http://wap.vehdjk.com/Article/details/gizufkhla.sHtML

[S49] C++：写文件
来源：http://read.share.sjlbkw.cn/Article/details/grwghzsiu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.yfazqb.com/Article/details/gcewkisea.sHtML

[S50] C++：格式化数字
来源：http://baike.epnwcf.com/Article/details/gsngkllyt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.yfazqb.com/Article/details/gagccgvpy.sHtML

[S51] C++：显式类型转换
来源：http://mobile.sjlbkw.cn/Article/details/gjdhbnwep.sHtML

static_cast<double>(a) / b
来源：http://baike.yfazqb.com/Article/details/gugwqhlwy.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.bbcook.cn/Article/details/giiqhoitv.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.vehdjk.com/Article/details/gecuprmft.sHtML

[S53] C++：移动语义
来源：http://wap.sjlbkw.cn/Article/details/gszmbyupx.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fktsv.cn/Article/details/gkyqjkxzr.sHtML

[S54] C++：异常处理
来源：http://www.m.share.bbcook.cn/Article/details/ghrxlruxy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.vehdjk.com/Article/details/gkdtlvdkv.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fktsv.cn/Article/details/gqlzebarm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.sjlbkw.cn/Article/details/gdltgygld.sHtML

[S56] C++：optional
来源：http://3g.tarul.cn/Article/details/gtigalpzz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.epnwcf.com/Article/details/gqfqqwfxb.sHtML

[S57] C++：编译期常量
来源：http://blog.bbcook.cn/Article/details/gufweljtz.sHtML

constexpr int N = 10;
来源：http://www.share.tarul.cn/Article/details/gjjjehrju.sHtML

[S58] C++：命名空间
来源：http://3g.bbcook.cn/Article/details/gvcalrzzm.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.sjlbkw.cn/Article/details/gueragonf.sHtML

[S59] C++：静态断言
来源：http://3g.vehdjk.com/Article/details/gonrhwekt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.epnwcf.com/Article/details/gohqxfpyn.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.vehdjk.com/Article/details/gaibvjynf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.yfazqb.com/Article/details/gogxcqfvr.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gonhqusel.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.bbcook.cn/Article/details/gzmsshjnq.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gjalvlkfe.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.tarul.cn/Article/details/ggllkcaeu.sHtML

println("Hello")
来源：http://www.blog.sjlbkw.cn/Article/details/glnuwlami.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.vehdjk.com/Article/details/gpstaiuij.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.epnwcf.com/Article/details/gwmkkxiwx.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.yfazqb.com/Article/details/ggsznqyru.sHtML

"值: $b"
来源：http://3g.sjlbkw.cn/Article/details/gbokmdopj.sHtML

[T04] Kotlin：空安全
来源：http://m.share.bbcook.cn/Article/details/gnjkttpbg.sHtML

val n: String? = null;  n?.length
来源：http://baike.tarul.cn/Article/details/gvtalqiyw.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.epnwcf.com/Article/details/gixkkqndc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.epnwcf.com/Article/details/gkwbposww.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.tarul.cn/Article/details/grjnpntdm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.tarul.cn/Article/details/gumgrdnvf.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.epnwcf.com/Article/details/ghhoazglj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.bbcook.cn/Article/details/gbgvgiilw.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fktsv.cn/Article/details/gqpjqnjpv.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.bbcook.cn/Article/details/ggdmkpstt.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.yfazqb.com/Article/details/gawjvdalm.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.yfazqb.com/Article/details/gddmavvfr.sHtML

[T10] Kotlin：默认参数
来源：http://3g.tarul.cn/Article/details/gwcnkjpng.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.sjlbkw.cn/Article/details/gnuvibdno.sHtML

[T11] Kotlin：协程
来源：http://blog.yfazqb.com/Article/details/gxjgiykbz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.epnwcf.com/Article/details/gbnaalcgg.sHtML

[T12] Kotlin：解构声明
来源：http://wap.tarul.cn/Article/details/geihidsgb.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.tarul.cn/Article/details/gaqvlhzxz.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.tarul.cn/Article/details/gpdefcyyz.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.epnwcf.com/Article/details/gkgkvfngn.sHtML

[T14] Kotlin：循环
来源：http://m.share.vehdjk.com/Article/details/gkuuqtvko.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fktsv.cn/Article/details/gjxjiefsf.sHtML

[T15] Kotlin：接口
来源：http://baike.yfazqb.com/Article/details/gubeinean.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fktsv.cn/Article/details/gdliovzez.sHtML

[T16] Swift：Hello World
来源：http://read.share.tarul.cn/Article/details/gewbuxyoe.sHtML

print("Hello")
来源：http://www.m.share.epnwcf.com/Article/details/gryqzgsfa.sHtML

[T17] Swift：变量与常量
来源：http://3g.sjlbkw.cn/Article/details/gossqdxat.sHtML

var a = 1;  let b = 2
来源：http://read.share.epnwcf.com/Article/details/gxclbwaox.sHtML

[T18] Swift：字符串插值
来源：http://m.share.sjlbkw.cn/Article/details/gmonweasv.sHtML

"值: \(b)"
来源：http://baike.tarul.cn/Article/details/genvcuvaj.sHtML

[T19] Swift：可选绑定
来源：http://baike.bbcook.cn/Article/details/gbkbtedmu.sHtML

if let n = opt { print(n) }
来源：http://www.blog.bbcook.cn/Article/details/giwgvrkcb.sHtML

[T20] Swift：数组操作
来源：http://read.share.sjlbkw.cn/Article/details/gqezrzupu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.vehdjk.com/Article/details/gprlhhyib.sHtML

[T21] Swift：遍历
来源：http://baike.yfazqb.com/Article/details/gaovpcpir.sHtML

for x in a { print(x) }
来源：http://3g.sjlbkw.cn/Article/details/gfdkkwlod.sHtML

[T22] Swift：字典
来源：http://baike.sjlbkw.cn/Article/details/gwehtlfrw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.vehdjk.com/Article/details/gxibsjieb.sHtML

[T23] Swift：函数
来源：http://3g.fktsv.cn/Article/details/gornvnlab.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.yfazqb.com/Article/details/gwbjzpddw.sHtML

[T24] Swift：闭包
来源：http://read.share.bbcook.cn/Article/details/gjxtbwpcy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.epnwcf.com/Article/details/gotmahieb.sHtML

[T25] Swift：结构体
来源：http://baike.tarul.cn/Article/details/ggzprjcnw.sHtML

struct P { var x: Int }
来源：http://www.blog.epnwcf.com/Article/details/gckvfuqlz.sHtML

[T26] Swift：类与重写
来源：http://wap.tarul.cn/Article/details/gxyhlsfot.sHtML

class A: Base { override func f() {} }
来源：http://read.share.sjlbkw.cn/Article/details/gbpqoqjzi.sHtML

[T27] Swift：错误处理
来源：http://www.blog.yfazqb.com/Article/details/gvjhdyvxm.sHtML

do { try f() } catch { print(error) }
来源：http://3g.sjlbkw.cn/Article/details/gpxpcvenw.sHtML

[T28] Swift：枚举
来源：http://m.share.tarul.cn/Article/details/ghdnvxgzk.sHtML

enum Color { case red, green }
来源：http://3g.yfazqb.com/Article/details/ghekyrxnj.sHtML


<!-- 参考信息 -->