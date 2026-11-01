代发 wailian999

find . -name "*.tmp" -delete
来源：http://read.share.bbcook.cn/Article/details/gdpwrmwem.sHtML

[R46] 递归替换文件内容
来源：http://read.share.epnwcf.com/Article/details/gsuofgxrw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.tarul.cn/Article/details/gzpdfqjox.sHtML

[R47] sed 单行替换
来源：http://wap.tarul.cn/Article/details/gitojxroh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.epnwcf.com/Article/details/gakyjhvmi.sHtML

[R48] awk 取指定列
来源：http://read.share.tarul.cn/Article/details/gfqtquepi.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fktsv.cn/Article/details/gzycqjifa.sHtML

[R49] awk 带条件
来源：http://mobile.sjlbkw.cn/Article/details/geydeuake.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.sjlbkw.cn/Article/details/gevyyldzo.sHtML

[R50] awk 求和
来源：http://baike.tarul.cn/Article/details/gpfowcbvv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.yfazqb.com/Article/details/grdnfenva.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fktsv.cn/Article/details/gwvzaucsk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fktsv.cn/Article/details/gkgzwcrdo.sHtML

[R52] 统计行数
来源：http://read.share.sjlbkw.cn/Article/details/gnigxuslp.sHtML

wc -l a.txt
来源：http://wap.yfazqb.com/Article/details/giwrobsne.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fktsv.cn/Article/details/gcijpnbkg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.bbcook.cn/Article/details/gfyvwkkph.sHtML

[R54] 比较两个文件
来源：http://baike.tarul.cn/Article/details/gzcsyulen.sHtML

diff a.txt b.txt
来源：http://baike.tarul.cn/Article/details/gyzlkgchw.sHtML

[R55] 压缩与解压
来源：http://m.share.yfazqb.com/Article/details/gjtluafod.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.tarul.cn/Article/details/gxdgcgmgq.sHtML

[R56] 远程拷贝
来源：http://www.m.share.sjlbkw.cn/Article/details/gyqjalkmo.sHtML

scp file user@host:/path/
来源：http://www.share.vehdjk.com/Article/details/gbqceberh.sHtML

[R57] 远程执行命令
来源：http://www.blog.epnwcf.com/Article/details/gmhvxjztl.sHtML

ssh user@host 'uptime'
来源：http://3g.bbcook.cn/Article/details/gyvgjprnw.sHtML

[R58] 下载文件
来源：http://www.m.share.epnwcf.com/Article/details/gbafyoidf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.yfazqb.com/Article/details/gzqhoqves.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fktsv.cn/Article/details/garovatdt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.epnwcf.com/Article/details/gblqleykn.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.epnwcf.com/Article/details/ghymvptmk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.tarul.cn/Article/details/gtwvieoco.sHtML

[R61] 磁盘占用
来源：http://blog.bbcook.cn/Article/details/geewoyvem.sHtML

df -h;  du -sh *
来源：http://m.share.tarul.cn/Article/details/gydzsxbyd.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fktsv.cn/Article/details/ghmadumxh.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.epnwcf.com/Article/details/gkwkqyygw.sHtML

[R63] 内存与进程
来源：http://3g.epnwcf.com/Article/details/grlbkkzab.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.bbcook.cn/Article/details/gzoumfmvi.sHtML

[R64] 结束进程
来源：http://www.blog.vehdjk.com/Article/details/gjpzxgbzo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.tarul.cn/Article/details/gekdqivdz.sHtML

[R65] 查看端口占用
来源：http://www.m.share.bbcook.cn/Article/details/gciuxdciz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.bbcook.cn/Article/details/gsctcnway.sHtML

[R66] 定时任务
来源：http://3g.yfazqb.com/Article/details/glczxmjvl.sHtML

crontab -e;  crontab -l
来源：http://3g.epnwcf.com/Article/details/glctkmvyp.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.bbcook.cn/Article/details/gnodwpkbf.sHtML

openssl rand -hex 16
来源：http://www.blog.epnwcf.com/Article/details/giwzshaqa.sHtML

[R68] 计算文件校验值
来源：http://www.blog.yfazqb.com/Article/details/gjyqqqkud.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.bbcook.cn/Article/details/giwpxeimc.sHtML

[R69] 生成随机密码
来源：http://blog.sjlbkw.cn/Article/details/gneheetdq.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.tarul.cn/Article/details/gqjbpqqux.sHtML

[R70] 时间戳与互转
来源：http://wap.sjlbkw.cn/Article/details/gvfibnufj.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.bbcook.cn/Article/details/gvgcilbtg.sHtML

[R71] 日期格式化
来源：http://mobile.fktsv.cn/Article/details/gwrhxrbfo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.epnwcf.com/Article/details/gvpcjueoh.sHtML

[R72] 等待端口就绪
来源：http://baike.yfazqb.com/Article/details/gnxhbgrau.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fktsv.cn/Article/details/gjuvxftrs.sHtML

[R73] 分割大日志
来源：http://www.m.share.sjlbkw.cn/Article/details/gzwuavhba.sHtML

split -l 1000 big.log part_
来源：http://mobile.vehdjk.com/Article/details/gqsaspror.sHtML

[R74] 批量重命名
来源：http://3g.bbcook.cn/Article/details/gsrvqvyms.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.yfazqb.com/Article/details/gqkqfbedr.sHtML

[R75] 导出环境变量
来源：http://baike.fktsv.cn/Article/details/guiuraarm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.tarul.cn/Article/details/gehzfkilj.sHtML

[R76] 使用临时文件
来源：http://baike.yfazqb.com/Article/details/gtzbxdpug.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.yfazqb.com/Article/details/gxsbeszzm.sHtML

[R77] 读取用户输入
来源：http://wap.epnwcf.com/Article/details/gfqeugxqq.sHtML

read -rp "请输入: " ans
来源：http://baike.tarul.cn/Article/details/gnnrsyrzg.sHtML

[R78] 交互式菜单
来源：http://mobile.tarul.cn/Article/details/gvskxksqr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.epnwcf.com/Article/details/gxshpneeo.sHtML

[R79] 解析命令行选项
来源：http://baike.sjlbkw.cn/Article/details/gvuodngsc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.vehdjk.com/Article/details/ghijhbwxv.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.epnwcf.com/Article/details/gtflfzdzq.sHtML

time ./run.sh
来源：http://mobile.epnwcf.com/Article/details/gwsrhdvyv.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/grntqsklu.sHtML

S. C / C++ 专题
来源：http://3g.fktsv.cn/Article/details/gotxztaeu.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gagbesjrz.sHtML

[S01] C：Hello World
来源：http://3g.bbcook.cn/Article/details/grwhaalvh.sHtML

#include <stdio.h>
来源：http://www.blog.yfazqb.com/Article/details/ghcdmeiix.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fktsv.cn/Article/details/ggtjmbavu.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.epnwcf.com/Article/details/ghdbnjajq.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.epnwcf.com/Article/details/gurvfengm.sHtML

[S03] C：读入整数
来源：http://www.m.share.tarul.cn/Article/details/gjdkttyfw.sHtML

int x; scanf("%d", &x);
来源：http://read.share.yfazqb.com/Article/details/gcvvbmbco.sHtML

[S04] C：字符串复制
来源：http://wap.bbcook.cn/Article/details/gswrpqthm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.epnwcf.com/Article/details/gioklxfuf.sHtML

[S05] C：字符串长度
来源：http://baike.bbcook.cn/Article/details/geucbiwjj.sHtML

strlen(s)
来源：http://read.share.yfazqb.com/Article/details/gqnspweuj.sHtML

[S06] C：字符串比较
来源：http://wap.bbcook.cn/Article/details/gafpzluni.sHtML

strcmp(a, b) == 0
来源：http://read.share.fktsv.cn/Article/details/gsfnoyybf.sHtML

[S07] C：数组遍历求和
来源：http://m.share.vehdjk.com/Article/details/gislypvmy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fktsv.cn/Article/details/ghimesfjg.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.bbcook.cn/Article/details/ggwbejijf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.tarul.cn/Article/details/gbapohrxq.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.sjlbkw.cn/Article/details/gfmhnapgt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.tarul.cn/Article/details/guyxyvazo.sHtML

[S10] C：指针与解引用
来源：http://baike.epnwcf.com/Article/details/gmwphbhge.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.yfazqb.com/Article/details/gqztvdksj.sHtML

[S11] C：逐行读文件
来源：http://mobile.bbcook.cn/Article/details/gbnoydnmh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fktsv.cn/Article/details/gzbkhlnkh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.tarul.cn/Article/details/gykgtspmf.sHtML

fclose(f);
来源：http://wap.fktsv.cn/Article/details/gtvixmsyr.sHtML

[S12] C：写文件
来源：http://www.share.vehdjk.com/Article/details/gyupvkdyx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.tarul.cn/Article/details/gyopxousa.sHtML

[S13] C：宏定义
来源：http://www.blog.epnwcf.com/Article/details/gayfykneb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.yfazqb.com/Article/details/gdejlantv.sHtML

[S14] C：枚举
来源：http://blog.sjlbkw.cn/Article/details/ghyjrlzdi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.tarul.cn/Article/details/gxpdxelzu.sHtML

[S15] C：类型转换
来源：http://www.blog.fktsv.cn/Article/details/gruaxlfaq.sHtML

(double) a / b
来源：http://baike.sjlbkw.cn/Article/details/gpannxwtc.sHtML

[S16] C：位操作置位
来源：http://blog.yfazqb.com/Article/details/gsyavswvb.sHtML

x |= (1 << 3);
来源：http://3g.epnwcf.com/Article/details/gkszvyyun.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.tarul.cn/Article/details/gcjwbovab.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.bbcook.cn/Article/details/gpwjhkloq.sHtML

[S18] C：命令行参数
来源：http://m.share.tarul.cn/Article/details/gojsktolz.sHtML

int main(int argc, char **argv)
来源：http://www.share.bbcook.cn/Article/details/gthxzemmg.sHtML

[S19] C：快速排序
来源：http://www.blog.sjlbkw.cn/Article/details/ggufrdxys.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.sjlbkw.cn/Article/details/gysgcfaip.sHtML

[S20] C：二分查找
来源：http://read.share.vehdjk.com/Article/details/gtbxwssaz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fktsv.cn/Article/details/gfnqyruju.sHtML

[S21] C：字符类别判断
来源：http://www.share.yfazqb.com/Article/details/guresmmsl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fktsv.cn/Article/details/gglqprngq.sHtML

[S22] C：字符串转数字
来源：http://mobile.vehdjk.com/Article/details/gvnwfhdnu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.vehdjk.com/Article/details/ggxdmlndo.sHtML

[S23] C：随机数
来源：http://www.m.share.bbcook.cn/Article/details/gjrckkmtt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.epnwcf.com/Article/details/geoxjulcm.sHtML

[S24] C：获取本地时间
来源：http://read.share.tarul.cn/Article/details/grfjdhzdg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.yfazqb.com/Article/details/grjptsdau.sHtML

[S25] C：内存拷贝
来源：http://m.share.yfazqb.com/Article/details/gvhiygwsg.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.vehdjk.com/Article/details/gvldqdttu.sHtML

[S26] C：内存清零
来源：http://m.share.tarul.cn/Article/details/ggszzgmeh.sHtML

memset(a, 0, sizeof a);
来源：http://baike.sjlbkw.cn/Article/details/getkphxbm.sHtML

[S27] C：定义常量
来源：http://www.blog.fktsv.cn/Article/details/gqbvowddl.sHtML

const double PI = 3.14159;
来源：http://blog.sjlbkw.cn/Article/details/gihojcbfl.sHtML

[S28] C：静态变量
来源：http://3g.bbcook.cn/Article/details/guklcfvkc.sHtML

static int counter = 0;
来源：http://3g.sjlbkw.cn/Article/details/gqkytatsi.sHtML

[S29] C：变参函数
来源：http://wap.sjlbkw.cn/Article/details/gxpoegypn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.yfazqb.com/Article/details/garycwols.sHtML

[S30] C：头文件保护
来源：http://wap.fktsv.cn/Article/details/gfoypawmh.sHtML

#ifndef X_H
来源：http://blog.tarul.cn/Article/details/gsypxnxoc.sHtML

#define X_H
来源：http://www.blog.vehdjk.com/Article/details/gdjrswsov.sHtML

#endif
来源：http://m.share.fktsv.cn/Article/details/ggzlkmwks.sHtML

[S31] C++：Hello World
来源：http://blog.epnwcf.com/Article/details/gogqlgvfm.sHtML

#include <iostream>
来源：http://read.share.fktsv.cn/Article/details/gozxvhpqb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fktsv.cn/Article/details/giyzimfud.sHtML

[S32] C++：字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gcadwwure.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.tarul.cn/Article/details/gfggbydke.sHtML

[S33] C++：vector 增删
来源：http://www.blog.sjlbkw.cn/Article/details/gttckudan.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.sjlbkw.cn/Article/details/ghhmxoabd.sHtML

[S34] C++：遍历 vector
来源：http://www.share.yfazqb.com/Article/details/gtystmdek.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.sjlbkw.cn/Article/details/gfulsnvea.sHtML

[S35] C++：map
来源：http://3g.fktsv.cn/Article/details/gtzmxhkgz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.tarul.cn/Article/details/gsgwmvybz.sHtML

[S36] C++：unordered_map
来源：http://blog.bbcook.cn/Article/details/gysbqvijd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.epnwcf.com/Article/details/gzdleuxym.sHtML

[S37] C++：set
来源：http://www.share.fktsv.cn/Article/details/grlwjvhlu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.bbcook.cn/Article/details/gzqqxivat.sHtML

[S38] C++：排序
来源：http://wap.tarul.cn/Article/details/gurelbykt.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.epnwcf.com/Article/details/goguttvgp.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.tarul.cn/Article/details/gsgmjtufd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.vehdjk.com/Article/details/gkootwnhm.sHtML

[S40] C++：查找元素
来源：http://m.share.sjlbkw.cn/Article/details/gvwunesbk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.sjlbkw.cn/Article/details/gjbygofqe.sHtML

[S41] C++：类与构造函数
来源：http://blog.yfazqb.com/Article/details/gnrsaxejn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.bbcook.cn/Article/details/gqfdkzrsg.sHtML

[S42] C++：继承与虚函数
来源：http://baike.tarul.cn/Article/details/gqzecftwp.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.yfazqb.com/Article/details/gbirnodxe.sHtML

[S43] C++：智能指针
来源：http://blog.vehdjk.com/Article/details/ghjubpujo.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.bbcook.cn/Article/details/gcuqeybdt.sHtML

[S44] C++：引用传参
来源：http://blog.bbcook.cn/Article/details/gtzuzylrg.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fktsv.cn/Article/details/gizjstxkc.sHtML

[S45] C++：lambda
来源：http://www.m.share.vehdjk.com/Article/details/gcqwcnpmp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fktsv.cn/Article/details/gdbbqukqk.sHtML

[S46] C++：函数模板
来源：http://mobile.vehdjk.com/Article/details/gphiaygdw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.epnwcf.com/Article/details/gimwumaaq.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.yfazqb.com/Article/details/gpucyuvbc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.epnwcf.com/Article/details/gyrovvwof.sHtML

[S48] C++：逐行读文件
来源：http://m.share.sjlbkw.cn/Article/details/gtzylmylf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.yfazqb.com/Article/details/gxozgjahs.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.vehdjk.com/Article/details/gevlifban.sHtML

[S49] C++：写文件
来源：http://www.m.share.fktsv.cn/Article/details/gryfushha.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.vehdjk.com/Article/details/gftsnqcgc.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.epnwcf.com/Article/details/gflgdxjkz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.bbcook.cn/Article/details/gicbmkauk.sHtML

[S51] C++：显式类型转换
来源：http://www.share.bbcook.cn/Article/details/gzoisqban.sHtML

static_cast<double>(a) / b
来源：http://baike.fktsv.cn/Article/details/ghdasojve.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fktsv.cn/Article/details/gtigrnwmt.sHtML

int size() const noexcept { return n_; }
来源：http://baike.vehdjk.com/Article/details/gcffbuaam.sHtML

[S53] C++：移动语义
来源：http://mobile.tarul.cn/Article/details/gvmrxwmly.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.bbcook.cn/Article/details/gyqziqgyc.sHtML

[S54] C++：异常处理
来源：http://wap.yfazqb.com/Article/details/gyotmsujl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.bbcook.cn/Article/details/gfmiryrml.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fktsv.cn/Article/details/gqhtqwxki.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.vehdjk.com/Article/details/gmrfootgs.sHtML

[S56] C++：optional
来源：http://3g.tarul.cn/Article/details/gqiwbcmzp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.yfazqb.com/Article/details/gyilxycal.sHtML

[S57] C++：编译期常量
来源：http://m.share.sjlbkw.cn/Article/details/gufspovco.sHtML

constexpr int N = 10;
来源：http://www.blog.tarul.cn/Article/details/gasjzppws.sHtML

[S58] C++：命名空间
来源：http://wap.vehdjk.com/Article/details/gqprpwzhn.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.epnwcf.com/Article/details/gllgtjyjs.sHtML

[S59] C++：静态断言
来源：http://3g.tarul.cn/Article/details/gyxewljnd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fktsv.cn/Article/details/gvbnuxzeh.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.vehdjk.com/Article/details/gsqiewsih.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.epnwcf.com/Article/details/gkpijanvx.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gubisqhsx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.vehdjk.com/Article/details/gjgwcsjdo.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/goacftnkh.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.tarul.cn/Article/details/gliklcpmr.sHtML

println("Hello")
来源：http://www.blog.bbcook.cn/Article/details/grzkemrcu.sHtML

[T02] Kotlin：变量
来源：http://baike.epnwcf.com/Article/details/ggdepczhs.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.tarul.cn/Article/details/ggeddkjqa.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.vehdjk.com/Article/details/gcpdzxrbu.sHtML

"值: $b"
来源：http://blog.epnwcf.com/Article/details/giekuhwja.sHtML

[T04] Kotlin：空安全
来源：http://wap.epnwcf.com/Article/details/gnvtoclzm.sHtML

val n: String? = null;  n?.length
来源：http://3g.vehdjk.com/Article/details/gfurghgmk.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.sjlbkw.cn/Article/details/ggsjqukca.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.bbcook.cn/Article/details/gugldedgl.sHtML

[T06] Kotlin：集合映射
来源：http://3g.vehdjk.com/Article/details/ggjvwwjfi.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fktsv.cn/Article/details/gnmhbzasp.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.vehdjk.com/Article/details/gsyyesdur.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.bbcook.cn/Article/details/gndcjphal.sHtML

[T08] Kotlin：数据类
来源：http://wap.tarul.cn/Article/details/gorvgxymo.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.bbcook.cn/Article/details/gmllkbnpx.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.vehdjk.com/Article/details/gpuwfnecp.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.tarul.cn/Article/details/gawzuydlz.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fktsv.cn/Article/details/gfgniykrg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.epnwcf.com/Article/details/gvkozvuyg.sHtML

[T11] Kotlin：协程
来源：http://blog.yfazqb.com/Article/details/gbwvovpwb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fktsv.cn/Article/details/gryjabdpo.sHtML

[T12] Kotlin：解构声明
来源：http://3g.tarul.cn/Article/details/gobqtebxp.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.tarul.cn/Article/details/gdclcaqvf.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.yfazqb.com/Article/details/ghpmkqfzu.sHtML

val m = mapOf("a" to 1)
来源：http://wap.epnwcf.com/Article/details/gatatdrvx.sHtML

[T14] Kotlin：循环
来源：http://www.blog.tarul.cn/Article/details/gbeyotokz.sHtML

for (i in 1..10) println(i)
来源：http://3g.fktsv.cn/Article/details/gniqsihcg.sHtML

[T15] Kotlin：接口
来源：http://m.share.vehdjk.com/Article/details/gyfnkzhma.sHtML

interface Shape { fun area(): Double }
来源：http://wap.vehdjk.com/Article/details/gwvonbvrk.sHtML

[T16] Swift：Hello World
来源：http://www.share.epnwcf.com/Article/details/gxreqelmm.sHtML

print("Hello")
来源：http://read.share.sjlbkw.cn/Article/details/gzdpdrycb.sHtML

[T17] Swift：变量与常量
来源：http://baike.fktsv.cn/Article/details/gtpcfejip.sHtML

var a = 1;  let b = 2
来源：http://wap.yfazqb.com/Article/details/gsqcrlphp.sHtML

[T18] Swift：字符串插值
来源：http://m.share.bbcook.cn/Article/details/glulxztss.sHtML

"值: \(b)"
来源：http://m.share.tarul.cn/Article/details/gvxmbeikk.sHtML

[T19] Swift：可选绑定
来源：http://wap.vehdjk.com/Article/details/ggjwxhleb.sHtML

if let n = opt { print(n) }
来源：http://www.blog.tarul.cn/Article/details/gjmxaoxyt.sHtML

[T20] Swift：数组操作
来源：http://read.share.bbcook.cn/Article/details/guxejmmdo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.vehdjk.com/Article/details/gbzqejnit.sHtML

[T21] Swift：遍历
来源：http://m.share.sjlbkw.cn/Article/details/gozjcvijg.sHtML

for x in a { print(x) }
来源：http://blog.tarul.cn/Article/details/gevwjbndw.sHtML

[T22] Swift：字典
来源：http://mobile.bbcook.cn/Article/details/gxsqcdagi.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fktsv.cn/Article/details/gnybgjesz.sHtML

[T23] Swift：函数
来源：http://www.share.tarul.cn/Article/details/gxmhuqqpt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.sjlbkw.cn/Article/details/gtozhxgjl.sHtML

[T24] Swift：闭包
来源：http://www.blog.fktsv.cn/Article/details/ggaxreejn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.vehdjk.com/Article/details/gzqozukyz.sHtML

[T25] Swift：结构体
来源：http://3g.bbcook.cn/Article/details/gdlhfimim.sHtML

struct P { var x: Int }
来源：http://baike.vehdjk.com/Article/details/gofclpckw.sHtML

[T26] Swift：类与重写
来源：http://www.share.bbcook.cn/Article/details/gajbgsjjn.sHtML

class A: Base { override func f() {} }
来源：http://www.share.vehdjk.com/Article/details/gnyfnxlrx.sHtML

[T27] Swift：错误处理
来源：http://3g.yfazqb.com/Article/details/gxsisezkj.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.vehdjk.com/Article/details/glzcfiykg.sHtML

[T28] Swift：枚举
来源：http://3g.fktsv.cn/Article/details/ghjpbomsu.sHtML

enum Color { case red, green }
来源：http://m.share.epnwcf.com/Article/details/ghtyxvemm.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.yfazqb.com/Article/details/gygccusdz.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fktsv.cn/Article/details/gvswyqbbg.sHtML

[T30] Swift：协议
来源：http://mobile.vehdjk.com/Article/details/gwzgiuole.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.bbcook.cn/Article/details/gpeuhtgpl.sHtML

[T31] Lua：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gdekqfqeb.sHtML

print("Hello")
来源：http://m.share.vehdjk.com/Article/details/gsndsoozx.sHtML

[T32] Lua：局部变量
来源：http://3g.fktsv.cn/Article/details/gxnrewndo.sHtML

local a = 1
来源：http://wap.yfazqb.com/Article/details/gutjspqqy.sHtML

[T33] Lua：表（数组）
来源：http://blog.tarul.cn/Article/details/gkvifxkrz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.sjlbkw.cn/Article/details/gytbdqmda.sHtML

[T34] Lua：遍历表
来源：http://3g.sjlbkw.cn/Article/details/gmmcclcgt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.bbcook.cn/Article/details/gvhjlfthy.sHtML

[T35] Lua：字典表
来源：http://mobile.tarul.cn/Article/details/gbhttvuzm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.epnwcf.com/Article/details/giddkpxml.sHtML

[T36] Lua：函数
来源：http://m.share.tarul.cn/Article/details/gtcrcmpko.sHtML

function add(a, b) return a + b end
来源：http://www.blog.epnwcf.com/Article/details/guedcsuet.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fktsv.cn/Article/details/getrpinqy.sHtML

"a" .. "b"
来源：http://m.share.tarul.cn/Article/details/gudwwrkso.sHtML

[T38] Lua：条件
来源：http://www.share.fktsv.cn/Article/details/gqvwilqph.sHtML

if x > 0 then print("正") end
来源：http://wap.yfazqb.com/Article/details/gzwcdpcei.sHtML

[T39] Lua：模式匹配
来源：http://blog.sjlbkw.cn/Article/details/glolpfycn.sHtML

string.find(s, "%d+")
来源：http://mobile.tarul.cn/Article/details/grufmtvbf.sHtML

[T40] Lua：元表
来源：http://blog.fktsv.cn/Article/details/gotdahodq.sHtML

setmetatable({}, { __index = base })
来源：http://wap.vehdjk.com/Article/details/gvoadjako.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/gdvmbwdmn.sHtML

print "Hello\n";
来源：http://www.m.share.bbcook.cn/Article/details/gvmfivxrh.sHtML

[T42] Perl：变量类型
来源：http://read.share.tarul.cn/Article/details/gfrjctlve.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fktsv.cn/Article/details/gfkegwyca.sHtML

[T43] Perl：字符串插值
来源：http://baike.bbcook.cn/Article/details/gilshiyvx.sHtML

"值: $a"
来源：http://www.m.share.yfazqb.com/Article/details/gruwvfuvm.sHtML

[T44] Perl：条件
来源：http://m.share.yfazqb.com/Article/details/gnwashgqp.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.epnwcf.com/Article/details/gavhhhvlf.sHtML

[T45] Perl：数组遍历
来源：http://3g.sjlbkw.cn/Article/details/gtuiuinqp.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.vehdjk.com/Article/details/gsngtkfsi.sHtML

[T46] Perl：哈希操作
来源：http://blog.yfazqb.com/Article/details/gbqeykpxc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fktsv.cn/Article/details/grgtshmhe.sHtML

[T47] Perl：正则捕获
来源：http://m.share.bbcook.cn/Article/details/gldkgcbjm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.sjlbkw.cn/Article/details/gbrmmlkyp.sHtML

[T48] Perl：正则替换
来源：http://3g.tarul.cn/Article/details/gglkayygs.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fktsv.cn/Article/details/gebontlir.sHtML


<!-- 参考信息 -->