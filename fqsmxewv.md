代发 wailian999

S. C / C++ 专题
来源：http://fvw.bbcook.cn

================================================================================
来源：http://qhl.yj20258.top

[S01] C：Hello World
来源：http://hfo.zhixingplan.top

#include <stdio.h>
来源：http://xwl.c1oappe.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://cyf.jlsjyb.cn

[S02] C：变量与格式化输出
来源：http://poy.pycfn.com

int a = 10; printf("%d\n", a);
来源：http://ktj.jinqigfzy.top

[S03] C：读入整数
来源：http://pvc.yanxiufei.cn

int x; scanf("%d", &x);
来源：http://ogq.tianlin.xyz

[S04] C：字符串复制
来源：http://gim.guowangkeji.top

char dst[32]; strcpy(dst, "hi");
来源：http://tpd.9152youxi.cn

[S05] C：字符串长度
来源：http://cck.hammf.cn

strlen(s)
来源：http://oei.yuxming.cn

[S06] C：字符串比较
来源：http://frn.havefunace.top

strcmp(a, b) == 0
来源：http://hih.sufxvd.cn

[S07] C：数组遍历求和
来源：http://fxq.guannengcc.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kwv.ehwqpu.com

[S08] C：动态内存分配与释放
来源：http://ezi.fzhhl.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yco.hfpthk.cn

[S09] C：结构体定义与初始化
来源：http://bep.jinghuilouyu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ffu.ppjwa.cn

[S10] C：指针与解引用
来源：http://eif.tianlin.xyz

int *p = &a;  *p = 5;
来源：http://odn.uphjek.com

[S11] C：逐行读文件
来源：http://pyt.birdmap.top

FILE *f = fopen("a.txt", "r");
来源：http://wzq.xuetiantiany.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://anr.jinqigfzy.top

fclose(f);
来源：http://vve.shuidangran.top

[S12] C：写文件
来源：http://egh.ppjwa.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xla.svipenyu.cn

[S13] C：宏定义
来源：http://wjl.jlsjyb.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://oas.fktsv.cn

[S14] C：枚举
来源：http://scw.smart0.xyz

enum Color { RED, GREEN, BLUE };
来源：http://oor.andypj.xyz

[S15] C：类型转换
来源：http://xro.hongshengwenyu.top

(double) a / b
来源：http://xkw.wangdashe.top

[S16] C：位操作置位
来源：http://xjn.shanyushiyangtech.top

x |= (1 << 3);
来源：http://zip.zhijiandao.cn

[S17] C：安全拼接字符串
来源：http://qxu.vqdsnc.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jop.sweek.top

[S18] C：命令行参数
来源：http://nbl.bbcook.cn

int main(int argc, char **argv)
来源：http://dbn.yj20258.top

[S19] C：快速排序
来源：http://toi.cashguo.top

qsort(a, n, sizeof(int), cmp);
来源：http://bzz.shuidangran.top

[S20] C：二分查找
来源：http://hnb.smart0.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xbf.yuanzhike.top

[S21] C：字符类别判断
来源：http://kgf.gzhubu.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sph.dashuyun.cn

[S22] C：字符串转数字
来源：http://qwg.sxryk.cn

atoi("42");  strtod("3.14", NULL);
来源：http://jgr.zycfv.cn

[S23] C：随机数
来源：http://xss.yfazqb.com

srand(time(NULL));  int r = rand() % 100;
来源：http://ppc.yongpay.top

[S24] C：获取本地时间
来源：http://fre.zdqjudy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://quv.zdqjudy.top

[S25] C：内存拷贝
来源：http://gpp.yj20258888.top

memcpy(dst, src, n);
来源：http://ypy.sufxvd.cn

[S26] C：内存清零
来源：http://wmv.zhongyouzk.top

memset(a, 0, sizeof a);
来源：http://zuq.jyoumei.cn

[S27] C：定义常量
来源：http://bud.yueranfly.top

const double PI = 3.14159;
来源：http://fwq.ctjpmb.com

[S28] C：静态变量
来源：http://htj.birdmap.top

static int counter = 0;
来源：http://ywf.zhaomingkeji.xyz

[S29] C：变参函数
来源：http://mfr.gzhubu.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://svc.sweek.top

[S30] C：头文件保护
来源：http://axv.mhx1999.top

#ifndef X_H
来源：http://dty.sufxvd.cn

#define X_H
来源：http://oik.iojbl.cn

#endif
来源：http://qht.gzhubu.top

[S31] C++：Hello World
来源：http://jvl.sxryk.cn

#include <iostream>
来源：http://zke.hnqzz.top

int main() { std::cout << "Hello\n"; }
来源：http://iyu.dashuyun.cn

[S32] C++：字符串
来源：http://qqd.9152youxi.cn

std::string s = "hi";  s += "!";
来源：http://zrx.zdqjudy.top

[S33] C++：vector 增删
来源：http://kcq.ppjwa.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jby.cucudq.cn

[S34] C++：遍历 vector
来源：http://mxg.jlsjyb.cn

for (auto &x : v) { std::cout << x; }
来源：http://fdc.zhixingplan.top

[S35] C++：map
来源：http://vhc.andypj.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://iyi.chenjidiqi.icu

[S36] C++：unordered_map
来源：http://dlb.chenlongwang.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://car.hnxiangtu.top

[S37] C++：set
来源：http://bgd.tanke756.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://htz.yuanzhike.top

[S38] C++：排序
来源：http://yzh.daria6918.cn

std::sort(v.begin(), v.end());
来源：http://ych.feifeiyinyue.top

[S39] C++：自定义比较器排序
来源：http://kjo.xuanzx.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vxa.shuidangran.top

[S40] C++：查找元素
来源：http://kvg.chenlongwang.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pho.fehbvm.com

[S41] C++：类与构造函数
来源：http://mcu.kuanghao11.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jai.ydzc1.top

[S42] C++：继承与虚函数
来源：http://lei.yj20258888.top

class B : public Base { public: void f() override {} };
来源：http://piy.yueranfly.top

[S43] C++：智能指针
来源：http://zoj.svipenyu.cn

auto p = std::make_unique<int>(5);
来源：http://xqb.havefunace.top

[S44] C++：引用传参
来源：http://nox.0kj1m.cn

void inc(int &x) { ++x; }
来源：http://ppe.epnwcf.com

[S45] C++：lambda
来源：http://yla.shanyushiyangtech.top

auto add = [](int a, int b) { return a + b; };
来源：http://orw.jinyuanbaomall.cn

[S46] C++：函数模板
来源：http://thv.hesvh.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ncw.dashuyun.cn

[S47] C++：结构化绑定遍历
来源：http://isa.andypj.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://var.sjlbkw.cn

[S48] C++：逐行读文件
来源：http://cnu.shanyushiyangkeji.top

std::ifstream in("a.txt");  std::string line;
来源：http://pmt.yanxiufei.cn

while (std::getline(in, line)) { }
来源：http://qis.tanke756.top

[S49] C++：写文件
来源：http://uey.sweek.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bxl.zhaomingkeji.xyz

[S50] C++：格式化数字
来源：http://gvc.jqgfzy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gqz.hywenlv.cn

[S51] C++：显式类型转换
来源：http://bir.yfazqb.com

static_cast<double>(a) / b
来源：http://bbv.jinqigfzy.top

[S52] C++：const 与 noexcept
来源：http://myw.hysaishi.cn

int size() const noexcept { return n_; }
来源：http://acw.hnxiangtu.top

[S53] C++：移动语义
来源：http://rxd.hammf.cn

std::vector<int> w = std::move(v);
来源：http://alv.0kj1m.cn

[S54] C++：异常处理
来源：http://mtt.yj202588.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tys.jyoumei.cn

[S55] C++：结构化绑定
来源：http://pvp.fanxiaobao.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://gqm.zycfv.cn

[S56] C++：optional
来源：http://qrr.yangfankeji.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ilu.nanxuanxn.top

[S57] C++：编译期常量
来源：http://opx.bjfxy.top

constexpr int N = 10;
来源：http://ldy.snrcjt.cn

[S58] C++：命名空间
来源：http://gmm.gotoacloud.top

namespace ns { int f() { return 1; } }
来源：http://toa.yongpay.top

[S59] C++：静态断言
来源：http://oqh.fktsv.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yvq.redwolf501.top

[S60] C++：遍历并删除元素
来源：http://pxh.meibo888.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yfw.zdbjq.cn

================================================================================
来源：http://kfu.sufxvd.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jbu.316326.xyz

================================================================================
来源：http://xwe.xylfe.cn

[T01] Kotlin：Hello World
来源：http://hfb.yj202588.top

println("Hello")
来源：http://vea.52xcode.cn

[T02] Kotlin：变量
来源：http://cpc.bjfxy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hri.jinghuilouyu.cn

[T03] Kotlin：字符串模板
来源：http://dqa.svipenyu.cn

"值: $b"
来源：http://mtn.ehwqpu.com

[T04] Kotlin：空安全
来源：http://cwe.epnwcf.com

val n: String? = null;  n?.length
来源：http://tvf.jianghu66.top

[T05] Kotlin：when 表达式
来源：http://fhy.redwolf501.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jen.birdmap.top

[T06] Kotlin：集合映射
来源：http://vik.zhoulong.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://jwg.hongshengwenyu.top

[T07] Kotlin：集合过滤
来源：http://hcy.ehwqpu.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://mkv.ivvv.top

[T08] Kotlin：数据类
来源：http://gtu.uphjek.com

data class User(val name: String, val age: Int)
来源：http://ubj.nanxuanxn.top

[T09] Kotlin：扩展函数
来源：http://fyj.fengsongda.top

fun String.exclaim() = this + "!"
来源：http://hlk.cheryme.top

[T10] Kotlin：默认参数
来源：http://hqv.gogol.net.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://hso.gaohongyu789.top

[T11] Kotlin：协程
来源：http://rtq.vehdjk.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://lnc.zdqjudy.top

[T12] Kotlin：解构声明
来源：http://anr.pengpengdd.cyou

val (a, b) = Pair(1, 2)
来源：http://xku.52xcode.cn

[T13] Kotlin：只读 Map
来源：http://bgq.epnwcf.com

val m = mapOf("a" to 1)
来源：http://edn.fktsv.cn

[T14] Kotlin：循环
来源：http://brf.daxiang520.top

for (i in 1..10) println(i)
来源：http://ocg.hnqzz.top

[T15] Kotlin：接口
来源：http://lly.zhiwuduotai.top

interface Shape { fun area(): Double }
来源：http://txx.hesvh.cn

[T16] Swift：Hello World
来源：http://ltq.cdnleiting.top

print("Hello")
来源：http://frv.gogol.net.cn

[T17] Swift：变量与常量
来源：http://nhk.cqqwz.cn

var a = 1;  let b = 2
来源：http://grc.zdbjq.cn

[T18] Swift：字符串插值
来源：http://wkn.bbcook.cn

"值: \(b)"
来源：http://sdn.zhijiandao.cn

[T19] Swift：可选绑定
来源：http://jml.wangshuangyany.cn

if let n = opt { print(n) }
来源：http://nax.aizwys.cn

[T20] Swift：数组操作
来源：http://prp.havefunace.top

var a = [1, 2, 3];  a.append(4)
来源：http://rtn.ydzc1.top

[T21] Swift：遍历
来源：http://nxv.bjfxy.top

for x in a { print(x) }
来源：http://ipt.yj202588.top

[T22] Swift：字典
来源：http://gko.zhixingplan.top

var d = ["a": 1];  d["b"] = 2
来源：http://lkw.ywan-chungtsiang.top

[T23] Swift：函数
来源：http://lvq.jianghu66.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://add.mhx1999.top

[T24] Swift：闭包
来源：http://lde.redwolf501.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://fts.wangdashe.top

[T25] Swift：结构体
来源：http://svy.chenzaomai.com

struct P { var x: Int }
来源：http://abh.hysaishi.cn

[T26] Swift：类与重写
来源：http://cke.yanxiufei.cn

class A: Base { override func f() {} }
来源：http://cwg.guannengcc.top

[T27] Swift：错误处理
来源：http://xjb.nanxuanxn.top

do { try f() } catch { print(error) }
来源：http://kfg.yj202588.top

[T28] Swift：枚举
来源：http://rvr.zhiwuduotai.top

enum Color { case red, green }
来源：http://ytv.shuidangran.top

[T29] Swift：guard 提前返回
来源：http://lzs.feifeiyinyue.top

guard let x = opt else { return }
来源：http://ele.gaohongyu789.top

[T30] Swift：协议
来源：http://zwp.zdbjq.cn

protocol Shape { func area() -> Double }
来源：http://ywf.nwbrower.top

[T31] Lua：Hello World
来源：http://hey.sweek.top

print("Hello")
来源：http://cla.yj20258.top

[T32] Lua：局部变量
来源：http://edi.jinqigfzy.top

local a = 1
来源：http://fxt.jinqigfzy.top

[T33] Lua：表（数组）
来源：http://ydl.nwbrower.top

local t = {1, 2, 3};  t[4] = 4
来源：http://peh.iojbl.cn

[T34] Lua：遍历表
来源：http://xjn.zhoulong.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://zcj.zhaomingkeji.xyz

[T35] Lua：字典表
来源：http://vds.gaohongyu789.top

local d = { a = 1 };  d.b = 2
来源：http://ayo.shuidangran.top

[T36] Lua：函数
来源：http://nxy.wangshuangyany.cn

function add(a, b) return a + b end
来源：http://qov.ctjpmb.com

[T37] Lua：字符串拼接
来源：http://pvw.jinqigfzy.top

"a" .. "b"
来源：http://zrs.gogol.net.cn

[T38] Lua：条件
来源：http://scx.jyoumei.cn

if x > 0 then print("正") end
来源：http://wod.feifeiyinyue.top

[T39] Lua：模式匹配
来源：http://fol.vehdjk.com

string.find(s, "%d+")
来源：http://yqr.jqgfzy.top

[T40] Lua：元表
来源：http://ohg.ydzc1.top

setmetatable({}, { __index = base })
来源：http://wao.yj20258.top

[T41] Perl：Hello World
来源：http://xse.yj202588.top

print "Hello\n";
来源：http://pij.zhixingplan.top

[T42] Perl：变量类型
来源：http://kqe.daxiang520.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nbr.mhx1999.top

[T43] Perl：字符串插值
来源：http://esa.c1oappe.top

"值: $a"
来源：http://the.9152youxi.cn

[T44] Perl：条件
来源：http://ppb.redwolf501.top

if ($a > 0) { print "正"; }
来源：http://npn.daxiang520.top

[T45] Perl：数组遍历
来源：http://eoh.hesvh.cn

for my $x (@arr) { print $x; }
来源：http://kgp.shangyingyoupin.top

[T46] Perl：哈希操作
来源：http://bsy.svipenyu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wts.svipenyu.cn

[T47] Perl：正则捕获
来源：http://hvf.yongpay.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://klj.tanke756.top

[T48] Perl：正则替换
来源：http://khf.zhiwuduotai.top

$s =~ s/old/new/g;
来源：http://sfr.sufxvd.cn

[T49] Perl：函数
来源：http://xah.yvedp.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://psx.ydjk.org.cn

[T50] Perl：逐行读文件
来源：http://axi.yuanzhike.top

open my $fh, "<", "a.txt" or die $!;
来源：http://wrb.shanyushiyangkeji.top

while (my $line = <$fh>) { print $line; }
来源：http://hph.jinqigufen.top

[T51] Scala：Hello World
来源：http://axc.ydjk.org.cn

println("Hello")
来源：http://onj.zycfv.cn

[T52] Scala：变量
来源：http://mny.svipenyu.cn

val a = 1;  var b = 2
来源：http://veg.yangfankeji.com

[T53] Scala：字符串插值
来源：http://yuv.fzhhl.top

s"值: $b"
来源：http://dnv.xylfe.cn

[T54] Scala：集合映射
来源：http://epg.kuanghao11.cn

List(1, 2, 3).map(_ * 2)
来源：http://edl.cdnleiting.top

[T55] Scala：集合过滤
来源：http://bvj.bjfxy.top

List(1, 2, 3).filter(_ > 1)
来源：http://gyb.yj20258.top

[T56] Scala：样例类
来源：http://guy.hnqzz.top

case class User(name: String, age: Int)
来源：http://gil.zhiwuduotai.top

[T57] Scala：模式匹配
来源：http://jwc.svipenyu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vzk.snrcjt.cn

[T58] Scala：函数定义
来源：http://mqm.gzhubu.top

def add(a: Int, b: Int): Int = a + b
来源：http://ycs.yj202588.top

[T59] Scala：循环
来源：http://dod.feifeiyinyue.top

for (i <- 1 to 10) println(i)
来源：http://isg.yongpay.top

[T60] Scala：折叠
来源：http://gdp.cqqwz.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://eej.xylfe.cn

================================================================================
来源：http://ags.9152youxi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://isn.yueranfly.top

================================================================================
来源：http://oai.aizwys.cn

[U01] Py：创建虚拟环境
来源：http://npt.dashuyun.cn

python -m venv .venv && source .venv/bin/activate
来源：http://agz.xinyue.icu

[U02] Py：导出 / 安装依赖
来源：http://frl.yfazqb.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zbf.quarkkingdee.top

[U03] Py：加载 .env 配置
来源：http://tee.c1oappe.top

from dotenv import load_dotenv; load_dotenv()
来源：http://thu.zdbjq.cn

[U04] Py：变量调试打印
来源：http://xpi.vqdsnc.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://efb.zhijiandao.cn

[U05] Py：列表去重且保序
来源：http://ymq.zycfv.cn

list(dict.fromkeys(arr))
来源：http://kcs.chenzaomai.com

[U06] Py：合并两个字典
来源：http://fnq.yfazqb.com

{**a, **b}
来源：http://nxd.shanyushiyangkeji.top

[U07] Py：反转字典键值
来源：http://bch.iojbl.cn

{v: k for k, v in d.items()}
来源：http://lin.c1oappe.top

[U08] Py：展平二维列表
来源：http://nqq.fzhhl.top

[y for x in nested for y in x]
来源：http://qig.ivvv.top

[U09] Py：字典取最大值的键
来源：http://sgr.jqgufenzy.top

max(d, key=d.get)
来源：http://jfj.yangfankeji.com

[U10] Py：按值排序字典
来源：http://xnh.jqgufenzy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wbm.shanyushiyangkeji.top

[U11] Py：生成器表达式
来源：http://fvm.nanxuanxn.top

(x * 2 for x in arr)
来源：http://swc.svipenyu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://gyg.haohaochexian.top

Counter(arr).most_common(3)
来源：http://qwl.yj20258888.top

[U13] Py：固定长度队列
来源：http://bte.zdqjudy.top

deque(maxlen=10)
来源：http://vph.hammf.cn

[U14] Py：分组收集到列表
来源：http://qxx.vqdsnc.cn

defaultdict(list)
来源：http://hmi.ppjwa.cn

[U15] Py：高精度计时
来源：http://ujr.hywenlv.cn

t = time.perf_counter()
来源：http://mlw.nanxinkj.top

[U16] Py：命令行参数解析
来源：http://eav.yuanzhike.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://las.haohaochexian.top

[U17] Py：初始化日志
来源：http://apc.ywan-chungtsiang.top

logging.basicConfig(level=logging.INFO)
来源：http://xjq.jinqigufen.top

[U18] Py：预编译正则
来源：http://hsj.ydjk.org.cn

pat = re.compile(r"\d+")
来源：http://vwl.sxryk.cn

[U19] Py：正则替换带回调
来源：http://sbk.jinghuilouyu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://exg.jqgufenzy.top

[U20] Py：缓存函数结果
来源：http://thp.zhijiandao.cn

@functools.lru_cache(maxsize=None)
来源：http://bty.meibo888.top

[U21] Py：自定义上下文管理器
来源：http://bzf.shzxlz.cn

@contextlib.contextmanager
来源：http://ejb.jinqigufen.top

[U22] Py：矩阵转置
来源：http://jgq.sjlbkw.cn

list(zip(*m))
来源：http://ruy.zycfv.cn


<!-- 参考信息 -->