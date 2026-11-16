代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://luf.dashuyun.cn

[S21] C：字符类别判断
来源：http://xiw.svipenyu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dep.birdmap.top

[S22] C：字符串转数字
来源：http://zrz.kuanghao11.cn

atoi("42");  strtod("3.14", NULL);
来源：http://yto.fehbvm.com

[S23] C：随机数
来源：http://ssy.tarul.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://pkc.dianchejie.cn

[S24] C：获取本地时间
来源：http://niq.cdnleiting.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lmt.jinghuilouyu.cn

[S25] C：内存拷贝
来源：http://rzr.zhixingplan.top

memcpy(dst, src, n);
来源：http://zgb.yongpay.top

[S26] C：内存清零
来源：http://nir.iojbl.cn

memset(a, 0, sizeof a);
来源：http://lfo.haohaochexian.top

[S27] C：定义常量
来源：http://nld.ydzc1.top

const double PI = 3.14159;
来源：http://lyc.ctjpmb.com

[S28] C：静态变量
来源：http://kwf.svipenyu.cn

static int counter = 0;
来源：http://ogf.quarkkingdee.top

[S29] C：变参函数
来源：http://keb.gaohongyu789.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cdz.c1oappe.top

[S30] C：头文件保护
来源：http://wcz.ppjwa.cn

#ifndef X_H
来源：http://xmo.dianchejie.cn

#define X_H
来源：http://wer.fengsongda.top

#endif
来源：http://kmb.316326.xyz

[S31] C++：Hello World
来源：http://jqi.daria6918.cn

#include <iostream>
来源：http://cgd.aibaodan.cn

int main() { std::cout << "Hello\n"; }
来源：http://mvr.hammf.cn

[S32] C++：字符串
来源：http://hmf.bbcook.cn

std::string s = "hi";  s += "!";
来源：http://hir.xziqi.cn

[S33] C++：vector 增删
来源：http://wew.shanyushiyangkeji.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hyp.daxiang520.top

[S34] C++：遍历 vector
来源：http://xag.bbcook.cn

for (auto &x : v) { std::cout << x; }
来源：http://dbj.zhijiandao.cn

[S35] C++：map
来源：http://pcj.nanxinkj.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://msx.pengpengdd.cyou

[S36] C++：unordered_map
来源：http://bvd.cheryme.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pdu.sweek.top

[S37] C++：set
来源：http://ozl.cheryme.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wvl.gogol.net.cn

[S38] C++：排序
来源：http://snn.fehbvm.com

std::sort(v.begin(), v.end());
来源：http://lai.sysykeji.top

[S39] C++：自定义比较器排序
来源：http://ufd.cdnleiting.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://oie.nanxuanxn.top

[S40] C++：查找元素
来源：http://dcm.guannengcc.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://upw.zdbjq.cn

[S41] C++：类与构造函数
来源：http://knn.jlsjyb.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ygd.aibaodan.cn

[S42] C++：继承与虚函数
来源：http://nla.sysykeji.top

class B : public Base { public: void f() override {} };
来源：http://bdu.ivvv.top

[S43] C++：智能指针
来源：http://red.hnxiangtu.top

auto p = std::make_unique<int>(5);
来源：http://urz.bbcook.cn

[S44] C++：引用传参
来源：http://azz.jinqigufen.top

void inc(int &x) { ++x; }
来源：http://mrn.pengpengdd.cyou

[S45] C++：lambda
来源：http://umn.316326.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://yzu.zhongyouzk.top

[S46] C++：函数模板
来源：http://tsw.aizwys.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bmb.c1oappe.top

[S47] C++：结构化绑定遍历
来源：http://hjh.pengpengdd.cyou

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://arf.redwolf501.top

[S48] C++：逐行读文件
来源：http://pcc.ydjk.org.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ipg.gogol.net.cn

while (std::getline(in, line)) { }
来源：http://rvh.316326.xyz

[S49] C++：写文件
来源：http://ntk.andypj.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yju.ywan-chungtsiang.top

[S50] C++：格式化数字
来源：http://cgo.fanxiaobao.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://uin.zhijiandao.cn

[S51] C++：显式类型转换
来源：http://nbq.jyoumei.cn

static_cast<double>(a) / b
来源：http://elu.guannengcc.top

[S52] C++：const 与 noexcept
来源：http://yik.snrcjt.cn

int size() const noexcept { return n_; }
来源：http://syk.haohaochexian.top

[S53] C++：移动语义
来源：http://ges.uphjek.com

std::vector<int> w = std::move(v);
来源：http://acm.dianchejie.cn

[S54] C++：异常处理
来源：http://wii.nwbrower.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wdr.quarkkingdee.top

[S55] C++：结构化绑定
来源：http://nyp.tian-w.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://cgq.chenlongwang.top

[S56] C++：optional
来源：http://wiv.yuanzhike.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ixt.c1oappe.top

[S57] C++：编译期常量
来源：http://tyx.xziqi.cn

constexpr int N = 10;
来源：http://vih.gotoacloud.top

[S58] C++：命名空间
来源：http://cdd.fehbvm.com

namespace ns { int f() { return 1; } }
来源：http://wjd.fengsongda.top

[S59] C++：静态断言
来源：http://kvs.yangfankeji.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://crf.svipenyu.cn

[S60] C++：遍历并删除元素
来源：http://yue.xylfe.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wca.pengpengdd.cyou

================================================================================
来源：http://pbb.ehwqpu.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nme.pycfn.com

================================================================================
来源：http://sbl.dianchejie.cn

[T01] Kotlin：Hello World
来源：http://weh.cqqwz.cn

println("Hello")
来源：http://hkl.tianlin.xyz

[T02] Kotlin：变量
来源：http://vzw.daxiang520.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qxs.cqqwz.cn

[T03] Kotlin：字符串模板
来源：http://xvy.52xcode.cn

"值: $b"
来源：http://oyf.tarul.cn

[T04] Kotlin：空安全
来源：http://nis.jlsjyb.cn

val n: String? = null;  n?.length
来源：http://yup.hnxiangtu.top

[T05] Kotlin：when 表达式
来源：http://zho.fanxiaobao.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ekm.zhiwuduotai.top

[T06] Kotlin：集合映射
来源：http://kgd.shanyushiyangtech.top

listOf(1, 2, 3).map { it * 2 }
来源：http://pjh.andypj.xyz

[T07] Kotlin：集合过滤
来源：http://xtx.fanxiaobao.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://tzm.tanke756.top

[T08] Kotlin：数据类
来源：http://exz.c1oappe.top

data class User(val name: String, val age: Int)
来源：http://iee.cqqwz.cn

[T09] Kotlin：扩展函数
来源：http://qdl.ydjk.org.cn

fun String.exclaim() = this + "!"
来源：http://cll.yongpay.top

[T10] Kotlin：默认参数
来源：http://jzz.aibaodan.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://oaz.chenzaomai.com

[T11] Kotlin：协程
来源：http://bed.yuxming.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://cwl.zhongyouzk.top

[T12] Kotlin：解构声明
来源：http://tuj.yueranfly.top

val (a, b) = Pair(1, 2)
来源：http://pjd.jinyuanbaomall.cn

[T13] Kotlin：只读 Map
来源：http://rkc.ywan-chungtsiang.top

val m = mapOf("a" to 1)
来源：http://rqf.zycfv.cn

[T14] Kotlin：循环
来源：http://bnl.shanyushiyangtech.top

for (i in 1..10) println(i)
来源：http://yxi.hongshengwenyu.top

[T15] Kotlin：接口
来源：http://hxx.yfazqb.com

interface Shape { fun area(): Double }
来源：http://jcg.chenlongwang.top

[T16] Swift：Hello World
来源：http://lhm.zhiwuduotai.top

print("Hello")
来源：http://fhj.sweek.top

[T17] Swift：变量与常量
来源：http://guo.fehbvm.com

var a = 1;  let b = 2
来源：http://otv.yj202588.top

[T18] Swift：字符串插值
来源：http://uva.c1oappe.top

"值: \(b)"
来源：http://nte.zhijiandao.cn

[T19] Swift：可选绑定
来源：http://hdr.yueranfly.top

if let n = opt { print(n) }
来源：http://smm.jqgfzy.top

[T20] Swift：数组操作
来源：http://wwq.shanyushiyangtech.top

var a = [1, 2, 3];  a.append(4)
来源：http://fje.sxryk.cn

[T21] Swift：遍历
来源：http://nql.ehwqpu.com

for x in a { print(x) }
来源：http://cbt.jiagoushi.top

[T22] Swift：字典
来源：http://qpe.haohaochexian.top

var d = ["a": 1];  d["b"] = 2
来源：http://yiv.fehbvm.com

[T23] Swift：函数
来源：http://jof.tianlin.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://opy.feifeiyinyue.top

[T24] Swift：闭包
来源：http://lod.sweek.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://rrr.feifeiyinyue.top

[T25] Swift：结构体
来源：http://jkl.cdnleiting.top

struct P { var x: Int }
来源：http://lfc.chenjidiqi.icu

[T26] Swift：类与重写
来源：http://bml.jinqigufen.top

class A: Base { override func f() {} }
来源：http://dot.shanyushiyangtech.top

[T27] Swift：错误处理
来源：http://pxa.nwbrower.top

do { try f() } catch { print(error) }
来源：http://jlf.hongshengwenyu.top

[T28] Swift：枚举
来源：http://tlv.vehdjk.com

enum Color { case red, green }
来源：http://qmh.cashguo.top

[T29] Swift：guard 提前返回
来源：http://hsz.hnqzz.top

guard let x = opt else { return }
来源：http://xzt.316326.xyz

[T30] Swift：协议
来源：http://jtv.wangshuangyany.cn

protocol Shape { func area() -> Double }
来源：http://gmb.vehdjk.com

[T31] Lua：Hello World
来源：http://acu.epnwcf.com

print("Hello")
来源：http://nhm.kuanghao11.cn

[T32] Lua：局部变量
来源：http://kwg.xinyue.icu

local a = 1
来源：http://vih.ctjpmb.com

[T33] Lua：表（数组）
来源：http://whj.kuanghao11.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://opq.zdqjudy.top

[T34] Lua：遍历表
来源：http://laf.hysaishi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://evc.zdqjudy.top

[T35] Lua：字典表
来源：http://rzl.hnxiangtu.top

local d = { a = 1 };  d.b = 2
来源：http://iup.sysykeji.top

[T36] Lua：函数
来源：http://rgo.yuxming.cn

function add(a, b) return a + b end
来源：http://jat.quarkkingdee.top

[T37] Lua：字符串拼接
来源：http://vmj.aibaodan.cn

"a" .. "b"
来源：http://ssu.iojbl.cn

[T38] Lua：条件
来源：http://nsp.52xcode.cn

if x > 0 then print("正") end
来源：http://ikc.zhixingplan.top

[T39] Lua：模式匹配
来源：http://enq.jinyuanbaomall.cn

string.find(s, "%d+")
来源：http://mum.jlsjyb.cn

[T40] Lua：元表
来源：http://nad.ybcxt.top

setmetatable({}, { __index = base })
来源：http://cea.zycfv.cn

[T41] Perl：Hello World
来源：http://mbu.zhiwuduotai.top

print "Hello\n";
来源：http://kpd.hammf.cn

[T42] Perl：变量类型
来源：http://agh.xinyue.icu

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kbd.ivvv.top

[T43] Perl：字符串插值
来源：http://ysx.pycfn.com

"值: $a"
来源：http://mbs.zhiwuduotai.top

[T44] Perl：条件
来源：http://grc.zycfv.cn

if ($a > 0) { print "正"; }
来源：http://iqj.ywan-chungtsiang.top

[T45] Perl：数组遍历
来源：http://ust.wangshuangyany.cn

for my $x (@arr) { print $x; }
来源：http://yfv.gogol.net.cn

[T46] Perl：哈希操作
来源：http://vni.yueranfly.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wpk.yanxiufei.cn

[T47] Perl：正则捕获
来源：http://lky.bbcook.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://hlu.yangfankeji.com

[T48] Perl：正则替换
来源：http://frc.andypj.xyz

$s =~ s/old/new/g;
来源：http://bsa.xziqi.cn

[T49] Perl：函数
来源：http://qwq.jinqigfzy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ulu.gotoacloud.top

[T50] Perl：逐行读文件
来源：http://aud.snrcjt.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://aec.tarul.cn

while (my $line = <$fh>) { print $line; }
来源：http://dvg.zhongyouzk.top

[T51] Scala：Hello World
来源：http://ldv.feifeiyinyue.top

println("Hello")
来源：http://mdt.shanyushiyangkeji.top

[T52] Scala：变量
来源：http://crr.shzxlz.cn

val a = 1;  var b = 2
来源：http://ndf.tianlin.xyz

[T53] Scala：字符串插值
来源：http://obv.nanxuanxn.top

s"值: $b"
来源：http://vca.ydzc1.top

[T54] Scala：集合映射
来源：http://dri.tian-w.cn

List(1, 2, 3).map(_ * 2)
来源：http://nea.quarkkingdee.top

[T55] Scala：集合过滤
来源：http://cmr.yvedp.cn

List(1, 2, 3).filter(_ > 1)
来源：http://djl.0kj1m.cn

[T56] Scala：样例类
来源：http://jwt.jlsjyb.cn

case class User(name: String, age: Int)
来源：http://wrw.yfazqb.com

[T57] Scala：模式匹配
来源：http://eju.jianghu66.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://zsw.guannengcc.top

[T58] Scala：函数定义
来源：http://dtv.xziqi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://vtz.jianghu66.top

[T59] Scala：循环
来源：http://prr.xylfe.cn

for (i <- 1 to 10) println(i)
来源：http://aqr.smart0.xyz

[T60] Scala：折叠
来源：http://eel.nwbrower.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jel.xuetiantiany.cn

================================================================================
来源：http://wcy.yangfankeji.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jsw.xinyue.icu

================================================================================
来源：http://vni.dashuyun.cn

[U01] Py：创建虚拟环境
来源：http://czm.jianghu66.top

python -m venv .venv && source .venv/bin/activate
来源：http://osx.yanxiufei.cn

[U02] Py：导出 / 安装依赖
来源：http://fsv.daxiang520.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zny.zdqjudy.top

[U03] Py：加载 .env 配置
来源：http://cba.jinqigufen.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ckz.andypj.xyz

[U04] Py：变量调试打印
来源：http://znk.hysaishi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dog.yfazqb.com

[U05] Py：列表去重且保序
来源：http://ute.fengsongda.top

list(dict.fromkeys(arr))
来源：http://lrk.zhaomingkeji.xyz

[U06] Py：合并两个字典
来源：http://cev.fengsongda.top

{**a, **b}
来源：http://lii.jinqigfzy.top

[U07] Py：反转字典键值
来源：http://ozt.cucudq.cn

{v: k for k, v in d.items()}
来源：http://bpz.daria6918.cn

[U08] Py：展平二维列表
来源：http://oie.zhengqikj.top

[y for x in nested for y in x]
来源：http://tsq.dianchejie.cn

[U09] Py：字典取最大值的键
来源：http://odk.smart0.xyz

max(d, key=d.get)
来源：http://ytn.c1oappe.top

[U10] Py：按值排序字典
来源：http://jmt.cheryme.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cll.9152youxi.cn

[U11] Py：生成器表达式
来源：http://izi.yj20258888.top

(x * 2 for x in arr)
来源：http://dwd.dashuyun.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xdj.cashguo.top

Counter(arr).most_common(3)
来源：http://hah.birdmap.top

[U13] Py：固定长度队列
来源：http://etg.ivvv.top

deque(maxlen=10)
来源：http://xau.cdnleiting.top

[U14] Py：分组收集到列表
来源：http://uns.sysykeji.top

defaultdict(list)
来源：http://qpy.yj202588.top

[U15] Py：高精度计时
来源：http://ywg.nanxuanxn.top

t = time.perf_counter()
来源：http://rjx.daxiang520.top

[U16] Py：命令行参数解析
来源：http://zbj.yj20258888.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://szp.vehdjk.com

[U17] Py：初始化日志
来源：http://zoz.daria6918.cn

logging.basicConfig(level=logging.INFO)
来源：http://dmp.ywan-chungtsiang.top

[U18] Py：预编译正则
来源：http://taz.cdnleiting.top

pat = re.compile(r"\d+")
来源：http://tnb.gaohongyu789.top

[U19] Py：正则替换带回调
来源：http://hul.cashguo.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://apl.iojbl.cn

[U20] Py：缓存函数结果
来源：http://uba.xuetiantiany.cn

@functools.lru_cache(maxsize=None)
来源：http://siu.epnwcf.com

[U21] Py：自定义上下文管理器
来源：http://wgh.jinqigfzy.top

@contextlib.contextmanager
来源：http://uug.zycfv.cn

[U22] Py：矩阵转置
来源：http://bhm.yueranfly.top

list(zip(*m))
来源：http://mya.chenjidiqi.icu

[U23] Py：分块读取大文件
来源：http://enk.cdnleiting.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rvr.iojbl.cn

[U24] Py：路径操作
来源：http://ngm.sxryk.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mbt.52xcode.cn

[U25] Py：CSV 按字典读
来源：http://kit.hammf.cn

csv.DictReader(f)
来源：http://tzp.yj20258888.top

[U26] Py：并发下载
来源：http://uva.fehbvm.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pyg.zhixingplan.top

[U27] Py：异步 HTTP
来源：http://kbm.zhengqikj.top

aiohttp.ClientSession() 配合 async with
来源：http://atw.yj20258.top

[U28] Py：类型别名
来源：http://whf.zhijiandao.cn

UserId = int
来源：http://ccp.ywan-chungtsiang.top

[U29] Py：属性校验
来源：http://jyg.yueranfly.top

@property 与 @x.setter 配合
来源：http://lst.jinqigfzy.top

[U30] Py：数据类
来源：http://yzc.jinyuanbaomall.cn

@dataclass(slots=True)
来源：http://zfx.zhongyouzk.top

[U31] Py：单测
来源：http://ghk.zhixingplan.top

python -m pytest -q
来源：http://sun.cqqwz.cn

[U32] Py：代码格式化
来源：http://shi.cdnleiting.top

ruff format . && ruff check --fix .
来源：http://ogh.feifeiyinyue.top

[U33] Py：打包发布
来源：http://uuu.zhongyouzk.top

python -m build  （依赖 pyproject.toml）
来源：http://jew.fzhhl.top

[U34] Py：判断编码
来源：http://wgi.pengpengdd.cyou

chardet.detect(raw)
来源：http://twi.cheryme.top

[U35] Py：发送邮件
来源：http://ugg.zhixingplan.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bsj.havefunace.top

[U36] Py：定时任务
来源：http://cks.ybcxt.top

schedule.every(10).minutes.do(job)
来源：http://tan.aibaodan.cn

[U37] Py：读写 Excel
来源：http://jyo.fengsongda.top

pandas.read_excel / DataFrame.to_excel
来源：http://rnf.chenlongwang.top

[U38] Py：获取脚本所在目录
来源：http://iek.sjlbkw.cn

Path(__file__).resolve().parent
来源：http://efh.andypj.xyz

[U39] Py：判断是否在交互环境
来源：http://sli.xuetiantiany.cn

sys.stdout.isatty()
来源：http://ltk.jinqigfzy.top

[U40] Py：打印到标准错误
来源：http://pbf.shanyushiyangkeji.top

print("err", file=sys.stderr)
来源：http://bkw.316326.xyz

[U41] PHP：初始化 Composer 项目
来源：http://vgd.zhaomingkeji.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://byl.xinyue.icu

[U42] PHP：PSR-4 自动加载
来源：http://ykq.feifeiyinyue.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cqt.fzhhl.top

[U43] PHP：声明命名空间
来源：http://jhg.gaohongyu789.top

namespace App\Http;
来源：http://srt.zhixingplan.top

[U44] PHP：开启严格类型
来源：http://ktv.shzxlz.cn

declare(strict_types=1);
来源：http://szd.chenjidiqi.icu


<!-- 参考信息 -->