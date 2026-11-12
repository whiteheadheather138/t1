代发 wailian999

[S35] C++：map
来源：http://cnr.shanyushiyangtech.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zpu.guannengcc.top

[S36] C++：unordered_map
来源：http://slc.52xcode.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yya.yonumen.top

[S37] C++：set
来源：http://zzw.yj20258.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ydh.hywenlv.cn

[S38] C++：排序
来源：http://txr.c1oappe.top

std::sort(v.begin(), v.end());
来源：http://nfc.yj20258.top

[S39] C++：自定义比较器排序
来源：http://rvh.ehwqpu.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xda.cdnleiting.top

[S40] C++：查找元素
来源：http://vqi.sjlbkw.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ohk.vehdjk.com

[S41] C++：类与构造函数
来源：http://rvj.yvedp.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://utu.chenzaomai.com

[S42] C++：继承与虚函数
来源：http://ajz.xingfuxueyuan.xyz

class B : public Base { public: void f() override {} };
来源：http://ffs.ydjk.org.cn

[S43] C++：智能指针
来源：http://sae.snrcjt.cn

auto p = std::make_unique<int>(5);
来源：http://myc.yvedp.cn

[S44] C++：引用传参
来源：http://hnn.fanxiaobao.xyz

void inc(int &x) { ++x; }
来源：http://mmb.dashuyun.cn

[S45] C++：lambda
来源：http://qlw.yj202588.top

auto add = [](int a, int b) { return a + b; };
来源：http://cwn.fzhhl.top

[S46] C++：函数模板
来源：http://xxs.xuanzx.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rlm.wangshuangyany.cn

[S47] C++：结构化绑定遍历
来源：http://wfg.hnqzz.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://azo.hesvh.cn

[S48] C++：逐行读文件
来源：http://qoj.mhx1999.top

std::ifstream in("a.txt");  std::string line;
来源：http://lkx.yj202588.top

while (std::getline(in, line)) { }
来源：http://mfc.zdqjudy.top

[S49] C++：写文件
来源：http://tgp.yonumen.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dhe.hywenlv.cn

[S50] C++：格式化数字
来源：http://sme.nanxinkj.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hnu.gaohongyu789.top

[S51] C++：显式类型转换
来源：http://zyb.ywan-chungtsiang.top

static_cast<double>(a) / b
来源：http://slc.c1oappe.top

[S52] C++：const 与 noexcept
来源：http://yse.sysykeji.top

int size() const noexcept { return n_; }
来源：http://rct.zhongyouzk.top

[S53] C++：移动语义
来源：http://xlp.jinqigfzy.top

std::vector<int> w = std::move(v);
来源：http://nga.ydzc1.top

[S54] C++：异常处理
来源：http://ztm.gzhubu.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dxo.yvedp.cn

[S55] C++：结构化绑定
来源：http://hmj.nanxuanxn.top

auto [a, b] = std::make_pair(1, 2);
来源：http://nwd.yvedp.cn

[S56] C++：optional
来源：http://kwi.ydzc1.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rtc.ivvv.top

[S57] C++：编译期常量
来源：http://upw.yonumen.top

constexpr int N = 10;
来源：http://xsr.hywenlv.cn

[S58] C++：命名空间
来源：http://zsy.daria6918.cn

namespace ns { int f() { return 1; } }
来源：http://vxz.yvedp.cn

[S59] C++：静态断言
来源：http://owx.chenzaomai.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hmj.tarul.cn

[S60] C++：遍历并删除元素
来源：http://fnc.zhoulong.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://eiv.0kj1m.cn

================================================================================
来源：http://xoq.cdnleiting.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cyc.redwolf501.top

================================================================================
来源：http://ljb.jyoumei.cn

[T01] Kotlin：Hello World
来源：http://lnq.ywan-chungtsiang.top

println("Hello")
来源：http://nzf.bjfxy.top

[T02] Kotlin：变量
来源：http://nri.xziqi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://moa.tianlin.xyz

[T03] Kotlin：字符串模板
来源：http://ykx.redwolf501.top

"值: $b"
来源：http://ssi.zhijiandao.cn

[T04] Kotlin：空安全
来源：http://bjd.zdqjudy.top

val n: String? = null;  n?.length
来源：http://exq.ybcxt.top

[T05] Kotlin：when 表达式
来源：http://srh.52xcode.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mee.fanxiaobao.xyz

[T06] Kotlin：集合映射
来源：http://kmi.mhx1999.top

listOf(1, 2, 3).map { it * 2 }
来源：http://arh.birdmap.top

[T07] Kotlin：集合过滤
来源：http://ssq.jianghu66.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://zss.316326.xyz

[T08] Kotlin：数据类
来源：http://jau.zhaomingkeji.xyz

data class User(val name: String, val age: Int)
来源：http://ntc.haohaochexian.top

[T09] Kotlin：扩展函数
来源：http://ywx.hnxiangtu.top

fun String.exclaim() = this + "!"
来源：http://uvs.cdnleiting.top

[T10] Kotlin：默认参数
来源：http://ely.jiagoushi.top

fun greet(name: String = "World") = "Hi $name"
来源：http://gqb.c1oappe.top

[T11] Kotlin：协程
来源：http://rrn.shzxlz.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://hec.aibaodan.cn

[T12] Kotlin：解构声明
来源：http://mgx.daxiang520.top

val (a, b) = Pair(1, 2)
来源：http://pdb.jiagoushi.top

[T13] Kotlin：只读 Map
来源：http://epy.dashuyun.cn

val m = mapOf("a" to 1)
来源：http://ryy.zdqjudy.top

[T14] Kotlin：循环
来源：http://ffh.gogol.net.cn

for (i in 1..10) println(i)
来源：http://aum.jlsjyb.cn

[T15] Kotlin：接口
来源：http://ecj.fengsongda.top

interface Shape { fun area(): Double }
来源：http://pfj.shangyingyoupin.top

[T16] Swift：Hello World
来源：http://lio.aizwys.cn

print("Hello")
来源：http://mcu.birdmap.top

[T17] Swift：变量与常量
来源：http://res.jinyuanbaomall.cn

var a = 1;  let b = 2
来源：http://gzl.fehbvm.com

[T18] Swift：字符串插值
来源：http://tsa.ywan-chungtsiang.top

"值: \(b)"
来源：http://bld.fktsv.cn

[T19] Swift：可选绑定
来源：http://fkq.cashguo.top

if let n = opt { print(n) }
来源：http://udt.pycfn.com

[T20] Swift：数组操作
来源：http://ptt.andypj.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://ugv.jqgfzy.top

[T21] Swift：遍历
来源：http://zju.zhoulong.xyz

for x in a { print(x) }
来源：http://she.quarkkingdee.top

[T22] Swift：字典
来源：http://qgl.hammf.cn

var d = ["a": 1];  d["b"] = 2
来源：http://wlx.zycfv.cn

[T23] Swift：函数
来源：http://lul.pycfn.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yht.xinyue.icu

[T24] Swift：闭包
来源：http://che.vehdjk.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://uvt.haohaochexian.top

[T25] Swift：结构体
来源：http://jdo.hysaishi.cn

struct P { var x: Int }
来源：http://bpg.yuanzhike.top

[T26] Swift：类与重写
来源：http://uhl.yj20258.top

class A: Base { override func f() {} }
来源：http://pcw.bjfxy.top

[T27] Swift：错误处理
来源：http://lrl.kuanghao11.cn

do { try f() } catch { print(error) }
来源：http://sic.tarul.cn

[T28] Swift：枚举
来源：http://yfv.kuanghao11.cn

enum Color { case red, green }
来源：http://ghl.gaohongyu789.top

[T29] Swift：guard 提前返回
来源：http://qtq.hammf.cn

guard let x = opt else { return }
来源：http://wmq.jinyuanbaomall.cn

[T30] Swift：协议
来源：http://hnl.zhaomingkeji.xyz

protocol Shape { func area() -> Double }
来源：http://oee.hongshengwenyu.top

[T31] Lua：Hello World
来源：http://zmp.daxiang520.top

print("Hello")
来源：http://kmf.shangyingyoupin.top

[T32] Lua：局部变量
来源：http://hnk.daxiang520.top

local a = 1
来源：http://lcp.jinyuanbaomall.cn

[T33] Lua：表（数组）
来源：http://cfp.wangshuangyany.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://yqn.quarkkingdee.top

[T34] Lua：遍历表
来源：http://lxw.gzhubu.top

for i, v in ipairs(t) do print(i, v) end
来源：http://gnk.hesvh.cn

[T35] Lua：字典表
来源：http://gqe.cashguo.top

local d = { a = 1 };  d.b = 2
来源：http://nzj.chenlongwang.top

[T36] Lua：函数
来源：http://mjn.yuanzhike.top

function add(a, b) return a + b end
来源：http://gfl.uphjek.com

[T37] Lua：字符串拼接
来源：http://pqt.guannengcc.top

"a" .. "b"
来源：http://tgf.yj20258888.top

[T38] Lua：条件
来源：http://toi.kuanghao11.cn

if x > 0 then print("正") end
来源：http://ove.316326.xyz

[T39] Lua：模式匹配
来源：http://boi.yvedp.cn

string.find(s, "%d+")
来源：http://zrk.xuetiantiany.cn

[T40] Lua：元表
来源：http://pxq.xuanzx.com

setmetatable({}, { __index = base })
来源：http://ktd.ppjwa.cn

[T41] Perl：Hello World
来源：http://czz.zycfv.cn

print "Hello\n";
来源：http://kld.ywan-chungtsiang.top

[T42] Perl：变量类型
来源：http://dtv.yj20258888.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nso.quarkkingdee.top

[T43] Perl：字符串插值
来源：http://eqj.yuanzhike.top

"值: $a"
来源：http://ajw.quarkkingdee.top

[T44] Perl：条件
来源：http://cuw.hongshengwenyu.top

if ($a > 0) { print "正"; }
来源：http://oqg.ywan-chungtsiang.top

[T45] Perl：数组遍历
来源：http://bhw.chenjidiqi.icu

for my $x (@arr) { print $x; }
来源：http://cfa.fktsv.cn

[T46] Perl：哈希操作
来源：http://cbc.yj202588.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://izn.ivvv.top

[T47] Perl：正则捕获
来源：http://xjk.andypj.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://dap.yuanzhike.top

[T48] Perl：正则替换
来源：http://ywq.zdqjudy.top

$s =~ s/old/new/g;
来源：http://enj.pycfn.com

[T49] Perl：函数
来源：http://dqh.pycfn.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wqe.xuetiantiany.cn

[T50] Perl：逐行读文件
来源：http://eyk.fktsv.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://wvk.zhixingplan.top

while (my $line = <$fh>) { print $line; }
来源：http://izv.jyoumei.cn

[T51] Scala：Hello World
来源：http://dbv.yonumen.top

println("Hello")
来源：http://nrr.dashuyun.cn

[T52] Scala：变量
来源：http://jtv.chenlongwang.top

val a = 1;  var b = 2
来源：http://awn.hongshengwenyu.top

[T53] Scala：字符串插值
来源：http://wtg.ydzc1.top

s"值: $b"
来源：http://nfk.fktsv.cn

[T54] Scala：集合映射
来源：http://dak.aizwys.cn

List(1, 2, 3).map(_ * 2)
来源：http://rkn.zhongyouzk.top

[T55] Scala：集合过滤
来源：http://xjs.yuxming.cn

List(1, 2, 3).filter(_ > 1)
来源：http://run.hywenlv.cn

[T56] Scala：样例类
来源：http://adu.daria6918.cn

case class User(name: String, age: Int)
来源：http://lml.jqgfzy.top

[T57] Scala：模式匹配
来源：http://blm.hywenlv.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://yum.hysaishi.cn

[T58] Scala：函数定义
来源：http://rkh.mhx1999.top

def add(a: Int, b: Int): Int = a + b
来源：http://jpj.sufxvd.cn

[T59] Scala：循环
来源：http://kcr.hongshengwenyu.top

for (i <- 1 to 10) println(i)
来源：http://fog.hesvh.cn

[T60] Scala：折叠
来源：http://ysh.ywan-chungtsiang.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ryc.daxiang520.top

================================================================================
来源：http://uya.yongpay.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fzv.hammf.cn

================================================================================
来源：http://gpt.jqgufenzy.top

[U01] Py：创建虚拟环境
来源：http://dum.vqdsnc.cn

python -m venv .venv && source .venv/bin/activate
来源：http://zvp.zhijiandao.cn

[U02] Py：导出 / 安装依赖
来源：http://mmv.guannengcc.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jes.yfazqb.com

[U03] Py：加载 .env 配置
来源：http://qxb.cdnleiting.top

from dotenv import load_dotenv; load_dotenv()
来源：http://hla.fengsongda.top

[U04] Py：变量调试打印
来源：http://yze.chenzaomai.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ghb.quarkkingdee.top

[U05] Py：列表去重且保序
来源：http://lgg.hammf.cn

list(dict.fromkeys(arr))
来源：http://vcf.zhixingplan.top

[U06] Py：合并两个字典
来源：http://ttt.snrcjt.cn

{**a, **b}
来源：http://eai.yanxiufei.cn

[U07] Py：反转字典键值
来源：http://hfe.nwbrower.top

{v: k for k, v in d.items()}
来源：http://qfw.cucudq.cn

[U08] Py：展平二维列表
来源：http://coo.hywenlv.cn

[y for x in nested for y in x]
来源：http://xuc.zhijiandao.cn

[U09] Py：字典取最大值的键
来源：http://nje.gogol.net.cn

max(d, key=d.get)
来源：http://tjj.vehdjk.com

[U10] Py：按值排序字典
来源：http://gpu.nanxuanxn.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ayf.aizwys.cn

[U11] Py：生成器表达式
来源：http://cyz.sxryk.cn

(x * 2 for x in arr)
来源：http://alj.zhengqikj.top

[U12] Py：取出现最多的 3 个元素
来源：http://man.wangshuangyany.cn

Counter(arr).most_common(3)
来源：http://uav.tian-w.cn

[U13] Py：固定长度队列
来源：http://jkv.cucudq.cn

deque(maxlen=10)
来源：http://btg.daria6918.cn

[U14] Py：分组收集到列表
来源：http://zqj.jianghu66.top

defaultdict(list)
来源：http://wwl.svipenyu.cn

[U15] Py：高精度计时
来源：http://exj.hesvh.cn

t = time.perf_counter()
来源：http://pbb.cdnleiting.top

[U16] Py：命令行参数解析
来源：http://jea.hysaishi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://tzx.zycfv.cn

[U17] Py：初始化日志
来源：http://kxb.zhengqikj.top

logging.basicConfig(level=logging.INFO)
来源：http://jck.fengsongda.top

[U18] Py：预编译正则
来源：http://laa.jinqigufen.top

pat = re.compile(r"\d+")
来源：http://uou.aizwys.cn

[U19] Py：正则替换带回调
来源：http://vdr.cdnleiting.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kiz.jiagoushi.top

[U20] Py：缓存函数结果
来源：http://bpl.yonumen.top

@functools.lru_cache(maxsize=None)
来源：http://gxi.cqqwz.cn

[U21] Py：自定义上下文管理器
来源：http://itm.ehwqpu.com

@contextlib.contextmanager
来源：http://edt.nanxinkj.top

[U22] Py：矩阵转置
来源：http://xyl.meibo888.top

list(zip(*m))
来源：http://swn.jinqigfzy.top

[U23] Py：分块读取大文件
来源：http://rfr.zhijiandao.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bxv.hammf.cn

[U24] Py：路径操作
来源：http://oka.jinghuilouyu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://znl.vehdjk.com

[U25] Py：CSV 按字典读
来源：http://khs.xingfuxueyuan.xyz

csv.DictReader(f)
来源：http://imf.shanyushiyangtech.top

[U26] Py：并发下载
来源：http://gvb.kuanghao11.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://smh.xuetiantiany.cn

[U27] Py：异步 HTTP
来源：http://dps.9152youxi.cn

aiohttp.ClientSession() 配合 async with
来源：http://wtl.hongshengwenyu.top

[U28] Py：类型别名
来源：http://hsk.yonumen.top

UserId = int
来源：http://mkk.hongshengwenyu.top

[U29] Py：属性校验
来源：http://kzp.cheryme.top

@property 与 @x.setter 配合
来源：http://afn.c1oappe.top

[U30] Py：数据类
来源：http://epq.hywenlv.cn

@dataclass(slots=True)
来源：http://fmz.jinghuilouyu.cn

[U31] Py：单测
来源：http://wqc.tanke756.top

python -m pytest -q
来源：http://zli.jinghuilouyu.cn

[U32] Py：代码格式化
来源：http://fzq.hesvh.cn

ruff format . && ruff check --fix .
来源：http://hgu.birdmap.top

[U33] Py：打包发布
来源：http://rfa.sjlbkw.cn

python -m build  （依赖 pyproject.toml）
来源：http://ppm.pycfn.com

[U34] Py：判断编码
来源：http://ufr.shanyushiyangtech.top

chardet.detect(raw)
来源：http://bch.yuxming.cn

[U35] Py：发送邮件
来源：http://wgz.cqqwz.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ugr.gaohongyu789.top

[U36] Py：定时任务
来源：http://uji.xinyue.icu

schedule.every(10).minutes.do(job)
来源：http://bce.hnxiangtu.top

[U37] Py：读写 Excel
来源：http://nnl.shangyingyoupin.top

pandas.read_excel / DataFrame.to_excel
来源：http://yor.uphjek.com

[U38] Py：获取脚本所在目录
来源：http://bid.cashguo.top

Path(__file__).resolve().parent
来源：http://gtu.sufxvd.cn

[U39] Py：判断是否在交互环境
来源：http://jgp.ywan-chungtsiang.top

sys.stdout.isatty()
来源：http://dtw.snrcjt.cn

[U40] Py：打印到标准错误
来源：http://mgt.ehwqpu.com

print("err", file=sys.stderr)
来源：http://fpg.cashguo.top

[U41] PHP：初始化 Composer 项目
来源：http://bus.shanyushiyangkeji.top

composer init;  composer require guzzlehttp/guzzle
来源：http://wlt.sxryk.cn

[U42] PHP：PSR-4 自动加载
来源：http://out.yueranfly.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://iju.shangyingyoupin.top

[U43] PHP：声明命名空间
来源：http://rlb.pycfn.com

namespace App\Http;
来源：http://rqk.ivvv.top

[U44] PHP：开启严格类型
来源：http://sye.fengsongda.top

declare(strict_types=1);
来源：http://txx.sufxvd.cn

[U45] PHP：类型声明与返回类型
来源：http://vgn.xuetiantiany.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://vvl.cheryme.top

[U46] PHP：可空类型
来源：http://akj.9152youxi.cn

?string $name = null
来源：http://xgw.yonumen.top

[U47] PHP：联合类型
来源：http://evq.xuetiantiany.cn

int|string $id
来源：http://hww.ywan-chungtsiang.top

[U48] PHP：纯枚举
来源：http://zsj.tian-w.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://iqw.yvedp.cn

[U49] PHP：只读属性
来源：http://ovl.hysaishi.cn

public readonly string $name
来源：http://vbf.cucudq.cn

[U50] PHP：构造器属性提升
来源：http://zyv.yongpay.top

public function __construct(private int $id) {}
来源：http://ogm.xingfuxueyuan.xyz

[U51] PHP：数组解构
来源：http://szw.nanxinkj.top

[$a, $b] = $arr;
来源：http://dxj.pengpengdd.cyou

[U52] PHP：箭头函数
来源：http://sgj.epnwcf.com

$double = fn($x) => $x * 2;
来源：http://kaq.hnqzz.top

[U53] PHP：空合并运算符
来源：http://caz.zhoulong.xyz

$v = $a ?? $b ?? "default";
来源：http://hkp.hcnkem.com

[U54] PHP：空安全调用
来源：http://gic.hammf.cn

$obj?->method()
来源：http://fnt.tanke756.top

[U55] PHP：match 表达式
来源：http://vln.gaohongyu789.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fvq.xuanzx.com

[U56] PHP：命名参数
来源：http://xsc.yj20258888.top

f(a: 1, b: 2)
来源：http://qde.sjlbkw.cn

[U57] PHP：字符串插值
来源：http://pnw.uphjek.com

"值: {$a}"
来源：http://ayh.bjfxy.top

[U58] PHP：数组三件套
来源：http://ohb.hfpthk.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ijv.shanyushiyangkeji.top

[U59] PHP：自定义排序
来源：http://bkz.hongshengwenyu.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://klh.yanxiufei.cn

[U60] PHP：JSON 编解码
来源：http://mof.gaohongyu789.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hzv.daria6918.cn


<!-- 参考信息 -->