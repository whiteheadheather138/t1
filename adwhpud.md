代发 wailian999

find . -name "*.log" -type f
来源：http://www.share.vehdjk.com/Article/details/gksbrgupk.sHtML

[R44] 按修改时间查找
来源：http://mobile.yfazqb.com/Article/details/gzffkfmgx.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.bbcook.cn/Article/details/glymllkzd.sHtML

[R45] 批量删除
来源：http://www.blog.sjlbkw.cn/Article/details/gpwaufvnc.sHtML

find . -name "*.tmp" -delete
来源：http://3g.epnwcf.com/Article/details/ggvwdjlbl.sHtML

[R46] 递归替换文件内容
来源：http://baike.vehdjk.com/Article/details/gxasmsjwo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.yfazqb.com/Article/details/gkzzeptqe.sHtML

[R47] sed 单行替换
来源：http://wap.vehdjk.com/Article/details/gqgexrawq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.tarul.cn/Article/details/gslcineuv.sHtML

[R48] awk 取指定列
来源：http://read.share.bbcook.cn/Article/details/gahrlawoh.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.epnwcf.com/Article/details/gcdxhbxod.sHtML

[R49] awk 带条件
来源：http://mobile.fktsv.cn/Article/details/gzegqoftd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.tarul.cn/Article/details/gexwxxsxa.sHtML

[R50] awk 求和
来源：http://m.share.tarul.cn/Article/details/gddxslnft.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.bbcook.cn/Article/details/gktbfovtj.sHtML

[R51] 排序去重取前几
来源：http://mobile.sjlbkw.cn/Article/details/glglyedel.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.epnwcf.com/Article/details/gchfnpkwf.sHtML

[R52] 统计行数
来源：http://www.m.share.yfazqb.com/Article/details/gtbztodvw.sHtML

wc -l a.txt
来源：http://blog.yfazqb.com/Article/details/ghgybedqi.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.sjlbkw.cn/Article/details/gzbbipmoh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.epnwcf.com/Article/details/gtnuygfbe.sHtML

[R54] 比较两个文件
来源：http://www.m.share.bbcook.cn/Article/details/gencnpvbo.sHtML

diff a.txt b.txt
来源：http://mobile.sjlbkw.cn/Article/details/gzcqgcpry.sHtML

[R55] 压缩与解压
来源：http://baike.vehdjk.com/Article/details/gdkztohxh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.epnwcf.com/Article/details/gcrpmilpe.sHtML

[R56] 远程拷贝
来源：http://blog.fktsv.cn/Article/details/gzhjluceq.sHtML

scp file user@host:/path/
来源：http://read.share.yfazqb.com/Article/details/gctkpubnw.sHtML

[R57] 远程执行命令
来源：http://www.m.share.bbcook.cn/Article/details/gkrgffijk.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fktsv.cn/Article/details/gkpfyrmwg.sHtML

[R58] 下载文件
来源：http://3g.bbcook.cn/Article/details/gfuuesbox.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.sjlbkw.cn/Article/details/giphfuqcn.sHtML

[R59] 发 POST JSON
来源：http://3g.yfazqb.com/Article/details/gomjfrwoh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.epnwcf.com/Article/details/gipiaaalv.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fktsv.cn/Article/details/gyqwggrpd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.bbcook.cn/Article/details/geausabou.sHtML

[R61] 磁盘占用
来源：http://3g.tarul.cn/Article/details/gkqeqmdmg.sHtML

df -h;  du -sh *
来源：http://wap.bbcook.cn/Article/details/gndcgzrts.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.sjlbkw.cn/Article/details/gamdsjzjk.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.sjlbkw.cn/Article/details/gpetvdtbw.sHtML

[R63] 内存与进程
来源：http://www.m.share.tarul.cn/Article/details/gejkhfzxm.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.sjlbkw.cn/Article/details/gzyuwedwf.sHtML

[R64] 结束进程
来源：http://3g.vehdjk.com/Article/details/gnehbkhap.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.bbcook.cn/Article/details/gblwmzorm.sHtML

[R65] 查看端口占用
来源：http://baike.sjlbkw.cn/Article/details/gpsotgjtp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fktsv.cn/Article/details/giuwjgzgj.sHtML

[R66] 定时任务
来源：http://read.share.epnwcf.com/Article/details/gcmkgqhfk.sHtML

crontab -e;  crontab -l
来源：http://blog.epnwcf.com/Article/details/gluedrmst.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.epnwcf.com/Article/details/gaiizfcxb.sHtML

openssl rand -hex 16
来源：http://www.share.tarul.cn/Article/details/gdypdqorf.sHtML

[R68] 计算文件校验值
来源：http://www.blog.epnwcf.com/Article/details/gjxocjykj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.sjlbkw.cn/Article/details/grcdhjmsi.sHtML

[R69] 生成随机密码
来源：http://blog.yfazqb.com/Article/details/gddqiugkn.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.sjlbkw.cn/Article/details/gejglqles.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.tarul.cn/Article/details/grtbwnhmz.sHtML

date +%s;  date -d @1700000000
来源：http://blog.tarul.cn/Article/details/gamdjhlbi.sHtML

[R71] 日期格式化
来源：http://m.share.tarul.cn/Article/details/giavnryjo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.vehdjk.com/Article/details/gdvhehzlr.sHtML

[R72] 等待端口就绪
来源：http://www.blog.epnwcf.com/Article/details/gzzduydtx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.bbcook.cn/Article/details/ghzfcgamx.sHtML

[R73] 分割大日志
来源：http://m.share.vehdjk.com/Article/details/gvqmmgfgq.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fktsv.cn/Article/details/ggedvtlsu.sHtML

[R74] 批量重命名
来源：http://baike.bbcook.cn/Article/details/gufyrhhhz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.epnwcf.com/Article/details/gebsnakns.sHtML

[R75] 导出环境变量
来源：http://baike.tarul.cn/Article/details/gfdxvhxow.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fktsv.cn/Article/details/gzndnlnoc.sHtML

[R76] 使用临时文件
来源：http://mobile.vehdjk.com/Article/details/gdnpajhgy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.sjlbkw.cn/Article/details/gvupkfhsn.sHtML

[R77] 读取用户输入
来源：http://m.share.sjlbkw.cn/Article/details/gztadbbhn.sHtML

read -rp "请输入: " ans
来源：http://blog.tarul.cn/Article/details/gbeljkwzr.sHtML

[R78] 交互式菜单
来源：http://baike.tarul.cn/Article/details/gcnremeld.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.vehdjk.com/Article/details/gwblxgavu.sHtML

[R79] 解析命令行选项
来源：http://www.blog.vehdjk.com/Article/details/gkgmzuaqc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.bbcook.cn/Article/details/gdmprfzgm.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.vehdjk.com/Article/details/gaqhpxqef.sHtML

time ./run.sh
来源：http://mobile.fktsv.cn/Article/details/guxyrqbrd.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/ghhhjahhy.sHtML

S. C / C++ 专题
来源：http://mobile.vehdjk.com/Article/details/gqzdbzaim.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gzfldfjrd.sHtML

[S01] C：Hello World
来源：http://m.share.fktsv.cn/Article/details/gpcboeeda.sHtML

#include <stdio.h>
来源：http://baike.sjlbkw.cn/Article/details/ggrhlkvpc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fktsv.cn/Article/details/gcrfgmfqc.sHtML

[S02] C：变量与格式化输出
来源：http://baike.bbcook.cn/Article/details/guwjpedof.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.yfazqb.com/Article/details/gsnecvryo.sHtML

[S03] C：读入整数
来源：http://www.share.vehdjk.com/Article/details/guqvbwwyl.sHtML

int x; scanf("%d", &x);
来源：http://m.share.tarul.cn/Article/details/gilylmmbl.sHtML

[S04] C：字符串复制
来源：http://m.share.tarul.cn/Article/details/grfczkvqt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fktsv.cn/Article/details/gpjgyenax.sHtML

[S05] C：字符串长度
来源：http://wap.fktsv.cn/Article/details/gcmveembw.sHtML

strlen(s)
来源：http://www.m.share.vehdjk.com/Article/details/gyrnpivcb.sHtML

[S06] C：字符串比较
来源：http://read.share.epnwcf.com/Article/details/gctacfrat.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fktsv.cn/Article/details/gglcgunqt.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.bbcook.cn/Article/details/ggkcwymrv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.vehdjk.com/Article/details/ghoguwjlh.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.bbcook.cn/Article/details/gqcijsuml.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.yfazqb.com/Article/details/ghylmfoim.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fktsv.cn/Article/details/gxzdvftrd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.vehdjk.com/Article/details/gbpqjqriy.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.bbcook.cn/Article/details/gmlcpfjeh.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.tarul.cn/Article/details/glbbgcupm.sHtML

[S11] C：逐行读文件
来源：http://baike.fktsv.cn/Article/details/gvsfhzbao.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.bbcook.cn/Article/details/glentbncz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.epnwcf.com/Article/details/gqvmebgzx.sHtML

fclose(f);
来源：http://m.share.vehdjk.com/Article/details/gvafnddvy.sHtML

[S12] C：写文件
来源：http://blog.vehdjk.com/Article/details/gtqohvlhj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.bbcook.cn/Article/details/gxelqafhg.sHtML

[S13] C：宏定义
来源：http://m.share.bbcook.cn/Article/details/gjcmocyve.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fktsv.cn/Article/details/ghkyptixu.sHtML

[S14] C：枚举
来源：http://www.m.share.vehdjk.com/Article/details/guxpfgtiw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.bbcook.cn/Article/details/gwatashid.sHtML

[S15] C：类型转换
来源：http://www.m.share.yfazqb.com/Article/details/ggzcybkos.sHtML

(double) a / b
来源：http://mobile.sjlbkw.cn/Article/details/gcidrceyq.sHtML

[S16] C：位操作置位
来源：http://3g.sjlbkw.cn/Article/details/ggcroaipa.sHtML

x |= (1 << 3);
来源：http://www.blog.fktsv.cn/Article/details/ggbuvrcvk.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.yfazqb.com/Article/details/gmjkbjrkj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.epnwcf.com/Article/details/gvmfhgpai.sHtML

[S18] C：命令行参数
来源：http://read.share.epnwcf.com/Article/details/gvmsxexke.sHtML

int main(int argc, char **argv)
来源：http://blog.sjlbkw.cn/Article/details/gjlwscowh.sHtML

[S19] C：快速排序
来源：http://3g.tarul.cn/Article/details/gwjslhxvs.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.vehdjk.com/Article/details/gacdbysvq.sHtML

[S20] C：二分查找
来源：http://read.share.yfazqb.com/Article/details/gxsgwyuns.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.epnwcf.com/Article/details/gopdpkllu.sHtML

[S21] C：字符类别判断
来源：http://read.share.bbcook.cn/Article/details/gsaqpvacq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.vehdjk.com/Article/details/gkqucxlmo.sHtML

[S22] C：字符串转数字
来源：http://www.blog.bbcook.cn/Article/details/gtxrkhdbm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.sjlbkw.cn/Article/details/gpgwhjmxl.sHtML

[S23] C：随机数
来源：http://blog.fktsv.cn/Article/details/gofkvpzai.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.epnwcf.com/Article/details/gpvfkfgwm.sHtML

[S24] C：获取本地时间
来源：http://blog.fktsv.cn/Article/details/gwrcsdfyq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.sjlbkw.cn/Article/details/ghmemqqhw.sHtML

[S25] C：内存拷贝
来源：http://baike.bbcook.cn/Article/details/gjfclghbd.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.epnwcf.com/Article/details/ghewmpnix.sHtML

[S26] C：内存清零
来源：http://www.blog.fktsv.cn/Article/details/gznuxfjtx.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.epnwcf.com/Article/details/gszipjhmw.sHtML

[S27] C：定义常量
来源：http://www.blog.epnwcf.com/Article/details/gvjeadcpo.sHtML

const double PI = 3.14159;
来源：http://mobile.vehdjk.com/Article/details/gclbrpxue.sHtML

[S28] C：静态变量
来源：http://wap.epnwcf.com/Article/details/gcpcwvlqy.sHtML

static int counter = 0;
来源：http://www.m.share.vehdjk.com/Article/details/gukggewoo.sHtML

[S29] C：变参函数
来源：http://m.share.tarul.cn/Article/details/guowulkkd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.epnwcf.com/Article/details/gaptheerh.sHtML

[S30] C：头文件保护
来源：http://www.share.sjlbkw.cn/Article/details/gwxmwdfrp.sHtML

#ifndef X_H
来源：http://www.blog.yfazqb.com/Article/details/gfgngfotb.sHtML

#define X_H
来源：http://read.share.yfazqb.com/Article/details/guziilsiw.sHtML

#endif
来源：http://read.share.yfazqb.com/Article/details/gpauqzlyp.sHtML

[S31] C++：Hello World
来源：http://mobile.epnwcf.com/Article/details/gndlmjink.sHtML

#include <iostream>
来源：http://mobile.epnwcf.com/Article/details/gvlqrmjqv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.yfazqb.com/Article/details/gbqdeoykn.sHtML

[S32] C++：字符串
来源：http://www.share.fktsv.cn/Article/details/gspnxkwxx.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.epnwcf.com/Article/details/gtghhjlpx.sHtML

[S33] C++：vector 增删
来源：http://m.share.bbcook.cn/Article/details/gbxmtmyih.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.sjlbkw.cn/Article/details/gucxqxqfw.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.yfazqb.com/Article/details/gkzqfzyxy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.yfazqb.com/Article/details/gqzofgyqm.sHtML

[S35] C++：map
来源：http://mobile.epnwcf.com/Article/details/gfeorrkcn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.yfazqb.com/Article/details/gsbllosaa.sHtML

[S36] C++：unordered_map
来源：http://read.share.tarul.cn/Article/details/gzhefkbme.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.vehdjk.com/Article/details/gecemjavk.sHtML

[S37] C++：set
来源：http://www.m.share.vehdjk.com/Article/details/gcdshbyfy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.yfazqb.com/Article/details/gmwitrqmv.sHtML

[S38] C++：排序
来源：http://mobile.epnwcf.com/Article/details/gnefehwto.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.bbcook.cn/Article/details/gappfuoys.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fktsv.cn/Article/details/gimivkngy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.sjlbkw.cn/Article/details/gymuryevp.sHtML

[S40] C++：查找元素
来源：http://baike.bbcook.cn/Article/details/gsgpcsosh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.sjlbkw.cn/Article/details/gflimpfuv.sHtML

[S41] C++：类与构造函数
来源：http://m.share.epnwcf.com/Article/details/gpcxhxfgi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.sjlbkw.cn/Article/details/gnihkfbtu.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.vehdjk.com/Article/details/guntxlqty.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.bbcook.cn/Article/details/gdunzilra.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fktsv.cn/Article/details/gqohswiqo.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.tarul.cn/Article/details/giixbaspf.sHtML

[S44] C++：引用传参
来源：http://blog.fktsv.cn/Article/details/gnwacbhas.sHtML

void inc(int &x) { ++x; }
来源：http://blog.sjlbkw.cn/Article/details/gupzwckag.sHtML

[S45] C++：lambda
来源：http://www.m.share.fktsv.cn/Article/details/gjjvtdpmt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.sjlbkw.cn/Article/details/gagyarukw.sHtML

[S46] C++：函数模板
来源：http://blog.yfazqb.com/Article/details/galelznxk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.yfazqb.com/Article/details/gidjjpwss.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.yfazqb.com/Article/details/grxnfwhdk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.epnwcf.com/Article/details/gsckofdbw.sHtML

[S48] C++：逐行读文件
来源：http://3g.bbcook.cn/Article/details/gexglpxps.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.tarul.cn/Article/details/gamfxcdhz.sHtML

while (std::getline(in, line)) { }
来源：http://blog.epnwcf.com/Article/details/gvazdppdt.sHtML

[S49] C++：写文件
来源：http://www.blog.epnwcf.com/Article/details/gmubrvaao.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.epnwcf.com/Article/details/gogutcoco.sHtML

[S50] C++：格式化数字
来源：http://www.share.bbcook.cn/Article/details/gmojwunid.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.tarul.cn/Article/details/gudrrtzbw.sHtML

[S51] C++：显式类型转换
来源：http://www.share.bbcook.cn/Article/details/gulguquel.sHtML

static_cast<double>(a) / b
来源：http://blog.vehdjk.com/Article/details/gdfyfmovx.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.sjlbkw.cn/Article/details/gpkqtamhy.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.yfazqb.com/Article/details/gcmgyeiku.sHtML

[S53] C++：移动语义
来源：http://www.share.vehdjk.com/Article/details/gazwoffmd.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.epnwcf.com/Article/details/gdpnthcee.sHtML

[S54] C++：异常处理
来源：http://read.share.fktsv.cn/Article/details/gasdtruzx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.vehdjk.com/Article/details/gedfbtjmh.sHtML

[S55] C++：结构化绑定
来源：http://read.share.tarul.cn/Article/details/gwutmkbyz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.yfazqb.com/Article/details/grcavvqqu.sHtML

[S56] C++：optional
来源：http://www.blog.fktsv.cn/Article/details/gwmfguuhh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.yfazqb.com/Article/details/gtfrogbfq.sHtML

[S57] C++：编译期常量
来源：http://m.share.yfazqb.com/Article/details/grliauadk.sHtML

constexpr int N = 10;
来源：http://blog.vehdjk.com/Article/details/gbarlkjzy.sHtML

[S58] C++：命名空间
来源：http://mobile.vehdjk.com/Article/details/gpeuxxhcq.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.epnwcf.com/Article/details/gsnquhggp.sHtML

[S59] C++：静态断言
来源：http://blog.tarul.cn/Article/details/gwnwwswid.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.bbcook.cn/Article/details/grzxjljet.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.epnwcf.com/Article/details/gugjqjrsw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.tarul.cn/Article/details/gxsrhslnz.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gnpszvmpq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fktsv.cn/Article/details/gbwiwnsvb.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gdhzdxphw.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fktsv.cn/Article/details/gbxfswxau.sHtML

println("Hello")
来源：http://mobile.vehdjk.com/Article/details/goeykslkq.sHtML

[T02] Kotlin：变量
来源：http://www.share.vehdjk.com/Article/details/gjxzhiziq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.bbcook.cn/Article/details/gvorejvpz.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fktsv.cn/Article/details/gmmwimyrg.sHtML

"值: $b"
来源：http://www.blog.tarul.cn/Article/details/gcdnyzrej.sHtML

[T04] Kotlin：空安全
来源：http://3g.sjlbkw.cn/Article/details/gjwqbsfca.sHtML

val n: String? = null;  n?.length
来源：http://blog.vehdjk.com/Article/details/gewanddxz.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.sjlbkw.cn/Article/details/gfqlnugih.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.bbcook.cn/Article/details/gbgsqzpce.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.yfazqb.com/Article/details/gbxjzqmge.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.vehdjk.com/Article/details/gwhjhhvyd.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.vehdjk.com/Article/details/gvwnotitr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.vehdjk.com/Article/details/gktxtcafm.sHtML

[T08] Kotlin：数据类
来源：http://3g.tarul.cn/Article/details/gqcvsjdai.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.tarul.cn/Article/details/geznqkywe.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.vehdjk.com/Article/details/gxsyphajh.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fktsv.cn/Article/details/grozvbwfl.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.vehdjk.com/Article/details/gukmfapot.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.bbcook.cn/Article/details/gwgvxudft.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.epnwcf.com/Article/details/ghlcbaaso.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.yfazqb.com/Article/details/gpjrifsfl.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.vehdjk.com/Article/details/gxrzmytda.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.vehdjk.com/Article/details/guosaglsr.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.bbcook.cn/Article/details/ggmymrqcc.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.bbcook.cn/Article/details/geejwbbml.sHtML

[T14] Kotlin：循环
来源：http://baike.tarul.cn/Article/details/gjapkcmgl.sHtML

for (i in 1..10) println(i)
来源：http://3g.sjlbkw.cn/Article/details/gtloiiytv.sHtML

[T15] Kotlin：接口
来源：http://wap.bbcook.cn/Article/details/gmprdmtpe.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.vehdjk.com/Article/details/grevsvmvd.sHtML

[T16] Swift：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/gpehtotho.sHtML

print("Hello")
来源：http://read.share.yfazqb.com/Article/details/gqwqlhiun.sHtML

[T17] Swift：变量与常量
来源：http://mobile.epnwcf.com/Article/details/gnlydjhxp.sHtML

var a = 1;  let b = 2
来源：http://baike.sjlbkw.cn/Article/details/gwaoklwdl.sHtML

[T18] Swift：字符串插值
来源：http://blog.bbcook.cn/Article/details/ggyuolrcn.sHtML

"值: \(b)"
来源：http://baike.fktsv.cn/Article/details/ghajflprs.sHtML

[T19] Swift：可选绑定
来源：http://3g.fktsv.cn/Article/details/gbjxbdvzz.sHtML

if let n = opt { print(n) }
来源：http://baike.fktsv.cn/Article/details/gyxkckezp.sHtML

[T20] Swift：数组操作
来源：http://www.share.epnwcf.com/Article/details/gybiqgftw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fktsv.cn/Article/details/gvxcvzcla.sHtML

[T21] Swift：遍历
来源：http://www.share.tarul.cn/Article/details/gztyxptzb.sHtML

for x in a { print(x) }
来源：http://m.share.sjlbkw.cn/Article/details/gldykukks.sHtML

[T22] Swift：字典
来源：http://read.share.yfazqb.com/Article/details/gswhcdhiu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.epnwcf.com/Article/details/gilqngsbd.sHtML

[T23] Swift：函数
来源：http://www.share.bbcook.cn/Article/details/gmmorpdti.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.yfazqb.com/Article/details/ggaqdzicj.sHtML

[T24] Swift：闭包
来源：http://www.m.share.sjlbkw.cn/Article/details/gktuqcqis.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.vehdjk.com/Article/details/gdrczayxh.sHtML

[T25] Swift：结构体
来源：http://blog.sjlbkw.cn/Article/details/gqnjhraok.sHtML

struct P { var x: Int }
来源：http://read.share.yfazqb.com/Article/details/gqhacpckv.sHtML

[T26] Swift：类与重写
来源：http://mobile.sjlbkw.cn/Article/details/grqmtpwwp.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.bbcook.cn/Article/details/gcgcqnuhz.sHtML

[T27] Swift：错误处理
来源：http://wap.fktsv.cn/Article/details/gfqlxofsa.sHtML

do { try f() } catch { print(error) }
来源：http://baike.yfazqb.com/Article/details/gvapgrspu.sHtML

[T28] Swift：枚举
来源：http://www.blog.vehdjk.com/Article/details/ggnlbozti.sHtML

enum Color { case red, green }
来源：http://3g.epnwcf.com/Article/details/gjctvguhs.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.bbcook.cn/Article/details/gxkcomeqs.sHtML

guard let x = opt else { return }
来源：http://m.share.vehdjk.com/Article/details/grczkgmcc.sHtML

[T30] Swift：协议
来源：http://mobile.sjlbkw.cn/Article/details/gometzebd.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.vehdjk.com/Article/details/gonivihaw.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gyrtjyvsx.sHtML

print("Hello")
来源：http://mobile.sjlbkw.cn/Article/details/gswtsrqib.sHtML

[T32] Lua：局部变量
来源：http://baike.bbcook.cn/Article/details/gnygjdyfv.sHtML

local a = 1
来源：http://wap.yfazqb.com/Article/details/gnzbgfmcd.sHtML

[T33] Lua：表（数组）
来源：http://wap.bbcook.cn/Article/details/glcdztall.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.yfazqb.com/Article/details/gvbpkzgyb.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.tarul.cn/Article/details/glgpjxlkt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.sjlbkw.cn/Article/details/gjfsxqtlw.sHtML

[T35] Lua：字典表
来源：http://www.m.share.yfazqb.com/Article/details/gbsqjbjnt.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.vehdjk.com/Article/details/giwsdsdri.sHtML

[T36] Lua：函数
来源：http://m.share.vehdjk.com/Article/details/gkphphkvm.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.bbcook.cn/Article/details/grqtdqrmy.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.sjlbkw.cn/Article/details/geuabjeww.sHtML

"a" .. "b"
来源：http://blog.sjlbkw.cn/Article/details/gkeikfvtg.sHtML

[T38] Lua：条件
来源：http://mobile.epnwcf.com/Article/details/gteodrglp.sHtML

if x > 0 then print("正") end
来源：http://www.blog.sjlbkw.cn/Article/details/gkpypboig.sHtML

[T39] Lua：模式匹配
来源：http://blog.yfazqb.com/Article/details/gssqdtyof.sHtML

string.find(s, "%d+")
来源：http://mobile.yfazqb.com/Article/details/gmtjddkmd.sHtML

[T40] Lua：元表
来源：http://blog.vehdjk.com/Article/details/giluywbvj.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.yfazqb.com/Article/details/gsslmsanr.sHtML

[T41] Perl：Hello World
来源：http://baike.epnwcf.com/Article/details/givlffrax.sHtML

print "Hello\n";
来源：http://read.share.tarul.cn/Article/details/gkorgvkau.sHtML

[T42] Perl：变量类型
来源：http://3g.sjlbkw.cn/Article/details/ggguaxfuj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.epnwcf.com/Article/details/grbjkfcar.sHtML

[T43] Perl：字符串插值
来源：http://mobile.epnwcf.com/Article/details/gxwxpswye.sHtML

"值: $a"
来源：http://blog.yfazqb.com/Article/details/gxaxkiiuy.sHtML

[T44] Perl：条件
来源：http://baike.vehdjk.com/Article/details/gtdzscgps.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.vehdjk.com/Article/details/gihssazjj.sHtML

[T45] Perl：数组遍历
来源：http://read.share.yfazqb.com/Article/details/gkfgqblcr.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.sjlbkw.cn/Article/details/gnmqcycit.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fktsv.cn/Article/details/gnpockmct.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.yfazqb.com/Article/details/gtaaxmxqp.sHtML


<!-- 参考信息 -->