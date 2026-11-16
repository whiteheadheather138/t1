代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cbf.sweek.top

[S25] C：内存拷贝
来源：http://tia.yvedp.cn

memcpy(dst, src, n);
来源：http://jap.daria6918.cn

[S26] C：内存清零
来源：http://rsx.tarul.cn

memset(a, 0, sizeof a);
来源：http://wyu.redwolf501.top

[S27] C：定义常量
来源：http://vcc.yangfankeji.com

const double PI = 3.14159;
来源：http://cdh.xziqi.cn

[S28] C：静态变量
来源：http://aoq.sweek.top

static int counter = 0;
来源：http://kmd.shangyingyoupin.top

[S29] C：变参函数
来源：http://icb.uphjek.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://izl.ppjwa.cn

[S30] C：头文件保护
来源：http://vrg.aizwys.cn

#ifndef X_H
来源：http://wqp.tianlin.xyz

#define X_H
来源：http://ogs.shanyushiyangtech.top

#endif
来源：http://ovv.bbcook.cn

[S31] C++：Hello World
来源：http://klh.ehwqpu.com

#include <iostream>
来源：http://vda.daxiang520.top

int main() { std::cout << "Hello\n"; }
来源：http://bpq.dianchejie.cn

[S32] C++：字符串
来源：http://prk.chenjidiqi.icu

std::string s = "hi";  s += "!";
来源：http://saf.zdqjudy.top

[S33] C++：vector 增删
来源：http://gjk.nanxinkj.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xnn.svipenyu.cn

[S34] C++：遍历 vector
来源：http://bdd.yangfankeji.com

for (auto &x : v) { std::cout << x; }
来源：http://bbe.yj20258888.top

[S35] C++：map
来源：http://gsh.yongpay.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nsx.bbcook.cn

[S36] C++：unordered_map
来源：http://bgk.sysykeji.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tjd.sweek.top

[S37] C++：set
来源：http://ixa.xylfe.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rgd.gzhubu.top

[S38] C++：排序
来源：http://ycr.zhaomingkeji.xyz

std::sort(v.begin(), v.end());
来源：http://nzs.ywan-chungtsiang.top

[S39] C++：自定义比较器排序
来源：http://fto.ctjpmb.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://oue.yj20258.top

[S40] C++：查找元素
来源：http://kij.hcnkem.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gcu.c1oappe.top

[S41] C++：类与构造函数
来源：http://nze.jiagoushi.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://prl.jinghuilouyu.cn

[S42] C++：继承与虚函数
来源：http://xfz.xylfe.cn

class B : public Base { public: void f() override {} };
来源：http://bhn.hcnkem.com

[S43] C++：智能指针
来源：http://zlt.xziqi.cn

auto p = std::make_unique<int>(5);
来源：http://bgd.zhiwuduotai.top

[S44] C++：引用传参
来源：http://dsf.pengpengdd.cyou

void inc(int &x) { ++x; }
来源：http://aib.jyoumei.cn

[S45] C++：lambda
来源：http://vjk.tarul.cn

auto add = [](int a, int b) { return a + b; };
来源：http://mrx.jyoumei.cn

[S46] C++：函数模板
来源：http://dvc.jlsjyb.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xsf.zhengqikj.top

[S47] C++：结构化绑定遍历
来源：http://jkn.cucudq.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bma.yj202588.top

[S48] C++：逐行读文件
来源：http://iho.gzhubu.top

std::ifstream in("a.txt");  std::string line;
来源：http://bcm.vehdjk.com

while (std::getline(in, line)) { }
来源：http://qlp.hysaishi.cn

[S49] C++：写文件
来源：http://baa.jlsjyb.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tii.chenjidiqi.icu

[S50] C++：格式化数字
来源：http://mvr.yonumen.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hvd.shangyingyoupin.top

[S51] C++：显式类型转换
来源：http://sif.0kj1m.cn

static_cast<double>(a) / b
来源：http://qqk.cqqwz.cn

[S52] C++：const 与 noexcept
来源：http://fsm.nwbrower.top

int size() const noexcept { return n_; }
来源：http://bao.tian-w.cn

[S53] C++：移动语义
来源：http://keo.zhaomingkeji.xyz

std::vector<int> w = std::move(v);
来源：http://ugz.zhaomingkeji.xyz

[S54] C++：异常处理
来源：http://zuu.zhiwuduotai.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gmw.cqqwz.cn

[S55] C++：结构化绑定
来源：http://ubu.uphjek.com

auto [a, b] = std::make_pair(1, 2);
来源：http://ikq.wangdashe.top

[S56] C++：optional
来源：http://bbh.aizwys.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gim.shangyingyoupin.top

[S57] C++：编译期常量
来源：http://dgw.guowangkeji.top

constexpr int N = 10;
来源：http://sid.yuxming.cn

[S58] C++：命名空间
来源：http://moz.zdbjq.cn

namespace ns { int f() { return 1; } }
来源：http://mkl.jinqigufen.top

[S59] C++：静态断言
来源：http://ord.epnwcf.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vst.jianghu66.top

[S60] C++：遍历并删除元素
来源：http://egp.chenlongwang.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://trw.svipenyu.cn

================================================================================
来源：http://tqn.sufxvd.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hqb.shuidangran.top

================================================================================
来源：http://itu.cdnleiting.top

[T01] Kotlin：Hello World
来源：http://giw.meibo888.top

println("Hello")
来源：http://kkq.cqqwz.cn

[T02] Kotlin：变量
来源：http://ebn.ctjpmb.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ouz.pycfn.com

[T03] Kotlin：字符串模板
来源：http://pns.ivvv.top

"值: $b"
来源：http://pja.shangyingyoupin.top

[T04] Kotlin：空安全
来源：http://klw.fktsv.cn

val n: String? = null;  n?.length
来源：http://enp.ywan-chungtsiang.top

[T05] Kotlin：when 表达式
来源：http://whf.tarul.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sgw.tianlin.xyz

[T06] Kotlin：集合映射
来源：http://tns.yueranfly.top

listOf(1, 2, 3).map { it * 2 }
来源：http://cvc.havefunace.top

[T07] Kotlin：集合过滤
来源：http://ysz.zdbjq.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://vbu.shanyushiyangkeji.top

[T08] Kotlin：数据类
来源：http://yua.ppjwa.cn

data class User(val name: String, val age: Int)
来源：http://vty.sxryk.cn

[T09] Kotlin：扩展函数
来源：http://pvn.jianghu66.top

fun String.exclaim() = this + "!"
来源：http://zrj.iojbl.cn

[T10] Kotlin：默认参数
来源：http://vah.wangshuangyany.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://spu.bjfxy.top

[T11] Kotlin：协程
来源：http://hbb.hammf.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://rbv.cqqwz.cn

[T12] Kotlin：解构声明
来源：http://wbj.yj20258888.top

val (a, b) = Pair(1, 2)
来源：http://lgg.svipenyu.cn

[T13] Kotlin：只读 Map
来源：http://rnv.sweek.top

val m = mapOf("a" to 1)
来源：http://owt.ydjk.org.cn

[T14] Kotlin：循环
来源：http://xpp.yonumen.top

for (i in 1..10) println(i)
来源：http://hic.hfpthk.cn

[T15] Kotlin：接口
来源：http://lyj.chenzaomai.com

interface Shape { fun area(): Double }
来源：http://smh.52xcode.cn

[T16] Swift：Hello World
来源：http://eaq.pengpengdd.cyou

print("Hello")
来源：http://mio.xuetiantiany.cn

[T17] Swift：变量与常量
来源：http://tvh.sxryk.cn

var a = 1;  let b = 2
来源：http://zlb.mhx1999.top

[T18] Swift：字符串插值
来源：http://gbr.jyoumei.cn

"值: \(b)"
来源：http://pog.meibo888.top

[T19] Swift：可选绑定
来源：http://ggs.c1oappe.top

if let n = opt { print(n) }
来源：http://siw.feifeiyinyue.top

[T20] Swift：数组操作
来源：http://txt.fzhhl.top

var a = [1, 2, 3];  a.append(4)
来源：http://ial.yanxiufei.cn

[T21] Swift：遍历
来源：http://ysh.zhaomingkeji.xyz

for x in a { print(x) }
来源：http://lmi.chenlongwang.top

[T22] Swift：字典
来源：http://jxv.hnxiangtu.top

var d = ["a": 1];  d["b"] = 2
来源：http://ivl.vqdsnc.cn

[T23] Swift：函数
来源：http://ioc.andypj.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tgi.vqdsnc.cn

[T24] Swift：闭包
来源：http://apn.guannengcc.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://tyc.ybcxt.top

[T25] Swift：结构体
来源：http://lvg.yj20258888.top

struct P { var x: Int }
来源：http://hrf.zhixingplan.top

[T26] Swift：类与重写
来源：http://zkn.gotoacloud.top

class A: Base { override func f() {} }
来源：http://rmb.0kj1m.cn

[T27] Swift：错误处理
来源：http://wcg.zhongyouzk.top

do { try f() } catch { print(error) }
来源：http://lfn.gzhubu.top

[T28] Swift：枚举
来源：http://vld.hywenlv.cn

enum Color { case red, green }
来源：http://kjk.zdqjudy.top

[T29] Swift：guard 提前返回
来源：http://lko.ivvv.top

guard let x = opt else { return }
来源：http://nvg.jyoumei.cn

[T30] Swift：协议
来源：http://ral.hammf.cn

protocol Shape { func area() -> Double }
来源：http://saq.tanke756.top

[T31] Lua：Hello World
来源：http://krw.ydjk.org.cn

print("Hello")
来源：http://gyw.cheryme.top

[T32] Lua：局部变量
来源：http://zyh.wangshuangyany.cn

local a = 1
来源：http://jus.tarul.cn

[T33] Lua：表（数组）
来源：http://eaz.uphjek.com

local t = {1, 2, 3};  t[4] = 4
来源：http://crk.tanke756.top

[T34] Lua：遍历表
来源：http://vid.ydzc1.top

for i, v in ipairs(t) do print(i, v) end
来源：http://yro.jinyuanbaomall.cn

[T35] Lua：字典表
来源：http://gma.yj20258.top

local d = { a = 1 };  d.b = 2
来源：http://qlf.shanyushiyangtech.top

[T36] Lua：函数
来源：http://izl.c1oappe.top

function add(a, b) return a + b end
来源：http://oaw.yonumen.top

[T37] Lua：字符串拼接
来源：http://oye.hywenlv.cn

"a" .. "b"
来源：http://xgq.gzhubu.top

[T38] Lua：条件
来源：http://czv.jinqigufen.top

if x > 0 then print("正") end
来源：http://nso.daxiang520.top

[T39] Lua：模式匹配
来源：http://mjx.daxiang520.top

string.find(s, "%d+")
来源：http://usr.chenzaomai.com

[T40] Lua：元表
来源：http://tkc.jinghuilouyu.cn

setmetatable({}, { __index = base })
来源：http://kxs.iojbl.cn

[T41] Perl：Hello World
来源：http://unz.xziqi.cn

print "Hello\n";
来源：http://txf.yongpay.top

[T42] Perl：变量类型
来源：http://tou.zycfv.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lrb.meibo888.top

[T43] Perl：字符串插值
来源：http://wpl.feifeiyinyue.top

"值: $a"
来源：http://ymb.sxryk.cn

[T44] Perl：条件
来源：http://ous.zdbjq.cn

if ($a > 0) { print "正"; }
来源：http://pie.cqqwz.cn

[T45] Perl：数组遍历
来源：http://dtm.meibo888.top

for my $x (@arr) { print $x; }
来源：http://ymo.xylfe.cn

[T46] Perl：哈希操作
来源：http://msl.jinqigufen.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://aah.yongpay.top

[T47] Perl：正则捕获
来源：http://wky.fanxiaobao.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://aqc.cqqwz.cn

[T48] Perl：正则替换
来源：http://flb.zhongyouzk.top

$s =~ s/old/new/g;
来源：http://guk.bjfxy.top

[T49] Perl：函数
来源：http://fzo.nwbrower.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qvc.yanxiufei.cn

[T50] Perl：逐行读文件
来源：http://wbr.gzhubu.top

open my $fh, "<", "a.txt" or die $!;
来源：http://egs.xylfe.cn

while (my $line = <$fh>) { print $line; }
来源：http://wis.uphjek.com

[T51] Scala：Hello World
来源：http://vju.hesvh.cn

println("Hello")
来源：http://rft.jqgufenzy.top

[T52] Scala：变量
来源：http://wuc.yj20258.top

val a = 1;  var b = 2
来源：http://dhi.hfpthk.cn

[T53] Scala：字符串插值
来源：http://ksp.jqgufenzy.top

s"值: $b"
来源：http://cys.zhijiandao.cn

[T54] Scala：集合映射
来源：http://znl.kuanghao11.cn

List(1, 2, 3).map(_ * 2)
来源：http://ceo.birdmap.top

[T55] Scala：集合过滤
来源：http://kvu.xinyue.icu

List(1, 2, 3).filter(_ > 1)
来源：http://adq.nwbrower.top

[T56] Scala：样例类
来源：http://bvq.uphjek.com

case class User(name: String, age: Int)
来源：http://jhv.shanyushiyangtech.top

[T57] Scala：模式匹配
来源：http://awx.zdqjudy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://efp.dianchejie.cn

[T58] Scala：函数定义
来源：http://vbt.fehbvm.com

def add(a: Int, b: Int): Int = a + b
来源：http://ghq.redwolf501.top

[T59] Scala：循环
来源：http://oet.sysykeji.top

for (i <- 1 to 10) println(i)
来源：http://yxx.xziqi.cn

[T60] Scala：折叠
来源：http://jto.yongpay.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nml.shanyushiyangkeji.top

================================================================================
来源：http://gsd.xylfe.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wvx.yuanzhike.top

================================================================================
来源：http://iwr.wangdashe.top

[U01] Py：创建虚拟环境
来源：http://rhn.jinyuanbaomall.cn

python -m venv .venv && source .venv/bin/activate
来源：http://bwf.xingfuxueyuan.xyz

[U02] Py：导出 / 安装依赖
来源：http://kbp.bjfxy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://avu.zhengqikj.top

[U03] Py：加载 .env 配置
来源：http://upg.yanxiufei.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://swq.yj20258.top

[U04] Py：变量调试打印
来源：http://jse.svipenyu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dbe.zhoulong.xyz

[U05] Py：列表去重且保序
来源：http://myw.smart0.xyz

list(dict.fromkeys(arr))
来源：http://gqi.nanxinkj.top

[U06] Py：合并两个字典
来源：http://fpc.c1oappe.top

{**a, **b}
来源：http://gtx.xingfuxueyuan.xyz

[U07] Py：反转字典键值
来源：http://ulc.yj202588.top

{v: k for k, v in d.items()}
来源：http://caj.sweek.top

[U08] Py：展平二维列表
来源：http://vsw.havefunace.top

[y for x in nested for y in x]
来源：http://fqx.hcnkem.com

[U09] Py：字典取最大值的键
来源：http://pnh.daxiang520.top

max(d, key=d.get)
来源：http://euc.wangdashe.top

[U10] Py：按值排序字典
来源：http://qzt.sysykeji.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://frk.zhaomingkeji.xyz

[U11] Py：生成器表达式
来源：http://oum.hcnkem.com

(x * 2 for x in arr)
来源：http://qel.sufxvd.cn

[U12] Py：取出现最多的 3 个元素
来源：http://rwy.hysaishi.cn

Counter(arr).most_common(3)
来源：http://sha.9152youxi.cn

[U13] Py：固定长度队列
来源：http://rxr.gaohongyu789.top

deque(maxlen=10)
来源：http://vtk.cqqwz.cn

[U14] Py：分组收集到列表
来源：http://hbl.shanyushiyangkeji.top

defaultdict(list)
来源：http://zah.fktsv.cn

[U15] Py：高精度计时
来源：http://ilu.bbcook.cn

t = time.perf_counter()
来源：http://iei.ctjpmb.com

[U16] Py：命令行参数解析
来源：http://tec.wangdashe.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lvu.mhx1999.top

[U17] Py：初始化日志
来源：http://siv.bjfxy.top

logging.basicConfig(level=logging.INFO)
来源：http://vhb.zhengqikj.top

[U18] Py：预编译正则
来源：http://tgd.ydjk.org.cn

pat = re.compile(r"\d+")
来源：http://ion.yj20258.top

[U19] Py：正则替换带回调
来源：http://fvw.jqgufenzy.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://brx.zhoulong.xyz

[U20] Py：缓存函数结果
来源：http://hag.sweek.top

@functools.lru_cache(maxsize=None)
来源：http://pxb.wangshuangyany.cn

[U21] Py：自定义上下文管理器
来源：http://xyw.jqgufenzy.top

@contextlib.contextmanager
来源：http://wke.zhijiandao.cn

[U22] Py：矩阵转置
来源：http://hhx.hnqzz.top

list(zip(*m))
来源：http://gli.jiagoushi.top

[U23] Py：分块读取大文件
来源：http://sgi.aizwys.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://slg.gogol.net.cn

[U24] Py：路径操作
来源：http://mfp.hfpthk.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vnn.wangshuangyany.cn

[U25] Py：CSV 按字典读
来源：http://rzs.hnqzz.top

csv.DictReader(f)
来源：http://qpi.0kj1m.cn

[U26] Py：并发下载
来源：http://dnp.sweek.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lwg.andypj.xyz

[U27] Py：异步 HTTP
来源：http://snu.tanke756.top

aiohttp.ClientSession() 配合 async with
来源：http://cgn.hnqzz.top

[U28] Py：类型别名
来源：http://qcv.shanyushiyangtech.top

UserId = int
来源：http://hvq.xziqi.cn

[U29] Py：属性校验
来源：http://qok.ydzc1.top

@property 与 @x.setter 配合
来源：http://dld.fengsongda.top

[U30] Py：数据类
来源：http://avl.zhiwuduotai.top

@dataclass(slots=True)
来源：http://qhj.ppjwa.cn

[U31] Py：单测
来源：http://edo.ivvv.top

python -m pytest -q
来源：http://ljm.c1oappe.top

[U32] Py：代码格式化
来源：http://pjv.wangshuangyany.cn

ruff format . && ruff check --fix .
来源：http://vxq.zhiwuduotai.top

[U33] Py：打包发布
来源：http://zni.jiagoushi.top

python -m build  （依赖 pyproject.toml）
来源：http://hgd.daria6918.cn

[U34] Py：判断编码
来源：http://tdw.iojbl.cn

chardet.detect(raw)
来源：http://bon.guannengcc.top

[U35] Py：发送邮件
来源：http://beq.snrcjt.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ogv.dashuyun.cn

[U36] Py：定时任务
来源：http://adz.vqdsnc.cn

schedule.every(10).minutes.do(job)
来源：http://njo.yfazqb.com

[U37] Py：读写 Excel
来源：http://oxi.yueranfly.top

pandas.read_excel / DataFrame.to_excel
来源：http://qiy.andypj.xyz

[U38] Py：获取脚本所在目录
来源：http://nvd.yj20258888.top

Path(__file__).resolve().parent
来源：http://qnh.yanxiufei.cn

[U39] Py：判断是否在交互环境
来源：http://upv.mhx1999.top

sys.stdout.isatty()
来源：http://tsu.yj20258888.top

[U40] Py：打印到标准错误
来源：http://zht.jinyuanbaomall.cn

print("err", file=sys.stderr)
来源：http://zuw.jinyuanbaomall.cn

[U41] PHP：初始化 Composer 项目
来源：http://hfj.haohaochexian.top

composer init;  composer require guzzlehttp/guzzle
来源：http://fvt.nanxinkj.top

[U42] PHP：PSR-4 自动加载
来源：http://udm.vehdjk.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vos.yanxiufei.cn

[U43] PHP：声明命名空间
来源：http://ljh.sxryk.cn

namespace App\Http;
来源：http://zrg.aizwys.cn

[U44] PHP：开启严格类型
来源：http://ild.shangyingyoupin.top

declare(strict_types=1);
来源：http://zks.yj202588.top

[U45] PHP：类型声明与返回类型
来源：http://bvs.jinqigfzy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://njt.tianlin.xyz

[U46] PHP：可空类型
来源：http://kfu.smart0.xyz

?string $name = null
来源：http://yik.hnxiangtu.top

[U47] PHP：联合类型
来源：http://bgs.tanke756.top

int|string $id
来源：http://qtv.vqdsnc.cn

[U48] PHP：纯枚举
来源：http://ubi.yueranfly.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tal.uphjek.com


<!-- 参考信息 -->