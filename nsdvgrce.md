代发 wailian999

memset(a, 0, sizeof a);
来源：http://euk.mhx1999.top

[S27] C：定义常量
来源：http://nfv.daria6918.cn

const double PI = 3.14159;
来源：http://rla.hfpthk.cn

[S28] C：静态变量
来源：http://kti.52xcode.cn

static int counter = 0;
来源：http://som.sweek.top

[S29] C：变参函数
来源：http://ofy.52xcode.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yee.hywenlv.cn

[S30] C：头文件保护
来源：http://cvg.tian-w.cn

#ifndef X_H
来源：http://dre.redwolf501.top

#define X_H
来源：http://abe.hesvh.cn

#endif
来源：http://icr.nanxinkj.top

[S31] C++：Hello World
来源：http://jzw.zhijiandao.cn

#include <iostream>
来源：http://amd.ehwqpu.com

int main() { std::cout << "Hello\n"; }
来源：http://bop.zhongyouzk.top

[S32] C++：字符串
来源：http://ohy.pengpengdd.cyou

std::string s = "hi";  s += "!";
来源：http://xuu.vqdsnc.cn

[S33] C++：vector 增删
来源：http://rou.hnxiangtu.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tuf.xylfe.cn

[S34] C++：遍历 vector
来源：http://hiq.feifeiyinyue.top

for (auto &x : v) { std::cout << x; }
来源：http://krc.feifeiyinyue.top

[S35] C++：map
来源：http://zfo.52xcode.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fsz.yj202588.top

[S36] C++：unordered_map
来源：http://lzz.yfazqb.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tey.sufxvd.cn

[S37] C++：set
来源：http://oex.dashuyun.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dvw.mhx1999.top

[S38] C++：排序
来源：http://wid.sysykeji.top

std::sort(v.begin(), v.end());
来源：http://fyi.jqgufenzy.top

[S39] C++：自定义比较器排序
来源：http://bgh.yj20258.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zxo.redwolf501.top

[S40] C++：查找元素
来源：http://ebw.chenzaomai.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dfr.shangyingyoupin.top

[S41] C++：类与构造函数
来源：http://dmr.sysykeji.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://psz.fehbvm.com

[S42] C++：继承与虚函数
来源：http://bds.c1oappe.top

class B : public Base { public: void f() override {} };
来源：http://eng.shzxlz.cn

[S43] C++：智能指针
来源：http://wpj.fehbvm.com

auto p = std::make_unique<int>(5);
来源：http://iys.nwbrower.top

[S44] C++：引用传参
来源：http://vrd.fzhhl.top

void inc(int &x) { ++x; }
来源：http://vqa.zdqjudy.top

[S45] C++：lambda
来源：http://pfc.ehwqpu.com

auto add = [](int a, int b) { return a + b; };
来源：http://ubo.wangshuangyany.cn

[S46] C++：函数模板
来源：http://mkg.jlsjyb.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nnv.zdbjq.cn

[S47] C++：结构化绑定遍历
来源：http://akh.yueranfly.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kwu.jyoumei.cn

[S48] C++：逐行读文件
来源：http://hgz.xingfuxueyuan.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://msd.smart0.xyz

while (std::getline(in, line)) { }
来源：http://kys.cdnleiting.top

[S49] C++：写文件
来源：http://wki.guannengcc.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mlz.pengpengdd.cyou

[S50] C++：格式化数字
来源：http://mpp.zdbjq.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ccb.yonumen.top

[S51] C++：显式类型转换
来源：http://djo.daxiang520.top

static_cast<double>(a) / b
来源：http://kux.aibaodan.cn

[S52] C++：const 与 noexcept
来源：http://ucj.yuanzhike.top

int size() const noexcept { return n_; }
来源：http://jum.wangdashe.top

[S53] C++：移动语义
来源：http://ltd.jqgufenzy.top

std::vector<int> w = std::move(v);
来源：http://cxg.shuidangran.top

[S54] C++：异常处理
来源：http://zyr.vqdsnc.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hlp.zhaomingkeji.xyz

[S55] C++：结构化绑定
来源：http://ezc.nanxinkj.top

auto [a, b] = std::make_pair(1, 2);
来源：http://dqs.yonumen.top

[S56] C++：optional
来源：http://zpj.wangshuangyany.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://swl.daxiang520.top

[S57] C++：编译期常量
来源：http://tal.sufxvd.cn

constexpr int N = 10;
来源：http://equ.sysykeji.top

[S58] C++：命名空间
来源：http://pgb.cqqwz.cn

namespace ns { int f() { return 1; } }
来源：http://ttb.hywenlv.cn

[S59] C++：静态断言
来源：http://kds.shuidangran.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gbm.yonumen.top

[S60] C++：遍历并删除元素
来源：http://kwv.zdbjq.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mnx.jqgfzy.top

================================================================================
来源：http://knm.sweek.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uul.bjfxy.top

================================================================================
来源：http://oyg.hfpthk.cn

[T01] Kotlin：Hello World
来源：http://twf.xinyue.icu

println("Hello")
来源：http://sta.zhongyouzk.top

[T02] Kotlin：变量
来源：http://arc.guowangkeji.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qri.yj202588.top

[T03] Kotlin：字符串模板
来源：http://clq.nwbrower.top

"值: $b"
来源：http://lzd.vehdjk.com

[T04] Kotlin：空安全
来源：http://rxc.bbcook.cn

val n: String? = null;  n?.length
来源：http://coa.tianlin.xyz

[T05] Kotlin：when 表达式
来源：http://xet.jiagoushi.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nlt.shanyushiyangkeji.top

[T06] Kotlin：集合映射
来源：http://goq.xylfe.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://inu.sweek.top

[T07] Kotlin：集合过滤
来源：http://ltx.cheryme.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://zto.chenzaomai.com

[T08] Kotlin：数据类
来源：http://pkr.nwbrower.top

data class User(val name: String, val age: Int)
来源：http://ksz.sysykeji.top

[T09] Kotlin：扩展函数
来源：http://dmr.hnxiangtu.top

fun String.exclaim() = this + "!"
来源：http://vat.shanyushiyangtech.top

[T10] Kotlin：默认参数
来源：http://ntk.9152youxi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://yhx.yonumen.top

[T11] Kotlin：协程
来源：http://pvy.ivvv.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://moz.cashguo.top

[T12] Kotlin：解构声明
来源：http://oqb.shanyushiyangtech.top

val (a, b) = Pair(1, 2)
来源：http://tbr.jianghu66.top

[T13] Kotlin：只读 Map
来源：http://zdy.hongshengwenyu.top

val m = mapOf("a" to 1)
来源：http://zbc.zdbjq.cn

[T14] Kotlin：循环
来源：http://kxc.zdqjudy.top

for (i in 1..10) println(i)
来源：http://ydz.tanke756.top

[T15] Kotlin：接口
来源：http://vyk.pengpengdd.cyou

interface Shape { fun area(): Double }
来源：http://xmy.hnxiangtu.top

[T16] Swift：Hello World
来源：http://ubf.c1oappe.top

print("Hello")
来源：http://qby.shzxlz.cn

[T17] Swift：变量与常量
来源：http://yol.fanxiaobao.xyz

var a = 1;  let b = 2
来源：http://qyh.ivvv.top

[T18] Swift：字符串插值
来源：http://ivd.vqdsnc.cn

"值: \(b)"
来源：http://cea.wangshuangyany.cn

[T19] Swift：可选绑定
来源：http://zqr.hesvh.cn

if let n = opt { print(n) }
来源：http://zlc.cucudq.cn

[T20] Swift：数组操作
来源：http://wkx.hesvh.cn

var a = [1, 2, 3];  a.append(4)
来源：http://zrb.yvedp.cn

[T21] Swift：遍历
来源：http://nfc.yj202588.top

for x in a { print(x) }
来源：http://mpl.smart0.xyz

[T22] Swift：字典
来源：http://pwo.cqqwz.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ewf.aibaodan.cn

[T23] Swift：函数
来源：http://paw.fanxiaobao.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://uqj.wangdashe.top

[T24] Swift：闭包
来源：http://oqm.9152youxi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://wds.yanxiufei.cn

[T25] Swift：结构体
来源：http://fck.yangfankeji.com

struct P { var x: Int }
来源：http://qdj.redwolf501.top

[T26] Swift：类与重写
来源：http://oyd.xinyue.icu

class A: Base { override func f() {} }
来源：http://bjv.chenzaomai.com

[T27] Swift：错误处理
来源：http://oqx.zhoulong.xyz

do { try f() } catch { print(error) }
来源：http://gsi.jinghuilouyu.cn

[T28] Swift：枚举
来源：http://wnb.cheryme.top

enum Color { case red, green }
来源：http://trf.zhoulong.xyz

[T29] Swift：guard 提前返回
来源：http://wuz.yvedp.cn

guard let x = opt else { return }
来源：http://hqg.yangfankeji.com

[T30] Swift：协议
来源：http://lip.xuanzx.com

protocol Shape { func area() -> Double }
来源：http://ohx.vqdsnc.cn

[T31] Lua：Hello World
来源：http://ksl.daria6918.cn

print("Hello")
来源：http://oae.feifeiyinyue.top

[T32] Lua：局部变量
来源：http://ksw.jinghuilouyu.cn

local a = 1
来源：http://lle.feifeiyinyue.top

[T33] Lua：表（数组）
来源：http://yjp.ywan-chungtsiang.top

local t = {1, 2, 3};  t[4] = 4
来源：http://lmv.52xcode.cn

[T34] Lua：遍历表
来源：http://zen.c1oappe.top

for i, v in ipairs(t) do print(i, v) end
来源：http://znp.jqgfzy.top

[T35] Lua：字典表
来源：http://ecy.pycfn.com

local d = { a = 1 };  d.b = 2
来源：http://ckb.yongpay.top

[T36] Lua：函数
来源：http://jtb.jqgfzy.top

function add(a, b) return a + b end
来源：http://neh.birdmap.top

[T37] Lua：字符串拼接
来源：http://bwa.gotoacloud.top

"a" .. "b"
来源：http://lkw.dianchejie.cn

[T38] Lua：条件
来源：http://ova.xingfuxueyuan.xyz

if x > 0 then print("正") end
来源：http://dlf.bbcook.cn

[T39] Lua：模式匹配
来源：http://fiy.nwbrower.top

string.find(s, "%d+")
来源：http://mrz.smart0.xyz

[T40] Lua：元表
来源：http://hqm.sufxvd.cn

setmetatable({}, { __index = base })
来源：http://uuq.fanxiaobao.xyz

[T41] Perl：Hello World
来源：http://lzs.havefunace.top

print "Hello\n";
来源：http://kbv.sweek.top

[T42] Perl：变量类型
来源：http://bog.fanxiaobao.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://uff.cashguo.top

[T43] Perl：字符串插值
来源：http://pnv.jinghuilouyu.cn

"值: $a"
来源：http://ziu.316326.xyz

[T44] Perl：条件
来源：http://kvd.c1oappe.top

if ($a > 0) { print "正"; }
来源：http://mnk.sweek.top

[T45] Perl：数组遍历
来源：http://wdh.nanxuanxn.top

for my $x (@arr) { print $x; }
来源：http://fry.sysykeji.top

[T46] Perl：哈希操作
来源：http://wgd.gaohongyu789.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pjf.zhixingplan.top

[T47] Perl：正则捕获
来源：http://pdq.sysykeji.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://hpj.yfazqb.com

[T48] Perl：正则替换
来源：http://csy.fktsv.cn

$s =~ s/old/new/g;
来源：http://dte.52xcode.cn

[T49] Perl：函数
来源：http://yvr.shanyushiyangtech.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rki.dashuyun.cn

[T50] Perl：逐行读文件
来源：http://ovq.aibaodan.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qvt.hnqzz.top

while (my $line = <$fh>) { print $line; }
来源：http://yld.ctjpmb.com

[T51] Scala：Hello World
来源：http://guo.ywan-chungtsiang.top

println("Hello")
来源：http://low.sxryk.cn

[T52] Scala：变量
来源：http://bct.tianlin.xyz

val a = 1;  var b = 2
来源：http://lms.zhengqikj.top

[T53] Scala：字符串插值
来源：http://kbw.hysaishi.cn

s"值: $b"
来源：http://yln.yuanzhike.top

[T54] Scala：集合映射
来源：http://sla.shanyushiyangtech.top

List(1, 2, 3).map(_ * 2)
来源：http://hbh.yj20258.top

[T55] Scala：集合过滤
来源：http://ojl.nanxuanxn.top

List(1, 2, 3).filter(_ > 1)
来源：http://dyi.vqdsnc.cn

[T56] Scala：样例类
来源：http://mbm.nanxinkj.top

case class User(name: String, age: Int)
来源：http://smh.jqgfzy.top

[T57] Scala：模式匹配
来源：http://mga.jlsjyb.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://svl.yueranfly.top

[T58] Scala：函数定义
来源：http://hmm.ybcxt.top

def add(a: Int, b: Int): Int = a + b
来源：http://con.hesvh.cn

[T59] Scala：循环
来源：http://coq.zhoulong.xyz

for (i <- 1 to 10) println(i)
来源：http://byt.cheryme.top

[T60] Scala：折叠
来源：http://txl.shzxlz.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vfd.nanxinkj.top

================================================================================
来源：http://bcq.zhengqikj.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gdb.nanxinkj.top

================================================================================
来源：http://fja.havefunace.top

[U01] Py：创建虚拟环境
来源：http://rsf.shuidangran.top

python -m venv .venv && source .venv/bin/activate
来源：http://zep.jqgfzy.top

[U02] Py：导出 / 安装依赖
来源：http://mbn.ivvv.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wfe.dianchejie.cn

[U03] Py：加载 .env 配置
来源：http://ver.havefunace.top

from dotenv import load_dotenv; load_dotenv()
来源：http://lfb.xingfuxueyuan.xyz

[U04] Py：变量调试打印
来源：http://ahv.shuidangran.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mqg.sjlbkw.cn

[U05] Py：列表去重且保序
来源：http://nzv.mhx1999.top

list(dict.fromkeys(arr))
来源：http://lqo.gzhubu.top

[U06] Py：合并两个字典
来源：http://kvi.hfpthk.cn

{**a, **b}
来源：http://bxz.ydzc1.top

[U07] Py：反转字典键值
来源：http://lbq.hnxiangtu.top

{v: k for k, v in d.items()}
来源：http://ize.wangshuangyany.cn

[U08] Py：展平二维列表
来源：http://adh.chenzaomai.com

[y for x in nested for y in x]
来源：http://yrh.chenlongwang.top

[U09] Py：字典取最大值的键
来源：http://opq.hywenlv.cn

max(d, key=d.get)
来源：http://bgf.wangdashe.top

[U10] Py：按值排序字典
来源：http://juh.cheryme.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lno.xuetiantiany.cn

[U11] Py：生成器表达式
来源：http://tqu.yj20258888.top

(x * 2 for x in arr)
来源：http://kor.guannengcc.top

[U12] Py：取出现最多的 3 个元素
来源：http://nre.sufxvd.cn

Counter(arr).most_common(3)
来源：http://ugy.feifeiyinyue.top

[U13] Py：固定长度队列
来源：http://fqp.ywan-chungtsiang.top

deque(maxlen=10)
来源：http://ezd.zhijiandao.cn

[U14] Py：分组收集到列表
来源：http://svb.jiagoushi.top

defaultdict(list)
来源：http://jjj.zhiwuduotai.top

[U15] Py：高精度计时
来源：http://aps.hammf.cn

t = time.perf_counter()
来源：http://yjk.jianghu66.top

[U16] Py：命令行参数解析
来源：http://ett.cheryme.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yyd.shanyushiyangkeji.top

[U17] Py：初始化日志
来源：http://guo.cashguo.top

logging.basicConfig(level=logging.INFO)
来源：http://nvw.bjfxy.top

[U18] Py：预编译正则
来源：http://gov.zhengqikj.top

pat = re.compile(r"\d+")
来源：http://nhg.andypj.xyz

[U19] Py：正则替换带回调
来源：http://ala.zhaomingkeji.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ieh.yongpay.top

[U20] Py：缓存函数结果
来源：http://bsy.0kj1m.cn

@functools.lru_cache(maxsize=None)
来源：http://cwj.tarul.cn

[U21] Py：自定义上下文管理器
来源：http://wvf.xylfe.cn

@contextlib.contextmanager
来源：http://ujl.gotoacloud.top

[U22] Py：矩阵转置
来源：http://jhx.gzhubu.top

list(zip(*m))
来源：http://hmr.zhoulong.xyz

[U23] Py：分块读取大文件
来源：http://zew.daria6918.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://aeu.zhoulong.xyz

[U24] Py：路径操作
来源：http://ijp.yj20258888.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tww.ydzc1.top

[U25] Py：CSV 按字典读
来源：http://xzl.daria6918.cn

csv.DictReader(f)
来源：http://pcf.xziqi.cn

[U26] Py：并发下载
来源：http://opn.kuanghao11.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vew.zdqjudy.top

[U27] Py：异步 HTTP
来源：http://yyz.cucudq.cn

aiohttp.ClientSession() 配合 async with
来源：http://bop.sufxvd.cn

[U28] Py：类型别名
来源：http://gom.shanyushiyangtech.top

UserId = int
来源：http://boq.zhoulong.xyz

[U29] Py：属性校验
来源：http://nve.hcnkem.com

@property 与 @x.setter 配合
来源：http://cea.fktsv.cn

[U30] Py：数据类
来源：http://znp.ydzc1.top

@dataclass(slots=True)
来源：http://lik.xziqi.cn

[U31] Py：单测
来源：http://toz.hywenlv.cn

python -m pytest -q
来源：http://kuw.wangdashe.top

[U32] Py：代码格式化
来源：http://jrz.yueranfly.top

ruff format . && ruff check --fix .
来源：http://euv.xuanzx.com

[U33] Py：打包发布
来源：http://cmk.yanxiufei.cn

python -m build  （依赖 pyproject.toml）
来源：http://icf.jqgfzy.top

[U34] Py：判断编码
来源：http://bym.wangshuangyany.cn

chardet.detect(raw)
来源：http://wjj.hcnkem.com

[U35] Py：发送邮件
来源：http://tnz.shuidangran.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cut.yvedp.cn

[U36] Py：定时任务
来源：http://nid.sweek.top

schedule.every(10).minutes.do(job)
来源：http://ylp.smart0.xyz

[U37] Py：读写 Excel
来源：http://doh.yongpay.top

pandas.read_excel / DataFrame.to_excel
来源：http://zto.jiagoushi.top

[U38] Py：获取脚本所在目录
来源：http://ado.zhoulong.xyz

Path(__file__).resolve().parent
来源：http://xiy.xziqi.cn

[U39] Py：判断是否在交互环境
来源：http://gao.jqgfzy.top

sys.stdout.isatty()
来源：http://twr.jinqigufen.top

[U40] Py：打印到标准错误
来源：http://frl.havefunace.top

print("err", file=sys.stderr)
来源：http://jvv.xylfe.cn

[U41] PHP：初始化 Composer 项目
来源：http://sdb.quarkkingdee.top

composer init;  composer require guzzlehttp/guzzle
来源：http://hdm.yanxiufei.cn

[U42] PHP：PSR-4 自动加载
来源：http://cbh.ydzc1.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://eoz.haohaochexian.top

[U43] PHP：声明命名空间
来源：http://igy.zhijiandao.cn

namespace App\Http;
来源：http://vsb.snrcjt.cn

[U44] PHP：开启严格类型
来源：http://tbm.hcnkem.com

declare(strict_types=1);
来源：http://wiq.cucudq.cn

[U45] PHP：类型声明与返回类型
来源：http://isp.jyoumei.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://jyh.nanxuanxn.top

[U46] PHP：可空类型
来源：http://quh.meibo888.top

?string $name = null
来源：http://tsd.smart0.xyz

[U47] PHP：联合类型
来源：http://gmm.xinyue.icu

int|string $id
来源：http://xyn.zhengqikj.top

[U48] PHP：纯枚举
来源：http://ceb.shangyingyoupin.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dxj.hammf.cn

[U49] PHP：只读属性
来源：http://jto.ctjpmb.com

public readonly string $name
来源：http://ldu.sufxvd.cn

[U50] PHP：构造器属性提升
来源：http://yql.mhx1999.top

public function __construct(private int $id) {}
来源：http://wgz.yonumen.top


<!-- 参考信息 -->