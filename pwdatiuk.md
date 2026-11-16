代发 wailian999

[S33] C++：vector 增删
来源：http://nvx.xziqi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://egj.zdbjq.cn

[S34] C++：遍历 vector
来源：http://hkr.zdbjq.cn

for (auto &x : v) { std::cout << x; }
来源：http://fat.jinqigufen.top

[S35] C++：map
来源：http://fuj.yonumen.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vla.fktsv.cn

[S36] C++：unordered_map
来源：http://wko.epnwcf.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tsk.hcnkem.com

[S37] C++：set
来源：http://beb.zhengqikj.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pyg.fengsongda.top

[S38] C++：排序
来源：http://gqg.xziqi.cn

std::sort(v.begin(), v.end());
来源：http://ric.ivvv.top

[S39] C++：自定义比较器排序
来源：http://hwi.zhijiandao.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://raa.aizwys.cn

[S40] C++：查找元素
来源：http://yyw.cqqwz.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wag.shzxlz.cn

[S41] C++：类与构造函数
来源：http://neh.yvedp.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://iql.cheryme.top

[S42] C++：继承与虚函数
来源：http://ofb.jyoumei.cn

class B : public Base { public: void f() override {} };
来源：http://nua.sufxvd.cn

[S43] C++：智能指针
来源：http://wzr.mhx1999.top

auto p = std::make_unique<int>(5);
来源：http://yij.yanxiufei.cn

[S44] C++：引用传参
来源：http://ums.sjlbkw.cn

void inc(int &x) { ++x; }
来源：http://snl.ybcxt.top

[S45] C++：lambda
来源：http://jsg.hfpthk.cn

auto add = [](int a, int b) { return a + b; };
来源：http://jdq.shangyingyoupin.top

[S46] C++：函数模板
来源：http://wgl.zhongyouzk.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wav.yvedp.cn

[S47] C++：结构化绑定遍历
来源：http://yzt.cucudq.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pwh.ivvv.top

[S48] C++：逐行读文件
来源：http://dtl.shangyingyoupin.top

std::ifstream in("a.txt");  std::string line;
来源：http://hup.cucudq.cn

while (std::getline(in, line)) { }
来源：http://tfh.dianchejie.cn

[S49] C++：写文件
来源：http://avc.zhoulong.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nsg.dianchejie.cn

[S50] C++：格式化数字
来源：http://pea.uphjek.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xsn.hammf.cn

[S51] C++：显式类型转换
来源：http://baf.wangdashe.top

static_cast<double>(a) / b
来源：http://ymk.meibo888.top

[S52] C++：const 与 noexcept
来源：http://okr.gotoacloud.top

int size() const noexcept { return n_; }
来源：http://ogv.sxryk.cn

[S53] C++：移动语义
来源：http://wzv.jlsjyb.cn

std::vector<int> w = std::move(v);
来源：http://uwt.yonumen.top

[S54] C++：异常处理
来源：http://flq.gotoacloud.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://uso.yonumen.top

[S55] C++：结构化绑定
来源：http://hps.dianchejie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://pwz.yuxming.cn

[S56] C++：optional
来源：http://xih.ivvv.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kbl.xingfuxueyuan.xyz

[S57] C++：编译期常量
来源：http://yln.hnqzz.top

constexpr int N = 10;
来源：http://gbj.yongpay.top

[S58] C++：命名空间
来源：http://tqv.xingfuxueyuan.xyz

namespace ns { int f() { return 1; } }
来源：http://wrx.birdmap.top

[S59] C++：静态断言
来源：http://xdg.gotoacloud.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nok.tarul.cn

[S60] C++：遍历并删除元素
来源：http://mdj.xuetiantiany.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tad.yangfankeji.com

================================================================================
来源：http://mlz.jqgfzy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tbq.bbcook.cn

================================================================================
来源：http://seg.kuanghao11.cn

[T01] Kotlin：Hello World
来源：http://dvd.gzhubu.top

println("Hello")
来源：http://ggq.daria6918.cn

[T02] Kotlin：变量
来源：http://skp.zhijiandao.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://epi.316326.xyz

[T03] Kotlin：字符串模板
来源：http://ubx.sufxvd.cn

"值: $b"
来源：http://zpn.cashguo.top

[T04] Kotlin：空安全
来源：http://khp.nanxinkj.top

val n: String? = null;  n?.length
来源：http://xpr.hnqzz.top

[T05] Kotlin：when 表达式
来源：http://gnv.jqgfzy.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ezm.9152youxi.cn

[T06] Kotlin：集合映射
来源：http://jve.ywan-chungtsiang.top

listOf(1, 2, 3).map { it * 2 }
来源：http://hii.zhiwuduotai.top

[T07] Kotlin：集合过滤
来源：http://zbn.daria6918.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ppa.pycfn.com

[T08] Kotlin：数据类
来源：http://pls.zhongyouzk.top

data class User(val name: String, val age: Int)
来源：http://fqs.zhaomingkeji.xyz

[T09] Kotlin：扩展函数
来源：http://twd.pengpengdd.cyou

fun String.exclaim() = this + "!"
来源：http://xek.jianghu66.top

[T10] Kotlin：默认参数
来源：http://ctg.hesvh.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://dew.sxryk.cn

[T11] Kotlin：协程
来源：http://scj.ehwqpu.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://bpa.meibo888.top

[T12] Kotlin：解构声明
来源：http://oxu.shangyingyoupin.top

val (a, b) = Pair(1, 2)
来源：http://xnq.yj20258888.top

[T13] Kotlin：只读 Map
来源：http://yfg.hesvh.cn

val m = mapOf("a" to 1)
来源：http://fdd.nanxinkj.top

[T14] Kotlin：循环
来源：http://nmj.zhengqikj.top

for (i in 1..10) println(i)
来源：http://raq.yangfankeji.com

[T15] Kotlin：接口
来源：http://tpq.zdqjudy.top

interface Shape { fun area(): Double }
来源：http://lpj.yueranfly.top

[T16] Swift：Hello World
来源：http://adf.birdmap.top

print("Hello")
来源：http://lnt.xingfuxueyuan.xyz

[T17] Swift：变量与常量
来源：http://plz.ydzc1.top

var a = 1;  let b = 2
来源：http://yuu.cashguo.top

[T18] Swift：字符串插值
来源：http://jhr.tanke756.top

"值: \(b)"
来源：http://rft.uphjek.com

[T19] Swift：可选绑定
来源：http://wxz.jinghuilouyu.cn

if let n = opt { print(n) }
来源：http://ovm.zhaomingkeji.xyz

[T20] Swift：数组操作
来源：http://clr.shanyushiyangkeji.top

var a = [1, 2, 3];  a.append(4)
来源：http://fjt.gotoacloud.top

[T21] Swift：遍历
来源：http://uno.andypj.xyz

for x in a { print(x) }
来源：http://suu.shangyingyoupin.top

[T22] Swift：字典
来源：http://ldq.hysaishi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://iwu.hongshengwenyu.top

[T23] Swift：函数
来源：http://iva.zhijiandao.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ipp.0kj1m.cn

[T24] Swift：闭包
来源：http://vjc.guowangkeji.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ezx.pengpengdd.cyou

[T25] Swift：结构体
来源：http://vbq.shanyushiyangtech.top

struct P { var x: Int }
来源：http://vkv.dianchejie.cn

[T26] Swift：类与重写
来源：http://anq.sjlbkw.cn

class A: Base { override func f() {} }
来源：http://jhe.zhongyouzk.top

[T27] Swift：错误处理
来源：http://atu.52xcode.cn

do { try f() } catch { print(error) }
来源：http://ogm.yfazqb.com

[T28] Swift：枚举
来源：http://ywm.zhoulong.xyz

enum Color { case red, green }
来源：http://mbp.sufxvd.cn

[T29] Swift：guard 提前返回
来源：http://cpk.fehbvm.com

guard let x = opt else { return }
来源：http://vqe.aizwys.cn

[T30] Swift：协议
来源：http://vri.fktsv.cn

protocol Shape { func area() -> Double }
来源：http://bdg.nanxuanxn.top

[T31] Lua：Hello World
来源：http://cte.yvedp.cn

print("Hello")
来源：http://ooi.shuidangran.top

[T32] Lua：局部变量
来源：http://ayp.ybcxt.top

local a = 1
来源：http://ftr.xylfe.cn

[T33] Lua：表（数组）
来源：http://hdy.mhx1999.top

local t = {1, 2, 3};  t[4] = 4
来源：http://chb.sjlbkw.cn

[T34] Lua：遍历表
来源：http://gso.uphjek.com

for i, v in ipairs(t) do print(i, v) end
来源：http://dzd.havefunace.top

[T35] Lua：字典表
来源：http://ycj.cheryme.top

local d = { a = 1 };  d.b = 2
来源：http://wwf.ydjk.org.cn

[T36] Lua：函数
来源：http://tbw.jinqigfzy.top

function add(a, b) return a + b end
来源：http://afh.tanke756.top

[T37] Lua：字符串拼接
来源：http://jyj.wangshuangyany.cn

"a" .. "b"
来源：http://jmc.ywan-chungtsiang.top

[T38] Lua：条件
来源：http://yco.svipenyu.cn

if x > 0 then print("正") end
来源：http://ett.shanyushiyangkeji.top

[T39] Lua：模式匹配
来源：http://iot.vqdsnc.cn

string.find(s, "%d+")
来源：http://bdh.aizwys.cn

[T40] Lua：元表
来源：http://pye.shangyingyoupin.top

setmetatable({}, { __index = base })
来源：http://avl.tanke756.top

[T41] Perl：Hello World
来源：http://ugo.sysykeji.top

print "Hello\n";
来源：http://bmp.nanxuanxn.top

[T42] Perl：变量类型
来源：http://iqu.zycfv.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://sod.jqgufenzy.top

[T43] Perl：字符串插值
来源：http://hcc.nanxuanxn.top

"值: $a"
来源：http://chx.bbcook.cn

[T44] Perl：条件
来源：http://erf.bjfxy.top

if ($a > 0) { print "正"; }
来源：http://xdt.tanke756.top

[T45] Perl：数组遍历
来源：http://otg.gzhubu.top

for my $x (@arr) { print $x; }
来源：http://lmq.xziqi.cn

[T46] Perl：哈希操作
来源：http://zcz.haohaochexian.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sbv.uphjek.com

[T47] Perl：正则捕获
来源：http://vdu.pengpengdd.cyou

if ($s =~ /(\d+)/) { print $1; }
来源：http://blf.xuetiantiany.cn

[T48] Perl：正则替换
来源：http://uvu.jinyuanbaomall.cn

$s =~ s/old/new/g;
来源：http://deb.tian-w.cn

[T49] Perl：函数
来源：http://vbq.daria6918.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kkn.shuidangran.top

[T50] Perl：逐行读文件
来源：http://vrl.jiagoushi.top

open my $fh, "<", "a.txt" or die $!;
来源：http://cqh.hysaishi.cn

while (my $line = <$fh>) { print $line; }
来源：http://qbg.ehwqpu.com

[T51] Scala：Hello World
来源：http://jdq.epnwcf.com

println("Hello")
来源：http://zhv.zdbjq.cn

[T52] Scala：变量
来源：http://xoo.vehdjk.com

val a = 1;  var b = 2
来源：http://dlp.wangshuangyany.cn

[T53] Scala：字符串插值
来源：http://ybk.ydjk.org.cn

s"值: $b"
来源：http://adb.ydjk.org.cn

[T54] Scala：集合映射
来源：http://ewu.bjfxy.top

List(1, 2, 3).map(_ * 2)
来源：http://erf.ppjwa.cn

[T55] Scala：集合过滤
来源：http://yrp.guowangkeji.top

List(1, 2, 3).filter(_ > 1)
来源：http://hpt.zhiwuduotai.top

[T56] Scala：样例类
来源：http://oid.jqgfzy.top

case class User(name: String, age: Int)
来源：http://pat.mhx1999.top

[T57] Scala：模式匹配
来源：http://hzg.ctjpmb.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://atg.zhijiandao.cn

[T58] Scala：函数定义
来源：http://ajx.hongshengwenyu.top

def add(a: Int, b: Int): Int = a + b
来源：http://zqf.yj20258.top

[T59] Scala：循环
来源：http://tub.ywan-chungtsiang.top

for (i <- 1 to 10) println(i)
来源：http://udn.yfazqb.com

[T60] Scala：折叠
来源：http://uyp.cdnleiting.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wzq.wangshuangyany.cn

================================================================================
来源：http://tyf.gotoacloud.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://etb.yueranfly.top

================================================================================
来源：http://iip.zdqjudy.top

[U01] Py：创建虚拟环境
来源：http://esj.aibaodan.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qga.yongpay.top

[U02] Py：导出 / 安装依赖
来源：http://ajj.zhiwuduotai.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lgy.gogol.net.cn

[U03] Py：加载 .env 配置
来源：http://wlv.gogol.net.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xld.xuetiantiany.cn

[U04] Py：变量调试打印
来源：http://bmq.meibo888.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://cra.nanxinkj.top

[U05] Py：列表去重且保序
来源：http://lvr.ydzc1.top

list(dict.fromkeys(arr))
来源：http://zsu.yj20258888.top

[U06] Py：合并两个字典
来源：http://myw.jiagoushi.top

{**a, **b}
来源：http://oig.shuidangran.top

[U07] Py：反转字典键值
来源：http://eyy.gotoacloud.top

{v: k for k, v in d.items()}
来源：http://ufy.zhoulong.xyz

[U08] Py：展平二维列表
来源：http://lzi.316326.xyz

[y for x in nested for y in x]
来源：http://gra.xuanzx.com

[U09] Py：字典取最大值的键
来源：http://ysu.uphjek.com

max(d, key=d.get)
来源：http://uhy.svipenyu.cn

[U10] Py：按值排序字典
来源：http://bmu.yongpay.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jkl.wangshuangyany.cn

[U11] Py：生成器表达式
来源：http://dfe.svipenyu.cn

(x * 2 for x in arr)
来源：http://ddt.cucudq.cn

[U12] Py：取出现最多的 3 个元素
来源：http://uhw.quarkkingdee.top

Counter(arr).most_common(3)
来源：http://jfb.aibaodan.cn

[U13] Py：固定长度队列
来源：http://bct.fktsv.cn

deque(maxlen=10)
来源：http://uej.sjlbkw.cn

[U14] Py：分组收集到列表
来源：http://fau.svipenyu.cn

defaultdict(list)
来源：http://qqo.yangfankeji.com

[U15] Py：高精度计时
来源：http://dnz.guowangkeji.top

t = time.perf_counter()
来源：http://gnl.birdmap.top

[U16] Py：命令行参数解析
来源：http://jnf.hesvh.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rio.andypj.xyz

[U17] Py：初始化日志
来源：http://bly.shzxlz.cn

logging.basicConfig(level=logging.INFO)
来源：http://kqq.iojbl.cn

[U18] Py：预编译正则
来源：http://oez.pengpengdd.cyou

pat = re.compile(r"\d+")
来源：http://cnr.yj20258.top

[U19] Py：正则替换带回调
来源：http://hzq.redwolf501.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kxm.hfpthk.cn

[U20] Py：缓存函数结果
来源：http://ukx.jinqigufen.top

@functools.lru_cache(maxsize=None)
来源：http://sjt.tianlin.xyz

[U21] Py：自定义上下文管理器
来源：http://wvy.gaohongyu789.top

@contextlib.contextmanager
来源：http://djj.snrcjt.cn

[U22] Py：矩阵转置
来源：http://byf.meibo888.top

list(zip(*m))
来源：http://ctu.shuidangran.top

[U23] Py：分块读取大文件
来源：http://edv.svipenyu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rkf.jlsjyb.cn

[U24] Py：路径操作
来源：http://ksx.hfpthk.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jqd.meibo888.top

[U25] Py：CSV 按字典读
来源：http://bnw.jqgufenzy.top

csv.DictReader(f)
来源：http://nju.yvedp.cn

[U26] Py：并发下载
来源：http://gur.vqdsnc.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pjh.dashuyun.cn

[U27] Py：异步 HTTP
来源：http://pfh.cdnleiting.top

aiohttp.ClientSession() 配合 async with
来源：http://icw.yongpay.top

[U28] Py：类型别名
来源：http://dar.sufxvd.cn

UserId = int
来源：http://eqb.guannengcc.top

[U29] Py：属性校验
来源：http://sgm.jiagoushi.top

@property 与 @x.setter 配合
来源：http://ugs.yj20258888.top

[U30] Py：数据类
来源：http://chf.jiagoushi.top

@dataclass(slots=True)
来源：http://yil.jinyuanbaomall.cn

[U31] Py：单测
来源：http://jly.zdbjq.cn

python -m pytest -q
来源：http://uvj.andypj.xyz

[U32] Py：代码格式化
来源：http://hwy.fanxiaobao.xyz

ruff format . && ruff check --fix .
来源：http://kei.yvedp.cn

[U33] Py：打包发布
来源：http://vat.ybcxt.top

python -m build  （依赖 pyproject.toml）
来源：http://thw.jinqigufen.top

[U34] Py：判断编码
来源：http://ffp.iojbl.cn

chardet.detect(raw)
来源：http://cvp.xylfe.cn

[U35] Py：发送邮件
来源：http://iey.yonumen.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fds.zhengqikj.top

[U36] Py：定时任务
来源：http://azv.cqqwz.cn

schedule.every(10).minutes.do(job)
来源：http://dba.guannengcc.top

[U37] Py：读写 Excel
来源：http://ejc.xuanzx.com

pandas.read_excel / DataFrame.to_excel
来源：http://zjg.ybcxt.top

[U38] Py：获取脚本所在目录
来源：http://xaw.fehbvm.com

Path(__file__).resolve().parent
来源：http://pvy.shangyingyoupin.top

[U39] Py：判断是否在交互环境
来源：http://ral.shangyingyoupin.top

sys.stdout.isatty()
来源：http://zvb.yj202588.top

[U40] Py：打印到标准错误
来源：http://pyh.zdqjudy.top

print("err", file=sys.stderr)
来源：http://glo.aizwys.cn

[U41] PHP：初始化 Composer 项目
来源：http://tko.aizwys.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://duq.316326.xyz

[U42] PHP：PSR-4 自动加载
来源：http://kkj.pycfn.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cbs.kuanghao11.cn

[U43] PHP：声明命名空间
来源：http://pkg.pengpengdd.cyou

namespace App\Http;
来源：http://ynw.shuidangran.top

[U44] PHP：开启严格类型
来源：http://bmb.tanke756.top

declare(strict_types=1);
来源：http://iha.yangfankeji.com

[U45] PHP：类型声明与返回类型
来源：http://xhu.hcnkem.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://byq.birdmap.top

[U46] PHP：可空类型
来源：http://rbw.zhixingplan.top

?string $name = null
来源：http://sbd.nwbrower.top

[U47] PHP：联合类型
来源：http://yup.sufxvd.cn

int|string $id
来源：http://dhn.chenlongwang.top

[U48] PHP：纯枚举
来源：http://zmo.quarkkingdee.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ekp.ivvv.top

[U49] PHP：只读属性
来源：http://ljq.yonumen.top

public readonly string $name
来源：http://cny.tanke756.top

[U50] PHP：构造器属性提升
来源：http://fzm.birdmap.top

public function __construct(private int $id) {}
来源：http://rqk.sweek.top

[U51] PHP：数组解构
来源：http://gwh.shzxlz.cn

[$a, $b] = $arr;
来源：http://wci.sxryk.cn

[U52] PHP：箭头函数
来源：http://hxd.redwolf501.top

$double = fn($x) => $x * 2;
来源：http://kfb.vqdsnc.cn

[U53] PHP：空合并运算符
来源：http://rpw.xingfuxueyuan.xyz

$v = $a ?? $b ?? "default";
来源：http://tfv.hongshengwenyu.top

[U54] PHP：空安全调用
来源：http://tea.zhixingplan.top

$obj?->method()
来源：http://ben.nanxuanxn.top

[U55] PHP：match 表达式
来源：http://xxd.xinyue.icu

$s = match($x) { 1 => "一", default => "其他" };
来源：http://icm.dashuyun.cn

[U56] PHP：命名参数
来源：http://tht.daria6918.cn

f(a: 1, b: 2)
来源：http://gmp.ywan-chungtsiang.top

[U57] PHP：字符串插值
来源：http://msw.hfpthk.cn

"值: {$a}"
来源：http://lcm.gaohongyu789.top

[U58] PHP：数组三件套
来源：http://oxt.316326.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vvh.yuxming.cn


<!-- 参考信息 -->