代发 wailian999

cmd >/dev/null 2>&1
来源：http://m.share.epnwcf.com/Article/details/grmyylhui.sHtML

[R42] 输入重定向
来源：http://www.share.sjlbkw.cn/Article/details/girabyhru.sHtML

wc -l < a.txt
来源：http://read.share.fktsv.cn/Article/details/gvazupfpg.sHtML

[R43] 按名字查找文件
来源：http://read.share.sjlbkw.cn/Article/details/gtgadizvv.sHtML

find . -name "*.log" -type f
来源：http://www.share.yfazqb.com/Article/details/gdgtsoyiw.sHtML

[R44] 按修改时间查找
来源：http://blog.bbcook.cn/Article/details/gabmqqjhy.sHtML

find . -mtime -7 -type f
来源：http://wap.epnwcf.com/Article/details/gfdupchbr.sHtML

[R45] 批量删除
来源：http://www.blog.vehdjk.com/Article/details/ghixkkaaf.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.yfazqb.com/Article/details/gckenkoht.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.epnwcf.com/Article/details/geeladnkd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fktsv.cn/Article/details/gxnjylipd.sHtML

[R47] sed 单行替换
来源：http://wap.yfazqb.com/Article/details/gcvmkztzr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.vehdjk.com/Article/details/ginnsjrxw.sHtML

[R48] awk 取指定列
来源：http://baike.vehdjk.com/Article/details/gwzijhklb.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.yfazqb.com/Article/details/gormqmaci.sHtML

[R49] awk 带条件
来源：http://wap.tarul.cn/Article/details/gtsnudxjb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.tarul.cn/Article/details/gvieenwoj.sHtML

[R50] awk 求和
来源：http://baike.bbcook.cn/Article/details/gideldwyp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.bbcook.cn/Article/details/ggrpjclui.sHtML

[R51] 排序去重取前几
来源：http://blog.fktsv.cn/Article/details/goatsakha.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.yfazqb.com/Article/details/gwaodmacj.sHtML

[R52] 统计行数
来源：http://www.m.share.bbcook.cn/Article/details/grcjotofr.sHtML

wc -l a.txt
来源：http://mobile.fktsv.cn/Article/details/glgoswzqz.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.tarul.cn/Article/details/ghkaxehio.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fktsv.cn/Article/details/gjqpvyplr.sHtML

[R54] 比较两个文件
来源：http://m.share.sjlbkw.cn/Article/details/gwmtrobxa.sHtML

diff a.txt b.txt
来源：http://baike.vehdjk.com/Article/details/gmhmmpjcb.sHtML

[R55] 压缩与解压
来源：http://m.share.sjlbkw.cn/Article/details/gjenqhvyk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.tarul.cn/Article/details/grsqpwgvs.sHtML

[R56] 远程拷贝
来源：http://3g.bbcook.cn/Article/details/grwovluxy.sHtML

scp file user@host:/path/
来源：http://m.share.sjlbkw.cn/Article/details/ghshmjwey.sHtML

[R57] 远程执行命令
来源：http://blog.fktsv.cn/Article/details/gdeebqdaa.sHtML

ssh user@host 'uptime'
来源：http://wap.tarul.cn/Article/details/guufuvekw.sHtML

[R58] 下载文件
来源：http://www.m.share.epnwcf.com/Article/details/gihwsfkjb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.vehdjk.com/Article/details/gcqcxhced.sHtML

[R59] 发 POST JSON
来源：http://m.share.yfazqb.com/Article/details/gfnrajjub.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.epnwcf.com/Article/details/gzkvduhqf.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fktsv.cn/Article/details/gwtiypfqm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fktsv.cn/Article/details/gdudzfodn.sHtML

[R61] 磁盘占用
来源：http://www.share.vehdjk.com/Article/details/gcbwpnwxg.sHtML

df -h;  du -sh *
来源：http://wap.sjlbkw.cn/Article/details/gouvdytuj.sHtML

[R62] 找最占空间的文件
来源：http://baike.epnwcf.com/Article/details/gmcquodin.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.sjlbkw.cn/Article/details/gnnkfvqye.sHtML

[R63] 内存与进程
来源：http://m.share.bbcook.cn/Article/details/gfleibngi.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.tarul.cn/Article/details/gjpgibepe.sHtML

[R64] 结束进程
来源：http://www.blog.tarul.cn/Article/details/gjpfkdbfd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.vehdjk.com/Article/details/giuzbvknj.sHtML

[R65] 查看端口占用
来源：http://www.m.share.tarul.cn/Article/details/gnunzuuom.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.sjlbkw.cn/Article/details/gkafvlbrd.sHtML

[R66] 定时任务
来源：http://www.blog.sjlbkw.cn/Article/details/ghzxywtyh.sHtML

crontab -e;  crontab -l
来源：http://m.share.yfazqb.com/Article/details/gesdxicml.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.tarul.cn/Article/details/gyhvtkofq.sHtML

openssl rand -hex 16
来源：http://www.m.share.vehdjk.com/Article/details/gwxpdqmwb.sHtML

[R68] 计算文件校验值
来源：http://baike.tarul.cn/Article/details/gyvjsedyu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.sjlbkw.cn/Article/details/gplagpoem.sHtML

[R69] 生成随机密码
来源：http://blog.vehdjk.com/Article/details/grlefvxii.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.vehdjk.com/Article/details/gdhzjvgvg.sHtML

[R70] 时间戳与互转
来源：http://3g.fktsv.cn/Article/details/gtkkrlnza.sHtML

date +%s;  date -d @1700000000
来源：http://3g.vehdjk.com/Article/details/gawyceucv.sHtML

[R71] 日期格式化
来源：http://read.share.epnwcf.com/Article/details/gxiulduaf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.epnwcf.com/Article/details/geyexqjjd.sHtML

[R72] 等待端口就绪
来源：http://read.share.epnwcf.com/Article/details/gbzuuhytb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.epnwcf.com/Article/details/gjbcpxclx.sHtML

[R73] 分割大日志
来源：http://www.m.share.vehdjk.com/Article/details/gvfaoaxen.sHtML

split -l 1000 big.log part_
来源：http://www.share.sjlbkw.cn/Article/details/gbbywnbtr.sHtML

[R74] 批量重命名
来源：http://mobile.tarul.cn/Article/details/gblkgovvk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.vehdjk.com/Article/details/gwervsaov.sHtML

[R75] 导出环境变量
来源：http://www.blog.vehdjk.com/Article/details/glqoizdeo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.sjlbkw.cn/Article/details/gjbshwepm.sHtML

[R76] 使用临时文件
来源：http://baike.vehdjk.com/Article/details/gcjxymyqj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.yfazqb.com/Article/details/gavvryzgu.sHtML

[R77] 读取用户输入
来源：http://wap.vehdjk.com/Article/details/gfkwiapfa.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.tarul.cn/Article/details/geosbxlsu.sHtML

[R78] 交互式菜单
来源：http://www.blog.sjlbkw.cn/Article/details/ghwfytmqp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.tarul.cn/Article/details/gpgjsbqyz.sHtML

[R79] 解析命令行选项
来源：http://3g.epnwcf.com/Article/details/gvahwmdsv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.yfazqb.com/Article/details/grnbqaduo.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.epnwcf.com/Article/details/grcxhycmf.sHtML

time ./run.sh
来源：http://wap.vehdjk.com/Article/details/gxclpecmf.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gprfandpe.sHtML

S. C / C++ 专题
来源：http://blog.bbcook.cn/Article/details/gfidfjemx.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gboxcdsel.sHtML

[S01] C：Hello World
来源：http://3g.yfazqb.com/Article/details/gbwocogss.sHtML

#include <stdio.h>
来源：http://baike.tarul.cn/Article/details/gagwwfguy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.bbcook.cn/Article/details/gderfzrao.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.epnwcf.com/Article/details/gvyqdjgxz.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.sjlbkw.cn/Article/details/gfyvrtobn.sHtML

[S03] C：读入整数
来源：http://baike.yfazqb.com/Article/details/gpowekvus.sHtML

int x; scanf("%d", &x);
来源：http://baike.vehdjk.com/Article/details/gqhbplgur.sHtML

[S04] C：字符串复制
来源：http://wap.vehdjk.com/Article/details/gadpzpspi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.tarul.cn/Article/details/gqjhymvrm.sHtML

[S05] C：字符串长度
来源：http://3g.bbcook.cn/Article/details/ghflvoabd.sHtML

strlen(s)
来源：http://m.share.epnwcf.com/Article/details/gisaeqehl.sHtML

[S06] C：字符串比较
来源：http://www.m.share.epnwcf.com/Article/details/gfpymswyw.sHtML

strcmp(a, b) == 0
来源：http://m.share.vehdjk.com/Article/details/gvtazpwvf.sHtML

[S07] C：数组遍历求和
来源：http://wap.tarul.cn/Article/details/gkthznsep.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fktsv.cn/Article/details/gfmwpyppy.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.bbcook.cn/Article/details/gwmustywz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.epnwcf.com/Article/details/gygcjiqei.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.tarul.cn/Article/details/gdycldxad.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.vehdjk.com/Article/details/gbhhgvutf.sHtML

[S10] C：指针与解引用
来源：http://www.blog.yfazqb.com/Article/details/gkstlgail.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.sjlbkw.cn/Article/details/gqiglidlg.sHtML

[S11] C：逐行读文件
来源：http://3g.tarul.cn/Article/details/gfivhoght.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.epnwcf.com/Article/details/gpalczgzn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.vehdjk.com/Article/details/geahfgkad.sHtML

fclose(f);
来源：http://read.share.epnwcf.com/Article/details/gdmzpkudw.sHtML

[S12] C：写文件
来源：http://m.share.tarul.cn/Article/details/glhpjolow.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.yfazqb.com/Article/details/gzmmypadf.sHtML

[S13] C：宏定义
来源：http://www.share.yfazqb.com/Article/details/gwbksggfr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fktsv.cn/Article/details/gbgsljefd.sHtML

[S14] C：枚举
来源：http://m.share.yfazqb.com/Article/details/gnamhcpye.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.tarul.cn/Article/details/grgewoflb.sHtML

[S15] C：类型转换
来源：http://www.share.bbcook.cn/Article/details/gubclngwm.sHtML

(double) a / b
来源：http://read.share.vehdjk.com/Article/details/gahbioyoh.sHtML

[S16] C：位操作置位
来源：http://read.share.bbcook.cn/Article/details/gylghoxmz.sHtML

x |= (1 << 3);
来源：http://mobile.vehdjk.com/Article/details/gvcdxpkih.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fktsv.cn/Article/details/gmevvrudu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.epnwcf.com/Article/details/goeurltlz.sHtML

[S18] C：命令行参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gdizxwoce.sHtML

int main(int argc, char **argv)
来源：http://read.share.tarul.cn/Article/details/gbdnajbva.sHtML

[S19] C：快速排序
来源：http://mobile.vehdjk.com/Article/details/gnwzippbr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.yfazqb.com/Article/details/geynylsog.sHtML

[S20] C：二分查找
来源：http://read.share.fktsv.cn/Article/details/ghehurvwe.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.tarul.cn/Article/details/gbfdyycee.sHtML

[S21] C：字符类别判断
来源：http://baike.tarul.cn/Article/details/gwafmisss.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fktsv.cn/Article/details/gdckgwsij.sHtML

[S22] C：字符串转数字
来源：http://www.blog.tarul.cn/Article/details/gbtiveyqx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fktsv.cn/Article/details/gjridzrft.sHtML

[S23] C：随机数
来源：http://3g.vehdjk.com/Article/details/gqhqogwme.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.epnwcf.com/Article/details/gvavzpbtt.sHtML

[S24] C：获取本地时间
来源：http://baike.bbcook.cn/Article/details/gpqnotvxr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.sjlbkw.cn/Article/details/gmxcltixs.sHtML

[S25] C：内存拷贝
来源：http://baike.epnwcf.com/Article/details/gestixcfx.sHtML

memcpy(dst, src, n);
来源：http://www.share.tarul.cn/Article/details/gdrpmmldc.sHtML

[S26] C：内存清零
来源：http://m.share.vehdjk.com/Article/details/gskzzaexn.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.bbcook.cn/Article/details/gicrxiznw.sHtML

[S27] C：定义常量
来源：http://read.share.bbcook.cn/Article/details/gewpekaxl.sHtML

const double PI = 3.14159;
来源：http://3g.epnwcf.com/Article/details/gggrejhwa.sHtML

[S28] C：静态变量
来源：http://blog.fktsv.cn/Article/details/gxootfuaz.sHtML

static int counter = 0;
来源：http://3g.tarul.cn/Article/details/gvnmjruuk.sHtML

[S29] C：变参函数
来源：http://www.blog.tarul.cn/Article/details/gqgfcjljt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.tarul.cn/Article/details/gtprcritb.sHtML

[S30] C：头文件保护
来源：http://blog.epnwcf.com/Article/details/gpkbofpmr.sHtML

#ifndef X_H
来源：http://mobile.fktsv.cn/Article/details/gmgjuhgey.sHtML

#define X_H
来源：http://www.share.fktsv.cn/Article/details/gajknoapn.sHtML

#endif
来源：http://wap.epnwcf.com/Article/details/gcqlrfrax.sHtML

[S31] C++：Hello World
来源：http://wap.sjlbkw.cn/Article/details/gwydrympy.sHtML

#include <iostream>
来源：http://read.share.sjlbkw.cn/Article/details/gedhwzogw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.bbcook.cn/Article/details/glfctazbe.sHtML

[S32] C++：字符串
来源：http://baike.fktsv.cn/Article/details/gwgnudpoi.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.tarul.cn/Article/details/gxpbnqbjs.sHtML

[S33] C++：vector 增删
来源：http://3g.bbcook.cn/Article/details/gozvntheg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.vehdjk.com/Article/details/glsbywlih.sHtML

[S34] C++：遍历 vector
来源：http://baike.tarul.cn/Article/details/gueerhngc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.bbcook.cn/Article/details/gynrtklvq.sHtML

[S35] C++：map
来源：http://wap.yfazqb.com/Article/details/grbhjntuf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.bbcook.cn/Article/details/gtbvmcpua.sHtML

[S36] C++：unordered_map
来源：http://wap.yfazqb.com/Article/details/gfwjbweuk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.yfazqb.com/Article/details/gzbjylnxl.sHtML

[S37] C++：set
来源：http://mobile.yfazqb.com/Article/details/gzbiokhel.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.tarul.cn/Article/details/gfirtmrvh.sHtML

[S38] C++：排序
来源：http://m.share.yfazqb.com/Article/details/gopsuhxqi.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.sjlbkw.cn/Article/details/ghbcqxqex.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.bbcook.cn/Article/details/growjjzdy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.bbcook.cn/Article/details/gelvuvxjz.sHtML

[S40] C++：查找元素
来源：http://blog.vehdjk.com/Article/details/gzxcegjpn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.epnwcf.com/Article/details/gygpxdxkv.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.tarul.cn/Article/details/gfzltgehw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.sjlbkw.cn/Article/details/gteimymtl.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.vehdjk.com/Article/details/grwqaqbre.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fktsv.cn/Article/details/grqqgvrnr.sHtML

[S43] C++：智能指针
来源：http://www.blog.sjlbkw.cn/Article/details/goynfkxst.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.yfazqb.com/Article/details/gqwvscxtq.sHtML

[S44] C++：引用传参
来源：http://m.share.epnwcf.com/Article/details/gvbtwylqn.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.yfazqb.com/Article/details/ggyfivodn.sHtML

[S45] C++：lambda
来源：http://www.share.fktsv.cn/Article/details/geonphajo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.yfazqb.com/Article/details/gydmdwowt.sHtML

[S46] C++：函数模板
来源：http://read.share.epnwcf.com/Article/details/gakuakjdk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fktsv.cn/Article/details/gpxzslxjy.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.yfazqb.com/Article/details/gbcrrfuoc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.epnwcf.com/Article/details/glnmscjug.sHtML

[S48] C++：逐行读文件
来源：http://wap.sjlbkw.cn/Article/details/ggjeyjkey.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fktsv.cn/Article/details/gadfvbhpq.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.epnwcf.com/Article/details/gtkyciwdm.sHtML

[S49] C++：写文件
来源：http://read.share.sjlbkw.cn/Article/details/gmyixgacp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.vehdjk.com/Article/details/goscjttlx.sHtML

[S50] C++：格式化数字
来源：http://m.share.vehdjk.com/Article/details/guebksdhq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.bbcook.cn/Article/details/grahiyrkg.sHtML

[S51] C++：显式类型转换
来源：http://mobile.vehdjk.com/Article/details/gsxzjumpm.sHtML

static_cast<double>(a) / b
来源：http://m.share.tarul.cn/Article/details/gapcxntmd.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.sjlbkw.cn/Article/details/gyriswjyq.sHtML

int size() const noexcept { return n_; }
来源：http://wap.tarul.cn/Article/details/gqniuzlmk.sHtML

[S53] C++：移动语义
来源：http://mobile.fktsv.cn/Article/details/grbfzzrgs.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.bbcook.cn/Article/details/gvqkhaaqn.sHtML

[S54] C++：异常处理
来源：http://mobile.vehdjk.com/Article/details/gmokplzkw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.epnwcf.com/Article/details/gfeznqzeh.sHtML

[S55] C++：结构化绑定
来源：http://mobile.bbcook.cn/Article/details/glsvtvaid.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.bbcook.cn/Article/details/glzgmaqms.sHtML

[S56] C++：optional
来源：http://wap.sjlbkw.cn/Article/details/gderqcszm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.vehdjk.com/Article/details/gfsmfwpdk.sHtML

[S57] C++：编译期常量
来源：http://www.blog.vehdjk.com/Article/details/gkikjrcbd.sHtML

constexpr int N = 10;
来源：http://3g.vehdjk.com/Article/details/gerjlogzu.sHtML

[S58] C++：命名空间
来源：http://www.share.bbcook.cn/Article/details/gmucehasi.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.yfazqb.com/Article/details/gtddxilzw.sHtML

[S59] C++：静态断言
来源：http://www.share.epnwcf.com/Article/details/gkoldsygy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.sjlbkw.cn/Article/details/gazzoijib.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.bbcook.cn/Article/details/gakrdmdmp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.vehdjk.com/Article/details/glkyqomwo.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/guwqyozij.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fktsv.cn/Article/details/gbsxjhqir.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/guqhkeboh.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.yfazqb.com/Article/details/gqmabpydi.sHtML

println("Hello")
来源：http://blog.fktsv.cn/Article/details/guqhrhjkn.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fktsv.cn/Article/details/gdujjcsox.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.bbcook.cn/Article/details/gmbiefzwc.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fktsv.cn/Article/details/gfzzcxdem.sHtML

"值: $b"
来源：http://read.share.yfazqb.com/Article/details/gxgxzdksi.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.vehdjk.com/Article/details/gfwbfbevd.sHtML

val n: String? = null;  n?.length
来源：http://m.share.sjlbkw.cn/Article/details/gvazkxwmg.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fktsv.cn/Article/details/gnyolqick.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fktsv.cn/Article/details/gwkqbdvue.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.epnwcf.com/Article/details/ggtpjradk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.epnwcf.com/Article/details/ghsmjreld.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.tarul.cn/Article/details/gvbgqutsd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.yfazqb.com/Article/details/gnvqvmzub.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fktsv.cn/Article/details/gshgosmwm.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.yfazqb.com/Article/details/gtswvsbjt.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.vehdjk.com/Article/details/gssoocqmm.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.yfazqb.com/Article/details/gyubhjwax.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.epnwcf.com/Article/details/gtnnemxim.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.bbcook.cn/Article/details/gztprslfb.sHtML

[T11] Kotlin：协程
来源：http://3g.tarul.cn/Article/details/gsmakxazl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.sjlbkw.cn/Article/details/gqdrbeuun.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.tarul.cn/Article/details/gpdcahlqq.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.yfazqb.com/Article/details/gbsuvpkbr.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.yfazqb.com/Article/details/guxjufahe.sHtML

val m = mapOf("a" to 1)
来源：http://blog.yfazqb.com/Article/details/glszngesr.sHtML

[T14] Kotlin：循环
来源：http://m.share.sjlbkw.cn/Article/details/gzbbixfwf.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.epnwcf.com/Article/details/guytqpnxf.sHtML

[T15] Kotlin：接口
来源：http://www.blog.sjlbkw.cn/Article/details/gieccqjsu.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.yfazqb.com/Article/details/gokdespkx.sHtML

[T16] Swift：Hello World
来源：http://blog.fktsv.cn/Article/details/gcrrmslfy.sHtML

print("Hello")
来源：http://baike.fktsv.cn/Article/details/gtvwwlgyn.sHtML

[T17] Swift：变量与常量
来源：http://mobile.vehdjk.com/Article/details/gnmqhjqwg.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fktsv.cn/Article/details/gtyzdjwzx.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.epnwcf.com/Article/details/gsyxnwlmx.sHtML

"值: \(b)"
来源：http://3g.yfazqb.com/Article/details/gegqstuic.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.sjlbkw.cn/Article/details/gknmfazqx.sHtML

if let n = opt { print(n) }
来源：http://www.share.epnwcf.com/Article/details/gvjecojkr.sHtML

[T20] Swift：数组操作
来源：http://3g.tarul.cn/Article/details/ggrufatmz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.vehdjk.com/Article/details/giexdclqn.sHtML

[T21] Swift：遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gqetsllbn.sHtML

for x in a { print(x) }
来源：http://blog.sjlbkw.cn/Article/details/gfygemaeg.sHtML

[T22] Swift：字典
来源：http://baike.bbcook.cn/Article/details/gpqvoxwpr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.vehdjk.com/Article/details/gawtjfwmy.sHtML

[T23] Swift：函数
来源：http://blog.yfazqb.com/Article/details/gonluwfmw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.vehdjk.com/Article/details/gtkdheoyd.sHtML

[T24] Swift：闭包
来源：http://wap.yfazqb.com/Article/details/gexhhwtnt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.tarul.cn/Article/details/ghzeagejw.sHtML

[T25] Swift：结构体
来源：http://mobile.fktsv.cn/Article/details/ghszwohwa.sHtML

struct P { var x: Int }
来源：http://3g.vehdjk.com/Article/details/glzcnwymk.sHtML

[T26] Swift：类与重写
来源：http://m.share.yfazqb.com/Article/details/gddmlkpkx.sHtML

class A: Base { override func f() {} }
来源：http://mobile.sjlbkw.cn/Article/details/gflizufnx.sHtML

[T27] Swift：错误处理
来源：http://www.blog.sjlbkw.cn/Article/details/gmkssijll.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.bbcook.cn/Article/details/gldegjief.sHtML

[T28] Swift：枚举
来源：http://wap.tarul.cn/Article/details/gnuvcciol.sHtML

enum Color { case red, green }
来源：http://www.m.share.sjlbkw.cn/Article/details/gowlxykhs.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.bbcook.cn/Article/details/gbigkeayv.sHtML

guard let x = opt else { return }
来源：http://www.m.share.tarul.cn/Article/details/gtsotifqg.sHtML

[T30] Swift：协议
来源：http://blog.epnwcf.com/Article/details/gsxciclnl.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fktsv.cn/Article/details/gghcirjka.sHtML

[T31] Lua：Hello World
来源：http://www.share.fktsv.cn/Article/details/guqpyibzp.sHtML

print("Hello")
来源：http://blog.bbcook.cn/Article/details/gyiyjugux.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fktsv.cn/Article/details/geifbmxwx.sHtML

local a = 1
来源：http://baike.yfazqb.com/Article/details/gfxjwrmmo.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.vehdjk.com/Article/details/gulnlozen.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fktsv.cn/Article/details/gasikivuw.sHtML

[T34] Lua：遍历表
来源：http://read.share.bbcook.cn/Article/details/gpwlwuekt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fktsv.cn/Article/details/gwjbyiely.sHtML

[T35] Lua：字典表
来源：http://mobile.tarul.cn/Article/details/gxoguqtnx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.epnwcf.com/Article/details/gegyjjjof.sHtML

[T36] Lua：函数
来源：http://m.share.sjlbkw.cn/Article/details/gsvbiqvmz.sHtML

function add(a, b) return a + b end
来源：http://3g.vehdjk.com/Article/details/gnnlniold.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.sjlbkw.cn/Article/details/gkukpgqhk.sHtML

"a" .. "b"
来源：http://blog.vehdjk.com/Article/details/gjjpvuxvw.sHtML

[T38] Lua：条件
来源：http://baike.epnwcf.com/Article/details/gpaknyrtl.sHtML

if x > 0 then print("正") end
来源：http://3g.vehdjk.com/Article/details/glctleyjj.sHtML

[T39] Lua：模式匹配
来源：http://wap.bbcook.cn/Article/details/gataupzpj.sHtML

string.find(s, "%d+")
来源：http://www.blog.sjlbkw.cn/Article/details/ggiimdcos.sHtML

[T40] Lua：元表
来源：http://m.share.yfazqb.com/Article/details/gsuckxmxb.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.epnwcf.com/Article/details/gmlsqyarj.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.yfazqb.com/Article/details/gjummqauh.sHtML

print "Hello\n";
来源：http://www.blog.tarul.cn/Article/details/gxfbwwiti.sHtML

[T42] Perl：变量类型
来源：http://m.share.fktsv.cn/Article/details/gojryxbaa.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.epnwcf.com/Article/details/gfsdhhofo.sHtML

[T43] Perl：字符串插值
来源：http://3g.sjlbkw.cn/Article/details/guagynmkg.sHtML

"值: $a"
来源：http://read.share.yfazqb.com/Article/details/gpckytpgd.sHtML

[T44] Perl：条件
来源：http://baike.sjlbkw.cn/Article/details/ghizuzjhi.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdrwgtfrk.sHtML


<!-- 参考信息 -->