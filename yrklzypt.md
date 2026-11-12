代发 wailian999

int main(int argc, char **argv)
来源：http://fwf.kuanghao11.cn

[S19] C：快速排序
来源：http://uim.yuxming.cn

qsort(a, n, sizeof(int), cmp);
来源：http://kym.shanyushiyangkeji.top

[S20] C：二分查找
来源：http://und.xuetiantiany.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ruv.yongpay.top

[S21] C：字符类别判断
来源：http://fzz.hywenlv.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fow.kuanghao11.cn

[S22] C：字符串转数字
来源：http://dew.gogol.net.cn

atoi("42");  strtod("3.14", NULL);
来源：http://fwv.ywan-chungtsiang.top

[S23] C：随机数
来源：http://qfh.nwbrower.top

srand(time(NULL));  int r = rand() % 100;
来源：http://wsx.daria6918.cn

[S24] C：获取本地时间
来源：http://zus.sjlbkw.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bqm.hfpthk.cn

[S25] C：内存拷贝
来源：http://jbl.gogol.net.cn

memcpy(dst, src, n);
来源：http://fkp.xuanzx.com

[S26] C：内存清零
来源：http://bgt.xingfuxueyuan.xyz

memset(a, 0, sizeof a);
来源：http://noz.fehbvm.com

[S27] C：定义常量
来源：http://rwv.cdnleiting.top

const double PI = 3.14159;
来源：http://luj.sweek.top

[S28] C：静态变量
来源：http://brc.hesvh.cn

static int counter = 0;
来源：http://jzm.hnxiangtu.top

[S29] C：变参函数
来源：http://dyv.aibaodan.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xxo.zhiwuduotai.top

[S30] C：头文件保护
来源：http://osa.shangyingyoupin.top

#ifndef X_H
来源：http://zqb.sxryk.cn

#define X_H
来源：http://hpa.hysaishi.cn

#endif
来源：http://dyx.fanxiaobao.xyz

[S31] C++：Hello World
来源：http://dal.ywan-chungtsiang.top

#include <iostream>
来源：http://lng.zdqjudy.top

int main() { std::cout << "Hello\n"; }
来源：http://mrz.hfpthk.cn

[S32] C++：字符串
来源：http://jcp.jqgufenzy.top

std::string s = "hi";  s += "!";
来源：http://rts.jlsjyb.cn

[S33] C++：vector 增删
来源：http://jsl.hywenlv.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pgj.jlsjyb.cn

[S34] C++：遍历 vector
来源：http://hvq.gzhubu.top

for (auto &x : v) { std::cout << x; }
来源：http://bhs.ydjk.org.cn

[S35] C++：map
来源：http://bga.wangdashe.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://iwx.zdbjq.cn

[S36] C++：unordered_map
来源：http://fau.yueranfly.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fha.hysaishi.cn

[S37] C++：set
来源：http://amu.hnqzz.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fxy.xingfuxueyuan.xyz

[S38] C++：排序
来源：http://ask.xuanzx.com

std::sort(v.begin(), v.end());
来源：http://esl.jiagoushi.top

[S39] C++：自定义比较器排序
来源：http://sgu.hnqzz.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mxy.havefunace.top

[S40] C++：查找元素
来源：http://yrr.feifeiyinyue.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://azm.zhongyouzk.top

[S41] C++：类与构造函数
来源：http://zpq.hnxiangtu.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hvr.tanke756.top

[S42] C++：继承与虚函数
来源：http://kcd.hongshengwenyu.top

class B : public Base { public: void f() override {} };
来源：http://ino.hesvh.cn

[S43] C++：智能指针
来源：http://ofb.ydzc1.top

auto p = std::make_unique<int>(5);
来源：http://vta.xuanzx.com

[S44] C++：引用传参
来源：http://nty.yfazqb.com

void inc(int &x) { ++x; }
来源：http://yid.vqdsnc.cn

[S45] C++：lambda
来源：http://tkc.fehbvm.com

auto add = [](int a, int b) { return a + b; };
来源：http://xdh.meibo888.top

[S46] C++：函数模板
来源：http://uuh.cqqwz.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rvd.xylfe.cn

[S47] C++：结构化绑定遍历
来源：http://wsv.fzhhl.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://izd.wangdashe.top

[S48] C++：逐行读文件
来源：http://suf.jyoumei.cn

std::ifstream in("a.txt");  std::string line;
来源：http://crs.ybcxt.top

while (std::getline(in, line)) { }
来源：http://nya.fanxiaobao.xyz

[S49] C++：写文件
来源：http://lmj.hysaishi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mcx.cashguo.top

[S50] C++：格式化数字
来源：http://hqt.vehdjk.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pmw.chenlongwang.top

[S51] C++：显式类型转换
来源：http://pzm.yuanzhike.top

static_cast<double>(a) / b
来源：http://zas.yueranfly.top

[S52] C++：const 与 noexcept
来源：http://kqo.yongpay.top

int size() const noexcept { return n_; }
来源：http://ura.cdnleiting.top

[S53] C++：移动语义
来源：http://ykw.bjfxy.top

std::vector<int> w = std::move(v);
来源：http://sol.sjlbkw.cn

[S54] C++：异常处理
来源：http://eiu.zdbjq.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gzy.yj20258888.top

[S55] C++：结构化绑定
来源：http://var.shangyingyoupin.top

auto [a, b] = std::make_pair(1, 2);
来源：http://fcj.ctjpmb.com

[S56] C++：optional
来源：http://zcn.jianghu66.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xvc.dashuyun.cn

[S57] C++：编译期常量
来源：http://biv.redwolf501.top

constexpr int N = 10;
来源：http://cgf.mhx1999.top

[S58] C++：命名空间
来源：http://cey.hesvh.cn

namespace ns { int f() { return 1; } }
来源：http://qpy.yangfankeji.com

[S59] C++：静态断言
来源：http://ter.xuanzx.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://eyv.316326.xyz

[S60] C++：遍历并删除元素
来源：http://xyo.ybcxt.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cte.zhaomingkeji.xyz

================================================================================
来源：http://nwp.yonumen.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rnp.yj202588.top

================================================================================
来源：http://zma.xinyue.icu

[T01] Kotlin：Hello World
来源：http://vms.jlsjyb.cn

println("Hello")
来源：http://rhh.9152youxi.cn

[T02] Kotlin：变量
来源：http://zje.aizwys.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sgx.cucudq.cn

[T03] Kotlin：字符串模板
来源：http://asb.daxiang520.top

"值: $b"
来源：http://pwx.52xcode.cn

[T04] Kotlin：空安全
来源：http://wrz.sxryk.cn

val n: String? = null;  n?.length
来源：http://lra.yongpay.top

[T05] Kotlin：when 表达式
来源：http://ahc.hammf.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bkn.shanyushiyangtech.top

[T06] Kotlin：集合映射
来源：http://nei.ivvv.top

listOf(1, 2, 3).map { it * 2 }
来源：http://dxi.cucudq.cn

[T07] Kotlin：集合过滤
来源：http://ays.ppjwa.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://blx.hesvh.cn

[T08] Kotlin：数据类
来源：http://lup.aibaodan.cn

data class User(val name: String, val age: Int)
来源：http://gqk.c1oappe.top

[T09] Kotlin：扩展函数
来源：http://caa.jinyuanbaomall.cn

fun String.exclaim() = this + "!"
来源：http://zpf.yanxiufei.cn

[T10] Kotlin：默认参数
来源：http://axa.jinqigfzy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://niw.316326.xyz

[T11] Kotlin：协程
来源：http://ses.nanxuanxn.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://apc.uphjek.com

[T12] Kotlin：解构声明
来源：http://dgt.daxiang520.top

val (a, b) = Pair(1, 2)
来源：http://nzb.zhengqikj.top

[T13] Kotlin：只读 Map
来源：http://tog.zdqjudy.top

val m = mapOf("a" to 1)
来源：http://apq.chenlongwang.top

[T14] Kotlin：循环
来源：http://shm.andypj.xyz

for (i in 1..10) println(i)
来源：http://eeg.yj202588.top

[T15] Kotlin：接口
来源：http://jic.uphjek.com

interface Shape { fun area(): Double }
来源：http://fic.gzhubu.top

[T16] Swift：Hello World
来源：http://nla.shuidangran.top

print("Hello")
来源：http://mmh.aibaodan.cn

[T17] Swift：变量与常量
来源：http://ptr.yueranfly.top

var a = 1;  let b = 2
来源：http://qqm.birdmap.top

[T18] Swift：字符串插值
来源：http://zmd.chenzaomai.com

"值: \(b)"
来源：http://oeb.havefunace.top

[T19] Swift：可选绑定
来源：http://zyi.dianchejie.cn

if let n = opt { print(n) }
来源：http://exr.jiagoushi.top

[T20] Swift：数组操作
来源：http://zud.chenlongwang.top

var a = [1, 2, 3];  a.append(4)
来源：http://bny.feifeiyinyue.top

[T21] Swift：遍历
来源：http://lon.gzhubu.top

for x in a { print(x) }
来源：http://zof.xuetiantiany.cn

[T22] Swift：字典
来源：http://kvw.52xcode.cn

var d = ["a": 1];  d["b"] = 2
来源：http://nvx.pengpengdd.cyou

[T23] Swift：函数
来源：http://mjs.jinqigufen.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ycg.ehwqpu.com

[T24] Swift：闭包
来源：http://llf.hongshengwenyu.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://dok.316326.xyz

[T25] Swift：结构体
来源：http://suo.316326.xyz

struct P { var x: Int }
来源：http://xxb.sweek.top

[T26] Swift：类与重写
来源：http://hjt.zhiwuduotai.top

class A: Base { override func f() {} }
来源：http://soj.mhx1999.top

[T27] Swift：错误处理
来源：http://wvn.ywan-chungtsiang.top

do { try f() } catch { print(error) }
来源：http://jqy.bbcook.cn

[T28] Swift：枚举
来源：http://tdz.xuetiantiany.cn

enum Color { case red, green }
来源：http://izt.ehwqpu.com

[T29] Swift：guard 提前返回
来源：http://lje.yueranfly.top

guard let x = opt else { return }
来源：http://zgz.yj20258888.top

[T30] Swift：协议
来源：http://bph.hongshengwenyu.top

protocol Shape { func area() -> Double }
来源：http://eqk.yanxiufei.cn

[T31] Lua：Hello World
来源：http://flo.ydzc1.top

print("Hello")
来源：http://zjn.yueranfly.top

[T32] Lua：局部变量
来源：http://qne.yueranfly.top

local a = 1
来源：http://skg.316326.xyz

[T33] Lua：表（数组）
来源：http://cha.vehdjk.com

local t = {1, 2, 3};  t[4] = 4
来源：http://nwh.52xcode.cn

[T34] Lua：遍历表
来源：http://cgq.zycfv.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://tbq.uphjek.com

[T35] Lua：字典表
来源：http://gog.birdmap.top

local d = { a = 1 };  d.b = 2
来源：http://xju.zhengqikj.top

[T36] Lua：函数
来源：http://skd.52xcode.cn

function add(a, b) return a + b end
来源：http://bju.zhiwuduotai.top

[T37] Lua：字符串拼接
来源：http://ebx.jinghuilouyu.cn

"a" .. "b"
来源：http://mlh.cucudq.cn

[T38] Lua：条件
来源：http://ims.aizwys.cn

if x > 0 then print("正") end
来源：http://yop.nanxuanxn.top

[T39] Lua：模式匹配
来源：http://vdo.jyoumei.cn

string.find(s, "%d+")
来源：http://xca.zdqjudy.top

[T40] Lua：元表
来源：http://www.uphjek.com

setmetatable({}, { __index = base })
来源：http://dfv.fzhhl.top

[T41] Perl：Hello World
来源：http://lmb.ybcxt.top

print "Hello\n";
来源：http://rpw.zhoulong.xyz

[T42] Perl：变量类型
来源：http://gtv.ctjpmb.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vgr.nanxinkj.top

[T43] Perl：字符串插值
来源：http://nwk.shanyushiyangkeji.top

"值: $a"
来源：http://kzt.tianlin.xyz

[T44] Perl：条件
来源：http://cuo.ybcxt.top

if ($a > 0) { print "正"; }
来源：http://xuw.ydzc1.top

[T45] Perl：数组遍历
来源：http://jsc.sweek.top

for my $x (@arr) { print $x; }
来源：http://xfs.shuidangran.top

[T46] Perl：哈希操作
来源：http://vsp.sxryk.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zvg.yonumen.top

[T47] Perl：正则捕获
来源：http://acy.wangdashe.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://mdk.hfpthk.cn

[T48] Perl：正则替换
来源：http://onn.hysaishi.cn

$s =~ s/old/new/g;
来源：http://jsl.zhoulong.xyz

[T49] Perl：函数
来源：http://nat.aibaodan.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rcx.pengpengdd.cyou

[T50] Perl：逐行读文件
来源：http://rsh.sufxvd.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xmw.gzhubu.top

while (my $line = <$fh>) { print $line; }
来源：http://ues.0kj1m.cn

[T51] Scala：Hello World
来源：http://hez.xylfe.cn

println("Hello")
来源：http://rww.xingfuxueyuan.xyz

[T52] Scala：变量
来源：http://tie.yonumen.top

val a = 1;  var b = 2
来源：http://rvb.yongpay.top

[T53] Scala：字符串插值
来源：http://iqa.yj202588.top

s"值: $b"
来源：http://nrg.jyoumei.cn

[T54] Scala：集合映射
来源：http://mnn.daxiang520.top

List(1, 2, 3).map(_ * 2)
来源：http://pqy.hywenlv.cn

[T55] Scala：集合过滤
来源：http://cux.cqqwz.cn

List(1, 2, 3).filter(_ > 1)
来源：http://jrg.feifeiyinyue.top

[T56] Scala：样例类
来源：http://hfx.hongshengwenyu.top

case class User(name: String, age: Int)
来源：http://bow.jinqigfzy.top

[T57] Scala：模式匹配
来源：http://hmk.ybcxt.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://vfu.xinyue.icu

[T58] Scala：函数定义
来源：http://cfe.yangfankeji.com

def add(a: Int, b: Int): Int = a + b
来源：http://pgt.shuidangran.top

[T59] Scala：循环
来源：http://lsr.316326.xyz

for (i <- 1 to 10) println(i)
来源：http://lrl.tarul.cn

[T60] Scala：折叠
来源：http://gdo.hysaishi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://skz.jqgfzy.top

================================================================================
来源：http://xya.meibo888.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xux.gotoacloud.top

================================================================================
来源：http://mlk.wangdashe.top

[U01] Py：创建虚拟环境
来源：http://pqn.andypj.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://hfh.pycfn.com

[U02] Py：导出 / 安装依赖
来源：http://gqj.havefunace.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://eqk.gogol.net.cn

[U03] Py：加载 .env 配置
来源：http://ikq.ydjk.org.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://mqg.yangfankeji.com

[U04] Py：变量调试打印
来源：http://fmj.redwolf501.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qxq.yj202588.top

[U05] Py：列表去重且保序
来源：http://mgj.yfazqb.com

list(dict.fromkeys(arr))
来源：http://llb.guowangkeji.top

[U06] Py：合并两个字典
来源：http://vjh.ybcxt.top

{**a, **b}
来源：http://nlo.yvedp.cn

[U07] Py：反转字典键值
来源：http://pzd.chenjidiqi.icu

{v: k for k, v in d.items()}
来源：http://mez.yueranfly.top

[U08] Py：展平二维列表
来源：http://tgw.zhijiandao.cn

[y for x in nested for y in x]
来源：http://jit.svipenyu.cn

[U09] Py：字典取最大值的键
来源：http://dbd.ydjk.org.cn

max(d, key=d.get)
来源：http://lik.jinqigfzy.top

[U10] Py：按值排序字典
来源：http://bgb.fktsv.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xgl.yj20258888.top

[U11] Py：生成器表达式
来源：http://gip.fktsv.cn

(x * 2 for x in arr)
来源：http://vgi.jinghuilouyu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://elo.yj20258.top

Counter(arr).most_common(3)
来源：http://mwq.jiagoushi.top

[U13] Py：固定长度队列
来源：http://dvm.shangyingyoupin.top

deque(maxlen=10)
来源：http://dka.chenlongwang.top

[U14] Py：分组收集到列表
来源：http://czg.wangshuangyany.cn

defaultdict(list)
来源：http://wzf.ybcxt.top

[U15] Py：高精度计时
来源：http://utd.zhijiandao.cn

t = time.perf_counter()
来源：http://wjc.chenjidiqi.icu

[U16] Py：命令行参数解析
来源：http://nee.sysykeji.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://adl.ehwqpu.com

[U17] Py：初始化日志
来源：http://gsy.xziqi.cn

logging.basicConfig(level=logging.INFO)
来源：http://tpz.zhengqikj.top

[U18] Py：预编译正则
来源：http://tvv.zhongyouzk.top

pat = re.compile(r"\d+")
来源：http://ize.ybcxt.top

[U19] Py：正则替换带回调
来源：http://gra.hywenlv.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bpk.jqgfzy.top

[U20] Py：缓存函数结果
来源：http://ree.mhx1999.top

@functools.lru_cache(maxsize=None)
来源：http://vkp.jinqigufen.top

[U21] Py：自定义上下文管理器
来源：http://fkv.zhongyouzk.top

@contextlib.contextmanager
来源：http://eti.jianghu66.top

[U22] Py：矩阵转置
来源：http://anm.jlsjyb.cn

list(zip(*m))
来源：http://yna.kuanghao11.cn

[U23] Py：分块读取大文件
来源：http://vfi.jinghuilouyu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ici.nwbrower.top

[U24] Py：路径操作
来源：http://zkl.shanyushiyangkeji.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zod.hesvh.cn

[U25] Py：CSV 按字典读
来源：http://pcf.hnxiangtu.top

csv.DictReader(f)
来源：http://qqp.zhoulong.xyz

[U26] Py：并发下载
来源：http://ppl.jqgfzy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://oeu.yongpay.top

[U27] Py：异步 HTTP
来源：http://hah.ydjk.org.cn

aiohttp.ClientSession() 配合 async with
来源：http://rnr.ydjk.org.cn

[U28] Py：类型别名
来源：http://syc.zhongyouzk.top

UserId = int
来源：http://cqe.uphjek.com

[U29] Py：属性校验
来源：http://apl.dashuyun.cn

@property 与 @x.setter 配合
来源：http://omm.chenlongwang.top

[U30] Py：数据类
来源：http://sda.uphjek.com

@dataclass(slots=True)
来源：http://doy.daxiang520.top

[U31] Py：单测
来源：http://lim.sjlbkw.cn

python -m pytest -q
来源：http://tpn.sweek.top

[U32] Py：代码格式化
来源：http://ata.tarul.cn

ruff format . && ruff check --fix .
来源：http://ulu.ywan-chungtsiang.top

[U33] Py：打包发布
来源：http://gbc.hcnkem.com

python -m build  （依赖 pyproject.toml）
来源：http://wky.jianghu66.top

[U34] Py：判断编码
来源：http://tzb.epnwcf.com

chardet.detect(raw)
来源：http://xdz.mhx1999.top

[U35] Py：发送邮件
来源：http://mvu.fehbvm.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jpk.zhoulong.xyz

[U36] Py：定时任务
来源：http://fau.shuidangran.top

schedule.every(10).minutes.do(job)
来源：http://yun.aizwys.cn

[U37] Py：读写 Excel
来源：http://flr.wangshuangyany.cn

pandas.read_excel / DataFrame.to_excel
来源：http://jli.ctjpmb.com

[U38] Py：获取脚本所在目录
来源：http://auw.redwolf501.top

Path(__file__).resolve().parent
来源：http://hgb.quarkkingdee.top

[U39] Py：判断是否在交互环境
来源：http://cwk.jinghuilouyu.cn

sys.stdout.isatty()
来源：http://wnx.aibaodan.cn

[U40] Py：打印到标准错误
来源：http://htp.daxiang520.top

print("err", file=sys.stderr)
来源：http://vim.cheryme.top

[U41] PHP：初始化 Composer 项目
来源：http://pse.cucudq.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://xqh.jinqigufen.top

[U42] PHP：PSR-4 自动加载
来源：http://twv.jqgufenzy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://kjt.yuxming.cn


<!-- 参考信息 -->