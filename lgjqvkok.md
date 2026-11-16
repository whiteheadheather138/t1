代发 wailian999

[S33] C++：vector 增删
来源：http://gyx.snrcjt.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qpr.xylfe.cn

[S34] C++：遍历 vector
来源：http://zsz.jianghu66.top

for (auto &x : v) { std::cout << x; }
来源：http://sql.sweek.top

[S35] C++：map
来源：http://tny.gaohongyu789.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ihv.wangshuangyany.cn

[S36] C++：unordered_map
来源：http://vuu.tian-w.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://inh.zdbjq.cn

[S37] C++：set
来源：http://asz.cashguo.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gej.gzhubu.top

[S38] C++：排序
来源：http://jsv.vehdjk.com

std::sort(v.begin(), v.end());
来源：http://lue.fktsv.cn

[S39] C++：自定义比较器排序
来源：http://oou.nanxuanxn.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wfr.smart0.xyz

[S40] C++：查找元素
来源：http://jct.c1oappe.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vke.ydzc1.top

[S41] C++：类与构造函数
来源：http://dni.xinyue.icu

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lnf.aibaodan.cn

[S42] C++：继承与虚函数
来源：http://pwj.jiagoushi.top

class B : public Base { public: void f() override {} };
来源：http://hfu.svipenyu.cn

[S43] C++：智能指针
来源：http://tgg.chenzaomai.com

auto p = std::make_unique<int>(5);
来源：http://egs.9152youxi.cn

[S44] C++：引用传参
来源：http://nda.zhijiandao.cn

void inc(int &x) { ++x; }
来源：http://mne.aizwys.cn

[S45] C++：lambda
来源：http://gyj.svipenyu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://koo.ydjk.org.cn

[S46] C++：函数模板
来源：http://erc.yj20258888.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hrv.hywenlv.cn

[S47] C++：结构化绑定遍历
来源：http://djv.c1oappe.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zen.sjlbkw.cn

[S48] C++：逐行读文件
来源：http://qrd.tanke756.top

std::ifstream in("a.txt");  std::string line;
来源：http://vlr.epnwcf.com

while (std::getline(in, line)) { }
来源：http://lrq.ehwqpu.com

[S49] C++：写文件
来源：http://edz.smart0.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xab.ywan-chungtsiang.top

[S50] C++：格式化数字
来源：http://ldu.tanke756.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wiw.ehwqpu.com

[S51] C++：显式类型转换
来源：http://zmp.hfpthk.cn

static_cast<double>(a) / b
来源：http://zwy.zhixingplan.top

[S52] C++：const 与 noexcept
来源：http://lmc.fanxiaobao.xyz

int size() const noexcept { return n_; }
来源：http://yha.cucudq.cn

[S53] C++：移动语义
来源：http://szt.shangyingyoupin.top

std::vector<int> w = std::move(v);
来源：http://vkr.nanxinkj.top

[S54] C++：异常处理
来源：http://xzn.bjfxy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://acq.zycfv.cn

[S55] C++：结构化绑定
来源：http://ves.zdqjudy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://qek.jinghuilouyu.cn

[S56] C++：optional
来源：http://xot.hammf.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://sij.hysaishi.cn

[S57] C++：编译期常量
来源：http://enu.chenjidiqi.icu

constexpr int N = 10;
来源：http://bsd.shanyushiyangtech.top

[S58] C++：命名空间
来源：http://vrq.sxryk.cn

namespace ns { int f() { return 1; } }
来源：http://muf.fktsv.cn

[S59] C++：静态断言
来源：http://syj.gotoacloud.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vgb.yongpay.top

[S60] C++：遍历并删除元素
来源：http://czl.daria6918.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lck.hnxiangtu.top

================================================================================
来源：http://wzg.vqdsnc.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://srf.yangfankeji.com

================================================================================
来源：http://aqm.zycfv.cn

[T01] Kotlin：Hello World
来源：http://hvj.uphjek.com

println("Hello")
来源：http://xas.yonumen.top

[T02] Kotlin：变量
来源：http://rqc.snrcjt.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ucx.tarul.cn

[T03] Kotlin：字符串模板
来源：http://lvp.dashuyun.cn

"值: $b"
来源：http://knz.hesvh.cn

[T04] Kotlin：空安全
来源：http://ozz.zhixingplan.top

val n: String? = null;  n?.length
来源：http://gub.xuanzx.com

[T05] Kotlin：when 表达式
来源：http://osd.hcnkem.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yld.fengsongda.top

[T06] Kotlin：集合映射
来源：http://ley.xylfe.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://qng.feifeiyinyue.top

[T07] Kotlin：集合过滤
来源：http://cwe.wangshuangyany.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://blk.tanke756.top

[T08] Kotlin：数据类
来源：http://cdt.aibaodan.cn

data class User(val name: String, val age: Int)
来源：http://pbj.jqgufenzy.top

[T09] Kotlin：扩展函数
来源：http://beq.hammf.cn

fun String.exclaim() = this + "!"
来源：http://abp.cqqwz.cn

[T10] Kotlin：默认参数
来源：http://mos.jianghu66.top

fun greet(name: String = "World") = "Hi $name"
来源：http://bay.c1oappe.top

[T11] Kotlin：协程
来源：http://dyq.fanxiaobao.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://sgd.hysaishi.cn

[T12] Kotlin：解构声明
来源：http://sln.xinyue.icu

val (a, b) = Pair(1, 2)
来源：http://sbc.tanke756.top

[T13] Kotlin：只读 Map
来源：http://mil.sjlbkw.cn

val m = mapOf("a" to 1)
来源：http://kxb.chenjidiqi.icu

[T14] Kotlin：循环
来源：http://nqb.daxiang520.top

for (i in 1..10) println(i)
来源：http://dcb.shuidangran.top

[T15] Kotlin：接口
来源：http://hsy.sjlbkw.cn

interface Shape { fun area(): Double }
来源：http://kuk.shanyushiyangtech.top

[T16] Swift：Hello World
来源：http://pxv.chenjidiqi.icu

print("Hello")
来源：http://zlb.wangshuangyany.cn

[T17] Swift：变量与常量
来源：http://mgc.hcnkem.com

var a = 1;  let b = 2
来源：http://pdz.xziqi.cn

[T18] Swift：字符串插值
来源：http://egn.xingfuxueyuan.xyz

"值: \(b)"
来源：http://tmc.ctjpmb.com

[T19] Swift：可选绑定
来源：http://lim.zhixingplan.top

if let n = opt { print(n) }
来源：http://nay.xinyue.icu

[T20] Swift：数组操作
来源：http://aqe.uphjek.com

var a = [1, 2, 3];  a.append(4)
来源：http://euk.zhixingplan.top

[T21] Swift：遍历
来源：http://psj.fengsongda.top

for x in a { print(x) }
来源：http://hej.jinghuilouyu.cn

[T22] Swift：字典
来源：http://cup.yanxiufei.cn

var d = ["a": 1];  d["b"] = 2
来源：http://uas.shzxlz.cn

[T23] Swift：函数
来源：http://oba.sweek.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dke.chenzaomai.com

[T24] Swift：闭包
来源：http://eae.haohaochexian.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://vsn.fengsongda.top

[T25] Swift：结构体
来源：http://ass.yj20258.top

struct P { var x: Int }
来源：http://jan.feifeiyinyue.top

[T26] Swift：类与重写
来源：http://jkr.gaohongyu789.top

class A: Base { override func f() {} }
来源：http://ukp.hywenlv.cn

[T27] Swift：错误处理
来源：http://amp.gzhubu.top

do { try f() } catch { print(error) }
来源：http://soa.tarul.cn

[T28] Swift：枚举
来源：http://inn.yj20258.top

enum Color { case red, green }
来源：http://giv.vehdjk.com

[T29] Swift：guard 提前返回
来源：http://vqh.uphjek.com

guard let x = opt else { return }
来源：http://ezl.svipenyu.cn

[T30] Swift：协议
来源：http://wwq.jinqigfzy.top

protocol Shape { func area() -> Double }
来源：http://rar.yonumen.top

[T31] Lua：Hello World
来源：http://cpi.jlsjyb.cn

print("Hello")
来源：http://lmw.xuetiantiany.cn

[T32] Lua：局部变量
来源：http://zjt.zhongyouzk.top

local a = 1
来源：http://whx.redwolf501.top

[T33] Lua：表（数组）
来源：http://mjt.ehwqpu.com

local t = {1, 2, 3};  t[4] = 4
来源：http://ghc.ybcxt.top

[T34] Lua：遍历表
来源：http://qwe.chenjidiqi.icu

for i, v in ipairs(t) do print(i, v) end
来源：http://ued.jyoumei.cn

[T35] Lua：字典表
来源：http://vjo.sufxvd.cn

local d = { a = 1 };  d.b = 2
来源：http://jyp.zdqjudy.top

[T36] Lua：函数
来源：http://tay.cucudq.cn

function add(a, b) return a + b end
来源：http://ihb.0kj1m.cn

[T37] Lua：字符串拼接
来源：http://luf.hysaishi.cn

"a" .. "b"
来源：http://bmq.mhx1999.top

[T38] Lua：条件
来源：http://bqh.zhixingplan.top

if x > 0 then print("正") end
来源：http://mfw.hcnkem.com

[T39] Lua：模式匹配
来源：http://wsv.yj202588.top

string.find(s, "%d+")
来源：http://bch.aizwys.cn

[T40] Lua：元表
来源：http://kiz.hfpthk.cn

setmetatable({}, { __index = base })
来源：http://kcm.jiagoushi.top

[T41] Perl：Hello World
来源：http://dno.jianghu66.top

print "Hello\n";
来源：http://jtd.jiagoushi.top

[T42] Perl：变量类型
来源：http://vwr.xingfuxueyuan.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vdw.xingfuxueyuan.xyz

[T43] Perl：字符串插值
来源：http://owf.yj20258888.top

"值: $a"
来源：http://foa.jianghu66.top

[T44] Perl：条件
来源：http://lvq.iojbl.cn

if ($a > 0) { print "正"; }
来源：http://rim.jqgufenzy.top

[T45] Perl：数组遍历
来源：http://svd.yueranfly.top

for my $x (@arr) { print $x; }
来源：http://syy.snrcjt.cn

[T46] Perl：哈希操作
来源：http://ttf.xinyue.icu

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jbr.hfpthk.cn

[T47] Perl：正则捕获
来源：http://izt.hnxiangtu.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://jwn.yangfankeji.com

[T48] Perl：正则替换
来源：http://clh.quarkkingdee.top

$s =~ s/old/new/g;
来源：http://rji.shangyingyoupin.top

[T49] Perl：函数
来源：http://etd.zhaomingkeji.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ssd.fktsv.cn

[T50] Perl：逐行读文件
来源：http://son.daria6918.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://dfl.shanyushiyangtech.top

while (my $line = <$fh>) { print $line; }
来源：http://nun.xuetiantiany.cn

[T51] Scala：Hello World
来源：http://uds.dianchejie.cn

println("Hello")
来源：http://ogr.cucudq.cn

[T52] Scala：变量
来源：http://jrw.tarul.cn

val a = 1;  var b = 2
来源：http://iqy.quarkkingdee.top

[T53] Scala：字符串插值
来源：http://uiy.jyoumei.cn

s"值: $b"
来源：http://tpt.9152youxi.cn

[T54] Scala：集合映射
来源：http://phn.cdnleiting.top

List(1, 2, 3).map(_ * 2)
来源：http://sbj.yfazqb.com

[T55] Scala：集合过滤
来源：http://qyz.sweek.top

List(1, 2, 3).filter(_ > 1)
来源：http://jyv.mhx1999.top

[T56] Scala：样例类
来源：http://zok.zdbjq.cn

case class User(name: String, age: Int)
来源：http://bxd.pycfn.com

[T57] Scala：模式匹配
来源：http://blp.xziqi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://igq.chenjidiqi.icu

[T58] Scala：函数定义
来源：http://lxm.xuanzx.com

def add(a: Int, b: Int): Int = a + b
来源：http://lwh.gotoacloud.top

[T59] Scala：循环
来源：http://lvc.yfazqb.com

for (i <- 1 to 10) println(i)
来源：http://dxr.zhoulong.xyz

[T60] Scala：折叠
来源：http://cit.zhoulong.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zmv.uphjek.com

================================================================================
来源：http://ahi.yvedp.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://whl.zdbjq.cn

================================================================================
来源：http://maz.chenzaomai.com

[U01] Py：创建虚拟环境
来源：http://dow.jinyuanbaomall.cn

python -m venv .venv && source .venv/bin/activate
来源：http://yum.gaohongyu789.top

[U02] Py：导出 / 安装依赖
来源：http://hor.c1oappe.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gzl.xziqi.cn

[U03] Py：加载 .env 配置
来源：http://xvc.vqdsnc.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://cxd.birdmap.top

[U04] Py：变量调试打印
来源：http://vmr.gaohongyu789.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nrm.shanyushiyangkeji.top

[U05] Py：列表去重且保序
来源：http://maz.guannengcc.top

list(dict.fromkeys(arr))
来源：http://hgx.jqgfzy.top

[U06] Py：合并两个字典
来源：http://sjd.shuidangran.top

{**a, **b}
来源：http://huk.shanyushiyangkeji.top

[U07] Py：反转字典键值
来源：http://gkc.jinqigfzy.top

{v: k for k, v in d.items()}
来源：http://byb.fktsv.cn

[U08] Py：展平二维列表
来源：http://ydz.zhixingplan.top

[y for x in nested for y in x]
来源：http://ibx.yuanzhike.top

[U09] Py：字典取最大值的键
来源：http://hmp.fanxiaobao.xyz

max(d, key=d.get)
来源：http://pyr.cqqwz.cn

[U10] Py：按值排序字典
来源：http://iuh.ivvv.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mkf.9152youxi.cn

[U11] Py：生成器表达式
来源：http://hxz.yuanzhike.top

(x * 2 for x in arr)
来源：http://rfn.zhijiandao.cn

[U12] Py：取出现最多的 3 个元素
来源：http://knt.tanke756.top

Counter(arr).most_common(3)
来源：http://edi.zhiwuduotai.top

[U13] Py：固定长度队列
来源：http://xux.andypj.xyz

deque(maxlen=10)
来源：http://coz.ehwqpu.com

[U14] Py：分组收集到列表
来源：http://nxa.hfpthk.cn

defaultdict(list)
来源：http://rij.svipenyu.cn

[U15] Py：高精度计时
来源：http://gmo.jinqigfzy.top

t = time.perf_counter()
来源：http://oee.epnwcf.com

[U16] Py：命令行参数解析
来源：http://whg.fengsongda.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fta.pengpengdd.cyou

[U17] Py：初始化日志
来源：http://kcc.fktsv.cn

logging.basicConfig(level=logging.INFO)
来源：http://utp.cucudq.cn

[U18] Py：预编译正则
来源：http://sbu.sweek.top

pat = re.compile(r"\d+")
来源：http://jyr.bjfxy.top

[U19] Py：正则替换带回调
来源：http://gyi.xingfuxueyuan.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://dmn.hnxiangtu.top

[U20] Py：缓存函数结果
来源：http://rpf.9152youxi.cn

@functools.lru_cache(maxsize=None)
来源：http://may.yj202588.top

[U21] Py：自定义上下文管理器
来源：http://gjo.hfpthk.cn

@contextlib.contextmanager
来源：http://jvo.aizwys.cn

[U22] Py：矩阵转置
来源：http://ppc.feifeiyinyue.top

list(zip(*m))
来源：http://tni.yfazqb.com

[U23] Py：分块读取大文件
来源：http://rgp.cdnleiting.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://kgk.jlsjyb.cn

[U24] Py：路径操作
来源：http://zsb.chenjidiqi.icu

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://eqn.ivvv.top

[U25] Py：CSV 按字典读
来源：http://kxc.chenlongwang.top

csv.DictReader(f)
来源：http://pgn.xuetiantiany.cn

[U26] Py：并发下载
来源：http://bpt.pycfn.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://buv.fehbvm.com

[U27] Py：异步 HTTP
来源：http://ptp.jyoumei.cn

aiohttp.ClientSession() 配合 async with
来源：http://jur.xylfe.cn

[U28] Py：类型别名
来源：http://ekh.sysykeji.top

UserId = int
来源：http://ifg.yuxming.cn

[U29] Py：属性校验
来源：http://wxx.hesvh.cn

@property 与 @x.setter 配合
来源：http://wjf.dashuyun.cn

[U30] Py：数据类
来源：http://utq.jqgufenzy.top

@dataclass(slots=True)
来源：http://vnb.jlsjyb.cn

[U31] Py：单测
来源：http://cmf.ppjwa.cn

python -m pytest -q
来源：http://ftg.gogol.net.cn

[U32] Py：代码格式化
来源：http://obb.ppjwa.cn

ruff format . && ruff check --fix .
来源：http://thu.yonumen.top

[U33] Py：打包发布
来源：http://eps.redwolf501.top

python -m build  （依赖 pyproject.toml）
来源：http://cvn.hcnkem.com

[U34] Py：判断编码
来源：http://ntu.jinqigfzy.top

chardet.detect(raw)
来源：http://sua.nwbrower.top

[U35] Py：发送邮件
来源：http://haf.cqqwz.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jmj.zhongyouzk.top

[U36] Py：定时任务
来源：http://uxg.uphjek.com

schedule.every(10).minutes.do(job)
来源：http://nuj.guannengcc.top

[U37] Py：读写 Excel
来源：http://hut.shzxlz.cn

pandas.read_excel / DataFrame.to_excel
来源：http://oqs.jyoumei.cn

[U38] Py：获取脚本所在目录
来源：http://imx.xuetiantiany.cn

Path(__file__).resolve().parent
来源：http://awt.jqgfzy.top

[U39] Py：判断是否在交互环境
来源：http://wht.shanyushiyangtech.top

sys.stdout.isatty()
来源：http://bzq.bbcook.cn

[U40] Py：打印到标准错误
来源：http://yab.xuetiantiany.cn

print("err", file=sys.stderr)
来源：http://cwq.dianchejie.cn

[U41] PHP：初始化 Composer 项目
来源：http://mec.sjlbkw.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://div.gaohongyu789.top

[U42] PHP：PSR-4 自动加载
来源：http://tfu.smart0.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hui.zhaomingkeji.xyz

[U43] PHP：声明命名空间
来源：http://snc.gogol.net.cn

namespace App\Http;
来源：http://mpv.jiagoushi.top

[U44] PHP：开启严格类型
来源：http://vja.kuanghao11.cn

declare(strict_types=1);
来源：http://fsg.ivvv.top

[U45] PHP：类型声明与返回类型
来源：http://kof.316326.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://hnv.ivvv.top

[U46] PHP：可空类型
来源：http://ocd.zhoulong.xyz

?string $name = null
来源：http://oqp.cucudq.cn

[U47] PHP：联合类型
来源：http://ffu.hnxiangtu.top

int|string $id
来源：http://yyx.jinghuilouyu.cn

[U48] PHP：纯枚举
来源：http://hbj.xinyue.icu

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://fpr.shzxlz.cn

[U49] PHP：只读属性
来源：http://uys.dashuyun.cn

public readonly string $name
来源：http://geg.pengpengdd.cyou

[U50] PHP：构造器属性提升
来源：http://sgz.chenzaomai.com

public function __construct(private int $id) {}
来源：http://iuz.zhongyouzk.top

[U51] PHP：数组解构
来源：http://wqq.pycfn.com

[$a, $b] = $arr;
来源：http://tam.hongshengwenyu.top

[U52] PHP：箭头函数
来源：http://mnk.fzhhl.top

$double = fn($x) => $x * 2;
来源：http://ovr.0kj1m.cn

[U53] PHP：空合并运算符
来源：http://uoo.zdbjq.cn

$v = $a ?? $b ?? "default";
来源：http://wkz.haohaochexian.top

[U54] PHP：空安全调用
来源：http://mfk.chenzaomai.com

$obj?->method()
来源：http://jwr.ybcxt.top

[U55] PHP：match 表达式
来源：http://vdm.hongshengwenyu.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://sjl.yj20258.top

[U56] PHP：命名参数
来源：http://jqu.zhixingplan.top

f(a: 1, b: 2)
来源：http://kbv.zdqjudy.top

[U57] PHP：字符串插值
来源：http://hwd.dashuyun.cn

"值: {$a}"
来源：http://ago.hnqzz.top

[U58] PHP：数组三件套
来源：http://kgi.pengpengdd.cyou

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rzn.yvedp.cn


<!-- 参考信息 -->