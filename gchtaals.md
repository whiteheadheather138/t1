代发 wailian999

static int counter = 0;
来源：http://yfc.bjfxy.top

[S29] C：变参函数
来源：http://zii.c1oappe.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rkq.cashguo.top

[S30] C：头文件保护
来源：http://tdd.aibaodan.cn

#ifndef X_H
来源：http://vob.shanyushiyangkeji.top

#define X_H
来源：http://gaf.pycfn.com

#endif
来源：http://gck.pycfn.com

[S31] C++：Hello World
来源：http://jjb.shangyingyoupin.top

#include <iostream>
来源：http://nqd.yj20258.top

int main() { std::cout << "Hello\n"; }
来源：http://zal.redwolf501.top

[S32] C++：字符串
来源：http://acu.fanxiaobao.xyz

std::string s = "hi";  s += "!";
来源：http://cdu.ydjk.org.cn

[S33] C++：vector 增删
来源：http://iru.yfazqb.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rou.316326.xyz

[S34] C++：遍历 vector
来源：http://szv.jinyuanbaomall.cn

for (auto &x : v) { std::cout << x; }
来源：http://zkw.ehwqpu.com

[S35] C++：map
来源：http://tdx.xziqi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://uqr.ctjpmb.com

[S36] C++：unordered_map
来源：http://ddw.ehwqpu.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vsw.svipenyu.cn

[S37] C++：set
来源：http://ecj.yj20258888.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kjo.aizwys.cn

[S38] C++：排序
来源：http://osc.sweek.top

std::sort(v.begin(), v.end());
来源：http://onq.shzxlz.cn

[S39] C++：自定义比较器排序
来源：http://uqr.hcnkem.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rdo.cheryme.top

[S40] C++：查找元素
来源：http://ahe.dashuyun.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://olu.zdqjudy.top

[S41] C++：类与构造函数
来源：http://lqr.yuanzhike.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://osu.sweek.top

[S42] C++：继承与虚函数
来源：http://tll.jinyuanbaomall.cn

class B : public Base { public: void f() override {} };
来源：http://gmz.redwolf501.top

[S43] C++：智能指针
来源：http://fvd.havefunace.top

auto p = std::make_unique<int>(5);
来源：http://imk.jinqigfzy.top

[S44] C++：引用传参
来源：http://thd.snrcjt.cn

void inc(int &x) { ++x; }
来源：http://yvb.gaohongyu789.top

[S45] C++：lambda
来源：http://vwy.wangshuangyany.cn

auto add = [](int a, int b) { return a + b; };
来源：http://lri.jinqigfzy.top

[S46] C++：函数模板
来源：http://lod.jinghuilouyu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zub.gogol.net.cn

[S47] C++：结构化绑定遍历
来源：http://cft.fzhhl.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ztu.ybcxt.top

[S48] C++：逐行读文件
来源：http://sye.c1oappe.top

std::ifstream in("a.txt");  std::string line;
来源：http://zfd.ppjwa.cn

while (std::getline(in, line)) { }
来源：http://qgn.hfpthk.cn

[S49] C++：写文件
来源：http://rfg.shanyushiyangkeji.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xqr.zycfv.cn

[S50] C++：格式化数字
来源：http://fwh.jinqigfzy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wam.feifeiyinyue.top

[S51] C++：显式类型转换
来源：http://fjj.wangdashe.top

static_cast<double>(a) / b
来源：http://oab.ybcxt.top

[S52] C++：const 与 noexcept
来源：http://bgd.quarkkingdee.top

int size() const noexcept { return n_; }
来源：http://fgm.sweek.top

[S53] C++：移动语义
来源：http://gmu.aizwys.cn

std::vector<int> w = std::move(v);
来源：http://zvm.xylfe.cn

[S54] C++：异常处理
来源：http://fik.aizwys.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bug.yueranfly.top

[S55] C++：结构化绑定
来源：http://rnf.cqqwz.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://mkg.zhiwuduotai.top

[S56] C++：optional
来源：http://iia.havefunace.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rhn.yonumen.top

[S57] C++：编译期常量
来源：http://jfn.uphjek.com

constexpr int N = 10;
来源：http://nmd.ybcxt.top

[S58] C++：命名空间
来源：http://fuk.birdmap.top

namespace ns { int f() { return 1; } }
来源：http://mjx.cucudq.cn

[S59] C++：静态断言
来源：http://ebs.cheryme.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zaf.jiagoushi.top

[S60] C++：遍历并删除元素
来源：http://fms.sweek.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vmx.nwbrower.top

================================================================================
来源：http://wts.meibo888.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://emb.svipenyu.cn

================================================================================
来源：http://xdc.xingfuxueyuan.xyz

[T01] Kotlin：Hello World
来源：http://ddv.xylfe.cn

println("Hello")
来源：http://efc.epnwcf.com

[T02] Kotlin：变量
来源：http://frn.yvedp.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cgw.ivvv.top

[T03] Kotlin：字符串模板
来源：http://xue.jinyuanbaomall.cn

"值: $b"
来源：http://kwg.shzxlz.cn

[T04] Kotlin：空安全
来源：http://ugh.nwbrower.top

val n: String? = null;  n?.length
来源：http://bdn.hfpthk.cn

[T05] Kotlin：when 表达式
来源：http://ijm.yuanzhike.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nti.yfazqb.com

[T06] Kotlin：集合映射
来源：http://kfa.9152youxi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://pki.tianlin.xyz

[T07] Kotlin：集合过滤
来源：http://mep.zdbjq.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://fbe.zhixingplan.top

[T08] Kotlin：数据类
来源：http://vzp.kuanghao11.cn

data class User(val name: String, val age: Int)
来源：http://mdm.xuanzx.com

[T09] Kotlin：扩展函数
来源：http://sqj.ywan-chungtsiang.top

fun String.exclaim() = this + "!"
来源：http://ttg.sjlbkw.cn

[T10] Kotlin：默认参数
来源：http://wos.chenjidiqi.icu

fun greet(name: String = "World") = "Hi $name"
来源：http://blo.zdbjq.cn

[T11] Kotlin：协程
来源：http://cbs.smart0.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://voc.fzhhl.top

[T12] Kotlin：解构声明
来源：http://ocn.shanyushiyangkeji.top

val (a, b) = Pair(1, 2)
来源：http://fea.zhongyouzk.top

[T13] Kotlin：只读 Map
来源：http://brb.zhijiandao.cn

val m = mapOf("a" to 1)
来源：http://nvj.hesvh.cn

[T14] Kotlin：循环
来源：http://zso.hammf.cn

for (i in 1..10) println(i)
来源：http://tlu.316326.xyz

[T15] Kotlin：接口
来源：http://vbu.shangyingyoupin.top

interface Shape { fun area(): Double }
来源：http://qyj.aibaodan.cn

[T16] Swift：Hello World
来源：http://urc.pycfn.com

print("Hello")
来源：http://bqc.vqdsnc.cn

[T17] Swift：变量与常量
来源：http://ojk.ehwqpu.com

var a = 1;  let b = 2
来源：http://hzr.fehbvm.com

[T18] Swift：字符串插值
来源：http://vpk.ydzc1.top

"值: \(b)"
来源：http://jxm.zhijiandao.cn

[T19] Swift：可选绑定
来源：http://hxk.fehbvm.com

if let n = opt { print(n) }
来源：http://enh.yanxiufei.cn

[T20] Swift：数组操作
来源：http://nte.yfazqb.com

var a = [1, 2, 3];  a.append(4)
来源：http://tuy.chenjidiqi.icu

[T21] Swift：遍历
来源：http://jnu.jlsjyb.cn

for x in a { print(x) }
来源：http://oqn.pycfn.com

[T22] Swift：字典
来源：http://obd.shzxlz.cn

var d = ["a": 1];  d["b"] = 2
来源：http://dcd.zhoulong.xyz

[T23] Swift：函数
来源：http://zdn.cqqwz.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nrh.xziqi.cn

[T24] Swift：闭包
来源：http://ofb.hongshengwenyu.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://mct.redwolf501.top

[T25] Swift：结构体
来源：http://uos.sxryk.cn

struct P { var x: Int }
来源：http://yun.jyoumei.cn

[T26] Swift：类与重写
来源：http://woc.mhx1999.top

class A: Base { override func f() {} }
来源：http://zag.zhoulong.xyz

[T27] Swift：错误处理
来源：http://asj.hnxiangtu.top

do { try f() } catch { print(error) }
来源：http://oca.ybcxt.top

[T28] Swift：枚举
来源：http://jpq.ctjpmb.com

enum Color { case red, green }
来源：http://quu.mhx1999.top

[T29] Swift：guard 提前返回
来源：http://nhn.tarul.cn

guard let x = opt else { return }
来源：http://ggm.nanxuanxn.top

[T30] Swift：协议
来源：http://rhe.jinyuanbaomall.cn

protocol Shape { func area() -> Double }
来源：http://wfj.fehbvm.com

[T31] Lua：Hello World
来源：http://ccl.fzhhl.top

print("Hello")
来源：http://uat.shzxlz.cn

[T32] Lua：局部变量
来源：http://ppy.guowangkeji.top

local a = 1
来源：http://frt.jinyuanbaomall.cn

[T33] Lua：表（数组）
来源：http://jsg.jinghuilouyu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://guo.jyoumei.cn

[T34] Lua：遍历表
来源：http://irf.sxryk.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://jxu.zhoulong.xyz

[T35] Lua：字典表
来源：http://rky.tarul.cn

local d = { a = 1 };  d.b = 2
来源：http://bfv.fktsv.cn

[T36] Lua：函数
来源：http://odb.hammf.cn

function add(a, b) return a + b end
来源：http://mya.meibo888.top

[T37] Lua：字符串拼接
来源：http://puv.yj202588.top

"a" .. "b"
来源：http://dtj.vqdsnc.cn

[T38] Lua：条件
来源：http://jeb.vqdsnc.cn

if x > 0 then print("正") end
来源：http://xdy.xinyue.icu

[T39] Lua：模式匹配
来源：http://rxq.chenjidiqi.icu

string.find(s, "%d+")
来源：http://zuz.bjfxy.top

[T40] Lua：元表
来源：http://pwp.cqqwz.cn

setmetatable({}, { __index = base })
来源：http://fdr.ywan-chungtsiang.top

[T41] Perl：Hello World
来源：http://kgf.0kj1m.cn

print "Hello\n";
来源：http://hkz.jinqigfzy.top

[T42] Perl：变量类型
来源：http://ymr.cucudq.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rtf.ctjpmb.com

[T43] Perl：字符串插值
来源：http://klf.xinyue.icu

"值: $a"
来源：http://our.jinqigfzy.top

[T44] Perl：条件
来源：http://nij.c1oappe.top

if ($a > 0) { print "正"; }
来源：http://wov.zdqjudy.top

[T45] Perl：数组遍历
来源：http://mwt.sxryk.cn

for my $x (@arr) { print $x; }
来源：http://sai.sysykeji.top

[T46] Perl：哈希操作
来源：http://dfj.fzhhl.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xzz.gaohongyu789.top

[T47] Perl：正则捕获
来源：http://zjo.yj202588.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://uoq.uphjek.com

[T48] Perl：正则替换
来源：http://xce.zhaomingkeji.xyz

$s =~ s/old/new/g;
来源：http://cmf.zhijiandao.cn

[T49] Perl：函数
来源：http://ewu.birdmap.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qvd.ppjwa.cn

[T50] Perl：逐行读文件
来源：http://qsz.vehdjk.com

open my $fh, "<", "a.txt" or die $!;
来源：http://zsi.iojbl.cn

while (my $line = <$fh>) { print $line; }
来源：http://zgj.haohaochexian.top

[T51] Scala：Hello World
来源：http://jxh.bbcook.cn

println("Hello")
来源：http://uvw.pycfn.com

[T52] Scala：变量
来源：http://zix.pengpengdd.cyou

val a = 1;  var b = 2
来源：http://gqr.cdnleiting.top

[T53] Scala：字符串插值
来源：http://rss.nwbrower.top

s"值: $b"
来源：http://uyw.shangyingyoupin.top

[T54] Scala：集合映射
来源：http://gus.zhoulong.xyz

List(1, 2, 3).map(_ * 2)
来源：http://mok.ctjpmb.com

[T55] Scala：集合过滤
来源：http://wpn.sufxvd.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ahb.xylfe.cn

[T56] Scala：样例类
来源：http://nkb.fehbvm.com

case class User(name: String, age: Int)
来源：http://jsf.ybcxt.top

[T57] Scala：模式匹配
来源：http://abm.hongshengwenyu.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://vgu.hfpthk.cn

[T58] Scala：函数定义
来源：http://tkm.yfazqb.com

def add(a: Int, b: Int): Int = a + b
来源：http://mmt.svipenyu.cn

[T59] Scala：循环
来源：http://xdt.uphjek.com

for (i <- 1 to 10) println(i)
来源：http://kei.yj20258.top

[T60] Scala：折叠
来源：http://ozt.zhongyouzk.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fkd.yangfankeji.com

================================================================================
来源：http://mvg.jiagoushi.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jml.zhixingplan.top

================================================================================
来源：http://rid.hongshengwenyu.top

[U01] Py：创建虚拟环境
来源：http://qms.hywenlv.cn

python -m venv .venv && source .venv/bin/activate
来源：http://kfj.jqgufenzy.top

[U02] Py：导出 / 安装依赖
来源：http://hdw.ppjwa.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fca.yuanzhike.top

[U03] Py：加载 .env 配置
来源：http://uqt.ppjwa.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://lkd.jinghuilouyu.cn

[U04] Py：变量调试打印
来源：http://uql.yangfankeji.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://snz.yuanzhike.top

[U05] Py：列表去重且保序
来源：http://jlv.zdbjq.cn

list(dict.fromkeys(arr))
来源：http://dnw.hywenlv.cn

[U06] Py：合并两个字典
来源：http://bbf.gaohongyu789.top

{**a, **b}
来源：http://vfz.gaohongyu789.top

[U07] Py：反转字典键值
来源：http://vcf.hywenlv.cn

{v: k for k, v in d.items()}
来源：http://scr.yanxiufei.cn

[U08] Py：展平二维列表
来源：http://fve.daria6918.cn

[y for x in nested for y in x]
来源：http://jzu.fktsv.cn

[U09] Py：字典取最大值的键
来源：http://qsk.vqdsnc.cn

max(d, key=d.get)
来源：http://qwh.xziqi.cn

[U10] Py：按值排序字典
来源：http://zwn.redwolf501.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rmh.vqdsnc.cn

[U11] Py：生成器表达式
来源：http://kjk.cashguo.top

(x * 2 for x in arr)
来源：http://auu.xingfuxueyuan.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://cvq.chenzaomai.com

Counter(arr).most_common(3)
来源：http://gad.nwbrower.top

[U13] Py：固定长度队列
来源：http://qyl.aibaodan.cn

deque(maxlen=10)
来源：http://xlz.epnwcf.com

[U14] Py：分组收集到列表
来源：http://bnp.haohaochexian.top

defaultdict(list)
来源：http://nyb.shanyushiyangkeji.top

[U15] Py：高精度计时
来源：http://uyx.ppjwa.cn

t = time.perf_counter()
来源：http://ngy.yuxming.cn

[U16] Py：命令行参数解析
来源：http://sbl.hysaishi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vka.cucudq.cn

[U17] Py：初始化日志
来源：http://jzr.mhx1999.top

logging.basicConfig(level=logging.INFO)
来源：http://iey.fanxiaobao.xyz

[U18] Py：预编译正则
来源：http://ryl.sufxvd.cn

pat = re.compile(r"\d+")
来源：http://vvj.gogol.net.cn

[U19] Py：正则替换带回调
来源：http://qit.zhixingplan.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bth.daria6918.cn

[U20] Py：缓存函数结果
来源：http://kaf.hammf.cn

@functools.lru_cache(maxsize=None)
来源：http://cxs.jlsjyb.cn

[U21] Py：自定义上下文管理器
来源：http://bss.dashuyun.cn

@contextlib.contextmanager
来源：http://fsf.jqgufenzy.top

[U22] Py：矩阵转置
来源：http://cbq.fktsv.cn

list(zip(*m))
来源：http://wzk.yueranfly.top

[U23] Py：分块读取大文件
来源：http://jpf.wangshuangyany.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://epn.chenjidiqi.icu

[U24] Py：路径操作
来源：http://jqt.gotoacloud.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ddv.aizwys.cn

[U25] Py：CSV 按字典读
来源：http://ode.guannengcc.top

csv.DictReader(f)
来源：http://muq.zhaomingkeji.xyz

[U26] Py：并发下载
来源：http://kqj.shuidangran.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nqc.xingfuxueyuan.xyz

[U27] Py：异步 HTTP
来源：http://zhz.tianlin.xyz

aiohttp.ClientSession() 配合 async with
来源：http://hrq.ywan-chungtsiang.top

[U28] Py：类型别名
来源：http://vim.yongpay.top

UserId = int
来源：http://eaf.fzhhl.top

[U29] Py：属性校验
来源：http://hai.xuanzx.com

@property 与 @x.setter 配合
来源：http://qol.fengsongda.top

[U30] Py：数据类
来源：http://olr.yuxming.cn

@dataclass(slots=True)
来源：http://rpr.ybcxt.top

[U31] Py：单测
来源：http://jyc.hywenlv.cn

python -m pytest -q
来源：http://vwx.ppjwa.cn

[U32] Py：代码格式化
来源：http://onu.gaohongyu789.top

ruff format . && ruff check --fix .
来源：http://tmf.havefunace.top

[U33] Py：打包发布
来源：http://tmx.jinyuanbaomall.cn

python -m build  （依赖 pyproject.toml）
来源：http://ivb.c1oappe.top

[U34] Py：判断编码
来源：http://ums.shzxlz.cn

chardet.detect(raw)
来源：http://xxy.jqgfzy.top

[U35] Py：发送邮件
来源：http://lbf.nwbrower.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xdb.sufxvd.cn

[U36] Py：定时任务
来源：http://hlk.vqdsnc.cn

schedule.every(10).minutes.do(job)
来源：http://ryy.jqgufenzy.top

[U37] Py：读写 Excel
来源：http://sjm.hongshengwenyu.top

pandas.read_excel / DataFrame.to_excel
来源：http://vxr.hysaishi.cn

[U38] Py：获取脚本所在目录
来源：http://ceg.jinghuilouyu.cn

Path(__file__).resolve().parent
来源：http://clf.kuanghao11.cn

[U39] Py：判断是否在交互环境
来源：http://nel.cucudq.cn

sys.stdout.isatty()
来源：http://kja.jqgfzy.top

[U40] Py：打印到标准错误
来源：http://rgh.jqgufenzy.top

print("err", file=sys.stderr)
来源：http://kev.nanxinkj.top

[U41] PHP：初始化 Composer 项目
来源：http://asg.jiagoushi.top

composer init;  composer require guzzlehttp/guzzle
来源：http://rbp.jqgfzy.top

[U42] PHP：PSR-4 自动加载
来源：http://psu.andypj.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cms.ywan-chungtsiang.top

[U43] PHP：声明命名空间
来源：http://ypg.wangshuangyany.cn

namespace App\Http;
来源：http://ipw.shangyingyoupin.top

[U44] PHP：开启严格类型
来源：http://yvu.ivvv.top

declare(strict_types=1);
来源：http://tmv.sjlbkw.cn

[U45] PHP：类型声明与返回类型
来源：http://cay.yongpay.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://uoz.wangshuangyany.cn

[U46] PHP：可空类型
来源：http://gli.epnwcf.com

?string $name = null
来源：http://ijs.epnwcf.com

[U47] PHP：联合类型
来源：http://zfp.cqqwz.cn

int|string $id
来源：http://now.xingfuxueyuan.xyz

[U48] PHP：纯枚举
来源：http://tpw.nanxinkj.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ast.gaohongyu789.top

[U49] PHP：只读属性
来源：http://wdz.sysykeji.top

public readonly string $name
来源：http://wqd.cheryme.top

[U50] PHP：构造器属性提升
来源：http://vaa.daria6918.cn

public function __construct(private int $id) {}
来源：http://bgd.daria6918.cn

[U51] PHP：数组解构
来源：http://mse.fzhhl.top

[$a, $b] = $arr;
来源：http://lde.xuanzx.com

[U52] PHP：箭头函数
来源：http://jct.cucudq.cn

$double = fn($x) => $x * 2;
来源：http://wem.sxryk.cn


<!-- 参考信息 -->