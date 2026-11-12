代发 wailian999

#include <iostream>
来源：http://sug.sufxvd.cn

int main() { std::cout << "Hello\n"; }
来源：http://set.jianghu66.top

[S32] C++：字符串
来源：http://zeg.yj20258888.top

std::string s = "hi";  s += "!";
来源：http://egp.ydjk.org.cn

[S33] C++：vector 增删
来源：http://qml.ivvv.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vue.chenzaomai.com

[S34] C++：遍历 vector
来源：http://krq.yangfankeji.com

for (auto &x : v) { std::cout << x; }
来源：http://edk.zdbjq.cn

[S35] C++：map
来源：http://xfi.meibo888.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jmo.jqgfzy.top

[S36] C++：unordered_map
来源：http://zqs.0kj1m.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jcj.xziqi.cn

[S37] C++：set
来源：http://jxv.yangfankeji.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ulg.hesvh.cn

[S38] C++：排序
来源：http://mkg.yangfankeji.com

std::sort(v.begin(), v.end());
来源：http://joc.xinyue.icu

[S39] C++：自定义比较器排序
来源：http://xpc.shuidangran.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jhd.yangfankeji.com

[S40] C++：查找元素
来源：http://tyh.ywan-chungtsiang.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://equ.shangyingyoupin.top

[S41] C++：类与构造函数
来源：http://dlz.ydjk.org.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://utl.yanxiufei.cn

[S42] C++：继承与虚函数
来源：http://wmy.gzhubu.top

class B : public Base { public: void f() override {} };
来源：http://tdb.zycfv.cn

[S43] C++：智能指针
来源：http://lvr.cashguo.top

auto p = std::make_unique<int>(5);
来源：http://eid.yonumen.top

[S44] C++：引用传参
来源：http://kss.fanxiaobao.xyz

void inc(int &x) { ++x; }
来源：http://luu.yueranfly.top

[S45] C++：lambda
来源：http://wuz.yueranfly.top

auto add = [](int a, int b) { return a + b; };
来源：http://pza.tian-w.cn

[S46] C++：函数模板
来源：http://lvo.feifeiyinyue.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xmu.jlsjyb.cn

[S47] C++：结构化绑定遍历
来源：http://xto.shuidangran.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rgc.yvedp.cn

[S48] C++：逐行读文件
来源：http://zwu.sysykeji.top

std::ifstream in("a.txt");  std::string line;
来源：http://qwy.shangyingyoupin.top

while (std::getline(in, line)) { }
来源：http://cte.ydzc1.top

[S49] C++：写文件
来源：http://pmn.ppjwa.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://eii.havefunace.top

[S50] C++：格式化数字
来源：http://jds.dashuyun.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yyn.chenlongwang.top

[S51] C++：显式类型转换
来源：http://cjg.jinyuanbaomall.cn

static_cast<double>(a) / b
来源：http://tro.chenlongwang.top

[S52] C++：const 与 noexcept
来源：http://dob.andypj.xyz

int size() const noexcept { return n_; }
来源：http://bth.snrcjt.cn

[S53] C++：移动语义
来源：http://ags.0kj1m.cn

std::vector<int> w = std::move(v);
来源：http://gdw.hnqzz.top

[S54] C++：异常处理
来源：http://rkk.zhijiandao.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qrv.havefunace.top

[S55] C++：结构化绑定
来源：http://mfc.cqqwz.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://hfy.ehwqpu.com

[S56] C++：optional
来源：http://tsr.hesvh.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jkp.xylfe.cn

[S57] C++：编译期常量
来源：http://jpu.yonumen.top

constexpr int N = 10;
来源：http://wzo.yonumen.top

[S58] C++：命名空间
来源：http://mzn.bbcook.cn

namespace ns { int f() { return 1; } }
来源：http://ikb.jiagoushi.top

[S59] C++：静态断言
来源：http://gaw.andypj.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vmb.sjlbkw.cn

[S60] C++：遍历并删除元素
来源：http://zgd.pengpengdd.cyou

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gje.hesvh.cn

================================================================================
来源：http://gnj.yj20258.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://syd.yanxiufei.cn

================================================================================
来源：http://hqr.c1oappe.top

[T01] Kotlin：Hello World
来源：http://ola.hammf.cn

println("Hello")
来源：http://qvd.iojbl.cn

[T02] Kotlin：变量
来源：http://dkm.uphjek.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zrx.jinghuilouyu.cn

[T03] Kotlin：字符串模板
来源：http://qjn.9152youxi.cn

"值: $b"
来源：http://reh.sufxvd.cn

[T04] Kotlin：空安全
来源：http://rpr.ybcxt.top

val n: String? = null;  n?.length
来源：http://bgi.tian-w.cn

[T05] Kotlin：when 表达式
来源：http://pfl.mhx1999.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nwz.fktsv.cn

[T06] Kotlin：集合映射
来源：http://jib.ydzc1.top

listOf(1, 2, 3).map { it * 2 }
来源：http://jrb.meibo888.top

[T07] Kotlin：集合过滤
来源：http://roh.andypj.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://qkg.tanke756.top

[T08] Kotlin：数据类
来源：http://ccp.xuanzx.com

data class User(val name: String, val age: Int)
来源：http://miv.redwolf501.top

[T09] Kotlin：扩展函数
来源：http://tng.ctjpmb.com

fun String.exclaim() = this + "!"
来源：http://cqx.shanyushiyangkeji.top

[T10] Kotlin：默认参数
来源：http://doa.nwbrower.top

fun greet(name: String = "World") = "Hi $name"
来源：http://dsq.vqdsnc.cn

[T11] Kotlin：协程
来源：http://gtz.jianghu66.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://eud.9152youxi.cn

[T12] Kotlin：解构声明
来源：http://gob.meibo888.top

val (a, b) = Pair(1, 2)
来源：http://zrp.c1oappe.top

[T13] Kotlin：只读 Map
来源：http://mly.hysaishi.cn

val m = mapOf("a" to 1)
来源：http://jpm.c1oappe.top

[T14] Kotlin：循环
来源：http://tch.316326.xyz

for (i in 1..10) println(i)
来源：http://nrc.zhengqikj.top

[T15] Kotlin：接口
来源：http://peh.chenlongwang.top

interface Shape { fun area(): Double }
来源：http://sda.c1oappe.top

[T16] Swift：Hello World
来源：http://pma.yj20258.top

print("Hello")
来源：http://rdd.tanke756.top

[T17] Swift：变量与常量
来源：http://ilj.jqgufenzy.top

var a = 1;  let b = 2
来源：http://dfo.daria6918.cn

[T18] Swift：字符串插值
来源：http://woh.jqgfzy.top

"值: \(b)"
来源：http://jqj.cqqwz.cn

[T19] Swift：可选绑定
来源：http://gge.hysaishi.cn

if let n = opt { print(n) }
来源：http://drr.xingfuxueyuan.xyz

[T20] Swift：数组操作
来源：http://acz.fengsongda.top

var a = [1, 2, 3];  a.append(4)
来源：http://wgy.hywenlv.cn

[T21] Swift：遍历
来源：http://wum.jqgufenzy.top

for x in a { print(x) }
来源：http://aez.ydzc1.top

[T22] Swift：字典
来源：http://oeo.nanxinkj.top

var d = ["a": 1];  d["b"] = 2
来源：http://stm.kuanghao11.cn

[T23] Swift：函数
来源：http://tcp.mhx1999.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://uvr.hammf.cn

[T24] Swift：闭包
来源：http://ubr.yj20258.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://coo.shangyingyoupin.top

[T25] Swift：结构体
来源：http://smm.jqgufenzy.top

struct P { var x: Int }
来源：http://eub.fktsv.cn

[T26] Swift：类与重写
来源：http://inf.jlsjyb.cn

class A: Base { override func f() {} }
来源：http://piw.pengpengdd.cyou

[T27] Swift：错误处理
来源：http://zgn.jinqigufen.top

do { try f() } catch { print(error) }
来源：http://cni.jqgufenzy.top

[T28] Swift：枚举
来源：http://hyv.fzhhl.top

enum Color { case red, green }
来源：http://jqo.yuxming.cn

[T29] Swift：guard 提前返回
来源：http://yzw.ydzc1.top

guard let x = opt else { return }
来源：http://rmi.yanxiufei.cn

[T30] Swift：协议
来源：http://eyi.jqgfzy.top

protocol Shape { func area() -> Double }
来源：http://nza.ydzc1.top

[T31] Lua：Hello World
来源：http://exw.hfpthk.cn

print("Hello")
来源：http://xvx.fanxiaobao.xyz

[T32] Lua：局部变量
来源：http://rqn.hongshengwenyu.top

local a = 1
来源：http://vyq.yanxiufei.cn

[T33] Lua：表（数组）
来源：http://bgf.yanxiufei.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://pwi.ywan-chungtsiang.top

[T34] Lua：遍历表
来源：http://kis.yueranfly.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ekw.shzxlz.cn

[T35] Lua：字典表
来源：http://gwn.jqgfzy.top

local d = { a = 1 };  d.b = 2
来源：http://ems.yonumen.top

[T36] Lua：函数
来源：http://rhj.hcnkem.com

function add(a, b) return a + b end
来源：http://plp.dashuyun.cn

[T37] Lua：字符串拼接
来源：http://ujx.andypj.xyz

"a" .. "b"
来源：http://tcd.havefunace.top

[T38] Lua：条件
来源：http://spb.xylfe.cn

if x > 0 then print("正") end
来源：http://ojd.yvedp.cn

[T39] Lua：模式匹配
来源：http://ykf.hongshengwenyu.top

string.find(s, "%d+")
来源：http://mvn.yanxiufei.cn

[T40] Lua：元表
来源：http://iqe.yj202588.top

setmetatable({}, { __index = base })
来源：http://rkv.hysaishi.cn

[T41] Perl：Hello World
来源：http://pns.hongshengwenyu.top

print "Hello\n";
来源：http://nzl.yongpay.top

[T42] Perl：变量类型
来源：http://mhn.wangdashe.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ett.shanyushiyangkeji.top

[T43] Perl：字符串插值
来源：http://anw.daxiang520.top

"值: $a"
来源：http://mrt.yuanzhike.top

[T44] Perl：条件
来源：http://eyt.tian-w.cn

if ($a > 0) { print "正"; }
来源：http://kkv.yanxiufei.cn

[T45] Perl：数组遍历
来源：http://ybc.cqqwz.cn

for my $x (@arr) { print $x; }
来源：http://sro.xylfe.cn

[T46] Perl：哈希操作
来源：http://drf.epnwcf.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cmv.tian-w.cn

[T47] Perl：正则捕获
来源：http://tuv.bbcook.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://hmd.jinqigufen.top

[T48] Perl：正则替换
来源：http://zxg.chenlongwang.top

$s =~ s/old/new/g;
来源：http://cei.haohaochexian.top

[T49] Perl：函数
来源：http://raf.hnqzz.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dsr.hesvh.cn

[T50] Perl：逐行读文件
来源：http://unb.zhongyouzk.top

open my $fh, "<", "a.txt" or die $!;
来源：http://hzz.zdbjq.cn

while (my $line = <$fh>) { print $line; }
来源：http://iqk.ehwqpu.com

[T51] Scala：Hello World
来源：http://mpt.shangyingyoupin.top

println("Hello")
来源：http://cix.guannengcc.top

[T52] Scala：变量
来源：http://tts.ywan-chungtsiang.top

val a = 1;  var b = 2
来源：http://ydo.yj20258.top

[T53] Scala：字符串插值
来源：http://gwy.guowangkeji.top

s"值: $b"
来源：http://hrq.yj20258888.top

[T54] Scala：集合映射
来源：http://muz.haohaochexian.top

List(1, 2, 3).map(_ * 2)
来源：http://gnq.dashuyun.cn

[T55] Scala：集合过滤
来源：http://zoa.yangfankeji.com

List(1, 2, 3).filter(_ > 1)
来源：http://hqs.fanxiaobao.xyz

[T56] Scala：样例类
来源：http://kpo.svipenyu.cn

case class User(name: String, age: Int)
来源：http://mru.mhx1999.top

[T57] Scala：模式匹配
来源：http://acl.jinyuanbaomall.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://hnm.ydjk.org.cn

[T58] Scala：函数定义
来源：http://ztp.yuxming.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ege.sjlbkw.cn

[T59] Scala：循环
来源：http://rrk.hcnkem.com

for (i <- 1 to 10) println(i)
来源：http://jsv.zhixingplan.top

[T60] Scala：折叠
来源：http://kos.hesvh.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wqn.hywenlv.cn

================================================================================
来源：http://iyn.ctjpmb.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://imu.iojbl.cn

================================================================================
来源：http://ghm.shanyushiyangtech.top

[U01] Py：创建虚拟环境
来源：http://fqw.daria6918.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ksx.xuetiantiany.cn

[U02] Py：导出 / 安装依赖
来源：http://cjb.9152youxi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://oel.fzhhl.top

[U03] Py：加载 .env 配置
来源：http://hbx.ehwqpu.com

from dotenv import load_dotenv; load_dotenv()
来源：http://jzm.tianlin.xyz

[U04] Py：变量调试打印
来源：http://mtz.shanyushiyangkeji.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lzq.feifeiyinyue.top

[U05] Py：列表去重且保序
来源：http://jvr.shanyushiyangkeji.top

list(dict.fromkeys(arr))
来源：http://nry.shanyushiyangkeji.top

[U06] Py：合并两个字典
来源：http://ttx.gzhubu.top

{**a, **b}
来源：http://lvh.jlsjyb.cn

[U07] Py：反转字典键值
来源：http://iro.cheryme.top

{v: k for k, v in d.items()}
来源：http://gsr.jqgfzy.top

[U08] Py：展平二维列表
来源：http://sfr.redwolf501.top

[y for x in nested for y in x]
来源：http://fap.jiagoushi.top

[U09] Py：字典取最大值的键
来源：http://kta.jqgfzy.top

max(d, key=d.get)
来源：http://hka.cucudq.cn

[U10] Py：按值排序字典
来源：http://kkb.pengpengdd.cyou

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://orn.xuetiantiany.cn

[U11] Py：生成器表达式
来源：http://wxv.wangdashe.top

(x * 2 for x in arr)
来源：http://xob.jinyuanbaomall.cn

[U12] Py：取出现最多的 3 个元素
来源：http://rbm.yvedp.cn

Counter(arr).most_common(3)
来源：http://ble.daria6918.cn

[U13] Py：固定长度队列
来源：http://mty.ydjk.org.cn

deque(maxlen=10)
来源：http://ceq.jinyuanbaomall.cn

[U14] Py：分组收集到列表
来源：http://xjt.gotoacloud.top

defaultdict(list)
来源：http://ztv.52xcode.cn

[U15] Py：高精度计时
来源：http://whd.chenlongwang.top

t = time.perf_counter()
来源：http://ivq.xziqi.cn

[U16] Py：命令行参数解析
来源：http://eqk.jianghu66.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kew.sysykeji.top

[U17] Py：初始化日志
来源：http://tre.9152youxi.cn

logging.basicConfig(level=logging.INFO)
来源：http://ubi.quarkkingdee.top

[U18] Py：预编译正则
来源：http://zex.cheryme.top

pat = re.compile(r"\d+")
来源：http://hox.epnwcf.com

[U19] Py：正则替换带回调
来源：http://byg.redwolf501.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kbe.snrcjt.cn

[U20] Py：缓存函数结果
来源：http://sdj.yueranfly.top

@functools.lru_cache(maxsize=None)
来源：http://hed.wangshuangyany.cn

[U21] Py：自定义上下文管理器
来源：http://bwi.jinghuilouyu.cn

@contextlib.contextmanager
来源：http://szc.smart0.xyz

[U22] Py：矩阵转置
来源：http://gwc.cashguo.top

list(zip(*m))
来源：http://pts.tarul.cn

[U23] Py：分块读取大文件
来源：http://ogr.yuanzhike.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jst.jinghuilouyu.cn

[U24] Py：路径操作
来源：http://jyi.zhaomingkeji.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wri.hnqzz.top

[U25] Py：CSV 按字典读
来源：http://pww.gotoacloud.top

csv.DictReader(f)
来源：http://zrs.aizwys.cn

[U26] Py：并发下载
来源：http://ljr.0kj1m.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://awy.vehdjk.com

[U27] Py：异步 HTTP
来源：http://muw.tian-w.cn

aiohttp.ClientSession() 配合 async with
来源：http://ajg.zhijiandao.cn

[U28] Py：类型别名
来源：http://eos.fzhhl.top

UserId = int
来源：http://dbs.52xcode.cn

[U29] Py：属性校验
来源：http://jbd.epnwcf.com

@property 与 @x.setter 配合
来源：http://hol.0kj1m.cn

[U30] Py：数据类
来源：http://ftq.hesvh.cn

@dataclass(slots=True)
来源：http://sms.gzhubu.top

[U31] Py：单测
来源：http://stb.dianchejie.cn

python -m pytest -q
来源：http://jkf.ywan-chungtsiang.top

[U32] Py：代码格式化
来源：http://eui.redwolf501.top

ruff format . && ruff check --fix .
来源：http://ski.hnxiangtu.top

[U33] Py：打包发布
来源：http://zzg.mhx1999.top

python -m build  （依赖 pyproject.toml）
来源：http://eid.uphjek.com

[U34] Py：判断编码
来源：http://ywc.dianchejie.cn

chardet.detect(raw)
来源：http://vlc.jinqigufen.top

[U35] Py：发送邮件
来源：http://tvg.hfpthk.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ybq.c1oappe.top

[U36] Py：定时任务
来源：http://byg.shanyushiyangtech.top

schedule.every(10).minutes.do(job)
来源：http://lsa.gotoacloud.top

[U37] Py：读写 Excel
来源：http://mqn.jinqigufen.top

pandas.read_excel / DataFrame.to_excel
来源：http://gcj.nanxuanxn.top

[U38] Py：获取脚本所在目录
来源：http://flg.cqqwz.cn

Path(__file__).resolve().parent
来源：http://trg.jianghu66.top

[U39] Py：判断是否在交互环境
来源：http://nro.ctjpmb.com

sys.stdout.isatty()
来源：http://cho.dianchejie.cn

[U40] Py：打印到标准错误
来源：http://awx.cashguo.top

print("err", file=sys.stderr)
来源：http://zkr.yj20258888.top

[U41] PHP：初始化 Composer 项目
来源：http://tup.sjlbkw.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ivs.zhengqikj.top

[U42] PHP：PSR-4 自动加载
来源：http://voj.aibaodan.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qtr.xylfe.cn

[U43] PHP：声明命名空间
来源：http://kqo.fzhhl.top

namespace App\Http;
来源：http://azm.gzhubu.top

[U44] PHP：开启严格类型
来源：http://zyl.xingfuxueyuan.xyz

declare(strict_types=1);
来源：http://hil.yj202588.top

[U45] PHP：类型声明与返回类型
来源：http://wub.zhaomingkeji.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://yel.hfpthk.cn

[U46] PHP：可空类型
来源：http://wcv.9152youxi.cn

?string $name = null
来源：http://uoq.hysaishi.cn

[U47] PHP：联合类型
来源：http://pwx.shanyushiyangtech.top

int|string $id
来源：http://bsz.aizwys.cn

[U48] PHP：纯枚举
来源：http://kta.hysaishi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cgo.xziqi.cn

[U49] PHP：只读属性
来源：http://mdb.havefunace.top

public readonly string $name
来源：http://drg.yvedp.cn

[U50] PHP：构造器属性提升
来源：http://lxr.tianlin.xyz

public function __construct(private int $id) {}
来源：http://cve.xinyue.icu

[U51] PHP：数组解构
来源：http://rrm.meibo888.top

[$a, $b] = $arr;
来源：http://pop.zhongyouzk.top

[U52] PHP：箭头函数
来源：http://dtj.xuanzx.com

$double = fn($x) => $x * 2;
来源：http://yrj.jiagoushi.top

[U53] PHP：空合并运算符
来源：http://cvu.xuetiantiany.cn

$v = $a ?? $b ?? "default";
来源：http://ymo.nanxuanxn.top

[U54] PHP：空安全调用
来源：http://ugx.ppjwa.cn

$obj?->method()
来源：http://zid.pycfn.com

[U55] PHP：match 表达式
来源：http://jxf.vqdsnc.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hye.hywenlv.cn

[U56] PHP：命名参数
来源：http://klo.sjlbkw.cn

f(a: 1, b: 2)
来源：http://sdp.daxiang520.top


<!-- 参考信息 -->