代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://axg.nwbrower.top

[S25] C：内存拷贝
来源：http://qyr.xingfuxueyuan.xyz

memcpy(dst, src, n);
来源：http://qwg.chenlongwang.top

[S26] C：内存清零
来源：http://zph.nwbrower.top

memset(a, 0, sizeof a);
来源：http://uvt.cheryme.top

[S27] C：定义常量
来源：http://mcj.guowangkeji.top

const double PI = 3.14159;
来源：http://nag.yj202588.top

[S28] C：静态变量
来源：http://kou.jianghu66.top

static int counter = 0;
来源：http://hid.yanxiufei.cn

[S29] C：变参函数
来源：http://btg.ivvv.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ijo.zhiwuduotai.top

[S30] C：头文件保护
来源：http://ooz.daxiang520.top

#ifndef X_H
来源：http://kuk.sweek.top

#define X_H
来源：http://vrl.guannengcc.top

#endif
来源：http://ilp.hammf.cn

[S31] C++：Hello World
来源：http://zqg.hcnkem.com

#include <iostream>
来源：http://dbt.mhx1999.top

int main() { std::cout << "Hello\n"; }
来源：http://dok.sweek.top

[S32] C++：字符串
来源：http://kme.haohaochexian.top

std::string s = "hi";  s += "!";
来源：http://gzb.vehdjk.com

[S33] C++：vector 增删
来源：http://uso.cheryme.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gsd.zdqjudy.top

[S34] C++：遍历 vector
来源：http://xlb.zhijiandao.cn

for (auto &x : v) { std::cout << x; }
来源：http://aiy.feifeiyinyue.top

[S35] C++：map
来源：http://aha.chenjidiqi.icu

std::map<std::string, int> m;  m["a"] = 1;
来源：http://miw.52xcode.cn

[S36] C++：unordered_map
来源：http://zpj.c1oappe.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vog.nwbrower.top

[S37] C++：set
来源：http://jpu.ywan-chungtsiang.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://utn.gaohongyu789.top

[S38] C++：排序
来源：http://krn.sufxvd.cn

std::sort(v.begin(), v.end());
来源：http://ixz.hnxiangtu.top

[S39] C++：自定义比较器排序
来源：http://byy.52xcode.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ryt.xziqi.cn

[S40] C++：查找元素
来源：http://zhk.zhiwuduotai.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://eym.ppjwa.cn

[S41] C++：类与构造函数
来源：http://cqk.jinghuilouyu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wsq.redwolf501.top

[S42] C++：继承与虚函数
来源：http://pzp.tarul.cn

class B : public Base { public: void f() override {} };
来源：http://fju.vqdsnc.cn

[S43] C++：智能指针
来源：http://jcj.fktsv.cn

auto p = std::make_unique<int>(5);
来源：http://yct.yangfankeji.com

[S44] C++：引用传参
来源：http://eua.yj20258.top

void inc(int &x) { ++x; }
来源：http://hin.yj20258.top

[S45] C++：lambda
来源：http://pau.haohaochexian.top

auto add = [](int a, int b) { return a + b; };
来源：http://awx.quarkkingdee.top

[S46] C++：函数模板
来源：http://aky.redwolf501.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fhq.shanyushiyangtech.top

[S47] C++：结构化绑定遍历
来源：http://dum.yvedp.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jbr.yuxming.cn

[S48] C++：逐行读文件
来源：http://rgr.gogol.net.cn

std::ifstream in("a.txt");  std::string line;
来源：http://teg.zdqjudy.top

while (std::getline(in, line)) { }
来源：http://vzr.iojbl.cn

[S49] C++：写文件
来源：http://hlb.shanyushiyangkeji.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qln.hcnkem.com

[S50] C++：格式化数字
来源：http://cwd.xingfuxueyuan.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ijw.zhiwuduotai.top

[S51] C++：显式类型转换
来源：http://mxy.bjfxy.top

static_cast<double>(a) / b
来源：http://ygv.ivvv.top

[S52] C++：const 与 noexcept
来源：http://jjh.jinqigfzy.top

int size() const noexcept { return n_; }
来源：http://ail.316326.xyz

[S53] C++：移动语义
来源：http://los.aibaodan.cn

std::vector<int> w = std::move(v);
来源：http://kbw.vehdjk.com

[S54] C++：异常处理
来源：http://gzx.0kj1m.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dtj.cheryme.top

[S55] C++：结构化绑定
来源：http://tif.0kj1m.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://xtq.sxryk.cn

[S56] C++：optional
来源：http://fjq.aibaodan.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qsa.nanxuanxn.top

[S57] C++：编译期常量
来源：http://qmw.sweek.top

constexpr int N = 10;
来源：http://jfv.hnxiangtu.top

[S58] C++：命名空间
来源：http://ivb.nanxuanxn.top

namespace ns { int f() { return 1; } }
来源：http://xfv.gaohongyu789.top

[S59] C++：静态断言
来源：http://ahm.guowangkeji.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zqn.zycfv.cn

[S60] C++：遍历并删除元素
来源：http://jis.chenzaomai.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://uoq.hfpthk.cn

================================================================================
来源：http://uoa.sjlbkw.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ruq.gaohongyu789.top

================================================================================
来源：http://oar.yuxming.cn

[T01] Kotlin：Hello World
来源：http://amq.chenjidiqi.icu

println("Hello")
来源：http://ryo.xylfe.cn

[T02] Kotlin：变量
来源：http://zzk.iojbl.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gnv.sjlbkw.cn

[T03] Kotlin：字符串模板
来源：http://ddg.tian-w.cn

"值: $b"
来源：http://iwd.ctjpmb.com

[T04] Kotlin：空安全
来源：http://jld.yonumen.top

val n: String? = null;  n?.length
来源：http://wuw.jlsjyb.cn

[T05] Kotlin：when 表达式
来源：http://qni.hnxiangtu.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://msy.xylfe.cn

[T06] Kotlin：集合映射
来源：http://pco.zdbjq.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://erw.uphjek.com

[T07] Kotlin：集合过滤
来源：http://zke.cheryme.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://tmg.zdqjudy.top

[T08] Kotlin：数据类
来源：http://oza.xuanzx.com

data class User(val name: String, val age: Int)
来源：http://inw.gzhubu.top

[T09] Kotlin：扩展函数
来源：http://tyx.pycfn.com

fun String.exclaim() = this + "!"
来源：http://vle.kuanghao11.cn

[T10] Kotlin：默认参数
来源：http://ouu.zhengqikj.top

fun greet(name: String = "World") = "Hi $name"
来源：http://qwv.jianghu66.top

[T11] Kotlin：协程
来源：http://kwf.feifeiyinyue.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://iqa.hesvh.cn

[T12] Kotlin：解构声明
来源：http://jfs.shzxlz.cn

val (a, b) = Pair(1, 2)
来源：http://lql.hysaishi.cn

[T13] Kotlin：只读 Map
来源：http://yrr.ydjk.org.cn

val m = mapOf("a" to 1)
来源：http://jmz.yj202588.top

[T14] Kotlin：循环
来源：http://pub.ctjpmb.com

for (i in 1..10) println(i)
来源：http://qbs.hammf.cn

[T15] Kotlin：接口
来源：http://fxh.yvedp.cn

interface Shape { fun area(): Double }
来源：http://wpx.cdnleiting.top

[T16] Swift：Hello World
来源：http://smi.shanyushiyangkeji.top

print("Hello")
来源：http://llz.smart0.xyz

[T17] Swift：变量与常量
来源：http://hjj.hnxiangtu.top

var a = 1;  let b = 2
来源：http://ejv.hnxiangtu.top

[T18] Swift：字符串插值
来源：http://kxp.xuetiantiany.cn

"值: \(b)"
来源：http://rxk.svipenyu.cn

[T19] Swift：可选绑定
来源：http://yak.tanke756.top

if let n = opt { print(n) }
来源：http://tci.sxryk.cn

[T20] Swift：数组操作
来源：http://jru.hfpthk.cn

var a = [1, 2, 3];  a.append(4)
来源：http://kkn.yongpay.top

[T21] Swift：遍历
来源：http://ggh.fanxiaobao.xyz

for x in a { print(x) }
来源：http://fbb.kuanghao11.cn

[T22] Swift：字典
来源：http://rws.hcnkem.com

var d = ["a": 1];  d["b"] = 2
来源：http://zsh.hywenlv.cn

[T23] Swift：函数
来源：http://een.xinyue.icu

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wxo.sxryk.cn

[T24] Swift：闭包
来源：http://ukz.gaohongyu789.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ybr.ctjpmb.com

[T25] Swift：结构体
来源：http://zkt.zhaomingkeji.xyz

struct P { var x: Int }
来源：http://snv.guannengcc.top

[T26] Swift：类与重写
来源：http://jxv.aibaodan.cn

class A: Base { override func f() {} }
来源：http://pvx.fanxiaobao.xyz

[T27] Swift：错误处理
来源：http://noc.chenzaomai.com

do { try f() } catch { print(error) }
来源：http://exw.yj20258.top

[T28] Swift：枚举
来源：http://ukx.xuanzx.com

enum Color { case red, green }
来源：http://pbp.yfazqb.com

[T29] Swift：guard 提前返回
来源：http://mvm.chenzaomai.com

guard let x = opt else { return }
来源：http://hdz.hfpthk.cn

[T30] Swift：协议
来源：http://keg.tianlin.xyz

protocol Shape { func area() -> Double }
来源：http://rev.jinqigufen.top

[T31] Lua：Hello World
来源：http://wxa.hongshengwenyu.top

print("Hello")
来源：http://pwr.316326.xyz

[T32] Lua：局部变量
来源：http://nan.fktsv.cn

local a = 1
来源：http://cgu.xziqi.cn

[T33] Lua：表（数组）
来源：http://txy.ppjwa.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://mwf.xuanzx.com

[T34] Lua：遍历表
来源：http://qvg.316326.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://wio.gaohongyu789.top

[T35] Lua：字典表
来源：http://uiq.iojbl.cn

local d = { a = 1 };  d.b = 2
来源：http://bwi.hysaishi.cn

[T36] Lua：函数
来源：http://pkh.ivvv.top

function add(a, b) return a + b end
来源：http://rlf.haohaochexian.top

[T37] Lua：字符串拼接
来源：http://tur.quarkkingdee.top

"a" .. "b"
来源：http://jej.vqdsnc.cn

[T38] Lua：条件
来源：http://bku.chenjidiqi.icu

if x > 0 then print("正") end
来源：http://vyt.cucudq.cn

[T39] Lua：模式匹配
来源：http://jrs.ydjk.org.cn

string.find(s, "%d+")
来源：http://pga.snrcjt.cn

[T40] Lua：元表
来源：http://arl.sxryk.cn

setmetatable({}, { __index = base })
来源：http://bdv.cucudq.cn

[T41] Perl：Hello World
来源：http://rmu.haohaochexian.top

print "Hello\n";
来源：http://pub.epnwcf.com

[T42] Perl：变量类型
来源：http://jbg.hesvh.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fgk.gzhubu.top

[T43] Perl：字符串插值
来源：http://fqp.jinqigufen.top

"值: $a"
来源：http://ixk.dashuyun.cn

[T44] Perl：条件
来源：http://wnh.epnwcf.com

if ($a > 0) { print "正"; }
来源：http://hkd.yueranfly.top

[T45] Perl：数组遍历
来源：http://fbm.0kj1m.cn

for my $x (@arr) { print $x; }
来源：http://iwa.cqqwz.cn

[T46] Perl：哈希操作
来源：http://ijr.guannengcc.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gfh.guowangkeji.top

[T47] Perl：正则捕获
来源：http://gqt.pycfn.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://nye.fengsongda.top

[T48] Perl：正则替换
来源：http://ydv.dashuyun.cn

$s =~ s/old/new/g;
来源：http://lsd.fehbvm.com

[T49] Perl：函数
来源：http://dsg.sufxvd.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hyy.xziqi.cn

[T50] Perl：逐行读文件
来源：http://rrc.jlsjyb.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://avt.epnwcf.com

while (my $line = <$fh>) { print $line; }
来源：http://cxc.guannengcc.top

[T51] Scala：Hello World
来源：http://gbl.kuanghao11.cn

println("Hello")
来源：http://zwu.zhoulong.xyz

[T52] Scala：变量
来源：http://cbq.jinyuanbaomall.cn

val a = 1;  var b = 2
来源：http://mqh.cdnleiting.top

[T53] Scala：字符串插值
来源：http://ybg.tarul.cn

s"值: $b"
来源：http://bzy.ywan-chungtsiang.top

[T54] Scala：集合映射
来源：http://qdp.zdbjq.cn

List(1, 2, 3).map(_ * 2)
来源：http://gmn.uphjek.com

[T55] Scala：集合过滤
来源：http://gxo.jqgfzy.top

List(1, 2, 3).filter(_ > 1)
来源：http://rmk.0kj1m.cn

[T56] Scala：样例类
来源：http://fwi.zdbjq.cn

case class User(name: String, age: Int)
来源：http://xqt.zhaomingkeji.xyz

[T57] Scala：模式匹配
来源：http://thl.zhaomingkeji.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://qpa.daria6918.cn

[T58] Scala：函数定义
来源：http://bxu.yueranfly.top

def add(a: Int, b: Int): Int = a + b
来源：http://pey.yongpay.top

[T59] Scala：循环
来源：http://acd.yvedp.cn

for (i <- 1 to 10) println(i)
来源：http://sgs.sxryk.cn

[T60] Scala：折叠
来源：http://ncp.uphjek.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://znw.guannengcc.top

================================================================================
来源：http://xcx.zhaomingkeji.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tud.snrcjt.cn

================================================================================
来源：http://mis.ybcxt.top

[U01] Py：创建虚拟环境
来源：http://pmz.chenlongwang.top

python -m venv .venv && source .venv/bin/activate
来源：http://hia.zhengqikj.top

[U02] Py：导出 / 安装依赖
来源：http://shr.shangyingyoupin.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hkz.ywan-chungtsiang.top

[U03] Py：加载 .env 配置
来源：http://gil.yj20258.top

from dotenv import load_dotenv; load_dotenv()
来源：http://gas.jiagoushi.top

[U04] Py：变量调试打印
来源：http://wml.snrcjt.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vln.xinyue.icu

[U05] Py：列表去重且保序
来源：http://hzw.jqgfzy.top

list(dict.fromkeys(arr))
来源：http://fkc.hongshengwenyu.top

[U06] Py：合并两个字典
来源：http://rwp.fehbvm.com

{**a, **b}
来源：http://pcf.wangshuangyany.cn

[U07] Py：反转字典键值
来源：http://cnt.hywenlv.cn

{v: k for k, v in d.items()}
来源：http://wff.ivvv.top

[U08] Py：展平二维列表
来源：http://lgh.hcnkem.com

[y for x in nested for y in x]
来源：http://hdk.jyoumei.cn

[U09] Py：字典取最大值的键
来源：http://qrv.jqgufenzy.top

max(d, key=d.get)
来源：http://ntj.nanxinkj.top

[U10] Py：按值排序字典
来源：http://wqg.nwbrower.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ywv.nanxuanxn.top

[U11] Py：生成器表达式
来源：http://qrb.xylfe.cn

(x * 2 for x in arr)
来源：http://zec.zhongyouzk.top

[U12] Py：取出现最多的 3 个元素
来源：http://enz.zycfv.cn

Counter(arr).most_common(3)
来源：http://jly.zhongyouzk.top

[U13] Py：固定长度队列
来源：http://lha.ydjk.org.cn

deque(maxlen=10)
来源：http://sos.xuanzx.com

[U14] Py：分组收集到列表
来源：http://lhk.yuanzhike.top

defaultdict(list)
来源：http://nsc.zhixingplan.top

[U15] Py：高精度计时
来源：http://zyt.fehbvm.com

t = time.perf_counter()
来源：http://fwj.shanyushiyangtech.top

[U16] Py：命令行参数解析
来源：http://ofe.fktsv.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://aqq.daxiang520.top

[U17] Py：初始化日志
来源：http://ppy.xuetiantiany.cn

logging.basicConfig(level=logging.INFO)
来源：http://spn.316326.xyz

[U18] Py：预编译正则
来源：http://pnc.xingfuxueyuan.xyz

pat = re.compile(r"\d+")
来源：http://qeq.yangfankeji.com

[U19] Py：正则替换带回调
来源：http://oss.cucudq.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://uxk.nanxinkj.top

[U20] Py：缓存函数结果
来源：http://tes.tian-w.cn

@functools.lru_cache(maxsize=None)
来源：http://znf.pengpengdd.cyou

[U21] Py：自定义上下文管理器
来源：http://lfc.ybcxt.top

@contextlib.contextmanager
来源：http://vgl.kuanghao11.cn

[U22] Py：矩阵转置
来源：http://njw.jqgufenzy.top

list(zip(*m))
来源：http://hwh.yj20258888.top

[U23] Py：分块读取大文件
来源：http://kyq.redwolf501.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://uvf.aibaodan.cn

[U24] Py：路径操作
来源：http://zaf.ydzc1.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://skp.shuidangran.top

[U25] Py：CSV 按字典读
来源：http://wxo.zhiwuduotai.top

csv.DictReader(f)
来源：http://gya.fehbvm.com

[U26] Py：并发下载
来源：http://fgp.dianchejie.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ber.cqqwz.cn

[U27] Py：异步 HTTP
来源：http://dvm.yueranfly.top

aiohttp.ClientSession() 配合 async with
来源：http://kre.cqqwz.cn

[U28] Py：类型别名
来源：http://cxe.yj20258888.top

UserId = int
来源：http://tpr.9152youxi.cn

[U29] Py：属性校验
来源：http://ibt.jqgufenzy.top

@property 与 @x.setter 配合
来源：http://pqo.jlsjyb.cn

[U30] Py：数据类
来源：http://jmq.ydzc1.top

@dataclass(slots=True)
来源：http://lfe.zhengqikj.top

[U31] Py：单测
来源：http://cxd.chenjidiqi.icu

python -m pytest -q
来源：http://hlp.daxiang520.top

[U32] Py：代码格式化
来源：http://ric.chenzaomai.com

ruff format . && ruff check --fix .
来源：http://jpv.chenjidiqi.icu

[U33] Py：打包发布
来源：http://qqw.daxiang520.top

python -m build  （依赖 pyproject.toml）
来源：http://gct.jiagoushi.top

[U34] Py：判断编码
来源：http://jzt.hammf.cn

chardet.detect(raw)
来源：http://nrr.fengsongda.top

[U35] Py：发送邮件
来源：http://ujl.hnxiangtu.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://byb.zdbjq.cn

[U36] Py：定时任务
来源：http://dnj.feifeiyinyue.top

schedule.every(10).minutes.do(job)
来源：http://nuh.fehbvm.com

[U37] Py：读写 Excel
来源：http://yos.zhixingplan.top

pandas.read_excel / DataFrame.to_excel
来源：http://kzr.jiagoushi.top

[U38] Py：获取脚本所在目录
来源：http://bpj.zhixingplan.top

Path(__file__).resolve().parent
来源：http://slw.snrcjt.cn

[U39] Py：判断是否在交互环境
来源：http://cln.feifeiyinyue.top

sys.stdout.isatty()
来源：http://itw.yj20258888.top

[U40] Py：打印到标准错误
来源：http://djh.vehdjk.com

print("err", file=sys.stderr)
来源：http://xhz.zhijiandao.cn

[U41] PHP：初始化 Composer 项目
来源：http://upr.fanxiaobao.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://vcb.redwolf501.top

[U42] PHP：PSR-4 自动加载
来源：http://eez.fengsongda.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mzv.jinyuanbaomall.cn

[U43] PHP：声明命名空间
来源：http://wgj.kuanghao11.cn

namespace App\Http;
来源：http://hko.vehdjk.com

[U44] PHP：开启严格类型
来源：http://gjz.yueranfly.top

declare(strict_types=1);
来源：http://mlg.ybcxt.top

[U45] PHP：类型声明与返回类型
来源：http://cbo.shanyushiyangtech.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://syk.jianghu66.top

[U46] PHP：可空类型
来源：http://qfr.zycfv.cn

?string $name = null
来源：http://yeg.jinqigfzy.top

[U47] PHP：联合类型
来源：http://ecr.c1oappe.top

int|string $id
来源：http://yoy.shanyushiyangtech.top

[U48] PHP：纯枚举
来源：http://dcy.chenzaomai.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://msi.nanxuanxn.top


<!-- 参考信息 -->