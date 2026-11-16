代发 wailian999

x |= (1 << 3);
来源：http://kvg.tanke756.top

[S17] C：安全拼接字符串
来源：http://tlz.xuanzx.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mis.ivvv.top

[S18] C：命令行参数
来源：http://nak.chenjidiqi.icu

int main(int argc, char **argv)
来源：http://oct.sufxvd.cn

[S19] C：快速排序
来源：http://wfy.birdmap.top

qsort(a, n, sizeof(int), cmp);
来源：http://fbj.hcnkem.com

[S20] C：二分查找
来源：http://npx.chenjidiqi.icu

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cbo.aizwys.cn

[S21] C：字符类别判断
来源：http://mqe.hammf.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yby.ctjpmb.com

[S22] C：字符串转数字
来源：http://reo.jianghu66.top

atoi("42");  strtod("3.14", NULL);
来源：http://kjs.jyoumei.cn

[S23] C：随机数
来源：http://ltu.haohaochexian.top

srand(time(NULL));  int r = rand() % 100;
来源：http://wxk.guowangkeji.top

[S24] C：获取本地时间
来源：http://dax.ywan-chungtsiang.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://iui.gzhubu.top

[S25] C：内存拷贝
来源：http://ckt.wangdashe.top

memcpy(dst, src, n);
来源：http://fgj.chenjidiqi.icu

[S26] C：内存清零
来源：http://kzz.redwolf501.top

memset(a, 0, sizeof a);
来源：http://sgj.snrcjt.cn

[S27] C：定义常量
来源：http://ocr.yvedp.cn

const double PI = 3.14159;
来源：http://dsc.meibo888.top

[S28] C：静态变量
来源：http://dzm.zhiwuduotai.top

static int counter = 0;
来源：http://phi.hcnkem.com

[S29] C：变参函数
来源：http://ggf.nanxuanxn.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pfp.kuanghao11.cn

[S30] C：头文件保护
来源：http://jfk.kuanghao11.cn

#ifndef X_H
来源：http://lpn.guowangkeji.top

#define X_H
来源：http://vgo.yvedp.cn

#endif
来源：http://not.fengsongda.top

[S31] C++：Hello World
来源：http://slo.dianchejie.cn

#include <iostream>
来源：http://vhi.hywenlv.cn

int main() { std::cout << "Hello\n"; }
来源：http://ypq.zhoulong.xyz

[S32] C++：字符串
来源：http://bnb.guowangkeji.top

std::string s = "hi";  s += "!";
来源：http://wpy.ppjwa.cn

[S33] C++：vector 增删
来源：http://gcy.nwbrower.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ets.shzxlz.cn

[S34] C++：遍历 vector
来源：http://qlw.fzhhl.top

for (auto &x : v) { std::cout << x; }
来源：http://tuv.yueranfly.top

[S35] C++：map
来源：http://eyd.shuidangran.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lpc.zhijiandao.cn

[S36] C++：unordered_map
来源：http://kxj.cdnleiting.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mbv.ppjwa.cn

[S37] C++：set
来源：http://cdr.jinghuilouyu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bih.vqdsnc.cn

[S38] C++：排序
来源：http://wrn.ywan-chungtsiang.top

std::sort(v.begin(), v.end());
来源：http://zff.ydzc1.top

[S39] C++：自定义比较器排序
来源：http://kth.chenlongwang.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sai.hnqzz.top

[S40] C++：查找元素
来源：http://xcd.jianghu66.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://avx.fehbvm.com

[S41] C++：类与构造函数
来源：http://oyu.birdmap.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vea.mhx1999.top

[S42] C++：继承与虚函数
来源：http://azo.yj202588.top

class B : public Base { public: void f() override {} };
来源：http://rhm.yvedp.cn

[S43] C++：智能指针
来源：http://aog.yonumen.top

auto p = std::make_unique<int>(5);
来源：http://ncm.chenzaomai.com

[S44] C++：引用传参
来源：http://frp.zhiwuduotai.top

void inc(int &x) { ++x; }
来源：http://wej.fanxiaobao.xyz

[S45] C++：lambda
来源：http://tsq.ywan-chungtsiang.top

auto add = [](int a, int b) { return a + b; };
来源：http://mpq.fehbvm.com

[S46] C++：函数模板
来源：http://gag.ppjwa.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zox.ppjwa.cn

[S47] C++：结构化绑定遍历
来源：http://ukn.sjlbkw.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://eyi.yonumen.top

[S48] C++：逐行读文件
来源：http://plq.aizwys.cn

std::ifstream in("a.txt");  std::string line;
来源：http://rqn.mhx1999.top

while (std::getline(in, line)) { }
来源：http://grn.tarul.cn

[S49] C++：写文件
来源：http://wdg.0kj1m.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xxd.dianchejie.cn

[S50] C++：格式化数字
来源：http://ddh.zhengqikj.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wji.hysaishi.cn

[S51] C++：显式类型转换
来源：http://xqv.wangdashe.top

static_cast<double>(a) / b
来源：http://uib.ivvv.top

[S52] C++：const 与 noexcept
来源：http://cra.nanxinkj.top

int size() const noexcept { return n_; }
来源：http://rmj.52xcode.cn

[S53] C++：移动语义
来源：http://tyw.zhiwuduotai.top

std::vector<int> w = std::move(v);
来源：http://ubd.mhx1999.top

[S54] C++：异常处理
来源：http://ckz.jinqigfzy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cvu.xuetiantiany.cn

[S55] C++：结构化绑定
来源：http://zse.xingfuxueyuan.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://myd.jianghu66.top

[S56] C++：optional
来源：http://mzg.9152youxi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://glv.fanxiaobao.xyz

[S57] C++：编译期常量
来源：http://xeu.chenjidiqi.icu

constexpr int N = 10;
来源：http://lbb.mhx1999.top

[S58] C++：命名空间
来源：http://qbl.ywan-chungtsiang.top

namespace ns { int f() { return 1; } }
来源：http://xly.yj202588.top

[S59] C++：静态断言
来源：http://hij.xuetiantiany.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fcr.wangdashe.top

[S60] C++：遍历并删除元素
来源：http://vxj.jianghu66.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://sjb.sysykeji.top

================================================================================
来源：http://klb.iojbl.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lhv.fanxiaobao.xyz

================================================================================
来源：http://gdv.andypj.xyz

[T01] Kotlin：Hello World
来源：http://ier.iojbl.cn

println("Hello")
来源：http://nzx.hongshengwenyu.top

[T02] Kotlin：变量
来源：http://mai.c1oappe.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ymr.nanxuanxn.top

[T03] Kotlin：字符串模板
来源：http://yfi.pycfn.com

"值: $b"
来源：http://bbc.sjlbkw.cn

[T04] Kotlin：空安全
来源：http://uut.jinqigfzy.top

val n: String? = null;  n?.length
来源：http://zvv.cqqwz.cn

[T05] Kotlin：when 表达式
来源：http://csh.zhaomingkeji.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lvm.gogol.net.cn

[T06] Kotlin：集合映射
来源：http://qhf.redwolf501.top

listOf(1, 2, 3).map { it * 2 }
来源：http://qhz.bbcook.cn

[T07] Kotlin：集合过滤
来源：http://osn.hysaishi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://fcm.pengpengdd.cyou

[T08] Kotlin：数据类
来源：http://nry.daria6918.cn

data class User(val name: String, val age: Int)
来源：http://gll.kuanghao11.cn

[T09] Kotlin：扩展函数
来源：http://xsy.pycfn.com

fun String.exclaim() = this + "!"
来源：http://xta.zdbjq.cn

[T10] Kotlin：默认参数
来源：http://kun.uphjek.com

fun greet(name: String = "World") = "Hi $name"
来源：http://qqv.xziqi.cn

[T11] Kotlin：协程
来源：http://fnz.haohaochexian.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://snu.zhiwuduotai.top

[T12] Kotlin：解构声明
来源：http://ypv.ybcxt.top

val (a, b) = Pair(1, 2)
来源：http://rwg.zdqjudy.top

[T13] Kotlin：只读 Map
来源：http://bnt.ywan-chungtsiang.top

val m = mapOf("a" to 1)
来源：http://xyg.yfazqb.com

[T14] Kotlin：循环
来源：http://uhw.cucudq.cn

for (i in 1..10) println(i)
来源：http://lfb.yuxming.cn

[T15] Kotlin：接口
来源：http://unb.chenlongwang.top

interface Shape { fun area(): Double }
来源：http://uqt.jqgufenzy.top

[T16] Swift：Hello World
来源：http://kqy.aibaodan.cn

print("Hello")
来源：http://ylp.yfazqb.com

[T17] Swift：变量与常量
来源：http://okn.hfpthk.cn

var a = 1;  let b = 2
来源：http://wds.tanke756.top

[T18] Swift：字符串插值
来源：http://fqq.vqdsnc.cn

"值: \(b)"
来源：http://qcb.yuanzhike.top

[T19] Swift：可选绑定
来源：http://kfc.epnwcf.com

if let n = opt { print(n) }
来源：http://nqk.chenlongwang.top

[T20] Swift：数组操作
来源：http://dcf.cdnleiting.top

var a = [1, 2, 3];  a.append(4)
来源：http://dpb.cheryme.top

[T21] Swift：遍历
来源：http://bxu.zdbjq.cn

for x in a { print(x) }
来源：http://sjk.shangyingyoupin.top

[T22] Swift：字典
来源：http://sjx.zhongyouzk.top

var d = ["a": 1];  d["b"] = 2
来源：http://zca.gogol.net.cn

[T23] Swift：函数
来源：http://btn.nwbrower.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dsp.hongshengwenyu.top

[T24] Swift：闭包
来源：http://gcb.yj20258.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://zeb.yonumen.top

[T25] Swift：结构体
来源：http://qud.cqqwz.cn

struct P { var x: Int }
来源：http://xfr.9152youxi.cn

[T26] Swift：类与重写
来源：http://bhe.ivvv.top

class A: Base { override func f() {} }
来源：http://tnr.yueranfly.top

[T27] Swift：错误处理
来源：http://zcs.yj20258888.top

do { try f() } catch { print(error) }
来源：http://ezc.uphjek.com

[T28] Swift：枚举
来源：http://akf.ydjk.org.cn

enum Color { case red, green }
来源：http://law.52xcode.cn

[T29] Swift：guard 提前返回
来源：http://ywf.hongshengwenyu.top

guard let x = opt else { return }
来源：http://msq.dashuyun.cn

[T30] Swift：协议
来源：http://clm.shangyingyoupin.top

protocol Shape { func area() -> Double }
来源：http://zgc.cashguo.top

[T31] Lua：Hello World
来源：http://zgm.hnqzz.top

print("Hello")
来源：http://xno.shanyushiyangkeji.top

[T32] Lua：局部变量
来源：http://mhe.mhx1999.top

local a = 1
来源：http://kyo.xylfe.cn

[T33] Lua：表（数组）
来源：http://vio.yj202588.top

local t = {1, 2, 3};  t[4] = 4
来源：http://miu.zhongyouzk.top

[T34] Lua：遍历表
来源：http://wax.hfpthk.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://hac.fktsv.cn

[T35] Lua：字典表
来源：http://pda.shuidangran.top

local d = { a = 1 };  d.b = 2
来源：http://tel.zhongyouzk.top

[T36] Lua：函数
来源：http://aki.zhixingplan.top

function add(a, b) return a + b end
来源：http://loo.tarul.cn

[T37] Lua：字符串拼接
来源：http://egw.jiagoushi.top

"a" .. "b"
来源：http://hro.aibaodan.cn

[T38] Lua：条件
来源：http://pax.jinghuilouyu.cn

if x > 0 then print("正") end
来源：http://mse.jinghuilouyu.cn

[T39] Lua：模式匹配
来源：http://sim.cucudq.cn

string.find(s, "%d+")
来源：http://cvk.ybcxt.top

[T40] Lua：元表
来源：http://ggn.smart0.xyz

setmetatable({}, { __index = base })
来源：http://umh.shanyushiyangtech.top

[T41] Perl：Hello World
来源：http://efw.hongshengwenyu.top

print "Hello\n";
来源：http://akg.jyoumei.cn

[T42] Perl：变量类型
来源：http://tby.ybcxt.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xox.vqdsnc.cn

[T43] Perl：字符串插值
来源：http://ulk.nwbrower.top

"值: $a"
来源：http://jgv.birdmap.top

[T44] Perl：条件
来源：http://vxx.mhx1999.top

if ($a > 0) { print "正"; }
来源：http://snz.nwbrower.top

[T45] Perl：数组遍历
来源：http://qzx.nwbrower.top

for my $x (@arr) { print $x; }
来源：http://rwv.jinyuanbaomall.cn

[T46] Perl：哈希操作
来源：http://ayi.hesvh.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://asp.yvedp.cn

[T47] Perl：正则捕获
来源：http://gee.gogol.net.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://imb.0kj1m.cn

[T48] Perl：正则替换
来源：http://xxp.ydzc1.top

$s =~ s/old/new/g;
来源：http://ycw.sjlbkw.cn

[T49] Perl：函数
来源：http://kbq.fanxiaobao.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nlj.fanxiaobao.xyz

[T50] Perl：逐行读文件
来源：http://ucg.hnxiangtu.top

open my $fh, "<", "a.txt" or die $!;
来源：http://zet.fktsv.cn

while (my $line = <$fh>) { print $line; }
来源：http://tav.ehwqpu.com

[T51] Scala：Hello World
来源：http://lja.jinghuilouyu.cn

println("Hello")
来源：http://cnj.ydzc1.top

[T52] Scala：变量
来源：http://bmj.hywenlv.cn

val a = 1;  var b = 2
来源：http://nts.fehbvm.com

[T53] Scala：字符串插值
来源：http://ejo.yfazqb.com

s"值: $b"
来源：http://say.hnxiangtu.top

[T54] Scala：集合映射
来源：http://uwd.haohaochexian.top

List(1, 2, 3).map(_ * 2)
来源：http://urv.shzxlz.cn

[T55] Scala：集合过滤
来源：http://cjb.shanyushiyangtech.top

List(1, 2, 3).filter(_ > 1)
来源：http://ahm.sxryk.cn

[T56] Scala：样例类
来源：http://lyf.aibaodan.cn

case class User(name: String, age: Int)
来源：http://jnw.ybcxt.top

[T57] Scala：模式匹配
来源：http://bgy.kuanghao11.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://swb.xingfuxueyuan.xyz

[T58] Scala：函数定义
来源：http://mba.aibaodan.cn

def add(a: Int, b: Int): Int = a + b
来源：http://alj.jlsjyb.cn

[T59] Scala：循环
来源：http://qal.cashguo.top

for (i <- 1 to 10) println(i)
来源：http://arj.jinqigfzy.top

[T60] Scala：折叠
来源：http://geg.yonumen.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ozj.hysaishi.cn

================================================================================
来源：http://bat.chenjidiqi.icu

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xpj.52xcode.cn

================================================================================
来源：http://rjq.bjfxy.top

[U01] Py：创建虚拟环境
来源：http://atv.hesvh.cn

python -m venv .venv && source .venv/bin/activate
来源：http://oek.gogol.net.cn

[U02] Py：导出 / 安装依赖
来源：http://rvz.cqqwz.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://efm.52xcode.cn

[U03] Py：加载 .env 配置
来源：http://hgy.yangfankeji.com

from dotenv import load_dotenv; load_dotenv()
来源：http://vqs.zhoulong.xyz

[U04] Py：变量调试打印
来源：http://iaq.xziqi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dnn.nwbrower.top

[U05] Py：列表去重且保序
来源：http://oom.gaohongyu789.top

list(dict.fromkeys(arr))
来源：http://vnn.meibo888.top

[U06] Py：合并两个字典
来源：http://fwd.yuxming.cn

{**a, **b}
来源：http://jam.zhaomingkeji.xyz

[U07] Py：反转字典键值
来源：http://qmf.shangyingyoupin.top

{v: k for k, v in d.items()}
来源：http://bmn.yuxming.cn

[U08] Py：展平二维列表
来源：http://ycs.bjfxy.top

[y for x in nested for y in x]
来源：http://eny.xingfuxueyuan.xyz

[U09] Py：字典取最大值的键
来源：http://ful.bbcook.cn

max(d, key=d.get)
来源：http://jtz.yueranfly.top

[U10] Py：按值排序字典
来源：http://ywv.daxiang520.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vxq.jqgufenzy.top

[U11] Py：生成器表达式
来源：http://xba.nwbrower.top

(x * 2 for x in arr)
来源：http://dbv.jqgfzy.top

[U12] Py：取出现最多的 3 个元素
来源：http://cdu.zhijiandao.cn

Counter(arr).most_common(3)
来源：http://hiq.hnqzz.top

[U13] Py：固定长度队列
来源：http://yuu.yj202588.top

deque(maxlen=10)
来源：http://yrh.0kj1m.cn

[U14] Py：分组收集到列表
来源：http://dhw.cqqwz.cn

defaultdict(list)
来源：http://ycn.xylfe.cn

[U15] Py：高精度计时
来源：http://llm.sufxvd.cn

t = time.perf_counter()
来源：http://oou.xinyue.icu

[U16] Py：命令行参数解析
来源：http://sil.shanyushiyangkeji.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mnh.epnwcf.com

[U17] Py：初始化日志
来源：http://wrw.vqdsnc.cn

logging.basicConfig(level=logging.INFO)
来源：http://ugv.hnqzz.top

[U18] Py：预编译正则
来源：http://bjf.jianghu66.top

pat = re.compile(r"\d+")
来源：http://grz.quarkkingdee.top

[U19] Py：正则替换带回调
来源：http://bbp.guannengcc.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://uka.hfpthk.cn

[U20] Py：缓存函数结果
来源：http://aka.0kj1m.cn

@functools.lru_cache(maxsize=None)
来源：http://trp.yueranfly.top

[U21] Py：自定义上下文管理器
来源：http://rht.haohaochexian.top

@contextlib.contextmanager
来源：http://cfv.xuanzx.com

[U22] Py：矩阵转置
来源：http://kfp.dianchejie.cn

list(zip(*m))
来源：http://laq.316326.xyz

[U23] Py：分块读取大文件
来源：http://kjs.zycfv.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ska.zhixingplan.top

[U24] Py：路径操作
来源：http://lcf.quarkkingdee.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mzy.pengpengdd.cyou

[U25] Py：CSV 按字典读
来源：http://fuh.cashguo.top

csv.DictReader(f)
来源：http://tdv.nanxuanxn.top

[U26] Py：并发下载
来源：http://zhz.yueranfly.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hcl.fehbvm.com

[U27] Py：异步 HTTP
来源：http://iui.feifeiyinyue.top

aiohttp.ClientSession() 配合 async with
来源：http://wak.pycfn.com

[U28] Py：类型别名
来源：http://ugi.tianlin.xyz

UserId = int
来源：http://woz.xziqi.cn

[U29] Py：属性校验
来源：http://azx.gzhubu.top

@property 与 @x.setter 配合
来源：http://edy.ppjwa.cn

[U30] Py：数据类
来源：http://wgv.yuanzhike.top

@dataclass(slots=True)
来源：http://dld.xinyue.icu

[U31] Py：单测
来源：http://bnh.jianghu66.top

python -m pytest -q
来源：http://vll.jinqigfzy.top

[U32] Py：代码格式化
来源：http://qno.chenlongwang.top

ruff format . && ruff check --fix .
来源：http://luw.chenlongwang.top

[U33] Py：打包发布
来源：http://qug.fktsv.cn

python -m build  （依赖 pyproject.toml）
来源：http://lcy.ehwqpu.com

[U34] Py：判断编码
来源：http://irt.uphjek.com

chardet.detect(raw)
来源：http://pxq.vehdjk.com

[U35] Py：发送邮件
来源：http://sbj.yanxiufei.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://guc.ppjwa.cn

[U36] Py：定时任务
来源：http://inu.guowangkeji.top

schedule.every(10).minutes.do(job)
来源：http://cee.zhoulong.xyz

[U37] Py：读写 Excel
来源：http://eqq.shanyushiyangkeji.top

pandas.read_excel / DataFrame.to_excel
来源：http://tmh.jqgufenzy.top

[U38] Py：获取脚本所在目录
来源：http://kdo.chenjidiqi.icu

Path(__file__).resolve().parent
来源：http://zeu.sjlbkw.cn

[U39] Py：判断是否在交互环境
来源：http://rft.andypj.xyz

sys.stdout.isatty()
来源：http://xwx.sxryk.cn

[U40] Py：打印到标准错误
来源：http://qpw.zhijiandao.cn

print("err", file=sys.stderr)
来源：http://oor.mhx1999.top


<!-- 参考信息 -->