代发 wailian999

int main(int argc, char **argv)
来源：http://tvx.yj20258.top

[S19] C：快速排序
来源：http://dil.zdqjudy.top

qsort(a, n, sizeof(int), cmp);
来源：http://atv.hysaishi.cn

[S20] C：二分查找
来源：http://bac.jyoumei.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fxh.hfpthk.cn

[S21] C：字符类别判断
来源：http://osz.ehwqpu.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zoo.shuidangran.top

[S22] C：字符串转数字
来源：http://bbq.ctjpmb.com

atoi("42");  strtod("3.14", NULL);
来源：http://tee.kuanghao11.cn

[S23] C：随机数
来源：http://htk.jqgufenzy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ukf.kuanghao11.cn

[S24] C：获取本地时间
来源：http://wrz.yonumen.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tse.zdbjq.cn

[S25] C：内存拷贝
来源：http://sat.shangyingyoupin.top

memcpy(dst, src, n);
来源：http://lvl.yanxiufei.cn

[S26] C：内存清零
来源：http://xjp.yonumen.top

memset(a, 0, sizeof a);
来源：http://rma.tian-w.cn

[S27] C：定义常量
来源：http://hgn.jyoumei.cn

const double PI = 3.14159;
来源：http://dql.hcnkem.com

[S28] C：静态变量
来源：http://yhl.bbcook.cn

static int counter = 0;
来源：http://ppp.fzhhl.top

[S29] C：变参函数
来源：http://vxm.zhijiandao.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://apc.jinqigufen.top

[S30] C：头文件保护
来源：http://ukb.hongshengwenyu.top

#ifndef X_H
来源：http://gdx.c1oappe.top

#define X_H
来源：http://hud.snrcjt.cn

#endif
来源：http://neo.nanxuanxn.top

[S31] C++：Hello World
来源：http://uyw.tian-w.cn

#include <iostream>
来源：http://svz.fktsv.cn

int main() { std::cout << "Hello\n"; }
来源：http://nug.shanyushiyangtech.top

[S32] C++：字符串
来源：http://jmz.yonumen.top

std::string s = "hi";  s += "!";
来源：http://cxd.nwbrower.top

[S33] C++：vector 增删
来源：http://qtl.316326.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gnn.haohaochexian.top

[S34] C++：遍历 vector
来源：http://ngb.sufxvd.cn

for (auto &x : v) { std::cout << x; }
来源：http://crs.yj202588.top

[S35] C++：map
来源：http://nig.zhixingplan.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vfm.jqgfzy.top

[S36] C++：unordered_map
来源：http://lvu.xuanzx.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rhq.shuidangran.top

[S37] C++：set
来源：http://qjg.yfazqb.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zeq.hnqzz.top

[S38] C++：排序
来源：http://knz.sxryk.cn

std::sort(v.begin(), v.end());
来源：http://trb.feifeiyinyue.top

[S39] C++：自定义比较器排序
来源：http://asl.chenzaomai.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bhx.hcnkem.com

[S40] C++：查找元素
来源：http://zgf.zhijiandao.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uyi.dianchejie.cn

[S41] C++：类与构造函数
来源：http://ccg.xuetiantiany.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://may.hfpthk.cn

[S42] C++：继承与虚函数
来源：http://xgd.jlsjyb.cn

class B : public Base { public: void f() override {} };
来源：http://scz.iojbl.cn

[S43] C++：智能指针
来源：http://ier.tian-w.cn

auto p = std::make_unique<int>(5);
来源：http://son.ywan-chungtsiang.top

[S44] C++：引用传参
来源：http://cel.52xcode.cn

void inc(int &x) { ++x; }
来源：http://oxe.ywan-chungtsiang.top

[S45] C++：lambda
来源：http://eyf.tanke756.top

auto add = [](int a, int b) { return a + b; };
来源：http://ivy.ctjpmb.com

[S46] C++：函数模板
来源：http://bzv.yj20258.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qgz.guannengcc.top

[S47] C++：结构化绑定遍历
来源：http://exy.guowangkeji.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://msn.wangshuangyany.cn

[S48] C++：逐行读文件
来源：http://tls.cashguo.top

std::ifstream in("a.txt");  std::string line;
来源：http://sja.nwbrower.top

while (std::getline(in, line)) { }
来源：http://whb.wangshuangyany.cn

[S49] C++：写文件
来源：http://aje.daria6918.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fiu.ydjk.org.cn

[S50] C++：格式化数字
来源：http://uys.hysaishi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tnr.jianghu66.top

[S51] C++：显式类型转换
来源：http://wqv.ywan-chungtsiang.top

static_cast<double>(a) / b
来源：http://xaw.ybcxt.top

[S52] C++：const 与 noexcept
来源：http://loc.shangyingyoupin.top

int size() const noexcept { return n_; }
来源：http://vhj.jinqigufen.top

[S53] C++：移动语义
来源：http://cwi.yuxming.cn

std::vector<int> w = std::move(v);
来源：http://jtc.hammf.cn

[S54] C++：异常处理
来源：http://meg.kuanghao11.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lrj.birdmap.top

[S55] C++：结构化绑定
来源：http://fot.jqgfzy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://hrq.yuxming.cn

[S56] C++：optional
来源：http://eca.zhoulong.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wtc.andypj.xyz

[S57] C++：编译期常量
来源：http://vlg.ydjk.org.cn

constexpr int N = 10;
来源：http://jpy.ydjk.org.cn

[S58] C++：命名空间
来源：http://lpx.yangfankeji.com

namespace ns { int f() { return 1; } }
来源：http://fao.hcnkem.com

[S59] C++：静态断言
来源：http://gkr.dianchejie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://njx.kuanghao11.cn

[S60] C++：遍历并删除元素
来源：http://vbo.ivvv.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ngj.jianghu66.top

================================================================================
来源：http://zcy.yuanzhike.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fjr.hnqzz.top

================================================================================
来源：http://yho.yanxiufei.cn

[T01] Kotlin：Hello World
来源：http://mor.daxiang520.top

println("Hello")
来源：http://iky.nanxuanxn.top

[T02] Kotlin：变量
来源：http://bof.sysykeji.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yfa.jyoumei.cn

[T03] Kotlin：字符串模板
来源：http://ssw.uphjek.com

"值: $b"
来源：http://oga.zhengqikj.top

[T04] Kotlin：空安全
来源：http://egk.hfpthk.cn

val n: String? = null;  n?.length
来源：http://qyn.hysaishi.cn

[T05] Kotlin：when 表达式
来源：http://nxo.quarkkingdee.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ary.birdmap.top

[T06] Kotlin：集合映射
来源：http://rdf.sufxvd.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://swq.mhx1999.top

[T07] Kotlin：集合过滤
来源：http://hkw.redwolf501.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://rku.hnqzz.top

[T08] Kotlin：数据类
来源：http://zoc.gogol.net.cn

data class User(val name: String, val age: Int)
来源：http://kmr.birdmap.top

[T09] Kotlin：扩展函数
来源：http://pcf.dashuyun.cn

fun String.exclaim() = this + "!"
来源：http://qgl.zhaomingkeji.xyz

[T10] Kotlin：默认参数
来源：http://kqw.sufxvd.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://eqi.wangdashe.top

[T11] Kotlin：协程
来源：http://rcg.shanyushiyangkeji.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://erc.9152youxi.cn

[T12] Kotlin：解构声明
来源：http://xle.jianghu66.top

val (a, b) = Pair(1, 2)
来源：http://ipe.zdqjudy.top

[T13] Kotlin：只读 Map
来源：http://cbs.pycfn.com

val m = mapOf("a" to 1)
来源：http://evr.ctjpmb.com

[T14] Kotlin：循环
来源：http://qcy.jinqigufen.top

for (i in 1..10) println(i)
来源：http://eiq.jqgufenzy.top

[T15] Kotlin：接口
来源：http://jqz.snrcjt.cn

interface Shape { fun area(): Double }
来源：http://oeo.xingfuxueyuan.xyz

[T16] Swift：Hello World
来源：http://xit.meibo888.top

print("Hello")
来源：http://fwo.0kj1m.cn

[T17] Swift：变量与常量
来源：http://bhm.vehdjk.com

var a = 1;  let b = 2
来源：http://eyo.epnwcf.com

[T18] Swift：字符串插值
来源：http://daq.gotoacloud.top

"值: \(b)"
来源：http://rhr.yongpay.top

[T19] Swift：可选绑定
来源：http://ymj.havefunace.top

if let n = opt { print(n) }
来源：http://gfo.birdmap.top

[T20] Swift：数组操作
来源：http://tfi.jiagoushi.top

var a = [1, 2, 3];  a.append(4)
来源：http://lzr.cucudq.cn

[T21] Swift：遍历
来源：http://xeh.ydzc1.top

for x in a { print(x) }
来源：http://adv.zhongyouzk.top

[T22] Swift：字典
来源：http://ewc.zhengqikj.top

var d = ["a": 1];  d["b"] = 2
来源：http://nne.jinqigufen.top

[T23] Swift：函数
来源：http://mck.dianchejie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://avw.feifeiyinyue.top

[T24] Swift：闭包
来源：http://mqm.gaohongyu789.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://evr.zdbjq.cn

[T25] Swift：结构体
来源：http://gal.jinqigfzy.top

struct P { var x: Int }
来源：http://wws.svipenyu.cn

[T26] Swift：类与重写
来源：http://koh.andypj.xyz

class A: Base { override func f() {} }
来源：http://nqx.ehwqpu.com

[T27] Swift：错误处理
来源：http://vpq.vehdjk.com

do { try f() } catch { print(error) }
来源：http://hum.tanke756.top

[T28] Swift：枚举
来源：http://azc.ywan-chungtsiang.top

enum Color { case red, green }
来源：http://ieg.jqgfzy.top

[T29] Swift：guard 提前返回
来源：http://avt.zhongyouzk.top

guard let x = opt else { return }
来源：http://atu.daxiang520.top

[T30] Swift：协议
来源：http://uxr.9152youxi.cn

protocol Shape { func area() -> Double }
来源：http://jzx.zhongyouzk.top

[T31] Lua：Hello World
来源：http://thf.haohaochexian.top

print("Hello")
来源：http://usp.hnqzz.top

[T32] Lua：局部变量
来源：http://yyu.zdqjudy.top

local a = 1
来源：http://dql.c1oappe.top

[T33] Lua：表（数组）
来源：http://ltw.tian-w.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://zgx.jinyuanbaomall.cn

[T34] Lua：遍历表
来源：http://ijq.jiagoushi.top

for i, v in ipairs(t) do print(i, v) end
来源：http://gns.wangshuangyany.cn

[T35] Lua：字典表
来源：http://fjt.hnqzz.top

local d = { a = 1 };  d.b = 2
来源：http://jnp.cdnleiting.top

[T36] Lua：函数
来源：http://txz.vqdsnc.cn

function add(a, b) return a + b end
来源：http://xjg.guowangkeji.top

[T37] Lua：字符串拼接
来源：http://pmn.yangfankeji.com

"a" .. "b"
来源：http://yjf.hfpthk.cn

[T38] Lua：条件
来源：http://ejw.jiagoushi.top

if x > 0 then print("正") end
来源：http://dko.xylfe.cn

[T39] Lua：模式匹配
来源：http://sdh.cucudq.cn

string.find(s, "%d+")
来源：http://zro.mhx1999.top

[T40] Lua：元表
来源：http://zbm.havefunace.top

setmetatable({}, { __index = base })
来源：http://emj.shanyushiyangtech.top

[T41] Perl：Hello World
来源：http://qbc.fzhhl.top

print "Hello\n";
来源：http://bey.jianghu66.top

[T42] Perl：变量类型
来源：http://vou.jinghuilouyu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dju.nanxinkj.top

[T43] Perl：字符串插值
来源：http://ddr.ydjk.org.cn

"值: $a"
来源：http://tvl.kuanghao11.cn

[T44] Perl：条件
来源：http://xuk.tianlin.xyz

if ($a > 0) { print "正"; }
来源：http://vxh.9152youxi.cn

[T45] Perl：数组遍历
来源：http://ehh.yj20258888.top

for my $x (@arr) { print $x; }
来源：http://xqb.tianlin.xyz

[T46] Perl：哈希操作
来源：http://nrd.jianghu66.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://joc.zhengqikj.top

[T47] Perl：正则捕获
来源：http://xja.fktsv.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://irt.ybcxt.top

[T48] Perl：正则替换
来源：http://hqy.jiagoushi.top

$s =~ s/old/new/g;
来源：http://tuv.wangdashe.top

[T49] Perl：函数
来源：http://xab.jinqigfzy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hos.zdbjq.cn

[T50] Perl：逐行读文件
来源：http://cig.zhoulong.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://fuf.snrcjt.cn

while (my $line = <$fh>) { print $line; }
来源：http://tse.hongshengwenyu.top

[T51] Scala：Hello World
来源：http://mdn.jinyuanbaomall.cn

println("Hello")
来源：http://fbi.sjlbkw.cn

[T52] Scala：变量
来源：http://djy.ppjwa.cn

val a = 1;  var b = 2
来源：http://mjv.zhiwuduotai.top

[T53] Scala：字符串插值
来源：http://vnj.nanxuanxn.top

s"值: $b"
来源：http://lnz.cashguo.top

[T54] Scala：集合映射
来源：http://glm.zdqjudy.top

List(1, 2, 3).map(_ * 2)
来源：http://wll.cashguo.top

[T55] Scala：集合过滤
来源：http://emp.hammf.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ckf.dashuyun.cn

[T56] Scala：样例类
来源：http://lyb.dashuyun.cn

case class User(name: String, age: Int)
来源：http://alr.ydjk.org.cn

[T57] Scala：模式匹配
来源：http://nmv.yuanzhike.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://xvp.tian-w.cn

[T58] Scala：函数定义
来源：http://ifd.chenlongwang.top

def add(a: Int, b: Int): Int = a + b
来源：http://jrg.jinqigufen.top

[T59] Scala：循环
来源：http://inu.mhx1999.top

for (i <- 1 to 10) println(i)
来源：http://wiw.jinghuilouyu.cn

[T60] Scala：折叠
来源：http://sdl.meibo888.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://oez.yuxming.cn

================================================================================
来源：http://jjg.daxiang520.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://iii.jqgfzy.top

================================================================================
来源：http://oad.aibaodan.cn

[U01] Py：创建虚拟环境
来源：http://qdl.jianghu66.top

python -m venv .venv && source .venv/bin/activate
来源：http://mvy.fktsv.cn

[U02] Py：导出 / 安装依赖
来源：http://app.pengpengdd.cyou

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ahz.sweek.top

[U03] Py：加载 .env 配置
来源：http://zkr.jinghuilouyu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://cbu.yueranfly.top

[U04] Py：变量调试打印
来源：http://eho.nanxuanxn.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://tnu.hywenlv.cn

[U05] Py：列表去重且保序
来源：http://uta.fehbvm.com

list(dict.fromkeys(arr))
来源：http://pol.smart0.xyz

[U06] Py：合并两个字典
来源：http://zte.hnxiangtu.top

{**a, **b}
来源：http://cln.zhijiandao.cn

[U07] Py：反转字典键值
来源：http://vmx.hnxiangtu.top

{v: k for k, v in d.items()}
来源：http://cdx.9152youxi.cn

[U08] Py：展平二维列表
来源：http://fcx.hesvh.cn

[y for x in nested for y in x]
来源：http://jtl.xylfe.cn

[U09] Py：字典取最大值的键
来源：http://vix.jyoumei.cn

max(d, key=d.get)
来源：http://nsw.jinghuilouyu.cn

[U10] Py：按值排序字典
来源：http://cbx.vehdjk.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kht.jianghu66.top

[U11] Py：生成器表达式
来源：http://noj.yonumen.top

(x * 2 for x in arr)
来源：http://zgb.gzhubu.top

[U12] Py：取出现最多的 3 个元素
来源：http://nza.tarul.cn

Counter(arr).most_common(3)
来源：http://lhh.jinyuanbaomall.cn

[U13] Py：固定长度队列
来源：http://our.ppjwa.cn

deque(maxlen=10)
来源：http://pdl.jianghu66.top

[U14] Py：分组收集到列表
来源：http://rau.shzxlz.cn

defaultdict(list)
来源：http://tju.gotoacloud.top

[U15] Py：高精度计时
来源：http://joq.tanke756.top

t = time.perf_counter()
来源：http://tqp.cheryme.top

[U16] Py：命令行参数解析
来源：http://mhb.shzxlz.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qzn.316326.xyz

[U17] Py：初始化日志
来源：http://txo.ehwqpu.com

logging.basicConfig(level=logging.INFO)
来源：http://bdr.hammf.cn

[U18] Py：预编译正则
来源：http://aue.daria6918.cn

pat = re.compile(r"\d+")
来源：http://ipn.ivvv.top

[U19] Py：正则替换带回调
来源：http://whn.fanxiaobao.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fwo.hcnkem.com

[U20] Py：缓存函数结果
来源：http://ato.svipenyu.cn

@functools.lru_cache(maxsize=None)
来源：http://unc.aizwys.cn

[U21] Py：自定义上下文管理器
来源：http://ceg.ctjpmb.com

@contextlib.contextmanager
来源：http://xll.jqgfzy.top

[U22] Py：矩阵转置
来源：http://bxn.birdmap.top

list(zip(*m))
来源：http://uim.zhongyouzk.top

[U23] Py：分块读取大文件
来源：http://yxy.bbcook.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hkw.havefunace.top

[U24] Py：路径操作
来源：http://pyh.yj202588.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://osh.bbcook.cn

[U25] Py：CSV 按字典读
来源：http://fek.jyoumei.cn

csv.DictReader(f)
来源：http://ruv.9152youxi.cn

[U26] Py：并发下载
来源：http://acy.jiagoushi.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ypv.snrcjt.cn

[U27] Py：异步 HTTP
来源：http://bqz.shzxlz.cn

aiohttp.ClientSession() 配合 async with
来源：http://zcj.gotoacloud.top

[U28] Py：类型别名
来源：http://amq.hysaishi.cn

UserId = int
来源：http://hcq.chenlongwang.top

[U29] Py：属性校验
来源：http://dix.cheryme.top

@property 与 @x.setter 配合
来源：http://bjc.pycfn.com

[U30] Py：数据类
来源：http://hou.svipenyu.cn

@dataclass(slots=True)
来源：http://xak.quarkkingdee.top

[U31] Py：单测
来源：http://uqw.bjfxy.top

python -m pytest -q
来源：http://qcu.chenzaomai.com

[U32] Py：代码格式化
来源：http://osm.jinghuilouyu.cn

ruff format . && ruff check --fix .
来源：http://voz.andypj.xyz

[U33] Py：打包发布
来源：http://kfb.shangyingyoupin.top

python -m build  （依赖 pyproject.toml）
来源：http://cua.yongpay.top

[U34] Py：判断编码
来源：http://asb.jinqigufen.top

chardet.detect(raw)
来源：http://gxv.havefunace.top

[U35] Py：发送邮件
来源：http://tjn.shangyingyoupin.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tcu.xuetiantiany.cn

[U36] Py：定时任务
来源：http://aki.sjlbkw.cn

schedule.every(10).minutes.do(job)
来源：http://iid.yuxming.cn

[U37] Py：读写 Excel
来源：http://blh.jinghuilouyu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://koj.xylfe.cn

[U38] Py：获取脚本所在目录
来源：http://wgf.uphjek.com

Path(__file__).resolve().parent
来源：http://xeg.sweek.top

[U39] Py：判断是否在交互环境
来源：http://cta.kuanghao11.cn

sys.stdout.isatty()
来源：http://xhb.daria6918.cn

[U40] Py：打印到标准错误
来源：http://hmb.iojbl.cn

print("err", file=sys.stderr)
来源：http://yqn.zhongyouzk.top

[U41] PHP：初始化 Composer 项目
来源：http://sjh.xinyue.icu

composer init;  composer require guzzlehttp/guzzle
来源：http://vyx.ybcxt.top

[U42] PHP：PSR-4 自动加载
来源：http://lnt.aizwys.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://sip.guannengcc.top


<!-- 参考信息 -->