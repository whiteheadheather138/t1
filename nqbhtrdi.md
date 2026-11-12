代发 wailian999

memset(a, 0, sizeof a);
来源：http://ovk.hnxiangtu.top

[S27] C：定义常量
来源：http://ikx.smart0.xyz

const double PI = 3.14159;
来源：http://htn.vqdsnc.cn

[S28] C：静态变量
来源：http://rpv.zhaomingkeji.xyz

static int counter = 0;
来源：http://ipy.nwbrower.top

[S29] C：变参函数
来源：http://gyg.chenjidiqi.icu

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dtu.tanke756.top

[S30] C：头文件保护
来源：http://wkt.daxiang520.top

#ifndef X_H
来源：http://sbw.xuetiantiany.cn

#define X_H
来源：http://abi.epnwcf.com

#endif
来源：http://pzz.c1oappe.top

[S31] C++：Hello World
来源：http://jwc.jinqigfzy.top

#include <iostream>
来源：http://jhh.ydjk.org.cn

int main() { std::cout << "Hello\n"; }
来源：http://zci.ppjwa.cn

[S32] C++：字符串
来源：http://ivu.hysaishi.cn

std::string s = "hi";  s += "!";
来源：http://fjn.hammf.cn

[S33] C++：vector 增删
来源：http://gho.chenjidiqi.icu

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xyq.hammf.cn

[S34] C++：遍历 vector
来源：http://qbw.pengpengdd.cyou

for (auto &x : v) { std::cout << x; }
来源：http://fic.iojbl.cn

[S35] C++：map
来源：http://hks.xingfuxueyuan.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ozv.tanke756.top

[S36] C++：unordered_map
来源：http://uoa.shangyingyoupin.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qwp.havefunace.top

[S37] C++：set
来源：http://ctq.ydzc1.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lvg.tianlin.xyz

[S38] C++：排序
来源：http://kkz.yongpay.top

std::sort(v.begin(), v.end());
来源：http://mnr.smart0.xyz

[S39] C++：自定义比较器排序
来源：http://mwq.jiagoushi.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nlq.aibaodan.cn

[S40] C++：查找元素
来源：http://hax.hnxiangtu.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tyb.zhengqikj.top

[S41] C++：类与构造函数
来源：http://xqz.gogol.net.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hgw.cheryme.top

[S42] C++：继承与虚函数
来源：http://wcl.chenzaomai.com

class B : public Base { public: void f() override {} };
来源：http://sdw.gotoacloud.top

[S43] C++：智能指针
来源：http://oha.zhiwuduotai.top

auto p = std::make_unique<int>(5);
来源：http://tcu.zhengqikj.top

[S44] C++：引用传参
来源：http://kik.hywenlv.cn

void inc(int &x) { ++x; }
来源：http://roq.sxryk.cn

[S45] C++：lambda
来源：http://vmz.hesvh.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ixp.yj20258888.top

[S46] C++：函数模板
来源：http://wpi.yanxiufei.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vic.xuetiantiany.cn

[S47] C++：结构化绑定遍历
来源：http://vtr.hcnkem.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dka.vqdsnc.cn

[S48] C++：逐行读文件
来源：http://yau.aibaodan.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vci.vehdjk.com

while (std::getline(in, line)) { }
来源：http://rqn.ywan-chungtsiang.top

[S49] C++：写文件
来源：http://czj.ctjpmb.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yyr.uphjek.com

[S50] C++：格式化数字
来源：http://qqk.wangdashe.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tts.daria6918.cn

[S51] C++：显式类型转换
来源：http://sug.jianghu66.top

static_cast<double>(a) / b
来源：http://jam.havefunace.top

[S52] C++：const 与 noexcept
来源：http://utc.wangshuangyany.cn

int size() const noexcept { return n_; }
来源：http://bbx.yonumen.top

[S53] C++：移动语义
来源：http://sdp.zhixingplan.top

std::vector<int> w = std::move(v);
来源：http://xel.andypj.xyz

[S54] C++：异常处理
来源：http://lwo.iojbl.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mxt.bbcook.cn

[S55] C++：结构化绑定
来源：http://psg.sweek.top

auto [a, b] = std::make_pair(1, 2);
来源：http://izl.svipenyu.cn

[S56] C++：optional
来源：http://iph.daxiang520.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cfs.0kj1m.cn

[S57] C++：编译期常量
来源：http://sie.tianlin.xyz

constexpr int N = 10;
来源：http://ihz.kuanghao11.cn

[S58] C++：命名空间
来源：http://sul.zhiwuduotai.top

namespace ns { int f() { return 1; } }
来源：http://owl.tanke756.top

[S59] C++：静态断言
来源：http://cel.ywan-chungtsiang.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wxv.jinqigfzy.top

[S60] C++：遍历并删除元素
来源：http://ylp.chenlongwang.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mqj.pengpengdd.cyou

================================================================================
来源：http://jig.ehwqpu.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uir.zhongyouzk.top

================================================================================
来源：http://dfv.iojbl.cn

[T01] Kotlin：Hello World
来源：http://yud.gotoacloud.top

println("Hello")
来源：http://ngl.yj202588.top

[T02] Kotlin：变量
来源：http://ajf.ydzc1.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fgv.xziqi.cn

[T03] Kotlin：字符串模板
来源：http://rjd.xingfuxueyuan.xyz

"值: $b"
来源：http://vjp.fehbvm.com

[T04] Kotlin：空安全
来源：http://rqv.cheryme.top

val n: String? = null;  n?.length
来源：http://ygd.zhixingplan.top

[T05] Kotlin：when 表达式
来源：http://usx.nwbrower.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tat.yj202588.top

[T06] Kotlin：集合映射
来源：http://rnr.shzxlz.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://aqb.jyoumei.cn

[T07] Kotlin：集合过滤
来源：http://sqi.wangshuangyany.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ash.kuanghao11.cn

[T08] Kotlin：数据类
来源：http://gjk.kuanghao11.cn

data class User(val name: String, val age: Int)
来源：http://far.ctjpmb.com

[T09] Kotlin：扩展函数
来源：http://aoy.jinqigfzy.top

fun String.exclaim() = this + "!"
来源：http://zlg.quarkkingdee.top

[T10] Kotlin：默认参数
来源：http://rri.sxryk.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://zcd.shuidangran.top

[T11] Kotlin：协程
来源：http://vie.wangshuangyany.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://dks.nwbrower.top

[T12] Kotlin：解构声明
来源：http://gdm.aibaodan.cn

val (a, b) = Pair(1, 2)
来源：http://ntd.hywenlv.cn

[T13] Kotlin：只读 Map
来源：http://mqv.zhiwuduotai.top

val m = mapOf("a" to 1)
来源：http://xpt.xziqi.cn

[T14] Kotlin：循环
来源：http://rtn.haohaochexian.top

for (i in 1..10) println(i)
来源：http://hvb.cashguo.top

[T15] Kotlin：接口
来源：http://fob.vehdjk.com

interface Shape { fun area(): Double }
来源：http://cae.hysaishi.cn

[T16] Swift：Hello World
来源：http://fvx.zhixingplan.top

print("Hello")
来源：http://zaa.cucudq.cn

[T17] Swift：变量与常量
来源：http://yig.fengsongda.top

var a = 1;  let b = 2
来源：http://moi.gotoacloud.top

[T18] Swift：字符串插值
来源：http://jwz.gotoacloud.top

"值: \(b)"
来源：http://iyp.guannengcc.top

[T19] Swift：可选绑定
来源：http://ybb.xuetiantiany.cn

if let n = opt { print(n) }
来源：http://cir.52xcode.cn

[T20] Swift：数组操作
来源：http://inv.dashuyun.cn

var a = [1, 2, 3];  a.append(4)
来源：http://axi.ydjk.org.cn

[T21] Swift：遍历
来源：http://cho.hongshengwenyu.top

for x in a { print(x) }
来源：http://els.bbcook.cn

[T22] Swift：字典
来源：http://pkb.9152youxi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://jzt.hfpthk.cn

[T23] Swift：函数
来源：http://kre.cheryme.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://suc.svipenyu.cn

[T24] Swift：闭包
来源：http://xva.shzxlz.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xms.havefunace.top

[T25] Swift：结构体
来源：http://hlo.yj20258.top

struct P { var x: Int }
来源：http://ktx.gzhubu.top

[T26] Swift：类与重写
来源：http://riq.ywan-chungtsiang.top

class A: Base { override func f() {} }
来源：http://vtf.jiagoushi.top

[T27] Swift：错误处理
来源：http://pmq.yonumen.top

do { try f() } catch { print(error) }
来源：http://mdn.hongshengwenyu.top

[T28] Swift：枚举
来源：http://anl.aizwys.cn

enum Color { case red, green }
来源：http://umj.jiagoushi.top

[T29] Swift：guard 提前返回
来源：http://pvb.xuetiantiany.cn

guard let x = opt else { return }
来源：http://ubn.cheryme.top

[T30] Swift：协议
来源：http://znl.nanxuanxn.top

protocol Shape { func area() -> Double }
来源：http://ylp.vqdsnc.cn

[T31] Lua：Hello World
来源：http://jjx.svipenyu.cn

print("Hello")
来源：http://qnb.hammf.cn

[T32] Lua：局部变量
来源：http://qzg.zhengqikj.top

local a = 1
来源：http://qhx.ywan-chungtsiang.top

[T33] Lua：表（数组）
来源：http://vxs.zhiwuduotai.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ybn.gzhubu.top

[T34] Lua：遍历表
来源：http://dtp.iojbl.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://zab.guannengcc.top

[T35] Lua：字典表
来源：http://djs.nwbrower.top

local d = { a = 1 };  d.b = 2
来源：http://akh.c1oappe.top

[T36] Lua：函数
来源：http://rdk.pycfn.com

function add(a, b) return a + b end
来源：http://crz.yanxiufei.cn

[T37] Lua：字符串拼接
来源：http://kkd.jinyuanbaomall.cn

"a" .. "b"
来源：http://ige.daria6918.cn

[T38] Lua：条件
来源：http://nxx.yongpay.top

if x > 0 then print("正") end
来源：http://ahv.chenjidiqi.icu

[T39] Lua：模式匹配
来源：http://zmk.hongshengwenyu.top

string.find(s, "%d+")
来源：http://tsj.sweek.top

[T40] Lua：元表
来源：http://ica.52xcode.cn

setmetatable({}, { __index = base })
来源：http://unz.xuanzx.com

[T41] Perl：Hello World
来源：http://vrw.gotoacloud.top

print "Hello\n";
来源：http://nqc.wangshuangyany.cn

[T42] Perl：变量类型
来源：http://llm.aibaodan.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hvo.jinyuanbaomall.cn

[T43] Perl：字符串插值
来源：http://vtc.feifeiyinyue.top

"值: $a"
来源：http://itu.redwolf501.top

[T44] Perl：条件
来源：http://vvg.xuanzx.com

if ($a > 0) { print "正"; }
来源：http://zvh.vqdsnc.cn

[T45] Perl：数组遍历
来源：http://ofi.yueranfly.top

for my $x (@arr) { print $x; }
来源：http://iuj.daxiang520.top

[T46] Perl：哈希操作
来源：http://yno.smart0.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ljv.xinyue.icu

[T47] Perl：正则捕获
来源：http://hii.gzhubu.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://fla.xylfe.cn

[T48] Perl：正则替换
来源：http://kqv.xuetiantiany.cn

$s =~ s/old/new/g;
来源：http://nom.fengsongda.top

[T49] Perl：函数
来源：http://brx.hesvh.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ehj.uphjek.com

[T50] Perl：逐行读文件
来源：http://tns.sufxvd.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ljq.fktsv.cn

while (my $line = <$fh>) { print $line; }
来源：http://lea.ydzc1.top

[T51] Scala：Hello World
来源：http://lti.havefunace.top

println("Hello")
来源：http://xco.bjfxy.top

[T52] Scala：变量
来源：http://euv.jinyuanbaomall.cn

val a = 1;  var b = 2
来源：http://anu.bjfxy.top

[T53] Scala：字符串插值
来源：http://skg.hcnkem.com

s"值: $b"
来源：http://rsx.jinghuilouyu.cn

[T54] Scala：集合映射
来源：http://wbj.haohaochexian.top

List(1, 2, 3).map(_ * 2)
来源：http://tsr.havefunace.top

[T55] Scala：集合过滤
来源：http://vnc.nanxuanxn.top

List(1, 2, 3).filter(_ > 1)
来源：http://byu.hcnkem.com

[T56] Scala：样例类
来源：http://blp.jqgufenzy.top

case class User(name: String, age: Int)
来源：http://qwu.shanyushiyangtech.top

[T57] Scala：模式匹配
来源：http://nge.mhx1999.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://zcf.ydjk.org.cn

[T58] Scala：函数定义
来源：http://zqx.tanke756.top

def add(a: Int, b: Int): Int = a + b
来源：http://dsu.hfpthk.cn

[T59] Scala：循环
来源：http://hxq.tarul.cn

for (i <- 1 to 10) println(i)
来源：http://uei.jqgufenzy.top

[T60] Scala：折叠
来源：http://zjw.vehdjk.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://eos.yueranfly.top

================================================================================
来源：http://zbm.epnwcf.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://unb.xylfe.cn

================================================================================
来源：http://fer.uphjek.com

[U01] Py：创建虚拟环境
来源：http://ace.yfazqb.com

python -m venv .venv && source .venv/bin/activate
来源：http://pxy.jinghuilouyu.cn

[U02] Py：导出 / 安装依赖
来源：http://egb.sjlbkw.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dtv.sufxvd.cn

[U03] Py：加载 .env 配置
来源：http://jft.bjfxy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://nxy.nanxinkj.top

[U04] Py：变量调试打印
来源：http://txs.xuanzx.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mmp.yanxiufei.cn

[U05] Py：列表去重且保序
来源：http://ccb.ivvv.top

list(dict.fromkeys(arr))
来源：http://fzl.gaohongyu789.top

[U06] Py：合并两个字典
来源：http://ubk.tianlin.xyz

{**a, **b}
来源：http://oef.nwbrower.top

[U07] Py：反转字典键值
来源：http://uxl.yangfankeji.com

{v: k for k, v in d.items()}
来源：http://xkr.jinyuanbaomall.cn

[U08] Py：展平二维列表
来源：http://vne.sjlbkw.cn

[y for x in nested for y in x]
来源：http://lrw.yongpay.top

[U09] Py：字典取最大值的键
来源：http://gmt.yj20258888.top

max(d, key=d.get)
来源：http://pqn.yueranfly.top

[U10] Py：按值排序字典
来源：http://ckj.chenzaomai.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ymf.jianghu66.top

[U11] Py：生成器表达式
来源：http://mws.fktsv.cn

(x * 2 for x in arr)
来源：http://ruc.pycfn.com

[U12] Py：取出现最多的 3 个元素
来源：http://jqs.zhijiandao.cn

Counter(arr).most_common(3)
来源：http://uwk.yueranfly.top

[U13] Py：固定长度队列
来源：http://kjs.smart0.xyz

deque(maxlen=10)
来源：http://yie.yj20258.top

[U14] Py：分组收集到列表
来源：http://fwa.fengsongda.top

defaultdict(list)
来源：http://her.zhongyouzk.top

[U15] Py：高精度计时
来源：http://nxr.jiagoushi.top

t = time.perf_counter()
来源：http://yuz.jlsjyb.cn

[U16] Py：命令行参数解析
来源：http://rkl.tarul.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sip.shangyingyoupin.top

[U17] Py：初始化日志
来源：http://dhy.feifeiyinyue.top

logging.basicConfig(level=logging.INFO)
来源：http://qas.sjlbkw.cn

[U18] Py：预编译正则
来源：http://jsl.epnwcf.com

pat = re.compile(r"\d+")
来源：http://bye.nanxinkj.top

[U19] Py：正则替换带回调
来源：http://kzn.gotoacloud.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mun.uphjek.com

[U20] Py：缓存函数结果
来源：http://clp.hywenlv.cn

@functools.lru_cache(maxsize=None)
来源：http://hrr.jinqigufen.top

[U21] Py：自定义上下文管理器
来源：http://snr.c1oappe.top

@contextlib.contextmanager
来源：http://pas.yj20258.top

[U22] Py：矩阵转置
来源：http://kwy.gaohongyu789.top

list(zip(*m))
来源：http://djj.tanke756.top

[U23] Py：分块读取大文件
来源：http://ojh.yj202588.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pde.cqqwz.cn

[U24] Py：路径操作
来源：http://ixs.guannengcc.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://cff.pycfn.com

[U25] Py：CSV 按字典读
来源：http://dra.vqdsnc.cn

csv.DictReader(f)
来源：http://poo.zycfv.cn

[U26] Py：并发下载
来源：http://rld.zhengqikj.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gqr.birdmap.top

[U27] Py：异步 HTTP
来源：http://fbo.fanxiaobao.xyz

aiohttp.ClientSession() 配合 async with
来源：http://zzy.cheryme.top

[U28] Py：类型别名
来源：http://evl.shangyingyoupin.top

UserId = int
来源：http://rhr.feifeiyinyue.top

[U29] Py：属性校验
来源：http://gdn.wangdashe.top

@property 与 @x.setter 配合
来源：http://mfk.yongpay.top

[U30] Py：数据类
来源：http://gpr.sxryk.cn

@dataclass(slots=True)
来源：http://cti.quarkkingdee.top

[U31] Py：单测
来源：http://mgi.yuanzhike.top

python -m pytest -q
来源：http://sjh.epnwcf.com

[U32] Py：代码格式化
来源：http://mys.yueranfly.top

ruff format . && ruff check --fix .
来源：http://cff.vqdsnc.cn

[U33] Py：打包发布
来源：http://ivn.epnwcf.com

python -m build  （依赖 pyproject.toml）
来源：http://pzg.316326.xyz

[U34] Py：判断编码
来源：http://pre.jlsjyb.cn

chardet.detect(raw)
来源：http://ezy.ctjpmb.com

[U35] Py：发送邮件
来源：http://iva.ppjwa.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://syu.nwbrower.top

[U36] Py：定时任务
来源：http://tqb.chenlongwang.top

schedule.every(10).minutes.do(job)
来源：http://dws.xziqi.cn

[U37] Py：读写 Excel
来源：http://lue.chenjidiqi.icu

pandas.read_excel / DataFrame.to_excel
来源：http://ont.yvedp.cn

[U38] Py：获取脚本所在目录
来源：http://mhn.jianghu66.top

Path(__file__).resolve().parent
来源：http://cbl.aizwys.cn

[U39] Py：判断是否在交互环境
来源：http://nvz.sxryk.cn

sys.stdout.isatty()
来源：http://fkz.redwolf501.top

[U40] Py：打印到标准错误
来源：http://jxb.ctjpmb.com

print("err", file=sys.stderr)
来源：http://eyj.chenjidiqi.icu

[U41] PHP：初始化 Composer 项目
来源：http://hrc.cdnleiting.top

composer init;  composer require guzzlehttp/guzzle
来源：http://wuh.snrcjt.cn

[U42] PHP：PSR-4 自动加载
来源：http://lxe.jqgufenzy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://pdu.shuidangran.top

[U43] PHP：声明命名空间
来源：http://mqj.jinyuanbaomall.cn

namespace App\Http;
来源：http://poa.svipenyu.cn

[U44] PHP：开启严格类型
来源：http://niq.yonumen.top

declare(strict_types=1);
来源：http://qmp.jinqigfzy.top

[U45] PHP：类型声明与返回类型
来源：http://pnv.hesvh.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://qpk.cheryme.top

[U46] PHP：可空类型
来源：http://ldt.kuanghao11.cn

?string $name = null
来源：http://rkd.sysykeji.top

[U47] PHP：联合类型
来源：http://ngj.yj202588.top

int|string $id
来源：http://tlv.yj20258.top

[U48] PHP：纯枚举
来源：http://dok.guowangkeji.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://njp.chenjidiqi.icu

[U49] PHP：只读属性
来源：http://rym.nwbrower.top

public readonly string $name
来源：http://jma.dianchejie.cn

[U50] PHP：构造器属性提升
来源：http://lqy.snrcjt.cn

public function __construct(private int $id) {}
来源：http://fol.c1oappe.top


<!-- 参考信息 -->