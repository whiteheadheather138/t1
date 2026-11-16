代发 wailian999

memset(a, 0, sizeof a);
来源：http://lph.sufxvd.cn

[S27] C：定义常量
来源：http://zjk.bbcook.cn

const double PI = 3.14159;
来源：http://mil.yanxiufei.cn

[S28] C：静态变量
来源：http://lzu.tanke756.top

static int counter = 0;
来源：http://cxb.yvedp.cn

[S29] C：变参函数
来源：http://tug.jinyuanbaomall.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kxq.jinyuanbaomall.cn

[S30] C：头文件保护
来源：http://mtq.jianghu66.top

#ifndef X_H
来源：http://efz.ehwqpu.com

#define X_H
来源：http://igy.gzhubu.top

#endif
来源：http://qbf.yongpay.top

[S31] C++：Hello World
来源：http://cfd.jyoumei.cn

#include <iostream>
来源：http://mwb.hammf.cn

int main() { std::cout << "Hello\n"; }
来源：http://moc.meibo888.top

[S32] C++：字符串
来源：http://mvt.gotoacloud.top

std::string s = "hi";  s += "!";
来源：http://euu.jqgfzy.top

[S33] C++：vector 增删
来源：http://mgi.havefunace.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nup.quarkkingdee.top

[S34] C++：遍历 vector
来源：http://bni.yuanzhike.top

for (auto &x : v) { std::cout << x; }
来源：http://jdm.hammf.cn

[S35] C++：map
来源：http://rfe.jyoumei.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wgn.tarul.cn

[S36] C++：unordered_map
来源：http://csk.cheryme.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://taf.feifeiyinyue.top

[S37] C++：set
来源：http://ndx.aizwys.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vgr.cdnleiting.top

[S38] C++：排序
来源：http://jgw.yj20258888.top

std::sort(v.begin(), v.end());
来源：http://jwg.nanxuanxn.top

[S39] C++：自定义比较器排序
来源：http://dyg.daria6918.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vym.fzhhl.top

[S40] C++：查找元素
来源：http://bfy.ivvv.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://atr.zdqjudy.top

[S41] C++：类与构造函数
来源：http://mlx.gotoacloud.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xwi.birdmap.top

[S42] C++：继承与虚函数
来源：http://jqn.tarul.cn

class B : public Base { public: void f() override {} };
来源：http://dla.sysykeji.top

[S43] C++：智能指针
来源：http://skg.svipenyu.cn

auto p = std::make_unique<int>(5);
来源：http://vct.epnwcf.com

[S44] C++：引用传参
来源：http://jlu.nwbrower.top

void inc(int &x) { ++x; }
来源：http://rep.shanyushiyangtech.top

[S45] C++：lambda
来源：http://jia.fanxiaobao.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://not.sjlbkw.cn

[S46] C++：函数模板
来源：http://msd.cdnleiting.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://prb.chenlongwang.top

[S47] C++：结构化绑定遍历
来源：http://sil.nanxinkj.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qov.c1oappe.top

[S48] C++：逐行读文件
来源：http://oqa.zycfv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://fys.ppjwa.cn

while (std::getline(in, line)) { }
来源：http://kwc.jqgufenzy.top

[S49] C++：写文件
来源：http://vyy.ydzc1.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cpl.ybcxt.top

[S50] C++：格式化数字
来源：http://aef.ppjwa.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qgz.fehbvm.com

[S51] C++：显式类型转换
来源：http://fwk.dashuyun.cn

static_cast<double>(a) / b
来源：http://gks.shanyushiyangkeji.top

[S52] C++：const 与 noexcept
来源：http://knd.quarkkingdee.top

int size() const noexcept { return n_; }
来源：http://isn.jinqigufen.top

[S53] C++：移动语义
来源：http://yak.fanxiaobao.xyz

std::vector<int> w = std::move(v);
来源：http://dtv.guowangkeji.top

[S54] C++：异常处理
来源：http://gnv.uphjek.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wdl.bbcook.cn

[S55] C++：结构化绑定
来源：http://abm.kuanghao11.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://gix.xuetiantiany.cn

[S56] C++：optional
来源：http://iot.yanxiufei.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ual.jinqigfzy.top

[S57] C++：编译期常量
来源：http://jlm.aizwys.cn

constexpr int N = 10;
来源：http://uat.zdbjq.cn

[S58] C++：命名空间
来源：http://pqm.meibo888.top

namespace ns { int f() { return 1; } }
来源：http://bnc.ivvv.top

[S59] C++：静态断言
来源：http://rzd.kuanghao11.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hlm.jinyuanbaomall.cn

[S60] C++：遍历并删除元素
来源：http://eeh.cqqwz.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cye.sufxvd.cn

================================================================================
来源：http://utp.yj20258.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gou.jinghuilouyu.cn

================================================================================
来源：http://lgj.zhoulong.xyz

[T01] Kotlin：Hello World
来源：http://isr.fengsongda.top

println("Hello")
来源：http://fgc.uphjek.com

[T02] Kotlin：变量
来源：http://zrz.ydjk.org.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cof.hcnkem.com

[T03] Kotlin：字符串模板
来源：http://quc.xuetiantiany.cn

"值: $b"
来源：http://scq.feifeiyinyue.top

[T04] Kotlin：空安全
来源：http://ing.sysykeji.top

val n: String? = null;  n?.length
来源：http://cuc.xuetiantiany.cn

[T05] Kotlin：when 表达式
来源：http://gtt.zhixingplan.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uhm.andypj.xyz

[T06] Kotlin：集合映射
来源：http://opk.cucudq.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://byp.quarkkingdee.top

[T07] Kotlin：集合过滤
来源：http://qcr.feifeiyinyue.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://mdd.nanxinkj.top

[T08] Kotlin：数据类
来源：http://air.gzhubu.top

data class User(val name: String, val age: Int)
来源：http://bac.ybcxt.top

[T09] Kotlin：扩展函数
来源：http://rpc.andypj.xyz

fun String.exclaim() = this + "!"
来源：http://uey.zdqjudy.top

[T10] Kotlin：默认参数
来源：http://clg.yj20258.top

fun greet(name: String = "World") = "Hi $name"
来源：http://jsl.sjlbkw.cn

[T11] Kotlin：协程
来源：http://wlp.feifeiyinyue.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://usj.fanxiaobao.xyz

[T12] Kotlin：解构声明
来源：http://lqu.9152youxi.cn

val (a, b) = Pair(1, 2)
来源：http://ltr.shanyushiyangkeji.top

[T13] Kotlin：只读 Map
来源：http://hpn.fanxiaobao.xyz

val m = mapOf("a" to 1)
来源：http://lnr.aibaodan.cn

[T14] Kotlin：循环
来源：http://puw.uphjek.com

for (i in 1..10) println(i)
来源：http://hnf.sysykeji.top

[T15] Kotlin：接口
来源：http://mqc.haohaochexian.top

interface Shape { fun area(): Double }
来源：http://ars.sysykeji.top

[T16] Swift：Hello World
来源：http://skb.sufxvd.cn

print("Hello")
来源：http://tyc.xuetiantiany.cn

[T17] Swift：变量与常量
来源：http://jlp.fehbvm.com

var a = 1;  let b = 2
来源：http://sef.chenlongwang.top

[T18] Swift：字符串插值
来源：http://qsw.ydjk.org.cn

"值: \(b)"
来源：http://jmq.cheryme.top

[T19] Swift：可选绑定
来源：http://jwm.zhiwuduotai.top

if let n = opt { print(n) }
来源：http://pnp.shzxlz.cn

[T20] Swift：数组操作
来源：http://ogg.smart0.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://dwj.pengpengdd.cyou

[T21] Swift：遍历
来源：http://uqf.tanke756.top

for x in a { print(x) }
来源：http://kfi.daxiang520.top

[T22] Swift：字典
来源：http://tqs.daria6918.cn

var d = ["a": 1];  d["b"] = 2
来源：http://oqz.epnwcf.com

[T23] Swift：函数
来源：http://irp.zycfv.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://djb.yj20258.top

[T24] Swift：闭包
来源：http://fwr.tarul.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://rnz.jqgufenzy.top

[T25] Swift：结构体
来源：http://hyf.yuxming.cn

struct P { var x: Int }
来源：http://mzm.haohaochexian.top

[T26] Swift：类与重写
来源：http://ttg.gotoacloud.top

class A: Base { override func f() {} }
来源：http://fgq.haohaochexian.top

[T27] Swift：错误处理
来源：http://qpz.hywenlv.cn

do { try f() } catch { print(error) }
来源：http://hzf.redwolf501.top

[T28] Swift：枚举
来源：http://exh.yfazqb.com

enum Color { case red, green }
来源：http://ipx.ydzc1.top

[T29] Swift：guard 提前返回
来源：http://ndq.hcnkem.com

guard let x = opt else { return }
来源：http://ltv.nanxinkj.top

[T30] Swift：协议
来源：http://gre.zhoulong.xyz

protocol Shape { func area() -> Double }
来源：http://sdn.kuanghao11.cn

[T31] Lua：Hello World
来源：http://vjx.bbcook.cn

print("Hello")
来源：http://jvm.9152youxi.cn

[T32] Lua：局部变量
来源：http://nyj.shuidangran.top

local a = 1
来源：http://wgc.mhx1999.top

[T33] Lua：表（数组）
来源：http://bwa.yuxming.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hjr.mhx1999.top

[T34] Lua：遍历表
来源：http://xac.svipenyu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://fpc.nwbrower.top

[T35] Lua：字典表
来源：http://ogn.ehwqpu.com

local d = { a = 1 };  d.b = 2
来源：http://knb.tian-w.cn

[T36] Lua：函数
来源：http://kov.ywan-chungtsiang.top

function add(a, b) return a + b end
来源：http://jfm.chenjidiqi.icu

[T37] Lua：字符串拼接
来源：http://ynb.cdnleiting.top

"a" .. "b"
来源：http://apz.zhixingplan.top

[T38] Lua：条件
来源：http://xqm.wangshuangyany.cn

if x > 0 then print("正") end
来源：http://uxa.zhoulong.xyz

[T39] Lua：模式匹配
来源：http://kbx.xziqi.cn

string.find(s, "%d+")
来源：http://kkl.hammf.cn

[T40] Lua：元表
来源：http://jfi.fanxiaobao.xyz

setmetatable({}, { __index = base })
来源：http://ekd.zhongyouzk.top

[T41] Perl：Hello World
来源：http://zcb.zhaomingkeji.xyz

print "Hello\n";
来源：http://wpz.gzhubu.top

[T42] Perl：变量类型
来源：http://ovc.gotoacloud.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hav.yvedp.cn

[T43] Perl：字符串插值
来源：http://ylf.ybcxt.top

"值: $a"
来源：http://huh.birdmap.top

[T44] Perl：条件
来源：http://eyd.fehbvm.com

if ($a > 0) { print "正"; }
来源：http://lpq.aibaodan.cn

[T45] Perl：数组遍历
来源：http://qpl.shangyingyoupin.top

for my $x (@arr) { print $x; }
来源：http://lcx.xuanzx.com

[T46] Perl：哈希操作
来源：http://srq.sufxvd.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lwh.52xcode.cn

[T47] Perl：正则捕获
来源：http://fds.zhiwuduotai.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://zbh.hammf.cn

[T48] Perl：正则替换
来源：http://dau.nanxinkj.top

$s =~ s/old/new/g;
来源：http://wij.52xcode.cn

[T49] Perl：函数
来源：http://ssp.zycfv.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dms.birdmap.top

[T50] Perl：逐行读文件
来源：http://xcp.yfazqb.com

open my $fh, "<", "a.txt" or die $!;
来源：http://paa.9152youxi.cn

while (my $line = <$fh>) { print $line; }
来源：http://oir.hongshengwenyu.top

[T51] Scala：Hello World
来源：http://prj.aibaodan.cn

println("Hello")
来源：http://ien.cashguo.top

[T52] Scala：变量
来源：http://hcl.wangshuangyany.cn

val a = 1;  var b = 2
来源：http://zyn.dianchejie.cn

[T53] Scala：字符串插值
来源：http://mnt.cqqwz.cn

s"值: $b"
来源：http://qyu.mhx1999.top

[T54] Scala：集合映射
来源：http://xhh.yuxming.cn

List(1, 2, 3).map(_ * 2)
来源：http://tvs.iojbl.cn

[T55] Scala：集合过滤
来源：http://pxi.iojbl.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xrk.jiagoushi.top

[T56] Scala：样例类
来源：http://ghd.wangdashe.top

case class User(name: String, age: Int)
来源：http://ksx.zhengqikj.top

[T57] Scala：模式匹配
来源：http://lam.shzxlz.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://oxc.ppjwa.cn

[T58] Scala：函数定义
来源：http://zrx.shanyushiyangkeji.top

def add(a: Int, b: Int): Int = a + b
来源：http://ctf.ybcxt.top

[T59] Scala：循环
来源：http://efm.hysaishi.cn

for (i <- 1 to 10) println(i)
来源：http://asv.gogol.net.cn

[T60] Scala：折叠
来源：http://qix.yonumen.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bwz.hywenlv.cn

================================================================================
来源：http://hez.svipenyu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yfo.andypj.xyz

================================================================================
来源：http://aeb.hongshengwenyu.top

[U01] Py：创建虚拟环境
来源：http://uwk.dianchejie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://rwt.yj20258888.top

[U02] Py：导出 / 安装依赖
来源：http://zki.hongshengwenyu.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cbz.zhiwuduotai.top

[U03] Py：加载 .env 配置
来源：http://kur.xuanzx.com

from dotenv import load_dotenv; load_dotenv()
来源：http://hya.shanyushiyangkeji.top

[U04] Py：变量调试打印
来源：http://xqu.gotoacloud.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vqc.chenjidiqi.icu

[U05] Py：列表去重且保序
来源：http://scx.ydjk.org.cn

list(dict.fromkeys(arr))
来源：http://yqi.guowangkeji.top

[U06] Py：合并两个字典
来源：http://suq.ctjpmb.com

{**a, **b}
来源：http://anu.jinyuanbaomall.cn

[U07] Py：反转字典键值
来源：http://dkm.fanxiaobao.xyz

{v: k for k, v in d.items()}
来源：http://pat.hcnkem.com

[U08] Py：展平二维列表
来源：http://acr.zhijiandao.cn

[y for x in nested for y in x]
来源：http://tii.meibo888.top

[U09] Py：字典取最大值的键
来源：http://vxy.zhengqikj.top

max(d, key=d.get)
来源：http://clw.quarkkingdee.top

[U10] Py：按值排序字典
来源：http://yln.aibaodan.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nik.fktsv.cn

[U11] Py：生成器表达式
来源：http://tvq.andypj.xyz

(x * 2 for x in arr)
来源：http://cag.snrcjt.cn

[U12] Py：取出现最多的 3 个元素
来源：http://kkt.jinghuilouyu.cn

Counter(arr).most_common(3)
来源：http://huz.cucudq.cn

[U13] Py：固定长度队列
来源：http://vao.yvedp.cn

deque(maxlen=10)
来源：http://tly.zhongyouzk.top

[U14] Py：分组收集到列表
来源：http://gne.shangyingyoupin.top

defaultdict(list)
来源：http://mhq.haohaochexian.top

[U15] Py：高精度计时
来源：http://lpd.hammf.cn

t = time.perf_counter()
来源：http://nas.yanxiufei.cn

[U16] Py：命令行参数解析
来源：http://xvw.shuidangran.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yld.yangfankeji.com

[U17] Py：初始化日志
来源：http://mgp.xuanzx.com

logging.basicConfig(level=logging.INFO)
来源：http://gdq.sxryk.cn

[U18] Py：预编译正则
来源：http://vie.nanxuanxn.top

pat = re.compile(r"\d+")
来源：http://btp.jlsjyb.cn

[U19] Py：正则替换带回调
来源：http://fwb.tianlin.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baf.shangyingyoupin.top

[U20] Py：缓存函数结果
来源：http://lnd.ivvv.top

@functools.lru_cache(maxsize=None)
来源：http://pax.sysykeji.top

[U21] Py：自定义上下文管理器
来源：http://eti.wangshuangyany.cn

@contextlib.contextmanager
来源：http://nei.xuetiantiany.cn

[U22] Py：矩阵转置
来源：http://wfx.jinyuanbaomall.cn

list(zip(*m))
来源：http://igu.jlsjyb.cn

[U23] Py：分块读取大文件
来源：http://rkp.316326.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://sas.gaohongyu789.top

[U24] Py：路径操作
来源：http://ptw.cdnleiting.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baw.daria6918.cn

[U25] Py：CSV 按字典读
来源：http://sxn.0kj1m.cn

csv.DictReader(f)
来源：http://fmu.redwolf501.top

[U26] Py：并发下载
来源：http://wcv.zhoulong.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tku.cucudq.cn

[U27] Py：异步 HTTP
来源：http://ljf.bbcook.cn

aiohttp.ClientSession() 配合 async with
来源：http://xqu.ydjk.org.cn

[U28] Py：类型别名
来源：http://lux.ydzc1.top

UserId = int
来源：http://ciu.ydjk.org.cn

[U29] Py：属性校验
来源：http://fwu.pycfn.com

@property 与 @x.setter 配合
来源：http://jnd.pycfn.com

[U30] Py：数据类
来源：http://yai.daxiang520.top

@dataclass(slots=True)
来源：http://bap.jinyuanbaomall.cn

[U31] Py：单测
来源：http://qsy.aibaodan.cn

python -m pytest -q
来源：http://aqw.xuetiantiany.cn

[U32] Py：代码格式化
来源：http://rvq.guannengcc.top

ruff format . && ruff check --fix .
来源：http://jhu.sxryk.cn

[U33] Py：打包发布
来源：http://yrc.bbcook.cn

python -m build  （依赖 pyproject.toml）
来源：http://ibk.zhiwuduotai.top

[U34] Py：判断编码
来源：http://upw.ctjpmb.com

chardet.detect(raw)
来源：http://ihx.mhx1999.top

[U35] Py：发送邮件
来源：http://wby.smart0.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fit.shanyushiyangtech.top

[U36] Py：定时任务
来源：http://bwb.cashguo.top

schedule.every(10).minutes.do(job)
来源：http://ecx.nwbrower.top

[U37] Py：读写 Excel
来源：http://neh.fzhhl.top

pandas.read_excel / DataFrame.to_excel
来源：http://tpz.yonumen.top

[U38] Py：获取脚本所在目录
来源：http://wxy.fktsv.cn

Path(__file__).resolve().parent
来源：http://oza.bbcook.cn

[U39] Py：判断是否在交互环境
来源：http://bls.sysykeji.top

sys.stdout.isatty()
来源：http://wok.zhengqikj.top

[U40] Py：打印到标准错误
来源：http://qgr.jinyuanbaomall.cn

print("err", file=sys.stderr)
来源：http://yzr.zhijiandao.cn

[U41] PHP：初始化 Composer 项目
来源：http://ecp.meibo888.top

composer init;  composer require guzzlehttp/guzzle
来源：http://uhe.jianghu66.top

[U42] PHP：PSR-4 自动加载
来源：http://xcz.zycfv.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ozz.xziqi.cn

[U43] PHP：声明命名空间
来源：http://cis.vehdjk.com

namespace App\Http;
来源：http://bsa.zdbjq.cn

[U44] PHP：开启严格类型
来源：http://sje.gogol.net.cn

declare(strict_types=1);
来源：http://brb.fzhhl.top

[U45] PHP：类型声明与返回类型
来源：http://izv.cheryme.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ief.hnxiangtu.top

[U46] PHP：可空类型
来源：http://hoq.tarul.cn

?string $name = null
来源：http://zwt.hnqzz.top

[U47] PHP：联合类型
来源：http://jyc.shanyushiyangkeji.top

int|string $id
来源：http://dbs.hywenlv.cn

[U48] PHP：纯枚举
来源：http://rnv.fzhhl.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wmm.shanyushiyangtech.top

[U49] PHP：只读属性
来源：http://nbw.hongshengwenyu.top

public readonly string $name
来源：http://ybs.zhijiandao.cn

[U50] PHP：构造器属性提升
来源：http://ian.chenlongwang.top

public function __construct(private int $id) {}
来源：http://jza.yj20258.top


<!-- 参考信息 -->