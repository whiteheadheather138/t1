代发 wailian999

#include <iostream>
来源：http://ygt.yonumen.top

int main() { std::cout << "Hello\n"; }
来源：http://vty.snrcjt.cn

[S32] C++：字符串
来源：http://mph.ybcxt.top

std::string s = "hi";  s += "!";
来源：http://bty.svipenyu.cn

[S33] C++：vector 增删
来源：http://rlg.fengsongda.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rid.zhengqikj.top

[S34] C++：遍历 vector
来源：http://kni.tianlin.xyz

for (auto &x : v) { std::cout << x; }
来源：http://lqb.pengpengdd.cyou

[S35] C++：map
来源：http://dqm.yj20258888.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xru.xinyue.icu

[S36] C++：unordered_map
来源：http://ajz.aibaodan.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qgs.nanxinkj.top

[S37] C++：set
来源：http://ght.xziqi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://amz.9152youxi.cn

[S38] C++：排序
来源：http://otn.jiagoushi.top

std::sort(v.begin(), v.end());
来源：http://bvl.fehbvm.com

[S39] C++：自定义比较器排序
来源：http://zzn.sxryk.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ham.fzhhl.top

[S40] C++：查找元素
来源：http://sly.fzhhl.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://usm.yj20258888.top

[S41] C++：类与构造函数
来源：http://crk.zhijiandao.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ulb.cdnleiting.top

[S42] C++：继承与虚函数
来源：http://ndr.cashguo.top

class B : public Base { public: void f() override {} };
来源：http://thq.sweek.top

[S43] C++：智能指针
来源：http://xvc.gotoacloud.top

auto p = std::make_unique<int>(5);
来源：http://dqt.yonumen.top

[S44] C++：引用传参
来源：http://hul.quarkkingdee.top

void inc(int &x) { ++x; }
来源：http://uad.chenlongwang.top

[S45] C++：lambda
来源：http://qff.cheryme.top

auto add = [](int a, int b) { return a + b; };
来源：http://uar.hcnkem.com

[S46] C++：函数模板
来源：http://fye.yj20258.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://euj.yangfankeji.com

[S47] C++：结构化绑定遍历
来源：http://fat.zhengqikj.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zqh.sxryk.cn

[S48] C++：逐行读文件
来源：http://cdh.sxryk.cn

std::ifstream in("a.txt");  std::string line;
来源：http://whm.chenlongwang.top

while (std::getline(in, line)) { }
来源：http://kcd.yongpay.top

[S49] C++：写文件
来源：http://zga.hnxiangtu.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ovs.hnqzz.top

[S50] C++：格式化数字
来源：http://ity.ppjwa.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cox.yueranfly.top

[S51] C++：显式类型转换
来源：http://joz.hammf.cn

static_cast<double>(a) / b
来源：http://nvx.cdnleiting.top

[S52] C++：const 与 noexcept
来源：http://pxn.vqdsnc.cn

int size() const noexcept { return n_; }
来源：http://guf.daxiang520.top

[S53] C++：移动语义
来源：http://uoq.andypj.xyz

std::vector<int> w = std::move(v);
来源：http://mnv.fanxiaobao.xyz

[S54] C++：异常处理
来源：http://xoo.tarul.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pxo.meibo888.top

[S55] C++：结构化绑定
来源：http://mvx.svipenyu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://mtu.shzxlz.cn

[S56] C++：optional
来源：http://akm.hnqzz.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mkt.shuidangran.top

[S57] C++：编译期常量
来源：http://hqo.gotoacloud.top

constexpr int N = 10;
来源：http://ctx.ctjpmb.com

[S58] C++：命名空间
来源：http://ahu.zhiwuduotai.top

namespace ns { int f() { return 1; } }
来源：http://evq.zdqjudy.top

[S59] C++：静态断言
来源：http://szt.ivvv.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://sxx.hywenlv.cn

[S60] C++：遍历并删除元素
来源：http://poi.yvedp.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lbg.9152youxi.cn

================================================================================
来源：http://xnx.fzhhl.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pnt.ehwqpu.com

================================================================================
来源：http://cma.ctjpmb.com

[T01] Kotlin：Hello World
来源：http://bsr.shangyingyoupin.top

println("Hello")
来源：http://lan.cucudq.cn

[T02] Kotlin：变量
来源：http://ysu.yuxming.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yjh.hesvh.cn

[T03] Kotlin：字符串模板
来源：http://ytb.uphjek.com

"值: $b"
来源：http://ojf.svipenyu.cn

[T04] Kotlin：空安全
来源：http://kbd.ivvv.top

val n: String? = null;  n?.length
来源：http://czd.ctjpmb.com

[T05] Kotlin：when 表达式
来源：http://fpb.hnqzz.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xwi.shanyushiyangkeji.top

[T06] Kotlin：集合映射
来源：http://dpt.wangshuangyany.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://oyt.yj20258.top

[T07] Kotlin：集合过滤
来源：http://mpe.yj20258.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://mjc.jinyuanbaomall.cn

[T08] Kotlin：数据类
来源：http://cgr.iojbl.cn

data class User(val name: String, val age: Int)
来源：http://oog.yj20258888.top

[T09] Kotlin：扩展函数
来源：http://hcu.nanxinkj.top

fun String.exclaim() = this + "!"
来源：http://itu.hysaishi.cn

[T10] Kotlin：默认参数
来源：http://drb.gogol.net.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://bdj.ehwqpu.com

[T11] Kotlin：协程
来源：http://xrs.jyoumei.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://agq.fktsv.cn

[T12] Kotlin：解构声明
来源：http://jjs.wangdashe.top

val (a, b) = Pair(1, 2)
来源：http://ccd.zhiwuduotai.top

[T13] Kotlin：只读 Map
来源：http://mmi.hfpthk.cn

val m = mapOf("a" to 1)
来源：http://ndl.birdmap.top

[T14] Kotlin：循环
来源：http://wdo.52xcode.cn

for (i in 1..10) println(i)
来源：http://hao.chenzaomai.com

[T15] Kotlin：接口
来源：http://unl.havefunace.top

interface Shape { fun area(): Double }
来源：http://ksi.jlsjyb.cn

[T16] Swift：Hello World
来源：http://slk.jianghu66.top

print("Hello")
来源：http://poy.yuxming.cn

[T17] Swift：变量与常量
来源：http://fbq.havefunace.top

var a = 1;  let b = 2
来源：http://bwu.bjfxy.top

[T18] Swift：字符串插值
来源：http://wqw.pycfn.com

"值: \(b)"
来源：http://fed.epnwcf.com

[T19] Swift：可选绑定
来源：http://jdi.hnxiangtu.top

if let n = opt { print(n) }
来源：http://djh.xziqi.cn

[T20] Swift：数组操作
来源：http://wld.shanyushiyangkeji.top

var a = [1, 2, 3];  a.append(4)
来源：http://knq.shuidangran.top

[T21] Swift：遍历
来源：http://zmk.ehwqpu.com

for x in a { print(x) }
来源：http://had.redwolf501.top

[T22] Swift：字典
来源：http://ctw.ppjwa.cn

var d = ["a": 1];  d["b"] = 2
来源：http://wcj.meibo888.top

[T23] Swift：函数
来源：http://dps.wangshuangyany.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://emp.sufxvd.cn

[T24] Swift：闭包
来源：http://bea.birdmap.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://iek.ybcxt.top

[T25] Swift：结构体
来源：http://nse.jqgufenzy.top

struct P { var x: Int }
来源：http://yyx.yuanzhike.top

[T26] Swift：类与重写
来源：http://drv.cheryme.top

class A: Base { override func f() {} }
来源：http://ywt.hesvh.cn

[T27] Swift：错误处理
来源：http://hzf.snrcjt.cn

do { try f() } catch { print(error) }
来源：http://aal.nanxinkj.top

[T28] Swift：枚举
来源：http://yvp.bbcook.cn

enum Color { case red, green }
来源：http://dlm.sysykeji.top

[T29] Swift：guard 提前返回
来源：http://pxq.jyoumei.cn

guard let x = opt else { return }
来源：http://ssu.ivvv.top

[T30] Swift：协议
来源：http://xah.hammf.cn

protocol Shape { func area() -> Double }
来源：http://uxz.tianlin.xyz

[T31] Lua：Hello World
来源：http://ulh.yueranfly.top

print("Hello")
来源：http://iiw.pengpengdd.cyou

[T32] Lua：局部变量
来源：http://qwt.wangdashe.top

local a = 1
来源：http://hrg.ywan-chungtsiang.top

[T33] Lua：表（数组）
来源：http://vus.gotoacloud.top

local t = {1, 2, 3};  t[4] = 4
来源：http://dcp.yuxming.cn

[T34] Lua：遍历表
来源：http://npr.fehbvm.com

for i, v in ipairs(t) do print(i, v) end
来源：http://xqk.havefunace.top

[T35] Lua：字典表
来源：http://yba.yonumen.top

local d = { a = 1 };  d.b = 2
来源：http://vzr.xziqi.cn

[T36] Lua：函数
来源：http://iip.c1oappe.top

function add(a, b) return a + b end
来源：http://gum.guannengcc.top

[T37] Lua：字符串拼接
来源：http://ccd.bjfxy.top

"a" .. "b"
来源：http://jwu.pengpengdd.cyou

[T38] Lua：条件
来源：http://haz.jinyuanbaomall.cn

if x > 0 then print("正") end
来源：http://vcr.svipenyu.cn

[T39] Lua：模式匹配
来源：http://zfi.kuanghao11.cn

string.find(s, "%d+")
来源：http://cnh.316326.xyz

[T40] Lua：元表
来源：http://lkg.chenlongwang.top

setmetatable({}, { __index = base })
来源：http://eee.shangyingyoupin.top

[T41] Perl：Hello World
来源：http://esy.ivvv.top

print "Hello\n";
来源：http://csz.nanxuanxn.top

[T42] Perl：变量类型
来源：http://awr.ivvv.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jds.shanyushiyangkeji.top

[T43] Perl：字符串插值
来源：http://mbj.gzhubu.top

"值: $a"
来源：http://wek.tianlin.xyz

[T44] Perl：条件
来源：http://kzy.hfpthk.cn

if ($a > 0) { print "正"; }
来源：http://cnf.jiagoushi.top

[T45] Perl：数组遍历
来源：http://cuz.zhongyouzk.top

for my $x (@arr) { print $x; }
来源：http://hdz.jqgufenzy.top

[T46] Perl：哈希操作
来源：http://ypz.epnwcf.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qms.daria6918.cn

[T47] Perl：正则捕获
来源：http://rhj.fehbvm.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://fuj.dashuyun.cn

[T48] Perl：正则替换
来源：http://hho.daxiang520.top

$s =~ s/old/new/g;
来源：http://she.svipenyu.cn

[T49] Perl：函数
来源：http://bfl.chenzaomai.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://akf.ehwqpu.com

[T50] Perl：逐行读文件
来源：http://cgk.jlsjyb.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://iwf.tarul.cn

while (my $line = <$fh>) { print $line; }
来源：http://axc.chenjidiqi.icu

[T51] Scala：Hello World
来源：http://sjb.aizwys.cn

println("Hello")
来源：http://ymd.jinqigufen.top

[T52] Scala：变量
来源：http://biu.cucudq.cn

val a = 1;  var b = 2
来源：http://ipw.vqdsnc.cn

[T53] Scala：字符串插值
来源：http://xlp.dashuyun.cn

s"值: $b"
来源：http://owq.zhixingplan.top

[T54] Scala：集合映射
来源：http://yzq.sjlbkw.cn

List(1, 2, 3).map(_ * 2)
来源：http://cvp.wangshuangyany.cn

[T55] Scala：集合过滤
来源：http://dyd.sjlbkw.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xcw.ctjpmb.com

[T56] Scala：样例类
来源：http://poj.dashuyun.cn

case class User(name: String, age: Int)
来源：http://dzw.gogol.net.cn

[T57] Scala：模式匹配
来源：http://lmn.dashuyun.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://kqw.fktsv.cn

[T58] Scala：函数定义
来源：http://nza.smart0.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://pxm.nanxuanxn.top

[T59] Scala：循环
来源：http://ulz.havefunace.top

for (i <- 1 to 10) println(i)
来源：http://krl.ywan-chungtsiang.top

[T60] Scala：折叠
来源：http://mne.guowangkeji.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hyf.pycfn.com

================================================================================
来源：http://jfx.gotoacloud.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://goa.9152youxi.cn

================================================================================
来源：http://nkp.jqgufenzy.top

[U01] Py：创建虚拟环境
来源：http://cpd.birdmap.top

python -m venv .venv && source .venv/bin/activate
来源：http://acx.zdqjudy.top

[U02] Py：导出 / 安装依赖
来源：http://zvf.zhoulong.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zvu.hammf.cn

[U03] Py：加载 .env 配置
来源：http://enu.hnxiangtu.top

from dotenv import load_dotenv; load_dotenv()
来源：http://bml.sjlbkw.cn

[U04] Py：变量调试打印
来源：http://kle.ivvv.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://aor.ydzc1.top

[U05] Py：列表去重且保序
来源：http://zox.hnqzz.top

list(dict.fromkeys(arr))
来源：http://qmo.yvedp.cn

[U06] Py：合并两个字典
来源：http://clc.nwbrower.top

{**a, **b}
来源：http://vxk.haohaochexian.top

[U07] Py：反转字典键值
来源：http://hgm.mhx1999.top

{v: k for k, v in d.items()}
来源：http://cix.kuanghao11.cn

[U08] Py：展平二维列表
来源：http://jom.316326.xyz

[y for x in nested for y in x]
来源：http://lgl.pengpengdd.cyou

[U09] Py：字典取最大值的键
来源：http://mgi.zycfv.cn

max(d, key=d.get)
来源：http://jjo.pycfn.com

[U10] Py：按值排序字典
来源：http://rjk.yfazqb.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jzp.fehbvm.com

[U11] Py：生成器表达式
来源：http://boo.shuidangran.top

(x * 2 for x in arr)
来源：http://mns.yvedp.cn

[U12] Py：取出现最多的 3 个元素
来源：http://phc.hysaishi.cn

Counter(arr).most_common(3)
来源：http://bsm.tarul.cn

[U13] Py：固定长度队列
来源：http://aki.feifeiyinyue.top

deque(maxlen=10)
来源：http://xyj.fanxiaobao.xyz

[U14] Py：分组收集到列表
来源：http://upd.jlsjyb.cn

defaultdict(list)
来源：http://qvd.guannengcc.top

[U15] Py：高精度计时
来源：http://zhh.yueranfly.top

t = time.perf_counter()
来源：http://bhr.sjlbkw.cn

[U16] Py：命令行参数解析
来源：http://jlc.pengpengdd.cyou

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xmu.52xcode.cn

[U17] Py：初始化日志
来源：http://igg.yfazqb.com

logging.basicConfig(level=logging.INFO)
来源：http://nur.hysaishi.cn

[U18] Py：预编译正则
来源：http://ewx.hnqzz.top

pat = re.compile(r"\d+")
来源：http://imk.yueranfly.top

[U19] Py：正则替换带回调
来源：http://jfz.yj20258888.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vdq.kuanghao11.cn

[U20] Py：缓存函数结果
来源：http://elj.epnwcf.com

@functools.lru_cache(maxsize=None)
来源：http://rld.sweek.top

[U21] Py：自定义上下文管理器
来源：http://bho.zdbjq.cn

@contextlib.contextmanager
来源：http://fwx.nanxuanxn.top

[U22] Py：矩阵转置
来源：http://jwy.jinqigufen.top

list(zip(*m))
来源：http://cze.jyoumei.cn

[U23] Py：分块读取大文件
来源：http://bdo.svipenyu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://prq.yuanzhike.top

[U24] Py：路径操作
来源：http://bss.aibaodan.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://irv.pycfn.com

[U25] Py：CSV 按字典读
来源：http://cmv.snrcjt.cn

csv.DictReader(f)
来源：http://ofz.tarul.cn

[U26] Py：并发下载
来源：http://jph.daria6918.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xbf.hesvh.cn

[U27] Py：异步 HTTP
来源：http://bdn.iojbl.cn

aiohttp.ClientSession() 配合 async with
来源：http://jsy.sweek.top

[U28] Py：类型别名
来源：http://yvv.hfpthk.cn

UserId = int
来源：http://tke.ybcxt.top

[U29] Py：属性校验
来源：http://dab.gaohongyu789.top

@property 与 @x.setter 配合
来源：http://ndm.yongpay.top

[U30] Py：数据类
来源：http://evp.ywan-chungtsiang.top

@dataclass(slots=True)
来源：http://hnl.uphjek.com

[U31] Py：单测
来源：http://pwu.jqgfzy.top

python -m pytest -q
来源：http://vgk.zhixingplan.top

[U32] Py：代码格式化
来源：http://gic.ybcxt.top

ruff format . && ruff check --fix .
来源：http://qgf.xingfuxueyuan.xyz

[U33] Py：打包发布
来源：http://pfq.xylfe.cn

python -m build  （依赖 pyproject.toml）
来源：http://rdn.xuanzx.com

[U34] Py：判断编码
来源：http://hot.dashuyun.cn

chardet.detect(raw)
来源：http://cmr.fanxiaobao.xyz

[U35] Py：发送邮件
来源：http://ajk.zhiwuduotai.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hdg.hnxiangtu.top

[U36] Py：定时任务
来源：http://thl.yj20258.top

schedule.every(10).minutes.do(job)
来源：http://vsf.nanxuanxn.top

[U37] Py：读写 Excel
来源：http://enu.zdqjudy.top

pandas.read_excel / DataFrame.to_excel
来源：http://gfj.iojbl.cn

[U38] Py：获取脚本所在目录
来源：http://kpg.jqgfzy.top

Path(__file__).resolve().parent
来源：http://rec.feifeiyinyue.top

[U39] Py：判断是否在交互环境
来源：http://mwc.wangshuangyany.cn

sys.stdout.isatty()
来源：http://mtk.52xcode.cn

[U40] Py：打印到标准错误
来源：http://hyk.guowangkeji.top

print("err", file=sys.stderr)
来源：http://mgh.vehdjk.com

[U41] PHP：初始化 Composer 项目
来源：http://dox.zhoulong.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://qtt.epnwcf.com

[U42] PHP：PSR-4 自动加载
来源：http://ypj.jinyuanbaomall.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://sac.9152youxi.cn

[U43] PHP：声明命名空间
来源：http://vhd.daxiang520.top

namespace App\Http;
来源：http://xvv.yangfankeji.com

[U44] PHP：开启严格类型
来源：http://edk.jinqigufen.top

declare(strict_types=1);
来源：http://yrd.c1oappe.top

[U45] PHP：类型声明与返回类型
来源：http://imo.andypj.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://znq.cashguo.top

[U46] PHP：可空类型
来源：http://yjd.ivvv.top

?string $name = null
来源：http://jbw.jinqigfzy.top

[U47] PHP：联合类型
来源：http://zbh.wangshuangyany.cn

int|string $id
来源：http://hdi.nanxuanxn.top

[U48] PHP：纯枚举
来源：http://etd.fzhhl.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://euh.hnxiangtu.top

[U49] PHP：只读属性
来源：http://ycg.sysykeji.top

public readonly string $name
来源：http://doy.zycfv.cn

[U50] PHP：构造器属性提升
来源：http://kjr.pengpengdd.cyou

public function __construct(private int $id) {}
来源：http://ovy.yuanzhike.top

[U51] PHP：数组解构
来源：http://sff.shanyushiyangtech.top

[$a, $b] = $arr;
来源：http://fbj.wangdashe.top

[U52] PHP：箭头函数
来源：http://dcf.wangshuangyany.cn

$double = fn($x) => $x * 2;
来源：http://luw.ppjwa.cn

[U53] PHP：空合并运算符
来源：http://lda.zhaomingkeji.xyz

$v = $a ?? $b ?? "default";
来源：http://qms.haohaochexian.top

[U54] PHP：空安全调用
来源：http://kvx.nwbrower.top

$obj?->method()
来源：http://qwk.yongpay.top

[U55] PHP：match 表达式
来源：http://ouy.ehwqpu.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gio.guowangkeji.top

[U56] PHP：命名参数
来源：http://dyu.vqdsnc.cn

f(a: 1, b: 2)
来源：http://ksh.gzhubu.top


<!-- 参考信息 -->