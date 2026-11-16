代发 wailian999

memset(a, 0, sizeof a);
来源：http://roa.xinyue.icu

[S27] C：定义常量
来源：http://nka.iojbl.cn

const double PI = 3.14159;
来源：http://dck.kuanghao11.cn

[S28] C：静态变量
来源：http://dxp.tarul.cn

static int counter = 0;
来源：http://adr.aibaodan.cn

[S29] C：变参函数
来源：http://biq.jinyuanbaomall.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jnz.0kj1m.cn

[S30] C：头文件保护
来源：http://qjz.birdmap.top

#ifndef X_H
来源：http://eqk.ctjpmb.com

#define X_H
来源：http://drw.ybcxt.top

#endif
来源：http://onk.cheryme.top

[S31] C++：Hello World
来源：http://nty.shanyushiyangkeji.top

#include <iostream>
来源：http://vsn.jlsjyb.cn

int main() { std::cout << "Hello\n"; }
来源：http://tsr.chenjidiqi.icu

[S32] C++：字符串
来源：http://ign.hammf.cn

std::string s = "hi";  s += "!";
来源：http://ocg.ywan-chungtsiang.top

[S33] C++：vector 增删
来源：http://qfw.shanyushiyangtech.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://obl.zhoulong.xyz

[S34] C++：遍历 vector
来源：http://bax.zycfv.cn

for (auto &x : v) { std::cout << x; }
来源：http://zqw.aibaodan.cn

[S35] C++：map
来源：http://mze.52xcode.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rsv.yueranfly.top

[S36] C++：unordered_map
来源：http://ofx.yj202588.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gum.ehwqpu.com

[S37] C++：set
来源：http://mzl.cucudq.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ycy.yueranfly.top

[S38] C++：排序
来源：http://mua.c1oappe.top

std::sort(v.begin(), v.end());
来源：http://nzs.jqgfzy.top

[S39] C++：自定义比较器排序
来源：http://seo.jqgufenzy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uwg.daria6918.cn

[S40] C++：查找元素
来源：http://wdn.xuetiantiany.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wzk.fktsv.cn

[S41] C++：类与构造函数
来源：http://xhr.quarkkingdee.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rtw.snrcjt.cn

[S42] C++：继承与虚函数
来源：http://fhw.redwolf501.top

class B : public Base { public: void f() override {} };
来源：http://jxt.cheryme.top

[S43] C++：智能指针
来源：http://lmh.jqgufenzy.top

auto p = std::make_unique<int>(5);
来源：http://zic.chenlongwang.top

[S44] C++：引用传参
来源：http://tjv.chenzaomai.com

void inc(int &x) { ++x; }
来源：http://xzk.yangfankeji.com

[S45] C++：lambda
来源：http://kwv.aibaodan.cn

auto add = [](int a, int b) { return a + b; };
来源：http://nte.zdbjq.cn

[S46] C++：函数模板
来源：http://sld.cqqwz.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://uuw.chenjidiqi.icu

[S47] C++：结构化绑定遍历
来源：http://yym.hnqzz.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ppq.guowangkeji.top

[S48] C++：逐行读文件
来源：http://anw.daxiang520.top

std::ifstream in("a.txt");  std::string line;
来源：http://sej.fehbvm.com

while (std::getline(in, line)) { }
来源：http://uhm.yj20258888.top

[S49] C++：写文件
来源：http://bwi.xingfuxueyuan.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fcm.gaohongyu789.top

[S50] C++：格式化数字
来源：http://wwo.xuanzx.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gts.hnqzz.top

[S51] C++：显式类型转换
来源：http://odl.nwbrower.top

static_cast<double>(a) / b
来源：http://msf.aizwys.cn

[S52] C++：const 与 noexcept
来源：http://fdp.shanyushiyangtech.top

int size() const noexcept { return n_; }
来源：http://ybu.xylfe.cn

[S53] C++：移动语义
来源：http://jvt.ehwqpu.com

std::vector<int> w = std::move(v);
来源：http://ikw.jinyuanbaomall.cn

[S54] C++：异常处理
来源：http://dyu.yongpay.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://urc.jianghu66.top

[S55] C++：结构化绑定
来源：http://ppr.yueranfly.top

auto [a, b] = std::make_pair(1, 2);
来源：http://hic.jyoumei.cn

[S56] C++：optional
来源：http://bme.birdmap.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gql.svipenyu.cn

[S57] C++：编译期常量
来源：http://cfy.ybcxt.top

constexpr int N = 10;
来源：http://flr.bjfxy.top

[S58] C++：命名空间
来源：http://fci.9152youxi.cn

namespace ns { int f() { return 1; } }
来源：http://jyq.shangyingyoupin.top

[S59] C++：静态断言
来源：http://vqc.yonumen.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rxr.nanxuanxn.top

[S60] C++：遍历并删除元素
来源：http://cmo.yonumen.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://shy.ybcxt.top

================================================================================
来源：http://qgf.yj20258888.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ggt.quarkkingdee.top

================================================================================
来源：http://zuv.c1oappe.top

[T01] Kotlin：Hello World
来源：http://pis.0kj1m.cn

println("Hello")
来源：http://dgx.hesvh.cn

[T02] Kotlin：变量
来源：http://fwh.shzxlz.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wot.jlsjyb.cn

[T03] Kotlin：字符串模板
来源：http://hkg.jinqigufen.top

"值: $b"
来源：http://nyg.52xcode.cn

[T04] Kotlin：空安全
来源：http://hrs.aibaodan.cn

val n: String? = null;  n?.length
来源：http://pza.wangshuangyany.cn

[T05] Kotlin：when 表达式
来源：http://rtg.jinghuilouyu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gfs.ydzc1.top

[T06] Kotlin：集合映射
来源：http://cxp.zhiwuduotai.top

listOf(1, 2, 3).map { it * 2 }
来源：http://wyv.ybcxt.top

[T07] Kotlin：集合过滤
来源：http://yrx.xinyue.icu

listOf(1, 2, 3).filter { it > 1 }
来源：http://bcu.yuanzhike.top

[T08] Kotlin：数据类
来源：http://fab.tanke756.top

data class User(val name: String, val age: Int)
来源：http://mni.cucudq.cn

[T09] Kotlin：扩展函数
来源：http://exx.shanyushiyangtech.top

fun String.exclaim() = this + "!"
来源：http://gip.zhoulong.xyz

[T10] Kotlin：默认参数
来源：http://tad.316326.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://fcq.cqqwz.cn

[T11] Kotlin：协程
来源：http://ncb.zhoulong.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://phf.zhongyouzk.top

[T12] Kotlin：解构声明
来源：http://iwd.havefunace.top

val (a, b) = Pair(1, 2)
来源：http://odt.zhongyouzk.top

[T13] Kotlin：只读 Map
来源：http://fle.wangshuangyany.cn

val m = mapOf("a" to 1)
来源：http://hga.zdqjudy.top

[T14] Kotlin：循环
来源：http://sds.nanxuanxn.top

for (i in 1..10) println(i)
来源：http://edb.svipenyu.cn

[T15] Kotlin：接口
来源：http://eqf.fktsv.cn

interface Shape { fun area(): Double }
来源：http://hjq.fanxiaobao.xyz

[T16] Swift：Hello World
来源：http://etx.zdqjudy.top

print("Hello")
来源：http://xhs.sufxvd.cn

[T17] Swift：变量与常量
来源：http://dfs.ywan-chungtsiang.top

var a = 1;  let b = 2
来源：http://bvy.tarul.cn

[T18] Swift：字符串插值
来源：http://iln.zycfv.cn

"值: \(b)"
来源：http://wul.vehdjk.com

[T19] Swift：可选绑定
来源：http://ngy.ivvv.top

if let n = opt { print(n) }
来源：http://qgj.sxryk.cn

[T20] Swift：数组操作
来源：http://dwh.daria6918.cn

var a = [1, 2, 3];  a.append(4)
来源：http://nxe.daxiang520.top

[T21] Swift：遍历
来源：http://rpf.yvedp.cn

for x in a { print(x) }
来源：http://kcx.yuxming.cn

[T22] Swift：字典
来源：http://yfl.gaohongyu789.top

var d = ["a": 1];  d["b"] = 2
来源：http://sdd.zhengqikj.top

[T23] Swift：函数
来源：http://upc.c1oappe.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://sxl.0kj1m.cn

[T24] Swift：闭包
来源：http://wes.cashguo.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://kap.guannengcc.top

[T25] Swift：结构体
来源：http://hwi.wangdashe.top

struct P { var x: Int }
来源：http://tfm.hcnkem.com

[T26] Swift：类与重写
来源：http://vjo.hesvh.cn

class A: Base { override func f() {} }
来源：http://kxi.hongshengwenyu.top

[T27] Swift：错误处理
来源：http://eeg.jinghuilouyu.cn

do { try f() } catch { print(error) }
来源：http://rnf.birdmap.top

[T28] Swift：枚举
来源：http://lcg.ppjwa.cn

enum Color { case red, green }
来源：http://mri.fanxiaobao.xyz

[T29] Swift：guard 提前返回
来源：http://hxq.chenzaomai.com

guard let x = opt else { return }
来源：http://iml.kuanghao11.cn

[T30] Swift：协议
来源：http://xuw.hnxiangtu.top

protocol Shape { func area() -> Double }
来源：http://ctw.jinqigufen.top

[T31] Lua：Hello World
来源：http://rzv.havefunace.top

print("Hello")
来源：http://wdk.xuanzx.com

[T32] Lua：局部变量
来源：http://rgo.aibaodan.cn

local a = 1
来源：http://yov.shuidangran.top

[T33] Lua：表（数组）
来源：http://pnm.guannengcc.top

local t = {1, 2, 3};  t[4] = 4
来源：http://kcb.zhoulong.xyz

[T34] Lua：遍历表
来源：http://lmz.kuanghao11.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://eon.xuanzx.com

[T35] Lua：字典表
来源：http://qis.redwolf501.top

local d = { a = 1 };  d.b = 2
来源：http://ifg.c1oappe.top

[T36] Lua：函数
来源：http://pfa.nwbrower.top

function add(a, b) return a + b end
来源：http://jes.bbcook.cn

[T37] Lua：字符串拼接
来源：http://boc.tianlin.xyz

"a" .. "b"
来源：http://jek.fehbvm.com

[T38] Lua：条件
来源：http://jhv.zdbjq.cn

if x > 0 then print("正") end
来源：http://jrd.zhongyouzk.top

[T39] Lua：模式匹配
来源：http://wct.hnqzz.top

string.find(s, "%d+")
来源：http://dsp.bbcook.cn

[T40] Lua：元表
来源：http://yhd.hongshengwenyu.top

setmetatable({}, { __index = base })
来源：http://jit.jiagoushi.top

[T41] Perl：Hello World
来源：http://uwt.iojbl.cn

print "Hello\n";
来源：http://zut.ivvv.top

[T42] Perl：变量类型
来源：http://mks.cucudq.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://sei.c1oappe.top

[T43] Perl：字符串插值
来源：http://ize.yvedp.cn

"值: $a"
来源：http://ewx.quarkkingdee.top

[T44] Perl：条件
来源：http://dgc.ctjpmb.com

if ($a > 0) { print "正"; }
来源：http://wun.jqgufenzy.top

[T45] Perl：数组遍历
来源：http://bvr.yuxming.cn

for my $x (@arr) { print $x; }
来源：http://xbl.9152youxi.cn

[T46] Perl：哈希操作
来源：http://xgl.sysykeji.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lxs.yanxiufei.cn

[T47] Perl：正则捕获
来源：http://lnx.vehdjk.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://lqw.kuanghao11.cn

[T48] Perl：正则替换
来源：http://oie.hnqzz.top

$s =~ s/old/new/g;
来源：http://mza.jqgufenzy.top

[T49] Perl：函数
来源：http://oet.gogol.net.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gra.wangshuangyany.cn

[T50] Perl：逐行读文件
来源：http://lcc.nanxuanxn.top

open my $fh, "<", "a.txt" or die $!;
来源：http://kur.c1oappe.top

while (my $line = <$fh>) { print $line; }
来源：http://euq.0kj1m.cn

[T51] Scala：Hello World
来源：http://cju.quarkkingdee.top

println("Hello")
来源：http://cxw.jiagoushi.top

[T52] Scala：变量
来源：http://zpq.sxryk.cn

val a = 1;  var b = 2
来源：http://vcp.jyoumei.cn

[T53] Scala：字符串插值
来源：http://lmv.shanyushiyangtech.top

s"值: $b"
来源：http://epk.guannengcc.top

[T54] Scala：集合映射
来源：http://qwi.pengpengdd.cyou

List(1, 2, 3).map(_ * 2)
来源：http://aep.shuidangran.top

[T55] Scala：集合过滤
来源：http://eej.zhiwuduotai.top

List(1, 2, 3).filter(_ > 1)
来源：http://bts.fehbvm.com

[T56] Scala：样例类
来源：http://pch.hammf.cn

case class User(name: String, age: Int)
来源：http://nxf.zhixingplan.top

[T57] Scala：模式匹配
来源：http://vzi.kuanghao11.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://pho.snrcjt.cn

[T58] Scala：函数定义
来源：http://hkb.jinqigufen.top

def add(a: Int, b: Int): Int = a + b
来源：http://qye.pycfn.com

[T59] Scala：循环
来源：http://vil.zycfv.cn

for (i <- 1 to 10) println(i)
来源：http://jtg.jyoumei.cn

[T60] Scala：折叠
来源：http://tpk.vehdjk.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bkp.wangshuangyany.cn

================================================================================
来源：http://vvf.shanyushiyangtech.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ydb.havefunace.top

================================================================================
来源：http://qza.hcnkem.com

[U01] Py：创建虚拟环境
来源：http://aaa.iojbl.cn

python -m venv .venv && source .venv/bin/activate
来源：http://mge.yonumen.top

[U02] Py：导出 / 安装依赖
来源：http://fqz.jyoumei.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hfz.mhx1999.top

[U03] Py：加载 .env 配置
来源：http://fxt.jiagoushi.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ntx.chenzaomai.com

[U04] Py：变量调试打印
来源：http://hga.fengsongda.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://iei.yj20258888.top

[U05] Py：列表去重且保序
来源：http://hyn.c1oappe.top

list(dict.fromkeys(arr))
来源：http://qrc.xingfuxueyuan.xyz

[U06] Py：合并两个字典
来源：http://prj.pengpengdd.cyou

{**a, **b}
来源：http://rka.kuanghao11.cn

[U07] Py：反转字典键值
来源：http://sex.yvedp.cn

{v: k for k, v in d.items()}
来源：http://bsf.cashguo.top

[U08] Py：展平二维列表
来源：http://aty.zhijiandao.cn

[y for x in nested for y in x]
来源：http://klm.nanxuanxn.top

[U09] Py：字典取最大值的键
来源：http://wdx.jlsjyb.cn

max(d, key=d.get)
来源：http://uic.jyoumei.cn

[U10] Py：按值排序字典
来源：http://vjn.chenzaomai.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://foj.fehbvm.com

[U11] Py：生成器表达式
来源：http://wxx.iojbl.cn

(x * 2 for x in arr)
来源：http://eng.jinyuanbaomall.cn

[U12] Py：取出现最多的 3 个元素
来源：http://huh.smart0.xyz

Counter(arr).most_common(3)
来源：http://fhf.hammf.cn

[U13] Py：固定长度队列
来源：http://fqm.sweek.top

deque(maxlen=10)
来源：http://snk.tarul.cn

[U14] Py：分组收集到列表
来源：http://iez.zhixingplan.top

defaultdict(list)
来源：http://tkp.tian-w.cn

[U15] Py：高精度计时
来源：http://mng.bbcook.cn

t = time.perf_counter()
来源：http://yvz.feifeiyinyue.top

[U16] Py：命令行参数解析
来源：http://duf.fengsongda.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hhe.zdbjq.cn

[U17] Py：初始化日志
来源：http://moq.jqgufenzy.top

logging.basicConfig(level=logging.INFO)
来源：http://adz.yangfankeji.com

[U18] Py：预编译正则
来源：http://exb.cheryme.top

pat = re.compile(r"\d+")
来源：http://qpk.gogol.net.cn

[U19] Py：正则替换带回调
来源：http://uoi.dianchejie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hli.jlsjyb.cn

[U20] Py：缓存函数结果
来源：http://uzw.gzhubu.top

@functools.lru_cache(maxsize=None)
来源：http://kup.yongpay.top

[U21] Py：自定义上下文管理器
来源：http://pbv.zhongyouzk.top

@contextlib.contextmanager
来源：http://jtz.yj20258.top

[U22] Py：矩阵转置
来源：http://pse.hywenlv.cn

list(zip(*m))
来源：http://lxc.andypj.xyz

[U23] Py：分块读取大文件
来源：http://jhs.xuanzx.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bgp.guannengcc.top

[U24] Py：路径操作
来源：http://cjh.dashuyun.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vux.feifeiyinyue.top

[U25] Py：CSV 按字典读
来源：http://lvl.fktsv.cn

csv.DictReader(f)
来源：http://sxl.redwolf501.top

[U26] Py：并发下载
来源：http://zxj.uphjek.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xwn.pycfn.com

[U27] Py：异步 HTTP
来源：http://maw.cqqwz.cn

aiohttp.ClientSession() 配合 async with
来源：http://tpp.52xcode.cn

[U28] Py：类型别名
来源：http://omm.hnxiangtu.top

UserId = int
来源：http://gdz.iojbl.cn

[U29] Py：属性校验
来源：http://oyg.hesvh.cn

@property 与 @x.setter 配合
来源：http://zik.yj20258.top

[U30] Py：数据类
来源：http://tzd.zdbjq.cn

@dataclass(slots=True)
来源：http://olc.hysaishi.cn

[U31] Py：单测
来源：http://yec.meibo888.top

python -m pytest -q
来源：http://iwe.gaohongyu789.top

[U32] Py：代码格式化
来源：http://vlv.hfpthk.cn

ruff format . && ruff check --fix .
来源：http://bgp.cucudq.cn

[U33] Py：打包发布
来源：http://ogj.haohaochexian.top

python -m build  （依赖 pyproject.toml）
来源：http://rzc.zhiwuduotai.top

[U34] Py：判断编码
来源：http://bio.xuanzx.com

chardet.detect(raw)
来源：http://xwa.chenzaomai.com

[U35] Py：发送邮件
来源：http://zml.ydzc1.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://awh.vqdsnc.cn

[U36] Py：定时任务
来源：http://emt.gaohongyu789.top

schedule.every(10).minutes.do(job)
来源：http://pho.guannengcc.top

[U37] Py：读写 Excel
来源：http://dqt.gzhubu.top

pandas.read_excel / DataFrame.to_excel
来源：http://kdp.ydzc1.top

[U38] Py：获取脚本所在目录
来源：http://dtb.ctjpmb.com

Path(__file__).resolve().parent
来源：http://bah.tianlin.xyz

[U39] Py：判断是否在交互环境
来源：http://yiw.ppjwa.cn

sys.stdout.isatty()
来源：http://dxi.fzhhl.top

[U40] Py：打印到标准错误
来源：http://fbv.cheryme.top

print("err", file=sys.stderr)
来源：http://qec.zhiwuduotai.top

[U41] PHP：初始化 Composer 项目
来源：http://brg.svipenyu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://hok.aibaodan.cn

[U42] PHP：PSR-4 自动加载
来源：http://ebf.dashuyun.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bmo.jianghu66.top

[U43] PHP：声明命名空间
来源：http://yyq.cdnleiting.top

namespace App\Http;
来源：http://hlo.zhengqikj.top

[U44] PHP：开启严格类型
来源：http://mms.jianghu66.top

declare(strict_types=1);
来源：http://bnb.zhixingplan.top

[U45] PHP：类型声明与返回类型
来源：http://vdt.zhongyouzk.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://pva.svipenyu.cn

[U46] PHP：可空类型
来源：http://kdh.xziqi.cn

?string $name = null
来源：http://cdt.guannengcc.top

[U47] PHP：联合类型
来源：http://rol.pycfn.com

int|string $id
来源：http://bhx.yangfankeji.com

[U48] PHP：纯枚举
来源：http://tyf.xuetiantiany.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kaq.jinghuilouyu.cn

[U49] PHP：只读属性
来源：http://urp.sufxvd.cn

public readonly string $name
来源：http://cyp.cashguo.top

[U50] PHP：构造器属性提升
来源：http://rqa.cashguo.top

public function __construct(private int $id) {}
来源：http://hdx.9152youxi.cn


<!-- 参考信息 -->