代发 wailian999

files=$(ls -1)
来源：http://blog.bbcook.cn/Article/details/gcfzvfcfc.sHtML

[R38] 管道串联
来源：http://www.blog.tarul.cn/Article/details/gljrdvdca.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.yfazqb.com/Article/details/grpjhiwoi.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.sjlbkw.cn/Article/details/gwcsgwtit.sHtML

cmd > out.log 2>&1
来源：http://www.blog.vehdjk.com/Article/details/gcnezonws.sHtML

[R40] 追加写日志
来源：http://www.m.share.epnwcf.com/Article/details/garprktib.sHtML

echo "log" >> out.log
来源：http://blog.yfazqb.com/Article/details/gmlaehbpk.sHtML

[R41] 丢弃输出
来源：http://blog.vehdjk.com/Article/details/gkagbetht.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fktsv.cn/Article/details/gdokytohn.sHtML

[R42] 输入重定向
来源：http://www.blog.vehdjk.com/Article/details/gfftirrhx.sHtML

wc -l < a.txt
来源：http://read.share.sjlbkw.cn/Article/details/gemhdubsl.sHtML

[R43] 按名字查找文件
来源：http://m.share.yfazqb.com/Article/details/guoxvuota.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fktsv.cn/Article/details/gvkiqnryo.sHtML

[R44] 按修改时间查找
来源：http://read.share.tarul.cn/Article/details/glaqvljbl.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.bbcook.cn/Article/details/gabdfrnhs.sHtML

[R45] 批量删除
来源：http://wap.vehdjk.com/Article/details/gncckxfbr.sHtML

find . -name "*.tmp" -delete
来源：http://baike.epnwcf.com/Article/details/gfpmvnvtf.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.vehdjk.com/Article/details/glfafhlln.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fktsv.cn/Article/details/grasslwcb.sHtML

[R47] sed 单行替换
来源：http://www.blog.sjlbkw.cn/Article/details/giopcbmkc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.tarul.cn/Article/details/gvdpastii.sHtML

[R48] awk 取指定列
来源：http://mobile.yfazqb.com/Article/details/goyiihtmw.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.vehdjk.com/Article/details/gqfxbifea.sHtML

[R49] awk 带条件
来源：http://m.share.epnwcf.com/Article/details/gzrhbdnam.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.bbcook.cn/Article/details/gaezsuugf.sHtML

[R50] awk 求和
来源：http://m.share.sjlbkw.cn/Article/details/gafwnxzqq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.yfazqb.com/Article/details/gyxflyevi.sHtML

[R51] 排序去重取前几
来源：http://read.share.yfazqb.com/Article/details/gfsujiena.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.vehdjk.com/Article/details/goqvvkoqz.sHtML

[R52] 统计行数
来源：http://3g.vehdjk.com/Article/details/ggivradsd.sHtML

wc -l a.txt
来源：http://read.share.vehdjk.com/Article/details/glforrlwy.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.vehdjk.com/Article/details/grxkqjisu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.epnwcf.com/Article/details/guqqlqcyd.sHtML

[R54] 比较两个文件
来源：http://baike.vehdjk.com/Article/details/gixluhtir.sHtML

diff a.txt b.txt
来源：http://www.m.share.fktsv.cn/Article/details/gnmrzxduv.sHtML

[R55] 压缩与解压
来源：http://blog.sjlbkw.cn/Article/details/gqrjcdtmf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fktsv.cn/Article/details/gtnrxsquh.sHtML

[R56] 远程拷贝
来源：http://3g.bbcook.cn/Article/details/grglndpjo.sHtML

scp file user@host:/path/
来源：http://www.blog.epnwcf.com/Article/details/gmwkicryh.sHtML

[R57] 远程执行命令
来源：http://www.blog.sjlbkw.cn/Article/details/ghnaxkcpj.sHtML

ssh user@host 'uptime'
来源：http://baike.sjlbkw.cn/Article/details/gzewytatq.sHtML

[R58] 下载文件
来源：http://mobile.epnwcf.com/Article/details/grxhfbjiv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.vehdjk.com/Article/details/gfbebtpfh.sHtML

[R59] 发 POST JSON
来源：http://www.share.epnwcf.com/Article/details/gfeeeeeio.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.sjlbkw.cn/Article/details/gxpdhqsfp.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.yfazqb.com/Article/details/gozibrdfx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.tarul.cn/Article/details/gzcydhhwk.sHtML

[R61] 磁盘占用
来源：http://read.share.sjlbkw.cn/Article/details/ggcueshlc.sHtML

df -h;  du -sh *
来源：http://baike.vehdjk.com/Article/details/guyovatjc.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.sjlbkw.cn/Article/details/gygufzfts.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.tarul.cn/Article/details/gpypvbfwt.sHtML

[R63] 内存与进程
来源：http://mobile.epnwcf.com/Article/details/ghzfpdpyd.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.sjlbkw.cn/Article/details/ghyryljaj.sHtML

[R64] 结束进程
来源：http://3g.sjlbkw.cn/Article/details/gppwktwdw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.sjlbkw.cn/Article/details/gwhfnsuoh.sHtML

[R65] 查看端口占用
来源：http://www.share.epnwcf.com/Article/details/grvuempje.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fktsv.cn/Article/details/gwiwnywyo.sHtML

[R66] 定时任务
来源：http://baike.tarul.cn/Article/details/gamibewrq.sHtML

crontab -e;  crontab -l
来源：http://m.share.bbcook.cn/Article/details/gmjrqmppf.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.yfazqb.com/Article/details/gaoqhdpfa.sHtML

openssl rand -hex 16
来源：http://read.share.bbcook.cn/Article/details/gunmubbxx.sHtML

[R68] 计算文件校验值
来源：http://mobile.vehdjk.com/Article/details/gdnhzwwtr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.yfazqb.com/Article/details/gnafhtubf.sHtML

[R69] 生成随机密码
来源：http://read.share.bbcook.cn/Article/details/gzwugybkb.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.tarul.cn/Article/details/gvthcknwp.sHtML

[R70] 时间戳与互转
来源：http://m.share.fktsv.cn/Article/details/gurvvmwzi.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.sjlbkw.cn/Article/details/ggtxwsgnx.sHtML

[R71] 日期格式化
来源：http://www.m.share.epnwcf.com/Article/details/ghcyeawlg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.tarul.cn/Article/details/gfjrerubx.sHtML

[R72] 等待端口就绪
来源：http://blog.tarul.cn/Article/details/gnzsjcjqj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.yfazqb.com/Article/details/gtffxtrbx.sHtML

[R73] 分割大日志
来源：http://read.share.sjlbkw.cn/Article/details/geavyoeza.sHtML

split -l 1000 big.log part_
来源：http://read.share.tarul.cn/Article/details/guhtonrug.sHtML

[R74] 批量重命名
来源：http://read.share.epnwcf.com/Article/details/galnqfqyq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.yfazqb.com/Article/details/glrvsmjfd.sHtML

[R75] 导出环境变量
来源：http://www.share.fktsv.cn/Article/details/gwcdufowt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.epnwcf.com/Article/details/gdwmncwyr.sHtML

[R76] 使用临时文件
来源：http://mobile.sjlbkw.cn/Article/details/gykfbdxmk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.bbcook.cn/Article/details/gqvtcspgq.sHtML

[R77] 读取用户输入
来源：http://3g.vehdjk.com/Article/details/gagbkjxah.sHtML

read -rp "请输入: " ans
来源：http://wap.sjlbkw.cn/Article/details/glehrhaeh.sHtML

[R78] 交互式菜单
来源：http://www.blog.yfazqb.com/Article/details/gkqcbbqpz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fktsv.cn/Article/details/gffzvxtdf.sHtML

[R79] 解析命令行选项
来源：http://www.blog.bbcook.cn/Article/details/gbbcfvevm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.sjlbkw.cn/Article/details/ggjoofibf.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.sjlbkw.cn/Article/details/gorjqdlvn.sHtML

time ./run.sh
来源：http://mobile.sjlbkw.cn/Article/details/gckuwvymk.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/glputxkvf.sHtML

S. C / C++ 专题
来源：http://wap.yfazqb.com/Article/details/gbghnjgff.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gpizdsqzp.sHtML

[S01] C：Hello World
来源：http://m.share.tarul.cn/Article/details/ggdygonfh.sHtML

#include <stdio.h>
来源：http://www.m.share.yfazqb.com/Article/details/grdhyqams.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.vehdjk.com/Article/details/gbmycsncp.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.tarul.cn/Article/details/ggkncbvcy.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.vehdjk.com/Article/details/ggljossml.sHtML

[S03] C：读入整数
来源：http://m.share.yfazqb.com/Article/details/ginezlyqw.sHtML

int x; scanf("%d", &x);
来源：http://m.share.tarul.cn/Article/details/gysbtpdsz.sHtML

[S04] C：字符串复制
来源：http://blog.yfazqb.com/Article/details/gaexarfme.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.sjlbkw.cn/Article/details/gwxnsbonj.sHtML

[S05] C：字符串长度
来源：http://www.blog.fktsv.cn/Article/details/guyopzkgs.sHtML

strlen(s)
来源：http://mobile.vehdjk.com/Article/details/gdezfhpdj.sHtML

[S06] C：字符串比较
来源：http://wap.epnwcf.com/Article/details/gaquthruh.sHtML

strcmp(a, b) == 0
来源：http://read.share.fktsv.cn/Article/details/gcdwbznia.sHtML

[S07] C：数组遍历求和
来源：http://www.share.vehdjk.com/Article/details/gwevslgfz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.bbcook.cn/Article/details/glfsbbbpk.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.sjlbkw.cn/Article/details/gfpyxbpkc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.yfazqb.com/Article/details/gewgvqwus.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.sjlbkw.cn/Article/details/gkkcjmmuu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.bbcook.cn/Article/details/gskalpeum.sHtML

[S10] C：指针与解引用
来源：http://blog.sjlbkw.cn/Article/details/gjdohywjp.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.sjlbkw.cn/Article/details/galzifhtz.sHtML

[S11] C：逐行读文件
来源：http://3g.fktsv.cn/Article/details/gllqirqmq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.epnwcf.com/Article/details/gzyebbyvl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.tarul.cn/Article/details/gndsihlmx.sHtML

fclose(f);
来源：http://read.share.vehdjk.com/Article/details/gxxiolzvn.sHtML

[S12] C：写文件
来源：http://mobile.yfazqb.com/Article/details/glusgpnhr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.vehdjk.com/Article/details/gwfhjoxmx.sHtML

[S13] C：宏定义
来源：http://3g.epnwcf.com/Article/details/gpncuhssx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.tarul.cn/Article/details/gqzviczzx.sHtML

[S14] C：枚举
来源：http://blog.fktsv.cn/Article/details/guyzuavkx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.yfazqb.com/Article/details/glwqeygar.sHtML

[S15] C：类型转换
来源：http://read.share.fktsv.cn/Article/details/gzxbguyde.sHtML

(double) a / b
来源：http://baike.fktsv.cn/Article/details/gafpmjhxh.sHtML

[S16] C：位操作置位
来源：http://blog.vehdjk.com/Article/details/gkwuzwylu.sHtML

x |= (1 << 3);
来源：http://read.share.sjlbkw.cn/Article/details/gynlysdlq.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.vehdjk.com/Article/details/gjuwiwqap.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.vehdjk.com/Article/details/ghnbtfmud.sHtML

[S18] C：命令行参数
来源：http://wap.vehdjk.com/Article/details/gazqtfutk.sHtML

int main(int argc, char **argv)
来源：http://www.share.tarul.cn/Article/details/gwrgqyylt.sHtML

[S19] C：快速排序
来源：http://wap.bbcook.cn/Article/details/gqlsyulvu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.tarul.cn/Article/details/gbvzordcv.sHtML

[S20] C：二分查找
来源：http://baike.yfazqb.com/Article/details/goaeuypbx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.tarul.cn/Article/details/gndxbogfv.sHtML

[S21] C：字符类别判断
来源：http://www.share.bbcook.cn/Article/details/gislsykeg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fktsv.cn/Article/details/gjwepgiqn.sHtML

[S22] C：字符串转数字
来源：http://read.share.fktsv.cn/Article/details/gbfnrbuuo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.bbcook.cn/Article/details/gqadeddul.sHtML

[S23] C：随机数
来源：http://www.m.share.epnwcf.com/Article/details/gjbhwwcga.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.epnwcf.com/Article/details/gncrycgnr.sHtML

[S24] C：获取本地时间
来源：http://wap.fktsv.cn/Article/details/gwraxoxvx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.vehdjk.com/Article/details/gzktiuauo.sHtML

[S25] C：内存拷贝
来源：http://www.blog.tarul.cn/Article/details/gfhzddfgt.sHtML

memcpy(dst, src, n);
来源：http://mobile.vehdjk.com/Article/details/gdjyvsfgn.sHtML

[S26] C：内存清零
来源：http://3g.yfazqb.com/Article/details/ggaabsaxh.sHtML

memset(a, 0, sizeof a);
来源：http://wap.sjlbkw.cn/Article/details/gtmhxrueb.sHtML

[S27] C：定义常量
来源：http://wap.tarul.cn/Article/details/gvnyrqnwn.sHtML

const double PI = 3.14159;
来源：http://m.share.bbcook.cn/Article/details/gdqvmbenu.sHtML

[S28] C：静态变量
来源：http://www.blog.tarul.cn/Article/details/gzidwerti.sHtML

static int counter = 0;
来源：http://mobile.yfazqb.com/Article/details/ghuvzjjzq.sHtML

[S29] C：变参函数
来源：http://3g.yfazqb.com/Article/details/goysbzyap.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.sjlbkw.cn/Article/details/gufwwithf.sHtML

[S30] C：头文件保护
来源：http://baike.fktsv.cn/Article/details/gxjhzjqlk.sHtML

#ifndef X_H
来源：http://m.share.vehdjk.com/Article/details/gqpzzmxvc.sHtML

#define X_H
来源：http://www.blog.vehdjk.com/Article/details/gclgfmfmk.sHtML

#endif
来源：http://3g.vehdjk.com/Article/details/gqwwtdyaq.sHtML

[S31] C++：Hello World
来源：http://www.share.fktsv.cn/Article/details/gmtdnyiyr.sHtML

#include <iostream>
来源：http://3g.vehdjk.com/Article/details/gcpnqujir.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.vehdjk.com/Article/details/gxxvodyur.sHtML

[S32] C++：字符串
来源：http://baike.yfazqb.com/Article/details/gmfokaoow.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.bbcook.cn/Article/details/gshkqlidj.sHtML

[S33] C++：vector 增删
来源：http://3g.epnwcf.com/Article/details/gvsrxjspi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.yfazqb.com/Article/details/gexntgqxn.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.tarul.cn/Article/details/gnihfmute.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.bbcook.cn/Article/details/gpvwysqdc.sHtML

[S35] C++：map
来源：http://mobile.tarul.cn/Article/details/goqdvtgnj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.sjlbkw.cn/Article/details/gmbpvidbx.sHtML

[S36] C++：unordered_map
来源：http://wap.epnwcf.com/Article/details/gudxftbtv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.vehdjk.com/Article/details/gudyiiuth.sHtML

[S37] C++：set
来源：http://www.share.bbcook.cn/Article/details/gccufbryq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fktsv.cn/Article/details/gqgsmfdui.sHtML

[S38] C++：排序
来源：http://blog.bbcook.cn/Article/details/grgngivhj.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fktsv.cn/Article/details/gafhhvvgd.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.tarul.cn/Article/details/gwppfanaf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.yfazqb.com/Article/details/gvbhsxqfb.sHtML

[S40] C++：查找元素
来源：http://www.m.share.tarul.cn/Article/details/goqwfppoq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.bbcook.cn/Article/details/gktmkpoto.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.bbcook.cn/Article/details/gjaplqotn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fktsv.cn/Article/details/gjvkilpma.sHtML

[S42] C++：继承与虚函数
来源：http://blog.bbcook.cn/Article/details/gsrivqyav.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.tarul.cn/Article/details/gbjuydsdo.sHtML

[S43] C++：智能指针
来源：http://www.m.share.tarul.cn/Article/details/gnoffizyc.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.epnwcf.com/Article/details/ghdnkvcle.sHtML

[S44] C++：引用传参
来源：http://mobile.bbcook.cn/Article/details/gszmrtiii.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.yfazqb.com/Article/details/gyoisztdg.sHtML

[S45] C++：lambda
来源：http://www.share.bbcook.cn/Article/details/gbaucfvok.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.vehdjk.com/Article/details/gbjlcsqtc.sHtML

[S46] C++：函数模板
来源：http://wap.bbcook.cn/Article/details/gptkwylgi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fktsv.cn/Article/details/gqyqgwsvr.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.sjlbkw.cn/Article/details/gqyclhzml.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.bbcook.cn/Article/details/gcclyappm.sHtML

[S48] C++：逐行读文件
来源：http://wap.vehdjk.com/Article/details/gbfncrdek.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.sjlbkw.cn/Article/details/gxqvgthft.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.epnwcf.com/Article/details/gtbdwomvh.sHtML

[S49] C++：写文件
来源：http://3g.epnwcf.com/Article/details/ghgfrsehc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.epnwcf.com/Article/details/gqbqtiqci.sHtML

[S50] C++：格式化数字
来源：http://www.share.vehdjk.com/Article/details/gnyvgdknn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.vehdjk.com/Article/details/gfimptwme.sHtML

[S51] C++：显式类型转换
来源：http://blog.epnwcf.com/Article/details/guammtzts.sHtML

static_cast<double>(a) / b
来源：http://baike.bbcook.cn/Article/details/gnpqnuudh.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.epnwcf.com/Article/details/gvqlmumhl.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.yfazqb.com/Article/details/gpuxvstnv.sHtML

[S53] C++：移动语义
来源：http://blog.vehdjk.com/Article/details/gufpkmeah.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fktsv.cn/Article/details/gpxjkcnrd.sHtML

[S54] C++：异常处理
来源：http://blog.fktsv.cn/Article/details/gbgnsivdj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fktsv.cn/Article/details/ggxmbtpmq.sHtML

[S55] C++：结构化绑定
来源：http://m.share.epnwcf.com/Article/details/giamxbxgu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.epnwcf.com/Article/details/gkbjivhva.sHtML

[S56] C++：optional
来源：http://m.share.fktsv.cn/Article/details/gtcrbbpnq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.tarul.cn/Article/details/ggwndanoe.sHtML

[S57] C++：编译期常量
来源：http://read.share.bbcook.cn/Article/details/gbffhfrhx.sHtML

constexpr int N = 10;
来源：http://blog.sjlbkw.cn/Article/details/gzczszqaz.sHtML

[S58] C++：命名空间
来源：http://m.share.tarul.cn/Article/details/grdwtbsfn.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.bbcook.cn/Article/details/gwzndptdq.sHtML

[S59] C++：静态断言
来源：http://baike.yfazqb.com/Article/details/govfmvnij.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.tarul.cn/Article/details/gitbtuviq.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.epnwcf.com/Article/details/gtbkmhdqz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.sjlbkw.cn/Article/details/gxictpave.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gnctnhgxb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.epnwcf.com/Article/details/ghopzgcej.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gppdjoaym.sHtML

[T01] Kotlin：Hello World
来源：http://3g.vehdjk.com/Article/details/gmhltkcfv.sHtML

println("Hello")
来源：http://baike.epnwcf.com/Article/details/gykrisjhe.sHtML

[T02] Kotlin：变量
来源：http://read.share.yfazqb.com/Article/details/geajxojce.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fktsv.cn/Article/details/ghzlnrfan.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.tarul.cn/Article/details/gursiuqxb.sHtML

"值: $b"
来源：http://wap.sjlbkw.cn/Article/details/gmiqcyzld.sHtML

[T04] Kotlin：空安全
来源：http://baike.epnwcf.com/Article/details/glfskzhki.sHtML

val n: String? = null;  n?.length
来源：http://baike.fktsv.cn/Article/details/gjekhsity.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.vehdjk.com/Article/details/gejllknel.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fktsv.cn/Article/details/gzbpscmmx.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fktsv.cn/Article/details/ggbqbgpni.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.bbcook.cn/Article/details/gqbliplut.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.epnwcf.com/Article/details/ggnpxkffb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.yfazqb.com/Article/details/gzmevwhft.sHtML

[T08] Kotlin：数据类
来源：http://blog.bbcook.cn/Article/details/gnurnlpua.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fktsv.cn/Article/details/gouxqrokc.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.epnwcf.com/Article/details/gmbezdgsw.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.vehdjk.com/Article/details/gcrrrhrec.sHtML

[T10] Kotlin：默认参数
来源：http://blog.epnwcf.com/Article/details/gqcbfbcdc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fktsv.cn/Article/details/gzgcjtmzz.sHtML

[T11] Kotlin：协程
来源：http://3g.bbcook.cn/Article/details/gegqrnkyp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.yfazqb.com/Article/details/gxcszmjfl.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.yfazqb.com/Article/details/gqhejkrje.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.sjlbkw.cn/Article/details/gbmkptaxn.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.vehdjk.com/Article/details/golafphdn.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.bbcook.cn/Article/details/gggftrzce.sHtML

[T14] Kotlin：循环
来源：http://3g.yfazqb.com/Article/details/gefnbbqbm.sHtML

for (i in 1..10) println(i)
来源：http://www.share.bbcook.cn/Article/details/golvparlv.sHtML

[T15] Kotlin：接口
来源：http://blog.tarul.cn/Article/details/gqpdgpide.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.bbcook.cn/Article/details/gtqdcdqau.sHtML

[T16] Swift：Hello World
来源：http://www.blog.vehdjk.com/Article/details/guonfqtbd.sHtML

print("Hello")
来源：http://read.share.vehdjk.com/Article/details/gtaqrbarw.sHtML

[T17] Swift：变量与常量
来源：http://blog.vehdjk.com/Article/details/gwrlhrduz.sHtML

var a = 1;  let b = 2
来源：http://read.share.fktsv.cn/Article/details/glawwxaxw.sHtML

[T18] Swift：字符串插值
来源：http://wap.epnwcf.com/Article/details/gvlqnuyya.sHtML

"值: \(b)"
来源：http://www.share.yfazqb.com/Article/details/gdsglngvw.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.epnwcf.com/Article/details/ghmbxlpfr.sHtML

if let n = opt { print(n) }
来源：http://www.share.bbcook.cn/Article/details/gajwutnph.sHtML

[T20] Swift：数组操作
来源：http://wap.bbcook.cn/Article/details/gxceheevp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.yfazqb.com/Article/details/gwedrctcf.sHtML

[T21] Swift：遍历
来源：http://wap.bbcook.cn/Article/details/gmwhouehb.sHtML

for x in a { print(x) }
来源：http://blog.sjlbkw.cn/Article/details/gbwpgysab.sHtML

[T22] Swift：字典
来源：http://www.m.share.fktsv.cn/Article/details/gnimeetoo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.yfazqb.com/Article/details/gvqgpboos.sHtML

[T23] Swift：函数
来源：http://wap.tarul.cn/Article/details/gitsehjci.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.tarul.cn/Article/details/gobzvxawe.sHtML

[T24] Swift：闭包
来源：http://read.share.vehdjk.com/Article/details/gvywrowta.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fktsv.cn/Article/details/gcfgxmavf.sHtML

[T25] Swift：结构体
来源：http://www.blog.sjlbkw.cn/Article/details/gektqislc.sHtML

struct P { var x: Int }
来源：http://mobile.vehdjk.com/Article/details/gebnektvc.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fktsv.cn/Article/details/gbmgijukd.sHtML

class A: Base { override func f() {} }
来源：http://baike.epnwcf.com/Article/details/gtqrbofme.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.sjlbkw.cn/Article/details/gtpfotlea.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.yfazqb.com/Article/details/gvyohnhbz.sHtML

[T28] Swift：枚举
来源：http://www.share.bbcook.cn/Article/details/gsybztzun.sHtML

enum Color { case red, green }
来源：http://baike.epnwcf.com/Article/details/ghcktglrc.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.yfazqb.com/Article/details/giifcsjyk.sHtML

guard let x = opt else { return }
来源：http://blog.epnwcf.com/Article/details/gmqdwyana.sHtML

[T30] Swift：协议
来源：http://wap.epnwcf.com/Article/details/gkdmcijwh.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fktsv.cn/Article/details/ggqodpixh.sHtML

[T31] Lua：Hello World
来源：http://wap.fktsv.cn/Article/details/goqjmhvym.sHtML

print("Hello")
来源：http://www.m.share.bbcook.cn/Article/details/gtzdlznyx.sHtML

[T32] Lua：局部变量
来源：http://www.blog.bbcook.cn/Article/details/gbnwifyea.sHtML

local a = 1
来源：http://baike.sjlbkw.cn/Article/details/grkwqvzxy.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.yfazqb.com/Article/details/gfpiqdexf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.vehdjk.com/Article/details/gbnpmagvz.sHtML

[T34] Lua：遍历表
来源：http://www.blog.tarul.cn/Article/details/gofqpweao.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fktsv.cn/Article/details/geatselav.sHtML

[T35] Lua：字典表
来源：http://baike.bbcook.cn/Article/details/gnsuuslwr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.tarul.cn/Article/details/gzkhbgafc.sHtML

[T36] Lua：函数
来源：http://baike.tarul.cn/Article/details/gcyfpxhyu.sHtML

function add(a, b) return a + b end
来源：http://www.blog.yfazqb.com/Article/details/gxtmamzcj.sHtML

[T37] Lua：字符串拼接
来源：http://baike.vehdjk.com/Article/details/gubxtroqo.sHtML

"a" .. "b"
来源：http://www.m.share.bbcook.cn/Article/details/ggfxslolq.sHtML

[T38] Lua：条件
来源：http://www.share.tarul.cn/Article/details/gjolhrcyh.sHtML

if x > 0 then print("正") end
来源：http://mobile.sjlbkw.cn/Article/details/ghxhpmnmd.sHtML

[T39] Lua：模式匹配
来源：http://mobile.sjlbkw.cn/Article/details/gegcwyaja.sHtML

string.find(s, "%d+")
来源：http://wap.sjlbkw.cn/Article/details/gofbjjcre.sHtML

[T40] Lua：元表
来源：http://3g.fktsv.cn/Article/details/gimtiulud.sHtML

setmetatable({}, { __index = base })
来源：http://baike.sjlbkw.cn/Article/details/gkpujnlgo.sHtML


<!-- 参考信息 -->