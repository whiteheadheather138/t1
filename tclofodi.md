代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://uyh.xuanzx.com

[S15] C：类型转换
来源：http://qou.hnxiangtu.top

(double) a / b
来源：http://oyt.jinqigfzy.top

[S16] C：位操作置位
来源：http://qsf.gzhubu.top

x |= (1 << 3);
来源：http://syj.shzxlz.cn

[S17] C：安全拼接字符串
来源：http://cbb.ydjk.org.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mtc.cucudq.cn

[S18] C：命令行参数
来源：http://yao.shangyingyoupin.top

int main(int argc, char **argv)
来源：http://hid.shangyingyoupin.top

[S19] C：快速排序
来源：http://uiw.c1oappe.top

qsort(a, n, sizeof(int), cmp);
来源：http://poe.tianlin.xyz

[S20] C：二分查找
来源：http://xbs.hongshengwenyu.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yet.wangdashe.top

[S21] C：字符类别判断
来源：http://keb.tarul.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://opd.tian-w.cn

[S22] C：字符串转数字
来源：http://wly.zhoulong.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://jlj.ydzc1.top

[S23] C：随机数
来源：http://yal.cashguo.top

srand(time(NULL));  int r = rand() % 100;
来源：http://thr.zycfv.cn

[S24] C：获取本地时间
来源：http://gxm.mhx1999.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zvx.zhaomingkeji.xyz

[S25] C：内存拷贝
来源：http://meg.xingfuxueyuan.xyz

memcpy(dst, src, n);
来源：http://npr.yj20258888.top

[S26] C：内存清零
来源：http://lrh.yj202588.top

memset(a, 0, sizeof a);
来源：http://sse.chenlongwang.top

[S27] C：定义常量
来源：http://nhw.fanxiaobao.xyz

const double PI = 3.14159;
来源：http://cdh.zhoulong.xyz

[S28] C：静态变量
来源：http://wkp.jqgufenzy.top

static int counter = 0;
来源：http://kxd.haohaochexian.top

[S29] C：变参函数
来源：http://npj.0kj1m.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nkr.ybcxt.top

[S30] C：头文件保护
来源：http://xtm.fzhhl.top

#ifndef X_H
来源：http://atz.nanxinkj.top

#define X_H
来源：http://sex.yj20258.top

#endif
来源：http://hoz.yfazqb.com

[S31] C++：Hello World
来源：http://eqb.sjlbkw.cn

#include <iostream>
来源：http://gdb.andypj.xyz

int main() { std::cout << "Hello\n"; }
来源：http://xyj.yongpay.top

[S32] C++：字符串
来源：http://kgy.yonumen.top

std::string s = "hi";  s += "!";
来源：http://khm.yonumen.top

[S33] C++：vector 增删
来源：http://xvm.shuidangran.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://car.jqgfzy.top

[S34] C++：遍历 vector
来源：http://rwr.zhijiandao.cn

for (auto &x : v) { std::cout << x; }
来源：http://cmm.ivvv.top

[S35] C++：map
来源：http://dou.aizwys.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zap.yj202588.top

[S36] C++：unordered_map
来源：http://qhn.yuanzhike.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fwn.uphjek.com

[S37] C++：set
来源：http://eqj.shanyushiyangtech.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hnh.fengsongda.top

[S38] C++：排序
来源：http://zar.guowangkeji.top

std::sort(v.begin(), v.end());
来源：http://mev.chenzaomai.com

[S39] C++：自定义比较器排序
来源：http://sod.cqqwz.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dco.yueranfly.top

[S40] C++：查找元素
来源：http://zcb.birdmap.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fri.kuanghao11.cn

[S41] C++：类与构造函数
来源：http://zvs.yuxming.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fkf.wangshuangyany.cn

[S42] C++：继承与虚函数
来源：http://xct.hcnkem.com

class B : public Base { public: void f() override {} };
来源：http://jnt.mhx1999.top

[S43] C++：智能指针
来源：http://hpr.jinyuanbaomall.cn

auto p = std::make_unique<int>(5);
来源：http://han.jiagoushi.top

[S44] C++：引用传参
来源：http://hgs.kuanghao11.cn

void inc(int &x) { ++x; }
来源：http://crn.kuanghao11.cn

[S45] C++：lambda
来源：http://udu.gogol.net.cn

auto add = [](int a, int b) { return a + b; };
来源：http://naj.epnwcf.com

[S46] C++：函数模板
来源：http://cpy.ppjwa.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ywx.aizwys.cn

[S47] C++：结构化绑定遍历
来源：http://hoj.dianchejie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bpl.nanxinkj.top

[S48] C++：逐行读文件
来源：http://kpd.shuidangran.top

std::ifstream in("a.txt");  std::string line;
来源：http://kju.zhijiandao.cn

while (std::getline(in, line)) { }
来源：http://duw.xuanzx.com

[S49] C++：写文件
来源：http://awv.bbcook.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nwh.cqqwz.cn

[S50] C++：格式化数字
来源：http://diz.bbcook.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ryl.aizwys.cn

[S51] C++：显式类型转换
来源：http://dca.sysykeji.top

static_cast<double>(a) / b
来源：http://xhn.52xcode.cn

[S52] C++：const 与 noexcept
来源：http://vzt.redwolf501.top

int size() const noexcept { return n_; }
来源：http://oec.aizwys.cn

[S53] C++：移动语义
来源：http://tfu.xingfuxueyuan.xyz

std::vector<int> w = std::move(v);
来源：http://ehs.kuanghao11.cn

[S54] C++：异常处理
来源：http://bzo.gzhubu.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://oba.tanke756.top

[S55] C++：结构化绑定
来源：http://pjw.0kj1m.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zgb.yuxming.cn

[S56] C++：optional
来源：http://vmu.zhoulong.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tgu.smart0.xyz

[S57] C++：编译期常量
来源：http://ijf.zhengqikj.top

constexpr int N = 10;
来源：http://eky.jianghu66.top

[S58] C++：命名空间
来源：http://nok.nanxuanxn.top

namespace ns { int f() { return 1; } }
来源：http://ltq.gotoacloud.top

[S59] C++：静态断言
来源：http://bkg.yj202588.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dhw.hcnkem.com

[S60] C++：遍历并删除元素
来源：http://swu.iojbl.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cwv.aizwys.cn

================================================================================
来源：http://lig.hfpthk.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://opl.bjfxy.top

================================================================================
来源：http://eso.havefunace.top

[T01] Kotlin：Hello World
来源：http://maq.svipenyu.cn

println("Hello")
来源：http://hmj.xingfuxueyuan.xyz

[T02] Kotlin：变量
来源：http://dii.jianghu66.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yal.hnqzz.top

[T03] Kotlin：字符串模板
来源：http://lbb.chenlongwang.top

"值: $b"
来源：http://fpx.fzhhl.top

[T04] Kotlin：空安全
来源：http://hta.sxryk.cn

val n: String? = null;  n?.length
来源：http://vox.yvedp.cn

[T05] Kotlin：when 表达式
来源：http://gyn.hywenlv.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://eis.aibaodan.cn

[T06] Kotlin：集合映射
来源：http://ojr.yfazqb.com

listOf(1, 2, 3).map { it * 2 }
来源：http://efa.tianlin.xyz

[T07] Kotlin：集合过滤
来源：http://qou.jinqigufen.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://jvf.zdbjq.cn

[T08] Kotlin：数据类
来源：http://lfg.zhixingplan.top

data class User(val name: String, val age: Int)
来源：http://lpm.bjfxy.top

[T09] Kotlin：扩展函数
来源：http://jif.ehwqpu.com

fun String.exclaim() = this + "!"
来源：http://pkp.nanxuanxn.top

[T10] Kotlin：默认参数
来源：http://qyx.redwolf501.top

fun greet(name: String = "World") = "Hi $name"
来源：http://tkq.zdqjudy.top

[T11] Kotlin：协程
来源：http://oxb.chenzaomai.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://awo.cqqwz.cn

[T12] Kotlin：解构声明
来源：http://rjn.aibaodan.cn

val (a, b) = Pair(1, 2)
来源：http://sju.sufxvd.cn

[T13] Kotlin：只读 Map
来源：http://hkh.sjlbkw.cn

val m = mapOf("a" to 1)
来源：http://kof.shanyushiyangtech.top

[T14] Kotlin：循环
来源：http://dfr.xuanzx.com

for (i in 1..10) println(i)
来源：http://jdr.zhengqikj.top

[T15] Kotlin：接口
来源：http://gzr.feifeiyinyue.top

interface Shape { fun area(): Double }
来源：http://mjv.haohaochexian.top

[T16] Swift：Hello World
来源：http://gfa.mhx1999.top

print("Hello")
来源：http://yvh.cdnleiting.top

[T17] Swift：变量与常量
来源：http://sec.aibaodan.cn

var a = 1;  let b = 2
来源：http://qsw.guowangkeji.top

[T18] Swift：字符串插值
来源：http://xea.cdnleiting.top

"值: \(b)"
来源：http://ypm.pycfn.com

[T19] Swift：可选绑定
来源：http://pou.gaohongyu789.top

if let n = opt { print(n) }
来源：http://zsu.kuanghao11.cn

[T20] Swift：数组操作
来源：http://iyc.havefunace.top

var a = [1, 2, 3];  a.append(4)
来源：http://eph.sysykeji.top

[T21] Swift：遍历
来源：http://gky.yueranfly.top

for x in a { print(x) }
来源：http://nzd.gaohongyu789.top

[T22] Swift：字典
来源：http://ipv.cashguo.top

var d = ["a": 1];  d["b"] = 2
来源：http://csd.xingfuxueyuan.xyz

[T23] Swift：函数
来源：http://tyq.svipenyu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xhq.yj20258.top

[T24] Swift：闭包
来源：http://lrv.9152youxi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qxa.zhaomingkeji.xyz

[T25] Swift：结构体
来源：http://asr.smart0.xyz

struct P { var x: Int }
来源：http://jcq.yonumen.top

[T26] Swift：类与重写
来源：http://twp.zhongyouzk.top

class A: Base { override func f() {} }
来源：http://dxc.mhx1999.top

[T27] Swift：错误处理
来源：http://xlv.mhx1999.top

do { try f() } catch { print(error) }
来源：http://qze.aibaodan.cn

[T28] Swift：枚举
来源：http://skl.mhx1999.top

enum Color { case red, green }
来源：http://bvn.fehbvm.com

[T29] Swift：guard 提前返回
来源：http://axg.pycfn.com

guard let x = opt else { return }
来源：http://nxo.havefunace.top

[T30] Swift：协议
来源：http://ylv.jlsjyb.cn

protocol Shape { func area() -> Double }
来源：http://boo.hammf.cn

[T31] Lua：Hello World
来源：http://pxe.shanyushiyangkeji.top

print("Hello")
来源：http://tuv.kuanghao11.cn

[T32] Lua：局部变量
来源：http://xda.xziqi.cn

local a = 1
来源：http://hwg.ydzc1.top

[T33] Lua：表（数组）
来源：http://abg.zhixingplan.top

local t = {1, 2, 3};  t[4] = 4
来源：http://aur.sufxvd.cn

[T34] Lua：遍历表
来源：http://szh.hywenlv.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://sca.ydzc1.top

[T35] Lua：字典表
来源：http://qgg.9152youxi.cn

local d = { a = 1 };  d.b = 2
来源：http://bnn.yuanzhike.top

[T36] Lua：函数
来源：http://voy.gaohongyu789.top

function add(a, b) return a + b end
来源：http://ecl.feifeiyinyue.top

[T37] Lua：字符串拼接
来源：http://epz.cdnleiting.top

"a" .. "b"
来源：http://yip.svipenyu.cn

[T38] Lua：条件
来源：http://rbc.yj202588.top

if x > 0 then print("正") end
来源：http://mbc.chenlongwang.top

[T39] Lua：模式匹配
来源：http://zps.wangdashe.top

string.find(s, "%d+")
来源：http://vko.shanyushiyangkeji.top

[T40] Lua：元表
来源：http://cxa.aibaodan.cn

setmetatable({}, { __index = base })
来源：http://zyp.yonumen.top

[T41] Perl：Hello World
来源：http://gay.shuidangran.top

print "Hello\n";
来源：http://xbu.wangshuangyany.cn

[T42] Perl：变量类型
来源：http://cqu.xuetiantiany.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pml.yuxming.cn

[T43] Perl：字符串插值
来源：http://sct.zycfv.cn

"值: $a"
来源：http://pbf.ydzc1.top

[T44] Perl：条件
来源：http://pdb.dianchejie.cn

if ($a > 0) { print "正"; }
来源：http://mem.feifeiyinyue.top

[T45] Perl：数组遍历
来源：http://vju.tian-w.cn

for my $x (@arr) { print $x; }
来源：http://eyt.zhoulong.xyz

[T46] Perl：哈希操作
来源：http://bmx.jinyuanbaomall.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jbx.jinqigfzy.top

[T47] Perl：正则捕获
来源：http://gnc.c1oappe.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://htg.jqgfzy.top

[T48] Perl：正则替换
来源：http://pwd.tian-w.cn

$s =~ s/old/new/g;
来源：http://eod.xingfuxueyuan.xyz

[T49] Perl：函数
来源：http://iti.cdnleiting.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cer.fktsv.cn

[T50] Perl：逐行读文件
来源：http://mgs.dashuyun.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ynd.xziqi.cn

while (my $line = <$fh>) { print $line; }
来源：http://zfu.xinyue.icu

[T51] Scala：Hello World
来源：http://mae.hesvh.cn

println("Hello")
来源：http://luk.hnxiangtu.top

[T52] Scala：变量
来源：http://kao.guowangkeji.top

val a = 1;  var b = 2
来源：http://mgt.fzhhl.top

[T53] Scala：字符串插值
来源：http://lpj.yangfankeji.com

s"值: $b"
来源：http://xyz.ehwqpu.com

[T54] Scala：集合映射
来源：http://mdh.jinghuilouyu.cn

List(1, 2, 3).map(_ * 2)
来源：http://bsf.cashguo.top

[T55] Scala：集合过滤
来源：http://spo.yuxming.cn

List(1, 2, 3).filter(_ > 1)
来源：http://div.yuxming.cn

[T56] Scala：样例类
来源：http://gsi.jiagoushi.top

case class User(name: String, age: Int)
来源：http://fok.yuxming.cn

[T57] Scala：模式匹配
来源：http://czk.c1oappe.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://blz.havefunace.top

[T58] Scala：函数定义
来源：http://ghr.cqqwz.cn

def add(a: Int, b: Int): Int = a + b
来源：http://xpr.feifeiyinyue.top

[T59] Scala：循环
来源：http://gbi.sjlbkw.cn

for (i <- 1 to 10) println(i)
来源：http://ndo.0kj1m.cn

[T60] Scala：折叠
来源：http://hnd.xinyue.icu

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fal.pengpengdd.cyou

================================================================================
来源：http://gis.wangshuangyany.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cbj.fktsv.cn

================================================================================
来源：http://inj.hammf.cn

[U01] Py：创建虚拟环境
来源：http://gkd.uphjek.com

python -m venv .venv && source .venv/bin/activate
来源：http://grr.aibaodan.cn

[U02] Py：导出 / 安装依赖
来源：http://bxu.yvedp.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cqn.fzhhl.top

[U03] Py：加载 .env 配置
来源：http://npj.wangdashe.top

from dotenv import load_dotenv; load_dotenv()
来源：http://bdt.jqgufenzy.top

[U04] Py：变量调试打印
来源：http://zjp.jinghuilouyu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bqy.hnqzz.top

[U05] Py：列表去重且保序
来源：http://sjf.yongpay.top

list(dict.fromkeys(arr))
来源：http://faz.chenzaomai.com

[U06] Py：合并两个字典
来源：http://jsw.zdqjudy.top

{**a, **b}
来源：http://fqz.aizwys.cn

[U07] Py：反转字典键值
来源：http://sja.yueranfly.top

{v: k for k, v in d.items()}
来源：http://vbv.dashuyun.cn

[U08] Py：展平二维列表
来源：http://vze.gotoacloud.top

[y for x in nested for y in x]
来源：http://nss.zhixingplan.top

[U09] Py：字典取最大值的键
来源：http://vur.xinyue.icu

max(d, key=d.get)
来源：http://yil.nanxinkj.top

[U10] Py：按值排序字典
来源：http://twl.guowangkeji.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ogq.ehwqpu.com

[U11] Py：生成器表达式
来源：http://sxw.chenjidiqi.icu

(x * 2 for x in arr)
来源：http://cai.ybcxt.top

[U12] Py：取出现最多的 3 个元素
来源：http://ect.xingfuxueyuan.xyz

Counter(arr).most_common(3)
来源：http://jrc.zhongyouzk.top

[U13] Py：固定长度队列
来源：http://yrd.zdbjq.cn

deque(maxlen=10)
来源：http://dtf.316326.xyz

[U14] Py：分组收集到列表
来源：http://gjv.xuetiantiany.cn

defaultdict(list)
来源：http://oqk.ctjpmb.com

[U15] Py：高精度计时
来源：http://xpx.52xcode.cn

t = time.perf_counter()
来源：http://qat.zhiwuduotai.top

[U16] Py：命令行参数解析
来源：http://bcu.cucudq.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gjr.52xcode.cn

[U17] Py：初始化日志
来源：http://myq.tian-w.cn

logging.basicConfig(level=logging.INFO)
来源：http://rti.gogol.net.cn

[U18] Py：预编译正则
来源：http://yld.zhiwuduotai.top

pat = re.compile(r"\d+")
来源：http://vxd.zdbjq.cn

[U19] Py：正则替换带回调
来源：http://emb.daria6918.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tvy.cheryme.top

[U20] Py：缓存函数结果
来源：http://dzg.guowangkeji.top

@functools.lru_cache(maxsize=None)
来源：http://mzb.52xcode.cn

[U21] Py：自定义上下文管理器
来源：http://xzx.zhaomingkeji.xyz

@contextlib.contextmanager
来源：http://itv.daria6918.cn

[U22] Py：矩阵转置
来源：http://ktn.aibaodan.cn

list(zip(*m))
来源：http://tel.iojbl.cn

[U23] Py：分块读取大文件
来源：http://adb.hcnkem.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://koa.yueranfly.top

[U24] Py：路径操作
来源：http://hxj.guannengcc.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ttf.wangdashe.top

[U25] Py：CSV 按字典读
来源：http://gyt.gogol.net.cn

csv.DictReader(f)
来源：http://ezd.uphjek.com

[U26] Py：并发下载
来源：http://dhl.meibo888.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://uxg.tarul.cn

[U27] Py：异步 HTTP
来源：http://ozr.mhx1999.top

aiohttp.ClientSession() 配合 async with
来源：http://omi.ybcxt.top

[U28] Py：类型别名
来源：http://xtf.hongshengwenyu.top

UserId = int
来源：http://hfs.yuxming.cn

[U29] Py：属性校验
来源：http://qvn.hnqzz.top

@property 与 @x.setter 配合
来源：http://zpa.ctjpmb.com

[U30] Py：数据类
来源：http://vhu.zhiwuduotai.top

@dataclass(slots=True)
来源：http://szr.sweek.top

[U31] Py：单测
来源：http://rqy.yfazqb.com

python -m pytest -q
来源：http://dxi.shzxlz.cn

[U32] Py：代码格式化
来源：http://gfd.jqgufenzy.top

ruff format . && ruff check --fix .
来源：http://inn.haohaochexian.top

[U33] Py：打包发布
来源：http://ujj.shzxlz.cn

python -m build  （依赖 pyproject.toml）
来源：http://iek.mhx1999.top

[U34] Py：判断编码
来源：http://ehf.shanyushiyangkeji.top

chardet.detect(raw)
来源：http://tpz.shanyushiyangtech.top

[U35] Py：发送邮件
来源：http://ucg.ivvv.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rsl.xylfe.cn

[U36] Py：定时任务
来源：http://eqb.nwbrower.top

schedule.every(10).minutes.do(job)
来源：http://wdi.c1oappe.top

[U37] Py：读写 Excel
来源：http://eal.hnqzz.top

pandas.read_excel / DataFrame.to_excel
来源：http://qcr.chenlongwang.top

[U38] Py：获取脚本所在目录
来源：http://crk.uphjek.com

Path(__file__).resolve().parent
来源：http://kqp.gzhubu.top


<!-- 参考信息 -->