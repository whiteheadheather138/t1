代发 wailian999

files=$(ls -1)
来源：http://baike.fktsv.cn/Article/details/gxldfypgl.sHtML

[R38] 管道串联
来源：http://blog.epnwcf.com/Article/details/grdyuobjg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.tarul.cn/Article/details/gtqwwkznt.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fktsv.cn/Article/details/gycvojosr.sHtML

cmd > out.log 2>&1
来源：http://www.blog.epnwcf.com/Article/details/gdywhtbhk.sHtML

[R40] 追加写日志
来源：http://www.m.share.epnwcf.com/Article/details/gexjogfix.sHtML

echo "log" >> out.log
来源：http://www.share.tarul.cn/Article/details/gzrzwxijw.sHtML

[R41] 丢弃输出
来源：http://m.share.bbcook.cn/Article/details/ghjmjzqve.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.sjlbkw.cn/Article/details/goinicbhs.sHtML

[R42] 输入重定向
来源：http://www.blog.yfazqb.com/Article/details/gnsmqcfyg.sHtML

wc -l < a.txt
来源：http://www.share.vehdjk.com/Article/details/grbnkjoom.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fktsv.cn/Article/details/gboftcauc.sHtML

find . -name "*.log" -type f
来源：http://3g.fktsv.cn/Article/details/gwirauhea.sHtML

[R44] 按修改时间查找
来源：http://read.share.fktsv.cn/Article/details/gbvwzwzhp.sHtML

find . -mtime -7 -type f
来源：http://m.share.vehdjk.com/Article/details/gsissczli.sHtML

[R45] 批量删除
来源：http://www.m.share.sjlbkw.cn/Article/details/gcwvwstxm.sHtML

find . -name "*.tmp" -delete
来源：http://wap.tarul.cn/Article/details/gxtzekuxp.sHtML

[R46] 递归替换文件内容
来源：http://blog.fktsv.cn/Article/details/gxfzavrwv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.yfazqb.com/Article/details/gfpqnqzcu.sHtML

[R47] sed 单行替换
来源：http://m.share.bbcook.cn/Article/details/gtjybtbhu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.bbcook.cn/Article/details/glyvikekg.sHtML

[R48] awk 取指定列
来源：http://baike.fktsv.cn/Article/details/gablihejs.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.tarul.cn/Article/details/gphimdhpd.sHtML

[R49] awk 带条件
来源：http://baike.epnwcf.com/Article/details/gccafulvg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fktsv.cn/Article/details/gwvhpnpjd.sHtML

[R50] awk 求和
来源：http://www.blog.yfazqb.com/Article/details/gmbrhziae.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.vehdjk.com/Article/details/gcvibyber.sHtML

[R51] 排序去重取前几
来源：http://mobile.fktsv.cn/Article/details/gmboeanmf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.yfazqb.com/Article/details/geexsshwu.sHtML

[R52] 统计行数
来源：http://3g.yfazqb.com/Article/details/gedtkqmfd.sHtML

wc -l a.txt
来源：http://mobile.yfazqb.com/Article/details/grrciknvj.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.sjlbkw.cn/Article/details/gzjppfbvx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fktsv.cn/Article/details/gvdwyvlfz.sHtML

[R54] 比较两个文件
来源：http://m.share.tarul.cn/Article/details/gzjbujtyw.sHtML

diff a.txt b.txt
来源：http://www.m.share.fktsv.cn/Article/details/gwrtvssbw.sHtML

[R55] 压缩与解压
来源：http://blog.yfazqb.com/Article/details/gdkfqfhry.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.yfazqb.com/Article/details/gxhkgnbrd.sHtML

[R56] 远程拷贝
来源：http://read.share.yfazqb.com/Article/details/gohnzxopu.sHtML

scp file user@host:/path/
来源：http://m.share.fktsv.cn/Article/details/ghbvruiiw.sHtML

[R57] 远程执行命令
来源：http://www.blog.tarul.cn/Article/details/gvrisvzru.sHtML

ssh user@host 'uptime'
来源：http://m.share.fktsv.cn/Article/details/gaszylyiy.sHtML

[R58] 下载文件
来源：http://mobile.bbcook.cn/Article/details/gkppeofvb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.vehdjk.com/Article/details/gxezwswde.sHtML

[R59] 发 POST JSON
来源：http://baike.epnwcf.com/Article/details/gwcofisoi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.epnwcf.com/Article/details/gglnapmor.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.tarul.cn/Article/details/gjcdyvifd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.vehdjk.com/Article/details/gxcimpkpc.sHtML

[R61] 磁盘占用
来源：http://www.share.tarul.cn/Article/details/gpomacpqi.sHtML

df -h;  du -sh *
来源：http://www.blog.tarul.cn/Article/details/gpkfrpmnf.sHtML

[R62] 找最占空间的文件
来源：http://wap.sjlbkw.cn/Article/details/gbhbcxwvh.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.tarul.cn/Article/details/ganwhqxag.sHtML

[R63] 内存与进程
来源：http://www.share.sjlbkw.cn/Article/details/gijnvbych.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.vehdjk.com/Article/details/gicslbeql.sHtML

[R64] 结束进程
来源：http://wap.fktsv.cn/Article/details/gltjrrsqb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.yfazqb.com/Article/details/gbmdgmdbw.sHtML

[R65] 查看端口占用
来源：http://www.m.share.sjlbkw.cn/Article/details/gsirxldyu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.vehdjk.com/Article/details/gfunqqhqk.sHtML

[R66] 定时任务
来源：http://wap.epnwcf.com/Article/details/gehbbcufz.sHtML

crontab -e;  crontab -l
来源：http://m.share.epnwcf.com/Article/details/grqyxxjav.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fktsv.cn/Article/details/gpufrbsbk.sHtML

openssl rand -hex 16
来源：http://www.share.yfazqb.com/Article/details/ggxlwnazb.sHtML

[R68] 计算文件校验值
来源：http://3g.yfazqb.com/Article/details/gaigevppt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.epnwcf.com/Article/details/geteepkrx.sHtML

[R69] 生成随机密码
来源：http://read.share.bbcook.cn/Article/details/gdywsnhho.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fktsv.cn/Article/details/ghpwijsyz.sHtML

[R70] 时间戳与互转
来源：http://m.share.yfazqb.com/Article/details/gvuxoswmi.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.sjlbkw.cn/Article/details/gdcmjjwga.sHtML

[R71] 日期格式化
来源：http://www.m.share.tarul.cn/Article/details/gemtrdgby.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.tarul.cn/Article/details/gutyqhgba.sHtML

[R72] 等待端口就绪
来源：http://www.blog.bbcook.cn/Article/details/gdhqlvjrs.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.tarul.cn/Article/details/grrjurlhw.sHtML

[R73] 分割大日志
来源：http://baike.tarul.cn/Article/details/gaykfrqjk.sHtML

split -l 1000 big.log part_
来源：http://3g.bbcook.cn/Article/details/gcdubnxyw.sHtML

[R74] 批量重命名
来源：http://www.m.share.bbcook.cn/Article/details/gpsdxfuei.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.vehdjk.com/Article/details/gsfzhjfzn.sHtML

[R75] 导出环境变量
来源：http://wap.yfazqb.com/Article/details/gmqpfpzsy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fktsv.cn/Article/details/gdnjhkyzj.sHtML

[R76] 使用临时文件
来源：http://www.m.share.tarul.cn/Article/details/gbxskuoed.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.vehdjk.com/Article/details/ghoakiqrl.sHtML

[R77] 读取用户输入
来源：http://wap.bbcook.cn/Article/details/gckgqybyz.sHtML

read -rp "请输入: " ans
来源：http://wap.sjlbkw.cn/Article/details/gpxdpaigs.sHtML

[R78] 交互式菜单
来源：http://www.m.share.tarul.cn/Article/details/gavqeppjv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.vehdjk.com/Article/details/gjctndpdn.sHtML

[R79] 解析命令行选项
来源：http://read.share.tarul.cn/Article/details/gnzrazqvn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.sjlbkw.cn/Article/details/gvzbdcbow.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.yfazqb.com/Article/details/gvpacinkq.sHtML

time ./run.sh
来源：http://www.blog.sjlbkw.cn/Article/details/godehpeds.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/giliqtdry.sHtML

S. C / C++ 专题
来源：http://m.share.fktsv.cn/Article/details/ggdlftlaz.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gwdtdahza.sHtML

[S01] C：Hello World
来源：http://m.share.fktsv.cn/Article/details/gzezcwgti.sHtML

#include <stdio.h>
来源：http://3g.tarul.cn/Article/details/geoeilgud.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.yfazqb.com/Article/details/gqturzrrb.sHtML

[S02] C：变量与格式化输出
来源：http://baike.epnwcf.com/Article/details/gykgdgdhu.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.tarul.cn/Article/details/gyjlqwwtu.sHtML

[S03] C：读入整数
来源：http://read.share.bbcook.cn/Article/details/godbybxxh.sHtML

int x; scanf("%d", &x);
来源：http://blog.fktsv.cn/Article/details/gcppmhzge.sHtML

[S04] C：字符串复制
来源：http://3g.bbcook.cn/Article/details/gxxibskbw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.yfazqb.com/Article/details/goxvhtpcu.sHtML

[S05] C：字符串长度
来源：http://mobile.yfazqb.com/Article/details/gfhkpvaec.sHtML

strlen(s)
来源：http://read.share.epnwcf.com/Article/details/gtgrfzksl.sHtML

[S06] C：字符串比较
来源：http://baike.vehdjk.com/Article/details/guugzdump.sHtML

strcmp(a, b) == 0
来源：http://3g.bbcook.cn/Article/details/gskovefcp.sHtML

[S07] C：数组遍历求和
来源：http://mobile.yfazqb.com/Article/details/gdwzyclom.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fktsv.cn/Article/details/geroztvuu.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fktsv.cn/Article/details/gcnlnlkol.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.bbcook.cn/Article/details/gsqjnkfpt.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.epnwcf.com/Article/details/gwahtaiym.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.yfazqb.com/Article/details/gmajwkivp.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.sjlbkw.cn/Article/details/gfzwtckke.sHtML

int *p = &a;  *p = 5;
来源：http://wap.bbcook.cn/Article/details/giyroapxa.sHtML

[S11] C：逐行读文件
来源：http://wap.tarul.cn/Article/details/gcrxeqdzf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.tarul.cn/Article/details/ggxbhhvpd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.sjlbkw.cn/Article/details/gvatcimxx.sHtML

fclose(f);
来源：http://read.share.fktsv.cn/Article/details/gobirlxes.sHtML

[S12] C：写文件
来源：http://3g.fktsv.cn/Article/details/gaombizek.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.bbcook.cn/Article/details/gbaoyhbpw.sHtML

[S13] C：宏定义
来源：http://3g.sjlbkw.cn/Article/details/gqojpkkji.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.bbcook.cn/Article/details/gcnbezxjo.sHtML

[S14] C：枚举
来源：http://www.blog.epnwcf.com/Article/details/gkobsjdej.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fktsv.cn/Article/details/gqzkfkbrl.sHtML

[S15] C：类型转换
来源：http://m.share.sjlbkw.cn/Article/details/gakpyomtz.sHtML

(double) a / b
来源：http://3g.sjlbkw.cn/Article/details/ggzpgnlnd.sHtML

[S16] C：位操作置位
来源：http://www.share.tarul.cn/Article/details/gbglbhaii.sHtML

x |= (1 << 3);
来源：http://baike.vehdjk.com/Article/details/gxcysrdci.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.sjlbkw.cn/Article/details/ginhtbuqb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.epnwcf.com/Article/details/gytuwbogs.sHtML

[S18] C：命令行参数
来源：http://3g.vehdjk.com/Article/details/gjowdmygm.sHtML

int main(int argc, char **argv)
来源：http://www.share.epnwcf.com/Article/details/gfuyetnjm.sHtML

[S19] C：快速排序
来源：http://baike.yfazqb.com/Article/details/gntinxqcr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.vehdjk.com/Article/details/gepvuhmnp.sHtML

[S20] C：二分查找
来源：http://wap.bbcook.cn/Article/details/ghdxoyyzb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.yfazqb.com/Article/details/gjreqtuhs.sHtML

[S21] C：字符类别判断
来源：http://baike.vehdjk.com/Article/details/gnpkujnax.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.epnwcf.com/Article/details/gpsawfkyr.sHtML

[S22] C：字符串转数字
来源：http://read.share.yfazqb.com/Article/details/gfyxxzqzv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.yfazqb.com/Article/details/gxeyqzxdk.sHtML

[S23] C：随机数
来源：http://www.m.share.vehdjk.com/Article/details/gjvwaixdb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.sjlbkw.cn/Article/details/gyibflmfi.sHtML

[S24] C：获取本地时间
来源：http://3g.fktsv.cn/Article/details/guyvzivst.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fktsv.cn/Article/details/gjpfnrxsi.sHtML

[S25] C：内存拷贝
来源：http://baike.vehdjk.com/Article/details/gxriitlvy.sHtML

memcpy(dst, src, n);
来源：http://baike.yfazqb.com/Article/details/gvbyngwtf.sHtML

[S26] C：内存清零
来源：http://m.share.yfazqb.com/Article/details/ghjlkfarn.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.epnwcf.com/Article/details/gxsddcrpz.sHtML

[S27] C：定义常量
来源：http://m.share.tarul.cn/Article/details/gosmxvyyw.sHtML

const double PI = 3.14159;
来源：http://m.share.epnwcf.com/Article/details/gmxpuiypo.sHtML

[S28] C：静态变量
来源：http://3g.yfazqb.com/Article/details/gfdzqzekg.sHtML

static int counter = 0;
来源：http://www.blog.fktsv.cn/Article/details/gzxdutyja.sHtML

[S29] C：变参函数
来源：http://baike.yfazqb.com/Article/details/gqvnhwllc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.tarul.cn/Article/details/galmozbdc.sHtML

[S30] C：头文件保护
来源：http://mobile.tarul.cn/Article/details/gsisqjioi.sHtML

#ifndef X_H
来源：http://blog.yfazqb.com/Article/details/gomluvoke.sHtML

#define X_H
来源：http://3g.yfazqb.com/Article/details/gsppjpbsu.sHtML

#endif
来源：http://baike.vehdjk.com/Article/details/guonrebcn.sHtML

[S31] C++：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gpxvyphmw.sHtML

#include <iostream>
来源：http://baike.sjlbkw.cn/Article/details/gbxahkbcz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.epnwcf.com/Article/details/gznjueoya.sHtML

[S32] C++：字符串
来源：http://mobile.vehdjk.com/Article/details/gejmketgi.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.bbcook.cn/Article/details/genakbayv.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fktsv.cn/Article/details/guxufulsh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fktsv.cn/Article/details/gdjsfcyak.sHtML

[S34] C++：遍历 vector
来源：http://wap.yfazqb.com/Article/details/gcfwvaqlq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fktsv.cn/Article/details/gldhoucxq.sHtML

[S35] C++：map
来源：http://www.m.share.epnwcf.com/Article/details/gzygtbvlw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.yfazqb.com/Article/details/griofhhmc.sHtML

[S36] C++：unordered_map
来源：http://www.share.yfazqb.com/Article/details/gwuzpsuei.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.sjlbkw.cn/Article/details/gxfaqirfs.sHtML

[S37] C++：set
来源：http://blog.fktsv.cn/Article/details/giiazrjib.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.bbcook.cn/Article/details/giyaqixwr.sHtML

[S38] C++：排序
来源：http://3g.fktsv.cn/Article/details/gaycdgbco.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.vehdjk.com/Article/details/gkousallu.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.vehdjk.com/Article/details/gaezyahjs.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.tarul.cn/Article/details/gtevuftoe.sHtML

[S40] C++：查找元素
来源：http://3g.bbcook.cn/Article/details/gxjjifrxr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fktsv.cn/Article/details/guzhfnlrf.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.bbcook.cn/Article/details/guozbntjq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.vehdjk.com/Article/details/gaehwmhqb.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.bbcook.cn/Article/details/gaonxzden.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.yfazqb.com/Article/details/gczwolkdl.sHtML

[S43] C++：智能指针
来源：http://www.blog.yfazqb.com/Article/details/gdxitwivc.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.bbcook.cn/Article/details/gzydvtrle.sHtML

[S44] C++：引用传参
来源：http://baike.epnwcf.com/Article/details/ggwkjmxgu.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.yfazqb.com/Article/details/ghxzuvaun.sHtML

[S45] C++：lambda
来源：http://wap.bbcook.cn/Article/details/grsgdmzkx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.sjlbkw.cn/Article/details/gulgzwvmw.sHtML

[S46] C++：函数模板
来源：http://m.share.yfazqb.com/Article/details/gabrgchwg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fktsv.cn/Article/details/grgtltdew.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.tarul.cn/Article/details/gicylgcyb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.yfazqb.com/Article/details/gslalphni.sHtML

[S48] C++：逐行读文件
来源：http://wap.vehdjk.com/Article/details/gnaqceiwm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.tarul.cn/Article/details/gbxabpprb.sHtML

while (std::getline(in, line)) { }
来源：http://wap.yfazqb.com/Article/details/gzimbvqfz.sHtML

[S49] C++：写文件
来源：http://3g.tarul.cn/Article/details/gcwbrqhql.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.sjlbkw.cn/Article/details/glrycesjw.sHtML

[S50] C++：格式化数字
来源：http://www.blog.vehdjk.com/Article/details/ggvbkrkkz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.tarul.cn/Article/details/ghdaorivp.sHtML

[S51] C++：显式类型转换
来源：http://blog.yfazqb.com/Article/details/ghxytnfnd.sHtML

static_cast<double>(a) / b
来源：http://blog.epnwcf.com/Article/details/gqmaqhegk.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fktsv.cn/Article/details/ghqkjzpvm.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.yfazqb.com/Article/details/geipirikv.sHtML

[S53] C++：移动语义
来源：http://www.blog.epnwcf.com/Article/details/gzovcjhxe.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.sjlbkw.cn/Article/details/gwdszsiqy.sHtML

[S54] C++：异常处理
来源：http://blog.yfazqb.com/Article/details/givtsfwqk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.sjlbkw.cn/Article/details/ggdejxwjv.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fktsv.cn/Article/details/gutclzzvz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.bbcook.cn/Article/details/gnmdpiayk.sHtML

[S56] C++：optional
来源：http://baike.fktsv.cn/Article/details/geunishqi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.epnwcf.com/Article/details/gkozjufue.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.bbcook.cn/Article/details/ghonqwlyt.sHtML

constexpr int N = 10;
来源：http://www.blog.tarul.cn/Article/details/gfhjohyjy.sHtML

[S58] C++：命名空间
来源：http://www.blog.sjlbkw.cn/Article/details/gkptwvijt.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fktsv.cn/Article/details/gulinwisw.sHtML

[S59] C++：静态断言
来源：http://m.share.bbcook.cn/Article/details/groyspsrg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fktsv.cn/Article/details/gllykbyzc.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fktsv.cn/Article/details/glxryjfyl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.vehdjk.com/Article/details/gltzlqnna.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/goedsfmyt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.vehdjk.com/Article/details/ggpvntjuz.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gxovfzogy.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/gyprtncgr.sHtML

println("Hello")
来源：http://3g.fktsv.cn/Article/details/gjfgrqbly.sHtML

[T02] Kotlin：变量
来源：http://blog.bbcook.cn/Article/details/gaqwqyswu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.epnwcf.com/Article/details/gaqhdmvzu.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.bbcook.cn/Article/details/gsfqacrzm.sHtML

"值: $b"
来源：http://baike.sjlbkw.cn/Article/details/ggclnrijt.sHtML

[T04] Kotlin：空安全
来源：http://baike.epnwcf.com/Article/details/gvodwchvq.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.bbcook.cn/Article/details/gzvcxyvie.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.yfazqb.com/Article/details/gjgbukblz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.tarul.cn/Article/details/gypsrrjvv.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fktsv.cn/Article/details/ggrcphyhr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.bbcook.cn/Article/details/gxlwsgqqu.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.epnwcf.com/Article/details/glwuvinzc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.vehdjk.com/Article/details/gsyjldpsn.sHtML

[T08] Kotlin：数据类
来源：http://m.share.sjlbkw.cn/Article/details/gukcxldqd.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.yfazqb.com/Article/details/ghnxrhfbc.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.tarul.cn/Article/details/gimsctnxw.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.bbcook.cn/Article/details/ghmnlrkxi.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fktsv.cn/Article/details/ghikhxvig.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.sjlbkw.cn/Article/details/gsccdezdr.sHtML

[T11] Kotlin：协程
来源：http://wap.bbcook.cn/Article/details/gjzydnwin.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.sjlbkw.cn/Article/details/glsnrxddd.sHtML

[T12] Kotlin：解构声明
来源：http://3g.yfazqb.com/Article/details/gtitonseq.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.tarul.cn/Article/details/gygvetgdw.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fktsv.cn/Article/details/gwzkgcxoz.sHtML

val m = mapOf("a" to 1)
来源：http://3g.bbcook.cn/Article/details/gwqihxynk.sHtML

[T14] Kotlin：循环
来源：http://www.share.sjlbkw.cn/Article/details/gfnjajwei.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fktsv.cn/Article/details/gcwpgqwrk.sHtML

[T15] Kotlin：接口
来源：http://baike.vehdjk.com/Article/details/gsgyhbxmt.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.tarul.cn/Article/details/gifutywql.sHtML

[T16] Swift：Hello World
来源：http://mobile.fktsv.cn/Article/details/gbdvhljke.sHtML

print("Hello")
来源：http://baike.epnwcf.com/Article/details/gvrtsdwlt.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fktsv.cn/Article/details/ggqjtalhd.sHtML

var a = 1;  let b = 2
来源：http://blog.yfazqb.com/Article/details/guvocjjxc.sHtML

[T18] Swift：字符串插值
来源：http://m.share.bbcook.cn/Article/details/gzlaihpaq.sHtML

"值: \(b)"
来源：http://mobile.epnwcf.com/Article/details/gnzvzzbyk.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fktsv.cn/Article/details/gdlsxgdez.sHtML

if let n = opt { print(n) }
来源：http://m.share.sjlbkw.cn/Article/details/guttwhnrk.sHtML

[T20] Swift：数组操作
来源：http://www.blog.sjlbkw.cn/Article/details/gjkwabrll.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.tarul.cn/Article/details/gcrcgmrdw.sHtML

[T21] Swift：遍历
来源：http://3g.tarul.cn/Article/details/glqemonvo.sHtML

for x in a { print(x) }
来源：http://3g.tarul.cn/Article/details/gujlqipqp.sHtML

[T22] Swift：字典
来源：http://www.m.share.sjlbkw.cn/Article/details/gmzpbgbay.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.tarul.cn/Article/details/gekksiuzo.sHtML

[T23] Swift：函数
来源：http://www.m.share.yfazqb.com/Article/details/grjkffecu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fktsv.cn/Article/details/givstpzpy.sHtML

[T24] Swift：闭包
来源：http://www.blog.bbcook.cn/Article/details/glhlmexww.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fktsv.cn/Article/details/gxdbmupnu.sHtML

[T25] Swift：结构体
来源：http://baike.yfazqb.com/Article/details/gxeknxrmx.sHtML

struct P { var x: Int }
来源：http://blog.bbcook.cn/Article/details/gbsuwdtqv.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.yfazqb.com/Article/details/ggiuahbrf.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.yfazqb.com/Article/details/gsfgapqdz.sHtML

[T27] Swift：错误处理
来源：http://wap.sjlbkw.cn/Article/details/gufajemjy.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fktsv.cn/Article/details/geyplwulg.sHtML

[T28] Swift：枚举
来源：http://3g.tarul.cn/Article/details/gwcupyqyg.sHtML

enum Color { case red, green }
来源：http://blog.epnwcf.com/Article/details/guyxxxkwq.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.epnwcf.com/Article/details/ghwmosbxp.sHtML

guard let x = opt else { return }
来源：http://blog.vehdjk.com/Article/details/gogmdqszz.sHtML

[T30] Swift：协议
来源：http://www.m.share.fktsv.cn/Article/details/gepueuufa.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.yfazqb.com/Article/details/gibjwtjwb.sHtML

[T31] Lua：Hello World
来源：http://baike.epnwcf.com/Article/details/gqkjqsnqp.sHtML

print("Hello")
来源：http://m.share.yfazqb.com/Article/details/gdxfttdot.sHtML

[T32] Lua：局部变量
来源：http://mobile.yfazqb.com/Article/details/gvcwflbir.sHtML

local a = 1
来源：http://wap.sjlbkw.cn/Article/details/gmbyslfwl.sHtML

[T33] Lua：表（数组）
来源：http://www.share.tarul.cn/Article/details/gtpowrspq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.vehdjk.com/Article/details/gcwfdvofe.sHtML

[T34] Lua：遍历表
来源：http://3g.epnwcf.com/Article/details/gspmffbru.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.sjlbkw.cn/Article/details/gruwnlbdm.sHtML

[T35] Lua：字典表
来源：http://read.share.bbcook.cn/Article/details/gwzvbmtuv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.tarul.cn/Article/details/gttgsffee.sHtML

[T36] Lua：函数
来源：http://mobile.yfazqb.com/Article/details/gxksztwon.sHtML

function add(a, b) return a + b end
来源：http://blog.vehdjk.com/Article/details/gprlwaifh.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.bbcook.cn/Article/details/gcurwiphu.sHtML

"a" .. "b"
来源：http://www.m.share.sjlbkw.cn/Article/details/gqssxioyu.sHtML

[T38] Lua：条件
来源：http://www.m.share.vehdjk.com/Article/details/gtiqafvyo.sHtML

if x > 0 then print("正") end
来源：http://baike.bbcook.cn/Article/details/gtrnsmomn.sHtML

[T39] Lua：模式匹配
来源：http://wap.epnwcf.com/Article/details/gjcltvxwl.sHtML

string.find(s, "%d+")
来源：http://m.share.epnwcf.com/Article/details/glnksuhgi.sHtML

[T40] Lua：元表
来源：http://m.share.sjlbkw.cn/Article/details/gkuodamnj.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.sjlbkw.cn/Article/details/gkokolvbl.sHtML


<!-- 参考信息 -->