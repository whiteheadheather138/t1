代发 wailian999

#include <iostream>
来源：http://kib.jlsjyb.cn

int main() { std::cout << "Hello\n"; }
来源：http://dct.shzxlz.cn

[S32] C++：字符串
来源：http://ywq.hnqzz.top

std::string s = "hi";  s += "!";
来源：http://nua.yongpay.top

[S33] C++：vector 增删
来源：http://vdt.sweek.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vtd.jlsjyb.cn

[S34] C++：遍历 vector
来源：http://wkk.zdqjudy.top

for (auto &x : v) { std::cout << x; }
来源：http://sxh.jinghuilouyu.cn

[S35] C++：map
来源：http://uyc.hfpthk.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qnj.yuxming.cn

[S36] C++：unordered_map
来源：http://peh.pycfn.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://svj.vqdsnc.cn

[S37] C++：set
来源：http://iet.daxiang520.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://eai.cdnleiting.top

[S38] C++：排序
来源：http://fba.cucudq.cn

std::sort(v.begin(), v.end());
来源：http://egx.shanyushiyangkeji.top

[S39] C++：自定义比较器排序
来源：http://sxe.gotoacloud.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gid.xuetiantiany.cn

[S40] C++：查找元素
来源：http://ria.hnxiangtu.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pjv.tianlin.xyz

[S41] C++：类与构造函数
来源：http://rfj.dianchejie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zai.aizwys.cn

[S42] C++：继承与虚函数
来源：http://ryl.snrcjt.cn

class B : public Base { public: void f() override {} };
来源：http://yyo.pengpengdd.cyou

[S43] C++：智能指针
来源：http://eer.yuxming.cn

auto p = std::make_unique<int>(5);
来源：http://lim.nwbrower.top

[S44] C++：引用传参
来源：http://onr.snrcjt.cn

void inc(int &x) { ++x; }
来源：http://weq.cucudq.cn

[S45] C++：lambda
来源：http://gfw.ydjk.org.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ynf.zdqjudy.top

[S46] C++：函数模板
来源：http://bgt.havefunace.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gss.yj20258.top

[S47] C++：结构化绑定遍历
来源：http://ogj.quarkkingdee.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mwr.hammf.cn

[S48] C++：逐行读文件
来源：http://juo.gotoacloud.top

std::ifstream in("a.txt");  std::string line;
来源：http://fla.bjfxy.top

while (std::getline(in, line)) { }
来源：http://pyl.shzxlz.cn

[S49] C++：写文件
来源：http://apc.xuetiantiany.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ilc.tanke756.top

[S50] C++：格式化数字
来源：http://zie.xinyue.icu

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zxs.pengpengdd.cyou

[S51] C++：显式类型转换
来源：http://ixd.fzhhl.top

static_cast<double>(a) / b
来源：http://jjd.wangshuangyany.cn

[S52] C++：const 与 noexcept
来源：http://dbl.ivvv.top

int size() const noexcept { return n_; }
来源：http://xsc.yj202588.top

[S53] C++：移动语义
来源：http://eix.zhongyouzk.top

std::vector<int> w = std::move(v);
来源：http://qrw.yonumen.top

[S54] C++：异常处理
来源：http://nru.yj202588.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://udw.redwolf501.top

[S55] C++：结构化绑定
来源：http://hlr.yj202588.top

auto [a, b] = std::make_pair(1, 2);
来源：http://pye.yj202588.top

[S56] C++：optional
来源：http://pvi.xuetiantiany.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lqw.havefunace.top

[S57] C++：编译期常量
来源：http://htz.haohaochexian.top

constexpr int N = 10;
来源：http://smg.svipenyu.cn

[S58] C++：命名空间
来源：http://jqk.yuxming.cn

namespace ns { int f() { return 1; } }
来源：http://ioz.haohaochexian.top

[S59] C++：静态断言
来源：http://rxf.nanxuanxn.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hlx.yj20258.top

[S60] C++：遍历并删除元素
来源：http://ywr.jianghu66.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wuw.dashuyun.cn

================================================================================
来源：http://xet.kuanghao11.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xeu.iojbl.cn

================================================================================
来源：http://ecr.xylfe.cn

[T01] Kotlin：Hello World
来源：http://skk.uphjek.com

println("Hello")
来源：http://xht.vqdsnc.cn

[T02] Kotlin：变量
来源：http://poj.feifeiyinyue.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xlq.jqgufenzy.top

[T03] Kotlin：字符串模板
来源：http://vra.shanyushiyangkeji.top

"值: $b"
来源：http://omt.vehdjk.com

[T04] Kotlin：空安全
来源：http://xin.ybcxt.top

val n: String? = null;  n?.length
来源：http://xpx.ywan-chungtsiang.top

[T05] Kotlin：when 表达式
来源：http://fxz.andypj.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nfm.daria6918.cn

[T06] Kotlin：集合映射
来源：http://wgr.xuetiantiany.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://qbe.fzhhl.top

[T07] Kotlin：集合过滤
来源：http://wjh.xuetiantiany.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ync.cucudq.cn

[T08] Kotlin：数据类
来源：http://caw.yvedp.cn

data class User(val name: String, val age: Int)
来源：http://hjn.yvedp.cn

[T09] Kotlin：扩展函数
来源：http://ohe.guannengcc.top

fun String.exclaim() = this + "!"
来源：http://ykt.yongpay.top

[T10] Kotlin：默认参数
来源：http://nru.uphjek.com

fun greet(name: String = "World") = "Hi $name"
来源：http://qga.zhiwuduotai.top

[T11] Kotlin：协程
来源：http://kpd.hongshengwenyu.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://bjk.vqdsnc.cn

[T12] Kotlin：解构声明
来源：http://kzo.sxryk.cn

val (a, b) = Pair(1, 2)
来源：http://tbw.zhixingplan.top

[T13] Kotlin：只读 Map
来源：http://ydb.52xcode.cn

val m = mapOf("a" to 1)
来源：http://sbd.cdnleiting.top

[T14] Kotlin：循环
来源：http://cvw.wangshuangyany.cn

for (i in 1..10) println(i)
来源：http://ftd.nwbrower.top

[T15] Kotlin：接口
来源：http://mcv.yj20258888.top

interface Shape { fun area(): Double }
来源：http://mbe.jiagoushi.top

[T16] Swift：Hello World
来源：http://hvx.epnwcf.com

print("Hello")
来源：http://veu.zycfv.cn

[T17] Swift：变量与常量
来源：http://plk.jyoumei.cn

var a = 1;  let b = 2
来源：http://ibd.mhx1999.top

[T18] Swift：字符串插值
来源：http://utf.chenlongwang.top

"值: \(b)"
来源：http://zkv.yuanzhike.top

[T19] Swift：可选绑定
来源：http://rtg.jianghu66.top

if let n = opt { print(n) }
来源：http://set.sjlbkw.cn

[T20] Swift：数组操作
来源：http://djg.pycfn.com

var a = [1, 2, 3];  a.append(4)
来源：http://vma.aizwys.cn

[T21] Swift：遍历
来源：http://bvr.yanxiufei.cn

for x in a { print(x) }
来源：http://kmd.yangfankeji.com

[T22] Swift：字典
来源：http://rgd.yangfankeji.com

var d = ["a": 1];  d["b"] = 2
来源：http://grn.ydzc1.top

[T23] Swift：函数
来源：http://rnf.shuidangran.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ybf.zhengqikj.top

[T24] Swift：闭包
来源：http://puu.0kj1m.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ulj.sufxvd.cn

[T25] Swift：结构体
来源：http://rvk.birdmap.top

struct P { var x: Int }
来源：http://cfe.xuanzx.com

[T26] Swift：类与重写
来源：http://eps.iojbl.cn

class A: Base { override func f() {} }
来源：http://mmi.tian-w.cn

[T27] Swift：错误处理
来源：http://sno.xuetiantiany.cn

do { try f() } catch { print(error) }
来源：http://hvz.zhongyouzk.top

[T28] Swift：枚举
来源：http://znf.gogol.net.cn

enum Color { case red, green }
来源：http://lwz.yuxming.cn

[T29] Swift：guard 提前返回
来源：http://vfz.ivvv.top

guard let x = opt else { return }
来源：http://src.hfpthk.cn

[T30] Swift：协议
来源：http://zuk.jiagoushi.top

protocol Shape { func area() -> Double }
来源：http://kxd.xylfe.cn

[T31] Lua：Hello World
来源：http://phk.xylfe.cn

print("Hello")
来源：http://jma.zhengqikj.top

[T32] Lua：局部变量
来源：http://hvj.shuidangran.top

local a = 1
来源：http://qsu.zhiwuduotai.top

[T33] Lua：表（数组）
来源：http://kbz.daria6918.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://yey.wangshuangyany.cn

[T34] Lua：遍历表
来源：http://tzs.ppjwa.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://xrt.fzhhl.top

[T35] Lua：字典表
来源：http://vlp.cashguo.top

local d = { a = 1 };  d.b = 2
来源：http://rqr.yuxming.cn

[T36] Lua：函数
来源：http://sws.tarul.cn

function add(a, b) return a + b end
来源：http://xng.birdmap.top

[T37] Lua：字符串拼接
来源：http://tkv.tianlin.xyz

"a" .. "b"
来源：http://plo.sufxvd.cn

[T38] Lua：条件
来源：http://qov.jlsjyb.cn

if x > 0 then print("正") end
来源：http://uiw.yangfankeji.com

[T39] Lua：模式匹配
来源：http://lvs.zhongyouzk.top

string.find(s, "%d+")
来源：http://dyw.tarul.cn

[T40] Lua：元表
来源：http://rpw.sjlbkw.cn

setmetatable({}, { __index = base })
来源：http://afo.xylfe.cn

[T41] Perl：Hello World
来源：http://fyc.hongshengwenyu.top

print "Hello\n";
来源：http://tvv.sysykeji.top

[T42] Perl：变量类型
来源：http://sry.iojbl.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vrl.0kj1m.cn

[T43] Perl：字符串插值
来源：http://fjy.ywan-chungtsiang.top

"值: $a"
来源：http://iwd.ctjpmb.com

[T44] Perl：条件
来源：http://yji.zhixingplan.top

if ($a > 0) { print "正"; }
来源：http://vya.andypj.xyz

[T45] Perl：数组遍历
来源：http://cmp.chenzaomai.com

for my $x (@arr) { print $x; }
来源：http://yui.wangshuangyany.cn

[T46] Perl：哈希操作
来源：http://ffl.jiagoushi.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nxn.tarul.cn

[T47] Perl：正则捕获
来源：http://ezp.sxryk.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://dcz.jinghuilouyu.cn

[T48] Perl：正则替换
来源：http://kkx.tianlin.xyz

$s =~ s/old/new/g;
来源：http://qcb.xziqi.cn

[T49] Perl：函数
来源：http://jiu.zhixingplan.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ozs.sweek.top

[T50] Perl：逐行读文件
来源：http://wda.jiagoushi.top

open my $fh, "<", "a.txt" or die $!;
来源：http://knn.nanxuanxn.top

while (my $line = <$fh>) { print $line; }
来源：http://lry.yongpay.top

[T51] Scala：Hello World
来源：http://tyz.hesvh.cn

println("Hello")
来源：http://mwk.kuanghao11.cn

[T52] Scala：变量
来源：http://xhx.gaohongyu789.top

val a = 1;  var b = 2
来源：http://bnk.yueranfly.top

[T53] Scala：字符串插值
来源：http://qwg.xylfe.cn

s"值: $b"
来源：http://tgj.zhijiandao.cn

[T54] Scala：集合映射
来源：http://edn.zhoulong.xyz

List(1, 2, 3).map(_ * 2)
来源：http://hbe.guowangkeji.top

[T55] Scala：集合过滤
来源：http://pzb.dashuyun.cn

List(1, 2, 3).filter(_ > 1)
来源：http://wkh.nwbrower.top

[T56] Scala：样例类
来源：http://vvs.cashguo.top

case class User(name: String, age: Int)
来源：http://ljl.jqgfzy.top

[T57] Scala：模式匹配
来源：http://xkj.svipenyu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://qyp.hysaishi.cn

[T58] Scala：函数定义
来源：http://ggf.shangyingyoupin.top

def add(a: Int, b: Int): Int = a + b
来源：http://tnm.0kj1m.cn

[T59] Scala：循环
来源：http://mnw.ctjpmb.com

for (i <- 1 to 10) println(i)
来源：http://jbj.hywenlv.cn

[T60] Scala：折叠
来源：http://iqh.smart0.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pdk.jinyuanbaomall.cn

================================================================================
来源：http://kpw.0kj1m.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vzl.hammf.cn

================================================================================
来源：http://rkc.haohaochexian.top

[U01] Py：创建虚拟环境
来源：http://umh.ivvv.top

python -m venv .venv && source .venv/bin/activate
来源：http://zcu.hammf.cn

[U02] Py：导出 / 安装依赖
来源：http://mdc.haohaochexian.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hlb.cheryme.top

[U03] Py：加载 .env 配置
来源：http://hdo.fengsongda.top

from dotenv import load_dotenv; load_dotenv()
来源：http://vbj.gaohongyu789.top

[U04] Py：变量调试打印
来源：http://mbd.ppjwa.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hdu.cucudq.cn

[U05] Py：列表去重且保序
来源：http://zws.dashuyun.cn

list(dict.fromkeys(arr))
来源：http://guc.ydjk.org.cn

[U06] Py：合并两个字典
来源：http://jls.jinqigufen.top

{**a, **b}
来源：http://not.havefunace.top

[U07] Py：反转字典键值
来源：http://mps.snrcjt.cn

{v: k for k, v in d.items()}
来源：http://voe.cdnleiting.top

[U08] Py：展平二维列表
来源：http://fon.tianlin.xyz

[y for x in nested for y in x]
来源：http://gus.xziqi.cn

[U09] Py：字典取最大值的键
来源：http://nzz.jianghu66.top

max(d, key=d.get)
来源：http://tqx.nanxinkj.top

[U10] Py：按值排序字典
来源：http://hko.guannengcc.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hsd.fktsv.cn

[U11] Py：生成器表达式
来源：http://daa.pengpengdd.cyou

(x * 2 for x in arr)
来源：http://kbq.xylfe.cn

[U12] Py：取出现最多的 3 个元素
来源：http://keu.hammf.cn

Counter(arr).most_common(3)
来源：http://qup.zdqjudy.top

[U13] Py：固定长度队列
来源：http://yls.ydzc1.top

deque(maxlen=10)
来源：http://xfg.uphjek.com

[U14] Py：分组收集到列表
来源：http://vgc.hammf.cn

defaultdict(list)
来源：http://iyl.yanxiufei.cn

[U15] Py：高精度计时
来源：http://tuy.hnxiangtu.top

t = time.perf_counter()
来源：http://ylj.9152youxi.cn

[U16] Py：命令行参数解析
来源：http://lhu.hywenlv.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lqq.snrcjt.cn

[U17] Py：初始化日志
来源：http://zbe.chenzaomai.com

logging.basicConfig(level=logging.INFO)
来源：http://bic.xuanzx.com

[U18] Py：预编译正则
来源：http://rwr.sweek.top

pat = re.compile(r"\d+")
来源：http://sua.cdnleiting.top

[U19] Py：正则替换带回调
来源：http://tdn.tian-w.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xal.xuetiantiany.cn

[U20] Py：缓存函数结果
来源：http://hrw.nwbrower.top

@functools.lru_cache(maxsize=None)
来源：http://vgm.ivvv.top

[U21] Py：自定义上下文管理器
来源：http://vtw.hysaishi.cn

@contextlib.contextmanager
来源：http://qge.dianchejie.cn

[U22] Py：矩阵转置
来源：http://kwa.zhiwuduotai.top

list(zip(*m))
来源：http://sex.bbcook.cn

[U23] Py：分块读取大文件
来源：http://wnd.jlsjyb.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qeg.vehdjk.com

[U24] Py：路径操作
来源：http://wim.mhx1999.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://isz.mhx1999.top

[U25] Py：CSV 按字典读
来源：http://ozs.zycfv.cn

csv.DictReader(f)
来源：http://wfx.zhengqikj.top

[U26] Py：并发下载
来源：http://htu.jiagoushi.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jwg.hywenlv.cn

[U27] Py：异步 HTTP
来源：http://fro.fzhhl.top

aiohttp.ClientSession() 配合 async with
来源：http://ogi.meibo888.top

[U28] Py：类型别名
来源：http://swu.jinqigufen.top

UserId = int
来源：http://pfi.haohaochexian.top

[U29] Py：属性校验
来源：http://ljj.zhongyouzk.top

@property 与 @x.setter 配合
来源：http://ack.gotoacloud.top

[U30] Py：数据类
来源：http://cko.jinyuanbaomall.cn

@dataclass(slots=True)
来源：http://jha.fanxiaobao.xyz

[U31] Py：单测
来源：http://tsw.fehbvm.com

python -m pytest -q
来源：http://kcw.yfazqb.com

[U32] Py：代码格式化
来源：http://mdo.hongshengwenyu.top

ruff format . && ruff check --fix .
来源：http://jwv.cdnleiting.top

[U33] Py：打包发布
来源：http://vfa.wangdashe.top

python -m build  （依赖 pyproject.toml）
来源：http://ijc.jqgfzy.top

[U34] Py：判断编码
来源：http://jnr.xuanzx.com

chardet.detect(raw)
来源：http://hdd.sxryk.cn

[U35] Py：发送邮件
来源：http://wjv.yuanzhike.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://iko.xuanzx.com

[U36] Py：定时任务
来源：http://ist.yueranfly.top

schedule.every(10).minutes.do(job)
来源：http://bzp.yuanzhike.top

[U37] Py：读写 Excel
来源：http://mxb.ydjk.org.cn

pandas.read_excel / DataFrame.to_excel
来源：http://rrw.pengpengdd.cyou

[U38] Py：获取脚本所在目录
来源：http://rgz.jqgfzy.top

Path(__file__).resolve().parent
来源：http://cch.daxiang520.top

[U39] Py：判断是否在交互环境
来源：http://ddp.cashguo.top

sys.stdout.isatty()
来源：http://nga.hfpthk.cn

[U40] Py：打印到标准错误
来源：http://ipn.yj20258888.top

print("err", file=sys.stderr)
来源：http://jes.sjlbkw.cn

[U41] PHP：初始化 Composer 项目
来源：http://jzy.meibo888.top

composer init;  composer require guzzlehttp/guzzle
来源：http://cjg.chenlongwang.top

[U42] PHP：PSR-4 自动加载
来源：http://nuw.hnqzz.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://apo.fzhhl.top

[U43] PHP：声明命名空间
来源：http://uvw.jqgufenzy.top

namespace App\Http;
来源：http://hxq.wangshuangyany.cn

[U44] PHP：开启严格类型
来源：http://itf.sweek.top

declare(strict_types=1);
来源：http://oxn.yueranfly.top

[U45] PHP：类型声明与返回类型
来源：http://roo.iojbl.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://pxt.dashuyun.cn

[U46] PHP：可空类型
来源：http://vgj.tianlin.xyz

?string $name = null
来源：http://zty.svipenyu.cn

[U47] PHP：联合类型
来源：http://yip.shuidangran.top

int|string $id
来源：http://kgg.316326.xyz

[U48] PHP：纯枚举
来源：http://jcw.xziqi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nwr.xingfuxueyuan.xyz

[U49] PHP：只读属性
来源：http://vrm.sysykeji.top

public readonly string $name
来源：http://mkq.yj20258888.top

[U50] PHP：构造器属性提升
来源：http://ynp.shangyingyoupin.top

public function __construct(private int $id) {}
来源：http://ufz.hfpthk.cn

[U51] PHP：数组解构
来源：http://wim.snrcjt.cn

[$a, $b] = $arr;
来源：http://rac.aibaodan.cn

[U52] PHP：箭头函数
来源：http://gua.hnqzz.top

$double = fn($x) => $x * 2;
来源：http://zsc.epnwcf.com

[U53] PHP：空合并运算符
来源：http://eva.fzhhl.top

$v = $a ?? $b ?? "default";
来源：http://rdz.yfazqb.com

[U54] PHP：空安全调用
来源：http://hak.zdbjq.cn

$obj?->method()
来源：http://bjj.yueranfly.top

[U55] PHP：match 表达式
来源：http://kwj.epnwcf.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lhp.xingfuxueyuan.xyz

[U56] PHP：命名参数
来源：http://axf.ehwqpu.com

f(a: 1, b: 2)
来源：http://ytc.ydjk.org.cn


<!-- 参考信息 -->