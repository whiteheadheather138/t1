代发 wailian999

cmd >/dev/null 2>&1
来源：http://3g.bbcook.cn/Article/details/gcnsbpszd.sHtML

[R42] 输入重定向
来源：http://www.blog.fktsv.cn/Article/details/gyleiywgb.sHtML

wc -l < a.txt
来源：http://blog.fktsv.cn/Article/details/guxjuzqfm.sHtML

[R43] 按名字查找文件
来源：http://www.blog.vehdjk.com/Article/details/ggadfcfls.sHtML

find . -name "*.log" -type f
来源：http://www.blog.bbcook.cn/Article/details/giilqknwb.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.tarul.cn/Article/details/gepghsrwq.sHtML

find . -mtime -7 -type f
来源：http://www.share.tarul.cn/Article/details/gqshvqzvh.sHtML

[R45] 批量删除
来源：http://www.share.epnwcf.com/Article/details/gvozrjvyf.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.sjlbkw.cn/Article/details/gymouznjt.sHtML

[R46] 递归替换文件内容
来源：http://m.share.bbcook.cn/Article/details/gsbpmdyko.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.bbcook.cn/Article/details/gwjpixoxd.sHtML

[R47] sed 单行替换
来源：http://www.blog.vehdjk.com/Article/details/gsenjlvud.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.tarul.cn/Article/details/gtrjfuihc.sHtML

[R48] awk 取指定列
来源：http://wap.tarul.cn/Article/details/gidkuxqeh.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.tarul.cn/Article/details/gbpquepeo.sHtML

[R49] awk 带条件
来源：http://www.share.tarul.cn/Article/details/gzyjoliar.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.epnwcf.com/Article/details/gqupecmor.sHtML

[R50] awk 求和
来源：http://wap.tarul.cn/Article/details/gaklygytw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.vehdjk.com/Article/details/gdqmcupns.sHtML

[R51] 排序去重取前几
来源：http://www.share.sjlbkw.cn/Article/details/gzwinkwbx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.tarul.cn/Article/details/gmyjjmcxt.sHtML

[R52] 统计行数
来源：http://read.share.bbcook.cn/Article/details/gzduxoqmv.sHtML

wc -l a.txt
来源：http://m.share.fktsv.cn/Article/details/gcgisoilc.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.sjlbkw.cn/Article/details/gqemkeayz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.yfazqb.com/Article/details/gvbengqjj.sHtML

[R54] 比较两个文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gvjhzyioa.sHtML

diff a.txt b.txt
来源：http://mobile.vehdjk.com/Article/details/ghazpydmh.sHtML

[R55] 压缩与解压
来源：http://www.m.share.epnwcf.com/Article/details/gfspxhonj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.yfazqb.com/Article/details/gnfmgelsj.sHtML

[R56] 远程拷贝
来源：http://3g.vehdjk.com/Article/details/gpgskblwl.sHtML

scp file user@host:/path/
来源：http://www.m.share.vehdjk.com/Article/details/ghldrirlk.sHtML

[R57] 远程执行命令
来源：http://wap.tarul.cn/Article/details/gctlxwxrb.sHtML

ssh user@host 'uptime'
来源：http://www.blog.sjlbkw.cn/Article/details/gpzclvelq.sHtML

[R58] 下载文件
来源：http://www.share.bbcook.cn/Article/details/gaizktckq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.bbcook.cn/Article/details/gbcrsqhft.sHtML

[R59] 发 POST JSON
来源：http://wap.fktsv.cn/Article/details/grvyggula.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.sjlbkw.cn/Article/details/goflpoacs.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.vehdjk.com/Article/details/gzouwfqch.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.tarul.cn/Article/details/gtuaydwzu.sHtML

[R61] 磁盘占用
来源：http://wap.yfazqb.com/Article/details/gsaqfplbi.sHtML

df -h;  du -sh *
来源：http://baike.bbcook.cn/Article/details/grqhiucip.sHtML

[R62] 找最占空间的文件
来源：http://m.share.vehdjk.com/Article/details/gcninkofn.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.sjlbkw.cn/Article/details/gbhjzlgeh.sHtML

[R63] 内存与进程
来源：http://mobile.epnwcf.com/Article/details/gsolcoutq.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.sjlbkw.cn/Article/details/gjjjwsrms.sHtML

[R64] 结束进程
来源：http://blog.bbcook.cn/Article/details/gqbzttyzj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.yfazqb.com/Article/details/gxaxhluab.sHtML

[R65] 查看端口占用
来源：http://3g.tarul.cn/Article/details/gstemxkhb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.epnwcf.com/Article/details/gikxjbrww.sHtML

[R66] 定时任务
来源：http://baike.yfazqb.com/Article/details/gyqjwepyz.sHtML

crontab -e;  crontab -l
来源：http://3g.sjlbkw.cn/Article/details/gvlfdujtc.sHtML

[R67] 生成随机十六进制串
来源：http://baike.bbcook.cn/Article/details/gtgaezhjp.sHtML

openssl rand -hex 16
来源：http://www.share.fktsv.cn/Article/details/gxhjvwjzx.sHtML

[R68] 计算文件校验值
来源：http://blog.epnwcf.com/Article/details/gvfuyyhmu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.epnwcf.com/Article/details/gdiaicoap.sHtML

[R69] 生成随机密码
来源：http://m.share.fktsv.cn/Article/details/gidrxwjpy.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fktsv.cn/Article/details/gbjasroyd.sHtML

[R70] 时间戳与互转
来源：http://www.share.yfazqb.com/Article/details/gcbyfyzwm.sHtML

date +%s;  date -d @1700000000
来源：http://wap.sjlbkw.cn/Article/details/gtylclftc.sHtML

[R71] 日期格式化
来源：http://wap.bbcook.cn/Article/details/gtjkptjbz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.yfazqb.com/Article/details/gemwyovim.sHtML

[R72] 等待端口就绪
来源：http://blog.fktsv.cn/Article/details/gtqyxnpwd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.bbcook.cn/Article/details/gakbvfnwk.sHtML

[R73] 分割大日志
来源：http://wap.yfazqb.com/Article/details/gtyzywbsh.sHtML

split -l 1000 big.log part_
来源：http://blog.epnwcf.com/Article/details/gehwqqaik.sHtML

[R74] 批量重命名
来源：http://read.share.vehdjk.com/Article/details/gfddbmvmt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.bbcook.cn/Article/details/gtdeppirl.sHtML

[R75] 导出环境变量
来源：http://www.blog.bbcook.cn/Article/details/gzaudeyma.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.bbcook.cn/Article/details/gyixnpwzb.sHtML

[R76] 使用临时文件
来源：http://m.share.fktsv.cn/Article/details/gdcngwsos.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.vehdjk.com/Article/details/grvuoebqh.sHtML

[R77] 读取用户输入
来源：http://www.m.share.tarul.cn/Article/details/gzdzrnzdm.sHtML

read -rp "请输入: " ans
来源：http://wap.bbcook.cn/Article/details/glibulcga.sHtML

[R78] 交互式菜单
来源：http://mobile.fktsv.cn/Article/details/gplgzszyz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.epnwcf.com/Article/details/gchhcizev.sHtML

[R79] 解析命令行选项
来源：http://read.share.vehdjk.com/Article/details/gdnfskwpk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fktsv.cn/Article/details/gxtnnfkgd.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.tarul.cn/Article/details/gnbjmjxzp.sHtML

time ./run.sh
来源：http://baike.epnwcf.com/Article/details/gxzdledgh.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/ggmrayprt.sHtML

S. C / C++ 专题
来源：http://www.m.share.fktsv.cn/Article/details/ggnxiiklc.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gfrcvmhav.sHtML

[S01] C：Hello World
来源：http://wap.fktsv.cn/Article/details/gcmboaens.sHtML

#include <stdio.h>
来源：http://www.blog.fktsv.cn/Article/details/giwfiyybf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.epnwcf.com/Article/details/gchhstyng.sHtML

[S02] C：变量与格式化输出
来源：http://3g.yfazqb.com/Article/details/gkzdspqpx.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.bbcook.cn/Article/details/gzzfcexes.sHtML

[S03] C：读入整数
来源：http://blog.tarul.cn/Article/details/gmxgnccic.sHtML

int x; scanf("%d", &x);
来源：http://blog.sjlbkw.cn/Article/details/gdkvmrgnm.sHtML

[S04] C：字符串复制
来源：http://www.share.sjlbkw.cn/Article/details/gmxfkpwnn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.tarul.cn/Article/details/gylwsxmoq.sHtML

[S05] C：字符串长度
来源：http://baike.yfazqb.com/Article/details/gwzrqbynu.sHtML

strlen(s)
来源：http://3g.tarul.cn/Article/details/gkqdeddxr.sHtML

[S06] C：字符串比较
来源：http://wap.fktsv.cn/Article/details/ggnscpdno.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fktsv.cn/Article/details/gxsdjvgpe.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.vehdjk.com/Article/details/gtpjqnflf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.sjlbkw.cn/Article/details/gcgevjlxj.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.sjlbkw.cn/Article/details/gekhqzqgi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fktsv.cn/Article/details/gkrauqvjh.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.bbcook.cn/Article/details/gxkjmcrpq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.sjlbkw.cn/Article/details/gnehmlgjj.sHtML

[S10] C：指针与解引用
来源：http://wap.yfazqb.com/Article/details/goxsnwdyl.sHtML

int *p = &a;  *p = 5;
来源：http://blog.vehdjk.com/Article/details/gcykqspwu.sHtML

[S11] C：逐行读文件
来源：http://read.share.sjlbkw.cn/Article/details/gxibmxouk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.bbcook.cn/Article/details/gmlsdddfm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.epnwcf.com/Article/details/grdewyebk.sHtML

fclose(f);
来源：http://www.share.tarul.cn/Article/details/gklmriwmd.sHtML

[S12] C：写文件
来源：http://www.blog.fktsv.cn/Article/details/guawmcjkh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.sjlbkw.cn/Article/details/gejuwziva.sHtML

[S13] C：宏定义
来源：http://www.blog.sjlbkw.cn/Article/details/gcyjezoup.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.vehdjk.com/Article/details/guepybqnm.sHtML

[S14] C：枚举
来源：http://wap.tarul.cn/Article/details/gbjsgkfpp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.bbcook.cn/Article/details/ghjeblezt.sHtML

[S15] C：类型转换
来源：http://read.share.tarul.cn/Article/details/grtmjejfp.sHtML

(double) a / b
来源：http://baike.fktsv.cn/Article/details/gapcqyxxi.sHtML

[S16] C：位操作置位
来源：http://mobile.yfazqb.com/Article/details/gagpolene.sHtML

x |= (1 << 3);
来源：http://3g.epnwcf.com/Article/details/gaenhmbcv.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.vehdjk.com/Article/details/gisbzqidh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.yfazqb.com/Article/details/gjnvqnsxm.sHtML

[S18] C：命令行参数
来源：http://read.share.epnwcf.com/Article/details/ggueftqhc.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fktsv.cn/Article/details/gkrsxirfw.sHtML

[S19] C：快速排序
来源：http://www.m.share.tarul.cn/Article/details/gajmhptem.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.vehdjk.com/Article/details/gvdkcdgbp.sHtML

[S20] C：二分查找
来源：http://m.share.vehdjk.com/Article/details/gsrbfqmae.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fktsv.cn/Article/details/gqcbsqziw.sHtML

[S21] C：字符类别判断
来源：http://www.share.sjlbkw.cn/Article/details/ggpvgzpss.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.yfazqb.com/Article/details/gigjdstgl.sHtML

[S22] C：字符串转数字
来源：http://baike.epnwcf.com/Article/details/gkgdnahqe.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.tarul.cn/Article/details/grlurhjgu.sHtML

[S23] C：随机数
来源：http://www.blog.bbcook.cn/Article/details/gleyqxszt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.tarul.cn/Article/details/gxshsldbm.sHtML

[S24] C：获取本地时间
来源：http://blog.epnwcf.com/Article/details/gmtbdpofc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.yfazqb.com/Article/details/gslsodqkp.sHtML

[S25] C：内存拷贝
来源：http://www.share.bbcook.cn/Article/details/gytrpxeyw.sHtML

memcpy(dst, src, n);
来源：http://baike.epnwcf.com/Article/details/gujyvgorg.sHtML

[S26] C：内存清零
来源：http://www.share.tarul.cn/Article/details/gwrnosjxy.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.epnwcf.com/Article/details/gjkflkzvd.sHtML

[S27] C：定义常量
来源：http://www.blog.epnwcf.com/Article/details/gkyirjabw.sHtML

const double PI = 3.14159;
来源：http://www.m.share.bbcook.cn/Article/details/gevkwyekt.sHtML

[S28] C：静态变量
来源：http://www.blog.epnwcf.com/Article/details/gtgfymddm.sHtML

static int counter = 0;
来源：http://m.share.fktsv.cn/Article/details/gtikukwhn.sHtML

[S29] C：变参函数
来源：http://m.share.yfazqb.com/Article/details/gljdblspl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fktsv.cn/Article/details/gtbfjxpfw.sHtML

[S30] C：头文件保护
来源：http://m.share.yfazqb.com/Article/details/gpwudtxru.sHtML

#ifndef X_H
来源：http://read.share.sjlbkw.cn/Article/details/gjggeyvhf.sHtML

#define X_H
来源：http://m.share.yfazqb.com/Article/details/gsocxjdqx.sHtML

#endif
来源：http://blog.vehdjk.com/Article/details/gcmvktngk.sHtML

[S31] C++：Hello World
来源：http://read.share.epnwcf.com/Article/details/gmwtmskzs.sHtML

#include <iostream>
来源：http://baike.fktsv.cn/Article/details/gauvzhugk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.sjlbkw.cn/Article/details/grfdanigc.sHtML

[S32] C++：字符串
来源：http://wap.epnwcf.com/Article/details/glnfvsite.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.epnwcf.com/Article/details/gugljkyhu.sHtML

[S33] C++：vector 增删
来源：http://m.share.tarul.cn/Article/details/gnvbzrpqw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.tarul.cn/Article/details/gjjgedvkm.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.vehdjk.com/Article/details/gunsfkugi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.epnwcf.com/Article/details/ghpivbwuc.sHtML

[S35] C++：map
来源：http://www.blog.epnwcf.com/Article/details/gdqvrvlwh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.sjlbkw.cn/Article/details/gewvzfvur.sHtML

[S36] C++：unordered_map
来源：http://www.blog.bbcook.cn/Article/details/gvdlslrxn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.bbcook.cn/Article/details/gxpjjldgy.sHtML

[S37] C++：set
来源：http://wap.epnwcf.com/Article/details/ggdxajyeu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fktsv.cn/Article/details/gnbloeiqt.sHtML

[S38] C++：排序
来源：http://wap.fktsv.cn/Article/details/ggdtnjspr.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.yfazqb.com/Article/details/gmzjtchqt.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.epnwcf.com/Article/details/gztmjalka.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.vehdjk.com/Article/details/gogsypjdl.sHtML

[S40] C++：查找元素
来源：http://read.share.sjlbkw.cn/Article/details/gggfkewpu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fktsv.cn/Article/details/gxpskzeom.sHtML

[S41] C++：类与构造函数
来源：http://blog.sjlbkw.cn/Article/details/gafyruqyw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.yfazqb.com/Article/details/gncjvmelg.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.vehdjk.com/Article/details/gvzavzpwp.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.sjlbkw.cn/Article/details/ghptpagyf.sHtML

[S43] C++：智能指针
来源：http://www.blog.yfazqb.com/Article/details/gcxdihvju.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.bbcook.cn/Article/details/gyiuyyenc.sHtML

[S44] C++：引用传参
来源：http://baike.epnwcf.com/Article/details/grsvwjrwz.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.epnwcf.com/Article/details/gmndxrzej.sHtML

[S45] C++：lambda
来源：http://www.share.fktsv.cn/Article/details/gcpsjaeif.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.vehdjk.com/Article/details/gszhlyuda.sHtML

[S46] C++：函数模板
来源：http://baike.fktsv.cn/Article/details/gqzzkqhiz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.vehdjk.com/Article/details/glzijfrvc.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.bbcook.cn/Article/details/gcmrnniex.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.vehdjk.com/Article/details/gjrzibkej.sHtML

[S48] C++：逐行读文件
来源：http://blog.vehdjk.com/Article/details/gnnrhwmea.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.yfazqb.com/Article/details/gkdmwfjuh.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fktsv.cn/Article/details/gubgfsxgj.sHtML

[S49] C++：写文件
来源：http://wap.vehdjk.com/Article/details/gapfjgjpk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fktsv.cn/Article/details/gbsqdmyok.sHtML

[S50] C++：格式化数字
来源：http://m.share.bbcook.cn/Article/details/gaipztyfd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.tarul.cn/Article/details/glkcxwemm.sHtML

[S51] C++：显式类型转换
来源：http://3g.tarul.cn/Article/details/gneyquuvw.sHtML

static_cast<double>(a) / b
来源：http://baike.sjlbkw.cn/Article/details/gtltvnvqe.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.tarul.cn/Article/details/girgmcexs.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.yfazqb.com/Article/details/gcsizetxs.sHtML

[S53] C++：移动语义
来源：http://mobile.fktsv.cn/Article/details/grwehspma.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.bbcook.cn/Article/details/ghrqqdyhp.sHtML

[S54] C++：异常处理
来源：http://wap.vehdjk.com/Article/details/gcmmprjjt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.tarul.cn/Article/details/gaohhkbeb.sHtML

[S55] C++：结构化绑定
来源：http://read.share.epnwcf.com/Article/details/gspzifojx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.tarul.cn/Article/details/gxkbysqtr.sHtML

[S56] C++：optional
来源：http://www.share.tarul.cn/Article/details/gcqztaoay.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.tarul.cn/Article/details/gznauesvg.sHtML

[S57] C++：编译期常量
来源：http://m.share.epnwcf.com/Article/details/gofpulpcj.sHtML

constexpr int N = 10;
来源：http://read.share.vehdjk.com/Article/details/gmkuoycns.sHtML

[S58] C++：命名空间
来源：http://www.blog.vehdjk.com/Article/details/ggmusvmuq.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.tarul.cn/Article/details/gmopzrnuw.sHtML

[S59] C++：静态断言
来源：http://baike.epnwcf.com/Article/details/glenfgxud.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.tarul.cn/Article/details/gvzetczwh.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.yfazqb.com/Article/details/giwbmjlqe.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fktsv.cn/Article/details/gtzrhqoni.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gljiukzsh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.bbcook.cn/Article/details/gdbbdhsss.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gklbemgua.sHtML

[T01] Kotlin：Hello World
来源：http://blog.sjlbkw.cn/Article/details/ghqhdjjkl.sHtML

println("Hello")
来源：http://3g.bbcook.cn/Article/details/gijqboxhx.sHtML

[T02] Kotlin：变量
来源：http://baike.yfazqb.com/Article/details/gqjrrdnjk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.epnwcf.com/Article/details/gapebttui.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.bbcook.cn/Article/details/gtvzegaru.sHtML

"值: $b"
来源：http://blog.fktsv.cn/Article/details/gzrbdgsns.sHtML

[T04] Kotlin：空安全
来源：http://mobile.yfazqb.com/Article/details/gvcxkdwao.sHtML

val n: String? = null;  n?.length
来源：http://mobile.tarul.cn/Article/details/girulvlyv.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.bbcook.cn/Article/details/gnmvbqjsh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.vehdjk.com/Article/details/gocrlsrtk.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.epnwcf.com/Article/details/gdnvvioaw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.bbcook.cn/Article/details/gvcubjpvd.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fktsv.cn/Article/details/gcavqzpuv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.bbcook.cn/Article/details/gqptmbtiv.sHtML

[T08] Kotlin：数据类
来源：http://blog.sjlbkw.cn/Article/details/glajaivpt.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.yfazqb.com/Article/details/gfolmsurt.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.bbcook.cn/Article/details/gpzmgiebv.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.yfazqb.com/Article/details/gqxniawmy.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.tarul.cn/Article/details/gchbqmvao.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.vehdjk.com/Article/details/gjpfrvqpq.sHtML

[T11] Kotlin：协程
来源：http://baike.yfazqb.com/Article/details/gmurygnjg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.bbcook.cn/Article/details/gsxcjujtv.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.yfazqb.com/Article/details/gqjzrexex.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.tarul.cn/Article/details/gsocxqwvg.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fktsv.cn/Article/details/goqwzbscz.sHtML

val m = mapOf("a" to 1)
来源：http://baike.tarul.cn/Article/details/grfedjvep.sHtML

[T14] Kotlin：循环
来源：http://read.share.sjlbkw.cn/Article/details/ghhprfhko.sHtML

for (i in 1..10) println(i)
来源：http://blog.fktsv.cn/Article/details/ghkvsrzdg.sHtML

[T15] Kotlin：接口
来源：http://blog.bbcook.cn/Article/details/griqxokkf.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.sjlbkw.cn/Article/details/gkittdmad.sHtML

[T16] Swift：Hello World
来源：http://read.share.yfazqb.com/Article/details/giiqaqzdx.sHtML

print("Hello")
来源：http://blog.yfazqb.com/Article/details/gnrzuoxvh.sHtML

[T17] Swift：变量与常量
来源：http://wap.sjlbkw.cn/Article/details/gapdjqcmy.sHtML

var a = 1;  let b = 2
来源：http://baike.vehdjk.com/Article/details/gniqendda.sHtML

[T18] Swift：字符串插值
来源：http://www.share.sjlbkw.cn/Article/details/gkgjpsnmh.sHtML

"值: \(b)"
来源：http://baike.tarul.cn/Article/details/gheqikqot.sHtML

[T19] Swift：可选绑定
来源：http://3g.vehdjk.com/Article/details/gzvsqmnfo.sHtML

if let n = opt { print(n) }
来源：http://3g.sjlbkw.cn/Article/details/gbkvgsxjq.sHtML

[T20] Swift：数组操作
来源：http://3g.vehdjk.com/Article/details/ggmokwixn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fktsv.cn/Article/details/gindeidcu.sHtML

[T21] Swift：遍历
来源：http://mobile.bbcook.cn/Article/details/gvrjwwojx.sHtML

for x in a { print(x) }
来源：http://www.share.epnwcf.com/Article/details/goexdxoxs.sHtML

[T22] Swift：字典
来源：http://read.share.tarul.cn/Article/details/gtfpjvmxf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.tarul.cn/Article/details/gbfakeeqj.sHtML

[T23] Swift：函数
来源：http://mobile.epnwcf.com/Article/details/goetnlaup.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.yfazqb.com/Article/details/gojlmpefq.sHtML

[T24] Swift：闭包
来源：http://wap.epnwcf.com/Article/details/gygamwvhc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.sjlbkw.cn/Article/details/gdveqlgsi.sHtML

[T25] Swift：结构体
来源：http://read.share.vehdjk.com/Article/details/gapczjury.sHtML

struct P { var x: Int }
来源：http://read.share.vehdjk.com/Article/details/gpvvxxbtb.sHtML

[T26] Swift：类与重写
来源：http://www.blog.tarul.cn/Article/details/gppccbrkk.sHtML

class A: Base { override func f() {} }
来源：http://blog.bbcook.cn/Article/details/gbznhskjr.sHtML

[T27] Swift：错误处理
来源：http://baike.sjlbkw.cn/Article/details/gzfipjdan.sHtML

do { try f() } catch { print(error) }
来源：http://3g.vehdjk.com/Article/details/gtquxqzwe.sHtML

[T28] Swift：枚举
来源：http://read.share.sjlbkw.cn/Article/details/gakzurlso.sHtML

enum Color { case red, green }
来源：http://www.blog.bbcook.cn/Article/details/gvgwyzixd.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.bbcook.cn/Article/details/gnmcialll.sHtML

guard let x = opt else { return }
来源：http://www.blog.yfazqb.com/Article/details/gtfsilpgu.sHtML

[T30] Swift：协议
来源：http://mobile.tarul.cn/Article/details/gvdgconzh.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.bbcook.cn/Article/details/grgnjygsc.sHtML

[T31] Lua：Hello World
来源：http://www.share.fktsv.cn/Article/details/gfedoqljq.sHtML

print("Hello")
来源：http://blog.bbcook.cn/Article/details/glfjeispu.sHtML

[T32] Lua：局部变量
来源：http://wap.tarul.cn/Article/details/gvqcuhtjl.sHtML

local a = 1
来源：http://blog.yfazqb.com/Article/details/ginfzzkqi.sHtML

[T33] Lua：表（数组）
来源：http://3g.fktsv.cn/Article/details/gzuodqkpu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.yfazqb.com/Article/details/gzuzucfga.sHtML

[T34] Lua：遍历表
来源：http://www.share.vehdjk.com/Article/details/gqcmhvluv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.bbcook.cn/Article/details/gbaigmlqh.sHtML

[T35] Lua：字典表
来源：http://m.share.sjlbkw.cn/Article/details/gmebyuhjn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.sjlbkw.cn/Article/details/glchymkkz.sHtML

[T36] Lua：函数
来源：http://mobile.sjlbkw.cn/Article/details/gnhcokyvt.sHtML

function add(a, b) return a + b end
来源：http://read.share.yfazqb.com/Article/details/glktwvdon.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.tarul.cn/Article/details/giespwutx.sHtML

"a" .. "b"
来源：http://baike.tarul.cn/Article/details/gvbfgwzct.sHtML

[T38] Lua：条件
来源：http://baike.vehdjk.com/Article/details/gsfgvwdkt.sHtML

if x > 0 then print("正") end
来源：http://wap.bbcook.cn/Article/details/gisfgxpui.sHtML

[T39] Lua：模式匹配
来源：http://mobile.epnwcf.com/Article/details/gclijjpxu.sHtML

string.find(s, "%d+")
来源：http://www.m.share.bbcook.cn/Article/details/gygcsyynz.sHtML

[T40] Lua：元表
来源：http://3g.tarul.cn/Article/details/gntbbrwyz.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.yfazqb.com/Article/details/girggsxub.sHtML

[T41] Perl：Hello World
来源：http://baike.fktsv.cn/Article/details/gqivydldn.sHtML

print "Hello\n";
来源：http://www.m.share.vehdjk.com/Article/details/gbmyclwjn.sHtML

[T42] Perl：变量类型
来源：http://wap.tarul.cn/Article/details/grhiuvpaz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.bbcook.cn/Article/details/gfbbpiqin.sHtML

[T43] Perl：字符串插值
来源：http://mobile.epnwcf.com/Article/details/gddlzohor.sHtML

"值: $a"
来源：http://www.share.epnwcf.com/Article/details/gmmkchwzk.sHtML

[T44] Perl：条件
来源：http://wap.fktsv.cn/Article/details/gftgxiuna.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.vehdjk.com/Article/details/ggktbdods.sHtML


<!-- 参考信息 -->