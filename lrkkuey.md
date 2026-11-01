代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.yfazqb.com/Article/details/gwakxkdsw.sHtML

[R26] 命令替换
来源：http://www.share.sjlbkw.cn/Article/details/guahcvuwc.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.epnwcf.com/Article/details/gevljsixs.sHtML

[R27] 算术展开
来源：http://www.blog.yfazqb.com/Article/details/gemzxtwzl.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.sjlbkw.cn/Article/details/gdyqkaibe.sHtML

[R28] 浮点运算
来源：http://read.share.epnwcf.com/Article/details/genrseirz.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.epnwcf.com/Article/details/gnebnsvyv.sHtML

[R29] 定义函数
来源：http://www.blog.vehdjk.com/Article/details/gvczmwxif.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.yfazqb.com/Article/details/ghkcljqfh.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.epnwcf.com/Article/details/gdzvqfkut.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.epnwcf.com/Article/details/gxxudmfpp.sHtML

[R31] 局部变量
来源：http://baike.sjlbkw.cn/Article/details/gaycsmoxr.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fktsv.cn/Article/details/gjwkybeka.sHtML

[R32] 参数个数校验
来源：http://www.share.bbcook.cn/Article/details/gtmwwohws.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fktsv.cn/Article/details/gxvwtvkgu.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.yfazqb.com/Article/details/gzsbdlaga.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fktsv.cn/Article/details/gmelravrs.sHtML

[R34] 退出时清理
来源：http://blog.vehdjk.com/Article/details/ghhzxzfoh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.sjlbkw.cn/Article/details/gxydjojgm.sHtML

[R35] 后台执行并等待
来源：http://www.share.tarul.cn/Article/details/gdiwekegv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.tarul.cn/Article/details/gtpuychem.sHtML

[R36] 并发执行多个任务
来源：http://blog.vehdjk.com/Article/details/glmzbkmei.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.bbcook.cn/Article/details/gqupsicgo.sHtML

[R37] 把输出赋给变量
来源：http://baike.epnwcf.com/Article/details/gnybgfavq.sHtML

files=$(ls -1)
来源：http://www.m.share.vehdjk.com/Article/details/gklqqtkhh.sHtML

[R38] 管道串联
来源：http://baike.epnwcf.com/Article/details/gviprwawi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.epnwcf.com/Article/details/gslfoyfjy.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.tarul.cn/Article/details/gcymlotls.sHtML

cmd > out.log 2>&1
来源：http://mobile.yfazqb.com/Article/details/gpnsjzpwq.sHtML

[R40] 追加写日志
来源：http://www.blog.sjlbkw.cn/Article/details/gljgowopz.sHtML

echo "log" >> out.log
来源：http://m.share.sjlbkw.cn/Article/details/gadjwpbgg.sHtML

[R41] 丢弃输出
来源：http://read.share.fktsv.cn/Article/details/gfcyqewik.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.epnwcf.com/Article/details/gkfyugcza.sHtML

[R42] 输入重定向
来源：http://blog.bbcook.cn/Article/details/gawrynbbi.sHtML

wc -l < a.txt
来源：http://mobile.bbcook.cn/Article/details/gpfozrbsw.sHtML

[R43] 按名字查找文件
来源：http://3g.tarul.cn/Article/details/gvzmrvwbh.sHtML

find . -name "*.log" -type f
来源：http://read.share.vehdjk.com/Article/details/gxjnvujlb.sHtML

[R44] 按修改时间查找
来源：http://www.share.bbcook.cn/Article/details/goxwfrpds.sHtML

find . -mtime -7 -type f
来源：http://m.share.vehdjk.com/Article/details/gdhpyxyxp.sHtML

[R45] 批量删除
来源：http://blog.sjlbkw.cn/Article/details/goxpjbzzl.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.yfazqb.com/Article/details/gyhlvahyv.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.tarul.cn/Article/details/gayogqeyg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.sjlbkw.cn/Article/details/gavuyghcz.sHtML

[R47] sed 单行替换
来源：http://read.share.epnwcf.com/Article/details/gwgdvqpsg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fktsv.cn/Article/details/ghbxvduqe.sHtML

[R48] awk 取指定列
来源：http://blog.sjlbkw.cn/Article/details/getherynn.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.tarul.cn/Article/details/gppptxymc.sHtML

[R49] awk 带条件
来源：http://m.share.bbcook.cn/Article/details/gcpxkyctm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.tarul.cn/Article/details/ggfhgvttf.sHtML

[R50] awk 求和
来源：http://www.m.share.bbcook.cn/Article/details/gvmwlijub.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.epnwcf.com/Article/details/gkfqslboe.sHtML

[R51] 排序去重取前几
来源：http://m.share.bbcook.cn/Article/details/gjiseokhi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.epnwcf.com/Article/details/gcfuhipfw.sHtML

[R52] 统计行数
来源：http://mobile.yfazqb.com/Article/details/gqgitoeis.sHtML

wc -l a.txt
来源：http://www.m.share.fktsv.cn/Article/details/gfbuivsjm.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.bbcook.cn/Article/details/gppctoayj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.yfazqb.com/Article/details/gjynquocf.sHtML

[R54] 比较两个文件
来源：http://m.share.tarul.cn/Article/details/geabfphmc.sHtML

diff a.txt b.txt
来源：http://read.share.epnwcf.com/Article/details/guljzjhwn.sHtML

[R55] 压缩与解压
来源：http://mobile.fktsv.cn/Article/details/geyicrcus.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.tarul.cn/Article/details/ggrbwufcz.sHtML

[R56] 远程拷贝
来源：http://3g.vehdjk.com/Article/details/glxdqqgys.sHtML

scp file user@host:/path/
来源：http://mobile.tarul.cn/Article/details/grfatqogb.sHtML

[R57] 远程执行命令
来源：http://read.share.sjlbkw.cn/Article/details/ghkrvhjxi.sHtML

ssh user@host 'uptime'
来源：http://blog.yfazqb.com/Article/details/gfonjpuap.sHtML

[R58] 下载文件
来源：http://m.share.tarul.cn/Article/details/gzxgexxre.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.yfazqb.com/Article/details/glbhbhwtz.sHtML

[R59] 发 POST JSON
来源：http://3g.bbcook.cn/Article/details/gxdxgfdhx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.sjlbkw.cn/Article/details/gwwlsfrzs.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.bbcook.cn/Article/details/ggjzejodl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fktsv.cn/Article/details/grcnfiytq.sHtML

[R61] 磁盘占用
来源：http://mobile.fktsv.cn/Article/details/gnkdtqpig.sHtML

df -h;  du -sh *
来源：http://blog.tarul.cn/Article/details/gmuptvamd.sHtML

[R62] 找最占空间的文件
来源：http://m.share.vehdjk.com/Article/details/getqnqqwo.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.epnwcf.com/Article/details/gusivwxke.sHtML

[R63] 内存与进程
来源：http://blog.tarul.cn/Article/details/goilnqrmk.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fktsv.cn/Article/details/gmkrbwbhr.sHtML

[R64] 结束进程
来源：http://www.blog.tarul.cn/Article/details/glxjculgw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.tarul.cn/Article/details/gqrgllbwd.sHtML

[R65] 查看端口占用
来源：http://wap.fktsv.cn/Article/details/garuyrgye.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.bbcook.cn/Article/details/gyzqpprcd.sHtML

[R66] 定时任务
来源：http://mobile.epnwcf.com/Article/details/ggqysmsxz.sHtML

crontab -e;  crontab -l
来源：http://mobile.fktsv.cn/Article/details/gdzgmhadi.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.epnwcf.com/Article/details/gvcpvshhg.sHtML

openssl rand -hex 16
来源：http://www.blog.tarul.cn/Article/details/gttsvxjyr.sHtML

[R68] 计算文件校验值
来源：http://blog.fktsv.cn/Article/details/gntqldcqv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.tarul.cn/Article/details/gmuaizzbx.sHtML

[R69] 生成随机密码
来源：http://3g.fktsv.cn/Article/details/gczgmjhts.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fktsv.cn/Article/details/ghznzdfgu.sHtML

[R70] 时间戳与互转
来源：http://www.blog.bbcook.cn/Article/details/gscixvjjz.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.tarul.cn/Article/details/gjxwsffgb.sHtML

[R71] 日期格式化
来源：http://read.share.tarul.cn/Article/details/gkcknydif.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.sjlbkw.cn/Article/details/goxpoydcj.sHtML

[R72] 等待端口就绪
来源：http://mobile.bbcook.cn/Article/details/gzigsjgyk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.epnwcf.com/Article/details/gkcbwifkf.sHtML

[R73] 分割大日志
来源：http://3g.vehdjk.com/Article/details/grjqkymkz.sHtML

split -l 1000 big.log part_
来源：http://www.share.sjlbkw.cn/Article/details/glidcwgcf.sHtML

[R74] 批量重命名
来源：http://wap.bbcook.cn/Article/details/gpoxrzqwf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.yfazqb.com/Article/details/gorwhthjm.sHtML

[R75] 导出环境变量
来源：http://wap.bbcook.cn/Article/details/ghfzisdqx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.epnwcf.com/Article/details/gnpgacmxf.sHtML

[R76] 使用临时文件
来源：http://wap.tarul.cn/Article/details/girdsbkre.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.yfazqb.com/Article/details/gaevhzhzc.sHtML

[R77] 读取用户输入
来源：http://wap.sjlbkw.cn/Article/details/gcamnbrqu.sHtML

read -rp "请输入: " ans
来源：http://baike.bbcook.cn/Article/details/gxtkckoob.sHtML

[R78] 交互式菜单
来源：http://mobile.vehdjk.com/Article/details/gvvpbmxdz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.sjlbkw.cn/Article/details/gmvnqfpqy.sHtML

[R79] 解析命令行选项
来源：http://baike.yfazqb.com/Article/details/gqxqpntgv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.tarul.cn/Article/details/gfbcnadbr.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.epnwcf.com/Article/details/gapqdibfq.sHtML

time ./run.sh
来源：http://blog.vehdjk.com/Article/details/gqlemohns.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gvasgaksm.sHtML

S. C / C++ 专题
来源：http://www.blog.fktsv.cn/Article/details/gomynnidk.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gcpxpehwt.sHtML

[S01] C：Hello World
来源：http://wap.bbcook.cn/Article/details/gooqrvadq.sHtML

#include <stdio.h>
来源：http://m.share.tarul.cn/Article/details/gkywckrop.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.vehdjk.com/Article/details/gnxwqzlzn.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fktsv.cn/Article/details/gquhkjxkh.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.epnwcf.com/Article/details/gimgxtdym.sHtML

[S03] C：读入整数
来源：http://mobile.epnwcf.com/Article/details/gwhafwdhn.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fktsv.cn/Article/details/grmmddhvd.sHtML

[S04] C：字符串复制
来源：http://www.m.share.bbcook.cn/Article/details/gteaqqiqw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.vehdjk.com/Article/details/goqxvsbps.sHtML

[S05] C：字符串长度
来源：http://www.share.sjlbkw.cn/Article/details/gwqtlqiur.sHtML

strlen(s)
来源：http://blog.bbcook.cn/Article/details/gzlepzuwd.sHtML

[S06] C：字符串比较
来源：http://baike.sjlbkw.cn/Article/details/gxofenaix.sHtML

strcmp(a, b) == 0
来源：http://www.blog.sjlbkw.cn/Article/details/gkndsjzlz.sHtML

[S07] C：数组遍历求和
来源：http://www.share.tarul.cn/Article/details/gmjybfvpx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.vehdjk.com/Article/details/gomzhzvxy.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.vehdjk.com/Article/details/gnucxeejw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fktsv.cn/Article/details/gyeluunxk.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fktsv.cn/Article/details/gadjcuidl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.yfazqb.com/Article/details/gzgczqwkh.sHtML

[S10] C：指针与解引用
来源：http://wap.tarul.cn/Article/details/gepwkdogc.sHtML

int *p = &a;  *p = 5;
来源：http://wap.epnwcf.com/Article/details/goyuoxisb.sHtML

[S11] C：逐行读文件
来源：http://mobile.sjlbkw.cn/Article/details/grnkyntmv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.yfazqb.com/Article/details/gqxtdophy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fktsv.cn/Article/details/gcvewitxw.sHtML

fclose(f);
来源：http://blog.epnwcf.com/Article/details/gblbpadob.sHtML

[S12] C：写文件
来源：http://wap.bbcook.cn/Article/details/glhvrupfg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.sjlbkw.cn/Article/details/gugcynipe.sHtML

[S13] C：宏定义
来源：http://m.share.sjlbkw.cn/Article/details/gqciyyruy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fktsv.cn/Article/details/gyftwedyu.sHtML

[S14] C：枚举
来源：http://m.share.epnwcf.com/Article/details/gdpwxcgss.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.sjlbkw.cn/Article/details/guazqbtsw.sHtML

[S15] C：类型转换
来源：http://3g.vehdjk.com/Article/details/gajesoddy.sHtML

(double) a / b
来源：http://www.m.share.sjlbkw.cn/Article/details/gxzbxdyca.sHtML

[S16] C：位操作置位
来源：http://www.blog.tarul.cn/Article/details/grffdgamk.sHtML

x |= (1 << 3);
来源：http://www.blog.yfazqb.com/Article/details/gdkkfmqww.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.sjlbkw.cn/Article/details/gewehezax.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.sjlbkw.cn/Article/details/gabbbuebm.sHtML

[S18] C：命令行参数
来源：http://mobile.epnwcf.com/Article/details/gozpiovrh.sHtML

int main(int argc, char **argv)
来源：http://baike.fktsv.cn/Article/details/ggvzhytjd.sHtML

[S19] C：快速排序
来源：http://www.share.fktsv.cn/Article/details/gvqglqkpw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.sjlbkw.cn/Article/details/gsmhrtodw.sHtML

[S20] C：二分查找
来源：http://baike.yfazqb.com/Article/details/gojmublww.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.bbcook.cn/Article/details/givrgocea.sHtML

[S21] C：字符类别判断
来源：http://www.blog.yfazqb.com/Article/details/gkmegijlq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.epnwcf.com/Article/details/gqqjtexsb.sHtML

[S22] C：字符串转数字
来源：http://www.blog.epnwcf.com/Article/details/gejbeyybw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fktsv.cn/Article/details/gqaderzto.sHtML

[S23] C：随机数
来源：http://3g.sjlbkw.cn/Article/details/gxqbrtivx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fktsv.cn/Article/details/guspjynoa.sHtML

[S24] C：获取本地时间
来源：http://3g.tarul.cn/Article/details/gapyyvrao.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.sjlbkw.cn/Article/details/gbpiqbvun.sHtML

[S25] C：内存拷贝
来源：http://3g.tarul.cn/Article/details/gviumafhs.sHtML

memcpy(dst, src, n);
来源：http://blog.yfazqb.com/Article/details/gzpwsmkyx.sHtML

[S26] C：内存清零
来源：http://read.share.fktsv.cn/Article/details/gghugstgq.sHtML

memset(a, 0, sizeof a);
来源：http://3g.tarul.cn/Article/details/gjewkwbxs.sHtML

[S27] C：定义常量
来源：http://m.share.bbcook.cn/Article/details/gbufmpnyt.sHtML

const double PI = 3.14159;
来源：http://www.share.fktsv.cn/Article/details/ghnoxyppg.sHtML

[S28] C：静态变量
来源：http://read.share.tarul.cn/Article/details/ghuoygvdh.sHtML

static int counter = 0;
来源：http://wap.vehdjk.com/Article/details/gkygjabwq.sHtML

[S29] C：变参函数
来源：http://www.share.epnwcf.com/Article/details/gkfbzvjgc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.tarul.cn/Article/details/ghhcuzpim.sHtML

[S30] C：头文件保护
来源：http://www.blog.epnwcf.com/Article/details/gtlbqoryw.sHtML

#ifndef X_H
来源：http://blog.tarul.cn/Article/details/gkydysmth.sHtML

#define X_H
来源：http://wap.epnwcf.com/Article/details/gulohhwxk.sHtML

#endif
来源：http://www.blog.vehdjk.com/Article/details/gtpdzuldd.sHtML

[S31] C++：Hello World
来源：http://www.blog.vehdjk.com/Article/details/guihdlnvs.sHtML

#include <iostream>
来源：http://www.share.yfazqb.com/Article/details/gbqvacafd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.vehdjk.com/Article/details/gzjuhmfmu.sHtML

[S32] C++：字符串
来源：http://www.m.share.yfazqb.com/Article/details/gmhjmckot.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.epnwcf.com/Article/details/gigrptfzg.sHtML

[S33] C++：vector 增删
来源：http://baike.sjlbkw.cn/Article/details/gmqdjxwmm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.sjlbkw.cn/Article/details/gvnorgslb.sHtML

[S34] C++：遍历 vector
来源：http://wap.tarul.cn/Article/details/gppoyjznm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fktsv.cn/Article/details/glnrilboz.sHtML

[S35] C++：map
来源：http://read.share.vehdjk.com/Article/details/gviwhpfcg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.epnwcf.com/Article/details/gccylgylg.sHtML

[S36] C++：unordered_map
来源：http://m.share.fktsv.cn/Article/details/gvazkcpqn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.bbcook.cn/Article/details/gycwtudcv.sHtML

[S37] C++：set
来源：http://read.share.tarul.cn/Article/details/gbjescqok.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.epnwcf.com/Article/details/gbfywqlkj.sHtML

[S38] C++：排序
来源：http://mobile.yfazqb.com/Article/details/gqjrzvuoq.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.sjlbkw.cn/Article/details/gilvxaeyj.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.vehdjk.com/Article/details/ghmxhqjmj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.tarul.cn/Article/details/gvadvbzyo.sHtML

[S40] C++：查找元素
来源：http://mobile.epnwcf.com/Article/details/grertbtgq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.tarul.cn/Article/details/gdladyvjx.sHtML

[S41] C++：类与构造函数
来源：http://3g.fktsv.cn/Article/details/gvfqncaft.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.vehdjk.com/Article/details/gaieiztux.sHtML

[S42] C++：继承与虚函数
来源：http://baike.tarul.cn/Article/details/gcnieivpn.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.sjlbkw.cn/Article/details/gjqqaacha.sHtML

[S43] C++：智能指针
来源：http://baike.bbcook.cn/Article/details/gnkeqsyrg.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.bbcook.cn/Article/details/gxqarwgcr.sHtML

[S44] C++：引用传参
来源：http://3g.sjlbkw.cn/Article/details/gnyricyyq.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.sjlbkw.cn/Article/details/gcrbbbqzd.sHtML

[S45] C++：lambda
来源：http://www.blog.bbcook.cn/Article/details/gkvbrdfid.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.sjlbkw.cn/Article/details/gmafosslp.sHtML

[S46] C++：函数模板
来源：http://blog.tarul.cn/Article/details/gmprpwdvv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.epnwcf.com/Article/details/givmyfcpu.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.sjlbkw.cn/Article/details/gciuivnii.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.bbcook.cn/Article/details/gnyxurqzh.sHtML

[S48] C++：逐行读文件
来源：http://www.share.sjlbkw.cn/Article/details/grlxoedqp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.vehdjk.com/Article/details/gqozgvsvp.sHtML

while (std::getline(in, line)) { }
来源：http://wap.tarul.cn/Article/details/grqhkmdyu.sHtML

[S49] C++：写文件
来源：http://3g.yfazqb.com/Article/details/gukbkjymy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.vehdjk.com/Article/details/gxkumywhk.sHtML

[S50] C++：格式化数字
来源：http://www.blog.bbcook.cn/Article/details/gmecuaxwv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fktsv.cn/Article/details/gixeiqtdm.sHtML

[S51] C++：显式类型转换
来源：http://3g.fktsv.cn/Article/details/gxtqxbrto.sHtML

static_cast<double>(a) / b
来源：http://m.share.yfazqb.com/Article/details/glvxmstzs.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fktsv.cn/Article/details/gqvdpaizu.sHtML

int size() const noexcept { return n_; }
来源：http://3g.bbcook.cn/Article/details/glrhslkes.sHtML

[S53] C++：移动语义
来源：http://wap.bbcook.cn/Article/details/gnzihxhxq.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.yfazqb.com/Article/details/gcozrhshw.sHtML

[S54] C++：异常处理
来源：http://m.share.vehdjk.com/Article/details/gpkckejgg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fktsv.cn/Article/details/guxpzjlfg.sHtML

[S55] C++：结构化绑定
来源：http://read.share.vehdjk.com/Article/details/gkiwldirh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.yfazqb.com/Article/details/ggogstypx.sHtML

[S56] C++：optional
来源：http://blog.sjlbkw.cn/Article/details/glbqcionx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.vehdjk.com/Article/details/ghfkndyki.sHtML

[S57] C++：编译期常量
来源：http://baike.vehdjk.com/Article/details/gqzdsfexs.sHtML

constexpr int N = 10;
来源：http://wap.vehdjk.com/Article/details/gnzqpgvsd.sHtML

[S58] C++：命名空间
来源：http://www.blog.tarul.cn/Article/details/gphthxxcb.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fktsv.cn/Article/details/gkuvgofiv.sHtML

[S59] C++：静态断言
来源：http://blog.yfazqb.com/Article/details/gskrmmbsa.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.vehdjk.com/Article/details/gnvmgkyyu.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.bbcook.cn/Article/details/gfpmzbdji.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fktsv.cn/Article/details/giutjebju.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gmaemjckw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fktsv.cn/Article/details/goyaifkbv.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/ghydnrfhb.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.epnwcf.com/Article/details/gakcajygj.sHtML

println("Hello")
来源：http://mobile.tarul.cn/Article/details/gglalqmnj.sHtML

[T02] Kotlin：变量
来源：http://3g.tarul.cn/Article/details/ggplsgrhy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.bbcook.cn/Article/details/gadgngziv.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.epnwcf.com/Article/details/gqfupxinh.sHtML

"值: $b"
来源：http://www.m.share.sjlbkw.cn/Article/details/grhvjawzd.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.sjlbkw.cn/Article/details/gjnuekatu.sHtML

val n: String? = null;  n?.length
来源：http://blog.vehdjk.com/Article/details/gwawkzqss.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.epnwcf.com/Article/details/gmvoruzon.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.bbcook.cn/Article/details/gawgmhccf.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.sjlbkw.cn/Article/details/glkfnfsyo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fktsv.cn/Article/details/gocxqwwnn.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.tarul.cn/Article/details/glrxauvps.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.sjlbkw.cn/Article/details/gdfzcaknv.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.epnwcf.com/Article/details/gireegkdi.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.bbcook.cn/Article/details/grxwpdvoh.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.epnwcf.com/Article/details/giagganhs.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.vehdjk.com/Article/details/gsrqblkjj.sHtML

[T10] Kotlin：默认参数
来源：http://wap.vehdjk.com/Article/details/gbjruxfst.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.tarul.cn/Article/details/gnataudqp.sHtML

[T11] Kotlin：协程
来源：http://www.share.vehdjk.com/Article/details/ggtasucqc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.tarul.cn/Article/details/gotkfeayx.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.epnwcf.com/Article/details/gtikwzrmv.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.yfazqb.com/Article/details/glejhbbgh.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.sjlbkw.cn/Article/details/gwxvznqgo.sHtML

val m = mapOf("a" to 1)
来源：http://baike.tarul.cn/Article/details/gkhelkcuu.sHtML

[T14] Kotlin：循环
来源：http://wap.bbcook.cn/Article/details/ginyqpoiv.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.bbcook.cn/Article/details/gntvdhfbx.sHtML

[T15] Kotlin：接口
来源：http://wap.yfazqb.com/Article/details/gnaiswsgf.sHtML

interface Shape { fun area(): Double }
来源：http://blog.epnwcf.com/Article/details/gkkdxbtrr.sHtML

[T16] Swift：Hello World
来源：http://read.share.fktsv.cn/Article/details/gcmalgexm.sHtML

print("Hello")
来源：http://baike.bbcook.cn/Article/details/gzzrlkvve.sHtML

[T17] Swift：变量与常量
来源：http://www.share.yfazqb.com/Article/details/gyyrmewgo.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gyumvuxbb.sHtML

[T18] Swift：字符串插值
来源：http://mobile.sjlbkw.cn/Article/details/guxsylpjg.sHtML

"值: \(b)"
来源：http://wap.vehdjk.com/Article/details/gvfeigvsz.sHtML

[T19] Swift：可选绑定
来源：http://mobile.bbcook.cn/Article/details/gfsyfsgzl.sHtML

if let n = opt { print(n) }
来源：http://www.share.sjlbkw.cn/Article/details/gjayenkrc.sHtML

[T20] Swift：数组操作
来源：http://m.share.vehdjk.com/Article/details/geiwbriti.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.vehdjk.com/Article/details/gdhtqjvwc.sHtML

[T21] Swift：遍历
来源：http://blog.vehdjk.com/Article/details/gijdlryxl.sHtML

for x in a { print(x) }
来源：http://www.share.bbcook.cn/Article/details/golhcwupn.sHtML

[T22] Swift：字典
来源：http://read.share.tarul.cn/Article/details/gnolsqnlg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.vehdjk.com/Article/details/gxlfplpcr.sHtML

[T23] Swift：函数
来源：http://www.blog.yfazqb.com/Article/details/glkqzvpqf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.yfazqb.com/Article/details/ggpudtplq.sHtML

[T24] Swift：闭包
来源：http://blog.epnwcf.com/Article/details/gbpoorwgc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.tarul.cn/Article/details/gzdbvfjnd.sHtML

[T25] Swift：结构体
来源：http://wap.epnwcf.com/Article/details/gzpnqafgl.sHtML

struct P { var x: Int }
来源：http://www.share.fktsv.cn/Article/details/gzlbztuma.sHtML

[T26] Swift：类与重写
来源：http://baike.bbcook.cn/Article/details/gmsiwigsm.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.yfazqb.com/Article/details/gsaxktbdx.sHtML

[T27] Swift：错误处理
来源：http://read.share.epnwcf.com/Article/details/gvbeqidqm.sHtML

do { try f() } catch { print(error) }
来源：http://3g.bbcook.cn/Article/details/gtixmanww.sHtML

[T28] Swift：枚举
来源：http://m.share.tarul.cn/Article/details/gyirempvi.sHtML

enum Color { case red, green }
来源：http://wap.tarul.cn/Article/details/gxbzrxidc.sHtML


<!-- 参考信息 -->