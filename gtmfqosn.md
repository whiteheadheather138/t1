代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zuw.jianghu66.top

[S21] C：字符类别判断
来源：http://uji.xingfuxueyuan.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jmz.meibo888.top

[S22] C：字符串转数字
来源：http://tve.aibaodan.cn

atoi("42");  strtod("3.14", NULL);
来源：http://fij.daria6918.cn

[S23] C：随机数
来源：http://oqp.kuanghao11.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://tsd.fktsv.cn

[S24] C：获取本地时间
来源：http://rrz.gotoacloud.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://uut.daria6918.cn

[S25] C：内存拷贝
来源：http://een.yanxiufei.cn

memcpy(dst, src, n);
来源：http://nyp.zhongyouzk.top

[S26] C：内存清零
来源：http://nsb.chenlongwang.top

memset(a, 0, sizeof a);
来源：http://lce.iojbl.cn

[S27] C：定义常量
来源：http://lmu.cqqwz.cn

const double PI = 3.14159;
来源：http://dqf.vqdsnc.cn

[S28] C：静态变量
来源：http://gbw.shanyushiyangkeji.top

static int counter = 0;
来源：http://ese.wangdashe.top

[S29] C：变参函数
来源：http://ysq.ctjpmb.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://avn.xuanzx.com

[S30] C：头文件保护
来源：http://nkw.c1oappe.top

#ifndef X_H
来源：http://ait.wangdashe.top

#define X_H
来源：http://vjr.guannengcc.top

#endif
来源：http://vos.zhoulong.xyz

[S31] C++：Hello World
来源：http://edl.pycfn.com

#include <iostream>
来源：http://aby.ydzc1.top

int main() { std::cout << "Hello\n"; }
来源：http://kni.yj20258888.top

[S32] C++：字符串
来源：http://qcp.sjlbkw.cn

std::string s = "hi";  s += "!";
来源：http://dxo.gzhubu.top

[S33] C++：vector 增删
来源：http://pnp.ywan-chungtsiang.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zyg.tanke756.top

[S34] C++：遍历 vector
来源：http://flr.shanyushiyangtech.top

for (auto &x : v) { std::cout << x; }
来源：http://tey.yanxiufei.cn

[S35] C++：map
来源：http://kkd.fzhhl.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://odg.vqdsnc.cn

[S36] C++：unordered_map
来源：http://kjy.xinyue.icu

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xkw.fzhhl.top

[S37] C++：set
来源：http://qwx.xuanzx.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://afg.ydzc1.top

[S38] C++：排序
来源：http://frg.nwbrower.top

std::sort(v.begin(), v.end());
来源：http://tbb.cheryme.top

[S39] C++：自定义比较器排序
来源：http://mkv.vehdjk.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://psi.fktsv.cn

[S40] C++：查找元素
来源：http://gtv.fengsongda.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rer.xuetiantiany.cn

[S41] C++：类与构造函数
来源：http://aei.gotoacloud.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gju.fengsongda.top

[S42] C++：继承与虚函数
来源：http://ntv.cheryme.top

class B : public Base { public: void f() override {} };
来源：http://mjp.nanxinkj.top

[S43] C++：智能指针
来源：http://cnx.fehbvm.com

auto p = std::make_unique<int>(5);
来源：http://lxl.vqdsnc.cn

[S44] C++：引用传参
来源：http://qsr.sysykeji.top

void inc(int &x) { ++x; }
来源：http://ogv.jqgfzy.top

[S45] C++：lambda
来源：http://lpm.shuidangran.top

auto add = [](int a, int b) { return a + b; };
来源：http://uwh.hnqzz.top

[S46] C++：函数模板
来源：http://mil.epnwcf.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pwz.ehwqpu.com

[S47] C++：结构化绑定遍历
来源：http://yeq.nanxuanxn.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zqk.yueranfly.top

[S48] C++：逐行读文件
来源：http://uam.zycfv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vdw.zhixingplan.top

while (std::getline(in, line)) { }
来源：http://usz.haohaochexian.top

[S49] C++：写文件
来源：http://pfz.daxiang520.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://spg.hywenlv.cn

[S50] C++：格式化数字
来源：http://sgj.gogol.net.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ocn.tarul.cn

[S51] C++：显式类型转换
来源：http://wfx.nwbrower.top

static_cast<double>(a) / b
来源：http://byt.daxiang520.top

[S52] C++：const 与 noexcept
来源：http://vuk.hnqzz.top

int size() const noexcept { return n_; }
来源：http://czt.feifeiyinyue.top

[S53] C++：移动语义
来源：http://ndj.tanke756.top

std::vector<int> w = std::move(v);
来源：http://pqi.hfpthk.cn

[S54] C++：异常处理
来源：http://eim.ydjk.org.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tzu.iojbl.cn

[S55] C++：结构化绑定
来源：http://hle.meibo888.top

auto [a, b] = std::make_pair(1, 2);
来源：http://hpl.yanxiufei.cn

[S56] C++：optional
来源：http://zlj.zhijiandao.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pje.gaohongyu789.top

[S57] C++：编译期常量
来源：http://mjy.jinghuilouyu.cn

constexpr int N = 10;
来源：http://qnv.chenlongwang.top

[S58] C++：命名空间
来源：http://bcq.nanxinkj.top

namespace ns { int f() { return 1; } }
来源：http://fbh.smart0.xyz

[S59] C++：静态断言
来源：http://gnp.9152youxi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mkz.fehbvm.com

[S60] C++：遍历并删除元素
来源：http://gif.316326.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ncd.vqdsnc.cn

================================================================================
来源：http://fzy.zhixingplan.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vza.nanxinkj.top

================================================================================
来源：http://yhu.yj20258888.top

[T01] Kotlin：Hello World
来源：http://gks.c1oappe.top

println("Hello")
来源：http://aqw.jinqigufen.top

[T02] Kotlin：变量
来源：http://eaf.xylfe.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nnh.hesvh.cn

[T03] Kotlin：字符串模板
来源：http://ypf.jinyuanbaomall.cn

"值: $b"
来源：http://lyp.mhx1999.top

[T04] Kotlin：空安全
来源：http://jct.kuanghao11.cn

val n: String? = null;  n?.length
来源：http://ndq.yvedp.cn

[T05] Kotlin：when 表达式
来源：http://gzf.nanxinkj.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://orr.9152youxi.cn

[T06] Kotlin：集合映射
来源：http://zti.tian-w.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://iiv.jqgfzy.top

[T07] Kotlin：集合过滤
来源：http://swn.hfpthk.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ife.andypj.xyz

[T08] Kotlin：数据类
来源：http://wve.zhongyouzk.top

data class User(val name: String, val age: Int)
来源：http://wws.ctjpmb.com

[T09] Kotlin：扩展函数
来源：http://bdm.guannengcc.top

fun String.exclaim() = this + "!"
来源：http://gfi.yj202588.top

[T10] Kotlin：默认参数
来源：http://slk.yonumen.top

fun greet(name: String = "World") = "Hi $name"
来源：http://cpz.mhx1999.top

[T11] Kotlin：协程
来源：http://uct.yonumen.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ppk.chenzaomai.com

[T12] Kotlin：解构声明
来源：http://ncy.uphjek.com

val (a, b) = Pair(1, 2)
来源：http://ykz.bjfxy.top

[T13] Kotlin：只读 Map
来源：http://tec.tarul.cn

val m = mapOf("a" to 1)
来源：http://squ.c1oappe.top

[T14] Kotlin：循环
来源：http://del.yuanzhike.top

for (i in 1..10) println(i)
来源：http://lpi.fanxiaobao.xyz

[T15] Kotlin：接口
来源：http://uwp.cucudq.cn

interface Shape { fun area(): Double }
来源：http://pvy.xingfuxueyuan.xyz

[T16] Swift：Hello World
来源：http://jzi.jiagoushi.top

print("Hello")
来源：http://gif.gotoacloud.top

[T17] Swift：变量与常量
来源：http://eso.smart0.xyz

var a = 1;  let b = 2
来源：http://pcw.cheryme.top

[T18] Swift：字符串插值
来源：http://ufd.hammf.cn

"值: \(b)"
来源：http://upg.ctjpmb.com

[T19] Swift：可选绑定
来源：http://qpr.shanyushiyangkeji.top

if let n = opt { print(n) }
来源：http://fcp.xylfe.cn

[T20] Swift：数组操作
来源：http://ysc.aibaodan.cn

var a = [1, 2, 3];  a.append(4)
来源：http://yps.dashuyun.cn

[T21] Swift：遍历
来源：http://fed.jyoumei.cn

for x in a { print(x) }
来源：http://sjl.hywenlv.cn

[T22] Swift：字典
来源：http://nwv.jqgufenzy.top

var d = ["a": 1];  d["b"] = 2
来源：http://jmx.aibaodan.cn

[T23] Swift：函数
来源：http://mdz.xuanzx.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gei.fzhhl.top

[T24] Swift：闭包
来源：http://sqs.shuidangran.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.uphjek.com

[T25] Swift：结构体
来源：http://ktl.ydzc1.top

struct P { var x: Int }
来源：http://gax.hammf.cn

[T26] Swift：类与重写
来源：http://ogm.yj20258888.top

class A: Base { override func f() {} }
来源：http://rok.nanxuanxn.top

[T27] Swift：错误处理
来源：http://ydh.ivvv.top

do { try f() } catch { print(error) }
来源：http://fzc.cucudq.cn

[T28] Swift：枚举
来源：http://fqr.wangdashe.top

enum Color { case red, green }
来源：http://ogh.shuidangran.top

[T29] Swift：guard 提前返回
来源：http://jvh.daxiang520.top

guard let x = opt else { return }
来源：http://pjk.chenjidiqi.icu

[T30] Swift：协议
来源：http://khz.pycfn.com

protocol Shape { func area() -> Double }
来源：http://tsw.smart0.xyz

[T31] Lua：Hello World
来源：http://rlu.haohaochexian.top

print("Hello")
来源：http://fbf.hnxiangtu.top

[T32] Lua：局部变量
来源：http://rhq.hnqzz.top

local a = 1
来源：http://tsw.jiagoushi.top

[T33] Lua：表（数组）
来源：http://zks.mhx1999.top

local t = {1, 2, 3};  t[4] = 4
来源：http://qtc.jqgfzy.top

[T34] Lua：遍历表
来源：http://ngv.yj20258888.top

for i, v in ipairs(t) do print(i, v) end
来源：http://cup.meibo888.top

[T35] Lua：字典表
来源：http://ykm.gogol.net.cn

local d = { a = 1 };  d.b = 2
来源：http://cyc.sjlbkw.cn

[T36] Lua：函数
来源：http://mjg.yj20258888.top

function add(a, b) return a + b end
来源：http://tbg.cashguo.top

[T37] Lua：字符串拼接
来源：http://hqm.shzxlz.cn

"a" .. "b"
来源：http://sno.hammf.cn

[T38] Lua：条件
来源：http://key.vehdjk.com

if x > 0 then print("正") end
来源：http://xmo.yfazqb.com

[T39] Lua：模式匹配
来源：http://vaf.jqgufenzy.top

string.find(s, "%d+")
来源：http://xgz.ydjk.org.cn

[T40] Lua：元表
来源：http://gkg.guannengcc.top

setmetatable({}, { __index = base })
来源：http://ndf.yj20258.top

[T41] Perl：Hello World
来源：http://hhx.zhiwuduotai.top

print "Hello\n";
来源：http://cox.zhengqikj.top

[T42] Perl：变量类型
来源：http://rzv.xziqi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fes.52xcode.cn

[T43] Perl：字符串插值
来源：http://ohj.ctjpmb.com

"值: $a"
来源：http://syu.shanyushiyangtech.top

[T44] Perl：条件
来源：http://jup.xingfuxueyuan.xyz

if ($a > 0) { print "正"; }
来源：http://gui.cqqwz.cn

[T45] Perl：数组遍历
来源：http://gus.jqgfzy.top

for my $x (@arr) { print $x; }
来源：http://wga.nanxuanxn.top

[T46] Perl：哈希操作
来源：http://ist.ybcxt.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://yez.tianlin.xyz

[T47] Perl：正则捕获
来源：http://ncv.hnxiangtu.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ibu.haohaochexian.top

[T48] Perl：正则替换
来源：http://vtv.meibo888.top

$s =~ s/old/new/g;
来源：http://bzd.uphjek.com

[T49] Perl：函数
来源：http://mts.feifeiyinyue.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://moq.fzhhl.top

[T50] Perl：逐行读文件
来源：http://ibf.gaohongyu789.top

open my $fh, "<", "a.txt" or die $!;
来源：http://qbo.fanxiaobao.xyz

while (my $line = <$fh>) { print $line; }
来源：http://arq.shuidangran.top

[T51] Scala：Hello World
来源：http://rvz.tianlin.xyz

println("Hello")
来源：http://xit.fengsongda.top

[T52] Scala：变量
来源：http://pkz.guowangkeji.top

val a = 1;  var b = 2
来源：http://pnc.xuanzx.com

[T53] Scala：字符串插值
来源：http://kgr.cucudq.cn

s"值: $b"
来源：http://qtt.bbcook.cn

[T54] Scala：集合映射
来源：http://hck.hywenlv.cn

List(1, 2, 3).map(_ * 2)
来源：http://wxp.andypj.xyz

[T55] Scala：集合过滤
来源：http://ftz.birdmap.top

List(1, 2, 3).filter(_ > 1)
来源：http://jun.daria6918.cn

[T56] Scala：样例类
来源：http://nbx.ydzc1.top

case class User(name: String, age: Int)
来源：http://wuj.wangdashe.top

[T57] Scala：模式匹配
来源：http://euh.cdnleiting.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://seq.fehbvm.com

[T58] Scala：函数定义
来源：http://lcz.wangdashe.top

def add(a: Int, b: Int): Int = a + b
来源：http://rwk.xuanzx.com

[T59] Scala：循环
来源：http://lav.ybcxt.top

for (i <- 1 to 10) println(i)
来源：http://geo.cdnleiting.top

[T60] Scala：折叠
来源：http://for.vqdsnc.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://syf.shanyushiyangkeji.top

================================================================================
来源：http://wgf.hywenlv.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vab.c1oappe.top

================================================================================
来源：http://dvd.haohaochexian.top

[U01] Py：创建虚拟环境
来源：http://nsk.daxiang520.top

python -m venv .venv && source .venv/bin/activate
来源：http://szp.xinyue.icu

[U02] Py：导出 / 安装依赖
来源：http://rnf.xingfuxueyuan.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://sdv.hcnkem.com

[U03] Py：加载 .env 配置
来源：http://ehr.tian-w.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://uju.yongpay.top

[U04] Py：变量调试打印
来源：http://apv.zhaomingkeji.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ncr.zhengqikj.top

[U05] Py：列表去重且保序
来源：http://tky.xylfe.cn

list(dict.fromkeys(arr))
来源：http://qfs.shanyushiyangtech.top

[U06] Py：合并两个字典
来源：http://ntf.tianlin.xyz

{**a, **b}
来源：http://edh.hongshengwenyu.top

[U07] Py：反转字典键值
来源：http://wfa.yueranfly.top

{v: k for k, v in d.items()}
来源：http://qrx.cheryme.top

[U08] Py：展平二维列表
来源：http://fnq.316326.xyz

[y for x in nested for y in x]
来源：http://zkx.haohaochexian.top

[U09] Py：字典取最大值的键
来源：http://omz.yueranfly.top

max(d, key=d.get)
来源：http://jst.xuanzx.com

[U10] Py：按值排序字典
来源：http://une.sjlbkw.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://txr.jqgufenzy.top

[U11] Py：生成器表达式
来源：http://jmu.cqqwz.cn

(x * 2 for x in arr)
来源：http://qfw.guannengcc.top

[U12] Py：取出现最多的 3 个元素
来源：http://ecv.vqdsnc.cn

Counter(arr).most_common(3)
来源：http://dkt.ywan-chungtsiang.top

[U13] Py：固定长度队列
来源：http://qpg.jyoumei.cn

deque(maxlen=10)
来源：http://ayc.hcnkem.com

[U14] Py：分组收集到列表
来源：http://fil.epnwcf.com

defaultdict(list)
来源：http://qbs.meibo888.top

[U15] Py：高精度计时
来源：http://xsc.andypj.xyz

t = time.perf_counter()
来源：http://ypg.vqdsnc.cn

[U16] Py：命令行参数解析
来源：http://qhk.zhongyouzk.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cmd.guannengcc.top

[U17] Py：初始化日志
来源：http://cmw.haohaochexian.top

logging.basicConfig(level=logging.INFO)
来源：http://xdb.hysaishi.cn

[U18] Py：预编译正则
来源：http://rca.mhx1999.top

pat = re.compile(r"\d+")
来源：http://lpg.ybcxt.top

[U19] Py：正则替换带回调
来源：http://udv.hesvh.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ila.cdnleiting.top

[U20] Py：缓存函数结果
来源：http://yan.birdmap.top

@functools.lru_cache(maxsize=None)
来源：http://gsl.aibaodan.cn

[U21] Py：自定义上下文管理器
来源：http://doq.yj20258888.top

@contextlib.contextmanager
来源：http://knm.wangshuangyany.cn

[U22] Py：矩阵转置
来源：http://qck.c1oappe.top

list(zip(*m))
来源：http://trs.aibaodan.cn

[U23] Py：分块读取大文件
来源：http://cjj.kuanghao11.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gex.hfpthk.cn

[U24] Py：路径操作
来源：http://itw.kuanghao11.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zto.yonumen.top

[U25] Py：CSV 按字典读
来源：http://qiz.316326.xyz

csv.DictReader(f)
来源：http://xwj.wangshuangyany.cn

[U26] Py：并发下载
来源：http://hlj.xinyue.icu

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://joo.ppjwa.cn

[U27] Py：异步 HTTP
来源：http://msc.ydzc1.top

aiohttp.ClientSession() 配合 async with
来源：http://ech.yj202588.top

[U28] Py：类型别名
来源：http://cps.yanxiufei.cn

UserId = int
来源：http://cbg.daxiang520.top

[U29] Py：属性校验
来源：http://raj.ydjk.org.cn

@property 与 @x.setter 配合
来源：http://gvr.0kj1m.cn

[U30] Py：数据类
来源：http://txg.zhiwuduotai.top

@dataclass(slots=True)
来源：http://pzu.havefunace.top

[U31] Py：单测
来源：http://btt.hnqzz.top

python -m pytest -q
来源：http://jet.zdqjudy.top

[U32] Py：代码格式化
来源：http://czp.hnxiangtu.top

ruff format . && ruff check --fix .
来源：http://nyx.xingfuxueyuan.xyz

[U33] Py：打包发布
来源：http://xsy.nanxuanxn.top

python -m build  （依赖 pyproject.toml）
来源：http://isl.jqgufenzy.top

[U34] Py：判断编码
来源：http://ypf.quarkkingdee.top

chardet.detect(raw)
来源：http://blf.yvedp.cn

[U35] Py：发送邮件
来源：http://zuw.zdbjq.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qhy.9152youxi.cn

[U36] Py：定时任务
来源：http://mkj.hfpthk.cn

schedule.every(10).minutes.do(job)
来源：http://bmt.shangyingyoupin.top

[U37] Py：读写 Excel
来源：http://gvr.tian-w.cn

pandas.read_excel / DataFrame.to_excel
来源：http://lmm.ydjk.org.cn

[U38] Py：获取脚本所在目录
来源：http://huh.cheryme.top

Path(__file__).resolve().parent
来源：http://zay.xuetiantiany.cn

[U39] Py：判断是否在交互环境
来源：http://igt.wangdashe.top

sys.stdout.isatty()
来源：http://eys.mhx1999.top

[U40] Py：打印到标准错误
来源：http://mdc.zhengqikj.top

print("err", file=sys.stderr)
来源：http://bem.zhiwuduotai.top

[U41] PHP：初始化 Composer 项目
来源：http://jyb.0kj1m.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://dex.sweek.top

[U42] PHP：PSR-4 自动加载
来源：http://kha.cucudq.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://kzd.fanxiaobao.xyz

[U43] PHP：声明命名空间
来源：http://iin.cucudq.cn

namespace App\Http;
来源：http://bup.ywan-chungtsiang.top

[U44] PHP：开启严格类型
来源：http://ilq.yuanzhike.top

declare(strict_types=1);
来源：http://gil.fengsongda.top


<!-- 参考信息 -->