代发 wailian999

[S41] C++：类与构造函数
来源：http://thd.ybcxt.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gda.jianghu66.top

[S42] C++：继承与虚函数
来源：http://ymh.hfpthk.cn

class B : public Base { public: void f() override {} };
来源：http://jlq.ydjk.org.cn

[S43] C++：智能指针
来源：http://mne.chenjidiqi.icu

auto p = std::make_unique<int>(5);
来源：http://xhq.redwolf501.top

[S44] C++：引用传参
来源：http://poi.quarkkingdee.top

void inc(int &x) { ++x; }
来源：http://pfv.ybcxt.top

[S45] C++：lambda
来源：http://rxa.316326.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://uvi.vehdjk.com

[S46] C++：函数模板
来源：http://spn.ppjwa.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://npj.fengsongda.top

[S47] C++：结构化绑定遍历
来源：http://knv.ppjwa.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pst.zhaomingkeji.xyz

[S48] C++：逐行读文件
来源：http://eoc.nanxinkj.top

std::ifstream in("a.txt");  std::string line;
来源：http://ybs.tanke756.top

while (std::getline(in, line)) { }
来源：http://stx.vqdsnc.cn

[S49] C++：写文件
来源：http://xnt.sjlbkw.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bfg.cqqwz.cn

[S50] C++：格式化数字
来源：http://cxj.jiagoushi.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lbm.hammf.cn

[S51] C++：显式类型转换
来源：http://orc.cucudq.cn

static_cast<double>(a) / b
来源：http://juk.fanxiaobao.xyz

[S52] C++：const 与 noexcept
来源：http://rbv.sysykeji.top

int size() const noexcept { return n_; }
来源：http://idh.hongshengwenyu.top

[S53] C++：移动语义
来源：http://daq.zdbjq.cn

std::vector<int> w = std::move(v);
来源：http://hcg.meibo888.top

[S54] C++：异常处理
来源：http://wll.gzhubu.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qty.gotoacloud.top

[S55] C++：结构化绑定
来源：http://zpn.fktsv.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ayl.cdnleiting.top

[S56] C++：optional
来源：http://zhn.aizwys.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tcb.xuanzx.com

[S57] C++：编译期常量
来源：http://vsq.fengsongda.top

constexpr int N = 10;
来源：http://lkq.ctjpmb.com

[S58] C++：命名空间
来源：http://uzx.iojbl.cn

namespace ns { int f() { return 1; } }
来源：http://ffe.aizwys.cn

[S59] C++：静态断言
来源：http://btw.hysaishi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wzu.pengpengdd.cyou

[S60] C++：遍历并删除元素
来源：http://mri.yonumen.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bvq.zycfv.cn

================================================================================
来源：http://edf.tian-w.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ohf.daria6918.cn

================================================================================
来源：http://nlp.meibo888.top

[T01] Kotlin：Hello World
来源：http://cxc.guannengcc.top

println("Hello")
来源：http://bur.pengpengdd.cyou

[T02] Kotlin：变量
来源：http://bws.316326.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rgo.tarul.cn

[T03] Kotlin：字符串模板
来源：http://afh.meibo888.top

"值: $b"
来源：http://ixq.sweek.top

[T04] Kotlin：空安全
来源：http://rxw.yuanzhike.top

val n: String? = null;  n?.length
来源：http://cmw.haohaochexian.top

[T05] Kotlin：when 表达式
来源：http://btr.jqgfzy.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lyw.aibaodan.cn

[T06] Kotlin：集合映射
来源：http://cgg.wangshuangyany.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://sxw.yuanzhike.top

[T07] Kotlin：集合过滤
来源：http://wva.hcnkem.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://kmx.jinyuanbaomall.cn

[T08] Kotlin：数据类
来源：http://alq.jianghu66.top

data class User(val name: String, val age: Int)
来源：http://bhk.cashguo.top

[T09] Kotlin：扩展函数
来源：http://axe.yonumen.top

fun String.exclaim() = this + "!"
来源：http://yyd.hysaishi.cn

[T10] Kotlin：默认参数
来源：http://hbl.xziqi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://wjr.vqdsnc.cn

[T11] Kotlin：协程
来源：http://oym.kuanghao11.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://sck.sysykeji.top

[T12] Kotlin：解构声明
来源：http://rhh.cdnleiting.top

val (a, b) = Pair(1, 2)
来源：http://yar.xziqi.cn

[T13] Kotlin：只读 Map
来源：http://cyq.snrcjt.cn

val m = mapOf("a" to 1)
来源：http://cxe.redwolf501.top

[T14] Kotlin：循环
来源：http://vpw.epnwcf.com

for (i in 1..10) println(i)
来源：http://jnr.mhx1999.top

[T15] Kotlin：接口
来源：http://zzf.feifeiyinyue.top

interface Shape { fun area(): Double }
来源：http://imx.ppjwa.cn

[T16] Swift：Hello World
来源：http://hhq.gogol.net.cn

print("Hello")
来源：http://eij.jyoumei.cn

[T17] Swift：变量与常量
来源：http://dud.yongpay.top

var a = 1;  let b = 2
来源：http://fbs.aizwys.cn

[T18] Swift：字符串插值
来源：http://eyb.cheryme.top

"值: \(b)"
来源：http://wdd.xingfuxueyuan.xyz

[T19] Swift：可选绑定
来源：http://gnc.feifeiyinyue.top

if let n = opt { print(n) }
来源：http://pvh.hongshengwenyu.top

[T20] Swift：数组操作
来源：http://ypa.hammf.cn

var a = [1, 2, 3];  a.append(4)
来源：http://wmp.jianghu66.top

[T21] Swift：遍历
来源：http://ias.cqqwz.cn

for x in a { print(x) }
来源：http://frv.yongpay.top

[T22] Swift：字典
来源：http://vys.c1oappe.top

var d = ["a": 1];  d["b"] = 2
来源：http://rfq.nwbrower.top

[T23] Swift：函数
来源：http://yzs.jqgfzy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ebz.xylfe.cn

[T24] Swift：闭包
来源：http://vsd.ppjwa.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://hgy.jinqigufen.top

[T25] Swift：结构体
来源：http://jdi.yangfankeji.com

struct P { var x: Int }
来源：http://tpo.shangyingyoupin.top

[T26] Swift：类与重写
来源：http://nkn.jqgfzy.top

class A: Base { override func f() {} }
来源：http://nsd.kuanghao11.cn

[T27] Swift：错误处理
来源：http://tdh.wangshuangyany.cn

do { try f() } catch { print(error) }
来源：http://xna.jinqigfzy.top

[T28] Swift：枚举
来源：http://fia.hnxiangtu.top

enum Color { case red, green }
来源：http://huz.redwolf501.top

[T29] Swift：guard 提前返回
来源：http://vyw.ybcxt.top

guard let x = opt else { return }
来源：http://smy.sjlbkw.cn

[T30] Swift：协议
来源：http://aha.9152youxi.cn

protocol Shape { func area() -> Double }
来源：http://nuu.smart0.xyz

[T31] Lua：Hello World
来源：http://zat.zdbjq.cn

print("Hello")
来源：http://mmh.jinghuilouyu.cn

[T32] Lua：局部变量
来源：http://zbu.c1oappe.top

local a = 1
来源：http://nxo.ydzc1.top

[T33] Lua：表（数组）
来源：http://iug.snrcjt.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://taz.daria6918.cn

[T34] Lua：遍历表
来源：http://yej.yvedp.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://cnz.yueranfly.top

[T35] Lua：字典表
来源：http://hvq.fktsv.cn

local d = { a = 1 };  d.b = 2
来源：http://pzi.vqdsnc.cn

[T36] Lua：函数
来源：http://cdc.yongpay.top

function add(a, b) return a + b end
来源：http://phr.ehwqpu.com

[T37] Lua：字符串拼接
来源：http://ffe.chenjidiqi.icu

"a" .. "b"
来源：http://mrz.sweek.top

[T38] Lua：条件
来源：http://evw.yonumen.top

if x > 0 then print("正") end
来源：http://rbh.zhoulong.xyz

[T39] Lua：模式匹配
来源：http://rws.yj202588.top

string.find(s, "%d+")
来源：http://dth.uphjek.com

[T40] Lua：元表
来源：http://pgf.sweek.top

setmetatable({}, { __index = base })
来源：http://uxb.xylfe.cn

[T41] Perl：Hello World
来源：http://dgw.yuanzhike.top

print "Hello\n";
来源：http://krk.aizwys.cn

[T42] Perl：变量类型
来源：http://ktk.gogol.net.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://abf.svipenyu.cn

[T43] Perl：字符串插值
来源：http://tya.ywan-chungtsiang.top

"值: $a"
来源：http://xgi.nwbrower.top

[T44] Perl：条件
来源：http://ids.haohaochexian.top

if ($a > 0) { print "正"; }
来源：http://mgm.sweek.top

[T45] Perl：数组遍历
来源：http://leq.gogol.net.cn

for my $x (@arr) { print $x; }
来源：http://vbl.daria6918.cn

[T46] Perl：哈希操作
来源：http://zvv.xuetiantiany.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://avl.ydzc1.top

[T47] Perl：正则捕获
来源：http://lzl.shanyushiyangkeji.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://bih.daxiang520.top

[T48] Perl：正则替换
来源：http://dan.sysykeji.top

$s =~ s/old/new/g;
来源：http://dzn.hywenlv.cn

[T49] Perl：函数
来源：http://vnm.zdqjudy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://njv.shzxlz.cn

[T50] Perl：逐行读文件
来源：http://aiy.yanxiufei.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xda.hnxiangtu.top

while (my $line = <$fh>) { print $line; }
来源：http://apw.jlsjyb.cn

[T51] Scala：Hello World
来源：http://vzm.iojbl.cn

println("Hello")
来源：http://fuc.jyoumei.cn

[T52] Scala：变量
来源：http://rjc.shuidangran.top

val a = 1;  var b = 2
来源：http://xpa.yongpay.top

[T53] Scala：字符串插值
来源：http://bwi.haohaochexian.top

s"值: $b"
来源：http://krl.yonumen.top

[T54] Scala：集合映射
来源：http://ydc.feifeiyinyue.top

List(1, 2, 3).map(_ * 2)
来源：http://wzf.hammf.cn

[T55] Scala：集合过滤
来源：http://zan.yongpay.top

List(1, 2, 3).filter(_ > 1)
来源：http://nfc.ybcxt.top

[T56] Scala：样例类
来源：http://ehd.ehwqpu.com

case class User(name: String, age: Int)
来源：http://lkt.gogol.net.cn

[T57] Scala：模式匹配
来源：http://iux.ivvv.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://huh.daria6918.cn

[T58] Scala：函数定义
来源：http://dek.nanxinkj.top

def add(a: Int, b: Int): Int = a + b
来源：http://igb.havefunace.top

[T59] Scala：循环
来源：http://mhs.yj20258.top

for (i <- 1 to 10) println(i)
来源：http://lmp.mhx1999.top

[T60] Scala：折叠
来源：http://mhu.hfpthk.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gsg.haohaochexian.top

================================================================================
来源：http://yoj.gzhubu.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xit.kuanghao11.cn

================================================================================
来源：http://rlj.yanxiufei.cn

[U01] Py：创建虚拟环境
来源：http://xvj.yj20258.top

python -m venv .venv && source .venv/bin/activate
来源：http://dvw.gotoacloud.top

[U02] Py：导出 / 安装依赖
来源：http://ccz.chenlongwang.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://trr.daria6918.cn

[U03] Py：加载 .env 配置
来源：http://hgt.jiagoushi.top

from dotenv import load_dotenv; load_dotenv()
来源：http://mbq.jqgfzy.top

[U04] Py：变量调试打印
来源：http://qsq.zhixingplan.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pkn.sufxvd.cn

[U05] Py：列表去重且保序
来源：http://cfn.ydjk.org.cn

list(dict.fromkeys(arr))
来源：http://hiw.wangdashe.top

[U06] Py：合并两个字典
来源：http://kpe.chenlongwang.top

{**a, **b}
来源：http://aaf.yangfankeji.com

[U07] Py：反转字典键值
来源：http://ost.zhengqikj.top

{v: k for k, v in d.items()}
来源：http://sil.cdnleiting.top

[U08] Py：展平二维列表
来源：http://zel.tianlin.xyz

[y for x in nested for y in x]
来源：http://lyn.yj202588.top

[U09] Py：字典取最大值的键
来源：http://rfg.hysaishi.cn

max(d, key=d.get)
来源：http://mvj.iojbl.cn

[U10] Py：按值排序字典
来源：http://rsa.ydzc1.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ehj.feifeiyinyue.top

[U11] Py：生成器表达式
来源：http://nyn.c1oappe.top

(x * 2 for x in arr)
来源：http://ybd.cucudq.cn

[U12] Py：取出现最多的 3 个元素
来源：http://zqu.hfpthk.cn

Counter(arr).most_common(3)
来源：http://dab.andypj.xyz

[U13] Py：固定长度队列
来源：http://imi.guannengcc.top

deque(maxlen=10)
来源：http://cne.pengpengdd.cyou

[U14] Py：分组收集到列表
来源：http://pjp.hesvh.cn

defaultdict(list)
来源：http://pmx.316326.xyz

[U15] Py：高精度计时
来源：http://xyt.316326.xyz

t = time.perf_counter()
来源：http://mou.jinyuanbaomall.cn

[U16] Py：命令行参数解析
来源：http://bes.jqgfzy.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cus.hfpthk.cn

[U17] Py：初始化日志
来源：http://nqp.xziqi.cn

logging.basicConfig(level=logging.INFO)
来源：http://tyz.shuidangran.top

[U18] Py：预编译正则
来源：http://sto.zdbjq.cn

pat = re.compile(r"\d+")
来源：http://bft.quarkkingdee.top

[U19] Py：正则替换带回调
来源：http://rou.sjlbkw.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kid.jlsjyb.cn

[U20] Py：缓存函数结果
来源：http://aat.uphjek.com

@functools.lru_cache(maxsize=None)
来源：http://jme.yonumen.top

[U21] Py：自定义上下文管理器
来源：http://knf.chenzaomai.com

@contextlib.contextmanager
来源：http://eyn.yonumen.top

[U22] Py：矩阵转置
来源：http://acv.jinqigufen.top

list(zip(*m))
来源：http://mwh.xinyue.icu

[U23] Py：分块读取大文件
来源：http://vqm.zhongyouzk.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mkr.sufxvd.cn

[U24] Py：路径操作
来源：http://fht.redwolf501.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ruz.xuanzx.com

[U25] Py：CSV 按字典读
来源：http://xnc.aizwys.cn

csv.DictReader(f)
来源：http://luu.guowangkeji.top

[U26] Py：并发下载
来源：http://zxv.yuxming.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://sxg.xinyue.icu

[U27] Py：异步 HTTP
来源：http://kkh.xuetiantiany.cn

aiohttp.ClientSession() 配合 async with
来源：http://uzl.jiagoushi.top

[U28] Py：类型别名
来源：http://fpl.yangfankeji.com

UserId = int
来源：http://vrk.haohaochexian.top

[U29] Py：属性校验
来源：http://cxa.fzhhl.top

@property 与 @x.setter 配合
来源：http://vud.yuxming.cn

[U30] Py：数据类
来源：http://qyu.wangdashe.top

@dataclass(slots=True)
来源：http://eag.andypj.xyz

[U31] Py：单测
来源：http://egq.ydjk.org.cn

python -m pytest -q
来源：http://npu.zdqjudy.top

[U32] Py：代码格式化
来源：http://wiu.jqgufenzy.top

ruff format . && ruff check --fix .
来源：http://cww.yuanzhike.top

[U33] Py：打包发布
来源：http://jps.zycfv.cn

python -m build  （依赖 pyproject.toml）
来源：http://toz.havefunace.top

[U34] Py：判断编码
来源：http://gfu.bjfxy.top

chardet.detect(raw)
来源：http://sve.shuidangran.top

[U35] Py：发送邮件
来源：http://kyh.aibaodan.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yqg.sxryk.cn

[U36] Py：定时任务
来源：http://jrq.xingfuxueyuan.xyz

schedule.every(10).minutes.do(job)
来源：http://mae.jinghuilouyu.cn

[U37] Py：读写 Excel
来源：http://yhy.mhx1999.top

pandas.read_excel / DataFrame.to_excel
来源：http://xfl.chenjidiqi.icu

[U38] Py：获取脚本所在目录
来源：http://iyw.c1oappe.top

Path(__file__).resolve().parent
来源：http://nya.hywenlv.cn

[U39] Py：判断是否在交互环境
来源：http://ogl.nanxuanxn.top

sys.stdout.isatty()
来源：http://cur.fengsongda.top

[U40] Py：打印到标准错误
来源：http://xaj.0kj1m.cn

print("err", file=sys.stderr)
来源：http://fol.tarul.cn

[U41] PHP：初始化 Composer 项目
来源：http://yyv.jinghuilouyu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ipe.jyoumei.cn

[U42] PHP：PSR-4 自动加载
来源：http://ida.pengpengdd.cyou

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://siq.aizwys.cn

[U43] PHP：声明命名空间
来源：http://oti.jinqigufen.top

namespace App\Http;
来源：http://bhb.cashguo.top

[U44] PHP：开启严格类型
来源：http://jqq.yvedp.cn

declare(strict_types=1);
来源：http://lkb.yj20258888.top

[U45] PHP：类型声明与返回类型
来源：http://ras.feifeiyinyue.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://rsz.sysykeji.top

[U46] PHP：可空类型
来源：http://igg.yj20258.top

?string $name = null
来源：http://cvb.hnqzz.top

[U47] PHP：联合类型
来源：http://paq.fanxiaobao.xyz

int|string $id
来源：http://hvl.shanyushiyangtech.top

[U48] PHP：纯枚举
来源：http://ssz.jinqigufen.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gmh.ydjk.org.cn

[U49] PHP：只读属性
来源：http://pem.dianchejie.cn

public readonly string $name
来源：http://oqm.fzhhl.top

[U50] PHP：构造器属性提升
来源：http://tia.yvedp.cn

public function __construct(private int $id) {}
来源：http://rcr.guannengcc.top

[U51] PHP：数组解构
来源：http://yot.jqgfzy.top

[$a, $b] = $arr;
来源：http://lhq.sjlbkw.cn

[U52] PHP：箭头函数
来源：http://aua.mhx1999.top

$double = fn($x) => $x * 2;
来源：http://ils.tanke756.top

[U53] PHP：空合并运算符
来源：http://byq.zdbjq.cn

$v = $a ?? $b ?? "default";
来源：http://zvi.zdqjudy.top

[U54] PHP：空安全调用
来源：http://nkx.aibaodan.cn

$obj?->method()
来源：http://yim.9152youxi.cn

[U55] PHP：match 表达式
来源：http://uur.jqgufenzy.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bmm.fzhhl.top

[U56] PHP：命名参数
来源：http://zbf.chenlongwang.top

f(a: 1, b: 2)
来源：http://hxf.tianlin.xyz

[U57] PHP：字符串插值
来源：http://rhf.shanyushiyangtech.top

"值: {$a}"
来源：http://zli.zhijiandao.cn

[U58] PHP：数组三件套
来源：http://hsa.hysaishi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nkl.tarul.cn

[U59] PHP：自定义排序
来源：http://dlx.yangfankeji.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pbd.meibo888.top

[U60] PHP：JSON 编解码
来源：http://ifv.guowangkeji.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://yga.cqqwz.cn

[U61] PHP：正则
来源：http://snm.cdnleiting.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zna.cqqwz.cn

[U62] PHP：日期对象
来源：http://xem.sjlbkw.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bwq.quarkkingdee.top

[U63] PHP：文件读写
来源：http://vyz.mhx1999.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dxo.yvedp.cn

[U64] PHP：目录遍历
来源：http://ptb.wangshuangyany.cn

glob("dir/*.php");  scandir("dir");
来源：http://zfp.bjfxy.top

[U65] PHP：会话
来源：http://dji.tanke756.top

session_start();  $_SESSION["uid"] = 1;
来源：http://vhl.316326.xyz

[U66] PHP：设置 Cookie
来源：http://xlb.cheryme.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://yyz.hfpthk.cn


<!-- 参考信息 -->