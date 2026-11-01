代发 wailian999

echo $((1 + 2 * 3))
来源：http://www.share.vehdjk.com/Article/details/gnkauxmdw.sHtML

[R28] 浮点运算
来源：http://blog.bbcook.cn/Article/details/gxscuzflh.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.vehdjk.com/Article/details/ggccmxyuo.sHtML

[R29] 定义函数
来源：http://www.m.share.fktsv.cn/Article/details/gbirkuoud.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.tarul.cn/Article/details/gtxozdaks.sHtML

[R30] 函数返回状态码
来源：http://read.share.epnwcf.com/Article/details/gzexyveja.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.yfazqb.com/Article/details/gdxllryqh.sHtML

[R31] 局部变量
来源：http://read.share.sjlbkw.cn/Article/details/gyfvwhpvh.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.vehdjk.com/Article/details/gxheexrwb.sHtML

[R32] 参数个数校验
来源：http://www.blog.yfazqb.com/Article/details/gmjbxhthp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkphrnsoi.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.sjlbkw.cn/Article/details/gunxkysun.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.yfazqb.com/Article/details/ggkrajkpt.sHtML

[R34] 退出时清理
来源：http://www.blog.vehdjk.com/Article/details/gbgtstnno.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.yfazqb.com/Article/details/glpgalnxf.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.epnwcf.com/Article/details/gkwqmvxjn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.epnwcf.com/Article/details/ggkknggbe.sHtML

[R36] 并发执行多个任务
来源：http://blog.yfazqb.com/Article/details/gntrpxpyt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.epnwcf.com/Article/details/gejxslvra.sHtML

[R37] 把输出赋给变量
来源：http://3g.vehdjk.com/Article/details/gvplqfici.sHtML

files=$(ls -1)
来源：http://wap.bbcook.cn/Article/details/gwlkdhdzt.sHtML

[R38] 管道串联
来源：http://www.blog.sjlbkw.cn/Article/details/gxmkwwvcx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.sjlbkw.cn/Article/details/gknriuzkc.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.yfazqb.com/Article/details/gdutgcdcs.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fktsv.cn/Article/details/ggwxotyzm.sHtML

[R40] 追加写日志
来源：http://www.share.yfazqb.com/Article/details/gjtebzvyy.sHtML

echo "log" >> out.log
来源：http://www.blog.vehdjk.com/Article/details/glxzpencw.sHtML

[R41] 丢弃输出
来源：http://www.m.share.sjlbkw.cn/Article/details/gssfinwsa.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.bbcook.cn/Article/details/gzxfdgaeh.sHtML

[R42] 输入重定向
来源：http://read.share.epnwcf.com/Article/details/gxxcdpqxd.sHtML

wc -l < a.txt
来源：http://mobile.tarul.cn/Article/details/gucusgptv.sHtML

[R43] 按名字查找文件
来源：http://read.share.fktsv.cn/Article/details/gfymqwdtm.sHtML

find . -name "*.log" -type f
来源：http://3g.fktsv.cn/Article/details/gnjoowfzw.sHtML

[R44] 按修改时间查找
来源：http://www.share.vehdjk.com/Article/details/gsqbokovf.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fktsv.cn/Article/details/gyyknljwm.sHtML

[R45] 批量删除
来源：http://www.m.share.vehdjk.com/Article/details/goqtjtayd.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.bbcook.cn/Article/details/gblbgiost.sHtML

[R46] 递归替换文件内容
来源：http://m.share.tarul.cn/Article/details/gizwkpgkf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.epnwcf.com/Article/details/gtksuphbt.sHtML

[R47] sed 单行替换
来源：http://mobile.yfazqb.com/Article/details/gmcvfwscw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.tarul.cn/Article/details/gzhaunfxz.sHtML

[R48] awk 取指定列
来源：http://m.share.fktsv.cn/Article/details/gtkayphky.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.tarul.cn/Article/details/gqeiuoftp.sHtML

[R49] awk 带条件
来源：http://read.share.fktsv.cn/Article/details/gnypxnwou.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fktsv.cn/Article/details/glgvkpafh.sHtML

[R50] awk 求和
来源：http://www.share.bbcook.cn/Article/details/gykshulms.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.sjlbkw.cn/Article/details/gfmzgfxfa.sHtML

[R51] 排序去重取前几
来源：http://m.share.sjlbkw.cn/Article/details/gdlfchigg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.sjlbkw.cn/Article/details/gkcjehcbv.sHtML

[R52] 统计行数
来源：http://blog.sjlbkw.cn/Article/details/gdyaqjhad.sHtML

wc -l a.txt
来源：http://m.share.yfazqb.com/Article/details/gbmsfghyd.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.bbcook.cn/Article/details/gnfhiwkqo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.sjlbkw.cn/Article/details/gkerazaeo.sHtML

[R54] 比较两个文件
来源：http://www.share.bbcook.cn/Article/details/goevhvqia.sHtML

diff a.txt b.txt
来源：http://www.share.fktsv.cn/Article/details/gqlijspeu.sHtML

[R55] 压缩与解压
来源：http://baike.sjlbkw.cn/Article/details/gfirppruh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.vehdjk.com/Article/details/glcorsmcr.sHtML

[R56] 远程拷贝
来源：http://www.blog.sjlbkw.cn/Article/details/gmrioqvws.sHtML

scp file user@host:/path/
来源：http://baike.yfazqb.com/Article/details/gycrbljgg.sHtML

[R57] 远程执行命令
来源：http://www.m.share.sjlbkw.cn/Article/details/gygdpqcts.sHtML

ssh user@host 'uptime'
来源：http://mobile.tarul.cn/Article/details/geajcxkpy.sHtML

[R58] 下载文件
来源：http://www.share.vehdjk.com/Article/details/gjxbdwkqo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.vehdjk.com/Article/details/gqsvibtbc.sHtML

[R59] 发 POST JSON
来源：http://www.blog.tarul.cn/Article/details/gbhwvjnew.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.bbcook.cn/Article/details/grloolhkw.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.vehdjk.com/Article/details/gertwpslg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.yfazqb.com/Article/details/gqyyjufos.sHtML

[R61] 磁盘占用
来源：http://baike.bbcook.cn/Article/details/gqtsbacsl.sHtML

df -h;  du -sh *
来源：http://baike.epnwcf.com/Article/details/gpvmsxqoc.sHtML

[R62] 找最占空间的文件
来源：http://mobile.epnwcf.com/Article/details/gjtvxbswv.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.epnwcf.com/Article/details/gxpyqaoaw.sHtML

[R63] 内存与进程
来源：http://blog.tarul.cn/Article/details/gubwktfvb.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fktsv.cn/Article/details/grvhaxdwa.sHtML

[R64] 结束进程
来源：http://baike.yfazqb.com/Article/details/gbtdkvzoa.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fktsv.cn/Article/details/gqdatqcql.sHtML

[R65] 查看端口占用
来源：http://wap.sjlbkw.cn/Article/details/gugjsitvf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.tarul.cn/Article/details/gsqmlgczq.sHtML

[R66] 定时任务
来源：http://wap.vehdjk.com/Article/details/gyhshbrzf.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.tarul.cn/Article/details/gqomwntdp.sHtML

[R67] 生成随机十六进制串
来源：http://wap.bbcook.cn/Article/details/gwntgxguc.sHtML

openssl rand -hex 16
来源：http://3g.sjlbkw.cn/Article/details/gjijsqrtf.sHtML

[R68] 计算文件校验值
来源：http://3g.yfazqb.com/Article/details/gnlkaihjh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.vehdjk.com/Article/details/guhjcsxna.sHtML

[R69] 生成随机密码
来源：http://www.blog.sjlbkw.cn/Article/details/gpmjuyxjp.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fktsv.cn/Article/details/gjmtqyufr.sHtML

[R70] 时间戳与互转
来源：http://3g.fktsv.cn/Article/details/gyudsbqgn.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.sjlbkw.cn/Article/details/gotoeaqtr.sHtML

[R71] 日期格式化
来源：http://3g.epnwcf.com/Article/details/gfehrxaac.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.epnwcf.com/Article/details/gvbrjbjbz.sHtML

[R72] 等待端口就绪
来源：http://blog.sjlbkw.cn/Article/details/gicmxxszs.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.vehdjk.com/Article/details/gbnfzlrbo.sHtML

[R73] 分割大日志
来源：http://blog.epnwcf.com/Article/details/gathdbnrq.sHtML

split -l 1000 big.log part_
来源：http://blog.epnwcf.com/Article/details/guxroehut.sHtML

[R74] 批量重命名
来源：http://mobile.epnwcf.com/Article/details/girhhnzps.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.yfazqb.com/Article/details/gwwrdklhg.sHtML

[R75] 导出环境变量
来源：http://wap.tarul.cn/Article/details/gvnidxalm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.vehdjk.com/Article/details/gdvmwzbzu.sHtML

[R76] 使用临时文件
来源：http://m.share.vehdjk.com/Article/details/gwcdzcicc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.sjlbkw.cn/Article/details/gblukalti.sHtML

[R77] 读取用户输入
来源：http://m.share.tarul.cn/Article/details/giszjrege.sHtML

read -rp "请输入: " ans
来源：http://mobile.bbcook.cn/Article/details/givohjgvg.sHtML

[R78] 交互式菜单
来源：http://baike.sjlbkw.cn/Article/details/gyxfofefa.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.vehdjk.com/Article/details/grfoqsgnm.sHtML

[R79] 解析命令行选项
来源：http://wap.bbcook.cn/Article/details/ggycaiqxl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fktsv.cn/Article/details/gpijrmzfi.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.bbcook.cn/Article/details/gicwgswcb.sHtML

time ./run.sh
来源：http://www.share.sjlbkw.cn/Article/details/ganmbnypp.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gtrbeugvs.sHtML

S. C / C++ 专题
来源：http://baike.epnwcf.com/Article/details/gwjtolclk.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gtmaosscw.sHtML

[S01] C：Hello World
来源：http://www.m.share.epnwcf.com/Article/details/glbwmbrxw.sHtML

#include <stdio.h>
来源：http://www.blog.tarul.cn/Article/details/gaxrzkeer.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.bbcook.cn/Article/details/gsgxvcwoh.sHtML

[S02] C：变量与格式化输出
来源：http://baike.tarul.cn/Article/details/gicpavfuc.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.vehdjk.com/Article/details/gxcbnwrhy.sHtML

[S03] C：读入整数
来源：http://www.m.share.bbcook.cn/Article/details/grvocvioc.sHtML

int x; scanf("%d", &x);
来源：http://wap.tarul.cn/Article/details/gcnmwthtn.sHtML

[S04] C：字符串复制
来源：http://mobile.sjlbkw.cn/Article/details/gxuoopuzk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.bbcook.cn/Article/details/gtthrxoxm.sHtML

[S05] C：字符串长度
来源：http://m.share.vehdjk.com/Article/details/gfvbhwzud.sHtML

strlen(s)
来源：http://read.share.fktsv.cn/Article/details/ggbnbocsg.sHtML

[S06] C：字符串比较
来源：http://3g.bbcook.cn/Article/details/ggpvadxyt.sHtML

strcmp(a, b) == 0
来源：http://baike.sjlbkw.cn/Article/details/gcbuqrhsr.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.sjlbkw.cn/Article/details/gdjprtuik.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fktsv.cn/Article/details/gfxispyux.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.bbcook.cn/Article/details/gwkznqasw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.epnwcf.com/Article/details/gjdzxvcaz.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.epnwcf.com/Article/details/gstsrwdxg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.vehdjk.com/Article/details/gbharalpm.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fktsv.cn/Article/details/gmozbebqr.sHtML

int *p = &a;  *p = 5;
来源：http://3g.tarul.cn/Article/details/gtjyqlast.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.epnwcf.com/Article/details/gfyneikkv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.bbcook.cn/Article/details/gknbhttre.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.epnwcf.com/Article/details/gixcnumwj.sHtML

fclose(f);
来源：http://www.blog.tarul.cn/Article/details/gnqtveqka.sHtML

[S12] C：写文件
来源：http://read.share.yfazqb.com/Article/details/gmtnedkev.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.epnwcf.com/Article/details/gjfaphbhm.sHtML

[S13] C：宏定义
来源：http://baike.epnwcf.com/Article/details/gjvrrltiu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.yfazqb.com/Article/details/ghfstrnne.sHtML

[S14] C：枚举
来源：http://read.share.bbcook.cn/Article/details/gphdfcfjg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.bbcook.cn/Article/details/ghentmboz.sHtML

[S15] C：类型转换
来源：http://baike.epnwcf.com/Article/details/ggpvkxgdg.sHtML

(double) a / b
来源：http://read.share.sjlbkw.cn/Article/details/gopnswgow.sHtML

[S16] C：位操作置位
来源：http://m.share.epnwcf.com/Article/details/gibcvcney.sHtML

x |= (1 << 3);
来源：http://baike.bbcook.cn/Article/details/gvjrrkyrx.sHtML

[S17] C：安全拼接字符串
来源：http://blog.bbcook.cn/Article/details/gvaupvovm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.sjlbkw.cn/Article/details/guydhndin.sHtML

[S18] C：命令行参数
来源：http://www.blog.vehdjk.com/Article/details/grfsznpff.sHtML

int main(int argc, char **argv)
来源：http://mobile.vehdjk.com/Article/details/glljxstxp.sHtML

[S19] C：快速排序
来源：http://blog.sjlbkw.cn/Article/details/gguqhtern.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.bbcook.cn/Article/details/gqycdgcqw.sHtML

[S20] C：二分查找
来源：http://m.share.vehdjk.com/Article/details/gmcurdhit.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.yfazqb.com/Article/details/gqqsxaxwa.sHtML

[S21] C：字符类别判断
来源：http://mobile.vehdjk.com/Article/details/goikjezkf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.tarul.cn/Article/details/grovwedlt.sHtML

[S22] C：字符串转数字
来源：http://3g.bbcook.cn/Article/details/gpynkouwe.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.sjlbkw.cn/Article/details/gvqrdgclb.sHtML

[S23] C：随机数
来源：http://m.share.yfazqb.com/Article/details/gyiefklir.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.vehdjk.com/Article/details/gpmumffpd.sHtML

[S24] C：获取本地时间
来源：http://baike.vehdjk.com/Article/details/gjozfkjze.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.bbcook.cn/Article/details/gyqhdeunn.sHtML

[S25] C：内存拷贝
来源：http://www.blog.tarul.cn/Article/details/gypybiisg.sHtML

memcpy(dst, src, n);
来源：http://wap.yfazqb.com/Article/details/gnhnskfnj.sHtML

[S26] C：内存清零
来源：http://read.share.vehdjk.com/Article/details/gaaulbjvr.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.vehdjk.com/Article/details/gvnkbjkzj.sHtML

[S27] C：定义常量
来源：http://m.share.tarul.cn/Article/details/gsjtmxbka.sHtML

const double PI = 3.14159;
来源：http://read.share.vehdjk.com/Article/details/gzioycnhv.sHtML

[S28] C：静态变量
来源：http://www.m.share.tarul.cn/Article/details/ghiuajrdc.sHtML

static int counter = 0;
来源：http://wap.sjlbkw.cn/Article/details/grdrhvpgl.sHtML

[S29] C：变参函数
来源：http://www.blog.sjlbkw.cn/Article/details/gtmlvnpct.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.bbcook.cn/Article/details/gruczkoyi.sHtML

[S30] C：头文件保护
来源：http://read.share.tarul.cn/Article/details/ghkwvqmfg.sHtML

#ifndef X_H
来源：http://wap.vehdjk.com/Article/details/gllmneuoc.sHtML

#define X_H
来源：http://3g.tarul.cn/Article/details/gcgppyuov.sHtML

#endif
来源：http://m.share.tarul.cn/Article/details/gqzbdbown.sHtML

[S31] C++：Hello World
来源：http://www.m.share.epnwcf.com/Article/details/gszyvphqi.sHtML

#include <iostream>
来源：http://wap.vehdjk.com/Article/details/gnmaxgwnl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.bbcook.cn/Article/details/gahuycbzw.sHtML

[S32] C++：字符串
来源：http://www.m.share.fktsv.cn/Article/details/gnqnzhjvw.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.epnwcf.com/Article/details/gwiwmteeb.sHtML

[S33] C++：vector 增删
来源：http://m.share.vehdjk.com/Article/details/grwhiaxpr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.bbcook.cn/Article/details/gwtrgcdth.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.vehdjk.com/Article/details/gdeuzolfk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.tarul.cn/Article/details/gzoodvchu.sHtML

[S35] C++：map
来源：http://blog.fktsv.cn/Article/details/gzfpocbru.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.tarul.cn/Article/details/giolwzknc.sHtML

[S36] C++：unordered_map
来源：http://3g.vehdjk.com/Article/details/gshuxrurp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.sjlbkw.cn/Article/details/gayamehbx.sHtML

[S37] C++：set
来源：http://mobile.tarul.cn/Article/details/grpmhwntb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.vehdjk.com/Article/details/gipsvtfsx.sHtML

[S38] C++：排序
来源：http://baike.vehdjk.com/Article/details/govjoidbf.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.yfazqb.com/Article/details/gjdkhbetn.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.tarul.cn/Article/details/gejwnrcrh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.yfazqb.com/Article/details/gzorbkenv.sHtML

[S40] C++：查找元素
来源：http://read.share.yfazqb.com/Article/details/gblnecswy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.bbcook.cn/Article/details/gtxcvulgt.sHtML

[S41] C++：类与构造函数
来源：http://mobile.epnwcf.com/Article/details/goiqlihbf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.epnwcf.com/Article/details/ghbfwudxx.sHtML

[S42] C++：继承与虚函数
来源：http://3g.epnwcf.com/Article/details/glmudaknt.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.yfazqb.com/Article/details/gqfrqimmq.sHtML

[S43] C++：智能指针
来源：http://mobile.fktsv.cn/Article/details/gygymfspv.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.vehdjk.com/Article/details/gkzeekmsu.sHtML

[S44] C++：引用传参
来源：http://www.share.tarul.cn/Article/details/gcpkmhesp.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.tarul.cn/Article/details/gwucgwsxq.sHtML

[S45] C++：lambda
来源：http://blog.sjlbkw.cn/Article/details/gahneoenm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.bbcook.cn/Article/details/ghmnuenwu.sHtML

[S46] C++：函数模板
来源：http://3g.vehdjk.com/Article/details/grhbvnlhu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.vehdjk.com/Article/details/gbdhmtlrm.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.vehdjk.com/Article/details/gmokspfwi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fktsv.cn/Article/details/gabbitaon.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.vehdjk.com/Article/details/gdnjlkrzq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.epnwcf.com/Article/details/gtqkfrgrc.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.epnwcf.com/Article/details/gisookehe.sHtML

[S49] C++：写文件
来源：http://baike.sjlbkw.cn/Article/details/gvsrzctqm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.bbcook.cn/Article/details/gkazgvpgv.sHtML

[S50] C++：格式化数字
来源：http://www.share.bbcook.cn/Article/details/gvpkhggbo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.yfazqb.com/Article/details/gmsdxwwba.sHtML

[S51] C++：显式类型转换
来源：http://mobile.bbcook.cn/Article/details/gdxmnfcjm.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.bbcook.cn/Article/details/gkoflxizb.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.epnwcf.com/Article/details/givjoqkqn.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fktsv.cn/Article/details/gcrdzqqha.sHtML

[S53] C++：移动语义
来源：http://baike.sjlbkw.cn/Article/details/gxauqhxsf.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.yfazqb.com/Article/details/ggxkjioov.sHtML

[S54] C++：异常处理
来源：http://www.m.share.sjlbkw.cn/Article/details/geqrdnvkv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fktsv.cn/Article/details/gpzbjwmis.sHtML

[S55] C++：结构化绑定
来源：http://wap.vehdjk.com/Article/details/ghwgondtx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.vehdjk.com/Article/details/gnynjltdu.sHtML

[S56] C++：optional
来源：http://www.m.share.yfazqb.com/Article/details/gtrqryrue.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.bbcook.cn/Article/details/gnwvppisi.sHtML

[S57] C++：编译期常量
来源：http://3g.bbcook.cn/Article/details/ggocpnlyq.sHtML

constexpr int N = 10;
来源：http://www.m.share.sjlbkw.cn/Article/details/gxkmpubva.sHtML

[S58] C++：命名空间
来源：http://www.m.share.yfazqb.com/Article/details/gtelupmqx.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.tarul.cn/Article/details/gikbtfsjk.sHtML

[S59] C++：静态断言
来源：http://www.blog.yfazqb.com/Article/details/gbqxulxhr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.yfazqb.com/Article/details/gibfpivtg.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.bbcook.cn/Article/details/gpmfehgcf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.epnwcf.com/Article/details/ggyurcjlb.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gjvmxeqcb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.yfazqb.com/Article/details/gkvjpkhky.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gvlfyihzr.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.epnwcf.com/Article/details/gycbfxewo.sHtML

println("Hello")
来源：http://www.blog.epnwcf.com/Article/details/gtvglzqyt.sHtML

[T02] Kotlin：变量
来源：http://www.blog.vehdjk.com/Article/details/gddsjncys.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.bbcook.cn/Article/details/gmrnqynya.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.yfazqb.com/Article/details/gcyfbshzb.sHtML

"值: $b"
来源：http://read.share.sjlbkw.cn/Article/details/gtrbpgbfl.sHtML

[T04] Kotlin：空安全
来源：http://m.share.yfazqb.com/Article/details/gwuaovgon.sHtML

val n: String? = null;  n?.length
来源：http://3g.fktsv.cn/Article/details/geuwvxjhd.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.epnwcf.com/Article/details/gymaotvrf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.bbcook.cn/Article/details/gmafwdhtz.sHtML

[T06] Kotlin：集合映射
来源：http://blog.sjlbkw.cn/Article/details/gqgvktbkm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.epnwcf.com/Article/details/gxicqsoar.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.vehdjk.com/Article/details/gaetltdas.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.bbcook.cn/Article/details/gaozlqgrr.sHtML

[T08] Kotlin：数据类
来源：http://baike.vehdjk.com/Article/details/gwtgiiayd.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.vehdjk.com/Article/details/gjbajgtkk.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.tarul.cn/Article/details/gktpvuwsm.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.sjlbkw.cn/Article/details/gqvgonixj.sHtML

[T10] Kotlin：默认参数
来源：http://wap.yfazqb.com/Article/details/gmpayocei.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.epnwcf.com/Article/details/gitdctang.sHtML

[T11] Kotlin：协程
来源：http://www.blog.vehdjk.com/Article/details/gpaopwjlr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.epnwcf.com/Article/details/ghlqzazxw.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.tarul.cn/Article/details/ggnlbiden.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.epnwcf.com/Article/details/ggclwvrdh.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.sjlbkw.cn/Article/details/gpznzyixk.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.tarul.cn/Article/details/gvypjfftx.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.epnwcf.com/Article/details/ggvjcaelg.sHtML

for (i in 1..10) println(i)
来源：http://3g.bbcook.cn/Article/details/gwsrmcqrm.sHtML

[T15] Kotlin：接口
来源：http://blog.vehdjk.com/Article/details/gfrldjyyp.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxbhywnrw.sHtML

[T16] Swift：Hello World
来源：http://blog.sjlbkw.cn/Article/details/guvtwewvm.sHtML

print("Hello")
来源：http://mobile.vehdjk.com/Article/details/gofdbcxdp.sHtML

[T17] Swift：变量与常量
来源：http://m.share.yfazqb.com/Article/details/gduvakcpm.sHtML

var a = 1;  let b = 2
来源：http://baike.bbcook.cn/Article/details/ggmfrstsl.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.vehdjk.com/Article/details/gqgmqigse.sHtML

"值: \(b)"
来源：http://wap.vehdjk.com/Article/details/gxwynmdor.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.vehdjk.com/Article/details/gtrdwxwal.sHtML

if let n = opt { print(n) }
来源：http://wap.bbcook.cn/Article/details/gffvrrzjj.sHtML

[T20] Swift：数组操作
来源：http://baike.sjlbkw.cn/Article/details/gwbwizpba.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.vehdjk.com/Article/details/gzytplccx.sHtML

[T21] Swift：遍历
来源：http://read.share.vehdjk.com/Article/details/gzrkieyig.sHtML

for x in a { print(x) }
来源：http://www.share.vehdjk.com/Article/details/ggzzdrmhq.sHtML

[T22] Swift：字典
来源：http://m.share.epnwcf.com/Article/details/gxcakergt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.sjlbkw.cn/Article/details/giyrbxzdh.sHtML

[T23] Swift：函数
来源：http://www.share.yfazqb.com/Article/details/gyahsntzr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.vehdjk.com/Article/details/gdjbdntge.sHtML

[T24] Swift：闭包
来源：http://www.share.epnwcf.com/Article/details/gzjvcbswu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.sjlbkw.cn/Article/details/gbxevyrwj.sHtML

[T25] Swift：结构体
来源：http://wap.fktsv.cn/Article/details/gbzaiysku.sHtML

struct P { var x: Int }
来源：http://mobile.sjlbkw.cn/Article/details/guuomemdv.sHtML

[T26] Swift：类与重写
来源：http://mobile.sjlbkw.cn/Article/details/gnmdtorkz.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.bbcook.cn/Article/details/ghvulzmms.sHtML

[T27] Swift：错误处理
来源：http://read.share.fktsv.cn/Article/details/gdagzbiyu.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.bbcook.cn/Article/details/gdzllvypv.sHtML

[T28] Swift：枚举
来源：http://read.share.bbcook.cn/Article/details/gxiipponv.sHtML

enum Color { case red, green }
来源：http://baike.epnwcf.com/Article/details/grosxeblu.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.bbcook.cn/Article/details/grqowlkjh.sHtML

guard let x = opt else { return }
来源：http://mobile.fktsv.cn/Article/details/gmltsppoo.sHtML

[T30] Swift：协议
来源：http://3g.fktsv.cn/Article/details/gdcjnixoy.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fktsv.cn/Article/details/gnfpbdtrm.sHtML


<!-- 参考信息 -->