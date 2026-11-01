代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.yfazqb.com/Article/details/gkczvnswc.sHtML

[R36] 并发执行多个任务
来源：http://mobile.epnwcf.com/Article/details/gemlfoujh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.epnwcf.com/Article/details/gqytikjid.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.sjlbkw.cn/Article/details/gzzcxlpgc.sHtML

files=$(ls -1)
来源：http://www.blog.epnwcf.com/Article/details/grrxeftrg.sHtML

[R38] 管道串联
来源：http://m.share.vehdjk.com/Article/details/gshtimoqu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.bbcook.cn/Article/details/ghwnydlbt.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.bbcook.cn/Article/details/gicsmtskj.sHtML

cmd > out.log 2>&1
来源：http://read.share.vehdjk.com/Article/details/gmdowuvfn.sHtML

[R40] 追加写日志
来源：http://blog.bbcook.cn/Article/details/gasitfhtx.sHtML

echo "log" >> out.log
来源：http://www.blog.bbcook.cn/Article/details/gmrqipams.sHtML

[R41] 丢弃输出
来源：http://www.blog.yfazqb.com/Article/details/gmdmtufcr.sHtML

cmd >/dev/null 2>&1
来源：http://wap.yfazqb.com/Article/details/gbolkfdmp.sHtML

[R42] 输入重定向
来源：http://www.share.yfazqb.com/Article/details/gwnyjgchf.sHtML

wc -l < a.txt
来源：http://read.share.epnwcf.com/Article/details/gcuzmlfsa.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fktsv.cn/Article/details/gdnrxqget.sHtML

find . -name "*.log" -type f
来源：http://read.share.vehdjk.com/Article/details/glddctqni.sHtML

[R44] 按修改时间查找
来源：http://www.blog.bbcook.cn/Article/details/gmpcndgcw.sHtML

find . -mtime -7 -type f
来源：http://m.share.tarul.cn/Article/details/gjfkbxhta.sHtML

[R45] 批量删除
来源：http://www.share.vehdjk.com/Article/details/gsmegflfy.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.tarul.cn/Article/details/gzyaaxrre.sHtML

[R46] 递归替换文件内容
来源：http://m.share.vehdjk.com/Article/details/gvlruwpfr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.epnwcf.com/Article/details/ggjvianva.sHtML

[R47] sed 单行替换
来源：http://read.share.tarul.cn/Article/details/ggbrhatrc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.yfazqb.com/Article/details/guyygsnik.sHtML

[R48] awk 取指定列
来源：http://mobile.epnwcf.com/Article/details/gycrywakw.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fktsv.cn/Article/details/gystwmdrc.sHtML

[R49] awk 带条件
来源：http://www.m.share.tarul.cn/Article/details/gxwqwsxrc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.epnwcf.com/Article/details/gligafmnr.sHtML

[R50] awk 求和
来源：http://mobile.bbcook.cn/Article/details/gcfswdjxy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.yfazqb.com/Article/details/ggauocagw.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.sjlbkw.cn/Article/details/gpdvangmt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.epnwcf.com/Article/details/gentvgftm.sHtML

[R52] 统计行数
来源：http://mobile.yfazqb.com/Article/details/gecjxvxsf.sHtML

wc -l a.txt
来源：http://wap.sjlbkw.cn/Article/details/glvabcgse.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.epnwcf.com/Article/details/gfbocvzaw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.sjlbkw.cn/Article/details/gjedcqshl.sHtML

[R54] 比较两个文件
来源：http://m.share.fktsv.cn/Article/details/gebxevspf.sHtML

diff a.txt b.txt
来源：http://mobile.bbcook.cn/Article/details/giyardsrr.sHtML

[R55] 压缩与解压
来源：http://www.m.share.tarul.cn/Article/details/gxqpegmtg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.tarul.cn/Article/details/grjveokba.sHtML

[R56] 远程拷贝
来源：http://baike.epnwcf.com/Article/details/gpmvexmrj.sHtML

scp file user@host:/path/
来源：http://3g.bbcook.cn/Article/details/ghjbkpfue.sHtML

[R57] 远程执行命令
来源：http://read.share.fktsv.cn/Article/details/guatmbigs.sHtML

ssh user@host 'uptime'
来源：http://m.share.tarul.cn/Article/details/godygfkww.sHtML

[R58] 下载文件
来源：http://m.share.vehdjk.com/Article/details/gwrhhmdga.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.sjlbkw.cn/Article/details/gzffwklqg.sHtML

[R59] 发 POST JSON
来源：http://wap.sjlbkw.cn/Article/details/gjmwwdgxn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.tarul.cn/Article/details/gwogxklpx.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.sjlbkw.cn/Article/details/gxcunmmqt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.vehdjk.com/Article/details/grxaelhwz.sHtML

[R61] 磁盘占用
来源：http://mobile.yfazqb.com/Article/details/gqklnunlr.sHtML

df -h;  du -sh *
来源：http://wap.epnwcf.com/Article/details/gpccnfbxb.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.tarul.cn/Article/details/gfbdntjzh.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.epnwcf.com/Article/details/gzbykbmja.sHtML

[R63] 内存与进程
来源：http://mobile.bbcook.cn/Article/details/gfdoukcvg.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.epnwcf.com/Article/details/gznqrbtup.sHtML

[R64] 结束进程
来源：http://www.share.epnwcf.com/Article/details/gjltndgqv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.yfazqb.com/Article/details/gtpwemsjs.sHtML

[R65] 查看端口占用
来源：http://blog.yfazqb.com/Article/details/gmyhogjlh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.tarul.cn/Article/details/gscydmckv.sHtML

[R66] 定时任务
来源：http://wap.tarul.cn/Article/details/grddrpswa.sHtML

crontab -e;  crontab -l
来源：http://mobile.tarul.cn/Article/details/gccjprapg.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.bbcook.cn/Article/details/gnevlxrnl.sHtML

openssl rand -hex 16
来源：http://wap.tarul.cn/Article/details/gjblhopww.sHtML

[R68] 计算文件校验值
来源：http://baike.sjlbkw.cn/Article/details/gexmageht.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.bbcook.cn/Article/details/granmlzwd.sHtML

[R69] 生成随机密码
来源：http://www.m.share.epnwcf.com/Article/details/gfdsccgzm.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.epnwcf.com/Article/details/gnpirkflw.sHtML

[R70] 时间戳与互转
来源：http://3g.epnwcf.com/Article/details/gbkbbnwft.sHtML

date +%s;  date -d @1700000000
来源：http://baike.tarul.cn/Article/details/gcxjhgnqg.sHtML

[R71] 日期格式化
来源：http://www.share.sjlbkw.cn/Article/details/gsmwrbyxx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.bbcook.cn/Article/details/gcveajuku.sHtML

[R72] 等待端口就绪
来源：http://mobile.vehdjk.com/Article/details/gommkukml.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.bbcook.cn/Article/details/gjnlumbfe.sHtML

[R73] 分割大日志
来源：http://3g.bbcook.cn/Article/details/gwsmggzpm.sHtML

split -l 1000 big.log part_
来源：http://read.share.sjlbkw.cn/Article/details/guserbcpq.sHtML

[R74] 批量重命名
来源：http://blog.sjlbkw.cn/Article/details/ghfoqaisp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gzbdplysy.sHtML

[R75] 导出环境变量
来源：http://read.share.tarul.cn/Article/details/gullcheua.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.bbcook.cn/Article/details/gkhnkgiuk.sHtML

[R76] 使用临时文件
来源：http://blog.fktsv.cn/Article/details/gmlbabnry.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fktsv.cn/Article/details/gxgmhjqbm.sHtML

[R77] 读取用户输入
来源：http://blog.fktsv.cn/Article/details/glxmzahdw.sHtML

read -rp "请输入: " ans
来源：http://www.blog.tarul.cn/Article/details/gnjaixpen.sHtML

[R78] 交互式菜单
来源：http://m.share.sjlbkw.cn/Article/details/gmogpmeaq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.sjlbkw.cn/Article/details/gibrtyool.sHtML

[R79] 解析命令行选项
来源：http://read.share.tarul.cn/Article/details/gmqqjdwen.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.yfazqb.com/Article/details/gtxlzzdiu.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.sjlbkw.cn/Article/details/gwxewkybp.sHtML

time ./run.sh
来源：http://www.m.share.fktsv.cn/Article/details/gdyjsvfsp.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/glewlsiux.sHtML

S. C / C++ 专题
来源：http://3g.epnwcf.com/Article/details/gxlgtluci.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/ggzyijhkz.sHtML

[S01] C：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/gafoxoyni.sHtML

#include <stdio.h>
来源：http://www.m.share.tarul.cn/Article/details/gptlepewx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.bbcook.cn/Article/details/gukbnekjy.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.epnwcf.com/Article/details/giezkevte.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.bbcook.cn/Article/details/ggoxtphai.sHtML

[S03] C：读入整数
来源：http://www.blog.bbcook.cn/Article/details/gnbmelwbq.sHtML

int x; scanf("%d", &x);
来源：http://baike.vehdjk.com/Article/details/gdwwdxzfq.sHtML

[S04] C：字符串复制
来源：http://www.m.share.tarul.cn/Article/details/gtmtmowrf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.vehdjk.com/Article/details/ghbajxmri.sHtML

[S05] C：字符串长度
来源：http://www.m.share.tarul.cn/Article/details/gngrmxsdp.sHtML

strlen(s)
来源：http://blog.yfazqb.com/Article/details/gsjnovmdp.sHtML

[S06] C：字符串比较
来源：http://read.share.tarul.cn/Article/details/gtmbjbsvp.sHtML

strcmp(a, b) == 0
来源：http://3g.yfazqb.com/Article/details/gyjrhivmh.sHtML

[S07] C：数组遍历求和
来源：http://wap.yfazqb.com/Article/details/gozzqolpv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.sjlbkw.cn/Article/details/gvwfmznfd.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.epnwcf.com/Article/details/gqeokgaao.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.tarul.cn/Article/details/gptpbqgse.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.sjlbkw.cn/Article/details/gtyanyngr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.sjlbkw.cn/Article/details/gtauozcls.sHtML

[S10] C：指针与解引用
来源：http://www.blog.epnwcf.com/Article/details/gigexdafc.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.vehdjk.com/Article/details/gfyaefjuf.sHtML

[S11] C：逐行读文件
来源：http://read.share.tarul.cn/Article/details/gwcavsmfe.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fktsv.cn/Article/details/gampsvvzs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.yfazqb.com/Article/details/gkbldhtso.sHtML

fclose(f);
来源：http://3g.bbcook.cn/Article/details/giwolehqm.sHtML

[S12] C：写文件
来源：http://3g.bbcook.cn/Article/details/ggghpnjuy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.yfazqb.com/Article/details/ggpzylyfb.sHtML

[S13] C：宏定义
来源：http://m.share.epnwcf.com/Article/details/gljbjkfsk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.epnwcf.com/Article/details/gftbiyrtz.sHtML

[S14] C：枚举
来源：http://www.m.share.epnwcf.com/Article/details/gtkkpxvda.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.yfazqb.com/Article/details/gpuyvwmvc.sHtML

[S15] C：类型转换
来源：http://www.blog.yfazqb.com/Article/details/gnxyuplzx.sHtML

(double) a / b
来源：http://mobile.epnwcf.com/Article/details/gnaddelnt.sHtML

[S16] C：位操作置位
来源：http://www.share.tarul.cn/Article/details/glcjipvyw.sHtML

x |= (1 << 3);
来源：http://www.m.share.bbcook.cn/Article/details/giooawlij.sHtML

[S17] C：安全拼接字符串
来源：http://wap.epnwcf.com/Article/details/gybiqxyzo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.epnwcf.com/Article/details/gaeqamspm.sHtML

[S18] C：命令行参数
来源：http://www.m.share.yfazqb.com/Article/details/gjyxdxuyy.sHtML

int main(int argc, char **argv)
来源：http://m.share.epnwcf.com/Article/details/gatqfpwth.sHtML

[S19] C：快速排序
来源：http://read.share.bbcook.cn/Article/details/gbpxivwsl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.yfazqb.com/Article/details/gavnytbua.sHtML

[S20] C：二分查找
来源：http://mobile.sjlbkw.cn/Article/details/gsrsgmgun.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.epnwcf.com/Article/details/gvvigayzh.sHtML

[S21] C：字符类别判断
来源：http://read.share.fktsv.cn/Article/details/gypetmehf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.sjlbkw.cn/Article/details/gqzzpeyxn.sHtML

[S22] C：字符串转数字
来源：http://www.blog.yfazqb.com/Article/details/gypgrwqoe.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fktsv.cn/Article/details/gjehgxddd.sHtML

[S23] C：随机数
来源：http://mobile.fktsv.cn/Article/details/gfvxgrruz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.bbcook.cn/Article/details/gemhlrlmx.sHtML

[S24] C：获取本地时间
来源：http://mobile.fktsv.cn/Article/details/gdswjgiwi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.yfazqb.com/Article/details/ghvcxjzkt.sHtML

[S25] C：内存拷贝
来源：http://m.share.sjlbkw.cn/Article/details/gcnnqiivt.sHtML

memcpy(dst, src, n);
来源：http://3g.tarul.cn/Article/details/ggrdtdlfg.sHtML

[S26] C：内存清零
来源：http://wap.bbcook.cn/Article/details/gwietjrqw.sHtML

memset(a, 0, sizeof a);
来源：http://wap.yfazqb.com/Article/details/gwtlihlhc.sHtML

[S27] C：定义常量
来源：http://3g.bbcook.cn/Article/details/geukwncgu.sHtML

const double PI = 3.14159;
来源：http://mobile.bbcook.cn/Article/details/gxrwkmtvp.sHtML

[S28] C：静态变量
来源：http://baike.fktsv.cn/Article/details/goifmhoeu.sHtML

static int counter = 0;
来源：http://read.share.yfazqb.com/Article/details/gztyvmbew.sHtML

[S29] C：变参函数
来源：http://www.m.share.yfazqb.com/Article/details/ghwhweutn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.tarul.cn/Article/details/gazimllip.sHtML

[S30] C：头文件保护
来源：http://3g.fktsv.cn/Article/details/glgeflbpx.sHtML

#ifndef X_H
来源：http://mobile.vehdjk.com/Article/details/gyzczgvzu.sHtML

#define X_H
来源：http://www.blog.bbcook.cn/Article/details/gsxrkwewb.sHtML

#endif
来源：http://www.blog.tarul.cn/Article/details/gmpremzan.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gjfnjzdkd.sHtML

#include <iostream>
来源：http://3g.bbcook.cn/Article/details/gxugjkftr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fktsv.cn/Article/details/gtqtjgcde.sHtML

[S32] C++：字符串
来源：http://mobile.yfazqb.com/Article/details/gdlkqjjaw.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.vehdjk.com/Article/details/gtahmknuc.sHtML

[S33] C++：vector 增删
来源：http://www.share.fktsv.cn/Article/details/gomdzrttx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.sjlbkw.cn/Article/details/gadbuhnkd.sHtML

[S34] C++：遍历 vector
来源：http://baike.bbcook.cn/Article/details/goagjzvwa.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.epnwcf.com/Article/details/ggchsfwxh.sHtML

[S35] C++：map
来源：http://baike.bbcook.cn/Article/details/gjbphbcrb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.sjlbkw.cn/Article/details/gkjdptoyx.sHtML

[S36] C++：unordered_map
来源：http://wap.yfazqb.com/Article/details/gyezqosof.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fktsv.cn/Article/details/gyplfjjch.sHtML

[S37] C++：set
来源：http://www.blog.fktsv.cn/Article/details/gtmwdlhmi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.yfazqb.com/Article/details/gkawaeoql.sHtML

[S38] C++：排序
来源：http://m.share.sjlbkw.cn/Article/details/gybvzslkm.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fktsv.cn/Article/details/gtvvotulh.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.bbcook.cn/Article/details/gfccmlwhx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.yfazqb.com/Article/details/goqyugiba.sHtML

[S40] C++：查找元素
来源：http://mobile.fktsv.cn/Article/details/grdishnat.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.vehdjk.com/Article/details/guxixxmap.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fktsv.cn/Article/details/ghomxhdgf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.yfazqb.com/Article/details/gdvooejxl.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.epnwcf.com/Article/details/gnyjjboao.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.epnwcf.com/Article/details/gknskafkr.sHtML

[S43] C++：智能指针
来源：http://www.m.share.bbcook.cn/Article/details/grpjpogni.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.yfazqb.com/Article/details/gwetqpbke.sHtML

[S44] C++：引用传参
来源：http://www.share.tarul.cn/Article/details/gwnhmjigs.sHtML

void inc(int &x) { ++x; }
来源：http://3g.bbcook.cn/Article/details/guzduklur.sHtML

[S45] C++：lambda
来源：http://wap.epnwcf.com/Article/details/gwqjkdlmr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.tarul.cn/Article/details/gkcolokdo.sHtML

[S46] C++：函数模板
来源：http://www.blog.yfazqb.com/Article/details/garwbpjwk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.tarul.cn/Article/details/gffyvwjgl.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.yfazqb.com/Article/details/gdvpxlfpe.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.sjlbkw.cn/Article/details/gtnyfbcko.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.bbcook.cn/Article/details/gfvjmtozp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.tarul.cn/Article/details/gevbrodqm.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fktsv.cn/Article/details/givopxhgi.sHtML

[S49] C++：写文件
来源：http://www.share.vehdjk.com/Article/details/ggjtjaims.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fktsv.cn/Article/details/gdcipzrtr.sHtML

[S50] C++：格式化数字
来源：http://3g.fktsv.cn/Article/details/gxggerryd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fktsv.cn/Article/details/ghohrlhtu.sHtML

[S51] C++：显式类型转换
来源：http://read.share.bbcook.cn/Article/details/ggzbxzrhh.sHtML

static_cast<double>(a) / b
来源：http://wap.yfazqb.com/Article/details/gfujwkymt.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.yfazqb.com/Article/details/gkwrshgiv.sHtML

int size() const noexcept { return n_; }
来源：http://baike.sjlbkw.cn/Article/details/gsyeabead.sHtML

[S53] C++：移动语义
来源：http://www.share.bbcook.cn/Article/details/gslxunsju.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.epnwcf.com/Article/details/ghfhtevne.sHtML

[S54] C++：异常处理
来源：http://mobile.yfazqb.com/Article/details/gibmflsqi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.epnwcf.com/Article/details/gijsatujx.sHtML

[S55] C++：结构化绑定
来源：http://3g.epnwcf.com/Article/details/gpovvnefd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.bbcook.cn/Article/details/gqkoknriu.sHtML

[S56] C++：optional
来源：http://mobile.epnwcf.com/Article/details/gulswhmha.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.epnwcf.com/Article/details/gadpokxhj.sHtML

[S57] C++：编译期常量
来源：http://wap.tarul.cn/Article/details/gaitorksw.sHtML

constexpr int N = 10;
来源：http://www.share.fktsv.cn/Article/details/gardeazve.sHtML

[S58] C++：命名空间
来源：http://m.share.epnwcf.com/Article/details/gecszbmdm.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.bbcook.cn/Article/details/grwavknhw.sHtML

[S59] C++：静态断言
来源：http://3g.tarul.cn/Article/details/gmwridnze.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.sjlbkw.cn/Article/details/geuxeavwq.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.vehdjk.com/Article/details/gpmgsqtux.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.yfazqb.com/Article/details/gcxhtqpsz.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gnnabhrfg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.sjlbkw.cn/Article/details/gammxdzcw.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gjizxqpig.sHtML

[T01] Kotlin：Hello World
来源：http://blog.tarul.cn/Article/details/garwxrwcl.sHtML

println("Hello")
来源：http://mobile.tarul.cn/Article/details/gfaesdjhd.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fktsv.cn/Article/details/gczjfmuqx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.yfazqb.com/Article/details/gubfypyip.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.bbcook.cn/Article/details/grgnnalnr.sHtML

"值: $b"
来源：http://baike.yfazqb.com/Article/details/gvlmitlcd.sHtML

[T04] Kotlin：空安全
来源：http://3g.epnwcf.com/Article/details/gvhmaovul.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.yfazqb.com/Article/details/gbszfnxdz.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.epnwcf.com/Article/details/gytyilxqf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.tarul.cn/Article/details/gyrgluztl.sHtML

[T06] Kotlin：集合映射
来源：http://3g.bbcook.cn/Article/details/gqwpbolka.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.sjlbkw.cn/Article/details/gfxeeavhd.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.sjlbkw.cn/Article/details/gsivuvocn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.epnwcf.com/Article/details/grwfupekc.sHtML

[T08] Kotlin：数据类
来源：http://m.share.tarul.cn/Article/details/gheuqxpwz.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.tarul.cn/Article/details/gtrolosgr.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.tarul.cn/Article/details/gtcbzilqy.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.vehdjk.com/Article/details/gwnqavmvb.sHtML

[T10] Kotlin：默认参数
来源：http://3g.epnwcf.com/Article/details/gnwtxcfhn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.vehdjk.com/Article/details/gkhkjoqbs.sHtML

[T11] Kotlin：协程
来源：http://baike.yfazqb.com/Article/details/gllljkfla.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.yfazqb.com/Article/details/gtnqzoewo.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.yfazqb.com/Article/details/gwyfwwlbo.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.yfazqb.com/Article/details/gwefermvx.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.vehdjk.com/Article/details/glkplbvrs.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfzvzrmqz.sHtML

[T14] Kotlin：循环
来源：http://mobile.bbcook.cn/Article/details/ghiiraurp.sHtML

for (i in 1..10) println(i)
来源：http://read.share.tarul.cn/Article/details/gbpdsvyik.sHtML

[T15] Kotlin：接口
来源：http://www.share.yfazqb.com/Article/details/gnzukfhum.sHtML

interface Shape { fun area(): Double }
来源：http://3g.vehdjk.com/Article/details/gcuswqjnl.sHtML

[T16] Swift：Hello World
来源：http://mobile.bbcook.cn/Article/details/gpeuqmrxh.sHtML

print("Hello")
来源：http://www.blog.fktsv.cn/Article/details/gylbgsmyq.sHtML

[T17] Swift：变量与常量
来源：http://mobile.yfazqb.com/Article/details/ggaywehvz.sHtML

var a = 1;  let b = 2
来源：http://read.share.fktsv.cn/Article/details/gpqnrymgn.sHtML

[T18] Swift：字符串插值
来源：http://www.share.bbcook.cn/Article/details/ghcydqjry.sHtML

"值: \(b)"
来源：http://3g.epnwcf.com/Article/details/gleiesijk.sHtML

[T19] Swift：可选绑定
来源：http://read.share.sjlbkw.cn/Article/details/gcomzrrvl.sHtML

if let n = opt { print(n) }
来源：http://read.share.bbcook.cn/Article/details/gldyxckei.sHtML

[T20] Swift：数组操作
来源：http://3g.vehdjk.com/Article/details/gbhbacyuu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.tarul.cn/Article/details/gowazzlpy.sHtML

[T21] Swift：遍历
来源：http://www.share.yfazqb.com/Article/details/gojhnomdn.sHtML

for x in a { print(x) }
来源：http://www.share.tarul.cn/Article/details/gmlhkjhsn.sHtML

[T22] Swift：字典
来源：http://www.blog.tarul.cn/Article/details/grhzylzht.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.bbcook.cn/Article/details/gntsxrhus.sHtML

[T23] Swift：函数
来源：http://wap.epnwcf.com/Article/details/gmoigrxde.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpywjmmit.sHtML

[T24] Swift：闭包
来源：http://read.share.epnwcf.com/Article/details/gqipctssa.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.tarul.cn/Article/details/gtrjkwesk.sHtML

[T25] Swift：结构体
来源：http://www.share.bbcook.cn/Article/details/gabkuymtq.sHtML

struct P { var x: Int }
来源：http://mobile.tarul.cn/Article/details/ghbqlamgi.sHtML

[T26] Swift：类与重写
来源：http://read.share.bbcook.cn/Article/details/gfmnelgix.sHtML

class A: Base { override func f() {} }
来源：http://3g.sjlbkw.cn/Article/details/gdeqwttei.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fktsv.cn/Article/details/gagrdlqkh.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.yfazqb.com/Article/details/ghnpeqhvx.sHtML

[T28] Swift：枚举
来源：http://baike.yfazqb.com/Article/details/gegelisve.sHtML

enum Color { case red, green }
来源：http://m.share.yfazqb.com/Article/details/ghrzyltcc.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.bbcook.cn/Article/details/gwwnzfmng.sHtML

guard let x = opt else { return }
来源：http://mobile.vehdjk.com/Article/details/gaoefbzre.sHtML

[T30] Swift：协议
来源：http://blog.fktsv.cn/Article/details/gjfoilmjx.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.bbcook.cn/Article/details/gjtqucexm.sHtML

[T31] Lua：Hello World
来源：http://wap.bbcook.cn/Article/details/gjfvlvodo.sHtML

print("Hello")
来源：http://blog.tarul.cn/Article/details/gfivdspgb.sHtML

[T32] Lua：局部变量
来源：http://blog.tarul.cn/Article/details/gcncmzoqt.sHtML

local a = 1
来源：http://www.m.share.fktsv.cn/Article/details/gbbvnsjxi.sHtML

[T33] Lua：表（数组）
来源：http://www.share.tarul.cn/Article/details/ghpoztnrh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.bbcook.cn/Article/details/gptphyrrn.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.epnwcf.com/Article/details/gtskjtsms.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.epnwcf.com/Article/details/gtdraxdbf.sHtML

[T35] Lua：字典表
来源：http://3g.sjlbkw.cn/Article/details/gzqfukptc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fktsv.cn/Article/details/gnemqavjb.sHtML

[T36] Lua：函数
来源：http://read.share.yfazqb.com/Article/details/gbzlylnwt.sHtML

function add(a, b) return a + b end
来源：http://wap.vehdjk.com/Article/details/geknyybup.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.bbcook.cn/Article/details/gpkyvsdbi.sHtML

"a" .. "b"
来源：http://blog.fktsv.cn/Article/details/grhxdwszh.sHtML

[T38] Lua：条件
来源：http://www.share.bbcook.cn/Article/details/gvilsjwub.sHtML

if x > 0 then print("正") end
来源：http://m.share.tarul.cn/Article/details/gxkhdwixo.sHtML


<!-- 参考信息 -->