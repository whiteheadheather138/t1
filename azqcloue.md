代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://anm.vqdsnc.cn

[S15] C：类型转换
来源：http://znl.cheryme.top

(double) a / b
来源：http://dwn.jianghu66.top

[S16] C：位操作置位
来源：http://xod.dashuyun.cn

x |= (1 << 3);
来源：http://rjj.bbcook.cn

[S17] C：安全拼接字符串
来源：http://qiv.zhongyouzk.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://arf.andypj.xyz

[S18] C：命令行参数
来源：http://eud.xinyue.icu

int main(int argc, char **argv)
来源：http://cgd.uphjek.com

[S19] C：快速排序
来源：http://arx.chenzaomai.com

qsort(a, n, sizeof(int), cmp);
来源：http://ivw.zycfv.cn

[S20] C：二分查找
来源：http://soc.ctjpmb.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sec.cucudq.cn

[S21] C：字符类别判断
来源：http://dhe.gogol.net.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://exv.sweek.top

[S22] C：字符串转数字
来源：http://iuu.andypj.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://kym.xziqi.cn

[S23] C：随机数
来源：http://vie.cheryme.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ons.ywan-chungtsiang.top

[S24] C：获取本地时间
来源：http://hal.0kj1m.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://knp.yvedp.cn

[S25] C：内存拷贝
来源：http://vry.jyoumei.cn

memcpy(dst, src, n);
来源：http://xuy.fzhhl.top

[S26] C：内存清零
来源：http://pkk.ydjk.org.cn

memset(a, 0, sizeof a);
来源：http://yno.hfpthk.cn

[S27] C：定义常量
来源：http://wyh.jinqigufen.top

const double PI = 3.14159;
来源：http://sgi.zhengqikj.top

[S28] C：静态变量
来源：http://bwh.jiagoushi.top

static int counter = 0;
来源：http://mxb.jinghuilouyu.cn

[S29] C：变参函数
来源：http://ihk.dianchejie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://eaj.hcnkem.com

[S30] C：头文件保护
来源：http://oyt.jyoumei.cn

#ifndef X_H
来源：http://oud.dianchejie.cn

#define X_H
来源：http://anw.quarkkingdee.top

#endif
来源：http://bif.jqgfzy.top

[S31] C++：Hello World
来源：http://mwy.meibo888.top

#include <iostream>
来源：http://ybh.sysykeji.top

int main() { std::cout << "Hello\n"; }
来源：http://nzs.tianlin.xyz

[S32] C++：字符串
来源：http://iqp.snrcjt.cn

std::string s = "hi";  s += "!";
来源：http://thu.zhiwuduotai.top

[S33] C++：vector 增删
来源：http://hxi.jinqigufen.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qvk.zhaomingkeji.xyz

[S34] C++：遍历 vector
来源：http://fvp.yfazqb.com

for (auto &x : v) { std::cout << x; }
来源：http://gsn.wangdashe.top

[S35] C++：map
来源：http://jhe.gzhubu.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://plj.daxiang520.top

[S36] C++：unordered_map
来源：http://emk.kuanghao11.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rvu.bjfxy.top

[S37] C++：set
来源：http://drc.tian-w.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wik.nanxinkj.top

[S38] C++：排序
来源：http://leb.andypj.xyz

std::sort(v.begin(), v.end());
来源：http://yha.yanxiufei.cn

[S39] C++：自定义比较器排序
来源：http://igy.jianghu66.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xgb.tian-w.cn

[S40] C++：查找元素
来源：http://ynv.9152youxi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cmc.ydzc1.top

[S41] C++：类与构造函数
来源：http://xhz.bbcook.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://thh.cdnleiting.top

[S42] C++：继承与虚函数
来源：http://buj.chenjidiqi.icu

class B : public Base { public: void f() override {} };
来源：http://qzi.xuanzx.com

[S43] C++：智能指针
来源：http://dsp.shanyushiyangtech.top

auto p = std::make_unique<int>(5);
来源：http://eof.xziqi.cn

[S44] C++：引用传参
来源：http://hlw.daria6918.cn

void inc(int &x) { ++x; }
来源：http://pco.tian-w.cn

[S45] C++：lambda
来源：http://bnb.jiagoushi.top

auto add = [](int a, int b) { return a + b; };
来源：http://rif.gaohongyu789.top

[S46] C++：函数模板
来源：http://fwn.shuidangran.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wgs.fengsongda.top

[S47] C++：结构化绑定遍历
来源：http://srb.ppjwa.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xsf.andypj.xyz

[S48] C++：逐行读文件
来源：http://osp.hysaishi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gdt.smart0.xyz

while (std::getline(in, line)) { }
来源：http://luh.c1oappe.top

[S49] C++：写文件
来源：http://llg.haohaochexian.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bga.chenjidiqi.icu

[S50] C++：格式化数字
来源：http://gkl.fzhhl.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zri.ydzc1.top

[S51] C++：显式类型转换
来源：http://uev.gotoacloud.top

static_cast<double>(a) / b
来源：http://zps.wangshuangyany.cn

[S52] C++：const 与 noexcept
来源：http://psv.jyoumei.cn

int size() const noexcept { return n_; }
来源：http://gwm.zdqjudy.top

[S53] C++：移动语义
来源：http://xul.jiagoushi.top

std::vector<int> w = std::move(v);
来源：http://wuw.cdnleiting.top

[S54] C++：异常处理
来源：http://hzs.dianchejie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jly.hcnkem.com

[S55] C++：结构化绑定
来源：http://upw.yj202588.top

auto [a, b] = std::make_pair(1, 2);
来源：http://hzo.sufxvd.cn

[S56] C++：optional
来源：http://nqi.shanyushiyangkeji.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://odc.jqgfzy.top

[S57] C++：编译期常量
来源：http://pwf.hammf.cn

constexpr int N = 10;
来源：http://jte.xuetiantiany.cn

[S58] C++：命名空间
来源：http://xng.xinyue.icu

namespace ns { int f() { return 1; } }
来源：http://niy.yj20258.top

[S59] C++：静态断言
来源：http://wki.xingfuxueyuan.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pgu.hcnkem.com

[S60] C++：遍历并删除元素
来源：http://xdo.ehwqpu.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rdh.gogol.net.cn

================================================================================
来源：http://fwf.epnwcf.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://sac.fengsongda.top

================================================================================
来源：http://csf.jianghu66.top

[T01] Kotlin：Hello World
来源：http://dvr.ydzc1.top

println("Hello")
来源：http://sil.hnqzz.top

[T02] Kotlin：变量
来源：http://lng.tarul.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hmq.fengsongda.top

[T03] Kotlin：字符串模板
来源：http://dsn.chenlongwang.top

"值: $b"
来源：http://xow.hywenlv.cn

[T04] Kotlin：空安全
来源：http://rdw.fanxiaobao.xyz

val n: String? = null;  n?.length
来源：http://wtj.pengpengdd.cyou

[T05] Kotlin：when 表达式
来源：http://fko.yonumen.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://idn.chenlongwang.top

[T06] Kotlin：集合映射
来源：http://wwm.jyoumei.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tfu.smart0.xyz

[T07] Kotlin：集合过滤
来源：http://nmy.jqgufenzy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://wnp.shzxlz.cn

[T08] Kotlin：数据类
来源：http://sif.zhijiandao.cn

data class User(val name: String, val age: Int)
来源：http://ldk.shzxlz.cn

[T09] Kotlin：扩展函数
来源：http://rsp.shanyushiyangkeji.top

fun String.exclaim() = this + "!"
来源：http://gcw.fzhhl.top

[T10] Kotlin：默认参数
来源：http://tlm.hysaishi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://krf.jinyuanbaomall.cn

[T11] Kotlin：协程
来源：http://yvv.vqdsnc.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://hyn.yonumen.top

[T12] Kotlin：解构声明
来源：http://lsh.birdmap.top

val (a, b) = Pair(1, 2)
来源：http://arj.shzxlz.cn

[T13] Kotlin：只读 Map
来源：http://ihv.ydzc1.top

val m = mapOf("a" to 1)
来源：http://fra.yuanzhike.top

[T14] Kotlin：循环
来源：http://ush.yangfankeji.com

for (i in 1..10) println(i)
来源：http://tzs.zhijiandao.cn

[T15] Kotlin：接口
来源：http://ybj.ppjwa.cn

interface Shape { fun area(): Double }
来源：http://jdh.svipenyu.cn

[T16] Swift：Hello World
来源：http://dky.iojbl.cn

print("Hello")
来源：http://ssb.zdqjudy.top

[T17] Swift：变量与常量
来源：http://hfh.iojbl.cn

var a = 1;  let b = 2
来源：http://rqa.xuetiantiany.cn

[T18] Swift：字符串插值
来源：http://kmu.zhoulong.xyz

"值: \(b)"
来源：http://yty.hesvh.cn

[T19] Swift：可选绑定
来源：http://sqg.ctjpmb.com

if let n = opt { print(n) }
来源：http://vwp.zdbjq.cn

[T20] Swift：数组操作
来源：http://cmk.svipenyu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://umf.jinqigufen.top

[T21] Swift：遍历
来源：http://pue.zhiwuduotai.top

for x in a { print(x) }
来源：http://hju.xuetiantiany.cn

[T22] Swift：字典
来源：http://tjl.daxiang520.top

var d = ["a": 1];  d["b"] = 2
来源：http://mlk.hfpthk.cn

[T23] Swift：函数
来源：http://agg.dianchejie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hqb.0kj1m.cn

[T24] Swift：闭包
来源：http://zjb.zhixingplan.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://mlt.yueranfly.top

[T25] Swift：结构体
来源：http://hix.shanyushiyangkeji.top

struct P { var x: Int }
来源：http://ium.hongshengwenyu.top

[T26] Swift：类与重写
来源：http://vcp.shzxlz.cn

class A: Base { override func f() {} }
来源：http://nqu.fzhhl.top

[T27] Swift：错误处理
来源：http://rek.yfazqb.com

do { try f() } catch { print(error) }
来源：http://vns.fehbvm.com

[T28] Swift：枚举
来源：http://jgg.52xcode.cn

enum Color { case red, green }
来源：http://kzw.guannengcc.top

[T29] Swift：guard 提前返回
来源：http://wrl.quarkkingdee.top

guard let x = opt else { return }
来源：http://wyp.mhx1999.top

[T30] Swift：协议
来源：http://caj.tanke756.top

protocol Shape { func area() -> Double }
来源：http://stv.fehbvm.com

[T31] Lua：Hello World
来源：http://wzy.jqgufenzy.top

print("Hello")
来源：http://alo.yuanzhike.top

[T32] Lua：局部变量
来源：http://sue.9152youxi.cn

local a = 1
来源：http://ani.bbcook.cn

[T33] Lua：表（数组）
来源：http://xdu.aibaodan.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://tau.yueranfly.top

[T34] Lua：遍历表
来源：http://ehd.vqdsnc.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://myx.pycfn.com

[T35] Lua：字典表
来源：http://jxz.fengsongda.top

local d = { a = 1 };  d.b = 2
来源：http://iij.meibo888.top

[T36] Lua：函数
来源：http://sgz.haohaochexian.top

function add(a, b) return a + b end
来源：http://doh.ydzc1.top

[T37] Lua：字符串拼接
来源：http://ygw.cucudq.cn

"a" .. "b"
来源：http://yfv.chenzaomai.com

[T38] Lua：条件
来源：http://jtb.sjlbkw.cn

if x > 0 then print("正") end
来源：http://dwl.uphjek.com

[T39] Lua：模式匹配
来源：http://imw.hammf.cn

string.find(s, "%d+")
来源：http://yld.sweek.top

[T40] Lua：元表
来源：http://oxk.jinghuilouyu.cn

setmetatable({}, { __index = base })
来源：http://ida.smart0.xyz

[T41] Perl：Hello World
来源：http://lii.tanke756.top

print "Hello\n";
来源：http://ygf.hongshengwenyu.top

[T42] Perl：变量类型
来源：http://kac.fzhhl.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ujg.meibo888.top

[T43] Perl：字符串插值
来源：http://xap.zycfv.cn

"值: $a"
来源：http://toh.fktsv.cn

[T44] Perl：条件
来源：http://pon.gotoacloud.top

if ($a > 0) { print "正"; }
来源：http://mwq.52xcode.cn

[T45] Perl：数组遍历
来源：http://jxl.yj20258.top

for my $x (@arr) { print $x; }
来源：http://mfa.zycfv.cn

[T46] Perl：哈希操作
来源：http://uzj.hfpthk.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zkq.9152youxi.cn

[T47] Perl：正则捕获
来源：http://xqw.wangshuangyany.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://mpr.guannengcc.top

[T48] Perl：正则替换
来源：http://gyf.zdqjudy.top

$s =~ s/old/new/g;
来源：http://rqd.kuanghao11.cn

[T49] Perl：函数
来源：http://sdi.shanyushiyangkeji.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rhz.zycfv.cn

[T50] Perl：逐行读文件
来源：http://hsl.pengpengdd.cyou

open my $fh, "<", "a.txt" or die $!;
来源：http://aqy.xingfuxueyuan.xyz

while (my $line = <$fh>) { print $line; }
来源：http://ywo.kuanghao11.cn

[T51] Scala：Hello World
来源：http://ghd.shzxlz.cn

println("Hello")
来源：http://sjs.sjlbkw.cn

[T52] Scala：变量
来源：http://typ.gogol.net.cn

val a = 1;  var b = 2
来源：http://vmh.tanke756.top

[T53] Scala：字符串插值
来源：http://shi.tian-w.cn

s"值: $b"
来源：http://xfw.yonumen.top

[T54] Scala：集合映射
来源：http://gny.nanxinkj.top

List(1, 2, 3).map(_ * 2)
来源：http://boi.meibo888.top

[T55] Scala：集合过滤
来源：http://vep.feifeiyinyue.top

List(1, 2, 3).filter(_ > 1)
来源：http://ind.haohaochexian.top

[T56] Scala：样例类
来源：http://cdf.tanke756.top

case class User(name: String, age: Int)
来源：http://vny.shanyushiyangkeji.top

[T57] Scala：模式匹配
来源：http://lsd.aizwys.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://xih.uphjek.com

[T58] Scala：函数定义
来源：http://ftm.316326.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://emc.wangdashe.top

[T59] Scala：循环
来源：http://rou.haohaochexian.top

for (i <- 1 to 10) println(i)
来源：http://olp.zhengqikj.top

[T60] Scala：折叠
来源：http://zdl.tanke756.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bkk.tianlin.xyz

================================================================================
来源：http://dqh.daria6918.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mgz.xylfe.cn

================================================================================
来源：http://stx.ehwqpu.com

[U01] Py：创建虚拟环境
来源：http://gfo.jinqigufen.top

python -m venv .venv && source .venv/bin/activate
来源：http://nrm.hesvh.cn

[U02] Py：导出 / 安装依赖
来源：http://jpn.yuanzhike.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://upt.zdqjudy.top

[U03] Py：加载 .env 配置
来源：http://ken.pengpengdd.cyou

from dotenv import load_dotenv; load_dotenv()
来源：http://qim.mhx1999.top

[U04] Py：变量调试打印
来源：http://agb.havefunace.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ksl.hnxiangtu.top

[U05] Py：列表去重且保序
来源：http://mnc.hnxiangtu.top

list(dict.fromkeys(arr))
来源：http://sak.jyoumei.cn

[U06] Py：合并两个字典
来源：http://xwd.birdmap.top

{**a, **b}
来源：http://ygv.52xcode.cn

[U07] Py：反转字典键值
来源：http://pxh.yfazqb.com

{v: k for k, v in d.items()}
来源：http://thr.birdmap.top

[U08] Py：展平二维列表
来源：http://ptk.316326.xyz

[y for x in nested for y in x]
来源：http://ngv.ydjk.org.cn

[U09] Py：字典取最大值的键
来源：http://ism.havefunace.top

max(d, key=d.get)
来源：http://cwz.hesvh.cn

[U10] Py：按值排序字典
来源：http://lyt.daxiang520.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dza.jqgufenzy.top

[U11] Py：生成器表达式
来源：http://nfa.dashuyun.cn

(x * 2 for x in arr)
来源：http://sne.ywan-chungtsiang.top

[U12] Py：取出现最多的 3 个元素
来源：http://jyy.yongpay.top

Counter(arr).most_common(3)
来源：http://stt.dianchejie.cn

[U13] Py：固定长度队列
来源：http://byb.hfpthk.cn

deque(maxlen=10)
来源：http://tcu.zycfv.cn

[U14] Py：分组收集到列表
来源：http://yev.gogol.net.cn

defaultdict(list)
来源：http://kxa.zhiwuduotai.top

[U15] Py：高精度计时
来源：http://jra.tanke756.top

t = time.perf_counter()
来源：http://rxy.gzhubu.top

[U16] Py：命令行参数解析
来源：http://jrt.hnqzz.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mnd.kuanghao11.cn

[U17] Py：初始化日志
来源：http://mfu.meibo888.top

logging.basicConfig(level=logging.INFO)
来源：http://dkz.xuanzx.com

[U18] Py：预编译正则
来源：http://bmc.yangfankeji.com

pat = re.compile(r"\d+")
来源：http://bup.meibo888.top

[U19] Py：正则替换带回调
来源：http://aig.ehwqpu.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://uqb.shuidangran.top

[U20] Py：缓存函数结果
来源：http://apn.52xcode.cn

@functools.lru_cache(maxsize=None)
来源：http://yyt.vehdjk.com

[U21] Py：自定义上下文管理器
来源：http://xvv.xylfe.cn

@contextlib.contextmanager
来源：http://wdj.havefunace.top

[U22] Py：矩阵转置
来源：http://enj.ydjk.org.cn

list(zip(*m))
来源：http://igo.svipenyu.cn

[U23] Py：分块读取大文件
来源：http://kxl.xuetiantiany.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://iay.guannengcc.top

[U24] Py：路径操作
来源：http://opi.ppjwa.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ttz.smart0.xyz

[U25] Py：CSV 按字典读
来源：http://jfj.zdbjq.cn

csv.DictReader(f)
来源：http://syg.wangshuangyany.cn

[U26] Py：并发下载
来源：http://zxb.fehbvm.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://eor.ctjpmb.com

[U27] Py：异步 HTTP
来源：http://kok.xuanzx.com

aiohttp.ClientSession() 配合 async with
来源：http://bol.cucudq.cn

[U28] Py：类型别名
来源：http://gbs.yj20258.top

UserId = int
来源：http://wab.fktsv.cn

[U29] Py：属性校验
来源：http://zei.hywenlv.cn

@property 与 @x.setter 配合
来源：http://oaq.52xcode.cn

[U30] Py：数据类
来源：http://fvp.havefunace.top

@dataclass(slots=True)
来源：http://vlz.hongshengwenyu.top

[U31] Py：单测
来源：http://rjk.epnwcf.com

python -m pytest -q
来源：http://yrz.hnxiangtu.top

[U32] Py：代码格式化
来源：http://bpo.yj202588.top

ruff format . && ruff check --fix .
来源：http://ibd.zhengqikj.top

[U33] Py：打包发布
来源：http://tes.tanke756.top

python -m build  （依赖 pyproject.toml）
来源：http://uoh.yvedp.cn

[U34] Py：判断编码
来源：http://aey.zhoulong.xyz

chardet.detect(raw)
来源：http://mjw.fzhhl.top

[U35] Py：发送邮件
来源：http://pyg.epnwcf.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://uzr.birdmap.top

[U36] Py：定时任务
来源：http://xdf.yongpay.top

schedule.every(10).minutes.do(job)
来源：http://tys.xingfuxueyuan.xyz

[U37] Py：读写 Excel
来源：http://egt.jinqigufen.top

pandas.read_excel / DataFrame.to_excel
来源：http://bbe.tian-w.cn

[U38] Py：获取脚本所在目录
来源：http://aan.ehwqpu.com

Path(__file__).resolve().parent
来源：http://env.feifeiyinyue.top


<!-- 参考信息 -->