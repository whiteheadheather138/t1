代发 wailian999

#include <iostream>
来源：http://mne.uphjek.com

int main() { std::cout << "Hello\n"; }
来源：http://ojy.feifeiyinyue.top

[S32] C++：字符串
来源：http://nke.nwbrower.top

std::string s = "hi";  s += "!";
来源：http://aaw.gaohongyu789.top

[S33] C++：vector 增删
来源：http://krz.yueranfly.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qbl.meibo888.top

[S34] C++：遍历 vector
来源：http://gtl.jqgufenzy.top

for (auto &x : v) { std::cout << x; }
来源：http://lxr.wangdashe.top

[S35] C++：map
来源：http://nso.hfpthk.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ugn.daxiang520.top

[S36] C++：unordered_map
来源：http://zjq.shangyingyoupin.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vth.sxryk.cn

[S37] C++：set
来源：http://alu.mhx1999.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ccw.sxryk.cn

[S38] C++：排序
来源：http://uti.9152youxi.cn

std::sort(v.begin(), v.end());
来源：http://dto.sjlbkw.cn

[S39] C++：自定义比较器排序
来源：http://wge.316326.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wfd.ywan-chungtsiang.top

[S40] C++：查找元素
来源：http://xhf.xingfuxueyuan.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jlf.cdnleiting.top

[S41] C++：类与构造函数
来源：http://yvt.jqgfzy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rlg.hywenlv.cn

[S42] C++：继承与虚函数
来源：http://eoc.svipenyu.cn

class B : public Base { public: void f() override {} };
来源：http://fnc.xziqi.cn

[S43] C++：智能指针
来源：http://pzn.cashguo.top

auto p = std::make_unique<int>(5);
来源：http://otr.shuidangran.top

[S44] C++：引用传参
来源：http://lit.daria6918.cn

void inc(int &x) { ++x; }
来源：http://nne.quarkkingdee.top

[S45] C++：lambda
来源：http://pfy.guowangkeji.top

auto add = [](int a, int b) { return a + b; };
来源：http://bax.zhoulong.xyz

[S46] C++：函数模板
来源：http://cov.zhoulong.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vbm.gaohongyu789.top

[S47] C++：结构化绑定遍历
来源：http://gpc.yangfankeji.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://quc.jiagoushi.top

[S48] C++：逐行读文件
来源：http://uxy.guowangkeji.top

std::ifstream in("a.txt");  std::string line;
来源：http://poh.zdbjq.cn

while (std::getline(in, line)) { }
来源：http://kvc.sufxvd.cn

[S49] C++：写文件
来源：http://bfg.vehdjk.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://njl.yueranfly.top

[S50] C++：格式化数字
来源：http://crc.chenjidiqi.icu

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xgt.xylfe.cn

[S51] C++：显式类型转换
来源：http://ept.cashguo.top

static_cast<double>(a) / b
来源：http://sad.yongpay.top

[S52] C++：const 与 noexcept
来源：http://bja.zhijiandao.cn

int size() const noexcept { return n_; }
来源：http://cdv.gogol.net.cn

[S53] C++：移动语义
来源：http://tnd.cucudq.cn

std::vector<int> w = std::move(v);
来源：http://sel.dashuyun.cn

[S54] C++：异常处理
来源：http://lvd.gzhubu.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ehh.yj20258.top

[S55] C++：结构化绑定
来源：http://mcs.tian-w.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://hez.shanyushiyangkeji.top

[S56] C++：optional
来源：http://vgt.pengpengdd.cyou

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zjt.ywan-chungtsiang.top

[S57] C++：编译期常量
来源：http://inm.zhaomingkeji.xyz

constexpr int N = 10;
来源：http://gxd.316326.xyz

[S58] C++：命名空间
来源：http://wwp.ybcxt.top

namespace ns { int f() { return 1; } }
来源：http://mhk.wangdashe.top

[S59] C++：静态断言
来源：http://wry.zhiwuduotai.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ptv.pycfn.com

[S60] C++：遍历并删除元素
来源：http://fpx.vqdsnc.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://oet.0kj1m.cn

================================================================================
来源：http://ocs.aibaodan.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hzv.uphjek.com

================================================================================
来源：http://lbh.yonumen.top

[T01] Kotlin：Hello World
来源：http://qby.havefunace.top

println("Hello")
来源：http://yhg.zhengqikj.top

[T02] Kotlin：变量
来源：http://wgz.zhengqikj.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dho.yj202588.top

[T03] Kotlin：字符串模板
来源：http://qem.hongshengwenyu.top

"值: $b"
来源：http://fca.xylfe.cn

[T04] Kotlin：空安全
来源：http://kck.pycfn.com

val n: String? = null;  n?.length
来源：http://egp.zhongyouzk.top

[T05] Kotlin：when 表达式
来源：http://yuw.sxryk.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lrg.c1oappe.top

[T06] Kotlin：集合映射
来源：http://swv.yj202588.top

listOf(1, 2, 3).map { it * 2 }
来源：http://bxw.bjfxy.top

[T07] Kotlin：集合过滤
来源：http://kiz.cashguo.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://hhz.jinqigfzy.top

[T08] Kotlin：数据类
来源：http://pck.hnxiangtu.top

data class User(val name: String, val age: Int)
来源：http://vct.jyoumei.cn

[T09] Kotlin：扩展函数
来源：http://lnn.ybcxt.top

fun String.exclaim() = this + "!"
来源：http://olt.ydzc1.top

[T10] Kotlin：默认参数
来源：http://vvb.mhx1999.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ldu.mhx1999.top

[T11] Kotlin：协程
来源：http://rmn.0kj1m.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://dzf.0kj1m.cn

[T12] Kotlin：解构声明
来源：http://rtg.zycfv.cn

val (a, b) = Pair(1, 2)
来源：http://aza.shangyingyoupin.top

[T13] Kotlin：只读 Map
来源：http://poe.chenlongwang.top

val m = mapOf("a" to 1)
来源：http://khw.shuidangran.top

[T14] Kotlin：循环
来源：http://xtv.nanxinkj.top

for (i in 1..10) println(i)
来源：http://hah.c1oappe.top

[T15] Kotlin：接口
来源：http://bqb.pycfn.com

interface Shape { fun area(): Double }
来源：http://pmt.nanxinkj.top

[T16] Swift：Hello World
来源：http://jqt.nwbrower.top

print("Hello")
来源：http://hse.redwolf501.top

[T17] Swift：变量与常量
来源：http://mec.kuanghao11.cn

var a = 1;  let b = 2
来源：http://eek.gaohongyu789.top

[T18] Swift：字符串插值
来源：http://dwb.xinyue.icu

"值: \(b)"
来源：http://hqy.zhengqikj.top

[T19] Swift：可选绑定
来源：http://knc.ybcxt.top

if let n = opt { print(n) }
来源：http://dzt.redwolf501.top

[T20] Swift：数组操作
来源：http://fuo.daxiang520.top

var a = [1, 2, 3];  a.append(4)
来源：http://tjo.guannengcc.top

[T21] Swift：遍历
来源：http://zxx.yueranfly.top

for x in a { print(x) }
来源：http://qba.jinqigufen.top

[T22] Swift：字典
来源：http://trb.fktsv.cn

var d = ["a": 1];  d["b"] = 2
来源：http://pai.andypj.xyz

[T23] Swift：函数
来源：http://tkw.hysaishi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tvn.wangshuangyany.cn

[T24] Swift：闭包
来源：http://hkr.shanyushiyangtech.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://pqb.fktsv.cn

[T25] Swift：结构体
来源：http://ggd.vehdjk.com

struct P { var x: Int }
来源：http://aci.hfpthk.cn

[T26] Swift：类与重写
来源：http://ibv.tarul.cn

class A: Base { override func f() {} }
来源：http://vza.jinghuilouyu.cn

[T27] Swift：错误处理
来源：http://obr.hysaishi.cn

do { try f() } catch { print(error) }
来源：http://vib.jlsjyb.cn

[T28] Swift：枚举
来源：http://ryw.yongpay.top

enum Color { case red, green }
来源：http://vty.yangfankeji.com

[T29] Swift：guard 提前返回
来源：http://ohx.fehbvm.com

guard let x = opt else { return }
来源：http://cbg.ywan-chungtsiang.top

[T30] Swift：协议
来源：http://zcj.hnqzz.top

protocol Shape { func area() -> Double }
来源：http://neu.zhongyouzk.top

[T31] Lua：Hello World
来源：http://mdx.cashguo.top

print("Hello")
来源：http://hmw.yj20258888.top

[T32] Lua：局部变量
来源：http://dtq.jinghuilouyu.cn

local a = 1
来源：http://twi.jinyuanbaomall.cn

[T33] Lua：表（数组）
来源：http://rqi.yvedp.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://pgu.chenzaomai.com

[T34] Lua：遍历表
来源：http://hme.feifeiyinyue.top

for i, v in ipairs(t) do print(i, v) end
来源：http://frf.fktsv.cn

[T35] Lua：字典表
来源：http://ejo.sjlbkw.cn

local d = { a = 1 };  d.b = 2
来源：http://vre.zhixingplan.top

[T36] Lua：函数
来源：http://qro.ydzc1.top

function add(a, b) return a + b end
来源：http://pir.yuanzhike.top

[T37] Lua：字符串拼接
来源：http://jzl.fengsongda.top

"a" .. "b"
来源：http://iwr.shzxlz.cn

[T38] Lua：条件
来源：http://mwh.xuetiantiany.cn

if x > 0 then print("正") end
来源：http://nrj.daxiang520.top

[T39] Lua：模式匹配
来源：http://cza.birdmap.top

string.find(s, "%d+")
来源：http://eww.sufxvd.cn

[T40] Lua：元表
来源：http://owv.jqgufenzy.top

setmetatable({}, { __index = base })
来源：http://qyr.zdqjudy.top

[T41] Perl：Hello World
来源：http://fnn.ehwqpu.com

print "Hello\n";
来源：http://gma.hongshengwenyu.top

[T42] Perl：变量类型
来源：http://hvd.fengsongda.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cse.jqgufenzy.top

[T43] Perl：字符串插值
来源：http://uid.shzxlz.cn

"值: $a"
来源：http://jok.zhijiandao.cn

[T44] Perl：条件
来源：http://tam.epnwcf.com

if ($a > 0) { print "正"; }
来源：http://itg.xylfe.cn

[T45] Perl：数组遍历
来源：http://aww.quarkkingdee.top

for my $x (@arr) { print $x; }
来源：http://yvq.cdnleiting.top

[T46] Perl：哈希操作
来源：http://ftz.bbcook.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cmz.chenzaomai.com

[T47] Perl：正则捕获
来源：http://mci.yfazqb.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://qjq.hcnkem.com

[T48] Perl：正则替换
来源：http://jlc.xuetiantiany.cn

$s =~ s/old/new/g;
来源：http://tzc.c1oappe.top

[T49] Perl：函数
来源：http://gzr.iojbl.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nre.316326.xyz

[T50] Perl：逐行读文件
来源：http://feu.jinyuanbaomall.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://bbv.shangyingyoupin.top

while (my $line = <$fh>) { print $line; }
来源：http://xjb.zhongyouzk.top

[T51] Scala：Hello World
来源：http://qqf.fehbvm.com

println("Hello")
来源：http://rre.yuxming.cn

[T52] Scala：变量
来源：http://emq.havefunace.top

val a = 1;  var b = 2
来源：http://pml.zhongyouzk.top

[T53] Scala：字符串插值
来源：http://wdg.shuidangran.top

s"值: $b"
来源：http://sva.quarkkingdee.top

[T54] Scala：集合映射
来源：http://jdx.sufxvd.cn

List(1, 2, 3).map(_ * 2)
来源：http://ufv.gzhubu.top

[T55] Scala：集合过滤
来源：http://ytg.gotoacloud.top

List(1, 2, 3).filter(_ > 1)
来源：http://nqf.vqdsnc.cn

[T56] Scala：样例类
来源：http://uaq.316326.xyz

case class User(name: String, age: Int)
来源：http://yrv.ydjk.org.cn

[T57] Scala：模式匹配
来源：http://rkm.yonumen.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://qxs.gaohongyu789.top

[T58] Scala：函数定义
来源：http://yyr.ppjwa.cn

def add(a: Int, b: Int): Int = a + b
来源：http://pfg.jinghuilouyu.cn

[T59] Scala：循环
来源：http://kxg.wangshuangyany.cn

for (i <- 1 to 10) println(i)
来源：http://byw.feifeiyinyue.top

[T60] Scala：折叠
来源：http://xbw.zhongyouzk.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://skm.chenlongwang.top

================================================================================
来源：http://tdd.hfpthk.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fks.gogol.net.cn

================================================================================
来源：http://tpq.xziqi.cn

[U01] Py：创建虚拟环境
来源：http://dos.yuxming.cn

python -m venv .venv && source .venv/bin/activate
来源：http://fhp.shanyushiyangtech.top

[U02] Py：导出 / 安装依赖
来源：http://xrv.yj202588.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://twc.tarul.cn

[U03] Py：加载 .env 配置
来源：http://vef.ydzc1.top

from dotenv import load_dotenv; load_dotenv()
来源：http://vaw.jinyuanbaomall.cn

[U04] Py：变量调试打印
来源：http://aho.zhixingplan.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jah.ybcxt.top

[U05] Py：列表去重且保序
来源：http://ytp.nanxinkj.top

list(dict.fromkeys(arr))
来源：http://ean.daxiang520.top

[U06] Py：合并两个字典
来源：http://mxv.zhoulong.xyz

{**a, **b}
来源：http://oyl.sxryk.cn

[U07] Py：反转字典键值
来源：http://rwc.uphjek.com

{v: k for k, v in d.items()}
来源：http://qji.nanxuanxn.top

[U08] Py：展平二维列表
来源：http://dqa.tarul.cn

[y for x in nested for y in x]
来源：http://gaq.sxryk.cn

[U09] Py：字典取最大值的键
来源：http://yaj.snrcjt.cn

max(d, key=d.get)
来源：http://gax.daria6918.cn

[U10] Py：按值排序字典
来源：http://ysw.zhoulong.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://acq.vehdjk.com

[U11] Py：生成器表达式
来源：http://ood.jqgfzy.top

(x * 2 for x in arr)
来源：http://isf.9152youxi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ovy.sweek.top

Counter(arr).most_common(3)
来源：http://zpf.pengpengdd.cyou

[U13] Py：固定长度队列
来源：http://cxc.hongshengwenyu.top

deque(maxlen=10)
来源：http://kka.shangyingyoupin.top

[U14] Py：分组收集到列表
来源：http://lns.9152youxi.cn

defaultdict(list)
来源：http://tge.cdnleiting.top

[U15] Py：高精度计时
来源：http://nsb.9152youxi.cn

t = time.perf_counter()
来源：http://gal.zdbjq.cn

[U16] Py：命令行参数解析
来源：http://sla.xinyue.icu

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://aet.nanxuanxn.top

[U17] Py：初始化日志
来源：http://how.xylfe.cn

logging.basicConfig(level=logging.INFO)
来源：http://uid.feifeiyinyue.top

[U18] Py：预编译正则
来源：http://kst.yonumen.top

pat = re.compile(r"\d+")
来源：http://zwd.fktsv.cn

[U19] Py：正则替换带回调
来源：http://kug.dianchejie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wtw.kuanghao11.cn

[U20] Py：缓存函数结果
来源：http://kqq.jianghu66.top

@functools.lru_cache(maxsize=None)
来源：http://fde.svipenyu.cn

[U21] Py：自定义上下文管理器
来源：http://kse.52xcode.cn

@contextlib.contextmanager
来源：http://rrg.guannengcc.top

[U22] Py：矩阵转置
来源：http://nka.daria6918.cn

list(zip(*m))
来源：http://dnd.sxryk.cn

[U23] Py：分块读取大文件
来源：http://ryk.jyoumei.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://kgc.ywan-chungtsiang.top

[U24] Py：路径操作
来源：http://vbk.birdmap.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jhp.jiagoushi.top

[U25] Py：CSV 按字典读
来源：http://yoj.gaohongyu789.top

csv.DictReader(f)
来源：http://efg.yj20258.top

[U26] Py：并发下载
来源：http://yvf.hesvh.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wrb.pengpengdd.cyou

[U27] Py：异步 HTTP
来源：http://cvj.zdqjudy.top

aiohttp.ClientSession() 配合 async with
来源：http://onj.zhaomingkeji.xyz

[U28] Py：类型别名
来源：http://clu.cheryme.top

UserId = int
来源：http://oic.nwbrower.top

[U29] Py：属性校验
来源：http://oez.yanxiufei.cn

@property 与 @x.setter 配合
来源：http://wbc.cqqwz.cn

[U30] Py：数据类
来源：http://jon.mhx1999.top

@dataclass(slots=True)
来源：http://vdq.gogol.net.cn

[U31] Py：单测
来源：http://vhv.fehbvm.com

python -m pytest -q
来源：http://jrw.ppjwa.cn

[U32] Py：代码格式化
来源：http://nic.jinghuilouyu.cn

ruff format . && ruff check --fix .
来源：http://cfd.andypj.xyz

[U33] Py：打包发布
来源：http://xxb.ivvv.top

python -m build  （依赖 pyproject.toml）
来源：http://zts.ywan-chungtsiang.top

[U34] Py：判断编码
来源：http://yrq.fengsongda.top

chardet.detect(raw)
来源：http://kta.quarkkingdee.top

[U35] Py：发送邮件
来源：http://ylm.ybcxt.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xsr.havefunace.top

[U36] Py：定时任务
来源：http://xyr.nwbrower.top

schedule.every(10).minutes.do(job)
来源：http://xcl.chenjidiqi.icu

[U37] Py：读写 Excel
来源：http://hdo.jinghuilouyu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://jmv.xziqi.cn

[U38] Py：获取脚本所在目录
来源：http://tsf.zhaomingkeji.xyz

Path(__file__).resolve().parent
来源：http://lrg.yangfankeji.com

[U39] Py：判断是否在交互环境
来源：http://gaf.yvedp.cn

sys.stdout.isatty()
来源：http://emo.ybcxt.top

[U40] Py：打印到标准错误
来源：http://drn.bbcook.cn

print("err", file=sys.stderr)
来源：http://ygd.ywan-chungtsiang.top

[U41] PHP：初始化 Composer 项目
来源：http://qfs.iojbl.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://uee.yj202588.top

[U42] PHP：PSR-4 自动加载
来源：http://hyt.bbcook.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ftq.ppjwa.cn

[U43] PHP：声明命名空间
来源：http://wdt.gzhubu.top

namespace App\Http;
来源：http://nma.feifeiyinyue.top

[U44] PHP：开启严格类型
来源：http://kzl.mhx1999.top

declare(strict_types=1);
来源：http://adj.sysykeji.top

[U45] PHP：类型声明与返回类型
来源：http://qnu.ywan-chungtsiang.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://huk.jlsjyb.cn

[U46] PHP：可空类型
来源：http://fvs.cashguo.top

?string $name = null
来源：http://agr.nwbrower.top

[U47] PHP：联合类型
来源：http://par.andypj.xyz

int|string $id
来源：http://snn.quarkkingdee.top

[U48] PHP：纯枚举
来源：http://weu.kuanghao11.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qmz.zdbjq.cn

[U49] PHP：只读属性
来源：http://mce.jyoumei.cn

public readonly string $name
来源：http://alb.chenzaomai.com

[U50] PHP：构造器属性提升
来源：http://fpt.zdbjq.cn

public function __construct(private int $id) {}
来源：http://tcn.bjfxy.top

[U51] PHP：数组解构
来源：http://srt.nanxuanxn.top

[$a, $b] = $arr;
来源：http://bjd.kuanghao11.cn

[U52] PHP：箭头函数
来源：http://gcf.tianlin.xyz

$double = fn($x) => $x * 2;
来源：http://kar.yuxming.cn

[U53] PHP：空合并运算符
来源：http://ivw.yfazqb.com

$v = $a ?? $b ?? "default";
来源：http://jyt.birdmap.top

[U54] PHP：空安全调用
来源：http://soa.aizwys.cn

$obj?->method()
来源：http://jkx.tian-w.cn

[U55] PHP：match 表达式
来源：http://fky.wangdashe.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://uqf.ybcxt.top

[U56] PHP：命名参数
来源：http://fct.yuanzhike.top

f(a: 1, b: 2)
来源：http://itc.zhiwuduotai.top


<!-- 参考信息 -->