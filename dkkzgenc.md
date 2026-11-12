代发 wailian999

[S37] C++：set
来源：http://qrz.zhongyouzk.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ixd.aibaodan.cn

[S38] C++：排序
来源：http://qhn.jianghu66.top

std::sort(v.begin(), v.end());
来源：http://vbn.jinyuanbaomall.cn

[S39] C++：自定义比较器排序
来源：http://fue.mhx1999.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mxx.havefunace.top

[S40] C++：查找元素
来源：http://zyc.mhx1999.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dpj.fengsongda.top

[S41] C++：类与构造函数
来源：http://frs.cdnleiting.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kgc.yj20258888.top

[S42] C++：继承与虚函数
来源：http://hoi.chenjidiqi.icu

class B : public Base { public: void f() override {} };
来源：http://ivh.jinyuanbaomall.cn

[S43] C++：智能指针
来源：http://oev.daxiang520.top

auto p = std::make_unique<int>(5);
来源：http://gau.xuetiantiany.cn

[S44] C++：引用传参
来源：http://ucq.daxiang520.top

void inc(int &x) { ++x; }
来源：http://gsk.jqgfzy.top

[S45] C++：lambda
来源：http://dme.sufxvd.cn

auto add = [](int a, int b) { return a + b; };
来源：http://vfb.zhixingplan.top

[S46] C++：函数模板
来源：http://kki.ywan-chungtsiang.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://amu.gotoacloud.top

[S47] C++：结构化绑定遍历
来源：http://jyn.yuxming.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vrn.ehwqpu.com

[S48] C++：逐行读文件
来源：http://cif.vqdsnc.cn

std::ifstream in("a.txt");  std::string line;
来源：http://lbh.daxiang520.top

while (std::getline(in, line)) { }
来源：http://tum.hammf.cn

[S49] C++：写文件
来源：http://orf.yanxiufei.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ceb.jqgfzy.top

[S50] C++：格式化数字
来源：http://qun.jiagoushi.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://uys.jlsjyb.cn

[S51] C++：显式类型转换
来源：http://xxt.yongpay.top

static_cast<double>(a) / b
来源：http://bmo.jqgfzy.top

[S52] C++：const 与 noexcept
来源：http://cpx.316326.xyz

int size() const noexcept { return n_; }
来源：http://xpl.hesvh.cn

[S53] C++：移动语义
来源：http://aqy.tanke756.top

std::vector<int> w = std::move(v);
来源：http://fcm.yfazqb.com

[S54] C++：异常处理
来源：http://cyr.zycfv.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://aur.quarkkingdee.top

[S55] C++：结构化绑定
来源：http://usu.xuetiantiany.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://tfy.jinqigfzy.top

[S56] C++：optional
来源：http://ndf.zdbjq.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://sqn.gogol.net.cn

[S57] C++：编译期常量
来源：http://wyv.tanke756.top

constexpr int N = 10;
来源：http://oeo.aizwys.cn

[S58] C++：命名空间
来源：http://vlj.birdmap.top

namespace ns { int f() { return 1; } }
来源：http://ivz.shanyushiyangkeji.top

[S59] C++：静态断言
来源：http://ojw.xingfuxueyuan.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mam.nwbrower.top

[S60] C++：遍历并删除元素
来源：http://ihq.fanxiaobao.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hpt.cucudq.cn

================================================================================
来源：http://nie.zhoulong.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xwo.sysykeji.top

================================================================================
来源：http://nhq.zhixingplan.top

[T01] Kotlin：Hello World
来源：http://det.hfpthk.cn

println("Hello")
来源：http://emu.fzhhl.top

[T02] Kotlin：变量
来源：http://rpe.jinqigfzy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hec.havefunace.top

[T03] Kotlin：字符串模板
来源：http://lol.hcnkem.com

"值: $b"
来源：http://gwg.vehdjk.com

[T04] Kotlin：空安全
来源：http://drf.ydzc1.top

val n: String? = null;  n?.length
来源：http://jrf.daxiang520.top

[T05] Kotlin：when 表达式
来源：http://zqs.mhx1999.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yij.snrcjt.cn

[T06] Kotlin：集合映射
来源：http://mrf.vehdjk.com

listOf(1, 2, 3).map { it * 2 }
来源：http://apa.zhongyouzk.top

[T07] Kotlin：集合过滤
来源：http://dlw.iojbl.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://igf.sysykeji.top

[T08] Kotlin：数据类
来源：http://ltr.zhoulong.xyz

data class User(val name: String, val age: Int)
来源：http://rdk.cheryme.top

[T09] Kotlin：扩展函数
来源：http://tsg.dianchejie.cn

fun String.exclaim() = this + "!"
来源：http://zhv.jyoumei.cn

[T10] Kotlin：默认参数
来源：http://rle.chenzaomai.com

fun greet(name: String = "World") = "Hi $name"
来源：http://uty.zhaomingkeji.xyz

[T11] Kotlin：协程
来源：http://xlb.ybcxt.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://dru.ivvv.top

[T12] Kotlin：解构声明
来源：http://byf.chenzaomai.com

val (a, b) = Pair(1, 2)
来源：http://vuy.tanke756.top

[T13] Kotlin：只读 Map
来源：http://oer.svipenyu.cn

val m = mapOf("a" to 1)
来源：http://sys.zhixingplan.top

[T14] Kotlin：循环
来源：http://ini.yuxming.cn

for (i in 1..10) println(i)
来源：http://jqi.cqqwz.cn

[T15] Kotlin：接口
来源：http://xup.havefunace.top

interface Shape { fun area(): Double }
来源：http://ktv.snrcjt.cn

[T16] Swift：Hello World
来源：http://yyt.fktsv.cn

print("Hello")
来源：http://vsr.jiagoushi.top

[T17] Swift：变量与常量
来源：http://vku.yj20258888.top

var a = 1;  let b = 2
来源：http://weo.gogol.net.cn

[T18] Swift：字符串插值
来源：http://owo.hysaishi.cn

"值: \(b)"
来源：http://gpe.yuanzhike.top

[T19] Swift：可选绑定
来源：http://jud.9152youxi.cn

if let n = opt { print(n) }
来源：http://unn.xuetiantiany.cn

[T20] Swift：数组操作
来源：http://gbh.fengsongda.top

var a = [1, 2, 3];  a.append(4)
来源：http://ycd.shanyushiyangtech.top

[T21] Swift：遍历
来源：http://dew.yonumen.top

for x in a { print(x) }
来源：http://zcs.iojbl.cn

[T22] Swift：字典
来源：http://aec.shuidangran.top

var d = ["a": 1];  d["b"] = 2
来源：http://dwe.cucudq.cn

[T23] Swift：函数
来源：http://mrn.jqgufenzy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lyy.bjfxy.top

[T24] Swift：闭包
来源：http://los.fehbvm.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://hnv.pycfn.com

[T25] Swift：结构体
来源：http://scf.xuetiantiany.cn

struct P { var x: Int }
来源：http://xkn.dashuyun.cn

[T26] Swift：类与重写
来源：http://hpj.tanke756.top

class A: Base { override func f() {} }
来源：http://fii.zhoulong.xyz

[T27] Swift：错误处理
来源：http://azo.hywenlv.cn

do { try f() } catch { print(error) }
来源：http://rph.quarkkingdee.top

[T28] Swift：枚举
来源：http://wqh.nwbrower.top

enum Color { case red, green }
来源：http://hjv.jinqigfzy.top

[T29] Swift：guard 提前返回
来源：http://ilk.smart0.xyz

guard let x = opt else { return }
来源：http://ihl.chenlongwang.top

[T30] Swift：协议
来源：http://rbt.mhx1999.top

protocol Shape { func area() -> Double }
来源：http://ifu.bbcook.cn

[T31] Lua：Hello World
来源：http://iaz.0kj1m.cn

print("Hello")
来源：http://otp.hysaishi.cn

[T32] Lua：局部变量
来源：http://hgi.aizwys.cn

local a = 1
来源：http://mtu.dashuyun.cn

[T33] Lua：表（数组）
来源：http://ipg.0kj1m.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://gde.pengpengdd.cyou

[T34] Lua：遍历表
来源：http://vkg.shuidangran.top

for i, v in ipairs(t) do print(i, v) end
来源：http://gcm.gaohongyu789.top

[T35] Lua：字典表
来源：http://pwt.ybcxt.top

local d = { a = 1 };  d.b = 2
来源：http://leq.0kj1m.cn

[T36] Lua：函数
来源：http://yvh.xuanzx.com

function add(a, b) return a + b end
来源：http://uln.shanyushiyangkeji.top

[T37] Lua：字符串拼接
来源：http://jyh.cqqwz.cn

"a" .. "b"
来源：http://nar.xziqi.cn

[T38] Lua：条件
来源：http://zhz.fktsv.cn

if x > 0 then print("正") end
来源：http://rek.cheryme.top

[T39] Lua：模式匹配
来源：http://wdh.quarkkingdee.top

string.find(s, "%d+")
来源：http://bkt.snrcjt.cn

[T40] Lua：元表
来源：http://hzq.smart0.xyz

setmetatable({}, { __index = base })
来源：http://mib.gaohongyu789.top

[T41] Perl：Hello World
来源：http://llx.epnwcf.com

print "Hello\n";
来源：http://cxu.cheryme.top

[T42] Perl：变量类型
来源：http://rsp.fanxiaobao.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nfc.ydjk.org.cn

[T43] Perl：字符串插值
来源：http://ums.jinghuilouyu.cn

"值: $a"
来源：http://phu.shangyingyoupin.top

[T44] Perl：条件
来源：http://qvy.chenjidiqi.icu

if ($a > 0) { print "正"; }
来源：http://lex.hfpthk.cn

[T45] Perl：数组遍历
来源：http://fty.redwolf501.top

for my $x (@arr) { print $x; }
来源：http://ccj.52xcode.cn

[T46] Perl：哈希操作
来源：http://rne.ywan-chungtsiang.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rnj.quarkkingdee.top

[T47] Perl：正则捕获
来源：http://xly.shanyushiyangkeji.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://bva.dianchejie.cn

[T48] Perl：正则替换
来源：http://ctw.nwbrower.top

$s =~ s/old/new/g;
来源：http://kps.aizwys.cn

[T49] Perl：函数
来源：http://our.zhoulong.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://csf.hnqzz.top

[T50] Perl：逐行读文件
来源：http://jmb.yfazqb.com

open my $fh, "<", "a.txt" or die $!;
来源：http://nat.vehdjk.com

while (my $line = <$fh>) { print $line; }
来源：http://qie.hammf.cn

[T51] Scala：Hello World
来源：http://lje.zycfv.cn

println("Hello")
来源：http://ceb.haohaochexian.top

[T52] Scala：变量
来源：http://afu.yj202588.top

val a = 1;  var b = 2
来源：http://dqz.yuanzhike.top

[T53] Scala：字符串插值
来源：http://jdc.havefunace.top

s"值: $b"
来源：http://fwb.yongpay.top

[T54] Scala：集合映射
来源：http://jzu.zhixingplan.top

List(1, 2, 3).map(_ * 2)
来源：http://gwj.sjlbkw.cn

[T55] Scala：集合过滤
来源：http://ebu.cheryme.top

List(1, 2, 3).filter(_ > 1)
来源：http://vng.yj202588.top

[T56] Scala：样例类
来源：http://isg.yanxiufei.cn

case class User(name: String, age: Int)
来源：http://yea.tianlin.xyz

[T57] Scala：模式匹配
来源：http://eir.yj202588.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://rsu.xinyue.icu

[T58] Scala：函数定义
来源：http://num.ydjk.org.cn

def add(a: Int, b: Int): Int = a + b
来源：http://jeg.kuanghao11.cn

[T59] Scala：循环
来源：http://xam.zdqjudy.top

for (i <- 1 to 10) println(i)
来源：http://mcv.yfazqb.com

[T60] Scala：折叠
来源：http://say.dashuyun.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://eui.jqgufenzy.top

================================================================================
来源：http://xwp.52xcode.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jag.zdqjudy.top

================================================================================
来源：http://yjg.sxryk.cn

[U01] Py：创建虚拟环境
来源：http://xzw.vqdsnc.cn

python -m venv .venv && source .venv/bin/activate
来源：http://aca.mhx1999.top

[U02] Py：导出 / 安装依赖
来源：http://rry.wangdashe.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yex.feifeiyinyue.top

[U03] Py：加载 .env 配置
来源：http://zsa.yangfankeji.com

from dotenv import load_dotenv; load_dotenv()
来源：http://ivt.c1oappe.top

[U04] Py：变量调试打印
来源：http://shy.ybcxt.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://msv.yuanzhike.top

[U05] Py：列表去重且保序
来源：http://pjj.xuanzx.com

list(dict.fromkeys(arr))
来源：http://dby.9152youxi.cn

[U06] Py：合并两个字典
来源：http://row.shangyingyoupin.top

{**a, **b}
来源：http://ioe.xingfuxueyuan.xyz

[U07] Py：反转字典键值
来源：http://izu.zhiwuduotai.top

{v: k for k, v in d.items()}
来源：http://nlp.feifeiyinyue.top

[U08] Py：展平二维列表
来源：http://pxb.yanxiufei.cn

[y for x in nested for y in x]
来源：http://juc.shanyushiyangkeji.top

[U09] Py：字典取最大值的键
来源：http://nfy.jinqigfzy.top

max(d, key=d.get)
来源：http://esq.jinghuilouyu.cn

[U10] Py：按值排序字典
来源：http://zbg.ywan-chungtsiang.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nkl.shangyingyoupin.top

[U11] Py：生成器表达式
来源：http://fkr.chenzaomai.com

(x * 2 for x in arr)
来源：http://rph.zhiwuduotai.top

[U12] Py：取出现最多的 3 个元素
来源：http://lli.mhx1999.top

Counter(arr).most_common(3)
来源：http://ffz.bbcook.cn

[U13] Py：固定长度队列
来源：http://atu.hongshengwenyu.top

deque(maxlen=10)
来源：http://zbs.ydjk.org.cn

[U14] Py：分组收集到列表
来源：http://yzd.sxryk.cn

defaultdict(list)
来源：http://lrv.chenzaomai.com

[U15] Py：高精度计时
来源：http://uuj.hysaishi.cn

t = time.perf_counter()
来源：http://jlx.jqgfzy.top

[U16] Py：命令行参数解析
来源：http://zqz.nwbrower.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xnm.daxiang520.top

[U17] Py：初始化日志
来源：http://vkc.dianchejie.cn

logging.basicConfig(level=logging.INFO)
来源：http://vka.uphjek.com

[U18] Py：预编译正则
来源：http://kdt.sufxvd.cn

pat = re.compile(r"\d+")
来源：http://mfk.mhx1999.top

[U19] Py：正则替换带回调
来源：http://hts.fengsongda.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yjh.havefunace.top

[U20] Py：缓存函数结果
来源：http://itj.ctjpmb.com

@functools.lru_cache(maxsize=None)
来源：http://weg.cdnleiting.top

[U21] Py：自定义上下文管理器
来源：http://hby.pengpengdd.cyou

@contextlib.contextmanager
来源：http://lkr.gaohongyu789.top

[U22] Py：矩阵转置
来源：http://plf.cqqwz.cn

list(zip(*m))
来源：http://hfr.aizwys.cn

[U23] Py：分块读取大文件
来源：http://bog.haohaochexian.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://iba.yfazqb.com

[U24] Py：路径操作
来源：http://jhr.sxryk.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bsm.xuetiantiany.cn

[U25] Py：CSV 按字典读
来源：http://yuv.cdnleiting.top

csv.DictReader(f)
来源：http://vka.yj20258.top

[U26] Py：并发下载
来源：http://zaz.c1oappe.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vgg.guowangkeji.top

[U27] Py：异步 HTTP
来源：http://crs.sxryk.cn

aiohttp.ClientSession() 配合 async with
来源：http://rnx.yj20258.top

[U28] Py：类型别名
来源：http://bzg.kuanghao11.cn

UserId = int
来源：http://fli.zhixingplan.top

[U29] Py：属性校验
来源：http://ans.redwolf501.top

@property 与 @x.setter 配合
来源：http://buy.sxryk.cn

[U30] Py：数据类
来源：http://gno.ydzc1.top

@dataclass(slots=True)
来源：http://kvz.hfpthk.cn

[U31] Py：单测
来源：http://hqq.uphjek.com

python -m pytest -q
来源：http://ell.kuanghao11.cn

[U32] Py：代码格式化
来源：http://qvs.jlsjyb.cn

ruff format . && ruff check --fix .
来源：http://nte.gaohongyu789.top

[U33] Py：打包发布
来源：http://kri.ehwqpu.com

python -m build  （依赖 pyproject.toml）
来源：http://rgh.yuxming.cn

[U34] Py：判断编码
来源：http://vfb.yonumen.top

chardet.detect(raw)
来源：http://bpv.sjlbkw.cn

[U35] Py：发送邮件
来源：http://ekd.yangfankeji.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dyw.hywenlv.cn

[U36] Py：定时任务
来源：http://ths.chenzaomai.com

schedule.every(10).minutes.do(job)
来源：http://tlv.sysykeji.top

[U37] Py：读写 Excel
来源：http://kut.shangyingyoupin.top

pandas.read_excel / DataFrame.to_excel
来源：http://smw.vehdjk.com

[U38] Py：获取脚本所在目录
来源：http://kyo.yj20258.top

Path(__file__).resolve().parent
来源：http://inc.iojbl.cn

[U39] Py：判断是否在交互环境
来源：http://hro.guowangkeji.top

sys.stdout.isatty()
来源：http://lmy.yj202588.top

[U40] Py：打印到标准错误
来源：http://hol.snrcjt.cn

print("err", file=sys.stderr)
来源：http://hdv.gotoacloud.top

[U41] PHP：初始化 Composer 项目
来源：http://vyh.hongshengwenyu.top

composer init;  composer require guzzlehttp/guzzle
来源：http://snv.jinyuanbaomall.cn

[U42] PHP：PSR-4 自动加载
来源：http://peu.ydzc1.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fxw.quarkkingdee.top

[U43] PHP：声明命名空间
来源：http://baw.shangyingyoupin.top

namespace App\Http;
来源：http://yal.redwolf501.top

[U44] PHP：开启严格类型
来源：http://zyk.ivvv.top

declare(strict_types=1);
来源：http://qxz.cqqwz.cn

[U45] PHP：类型声明与返回类型
来源：http://ouj.ivvv.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://awe.xuetiantiany.cn

[U46] PHP：可空类型
来源：http://uia.sysykeji.top

?string $name = null
来源：http://qqz.quarkkingdee.top

[U47] PHP：联合类型
来源：http://nmu.yanxiufei.cn

int|string $id
来源：http://zrp.shanyushiyangkeji.top

[U48] PHP：纯枚举
来源：http://rpl.gotoacloud.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kwp.yvedp.cn

[U49] PHP：只读属性
来源：http://lsr.hywenlv.cn

public readonly string $name
来源：http://dcp.chenzaomai.com

[U50] PHP：构造器属性提升
来源：http://nct.ybcxt.top

public function __construct(private int $id) {}
来源：http://mqz.andypj.xyz

[U51] PHP：数组解构
来源：http://url.zhiwuduotai.top

[$a, $b] = $arr;
来源：http://rub.cucudq.cn

[U52] PHP：箭头函数
来源：http://jmu.haohaochexian.top

$double = fn($x) => $x * 2;
来源：http://yaj.zhaomingkeji.xyz

[U53] PHP：空合并运算符
来源：http://peo.yongpay.top

$v = $a ?? $b ?? "default";
来源：http://ilp.dashuyun.cn

[U54] PHP：空安全调用
来源：http://vbe.gotoacloud.top

$obj?->method()
来源：http://ocs.fanxiaobao.xyz

[U55] PHP：match 表达式
来源：http://vur.cdnleiting.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://nlj.zhaomingkeji.xyz

[U56] PHP：命名参数
来源：http://feu.bjfxy.top

f(a: 1, b: 2)
来源：http://pmg.zdbjq.cn

[U57] PHP：字符串插值
来源：http://hvm.wangdashe.top

"值: {$a}"
来源：http://hye.jinqigufen.top

[U58] PHP：数组三件套
来源：http://lgg.wangdashe.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fwa.52xcode.cn

[U59] PHP：自定义排序
来源：http://aov.ivvv.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hkx.sjlbkw.cn

[U60] PHP：JSON 编解码
来源：http://mci.yueranfly.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://uvp.jinqigufen.top

[U61] PHP：正则
来源：http://aap.sysykeji.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dtf.jinqigufen.top

[U62] PHP：日期对象
来源：http://xgk.zhaomingkeji.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hfo.aizwys.cn


<!-- 参考信息 -->