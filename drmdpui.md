代发 wailian999

cmd > out.log 2>&1
来源：http://www.m.share.epnwcf.com/Article/details/gzhxnjqgl.sHtML

[R40] 追加写日志
来源：http://mobile.bbcook.cn/Article/details/gcqylldsf.sHtML

echo "log" >> out.log
来源：http://www.blog.sjlbkw.cn/Article/details/gkjmhaigd.sHtML

[R41] 丢弃输出
来源：http://mobile.fktsv.cn/Article/details/gziagodui.sHtML

cmd >/dev/null 2>&1
来源：http://wap.yfazqb.com/Article/details/gwsgxcday.sHtML

[R42] 输入重定向
来源：http://www.m.share.bbcook.cn/Article/details/gfzsuxnug.sHtML

wc -l < a.txt
来源：http://m.share.bbcook.cn/Article/details/gudqcicnc.sHtML

[R43] 按名字查找文件
来源：http://m.share.fktsv.cn/Article/details/gxfzdosip.sHtML

find . -name "*.log" -type f
来源：http://m.share.epnwcf.com/Article/details/gzdpivwmd.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.epnwcf.com/Article/details/gzmbecswj.sHtML

find . -mtime -7 -type f
来源：http://blog.yfazqb.com/Article/details/gjcbplbgt.sHtML

[R45] 批量删除
来源：http://3g.tarul.cn/Article/details/gxzoziwvy.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.sjlbkw.cn/Article/details/gimpzhcza.sHtML

[R46] 递归替换文件内容
来源：http://blog.fktsv.cn/Article/details/gtisuhnzu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.bbcook.cn/Article/details/gruyhbtzy.sHtML

[R47] sed 单行替换
来源：http://read.share.fktsv.cn/Article/details/gvjprebtb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.epnwcf.com/Article/details/gbzzcetil.sHtML

[R48] awk 取指定列
来源：http://www.m.share.epnwcf.com/Article/details/gvbemslpg.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.bbcook.cn/Article/details/gnntisdwp.sHtML

[R49] awk 带条件
来源：http://baike.fktsv.cn/Article/details/gmeynyzcl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.epnwcf.com/Article/details/gxdizmkzm.sHtML

[R50] awk 求和
来源：http://baike.sjlbkw.cn/Article/details/gsmwhqioa.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.yfazqb.com/Article/details/gmrteafzx.sHtML

[R51] 排序去重取前几
来源：http://blog.fktsv.cn/Article/details/gylsbmzmv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.yfazqb.com/Article/details/gryetyblg.sHtML

[R52] 统计行数
来源：http://mobile.tarul.cn/Article/details/geubbrajc.sHtML

wc -l a.txt
来源：http://www.m.share.yfazqb.com/Article/details/gqfuuzkxw.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.yfazqb.com/Article/details/guyuuloew.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.sjlbkw.cn/Article/details/ggbqisaoe.sHtML

[R54] 比较两个文件
来源：http://mobile.yfazqb.com/Article/details/gbmumxgyw.sHtML

diff a.txt b.txt
来源：http://wap.fktsv.cn/Article/details/grsguqwze.sHtML

[R55] 压缩与解压
来源：http://m.share.tarul.cn/Article/details/gotfoysml.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.bbcook.cn/Article/details/gtkcptxbz.sHtML

[R56] 远程拷贝
来源：http://m.share.sjlbkw.cn/Article/details/gymjabkxk.sHtML

scp file user@host:/path/
来源：http://www.blog.bbcook.cn/Article/details/gkxndaleh.sHtML

[R57] 远程执行命令
来源：http://baike.sjlbkw.cn/Article/details/gshdtabml.sHtML

ssh user@host 'uptime'
来源：http://baike.epnwcf.com/Article/details/gqkxiiofm.sHtML

[R58] 下载文件
来源：http://www.m.share.vehdjk.com/Article/details/gjzneznfl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.vehdjk.com/Article/details/gtityqtmu.sHtML

[R59] 发 POST JSON
来源：http://mobile.yfazqb.com/Article/details/gtgmzmckz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fktsv.cn/Article/details/gchoqdelg.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.epnwcf.com/Article/details/gmddsuetl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.sjlbkw.cn/Article/details/gjydvsiql.sHtML

[R61] 磁盘占用
来源：http://blog.bbcook.cn/Article/details/gnbjqkncg.sHtML

df -h;  du -sh *
来源：http://www.blog.bbcook.cn/Article/details/gxlxraayk.sHtML

[R62] 找最占空间的文件
来源：http://wap.bbcook.cn/Article/details/gomurztff.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.sjlbkw.cn/Article/details/ggkxvxoua.sHtML

[R63] 内存与进程
来源：http://mobile.fktsv.cn/Article/details/gdpvwvrzi.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.sjlbkw.cn/Article/details/giuiefsoh.sHtML

[R64] 结束进程
来源：http://mobile.vehdjk.com/Article/details/gpbxrpglm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.epnwcf.com/Article/details/govzguwfm.sHtML

[R65] 查看端口占用
来源：http://www.m.share.yfazqb.com/Article/details/guoqdhtgz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.tarul.cn/Article/details/gndbgpkgq.sHtML

[R66] 定时任务
来源：http://baike.yfazqb.com/Article/details/gitlpyyjg.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.bbcook.cn/Article/details/gmlopawoy.sHtML

[R67] 生成随机十六进制串
来源：http://blog.bbcook.cn/Article/details/gwspivepa.sHtML

openssl rand -hex 16
来源：http://www.share.sjlbkw.cn/Article/details/grryzvnpd.sHtML

[R68] 计算文件校验值
来源：http://blog.sjlbkw.cn/Article/details/gobdtevcp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fktsv.cn/Article/details/ghnmpwbjg.sHtML

[R69] 生成随机密码
来源：http://baike.yfazqb.com/Article/details/gsfbnbhix.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.epnwcf.com/Article/details/gkcripfua.sHtML

[R70] 时间戳与互转
来源：http://www.blog.sjlbkw.cn/Article/details/gijczcptr.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fktsv.cn/Article/details/gkojeonaf.sHtML

[R71] 日期格式化
来源：http://www.blog.epnwcf.com/Article/details/guaxaormk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.yfazqb.com/Article/details/goposxicg.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.sjlbkw.cn/Article/details/gpzxyeygj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.epnwcf.com/Article/details/gvktivzdj.sHtML

[R73] 分割大日志
来源：http://wap.sjlbkw.cn/Article/details/ggmnpdcbd.sHtML

split -l 1000 big.log part_
来源：http://read.share.sjlbkw.cn/Article/details/gtcswnidi.sHtML

[R74] 批量重命名
来源：http://m.share.epnwcf.com/Article/details/gyuxfivfd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.vehdjk.com/Article/details/gmljuufzd.sHtML

[R75] 导出环境变量
来源：http://www.blog.yfazqb.com/Article/details/gfqyxkddr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.epnwcf.com/Article/details/gmxmzjmuy.sHtML

[R76] 使用临时文件
来源：http://m.share.epnwcf.com/Article/details/gqysqchdd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fktsv.cn/Article/details/ggzftxsba.sHtML

[R77] 读取用户输入
来源：http://wap.vehdjk.com/Article/details/grcpyovkf.sHtML

read -rp "请输入: " ans
来源：http://baike.sjlbkw.cn/Article/details/gxdxjnmaf.sHtML

[R78] 交互式菜单
来源：http://blog.bbcook.cn/Article/details/giabcvwlw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.sjlbkw.cn/Article/details/gynqrttof.sHtML

[R79] 解析命令行选项
来源：http://baike.tarul.cn/Article/details/gyhodnhpk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.sjlbkw.cn/Article/details/gcwohoxdv.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.yfazqb.com/Article/details/gmdojdrlz.sHtML

time ./run.sh
来源：http://wap.tarul.cn/Article/details/gldndtwvv.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/ghczwvbvg.sHtML

S. C / C++ 专题
来源：http://blog.yfazqb.com/Article/details/ghojbbuyz.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/ggudclgjc.sHtML

[S01] C：Hello World
来源：http://www.share.epnwcf.com/Article/details/gokejwtfz.sHtML

#include <stdio.h>
来源：http://blog.fktsv.cn/Article/details/glplcmpnn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.yfazqb.com/Article/details/gpafqvpvl.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.sjlbkw.cn/Article/details/ggkifdbim.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fktsv.cn/Article/details/gdpnijmxe.sHtML

[S03] C：读入整数
来源：http://www.blog.yfazqb.com/Article/details/gptxvsfmf.sHtML

int x; scanf("%d", &x);
来源：http://m.share.yfazqb.com/Article/details/garkzeehm.sHtML

[S04] C：字符串复制
来源：http://mobile.yfazqb.com/Article/details/gbjxpytpf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.epnwcf.com/Article/details/ggmdsgifl.sHtML

[S05] C：字符串长度
来源：http://www.share.bbcook.cn/Article/details/gggyqexyy.sHtML

strlen(s)
来源：http://baike.fktsv.cn/Article/details/ggkxuugtj.sHtML

[S06] C：字符串比较
来源：http://3g.fktsv.cn/Article/details/giuqtmezo.sHtML

strcmp(a, b) == 0
来源：http://www.share.fktsv.cn/Article/details/gfijsfyfq.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fktsv.cn/Article/details/gnddulgeh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fktsv.cn/Article/details/gkxucnyry.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.sjlbkw.cn/Article/details/gnttmaosj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fktsv.cn/Article/details/gtsjyhxog.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.sjlbkw.cn/Article/details/gueirmrrt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.sjlbkw.cn/Article/details/ghwqyjtjq.sHtML

[S10] C：指针与解引用
来源：http://www.share.vehdjk.com/Article/details/geypwadqt.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.yfazqb.com/Article/details/ghjaqibjo.sHtML

[S11] C：逐行读文件
来源：http://blog.tarul.cn/Article/details/gloavgkms.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.tarul.cn/Article/details/gkpsdynnp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.yfazqb.com/Article/details/ggfjdywov.sHtML

fclose(f);
来源：http://read.share.fktsv.cn/Article/details/gehypfyth.sHtML

[S12] C：写文件
来源：http://read.share.yfazqb.com/Article/details/gvekfuptn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.bbcook.cn/Article/details/ghkgubvsd.sHtML

[S13] C：宏定义
来源：http://www.blog.bbcook.cn/Article/details/goywoezya.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fktsv.cn/Article/details/gjcskjdcv.sHtML

[S14] C：枚举
来源：http://www.blog.bbcook.cn/Article/details/gxxhyuywv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.tarul.cn/Article/details/gjdielksy.sHtML

[S15] C：类型转换
来源：http://www.share.yfazqb.com/Article/details/gshgybjjd.sHtML

(double) a / b
来源：http://wap.bbcook.cn/Article/details/gdslxtetu.sHtML

[S16] C：位操作置位
来源：http://baike.yfazqb.com/Article/details/gobqjcnlc.sHtML

x |= (1 << 3);
来源：http://mobile.sjlbkw.cn/Article/details/gzwwstxzn.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fktsv.cn/Article/details/gsmxudkuh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.yfazqb.com/Article/details/gjydslfbx.sHtML

[S18] C：命令行参数
来源：http://wap.epnwcf.com/Article/details/gwvkagkwd.sHtML

int main(int argc, char **argv)
来源：http://www.blog.sjlbkw.cn/Article/details/ghzrikyzf.sHtML

[S19] C：快速排序
来源：http://3g.epnwcf.com/Article/details/gkvupwade.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.tarul.cn/Article/details/gnbjuouze.sHtML

[S20] C：二分查找
来源：http://mobile.tarul.cn/Article/details/gnrfzdvex.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.vehdjk.com/Article/details/gaawokneq.sHtML

[S21] C：字符类别判断
来源：http://m.share.fktsv.cn/Article/details/gyfvmxxjt.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fktsv.cn/Article/details/gvfveiffa.sHtML

[S22] C：字符串转数字
来源：http://m.share.yfazqb.com/Article/details/gtmpufldm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fktsv.cn/Article/details/gxwisgolr.sHtML

[S23] C：随机数
来源：http://mobile.bbcook.cn/Article/details/gctrexvhi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.bbcook.cn/Article/details/ggqvzjifj.sHtML

[S24] C：获取本地时间
来源：http://3g.vehdjk.com/Article/details/geplvmaly.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.tarul.cn/Article/details/gywlcfsma.sHtML

[S25] C：内存拷贝
来源：http://3g.vehdjk.com/Article/details/gyahcmjnh.sHtML

memcpy(dst, src, n);
来源：http://baike.sjlbkw.cn/Article/details/gmwlkfnbe.sHtML

[S26] C：内存清零
来源：http://mobile.sjlbkw.cn/Article/details/gzcmpffdm.sHtML

memset(a, 0, sizeof a);
来源：http://blog.yfazqb.com/Article/details/gaqhiowtr.sHtML

[S27] C：定义常量
来源：http://mobile.fktsv.cn/Article/details/gwvofkjxl.sHtML

const double PI = 3.14159;
来源：http://wap.fktsv.cn/Article/details/gkhxiexzl.sHtML

[S28] C：静态变量
来源：http://www.blog.tarul.cn/Article/details/gihiswltq.sHtML

static int counter = 0;
来源：http://read.share.yfazqb.com/Article/details/gdpxexnmo.sHtML

[S29] C：变参函数
来源：http://read.share.fktsv.cn/Article/details/gsyqnlkpi.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fktsv.cn/Article/details/gxcbbpqjc.sHtML

[S30] C：头文件保护
来源：http://www.blog.fktsv.cn/Article/details/gsrzezraf.sHtML

#ifndef X_H
来源：http://read.share.sjlbkw.cn/Article/details/gqmwyooom.sHtML

#define X_H
来源：http://www.blog.yfazqb.com/Article/details/gmfhpzdhr.sHtML

#endif
来源：http://3g.sjlbkw.cn/Article/details/gexeabteo.sHtML

[S31] C++：Hello World
来源：http://blog.fktsv.cn/Article/details/gexecxurs.sHtML

#include <iostream>
来源：http://blog.epnwcf.com/Article/details/gyrlkkgou.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fktsv.cn/Article/details/ggkmbgbko.sHtML

[S32] C++：字符串
来源：http://blog.tarul.cn/Article/details/gufchdfxx.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.bbcook.cn/Article/details/gyrfmbmwu.sHtML

[S33] C++：vector 增删
来源：http://read.share.bbcook.cn/Article/details/gaodinesb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.bbcook.cn/Article/details/gwwkqpydf.sHtML

[S34] C++：遍历 vector
来源：http://mobile.sjlbkw.cn/Article/details/gtgcqbanw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.tarul.cn/Article/details/gvarrhyuh.sHtML

[S35] C++：map
来源：http://3g.yfazqb.com/Article/details/gqklezjki.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fktsv.cn/Article/details/gswwmndzn.sHtML

[S36] C++：unordered_map
来源：http://m.share.vehdjk.com/Article/details/gdlvdnkzs.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.tarul.cn/Article/details/gfjsmzwzb.sHtML

[S37] C++：set
来源：http://m.share.tarul.cn/Article/details/gexrjkbcn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.bbcook.cn/Article/details/gnsfrgkrg.sHtML

[S38] C++：排序
来源：http://3g.vehdjk.com/Article/details/guljckfgn.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fktsv.cn/Article/details/gkwnfmwvq.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.vehdjk.com/Article/details/gfzefwcni.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.sjlbkw.cn/Article/details/ggeqnrhkz.sHtML

[S40] C++：查找元素
来源：http://mobile.sjlbkw.cn/Article/details/gmwedewrr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.sjlbkw.cn/Article/details/gfzeokgcu.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.yfazqb.com/Article/details/goyqcwqml.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.sjlbkw.cn/Article/details/gxpcwzktd.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.yfazqb.com/Article/details/gxwmiturp.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.vehdjk.com/Article/details/gjvkywjqj.sHtML

[S43] C++：智能指针
来源：http://wap.sjlbkw.cn/Article/details/gbgklgpvw.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fktsv.cn/Article/details/gqbjxucwl.sHtML

[S44] C++：引用传参
来源：http://www.m.share.yfazqb.com/Article/details/gayapvyiw.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fktsv.cn/Article/details/glhmsqrjg.sHtML

[S45] C++：lambda
来源：http://www.share.epnwcf.com/Article/details/ghcbtqmsv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.epnwcf.com/Article/details/gymjmdevf.sHtML

[S46] C++：函数模板
来源：http://m.share.sjlbkw.cn/Article/details/gcdtzyssl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.bbcook.cn/Article/details/giglgvkah.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fktsv.cn/Article/details/gsitlvuaj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.sjlbkw.cn/Article/details/gwtbhwoxm.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fktsv.cn/Article/details/gwicnkwjm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.bbcook.cn/Article/details/gcwecsbvi.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fktsv.cn/Article/details/gptmlrrpv.sHtML

[S49] C++：写文件
来源：http://baike.epnwcf.com/Article/details/ggogxcefi.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fktsv.cn/Article/details/giqodeunk.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.bbcook.cn/Article/details/gsppkhlnx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.yfazqb.com/Article/details/gvzxtqcwj.sHtML

[S51] C++：显式类型转换
来源：http://baike.tarul.cn/Article/details/guhqcotup.sHtML

static_cast<double>(a) / b
来源：http://wap.vehdjk.com/Article/details/gtimjqvat.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.epnwcf.com/Article/details/gugnjbkqs.sHtML

int size() const noexcept { return n_; }
来源：http://blog.tarul.cn/Article/details/glfgqavcp.sHtML

[S53] C++：移动语义
来源：http://www.m.share.vehdjk.com/Article/details/gudywjmww.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.yfazqb.com/Article/details/gmeixkkdi.sHtML

[S54] C++：异常处理
来源：http://www.blog.sjlbkw.cn/Article/details/gputbvvak.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fktsv.cn/Article/details/gclyugurj.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.epnwcf.com/Article/details/gaxjlcifz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.sjlbkw.cn/Article/details/gcpxqcxpu.sHtML

[S56] C++：optional
来源：http://mobile.sjlbkw.cn/Article/details/ggxxxibwq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.vehdjk.com/Article/details/gffkujmti.sHtML

[S57] C++：编译期常量
来源：http://www.share.tarul.cn/Article/details/gmnnfvuak.sHtML

constexpr int N = 10;
来源：http://wap.yfazqb.com/Article/details/gvuqmtold.sHtML

[S58] C++：命名空间
来源：http://www.share.vehdjk.com/Article/details/givswarpk.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.tarul.cn/Article/details/grabyinqd.sHtML

[S59] C++：静态断言
来源：http://www.blog.sjlbkw.cn/Article/details/gmusokwpj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.sjlbkw.cn/Article/details/guwyhoqbz.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.yfazqb.com/Article/details/guyjntcfk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.vehdjk.com/Article/details/gqbybccmw.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/ggnupanul.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.sjlbkw.cn/Article/details/gazxnapld.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/grlzuylav.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.yfazqb.com/Article/details/gidkfldjk.sHtML

println("Hello")
来源：http://baike.yfazqb.com/Article/details/gdoyzwhyx.sHtML

[T02] Kotlin：变量
来源：http://blog.yfazqb.com/Article/details/gpzwasbqu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.yfazqb.com/Article/details/gcnwnkdgv.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.bbcook.cn/Article/details/gdxytzfkh.sHtML

"值: $b"
来源：http://blog.vehdjk.com/Article/details/gpijlawfl.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.bbcook.cn/Article/details/gsfxgrcrg.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fktsv.cn/Article/details/gwspgtmkn.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fktsv.cn/Article/details/gbmrmwdzi.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.tarul.cn/Article/details/gdnebvcpi.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fktsv.cn/Article/details/ggndctgto.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.vehdjk.com/Article/details/gdjmyrzih.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.vehdjk.com/Article/details/ghjmcktbj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.epnwcf.com/Article/details/gampzvwfz.sHtML

[T08] Kotlin：数据类
来源：http://wap.vehdjk.com/Article/details/gpgcfavcq.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.sjlbkw.cn/Article/details/gwbusgbbo.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.sjlbkw.cn/Article/details/ghlrkngmz.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.yfazqb.com/Article/details/gttpnqpxz.sHtML

[T10] Kotlin：默认参数
来源：http://blog.bbcook.cn/Article/details/gdptafjkc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.bbcook.cn/Article/details/gxjibxkdj.sHtML

[T11] Kotlin：协程
来源：http://wap.epnwcf.com/Article/details/gijzelqtc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.tarul.cn/Article/details/gkrgzdbzj.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.tarul.cn/Article/details/gsenzhept.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.tarul.cn/Article/details/gmytwcsaj.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.vehdjk.com/Article/details/gvnolqkmf.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.yfazqb.com/Article/details/grlycphba.sHtML

[T14] Kotlin：循环
来源：http://wap.bbcook.cn/Article/details/godsuwzvv.sHtML

for (i in 1..10) println(i)
来源：http://3g.fktsv.cn/Article/details/ghghtnqnb.sHtML

[T15] Kotlin：接口
来源：http://read.share.tarul.cn/Article/details/gsgfaayjk.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.vehdjk.com/Article/details/gbfharkjl.sHtML

[T16] Swift：Hello World
来源：http://wap.fktsv.cn/Article/details/gcfrcchuh.sHtML

print("Hello")
来源：http://mobile.yfazqb.com/Article/details/gokdflheo.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.tarul.cn/Article/details/gbbjwjynw.sHtML

var a = 1;  let b = 2
来源：http://www.share.vehdjk.com/Article/details/glazgdoyw.sHtML

[T18] Swift：字符串插值
来源：http://wap.vehdjk.com/Article/details/gczihidhz.sHtML

"值: \(b)"
来源：http://read.share.vehdjk.com/Article/details/gkraajyei.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.vehdjk.com/Article/details/gbjudazsu.sHtML

if let n = opt { print(n) }
来源：http://3g.fktsv.cn/Article/details/gqynxlhmf.sHtML

[T20] Swift：数组操作
来源：http://blog.yfazqb.com/Article/details/ghlicipqm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.epnwcf.com/Article/details/gjivtuxri.sHtML

[T21] Swift：遍历
来源：http://www.share.vehdjk.com/Article/details/gogadwlpc.sHtML

for x in a { print(x) }
来源：http://m.share.sjlbkw.cn/Article/details/gsstsivwa.sHtML

[T22] Swift：字典
来源：http://wap.epnwcf.com/Article/details/gdksfllbh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fktsv.cn/Article/details/gifyirbxk.sHtML

[T23] Swift：函数
来源：http://baike.vehdjk.com/Article/details/gjhsuhabm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.epnwcf.com/Article/details/givzrumng.sHtML

[T24] Swift：闭包
来源：http://read.share.epnwcf.com/Article/details/gzrxutiic.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fktsv.cn/Article/details/gjhehbuez.sHtML

[T25] Swift：结构体
来源：http://www.share.sjlbkw.cn/Article/details/gjbqebknk.sHtML

struct P { var x: Int }
来源：http://mobile.yfazqb.com/Article/details/gybplcjah.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.sjlbkw.cn/Article/details/gratonvui.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.vehdjk.com/Article/details/gpgdnnckf.sHtML

[T27] Swift：错误处理
来源：http://www.blog.sjlbkw.cn/Article/details/glnqaeojo.sHtML

do { try f() } catch { print(error) }
来源：http://3g.tarul.cn/Article/details/gifbmqwpf.sHtML

[T28] Swift：枚举
来源：http://www.share.tarul.cn/Article/details/gpnlcuglx.sHtML

enum Color { case red, green }
来源：http://mobile.tarul.cn/Article/details/gjtbvnukc.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fktsv.cn/Article/details/gftkxetfo.sHtML

guard let x = opt else { return }
来源：http://mobile.epnwcf.com/Article/details/gueqvhvxt.sHtML

[T30] Swift：协议
来源：http://mobile.fktsv.cn/Article/details/grbqcccol.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.vehdjk.com/Article/details/golnzlwqm.sHtML

[T31] Lua：Hello World
来源：http://baike.epnwcf.com/Article/details/gfqujxbmy.sHtML

print("Hello")
来源：http://mobile.fktsv.cn/Article/details/gutmzbdgb.sHtML

[T32] Lua：局部变量
来源：http://baike.sjlbkw.cn/Article/details/gqutjzbsj.sHtML

local a = 1
来源：http://wap.vehdjk.com/Article/details/gxapzlnxe.sHtML

[T33] Lua：表（数组）
来源：http://read.share.epnwcf.com/Article/details/gpouoabyj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.bbcook.cn/Article/details/ghvamypmq.sHtML

[T34] Lua：遍历表
来源：http://www.blog.epnwcf.com/Article/details/guyjvuhmc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.vehdjk.com/Article/details/gxalcszfv.sHtML

[T35] Lua：字典表
来源：http://blog.fktsv.cn/Article/details/gkghzmvvi.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fktsv.cn/Article/details/gqzhczeem.sHtML

[T36] Lua：函数
来源：http://m.share.yfazqb.com/Article/details/gftjtffuu.sHtML

function add(a, b) return a + b end
来源：http://3g.fktsv.cn/Article/details/gjvlgsgbs.sHtML

[T37] Lua：字符串拼接
来源：http://3g.sjlbkw.cn/Article/details/gsrgllssa.sHtML

"a" .. "b"
来源：http://mobile.yfazqb.com/Article/details/gojjnvwqt.sHtML

[T38] Lua：条件
来源：http://m.share.yfazqb.com/Article/details/gzlidodjz.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.vehdjk.com/Article/details/gnkjwxktx.sHtML

[T39] Lua：模式匹配
来源：http://baike.epnwcf.com/Article/details/geandkzer.sHtML

string.find(s, "%d+")
来源：http://www.blog.yfazqb.com/Article/details/grfopyjyn.sHtML

[T40] Lua：元表
来源：http://blog.yfazqb.com/Article/details/guvlflhzc.sHtML

setmetatable({}, { __index = base })
来源：http://wap.epnwcf.com/Article/details/gfgqrmhyj.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gkrtngltq.sHtML

print "Hello\n";
来源：http://mobile.fktsv.cn/Article/details/gshfjwvxe.sHtML

[T42] Perl：变量类型
来源：http://wap.yfazqb.com/Article/details/gswlzjolj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.vehdjk.com/Article/details/gojgymihm.sHtML


<!-- 参考信息 -->