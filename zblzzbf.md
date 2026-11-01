代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://3g.vehdjk.com/Article/details/gulzuzzsh.sHtML

[R48] awk 取指定列
来源：http://www.share.vehdjk.com/Article/details/ggsldrksc.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.yfazqb.com/Article/details/gsnyuepap.sHtML

[R49] awk 带条件
来源：http://www.blog.bbcook.cn/Article/details/gmejrnrmw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.yfazqb.com/Article/details/gjjuliard.sHtML

[R50] awk 求和
来源：http://m.share.yfazqb.com/Article/details/gimqwpfeq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fktsv.cn/Article/details/gpnirlifx.sHtML

[R51] 排序去重取前几
来源：http://www.blog.vehdjk.com/Article/details/gzdoujkwt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.yfazqb.com/Article/details/glswdwawb.sHtML

[R52] 统计行数
来源：http://www.blog.tarul.cn/Article/details/gjtjczubz.sHtML

wc -l a.txt
来源：http://www.blog.yfazqb.com/Article/details/gheojytha.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fktsv.cn/Article/details/goxwkdzot.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.bbcook.cn/Article/details/grprxarqp.sHtML

[R54] 比较两个文件
来源：http://www.share.bbcook.cn/Article/details/guzwqcrlj.sHtML

diff a.txt b.txt
来源：http://3g.bbcook.cn/Article/details/ggglpxtdy.sHtML

[R55] 压缩与解压
来源：http://mobile.fktsv.cn/Article/details/gpuaulaud.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.tarul.cn/Article/details/grnuldrhr.sHtML

[R56] 远程拷贝
来源：http://m.share.vehdjk.com/Article/details/grrlvzqma.sHtML

scp file user@host:/path/
来源：http://m.share.bbcook.cn/Article/details/gdiermlzr.sHtML

[R57] 远程执行命令
来源：http://www.blog.tarul.cn/Article/details/gblzzabhn.sHtML

ssh user@host 'uptime'
来源：http://read.share.sjlbkw.cn/Article/details/gulbvkyud.sHtML

[R58] 下载文件
来源：http://wap.tarul.cn/Article/details/gtbniazro.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.tarul.cn/Article/details/gkxdbgepu.sHtML

[R59] 发 POST JSON
来源：http://www.blog.sjlbkw.cn/Article/details/gygnlwbsd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.tarul.cn/Article/details/gpkrybydl.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.bbcook.cn/Article/details/glivakqhu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.bbcook.cn/Article/details/gagfcjsmu.sHtML

[R61] 磁盘占用
来源：http://baike.bbcook.cn/Article/details/grkuwahit.sHtML

df -h;  du -sh *
来源：http://3g.yfazqb.com/Article/details/gduhydseq.sHtML

[R62] 找最占空间的文件
来源：http://wap.sjlbkw.cn/Article/details/gwylcjxst.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.yfazqb.com/Article/details/giygqqyzv.sHtML

[R63] 内存与进程
来源：http://wap.tarul.cn/Article/details/gyxunkloc.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.epnwcf.com/Article/details/gmznosylj.sHtML

[R64] 结束进程
来源：http://mobile.sjlbkw.cn/Article/details/gljtgxlzu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fktsv.cn/Article/details/gofcwvmen.sHtML

[R65] 查看端口占用
来源：http://baike.vehdjk.com/Article/details/gjdyrlcvo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.vehdjk.com/Article/details/gsgzgyevq.sHtML

[R66] 定时任务
来源：http://www.m.share.bbcook.cn/Article/details/gtbpghhpl.sHtML

crontab -e;  crontab -l
来源：http://mobile.sjlbkw.cn/Article/details/gmrunqegg.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.bbcook.cn/Article/details/gxaymbqui.sHtML

openssl rand -hex 16
来源：http://www.m.share.fktsv.cn/Article/details/gljswqyrc.sHtML

[R68] 计算文件校验值
来源：http://mobile.vehdjk.com/Article/details/gjyuojawg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.vehdjk.com/Article/details/gioonjnma.sHtML

[R69] 生成随机密码
来源：http://mobile.fktsv.cn/Article/details/glughsgvz.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.epnwcf.com/Article/details/gscwwlegf.sHtML

[R70] 时间戳与互转
来源：http://wap.sjlbkw.cn/Article/details/gpltuxpte.sHtML

date +%s;  date -d @1700000000
来源：http://blog.vehdjk.com/Article/details/gduosswhk.sHtML

[R71] 日期格式化
来源：http://www.blog.epnwcf.com/Article/details/gvlaekqqx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.bbcook.cn/Article/details/gjwclvwjm.sHtML

[R72] 等待端口就绪
来源：http://baike.vehdjk.com/Article/details/gnngozzyx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.sjlbkw.cn/Article/details/gscxfpivn.sHtML

[R73] 分割大日志
来源：http://www.m.share.vehdjk.com/Article/details/gwuhiwrem.sHtML

split -l 1000 big.log part_
来源：http://m.share.vehdjk.com/Article/details/guoqzebxy.sHtML

[R74] 批量重命名
来源：http://read.share.yfazqb.com/Article/details/gtcovssop.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.tarul.cn/Article/details/ghyuqyupc.sHtML

[R75] 导出环境变量
来源：http://www.m.share.bbcook.cn/Article/details/gznxufvvp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.yfazqb.com/Article/details/gehzolsqk.sHtML

[R76] 使用临时文件
来源：http://baike.sjlbkw.cn/Article/details/gtlhxslvs.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.bbcook.cn/Article/details/gtpcfsctf.sHtML

[R77] 读取用户输入
来源：http://blog.yfazqb.com/Article/details/gcyxjwzrn.sHtML

read -rp "请输入: " ans
来源：http://3g.vehdjk.com/Article/details/gqitwsiiz.sHtML

[R78] 交互式菜单
来源：http://3g.sjlbkw.cn/Article/details/gfytfylcz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.yfazqb.com/Article/details/gwjmcnnfl.sHtML

[R79] 解析命令行选项
来源：http://read.share.bbcook.cn/Article/details/gwcmstdyq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.bbcook.cn/Article/details/grrprzhdd.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.vehdjk.com/Article/details/gkskqfyrf.sHtML

time ./run.sh
来源：http://baike.epnwcf.com/Article/details/gnpjgvizs.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/glmoibyml.sHtML

S. C / C++ 专题
来源：http://read.share.tarul.cn/Article/details/gpnjyogpz.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gdnxskzcv.sHtML

[S01] C：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gkacwzvff.sHtML

#include <stdio.h>
来源：http://m.share.epnwcf.com/Article/details/gevkllaax.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.tarul.cn/Article/details/gjbongezf.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.sjlbkw.cn/Article/details/goniywjzs.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.epnwcf.com/Article/details/gjtpnvpsw.sHtML

[S03] C：读入整数
来源：http://blog.bbcook.cn/Article/details/gtywpwcqd.sHtML

int x; scanf("%d", &x);
来源：http://mobile.yfazqb.com/Article/details/gfhyzbjjx.sHtML

[S04] C：字符串复制
来源：http://www.m.share.epnwcf.com/Article/details/galyiplbq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.epnwcf.com/Article/details/gvjxtdrvl.sHtML

[S05] C：字符串长度
来源：http://mobile.vehdjk.com/Article/details/ghugdfhvw.sHtML

strlen(s)
来源：http://3g.fktsv.cn/Article/details/gvoyooydm.sHtML

[S06] C：字符串比较
来源：http://mobile.yfazqb.com/Article/details/gyhdwidwc.sHtML

strcmp(a, b) == 0
来源：http://read.share.epnwcf.com/Article/details/gvorsrgtt.sHtML

[S07] C：数组遍历求和
来源：http://baike.sjlbkw.cn/Article/details/giscstkqq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.vehdjk.com/Article/details/gncinjvdq.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.epnwcf.com/Article/details/gkladpiux.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.vehdjk.com/Article/details/gtnaftvtf.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fktsv.cn/Article/details/gtdvqojkf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.yfazqb.com/Article/details/gjzfyjcse.sHtML

[S10] C：指针与解引用
来源：http://baike.epnwcf.com/Article/details/ghjboyetx.sHtML

int *p = &a;  *p = 5;
来源：http://wap.epnwcf.com/Article/details/gblyzdmza.sHtML

[S11] C：逐行读文件
来源：http://baike.bbcook.cn/Article/details/gdlvrsyxp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.yfazqb.com/Article/details/gcyqzctje.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.tarul.cn/Article/details/gfcibckpr.sHtML

fclose(f);
来源：http://3g.fktsv.cn/Article/details/gyzszlfdu.sHtML

[S12] C：写文件
来源：http://read.share.yfazqb.com/Article/details/gliqpttkt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.tarul.cn/Article/details/ggaxusygb.sHtML

[S13] C：宏定义
来源：http://www.blog.bbcook.cn/Article/details/grzwxqqme.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.epnwcf.com/Article/details/ggufiaiem.sHtML

[S14] C：枚举
来源：http://www.m.share.tarul.cn/Article/details/gucyckjij.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.tarul.cn/Article/details/gmfmtqhga.sHtML

[S15] C：类型转换
来源：http://3g.sjlbkw.cn/Article/details/gvqamwryq.sHtML

(double) a / b
来源：http://m.share.tarul.cn/Article/details/gszfdentt.sHtML

[S16] C：位操作置位
来源：http://m.share.fktsv.cn/Article/details/geabtbtqx.sHtML

x |= (1 << 3);
来源：http://mobile.yfazqb.com/Article/details/gckezftbk.sHtML

[S17] C：安全拼接字符串
来源：http://wap.epnwcf.com/Article/details/gnsegvtws.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.epnwcf.com/Article/details/gvmvhpstc.sHtML

[S18] C：命令行参数
来源：http://www.share.bbcook.cn/Article/details/gtyjtflyi.sHtML

int main(int argc, char **argv)
来源：http://3g.tarul.cn/Article/details/guukabzjh.sHtML

[S19] C：快速排序
来源：http://wap.tarul.cn/Article/details/ggmvplkpm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.sjlbkw.cn/Article/details/glnjmcwgq.sHtML

[S20] C：二分查找
来源：http://wap.epnwcf.com/Article/details/ggccuavdu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.yfazqb.com/Article/details/gengbijnw.sHtML

[S21] C：字符类别判断
来源：http://baike.tarul.cn/Article/details/gebufipgk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.bbcook.cn/Article/details/ggwpjjtse.sHtML

[S22] C：字符串转数字
来源：http://3g.yfazqb.com/Article/details/gppmenhjm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.bbcook.cn/Article/details/gkucxlfhi.sHtML

[S23] C：随机数
来源：http://wap.vehdjk.com/Article/details/gqotgoavq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.epnwcf.com/Article/details/gnabcblob.sHtML

[S24] C：获取本地时间
来源：http://mobile.sjlbkw.cn/Article/details/gprrwxwmu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.yfazqb.com/Article/details/gggknwjqn.sHtML

[S25] C：内存拷贝
来源：http://wap.vehdjk.com/Article/details/govctnwil.sHtML

memcpy(dst, src, n);
来源：http://3g.bbcook.cn/Article/details/grkcszooc.sHtML

[S26] C：内存清零
来源：http://3g.bbcook.cn/Article/details/gwthievvo.sHtML

memset(a, 0, sizeof a);
来源：http://wap.sjlbkw.cn/Article/details/grjopdncc.sHtML

[S27] C：定义常量
来源：http://www.share.vehdjk.com/Article/details/gapkgzdta.sHtML

const double PI = 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/gierfhtzh.sHtML

[S28] C：静态变量
来源：http://baike.epnwcf.com/Article/details/gajfokxwl.sHtML

static int counter = 0;
来源：http://wap.fktsv.cn/Article/details/gtplqdhoa.sHtML

[S29] C：变参函数
来源：http://www.m.share.tarul.cn/Article/details/gdbgbqool.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.vehdjk.com/Article/details/gihpwqgxg.sHtML

[S30] C：头文件保护
来源：http://baike.epnwcf.com/Article/details/gcxcypbyx.sHtML

#ifndef X_H
来源：http://baike.yfazqb.com/Article/details/gvpxhtxkz.sHtML

#define X_H
来源：http://3g.vehdjk.com/Article/details/grgtocfia.sHtML

#endif
来源：http://m.share.bbcook.cn/Article/details/gmvnqkutn.sHtML

[S31] C++：Hello World
来源：http://m.share.bbcook.cn/Article/details/gfnypbbai.sHtML

#include <iostream>
来源：http://blog.yfazqb.com/Article/details/geztpopzs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fktsv.cn/Article/details/grjncvanx.sHtML

[S32] C++：字符串
来源：http://blog.yfazqb.com/Article/details/goliaqlcj.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.epnwcf.com/Article/details/ggraeiokj.sHtML

[S33] C++：vector 增删
来源：http://mobile.yfazqb.com/Article/details/gmukjgxvb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.vehdjk.com/Article/details/ggxtugaiv.sHtML

[S34] C++：遍历 vector
来源：http://wap.tarul.cn/Article/details/gwpzurasl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.tarul.cn/Article/details/ghlofupfw.sHtML

[S35] C++：map
来源：http://wap.yfazqb.com/Article/details/gdrhrtcmv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.yfazqb.com/Article/details/glqfcktam.sHtML

[S36] C++：unordered_map
来源：http://www.blog.yfazqb.com/Article/details/gkesicswy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.bbcook.cn/Article/details/gegthgldu.sHtML

[S37] C++：set
来源：http://m.share.sjlbkw.cn/Article/details/glgqqdoug.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.bbcook.cn/Article/details/gmmvyfjmu.sHtML

[S38] C++：排序
来源：http://www.blog.vehdjk.com/Article/details/gzwpaeqjz.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.epnwcf.com/Article/details/ghbhiibaw.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.sjlbkw.cn/Article/details/gyqrjgmhu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.vehdjk.com/Article/details/guyrgwrix.sHtML

[S40] C++：查找元素
来源：http://3g.sjlbkw.cn/Article/details/glizmxseh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.vehdjk.com/Article/details/gjkvrqkjl.sHtML

[S41] C++：类与构造函数
来源：http://read.share.yfazqb.com/Article/details/gwgkrchqx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.bbcook.cn/Article/details/gkmffhred.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.yfazqb.com/Article/details/grzdrdsnf.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.epnwcf.com/Article/details/gnpdgezdq.sHtML

[S43] C++：智能指针
来源：http://m.share.vehdjk.com/Article/details/grcedxmuf.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fktsv.cn/Article/details/gfaxoydnp.sHtML

[S44] C++：引用传参
来源：http://www.blog.epnwcf.com/Article/details/grgfkxnsv.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.tarul.cn/Article/details/gycyvzgyl.sHtML

[S45] C++：lambda
来源：http://blog.yfazqb.com/Article/details/ghufwyjol.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.bbcook.cn/Article/details/gpfbaeeoh.sHtML

[S46] C++：函数模板
来源：http://mobile.fktsv.cn/Article/details/gvlxyhjjz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.bbcook.cn/Article/details/gmxkbizqx.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fktsv.cn/Article/details/ggmnpvesp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.yfazqb.com/Article/details/gsgutnbko.sHtML

[S48] C++：逐行读文件
来源：http://www.share.epnwcf.com/Article/details/glmibciji.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.yfazqb.com/Article/details/gzwebikbg.sHtML

while (std::getline(in, line)) { }
来源：http://blog.yfazqb.com/Article/details/gmysqkaor.sHtML

[S49] C++：写文件
来源：http://read.share.yfazqb.com/Article/details/gahhnkbft.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fktsv.cn/Article/details/gkrmuicxn.sHtML

[S50] C++：格式化数字
来源：http://3g.yfazqb.com/Article/details/ghiniiobn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.bbcook.cn/Article/details/gxlyqyfpy.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fktsv.cn/Article/details/gglcbxonb.sHtML

static_cast<double>(a) / b
来源：http://mobile.epnwcf.com/Article/details/gxszfuaoa.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.epnwcf.com/Article/details/geunkxlyi.sHtML

int size() const noexcept { return n_; }
来源：http://blog.sjlbkw.cn/Article/details/gcjpavylu.sHtML

[S53] C++：移动语义
来源：http://m.share.vehdjk.com/Article/details/gckblnmpx.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.yfazqb.com/Article/details/gkhrrngjm.sHtML

[S54] C++：异常处理
来源：http://baike.bbcook.cn/Article/details/grfpiafsj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.bbcook.cn/Article/details/grpuodvqv.sHtML

[S55] C++：结构化绑定
来源：http://baike.sjlbkw.cn/Article/details/gnttankgc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.tarul.cn/Article/details/gdlurewzr.sHtML

[S56] C++：optional
来源：http://3g.sjlbkw.cn/Article/details/gzeyyanjs.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.vehdjk.com/Article/details/gtmeusjzq.sHtML

[S57] C++：编译期常量
来源：http://read.share.sjlbkw.cn/Article/details/gwlqulxpn.sHtML

constexpr int N = 10;
来源：http://www.blog.bbcook.cn/Article/details/gkirlrjvs.sHtML

[S58] C++：命名空间
来源：http://blog.epnwcf.com/Article/details/grmqwcuqh.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.tarul.cn/Article/details/gqfacznhg.sHtML

[S59] C++：静态断言
来源：http://www.m.share.sjlbkw.cn/Article/details/gbfoalhyo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.yfazqb.com/Article/details/gqrrlbaie.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.epnwcf.com/Article/details/ggotskxxv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.tarul.cn/Article/details/gbforwutj.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gympgivbp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.epnwcf.com/Article/details/gpqdwbpxb.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gzplwcatp.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gfhgzvovn.sHtML

println("Hello")
来源：http://wap.fktsv.cn/Article/details/gsybquufo.sHtML

[T02] Kotlin：变量
来源：http://baike.epnwcf.com/Article/details/gwfcmphsr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.epnwcf.com/Article/details/gzkdscuvv.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fktsv.cn/Article/details/grzcvzpgr.sHtML

"值: $b"
来源：http://wap.vehdjk.com/Article/details/gbktfvyjc.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.tarul.cn/Article/details/gjdtzinxe.sHtML

val n: String? = null;  n?.length
来源：http://read.share.vehdjk.com/Article/details/gtkqbyuto.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.bbcook.cn/Article/details/gdjkvovus.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.sjlbkw.cn/Article/details/gcakmyktp.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.yfazqb.com/Article/details/grulajhnv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fktsv.cn/Article/details/gsjipohca.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.epnwcf.com/Article/details/geocjgymb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.yfazqb.com/Article/details/gtfbllkgh.sHtML

[T08] Kotlin：数据类
来源：http://blog.fktsv.cn/Article/details/gxqlhdfke.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fktsv.cn/Article/details/gdxnmsnmp.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fktsv.cn/Article/details/gfzpipawu.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.sjlbkw.cn/Article/details/gfauqymft.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.yfazqb.com/Article/details/gkaebrlpr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.epnwcf.com/Article/details/gbtpkeiki.sHtML

[T11] Kotlin：协程
来源：http://3g.fktsv.cn/Article/details/gfgbykftc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fktsv.cn/Article/details/gejrhjsrx.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fktsv.cn/Article/details/glphdzdem.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.bbcook.cn/Article/details/gbvszjzqy.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.bbcook.cn/Article/details/gdlwotsgv.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.sjlbkw.cn/Article/details/grlzqvhsq.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.yfazqb.com/Article/details/gzmtjwcud.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.bbcook.cn/Article/details/gfhswucvv.sHtML

[T15] Kotlin：接口
来源：http://m.share.tarul.cn/Article/details/gsvejvexf.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.bbcook.cn/Article/details/gaxczjynm.sHtML

[T16] Swift：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/ghoovewqq.sHtML

print("Hello")
来源：http://3g.yfazqb.com/Article/details/gugnwibzt.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.epnwcf.com/Article/details/gaecjxtpm.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.yfazqb.com/Article/details/gfpjzojre.sHtML

[T18] Swift：字符串插值
来源：http://read.share.sjlbkw.cn/Article/details/gkxeaseqy.sHtML

"值: \(b)"
来源：http://mobile.bbcook.cn/Article/details/gqjawizip.sHtML

[T19] Swift：可选绑定
来源：http://blog.epnwcf.com/Article/details/gwkvgksva.sHtML

if let n = opt { print(n) }
来源：http://blog.tarul.cn/Article/details/gaqzlbzem.sHtML

[T20] Swift：数组操作
来源：http://baike.bbcook.cn/Article/details/gvklkhxed.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.vehdjk.com/Article/details/gmaxgfets.sHtML

[T21] Swift：遍历
来源：http://blog.sjlbkw.cn/Article/details/gbsffbcrv.sHtML

for x in a { print(x) }
来源：http://m.share.bbcook.cn/Article/details/gfwbojryi.sHtML

[T22] Swift：字典
来源：http://read.share.sjlbkw.cn/Article/details/gdnojizee.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fktsv.cn/Article/details/gliscqjfk.sHtML

[T23] Swift：函数
来源：http://blog.bbcook.cn/Article/details/gffdkagwp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.sjlbkw.cn/Article/details/giajntheb.sHtML

[T24] Swift：闭包
来源：http://www.share.sjlbkw.cn/Article/details/gkunrpwbz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.bbcook.cn/Article/details/gyatkawhv.sHtML

[T25] Swift：结构体
来源：http://blog.yfazqb.com/Article/details/gsykpdprk.sHtML

struct P { var x: Int }
来源：http://read.share.vehdjk.com/Article/details/gpglefsvx.sHtML

[T26] Swift：类与重写
来源：http://wap.fktsv.cn/Article/details/grdktjlrh.sHtML

class A: Base { override func f() {} }
来源：http://blog.yfazqb.com/Article/details/gmwwwzhuq.sHtML

[T27] Swift：错误处理
来源：http://wap.yfazqb.com/Article/details/gskianrmg.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.yfazqb.com/Article/details/gdssbyntv.sHtML

[T28] Swift：枚举
来源：http://mobile.sjlbkw.cn/Article/details/gfujqajqp.sHtML

enum Color { case red, green }
来源：http://baike.yfazqb.com/Article/details/gtrfxjczh.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.epnwcf.com/Article/details/gmrzusvtf.sHtML

guard let x = opt else { return }
来源：http://m.share.sjlbkw.cn/Article/details/gtlvhexvq.sHtML

[T30] Swift：协议
来源：http://wap.sjlbkw.cn/Article/details/ghmgawlqu.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.vehdjk.com/Article/details/gkmwainlf.sHtML

[T31] Lua：Hello World
来源：http://www.blog.sjlbkw.cn/Article/details/gukptaeio.sHtML

print("Hello")
来源：http://3g.epnwcf.com/Article/details/gfmczjplk.sHtML

[T32] Lua：局部变量
来源：http://baike.bbcook.cn/Article/details/gxfgoqitx.sHtML

local a = 1
来源：http://blog.epnwcf.com/Article/details/gderneuiv.sHtML

[T33] Lua：表（数组）
来源：http://wap.vehdjk.com/Article/details/glanxpdht.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.epnwcf.com/Article/details/gtdlgfmoe.sHtML

[T34] Lua：遍历表
来源：http://wap.fktsv.cn/Article/details/grxbgjoap.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.vehdjk.com/Article/details/gdzhgdqks.sHtML

[T35] Lua：字典表
来源：http://baike.fktsv.cn/Article/details/gtzgsnhoy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.epnwcf.com/Article/details/gnvqrsmik.sHtML

[T36] Lua：函数
来源：http://baike.bbcook.cn/Article/details/guyskjcxs.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.sjlbkw.cn/Article/details/gqqpzdqlv.sHtML

[T37] Lua：字符串拼接
来源：http://3g.yfazqb.com/Article/details/goxpkzcgt.sHtML

"a" .. "b"
来源：http://3g.yfazqb.com/Article/details/grnerocxl.sHtML

[T38] Lua：条件
来源：http://blog.epnwcf.com/Article/details/gfkyahtid.sHtML

if x > 0 then print("正") end
来源：http://3g.fktsv.cn/Article/details/gzrdokfaj.sHtML

[T39] Lua：模式匹配
来源：http://baike.tarul.cn/Article/details/gnfphjpqj.sHtML

string.find(s, "%d+")
来源：http://blog.epnwcf.com/Article/details/gwcjarymz.sHtML

[T40] Lua：元表
来源：http://baike.vehdjk.com/Article/details/goummfjkp.sHtML

setmetatable({}, { __index = base })
来源：http://wap.yfazqb.com/Article/details/gesmleioq.sHtML

[T41] Perl：Hello World
来源：http://m.share.epnwcf.com/Article/details/glxsngyxs.sHtML

print "Hello\n";
来源：http://wap.fktsv.cn/Article/details/gmclpapeo.sHtML

[T42] Perl：变量类型
来源：http://www.blog.tarul.cn/Article/details/gxeilqtis.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.vehdjk.com/Article/details/gauprkzct.sHtML

[T43] Perl：字符串插值
来源：http://3g.yfazqb.com/Article/details/gwmnjbhkk.sHtML

"值: $a"
来源：http://baike.epnwcf.com/Article/details/gpoochgfp.sHtML

[T44] Perl：条件
来源：http://baike.vehdjk.com/Article/details/glkiszlyi.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.tarul.cn/Article/details/gwlbttmuy.sHtML

[T45] Perl：数组遍历
来源：http://baike.sjlbkw.cn/Article/details/gtlogqxjm.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.epnwcf.com/Article/details/gchgbfiyw.sHtML

[T46] Perl：哈希操作
来源：http://3g.tarul.cn/Article/details/gsijcgqug.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.tarul.cn/Article/details/gywmwuymp.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.epnwcf.com/Article/details/guldrlqqq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fktsv.cn/Article/details/gpkgedvtq.sHtML

[T48] Perl：正则替换
来源：http://wap.tarul.cn/Article/details/gbvoyiagy.sHtML

$s =~ s/old/new/g;
来源：http://read.share.yfazqb.com/Article/details/gwkmbecsb.sHtML

[T49] Perl：函数
来源：http://mobile.tarul.cn/Article/details/grkhaykkt.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.vehdjk.com/Article/details/gihwzrrzx.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.tarul.cn/Article/details/gykjwqgwx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.tarul.cn/Article/details/gctdrycat.sHtML


<!-- 参考信息 -->