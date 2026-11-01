代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fktsv.cn/Article/details/gwlawabac.sHtML

[R26] 命令替换
来源：http://www.m.share.epnwcf.com/Article/details/gtrbxkgzq.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.yfazqb.com/Article/details/gnvlzkpnm.sHtML

[R27] 算术展开
来源：http://mobile.fktsv.cn/Article/details/gvbhfxuun.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.sjlbkw.cn/Article/details/gksvinjow.sHtML

[R28] 浮点运算
来源：http://read.share.epnwcf.com/Article/details/gzjqgywag.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.tarul.cn/Article/details/goxoawxma.sHtML

[R29] 定义函数
来源：http://baike.bbcook.cn/Article/details/gumdpjfrp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fktsv.cn/Article/details/gmyhlfmyb.sHtML

[R30] 函数返回状态码
来源：http://www.share.fktsv.cn/Article/details/ganikszdd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.epnwcf.com/Article/details/gronvsral.sHtML

[R31] 局部变量
来源：http://www.share.bbcook.cn/Article/details/ghurzhtks.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.tarul.cn/Article/details/gixqyprfu.sHtML

[R32] 参数个数校验
来源：http://read.share.vehdjk.com/Article/details/gvbdzouli.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.vehdjk.com/Article/details/gpnonjtwo.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.tarul.cn/Article/details/gtcwieuhn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.epnwcf.com/Article/details/gxourudni.sHtML

[R34] 退出时清理
来源：http://read.share.vehdjk.com/Article/details/govrtbgcg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.vehdjk.com/Article/details/gdfzkpbve.sHtML

[R35] 后台执行并等待
来源：http://www.share.vehdjk.com/Article/details/gwzpopzxs.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.epnwcf.com/Article/details/geikbluin.sHtML

[R36] 并发执行多个任务
来源：http://www.share.epnwcf.com/Article/details/guaiuqopa.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.tarul.cn/Article/details/grgylehkc.sHtML

[R37] 把输出赋给变量
来源：http://blog.vehdjk.com/Article/details/gueitvgsm.sHtML

files=$(ls -1)
来源：http://3g.fktsv.cn/Article/details/gkectwlof.sHtML

[R38] 管道串联
来源：http://www.m.share.yfazqb.com/Article/details/ggpiroxzp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.sjlbkw.cn/Article/details/gyxiruwmv.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.tarul.cn/Article/details/gfwdzriho.sHtML

cmd > out.log 2>&1
来源：http://baike.bbcook.cn/Article/details/gharcbhtt.sHtML

[R40] 追加写日志
来源：http://www.blog.vehdjk.com/Article/details/gwblstntf.sHtML

echo "log" >> out.log
来源：http://read.share.bbcook.cn/Article/details/gjislvwzb.sHtML

[R41] 丢弃输出
来源：http://mobile.yfazqb.com/Article/details/grlmgntzp.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.tarul.cn/Article/details/gujsudrgh.sHtML

[R42] 输入重定向
来源：http://blog.vehdjk.com/Article/details/gohacufgi.sHtML

wc -l < a.txt
来源：http://wap.bbcook.cn/Article/details/gbudshnyx.sHtML

[R43] 按名字查找文件
来源：http://read.share.yfazqb.com/Article/details/gaarfwakm.sHtML

find . -name "*.log" -type f
来源：http://3g.vehdjk.com/Article/details/gascwkwad.sHtML

[R44] 按修改时间查找
来源：http://read.share.fktsv.cn/Article/details/gfpaxeyzs.sHtML

find . -mtime -7 -type f
来源：http://m.share.fktsv.cn/Article/details/gregheibb.sHtML

[R45] 批量删除
来源：http://mobile.bbcook.cn/Article/details/gtzshhaka.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fktsv.cn/Article/details/grfezcmhf.sHtML

[R46] 递归替换文件内容
来源：http://m.share.epnwcf.com/Article/details/gbwfcmawm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.vehdjk.com/Article/details/gyvilmqya.sHtML

[R47] sed 单行替换
来源：http://mobile.bbcook.cn/Article/details/gieotnuuw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.epnwcf.com/Article/details/gaegxnbix.sHtML

[R48] awk 取指定列
来源：http://blog.bbcook.cn/Article/details/ganycoobo.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.yfazqb.com/Article/details/gekkqlsnr.sHtML

[R49] awk 带条件
来源：http://baike.bbcook.cn/Article/details/guirwynag.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.bbcook.cn/Article/details/gengoovha.sHtML

[R50] awk 求和
来源：http://www.share.vehdjk.com/Article/details/gxtfhvzip.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.tarul.cn/Article/details/gzowymeyn.sHtML

[R51] 排序去重取前几
来源：http://mobile.yfazqb.com/Article/details/gqauxafqn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fktsv.cn/Article/details/glqycwzta.sHtML

[R52] 统计行数
来源：http://read.share.tarul.cn/Article/details/gdjrlirtc.sHtML

wc -l a.txt
来源：http://read.share.vehdjk.com/Article/details/gfdfhhnvy.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.tarul.cn/Article/details/gcagwnyut.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.epnwcf.com/Article/details/gfroukrtj.sHtML

[R54] 比较两个文件
来源：http://blog.sjlbkw.cn/Article/details/ggghzjjmw.sHtML

diff a.txt b.txt
来源：http://mobile.sjlbkw.cn/Article/details/gvasidahu.sHtML

[R55] 压缩与解压
来源：http://www.share.yfazqb.com/Article/details/gvtkjacbd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.epnwcf.com/Article/details/gkpjteeae.sHtML

[R56] 远程拷贝
来源：http://www.blog.vehdjk.com/Article/details/gukbnwxup.sHtML

scp file user@host:/path/
来源：http://wap.sjlbkw.cn/Article/details/gwgujqrhu.sHtML

[R57] 远程执行命令
来源：http://3g.tarul.cn/Article/details/gikvltblk.sHtML

ssh user@host 'uptime'
来源：http://www.blog.vehdjk.com/Article/details/gszkwaotj.sHtML

[R58] 下载文件
来源：http://baike.sjlbkw.cn/Article/details/gcagdzdvs.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.sjlbkw.cn/Article/details/gypobslpf.sHtML

[R59] 发 POST JSON
来源：http://www.blog.tarul.cn/Article/details/gxexxtgmi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.epnwcf.com/Article/details/gupcmniqo.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.vehdjk.com/Article/details/gbndwohqu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.tarul.cn/Article/details/gjeydneqo.sHtML

[R61] 磁盘占用
来源：http://m.share.vehdjk.com/Article/details/gisbmjlxk.sHtML

df -h;  du -sh *
来源：http://m.share.bbcook.cn/Article/details/gcsdgprdy.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fktsv.cn/Article/details/gkhoskozo.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.bbcook.cn/Article/details/gmociesjn.sHtML

[R63] 内存与进程
来源：http://www.m.share.bbcook.cn/Article/details/gvrkszcyb.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.vehdjk.com/Article/details/gtkxkmrjj.sHtML

[R64] 结束进程
来源：http://m.share.fktsv.cn/Article/details/gdchobctk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.yfazqb.com/Article/details/gpjzbdonv.sHtML

[R65] 查看端口占用
来源：http://m.share.bbcook.cn/Article/details/ghizxpabc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.tarul.cn/Article/details/gqtryrjga.sHtML

[R66] 定时任务
来源：http://www.blog.vehdjk.com/Article/details/geiotvtay.sHtML

crontab -e;  crontab -l
来源：http://m.share.tarul.cn/Article/details/gquptopen.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fktsv.cn/Article/details/gqfedqdqf.sHtML

openssl rand -hex 16
来源：http://www.share.sjlbkw.cn/Article/details/gebyjsohf.sHtML

[R68] 计算文件校验值
来源：http://3g.yfazqb.com/Article/details/goaxociav.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fktsv.cn/Article/details/gypawtycr.sHtML

[R69] 生成随机密码
来源：http://www.blog.tarul.cn/Article/details/gqmebijkk.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fktsv.cn/Article/details/ghhgeofvh.sHtML

[R70] 时间戳与互转
来源：http://mobile.vehdjk.com/Article/details/grgmzsluw.sHtML

date +%s;  date -d @1700000000
来源：http://wap.bbcook.cn/Article/details/ghvosssax.sHtML

[R71] 日期格式化
来源：http://read.share.vehdjk.com/Article/details/glvmagyxc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.yfazqb.com/Article/details/gjszjcmmm.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fktsv.cn/Article/details/gpzutuopi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.vehdjk.com/Article/details/gudxhwpcw.sHtML

[R73] 分割大日志
来源：http://www.share.epnwcf.com/Article/details/gctpfnyvk.sHtML

split -l 1000 big.log part_
来源：http://www.blog.yfazqb.com/Article/details/gfmxslxxv.sHtML

[R74] 批量重命名
来源：http://mobile.bbcook.cn/Article/details/gjnhaleol.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fktsv.cn/Article/details/gjdfumuzq.sHtML

[R75] 导出环境变量
来源：http://www.blog.yfazqb.com/Article/details/gxkvtnkpd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.yfazqb.com/Article/details/gisuciosk.sHtML

[R76] 使用临时文件
来源：http://www.blog.epnwcf.com/Article/details/gkrrvthmt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.bbcook.cn/Article/details/gtnssvxzc.sHtML

[R77] 读取用户输入
来源：http://www.blog.yfazqb.com/Article/details/gozlzdpen.sHtML

read -rp "请输入: " ans
来源：http://mobile.vehdjk.com/Article/details/gppgnfnoa.sHtML

[R78] 交互式菜单
来源：http://read.share.epnwcf.com/Article/details/gzmqtgyzf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.yfazqb.com/Article/details/grtzlkzuz.sHtML

[R79] 解析命令行选项
来源：http://mobile.epnwcf.com/Article/details/gqupfknij.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.yfazqb.com/Article/details/gurhtxlmb.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.bbcook.cn/Article/details/gbbxmrsrc.sHtML

time ./run.sh
来源：http://www.share.vehdjk.com/Article/details/gzcpxbrtg.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/grltckheb.sHtML

S. C / C++ 专题
来源：http://baike.vehdjk.com/Article/details/ghotruetu.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gralgyafg.sHtML

[S01] C：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gxgtocgyh.sHtML

#include <stdio.h>
来源：http://blog.fktsv.cn/Article/details/gwjicyfus.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.vehdjk.com/Article/details/glnqbgnsa.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.bbcook.cn/Article/details/gtqufkphn.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.bbcook.cn/Article/details/gxywshynf.sHtML

[S03] C：读入整数
来源：http://www.m.share.vehdjk.com/Article/details/gvjyvixgc.sHtML

int x; scanf("%d", &x);
来源：http://baike.yfazqb.com/Article/details/gexzertso.sHtML

[S04] C：字符串复制
来源：http://mobile.sjlbkw.cn/Article/details/gtwxpjyts.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.sjlbkw.cn/Article/details/gsebllbey.sHtML

[S05] C：字符串长度
来源：http://wap.fktsv.cn/Article/details/glwwcwmfd.sHtML

strlen(s)
来源：http://www.blog.bbcook.cn/Article/details/gjxlkhdxh.sHtML

[S06] C：字符串比较
来源：http://3g.epnwcf.com/Article/details/gnrqrzxad.sHtML

strcmp(a, b) == 0
来源：http://mobile.sjlbkw.cn/Article/details/ghduablkm.sHtML

[S07] C：数组遍历求和
来源：http://blog.vehdjk.com/Article/details/guwrsltbk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.yfazqb.com/Article/details/gyjfhhzjr.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.yfazqb.com/Article/details/gmlynzpae.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.epnwcf.com/Article/details/gkuquqodg.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.yfazqb.com/Article/details/gdnghbbdi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.bbcook.cn/Article/details/grlyktaav.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.epnwcf.com/Article/details/gdzkhshhy.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.sjlbkw.cn/Article/details/gkkcayvgg.sHtML

[S11] C：逐行读文件
来源：http://read.share.fktsv.cn/Article/details/gikdequhi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.sjlbkw.cn/Article/details/gzlsvwgjf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.epnwcf.com/Article/details/gdlsppnno.sHtML

fclose(f);
来源：http://www.m.share.tarul.cn/Article/details/gnwavaewk.sHtML

[S12] C：写文件
来源：http://www.blog.epnwcf.com/Article/details/gdeobgvgd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fktsv.cn/Article/details/grchtwdsg.sHtML

[S13] C：宏定义
来源：http://www.share.fktsv.cn/Article/details/ghkvguvtv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fktsv.cn/Article/details/gqcyelozh.sHtML

[S14] C：枚举
来源：http://wap.vehdjk.com/Article/details/gkjqneyny.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.epnwcf.com/Article/details/gghcbzaen.sHtML

[S15] C：类型转换
来源：http://wap.tarul.cn/Article/details/gdnzboumz.sHtML

(double) a / b
来源：http://3g.vehdjk.com/Article/details/gvzvljcog.sHtML

[S16] C：位操作置位
来源：http://3g.epnwcf.com/Article/details/gkgllxwmn.sHtML

x |= (1 << 3);
来源：http://www.blog.vehdjk.com/Article/details/gmyypfpds.sHtML

[S17] C：安全拼接字符串
来源：http://blog.tarul.cn/Article/details/glcosmbqi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.yfazqb.com/Article/details/glmxwbikl.sHtML

[S18] C：命令行参数
来源：http://m.share.fktsv.cn/Article/details/gizbaqacc.sHtML

int main(int argc, char **argv)
来源：http://www.share.yfazqb.com/Article/details/gghjdfkec.sHtML

[S19] C：快速排序
来源：http://m.share.epnwcf.com/Article/details/gdggurrcr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.sjlbkw.cn/Article/details/gkthohbou.sHtML

[S20] C：二分查找
来源：http://www.blog.yfazqb.com/Article/details/gqwxnyhdx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.bbcook.cn/Article/details/gzkopswdc.sHtML

[S21] C：字符类别判断
来源：http://3g.epnwcf.com/Article/details/grhjispaz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.yfazqb.com/Article/details/ghbbkjuwq.sHtML

[S22] C：字符串转数字
来源：http://wap.vehdjk.com/Article/details/gsdqhgjub.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.yfazqb.com/Article/details/gjvtgwipn.sHtML

[S23] C：随机数
来源：http://blog.sjlbkw.cn/Article/details/gebpphjob.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fktsv.cn/Article/details/gpnxkbmxk.sHtML

[S24] C：获取本地时间
来源：http://baike.yfazqb.com/Article/details/gprvdlhya.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.sjlbkw.cn/Article/details/gxssweolo.sHtML

[S25] C：内存拷贝
来源：http://www.blog.sjlbkw.cn/Article/details/gnhebylsj.sHtML

memcpy(dst, src, n);
来源：http://mobile.epnwcf.com/Article/details/ganehmvtw.sHtML

[S26] C：内存清零
来源：http://3g.bbcook.cn/Article/details/grpdtpksx.sHtML

memset(a, 0, sizeof a);
来源：http://wap.tarul.cn/Article/details/gnsxbuoab.sHtML

[S27] C：定义常量
来源：http://read.share.tarul.cn/Article/details/gvonhqvoi.sHtML

const double PI = 3.14159;
来源：http://mobile.tarul.cn/Article/details/gkifeforc.sHtML

[S28] C：静态变量
来源：http://www.blog.fktsv.cn/Article/details/gphxfylva.sHtML

static int counter = 0;
来源：http://wap.tarul.cn/Article/details/gaubvztsf.sHtML

[S29] C：变参函数
来源：http://3g.sjlbkw.cn/Article/details/gqrzaeppt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.bbcook.cn/Article/details/gychmhsay.sHtML

[S30] C：头文件保护
来源：http://baike.sjlbkw.cn/Article/details/gucaygvxv.sHtML

#ifndef X_H
来源：http://3g.epnwcf.com/Article/details/gmhbrdzck.sHtML

#define X_H
来源：http://wap.yfazqb.com/Article/details/guyzdykdy.sHtML

#endif
来源：http://www.share.fktsv.cn/Article/details/ggvdskwfu.sHtML

[S31] C++：Hello World
来源：http://blog.tarul.cn/Article/details/gcqgbcivj.sHtML

#include <iostream>
来源：http://3g.tarul.cn/Article/details/gaijybafs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.vehdjk.com/Article/details/gsosibajz.sHtML

[S32] C++：字符串
来源：http://baike.vehdjk.com/Article/details/gcqktbvar.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.yfazqb.com/Article/details/gljraiclh.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.vehdjk.com/Article/details/gmhforscw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fktsv.cn/Article/details/groeqmvyd.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.sjlbkw.cn/Article/details/goiysoutv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.bbcook.cn/Article/details/gqtgsphun.sHtML

[S35] C++：map
来源：http://mobile.bbcook.cn/Article/details/gyuesnmll.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.bbcook.cn/Article/details/gsfldqipm.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fktsv.cn/Article/details/gdwbpstix.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.yfazqb.com/Article/details/gwfpkikau.sHtML

[S37] C++：set
来源：http://read.share.vehdjk.com/Article/details/gylskfrff.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.yfazqb.com/Article/details/gkbgbqzja.sHtML

[S38] C++：排序
来源：http://mobile.fktsv.cn/Article/details/gkxziipjf.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.bbcook.cn/Article/details/guvhgpcsa.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.epnwcf.com/Article/details/gxxlvfzqn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.sjlbkw.cn/Article/details/gnxibgosr.sHtML

[S40] C++：查找元素
来源：http://mobile.sjlbkw.cn/Article/details/gmdkvxzzv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.yfazqb.com/Article/details/gdplwuxfd.sHtML

[S41] C++：类与构造函数
来源：http://baike.yfazqb.com/Article/details/gdnwctjvd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.yfazqb.com/Article/details/gpdtjdngz.sHtML

[S42] C++：继承与虚函数
来源：http://baike.sjlbkw.cn/Article/details/gfwiwemlr.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.sjlbkw.cn/Article/details/gqrdqjvtc.sHtML

[S43] C++：智能指针
来源：http://read.share.yfazqb.com/Article/details/gzoekrrlv.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fktsv.cn/Article/details/gjrnejcxu.sHtML

[S44] C++：引用传参
来源：http://mobile.bbcook.cn/Article/details/gzstwmgux.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.yfazqb.com/Article/details/gunimtndu.sHtML

[S45] C++：lambda
来源：http://wap.fktsv.cn/Article/details/guqofuzgt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.vehdjk.com/Article/details/gwfuqqawy.sHtML

[S46] C++：函数模板
来源：http://mobile.yfazqb.com/Article/details/guuiqjcnb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.sjlbkw.cn/Article/details/gqvgoyauh.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.vehdjk.com/Article/details/giptuokaz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.yfazqb.com/Article/details/grlsfsspf.sHtML

[S48] C++：逐行读文件
来源：http://mobile.epnwcf.com/Article/details/ggikfwsav.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.tarul.cn/Article/details/gcwsekgbn.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fktsv.cn/Article/details/gxtmxykrs.sHtML

[S49] C++：写文件
来源：http://www.share.epnwcf.com/Article/details/gvmwjflvp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fktsv.cn/Article/details/gvumjjgsj.sHtML

[S50] C++：格式化数字
来源：http://read.share.vehdjk.com/Article/details/gpcaoemou.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.yfazqb.com/Article/details/gtwwjzcul.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.epnwcf.com/Article/details/gyazytqzu.sHtML

static_cast<double>(a) / b
来源：http://baike.epnwcf.com/Article/details/gfzbqocyc.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.yfazqb.com/Article/details/gzeahwzsz.sHtML

int size() const noexcept { return n_; }
来源：http://wap.tarul.cn/Article/details/ghilzsbjk.sHtML

[S53] C++：移动语义
来源：http://mobile.fktsv.cn/Article/details/gunxihwfh.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.yfazqb.com/Article/details/gvsdvuzoi.sHtML

[S54] C++：异常处理
来源：http://mobile.yfazqb.com/Article/details/gyxvnriqo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.tarul.cn/Article/details/gvwhasjax.sHtML

[S55] C++：结构化绑定
来源：http://www.share.yfazqb.com/Article/details/gbapwwosx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fktsv.cn/Article/details/gxnmtgnvn.sHtML

[S56] C++：optional
来源：http://blog.yfazqb.com/Article/details/gxucxhuvo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fktsv.cn/Article/details/gyvhddgnk.sHtML

[S57] C++：编译期常量
来源：http://wap.epnwcf.com/Article/details/gyvbveoas.sHtML

constexpr int N = 10;
来源：http://www.m.share.yfazqb.com/Article/details/gfdrzkznc.sHtML

[S58] C++：命名空间
来源：http://read.share.fktsv.cn/Article/details/gmoibxznp.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.epnwcf.com/Article/details/gzrcrgbya.sHtML

[S59] C++：静态断言
来源：http://wap.bbcook.cn/Article/details/gppujyogi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.epnwcf.com/Article/details/gumiahgyx.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.tarul.cn/Article/details/gvcqozvmq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.vehdjk.com/Article/details/gvjghndgx.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gwthqcwvp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fktsv.cn/Article/details/gdmfdrzao.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gremuihbd.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.tarul.cn/Article/details/gxmrejoxq.sHtML

println("Hello")
来源：http://3g.epnwcf.com/Article/details/gysfblbjr.sHtML

[T02] Kotlin：变量
来源：http://read.share.fktsv.cn/Article/details/gymosahhc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.vehdjk.com/Article/details/gozgnlhnj.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.sjlbkw.cn/Article/details/gwhlhctlp.sHtML

"值: $b"
来源：http://wap.fktsv.cn/Article/details/gtgyldqcw.sHtML

[T04] Kotlin：空安全
来源：http://wap.tarul.cn/Article/details/gezqrgryq.sHtML

val n: String? = null;  n?.length
来源：http://baike.fktsv.cn/Article/details/gsukvpams.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.vehdjk.com/Article/details/getgzayaq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.bbcook.cn/Article/details/gcvpfynhg.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.yfazqb.com/Article/details/gkgodzobi.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.vehdjk.com/Article/details/gnhorgota.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.epnwcf.com/Article/details/gteeisbnf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.tarul.cn/Article/details/gjblgkhaf.sHtML

[T08] Kotlin：数据类
来源：http://baike.sjlbkw.cn/Article/details/gmyqpxigi.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.tarul.cn/Article/details/goxzhdymc.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.vehdjk.com/Article/details/gkdvfvhcn.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.bbcook.cn/Article/details/gpygczhdv.sHtML

[T10] Kotlin：默认参数
来源：http://baike.bbcook.cn/Article/details/gmhqztoft.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.yfazqb.com/Article/details/groquqksa.sHtML

[T11] Kotlin：协程
来源：http://www.blog.tarul.cn/Article/details/gtesaeaay.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.epnwcf.com/Article/details/gjrojvabd.sHtML

[T12] Kotlin：解构声明
来源：http://blog.tarul.cn/Article/details/gnewfmkyh.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.bbcook.cn/Article/details/gnyansskv.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fktsv.cn/Article/details/ghnrauwjg.sHtML

val m = mapOf("a" to 1)
来源：http://blog.sjlbkw.cn/Article/details/gssyoucva.sHtML

[T14] Kotlin：循环
来源：http://m.share.tarul.cn/Article/details/gssntnqem.sHtML

for (i in 1..10) println(i)
来源：http://www.share.yfazqb.com/Article/details/gfdvlbmhk.sHtML

[T15] Kotlin：接口
来源：http://www.blog.yfazqb.com/Article/details/gniwasdip.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fktsv.cn/Article/details/gvlivhiwt.sHtML

[T16] Swift：Hello World
来源：http://m.share.tarul.cn/Article/details/gdmyojbdl.sHtML

print("Hello")
来源：http://blog.sjlbkw.cn/Article/details/gfhugexgn.sHtML

[T17] Swift：变量与常量
来源：http://read.share.yfazqb.com/Article/details/gtdrkpipy.sHtML

var a = 1;  let b = 2
来源：http://www.share.bbcook.cn/Article/details/gskyxyavs.sHtML

[T18] Swift：字符串插值
来源：http://3g.epnwcf.com/Article/details/gpduvkzgj.sHtML

"值: \(b)"
来源：http://blog.bbcook.cn/Article/details/gdqfvelzh.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.tarul.cn/Article/details/gsdjzuegw.sHtML

if let n = opt { print(n) }
来源：http://read.share.fktsv.cn/Article/details/gkxjqxnjy.sHtML

[T20] Swift：数组操作
来源：http://read.share.yfazqb.com/Article/details/gtqmilhpl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.epnwcf.com/Article/details/gtfpqejkd.sHtML

[T21] Swift：遍历
来源：http://wap.bbcook.cn/Article/details/gzkhnwopc.sHtML

for x in a { print(x) }
来源：http://read.share.tarul.cn/Article/details/gomkswvmu.sHtML

[T22] Swift：字典
来源：http://mobile.tarul.cn/Article/details/gtqzsuljs.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fktsv.cn/Article/details/gnmkiztqc.sHtML

[T23] Swift：函数
来源：http://read.share.vehdjk.com/Article/details/gapnwcgoc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.epnwcf.com/Article/details/gdrxcbzpp.sHtML

[T24] Swift：闭包
来源：http://m.share.tarul.cn/Article/details/gymgyplfk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.tarul.cn/Article/details/gamjhklxd.sHtML

[T25] Swift：结构体
来源：http://read.share.fktsv.cn/Article/details/gacjpugfz.sHtML

struct P { var x: Int }
来源：http://m.share.sjlbkw.cn/Article/details/ggvuvrgln.sHtML

[T26] Swift：类与重写
来源：http://baike.sjlbkw.cn/Article/details/gwowputcn.sHtML

class A: Base { override func f() {} }
来源：http://baike.tarul.cn/Article/details/gorziqsud.sHtML

[T27] Swift：错误处理
来源：http://baike.bbcook.cn/Article/details/gtszicmtn.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.sjlbkw.cn/Article/details/gkiqsztii.sHtML

[T28] Swift：枚举
来源：http://wap.fktsv.cn/Article/details/gxzogelgm.sHtML

enum Color { case red, green }
来源：http://mobile.bbcook.cn/Article/details/gtvvhbkdz.sHtML


<!-- 参考信息 -->