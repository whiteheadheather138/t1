代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rax.vehdjk.com

[S21] C：字符类别判断
来源：http://irq.yongpay.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fka.yfazqb.com

[S22] C：字符串转数字
来源：http://zhb.yueranfly.top

atoi("42");  strtod("3.14", NULL);
来源：http://rph.snrcjt.cn

[S23] C：随机数
来源：http://muf.jqgufenzy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://osj.mhx1999.top

[S24] C：获取本地时间
来源：http://pjm.shanyushiyangtech.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xkt.nanxinkj.top

[S25] C：内存拷贝
来源：http://ibo.ctjpmb.com

memcpy(dst, src, n);
来源：http://evs.dianchejie.cn

[S26] C：内存清零
来源：http://dyt.chenjidiqi.icu

memset(a, 0, sizeof a);
来源：http://iyl.hongshengwenyu.top

[S27] C：定义常量
来源：http://caj.zhaomingkeji.xyz

const double PI = 3.14159;
来源：http://uja.snrcjt.cn

[S28] C：静态变量
来源：http://ykd.0kj1m.cn

static int counter = 0;
来源：http://tsz.andypj.xyz

[S29] C：变参函数
来源：http://wta.guowangkeji.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ars.cashguo.top

[S30] C：头文件保护
来源：http://don.jlsjyb.cn

#ifndef X_H
来源：http://iis.vqdsnc.cn

#define X_H
来源：http://gsm.ctjpmb.com

#endif
来源：http://ujw.xylfe.cn

[S31] C++：Hello World
来源：http://pwb.chenzaomai.com

#include <iostream>
来源：http://ssb.zycfv.cn

int main() { std::cout << "Hello\n"; }
来源：http://irz.ydjk.org.cn

[S32] C++：字符串
来源：http://gdl.wangdashe.top

std::string s = "hi";  s += "!";
来源：http://kfu.jiagoushi.top

[S33] C++：vector 增删
来源：http://crn.chenlongwang.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tyg.chenzaomai.com

[S34] C++：遍历 vector
来源：http://jrj.epnwcf.com

for (auto &x : v) { std::cout << x; }
来源：http://hxo.tian-w.cn

[S35] C++：map
来源：http://ovr.nanxinkj.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mzo.andypj.xyz

[S36] C++：unordered_map
来源：http://ico.cdnleiting.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zcz.jqgfzy.top

[S37] C++：set
来源：http://kdg.haohaochexian.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zvx.yonumen.top

[S38] C++：排序
来源：http://tos.yj20258888.top

std::sort(v.begin(), v.end());
来源：http://gzs.ydzc1.top

[S39] C++：自定义比较器排序
来源：http://hkk.fktsv.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://iqy.vqdsnc.cn

[S40] C++：查找元素
来源：http://uhw.yfazqb.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://czg.epnwcf.com

[S41] C++：类与构造函数
来源：http://zdf.hfpthk.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mgj.hammf.cn

[S42] C++：继承与虚函数
来源：http://kfl.tarul.cn

class B : public Base { public: void f() override {} };
来源：http://tax.xuanzx.com

[S43] C++：智能指针
来源：http://whn.52xcode.cn

auto p = std::make_unique<int>(5);
来源：http://ubu.hywenlv.cn

[S44] C++：引用传参
来源：http://zcc.hnxiangtu.top

void inc(int &x) { ++x; }
来源：http://clh.yongpay.top

[S45] C++：lambda
来源：http://xdg.chenzaomai.com

auto add = [](int a, int b) { return a + b; };
来源：http://nms.jinqigufen.top

[S46] C++：函数模板
来源：http://gve.shzxlz.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hpp.chenlongwang.top

[S47] C++：结构化绑定遍历
来源：http://egj.hysaishi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mhg.hnxiangtu.top

[S48] C++：逐行读文件
来源：http://ant.52xcode.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jkr.pycfn.com

while (std::getline(in, line)) { }
来源：http://sch.zhijiandao.cn

[S49] C++：写文件
来源：http://rqg.shanyushiyangkeji.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gij.9152youxi.cn

[S50] C++：格式化数字
来源：http://ffj.hnqzz.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://obf.ppjwa.cn

[S51] C++：显式类型转换
来源：http://nqz.xziqi.cn

static_cast<double>(a) / b
来源：http://xog.ywan-chungtsiang.top

[S52] C++：const 与 noexcept
来源：http://ssz.haohaochexian.top

int size() const noexcept { return n_; }
来源：http://wcl.gaohongyu789.top

[S53] C++：移动语义
来源：http://spd.shangyingyoupin.top

std::vector<int> w = std::move(v);
来源：http://jga.gogol.net.cn

[S54] C++：异常处理
来源：http://lcd.fktsv.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://alw.gogol.net.cn

[S55] C++：结构化绑定
来源：http://hug.tianlin.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://yqu.fktsv.cn

[S56] C++：optional
来源：http://brn.bbcook.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ntp.hysaishi.cn

[S57] C++：编译期常量
来源：http://jbv.gogol.net.cn

constexpr int N = 10;
来源：http://lri.smart0.xyz

[S58] C++：命名空间
来源：http://zbd.ywan-chungtsiang.top

namespace ns { int f() { return 1; } }
来源：http://kap.svipenyu.cn

[S59] C++：静态断言
来源：http://eto.gogol.net.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zpt.vehdjk.com

[S60] C++：遍历并删除元素
来源：http://pkk.jyoumei.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://esm.tian-w.cn

================================================================================
来源：http://kgi.bbcook.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vqv.fengsongda.top

================================================================================
来源：http://vkf.cashguo.top

[T01] Kotlin：Hello World
来源：http://wcv.zhiwuduotai.top

println("Hello")
来源：http://kgy.cucudq.cn

[T02] Kotlin：变量
来源：http://hfg.jyoumei.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ctv.jqgufenzy.top

[T03] Kotlin：字符串模板
来源：http://yef.epnwcf.com

"值: $b"
来源：http://wfr.zhiwuduotai.top

[T04] Kotlin：空安全
来源：http://uky.nwbrower.top

val n: String? = null;  n?.length
来源：http://thl.meibo888.top

[T05] Kotlin：when 表达式
来源：http://esj.hammf.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gre.hnqzz.top

[T06] Kotlin：集合映射
来源：http://sqj.nanxinkj.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ahm.zhaomingkeji.xyz

[T07] Kotlin：集合过滤
来源：http://gjp.shuidangran.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://adw.iojbl.cn

[T08] Kotlin：数据类
来源：http://vot.yangfankeji.com

data class User(val name: String, val age: Int)
来源：http://raw.jianghu66.top

[T09] Kotlin：扩展函数
来源：http://cao.hammf.cn

fun String.exclaim() = this + "!"
来源：http://zju.jinqigufen.top

[T10] Kotlin：默认参数
来源：http://yoq.guannengcc.top

fun greet(name: String = "World") = "Hi $name"
来源：http://zfy.daxiang520.top

[T11] Kotlin：协程
来源：http://kro.fanxiaobao.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://yah.wangdashe.top

[T12] Kotlin：解构声明
来源：http://bvs.gaohongyu789.top

val (a, b) = Pair(1, 2)
来源：http://ryc.daria6918.cn

[T13] Kotlin：只读 Map
来源：http://mlx.uphjek.com

val m = mapOf("a" to 1)
来源：http://upx.zdqjudy.top

[T14] Kotlin：循环
来源：http://dpn.jianghu66.top

for (i in 1..10) println(i)
来源：http://nzi.zycfv.cn

[T15] Kotlin：接口
来源：http://kra.yj202588.top

interface Shape { fun area(): Double }
来源：http://yfg.zhongyouzk.top

[T16] Swift：Hello World
来源：http://gli.hnqzz.top

print("Hello")
来源：http://lom.fzhhl.top

[T17] Swift：变量与常量
来源：http://uwb.jlsjyb.cn

var a = 1;  let b = 2
来源：http://hqt.xingfuxueyuan.xyz

[T18] Swift：字符串插值
来源：http://twa.9152youxi.cn

"值: \(b)"
来源：http://ccl.yanxiufei.cn

[T19] Swift：可选绑定
来源：http://sdc.quarkkingdee.top

if let n = opt { print(n) }
来源：http://fph.quarkkingdee.top

[T20] Swift：数组操作
来源：http://ljr.zhaomingkeji.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://ihv.mhx1999.top

[T21] Swift：遍历
来源：http://hih.yuanzhike.top

for x in a { print(x) }
来源：http://rwf.nwbrower.top

[T22] Swift：字典
来源：http://xsn.yueranfly.top

var d = ["a": 1];  d["b"] = 2
来源：http://mhc.zhaomingkeji.xyz

[T23] Swift：函数
来源：http://ppv.yangfankeji.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://sdb.ivvv.top

[T24] Swift：闭包
来源：http://yur.iojbl.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://lhf.yanxiufei.cn

[T25] Swift：结构体
来源：http://mic.c1oappe.top

struct P { var x: Int }
来源：http://rye.wangdashe.top

[T26] Swift：类与重写
来源：http://nat.fanxiaobao.xyz

class A: Base { override func f() {} }
来源：http://rjo.hcnkem.com

[T27] Swift：错误处理
来源：http://evd.iojbl.cn

do { try f() } catch { print(error) }
来源：http://qwq.yanxiufei.cn

[T28] Swift：枚举
来源：http://rwr.yj20258888.top

enum Color { case red, green }
来源：http://upe.yuanzhike.top

[T29] Swift：guard 提前返回
来源：http://dwy.shangyingyoupin.top

guard let x = opt else { return }
来源：http://znp.shanyushiyangtech.top

[T30] Swift：协议
来源：http://rek.yuxming.cn

protocol Shape { func area() -> Double }
来源：http://eip.xylfe.cn

[T31] Lua：Hello World
来源：http://nzz.ydjk.org.cn

print("Hello")
来源：http://skm.9152youxi.cn

[T32] Lua：局部变量
来源：http://hfp.wangshuangyany.cn

local a = 1
来源：http://xlw.gotoacloud.top

[T33] Lua：表（数组）
来源：http://qok.cqqwz.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ptx.zdqjudy.top

[T34] Lua：遍历表
来源：http://hjh.fktsv.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://aji.wangshuangyany.cn

[T35] Lua：字典表
来源：http://tix.shuidangran.top

local d = { a = 1 };  d.b = 2
来源：http://mfn.daxiang520.top

[T36] Lua：函数
来源：http://fvi.iojbl.cn

function add(a, b) return a + b end
来源：http://dwg.zhoulong.xyz

[T37] Lua：字符串拼接
来源：http://mmv.andypj.xyz

"a" .. "b"
来源：http://wff.zycfv.cn

[T38] Lua：条件
来源：http://fuj.c1oappe.top

if x > 0 then print("正") end
来源：http://lpl.meibo888.top

[T39] Lua：模式匹配
来源：http://srn.xuetiantiany.cn

string.find(s, "%d+")
来源：http://uea.zdqjudy.top

[T40] Lua：元表
来源：http://rjf.quarkkingdee.top

setmetatable({}, { __index = base })
来源：http://lfh.yfazqb.com

[T41] Perl：Hello World
来源：http://gyq.zdbjq.cn

print "Hello\n";
来源：http://uwx.hammf.cn

[T42] Perl：变量类型
来源：http://xnp.chenlongwang.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wuw.zhongyouzk.top

[T43] Perl：字符串插值
来源：http://zup.xuanzx.com

"值: $a"
来源：http://nqm.zdqjudy.top

[T44] Perl：条件
来源：http://mwn.zdqjudy.top

if ($a > 0) { print "正"; }
来源：http://oon.xinyue.icu

[T45] Perl：数组遍历
来源：http://kvi.uphjek.com

for my $x (@arr) { print $x; }
来源：http://hlj.jianghu66.top

[T46] Perl：哈希操作
来源：http://utr.yj20258.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cqa.gaohongyu789.top

[T47] Perl：正则捕获
来源：http://xrs.yj202588.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://fyr.fzhhl.top

[T48] Perl：正则替换
来源：http://jjt.shanyushiyangtech.top

$s =~ s/old/new/g;
来源：http://qfp.zdqjudy.top

[T49] Perl：函数
来源：http://zqq.jlsjyb.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kvu.kuanghao11.cn

[T50] Perl：逐行读文件
来源：http://fgq.c1oappe.top

open my $fh, "<", "a.txt" or die $!;
来源：http://qjz.pycfn.com

while (my $line = <$fh>) { print $line; }
来源：http://dtc.hnqzz.top

[T51] Scala：Hello World
来源：http://lxq.yonumen.top

println("Hello")
来源：http://rtv.hongshengwenyu.top

[T52] Scala：变量
来源：http://uhk.hywenlv.cn

val a = 1;  var b = 2
来源：http://dpk.hesvh.cn

[T53] Scala：字符串插值
来源：http://yfk.c1oappe.top

s"值: $b"
来源：http://eyr.ydzc1.top

[T54] Scala：集合映射
来源：http://hmp.jyoumei.cn

List(1, 2, 3).map(_ * 2)
来源：http://low.daxiang520.top

[T55] Scala：集合过滤
来源：http://duq.zhongyouzk.top

List(1, 2, 3).filter(_ > 1)
来源：http://wpt.ctjpmb.com

[T56] Scala：样例类
来源：http://dgt.xylfe.cn

case class User(name: String, age: Int)
来源：http://hyx.jinqigfzy.top

[T57] Scala：模式匹配
来源：http://cnx.0kj1m.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://alm.shangyingyoupin.top

[T58] Scala：函数定义
来源：http://pne.ybcxt.top

def add(a: Int, b: Int): Int = a + b
来源：http://ved.bjfxy.top

[T59] Scala：循环
来源：http://hrx.fzhhl.top

for (i <- 1 to 10) println(i)
来源：http://uaj.yuxming.cn

[T60] Scala：折叠
来源：http://kqz.ywan-chungtsiang.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rjl.9152youxi.cn

================================================================================
来源：http://ftl.gzhubu.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xyl.jiagoushi.top

================================================================================
来源：http://abv.shuidangran.top

[U01] Py：创建虚拟环境
来源：http://kps.ivvv.top

python -m venv .venv && source .venv/bin/activate
来源：http://tch.jqgfzy.top

[U02] Py：导出 / 安装依赖
来源：http://whf.cheryme.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rma.wangshuangyany.cn

[U03] Py：加载 .env 配置
来源：http://jpu.meibo888.top

from dotenv import load_dotenv; load_dotenv()
来源：http://xfw.guowangkeji.top

[U04] Py：变量调试打印
来源：http://aky.jqgfzy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ugs.ydzc1.top

[U05] Py：列表去重且保序
来源：http://ynl.ydzc1.top

list(dict.fromkeys(arr))
来源：http://vbi.gaohongyu789.top

[U06] Py：合并两个字典
来源：http://ywc.shzxlz.cn

{**a, **b}
来源：http://yjf.cdnleiting.top

[U07] Py：反转字典键值
来源：http://wfq.sjlbkw.cn

{v: k for k, v in d.items()}
来源：http://kgm.snrcjt.cn

[U08] Py：展平二维列表
来源：http://fpc.haohaochexian.top

[y for x in nested for y in x]
来源：http://uks.0kj1m.cn

[U09] Py：字典取最大值的键
来源：http://hwe.guannengcc.top

max(d, key=d.get)
来源：http://pvg.fktsv.cn

[U10] Py：按值排序字典
来源：http://avd.xinyue.icu

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tov.guowangkeji.top

[U11] Py：生成器表达式
来源：http://rem.zhoulong.xyz

(x * 2 for x in arr)
来源：http://ten.hysaishi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://maa.mhx1999.top

Counter(arr).most_common(3)
来源：http://xol.nanxinkj.top

[U13] Py：固定长度队列
来源：http://edo.iojbl.cn

deque(maxlen=10)
来源：http://orn.dashuyun.cn

[U14] Py：分组收集到列表
来源：http://nqf.sjlbkw.cn

defaultdict(list)
来源：http://mcm.yj202588.top

[U15] Py：高精度计时
来源：http://byc.jyoumei.cn

t = time.perf_counter()
来源：http://bxf.chenlongwang.top

[U16] Py：命令行参数解析
来源：http://kyp.xinyue.icu

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sgy.shanyushiyangkeji.top

[U17] Py：初始化日志
来源：http://lbr.gotoacloud.top

logging.basicConfig(level=logging.INFO)
来源：http://ofa.hesvh.cn

[U18] Py：预编译正则
来源：http://eug.uphjek.com

pat = re.compile(r"\d+")
来源：http://jwh.ydjk.org.cn

[U19] Py：正则替换带回调
来源：http://bpp.mhx1999.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xgd.hcnkem.com

[U20] Py：缓存函数结果
来源：http://fww.gotoacloud.top

@functools.lru_cache(maxsize=None)
来源：http://yod.hnqzz.top

[U21] Py：自定义上下文管理器
来源：http://jki.jinghuilouyu.cn

@contextlib.contextmanager
来源：http://wlo.yj202588.top

[U22] Py：矩阵转置
来源：http://wgd.sxryk.cn

list(zip(*m))
来源：http://vvb.316326.xyz

[U23] Py：分块读取大文件
来源：http://qos.dianchejie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://emt.shanyushiyangtech.top

[U24] Py：路径操作
来源：http://pla.ehwqpu.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pcr.mhx1999.top

[U25] Py：CSV 按字典读
来源：http://snl.xuetiantiany.cn

csv.DictReader(f)
来源：http://dhu.chenjidiqi.icu

[U26] Py：并发下载
来源：http://uxs.ydzc1.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://kbh.cucudq.cn

[U27] Py：异步 HTTP
来源：http://sxg.jiagoushi.top

aiohttp.ClientSession() 配合 async with
来源：http://rbc.jqgfzy.top

[U28] Py：类型别名
来源：http://wci.cdnleiting.top

UserId = int
来源：http://bue.fzhhl.top

[U29] Py：属性校验
来源：http://fxp.dashuyun.cn

@property 与 @x.setter 配合
来源：http://bmx.pengpengdd.cyou

[U30] Py：数据类
来源：http://udt.uphjek.com

@dataclass(slots=True)
来源：http://rxd.nanxuanxn.top

[U31] Py：单测
来源：http://lyw.fzhhl.top

python -m pytest -q
来源：http://rxp.quarkkingdee.top

[U32] Py：代码格式化
来源：http://idu.epnwcf.com

ruff format . && ruff check --fix .
来源：http://gxe.jinqigfzy.top

[U33] Py：打包发布
来源：http://bbi.hywenlv.cn

python -m build  （依赖 pyproject.toml）
来源：http://buq.yuxming.cn

[U34] Py：判断编码
来源：http://paw.yfazqb.com

chardet.detect(raw)
来源：http://kvn.xuetiantiany.cn

[U35] Py：发送邮件
来源：http://ihs.bbcook.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://spr.ehwqpu.com

[U36] Py：定时任务
来源：http://wqy.havefunace.top

schedule.every(10).minutes.do(job)
来源：http://nsd.zhixingplan.top

[U37] Py：读写 Excel
来源：http://bma.zhengqikj.top

pandas.read_excel / DataFrame.to_excel
来源：http://hcu.pycfn.com

[U38] Py：获取脚本所在目录
来源：http://vzl.smart0.xyz

Path(__file__).resolve().parent
来源：http://zle.zdbjq.cn

[U39] Py：判断是否在交互环境
来源：http://itu.hammf.cn

sys.stdout.isatty()
来源：http://qwg.haohaochexian.top

[U40] Py：打印到标准错误
来源：http://osg.cdnleiting.top

print("err", file=sys.stderr)
来源：http://iyy.chenjidiqi.icu

[U41] PHP：初始化 Composer 项目
来源：http://jzv.fanxiaobao.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://ucr.guannengcc.top

[U42] PHP：PSR-4 自动加载
来源：http://ccu.birdmap.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yuo.gaohongyu789.top

[U43] PHP：声明命名空间
来源：http://vuo.jinqigfzy.top

namespace App\Http;
来源：http://iul.yueranfly.top

[U44] PHP：开启严格类型
来源：http://wsa.fzhhl.top

declare(strict_types=1);
来源：http://par.ehwqpu.com


<!-- 参考信息 -->