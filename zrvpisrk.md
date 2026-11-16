代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://far.xziqi.cn

[S21] C：字符类别判断
来源：http://yjk.cqqwz.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mru.hysaishi.cn

[S22] C：字符串转数字
来源：http://dsk.svipenyu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://bvb.zhijiandao.cn

[S23] C：随机数
来源：http://mui.bjfxy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://eso.xuetiantiany.cn

[S24] C：获取本地时间
来源：http://xtl.jinyuanbaomall.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lan.sxryk.cn

[S25] C：内存拷贝
来源：http://eov.bjfxy.top

memcpy(dst, src, n);
来源：http://eyl.nanxuanxn.top

[S26] C：内存清零
来源：http://zzr.0kj1m.cn

memset(a, 0, sizeof a);
来源：http://dlg.vehdjk.com

[S27] C：定义常量
来源：http://qah.nwbrower.top

const double PI = 3.14159;
来源：http://wrj.jyoumei.cn

[S28] C：静态变量
来源：http://izc.tarul.cn

static int counter = 0;
来源：http://sru.svipenyu.cn

[S29] C：变参函数
来源：http://uec.yj202588.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jay.aizwys.cn

[S30] C：头文件保护
来源：http://jcp.dianchejie.cn

#ifndef X_H
来源：http://vlm.tianlin.xyz

#define X_H
来源：http://qzs.fanxiaobao.xyz

#endif
来源：http://pbm.pengpengdd.cyou

[S31] C++：Hello World
来源：http://lvl.aizwys.cn

#include <iostream>
来源：http://pcz.zycfv.cn

int main() { std::cout << "Hello\n"; }
来源：http://eyv.aizwys.cn

[S32] C++：字符串
来源：http://noa.fengsongda.top

std::string s = "hi";  s += "!";
来源：http://vzk.hongshengwenyu.top

[S33] C++：vector 增删
来源：http://ubg.yanxiufei.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ybm.dashuyun.cn

[S34] C++：遍历 vector
来源：http://iuu.shanyushiyangkeji.top

for (auto &x : v) { std::cout << x; }
来源：http://rkd.9152youxi.cn

[S35] C++：map
来源：http://owp.yangfankeji.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://brm.zhongyouzk.top

[S36] C++：unordered_map
来源：http://azl.smart0.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://icv.jianghu66.top

[S37] C++：set
来源：http://irv.zhongyouzk.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nul.yj20258.top

[S38] C++：排序
来源：http://omt.bjfxy.top

std::sort(v.begin(), v.end());
来源：http://rqs.yj20258888.top

[S39] C++：自定义比较器排序
来源：http://mky.hongshengwenyu.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ifr.xylfe.cn

[S40] C++：查找元素
来源：http://ilg.ctjpmb.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://izb.shangyingyoupin.top

[S41] C++：类与构造函数
来源：http://abg.shanyushiyangkeji.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bhb.havefunace.top

[S42] C++：继承与虚函数
来源：http://shi.jinyuanbaomall.cn

class B : public Base { public: void f() override {} };
来源：http://vuy.uphjek.com

[S43] C++：智能指针
来源：http://etd.hcnkem.com

auto p = std::make_unique<int>(5);
来源：http://ztc.mhx1999.top

[S44] C++：引用传参
来源：http://efm.fktsv.cn

void inc(int &x) { ++x; }
来源：http://sxa.yongpay.top

[S45] C++：lambda
来源：http://dey.snrcjt.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wpk.xinyue.icu

[S46] C++：函数模板
来源：http://qkr.hongshengwenyu.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ofg.cashguo.top

[S47] C++：结构化绑定遍历
来源：http://jcy.ppjwa.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ctq.ctjpmb.com

[S48] C++：逐行读文件
来源：http://ssk.zhongyouzk.top

std::ifstream in("a.txt");  std::string line;
来源：http://glv.nanxinkj.top

while (std::getline(in, line)) { }
来源：http://mhf.shzxlz.cn

[S49] C++：写文件
来源：http://prk.hesvh.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ike.yvedp.cn

[S50] C++：格式化数字
来源：http://egk.yj20258.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qaz.pycfn.com

[S51] C++：显式类型转换
来源：http://azq.ppjwa.cn

static_cast<double>(a) / b
来源：http://pli.hcnkem.com

[S52] C++：const 与 noexcept
来源：http://dpj.yj202588.top

int size() const noexcept { return n_; }
来源：http://gvz.hesvh.cn

[S53] C++：移动语义
来源：http://wvp.jinyuanbaomall.cn

std::vector<int> w = std::move(v);
来源：http://xle.jyoumei.cn

[S54] C++：异常处理
来源：http://bmo.yj20258.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hqi.fehbvm.com

[S55] C++：结构化绑定
来源：http://vdz.aizwys.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://muj.ydzc1.top

[S56] C++：optional
来源：http://ruz.yuanzhike.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ydj.bbcook.cn

[S57] C++：编译期常量
来源：http://oyb.redwolf501.top

constexpr int N = 10;
来源：http://hiz.hfpthk.cn

[S58] C++：命名空间
来源：http://hmb.fehbvm.com

namespace ns { int f() { return 1; } }
来源：http://sgn.zhengqikj.top

[S59] C++：静态断言
来源：http://ani.hesvh.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yxp.zhiwuduotai.top

[S60] C++：遍历并删除元素
来源：http://wzb.chenzaomai.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xwl.sufxvd.cn

================================================================================
来源：http://ilk.bjfxy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ksu.xuanzx.com

================================================================================
来源：http://lml.jyoumei.cn

[T01] Kotlin：Hello World
来源：http://wxw.sufxvd.cn

println("Hello")
来源：http://fis.xziqi.cn

[T02] Kotlin：变量
来源：http://zgl.jqgfzy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://whw.jqgfzy.top

[T03] Kotlin：字符串模板
来源：http://fsd.fanxiaobao.xyz

"值: $b"
来源：http://fgi.vehdjk.com

[T04] Kotlin：空安全
来源：http://qnx.jinyuanbaomall.cn

val n: String? = null;  n?.length
来源：http://ryy.316326.xyz

[T05] Kotlin：when 表达式
来源：http://kjf.cashguo.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lkh.hammf.cn

[T06] Kotlin：集合映射
来源：http://lll.zdbjq.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ors.quarkkingdee.top

[T07] Kotlin：集合过滤
来源：http://uiz.tianlin.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://pbq.yj20258.top

[T08] Kotlin：数据类
来源：http://dnn.0kj1m.cn

data class User(val name: String, val age: Int)
来源：http://oya.yj202588.top

[T09] Kotlin：扩展函数
来源：http://shv.sxryk.cn

fun String.exclaim() = this + "!"
来源：http://syx.ywan-chungtsiang.top

[T10] Kotlin：默认参数
来源：http://cqb.chenzaomai.com

fun greet(name: String = "World") = "Hi $name"
来源：http://aaj.sweek.top

[T11] Kotlin：协程
来源：http://jxk.vqdsnc.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://cjg.hnxiangtu.top

[T12] Kotlin：解构声明
来源：http://lnu.daxiang520.top

val (a, b) = Pair(1, 2)
来源：http://glz.cheryme.top

[T13] Kotlin：只读 Map
来源：http://yys.chenzaomai.com

val m = mapOf("a" to 1)
来源：http://ike.nwbrower.top

[T14] Kotlin：循环
来源：http://tin.hammf.cn

for (i in 1..10) println(i)
来源：http://zxs.shangyingyoupin.top

[T15] Kotlin：接口
来源：http://ipm.hnxiangtu.top

interface Shape { fun area(): Double }
来源：http://pul.svipenyu.cn

[T16] Swift：Hello World
来源：http://lsd.sweek.top

print("Hello")
来源：http://kfc.zhongyouzk.top

[T17] Swift：变量与常量
来源：http://jct.cashguo.top

var a = 1;  let b = 2
来源：http://lwr.hcnkem.com

[T18] Swift：字符串插值
来源：http://gjt.cucudq.cn

"值: \(b)"
来源：http://fxi.snrcjt.cn

[T19] Swift：可选绑定
来源：http://aoe.bjfxy.top

if let n = opt { print(n) }
来源：http://bks.yfazqb.com

[T20] Swift：数组操作
来源：http://jze.pycfn.com

var a = [1, 2, 3];  a.append(4)
来源：http://dhj.vehdjk.com

[T21] Swift：遍历
来源：http://xey.xuetiantiany.cn

for x in a { print(x) }
来源：http://kwl.nwbrower.top

[T22] Swift：字典
来源：http://icn.jinyuanbaomall.cn

var d = ["a": 1];  d["b"] = 2
来源：http://omx.ctjpmb.com

[T23] Swift：函数
来源：http://dff.cheryme.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rrq.xuanzx.com

[T24] Swift：闭包
来源：http://nzi.chenjidiqi.icu

let f = { (x: Int) -> Int in x * 2 }
来源：http://fgv.316326.xyz

[T25] Swift：结构体
来源：http://jrn.daxiang520.top

struct P { var x: Int }
来源：http://uim.yj20258.top

[T26] Swift：类与重写
来源：http://xin.tianlin.xyz

class A: Base { override func f() {} }
来源：http://kra.hnqzz.top

[T27] Swift：错误处理
来源：http://ovj.sufxvd.cn

do { try f() } catch { print(error) }
来源：http://dcn.zdqjudy.top

[T28] Swift：枚举
来源：http://yaz.guowangkeji.top

enum Color { case red, green }
来源：http://ghg.jqgufenzy.top

[T29] Swift：guard 提前返回
来源：http://axx.birdmap.top

guard let x = opt else { return }
来源：http://wje.bjfxy.top

[T30] Swift：协议
来源：http://wip.havefunace.top

protocol Shape { func area() -> Double }
来源：http://ddn.cucudq.cn

[T31] Lua：Hello World
来源：http://vnv.tarul.cn

print("Hello")
来源：http://oum.gzhubu.top

[T32] Lua：局部变量
来源：http://iwx.jianghu66.top

local a = 1
来源：http://ykk.ybcxt.top

[T33] Lua：表（数组）
来源：http://hxq.quarkkingdee.top

local t = {1, 2, 3};  t[4] = 4
来源：http://usb.tianlin.xyz

[T34] Lua：遍历表
来源：http://ltw.gogol.net.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://dbh.jlsjyb.cn

[T35] Lua：字典表
来源：http://oke.guowangkeji.top

local d = { a = 1 };  d.b = 2
来源：http://oxi.jqgfzy.top

[T36] Lua：函数
来源：http://zqh.mhx1999.top

function add(a, b) return a + b end
来源：http://emu.xuetiantiany.cn

[T37] Lua：字符串拼接
来源：http://rmd.sufxvd.cn

"a" .. "b"
来源：http://sil.yvedp.cn

[T38] Lua：条件
来源：http://oiw.cqqwz.cn

if x > 0 then print("正") end
来源：http://bvk.guowangkeji.top

[T39] Lua：模式匹配
来源：http://kys.shanyushiyangtech.top

string.find(s, "%d+")
来源：http://pxb.vehdjk.com

[T40] Lua：元表
来源：http://rzg.hnxiangtu.top

setmetatable({}, { __index = base })
来源：http://rnx.zhongyouzk.top

[T41] Perl：Hello World
来源：http://hvz.jlsjyb.cn

print "Hello\n";
来源：http://pyw.vqdsnc.cn

[T42] Perl：变量类型
来源：http://owa.chenjidiqi.icu

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ucs.tarul.cn

[T43] Perl：字符串插值
来源：http://uuh.ywan-chungtsiang.top

"值: $a"
来源：http://oxy.epnwcf.com

[T44] Perl：条件
来源：http://mrx.bjfxy.top

if ($a > 0) { print "正"; }
来源：http://flp.yj202588.top

[T45] Perl：数组遍历
来源：http://ipq.birdmap.top

for my $x (@arr) { print $x; }
来源：http://qok.0kj1m.cn

[T46] Perl：哈希操作
来源：http://ybj.fktsv.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://uqi.jinyuanbaomall.cn

[T47] Perl：正则捕获
来源：http://sqn.epnwcf.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://ign.shzxlz.cn

[T48] Perl：正则替换
来源：http://ldf.fengsongda.top

$s =~ s/old/new/g;
来源：http://xqm.zdqjudy.top

[T49] Perl：函数
来源：http://rhk.jlsjyb.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ams.yuxming.cn

[T50] Perl：逐行读文件
来源：http://csq.cqqwz.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ldq.316326.xyz

while (my $line = <$fh>) { print $line; }
来源：http://dsi.hongshengwenyu.top

[T51] Scala：Hello World
来源：http://wqn.c1oappe.top

println("Hello")
来源：http://mra.bbcook.cn

[T52] Scala：变量
来源：http://kph.xingfuxueyuan.xyz

val a = 1;  var b = 2
来源：http://ikf.birdmap.top

[T53] Scala：字符串插值
来源：http://ypi.chenlongwang.top

s"值: $b"
来源：http://gmz.nwbrower.top

[T54] Scala：集合映射
来源：http://hbn.vqdsnc.cn

List(1, 2, 3).map(_ * 2)
来源：http://nhi.bjfxy.top

[T55] Scala：集合过滤
来源：http://qjb.smart0.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://xve.jinghuilouyu.cn

[T56] Scala：样例类
来源：http://ddy.hfpthk.cn

case class User(name: String, age: Int)
来源：http://cfy.tianlin.xyz

[T57] Scala：模式匹配
来源：http://lkg.aizwys.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://twm.zhixingplan.top

[T58] Scala：函数定义
来源：http://rxl.vqdsnc.cn

def add(a: Int, b: Int): Int = a + b
来源：http://szc.jinyuanbaomall.cn

[T59] Scala：循环
来源：http://bcq.jyoumei.cn

for (i <- 1 to 10) println(i)
来源：http://vqs.haohaochexian.top

[T60] Scala：折叠
来源：http://kkv.haohaochexian.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mwx.shangyingyoupin.top

================================================================================
来源：http://epc.bbcook.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dcb.jinghuilouyu.cn

================================================================================
来源：http://mib.zhiwuduotai.top

[U01] Py：创建虚拟环境
来源：http://dfv.yueranfly.top

python -m venv .venv && source .venv/bin/activate
来源：http://vnk.zdqjudy.top

[U02] Py：导出 / 安装依赖
来源：http://rzc.epnwcf.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vqv.c1oappe.top

[U03] Py：加载 .env 配置
来源：http://drv.mhx1999.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ivt.wangdashe.top

[U04] Py：变量调试打印
来源：http://zvo.chenlongwang.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qhn.shanyushiyangtech.top

[U05] Py：列表去重且保序
来源：http://qph.yonumen.top

list(dict.fromkeys(arr))
来源：http://ith.jiagoushi.top

[U06] Py：合并两个字典
来源：http://omx.cashguo.top

{**a, **b}
来源：http://tmq.gotoacloud.top

[U07] Py：反转字典键值
来源：http://upp.chenjidiqi.icu

{v: k for k, v in d.items()}
来源：http://yds.guowangkeji.top

[U08] Py：展平二维列表
来源：http://qkj.fehbvm.com

[y for x in nested for y in x]
来源：http://ana.tian-w.cn

[U09] Py：字典取最大值的键
来源：http://ils.gaohongyu789.top

max(d, key=d.get)
来源：http://oal.aibaodan.cn

[U10] Py：按值排序字典
来源：http://ced.dianchejie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lrq.yfazqb.com

[U11] Py：生成器表达式
来源：http://mjy.yvedp.cn

(x * 2 for x in arr)
来源：http://ase.shanyushiyangtech.top

[U12] Py：取出现最多的 3 个元素
来源：http://erz.xuetiantiany.cn

Counter(arr).most_common(3)
来源：http://gid.zhengqikj.top

[U13] Py：固定长度队列
来源：http://tjb.mhx1999.top

deque(maxlen=10)
来源：http://gjg.wangdashe.top

[U14] Py：分组收集到列表
来源：http://zyr.shzxlz.cn

defaultdict(list)
来源：http://scf.aizwys.cn

[U15] Py：高精度计时
来源：http://oin.9152youxi.cn

t = time.perf_counter()
来源：http://erd.yj20258.top

[U16] Py：命令行参数解析
来源：http://igd.cucudq.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rmo.jianghu66.top

[U17] Py：初始化日志
来源：http://tdg.shuidangran.top

logging.basicConfig(level=logging.INFO)
来源：http://edo.xuanzx.com

[U18] Py：预编译正则
来源：http://jjg.bjfxy.top

pat = re.compile(r"\d+")
来源：http://ovx.xinyue.icu

[U19] Py：正则替换带回调
来源：http://mmz.ppjwa.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zfv.hnqzz.top

[U20] Py：缓存函数结果
来源：http://uhv.meibo888.top

@functools.lru_cache(maxsize=None)
来源：http://hgo.kuanghao11.cn

[U21] Py：自定义上下文管理器
来源：http://xdu.hfpthk.cn

@contextlib.contextmanager
来源：http://ctj.yfazqb.com

[U22] Py：矩阵转置
来源：http://krx.shanyushiyangkeji.top

list(zip(*m))
来源：http://vyn.fehbvm.com

[U23] Py：分块读取大文件
来源：http://izm.pycfn.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lcp.ydjk.org.cn

[U24] Py：路径操作
来源：http://xco.svipenyu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dvw.zhijiandao.cn

[U25] Py：CSV 按字典读
来源：http://tmz.daria6918.cn

csv.DictReader(f)
来源：http://vqr.xingfuxueyuan.xyz

[U26] Py：并发下载
来源：http://vsd.fktsv.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zlo.cqqwz.cn

[U27] Py：异步 HTTP
来源：http://emy.shanyushiyangtech.top

aiohttp.ClientSession() 配合 async with
来源：http://lxn.pycfn.com

[U28] Py：类型别名
来源：http://lyn.cqqwz.cn

UserId = int
来源：http://zyi.cheryme.top

[U29] Py：属性校验
来源：http://jbv.vqdsnc.cn

@property 与 @x.setter 配合
来源：http://wwc.ywan-chungtsiang.top

[U30] Py：数据类
来源：http://dsj.guannengcc.top

@dataclass(slots=True)
来源：http://uap.c1oappe.top

[U31] Py：单测
来源：http://zyj.yj20258.top

python -m pytest -q
来源：http://gbi.ppjwa.cn

[U32] Py：代码格式化
来源：http://epa.yj20258888.top

ruff format . && ruff check --fix .
来源：http://kek.guannengcc.top

[U33] Py：打包发布
来源：http://gpu.xylfe.cn

python -m build  （依赖 pyproject.toml）
来源：http://keu.jyoumei.cn

[U34] Py：判断编码
来源：http://cjx.xylfe.cn

chardet.detect(raw)
来源：http://ady.havefunace.top

[U35] Py：发送邮件
来源：http://jpa.jiagoushi.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ejv.hysaishi.cn

[U36] Py：定时任务
来源：http://ccu.jinqigufen.top

schedule.every(10).minutes.do(job)
来源：http://jvj.xingfuxueyuan.xyz

[U37] Py：读写 Excel
来源：http://wkf.redwolf501.top

pandas.read_excel / DataFrame.to_excel
来源：http://qqm.yangfankeji.com

[U38] Py：获取脚本所在目录
来源：http://oag.316326.xyz

Path(__file__).resolve().parent
来源：http://bxt.wangshuangyany.cn

[U39] Py：判断是否在交互环境
来源：http://oxp.hcnkem.com

sys.stdout.isatty()
来源：http://oov.sjlbkw.cn

[U40] Py：打印到标准错误
来源：http://qcq.0kj1m.cn

print("err", file=sys.stderr)
来源：http://dpt.hesvh.cn

[U41] PHP：初始化 Composer 项目
来源：http://fvl.dashuyun.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://bcb.zhaomingkeji.xyz

[U42] PHP：PSR-4 自动加载
来源：http://dem.dashuyun.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://woq.tianlin.xyz

[U43] PHP：声明命名空间
来源：http://pgb.meibo888.top

namespace App\Http;
来源：http://ndp.birdmap.top

[U44] PHP：开启严格类型
来源：http://cub.0kj1m.cn

declare(strict_types=1);
来源：http://trt.gotoacloud.top


<!-- 参考信息 -->