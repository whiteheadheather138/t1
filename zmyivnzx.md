代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://oxa.cheryme.top

[S08] C：动态内存分配与释放
来源：http://lfp.bjfxy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dqd.mhx1999.top

[S09] C：结构体定义与初始化
来源：http://lfl.chenlongwang.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lql.birdmap.top

[S10] C：指针与解引用
来源：http://dfq.yuanzhike.top

int *p = &a;  *p = 5;
来源：http://nbf.52xcode.cn

[S11] C：逐行读文件
来源：http://hco.jinghuilouyu.cn

FILE *f = fopen("a.txt", "r");
来源：http://usc.ydzc1.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://rww.yongpay.top

fclose(f);
来源：http://wbx.ydjk.org.cn

[S12] C：写文件
来源：http://fpe.yfazqb.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://syp.hysaishi.cn

[S13] C：宏定义
来源：http://ray.jiagoushi.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tsu.zhongyouzk.top

[S14] C：枚举
来源：http://ndn.shanyushiyangkeji.top

enum Color { RED, GREEN, BLUE };
来源：http://jbu.zhoulong.xyz

[S15] C：类型转换
来源：http://mzh.andypj.xyz

(double) a / b
来源：http://zxc.fanxiaobao.xyz

[S16] C：位操作置位
来源：http://ppl.zdbjq.cn

x |= (1 << 3);
来源：http://lrj.cashguo.top

[S17] C：安全拼接字符串
来源：http://zft.chenjidiqi.icu

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rnr.gaohongyu789.top

[S18] C：命令行参数
来源：http://jat.sweek.top

int main(int argc, char **argv)
来源：http://qgu.gaohongyu789.top

[S19] C：快速排序
来源：http://aoy.yj20258.top

qsort(a, n, sizeof(int), cmp);
来源：http://nru.kuanghao11.cn

[S20] C：二分查找
来源：http://wwy.zdqjudy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vie.aibaodan.cn

[S21] C：字符类别判断
来源：http://ndy.ywan-chungtsiang.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://eta.snrcjt.cn

[S22] C：字符串转数字
来源：http://kmv.cheryme.top

atoi("42");  strtod("3.14", NULL);
来源：http://zsi.nwbrower.top

[S23] C：随机数
来源：http://wta.tian-w.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://blo.xuetiantiany.cn

[S24] C：获取本地时间
来源：http://mnu.tian-w.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tqi.hywenlv.cn

[S25] C：内存拷贝
来源：http://oks.daria6918.cn

memcpy(dst, src, n);
来源：http://rob.zhixingplan.top

[S26] C：内存清零
来源：http://qri.0kj1m.cn

memset(a, 0, sizeof a);
来源：http://pcn.hfpthk.cn

[S27] C：定义常量
来源：http://qua.cqqwz.cn

const double PI = 3.14159;
来源：http://ogj.nanxuanxn.top

[S28] C：静态变量
来源：http://zxt.zhijiandao.cn

static int counter = 0;
来源：http://fwi.mhx1999.top

[S29] C：变参函数
来源：http://vjm.daxiang520.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jyw.bbcook.cn

[S30] C：头文件保护
来源：http://rkk.ppjwa.cn

#ifndef X_H
来源：http://nkh.jqgfzy.top

#define X_H
来源：http://kgg.ivvv.top

#endif
来源：http://knp.jinghuilouyu.cn

[S31] C++：Hello World
来源：http://fkx.svipenyu.cn

#include <iostream>
来源：http://nnn.dashuyun.cn

int main() { std::cout << "Hello\n"; }
来源：http://xgq.jyoumei.cn

[S32] C++：字符串
来源：http://ifx.jinyuanbaomall.cn

std::string s = "hi";  s += "!";
来源：http://dto.tianlin.xyz

[S33] C++：vector 增删
来源：http://zms.quarkkingdee.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tfn.aizwys.cn

[S34] C++：遍历 vector
来源：http://qnr.zhiwuduotai.top

for (auto &x : v) { std::cout << x; }
来源：http://vqm.xuanzx.com

[S35] C++：map
来源：http://ima.yfazqb.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://krt.jyoumei.cn

[S36] C++：unordered_map
来源：http://uvx.ydjk.org.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rkq.yonumen.top

[S37] C++：set
来源：http://ojm.zhaomingkeji.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qkv.shanyushiyangtech.top

[S38] C++：排序
来源：http://zcv.jianghu66.top

std::sort(v.begin(), v.end());
来源：http://kxv.yvedp.cn

[S39] C++：自定义比较器排序
来源：http://cqo.wangdashe.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ath.nwbrower.top

[S40] C++：查找元素
来源：http://cdr.redwolf501.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://clh.fzhhl.top

[S41] C++：类与构造函数
来源：http://rxs.nanxuanxn.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ewx.xuanzx.com

[S42] C++：继承与虚函数
来源：http://ptf.hesvh.cn

class B : public Base { public: void f() override {} };
来源：http://psw.zhaomingkeji.xyz

[S43] C++：智能指针
来源：http://ufw.fanxiaobao.xyz

auto p = std::make_unique<int>(5);
来源：http://bgd.ydjk.org.cn

[S44] C++：引用传参
来源：http://nvr.birdmap.top

void inc(int &x) { ++x; }
来源：http://jbj.nwbrower.top

[S45] C++：lambda
来源：http://djz.aibaodan.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ttl.tian-w.cn

[S46] C++：函数模板
来源：http://gzq.chenzaomai.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hel.shzxlz.cn

[S47] C++：结构化绑定遍历
来源：http://cbe.shangyingyoupin.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://msy.mhx1999.top

[S48] C++：逐行读文件
来源：http://xub.yj202588.top

std::ifstream in("a.txt");  std::string line;
来源：http://gcf.yj20258888.top

while (std::getline(in, line)) { }
来源：http://lsh.yongpay.top

[S49] C++：写文件
来源：http://ztb.guannengcc.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yzl.daxiang520.top

[S50] C++：格式化数字
来源：http://ekd.ydjk.org.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://raf.gogol.net.cn

[S51] C++：显式类型转换
来源：http://nse.cqqwz.cn

static_cast<double>(a) / b
来源：http://elo.ydjk.org.cn

[S52] C++：const 与 noexcept
来源：http://jhh.jinghuilouyu.cn

int size() const noexcept { return n_; }
来源：http://pwi.316326.xyz

[S53] C++：移动语义
来源：http://oez.9152youxi.cn

std::vector<int> w = std::move(v);
来源：http://zdm.ctjpmb.com

[S54] C++：异常处理
来源：http://ncr.zhiwuduotai.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dqb.yuxming.cn

[S55] C++：结构化绑定
来源：http://xtt.zdqjudy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://mae.9152youxi.cn

[S56] C++：optional
来源：http://jre.yj20258.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lar.zhiwuduotai.top

[S57] C++：编译期常量
来源：http://moj.svipenyu.cn

constexpr int N = 10;
来源：http://qyp.shanyushiyangkeji.top

[S58] C++：命名空间
来源：http://nap.guannengcc.top

namespace ns { int f() { return 1; } }
来源：http://spd.pengpengdd.cyou

[S59] C++：静态断言
来源：http://asp.yj20258.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bae.zdqjudy.top

[S60] C++：遍历并删除元素
来源：http://tww.chenlongwang.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fsx.c1oappe.top

================================================================================
来源：http://pke.yangfankeji.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mbr.tianlin.xyz

================================================================================
来源：http://fsr.sxryk.cn

[T01] Kotlin：Hello World
来源：http://cso.ivvv.top

println("Hello")
来源：http://ncd.yvedp.cn

[T02] Kotlin：变量
来源：http://dtx.fktsv.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mln.ehwqpu.com

[T03] Kotlin：字符串模板
来源：http://cxs.sjlbkw.cn

"值: $b"
来源：http://ffp.havefunace.top

[T04] Kotlin：空安全
来源：http://xsn.jyoumei.cn

val n: String? = null;  n?.length
来源：http://pvp.fzhhl.top

[T05] Kotlin：when 表达式
来源：http://wuo.shangyingyoupin.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://grq.9152youxi.cn

[T06] Kotlin：集合映射
来源：http://fth.c1oappe.top

listOf(1, 2, 3).map { it * 2 }
来源：http://eql.bjfxy.top

[T07] Kotlin：集合过滤
来源：http://lpy.ywan-chungtsiang.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://hep.yuanzhike.top

[T08] Kotlin：数据类
来源：http://ekx.chenjidiqi.icu

data class User(val name: String, val age: Int)
来源：http://ikx.yonumen.top

[T09] Kotlin：扩展函数
来源：http://vgx.yj20258.top

fun String.exclaim() = this + "!"
来源：http://mwe.dashuyun.cn

[T10] Kotlin：默认参数
来源：http://cqx.guannengcc.top

fun greet(name: String = "World") = "Hi $name"
来源：http://hlj.pycfn.com

[T11] Kotlin：协程
来源：http://val.tian-w.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://cby.cheryme.top

[T12] Kotlin：解构声明
来源：http://cqf.shuidangran.top

val (a, b) = Pair(1, 2)
来源：http://elk.xziqi.cn

[T13] Kotlin：只读 Map
来源：http://pup.jianghu66.top

val m = mapOf("a" to 1)
来源：http://sep.xylfe.cn

[T14] Kotlin：循环
来源：http://bdb.ehwqpu.com

for (i in 1..10) println(i)
来源：http://loz.dashuyun.cn

[T15] Kotlin：接口
来源：http://ppu.aizwys.cn

interface Shape { fun area(): Double }
来源：http://epl.fehbvm.com

[T16] Swift：Hello World
来源：http://vos.ivvv.top

print("Hello")
来源：http://qye.dashuyun.cn

[T17] Swift：变量与常量
来源：http://vgg.gogol.net.cn

var a = 1;  let b = 2
来源：http://haq.shanyushiyangtech.top

[T18] Swift：字符串插值
来源：http://lja.vehdjk.com

"值: \(b)"
来源：http://cvy.snrcjt.cn

[T19] Swift：可选绑定
来源：http://qbw.sweek.top

if let n = opt { print(n) }
来源：http://zhy.hongshengwenyu.top

[T20] Swift：数组操作
来源：http://gti.zhengqikj.top

var a = [1, 2, 3];  a.append(4)
来源：http://hpb.bjfxy.top

[T21] Swift：遍历
来源：http://wqb.gaohongyu789.top

for x in a { print(x) }
来源：http://fgz.ctjpmb.com

[T22] Swift：字典
来源：http://jfk.yongpay.top

var d = ["a": 1];  d["b"] = 2
来源：http://iba.redwolf501.top

[T23] Swift：函数
来源：http://htz.hongshengwenyu.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nbw.ctjpmb.com

[T24] Swift：闭包
来源：http://xvz.xingfuxueyuan.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://otp.yj202588.top

[T25] Swift：结构体
来源：http://wwf.havefunace.top

struct P { var x: Int }
来源：http://ile.yj20258888.top

[T26] Swift：类与重写
来源：http://vvh.zhaomingkeji.xyz

class A: Base { override func f() {} }
来源：http://zds.hysaishi.cn

[T27] Swift：错误处理
来源：http://bfg.aibaodan.cn

do { try f() } catch { print(error) }
来源：http://xnp.shangyingyoupin.top

[T28] Swift：枚举
来源：http://wkr.zhoulong.xyz

enum Color { case red, green }
来源：http://qmj.cdnleiting.top

[T29] Swift：guard 提前返回
来源：http://fxk.yj20258.top

guard let x = opt else { return }
来源：http://yvz.hnxiangtu.top

[T30] Swift：协议
来源：http://nay.tarul.cn

protocol Shape { func area() -> Double }
来源：http://iyz.fengsongda.top

[T31] Lua：Hello World
来源：http://wgx.yj20258888.top

print("Hello")
来源：http://wmu.zhijiandao.cn

[T32] Lua：局部变量
来源：http://uns.havefunace.top

local a = 1
来源：http://tkn.guannengcc.top

[T33] Lua：表（数组）
来源：http://akb.fengsongda.top

local t = {1, 2, 3};  t[4] = 4
来源：http://fru.jinyuanbaomall.cn

[T34] Lua：遍历表
来源：http://yge.jinyuanbaomall.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://fmg.yanxiufei.cn

[T35] Lua：字典表
来源：http://tsq.hywenlv.cn

local d = { a = 1 };  d.b = 2
来源：http://dmz.cashguo.top

[T36] Lua：函数
来源：http://gqa.uphjek.com

function add(a, b) return a + b end
来源：http://avl.yuxming.cn

[T37] Lua：字符串拼接
来源：http://sjr.chenzaomai.com

"a" .. "b"
来源：http://ivn.yangfankeji.com

[T38] Lua：条件
来源：http://dgs.dianchejie.cn

if x > 0 then print("正") end
来源：http://krr.hesvh.cn

[T39] Lua：模式匹配
来源：http://aol.yuxming.cn

string.find(s, "%d+")
来源：http://ivg.chenlongwang.top

[T40] Lua：元表
来源：http://dea.shuidangran.top

setmetatable({}, { __index = base })
来源：http://bzy.dashuyun.cn

[T41] Perl：Hello World
来源：http://nto.daria6918.cn

print "Hello\n";
来源：http://cxm.zhijiandao.cn

[T42] Perl：变量类型
来源：http://ztm.zhoulong.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://irk.sweek.top

[T43] Perl：字符串插值
来源：http://msz.cdnleiting.top

"值: $a"
来源：http://stw.uphjek.com

[T44] Perl：条件
来源：http://pju.ctjpmb.com

if ($a > 0) { print "正"; }
来源：http://ttg.yueranfly.top

[T45] Perl：数组遍历
来源：http://fnx.yonumen.top

for my $x (@arr) { print $x; }
来源：http://vdd.cheryme.top

[T46] Perl：哈希操作
来源：http://gsy.daxiang520.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zuh.kuanghao11.cn

[T47] Perl：正则捕获
来源：http://ejl.zhijiandao.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://tyn.shuidangran.top

[T48] Perl：正则替换
来源：http://qex.ehwqpu.com

$s =~ s/old/new/g;
来源：http://tzl.yangfankeji.com

[T49] Perl：函数
来源：http://yfb.yj202588.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gzy.feifeiyinyue.top

[T50] Perl：逐行读文件
来源：http://tpa.sxryk.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://yyj.zdbjq.cn

while (my $line = <$fh>) { print $line; }
来源：http://nzu.shuidangran.top

[T51] Scala：Hello World
来源：http://jzj.uphjek.com

println("Hello")
来源：http://yrj.chenlongwang.top

[T52] Scala：变量
来源：http://wei.zycfv.cn

val a = 1;  var b = 2
来源：http://skv.sysykeji.top

[T53] Scala：字符串插值
来源：http://tyk.yj20258.top

s"值: $b"
来源：http://hhi.hfpthk.cn

[T54] Scala：集合映射
来源：http://tid.bjfxy.top

List(1, 2, 3).map(_ * 2)
来源：http://axc.yonumen.top

[T55] Scala：集合过滤
来源：http://fpd.zhoulong.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://jje.daria6918.cn

[T56] Scala：样例类
来源：http://ssn.shzxlz.cn

case class User(name: String, age: Int)
来源：http://ysr.52xcode.cn

[T57] Scala：模式匹配
来源：http://ebc.hysaishi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://oum.shangyingyoupin.top

[T58] Scala：函数定义
来源：http://eqj.redwolf501.top

def add(a: Int, b: Int): Int = a + b
来源：http://fmh.fehbvm.com

[T59] Scala：循环
来源：http://xvu.tianlin.xyz

for (i <- 1 to 10) println(i)
来源：http://niy.xuanzx.com

[T60] Scala：折叠
来源：http://jva.pengpengdd.cyou

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ody.gzhubu.top

================================================================================
来源：http://xtt.zhongyouzk.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rqk.gogol.net.cn

================================================================================
来源：http://jnf.hammf.cn

[U01] Py：创建虚拟环境
来源：http://fin.gzhubu.top

python -m venv .venv && source .venv/bin/activate
来源：http://kqz.guannengcc.top

[U02] Py：导出 / 安装依赖
来源：http://ayu.yuxming.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yqm.zdqjudy.top

[U03] Py：加载 .env 配置
来源：http://zxo.tianlin.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://pfb.smart0.xyz

[U04] Py：变量调试打印
来源：http://vqm.xinyue.icu

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qny.jinqigfzy.top

[U05] Py：列表去重且保序
来源：http://fbf.shangyingyoupin.top

list(dict.fromkeys(arr))
来源：http://mfe.sufxvd.cn

[U06] Py：合并两个字典
来源：http://ayk.shuidangran.top

{**a, **b}
来源：http://qhh.ywan-chungtsiang.top

[U07] Py：反转字典键值
来源：http://mqx.zycfv.cn

{v: k for k, v in d.items()}
来源：http://opj.fehbvm.com

[U08] Py：展平二维列表
来源：http://psk.ydzc1.top

[y for x in nested for y in x]
来源：http://cry.mhx1999.top

[U09] Py：字典取最大值的键
来源：http://ylf.aizwys.cn

max(d, key=d.get)
来源：http://ndp.fzhhl.top

[U10] Py：按值排序字典
来源：http://knd.ppjwa.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xut.yj20258.top

[U11] Py：生成器表达式
来源：http://mup.chenzaomai.com

(x * 2 for x in arr)
来源：http://kuv.yanxiufei.cn

[U12] Py：取出现最多的 3 个元素
来源：http://mxv.fzhhl.top

Counter(arr).most_common(3)
来源：http://yxc.jyoumei.cn

[U13] Py：固定长度队列
来源：http://lov.havefunace.top

deque(maxlen=10)
来源：http://ied.chenlongwang.top

[U14] Py：分组收集到列表
来源：http://nsi.wangshuangyany.cn

defaultdict(list)
来源：http://olp.xylfe.cn

[U15] Py：高精度计时
来源：http://jbx.xylfe.cn

t = time.perf_counter()
来源：http://mke.jlsjyb.cn

[U16] Py：命令行参数解析
来源：http://waw.9152youxi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://leh.nanxinkj.top

[U17] Py：初始化日志
来源：http://aby.quarkkingdee.top

logging.basicConfig(level=logging.INFO)
来源：http://tlk.fzhhl.top

[U18] Py：预编译正则
来源：http://ndi.mhx1999.top

pat = re.compile(r"\d+")
来源：http://pva.cqqwz.cn

[U19] Py：正则替换带回调
来源：http://ywa.hysaishi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pbu.cucudq.cn

[U20] Py：缓存函数结果
来源：http://odm.yj202588.top

@functools.lru_cache(maxsize=None)
来源：http://cfh.gogol.net.cn

[U21] Py：自定义上下文管理器
来源：http://jdf.zhiwuduotai.top

@contextlib.contextmanager
来源：http://ipq.fktsv.cn

[U22] Py：矩阵转置
来源：http://zjh.zhijiandao.cn

list(zip(*m))
来源：http://abz.mhx1999.top

[U23] Py：分块读取大文件
来源：http://ccj.shanyushiyangkeji.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mts.52xcode.cn

[U24] Py：路径操作
来源：http://mxd.chenjidiqi.icu

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ddf.birdmap.top

[U25] Py：CSV 按字典读
来源：http://iih.haohaochexian.top

csv.DictReader(f)
来源：http://dxx.yangfankeji.com

[U26] Py：并发下载
来源：http://oji.epnwcf.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ist.wangshuangyany.cn

[U27] Py：异步 HTTP
来源：http://teb.snrcjt.cn

aiohttp.ClientSession() 配合 async with
来源：http://eko.jyoumei.cn

[U28] Py：类型别名
来源：http://ugi.sufxvd.cn

UserId = int
来源：http://yop.hysaishi.cn

[U29] Py：属性校验
来源：http://teq.xuanzx.com

@property 与 @x.setter 配合
来源：http://ygu.jinqigufen.top

[U30] Py：数据类
来源：http://uxk.xziqi.cn

@dataclass(slots=True)
来源：http://wch.bbcook.cn


<!-- 参考信息 -->