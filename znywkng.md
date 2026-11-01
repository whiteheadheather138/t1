代发 wailian999

files=$(ls -1)
来源：http://www.share.sjlbkw.cn/Article/details/gnnufoupe.sHtML

[R38] 管道串联
来源：http://www.m.share.yfazqb.com/Article/details/gzkjyvtky.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.sjlbkw.cn/Article/details/gllktlggm.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.epnwcf.com/Article/details/gbqzgqaus.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.yfazqb.com/Article/details/govargnxa.sHtML

[R40] 追加写日志
来源：http://baike.epnwcf.com/Article/details/giuzhspch.sHtML

echo "log" >> out.log
来源：http://www.share.vehdjk.com/Article/details/gmiaprtqo.sHtML

[R41] 丢弃输出
来源：http://blog.epnwcf.com/Article/details/gebxudobl.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.bbcook.cn/Article/details/ghlxmreyh.sHtML

[R42] 输入重定向
来源：http://blog.bbcook.cn/Article/details/gklpokcap.sHtML

wc -l < a.txt
来源：http://www.m.share.bbcook.cn/Article/details/gtzrbjcsl.sHtML

[R43] 按名字查找文件
来源：http://m.share.sjlbkw.cn/Article/details/girnfijcw.sHtML

find . -name "*.log" -type f
来源：http://wap.epnwcf.com/Article/details/gmgusjwss.sHtML

[R44] 按修改时间查找
来源：http://blog.fktsv.cn/Article/details/gqnrddxoh.sHtML

find . -mtime -7 -type f
来源：http://mobile.epnwcf.com/Article/details/gihlibbmu.sHtML

[R45] 批量删除
来源：http://mobile.yfazqb.com/Article/details/goaaiokwp.sHtML

find . -name "*.tmp" -delete
来源：http://blog.vehdjk.com/Article/details/grrrcmptq.sHtML

[R46] 递归替换文件内容
来源：http://3g.vehdjk.com/Article/details/gprbrmxzo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fktsv.cn/Article/details/gmqjxgrnz.sHtML

[R47] sed 单行替换
来源：http://m.share.fktsv.cn/Article/details/gxealbhwg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.epnwcf.com/Article/details/gruerpgba.sHtML

[R48] awk 取指定列
来源：http://www.share.yfazqb.com/Article/details/gcagwkvrg.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.bbcook.cn/Article/details/gvqquegfx.sHtML

[R49] awk 带条件
来源：http://www.m.share.bbcook.cn/Article/details/gomykasup.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fktsv.cn/Article/details/gynxnfhrj.sHtML

[R50] awk 求和
来源：http://baike.fktsv.cn/Article/details/gpaecwlzz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.epnwcf.com/Article/details/gdqjegdaf.sHtML

[R51] 排序去重取前几
来源：http://baike.fktsv.cn/Article/details/gmntilmcp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.yfazqb.com/Article/details/gtpvdylrk.sHtML

[R52] 统计行数
来源：http://m.share.sjlbkw.cn/Article/details/gfndrwhwc.sHtML

wc -l a.txt
来源：http://wap.epnwcf.com/Article/details/glgswryxw.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.yfazqb.com/Article/details/gsytowveb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.vehdjk.com/Article/details/ggbyiswip.sHtML

[R54] 比较两个文件
来源：http://baike.tarul.cn/Article/details/ggziqdzen.sHtML

diff a.txt b.txt
来源：http://www.m.share.tarul.cn/Article/details/gujqbwgsn.sHtML

[R55] 压缩与解压
来源：http://wap.epnwcf.com/Article/details/ghqrucrgu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.bbcook.cn/Article/details/gbdlxmkcb.sHtML

[R56] 远程拷贝
来源：http://www.m.share.epnwcf.com/Article/details/gdnxnsmxl.sHtML

scp file user@host:/path/
来源：http://m.share.yfazqb.com/Article/details/gevytmcop.sHtML

[R57] 远程执行命令
来源：http://baike.sjlbkw.cn/Article/details/gdtwldxdg.sHtML

ssh user@host 'uptime'
来源：http://mobile.bbcook.cn/Article/details/gjdwqtlgy.sHtML

[R58] 下载文件
来源：http://blog.bbcook.cn/Article/details/gqaitqfef.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.sjlbkw.cn/Article/details/gctwofvgn.sHtML

[R59] 发 POST JSON
来源：http://m.share.fktsv.cn/Article/details/gievvfuzr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.bbcook.cn/Article/details/gkujmhhnp.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fktsv.cn/Article/details/gjifmsksz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.vehdjk.com/Article/details/grayqelqf.sHtML

[R61] 磁盘占用
来源：http://www.blog.fktsv.cn/Article/details/gsdsaegpp.sHtML

df -h;  du -sh *
来源：http://www.blog.yfazqb.com/Article/details/geamyjrpc.sHtML

[R62] 找最占空间的文件
来源：http://m.share.vehdjk.com/Article/details/gxjhylzfe.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.tarul.cn/Article/details/gvupsdhxd.sHtML

[R63] 内存与进程
来源：http://3g.bbcook.cn/Article/details/guzkktncx.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.sjlbkw.cn/Article/details/ggxkkdqme.sHtML

[R64] 结束进程
来源：http://read.share.sjlbkw.cn/Article/details/gzuvisttw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fktsv.cn/Article/details/gnvhbbhjw.sHtML

[R65] 查看端口占用
来源：http://read.share.tarul.cn/Article/details/gjuzowmrw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.bbcook.cn/Article/details/gvqigxqjl.sHtML

[R66] 定时任务
来源：http://m.share.bbcook.cn/Article/details/gcqribsno.sHtML

crontab -e;  crontab -l
来源：http://baike.fktsv.cn/Article/details/ggnilnxdn.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fktsv.cn/Article/details/gvoqndloe.sHtML

openssl rand -hex 16
来源：http://blog.tarul.cn/Article/details/gjhvyfckb.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.vehdjk.com/Article/details/gfpmratyu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fktsv.cn/Article/details/gnfzzhhpa.sHtML

[R69] 生成随机密码
来源：http://m.share.bbcook.cn/Article/details/gfvmnuibg.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.yfazqb.com/Article/details/gkwxgptnl.sHtML

[R70] 时间戳与互转
来源：http://blog.vehdjk.com/Article/details/giokzkxfc.sHtML

date +%s;  date -d @1700000000
来源：http://wap.sjlbkw.cn/Article/details/gblwzotss.sHtML

[R71] 日期格式化
来源：http://m.share.yfazqb.com/Article/details/goqwmztfb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.epnwcf.com/Article/details/ghmmaunzl.sHtML

[R72] 等待端口就绪
来源：http://read.share.vehdjk.com/Article/details/gqavubgul.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.bbcook.cn/Article/details/gufdrsalq.sHtML

[R73] 分割大日志
来源：http://www.m.share.tarul.cn/Article/details/gpduqivpl.sHtML

split -l 1000 big.log part_
来源：http://3g.yfazqb.com/Article/details/guemqvliq.sHtML

[R74] 批量重命名
来源：http://3g.epnwcf.com/Article/details/guntgcgse.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.vehdjk.com/Article/details/golmlnojh.sHtML

[R75] 导出环境变量
来源：http://mobile.tarul.cn/Article/details/gqvixoczf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.tarul.cn/Article/details/gxyjdpwig.sHtML

[R76] 使用临时文件
来源：http://blog.tarul.cn/Article/details/gusrpadms.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fktsv.cn/Article/details/gqmjfzuxt.sHtML

[R77] 读取用户输入
来源：http://mobile.epnwcf.com/Article/details/guizdzjsa.sHtML

read -rp "请输入: " ans
来源：http://www.blog.sjlbkw.cn/Article/details/gmveravqy.sHtML

[R78] 交互式菜单
来源：http://www.m.share.yfazqb.com/Article/details/gpmjojntv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.tarul.cn/Article/details/gppbbhsfb.sHtML

[R79] 解析命令行选项
来源：http://baike.epnwcf.com/Article/details/gsbuklqsc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.tarul.cn/Article/details/ganrqsunr.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.vehdjk.com/Article/details/grzvpqlzy.sHtML

time ./run.sh
来源：http://mobile.tarul.cn/Article/details/gbqfzpyuy.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/geptphwgk.sHtML

S. C / C++ 专题
来源：http://mobile.epnwcf.com/Article/details/gnpfadbpd.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gfpxaveyx.sHtML

[S01] C：Hello World
来源：http://blog.yfazqb.com/Article/details/gnfifsvfp.sHtML

#include <stdio.h>
来源：http://www.share.tarul.cn/Article/details/goivxiyjv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.sjlbkw.cn/Article/details/gckwfxkkm.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.yfazqb.com/Article/details/gbadsrqjk.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.epnwcf.com/Article/details/gyhldzlwg.sHtML

[S03] C：读入整数
来源：http://wap.epnwcf.com/Article/details/gsjkekwna.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fktsv.cn/Article/details/goqhoykpe.sHtML

[S04] C：字符串复制
来源：http://blog.epnwcf.com/Article/details/gcqljffyw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.sjlbkw.cn/Article/details/gqxfeyzav.sHtML

[S05] C：字符串长度
来源：http://mobile.tarul.cn/Article/details/glrxbswaf.sHtML

strlen(s)
来源：http://3g.vehdjk.com/Article/details/gbossbkcr.sHtML

[S06] C：字符串比较
来源：http://m.share.epnwcf.com/Article/details/gewbfekpu.sHtML

strcmp(a, b) == 0
来源：http://baike.yfazqb.com/Article/details/grhfdrpxx.sHtML

[S07] C：数组遍历求和
来源：http://mobile.bbcook.cn/Article/details/gwdvxpeyv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fktsv.cn/Article/details/gsgkvjjsv.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.sjlbkw.cn/Article/details/gkykdvmzn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.bbcook.cn/Article/details/gcbkbqipq.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.epnwcf.com/Article/details/gplzbipjf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.vehdjk.com/Article/details/gxmpnscoi.sHtML

[S10] C：指针与解引用
来源：http://www.share.sjlbkw.cn/Article/details/gplaprikz.sHtML

int *p = &a;  *p = 5;
来源：http://wap.tarul.cn/Article/details/gmrlnhbbl.sHtML

[S11] C：逐行读文件
来源：http://mobile.sjlbkw.cn/Article/details/gsoaaakmm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.epnwcf.com/Article/details/gakhxviiy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.epnwcf.com/Article/details/gipcvdfih.sHtML

fclose(f);
来源：http://m.share.sjlbkw.cn/Article/details/geqpwhria.sHtML

[S12] C：写文件
来源：http://read.share.yfazqb.com/Article/details/gtvxapjcs.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.vehdjk.com/Article/details/gzlbkmsla.sHtML

[S13] C：宏定义
来源：http://baike.vehdjk.com/Article/details/grlydzhhg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.tarul.cn/Article/details/gnylscjvt.sHtML

[S14] C：枚举
来源：http://wap.bbcook.cn/Article/details/gsbubiccl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.tarul.cn/Article/details/gpssyggyn.sHtML

[S15] C：类型转换
来源：http://mobile.yfazqb.com/Article/details/gteuhesjg.sHtML

(double) a / b
来源：http://wap.tarul.cn/Article/details/ghlfezcyq.sHtML

[S16] C：位操作置位
来源：http://read.share.yfazqb.com/Article/details/glinucrmh.sHtML

x |= (1 << 3);
来源：http://wap.vehdjk.com/Article/details/gdcyfbjeh.sHtML

[S17] C：安全拼接字符串
来源：http://wap.sjlbkw.cn/Article/details/gzlygnzre.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fktsv.cn/Article/details/gksezlzxt.sHtML

[S18] C：命令行参数
来源：http://www.blog.bbcook.cn/Article/details/ggtrnwdyy.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggtwiocef.sHtML

[S19] C：快速排序
来源：http://www.m.share.sjlbkw.cn/Article/details/gottrppga.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.sjlbkw.cn/Article/details/gaommcypj.sHtML

[S20] C：二分查找
来源：http://www.blog.yfazqb.com/Article/details/ggfzmkswg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.tarul.cn/Article/details/guybpvghh.sHtML

[S21] C：字符类别判断
来源：http://www.share.epnwcf.com/Article/details/gdmdypgkh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.tarul.cn/Article/details/ghbnznjme.sHtML

[S22] C：字符串转数字
来源：http://read.share.fktsv.cn/Article/details/gonyykheh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.bbcook.cn/Article/details/gaswcoegy.sHtML

[S23] C：随机数
来源：http://wap.tarul.cn/Article/details/gvrqjpzyq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.epnwcf.com/Article/details/gtbngfuar.sHtML

[S24] C：获取本地时间
来源：http://www.share.tarul.cn/Article/details/gztzydyfk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.yfazqb.com/Article/details/gtltnsjaq.sHtML

[S25] C：内存拷贝
来源：http://baike.bbcook.cn/Article/details/grcsinaxd.sHtML

memcpy(dst, src, n);
来源：http://3g.fktsv.cn/Article/details/guufxtbaz.sHtML

[S26] C：内存清零
来源：http://baike.tarul.cn/Article/details/gvyodckxt.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.yfazqb.com/Article/details/gmgsbvalf.sHtML

[S27] C：定义常量
来源：http://www.share.epnwcf.com/Article/details/gliyblhwc.sHtML

const double PI = 3.14159;
来源：http://read.share.vehdjk.com/Article/details/glzhtwpwd.sHtML

[S28] C：静态变量
来源：http://baike.epnwcf.com/Article/details/gokymrafs.sHtML

static int counter = 0;
来源：http://m.share.sjlbkw.cn/Article/details/gdgokbryu.sHtML

[S29] C：变参函数
来源：http://mobile.bbcook.cn/Article/details/gcurfxuqn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.vehdjk.com/Article/details/gpwngoyeg.sHtML

[S30] C：头文件保护
来源：http://read.share.vehdjk.com/Article/details/ggicilbra.sHtML

#ifndef X_H
来源：http://blog.yfazqb.com/Article/details/gxmtdufgg.sHtML

#define X_H
来源：http://read.share.tarul.cn/Article/details/gfjhexyor.sHtML

#endif
来源：http://wap.bbcook.cn/Article/details/gfzvsyjxa.sHtML

[S31] C++：Hello World
来源：http://wap.epnwcf.com/Article/details/geyhhiimu.sHtML

#include <iostream>
来源：http://read.share.epnwcf.com/Article/details/gdoxurxuy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.yfazqb.com/Article/details/guhdjkoev.sHtML

[S32] C++：字符串
来源：http://wap.fktsv.cn/Article/details/gwmffhisc.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.vehdjk.com/Article/details/gsknmytqh.sHtML

[S33] C++：vector 增删
来源：http://blog.bbcook.cn/Article/details/gdahnbxju.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.yfazqb.com/Article/details/ggnkrjwmn.sHtML

[S34] C++：遍历 vector
来源：http://www.share.tarul.cn/Article/details/gfdxnsrly.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.yfazqb.com/Article/details/giykttdtn.sHtML

[S35] C++：map
来源：http://m.share.tarul.cn/Article/details/gmhszrmsu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.vehdjk.com/Article/details/geoykiqvc.sHtML

[S36] C++：unordered_map
来源：http://read.share.yfazqb.com/Article/details/gawtnifbn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fktsv.cn/Article/details/gvmsidxug.sHtML

[S37] C++：set
来源：http://www.share.bbcook.cn/Article/details/gbbrkdatb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.bbcook.cn/Article/details/gvntjjimr.sHtML

[S38] C++：排序
来源：http://www.blog.epnwcf.com/Article/details/gnobnpbuk.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fktsv.cn/Article/details/gpowhcdye.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.yfazqb.com/Article/details/gxorfftxn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.epnwcf.com/Article/details/glkobeezb.sHtML

[S40] C++：查找元素
来源：http://3g.sjlbkw.cn/Article/details/gfqtawrpn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.tarul.cn/Article/details/gdmzmqtxg.sHtML

[S41] C++：类与构造函数
来源：http://3g.sjlbkw.cn/Article/details/gjvbeeadh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.bbcook.cn/Article/details/gnniwvqgj.sHtML

[S42] C++：继承与虚函数
来源：http://baike.yfazqb.com/Article/details/gfdalinmb.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.vehdjk.com/Article/details/groaxtdsb.sHtML

[S43] C++：智能指针
来源：http://read.share.fktsv.cn/Article/details/gwnvznxgv.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fktsv.cn/Article/details/gcqxmihmg.sHtML

[S44] C++：引用传参
来源：http://read.share.bbcook.cn/Article/details/grbjefgsx.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.yfazqb.com/Article/details/ggtnpjfbu.sHtML

[S45] C++：lambda
来源：http://read.share.sjlbkw.cn/Article/details/gdlawqvor.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.yfazqb.com/Article/details/gjydgialf.sHtML

[S46] C++：函数模板
来源：http://blog.sjlbkw.cn/Article/details/gyuhfypct.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.epnwcf.com/Article/details/giggolcer.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.vehdjk.com/Article/details/gpbvmamvr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fktsv.cn/Article/details/gwkeibsgv.sHtML

[S48] C++：逐行读文件
来源：http://read.share.vehdjk.com/Article/details/gixegcvkv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.epnwcf.com/Article/details/ggjwzbuzm.sHtML

while (std::getline(in, line)) { }
来源：http://baike.bbcook.cn/Article/details/gjifihnaf.sHtML

[S49] C++：写文件
来源：http://www.blog.bbcook.cn/Article/details/gzjvatsvs.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.vehdjk.com/Article/details/gfdmbnxba.sHtML

[S50] C++：格式化数字
来源：http://read.share.bbcook.cn/Article/details/ggyitqyhl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.vehdjk.com/Article/details/gyvgkkuyw.sHtML

[S51] C++：显式类型转换
来源：http://3g.vehdjk.com/Article/details/gccutzwbv.sHtML

static_cast<double>(a) / b
来源：http://m.share.vehdjk.com/Article/details/gcxyfqhmj.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.epnwcf.com/Article/details/gfufrmefk.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.yfazqb.com/Article/details/gvbfrffwf.sHtML

[S53] C++：移动语义
来源：http://www.m.share.yfazqb.com/Article/details/gjumtrbev.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.sjlbkw.cn/Article/details/gmusnerzw.sHtML

[S54] C++：异常处理
来源：http://www.m.share.epnwcf.com/Article/details/gywewtfyl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.epnwcf.com/Article/details/gbzmvemzx.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.bbcook.cn/Article/details/gauildrxs.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.vehdjk.com/Article/details/gucjedtiw.sHtML

[S56] C++：optional
来源：http://3g.fktsv.cn/Article/details/ghydgrzgz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.sjlbkw.cn/Article/details/gkphesgnh.sHtML

[S57] C++：编译期常量
来源：http://3g.vehdjk.com/Article/details/gavwxneaq.sHtML

constexpr int N = 10;
来源：http://mobile.sjlbkw.cn/Article/details/gioolloid.sHtML

[S58] C++：命名空间
来源：http://www.m.share.tarul.cn/Article/details/gvfqledvw.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.bbcook.cn/Article/details/gnzasmeyv.sHtML

[S59] C++：静态断言
来源：http://read.share.vehdjk.com/Article/details/gallimhhg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.tarul.cn/Article/details/gwrjgvkpl.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.bbcook.cn/Article/details/gngmuowbf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.bbcook.cn/Article/details/gegljueot.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gixfkqhlj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.epnwcf.com/Article/details/gkwytaeig.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/grjzddbfv.sHtML

[T01] Kotlin：Hello World
来源：http://3g.vehdjk.com/Article/details/gqifwccoy.sHtML

println("Hello")
来源：http://baike.vehdjk.com/Article/details/gfspdmwjl.sHtML

[T02] Kotlin：变量
来源：http://3g.yfazqb.com/Article/details/ghylbujax.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.tarul.cn/Article/details/giqdhynbj.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fktsv.cn/Article/details/geiyfryny.sHtML

"值: $b"
来源：http://m.share.fktsv.cn/Article/details/gzganzrlb.sHtML

[T04] Kotlin：空安全
来源：http://blog.sjlbkw.cn/Article/details/gncydcbct.sHtML

val n: String? = null;  n?.length
来源：http://wap.epnwcf.com/Article/details/gcdzydphf.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.bbcook.cn/Article/details/gpstdovaf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.yfazqb.com/Article/details/grblucbmz.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.bbcook.cn/Article/details/gvbyjewln.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.bbcook.cn/Article/details/grjzvyxkc.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.epnwcf.com/Article/details/ggkclttzu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.bbcook.cn/Article/details/gxkboielz.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fktsv.cn/Article/details/gqamevzqr.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.sjlbkw.cn/Article/details/gvcjvrhui.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.epnwcf.com/Article/details/gobpyugiw.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.vehdjk.com/Article/details/gmwjxmkgp.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.tarul.cn/Article/details/gmscyykly.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.bbcook.cn/Article/details/gldqrzhuc.sHtML

[T11] Kotlin：协程
来源：http://www.blog.yfazqb.com/Article/details/gebtdbclq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.vehdjk.com/Article/details/gyihqurwy.sHtML

[T12] Kotlin：解构声明
来源：http://3g.bbcook.cn/Article/details/gyghurhpq.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.yfazqb.com/Article/details/gthwfritt.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.bbcook.cn/Article/details/gbsogblwh.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fktsv.cn/Article/details/gghjvoexh.sHtML

[T14] Kotlin：循环
来源：http://m.share.yfazqb.com/Article/details/gopxqdnng.sHtML

for (i in 1..10) println(i)
来源：http://www.share.bbcook.cn/Article/details/gzizpzfqt.sHtML

[T15] Kotlin：接口
来源：http://www.share.vehdjk.com/Article/details/gfjqabetf.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.yfazqb.com/Article/details/gqdysobmo.sHtML

[T16] Swift：Hello World
来源：http://www.blog.bbcook.cn/Article/details/gsxwlqged.sHtML

print("Hello")
来源：http://baike.tarul.cn/Article/details/gzsxtbgul.sHtML

[T17] Swift：变量与常量
来源：http://read.share.epnwcf.com/Article/details/gxlhxtnae.sHtML

var a = 1;  let b = 2
来源：http://m.share.bbcook.cn/Article/details/ghreugdfq.sHtML

[T18] Swift：字符串插值
来源：http://wap.fktsv.cn/Article/details/gnkpuuiiq.sHtML

"值: \(b)"
来源：http://www.m.share.fktsv.cn/Article/details/giluhxhxi.sHtML

[T19] Swift：可选绑定
来源：http://baike.fktsv.cn/Article/details/gvpojothn.sHtML

if let n = opt { print(n) }
来源：http://www.blog.sjlbkw.cn/Article/details/gacigtoqw.sHtML

[T20] Swift：数组操作
来源：http://www.share.bbcook.cn/Article/details/gfcyrwsfj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.vehdjk.com/Article/details/gvxfqasgi.sHtML

[T21] Swift：遍历
来源：http://blog.fktsv.cn/Article/details/ghjvkhhty.sHtML

for x in a { print(x) }
来源：http://mobile.vehdjk.com/Article/details/gvibzzmwu.sHtML

[T22] Swift：字典
来源：http://blog.tarul.cn/Article/details/gizbljutw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.epnwcf.com/Article/details/gsrobbdiv.sHtML

[T23] Swift：函数
来源：http://read.share.bbcook.cn/Article/details/gxzktxbbb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.tarul.cn/Article/details/gyuypfinq.sHtML

[T24] Swift：闭包
来源：http://www.m.share.sjlbkw.cn/Article/details/gnydrjycz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.yfazqb.com/Article/details/gmvyckqqm.sHtML

[T25] Swift：结构体
来源：http://www.blog.sjlbkw.cn/Article/details/grqxxltcf.sHtML

struct P { var x: Int }
来源：http://m.share.epnwcf.com/Article/details/gyyqjsdaz.sHtML

[T26] Swift：类与重写
来源：http://baike.sjlbkw.cn/Article/details/gfrhplogk.sHtML

class A: Base { override func f() {} }
来源：http://mobile.bbcook.cn/Article/details/gnqgfzewt.sHtML

[T27] Swift：错误处理
来源：http://blog.fktsv.cn/Article/details/gukbdsmwz.sHtML

do { try f() } catch { print(error) }
来源：http://3g.sjlbkw.cn/Article/details/gnvvejtxd.sHtML

[T28] Swift：枚举
来源：http://www.share.sjlbkw.cn/Article/details/gfzybshnp.sHtML

enum Color { case red, green }
来源：http://m.share.bbcook.cn/Article/details/ghleoyugf.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.tarul.cn/Article/details/gcxcrswyt.sHtML

guard let x = opt else { return }
来源：http://m.share.bbcook.cn/Article/details/grbgdftcq.sHtML

[T30] Swift：协议
来源：http://www.m.share.fktsv.cn/Article/details/gbckxiixn.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.sjlbkw.cn/Article/details/gtjzonykd.sHtML

[T31] Lua：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gndlyvnox.sHtML

print("Hello")
来源：http://3g.vehdjk.com/Article/details/gydzzqesa.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.tarul.cn/Article/details/gpnkejztg.sHtML

local a = 1
来源：http://wap.epnwcf.com/Article/details/gmwhiegkj.sHtML

[T33] Lua：表（数组）
来源：http://read.share.tarul.cn/Article/details/gccozydui.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.epnwcf.com/Article/details/gqbglxubr.sHtML

[T34] Lua：遍历表
来源：http://3g.vehdjk.com/Article/details/gmrpbaeqo.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.vehdjk.com/Article/details/ggalvffwf.sHtML

[T35] Lua：字典表
来源：http://m.share.sjlbkw.cn/Article/details/gejnxfmry.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.tarul.cn/Article/details/gftyddpyz.sHtML

[T36] Lua：函数
来源：http://baike.epnwcf.com/Article/details/ggihinrvo.sHtML

function add(a, b) return a + b end
来源：http://www.blog.epnwcf.com/Article/details/gjrkfsikr.sHtML

[T37] Lua：字符串拼接
来源：http://wap.vehdjk.com/Article/details/gkgmoswzd.sHtML

"a" .. "b"
来源：http://m.share.fktsv.cn/Article/details/gorlxluxb.sHtML

[T38] Lua：条件
来源：http://blog.vehdjk.com/Article/details/gpouiuxcf.sHtML

if x > 0 then print("正") end
来源：http://read.share.vehdjk.com/Article/details/gqnbydbwp.sHtML

[T39] Lua：模式匹配
来源：http://www.share.bbcook.cn/Article/details/girnuvdkl.sHtML

string.find(s, "%d+")
来源：http://3g.yfazqb.com/Article/details/gisdocjfn.sHtML

[T40] Lua：元表
来源：http://baike.bbcook.cn/Article/details/gfmtksnur.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.vehdjk.com/Article/details/gckdqlmgb.sHtML


<!-- 参考信息 -->