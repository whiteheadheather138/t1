代发 wailian999

#include <iostream>
来源：http://okc.chenzaomai.com

int main() { std::cout << "Hello\n"; }
来源：http://bjw.nwbrower.top

[S32] C++：字符串
来源：http://mso.gogol.net.cn

std::string s = "hi";  s += "!";
来源：http://drw.shanyushiyangtech.top

[S33] C++：vector 增删
来源：http://jgp.gaohongyu789.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bsy.nanxinkj.top

[S34] C++：遍历 vector
来源：http://ujk.sxryk.cn

for (auto &x : v) { std::cout << x; }
来源：http://kzx.shuidangran.top

[S35] C++：map
来源：http://zop.cheryme.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://uqi.yvedp.cn

[S36] C++：unordered_map
来源：http://hjw.sxryk.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://otj.xingfuxueyuan.xyz

[S37] C++：set
来源：http://ruj.zhongyouzk.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tby.gzhubu.top

[S38] C++：排序
来源：http://aee.ywan-chungtsiang.top

std::sort(v.begin(), v.end());
来源：http://pck.tianlin.xyz

[S39] C++：自定义比较器排序
来源：http://pdx.yanxiufei.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yce.tanke756.top

[S40] C++：查找元素
来源：http://uqa.shangyingyoupin.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dgp.shanyushiyangkeji.top

[S41] C++：类与构造函数
来源：http://fii.shanyushiyangkeji.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dwt.yj20258888.top

[S42] C++：继承与虚函数
来源：http://wii.xingfuxueyuan.xyz

class B : public Base { public: void f() override {} };
来源：http://nac.daria6918.cn

[S43] C++：智能指针
来源：http://zrb.yvedp.cn

auto p = std::make_unique<int>(5);
来源：http://afm.ydjk.org.cn

[S44] C++：引用传参
来源：http://nat.gaohongyu789.top

void inc(int &x) { ++x; }
来源：http://dvp.yj20258888.top

[S45] C++：lambda
来源：http://iuy.yj20258888.top

auto add = [](int a, int b) { return a + b; };
来源：http://kas.zhixingplan.top

[S46] C++：函数模板
来源：http://xns.cqqwz.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fxk.hesvh.cn

[S47] C++：结构化绑定遍历
来源：http://fdb.fanxiaobao.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://brz.yfazqb.com

[S48] C++：逐行读文件
来源：http://rnd.yj202588.top

std::ifstream in("a.txt");  std::string line;
来源：http://ioo.ctjpmb.com

while (std::getline(in, line)) { }
来源：http://yxx.hnqzz.top

[S49] C++：写文件
来源：http://gik.hammf.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://euf.yueranfly.top

[S50] C++：格式化数字
来源：http://ajf.cashguo.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wpo.hfpthk.cn

[S51] C++：显式类型转换
来源：http://byz.jinqigfzy.top

static_cast<double>(a) / b
来源：http://kqi.zhiwuduotai.top

[S52] C++：const 与 noexcept
来源：http://roe.nwbrower.top

int size() const noexcept { return n_; }
来源：http://ycy.sysykeji.top

[S53] C++：移动语义
来源：http://vgb.chenjidiqi.icu

std::vector<int> w = std::move(v);
来源：http://jqw.zhiwuduotai.top

[S54] C++：异常处理
来源：http://lxe.yanxiufei.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xnj.birdmap.top

[S55] C++：结构化绑定
来源：http://tkr.hesvh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ner.tarul.cn

[S56] C++：optional
来源：http://yrz.hysaishi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jgt.sxryk.cn

[S57] C++：编译期常量
来源：http://lxk.yj20258.top

constexpr int N = 10;
来源：http://zah.ydjk.org.cn

[S58] C++：命名空间
来源：http://cwt.ppjwa.cn

namespace ns { int f() { return 1; } }
来源：http://pmk.ywan-chungtsiang.top

[S59] C++：静态断言
来源：http://vea.yfazqb.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yoj.xylfe.cn

[S60] C++：遍历并删除元素
来源：http://wrh.birdmap.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://awv.cucudq.cn

================================================================================
来源：http://yon.sysykeji.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vmk.fzhhl.top

================================================================================
来源：http://psn.mhx1999.top

[T01] Kotlin：Hello World
来源：http://bbw.hammf.cn

println("Hello")
来源：http://gic.shuidangran.top

[T02] Kotlin：变量
来源：http://drn.9152youxi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qnh.havefunace.top

[T03] Kotlin：字符串模板
来源：http://vhj.c1oappe.top

"值: $b"
来源：http://anp.ydjk.org.cn

[T04] Kotlin：空安全
来源：http://rzr.meibo888.top

val n: String? = null;  n?.length
来源：http://zxq.yuxming.cn

[T05] Kotlin：when 表达式
来源：http://fmm.hnxiangtu.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cdu.jinqigufen.top

[T06] Kotlin：集合映射
来源：http://rcr.jqgfzy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://jnj.sysykeji.top

[T07] Kotlin：集合过滤
来源：http://isc.fzhhl.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://wna.hnxiangtu.top

[T08] Kotlin：数据类
来源：http://znz.gaohongyu789.top

data class User(val name: String, val age: Int)
来源：http://gtk.cqqwz.cn

[T09] Kotlin：扩展函数
来源：http://hdk.52xcode.cn

fun String.exclaim() = this + "!"
来源：http://acx.meibo888.top

[T10] Kotlin：默认参数
来源：http://aji.iojbl.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://sky.zhixingplan.top

[T11] Kotlin：协程
来源：http://vxj.daxiang520.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://rov.jyoumei.cn

[T12] Kotlin：解构声明
来源：http://okm.xuetiantiany.cn

val (a, b) = Pair(1, 2)
来源：http://tey.zycfv.cn

[T13] Kotlin：只读 Map
来源：http://zfa.guannengcc.top

val m = mapOf("a" to 1)
来源：http://vzm.gotoacloud.top

[T14] Kotlin：循环
来源：http://qfg.fzhhl.top

for (i in 1..10) println(i)
来源：http://qrb.nwbrower.top

[T15] Kotlin：接口
来源：http://wli.epnwcf.com

interface Shape { fun area(): Double }
来源：http://sdz.sjlbkw.cn

[T16] Swift：Hello World
来源：http://vli.jianghu66.top

print("Hello")
来源：http://uju.wangshuangyany.cn

[T17] Swift：变量与常量
来源：http://czj.pengpengdd.cyou

var a = 1;  let b = 2
来源：http://aji.zhengqikj.top

[T18] Swift：字符串插值
来源：http://mav.hfpthk.cn

"值: \(b)"
来源：http://ldx.epnwcf.com

[T19] Swift：可选绑定
来源：http://bdb.xingfuxueyuan.xyz

if let n = opt { print(n) }
来源：http://zpb.zhaomingkeji.xyz

[T20] Swift：数组操作
来源：http://xvt.zhoulong.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://sam.xuetiantiany.cn

[T21] Swift：遍历
来源：http://yuc.yuxming.cn

for x in a { print(x) }
来源：http://bhk.guannengcc.top

[T22] Swift：字典
来源：http://pao.guowangkeji.top

var d = ["a": 1];  d["b"] = 2
来源：http://mds.gotoacloud.top

[T23] Swift：函数
来源：http://gzw.daxiang520.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lfr.zhiwuduotai.top

[T24] Swift：闭包
来源：http://euu.nanxuanxn.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://cyr.iojbl.cn

[T25] Swift：结构体
来源：http://por.ybcxt.top

struct P { var x: Int }
来源：http://fei.yvedp.cn

[T26] Swift：类与重写
来源：http://kzg.shzxlz.cn

class A: Base { override func f() {} }
来源：http://tjl.fehbvm.com

[T27] Swift：错误处理
来源：http://mwc.zdqjudy.top

do { try f() } catch { print(error) }
来源：http://kxl.iojbl.cn

[T28] Swift：枚举
来源：http://wjy.aizwys.cn

enum Color { case red, green }
来源：http://kxs.quarkkingdee.top

[T29] Swift：guard 提前返回
来源：http://mvf.iojbl.cn

guard let x = opt else { return }
来源：http://ocl.52xcode.cn

[T30] Swift：协议
来源：http://esn.shangyingyoupin.top

protocol Shape { func area() -> Double }
来源：http://ols.yuxming.cn

[T31] Lua：Hello World
来源：http://aba.meibo888.top

print("Hello")
来源：http://mvu.zhoulong.xyz

[T32] Lua：局部变量
来源：http://kyx.cdnleiting.top

local a = 1
来源：http://jzu.mhx1999.top

[T33] Lua：表（数组）
来源：http://hkv.daria6918.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ezw.chenjidiqi.icu

[T34] Lua：遍历表
来源：http://cnv.daxiang520.top

for i, v in ipairs(t) do print(i, v) end
来源：http://wwb.dashuyun.cn

[T35] Lua：字典表
来源：http://wsd.zycfv.cn

local d = { a = 1 };  d.b = 2
来源：http://owx.yj20258888.top

[T36] Lua：函数
来源：http://ivf.jinqigfzy.top

function add(a, b) return a + b end
来源：http://eib.jinqigufen.top

[T37] Lua：字符串拼接
来源：http://lmq.yj20258888.top

"a" .. "b"
来源：http://pez.zhiwuduotai.top

[T38] Lua：条件
来源：http://uzv.ehwqpu.com

if x > 0 then print("正") end
来源：http://fmh.dashuyun.cn

[T39] Lua：模式匹配
来源：http://zow.tianlin.xyz

string.find(s, "%d+")
来源：http://wif.gotoacloud.top

[T40] Lua：元表
来源：http://vzy.jinqigufen.top

setmetatable({}, { __index = base })
来源：http://wxr.fanxiaobao.xyz

[T41] Perl：Hello World
来源：http://mus.zhijiandao.cn

print "Hello\n";
来源：http://uao.316326.xyz

[T42] Perl：变量类型
来源：http://myt.sysykeji.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fub.yanxiufei.cn

[T43] Perl：字符串插值
来源：http://osv.ctjpmb.com

"值: $a"
来源：http://jsl.gaohongyu789.top

[T44] Perl：条件
来源：http://ahk.ctjpmb.com

if ($a > 0) { print "正"; }
来源：http://byu.cqqwz.cn

[T45] Perl：数组遍历
来源：http://mtj.fanxiaobao.xyz

for my $x (@arr) { print $x; }
来源：http://irg.jqgfzy.top

[T46] Perl：哈希操作
来源：http://qdc.jlsjyb.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nbn.zycfv.cn

[T47] Perl：正则捕获
来源：http://cvv.gotoacloud.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://bov.wangdashe.top

[T48] Perl：正则替换
来源：http://ivy.sxryk.cn

$s =~ s/old/new/g;
来源：http://mln.dashuyun.cn

[T49] Perl：函数
来源：http://xwc.tarul.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ytt.yangfankeji.com

[T50] Perl：逐行读文件
来源：http://ljc.guowangkeji.top

open my $fh, "<", "a.txt" or die $!;
来源：http://fse.mhx1999.top

while (my $line = <$fh>) { print $line; }
来源：http://czx.andypj.xyz

[T51] Scala：Hello World
来源：http://ovw.ydzc1.top

println("Hello")
来源：http://uwq.aizwys.cn

[T52] Scala：变量
来源：http://aea.epnwcf.com

val a = 1;  var b = 2
来源：http://wkb.mhx1999.top

[T53] Scala：字符串插值
来源：http://ded.yangfankeji.com

s"值: $b"
来源：http://mup.birdmap.top

[T54] Scala：集合映射
来源：http://vhi.wangdashe.top

List(1, 2, 3).map(_ * 2)
来源：http://vge.guannengcc.top

[T55] Scala：集合过滤
来源：http://yox.zhiwuduotai.top

List(1, 2, 3).filter(_ > 1)
来源：http://amk.chenzaomai.com

[T56] Scala：样例类
来源：http://xfc.yfazqb.com

case class User(name: String, age: Int)
来源：http://mla.jqgufenzy.top

[T57] Scala：模式匹配
来源：http://tsa.ybcxt.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ubw.cheryme.top

[T58] Scala：函数定义
来源：http://szm.yongpay.top

def add(a: Int, b: Int): Int = a + b
来源：http://ldg.hongshengwenyu.top

[T59] Scala：循环
来源：http://emo.iojbl.cn

for (i <- 1 to 10) println(i)
来源：http://hhp.meibo888.top

[T60] Scala：折叠
来源：http://qbz.cheryme.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bgp.ppjwa.cn

================================================================================
来源：http://ies.ybcxt.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mdo.chenlongwang.top

================================================================================
来源：http://cmq.epnwcf.com

[U01] Py：创建虚拟环境
来源：http://lno.birdmap.top

python -m venv .venv && source .venv/bin/activate
来源：http://qhg.zhiwuduotai.top

[U02] Py：导出 / 安装依赖
来源：http://pqo.zycfv.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ihs.epnwcf.com

[U03] Py：加载 .env 配置
来源：http://syh.jinqigfzy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://sit.yangfankeji.com

[U04] Py：变量调试打印
来源：http://bxr.hnxiangtu.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vbd.tanke756.top

[U05] Py：列表去重且保序
来源：http://kvd.zhengqikj.top

list(dict.fromkeys(arr))
来源：http://wdm.jqgufenzy.top

[U06] Py：合并两个字典
来源：http://cke.ehwqpu.com

{**a, **b}
来源：http://sba.gaohongyu789.top

[U07] Py：反转字典键值
来源：http://toq.quarkkingdee.top

{v: k for k, v in d.items()}
来源：http://xld.bjfxy.top

[U08] Py：展平二维列表
来源：http://fmb.quarkkingdee.top

[y for x in nested for y in x]
来源：http://oov.yj202588.top

[U09] Py：字典取最大值的键
来源：http://wcl.hcnkem.com

max(d, key=d.get)
来源：http://una.jinghuilouyu.cn

[U10] Py：按值排序字典
来源：http://hep.daria6918.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zpi.yj20258.top

[U11] Py：生成器表达式
来源：http://dyx.jiagoushi.top

(x * 2 for x in arr)
来源：http://iog.gogol.net.cn

[U12] Py：取出现最多的 3 个元素
来源：http://vti.ctjpmb.com

Counter(arr).most_common(3)
来源：http://pka.zycfv.cn

[U13] Py：固定长度队列
来源：http://lrc.zhengqikj.top

deque(maxlen=10)
来源：http://tay.fktsv.cn

[U14] Py：分组收集到列表
来源：http://xye.wangdashe.top

defaultdict(list)
来源：http://ftv.jinghuilouyu.cn

[U15] Py：高精度计时
来源：http://njb.haohaochexian.top

t = time.perf_counter()
来源：http://vqa.yanxiufei.cn

[U16] Py：命令行参数解析
来源：http://itv.nwbrower.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://iwz.cqqwz.cn

[U17] Py：初始化日志
来源：http://asn.xuanzx.com

logging.basicConfig(level=logging.INFO)
来源：http://nus.c1oappe.top

[U18] Py：预编译正则
来源：http://bgu.zhixingplan.top

pat = re.compile(r"\d+")
来源：http://rgx.ydzc1.top

[U19] Py：正则替换带回调
来源：http://tqm.zhoulong.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kzb.shanyushiyangtech.top

[U20] Py：缓存函数结果
来源：http://jri.aibaodan.cn

@functools.lru_cache(maxsize=None)
来源：http://mhi.shanyushiyangkeji.top

[U21] Py：自定义上下文管理器
来源：http://ogk.yanxiufei.cn

@contextlib.contextmanager
来源：http://obd.andypj.xyz

[U22] Py：矩阵转置
来源：http://wgv.fengsongda.top

list(zip(*m))
来源：http://dua.feifeiyinyue.top

[U23] Py：分块读取大文件
来源：http://get.aibaodan.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lod.yongpay.top

[U24] Py：路径操作
来源：http://cii.andypj.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dyy.ivvv.top

[U25] Py：CSV 按字典读
来源：http://siz.hongshengwenyu.top

csv.DictReader(f)
来源：http://xec.yueranfly.top

[U26] Py：并发下载
来源：http://ren.bjfxy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://njp.zhiwuduotai.top

[U27] Py：异步 HTTP
来源：http://bmj.tarul.cn

aiohttp.ClientSession() 配合 async with
来源：http://kvz.hammf.cn

[U28] Py：类型别名
来源：http://axj.nanxinkj.top

UserId = int
来源：http://kqf.cheryme.top

[U29] Py：属性校验
来源：http://ewd.ivvv.top

@property 与 @x.setter 配合
来源：http://mwc.zdqjudy.top

[U30] Py：数据类
来源：http://zpf.jinqigufen.top

@dataclass(slots=True)
来源：http://mrj.chenjidiqi.icu

[U31] Py：单测
来源：http://jzi.xingfuxueyuan.xyz

python -m pytest -q
来源：http://fxh.feifeiyinyue.top

[U32] Py：代码格式化
来源：http://vpd.pengpengdd.cyou

ruff format . && ruff check --fix .
来源：http://peh.ehwqpu.com

[U33] Py：打包发布
来源：http://djv.sysykeji.top

python -m build  （依赖 pyproject.toml）
来源：http://ekb.cashguo.top

[U34] Py：判断编码
来源：http://hor.daxiang520.top

chardet.detect(raw)
来源：http://seq.fanxiaobao.xyz

[U35] Py：发送邮件
来源：http://yez.shuidangran.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gtd.sjlbkw.cn

[U36] Py：定时任务
来源：http://rhe.jiagoushi.top

schedule.every(10).minutes.do(job)
来源：http://oek.zdqjudy.top

[U37] Py：读写 Excel
来源：http://szg.zdqjudy.top

pandas.read_excel / DataFrame.to_excel
来源：http://qnr.fzhhl.top

[U38] Py：获取脚本所在目录
来源：http://szj.gotoacloud.top

Path(__file__).resolve().parent
来源：http://kct.sxryk.cn

[U39] Py：判断是否在交互环境
来源：http://hpw.jyoumei.cn

sys.stdout.isatty()
来源：http://fex.aizwys.cn

[U40] Py：打印到标准错误
来源：http://cpn.bbcook.cn

print("err", file=sys.stderr)
来源：http://sye.ydzc1.top

[U41] PHP：初始化 Composer 项目
来源：http://wcd.gzhubu.top

composer init;  composer require guzzlehttp/guzzle
来源：http://vee.xingfuxueyuan.xyz

[U42] PHP：PSR-4 自动加载
来源：http://enn.fktsv.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://eas.jinyuanbaomall.cn

[U43] PHP：声明命名空间
来源：http://lhr.yangfankeji.com

namespace App\Http;
来源：http://mez.yuanzhike.top

[U44] PHP：开启严格类型
来源：http://kib.zdbjq.cn

declare(strict_types=1);
来源：http://uue.cucudq.cn

[U45] PHP：类型声明与返回类型
来源：http://kgu.xuanzx.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://xoh.yangfankeji.com

[U46] PHP：可空类型
来源：http://mmy.chenlongwang.top

?string $name = null
来源：http://mwh.jinghuilouyu.cn

[U47] PHP：联合类型
来源：http://dqq.ydzc1.top

int|string $id
来源：http://tol.zhoulong.xyz

[U48] PHP：纯枚举
来源：http://rfd.hysaishi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jmd.daxiang520.top

[U49] PHP：只读属性
来源：http://jbk.yueranfly.top

public readonly string $name
来源：http://syz.zhengqikj.top

[U50] PHP：构造器属性提升
来源：http://emh.guannengcc.top

public function __construct(private int $id) {}
来源：http://mse.c1oappe.top

[U51] PHP：数组解构
来源：http://rda.yuanzhike.top

[$a, $b] = $arr;
来源：http://fqs.chenjidiqi.icu

[U52] PHP：箭头函数
来源：http://drn.quarkkingdee.top

$double = fn($x) => $x * 2;
来源：http://hrh.snrcjt.cn

[U53] PHP：空合并运算符
来源：http://bce.svipenyu.cn

$v = $a ?? $b ?? "default";
来源：http://cvv.ivvv.top

[U54] PHP：空安全调用
来源：http://msq.daria6918.cn

$obj?->method()
来源：http://eye.fktsv.cn

[U55] PHP：match 表达式
来源：http://ome.shanyushiyangkeji.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rng.vehdjk.com

[U56] PHP：命名参数
来源：http://axa.nanxuanxn.top

f(a: 1, b: 2)
来源：http://rin.ehwqpu.com


<!-- 参考信息 -->