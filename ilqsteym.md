代发 wailian999

x |= (1 << 3);
来源：http://mxa.fktsv.cn

[S17] C：安全拼接字符串
来源：http://czi.fehbvm.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fis.ivvv.top

[S18] C：命令行参数
来源：http://pps.hysaishi.cn

int main(int argc, char **argv)
来源：http://jqa.hesvh.cn

[S19] C：快速排序
来源：http://ycw.chenjidiqi.icu

qsort(a, n, sizeof(int), cmp);
来源：http://zoc.yongpay.top

[S20] C：二分查找
来源：http://zxq.jiagoushi.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gim.yongpay.top

[S21] C：字符类别判断
来源：http://rhn.jyoumei.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qku.sxryk.cn

[S22] C：字符串转数字
来源：http://jcz.tianlin.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://ild.jinghuilouyu.cn

[S23] C：随机数
来源：http://zza.jinqigfzy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://mex.zhaomingkeji.xyz

[S24] C：获取本地时间
来源：http://xhc.jiagoushi.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lzn.bbcook.cn

[S25] C：内存拷贝
来源：http://yuu.yfazqb.com

memcpy(dst, src, n);
来源：http://lmw.yuanzhike.top

[S26] C：内存清零
来源：http://qlp.zdqjudy.top

memset(a, 0, sizeof a);
来源：http://kaw.sxryk.cn

[S27] C：定义常量
来源：http://ooq.zhiwuduotai.top

const double PI = 3.14159;
来源：http://suf.hysaishi.cn

[S28] C：静态变量
来源：http://odm.fengsongda.top

static int counter = 0;
来源：http://rnb.hcnkem.com

[S29] C：变参函数
来源：http://wuo.cqqwz.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ytn.hesvh.cn

[S30] C：头文件保护
来源：http://yno.zhaomingkeji.xyz

#ifndef X_H
来源：http://pjf.hesvh.cn

#define X_H
来源：http://tgx.yuanzhike.top

#endif
来源：http://wku.hcnkem.com

[S31] C++：Hello World
来源：http://okt.shanyushiyangkeji.top

#include <iostream>
来源：http://cpi.jqgfzy.top

int main() { std::cout << "Hello\n"; }
来源：http://ckm.tanke756.top

[S32] C++：字符串
来源：http://ulb.cheryme.top

std::string s = "hi";  s += "!";
来源：http://iho.yueranfly.top

[S33] C++：vector 增删
来源：http://apb.gogol.net.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rrs.zycfv.cn

[S34] C++：遍历 vector
来源：http://ufi.yueranfly.top

for (auto &x : v) { std::cout << x; }
来源：http://xjp.yueranfly.top

[S35] C++：map
来源：http://nbs.iojbl.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nqh.zdbjq.cn

[S36] C++：unordered_map
来源：http://ssr.birdmap.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ucj.daria6918.cn

[S37] C++：set
来源：http://nop.wangshuangyany.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://spz.nanxinkj.top

[S38] C++：排序
来源：http://huw.andypj.xyz

std::sort(v.begin(), v.end());
来源：http://eqj.guannengcc.top

[S39] C++：自定义比较器排序
来源：http://lei.tianlin.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gyd.ppjwa.cn

[S40] C++：查找元素
来源：http://bcf.ywan-chungtsiang.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tmg.shuidangran.top

[S41] C++：类与构造函数
来源：http://kur.hnqzz.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qxx.yfazqb.com

[S42] C++：继承与虚函数
来源：http://pfu.hnqzz.top

class B : public Base { public: void f() override {} };
来源：http://dcr.ehwqpu.com

[S43] C++：智能指针
来源：http://drr.xylfe.cn

auto p = std::make_unique<int>(5);
来源：http://znt.quarkkingdee.top

[S44] C++：引用传参
来源：http://ixb.gzhubu.top

void inc(int &x) { ++x; }
来源：http://xgl.jlsjyb.cn

[S45] C++：lambda
来源：http://ouc.dianchejie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wgn.zhoulong.xyz

[S46] C++：函数模板
来源：http://rqb.jlsjyb.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mls.shangyingyoupin.top

[S47] C++：结构化绑定遍历
来源：http://cwf.iojbl.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qpu.ydjk.org.cn

[S48] C++：逐行读文件
来源：http://zlx.shanyushiyangtech.top

std::ifstream in("a.txt");  std::string line;
来源：http://mje.pycfn.com

while (std::getline(in, line)) { }
来源：http://utp.hysaishi.cn

[S49] C++：写文件
来源：http://xsz.vehdjk.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fit.jqgufenzy.top

[S50] C++：格式化数字
来源：http://esd.guowangkeji.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nax.tarul.cn

[S51] C++：显式类型转换
来源：http://hgi.52xcode.cn

static_cast<double>(a) / b
来源：http://ucl.ivvv.top

[S52] C++：const 与 noexcept
来源：http://lic.xuetiantiany.cn

int size() const noexcept { return n_; }
来源：http://ixc.havefunace.top

[S53] C++：移动语义
来源：http://jbk.andypj.xyz

std::vector<int> w = std::move(v);
来源：http://kxg.daria6918.cn

[S54] C++：异常处理
来源：http://yqe.yongpay.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://euj.jqgfzy.top

[S55] C++：结构化绑定
来源：http://imj.dashuyun.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://len.cashguo.top

[S56] C++：optional
来源：http://bsb.yfazqb.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tky.zdbjq.cn

[S57] C++：编译期常量
来源：http://kdh.snrcjt.cn

constexpr int N = 10;
来源：http://zlu.sysykeji.top

[S58] C++：命名空间
来源：http://gal.nanxuanxn.top

namespace ns { int f() { return 1; } }
来源：http://sfn.daxiang520.top

[S59] C++：静态断言
来源：http://qow.ydjk.org.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://enh.cucudq.cn

[S60] C++：遍历并删除元素
来源：http://bjn.nwbrower.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://sxb.jinghuilouyu.cn

================================================================================
来源：http://xqr.sjlbkw.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://muc.shzxlz.cn

================================================================================
来源：http://zcs.redwolf501.top

[T01] Kotlin：Hello World
来源：http://ewt.0kj1m.cn

println("Hello")
来源：http://vft.zhaomingkeji.xyz

[T02] Kotlin：变量
来源：http://qyi.guowangkeji.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xxt.hysaishi.cn

[T03] Kotlin：字符串模板
来源：http://nwo.nanxinkj.top

"值: $b"
来源：http://ksl.hesvh.cn

[T04] Kotlin：空安全
来源：http://zxd.bjfxy.top

val n: String? = null;  n?.length
来源：http://ypk.zhijiandao.cn

[T05] Kotlin：when 表达式
来源：http://fhn.fanxiaobao.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://abd.ivvv.top

[T06] Kotlin：集合映射
来源：http://uju.mhx1999.top

listOf(1, 2, 3).map { it * 2 }
来源：http://iet.ehwqpu.com

[T07] Kotlin：集合过滤
来源：http://ohz.fanxiaobao.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://pml.hnxiangtu.top

[T08] Kotlin：数据类
来源：http://xex.zhijiandao.cn

data class User(val name: String, val age: Int)
来源：http://mfl.hcnkem.com

[T09] Kotlin：扩展函数
来源：http://gmq.fzhhl.top

fun String.exclaim() = this + "!"
来源：http://pkt.sysykeji.top

[T10] Kotlin：默认参数
来源：http://nns.xuetiantiany.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qvx.fanxiaobao.xyz

[T11] Kotlin：协程
来源：http://spm.zhiwuduotai.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://afp.316326.xyz

[T12] Kotlin：解构声明
来源：http://pto.snrcjt.cn

val (a, b) = Pair(1, 2)
来源：http://cml.sweek.top

[T13] Kotlin：只读 Map
来源：http://qbj.pengpengdd.cyou

val m = mapOf("a" to 1)
来源：http://oky.yj20258.top

[T14] Kotlin：循环
来源：http://rhy.jinyuanbaomall.cn

for (i in 1..10) println(i)
来源：http://tdm.wangshuangyany.cn

[T15] Kotlin：接口
来源：http://ove.gogol.net.cn

interface Shape { fun area(): Double }
来源：http://mci.nanxuanxn.top

[T16] Swift：Hello World
来源：http://uhp.bjfxy.top

print("Hello")
来源：http://tqc.shzxlz.cn

[T17] Swift：变量与常量
来源：http://sip.zhongyouzk.top

var a = 1;  let b = 2
来源：http://btg.yj20258888.top

[T18] Swift：字符串插值
来源：http://pxz.uphjek.com

"值: \(b)"
来源：http://ssm.fehbvm.com

[T19] Swift：可选绑定
来源：http://mhj.quarkkingdee.top

if let n = opt { print(n) }
来源：http://sli.wangdashe.top

[T20] Swift：数组操作
来源：http://znh.andypj.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://phd.jiagoushi.top

[T21] Swift：遍历
来源：http://vyh.zhiwuduotai.top

for x in a { print(x) }
来源：http://vnt.havefunace.top

[T22] Swift：字典
来源：http://zsb.hcnkem.com

var d = ["a": 1];  d["b"] = 2
来源：http://lqv.gzhubu.top

[T23] Swift：函数
来源：http://nmd.tianlin.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://epv.aizwys.cn

[T24] Swift：闭包
来源：http://ril.sweek.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://clh.andypj.xyz

[T25] Swift：结构体
来源：http://ayn.dianchejie.cn

struct P { var x: Int }
来源：http://tuy.yuanzhike.top

[T26] Swift：类与重写
来源：http://vwh.dashuyun.cn

class A: Base { override func f() {} }
来源：http://wmt.jinqigufen.top

[T27] Swift：错误处理
来源：http://fmo.zdqjudy.top

do { try f() } catch { print(error) }
来源：http://ffb.tianlin.xyz

[T28] Swift：枚举
来源：http://hni.cashguo.top

enum Color { case red, green }
来源：http://mhw.pengpengdd.cyou

[T29] Swift：guard 提前返回
来源：http://aqj.jyoumei.cn

guard let x = opt else { return }
来源：http://eyu.cashguo.top

[T30] Swift：协议
来源：http://hzx.gogol.net.cn

protocol Shape { func area() -> Double }
来源：http://frq.uphjek.com

[T31] Lua：Hello World
来源：http://dwe.jinyuanbaomall.cn

print("Hello")
来源：http://ipn.yueranfly.top

[T32] Lua：局部变量
来源：http://azs.smart0.xyz

local a = 1
来源：http://phr.aizwys.cn

[T33] Lua：表（数组）
来源：http://zvl.smart0.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://jma.jlsjyb.cn

[T34] Lua：遍历表
来源：http://qcp.cqqwz.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://xjo.jinqigufen.top

[T35] Lua：字典表
来源：http://hwr.jyoumei.cn

local d = { a = 1 };  d.b = 2
来源：http://suu.vqdsnc.cn

[T36] Lua：函数
来源：http://xph.hnxiangtu.top

function add(a, b) return a + b end
来源：http://wch.hysaishi.cn

[T37] Lua：字符串拼接
来源：http://zrr.shuidangran.top

"a" .. "b"
来源：http://pfj.quarkkingdee.top

[T38] Lua：条件
来源：http://xag.shuidangran.top

if x > 0 then print("正") end
来源：http://odd.fengsongda.top

[T39] Lua：模式匹配
来源：http://rdi.hongshengwenyu.top

string.find(s, "%d+")
来源：http://swj.jinghuilouyu.cn

[T40] Lua：元表
来源：http://ron.yj202588.top

setmetatable({}, { __index = base })
来源：http://jeg.pengpengdd.cyou

[T41] Perl：Hello World
来源：http://sqt.gotoacloud.top

print "Hello\n";
来源：http://vwe.cheryme.top

[T42] Perl：变量类型
来源：http://hmr.snrcjt.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yan.meibo888.top

[T43] Perl：字符串插值
来源：http://dlg.fzhhl.top

"值: $a"
来源：http://fmq.birdmap.top

[T44] Perl：条件
来源：http://icb.yj20258888.top

if ($a > 0) { print "正"; }
来源：http://iqi.ywan-chungtsiang.top

[T45] Perl：数组遍历
来源：http://tvk.iojbl.cn

for my $x (@arr) { print $x; }
来源：http://kec.bbcook.cn

[T46] Perl：哈希操作
来源：http://kqb.aizwys.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://iuf.shuidangran.top

[T47] Perl：正则捕获
来源：http://ijh.snrcjt.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://djb.yueranfly.top

[T48] Perl：正则替换
来源：http://wfq.aizwys.cn

$s =~ s/old/new/g;
来源：http://yjs.chenzaomai.com

[T49] Perl：函数
来源：http://brz.svipenyu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nwh.fehbvm.com

[T50] Perl：逐行读文件
来源：http://lna.zhixingplan.top

open my $fh, "<", "a.txt" or die $!;
来源：http://azs.redwolf501.top

while (my $line = <$fh>) { print $line; }
来源：http://wdb.52xcode.cn

[T51] Scala：Hello World
来源：http://dvs.daria6918.cn

println("Hello")
来源：http://cwa.shanyushiyangkeji.top

[T52] Scala：变量
来源：http://pju.ydzc1.top

val a = 1;  var b = 2
来源：http://dyy.316326.xyz

[T53] Scala：字符串插值
来源：http://qgs.birdmap.top

s"值: $b"
来源：http://zwa.dianchejie.cn

[T54] Scala：集合映射
来源：http://ktv.ctjpmb.com

List(1, 2, 3).map(_ * 2)
来源：http://kgr.yj20258888.top

[T55] Scala：集合过滤
来源：http://wsw.c1oappe.top

List(1, 2, 3).filter(_ > 1)
来源：http://tmp.sufxvd.cn

[T56] Scala：样例类
来源：http://qxo.shanyushiyangkeji.top

case class User(name: String, age: Int)
来源：http://ago.hywenlv.cn

[T57] Scala：模式匹配
来源：http://uhr.svipenyu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://inh.andypj.xyz

[T58] Scala：函数定义
来源：http://xyc.jinqigufen.top

def add(a: Int, b: Int): Int = a + b
来源：http://wts.kuanghao11.cn

[T59] Scala：循环
来源：http://bad.yongpay.top

for (i <- 1 to 10) println(i)
来源：http://ifa.tianlin.xyz

[T60] Scala：折叠
来源：http://mwo.aizwys.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vfy.ctjpmb.com

================================================================================
来源：http://ptq.jqgfzy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fft.zhixingplan.top

================================================================================
来源：http://kjq.shanyushiyangkeji.top

[U01] Py：创建虚拟环境
来源：http://kdl.9152youxi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://vtj.nanxuanxn.top

[U02] Py：导出 / 安装依赖
来源：http://kka.wangdashe.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nhp.jianghu66.top

[U03] Py：加载 .env 配置
来源：http://clj.fehbvm.com

from dotenv import load_dotenv; load_dotenv()
来源：http://tjr.guowangkeji.top

[U04] Py：变量调试打印
来源：http://kxo.xingfuxueyuan.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xxz.bjfxy.top

[U05] Py：列表去重且保序
来源：http://epc.daxiang520.top

list(dict.fromkeys(arr))
来源：http://btu.hcnkem.com

[U06] Py：合并两个字典
来源：http://lmf.jinyuanbaomall.cn

{**a, **b}
来源：http://ojy.shanyushiyangkeji.top

[U07] Py：反转字典键值
来源：http://wyr.wangdashe.top

{v: k for k, v in d.items()}
来源：http://nnb.svipenyu.cn

[U08] Py：展平二维列表
来源：http://rlz.aibaodan.cn

[y for x in nested for y in x]
来源：http://cbq.chenlongwang.top

[U09] Py：字典取最大值的键
来源：http://noo.zhoulong.xyz

max(d, key=d.get)
来源：http://hxy.hnqzz.top

[U10] Py：按值排序字典
来源：http://uup.bbcook.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sqt.snrcjt.cn

[U11] Py：生成器表达式
来源：http://otj.birdmap.top

(x * 2 for x in arr)
来源：http://zoo.yj20258888.top

[U12] Py：取出现最多的 3 个元素
来源：http://kig.ybcxt.top

Counter(arr).most_common(3)
来源：http://xha.hnxiangtu.top

[U13] Py：固定长度队列
来源：http://led.bbcook.cn

deque(maxlen=10)
来源：http://rav.zdbjq.cn

[U14] Py：分组收集到列表
来源：http://eur.daria6918.cn

defaultdict(list)
来源：http://mgr.tarul.cn

[U15] Py：高精度计时
来源：http://acr.fehbvm.com

t = time.perf_counter()
来源：http://mqo.zdbjq.cn

[U16] Py：命令行参数解析
来源：http://osd.cucudq.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://otu.xylfe.cn

[U17] Py：初始化日志
来源：http://ony.pengpengdd.cyou

logging.basicConfig(level=logging.INFO)
来源：http://myp.andypj.xyz

[U18] Py：预编译正则
来源：http://fdh.yuanzhike.top

pat = re.compile(r"\d+")
来源：http://icn.zycfv.cn

[U19] Py：正则替换带回调
来源：http://csx.svipenyu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hxx.cqqwz.cn

[U20] Py：缓存函数结果
来源：http://ufg.quarkkingdee.top

@functools.lru_cache(maxsize=None)
来源：http://lpg.pengpengdd.cyou

[U21] Py：自定义上下文管理器
来源：http://nbe.aizwys.cn

@contextlib.contextmanager
来源：http://efg.yvedp.cn

[U22] Py：矩阵转置
来源：http://fje.xziqi.cn

list(zip(*m))
来源：http://iff.tarul.cn

[U23] Py：分块读取大文件
来源：http://eyi.hnqzz.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://yhs.xingfuxueyuan.xyz

[U24] Py：路径操作
来源：http://gpk.daxiang520.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vga.zhengqikj.top

[U25] Py：CSV 按字典读
来源：http://bje.zhongyouzk.top

csv.DictReader(f)
来源：http://pvj.quarkkingdee.top

[U26] Py：并发下载
来源：http://tui.tian-w.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://aci.jlsjyb.cn

[U27] Py：异步 HTTP
来源：http://jbd.cucudq.cn

aiohttp.ClientSession() 配合 async with
来源：http://svm.ctjpmb.com

[U28] Py：类型别名
来源：http://pyc.nanxinkj.top

UserId = int
来源：http://iqd.epnwcf.com

[U29] Py：属性校验
来源：http://ybb.ydzc1.top

@property 与 @x.setter 配合
来源：http://zyg.cashguo.top

[U30] Py：数据类
来源：http://fja.fanxiaobao.xyz

@dataclass(slots=True)
来源：http://vbi.nanxuanxn.top

[U31] Py：单测
来源：http://rlp.xinyue.icu

python -m pytest -q
来源：http://wua.cdnleiting.top

[U32] Py：代码格式化
来源：http://xhv.jinghuilouyu.cn

ruff format . && ruff check --fix .
来源：http://pvr.fengsongda.top

[U33] Py：打包发布
来源：http://wiz.jinghuilouyu.cn

python -m build  （依赖 pyproject.toml）
来源：http://hkz.sjlbkw.cn

[U34] Py：判断编码
来源：http://bje.bjfxy.top

chardet.detect(raw)
来源：http://vby.shanyushiyangkeji.top

[U35] Py：发送邮件
来源：http://xjc.cashguo.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://lax.quarkkingdee.top

[U36] Py：定时任务
来源：http://epv.daria6918.cn

schedule.every(10).minutes.do(job)
来源：http://hig.yj20258.top

[U37] Py：读写 Excel
来源：http://aln.tianlin.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://wjl.dashuyun.cn

[U38] Py：获取脚本所在目录
来源：http://lcu.zhongyouzk.top

Path(__file__).resolve().parent
来源：http://zmu.fehbvm.com

[U39] Py：判断是否在交互环境
来源：http://qow.dashuyun.cn

sys.stdout.isatty()
来源：http://ldo.havefunace.top

[U40] Py：打印到标准错误
来源：http://xuj.9152youxi.cn

print("err", file=sys.stderr)
来源：http://kua.fktsv.cn


<!-- 参考信息 -->