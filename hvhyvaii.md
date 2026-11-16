代发 wailian999

memset(a, 0, sizeof a);
来源：http://cjz.vehdjk.com

[S27] C：定义常量
来源：http://nvn.chenlongwang.top

const double PI = 3.14159;
来源：http://fgz.aizwys.cn

[S28] C：静态变量
来源：http://hir.havefunace.top

static int counter = 0;
来源：http://knl.epnwcf.com

[S29] C：变参函数
来源：http://ird.sufxvd.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vme.shuidangran.top

[S30] C：头文件保护
来源：http://heg.gogol.net.cn

#ifndef X_H
来源：http://mmv.zhaomingkeji.xyz

#define X_H
来源：http://tfk.nanxinkj.top

#endif
来源：http://uof.jianghu66.top

[S31] C++：Hello World
来源：http://ook.quarkkingdee.top

#include <iostream>
来源：http://lft.andypj.xyz

int main() { std::cout << "Hello\n"; }
来源：http://fir.zhaomingkeji.xyz

[S32] C++：字符串
来源：http://ydd.ivvv.top

std::string s = "hi";  s += "!";
来源：http://fsl.kuanghao11.cn

[S33] C++：vector 增删
来源：http://zjl.jinyuanbaomall.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zyt.xuanzx.com

[S34] C++：遍历 vector
来源：http://ecl.bjfxy.top

for (auto &x : v) { std::cout << x; }
来源：http://qnt.chenlongwang.top

[S35] C++：map
来源：http://vzi.dianchejie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qyu.smart0.xyz

[S36] C++：unordered_map
来源：http://lng.xuetiantiany.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qcf.bbcook.cn

[S37] C++：set
来源：http://sdq.vehdjk.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tlw.fanxiaobao.xyz

[S38] C++：排序
来源：http://tay.sweek.top

std::sort(v.begin(), v.end());
来源：http://blk.sxryk.cn

[S39] C++：自定义比较器排序
来源：http://izm.gzhubu.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://idj.xuanzx.com

[S40] C++：查找元素
来源：http://zas.zhixingplan.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://stw.jqgfzy.top

[S41] C++：类与构造函数
来源：http://kha.sxryk.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jwm.yuxming.cn

[S42] C++：继承与虚函数
来源：http://ddd.nanxinkj.top

class B : public Base { public: void f() override {} };
来源：http://azq.xuetiantiany.cn

[S43] C++：智能指针
来源：http://exl.yuxming.cn

auto p = std::make_unique<int>(5);
来源：http://bed.yuanzhike.top

[S44] C++：引用传参
来源：http://oqd.andypj.xyz

void inc(int &x) { ++x; }
来源：http://aly.ctjpmb.com

[S45] C++：lambda
来源：http://aio.cucudq.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xva.smart0.xyz

[S46] C++：函数模板
来源：http://ndj.hongshengwenyu.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dza.hcnkem.com

[S47] C++：结构化绑定遍历
来源：http://dgb.yongpay.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://krn.guowangkeji.top

[S48] C++：逐行读文件
来源：http://epk.xingfuxueyuan.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://hss.cdnleiting.top

while (std::getline(in, line)) { }
来源：http://zty.cucudq.cn

[S49] C++：写文件
来源：http://eks.kuanghao11.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fhs.shanyushiyangtech.top

[S50] C++：格式化数字
来源：http://why.chenzaomai.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qyh.316326.xyz

[S51] C++：显式类型转换
来源：http://efh.ywan-chungtsiang.top

static_cast<double>(a) / b
来源：http://yer.redwolf501.top

[S52] C++：const 与 noexcept
来源：http://ykt.bbcook.cn

int size() const noexcept { return n_; }
来源：http://tvj.cashguo.top

[S53] C++：移动语义
来源：http://ana.cheryme.top

std::vector<int> w = std::move(v);
来源：http://bnr.daria6918.cn

[S54] C++：异常处理
来源：http://hgo.fengsongda.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hcp.cucudq.cn

[S55] C++：结构化绑定
来源：http://trr.hfpthk.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://yvg.feifeiyinyue.top

[S56] C++：optional
来源：http://dut.fanxiaobao.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dff.guowangkeji.top

[S57] C++：编译期常量
来源：http://gzk.sjlbkw.cn

constexpr int N = 10;
来源：http://fmg.havefunace.top

[S58] C++：命名空间
来源：http://bbh.zhengqikj.top

namespace ns { int f() { return 1; } }
来源：http://coa.shanyushiyangkeji.top

[S59] C++：静态断言
来源：http://tpf.meibo888.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mwk.gotoacloud.top

[S60] C++：遍历并删除元素
来源：http://cfg.yfazqb.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mfp.jinqigfzy.top

================================================================================
来源：http://ytq.ctjpmb.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wtv.xziqi.cn

================================================================================
来源：http://rrx.gaohongyu789.top

[T01] Kotlin：Hello World
来源：http://aii.hammf.cn

println("Hello")
来源：http://kkc.fanxiaobao.xyz

[T02] Kotlin：变量
来源：http://zdv.birdmap.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gvc.shanyushiyangkeji.top

[T03] Kotlin：字符串模板
来源：http://aap.cucudq.cn

"值: $b"
来源：http://xtl.hcnkem.com

[T04] Kotlin：空安全
来源：http://bmy.yongpay.top

val n: String? = null;  n?.length
来源：http://scg.aibaodan.cn

[T05] Kotlin：when 表达式
来源：http://vts.wangshuangyany.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hkf.ydjk.org.cn

[T06] Kotlin：集合映射
来源：http://bde.yueranfly.top

listOf(1, 2, 3).map { it * 2 }
来源：http://bed.hysaishi.cn

[T07] Kotlin：集合过滤
来源：http://uyk.hcnkem.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://pzl.ppjwa.cn

[T08] Kotlin：数据类
来源：http://ouv.c1oappe.top

data class User(val name: String, val age: Int)
来源：http://cvp.yonumen.top

[T09] Kotlin：扩展函数
来源：http://mvi.shanyushiyangtech.top

fun String.exclaim() = this + "!"
来源：http://iey.fzhhl.top

[T10] Kotlin：默认参数
来源：http://trq.ppjwa.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://rrx.ppjwa.cn

[T11] Kotlin：协程
来源：http://gds.yongpay.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://elj.jianghu66.top

[T12] Kotlin：解构声明
来源：http://mye.zhaomingkeji.xyz

val (a, b) = Pair(1, 2)
来源：http://bws.svipenyu.cn

[T13] Kotlin：只读 Map
来源：http://dfv.zdqjudy.top

val m = mapOf("a" to 1)
来源：http://olh.xinyue.icu

[T14] Kotlin：循环
来源：http://rjv.fehbvm.com

for (i in 1..10) println(i)
来源：http://rjl.jinyuanbaomall.cn

[T15] Kotlin：接口
来源：http://qnd.yj20258.top

interface Shape { fun area(): Double }
来源：http://wrv.shuidangran.top

[T16] Swift：Hello World
来源：http://amc.jyoumei.cn

print("Hello")
来源：http://dnp.kuanghao11.cn

[T17] Swift：变量与常量
来源：http://ort.chenzaomai.com

var a = 1;  let b = 2
来源：http://orh.zdqjudy.top

[T18] Swift：字符串插值
来源：http://qxr.haohaochexian.top

"值: \(b)"
来源：http://sah.cqqwz.cn

[T19] Swift：可选绑定
来源：http://ckb.gogol.net.cn

if let n = opt { print(n) }
来源：http://prz.yangfankeji.com

[T20] Swift：数组操作
来源：http://mna.tianlin.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://del.svipenyu.cn

[T21] Swift：遍历
来源：http://gqq.svipenyu.cn

for x in a { print(x) }
来源：http://xsq.zhengqikj.top

[T22] Swift：字典
来源：http://ewl.yanxiufei.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ftk.xingfuxueyuan.xyz

[T23] Swift：函数
来源：http://aiv.sufxvd.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ixk.hnxiangtu.top

[T24] Swift：闭包
来源：http://uxi.hesvh.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://crz.guannengcc.top

[T25] Swift：结构体
来源：http://cwc.hammf.cn

struct P { var x: Int }
来源：http://jdx.hysaishi.cn

[T26] Swift：类与重写
来源：http://ubw.hcnkem.com

class A: Base { override func f() {} }
来源：http://dxk.hysaishi.cn

[T27] Swift：错误处理
来源：http://aro.ppjwa.cn

do { try f() } catch { print(error) }
来源：http://scq.yanxiufei.cn

[T28] Swift：枚举
来源：http://syg.tianlin.xyz

enum Color { case red, green }
来源：http://omd.cdnleiting.top

[T29] Swift：guard 提前返回
来源：http://isf.vehdjk.com

guard let x = opt else { return }
来源：http://mmj.sweek.top

[T30] Swift：协议
来源：http://dbr.aibaodan.cn

protocol Shape { func area() -> Double }
来源：http://gji.guowangkeji.top

[T31] Lua：Hello World
来源：http://wie.316326.xyz

print("Hello")
来源：http://cmr.feifeiyinyue.top

[T32] Lua：局部变量
来源：http://vli.tian-w.cn

local a = 1
来源：http://ibi.hnxiangtu.top

[T33] Lua：表（数组）
来源：http://fxx.ydjk.org.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ckl.chenjidiqi.icu

[T34] Lua：遍历表
来源：http://hra.uphjek.com

for i, v in ipairs(t) do print(i, v) end
来源：http://jdz.tianlin.xyz

[T35] Lua：字典表
来源：http://nww.shanyushiyangkeji.top

local d = { a = 1 };  d.b = 2
来源：http://jix.bbcook.cn

[T36] Lua：函数
来源：http://zqf.bbcook.cn

function add(a, b) return a + b end
来源：http://ugk.aizwys.cn

[T37] Lua：字符串拼接
来源：http://jwm.shanyushiyangtech.top

"a" .. "b"
来源：http://hrh.ydjk.org.cn

[T38] Lua：条件
来源：http://jcf.guowangkeji.top

if x > 0 then print("正") end
来源：http://tne.cheryme.top

[T39] Lua：模式匹配
来源：http://kxw.jianghu66.top

string.find(s, "%d+")
来源：http://gqe.hywenlv.cn

[T40] Lua：元表
来源：http://npo.jiagoushi.top

setmetatable({}, { __index = base })
来源：http://iff.dianchejie.cn

[T41] Perl：Hello World
来源：http://sbm.havefunace.top

print "Hello\n";
来源：http://vwe.sweek.top

[T42] Perl：变量类型
来源：http://csy.snrcjt.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fio.zhiwuduotai.top

[T43] Perl：字符串插值
来源：http://sin.birdmap.top

"值: $a"
来源：http://mhr.dianchejie.cn

[T44] Perl：条件
来源：http://ahv.gotoacloud.top

if ($a > 0) { print "正"; }
来源：http://gzf.c1oappe.top

[T45] Perl：数组遍历
来源：http://lzg.hnxiangtu.top

for my $x (@arr) { print $x; }
来源：http://ofn.cqqwz.cn

[T46] Perl：哈希操作
来源：http://lay.cdnleiting.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dcn.zhiwuduotai.top

[T47] Perl：正则捕获
来源：http://gax.yj20258.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://mor.nwbrower.top

[T48] Perl：正则替换
来源：http://apr.sxryk.cn

$s =~ s/old/new/g;
来源：http://uzu.wangdashe.top

[T49] Perl：函数
来源：http://wrz.jiagoushi.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ees.ivvv.top

[T50] Perl：逐行读文件
来源：http://nkj.nanxinkj.top

open my $fh, "<", "a.txt" or die $!;
来源：http://nfl.jyoumei.cn

while (my $line = <$fh>) { print $line; }
来源：http://nje.cucudq.cn

[T51] Scala：Hello World
来源：http://ckn.ywan-chungtsiang.top

println("Hello")
来源：http://pni.zhiwuduotai.top

[T52] Scala：变量
来源：http://cwp.hysaishi.cn

val a = 1;  var b = 2
来源：http://bre.chenjidiqi.icu

[T53] Scala：字符串插值
来源：http://prb.zhixingplan.top

s"值: $b"
来源：http://huj.jinqigfzy.top

[T54] Scala：集合映射
来源：http://ffl.birdmap.top

List(1, 2, 3).map(_ * 2)
来源：http://cpa.guowangkeji.top

[T55] Scala：集合过滤
来源：http://gxj.fengsongda.top

List(1, 2, 3).filter(_ > 1)
来源：http://wpb.52xcode.cn

[T56] Scala：样例类
来源：http://jgj.fengsongda.top

case class User(name: String, age: Int)
来源：http://xox.mhx1999.top

[T57] Scala：模式匹配
来源：http://aby.hongshengwenyu.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://xhg.gaohongyu789.top

[T58] Scala：函数定义
来源：http://hyz.yfazqb.com

def add(a: Int, b: Int): Int = a + b
来源：http://tde.shanyushiyangkeji.top

[T59] Scala：循环
来源：http://odu.snrcjt.cn

for (i <- 1 to 10) println(i)
来源：http://lsi.tanke756.top

[T60] Scala：折叠
来源：http://uhc.cashguo.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nkp.fehbvm.com

================================================================================
来源：http://ojn.jinyuanbaomall.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qxk.shangyingyoupin.top

================================================================================
来源：http://kcr.hfpthk.cn

[U01] Py：创建虚拟环境
来源：http://igd.chenzaomai.com

python -m venv .venv && source .venv/bin/activate
来源：http://snc.guowangkeji.top

[U02] Py：导出 / 安装依赖
来源：http://nxa.mhx1999.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yku.aizwys.cn

[U03] Py：加载 .env 配置
来源：http://xuk.pengpengdd.cyou

from dotenv import load_dotenv; load_dotenv()
来源：http://olo.xinyue.icu

[U04] Py：变量调试打印
来源：http://xpe.hongshengwenyu.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://evf.zhaomingkeji.xyz

[U05] Py：列表去重且保序
来源：http://rfz.shuidangran.top

list(dict.fromkeys(arr))
来源：http://bqi.uphjek.com

[U06] Py：合并两个字典
来源：http://hog.nwbrower.top

{**a, **b}
来源：http://wyw.fehbvm.com

[U07] Py：反转字典键值
来源：http://zgj.jqgufenzy.top

{v: k for k, v in d.items()}
来源：http://nhx.0kj1m.cn

[U08] Py：展平二维列表
来源：http://nvw.birdmap.top

[y for x in nested for y in x]
来源：http://nfq.ywan-chungtsiang.top

[U09] Py：字典取最大值的键
来源：http://fup.cheryme.top

max(d, key=d.get)
来源：http://ijr.wangshuangyany.cn

[U10] Py：按值排序字典
来源：http://fns.52xcode.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mfz.shanyushiyangtech.top

[U11] Py：生成器表达式
来源：http://som.hnxiangtu.top

(x * 2 for x in arr)
来源：http://fce.cashguo.top

[U12] Py：取出现最多的 3 个元素
来源：http://ghq.sufxvd.cn

Counter(arr).most_common(3)
来源：http://bku.quarkkingdee.top

[U13] Py：固定长度队列
来源：http://etz.zhoulong.xyz

deque(maxlen=10)
来源：http://pva.xinyue.icu

[U14] Py：分组收集到列表
来源：http://wxt.9152youxi.cn

defaultdict(list)
来源：http://frl.yonumen.top

[U15] Py：高精度计时
来源：http://mtr.gotoacloud.top

t = time.perf_counter()
来源：http://zbb.hywenlv.cn

[U16] Py：命令行参数解析
来源：http://rcl.jianghu66.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gwb.vqdsnc.cn

[U17] Py：初始化日志
来源：http://whf.birdmap.top

logging.basicConfig(level=logging.INFO)
来源：http://vmp.316326.xyz

[U18] Py：预编译正则
来源：http://mqy.316326.xyz

pat = re.compile(r"\d+")
来源：http://tzf.shangyingyoupin.top

[U19] Py：正则替换带回调
来源：http://rhx.nanxinkj.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xjp.yfazqb.com

[U20] Py：缓存函数结果
来源：http://yan.9152youxi.cn

@functools.lru_cache(maxsize=None)
来源：http://ilq.shanyushiyangtech.top

[U21] Py：自定义上下文管理器
来源：http://xta.hnqzz.top

@contextlib.contextmanager
来源：http://vti.52xcode.cn

[U22] Py：矩阵转置
来源：http://lnp.9152youxi.cn

list(zip(*m))
来源：http://smk.aibaodan.cn

[U23] Py：分块读取大文件
来源：http://eqb.daria6918.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qrs.jinyuanbaomall.cn

[U24] Py：路径操作
来源：http://ooy.zhaomingkeji.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ven.hesvh.cn

[U25] Py：CSV 按字典读
来源：http://nnp.shangyingyoupin.top

csv.DictReader(f)
来源：http://lpd.jqgfzy.top

[U26] Py：并发下载
来源：http://grb.zhaomingkeji.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xzc.jqgfzy.top

[U27] Py：异步 HTTP
来源：http://ypc.yangfankeji.com

aiohttp.ClientSession() 配合 async with
来源：http://hsi.xuanzx.com

[U28] Py：类型别名
来源：http://nni.zdqjudy.top

UserId = int
来源：http://iuh.yj202588.top

[U29] Py：属性校验
来源：http://rld.yanxiufei.cn

@property 与 @x.setter 配合
来源：http://akb.hongshengwenyu.top

[U30] Py：数据类
来源：http://jeu.ctjpmb.com

@dataclass(slots=True)
来源：http://jng.gzhubu.top

[U31] Py：单测
来源：http://pbo.ctjpmb.com

python -m pytest -q
来源：http://ceu.nanxinkj.top

[U32] Py：代码格式化
来源：http://hsa.kuanghao11.cn

ruff format . && ruff check --fix .
来源：http://xhk.yfazqb.com

[U33] Py：打包发布
来源：http://fda.zhaomingkeji.xyz

python -m build  （依赖 pyproject.toml）
来源：http://zcf.jiagoushi.top

[U34] Py：判断编码
来源：http://mym.xylfe.cn

chardet.detect(raw)
来源：http://qnm.xziqi.cn

[U35] Py：发送邮件
来源：http://eex.shuidangran.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zxf.vqdsnc.cn

[U36] Py：定时任务
来源：http://hfe.yanxiufei.cn

schedule.every(10).minutes.do(job)
来源：http://hvz.yuxming.cn

[U37] Py：读写 Excel
来源：http://lsd.ywan-chungtsiang.top

pandas.read_excel / DataFrame.to_excel
来源：http://fbs.yvedp.cn

[U38] Py：获取脚本所在目录
来源：http://sdq.haohaochexian.top

Path(__file__).resolve().parent
来源：http://zwo.bbcook.cn

[U39] Py：判断是否在交互环境
来源：http://xuc.jianghu66.top

sys.stdout.isatty()
来源：http://rdh.quarkkingdee.top

[U40] Py：打印到标准错误
来源：http://ojj.ctjpmb.com

print("err", file=sys.stderr)
来源：http://mtj.52xcode.cn

[U41] PHP：初始化 Composer 项目
来源：http://bpe.sysykeji.top

composer init;  composer require guzzlehttp/guzzle
来源：http://elq.jianghu66.top

[U42] PHP：PSR-4 自动加载
来源：http://cjf.shangyingyoupin.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://sbi.gotoacloud.top

[U43] PHP：声明命名空间
来源：http://ogd.sysykeji.top

namespace App\Http;
来源：http://spz.yongpay.top

[U44] PHP：开启严格类型
来源：http://gqs.yanxiufei.cn

declare(strict_types=1);
来源：http://giq.uphjek.com

[U45] PHP：类型声明与返回类型
来源：http://yua.ehwqpu.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://idk.jinqigufen.top

[U46] PHP：可空类型
来源：http://quz.wangshuangyany.cn

?string $name = null
来源：http://jbo.daria6918.cn

[U47] PHP：联合类型
来源：http://osb.bjfxy.top

int|string $id
来源：http://yqh.cqqwz.cn

[U48] PHP：纯枚举
来源：http://vxd.jqgufenzy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://azh.jianghu66.top

[U49] PHP：只读属性
来源：http://hzz.jinghuilouyu.cn

public readonly string $name
来源：http://gpa.zdbjq.cn

[U50] PHP：构造器属性提升
来源：http://ifl.gzhubu.top

public function __construct(private int $id) {}
来源：http://gnr.zycfv.cn


<!-- 参考信息 -->