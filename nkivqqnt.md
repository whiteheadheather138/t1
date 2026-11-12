代发 wailian999

files=$(ls -1)
来源：http://bvz.shanyushiyangtech.top

[R38] 管道串联
来源：http://fvm.52xcode.cn

cat a.txt | grep -i error | wc -l
来源：http://nhg.xylfe.cn

[R39] 重定向标准输出与错误
来源：http://raa.hnxiangtu.top

cmd > out.log 2>&1
来源：http://ocz.ivvv.top

[R40] 追加写日志
来源：http://scq.snrcjt.cn

echo "log" >> out.log
来源：http://lmm.yj20258888.top

[R41] 丢弃输出
来源：http://hcn.yj20258888.top

cmd >/dev/null 2>&1
来源：http://nxa.cucudq.cn

[R42] 输入重定向
来源：http://ejk.xziqi.cn

wc -l < a.txt
来源：http://mvp.cdnleiting.top

[R43] 按名字查找文件
来源：http://gmm.fanxiaobao.xyz

find . -name "*.log" -type f
来源：http://dlf.jqgfzy.top

[R44] 按修改时间查找
来源：http://kbq.pycfn.com

find . -mtime -7 -type f
来源：http://ksg.sweek.top

[R45] 批量删除
来源：http://aqn.epnwcf.com

find . -name "*.tmp" -delete
来源：http://bvk.hfpthk.cn

[R46] 递归替换文件内容
来源：http://quc.hnqzz.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nau.ppjwa.cn

[R47] sed 单行替换
来源：http://dpt.nwbrower.top

sed -i 's/foo/bar/g' a.txt
来源：http://gzn.jiagoushi.top

[R48] awk 取指定列
来源：http://hbx.jqgfzy.top

awk '{print $1, $3}' a.txt
来源：http://ieg.fzhhl.top

[R49] awk 带条件
来源：http://ieb.shanyushiyangkeji.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lct.feifeiyinyue.top

[R50] awk 求和
来源：http://egy.hongshengwenyu.top

awk '{s += $2} END {print s}' a.txt
来源：http://bgz.chenzaomai.com

[R51] 排序去重取前几
来源：http://kwp.jinqigufen.top

sort a.txt | uniq -c | sort -rn | head
来源：http://twd.jqgufenzy.top

[R52] 统计行数
来源：http://lsx.bjfxy.top

wc -l a.txt
来源：http://gtq.xingfuxueyuan.xyz

[R53] 查看文件头与实时尾
来源：http://btq.hesvh.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rkq.guowangkeji.top

[R54] 比较两个文件
来源：http://wsp.dianchejie.cn

diff a.txt b.txt
来源：http://hnc.jinqigfzy.top

[R55] 压缩与解压
来源：http://ypn.dashuyun.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wno.jinyuanbaomall.cn

[R56] 远程拷贝
来源：http://kag.shangyingyoupin.top

scp file user@host:/path/
来源：http://cih.chenjidiqi.icu

[R57] 远程执行命令
来源：http://cgf.cashguo.top

ssh user@host 'uptime'
来源：http://wvg.yuanzhike.top

[R58] 下载文件
来源：http://fag.xingfuxueyuan.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ewj.jlsjyb.cn

[R59] 发 POST JSON
来源：http://rny.vqdsnc.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rdf.ywan-chungtsiang.top

[R60] 只看 HTTP 状态码
来源：http://uqe.daria6918.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://foc.yj20258.top

[R61] 磁盘占用
来源：http://crs.uphjek.com

df -h;  du -sh *
来源：http://dqa.gogol.net.cn

[R62] 找最占空间的文件
来源：http://usj.sweek.top

du -ah . | sort -rh | head -10
来源：http://ydo.hesvh.cn

[R63] 内存与进程
来源：http://mnm.cucudq.cn

free -h;  ps aux | grep nginx
来源：http://kfw.yueranfly.top

[R64] 结束进程
来源：http://jdh.nanxuanxn.top

kill -9 $(pgrep -f app.py)
来源：http://nmx.jlsjyb.cn

[R65] 查看端口占用
来源：http://bjs.jinqigufen.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pak.ehwqpu.com

[R66] 定时任务
来源：http://dtw.nanxinkj.top

crontab -e;  crontab -l
来源：http://lwc.gotoacloud.top

[R67] 生成随机十六进制串
来源：http://klo.svipenyu.cn

openssl rand -hex 16
来源：http://ryc.yj20258888.top

[R68] 计算文件校验值
来源：http://qod.xylfe.cn

sha256sum a.txt;  md5sum a.txt
来源：http://qfq.chenlongwang.top

[R69] 生成随机密码
来源：http://dpy.yangfankeji.com

head -c 16 /dev/urandom | base64
来源：http://ohi.jlsjyb.cn

[R70] 时间戳与互转
来源：http://cle.hesvh.cn

date +%s;  date -d @1700000000
来源：http://soc.haohaochexian.top

[R71] 日期格式化
来源：http://siv.yj20258.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ikb.hongshengwenyu.top

[R72] 等待端口就绪
来源：http://yqi.havefunace.top

until nc -z localhost 3306; do sleep 1; done
来源：http://yfb.bjfxy.top

[R73] 分割大日志
来源：http://yli.vqdsnc.cn

split -l 1000 big.log part_
来源：http://igs.zhengqikj.top

[R74] 批量重命名
来源：http://sbb.xylfe.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gam.zdqjudy.top

[R75] 导出环境变量
来源：http://kww.iojbl.cn

export PATH="$HOME/bin:$PATH"
来源：http://kja.shanyushiyangtech.top

[R76] 使用临时文件
来源：http://qnf.gogol.net.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hiy.jlsjyb.cn

[R77] 读取用户输入
来源：http://ass.guowangkeji.top

read -rp "请输入: " ans
来源：http://cdy.yj20258.top

[R78] 交互式菜单
来源：http://lhp.epnwcf.com

select opt in a b c; do echo "$opt"; break; done
来源：http://cvb.zdbjq.cn

[R79] 解析命令行选项
来源：http://lno.hysaishi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pwv.svipenyu.cn

[R80] 查看脚本执行耗时
来源：http://wrz.zhengqikj.top

time ./run.sh
来源：http://hgk.epnwcf.com

================================================================================
来源：http://pgb.jinyuanbaomall.cn

S. C / C++ 专题
来源：http://bxr.hnqzz.top

================================================================================
来源：http://cjy.redwolf501.top

[S01] C：Hello World
来源：http://eyp.vehdjk.com

#include <stdio.h>
来源：http://ork.jinghuilouyu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://iek.jinghuilouyu.cn

[S02] C：变量与格式化输出
来源：http://cjt.fengsongda.top

int a = 10; printf("%d\n", a);
来源：http://ngw.jinyuanbaomall.cn

[S03] C：读入整数
来源：http://giz.smart0.xyz

int x; scanf("%d", &x);
来源：http://syk.9152youxi.cn

[S04] C：字符串复制
来源：http://phl.cqqwz.cn

char dst[32]; strcpy(dst, "hi");
来源：http://bvq.vehdjk.com

[S05] C：字符串长度
来源：http://etl.bjfxy.top

strlen(s)
来源：http://xua.hysaishi.cn

[S06] C：字符串比较
来源：http://dpw.tanke756.top

strcmp(a, b) == 0
来源：http://jff.jqgfzy.top

[S07] C：数组遍历求和
来源：http://zhx.zhixingplan.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kwz.smart0.xyz

[S08] C：动态内存分配与释放
来源：http://ktn.ivvv.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hdx.yfazqb.com

[S09] C：结构体定义与初始化
来源：http://rks.svipenyu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dvf.fanxiaobao.xyz

[S10] C：指针与解引用
来源：http://qxt.yangfankeji.com

int *p = &a;  *p = 5;
来源：http://nqd.yonumen.top

[S11] C：逐行读文件
来源：http://ejs.hywenlv.cn

FILE *f = fopen("a.txt", "r");
来源：http://qit.cucudq.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://wwg.cheryme.top

fclose(f);
来源：http://vtf.yj202588.top

[S12] C：写文件
来源：http://tqe.bjfxy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tny.chenjidiqi.icu

[S13] C：宏定义
来源：http://aak.tian-w.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fjs.sjlbkw.cn

[S14] C：枚举
来源：http://ukl.gogol.net.cn

enum Color { RED, GREEN, BLUE };
来源：http://wzy.smart0.xyz

[S15] C：类型转换
来源：http://mdb.yuanzhike.top

(double) a / b
来源：http://ybq.zycfv.cn

[S16] C：位操作置位
来源：http://tjm.hongshengwenyu.top

x |= (1 << 3);
来源：http://owq.hammf.cn

[S17] C：安全拼接字符串
来源：http://lfp.hywenlv.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wtm.jianghu66.top

[S18] C：命令行参数
来源：http://pim.zhoulong.xyz

int main(int argc, char **argv)
来源：http://cni.uphjek.com

[S19] C：快速排序
来源：http://xtu.gzhubu.top

qsort(a, n, sizeof(int), cmp);
来源：http://eyt.fengsongda.top

[S20] C：二分查找
来源：http://taw.quarkkingdee.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hbw.52xcode.cn

[S21] C：字符类别判断
来源：http://uzk.52xcode.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://omk.tianlin.xyz

[S22] C：字符串转数字
来源：http://far.jyoumei.cn

atoi("42");  strtod("3.14", NULL);
来源：http://kts.tarul.cn

[S23] C：随机数
来源：http://vlk.cashguo.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ksx.birdmap.top

[S24] C：获取本地时间
来源：http://zoy.tarul.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hgd.yvedp.cn

[S25] C：内存拷贝
来源：http://mat.yueranfly.top

memcpy(dst, src, n);
来源：http://osg.mhx1999.top

[S26] C：内存清零
来源：http://brd.dashuyun.cn

memset(a, 0, sizeof a);
来源：http://rvz.fengsongda.top

[S27] C：定义常量
来源：http://mam.nwbrower.top

const double PI = 3.14159;
来源：http://mic.shzxlz.cn

[S28] C：静态变量
来源：http://rrw.zhoulong.xyz

static int counter = 0;
来源：http://fxt.nwbrower.top

[S29] C：变参函数
来源：http://vbe.ivvv.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://flx.jinyuanbaomall.cn

[S30] C：头文件保护
来源：http://kfl.snrcjt.cn

#ifndef X_H
来源：http://jhl.ydjk.org.cn

#define X_H
来源：http://sbl.zhoulong.xyz

#endif
来源：http://uzb.ppjwa.cn

[S31] C++：Hello World
来源：http://nbk.tianlin.xyz

#include <iostream>
来源：http://svs.zhijiandao.cn

int main() { std::cout << "Hello\n"; }
来源：http://hkp.hcnkem.com

[S32] C++：字符串
来源：http://bfs.sjlbkw.cn

std::string s = "hi";  s += "!";
来源：http://ryw.jqgfzy.top

[S33] C++：vector 增删
来源：http://izf.jinghuilouyu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wgr.yonumen.top

[S34] C++：遍历 vector
来源：http://uii.yj20258888.top

for (auto &x : v) { std::cout << x; }
来源：http://wvu.9152youxi.cn

[S35] C++：map
来源：http://pyh.chenjidiqi.icu

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bsl.jinyuanbaomall.cn

[S36] C++：unordered_map
来源：http://vnf.quarkkingdee.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lmm.cucudq.cn

[S37] C++：set
来源：http://cfz.vqdsnc.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xif.cashguo.top

[S38] C++：排序
来源：http://qsf.jlsjyb.cn

std::sort(v.begin(), v.end());
来源：http://ahw.yangfankeji.com

[S39] C++：自定义比较器排序
来源：http://cmj.gogol.net.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zpm.zhaomingkeji.xyz

[S40] C++：查找元素
来源：http://uot.yj202588.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rla.chenlongwang.top

[S41] C++：类与构造函数
来源：http://der.snrcjt.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://frh.nwbrower.top

[S42] C++：继承与虚函数
来源：http://dvz.hesvh.cn

class B : public Base { public: void f() override {} };
来源：http://bso.birdmap.top

[S43] C++：智能指针
来源：http://dwn.pycfn.com

auto p = std::make_unique<int>(5);
来源：http://yuk.fengsongda.top

[S44] C++：引用传参
来源：http://xbf.cheryme.top

void inc(int &x) { ++x; }
来源：http://tum.havefunace.top

[S45] C++：lambda
来源：http://uoa.vqdsnc.cn

auto add = [](int a, int b) { return a + b; };
来源：http://jxk.jinqigufen.top

[S46] C++：函数模板
来源：http://idu.wangshuangyany.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dvi.tarul.cn

[S47] C++：结构化绑定遍历
来源：http://nxv.smart0.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nqq.tian-w.cn

[S48] C++：逐行读文件
来源：http://wlk.jqgufenzy.top

std::ifstream in("a.txt");  std::string line;
来源：http://wlf.9152youxi.cn

while (std::getline(in, line)) { }
来源：http://ctw.9152youxi.cn

[S49] C++：写文件
来源：http://lfo.hesvh.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://guu.zycfv.cn

[S50] C++：格式化数字
来源：http://eah.cheryme.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hdh.gzhubu.top

[S51] C++：显式类型转换
来源：http://bke.andypj.xyz

static_cast<double>(a) / b
来源：http://oyg.chenjidiqi.icu

[S52] C++：const 与 noexcept
来源：http://jcw.jianghu66.top

int size() const noexcept { return n_; }
来源：http://ztp.zhaomingkeji.xyz

[S53] C++：移动语义
来源：http://ugx.xingfuxueyuan.xyz

std::vector<int> w = std::move(v);
来源：http://thv.gogol.net.cn

[S54] C++：异常处理
来源：http://jkk.shangyingyoupin.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mqj.sjlbkw.cn

[S55] C++：结构化绑定
来源：http://sjp.yonumen.top

auto [a, b] = std::make_pair(1, 2);
来源：http://rvs.guannengcc.top

[S56] C++：optional
来源：http://ahx.52xcode.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wra.kuanghao11.cn

[S57] C++：编译期常量
来源：http://ksm.feifeiyinyue.top

constexpr int N = 10;
来源：http://kjy.yangfankeji.com

[S58] C++：命名空间
来源：http://mni.fktsv.cn

namespace ns { int f() { return 1; } }
来源：http://kcu.nwbrower.top

[S59] C++：静态断言
来源：http://xgx.pycfn.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jhq.cqqwz.cn

[S60] C++：遍历并删除元素
来源：http://afa.sxryk.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://exs.jinqigfzy.top

================================================================================
来源：http://qbe.ydzc1.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fom.nanxinkj.top

================================================================================
来源：http://dhz.gzhubu.top

[T01] Kotlin：Hello World
来源：http://oiq.svipenyu.cn

println("Hello")
来源：http://cqf.svipenyu.cn

[T02] Kotlin：变量
来源：http://rgc.52xcode.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cxo.jlsjyb.cn

[T03] Kotlin：字符串模板
来源：http://jou.zhengqikj.top

"值: $b"
来源：http://mzm.zhixingplan.top

[T04] Kotlin：空安全
来源：http://vqk.guowangkeji.top

val n: String? = null;  n?.length
来源：http://kgm.daxiang520.top

[T05] Kotlin：when 表达式
来源：http://xvs.iojbl.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xpi.yvedp.cn

[T06] Kotlin：集合映射
来源：http://fpj.xuanzx.com

listOf(1, 2, 3).map { it * 2 }
来源：http://xut.hysaishi.cn

[T07] Kotlin：集合过滤
来源：http://coe.jinqigufen.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://thx.hywenlv.cn

[T08] Kotlin：数据类
来源：http://dvz.yj20258.top

data class User(val name: String, val age: Int)
来源：http://xma.guannengcc.top

[T09] Kotlin：扩展函数
来源：http://imu.fktsv.cn

fun String.exclaim() = this + "!"
来源：http://alq.jinqigufen.top

[T10] Kotlin：默认参数
来源：http://whb.jlsjyb.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://xni.hnxiangtu.top

[T11] Kotlin：协程
来源：http://jbs.vqdsnc.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://nth.guowangkeji.top

[T12] Kotlin：解构声明
来源：http://ybi.nanxinkj.top

val (a, b) = Pair(1, 2)
来源：http://vsx.fehbvm.com

[T13] Kotlin：只读 Map
来源：http://jcc.zhiwuduotai.top

val m = mapOf("a" to 1)
来源：http://yde.shangyingyoupin.top

[T14] Kotlin：循环
来源：http://gxr.zhengqikj.top

for (i in 1..10) println(i)
来源：http://nbk.yj20258.top

[T15] Kotlin：接口
来源：http://qzy.shuidangran.top

interface Shape { fun area(): Double }
来源：http://cdi.dianchejie.cn

[T16] Swift：Hello World
来源：http://eda.zdqjudy.top

print("Hello")
来源：http://ntu.sjlbkw.cn

[T17] Swift：变量与常量
来源：http://ksx.ppjwa.cn

var a = 1;  let b = 2
来源：http://uah.yangfankeji.com

[T18] Swift：字符串插值
来源：http://bud.jlsjyb.cn

"值: \(b)"
来源：http://gvo.sjlbkw.cn

[T19] Swift：可选绑定
来源：http://ajt.jyoumei.cn

if let n = opt { print(n) }
来源：http://wtx.jlsjyb.cn

[T20] Swift：数组操作
来源：http://yet.316326.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://mln.sweek.top

[T21] Swift：遍历
来源：http://xui.xingfuxueyuan.xyz

for x in a { print(x) }
来源：http://pzz.jlsjyb.cn

[T22] Swift：字典
来源：http://ywk.bjfxy.top

var d = ["a": 1];  d["b"] = 2
来源：http://ocz.zhongyouzk.top

[T23] Swift：函数
来源：http://eod.feifeiyinyue.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ndc.hcnkem.com

[T24] Swift：闭包
来源：http://zsw.smart0.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://wgk.nwbrower.top

[T25] Swift：结构体
来源：http://dtd.wangshuangyany.cn

struct P { var x: Int }
来源：http://slu.jinghuilouyu.cn

[T26] Swift：类与重写
来源：http://hsc.shuidangran.top

class A: Base { override func f() {} }
来源：http://zim.jinqigufen.top

[T27] Swift：错误处理
来源：http://hfh.meibo888.top

do { try f() } catch { print(error) }
来源：http://mlu.gzhubu.top

[T28] Swift：枚举
来源：http://ndd.sysykeji.top

enum Color { case red, green }
来源：http://orc.hongshengwenyu.top

[T29] Swift：guard 提前返回
来源：http://iry.tianlin.xyz

guard let x = opt else { return }
来源：http://pcw.fehbvm.com

[T30] Swift：协议
来源：http://ppl.ybcxt.top

protocol Shape { func area() -> Double }
来源：http://fpf.nanxinkj.top

[T31] Lua：Hello World
来源：http://lxg.zycfv.cn

print("Hello")
来源：http://zcd.fzhhl.top

[T32] Lua：局部变量
来源：http://zfm.zhixingplan.top

local a = 1
来源：http://pur.cqqwz.cn

[T33] Lua：表（数组）
来源：http://flo.jianghu66.top

local t = {1, 2, 3};  t[4] = 4
来源：http://fjx.cqqwz.cn

[T34] Lua：遍历表
来源：http://aih.9152youxi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://wff.nwbrower.top

[T35] Lua：字典表
来源：http://fao.ehwqpu.com

local d = { a = 1 };  d.b = 2
来源：http://aen.yj20258888.top

[T36] Lua：函数
来源：http://atr.ivvv.top

function add(a, b) return a + b end
来源：http://lvo.zhixingplan.top

[T37] Lua：字符串拼接
来源：http://dnz.aibaodan.cn

"a" .. "b"
来源：http://vdv.cucudq.cn

[T38] Lua：条件
来源：http://jpx.jianghu66.top

if x > 0 then print("正") end
来源：http://ieh.havefunace.top

[T39] Lua：模式匹配
来源：http://cis.yfazqb.com

string.find(s, "%d+")
来源：http://drn.sufxvd.cn

[T40] Lua：元表
来源：http://zpj.shanyushiyangtech.top

setmetatable({}, { __index = base })
来源：http://kpd.xziqi.cn


<!-- 参考信息 -->