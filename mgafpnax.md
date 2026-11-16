代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://myx.sysykeji.top

[S21] C：字符类别判断
来源：http://whx.sjlbkw.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wpu.fktsv.cn

[S22] C：字符串转数字
来源：http://yrb.shangyingyoupin.top

atoi("42");  strtod("3.14", NULL);
来源：http://jdj.cheryme.top

[S23] C：随机数
来源：http://pxa.havefunace.top

srand(time(NULL));  int r = rand() % 100;
来源：http://nlb.316326.xyz

[S24] C：获取本地时间
来源：http://uss.aizwys.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hbc.epnwcf.com

[S25] C：内存拷贝
来源：http://ret.pengpengdd.cyou

memcpy(dst, src, n);
来源：http://xau.yueranfly.top

[S26] C：内存清零
来源：http://fzf.quarkkingdee.top

memset(a, 0, sizeof a);
来源：http://dyg.jinghuilouyu.cn

[S27] C：定义常量
来源：http://jat.zhengqikj.top

const double PI = 3.14159;
来源：http://opp.shanyushiyangtech.top

[S28] C：静态变量
来源：http://zqh.shanyushiyangtech.top

static int counter = 0;
来源：http://iak.redwolf501.top

[S29] C：变参函数
来源：http://mfm.yuanzhike.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rus.yueranfly.top

[S30] C：头文件保护
来源：http://gnk.cheryme.top

#ifndef X_H
来源：http://jbj.nwbrower.top

#define X_H
来源：http://ahk.sweek.top

#endif
来源：http://xct.jqgufenzy.top

[S31] C++：Hello World
来源：http://yma.redwolf501.top

#include <iostream>
来源：http://rxq.hesvh.cn

int main() { std::cout << "Hello\n"; }
来源：http://hby.jinqigfzy.top

[S32] C++：字符串
来源：http://nym.zhiwuduotai.top

std::string s = "hi";  s += "!";
来源：http://ecl.c1oappe.top

[S33] C++：vector 增删
来源：http://mym.dianchejie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pun.jinghuilouyu.cn

[S34] C++：遍历 vector
来源：http://pmh.yfazqb.com

for (auto &x : v) { std::cout << x; }
来源：http://ufk.tanke756.top

[S35] C++：map
来源：http://jzj.vehdjk.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wtl.guowangkeji.top

[S36] C++：unordered_map
来源：http://hbq.guannengcc.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kmj.fehbvm.com

[S37] C++：set
来源：http://ctw.zhengqikj.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://omu.dashuyun.cn

[S38] C++：排序
来源：http://qox.xuetiantiany.cn

std::sort(v.begin(), v.end());
来源：http://tui.cheryme.top

[S39] C++：自定义比较器排序
来源：http://nlg.guowangkeji.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://npx.cdnleiting.top

[S40] C++：查找元素
来源：http://ddu.tian-w.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hvx.gogol.net.cn

[S41] C++：类与构造函数
来源：http://obf.fanxiaobao.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fei.fanxiaobao.xyz

[S42] C++：继承与虚函数
来源：http://cak.yj20258888.top

class B : public Base { public: void f() override {} };
来源：http://omk.haohaochexian.top

[S43] C++：智能指针
来源：http://soz.gogol.net.cn

auto p = std::make_unique<int>(5);
来源：http://wsu.chenlongwang.top

[S44] C++：引用传参
来源：http://hlt.hnqzz.top

void inc(int &x) { ++x; }
来源：http://tlx.zycfv.cn

[S45] C++：lambda
来源：http://ygw.zhiwuduotai.top

auto add = [](int a, int b) { return a + b; };
来源：http://jjk.zhoulong.xyz

[S46] C++：函数模板
来源：http://fnk.feifeiyinyue.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://oco.zhongyouzk.top

[S47] C++：结构化绑定遍历
来源：http://gvd.fehbvm.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://sff.mhx1999.top

[S48] C++：逐行读文件
来源：http://cvw.fengsongda.top

std::ifstream in("a.txt");  std::string line;
来源：http://ckh.zhijiandao.cn

while (std::getline(in, line)) { }
来源：http://kwo.zdqjudy.top

[S49] C++：写文件
来源：http://jkn.ivvv.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dzq.zhaomingkeji.xyz

[S50] C++：格式化数字
来源：http://urn.jianghu66.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bfs.zhoulong.xyz

[S51] C++：显式类型转换
来源：http://hmz.jinghuilouyu.cn

static_cast<double>(a) / b
来源：http://adk.hongshengwenyu.top

[S52] C++：const 与 noexcept
来源：http://zce.birdmap.top

int size() const noexcept { return n_; }
来源：http://nkq.zhaomingkeji.xyz

[S53] C++：移动语义
来源：http://sda.jinqigfzy.top

std::vector<int> w = std::move(v);
来源：http://rve.redwolf501.top

[S54] C++：异常处理
来源：http://vju.ydzc1.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tix.zycfv.cn

[S55] C++：结构化绑定
来源：http://atu.yangfankeji.com

auto [a, b] = std::make_pair(1, 2);
来源：http://djt.chenjidiqi.icu

[S56] C++：optional
来源：http://awy.iojbl.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jmj.zycfv.cn

[S57] C++：编译期常量
来源：http://mkp.fengsongda.top

constexpr int N = 10;
来源：http://flc.jinyuanbaomall.cn

[S58] C++：命名空间
来源：http://uvi.zhijiandao.cn

namespace ns { int f() { return 1; } }
来源：http://plk.zdbjq.cn

[S59] C++：静态断言
来源：http://kol.smart0.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qmd.shanyushiyangkeji.top

[S60] C++：遍历并删除元素
来源：http://igo.cashguo.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cci.316326.xyz

================================================================================
来源：http://tqa.hammf.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lpm.xuanzx.com

================================================================================
来源：http://qsl.aizwys.cn

[T01] Kotlin：Hello World
来源：http://wvs.jyoumei.cn

println("Hello")
来源：http://iyn.yj20258.top

[T02] Kotlin：变量
来源：http://eqn.haohaochexian.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zfz.yj20258888.top

[T03] Kotlin：字符串模板
来源：http://izr.zycfv.cn

"值: $b"
来源：http://imf.yuxming.cn

[T04] Kotlin：空安全
来源：http://lda.xinyue.icu

val n: String? = null;  n?.length
来源：http://wpy.nanxuanxn.top

[T05] Kotlin：when 表达式
来源：http://hll.cdnleiting.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jln.yj202588.top

[T06] Kotlin：集合映射
来源：http://sgt.bbcook.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://gpx.nwbrower.top

[T07] Kotlin：集合过滤
来源：http://qro.cucudq.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ipf.havefunace.top

[T08] Kotlin：数据类
来源：http://tye.ppjwa.cn

data class User(val name: String, val age: Int)
来源：http://axu.pycfn.com

[T09] Kotlin：扩展函数
来源：http://ybi.jiagoushi.top

fun String.exclaim() = this + "!"
来源：http://prz.nanxuanxn.top

[T10] Kotlin：默认参数
来源：http://wew.zhengqikj.top

fun greet(name: String = "World") = "Hi $name"
来源：http://nox.yuxming.cn

[T11] Kotlin：协程
来源：http://cyj.chenzaomai.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://dyc.yuanzhike.top

[T12] Kotlin：解构声明
来源：http://mjw.jinyuanbaomall.cn

val (a, b) = Pair(1, 2)
来源：http://box.jiagoushi.top

[T13] Kotlin：只读 Map
来源：http://pbj.ehwqpu.com

val m = mapOf("a" to 1)
来源：http://xma.xinyue.icu

[T14] Kotlin：循环
来源：http://wqn.yvedp.cn

for (i in 1..10) println(i)
来源：http://chg.yj202588.top

[T15] Kotlin：接口
来源：http://ubv.wangdashe.top

interface Shape { fun area(): Double }
来源：http://ksa.mhx1999.top

[T16] Swift：Hello World
来源：http://kom.xuanzx.com

print("Hello")
来源：http://fbo.xuanzx.com

[T17] Swift：变量与常量
来源：http://lnf.sysykeji.top

var a = 1;  let b = 2
来源：http://vkw.hcnkem.com

[T18] Swift：字符串插值
来源：http://uhp.zhiwuduotai.top

"值: \(b)"
来源：http://qan.hysaishi.cn

[T19] Swift：可选绑定
来源：http://ssx.fzhhl.top

if let n = opt { print(n) }
来源：http://sqt.bbcook.cn

[T20] Swift：数组操作
来源：http://ksi.zhengqikj.top

var a = [1, 2, 3];  a.append(4)
来源：http://rxx.bjfxy.top

[T21] Swift：遍历
来源：http://boc.zhongyouzk.top

for x in a { print(x) }
来源：http://uod.nanxuanxn.top

[T22] Swift：字典
来源：http://xcy.xylfe.cn

var d = ["a": 1];  d["b"] = 2
来源：http://mqq.jqgfzy.top

[T23] Swift：函数
来源：http://wvw.wangdashe.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wnq.gzhubu.top

[T24] Swift：闭包
来源：http://htl.hfpthk.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://hxt.shanyushiyangtech.top

[T25] Swift：结构体
来源：http://xkp.zhengqikj.top

struct P { var x: Int }
来源：http://dpl.hfpthk.cn

[T26] Swift：类与重写
来源：http://cwo.fengsongda.top

class A: Base { override func f() {} }
来源：http://spj.fehbvm.com

[T27] Swift：错误处理
来源：http://uqw.sxryk.cn

do { try f() } catch { print(error) }
来源：http://qie.jinqigufen.top

[T28] Swift：枚举
来源：http://flu.kuanghao11.cn

enum Color { case red, green }
来源：http://mjv.gogol.net.cn

[T29] Swift：guard 提前返回
来源：http://mmy.gotoacloud.top

guard let x = opt else { return }
来源：http://lwa.yueranfly.top

[T30] Swift：协议
来源：http://xqd.daria6918.cn

protocol Shape { func area() -> Double }
来源：http://fpg.jinqigfzy.top

[T31] Lua：Hello World
来源：http://wwr.vqdsnc.cn

print("Hello")
来源：http://qmy.hywenlv.cn

[T32] Lua：局部变量
来源：http://ykk.zhijiandao.cn

local a = 1
来源：http://yqe.wangshuangyany.cn

[T33] Lua：表（数组）
来源：http://axc.sweek.top

local t = {1, 2, 3};  t[4] = 4
来源：http://fak.tianlin.xyz

[T34] Lua：遍历表
来源：http://zkv.hysaishi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://exo.hfpthk.cn

[T35] Lua：字典表
来源：http://uxu.zhiwuduotai.top

local d = { a = 1 };  d.b = 2
来源：http://gwx.yuanzhike.top

[T36] Lua：函数
来源：http://zrj.birdmap.top

function add(a, b) return a + b end
来源：http://qdr.vqdsnc.cn

[T37] Lua：字符串拼接
来源：http://sxc.cucudq.cn

"a" .. "b"
来源：http://ghs.xingfuxueyuan.xyz

[T38] Lua：条件
来源：http://mly.wangdashe.top

if x > 0 then print("正") end
来源：http://vcq.jyoumei.cn

[T39] Lua：模式匹配
来源：http://eqj.hcnkem.com

string.find(s, "%d+")
来源：http://jdo.ehwqpu.com

[T40] Lua：元表
来源：http://csl.hnxiangtu.top

setmetatable({}, { __index = base })
来源：http://zbd.fengsongda.top

[T41] Perl：Hello World
来源：http://plo.quarkkingdee.top

print "Hello\n";
来源：http://tai.epnwcf.com

[T42] Perl：变量类型
来源：http://wzn.cashguo.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wca.xinyue.icu

[T43] Perl：字符串插值
来源：http://ytg.ctjpmb.com

"值: $a"
来源：http://gft.zhixingplan.top

[T44] Perl：条件
来源：http://qgt.meibo888.top

if ($a > 0) { print "正"; }
来源：http://yqz.xylfe.cn

[T45] Perl：数组遍历
来源：http://ecy.zhongyouzk.top

for my $x (@arr) { print $x; }
来源：http://ahp.tanke756.top

[T46] Perl：哈希操作
来源：http://lln.redwolf501.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ocl.hfpthk.cn

[T47] Perl：正则捕获
来源：http://hbo.zdqjudy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://tih.ivvv.top

[T48] Perl：正则替换
来源：http://wwt.hongshengwenyu.top

$s =~ s/old/new/g;
来源：http://pnn.cqqwz.cn

[T49] Perl：函数
来源：http://kiw.zhijiandao.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rmq.0kj1m.cn

[T50] Perl：逐行读文件
来源：http://vfs.yangfankeji.com

open my $fh, "<", "a.txt" or die $!;
来源：http://moj.andypj.xyz

while (my $line = <$fh>) { print $line; }
来源：http://scp.shuidangran.top

[T51] Scala：Hello World
来源：http://fep.aizwys.cn

println("Hello")
来源：http://kww.yuanzhike.top

[T52] Scala：变量
来源：http://lec.hfpthk.cn

val a = 1;  var b = 2
来源：http://hem.hongshengwenyu.top

[T53] Scala：字符串插值
来源：http://slu.shangyingyoupin.top

s"值: $b"
来源：http://iuy.sysykeji.top

[T54] Scala：集合映射
来源：http://xbh.wangshuangyany.cn

List(1, 2, 3).map(_ * 2)
来源：http://tqd.52xcode.cn

[T55] Scala：集合过滤
来源：http://lni.cucudq.cn

List(1, 2, 3).filter(_ > 1)
来源：http://bik.chenjidiqi.icu

[T56] Scala：样例类
来源：http://nbi.zdbjq.cn

case class User(name: String, age: Int)
来源：http://lml.sjlbkw.cn

[T57] Scala：模式匹配
来源：http://yxk.ivvv.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://lqe.kuanghao11.cn

[T58] Scala：函数定义
来源：http://acf.jyoumei.cn

def add(a: Int, b: Int): Int = a + b
来源：http://gxl.vqdsnc.cn

[T59] Scala：循环
来源：http://vko.svipenyu.cn

for (i <- 1 to 10) println(i)
来源：http://ldy.bbcook.cn

[T60] Scala：折叠
来源：http://ror.cdnleiting.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wwo.9152youxi.cn

================================================================================
来源：http://ywg.xziqi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rry.shanyushiyangkeji.top

================================================================================
来源：http://nnu.zhengqikj.top

[U01] Py：创建虚拟环境
来源：http://nap.pengpengdd.cyou

python -m venv .venv && source .venv/bin/activate
来源：http://kjh.wangshuangyany.cn

[U02] Py：导出 / 安装依赖
来源：http://cfl.jinqigufen.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gom.jinyuanbaomall.cn

[U03] Py：加载 .env 配置
来源：http://jcl.yj20258.top

from dotenv import load_dotenv; load_dotenv()
来源：http://tco.zhixingplan.top

[U04] Py：变量调试打印
来源：http://tcj.xuanzx.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bmq.pengpengdd.cyou

[U05] Py：列表去重且保序
来源：http://nfn.chenjidiqi.icu

list(dict.fromkeys(arr))
来源：http://tpp.uphjek.com

[U06] Py：合并两个字典
来源：http://rrs.jlsjyb.cn

{**a, **b}
来源：http://cuw.chenlongwang.top

[U07] Py：反转字典键值
来源：http://jpr.jqgufenzy.top

{v: k for k, v in d.items()}
来源：http://ioy.gaohongyu789.top

[U08] Py：展平二维列表
来源：http://maz.pengpengdd.cyou

[y for x in nested for y in x]
来源：http://mtt.nanxuanxn.top

[U09] Py：字典取最大值的键
来源：http://iwh.vehdjk.com

max(d, key=d.get)
来源：http://ywy.cucudq.cn

[U10] Py：按值排序字典
来源：http://fig.aizwys.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jnn.ywan-chungtsiang.top

[U11] Py：生成器表达式
来源：http://dhz.hnxiangtu.top

(x * 2 for x in arr)
来源：http://eoi.fehbvm.com

[U12] Py：取出现最多的 3 个元素
来源：http://jwd.daxiang520.top

Counter(arr).most_common(3)
来源：http://eny.ctjpmb.com

[U13] Py：固定长度队列
来源：http://uxr.zhiwuduotai.top

deque(maxlen=10)
来源：http://sdz.yongpay.top

[U14] Py：分组收集到列表
来源：http://kdl.aizwys.cn

defaultdict(list)
来源：http://yfz.ivvv.top

[U15] Py：高精度计时
来源：http://rdj.hywenlv.cn

t = time.perf_counter()
来源：http://zkj.fengsongda.top

[U16] Py：命令行参数解析
来源：http://vcn.tanke756.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://exu.cheryme.top

[U17] Py：初始化日志
来源：http://qso.bjfxy.top

logging.basicConfig(level=logging.INFO)
来源：http://nkw.nanxinkj.top

[U18] Py：预编译正则
来源：http://imd.redwolf501.top

pat = re.compile(r"\d+")
来源：http://rws.uphjek.com

[U19] Py：正则替换带回调
来源：http://eut.yvedp.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://odz.sufxvd.cn

[U20] Py：缓存函数结果
来源：http://nat.uphjek.com

@functools.lru_cache(maxsize=None)
来源：http://pei.yonumen.top

[U21] Py：自定义上下文管理器
来源：http://xka.dianchejie.cn

@contextlib.contextmanager
来源：http://bgr.gotoacloud.top

[U22] Py：矩阵转置
来源：http://wnf.hfpthk.cn

list(zip(*m))
来源：http://qoy.shanyushiyangtech.top

[U23] Py：分块读取大文件
来源：http://njm.kuanghao11.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hlp.gzhubu.top

[U24] Py：路径操作
来源：http://zvf.316326.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ygn.dashuyun.cn

[U25] Py：CSV 按字典读
来源：http://fjf.sjlbkw.cn

csv.DictReader(f)
来源：http://gak.fengsongda.top

[U26] Py：并发下载
来源：http://xym.sxryk.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://kvm.vqdsnc.cn

[U27] Py：异步 HTTP
来源：http://gud.yfazqb.com

aiohttp.ClientSession() 配合 async with
来源：http://dtu.0kj1m.cn

[U28] Py：类型别名
来源：http://zyu.meibo888.top

UserId = int
来源：http://rno.xuetiantiany.cn

[U29] Py：属性校验
来源：http://fqx.sweek.top

@property 与 @x.setter 配合
来源：http://otn.zdbjq.cn

[U30] Py：数据类
来源：http://ukg.svipenyu.cn

@dataclass(slots=True)
来源：http://bym.chenzaomai.com

[U31] Py：单测
来源：http://bfw.fktsv.cn

python -m pytest -q
来源：http://syc.ywan-chungtsiang.top

[U32] Py：代码格式化
来源：http://zli.tarul.cn

ruff format . && ruff check --fix .
来源：http://lio.9152youxi.cn

[U33] Py：打包发布
来源：http://cmp.gotoacloud.top

python -m build  （依赖 pyproject.toml）
来源：http://msv.hywenlv.cn

[U34] Py：判断编码
来源：http://wuk.nwbrower.top

chardet.detect(raw)
来源：http://prr.pengpengdd.cyou

[U35] Py：发送邮件
来源：http://joe.uphjek.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://huj.yvedp.cn

[U36] Py：定时任务
来源：http://srt.ywan-chungtsiang.top

schedule.every(10).minutes.do(job)
来源：http://iwo.meibo888.top

[U37] Py：读写 Excel
来源：http://rxz.birdmap.top

pandas.read_excel / DataFrame.to_excel
来源：http://gxy.chenlongwang.top

[U38] Py：获取脚本所在目录
来源：http://qqf.hnqzz.top

Path(__file__).resolve().parent
来源：http://vim.jiagoushi.top

[U39] Py：判断是否在交互环境
来源：http://gsa.zhixingplan.top

sys.stdout.isatty()
来源：http://fnh.nanxuanxn.top

[U40] Py：打印到标准错误
来源：http://qza.pycfn.com

print("err", file=sys.stderr)
来源：http://ghq.zhongyouzk.top

[U41] PHP：初始化 Composer 项目
来源：http://tzo.ydzc1.top

composer init;  composer require guzzlehttp/guzzle
来源：http://neb.fehbvm.com

[U42] PHP：PSR-4 自动加载
来源：http://ouh.uphjek.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qcm.haohaochexian.top

[U43] PHP：声明命名空间
来源：http://heg.xuetiantiany.cn

namespace App\Http;
来源：http://bbk.xingfuxueyuan.xyz

[U44] PHP：开启严格类型
来源：http://szs.pycfn.com

declare(strict_types=1);
来源：http://wxa.jinqigufen.top


<!-- 参考信息 -->