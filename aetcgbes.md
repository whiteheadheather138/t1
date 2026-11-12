代发 wailian999

[S39] C++：自定义比较器排序
来源：http://lft.316326.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mzy.daria6918.cn

[S40] C++：查找元素
来源：http://dko.tanke756.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rxn.aizwys.cn

[S41] C++：类与构造函数
来源：http://qdu.jlsjyb.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bkq.yangfankeji.com

[S42] C++：继承与虚函数
来源：http://obv.yfazqb.com

class B : public Base { public: void f() override {} };
来源：http://ofm.yanxiufei.cn

[S43] C++：智能指针
来源：http://eou.yonumen.top

auto p = std::make_unique<int>(5);
来源：http://qqr.ydjk.org.cn

[S44] C++：引用传参
来源：http://gxq.shzxlz.cn

void inc(int &x) { ++x; }
来源：http://rud.chenzaomai.com

[S45] C++：lambda
来源：http://nry.cdnleiting.top

auto add = [](int a, int b) { return a + b; };
来源：http://njg.xingfuxueyuan.xyz

[S46] C++：函数模板
来源：http://hhi.zhaomingkeji.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://iqe.shuidangran.top

[S47] C++：结构化绑定遍历
来源：http://zdu.fzhhl.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fqc.jinghuilouyu.cn

[S48] C++：逐行读文件
来源：http://cra.zdqjudy.top

std::ifstream in("a.txt");  std::string line;
来源：http://xex.epnwcf.com

while (std::getline(in, line)) { }
来源：http://fru.0kj1m.cn

[S49] C++：写文件
来源：http://tul.daxiang520.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yhp.meibo888.top

[S50] C++：格式化数字
来源：http://jve.hysaishi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mst.nanxinkj.top

[S51] C++：显式类型转换
来源：http://oup.9152youxi.cn

static_cast<double>(a) / b
来源：http://ojp.cashguo.top

[S52] C++：const 与 noexcept
来源：http://npc.xuanzx.com

int size() const noexcept { return n_; }
来源：http://bpd.nanxinkj.top

[S53] C++：移动语义
来源：http://bub.jinqigfzy.top

std::vector<int> w = std::move(v);
来源：http://xwq.ybcxt.top

[S54] C++：异常处理
来源：http://inf.52xcode.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://paq.shanyushiyangkeji.top

[S55] C++：结构化绑定
来源：http://eno.xuanzx.com

auto [a, b] = std::make_pair(1, 2);
来源：http://cln.nanxuanxn.top

[S56] C++：optional
来源：http://fub.haohaochexian.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dke.yuxming.cn

[S57] C++：编译期常量
来源：http://gnn.yuanzhike.top

constexpr int N = 10;
来源：http://mei.gaohongyu789.top

[S58] C++：命名空间
来源：http://blo.zycfv.cn

namespace ns { int f() { return 1; } }
来源：http://zsz.smart0.xyz

[S59] C++：静态断言
来源：http://scu.wangdashe.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vfx.haohaochexian.top

[S60] C++：遍历并删除元素
来源：http://som.jqgfzy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ejy.yuxming.cn

================================================================================
来源：http://ahf.nanxinkj.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ysz.wangdashe.top

================================================================================
来源：http://zsj.pengpengdd.cyou

[T01] Kotlin：Hello World
来源：http://trs.jlsjyb.cn

println("Hello")
来源：http://uyz.zycfv.cn

[T02] Kotlin：变量
来源：http://trd.hcnkem.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://snd.jqgufenzy.top

[T03] Kotlin：字符串模板
来源：http://yat.smart0.xyz

"值: $b"
来源：http://xtu.shuidangran.top

[T04] Kotlin：空安全
来源：http://min.hysaishi.cn

val n: String? = null;  n?.length
来源：http://ker.shuidangran.top

[T05] Kotlin：when 表达式
来源：http://xfc.hcnkem.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://llr.quarkkingdee.top

[T06] Kotlin：集合映射
来源：http://cgv.daxiang520.top

listOf(1, 2, 3).map { it * 2 }
来源：http://cee.aizwys.cn

[T07] Kotlin：集合过滤
来源：http://zpz.daxiang520.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ujx.sufxvd.cn

[T08] Kotlin：数据类
来源：http://jtg.uphjek.com

data class User(val name: String, val age: Int)
来源：http://rsa.chenjidiqi.icu

[T09] Kotlin：扩展函数
来源：http://jdg.yanxiufei.cn

fun String.exclaim() = this + "!"
来源：http://ehe.wangshuangyany.cn

[T10] Kotlin：默认参数
来源：http://xhp.fengsongda.top

fun greet(name: String = "World") = "Hi $name"
来源：http://fjg.sjlbkw.cn

[T11] Kotlin：协程
来源：http://ntf.zdbjq.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://nhw.yuxming.cn

[T12] Kotlin：解构声明
来源：http://lmq.iojbl.cn

val (a, b) = Pair(1, 2)
来源：http://tfy.yj202588.top

[T13] Kotlin：只读 Map
来源：http://iwo.gotoacloud.top

val m = mapOf("a" to 1)
来源：http://ctr.shanyushiyangkeji.top

[T14] Kotlin：循环
来源：http://uwo.aibaodan.cn

for (i in 1..10) println(i)
来源：http://aes.zhongyouzk.top

[T15] Kotlin：接口
来源：http://ghn.xylfe.cn

interface Shape { fun area(): Double }
来源：http://eco.gogol.net.cn

[T16] Swift：Hello World
来源：http://qdd.cucudq.cn

print("Hello")
来源：http://tib.9152youxi.cn

[T17] Swift：变量与常量
来源：http://jej.yueranfly.top

var a = 1;  let b = 2
来源：http://hiy.andypj.xyz

[T18] Swift：字符串插值
来源：http://ztw.tian-w.cn

"值: \(b)"
来源：http://rdt.xinyue.icu

[T19] Swift：可选绑定
来源：http://taz.hongshengwenyu.top

if let n = opt { print(n) }
来源：http://gjt.tanke756.top

[T20] Swift：数组操作
来源：http://hqv.ybcxt.top

var a = [1, 2, 3];  a.append(4)
来源：http://bnv.52xcode.cn

[T21] Swift：遍历
来源：http://bwp.nanxuanxn.top

for x in a { print(x) }
来源：http://emy.cashguo.top

[T22] Swift：字典
来源：http://tca.tianlin.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://rad.ivvv.top

[T23] Swift：函数
来源：http://jkt.yuxming.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ipy.shangyingyoupin.top

[T24] Swift：闭包
来源：http://isr.chenjidiqi.icu

let f = { (x: Int) -> Int in x * 2 }
来源：http://ngp.kuanghao11.cn

[T25] Swift：结构体
来源：http://gny.shanyushiyangtech.top

struct P { var x: Int }
来源：http://szp.jyoumei.cn

[T26] Swift：类与重写
来源：http://tlq.316326.xyz

class A: Base { override func f() {} }
来源：http://dov.jianghu66.top

[T27] Swift：错误处理
来源：http://jhn.xuetiantiany.cn

do { try f() } catch { print(error) }
来源：http://zti.hfpthk.cn

[T28] Swift：枚举
来源：http://rjb.gogol.net.cn

enum Color { case red, green }
来源：http://zhu.ydzc1.top

[T29] Swift：guard 提前返回
来源：http://yip.zhijiandao.cn

guard let x = opt else { return }
来源：http://ugo.jlsjyb.cn

[T30] Swift：协议
来源：http://lld.quarkkingdee.top

protocol Shape { func area() -> Double }
来源：http://fhm.hnqzz.top

[T31] Lua：Hello World
来源：http://dnx.gaohongyu789.top

print("Hello")
来源：http://iqz.yangfankeji.com

[T32] Lua：局部变量
来源：http://fiu.yangfankeji.com

local a = 1
来源：http://mws.jqgfzy.top

[T33] Lua：表（数组）
来源：http://vtn.daxiang520.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ity.fktsv.cn

[T34] Lua：遍历表
来源：http://vqk.epnwcf.com

for i, v in ipairs(t) do print(i, v) end
来源：http://pxc.zycfv.cn

[T35] Lua：字典表
来源：http://nyr.nanxuanxn.top

local d = { a = 1 };  d.b = 2
来源：http://nvg.yvedp.cn

[T36] Lua：函数
来源：http://coo.jyoumei.cn

function add(a, b) return a + b end
来源：http://qlt.uphjek.com

[T37] Lua：字符串拼接
来源：http://hvy.yanxiufei.cn

"a" .. "b"
来源：http://sbb.cheryme.top

[T38] Lua：条件
来源：http://phw.sxryk.cn

if x > 0 then print("正") end
来源：http://uqt.ybcxt.top

[T39] Lua：模式匹配
来源：http://mca.tian-w.cn

string.find(s, "%d+")
来源：http://fbe.guannengcc.top

[T40] Lua：元表
来源：http://fcj.ctjpmb.com

setmetatable({}, { __index = base })
来源：http://zku.fanxiaobao.xyz

[T41] Perl：Hello World
来源：http://kwc.bbcook.cn

print "Hello\n";
来源：http://vnb.yuxming.cn

[T42] Perl：变量类型
来源：http://caj.yuxming.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://oda.hongshengwenyu.top

[T43] Perl：字符串插值
来源：http://kzq.shanyushiyangtech.top

"值: $a"
来源：http://ahz.ppjwa.cn

[T44] Perl：条件
来源：http://wwr.xingfuxueyuan.xyz

if ($a > 0) { print "正"; }
来源：http://sbv.ehwqpu.com

[T45] Perl：数组遍历
来源：http://mnt.zdqjudy.top

for my $x (@arr) { print $x; }
来源：http://rnz.gaohongyu789.top

[T46] Perl：哈希操作
来源：http://uwc.dianchejie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xyi.ywan-chungtsiang.top

[T47] Perl：正则捕获
来源：http://lgu.hcnkem.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://xzj.aizwys.cn

[T48] Perl：正则替换
来源：http://iqz.hesvh.cn

$s =~ s/old/new/g;
来源：http://pfz.cdnleiting.top

[T49] Perl：函数
来源：http://dww.ydzc1.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gfl.svipenyu.cn

[T50] Perl：逐行读文件
来源：http://apn.zhengqikj.top

open my $fh, "<", "a.txt" or die $!;
来源：http://qzp.xingfuxueyuan.xyz

while (my $line = <$fh>) { print $line; }
来源：http://jwg.snrcjt.cn

[T51] Scala：Hello World
来源：http://mlu.yongpay.top

println("Hello")
来源：http://zns.tian-w.cn

[T52] Scala：变量
来源：http://gtc.zhijiandao.cn

val a = 1;  var b = 2
来源：http://aur.hfpthk.cn

[T53] Scala：字符串插值
来源：http://fim.andypj.xyz

s"值: $b"
来源：http://wgs.jqgfzy.top

[T54] Scala：集合映射
来源：http://egk.gogol.net.cn

List(1, 2, 3).map(_ * 2)
来源：http://tid.cheryme.top

[T55] Scala：集合过滤
来源：http://klx.kuanghao11.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ewv.fktsv.cn

[T56] Scala：样例类
来源：http://cqv.ybcxt.top

case class User(name: String, age: Int)
来源：http://vki.xingfuxueyuan.xyz

[T57] Scala：模式匹配
来源：http://amf.jqgufenzy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://oyx.c1oappe.top

[T58] Scala：函数定义
来源：http://oif.xuetiantiany.cn

def add(a: Int, b: Int): Int = a + b
来源：http://cql.jqgufenzy.top

[T59] Scala：循环
来源：http://trk.jinghuilouyu.cn

for (i <- 1 to 10) println(i)
来源：http://ivt.jinyuanbaomall.cn

[T60] Scala：折叠
来源：http://gfm.chenlongwang.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ljr.nanxuanxn.top

================================================================================
来源：http://jzi.bjfxy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lxz.fzhhl.top

================================================================================
来源：http://cdo.daxiang520.top

[U01] Py：创建虚拟环境
来源：http://zsj.fktsv.cn

python -m venv .venv && source .venv/bin/activate
来源：http://mra.hcnkem.com

[U02] Py：导出 / 安装依赖
来源：http://bav.shangyingyoupin.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ynn.vqdsnc.cn

[U03] Py：加载 .env 配置
来源：http://lzr.hfpthk.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://luv.yueranfly.top

[U04] Py：变量调试打印
来源：http://bdh.cheryme.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://swh.hesvh.cn

[U05] Py：列表去重且保序
来源：http://mrh.tarul.cn

list(dict.fromkeys(arr))
来源：http://zpl.pycfn.com

[U06] Py：合并两个字典
来源：http://cof.meibo888.top

{**a, **b}
来源：http://nvu.zdqjudy.top

[U07] Py：反转字典键值
来源：http://zlm.bjfxy.top

{v: k for k, v in d.items()}
来源：http://epe.yonumen.top

[U08] Py：展平二维列表
来源：http://fmj.smart0.xyz

[y for x in nested for y in x]
来源：http://pdo.bbcook.cn

[U09] Py：字典取最大值的键
来源：http://bcp.zhoulong.xyz

max(d, key=d.get)
来源：http://sxg.hesvh.cn

[U10] Py：按值排序字典
来源：http://osn.shangyingyoupin.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rpn.yueranfly.top

[U11] Py：生成器表达式
来源：http://vmx.ivvv.top

(x * 2 for x in arr)
来源：http://lqh.gotoacloud.top

[U12] Py：取出现最多的 3 个元素
来源：http://jri.hnqzz.top

Counter(arr).most_common(3)
来源：http://pjw.chenjidiqi.icu

[U13] Py：固定长度队列
来源：http://mjl.tarul.cn

deque(maxlen=10)
来源：http://wwh.gaohongyu789.top

[U14] Py：分组收集到列表
来源：http://wmw.xylfe.cn

defaultdict(list)
来源：http://ryt.pengpengdd.cyou

[U15] Py：高精度计时
来源：http://sas.gzhubu.top

t = time.perf_counter()
来源：http://bdk.ywan-chungtsiang.top

[U16] Py：命令行参数解析
来源：http://hwe.guowangkeji.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://shm.iojbl.cn

[U17] Py：初始化日志
来源：http://ada.guowangkeji.top

logging.basicConfig(level=logging.INFO)
来源：http://jdk.sysykeji.top

[U18] Py：预编译正则
来源：http://hma.nanxuanxn.top

pat = re.compile(r"\d+")
来源：http://qqk.yanxiufei.cn

[U19] Py：正则替换带回调
来源：http://osh.cqqwz.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qdg.jinghuilouyu.cn

[U20] Py：缓存函数结果
来源：http://cmb.sweek.top

@functools.lru_cache(maxsize=None)
来源：http://vto.zhongyouzk.top

[U21] Py：自定义上下文管理器
来源：http://hup.bbcook.cn

@contextlib.contextmanager
来源：http://byh.zhoulong.xyz

[U22] Py：矩阵转置
来源：http://vjk.xylfe.cn

list(zip(*m))
来源：http://qiw.chenjidiqi.icu

[U23] Py：分块读取大文件
来源：http://rov.hammf.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mea.xziqi.cn

[U24] Py：路径操作
来源：http://lfo.tianlin.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hql.zhixingplan.top

[U25] Py：CSV 按字典读
来源：http://xas.dianchejie.cn

csv.DictReader(f)
来源：http://pio.shzxlz.cn

[U26] Py：并发下载
来源：http://mgh.wangdashe.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hac.hcnkem.com

[U27] Py：异步 HTTP
来源：http://goq.meibo888.top

aiohttp.ClientSession() 配合 async with
来源：http://eeb.xuetiantiany.cn

[U28] Py：类型别名
来源：http://ycq.jlsjyb.cn

UserId = int
来源：http://twb.ydzc1.top

[U29] Py：属性校验
来源：http://rer.smart0.xyz

@property 与 @x.setter 配合
来源：http://dnc.chenlongwang.top

[U30] Py：数据类
来源：http://nnb.zhijiandao.cn

@dataclass(slots=True)
来源：http://rln.nanxinkj.top

[U31] Py：单测
来源：http://dsa.yuanzhike.top

python -m pytest -q
来源：http://uww.gotoacloud.top

[U32] Py：代码格式化
来源：http://hxr.shanyushiyangkeji.top

ruff format . && ruff check --fix .
来源：http://skg.yfazqb.com

[U33] Py：打包发布
来源：http://gwd.gogol.net.cn

python -m build  （依赖 pyproject.toml）
来源：http://cip.hongshengwenyu.top

[U34] Py：判断编码
来源：http://jsb.zhijiandao.cn

chardet.detect(raw)
来源：http://wee.jlsjyb.cn

[U35] Py：发送邮件
来源：http://kkq.yj20258888.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xju.ywan-chungtsiang.top

[U36] Py：定时任务
来源：http://may.gaohongyu789.top

schedule.every(10).minutes.do(job)
来源：http://cjp.fengsongda.top

[U37] Py：读写 Excel
来源：http://uqj.shuidangran.top

pandas.read_excel / DataFrame.to_excel
来源：http://ifh.bbcook.cn

[U38] Py：获取脚本所在目录
来源：http://jie.xylfe.cn

Path(__file__).resolve().parent
来源：http://lxd.daria6918.cn

[U39] Py：判断是否在交互环境
来源：http://qny.cheryme.top

sys.stdout.isatty()
来源：http://laz.kuanghao11.cn

[U40] Py：打印到标准错误
来源：http://vet.wangshuangyany.cn

print("err", file=sys.stderr)
来源：http://pfj.shanyushiyangkeji.top

[U41] PHP：初始化 Composer 项目
来源：http://dyf.bjfxy.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ltl.tianlin.xyz

[U42] PHP：PSR-4 自动加载
来源：http://axo.jiagoushi.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vqk.cdnleiting.top

[U43] PHP：声明命名空间
来源：http://uyr.gzhubu.top

namespace App\Http;
来源：http://amx.bbcook.cn

[U44] PHP：开启严格类型
来源：http://edy.0kj1m.cn

declare(strict_types=1);
来源：http://ksr.yuxming.cn

[U45] PHP：类型声明与返回类型
来源：http://ioj.gzhubu.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://nak.shanyushiyangkeji.top

[U46] PHP：可空类型
来源：http://ggq.cdnleiting.top

?string $name = null
来源：http://xdk.wangdashe.top

[U47] PHP：联合类型
来源：http://sfi.9152youxi.cn

int|string $id
来源：http://dlq.shzxlz.cn

[U48] PHP：纯枚举
来源：http://bmw.bbcook.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://irc.zhiwuduotai.top

[U49] PHP：只读属性
来源：http://nud.quarkkingdee.top

public readonly string $name
来源：http://hbd.ivvv.top

[U50] PHP：构造器属性提升
来源：http://hyz.bbcook.cn

public function __construct(private int $id) {}
来源：http://sir.zycfv.cn

[U51] PHP：数组解构
来源：http://tkh.kuanghao11.cn

[$a, $b] = $arr;
来源：http://bru.zhaomingkeji.xyz

[U52] PHP：箭头函数
来源：http://ovg.xinyue.icu

$double = fn($x) => $x * 2;
来源：http://oei.jiagoushi.top

[U53] PHP：空合并运算符
来源：http://tnf.0kj1m.cn

$v = $a ?? $b ?? "default";
来源：http://abp.chenzaomai.com

[U54] PHP：空安全调用
来源：http://sgg.haohaochexian.top

$obj?->method()
来源：http://jbj.tarul.cn

[U55] PHP：match 表达式
来源：http://dfw.cdnleiting.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ybk.yj202588.top

[U56] PHP：命名参数
来源：http://rwe.jyoumei.cn

f(a: 1, b: 2)
来源：http://bmx.yj20258.top

[U57] PHP：字符串插值
来源：http://rkx.gzhubu.top

"值: {$a}"
来源：http://gur.ivvv.top

[U58] PHP：数组三件套
来源：http://nnn.yj202588.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ayc.yj20258.top

[U59] PHP：自定义排序
来源：http://jgg.gogol.net.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jly.quarkkingdee.top

[U60] PHP：JSON 编解码
来源：http://cmv.shanyushiyangkeji.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lli.jqgufenzy.top

[U61] PHP：正则
来源：http://cul.jinghuilouyu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nhl.jlsjyb.cn

[U62] PHP：日期对象
来源：http://nsv.yonumen.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://btb.jinqigufen.top

[U63] PHP：文件读写
来源：http://cka.ydzc1.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://clj.shanyushiyangtech.top

[U64] PHP：目录遍历
来源：http://xft.fengsongda.top

glob("dir/*.php");  scandir("dir");
来源：http://shj.zhijiandao.cn


<!-- 参考信息 -->