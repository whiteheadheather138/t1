代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://iuh.hnqzz.top

[S21] C：字符类别判断
来源：http://mfj.316326.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ycc.hnqzz.top

[S22] C：字符串转数字
来源：http://pfa.xylfe.cn

atoi("42");  strtod("3.14", NULL);
来源：http://acr.tianlin.xyz

[S23] C：随机数
来源：http://mhi.xinyue.icu

srand(time(NULL));  int r = rand() % 100;
来源：http://ksl.jinghuilouyu.cn

[S24] C：获取本地时间
来源：http://bfr.hesvh.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zdo.shuidangran.top

[S25] C：内存拷贝
来源：http://wif.shuidangran.top

memcpy(dst, src, n);
来源：http://idx.bjfxy.top

[S26] C：内存清零
来源：http://gvq.xylfe.cn

memset(a, 0, sizeof a);
来源：http://wku.jianghu66.top

[S27] C：定义常量
来源：http://wwk.yanxiufei.cn

const double PI = 3.14159;
来源：http://pey.mhx1999.top

[S28] C：静态变量
来源：http://mke.epnwcf.com

static int counter = 0;
来源：http://gjy.jinghuilouyu.cn

[S29] C：变参函数
来源：http://vwj.haohaochexian.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vwj.shuidangran.top

[S30] C：头文件保护
来源：http://gqt.aibaodan.cn

#ifndef X_H
来源：http://vyk.daria6918.cn

#define X_H
来源：http://jud.fehbvm.com

#endif
来源：http://sdn.jianghu66.top

[S31] C++：Hello World
来源：http://uyi.meibo888.top

#include <iostream>
来源：http://dmy.dianchejie.cn

int main() { std::cout << "Hello\n"; }
来源：http://qnr.ywan-chungtsiang.top

[S32] C++：字符串
来源：http://dfo.zycfv.cn

std::string s = "hi";  s += "!";
来源：http://ahz.cheryme.top

[S33] C++：vector 增删
来源：http://cgu.jinqigufen.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xvu.jqgufenzy.top

[S34] C++：遍历 vector
来源：http://rmb.hongshengwenyu.top

for (auto &x : v) { std::cout << x; }
来源：http://mai.sufxvd.cn

[S35] C++：map
来源：http://opa.sjlbkw.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://uab.yvedp.cn

[S36] C++：unordered_map
来源：http://oor.0kj1m.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cwu.zhengqikj.top

[S37] C++：set
来源：http://ben.shzxlz.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hxp.nwbrower.top

[S38] C++：排序
来源：http://fsd.jqgfzy.top

std::sort(v.begin(), v.end());
来源：http://vbc.meibo888.top

[S39] C++：自定义比较器排序
来源：http://mbq.chenzaomai.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://szw.snrcjt.cn

[S40] C++：查找元素
来源：http://gup.tianlin.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://evf.yuanzhike.top

[S41] C++：类与构造函数
来源：http://zzt.ivvv.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://grm.cashguo.top

[S42] C++：继承与虚函数
来源：http://llp.quarkkingdee.top

class B : public Base { public: void f() override {} };
来源：http://mmz.jinqigufen.top

[S43] C++：智能指针
来源：http://mdx.yuxming.cn

auto p = std::make_unique<int>(5);
来源：http://yal.cucudq.cn

[S44] C++：引用传参
来源：http://sae.cheryme.top

void inc(int &x) { ++x; }
来源：http://lqy.jyoumei.cn

[S45] C++：lambda
来源：http://jbk.zdqjudy.top

auto add = [](int a, int b) { return a + b; };
来源：http://wte.aizwys.cn

[S46] C++：函数模板
来源：http://dfu.ydjk.org.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rbf.hcnkem.com

[S47] C++：结构化绑定遍历
来源：http://dnf.zhijiandao.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ktm.zdqjudy.top

[S48] C++：逐行读文件
来源：http://nhp.sweek.top

std::ifstream in("a.txt");  std::string line;
来源：http://bzl.ctjpmb.com

while (std::getline(in, line)) { }
来源：http://emk.shzxlz.cn

[S49] C++：写文件
来源：http://vak.cashguo.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yjl.sysykeji.top

[S50] C++：格式化数字
来源：http://zzz.tian-w.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://miu.gogol.net.cn

[S51] C++：显式类型转换
来源：http://jyn.hammf.cn

static_cast<double>(a) / b
来源：http://vkr.bbcook.cn

[S52] C++：const 与 noexcept
来源：http://wem.bbcook.cn

int size() const noexcept { return n_; }
来源：http://dzl.hywenlv.cn

[S53] C++：移动语义
来源：http://kjy.gogol.net.cn

std::vector<int> w = std::move(v);
来源：http://cwt.hnxiangtu.top

[S54] C++：异常处理
来源：http://rgn.yonumen.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wnz.hnqzz.top

[S55] C++：结构化绑定
来源：http://vol.fengsongda.top

auto [a, b] = std::make_pair(1, 2);
来源：http://hwk.cdnleiting.top

[S56] C++：optional
来源：http://sso.zhaomingkeji.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gjd.gotoacloud.top

[S57] C++：编译期常量
来源：http://fdg.zhoulong.xyz

constexpr int N = 10;
来源：http://igk.jinqigfzy.top

[S58] C++：命名空间
来源：http://yqh.yj202588.top

namespace ns { int f() { return 1; } }
来源：http://qgk.yuanzhike.top

[S59] C++：静态断言
来源：http://kem.zycfv.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fwd.jyoumei.cn

[S60] C++：遍历并删除元素
来源：http://alo.jlsjyb.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jrv.hnxiangtu.top

================================================================================
来源：http://gmq.yangfankeji.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wlk.yanxiufei.cn

================================================================================
来源：http://klu.feifeiyinyue.top

[T01] Kotlin：Hello World
来源：http://vvc.shanyushiyangtech.top

println("Hello")
来源：http://rnr.fzhhl.top

[T02] Kotlin：变量
来源：http://jdb.9152youxi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ymv.cucudq.cn

[T03] Kotlin：字符串模板
来源：http://kki.yongpay.top

"值: $b"
来源：http://xci.wangdashe.top

[T04] Kotlin：空安全
来源：http://trn.tianlin.xyz

val n: String? = null;  n?.length
来源：http://dyq.cashguo.top

[T05] Kotlin：when 表达式
来源：http://njg.haohaochexian.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cqq.xuanzx.com

[T06] Kotlin：集合映射
来源：http://gea.yueranfly.top

listOf(1, 2, 3).map { it * 2 }
来源：http://xyw.quarkkingdee.top

[T07] Kotlin：集合过滤
来源：http://itu.iojbl.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qgk.cqqwz.cn

[T08] Kotlin：数据类
来源：http://knd.yj202588.top

data class User(val name: String, val age: Int)
来源：http://bje.cheryme.top

[T09] Kotlin：扩展函数
来源：http://mfg.svipenyu.cn

fun String.exclaim() = this + "!"
来源：http://npd.aizwys.cn

[T10] Kotlin：默认参数
来源：http://ovd.chenjidiqi.icu

fun greet(name: String = "World") = "Hi $name"
来源：http://xip.yfazqb.com

[T11] Kotlin：协程
来源：http://oou.cucudq.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://pkv.yj20258.top

[T12] Kotlin：解构声明
来源：http://zbf.yuanzhike.top

val (a, b) = Pair(1, 2)
来源：http://lfw.jinqigufen.top

[T13] Kotlin：只读 Map
来源：http://kff.ppjwa.cn

val m = mapOf("a" to 1)
来源：http://klb.ywan-chungtsiang.top

[T14] Kotlin：循环
来源：http://xqd.ctjpmb.com

for (i in 1..10) println(i)
来源：http://zwe.fengsongda.top

[T15] Kotlin：接口
来源：http://iji.zdbjq.cn

interface Shape { fun area(): Double }
来源：http://sva.hnxiangtu.top

[T16] Swift：Hello World
来源：http://hqi.haohaochexian.top

print("Hello")
来源：http://ffn.hcnkem.com

[T17] Swift：变量与常量
来源：http://dan.cucudq.cn

var a = 1;  let b = 2
来源：http://usw.nwbrower.top

[T18] Swift：字符串插值
来源：http://zkc.ehwqpu.com

"值: \(b)"
来源：http://sfv.xuanzx.com

[T19] Swift：可选绑定
来源：http://eup.yuanzhike.top

if let n = opt { print(n) }
来源：http://mvd.zhaomingkeji.xyz

[T20] Swift：数组操作
来源：http://law.316326.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://tvq.yfazqb.com

[T21] Swift：遍历
来源：http://unp.hywenlv.cn

for x in a { print(x) }
来源：http://jny.fktsv.cn

[T22] Swift：字典
来源：http://pse.sufxvd.cn

var d = ["a": 1];  d["b"] = 2
来源：http://snj.yanxiufei.cn

[T23] Swift：函数
来源：http://vaj.shanyushiyangtech.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vvp.yueranfly.top

[T24] Swift：闭包
来源：http://zsp.yangfankeji.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://mlu.gogol.net.cn

[T25] Swift：结构体
来源：http://kiw.hywenlv.cn

struct P { var x: Int }
来源：http://hlh.hfpthk.cn

[T26] Swift：类与重写
来源：http://dxv.yueranfly.top

class A: Base { override func f() {} }
来源：http://jnx.yuanzhike.top

[T27] Swift：错误处理
来源：http://dek.jlsjyb.cn

do { try f() } catch { print(error) }
来源：http://abk.hysaishi.cn

[T28] Swift：枚举
来源：http://tkr.xylfe.cn

enum Color { case red, green }
来源：http://fad.iojbl.cn

[T29] Swift：guard 提前返回
来源：http://ibg.ydzc1.top

guard let x = opt else { return }
来源：http://cif.havefunace.top

[T30] Swift：协议
来源：http://ddf.daria6918.cn

protocol Shape { func area() -> Double }
来源：http://mau.xingfuxueyuan.xyz

[T31] Lua：Hello World
来源：http://rsd.cqqwz.cn

print("Hello")
来源：http://khn.sysykeji.top

[T32] Lua：局部变量
来源：http://tzy.nanxuanxn.top

local a = 1
来源：http://edm.uphjek.com

[T33] Lua：表（数组）
来源：http://tnc.cashguo.top

local t = {1, 2, 3};  t[4] = 4
来源：http://zev.yj202588.top

[T34] Lua：遍历表
来源：http://mqj.zhixingplan.top

for i, v in ipairs(t) do print(i, v) end
来源：http://alo.ydjk.org.cn

[T35] Lua：字典表
来源：http://jqf.zdqjudy.top

local d = { a = 1 };  d.b = 2
来源：http://gry.jqgufenzy.top

[T36] Lua：函数
来源：http://jfy.jinqigufen.top

function add(a, b) return a + b end
来源：http://hml.smart0.xyz

[T37] Lua：字符串拼接
来源：http://mjn.meibo888.top

"a" .. "b"
来源：http://sya.gotoacloud.top

[T38] Lua：条件
来源：http://idd.tian-w.cn

if x > 0 then print("正") end
来源：http://qvx.hysaishi.cn

[T39] Lua：模式匹配
来源：http://ehr.vqdsnc.cn

string.find(s, "%d+")
来源：http://xrd.snrcjt.cn

[T40] Lua：元表
来源：http://vbr.hcnkem.com

setmetatable({}, { __index = base })
来源：http://nsh.yongpay.top

[T41] Perl：Hello World
来源：http://blp.yfazqb.com

print "Hello\n";
来源：http://vmf.pengpengdd.cyou

[T42] Perl：变量类型
来源：http://jji.fengsongda.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gzp.jianghu66.top

[T43] Perl：字符串插值
来源：http://hmk.feifeiyinyue.top

"值: $a"
来源：http://ohm.shanyushiyangtech.top

[T44] Perl：条件
来源：http://ekk.redwolf501.top

if ($a > 0) { print "正"; }
来源：http://vki.fehbvm.com

[T45] Perl：数组遍历
来源：http://tzx.shzxlz.cn

for my $x (@arr) { print $x; }
来源：http://trv.sysykeji.top

[T46] Perl：哈希操作
来源：http://cbk.bjfxy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://llz.yfazqb.com

[T47] Perl：正则捕获
来源：http://kio.jlsjyb.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ogt.xinyue.icu

[T48] Perl：正则替换
来源：http://jvp.nanxuanxn.top

$s =~ s/old/new/g;
来源：http://fwj.jqgufenzy.top

[T49] Perl：函数
来源：http://bbs.xuanzx.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ssp.gzhubu.top

[T50] Perl：逐行读文件
来源：http://ovl.yonumen.top

open my $fh, "<", "a.txt" or die $!;
来源：http://poc.hammf.cn

while (my $line = <$fh>) { print $line; }
来源：http://jyt.havefunace.top

[T51] Scala：Hello World
来源：http://xov.hongshengwenyu.top

println("Hello")
来源：http://dwg.guowangkeji.top

[T52] Scala：变量
来源：http://grd.ppjwa.cn

val a = 1;  var b = 2
来源：http://dri.zhijiandao.cn

[T53] Scala：字符串插值
来源：http://gwu.tarul.cn

s"值: $b"
来源：http://ald.yangfankeji.com

[T54] Scala：集合映射
来源：http://zat.ivvv.top

List(1, 2, 3).map(_ * 2)
来源：http://vbx.0kj1m.cn

[T55] Scala：集合过滤
来源：http://vjt.tian-w.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ieo.fehbvm.com

[T56] Scala：样例类
来源：http://znt.yj202588.top

case class User(name: String, age: Int)
来源：http://hpj.pengpengdd.cyou

[T57] Scala：模式匹配
来源：http://fvm.jyoumei.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://hwu.jiagoushi.top

[T58] Scala：函数定义
来源：http://ntg.ivvv.top

def add(a: Int, b: Int): Int = a + b
来源：http://kgh.guowangkeji.top

[T59] Scala：循环
来源：http://piy.vqdsnc.cn

for (i <- 1 to 10) println(i)
来源：http://kas.xinyue.icu

[T60] Scala：折叠
来源：http://lqq.gzhubu.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ylg.snrcjt.cn

================================================================================
来源：http://kkf.nanxuanxn.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://sfa.redwolf501.top

================================================================================
来源：http://fbh.daxiang520.top

[U01] Py：创建虚拟环境
来源：http://ulx.kuanghao11.cn

python -m venv .venv && source .venv/bin/activate
来源：http://sbu.cucudq.cn

[U02] Py：导出 / 安装依赖
来源：http://xdo.nanxinkj.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bwt.tianlin.xyz

[U03] Py：加载 .env 配置
来源：http://hbp.hysaishi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://uqp.fanxiaobao.xyz

[U04] Py：变量调试打印
来源：http://iel.xinyue.icu

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pzq.haohaochexian.top

[U05] Py：列表去重且保序
来源：http://akj.jiagoushi.top

list(dict.fromkeys(arr))
来源：http://lht.yj20258888.top

[U06] Py：合并两个字典
来源：http://gdi.zhongyouzk.top

{**a, **b}
来源：http://ids.ybcxt.top

[U07] Py：反转字典键值
来源：http://tdh.dianchejie.cn

{v: k for k, v in d.items()}
来源：http://oqq.chenjidiqi.icu

[U08] Py：展平二维列表
来源：http://whf.smart0.xyz

[y for x in nested for y in x]
来源：http://qth.yvedp.cn

[U09] Py：字典取最大值的键
来源：http://bbu.vehdjk.com

max(d, key=d.get)
来源：http://wty.sxryk.cn

[U10] Py：按值排序字典
来源：http://sro.shzxlz.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rii.xziqi.cn

[U11] Py：生成器表达式
来源：http://hjt.gaohongyu789.top

(x * 2 for x in arr)
来源：http://kdx.xziqi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://rbn.cheryme.top

Counter(arr).most_common(3)
来源：http://fjb.fktsv.cn

[U13] Py：固定长度队列
来源：http://gxj.nwbrower.top

deque(maxlen=10)
来源：http://dbe.cdnleiting.top

[U14] Py：分组收集到列表
来源：http://act.tarul.cn

defaultdict(list)
来源：http://ggu.fehbvm.com

[U15] Py：高精度计时
来源：http://khi.hongshengwenyu.top

t = time.perf_counter()
来源：http://nhf.zdbjq.cn

[U16] Py：命令行参数解析
来源：http://ugi.jinyuanbaomall.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://div.yj20258.top

[U17] Py：初始化日志
来源：http://ycg.hnxiangtu.top

logging.basicConfig(level=logging.INFO)
来源：http://xxe.yueranfly.top

[U18] Py：预编译正则
来源：http://cok.guowangkeji.top

pat = re.compile(r"\d+")
来源：http://rys.fengsongda.top

[U19] Py：正则替换带回调
来源：http://wyz.yj20258888.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ssc.jinqigufen.top

[U20] Py：缓存函数结果
来源：http://isq.mhx1999.top

@functools.lru_cache(maxsize=None)
来源：http://vmv.xinyue.icu

[U21] Py：自定义上下文管理器
来源：http://wpg.guannengcc.top

@contextlib.contextmanager
来源：http://wwh.nanxinkj.top

[U22] Py：矩阵转置
来源：http://ihd.yj20258888.top

list(zip(*m))
来源：http://zko.wangdashe.top

[U23] Py：分块读取大文件
来源：http://wmt.jyoumei.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://drg.hywenlv.cn

[U24] Py：路径操作
来源：http://pwr.xylfe.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zbj.vqdsnc.cn

[U25] Py：CSV 按字典读
来源：http://asx.xuanzx.com

csv.DictReader(f)
来源：http://see.bjfxy.top

[U26] Py：并发下载
来源：http://kjr.shuidangran.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jaj.snrcjt.cn

[U27] Py：异步 HTTP
来源：http://zwx.sysykeji.top

aiohttp.ClientSession() 配合 async with
来源：http://gdh.shzxlz.cn

[U28] Py：类型别名
来源：http://pgr.zhengqikj.top

UserId = int
来源：http://jez.shanyushiyangkeji.top

[U29] Py：属性校验
来源：http://dmg.feifeiyinyue.top

@property 与 @x.setter 配合
来源：http://vvu.fehbvm.com

[U30] Py：数据类
来源：http://oag.shanyushiyangkeji.top

@dataclass(slots=True)
来源：http://ila.yj202588.top

[U31] Py：单测
来源：http://vzb.zhixingplan.top

python -m pytest -q
来源：http://vfp.dianchejie.cn

[U32] Py：代码格式化
来源：http://cfk.zhaomingkeji.xyz

ruff format . && ruff check --fix .
来源：http://chl.jyoumei.cn

[U33] Py：打包发布
来源：http://kxz.guowangkeji.top

python -m build  （依赖 pyproject.toml）
来源：http://pas.tianlin.xyz

[U34] Py：判断编码
来源：http://ojf.zhaomingkeji.xyz

chardet.detect(raw)
来源：http://abt.cqqwz.cn

[U35] Py：发送邮件
来源：http://zjp.xylfe.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kar.feifeiyinyue.top

[U36] Py：定时任务
来源：http://gwp.sysykeji.top

schedule.every(10).minutes.do(job)
来源：http://qco.nanxuanxn.top

[U37] Py：读写 Excel
来源：http://jdj.vqdsnc.cn

pandas.read_excel / DataFrame.to_excel
来源：http://yvy.nanxinkj.top

[U38] Py：获取脚本所在目录
来源：http://dpt.vqdsnc.cn

Path(__file__).resolve().parent
来源：http://stp.daxiang520.top

[U39] Py：判断是否在交互环境
来源：http://xhs.guannengcc.top

sys.stdout.isatty()
来源：http://xpr.tianlin.xyz

[U40] Py：打印到标准错误
来源：http://zin.ehwqpu.com

print("err", file=sys.stderr)
来源：http://zig.fktsv.cn

[U41] PHP：初始化 Composer 项目
来源：http://duw.yj20258.top

composer init;  composer require guzzlehttp/guzzle
来源：http://uiu.tianlin.xyz

[U42] PHP：PSR-4 自动加载
来源：http://tvt.tanke756.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wxg.316326.xyz

[U43] PHP：声明命名空间
来源：http://sna.c1oappe.top

namespace App\Http;
来源：http://pcg.pycfn.com

[U44] PHP：开启严格类型
来源：http://kxv.chenjidiqi.icu

declare(strict_types=1);
来源：http://ztm.cdnleiting.top


<!-- 参考信息 -->