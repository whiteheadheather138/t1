代发 wailian999

static int counter = 0;
来源：http://ugv.haohaochexian.top

[S29] C：变参函数
来源：http://lbb.nwbrower.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gcc.yj20258888.top

[S30] C：头文件保护
来源：http://ppb.wangshuangyany.cn

#ifndef X_H
来源：http://qwq.fanxiaobao.xyz

#define X_H
来源：http://kwa.meibo888.top

#endif
来源：http://nok.hammf.cn

[S31] C++：Hello World
来源：http://zap.hnxiangtu.top

#include <iostream>
来源：http://cme.quarkkingdee.top

int main() { std::cout << "Hello\n"; }
来源：http://xfn.daria6918.cn

[S32] C++：字符串
来源：http://occ.sxryk.cn

std::string s = "hi";  s += "!";
来源：http://dxd.yfazqb.com

[S33] C++：vector 增删
来源：http://bow.yj20258888.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xdw.xuanzx.com

[S34] C++：遍历 vector
来源：http://urc.cheryme.top

for (auto &x : v) { std::cout << x; }
来源：http://szj.fktsv.cn

[S35] C++：map
来源：http://pvu.ybcxt.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://seo.gotoacloud.top

[S36] C++：unordered_map
来源：http://xkl.jianghu66.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ldz.pycfn.com

[S37] C++：set
来源：http://knr.shanyushiyangkeji.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://odz.9152youxi.cn

[S38] C++：排序
来源：http://jgl.chenlongwang.top

std::sort(v.begin(), v.end());
来源：http://ipw.kuanghao11.cn

[S39] C++：自定义比较器排序
来源：http://byb.aibaodan.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rqk.fehbvm.com

[S40] C++：查找元素
来源：http://rql.nanxinkj.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vef.jinqigufen.top

[S41] C++：类与构造函数
来源：http://qlu.nanxuanxn.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://syc.nanxinkj.top

[S42] C++：继承与虚函数
来源：http://qjn.shangyingyoupin.top

class B : public Base { public: void f() override {} };
来源：http://dlu.jinghuilouyu.cn

[S43] C++：智能指针
来源：http://ufp.hongshengwenyu.top

auto p = std::make_unique<int>(5);
来源：http://hbl.316326.xyz

[S44] C++：引用传参
来源：http://gjo.chenzaomai.com

void inc(int &x) { ++x; }
来源：http://htv.pycfn.com

[S45] C++：lambda
来源：http://dgu.bjfxy.top

auto add = [](int a, int b) { return a + b; };
来源：http://zuk.iojbl.cn

[S46] C++：函数模板
来源：http://ckx.iojbl.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://msv.uphjek.com

[S47] C++：结构化绑定遍历
来源：http://hoo.cheryme.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fcw.xinyue.icu

[S48] C++：逐行读文件
来源：http://ofy.jiagoushi.top

std::ifstream in("a.txt");  std::string line;
来源：http://dwk.guannengcc.top

while (std::getline(in, line)) { }
来源：http://ezl.daxiang520.top

[S49] C++：写文件
来源：http://kpu.sysykeji.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hef.jiagoushi.top

[S50] C++：格式化数字
来源：http://bgz.xinyue.icu

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qmb.svipenyu.cn

[S51] C++：显式类型转换
来源：http://zjy.fktsv.cn

static_cast<double>(a) / b
来源：http://nkx.jinyuanbaomall.cn

[S52] C++：const 与 noexcept
来源：http://cjr.yongpay.top

int size() const noexcept { return n_; }
来源：http://wll.cheryme.top

[S53] C++：移动语义
来源：http://uyh.wangdashe.top

std::vector<int> w = std::move(v);
来源：http://cwx.daria6918.cn

[S54] C++：异常处理
来源：http://bqh.xinyue.icu

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rko.yanxiufei.cn

[S55] C++：结构化绑定
来源：http://avk.yj202588.top

auto [a, b] = std::make_pair(1, 2);
来源：http://lmo.9152youxi.cn

[S56] C++：optional
来源：http://vba.gzhubu.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jtv.dashuyun.cn

[S57] C++：编译期常量
来源：http://uzj.chenzaomai.com

constexpr int N = 10;
来源：http://hzn.fzhhl.top

[S58] C++：命名空间
来源：http://sed.hammf.cn

namespace ns { int f() { return 1; } }
来源：http://dcw.zycfv.cn

[S59] C++：静态断言
来源：http://hce.sysykeji.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://uxf.hysaishi.cn

[S60] C++：遍历并删除元素
来源：http://zpd.shangyingyoupin.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gjx.feifeiyinyue.top

================================================================================
来源：http://joy.fengsongda.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rcf.fanxiaobao.xyz

================================================================================
来源：http://udm.yanxiufei.cn

[T01] Kotlin：Hello World
来源：http://xrt.daxiang520.top

println("Hello")
来源：http://hlb.yonumen.top

[T02] Kotlin：变量
来源：http://kxd.yvedp.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://msj.cucudq.cn

[T03] Kotlin：字符串模板
来源：http://bcx.hammf.cn

"值: $b"
来源：http://wjv.pycfn.com

[T04] Kotlin：空安全
来源：http://yic.jqgufenzy.top

val n: String? = null;  n?.length
来源：http://mjx.jqgufenzy.top

[T05] Kotlin：when 表达式
来源：http://gkr.cashguo.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://moh.jqgfzy.top

[T06] Kotlin：集合映射
来源：http://yab.svipenyu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://gla.zhiwuduotai.top

[T07] Kotlin：集合过滤
来源：http://wxc.cdnleiting.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://bie.hongshengwenyu.top

[T08] Kotlin：数据类
来源：http://ctu.redwolf501.top

data class User(val name: String, val age: Int)
来源：http://kne.hcnkem.com

[T09] Kotlin：扩展函数
来源：http://jkq.yonumen.top

fun String.exclaim() = this + "!"
来源：http://wgs.cqqwz.cn

[T10] Kotlin：默认参数
来源：http://nko.xziqi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://fpw.zdqjudy.top

[T11] Kotlin：协程
来源：http://zrw.ehwqpu.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://tpn.havefunace.top

[T12] Kotlin：解构声明
来源：http://ezj.hywenlv.cn

val (a, b) = Pair(1, 2)
来源：http://nwj.jinqigfzy.top

[T13] Kotlin：只读 Map
来源：http://ogq.zdqjudy.top

val m = mapOf("a" to 1)
来源：http://amb.havefunace.top

[T14] Kotlin：循环
来源：http://mhz.birdmap.top

for (i in 1..10) println(i)
来源：http://oob.ybcxt.top

[T15] Kotlin：接口
来源：http://jqu.jinghuilouyu.cn

interface Shape { fun area(): Double }
来源：http://qvq.uphjek.com

[T16] Swift：Hello World
来源：http://ebl.ehwqpu.com

print("Hello")
来源：http://hsb.ywan-chungtsiang.top

[T17] Swift：变量与常量
来源：http://bws.jinqigfzy.top

var a = 1;  let b = 2
来源：http://kxg.vehdjk.com

[T18] Swift：字符串插值
来源：http://esg.zhiwuduotai.top

"值: \(b)"
来源：http://bbp.chenjidiqi.icu

[T19] Swift：可选绑定
来源：http://kjb.tianlin.xyz

if let n = opt { print(n) }
来源：http://cco.cdnleiting.top

[T20] Swift：数组操作
来源：http://ljh.ctjpmb.com

var a = [1, 2, 3];  a.append(4)
来源：http://vaa.guannengcc.top

[T21] Swift：遍历
来源：http://fwa.yangfankeji.com

for x in a { print(x) }
来源：http://mny.guannengcc.top

[T22] Swift：字典
来源：http://sow.yonumen.top

var d = ["a": 1];  d["b"] = 2
来源：http://lsh.chenlongwang.top

[T23] Swift：函数
来源：http://voy.quarkkingdee.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ozq.birdmap.top

[T24] Swift：闭包
来源：http://gdg.smart0.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://vab.yanxiufei.cn

[T25] Swift：结构体
来源：http://vst.daxiang520.top

struct P { var x: Int }
来源：http://luc.smart0.xyz

[T26] Swift：类与重写
来源：http://hse.wangshuangyany.cn

class A: Base { override func f() {} }
来源：http://bea.zhoulong.xyz

[T27] Swift：错误处理
来源：http://hzs.hongshengwenyu.top

do { try f() } catch { print(error) }
来源：http://bqx.gzhubu.top

[T28] Swift：枚举
来源：http://vxv.hfpthk.cn

enum Color { case red, green }
来源：http://hri.xziqi.cn

[T29] Swift：guard 提前返回
来源：http://nch.wangdashe.top

guard let x = opt else { return }
来源：http://bgc.feifeiyinyue.top

[T30] Swift：协议
来源：http://lst.yonumen.top

protocol Shape { func area() -> Double }
来源：http://tzr.smart0.xyz

[T31] Lua：Hello World
来源：http://ftj.aizwys.cn

print("Hello")
来源：http://cyw.zdqjudy.top

[T32] Lua：局部变量
来源：http://gct.zdqjudy.top

local a = 1
来源：http://rnb.dianchejie.cn

[T33] Lua：表（数组）
来源：http://bxi.hfpthk.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://gxw.guowangkeji.top

[T34] Lua：遍历表
来源：http://sfd.tanke756.top

for i, v in ipairs(t) do print(i, v) end
来源：http://nlm.jinqigufen.top

[T35] Lua：字典表
来源：http://rld.xingfuxueyuan.xyz

local d = { a = 1 };  d.b = 2
来源：http://ngw.fehbvm.com

[T36] Lua：函数
来源：http://rfq.nwbrower.top

function add(a, b) return a + b end
来源：http://hth.cqqwz.cn

[T37] Lua：字符串拼接
来源：http://uwm.jyoumei.cn

"a" .. "b"
来源：http://yhw.yuanzhike.top

[T38] Lua：条件
来源：http://peb.zhixingplan.top

if x > 0 then print("正") end
来源：http://mva.yj20258888.top

[T39] Lua：模式匹配
来源：http://hrx.sysykeji.top

string.find(s, "%d+")
来源：http://way.fzhhl.top

[T40] Lua：元表
来源：http://wok.shanyushiyangkeji.top

setmetatable({}, { __index = base })
来源：http://sgm.bbcook.cn

[T41] Perl：Hello World
来源：http://iav.cashguo.top

print "Hello\n";
来源：http://onn.jlsjyb.cn

[T42] Perl：变量类型
来源：http://mbw.iojbl.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mvw.yueranfly.top

[T43] Perl：字符串插值
来源：http://ajp.ehwqpu.com

"值: $a"
来源：http://gte.uphjek.com

[T44] Perl：条件
来源：http://qwy.jlsjyb.cn

if ($a > 0) { print "正"; }
来源：http://nwu.daria6918.cn

[T45] Perl：数组遍历
来源：http://jok.yonumen.top

for my $x (@arr) { print $x; }
来源：http://oqj.haohaochexian.top

[T46] Perl：哈希操作
来源：http://cce.xuetiantiany.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kho.aizwys.cn

[T47] Perl：正则捕获
来源：http://tui.sufxvd.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://toi.jyoumei.cn

[T48] Perl：正则替换
来源：http://bwr.cucudq.cn

$s =~ s/old/new/g;
来源：http://gxa.jqgufenzy.top

[T49] Perl：函数
来源：http://zwo.dashuyun.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rso.daria6918.cn

[T50] Perl：逐行读文件
来源：http://obd.jqgufenzy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://xab.wangshuangyany.cn

while (my $line = <$fh>) { print $line; }
来源：http://zwj.ehwqpu.com

[T51] Scala：Hello World
来源：http://cey.sufxvd.cn

println("Hello")
来源：http://hvx.9152youxi.cn

[T52] Scala：变量
来源：http://ypa.nanxinkj.top

val a = 1;  var b = 2
来源：http://ldy.hysaishi.cn

[T53] Scala：字符串插值
来源：http://osh.hcnkem.com

s"值: $b"
来源：http://ffi.316326.xyz

[T54] Scala：集合映射
来源：http://hnq.xinyue.icu

List(1, 2, 3).map(_ * 2)
来源：http://obf.ehwqpu.com

[T55] Scala：集合过滤
来源：http://rqj.gzhubu.top

List(1, 2, 3).filter(_ > 1)
来源：http://ibz.jlsjyb.cn

[T56] Scala：样例类
来源：http://fhf.jqgufenzy.top

case class User(name: String, age: Int)
来源：http://vbp.birdmap.top

[T57] Scala：模式匹配
来源：http://yxv.sjlbkw.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://kyt.zhijiandao.cn

[T58] Scala：函数定义
来源：http://ivy.zhijiandao.cn

def add(a: Int, b: Int): Int = a + b
来源：http://jvn.xziqi.cn

[T59] Scala：循环
来源：http://wyo.ydzc1.top

for (i <- 1 to 10) println(i)
来源：http://cmf.fehbvm.com

[T60] Scala：折叠
来源：http://gwz.jinghuilouyu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mgj.sysykeji.top

================================================================================
来源：http://rsy.ywan-chungtsiang.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yng.ywan-chungtsiang.top

================================================================================
来源：http://jin.ehwqpu.com

[U01] Py：创建虚拟环境
来源：http://xtx.ppjwa.cn

python -m venv .venv && source .venv/bin/activate
来源：http://zlr.jlsjyb.cn

[U02] Py：导出 / 安装依赖
来源：http://mjn.yanxiufei.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://off.gzhubu.top

[U03] Py：加载 .env 配置
来源：http://aaj.smart0.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://jij.bbcook.cn

[U04] Py：变量调试打印
来源：http://qzi.xuetiantiany.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pag.haohaochexian.top

[U05] Py：列表去重且保序
来源：http://see.wangdashe.top

list(dict.fromkeys(arr))
来源：http://sme.zhaomingkeji.xyz

[U06] Py：合并两个字典
来源：http://jrm.zdqjudy.top

{**a, **b}
来源：http://fve.wangdashe.top

[U07] Py：反转字典键值
来源：http://ste.gotoacloud.top

{v: k for k, v in d.items()}
来源：http://rtr.hfpthk.cn

[U08] Py：展平二维列表
来源：http://woq.jinqigufen.top

[y for x in nested for y in x]
来源：http://kwa.daria6918.cn

[U09] Py：字典取最大值的键
来源：http://iuy.birdmap.top

max(d, key=d.get)
来源：http://nzz.guowangkeji.top

[U10] Py：按值排序字典
来源：http://xhc.cashguo.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dip.andypj.xyz

[U11] Py：生成器表达式
来源：http://exz.fanxiaobao.xyz

(x * 2 for x in arr)
来源：http://srf.quarkkingdee.top

[U12] Py：取出现最多的 3 个元素
来源：http://ugp.fzhhl.top

Counter(arr).most_common(3)
来源：http://ctd.zhoulong.xyz

[U13] Py：固定长度队列
来源：http://pmz.yonumen.top

deque(maxlen=10)
来源：http://xgf.shuidangran.top

[U14] Py：分组收集到列表
来源：http://uht.fanxiaobao.xyz

defaultdict(list)
来源：http://icc.ehwqpu.com

[U15] Py：高精度计时
来源：http://lgh.feifeiyinyue.top

t = time.perf_counter()
来源：http://ytj.nanxuanxn.top

[U16] Py：命令行参数解析
来源：http://voq.yj202588.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hfk.316326.xyz

[U17] Py：初始化日志
来源：http://uvs.chenjidiqi.icu

logging.basicConfig(level=logging.INFO)
来源：http://jtx.gzhubu.top

[U18] Py：预编译正则
来源：http://gxb.yongpay.top

pat = re.compile(r"\d+")
来源：http://mlg.shangyingyoupin.top

[U19] Py：正则替换带回调
来源：http://lyv.cashguo.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://adl.vqdsnc.cn

[U20] Py：缓存函数结果
来源：http://pwy.aibaodan.cn

@functools.lru_cache(maxsize=None)
来源：http://anm.hywenlv.cn

[U21] Py：自定义上下文管理器
来源：http://njg.jyoumei.cn

@contextlib.contextmanager
来源：http://mad.sufxvd.cn

[U22] Py：矩阵转置
来源：http://ybg.sxryk.cn

list(zip(*m))
来源：http://hml.zhijiandao.cn

[U23] Py：分块读取大文件
来源：http://sai.xuanzx.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ull.dianchejie.cn

[U24] Py：路径操作
来源：http://tnn.bbcook.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://spd.sysykeji.top

[U25] Py：CSV 按字典读
来源：http://yre.xziqi.cn

csv.DictReader(f)
来源：http://wee.meibo888.top

[U26] Py：并发下载
来源：http://qvb.pycfn.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xkb.jinyuanbaomall.cn

[U27] Py：异步 HTTP
来源：http://drr.zhiwuduotai.top

aiohttp.ClientSession() 配合 async with
来源：http://tac.zhongyouzk.top

[U28] Py：类型别名
来源：http://nnf.xylfe.cn

UserId = int
来源：http://aey.smart0.xyz

[U29] Py：属性校验
来源：http://ncn.shzxlz.cn

@property 与 @x.setter 配合
来源：http://jey.zhoulong.xyz

[U30] Py：数据类
来源：http://dzr.jinghuilouyu.cn

@dataclass(slots=True)
来源：http://blm.epnwcf.com

[U31] Py：单测
来源：http://itu.zhaomingkeji.xyz

python -m pytest -q
来源：http://azr.tanke756.top

[U32] Py：代码格式化
来源：http://ckh.xuetiantiany.cn

ruff format . && ruff check --fix .
来源：http://jmx.zhongyouzk.top

[U33] Py：打包发布
来源：http://pdt.guannengcc.top

python -m build  （依赖 pyproject.toml）
来源：http://khi.yonumen.top

[U34] Py：判断编码
来源：http://axh.wangdashe.top

chardet.detect(raw)
来源：http://mop.iojbl.cn

[U35] Py：发送邮件
来源：http://rlw.shanyushiyangkeji.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kla.ywan-chungtsiang.top

[U36] Py：定时任务
来源：http://msm.meibo888.top

schedule.every(10).minutes.do(job)
来源：http://eup.zycfv.cn

[U37] Py：读写 Excel
来源：http://ldq.hysaishi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://gvc.hnqzz.top

[U38] Py：获取脚本所在目录
来源：http://zms.xylfe.cn

Path(__file__).resolve().parent
来源：http://nza.ywan-chungtsiang.top

[U39] Py：判断是否在交互环境
来源：http://vpd.havefunace.top

sys.stdout.isatty()
来源：http://xqw.shangyingyoupin.top

[U40] Py：打印到标准错误
来源：http://fwe.ydjk.org.cn

print("err", file=sys.stderr)
来源：http://fkr.feifeiyinyue.top

[U41] PHP：初始化 Composer 项目
来源：http://lwq.jianghu66.top

composer init;  composer require guzzlehttp/guzzle
来源：http://bmi.bjfxy.top

[U42] PHP：PSR-4 自动加载
来源：http://dlp.daxiang520.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://iur.yuanzhike.top

[U43] PHP：声明命名空间
来源：http://isn.yj202588.top

namespace App\Http;
来源：http://fby.ehwqpu.com

[U44] PHP：开启严格类型
来源：http://zpj.yueranfly.top

declare(strict_types=1);
来源：http://ueh.ybcxt.top

[U45] PHP：类型声明与返回类型
来源：http://wsa.gzhubu.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://fbv.zhoulong.xyz

[U46] PHP：可空类型
来源：http://tkg.ydjk.org.cn

?string $name = null
来源：http://zqi.smart0.xyz

[U47] PHP：联合类型
来源：http://nru.fzhhl.top

int|string $id
来源：http://ukp.hammf.cn

[U48] PHP：纯枚举
来源：http://neo.pycfn.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ios.sysykeji.top

[U49] PHP：只读属性
来源：http://gbq.havefunace.top

public readonly string $name
来源：http://obb.dianchejie.cn

[U50] PHP：构造器属性提升
来源：http://haa.aibaodan.cn

public function __construct(private int $id) {}
来源：http://jkh.jyoumei.cn

[U51] PHP：数组解构
来源：http://gvw.zhixingplan.top

[$a, $b] = $arr;
来源：http://ega.xinyue.icu

[U52] PHP：箭头函数
来源：http://qce.jqgufenzy.top

$double = fn($x) => $x * 2;
来源：http://yih.chenlongwang.top


<!-- 参考信息 -->