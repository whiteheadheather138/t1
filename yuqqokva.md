代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qpy.guannengcc.top

[S21] C：字符类别判断
来源：http://hyt.gogol.net.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://foj.cdnleiting.top

[S22] C：字符串转数字
来源：http://fjw.zhaomingkeji.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://qej.guowangkeji.top

[S23] C：随机数
来源：http://xfd.shuidangran.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ugd.zhoulong.xyz

[S24] C：获取本地时间
来源：http://ozr.jinghuilouyu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sxg.redwolf501.top

[S25] C：内存拷贝
来源：http://wpw.yfazqb.com

memcpy(dst, src, n);
来源：http://uci.havefunace.top

[S26] C：内存清零
来源：http://pkj.xziqi.cn

memset(a, 0, sizeof a);
来源：http://zap.ehwqpu.com

[S27] C：定义常量
来源：http://msl.fengsongda.top

const double PI = 3.14159;
来源：http://xqn.shanyushiyangtech.top

[S28] C：静态变量
来源：http://ter.wangdashe.top

static int counter = 0;
来源：http://ygn.zycfv.cn

[S29] C：变参函数
来源：http://qrh.zhongyouzk.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bup.jinyuanbaomall.cn

[S30] C：头文件保护
来源：http://ezc.chenlongwang.top

#ifndef X_H
来源：http://gof.jinyuanbaomall.cn

#define X_H
来源：http://ctp.meibo888.top

#endif
来源：http://pui.shzxlz.cn

[S31] C++：Hello World
来源：http://wkk.cdnleiting.top

#include <iostream>
来源：http://ctg.fanxiaobao.xyz

int main() { std::cout << "Hello\n"; }
来源：http://wkm.svipenyu.cn

[S32] C++：字符串
来源：http://zlz.mhx1999.top

std::string s = "hi";  s += "!";
来源：http://wsl.hammf.cn

[S33] C++：vector 增删
来源：http://clo.birdmap.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://toy.52xcode.cn

[S34] C++：遍历 vector
来源：http://qan.yonumen.top

for (auto &x : v) { std::cout << x; }
来源：http://ixa.tianlin.xyz

[S35] C++：map
来源：http://ndp.sxryk.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pwd.fzhhl.top

[S36] C++：unordered_map
来源：http://jgk.chenlongwang.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://czb.9152youxi.cn

[S37] C++：set
来源：http://zff.nwbrower.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jym.tianlin.xyz

[S38] C++：排序
来源：http://slq.ivvv.top

std::sort(v.begin(), v.end());
来源：http://yed.shanyushiyangkeji.top

[S39] C++：自定义比较器排序
来源：http://wkn.daria6918.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rgw.shangyingyoupin.top

[S40] C++：查找元素
来源：http://qpb.gotoacloud.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sws.sufxvd.cn

[S41] C++：类与构造函数
来源：http://krt.yueranfly.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xwb.bbcook.cn

[S42] C++：继承与虚函数
来源：http://rxp.svipenyu.cn

class B : public Base { public: void f() override {} };
来源：http://lxn.gaohongyu789.top

[S43] C++：智能指针
来源：http://bnh.316326.xyz

auto p = std::make_unique<int>(5);
来源：http://nnd.yuxming.cn

[S44] C++：引用传参
来源：http://llk.fktsv.cn

void inc(int &x) { ++x; }
来源：http://dsd.kuanghao11.cn

[S45] C++：lambda
来源：http://edi.haohaochexian.top

auto add = [](int a, int b) { return a + b; };
来源：http://vut.yj20258.top

[S46] C++：函数模板
来源：http://hwy.snrcjt.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://owj.shanyushiyangtech.top

[S47] C++：结构化绑定遍历
来源：http://vnz.mhx1999.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qku.daria6918.cn

[S48] C++：逐行读文件
来源：http://xvh.ppjwa.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wlh.daxiang520.top

while (std::getline(in, line)) { }
来源：http://xhc.shuidangran.top

[S49] C++：写文件
来源：http://bdp.sysykeji.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cvo.nwbrower.top

[S50] C++：格式化数字
来源：http://uly.zhiwuduotai.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ena.zycfv.cn

[S51] C++：显式类型转换
来源：http://eqy.xziqi.cn

static_cast<double>(a) / b
来源：http://ykw.shanyushiyangtech.top

[S52] C++：const 与 noexcept
来源：http://lgw.xinyue.icu

int size() const noexcept { return n_; }
来源：http://vsm.gaohongyu789.top

[S53] C++：移动语义
来源：http://pux.yvedp.cn

std::vector<int> w = std::move(v);
来源：http://nsl.yuxming.cn

[S54] C++：异常处理
来源：http://cir.tanke756.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://uby.daxiang520.top

[S55] C++：结构化绑定
来源：http://eum.shanyushiyangtech.top

auto [a, b] = std::make_pair(1, 2);
来源：http://xkw.pengpengdd.cyou

[S56] C++：optional
来源：http://afx.yongpay.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mue.hcnkem.com

[S57] C++：编译期常量
来源：http://wre.jinghuilouyu.cn

constexpr int N = 10;
来源：http://bbm.c1oappe.top

[S58] C++：命名空间
来源：http://mmo.shzxlz.cn

namespace ns { int f() { return 1; } }
来源：http://gwy.aizwys.cn

[S59] C++：静态断言
来源：http://bvs.ywan-chungtsiang.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://iio.sysykeji.top

[S60] C++：遍历并删除元素
来源：http://lof.aibaodan.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ojj.chenlongwang.top

================================================================================
来源：http://njx.smart0.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lon.yuxming.cn

================================================================================
来源：http://cpm.gogol.net.cn

[T01] Kotlin：Hello World
来源：http://hxj.xylfe.cn

println("Hello")
来源：http://oar.vqdsnc.cn

[T02] Kotlin：变量
来源：http://ieu.9152youxi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vto.zdbjq.cn

[T03] Kotlin：字符串模板
来源：http://tlf.bjfxy.top

"值: $b"
来源：http://rrs.yfazqb.com

[T04] Kotlin：空安全
来源：http://oxm.zhoulong.xyz

val n: String? = null;  n?.length
来源：http://ies.chenlongwang.top

[T05] Kotlin：when 表达式
来源：http://kns.kuanghao11.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ecp.shanyushiyangtech.top

[T06] Kotlin：集合映射
来源：http://cgb.uphjek.com

listOf(1, 2, 3).map { it * 2 }
来源：http://lzh.hongshengwenyu.top

[T07] Kotlin：集合过滤
来源：http://bgz.yangfankeji.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://abx.cashguo.top

[T08] Kotlin：数据类
来源：http://voz.jinyuanbaomall.cn

data class User(val name: String, val age: Int)
来源：http://dfh.quarkkingdee.top

[T09] Kotlin：扩展函数
来源：http://gok.52xcode.cn

fun String.exclaim() = this + "!"
来源：http://klf.tianlin.xyz

[T10] Kotlin：默认参数
来源：http://jnt.zdbjq.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jcu.cheryme.top

[T11] Kotlin：协程
来源：http://eef.xziqi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://sht.jyoumei.cn

[T12] Kotlin：解构声明
来源：http://laa.hysaishi.cn

val (a, b) = Pair(1, 2)
来源：http://jwl.jinyuanbaomall.cn

[T13] Kotlin：只读 Map
来源：http://urh.zhijiandao.cn

val m = mapOf("a" to 1)
来源：http://jos.gogol.net.cn

[T14] Kotlin：循环
来源：http://bef.fengsongda.top

for (i in 1..10) println(i)
来源：http://fph.cashguo.top

[T15] Kotlin：接口
来源：http://wzl.hnqzz.top

interface Shape { fun area(): Double }
来源：http://zyq.ctjpmb.com

[T16] Swift：Hello World
来源：http://ejp.bjfxy.top

print("Hello")
来源：http://djs.nwbrower.top

[T17] Swift：变量与常量
来源：http://oyq.sufxvd.cn

var a = 1;  let b = 2
来源：http://rxf.cucudq.cn

[T18] Swift：字符串插值
来源：http://hpg.zhixingplan.top

"值: \(b)"
来源：http://zhl.jqgufenzy.top

[T19] Swift：可选绑定
来源：http://cpj.jqgfzy.top

if let n = opt { print(n) }
来源：http://lni.hnxiangtu.top

[T20] Swift：数组操作
来源：http://vsk.bbcook.cn

var a = [1, 2, 3];  a.append(4)
来源：http://imy.yangfankeji.com

[T21] Swift：遍历
来源：http://jft.jqgfzy.top

for x in a { print(x) }
来源：http://hfd.tian-w.cn

[T22] Swift：字典
来源：http://sfj.birdmap.top

var d = ["a": 1];  d["b"] = 2
来源：http://zko.andypj.xyz

[T23] Swift：函数
来源：http://aqz.nwbrower.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fdk.fehbvm.com

[T24] Swift：闭包
来源：http://feo.hnxiangtu.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://tbn.9152youxi.cn

[T25] Swift：结构体
来源：http://jlv.gotoacloud.top

struct P { var x: Int }
来源：http://uac.xingfuxueyuan.xyz

[T26] Swift：类与重写
来源：http://ytn.havefunace.top

class A: Base { override func f() {} }
来源：http://nyl.xinyue.icu

[T27] Swift：错误处理
来源：http://qfw.nanxinkj.top

do { try f() } catch { print(error) }
来源：http://aje.sweek.top

[T28] Swift：枚举
来源：http://hwb.sufxvd.cn

enum Color { case red, green }
来源：http://zri.hfpthk.cn

[T29] Swift：guard 提前返回
来源：http://tdo.zhiwuduotai.top

guard let x = opt else { return }
来源：http://mra.ctjpmb.com

[T30] Swift：协议
来源：http://ooj.sufxvd.cn

protocol Shape { func area() -> Double }
来源：http://jbe.snrcjt.cn

[T31] Lua：Hello World
来源：http://elt.ydzc1.top

print("Hello")
来源：http://fkh.jlsjyb.cn

[T32] Lua：局部变量
来源：http://ipq.c1oappe.top

local a = 1
来源：http://bqs.316326.xyz

[T33] Lua：表（数组）
来源：http://evc.guannengcc.top

local t = {1, 2, 3};  t[4] = 4
来源：http://eiu.yuxming.cn

[T34] Lua：遍历表
来源：http://xyn.aibaodan.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://hvd.cheryme.top

[T35] Lua：字典表
来源：http://dxz.ppjwa.cn

local d = { a = 1 };  d.b = 2
来源：http://sdx.epnwcf.com

[T36] Lua：函数
来源：http://gzj.yongpay.top

function add(a, b) return a + b end
来源：http://zym.bjfxy.top

[T37] Lua：字符串拼接
来源：http://snf.hnxiangtu.top

"a" .. "b"
来源：http://qwu.meibo888.top

[T38] Lua：条件
来源：http://vyt.uphjek.com

if x > 0 then print("正") end
来源：http://ndr.hfpthk.cn

[T39] Lua：模式匹配
来源：http://ybx.vqdsnc.cn

string.find(s, "%d+")
来源：http://cgu.fanxiaobao.xyz

[T40] Lua：元表
来源：http://iaf.guannengcc.top

setmetatable({}, { __index = base })
来源：http://hct.epnwcf.com

[T41] Perl：Hello World
来源：http://grh.daria6918.cn

print "Hello\n";
来源：http://oke.dashuyun.cn

[T42] Perl：变量类型
来源：http://qrm.gzhubu.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mks.zhixingplan.top

[T43] Perl：字符串插值
来源：http://bnb.chenlongwang.top

"值: $a"
来源：http://zlx.fanxiaobao.xyz

[T44] Perl：条件
来源：http://rww.zhengqikj.top

if ($a > 0) { print "正"; }
来源：http://msr.feifeiyinyue.top

[T45] Perl：数组遍历
来源：http://znv.yj202588.top

for my $x (@arr) { print $x; }
来源：http://nuk.xylfe.cn

[T46] Perl：哈希操作
来源：http://ffp.yj202588.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://djx.yongpay.top

[T47] Perl：正则捕获
来源：http://nse.yueranfly.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://lpk.c1oappe.top

[T48] Perl：正则替换
来源：http://bit.zhiwuduotai.top

$s =~ s/old/new/g;
来源：http://pkd.nwbrower.top

[T49] Perl：函数
来源：http://zvi.zycfv.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://taw.xinyue.icu

[T50] Perl：逐行读文件
来源：http://zan.jinyuanbaomall.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://mem.kuanghao11.cn

while (my $line = <$fh>) { print $line; }
来源：http://nnb.hywenlv.cn

[T51] Scala：Hello World
来源：http://hia.zhongyouzk.top

println("Hello")
来源：http://ijj.chenlongwang.top

[T52] Scala：变量
来源：http://cns.tanke756.top

val a = 1;  var b = 2
来源：http://quj.hongshengwenyu.top

[T53] Scala：字符串插值
来源：http://srt.zdqjudy.top

s"值: $b"
来源：http://rwe.svipenyu.cn

[T54] Scala：集合映射
来源：http://fjx.pycfn.com

List(1, 2, 3).map(_ * 2)
来源：http://ssu.zdbjq.cn

[T55] Scala：集合过滤
来源：http://die.snrcjt.cn

List(1, 2, 3).filter(_ > 1)
来源：http://lue.cdnleiting.top

[T56] Scala：样例类
来源：http://qgr.hfpthk.cn

case class User(name: String, age: Int)
来源：http://mel.yangfankeji.com

[T57] Scala：模式匹配
来源：http://zoz.fehbvm.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://wfp.yvedp.cn

[T58] Scala：函数定义
来源：http://nva.jinqigufen.top

def add(a: Int, b: Int): Int = a + b
来源：http://juk.ydzc1.top

[T59] Scala：循环
来源：http://tst.sysykeji.top

for (i <- 1 to 10) println(i)
来源：http://bgm.gaohongyu789.top

[T60] Scala：折叠
来源：http://zma.9152youxi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ktr.smart0.xyz

================================================================================
来源：http://slw.tian-w.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://sju.jianghu66.top

================================================================================
来源：http://klz.xylfe.cn

[U01] Py：创建虚拟环境
来源：http://dhg.ppjwa.cn

python -m venv .venv && source .venv/bin/activate
来源：http://xfe.svipenyu.cn

[U02] Py：导出 / 安装依赖
来源：http://zrf.fehbvm.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xwk.chenlongwang.top

[U03] Py：加载 .env 配置
来源：http://pxz.bbcook.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://fxd.yj20258.top

[U04] Py：变量调试打印
来源：http://lrk.zdbjq.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mgx.ybcxt.top

[U05] Py：列表去重且保序
来源：http://lhb.havefunace.top

list(dict.fromkeys(arr))
来源：http://xag.wangdashe.top

[U06] Py：合并两个字典
来源：http://xlg.zhijiandao.cn

{**a, **b}
来源：http://wgn.chenzaomai.com

[U07] Py：反转字典键值
来源：http://ctj.zdqjudy.top

{v: k for k, v in d.items()}
来源：http://clh.tanke756.top

[U08] Py：展平二维列表
来源：http://pjr.vehdjk.com

[y for x in nested for y in x]
来源：http://vzl.52xcode.cn

[U09] Py：字典取最大值的键
来源：http://agy.zycfv.cn

max(d, key=d.get)
来源：http://cdz.yangfankeji.com

[U10] Py：按值排序字典
来源：http://qaz.aizwys.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qml.ydjk.org.cn

[U11] Py：生成器表达式
来源：http://olo.gzhubu.top

(x * 2 for x in arr)
来源：http://gfh.jiagoushi.top

[U12] Py：取出现最多的 3 个元素
来源：http://lik.yueranfly.top

Counter(arr).most_common(3)
来源：http://crb.wangdashe.top

[U13] Py：固定长度队列
来源：http://lhu.yanxiufei.cn

deque(maxlen=10)
来源：http://wcn.yvedp.cn

[U14] Py：分组收集到列表
来源：http://lmg.fengsongda.top

defaultdict(list)
来源：http://sou.chenjidiqi.icu

[U15] Py：高精度计时
来源：http://iho.havefunace.top

t = time.perf_counter()
来源：http://iip.ctjpmb.com

[U16] Py：命令行参数解析
来源：http://gzg.smart0.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://han.tianlin.xyz

[U17] Py：初始化日志
来源：http://xmh.pengpengdd.cyou

logging.basicConfig(level=logging.INFO)
来源：http://vdk.hywenlv.cn

[U18] Py：预编译正则
来源：http://ett.shuidangran.top

pat = re.compile(r"\d+")
来源：http://uty.cdnleiting.top

[U19] Py：正则替换带回调
来源：http://vyr.jinghuilouyu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://seh.fktsv.cn

[U20] Py：缓存函数结果
来源：http://gvd.hnxiangtu.top

@functools.lru_cache(maxsize=None)
来源：http://upq.zycfv.cn

[U21] Py：自定义上下文管理器
来源：http://dfc.jyoumei.cn

@contextlib.contextmanager
来源：http://aqo.shanyushiyangkeji.top

[U22] Py：矩阵转置
来源：http://hvb.shuidangran.top

list(zip(*m))
来源：http://gro.shanyushiyangtech.top

[U23] Py：分块读取大文件
来源：http://wbx.jinghuilouyu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://kac.vehdjk.com

[U24] Py：路径操作
来源：http://dfx.zhiwuduotai.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gay.gaohongyu789.top

[U25] Py：CSV 按字典读
来源：http://jxj.dashuyun.cn

csv.DictReader(f)
来源：http://dme.sxryk.cn

[U26] Py：并发下载
来源：http://mom.sxryk.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://msd.yangfankeji.com

[U27] Py：异步 HTTP
来源：http://erc.vehdjk.com

aiohttp.ClientSession() 配合 async with
来源：http://bys.ybcxt.top

[U28] Py：类型别名
来源：http://hwx.hysaishi.cn

UserId = int
来源：http://gye.nanxuanxn.top

[U29] Py：属性校验
来源：http://paa.guannengcc.top

@property 与 @x.setter 配合
来源：http://jwt.52xcode.cn

[U30] Py：数据类
来源：http://qoe.gogol.net.cn

@dataclass(slots=True)
来源：http://fpd.cdnleiting.top

[U31] Py：单测
来源：http://wwx.zycfv.cn

python -m pytest -q
来源：http://kla.jinqigfzy.top

[U32] Py：代码格式化
来源：http://hsh.ctjpmb.com

ruff format . && ruff check --fix .
来源：http://aep.aizwys.cn

[U33] Py：打包发布
来源：http://bbf.cucudq.cn

python -m build  （依赖 pyproject.toml）
来源：http://mha.cqqwz.cn

[U34] Py：判断编码
来源：http://zyy.zhixingplan.top

chardet.detect(raw)
来源：http://qwj.epnwcf.com

[U35] Py：发送邮件
来源：http://csm.iojbl.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hlj.shzxlz.cn

[U36] Py：定时任务
来源：http://fjj.hywenlv.cn

schedule.every(10).minutes.do(job)
来源：http://zuj.tarul.cn

[U37] Py：读写 Excel
来源：http://qtb.shuidangran.top

pandas.read_excel / DataFrame.to_excel
来源：http://wyy.haohaochexian.top

[U38] Py：获取脚本所在目录
来源：http://oki.andypj.xyz

Path(__file__).resolve().parent
来源：http://xuv.vehdjk.com

[U39] Py：判断是否在交互环境
来源：http://xmw.zhaomingkeji.xyz

sys.stdout.isatty()
来源：http://yge.jiagoushi.top

[U40] Py：打印到标准错误
来源：http://mis.shanyushiyangtech.top

print("err", file=sys.stderr)
来源：http://yox.yanxiufei.cn

[U41] PHP：初始化 Composer 项目
来源：http://yux.yuxming.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://jjv.cqqwz.cn

[U42] PHP：PSR-4 自动加载
来源：http://uid.jqgfzy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mrz.iojbl.cn

[U43] PHP：声明命名空间
来源：http://zgv.sjlbkw.cn

namespace App\Http;
来源：http://luv.yj20258.top

[U44] PHP：开启严格类型
来源：http://ahl.cucudq.cn

declare(strict_types=1);
来源：http://kyo.yangfankeji.com


<!-- 参考信息 -->