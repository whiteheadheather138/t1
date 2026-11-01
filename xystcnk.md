代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.vehdjk.com/Article/details/gykgpwgkj.sHtML

[R48] awk 取指定列
来源：http://3g.sjlbkw.cn/Article/details/gjxxmydtt.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fktsv.cn/Article/details/gorswiruo.sHtML

[R49] awk 带条件
来源：http://www.m.share.yfazqb.com/Article/details/gniogtjqz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.vehdjk.com/Article/details/gboqwtjwi.sHtML

[R50] awk 求和
来源：http://www.blog.tarul.cn/Article/details/gkzrdawgx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fktsv.cn/Article/details/gdqeiaikx.sHtML

[R51] 排序去重取前几
来源：http://baike.yfazqb.com/Article/details/gpllkyure.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.yfazqb.com/Article/details/gkjtybocl.sHtML

[R52] 统计行数
来源：http://mobile.sjlbkw.cn/Article/details/guolzsulx.sHtML

wc -l a.txt
来源：http://blog.bbcook.cn/Article/details/gqemwjxxk.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.epnwcf.com/Article/details/grjfanskf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.sjlbkw.cn/Article/details/gvnyhqimz.sHtML

[R54] 比较两个文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gloueahfz.sHtML

diff a.txt b.txt
来源：http://www.share.yfazqb.com/Article/details/gxlnodedm.sHtML

[R55] 压缩与解压
来源：http://blog.fktsv.cn/Article/details/gewoankom.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.bbcook.cn/Article/details/grxmuihnh.sHtML

[R56] 远程拷贝
来源：http://m.share.epnwcf.com/Article/details/gzbvqyhqu.sHtML

scp file user@host:/path/
来源：http://3g.epnwcf.com/Article/details/gujjlacrh.sHtML

[R57] 远程执行命令
来源：http://baike.fktsv.cn/Article/details/gydccpkhg.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fktsv.cn/Article/details/gsamlobmj.sHtML

[R58] 下载文件
来源：http://blog.fktsv.cn/Article/details/gzymahmfn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.yfazqb.com/Article/details/gfuvosbhw.sHtML

[R59] 发 POST JSON
来源：http://mobile.sjlbkw.cn/Article/details/gezrqxocf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fktsv.cn/Article/details/gvaqevbyz.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.sjlbkw.cn/Article/details/ghjlxwgzb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.yfazqb.com/Article/details/gvtxaanpa.sHtML

[R61] 磁盘占用
来源：http://blog.sjlbkw.cn/Article/details/goudpupus.sHtML

df -h;  du -sh *
来源：http://www.m.share.vehdjk.com/Article/details/ghjbkdduf.sHtML

[R62] 找最占空间的文件
来源：http://baike.fktsv.cn/Article/details/gyldujxgt.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.tarul.cn/Article/details/gvwrrmgrd.sHtML

[R63] 内存与进程
来源：http://blog.fktsv.cn/Article/details/gihndgzow.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.sjlbkw.cn/Article/details/gtygwizwo.sHtML

[R64] 结束进程
来源：http://wap.epnwcf.com/Article/details/ginxgyrko.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.epnwcf.com/Article/details/goqzwcasi.sHtML

[R65] 查看端口占用
来源：http://www.m.share.sjlbkw.cn/Article/details/gizsctwiq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.bbcook.cn/Article/details/guzblotgh.sHtML

[R66] 定时任务
来源：http://wap.vehdjk.com/Article/details/gzaelelxk.sHtML

crontab -e;  crontab -l
来源：http://3g.bbcook.cn/Article/details/giqzefcry.sHtML

[R67] 生成随机十六进制串
来源：http://blog.tarul.cn/Article/details/gntxrqptv.sHtML

openssl rand -hex 16
来源：http://blog.bbcook.cn/Article/details/gkzftmqht.sHtML

[R68] 计算文件校验值
来源：http://www.blog.tarul.cn/Article/details/gweizkxvc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.bbcook.cn/Article/details/gutbntskf.sHtML

[R69] 生成随机密码
来源：http://www.share.epnwcf.com/Article/details/gbaiqalsp.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.bbcook.cn/Article/details/gapokcsvs.sHtML

[R70] 时间戳与互转
来源：http://3g.yfazqb.com/Article/details/gfvayroqe.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fktsv.cn/Article/details/gxyvzrfro.sHtML

[R71] 日期格式化
来源：http://www.blog.yfazqb.com/Article/details/gjdzmmamd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.bbcook.cn/Article/details/gumnaifww.sHtML

[R72] 等待端口就绪
来源：http://baike.epnwcf.com/Article/details/ghfcdqoje.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.vehdjk.com/Article/details/gvvyvftrx.sHtML

[R73] 分割大日志
来源：http://blog.tarul.cn/Article/details/ghzjuaqrr.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.yfazqb.com/Article/details/gmtrlkwtw.sHtML

[R74] 批量重命名
来源：http://www.blog.epnwcf.com/Article/details/gdznjodog.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.sjlbkw.cn/Article/details/gfghfjmle.sHtML

[R75] 导出环境变量
来源：http://www.share.bbcook.cn/Article/details/guuiapnin.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.bbcook.cn/Article/details/gdbzcenoc.sHtML

[R76] 使用临时文件
来源：http://blog.vehdjk.com/Article/details/gkwobqvoi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.epnwcf.com/Article/details/gksjlgsyp.sHtML

[R77] 读取用户输入
来源：http://blog.yfazqb.com/Article/details/groylwcpy.sHtML

read -rp "请输入: " ans
来源：http://baike.bbcook.cn/Article/details/gicxpbqde.sHtML

[R78] 交互式菜单
来源：http://www.blog.yfazqb.com/Article/details/gvvyqevou.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.tarul.cn/Article/details/gsemovhfy.sHtML

[R79] 解析命令行选项
来源：http://wap.tarul.cn/Article/details/gthsdmrmj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.bbcook.cn/Article/details/gyxrxkrdg.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.tarul.cn/Article/details/gxmrjgyrq.sHtML

time ./run.sh
来源：http://baike.bbcook.cn/Article/details/gmcwapygw.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/glnqecycb.sHtML

S. C / C++ 专题
来源：http://wap.epnwcf.com/Article/details/gyardcjcp.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gbfeoopdy.sHtML

[S01] C：Hello World
来源：http://baike.epnwcf.com/Article/details/gdpzlpuop.sHtML

#include <stdio.h>
来源：http://baike.sjlbkw.cn/Article/details/gzslsjmpo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.epnwcf.com/Article/details/gbncaigpm.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.bbcook.cn/Article/details/gldyniquj.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.epnwcf.com/Article/details/gtddyfoyy.sHtML

[S03] C：读入整数
来源：http://www.blog.tarul.cn/Article/details/gpdvkxvnk.sHtML

int x; scanf("%d", &x);
来源：http://mobile.sjlbkw.cn/Article/details/gtytcrgau.sHtML

[S04] C：字符串复制
来源：http://mobile.vehdjk.com/Article/details/gpjmfrgqu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.yfazqb.com/Article/details/gqejbtylv.sHtML

[S05] C：字符串长度
来源：http://read.share.yfazqb.com/Article/details/glczvtfbc.sHtML

strlen(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkolmduhg.sHtML

[S06] C：字符串比较
来源：http://3g.tarul.cn/Article/details/ggfwdtwia.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fktsv.cn/Article/details/gvgjeptgh.sHtML

[S07] C：数组遍历求和
来源：http://m.share.yfazqb.com/Article/details/gupkiwhnr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.bbcook.cn/Article/details/guhnjzyxc.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.vehdjk.com/Article/details/gmfkedygn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.sjlbkw.cn/Article/details/gzfbkuiem.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fktsv.cn/Article/details/gdjntznxs.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.sjlbkw.cn/Article/details/gadkbpwlw.sHtML

[S10] C：指针与解引用
来源：http://wap.vehdjk.com/Article/details/gzcxbxzay.sHtML

int *p = &a;  *p = 5;
来源：http://baike.yfazqb.com/Article/details/ggonplvjr.sHtML

[S11] C：逐行读文件
来源：http://www.share.sjlbkw.cn/Article/details/gwfwqcdtf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.bbcook.cn/Article/details/gagjsyhbd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fktsv.cn/Article/details/gpaxiurwb.sHtML

fclose(f);
来源：http://3g.sjlbkw.cn/Article/details/gvogxsxac.sHtML

[S12] C：写文件
来源：http://www.m.share.epnwcf.com/Article/details/gxekgmmtd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.yfazqb.com/Article/details/gepmtwkck.sHtML

[S13] C：宏定义
来源：http://mobile.yfazqb.com/Article/details/gjpfvilrx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.sjlbkw.cn/Article/details/grmkqfday.sHtML

[S14] C：枚举
来源：http://read.share.tarul.cn/Article/details/gqusmonnu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.vehdjk.com/Article/details/galpqycjq.sHtML

[S15] C：类型转换
来源：http://www.share.fktsv.cn/Article/details/glcjacyhd.sHtML

(double) a / b
来源：http://www.blog.yfazqb.com/Article/details/gpzumoyge.sHtML

[S16] C：位操作置位
来源：http://3g.tarul.cn/Article/details/gptwlbhdz.sHtML

x |= (1 << 3);
来源：http://mobile.sjlbkw.cn/Article/details/gwnjpyktv.sHtML

[S17] C：安全拼接字符串
来源：http://blog.sjlbkw.cn/Article/details/grasfrvul.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.bbcook.cn/Article/details/gvzyehnjc.sHtML

[S18] C：命令行参数
来源：http://www.blog.tarul.cn/Article/details/gzuroluvu.sHtML

int main(int argc, char **argv)
来源：http://baike.vehdjk.com/Article/details/gafuheexq.sHtML

[S19] C：快速排序
来源：http://mobile.yfazqb.com/Article/details/gckumyvkp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.vehdjk.com/Article/details/gvewvnjgn.sHtML

[S20] C：二分查找
来源：http://wap.epnwcf.com/Article/details/gvhzifeai.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.yfazqb.com/Article/details/gtdxfhbsh.sHtML

[S21] C：字符类别判断
来源：http://mobile.bbcook.cn/Article/details/gdpwpquco.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.sjlbkw.cn/Article/details/gyvmkhevq.sHtML

[S22] C：字符串转数字
来源：http://mobile.tarul.cn/Article/details/gsvxzyfwa.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.sjlbkw.cn/Article/details/gwvlzqlyb.sHtML

[S23] C：随机数
来源：http://read.share.vehdjk.com/Article/details/gvznbdwdu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.yfazqb.com/Article/details/gndxspjdo.sHtML

[S24] C：获取本地时间
来源：http://www.share.tarul.cn/Article/details/gtpibgllh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.tarul.cn/Article/details/gnihgzsgx.sHtML

[S25] C：内存拷贝
来源：http://www.share.fktsv.cn/Article/details/glvcqmftv.sHtML

memcpy(dst, src, n);
来源：http://mobile.tarul.cn/Article/details/gzlbgjzta.sHtML

[S26] C：内存清零
来源：http://read.share.tarul.cn/Article/details/gqnxnauxg.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fktsv.cn/Article/details/gtvepqezy.sHtML

[S27] C：定义常量
来源：http://baike.bbcook.cn/Article/details/gzdxylgxo.sHtML

const double PI = 3.14159;
来源：http://baike.fktsv.cn/Article/details/geombvbku.sHtML

[S28] C：静态变量
来源：http://blog.yfazqb.com/Article/details/gctsuxoik.sHtML

static int counter = 0;
来源：http://baike.yfazqb.com/Article/details/githcrsik.sHtML

[S29] C：变参函数
来源：http://m.share.fktsv.cn/Article/details/ghmdjktka.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.yfazqb.com/Article/details/gruuhppxb.sHtML

[S30] C：头文件保护
来源：http://3g.tarul.cn/Article/details/gnjtotpao.sHtML

#ifndef X_H
来源：http://m.share.epnwcf.com/Article/details/gyztqtlgw.sHtML

#define X_H
来源：http://baike.epnwcf.com/Article/details/gedmifyto.sHtML

#endif
来源：http://3g.epnwcf.com/Article/details/gjvxopxpf.sHtML

[S31] C++：Hello World
来源：http://www.share.yfazqb.com/Article/details/gmdtzzvhp.sHtML

#include <iostream>
来源：http://www.share.epnwcf.com/Article/details/gnzhbcojw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.tarul.cn/Article/details/gjixmgkqj.sHtML

[S32] C++：字符串
来源：http://baike.fktsv.cn/Article/details/gaaazvgbr.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.yfazqb.com/Article/details/givwxuifc.sHtML

[S33] C++：vector 增删
来源：http://3g.bbcook.cn/Article/details/gjagkehxa.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.tarul.cn/Article/details/gzewlgmja.sHtML

[S34] C++：遍历 vector
来源：http://3g.sjlbkw.cn/Article/details/giylwufzz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.epnwcf.com/Article/details/ghtbnzqmf.sHtML

[S35] C++：map
来源：http://mobile.tarul.cn/Article/details/glttstuxi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.yfazqb.com/Article/details/grcxkdlwu.sHtML

[S36] C++：unordered_map
来源：http://mobile.bbcook.cn/Article/details/gvywrrmbv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.sjlbkw.cn/Article/details/gmqauvwgi.sHtML

[S37] C++：set
来源：http://3g.sjlbkw.cn/Article/details/gpzxodtjc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.vehdjk.com/Article/details/ghifgoizd.sHtML

[S38] C++：排序
来源：http://3g.yfazqb.com/Article/details/ggpmkfmxz.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.tarul.cn/Article/details/gnrgxgblw.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.bbcook.cn/Article/details/gxsfvzgnw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.tarul.cn/Article/details/gxiyonjal.sHtML

[S40] C++：查找元素
来源：http://3g.tarul.cn/Article/details/geepbnejo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fktsv.cn/Article/details/gsnaenctr.sHtML

[S41] C++：类与构造函数
来源：http://mobile.tarul.cn/Article/details/gcvxzpqef.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.bbcook.cn/Article/details/gceisalmc.sHtML

[S42] C++：继承与虚函数
来源：http://wap.tarul.cn/Article/details/gtmohzowx.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.vehdjk.com/Article/details/gktuhsafy.sHtML

[S43] C++：智能指针
来源：http://baike.sjlbkw.cn/Article/details/gavuctfzf.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fktsv.cn/Article/details/ghkrvmhoe.sHtML

[S44] C++：引用传参
来源：http://read.share.vehdjk.com/Article/details/gjavtplro.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.epnwcf.com/Article/details/gzfqtxljw.sHtML

[S45] C++：lambda
来源：http://wap.sjlbkw.cn/Article/details/gtfypyfxs.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.sjlbkw.cn/Article/details/gevzuckqv.sHtML

[S46] C++：函数模板
来源：http://www.blog.tarul.cn/Article/details/gqxigeqxp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.vehdjk.com/Article/details/gixtqucyx.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.epnwcf.com/Article/details/gpwdbynkq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fktsv.cn/Article/details/gtamdzqmb.sHtML

[S48] C++：逐行读文件
来源：http://www.share.vehdjk.com/Article/details/goccrphup.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.epnwcf.com/Article/details/geewbjoln.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fktsv.cn/Article/details/gsvcbhuqc.sHtML

[S49] C++：写文件
来源：http://baike.fktsv.cn/Article/details/gjthzewej.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.bbcook.cn/Article/details/gificevag.sHtML

[S50] C++：格式化数字
来源：http://wap.sjlbkw.cn/Article/details/gysmarrsv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/gglsabzvn.sHtML

[S51] C++：显式类型转换
来源：http://blog.epnwcf.com/Article/details/gqkidkhfe.sHtML

static_cast<double>(a) / b
来源：http://wap.fktsv.cn/Article/details/gdzibfatu.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.vehdjk.com/Article/details/gtopgrwgo.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.vehdjk.com/Article/details/gurbbvusa.sHtML

[S53] C++：移动语义
来源：http://www.m.share.epnwcf.com/Article/details/gweqfvyti.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.yfazqb.com/Article/details/gjylpvjfv.sHtML

[S54] C++：异常处理
来源：http://mobile.sjlbkw.cn/Article/details/gaefwfmxq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fktsv.cn/Article/details/gqbdeskjb.sHtML

[S55] C++：结构化绑定
来源：http://3g.yfazqb.com/Article/details/gcuwwbxkn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.tarul.cn/Article/details/gucrhnioo.sHtML

[S56] C++：optional
来源：http://wap.sjlbkw.cn/Article/details/gqqmpqqfo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fktsv.cn/Article/details/ggacfshsq.sHtML

[S57] C++：编译期常量
来源：http://3g.tarul.cn/Article/details/gtjbmrwta.sHtML

constexpr int N = 10;
来源：http://wap.tarul.cn/Article/details/gefbqizma.sHtML

[S58] C++：命名空间
来源：http://wap.tarul.cn/Article/details/ggggqhawg.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.yfazqb.com/Article/details/ghrdnuqlx.sHtML

[S59] C++：静态断言
来源：http://blog.bbcook.cn/Article/details/gpueycaew.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.sjlbkw.cn/Article/details/gblqyhvju.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.epnwcf.com/Article/details/gfstaakzy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.tarul.cn/Article/details/giqkqjdsc.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/glnsxipsb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.vehdjk.com/Article/details/gpdnuycxs.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gatvfvesi.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.bbcook.cn/Article/details/gkbzcjruj.sHtML

println("Hello")
来源：http://www.share.yfazqb.com/Article/details/grungjxmt.sHtML

[T02] Kotlin：变量
来源：http://read.share.fktsv.cn/Article/details/gcwsyvxra.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.yfazqb.com/Article/details/gnljebfli.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.epnwcf.com/Article/details/gfemruxri.sHtML

"值: $b"
来源：http://mobile.bbcook.cn/Article/details/gfxzwnfqq.sHtML

[T04] Kotlin：空安全
来源：http://baike.yfazqb.com/Article/details/glsrpwebg.sHtML

val n: String? = null;  n?.length
来源：http://blog.tarul.cn/Article/details/ggwyfsdyl.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fktsv.cn/Article/details/gqlpxlfkb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fktsv.cn/Article/details/gijwnfhzx.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.vehdjk.com/Article/details/gzzuqqhsx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.vehdjk.com/Article/details/gdlxcsusa.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.tarul.cn/Article/details/ghoqiqlyg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.tarul.cn/Article/details/gbslsphbc.sHtML

[T08] Kotlin：数据类
来源：http://blog.bbcook.cn/Article/details/gvwfrlroo.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.vehdjk.com/Article/details/geanociru.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.yfazqb.com/Article/details/gusdfneay.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.vehdjk.com/Article/details/gnswjgqdy.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.vehdjk.com/Article/details/gcucdvaiv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.bbcook.cn/Article/details/gipbuciqz.sHtML

[T11] Kotlin：协程
来源：http://wap.sjlbkw.cn/Article/details/gazdcocln.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.yfazqb.com/Article/details/gdamzrdit.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fktsv.cn/Article/details/ggffgwcui.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.sjlbkw.cn/Article/details/gwmybumli.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.tarul.cn/Article/details/gnbjliwbo.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.bbcook.cn/Article/details/gdoxcjfzr.sHtML

[T14] Kotlin：循环
来源：http://mobile.vehdjk.com/Article/details/gkmacnjio.sHtML

for (i in 1..10) println(i)
来源：http://www.share.vehdjk.com/Article/details/gwxosvsuh.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.epnwcf.com/Article/details/guwcahoxy.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.vehdjk.com/Article/details/gcqteqdpc.sHtML

[T16] Swift：Hello World
来源：http://read.share.epnwcf.com/Article/details/gmxuxbvma.sHtML

print("Hello")
来源：http://m.share.yfazqb.com/Article/details/gczrjaoub.sHtML

[T17] Swift：变量与常量
来源：http://baike.yfazqb.com/Article/details/gmgplnyiw.sHtML

var a = 1;  let b = 2
来源：http://www.share.vehdjk.com/Article/details/grnejvzhf.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.bbcook.cn/Article/details/gxtttdeus.sHtML

"值: \(b)"
来源：http://www.blog.epnwcf.com/Article/details/gxrmodbsg.sHtML

[T19] Swift：可选绑定
来源：http://blog.bbcook.cn/Article/details/gnmqophjv.sHtML

if let n = opt { print(n) }
来源：http://blog.bbcook.cn/Article/details/gryaxokii.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.tarul.cn/Article/details/gnvwjcwdq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.sjlbkw.cn/Article/details/gdslxqqhk.sHtML

[T21] Swift：遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/ghmbyzwry.sHtML

for x in a { print(x) }
来源：http://www.share.bbcook.cn/Article/details/gndqulgdo.sHtML

[T22] Swift：字典
来源：http://blog.fktsv.cn/Article/details/gskwxqimw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.vehdjk.com/Article/details/gwdxbjdix.sHtML

[T23] Swift：函数
来源：http://wap.yfazqb.com/Article/details/gbpugpgwv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.tarul.cn/Article/details/gtbzsuxlx.sHtML

[T24] Swift：闭包
来源：http://blog.fktsv.cn/Article/details/gprghkexv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fktsv.cn/Article/details/gxzsudukr.sHtML

[T25] Swift：结构体
来源：http://www.blog.sjlbkw.cn/Article/details/gqqewypkx.sHtML

struct P { var x: Int }
来源：http://baike.fktsv.cn/Article/details/genbnvurh.sHtML

[T26] Swift：类与重写
来源：http://www.share.yfazqb.com/Article/details/gqllvxmyl.sHtML

class A: Base { override func f() {} }
来源：http://wap.bbcook.cn/Article/details/gtszchjtx.sHtML

[T27] Swift：错误处理
来源：http://read.share.sjlbkw.cn/Article/details/grvkfsnps.sHtML

do { try f() } catch { print(error) }
来源：http://blog.yfazqb.com/Article/details/gvhptaoge.sHtML

[T28] Swift：枚举
来源：http://m.share.vehdjk.com/Article/details/ggiiuazog.sHtML

enum Color { case red, green }
来源：http://read.share.fktsv.cn/Article/details/gpnfnbcdq.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.epnwcf.com/Article/details/grjpftrqz.sHtML

guard let x = opt else { return }
来源：http://www.m.share.yfazqb.com/Article/details/gzqfwfhif.sHtML

[T30] Swift：协议
来源：http://www.share.tarul.cn/Article/details/gqlzjqswt.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.tarul.cn/Article/details/gthnpqrpw.sHtML

[T31] Lua：Hello World
来源：http://wap.bbcook.cn/Article/details/ghprclowd.sHtML

print("Hello")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxhkvmyrf.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.epnwcf.com/Article/details/gsfruovsa.sHtML

local a = 1
来源：http://baike.epnwcf.com/Article/details/gasdwmkdl.sHtML

[T33] Lua：表（数组）
来源：http://m.share.vehdjk.com/Article/details/grzdhfkjc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.sjlbkw.cn/Article/details/gkhlbseae.sHtML

[T34] Lua：遍历表
来源：http://mobile.sjlbkw.cn/Article/details/gksmieskh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.yfazqb.com/Article/details/gqgskjzqs.sHtML

[T35] Lua：字典表
来源：http://m.share.yfazqb.com/Article/details/gufjdtpmj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.vehdjk.com/Article/details/gaegzfock.sHtML

[T36] Lua：函数
来源：http://www.m.share.tarul.cn/Article/details/gbzcquvwc.sHtML

function add(a, b) return a + b end
来源：http://blog.yfazqb.com/Article/details/gjhpxakbe.sHtML

[T37] Lua：字符串拼接
来源：http://wap.vehdjk.com/Article/details/gtapvrjci.sHtML

"a" .. "b"
来源：http://3g.fktsv.cn/Article/details/gdadylzhs.sHtML

[T38] Lua：条件
来源：http://mobile.bbcook.cn/Article/details/gmvruodcp.sHtML

if x > 0 then print("正") end
来源：http://www.blog.sjlbkw.cn/Article/details/gspucxgtr.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fktsv.cn/Article/details/grykxepen.sHtML

string.find(s, "%d+")
来源：http://3g.sjlbkw.cn/Article/details/gfbyydhbe.sHtML

[T40] Lua：元表
来源：http://www.share.epnwcf.com/Article/details/gucqoajcv.sHtML

setmetatable({}, { __index = base })
来源：http://wap.vehdjk.com/Article/details/gcdtohemu.sHtML

[T41] Perl：Hello World
来源：http://www.share.vehdjk.com/Article/details/gooobkjvh.sHtML

print "Hello\n";
来源：http://www.blog.epnwcf.com/Article/details/gisursaln.sHtML

[T42] Perl：变量类型
来源：http://read.share.bbcook.cn/Article/details/giiympgoz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.vehdjk.com/Article/details/gtwumqsdg.sHtML

[T43] Perl：字符串插值
来源：http://mobile.sjlbkw.cn/Article/details/gzwxfurfx.sHtML

"值: $a"
来源：http://mobile.epnwcf.com/Article/details/gfmqvmomh.sHtML

[T44] Perl：条件
来源：http://www.blog.bbcook.cn/Article/details/glscwiczg.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.yfazqb.com/Article/details/grachsmrh.sHtML

[T45] Perl：数组遍历
来源：http://blog.bbcook.cn/Article/details/gpwcmvduu.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.bbcook.cn/Article/details/gigzcbucy.sHtML

[T46] Perl：哈希操作
来源：http://read.share.bbcook.cn/Article/details/gukcfuuek.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.epnwcf.com/Article/details/gqihtijhu.sHtML

[T47] Perl：正则捕获
来源：http://baike.tarul.cn/Article/details/ghusscdja.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.bbcook.cn/Article/details/gohcsvaub.sHtML

[T48] Perl：正则替换
来源：http://wap.bbcook.cn/Article/details/glbnukzrc.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.yfazqb.com/Article/details/gjwmsdiha.sHtML

[T49] Perl：函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gmcxewemr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.tarul.cn/Article/details/ghmehwctj.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.yfazqb.com/Article/details/gvltkfdrf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.vehdjk.com/Article/details/ghzkclvwe.sHtML


<!-- 参考信息 -->