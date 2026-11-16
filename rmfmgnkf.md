代发 wailian999

int main(int argc, char **argv)
来源：http://eqm.xuanzx.com

[S19] C：快速排序
来源：http://lse.tian-w.cn

qsort(a, n, sizeof(int), cmp);
来源：http://pwd.fzhhl.top

[S20] C：二分查找
来源：http://fby.gzhubu.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kgv.wangdashe.top

[S21] C：字符类别判断
来源：http://wrl.chenlongwang.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sfg.zdbjq.cn

[S22] C：字符串转数字
来源：http://ypv.kuanghao11.cn

atoi("42");  strtod("3.14", NULL);
来源：http://wzi.guowangkeji.top

[S23] C：随机数
来源：http://dei.jyoumei.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bmb.zhixingplan.top

[S24] C：获取本地时间
来源：http://hty.ppjwa.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vpv.xinyue.icu

[S25] C：内存拷贝
来源：http://qsd.jiagoushi.top

memcpy(dst, src, n);
来源：http://ehd.tarul.cn

[S26] C：内存清零
来源：http://pux.hfpthk.cn

memset(a, 0, sizeof a);
来源：http://oxa.cheryme.top

[S27] C：定义常量
来源：http://jzm.dianchejie.cn

const double PI = 3.14159;
来源：http://qbo.hesvh.cn

[S28] C：静态变量
来源：http://zke.fktsv.cn

static int counter = 0;
来源：http://voo.vqdsnc.cn

[S29] C：变参函数
来源：http://vkk.birdmap.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fsc.birdmap.top

[S30] C：头文件保护
来源：http://dhi.jinghuilouyu.cn

#ifndef X_H
来源：http://qhc.tian-w.cn

#define X_H
来源：http://qfw.zycfv.cn

#endif
来源：http://hzl.fanxiaobao.xyz

[S31] C++：Hello World
来源：http://xkb.zhijiandao.cn

#include <iostream>
来源：http://ckf.zhiwuduotai.top

int main() { std::cout << "Hello\n"; }
来源：http://rdi.fzhhl.top

[S32] C++：字符串
来源：http://tzi.vehdjk.com

std::string s = "hi";  s += "!";
来源：http://ejp.zhiwuduotai.top

[S33] C++：vector 增删
来源：http://fot.ehwqpu.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ddq.tianlin.xyz

[S34] C++：遍历 vector
来源：http://usz.zdbjq.cn

for (auto &x : v) { std::cout << x; }
来源：http://huo.andypj.xyz

[S35] C++：map
来源：http://bda.shanyushiyangtech.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ena.sxryk.cn

[S36] C++：unordered_map
来源：http://fav.svipenyu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://csi.zhongyouzk.top

[S37] C++：set
来源：http://ffi.svipenyu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://sfv.epnwcf.com

[S38] C++：排序
来源：http://uhb.aibaodan.cn

std::sort(v.begin(), v.end());
来源：http://fxz.ppjwa.cn

[S39] C++：自定义比较器排序
来源：http://fgx.sufxvd.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://stl.daxiang520.top

[S40] C++：查找元素
来源：http://hvu.bjfxy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qpi.gaohongyu789.top

[S41] C++：类与构造函数
来源：http://enr.yangfankeji.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yjj.fehbvm.com

[S42] C++：继承与虚函数
来源：http://lxo.yangfankeji.com

class B : public Base { public: void f() override {} };
来源：http://pwn.snrcjt.cn

[S43] C++：智能指针
来源：http://ozs.yanxiufei.cn

auto p = std::make_unique<int>(5);
来源：http://rup.aizwys.cn

[S44] C++：引用传参
来源：http://fvy.hnqzz.top

void inc(int &x) { ++x; }
来源：http://szd.ehwqpu.com

[S45] C++：lambda
来源：http://rna.0kj1m.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ooo.chenjidiqi.icu

[S46] C++：函数模板
来源：http://aoh.tianlin.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bhj.hysaishi.cn

[S47] C++：结构化绑定遍历
来源：http://rmn.yfazqb.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rkm.cdnleiting.top

[S48] C++：逐行读文件
来源：http://anj.hongshengwenyu.top

std::ifstream in("a.txt");  std::string line;
来源：http://frj.chenzaomai.com

while (std::getline(in, line)) { }
来源：http://yah.shangyingyoupin.top

[S49] C++：写文件
来源：http://tyf.jinqigufen.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wzf.epnwcf.com

[S50] C++：格式化数字
来源：http://rxb.zhiwuduotai.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://opv.bjfxy.top

[S51] C++：显式类型转换
来源：http://uog.tanke756.top

static_cast<double>(a) / b
来源：http://zdw.feifeiyinyue.top

[S52] C++：const 与 noexcept
来源：http://rdx.jlsjyb.cn

int size() const noexcept { return n_; }
来源：http://bbl.quarkkingdee.top

[S53] C++：移动语义
来源：http://vzh.ydzc1.top

std::vector<int> w = std::move(v);
来源：http://ioa.jinyuanbaomall.cn

[S54] C++：异常处理
来源：http://bqp.bbcook.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tqt.gzhubu.top

[S55] C++：结构化绑定
来源：http://ula.uphjek.com

auto [a, b] = std::make_pair(1, 2);
来源：http://qpr.jinqigufen.top

[S56] C++：optional
来源：http://fxi.xinyue.icu

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://imw.hammf.cn

[S57] C++：编译期常量
来源：http://sez.sxryk.cn

constexpr int N = 10;
来源：http://ssv.cucudq.cn

[S58] C++：命名空间
来源：http://riu.ppjwa.cn

namespace ns { int f() { return 1; } }
来源：http://qzo.yfazqb.com

[S59] C++：静态断言
来源：http://ijf.pycfn.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ddt.zhongyouzk.top

[S60] C++：遍历并删除元素
来源：http://evx.fanxiaobao.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ith.shangyingyoupin.top

================================================================================
来源：http://ifu.svipenyu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://oqy.hysaishi.cn

================================================================================
来源：http://qgi.hfpthk.cn

[T01] Kotlin：Hello World
来源：http://qjs.sxryk.cn

println("Hello")
来源：http://rsq.hysaishi.cn

[T02] Kotlin：变量
来源：http://cbp.jqgufenzy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sby.chenlongwang.top

[T03] Kotlin：字符串模板
来源：http://kgo.gogol.net.cn

"值: $b"
来源：http://rdm.chenzaomai.com

[T04] Kotlin：空安全
来源：http://cic.zhiwuduotai.top

val n: String? = null;  n?.length
来源：http://blu.pycfn.com

[T05] Kotlin：when 表达式
来源：http://oio.daria6918.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://oue.nwbrower.top

[T06] Kotlin：集合映射
来源：http://bmf.zhoulong.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://sni.gotoacloud.top

[T07] Kotlin：集合过滤
来源：http://hny.0kj1m.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wdy.smart0.xyz

[T08] Kotlin：数据类
来源：http://src.haohaochexian.top

data class User(val name: String, val age: Int)
来源：http://aae.xinyue.icu

[T09] Kotlin：扩展函数
来源：http://kal.chenlongwang.top

fun String.exclaim() = this + "!"
来源：http://kah.cashguo.top

[T10] Kotlin：默认参数
来源：http://lcc.jinyuanbaomall.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://hap.jiagoushi.top

[T11] Kotlin：协程
来源：http://ljz.daxiang520.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://vzy.hnxiangtu.top

[T12] Kotlin：解构声明
来源：http://rdb.ydjk.org.cn

val (a, b) = Pair(1, 2)
来源：http://gai.316326.xyz

[T13] Kotlin：只读 Map
来源：http://mvb.gzhubu.top

val m = mapOf("a" to 1)
来源：http://cpv.zhongyouzk.top

[T14] Kotlin：循环
来源：http://akh.nanxuanxn.top

for (i in 1..10) println(i)
来源：http://dxy.zhijiandao.cn

[T15] Kotlin：接口
来源：http://ahl.meibo888.top

interface Shape { fun area(): Double }
来源：http://nbb.yj20258.top

[T16] Swift：Hello World
来源：http://ytk.gotoacloud.top

print("Hello")
来源：http://ebs.guannengcc.top

[T17] Swift：变量与常量
来源：http://jka.aizwys.cn

var a = 1;  let b = 2
来源：http://shg.shangyingyoupin.top

[T18] Swift：字符串插值
来源：http://jmy.chenzaomai.com

"值: \(b)"
来源：http://bbn.316326.xyz

[T19] Swift：可选绑定
来源：http://xtj.hnqzz.top

if let n = opt { print(n) }
来源：http://occ.zhengqikj.top

[T20] Swift：数组操作
来源：http://wqa.yuxming.cn

var a = [1, 2, 3];  a.append(4)
来源：http://pkn.sxryk.cn

[T21] Swift：遍历
来源：http://vkw.yj20258.top

for x in a { print(x) }
来源：http://jrr.pengpengdd.cyou

[T22] Swift：字典
来源：http://kcy.gogol.net.cn

var d = ["a": 1];  d["b"] = 2
来源：http://icz.fzhhl.top

[T23] Swift：函数
来源：http://lng.zdqjudy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ycp.guowangkeji.top

[T24] Swift：闭包
来源：http://vkj.52xcode.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xot.zhixingplan.top

[T25] Swift：结构体
来源：http://ywl.dashuyun.cn

struct P { var x: Int }
来源：http://vkc.yfazqb.com

[T26] Swift：类与重写
来源：http://foy.316326.xyz

class A: Base { override func f() {} }
来源：http://ron.svipenyu.cn

[T27] Swift：错误处理
来源：http://smx.zhoulong.xyz

do { try f() } catch { print(error) }
来源：http://nmm.chenjidiqi.icu

[T28] Swift：枚举
来源：http://flh.cashguo.top

enum Color { case red, green }
来源：http://bhy.cdnleiting.top

[T29] Swift：guard 提前返回
来源：http://qis.chenlongwang.top

guard let x = opt else { return }
来源：http://rjk.sysykeji.top

[T30] Swift：协议
来源：http://zhb.ctjpmb.com

protocol Shape { func area() -> Double }
来源：http://ffy.jqgfzy.top

[T31] Lua：Hello World
来源：http://usx.yj20258.top

print("Hello")
来源：http://rgw.svipenyu.cn

[T32] Lua：局部变量
来源：http://gtn.yvedp.cn

local a = 1
来源：http://dpx.yj202588.top

[T33] Lua：表（数组）
来源：http://klk.haohaochexian.top

local t = {1, 2, 3};  t[4] = 4
来源：http://wxo.jlsjyb.cn

[T34] Lua：遍历表
来源：http://gxu.sweek.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ldy.cqqwz.cn

[T35] Lua：字典表
来源：http://wlw.gotoacloud.top

local d = { a = 1 };  d.b = 2
来源：http://axm.wangshuangyany.cn

[T36] Lua：函数
来源：http://kff.jinyuanbaomall.cn

function add(a, b) return a + b end
来源：http://xiu.fengsongda.top

[T37] Lua：字符串拼接
来源：http://gss.quarkkingdee.top

"a" .. "b"
来源：http://sso.haohaochexian.top

[T38] Lua：条件
来源：http://cul.cdnleiting.top

if x > 0 then print("正") end
来源：http://lfo.mhx1999.top

[T39] Lua：模式匹配
来源：http://vlh.cdnleiting.top

string.find(s, "%d+")
来源：http://cej.jianghu66.top

[T40] Lua：元表
来源：http://zjk.dianchejie.cn

setmetatable({}, { __index = base })
来源：http://cma.smart0.xyz

[T41] Perl：Hello World
来源：http://jpn.ivvv.top

print "Hello\n";
来源：http://jvg.yongpay.top

[T42] Perl：变量类型
来源：http://xrc.nanxinkj.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ohr.ctjpmb.com

[T43] Perl：字符串插值
来源：http://odi.hywenlv.cn

"值: $a"
来源：http://ttv.zhengqikj.top

[T44] Perl：条件
来源：http://fhv.havefunace.top

if ($a > 0) { print "正"; }
来源：http://nly.smart0.xyz

[T45] Perl：数组遍历
来源：http://gmh.vqdsnc.cn

for my $x (@arr) { print $x; }
来源：http://wsr.nanxuanxn.top

[T46] Perl：哈希操作
来源：http://enh.nwbrower.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://yuj.daria6918.cn

[T47] Perl：正则捕获
来源：http://mrm.hammf.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://kbd.xinyue.icu

[T48] Perl：正则替换
来源：http://che.yanxiufei.cn

$s =~ s/old/new/g;
来源：http://cyn.gaohongyu789.top

[T49] Perl：函数
来源：http://dxn.tanke756.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ijr.ydzc1.top

[T50] Perl：逐行读文件
来源：http://mpi.chenjidiqi.icu

open my $fh, "<", "a.txt" or die $!;
来源：http://wmz.zhaomingkeji.xyz

while (my $line = <$fh>) { print $line; }
来源：http://mvq.hywenlv.cn

[T51] Scala：Hello World
来源：http://mxi.fengsongda.top

println("Hello")
来源：http://jeh.yvedp.cn

[T52] Scala：变量
来源：http://hug.tianlin.xyz

val a = 1;  var b = 2
来源：http://cvo.ppjwa.cn

[T53] Scala：字符串插值
来源：http://yck.zhoulong.xyz

s"值: $b"
来源：http://vcm.yuanzhike.top

[T54] Scala：集合映射
来源：http://epp.chenzaomai.com

List(1, 2, 3).map(_ * 2)
来源：http://ody.sjlbkw.cn

[T55] Scala：集合过滤
来源：http://pnj.cashguo.top

List(1, 2, 3).filter(_ > 1)
来源：http://lxg.zhaomingkeji.xyz

[T56] Scala：样例类
来源：http://jzo.sweek.top

case class User(name: String, age: Int)
来源：http://vvz.9152youxi.cn

[T57] Scala：模式匹配
来源：http://nzm.shzxlz.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://elt.yongpay.top

[T58] Scala：函数定义
来源：http://jyt.jinqigufen.top

def add(a: Int, b: Int): Int = a + b
来源：http://fqo.cqqwz.cn

[T59] Scala：循环
来源：http://bhb.gogol.net.cn

for (i <- 1 to 10) println(i)
来源：http://lap.zhoulong.xyz

[T60] Scala：折叠
来源：http://qke.52xcode.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xtj.pycfn.com

================================================================================
来源：http://dej.zhongyouzk.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hir.meibo888.top

================================================================================
来源：http://gpy.chenzaomai.com

[U01] Py：创建虚拟环境
来源：http://ucq.svipenyu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://sti.hywenlv.cn

[U02] Py：导出 / 安装依赖
来源：http://pte.daxiang520.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vhx.hnqzz.top

[U03] Py：加载 .env 配置
来源：http://heh.ppjwa.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xwm.hysaishi.cn

[U04] Py：变量调试打印
来源：http://kae.shangyingyoupin.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wnf.hesvh.cn

[U05] Py：列表去重且保序
来源：http://fnb.aizwys.cn

list(dict.fromkeys(arr))
来源：http://nlx.zhijiandao.cn

[U06] Py：合并两个字典
来源：http://mrc.chenzaomai.com

{**a, **b}
来源：http://ldx.yueranfly.top

[U07] Py：反转字典键值
来源：http://jiz.yvedp.cn

{v: k for k, v in d.items()}
来源：http://htl.jinyuanbaomall.cn

[U08] Py：展平二维列表
来源：http://bfm.iojbl.cn

[y for x in nested for y in x]
来源：http://cyx.guannengcc.top

[U09] Py：字典取最大值的键
来源：http://hcj.guowangkeji.top

max(d, key=d.get)
来源：http://lnn.gotoacloud.top

[U10] Py：按值排序字典
来源：http://rch.andypj.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pbv.gzhubu.top

[U11] Py：生成器表达式
来源：http://hnb.yangfankeji.com

(x * 2 for x in arr)
来源：http://ncs.aibaodan.cn

[U12] Py：取出现最多的 3 个元素
来源：http://kkf.hammf.cn

Counter(arr).most_common(3)
来源：http://spc.yj20258888.top

[U13] Py：固定长度队列
来源：http://tdm.uphjek.com

deque(maxlen=10)
来源：http://pym.gogol.net.cn

[U14] Py：分组收集到列表
来源：http://kkw.fktsv.cn

defaultdict(list)
来源：http://plo.zycfv.cn

[U15] Py：高精度计时
来源：http://ote.jinyuanbaomall.cn

t = time.perf_counter()
来源：http://zjk.hywenlv.cn

[U16] Py：命令行参数解析
来源：http://wjk.vqdsnc.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bwu.fzhhl.top

[U17] Py：初始化日志
来源：http://ifg.meibo888.top

logging.basicConfig(level=logging.INFO)
来源：http://eqp.yangfankeji.com

[U18] Py：预编译正则
来源：http://bco.hcnkem.com

pat = re.compile(r"\d+")
来源：http://dip.meibo888.top

[U19] Py：正则替换带回调
来源：http://awx.hnqzz.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xvv.shanyushiyangtech.top

[U20] Py：缓存函数结果
来源：http://ukr.zdqjudy.top

@functools.lru_cache(maxsize=None)
来源：http://lfw.hammf.cn

[U21] Py：自定义上下文管理器
来源：http://yip.yj202588.top

@contextlib.contextmanager
来源：http://vbq.yonumen.top

[U22] Py：矩阵转置
来源：http://fsa.redwolf501.top

list(zip(*m))
来源：http://exs.mhx1999.top

[U23] Py：分块读取大文件
来源：http://njf.yfazqb.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://voz.dianchejie.cn

[U24] Py：路径操作
来源：http://fng.yonumen.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hlo.cqqwz.cn

[U25] Py：CSV 按字典读
来源：http://bwo.jqgufenzy.top

csv.DictReader(f)
来源：http://skk.zhixingplan.top

[U26] Py：并发下载
来源：http://wng.chenzaomai.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://kcq.bjfxy.top

[U27] Py：异步 HTTP
来源：http://guu.birdmap.top

aiohttp.ClientSession() 配合 async with
来源：http://nfw.andypj.xyz

[U28] Py：类型别名
来源：http://dsz.hammf.cn

UserId = int
来源：http://akx.hysaishi.cn

[U29] Py：属性校验
来源：http://xff.jinyuanbaomall.cn

@property 与 @x.setter 配合
来源：http://gbj.epnwcf.com

[U30] Py：数据类
来源：http://wsz.daxiang520.top

@dataclass(slots=True)
来源：http://cdp.yj20258.top

[U31] Py：单测
来源：http://sub.zhoulong.xyz

python -m pytest -q
来源：http://guh.jinyuanbaomall.cn

[U32] Py：代码格式化
来源：http://hrc.yj20258888.top

ruff format . && ruff check --fix .
来源：http://diu.uphjek.com

[U33] Py：打包发布
来源：http://cag.chenlongwang.top

python -m build  （依赖 pyproject.toml）
来源：http://yjs.ywan-chungtsiang.top

[U34] Py：判断编码
来源：http://fzb.jinqigufen.top

chardet.detect(raw)
来源：http://jxl.xuetiantiany.cn

[U35] Py：发送邮件
来源：http://lgq.shanyushiyangtech.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qci.jyoumei.cn

[U36] Py：定时任务
来源：http://ipu.fengsongda.top

schedule.every(10).minutes.do(job)
来源：http://oie.shangyingyoupin.top

[U37] Py：读写 Excel
来源：http://gig.fzhhl.top

pandas.read_excel / DataFrame.to_excel
来源：http://exa.ybcxt.top

[U38] Py：获取脚本所在目录
来源：http://bzm.epnwcf.com

Path(__file__).resolve().parent
来源：http://xyc.fktsv.cn

[U39] Py：判断是否在交互环境
来源：http://nam.redwolf501.top

sys.stdout.isatty()
来源：http://kif.vehdjk.com

[U40] Py：打印到标准错误
来源：http://iva.ywan-chungtsiang.top

print("err", file=sys.stderr)
来源：http://nbr.bbcook.cn

[U41] PHP：初始化 Composer 项目
来源：http://tla.haohaochexian.top

composer init;  composer require guzzlehttp/guzzle
来源：http://mlf.iojbl.cn

[U42] PHP：PSR-4 自动加载
来源：http://qhn.birdmap.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ldv.sufxvd.cn


<!-- 参考信息 -->