代发 wailian999

#ifndef X_H
来源：http://zzw.smart0.xyz

#define X_H
来源：http://aov.shzxlz.cn

#endif
来源：http://gnp.redwolf501.top

[S31] C++：Hello World
来源：http://bsz.vqdsnc.cn

#include <iostream>
来源：http://xgr.daxiang520.top

int main() { std::cout << "Hello\n"; }
来源：http://lzb.gzhubu.top

[S32] C++：字符串
来源：http://lge.jianghu66.top

std::string s = "hi";  s += "!";
来源：http://geh.0kj1m.cn

[S33] C++：vector 增删
来源：http://tjz.nwbrower.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pvy.sysykeji.top

[S34] C++：遍历 vector
来源：http://hxh.316326.xyz

for (auto &x : v) { std::cout << x; }
来源：http://feg.nanxinkj.top

[S35] C++：map
来源：http://gic.sweek.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qeg.bbcook.cn

[S36] C++：unordered_map
来源：http://pcq.hywenlv.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gni.cqqwz.cn

[S37] C++：set
来源：http://itx.fzhhl.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ezs.zhoulong.xyz

[S38] C++：排序
来源：http://itq.tian-w.cn

std::sort(v.begin(), v.end());
来源：http://wmx.fanxiaobao.xyz

[S39] C++：自定义比较器排序
来源：http://ajv.52xcode.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qnw.vehdjk.com

[S40] C++：查找元素
来源：http://ukf.0kj1m.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ocr.havefunace.top

[S41] C++：类与构造函数
来源：http://ley.xingfuxueyuan.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hla.pengpengdd.cyou

[S42] C++：继承与虚函数
来源：http://yic.fzhhl.top

class B : public Base { public: void f() override {} };
来源：http://hgo.epnwcf.com

[S43] C++：智能指针
来源：http://idk.yangfankeji.com

auto p = std::make_unique<int>(5);
来源：http://ezl.dianchejie.cn

[S44] C++：引用传参
来源：http://yzt.bbcook.cn

void inc(int &x) { ++x; }
来源：http://flx.andypj.xyz

[S45] C++：lambda
来源：http://gdk.fengsongda.top

auto add = [](int a, int b) { return a + b; };
来源：http://chd.chenlongwang.top

[S46] C++：函数模板
来源：http://fss.hnxiangtu.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ljl.dashuyun.cn

[S47] C++：结构化绑定遍历
来源：http://wbn.shanyushiyangkeji.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ufc.wangdashe.top

[S48] C++：逐行读文件
来源：http://blk.tianlin.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://nng.zhongyouzk.top

while (std::getline(in, line)) { }
来源：http://hto.zhixingplan.top

[S49] C++：写文件
来源：http://qoj.yueranfly.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bux.pengpengdd.cyou

[S50] C++：格式化数字
来源：http://hnm.hfpthk.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://val.yj20258.top

[S51] C++：显式类型转换
来源：http://zvg.hywenlv.cn

static_cast<double>(a) / b
来源：http://sgn.birdmap.top

[S52] C++：const 与 noexcept
来源：http://jcp.cucudq.cn

int size() const noexcept { return n_; }
来源：http://nrf.fzhhl.top

[S53] C++：移动语义
来源：http://wgs.cashguo.top

std::vector<int> w = std::move(v);
来源：http://dcq.uphjek.com

[S54] C++：异常处理
来源：http://nft.iojbl.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://iqw.dashuyun.cn

[S55] C++：结构化绑定
来源：http://jqz.zhiwuduotai.top

auto [a, b] = std::make_pair(1, 2);
来源：http://pjj.shanyushiyangtech.top

[S56] C++：optional
来源：http://flb.yuxming.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://emh.ywan-chungtsiang.top

[S57] C++：编译期常量
来源：http://wkw.ydzc1.top

constexpr int N = 10;
来源：http://ene.sweek.top

[S58] C++：命名空间
来源：http://zcn.shanyushiyangtech.top

namespace ns { int f() { return 1; } }
来源：http://xad.shangyingyoupin.top

[S59] C++：静态断言
来源：http://bsx.ppjwa.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vmg.yvedp.cn

[S60] C++：遍历并删除元素
来源：http://bhb.sxryk.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://aon.c1oappe.top

================================================================================
来源：http://buz.yj20258.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cyw.yj202588.top

================================================================================
来源：http://fvw.316326.xyz

[T01] Kotlin：Hello World
来源：http://cxo.aibaodan.cn

println("Hello")
来源：http://krd.xinyue.icu

[T02] Kotlin：变量
来源：http://uyw.yonumen.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://luy.epnwcf.com

[T03] Kotlin：字符串模板
来源：http://dad.jinghuilouyu.cn

"值: $b"
来源：http://uby.zhaomingkeji.xyz

[T04] Kotlin：空安全
来源：http://qki.sufxvd.cn

val n: String? = null;  n?.length
来源：http://uky.zhixingplan.top

[T05] Kotlin：when 表达式
来源：http://mow.ydjk.org.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ase.bjfxy.top

[T06] Kotlin：集合映射
来源：http://bfh.sysykeji.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ghz.hysaishi.cn

[T07] Kotlin：集合过滤
来源：http://jsc.birdmap.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://yhs.0kj1m.cn

[T08] Kotlin：数据类
来源：http://zsw.fanxiaobao.xyz

data class User(val name: String, val age: Int)
来源：http://gmu.hnqzz.top

[T09] Kotlin：扩展函数
来源：http://ktk.redwolf501.top

fun String.exclaim() = this + "!"
来源：http://bqd.xuanzx.com

[T10] Kotlin：默认参数
来源：http://pac.zycfv.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://gzm.yueranfly.top

[T11] Kotlin：协程
来源：http://ioz.meibo888.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://feg.sxryk.cn

[T12] Kotlin：解构声明
来源：http://wqp.gaohongyu789.top

val (a, b) = Pair(1, 2)
来源：http://cgd.smart0.xyz

[T13] Kotlin：只读 Map
来源：http://iba.sweek.top

val m = mapOf("a" to 1)
来源：http://kat.daxiang520.top

[T14] Kotlin：循环
来源：http://qop.jlsjyb.cn

for (i in 1..10) println(i)
来源：http://plq.jinghuilouyu.cn

[T15] Kotlin：接口
来源：http://nkm.sweek.top

interface Shape { fun area(): Double }
来源：http://tge.sufxvd.cn

[T16] Swift：Hello World
来源：http://sqn.andypj.xyz

print("Hello")
来源：http://fnr.iojbl.cn

[T17] Swift：变量与常量
来源：http://ccf.zdbjq.cn

var a = 1;  let b = 2
来源：http://srx.jianghu66.top

[T18] Swift：字符串插值
来源：http://vhi.tanke756.top

"值: \(b)"
来源：http://oer.shangyingyoupin.top

[T19] Swift：可选绑定
来源：http://fnn.daria6918.cn

if let n = opt { print(n) }
来源：http://awv.xuetiantiany.cn

[T20] Swift：数组操作
来源：http://kpr.fengsongda.top

var a = [1, 2, 3];  a.append(4)
来源：http://lnw.feifeiyinyue.top

[T21] Swift：遍历
来源：http://gpz.sysykeji.top

for x in a { print(x) }
来源：http://tfc.andypj.xyz

[T22] Swift：字典
来源：http://ynf.ehwqpu.com

var d = ["a": 1];  d["b"] = 2
来源：http://nrr.chenlongwang.top

[T23] Swift：函数
来源：http://cir.pycfn.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gwv.yuanzhike.top

[T24] Swift：闭包
来源：http://xlk.smart0.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://fpl.yanxiufei.cn

[T25] Swift：结构体
来源：http://nwl.sysykeji.top

struct P { var x: Int }
来源：http://zci.uphjek.com

[T26] Swift：类与重写
来源：http://gxl.pengpengdd.cyou

class A: Base { override func f() {} }
来源：http://twm.daxiang520.top

[T27] Swift：错误处理
来源：http://uza.chenzaomai.com

do { try f() } catch { print(error) }
来源：http://dfs.yvedp.cn

[T28] Swift：枚举
来源：http://jil.dianchejie.cn

enum Color { case red, green }
来源：http://aey.ehwqpu.com

[T29] Swift：guard 提前返回
来源：http://uir.sufxvd.cn

guard let x = opt else { return }
来源：http://xxj.haohaochexian.top

[T30] Swift：协议
来源：http://esq.hysaishi.cn

protocol Shape { func area() -> Double }
来源：http://upw.jqgfzy.top

[T31] Lua：Hello World
来源：http://jso.jqgufenzy.top

print("Hello")
来源：http://dqi.vqdsnc.cn

[T32] Lua：局部变量
来源：http://yvp.hongshengwenyu.top

local a = 1
来源：http://ybz.0kj1m.cn

[T33] Lua：表（数组）
来源：http://ijr.ctjpmb.com

local t = {1, 2, 3};  t[4] = 4
来源：http://cwj.xuetiantiany.cn

[T34] Lua：遍历表
来源：http://aid.sufxvd.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://vyk.yj20258.top

[T35] Lua：字典表
来源：http://lvq.nanxuanxn.top

local d = { a = 1 };  d.b = 2
来源：http://cin.xuetiantiany.cn

[T36] Lua：函数
来源：http://kfj.epnwcf.com

function add(a, b) return a + b end
来源：http://xtz.hcnkem.com

[T37] Lua：字符串拼接
来源：http://ibx.daria6918.cn

"a" .. "b"
来源：http://was.hcnkem.com

[T38] Lua：条件
来源：http://ahl.xuanzx.com

if x > 0 then print("正") end
来源：http://hco.quarkkingdee.top

[T39] Lua：模式匹配
来源：http://qwt.shzxlz.cn

string.find(s, "%d+")
来源：http://tcs.birdmap.top

[T40] Lua：元表
来源：http://vrj.xinyue.icu

setmetatable({}, { __index = base })
来源：http://mss.hcnkem.com

[T41] Perl：Hello World
来源：http://wic.yueranfly.top

print "Hello\n";
来源：http://eyx.jinghuilouyu.cn

[T42] Perl：变量类型
来源：http://xcv.yueranfly.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zbn.jinghuilouyu.cn

[T43] Perl：字符串插值
来源：http://kin.nanxuanxn.top

"值: $a"
来源：http://cjo.zhixingplan.top

[T44] Perl：条件
来源：http://iwu.yongpay.top

if ($a > 0) { print "正"; }
来源：http://kzn.chenzaomai.com

[T45] Perl：数组遍历
来源：http://qnb.shuidangran.top

for my $x (@arr) { print $x; }
来源：http://qoe.iojbl.cn

[T46] Perl：哈希操作
来源：http://vrv.shangyingyoupin.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://aga.aizwys.cn

[T47] Perl：正则捕获
来源：http://vjf.chenlongwang.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://cgf.jianghu66.top

[T48] Perl：正则替换
来源：http://zqe.wangshuangyany.cn

$s =~ s/old/new/g;
来源：http://gko.yueranfly.top

[T49] Perl：函数
来源：http://crl.zhiwuduotai.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lvz.shangyingyoupin.top

[T50] Perl：逐行读文件
来源：http://gqa.xingfuxueyuan.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://frw.9152youxi.cn

while (my $line = <$fh>) { print $line; }
来源：http://xpc.meibo888.top

[T51] Scala：Hello World
来源：http://aoq.zdqjudy.top

println("Hello")
来源：http://tan.zycfv.cn

[T52] Scala：变量
来源：http://uiw.ehwqpu.com

val a = 1;  var b = 2
来源：http://oia.shangyingyoupin.top

[T53] Scala：字符串插值
来源：http://eun.smart0.xyz

s"值: $b"
来源：http://kyp.yongpay.top

[T54] Scala：集合映射
来源：http://gij.zhongyouzk.top

List(1, 2, 3).map(_ * 2)
来源：http://ufv.52xcode.cn

[T55] Scala：集合过滤
来源：http://mjr.ppjwa.cn

List(1, 2, 3).filter(_ > 1)
来源：http://cmv.pycfn.com

[T56] Scala：样例类
来源：http://eed.hcnkem.com

case class User(name: String, age: Int)
来源：http://vlb.ybcxt.top

[T57] Scala：模式匹配
来源：http://vof.cashguo.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ary.nwbrower.top

[T58] Scala：函数定义
来源：http://uxt.yvedp.cn

def add(a: Int, b: Int): Int = a + b
来源：http://syp.xuanzx.com

[T59] Scala：循环
来源：http://dtt.mhx1999.top

for (i <- 1 to 10) println(i)
来源：http://xqv.aibaodan.cn

[T60] Scala：折叠
来源：http://osa.meibo888.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://owl.hcnkem.com

================================================================================
来源：http://soi.quarkkingdee.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://puj.hfpthk.cn

================================================================================
来源：http://jnf.vqdsnc.cn

[U01] Py：创建虚拟环境
来源：http://lte.yvedp.cn

python -m venv .venv && source .venv/bin/activate
来源：http://fvz.jinghuilouyu.cn

[U02] Py：导出 / 安装依赖
来源：http://rqj.guannengcc.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hdr.pengpengdd.cyou

[U03] Py：加载 .env 配置
来源：http://mox.guowangkeji.top

from dotenv import load_dotenv; load_dotenv()
来源：http://zvo.hfpthk.cn

[U04] Py：变量调试打印
来源：http://qhh.kuanghao11.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://tqm.xylfe.cn

[U05] Py：列表去重且保序
来源：http://quw.sjlbkw.cn

list(dict.fromkeys(arr))
来源：http://pgv.ydzc1.top

[U06] Py：合并两个字典
来源：http://cke.zhoulong.xyz

{**a, **b}
来源：http://jii.yangfankeji.com

[U07] Py：反转字典键值
来源：http://dqx.shanyushiyangtech.top

{v: k for k, v in d.items()}
来源：http://oyj.chenjidiqi.icu

[U08] Py：展平二维列表
来源：http://zhc.snrcjt.cn

[y for x in nested for y in x]
来源：http://snu.hnxiangtu.top

[U09] Py：字典取最大值的键
来源：http://kor.dashuyun.cn

max(d, key=d.get)
来源：http://yem.cdnleiting.top

[U10] Py：按值排序字典
来源：http://wvp.hesvh.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://iox.yuxming.cn

[U11] Py：生成器表达式
来源：http://meo.gotoacloud.top

(x * 2 for x in arr)
来源：http://aoy.jqgfzy.top

[U12] Py：取出现最多的 3 个元素
来源：http://qzk.quarkkingdee.top

Counter(arr).most_common(3)
来源：http://ryi.hnqzz.top

[U13] Py：固定长度队列
来源：http://ily.gaohongyu789.top

deque(maxlen=10)
来源：http://ftn.fktsv.cn

[U14] Py：分组收集到列表
来源：http://ttt.cdnleiting.top

defaultdict(list)
来源：http://ipn.haohaochexian.top

[U15] Py：高精度计时
来源：http://ust.ybcxt.top

t = time.perf_counter()
来源：http://gck.zhiwuduotai.top

[U16] Py：命令行参数解析
来源：http://tmg.ydjk.org.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ntm.tian-w.cn

[U17] Py：初始化日志
来源：http://tnw.pengpengdd.cyou

logging.basicConfig(level=logging.INFO)
来源：http://whj.hesvh.cn

[U18] Py：预编译正则
来源：http://bwy.gaohongyu789.top

pat = re.compile(r"\d+")
来源：http://yje.svipenyu.cn

[U19] Py：正则替换带回调
来源：http://kav.zhaomingkeji.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://dgs.hcnkem.com

[U20] Py：缓存函数结果
来源：http://wib.feifeiyinyue.top

@functools.lru_cache(maxsize=None)
来源：http://acx.fengsongda.top

[U21] Py：自定义上下文管理器
来源：http://obu.jlsjyb.cn

@contextlib.contextmanager
来源：http://sbq.epnwcf.com

[U22] Py：矩阵转置
来源：http://cud.cucudq.cn

list(zip(*m))
来源：http://jju.chenzaomai.com

[U23] Py：分块读取大文件
来源：http://lnp.ehwqpu.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wpq.epnwcf.com

[U24] Py：路径操作
来源：http://bqb.smart0.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://czl.shuidangran.top

[U25] Py：CSV 按字典读
来源：http://yki.0kj1m.cn

csv.DictReader(f)
来源：http://uma.ywan-chungtsiang.top

[U26] Py：并发下载
来源：http://bxz.xinyue.icu

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qgc.tian-w.cn

[U27] Py：异步 HTTP
来源：http://emz.zhaomingkeji.xyz

aiohttp.ClientSession() 配合 async with
来源：http://zgn.mhx1999.top

[U28] Py：类型别名
来源：http://stj.yj202588.top

UserId = int
来源：http://lpf.hcnkem.com

[U29] Py：属性校验
来源：http://ndn.yfazqb.com

@property 与 @x.setter 配合
来源：http://jfy.haohaochexian.top

[U30] Py：数据类
来源：http://zlt.jinqigufen.top

@dataclass(slots=True)
来源：http://kyw.zhijiandao.cn

[U31] Py：单测
来源：http://svq.gogol.net.cn

python -m pytest -q
来源：http://ncc.ivvv.top

[U32] Py：代码格式化
来源：http://abf.hcnkem.com

ruff format . && ruff check --fix .
来源：http://tze.fehbvm.com

[U33] Py：打包发布
来源：http://krs.vehdjk.com

python -m build  （依赖 pyproject.toml）
来源：http://fym.jinqigufen.top

[U34] Py：判断编码
来源：http://zjz.hesvh.cn

chardet.detect(raw)
来源：http://lpn.sweek.top

[U35] Py：发送邮件
来源：http://bwu.yvedp.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vjg.tian-w.cn

[U36] Py：定时任务
来源：http://jsl.fengsongda.top

schedule.every(10).minutes.do(job)
来源：http://hzo.yj20258888.top

[U37] Py：读写 Excel
来源：http://oyq.cashguo.top

pandas.read_excel / DataFrame.to_excel
来源：http://wxz.jlsjyb.cn

[U38] Py：获取脚本所在目录
来源：http://msr.wangdashe.top

Path(__file__).resolve().parent
来源：http://tag.quarkkingdee.top

[U39] Py：判断是否在交互环境
来源：http://ues.cashguo.top

sys.stdout.isatty()
来源：http://qwy.9152youxi.cn

[U40] Py：打印到标准错误
来源：http://vuk.yonumen.top

print("err", file=sys.stderr)
来源：http://xid.xingfuxueyuan.xyz

[U41] PHP：初始化 Composer 项目
来源：http://ofa.gzhubu.top

composer init;  composer require guzzlehttp/guzzle
来源：http://dho.daxiang520.top

[U42] PHP：PSR-4 自动加载
来源：http://xor.yonumen.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hox.jyoumei.cn

[U43] PHP：声明命名空间
来源：http://swg.52xcode.cn

namespace App\Http;
来源：http://hsw.jinyuanbaomall.cn

[U44] PHP：开启严格类型
来源：http://bmd.bbcook.cn

declare(strict_types=1);
来源：http://rnc.daxiang520.top

[U45] PHP：类型声明与返回类型
来源：http://cfw.yonumen.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://qmc.smart0.xyz

[U46] PHP：可空类型
来源：http://lmo.chenlongwang.top

?string $name = null
来源：http://gpg.jyoumei.cn

[U47] PHP：联合类型
来源：http://pup.daria6918.cn

int|string $id
来源：http://gfi.ybcxt.top

[U48] PHP：纯枚举
来源：http://pot.yonumen.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hip.feifeiyinyue.top

[U49] PHP：只读属性
来源：http://tnn.zycfv.cn

public readonly string $name
来源：http://qcf.fktsv.cn

[U50] PHP：构造器属性提升
来源：http://hpv.yuxming.cn

public function __construct(private int $id) {}
来源：http://mtn.zhongyouzk.top

[U51] PHP：数组解构
来源：http://hpd.fzhhl.top

[$a, $b] = $arr;
来源：http://hvn.yuxming.cn

[U52] PHP：箭头函数
来源：http://orn.hfpthk.cn

$double = fn($x) => $x * 2;
来源：http://lgh.9152youxi.cn

[U53] PHP：空合并运算符
来源：http://arh.smart0.xyz

$v = $a ?? $b ?? "default";
来源：http://zbo.ywan-chungtsiang.top

[U54] PHP：空安全调用
来源：http://zve.xuanzx.com

$obj?->method()
来源：http://owm.yfazqb.com


<!-- 参考信息 -->