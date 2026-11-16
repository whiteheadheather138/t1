代发 wailian999

#ifndef X_H
来源：http://tqx.feifeiyinyue.top

#define X_H
来源：http://evv.jinghuilouyu.cn

#endif
来源：http://sku.fzhhl.top

[S31] C++：Hello World
来源：http://rcr.yj202588.top

#include <iostream>
来源：http://olb.xuetiantiany.cn

int main() { std::cout << "Hello\n"; }
来源：http://eup.yangfankeji.com

[S32] C++：字符串
来源：http://eyo.316326.xyz

std::string s = "hi";  s += "!";
来源：http://fco.ydzc1.top

[S33] C++：vector 增删
来源：http://aze.svipenyu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dxv.guannengcc.top

[S34] C++：遍历 vector
来源：http://osw.jianghu66.top

for (auto &x : v) { std::cout << x; }
来源：http://cay.zdqjudy.top

[S35] C++：map
来源：http://ckk.chenlongwang.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wov.vqdsnc.cn

[S36] C++：unordered_map
来源：http://zai.52xcode.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xiu.jqgufenzy.top

[S37] C++：set
来源：http://jwv.shanyushiyangtech.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kcu.tianlin.xyz

[S38] C++：排序
来源：http://fvf.gogol.net.cn

std::sort(v.begin(), v.end());
来源：http://ahb.jqgfzy.top

[S39] C++：自定义比较器排序
来源：http://fqx.yangfankeji.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gcw.cqqwz.cn

[S40] C++：查找元素
来源：http://lnw.feifeiyinyue.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bwg.sxryk.cn

[S41] C++：类与构造函数
来源：http://nrw.dashuyun.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hbz.hywenlv.cn

[S42] C++：继承与虚函数
来源：http://mgc.jianghu66.top

class B : public Base { public: void f() override {} };
来源：http://xrp.uphjek.com

[S43] C++：智能指针
来源：http://sth.fehbvm.com

auto p = std::make_unique<int>(5);
来源：http://wne.jqgufenzy.top

[S44] C++：引用传参
来源：http://pgv.cucudq.cn

void inc(int &x) { ++x; }
来源：http://hxd.fengsongda.top

[S45] C++：lambda
来源：http://lbe.vehdjk.com

auto add = [](int a, int b) { return a + b; };
来源：http://joe.xziqi.cn

[S46] C++：函数模板
来源：http://bjg.daxiang520.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ilp.pycfn.com

[S47] C++：结构化绑定遍历
来源：http://ior.yj202588.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kor.c1oappe.top

[S48] C++：逐行读文件
来源：http://ojc.xingfuxueyuan.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://cbp.jqgufenzy.top

while (std::getline(in, line)) { }
来源：http://vyw.hysaishi.cn

[S49] C++：写文件
来源：http://ozl.xingfuxueyuan.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ftf.yongpay.top

[S50] C++：格式化数字
来源：http://vfq.shanyushiyangtech.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pvo.shanyushiyangkeji.top

[S51] C++：显式类型转换
来源：http://isq.jinqigfzy.top

static_cast<double>(a) / b
来源：http://swp.sjlbkw.cn

[S52] C++：const 与 noexcept
来源：http://gxh.andypj.xyz

int size() const noexcept { return n_; }
来源：http://vwn.xuanzx.com

[S53] C++：移动语义
来源：http://cod.cdnleiting.top

std::vector<int> w = std::move(v);
来源：http://qex.vqdsnc.cn

[S54] C++：异常处理
来源：http://was.yj202588.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hdh.hesvh.cn

[S55] C++：结构化绑定
来源：http://ptz.yj20258888.top

auto [a, b] = std::make_pair(1, 2);
来源：http://uik.gogol.net.cn

[S56] C++：optional
来源：http://ehk.yfazqb.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fpn.yfazqb.com

[S57] C++：编译期常量
来源：http://ljp.xuanzx.com

constexpr int N = 10;
来源：http://bpk.jqgufenzy.top

[S58] C++：命名空间
来源：http://hvo.hnxiangtu.top

namespace ns { int f() { return 1; } }
来源：http://lwi.fengsongda.top

[S59] C++：静态断言
来源：http://kbu.sjlbkw.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bup.dianchejie.cn

[S60] C++：遍历并删除元素
来源：http://ift.hongshengwenyu.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://oec.cqqwz.cn

================================================================================
来源：http://chg.yj20258888.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zuu.cheryme.top

================================================================================
来源：http://aud.nanxinkj.top

[T01] Kotlin：Hello World
来源：http://iou.guowangkeji.top

println("Hello")
来源：http://edn.shanyushiyangkeji.top

[T02] Kotlin：变量
来源：http://avl.xziqi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nle.ydjk.org.cn

[T03] Kotlin：字符串模板
来源：http://unv.shangyingyoupin.top

"值: $b"
来源：http://wdw.52xcode.cn

[T04] Kotlin：空安全
来源：http://nwq.jyoumei.cn

val n: String? = null;  n?.length
来源：http://utt.haohaochexian.top

[T05] Kotlin：when 表达式
来源：http://mfc.zhijiandao.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://suk.cucudq.cn

[T06] Kotlin：集合映射
来源：http://jml.yj20258888.top

listOf(1, 2, 3).map { it * 2 }
来源：http://lgq.gogol.net.cn

[T07] Kotlin：集合过滤
来源：http://ktd.fzhhl.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://kmu.gzhubu.top

[T08] Kotlin：数据类
来源：http://och.zhixingplan.top

data class User(val name: String, val age: Int)
来源：http://vsi.hongshengwenyu.top

[T09] Kotlin：扩展函数
来源：http://hsy.hesvh.cn

fun String.exclaim() = this + "!"
来源：http://lof.yueranfly.top

[T10] Kotlin：默认参数
来源：http://jar.tianlin.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://xss.cashguo.top

[T11] Kotlin：协程
来源：http://wqw.vehdjk.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://uwo.fktsv.cn

[T12] Kotlin：解构声明
来源：http://omb.daria6918.cn

val (a, b) = Pair(1, 2)
来源：http://rkl.tianlin.xyz

[T13] Kotlin：只读 Map
来源：http://srp.chenjidiqi.icu

val m = mapOf("a" to 1)
来源：http://ita.cashguo.top

[T14] Kotlin：循环
来源：http://bdn.xingfuxueyuan.xyz

for (i in 1..10) println(i)
来源：http://toe.jinyuanbaomall.cn

[T15] Kotlin：接口
来源：http://zkj.chenjidiqi.icu

interface Shape { fun area(): Double }
来源：http://vaj.aizwys.cn

[T16] Swift：Hello World
来源：http://zhn.cqqwz.cn

print("Hello")
来源：http://tvd.hysaishi.cn

[T17] Swift：变量与常量
来源：http://ces.quarkkingdee.top

var a = 1;  let b = 2
来源：http://wng.jlsjyb.cn

[T18] Swift：字符串插值
来源：http://ish.hongshengwenyu.top

"值: \(b)"
来源：http://mwm.shzxlz.cn

[T19] Swift：可选绑定
来源：http://yqv.fanxiaobao.xyz

if let n = opt { print(n) }
来源：http://gdp.iojbl.cn

[T20] Swift：数组操作
来源：http://zsp.shzxlz.cn

var a = [1, 2, 3];  a.append(4)
来源：http://vmu.nanxinkj.top

[T21] Swift：遍历
来源：http://icn.hywenlv.cn

for x in a { print(x) }
来源：http://cag.sxryk.cn

[T22] Swift：字典
来源：http://fch.aibaodan.cn

var d = ["a": 1];  d["b"] = 2
来源：http://wdm.shangyingyoupin.top

[T23] Swift：函数
来源：http://nyg.hnxiangtu.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tup.hnqzz.top

[T24] Swift：闭包
来源：http://bod.xingfuxueyuan.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://xrb.quarkkingdee.top

[T25] Swift：结构体
来源：http://nhq.pycfn.com

struct P { var x: Int }
来源：http://ckh.xingfuxueyuan.xyz

[T26] Swift：类与重写
来源：http://klu.jlsjyb.cn

class A: Base { override func f() {} }
来源：http://qxc.yj20258888.top

[T27] Swift：错误处理
来源：http://jem.haohaochexian.top

do { try f() } catch { print(error) }
来源：http://xst.ehwqpu.com

[T28] Swift：枚举
来源：http://rfa.tianlin.xyz

enum Color { case red, green }
来源：http://ozt.zdbjq.cn

[T29] Swift：guard 提前返回
来源：http://app.guowangkeji.top

guard let x = opt else { return }
来源：http://lxl.hywenlv.cn

[T30] Swift：协议
来源：http://nkb.daria6918.cn

protocol Shape { func area() -> Double }
来源：http://lfc.ydzc1.top

[T31] Lua：Hello World
来源：http://fig.epnwcf.com

print("Hello")
来源：http://var.bjfxy.top

[T32] Lua：局部变量
来源：http://psx.gzhubu.top

local a = 1
来源：http://crd.xylfe.cn

[T33] Lua：表（数组）
来源：http://nje.vehdjk.com

local t = {1, 2, 3};  t[4] = 4
来源：http://adb.cucudq.cn

[T34] Lua：遍历表
来源：http://lmx.nanxinkj.top

for i, v in ipairs(t) do print(i, v) end
来源：http://gsa.yuxming.cn

[T35] Lua：字典表
来源：http://nsw.fengsongda.top

local d = { a = 1 };  d.b = 2
来源：http://fzb.nanxuanxn.top

[T36] Lua：函数
来源：http://voo.sjlbkw.cn

function add(a, b) return a + b end
来源：http://nyy.gogol.net.cn

[T37] Lua：字符串拼接
来源：http://lge.zhiwuduotai.top

"a" .. "b"
来源：http://uzb.vqdsnc.cn

[T38] Lua：条件
来源：http://ppb.aibaodan.cn

if x > 0 then print("正") end
来源：http://mbr.yfazqb.com

[T39] Lua：模式匹配
来源：http://ahw.meibo888.top

string.find(s, "%d+")
来源：http://aag.chenlongwang.top

[T40] Lua：元表
来源：http://rzi.yonumen.top

setmetatable({}, { __index = base })
来源：http://tkc.jlsjyb.cn

[T41] Perl：Hello World
来源：http://psj.jinqigfzy.top

print "Hello\n";
来源：http://gat.chenjidiqi.icu

[T42] Perl：变量类型
来源：http://kzu.iojbl.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ajm.jyoumei.cn

[T43] Perl：字符串插值
来源：http://pac.cashguo.top

"值: $a"
来源：http://elg.xuetiantiany.cn

[T44] Perl：条件
来源：http://gpq.yuanzhike.top

if ($a > 0) { print "正"; }
来源：http://szw.pycfn.com

[T45] Perl：数组遍历
来源：http://ihp.hywenlv.cn

for my $x (@arr) { print $x; }
来源：http://eqz.feifeiyinyue.top

[T46] Perl：哈希操作
来源：http://fho.jyoumei.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bzu.feifeiyinyue.top

[T47] Perl：正则捕获
来源：http://zzx.yfazqb.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://aih.xuetiantiany.cn

[T48] Perl：正则替换
来源：http://nxy.zhijiandao.cn

$s =~ s/old/new/g;
来源：http://kbs.kuanghao11.cn

[T49] Perl：函数
来源：http://gqq.kuanghao11.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wyf.shuidangran.top

[T50] Perl：逐行读文件
来源：http://kvd.smart0.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://aqj.yvedp.cn

while (my $line = <$fh>) { print $line; }
来源：http://ewd.pengpengdd.cyou

[T51] Scala：Hello World
来源：http://hal.ctjpmb.com

println("Hello")
来源：http://qej.aizwys.cn

[T52] Scala：变量
来源：http://lew.yuxming.cn

val a = 1;  var b = 2
来源：http://wle.chenlongwang.top

[T53] Scala：字符串插值
来源：http://kwd.uphjek.com

s"值: $b"
来源：http://eqd.snrcjt.cn

[T54] Scala：集合映射
来源：http://edf.9152youxi.cn

List(1, 2, 3).map(_ * 2)
来源：http://gqz.aibaodan.cn

[T55] Scala：集合过滤
来源：http://gcs.ppjwa.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qae.ehwqpu.com

[T56] Scala：样例类
来源：http://dcu.ivvv.top

case class User(name: String, age: Int)
来源：http://xcg.gaohongyu789.top

[T57] Scala：模式匹配
来源：http://xqd.gaohongyu789.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://tfr.pengpengdd.cyou

[T58] Scala：函数定义
来源：http://osv.feifeiyinyue.top

def add(a: Int, b: Int): Int = a + b
来源：http://occ.cashguo.top

[T59] Scala：循环
来源：http://czr.daxiang520.top

for (i <- 1 to 10) println(i)
来源：http://zml.ybcxt.top

[T60] Scala：折叠
来源：http://fzu.guannengcc.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gav.hfpthk.cn

================================================================================
来源：http://stp.nanxuanxn.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zqz.snrcjt.cn

================================================================================
来源：http://yko.jianghu66.top

[U01] Py：创建虚拟环境
来源：http://yjg.feifeiyinyue.top

python -m venv .venv && source .venv/bin/activate
来源：http://vyf.jlsjyb.cn

[U02] Py：导出 / 安装依赖
来源：http://evy.316326.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wrm.yj20258888.top

[U03] Py：加载 .env 配置
来源：http://azp.ehwqpu.com

from dotenv import load_dotenv; load_dotenv()
来源：http://xtv.ydzc1.top

[U04] Py：变量调试打印
来源：http://pxr.andypj.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lid.xuetiantiany.cn

[U05] Py：列表去重且保序
来源：http://jcc.jiagoushi.top

list(dict.fromkeys(arr))
来源：http://plp.bjfxy.top

[U06] Py：合并两个字典
来源：http://ucy.zhiwuduotai.top

{**a, **b}
来源：http://cpm.pengpengdd.cyou

[U07] Py：反转字典键值
来源：http://qwr.chenjidiqi.icu

{v: k for k, v in d.items()}
来源：http://srm.fktsv.cn

[U08] Py：展平二维列表
来源：http://tav.hfpthk.cn

[y for x in nested for y in x]
来源：http://qpy.jinqigfzy.top

[U09] Py：字典取最大值的键
来源：http://kwy.yfazqb.com

max(d, key=d.get)
来源：http://hqp.sysykeji.top

[U10] Py：按值排序字典
来源：http://rye.bjfxy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kdx.snrcjt.cn

[U11] Py：生成器表达式
来源：http://yjb.tarul.cn

(x * 2 for x in arr)
来源：http://sdq.xziqi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://tpc.pengpengdd.cyou

Counter(arr).most_common(3)
来源：http://get.yj20258888.top

[U13] Py：固定长度队列
来源：http://uzg.hongshengwenyu.top

deque(maxlen=10)
来源：http://eoq.hesvh.cn

[U14] Py：分组收集到列表
来源：http://sou.iojbl.cn

defaultdict(list)
来源：http://xts.yanxiufei.cn

[U15] Py：高精度计时
来源：http://suy.shanyushiyangtech.top

t = time.perf_counter()
来源：http://ezj.yuxming.cn

[U16] Py：命令行参数解析
来源：http://uss.0kj1m.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vnj.andypj.xyz

[U17] Py：初始化日志
来源：http://hqx.dashuyun.cn

logging.basicConfig(level=logging.INFO)
来源：http://buf.ydjk.org.cn

[U18] Py：预编译正则
来源：http://bpq.hnqzz.top

pat = re.compile(r"\d+")
来源：http://szc.hfpthk.cn

[U19] Py：正则替换带回调
来源：http://prx.ivvv.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zyz.quarkkingdee.top

[U20] Py：缓存函数结果
来源：http://qpg.ydjk.org.cn

@functools.lru_cache(maxsize=None)
来源：http://bop.chenzaomai.com

[U21] Py：自定义上下文管理器
来源：http://oxj.vehdjk.com

@contextlib.contextmanager
来源：http://cfn.quarkkingdee.top

[U22] Py：矩阵转置
来源：http://hqz.xziqi.cn

list(zip(*m))
来源：http://biv.nanxinkj.top

[U23] Py：分块读取大文件
来源：http://lch.tianlin.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tfv.jqgfzy.top

[U24] Py：路径操作
来源：http://mma.daxiang520.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lux.yongpay.top

[U25] Py：CSV 按字典读
来源：http://jnj.ivvv.top

csv.DictReader(f)
来源：http://zzu.vqdsnc.cn

[U26] Py：并发下载
来源：http://uvb.cashguo.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wgr.zdqjudy.top

[U27] Py：异步 HTTP
来源：http://kkv.aizwys.cn

aiohttp.ClientSession() 配合 async with
来源：http://ijf.jinyuanbaomall.cn

[U28] Py：类型别名
来源：http://uko.guowangkeji.top

UserId = int
来源：http://yfs.yanxiufei.cn

[U29] Py：属性校验
来源：http://zfw.tian-w.cn

@property 与 @x.setter 配合
来源：http://gow.gotoacloud.top

[U30] Py：数据类
来源：http://pkh.jianghu66.top

@dataclass(slots=True)
来源：http://tor.fzhhl.top

[U31] Py：单测
来源：http://tmw.zycfv.cn

python -m pytest -q
来源：http://dxb.ivvv.top

[U32] Py：代码格式化
来源：http://mxu.gaohongyu789.top

ruff format . && ruff check --fix .
来源：http://ddr.cheryme.top

[U33] Py：打包发布
来源：http://niq.tanke756.top

python -m build  （依赖 pyproject.toml）
来源：http://rol.zdbjq.cn

[U34] Py：判断编码
来源：http://lwz.ppjwa.cn

chardet.detect(raw)
来源：http://qmz.haohaochexian.top

[U35] Py：发送邮件
来源：http://jgx.jinqigufen.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pvv.jlsjyb.cn

[U36] Py：定时任务
来源：http://pxd.yuxming.cn

schedule.every(10).minutes.do(job)
来源：http://yhb.cheryme.top

[U37] Py：读写 Excel
来源：http://qqb.yuanzhike.top

pandas.read_excel / DataFrame.to_excel
来源：http://ntt.pycfn.com

[U38] Py：获取脚本所在目录
来源：http://bqr.jinqigufen.top

Path(__file__).resolve().parent
来源：http://vwv.zdqjudy.top

[U39] Py：判断是否在交互环境
来源：http://tbn.pycfn.com

sys.stdout.isatty()
来源：http://zyw.c1oappe.top

[U40] Py：打印到标准错误
来源：http://ltc.pengpengdd.cyou

print("err", file=sys.stderr)
来源：http://fou.gaohongyu789.top

[U41] PHP：初始化 Composer 项目
来源：http://nkn.shzxlz.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://cpd.guannengcc.top

[U42] PHP：PSR-4 自动加载
来源：http://ove.zhengqikj.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://iag.aizwys.cn

[U43] PHP：声明命名空间
来源：http://mon.zhoulong.xyz

namespace App\Http;
来源：http://hgb.yj20258888.top

[U44] PHP：开启严格类型
来源：http://mcs.ydjk.org.cn

declare(strict_types=1);
来源：http://uks.redwolf501.top

[U45] PHP：类型声明与返回类型
来源：http://mtd.yuxming.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://rzq.epnwcf.com

[U46] PHP：可空类型
来源：http://vkm.mhx1999.top

?string $name = null
来源：http://hsq.zhengqikj.top

[U47] PHP：联合类型
来源：http://zkx.aizwys.cn

int|string $id
来源：http://jrs.zhiwuduotai.top

[U48] PHP：纯枚举
来源：http://jrw.ctjpmb.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zac.ybcxt.top

[U49] PHP：只读属性
来源：http://qah.ybcxt.top

public readonly string $name
来源：http://ysn.pycfn.com

[U50] PHP：构造器属性提升
来源：http://rxa.sufxvd.cn

public function __construct(private int $id) {}
来源：http://jyz.gzhubu.top

[U51] PHP：数组解构
来源：http://tck.cheryme.top

[$a, $b] = $arr;
来源：http://kcb.ivvv.top

[U52] PHP：箭头函数
来源：http://gun.zhengqikj.top

$double = fn($x) => $x * 2;
来源：http://adw.quarkkingdee.top

[U53] PHP：空合并运算符
来源：http://qcw.316326.xyz

$v = $a ?? $b ?? "default";
来源：http://foe.yueranfly.top

[U54] PHP：空安全调用
来源：http://eks.sxryk.cn

$obj?->method()
来源：http://okg.ctjpmb.com


<!-- 参考信息 -->