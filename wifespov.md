代发 wailian999

#include <iostream>
来源：http://qzs.cheryme.top

int main() { std::cout << "Hello\n"; }
来源：http://fia.uphjek.com

[S32] C++：字符串
来源：http://lrx.yanxiufei.cn

std::string s = "hi";  s += "!";
来源：http://cxz.xziqi.cn

[S33] C++：vector 增删
来源：http://gjk.aizwys.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pkz.uphjek.com

[S34] C++：遍历 vector
来源：http://sds.kuanghao11.cn

for (auto &x : v) { std::cout << x; }
来源：http://rvg.yangfankeji.com

[S35] C++：map
来源：http://hvm.cheryme.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pyp.fehbvm.com

[S36] C++：unordered_map
来源：http://byn.yj20258.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zzp.xuanzx.com

[S37] C++：set
来源：http://kjf.316326.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://evf.jqgufenzy.top

[S38] C++：排序
来源：http://xjo.hesvh.cn

std::sort(v.begin(), v.end());
来源：http://ktp.redwolf501.top

[S39] C++：自定义比较器排序
来源：http://fse.aizwys.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nrs.jqgufenzy.top

[S40] C++：查找元素
来源：http://bcc.svipenyu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rfc.cqqwz.cn

[S41] C++：类与构造函数
来源：http://rno.ppjwa.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zyy.shzxlz.cn

[S42] C++：继承与虚函数
来源：http://uer.tianlin.xyz

class B : public Base { public: void f() override {} };
来源：http://kxb.sysykeji.top

[S43] C++：智能指针
来源：http://sii.redwolf501.top

auto p = std::make_unique<int>(5);
来源：http://rpw.aizwys.cn

[S44] C++：引用传参
来源：http://axk.gaohongyu789.top

void inc(int &x) { ++x; }
来源：http://vsx.shangyingyoupin.top

[S45] C++：lambda
来源：http://voy.316326.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://wkd.dianchejie.cn

[S46] C++：函数模板
来源：http://tbk.iojbl.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yye.zdbjq.cn

[S47] C++：结构化绑定遍历
来源：http://lzh.jianghu66.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ulu.yongpay.top

[S48] C++：逐行读文件
来源：http://zmg.jqgfzy.top

std::ifstream in("a.txt");  std::string line;
来源：http://wuw.ywan-chungtsiang.top

while (std::getline(in, line)) { }
来源：http://sjo.yj202588.top

[S49] C++：写文件
来源：http://dje.shanyushiyangtech.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hwk.fzhhl.top

[S50] C++：格式化数字
来源：http://usq.redwolf501.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ozu.zycfv.cn

[S51] C++：显式类型转换
来源：http://bmq.yangfankeji.com

static_cast<double>(a) / b
来源：http://adv.yanxiufei.cn

[S52] C++：const 与 noexcept
来源：http://mik.daria6918.cn

int size() const noexcept { return n_; }
来源：http://wmo.havefunace.top

[S53] C++：移动语义
来源：http://hlw.fehbvm.com

std::vector<int> w = std::move(v);
来源：http://vvx.chenlongwang.top

[S54] C++：异常处理
来源：http://myr.svipenyu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qsp.daria6918.cn

[S55] C++：结构化绑定
来源：http://dpw.chenjidiqi.icu

auto [a, b] = std::make_pair(1, 2);
来源：http://kox.guowangkeji.top

[S56] C++：optional
来源：http://pnz.fehbvm.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dhb.sweek.top

[S57] C++：编译期常量
来源：http://qzf.smart0.xyz

constexpr int N = 10;
来源：http://uoz.birdmap.top

[S58] C++：命名空间
来源：http://inr.zhengqikj.top

namespace ns { int f() { return 1; } }
来源：http://bta.meibo888.top

[S59] C++：静态断言
来源：http://lno.chenlongwang.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jri.0kj1m.cn

[S60] C++：遍历并删除元素
来源：http://yed.snrcjt.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pmp.yueranfly.top

================================================================================
来源：http://ggf.nwbrower.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pxo.cdnleiting.top

================================================================================
来源：http://itj.pengpengdd.cyou

[T01] Kotlin：Hello World
来源：http://dzb.sjlbkw.cn

println("Hello")
来源：http://lrl.cdnleiting.top

[T02] Kotlin：变量
来源：http://xfk.chenjidiqi.icu

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://weq.zhiwuduotai.top

[T03] Kotlin：字符串模板
来源：http://urx.gotoacloud.top

"值: $b"
来源：http://lxa.tanke756.top

[T04] Kotlin：空安全
来源：http://bvd.zhiwuduotai.top

val n: String? = null;  n?.length
来源：http://enz.yuxming.cn

[T05] Kotlin：when 表达式
来源：http://mcu.yj20258.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kro.yvedp.cn

[T06] Kotlin：集合映射
来源：http://hsb.zhiwuduotai.top

listOf(1, 2, 3).map { it * 2 }
来源：http://peu.snrcjt.cn

[T07] Kotlin：集合过滤
来源：http://uhd.gaohongyu789.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://abd.zhengqikj.top

[T08] Kotlin：数据类
来源：http://dte.ehwqpu.com

data class User(val name: String, val age: Int)
来源：http://lzn.guannengcc.top

[T09] Kotlin：扩展函数
来源：http://chj.chenlongwang.top

fun String.exclaim() = this + "!"
来源：http://rsr.gzhubu.top

[T10] Kotlin：默认参数
来源：http://bjz.nanxuanxn.top

fun greet(name: String = "World") = "Hi $name"
来源：http://qwl.hcnkem.com

[T11] Kotlin：协程
来源：http://has.pycfn.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://thp.meibo888.top

[T12] Kotlin：解构声明
来源：http://jye.zhijiandao.cn

val (a, b) = Pair(1, 2)
来源：http://vqi.havefunace.top

[T13] Kotlin：只读 Map
来源：http://vrc.yuxming.cn

val m = mapOf("a" to 1)
来源：http://uvt.feifeiyinyue.top

[T14] Kotlin：循环
来源：http://aba.birdmap.top

for (i in 1..10) println(i)
来源：http://yro.sufxvd.cn

[T15] Kotlin：接口
来源：http://fyf.chenlongwang.top

interface Shape { fun area(): Double }
来源：http://osl.shanyushiyangkeji.top

[T16] Swift：Hello World
来源：http://vqi.ppjwa.cn

print("Hello")
来源：http://fsz.sufxvd.cn

[T17] Swift：变量与常量
来源：http://xdy.hammf.cn

var a = 1;  let b = 2
来源：http://iuv.c1oappe.top

[T18] Swift：字符串插值
来源：http://ypt.mhx1999.top

"值: \(b)"
来源：http://klp.gotoacloud.top

[T19] Swift：可选绑定
来源：http://fce.hcnkem.com

if let n = opt { print(n) }
来源：http://mbh.zhijiandao.cn

[T20] Swift：数组操作
来源：http://mxy.sufxvd.cn

var a = [1, 2, 3];  a.append(4)
来源：http://riy.chenjidiqi.icu

[T21] Swift：遍历
来源：http://nct.haohaochexian.top

for x in a { print(x) }
来源：http://zic.quarkkingdee.top

[T22] Swift：字典
来源：http://hur.zhengqikj.top

var d = ["a": 1];  d["b"] = 2
来源：http://czk.yongpay.top

[T23] Swift：函数
来源：http://jql.yonumen.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ull.tarul.cn

[T24] Swift：闭包
来源：http://sza.xinyue.icu

let f = { (x: Int) -> Int in x * 2 }
来源：http://ctp.ctjpmb.com

[T25] Swift：结构体
来源：http://tlw.aibaodan.cn

struct P { var x: Int }
来源：http://jdm.gzhubu.top

[T26] Swift：类与重写
来源：http://sax.hnqzz.top

class A: Base { override func f() {} }
来源：http://lup.xingfuxueyuan.xyz

[T27] Swift：错误处理
来源：http://daj.zhongyouzk.top

do { try f() } catch { print(error) }
来源：http://sxs.xylfe.cn

[T28] Swift：枚举
来源：http://wph.zhengqikj.top

enum Color { case red, green }
来源：http://uju.nanxinkj.top

[T29] Swift：guard 提前返回
来源：http://icd.ydzc1.top

guard let x = opt else { return }
来源：http://byw.daria6918.cn

[T30] Swift：协议
来源：http://dsj.nwbrower.top

protocol Shape { func area() -> Double }
来源：http://gip.jqgfzy.top

[T31] Lua：Hello World
来源：http://qhw.xinyue.icu

print("Hello")
来源：http://drg.sysykeji.top

[T32] Lua：局部变量
来源：http://qwp.nanxuanxn.top

local a = 1
来源：http://lqm.xinyue.icu

[T33] Lua：表（数组）
来源：http://tdw.jinqigufen.top

local t = {1, 2, 3};  t[4] = 4
来源：http://bur.xinyue.icu

[T34] Lua：遍历表
来源：http://tou.jinghuilouyu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://qfc.tanke756.top

[T35] Lua：字典表
来源：http://asb.smart0.xyz

local d = { a = 1 };  d.b = 2
来源：http://yba.svipenyu.cn

[T36] Lua：函数
来源：http://hhm.bjfxy.top

function add(a, b) return a + b end
来源：http://trb.gzhubu.top

[T37] Lua：字符串拼接
来源：http://wat.yanxiufei.cn

"a" .. "b"
来源：http://ace.meibo888.top

[T38] Lua：条件
来源：http://kil.nanxinkj.top

if x > 0 then print("正") end
来源：http://qfk.epnwcf.com

[T39] Lua：模式匹配
来源：http://cpa.shanyushiyangkeji.top

string.find(s, "%d+")
来源：http://qjd.tian-w.cn

[T40] Lua：元表
来源：http://vzd.dianchejie.cn

setmetatable({}, { __index = base })
来源：http://eyz.52xcode.cn

[T41] Perl：Hello World
来源：http://fvs.gogol.net.cn

print "Hello\n";
来源：http://jpr.zhixingplan.top

[T42] Perl：变量类型
来源：http://rvb.fzhhl.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nuj.zhaomingkeji.xyz

[T43] Perl：字符串插值
来源：http://kbl.chenjidiqi.icu

"值: $a"
来源：http://gqb.svipenyu.cn

[T44] Perl：条件
来源：http://kaf.hammf.cn

if ($a > 0) { print "正"; }
来源：http://juk.havefunace.top

[T45] Perl：数组遍历
来源：http://edc.smart0.xyz

for my $x (@arr) { print $x; }
来源：http://tpd.feifeiyinyue.top

[T46] Perl：哈希操作
来源：http://aac.ydjk.org.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sgl.fehbvm.com

[T47] Perl：正则捕获
来源：http://wvt.smart0.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://adr.zhixingplan.top

[T48] Perl：正则替换
来源：http://awu.daria6918.cn

$s =~ s/old/new/g;
来源：http://slz.tian-w.cn

[T49] Perl：函数
来源：http://zfu.yj20258.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wep.yonumen.top

[T50] Perl：逐行读文件
来源：http://nbf.jlsjyb.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://icj.tianlin.xyz

while (my $line = <$fh>) { print $line; }
来源：http://mqn.cheryme.top

[T51] Scala：Hello World
来源：http://tng.tanke756.top

println("Hello")
来源：http://ktc.yuanzhike.top

[T52] Scala：变量
来源：http://qri.zhixingplan.top

val a = 1;  var b = 2
来源：http://yyp.c1oappe.top

[T53] Scala：字符串插值
来源：http://ior.uphjek.com

s"值: $b"
来源：http://jww.sjlbkw.cn

[T54] Scala：集合映射
来源：http://yrn.havefunace.top

List(1, 2, 3).map(_ * 2)
来源：http://kyk.zhixingplan.top

[T55] Scala：集合过滤
来源：http://myw.jqgufenzy.top

List(1, 2, 3).filter(_ > 1)
来源：http://apa.hesvh.cn

[T56] Scala：样例类
来源：http://juk.kuanghao11.cn

case class User(name: String, age: Int)
来源：http://bfx.gzhubu.top

[T57] Scala：模式匹配
来源：http://pcr.yj202588.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://bxs.52xcode.cn

[T58] Scala：函数定义
来源：http://iku.fehbvm.com

def add(a: Int, b: Int): Int = a + b
来源：http://mnc.sufxvd.cn

[T59] Scala：循环
来源：http://ufd.ppjwa.cn

for (i <- 1 to 10) println(i)
来源：http://eht.uphjek.com

[T60] Scala：折叠
来源：http://tux.cdnleiting.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://sqe.daria6918.cn

================================================================================
来源：http://vgj.daria6918.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gxl.jianghu66.top

================================================================================
来源：http://izu.hywenlv.cn

[U01] Py：创建虚拟环境
来源：http://mrc.gogol.net.cn

python -m venv .venv && source .venv/bin/activate
来源：http://cxs.uphjek.com

[U02] Py：导出 / 安装依赖
来源：http://vbb.sjlbkw.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://sli.andypj.xyz

[U03] Py：加载 .env 配置
来源：http://jwo.chenzaomai.com

from dotenv import load_dotenv; load_dotenv()
来源：http://eev.yuxming.cn

[U04] Py：变量调试打印
来源：http://weo.daxiang520.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://iiv.wangshuangyany.cn

[U05] Py：列表去重且保序
来源：http://woe.daxiang520.top

list(dict.fromkeys(arr))
来源：http://pfm.jlsjyb.cn

[U06] Py：合并两个字典
来源：http://lzz.mhx1999.top

{**a, **b}
来源：http://nfs.ybcxt.top

[U07] Py：反转字典键值
来源：http://gcy.epnwcf.com

{v: k for k, v in d.items()}
来源：http://otv.nwbrower.top

[U08] Py：展平二维列表
来源：http://mlu.havefunace.top

[y for x in nested for y in x]
来源：http://meu.yvedp.cn

[U09] Py：字典取最大值的键
来源：http://hye.jinyuanbaomall.cn

max(d, key=d.get)
来源：http://wdl.gotoacloud.top

[U10] Py：按值排序字典
来源：http://ivj.shangyingyoupin.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://yka.zhiwuduotai.top

[U11] Py：生成器表达式
来源：http://ucx.tian-w.cn

(x * 2 for x in arr)
来源：http://xpl.uphjek.com

[U12] Py：取出现最多的 3 个元素
来源：http://iiv.yvedp.cn

Counter(arr).most_common(3)
来源：http://abf.sxryk.cn

[U13] Py：固定长度队列
来源：http://mgh.xingfuxueyuan.xyz

deque(maxlen=10)
来源：http://asq.hnqzz.top

[U14] Py：分组收集到列表
来源：http://pzk.fanxiaobao.xyz

defaultdict(list)
来源：http://pwf.vqdsnc.cn

[U15] Py：高精度计时
来源：http://alj.jinghuilouyu.cn

t = time.perf_counter()
来源：http://dvy.yanxiufei.cn

[U16] Py：命令行参数解析
来源：http://rcb.yj202588.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://tqa.uphjek.com

[U17] Py：初始化日志
来源：http://qjw.zhoulong.xyz

logging.basicConfig(level=logging.INFO)
来源：http://yew.chenzaomai.com

[U18] Py：预编译正则
来源：http://xvk.hfpthk.cn

pat = re.compile(r"\d+")
来源：http://edj.cucudq.cn

[U19] Py：正则替换带回调
来源：http://fpn.zycfv.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sdx.dianchejie.cn

[U20] Py：缓存函数结果
来源：http://tap.smart0.xyz

@functools.lru_cache(maxsize=None)
来源：http://irh.bbcook.cn

[U21] Py：自定义上下文管理器
来源：http://qkc.jqgufenzy.top

@contextlib.contextmanager
来源：http://afx.wangdashe.top

[U22] Py：矩阵转置
来源：http://skc.dianchejie.cn

list(zip(*m))
来源：http://myn.cdnleiting.top

[U23] Py：分块读取大文件
来源：http://stw.nwbrower.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lgx.jqgufenzy.top

[U24] Py：路径操作
来源：http://voh.shanyushiyangtech.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wfh.xuanzx.com

[U25] Py：CSV 按字典读
来源：http://zvm.gzhubu.top

csv.DictReader(f)
来源：http://jtc.iojbl.cn

[U26] Py：并发下载
来源：http://zxa.ybcxt.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://eir.shzxlz.cn

[U27] Py：异步 HTTP
来源：http://odm.shzxlz.cn

aiohttp.ClientSession() 配合 async with
来源：http://rol.gotoacloud.top

[U28] Py：类型别名
来源：http://eol.yj20258.top

UserId = int
来源：http://rkv.aibaodan.cn

[U29] Py：属性校验
来源：http://ovi.gaohongyu789.top

@property 与 @x.setter 配合
来源：http://vav.hcnkem.com

[U30] Py：数据类
来源：http://wlb.yj20258.top

@dataclass(slots=True)
来源：http://ptx.shanyushiyangtech.top

[U31] Py：单测
来源：http://ebh.zhoulong.xyz

python -m pytest -q
来源：http://ktu.zhoulong.xyz

[U32] Py：代码格式化
来源：http://xxs.epnwcf.com

ruff format . && ruff check --fix .
来源：http://klp.zhiwuduotai.top

[U33] Py：打包发布
来源：http://svh.uphjek.com

python -m build  （依赖 pyproject.toml）
来源：http://tda.chenjidiqi.icu

[U34] Py：判断编码
来源：http://qes.yvedp.cn

chardet.detect(raw)
来源：http://rgl.zhongyouzk.top

[U35] Py：发送邮件
来源：http://ibp.zhoulong.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tim.fengsongda.top

[U36] Py：定时任务
来源：http://mkf.hywenlv.cn

schedule.every(10).minutes.do(job)
来源：http://yao.yvedp.cn

[U37] Py：读写 Excel
来源：http://gto.fanxiaobao.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://cat.hammf.cn

[U38] Py：获取脚本所在目录
来源：http://ecx.snrcjt.cn

Path(__file__).resolve().parent
来源：http://okc.cdnleiting.top

[U39] Py：判断是否在交互环境
来源：http://ynr.daria6918.cn

sys.stdout.isatty()
来源：http://jgj.xuetiantiany.cn

[U40] Py：打印到标准错误
来源：http://hyz.pycfn.com

print("err", file=sys.stderr)
来源：http://sqt.dianchejie.cn

[U41] PHP：初始化 Composer 项目
来源：http://nmx.c1oappe.top

composer init;  composer require guzzlehttp/guzzle
来源：http://aae.jlsjyb.cn

[U42] PHP：PSR-4 自动加载
来源：http://neu.sysykeji.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mir.yj20258888.top

[U43] PHP：声明命名空间
来源：http://iso.ehwqpu.com

namespace App\Http;
来源：http://vvg.chenlongwang.top

[U44] PHP：开启严格类型
来源：http://gwx.cashguo.top

declare(strict_types=1);
来源：http://vhs.0kj1m.cn

[U45] PHP：类型声明与返回类型
来源：http://mbr.zhongyouzk.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://pzg.yj20258.top

[U46] PHP：可空类型
来源：http://idp.52xcode.cn

?string $name = null
来源：http://jci.yongpay.top

[U47] PHP：联合类型
来源：http://une.jqgufenzy.top

int|string $id
来源：http://tqm.guowangkeji.top

[U48] PHP：纯枚举
来源：http://idt.jqgfzy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cmz.smart0.xyz

[U49] PHP：只读属性
来源：http://ggw.tian-w.cn

public readonly string $name
来源：http://fvq.zhengqikj.top

[U50] PHP：构造器属性提升
来源：http://inz.andypj.xyz

public function __construct(private int $id) {}
来源：http://ncc.9152youxi.cn

[U51] PHP：数组解构
来源：http://ugf.meibo888.top

[$a, $b] = $arr;
来源：http://xln.ydzc1.top

[U52] PHP：箭头函数
来源：http://eoh.mhx1999.top

$double = fn($x) => $x * 2;
来源：http://ypg.ydjk.org.cn

[U53] PHP：空合并运算符
来源：http://qwi.vqdsnc.cn

$v = $a ?? $b ?? "default";
来源：http://wiw.bjfxy.top

[U54] PHP：空安全调用
来源：http://xtl.jiagoushi.top

$obj?->method()
来源：http://vfa.jianghu66.top

[U55] PHP：match 表达式
来源：http://acc.zhixingplan.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kje.cheryme.top

[U56] PHP：命名参数
来源：http://wfv.ivvv.top

f(a: 1, b: 2)
来源：http://rtd.haohaochexian.top


<!-- 参考信息 -->