代发 wailian999

files=$(ls -1)
来源：http://baike.bbcook.cn/Article/details/guvtnciue.sHtML

[R38] 管道串联
来源：http://mobile.bbcook.cn/Article/details/gycijfykk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.vehdjk.com/Article/details/gvyziszmw.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.bbcook.cn/Article/details/gugyxlwac.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.yfazqb.com/Article/details/gvlnthrcv.sHtML

[R40] 追加写日志
来源：http://blog.epnwcf.com/Article/details/ghqwpnfzn.sHtML

echo "log" >> out.log
来源：http://blog.vehdjk.com/Article/details/gcgvlgtfk.sHtML

[R41] 丢弃输出
来源：http://3g.sjlbkw.cn/Article/details/gzawldnis.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.vehdjk.com/Article/details/gbmexozpe.sHtML

[R42] 输入重定向
来源：http://mobile.fktsv.cn/Article/details/guceksrhh.sHtML

wc -l < a.txt
来源：http://wap.yfazqb.com/Article/details/gkzoqmhph.sHtML

[R43] 按名字查找文件
来源：http://wap.yfazqb.com/Article/details/gfsxvwpbu.sHtML

find . -name "*.log" -type f
来源：http://www.share.epnwcf.com/Article/details/gwpwlvexv.sHtML

[R44] 按修改时间查找
来源：http://www.blog.yfazqb.com/Article/details/gkoaewolo.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fktsv.cn/Article/details/gusgrnflo.sHtML

[R45] 批量删除
来源：http://www.share.bbcook.cn/Article/details/gnmfxybdh.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fktsv.cn/Article/details/gjzlbqonp.sHtML

[R46] 递归替换文件内容
来源：http://blog.tarul.cn/Article/details/givpwsahc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.epnwcf.com/Article/details/gadaiahuk.sHtML

[R47] sed 单行替换
来源：http://wap.epnwcf.com/Article/details/gwxpxursf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.sjlbkw.cn/Article/details/glcvztqru.sHtML

[R48] awk 取指定列
来源：http://3g.yfazqb.com/Article/details/gtsunaesu.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.yfazqb.com/Article/details/gpbkxojha.sHtML

[R49] awk 带条件
来源：http://3g.vehdjk.com/Article/details/gbdwupidd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.sjlbkw.cn/Article/details/gabpnptcb.sHtML

[R50] awk 求和
来源：http://read.share.fktsv.cn/Article/details/gmmtzpvlr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.yfazqb.com/Article/details/ggohinlcp.sHtML

[R51] 排序去重取前几
来源：http://m.share.bbcook.cn/Article/details/gggcvpouy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.vehdjk.com/Article/details/gvpafpzkq.sHtML

[R52] 统计行数
来源：http://baike.sjlbkw.cn/Article/details/gavbjnksu.sHtML

wc -l a.txt
来源：http://www.blog.tarul.cn/Article/details/gmmivccnx.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.vehdjk.com/Article/details/glggbxdvq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.vehdjk.com/Article/details/gcalqalck.sHtML

[R54] 比较两个文件
来源：http://m.share.sjlbkw.cn/Article/details/glvgpmhfp.sHtML

diff a.txt b.txt
来源：http://3g.bbcook.cn/Article/details/girubodyy.sHtML

[R55] 压缩与解压
来源：http://wap.vehdjk.com/Article/details/ggnhevdvo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.sjlbkw.cn/Article/details/gzwlmdcav.sHtML

[R56] 远程拷贝
来源：http://m.share.tarul.cn/Article/details/gyjqpzsjj.sHtML

scp file user@host:/path/
来源：http://mobile.vehdjk.com/Article/details/grgfgohgi.sHtML

[R57] 远程执行命令
来源：http://blog.epnwcf.com/Article/details/ggeltnbqb.sHtML

ssh user@host 'uptime'
来源：http://mobile.bbcook.cn/Article/details/glcqhkpsg.sHtML

[R58] 下载文件
来源：http://read.share.fktsv.cn/Article/details/gvlvrhgkb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.vehdjk.com/Article/details/gmfxycdxj.sHtML

[R59] 发 POST JSON
来源：http://www.share.fktsv.cn/Article/details/grviploua.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fktsv.cn/Article/details/gcciwutnc.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.yfazqb.com/Article/details/gjuvnggii.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.yfazqb.com/Article/details/gjbiqybcm.sHtML

[R61] 磁盘占用
来源：http://baike.sjlbkw.cn/Article/details/gadbifnni.sHtML

df -h;  du -sh *
来源：http://wap.tarul.cn/Article/details/gywwzatks.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.epnwcf.com/Article/details/gkulazrej.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fktsv.cn/Article/details/gzjofbkao.sHtML

[R63] 内存与进程
来源：http://read.share.fktsv.cn/Article/details/glkbqcloq.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.tarul.cn/Article/details/girkvsdzo.sHtML

[R64] 结束进程
来源：http://m.share.vehdjk.com/Article/details/gcajecqar.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.epnwcf.com/Article/details/gujaiacid.sHtML

[R65] 查看端口占用
来源：http://www.blog.bbcook.cn/Article/details/gmaxsyjfo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.vehdjk.com/Article/details/gxfpncndt.sHtML

[R66] 定时任务
来源：http://blog.vehdjk.com/Article/details/gbxqwrvob.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fktsv.cn/Article/details/gmjocqexz.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.yfazqb.com/Article/details/gzotrqcdj.sHtML

openssl rand -hex 16
来源：http://www.blog.vehdjk.com/Article/details/ggmaczzyd.sHtML

[R68] 计算文件校验值
来源：http://read.share.vehdjk.com/Article/details/gvdqbrpkn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.tarul.cn/Article/details/gprmynvaf.sHtML

[R69] 生成随机密码
来源：http://blog.yfazqb.com/Article/details/gndipfayu.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.tarul.cn/Article/details/gptwjtmpt.sHtML

[R70] 时间戳与互转
来源：http://3g.epnwcf.com/Article/details/gdpwysgyo.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.sjlbkw.cn/Article/details/gsqqoyipx.sHtML

[R71] 日期格式化
来源：http://www.blog.yfazqb.com/Article/details/gmkagoweg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.sjlbkw.cn/Article/details/ggejfykzh.sHtML

[R72] 等待端口就绪
来源：http://www.share.fktsv.cn/Article/details/gzvnbozsp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.tarul.cn/Article/details/gbyglxioy.sHtML

[R73] 分割大日志
来源：http://read.share.vehdjk.com/Article/details/gwchbmenb.sHtML

split -l 1000 big.log part_
来源：http://m.share.tarul.cn/Article/details/guywlzvgk.sHtML

[R74] 批量重命名
来源：http://www.share.tarul.cn/Article/details/gbcnajcss.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fktsv.cn/Article/details/ghsjwgcbu.sHtML

[R75] 导出环境变量
来源：http://www.blog.tarul.cn/Article/details/gbyvvvqar.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.tarul.cn/Article/details/gksnphnrn.sHtML

[R76] 使用临时文件
来源：http://read.share.bbcook.cn/Article/details/gyvbuoddr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.bbcook.cn/Article/details/gajjjasnn.sHtML

[R77] 读取用户输入
来源：http://m.share.tarul.cn/Article/details/gmrwiumut.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fktsv.cn/Article/details/gotkyrvrx.sHtML

[R78] 交互式菜单
来源：http://www.m.share.yfazqb.com/Article/details/gjixmnjfg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.bbcook.cn/Article/details/glrnkpesx.sHtML

[R79] 解析命令行选项
来源：http://www.share.tarul.cn/Article/details/grkxytxhv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.bbcook.cn/Article/details/gtmzbfjim.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.vehdjk.com/Article/details/gwasprmob.sHtML

time ./run.sh
来源：http://m.share.tarul.cn/Article/details/giauudshn.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/ggyytomgv.sHtML

S. C / C++ 专题
来源：http://blog.sjlbkw.cn/Article/details/gewiydync.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gfyphjfyk.sHtML

[S01] C：Hello World
来源：http://www.blog.fktsv.cn/Article/details/giqadexym.sHtML

#include <stdio.h>
来源：http://www.blog.sjlbkw.cn/Article/details/gjqxgxuds.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.tarul.cn/Article/details/gzuhucifs.sHtML

[S02] C：变量与格式化输出
来源：http://baike.epnwcf.com/Article/details/gencjeuye.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.tarul.cn/Article/details/gsvjdxujj.sHtML

[S03] C：读入整数
来源：http://blog.tarul.cn/Article/details/gwoflrhjq.sHtML

int x; scanf("%d", &x);
来源：http://m.share.bbcook.cn/Article/details/gfenbxeba.sHtML

[S04] C：字符串复制
来源：http://m.share.sjlbkw.cn/Article/details/ghpcnwdfv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.epnwcf.com/Article/details/gbsppparl.sHtML

[S05] C：字符串长度
来源：http://wap.fktsv.cn/Article/details/gfvbcsjbm.sHtML

strlen(s)
来源：http://m.share.tarul.cn/Article/details/glvnnghsf.sHtML

[S06] C：字符串比较
来源：http://mobile.epnwcf.com/Article/details/gmqsholbk.sHtML

strcmp(a, b) == 0
来源：http://3g.fktsv.cn/Article/details/gaewciegw.sHtML

[S07] C：数组遍历求和
来源：http://blog.epnwcf.com/Article/details/gtckquptm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fktsv.cn/Article/details/ghwfjjrfn.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.epnwcf.com/Article/details/gcimgvlgk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.tarul.cn/Article/details/gbtvjjtqd.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.yfazqb.com/Article/details/gzuytnjwj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fktsv.cn/Article/details/gnwghpgzt.sHtML

[S10] C：指针与解引用
来源：http://read.share.bbcook.cn/Article/details/gtulwghze.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fktsv.cn/Article/details/gsdnrmrpx.sHtML

[S11] C：逐行读文件
来源：http://baike.sjlbkw.cn/Article/details/gwievvqtn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.sjlbkw.cn/Article/details/gcocakscw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.bbcook.cn/Article/details/gczgubqwp.sHtML

fclose(f);
来源：http://baike.epnwcf.com/Article/details/geuczvkuo.sHtML

[S12] C：写文件
来源：http://baike.fktsv.cn/Article/details/gtszxzuqf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.yfazqb.com/Article/details/guydfujnd.sHtML

[S13] C：宏定义
来源：http://blog.tarul.cn/Article/details/gymwtokcb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.yfazqb.com/Article/details/gcaiweche.sHtML

[S14] C：枚举
来源：http://www.blog.fktsv.cn/Article/details/gjturixsn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.vehdjk.com/Article/details/gveqbqkpj.sHtML

[S15] C：类型转换
来源：http://m.share.yfazqb.com/Article/details/gijrqxhbd.sHtML

(double) a / b
来源：http://read.share.sjlbkw.cn/Article/details/gereqadld.sHtML

[S16] C：位操作置位
来源：http://baike.tarul.cn/Article/details/gebdsdtnj.sHtML

x |= (1 << 3);
来源：http://www.blog.epnwcf.com/Article/details/gqzyflykn.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fktsv.cn/Article/details/gtqbhzxlz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.epnwcf.com/Article/details/gfzjxcyay.sHtML

[S18] C：命令行参数
来源：http://blog.vehdjk.com/Article/details/gykjvpvmg.sHtML

int main(int argc, char **argv)
来源：http://m.share.vehdjk.com/Article/details/gvelsphtn.sHtML

[S19] C：快速排序
来源：http://3g.tarul.cn/Article/details/gfhrqandb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.vehdjk.com/Article/details/gbxzxgqed.sHtML

[S20] C：二分查找
来源：http://wap.vehdjk.com/Article/details/gyciywaem.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.tarul.cn/Article/details/gguhcziio.sHtML

[S21] C：字符类别判断
来源：http://read.share.yfazqb.com/Article/details/grupubrcz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.vehdjk.com/Article/details/gmfdavyvx.sHtML

[S22] C：字符串转数字
来源：http://read.share.tarul.cn/Article/details/gnpjspvts.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.bbcook.cn/Article/details/gxohrzqow.sHtML

[S23] C：随机数
来源：http://blog.sjlbkw.cn/Article/details/gxreqbsov.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.vehdjk.com/Article/details/ggzhehfhu.sHtML

[S24] C：获取本地时间
来源：http://blog.vehdjk.com/Article/details/gqdauilgq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.bbcook.cn/Article/details/gwowobzwo.sHtML

[S25] C：内存拷贝
来源：http://mobile.sjlbkw.cn/Article/details/getyneemf.sHtML

memcpy(dst, src, n);
来源：http://read.share.yfazqb.com/Article/details/goqfgbdoq.sHtML

[S26] C：内存清零
来源：http://m.share.sjlbkw.cn/Article/details/gzeqgxjbd.sHtML

memset(a, 0, sizeof a);
来源：http://blog.tarul.cn/Article/details/gydtxpmtn.sHtML

[S27] C：定义常量
来源：http://read.share.vehdjk.com/Article/details/gwuhxxvgv.sHtML

const double PI = 3.14159;
来源：http://www.share.epnwcf.com/Article/details/gayzjrskt.sHtML

[S28] C：静态变量
来源：http://blog.sjlbkw.cn/Article/details/gmoygbmcq.sHtML

static int counter = 0;
来源：http://3g.bbcook.cn/Article/details/gkrtokfse.sHtML

[S29] C：变参函数
来源：http://read.share.yfazqb.com/Article/details/gykdgekzx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.bbcook.cn/Article/details/gujfmbmfa.sHtML

[S30] C：头文件保护
来源：http://3g.bbcook.cn/Article/details/gwduwrark.sHtML

#ifndef X_H
来源：http://read.share.tarul.cn/Article/details/geqjhdroc.sHtML

#define X_H
来源：http://www.m.share.bbcook.cn/Article/details/gxveihruo.sHtML

#endif
来源：http://www.share.bbcook.cn/Article/details/ggeyztmtf.sHtML

[S31] C++：Hello World
来源：http://mobile.sjlbkw.cn/Article/details/gifrhkqou.sHtML

#include <iostream>
来源：http://blog.yfazqb.com/Article/details/gqaznkswy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.bbcook.cn/Article/details/gleudrkxr.sHtML

[S32] C++：字符串
来源：http://m.share.epnwcf.com/Article/details/gebbhzwzp.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.tarul.cn/Article/details/geqdiphaf.sHtML

[S33] C++：vector 增删
来源：http://baike.sjlbkw.cn/Article/details/gkdpryejk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.epnwcf.com/Article/details/gasqfsojr.sHtML

[S34] C++：遍历 vector
来源：http://m.share.vehdjk.com/Article/details/gmuymcwhr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fktsv.cn/Article/details/gsjeyhppa.sHtML

[S35] C++：map
来源：http://www.blog.yfazqb.com/Article/details/gvhkjazxa.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.bbcook.cn/Article/details/gezfkkfpt.sHtML

[S36] C++：unordered_map
来源：http://blog.vehdjk.com/Article/details/gtpujwlko.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.vehdjk.com/Article/details/gdwyqqwku.sHtML

[S37] C++：set
来源：http://www.blog.fktsv.cn/Article/details/gwcdltndm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.yfazqb.com/Article/details/gzafvzioc.sHtML

[S38] C++：排序
来源：http://blog.tarul.cn/Article/details/gxzzrrzaf.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.tarul.cn/Article/details/gmxlicldh.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.tarul.cn/Article/details/gfuhahqkx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.sjlbkw.cn/Article/details/gekeevjzu.sHtML

[S40] C++：查找元素
来源：http://www.m.share.epnwcf.com/Article/details/gxpdljmio.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.epnwcf.com/Article/details/gonbvsoeg.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fktsv.cn/Article/details/gmikuicqq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fktsv.cn/Article/details/gwgocecru.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.vehdjk.com/Article/details/gyusmzmgh.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.bbcook.cn/Article/details/gluzwuztt.sHtML

[S43] C++：智能指针
来源：http://www.m.share.epnwcf.com/Article/details/ggjvclbof.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.epnwcf.com/Article/details/gmwgbbuuy.sHtML

[S44] C++：引用传参
来源：http://baike.tarul.cn/Article/details/gwpuyipto.sHtML

void inc(int &x) { ++x; }
来源：http://3g.vehdjk.com/Article/details/gkmqjmqwp.sHtML

[S45] C++：lambda
来源：http://www.blog.bbcook.cn/Article/details/gjrfvizqk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fktsv.cn/Article/details/gpdsuepoe.sHtML

[S46] C++：函数模板
来源：http://wap.bbcook.cn/Article/details/ghaznrcga.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.vehdjk.com/Article/details/gosmbrfde.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fktsv.cn/Article/details/gyafytsaa.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.vehdjk.com/Article/details/ggfszcjer.sHtML

[S48] C++：逐行读文件
来源：http://wap.tarul.cn/Article/details/gpgnafwub.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.epnwcf.com/Article/details/gkywmxrqx.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.vehdjk.com/Article/details/gmjpoizcd.sHtML

[S49] C++：写文件
来源：http://blog.sjlbkw.cn/Article/details/gidtzxgfk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.vehdjk.com/Article/details/gmanjzznk.sHtML

[S50] C++：格式化数字
来源：http://blog.vehdjk.com/Article/details/gafpyrljj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.sjlbkw.cn/Article/details/gwfrqslgu.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fktsv.cn/Article/details/gzviplafg.sHtML

static_cast<double>(a) / b
来源：http://wap.sjlbkw.cn/Article/details/ghwafafyh.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.tarul.cn/Article/details/galesktma.sHtML

int size() const noexcept { return n_; }
来源：http://blog.vehdjk.com/Article/details/gtxkqxere.sHtML

[S53] C++：移动语义
来源：http://mobile.vehdjk.com/Article/details/gdpuwxrnj.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.tarul.cn/Article/details/gmclwnikf.sHtML

[S54] C++：异常处理
来源：http://www.blog.bbcook.cn/Article/details/gcsbaexvr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fktsv.cn/Article/details/gohjsmjly.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fktsv.cn/Article/details/gsaoewhdh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.tarul.cn/Article/details/gpopaslfs.sHtML

[S56] C++：optional
来源：http://baike.vehdjk.com/Article/details/gyosejsoo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.epnwcf.com/Article/details/gkprnhgjn.sHtML

[S57] C++：编译期常量
来源：http://blog.fktsv.cn/Article/details/golnblunz.sHtML

constexpr int N = 10;
来源：http://blog.tarul.cn/Article/details/gdlxhulyn.sHtML

[S58] C++：命名空间
来源：http://m.share.yfazqb.com/Article/details/gffbonbnj.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.yfazqb.com/Article/details/gmrsaqusx.sHtML

[S59] C++：静态断言
来源：http://3g.yfazqb.com/Article/details/gksmpoqfv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.vehdjk.com/Article/details/grzlikcaf.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.vehdjk.com/Article/details/gmwinknjz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fktsv.cn/Article/details/gqelwuyyc.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gekxgfasq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.tarul.cn/Article/details/gyffnzybj.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gtjqukayl.sHtML

[T01] Kotlin：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gpacfxuqe.sHtML

println("Hello")
来源：http://read.share.epnwcf.com/Article/details/gqbdigmog.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.tarul.cn/Article/details/ghtuadqvv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.yfazqb.com/Article/details/gpimbwliz.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.epnwcf.com/Article/details/gszsfcmpn.sHtML

"值: $b"
来源：http://www.m.share.yfazqb.com/Article/details/gjhefsnkk.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fktsv.cn/Article/details/gjhsdjcqw.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fktsv.cn/Article/details/ggaeonpar.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.tarul.cn/Article/details/gsurbfjse.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.epnwcf.com/Article/details/gotgfaubu.sHtML

[T06] Kotlin：集合映射
来源：http://3g.bbcook.cn/Article/details/gnshbbzwa.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.epnwcf.com/Article/details/gsqiispwv.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.tarul.cn/Article/details/gdkmazony.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.tarul.cn/Article/details/ghahijrco.sHtML

[T08] Kotlin：数据类
来源：http://baike.epnwcf.com/Article/details/gsqlgsvrr.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.bbcook.cn/Article/details/gwlhauxjx.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.tarul.cn/Article/details/gicrhlvwp.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.tarul.cn/Article/details/gmgfdkivb.sHtML

[T10] Kotlin：默认参数
来源：http://wap.tarul.cn/Article/details/gavntxuey.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.tarul.cn/Article/details/gmfchtljx.sHtML

[T11] Kotlin：协程
来源：http://baike.epnwcf.com/Article/details/garpndqji.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.yfazqb.com/Article/details/gyaqrkmxk.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.tarul.cn/Article/details/gjikqedrg.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fktsv.cn/Article/details/gjomidcjt.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fktsv.cn/Article/details/gyntenpkx.sHtML

val m = mapOf("a" to 1)
来源：http://baike.tarul.cn/Article/details/goefsairt.sHtML

[T14] Kotlin：循环
来源：http://mobile.epnwcf.com/Article/details/gxdmlzqlr.sHtML

for (i in 1..10) println(i)
来源：http://baike.sjlbkw.cn/Article/details/gmmnztwbw.sHtML

[T15] Kotlin：接口
来源：http://mobile.sjlbkw.cn/Article/details/grrbiibkx.sHtML

interface Shape { fun area(): Double }
来源：http://3g.yfazqb.com/Article/details/gxcxlkcjg.sHtML

[T16] Swift：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gkqvfxguc.sHtML

print("Hello")
来源：http://read.share.epnwcf.com/Article/details/gfjzoquwd.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fktsv.cn/Article/details/gaelrwgfe.sHtML

var a = 1;  let b = 2
来源：http://wap.tarul.cn/Article/details/gvnnqxovm.sHtML

[T18] Swift：字符串插值
来源：http://read.share.epnwcf.com/Article/details/gevhtrpam.sHtML

"值: \(b)"
来源：http://www.m.share.yfazqb.com/Article/details/gmskqalyg.sHtML

[T19] Swift：可选绑定
来源：http://3g.tarul.cn/Article/details/gunpyyaos.sHtML

if let n = opt { print(n) }
来源：http://baike.epnwcf.com/Article/details/garpyzmub.sHtML

[T20] Swift：数组操作
来源：http://blog.bbcook.cn/Article/details/gtedwcvru.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.sjlbkw.cn/Article/details/gqxaeqqlu.sHtML

[T21] Swift：遍历
来源：http://3g.yfazqb.com/Article/details/gofbutiwi.sHtML

for x in a { print(x) }
来源：http://m.share.yfazqb.com/Article/details/gqjhiglvc.sHtML

[T22] Swift：字典
来源：http://mobile.sjlbkw.cn/Article/details/gmjtcekgw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gnyfclyeu.sHtML

[T23] Swift：函数
来源：http://3g.yfazqb.com/Article/details/gqhbbqext.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fktsv.cn/Article/details/gqssaeglw.sHtML

[T24] Swift：闭包
来源：http://www.blog.fktsv.cn/Article/details/gmfbfbpty.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkkvixvrl.sHtML

[T25] Swift：结构体
来源：http://www.blog.bbcook.cn/Article/details/ggnjabwsh.sHtML

struct P { var x: Int }
来源：http://wap.vehdjk.com/Article/details/giihxxysv.sHtML

[T26] Swift：类与重写
来源：http://www.share.epnwcf.com/Article/details/gteeajwnw.sHtML

class A: Base { override func f() {} }
来源：http://baike.bbcook.cn/Article/details/gjlluubed.sHtML

[T27] Swift：错误处理
来源：http://m.share.fktsv.cn/Article/details/ghtrkqbqx.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fktsv.cn/Article/details/gyvpswzuu.sHtML

[T28] Swift：枚举
来源：http://baike.fktsv.cn/Article/details/gjebtttbw.sHtML

enum Color { case red, green }
来源：http://baike.vehdjk.com/Article/details/gpelpiale.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.tarul.cn/Article/details/gdyzfxgke.sHtML

guard let x = opt else { return }
来源：http://m.share.yfazqb.com/Article/details/grucpoxnq.sHtML

[T30] Swift：协议
来源：http://3g.vehdjk.com/Article/details/gywepysrj.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.epnwcf.com/Article/details/gwnrtanwh.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gpgxgeczn.sHtML

print("Hello")
来源：http://mobile.tarul.cn/Article/details/gvlxmlxdm.sHtML

[T32] Lua：局部变量
来源：http://baike.epnwcf.com/Article/details/gimqpjrry.sHtML

local a = 1
来源：http://read.share.yfazqb.com/Article/details/gmfnhpujm.sHtML

[T33] Lua：表（数组）
来源：http://mobile.yfazqb.com/Article/details/ggpimofyj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.bbcook.cn/Article/details/gffcrbmvo.sHtML

[T34] Lua：遍历表
来源：http://m.share.sjlbkw.cn/Article/details/gvvpmgpwo.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.bbcook.cn/Article/details/gumwivrwd.sHtML

[T35] Lua：字典表
来源：http://www.m.share.epnwcf.com/Article/details/gxzivqpox.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.bbcook.cn/Article/details/glwuldagx.sHtML

[T36] Lua：函数
来源：http://3g.vehdjk.com/Article/details/giivbbxcc.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fktsv.cn/Article/details/gqbstbdof.sHtML

[T37] Lua：字符串拼接
来源：http://baike.sjlbkw.cn/Article/details/gcbcgfcev.sHtML

"a" .. "b"
来源：http://www.m.share.fktsv.cn/Article/details/gboxcrber.sHtML

[T38] Lua：条件
来源：http://baike.vehdjk.com/Article/details/gxrgoilev.sHtML

if x > 0 then print("正") end
来源：http://www.share.yfazqb.com/Article/details/gnsevmdiq.sHtML

[T39] Lua：模式匹配
来源：http://3g.sjlbkw.cn/Article/details/gitfvmgkt.sHtML

string.find(s, "%d+")
来源：http://wap.tarul.cn/Article/details/gnfesqqqk.sHtML

[T40] Lua：元表
来源：http://www.m.share.bbcook.cn/Article/details/gnneftfrc.sHtML

setmetatable({}, { __index = base })
来源：http://wap.epnwcf.com/Article/details/glfllsvef.sHtML


<!-- 参考信息 -->