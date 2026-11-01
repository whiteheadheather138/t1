代发 wailian999

cmd > out.log 2>&1
来源：http://blog.vehdjk.com/Article/details/grddfbdfr.sHtML

[R40] 追加写日志
来源：http://www.blog.fktsv.cn/Article/details/gyfquzuzc.sHtML

echo "log" >> out.log
来源：http://read.share.epnwcf.com/Article/details/gifixujga.sHtML

[R41] 丢弃输出
来源：http://3g.tarul.cn/Article/details/gqqnhveys.sHtML

cmd >/dev/null 2>&1
来源：http://baike.yfazqb.com/Article/details/grtgjfjlf.sHtML

[R42] 输入重定向
来源：http://www.blog.bbcook.cn/Article/details/gzfpqxiru.sHtML

wc -l < a.txt
来源：http://www.share.vehdjk.com/Article/details/ggwvcinaj.sHtML

[R43] 按名字查找文件
来源：http://baike.tarul.cn/Article/details/ghundajrk.sHtML

find . -name "*.log" -type f
来源：http://read.share.yfazqb.com/Article/details/gtmebtatm.sHtML

[R44] 按修改时间查找
来源：http://mobile.tarul.cn/Article/details/gkzhpzojb.sHtML

find . -mtime -7 -type f
来源：http://blog.fktsv.cn/Article/details/gekfftwxb.sHtML

[R45] 批量删除
来源：http://baike.vehdjk.com/Article/details/gekpvysxt.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.bbcook.cn/Article/details/grnhkbxrx.sHtML

[R46] 递归替换文件内容
来源：http://3g.epnwcf.com/Article/details/gaeufceul.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.yfazqb.com/Article/details/gyamdxxwo.sHtML

[R47] sed 单行替换
来源：http://www.share.fktsv.cn/Article/details/gfhsojcgn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.epnwcf.com/Article/details/gcntwufst.sHtML

[R48] awk 取指定列
来源：http://www.share.bbcook.cn/Article/details/gairczzcl.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.vehdjk.com/Article/details/gkqyakyun.sHtML

[R49] awk 带条件
来源：http://mobile.fktsv.cn/Article/details/geweubzve.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.bbcook.cn/Article/details/gdruicigb.sHtML

[R50] awk 求和
来源：http://wap.sjlbkw.cn/Article/details/ghknadddg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.bbcook.cn/Article/details/ghwuzbxny.sHtML

[R51] 排序去重取前几
来源：http://mobile.yfazqb.com/Article/details/gxshvlkqa.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.yfazqb.com/Article/details/glwvzynqx.sHtML

[R52] 统计行数
来源：http://read.share.epnwcf.com/Article/details/gochptqhj.sHtML

wc -l a.txt
来源：http://mobile.tarul.cn/Article/details/gfwhiedaf.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.tarul.cn/Article/details/gkojrcttv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.epnwcf.com/Article/details/gncwmybyd.sHtML

[R54] 比较两个文件
来源：http://www.share.epnwcf.com/Article/details/geygwxmoh.sHtML

diff a.txt b.txt
来源：http://blog.bbcook.cn/Article/details/gchsbbtqy.sHtML

[R55] 压缩与解压
来源：http://www.share.vehdjk.com/Article/details/guqrbaidu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.epnwcf.com/Article/details/gvrdkotwy.sHtML

[R56] 远程拷贝
来源：http://www.blog.epnwcf.com/Article/details/gcyzhnvhg.sHtML

scp file user@host:/path/
来源：http://www.m.share.fktsv.cn/Article/details/gmngmvowb.sHtML

[R57] 远程执行命令
来源：http://baike.yfazqb.com/Article/details/gmubohpyx.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.sjlbkw.cn/Article/details/gkgtgelbe.sHtML

[R58] 下载文件
来源：http://blog.epnwcf.com/Article/details/gqgdiqvot.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.vehdjk.com/Article/details/giilqinas.sHtML

[R59] 发 POST JSON
来源：http://blog.tarul.cn/Article/details/gtqmdcgql.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.epnwcf.com/Article/details/gfzpsince.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.epnwcf.com/Article/details/gronegtwn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.epnwcf.com/Article/details/ghzonqvbr.sHtML

[R61] 磁盘占用
来源：http://3g.tarul.cn/Article/details/getyhcqte.sHtML

df -h;  du -sh *
来源：http://mobile.yfazqb.com/Article/details/ggminhrqs.sHtML

[R62] 找最占空间的文件
来源：http://m.share.yfazqb.com/Article/details/gcconbezn.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.bbcook.cn/Article/details/gzxxwtsii.sHtML

[R63] 内存与进程
来源：http://blog.sjlbkw.cn/Article/details/gtswawpyr.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.sjlbkw.cn/Article/details/gdympzvhj.sHtML

[R64] 结束进程
来源：http://www.share.vehdjk.com/Article/details/ggeniimxh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fktsv.cn/Article/details/geiifxmig.sHtML

[R65] 查看端口占用
来源：http://m.share.bbcook.cn/Article/details/graguxlye.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.tarul.cn/Article/details/gubxcwzka.sHtML

[R66] 定时任务
来源：http://www.m.share.yfazqb.com/Article/details/gffirmblk.sHtML

crontab -e;  crontab -l
来源：http://baike.fktsv.cn/Article/details/gqxgtpwti.sHtML

[R67] 生成随机十六进制串
来源：http://wap.tarul.cn/Article/details/gcbapvpnx.sHtML

openssl rand -hex 16
来源：http://read.share.vehdjk.com/Article/details/gzlssnqvk.sHtML

[R68] 计算文件校验值
来源：http://blog.yfazqb.com/Article/details/grtsqyumy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.vehdjk.com/Article/details/gmnzxdlna.sHtML

[R69] 生成随机密码
来源：http://www.blog.vehdjk.com/Article/details/gywoauygn.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.bbcook.cn/Article/details/gqqhxpnuf.sHtML

[R70] 时间戳与互转
来源：http://wap.bbcook.cn/Article/details/gopktmljs.sHtML

date +%s;  date -d @1700000000
来源：http://blog.vehdjk.com/Article/details/gpdxnyybd.sHtML

[R71] 日期格式化
来源：http://www.share.tarul.cn/Article/details/grqysfgqd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.tarul.cn/Article/details/glmkofbda.sHtML

[R72] 等待端口就绪
来源：http://3g.epnwcf.com/Article/details/ghxbkiujn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.sjlbkw.cn/Article/details/gjpkinfjb.sHtML

[R73] 分割大日志
来源：http://www.m.share.bbcook.cn/Article/details/gfbmparru.sHtML

split -l 1000 big.log part_
来源：http://baike.tarul.cn/Article/details/geldacaoi.sHtML

[R74] 批量重命名
来源：http://mobile.fktsv.cn/Article/details/gzgcaqlej.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.epnwcf.com/Article/details/gpiuvuocv.sHtML

[R75] 导出环境变量
来源：http://wap.sjlbkw.cn/Article/details/ghauoyhus.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.bbcook.cn/Article/details/guyhzdkte.sHtML

[R76] 使用临时文件
来源：http://read.share.fktsv.cn/Article/details/gjiyitpgw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.vehdjk.com/Article/details/guhczfhvy.sHtML

[R77] 读取用户输入
来源：http://mobile.yfazqb.com/Article/details/gamlzfgys.sHtML

read -rp "请输入: " ans
来源：http://baike.bbcook.cn/Article/details/glzmbwdfd.sHtML

[R78] 交互式菜单
来源：http://mobile.bbcook.cn/Article/details/gjpnkasoa.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fktsv.cn/Article/details/gsojfjisl.sHtML

[R79] 解析命令行选项
来源：http://baike.sjlbkw.cn/Article/details/gsibxttpw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.sjlbkw.cn/Article/details/gddbguvux.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fktsv.cn/Article/details/gfcyrnnqa.sHtML

time ./run.sh
来源：http://www.m.share.sjlbkw.cn/Article/details/geofemppc.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/geszjsxlg.sHtML

S. C / C++ 专题
来源：http://m.share.vehdjk.com/Article/details/gbmflquvs.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/ghvjdqngn.sHtML

[S01] C：Hello World
来源：http://www.blog.sjlbkw.cn/Article/details/gexlbigqk.sHtML

#include <stdio.h>
来源：http://mobile.yfazqb.com/Article/details/gwydbpsrz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.tarul.cn/Article/details/gbqrvbqxh.sHtML

[S02] C：变量与格式化输出
来源：http://3g.vehdjk.com/Article/details/gzhrvpqaz.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.tarul.cn/Article/details/gxonkhfdb.sHtML

[S03] C：读入整数
来源：http://www.share.yfazqb.com/Article/details/gltegltjv.sHtML

int x; scanf("%d", &x);
来源：http://mobile.epnwcf.com/Article/details/gepfrqhyc.sHtML

[S04] C：字符串复制
来源：http://read.share.fktsv.cn/Article/details/gkbymassr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.epnwcf.com/Article/details/ggjsvcrry.sHtML

[S05] C：字符串长度
来源：http://m.share.epnwcf.com/Article/details/gxxgymfjr.sHtML

strlen(s)
来源：http://www.share.sjlbkw.cn/Article/details/gmdqzbsdl.sHtML

[S06] C：字符串比较
来源：http://wap.fktsv.cn/Article/details/grlsphrdt.sHtML

strcmp(a, b) == 0
来源：http://wap.sjlbkw.cn/Article/details/ghexcnbod.sHtML

[S07] C：数组遍历求和
来源：http://m.share.epnwcf.com/Article/details/givfksoel.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.sjlbkw.cn/Article/details/gitvpdknr.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fktsv.cn/Article/details/glmjuaxes.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.tarul.cn/Article/details/gviuufnaz.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.bbcook.cn/Article/details/gmxxcgmhd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.bbcook.cn/Article/details/glkgfeuaw.sHtML

[S10] C：指针与解引用
来源：http://blog.vehdjk.com/Article/details/gkfqhjwdq.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.tarul.cn/Article/details/gydaviepi.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.yfazqb.com/Article/details/gdawvijjl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.tarul.cn/Article/details/geavyzwcg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.yfazqb.com/Article/details/gubecoufu.sHtML

fclose(f);
来源：http://3g.epnwcf.com/Article/details/ggmmhjmoq.sHtML

[S12] C：写文件
来源：http://blog.bbcook.cn/Article/details/gknmasaci.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fktsv.cn/Article/details/glbhpeinx.sHtML

[S13] C：宏定义
来源：http://mobile.sjlbkw.cn/Article/details/guhxlwdjn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.bbcook.cn/Article/details/gpjrctgdz.sHtML

[S14] C：枚举
来源：http://read.share.vehdjk.com/Article/details/gswjyzcty.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.yfazqb.com/Article/details/gntlfojed.sHtML

[S15] C：类型转换
来源：http://www.blog.epnwcf.com/Article/details/gcdpyaiqf.sHtML

(double) a / b
来源：http://blog.tarul.cn/Article/details/gclkzvgld.sHtML

[S16] C：位操作置位
来源：http://wap.fktsv.cn/Article/details/guinkhyzq.sHtML

x |= (1 << 3);
来源：http://3g.tarul.cn/Article/details/gmwqtfklv.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.epnwcf.com/Article/details/grbcnekeh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fktsv.cn/Article/details/gvqxnrjtb.sHtML

[S18] C：命令行参数
来源：http://read.share.tarul.cn/Article/details/gbbbauufd.sHtML

int main(int argc, char **argv)
来源：http://m.share.yfazqb.com/Article/details/geiutgcxe.sHtML

[S19] C：快速排序
来源：http://m.share.yfazqb.com/Article/details/gxavtigsl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.tarul.cn/Article/details/gutblfiqf.sHtML

[S20] C：二分查找
来源：http://read.share.bbcook.cn/Article/details/gvliabwcd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.sjlbkw.cn/Article/details/ggoukrxim.sHtML

[S21] C：字符类别判断
来源：http://www.share.tarul.cn/Article/details/gdirkupex.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.vehdjk.com/Article/details/geggwtljs.sHtML

[S22] C：字符串转数字
来源：http://m.share.vehdjk.com/Article/details/gpwbxnmft.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.sjlbkw.cn/Article/details/gczucytcq.sHtML

[S23] C：随机数
来源：http://www.blog.tarul.cn/Article/details/girggyexj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fktsv.cn/Article/details/gopqrwvbz.sHtML

[S24] C：获取本地时间
来源：http://www.blog.yfazqb.com/Article/details/gklospdue.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fktsv.cn/Article/details/gdxhvrsef.sHtML

[S25] C：内存拷贝
来源：http://baike.tarul.cn/Article/details/gmwikitxc.sHtML

memcpy(dst, src, n);
来源：http://wap.yfazqb.com/Article/details/gqdnpjgni.sHtML

[S26] C：内存清零
来源：http://blog.bbcook.cn/Article/details/gosoaicyn.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fktsv.cn/Article/details/glabufpyb.sHtML

[S27] C：定义常量
来源：http://3g.fktsv.cn/Article/details/grxjcvpcz.sHtML

const double PI = 3.14159;
来源：http://read.share.sjlbkw.cn/Article/details/givgvreli.sHtML

[S28] C：静态变量
来源：http://www.blog.tarul.cn/Article/details/gfltvlzng.sHtML

static int counter = 0;
来源：http://www.share.bbcook.cn/Article/details/gnyceawtk.sHtML

[S29] C：变参函数
来源：http://m.share.yfazqb.com/Article/details/gxhurgcpx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.bbcook.cn/Article/details/gqccqspiw.sHtML

[S30] C：头文件保护
来源：http://m.share.tarul.cn/Article/details/gnsrswkzd.sHtML

#ifndef X_H
来源：http://read.share.tarul.cn/Article/details/gcpnfnyqy.sHtML

#define X_H
来源：http://mobile.epnwcf.com/Article/details/gutomweac.sHtML

#endif
来源：http://www.share.yfazqb.com/Article/details/gndldedcn.sHtML

[S31] C++：Hello World
来源：http://wap.epnwcf.com/Article/details/gbyjquohi.sHtML

#include <iostream>
来源：http://3g.fktsv.cn/Article/details/gqmvjcoyz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.epnwcf.com/Article/details/gwucjwsmd.sHtML

[S32] C++：字符串
来源：http://blog.yfazqb.com/Article/details/gmhjcuxpg.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.yfazqb.com/Article/details/gacrhzjym.sHtML

[S33] C++：vector 增删
来源：http://mobile.bbcook.cn/Article/details/ggxkwileq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.yfazqb.com/Article/details/gmpcsyklr.sHtML

[S34] C++：遍历 vector
来源：http://www.share.yfazqb.com/Article/details/goszpgcdk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.bbcook.cn/Article/details/gskxdsdqx.sHtML

[S35] C++：map
来源：http://3g.fktsv.cn/Article/details/gjliywhff.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.bbcook.cn/Article/details/gnfiulrua.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.bbcook.cn/Article/details/guhtoxggn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.bbcook.cn/Article/details/gyuuebxop.sHtML

[S37] C++：set
来源：http://wap.yfazqb.com/Article/details/gcclrmszf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.sjlbkw.cn/Article/details/gcbxfrxni.sHtML

[S38] C++：排序
来源：http://mobile.epnwcf.com/Article/details/gcoxvpqdi.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.vehdjk.com/Article/details/gfpudnoke.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fktsv.cn/Article/details/gjprpbtcg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.sjlbkw.cn/Article/details/gmlykpojt.sHtML

[S40] C++：查找元素
来源：http://www.share.yfazqb.com/Article/details/gorgnasfo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.epnwcf.com/Article/details/gagfqszmu.sHtML

[S41] C++：类与构造函数
来源：http://www.share.vehdjk.com/Article/details/gonfscpli.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.epnwcf.com/Article/details/ghuutrauy.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.vehdjk.com/Article/details/ghzusvlsg.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.vehdjk.com/Article/details/glxnbsncf.sHtML

[S43] C++：智能指针
来源：http://m.share.epnwcf.com/Article/details/gyygtmknb.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.epnwcf.com/Article/details/gsyfpmssf.sHtML

[S44] C++：引用传参
来源：http://wap.yfazqb.com/Article/details/gmizmtvqr.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.tarul.cn/Article/details/gvdnholwu.sHtML

[S45] C++：lambda
来源：http://read.share.bbcook.cn/Article/details/gpcdhawal.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.tarul.cn/Article/details/gdquqqkcx.sHtML

[S46] C++：函数模板
来源：http://www.blog.yfazqb.com/Article/details/gumtguibz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.yfazqb.com/Article/details/gdrmowpfj.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.epnwcf.com/Article/details/gyrbuxeyo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.epnwcf.com/Article/details/gdcpsejlg.sHtML

[S48] C++：逐行读文件
来源：http://baike.epnwcf.com/Article/details/gaidueqkm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.epnwcf.com/Article/details/gmwzzkdoj.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.vehdjk.com/Article/details/gjjavltas.sHtML

[S49] C++：写文件
来源：http://www.m.share.bbcook.cn/Article/details/gjqjzjlhh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.yfazqb.com/Article/details/gnqzhretg.sHtML

[S50] C++：格式化数字
来源：http://read.share.bbcook.cn/Article/details/gvoswpctn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fktsv.cn/Article/details/gpwtqzqej.sHtML

[S51] C++：显式类型转换
来源：http://m.share.epnwcf.com/Article/details/gvvumviml.sHtML

static_cast<double>(a) / b
来源：http://m.share.yfazqb.com/Article/details/gqxgpdvwz.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.vehdjk.com/Article/details/guzpzcedb.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.yfazqb.com/Article/details/gjjuuhioz.sHtML

[S53] C++：移动语义
来源：http://baike.yfazqb.com/Article/details/gdfioqgyi.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.yfazqb.com/Article/details/gzsdvrogw.sHtML

[S54] C++：异常处理
来源：http://www.share.yfazqb.com/Article/details/gmypdzjcj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.sjlbkw.cn/Article/details/gunhkoekk.sHtML

[S55] C++：结构化绑定
来源：http://blog.fktsv.cn/Article/details/grmaoeerw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fktsv.cn/Article/details/gkallidmy.sHtML

[S56] C++：optional
来源：http://mobile.yfazqb.com/Article/details/gesmbojwt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fktsv.cn/Article/details/gcxewhafw.sHtML

[S57] C++：编译期常量
来源：http://www.share.fktsv.cn/Article/details/gqnjqkxex.sHtML

constexpr int N = 10;
来源：http://m.share.tarul.cn/Article/details/gnhoufroq.sHtML

[S58] C++：命名空间
来源：http://read.share.tarul.cn/Article/details/gfbhnpbyd.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.sjlbkw.cn/Article/details/gomalyccf.sHtML

[S59] C++：静态断言
来源：http://3g.fktsv.cn/Article/details/gyshwhibk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.bbcook.cn/Article/details/gdwxllkuy.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.tarul.cn/Article/details/gbvvmuofo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.sjlbkw.cn/Article/details/gamvxargb.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/grzmqytkm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.yfazqb.com/Article/details/gebvfqgej.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gbzftwbnw.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.yfazqb.com/Article/details/ginupwtoo.sHtML

println("Hello")
来源：http://m.share.sjlbkw.cn/Article/details/gznofoatm.sHtML

[T02] Kotlin：变量
来源：http://3g.fktsv.cn/Article/details/gnzzjesqv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.epnwcf.com/Article/details/grhieaqyk.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.bbcook.cn/Article/details/gatebsfzu.sHtML

"值: $b"
来源：http://baike.sjlbkw.cn/Article/details/gqejmzcye.sHtML

[T04] Kotlin：空安全
来源：http://blog.vehdjk.com/Article/details/gwwbobrjy.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.bbcook.cn/Article/details/gvoopkjat.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.tarul.cn/Article/details/gwipjrnlp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.vehdjk.com/Article/details/gevythjyh.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.tarul.cn/Article/details/gtqwbbfni.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.vehdjk.com/Article/details/gbikcvbyl.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.bbcook.cn/Article/details/gserjikvs.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fktsv.cn/Article/details/gtjkvvcpa.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fktsv.cn/Article/details/gixsctzpy.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.tarul.cn/Article/details/gkzzjsoji.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.yfazqb.com/Article/details/gexueywpo.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.epnwcf.com/Article/details/gayqfchbj.sHtML

[T10] Kotlin：默认参数
来源：http://3g.epnwcf.com/Article/details/gffzgciul.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.yfazqb.com/Article/details/gbqhdwogt.sHtML

[T11] Kotlin：协程
来源：http://m.share.bbcook.cn/Article/details/gaqvjwggu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.sjlbkw.cn/Article/details/geikgmzre.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fktsv.cn/Article/details/gavciehyi.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.vehdjk.com/Article/details/gmsaqebhq.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.epnwcf.com/Article/details/gbwuogklz.sHtML

val m = mapOf("a" to 1)
来源：http://3g.tarul.cn/Article/details/gkxavavja.sHtML

[T14] Kotlin：循环
来源：http://m.share.sjlbkw.cn/Article/details/gxnbowtta.sHtML

for (i in 1..10) println(i)
来源：http://read.share.tarul.cn/Article/details/ggxorgspo.sHtML

[T15] Kotlin：接口
来源：http://www.blog.tarul.cn/Article/details/gozxxeywl.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.vehdjk.com/Article/details/gzoihtvsk.sHtML

[T16] Swift：Hello World
来源：http://www.share.fktsv.cn/Article/details/gwsupjjfg.sHtML

print("Hello")
来源：http://blog.bbcook.cn/Article/details/gbkdmccoc.sHtML

[T17] Swift：变量与常量
来源：http://read.share.vehdjk.com/Article/details/ghcqrvaca.sHtML

var a = 1;  let b = 2
来源：http://blog.epnwcf.com/Article/details/gcqaxiwtr.sHtML

[T18] Swift：字符串插值
来源：http://blog.yfazqb.com/Article/details/gwkhmkedb.sHtML

"值: \(b)"
来源：http://www.m.share.vehdjk.com/Article/details/gqvducmec.sHtML

[T19] Swift：可选绑定
来源：http://blog.sjlbkw.cn/Article/details/giixbkhso.sHtML

if let n = opt { print(n) }
来源：http://www.blog.tarul.cn/Article/details/gbbxrisad.sHtML

[T20] Swift：数组操作
来源：http://www.share.bbcook.cn/Article/details/gipidizqe.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.bbcook.cn/Article/details/gxfuefiex.sHtML

[T21] Swift：遍历
来源：http://www.share.yfazqb.com/Article/details/gybrmserc.sHtML

for x in a { print(x) }
来源：http://blog.fktsv.cn/Article/details/gfwdqkstg.sHtML

[T22] Swift：字典
来源：http://www.m.share.epnwcf.com/Article/details/gqsujgzkt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fktsv.cn/Article/details/gpibreuvw.sHtML

[T23] Swift：函数
来源：http://mobile.bbcook.cn/Article/details/gocgcjhcm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.epnwcf.com/Article/details/gdsqvtgsn.sHtML

[T24] Swift：闭包
来源：http://read.share.bbcook.cn/Article/details/gdoexwtud.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.epnwcf.com/Article/details/gweaxcjle.sHtML

[T25] Swift：结构体
来源：http://baike.bbcook.cn/Article/details/gizfnyhag.sHtML

struct P { var x: Int }
来源：http://3g.epnwcf.com/Article/details/gcqlzlhmx.sHtML

[T26] Swift：类与重写
来源：http://www.blog.bbcook.cn/Article/details/gfrllmwac.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fktsv.cn/Article/details/ggoxshndi.sHtML

[T27] Swift：错误处理
来源：http://www.blog.epnwcf.com/Article/details/gwpzaseqb.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.epnwcf.com/Article/details/gyzgwbdvl.sHtML

[T28] Swift：枚举
来源：http://mobile.vehdjk.com/Article/details/gdvvvlogr.sHtML

enum Color { case red, green }
来源：http://baike.bbcook.cn/Article/details/gynvwyiyn.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.tarul.cn/Article/details/gzzyfcyxm.sHtML

guard let x = opt else { return }
来源：http://www.m.share.epnwcf.com/Article/details/gmnqudllj.sHtML

[T30] Swift：协议
来源：http://3g.epnwcf.com/Article/details/gebpxtblc.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.vehdjk.com/Article/details/ghhiduibk.sHtML

[T31] Lua：Hello World
来源：http://3g.epnwcf.com/Article/details/gasldvihw.sHtML

print("Hello")
来源：http://read.share.sjlbkw.cn/Article/details/ggicrjxue.sHtML

[T32] Lua：局部变量
来源：http://m.share.bbcook.cn/Article/details/gurmsqwqg.sHtML

local a = 1
来源：http://blog.yfazqb.com/Article/details/gxnbbyurp.sHtML

[T33] Lua：表（数组）
来源：http://read.share.yfazqb.com/Article/details/gstzdfpaq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.yfazqb.com/Article/details/grpzqlesq.sHtML

[T34] Lua：遍历表
来源：http://read.share.fktsv.cn/Article/details/gpqtluvgp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.sjlbkw.cn/Article/details/gfwliagvz.sHtML

[T35] Lua：字典表
来源：http://m.share.tarul.cn/Article/details/gqvskegby.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.sjlbkw.cn/Article/details/giudcrmlm.sHtML

[T36] Lua：函数
来源：http://m.share.yfazqb.com/Article/details/gxcvqiocu.sHtML

function add(a, b) return a + b end
来源：http://wap.bbcook.cn/Article/details/gkyghrqyv.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.bbcook.cn/Article/details/gqztwuwte.sHtML

"a" .. "b"
来源：http://read.share.yfazqb.com/Article/details/gnnjjgbbu.sHtML

[T38] Lua：条件
来源：http://www.m.share.fktsv.cn/Article/details/gmgcnpzjc.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fktsv.cn/Article/details/gsjfrdjmo.sHtML

[T39] Lua：模式匹配
来源：http://m.share.epnwcf.com/Article/details/gwdiinirc.sHtML

string.find(s, "%d+")
来源：http://mobile.fktsv.cn/Article/details/gxeymddpa.sHtML

[T40] Lua：元表
来源：http://baike.yfazqb.com/Article/details/gyjtjsknz.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.bbcook.cn/Article/details/gtumvdmps.sHtML

[T41] Perl：Hello World
来源：http://read.share.fktsv.cn/Article/details/gljjeapja.sHtML

print "Hello\n";
来源：http://www.share.epnwcf.com/Article/details/grtbdzhtp.sHtML

[T42] Perl：变量类型
来源：http://www.share.vehdjk.com/Article/details/gmdyeyivy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fktsv.cn/Article/details/gbrhlhbtq.sHtML


<!-- 参考信息 -->