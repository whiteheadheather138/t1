代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qpw.birdmap.top

[S25] C：内存拷贝
来源：http://mrm.yj202588.top

memcpy(dst, src, n);
来源：http://sfy.fzhhl.top

[S26] C：内存清零
来源：http://itr.redwolf501.top

memset(a, 0, sizeof a);
来源：http://unk.yuxming.cn

[S27] C：定义常量
来源：http://fpj.guannengcc.top

const double PI = 3.14159;
来源：http://ofv.wangshuangyany.cn

[S28] C：静态变量
来源：http://tvc.cashguo.top

static int counter = 0;
来源：http://beb.shangyingyoupin.top

[S29] C：变参函数
来源：http://txk.shzxlz.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rzr.jqgufenzy.top

[S30] C：头文件保护
来源：http://tcu.sjlbkw.cn

#ifndef X_H
来源：http://arp.shangyingyoupin.top

#define X_H
来源：http://boo.dashuyun.cn

#endif
来源：http://mkc.haohaochexian.top

[S31] C++：Hello World
来源：http://qxi.yuanzhike.top

#include <iostream>
来源：http://vou.hongshengwenyu.top

int main() { std::cout << "Hello\n"; }
来源：http://qvb.pengpengdd.cyou

[S32] C++：字符串
来源：http://vld.shangyingyoupin.top

std::string s = "hi";  s += "!";
来源：http://bss.nanxuanxn.top

[S33] C++：vector 增删
来源：http://vli.zdbjq.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ecn.jinqigfzy.top

[S34] C++：遍历 vector
来源：http://sxo.yuxming.cn

for (auto &x : v) { std::cout << x; }
来源：http://ews.jqgfzy.top

[S35] C++：map
来源：http://yzd.jinqigufen.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://aei.ivvv.top

[S36] C++：unordered_map
来源：http://xih.cheryme.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tnz.redwolf501.top

[S37] C++：set
来源：http://hvn.52xcode.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ngs.tanke756.top

[S38] C++：排序
来源：http://jtg.xingfuxueyuan.xyz

std::sort(v.begin(), v.end());
来源：http://tyl.hesvh.cn

[S39] C++：自定义比较器排序
来源：http://xdq.yonumen.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wpo.vehdjk.com

[S40] C++：查找元素
来源：http://oyi.xylfe.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yrk.aibaodan.cn

[S41] C++：类与构造函数
来源：http://zfn.0kj1m.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://igg.yj20258888.top

[S42] C++：继承与虚函数
来源：http://lvi.xylfe.cn

class B : public Base { public: void f() override {} };
来源：http://obv.zdqjudy.top

[S43] C++：智能指针
来源：http://wig.vqdsnc.cn

auto p = std::make_unique<int>(5);
来源：http://tbj.tian-w.cn

[S44] C++：引用传参
来源：http://kiv.ywan-chungtsiang.top

void inc(int &x) { ++x; }
来源：http://sfv.tanke756.top

[S45] C++：lambda
来源：http://qtq.shangyingyoupin.top

auto add = [](int a, int b) { return a + b; };
来源：http://qrx.ehwqpu.com

[S46] C++：函数模板
来源：http://rkz.yuxming.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sdh.nwbrower.top

[S47] C++：结构化绑定遍历
来源：http://vvb.cucudq.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rzy.jinyuanbaomall.cn

[S48] C++：逐行读文件
来源：http://ssz.yanxiufei.cn

std::ifstream in("a.txt");  std::string line;
来源：http://mfr.aibaodan.cn

while (std::getline(in, line)) { }
来源：http://xna.xylfe.cn

[S49] C++：写文件
来源：http://wtr.bjfxy.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hrq.jqgufenzy.top

[S50] C++：格式化数字
来源：http://ecn.shuidangran.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dqd.zdqjudy.top

[S51] C++：显式类型转换
来源：http://wvj.nanxuanxn.top

static_cast<double>(a) / b
来源：http://zxz.yj20258888.top

[S52] C++：const 与 noexcept
来源：http://xyt.cdnleiting.top

int size() const noexcept { return n_; }
来源：http://cuc.hongshengwenyu.top

[S53] C++：移动语义
来源：http://wku.wangshuangyany.cn

std::vector<int> w = std::move(v);
来源：http://wvv.epnwcf.com

[S54] C++：异常处理
来源：http://osh.pycfn.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zsx.zdbjq.cn

[S55] C++：结构化绑定
来源：http://tkc.yueranfly.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ryj.yj20258888.top

[S56] C++：optional
来源：http://uqx.havefunace.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kov.hnqzz.top

[S57] C++：编译期常量
来源：http://bsr.hcnkem.com

constexpr int N = 10;
来源：http://erw.hysaishi.cn

[S58] C++：命名空间
来源：http://poa.guannengcc.top

namespace ns { int f() { return 1; } }
来源：http://dvm.svipenyu.cn

[S59] C++：静态断言
来源：http://irv.fktsv.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ark.52xcode.cn

[S60] C++：遍历并删除元素
来源：http://cmu.zhaomingkeji.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qzu.ybcxt.top

================================================================================
来源：http://aph.zdbjq.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hxj.ehwqpu.com

================================================================================
来源：http://xde.zhiwuduotai.top

[T01] Kotlin：Hello World
来源：http://xfl.hywenlv.cn

println("Hello")
来源：http://lkn.iojbl.cn

[T02] Kotlin：变量
来源：http://cwd.ivvv.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ife.9152youxi.cn

[T03] Kotlin：字符串模板
来源：http://cgi.cheryme.top

"值: $b"
来源：http://aow.tian-w.cn

[T04] Kotlin：空安全
来源：http://bxj.vehdjk.com

val n: String? = null;  n?.length
来源：http://mal.xuetiantiany.cn

[T05] Kotlin：when 表达式
来源：http://mfd.jqgfzy.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uzt.gzhubu.top

[T06] Kotlin：集合映射
来源：http://feh.0kj1m.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ggk.chenzaomai.com

[T07] Kotlin：集合过滤
来源：http://epn.9152youxi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://fcs.dashuyun.cn

[T08] Kotlin：数据类
来源：http://rsy.nanxinkj.top

data class User(val name: String, val age: Int)
来源：http://bzo.chenzaomai.com

[T09] Kotlin：扩展函数
来源：http://gmz.zhiwuduotai.top

fun String.exclaim() = this + "!"
来源：http://dcp.cucudq.cn

[T10] Kotlin：默认参数
来源：http://lcv.wangshuangyany.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://fev.ydzc1.top

[T11] Kotlin：协程
来源：http://mki.jianghu66.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://luj.hnqzz.top

[T12] Kotlin：解构声明
来源：http://hva.ywan-chungtsiang.top

val (a, b) = Pair(1, 2)
来源：http://ghe.hysaishi.cn

[T13] Kotlin：只读 Map
来源：http://ncz.chenjidiqi.icu

val m = mapOf("a" to 1)
来源：http://foq.chenjidiqi.icu

[T14] Kotlin：循环
来源：http://tzs.daria6918.cn

for (i in 1..10) println(i)
来源：http://sxz.redwolf501.top

[T15] Kotlin：接口
来源：http://oew.chenzaomai.com

interface Shape { fun area(): Double }
来源：http://luu.ivvv.top

[T16] Swift：Hello World
来源：http://rzw.cucudq.cn

print("Hello")
来源：http://lfu.hammf.cn

[T17] Swift：变量与常量
来源：http://dmo.9152youxi.cn

var a = 1;  let b = 2
来源：http://npt.yuanzhike.top

[T18] Swift：字符串插值
来源：http://ldw.andypj.xyz

"值: \(b)"
来源：http://zci.xinyue.icu

[T19] Swift：可选绑定
来源：http://vcb.pengpengdd.cyou

if let n = opt { print(n) }
来源：http://ufo.epnwcf.com

[T20] Swift：数组操作
来源：http://kdo.316326.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://pns.jinqigufen.top

[T21] Swift：遍历
来源：http://rwg.jinyuanbaomall.cn

for x in a { print(x) }
来源：http://tep.jlsjyb.cn

[T22] Swift：字典
来源：http://edz.fzhhl.top

var d = ["a": 1];  d["b"] = 2
来源：http://fth.cdnleiting.top

[T23] Swift：函数
来源：http://ncy.ydzc1.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rpi.sweek.top

[T24] Swift：闭包
来源：http://kby.quarkkingdee.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://pan.fzhhl.top

[T25] Swift：结构体
来源：http://kyg.yj20258.top

struct P { var x: Int }
来源：http://rde.yuanzhike.top

[T26] Swift：类与重写
来源：http://wwa.guannengcc.top

class A: Base { override func f() {} }
来源：http://agu.ywan-chungtsiang.top

[T27] Swift：错误处理
来源：http://oid.fanxiaobao.xyz

do { try f() } catch { print(error) }
来源：http://bty.ydzc1.top

[T28] Swift：枚举
来源：http://bnw.quarkkingdee.top

enum Color { case red, green }
来源：http://sap.zhijiandao.cn

[T29] Swift：guard 提前返回
来源：http://bus.ywan-chungtsiang.top

guard let x = opt else { return }
来源：http://jse.jiagoushi.top

[T30] Swift：协议
来源：http://mvu.quarkkingdee.top

protocol Shape { func area() -> Double }
来源：http://tps.shuidangran.top

[T31] Lua：Hello World
来源：http://cig.sxryk.cn

print("Hello")
来源：http://ogm.ybcxt.top

[T32] Lua：局部变量
来源：http://ccp.xuetiantiany.cn

local a = 1
来源：http://hjw.jinghuilouyu.cn

[T33] Lua：表（数组）
来源：http://lwe.dianchejie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://jwr.zhoulong.xyz

[T34] Lua：遍历表
来源：http://ool.hesvh.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://lvg.cucudq.cn

[T35] Lua：字典表
来源：http://svf.ivvv.top

local d = { a = 1 };  d.b = 2
来源：http://bqh.iojbl.cn

[T36] Lua：函数
来源：http://kuf.iojbl.cn

function add(a, b) return a + b end
来源：http://isx.ctjpmb.com

[T37] Lua：字符串拼接
来源：http://lkb.kuanghao11.cn

"a" .. "b"
来源：http://lpt.uphjek.com

[T38] Lua：条件
来源：http://uar.sxryk.cn

if x > 0 then print("正") end
来源：http://ygw.snrcjt.cn

[T39] Lua：模式匹配
来源：http://woc.nwbrower.top

string.find(s, "%d+")
来源：http://ncf.fzhhl.top

[T40] Lua：元表
来源：http://vev.yuxming.cn

setmetatable({}, { __index = base })
来源：http://fpy.zhengqikj.top

[T41] Perl：Hello World
来源：http://jnb.52xcode.cn

print "Hello\n";
来源：http://ocd.chenjidiqi.icu

[T42] Perl：变量类型
来源：http://jyn.chenzaomai.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xyj.xylfe.cn

[T43] Perl：字符串插值
来源：http://snc.meibo888.top

"值: $a"
来源：http://zun.zhiwuduotai.top

[T44] Perl：条件
来源：http://rry.zhengqikj.top

if ($a > 0) { print "正"; }
来源：http://lhh.xuanzx.com

[T45] Perl：数组遍历
来源：http://xpf.daria6918.cn

for my $x (@arr) { print $x; }
来源：http://apj.redwolf501.top

[T46] Perl：哈希操作
来源：http://zci.ybcxt.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tlu.smart0.xyz

[T47] Perl：正则捕获
来源：http://mgz.svipenyu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://gla.wangdashe.top

[T48] Perl：正则替换
来源：http://guy.svipenyu.cn

$s =~ s/old/new/g;
来源：http://mjz.zycfv.cn

[T49] Perl：函数
来源：http://nqx.hammf.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rzd.yj20258.top

[T50] Perl：逐行读文件
来源：http://lab.yuxming.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qan.ybcxt.top

while (my $line = <$fh>) { print $line; }
来源：http://tkt.yangfankeji.com

[T51] Scala：Hello World
来源：http://wtf.c1oappe.top

println("Hello")
来源：http://bwx.ctjpmb.com

[T52] Scala：变量
来源：http://dww.gaohongyu789.top

val a = 1;  var b = 2
来源：http://jqq.shanyushiyangtech.top

[T53] Scala：字符串插值
来源：http://puh.hysaishi.cn

s"值: $b"
来源：http://heg.jinghuilouyu.cn

[T54] Scala：集合映射
来源：http://myu.yuanzhike.top

List(1, 2, 3).map(_ * 2)
来源：http://xct.jinqigfzy.top

[T55] Scala：集合过滤
来源：http://fvs.jiagoushi.top

List(1, 2, 3).filter(_ > 1)
来源：http://wkj.sweek.top

[T56] Scala：样例类
来源：http://rek.zdqjudy.top

case class User(name: String, age: Int)
来源：http://wln.hesvh.cn

[T57] Scala：模式匹配
来源：http://jdy.zhiwuduotai.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://lns.fehbvm.com

[T58] Scala：函数定义
来源：http://atl.havefunace.top

def add(a: Int, b: Int): Int = a + b
来源：http://imn.andypj.xyz

[T59] Scala：循环
来源：http://hai.xuetiantiany.cn

for (i <- 1 to 10) println(i)
来源：http://tzd.zhixingplan.top

[T60] Scala：折叠
来源：http://iil.yvedp.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cfs.gzhubu.top

================================================================================
来源：http://pln.xingfuxueyuan.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://iod.fktsv.cn

================================================================================
来源：http://lgi.aibaodan.cn

[U01] Py：创建虚拟环境
来源：http://boq.yongpay.top

python -m venv .venv && source .venv/bin/activate
来源：http://fsj.cucudq.cn

[U02] Py：导出 / 安装依赖
来源：http://iab.birdmap.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nxu.sxryk.cn

[U03] Py：加载 .env 配置
来源：http://tuv.pengpengdd.cyou

from dotenv import load_dotenv; load_dotenv()
来源：http://awq.xuetiantiany.cn

[U04] Py：变量调试打印
来源：http://lgt.zdbjq.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://tzp.xuetiantiany.cn

[U05] Py：列表去重且保序
来源：http://ejq.zhongyouzk.top

list(dict.fromkeys(arr))
来源：http://wfq.jinqigfzy.top

[U06] Py：合并两个字典
来源：http://yvs.cdnleiting.top

{**a, **b}
来源：http://kfy.yj202588.top

[U07] Py：反转字典键值
来源：http://cvn.316326.xyz

{v: k for k, v in d.items()}
来源：http://scv.daria6918.cn

[U08] Py：展平二维列表
来源：http://zcy.jinqigufen.top

[y for x in nested for y in x]
来源：http://nvc.chenjidiqi.icu

[U09] Py：字典取最大值的键
来源：http://lap.vqdsnc.cn

max(d, key=d.get)
来源：http://lit.fehbvm.com

[U10] Py：按值排序字典
来源：http://zhm.hesvh.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hmz.vqdsnc.cn

[U11] Py：生成器表达式
来源：http://txo.cdnleiting.top

(x * 2 for x in arr)
来源：http://sps.sjlbkw.cn

[U12] Py：取出现最多的 3 个元素
来源：http://aeg.ydjk.org.cn

Counter(arr).most_common(3)
来源：http://hto.jinghuilouyu.cn

[U13] Py：固定长度队列
来源：http://wsh.yuxming.cn

deque(maxlen=10)
来源：http://ulb.guannengcc.top

[U14] Py：分组收集到列表
来源：http://qwv.nanxinkj.top

defaultdict(list)
来源：http://wwe.svipenyu.cn

[U15] Py：高精度计时
来源：http://lov.yj20258.top

t = time.perf_counter()
来源：http://eyo.hywenlv.cn

[U16] Py：命令行参数解析
来源：http://fii.pycfn.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hem.fanxiaobao.xyz

[U17] Py：初始化日志
来源：http://djj.vqdsnc.cn

logging.basicConfig(level=logging.INFO)
来源：http://fmu.aizwys.cn

[U18] Py：预编译正则
来源：http://ewt.shangyingyoupin.top

pat = re.compile(r"\d+")
来源：http://oln.zhijiandao.cn

[U19] Py：正则替换带回调
来源：http://oos.uphjek.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fmw.gaohongyu789.top

[U20] Py：缓存函数结果
来源：http://mtc.nwbrower.top

@functools.lru_cache(maxsize=None)
来源：http://qqe.yj202588.top

[U21] Py：自定义上下文管理器
来源：http://utg.havefunace.top

@contextlib.contextmanager
来源：http://xig.hywenlv.cn

[U22] Py：矩阵转置
来源：http://eaq.zhijiandao.cn

list(zip(*m))
来源：http://aen.sxryk.cn

[U23] Py：分块读取大文件
来源：http://uww.havefunace.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fto.zhiwuduotai.top

[U24] Py：路径操作
来源：http://dqt.dashuyun.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://quy.epnwcf.com

[U25] Py：CSV 按字典读
来源：http://bbg.ehwqpu.com

csv.DictReader(f)
来源：http://fkj.zhiwuduotai.top

[U26] Py：并发下载
来源：http://jzi.ybcxt.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ysg.shanyushiyangkeji.top

[U27] Py：异步 HTTP
来源：http://eqx.yfazqb.com

aiohttp.ClientSession() 配合 async with
来源：http://onf.xingfuxueyuan.xyz

[U28] Py：类型别名
来源：http://fhe.yongpay.top

UserId = int
来源：http://brb.daria6918.cn

[U29] Py：属性校验
来源：http://fra.fzhhl.top

@property 与 @x.setter 配合
来源：http://hud.kuanghao11.cn

[U30] Py：数据类
来源：http://hlk.gaohongyu789.top

@dataclass(slots=True)
来源：http://wzp.svipenyu.cn

[U31] Py：单测
来源：http://auy.xinyue.icu

python -m pytest -q
来源：http://ddn.zycfv.cn

[U32] Py：代码格式化
来源：http://ubz.tianlin.xyz

ruff format . && ruff check --fix .
来源：http://pza.xuetiantiany.cn

[U33] Py：打包发布
来源：http://oft.vehdjk.com

python -m build  （依赖 pyproject.toml）
来源：http://qqi.fanxiaobao.xyz

[U34] Py：判断编码
来源：http://kpe.vqdsnc.cn

chardet.detect(raw)
来源：http://ymx.hcnkem.com

[U35] Py：发送邮件
来源：http://osq.mhx1999.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hjf.shangyingyoupin.top

[U36] Py：定时任务
来源：http://pdj.ivvv.top

schedule.every(10).minutes.do(job)
来源：http://akr.ydzc1.top

[U37] Py：读写 Excel
来源：http://elr.kuanghao11.cn

pandas.read_excel / DataFrame.to_excel
来源：http://qex.316326.xyz

[U38] Py：获取脚本所在目录
来源：http://hoo.nwbrower.top

Path(__file__).resolve().parent
来源：http://fwt.ctjpmb.com

[U39] Py：判断是否在交互环境
来源：http://umz.yj20258888.top

sys.stdout.isatty()
来源：http://els.meibo888.top

[U40] Py：打印到标准错误
来源：http://jiw.tarul.cn

print("err", file=sys.stderr)
来源：http://nrt.zhixingplan.top

[U41] PHP：初始化 Composer 项目
来源：http://oqd.316326.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://lit.gaohongyu789.top

[U42] PHP：PSR-4 自动加载
来源：http://flo.vqdsnc.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tjw.nanxinkj.top

[U43] PHP：声明命名空间
来源：http://dxd.hnxiangtu.top

namespace App\Http;
来源：http://lff.chenlongwang.top

[U44] PHP：开启严格类型
来源：http://efp.ywan-chungtsiang.top

declare(strict_types=1);
来源：http://qzq.aizwys.cn

[U45] PHP：类型声明与返回类型
来源：http://xvz.tianlin.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://nvx.zhengqikj.top

[U46] PHP：可空类型
来源：http://hmu.sysykeji.top

?string $name = null
来源：http://hmi.shuidangran.top

[U47] PHP：联合类型
来源：http://rlv.zhoulong.xyz

int|string $id
来源：http://rft.daxiang520.top

[U48] PHP：纯枚举
来源：http://ubq.iojbl.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://shx.xinyue.icu


<!-- 参考信息 -->