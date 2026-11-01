代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://baike.fktsv.cn/Article/details/gncrccxkk.sHtML

[R32] 参数个数校验
来源：http://blog.tarul.cn/Article/details/gcrwarupz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.yfazqb.com/Article/details/geeawpwkz.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.tarul.cn/Article/details/gvauovwkp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.sjlbkw.cn/Article/details/gnyzunieu.sHtML

[R34] 退出时清理
来源：http://read.share.tarul.cn/Article/details/gwtzttzzi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.epnwcf.com/Article/details/gvxsvxnne.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.epnwcf.com/Article/details/gyrahgapr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.yfazqb.com/Article/details/giswxkcth.sHtML

[R36] 并发执行多个任务
来源：http://mobile.vehdjk.com/Article/details/gfnboaktl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.tarul.cn/Article/details/ghwnkuoja.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.yfazqb.com/Article/details/gvomuekhd.sHtML

files=$(ls -1)
来源：http://3g.sjlbkw.cn/Article/details/gicorbvkn.sHtML

[R38] 管道串联
来源：http://baike.bbcook.cn/Article/details/gsbkndlia.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.tarul.cn/Article/details/geifgkzcv.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fktsv.cn/Article/details/gpbiojrlz.sHtML

cmd > out.log 2>&1
来源：http://read.share.yfazqb.com/Article/details/gyuzyvvfg.sHtML

[R40] 追加写日志
来源：http://mobile.bbcook.cn/Article/details/gnzrrwbop.sHtML

echo "log" >> out.log
来源：http://www.share.epnwcf.com/Article/details/girynbfws.sHtML

[R41] 丢弃输出
来源：http://mobile.bbcook.cn/Article/details/gttzvmlwb.sHtML

cmd >/dev/null 2>&1
来源：http://3g.epnwcf.com/Article/details/gbujdteza.sHtML

[R42] 输入重定向
来源：http://3g.epnwcf.com/Article/details/gpjlekhwj.sHtML

wc -l < a.txt
来源：http://blog.bbcook.cn/Article/details/gcgrhfxbt.sHtML

[R43] 按名字查找文件
来源：http://m.share.epnwcf.com/Article/details/gonjfqpza.sHtML

find . -name "*.log" -type f
来源：http://baike.yfazqb.com/Article/details/gfmbaggmi.sHtML

[R44] 按修改时间查找
来源：http://blog.fktsv.cn/Article/details/gbhxtkpjq.sHtML

find . -mtime -7 -type f
来源：http://www.share.bbcook.cn/Article/details/gbripfbro.sHtML

[R45] 批量删除
来源：http://mobile.vehdjk.com/Article/details/gpbmgchgf.sHtML

find . -name "*.tmp" -delete
来源：http://blog.yfazqb.com/Article/details/gklmkvrzg.sHtML

[R46] 递归替换文件内容
来源：http://baike.epnwcf.com/Article/details/gazniygji.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.sjlbkw.cn/Article/details/gmsafcdfo.sHtML

[R47] sed 单行替换
来源：http://www.blog.yfazqb.com/Article/details/gdbcayjxb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.epnwcf.com/Article/details/gwqyamiqo.sHtML

[R48] awk 取指定列
来源：http://m.share.epnwcf.com/Article/details/ghgwowtoz.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.yfazqb.com/Article/details/grjesdolq.sHtML

[R49] awk 带条件
来源：http://wap.tarul.cn/Article/details/grgybvtgg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.vehdjk.com/Article/details/gavyomrlh.sHtML

[R50] awk 求和
来源：http://baike.bbcook.cn/Article/details/gpycjojbn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.tarul.cn/Article/details/getrifzhc.sHtML

[R51] 排序去重取前几
来源：http://baike.epnwcf.com/Article/details/gjccauguc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.vehdjk.com/Article/details/gdmuynahy.sHtML

[R52] 统计行数
来源：http://blog.bbcook.cn/Article/details/gbtpmshwu.sHtML

wc -l a.txt
来源：http://blog.yfazqb.com/Article/details/gqrcfempq.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fktsv.cn/Article/details/gmgnaazct.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.vehdjk.com/Article/details/gxfrbtull.sHtML

[R54] 比较两个文件
来源：http://baike.bbcook.cn/Article/details/gdseqecqc.sHtML

diff a.txt b.txt
来源：http://3g.tarul.cn/Article/details/galkuqxuv.sHtML

[R55] 压缩与解压
来源：http://3g.yfazqb.com/Article/details/gpofehbty.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.vehdjk.com/Article/details/gjebcttfo.sHtML

[R56] 远程拷贝
来源：http://www.share.fktsv.cn/Article/details/gzwmjzpuc.sHtML

scp file user@host:/path/
来源：http://blog.vehdjk.com/Article/details/gbeycmxsp.sHtML

[R57] 远程执行命令
来源：http://www.blog.sjlbkw.cn/Article/details/gutwjsbmv.sHtML

ssh user@host 'uptime'
来源：http://read.share.tarul.cn/Article/details/gmecfljje.sHtML

[R58] 下载文件
来源：http://wap.tarul.cn/Article/details/gdsaperib.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fktsv.cn/Article/details/gozmskhdt.sHtML

[R59] 发 POST JSON
来源：http://baike.epnwcf.com/Article/details/gbkykdxsl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fktsv.cn/Article/details/gjvvikcmc.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.tarul.cn/Article/details/gksigjsvq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.tarul.cn/Article/details/gyepfqzop.sHtML

[R61] 磁盘占用
来源：http://m.share.vehdjk.com/Article/details/gqxawzpgj.sHtML

df -h;  du -sh *
来源：http://www.share.vehdjk.com/Article/details/ggjhmujiu.sHtML

[R62] 找最占空间的文件
来源：http://3g.yfazqb.com/Article/details/gbmsofweu.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.tarul.cn/Article/details/gnyuxphhc.sHtML

[R63] 内存与进程
来源：http://www.share.bbcook.cn/Article/details/gcnwjomfi.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.tarul.cn/Article/details/gdcjzmvau.sHtML

[R64] 结束进程
来源：http://wap.fktsv.cn/Article/details/gefrptshh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.vehdjk.com/Article/details/gwcmbhahs.sHtML

[R65] 查看端口占用
来源：http://3g.fktsv.cn/Article/details/gjcbpiysn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.yfazqb.com/Article/details/gppjjtaji.sHtML

[R66] 定时任务
来源：http://blog.vehdjk.com/Article/details/gfeihrhjo.sHtML

crontab -e;  crontab -l
来源：http://m.share.bbcook.cn/Article/details/gbzirudzf.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.epnwcf.com/Article/details/gbedhmbyi.sHtML

openssl rand -hex 16
来源：http://www.blog.sjlbkw.cn/Article/details/gqaygppfy.sHtML

[R68] 计算文件校验值
来源：http://www.share.bbcook.cn/Article/details/gsdvmfalq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.yfazqb.com/Article/details/gjtiqrirh.sHtML

[R69] 生成随机密码
来源：http://blog.vehdjk.com/Article/details/gwayiatcq.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.sjlbkw.cn/Article/details/ggylswoje.sHtML

[R70] 时间戳与互转
来源：http://www.blog.bbcook.cn/Article/details/gcrmjtybv.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fktsv.cn/Article/details/glehcpmri.sHtML

[R71] 日期格式化
来源：http://3g.vehdjk.com/Article/details/gfhzmwwty.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.epnwcf.com/Article/details/giipwjuzx.sHtML

[R72] 等待端口就绪
来源：http://www.share.tarul.cn/Article/details/gxilwuzvm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fktsv.cn/Article/details/gwiqmgids.sHtML

[R73] 分割大日志
来源：http://wap.yfazqb.com/Article/details/gzalvkqfj.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.epnwcf.com/Article/details/gxykeqgac.sHtML

[R74] 批量重命名
来源：http://baike.sjlbkw.cn/Article/details/gcqkcrnlt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.tarul.cn/Article/details/gpujwtgnd.sHtML

[R75] 导出环境变量
来源：http://blog.vehdjk.com/Article/details/gthquewxf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.epnwcf.com/Article/details/ggpqddtdg.sHtML

[R76] 使用临时文件
来源：http://read.share.bbcook.cn/Article/details/groqqvwmw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.bbcook.cn/Article/details/gnslnnwon.sHtML

[R77] 读取用户输入
来源：http://www.blog.yfazqb.com/Article/details/geiswjvwf.sHtML

read -rp "请输入: " ans
来源：http://blog.yfazqb.com/Article/details/gdozafayu.sHtML

[R78] 交互式菜单
来源：http://www.share.tarul.cn/Article/details/geqsfxjxa.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.bbcook.cn/Article/details/gjyproglq.sHtML

[R79] 解析命令行选项
来源：http://mobile.tarul.cn/Article/details/gkuwdyoos.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fktsv.cn/Article/details/gbvqanpzi.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.epnwcf.com/Article/details/glocaifjd.sHtML

time ./run.sh
来源：http://blog.sjlbkw.cn/Article/details/geqwqxsas.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gndeqbtvi.sHtML

S. C / C++ 专题
来源：http://read.share.epnwcf.com/Article/details/gwyndrbxh.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gqmshhvyi.sHtML

[S01] C：Hello World
来源：http://3g.fktsv.cn/Article/details/gzecwqtvq.sHtML

#include <stdio.h>
来源：http://www.m.share.bbcook.cn/Article/details/gtqavzarh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.epnwcf.com/Article/details/gvdmtrytl.sHtML

[S02] C：变量与格式化输出
来源：http://baike.tarul.cn/Article/details/gkxaazlyi.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.sjlbkw.cn/Article/details/gnoonvzlq.sHtML

[S03] C：读入整数
来源：http://3g.bbcook.cn/Article/details/gyyvcltsu.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fktsv.cn/Article/details/gkmhoxmcm.sHtML

[S04] C：字符串复制
来源：http://baike.sjlbkw.cn/Article/details/gxyfgqwpz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fktsv.cn/Article/details/grwkranwd.sHtML

[S05] C：字符串长度
来源：http://3g.yfazqb.com/Article/details/gtntnpalr.sHtML

strlen(s)
来源：http://www.m.share.yfazqb.com/Article/details/gzkpxoniu.sHtML

[S06] C：字符串比较
来源：http://3g.vehdjk.com/Article/details/gruwyybqr.sHtML

strcmp(a, b) == 0
来源：http://wap.epnwcf.com/Article/details/gshjnexxc.sHtML

[S07] C：数组遍历求和
来源：http://3g.epnwcf.com/Article/details/gfcdgcucq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.vehdjk.com/Article/details/gfsnahovc.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.bbcook.cn/Article/details/ggmprhdvj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.tarul.cn/Article/details/gyevzirdp.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.epnwcf.com/Article/details/gbfnmtybw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fktsv.cn/Article/details/ghvsjuagh.sHtML

[S10] C：指针与解引用
来源：http://mobile.yfazqb.com/Article/details/gpsmwfdow.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.epnwcf.com/Article/details/gucrclhuo.sHtML

[S11] C：逐行读文件
来源：http://3g.fktsv.cn/Article/details/gbffigyvf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.epnwcf.com/Article/details/gtvkxebxm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.tarul.cn/Article/details/gcqjgqgjt.sHtML

fclose(f);
来源：http://www.blog.tarul.cn/Article/details/gndfokvqs.sHtML

[S12] C：写文件
来源：http://wap.yfazqb.com/Article/details/gssacomen.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.sjlbkw.cn/Article/details/gscfjugpx.sHtML

[S13] C：宏定义
来源：http://wap.yfazqb.com/Article/details/gthvqxmbe.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.vehdjk.com/Article/details/gpdanaqsu.sHtML

[S14] C：枚举
来源：http://baike.epnwcf.com/Article/details/glpfhwxtb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.bbcook.cn/Article/details/gbfprhazb.sHtML

[S15] C：类型转换
来源：http://3g.sjlbkw.cn/Article/details/gbgccedub.sHtML

(double) a / b
来源：http://www.blog.vehdjk.com/Article/details/gbicecjch.sHtML

[S16] C：位操作置位
来源：http://read.share.vehdjk.com/Article/details/guqgklwog.sHtML

x |= (1 << 3);
来源：http://blog.bbcook.cn/Article/details/gczveodmw.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fktsv.cn/Article/details/gtxfdgopd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fktsv.cn/Article/details/gllwwrmca.sHtML

[S18] C：命令行参数
来源：http://www.share.bbcook.cn/Article/details/gihxxgggo.sHtML

int main(int argc, char **argv)
来源：http://baike.sjlbkw.cn/Article/details/gqleipbzh.sHtML

[S19] C：快速排序
来源：http://blog.fktsv.cn/Article/details/glubtdtty.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.yfazqb.com/Article/details/gpiljjavm.sHtML

[S20] C：二分查找
来源：http://mobile.yfazqb.com/Article/details/girpqalhv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.bbcook.cn/Article/details/gnvprxkhl.sHtML

[S21] C：字符类别判断
来源：http://wap.tarul.cn/Article/details/gjowtpnat.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.bbcook.cn/Article/details/ghqjnbsoz.sHtML

[S22] C：字符串转数字
来源：http://m.share.fktsv.cn/Article/details/ghvavemgl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.vehdjk.com/Article/details/gyvvzoncp.sHtML

[S23] C：随机数
来源：http://www.m.share.sjlbkw.cn/Article/details/gursaqfgy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.epnwcf.com/Article/details/gxjxnlosa.sHtML

[S24] C：获取本地时间
来源：http://mobile.epnwcf.com/Article/details/gpcdxqzgm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.vehdjk.com/Article/details/gqewtsypi.sHtML

[S25] C：内存拷贝
来源：http://3g.sjlbkw.cn/Article/details/gcdnhxzru.sHtML

memcpy(dst, src, n);
来源：http://m.share.fktsv.cn/Article/details/gfphwrvue.sHtML

[S26] C：内存清零
来源：http://blog.tarul.cn/Article/details/gjtnsbhts.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.bbcook.cn/Article/details/ggqrzximj.sHtML

[S27] C：定义常量
来源：http://blog.epnwcf.com/Article/details/gtxyiwiok.sHtML

const double PI = 3.14159;
来源：http://3g.bbcook.cn/Article/details/gadsovvoi.sHtML

[S28] C：静态变量
来源：http://m.share.tarul.cn/Article/details/glweyghdu.sHtML

static int counter = 0;
来源：http://baike.yfazqb.com/Article/details/gqvommoxl.sHtML

[S29] C：变参函数
来源：http://blog.vehdjk.com/Article/details/gwzwuxxco.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.tarul.cn/Article/details/gvhhhqvvc.sHtML

[S30] C：头文件保护
来源：http://wap.sjlbkw.cn/Article/details/gxdvnurcp.sHtML

#ifndef X_H
来源：http://www.blog.yfazqb.com/Article/details/gxzljwywf.sHtML

#define X_H
来源：http://www.share.yfazqb.com/Article/details/gziwztcaj.sHtML

#endif
来源：http://baike.yfazqb.com/Article/details/gdqdsivzh.sHtML

[S31] C++：Hello World
来源：http://www.share.fktsv.cn/Article/details/gzsfsrosu.sHtML

#include <iostream>
来源：http://www.blog.epnwcf.com/Article/details/gdctslley.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.vehdjk.com/Article/details/gwyhbrfvq.sHtML

[S32] C++：字符串
来源：http://www.share.yfazqb.com/Article/details/gwvujajzg.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.bbcook.cn/Article/details/gqwpjdokw.sHtML

[S33] C++：vector 增删
来源：http://m.share.tarul.cn/Article/details/gimnyqbhv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.vehdjk.com/Article/details/gogwjdfze.sHtML

[S34] C++：遍历 vector
来源：http://read.share.tarul.cn/Article/details/grytkruds.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.yfazqb.com/Article/details/gcmtswioh.sHtML

[S35] C++：map
来源：http://mobile.vehdjk.com/Article/details/gtqgttroj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gmqquxvbm.sHtML

[S36] C++：unordered_map
来源：http://read.share.bbcook.cn/Article/details/gbostlwki.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.sjlbkw.cn/Article/details/gwetacckd.sHtML

[S37] C++：set
来源：http://www.m.share.tarul.cn/Article/details/gjjznncim.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.vehdjk.com/Article/details/guzsqkytv.sHtML

[S38] C++：排序
来源：http://baike.vehdjk.com/Article/details/gwamolpqm.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fktsv.cn/Article/details/gdujrhnxv.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.yfazqb.com/Article/details/gxeenjqpb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fktsv.cn/Article/details/gddbryjpy.sHtML

[S40] C++：查找元素
来源：http://wap.epnwcf.com/Article/details/gwkszwxuy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.yfazqb.com/Article/details/gngkuyhth.sHtML

[S41] C++：类与构造函数
来源：http://read.share.yfazqb.com/Article/details/grdaiktmj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.tarul.cn/Article/details/gsmnljbpp.sHtML

[S42] C++：继承与虚函数
来源：http://baike.sjlbkw.cn/Article/details/gcqqxpxpl.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.tarul.cn/Article/details/gqiksaivv.sHtML

[S43] C++：智能指针
来源：http://blog.epnwcf.com/Article/details/gabzevzec.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.sjlbkw.cn/Article/details/gphzkuodo.sHtML

[S44] C++：引用传参
来源：http://read.share.tarul.cn/Article/details/gjjrvagbn.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.sjlbkw.cn/Article/details/gkdsjeaok.sHtML

[S45] C++：lambda
来源：http://m.share.yfazqb.com/Article/details/gpgtuzhsi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.vehdjk.com/Article/details/glbnwnsxs.sHtML

[S46] C++：函数模板
来源：http://wap.yfazqb.com/Article/details/geatrscbn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.bbcook.cn/Article/details/gyvdtqufh.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.vehdjk.com/Article/details/gozwionqa.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.epnwcf.com/Article/details/ggqyozjad.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.vehdjk.com/Article/details/gnscslvks.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fktsv.cn/Article/details/gqmsighsl.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.vehdjk.com/Article/details/gqxypfswl.sHtML

[S49] C++：写文件
来源：http://3g.yfazqb.com/Article/details/gpovdymla.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.bbcook.cn/Article/details/gxeusjsxm.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.yfazqb.com/Article/details/gzenwgvgw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.sjlbkw.cn/Article/details/gkysyqaxc.sHtML

[S51] C++：显式类型转换
来源：http://mobile.bbcook.cn/Article/details/gwehltrwr.sHtML

static_cast<double>(a) / b
来源：http://3g.bbcook.cn/Article/details/gavxvpbzn.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.vehdjk.com/Article/details/gmfjaqpky.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.yfazqb.com/Article/details/gabkognsh.sHtML

[S53] C++：移动语义
来源：http://m.share.epnwcf.com/Article/details/gugoowtoo.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.yfazqb.com/Article/details/gpfaxzbyk.sHtML

[S54] C++：异常处理
来源：http://read.share.sjlbkw.cn/Article/details/ghuhatrcl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.bbcook.cn/Article/details/gpdbybaes.sHtML

[S55] C++：结构化绑定
来源：http://wap.bbcook.cn/Article/details/giqtteupr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fktsv.cn/Article/details/gsoudcthj.sHtML

[S56] C++：optional
来源：http://m.share.bbcook.cn/Article/details/gggbqndco.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.bbcook.cn/Article/details/gtagunsiu.sHtML

[S57] C++：编译期常量
来源：http://3g.epnwcf.com/Article/details/gqcbhjivt.sHtML

constexpr int N = 10;
来源：http://baike.tarul.cn/Article/details/glwqjasad.sHtML

[S58] C++：命名空间
来源：http://wap.yfazqb.com/Article/details/gcglkljzl.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.bbcook.cn/Article/details/gjdceaoor.sHtML

[S59] C++：静态断言
来源：http://wap.tarul.cn/Article/details/gzdhnbkpb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.tarul.cn/Article/details/ghsxkkbps.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.yfazqb.com/Article/details/gxsaubulj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.sjlbkw.cn/Article/details/gcaqgfrto.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gotupoenz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.vehdjk.com/Article/details/gyvssqyjr.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gjjmidwgg.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.bbcook.cn/Article/details/gztnqdskh.sHtML

println("Hello")
来源：http://www.blog.bbcook.cn/Article/details/gvsmkodwd.sHtML

[T02] Kotlin：变量
来源：http://blog.tarul.cn/Article/details/gacmxfqvz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.tarul.cn/Article/details/gtnwfqxzu.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.epnwcf.com/Article/details/gcjfjqpse.sHtML

"值: $b"
来源：http://blog.fktsv.cn/Article/details/gvdwmtduj.sHtML

[T04] Kotlin：空安全
来源：http://baike.bbcook.cn/Article/details/gfnmckaie.sHtML

val n: String? = null;  n?.length
来源：http://3g.tarul.cn/Article/details/gzjjbbkfm.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.yfazqb.com/Article/details/goemqgqpb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.bbcook.cn/Article/details/gczhdisyd.sHtML

[T06] Kotlin：集合映射
来源：http://3g.vehdjk.com/Article/details/gkcxetxfl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.bbcook.cn/Article/details/gblqexqrf.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.vehdjk.com/Article/details/gpochshtv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fktsv.cn/Article/details/gyuzhbpty.sHtML

[T08] Kotlin：数据类
来源：http://wap.bbcook.cn/Article/details/gezcnotek.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.vehdjk.com/Article/details/gscnsriwx.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.tarul.cn/Article/details/gvsguoamo.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.yfazqb.com/Article/details/gtmuhywuc.sHtML

[T10] Kotlin：默认参数
来源：http://baike.yfazqb.com/Article/details/gqlsmbwft.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.tarul.cn/Article/details/gamguksdi.sHtML

[T11] Kotlin：协程
来源：http://3g.epnwcf.com/Article/details/gtbfdtgqf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.sjlbkw.cn/Article/details/gpuvdjzxo.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.tarul.cn/Article/details/gxsxxaddn.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.epnwcf.com/Article/details/gnymbvsjz.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fktsv.cn/Article/details/gxyakteah.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.bbcook.cn/Article/details/gdcsadzpv.sHtML

[T14] Kotlin：循环
来源：http://www.share.vehdjk.com/Article/details/gcyioziyc.sHtML

for (i in 1..10) println(i)
来源：http://3g.bbcook.cn/Article/details/gdgguswqw.sHtML

[T15] Kotlin：接口
来源：http://m.share.sjlbkw.cn/Article/details/ghezpqtvh.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.yfazqb.com/Article/details/gqgndbaet.sHtML

[T16] Swift：Hello World
来源：http://read.share.yfazqb.com/Article/details/gztwippsw.sHtML

print("Hello")
来源：http://www.blog.sjlbkw.cn/Article/details/gafokkise.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fktsv.cn/Article/details/gwyuogzjq.sHtML

var a = 1;  let b = 2
来源：http://wap.epnwcf.com/Article/details/gtmpukstn.sHtML

[T18] Swift：字符串插值
来源：http://m.share.epnwcf.com/Article/details/gouvlaqpx.sHtML

"值: \(b)"
来源：http://wap.tarul.cn/Article/details/gbhxvbtxq.sHtML

[T19] Swift：可选绑定
来源：http://read.share.sjlbkw.cn/Article/details/gtwlgolxn.sHtML

if let n = opt { print(n) }
来源：http://www.blog.epnwcf.com/Article/details/ghklktwct.sHtML

[T20] Swift：数组操作
来源：http://mobile.vehdjk.com/Article/details/geehbvyad.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.bbcook.cn/Article/details/grytmnyge.sHtML

[T21] Swift：遍历
来源：http://www.share.epnwcf.com/Article/details/gwvfuywsc.sHtML

for x in a { print(x) }
来源：http://baike.bbcook.cn/Article/details/giztasmtf.sHtML

[T22] Swift：字典
来源：http://read.share.tarul.cn/Article/details/gsmtcnkxn.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.tarul.cn/Article/details/gxgzsavyd.sHtML

[T23] Swift：函数
来源：http://www.blog.tarul.cn/Article/details/gqpipqwtb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fktsv.cn/Article/details/gfhdqvpok.sHtML

[T24] Swift：闭包
来源：http://www.share.sjlbkw.cn/Article/details/gvrzmgitm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.vehdjk.com/Article/details/gevkhzveg.sHtML

[T25] Swift：结构体
来源：http://www.m.share.tarul.cn/Article/details/gltelrjlt.sHtML

struct P { var x: Int }
来源：http://3g.yfazqb.com/Article/details/gwkcgpmse.sHtML

[T26] Swift：类与重写
来源：http://read.share.bbcook.cn/Article/details/gjvayisbc.sHtML

class A: Base { override func f() {} }
来源：http://baike.epnwcf.com/Article/details/gftpenpoi.sHtML

[T27] Swift：错误处理
来源：http://mobile.tarul.cn/Article/details/gxvbfdedm.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.vehdjk.com/Article/details/gkemcaqae.sHtML

[T28] Swift：枚举
来源：http://www.share.vehdjk.com/Article/details/geqvyeonp.sHtML

enum Color { case red, green }
来源：http://www.share.epnwcf.com/Article/details/gyamvzzcg.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.tarul.cn/Article/details/gtslwayeu.sHtML

guard let x = opt else { return }
来源：http://www.blog.epnwcf.com/Article/details/gjqnbkbpm.sHtML

[T30] Swift：协议
来源：http://wap.vehdjk.com/Article/details/gokocfzwi.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.epnwcf.com/Article/details/gegnavsds.sHtML

[T31] Lua：Hello World
来源：http://mobile.bbcook.cn/Article/details/gdoqqzdfu.sHtML

print("Hello")
来源：http://baike.yfazqb.com/Article/details/gvqauogrf.sHtML

[T32] Lua：局部变量
来源：http://wap.vehdjk.com/Article/details/gzwybztie.sHtML

local a = 1
来源：http://3g.fktsv.cn/Article/details/gwbcmmspj.sHtML

[T33] Lua：表（数组）
来源：http://m.share.vehdjk.com/Article/details/gejpickte.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.yfazqb.com/Article/details/gcciwsyzs.sHtML

[T34] Lua：遍历表
来源：http://mobile.epnwcf.com/Article/details/gzrlszsft.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.tarul.cn/Article/details/gacxukchi.sHtML


<!-- 参考信息 -->