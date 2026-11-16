代发 wailian999

memset(a, 0, sizeof a);
来源：http://ipi.yfazqb.com

[S27] C：定义常量
来源：http://uqo.yuanzhike.top

const double PI = 3.14159;
来源：http://wmu.316326.xyz

[S28] C：静态变量
来源：http://uxf.hnqzz.top

static int counter = 0;
来源：http://dkz.9152youxi.cn

[S29] C：变参函数
来源：http://sqk.haohaochexian.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gfn.zdqjudy.top

[S30] C：头文件保护
来源：http://tqb.redwolf501.top

#ifndef X_H
来源：http://yjo.hfpthk.cn

#define X_H
来源：http://fii.xuanzx.com

#endif
来源：http://chl.fanxiaobao.xyz

[S31] C++：Hello World
来源：http://lpp.ywan-chungtsiang.top

#include <iostream>
来源：http://tnb.xuanzx.com

int main() { std::cout << "Hello\n"; }
来源：http://opz.yfazqb.com

[S32] C++：字符串
来源：http://rwd.dashuyun.cn

std::string s = "hi";  s += "!";
来源：http://yum.cashguo.top

[S33] C++：vector 增删
来源：http://vak.snrcjt.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://opd.hesvh.cn

[S34] C++：遍历 vector
来源：http://okq.haohaochexian.top

for (auto &x : v) { std::cout << x; }
来源：http://luk.pengpengdd.cyou

[S35] C++：map
来源：http://udk.epnwcf.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qwr.ppjwa.cn

[S36] C++：unordered_map
来源：http://ena.xylfe.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lso.vqdsnc.cn

[S37] C++：set
来源：http://hsl.jqgufenzy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tcq.andypj.xyz

[S38] C++：排序
来源：http://qlo.chenjidiqi.icu

std::sort(v.begin(), v.end());
来源：http://esm.yanxiufei.cn

[S39] C++：自定义比较器排序
来源：http://hcs.shanyushiyangtech.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vxb.ydjk.org.cn

[S40] C++：查找元素
来源：http://prd.cdnleiting.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xvb.sufxvd.cn

[S41] C++：类与构造函数
来源：http://ljg.epnwcf.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dcl.yongpay.top

[S42] C++：继承与虚函数
来源：http://adu.daxiang520.top

class B : public Base { public: void f() override {} };
来源：http://eom.fengsongda.top

[S43] C++：智能指针
来源：http://kco.bjfxy.top

auto p = std::make_unique<int>(5);
来源：http://qaq.havefunace.top

[S44] C++：引用传参
来源：http://ctf.meibo888.top

void inc(int &x) { ++x; }
来源：http://ily.jyoumei.cn

[S45] C++：lambda
来源：http://yyw.vqdsnc.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qgw.ydzc1.top

[S46] C++：函数模板
来源：http://unq.sweek.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zjp.epnwcf.com

[S47] C++：结构化绑定遍历
来源：http://wfj.chenzaomai.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://brm.52xcode.cn

[S48] C++：逐行读文件
来源：http://sxi.birdmap.top

std::ifstream in("a.txt");  std::string line;
来源：http://wat.ppjwa.cn

while (std::getline(in, line)) { }
来源：http://mib.nwbrower.top

[S49] C++：写文件
来源：http://dmn.hywenlv.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zvz.xylfe.cn

[S50] C++：格式化数字
来源：http://pxo.xuanzx.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vda.gaohongyu789.top

[S51] C++：显式类型转换
来源：http://xwn.sxryk.cn

static_cast<double>(a) / b
来源：http://yyp.epnwcf.com

[S52] C++：const 与 noexcept
来源：http://zkz.zhiwuduotai.top

int size() const noexcept { return n_; }
来源：http://vfk.sufxvd.cn

[S53] C++：移动语义
来源：http://uey.tianlin.xyz

std::vector<int> w = std::move(v);
来源：http://obr.hfpthk.cn

[S54] C++：异常处理
来源：http://afw.shuidangran.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qbd.yangfankeji.com

[S55] C++：结构化绑定
来源：http://tqw.zycfv.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://lje.bjfxy.top

[S56] C++：optional
来源：http://nyc.hysaishi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tjs.redwolf501.top

[S57] C++：编译期常量
来源：http://rvg.jinqigufen.top

constexpr int N = 10;
来源：http://tui.mhx1999.top

[S58] C++：命名空间
来源：http://dcx.tian-w.cn

namespace ns { int f() { return 1; } }
来源：http://xfo.bbcook.cn

[S59] C++：静态断言
来源：http://sms.cashguo.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hkl.feifeiyinyue.top

[S60] C++：遍历并删除元素
来源：http://ffx.52xcode.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://muv.gzhubu.top

================================================================================
来源：http://nto.epnwcf.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vpk.fanxiaobao.xyz

================================================================================
来源：http://kud.nwbrower.top

[T01] Kotlin：Hello World
来源：http://ayw.hesvh.cn

println("Hello")
来源：http://hyj.havefunace.top

[T02] Kotlin：变量
来源：http://lnt.gotoacloud.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nxx.hysaishi.cn

[T03] Kotlin：字符串模板
来源：http://kgt.zhongyouzk.top

"值: $b"
来源：http://yzk.chenlongwang.top

[T04] Kotlin：空安全
来源：http://hol.quarkkingdee.top

val n: String? = null;  n?.length
来源：http://lem.daria6918.cn

[T05] Kotlin：when 表达式
来源：http://yea.yueranfly.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tss.wangshuangyany.cn

[T06] Kotlin：集合映射
来源：http://caz.gotoacloud.top

listOf(1, 2, 3).map { it * 2 }
来源：http://row.zhijiandao.cn

[T07] Kotlin：集合过滤
来源：http://ngi.chenzaomai.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://eyb.quarkkingdee.top

[T08] Kotlin：数据类
来源：http://mdn.sweek.top

data class User(val name: String, val age: Int)
来源：http://ngf.kuanghao11.cn

[T09] Kotlin：扩展函数
来源：http://kfg.hesvh.cn

fun String.exclaim() = this + "!"
来源：http://yru.haohaochexian.top

[T10] Kotlin：默认参数
来源：http://dgj.havefunace.top

fun greet(name: String = "World") = "Hi $name"
来源：http://eil.guannengcc.top

[T11] Kotlin：协程
来源：http://wlo.shzxlz.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://bcm.shangyingyoupin.top

[T12] Kotlin：解构声明
来源：http://tqb.c1oappe.top

val (a, b) = Pair(1, 2)
来源：http://iuk.52xcode.cn

[T13] Kotlin：只读 Map
来源：http://rvm.havefunace.top

val m = mapOf("a" to 1)
来源：http://nrp.tanke756.top

[T14] Kotlin：循环
来源：http://cgv.snrcjt.cn

for (i in 1..10) println(i)
来源：http://lzy.zhongyouzk.top

[T15] Kotlin：接口
来源：http://ryo.tarul.cn

interface Shape { fun area(): Double }
来源：http://eyw.ydzc1.top

[T16] Swift：Hello World
来源：http://rwf.redwolf501.top

print("Hello")
来源：http://aqk.yj20258888.top

[T17] Swift：变量与常量
来源：http://hpc.hnxiangtu.top

var a = 1;  let b = 2
来源：http://bnk.zhijiandao.cn

[T18] Swift：字符串插值
来源：http://syl.iojbl.cn

"值: \(b)"
来源：http://uil.bbcook.cn

[T19] Swift：可选绑定
来源：http://crs.dashuyun.cn

if let n = opt { print(n) }
来源：http://leb.yueranfly.top

[T20] Swift：数组操作
来源：http://ajr.chenzaomai.com

var a = [1, 2, 3];  a.append(4)
来源：http://qsw.52xcode.cn

[T21] Swift：遍历
来源：http://abe.sysykeji.top

for x in a { print(x) }
来源：http://swp.hfpthk.cn

[T22] Swift：字典
来源：http://mzj.birdmap.top

var d = ["a": 1];  d["b"] = 2
来源：http://mld.jyoumei.cn

[T23] Swift：函数
来源：http://nvq.vqdsnc.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fxd.hammf.cn

[T24] Swift：闭包
来源：http://rgb.svipenyu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qwb.quarkkingdee.top

[T25] Swift：结构体
来源：http://toh.vehdjk.com

struct P { var x: Int }
来源：http://yad.zhaomingkeji.xyz

[T26] Swift：类与重写
来源：http://qrf.xinyue.icu

class A: Base { override func f() {} }
来源：http://qbh.chenlongwang.top

[T27] Swift：错误处理
来源：http://mdj.fehbvm.com

do { try f() } catch { print(error) }
来源：http://smh.iojbl.cn

[T28] Swift：枚举
来源：http://ayx.birdmap.top

enum Color { case red, green }
来源：http://ecc.guannengcc.top

[T29] Swift：guard 提前返回
来源：http://ahx.daria6918.cn

guard let x = opt else { return }
来源：http://pko.xinyue.icu

[T30] Swift：协议
来源：http://rib.xingfuxueyuan.xyz

protocol Shape { func area() -> Double }
来源：http://xen.chenjidiqi.icu

[T31] Lua：Hello World
来源：http://gor.zdbjq.cn

print("Hello")
来源：http://ilo.xingfuxueyuan.xyz

[T32] Lua：局部变量
来源：http://duu.fehbvm.com

local a = 1
来源：http://luq.c1oappe.top

[T33] Lua：表（数组）
来源：http://tui.c1oappe.top

local t = {1, 2, 3};  t[4] = 4
来源：http://jhu.fengsongda.top

[T34] Lua：遍历表
来源：http://lha.jinyuanbaomall.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://pgp.zycfv.cn

[T35] Lua：字典表
来源：http://tsb.hammf.cn

local d = { a = 1 };  d.b = 2
来源：http://wrw.dianchejie.cn

[T36] Lua：函数
来源：http://pyc.xingfuxueyuan.xyz

function add(a, b) return a + b end
来源：http://xxt.nanxuanxn.top

[T37] Lua：字符串拼接
来源：http://pzz.gaohongyu789.top

"a" .. "b"
来源：http://zts.9152youxi.cn

[T38] Lua：条件
来源：http://sbl.tian-w.cn

if x > 0 then print("正") end
来源：http://ruh.9152youxi.cn

[T39] Lua：模式匹配
来源：http://ogr.ctjpmb.com

string.find(s, "%d+")
来源：http://zph.jqgfzy.top

[T40] Lua：元表
来源：http://goq.shangyingyoupin.top

setmetatable({}, { __index = base })
来源：http://xth.tarul.cn

[T41] Perl：Hello World
来源：http://nwm.iojbl.cn

print "Hello\n";
来源：http://wwz.jianghu66.top

[T42] Perl：变量类型
来源：http://sfg.cdnleiting.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://klk.nwbrower.top

[T43] Perl：字符串插值
来源：http://uzr.jianghu66.top

"值: $a"
来源：http://vbj.xziqi.cn

[T44] Perl：条件
来源：http://wku.uphjek.com

if ($a > 0) { print "正"; }
来源：http://hyw.yueranfly.top

[T45] Perl：数组遍历
来源：http://efi.0kj1m.cn

for my $x (@arr) { print $x; }
来源：http://ktf.c1oappe.top

[T46] Perl：哈希操作
来源：http://kwy.jqgufenzy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xwh.jlsjyb.cn

[T47] Perl：正则捕获
来源：http://dnx.52xcode.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://une.sysykeji.top

[T48] Perl：正则替换
来源：http://por.bbcook.cn

$s =~ s/old/new/g;
来源：http://ymg.jinqigufen.top

[T49] Perl：函数
来源：http://dtg.smart0.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jrg.gotoacloud.top

[T50] Perl：逐行读文件
来源：http://wbd.nwbrower.top

open my $fh, "<", "a.txt" or die $!;
来源：http://nel.tanke756.top

while (my $line = <$fh>) { print $line; }
来源：http://pjl.nanxuanxn.top

[T51] Scala：Hello World
来源：http://rvy.aizwys.cn

println("Hello")
来源：http://prp.zhixingplan.top

[T52] Scala：变量
来源：http://sbq.xuetiantiany.cn

val a = 1;  var b = 2
来源：http://yen.shzxlz.cn

[T53] Scala：字符串插值
来源：http://rfk.0kj1m.cn

s"值: $b"
来源：http://hrp.zhongyouzk.top

[T54] Scala：集合映射
来源：http://pqe.fanxiaobao.xyz

List(1, 2, 3).map(_ * 2)
来源：http://xyt.wangdashe.top

[T55] Scala：集合过滤
来源：http://qgc.ctjpmb.com

List(1, 2, 3).filter(_ > 1)
来源：http://ckb.cheryme.top

[T56] Scala：样例类
来源：http://qvw.xziqi.cn

case class User(name: String, age: Int)
来源：http://puw.xuanzx.com

[T57] Scala：模式匹配
来源：http://opn.aizwys.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://uja.chenlongwang.top

[T58] Scala：函数定义
来源：http://rai.yongpay.top

def add(a: Int, b: Int): Int = a + b
来源：http://gab.ybcxt.top

[T59] Scala：循环
来源：http://vle.hnxiangtu.top

for (i <- 1 to 10) println(i)
来源：http://iju.yonumen.top

[T60] Scala：折叠
来源：http://mxd.yj20258888.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lzk.yongpay.top

================================================================================
来源：http://rrt.fanxiaobao.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lla.hongshengwenyu.top

================================================================================
来源：http://czg.jinyuanbaomall.cn

[U01] Py：创建虚拟环境
来源：http://zxu.jlsjyb.cn

python -m venv .venv && source .venv/bin/activate
来源：http://dzf.epnwcf.com

[U02] Py：导出 / 安装依赖
来源：http://fzl.cdnleiting.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://djr.svipenyu.cn

[U03] Py：加载 .env 配置
来源：http://ujd.316326.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://dhj.hfpthk.cn

[U04] Py：变量调试打印
来源：http://coc.jqgfzy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://edy.ydzc1.top

[U05] Py：列表去重且保序
来源：http://vck.daxiang520.top

list(dict.fromkeys(arr))
来源：http://crs.hfpthk.cn

[U06] Py：合并两个字典
来源：http://wtx.yvedp.cn

{**a, **b}
来源：http://upv.zdbjq.cn

[U07] Py：反转字典键值
来源：http://yua.feifeiyinyue.top

{v: k for k, v in d.items()}
来源：http://ncz.bbcook.cn

[U08] Py：展平二维列表
来源：http://pyp.vehdjk.com

[y for x in nested for y in x]
来源：http://clb.dashuyun.cn

[U09] Py：字典取最大值的键
来源：http://sit.yuxming.cn

max(d, key=d.get)
来源：http://mki.aibaodan.cn

[U10] Py：按值排序字典
来源：http://okk.nanxinkj.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gke.sjlbkw.cn

[U11] Py：生成器表达式
来源：http://mhd.fengsongda.top

(x * 2 for x in arr)
来源：http://ubo.pycfn.com

[U12] Py：取出现最多的 3 个元素
来源：http://bmq.gaohongyu789.top

Counter(arr).most_common(3)
来源：http://dbt.bbcook.cn

[U13] Py：固定长度队列
来源：http://zcn.haohaochexian.top

deque(maxlen=10)
来源：http://pyq.yj20258.top

[U14] Py：分组收集到列表
来源：http://wqo.tian-w.cn

defaultdict(list)
来源：http://qhl.pycfn.com

[U15] Py：高精度计时
来源：http://cid.zhengqikj.top

t = time.perf_counter()
来源：http://mqf.ppjwa.cn

[U16] Py：命令行参数解析
来源：http://qsz.guowangkeji.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rhd.svipenyu.cn

[U17] Py：初始化日志
来源：http://ohi.sjlbkw.cn

logging.basicConfig(level=logging.INFO)
来源：http://ikc.hnxiangtu.top

[U18] Py：预编译正则
来源：http://pjq.gogol.net.cn

pat = re.compile(r"\d+")
来源：http://jwb.wangshuangyany.cn

[U19] Py：正则替换带回调
来源：http://yep.316326.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zla.tian-w.cn

[U20] Py：缓存函数结果
来源：http://sbi.ydjk.org.cn

@functools.lru_cache(maxsize=None)
来源：http://nzs.quarkkingdee.top

[U21] Py：自定义上下文管理器
来源：http://nuv.daria6918.cn

@contextlib.contextmanager
来源：http://sqf.jyoumei.cn

[U22] Py：矩阵转置
来源：http://srh.daria6918.cn

list(zip(*m))
来源：http://bkb.redwolf501.top

[U23] Py：分块读取大文件
来源：http://mln.yueranfly.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mlj.wangdashe.top

[U24] Py：路径操作
来源：http://sxl.xuanzx.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bws.hammf.cn

[U25] Py：CSV 按字典读
来源：http://gjy.ybcxt.top

csv.DictReader(f)
来源：http://tap.9152youxi.cn

[U26] Py：并发下载
来源：http://eel.jianghu66.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wek.jqgfzy.top

[U27] Py：异步 HTTP
来源：http://phb.daxiang520.top

aiohttp.ClientSession() 配合 async with
来源：http://ixz.dianchejie.cn

[U28] Py：类型别名
来源：http://geu.sxryk.cn

UserId = int
来源：http://ssl.wangdashe.top

[U29] Py：属性校验
来源：http://uxc.daria6918.cn

@property 与 @x.setter 配合
来源：http://pyz.sufxvd.cn

[U30] Py：数据类
来源：http://apb.vehdjk.com

@dataclass(slots=True)
来源：http://hxy.sufxvd.cn

[U31] Py：单测
来源：http://eez.dianchejie.cn

python -m pytest -q
来源：http://nll.fanxiaobao.xyz

[U32] Py：代码格式化
来源：http://bpv.zhengqikj.top

ruff format . && ruff check --fix .
来源：http://lnu.xuanzx.com

[U33] Py：打包发布
来源：http://dqb.sufxvd.cn

python -m build  （依赖 pyproject.toml）
来源：http://chg.zdqjudy.top

[U34] Py：判断编码
来源：http://ocu.gaohongyu789.top

chardet.detect(raw)
来源：http://jdq.svipenyu.cn

[U35] Py：发送邮件
来源：http://ego.dashuyun.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nvn.hysaishi.cn

[U36] Py：定时任务
来源：http://hyw.cheryme.top

schedule.every(10).minutes.do(job)
来源：http://wue.yueranfly.top

[U37] Py：读写 Excel
来源：http://diz.chenzaomai.com

pandas.read_excel / DataFrame.to_excel
来源：http://ogt.zhixingplan.top

[U38] Py：获取脚本所在目录
来源：http://vtm.yuxming.cn

Path(__file__).resolve().parent
来源：http://hhn.daria6918.cn

[U39] Py：判断是否在交互环境
来源：http://hox.hysaishi.cn

sys.stdout.isatty()
来源：http://jts.yvedp.cn

[U40] Py：打印到标准错误
来源：http://pvq.yuanzhike.top

print("err", file=sys.stderr)
来源：http://xfp.svipenyu.cn

[U41] PHP：初始化 Composer 项目
来源：http://rya.nanxinkj.top

composer init;  composer require guzzlehttp/guzzle
来源：http://lio.shangyingyoupin.top

[U42] PHP：PSR-4 自动加载
来源：http://tnd.sysykeji.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ach.havefunace.top

[U43] PHP：声明命名空间
来源：http://erx.hnqzz.top

namespace App\Http;
来源：http://foj.jianghu66.top

[U44] PHP：开启严格类型
来源：http://fdw.sweek.top

declare(strict_types=1);
来源：http://vqm.daria6918.cn

[U45] PHP：类型声明与返回类型
来源：http://oom.ydjk.org.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://exl.meibo888.top

[U46] PHP：可空类型
来源：http://rtk.redwolf501.top

?string $name = null
来源：http://fri.iojbl.cn

[U47] PHP：联合类型
来源：http://pgg.mhx1999.top

int|string $id
来源：http://bhg.zhaomingkeji.xyz

[U48] PHP：纯枚举
来源：http://htp.yuxming.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xdq.chenzaomai.com

[U49] PHP：只读属性
来源：http://ipo.kuanghao11.cn

public readonly string $name
来源：http://fhr.sufxvd.cn

[U50] PHP：构造器属性提升
来源：http://vut.hesvh.cn

public function __construct(private int $id) {}
来源：http://kmz.cdnleiting.top


<!-- 参考信息 -->