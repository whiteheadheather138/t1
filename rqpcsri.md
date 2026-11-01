代发 wailian999

find . -name "*.log" -type f
来源：http://www.m.share.epnwcf.com/Article/details/gzejckwug.sHtML

[R44] 按修改时间查找
来源：http://read.share.fktsv.cn/Article/details/gwmrrwrjx.sHtML

find . -mtime -7 -type f
来源：http://baike.epnwcf.com/Article/details/gukfgxnhc.sHtML

[R45] 批量删除
来源：http://www.share.fktsv.cn/Article/details/gnxgnwvnj.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.bbcook.cn/Article/details/gztkaxzux.sHtML

[R46] 递归替换文件内容
来源：http://baike.vehdjk.com/Article/details/gopchukiq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fktsv.cn/Article/details/gqohcsnjx.sHtML

[R47] sed 单行替换
来源：http://read.share.tarul.cn/Article/details/gptjjfvlh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.epnwcf.com/Article/details/gxiihnnuc.sHtML

[R48] awk 取指定列
来源：http://m.share.yfazqb.com/Article/details/gcvjoagkk.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.epnwcf.com/Article/details/gqbcczlxk.sHtML

[R49] awk 带条件
来源：http://mobile.sjlbkw.cn/Article/details/ggnuypguh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.vehdjk.com/Article/details/gicpoqiha.sHtML

[R50] awk 求和
来源：http://3g.sjlbkw.cn/Article/details/ggqqczwkm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.bbcook.cn/Article/details/gsimbburg.sHtML

[R51] 排序去重取前几
来源：http://read.share.sjlbkw.cn/Article/details/gtvqrstrb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.yfazqb.com/Article/details/gpgdochkl.sHtML

[R52] 统计行数
来源：http://www.m.share.vehdjk.com/Article/details/gatcvoisj.sHtML

wc -l a.txt
来源：http://baike.tarul.cn/Article/details/gqihdjfnr.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fktsv.cn/Article/details/gkykoeaxu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.yfazqb.com/Article/details/gnldgyivm.sHtML

[R54] 比较两个文件
来源：http://3g.yfazqb.com/Article/details/gsypqfwzo.sHtML

diff a.txt b.txt
来源：http://baike.epnwcf.com/Article/details/gdjdsqxjh.sHtML

[R55] 压缩与解压
来源：http://m.share.sjlbkw.cn/Article/details/gqjndbghs.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.tarul.cn/Article/details/gkksjfane.sHtML

[R56] 远程拷贝
来源：http://wap.yfazqb.com/Article/details/gdenlevqy.sHtML

scp file user@host:/path/
来源：http://mobile.sjlbkw.cn/Article/details/gtgzqnpzh.sHtML

[R57] 远程执行命令
来源：http://m.share.sjlbkw.cn/Article/details/gmaqaitds.sHtML

ssh user@host 'uptime'
来源：http://read.share.fktsv.cn/Article/details/gdzyvrkms.sHtML

[R58] 下载文件
来源：http://mobile.bbcook.cn/Article/details/gjnobsacg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.yfazqb.com/Article/details/gkxijnvyg.sHtML

[R59] 发 POST JSON
来源：http://3g.tarul.cn/Article/details/gxtxwfhjl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.tarul.cn/Article/details/gqwtzwkjm.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.yfazqb.com/Article/details/gxxewfwtd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.vehdjk.com/Article/details/gquxemako.sHtML

[R61] 磁盘占用
来源：http://baike.bbcook.cn/Article/details/gmyorumog.sHtML

df -h;  du -sh *
来源：http://m.share.vehdjk.com/Article/details/gbjtkyrsi.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.yfazqb.com/Article/details/glyfpducn.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.epnwcf.com/Article/details/gswyskmwt.sHtML

[R63] 内存与进程
来源：http://m.share.fktsv.cn/Article/details/geitncccz.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fktsv.cn/Article/details/gadtocuyy.sHtML

[R64] 结束进程
来源：http://www.share.fktsv.cn/Article/details/grphqhczk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.epnwcf.com/Article/details/guidahoyh.sHtML

[R65] 查看端口占用
来源：http://www.share.yfazqb.com/Article/details/gdvxvgzeb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.tarul.cn/Article/details/gdfxoknay.sHtML

[R66] 定时任务
来源：http://www.m.share.vehdjk.com/Article/details/gbytafvcl.sHtML

crontab -e;  crontab -l
来源：http://read.share.epnwcf.com/Article/details/gstbsawsm.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.bbcook.cn/Article/details/gkawrznru.sHtML

openssl rand -hex 16
来源：http://baike.sjlbkw.cn/Article/details/gdmmrhivp.sHtML

[R68] 计算文件校验值
来源：http://baike.sjlbkw.cn/Article/details/gwpvwkttu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.epnwcf.com/Article/details/gvmwaluxi.sHtML

[R69] 生成随机密码
来源：http://read.share.fktsv.cn/Article/details/gmwjptlbm.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.yfazqb.com/Article/details/gnivmbudp.sHtML

[R70] 时间戳与互转
来源：http://baike.fktsv.cn/Article/details/gfpsmdkjz.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fktsv.cn/Article/details/grudlwwjn.sHtML

[R71] 日期格式化
来源：http://m.share.bbcook.cn/Article/details/gdbitpsly.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.sjlbkw.cn/Article/details/gwkqilswh.sHtML

[R72] 等待端口就绪
来源：http://3g.vehdjk.com/Article/details/gjrsumfug.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.bbcook.cn/Article/details/gvdxcxxeb.sHtML

[R73] 分割大日志
来源：http://mobile.bbcook.cn/Article/details/gvahbasgm.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.epnwcf.com/Article/details/gumkfxogg.sHtML

[R74] 批量重命名
来源：http://www.blog.fktsv.cn/Article/details/gzqiuiyla.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.yfazqb.com/Article/details/gkxdvmtob.sHtML

[R75] 导出环境变量
来源：http://read.share.tarul.cn/Article/details/gpcztoebu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fktsv.cn/Article/details/glfevmlmg.sHtML

[R76] 使用临时文件
来源：http://read.share.vehdjk.com/Article/details/gvmonwuvo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.sjlbkw.cn/Article/details/ghxrduiym.sHtML

[R77] 读取用户输入
来源：http://read.share.fktsv.cn/Article/details/gstceztny.sHtML

read -rp "请输入: " ans
来源：http://read.share.yfazqb.com/Article/details/gfrzldwtg.sHtML

[R78] 交互式菜单
来源：http://baike.vehdjk.com/Article/details/gjetfipzo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.bbcook.cn/Article/details/goyaljrbr.sHtML

[R79] 解析命令行选项
来源：http://wap.yfazqb.com/Article/details/gmkojuppy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.bbcook.cn/Article/details/gfyzasfwd.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.tarul.cn/Article/details/gcijsfell.sHtML

time ./run.sh
来源：http://www.blog.sjlbkw.cn/Article/details/gyykwnfvj.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gwnkpyykz.sHtML

S. C / C++ 专题
来源：http://baike.sjlbkw.cn/Article/details/gnnbrknxw.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/galbzmazq.sHtML

[S01] C：Hello World
来源：http://wap.bbcook.cn/Article/details/giierdlim.sHtML

#include <stdio.h>
来源：http://blog.bbcook.cn/Article/details/gqypnclru.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.vehdjk.com/Article/details/gomhvdije.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fktsv.cn/Article/details/gfvmvkxqu.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.yfazqb.com/Article/details/gsqcrwdkx.sHtML

[S03] C：读入整数
来源：http://www.m.share.tarul.cn/Article/details/gnsexnoja.sHtML

int x; scanf("%d", &x);
来源：http://3g.yfazqb.com/Article/details/gjpzvsayi.sHtML

[S04] C：字符串复制
来源：http://www.share.bbcook.cn/Article/details/grekczdou.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.sjlbkw.cn/Article/details/grovehvlj.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fktsv.cn/Article/details/giufavger.sHtML

strlen(s)
来源：http://wap.bbcook.cn/Article/details/gynccworz.sHtML

[S06] C：字符串比较
来源：http://m.share.epnwcf.com/Article/details/gjhyoikdk.sHtML

strcmp(a, b) == 0
来源：http://www.share.vehdjk.com/Article/details/gjqiwqcaa.sHtML

[S07] C：数组遍历求和
来源：http://read.share.yfazqb.com/Article/details/gpwucefez.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.bbcook.cn/Article/details/gbfmnswst.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.vehdjk.com/Article/details/gudckbikv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fktsv.cn/Article/details/gsnbioinl.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.vehdjk.com/Article/details/gjoiuxack.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.sjlbkw.cn/Article/details/gjqiktmqt.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.sjlbkw.cn/Article/details/gtxoosnsi.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fktsv.cn/Article/details/gnokmwpvj.sHtML

[S11] C：逐行读文件
来源：http://wap.tarul.cn/Article/details/gkcypbijf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.tarul.cn/Article/details/gzthnnozq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.vehdjk.com/Article/details/gqwpykjzs.sHtML

fclose(f);
来源：http://blog.sjlbkw.cn/Article/details/gppfcjhih.sHtML

[S12] C：写文件
来源：http://www.share.tarul.cn/Article/details/giucoiase.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.sjlbkw.cn/Article/details/gcxfkvoiw.sHtML

[S13] C：宏定义
来源：http://www.share.yfazqb.com/Article/details/gfxsrwfrl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.bbcook.cn/Article/details/gmuhavifz.sHtML

[S14] C：枚举
来源：http://3g.bbcook.cn/Article/details/gvpmaesmd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.vehdjk.com/Article/details/gyqdpglhx.sHtML

[S15] C：类型转换
来源：http://www.share.fktsv.cn/Article/details/gveovdheb.sHtML

(double) a / b
来源：http://3g.epnwcf.com/Article/details/ghqozquhc.sHtML

[S16] C：位操作置位
来源：http://read.share.sjlbkw.cn/Article/details/ghmugzirr.sHtML

x |= (1 << 3);
来源：http://mobile.vehdjk.com/Article/details/gxjuzmtyx.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.tarul.cn/Article/details/gbefyrtqs.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.yfazqb.com/Article/details/gkdhdmdre.sHtML

[S18] C：命令行参数
来源：http://blog.yfazqb.com/Article/details/gxudkizhs.sHtML

int main(int argc, char **argv)
来源：http://wap.sjlbkw.cn/Article/details/gfhevnpua.sHtML

[S19] C：快速排序
来源：http://baike.vehdjk.com/Article/details/ghkcojblr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.vehdjk.com/Article/details/gijcpzvjz.sHtML

[S20] C：二分查找
来源：http://baike.epnwcf.com/Article/details/gfcnucorz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fktsv.cn/Article/details/gfssjjpgn.sHtML

[S21] C：字符类别判断
来源：http://wap.tarul.cn/Article/details/gcsvnadkq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.tarul.cn/Article/details/giupktqge.sHtML

[S22] C：字符串转数字
来源：http://wap.sjlbkw.cn/Article/details/grsrdiawi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.tarul.cn/Article/details/gkhphkjac.sHtML

[S23] C：随机数
来源：http://www.blog.tarul.cn/Article/details/giqzkygbt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fktsv.cn/Article/details/gqezgiusr.sHtML

[S24] C：获取本地时间
来源：http://read.share.tarul.cn/Article/details/gbvuhbxrz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.bbcook.cn/Article/details/gdavwdqmp.sHtML

[S25] C：内存拷贝
来源：http://mobile.epnwcf.com/Article/details/gjzqnvdwh.sHtML

memcpy(dst, src, n);
来源：http://www.share.epnwcf.com/Article/details/gvdviofcm.sHtML

[S26] C：内存清零
来源：http://blog.epnwcf.com/Article/details/grrwhvulg.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.tarul.cn/Article/details/ghkjahpvw.sHtML

[S27] C：定义常量
来源：http://3g.vehdjk.com/Article/details/gaotjlcgc.sHtML

const double PI = 3.14159;
来源：http://baike.epnwcf.com/Article/details/gqhhsqedv.sHtML

[S28] C：静态变量
来源：http://m.share.yfazqb.com/Article/details/grlgxchtw.sHtML

static int counter = 0;
来源：http://wap.vehdjk.com/Article/details/ggetwkogu.sHtML

[S29] C：变参函数
来源：http://www.blog.bbcook.cn/Article/details/gcuogkcst.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.bbcook.cn/Article/details/gjriqrabq.sHtML

[S30] C：头文件保护
来源：http://wap.tarul.cn/Article/details/gpfcxbich.sHtML

#ifndef X_H
来源：http://baike.sjlbkw.cn/Article/details/gvtmjbxxg.sHtML

#define X_H
来源：http://3g.bbcook.cn/Article/details/grnyzimmz.sHtML

#endif
来源：http://read.share.vehdjk.com/Article/details/grouvyluc.sHtML

[S31] C++：Hello World
来源：http://baike.bbcook.cn/Article/details/gqafjhskw.sHtML

#include <iostream>
来源：http://baike.fktsv.cn/Article/details/gfbzkcuit.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.sjlbkw.cn/Article/details/gfndtmsaf.sHtML

[S32] C++：字符串
来源：http://m.share.epnwcf.com/Article/details/gxpglghbo.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.bbcook.cn/Article/details/gqjjkocgu.sHtML

[S33] C++：vector 增删
来源：http://read.share.tarul.cn/Article/details/ggapcwmse.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.sjlbkw.cn/Article/details/grzijkrma.sHtML

[S34] C++：遍历 vector
来源：http://wap.bbcook.cn/Article/details/gdziuqmam.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fktsv.cn/Article/details/gbdfntgfb.sHtML

[S35] C++：map
来源：http://m.share.yfazqb.com/Article/details/geoynkiaz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.tarul.cn/Article/details/gfinjseta.sHtML

[S36] C++：unordered_map
来源：http://blog.vehdjk.com/Article/details/gdiwilrnj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fktsv.cn/Article/details/giaknxwld.sHtML

[S37] C++：set
来源：http://baike.yfazqb.com/Article/details/gmyjipcdc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.tarul.cn/Article/details/gwbjengzf.sHtML

[S38] C++：排序
来源：http://www.m.share.fktsv.cn/Article/details/gwnllmwzi.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.yfazqb.com/Article/details/glkdadpev.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.epnwcf.com/Article/details/gwpopzxao.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.sjlbkw.cn/Article/details/gxdhupakj.sHtML

[S40] C++：查找元素
来源：http://mobile.sjlbkw.cn/Article/details/glducswtw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.bbcook.cn/Article/details/grenodsew.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fktsv.cn/Article/details/gqtkffvcn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.sjlbkw.cn/Article/details/gmjmuoxkz.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.yfazqb.com/Article/details/gtqtnqnya.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.vehdjk.com/Article/details/gioplzlsj.sHtML

[S43] C++：智能指针
来源：http://mobile.fktsv.cn/Article/details/gbjxenlyb.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fktsv.cn/Article/details/gparsfccy.sHtML

[S44] C++：引用传参
来源：http://www.share.bbcook.cn/Article/details/grlddhsos.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.tarul.cn/Article/details/gpajgbjwb.sHtML

[S45] C++：lambda
来源：http://mobile.yfazqb.com/Article/details/gyvmiohle.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fktsv.cn/Article/details/gsbajsrah.sHtML

[S46] C++：函数模板
来源：http://www.m.share.yfazqb.com/Article/details/gajgfpmte.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.sjlbkw.cn/Article/details/gopfgjazx.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.tarul.cn/Article/details/guqtsbiiy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.sjlbkw.cn/Article/details/gbmzqbqpo.sHtML

[S48] C++：逐行读文件
来源：http://wap.sjlbkw.cn/Article/details/ghfsjbtcf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fktsv.cn/Article/details/ggxgdxnrc.sHtML

while (std::getline(in, line)) { }
来源：http://3g.vehdjk.com/Article/details/gfdskdvok.sHtML

[S49] C++：写文件
来源：http://www.blog.yfazqb.com/Article/details/gdpsgsotx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.yfazqb.com/Article/details/gmtzqotbt.sHtML

[S50] C++：格式化数字
来源：http://3g.sjlbkw.cn/Article/details/gkmdvrafn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.bbcook.cn/Article/details/glieuyxlw.sHtML

[S51] C++：显式类型转换
来源：http://m.share.yfazqb.com/Article/details/ggjlncbop.sHtML

static_cast<double>(a) / b
来源：http://3g.sjlbkw.cn/Article/details/gwyiuaceg.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fktsv.cn/Article/details/gxuzapbuo.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fktsv.cn/Article/details/gmvnnltbm.sHtML

[S53] C++：移动语义
来源：http://www.share.yfazqb.com/Article/details/gijeysrai.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.epnwcf.com/Article/details/gonhmjyhh.sHtML

[S54] C++：异常处理
来源：http://wap.tarul.cn/Article/details/gnwbifrqw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.tarul.cn/Article/details/gexkekanf.sHtML

[S55] C++：结构化绑定
来源：http://3g.bbcook.cn/Article/details/gqfnwjxbj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gsemgnmdq.sHtML

[S56] C++：optional
来源：http://baike.sjlbkw.cn/Article/details/gdcusqmnw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.epnwcf.com/Article/details/gfeinqhlm.sHtML

[S57] C++：编译期常量
来源：http://blog.bbcook.cn/Article/details/giwsiapmg.sHtML

constexpr int N = 10;
来源：http://blog.fktsv.cn/Article/details/gakefulxl.sHtML

[S58] C++：命名空间
来源：http://baike.tarul.cn/Article/details/gyqbsqmrz.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fktsv.cn/Article/details/ghcsqywyu.sHtML

[S59] C++：静态断言
来源：http://3g.bbcook.cn/Article/details/ghptwrtce.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.bbcook.cn/Article/details/gemghzsxf.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.tarul.cn/Article/details/gbtcnyzzn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.vehdjk.com/Article/details/gxyymjnlf.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/ggwzffino.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.yfazqb.com/Article/details/gmrhciscu.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gnmsswisl.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.epnwcf.com/Article/details/gkhcksbpx.sHtML

println("Hello")
来源：http://blog.tarul.cn/Article/details/gxeghtlvc.sHtML

[T02] Kotlin：变量
来源：http://wap.yfazqb.com/Article/details/gjsiyddwq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.vehdjk.com/Article/details/gjtbijhbe.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.sjlbkw.cn/Article/details/grmtcbbyh.sHtML

"值: $b"
来源：http://www.m.share.tarul.cn/Article/details/gtyhuwdcq.sHtML

[T04] Kotlin：空安全
来源：http://baike.yfazqb.com/Article/details/gytefysyo.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fktsv.cn/Article/details/gpvynwtck.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.tarul.cn/Article/details/gpxrbmejt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.bbcook.cn/Article/details/gojxdcqnd.sHtML

[T06] Kotlin：集合映射
来源：http://wap.yfazqb.com/Article/details/grffhfxxj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.sjlbkw.cn/Article/details/gnhzrxkkg.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.bbcook.cn/Article/details/ggftqiuew.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.epnwcf.com/Article/details/gwzjpdpgh.sHtML

[T08] Kotlin：数据类
来源：http://wap.tarul.cn/Article/details/gmowtcjtm.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fktsv.cn/Article/details/grvvqpbzw.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.epnwcf.com/Article/details/gakfjezdb.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fktsv.cn/Article/details/gsvsypcuw.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fktsv.cn/Article/details/gsrobymxe.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fktsv.cn/Article/details/gskujybur.sHtML

[T11] Kotlin：协程
来源：http://www.share.tarul.cn/Article/details/gxmyoxphw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fktsv.cn/Article/details/golgmylnk.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.vehdjk.com/Article/details/gvqntdixf.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.bbcook.cn/Article/details/gkglgzsyi.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.tarul.cn/Article/details/gyitkkdro.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.tarul.cn/Article/details/gzzbesgah.sHtML

[T14] Kotlin：循环
来源：http://baike.sjlbkw.cn/Article/details/gvtucihvl.sHtML

for (i in 1..10) println(i)
来源：http://m.share.vehdjk.com/Article/details/geqycfrgy.sHtML

[T15] Kotlin：接口
来源：http://m.share.sjlbkw.cn/Article/details/gstkihfoj.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fktsv.cn/Article/details/gqtumvfht.sHtML

[T16] Swift：Hello World
来源：http://baike.vehdjk.com/Article/details/giiuhrvcr.sHtML

print("Hello")
来源：http://www.m.share.vehdjk.com/Article/details/gpkmwcglj.sHtML

[T17] Swift：变量与常量
来源：http://baike.sjlbkw.cn/Article/details/gcycfokve.sHtML

var a = 1;  let b = 2
来源：http://3g.vehdjk.com/Article/details/ghfovmygo.sHtML

[T18] Swift：字符串插值
来源：http://3g.fktsv.cn/Article/details/gzzccvkuo.sHtML

"值: \(b)"
来源：http://m.share.bbcook.cn/Article/details/gwouuudmc.sHtML

[T19] Swift：可选绑定
来源：http://read.share.yfazqb.com/Article/details/ghmecwrmn.sHtML

if let n = opt { print(n) }
来源：http://wap.vehdjk.com/Article/details/gvgtdbxsp.sHtML

[T20] Swift：数组操作
来源：http://mobile.yfazqb.com/Article/details/gnsshfhil.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.yfazqb.com/Article/details/gbjsaultl.sHtML

[T21] Swift：遍历
来源：http://read.share.sjlbkw.cn/Article/details/ghtgeqyjf.sHtML

for x in a { print(x) }
来源：http://3g.vehdjk.com/Article/details/goqlbkvvb.sHtML

[T22] Swift：字典
来源：http://read.share.yfazqb.com/Article/details/gnnvatzid.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.bbcook.cn/Article/details/gnpkmtdof.sHtML

[T23] Swift：函数
来源：http://www.share.vehdjk.com/Article/details/gzgnoswjq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fktsv.cn/Article/details/gftozwpgq.sHtML

[T24] Swift：闭包
来源：http://3g.sjlbkw.cn/Article/details/ghvlyaewf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.tarul.cn/Article/details/gowkmnkcw.sHtML

[T25] Swift：结构体
来源：http://wap.tarul.cn/Article/details/gljajljtw.sHtML

struct P { var x: Int }
来源：http://baike.bbcook.cn/Article/details/gutigpmhx.sHtML

[T26] Swift：类与重写
来源：http://www.share.sjlbkw.cn/Article/details/gomtdxvkl.sHtML

class A: Base { override func f() {} }
来源：http://baike.fktsv.cn/Article/details/gnlzbsupt.sHtML

[T27] Swift：错误处理
来源：http://read.share.fktsv.cn/Article/details/gmgjodhlc.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fktsv.cn/Article/details/gfxdukckg.sHtML

[T28] Swift：枚举
来源：http://read.share.fktsv.cn/Article/details/gdebuusyg.sHtML

enum Color { case red, green }
来源：http://www.m.share.bbcook.cn/Article/details/gwbyamzar.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fktsv.cn/Article/details/gnridunoz.sHtML

guard let x = opt else { return }
来源：http://blog.fktsv.cn/Article/details/gwkfxootg.sHtML

[T30] Swift：协议
来源：http://m.share.tarul.cn/Article/details/geotfuuob.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.tarul.cn/Article/details/govaydlzp.sHtML

[T31] Lua：Hello World
来源：http://wap.sjlbkw.cn/Article/details/givzknkpk.sHtML

print("Hello")
来源：http://www.blog.bbcook.cn/Article/details/gxgintcjs.sHtML

[T32] Lua：局部变量
来源：http://www.blog.epnwcf.com/Article/details/gxnncomau.sHtML

local a = 1
来源：http://www.blog.vehdjk.com/Article/details/ginyimajt.sHtML

[T33] Lua：表（数组）
来源：http://read.share.yfazqb.com/Article/details/gzzjlcvol.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.sjlbkw.cn/Article/details/gefrxamgo.sHtML

[T34] Lua：遍历表
来源：http://www.blog.bbcook.cn/Article/details/gutzqxdix.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.bbcook.cn/Article/details/glyrcqrxk.sHtML

[T35] Lua：字典表
来源：http://baike.epnwcf.com/Article/details/gqxhdsxsg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fktsv.cn/Article/details/gxiuzxwvo.sHtML

[T36] Lua：函数
来源：http://www.blog.yfazqb.com/Article/details/gtcjdjtvg.sHtML

function add(a, b) return a + b end
来源：http://m.share.yfazqb.com/Article/details/gpboyuaeb.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.sjlbkw.cn/Article/details/glmdesxse.sHtML

"a" .. "b"
来源：http://www.blog.yfazqb.com/Article/details/gkkudvlrh.sHtML

[T38] Lua：条件
来源：http://blog.vehdjk.com/Article/details/gbybqycsn.sHtML

if x > 0 then print("正") end
来源：http://read.share.epnwcf.com/Article/details/gececunrk.sHtML

[T39] Lua：模式匹配
来源：http://3g.epnwcf.com/Article/details/govrcwkvb.sHtML

string.find(s, "%d+")
来源：http://3g.epnwcf.com/Article/details/gwzwhfzse.sHtML

[T40] Lua：元表
来源：http://baike.bbcook.cn/Article/details/gaotldvxe.sHtML

setmetatable({}, { __index = base })
来源：http://baike.bbcook.cn/Article/details/gfpamxdzo.sHtML

[T41] Perl：Hello World
来源：http://www.share.epnwcf.com/Article/details/gicnbxxuc.sHtML

print "Hello\n";
来源：http://www.m.share.fktsv.cn/Article/details/ghdfrztsa.sHtML

[T42] Perl：变量类型
来源：http://wap.fktsv.cn/Article/details/gywtschhe.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fktsv.cn/Article/details/gzwurppkp.sHtML

[T43] Perl：字符串插值
来源：http://www.share.vehdjk.com/Article/details/golyqadhb.sHtML

"值: $a"
来源：http://read.share.fktsv.cn/Article/details/gxfbjcgdi.sHtML

[T44] Perl：条件
来源：http://www.share.tarul.cn/Article/details/gtcdmmyby.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.vehdjk.com/Article/details/gvidxnxxy.sHtML

[T45] Perl：数组遍历
来源：http://read.share.tarul.cn/Article/details/gnfvsqtzq.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.epnwcf.com/Article/details/goennhnld.sHtML

[T46] Perl：哈希操作
来源：http://3g.epnwcf.com/Article/details/geytsbuqx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.epnwcf.com/Article/details/gofatqbhw.sHtML


<!-- 参考信息 -->