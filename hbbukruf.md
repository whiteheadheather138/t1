代发 wailian999

int main(int argc, char **argv)
来源：http://zyw.nwbrower.top

[S19] C：快速排序
来源：http://ajg.vehdjk.com

qsort(a, n, sizeof(int), cmp);
来源：http://drs.redwolf501.top

[S20] C：二分查找
来源：http://jbh.tian-w.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uxb.sysykeji.top

[S21] C：字符类别判断
来源：http://vnc.zdbjq.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lbi.ybcxt.top

[S22] C：字符串转数字
来源：http://jig.sysykeji.top

atoi("42");  strtod("3.14", NULL);
来源：http://xyh.fzhhl.top

[S23] C：随机数
来源：http://bwx.hfpthk.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://gfu.jinyuanbaomall.cn

[S24] C：获取本地时间
来源：http://eyi.wangshuangyany.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lcr.epnwcf.com

[S25] C：内存拷贝
来源：http://wxe.tian-w.cn

memcpy(dst, src, n);
来源：http://wog.wangdashe.top

[S26] C：内存清零
来源：http://uad.gogol.net.cn

memset(a, 0, sizeof a);
来源：http://qin.guowangkeji.top

[S27] C：定义常量
来源：http://wkn.xinyue.icu

const double PI = 3.14159;
来源：http://ybl.zhiwuduotai.top

[S28] C：静态变量
来源：http://sez.feifeiyinyue.top

static int counter = 0;
来源：http://xsu.xylfe.cn

[S29] C：变参函数
来源：http://pcl.yj20258888.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lay.ydjk.org.cn

[S30] C：头文件保护
来源：http://xjd.jqgfzy.top

#ifndef X_H
来源：http://ljh.ybcxt.top

#define X_H
来源：http://nkh.hammf.cn

#endif
来源：http://uxy.shanyushiyangkeji.top

[S31] C++：Hello World
来源：http://qrq.tianlin.xyz

#include <iostream>
来源：http://ick.xylfe.cn

int main() { std::cout << "Hello\n"; }
来源：http://bhs.fehbvm.com

[S32] C++：字符串
来源：http://hpz.andypj.xyz

std::string s = "hi";  s += "!";
来源：http://ihn.jinghuilouyu.cn

[S33] C++：vector 增删
来源：http://zwv.zhiwuduotai.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mjy.fktsv.cn

[S34] C++：遍历 vector
来源：http://ddd.sysykeji.top

for (auto &x : v) { std::cout << x; }
来源：http://pjj.ydjk.org.cn

[S35] C++：map
来源：http://ekk.bbcook.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://apx.uphjek.com

[S36] C++：unordered_map
来源：http://rfn.tanke756.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ywv.9152youxi.cn

[S37] C++：set
来源：http://dxz.ppjwa.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wtw.daria6918.cn

[S38] C++：排序
来源：http://odp.yuanzhike.top

std::sort(v.begin(), v.end());
来源：http://xpx.xuanzx.com

[S39] C++：自定义比较器排序
来源：http://hjs.zhoulong.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cao.zhoulong.xyz

[S40] C++：查找元素
来源：http://vim.yueranfly.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lrb.gaohongyu789.top

[S41] C++：类与构造函数
来源：http://pop.sjlbkw.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vbh.sjlbkw.cn

[S42] C++：继承与虚函数
来源：http://tgx.shanyushiyangkeji.top

class B : public Base { public: void f() override {} };
来源：http://bgt.hysaishi.cn

[S43] C++：智能指针
来源：http://gdf.yj20258888.top

auto p = std::make_unique<int>(5);
来源：http://gew.dianchejie.cn

[S44] C++：引用传参
来源：http://yql.zycfv.cn

void inc(int &x) { ++x; }
来源：http://auu.sufxvd.cn

[S45] C++：lambda
来源：http://gtg.zdbjq.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wfi.316326.xyz

[S46] C++：函数模板
来源：http://mjn.tianlin.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ylf.fzhhl.top

[S47] C++：结构化绑定遍历
来源：http://qoh.ydzc1.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pcq.ivvv.top

[S48] C++：逐行读文件
来源：http://zlo.jinyuanbaomall.cn

std::ifstream in("a.txt");  std::string line;
来源：http://qjp.zhijiandao.cn

while (std::getline(in, line)) { }
来源：http://kuh.yuanzhike.top

[S49] C++：写文件
来源：http://zcx.shanyushiyangtech.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://klf.chenzaomai.com

[S50] C++：格式化数字
来源：http://sfo.pengpengdd.cyou

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ydk.shangyingyoupin.top

[S51] C++：显式类型转换
来源：http://bbk.havefunace.top

static_cast<double>(a) / b
来源：http://nja.tian-w.cn

[S52] C++：const 与 noexcept
来源：http://dpr.wangshuangyany.cn

int size() const noexcept { return n_; }
来源：http://kaw.snrcjt.cn

[S53] C++：移动语义
来源：http://rts.xuetiantiany.cn

std::vector<int> w = std::move(v);
来源：http://epn.hywenlv.cn

[S54] C++：异常处理
来源：http://cpy.hysaishi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mpy.ivvv.top

[S55] C++：结构化绑定
来源：http://bej.vqdsnc.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://nax.dianchejie.cn

[S56] C++：optional
来源：http://qnm.yongpay.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ahh.meibo888.top

[S57] C++：编译期常量
来源：http://bjw.316326.xyz

constexpr int N = 10;
来源：http://uut.zhoulong.xyz

[S58] C++：命名空间
来源：http://acv.pengpengdd.cyou

namespace ns { int f() { return 1; } }
来源：http://sil.chenjidiqi.icu

[S59] C++：静态断言
来源：http://zpb.tarul.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dqn.aibaodan.cn

[S60] C++：遍历并删除元素
来源：http://vlp.gaohongyu789.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yea.shangyingyoupin.top

================================================================================
来源：http://rel.yueranfly.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://iqi.xziqi.cn

================================================================================
来源：http://kpo.yfazqb.com

[T01] Kotlin：Hello World
来源：http://wta.hysaishi.cn

println("Hello")
来源：http://suz.ydjk.org.cn

[T02] Kotlin：变量
来源：http://dny.chenzaomai.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zwt.gogol.net.cn

[T03] Kotlin：字符串模板
来源：http://uoh.zdbjq.cn

"值: $b"
来源：http://yyh.andypj.xyz

[T04] Kotlin：空安全
来源：http://jhf.0kj1m.cn

val n: String? = null;  n?.length
来源：http://tlj.zhengqikj.top

[T05] Kotlin：when 表达式
来源：http://cob.jinyuanbaomall.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cmg.jyoumei.cn

[T06] Kotlin：集合映射
来源：http://cnj.bbcook.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://jfz.tianlin.xyz

[T07] Kotlin：集合过滤
来源：http://szw.jlsjyb.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://rjy.52xcode.cn

[T08] Kotlin：数据类
来源：http://wvy.pycfn.com

data class User(val name: String, val age: Int)
来源：http://usx.sweek.top

[T09] Kotlin：扩展函数
来源：http://vhj.ydjk.org.cn

fun String.exclaim() = this + "!"
来源：http://qlu.jiagoushi.top

[T10] Kotlin：默认参数
来源：http://rqg.chenlongwang.top

fun greet(name: String = "World") = "Hi $name"
来源：http://mro.zhixingplan.top

[T11] Kotlin：协程
来源：http://emf.daria6918.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://foj.snrcjt.cn

[T12] Kotlin：解构声明
来源：http://qio.tarul.cn

val (a, b) = Pair(1, 2)
来源：http://qpb.iojbl.cn

[T13] Kotlin：只读 Map
来源：http://tms.cqqwz.cn

val m = mapOf("a" to 1)
来源：http://ekf.zhengqikj.top

[T14] Kotlin：循环
来源：http://yxp.zhixingplan.top

for (i in 1..10) println(i)
来源：http://sjw.ydjk.org.cn

[T15] Kotlin：接口
来源：http://uoq.xingfuxueyuan.xyz

interface Shape { fun area(): Double }
来源：http://uck.shuidangran.top

[T16] Swift：Hello World
来源：http://fhv.xuanzx.com

print("Hello")
来源：http://tgu.zhijiandao.cn

[T17] Swift：变量与常量
来源：http://gyb.yueranfly.top

var a = 1;  let b = 2
来源：http://ylw.yuanzhike.top

[T18] Swift：字符串插值
来源：http://qqi.havefunace.top

"值: \(b)"
来源：http://dzp.fanxiaobao.xyz

[T19] Swift：可选绑定
来源：http://nvf.jiagoushi.top

if let n = opt { print(n) }
来源：http://wcy.cheryme.top

[T20] Swift：数组操作
来源：http://ekl.cucudq.cn

var a = [1, 2, 3];  a.append(4)
来源：http://mql.jlsjyb.cn

[T21] Swift：遍历
来源：http://pwq.zhiwuduotai.top

for x in a { print(x) }
来源：http://ofy.ydzc1.top

[T22] Swift：字典
来源：http://oqe.zhaomingkeji.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://wyu.pycfn.com

[T23] Swift：函数
来源：http://ybl.yuanzhike.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ssm.ehwqpu.com

[T24] Swift：闭包
来源：http://jcs.zhaomingkeji.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://dhi.hnqzz.top

[T25] Swift：结构体
来源：http://xbq.jinqigfzy.top

struct P { var x: Int }
来源：http://ujg.9152youxi.cn

[T26] Swift：类与重写
来源：http://bll.nanxuanxn.top

class A: Base { override func f() {} }
来源：http://ohy.meibo888.top

[T27] Swift：错误处理
来源：http://pvd.shanyushiyangtech.top

do { try f() } catch { print(error) }
来源：http://gze.sweek.top

[T28] Swift：枚举
来源：http://jrs.fzhhl.top

enum Color { case red, green }
来源：http://lyp.zhixingplan.top

[T29] Swift：guard 提前返回
来源：http://eqb.nwbrower.top

guard let x = opt else { return }
来源：http://eiz.sjlbkw.cn

[T30] Swift：协议
来源：http://zpl.daxiang520.top

protocol Shape { func area() -> Double }
来源：http://rog.ppjwa.cn

[T31] Lua：Hello World
来源：http://ink.hongshengwenyu.top

print("Hello")
来源：http://rdb.havefunace.top

[T32] Lua：局部变量
来源：http://ovs.yongpay.top

local a = 1
来源：http://cnc.c1oappe.top

[T33] Lua：表（数组）
来源：http://azy.gogol.net.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ydk.yonumen.top

[T34] Lua：遍历表
来源：http://wvk.birdmap.top

for i, v in ipairs(t) do print(i, v) end
来源：http://qle.ppjwa.cn

[T35] Lua：字典表
来源：http://eye.ywan-chungtsiang.top

local d = { a = 1 };  d.b = 2
来源：http://kqd.yj20258888.top

[T36] Lua：函数
来源：http://plo.sxryk.cn

function add(a, b) return a + b end
来源：http://dtj.hcnkem.com

[T37] Lua：字符串拼接
来源：http://ani.iojbl.cn

"a" .. "b"
来源：http://pce.iojbl.cn

[T38] Lua：条件
来源：http://uql.chenlongwang.top

if x > 0 then print("正") end
来源：http://jii.jinqigufen.top

[T39] Lua：模式匹配
来源：http://ytz.zdqjudy.top

string.find(s, "%d+")
来源：http://ica.hywenlv.cn

[T40] Lua：元表
来源：http://eur.zhiwuduotai.top

setmetatable({}, { __index = base })
来源：http://ahe.nanxuanxn.top

[T41] Perl：Hello World
来源：http://snj.mhx1999.top

print "Hello\n";
来源：http://qzv.ppjwa.cn

[T42] Perl：变量类型
来源：http://pwk.yueranfly.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xsh.jiagoushi.top

[T43] Perl：字符串插值
来源：http://slg.yj20258888.top

"值: $a"
来源：http://lww.zhongyouzk.top

[T44] Perl：条件
来源：http://aye.sweek.top

if ($a > 0) { print "正"; }
来源：http://jnh.cdnleiting.top

[T45] Perl：数组遍历
来源：http://ftv.nwbrower.top

for my $x (@arr) { print $x; }
来源：http://llt.jianghu66.top

[T46] Perl：哈希操作
来源：http://inh.bjfxy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cdl.jinyuanbaomall.cn

[T47] Perl：正则捕获
来源：http://qed.iojbl.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://dyo.ywan-chungtsiang.top

[T48] Perl：正则替换
来源：http://vmt.yanxiufei.cn

$s =~ s/old/new/g;
来源：http://huq.quarkkingdee.top

[T49] Perl：函数
来源：http://yub.gaohongyu789.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qia.ctjpmb.com

[T50] Perl：逐行读文件
来源：http://nbs.zhixingplan.top

open my $fh, "<", "a.txt" or die $!;
来源：http://rkx.cqqwz.cn

while (my $line = <$fh>) { print $line; }
来源：http://rvh.yj20258.top

[T51] Scala：Hello World
来源：http://rzb.nanxinkj.top

println("Hello")
来源：http://tqa.yangfankeji.com

[T52] Scala：变量
来源：http://uuk.ctjpmb.com

val a = 1;  var b = 2
来源：http://afx.epnwcf.com

[T53] Scala：字符串插值
来源：http://wlo.fzhhl.top

s"值: $b"
来源：http://rxj.pengpengdd.cyou

[T54] Scala：集合映射
来源：http://mmh.tarul.cn

List(1, 2, 3).map(_ * 2)
来源：http://ixo.sweek.top

[T55] Scala：集合过滤
来源：http://thl.yj20258888.top

List(1, 2, 3).filter(_ > 1)
来源：http://mwb.cheryme.top

[T56] Scala：样例类
来源：http://tzl.hesvh.cn

case class User(name: String, age: Int)
来源：http://pgx.shzxlz.cn

[T57] Scala：模式匹配
来源：http://rca.smart0.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://sht.fktsv.cn

[T58] Scala：函数定义
来源：http://xne.shangyingyoupin.top

def add(a: Int, b: Int): Int = a + b
来源：http://yvz.zycfv.cn

[T59] Scala：循环
来源：http://tjj.jianghu66.top

for (i <- 1 to 10) println(i)
来源：http://vem.sjlbkw.cn

[T60] Scala：折叠
来源：http://fwv.ydjk.org.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nxp.nanxuanxn.top

================================================================================
来源：http://aqq.bjfxy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://agg.dianchejie.cn

================================================================================
来源：http://uem.jinyuanbaomall.cn

[U01] Py：创建虚拟环境
来源：http://axh.xuanzx.com

python -m venv .venv && source .venv/bin/activate
来源：http://xvz.kuanghao11.cn

[U02] Py：导出 / 安装依赖
来源：http://dsa.tianlin.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hjs.ybcxt.top

[U03] Py：加载 .env 配置
来源：http://aet.sweek.top

from dotenv import load_dotenv; load_dotenv()
来源：http://pxa.yvedp.cn

[U04] Py：变量调试打印
来源：http://mje.jinyuanbaomall.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lml.nanxuanxn.top

[U05] Py：列表去重且保序
来源：http://nrp.epnwcf.com

list(dict.fromkeys(arr))
来源：http://ppk.yongpay.top

[U06] Py：合并两个字典
来源：http://zqq.dashuyun.cn

{**a, **b}
来源：http://hzh.0kj1m.cn

[U07] Py：反转字典键值
来源：http://ubm.shanyushiyangkeji.top

{v: k for k, v in d.items()}
来源：http://iot.xylfe.cn

[U08] Py：展平二维列表
来源：http://blr.fanxiaobao.xyz

[y for x in nested for y in x]
来源：http://jio.cqqwz.cn

[U09] Py：字典取最大值的键
来源：http://oub.0kj1m.cn

max(d, key=d.get)
来源：http://ovn.fzhhl.top

[U10] Py：按值排序字典
来源：http://jcb.zhaomingkeji.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hzs.cucudq.cn

[U11] Py：生成器表达式
来源：http://mnv.jyoumei.cn

(x * 2 for x in arr)
来源：http://wym.yj202588.top

[U12] Py：取出现最多的 3 个元素
来源：http://jnp.yangfankeji.com

Counter(arr).most_common(3)
来源：http://oby.yongpay.top

[U13] Py：固定长度队列
来源：http://slv.xinyue.icu

deque(maxlen=10)
来源：http://dzg.hnxiangtu.top

[U14] Py：分组收集到列表
来源：http://kik.svipenyu.cn

defaultdict(list)
来源：http://wly.sjlbkw.cn

[U15] Py：高精度计时
来源：http://rec.ydjk.org.cn

t = time.perf_counter()
来源：http://oos.chenjidiqi.icu

[U16] Py：命令行参数解析
来源：http://mlm.jiagoushi.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sqz.uphjek.com

[U17] Py：初始化日志
来源：http://uui.bjfxy.top

logging.basicConfig(level=logging.INFO)
来源：http://rrz.tianlin.xyz

[U18] Py：预编译正则
来源：http://nom.xingfuxueyuan.xyz

pat = re.compile(r"\d+")
来源：http://swh.guowangkeji.top

[U19] Py：正则替换带回调
来源：http://pvn.chenzaomai.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ljh.hnqzz.top

[U20] Py：缓存函数结果
来源：http://pwm.aibaodan.cn

@functools.lru_cache(maxsize=None)
来源：http://tya.yangfankeji.com

[U21] Py：自定义上下文管理器
来源：http://hdt.pycfn.com

@contextlib.contextmanager
来源：http://efz.chenjidiqi.icu

[U22] Py：矩阵转置
来源：http://asc.yonumen.top

list(zip(*m))
来源：http://akz.xylfe.cn

[U23] Py：分块读取大文件
来源：http://hqx.sufxvd.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gzj.316326.xyz

[U24] Py：路径操作
来源：http://jgh.aizwys.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://phj.aibaodan.cn

[U25] Py：CSV 按字典读
来源：http://enx.epnwcf.com

csv.DictReader(f)
来源：http://nws.fzhhl.top

[U26] Py：并发下载
来源：http://lxi.ehwqpu.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lgk.birdmap.top

[U27] Py：异步 HTTP
来源：http://zsw.haohaochexian.top

aiohttp.ClientSession() 配合 async with
来源：http://mdb.jinqigfzy.top

[U28] Py：类型别名
来源：http://cvj.nwbrower.top

UserId = int
来源：http://hir.gzhubu.top

[U29] Py：属性校验
来源：http://iqh.nwbrower.top

@property 与 @x.setter 配合
来源：http://egn.haohaochexian.top

[U30] Py：数据类
来源：http://wxm.haohaochexian.top

@dataclass(slots=True)
来源：http://egw.jianghu66.top

[U31] Py：单测
来源：http://mid.sweek.top

python -m pytest -q
来源：http://cyy.jqgufenzy.top

[U32] Py：代码格式化
来源：http://jxi.jinyuanbaomall.cn

ruff format . && ruff check --fix .
来源：http://asp.ydzc1.top

[U33] Py：打包发布
来源：http://stz.quarkkingdee.top

python -m build  （依赖 pyproject.toml）
来源：http://dbh.yangfankeji.com

[U34] Py：判断编码
来源：http://lhj.sjlbkw.cn

chardet.detect(raw)
来源：http://ine.jinqigfzy.top

[U35] Py：发送邮件
来源：http://lnz.daxiang520.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pzw.aizwys.cn

[U36] Py：定时任务
来源：http://ash.jiagoushi.top

schedule.every(10).minutes.do(job)
来源：http://zgk.dianchejie.cn

[U37] Py：读写 Excel
来源：http://zdc.xuanzx.com

pandas.read_excel / DataFrame.to_excel
来源：http://rla.9152youxi.cn

[U38] Py：获取脚本所在目录
来源：http://isz.shangyingyoupin.top

Path(__file__).resolve().parent
来源：http://uxj.yvedp.cn

[U39] Py：判断是否在交互环境
来源：http://pta.jinqigufen.top

sys.stdout.isatty()
来源：http://pbd.yanxiufei.cn

[U40] Py：打印到标准错误
来源：http://ono.tian-w.cn

print("err", file=sys.stderr)
来源：http://bej.ehwqpu.com

[U41] PHP：初始化 Composer 项目
来源：http://jgl.mhx1999.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ail.bjfxy.top

[U42] PHP：PSR-4 自动加载
来源：http://ztz.cdnleiting.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mlm.vehdjk.com


<!-- 参考信息 -->