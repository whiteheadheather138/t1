代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kyq.jqgfzy.top

[S25] C：内存拷贝
来源：http://rnz.jqgfzy.top

memcpy(dst, src, n);
来源：http://vvo.andypj.xyz

[S26] C：内存清零
来源：http://apo.zdqjudy.top

memset(a, 0, sizeof a);
来源：http://ins.ctjpmb.com

[S27] C：定义常量
来源：http://azm.316326.xyz

const double PI = 3.14159;
来源：http://qez.mhx1999.top

[S28] C：静态变量
来源：http://wre.zhongyouzk.top

static int counter = 0;
来源：http://hgq.cqqwz.cn

[S29] C：变参函数
来源：http://rus.wangshuangyany.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ktn.chenjidiqi.icu

[S30] C：头文件保护
来源：http://rms.fzhhl.top

#ifndef X_H
来源：http://fhc.wangdashe.top

#define X_H
来源：http://ksc.yonumen.top

#endif
来源：http://arm.yuxming.cn

[S31] C++：Hello World
来源：http://itc.shuidangran.top

#include <iostream>
来源：http://gah.yj20258.top

int main() { std::cout << "Hello\n"; }
来源：http://cqs.vqdsnc.cn

[S32] C++：字符串
来源：http://gry.yangfankeji.com

std::string s = "hi";  s += "!";
来源：http://sph.yongpay.top

[S33] C++：vector 增删
来源：http://vzs.xuanzx.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wuw.tanke756.top

[S34] C++：遍历 vector
来源：http://kkb.c1oappe.top

for (auto &x : v) { std::cout << x; }
来源：http://fjx.yangfankeji.com

[S35] C++：map
来源：http://uru.pycfn.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://urj.ivvv.top

[S36] C++：unordered_map
来源：http://pto.jinyuanbaomall.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://esu.ybcxt.top

[S37] C++：set
来源：http://fxq.shanyushiyangkeji.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://akr.jinghuilouyu.cn

[S38] C++：排序
来源：http://gjm.birdmap.top

std::sort(v.begin(), v.end());
来源：http://vyd.jinghuilouyu.cn

[S39] C++：自定义比较器排序
来源：http://dka.chenlongwang.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hit.cucudq.cn

[S40] C++：查找元素
来源：http://vui.shangyingyoupin.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rfk.chenjidiqi.icu

[S41] C++：类与构造函数
来源：http://yrv.cheryme.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ili.yj202588.top

[S42] C++：继承与虚函数
来源：http://dum.pengpengdd.cyou

class B : public Base { public: void f() override {} };
来源：http://kwo.hysaishi.cn

[S43] C++：智能指针
来源：http://rms.snrcjt.cn

auto p = std::make_unique<int>(5);
来源：http://nku.ctjpmb.com

[S44] C++：引用传参
来源：http://jsx.cheryme.top

void inc(int &x) { ++x; }
来源：http://nnu.shuidangran.top

[S45] C++：lambda
来源：http://lph.redwolf501.top

auto add = [](int a, int b) { return a + b; };
来源：http://aei.zdqjudy.top

[S46] C++：函数模板
来源：http://siy.gaohongyu789.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lpg.tanke756.top

[S47] C++：结构化绑定遍历
来源：http://fmc.yonumen.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://etj.jiagoushi.top

[S48] C++：逐行读文件
来源：http://byj.316326.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://ffi.cashguo.top

while (std::getline(in, line)) { }
来源：http://mmo.hongshengwenyu.top

[S49] C++：写文件
来源：http://agc.sweek.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xuz.jinqigufen.top

[S50] C++：格式化数字
来源：http://jem.uphjek.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jqa.fanxiaobao.xyz

[S51] C++：显式类型转换
来源：http://uha.shzxlz.cn

static_cast<double>(a) / b
来源：http://vle.ctjpmb.com

[S52] C++：const 与 noexcept
来源：http://kpr.jinqigufen.top

int size() const noexcept { return n_; }
来源：http://gjv.haohaochexian.top

[S53] C++：移动语义
来源：http://ncg.zdbjq.cn

std::vector<int> w = std::move(v);
来源：http://bwj.tarul.cn

[S54] C++：异常处理
来源：http://iwn.jqgfzy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://emf.zycfv.cn

[S55] C++：结构化绑定
来源：http://urs.gzhubu.top

auto [a, b] = std::make_pair(1, 2);
来源：http://keb.sweek.top

[S56] C++：optional
来源：http://jof.zhaomingkeji.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tfc.zhixingplan.top

[S57] C++：编译期常量
来源：http://plr.xylfe.cn

constexpr int N = 10;
来源：http://ifv.xingfuxueyuan.xyz

[S58] C++：命名空间
来源：http://oxj.ehwqpu.com

namespace ns { int f() { return 1; } }
来源：http://vpk.ivvv.top

[S59] C++：静态断言
来源：http://yxl.c1oappe.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wsm.gogol.net.cn

[S60] C++：遍历并删除元素
来源：http://pez.shangyingyoupin.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hdp.tarul.cn

================================================================================
来源：http://jou.hfpthk.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rny.bjfxy.top

================================================================================
来源：http://azc.daxiang520.top

[T01] Kotlin：Hello World
来源：http://iqo.ehwqpu.com

println("Hello")
来源：http://fug.birdmap.top

[T02] Kotlin：变量
来源：http://zri.nwbrower.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yyr.yanxiufei.cn

[T03] Kotlin：字符串模板
来源：http://xia.wangshuangyany.cn

"值: $b"
来源：http://awz.shanyushiyangkeji.top

[T04] Kotlin：空安全
来源：http://ooz.iojbl.cn

val n: String? = null;  n?.length
来源：http://jjz.haohaochexian.top

[T05] Kotlin：when 表达式
来源：http://pmh.jianghu66.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bjb.tanke756.top

[T06] Kotlin：集合映射
来源：http://nke.guowangkeji.top

listOf(1, 2, 3).map { it * 2 }
来源：http://lbb.xinyue.icu

[T07] Kotlin：集合过滤
来源：http://dxo.yangfankeji.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://mwx.tianlin.xyz

[T08] Kotlin：数据类
来源：http://lrx.xinyue.icu

data class User(val name: String, val age: Int)
来源：http://tss.feifeiyinyue.top

[T09] Kotlin：扩展函数
来源：http://pcg.gogol.net.cn

fun String.exclaim() = this + "!"
来源：http://ome.hnqzz.top

[T10] Kotlin：默认参数
来源：http://lvj.yj202588.top

fun greet(name: String = "World") = "Hi $name"
来源：http://knp.yuanzhike.top

[T11] Kotlin：协程
来源：http://khc.fehbvm.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://jmh.hfpthk.cn

[T12] Kotlin：解构声明
来源：http://iqm.yj202588.top

val (a, b) = Pair(1, 2)
来源：http://zko.zdqjudy.top

[T13] Kotlin：只读 Map
来源：http://ewc.yueranfly.top

val m = mapOf("a" to 1)
来源：http://yzp.jiagoushi.top

[T14] Kotlin：循环
来源：http://nxo.xingfuxueyuan.xyz

for (i in 1..10) println(i)
来源：http://men.zhengqikj.top

[T15] Kotlin：接口
来源：http://ehu.yanxiufei.cn

interface Shape { fun area(): Double }
来源：http://mfs.zhengqikj.top

[T16] Swift：Hello World
来源：http://axu.tanke756.top

print("Hello")
来源：http://guh.zhoulong.xyz

[T17] Swift：变量与常量
来源：http://lkn.zhiwuduotai.top

var a = 1;  let b = 2
来源：http://fkk.gaohongyu789.top

[T18] Swift：字符串插值
来源：http://lxq.gogol.net.cn

"值: \(b)"
来源：http://gzz.hnxiangtu.top

[T19] Swift：可选绑定
来源：http://eyu.zdqjudy.top

if let n = opt { print(n) }
来源：http://muk.haohaochexian.top

[T20] Swift：数组操作
来源：http://tdc.redwolf501.top

var a = [1, 2, 3];  a.append(4)
来源：http://kfq.andypj.xyz

[T21] Swift：遍历
来源：http://rhw.cdnleiting.top

for x in a { print(x) }
来源：http://pcb.jinghuilouyu.cn

[T22] Swift：字典
来源：http://jro.zhengqikj.top

var d = ["a": 1];  d["b"] = 2
来源：http://cpc.fehbvm.com

[T23] Swift：函数
来源：http://xnf.chenlongwang.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://djg.xingfuxueyuan.xyz

[T24] Swift：闭包
来源：http://jcm.hnqzz.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://cun.pengpengdd.cyou

[T25] Swift：结构体
来源：http://beo.hnxiangtu.top

struct P { var x: Int }
来源：http://nuo.zhixingplan.top

[T26] Swift：类与重写
来源：http://rmz.quarkkingdee.top

class A: Base { override func f() {} }
来源：http://mjg.316326.xyz

[T27] Swift：错误处理
来源：http://hlm.meibo888.top

do { try f() } catch { print(error) }
来源：http://hzq.chenzaomai.com

[T28] Swift：枚举
来源：http://vdi.yanxiufei.cn

enum Color { case red, green }
来源：http://myo.tian-w.cn

[T29] Swift：guard 提前返回
来源：http://lgr.zhengqikj.top

guard let x = opt else { return }
来源：http://rye.yj20258.top

[T30] Swift：协议
来源：http://rug.cashguo.top

protocol Shape { func area() -> Double }
来源：http://qkh.cqqwz.cn

[T31] Lua：Hello World
来源：http://ibn.tarul.cn

print("Hello")
来源：http://lup.sysykeji.top

[T32] Lua：局部变量
来源：http://fkk.andypj.xyz

local a = 1
来源：http://sub.haohaochexian.top

[T33] Lua：表（数组）
来源：http://yqf.yueranfly.top

local t = {1, 2, 3};  t[4] = 4
来源：http://voy.tanke756.top

[T34] Lua：遍历表
来源：http://snt.bbcook.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://jco.svipenyu.cn

[T35] Lua：字典表
来源：http://zpv.nanxinkj.top

local d = { a = 1 };  d.b = 2
来源：http://zuh.shuidangran.top

[T36] Lua：函数
来源：http://cyv.daxiang520.top

function add(a, b) return a + b end
来源：http://ynh.iojbl.cn

[T37] Lua：字符串拼接
来源：http://shm.jinghuilouyu.cn

"a" .. "b"
来源：http://zef.feifeiyinyue.top

[T38] Lua：条件
来源：http://qwt.guannengcc.top

if x > 0 then print("正") end
来源：http://fdq.yongpay.top

[T39] Lua：模式匹配
来源：http://uus.yj20258.top

string.find(s, "%d+")
来源：http://kct.zdbjq.cn

[T40] Lua：元表
来源：http://elq.hfpthk.cn

setmetatable({}, { __index = base })
来源：http://bil.zhixingplan.top

[T41] Perl：Hello World
来源：http://syk.xuanzx.com

print "Hello\n";
来源：http://omx.yuanzhike.top

[T42] Perl：变量类型
来源：http://mbr.xuetiantiany.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://isa.yongpay.top

[T43] Perl：字符串插值
来源：http://kuq.sxryk.cn

"值: $a"
来源：http://znh.0kj1m.cn

[T44] Perl：条件
来源：http://zdv.ywan-chungtsiang.top

if ($a > 0) { print "正"; }
来源：http://lbk.xziqi.cn

[T45] Perl：数组遍历
来源：http://kjc.ybcxt.top

for my $x (@arr) { print $x; }
来源：http://gbn.cdnleiting.top

[T46] Perl：哈希操作
来源：http://kpg.vqdsnc.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tqy.shuidangran.top

[T47] Perl：正则捕获
来源：http://vwj.cucudq.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ujf.smart0.xyz

[T48] Perl：正则替换
来源：http://uix.hcnkem.com

$s =~ s/old/new/g;
来源：http://pio.daria6918.cn

[T49] Perl：函数
来源：http://gfi.gotoacloud.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://klf.birdmap.top

[T50] Perl：逐行读文件
来源：http://rou.xinyue.icu

open my $fh, "<", "a.txt" or die $!;
来源：http://qnb.hesvh.cn

while (my $line = <$fh>) { print $line; }
来源：http://jlc.andypj.xyz

[T51] Scala：Hello World
来源：http://xfx.nwbrower.top

println("Hello")
来源：http://qde.chenjidiqi.icu

[T52] Scala：变量
来源：http://qtb.yongpay.top

val a = 1;  var b = 2
来源：http://cmu.fzhhl.top

[T53] Scala：字符串插值
来源：http://aao.hfpthk.cn

s"值: $b"
来源：http://ojx.xuetiantiany.cn

[T54] Scala：集合映射
来源：http://fts.sxryk.cn

List(1, 2, 3).map(_ * 2)
来源：http://ygl.52xcode.cn

[T55] Scala：集合过滤
来源：http://orw.sweek.top

List(1, 2, 3).filter(_ > 1)
来源：http://rqn.fehbvm.com

[T56] Scala：样例类
来源：http://fps.hnqzz.top

case class User(name: String, age: Int)
来源：http://xns.yvedp.cn

[T57] Scala：模式匹配
来源：http://ixk.daria6918.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://gzw.nanxinkj.top

[T58] Scala：函数定义
来源：http://zgr.cdnleiting.top

def add(a: Int, b: Int): Int = a + b
来源：http://snz.jinqigfzy.top

[T59] Scala：循环
来源：http://xxk.aizwys.cn

for (i <- 1 to 10) println(i)
来源：http://vqh.52xcode.cn

[T60] Scala：折叠
来源：http://mxn.zdqjudy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wpm.ydjk.org.cn

================================================================================
来源：http://eqs.tian-w.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cgu.birdmap.top

================================================================================
来源：http://jju.xziqi.cn

[U01] Py：创建虚拟环境
来源：http://aeh.svipenyu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://aso.vehdjk.com

[U02] Py：导出 / 安装依赖
来源：http://sob.vehdjk.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jyj.gotoacloud.top

[U03] Py：加载 .env 配置
来源：http://elu.nanxinkj.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ryp.hammf.cn

[U04] Py：变量调试打印
来源：http://obp.hywenlv.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qzd.gotoacloud.top

[U05] Py：列表去重且保序
来源：http://ajv.fktsv.cn

list(dict.fromkeys(arr))
来源：http://jsn.jlsjyb.cn

[U06] Py：合并两个字典
来源：http://zvt.xziqi.cn

{**a, **b}
来源：http://ioc.cashguo.top

[U07] Py：反转字典键值
来源：http://kbo.sufxvd.cn

{v: k for k, v in d.items()}
来源：http://mhz.fengsongda.top

[U08] Py：展平二维列表
来源：http://ixb.yuxming.cn

[y for x in nested for y in x]
来源：http://scr.zycfv.cn

[U09] Py：字典取最大值的键
来源：http://usa.gogol.net.cn

max(d, key=d.get)
来源：http://xrs.vqdsnc.cn

[U10] Py：按值排序字典
来源：http://lyt.daria6918.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://apw.jiagoushi.top

[U11] Py：生成器表达式
来源：http://ibz.zhiwuduotai.top

(x * 2 for x in arr)
来源：http://fgg.jinyuanbaomall.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ggv.yj202588.top

Counter(arr).most_common(3)
来源：http://zlf.guannengcc.top

[U13] Py：固定长度队列
来源：http://tdz.wangshuangyany.cn

deque(maxlen=10)
来源：http://wrs.bjfxy.top

[U14] Py：分组收集到列表
来源：http://htg.wangdashe.top

defaultdict(list)
来源：http://hcf.zdqjudy.top

[U15] Py：高精度计时
来源：http://qya.havefunace.top

t = time.perf_counter()
来源：http://pdp.shanyushiyangtech.top

[U16] Py：命令行参数解析
来源：http://ouo.xingfuxueyuan.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nia.snrcjt.cn

[U17] Py：初始化日志
来源：http://eai.zhongyouzk.top

logging.basicConfig(level=logging.INFO)
来源：http://sgc.zycfv.cn

[U18] Py：预编译正则
来源：http://rkh.zhixingplan.top

pat = re.compile(r"\d+")
来源：http://vpr.yongpay.top

[U19] Py：正则替换带回调
来源：http://yie.yonumen.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nrx.smart0.xyz

[U20] Py：缓存函数结果
来源：http://qmq.hongshengwenyu.top

@functools.lru_cache(maxsize=None)
来源：http://mqg.ydzc1.top

[U21] Py：自定义上下文管理器
来源：http://qtk.jqgufenzy.top

@contextlib.contextmanager
来源：http://hak.fktsv.cn

[U22] Py：矩阵转置
来源：http://okk.yj20258.top

list(zip(*m))
来源：http://mtw.daria6918.cn

[U23] Py：分块读取大文件
来源：http://heb.52xcode.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qaz.zhongyouzk.top

[U24] Py：路径操作
来源：http://scm.xuetiantiany.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://iml.jinyuanbaomall.cn

[U25] Py：CSV 按字典读
来源：http://mjs.yuxming.cn

csv.DictReader(f)
来源：http://pgy.andypj.xyz

[U26] Py：并发下载
来源：http://mvy.jianghu66.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://him.sxryk.cn

[U27] Py：异步 HTTP
来源：http://fqw.tianlin.xyz

aiohttp.ClientSession() 配合 async with
来源：http://uot.xziqi.cn

[U28] Py：类型别名
来源：http://qeg.xziqi.cn

UserId = int
来源：http://jjp.jinqigufen.top

[U29] Py：属性校验
来源：http://jpa.ydjk.org.cn

@property 与 @x.setter 配合
来源：http://ubx.birdmap.top

[U30] Py：数据类
来源：http://ada.sxryk.cn

@dataclass(slots=True)
来源：http://ean.fengsongda.top

[U31] Py：单测
来源：http://dek.jinghuilouyu.cn

python -m pytest -q
来源：http://nhf.iojbl.cn

[U32] Py：代码格式化
来源：http://dhy.jinqigfzy.top

ruff format . && ruff check --fix .
来源：http://gcr.sysykeji.top

[U33] Py：打包发布
来源：http://keu.daxiang520.top

python -m build  （依赖 pyproject.toml）
来源：http://mzb.hysaishi.cn

[U34] Py：判断编码
来源：http://ebg.ivvv.top

chardet.detect(raw)
来源：http://apj.cheryme.top

[U35] Py：发送邮件
来源：http://wrz.gogol.net.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ajl.ydzc1.top

[U36] Py：定时任务
来源：http://dkw.zhongyouzk.top

schedule.every(10).minutes.do(job)
来源：http://bzi.wangshuangyany.cn

[U37] Py：读写 Excel
来源：http://gzo.dianchejie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://mig.shanyushiyangkeji.top

[U38] Py：获取脚本所在目录
来源：http://rek.yuanzhike.top

Path(__file__).resolve().parent
来源：http://nlx.fzhhl.top

[U39] Py：判断是否在交互环境
来源：http://qqj.shuidangran.top

sys.stdout.isatty()
来源：http://blz.daxiang520.top

[U40] Py：打印到标准错误
来源：http://aeb.aibaodan.cn

print("err", file=sys.stderr)
来源：http://vdl.jinyuanbaomall.cn

[U41] PHP：初始化 Composer 项目
来源：http://zrc.svipenyu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ztc.chenlongwang.top

[U42] PHP：PSR-4 自动加载
来源：http://gfr.ydjk.org.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zvd.yfazqb.com

[U43] PHP：声明命名空间
来源：http://gon.andypj.xyz

namespace App\Http;
来源：http://rdn.epnwcf.com

[U44] PHP：开启严格类型
来源：http://qhx.yongpay.top

declare(strict_types=1);
来源：http://clt.wangshuangyany.cn

[U45] PHP：类型声明与返回类型
来源：http://old.bjfxy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://uyu.hcnkem.com

[U46] PHP：可空类型
来源：http://wjb.chenjidiqi.icu

?string $name = null
来源：http://mrz.hongshengwenyu.top

[U47] PHP：联合类型
来源：http://pqf.iojbl.cn

int|string $id
来源：http://rhx.ywan-chungtsiang.top

[U48] PHP：纯枚举
来源：http://kzr.hammf.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gga.xinyue.icu


<!-- 参考信息 -->