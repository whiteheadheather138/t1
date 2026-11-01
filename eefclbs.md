代发 wailian999

cmd > out.log 2>&1
来源：http://www.share.bbcook.cn/Article/details/gokqufcgx.sHtML

[R40] 追加写日志
来源：http://www.m.share.bbcook.cn/Article/details/gjhjohcgh.sHtML

echo "log" >> out.log
来源：http://3g.bbcook.cn/Article/details/grjudnmxl.sHtML

[R41] 丢弃输出
来源：http://mobile.bbcook.cn/Article/details/gknzqqsjp.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fktsv.cn/Article/details/gdkbhmpeq.sHtML

[R42] 输入重定向
来源：http://www.share.epnwcf.com/Article/details/gtffhupby.sHtML

wc -l < a.txt
来源：http://www.m.share.yfazqb.com/Article/details/ggjxxbrbk.sHtML

[R43] 按名字查找文件
来源：http://www.share.tarul.cn/Article/details/gmfdzwnyu.sHtML

find . -name "*.log" -type f
来源：http://baike.sjlbkw.cn/Article/details/gzpodditn.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.epnwcf.com/Article/details/glrviogsu.sHtML

find . -mtime -7 -type f
来源：http://www.share.bbcook.cn/Article/details/gryuyepxy.sHtML

[R45] 批量删除
来源：http://www.m.share.vehdjk.com/Article/details/ghqidmnis.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.yfazqb.com/Article/details/gyldpmqlk.sHtML

[R46] 递归替换文件内容
来源：http://read.share.yfazqb.com/Article/details/gkyxlxgwb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.epnwcf.com/Article/details/glynggttw.sHtML

[R47] sed 单行替换
来源：http://read.share.bbcook.cn/Article/details/gljkakfda.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.tarul.cn/Article/details/gtfmdgewv.sHtML

[R48] awk 取指定列
来源：http://m.share.tarul.cn/Article/details/gjzgudavk.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.vehdjk.com/Article/details/gvvrxsmir.sHtML

[R49] awk 带条件
来源：http://m.share.epnwcf.com/Article/details/ghoigacrz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.tarul.cn/Article/details/gmcikigpw.sHtML

[R50] awk 求和
来源：http://mobile.epnwcf.com/Article/details/gcyspiznt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.epnwcf.com/Article/details/gtzzkstyy.sHtML

[R51] 排序去重取前几
来源：http://mobile.yfazqb.com/Article/details/gzypknitg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.tarul.cn/Article/details/gbxgupxyr.sHtML

[R52] 统计行数
来源：http://www.blog.bbcook.cn/Article/details/gkzjdwyqf.sHtML

wc -l a.txt
来源：http://baike.epnwcf.com/Article/details/giwhpwfjx.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.yfazqb.com/Article/details/gapuysima.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.yfazqb.com/Article/details/gvrwndmyj.sHtML

[R54] 比较两个文件
来源：http://www.m.share.vehdjk.com/Article/details/gusityldb.sHtML

diff a.txt b.txt
来源：http://blog.vehdjk.com/Article/details/ghpaesghm.sHtML

[R55] 压缩与解压
来源：http://read.share.bbcook.cn/Article/details/glzjakbnd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.vehdjk.com/Article/details/gixbaapbx.sHtML

[R56] 远程拷贝
来源：http://www.m.share.tarul.cn/Article/details/gjxhtzprv.sHtML

scp file user@host:/path/
来源：http://mobile.tarul.cn/Article/details/gohailvjs.sHtML

[R57] 远程执行命令
来源：http://www.share.yfazqb.com/Article/details/gjrpwaqoz.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.yfazqb.com/Article/details/gufevbhzy.sHtML

[R58] 下载文件
来源：http://blog.vehdjk.com/Article/details/gkwswtaol.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.tarul.cn/Article/details/gayzxhmen.sHtML

[R59] 发 POST JSON
来源：http://www.blog.bbcook.cn/Article/details/gksnggnyz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.epnwcf.com/Article/details/gzytjtexa.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.sjlbkw.cn/Article/details/gwyvfassr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fktsv.cn/Article/details/gswrgmdkd.sHtML

[R61] 磁盘占用
来源：http://www.blog.sjlbkw.cn/Article/details/gvlnvahck.sHtML

df -h;  du -sh *
来源：http://mobile.tarul.cn/Article/details/glelnifzr.sHtML

[R62] 找最占空间的文件
来源：http://m.share.tarul.cn/Article/details/gnabmvjpa.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.epnwcf.com/Article/details/geeavrpin.sHtML

[R63] 内存与进程
来源：http://baike.epnwcf.com/Article/details/ginyyasqt.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.vehdjk.com/Article/details/gppuilqge.sHtML

[R64] 结束进程
来源：http://baike.fktsv.cn/Article/details/gqfgcramc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.sjlbkw.cn/Article/details/gfmfwyquw.sHtML

[R65] 查看端口占用
来源：http://mobile.yfazqb.com/Article/details/guvtydlyg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.vehdjk.com/Article/details/gwdxjzqpi.sHtML

[R66] 定时任务
来源：http://www.share.vehdjk.com/Article/details/gcanhyzoq.sHtML

crontab -e;  crontab -l
来源：http://baike.epnwcf.com/Article/details/gamcnuuxm.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fktsv.cn/Article/details/gvstsazun.sHtML

openssl rand -hex 16
来源：http://www.blog.tarul.cn/Article/details/ghgvvaosx.sHtML

[R68] 计算文件校验值
来源：http://3g.sjlbkw.cn/Article/details/glljnilyn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.yfazqb.com/Article/details/ghbwwxoxl.sHtML

[R69] 生成随机密码
来源：http://www.blog.tarul.cn/Article/details/gwkehouap.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.epnwcf.com/Article/details/gceoyshno.sHtML

[R70] 时间戳与互转
来源：http://3g.yfazqb.com/Article/details/gthetvvvb.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.yfazqb.com/Article/details/gqeibumge.sHtML

[R71] 日期格式化
来源：http://mobile.bbcook.cn/Article/details/gjicqompn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.tarul.cn/Article/details/gzdyvullg.sHtML

[R72] 等待端口就绪
来源：http://m.share.fktsv.cn/Article/details/gzehotdam.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fktsv.cn/Article/details/gzcfyqive.sHtML

[R73] 分割大日志
来源：http://www.share.tarul.cn/Article/details/grlqzijhc.sHtML

split -l 1000 big.log part_
来源：http://3g.epnwcf.com/Article/details/gkabkwwcj.sHtML

[R74] 批量重命名
来源：http://www.blog.epnwcf.com/Article/details/gnrodomxj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.bbcook.cn/Article/details/gxyvaycwa.sHtML

[R75] 导出环境变量
来源：http://mobile.bbcook.cn/Article/details/gyjoyjwcg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.sjlbkw.cn/Article/details/gctohovcf.sHtML

[R76] 使用临时文件
来源：http://www.blog.epnwcf.com/Article/details/gabhydpoh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.epnwcf.com/Article/details/gpqnhoqou.sHtML

[R77] 读取用户输入
来源：http://wap.sjlbkw.cn/Article/details/grhizfywn.sHtML

read -rp "请输入: " ans
来源：http://m.share.tarul.cn/Article/details/gjverpkti.sHtML

[R78] 交互式菜单
来源：http://wap.fktsv.cn/Article/details/glenqrwye.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.vehdjk.com/Article/details/grgphozsk.sHtML

[R79] 解析命令行选项
来源：http://mobile.sjlbkw.cn/Article/details/gpxekhncm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.tarul.cn/Article/details/gplvkhtnv.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.bbcook.cn/Article/details/gvrtfmzaj.sHtML

time ./run.sh
来源：http://www.blog.fktsv.cn/Article/details/gosshgmik.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gzuknsdrh.sHtML

S. C / C++ 专题
来源：http://www.share.yfazqb.com/Article/details/gfkihjocq.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gaeobogem.sHtML

[S01] C：Hello World
来源：http://m.share.tarul.cn/Article/details/ghybktlfv.sHtML

#include <stdio.h>
来源：http://mobile.sjlbkw.cn/Article/details/gsabocpkj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.tarul.cn/Article/details/gyxyzidvk.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fktsv.cn/Article/details/gvkgpeprc.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.tarul.cn/Article/details/gxamvzssi.sHtML

[S03] C：读入整数
来源：http://blog.epnwcf.com/Article/details/gmyqicvjv.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.tarul.cn/Article/details/gtsaxdstm.sHtML

[S04] C：字符串复制
来源：http://mobile.tarul.cn/Article/details/giwotdnlt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.vehdjk.com/Article/details/gfpptwpcu.sHtML

[S05] C：字符串长度
来源：http://www.share.vehdjk.com/Article/details/gtjmbnptc.sHtML

strlen(s)
来源：http://www.m.share.tarul.cn/Article/details/ghqgbcdgd.sHtML

[S06] C：字符串比较
来源：http://blog.sjlbkw.cn/Article/details/gjqbapvrb.sHtML

strcmp(a, b) == 0
来源：http://www.blog.sjlbkw.cn/Article/details/gdmtiwzqk.sHtML

[S07] C：数组遍历求和
来源：http://baike.yfazqb.com/Article/details/gfqjcwtxn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fktsv.cn/Article/details/gokzrwsga.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.yfazqb.com/Article/details/gatrmcgvv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.epnwcf.com/Article/details/gdtkkdicw.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fktsv.cn/Article/details/glqdaenwp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fktsv.cn/Article/details/gtrzptvvt.sHtML

[S10] C：指针与解引用
来源：http://mobile.vehdjk.com/Article/details/gvdsophed.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.tarul.cn/Article/details/gictgvavf.sHtML

[S11] C：逐行读文件
来源：http://blog.tarul.cn/Article/details/glpyyxoyp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fktsv.cn/Article/details/gvpshzpjp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fktsv.cn/Article/details/gbtbgegxp.sHtML

fclose(f);
来源：http://blog.epnwcf.com/Article/details/ggewkbosd.sHtML

[S12] C：写文件
来源：http://www.share.bbcook.cn/Article/details/gmgeeylak.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.vehdjk.com/Article/details/gfrkoagvw.sHtML

[S13] C：宏定义
来源：http://read.share.sjlbkw.cn/Article/details/gvufmawfi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.bbcook.cn/Article/details/ggrpvmnwk.sHtML

[S14] C：枚举
来源：http://www.share.fktsv.cn/Article/details/gdhtamlzp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.epnwcf.com/Article/details/gqlfchdik.sHtML

[S15] C：类型转换
来源：http://www.share.fktsv.cn/Article/details/glpzwdvkw.sHtML

(double) a / b
来源：http://baike.bbcook.cn/Article/details/gsmipxfkh.sHtML

[S16] C：位操作置位
来源：http://3g.fktsv.cn/Article/details/ghwyottfv.sHtML

x |= (1 << 3);
来源：http://3g.sjlbkw.cn/Article/details/gslrpinqc.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.sjlbkw.cn/Article/details/gepsoccrl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.bbcook.cn/Article/details/gziillgmd.sHtML

[S18] C：命令行参数
来源：http://www.share.fktsv.cn/Article/details/gamsquwmo.sHtML

int main(int argc, char **argv)
来源：http://baike.fktsv.cn/Article/details/grtscohcj.sHtML

[S19] C：快速排序
来源：http://www.share.epnwcf.com/Article/details/gsoeqanja.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.vehdjk.com/Article/details/ggvyzwzzk.sHtML

[S20] C：二分查找
来源：http://www.m.share.bbcook.cn/Article/details/gixltevtf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.epnwcf.com/Article/details/gmaxzqqnn.sHtML

[S21] C：字符类别判断
来源：http://wap.bbcook.cn/Article/details/giycjqryi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.yfazqb.com/Article/details/glnhzxakk.sHtML

[S22] C：字符串转数字
来源：http://mobile.epnwcf.com/Article/details/gaootlshz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.yfazqb.com/Article/details/glybeyitp.sHtML

[S23] C：随机数
来源：http://www.share.epnwcf.com/Article/details/gjhgbmqvz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.tarul.cn/Article/details/grkvtmfjc.sHtML

[S24] C：获取本地时间
来源：http://www.blog.sjlbkw.cn/Article/details/ghhqgvyxs.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.sjlbkw.cn/Article/details/gcsaeiasl.sHtML

[S25] C：内存拷贝
来源：http://blog.sjlbkw.cn/Article/details/gmmpjqnnc.sHtML

memcpy(dst, src, n);
来源：http://www.share.epnwcf.com/Article/details/gcbhvthkc.sHtML

[S26] C：内存清零
来源：http://3g.epnwcf.com/Article/details/gbesuvgyb.sHtML

memset(a, 0, sizeof a);
来源：http://baike.bbcook.cn/Article/details/ghwlbqlyn.sHtML

[S27] C：定义常量
来源：http://www.blog.tarul.cn/Article/details/gveefyfqp.sHtML

const double PI = 3.14159;
来源：http://3g.fktsv.cn/Article/details/gapdyyzxr.sHtML

[S28] C：静态变量
来源：http://3g.bbcook.cn/Article/details/gswqftrno.sHtML

static int counter = 0;
来源：http://baike.vehdjk.com/Article/details/gbhqurhiz.sHtML

[S29] C：变参函数
来源：http://wap.vehdjk.com/Article/details/gqnbirhss.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.sjlbkw.cn/Article/details/gndyunbzu.sHtML

[S30] C：头文件保护
来源：http://blog.yfazqb.com/Article/details/gscbbqscx.sHtML

#ifndef X_H
来源：http://blog.yfazqb.com/Article/details/gqgxiripc.sHtML

#define X_H
来源：http://3g.epnwcf.com/Article/details/ghlwmoftz.sHtML

#endif
来源：http://mobile.bbcook.cn/Article/details/gxlkkmspb.sHtML

[S31] C++：Hello World
来源：http://www.blog.epnwcf.com/Article/details/goccccbpf.sHtML

#include <iostream>
来源：http://mobile.bbcook.cn/Article/details/gwfwxthra.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.vehdjk.com/Article/details/gtzjehvpt.sHtML

[S32] C++：字符串
来源：http://baike.vehdjk.com/Article/details/gvxfgfsah.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.bbcook.cn/Article/details/ggtbycqxz.sHtML

[S33] C++：vector 增删
来源：http://mobile.bbcook.cn/Article/details/gkzhiggfa.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.sjlbkw.cn/Article/details/geiqwdizd.sHtML

[S34] C++：遍历 vector
来源：http://wap.yfazqb.com/Article/details/gsfcuuyvl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.epnwcf.com/Article/details/gcwqtcbjs.sHtML

[S35] C++：map
来源：http://www.blog.sjlbkw.cn/Article/details/gbbcbrsor.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.epnwcf.com/Article/details/gyhlosryx.sHtML

[S36] C++：unordered_map
来源：http://blog.yfazqb.com/Article/details/gwkutwhxq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.epnwcf.com/Article/details/gclfxlcte.sHtML

[S37] C++：set
来源：http://mobile.tarul.cn/Article/details/gjuphqqeg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.sjlbkw.cn/Article/details/gupyswbcn.sHtML

[S38] C++：排序
来源：http://wap.vehdjk.com/Article/details/gtijrfyap.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.yfazqb.com/Article/details/gzvgccxnr.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.bbcook.cn/Article/details/grsqaurkp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.sjlbkw.cn/Article/details/gufkpgjxx.sHtML

[S40] C++：查找元素
来源：http://wap.vehdjk.com/Article/details/gqbpamrfk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.bbcook.cn/Article/details/gjxinyumj.sHtML

[S41] C++：类与构造函数
来源：http://www.share.bbcook.cn/Article/details/gingemxqr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.bbcook.cn/Article/details/gjntrhihj.sHtML

[S42] C++：继承与虚函数
来源：http://3g.yfazqb.com/Article/details/glgqtfwte.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.yfazqb.com/Article/details/gfitscelc.sHtML

[S43] C++：智能指针
来源：http://www.m.share.sjlbkw.cn/Article/details/gcmqpmbdk.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.bbcook.cn/Article/details/gofvjkcoy.sHtML

[S44] C++：引用传参
来源：http://m.share.fktsv.cn/Article/details/gsdsuwrjw.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.vehdjk.com/Article/details/gakgjuvrb.sHtML

[S45] C++：lambda
来源：http://www.blog.tarul.cn/Article/details/gvvprasgy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.epnwcf.com/Article/details/gsmqxvfwe.sHtML

[S46] C++：函数模板
来源：http://www.share.epnwcf.com/Article/details/ghksnuzdu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.yfazqb.com/Article/details/ggsdgoreh.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.bbcook.cn/Article/details/gmrwevmdx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.yfazqb.com/Article/details/glwbnwgzx.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.yfazqb.com/Article/details/gsinxjbpn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.epnwcf.com/Article/details/gruilpviz.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.vehdjk.com/Article/details/gssyrlqcv.sHtML

[S49] C++：写文件
来源：http://www.share.sjlbkw.cn/Article/details/guzaxqgzl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.tarul.cn/Article/details/gblfnwjii.sHtML

[S50] C++：格式化数字
来源：http://3g.bbcook.cn/Article/details/gjkocvgjf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.tarul.cn/Article/details/gaagxrfuv.sHtML

[S51] C++：显式类型转换
来源：http://mobile.epnwcf.com/Article/details/gtmoaslfp.sHtML

static_cast<double>(a) / b
来源：http://www.share.tarul.cn/Article/details/ghkouplag.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.bbcook.cn/Article/details/gcejxtdfg.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fktsv.cn/Article/details/ggzxmvenj.sHtML

[S53] C++：移动语义
来源：http://mobile.tarul.cn/Article/details/guxflbalz.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.tarul.cn/Article/details/gqjiynnov.sHtML

[S54] C++：异常处理
来源：http://mobile.sjlbkw.cn/Article/details/gauadivde.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.sjlbkw.cn/Article/details/gmtaviwac.sHtML

[S55] C++：结构化绑定
来源：http://read.share.vehdjk.com/Article/details/gdhobzdca.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.yfazqb.com/Article/details/gperhliae.sHtML

[S56] C++：optional
来源：http://3g.yfazqb.com/Article/details/guxtmswkz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.yfazqb.com/Article/details/gorubmpwg.sHtML

[S57] C++：编译期常量
来源：http://blog.sjlbkw.cn/Article/details/ghfwdtwnx.sHtML

constexpr int N = 10;
来源：http://www.blog.epnwcf.com/Article/details/gefkrrkez.sHtML

[S58] C++：命名空间
来源：http://blog.fktsv.cn/Article/details/gqmqzmnjl.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.vehdjk.com/Article/details/gsykhdvdh.sHtML

[S59] C++：静态断言
来源：http://www.share.fktsv.cn/Article/details/gumtfnhus.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.yfazqb.com/Article/details/gbyzntmlo.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.bbcook.cn/Article/details/gzlgvyldz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.yfazqb.com/Article/details/gbhsqotgz.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gzqglknnv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fktsv.cn/Article/details/gfsahcmct.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gggtwvhxf.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/gabtcqpqi.sHtML

println("Hello")
来源：http://baike.epnwcf.com/Article/details/guhxsfgeg.sHtML

[T02] Kotlin：变量
来源：http://mobile.bbcook.cn/Article/details/gyuotiufr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.sjlbkw.cn/Article/details/gtyuokjsl.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.tarul.cn/Article/details/gbhjqapvo.sHtML

"值: $b"
来源：http://www.share.yfazqb.com/Article/details/gpehmtjpc.sHtML

[T04] Kotlin：空安全
来源：http://blog.bbcook.cn/Article/details/gvgjoulqk.sHtML

val n: String? = null;  n?.length
来源：http://mobile.yfazqb.com/Article/details/gymjyjjtl.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.sjlbkw.cn/Article/details/gjdymdyds.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.tarul.cn/Article/details/gegyzngwk.sHtML

[T06] Kotlin：集合映射
来源：http://3g.yfazqb.com/Article/details/gnbpzdkxt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.vehdjk.com/Article/details/gvyyqpggq.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fktsv.cn/Article/details/gkmukwctp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.vehdjk.com/Article/details/gncboqcjz.sHtML

[T08] Kotlin：数据类
来源：http://read.share.sjlbkw.cn/Article/details/ggtxmivtx.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.sjlbkw.cn/Article/details/gzhzptapp.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.epnwcf.com/Article/details/gfjpwrcov.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.tarul.cn/Article/details/gictzihfh.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.bbcook.cn/Article/details/gzbiferok.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.epnwcf.com/Article/details/gsvfjerij.sHtML

[T11] Kotlin：协程
来源：http://read.share.tarul.cn/Article/details/gztdqqkgb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.tarul.cn/Article/details/grlxtkgwb.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.tarul.cn/Article/details/gepbrxocs.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.bbcook.cn/Article/details/gggafqhif.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.bbcook.cn/Article/details/gmlswmmbw.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.epnwcf.com/Article/details/gwiocndbe.sHtML

[T14] Kotlin：循环
来源：http://blog.yfazqb.com/Article/details/gujdcejpg.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.vehdjk.com/Article/details/gnafimoca.sHtML

[T15] Kotlin：接口
来源：http://baike.epnwcf.com/Article/details/gyzzacned.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.sjlbkw.cn/Article/details/grsozlswy.sHtML

[T16] Swift：Hello World
来源：http://wap.tarul.cn/Article/details/gyrtbapxn.sHtML

print("Hello")
来源：http://baike.epnwcf.com/Article/details/gtjqrsdki.sHtML

[T17] Swift：变量与常量
来源：http://3g.fktsv.cn/Article/details/gmwcvscsr.sHtML

var a = 1;  let b = 2
来源：http://3g.yfazqb.com/Article/details/gaxdwklbc.sHtML

[T18] Swift：字符串插值
来源：http://m.share.epnwcf.com/Article/details/gkegtzngh.sHtML

"值: \(b)"
来源：http://www.blog.fktsv.cn/Article/details/gbxxfirvf.sHtML

[T19] Swift：可选绑定
来源：http://read.share.tarul.cn/Article/details/gqojhzyhw.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.tarul.cn/Article/details/gwrfnhglo.sHtML

[T20] Swift：数组操作
来源：http://wap.tarul.cn/Article/details/gfeimuvaq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.vehdjk.com/Article/details/gplalqbcv.sHtML

[T21] Swift：遍历
来源：http://mobile.vehdjk.com/Article/details/gfxxxptii.sHtML

for x in a { print(x) }
来源：http://baike.tarul.cn/Article/details/gmvijhntz.sHtML

[T22] Swift：字典
来源：http://www.blog.sjlbkw.cn/Article/details/ggwfmmvlu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.yfazqb.com/Article/details/gsnczaxfb.sHtML

[T23] Swift：函数
来源：http://wap.yfazqb.com/Article/details/ggkxluqep.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.bbcook.cn/Article/details/gkkmsaghg.sHtML

[T24] Swift：闭包
来源：http://blog.tarul.cn/Article/details/grybzacvv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.vehdjk.com/Article/details/gfifzixzf.sHtML

[T25] Swift：结构体
来源：http://mobile.tarul.cn/Article/details/gjitrfzdh.sHtML

struct P { var x: Int }
来源：http://m.share.yfazqb.com/Article/details/gbjcpxeub.sHtML

[T26] Swift：类与重写
来源：http://read.share.vehdjk.com/Article/details/galocmbes.sHtML

class A: Base { override func f() {} }
来源：http://www.share.vehdjk.com/Article/details/gkykqniff.sHtML

[T27] Swift：错误处理
来源：http://blog.yfazqb.com/Article/details/gmiqcevrb.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.epnwcf.com/Article/details/gqminazwr.sHtML

[T28] Swift：枚举
来源：http://blog.epnwcf.com/Article/details/ghkfhuffx.sHtML

enum Color { case red, green }
来源：http://www.blog.sjlbkw.cn/Article/details/gzoeglagj.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.epnwcf.com/Article/details/gkqssvtni.sHtML

guard let x = opt else { return }
来源：http://mobile.sjlbkw.cn/Article/details/gbnfoyqkm.sHtML

[T30] Swift：协议
来源：http://3g.yfazqb.com/Article/details/gsxcddana.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.yfazqb.com/Article/details/gnymxwqio.sHtML

[T31] Lua：Hello World
来源：http://blog.epnwcf.com/Article/details/gyavyljfu.sHtML

print("Hello")
来源：http://read.share.vehdjk.com/Article/details/gtzvgoqdi.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fktsv.cn/Article/details/ganozkmmn.sHtML

local a = 1
来源：http://m.share.bbcook.cn/Article/details/gaynndyho.sHtML

[T33] Lua：表（数组）
来源：http://m.share.bbcook.cn/Article/details/gesmhcule.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.yfazqb.com/Article/details/gxfmzewof.sHtML

[T34] Lua：遍历表
来源：http://wap.sjlbkw.cn/Article/details/gsnoknrab.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.yfazqb.com/Article/details/gsluhbdii.sHtML

[T35] Lua：字典表
来源：http://read.share.fktsv.cn/Article/details/gvcxdcipl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.yfazqb.com/Article/details/gqyziaqrm.sHtML

[T36] Lua：函数
来源：http://www.blog.fktsv.cn/Article/details/gqzrynjqx.sHtML

function add(a, b) return a + b end
来源：http://read.share.vehdjk.com/Article/details/gisukqvaw.sHtML

[T37] Lua：字符串拼接
来源：http://baike.tarul.cn/Article/details/gjcwzqpel.sHtML

"a" .. "b"
来源：http://baike.tarul.cn/Article/details/gndctnyuf.sHtML

[T38] Lua：条件
来源：http://www.m.share.yfazqb.com/Article/details/gbcaydaed.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fktsv.cn/Article/details/gvzxyofsf.sHtML

[T39] Lua：模式匹配
来源：http://m.share.vehdjk.com/Article/details/gpnzmzxko.sHtML

string.find(s, "%d+")
来源：http://blog.bbcook.cn/Article/details/gqqqlhlzs.sHtML

[T40] Lua：元表
来源：http://www.blog.bbcook.cn/Article/details/gdynklbxb.sHtML

setmetatable({}, { __index = base })
来源：http://wap.vehdjk.com/Article/details/gwrthqngj.sHtML

[T41] Perl：Hello World
来源：http://read.share.bbcook.cn/Article/details/godzpfhca.sHtML

print "Hello\n";
来源：http://www.share.epnwcf.com/Article/details/gbmkpjspd.sHtML

[T42] Perl：变量类型
来源：http://mobile.bbcook.cn/Article/details/gcsxrafeu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.epnwcf.com/Article/details/gceoeugdw.sHtML


<!-- 参考信息 -->