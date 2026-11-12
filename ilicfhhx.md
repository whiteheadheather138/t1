代发 wailian999

#include <iostream>
来源：http://jfq.epnwcf.com

int main() { std::cout << "Hello\n"; }
来源：http://gkq.9152youxi.cn

[S32] C++：字符串
来源：http://hyl.cdnleiting.top

std::string s = "hi";  s += "!";
来源：http://xql.haohaochexian.top

[S33] C++：vector 增删
来源：http://gms.vehdjk.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yaa.xylfe.cn

[S34] C++：遍历 vector
来源：http://snd.cqqwz.cn

for (auto &x : v) { std::cout << x; }
来源：http://ibo.yanxiufei.cn

[S35] C++：map
来源：http://jdi.gzhubu.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rii.gogol.net.cn

[S36] C++：unordered_map
来源：http://hke.zdbjq.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dkp.shangyingyoupin.top

[S37] C++：set
来源：http://cdq.epnwcf.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ngh.yonumen.top

[S38] C++：排序
来源：http://irw.yj20258888.top

std::sort(v.begin(), v.end());
来源：http://yjm.xziqi.cn

[S39] C++：自定义比较器排序
来源：http://izk.0kj1m.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tub.c1oappe.top

[S40] C++：查找元素
来源：http://jqq.ehwqpu.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fho.birdmap.top

[S41] C++：类与构造函数
来源：http://vmv.jiagoushi.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kvw.yuxming.cn

[S42] C++：继承与虚函数
来源：http://dwf.bjfxy.top

class B : public Base { public: void f() override {} };
来源：http://cic.hesvh.cn

[S43] C++：智能指针
来源：http://yhi.yuanzhike.top

auto p = std::make_unique<int>(5);
来源：http://mkm.aizwys.cn

[S44] C++：引用传参
来源：http://dta.zhengqikj.top

void inc(int &x) { ++x; }
来源：http://eeh.xuetiantiany.cn

[S45] C++：lambda
来源：http://zqz.9152youxi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://jpz.birdmap.top

[S46] C++：函数模板
来源：http://miz.cdnleiting.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://evv.jinghuilouyu.cn

[S47] C++：结构化绑定遍历
来源：http://emi.guowangkeji.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vts.tarul.cn

[S48] C++：逐行读文件
来源：http://uch.hongshengwenyu.top

std::ifstream in("a.txt");  std::string line;
来源：http://qvh.316326.xyz

while (std::getline(in, line)) { }
来源：http://lce.jyoumei.cn

[S49] C++：写文件
来源：http://mif.vqdsnc.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dva.zhaomingkeji.xyz

[S50] C++：格式化数字
来源：http://brl.dashuyun.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ljf.xinyue.icu

[S51] C++：显式类型转换
来源：http://coi.ydjk.org.cn

static_cast<double>(a) / b
来源：http://fbv.pycfn.com

[S52] C++：const 与 noexcept
来源：http://nvy.xingfuxueyuan.xyz

int size() const noexcept { return n_; }
来源：http://gbg.hywenlv.cn

[S53] C++：移动语义
来源：http://rfb.guannengcc.top

std::vector<int> w = std::move(v);
来源：http://liz.nanxuanxn.top

[S54] C++：异常处理
来源：http://tpa.gaohongyu789.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pwt.dianchejie.cn

[S55] C++：结构化绑定
来源：http://xfc.nanxuanxn.top

auto [a, b] = std::make_pair(1, 2);
来源：http://zig.xziqi.cn

[S56] C++：optional
来源：http://epc.dashuyun.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cxr.hywenlv.cn

[S57] C++：编译期常量
来源：http://qhi.yueranfly.top

constexpr int N = 10;
来源：http://jcg.nanxuanxn.top

[S58] C++：命名空间
来源：http://dff.tanke756.top

namespace ns { int f() { return 1; } }
来源：http://hwz.redwolf501.top

[S59] C++：静态断言
来源：http://gdo.redwolf501.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xaz.vqdsnc.cn

[S60] C++：遍历并删除元素
来源：http://xwf.shuidangran.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://phu.zhoulong.xyz

================================================================================
来源：http://pno.gotoacloud.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dum.zhaomingkeji.xyz

================================================================================
来源：http://zem.shzxlz.cn

[T01] Kotlin：Hello World
来源：http://lit.9152youxi.cn

println("Hello")
来源：http://tmy.c1oappe.top

[T02] Kotlin：变量
来源：http://vvw.ywan-chungtsiang.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://igu.nwbrower.top

[T03] Kotlin：字符串模板
来源：http://uqc.andypj.xyz

"值: $b"
来源：http://wmg.shangyingyoupin.top

[T04] Kotlin：空安全
来源：http://mfj.yuxming.cn

val n: String? = null;  n?.length
来源：http://xtz.jqgfzy.top

[T05] Kotlin：when 表达式
来源：http://poe.sweek.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://psv.hcnkem.com

[T06] Kotlin：集合映射
来源：http://tbd.fktsv.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://zzc.hesvh.cn

[T07] Kotlin：集合过滤
来源：http://poh.sysykeji.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://dib.uphjek.com

[T08] Kotlin：数据类
来源：http://xwo.haohaochexian.top

data class User(val name: String, val age: Int)
来源：http://vnb.havefunace.top

[T09] Kotlin：扩展函数
来源：http://zzh.yuanzhike.top

fun String.exclaim() = this + "!"
来源：http://jxm.wangshuangyany.cn

[T10] Kotlin：默认参数
来源：http://mto.xingfuxueyuan.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://pgi.tarul.cn

[T11] Kotlin：协程
来源：http://mwt.nanxuanxn.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://row.vehdjk.com

[T12] Kotlin：解构声明
来源：http://qmx.aibaodan.cn

val (a, b) = Pair(1, 2)
来源：http://usq.yj202588.top

[T13] Kotlin：只读 Map
来源：http://pmn.ppjwa.cn

val m = mapOf("a" to 1)
来源：http://rxf.kuanghao11.cn

[T14] Kotlin：循环
来源：http://oqj.tarul.cn

for (i in 1..10) println(i)
来源：http://yic.ydzc1.top

[T15] Kotlin：接口
来源：http://zex.wangdashe.top

interface Shape { fun area(): Double }
来源：http://ndk.aibaodan.cn

[T16] Swift：Hello World
来源：http://ekj.chenzaomai.com

print("Hello")
来源：http://tnc.xuetiantiany.cn

[T17] Swift：变量与常量
来源：http://lsz.hammf.cn

var a = 1;  let b = 2
来源：http://pan.hfpthk.cn

[T18] Swift：字符串插值
来源：http://qsz.zhiwuduotai.top

"值: \(b)"
来源：http://xbi.xylfe.cn

[T19] Swift：可选绑定
来源：http://ggt.yj20258.top

if let n = opt { print(n) }
来源：http://rtc.sxryk.cn

[T20] Swift：数组操作
来源：http://ckw.jqgufenzy.top

var a = [1, 2, 3];  a.append(4)
来源：http://wto.ehwqpu.com

[T21] Swift：遍历
来源：http://rsd.aibaodan.cn

for x in a { print(x) }
来源：http://mib.fktsv.cn

[T22] Swift：字典
来源：http://gtb.zhiwuduotai.top

var d = ["a": 1];  d["b"] = 2
来源：http://cxg.yj20258.top

[T23] Swift：函数
来源：http://tcf.svipenyu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fal.bbcook.cn

[T24] Swift：闭包
来源：http://rez.fanxiaobao.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://kau.wangdashe.top

[T25] Swift：结构体
来源：http://meo.xingfuxueyuan.xyz

struct P { var x: Int }
来源：http://gdw.sweek.top

[T26] Swift：类与重写
来源：http://mdy.52xcode.cn

class A: Base { override func f() {} }
来源：http://syt.shzxlz.cn

[T27] Swift：错误处理
来源：http://dqf.yonumen.top

do { try f() } catch { print(error) }
来源：http://swi.yj20258888.top

[T28] Swift：枚举
来源：http://ujc.yonumen.top

enum Color { case red, green }
来源：http://brq.jlsjyb.cn

[T29] Swift：guard 提前返回
来源：http://cxm.ehwqpu.com

guard let x = opt else { return }
来源：http://jhp.hammf.cn

[T30] Swift：协议
来源：http://jad.aizwys.cn

protocol Shape { func area() -> Double }
来源：http://vmr.zhoulong.xyz

[T31] Lua：Hello World
来源：http://jdl.sxryk.cn

print("Hello")
来源：http://obq.jianghu66.top

[T32] Lua：局部变量
来源：http://xuw.yongpay.top

local a = 1
来源：http://mxm.zhoulong.xyz

[T33] Lua：表（数组）
来源：http://wuy.jinyuanbaomall.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://whm.hcnkem.com

[T34] Lua：遍历表
来源：http://qmg.nanxuanxn.top

for i, v in ipairs(t) do print(i, v) end
来源：http://vmk.sjlbkw.cn

[T35] Lua：字典表
来源：http://pnd.tarul.cn

local d = { a = 1 };  d.b = 2
来源：http://scy.ctjpmb.com

[T36] Lua：函数
来源：http://zaa.wangshuangyany.cn

function add(a, b) return a + b end
来源：http://bnr.feifeiyinyue.top

[T37] Lua：字符串拼接
来源：http://wqo.svipenyu.cn

"a" .. "b"
来源：http://oga.cdnleiting.top

[T38] Lua：条件
来源：http://txq.aizwys.cn

if x > 0 then print("正") end
来源：http://ehm.ywan-chungtsiang.top

[T39] Lua：模式匹配
来源：http://fcr.uphjek.com

string.find(s, "%d+")
来源：http://oje.fzhhl.top

[T40] Lua：元表
来源：http://adp.gzhubu.top

setmetatable({}, { __index = base })
来源：http://axd.yongpay.top

[T41] Perl：Hello World
来源：http://twf.wangshuangyany.cn

print "Hello\n";
来源：http://ibg.zhiwuduotai.top

[T42] Perl：变量类型
来源：http://jau.mhx1999.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xjp.iojbl.cn

[T43] Perl：字符串插值
来源：http://lnk.zhongyouzk.top

"值: $a"
来源：http://nji.nanxinkj.top

[T44] Perl：条件
来源：http://fdq.sweek.top

if ($a > 0) { print "正"; }
来源：http://ewt.tanke756.top

[T45] Perl：数组遍历
来源：http://cbp.mhx1999.top

for my $x (@arr) { print $x; }
来源：http://fww.feifeiyinyue.top

[T46] Perl：哈希操作
来源：http://ske.chenlongwang.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cwq.fzhhl.top

[T47] Perl：正则捕获
来源：http://lwn.jianghu66.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://myv.hfpthk.cn

[T48] Perl：正则替换
来源：http://hpg.iojbl.cn

$s =~ s/old/new/g;
来源：http://wxd.hfpthk.cn

[T49] Perl：函数
来源：http://pea.zhaomingkeji.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://oac.sxryk.cn

[T50] Perl：逐行读文件
来源：http://clm.wangdashe.top

open my $fh, "<", "a.txt" or die $!;
来源：http://hev.shzxlz.cn

while (my $line = <$fh>) { print $line; }
来源：http://ypv.shuidangran.top

[T51] Scala：Hello World
来源：http://xbb.xinyue.icu

println("Hello")
来源：http://uwq.jqgufenzy.top

[T52] Scala：变量
来源：http://qgz.dianchejie.cn

val a = 1;  var b = 2
来源：http://kod.52xcode.cn

[T53] Scala：字符串插值
来源：http://dec.zhengqikj.top

s"值: $b"
来源：http://nrv.ydjk.org.cn

[T54] Scala：集合映射
来源：http://srw.jlsjyb.cn

List(1, 2, 3).map(_ * 2)
来源：http://kxk.zhaomingkeji.xyz

[T55] Scala：集合过滤
来源：http://ske.ydjk.org.cn

List(1, 2, 3).filter(_ > 1)
来源：http://uhu.jinyuanbaomall.cn

[T56] Scala：样例类
来源：http://dnr.daxiang520.top

case class User(name: String, age: Int)
来源：http://swr.fanxiaobao.xyz

[T57] Scala：模式匹配
来源：http://hzd.zhongyouzk.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://aod.zdqjudy.top

[T58] Scala：函数定义
来源：http://cpp.yonumen.top

def add(a: Int, b: Int): Int = a + b
来源：http://rgi.fzhhl.top

[T59] Scala：循环
来源：http://evt.zhiwuduotai.top

for (i <- 1 to 10) println(i)
来源：http://vwp.fanxiaobao.xyz

[T60] Scala：折叠
来源：http://prt.daria6918.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nwo.smart0.xyz

================================================================================
来源：http://oka.uphjek.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gyk.ppjwa.cn

================================================================================
来源：http://wzq.snrcjt.cn

[U01] Py：创建虚拟环境
来源：http://blw.52xcode.cn

python -m venv .venv && source .venv/bin/activate
来源：http://pjw.hywenlv.cn

[U02] Py：导出 / 安装依赖
来源：http://xdw.vehdjk.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://orw.guannengcc.top

[U03] Py：加载 .env 配置
来源：http://fwt.ywan-chungtsiang.top

from dotenv import load_dotenv; load_dotenv()
来源：http://qhs.sweek.top

[U04] Py：变量调试打印
来源：http://eul.tarul.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fea.xuetiantiany.cn

[U05] Py：列表去重且保序
来源：http://hdk.nanxuanxn.top

list(dict.fromkeys(arr))
来源：http://quz.redwolf501.top

[U06] Py：合并两个字典
来源：http://cra.vqdsnc.cn

{**a, **b}
来源：http://fwz.hongshengwenyu.top

[U07] Py：反转字典键值
来源：http://mgi.nanxinkj.top

{v: k for k, v in d.items()}
来源：http://kbo.jiagoushi.top

[U08] Py：展平二维列表
来源：http://mqz.birdmap.top

[y for x in nested for y in x]
来源：http://sxi.jinghuilouyu.cn

[U09] Py：字典取最大值的键
来源：http://lag.jinyuanbaomall.cn

max(d, key=d.get)
来源：http://wnv.316326.xyz

[U10] Py：按值排序字典
来源：http://gyp.jiagoushi.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jki.jqgfzy.top

[U11] Py：生成器表达式
来源：http://frb.gogol.net.cn

(x * 2 for x in arr)
来源：http://nnn.zhaomingkeji.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://hql.xingfuxueyuan.xyz

Counter(arr).most_common(3)
来源：http://ejp.hongshengwenyu.top

[U13] Py：固定长度队列
来源：http://dus.yj202588.top

deque(maxlen=10)
来源：http://umb.dashuyun.cn

[U14] Py：分组收集到列表
来源：http://jez.feifeiyinyue.top

defaultdict(list)
来源：http://bwv.hongshengwenyu.top

[U15] Py：高精度计时
来源：http://awx.yj202588.top

t = time.perf_counter()
来源：http://ecv.iojbl.cn

[U16] Py：命令行参数解析
来源：http://zbm.ydzc1.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yge.yuanzhike.top

[U17] Py：初始化日志
来源：http://jxh.xinyue.icu

logging.basicConfig(level=logging.INFO)
来源：http://trw.tianlin.xyz

[U18] Py：预编译正则
来源：http://zpk.tarul.cn

pat = re.compile(r"\d+")
来源：http://kig.shangyingyoupin.top

[U19] Py：正则替换带回调
来源：http://maj.iojbl.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wiz.yonumen.top

[U20] Py：缓存函数结果
来源：http://pfi.gaohongyu789.top

@functools.lru_cache(maxsize=None)
来源：http://jmy.0kj1m.cn

[U21] Py：自定义上下文管理器
来源：http://xcw.tanke756.top

@contextlib.contextmanager
来源：http://vpu.cqqwz.cn

[U22] Py：矩阵转置
来源：http://bsd.daxiang520.top

list(zip(*m))
来源：http://ifu.zhoulong.xyz

[U23] Py：分块读取大文件
来源：http://utu.snrcjt.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://svr.jlsjyb.cn

[U24] Py：路径操作
来源：http://gza.nanxuanxn.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hjd.jqgufenzy.top

[U25] Py：CSV 按字典读
来源：http://yfg.yvedp.cn

csv.DictReader(f)
来源：http://vdi.cashguo.top

[U26] Py：并发下载
来源：http://nbt.birdmap.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://oav.vehdjk.com

[U27] Py：异步 HTTP
来源：http://bky.yueranfly.top

aiohttp.ClientSession() 配合 async with
来源：http://ktl.fktsv.cn

[U28] Py：类型别名
来源：http://ocl.zdqjudy.top

UserId = int
来源：http://inh.andypj.xyz

[U29] Py：属性校验
来源：http://jzc.kuanghao11.cn

@property 与 @x.setter 配合
来源：http://iba.xuetiantiany.cn

[U30] Py：数据类
来源：http://hxi.cqqwz.cn

@dataclass(slots=True)
来源：http://hlv.fehbvm.com

[U31] Py：单测
来源：http://jmt.guannengcc.top

python -m pytest -q
来源：http://dee.hcnkem.com

[U32] Py：代码格式化
来源：http://nnv.shangyingyoupin.top

ruff format . && ruff check --fix .
来源：http://nfo.tianlin.xyz

[U33] Py：打包发布
来源：http://hzu.dianchejie.cn

python -m build  （依赖 pyproject.toml）
来源：http://cvk.52xcode.cn

[U34] Py：判断编码
来源：http://yvx.bjfxy.top

chardet.detect(raw)
来源：http://hdw.hesvh.cn

[U35] Py：发送邮件
来源：http://asl.9152youxi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://uer.jinqigufen.top

[U36] Py：定时任务
来源：http://ule.sufxvd.cn

schedule.every(10).minutes.do(job)
来源：http://zlr.ydjk.org.cn

[U37] Py：读写 Excel
来源：http://wvx.iojbl.cn

pandas.read_excel / DataFrame.to_excel
来源：http://sio.snrcjt.cn

[U38] Py：获取脚本所在目录
来源：http://lli.yonumen.top

Path(__file__).resolve().parent
来源：http://dct.pengpengdd.cyou

[U39] Py：判断是否在交互环境
来源：http://fzg.hcnkem.com

sys.stdout.isatty()
来源：http://qjg.guowangkeji.top

[U40] Py：打印到标准错误
来源：http://jll.guowangkeji.top

print("err", file=sys.stderr)
来源：http://tzp.sufxvd.cn

[U41] PHP：初始化 Composer 项目
来源：http://wnk.shanyushiyangtech.top

composer init;  composer require guzzlehttp/guzzle
来源：http://eyu.yuanzhike.top

[U42] PHP：PSR-4 自动加载
来源：http://vkm.yvedp.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://czn.fanxiaobao.xyz

[U43] PHP：声明命名空间
来源：http://nyh.bjfxy.top

namespace App\Http;
来源：http://wvz.yj20258888.top

[U44] PHP：开启严格类型
来源：http://iup.jinghuilouyu.cn

declare(strict_types=1);
来源：http://qqo.shanyushiyangkeji.top

[U45] PHP：类型声明与返回类型
来源：http://uyp.jyoumei.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://tmc.zhoulong.xyz

[U46] PHP：可空类型
来源：http://mqd.fktsv.cn

?string $name = null
来源：http://xsc.sjlbkw.cn

[U47] PHP：联合类型
来源：http://mlx.hongshengwenyu.top

int|string $id
来源：http://agu.yanxiufei.cn

[U48] PHP：纯枚举
来源：http://ocg.xylfe.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://iag.sysykeji.top

[U49] PHP：只读属性
来源：http://mgb.gaohongyu789.top

public readonly string $name
来源：http://oeg.yvedp.cn

[U50] PHP：构造器属性提升
来源：http://nym.feifeiyinyue.top

public function __construct(private int $id) {}
来源：http://frg.shanyushiyangtech.top

[U51] PHP：数组解构
来源：http://sla.xylfe.cn

[$a, $b] = $arr;
来源：http://wmh.quarkkingdee.top

[U52] PHP：箭头函数
来源：http://jmi.jyoumei.cn

$double = fn($x) => $x * 2;
来源：http://znt.fzhhl.top

[U53] PHP：空合并运算符
来源：http://kpc.hywenlv.cn

$v = $a ?? $b ?? "default";
来源：http://ajf.chenzaomai.com

[U54] PHP：空安全调用
来源：http://eov.fengsongda.top

$obj?->method()
来源：http://vvu.jinqigfzy.top

[U55] PHP：match 表达式
来源：http://tvc.tian-w.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qjz.zhijiandao.cn

[U56] PHP：命名参数
来源：http://ndt.dianchejie.cn

f(a: 1, b: 2)
来源：http://fqp.yueranfly.top


<!-- 参考信息 -->