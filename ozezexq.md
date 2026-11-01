代发 wailian999

cmd >/dev/null 2>&1
来源：http://m.share.tarul.cn/Article/details/gdwlfbwgc.sHtML

[R42] 输入重定向
来源：http://blog.yfazqb.com/Article/details/glseybbuu.sHtML

wc -l < a.txt
来源：http://blog.bbcook.cn/Article/details/gbxkzpgdg.sHtML

[R43] 按名字查找文件
来源：http://baike.yfazqb.com/Article/details/goarohnly.sHtML

find . -name "*.log" -type f
来源：http://www.share.sjlbkw.cn/Article/details/glakbyzbb.sHtML

[R44] 按修改时间查找
来源：http://blog.fktsv.cn/Article/details/gjemsclvq.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.yfazqb.com/Article/details/gbtmjzjxy.sHtML

[R45] 批量删除
来源：http://mobile.bbcook.cn/Article/details/gmduxgybm.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.vehdjk.com/Article/details/geyqwtdwg.sHtML

[R46] 递归替换文件内容
来源：http://baike.vehdjk.com/Article/details/gqnvwfyyk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.yfazqb.com/Article/details/gxvdxjnup.sHtML

[R47] sed 单行替换
来源：http://read.share.epnwcf.com/Article/details/gtlvhdicf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.tarul.cn/Article/details/gkxetdvef.sHtML

[R48] awk 取指定列
来源：http://3g.fktsv.cn/Article/details/gijebfvaw.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.epnwcf.com/Article/details/gccmxsyrk.sHtML

[R49] awk 带条件
来源：http://www.share.yfazqb.com/Article/details/grkiazhqo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fktsv.cn/Article/details/gqytehbtm.sHtML

[R50] awk 求和
来源：http://mobile.epnwcf.com/Article/details/gzeijeonj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.bbcook.cn/Article/details/gxvimfigf.sHtML

[R51] 排序去重取前几
来源：http://3g.vehdjk.com/Article/details/gfikbjftb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.sjlbkw.cn/Article/details/gajecslfi.sHtML

[R52] 统计行数
来源：http://read.share.bbcook.cn/Article/details/gkdqyazsq.sHtML

wc -l a.txt
来源：http://wap.yfazqb.com/Article/details/gvgeuvvce.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.bbcook.cn/Article/details/gndvthyxo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.yfazqb.com/Article/details/gmfgeumqa.sHtML

[R54] 比较两个文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gmpvsbdsv.sHtML

diff a.txt b.txt
来源：http://www.blog.vehdjk.com/Article/details/gbalwcrhl.sHtML

[R55] 压缩与解压
来源：http://wap.sjlbkw.cn/Article/details/geogspihb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.yfazqb.com/Article/details/gfyqlzkac.sHtML

[R56] 远程拷贝
来源：http://www.blog.fktsv.cn/Article/details/gdvpzvtwn.sHtML

scp file user@host:/path/
来源：http://read.share.tarul.cn/Article/details/gajatnovr.sHtML

[R57] 远程执行命令
来源：http://3g.epnwcf.com/Article/details/gzjggmosi.sHtML

ssh user@host 'uptime'
来源：http://read.share.tarul.cn/Article/details/gzanhpqnn.sHtML

[R58] 下载文件
来源：http://3g.fktsv.cn/Article/details/gwumruowb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.sjlbkw.cn/Article/details/gueqraarz.sHtML

[R59] 发 POST JSON
来源：http://wap.vehdjk.com/Article/details/gjkzczqcr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.vehdjk.com/Article/details/gyydjntag.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.tarul.cn/Article/details/geqdogqfi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.vehdjk.com/Article/details/gzxorqvyn.sHtML

[R61] 磁盘占用
来源：http://baike.fktsv.cn/Article/details/gpsoyrzee.sHtML

df -h;  du -sh *
来源：http://baike.tarul.cn/Article/details/gcgcwiacf.sHtML

[R62] 找最占空间的文件
来源：http://baike.tarul.cn/Article/details/gzcgwshmw.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fktsv.cn/Article/details/gelaithah.sHtML

[R63] 内存与进程
来源：http://wap.sjlbkw.cn/Article/details/gzftefqgl.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.bbcook.cn/Article/details/gohhxzxfq.sHtML

[R64] 结束进程
来源：http://wap.bbcook.cn/Article/details/gaiosrvua.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.bbcook.cn/Article/details/gmcnmcutv.sHtML

[R65] 查看端口占用
来源：http://mobile.bbcook.cn/Article/details/gjekkvsgy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.sjlbkw.cn/Article/details/gxvrinbxf.sHtML

[R66] 定时任务
来源：http://mobile.fktsv.cn/Article/details/ghxtgpwcr.sHtML

crontab -e;  crontab -l
来源：http://3g.yfazqb.com/Article/details/gcnaqzalz.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fktsv.cn/Article/details/gunalxgvh.sHtML

openssl rand -hex 16
来源：http://mobile.vehdjk.com/Article/details/gmbckdeei.sHtML

[R68] 计算文件校验值
来源：http://read.share.tarul.cn/Article/details/gdhapqkra.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.yfazqb.com/Article/details/gjtjkczad.sHtML

[R69] 生成随机密码
来源：http://read.share.bbcook.cn/Article/details/grufrqcfo.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.epnwcf.com/Article/details/gxsvdqaip.sHtML

[R70] 时间戳与互转
来源：http://blog.vehdjk.com/Article/details/gzexbwzmi.sHtML

date +%s;  date -d @1700000000
来源：http://3g.tarul.cn/Article/details/gztotoxyw.sHtML

[R71] 日期格式化
来源：http://read.share.epnwcf.com/Article/details/gilwzrubx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.sjlbkw.cn/Article/details/ggerfnyry.sHtML

[R72] 等待端口就绪
来源：http://www.share.yfazqb.com/Article/details/gkxrjaarq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fktsv.cn/Article/details/griaywtvu.sHtML

[R73] 分割大日志
来源：http://mobile.tarul.cn/Article/details/ghebolhpq.sHtML

split -l 1000 big.log part_
来源：http://www.share.yfazqb.com/Article/details/gppgrtnas.sHtML

[R74] 批量重命名
来源：http://www.blog.bbcook.cn/Article/details/gtsdxzbvv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fktsv.cn/Article/details/gqhlindmh.sHtML

[R75] 导出环境变量
来源：http://3g.bbcook.cn/Article/details/gergsprwo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.tarul.cn/Article/details/gqbgnhkhi.sHtML

[R76] 使用临时文件
来源：http://mobile.fktsv.cn/Article/details/gqhhydhak.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.yfazqb.com/Article/details/gdgqnrkpv.sHtML

[R77] 读取用户输入
来源：http://www.blog.bbcook.cn/Article/details/geqbaikjs.sHtML

read -rp "请输入: " ans
来源：http://3g.fktsv.cn/Article/details/ggziggtoj.sHtML

[R78] 交互式菜单
来源：http://www.blog.vehdjk.com/Article/details/gmccbmbyt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fktsv.cn/Article/details/gzzcejqla.sHtML

[R79] 解析命令行选项
来源：http://baike.vehdjk.com/Article/details/geykfhevu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fktsv.cn/Article/details/gmipohumd.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.sjlbkw.cn/Article/details/gycphpubi.sHtML

time ./run.sh
来源：http://blog.yfazqb.com/Article/details/glanqtfil.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/ggpicdtbh.sHtML

S. C / C++ 专题
来源：http://mobile.yfazqb.com/Article/details/gdxfhyunx.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gpmviesbd.sHtML

[S01] C：Hello World
来源：http://www.share.vehdjk.com/Article/details/gkseznopl.sHtML

#include <stdio.h>
来源：http://www.m.share.sjlbkw.cn/Article/details/gdmnlrjbx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.bbcook.cn/Article/details/gdkawtxww.sHtML

[S02] C：变量与格式化输出
来源：http://baike.epnwcf.com/Article/details/gqepmrfex.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.bbcook.cn/Article/details/gvvgbuujr.sHtML

[S03] C：读入整数
来源：http://3g.epnwcf.com/Article/details/gdkpxvupo.sHtML

int x; scanf("%d", &x);
来源：http://read.share.sjlbkw.cn/Article/details/gnhgkysqs.sHtML

[S04] C：字符串复制
来源：http://blog.fktsv.cn/Article/details/grsbqmgbv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.epnwcf.com/Article/details/gmeyrxcjs.sHtML

[S05] C：字符串长度
来源：http://m.share.fktsv.cn/Article/details/guchzedet.sHtML

strlen(s)
来源：http://mobile.yfazqb.com/Article/details/gwunvzdsi.sHtML

[S06] C：字符串比较
来源：http://baike.sjlbkw.cn/Article/details/gudoopuzk.sHtML

strcmp(a, b) == 0
来源：http://www.share.epnwcf.com/Article/details/ghdrfpudn.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.epnwcf.com/Article/details/gcgyqwfqu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.epnwcf.com/Article/details/ghcnqleqk.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.bbcook.cn/Article/details/gfcpmuxmh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.bbcook.cn/Article/details/gkmmyhbsd.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.epnwcf.com/Article/details/ghihepwqn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.epnwcf.com/Article/details/gflxzcxwv.sHtML

[S10] C：指针与解引用
来源：http://read.share.sjlbkw.cn/Article/details/gxzflhjzu.sHtML

int *p = &a;  *p = 5;
来源：http://3g.sjlbkw.cn/Article/details/gmjkaaywu.sHtML

[S11] C：逐行读文件
来源：http://wap.fktsv.cn/Article/details/gffwfkyae.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.tarul.cn/Article/details/gjsysaahx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.yfazqb.com/Article/details/gmzwjdzxe.sHtML

fclose(f);
来源：http://www.m.share.yfazqb.com/Article/details/gyqjujdps.sHtML

[S12] C：写文件
来源：http://baike.fktsv.cn/Article/details/gadpzdjqt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.bbcook.cn/Article/details/gdwbthmdb.sHtML

[S13] C：宏定义
来源：http://baike.yfazqb.com/Article/details/gnbsyogym.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.tarul.cn/Article/details/gdvksfjca.sHtML

[S14] C：枚举
来源：http://baike.yfazqb.com/Article/details/gojhyumvi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.sjlbkw.cn/Article/details/ghsnaqqql.sHtML

[S15] C：类型转换
来源：http://www.blog.vehdjk.com/Article/details/gmsinvrxw.sHtML

(double) a / b
来源：http://www.m.share.epnwcf.com/Article/details/gqwskzwqb.sHtML

[S16] C：位操作置位
来源：http://mobile.fktsv.cn/Article/details/gwkmholpx.sHtML

x |= (1 << 3);
来源：http://3g.fktsv.cn/Article/details/gaeqnoste.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.bbcook.cn/Article/details/gsqepaymq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.bbcook.cn/Article/details/guvksjixo.sHtML

[S18] C：命令行参数
来源：http://wap.bbcook.cn/Article/details/gzvhmjnml.sHtML

int main(int argc, char **argv)
来源：http://baike.tarul.cn/Article/details/gilnvhqjt.sHtML

[S19] C：快速排序
来源：http://mobile.sjlbkw.cn/Article/details/gfkkxaypc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.vehdjk.com/Article/details/gtikbdpqa.sHtML

[S20] C：二分查找
来源：http://read.share.vehdjk.com/Article/details/gxjbwolav.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.tarul.cn/Article/details/guxlpazzt.sHtML

[S21] C：字符类别判断
来源：http://www.share.epnwcf.com/Article/details/ggjthpfxe.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.bbcook.cn/Article/details/gcvvcltsw.sHtML

[S22] C：字符串转数字
来源：http://mobile.fktsv.cn/Article/details/gxajpzlsa.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.bbcook.cn/Article/details/gjgyqtlcn.sHtML

[S23] C：随机数
来源：http://www.blog.fktsv.cn/Article/details/ghqykblbp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.sjlbkw.cn/Article/details/gnyvcsgia.sHtML

[S24] C：获取本地时间
来源：http://3g.yfazqb.com/Article/details/glellmozl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.bbcook.cn/Article/details/godfoqhhu.sHtML

[S25] C：内存拷贝
来源：http://www.blog.vehdjk.com/Article/details/ggkxaiote.sHtML

memcpy(dst, src, n);
来源：http://www.share.tarul.cn/Article/details/gxkittnny.sHtML

[S26] C：内存清零
来源：http://www.m.share.bbcook.cn/Article/details/goroqttxj.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fktsv.cn/Article/details/givvkjtuj.sHtML

[S27] C：定义常量
来源：http://read.share.fktsv.cn/Article/details/gfuiwaloe.sHtML

const double PI = 3.14159;
来源：http://3g.sjlbkw.cn/Article/details/glykbewcv.sHtML

[S28] C：静态变量
来源：http://blog.tarul.cn/Article/details/gtyargjsm.sHtML

static int counter = 0;
来源：http://baike.yfazqb.com/Article/details/gszqnicxo.sHtML

[S29] C：变参函数
来源：http://mobile.sjlbkw.cn/Article/details/gzcohaxkh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.vehdjk.com/Article/details/geaacfvpu.sHtML

[S30] C：头文件保护
来源：http://mobile.vehdjk.com/Article/details/gzueuzmlb.sHtML

#ifndef X_H
来源：http://www.share.tarul.cn/Article/details/gkkekkqkl.sHtML

#define X_H
来源：http://read.share.bbcook.cn/Article/details/gbmijiqwp.sHtML

#endif
来源：http://www.share.fktsv.cn/Article/details/gmlipzmgh.sHtML

[S31] C++：Hello World
来源：http://www.share.vehdjk.com/Article/details/grjsrjarn.sHtML

#include <iostream>
来源：http://baike.yfazqb.com/Article/details/gwzogqgdi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.bbcook.cn/Article/details/gqcfnjytr.sHtML

[S32] C++：字符串
来源：http://m.share.vehdjk.com/Article/details/ghuyykibf.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.bbcook.cn/Article/details/gavxctoez.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.bbcook.cn/Article/details/gjmghzuii.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.tarul.cn/Article/details/gsgibcpjb.sHtML

[S34] C++：遍历 vector
来源：http://baike.fktsv.cn/Article/details/gfluvmlnh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.bbcook.cn/Article/details/gogjcnyok.sHtML

[S35] C++：map
来源：http://www.m.share.sjlbkw.cn/Article/details/gicwizhdp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.yfazqb.com/Article/details/gmtirihmv.sHtML

[S36] C++：unordered_map
来源：http://blog.fktsv.cn/Article/details/gjxvexyry.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.epnwcf.com/Article/details/grnvbzamb.sHtML

[S37] C++：set
来源：http://m.share.bbcook.cn/Article/details/glclouxxh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.bbcook.cn/Article/details/gzlotsvwv.sHtML

[S38] C++：排序
来源：http://blog.bbcook.cn/Article/details/giwgqupcl.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.vehdjk.com/Article/details/gkoxcncnq.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fktsv.cn/Article/details/ghdwcxvoo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.sjlbkw.cn/Article/details/gmzjawqap.sHtML

[S40] C++：查找元素
来源：http://blog.fktsv.cn/Article/details/ggjrjxvaj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.bbcook.cn/Article/details/ggjokkxtk.sHtML

[S41] C++：类与构造函数
来源：http://blog.fktsv.cn/Article/details/gkiecphop.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fktsv.cn/Article/details/gucxbagox.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.epnwcf.com/Article/details/guwsgnnoi.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.sjlbkw.cn/Article/details/gmhoucgtx.sHtML

[S43] C++：智能指针
来源：http://www.m.share.tarul.cn/Article/details/gwfgyfoxj.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.vehdjk.com/Article/details/gkijswnux.sHtML

[S44] C++：引用传参
来源：http://read.share.epnwcf.com/Article/details/gysmxafze.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.yfazqb.com/Article/details/gvndafzcu.sHtML

[S45] C++：lambda
来源：http://mobile.epnwcf.com/Article/details/gxyurugtx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.epnwcf.com/Article/details/gcpuumejw.sHtML

[S46] C++：函数模板
来源：http://m.share.sjlbkw.cn/Article/details/gnyinsyfj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fktsv.cn/Article/details/gvyedsshp.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.bbcook.cn/Article/details/grxisoncs.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.sjlbkw.cn/Article/details/gvhnqyzii.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.yfazqb.com/Article/details/gasefvefj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.vehdjk.com/Article/details/gctdhbefj.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.sjlbkw.cn/Article/details/gfhsdeigv.sHtML

[S49] C++：写文件
来源：http://mobile.vehdjk.com/Article/details/gmhqefghi.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.sjlbkw.cn/Article/details/gfjgsoled.sHtML

[S50] C++：格式化数字
来源：http://read.share.fktsv.cn/Article/details/gluxholaj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.epnwcf.com/Article/details/githlhcnt.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.vehdjk.com/Article/details/gjkxvjxuh.sHtML

static_cast<double>(a) / b
来源：http://wap.tarul.cn/Article/details/glsqqdehk.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.yfazqb.com/Article/details/gpndecbxv.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fktsv.cn/Article/details/gdtgzqnyv.sHtML

[S53] C++：移动语义
来源：http://www.blog.yfazqb.com/Article/details/gcdlmxpnu.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.vehdjk.com/Article/details/gzxxfagec.sHtML

[S54] C++：异常处理
来源：http://www.blog.tarul.cn/Article/details/gcojzrjdk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.bbcook.cn/Article/details/grmipynfg.sHtML

[S55] C++：结构化绑定
来源：http://mobile.vehdjk.com/Article/details/gcroppkce.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fktsv.cn/Article/details/gqhnupmxk.sHtML

[S56] C++：optional
来源：http://blog.bbcook.cn/Article/details/gndgglccg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.bbcook.cn/Article/details/gmzujcqtl.sHtML

[S57] C++：编译期常量
来源：http://wap.vehdjk.com/Article/details/gkrntgsis.sHtML

constexpr int N = 10;
来源：http://m.share.tarul.cn/Article/details/gvaeygujh.sHtML

[S58] C++：命名空间
来源：http://wap.sjlbkw.cn/Article/details/ggpjdndgk.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.sjlbkw.cn/Article/details/goisyffdq.sHtML

[S59] C++：静态断言
来源：http://www.m.share.bbcook.cn/Article/details/gztjyczzr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.tarul.cn/Article/details/gwpxfmgzs.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.yfazqb.com/Article/details/gvlekovjz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.sjlbkw.cn/Article/details/gejtekkmi.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gjppcscuk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fktsv.cn/Article/details/gshhfxgyf.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gvidehmmr.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/gbtbixxzt.sHtML

println("Hello")
来源：http://www.m.share.fktsv.cn/Article/details/gahkmqitw.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gkviccpjy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.bbcook.cn/Article/details/gmfkktbau.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.tarul.cn/Article/details/gcgzahhrp.sHtML

"值: $b"
来源：http://3g.yfazqb.com/Article/details/gafejtsjx.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.epnwcf.com/Article/details/gwjjadihj.sHtML

val n: String? = null;  n?.length
来源：http://wap.vehdjk.com/Article/details/gnmwsmeks.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.yfazqb.com/Article/details/gbskdclci.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.vehdjk.com/Article/details/gecierhpk.sHtML

[T06] Kotlin：集合映射
来源：http://wap.bbcook.cn/Article/details/gnitlzlmm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fktsv.cn/Article/details/ggcpyiozg.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fktsv.cn/Article/details/gzvtrnypq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.epnwcf.com/Article/details/gnlqxtwgr.sHtML

[T08] Kotlin：数据类
来源：http://www.share.sjlbkw.cn/Article/details/gokkvtxqe.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.sjlbkw.cn/Article/details/gzfpcwbcn.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fktsv.cn/Article/details/glqvcdohz.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.sjlbkw.cn/Article/details/gdlrwfxwo.sHtML

[T10] Kotlin：默认参数
来源：http://wap.sjlbkw.cn/Article/details/gihtydqxj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.tarul.cn/Article/details/gzsjtvqgg.sHtML

[T11] Kotlin：协程
来源：http://www.blog.tarul.cn/Article/details/gvxsfldiw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.vehdjk.com/Article/details/gkmoaxlxk.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.tarul.cn/Article/details/gwleiects.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.tarul.cn/Article/details/ghsvldpkr.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.tarul.cn/Article/details/gyaqgkyzv.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fktsv.cn/Article/details/gnbzeftyi.sHtML

[T14] Kotlin：循环
来源：http://www.blog.sjlbkw.cn/Article/details/gembpvxiv.sHtML

for (i in 1..10) println(i)
来源：http://read.share.sjlbkw.cn/Article/details/gyndjklvt.sHtML

[T15] Kotlin：接口
来源：http://blog.sjlbkw.cn/Article/details/ggkavsxaa.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.tarul.cn/Article/details/glhesijyk.sHtML

[T16] Swift：Hello World
来源：http://blog.sjlbkw.cn/Article/details/gdogaxnuf.sHtML

print("Hello")
来源：http://wap.bbcook.cn/Article/details/gkkgevpml.sHtML

[T17] Swift：变量与常量
来源：http://m.share.yfazqb.com/Article/details/ggqpcbgdx.sHtML

var a = 1;  let b = 2
来源：http://mobile.vehdjk.com/Article/details/ghsuzinqs.sHtML

[T18] Swift：字符串插值
来源：http://mobile.yfazqb.com/Article/details/gntandzdj.sHtML

"值: \(b)"
来源：http://baike.fktsv.cn/Article/details/gfvbyeaif.sHtML

[T19] Swift：可选绑定
来源：http://blog.epnwcf.com/Article/details/gjzvqgdgx.sHtML

if let n = opt { print(n) }
来源：http://wap.yfazqb.com/Article/details/gamcwertf.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fktsv.cn/Article/details/grtfcsmgq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fktsv.cn/Article/details/gxegapyqu.sHtML

[T21] Swift：遍历
来源：http://baike.tarul.cn/Article/details/gtbtqvoki.sHtML

for x in a { print(x) }
来源：http://mobile.tarul.cn/Article/details/gbfsvlpmp.sHtML

[T22] Swift：字典
来源：http://read.share.tarul.cn/Article/details/gdeppuics.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.vehdjk.com/Article/details/gsrnmkhnk.sHtML

[T23] Swift：函数
来源：http://mobile.fktsv.cn/Article/details/gchgdelkj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.epnwcf.com/Article/details/goermhhul.sHtML

[T24] Swift：闭包
来源：http://3g.epnwcf.com/Article/details/grwimpzkn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.tarul.cn/Article/details/gptcmugrp.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fktsv.cn/Article/details/gjwrpreho.sHtML

struct P { var x: Int }
来源：http://blog.tarul.cn/Article/details/gyhsnkdbr.sHtML

[T26] Swift：类与重写
来源：http://www.share.yfazqb.com/Article/details/gzvviewrf.sHtML

class A: Base { override func f() {} }
来源：http://read.share.bbcook.cn/Article/details/gatlnibih.sHtML

[T27] Swift：错误处理
来源：http://wap.yfazqb.com/Article/details/gihhwitxe.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.bbcook.cn/Article/details/gwspsmrwu.sHtML

[T28] Swift：枚举
来源：http://m.share.epnwcf.com/Article/details/gqdzdujlq.sHtML

enum Color { case red, green }
来源：http://m.share.sjlbkw.cn/Article/details/gtxjovlsl.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.sjlbkw.cn/Article/details/ggkbhnvoj.sHtML

guard let x = opt else { return }
来源：http://mobile.fktsv.cn/Article/details/gexueojrc.sHtML

[T30] Swift：协议
来源：http://baike.fktsv.cn/Article/details/gsoyqvxqv.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fktsv.cn/Article/details/guubknzls.sHtML

[T31] Lua：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/gbdnjrgca.sHtML

print("Hello")
来源：http://www.blog.fktsv.cn/Article/details/gdwvdmwnj.sHtML

[T32] Lua：局部变量
来源：http://baike.fktsv.cn/Article/details/gzwehjojm.sHtML

local a = 1
来源：http://blog.bbcook.cn/Article/details/gcsfgkrqq.sHtML

[T33] Lua：表（数组）
来源：http://mobile.vehdjk.com/Article/details/gxunwvvdq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.bbcook.cn/Article/details/gtgcxjmkd.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.tarul.cn/Article/details/grwssfsqn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.bbcook.cn/Article/details/gediyudgl.sHtML

[T35] Lua：字典表
来源：http://www.blog.fktsv.cn/Article/details/guupriemq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.vehdjk.com/Article/details/gmlafqwso.sHtML

[T36] Lua：函数
来源：http://3g.sjlbkw.cn/Article/details/gkuwrffyx.sHtML

function add(a, b) return a + b end
来源：http://m.share.bbcook.cn/Article/details/gxnojxyby.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.vehdjk.com/Article/details/ghayklnud.sHtML

"a" .. "b"
来源：http://baike.vehdjk.com/Article/details/gpcjdlard.sHtML

[T38] Lua：条件
来源：http://read.share.epnwcf.com/Article/details/guoxyqltw.sHtML

if x > 0 then print("正") end
来源：http://wap.yfazqb.com/Article/details/gnfvtmlze.sHtML

[T39] Lua：模式匹配
来源：http://baike.sjlbkw.cn/Article/details/gahxultju.sHtML

string.find(s, "%d+")
来源：http://mobile.fktsv.cn/Article/details/gdusqpmyo.sHtML

[T40] Lua：元表
来源：http://m.share.sjlbkw.cn/Article/details/grnqizrse.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.tarul.cn/Article/details/gjmvyttse.sHtML

[T41] Perl：Hello World
来源：http://read.share.vehdjk.com/Article/details/gdlcwybsj.sHtML

print "Hello\n";
来源：http://m.share.fktsv.cn/Article/details/gsvturbku.sHtML

[T42] Perl：变量类型
来源：http://www.blog.bbcook.cn/Article/details/gfpkdhrmu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fktsv.cn/Article/details/gjlwtkskl.sHtML

[T43] Perl：字符串插值
来源：http://m.share.epnwcf.com/Article/details/gfickgzop.sHtML

"值: $a"
来源：http://read.share.yfazqb.com/Article/details/gnomexaba.sHtML

[T44] Perl：条件
来源：http://read.share.yfazqb.com/Article/details/gqdvidpet.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.epnwcf.com/Article/details/gtmxogdrk.sHtML


<!-- 参考信息 -->