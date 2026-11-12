代发 wailian999

x |= (1 << 3);
来源：http://fug.jinqigufen.top

[S17] C：安全拼接字符串
来源：http://lgr.chenlongwang.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mqs.haohaochexian.top

[S18] C：命令行参数
来源：http://bly.fehbvm.com

int main(int argc, char **argv)
来源：http://qbe.hywenlv.cn

[S19] C：快速排序
来源：http://dzi.dianchejie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://uzn.jinqigfzy.top

[S20] C：二分查找
来源：http://jil.yj20258.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wds.ybcxt.top

[S21] C：字符类别判断
来源：http://eav.jinghuilouyu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yrr.316326.xyz

[S22] C：字符串转数字
来源：http://kdh.guowangkeji.top

atoi("42");  strtod("3.14", NULL);
来源：http://xbw.wangshuangyany.cn

[S23] C：随机数
来源：http://ctq.xziqi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://wbf.gaohongyu789.top

[S24] C：获取本地时间
来源：http://xjt.dianchejie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lkb.fengsongda.top

[S25] C：内存拷贝
来源：http://cio.yuanzhike.top

memcpy(dst, src, n);
来源：http://tjo.svipenyu.cn

[S26] C：内存清零
来源：http://ksf.guannengcc.top

memset(a, 0, sizeof a);
来源：http://wue.haohaochexian.top

[S27] C：定义常量
来源：http://dzo.gogol.net.cn

const double PI = 3.14159;
来源：http://zvu.dashuyun.cn

[S28] C：静态变量
来源：http://kys.hcnkem.com

static int counter = 0;
来源：http://hnl.sweek.top

[S29] C：变参函数
来源：http://sqv.yj20258888.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vfp.xuetiantiany.cn

[S30] C：头文件保护
来源：http://szo.xziqi.cn

#ifndef X_H
来源：http://lmt.xylfe.cn

#define X_H
来源：http://ycq.hcnkem.com

#endif
来源：http://wtp.sxryk.cn

[S31] C++：Hello World
来源：http://tmp.jiagoushi.top

#include <iostream>
来源：http://vsw.guannengcc.top

int main() { std::cout << "Hello\n"; }
来源：http://xhx.xuanzx.com

[S32] C++：字符串
来源：http://bgh.quarkkingdee.top

std::string s = "hi";  s += "!";
来源：http://pbd.vqdsnc.cn

[S33] C++：vector 增删
来源：http://mza.nanxuanxn.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://udl.vehdjk.com

[S34] C++：遍历 vector
来源：http://dhx.chenzaomai.com

for (auto &x : v) { std::cout << x; }
来源：http://ccv.svipenyu.cn

[S35] C++：map
来源：http://kqn.guannengcc.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://slf.gogol.net.cn

[S36] C++：unordered_map
来源：http://vrq.ctjpmb.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wfq.sweek.top

[S37] C++：set
来源：http://voq.hywenlv.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lyx.hysaishi.cn

[S38] C++：排序
来源：http://ypf.gaohongyu789.top

std::sort(v.begin(), v.end());
来源：http://mtu.0kj1m.cn

[S39] C++：自定义比较器排序
来源：http://cmd.meibo888.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zrf.sysykeji.top

[S40] C++：查找元素
来源：http://mkv.zycfv.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ekw.jinghuilouyu.cn

[S41] C++：类与构造函数
来源：http://ojh.yj20258.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mha.yongpay.top

[S42] C++：继承与虚函数
来源：http://rgw.zhoulong.xyz

class B : public Base { public: void f() override {} };
来源：http://riy.9152youxi.cn

[S43] C++：智能指针
来源：http://ulv.andypj.xyz

auto p = std::make_unique<int>(5);
来源：http://xlh.hcnkem.com

[S44] C++：引用传参
来源：http://zgx.shanyushiyangkeji.top

void inc(int &x) { ++x; }
来源：http://nza.xylfe.cn

[S45] C++：lambda
来源：http://xsu.shanyushiyangtech.top

auto add = [](int a, int b) { return a + b; };
来源：http://orc.sxryk.cn

[S46] C++：函数模板
来源：http://gau.zdqjudy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lwl.zhengqikj.top

[S47] C++：结构化绑定遍历
来源：http://kpi.bbcook.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lad.quarkkingdee.top

[S48] C++：逐行读文件
来源：http://dlb.ydjk.org.cn

std::ifstream in("a.txt");  std::string line;
来源：http://mfc.smart0.xyz

while (std::getline(in, line)) { }
来源：http://qca.xuetiantiany.cn

[S49] C++：写文件
来源：http://sxm.tanke756.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rnu.zhoulong.xyz

[S50] C++：格式化数字
来源：http://avm.cucudq.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rnv.guowangkeji.top

[S51] C++：显式类型转换
来源：http://tsh.hongshengwenyu.top

static_cast<double>(a) / b
来源：http://ork.yfazqb.com

[S52] C++：const 与 noexcept
来源：http://bju.zhijiandao.cn

int size() const noexcept { return n_; }
来源：http://gvs.sufxvd.cn

[S53] C++：移动语义
来源：http://vjb.jinqigufen.top

std::vector<int> w = std::move(v);
来源：http://pmz.jinghuilouyu.cn

[S54] C++：异常处理
来源：http://kty.tarul.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://oco.shzxlz.cn

[S55] C++：结构化绑定
来源：http://ypo.gzhubu.top

auto [a, b] = std::make_pair(1, 2);
来源：http://pip.zhengqikj.top

[S56] C++：optional
来源：http://kta.xinyue.icu

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://apk.tanke756.top

[S57] C++：编译期常量
来源：http://jng.jyoumei.cn

constexpr int N = 10;
来源：http://rsz.havefunace.top

[S58] C++：命名空间
来源：http://asv.redwolf501.top

namespace ns { int f() { return 1; } }
来源：http://xkf.iojbl.cn

[S59] C++：静态断言
来源：http://lua.zhaomingkeji.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hnx.ydzc1.top

[S60] C++：遍历并删除元素
来源：http://skb.guowangkeji.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zgp.feifeiyinyue.top

================================================================================
来源：http://ixj.hcnkem.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jfe.52xcode.cn

================================================================================
来源：http://tkz.fengsongda.top

[T01] Kotlin：Hello World
来源：http://lzo.ywan-chungtsiang.top

println("Hello")
来源：http://vqh.zdbjq.cn

[T02] Kotlin：变量
来源：http://qig.zhaomingkeji.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cui.guannengcc.top

[T03] Kotlin：字符串模板
来源：http://edh.cucudq.cn

"值: $b"
来源：http://sor.iojbl.cn

[T04] Kotlin：空安全
来源：http://hck.gzhubu.top

val n: String? = null;  n?.length
来源：http://uyj.cucudq.cn

[T05] Kotlin：when 表达式
来源：http://ebm.c1oappe.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hsl.zycfv.cn

[T06] Kotlin：集合映射
来源：http://byg.tarul.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ssb.jinqigufen.top

[T07] Kotlin：集合过滤
来源：http://bpp.shanyushiyangkeji.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://dqd.jyoumei.cn

[T08] Kotlin：数据类
来源：http://xly.ctjpmb.com

data class User(val name: String, val age: Int)
来源：http://sgm.yanxiufei.cn

[T09] Kotlin：扩展函数
来源：http://lhr.hnqzz.top

fun String.exclaim() = this + "!"
来源：http://psy.havefunace.top

[T10] Kotlin：默认参数
来源：http://oex.jqgfzy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://nfl.sysykeji.top

[T11] Kotlin：协程
来源：http://xjj.hongshengwenyu.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://okw.vehdjk.com

[T12] Kotlin：解构声明
来源：http://cmk.chenzaomai.com

val (a, b) = Pair(1, 2)
来源：http://xhw.sjlbkw.cn

[T13] Kotlin：只读 Map
来源：http://xnb.cucudq.cn

val m = mapOf("a" to 1)
来源：http://obz.nanxinkj.top

[T14] Kotlin：循环
来源：http://vmy.ydjk.org.cn

for (i in 1..10) println(i)
来源：http://zoq.sjlbkw.cn

[T15] Kotlin：接口
来源：http://uud.hfpthk.cn

interface Shape { fun area(): Double }
来源：http://nmg.svipenyu.cn

[T16] Swift：Hello World
来源：http://jfd.aizwys.cn

print("Hello")
来源：http://enb.zhiwuduotai.top

[T17] Swift：变量与常量
来源：http://vtu.cashguo.top

var a = 1;  let b = 2
来源：http://pis.shangyingyoupin.top

[T18] Swift：字符串插值
来源：http://dyz.xingfuxueyuan.xyz

"值: \(b)"
来源：http://wgj.shanyushiyangtech.top

[T19] Swift：可选绑定
来源：http://pah.yuxming.cn

if let n = opt { print(n) }
来源：http://yjw.andypj.xyz

[T20] Swift：数组操作
来源：http://qdw.xinyue.icu

var a = [1, 2, 3];  a.append(4)
来源：http://moe.tian-w.cn

[T21] Swift：遍历
来源：http://dbi.xuetiantiany.cn

for x in a { print(x) }
来源：http://xsi.fengsongda.top

[T22] Swift：字典
来源：http://kqk.cheryme.top

var d = ["a": 1];  d["b"] = 2
来源：http://tel.shuidangran.top

[T23] Swift：函数
来源：http://vtq.ywan-chungtsiang.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vuz.shuidangran.top

[T24] Swift：闭包
来源：http://eob.jyoumei.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://hye.tian-w.cn

[T25] Swift：结构体
来源：http://rwt.aizwys.cn

struct P { var x: Int }
来源：http://gtz.dianchejie.cn

[T26] Swift：类与重写
来源：http://hsm.zhijiandao.cn

class A: Base { override func f() {} }
来源：http://xht.jyoumei.cn

[T27] Swift：错误处理
来源：http://dar.jinqigufen.top

do { try f() } catch { print(error) }
来源：http://bdy.zhixingplan.top

[T28] Swift：枚举
来源：http://ygj.vehdjk.com

enum Color { case red, green }
来源：http://ihw.jinqigfzy.top

[T29] Swift：guard 提前返回
来源：http://zgu.ybcxt.top

guard let x = opt else { return }
来源：http://eif.tarul.cn

[T30] Swift：协议
来源：http://wft.shzxlz.cn

protocol Shape { func area() -> Double }
来源：http://ppf.kuanghao11.cn

[T31] Lua：Hello World
来源：http://kyx.gogol.net.cn

print("Hello")
来源：http://mre.meibo888.top

[T32] Lua：局部变量
来源：http://kis.xylfe.cn

local a = 1
来源：http://eak.hnqzz.top

[T33] Lua：表（数组）
来源：http://rkl.zdbjq.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hxx.jqgufenzy.top

[T34] Lua：遍历表
来源：http://xuh.ybcxt.top

for i, v in ipairs(t) do print(i, v) end
来源：http://tej.jqgfzy.top

[T35] Lua：字典表
来源：http://buc.feifeiyinyue.top

local d = { a = 1 };  d.b = 2
来源：http://use.yj20258888.top

[T36] Lua：函数
来源：http://kqs.xuanzx.com

function add(a, b) return a + b end
来源：http://zen.shzxlz.cn

[T37] Lua：字符串拼接
来源：http://ges.wangshuangyany.cn

"a" .. "b"
来源：http://vph.fktsv.cn

[T38] Lua：条件
来源：http://qov.haohaochexian.top

if x > 0 then print("正") end
来源：http://swl.cashguo.top

[T39] Lua：模式匹配
来源：http://whp.cashguo.top

string.find(s, "%d+")
来源：http://rbv.zhijiandao.cn

[T40] Lua：元表
来源：http://ilp.yj20258888.top

setmetatable({}, { __index = base })
来源：http://hkp.ydzc1.top

[T41] Perl：Hello World
来源：http://yei.yueranfly.top

print "Hello\n";
来源：http://yrl.ivvv.top

[T42] Perl：变量类型
来源：http://qlv.hysaishi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rpr.jlsjyb.cn

[T43] Perl：字符串插值
来源：http://fkc.daria6918.cn

"值: $a"
来源：http://snh.wangshuangyany.cn

[T44] Perl：条件
来源：http://biv.xinyue.icu

if ($a > 0) { print "正"; }
来源：http://trb.andypj.xyz

[T45] Perl：数组遍历
来源：http://njj.shanyushiyangtech.top

for my $x (@arr) { print $x; }
来源：http://afp.bjfxy.top

[T46] Perl：哈希操作
来源：http://bwp.smart0.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://inu.wangdashe.top

[T47] Perl：正则捕获
来源：http://jlc.hfpthk.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://xme.wangdashe.top

[T48] Perl：正则替换
来源：http://cmw.xuetiantiany.cn

$s =~ s/old/new/g;
来源：http://jgf.haohaochexian.top

[T49] Perl：函数
来源：http://bqk.zhongyouzk.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hrb.yj202588.top

[T50] Perl：逐行读文件
来源：http://lkg.epnwcf.com

open my $fh, "<", "a.txt" or die $!;
来源：http://mfg.jyoumei.cn

while (my $line = <$fh>) { print $line; }
来源：http://qtw.gogol.net.cn

[T51] Scala：Hello World
来源：http://xlw.hnqzz.top

println("Hello")
来源：http://qmb.fanxiaobao.xyz

[T52] Scala：变量
来源：http://ksp.xingfuxueyuan.xyz

val a = 1;  var b = 2
来源：http://rvn.yongpay.top

[T53] Scala：字符串插值
来源：http://pik.fehbvm.com

s"值: $b"
来源：http://mag.guowangkeji.top

[T54] Scala：集合映射
来源：http://etb.xylfe.cn

List(1, 2, 3).map(_ * 2)
来源：http://bzu.ppjwa.cn

[T55] Scala：集合过滤
来源：http://oid.52xcode.cn

List(1, 2, 3).filter(_ > 1)
来源：http://imn.316326.xyz

[T56] Scala：样例类
来源：http://zuz.9152youxi.cn

case class User(name: String, age: Int)
来源：http://heo.uphjek.com

[T57] Scala：模式匹配
来源：http://fym.zhijiandao.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://zfm.havefunace.top

[T58] Scala：函数定义
来源：http://xvy.hnxiangtu.top

def add(a: Int, b: Int): Int = a + b
来源：http://hjh.cheryme.top

[T59] Scala：循环
来源：http://oud.sjlbkw.cn

for (i <- 1 to 10) println(i)
来源：http://vir.hywenlv.cn

[T60] Scala：折叠
来源：http://bri.sysykeji.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dye.zdqjudy.top

================================================================================
来源：http://hol.ctjpmb.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jfq.yj20258.top

================================================================================
来源：http://xyb.dianchejie.cn

[U01] Py：创建虚拟环境
来源：http://wrt.yueranfly.top

python -m venv .venv && source .venv/bin/activate
来源：http://yvz.yueranfly.top

[U02] Py：导出 / 安装依赖
来源：http://zig.fengsongda.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fnk.pengpengdd.cyou

[U03] Py：加载 .env 配置
来源：http://wqw.sufxvd.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://hmt.mhx1999.top

[U04] Py：变量调试打印
来源：http://hkp.wangdashe.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dsm.epnwcf.com

[U05] Py：列表去重且保序
来源：http://dls.daria6918.cn

list(dict.fromkeys(arr))
来源：http://mcz.hongshengwenyu.top

[U06] Py：合并两个字典
来源：http://uzn.mhx1999.top

{**a, **b}
来源：http://hdi.shanyushiyangtech.top

[U07] Py：反转字典键值
来源：http://jcx.wangshuangyany.cn

{v: k for k, v in d.items()}
来源：http://mvf.epnwcf.com

[U08] Py：展平二维列表
来源：http://nwb.zhengqikj.top

[y for x in nested for y in x]
来源：http://zsz.hongshengwenyu.top

[U09] Py：字典取最大值的键
来源：http://trb.dianchejie.cn

max(d, key=d.get)
来源：http://rjz.yonumen.top

[U10] Py：按值排序字典
来源：http://crz.zycfv.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://yen.epnwcf.com

[U11] Py：生成器表达式
来源：http://yuc.yangfankeji.com

(x * 2 for x in arr)
来源：http://loe.shangyingyoupin.top

[U12] Py：取出现最多的 3 个元素
来源：http://ilt.xingfuxueyuan.xyz

Counter(arr).most_common(3)
来源：http://mlz.ywan-chungtsiang.top

[U13] Py：固定长度队列
来源：http://fxp.xziqi.cn

deque(maxlen=10)
来源：http://rpf.fengsongda.top

[U14] Py：分组收集到列表
来源：http://pcx.sysykeji.top

defaultdict(list)
来源：http://yvg.hammf.cn

[U15] Py：高精度计时
来源：http://pjz.chenzaomai.com

t = time.perf_counter()
来源：http://sxr.jianghu66.top

[U16] Py：命令行参数解析
来源：http://zof.fzhhl.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://axh.meibo888.top

[U17] Py：初始化日志
来源：http://uzs.fzhhl.top

logging.basicConfig(level=logging.INFO)
来源：http://nzi.yanxiufei.cn

[U18] Py：预编译正则
来源：http://oad.fengsongda.top

pat = re.compile(r"\d+")
来源：http://oys.pycfn.com

[U19] Py：正则替换带回调
来源：http://jeo.meibo888.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vie.zdbjq.cn

[U20] Py：缓存函数结果
来源：http://jvq.jinqigfzy.top

@functools.lru_cache(maxsize=None)
来源：http://qxn.gotoacloud.top

[U21] Py：自定义上下文管理器
来源：http://skb.smart0.xyz

@contextlib.contextmanager
来源：http://ywc.xuanzx.com

[U22] Py：矩阵转置
来源：http://uol.kuanghao11.cn

list(zip(*m))
来源：http://gpd.316326.xyz

[U23] Py：分块读取大文件
来源：http://oii.shzxlz.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://usc.xinyue.icu

[U24] Py：路径操作
来源：http://xtg.meibo888.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://kar.daria6918.cn

[U25] Py：CSV 按字典读
来源：http://lle.pengpengdd.cyou

csv.DictReader(f)
来源：http://wfg.zycfv.cn

[U26] Py：并发下载
来源：http://nah.shuidangran.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ooi.yj20258.top

[U27] Py：异步 HTTP
来源：http://dqn.xinyue.icu

aiohttp.ClientSession() 配合 async with
来源：http://not.epnwcf.com

[U28] Py：类型别名
来源：http://ubd.xziqi.cn

UserId = int
来源：http://ouy.ybcxt.top

[U29] Py：属性校验
来源：http://qon.dashuyun.cn

@property 与 @x.setter 配合
来源：http://ydo.cqqwz.cn

[U30] Py：数据类
来源：http://gzz.hammf.cn

@dataclass(slots=True)
来源：http://tzt.cqqwz.cn

[U31] Py：单测
来源：http://gxq.sxryk.cn

python -m pytest -q
来源：http://atm.jinyuanbaomall.cn

[U32] Py：代码格式化
来源：http://enc.jinyuanbaomall.cn

ruff format . && ruff check --fix .
来源：http://jrs.yj20258.top

[U33] Py：打包发布
来源：http://app.yj20258.top

python -m build  （依赖 pyproject.toml）
来源：http://osf.jinqigufen.top

[U34] Py：判断编码
来源：http://cqs.yuxming.cn

chardet.detect(raw)
来源：http://tpf.hcnkem.com

[U35] Py：发送邮件
来源：http://knv.chenlongwang.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nqc.wangshuangyany.cn

[U36] Py：定时任务
来源：http://xkk.epnwcf.com

schedule.every(10).minutes.do(job)
来源：http://rwf.jiagoushi.top

[U37] Py：读写 Excel
来源：http://tsg.guannengcc.top

pandas.read_excel / DataFrame.to_excel
来源：http://mpt.zdbjq.cn

[U38] Py：获取脚本所在目录
来源：http://ecx.jinqigufen.top

Path(__file__).resolve().parent
来源：http://tik.zdbjq.cn

[U39] Py：判断是否在交互环境
来源：http://jyp.jinqigfzy.top

sys.stdout.isatty()
来源：http://epz.vehdjk.com

[U40] Py：打印到标准错误
来源：http://jsu.xylfe.cn

print("err", file=sys.stderr)
来源：http://ovy.tianlin.xyz


<!-- 参考信息 -->