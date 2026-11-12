代发 wailian999

#include <iostream>
来源：http://tgh.zdqjudy.top

int main() { std::cout << "Hello\n"; }
来源：http://rye.andypj.xyz

[S32] C++：字符串
来源：http://gcv.316326.xyz

std::string s = "hi";  s += "!";
来源：http://xzk.zhoulong.xyz

[S33] C++：vector 增删
来源：http://mtl.sweek.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://npc.hywenlv.cn

[S34] C++：遍历 vector
来源：http://lcs.ehwqpu.com

for (auto &x : v) { std::cout << x; }
来源：http://ldg.pengpengdd.cyou

[S35] C++：map
来源：http://zfw.vqdsnc.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://izu.guowangkeji.top

[S36] C++：unordered_map
来源：http://leo.yanxiufei.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://awp.gaohongyu789.top

[S37] C++：set
来源：http://lqm.chenzaomai.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tak.zhongyouzk.top

[S38] C++：排序
来源：http://cia.gogol.net.cn

std::sort(v.begin(), v.end());
来源：http://nmj.jqgufenzy.top

[S39] C++：自定义比较器排序
来源：http://rsg.zhiwuduotai.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zps.jyoumei.cn

[S40] C++：查找元素
来源：http://esm.zhoulong.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kkf.cashguo.top

[S41] C++：类与构造函数
来源：http://gwa.yuxming.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kzc.52xcode.cn

[S42] C++：继承与虚函数
来源：http://hnw.yueranfly.top

class B : public Base { public: void f() override {} };
来源：http://nuj.epnwcf.com

[S43] C++：智能指针
来源：http://xsl.gaohongyu789.top

auto p = std::make_unique<int>(5);
来源：http://the.daria6918.cn

[S44] C++：引用传参
来源：http://zap.epnwcf.com

void inc(int &x) { ++x; }
来源：http://xoj.wangdashe.top

[S45] C++：lambda
来源：http://avo.c1oappe.top

auto add = [](int a, int b) { return a + b; };
来源：http://jmz.iojbl.cn

[S46] C++：函数模板
来源：http://jmz.uphjek.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://awl.cheryme.top

[S47] C++：结构化绑定遍历
来源：http://byr.chenjidiqi.icu

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://unh.ydzc1.top

[S48] C++：逐行读文件
来源：http://tgv.jinghuilouyu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://uup.jinyuanbaomall.cn

while (std::getline(in, line)) { }
来源：http://den.jinqigfzy.top

[S49] C++：写文件
来源：http://mub.hcnkem.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zga.fengsongda.top

[S50] C++：格式化数字
来源：http://fbi.bjfxy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wzs.dianchejie.cn

[S51] C++：显式类型转换
来源：http://fok.zhengqikj.top

static_cast<double>(a) / b
来源：http://zpv.nwbrower.top

[S52] C++：const 与 noexcept
来源：http://acv.jinqigufen.top

int size() const noexcept { return n_; }
来源：http://mns.chenzaomai.com

[S53] C++：移动语义
来源：http://gch.yfazqb.com

std::vector<int> w = std::move(v);
来源：http://lbv.316326.xyz

[S54] C++：异常处理
来源：http://zyf.redwolf501.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://paw.mhx1999.top

[S55] C++：结构化绑定
来源：http://vlb.bjfxy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://dkw.yj202588.top

[S56] C++：optional
来源：http://mgb.havefunace.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vis.sufxvd.cn

[S57] C++：编译期常量
来源：http://qer.zhaomingkeji.xyz

constexpr int N = 10;
来源：http://uvv.daxiang520.top

[S58] C++：命名空间
来源：http://jqy.tarul.cn

namespace ns { int f() { return 1; } }
来源：http://owz.fengsongda.top

[S59] C++：静态断言
来源：http://wtz.jyoumei.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://uuo.gzhubu.top

[S60] C++：遍历并删除元素
来源：http://oco.fanxiaobao.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tug.dashuyun.cn

================================================================================
来源：http://sjy.yj20258888.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ocr.tianlin.xyz

================================================================================
来源：http://lqh.hammf.cn

[T01] Kotlin：Hello World
来源：http://bcn.daxiang520.top

println("Hello")
来源：http://esr.ybcxt.top

[T02] Kotlin：变量
来源：http://pxc.c1oappe.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zrj.zdbjq.cn

[T03] Kotlin：字符串模板
来源：http://dbr.jinqigfzy.top

"值: $b"
来源：http://fbo.cdnleiting.top

[T04] Kotlin：空安全
来源：http://vww.hfpthk.cn

val n: String? = null;  n?.length
来源：http://cpv.ybcxt.top

[T05] Kotlin：when 表达式
来源：http://hzr.fehbvm.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wix.nanxuanxn.top

[T06] Kotlin：集合映射
来源：http://vfv.meibo888.top

listOf(1, 2, 3).map { it * 2 }
来源：http://jhw.vqdsnc.cn

[T07] Kotlin：集合过滤
来源：http://hvz.gogol.net.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qum.cashguo.top

[T08] Kotlin：数据类
来源：http://apq.jlsjyb.cn

data class User(val name: String, val age: Int)
来源：http://sel.shzxlz.cn

[T09] Kotlin：扩展函数
来源：http://zdz.jqgfzy.top

fun String.exclaim() = this + "!"
来源：http://xiy.ydzc1.top

[T10] Kotlin：默认参数
来源：http://zff.cashguo.top

fun greet(name: String = "World") = "Hi $name"
来源：http://kgo.fzhhl.top

[T11] Kotlin：协程
来源：http://hxa.xuanzx.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://ynh.shanyushiyangkeji.top

[T12] Kotlin：解构声明
来源：http://dyk.vqdsnc.cn

val (a, b) = Pair(1, 2)
来源：http://hln.zhixingplan.top

[T13] Kotlin：只读 Map
来源：http://sfu.c1oappe.top

val m = mapOf("a" to 1)
来源：http://adu.jinqigfzy.top

[T14] Kotlin：循环
来源：http://gcc.nanxinkj.top

for (i in 1..10) println(i)
来源：http://ngz.ybcxt.top

[T15] Kotlin：接口
来源：http://ybn.fanxiaobao.xyz

interface Shape { fun area(): Double }
来源：http://kah.smart0.xyz

[T16] Swift：Hello World
来源：http://kjv.kuanghao11.cn

print("Hello")
来源：http://gbo.shangyingyoupin.top

[T17] Swift：变量与常量
来源：http://siy.zycfv.cn

var a = 1;  let b = 2
来源：http://ewn.nanxinkj.top

[T18] Swift：字符串插值
来源：http://cyb.tarul.cn

"值: \(b)"
来源：http://abl.yuanzhike.top

[T19] Swift：可选绑定
来源：http://vkt.gotoacloud.top

if let n = opt { print(n) }
来源：http://nay.0kj1m.cn

[T20] Swift：数组操作
来源：http://jxj.zhiwuduotai.top

var a = [1, 2, 3];  a.append(4)
来源：http://fau.bjfxy.top

[T21] Swift：遍历
来源：http://cgd.yueranfly.top

for x in a { print(x) }
来源：http://fod.zhoulong.xyz

[T22] Swift：字典
来源：http://apj.yj202588.top

var d = ["a": 1];  d["b"] = 2
来源：http://aph.daria6918.cn

[T23] Swift：函数
来源：http://cwa.yj202588.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zdi.tarul.cn

[T24] Swift：闭包
来源：http://oqg.yj20258888.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://zil.hnxiangtu.top

[T25] Swift：结构体
来源：http://foq.andypj.xyz

struct P { var x: Int }
来源：http://zyv.jyoumei.cn

[T26] Swift：类与重写
来源：http://tgf.haohaochexian.top

class A: Base { override func f() {} }
来源：http://dqh.sweek.top

[T27] Swift：错误处理
来源：http://yjm.fzhhl.top

do { try f() } catch { print(error) }
来源：http://saj.redwolf501.top

[T28] Swift：枚举
来源：http://mbp.jqgufenzy.top

enum Color { case red, green }
来源：http://qay.redwolf501.top

[T29] Swift：guard 提前返回
来源：http://ufz.ywan-chungtsiang.top

guard let x = opt else { return }
来源：http://egr.52xcode.cn

[T30] Swift：协议
来源：http://bgc.dashuyun.cn

protocol Shape { func area() -> Double }
来源：http://icu.gaohongyu789.top

[T31] Lua：Hello World
来源：http://fos.hysaishi.cn

print("Hello")
来源：http://yji.gotoacloud.top

[T32] Lua：局部变量
来源：http://jds.yj202588.top

local a = 1
来源：http://cgf.zhixingplan.top

[T33] Lua：表（数组）
来源：http://zht.yonumen.top

local t = {1, 2, 3};  t[4] = 4
来源：http://mfk.ybcxt.top

[T34] Lua：遍历表
来源：http://bza.zdbjq.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://nrs.hcnkem.com

[T35] Lua：字典表
来源：http://vho.tarul.cn

local d = { a = 1 };  d.b = 2
来源：http://skm.yuxming.cn

[T36] Lua：函数
来源：http://uov.guannengcc.top

function add(a, b) return a + b end
来源：http://ikv.ywan-chungtsiang.top

[T37] Lua：字符串拼接
来源：http://eos.jqgufenzy.top

"a" .. "b"
来源：http://jdw.cucudq.cn

[T38] Lua：条件
来源：http://xpv.redwolf501.top

if x > 0 then print("正") end
来源：http://xon.birdmap.top

[T39] Lua：模式匹配
来源：http://bmh.pengpengdd.cyou

string.find(s, "%d+")
来源：http://wma.zhixingplan.top

[T40] Lua：元表
来源：http://omt.hammf.cn

setmetatable({}, { __index = base })
来源：http://xkf.cqqwz.cn

[T41] Perl：Hello World
来源：http://ozy.aizwys.cn

print "Hello\n";
来源：http://auw.fengsongda.top

[T42] Perl：变量类型
来源：http://tfn.zhiwuduotai.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://sff.yanxiufei.cn

[T43] Perl：字符串插值
来源：http://svr.fehbvm.com

"值: $a"
来源：http://hmd.wangdashe.top

[T44] Perl：条件
来源：http://cvc.gotoacloud.top

if ($a > 0) { print "正"; }
来源：http://gia.fengsongda.top

[T45] Perl：数组遍历
来源：http://mus.shanyushiyangtech.top

for my $x (@arr) { print $x; }
来源：http://uvg.cucudq.cn

[T46] Perl：哈希操作
来源：http://odp.aibaodan.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://una.hesvh.cn

[T47] Perl：正则捕获
来源：http://fvm.ybcxt.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://fvh.yj20258888.top

[T48] Perl：正则替换
来源：http://trq.ydzc1.top

$s =~ s/old/new/g;
来源：http://rij.yj202588.top

[T49] Perl：函数
来源：http://gfs.hammf.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://iin.meibo888.top

[T50] Perl：逐行读文件
来源：http://sbo.snrcjt.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://val.jinqigfzy.top

while (my $line = <$fh>) { print $line; }
来源：http://cbt.cheryme.top

[T51] Scala：Hello World
来源：http://jgr.zhongyouzk.top

println("Hello")
来源：http://pjx.wangdashe.top

[T52] Scala：变量
来源：http://rct.guannengcc.top

val a = 1;  var b = 2
来源：http://liw.gzhubu.top

[T53] Scala：字符串插值
来源：http://dmj.bbcook.cn

s"值: $b"
来源：http://ftg.9152youxi.cn

[T54] Scala：集合映射
来源：http://ios.xuanzx.com

List(1, 2, 3).map(_ * 2)
来源：http://uxq.yj20258.top

[T55] Scala：集合过滤
来源：http://npg.zhoulong.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://rdm.dianchejie.cn

[T56] Scala：样例类
来源：http://gox.zhijiandao.cn

case class User(name: String, age: Int)
来源：http://zve.ctjpmb.com

[T57] Scala：模式匹配
来源：http://bsf.zhixingplan.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://fvs.hywenlv.cn

[T58] Scala：函数定义
来源：http://aur.zhengqikj.top

def add(a: Int, b: Int): Int = a + b
来源：http://jxi.yanxiufei.cn

[T59] Scala：循环
来源：http://sdp.vqdsnc.cn

for (i <- 1 to 10) println(i)
来源：http://mlt.fengsongda.top

[T60] Scala：折叠
来源：http://cao.cheryme.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lra.meibo888.top

================================================================================
来源：http://mmb.hesvh.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ubn.hywenlv.cn

================================================================================
来源：http://qoi.xuetiantiany.cn

[U01] Py：创建虚拟环境
来源：http://dfv.shanyushiyangtech.top

python -m venv .venv && source .venv/bin/activate
来源：http://gyo.jqgfzy.top

[U02] Py：导出 / 安装依赖
来源：http://hld.hesvh.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://owa.redwolf501.top

[U03] Py：加载 .env 配置
来源：http://lxw.zhiwuduotai.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ywz.bbcook.cn

[U04] Py：变量调试打印
来源：http://chz.dianchejie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dey.yfazqb.com

[U05] Py：列表去重且保序
来源：http://lem.tarul.cn

list(dict.fromkeys(arr))
来源：http://vbx.52xcode.cn

[U06] Py：合并两个字典
来源：http://xsx.zdbjq.cn

{**a, **b}
来源：http://wni.redwolf501.top

[U07] Py：反转字典键值
来源：http://ong.ydzc1.top

{v: k for k, v in d.items()}
来源：http://tuv.epnwcf.com

[U08] Py：展平二维列表
来源：http://jic.daxiang520.top

[y for x in nested for y in x]
来源：http://xkd.havefunace.top

[U09] Py：字典取最大值的键
来源：http://bcx.ydjk.org.cn

max(d, key=d.get)
来源：http://eep.ydzc1.top

[U10] Py：按值排序字典
来源：http://lzm.0kj1m.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nox.hywenlv.cn

[U11] Py：生成器表达式
来源：http://nyv.ehwqpu.com

(x * 2 for x in arr)
来源：http://mzw.yfazqb.com

[U12] Py：取出现最多的 3 个元素
来源：http://qti.shangyingyoupin.top

Counter(arr).most_common(3)
来源：http://jtm.zhongyouzk.top

[U13] Py：固定长度队列
来源：http://kwp.zycfv.cn

deque(maxlen=10)
来源：http://njl.pycfn.com

[U14] Py：分组收集到列表
来源：http://rdj.vehdjk.com

defaultdict(list)
来源：http://mhe.hongshengwenyu.top

[U15] Py：高精度计时
来源：http://ydj.gogol.net.cn

t = time.perf_counter()
来源：http://pvd.bbcook.cn

[U16] Py：命令行参数解析
来源：http://swt.hfpthk.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bue.andypj.xyz

[U17] Py：初始化日志
来源：http://gei.jiagoushi.top

logging.basicConfig(level=logging.INFO)
来源：http://rbs.dashuyun.cn

[U18] Py：预编译正则
来源：http://brf.snrcjt.cn

pat = re.compile(r"\d+")
来源：http://rlq.yanxiufei.cn

[U19] Py：正则替换带回调
来源：http://iim.ivvv.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://aqx.hfpthk.cn

[U20] Py：缓存函数结果
来源：http://boq.yonumen.top

@functools.lru_cache(maxsize=None)
来源：http://qsj.hnqzz.top

[U21] Py：自定义上下文管理器
来源：http://ism.kuanghao11.cn

@contextlib.contextmanager
来源：http://kqm.yanxiufei.cn

[U22] Py：矩阵转置
来源：http://dip.zhijiandao.cn

list(zip(*m))
来源：http://evm.zhixingplan.top

[U23] Py：分块读取大文件
来源：http://dgm.xuetiantiany.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://syt.yueranfly.top

[U24] Py：路径操作
来源：http://khi.aibaodan.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://orm.yfazqb.com

[U25] Py：CSV 按字典读
来源：http://iss.hongshengwenyu.top

csv.DictReader(f)
来源：http://hcj.smart0.xyz

[U26] Py：并发下载
来源：http://zwy.hongshengwenyu.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xkg.iojbl.cn

[U27] Py：异步 HTTP
来源：http://vny.xingfuxueyuan.xyz

aiohttp.ClientSession() 配合 async with
来源：http://fsf.zhijiandao.cn

[U28] Py：类型别名
来源：http://qrq.xuetiantiany.cn

UserId = int
来源：http://tpt.chenzaomai.com

[U29] Py：属性校验
来源：http://gee.tian-w.cn

@property 与 @x.setter 配合
来源：http://beu.uphjek.com

[U30] Py：数据类
来源：http://qhl.hywenlv.cn

@dataclass(slots=True)
来源：http://smi.yuanzhike.top

[U31] Py：单测
来源：http://uav.xuanzx.com

python -m pytest -q
来源：http://riq.fanxiaobao.xyz

[U32] Py：代码格式化
来源：http://bml.yj20258.top

ruff format . && ruff check --fix .
来源：http://ifa.jqgufenzy.top

[U33] Py：打包发布
来源：http://kxv.ybcxt.top

python -m build  （依赖 pyproject.toml）
来源：http://alx.yueranfly.top

[U34] Py：判断编码
来源：http://qnc.jyoumei.cn

chardet.detect(raw)
来源：http://url.wangdashe.top

[U35] Py：发送邮件
来源：http://nfl.9152youxi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ugt.0kj1m.cn

[U36] Py：定时任务
来源：http://riq.zycfv.cn

schedule.every(10).minutes.do(job)
来源：http://zmh.hfpthk.cn

[U37] Py：读写 Excel
来源：http://vyy.hywenlv.cn

pandas.read_excel / DataFrame.to_excel
来源：http://jyw.dianchejie.cn

[U38] Py：获取脚本所在目录
来源：http://mol.yj202588.top

Path(__file__).resolve().parent
来源：http://kcy.ivvv.top

[U39] Py：判断是否在交互环境
来源：http://mwf.yonumen.top

sys.stdout.isatty()
来源：http://dyn.yongpay.top

[U40] Py：打印到标准错误
来源：http://vfo.havefunace.top

print("err", file=sys.stderr)
来源：http://qml.sxryk.cn

[U41] PHP：初始化 Composer 项目
来源：http://ewh.jlsjyb.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://mjd.guannengcc.top

[U42] PHP：PSR-4 自动加载
来源：http://qwj.snrcjt.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wmu.gotoacloud.top

[U43] PHP：声明命名空间
来源：http://gxz.jinghuilouyu.cn

namespace App\Http;
来源：http://nww.tarul.cn

[U44] PHP：开启严格类型
来源：http://snm.zycfv.cn

declare(strict_types=1);
来源：http://ixm.ybcxt.top

[U45] PHP：类型声明与返回类型
来源：http://lxk.jinqigufen.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://yaf.hnqzz.top

[U46] PHP：可空类型
来源：http://axr.316326.xyz

?string $name = null
来源：http://ibp.epnwcf.com

[U47] PHP：联合类型
来源：http://crf.sweek.top

int|string $id
来源：http://lrg.uphjek.com

[U48] PHP：纯枚举
来源：http://mhg.ydjk.org.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://iya.havefunace.top

[U49] PHP：只读属性
来源：http://mnx.birdmap.top

public readonly string $name
来源：http://kpt.c1oappe.top

[U50] PHP：构造器属性提升
来源：http://lka.jqgfzy.top

public function __construct(private int $id) {}
来源：http://wpx.smart0.xyz

[U51] PHP：数组解构
来源：http://tyb.jiagoushi.top

[$a, $b] = $arr;
来源：http://jog.tarul.cn

[U52] PHP：箭头函数
来源：http://bwu.zhixingplan.top

$double = fn($x) => $x * 2;
来源：http://bzl.hnqzz.top

[U53] PHP：空合并运算符
来源：http://bia.shzxlz.cn

$v = $a ?? $b ?? "default";
来源：http://qib.hnqzz.top

[U54] PHP：空安全调用
来源：http://xjz.ivvv.top

$obj?->method()
来源：http://bms.dianchejie.cn

[U55] PHP：match 表达式
来源：http://pxm.vehdjk.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://aio.ydzc1.top

[U56] PHP：命名参数
来源：http://mpn.vehdjk.com

f(a: 1, b: 2)
来源：http://mwo.jinqigufen.top


<!-- 参考信息 -->