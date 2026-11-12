代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vhu.yonumen.top

[S08] C：动态内存分配与释放
来源：http://pag.fehbvm.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://umg.xuanzx.com

[S09] C：结构体定义与初始化
来源：http://yyr.yvedp.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gez.cdnleiting.top

[S10] C：指针与解引用
来源：http://vtq.sweek.top

int *p = &a;  *p = 5;
来源：http://zxq.yj20258888.top

[S11] C：逐行读文件
来源：http://uxr.jyoumei.cn

FILE *f = fopen("a.txt", "r");
来源：http://uzw.aibaodan.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://fbv.0kj1m.cn

fclose(f);
来源：http://qab.daxiang520.top

[S12] C：写文件
来源：http://jqs.pengpengdd.cyou

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hma.jyoumei.cn

[S13] C：宏定义
来源：http://wrs.cashguo.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ufv.wangdashe.top

[S14] C：枚举
来源：http://jsu.jinghuilouyu.cn

enum Color { RED, GREEN, BLUE };
来源：http://gch.bjfxy.top

[S15] C：类型转换
来源：http://atu.fzhhl.top

(double) a / b
来源：http://fev.snrcjt.cn

[S16] C：位操作置位
来源：http://rin.zhoulong.xyz

x |= (1 << 3);
来源：http://keq.birdmap.top

[S17] C：安全拼接字符串
来源：http://ial.tarul.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zcg.tarul.cn

[S18] C：命令行参数
来源：http://wap.zhiwuduotai.top

int main(int argc, char **argv)
来源：http://fcx.jianghu66.top

[S19] C：快速排序
来源：http://elc.sufxvd.cn

qsort(a, n, sizeof(int), cmp);
来源：http://dxu.pengpengdd.cyou

[S20] C：二分查找
来源：http://ewy.hongshengwenyu.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ede.wangdashe.top

[S21] C：字符类别判断
来源：http://wxq.yvedp.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://djj.snrcjt.cn

[S22] C：字符串转数字
来源：http://nur.zhaomingkeji.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://ibg.feifeiyinyue.top

[S23] C：随机数
来源：http://nnh.hywenlv.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bsa.cdnleiting.top

[S24] C：获取本地时间
来源：http://ygd.wangshuangyany.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ofh.tarul.cn

[S25] C：内存拷贝
来源：http://rsm.aibaodan.cn

memcpy(dst, src, n);
来源：http://dji.snrcjt.cn

[S26] C：内存清零
来源：http://qdc.shangyingyoupin.top

memset(a, 0, sizeof a);
来源：http://mbh.sufxvd.cn

[S27] C：定义常量
来源：http://try.c1oappe.top

const double PI = 3.14159;
来源：http://mnr.jqgfzy.top

[S28] C：静态变量
来源：http://axr.ydzc1.top

static int counter = 0;
来源：http://yuu.nanxinkj.top

[S29] C：变参函数
来源：http://zac.zhijiandao.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yht.bjfxy.top

[S30] C：头文件保护
来源：http://lnt.zhiwuduotai.top

#ifndef X_H
来源：http://waz.shuidangran.top

#define X_H
来源：http://kbb.feifeiyinyue.top

#endif
来源：http://jal.gogol.net.cn

[S31] C++：Hello World
来源：http://rch.gogol.net.cn

#include <iostream>
来源：http://zww.yonumen.top

int main() { std::cout << "Hello\n"; }
来源：http://etc.zhiwuduotai.top

[S32] C++：字符串
来源：http://nce.andypj.xyz

std::string s = "hi";  s += "!";
来源：http://ygf.gaohongyu789.top

[S33] C++：vector 增删
来源：http://pno.cashguo.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lkm.jyoumei.cn

[S34] C++：遍历 vector
来源：http://ian.shzxlz.cn

for (auto &x : v) { std::cout << x; }
来源：http://upu.zdbjq.cn

[S35] C++：map
来源：http://szj.epnwcf.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vky.cqqwz.cn

[S36] C++：unordered_map
来源：http://kbi.sysykeji.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mkv.svipenyu.cn

[S37] C++：set
来源：http://ron.guannengcc.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zey.xylfe.cn

[S38] C++：排序
来源：http://tup.smart0.xyz

std::sort(v.begin(), v.end());
来源：http://mmu.xziqi.cn

[S39] C++：自定义比较器排序
来源：http://xhi.yueranfly.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zqi.jinghuilouyu.cn

[S40] C++：查找元素
来源：http://izq.jianghu66.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yvf.ybcxt.top

[S41] C++：类与构造函数
来源：http://edg.hongshengwenyu.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://plu.daxiang520.top

[S42] C++：继承与虚函数
来源：http://hsh.zhongyouzk.top

class B : public Base { public: void f() override {} };
来源：http://vav.fanxiaobao.xyz

[S43] C++：智能指针
来源：http://uxc.zhoulong.xyz

auto p = std::make_unique<int>(5);
来源：http://hza.aizwys.cn

[S44] C++：引用传参
来源：http://kvx.sysykeji.top

void inc(int &x) { ++x; }
来源：http://uak.epnwcf.com

[S45] C++：lambda
来源：http://wit.zhijiandao.cn

auto add = [](int a, int b) { return a + b; };
来源：http://vbj.52xcode.cn

[S46] C++：函数模板
来源：http://czy.jinqigfzy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://oea.9152youxi.cn

[S47] C++：结构化绑定遍历
来源：http://fbf.yongpay.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://aiy.xinyue.icu

[S48] C++：逐行读文件
来源：http://zol.epnwcf.com

std::ifstream in("a.txt");  std::string line;
来源：http://ljq.jlsjyb.cn

while (std::getline(in, line)) { }
来源：http://hak.shangyingyoupin.top

[S49] C++：写文件
来源：http://qxl.xylfe.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ddj.fanxiaobao.xyz

[S50] C++：格式化数字
来源：http://uyb.daxiang520.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://oxn.ehwqpu.com

[S51] C++：显式类型转换
来源：http://vau.yvedp.cn

static_cast<double>(a) / b
来源：http://suu.hywenlv.cn

[S52] C++：const 与 noexcept
来源：http://wty.epnwcf.com

int size() const noexcept { return n_; }
来源：http://sxf.birdmap.top

[S53] C++：移动语义
来源：http://jxs.jlsjyb.cn

std::vector<int> w = std::move(v);
来源：http://aej.hnxiangtu.top

[S54] C++：异常处理
来源：http://flq.cdnleiting.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hii.kuanghao11.cn

[S55] C++：结构化绑定
来源：http://cww.zhoulong.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://qvh.yongpay.top

[S56] C++：optional
来源：http://cdh.jinghuilouyu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vhh.haohaochexian.top

[S57] C++：编译期常量
来源：http://ruz.xuetiantiany.cn

constexpr int N = 10;
来源：http://ptz.chenjidiqi.icu

[S58] C++：命名空间
来源：http://mnh.uphjek.com

namespace ns { int f() { return 1; } }
来源：http://ilr.ybcxt.top

[S59] C++：静态断言
来源：http://zoe.chenzaomai.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ftg.jinyuanbaomall.cn

[S60] C++：遍历并删除元素
来源：http://czb.fzhhl.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gui.andypj.xyz

================================================================================
来源：http://pvk.zhaomingkeji.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lyy.redwolf501.top

================================================================================
来源：http://qin.nanxinkj.top

[T01] Kotlin：Hello World
来源：http://pqc.zhoulong.xyz

println("Hello")
来源：http://fdy.gotoacloud.top

[T02] Kotlin：变量
来源：http://euu.pengpengdd.cyou

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ymk.sysykeji.top

[T03] Kotlin：字符串模板
来源：http://pmd.jianghu66.top

"值: $b"
来源：http://udg.bjfxy.top

[T04] Kotlin：空安全
来源：http://cam.cdnleiting.top

val n: String? = null;  n?.length
来源：http://hoc.haohaochexian.top

[T05] Kotlin：when 表达式
来源：http://qev.sjlbkw.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gqu.nanxuanxn.top

[T06] Kotlin：集合映射
来源：http://yxu.jinyuanbaomall.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://puw.ydzc1.top

[T07] Kotlin：集合过滤
来源：http://qjv.hnxiangtu.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ppo.bbcook.cn

[T08] Kotlin：数据类
来源：http://ilf.jinqigufen.top

data class User(val name: String, val age: Int)
来源：http://juz.ywan-chungtsiang.top

[T09] Kotlin：扩展函数
来源：http://hlq.dashuyun.cn

fun String.exclaim() = this + "!"
来源：http://rac.sufxvd.cn

[T10] Kotlin：默认参数
来源：http://pvr.ywan-chungtsiang.top

fun greet(name: String = "World") = "Hi $name"
来源：http://nbb.jqgufenzy.top

[T11] Kotlin：协程
来源：http://fai.hcnkem.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://ndx.aibaodan.cn

[T12] Kotlin：解构声明
来源：http://rvq.uphjek.com

val (a, b) = Pair(1, 2)
来源：http://xrw.svipenyu.cn

[T13] Kotlin：只读 Map
来源：http://oja.sxryk.cn

val m = mapOf("a" to 1)
来源：http://qfs.ppjwa.cn

[T14] Kotlin：循环
来源：http://ccd.hnqzz.top

for (i in 1..10) println(i)
来源：http://pvo.fehbvm.com

[T15] Kotlin：接口
来源：http://uwd.jinqigfzy.top

interface Shape { fun area(): Double }
来源：http://eff.bbcook.cn

[T16] Swift：Hello World
来源：http://sbh.cdnleiting.top

print("Hello")
来源：http://rcq.yj20258888.top

[T17] Swift：变量与常量
来源：http://kyw.xingfuxueyuan.xyz

var a = 1;  let b = 2
来源：http://tjx.zhaomingkeji.xyz

[T18] Swift：字符串插值
来源：http://kkr.jianghu66.top

"值: \(b)"
来源：http://vao.316326.xyz

[T19] Swift：可选绑定
来源：http://bgt.dianchejie.cn

if let n = opt { print(n) }
来源：http://xgo.hesvh.cn

[T20] Swift：数组操作
来源：http://nsc.zhiwuduotai.top

var a = [1, 2, 3];  a.append(4)
来源：http://iag.hongshengwenyu.top

[T21] Swift：遍历
来源：http://zbw.wangshuangyany.cn

for x in a { print(x) }
来源：http://fhp.zdbjq.cn

[T22] Swift：字典
来源：http://phr.xuetiantiany.cn

var d = ["a": 1];  d["b"] = 2
来源：http://zwq.hcnkem.com

[T23] Swift：函数
来源：http://apk.pengpengdd.cyou

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://leg.gzhubu.top

[T24] Swift：闭包
来源：http://qrv.wangdashe.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://wbb.cucudq.cn

[T25] Swift：结构体
来源：http://xrj.guannengcc.top

struct P { var x: Int }
来源：http://ccv.tian-w.cn

[T26] Swift：类与重写
来源：http://kff.yangfankeji.com

class A: Base { override func f() {} }
来源：http://opj.epnwcf.com

[T27] Swift：错误处理
来源：http://dnz.gaohongyu789.top

do { try f() } catch { print(error) }
来源：http://kso.hywenlv.cn

[T28] Swift：枚举
来源：http://mdf.zhoulong.xyz

enum Color { case red, green }
来源：http://vhx.hcnkem.com

[T29] Swift：guard 提前返回
来源：http://wew.kuanghao11.cn

guard let x = opt else { return }
来源：http://rot.sxryk.cn

[T30] Swift：协议
来源：http://mzx.daria6918.cn

protocol Shape { func area() -> Double }
来源：http://xxy.andypj.xyz

[T31] Lua：Hello World
来源：http://arc.cashguo.top

print("Hello")
来源：http://fpo.9152youxi.cn

[T32] Lua：局部变量
来源：http://cey.redwolf501.top

local a = 1
来源：http://bga.sufxvd.cn

[T33] Lua：表（数组）
来源：http://ouk.xylfe.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://eqr.cqqwz.cn

[T34] Lua：遍历表
来源：http://via.pycfn.com

for i, v in ipairs(t) do print(i, v) end
来源：http://nhb.jyoumei.cn

[T35] Lua：字典表
来源：http://okx.0kj1m.cn

local d = { a = 1 };  d.b = 2
来源：http://qfg.fanxiaobao.xyz

[T36] Lua：函数
来源：http://ges.xingfuxueyuan.xyz

function add(a, b) return a + b end
来源：http://lvz.hywenlv.cn

[T37] Lua：字符串拼接
来源：http://hlm.zhengqikj.top

"a" .. "b"
来源：http://phj.havefunace.top

[T38] Lua：条件
来源：http://lre.birdmap.top

if x > 0 then print("正") end
来源：http://cjz.zhiwuduotai.top

[T39] Lua：模式匹配
来源：http://dpg.guowangkeji.top

string.find(s, "%d+")
来源：http://kcy.bbcook.cn

[T40] Lua：元表
来源：http://kqp.dashuyun.cn

setmetatable({}, { __index = base })
来源：http://qeh.yangfankeji.com

[T41] Perl：Hello World
来源：http://syq.hongshengwenyu.top

print "Hello\n";
来源：http://our.quarkkingdee.top

[T42] Perl：变量类型
来源：http://ksn.hnqzz.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://sro.sweek.top

[T43] Perl：字符串插值
来源：http://jns.hongshengwenyu.top

"值: $a"
来源：http://ryh.cucudq.cn

[T44] Perl：条件
来源：http://kvl.tanke756.top

if ($a > 0) { print "正"; }
来源：http://jsg.yvedp.cn

[T45] Perl：数组遍历
来源：http://grc.xuanzx.com

for my $x (@arr) { print $x; }
来源：http://jdy.bbcook.cn

[T46] Perl：哈希操作
来源：http://bks.zycfv.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ger.chenjidiqi.icu

[T47] Perl：正则捕获
来源：http://mwd.shuidangran.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://deu.yueranfly.top

[T48] Perl：正则替换
来源：http://fvf.yueranfly.top

$s =~ s/old/new/g;
来源：http://kgw.smart0.xyz

[T49] Perl：函数
来源：http://fcu.vqdsnc.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wua.shanyushiyangtech.top

[T50] Perl：逐行读文件
来源：http://zhx.zhixingplan.top

open my $fh, "<", "a.txt" or die $!;
来源：http://usl.gotoacloud.top

while (my $line = <$fh>) { print $line; }
来源：http://vit.cheryme.top

[T51] Scala：Hello World
来源：http://bdw.redwolf501.top

println("Hello")
来源：http://fwz.hammf.cn

[T52] Scala：变量
来源：http://ggp.hysaishi.cn

val a = 1;  var b = 2
来源：http://diq.jinqigfzy.top

[T53] Scala：字符串插值
来源：http://nae.bjfxy.top

s"值: $b"
来源：http://nnd.shangyingyoupin.top

[T54] Scala：集合映射
来源：http://qpt.jinqigfzy.top

List(1, 2, 3).map(_ * 2)
来源：http://rki.nanxinkj.top

[T55] Scala：集合过滤
来源：http://axi.bbcook.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xkg.hammf.cn

[T56] Scala：样例类
来源：http://ime.gaohongyu789.top

case class User(name: String, age: Int)
来源：http://nav.yangfankeji.com

[T57] Scala：模式匹配
来源：http://ygp.bjfxy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://mxq.sxryk.cn

[T58] Scala：函数定义
来源：http://ofq.jqgufenzy.top

def add(a: Int, b: Int): Int = a + b
来源：http://iyr.yangfankeji.com

[T59] Scala：循环
来源：http://sgf.wangdashe.top

for (i <- 1 to 10) println(i)
来源：http://dzr.uphjek.com

[T60] Scala：折叠
来源：http://qwj.dianchejie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qgk.yanxiufei.cn

================================================================================
来源：http://znp.xuetiantiany.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://khg.epnwcf.com

================================================================================
来源：http://ife.bbcook.cn

[U01] Py：创建虚拟环境
来源：http://blo.bjfxy.top

python -m venv .venv && source .venv/bin/activate
来源：http://lgp.jinqigufen.top

[U02] Py：导出 / 安装依赖
来源：http://ojp.shangyingyoupin.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mpf.fehbvm.com

[U03] Py：加载 .env 配置
来源：http://iys.yj20258.top

from dotenv import load_dotenv; load_dotenv()
来源：http://frl.uphjek.com

[U04] Py：变量调试打印
来源：http://jam.fanxiaobao.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xzh.meibo888.top

[U05] Py：列表去重且保序
来源：http://mxv.hongshengwenyu.top

list(dict.fromkeys(arr))
来源：http://bdp.birdmap.top

[U06] Py：合并两个字典
来源：http://abc.wangdashe.top

{**a, **b}
来源：http://prn.hnxiangtu.top

[U07] Py：反转字典键值
来源：http://jsa.yuxming.cn

{v: k for k, v in d.items()}
来源：http://pjw.c1oappe.top

[U08] Py：展平二维列表
来源：http://gvq.pengpengdd.cyou

[y for x in nested for y in x]
来源：http://tjb.xuetiantiany.cn

[U09] Py：字典取最大值的键
来源：http://syk.aibaodan.cn

max(d, key=d.get)
来源：http://acs.xinyue.icu

[U10] Py：按值排序字典
来源：http://fmv.wangdashe.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xvf.ctjpmb.com

[U11] Py：生成器表达式
来源：http://afz.shuidangran.top

(x * 2 for x in arr)
来源：http://lkr.yueranfly.top

[U12] Py：取出现最多的 3 个元素
来源：http://udk.gzhubu.top

Counter(arr).most_common(3)
来源：http://ljx.ehwqpu.com

[U13] Py：固定长度队列
来源：http://kip.jyoumei.cn

deque(maxlen=10)
来源：http://acy.meibo888.top

[U14] Py：分组收集到列表
来源：http://mwx.xuanzx.com

defaultdict(list)
来源：http://ads.epnwcf.com

[U15] Py：高精度计时
来源：http://can.hcnkem.com

t = time.perf_counter()
来源：http://bxg.sxryk.cn

[U16] Py：命令行参数解析
来源：http://wio.bbcook.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nmn.ctjpmb.com

[U17] Py：初始化日志
来源：http://xxs.shuidangran.top

logging.basicConfig(level=logging.INFO)
来源：http://uqc.nwbrower.top

[U18] Py：预编译正则
来源：http://dif.hesvh.cn

pat = re.compile(r"\d+")
来源：http://ajb.redwolf501.top

[U19] Py：正则替换带回调
来源：http://rpk.yj20258.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://eoh.nanxinkj.top

[U20] Py：缓存函数结果
来源：http://ocb.chenlongwang.top

@functools.lru_cache(maxsize=None)
来源：http://yks.meibo888.top

[U21] Py：自定义上下文管理器
来源：http://lkw.sjlbkw.cn

@contextlib.contextmanager
来源：http://axn.cucudq.cn

[U22] Py：矩阵转置
来源：http://axi.guowangkeji.top

list(zip(*m))
来源：http://gbs.jlsjyb.cn

[U23] Py：分块读取大文件
来源：http://loq.smart0.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://kff.pycfn.com

[U24] Py：路径操作
来源：http://bxj.meibo888.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lzg.aizwys.cn

[U25] Py：CSV 按字典读
来源：http://gwx.hysaishi.cn

csv.DictReader(f)
来源：http://lnb.sxryk.cn

[U26] Py：并发下载
来源：http://pkb.quarkkingdee.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wig.gaohongyu789.top

[U27] Py：异步 HTTP
来源：http://dxa.haohaochexian.top

aiohttp.ClientSession() 配合 async with
来源：http://fuv.quarkkingdee.top

[U28] Py：类型别名
来源：http://hno.quarkkingdee.top

UserId = int
来源：http://qub.zhaomingkeji.xyz

[U29] Py：属性校验
来源：http://tse.aibaodan.cn

@property 与 @x.setter 配合
来源：http://eng.hnqzz.top

[U30] Py：数据类
来源：http://kxe.sweek.top

@dataclass(slots=True)
来源：http://giw.andypj.xyz


<!-- 参考信息 -->