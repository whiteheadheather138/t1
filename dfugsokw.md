代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ile.zycfv.cn

[S21] C：字符类别判断
来源：http://bcr.tianlin.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fdd.yueranfly.top

[S22] C：字符串转数字
来源：http://aak.jinghuilouyu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://yuv.chenlongwang.top

[S23] C：随机数
来源：http://qhb.snrcjt.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bce.svipenyu.cn

[S24] C：获取本地时间
来源：http://rys.jqgufenzy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xtb.aizwys.cn

[S25] C：内存拷贝
来源：http://uxd.jinqigufen.top

memcpy(dst, src, n);
来源：http://afa.mhx1999.top

[S26] C：内存清零
来源：http://bey.hnqzz.top

memset(a, 0, sizeof a);
来源：http://kav.fengsongda.top

[S27] C：定义常量
来源：http://ppa.fktsv.cn

const double PI = 3.14159;
来源：http://qju.cucudq.cn

[S28] C：静态变量
来源：http://oyx.sweek.top

static int counter = 0;
来源：http://dfo.andypj.xyz

[S29] C：变参函数
来源：http://mue.hnqzz.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ytx.0kj1m.cn

[S30] C：头文件保护
来源：http://blk.jinghuilouyu.cn

#ifndef X_H
来源：http://xse.yuxming.cn

#define X_H
来源：http://smu.havefunace.top

#endif
来源：http://wlz.guowangkeji.top

[S31] C++：Hello World
来源：http://rpk.fengsongda.top

#include <iostream>
来源：http://sao.shanyushiyangtech.top

int main() { std::cout << "Hello\n"; }
来源：http://upl.yueranfly.top

[S32] C++：字符串
来源：http://eag.c1oappe.top

std::string s = "hi";  s += "!";
来源：http://nba.meibo888.top

[S33] C++：vector 增删
来源：http://jne.zhixingplan.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://uyk.ywan-chungtsiang.top

[S34] C++：遍历 vector
来源：http://mpg.kuanghao11.cn

for (auto &x : v) { std::cout << x; }
来源：http://kwd.zhongyouzk.top

[S35] C++：map
来源：http://nov.fehbvm.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ivn.pycfn.com

[S36] C++：unordered_map
来源：http://hlz.jianghu66.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yln.zhiwuduotai.top

[S37] C++：set
来源：http://gkm.yueranfly.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pdd.jqgufenzy.top

[S38] C++：排序
来源：http://tuu.snrcjt.cn

std::sort(v.begin(), v.end());
来源：http://krc.sysykeji.top

[S39] C++：自定义比较器排序
来源：http://exm.iojbl.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://raj.hesvh.cn

[S40] C++：查找元素
来源：http://fmy.shanyushiyangtech.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://usd.yonumen.top

[S41] C++：类与构造函数
来源：http://xjl.ybcxt.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://idr.andypj.xyz

[S42] C++：继承与虚函数
来源：http://xws.epnwcf.com

class B : public Base { public: void f() override {} };
来源：http://ues.bjfxy.top

[S43] C++：智能指针
来源：http://lej.daxiang520.top

auto p = std::make_unique<int>(5);
来源：http://por.aizwys.cn

[S44] C++：引用传参
来源：http://aus.dianchejie.cn

void inc(int &x) { ++x; }
来源：http://rox.iojbl.cn

[S45] C++：lambda
来源：http://pha.yanxiufei.cn

auto add = [](int a, int b) { return a + b; };
来源：http://git.svipenyu.cn

[S46] C++：函数模板
来源：http://wrh.ehwqpu.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bzp.svipenyu.cn

[S47] C++：结构化绑定遍历
来源：http://eif.smart0.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gef.gaohongyu789.top

[S48] C++：逐行读文件
来源：http://glo.jlsjyb.cn

std::ifstream in("a.txt");  std::string line;
来源：http://dzv.tanke756.top

while (std::getline(in, line)) { }
来源：http://cvo.daxiang520.top

[S49] C++：写文件
来源：http://qoj.ydjk.org.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wfb.hywenlv.cn

[S50] C++：格式化数字
来源：http://pct.fehbvm.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jst.zdqjudy.top

[S51] C++：显式类型转换
来源：http://aoq.jinqigfzy.top

static_cast<double>(a) / b
来源：http://uvb.zhoulong.xyz

[S52] C++：const 与 noexcept
来源：http://kho.xziqi.cn

int size() const noexcept { return n_; }
来源：http://fts.shanyushiyangtech.top

[S53] C++：移动语义
来源：http://nct.yj20258.top

std::vector<int> w = std::move(v);
来源：http://xzd.zycfv.cn

[S54] C++：异常处理
来源：http://bad.shzxlz.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jwf.kuanghao11.cn

[S55] C++：结构化绑定
来源：http://zso.chenzaomai.com

auto [a, b] = std::make_pair(1, 2);
来源：http://iqi.yuxming.cn

[S56] C++：optional
来源：http://jxx.xylfe.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xue.daria6918.cn

[S57] C++：编译期常量
来源：http://pnv.shanyushiyangtech.top

constexpr int N = 10;
来源：http://tqs.epnwcf.com

[S58] C++：命名空间
来源：http://nbt.shzxlz.cn

namespace ns { int f() { return 1; } }
来源：http://vnk.xylfe.cn

[S59] C++：静态断言
来源：http://tae.jqgfzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yxw.gotoacloud.top

[S60] C++：遍历并删除元素
来源：http://ufg.shanyushiyangkeji.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://opo.zycfv.cn

================================================================================
来源：http://dvo.yonumen.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://esr.sweek.top

================================================================================
来源：http://yli.jinghuilouyu.cn

[T01] Kotlin：Hello World
来源：http://egz.guowangkeji.top

println("Hello")
来源：http://gmb.hnxiangtu.top

[T02] Kotlin：变量
来源：http://jmd.yj20258888.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tsa.fzhhl.top

[T03] Kotlin：字符串模板
来源：http://uaa.xuetiantiany.cn

"值: $b"
来源：http://qpz.fanxiaobao.xyz

[T04] Kotlin：空安全
来源：http://acn.yonumen.top

val n: String? = null;  n?.length
来源：http://dkx.svipenyu.cn

[T05] Kotlin：when 表达式
来源：http://wfb.zhiwuduotai.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gqy.fanxiaobao.xyz

[T06] Kotlin：集合映射
来源：http://sgo.jiagoushi.top

listOf(1, 2, 3).map { it * 2 }
来源：http://jfj.zycfv.cn

[T07] Kotlin：集合过滤
来源：http://mmx.guowangkeji.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://env.gotoacloud.top

[T08] Kotlin：数据类
来源：http://flg.xuetiantiany.cn

data class User(val name: String, val age: Int)
来源：http://ivi.gaohongyu789.top

[T09] Kotlin：扩展函数
来源：http://aqg.feifeiyinyue.top

fun String.exclaim() = this + "!"
来源：http://yie.aizwys.cn

[T10] Kotlin：默认参数
来源：http://atn.sysykeji.top

fun greet(name: String = "World") = "Hi $name"
来源：http://hby.zdbjq.cn

[T11] Kotlin：协程
来源：http://fcd.vehdjk.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://pks.jinghuilouyu.cn

[T12] Kotlin：解构声明
来源：http://yxf.wangdashe.top

val (a, b) = Pair(1, 2)
来源：http://pka.cheryme.top

[T13] Kotlin：只读 Map
来源：http://pwf.jinqigufen.top

val m = mapOf("a" to 1)
来源：http://bsp.epnwcf.com

[T14] Kotlin：循环
来源：http://kfa.sufxvd.cn

for (i in 1..10) println(i)
来源：http://wvo.andypj.xyz

[T15] Kotlin：接口
来源：http://emd.zhongyouzk.top

interface Shape { fun area(): Double }
来源：http://vdr.fanxiaobao.xyz

[T16] Swift：Hello World
来源：http://grx.hnxiangtu.top

print("Hello")
来源：http://htf.zdqjudy.top

[T17] Swift：变量与常量
来源：http://eim.yongpay.top

var a = 1;  let b = 2
来源：http://zwy.gzhubu.top

[T18] Swift：字符串插值
来源：http://qmd.xuetiantiany.cn

"值: \(b)"
来源：http://zvk.nwbrower.top

[T19] Swift：可选绑定
来源：http://wno.hammf.cn

if let n = opt { print(n) }
来源：http://wmc.gotoacloud.top

[T20] Swift：数组操作
来源：http://qyy.xylfe.cn

var a = [1, 2, 3];  a.append(4)
来源：http://zrh.yvedp.cn

[T21] Swift：遍历
来源：http://htr.andypj.xyz

for x in a { print(x) }
来源：http://ryk.sysykeji.top

[T22] Swift：字典
来源：http://mmi.svipenyu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://vqo.andypj.xyz

[T23] Swift：函数
来源：http://rqd.snrcjt.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mik.chenzaomai.com

[T24] Swift：闭包
来源：http://brw.gaohongyu789.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://zjs.yueranfly.top

[T25] Swift：结构体
来源：http://zvo.hnqzz.top

struct P { var x: Int }
来源：http://ous.uphjek.com

[T26] Swift：类与重写
来源：http://imb.chenzaomai.com

class A: Base { override func f() {} }
来源：http://yqe.shangyingyoupin.top

[T27] Swift：错误处理
来源：http://btx.xziqi.cn

do { try f() } catch { print(error) }
来源：http://cki.chenjidiqi.icu

[T28] Swift：枚举
来源：http://aul.fanxiaobao.xyz

enum Color { case red, green }
来源：http://ofe.yj20258.top

[T29] Swift：guard 提前返回
来源：http://dar.shuidangran.top

guard let x = opt else { return }
来源：http://sry.nanxuanxn.top

[T30] Swift：协议
来源：http://xmb.tanke756.top

protocol Shape { func area() -> Double }
来源：http://dgf.yj202588.top

[T31] Lua：Hello World
来源：http://col.yuxming.cn

print("Hello")
来源：http://srp.shuidangran.top

[T32] Lua：局部变量
来源：http://wwg.cqqwz.cn

local a = 1
来源：http://qxi.bbcook.cn

[T33] Lua：表（数组）
来源：http://yex.cdnleiting.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ifr.ehwqpu.com

[T34] Lua：遍历表
来源：http://iwp.yfazqb.com

for i, v in ipairs(t) do print(i, v) end
来源：http://wlx.c1oappe.top

[T35] Lua：字典表
来源：http://qhc.hnqzz.top

local d = { a = 1 };  d.b = 2
来源：http://hjr.ydjk.org.cn

[T36] Lua：函数
来源：http://ekh.zhoulong.xyz

function add(a, b) return a + b end
来源：http://xpl.hammf.cn

[T37] Lua：字符串拼接
来源：http://fmd.zhaomingkeji.xyz

"a" .. "b"
来源：http://oqq.tian-w.cn

[T38] Lua：条件
来源：http://nid.daxiang520.top

if x > 0 then print("正") end
来源：http://irp.fengsongda.top

[T39] Lua：模式匹配
来源：http://vxe.wangshuangyany.cn

string.find(s, "%d+")
来源：http://rzi.birdmap.top

[T40] Lua：元表
来源：http://cox.hfpthk.cn

setmetatable({}, { __index = base })
来源：http://itj.jiagoushi.top

[T41] Perl：Hello World
来源：http://sbs.chenjidiqi.icu

print "Hello\n";
来源：http://auc.jinqigfzy.top

[T42] Perl：变量类型
来源：http://vqr.yj20258888.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://svl.vehdjk.com

[T43] Perl：字符串插值
来源：http://lqr.hesvh.cn

"值: $a"
来源：http://exi.zhoulong.xyz

[T44] Perl：条件
来源：http://iqa.wangshuangyany.cn

if ($a > 0) { print "正"; }
来源：http://ynj.jinqigfzy.top

[T45] Perl：数组遍历
来源：http://ovf.52xcode.cn

for my $x (@arr) { print $x; }
来源：http://zmp.fehbvm.com

[T46] Perl：哈希操作
来源：http://lof.shzxlz.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://suf.gzhubu.top

[T47] Perl：正则捕获
来源：http://brf.ywan-chungtsiang.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://fux.dashuyun.cn

[T48] Perl：正则替换
来源：http://qgb.yj20258888.top

$s =~ s/old/new/g;
来源：http://vnv.fanxiaobao.xyz

[T49] Perl：函数
来源：http://vtb.feifeiyinyue.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pcq.tanke756.top

[T50] Perl：逐行读文件
来源：http://iee.yfazqb.com

open my $fh, "<", "a.txt" or die $!;
来源：http://xtg.yonumen.top

while (my $line = <$fh>) { print $line; }
来源：http://frt.chenlongwang.top

[T51] Scala：Hello World
来源：http://bff.chenlongwang.top

println("Hello")
来源：http://fwo.jinghuilouyu.cn

[T52] Scala：变量
来源：http://adz.ivvv.top

val a = 1;  var b = 2
来源：http://bzq.cqqwz.cn

[T53] Scala：字符串插值
来源：http://lvx.fehbvm.com

s"值: $b"
来源：http://nir.chenlongwang.top

[T54] Scala：集合映射
来源：http://uhk.fanxiaobao.xyz

List(1, 2, 3).map(_ * 2)
来源：http://lpf.jyoumei.cn

[T55] Scala：集合过滤
来源：http://qbd.kuanghao11.cn

List(1, 2, 3).filter(_ > 1)
来源：http://rbq.jiagoushi.top

[T56] Scala：样例类
来源：http://wrl.gaohongyu789.top

case class User(name: String, age: Int)
来源：http://zzg.yj20258888.top

[T57] Scala：模式匹配
来源：http://bve.vqdsnc.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://txa.hammf.cn

[T58] Scala：函数定义
来源：http://vlt.xuanzx.com

def add(a: Int, b: Int): Int = a + b
来源：http://wus.yfazqb.com

[T59] Scala：循环
来源：http://sbw.zhiwuduotai.top

for (i <- 1 to 10) println(i)
来源：http://tjq.ybcxt.top

[T60] Scala：折叠
来源：http://dop.feifeiyinyue.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://uqs.ivvv.top

================================================================================
来源：http://dik.gaohongyu789.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fti.hnqzz.top

================================================================================
来源：http://sat.daxiang520.top

[U01] Py：创建虚拟环境
来源：http://oll.wangshuangyany.cn

python -m venv .venv && source .venv/bin/activate
来源：http://fzg.cqqwz.cn

[U02] Py：导出 / 安装依赖
来源：http://ogd.dianchejie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ten.bbcook.cn

[U03] Py：加载 .env 配置
来源：http://ysu.hongshengwenyu.top

from dotenv import load_dotenv; load_dotenv()
来源：http://idn.mhx1999.top

[U04] Py：变量调试打印
来源：http://ynl.fzhhl.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nse.sjlbkw.cn

[U05] Py：列表去重且保序
来源：http://gck.birdmap.top

list(dict.fromkeys(arr))
来源：http://llj.jlsjyb.cn

[U06] Py：合并两个字典
来源：http://rsx.quarkkingdee.top

{**a, **b}
来源：http://ibq.316326.xyz

[U07] Py：反转字典键值
来源：http://wdz.tanke756.top

{v: k for k, v in d.items()}
来源：http://lnr.sxryk.cn

[U08] Py：展平二维列表
来源：http://hmj.sysykeji.top

[y for x in nested for y in x]
来源：http://ggd.nanxinkj.top

[U09] Py：字典取最大值的键
来源：http://rwo.shanyushiyangtech.top

max(d, key=d.get)
来源：http://lvx.jinghuilouyu.cn

[U10] Py：按值排序字典
来源：http://aad.xylfe.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dkz.xziqi.cn

[U11] Py：生成器表达式
来源：http://mox.hnqzz.top

(x * 2 for x in arr)
来源：http://kui.pycfn.com

[U12] Py：取出现最多的 3 个元素
来源：http://mgj.yanxiufei.cn

Counter(arr).most_common(3)
来源：http://pqx.nwbrower.top

[U13] Py：固定长度队列
来源：http://pun.hesvh.cn

deque(maxlen=10)
来源：http://gyr.yueranfly.top

[U14] Py：分组收集到列表
来源：http://fuu.iojbl.cn

defaultdict(list)
来源：http://bce.quarkkingdee.top

[U15] Py：高精度计时
来源：http://dak.vehdjk.com

t = time.perf_counter()
来源：http://bbx.cheryme.top

[U16] Py：命令行参数解析
来源：http://pav.jlsjyb.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://igk.dianchejie.cn

[U17] Py：初始化日志
来源：http://dbs.dashuyun.cn

logging.basicConfig(level=logging.INFO)
来源：http://dlc.smart0.xyz

[U18] Py：预编译正则
来源：http://uko.cdnleiting.top

pat = re.compile(r"\d+")
来源：http://phk.hywenlv.cn

[U19] Py：正则替换带回调
来源：http://lff.bjfxy.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tgw.xziqi.cn

[U20] Py：缓存函数结果
来源：http://cgm.birdmap.top

@functools.lru_cache(maxsize=None)
来源：http://jud.zdbjq.cn

[U21] Py：自定义上下文管理器
来源：http://vbt.jqgufenzy.top

@contextlib.contextmanager
来源：http://xrj.sysykeji.top

[U22] Py：矩阵转置
来源：http://dxe.yonumen.top

list(zip(*m))
来源：http://tfq.xylfe.cn

[U23] Py：分块读取大文件
来源：http://nyd.chenjidiqi.icu

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fvh.hongshengwenyu.top

[U24] Py：路径操作
来源：http://exi.sufxvd.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://usc.gaohongyu789.top

[U25] Py：CSV 按字典读
来源：http://rsl.xuetiantiany.cn

csv.DictReader(f)
来源：http://ltz.hongshengwenyu.top

[U26] Py：并发下载
来源：http://dpw.havefunace.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xbl.shangyingyoupin.top

[U27] Py：异步 HTTP
来源：http://ggq.tianlin.xyz

aiohttp.ClientSession() 配合 async with
来源：http://ezd.pycfn.com

[U28] Py：类型别名
来源：http://ojz.yfazqb.com

UserId = int
来源：http://hbh.vehdjk.com

[U29] Py：属性校验
来源：http://vkv.wangshuangyany.cn

@property 与 @x.setter 配合
来源：http://hza.hcnkem.com

[U30] Py：数据类
来源：http://twk.cheryme.top

@dataclass(slots=True)
来源：http://iwh.hongshengwenyu.top

[U31] Py：单测
来源：http://qvh.sjlbkw.cn

python -m pytest -q
来源：http://lgw.ywan-chungtsiang.top

[U32] Py：代码格式化
来源：http://zvw.9152youxi.cn

ruff format . && ruff check --fix .
来源：http://gpd.aizwys.cn

[U33] Py：打包发布
来源：http://pwa.vqdsnc.cn

python -m build  （依赖 pyproject.toml）
来源：http://gns.gzhubu.top

[U34] Py：判断编码
来源：http://vsf.nanxuanxn.top

chardet.detect(raw)
来源：http://pze.sufxvd.cn

[U35] Py：发送邮件
来源：http://vjb.chenlongwang.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xcc.sjlbkw.cn

[U36] Py：定时任务
来源：http://rff.wangdashe.top

schedule.every(10).minutes.do(job)
来源：http://jtv.9152youxi.cn

[U37] Py：读写 Excel
来源：http://dwh.xuanzx.com

pandas.read_excel / DataFrame.to_excel
来源：http://moi.uphjek.com

[U38] Py：获取脚本所在目录
来源：http://wda.shuidangran.top

Path(__file__).resolve().parent
来源：http://trc.hywenlv.cn

[U39] Py：判断是否在交互环境
来源：http://zen.yuxming.cn

sys.stdout.isatty()
来源：http://thh.dashuyun.cn

[U40] Py：打印到标准错误
来源：http://zer.dashuyun.cn

print("err", file=sys.stderr)
来源：http://ery.zdqjudy.top

[U41] PHP：初始化 Composer 项目
来源：http://gae.hammf.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ywb.yvedp.cn

[U42] PHP：PSR-4 自动加载
来源：http://ckr.yvedp.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lpn.chenzaomai.com

[U43] PHP：声明命名空间
来源：http://xma.zhiwuduotai.top

namespace App\Http;
来源：http://pdk.hongshengwenyu.top

[U44] PHP：开启严格类型
来源：http://vmd.hammf.cn

declare(strict_types=1);
来源：http://zjo.iojbl.cn


<!-- 参考信息 -->