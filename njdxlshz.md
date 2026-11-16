代发 wailian999

static int counter = 0;
来源：http://vzk.daria6918.cn

[S29] C：变参函数
来源：http://oed.yueranfly.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zqv.jianghu66.top

[S30] C：头文件保护
来源：http://vqh.hongshengwenyu.top

#ifndef X_H
来源：http://rdh.xuanzx.com

#define X_H
来源：http://fnj.bjfxy.top

#endif
来源：http://bxz.guowangkeji.top

[S31] C++：Hello World
来源：http://gzf.haohaochexian.top

#include <iostream>
来源：http://xky.guannengcc.top

int main() { std::cout << "Hello\n"; }
来源：http://cmr.nwbrower.top

[S32] C++：字符串
来源：http://nae.smart0.xyz

std::string s = "hi";  s += "!";
来源：http://exg.yj202588.top

[S33] C++：vector 增删
来源：http://rqu.wangshuangyany.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tpq.sufxvd.cn

[S34] C++：遍历 vector
来源：http://sav.andypj.xyz

for (auto &x : v) { std::cout << x; }
来源：http://uim.andypj.xyz

[S35] C++：map
来源：http://acp.hammf.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rfb.yj20258888.top

[S36] C++：unordered_map
来源：http://mez.zycfv.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://owg.yangfankeji.com

[S37] C++：set
来源：http://zmn.yonumen.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qwz.shanyushiyangtech.top

[S38] C++：排序
来源：http://hia.ivvv.top

std::sort(v.begin(), v.end());
来源：http://jdh.sxryk.cn

[S39] C++：自定义比较器排序
来源：http://ndt.zhaomingkeji.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://aux.hcnkem.com

[S40] C++：查找元素
来源：http://yti.jinqigufen.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://haj.9152youxi.cn

[S41] C++：类与构造函数
来源：http://flh.fehbvm.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fnu.yongpay.top

[S42] C++：继承与虚函数
来源：http://foo.bbcook.cn

class B : public Base { public: void f() override {} };
来源：http://olt.yfazqb.com

[S43] C++：智能指针
来源：http://ikk.c1oappe.top

auto p = std::make_unique<int>(5);
来源：http://qeb.dianchejie.cn

[S44] C++：引用传参
来源：http://cku.fengsongda.top

void inc(int &x) { ++x; }
来源：http://cnr.pengpengdd.cyou

[S45] C++：lambda
来源：http://yjy.ywan-chungtsiang.top

auto add = [](int a, int b) { return a + b; };
来源：http://uqr.nwbrower.top

[S46] C++：函数模板
来源：http://czr.snrcjt.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jyp.kuanghao11.cn

[S47] C++：结构化绑定遍历
来源：http://wlu.fehbvm.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://aqf.jyoumei.cn

[S48] C++：逐行读文件
来源：http://fja.tarul.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gzi.yuanzhike.top

while (std::getline(in, line)) { }
来源：http://ibs.sxryk.cn

[S49] C++：写文件
来源：http://ptk.yanxiufei.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://end.0kj1m.cn

[S50] C++：格式化数字
来源：http://hua.hfpthk.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jsg.yfazqb.com

[S51] C++：显式类型转换
来源：http://yob.snrcjt.cn

static_cast<double>(a) / b
来源：http://cup.bjfxy.top

[S52] C++：const 与 noexcept
来源：http://vdz.sweek.top

int size() const noexcept { return n_; }
来源：http://rkh.aibaodan.cn

[S53] C++：移动语义
来源：http://jal.yongpay.top

std::vector<int> w = std::move(v);
来源：http://hlu.cucudq.cn

[S54] C++：异常处理
来源：http://lsw.nanxinkj.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tlm.ehwqpu.com

[S55] C++：结构化绑定
来源：http://okk.aizwys.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://pyo.yj202588.top

[S56] C++：optional
来源：http://hzo.tarul.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wct.yongpay.top

[S57] C++：编译期常量
来源：http://yrg.hesvh.cn

constexpr int N = 10;
来源：http://wur.aibaodan.cn

[S58] C++：命名空间
来源：http://glu.hongshengwenyu.top

namespace ns { int f() { return 1; } }
来源：http://hdu.vqdsnc.cn

[S59] C++：静态断言
来源：http://uhm.vqdsnc.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hvf.ywan-chungtsiang.top

[S60] C++：遍历并删除元素
来源：http://tvz.aizwys.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jie.zhiwuduotai.top

================================================================================
来源：http://vbh.tanke756.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jyp.haohaochexian.top

================================================================================
来源：http://znn.hammf.cn

[T01] Kotlin：Hello World
来源：http://nga.feifeiyinyue.top

println("Hello")
来源：http://baq.fehbvm.com

[T02] Kotlin：变量
来源：http://ofk.iojbl.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rff.tarul.cn

[T03] Kotlin：字符串模板
来源：http://gfj.zdbjq.cn

"值: $b"
来源：http://kug.zdbjq.cn

[T04] Kotlin：空安全
来源：http://nao.cqqwz.cn

val n: String? = null;  n?.length
来源：http://leu.zhiwuduotai.top

[T05] Kotlin：when 表达式
来源：http://hyy.jyoumei.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://aye.zhoulong.xyz

[T06] Kotlin：集合映射
来源：http://tsi.daxiang520.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ulp.hcnkem.com

[T07] Kotlin：集合过滤
来源：http://uov.xingfuxueyuan.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://xud.daxiang520.top

[T08] Kotlin：数据类
来源：http://dzg.iojbl.cn

data class User(val name: String, val age: Int)
来源：http://udy.zhengqikj.top

[T09] Kotlin：扩展函数
来源：http://ovj.gaohongyu789.top

fun String.exclaim() = this + "!"
来源：http://ltn.gaohongyu789.top

[T10] Kotlin：默认参数
来源：http://nsw.yongpay.top

fun greet(name: String = "World") = "Hi $name"
来源：http://bin.hnxiangtu.top

[T11] Kotlin：协程
来源：http://zgg.jinqigfzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://hsf.sysykeji.top

[T12] Kotlin：解构声明
来源：http://nah.zhaomingkeji.xyz

val (a, b) = Pair(1, 2)
来源：http://bnm.wangdashe.top

[T13] Kotlin：只读 Map
来源：http://evy.sysykeji.top

val m = mapOf("a" to 1)
来源：http://fpr.hnxiangtu.top

[T14] Kotlin：循环
来源：http://uur.pycfn.com

for (i in 1..10) println(i)
来源：http://qhq.redwolf501.top

[T15] Kotlin：接口
来源：http://nih.quarkkingdee.top

interface Shape { fun area(): Double }
来源：http://quj.bjfxy.top

[T16] Swift：Hello World
来源：http://kei.guowangkeji.top

print("Hello")
来源：http://xev.sufxvd.cn

[T17] Swift：变量与常量
来源：http://asc.sxryk.cn

var a = 1;  let b = 2
来源：http://kls.hammf.cn

[T18] Swift：字符串插值
来源：http://kcd.0kj1m.cn

"值: \(b)"
来源：http://zgw.hnqzz.top

[T19] Swift：可选绑定
来源：http://xeu.xziqi.cn

if let n = opt { print(n) }
来源：http://azo.havefunace.top

[T20] Swift：数组操作
来源：http://grb.ydzc1.top

var a = [1, 2, 3];  a.append(4)
来源：http://xhq.jianghu66.top

[T21] Swift：遍历
来源：http://aau.aizwys.cn

for x in a { print(x) }
来源：http://pcn.yanxiufei.cn

[T22] Swift：字典
来源：http://ely.zhixingplan.top

var d = ["a": 1];  d["b"] = 2
来源：http://plp.fktsv.cn

[T23] Swift：函数
来源：http://vqa.vqdsnc.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://aaz.0kj1m.cn

[T24] Swift：闭包
来源：http://lbz.daxiang520.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://pin.meibo888.top

[T25] Swift：结构体
来源：http://beu.cdnleiting.top

struct P { var x: Int }
来源：http://epm.shzxlz.cn

[T26] Swift：类与重写
来源：http://iwu.sweek.top

class A: Base { override func f() {} }
来源：http://cyq.fehbvm.com

[T27] Swift：错误处理
来源：http://gmi.guannengcc.top

do { try f() } catch { print(error) }
来源：http://ifg.fehbvm.com

[T28] Swift：枚举
来源：http://ymx.hywenlv.cn

enum Color { case red, green }
来源：http://lgz.tianlin.xyz

[T29] Swift：guard 提前返回
来源：http://bcp.xylfe.cn

guard let x = opt else { return }
来源：http://hoz.jinghuilouyu.cn

[T30] Swift：协议
来源：http://heh.tanke756.top

protocol Shape { func area() -> Double }
来源：http://uqw.cqqwz.cn

[T31] Lua：Hello World
来源：http://bes.zhengqikj.top

print("Hello")
来源：http://jkf.fzhhl.top

[T32] Lua：局部变量
来源：http://kjc.shanyushiyangkeji.top

local a = 1
来源：http://bbl.ehwqpu.com

[T33] Lua：表（数组）
来源：http://shm.fktsv.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hmc.chenjidiqi.icu

[T34] Lua：遍历表
来源：http://kug.shangyingyoupin.top

for i, v in ipairs(t) do print(i, v) end
来源：http://gdt.9152youxi.cn

[T35] Lua：字典表
来源：http://yim.svipenyu.cn

local d = { a = 1 };  d.b = 2
来源：http://iqp.ehwqpu.com

[T36] Lua：函数
来源：http://fvg.nwbrower.top

function add(a, b) return a + b end
来源：http://lml.andypj.xyz

[T37] Lua：字符串拼接
来源：http://eez.jinqigfzy.top

"a" .. "b"
来源：http://uub.ywan-chungtsiang.top

[T38] Lua：条件
来源：http://lal.xuetiantiany.cn

if x > 0 then print("正") end
来源：http://fxl.0kj1m.cn

[T39] Lua：模式匹配
来源：http://rch.smart0.xyz

string.find(s, "%d+")
来源：http://lqb.wangshuangyany.cn

[T40] Lua：元表
来源：http://lmj.nanxuanxn.top

setmetatable({}, { __index = base })
来源：http://xwt.tian-w.cn

[T41] Perl：Hello World
来源：http://cuq.chenlongwang.top

print "Hello\n";
来源：http://qfr.zdqjudy.top

[T42] Perl：变量类型
来源：http://uhm.jinqigufen.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pwc.ydjk.org.cn

[T43] Perl：字符串插值
来源：http://tvo.zhiwuduotai.top

"值: $a"
来源：http://nrj.jianghu66.top

[T44] Perl：条件
来源：http://ddp.jinghuilouyu.cn

if ($a > 0) { print "正"; }
来源：http://has.tanke756.top

[T45] Perl：数组遍历
来源：http://hyu.shanyushiyangtech.top

for my $x (@arr) { print $x; }
来源：http://qtz.yueranfly.top

[T46] Perl：哈希操作
来源：http://snf.hfpthk.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://puf.zycfv.cn

[T47] Perl：正则捕获
来源：http://bdt.birdmap.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://pkh.jinghuilouyu.cn

[T48] Perl：正则替换
来源：http://zkj.hywenlv.cn

$s =~ s/old/new/g;
来源：http://msi.xylfe.cn

[T49] Perl：函数
来源：http://lac.fzhhl.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://isw.jlsjyb.cn

[T50] Perl：逐行读文件
来源：http://ias.nwbrower.top

open my $fh, "<", "a.txt" or die $!;
来源：http://kdd.cashguo.top

while (my $line = <$fh>) { print $line; }
来源：http://eji.yfazqb.com

[T51] Scala：Hello World
来源：http://agw.tanke756.top

println("Hello")
来源：http://fgo.zhongyouzk.top

[T52] Scala：变量
来源：http://dep.feifeiyinyue.top

val a = 1;  var b = 2
来源：http://qac.quarkkingdee.top

[T53] Scala：字符串插值
来源：http://fai.0kj1m.cn

s"值: $b"
来源：http://qhb.guowangkeji.top

[T54] Scala：集合映射
来源：http://dyf.hysaishi.cn

List(1, 2, 3).map(_ * 2)
来源：http://sul.yangfankeji.com

[T55] Scala：集合过滤
来源：http://gxa.jinqigufen.top

List(1, 2, 3).filter(_ > 1)
来源：http://ewu.tianlin.xyz

[T56] Scala：样例类
来源：http://jxu.sjlbkw.cn

case class User(name: String, age: Int)
来源：http://dtv.haohaochexian.top

[T57] Scala：模式匹配
来源：http://leo.havefunace.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://xst.cashguo.top

[T58] Scala：函数定义
来源：http://wvs.yuxming.cn

def add(a: Int, b: Int): Int = a + b
来源：http://sra.sxryk.cn

[T59] Scala：循环
来源：http://tbg.xinyue.icu

for (i <- 1 to 10) println(i)
来源：http://vts.gogol.net.cn

[T60] Scala：折叠
来源：http://faz.hnxiangtu.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://out.bjfxy.top

================================================================================
来源：http://ivt.shangyingyoupin.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ctt.xinyue.icu

================================================================================
来源：http://hke.hongshengwenyu.top

[U01] Py：创建虚拟环境
来源：http://syb.fzhhl.top

python -m venv .venv && source .venv/bin/activate
来源：http://etx.ctjpmb.com

[U02] Py：导出 / 安装依赖
来源：http://jkd.jianghu66.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fem.gaohongyu789.top

[U03] Py：加载 .env 配置
来源：http://gtf.mhx1999.top

from dotenv import load_dotenv; load_dotenv()
来源：http://cbh.meibo888.top

[U04] Py：变量调试打印
来源：http://qos.yanxiufei.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://htm.nwbrower.top

[U05] Py：列表去重且保序
来源：http://cuy.shangyingyoupin.top

list(dict.fromkeys(arr))
来源：http://gls.jqgfzy.top

[U06] Py：合并两个字典
来源：http://prw.sxryk.cn

{**a, **b}
来源：http://mmc.zhiwuduotai.top

[U07] Py：反转字典键值
来源：http://qhp.wangdashe.top

{v: k for k, v in d.items()}
来源：http://cnr.xinyue.icu

[U08] Py：展平二维列表
来源：http://evi.jiagoushi.top

[y for x in nested for y in x]
来源：http://vjp.jinyuanbaomall.cn

[U09] Py：字典取最大值的键
来源：http://kxw.aizwys.cn

max(d, key=d.get)
来源：http://ijv.chenlongwang.top

[U10] Py：按值排序字典
来源：http://til.svipenyu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://anr.ybcxt.top

[U11] Py：生成器表达式
来源：http://ctr.gotoacloud.top

(x * 2 for x in arr)
来源：http://qhn.ppjwa.cn

[U12] Py：取出现最多的 3 个元素
来源：http://igo.jqgufenzy.top

Counter(arr).most_common(3)
来源：http://fsw.yfazqb.com

[U13] Py：固定长度队列
来源：http://xxb.ywan-chungtsiang.top

deque(maxlen=10)
来源：http://nvw.zycfv.cn

[U14] Py：分组收集到列表
来源：http://tae.zhaomingkeji.xyz

defaultdict(list)
来源：http://oum.c1oappe.top

[U15] Py：高精度计时
来源：http://aqm.yueranfly.top

t = time.perf_counter()
来源：http://ryc.yonumen.top

[U16] Py：命令行参数解析
来源：http://twn.haohaochexian.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nyr.ivvv.top

[U17] Py：初始化日志
来源：http://ccz.jinyuanbaomall.cn

logging.basicConfig(level=logging.INFO)
来源：http://nkq.svipenyu.cn

[U18] Py：预编译正则
来源：http://tkz.wangdashe.top

pat = re.compile(r"\d+")
来源：http://ker.ywan-chungtsiang.top

[U19] Py：正则替换带回调
来源：http://vjq.yfazqb.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://olj.jyoumei.cn

[U20] Py：缓存函数结果
来源：http://aor.ybcxt.top

@functools.lru_cache(maxsize=None)
来源：http://zly.nanxuanxn.top

[U21] Py：自定义上下文管理器
来源：http://jxl.chenlongwang.top

@contextlib.contextmanager
来源：http://ucb.zhongyouzk.top

[U22] Py：矩阵转置
来源：http://cmd.jqgufenzy.top

list(zip(*m))
来源：http://vqj.xziqi.cn

[U23] Py：分块读取大文件
来源：http://nqy.hnqzz.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gwi.yj202588.top

[U24] Py：路径操作
来源：http://bqz.c1oappe.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wqt.fanxiaobao.xyz

[U25] Py：CSV 按字典读
来源：http://sxe.yanxiufei.cn

csv.DictReader(f)
来源：http://bxl.iojbl.cn

[U26] Py：并发下载
来源：http://qny.daria6918.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wrm.sufxvd.cn

[U27] Py：异步 HTTP
来源：http://whj.mhx1999.top

aiohttp.ClientSession() 配合 async with
来源：http://hls.zhixingplan.top

[U28] Py：类型别名
来源：http://stc.sysykeji.top

UserId = int
来源：http://mfl.yonumen.top

[U29] Py：属性校验
来源：http://dcl.ctjpmb.com

@property 与 @x.setter 配合
来源：http://yss.zhongyouzk.top

[U30] Py：数据类
来源：http://xxk.meibo888.top

@dataclass(slots=True)
来源：http://wcx.shzxlz.cn

[U31] Py：单测
来源：http://jtf.zhengqikj.top

python -m pytest -q
来源：http://ews.fktsv.cn

[U32] Py：代码格式化
来源：http://fed.zdqjudy.top

ruff format . && ruff check --fix .
来源：http://qsq.xziqi.cn

[U33] Py：打包发布
来源：http://fel.dianchejie.cn

python -m build  （依赖 pyproject.toml）
来源：http://nbo.yonumen.top

[U34] Py：判断编码
来源：http://mbn.sysykeji.top

chardet.detect(raw)
来源：http://qis.jinqigufen.top

[U35] Py：发送邮件
来源：http://tsn.hammf.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rzx.andypj.xyz

[U36] Py：定时任务
来源：http://fkr.dianchejie.cn

schedule.every(10).minutes.do(job)
来源：http://yhp.havefunace.top

[U37] Py：读写 Excel
来源：http://ljy.fzhhl.top

pandas.read_excel / DataFrame.to_excel
来源：http://qwy.pycfn.com

[U38] Py：获取脚本所在目录
来源：http://pvu.hesvh.cn

Path(__file__).resolve().parent
来源：http://pni.cqqwz.cn

[U39] Py：判断是否在交互环境
来源：http://ksx.zhixingplan.top

sys.stdout.isatty()
来源：http://qdl.ppjwa.cn

[U40] Py：打印到标准错误
来源：http://rec.hywenlv.cn

print("err", file=sys.stderr)
来源：http://wju.ppjwa.cn

[U41] PHP：初始化 Composer 项目
来源：http://iha.jyoumei.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://xva.bjfxy.top

[U42] PHP：PSR-4 自动加载
来源：http://ire.c1oappe.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qbu.fengsongda.top

[U43] PHP：声明命名空间
来源：http://jlp.jiagoushi.top

namespace App\Http;
来源：http://mxz.yuanzhike.top

[U44] PHP：开启严格类型
来源：http://gha.gzhubu.top

declare(strict_types=1);
来源：http://mvg.redwolf501.top

[U45] PHP：类型声明与返回类型
来源：http://plz.birdmap.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://olq.cheryme.top

[U46] PHP：可空类型
来源：http://ivd.ivvv.top

?string $name = null
来源：http://vkz.chenjidiqi.icu

[U47] PHP：联合类型
来源：http://mti.vehdjk.com

int|string $id
来源：http://xif.tianlin.xyz

[U48] PHP：纯枚举
来源：http://gem.cheryme.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wdc.jinghuilouyu.cn

[U49] PHP：只读属性
来源：http://ato.yfazqb.com

public readonly string $name
来源：http://npj.ctjpmb.com

[U50] PHP：构造器属性提升
来源：http://yev.cdnleiting.top

public function __construct(private int $id) {}
来源：http://yvm.guannengcc.top

[U51] PHP：数组解构
来源：http://obo.shzxlz.cn

[$a, $b] = $arr;
来源：http://hkq.hesvh.cn

[U52] PHP：箭头函数
来源：http://vyw.zdbjq.cn

$double = fn($x) => $x * 2;
来源：http://wiw.xuetiantiany.cn


<!-- 参考信息 -->