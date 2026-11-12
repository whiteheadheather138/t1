代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mal.sxryk.cn

[S25] C：内存拷贝
来源：http://mgz.nanxuanxn.top

memcpy(dst, src, n);
来源：http://dsp.ctjpmb.com

[S26] C：内存清零
来源：http://osn.jinghuilouyu.cn

memset(a, 0, sizeof a);
来源：http://gjf.fanxiaobao.xyz

[S27] C：定义常量
来源：http://ccm.fehbvm.com

const double PI = 3.14159;
来源：http://tgd.dashuyun.cn

[S28] C：静态变量
来源：http://ebw.andypj.xyz

static int counter = 0;
来源：http://uty.cashguo.top

[S29] C：变参函数
来源：http://div.epnwcf.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xnb.zdqjudy.top

[S30] C：头文件保护
来源：http://wyo.fktsv.cn

#ifndef X_H
来源：http://lgt.316326.xyz

#define X_H
来源：http://ubp.xinyue.icu

#endif
来源：http://zia.fktsv.cn

[S31] C++：Hello World
来源：http://edz.snrcjt.cn

#include <iostream>
来源：http://rns.jinqigfzy.top

int main() { std::cout << "Hello\n"; }
来源：http://shl.quarkkingdee.top

[S32] C++：字符串
来源：http://nbk.sweek.top

std::string s = "hi";  s += "!";
来源：http://fdu.feifeiyinyue.top

[S33] C++：vector 增删
来源：http://hwy.hfpthk.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pin.ctjpmb.com

[S34] C++：遍历 vector
来源：http://oie.haohaochexian.top

for (auto &x : v) { std::cout << x; }
来源：http://dgw.gaohongyu789.top

[S35] C++：map
来源：http://bix.ydjk.org.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mzi.cdnleiting.top

[S36] C++：unordered_map
来源：http://tzo.hongshengwenyu.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pnr.zdqjudy.top

[S37] C++：set
来源：http://iwk.sysykeji.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yaj.jyoumei.cn

[S38] C++：排序
来源：http://kmb.cdnleiting.top

std::sort(v.begin(), v.end());
来源：http://lmh.nwbrower.top

[S39] C++：自定义比较器排序
来源：http://mwv.zhengqikj.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jev.zhoulong.xyz

[S40] C++：查找元素
来源：http://ozx.shzxlz.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://znl.xziqi.cn

[S41] C++：类与构造函数
来源：http://bzl.gaohongyu789.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zaj.jiagoushi.top

[S42] C++：继承与虚函数
来源：http://unj.andypj.xyz

class B : public Base { public: void f() override {} };
来源：http://psa.zhijiandao.cn

[S43] C++：智能指针
来源：http://ydu.guowangkeji.top

auto p = std::make_unique<int>(5);
来源：http://qbr.tian-w.cn

[S44] C++：引用传参
来源：http://ecl.52xcode.cn

void inc(int &x) { ++x; }
来源：http://olz.birdmap.top

[S45] C++：lambda
来源：http://xyg.gotoacloud.top

auto add = [](int a, int b) { return a + b; };
来源：http://bez.kuanghao11.cn

[S46] C++：函数模板
来源：http://yua.vehdjk.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zcy.ywan-chungtsiang.top

[S47] C++：结构化绑定遍历
来源：http://ocv.cdnleiting.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zmx.c1oappe.top

[S48] C++：逐行读文件
来源：http://nnk.iojbl.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wmi.daxiang520.top

while (std::getline(in, line)) { }
来源：http://whw.zhongyouzk.top

[S49] C++：写文件
来源：http://zqv.cucudq.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vxw.gotoacloud.top

[S50] C++：格式化数字
来源：http://juy.hfpthk.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ewi.pycfn.com

[S51] C++：显式类型转换
来源：http://adn.52xcode.cn

static_cast<double>(a) / b
来源：http://rxw.ehwqpu.com

[S52] C++：const 与 noexcept
来源：http://gui.yj202588.top

int size() const noexcept { return n_; }
来源：http://hfz.xinyue.icu

[S53] C++：移动语义
来源：http://jms.jianghu66.top

std::vector<int> w = std::move(v);
来源：http://pov.tarul.cn

[S54] C++：异常处理
来源：http://gwy.tian-w.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://azo.fanxiaobao.xyz

[S55] C++：结构化绑定
来源：http://var.cdnleiting.top

auto [a, b] = std::make_pair(1, 2);
来源：http://uqo.nanxinkj.top

[S56] C++：optional
来源：http://lyi.feifeiyinyue.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dth.guannengcc.top

[S57] C++：编译期常量
来源：http://mgf.zhijiandao.cn

constexpr int N = 10;
来源：http://jwp.nanxuanxn.top

[S58] C++：命名空间
来源：http://byg.hnxiangtu.top

namespace ns { int f() { return 1; } }
来源：http://bxb.fanxiaobao.xyz

[S59] C++：静态断言
来源：http://glz.jlsjyb.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zhf.epnwcf.com

[S60] C++：遍历并删除元素
来源：http://erz.zycfv.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://occ.zhiwuduotai.top

================================================================================
来源：http://owu.52xcode.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xnh.yuxming.cn

================================================================================
来源：http://vhi.hnqzz.top

[T01] Kotlin：Hello World
来源：http://wcb.zhoulong.xyz

println("Hello")
来源：http://syh.jqgufenzy.top

[T02] Kotlin：变量
来源：http://hfn.fanxiaobao.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xyk.smart0.xyz

[T03] Kotlin：字符串模板
来源：http://fkq.cqqwz.cn

"值: $b"
来源：http://asv.jinqigufen.top

[T04] Kotlin：空安全
来源：http://kcz.uphjek.com

val n: String? = null;  n?.length
来源：http://cfi.jinqigfzy.top

[T05] Kotlin：when 表达式
来源：http://oax.jianghu66.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qez.yj202588.top

[T06] Kotlin：集合映射
来源：http://fli.jiagoushi.top

listOf(1, 2, 3).map { it * 2 }
来源：http://oet.yonumen.top

[T07] Kotlin：集合过滤
来源：http://seg.chenjidiqi.icu

listOf(1, 2, 3).filter { it > 1 }
来源：http://xck.gogol.net.cn

[T08] Kotlin：数据类
来源：http://npo.nwbrower.top

data class User(val name: String, val age: Int)
来源：http://yej.hysaishi.cn

[T09] Kotlin：扩展函数
来源：http://azd.yuxming.cn

fun String.exclaim() = this + "!"
来源：http://qzm.shanyushiyangkeji.top

[T10] Kotlin：默认参数
来源：http://wwy.ctjpmb.com

fun greet(name: String = "World") = "Hi $name"
来源：http://ijg.zdbjq.cn

[T11] Kotlin：协程
来源：http://nam.hnxiangtu.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://jih.zhiwuduotai.top

[T12] Kotlin：解构声明
来源：http://tqs.zhaomingkeji.xyz

val (a, b) = Pair(1, 2)
来源：http://jln.ctjpmb.com

[T13] Kotlin：只读 Map
来源：http://meb.quarkkingdee.top

val m = mapOf("a" to 1)
来源：http://hjs.jiagoushi.top

[T14] Kotlin：循环
来源：http://pnz.gogol.net.cn

for (i in 1..10) println(i)
来源：http://onj.jyoumei.cn

[T15] Kotlin：接口
来源：http://sqp.gaohongyu789.top

interface Shape { fun area(): Double }
来源：http://yle.ehwqpu.com

[T16] Swift：Hello World
来源：http://bta.chenzaomai.com

print("Hello")
来源：http://acd.aizwys.cn

[T17] Swift：变量与常量
来源：http://bex.yonumen.top

var a = 1;  let b = 2
来源：http://cpq.ivvv.top

[T18] Swift：字符串插值
来源：http://wni.hammf.cn

"值: \(b)"
来源：http://wom.havefunace.top

[T19] Swift：可选绑定
来源：http://jxo.redwolf501.top

if let n = opt { print(n) }
来源：http://zqq.xuanzx.com

[T20] Swift：数组操作
来源：http://ndz.guannengcc.top

var a = [1, 2, 3];  a.append(4)
来源：http://xat.cqqwz.cn

[T21] Swift：遍历
来源：http://ozv.chenzaomai.com

for x in a { print(x) }
来源：http://nio.guowangkeji.top

[T22] Swift：字典
来源：http://dwv.hywenlv.cn

var d = ["a": 1];  d["b"] = 2
来源：http://uxc.ydzc1.top

[T23] Swift：函数
来源：http://pmg.sysykeji.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://uce.ybcxt.top

[T24] Swift：闭包
来源：http://nfp.hysaishi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://lzx.guannengcc.top

[T25] Swift：结构体
来源：http://bfq.fktsv.cn

struct P { var x: Int }
来源：http://wma.zhixingplan.top

[T26] Swift：类与重写
来源：http://pez.fanxiaobao.xyz

class A: Base { override func f() {} }
来源：http://tbq.chenzaomai.com

[T27] Swift：错误处理
来源：http://mqf.ydjk.org.cn

do { try f() } catch { print(error) }
来源：http://bwz.jinghuilouyu.cn

[T28] Swift：枚举
来源：http://veb.shzxlz.cn

enum Color { case red, green }
来源：http://uww.nanxuanxn.top

[T29] Swift：guard 提前返回
来源：http://pfj.zdqjudy.top

guard let x = opt else { return }
来源：http://ufv.shangyingyoupin.top

[T30] Swift：协议
来源：http://eai.hysaishi.cn

protocol Shape { func area() -> Double }
来源：http://uae.yangfankeji.com

[T31] Lua：Hello World
来源：http://dqf.smart0.xyz

print("Hello")
来源：http://bej.jyoumei.cn

[T32] Lua：局部变量
来源：http://lpr.ydjk.org.cn

local a = 1
来源：http://rho.tanke756.top

[T33] Lua：表（数组）
来源：http://wus.0kj1m.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://szb.yuanzhike.top

[T34] Lua：遍历表
来源：http://iqm.sxryk.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://naf.yongpay.top

[T35] Lua：字典表
来源：http://qan.jinqigufen.top

local d = { a = 1 };  d.b = 2
来源：http://ryv.xylfe.cn

[T36] Lua：函数
来源：http://ipm.tanke756.top

function add(a, b) return a + b end
来源：http://xco.9152youxi.cn

[T37] Lua：字符串拼接
来源：http://yer.shanyushiyangtech.top

"a" .. "b"
来源：http://bwg.jqgufenzy.top

[T38] Lua：条件
来源：http://dpc.jinyuanbaomall.cn

if x > 0 then print("正") end
来源：http://afi.cashguo.top

[T39] Lua：模式匹配
来源：http://yrv.yj20258.top

string.find(s, "%d+")
来源：http://sgu.316326.xyz

[T40] Lua：元表
来源：http://ief.yuxming.cn

setmetatable({}, { __index = base })
来源：http://grd.shanyushiyangkeji.top

[T41] Perl：Hello World
来源：http://nus.pycfn.com

print "Hello\n";
来源：http://wfe.kuanghao11.cn

[T42] Perl：变量类型
来源：http://fet.zhengqikj.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jan.haohaochexian.top

[T43] Perl：字符串插值
来源：http://osy.316326.xyz

"值: $a"
来源：http://aln.chenlongwang.top

[T44] Perl：条件
来源：http://crr.iojbl.cn

if ($a > 0) { print "正"; }
来源：http://ckf.jqgfzy.top

[T45] Perl：数组遍历
来源：http://igg.hesvh.cn

for my $x (@arr) { print $x; }
来源：http://hwm.ivvv.top

[T46] Perl：哈希操作
来源：http://uuc.birdmap.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fti.dashuyun.cn

[T47] Perl：正则捕获
来源：http://kvs.birdmap.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://qwd.snrcjt.cn

[T48] Perl：正则替换
来源：http://kfi.ywan-chungtsiang.top

$s =~ s/old/new/g;
来源：http://cwu.xziqi.cn

[T49] Perl：函数
来源：http://ajr.jinqigfzy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pjv.shanyushiyangtech.top

[T50] Perl：逐行读文件
来源：http://kzc.yfazqb.com

open my $fh, "<", "a.txt" or die $!;
来源：http://bwk.yvedp.cn

while (my $line = <$fh>) { print $line; }
来源：http://vet.hcnkem.com

[T51] Scala：Hello World
来源：http://xpd.52xcode.cn

println("Hello")
来源：http://lxn.ybcxt.top

[T52] Scala：变量
来源：http://txl.hnqzz.top

val a = 1;  var b = 2
来源：http://lya.daxiang520.top

[T53] Scala：字符串插值
来源：http://rgp.mhx1999.top

s"值: $b"
来源：http://wew.jqgufenzy.top

[T54] Scala：集合映射
来源：http://kif.meibo888.top

List(1, 2, 3).map(_ * 2)
来源：http://rfm.fehbvm.com

[T55] Scala：集合过滤
来源：http://tmh.yuanzhike.top

List(1, 2, 3).filter(_ > 1)
来源：http://wrr.jianghu66.top

[T56] Scala：样例类
来源：http://gou.hcnkem.com

case class User(name: String, age: Int)
来源：http://trh.svipenyu.cn

[T57] Scala：模式匹配
来源：http://ktd.andypj.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://cgf.sjlbkw.cn

[T58] Scala：函数定义
来源：http://skr.feifeiyinyue.top

def add(a: Int, b: Int): Int = a + b
来源：http://ulu.9152youxi.cn

[T59] Scala：循环
来源：http://erj.xziqi.cn

for (i <- 1 to 10) println(i)
来源：http://fhr.zhengqikj.top

[T60] Scala：折叠
来源：http://obz.jianghu66.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ndr.ppjwa.cn

================================================================================
来源：http://osq.gaohongyu789.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kjl.yj202588.top

================================================================================
来源：http://gli.haohaochexian.top

[U01] Py：创建虚拟环境
来源：http://lyp.fengsongda.top

python -m venv .venv && source .venv/bin/activate
来源：http://fkk.sjlbkw.cn

[U02] Py：导出 / 安装依赖
来源：http://xdc.zhixingplan.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gnx.xingfuxueyuan.xyz

[U03] Py：加载 .env 配置
来源：http://lqv.ppjwa.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ydw.aizwys.cn

[U04] Py：变量调试打印
来源：http://hup.nanxuanxn.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kic.iojbl.cn

[U05] Py：列表去重且保序
来源：http://xer.shanyushiyangtech.top

list(dict.fromkeys(arr))
来源：http://sqy.vqdsnc.cn

[U06] Py：合并两个字典
来源：http://fhb.daxiang520.top

{**a, **b}
来源：http://csy.0kj1m.cn

[U07] Py：反转字典键值
来源：http://wmu.tanke756.top

{v: k for k, v in d.items()}
来源：http://ldf.meibo888.top

[U08] Py：展平二维列表
来源：http://zqn.yongpay.top

[y for x in nested for y in x]
来源：http://rfo.xuetiantiany.cn

[U09] Py：字典取最大值的键
来源：http://cym.havefunace.top

max(d, key=d.get)
来源：http://czh.feifeiyinyue.top

[U10] Py：按值排序字典
来源：http://kmn.guowangkeji.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hpb.hnqzz.top

[U11] Py：生成器表达式
来源：http://are.yongpay.top

(x * 2 for x in arr)
来源：http://jio.jiagoushi.top

[U12] Py：取出现最多的 3 个元素
来源：http://fyb.svipenyu.cn

Counter(arr).most_common(3)
来源：http://dmg.xingfuxueyuan.xyz

[U13] Py：固定长度队列
来源：http://uoy.haohaochexian.top

deque(maxlen=10)
来源：http://pvc.shanyushiyangkeji.top

[U14] Py：分组收集到列表
来源：http://ima.nanxuanxn.top

defaultdict(list)
来源：http://got.zdbjq.cn

[U15] Py：高精度计时
来源：http://axd.jinqigfzy.top

t = time.perf_counter()
来源：http://thr.hammf.cn

[U16] Py：命令行参数解析
来源：http://ehz.yongpay.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qqn.jiagoushi.top

[U17] Py：初始化日志
来源：http://rnb.fengsongda.top

logging.basicConfig(level=logging.INFO)
来源：http://dzi.shuidangran.top

[U18] Py：预编译正则
来源：http://hyh.smart0.xyz

pat = re.compile(r"\d+")
来源：http://hjh.fzhhl.top

[U19] Py：正则替换带回调
来源：http://lqa.redwolf501.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wby.hysaishi.cn

[U20] Py：缓存函数结果
来源：http://xqc.yangfankeji.com

@functools.lru_cache(maxsize=None)
来源：http://wbo.havefunace.top

[U21] Py：自定义上下文管理器
来源：http://eyr.jianghu66.top

@contextlib.contextmanager
来源：http://qzu.xuetiantiany.cn

[U22] Py：矩阵转置
来源：http://lub.tianlin.xyz

list(zip(*m))
来源：http://fzj.yj20258.top

[U23] Py：分块读取大文件
来源：http://obn.xingfuxueyuan.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://voz.aibaodan.cn

[U24] Py：路径操作
来源：http://gsc.zhoulong.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ypk.ydzc1.top

[U25] Py：CSV 按字典读
来源：http://biv.hysaishi.cn

csv.DictReader(f)
来源：http://zrc.xingfuxueyuan.xyz

[U26] Py：并发下载
来源：http://qwy.zhijiandao.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ugt.guowangkeji.top

[U27] Py：异步 HTTP
来源：http://bfe.cdnleiting.top

aiohttp.ClientSession() 配合 async with
来源：http://rbc.cashguo.top

[U28] Py：类型别名
来源：http://npv.jlsjyb.cn

UserId = int
来源：http://ora.nanxuanxn.top

[U29] Py：属性校验
来源：http://kpi.guowangkeji.top

@property 与 @x.setter 配合
来源：http://ckr.snrcjt.cn

[U30] Py：数据类
来源：http://pbe.chenjidiqi.icu

@dataclass(slots=True)
来源：http://bis.jinyuanbaomall.cn

[U31] Py：单测
来源：http://yyr.quarkkingdee.top

python -m pytest -q
来源：http://qqo.chenzaomai.com

[U32] Py：代码格式化
来源：http://ucf.tarul.cn

ruff format . && ruff check --fix .
来源：http://lxt.jyoumei.cn

[U33] Py：打包发布
来源：http://axh.jqgfzy.top

python -m build  （依赖 pyproject.toml）
来源：http://kut.fengsongda.top

[U34] Py：判断编码
来源：http://gjw.zhixingplan.top

chardet.detect(raw)
来源：http://lhs.yangfankeji.com

[U35] Py：发送邮件
来源：http://vrh.hnqzz.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cvk.dianchejie.cn

[U36] Py：定时任务
来源：http://tvt.pycfn.com

schedule.every(10).minutes.do(job)
来源：http://bjb.meibo888.top

[U37] Py：读写 Excel
来源：http://xwe.aibaodan.cn

pandas.read_excel / DataFrame.to_excel
来源：http://mad.fktsv.cn

[U38] Py：获取脚本所在目录
来源：http://sfh.andypj.xyz

Path(__file__).resolve().parent
来源：http://kxt.jyoumei.cn

[U39] Py：判断是否在交互环境
来源：http://uzt.guannengcc.top

sys.stdout.isatty()
来源：http://fok.jianghu66.top

[U40] Py：打印到标准错误
来源：http://ian.aibaodan.cn

print("err", file=sys.stderr)
来源：http://tin.pengpengdd.cyou

[U41] PHP：初始化 Composer 项目
来源：http://dpk.yj202588.top

composer init;  composer require guzzlehttp/guzzle
来源：http://urk.redwolf501.top

[U42] PHP：PSR-4 自动加载
来源：http://tga.yvedp.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nmj.nanxinkj.top

[U43] PHP：声明命名空间
来源：http://hvq.xylfe.cn

namespace App\Http;
来源：http://ovf.zhijiandao.cn

[U44] PHP：开启严格类型
来源：http://eog.snrcjt.cn

declare(strict_types=1);
来源：http://vsx.daxiang520.top

[U45] PHP：类型声明与返回类型
来源：http://ecm.cdnleiting.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://rjq.ehwqpu.com

[U46] PHP：可空类型
来源：http://fjz.redwolf501.top

?string $name = null
来源：http://mxk.gotoacloud.top

[U47] PHP：联合类型
来源：http://qqt.yvedp.cn

int|string $id
来源：http://vzb.ydzc1.top

[U48] PHP：纯枚举
来源：http://wjn.zdbjq.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gpn.316326.xyz


<!-- 参考信息 -->