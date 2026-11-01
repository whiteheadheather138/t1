代发 wailian999

echo $((1 + 2 * 3))
来源：http://www.blog.bbcook.cn/Article/details/gjvvhtmqo.sHtML

[R28] 浮点运算
来源：http://read.share.bbcook.cn/Article/details/giqqhrloj.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.sjlbkw.cn/Article/details/gpbhkjlmy.sHtML

[R29] 定义函数
来源：http://blog.sjlbkw.cn/Article/details/gsliqboud.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.vehdjk.com/Article/details/gcijeppiz.sHtML

[R30] 函数返回状态码
来源：http://baike.tarul.cn/Article/details/gcjdroyha.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.vehdjk.com/Article/details/gyvclxdjv.sHtML

[R31] 局部变量
来源：http://baike.tarul.cn/Article/details/ghsxmkkpo.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.tarul.cn/Article/details/gmoohxkzy.sHtML

[R32] 参数个数校验
来源：http://blog.yfazqb.com/Article/details/gbfnpwyvc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.tarul.cn/Article/details/gnkiwfrqs.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fktsv.cn/Article/details/gscagsqmr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.epnwcf.com/Article/details/gjvesexqz.sHtML

[R34] 退出时清理
来源：http://mobile.yfazqb.com/Article/details/gzzjmnoxs.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.yfazqb.com/Article/details/gwdrflpax.sHtML

[R35] 后台执行并等待
来源：http://www.share.epnwcf.com/Article/details/gjoseiqta.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.bbcook.cn/Article/details/gvwakpzly.sHtML

[R36] 并发执行多个任务
来源：http://read.share.tarul.cn/Article/details/gzxwzjiza.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.bbcook.cn/Article/details/gbjjcacsm.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.tarul.cn/Article/details/gbltpcrqe.sHtML

files=$(ls -1)
来源：http://blog.yfazqb.com/Article/details/gyazagopd.sHtML

[R38] 管道串联
来源：http://mobile.sjlbkw.cn/Article/details/gmpmjrhpd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fktsv.cn/Article/details/gbkkhuixc.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.sjlbkw.cn/Article/details/ghuqqjdmq.sHtML

cmd > out.log 2>&1
来源：http://wap.sjlbkw.cn/Article/details/gjtfbqmrp.sHtML

[R40] 追加写日志
来源：http://mobile.sjlbkw.cn/Article/details/gcesbnylm.sHtML

echo "log" >> out.log
来源：http://m.share.sjlbkw.cn/Article/details/gpoelfkiz.sHtML

[R41] 丢弃输出
来源：http://read.share.sjlbkw.cn/Article/details/gbsopoapf.sHtML

cmd >/dev/null 2>&1
来源：http://wap.vehdjk.com/Article/details/gxrqtvcqm.sHtML

[R42] 输入重定向
来源：http://read.share.yfazqb.com/Article/details/gneptqzyf.sHtML

wc -l < a.txt
来源：http://www.blog.tarul.cn/Article/details/geqenuorz.sHtML

[R43] 按名字查找文件
来源：http://3g.yfazqb.com/Article/details/gxheylpcg.sHtML

find . -name "*.log" -type f
来源：http://wap.sjlbkw.cn/Article/details/ggvhcmcig.sHtML

[R44] 按修改时间查找
来源：http://www.blog.epnwcf.com/Article/details/gvdkxkyap.sHtML

find . -mtime -7 -type f
来源：http://m.share.bbcook.cn/Article/details/geqibmtvo.sHtML

[R45] 批量删除
来源：http://www.blog.fktsv.cn/Article/details/gazpgstko.sHtML

find . -name "*.tmp" -delete
来源：http://3g.vehdjk.com/Article/details/ggobkfmlq.sHtML

[R46] 递归替换文件内容
来源：http://blog.vehdjk.com/Article/details/grozowmqj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.yfazqb.com/Article/details/gskcidrgz.sHtML

[R47] sed 单行替换
来源：http://3g.vehdjk.com/Article/details/gzdfbdytv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.bbcook.cn/Article/details/grqhbuquq.sHtML

[R48] awk 取指定列
来源：http://3g.vehdjk.com/Article/details/gwzesllbp.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.vehdjk.com/Article/details/gzfgvskzr.sHtML

[R49] awk 带条件
来源：http://www.blog.sjlbkw.cn/Article/details/gmevhdsbo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.bbcook.cn/Article/details/gqhadpxxz.sHtML

[R50] awk 求和
来源：http://baike.epnwcf.com/Article/details/gnqjtogbb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.epnwcf.com/Article/details/gonjmkjox.sHtML

[R51] 排序去重取前几
来源：http://m.share.yfazqb.com/Article/details/grseccoxq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fktsv.cn/Article/details/glyvfsnnv.sHtML

[R52] 统计行数
来源：http://www.blog.bbcook.cn/Article/details/gvsqgwskc.sHtML

wc -l a.txt
来源：http://wap.bbcook.cn/Article/details/gwfujjlen.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fktsv.cn/Article/details/gwopogekk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.vehdjk.com/Article/details/gdtlydiua.sHtML

[R54] 比较两个文件
来源：http://3g.yfazqb.com/Article/details/gikumuzvf.sHtML

diff a.txt b.txt
来源：http://m.share.epnwcf.com/Article/details/gsyhleklc.sHtML

[R55] 压缩与解压
来源：http://www.blog.sjlbkw.cn/Article/details/guniohice.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.vehdjk.com/Article/details/gionprqpw.sHtML

[R56] 远程拷贝
来源：http://www.m.share.bbcook.cn/Article/details/gxkzqlime.sHtML

scp file user@host:/path/
来源：http://www.share.tarul.cn/Article/details/gxtwaubhq.sHtML

[R57] 远程执行命令
来源：http://www.share.yfazqb.com/Article/details/gaipbtexy.sHtML

ssh user@host 'uptime'
来源：http://wap.yfazqb.com/Article/details/ghaevyrhg.sHtML

[R58] 下载文件
来源：http://www.blog.fktsv.cn/Article/details/groutmlsw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.tarul.cn/Article/details/gklkziedx.sHtML

[R59] 发 POST JSON
来源：http://m.share.epnwcf.com/Article/details/ggazroina.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.yfazqb.com/Article/details/gcxfonkcy.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.yfazqb.com/Article/details/gipjdgzid.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.tarul.cn/Article/details/gyiymouao.sHtML

[R61] 磁盘占用
来源：http://baike.epnwcf.com/Article/details/gxxdgqnsp.sHtML

df -h;  du -sh *
来源：http://www.m.share.vehdjk.com/Article/details/gbhwdqsiy.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.bbcook.cn/Article/details/gdyrcjjai.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.yfazqb.com/Article/details/gfruorlpl.sHtML

[R63] 内存与进程
来源：http://wap.yfazqb.com/Article/details/gfgrpkwww.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.tarul.cn/Article/details/gsmevzbvi.sHtML

[R64] 结束进程
来源：http://m.share.tarul.cn/Article/details/glxtolhjh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fktsv.cn/Article/details/gqheawwev.sHtML

[R65] 查看端口占用
来源：http://read.share.epnwcf.com/Article/details/gxgqccugh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.bbcook.cn/Article/details/gwjdstuzi.sHtML

[R66] 定时任务
来源：http://wap.tarul.cn/Article/details/gwtyioiid.sHtML

crontab -e;  crontab -l
来源：http://baike.tarul.cn/Article/details/gqnkcexpz.sHtML

[R67] 生成随机十六进制串
来源：http://wap.yfazqb.com/Article/details/gwrhcpngt.sHtML

openssl rand -hex 16
来源：http://3g.sjlbkw.cn/Article/details/gxagdeqob.sHtML

[R68] 计算文件校验值
来源：http://www.blog.epnwcf.com/Article/details/gkijzhadi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.sjlbkw.cn/Article/details/gqlzmoamf.sHtML

[R69] 生成随机密码
来源：http://www.share.yfazqb.com/Article/details/gxsbyvbeq.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fktsv.cn/Article/details/gegomieqv.sHtML

[R70] 时间戳与互转
来源：http://mobile.sjlbkw.cn/Article/details/grpvfivcq.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.vehdjk.com/Article/details/gvooenfcj.sHtML

[R71] 日期格式化
来源：http://baike.sjlbkw.cn/Article/details/guvuancvq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.sjlbkw.cn/Article/details/gkybiteje.sHtML

[R72] 等待端口就绪
来源：http://m.share.bbcook.cn/Article/details/gpmakxedr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.tarul.cn/Article/details/gxrlixqml.sHtML

[R73] 分割大日志
来源：http://blog.tarul.cn/Article/details/gssaizsja.sHtML

split -l 1000 big.log part_
来源：http://baike.tarul.cn/Article/details/gvnddaaih.sHtML

[R74] 批量重命名
来源：http://m.share.epnwcf.com/Article/details/gmwylxhln.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.tarul.cn/Article/details/gyvfkboae.sHtML

[R75] 导出环境变量
来源：http://blog.sjlbkw.cn/Article/details/gldyyhqri.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fktsv.cn/Article/details/gmqdaenzs.sHtML

[R76] 使用临时文件
来源：http://read.share.epnwcf.com/Article/details/gfylfybss.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.sjlbkw.cn/Article/details/gkxxpmsrz.sHtML

[R77] 读取用户输入
来源：http://www.share.vehdjk.com/Article/details/geabunaie.sHtML

read -rp "请输入: " ans
来源：http://mobile.vehdjk.com/Article/details/gneznuxih.sHtML

[R78] 交互式菜单
来源：http://read.share.epnwcf.com/Article/details/gnxawzttu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fktsv.cn/Article/details/gorghjsck.sHtML

[R79] 解析命令行选项
来源：http://m.share.fktsv.cn/Article/details/gynylhdbc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.tarul.cn/Article/details/gtytkpcut.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.tarul.cn/Article/details/gemtjckhs.sHtML

time ./run.sh
来源：http://www.m.share.fktsv.cn/Article/details/gdhhivmns.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gtzvgclsh.sHtML

S. C / C++ 专题
来源：http://www.m.share.bbcook.cn/Article/details/geiymymng.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gmwxqnjnt.sHtML

[S01] C：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gzvcrjckp.sHtML

#include <stdio.h>
来源：http://www.blog.sjlbkw.cn/Article/details/ggmlrmlyt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.sjlbkw.cn/Article/details/gpxlyktte.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.bbcook.cn/Article/details/grqkpraup.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.epnwcf.com/Article/details/genglzsya.sHtML

[S03] C：读入整数
来源：http://www.share.sjlbkw.cn/Article/details/gzyjihetj.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.sjlbkw.cn/Article/details/gtteosabl.sHtML

[S04] C：字符串复制
来源：http://read.share.sjlbkw.cn/Article/details/gnadrxrdh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fktsv.cn/Article/details/gtzqkkrwz.sHtML

[S05] C：字符串长度
来源：http://mobile.bbcook.cn/Article/details/gylvpbjdh.sHtML

strlen(s)
来源：http://www.m.share.tarul.cn/Article/details/gcmiqgcmy.sHtML

[S06] C：字符串比较
来源：http://blog.vehdjk.com/Article/details/gduartxuz.sHtML

strcmp(a, b) == 0
来源：http://blog.vehdjk.com/Article/details/gpcrlclfg.sHtML

[S07] C：数组遍历求和
来源：http://mobile.epnwcf.com/Article/details/gxixcdxwc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.sjlbkw.cn/Article/details/gzotnwmsu.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.vehdjk.com/Article/details/gkpmokhjs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.tarul.cn/Article/details/ghbplhskd.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.vehdjk.com/Article/details/gxzzattnb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.vehdjk.com/Article/details/glbzwojwz.sHtML

[S10] C：指针与解引用
来源：http://m.share.bbcook.cn/Article/details/gngnadscb.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fktsv.cn/Article/details/guuzevnkq.sHtML

[S11] C：逐行读文件
来源：http://baike.bbcook.cn/Article/details/ggcvesaqp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.yfazqb.com/Article/details/gnzsvclex.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.yfazqb.com/Article/details/ghmequaln.sHtML

fclose(f);
来源：http://www.share.yfazqb.com/Article/details/geqhmsvdk.sHtML

[S12] C：写文件
来源：http://www.blog.vehdjk.com/Article/details/gwdadxqkg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.sjlbkw.cn/Article/details/gxyxgqdwf.sHtML

[S13] C：宏定义
来源：http://www.m.share.epnwcf.com/Article/details/gkedgdplb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.epnwcf.com/Article/details/gjcdrrbjv.sHtML

[S14] C：枚举
来源：http://read.share.tarul.cn/Article/details/gsqxhmqsa.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fktsv.cn/Article/details/gzebswybo.sHtML

[S15] C：类型转换
来源：http://www.share.bbcook.cn/Article/details/gupnwizca.sHtML

(double) a / b
来源：http://www.m.share.vehdjk.com/Article/details/gbaaorjjm.sHtML

[S16] C：位操作置位
来源：http://mobile.sjlbkw.cn/Article/details/ghkaazofh.sHtML

x |= (1 << 3);
来源：http://wap.bbcook.cn/Article/details/gsritcrxw.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fktsv.cn/Article/details/guydkrdst.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.epnwcf.com/Article/details/gdurxowjm.sHtML

[S18] C：命令行参数
来源：http://read.share.vehdjk.com/Article/details/gcahedauh.sHtML

int main(int argc, char **argv)
来源：http://m.share.fktsv.cn/Article/details/gtylcvuxi.sHtML

[S19] C：快速排序
来源：http://3g.yfazqb.com/Article/details/gpoajdubm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.sjlbkw.cn/Article/details/gndwpurca.sHtML

[S20] C：二分查找
来源：http://www.m.share.vehdjk.com/Article/details/gbpomktbw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.tarul.cn/Article/details/glmyhsevl.sHtML

[S21] C：字符类别判断
来源：http://blog.vehdjk.com/Article/details/gbwmwwkcw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.tarul.cn/Article/details/grljsgknz.sHtML

[S22] C：字符串转数字
来源：http://3g.sjlbkw.cn/Article/details/gjvkybmpp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.yfazqb.com/Article/details/gvwydoefi.sHtML

[S23] C：随机数
来源：http://3g.vehdjk.com/Article/details/gthbbbmlg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.vehdjk.com/Article/details/gwmyqpsia.sHtML

[S24] C：获取本地时间
来源：http://3g.bbcook.cn/Article/details/gyyvhlcoe.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.bbcook.cn/Article/details/gihjmrchh.sHtML

[S25] C：内存拷贝
来源：http://m.share.yfazqb.com/Article/details/gclpfqsfv.sHtML

memcpy(dst, src, n);
来源：http://baike.vehdjk.com/Article/details/gdkzdekys.sHtML

[S26] C：内存清零
来源：http://www.blog.bbcook.cn/Article/details/gekxcucrx.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.bbcook.cn/Article/details/gltayoawk.sHtML

[S27] C：定义常量
来源：http://www.share.fktsv.cn/Article/details/gcqcgxidi.sHtML

const double PI = 3.14159;
来源：http://3g.bbcook.cn/Article/details/ginckynrp.sHtML

[S28] C：静态变量
来源：http://www.m.share.fktsv.cn/Article/details/gbnrnnuvw.sHtML

static int counter = 0;
来源：http://read.share.tarul.cn/Article/details/gccvdhiee.sHtML

[S29] C：变参函数
来源：http://blog.sjlbkw.cn/Article/details/gcwdpoqxk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.yfazqb.com/Article/details/gkebfjxdi.sHtML

[S30] C：头文件保护
来源：http://blog.vehdjk.com/Article/details/gkxcfaaly.sHtML

#ifndef X_H
来源：http://m.share.tarul.cn/Article/details/gcrzmhblo.sHtML

#define X_H
来源：http://blog.epnwcf.com/Article/details/gvromksyy.sHtML

#endif
来源：http://wap.sjlbkw.cn/Article/details/gilgfqepu.sHtML

[S31] C++：Hello World
来源：http://baike.bbcook.cn/Article/details/gjqrynywc.sHtML

#include <iostream>
来源：http://www.m.share.bbcook.cn/Article/details/gsauziujx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.vehdjk.com/Article/details/gazyqwqaw.sHtML

[S32] C++：字符串
来源：http://mobile.yfazqb.com/Article/details/grlunvyzy.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.epnwcf.com/Article/details/gdbfxpmnv.sHtML

[S33] C++：vector 增删
来源：http://www.share.vehdjk.com/Article/details/gdeywsrwt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.epnwcf.com/Article/details/gitdegitk.sHtML

[S34] C++：遍历 vector
来源：http://mobile.yfazqb.com/Article/details/gzlahvjse.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fktsv.cn/Article/details/gqdloigsu.sHtML

[S35] C++：map
来源：http://mobile.tarul.cn/Article/details/gckarddcv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.vehdjk.com/Article/details/givhhcprj.sHtML

[S36] C++：unordered_map
来源：http://www.blog.epnwcf.com/Article/details/gcsmhbtjz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.sjlbkw.cn/Article/details/gkueepmpn.sHtML

[S37] C++：set
来源：http://wap.fktsv.cn/Article/details/gwuvtfzsu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.tarul.cn/Article/details/gevkgpclu.sHtML

[S38] C++：排序
来源：http://m.share.vehdjk.com/Article/details/gfxhkkshc.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fktsv.cn/Article/details/gjqepoqdx.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.epnwcf.com/Article/details/godmdnibw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.vehdjk.com/Article/details/gcgcqlnms.sHtML

[S40] C++：查找元素
来源：http://www.share.epnwcf.com/Article/details/ghyaqfboh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.epnwcf.com/Article/details/gbiosepmg.sHtML

[S41] C++：类与构造函数
来源：http://m.share.epnwcf.com/Article/details/gozkxbwsm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fktsv.cn/Article/details/gwmnivxjc.sHtML

[S42] C++：继承与虚函数
来源：http://blog.bbcook.cn/Article/details/gyedmpqdm.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fktsv.cn/Article/details/gfopiqhub.sHtML

[S43] C++：智能指针
来源：http://wap.vehdjk.com/Article/details/gxoyjblpg.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fktsv.cn/Article/details/ggkizeoso.sHtML

[S44] C++：引用传参
来源：http://baike.vehdjk.com/Article/details/glzclubex.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.sjlbkw.cn/Article/details/gctgzutgq.sHtML

[S45] C++：lambda
来源：http://baike.bbcook.cn/Article/details/gpuzexejb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.sjlbkw.cn/Article/details/gxbqlgpxi.sHtML

[S46] C++：函数模板
来源：http://wap.epnwcf.com/Article/details/gcbgldqgy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.yfazqb.com/Article/details/gqnchtiqq.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gwsqqotng.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.sjlbkw.cn/Article/details/gpxkliwav.sHtML

[S48] C++：逐行读文件
来源：http://wap.yfazqb.com/Article/details/gliqkyxcd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.tarul.cn/Article/details/ghientddb.sHtML

while (std::getline(in, line)) { }
来源：http://3g.bbcook.cn/Article/details/gztwxzjsd.sHtML

[S49] C++：写文件
来源：http://read.share.sjlbkw.cn/Article/details/gfuymozps.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.vehdjk.com/Article/details/gghfhollk.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.sjlbkw.cn/Article/details/gzdxhfppt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.yfazqb.com/Article/details/ggvjrrzyw.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.sjlbkw.cn/Article/details/gegfeiuep.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.tarul.cn/Article/details/gttopwehu.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.epnwcf.com/Article/details/guvnrzmgi.sHtML

int size() const noexcept { return n_; }
来源：http://blog.bbcook.cn/Article/details/gapvrhfkz.sHtML

[S53] C++：移动语义
来源：http://baike.sjlbkw.cn/Article/details/gfxvsnens.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.vehdjk.com/Article/details/geqeuwmia.sHtML

[S54] C++：异常处理
来源：http://www.share.vehdjk.com/Article/details/gpavnvrvf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.epnwcf.com/Article/details/glzbsjlxh.sHtML

[S55] C++：结构化绑定
来源：http://mobile.epnwcf.com/Article/details/guyllfjfw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.sjlbkw.cn/Article/details/gsuemzkww.sHtML

[S56] C++：optional
来源：http://wap.fktsv.cn/Article/details/glpemqqjb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fktsv.cn/Article/details/gyaiapcri.sHtML

[S57] C++：编译期常量
来源：http://read.share.yfazqb.com/Article/details/gjncigvzx.sHtML

constexpr int N = 10;
来源：http://baike.bbcook.cn/Article/details/gjqhhkklh.sHtML

[S58] C++：命名空间
来源：http://mobile.tarul.cn/Article/details/gtgqdpiih.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fktsv.cn/Article/details/gzvlyjyrz.sHtML

[S59] C++：静态断言
来源：http://www.m.share.sjlbkw.cn/Article/details/glzjnkdag.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fktsv.cn/Article/details/gfaftwjgp.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.yfazqb.com/Article/details/gbpsainaa.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.bbcook.cn/Article/details/gzfdiphpp.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gxfvddrgc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.yfazqb.com/Article/details/gyufavizb.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/glnwbyrjr.sHtML

[T01] Kotlin：Hello World
来源：http://blog.sjlbkw.cn/Article/details/gecynilbd.sHtML

println("Hello")
来源：http://wap.sjlbkw.cn/Article/details/gojofnhtr.sHtML

[T02] Kotlin：变量
来源：http://baike.tarul.cn/Article/details/gdslzmtxi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.sjlbkw.cn/Article/details/gnvihgttv.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.tarul.cn/Article/details/goefnukny.sHtML

"值: $b"
来源：http://3g.vehdjk.com/Article/details/gmayoqrmv.sHtML

[T04] Kotlin：空安全
来源：http://baike.tarul.cn/Article/details/gutektdeh.sHtML

val n: String? = null;  n?.length
来源：http://www.share.epnwcf.com/Article/details/glbatwrbv.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.epnwcf.com/Article/details/gksojkvwp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fktsv.cn/Article/details/guwevfrqa.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.epnwcf.com/Article/details/gmzmackrj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.bbcook.cn/Article/details/gegazwftn.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.vehdjk.com/Article/details/gvooarzrt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.yfazqb.com/Article/details/grgbflxjb.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.vehdjk.com/Article/details/ggcrzhfix.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.yfazqb.com/Article/details/gktydqntd.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fktsv.cn/Article/details/gyobemsvl.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.epnwcf.com/Article/details/gwxypyzsq.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.sjlbkw.cn/Article/details/gfbafvojb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.epnwcf.com/Article/details/gdtgxduho.sHtML

[T11] Kotlin：协程
来源：http://m.share.bbcook.cn/Article/details/gwzvfzhqo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fktsv.cn/Article/details/gdeyzhltr.sHtML

[T12] Kotlin：解构声明
来源：http://3g.yfazqb.com/Article/details/gsbxrwbni.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.tarul.cn/Article/details/gbdodmzuo.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.tarul.cn/Article/details/giqhbcefa.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.epnwcf.com/Article/details/glcypmxmx.sHtML

[T14] Kotlin：循环
来源：http://m.share.vehdjk.com/Article/details/gadfevcjm.sHtML

for (i in 1..10) println(i)
来源：http://wap.tarul.cn/Article/details/gtvkhwufa.sHtML

[T15] Kotlin：接口
来源：http://blog.sjlbkw.cn/Article/details/gplauqcvk.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.vehdjk.com/Article/details/gynahksuf.sHtML

[T16] Swift：Hello World
来源：http://m.share.epnwcf.com/Article/details/gskfkurgk.sHtML

print("Hello")
来源：http://3g.yfazqb.com/Article/details/gtszeenla.sHtML

[T17] Swift：变量与常量
来源：http://wap.bbcook.cn/Article/details/gcdemeryv.sHtML

var a = 1;  let b = 2
来源：http://www.blog.bbcook.cn/Article/details/gcgxvgkye.sHtML

[T18] Swift：字符串插值
来源：http://mobile.tarul.cn/Article/details/gpadzaeyf.sHtML

"值: \(b)"
来源：http://read.share.vehdjk.com/Article/details/glmeaxmdl.sHtML

[T19] Swift：可选绑定
来源：http://wap.bbcook.cn/Article/details/gkaduwtfk.sHtML

if let n = opt { print(n) }
来源：http://3g.tarul.cn/Article/details/gegyhvrrp.sHtML

[T20] Swift：数组操作
来源：http://read.share.sjlbkw.cn/Article/details/gnotsahnx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fktsv.cn/Article/details/gymfarkzu.sHtML

[T21] Swift：遍历
来源：http://www.share.tarul.cn/Article/details/gynagyxlv.sHtML

for x in a { print(x) }
来源：http://www.m.share.bbcook.cn/Article/details/gzlwoandl.sHtML

[T22] Swift：字典
来源：http://www.share.fktsv.cn/Article/details/gtolhiiiu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.yfazqb.com/Article/details/gmybwtlin.sHtML

[T23] Swift：函数
来源：http://wap.bbcook.cn/Article/details/gzisjzemb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.vehdjk.com/Article/details/gsjdaafak.sHtML

[T24] Swift：闭包
来源：http://3g.vehdjk.com/Article/details/gtpfrdxde.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.sjlbkw.cn/Article/details/geqhviaxq.sHtML

[T25] Swift：结构体
来源：http://blog.fktsv.cn/Article/details/gkxgmvjkp.sHtML

struct P { var x: Int }
来源：http://wap.sjlbkw.cn/Article/details/gmwwkqgfi.sHtML

[T26] Swift：类与重写
来源：http://blog.epnwcf.com/Article/details/gsjqgnodq.sHtML

class A: Base { override func f() {} }
来源：http://baike.vehdjk.com/Article/details/gyeqllfmh.sHtML

[T27] Swift：错误处理
来源：http://baike.tarul.cn/Article/details/gwexitxua.sHtML

do { try f() } catch { print(error) }
来源：http://blog.vehdjk.com/Article/details/ghjecmxxu.sHtML

[T28] Swift：枚举
来源：http://3g.vehdjk.com/Article/details/gycytsspl.sHtML

enum Color { case red, green }
来源：http://m.share.yfazqb.com/Article/details/gdkcowspr.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.vehdjk.com/Article/details/gpfewqjpr.sHtML

guard let x = opt else { return }
来源：http://m.share.epnwcf.com/Article/details/gyvqwfbbm.sHtML

[T30] Swift：协议
来源：http://m.share.epnwcf.com/Article/details/gogljenvd.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.yfazqb.com/Article/details/gtjoxqggr.sHtML


<!-- 参考信息 -->