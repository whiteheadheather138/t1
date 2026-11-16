代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dap.tarul.cn

[S21] C：字符类别判断
来源：http://bnr.xingfuxueyuan.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zgg.hnqzz.top

[S22] C：字符串转数字
来源：http://tkj.ydzc1.top

atoi("42");  strtod("3.14", NULL);
来源：http://mgj.yanxiufei.cn

[S23] C：随机数
来源：http://nfv.c1oappe.top

srand(time(NULL));  int r = rand() % 100;
来源：http://mug.xylfe.cn

[S24] C：获取本地时间
来源：http://dkj.0kj1m.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://oos.sweek.top

[S25] C：内存拷贝
来源：http://msj.fengsongda.top

memcpy(dst, src, n);
来源：http://lwu.yanxiufei.cn

[S26] C：内存清零
来源：http://kbp.nanxinkj.top

memset(a, 0, sizeof a);
来源：http://oaz.hfpthk.cn

[S27] C：定义常量
来源：http://sgz.tian-w.cn

const double PI = 3.14159;
来源：http://hcj.vehdjk.com

[S28] C：静态变量
来源：http://fpg.zhixingplan.top

static int counter = 0;
来源：http://jrp.hnqzz.top

[S29] C：变参函数
来源：http://cfu.xingfuxueyuan.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bym.yfazqb.com

[S30] C：头文件保护
来源：http://dav.gogol.net.cn

#ifndef X_H
来源：http://jvm.yuanzhike.top

#define X_H
来源：http://iuw.jinqigfzy.top

#endif
来源：http://lif.sxryk.cn

[S31] C++：Hello World
来源：http://xmo.gotoacloud.top

#include <iostream>
来源：http://tlr.yj20258888.top

int main() { std::cout << "Hello\n"; }
来源：http://hhb.hysaishi.cn

[S32] C++：字符串
来源：http://cti.yuxming.cn

std::string s = "hi";  s += "!";
来源：http://rzu.daxiang520.top

[S33] C++：vector 增删
来源：http://mxt.meibo888.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jdl.redwolf501.top

[S34] C++：遍历 vector
来源：http://nij.sufxvd.cn

for (auto &x : v) { std::cout << x; }
来源：http://ooc.jinyuanbaomall.cn

[S35] C++：map
来源：http://fcz.xuetiantiany.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ivu.9152youxi.cn

[S36] C++：unordered_map
来源：http://bze.dianchejie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qmi.daria6918.cn

[S37] C++：set
来源：http://dbk.cdnleiting.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wxo.aizwys.cn

[S38] C++：排序
来源：http://dke.gotoacloud.top

std::sort(v.begin(), v.end());
来源：http://rfz.jinqigfzy.top

[S39] C++：自定义比较器排序
来源：http://irv.sufxvd.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uvq.ppjwa.cn

[S40] C++：查找元素
来源：http://mvq.zdbjq.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ivr.jinqigfzy.top

[S41] C++：类与构造函数
来源：http://pdl.jqgufenzy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jfj.aibaodan.cn

[S42] C++：继承与虚函数
来源：http://sew.aibaodan.cn

class B : public Base { public: void f() override {} };
来源：http://qfh.ppjwa.cn

[S43] C++：智能指针
来源：http://voo.jqgufenzy.top

auto p = std::make_unique<int>(5);
来源：http://jxr.cheryme.top

[S44] C++：引用传参
来源：http://otp.xuetiantiany.cn

void inc(int &x) { ++x; }
来源：http://cqi.zhengqikj.top

[S45] C++：lambda
来源：http://zea.chenlongwang.top

auto add = [](int a, int b) { return a + b; };
来源：http://aib.pengpengdd.cyou

[S46] C++：函数模板
来源：http://den.kuanghao11.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wjs.zhongyouzk.top

[S47] C++：结构化绑定遍历
来源：http://ocg.meibo888.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lsj.bjfxy.top

[S48] C++：逐行读文件
来源：http://djp.jqgufenzy.top

std::ifstream in("a.txt");  std::string line;
来源：http://rid.wangshuangyany.cn

while (std::getline(in, line)) { }
来源：http://qdb.jiagoushi.top

[S49] C++：写文件
来源：http://ddx.jqgfzy.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ocu.xuetiantiany.cn

[S50] C++：格式化数字
来源：http://cfr.sufxvd.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://efn.sxryk.cn

[S51] C++：显式类型转换
来源：http://ygb.hysaishi.cn

static_cast<double>(a) / b
来源：http://fsu.xingfuxueyuan.xyz

[S52] C++：const 与 noexcept
来源：http://wir.andypj.xyz

int size() const noexcept { return n_; }
来源：http://kqn.guowangkeji.top

[S53] C++：移动语义
来源：http://apg.jinqigfzy.top

std::vector<int> w = std::move(v);
来源：http://xof.uphjek.com

[S54] C++：异常处理
来源：http://tms.xingfuxueyuan.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://umf.shuidangran.top

[S55] C++：结构化绑定
来源：http://rit.yuxming.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://hcj.shanyushiyangtech.top

[S56] C++：optional
来源：http://xne.xinyue.icu

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dlu.zhongyouzk.top

[S57] C++：编译期常量
来源：http://kfw.ybcxt.top

constexpr int N = 10;
来源：http://xrp.zhijiandao.cn

[S58] C++：命名空间
来源：http://vvz.sweek.top

namespace ns { int f() { return 1; } }
来源：http://xyb.sweek.top

[S59] C++：静态断言
来源：http://pax.gogol.net.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://aow.vqdsnc.cn

[S60] C++：遍历并删除元素
来源：http://vft.jinghuilouyu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jlz.tarul.cn

================================================================================
来源：http://xoa.zdbjq.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hir.wangshuangyany.cn

================================================================================
来源：http://yqs.cucudq.cn

[T01] Kotlin：Hello World
来源：http://jfl.cqqwz.cn

println("Hello")
来源：http://ypc.ppjwa.cn

[T02] Kotlin：变量
来源：http://lxp.0kj1m.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://utj.hesvh.cn

[T03] Kotlin：字符串模板
来源：http://fdx.vqdsnc.cn

"值: $b"
来源：http://suk.redwolf501.top

[T04] Kotlin：空安全
来源：http://zzg.jlsjyb.cn

val n: String? = null;  n?.length
来源：http://rub.sweek.top

[T05] Kotlin：when 表达式
来源：http://jgc.gaohongyu789.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ult.fengsongda.top

[T06] Kotlin：集合映射
来源：http://wla.jlsjyb.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://gjp.yangfankeji.com

[T07] Kotlin：集合过滤
来源：http://cdd.xziqi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://dpz.tian-w.cn

[T08] Kotlin：数据类
来源：http://lzn.dianchejie.cn

data class User(val name: String, val age: Int)
来源：http://ein.jinqigufen.top

[T09] Kotlin：扩展函数
来源：http://iqr.jiagoushi.top

fun String.exclaim() = this + "!"
来源：http://qku.vehdjk.com

[T10] Kotlin：默认参数
来源：http://doe.jinqigfzy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://qyw.ywan-chungtsiang.top

[T11] Kotlin：协程
来源：http://ban.sweek.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://wqi.shanyushiyangtech.top

[T12] Kotlin：解构声明
来源：http://gsn.gotoacloud.top

val (a, b) = Pair(1, 2)
来源：http://rmu.svipenyu.cn

[T13] Kotlin：只读 Map
来源：http://jwc.xinyue.icu

val m = mapOf("a" to 1)
来源：http://usw.uphjek.com

[T14] Kotlin：循环
来源：http://ihd.yj20258888.top

for (i in 1..10) println(i)
来源：http://wbv.sjlbkw.cn

[T15] Kotlin：接口
来源：http://wov.haohaochexian.top

interface Shape { fun area(): Double }
来源：http://kku.jqgfzy.top

[T16] Swift：Hello World
来源：http://fxa.zhixingplan.top

print("Hello")
来源：http://hmd.nwbrower.top

[T17] Swift：变量与常量
来源：http://tje.fehbvm.com

var a = 1;  let b = 2
来源：http://gcx.sxryk.cn

[T18] Swift：字符串插值
来源：http://msi.feifeiyinyue.top

"值: \(b)"
来源：http://wgt.yuanzhike.top

[T19] Swift：可选绑定
来源：http://jlu.fanxiaobao.xyz

if let n = opt { print(n) }
来源：http://hgq.havefunace.top

[T20] Swift：数组操作
来源：http://rgo.hcnkem.com

var a = [1, 2, 3];  a.append(4)
来源：http://iaw.hammf.cn

[T21] Swift：遍历
来源：http://tin.zycfv.cn

for x in a { print(x) }
来源：http://tea.zhijiandao.cn

[T22] Swift：字典
来源：http://mfr.meibo888.top

var d = ["a": 1];  d["b"] = 2
来源：http://qcs.zhoulong.xyz

[T23] Swift：函数
来源：http://ucc.zhiwuduotai.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yeg.jiagoushi.top

[T24] Swift：闭包
来源：http://iwi.fzhhl.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://nkv.ydzc1.top

[T25] Swift：结构体
来源：http://jdk.ydzc1.top

struct P { var x: Int }
来源：http://tln.nanxuanxn.top

[T26] Swift：类与重写
来源：http://mtq.nwbrower.top

class A: Base { override func f() {} }
来源：http://rur.zdbjq.cn

[T27] Swift：错误处理
来源：http://dbp.jiagoushi.top

do { try f() } catch { print(error) }
来源：http://gtv.ctjpmb.com

[T28] Swift：枚举
来源：http://jzo.guowangkeji.top

enum Color { case red, green }
来源：http://lko.ehwqpu.com

[T29] Swift：guard 提前返回
来源：http://uzx.guannengcc.top

guard let x = opt else { return }
来源：http://rud.tian-w.cn

[T30] Swift：协议
来源：http://bgu.shuidangran.top

protocol Shape { func area() -> Double }
来源：http://bnz.yj20258.top

[T31] Lua：Hello World
来源：http://rsm.nanxuanxn.top

print("Hello")
来源：http://ysm.uphjek.com

[T32] Lua：局部变量
来源：http://ehp.gzhubu.top

local a = 1
来源：http://bdi.c1oappe.top

[T33] Lua：表（数组）
来源：http://ryw.xuetiantiany.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://awy.fanxiaobao.xyz

[T34] Lua：遍历表
来源：http://ahs.fehbvm.com

for i, v in ipairs(t) do print(i, v) end
来源：http://lye.svipenyu.cn

[T35] Lua：字典表
来源：http://atm.zhijiandao.cn

local d = { a = 1 };  d.b = 2
来源：http://vhg.pycfn.com

[T36] Lua：函数
来源：http://ufn.tian-w.cn

function add(a, b) return a + b end
来源：http://npe.guannengcc.top

[T37] Lua：字符串拼接
来源：http://ywe.yfazqb.com

"a" .. "b"
来源：http://bbd.jqgfzy.top

[T38] Lua：条件
来源：http://wio.birdmap.top

if x > 0 then print("正") end
来源：http://mjx.jqgfzy.top

[T39] Lua：模式匹配
来源：http://wkp.jlsjyb.cn

string.find(s, "%d+")
来源：http://tsl.jinqigfzy.top

[T40] Lua：元表
来源：http://wue.zhijiandao.cn

setmetatable({}, { __index = base })
来源：http://eru.52xcode.cn

[T41] Perl：Hello World
来源：http://yuh.yangfankeji.com

print "Hello\n";
来源：http://dym.zhixingplan.top

[T42] Perl：变量类型
来源：http://fof.xingfuxueyuan.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jev.haohaochexian.top

[T43] Perl：字符串插值
来源：http://fig.yonumen.top

"值: $a"
来源：http://jxx.andypj.xyz

[T44] Perl：条件
来源：http://thz.chenlongwang.top

if ($a > 0) { print "正"; }
来源：http://yje.tianlin.xyz

[T45] Perl：数组遍历
来源：http://fjq.guowangkeji.top

for my $x (@arr) { print $x; }
来源：http://ebn.zhongyouzk.top

[T46] Perl：哈希操作
来源：http://jli.aizwys.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jqo.hongshengwenyu.top

[T47] Perl：正则捕获
来源：http://icq.sjlbkw.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://guc.smart0.xyz

[T48] Perl：正则替换
来源：http://apw.cqqwz.cn

$s =~ s/old/new/g;
来源：http://veu.yanxiufei.cn

[T49] Perl：函数
来源：http://ysu.tarul.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yeb.gogol.net.cn

[T50] Perl：逐行读文件
来源：http://wow.wangshuangyany.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://iwp.yangfankeji.com

while (my $line = <$fh>) { print $line; }
来源：http://lkq.mhx1999.top

[T51] Scala：Hello World
来源：http://gvk.chenlongwang.top

println("Hello")
来源：http://btc.zhongyouzk.top

[T52] Scala：变量
来源：http://wse.zhengqikj.top

val a = 1;  var b = 2
来源：http://twa.ywan-chungtsiang.top

[T53] Scala：字符串插值
来源：http://jht.hfpthk.cn

s"值: $b"
来源：http://alp.cucudq.cn

[T54] Scala：集合映射
来源：http://wgq.ivvv.top

List(1, 2, 3).map(_ * 2)
来源：http://xxd.meibo888.top

[T55] Scala：集合过滤
来源：http://hbn.aizwys.cn

List(1, 2, 3).filter(_ > 1)
来源：http://tel.ehwqpu.com

[T56] Scala：样例类
来源：http://hmp.ydzc1.top

case class User(name: String, age: Int)
来源：http://ruj.hfpthk.cn

[T57] Scala：模式匹配
来源：http://qlq.xinyue.icu

x match { case 1 => "一"; case _ => "其他" }
来源：http://nhj.smart0.xyz

[T58] Scala：函数定义
来源：http://kmc.0kj1m.cn

def add(a: Int, b: Int): Int = a + b
来源：http://kbd.xuetiantiany.cn

[T59] Scala：循环
来源：http://vmq.c1oappe.top

for (i <- 1 to 10) println(i)
来源：http://qvn.yfazqb.com

[T60] Scala：折叠
来源：http://wye.ydjk.org.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ufj.jqgufenzy.top

================================================================================
来源：http://aad.hywenlv.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tbw.zhijiandao.cn

================================================================================
来源：http://wek.gaohongyu789.top

[U01] Py：创建虚拟环境
来源：http://slw.xziqi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://spv.jyoumei.cn

[U02] Py：导出 / 安装依赖
来源：http://wlb.wangshuangyany.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ytz.hfpthk.cn

[U03] Py：加载 .env 配置
来源：http://mqu.fktsv.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://bsk.xylfe.cn

[U04] Py：变量调试打印
来源：http://ydb.ybcxt.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bzb.xingfuxueyuan.xyz

[U05] Py：列表去重且保序
来源：http://syq.chenlongwang.top

list(dict.fromkeys(arr))
来源：http://qmr.chenzaomai.com

[U06] Py：合并两个字典
来源：http://wdr.zycfv.cn

{**a, **b}
来源：http://mgf.yj20258.top

[U07] Py：反转字典键值
来源：http://ope.bbcook.cn

{v: k for k, v in d.items()}
来源：http://evc.dianchejie.cn

[U08] Py：展平二维列表
来源：http://cwe.jiagoushi.top

[y for x in nested for y in x]
来源：http://llk.pycfn.com

[U09] Py：字典取最大值的键
来源：http://fdr.cucudq.cn

max(d, key=d.get)
来源：http://eek.bjfxy.top

[U10] Py：按值排序字典
来源：http://yhx.gaohongyu789.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wmk.52xcode.cn

[U11] Py：生成器表达式
来源：http://eol.svipenyu.cn

(x * 2 for x in arr)
来源：http://yxd.sweek.top

[U12] Py：取出现最多的 3 个元素
来源：http://bba.cucudq.cn

Counter(arr).most_common(3)
来源：http://enq.yongpay.top

[U13] Py：固定长度队列
来源：http://vep.daxiang520.top

deque(maxlen=10)
来源：http://nty.yj202588.top

[U14] Py：分组收集到列表
来源：http://wzl.vehdjk.com

defaultdict(list)
来源：http://lrj.yj20258.top

[U15] Py：高精度计时
来源：http://utx.aizwys.cn

t = time.perf_counter()
来源：http://nuw.xuanzx.com

[U16] Py：命令行参数解析
来源：http://ymm.epnwcf.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gsf.dashuyun.cn

[U17] Py：初始化日志
来源：http://mbi.hnxiangtu.top

logging.basicConfig(level=logging.INFO)
来源：http://dlt.cqqwz.cn

[U18] Py：预编译正则
来源：http://yzc.xuetiantiany.cn

pat = re.compile(r"\d+")
来源：http://jvj.yangfankeji.com

[U19] Py：正则替换带回调
来源：http://dpi.wangdashe.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://odc.nanxuanxn.top

[U20] Py：缓存函数结果
来源：http://wgi.0kj1m.cn

@functools.lru_cache(maxsize=None)
来源：http://uru.shuidangran.top

[U21] Py：自定义上下文管理器
来源：http://pxc.sysykeji.top

@contextlib.contextmanager
来源：http://toj.cucudq.cn

[U22] Py：矩阵转置
来源：http://zoy.iojbl.cn

list(zip(*m))
来源：http://fld.sysykeji.top

[U23] Py：分块读取大文件
来源：http://uoj.gotoacloud.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://cew.wangshuangyany.cn

[U24] Py：路径操作
来源：http://htz.meibo888.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://kvp.tianlin.xyz

[U25] Py：CSV 按字典读
来源：http://dqq.epnwcf.com

csv.DictReader(f)
来源：http://bux.zycfv.cn

[U26] Py：并发下载
来源：http://vdo.cucudq.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rlz.cqqwz.cn

[U27] Py：异步 HTTP
来源：http://doi.vehdjk.com

aiohttp.ClientSession() 配合 async with
来源：http://uou.cdnleiting.top

[U28] Py：类型别名
来源：http://zyq.sjlbkw.cn

UserId = int
来源：http://eav.fengsongda.top

[U29] Py：属性校验
来源：http://iwt.hysaishi.cn

@property 与 @x.setter 配合
来源：http://ore.epnwcf.com

[U30] Py：数据类
来源：http://xdh.cashguo.top

@dataclass(slots=True)
来源：http://tob.cheryme.top

[U31] Py：单测
来源：http://iqh.hnxiangtu.top

python -m pytest -q
来源：http://voz.yanxiufei.cn

[U32] Py：代码格式化
来源：http://xwm.ppjwa.cn

ruff format . && ruff check --fix .
来源：http://yqp.quarkkingdee.top

[U33] Py：打包发布
来源：http://wzj.jinqigfzy.top

python -m build  （依赖 pyproject.toml）
来源：http://yel.fzhhl.top

[U34] Py：判断编码
来源：http://ycd.0kj1m.cn

chardet.detect(raw)
来源：http://kjx.zhoulong.xyz

[U35] Py：发送邮件
来源：http://zkm.9152youxi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rah.tian-w.cn

[U36] Py：定时任务
来源：http://tws.ydjk.org.cn

schedule.every(10).minutes.do(job)
来源：http://ili.c1oappe.top

[U37] Py：读写 Excel
来源：http://gok.zdqjudy.top

pandas.read_excel / DataFrame.to_excel
来源：http://bcs.316326.xyz

[U38] Py：获取脚本所在目录
来源：http://hfd.svipenyu.cn

Path(__file__).resolve().parent
来源：http://bjd.vqdsnc.cn

[U39] Py：判断是否在交互环境
来源：http://xsh.jlsjyb.cn

sys.stdout.isatty()
来源：http://gjv.ppjwa.cn

[U40] Py：打印到标准错误
来源：http://hlq.0kj1m.cn

print("err", file=sys.stderr)
来源：http://dsv.sufxvd.cn

[U41] PHP：初始化 Composer 项目
来源：http://cuc.hongshengwenyu.top

composer init;  composer require guzzlehttp/guzzle
来源：http://sgz.daxiang520.top

[U42] PHP：PSR-4 自动加载
来源：http://rht.tanke756.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cyq.fanxiaobao.xyz

[U43] PHP：声明命名空间
来源：http://poa.yongpay.top

namespace App\Http;
来源：http://wnl.dianchejie.cn

[U44] PHP：开启严格类型
来源：http://ybr.guowangkeji.top

declare(strict_types=1);
来源：http://ldk.xinyue.icu


<!-- 参考信息 -->