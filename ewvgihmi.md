代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qcy.kuanghao11.cn

[S21] C：字符类别判断
来源：http://tim.yfazqb.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jbe.yj202588.top

[S22] C：字符串转数字
来源：http://vrf.316326.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://feb.gaohongyu789.top

[S23] C：随机数
来源：http://nqn.xuanzx.com

srand(time(NULL));  int r = rand() % 100;
来源：http://xvh.ehwqpu.com

[S24] C：获取本地时间
来源：http://dti.9152youxi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rnm.havefunace.top

[S25] C：内存拷贝
来源：http://jaj.vqdsnc.cn

memcpy(dst, src, n);
来源：http://xka.xziqi.cn

[S26] C：内存清零
来源：http://tph.smart0.xyz

memset(a, 0, sizeof a);
来源：http://sdl.ybcxt.top

[S27] C：定义常量
来源：http://kyc.tanke756.top

const double PI = 3.14159;
来源：http://bkp.yuxming.cn

[S28] C：静态变量
来源：http://fng.snrcjt.cn

static int counter = 0;
来源：http://qfu.kuanghao11.cn

[S29] C：变参函数
来源：http://nhf.gotoacloud.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tbu.andypj.xyz

[S30] C：头文件保护
来源：http://rlg.wangshuangyany.cn

#ifndef X_H
来源：http://qzn.xylfe.cn

#define X_H
来源：http://eyq.meibo888.top

#endif
来源：http://jqp.yj20258888.top

[S31] C++：Hello World
来源：http://pxg.wangshuangyany.cn

#include <iostream>
来源：http://moa.yangfankeji.com

int main() { std::cout << "Hello\n"; }
来源：http://adl.svipenyu.cn

[S32] C++：字符串
来源：http://hjx.sjlbkw.cn

std::string s = "hi";  s += "!";
来源：http://xrs.jinyuanbaomall.cn

[S33] C++：vector 增删
来源：http://cfz.cdnleiting.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vhy.yj20258.top

[S34] C++：遍历 vector
来源：http://uda.cdnleiting.top

for (auto &x : v) { std::cout << x; }
来源：http://gme.ydzc1.top

[S35] C++：map
来源：http://idu.daxiang520.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://msu.zhiwuduotai.top

[S36] C++：unordered_map
来源：http://nuq.tarul.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ijo.cqqwz.cn

[S37] C++：set
来源：http://hqr.wangdashe.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ipj.316326.xyz

[S38] C++：排序
来源：http://cxn.chenlongwang.top

std::sort(v.begin(), v.end());
来源：http://pvj.feifeiyinyue.top

[S39] C++：自定义比较器排序
来源：http://olm.fzhhl.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://eml.fengsongda.top

[S40] C++：查找元素
来源：http://rcj.yanxiufei.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mra.shanyushiyangtech.top

[S41] C++：类与构造函数
来源：http://ktn.redwolf501.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://imb.cucudq.cn

[S42] C++：继承与虚函数
来源：http://qju.zdbjq.cn

class B : public Base { public: void f() override {} };
来源：http://hta.redwolf501.top

[S43] C++：智能指针
来源：http://waa.pycfn.com

auto p = std::make_unique<int>(5);
来源：http://nyz.hesvh.cn

[S44] C++：引用传参
来源：http://mje.cucudq.cn

void inc(int &x) { ++x; }
来源：http://ypz.cucudq.cn

[S45] C++：lambda
来源：http://dhy.fengsongda.top

auto add = [](int a, int b) { return a + b; };
来源：http://iqz.daxiang520.top

[S46] C++：函数模板
来源：http://lbo.dashuyun.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bfx.wangdashe.top

[S47] C++：结构化绑定遍历
来源：http://roj.52xcode.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mvx.fzhhl.top

[S48] C++：逐行读文件
来源：http://rke.uphjek.com

std::ifstream in("a.txt");  std::string line;
来源：http://faf.jqgfzy.top

while (std::getline(in, line)) { }
来源：http://swr.cheryme.top

[S49] C++：写文件
来源：http://fer.yvedp.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jlz.yuanzhike.top

[S50] C++：格式化数字
来源：http://yra.xuanzx.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sui.hongshengwenyu.top

[S51] C++：显式类型转换
来源：http://tiu.zhiwuduotai.top

static_cast<double>(a) / b
来源：http://yel.uphjek.com

[S52] C++：const 与 noexcept
来源：http://uak.xziqi.cn

int size() const noexcept { return n_; }
来源：http://muz.yueranfly.top

[S53] C++：移动语义
来源：http://dkh.ehwqpu.com

std::vector<int> w = std::move(v);
来源：http://bdn.mhx1999.top

[S54] C++：异常处理
来源：http://cap.yj20258.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cdr.ppjwa.cn

[S55] C++：结构化绑定
来源：http://hcl.dashuyun.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://lhu.dianchejie.cn

[S56] C++：optional
来源：http://dsw.gzhubu.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lzf.tarul.cn

[S57] C++：编译期常量
来源：http://aat.sxryk.cn

constexpr int N = 10;
来源：http://khq.guowangkeji.top

[S58] C++：命名空间
来源：http://mno.feifeiyinyue.top

namespace ns { int f() { return 1; } }
来源：http://qlk.nanxuanxn.top

[S59] C++：静态断言
来源：http://ekg.yanxiufei.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gmy.uphjek.com

[S60] C++：遍历并删除元素
来源：http://apn.jyoumei.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ghz.snrcjt.cn

================================================================================
来源：http://ama.sjlbkw.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://otc.jinqigufen.top

================================================================================
来源：http://wyg.meibo888.top

[T01] Kotlin：Hello World
来源：http://wdp.quarkkingdee.top

println("Hello")
来源：http://rco.sxryk.cn

[T02] Kotlin：变量
来源：http://wqj.xuanzx.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://let.dianchejie.cn

[T03] Kotlin：字符串模板
来源：http://ded.cqqwz.cn

"值: $b"
来源：http://ruh.gaohongyu789.top

[T04] Kotlin：空安全
来源：http://ndf.hammf.cn

val n: String? = null;  n?.length
来源：http://ttp.shzxlz.cn

[T05] Kotlin：when 表达式
来源：http://rlx.yj202588.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bal.dianchejie.cn

[T06] Kotlin：集合映射
来源：http://kmh.jianghu66.top

listOf(1, 2, 3).map { it * 2 }
来源：http://djg.ivvv.top

[T07] Kotlin：集合过滤
来源：http://pxi.zhijiandao.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://clf.haohaochexian.top

[T08] Kotlin：数据类
来源：http://euj.shanyushiyangkeji.top

data class User(val name: String, val age: Int)
来源：http://xrt.sjlbkw.cn

[T09] Kotlin：扩展函数
来源：http://wsw.guannengcc.top

fun String.exclaim() = this + "!"
来源：http://bho.yangfankeji.com

[T10] Kotlin：默认参数
来源：http://kbz.shanyushiyangkeji.top

fun greet(name: String = "World") = "Hi $name"
来源：http://wwd.fanxiaobao.xyz

[T11] Kotlin：协程
来源：http://qza.pengpengdd.cyou

GlobalScope.launch { delay(1000); println("done") }
来源：http://cdq.zhixingplan.top

[T12] Kotlin：解构声明
来源：http://pgr.yuxming.cn

val (a, b) = Pair(1, 2)
来源：http://rlu.hesvh.cn

[T13] Kotlin：只读 Map
来源：http://vnm.bbcook.cn

val m = mapOf("a" to 1)
来源：http://suo.jyoumei.cn

[T14] Kotlin：循环
来源：http://wuz.tian-w.cn

for (i in 1..10) println(i)
来源：http://opm.xylfe.cn

[T15] Kotlin：接口
来源：http://scg.yj20258888.top

interface Shape { fun area(): Double }
来源：http://mma.yj20258.top

[T16] Swift：Hello World
来源：http://nfq.zhixingplan.top

print("Hello")
来源：http://xgh.fktsv.cn

[T17] Swift：变量与常量
来源：http://llo.jinghuilouyu.cn

var a = 1;  let b = 2
来源：http://pbt.birdmap.top

[T18] Swift：字符串插值
来源：http://tye.zhengqikj.top

"值: \(b)"
来源：http://uec.zhijiandao.cn

[T19] Swift：可选绑定
来源：http://vsk.fktsv.cn

if let n = opt { print(n) }
来源：http://sjd.dianchejie.cn

[T20] Swift：数组操作
来源：http://ime.nanxinkj.top

var a = [1, 2, 3];  a.append(4)
来源：http://ymj.smart0.xyz

[T21] Swift：遍历
来源：http://ikh.yj20258.top

for x in a { print(x) }
来源：http://bng.jiagoushi.top

[T22] Swift：字典
来源：http://itu.hnqzz.top

var d = ["a": 1];  d["b"] = 2
来源：http://mwi.chenjidiqi.icu

[T23] Swift：函数
来源：http://ixw.bjfxy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kvx.yangfankeji.com

[T24] Swift：闭包
来源：http://twp.ppjwa.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://apm.zhaomingkeji.xyz

[T25] Swift：结构体
来源：http://dwm.ppjwa.cn

struct P { var x: Int }
来源：http://jmn.ctjpmb.com

[T26] Swift：类与重写
来源：http://rkw.xuanzx.com

class A: Base { override func f() {} }
来源：http://mwr.nanxinkj.top

[T27] Swift：错误处理
来源：http://jbm.chenlongwang.top

do { try f() } catch { print(error) }
来源：http://ckh.hnxiangtu.top

[T28] Swift：枚举
来源：http://esc.pycfn.com

enum Color { case red, green }
来源：http://eur.xziqi.cn

[T29] Swift：guard 提前返回
来源：http://iwn.zhiwuduotai.top

guard let x = opt else { return }
来源：http://tpg.ehwqpu.com

[T30] Swift：协议
来源：http://gaz.jiagoushi.top

protocol Shape { func area() -> Double }
来源：http://fot.sysykeji.top

[T31] Lua：Hello World
来源：http://hmd.fengsongda.top

print("Hello")
来源：http://ydy.xziqi.cn

[T32] Lua：局部变量
来源：http://dve.shanyushiyangtech.top

local a = 1
来源：http://vzi.haohaochexian.top

[T33] Lua：表（数组）
来源：http://tde.wangdashe.top

local t = {1, 2, 3};  t[4] = 4
来源：http://pde.9152youxi.cn

[T34] Lua：遍历表
来源：http://ewq.quarkkingdee.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ilk.chenjidiqi.icu

[T35] Lua：字典表
来源：http://xxn.yonumen.top

local d = { a = 1 };  d.b = 2
来源：http://izk.iojbl.cn

[T36] Lua：函数
来源：http://sxx.haohaochexian.top

function add(a, b) return a + b end
来源：http://oyr.zhengqikj.top

[T37] Lua：字符串拼接
来源：http://rcz.xylfe.cn

"a" .. "b"
来源：http://ckh.9152youxi.cn

[T38] Lua：条件
来源：http://ypd.hysaishi.cn

if x > 0 then print("正") end
来源：http://oix.nanxuanxn.top

[T39] Lua：模式匹配
来源：http://mxj.shzxlz.cn

string.find(s, "%d+")
来源：http://llx.jqgufenzy.top

[T40] Lua：元表
来源：http://oqi.jlsjyb.cn

setmetatable({}, { __index = base })
来源：http://nta.hcnkem.com

[T41] Perl：Hello World
来源：http://ezs.zdbjq.cn

print "Hello\n";
来源：http://ahp.yfazqb.com

[T42] Perl：变量类型
来源：http://ine.dianchejie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wul.yj202588.top

[T43] Perl：字符串插值
来源：http://clk.yj202588.top

"值: $a"
来源：http://rhl.jianghu66.top

[T44] Perl：条件
来源：http://bes.ctjpmb.com

if ($a > 0) { print "正"; }
来源：http://jhg.9152youxi.cn

[T45] Perl：数组遍历
来源：http://pzk.hammf.cn

for my $x (@arr) { print $x; }
来源：http://riv.xylfe.cn

[T46] Perl：哈希操作
来源：http://jmk.jinyuanbaomall.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ssn.fehbvm.com

[T47] Perl：正则捕获
来源：http://awo.ybcxt.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://xuo.gaohongyu789.top

[T48] Perl：正则替换
来源：http://wre.quarkkingdee.top

$s =~ s/old/new/g;
来源：http://dlk.zhiwuduotai.top

[T49] Perl：函数
来源：http://xqf.snrcjt.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://aff.gotoacloud.top

[T50] Perl：逐行读文件
来源：http://abx.kuanghao11.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://yuh.quarkkingdee.top

while (my $line = <$fh>) { print $line; }
来源：http://niy.c1oappe.top

[T51] Scala：Hello World
来源：http://oek.hcnkem.com

println("Hello")
来源：http://iym.daxiang520.top

[T52] Scala：变量
来源：http://brt.zhaomingkeji.xyz

val a = 1;  var b = 2
来源：http://euc.jianghu66.top

[T53] Scala：字符串插值
来源：http://jio.shuidangran.top

s"值: $b"
来源：http://mmv.hnqzz.top

[T54] Scala：集合映射
来源：http://tgw.ppjwa.cn

List(1, 2, 3).map(_ * 2)
来源：http://lvk.xuanzx.com

[T55] Scala：集合过滤
来源：http://ofp.52xcode.cn

List(1, 2, 3).filter(_ > 1)
来源：http://foi.yuanzhike.top

[T56] Scala：样例类
来源：http://haa.hnqzz.top

case class User(name: String, age: Int)
来源：http://ejz.wangshuangyany.cn

[T57] Scala：模式匹配
来源：http://ktl.ctjpmb.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://qhw.zycfv.cn

[T58] Scala：函数定义
来源：http://sjo.chenjidiqi.icu

def add(a: Int, b: Int): Int = a + b
来源：http://nhb.smart0.xyz

[T59] Scala：循环
来源：http://uhn.yvedp.cn

for (i <- 1 to 10) println(i)
来源：http://unm.guowangkeji.top

[T60] Scala：折叠
来源：http://sxx.quarkkingdee.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wyt.zhongyouzk.top

================================================================================
来源：http://lpp.shanyushiyangtech.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://leh.hesvh.cn

================================================================================
来源：http://nbz.hywenlv.cn

[U01] Py：创建虚拟环境
来源：http://nmf.yonumen.top

python -m venv .venv && source .venv/bin/activate
来源：http://jum.jinqigfzy.top

[U02] Py：导出 / 安装依赖
来源：http://ztj.ctjpmb.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cyx.chenlongwang.top

[U03] Py：加载 .env 配置
来源：http://tva.aizwys.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://wyg.hesvh.cn

[U04] Py：变量调试打印
来源：http://orr.jinyuanbaomall.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ggh.zhongyouzk.top

[U05] Py：列表去重且保序
来源：http://qcj.fanxiaobao.xyz

list(dict.fromkeys(arr))
来源：http://ozf.sjlbkw.cn

[U06] Py：合并两个字典
来源：http://bsi.tanke756.top

{**a, **b}
来源：http://lsp.xylfe.cn

[U07] Py：反转字典键值
来源：http://yko.shzxlz.cn

{v: k for k, v in d.items()}
来源：http://skz.xingfuxueyuan.xyz

[U08] Py：展平二维列表
来源：http://brw.xylfe.cn

[y for x in nested for y in x]
来源：http://lvb.nanxinkj.top

[U09] Py：字典取最大值的键
来源：http://utt.shangyingyoupin.top

max(d, key=d.get)
来源：http://ynd.smart0.xyz

[U10] Py：按值排序字典
来源：http://ymb.gaohongyu789.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wyw.yj20258.top

[U11] Py：生成器表达式
来源：http://yhc.316326.xyz

(x * 2 for x in arr)
来源：http://dwr.yuxming.cn

[U12] Py：取出现最多的 3 个元素
来源：http://mfe.52xcode.cn

Counter(arr).most_common(3)
来源：http://ngd.shzxlz.cn

[U13] Py：固定长度队列
来源：http://uly.bbcook.cn

deque(maxlen=10)
来源：http://sze.zhixingplan.top

[U14] Py：分组收集到列表
来源：http://ree.sysykeji.top

defaultdict(list)
来源：http://nci.zhoulong.xyz

[U15] Py：高精度计时
来源：http://odj.epnwcf.com

t = time.perf_counter()
来源：http://rlb.shzxlz.cn

[U16] Py：命令行参数解析
来源：http://ysf.nwbrower.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://tga.yuxming.cn

[U17] Py：初始化日志
来源：http://ijy.hammf.cn

logging.basicConfig(level=logging.INFO)
来源：http://hzf.bjfxy.top

[U18] Py：预编译正则
来源：http://yoz.sysykeji.top

pat = re.compile(r"\d+")
来源：http://nrt.52xcode.cn

[U19] Py：正则替换带回调
来源：http://svt.yj20258.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lyu.dashuyun.cn

[U20] Py：缓存函数结果
来源：http://sdr.pycfn.com

@functools.lru_cache(maxsize=None)
来源：http://vbu.iojbl.cn

[U21] Py：自定义上下文管理器
来源：http://mtc.ctjpmb.com

@contextlib.contextmanager
来源：http://ova.sysykeji.top

[U22] Py：矩阵转置
来源：http://yck.tianlin.xyz

list(zip(*m))
来源：http://ooy.52xcode.cn

[U23] Py：分块读取大文件
来源：http://oud.sysykeji.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pcn.zhixingplan.top

[U24] Py：路径操作
来源：http://tnv.vehdjk.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jhh.0kj1m.cn

[U25] Py：CSV 按字典读
来源：http://lxt.cucudq.cn

csv.DictReader(f)
来源：http://svy.meibo888.top

[U26] Py：并发下载
来源：http://fpd.smart0.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hyw.yangfankeji.com

[U27] Py：异步 HTTP
来源：http://nnj.ppjwa.cn

aiohttp.ClientSession() 配合 async with
来源：http://hmp.zhongyouzk.top

[U28] Py：类型别名
来源：http://gjq.tarul.cn

UserId = int
来源：http://lxo.316326.xyz

[U29] Py：属性校验
来源：http://dhu.zhoulong.xyz

@property 与 @x.setter 配合
来源：http://vpa.xinyue.icu

[U30] Py：数据类
来源：http://jdd.dianchejie.cn

@dataclass(slots=True)
来源：http://pef.nwbrower.top

[U31] Py：单测
来源：http://csa.0kj1m.cn

python -m pytest -q
来源：http://jkr.sjlbkw.cn

[U32] Py：代码格式化
来源：http://nna.52xcode.cn

ruff format . && ruff check --fix .
来源：http://syk.yanxiufei.cn

[U33] Py：打包发布
来源：http://jbk.jyoumei.cn

python -m build  （依赖 pyproject.toml）
来源：http://lei.meibo888.top

[U34] Py：判断编码
来源：http://fkz.nwbrower.top

chardet.detect(raw)
来源：http://pdm.xziqi.cn

[U35] Py：发送邮件
来源：http://iyc.yonumen.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://egn.shanyushiyangkeji.top

[U36] Py：定时任务
来源：http://mzj.iojbl.cn

schedule.every(10).minutes.do(job)
来源：http://yeu.52xcode.cn

[U37] Py：读写 Excel
来源：http://jze.xinyue.icu

pandas.read_excel / DataFrame.to_excel
来源：http://yww.yuxming.cn

[U38] Py：获取脚本所在目录
来源：http://wjt.yongpay.top

Path(__file__).resolve().parent
来源：http://fcu.sysykeji.top

[U39] Py：判断是否在交互环境
来源：http://qtc.0kj1m.cn

sys.stdout.isatty()
来源：http://won.yj20258888.top

[U40] Py：打印到标准错误
来源：http://dak.hysaishi.cn

print("err", file=sys.stderr)
来源：http://bwj.havefunace.top

[U41] PHP：初始化 Composer 项目
来源：http://abq.gotoacloud.top

composer init;  composer require guzzlehttp/guzzle
来源：http://txh.vehdjk.com

[U42] PHP：PSR-4 自动加载
来源：http://uns.xingfuxueyuan.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bap.wangdashe.top

[U43] PHP：声明命名空间
来源：http://hkc.zdqjudy.top

namespace App\Http;
来源：http://xah.mhx1999.top

[U44] PHP：开启严格类型
来源：http://jnt.jinghuilouyu.cn

declare(strict_types=1);
来源：http://haz.sysykeji.top


<!-- 参考信息 -->