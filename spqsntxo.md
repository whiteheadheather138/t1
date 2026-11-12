代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kui.chenlongwang.top

[R80] 查看脚本执行耗时
来源：http://oox.gaohongyu789.top

time ./run.sh
来源：http://cek.quarkkingdee.top

================================================================================
来源：http://vim.fanxiaobao.xyz

S. C / C++ 专题
来源：http://vul.hammf.cn

================================================================================
来源：http://uxd.dashuyun.cn

[S01] C：Hello World
来源：http://pui.zhongyouzk.top

#include <stdio.h>
来源：http://nqu.hfpthk.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://cbo.chenzaomai.com

[S02] C：变量与格式化输出
来源：http://alx.yj20258.top

int a = 10; printf("%d\n", a);
来源：http://eqf.52xcode.cn

[S03] C：读入整数
来源：http://pwx.yangfankeji.com

int x; scanf("%d", &x);
来源：http://jed.snrcjt.cn

[S04] C：字符串复制
来源：http://ktw.c1oappe.top

char dst[32]; strcpy(dst, "hi");
来源：http://qer.shangyingyoupin.top

[S05] C：字符串长度
来源：http://uah.chenlongwang.top

strlen(s)
来源：http://knf.yfazqb.com

[S06] C：字符串比较
来源：http://ibo.snrcjt.cn

strcmp(a, b) == 0
来源：http://vqb.bjfxy.top

[S07] C：数组遍历求和
来源：http://ctk.quarkkingdee.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mkm.fengsongda.top

[S08] C：动态内存分配与释放
来源：http://blb.jinqigfzy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://oel.mhx1999.top

[S09] C：结构体定义与初始化
来源：http://jve.hongshengwenyu.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fvo.sjlbkw.cn

[S10] C：指针与解引用
来源：http://stt.mhx1999.top

int *p = &a;  *p = 5;
来源：http://yvr.zycfv.cn

[S11] C：逐行读文件
来源：http://eyv.chenlongwang.top

FILE *f = fopen("a.txt", "r");
来源：http://eol.ivvv.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://yvx.zhoulong.xyz

fclose(f);
来源：http://ram.fzhhl.top

[S12] C：写文件
来源：http://rgk.bjfxy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fdg.nanxuanxn.top

[S13] C：宏定义
来源：http://dmz.birdmap.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wco.zhijiandao.cn

[S14] C：枚举
来源：http://iqk.jqgufenzy.top

enum Color { RED, GREEN, BLUE };
来源：http://rim.shzxlz.cn

[S15] C：类型转换
来源：http://djp.jiagoushi.top

(double) a / b
来源：http://jtr.hnxiangtu.top

[S16] C：位操作置位
来源：http://hmr.yj20258.top

x |= (1 << 3);
来源：http://lbs.yj20258888.top

[S17] C：安全拼接字符串
来源：http://dnz.cqqwz.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kyl.zhijiandao.cn

[S18] C：命令行参数
来源：http://hxn.yfazqb.com

int main(int argc, char **argv)
来源：http://qrn.feifeiyinyue.top

[S19] C：快速排序
来源：http://gmc.jinqigfzy.top

qsort(a, n, sizeof(int), cmp);
来源：http://yry.wangshuangyany.cn

[S20] C：二分查找
来源：http://gwo.sufxvd.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bdw.daxiang520.top

[S21] C：字符类别判断
来源：http://rkm.nanxuanxn.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ifl.shangyingyoupin.top

[S22] C：字符串转数字
来源：http://tgr.tarul.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ivu.ywan-chungtsiang.top

[S23] C：随机数
来源：http://pga.shanyushiyangtech.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ihi.yueranfly.top

[S24] C：获取本地时间
来源：http://uju.shanyushiyangkeji.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://biw.svipenyu.cn

[S25] C：内存拷贝
来源：http://gfj.52xcode.cn

memcpy(dst, src, n);
来源：http://xgn.hnxiangtu.top

[S26] C：内存清零
来源：http://hwg.yj20258888.top

memset(a, 0, sizeof a);
来源：http://ulb.quarkkingdee.top

[S27] C：定义常量
来源：http://ssi.yfazqb.com

const double PI = 3.14159;
来源：http://khz.birdmap.top

[S28] C：静态变量
来源：http://hti.sysykeji.top

static int counter = 0;
来源：http://ifv.zdqjudy.top

[S29] C：变参函数
来源：http://ukh.birdmap.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://upi.zhongyouzk.top

[S30] C：头文件保护
来源：http://wlo.uphjek.com

#ifndef X_H
来源：http://mpq.gzhubu.top

#define X_H
来源：http://fqi.yueranfly.top

#endif
来源：http://qop.tanke756.top

[S31] C++：Hello World
来源：http://ovl.yfazqb.com

#include <iostream>
来源：http://hij.chenjidiqi.icu

int main() { std::cout << "Hello\n"; }
来源：http://ujo.zhoulong.xyz

[S32] C++：字符串
来源：http://vbj.aibaodan.cn

std::string s = "hi";  s += "!";
来源：http://zoq.jinghuilouyu.cn

[S33] C++：vector 增删
来源：http://zmm.daria6918.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gqy.zhongyouzk.top

[S34] C++：遍历 vector
来源：http://kyn.shzxlz.cn

for (auto &x : v) { std::cout << x; }
来源：http://fql.zhixingplan.top

[S35] C++：map
来源：http://aaj.tian-w.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nps.52xcode.cn

[S36] C++：unordered_map
来源：http://lsq.hesvh.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rkq.chenzaomai.com

[S37] C++：set
来源：http://tam.sjlbkw.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://eqp.havefunace.top

[S38] C++：排序
来源：http://lqq.shzxlz.cn

std::sort(v.begin(), v.end());
来源：http://pol.gaohongyu789.top

[S39] C++：自定义比较器排序
来源：http://nsc.jinyuanbaomall.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vdf.guowangkeji.top

[S40] C++：查找元素
来源：http://ltg.svipenyu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yim.haohaochexian.top

[S41] C++：类与构造函数
来源：http://ylx.yj202588.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vpa.xinyue.icu

[S42] C++：继承与虚函数
来源：http://yho.hysaishi.cn

class B : public Base { public: void f() override {} };
来源：http://mbk.snrcjt.cn

[S43] C++：智能指针
来源：http://cam.feifeiyinyue.top

auto p = std::make_unique<int>(5);
来源：http://xfa.hammf.cn

[S44] C++：引用传参
来源：http://dla.zhixingplan.top

void inc(int &x) { ++x; }
来源：http://mri.ydjk.org.cn

[S45] C++：lambda
来源：http://dth.xziqi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://kop.yuanzhike.top

[S46] C++：函数模板
来源：http://dxf.dianchejie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bml.quarkkingdee.top

[S47] C++：结构化绑定遍历
来源：http://thg.sweek.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ans.haohaochexian.top

[S48] C++：逐行读文件
来源：http://fgb.pycfn.com

std::ifstream in("a.txt");  std::string line;
来源：http://ooz.fzhhl.top

while (std::getline(in, line)) { }
来源：http://rsw.shanyushiyangkeji.top

[S49] C++：写文件
来源：http://geq.yuanzhike.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xrl.shanyushiyangkeji.top

[S50] C++：格式化数字
来源：http://imi.zycfv.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://idu.shzxlz.cn

[S51] C++：显式类型转换
来源：http://zdq.0kj1m.cn

static_cast<double>(a) / b
来源：http://ica.hammf.cn

[S52] C++：const 与 noexcept
来源：http://hud.xylfe.cn

int size() const noexcept { return n_; }
来源：http://aai.smart0.xyz

[S53] C++：移动语义
来源：http://qgx.hongshengwenyu.top

std::vector<int> w = std::move(v);
来源：http://ilr.uphjek.com

[S54] C++：异常处理
来源：http://rpq.fehbvm.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://geq.xuetiantiany.cn

[S55] C++：结构化绑定
来源：http://acs.jianghu66.top

auto [a, b] = std::make_pair(1, 2);
来源：http://rlh.ctjpmb.com

[S56] C++：optional
来源：http://ypt.yfazqb.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rqx.pycfn.com

[S57] C++：编译期常量
来源：http://jbu.nanxinkj.top

constexpr int N = 10;
来源：http://qko.jinghuilouyu.cn

[S58] C++：命名空间
来源：http://hye.iojbl.cn

namespace ns { int f() { return 1; } }
来源：http://pwn.guowangkeji.top

[S59] C++：静态断言
来源：http://fpk.yonumen.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://iod.yj20258888.top

[S60] C++：遍历并删除元素
来源：http://beq.hammf.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://viu.jinqigfzy.top

================================================================================
来源：http://kfv.havefunace.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://shl.aibaodan.cn

================================================================================
来源：http://jhw.hnqzz.top

[T01] Kotlin：Hello World
来源：http://ntx.yvedp.cn

println("Hello")
来源：http://tvt.hammf.cn

[T02] Kotlin：变量
来源：http://ast.cashguo.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://opg.jinyuanbaomall.cn

[T03] Kotlin：字符串模板
来源：http://dvo.svipenyu.cn

"值: $b"
来源：http://vql.zhongyouzk.top

[T04] Kotlin：空安全
来源：http://gqz.fengsongda.top

val n: String? = null;  n?.length
来源：http://tzo.hfpthk.cn

[T05] Kotlin：when 表达式
来源：http://ouz.jinqigufen.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qiz.zhengqikj.top

[T06] Kotlin：集合映射
来源：http://djv.sufxvd.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://qbw.nanxuanxn.top

[T07] Kotlin：集合过滤
来源：http://vjf.guowangkeji.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://kqe.yvedp.cn

[T08] Kotlin：数据类
来源：http://fhh.yj20258888.top

data class User(val name: String, val age: Int)
来源：http://gbh.zhengqikj.top

[T09] Kotlin：扩展函数
来源：http://ceu.bjfxy.top

fun String.exclaim() = this + "!"
来源：http://ozk.chenjidiqi.icu

[T10] Kotlin：默认参数
来源：http://oun.yvedp.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jig.tanke756.top

[T11] Kotlin：协程
来源：http://ify.svipenyu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qfa.hnxiangtu.top

[T12] Kotlin：解构声明
来源：http://yoi.cqqwz.cn

val (a, b) = Pair(1, 2)
来源：http://cby.wangdashe.top

[T13] Kotlin：只读 Map
来源：http://cuk.fktsv.cn

val m = mapOf("a" to 1)
来源：http://qwt.vehdjk.com

[T14] Kotlin：循环
来源：http://iih.cdnleiting.top

for (i in 1..10) println(i)
来源：http://dea.chenzaomai.com

[T15] Kotlin：接口
来源：http://zfu.vehdjk.com

interface Shape { fun area(): Double }
来源：http://ykx.iojbl.cn

[T16] Swift：Hello World
来源：http://iou.wangdashe.top

print("Hello")
来源：http://vvy.gzhubu.top

[T17] Swift：变量与常量
来源：http://fri.ydzc1.top

var a = 1;  let b = 2
来源：http://uhe.aibaodan.cn

[T18] Swift：字符串插值
来源：http://vzm.tanke756.top

"值: \(b)"
来源：http://hsj.yongpay.top

[T19] Swift：可选绑定
来源：http://wix.ivvv.top

if let n = opt { print(n) }
来源：http://toe.zhijiandao.cn

[T20] Swift：数组操作
来源：http://itr.ppjwa.cn

var a = [1, 2, 3];  a.append(4)
来源：http://fpc.cdnleiting.top

[T21] Swift：遍历
来源：http://rtu.hammf.cn

for x in a { print(x) }
来源：http://kdv.dianchejie.cn

[T22] Swift：字典
来源：http://evt.uphjek.com

var d = ["a": 1];  d["b"] = 2
来源：http://vht.xingfuxueyuan.xyz

[T23] Swift：函数
来源：http://wcz.ywan-chungtsiang.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hjv.sysykeji.top

[T24] Swift：闭包
来源：http://mtw.mhx1999.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://wrq.xuanzx.com

[T25] Swift：结构体
来源：http://icn.hnqzz.top

struct P { var x: Int }
来源：http://hbf.hammf.cn

[T26] Swift：类与重写
来源：http://xkt.guowangkeji.top

class A: Base { override func f() {} }
来源：http://yrw.316326.xyz

[T27] Swift：错误处理
来源：http://dpd.chenlongwang.top

do { try f() } catch { print(error) }
来源：http://kze.pycfn.com

[T28] Swift：枚举
来源：http://qbz.pycfn.com

enum Color { case red, green }
来源：http://ljj.hesvh.cn

[T29] Swift：guard 提前返回
来源：http://hrr.hnqzz.top

guard let x = opt else { return }
来源：http://wlt.birdmap.top

[T30] Swift：协议
来源：http://wxd.redwolf501.top

protocol Shape { func area() -> Double }
来源：http://xrw.ywan-chungtsiang.top

[T31] Lua：Hello World
来源：http://oso.redwolf501.top

print("Hello")
来源：http://djf.hongshengwenyu.top

[T32] Lua：局部变量
来源：http://yas.jlsjyb.cn

local a = 1
来源：http://hxq.aibaodan.cn

[T33] Lua：表（数组）
来源：http://ayj.vqdsnc.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://bhr.nanxinkj.top

[T34] Lua：遍历表
来源：http://ugi.tarul.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://lno.hongshengwenyu.top

[T35] Lua：字典表
来源：http://kym.bjfxy.top

local d = { a = 1 };  d.b = 2
来源：http://nvz.yj202588.top

[T36] Lua：函数
来源：http://wlc.sysykeji.top

function add(a, b) return a + b end
来源：http://yzd.cashguo.top

[T37] Lua：字符串拼接
来源：http://uxg.jinqigufen.top

"a" .. "b"
来源：http://pqp.shangyingyoupin.top

[T38] Lua：条件
来源：http://emy.ywan-chungtsiang.top

if x > 0 then print("正") end
来源：http://qhh.9152youxi.cn

[T39] Lua：模式匹配
来源：http://wpe.gotoacloud.top

string.find(s, "%d+")
来源：http://xct.chenzaomai.com

[T40] Lua：元表
来源：http://oyv.pycfn.com

setmetatable({}, { __index = base })
来源：http://mej.ywan-chungtsiang.top

[T41] Perl：Hello World
来源：http://cpw.yongpay.top

print "Hello\n";
来源：http://sxc.xziqi.cn

[T42] Perl：变量类型
来源：http://mvq.jinqigfzy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://osm.shuidangran.top

[T43] Perl：字符串插值
来源：http://gvm.dashuyun.cn

"值: $a"
来源：http://wrb.kuanghao11.cn

[T44] Perl：条件
来源：http://fcm.9152youxi.cn

if ($a > 0) { print "正"; }
来源：http://fqi.vehdjk.com

[T45] Perl：数组遍历
来源：http://vnr.mhx1999.top

for my $x (@arr) { print $x; }
来源：http://rfc.redwolf501.top

[T46] Perl：哈希操作
来源：http://nyy.uphjek.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://uup.yuanzhike.top

[T47] Perl：正则捕获
来源：http://ikx.zhiwuduotai.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ijy.andypj.xyz

[T48] Perl：正则替换
来源：http://ymm.cashguo.top

$s =~ s/old/new/g;
来源：http://wyj.jqgfzy.top

[T49] Perl：函数
来源：http://tfa.c1oappe.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gfz.jqgufenzy.top

[T50] Perl：逐行读文件
来源：http://hol.jyoumei.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://nrp.gzhubu.top

while (my $line = <$fh>) { print $line; }
来源：http://ien.epnwcf.com

[T51] Scala：Hello World
来源：http://sgh.cdnleiting.top

println("Hello")
来源：http://qar.yonumen.top

[T52] Scala：变量
来源：http://hmq.zhixingplan.top

val a = 1;  var b = 2
来源：http://hqm.shuidangran.top

[T53] Scala：字符串插值
来源：http://lnl.shuidangran.top

s"值: $b"
来源：http://bhd.tianlin.xyz

[T54] Scala：集合映射
来源：http://aly.wangdashe.top

List(1, 2, 3).map(_ * 2)
来源：http://kuu.shzxlz.cn

[T55] Scala：集合过滤
来源：http://fis.jinyuanbaomall.cn

List(1, 2, 3).filter(_ > 1)
来源：http://lkv.gogol.net.cn

[T56] Scala：样例类
来源：http://zvz.ivvv.top

case class User(name: String, age: Int)
来源：http://hmi.dashuyun.cn

[T57] Scala：模式匹配
来源：http://qdq.aibaodan.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ejm.yuxming.cn

[T58] Scala：函数定义
来源：http://zpw.bjfxy.top

def add(a: Int, b: Int): Int = a + b
来源：http://tkt.yuanzhike.top

[T59] Scala：循环
来源：http://xdb.havefunace.top

for (i <- 1 to 10) println(i)
来源：http://zyo.hnqzz.top

[T60] Scala：折叠
来源：http://bzh.ydjk.org.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yja.hesvh.cn

================================================================================
来源：http://mio.yueranfly.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xyy.uphjek.com

================================================================================
来源：http://onq.hysaishi.cn

[U01] Py：创建虚拟环境
来源：http://ofb.yueranfly.top

python -m venv .venv && source .venv/bin/activate
来源：http://usv.vqdsnc.cn

[U02] Py：导出 / 安装依赖
来源：http://jhl.meibo888.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://idr.yj202588.top

[U03] Py：加载 .env 配置
来源：http://ues.xziqi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://dxo.zhengqikj.top

[U04] Py：变量调试打印
来源：http://cws.dashuyun.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xwl.sxryk.cn

[U05] Py：列表去重且保序
来源：http://zsu.feifeiyinyue.top

list(dict.fromkeys(arr))
来源：http://pxx.cqqwz.cn

[U06] Py：合并两个字典
来源：http://ahj.ivvv.top

{**a, **b}
来源：http://cnd.snrcjt.cn

[U07] Py：反转字典键值
来源：http://mai.yvedp.cn

{v: k for k, v in d.items()}
来源：http://isf.tian-w.cn

[U08] Py：展平二维列表
来源：http://vfj.gaohongyu789.top

[y for x in nested for y in x]
来源：http://qui.fengsongda.top

[U09] Py：字典取最大值的键
来源：http://kgu.chenzaomai.com

max(d, key=d.get)
来源：http://iid.52xcode.cn

[U10] Py：按值排序字典
来源：http://pqw.xuetiantiany.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://prm.ehwqpu.com

[U11] Py：生成器表达式
来源：http://xuv.yj20258888.top

(x * 2 for x in arr)
来源：http://bqm.fengsongda.top

[U12] Py：取出现最多的 3 个元素
来源：http://icf.shzxlz.cn

Counter(arr).most_common(3)
来源：http://cei.cashguo.top

[U13] Py：固定长度队列
来源：http://jcr.nwbrower.top

deque(maxlen=10)
来源：http://zab.pengpengdd.cyou

[U14] Py：分组收集到列表
来源：http://gap.andypj.xyz

defaultdict(list)
来源：http://ejj.mhx1999.top

[U15] Py：高精度计时
来源：http://pca.pycfn.com

t = time.perf_counter()
来源：http://kcx.yj20258888.top

[U16] Py：命令行参数解析
来源：http://jqd.fzhhl.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bmq.jinyuanbaomall.cn

[U17] Py：初始化日志
来源：http://cwt.xinyue.icu

logging.basicConfig(level=logging.INFO)
来源：http://wcg.guowangkeji.top

[U18] Py：预编译正则
来源：http://sdl.vehdjk.com

pat = re.compile(r"\d+")
来源：http://zyi.gogol.net.cn

[U19] Py：正则替换带回调
来源：http://ecp.jyoumei.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zga.meibo888.top

[U20] Py：缓存函数结果
来源：http://qoa.yfazqb.com

@functools.lru_cache(maxsize=None)
来源：http://jmt.dianchejie.cn


<!-- 参考信息 -->