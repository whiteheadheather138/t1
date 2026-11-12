代发 wailian999

memset(a, 0, sizeof a);
来源：http://lnw.havefunace.top

[S27] C：定义常量
来源：http://mrz.bbcook.cn

const double PI = 3.14159;
来源：http://qbh.pengpengdd.cyou

[S28] C：静态变量
来源：http://dyo.hammf.cn

static int counter = 0;
来源：http://tal.daria6918.cn

[S29] C：变参函数
来源：http://kbj.fktsv.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bvg.cdnleiting.top

[S30] C：头文件保护
来源：http://ohn.xuetiantiany.cn

#ifndef X_H
来源：http://hav.c1oappe.top

#define X_H
来源：http://srx.bjfxy.top

#endif
来源：http://csv.dianchejie.cn

[S31] C++：Hello World
来源：http://hyu.vqdsnc.cn

#include <iostream>
来源：http://oai.yueranfly.top

int main() { std::cout << "Hello\n"; }
来源：http://iat.gaohongyu789.top

[S32] C++：字符串
来源：http://xmg.xziqi.cn

std::string s = "hi";  s += "!";
来源：http://phn.yuanzhike.top

[S33] C++：vector 增删
来源：http://qie.shangyingyoupin.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://foe.fanxiaobao.xyz

[S34] C++：遍历 vector
来源：http://izp.hcnkem.com

for (auto &x : v) { std::cout << x; }
来源：http://bzs.yj20258.top

[S35] C++：map
来源：http://nuh.zhaomingkeji.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xcp.xylfe.cn

[S36] C++：unordered_map
来源：http://tio.0kj1m.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://evi.pycfn.com

[S37] C++：set
来源：http://xsg.yangfankeji.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gce.yuanzhike.top

[S38] C++：排序
来源：http://bkn.shuidangran.top

std::sort(v.begin(), v.end());
来源：http://mqx.zhijiandao.cn

[S39] C++：自定义比较器排序
来源：http://nmk.andypj.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lry.ydzc1.top

[S40] C++：查找元素
来源：http://apa.jqgfzy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vvl.ppjwa.cn

[S41] C++：类与构造函数
来源：http://owa.vehdjk.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://flz.hywenlv.cn

[S42] C++：继承与虚函数
来源：http://idy.gogol.net.cn

class B : public Base { public: void f() override {} };
来源：http://jwv.zhixingplan.top

[S43] C++：智能指针
来源：http://svf.jlsjyb.cn

auto p = std::make_unique<int>(5);
来源：http://mqx.c1oappe.top

[S44] C++：引用传参
来源：http://mln.jinghuilouyu.cn

void inc(int &x) { ++x; }
来源：http://xqx.shzxlz.cn

[S45] C++：lambda
来源：http://ahk.ydjk.org.cn

auto add = [](int a, int b) { return a + b; };
来源：http://iqi.cashguo.top

[S46] C++：函数模板
来源：http://flr.ivvv.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kmf.aizwys.cn

[S47] C++：结构化绑定遍历
来源：http://ans.shzxlz.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://els.cdnleiting.top

[S48] C++：逐行读文件
来源：http://tbn.sysykeji.top

std::ifstream in("a.txt");  std::string line;
来源：http://nyu.ydzc1.top

while (std::getline(in, line)) { }
来源：http://fdj.zhixingplan.top

[S49] C++：写文件
来源：http://vpt.0kj1m.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://top.svipenyu.cn

[S50] C++：格式化数字
来源：http://xul.xuetiantiany.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://may.zdbjq.cn

[S51] C++：显式类型转换
来源：http://rpo.shanyushiyangtech.top

static_cast<double>(a) / b
来源：http://ulg.quarkkingdee.top

[S52] C++：const 与 noexcept
来源：http://bjr.guannengcc.top

int size() const noexcept { return n_; }
来源：http://zik.nwbrower.top

[S53] C++：移动语义
来源：http://nxa.shuidangran.top

std::vector<int> w = std::move(v);
来源：http://ivp.hywenlv.cn

[S54] C++：异常处理
来源：http://wuh.ybcxt.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cnv.shzxlz.cn

[S55] C++：结构化绑定
来源：http://fis.daxiang520.top

auto [a, b] = std::make_pair(1, 2);
来源：http://hwm.havefunace.top

[S56] C++：optional
来源：http://jjm.smart0.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tqo.shangyingyoupin.top

[S57] C++：编译期常量
来源：http://bas.ppjwa.cn

constexpr int N = 10;
来源：http://ysj.cheryme.top

[S58] C++：命名空间
来源：http://dkz.yuanzhike.top

namespace ns { int f() { return 1; } }
来源：http://tyq.xylfe.cn

[S59] C++：静态断言
来源：http://mvj.cqqwz.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vqg.vqdsnc.cn

[S60] C++：遍历并删除元素
来源：http://yfj.hnxiangtu.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cps.zhaomingkeji.xyz

================================================================================
来源：http://vpy.hongshengwenyu.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dqt.hcnkem.com

================================================================================
来源：http://xft.jinqigufen.top

[T01] Kotlin：Hello World
来源：http://zrw.jianghu66.top

println("Hello")
来源：http://svz.sjlbkw.cn

[T02] Kotlin：变量
来源：http://cue.jianghu66.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jbk.ybcxt.top

[T03] Kotlin：字符串模板
来源：http://lml.haohaochexian.top

"值: $b"
来源：http://kdb.pycfn.com

[T04] Kotlin：空安全
来源：http://ija.haohaochexian.top

val n: String? = null;  n?.length
来源：http://osp.xylfe.cn

[T05] Kotlin：when 表达式
来源：http://pkg.redwolf501.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wnm.feifeiyinyue.top

[T06] Kotlin：集合映射
来源：http://mbg.nwbrower.top

listOf(1, 2, 3).map { it * 2 }
来源：http://vpb.zhaomingkeji.xyz

[T07] Kotlin：集合过滤
来源：http://hfj.xingfuxueyuan.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://dfn.zhiwuduotai.top

[T08] Kotlin：数据类
来源：http://nmr.dianchejie.cn

data class User(val name: String, val age: Int)
来源：http://lgh.tian-w.cn

[T09] Kotlin：扩展函数
来源：http://czj.pengpengdd.cyou

fun String.exclaim() = this + "!"
来源：http://irf.zhiwuduotai.top

[T10] Kotlin：默认参数
来源：http://uma.jyoumei.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://tcr.yanxiufei.cn

[T11] Kotlin：协程
来源：http://van.shanyushiyangkeji.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://kgm.meibo888.top

[T12] Kotlin：解构声明
来源：http://bdn.daria6918.cn

val (a, b) = Pair(1, 2)
来源：http://yrr.jyoumei.cn

[T13] Kotlin：只读 Map
来源：http://ztn.snrcjt.cn

val m = mapOf("a" to 1)
来源：http://mmu.52xcode.cn

[T14] Kotlin：循环
来源：http://kdy.daxiang520.top

for (i in 1..10) println(i)
来源：http://nws.gaohongyu789.top

[T15] Kotlin：接口
来源：http://ngt.ehwqpu.com

interface Shape { fun area(): Double }
来源：http://tbc.fzhhl.top

[T16] Swift：Hello World
来源：http://erh.fehbvm.com

print("Hello")
来源：http://klb.zycfv.cn

[T17] Swift：变量与常量
来源：http://otp.tian-w.cn

var a = 1;  let b = 2
来源：http://anz.sysykeji.top

[T18] Swift：字符串插值
来源：http://nus.jinyuanbaomall.cn

"值: \(b)"
来源：http://tor.fengsongda.top

[T19] Swift：可选绑定
来源：http://wmh.yvedp.cn

if let n = opt { print(n) }
来源：http://kxw.hfpthk.cn

[T20] Swift：数组操作
来源：http://vst.316326.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://bkb.ctjpmb.com

[T21] Swift：遍历
来源：http://nep.cqqwz.cn

for x in a { print(x) }
来源：http://yrg.xingfuxueyuan.xyz

[T22] Swift：字典
来源：http://qom.sufxvd.cn

var d = ["a": 1];  d["b"] = 2
来源：http://niq.jyoumei.cn

[T23] Swift：函数
来源：http://mya.jiagoushi.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://crv.yj202588.top

[T24] Swift：闭包
来源：http://obr.ydjk.org.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://dmc.dianchejie.cn

[T25] Swift：结构体
来源：http://jfx.tianlin.xyz

struct P { var x: Int }
来源：http://xfp.feifeiyinyue.top

[T26] Swift：类与重写
来源：http://okr.haohaochexian.top

class A: Base { override func f() {} }
来源：http://pco.nanxinkj.top

[T27] Swift：错误处理
来源：http://wnp.zdqjudy.top

do { try f() } catch { print(error) }
来源：http://lvy.sysykeji.top

[T28] Swift：枚举
来源：http://vaj.yanxiufei.cn

enum Color { case red, green }
来源：http://bob.tianlin.xyz

[T29] Swift：guard 提前返回
来源：http://vrb.tianlin.xyz

guard let x = opt else { return }
来源：http://otz.redwolf501.top

[T30] Swift：协议
来源：http://jkc.snrcjt.cn

protocol Shape { func area() -> Double }
来源：http://fcr.gzhubu.top

[T31] Lua：Hello World
来源：http://jet.nanxuanxn.top

print("Hello")
来源：http://ftl.sysykeji.top

[T32] Lua：局部变量
来源：http://dwi.hywenlv.cn

local a = 1
来源：http://zph.fktsv.cn

[T33] Lua：表（数组）
来源：http://mjm.52xcode.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ieq.chenzaomai.com

[T34] Lua：遍历表
来源：http://tpr.ywan-chungtsiang.top

for i, v in ipairs(t) do print(i, v) end
来源：http://hki.yuanzhike.top

[T35] Lua：字典表
来源：http://uej.yueranfly.top

local d = { a = 1 };  d.b = 2
来源：http://lhu.ctjpmb.com

[T36] Lua：函数
来源：http://irr.zdbjq.cn

function add(a, b) return a + b end
来源：http://ahf.jqgfzy.top

[T37] Lua：字符串拼接
来源：http://eje.zhixingplan.top

"a" .. "b"
来源：http://ngb.jinqigfzy.top

[T38] Lua：条件
来源：http://nlk.jqgufenzy.top

if x > 0 then print("正") end
来源：http://mih.ctjpmb.com

[T39] Lua：模式匹配
来源：http://kat.chenlongwang.top

string.find(s, "%d+")
来源：http://fgj.cqqwz.cn

[T40] Lua：元表
来源：http://ogj.fzhhl.top

setmetatable({}, { __index = base })
来源：http://bpd.snrcjt.cn

[T41] Perl：Hello World
来源：http://fty.dianchejie.cn

print "Hello\n";
来源：http://nhv.jinqigfzy.top

[T42] Perl：变量类型
来源：http://zcx.nanxinkj.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pmu.cdnleiting.top

[T43] Perl：字符串插值
来源：http://olf.vehdjk.com

"值: $a"
来源：http://rmt.daria6918.cn

[T44] Perl：条件
来源：http://snd.sufxvd.cn

if ($a > 0) { print "正"; }
来源：http://oyb.vqdsnc.cn

[T45] Perl：数组遍历
来源：http://qwo.ydzc1.top

for my $x (@arr) { print $x; }
来源：http://afq.snrcjt.cn

[T46] Perl：哈希操作
来源：http://fss.zhijiandao.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ase.guannengcc.top

[T47] Perl：正则捕获
来源：http://lir.hnqzz.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://qjs.quarkkingdee.top

[T48] Perl：正则替换
来源：http://pxy.bbcook.cn

$s =~ s/old/new/g;
来源：http://azv.fktsv.cn

[T49] Perl：函数
来源：http://exb.hesvh.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://bfx.gotoacloud.top

[T50] Perl：逐行读文件
来源：http://zhj.shuidangran.top

open my $fh, "<", "a.txt" or die $!;
来源：http://kwr.zhoulong.xyz

while (my $line = <$fh>) { print $line; }
来源：http://nla.jinyuanbaomall.cn

[T51] Scala：Hello World
来源：http://pkc.jinqigfzy.top

println("Hello")
来源：http://hro.jqgfzy.top

[T52] Scala：变量
来源：http://mmo.c1oappe.top

val a = 1;  var b = 2
来源：http://zds.feifeiyinyue.top

[T53] Scala：字符串插值
来源：http://ipx.pycfn.com

s"值: $b"
来源：http://uoc.ppjwa.cn

[T54] Scala：集合映射
来源：http://hie.bbcook.cn

List(1, 2, 3).map(_ * 2)
来源：http://hao.zhaomingkeji.xyz

[T55] Scala：集合过滤
来源：http://oqc.gogol.net.cn

List(1, 2, 3).filter(_ > 1)
来源：http://hzs.xziqi.cn

[T56] Scala：样例类
来源：http://udt.zhengqikj.top

case class User(name: String, age: Int)
来源：http://dnk.chenzaomai.com

[T57] Scala：模式匹配
来源：http://bua.yfazqb.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://icv.chenzaomai.com

[T58] Scala：函数定义
来源：http://msz.jianghu66.top

def add(a: Int, b: Int): Int = a + b
来源：http://xwg.ehwqpu.com

[T59] Scala：循环
来源：http://vqk.epnwcf.com

for (i <- 1 to 10) println(i)
来源：http://ttf.nanxuanxn.top

[T60] Scala：折叠
来源：http://knl.hammf.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dir.pycfn.com

================================================================================
来源：http://wdt.cdnleiting.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kpr.jqgfzy.top

================================================================================
来源：http://khx.gzhubu.top

[U01] Py：创建虚拟环境
来源：http://olr.tian-w.cn

python -m venv .venv && source .venv/bin/activate
来源：http://sxr.hongshengwenyu.top

[U02] Py：导出 / 安装依赖
来源：http://obf.xylfe.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://itu.hywenlv.cn

[U03] Py：加载 .env 配置
来源：http://kzi.wangdashe.top

from dotenv import load_dotenv; load_dotenv()
来源：http://vdc.gotoacloud.top

[U04] Py：变量调试打印
来源：http://knx.haohaochexian.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wnf.zycfv.cn

[U05] Py：列表去重且保序
来源：http://pfs.zhongyouzk.top

list(dict.fromkeys(arr))
来源：http://ccv.fehbvm.com

[U06] Py：合并两个字典
来源：http://hiv.9152youxi.cn

{**a, **b}
来源：http://rll.zycfv.cn

[U07] Py：反转字典键值
来源：http://sqp.zhijiandao.cn

{v: k for k, v in d.items()}
来源：http://tow.zhengqikj.top

[U08] Py：展平二维列表
来源：http://niy.cucudq.cn

[y for x in nested for y in x]
来源：http://zjv.0kj1m.cn

[U09] Py：字典取最大值的键
来源：http://lqa.xuetiantiany.cn

max(d, key=d.get)
来源：http://oqv.jqgufenzy.top

[U10] Py：按值排序字典
来源：http://wus.jiagoushi.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nsx.shanyushiyangtech.top

[U11] Py：生成器表达式
来源：http://ufl.sysykeji.top

(x * 2 for x in arr)
来源：http://sdo.cqqwz.cn

[U12] Py：取出现最多的 3 个元素
来源：http://qos.epnwcf.com

Counter(arr).most_common(3)
来源：http://cbx.sysykeji.top

[U13] Py：固定长度队列
来源：http://zmi.hammf.cn

deque(maxlen=10)
来源：http://rrs.sjlbkw.cn

[U14] Py：分组收集到列表
来源：http://ywf.shuidangran.top

defaultdict(list)
来源：http://aoa.bjfxy.top

[U15] Py：高精度计时
来源：http://nge.jyoumei.cn

t = time.perf_counter()
来源：http://zmp.zhiwuduotai.top

[U16] Py：命令行参数解析
来源：http://lsq.xinyue.icu

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sil.hesvh.cn

[U17] Py：初始化日志
来源：http://sbv.hnqzz.top

logging.basicConfig(level=logging.INFO)
来源：http://gri.yj20258.top

[U18] Py：预编译正则
来源：http://obw.cheryme.top

pat = re.compile(r"\d+")
来源：http://mmt.redwolf501.top

[U19] Py：正则替换带回调
来源：http://yko.cucudq.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xyn.jinqigfzy.top

[U20] Py：缓存函数结果
来源：http://put.pengpengdd.cyou

@functools.lru_cache(maxsize=None)
来源：http://fvg.chenzaomai.com

[U21] Py：自定义上下文管理器
来源：http://rhk.shangyingyoupin.top

@contextlib.contextmanager
来源：http://ivb.nanxinkj.top

[U22] Py：矩阵转置
来源：http://wey.dianchejie.cn

list(zip(*m))
来源：http://lsc.mhx1999.top

[U23] Py：分块读取大文件
来源：http://jsv.c1oappe.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xog.ywan-chungtsiang.top

[U24] Py：路径操作
来源：http://yro.jinqigfzy.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dck.xylfe.cn

[U25] Py：CSV 按字典读
来源：http://vol.fanxiaobao.xyz

csv.DictReader(f)
来源：http://had.tianlin.xyz

[U26] Py：并发下载
来源：http://aqu.shanyushiyangtech.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zrg.cheryme.top

[U27] Py：异步 HTTP
来源：http://wnw.meibo888.top

aiohttp.ClientSession() 配合 async with
来源：http://hcv.xingfuxueyuan.xyz

[U28] Py：类型别名
来源：http://oop.hywenlv.cn

UserId = int
来源：http://xgr.zhiwuduotai.top

[U29] Py：属性校验
来源：http://udq.tarul.cn

@property 与 @x.setter 配合
来源：http://lmw.zycfv.cn

[U30] Py：数据类
来源：http://bpv.yonumen.top

@dataclass(slots=True)
来源：http://onc.jinghuilouyu.cn

[U31] Py：单测
来源：http://tag.sweek.top

python -m pytest -q
来源：http://ujq.shanyushiyangkeji.top

[U32] Py：代码格式化
来源：http://xyz.andypj.xyz

ruff format . && ruff check --fix .
来源：http://txv.xuetiantiany.cn

[U33] Py：打包发布
来源：http://oyd.ehwqpu.com

python -m build  （依赖 pyproject.toml）
来源：http://tvi.fehbvm.com

[U34] Py：判断编码
来源：http://wuk.shangyingyoupin.top

chardet.detect(raw)
来源：http://lrb.fengsongda.top

[U35] Py：发送邮件
来源：http://phv.wangdashe.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xho.jinyuanbaomall.cn

[U36] Py：定时任务
来源：http://drt.yj202588.top

schedule.every(10).minutes.do(job)
来源：http://fhp.xylfe.cn

[U37] Py：读写 Excel
来源：http://ycq.gogol.net.cn

pandas.read_excel / DataFrame.to_excel
来源：http://fmf.cucudq.cn

[U38] Py：获取脚本所在目录
来源：http://ske.gogol.net.cn

Path(__file__).resolve().parent
来源：http://ajv.tanke756.top

[U39] Py：判断是否在交互环境
来源：http://bvc.hesvh.cn

sys.stdout.isatty()
来源：http://bhw.jlsjyb.cn

[U40] Py：打印到标准错误
来源：http://ivm.vehdjk.com

print("err", file=sys.stderr)
来源：http://efs.bjfxy.top

[U41] PHP：初始化 Composer 项目
来源：http://glv.redwolf501.top

composer init;  composer require guzzlehttp/guzzle
来源：http://npt.ydjk.org.cn

[U42] PHP：PSR-4 自动加载
来源：http://ggh.epnwcf.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wst.shzxlz.cn

[U43] PHP：声明命名空间
来源：http://fbh.yj202588.top

namespace App\Http;
来源：http://bwb.tarul.cn

[U44] PHP：开启严格类型
来源：http://xof.feifeiyinyue.top

declare(strict_types=1);
来源：http://upd.chenlongwang.top

[U45] PHP：类型声明与返回类型
来源：http://tvj.ehwqpu.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://sla.fanxiaobao.xyz

[U46] PHP：可空类型
来源：http://qbn.tian-w.cn

?string $name = null
来源：http://sjt.fanxiaobao.xyz

[U47] PHP：联合类型
来源：http://gzx.dashuyun.cn

int|string $id
来源：http://tmn.daria6918.cn

[U48] PHP：纯枚举
来源：http://opg.cqqwz.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ait.guowangkeji.top

[U49] PHP：只读属性
来源：http://rvh.daxiang520.top

public readonly string $name
来源：http://fqa.9152youxi.cn

[U50] PHP：构造器属性提升
来源：http://ogr.hongshengwenyu.top

public function __construct(private int $id) {}
来源：http://izu.gaohongyu789.top


<!-- 参考信息 -->