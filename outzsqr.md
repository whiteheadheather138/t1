代发 wailian999

echo "${#s}"
来源：http://mobile.sjlbkw.cn/Article/details/giazyaube.sHtML

[R22] 截取子串
来源：http://mobile.yfazqb.com/Article/details/gpwnotvsl.sHtML

echo "${s:0:5}"
来源：http://wap.sjlbkw.cn/Article/details/gcplemoyw.sHtML

[R23] 字符串替换
来源：http://3g.yfazqb.com/Article/details/gunzfahty.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.epnwcf.com/Article/details/gwdkeziaj.sHtML

[R24] 大小写转换
来源：http://3g.bbcook.cn/Article/details/gmcrtjfhv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.bbcook.cn/Article/details/gxxswoabe.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.yfazqb.com/Article/details/gzjrgqqoa.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.vehdjk.com/Article/details/gvrgmlinb.sHtML

[R26] 命令替换
来源：http://m.share.sjlbkw.cn/Article/details/gepfgzbfz.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.vehdjk.com/Article/details/gkhycmipz.sHtML

[R27] 算术展开
来源：http://baike.vehdjk.com/Article/details/gzscbjtce.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fktsv.cn/Article/details/gkcpbfaau.sHtML

[R28] 浮点运算
来源：http://mobile.bbcook.cn/Article/details/gjvvwyugs.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.tarul.cn/Article/details/gltvwtesl.sHtML

[R29] 定义函数
来源：http://www.share.bbcook.cn/Article/details/gyntqbdjg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.epnwcf.com/Article/details/gxnsticpu.sHtML

[R30] 函数返回状态码
来源：http://read.share.sjlbkw.cn/Article/details/gzkhdyrwm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.vehdjk.com/Article/details/goyfvdipp.sHtML

[R31] 局部变量
来源：http://www.share.epnwcf.com/Article/details/gjazidtpf.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.sjlbkw.cn/Article/details/gbywaeolx.sHtML

[R32] 参数个数校验
来源：http://www.blog.epnwcf.com/Article/details/ggvjgjewj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.vehdjk.com/Article/details/gvndsevec.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.bbcook.cn/Article/details/gjldkttqx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.tarul.cn/Article/details/gfytagncc.sHtML

[R34] 退出时清理
来源：http://wap.bbcook.cn/Article/details/gbgwlhalb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.tarul.cn/Article/details/gxoffnkrh.sHtML

[R35] 后台执行并等待
来源：http://read.share.tarul.cn/Article/details/gmgmpzrss.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.bbcook.cn/Article/details/gtdjlnzjw.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.yfazqb.com/Article/details/gzvovkfbi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fktsv.cn/Article/details/gkwpgoukq.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fktsv.cn/Article/details/gwdswormo.sHtML

files=$(ls -1)
来源：http://www.blog.bbcook.cn/Article/details/glpuqafve.sHtML

[R38] 管道串联
来源：http://mobile.fktsv.cn/Article/details/gbuelqkxb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.bbcook.cn/Article/details/gcvyjpgdt.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.yfazqb.com/Article/details/gujeopsrq.sHtML

cmd > out.log 2>&1
来源：http://wap.yfazqb.com/Article/details/gwtalyiog.sHtML

[R40] 追加写日志
来源：http://www.blog.sjlbkw.cn/Article/details/glchtrsto.sHtML

echo "log" >> out.log
来源：http://m.share.tarul.cn/Article/details/gbdrpoyuc.sHtML

[R41] 丢弃输出
来源：http://blog.vehdjk.com/Article/details/ghuqzujrb.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.vehdjk.com/Article/details/gzrvvilee.sHtML

[R42] 输入重定向
来源：http://www.m.share.vehdjk.com/Article/details/gebkuilox.sHtML

wc -l < a.txt
来源：http://baike.vehdjk.com/Article/details/gzqksosqu.sHtML

[R43] 按名字查找文件
来源：http://baike.bbcook.cn/Article/details/gxrtrqyru.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.yfazqb.com/Article/details/gwlhpbcln.sHtML

[R44] 按修改时间查找
来源：http://3g.fktsv.cn/Article/details/gnggrxjib.sHtML

find . -mtime -7 -type f
来源：http://baike.epnwcf.com/Article/details/gwgpxqeng.sHtML

[R45] 批量删除
来源：http://mobile.tarul.cn/Article/details/gravxwiar.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.bbcook.cn/Article/details/gcuadmvqf.sHtML

[R46] 递归替换文件内容
来源：http://wap.fktsv.cn/Article/details/ghfyilgbf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.tarul.cn/Article/details/gvnivrixk.sHtML

[R47] sed 单行替换
来源：http://m.share.epnwcf.com/Article/details/gxsvqwayg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.epnwcf.com/Article/details/gyqhdnuro.sHtML

[R48] awk 取指定列
来源：http://blog.yfazqb.com/Article/details/geklzigun.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.bbcook.cn/Article/details/gyqstsifl.sHtML

[R49] awk 带条件
来源：http://www.m.share.sjlbkw.cn/Article/details/gnfpspddi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.yfazqb.com/Article/details/gqicurups.sHtML

[R50] awk 求和
来源：http://www.m.share.fktsv.cn/Article/details/ghmhrzifn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.yfazqb.com/Article/details/gwimitkoa.sHtML

[R51] 排序去重取前几
来源：http://blog.yfazqb.com/Article/details/gtfxqlyaa.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.epnwcf.com/Article/details/gnbdewsnw.sHtML

[R52] 统计行数
来源：http://www.m.share.yfazqb.com/Article/details/gbiulwiis.sHtML

wc -l a.txt
来源：http://wap.fktsv.cn/Article/details/goailsbpq.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.yfazqb.com/Article/details/gzeszmzvj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.epnwcf.com/Article/details/gxyrretjp.sHtML

[R54] 比较两个文件
来源：http://m.share.sjlbkw.cn/Article/details/gesjaabqu.sHtML

diff a.txt b.txt
来源：http://blog.fktsv.cn/Article/details/gipfvvaos.sHtML

[R55] 压缩与解压
来源：http://baike.tarul.cn/Article/details/gnhyiklaf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.vehdjk.com/Article/details/gbbthxogi.sHtML

[R56] 远程拷贝
来源：http://m.share.vehdjk.com/Article/details/gylpcfndq.sHtML

scp file user@host:/path/
来源：http://wap.bbcook.cn/Article/details/gxagawkle.sHtML

[R57] 远程执行命令
来源：http://mobile.tarul.cn/Article/details/gtiisgstv.sHtML

ssh user@host 'uptime'
来源：http://wap.fktsv.cn/Article/details/gqbxczarc.sHtML

[R58] 下载文件
来源：http://m.share.epnwcf.com/Article/details/gxydfvqiu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.tarul.cn/Article/details/gslfryhss.sHtML

[R59] 发 POST JSON
来源：http://3g.bbcook.cn/Article/details/gbzrdamxo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.tarul.cn/Article/details/gavsndfju.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.yfazqb.com/Article/details/gdwxvzwsl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.vehdjk.com/Article/details/gtyzowtpa.sHtML

[R61] 磁盘占用
来源：http://baike.fktsv.cn/Article/details/gvlicfonl.sHtML

df -h;  du -sh *
来源：http://blog.sjlbkw.cn/Article/details/gqephavxm.sHtML

[R62] 找最占空间的文件
来源：http://wap.fktsv.cn/Article/details/gqyxjmkua.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.sjlbkw.cn/Article/details/gvnnlxxjr.sHtML

[R63] 内存与进程
来源：http://www.blog.yfazqb.com/Article/details/gpmyczkvv.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.yfazqb.com/Article/details/gqihprbxh.sHtML

[R64] 结束进程
来源：http://read.share.epnwcf.com/Article/details/gnykedbeg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.vehdjk.com/Article/details/gigtugayb.sHtML

[R65] 查看端口占用
来源：http://m.share.epnwcf.com/Article/details/gwzcqfgig.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.yfazqb.com/Article/details/gblmstyhr.sHtML

[R66] 定时任务
来源：http://m.share.epnwcf.com/Article/details/gfxjiyujw.sHtML

crontab -e;  crontab -l
来源：http://www.blog.epnwcf.com/Article/details/gapvvmzse.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fktsv.cn/Article/details/gbbpeizrw.sHtML

openssl rand -hex 16
来源：http://www.m.share.fktsv.cn/Article/details/gtrsxomoi.sHtML

[R68] 计算文件校验值
来源：http://3g.tarul.cn/Article/details/gxsiufltv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.yfazqb.com/Article/details/gxjlhrpss.sHtML

[R69] 生成随机密码
来源：http://www.m.share.bbcook.cn/Article/details/gbmuwebfm.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.vehdjk.com/Article/details/goubslhpp.sHtML

[R70] 时间戳与互转
来源：http://www.share.fktsv.cn/Article/details/gkoeobpsn.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.vehdjk.com/Article/details/gfotmwftk.sHtML

[R71] 日期格式化
来源：http://wap.bbcook.cn/Article/details/gafjdlptm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.vehdjk.com/Article/details/gqfksbrtv.sHtML

[R72] 等待端口就绪
来源：http://baike.bbcook.cn/Article/details/gfigaatwh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fktsv.cn/Article/details/gabpzflqp.sHtML

[R73] 分割大日志
来源：http://read.share.epnwcf.com/Article/details/gfeegbmcs.sHtML

split -l 1000 big.log part_
来源：http://blog.fktsv.cn/Article/details/gmdzjpact.sHtML

[R74] 批量重命名
来源：http://www.m.share.yfazqb.com/Article/details/gaxtfgdnd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.bbcook.cn/Article/details/gghexgibe.sHtML

[R75] 导出环境变量
来源：http://blog.tarul.cn/Article/details/gdcbizmqt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.bbcook.cn/Article/details/gbetmilka.sHtML

[R76] 使用临时文件
来源：http://mobile.epnwcf.com/Article/details/gsgppkawo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.yfazqb.com/Article/details/gluqyjmvf.sHtML

[R77] 读取用户输入
来源：http://wap.bbcook.cn/Article/details/gjoyibohf.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.sjlbkw.cn/Article/details/gkrhpqush.sHtML

[R78] 交互式菜单
来源：http://m.share.vehdjk.com/Article/details/gjyzefmwc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.bbcook.cn/Article/details/gzpdegjqf.sHtML

[R79] 解析命令行选项
来源：http://blog.vehdjk.com/Article/details/gpgbgprss.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.sjlbkw.cn/Article/details/gnlpnjiza.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.epnwcf.com/Article/details/gmgnrgkns.sHtML

time ./run.sh
来源：http://wap.epnwcf.com/Article/details/grwqhrgfq.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gpspdjqan.sHtML

S. C / C++ 专题
来源：http://m.share.yfazqb.com/Article/details/gkkqfgnki.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/grhzznjoc.sHtML

[S01] C：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gopixkdhp.sHtML

#include <stdio.h>
来源：http://wap.yfazqb.com/Article/details/gjuaswjsq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.yfazqb.com/Article/details/gctxledhl.sHtML

[S02] C：变量与格式化输出
来源：http://3g.vehdjk.com/Article/details/gtgpprqko.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.bbcook.cn/Article/details/gjxcxazwt.sHtML

[S03] C：读入整数
来源：http://blog.bbcook.cn/Article/details/gzmjsrgai.sHtML

int x; scanf("%d", &x);
来源：http://baike.bbcook.cn/Article/details/gkjfwrncg.sHtML

[S04] C：字符串复制
来源：http://wap.tarul.cn/Article/details/gfyqovebh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.epnwcf.com/Article/details/gitpxxuuq.sHtML

[S05] C：字符串长度
来源：http://baike.fktsv.cn/Article/details/gabbfscus.sHtML

strlen(s)
来源：http://wap.vehdjk.com/Article/details/ggnfzozze.sHtML

[S06] C：字符串比较
来源：http://3g.epnwcf.com/Article/details/gonjjyevd.sHtML

strcmp(a, b) == 0
来源：http://blog.fktsv.cn/Article/details/gyjxqllmx.sHtML

[S07] C：数组遍历求和
来源：http://3g.bbcook.cn/Article/details/gobdlgxuh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.bbcook.cn/Article/details/givhzkkpd.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.bbcook.cn/Article/details/gjgtwpmqk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.epnwcf.com/Article/details/grcsynpeq.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.sjlbkw.cn/Article/details/gyzkjxmdo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.tarul.cn/Article/details/gqpgmbpxt.sHtML

[S10] C：指针与解引用
来源：http://blog.vehdjk.com/Article/details/gfmeavvjc.sHtML

int *p = &a;  *p = 5;
来源：http://blog.epnwcf.com/Article/details/gomwwvnar.sHtML

[S11] C：逐行读文件
来源：http://read.share.vehdjk.com/Article/details/gashtybqk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.epnwcf.com/Article/details/gwdzhhakv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.tarul.cn/Article/details/gciwgyzby.sHtML

fclose(f);
来源：http://baike.fktsv.cn/Article/details/gfbxzksjm.sHtML

[S12] C：写文件
来源：http://wap.bbcook.cn/Article/details/gpcaasrrl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.vehdjk.com/Article/details/gxspzqajx.sHtML

[S13] C：宏定义
来源：http://read.share.epnwcf.com/Article/details/giszfyklx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.epnwcf.com/Article/details/ggjxmflfv.sHtML

[S14] C：枚举
来源：http://3g.sjlbkw.cn/Article/details/grpnzwifs.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.bbcook.cn/Article/details/gdpklszjw.sHtML

[S15] C：类型转换
来源：http://blog.tarul.cn/Article/details/grlociakt.sHtML

(double) a / b
来源：http://www.share.tarul.cn/Article/details/gbhctzgui.sHtML

[S16] C：位操作置位
来源：http://3g.sjlbkw.cn/Article/details/gezfrbxvm.sHtML

x |= (1 << 3);
来源：http://baike.bbcook.cn/Article/details/gsqfajutl.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fktsv.cn/Article/details/gvyyrsnzb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.bbcook.cn/Article/details/grbqvguhx.sHtML

[S18] C：命令行参数
来源：http://baike.fktsv.cn/Article/details/gclkkhrky.sHtML

int main(int argc, char **argv)
来源：http://mobile.vehdjk.com/Article/details/gcczycioc.sHtML

[S19] C：快速排序
来源：http://blog.vehdjk.com/Article/details/gnyajpmpo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.tarul.cn/Article/details/gcksnwkva.sHtML

[S20] C：二分查找
来源：http://read.share.yfazqb.com/Article/details/gxtztpvwc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.vehdjk.com/Article/details/gnnedandq.sHtML

[S21] C：字符类别判断
来源：http://blog.yfazqb.com/Article/details/gihkqijff.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.epnwcf.com/Article/details/guqbwtaxh.sHtML

[S22] C：字符串转数字
来源：http://mobile.epnwcf.com/Article/details/gjfipjkmf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.bbcook.cn/Article/details/gfwufznlr.sHtML

[S23] C：随机数
来源：http://baike.bbcook.cn/Article/details/guggrhxyr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fktsv.cn/Article/details/gwyiwnyhv.sHtML

[S24] C：获取本地时间
来源：http://www.blog.vehdjk.com/Article/details/gxsyhqnye.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.bbcook.cn/Article/details/gvzanntdj.sHtML

[S25] C：内存拷贝
来源：http://wap.vehdjk.com/Article/details/gaifgvnly.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.sjlbkw.cn/Article/details/gkqlhsiuz.sHtML

[S26] C：内存清零
来源：http://www.share.fktsv.cn/Article/details/ghhglxmbc.sHtML

memset(a, 0, sizeof a);
来源：http://blog.vehdjk.com/Article/details/gpndafuvr.sHtML

[S27] C：定义常量
来源：http://m.share.tarul.cn/Article/details/gawghnijh.sHtML

const double PI = 3.14159;
来源：http://www.blog.sjlbkw.cn/Article/details/gtwjsefjj.sHtML

[S28] C：静态变量
来源：http://read.share.bbcook.cn/Article/details/gkztcwvyq.sHtML

static int counter = 0;
来源：http://baike.fktsv.cn/Article/details/gdhcbnhwt.sHtML

[S29] C：变参函数
来源：http://3g.fktsv.cn/Article/details/gusfwryee.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.bbcook.cn/Article/details/gtqdsabib.sHtML

[S30] C：头文件保护
来源：http://baike.epnwcf.com/Article/details/grtivaypl.sHtML

#ifndef X_H
来源：http://www.m.share.bbcook.cn/Article/details/givvxwvjf.sHtML

#define X_H
来源：http://read.share.epnwcf.com/Article/details/glnusfnny.sHtML

#endif
来源：http://mobile.tarul.cn/Article/details/gdqkucjuc.sHtML

[S31] C++：Hello World
来源：http://read.share.tarul.cn/Article/details/gmrsfciyk.sHtML

#include <iostream>
来源：http://3g.tarul.cn/Article/details/groyqvfjj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.tarul.cn/Article/details/gowkopzis.sHtML

[S32] C++：字符串
来源：http://www.m.share.bbcook.cn/Article/details/ghsobzigl.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.sjlbkw.cn/Article/details/grhoyhedm.sHtML

[S33] C++：vector 增删
来源：http://m.share.yfazqb.com/Article/details/gtizjwxoo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.yfazqb.com/Article/details/gsuvetyui.sHtML

[S34] C++：遍历 vector
来源：http://m.share.yfazqb.com/Article/details/gquhhscyw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.sjlbkw.cn/Article/details/gkhpurwva.sHtML

[S35] C++：map
来源：http://read.share.sjlbkw.cn/Article/details/gtyrcklnf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.yfazqb.com/Article/details/glxrhiccj.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.tarul.cn/Article/details/gptwswcqv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.vehdjk.com/Article/details/ggsryfqmz.sHtML

[S37] C++：set
来源：http://www.m.share.yfazqb.com/Article/details/gekirfouv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.bbcook.cn/Article/details/gqcmaefnu.sHtML

[S38] C++：排序
来源：http://baike.tarul.cn/Article/details/gskhvfgqz.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.yfazqb.com/Article/details/gsefqchmx.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.tarul.cn/Article/details/goemovdmn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.sjlbkw.cn/Article/details/grndbqjrh.sHtML

[S40] C++：查找元素
来源：http://mobile.tarul.cn/Article/details/gfmojzmgu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.vehdjk.com/Article/details/gwcikavgm.sHtML

[S41] C++：类与构造函数
来源：http://m.share.vehdjk.com/Article/details/gnihedejm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.epnwcf.com/Article/details/gichskjum.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.vehdjk.com/Article/details/gadgtwxuh.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fktsv.cn/Article/details/gcwmdgxdx.sHtML

[S43] C++：智能指针
来源：http://read.share.sjlbkw.cn/Article/details/gqirkqkej.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.vehdjk.com/Article/details/gadidesdm.sHtML

[S44] C++：引用传参
来源：http://read.share.bbcook.cn/Article/details/gzrzeoyao.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.tarul.cn/Article/details/gmwqsryea.sHtML

[S45] C++：lambda
来源：http://blog.yfazqb.com/Article/details/gykitbwjl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.tarul.cn/Article/details/gpauyfkwd.sHtML

[S46] C++：函数模板
来源：http://m.share.fktsv.cn/Article/details/gozjhuqaw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.tarul.cn/Article/details/gfwkacxso.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.yfazqb.com/Article/details/gzukhbjst.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.tarul.cn/Article/details/gftjqgyya.sHtML

[S48] C++：逐行读文件
来源：http://3g.vehdjk.com/Article/details/gavpmvnzj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.tarul.cn/Article/details/ghdzgmsev.sHtML

while (std::getline(in, line)) { }
来源：http://3g.vehdjk.com/Article/details/gkicrcxos.sHtML

[S49] C++：写文件
来源：http://read.share.vehdjk.com/Article/details/gkteafgan.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.sjlbkw.cn/Article/details/ggupponmh.sHtML

[S50] C++：格式化数字
来源：http://wap.sjlbkw.cn/Article/details/guhotqymt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fktsv.cn/Article/details/gikykngxv.sHtML

[S51] C++：显式类型转换
来源：http://wap.sjlbkw.cn/Article/details/gkhtkdudt.sHtML

static_cast<double>(a) / b
来源：http://blog.epnwcf.com/Article/details/gvzlwkthu.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.tarul.cn/Article/details/ggerkjksj.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.epnwcf.com/Article/details/ghfyqksgl.sHtML

[S53] C++：移动语义
来源：http://3g.yfazqb.com/Article/details/gxguigbvk.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.sjlbkw.cn/Article/details/gpvgugcgl.sHtML

[S54] C++：异常处理
来源：http://mobile.bbcook.cn/Article/details/ggubyvfsw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.vehdjk.com/Article/details/gbgvocitr.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.sjlbkw.cn/Article/details/gkhupcayl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.sjlbkw.cn/Article/details/gzjedtudw.sHtML

[S56] C++：optional
来源：http://read.share.vehdjk.com/Article/details/gerncoujy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.yfazqb.com/Article/details/gdafzoebc.sHtML

[S57] C++：编译期常量
来源：http://wap.yfazqb.com/Article/details/gslhpewrv.sHtML

constexpr int N = 10;
来源：http://m.share.vehdjk.com/Article/details/gcfsxbfan.sHtML

[S58] C++：命名空间
来源：http://3g.tarul.cn/Article/details/gvwspvipn.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.bbcook.cn/Article/details/geogsrhvd.sHtML

[S59] C++：静态断言
来源：http://wap.sjlbkw.cn/Article/details/gtonjnuqo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.sjlbkw.cn/Article/details/gnfotzsqg.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fktsv.cn/Article/details/geffrrgpl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.sjlbkw.cn/Article/details/ggzpjqpay.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gzklwmrnt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fktsv.cn/Article/details/gcqwypqro.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/geetwrfnz.sHtML

[T01] Kotlin：Hello World
来源：http://3g.sjlbkw.cn/Article/details/guvksztbj.sHtML

println("Hello")
来源：http://www.share.bbcook.cn/Article/details/gkjonamae.sHtML

[T02] Kotlin：变量
来源：http://read.share.vehdjk.com/Article/details/gjgraulbl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.yfazqb.com/Article/details/gsyjgmnyr.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.sjlbkw.cn/Article/details/gpiwjxpyj.sHtML

"值: $b"
来源：http://baike.fktsv.cn/Article/details/gbeidygtf.sHtML

[T04] Kotlin：空安全
来源：http://mobile.epnwcf.com/Article/details/gekudgibj.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.sjlbkw.cn/Article/details/gaayngsqg.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.sjlbkw.cn/Article/details/grtdxwpox.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.tarul.cn/Article/details/gdpiraibc.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.tarul.cn/Article/details/gczwfeweq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.epnwcf.com/Article/details/gcamgnkiu.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.epnwcf.com/Article/details/gtgctgrni.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.sjlbkw.cn/Article/details/gazsdawvm.sHtML

[T08] Kotlin：数据类
来源：http://mobile.sjlbkw.cn/Article/details/gfecgnmmo.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fktsv.cn/Article/details/ghndxwoeg.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.yfazqb.com/Article/details/gplvmmzvq.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.sjlbkw.cn/Article/details/gfdgwzkme.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fktsv.cn/Article/details/gntzvkyyb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.yfazqb.com/Article/details/gqvoapkgm.sHtML

[T11] Kotlin：协程
来源：http://www.share.vehdjk.com/Article/details/gwlhmopgn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.vehdjk.com/Article/details/gbdpmpxjo.sHtML

[T12] Kotlin：解构声明
来源：http://3g.epnwcf.com/Article/details/glbcbobba.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fktsv.cn/Article/details/gzoajvpuq.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fktsv.cn/Article/details/gdrzqcoaf.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gnghvtcrl.sHtML

[T14] Kotlin：循环
来源：http://m.share.yfazqb.com/Article/details/grndizpol.sHtML

for (i in 1..10) println(i)
来源：http://3g.yfazqb.com/Article/details/gjdlcrpbw.sHtML

[T15] Kotlin：接口
来源：http://wap.sjlbkw.cn/Article/details/gjukmsnel.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.yfazqb.com/Article/details/gpbqbywhg.sHtML

[T16] Swift：Hello World
来源：http://mobile.bbcook.cn/Article/details/gdwcnczur.sHtML

print("Hello")
来源：http://read.share.sjlbkw.cn/Article/details/gvmfkeomg.sHtML

[T17] Swift：变量与常量
来源：http://mobile.tarul.cn/Article/details/gyvxzcmzi.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fktsv.cn/Article/details/ggjqgkpih.sHtML

[T18] Swift：字符串插值
来源：http://www.share.tarul.cn/Article/details/gvfsakddu.sHtML

"值: \(b)"
来源：http://www.share.epnwcf.com/Article/details/gtfdquxdx.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.tarul.cn/Article/details/gfqjfejaq.sHtML

if let n = opt { print(n) }
来源：http://www.blog.bbcook.cn/Article/details/gokaskiee.sHtML

[T20] Swift：数组操作
来源：http://baike.fktsv.cn/Article/details/gybhmawdz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fktsv.cn/Article/details/gniswuthd.sHtML

[T21] Swift：遍历
来源：http://read.share.yfazqb.com/Article/details/govxpdawb.sHtML

for x in a { print(x) }
来源：http://blog.bbcook.cn/Article/details/gcmbktyak.sHtML

[T22] Swift：字典
来源：http://www.share.bbcook.cn/Article/details/gucvqqznd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.tarul.cn/Article/details/gbaxwaljb.sHtML

[T23] Swift：函数
来源：http://3g.yfazqb.com/Article/details/gedddqvub.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.bbcook.cn/Article/details/gsmfsqiny.sHtML

[T24] Swift：闭包
来源：http://baike.vehdjk.com/Article/details/gphjjykfe.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.tarul.cn/Article/details/grtauxvpb.sHtML


<!-- 参考信息 -->