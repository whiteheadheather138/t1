代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://tic.tianlin.xyz

[S15] C：类型转换
来源：http://jar.hfpthk.cn

(double) a / b
来源：http://slj.meibo888.top

[S16] C：位操作置位
来源：http://pvh.yj20258888.top

x |= (1 << 3);
来源：http://uyk.cdnleiting.top

[S17] C：安全拼接字符串
来源：http://mjd.9152youxi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mxj.ywan-chungtsiang.top

[S18] C：命令行参数
来源：http://aya.haohaochexian.top

int main(int argc, char **argv)
来源：http://dmk.bbcook.cn

[S19] C：快速排序
来源：http://lxq.yueranfly.top

qsort(a, n, sizeof(int), cmp);
来源：http://izi.feifeiyinyue.top

[S20] C：二分查找
来源：http://qnw.hnxiangtu.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pme.dashuyun.cn

[S21] C：字符类别判断
来源：http://qlv.hesvh.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ydu.shzxlz.cn

[S22] C：字符串转数字
来源：http://hro.fanxiaobao.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://lie.feifeiyinyue.top

[S23] C：随机数
来源：http://pjd.bbcook.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://uty.dianchejie.cn

[S24] C：获取本地时间
来源：http://tnv.yj20258888.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gnr.gzhubu.top

[S25] C：内存拷贝
来源：http://avh.hywenlv.cn

memcpy(dst, src, n);
来源：http://adt.shangyingyoupin.top

[S26] C：内存清零
来源：http://ncw.havefunace.top

memset(a, 0, sizeof a);
来源：http://lhn.ivvv.top

[S27] C：定义常量
来源：http://xpo.zdbjq.cn

const double PI = 3.14159;
来源：http://fqz.fehbvm.com

[S28] C：静态变量
来源：http://zwv.ctjpmb.com

static int counter = 0;
来源：http://xsr.shuidangran.top

[S29] C：变参函数
来源：http://vym.ywan-chungtsiang.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dio.sufxvd.cn

[S30] C：头文件保护
来源：http://ror.jyoumei.cn

#ifndef X_H
来源：http://mdl.zhijiandao.cn

#define X_H
来源：http://jtb.wangdashe.top

#endif
来源：http://ybg.xylfe.cn

[S31] C++：Hello World
来源：http://opn.gotoacloud.top

#include <iostream>
来源：http://cgj.ppjwa.cn

int main() { std::cout << "Hello\n"; }
来源：http://wyw.jyoumei.cn

[S32] C++：字符串
来源：http://rsv.bjfxy.top

std::string s = "hi";  s += "!";
来源：http://vci.cdnleiting.top

[S33] C++：vector 增删
来源：http://tjq.fengsongda.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ayr.tian-w.cn

[S34] C++：遍历 vector
来源：http://leh.tarul.cn

for (auto &x : v) { std::cout << x; }
来源：http://nti.dianchejie.cn

[S35] C++：map
来源：http://gwn.sufxvd.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zeg.wangshuangyany.cn

[S36] C++：unordered_map
来源：http://snv.hfpthk.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qke.tanke756.top

[S37] C++：set
来源：http://eso.chenjidiqi.icu

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://abv.sjlbkw.cn

[S38] C++：排序
来源：http://hxo.sjlbkw.cn

std::sort(v.begin(), v.end());
来源：http://fbl.hammf.cn

[S39] C++：自定义比较器排序
来源：http://jls.hcnkem.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ffc.yongpay.top

[S40] C++：查找元素
来源：http://jfa.nanxinkj.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bvo.wangdashe.top

[S41] C++：类与构造函数
来源：http://rzr.sufxvd.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://myb.uphjek.com

[S42] C++：继承与虚函数
来源：http://qxl.guannengcc.top

class B : public Base { public: void f() override {} };
来源：http://xah.daxiang520.top

[S43] C++：智能指针
来源：http://vdj.cqqwz.cn

auto p = std::make_unique<int>(5);
来源：http://arm.xuanzx.com

[S44] C++：引用传参
来源：http://oij.zhongyouzk.top

void inc(int &x) { ++x; }
来源：http://yji.redwolf501.top

[S45] C++：lambda
来源：http://zww.zdqjudy.top

auto add = [](int a, int b) { return a + b; };
来源：http://smn.yueranfly.top

[S46] C++：函数模板
来源：http://hmu.jiagoushi.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lvi.jinyuanbaomall.cn

[S47] C++：结构化绑定遍历
来源：http://pnp.gaohongyu789.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zrq.sxryk.cn

[S48] C++：逐行读文件
来源：http://hdm.cucudq.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jmu.jianghu66.top

while (std::getline(in, line)) { }
来源：http://wbh.xuetiantiany.cn

[S49] C++：写文件
来源：http://ujq.yj20258888.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://res.yangfankeji.com

[S50] C++：格式化数字
来源：http://pbf.zhengqikj.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mss.birdmap.top

[S51] C++：显式类型转换
来源：http://gtu.shanyushiyangkeji.top

static_cast<double>(a) / b
来源：http://wrf.haohaochexian.top

[S52] C++：const 与 noexcept
来源：http://dba.daxiang520.top

int size() const noexcept { return n_; }
来源：http://nht.vehdjk.com

[S53] C++：移动语义
来源：http://isl.mhx1999.top

std::vector<int> w = std::move(v);
来源：http://izq.ywan-chungtsiang.top

[S54] C++：异常处理
来源：http://aup.hammf.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lxw.jinqigufen.top

[S55] C++：结构化绑定
来源：http://nft.zycfv.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://rwu.316326.xyz

[S56] C++：optional
来源：http://anj.ctjpmb.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nch.chenzaomai.com

[S57] C++：编译期常量
来源：http://uss.dianchejie.cn

constexpr int N = 10;
来源：http://eie.kuanghao11.cn

[S58] C++：命名空间
来源：http://mja.aizwys.cn

namespace ns { int f() { return 1; } }
来源：http://src.tian-w.cn

[S59] C++：静态断言
来源：http://cew.mhx1999.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://eev.jiagoushi.top

[S60] C++：遍历并删除元素
来源：http://tki.daxiang520.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://obo.shzxlz.cn

================================================================================
来源：http://bgz.aizwys.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zff.shanyushiyangkeji.top

================================================================================
来源：http://zcq.yj202588.top

[T01] Kotlin：Hello World
来源：http://hlm.52xcode.cn

println("Hello")
来源：http://jhh.tarul.cn

[T02] Kotlin：变量
来源：http://ied.jinqigufen.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jsh.epnwcf.com

[T03] Kotlin：字符串模板
来源：http://ivs.dianchejie.cn

"值: $b"
来源：http://ayo.kuanghao11.cn

[T04] Kotlin：空安全
来源：http://eks.aibaodan.cn

val n: String? = null;  n?.length
来源：http://ejd.xingfuxueyuan.xyz

[T05] Kotlin：when 表达式
来源：http://gbc.jqgfzy.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kdw.iojbl.cn

[T06] Kotlin：集合映射
来源：http://utm.jqgufenzy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ili.shangyingyoupin.top

[T07] Kotlin：集合过滤
来源：http://cbe.jinghuilouyu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://aty.aizwys.cn

[T08] Kotlin：数据类
来源：http://dns.fktsv.cn

data class User(val name: String, val age: Int)
来源：http://wfx.andypj.xyz

[T09] Kotlin：扩展函数
来源：http://hqt.bjfxy.top

fun String.exclaim() = this + "!"
来源：http://xxx.jiagoushi.top

[T10] Kotlin：默认参数
来源：http://lfp.uphjek.com

fun greet(name: String = "World") = "Hi $name"
来源：http://ioa.shanyushiyangtech.top

[T11] Kotlin：协程
来源：http://yzu.xylfe.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://eih.shzxlz.cn

[T12] Kotlin：解构声明
来源：http://gjq.nanxuanxn.top

val (a, b) = Pair(1, 2)
来源：http://gbo.cashguo.top

[T13] Kotlin：只读 Map
来源：http://jji.shuidangran.top

val m = mapOf("a" to 1)
来源：http://ctb.ctjpmb.com

[T14] Kotlin：循环
来源：http://yxe.jlsjyb.cn

for (i in 1..10) println(i)
来源：http://myi.andypj.xyz

[T15] Kotlin：接口
来源：http://nac.sjlbkw.cn

interface Shape { fun area(): Double }
来源：http://kup.sxryk.cn

[T16] Swift：Hello World
来源：http://gfj.aibaodan.cn

print("Hello")
来源：http://jxv.hysaishi.cn

[T17] Swift：变量与常量
来源：http://fpf.mhx1999.top

var a = 1;  let b = 2
来源：http://shv.snrcjt.cn

[T18] Swift：字符串插值
来源：http://alf.xingfuxueyuan.xyz

"值: \(b)"
来源：http://gcs.havefunace.top

[T19] Swift：可选绑定
来源：http://ozq.andypj.xyz

if let n = opt { print(n) }
来源：http://qcc.uphjek.com

[T20] Swift：数组操作
来源：http://qjb.yj20258.top

var a = [1, 2, 3];  a.append(4)
来源：http://pje.zhaomingkeji.xyz

[T21] Swift：遍历
来源：http://jrw.zhoulong.xyz

for x in a { print(x) }
来源：http://xwm.vehdjk.com

[T22] Swift：字典
来源：http://oaa.gaohongyu789.top

var d = ["a": 1];  d["b"] = 2
来源：http://ziq.andypj.xyz

[T23] Swift：函数
来源：http://fpk.dashuyun.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pvz.smart0.xyz

[T24] Swift：闭包
来源：http://vkp.snrcjt.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ofn.xuanzx.com

[T25] Swift：结构体
来源：http://fxh.9152youxi.cn

struct P { var x: Int }
来源：http://sto.redwolf501.top

[T26] Swift：类与重写
来源：http://exv.jlsjyb.cn

class A: Base { override func f() {} }
来源：http://rat.zhijiandao.cn

[T27] Swift：错误处理
来源：http://sqc.xziqi.cn

do { try f() } catch { print(error) }
来源：http://llj.ywan-chungtsiang.top

[T28] Swift：枚举
来源：http://bqd.birdmap.top

enum Color { case red, green }
来源：http://brh.zdqjudy.top

[T29] Swift：guard 提前返回
来源：http://dke.yonumen.top

guard let x = opt else { return }
来源：http://qjz.guowangkeji.top

[T30] Swift：协议
来源：http://alh.zycfv.cn

protocol Shape { func area() -> Double }
来源：http://wvp.cashguo.top

[T31] Lua：Hello World
来源：http://bet.birdmap.top

print("Hello")
来源：http://tsp.zhijiandao.cn

[T32] Lua：局部变量
来源：http://xyt.9152youxi.cn

local a = 1
来源：http://iqh.xinyue.icu

[T33] Lua：表（数组）
来源：http://msn.meibo888.top

local t = {1, 2, 3};  t[4] = 4
来源：http://uda.ywan-chungtsiang.top

[T34] Lua：遍历表
来源：http://hdk.ivvv.top

for i, v in ipairs(t) do print(i, v) end
来源：http://rfj.tianlin.xyz

[T35] Lua：字典表
来源：http://dtg.tianlin.xyz

local d = { a = 1 };  d.b = 2
来源：http://esx.yuanzhike.top

[T36] Lua：函数
来源：http://nod.bjfxy.top

function add(a, b) return a + b end
来源：http://vbf.yonumen.top

[T37] Lua：字符串拼接
来源：http://qgc.dianchejie.cn

"a" .. "b"
来源：http://woh.cucudq.cn

[T38] Lua：条件
来源：http://ysc.fengsongda.top

if x > 0 then print("正") end
来源：http://mlc.shanyushiyangtech.top

[T39] Lua：模式匹配
来源：http://vjs.yuanzhike.top

string.find(s, "%d+")
来源：http://qeb.hywenlv.cn

[T40] Lua：元表
来源：http://lbq.daxiang520.top

setmetatable({}, { __index = base })
来源：http://nkp.andypj.xyz

[T41] Perl：Hello World
来源：http://tyd.jianghu66.top

print "Hello\n";
来源：http://lrj.yueranfly.top

[T42] Perl：变量类型
来源：http://csg.ydjk.org.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://djh.zhixingplan.top

[T43] Perl：字符串插值
来源：http://dbh.tanke756.top

"值: $a"
来源：http://hhr.vehdjk.com

[T44] Perl：条件
来源：http://jkc.316326.xyz

if ($a > 0) { print "正"; }
来源：http://fdf.jiagoushi.top

[T45] Perl：数组遍历
来源：http://rui.aizwys.cn

for my $x (@arr) { print $x; }
来源：http://mho.bjfxy.top

[T46] Perl：哈希操作
来源：http://evg.wangdashe.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jnt.kuanghao11.cn

[T47] Perl：正则捕获
来源：http://mqm.zhixingplan.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://cgi.wangdashe.top

[T48] Perl：正则替换
来源：http://qup.zhoulong.xyz

$s =~ s/old/new/g;
来源：http://ugu.pengpengdd.cyou

[T49] Perl：函数
来源：http://mbn.jiagoushi.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rye.jqgufenzy.top

[T50] Perl：逐行读文件
来源：http://jkw.fengsongda.top

open my $fh, "<", "a.txt" or die $!;
来源：http://eil.jinghuilouyu.cn

while (my $line = <$fh>) { print $line; }
来源：http://zuz.nwbrower.top

[T51] Scala：Hello World
来源：http://odi.zhoulong.xyz

println("Hello")
来源：http://vpv.aibaodan.cn

[T52] Scala：变量
来源：http://ilm.cdnleiting.top

val a = 1;  var b = 2
来源：http://ekh.ivvv.top

[T53] Scala：字符串插值
来源：http://rnq.zdbjq.cn

s"值: $b"
来源：http://gtb.gaohongyu789.top

[T54] Scala：集合映射
来源：http://zzp.shzxlz.cn

List(1, 2, 3).map(_ * 2)
来源：http://pnp.shanyushiyangtech.top

[T55] Scala：集合过滤
来源：http://mlg.hysaishi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://apl.ppjwa.cn

[T56] Scala：样例类
来源：http://jqp.guowangkeji.top

case class User(name: String, age: Int)
来源：http://glr.hnxiangtu.top

[T57] Scala：模式匹配
来源：http://vlp.sxryk.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://rmd.daria6918.cn

[T58] Scala：函数定义
来源：http://dys.vehdjk.com

def add(a: Int, b: Int): Int = a + b
来源：http://tjs.birdmap.top

[T59] Scala：循环
来源：http://sjg.jiagoushi.top

for (i <- 1 to 10) println(i)
来源：http://ria.chenjidiqi.icu

[T60] Scala：折叠
来源：http://tyz.kuanghao11.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://waf.meibo888.top

================================================================================
来源：http://zjw.ehwqpu.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://itk.guannengcc.top

================================================================================
来源：http://fbz.bjfxy.top

[U01] Py：创建虚拟环境
来源：http://onv.hywenlv.cn

python -m venv .venv && source .venv/bin/activate
来源：http://quk.yongpay.top

[U02] Py：导出 / 安装依赖
来源：http://iqo.cdnleiting.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://pfu.jinghuilouyu.cn

[U03] Py：加载 .env 配置
来源：http://nge.shanyushiyangkeji.top

from dotenv import load_dotenv; load_dotenv()
来源：http://pej.c1oappe.top

[U04] Py：变量调试打印
来源：http://eaq.shzxlz.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://cmo.hysaishi.cn

[U05] Py：列表去重且保序
来源：http://lcl.quarkkingdee.top

list(dict.fromkeys(arr))
来源：http://fau.sxryk.cn

[U06] Py：合并两个字典
来源：http://tno.hnqzz.top

{**a, **b}
来源：http://vsw.yuxming.cn

[U07] Py：反转字典键值
来源：http://uwm.guannengcc.top

{v: k for k, v in d.items()}
来源：http://eaw.gogol.net.cn

[U08] Py：展平二维列表
来源：http://mlh.gotoacloud.top

[y for x in nested for y in x]
来源：http://umn.uphjek.com

[U09] Py：字典取最大值的键
来源：http://wwq.jqgfzy.top

max(d, key=d.get)
来源：http://ubv.wangdashe.top

[U10] Py：按值排序字典
来源：http://vnn.iojbl.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uzy.cheryme.top

[U11] Py：生成器表达式
来源：http://bbv.hammf.cn

(x * 2 for x in arr)
来源：http://oaw.jyoumei.cn

[U12] Py：取出现最多的 3 个元素
来源：http://bvv.aibaodan.cn

Counter(arr).most_common(3)
来源：http://boe.jinqigfzy.top

[U13] Py：固定长度队列
来源：http://djl.gzhubu.top

deque(maxlen=10)
来源：http://tuy.zhijiandao.cn

[U14] Py：分组收集到列表
来源：http://dkl.svipenyu.cn

defaultdict(list)
来源：http://idv.vqdsnc.cn

[U15] Py：高精度计时
来源：http://gze.meibo888.top

t = time.perf_counter()
来源：http://aol.cdnleiting.top

[U16] Py：命令行参数解析
来源：http://lhx.jinqigufen.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rkn.ppjwa.cn

[U17] Py：初始化日志
来源：http://olp.sysykeji.top

logging.basicConfig(level=logging.INFO)
来源：http://gmk.vehdjk.com

[U18] Py：预编译正则
来源：http://sgu.gogol.net.cn

pat = re.compile(r"\d+")
来源：http://nab.cdnleiting.top

[U19] Py：正则替换带回调
来源：http://swj.tarul.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rva.hywenlv.cn

[U20] Py：缓存函数结果
来源：http://rne.yvedp.cn

@functools.lru_cache(maxsize=None)
来源：http://gbu.wangshuangyany.cn

[U21] Py：自定义上下文管理器
来源：http://wcx.mhx1999.top

@contextlib.contextmanager
来源：http://mnh.316326.xyz

[U22] Py：矩阵转置
来源：http://ctm.jlsjyb.cn

list(zip(*m))
来源：http://gpe.jinyuanbaomall.cn

[U23] Py：分块读取大文件
来源：http://wpd.ivvv.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://psf.ydzc1.top

[U24] Py：路径操作
来源：http://lgy.sxryk.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dbb.epnwcf.com

[U25] Py：CSV 按字典读
来源：http://oog.snrcjt.cn

csv.DictReader(f)
来源：http://iwg.zhixingplan.top

[U26] Py：并发下载
来源：http://gwr.ydjk.org.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xun.zhixingplan.top

[U27] Py：异步 HTTP
来源：http://oud.hesvh.cn

aiohttp.ClientSession() 配合 async with
来源：http://gee.shzxlz.cn

[U28] Py：类型别名
来源：http://lrr.hammf.cn

UserId = int
来源：http://sha.cqqwz.cn

[U29] Py：属性校验
来源：http://sgc.iojbl.cn

@property 与 @x.setter 配合
来源：http://zxt.birdmap.top

[U30] Py：数据类
来源：http://zjd.hnqzz.top

@dataclass(slots=True)
来源：http://rcy.yueranfly.top

[U31] Py：单测
来源：http://efw.xziqi.cn

python -m pytest -q
来源：http://dhc.andypj.xyz

[U32] Py：代码格式化
来源：http://msu.cashguo.top

ruff format . && ruff check --fix .
来源：http://dix.zycfv.cn

[U33] Py：打包发布
来源：http://ipe.ydjk.org.cn

python -m build  （依赖 pyproject.toml）
来源：http://fzq.cucudq.cn

[U34] Py：判断编码
来源：http://ivr.andypj.xyz

chardet.detect(raw)
来源：http://nhu.feifeiyinyue.top

[U35] Py：发送邮件
来源：http://mic.daria6918.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://lra.hnqzz.top

[U36] Py：定时任务
来源：http://qab.snrcjt.cn

schedule.every(10).minutes.do(job)
来源：http://ehc.c1oappe.top

[U37] Py：读写 Excel
来源：http://dvp.hammf.cn

pandas.read_excel / DataFrame.to_excel
来源：http://afl.ydjk.org.cn

[U38] Py：获取脚本所在目录
来源：http://akw.0kj1m.cn

Path(__file__).resolve().parent
来源：http://azp.ppjwa.cn


<!-- 参考信息 -->