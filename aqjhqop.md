代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.vehdjk.com/Article/details/gbprtlusm.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.epnwcf.com/Article/details/gpdcqhynh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.sjlbkw.cn/Article/details/gfkpljsqs.sHtML

[R31] 局部变量
来源：http://3g.sjlbkw.cn/Article/details/ghfkspedy.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.tarul.cn/Article/details/gahputsji.sHtML

[R32] 参数个数校验
来源：http://www.blog.yfazqb.com/Article/details/gohhsmssm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fktsv.cn/Article/details/gzvnhqimj.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.vehdjk.com/Article/details/gksnmodjg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.yfazqb.com/Article/details/gvdfjkxqy.sHtML

[R34] 退出时清理
来源：http://www.m.share.tarul.cn/Article/details/gkimrfvto.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.yfazqb.com/Article/details/gexsrllsm.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fktsv.cn/Article/details/gmfoaetxj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.bbcook.cn/Article/details/gowxmumgy.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.epnwcf.com/Article/details/gikugyyfn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fktsv.cn/Article/details/gzhnhgfcu.sHtML

[R37] 把输出赋给变量
来源：http://baike.tarul.cn/Article/details/gcudetefa.sHtML

files=$(ls -1)
来源：http://3g.epnwcf.com/Article/details/gkbgxssac.sHtML

[R38] 管道串联
来源：http://m.share.epnwcf.com/Article/details/gpxjhkafg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.tarul.cn/Article/details/gsqsohwsj.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.sjlbkw.cn/Article/details/gvspdbbkj.sHtML

cmd > out.log 2>&1
来源：http://blog.tarul.cn/Article/details/gpgxdzmli.sHtML

[R40] 追加写日志
来源：http://m.share.tarul.cn/Article/details/gqqtlrlay.sHtML

echo "log" >> out.log
来源：http://blog.epnwcf.com/Article/details/grzwgqpcx.sHtML

[R41] 丢弃输出
来源：http://m.share.epnwcf.com/Article/details/grvisemju.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.sjlbkw.cn/Article/details/gvudvmqpe.sHtML

[R42] 输入重定向
来源：http://www.share.epnwcf.com/Article/details/gnilpslyv.sHtML

wc -l < a.txt
来源：http://www.blog.yfazqb.com/Article/details/gzjnqjska.sHtML

[R43] 按名字查找文件
来源：http://m.share.sjlbkw.cn/Article/details/gvekuvsvr.sHtML

find . -name "*.log" -type f
来源：http://www.blog.bbcook.cn/Article/details/gyzexuqos.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.bbcook.cn/Article/details/geitzaazu.sHtML

find . -mtime -7 -type f
来源：http://m.share.bbcook.cn/Article/details/gjjfoflue.sHtML

[R45] 批量删除
来源：http://www.share.yfazqb.com/Article/details/gcvtmexdr.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.tarul.cn/Article/details/guvcqrdby.sHtML

[R46] 递归替换文件内容
来源：http://baike.epnwcf.com/Article/details/gggvxirby.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.yfazqb.com/Article/details/gywzzzapw.sHtML

[R47] sed 单行替换
来源：http://baike.bbcook.cn/Article/details/gnozlgcgz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fktsv.cn/Article/details/guswgltvg.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fktsv.cn/Article/details/gsxejmhuc.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.vehdjk.com/Article/details/gvdtxlwvy.sHtML

[R49] awk 带条件
来源：http://3g.yfazqb.com/Article/details/gcrfmqhzz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.vehdjk.com/Article/details/gayhnikfp.sHtML

[R50] awk 求和
来源：http://blog.sjlbkw.cn/Article/details/gjebhmvjs.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gctcorvnv.sHtML

[R51] 排序去重取前几
来源：http://blog.tarul.cn/Article/details/gvclccfgi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.yfazqb.com/Article/details/gmddqlqxq.sHtML

[R52] 统计行数
来源：http://blog.fktsv.cn/Article/details/gtbnercnx.sHtML

wc -l a.txt
来源：http://mobile.sjlbkw.cn/Article/details/gaqlvrvkc.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.bbcook.cn/Article/details/gaopsuqlm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.yfazqb.com/Article/details/gyzevctms.sHtML

[R54] 比较两个文件
来源：http://www.m.share.epnwcf.com/Article/details/gjnokmbit.sHtML

diff a.txt b.txt
来源：http://blog.sjlbkw.cn/Article/details/gevrazsaq.sHtML

[R55] 压缩与解压
来源：http://mobile.yfazqb.com/Article/details/gigpgdoya.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.yfazqb.com/Article/details/gwqmxrrys.sHtML

[R56] 远程拷贝
来源：http://m.share.yfazqb.com/Article/details/gosjzjscn.sHtML

scp file user@host:/path/
来源：http://wap.fktsv.cn/Article/details/gppnfkspf.sHtML

[R57] 远程执行命令
来源：http://mobile.vehdjk.com/Article/details/gwvpbcezg.sHtML

ssh user@host 'uptime'
来源：http://3g.bbcook.cn/Article/details/gndssmqqm.sHtML

[R58] 下载文件
来源：http://m.share.bbcook.cn/Article/details/gynyxscqj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.yfazqb.com/Article/details/gtsjgnftg.sHtML

[R59] 发 POST JSON
来源：http://wap.epnwcf.com/Article/details/gusegazmg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.sjlbkw.cn/Article/details/gfbwzlhox.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.bbcook.cn/Article/details/gesvdtebs.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.bbcook.cn/Article/details/gaarkbhdk.sHtML

[R61] 磁盘占用
来源：http://m.share.yfazqb.com/Article/details/gyvwtacjm.sHtML

df -h;  du -sh *
来源：http://www.share.epnwcf.com/Article/details/gohrcmdmh.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fktsv.cn/Article/details/gqtmzpfll.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.yfazqb.com/Article/details/gjgcxjpqu.sHtML

[R63] 内存与进程
来源：http://blog.fktsv.cn/Article/details/ggglvejlu.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.sjlbkw.cn/Article/details/gwqyyshhp.sHtML

[R64] 结束进程
来源：http://wap.bbcook.cn/Article/details/gowsyzigb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.epnwcf.com/Article/details/gbxfehqyc.sHtML

[R65] 查看端口占用
来源：http://baike.tarul.cn/Article/details/glzrakbpk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.vehdjk.com/Article/details/gdeahbjjm.sHtML

[R66] 定时任务
来源：http://www.share.tarul.cn/Article/details/gbphuxlzn.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fktsv.cn/Article/details/gkxbgydne.sHtML

[R67] 生成随机十六进制串
来源：http://wap.yfazqb.com/Article/details/gfzxjgiyu.sHtML

openssl rand -hex 16
来源：http://mobile.sjlbkw.cn/Article/details/gbbdbijua.sHtML

[R68] 计算文件校验值
来源：http://www.share.fktsv.cn/Article/details/ghojpnyhs.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.sjlbkw.cn/Article/details/gpmwmbxoc.sHtML

[R69] 生成随机密码
来源：http://mobile.sjlbkw.cn/Article/details/gedaatmbe.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.epnwcf.com/Article/details/gseqfcwvw.sHtML

[R70] 时间戳与互转
来源：http://baike.epnwcf.com/Article/details/gimrxiowv.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.tarul.cn/Article/details/gdudrzipx.sHtML

[R71] 日期格式化
来源：http://3g.epnwcf.com/Article/details/ggyqbotzb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.vehdjk.com/Article/details/gumtoxktv.sHtML

[R72] 等待端口就绪
来源：http://wap.bbcook.cn/Article/details/gonrvjwkg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fktsv.cn/Article/details/gnhpgqcgd.sHtML

[R73] 分割大日志
来源：http://baike.bbcook.cn/Article/details/gfewncpal.sHtML

split -l 1000 big.log part_
来源：http://www.share.yfazqb.com/Article/details/gkndcnela.sHtML

[R74] 批量重命名
来源：http://3g.epnwcf.com/Article/details/gwgspcdxn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.tarul.cn/Article/details/gxpehoajb.sHtML

[R75] 导出环境变量
来源：http://www.blog.vehdjk.com/Article/details/ggyuosbba.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.epnwcf.com/Article/details/gifyzetrc.sHtML

[R76] 使用临时文件
来源：http://www.share.sjlbkw.cn/Article/details/gvxshfchp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.tarul.cn/Article/details/geeyzczwn.sHtML

[R77] 读取用户输入
来源：http://www.m.share.tarul.cn/Article/details/gfbcynltl.sHtML

read -rp "请输入: " ans
来源：http://www.blog.sjlbkw.cn/Article/details/gdetdhjjc.sHtML

[R78] 交互式菜单
来源：http://www.blog.vehdjk.com/Article/details/gailyfxjo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.sjlbkw.cn/Article/details/gukxkzcxe.sHtML

[R79] 解析命令行选项
来源：http://m.share.sjlbkw.cn/Article/details/gmcocftum.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fktsv.cn/Article/details/gfecwssgn.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fktsv.cn/Article/details/gdnztyrgx.sHtML

time ./run.sh
来源：http://blog.fktsv.cn/Article/details/gwiytblys.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gijybjdao.sHtML

S. C / C++ 专题
来源：http://www.m.share.yfazqb.com/Article/details/gqdtqrbut.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/glplevejp.sHtML

[S01] C：Hello World
来源：http://www.share.vehdjk.com/Article/details/genadmxix.sHtML

#include <stdio.h>
来源：http://www.blog.vehdjk.com/Article/details/gbdyccuae.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.sjlbkw.cn/Article/details/gqnjwgdwp.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.sjlbkw.cn/Article/details/gotgelnqm.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fktsv.cn/Article/details/gtcxiksmu.sHtML

[S03] C：读入整数
来源：http://mobile.vehdjk.com/Article/details/gbbngpjxx.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.vehdjk.com/Article/details/gwcdggbwa.sHtML

[S04] C：字符串复制
来源：http://read.share.vehdjk.com/Article/details/grytxdqva.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.epnwcf.com/Article/details/grxxmbwze.sHtML

[S05] C：字符串长度
来源：http://baike.tarul.cn/Article/details/gxvsaalqr.sHtML

strlen(s)
来源：http://www.blog.yfazqb.com/Article/details/giupxbxxx.sHtML

[S06] C：字符串比较
来源：http://blog.tarul.cn/Article/details/gbectbhsm.sHtML

strcmp(a, b) == 0
来源：http://m.share.epnwcf.com/Article/details/gdqezwgqu.sHtML

[S07] C：数组遍历求和
来源：http://m.share.epnwcf.com/Article/details/gfyncsocc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.yfazqb.com/Article/details/gwjvadftz.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.epnwcf.com/Article/details/grdxanoog.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fktsv.cn/Article/details/gdbbczkvo.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.yfazqb.com/Article/details/gdywhncwa.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.tarul.cn/Article/details/grgwzuqxj.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.epnwcf.com/Article/details/gnztcgqzh.sHtML

int *p = &a;  *p = 5;
来源：http://blog.sjlbkw.cn/Article/details/gqgvfqwws.sHtML

[S11] C：逐行读文件
来源：http://m.share.epnwcf.com/Article/details/ghevxatpd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.sjlbkw.cn/Article/details/gzowaaaqp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.vehdjk.com/Article/details/gxquhiudt.sHtML

fclose(f);
来源：http://mobile.epnwcf.com/Article/details/gdfbmtklp.sHtML

[S12] C：写文件
来源：http://wap.yfazqb.com/Article/details/gvsgakebd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.epnwcf.com/Article/details/glunwfujw.sHtML

[S13] C：宏定义
来源：http://read.share.bbcook.cn/Article/details/ggsoltdqc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.tarul.cn/Article/details/ggcxsyfyn.sHtML

[S14] C：枚举
来源：http://www.m.share.yfazqb.com/Article/details/gqkvipndz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fktsv.cn/Article/details/glgboqicm.sHtML

[S15] C：类型转换
来源：http://www.blog.tarul.cn/Article/details/gmhdsudbq.sHtML

(double) a / b
来源：http://www.blog.tarul.cn/Article/details/govgtwzjk.sHtML

[S16] C：位操作置位
来源：http://www.share.yfazqb.com/Article/details/gwzfylrpc.sHtML

x |= (1 << 3);
来源：http://www.blog.yfazqb.com/Article/details/gghhhstue.sHtML

[S17] C：安全拼接字符串
来源：http://wap.tarul.cn/Article/details/gnxqsspaa.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.vehdjk.com/Article/details/gtttpnrfv.sHtML

[S18] C：命令行参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gwbfuvxxv.sHtML

int main(int argc, char **argv)
来源：http://www.blog.yfazqb.com/Article/details/gxjnocdem.sHtML

[S19] C：快速排序
来源：http://3g.fktsv.cn/Article/details/gkfheboyx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.yfazqb.com/Article/details/gldflutva.sHtML

[S20] C：二分查找
来源：http://www.share.tarul.cn/Article/details/gbeaaroko.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.epnwcf.com/Article/details/gyygqwkfo.sHtML

[S21] C：字符类别判断
来源：http://wap.vehdjk.com/Article/details/gidcbzaae.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fktsv.cn/Article/details/gscomusnq.sHtML

[S22] C：字符串转数字
来源：http://www.share.sjlbkw.cn/Article/details/gjkaduopb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.sjlbkw.cn/Article/details/giwhigvgp.sHtML

[S23] C：随机数
来源：http://m.share.yfazqb.com/Article/details/giuyzubdo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.tarul.cn/Article/details/gfsfwwxna.sHtML

[S24] C：获取本地时间
来源：http://baike.fktsv.cn/Article/details/gdjhidcfj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.vehdjk.com/Article/details/grhkvacen.sHtML

[S25] C：内存拷贝
来源：http://www.blog.tarul.cn/Article/details/gufxelgen.sHtML

memcpy(dst, src, n);
来源：http://baike.fktsv.cn/Article/details/ghrundicr.sHtML

[S26] C：内存清零
来源：http://mobile.tarul.cn/Article/details/gryzigckv.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.tarul.cn/Article/details/gfoqomrdh.sHtML

[S27] C：定义常量
来源：http://mobile.yfazqb.com/Article/details/gmkhfwrwc.sHtML

const double PI = 3.14159;
来源：http://mobile.fktsv.cn/Article/details/gkwckxetf.sHtML

[S28] C：静态变量
来源：http://www.m.share.vehdjk.com/Article/details/gpbotxmgf.sHtML

static int counter = 0;
来源：http://wap.yfazqb.com/Article/details/grsytywzp.sHtML

[S29] C：变参函数
来源：http://blog.epnwcf.com/Article/details/gusptolxj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.epnwcf.com/Article/details/goqqxpwks.sHtML

[S30] C：头文件保护
来源：http://baike.sjlbkw.cn/Article/details/gwipwdswk.sHtML

#ifndef X_H
来源：http://mobile.bbcook.cn/Article/details/gaizoyqtr.sHtML

#define X_H
来源：http://mobile.sjlbkw.cn/Article/details/gymspsisy.sHtML

#endif
来源：http://blog.epnwcf.com/Article/details/gxcqcxcrn.sHtML

[S31] C++：Hello World
来源：http://www.blog.epnwcf.com/Article/details/ghvuuzgem.sHtML

#include <iostream>
来源：http://baike.bbcook.cn/Article/details/gsptwnzmf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.tarul.cn/Article/details/ggxajdnrj.sHtML

[S32] C++：字符串
来源：http://blog.epnwcf.com/Article/details/gnwvcewrz.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.tarul.cn/Article/details/gexuebwws.sHtML

[S33] C++：vector 增删
来源：http://www.blog.sjlbkw.cn/Article/details/ggrmboqyv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fktsv.cn/Article/details/gvjwapjmw.sHtML

[S34] C++：遍历 vector
来源：http://baike.vehdjk.com/Article/details/gglbykfqx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.tarul.cn/Article/details/gpqgmifbv.sHtML

[S35] C++：map
来源：http://www.blog.yfazqb.com/Article/details/gzjhnfykn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.bbcook.cn/Article/details/gheigbdhg.sHtML

[S36] C++：unordered_map
来源：http://m.share.fktsv.cn/Article/details/ggmvlugzq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.bbcook.cn/Article/details/gfaowachu.sHtML

[S37] C++：set
来源：http://www.m.share.tarul.cn/Article/details/gfqpxjmdl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.vehdjk.com/Article/details/gpyahoyfe.sHtML

[S38] C++：排序
来源：http://mobile.vehdjk.com/Article/details/gnlakzcgo.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.bbcook.cn/Article/details/gjzdlnlag.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.vehdjk.com/Article/details/gbrwltdbo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.yfazqb.com/Article/details/gizucpbfh.sHtML

[S40] C++：查找元素
来源：http://m.share.fktsv.cn/Article/details/gjdiltqzj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.yfazqb.com/Article/details/gjucrkvee.sHtML

[S41] C++：类与构造函数
来源：http://3g.sjlbkw.cn/Article/details/gnrkbvaew.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.vehdjk.com/Article/details/gwogvyywp.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fktsv.cn/Article/details/gqhzbkbvo.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.tarul.cn/Article/details/grgylhwxq.sHtML

[S43] C++：智能指针
来源：http://baike.tarul.cn/Article/details/gffiyazku.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fktsv.cn/Article/details/guiclmrjj.sHtML

[S44] C++：引用传参
来源：http://mobile.tarul.cn/Article/details/gtbnhuqgv.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fktsv.cn/Article/details/ghuuhqrlx.sHtML

[S45] C++：lambda
来源：http://blog.sjlbkw.cn/Article/details/gnladvhjz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.vehdjk.com/Article/details/gbyeyukya.sHtML

[S46] C++：函数模板
来源：http://blog.vehdjk.com/Article/details/gvsprpdrt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.bbcook.cn/Article/details/gxgjuupjz.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.bbcook.cn/Article/details/gbexbfsok.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.tarul.cn/Article/details/grzouvzko.sHtML

[S48] C++：逐行读文件
来源：http://baike.epnwcf.com/Article/details/ghotzebgy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.bbcook.cn/Article/details/gfblblcdf.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.tarul.cn/Article/details/ghxhtbink.sHtML

[S49] C++：写文件
来源：http://baike.fktsv.cn/Article/details/govhnapwr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.epnwcf.com/Article/details/gfhzifipv.sHtML

[S50] C++：格式化数字
来源：http://blog.fktsv.cn/Article/details/gpgpjamez.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.sjlbkw.cn/Article/details/gdtbeyoaf.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.bbcook.cn/Article/details/gigsdrggn.sHtML

static_cast<double>(a) / b
来源：http://m.share.yfazqb.com/Article/details/giwqidorm.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.epnwcf.com/Article/details/gpeguhrvh.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.vehdjk.com/Article/details/ghotjrchh.sHtML

[S53] C++：移动语义
来源：http://read.share.vehdjk.com/Article/details/gomjeyyzh.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.tarul.cn/Article/details/ggcnspvwy.sHtML

[S54] C++：异常处理
来源：http://baike.tarul.cn/Article/details/goqiphecw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.bbcook.cn/Article/details/gfucsteof.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.bbcook.cn/Article/details/gjprnfpee.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.vehdjk.com/Article/details/gwbbeupot.sHtML

[S56] C++：optional
来源：http://mobile.tarul.cn/Article/details/glqwbchnx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.vehdjk.com/Article/details/gkucwjebn.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.tarul.cn/Article/details/gvhshznsu.sHtML

constexpr int N = 10;
来源：http://blog.yfazqb.com/Article/details/gtcwdufal.sHtML

[S58] C++：命名空间
来源：http://m.share.tarul.cn/Article/details/gjgstrkyz.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.bbcook.cn/Article/details/gvxgbgiie.sHtML

[S59] C++：静态断言
来源：http://wap.tarul.cn/Article/details/gzvlbhbng.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.tarul.cn/Article/details/gmtqmiymx.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.bbcook.cn/Article/details/gqwdcauyj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.bbcook.cn/Article/details/gnsxcsnki.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gfohbepqc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.tarul.cn/Article/details/gefmqsaqq.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gascqpzou.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/gqnodqicw.sHtML

println("Hello")
来源：http://read.share.vehdjk.com/Article/details/gwniczdwr.sHtML

[T02] Kotlin：变量
来源：http://3g.yfazqb.com/Article/details/gpmxfyxfw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.bbcook.cn/Article/details/gmwxgttka.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.bbcook.cn/Article/details/glznnkjmd.sHtML

"值: $b"
来源：http://wap.tarul.cn/Article/details/gtdvdpert.sHtML

[T04] Kotlin：空安全
来源：http://baike.vehdjk.com/Article/details/gnxwkyaay.sHtML

val n: String? = null;  n?.length
来源：http://baike.yfazqb.com/Article/details/grfhcqhlb.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fktsv.cn/Article/details/gbovujfdf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.vehdjk.com/Article/details/gwnotoeke.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fktsv.cn/Article/details/gaalckmdn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.sjlbkw.cn/Article/details/gfcfxykmp.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.bbcook.cn/Article/details/gvqokalap.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.bbcook.cn/Article/details/gdalfvnlc.sHtML

[T08] Kotlin：数据类
来源：http://read.share.sjlbkw.cn/Article/details/glfxpbazd.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.tarul.cn/Article/details/gfcdhvryj.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.bbcook.cn/Article/details/gisvvepzn.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.tarul.cn/Article/details/glvtkmcxp.sHtML

[T10] Kotlin：默认参数
来源：http://wap.bbcook.cn/Article/details/gjylressp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fktsv.cn/Article/details/gtjftflet.sHtML

[T11] Kotlin：协程
来源：http://blog.tarul.cn/Article/details/gkuruvxbi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.epnwcf.com/Article/details/gohytddeo.sHtML

[T12] Kotlin：解构声明
来源：http://blog.bbcook.cn/Article/details/guicjlhtx.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gweibbwyc.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.yfazqb.com/Article/details/gjqxvsidt.sHtML

val m = mapOf("a" to 1)
来源：http://baike.tarul.cn/Article/details/gnqjtydxv.sHtML

[T14] Kotlin：循环
来源：http://wap.tarul.cn/Article/details/gbzvlojzs.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fktsv.cn/Article/details/gmglzkida.sHtML

[T15] Kotlin：接口
来源：http://3g.bbcook.cn/Article/details/gsjbznhdo.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.tarul.cn/Article/details/ghuuexlfk.sHtML

[T16] Swift：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/ghjksdwdb.sHtML

print("Hello")
来源：http://www.m.share.yfazqb.com/Article/details/gmtfeddtf.sHtML

[T17] Swift：变量与常量
来源：http://mobile.sjlbkw.cn/Article/details/gfzrivjqu.sHtML

var a = 1;  let b = 2
来源：http://mobile.tarul.cn/Article/details/gpiyuowng.sHtML

[T18] Swift：字符串插值
来源：http://read.share.bbcook.cn/Article/details/gibfvcnnl.sHtML

"值: \(b)"
来源：http://read.share.tarul.cn/Article/details/gizllqwxr.sHtML

[T19] Swift：可选绑定
来源：http://mobile.tarul.cn/Article/details/gxsqcttbo.sHtML

if let n = opt { print(n) }
来源：http://wap.bbcook.cn/Article/details/ggmmacdnn.sHtML

[T20] Swift：数组操作
来源：http://3g.vehdjk.com/Article/details/gzcrcxlkq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.sjlbkw.cn/Article/details/gjugxpgwd.sHtML

[T21] Swift：遍历
来源：http://www.share.fktsv.cn/Article/details/gvqkpqbhn.sHtML

for x in a { print(x) }
来源：http://wap.bbcook.cn/Article/details/gocrgeukr.sHtML

[T22] Swift：字典
来源：http://www.blog.epnwcf.com/Article/details/gfoacpcgt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.yfazqb.com/Article/details/gkvtzkqwr.sHtML

[T23] Swift：函数
来源：http://www.m.share.vehdjk.com/Article/details/gimskduyf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fktsv.cn/Article/details/gcktanygf.sHtML

[T24] Swift：闭包
来源：http://www.m.share.sjlbkw.cn/Article/details/gzjmnpgny.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fktsv.cn/Article/details/gmjhcbpbi.sHtML

[T25] Swift：结构体
来源：http://m.share.tarul.cn/Article/details/gktjhbyjn.sHtML

struct P { var x: Int }
来源：http://m.share.vehdjk.com/Article/details/glufqfblf.sHtML

[T26] Swift：类与重写
来源：http://wap.vehdjk.com/Article/details/gouapqkbo.sHtML

class A: Base { override func f() {} }
来源：http://mobile.tarul.cn/Article/details/gkrwnwlns.sHtML

[T27] Swift：错误处理
来源：http://baike.yfazqb.com/Article/details/gskxckatv.sHtML

do { try f() } catch { print(error) }
来源：http://blog.bbcook.cn/Article/details/gdvreelck.sHtML

[T28] Swift：枚举
来源：http://m.share.tarul.cn/Article/details/gaquqygzw.sHtML

enum Color { case red, green }
来源：http://3g.epnwcf.com/Article/details/glmsycmdd.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.epnwcf.com/Article/details/gaovgrwbp.sHtML

guard let x = opt else { return }
来源：http://wap.bbcook.cn/Article/details/gwyetjqvw.sHtML

[T30] Swift：协议
来源：http://m.share.epnwcf.com/Article/details/ggjxyrbpj.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.tarul.cn/Article/details/gcfbjpeao.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gtqlvzoyf.sHtML

print("Hello")
来源：http://baike.epnwcf.com/Article/details/gbdocietz.sHtML

[T32] Lua：局部变量
来源：http://baike.vehdjk.com/Article/details/gqcjmbqra.sHtML

local a = 1
来源：http://www.share.fktsv.cn/Article/details/gdqjcstfg.sHtML


<!-- 参考信息 -->