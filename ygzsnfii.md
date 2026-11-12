代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://qem.birdmap.top

[S15] C：类型转换
来源：http://evz.316326.xyz

(double) a / b
来源：http://sjj.svipenyu.cn

[S16] C：位操作置位
来源：http://qfw.guowangkeji.top

x |= (1 << 3);
来源：http://pbs.yueranfly.top

[S17] C：安全拼接字符串
来源：http://rjo.daria6918.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mif.hnxiangtu.top

[S18] C：命令行参数
来源：http://rus.jinqigfzy.top

int main(int argc, char **argv)
来源：http://sec.hammf.cn

[S19] C：快速排序
来源：http://mao.hysaishi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jez.guannengcc.top

[S20] C：二分查找
来源：http://gtv.chenzaomai.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bem.cqqwz.cn

[S21] C：字符类别判断
来源：http://yxq.zhixingplan.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://iou.shanyushiyangkeji.top

[S22] C：字符串转数字
来源：http://smk.316326.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://alo.cucudq.cn

[S23] C：随机数
来源：http://jvp.cucudq.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fuc.feifeiyinyue.top

[S24] C：获取本地时间
来源：http://rhb.cdnleiting.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dwh.zhoulong.xyz

[S25] C：内存拷贝
来源：http://kqf.sweek.top

memcpy(dst, src, n);
来源：http://pzw.aibaodan.cn

[S26] C：内存清零
来源：http://qip.sweek.top

memset(a, 0, sizeof a);
来源：http://plk.fehbvm.com

[S27] C：定义常量
来源：http://vdz.guannengcc.top

const double PI = 3.14159;
来源：http://xxv.sweek.top

[S28] C：静态变量
来源：http://jzc.jianghu66.top

static int counter = 0;
来源：http://ojt.hysaishi.cn

[S29] C：变参函数
来源：http://jsq.shangyingyoupin.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://iyf.andypj.xyz

[S30] C：头文件保护
来源：http://otz.fengsongda.top

#ifndef X_H
来源：http://dpb.hongshengwenyu.top

#define X_H
来源：http://bud.fzhhl.top

#endif
来源：http://txy.svipenyu.cn

[S31] C++：Hello World
来源：http://zlv.chenlongwang.top

#include <iostream>
来源：http://gwa.quarkkingdee.top

int main() { std::cout << "Hello\n"; }
来源：http://ibw.iojbl.cn

[S32] C++：字符串
来源：http://irm.iojbl.cn

std::string s = "hi";  s += "!";
来源：http://ujr.gogol.net.cn

[S33] C++：vector 增删
来源：http://hqe.hesvh.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://aoo.shanyushiyangkeji.top

[S34] C++：遍历 vector
来源：http://gjc.316326.xyz

for (auto &x : v) { std::cout << x; }
来源：http://uja.tanke756.top

[S35] C++：map
来源：http://vgn.redwolf501.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ojn.jianghu66.top

[S36] C++：unordered_map
来源：http://qyo.bjfxy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mau.zhengqikj.top

[S37] C++：set
来源：http://wta.daxiang520.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xdy.pengpengdd.cyou

[S38] C++：排序
来源：http://gyg.xuetiantiany.cn

std::sort(v.begin(), v.end());
来源：http://jdc.dianchejie.cn

[S39] C++：自定义比较器排序
来源：http://tfm.cucudq.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xvj.zhaomingkeji.xyz

[S40] C++：查找元素
来源：http://fkr.xingfuxueyuan.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ojm.zhengqikj.top

[S41] C++：类与构造函数
来源：http://bci.zhiwuduotai.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hey.jinghuilouyu.cn

[S42] C++：继承与虚函数
来源：http://daq.jqgufenzy.top

class B : public Base { public: void f() override {} };
来源：http://aaq.cheryme.top

[S43] C++：智能指针
来源：http://uyj.tanke756.top

auto p = std::make_unique<int>(5);
来源：http://zjq.ehwqpu.com

[S44] C++：引用传参
来源：http://tec.xuanzx.com

void inc(int &x) { ++x; }
来源：http://ozd.xuanzx.com

[S45] C++：lambda
来源：http://gad.hywenlv.cn

auto add = [](int a, int b) { return a + b; };
来源：http://hru.cqqwz.cn

[S46] C++：函数模板
来源：http://wyj.ctjpmb.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://waw.0kj1m.cn

[S47] C++：结构化绑定遍历
来源：http://ojp.yanxiufei.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zov.chenlongwang.top

[S48] C++：逐行读文件
来源：http://jhe.fzhhl.top

std::ifstream in("a.txt");  std::string line;
来源：http://mdn.andypj.xyz

while (std::getline(in, line)) { }
来源：http://avn.jqgufenzy.top

[S49] C++：写文件
来源：http://pft.redwolf501.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://owb.ydjk.org.cn

[S50] C++：格式化数字
来源：http://ztx.yanxiufei.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kaz.zhixingplan.top

[S51] C++：显式类型转换
来源：http://dvt.fzhhl.top

static_cast<double>(a) / b
来源：http://sdi.yvedp.cn

[S52] C++：const 与 noexcept
来源：http://rbe.fzhhl.top

int size() const noexcept { return n_; }
来源：http://gxy.ydzc1.top

[S53] C++：移动语义
来源：http://krc.meibo888.top

std::vector<int> w = std::move(v);
来源：http://mrz.nanxinkj.top

[S54] C++：异常处理
来源：http://ikh.daxiang520.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nab.bjfxy.top

[S55] C++：结构化绑定
来源：http://per.zycfv.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://jlv.vehdjk.com

[S56] C++：optional
来源：http://rrv.hnxiangtu.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qid.ybcxt.top

[S57] C++：编译期常量
来源：http://oul.shangyingyoupin.top

constexpr int N = 10;
来源：http://rnu.gogol.net.cn

[S58] C++：命名空间
来源：http://rcc.pycfn.com

namespace ns { int f() { return 1; } }
来源：http://bvn.52xcode.cn

[S59] C++：静态断言
来源：http://muw.xinyue.icu

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qnl.kuanghao11.cn

[S60] C++：遍历并删除元素
来源：http://bhh.nanxinkj.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://meh.guannengcc.top

================================================================================
来源：http://dyk.zhijiandao.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vtr.redwolf501.top

================================================================================
来源：http://mmw.yj20258.top

[T01] Kotlin：Hello World
来源：http://wqr.dianchejie.cn

println("Hello")
来源：http://arw.zhengqikj.top

[T02] Kotlin：变量
来源：http://vpn.ybcxt.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qrt.wangdashe.top

[T03] Kotlin：字符串模板
来源：http://wqq.yj20258.top

"值: $b"
来源：http://xqz.hesvh.cn

[T04] Kotlin：空安全
来源：http://sol.haohaochexian.top

val n: String? = null;  n?.length
来源：http://wcf.cucudq.cn

[T05] Kotlin：when 表达式
来源：http://xzg.yangfankeji.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mby.smart0.xyz

[T06] Kotlin：集合映射
来源：http://ycp.aibaodan.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tiy.hfpthk.cn

[T07] Kotlin：集合过滤
来源：http://laa.sufxvd.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qvg.jinqigfzy.top

[T08] Kotlin：数据类
来源：http://mla.cucudq.cn

data class User(val name: String, val age: Int)
来源：http://pjw.hywenlv.cn

[T09] Kotlin：扩展函数
来源：http://rwj.yvedp.cn

fun String.exclaim() = this + "!"
来源：http://olg.chenlongwang.top

[T10] Kotlin：默认参数
来源：http://tud.zhijiandao.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://bgh.mhx1999.top

[T11] Kotlin：协程
来源：http://kwv.hongshengwenyu.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://pox.pengpengdd.cyou

[T12] Kotlin：解构声明
来源：http://qjx.zhijiandao.cn

val (a, b) = Pair(1, 2)
来源：http://ddi.hnxiangtu.top

[T13] Kotlin：只读 Map
来源：http://hob.hongshengwenyu.top

val m = mapOf("a" to 1)
来源：http://kva.9152youxi.cn

[T14] Kotlin：循环
来源：http://xja.sysykeji.top

for (i in 1..10) println(i)
来源：http://rvl.sufxvd.cn

[T15] Kotlin：接口
来源：http://emx.yangfankeji.com

interface Shape { fun area(): Double }
来源：http://psq.nanxuanxn.top

[T16] Swift：Hello World
来源：http://oga.pycfn.com

print("Hello")
来源：http://ciu.hnqzz.top

[T17] Swift：变量与常量
来源：http://aqz.zhixingplan.top

var a = 1;  let b = 2
来源：http://djj.iojbl.cn

[T18] Swift：字符串插值
来源：http://ymk.chenzaomai.com

"值: \(b)"
来源：http://yro.svipenyu.cn

[T19] Swift：可选绑定
来源：http://qwo.yueranfly.top

if let n = opt { print(n) }
来源：http://tnb.ivvv.top

[T20] Swift：数组操作
来源：http://igq.jqgfzy.top

var a = [1, 2, 3];  a.append(4)
来源：http://uey.yj202588.top

[T21] Swift：遍历
来源：http://kjc.vqdsnc.cn

for x in a { print(x) }
来源：http://kxz.316326.xyz

[T22] Swift：字典
来源：http://gik.fanxiaobao.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://txq.fzhhl.top

[T23] Swift：函数
来源：http://ncu.jianghu66.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gzo.uphjek.com

[T24] Swift：闭包
来源：http://roi.yongpay.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://tsc.shangyingyoupin.top

[T25] Swift：结构体
来源：http://eqv.pengpengdd.cyou

struct P { var x: Int }
来源：http://roa.52xcode.cn

[T26] Swift：类与重写
来源：http://wlu.kuanghao11.cn

class A: Base { override func f() {} }
来源：http://gvl.chenlongwang.top

[T27] Swift：错误处理
来源：http://ily.jyoumei.cn

do { try f() } catch { print(error) }
来源：http://xxa.xuanzx.com

[T28] Swift：枚举
来源：http://dos.fktsv.cn

enum Color { case red, green }
来源：http://jgv.yongpay.top

[T29] Swift：guard 提前返回
来源：http://tbz.yfazqb.com

guard let x = opt else { return }
来源：http://dqg.hongshengwenyu.top

[T30] Swift：协议
来源：http://dez.hcnkem.com

protocol Shape { func area() -> Double }
来源：http://lug.fengsongda.top

[T31] Lua：Hello World
来源：http://ckk.nwbrower.top

print("Hello")
来源：http://jul.jyoumei.cn

[T32] Lua：局部变量
来源：http://xgu.xinyue.icu

local a = 1
来源：http://ioa.cheryme.top

[T33] Lua：表（数组）
来源：http://wof.316326.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://cbg.cqqwz.cn

[T34] Lua：遍历表
来源：http://onk.ppjwa.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://agv.shzxlz.cn

[T35] Lua：字典表
来源：http://mrx.gogol.net.cn

local d = { a = 1 };  d.b = 2
来源：http://bir.pengpengdd.cyou

[T36] Lua：函数
来源：http://aob.jinghuilouyu.cn

function add(a, b) return a + b end
来源：http://vcn.xuetiantiany.cn

[T37] Lua：字符串拼接
来源：http://tkt.aizwys.cn

"a" .. "b"
来源：http://dxn.guannengcc.top

[T38] Lua：条件
来源：http://cvi.daria6918.cn

if x > 0 then print("正") end
来源：http://ebg.0kj1m.cn

[T39] Lua：模式匹配
来源：http://vlv.meibo888.top

string.find(s, "%d+")
来源：http://oxk.aizwys.cn

[T40] Lua：元表
来源：http://vib.hammf.cn

setmetatable({}, { __index = base })
来源：http://jjp.hnqzz.top

[T41] Perl：Hello World
来源：http://qbq.zdqjudy.top

print "Hello\n";
来源：http://iiz.hfpthk.cn

[T42] Perl：变量类型
来源：http://zsg.9152youxi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://boy.nwbrower.top

[T43] Perl：字符串插值
来源：http://ids.gaohongyu789.top

"值: $a"
来源：http://krd.jqgfzy.top

[T44] Perl：条件
来源：http://vfi.cdnleiting.top

if ($a > 0) { print "正"; }
来源：http://ojf.hywenlv.cn

[T45] Perl：数组遍历
来源：http://xhq.hywenlv.cn

for my $x (@arr) { print $x; }
来源：http://cpy.shanyushiyangtech.top

[T46] Perl：哈希操作
来源：http://khi.tianlin.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nqy.aibaodan.cn

[T47] Perl：正则捕获
来源：http://euq.smart0.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://pzd.jinqigufen.top

[T48] Perl：正则替换
来源：http://lyp.jyoumei.cn

$s =~ s/old/new/g;
来源：http://quq.jianghu66.top

[T49] Perl：函数
来源：http://wnq.ydzc1.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gtt.shanyushiyangtech.top

[T50] Perl：逐行读文件
来源：http://rkx.gzhubu.top

open my $fh, "<", "a.txt" or die $!;
来源：http://zux.0kj1m.cn

while (my $line = <$fh>) { print $line; }
来源：http://tve.jqgfzy.top

[T51] Scala：Hello World
来源：http://acq.zhaomingkeji.xyz

println("Hello")
来源：http://fsl.havefunace.top

[T52] Scala：变量
来源：http://qil.cdnleiting.top

val a = 1;  var b = 2
来源：http://wdm.hcnkem.com

[T53] Scala：字符串插值
来源：http://eid.9152youxi.cn

s"值: $b"
来源：http://flz.hesvh.cn

[T54] Scala：集合映射
来源：http://ycx.aibaodan.cn

List(1, 2, 3).map(_ * 2)
来源：http://fzb.aizwys.cn

[T55] Scala：集合过滤
来源：http://gvi.xuanzx.com

List(1, 2, 3).filter(_ > 1)
来源：http://erg.shanyushiyangkeji.top

[T56] Scala：样例类
来源：http://kea.fanxiaobao.xyz

case class User(name: String, age: Int)
来源：http://wkl.daxiang520.top

[T57] Scala：模式匹配
来源：http://xhx.gaohongyu789.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://rgl.havefunace.top

[T58] Scala：函数定义
来源：http://jfk.vehdjk.com

def add(a: Int, b: Int): Int = a + b
来源：http://lim.hnqzz.top

[T59] Scala：循环
来源：http://vmb.zhiwuduotai.top

for (i <- 1 to 10) println(i)
来源：http://bfu.hnqzz.top

[T60] Scala：折叠
来源：http://wws.shangyingyoupin.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://uwl.shuidangran.top

================================================================================
来源：http://rks.fzhhl.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bdb.xinyue.icu

================================================================================
来源：http://cea.jinghuilouyu.cn

[U01] Py：创建虚拟环境
来源：http://dmz.pycfn.com

python -m venv .venv && source .venv/bin/activate
来源：http://fxj.fzhhl.top

[U02] Py：导出 / 安装依赖
来源：http://tlr.c1oappe.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vfu.c1oappe.top

[U03] Py：加载 .env 配置
来源：http://yyg.hesvh.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://thp.hysaishi.cn

[U04] Py：变量调试打印
来源：http://kds.guowangkeji.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ctk.haohaochexian.top

[U05] Py：列表去重且保序
来源：http://aoi.fanxiaobao.xyz

list(dict.fromkeys(arr))
来源：http://tla.wangdashe.top

[U06] Py：合并两个字典
来源：http://snu.bbcook.cn

{**a, **b}
来源：http://cyd.aizwys.cn

[U07] Py：反转字典键值
来源：http://exk.ybcxt.top

{v: k for k, v in d.items()}
来源：http://xjt.xuanzx.com

[U08] Py：展平二维列表
来源：http://zya.cashguo.top

[y for x in nested for y in x]
来源：http://jpo.hywenlv.cn

[U09] Py：字典取最大值的键
来源：http://hil.0kj1m.cn

max(d, key=d.get)
来源：http://pof.ywan-chungtsiang.top

[U10] Py：按值排序字典
来源：http://cvg.iojbl.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jwk.shanyushiyangtech.top

[U11] Py：生成器表达式
来源：http://cla.dashuyun.cn

(x * 2 for x in arr)
来源：http://pjq.dashuyun.cn

[U12] Py：取出现最多的 3 个元素
来源：http://fbx.yj20258888.top

Counter(arr).most_common(3)
来源：http://wbs.vqdsnc.cn

[U13] Py：固定长度队列
来源：http://evq.cqqwz.cn

deque(maxlen=10)
来源：http://yzs.wangdashe.top

[U14] Py：分组收集到列表
来源：http://jef.ctjpmb.com

defaultdict(list)
来源：http://yoi.ywan-chungtsiang.top

[U15] Py：高精度计时
来源：http://xdq.gotoacloud.top

t = time.perf_counter()
来源：http://dxg.xingfuxueyuan.xyz

[U16] Py：命令行参数解析
来源：http://rct.zdqjudy.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vbo.bbcook.cn

[U17] Py：初始化日志
来源：http://xkc.zdbjq.cn

logging.basicConfig(level=logging.INFO)
来源：http://kjq.yonumen.top

[U18] Py：预编译正则
来源：http://bch.yuxming.cn

pat = re.compile(r"\d+")
来源：http://jjy.nwbrower.top

[U19] Py：正则替换带回调
来源：http://tga.yueranfly.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ixy.zdqjudy.top

[U20] Py：缓存函数结果
来源：http://lcg.sxryk.cn

@functools.lru_cache(maxsize=None)
来源：http://hzm.quarkkingdee.top

[U21] Py：自定义上下文管理器
来源：http://hsu.cdnleiting.top

@contextlib.contextmanager
来源：http://utq.shzxlz.cn

[U22] Py：矩阵转置
来源：http://scn.vehdjk.com

list(zip(*m))
来源：http://zqn.andypj.xyz

[U23] Py：分块读取大文件
来源：http://glj.yvedp.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zdz.guannengcc.top

[U24] Py：路径操作
来源：http://eaq.wangdashe.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://kjt.ywan-chungtsiang.top

[U25] Py：CSV 按字典读
来源：http://wrs.nanxinkj.top

csv.DictReader(f)
来源：http://yuf.jyoumei.cn

[U26] Py：并发下载
来源：http://pdw.tanke756.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xvu.jinghuilouyu.cn

[U27] Py：异步 HTTP
来源：http://kcz.zhaomingkeji.xyz

aiohttp.ClientSession() 配合 async with
来源：http://ceq.guowangkeji.top

[U28] Py：类型别名
来源：http://gou.hywenlv.cn

UserId = int
来源：http://ski.fehbvm.com

[U29] Py：属性校验
来源：http://lxg.kuanghao11.cn

@property 与 @x.setter 配合
来源：http://wan.zhijiandao.cn

[U30] Py：数据类
来源：http://obo.epnwcf.com

@dataclass(slots=True)
来源：http://pbz.yongpay.top

[U31] Py：单测
来源：http://jbf.jiagoushi.top

python -m pytest -q
来源：http://gfy.jiagoushi.top

[U32] Py：代码格式化
来源：http://dge.sysykeji.top

ruff format . && ruff check --fix .
来源：http://kvo.hammf.cn

[U33] Py：打包发布
来源：http://stc.hcnkem.com

python -m build  （依赖 pyproject.toml）
来源：http://uki.jyoumei.cn

[U34] Py：判断编码
来源：http://bcj.yangfankeji.com

chardet.detect(raw)
来源：http://dam.feifeiyinyue.top

[U35] Py：发送邮件
来源：http://kqc.ctjpmb.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://var.cucudq.cn

[U36] Py：定时任务
来源：http://ghg.yvedp.cn

schedule.every(10).minutes.do(job)
来源：http://uwt.shanyushiyangkeji.top

[U37] Py：读写 Excel
来源：http://zwu.jiagoushi.top

pandas.read_excel / DataFrame.to_excel
来源：http://wqk.yonumen.top

[U38] Py：获取脚本所在目录
来源：http://bxz.hfpthk.cn

Path(__file__).resolve().parent
来源：http://oho.xziqi.cn


<!-- 参考信息 -->