代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.tarul.cn/Article/details/gzdjpgtwp.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fktsv.cn/Article/details/gdsuwrzbb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.tarul.cn/Article/details/gfvguqdmh.sHtML

[R37] 把输出赋给变量
来源：http://read.share.epnwcf.com/Article/details/gcnbsvrcl.sHtML

files=$(ls -1)
来源：http://m.share.bbcook.cn/Article/details/gnclhwolz.sHtML

[R38] 管道串联
来源：http://mobile.fktsv.cn/Article/details/gdmxcbplc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.yfazqb.com/Article/details/gzajcyndt.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.tarul.cn/Article/details/gfwrrvgjj.sHtML

cmd > out.log 2>&1
来源：http://m.share.sjlbkw.cn/Article/details/gsnlsxdse.sHtML

[R40] 追加写日志
来源：http://www.m.share.bbcook.cn/Article/details/glrtceqqv.sHtML

echo "log" >> out.log
来源：http://www.m.share.fktsv.cn/Article/details/gwrcaugos.sHtML

[R41] 丢弃输出
来源：http://mobile.sjlbkw.cn/Article/details/gtfafdlib.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.bbcook.cn/Article/details/gaodutsso.sHtML

[R42] 输入重定向
来源：http://wap.fktsv.cn/Article/details/gzdsyigjp.sHtML

wc -l < a.txt
来源：http://mobile.sjlbkw.cn/Article/details/gngumqfrn.sHtML

[R43] 按名字查找文件
来源：http://read.share.sjlbkw.cn/Article/details/gxdovdjrs.sHtML

find . -name "*.log" -type f
来源：http://www.share.yfazqb.com/Article/details/ggodsarly.sHtML

[R44] 按修改时间查找
来源：http://www.blog.sjlbkw.cn/Article/details/giautkkbo.sHtML

find . -mtime -7 -type f
来源：http://read.share.yfazqb.com/Article/details/gxqetpdmq.sHtML

[R45] 批量删除
来源：http://www.blog.sjlbkw.cn/Article/details/gjonqboag.sHtML

find . -name "*.tmp" -delete
来源：http://wap.vehdjk.com/Article/details/grnpoazrq.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fktsv.cn/Article/details/gorvitupx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.epnwcf.com/Article/details/ghbzcrfzd.sHtML

[R47] sed 单行替换
来源：http://3g.sjlbkw.cn/Article/details/ghxcxsony.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.yfazqb.com/Article/details/grzvworda.sHtML

[R48] awk 取指定列
来源：http://www.m.share.yfazqb.com/Article/details/gpxxvvcfb.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.tarul.cn/Article/details/gmpwartwy.sHtML

[R49] awk 带条件
来源：http://www.share.bbcook.cn/Article/details/gkwtpaoev.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.vehdjk.com/Article/details/ghmvtolhn.sHtML

[R50] awk 求和
来源：http://m.share.vehdjk.com/Article/details/gmapizucl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.tarul.cn/Article/details/gcatozbsb.sHtML

[R51] 排序去重取前几
来源：http://www.share.epnwcf.com/Article/details/gmmuwbxrp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.bbcook.cn/Article/details/ghtqbpryg.sHtML

[R52] 统计行数
来源：http://www.m.share.yfazqb.com/Article/details/giomroddo.sHtML

wc -l a.txt
来源：http://m.share.yfazqb.com/Article/details/gqrdisste.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.tarul.cn/Article/details/gbocqlgsu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.vehdjk.com/Article/details/glqynwcgt.sHtML

[R54] 比较两个文件
来源：http://read.share.yfazqb.com/Article/details/gnzgmcijy.sHtML

diff a.txt b.txt
来源：http://www.blog.bbcook.cn/Article/details/gxjojtdki.sHtML

[R55] 压缩与解压
来源：http://www.blog.tarul.cn/Article/details/gdpjnovzi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.sjlbkw.cn/Article/details/godnmdweo.sHtML

[R56] 远程拷贝
来源：http://baike.yfazqb.com/Article/details/ggtrnaddn.sHtML

scp file user@host:/path/
来源：http://www.m.share.epnwcf.com/Article/details/garkprfxu.sHtML

[R57] 远程执行命令
来源：http://wap.yfazqb.com/Article/details/guzaevfxx.sHtML

ssh user@host 'uptime'
来源：http://www.blog.yfazqb.com/Article/details/gtvlzlfgn.sHtML

[R58] 下载文件
来源：http://3g.epnwcf.com/Article/details/gqebkbekc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.epnwcf.com/Article/details/ggyimsisd.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fktsv.cn/Article/details/gbqgrqlzp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.bbcook.cn/Article/details/gllcvbapa.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.bbcook.cn/Article/details/ggeookqje.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.yfazqb.com/Article/details/grdnkzmgc.sHtML

[R61] 磁盘占用
来源：http://mobile.bbcook.cn/Article/details/gkxdgokhc.sHtML

df -h;  du -sh *
来源：http://www.m.share.tarul.cn/Article/details/gslwswbws.sHtML

[R62] 找最占空间的文件
来源：http://baike.tarul.cn/Article/details/gnnpenhxh.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fktsv.cn/Article/details/giqnopcfl.sHtML

[R63] 内存与进程
来源：http://www.m.share.sjlbkw.cn/Article/details/gtddmfrrl.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fktsv.cn/Article/details/gqgcsfbpl.sHtML

[R64] 结束进程
来源：http://www.m.share.vehdjk.com/Article/details/gknvvkrug.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.vehdjk.com/Article/details/ghhhsvgom.sHtML

[R65] 查看端口占用
来源：http://mobile.sjlbkw.cn/Article/details/gisncjprx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.tarul.cn/Article/details/ghzuijatc.sHtML

[R66] 定时任务
来源：http://www.blog.bbcook.cn/Article/details/gbyqkesze.sHtML

crontab -e;  crontab -l
来源：http://www.share.tarul.cn/Article/details/gboissezd.sHtML

[R67] 生成随机十六进制串
来源：http://3g.yfazqb.com/Article/details/gwfayvxoq.sHtML

openssl rand -hex 16
来源：http://www.blog.tarul.cn/Article/details/gylveusvn.sHtML

[R68] 计算文件校验值
来源：http://read.share.vehdjk.com/Article/details/gberqlvsr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.epnwcf.com/Article/details/gvlmfzyug.sHtML

[R69] 生成随机密码
来源：http://blog.fktsv.cn/Article/details/gdkijnmti.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.epnwcf.com/Article/details/gtvttdxby.sHtML

[R70] 时间戳与互转
来源：http://baike.tarul.cn/Article/details/glkzvwvzo.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.epnwcf.com/Article/details/goadokzry.sHtML

[R71] 日期格式化
来源：http://m.share.fktsv.cn/Article/details/gzilwshjq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fktsv.cn/Article/details/gmzidwsac.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fktsv.cn/Article/details/gfvkskcbh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.epnwcf.com/Article/details/gpmltjwja.sHtML

[R73] 分割大日志
来源：http://mobile.epnwcf.com/Article/details/gtbzczxsi.sHtML

split -l 1000 big.log part_
来源：http://blog.yfazqb.com/Article/details/gcermnfoj.sHtML

[R74] 批量重命名
来源：http://mobile.tarul.cn/Article/details/ggrzliile.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.epnwcf.com/Article/details/gljawlbrz.sHtML

[R75] 导出环境变量
来源：http://www.m.share.vehdjk.com/Article/details/gcwqhfhuz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.epnwcf.com/Article/details/ghlsndblq.sHtML

[R76] 使用临时文件
来源：http://www.m.share.bbcook.cn/Article/details/ghoeryhcx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.epnwcf.com/Article/details/gynfvesud.sHtML

[R77] 读取用户输入
来源：http://read.share.tarul.cn/Article/details/gvzwxxmhs.sHtML

read -rp "请输入: " ans
来源：http://m.share.tarul.cn/Article/details/gbuslltgu.sHtML

[R78] 交互式菜单
来源：http://mobile.fktsv.cn/Article/details/gedkygisg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.yfazqb.com/Article/details/gicerpedp.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fktsv.cn/Article/details/gnhwdxeoc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.sjlbkw.cn/Article/details/gmnepgcbt.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.bbcook.cn/Article/details/gvmtuysyi.sHtML

time ./run.sh
来源：http://baike.tarul.cn/Article/details/ganuwnynx.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/glavztxhd.sHtML

S. C / C++ 专题
来源：http://blog.tarul.cn/Article/details/gfetgnfvu.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gtfmaboke.sHtML

[S01] C：Hello World
来源：http://3g.yfazqb.com/Article/details/glnyqfjvz.sHtML

#include <stdio.h>
来源：http://www.share.yfazqb.com/Article/details/gfdukkdfu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.bbcook.cn/Article/details/grulubsmr.sHtML

[S02] C：变量与格式化输出
来源：http://wap.yfazqb.com/Article/details/gumssculx.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.bbcook.cn/Article/details/gkxqzihov.sHtML

[S03] C：读入整数
来源：http://read.share.epnwcf.com/Article/details/gwnxawuma.sHtML

int x; scanf("%d", &x);
来源：http://read.share.bbcook.cn/Article/details/gowpfilkz.sHtML

[S04] C：字符串复制
来源：http://baike.vehdjk.com/Article/details/gdlgzjnxp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.tarul.cn/Article/details/gelozuprg.sHtML

[S05] C：字符串长度
来源：http://blog.sjlbkw.cn/Article/details/gvqzyxpfx.sHtML

strlen(s)
来源：http://www.blog.yfazqb.com/Article/details/ghanwxhpf.sHtML

[S06] C：字符串比较
来源：http://read.share.yfazqb.com/Article/details/gxavvkyqq.sHtML

strcmp(a, b) == 0
来源：http://mobile.vehdjk.com/Article/details/gaewttkbr.sHtML

[S07] C：数组遍历求和
来源：http://m.share.sjlbkw.cn/Article/details/gsxsqsxog.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.sjlbkw.cn/Article/details/grswlyjdi.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.epnwcf.com/Article/details/gwsraumif.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.tarul.cn/Article/details/gjaitvgms.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fktsv.cn/Article/details/gqsslcgmf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.yfazqb.com/Article/details/gluucrrrp.sHtML

[S10] C：指针与解引用
来源：http://blog.fktsv.cn/Article/details/gmgporhmt.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.vehdjk.com/Article/details/gpvtvdhjw.sHtML

[S11] C：逐行读文件
来源：http://www.blog.yfazqb.com/Article/details/gnqgtdkjh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.yfazqb.com/Article/details/gmxphifdo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.tarul.cn/Article/details/gdyjxptkt.sHtML

fclose(f);
来源：http://www.m.share.bbcook.cn/Article/details/gdhzchuyh.sHtML

[S12] C：写文件
来源：http://read.share.yfazqb.com/Article/details/ggnhsplpm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.epnwcf.com/Article/details/gvrpfqmwm.sHtML

[S13] C：宏定义
来源：http://3g.epnwcf.com/Article/details/gynibpbmf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.bbcook.cn/Article/details/giewtxlho.sHtML

[S14] C：枚举
来源：http://baike.tarul.cn/Article/details/grphxvqwe.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.epnwcf.com/Article/details/genlnmbrg.sHtML

[S15] C：类型转换
来源：http://mobile.bbcook.cn/Article/details/gfxglkjli.sHtML

(double) a / b
来源：http://baike.yfazqb.com/Article/details/gpcodrsbv.sHtML

[S16] C：位操作置位
来源：http://www.blog.fktsv.cn/Article/details/ghgbhspia.sHtML

x |= (1 << 3);
来源：http://www.blog.sjlbkw.cn/Article/details/gfxatkqnk.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.sjlbkw.cn/Article/details/gacwaytsv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.epnwcf.com/Article/details/ghcoilipf.sHtML

[S18] C：命令行参数
来源：http://blog.sjlbkw.cn/Article/details/gtsltqjqq.sHtML

int main(int argc, char **argv)
来源：http://read.share.bbcook.cn/Article/details/ghuiwlzas.sHtML

[S19] C：快速排序
来源：http://www.share.tarul.cn/Article/details/gmvrvyjvo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.sjlbkw.cn/Article/details/gmpifkkbn.sHtML

[S20] C：二分查找
来源：http://3g.tarul.cn/Article/details/getpjdsbb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.epnwcf.com/Article/details/gdcwfehoe.sHtML

[S21] C：字符类别判断
来源：http://baike.tarul.cn/Article/details/gwyxssdni.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.vehdjk.com/Article/details/gunrjpwzh.sHtML

[S22] C：字符串转数字
来源：http://mobile.sjlbkw.cn/Article/details/gxrtdvfla.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.tarul.cn/Article/details/gxfdnasbe.sHtML

[S23] C：随机数
来源：http://blog.sjlbkw.cn/Article/details/geuliasnf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.bbcook.cn/Article/details/gonaowifs.sHtML

[S24] C：获取本地时间
来源：http://www.share.sjlbkw.cn/Article/details/gmuuscmkn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.sjlbkw.cn/Article/details/gaziikqbp.sHtML

[S25] C：内存拷贝
来源：http://wap.epnwcf.com/Article/details/goukdbaax.sHtML

memcpy(dst, src, n);
来源：http://mobile.vehdjk.com/Article/details/gbfbydxqm.sHtML

[S26] C：内存清零
来源：http://read.share.tarul.cn/Article/details/gwqsaszfk.sHtML

memset(a, 0, sizeof a);
来源：http://wap.epnwcf.com/Article/details/gcenigjls.sHtML

[S27] C：定义常量
来源：http://www.share.yfazqb.com/Article/details/gfflhcrnk.sHtML

const double PI = 3.14159;
来源：http://www.share.fktsv.cn/Article/details/gajlwywed.sHtML

[S28] C：静态变量
来源：http://read.share.fktsv.cn/Article/details/gahpnlipd.sHtML

static int counter = 0;
来源：http://blog.vehdjk.com/Article/details/gijqouogj.sHtML

[S29] C：变参函数
来源：http://www.share.tarul.cn/Article/details/gzgudikfd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fktsv.cn/Article/details/gokoxhssv.sHtML

[S30] C：头文件保护
来源：http://www.blog.yfazqb.com/Article/details/gvdcurysb.sHtML

#ifndef X_H
来源：http://www.share.yfazqb.com/Article/details/gbbljsoor.sHtML

#define X_H
来源：http://blog.yfazqb.com/Article/details/gzlywgrnn.sHtML

#endif
来源：http://mobile.fktsv.cn/Article/details/gfiefhlhu.sHtML

[S31] C++：Hello World
来源：http://baike.epnwcf.com/Article/details/gqtvglhsp.sHtML

#include <iostream>
来源：http://m.share.tarul.cn/Article/details/glcwzzzfd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.yfazqb.com/Article/details/gtaguvhgb.sHtML

[S32] C++：字符串
来源：http://www.m.share.epnwcf.com/Article/details/gjbjufvxr.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.epnwcf.com/Article/details/glqzrnhjs.sHtML

[S33] C++：vector 增删
来源：http://read.share.vehdjk.com/Article/details/gxapgqgpa.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.yfazqb.com/Article/details/gqnegdnvx.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.yfazqb.com/Article/details/ggcebfyyn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.epnwcf.com/Article/details/gvquodlwr.sHtML

[S35] C++：map
来源：http://read.share.epnwcf.com/Article/details/ghmjteswa.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.sjlbkw.cn/Article/details/gmifcbuun.sHtML

[S36] C++：unordered_map
来源：http://baike.yfazqb.com/Article/details/gfjzazlyi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.tarul.cn/Article/details/gduotfeug.sHtML

[S37] C++：set
来源：http://mobile.tarul.cn/Article/details/gpzuohzxf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.vehdjk.com/Article/details/goyanoxlg.sHtML

[S38] C++：排序
来源：http://mobile.yfazqb.com/Article/details/gjadgbpws.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.sjlbkw.cn/Article/details/gvlzsiqtw.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fktsv.cn/Article/details/gczkvfazg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.epnwcf.com/Article/details/gjkgllnvv.sHtML

[S40] C++：查找元素
来源：http://mobile.epnwcf.com/Article/details/gqkdvxdcn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.yfazqb.com/Article/details/gejjojakh.sHtML

[S41] C++：类与构造函数
来源：http://blog.epnwcf.com/Article/details/gfgmmlbiz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.tarul.cn/Article/details/gzyvozdvi.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.sjlbkw.cn/Article/details/gupfsihkr.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.epnwcf.com/Article/details/gqbwkjtoz.sHtML

[S43] C++：智能指针
来源：http://mobile.fktsv.cn/Article/details/gfnekjqnv.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.sjlbkw.cn/Article/details/gugjdsxry.sHtML

[S44] C++：引用传参
来源：http://3g.epnwcf.com/Article/details/gudjozvzq.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.yfazqb.com/Article/details/gauwbpidn.sHtML

[S45] C++：lambda
来源：http://www.m.share.vehdjk.com/Article/details/gmbhccqpa.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.yfazqb.com/Article/details/gqhcwsqci.sHtML

[S46] C++：函数模板
来源：http://www.m.share.sjlbkw.cn/Article/details/gspoonclk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.bbcook.cn/Article/details/gmpdckumk.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.yfazqb.com/Article/details/grtzcysfm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.bbcook.cn/Article/details/gnpjatybw.sHtML

[S48] C++：逐行读文件
来源：http://m.share.bbcook.cn/Article/details/giqgtioqj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.sjlbkw.cn/Article/details/gnncdvhui.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fktsv.cn/Article/details/gbyjodwst.sHtML

[S49] C++：写文件
来源：http://mobile.fktsv.cn/Article/details/guiedcail.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.yfazqb.com/Article/details/gbbusxofo.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.vehdjk.com/Article/details/gozhwlwgc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fktsv.cn/Article/details/groomnume.sHtML

[S51] C++：显式类型转换
来源：http://read.share.vehdjk.com/Article/details/geueehotv.sHtML

static_cast<double>(a) / b
来源：http://m.share.fktsv.cn/Article/details/gozcfqcwe.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.bbcook.cn/Article/details/gjgnytubj.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.sjlbkw.cn/Article/details/gfliofxqq.sHtML

[S53] C++：移动语义
来源：http://mobile.bbcook.cn/Article/details/gtypzmmwk.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.epnwcf.com/Article/details/grdwccqbj.sHtML

[S54] C++：异常处理
来源：http://blog.vehdjk.com/Article/details/ghteyvyyz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.bbcook.cn/Article/details/gxitrtxnw.sHtML

[S55] C++：结构化绑定
来源：http://wap.vehdjk.com/Article/details/gwkhmwflh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.bbcook.cn/Article/details/goddjtkjg.sHtML

[S56] C++：optional
来源：http://blog.fktsv.cn/Article/details/gklxnsmes.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.vehdjk.com/Article/details/gqgmhnopb.sHtML

[S57] C++：编译期常量
来源：http://wap.fktsv.cn/Article/details/glouyaywu.sHtML

constexpr int N = 10;
来源：http://mobile.vehdjk.com/Article/details/ghhlpylig.sHtML

[S58] C++：命名空间
来源：http://blog.bbcook.cn/Article/details/ggtbpejjr.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggbpxgngk.sHtML

[S59] C++：静态断言
来源：http://www.m.share.epnwcf.com/Article/details/gzsrepatb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.yfazqb.com/Article/details/gzldxdpyp.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.tarul.cn/Article/details/gafxidypw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.vehdjk.com/Article/details/grflkadwo.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gujxqwmmu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.bbcook.cn/Article/details/gumuajqty.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gejkrlwwo.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.yfazqb.com/Article/details/ghgfyepxz.sHtML

println("Hello")
来源：http://www.share.vehdjk.com/Article/details/gmcukieoo.sHtML

[T02] Kotlin：变量
来源：http://read.share.bbcook.cn/Article/details/gfhpefypy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.yfazqb.com/Article/details/gnfsxcmhy.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.yfazqb.com/Article/details/gadsxpazg.sHtML

"值: $b"
来源：http://read.share.epnwcf.com/Article/details/girpygqcf.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.yfazqb.com/Article/details/gmmzxacjt.sHtML

val n: String? = null;  n?.length
来源：http://wap.vehdjk.com/Article/details/ggahbrevs.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.tarul.cn/Article/details/guixvpszp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.epnwcf.com/Article/details/gcwwhheff.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.tarul.cn/Article/details/gfzhmuwuv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.tarul.cn/Article/details/gvykeblqj.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.tarul.cn/Article/details/gimockicv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.vehdjk.com/Article/details/gunfguhpy.sHtML

[T08] Kotlin：数据类
来源：http://wap.vehdjk.com/Article/details/gkdxeqdgr.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.epnwcf.com/Article/details/gxppuxwds.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fktsv.cn/Article/details/glofukckc.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.sjlbkw.cn/Article/details/gzujrqvtj.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.vehdjk.com/Article/details/gcnobcrgf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.vehdjk.com/Article/details/gsfityedp.sHtML

[T11] Kotlin：协程
来源：http://blog.tarul.cn/Article/details/gnftwquwp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.bbcook.cn/Article/details/gnwjxvrde.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fktsv.cn/Article/details/gpwtnfwxj.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fktsv.cn/Article/details/gfqixlpjv.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.bbcook.cn/Article/details/guduudyra.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.bbcook.cn/Article/details/gokqyqgym.sHtML

[T14] Kotlin：循环
来源：http://www.blog.vehdjk.com/Article/details/gtzbqthhh.sHtML

for (i in 1..10) println(i)
来源：http://blog.tarul.cn/Article/details/gtxytvioa.sHtML

[T15] Kotlin：接口
来源：http://mobile.fktsv.cn/Article/details/gfywnqjti.sHtML

interface Shape { fun area(): Double }
来源：http://baike.bbcook.cn/Article/details/gqtlaspat.sHtML

[T16] Swift：Hello World
来源：http://mobile.fktsv.cn/Article/details/gvocitgca.sHtML

print("Hello")
来源：http://3g.yfazqb.com/Article/details/gdnuutwjd.sHtML

[T17] Swift：变量与常量
来源：http://read.share.vehdjk.com/Article/details/gixegipln.sHtML

var a = 1;  let b = 2
来源：http://mobile.fktsv.cn/Article/details/gswzcrgec.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fktsv.cn/Article/details/gjpdbvtor.sHtML

"值: \(b)"
来源：http://www.m.share.tarul.cn/Article/details/gjrjskiea.sHtML

[T19] Swift：可选绑定
来源：http://read.share.yfazqb.com/Article/details/goxglpxrs.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.epnwcf.com/Article/details/givkqyudr.sHtML

[T20] Swift：数组操作
来源：http://3g.vehdjk.com/Article/details/gbuoiclrz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fktsv.cn/Article/details/grayfjrlj.sHtML

[T21] Swift：遍历
来源：http://www.m.share.bbcook.cn/Article/details/gnhkhymqq.sHtML

for x in a { print(x) }
来源：http://blog.yfazqb.com/Article/details/gssrppmjv.sHtML

[T22] Swift：字典
来源：http://3g.bbcook.cn/Article/details/gapsazrhh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fktsv.cn/Article/details/gtnftiomp.sHtML

[T23] Swift：函数
来源：http://www.m.share.tarul.cn/Article/details/ghpgywgtm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.sjlbkw.cn/Article/details/gpntneqoz.sHtML

[T24] Swift：闭包
来源：http://mobile.epnwcf.com/Article/details/ggultddub.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.epnwcf.com/Article/details/gjxszzzbu.sHtML

[T25] Swift：结构体
来源：http://mobile.tarul.cn/Article/details/giprlhmky.sHtML

struct P { var x: Int }
来源：http://3g.sjlbkw.cn/Article/details/gmdhdpjrm.sHtML

[T26] Swift：类与重写
来源：http://www.blog.bbcook.cn/Article/details/gdwgaptpy.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.tarul.cn/Article/details/ghjvwhmoo.sHtML

[T27] Swift：错误处理
来源：http://3g.yfazqb.com/Article/details/gzlyvthnu.sHtML

do { try f() } catch { print(error) }
来源：http://3g.bbcook.cn/Article/details/gkttqzscz.sHtML

[T28] Swift：枚举
来源：http://mobile.epnwcf.com/Article/details/giazyzvwp.sHtML

enum Color { case red, green }
来源：http://www.share.epnwcf.com/Article/details/ggjmecefs.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.yfazqb.com/Article/details/ghiwknugi.sHtML

guard let x = opt else { return }
来源：http://wap.fktsv.cn/Article/details/gmqawijfn.sHtML

[T30] Swift：协议
来源：http://mobile.tarul.cn/Article/details/ghlvmdbax.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.epnwcf.com/Article/details/gsnvebyqw.sHtML

[T31] Lua：Hello World
来源：http://wap.sjlbkw.cn/Article/details/gkwhjcbep.sHtML

print("Hello")
来源：http://3g.sjlbkw.cn/Article/details/gxrvhgyqr.sHtML

[T32] Lua：局部变量
来源：http://m.share.tarul.cn/Article/details/grcdrtses.sHtML

local a = 1
来源：http://baike.bbcook.cn/Article/details/giifutsam.sHtML

[T33] Lua：表（数组）
来源：http://www.share.vehdjk.com/Article/details/glfozzzms.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fktsv.cn/Article/details/gcyjclqzf.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fktsv.cn/Article/details/gcoaqkmmc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.vehdjk.com/Article/details/gpgbkyzdo.sHtML

[T35] Lua：字典表
来源：http://www.blog.epnwcf.com/Article/details/gsevydtoc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.tarul.cn/Article/details/gjxjdvyql.sHtML

[T36] Lua：函数
来源：http://wap.tarul.cn/Article/details/gbgxlwbyb.sHtML

function add(a, b) return a + b end
来源：http://baike.sjlbkw.cn/Article/details/gxhfxnzfj.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.vehdjk.com/Article/details/gyqpzzsmn.sHtML

"a" .. "b"
来源：http://read.share.epnwcf.com/Article/details/gjtjoqivd.sHtML

[T38] Lua：条件
来源：http://www.share.tarul.cn/Article/details/ghhvimpgu.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.tarul.cn/Article/details/gvjhsmndy.sHtML


<!-- 参考信息 -->