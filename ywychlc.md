代发 wailian999

echo $((1 + 2 * 3))
来源：http://www.share.vehdjk.com/Article/details/geptircso.sHtML

[R28] 浮点运算
来源：http://www.share.tarul.cn/Article/details/gydwssemz.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.sjlbkw.cn/Article/details/gquimwure.sHtML

[R29] 定义函数
来源：http://baike.sjlbkw.cn/Article/details/gkuultdop.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.bbcook.cn/Article/details/gkajxwqtv.sHtML

[R30] 函数返回状态码
来源：http://m.share.fktsv.cn/Article/details/gciwdfeuh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.bbcook.cn/Article/details/gvayfnbkp.sHtML

[R31] 局部变量
来源：http://www.m.share.epnwcf.com/Article/details/goersjpgw.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fktsv.cn/Article/details/gslmakvhn.sHtML

[R32] 参数个数校验
来源：http://wap.fktsv.cn/Article/details/gflahgzbq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fktsv.cn/Article/details/gkntgnybt.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.bbcook.cn/Article/details/gcuxjtozq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fktsv.cn/Article/details/gkrlfzbld.sHtML

[R34] 退出时清理
来源：http://wap.vehdjk.com/Article/details/gfxklplwp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.yfazqb.com/Article/details/gobjqiywg.sHtML

[R35] 后台执行并等待
来源：http://m.share.sjlbkw.cn/Article/details/gpqvphlhm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.epnwcf.com/Article/details/gqyaxgfhh.sHtML

[R36] 并发执行多个任务
来源：http://blog.epnwcf.com/Article/details/gasnqvebz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.epnwcf.com/Article/details/gwtvoszdb.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.vehdjk.com/Article/details/gwsamvpqc.sHtML

files=$(ls -1)
来源：http://baike.tarul.cn/Article/details/guyradzoq.sHtML

[R38] 管道串联
来源：http://mobile.sjlbkw.cn/Article/details/gqzzugugv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.sjlbkw.cn/Article/details/gtzcsekke.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.vehdjk.com/Article/details/gzqzgonsj.sHtML

cmd > out.log 2>&1
来源：http://baike.bbcook.cn/Article/details/gtddznjkv.sHtML

[R40] 追加写日志
来源：http://wap.yfazqb.com/Article/details/gjtgwtqig.sHtML

echo "log" >> out.log
来源：http://read.share.sjlbkw.cn/Article/details/ghzfydgua.sHtML

[R41] 丢弃输出
来源：http://3g.bbcook.cn/Article/details/gsmqchaja.sHtML

cmd >/dev/null 2>&1
来源：http://3g.epnwcf.com/Article/details/gslbdwday.sHtML

[R42] 输入重定向
来源：http://m.share.sjlbkw.cn/Article/details/gsovelfct.sHtML

wc -l < a.txt
来源：http://3g.tarul.cn/Article/details/gmngqhhsk.sHtML

[R43] 按名字查找文件
来源：http://3g.yfazqb.com/Article/details/ggbydcgxe.sHtML

find . -name "*.log" -type f
来源：http://m.share.sjlbkw.cn/Article/details/gcgdffnfn.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fktsv.cn/Article/details/gjnnmlkja.sHtML

find . -mtime -7 -type f
来源：http://www.share.sjlbkw.cn/Article/details/gnlcpvgoo.sHtML

[R45] 批量删除
来源：http://baike.fktsv.cn/Article/details/gttixivcf.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fktsv.cn/Article/details/gsejcvtiv.sHtML

[R46] 递归替换文件内容
来源：http://3g.yfazqb.com/Article/details/gawwtylay.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fktsv.cn/Article/details/gmsajyeeh.sHtML

[R47] sed 单行替换
来源：http://www.m.share.vehdjk.com/Article/details/gofxygwuo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.vehdjk.com/Article/details/guzknsatr.sHtML

[R48] awk 取指定列
来源：http://read.share.fktsv.cn/Article/details/gedboctmr.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.yfazqb.com/Article/details/gkjkszuxk.sHtML

[R49] awk 带条件
来源：http://mobile.bbcook.cn/Article/details/gapvyuuit.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.bbcook.cn/Article/details/gxcnagngl.sHtML

[R50] awk 求和
来源：http://mobile.epnwcf.com/Article/details/glvmfvyks.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.yfazqb.com/Article/details/gjguxstxr.sHtML

[R51] 排序去重取前几
来源：http://www.share.vehdjk.com/Article/details/gflwinbfm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.sjlbkw.cn/Article/details/gqhkfrmho.sHtML

[R52] 统计行数
来源：http://www.blog.tarul.cn/Article/details/gbpmucppq.sHtML

wc -l a.txt
来源：http://read.share.fktsv.cn/Article/details/gbepagvcm.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.tarul.cn/Article/details/gebwhzjgr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.sjlbkw.cn/Article/details/gectefhzl.sHtML

[R54] 比较两个文件
来源：http://baike.yfazqb.com/Article/details/ggvznvikk.sHtML

diff a.txt b.txt
来源：http://m.share.fktsv.cn/Article/details/gnqsrzmeh.sHtML

[R55] 压缩与解压
来源：http://blog.tarul.cn/Article/details/gbqbtzhsm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fktsv.cn/Article/details/gugwtpezt.sHtML

[R56] 远程拷贝
来源：http://m.share.sjlbkw.cn/Article/details/gtprosbdc.sHtML

scp file user@host:/path/
来源：http://3g.fktsv.cn/Article/details/gxlwhmmuq.sHtML

[R57] 远程执行命令
来源：http://blog.tarul.cn/Article/details/gsilirezi.sHtML

ssh user@host 'uptime'
来源：http://baike.fktsv.cn/Article/details/gyjnsgxxu.sHtML

[R58] 下载文件
来源：http://3g.sjlbkw.cn/Article/details/gwylbprvf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.bbcook.cn/Article/details/geloaualq.sHtML

[R59] 发 POST JSON
来源：http://www.share.fktsv.cn/Article/details/gwlzenudu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fktsv.cn/Article/details/gdkkasatn.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.epnwcf.com/Article/details/gnshdwxnj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.tarul.cn/Article/details/gmcyirrck.sHtML

[R61] 磁盘占用
来源：http://read.share.epnwcf.com/Article/details/gbtjrkrek.sHtML

df -h;  du -sh *
来源：http://3g.vehdjk.com/Article/details/gasyijjyg.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fktsv.cn/Article/details/gsygbjnop.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.sjlbkw.cn/Article/details/gjpdbeakm.sHtML

[R63] 内存与进程
来源：http://3g.bbcook.cn/Article/details/gqmqmmxfc.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fktsv.cn/Article/details/gidpslbtz.sHtML

[R64] 结束进程
来源：http://www.m.share.bbcook.cn/Article/details/gayolcyfy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.epnwcf.com/Article/details/gbawetfbk.sHtML

[R65] 查看端口占用
来源：http://m.share.sjlbkw.cn/Article/details/gollxgurp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.tarul.cn/Article/details/gzhxlqxhj.sHtML

[R66] 定时任务
来源：http://mobile.epnwcf.com/Article/details/gwdukrdud.sHtML

crontab -e;  crontab -l
来源：http://www.share.vehdjk.com/Article/details/gwtqnmqig.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.yfazqb.com/Article/details/gcxulnuzu.sHtML

openssl rand -hex 16
来源：http://www.share.bbcook.cn/Article/details/gyrdedimd.sHtML

[R68] 计算文件校验值
来源：http://mobile.bbcook.cn/Article/details/gdscpnvgw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.bbcook.cn/Article/details/gotaxixsf.sHtML

[R69] 生成随机密码
来源：http://blog.vehdjk.com/Article/details/gcrtziboh.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.tarul.cn/Article/details/gsosmsrrm.sHtML

[R70] 时间戳与互转
来源：http://3g.yfazqb.com/Article/details/gqsoupgan.sHtML

date +%s;  date -d @1700000000
来源：http://wap.sjlbkw.cn/Article/details/gohmkpfcs.sHtML

[R71] 日期格式化
来源：http://wap.vehdjk.com/Article/details/grnhplvyc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.vehdjk.com/Article/details/gfgbykgre.sHtML

[R72] 等待端口就绪
来源：http://read.share.fktsv.cn/Article/details/gmvykfcwq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.bbcook.cn/Article/details/gkstaxtue.sHtML

[R73] 分割大日志
来源：http://wap.fktsv.cn/Article/details/gnukykuip.sHtML

split -l 1000 big.log part_
来源：http://www.share.vehdjk.com/Article/details/gbewqinzr.sHtML

[R74] 批量重命名
来源：http://mobile.fktsv.cn/Article/details/gtzabxkfy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.sjlbkw.cn/Article/details/glkmzeqxi.sHtML

[R75] 导出环境变量
来源：http://blog.vehdjk.com/Article/details/gxpztzgeg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.tarul.cn/Article/details/gugqnmcrc.sHtML

[R76] 使用临时文件
来源：http://wap.fktsv.cn/Article/details/gldlmgbef.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.bbcook.cn/Article/details/gmhsyuzgo.sHtML

[R77] 读取用户输入
来源：http://read.share.epnwcf.com/Article/details/goqeiftbc.sHtML

read -rp "请输入: " ans
来源：http://3g.yfazqb.com/Article/details/gnlavlvfm.sHtML

[R78] 交互式菜单
来源：http://wap.yfazqb.com/Article/details/gfogffxmf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.vehdjk.com/Article/details/giddyhzre.sHtML

[R79] 解析命令行选项
来源：http://mobile.tarul.cn/Article/details/gmztmcwqk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.bbcook.cn/Article/details/glaumipnl.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.vehdjk.com/Article/details/geaxwpqpl.sHtML

time ./run.sh
来源：http://wap.fktsv.cn/Article/details/gmysnoeqe.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gtxlvvegb.sHtML

S. C / C++ 专题
来源：http://www.m.share.bbcook.cn/Article/details/gaimdhxqd.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gewcvikpm.sHtML

[S01] C：Hello World
来源：http://mobile.vehdjk.com/Article/details/gqmgbepzz.sHtML

#include <stdio.h>
来源：http://read.share.bbcook.cn/Article/details/gtmltkoja.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.sjlbkw.cn/Article/details/giygakdti.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fktsv.cn/Article/details/gqohmmpei.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.vehdjk.com/Article/details/gxghfswua.sHtML

[S03] C：读入整数
来源：http://www.share.yfazqb.com/Article/details/gzeijuxol.sHtML

int x; scanf("%d", &x);
来源：http://3g.epnwcf.com/Article/details/ggsybztcy.sHtML

[S04] C：字符串复制
来源：http://wap.vehdjk.com/Article/details/gygowinvr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.bbcook.cn/Article/details/gplriruny.sHtML

[S05] C：字符串长度
来源：http://read.share.fktsv.cn/Article/details/gtrugaoxq.sHtML

strlen(s)
来源：http://www.share.epnwcf.com/Article/details/gklrhmkkt.sHtML

[S06] C：字符串比较
来源：http://www.blog.epnwcf.com/Article/details/gjtdidcky.sHtML

strcmp(a, b) == 0
来源：http://www.blog.epnwcf.com/Article/details/gnljwxqdv.sHtML

[S07] C：数组遍历求和
来源：http://mobile.vehdjk.com/Article/details/gnqwdnmyc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.yfazqb.com/Article/details/gocxboxsv.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.bbcook.cn/Article/details/gasjrcrnu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.yfazqb.com/Article/details/gxjdjtmrk.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.vehdjk.com/Article/details/gheiynojj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.sjlbkw.cn/Article/details/gkaiwrukl.sHtML

[S10] C：指针与解引用
来源：http://3g.fktsv.cn/Article/details/gcuzodyoh.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.bbcook.cn/Article/details/gjavgaptx.sHtML

[S11] C：逐行读文件
来源：http://read.share.sjlbkw.cn/Article/details/gruqwocnw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.tarul.cn/Article/details/glbagmpuq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.sjlbkw.cn/Article/details/gffpdrmin.sHtML

fclose(f);
来源：http://read.share.epnwcf.com/Article/details/gcklnixck.sHtML

[S12] C：写文件
来源：http://3g.tarul.cn/Article/details/grzppkjxl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.yfazqb.com/Article/details/gtytgqctb.sHtML

[S13] C：宏定义
来源：http://www.m.share.fktsv.cn/Article/details/gbjnivicj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.tarul.cn/Article/details/gkzlyazqx.sHtML

[S14] C：枚举
来源：http://www.share.epnwcf.com/Article/details/ggikenolk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.yfazqb.com/Article/details/gxncwxrwu.sHtML

[S15] C：类型转换
来源：http://read.share.tarul.cn/Article/details/gnmjgkeof.sHtML

(double) a / b
来源：http://3g.sjlbkw.cn/Article/details/gwfcfdpjs.sHtML

[S16] C：位操作置位
来源：http://read.share.vehdjk.com/Article/details/gwdbbmubi.sHtML

x |= (1 << 3);
来源：http://read.share.epnwcf.com/Article/details/gvjpmmkdr.sHtML

[S17] C：安全拼接字符串
来源：http://blog.bbcook.cn/Article/details/gniquqxmk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fktsv.cn/Article/details/gzfybssfg.sHtML

[S18] C：命令行参数
来源：http://baike.epnwcf.com/Article/details/grkjoyntt.sHtML

int main(int argc, char **argv)
来源：http://mobile.bbcook.cn/Article/details/gqlsyhhuy.sHtML

[S19] C：快速排序
来源：http://blog.epnwcf.com/Article/details/gflhwdcdl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.tarul.cn/Article/details/gtgprmokh.sHtML

[S20] C：二分查找
来源：http://www.share.sjlbkw.cn/Article/details/gcydikjbu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.bbcook.cn/Article/details/grdwjihkf.sHtML

[S21] C：字符类别判断
来源：http://m.share.sjlbkw.cn/Article/details/gandfukwk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.bbcook.cn/Article/details/gmedpylyx.sHtML

[S22] C：字符串转数字
来源：http://www.blog.sjlbkw.cn/Article/details/gladzxexr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.yfazqb.com/Article/details/gnpevuelk.sHtML

[S23] C：随机数
来源：http://m.share.fktsv.cn/Article/details/gpwoxssuq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.sjlbkw.cn/Article/details/glmreujid.sHtML

[S24] C：获取本地时间
来源：http://m.share.epnwcf.com/Article/details/gunvkjqil.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.epnwcf.com/Article/details/gwtxhdmti.sHtML

[S25] C：内存拷贝
来源：http://www.blog.bbcook.cn/Article/details/gbhurivxp.sHtML

memcpy(dst, src, n);
来源：http://blog.vehdjk.com/Article/details/grlmphvvi.sHtML

[S26] C：内存清零
来源：http://www.m.share.sjlbkw.cn/Article/details/geipwgzlh.sHtML

memset(a, 0, sizeof a);
来源：http://wap.yfazqb.com/Article/details/gvcuvqjsy.sHtML

[S27] C：定义常量
来源：http://baike.vehdjk.com/Article/details/gishfgjld.sHtML

const double PI = 3.14159;
来源：http://baike.sjlbkw.cn/Article/details/gprzxqvim.sHtML

[S28] C：静态变量
来源：http://m.share.fktsv.cn/Article/details/gksmjbdqj.sHtML

static int counter = 0;
来源：http://blog.vehdjk.com/Article/details/gnfjzraeb.sHtML

[S29] C：变参函数
来源：http://www.share.bbcook.cn/Article/details/grwmxrwqh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.yfazqb.com/Article/details/gepiiypgj.sHtML

[S30] C：头文件保护
来源：http://wap.fktsv.cn/Article/details/grbtmzckn.sHtML

#ifndef X_H
来源：http://baike.tarul.cn/Article/details/gjnvfxnin.sHtML

#define X_H
来源：http://read.share.tarul.cn/Article/details/glsjkmqlh.sHtML

#endif
来源：http://baike.vehdjk.com/Article/details/grlrmrpqp.sHtML

[S31] C++：Hello World
来源：http://www.blog.sjlbkw.cn/Article/details/gngzccovg.sHtML

#include <iostream>
来源：http://baike.tarul.cn/Article/details/ghrskgcmp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fktsv.cn/Article/details/gxdrqaleh.sHtML

[S32] C++：字符串
来源：http://m.share.fktsv.cn/Article/details/gfsvcszkz.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.sjlbkw.cn/Article/details/gkjcschsw.sHtML

[S33] C++：vector 增删
来源：http://baike.bbcook.cn/Article/details/gseipehyy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.epnwcf.com/Article/details/grhxjsnwm.sHtML

[S34] C++：遍历 vector
来源：http://mobile.bbcook.cn/Article/details/gypskjsvq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fktsv.cn/Article/details/gfbruobxp.sHtML

[S35] C++：map
来源：http://m.share.fktsv.cn/Article/details/gyekwsryh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fktsv.cn/Article/details/gwhysvlcv.sHtML

[S36] C++：unordered_map
来源：http://mobile.tarul.cn/Article/details/gopjmarvx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.vehdjk.com/Article/details/ggawjhrnp.sHtML

[S37] C++：set
来源：http://www.m.share.fktsv.cn/Article/details/gxegmbspu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.bbcook.cn/Article/details/gcmzwujbp.sHtML

[S38] C++：排序
来源：http://3g.tarul.cn/Article/details/gthuvdunh.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fktsv.cn/Article/details/gmblnxikc.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.epnwcf.com/Article/details/gboonjpjn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fktsv.cn/Article/details/gojnlhgli.sHtML

[S40] C++：查找元素
来源：http://m.share.bbcook.cn/Article/details/gckxvceui.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fktsv.cn/Article/details/gbfkmncgk.sHtML

[S41] C++：类与构造函数
来源：http://wap.epnwcf.com/Article/details/gxqrhxkqi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.epnwcf.com/Article/details/gabqrnqqt.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.epnwcf.com/Article/details/ggwrbvseh.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.yfazqb.com/Article/details/gdzxozbge.sHtML

[S43] C++：智能指针
来源：http://www.blog.yfazqb.com/Article/details/gcquavmzh.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.vehdjk.com/Article/details/gltqnglbo.sHtML

[S44] C++：引用传参
来源：http://mobile.vehdjk.com/Article/details/gemzoovmh.sHtML

void inc(int &x) { ++x; }
来源：http://3g.sjlbkw.cn/Article/details/gjsxeqfdp.sHtML

[S45] C++：lambda
来源：http://m.share.bbcook.cn/Article/details/gqddklnok.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.sjlbkw.cn/Article/details/glnfcforr.sHtML

[S46] C++：函数模板
来源：http://blog.fktsv.cn/Article/details/gykyaikoi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fktsv.cn/Article/details/geukkrucv.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fktsv.cn/Article/details/gfuqqckbw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.bbcook.cn/Article/details/gltwjkwdp.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.vehdjk.com/Article/details/gcmyybyux.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.sjlbkw.cn/Article/details/gnjtvrqvm.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.bbcook.cn/Article/details/gxosnsnif.sHtML

[S49] C++：写文件
来源：http://blog.tarul.cn/Article/details/gsmyuqkcb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.sjlbkw.cn/Article/details/gdnedudpl.sHtML

[S50] C++：格式化数字
来源：http://wap.sjlbkw.cn/Article/details/gfijjkqrr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.epnwcf.com/Article/details/gvduygnvy.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.bbcook.cn/Article/details/gynwssfox.sHtML

static_cast<double>(a) / b
来源：http://wap.bbcook.cn/Article/details/gsygcyosd.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.yfazqb.com/Article/details/gttdaojmr.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fktsv.cn/Article/details/ggduywkgp.sHtML

[S53] C++：移动语义
来源：http://www.m.share.vehdjk.com/Article/details/gibylnyrk.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fktsv.cn/Article/details/gqgpwjvff.sHtML

[S54] C++：异常处理
来源：http://www.share.bbcook.cn/Article/details/guqrovxwl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.yfazqb.com/Article/details/gmttlfhwj.sHtML

[S55] C++：结构化绑定
来源：http://read.share.yfazqb.com/Article/details/gmqvyiklm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.epnwcf.com/Article/details/gwveqitht.sHtML

[S56] C++：optional
来源：http://baike.tarul.cn/Article/details/gfrdgdvsf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.sjlbkw.cn/Article/details/gixlgceck.sHtML

[S57] C++：编译期常量
来源：http://3g.epnwcf.com/Article/details/gsefqrdno.sHtML

constexpr int N = 10;
来源：http://www.share.bbcook.cn/Article/details/gmtlxljsm.sHtML

[S58] C++：命名空间
来源：http://www.blog.fktsv.cn/Article/details/gjsxggzdp.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fktsv.cn/Article/details/gnovmmrwk.sHtML

[S59] C++：静态断言
来源：http://read.share.vehdjk.com/Article/details/gyoeswbye.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.tarul.cn/Article/details/gztirathy.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.epnwcf.com/Article/details/grbqqhgai.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.bbcook.cn/Article/details/gqiwwigjf.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gyriqalsp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.tarul.cn/Article/details/gwvzwwrfj.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gesgvfdfx.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fktsv.cn/Article/details/ggjtqhpvm.sHtML

println("Hello")
来源：http://3g.sjlbkw.cn/Article/details/ggeghhdba.sHtML

[T02] Kotlin：变量
来源：http://baike.epnwcf.com/Article/details/gvsitbquz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.bbcook.cn/Article/details/gmaffybyr.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.yfazqb.com/Article/details/gihqcrngs.sHtML

"值: $b"
来源：http://www.m.share.vehdjk.com/Article/details/gscazfcug.sHtML

[T04] Kotlin：空安全
来源：http://baike.sjlbkw.cn/Article/details/gaszgkkrt.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.sjlbkw.cn/Article/details/gtfrkrxia.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.yfazqb.com/Article/details/gkwgxofof.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.tarul.cn/Article/details/gufmpdblh.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.vehdjk.com/Article/details/gttjljnpr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fktsv.cn/Article/details/gdxcurnxt.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.yfazqb.com/Article/details/gbhpdwfsk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fktsv.cn/Article/details/gombisggu.sHtML

[T08] Kotlin：数据类
来源：http://wap.vehdjk.com/Article/details/gmwgosegt.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.epnwcf.com/Article/details/gcnkgfxvv.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fktsv.cn/Article/details/gdiomvmem.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fktsv.cn/Article/details/grlltkrcc.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgtqvkzo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.sjlbkw.cn/Article/details/gecbhbbiz.sHtML

[T11] Kotlin：协程
来源：http://baike.sjlbkw.cn/Article/details/glpmulqya.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.epnwcf.com/Article/details/gmzqlsrtr.sHtML

[T12] Kotlin：解构声明
来源：http://baike.yfazqb.com/Article/details/grlmcchry.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/goyunihkj.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.yfazqb.com/Article/details/gpijszetk.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.bbcook.cn/Article/details/gxxbapptd.sHtML

[T14] Kotlin：循环
来源：http://m.share.fktsv.cn/Article/details/gothuogef.sHtML

for (i in 1..10) println(i)
来源：http://blog.tarul.cn/Article/details/gdbqgeboh.sHtML

[T15] Kotlin：接口
来源：http://www.share.tarul.cn/Article/details/gkiisgqhd.sHtML

interface Shape { fun area(): Double }
来源：http://baike.yfazqb.com/Article/details/gaekbnxzc.sHtML

[T16] Swift：Hello World
来源：http://mobile.epnwcf.com/Article/details/gkkvemhxa.sHtML

print("Hello")
来源：http://baike.vehdjk.com/Article/details/gwgvyguyq.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.bbcook.cn/Article/details/gxewhormw.sHtML

var a = 1;  let b = 2
来源：http://3g.fktsv.cn/Article/details/gkhqlvoyi.sHtML

[T18] Swift：字符串插值
来源：http://baike.fktsv.cn/Article/details/glvkrdkek.sHtML

"值: \(b)"
来源：http://baike.fktsv.cn/Article/details/glayytkqg.sHtML

[T19] Swift：可选绑定
来源：http://read.share.epnwcf.com/Article/details/gbnydhxqa.sHtML

if let n = opt { print(n) }
来源：http://mobile.bbcook.cn/Article/details/geqqjtnyp.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.vehdjk.com/Article/details/gbdlmxpyd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.tarul.cn/Article/details/gjoczvxkt.sHtML

[T21] Swift：遍历
来源：http://m.share.bbcook.cn/Article/details/gjdzxjflc.sHtML

for x in a { print(x) }
来源：http://mobile.epnwcf.com/Article/details/gpltzlzfa.sHtML

[T22] Swift：字典
来源：http://wap.sjlbkw.cn/Article/details/gxufjhpks.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.sjlbkw.cn/Article/details/gxusddcvx.sHtML

[T23] Swift：函数
来源：http://www.blog.fktsv.cn/Article/details/gboqnslwj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.bbcook.cn/Article/details/gndrqtvwj.sHtML

[T24] Swift：闭包
来源：http://www.share.fktsv.cn/Article/details/gtxdmwgvt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.tarul.cn/Article/details/geicotspt.sHtML

[T25] Swift：结构体
来源：http://baike.tarul.cn/Article/details/gytdpkxji.sHtML

struct P { var x: Int }
来源：http://m.share.tarul.cn/Article/details/gbpqaeeba.sHtML

[T26] Swift：类与重写
来源：http://www.blog.vehdjk.com/Article/details/gyzgyzexs.sHtML

class A: Base { override func f() {} }
来源：http://m.share.yfazqb.com/Article/details/gfchsrptk.sHtML

[T27] Swift：错误处理
来源：http://mobile.epnwcf.com/Article/details/gqkbqluyb.sHtML

do { try f() } catch { print(error) }
来源：http://baike.vehdjk.com/Article/details/gmljbveos.sHtML

[T28] Swift：枚举
来源：http://www.blog.yfazqb.com/Article/details/gzwuhmkre.sHtML

enum Color { case red, green }
来源：http://mobile.tarul.cn/Article/details/gifzvycda.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.bbcook.cn/Article/details/gjdlnobrd.sHtML

guard let x = opt else { return }
来源：http://3g.sjlbkw.cn/Article/details/gijnduorj.sHtML

[T30] Swift：协议
来源：http://www.m.share.vehdjk.com/Article/details/giocucipj.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.epnwcf.com/Article/details/gujbjwtya.sHtML


<!-- 参考信息 -->