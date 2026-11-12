代发 wailian999

[S37] C++：set
来源：http://llj.chenlongwang.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yav.ydjk.org.cn

[S38] C++：排序
来源：http://btp.hywenlv.cn

std::sort(v.begin(), v.end());
来源：http://tmg.shzxlz.cn

[S39] C++：自定义比较器排序
来源：http://cct.shuidangran.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ibw.wangshuangyany.cn

[S40] C++：查找元素
来源：http://wyg.9152youxi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://age.zhoulong.xyz

[S41] C++：类与构造函数
来源：http://ryb.yueranfly.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vxq.zhoulong.xyz

[S42] C++：继承与虚函数
来源：http://qci.fktsv.cn

class B : public Base { public: void f() override {} };
来源：http://mrx.yueranfly.top

[S43] C++：智能指针
来源：http://jkb.ivvv.top

auto p = std::make_unique<int>(5);
来源：http://asw.sxryk.cn

[S44] C++：引用传参
来源：http://dkh.nanxuanxn.top

void inc(int &x) { ++x; }
来源：http://kwf.yj20258888.top

[S45] C++：lambda
来源：http://hbv.fengsongda.top

auto add = [](int a, int b) { return a + b; };
来源：http://xfc.sufxvd.cn

[S46] C++：函数模板
来源：http://zsq.hywenlv.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qid.gaohongyu789.top

[S47] C++：结构化绑定遍历
来源：http://xfi.hammf.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://orv.xingfuxueyuan.xyz

[S48] C++：逐行读文件
来源：http://hkk.chenjidiqi.icu

std::ifstream in("a.txt");  std::string line;
来源：http://nlu.sxryk.cn

while (std::getline(in, line)) { }
来源：http://olg.gaohongyu789.top

[S49] C++：写文件
来源：http://cma.andypj.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bgq.wangdashe.top

[S50] C++：格式化数字
来源：http://jwr.vqdsnc.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gye.0kj1m.cn

[S51] C++：显式类型转换
来源：http://mou.zycfv.cn

static_cast<double>(a) / b
来源：http://vvw.cucudq.cn

[S52] C++：const 与 noexcept
来源：http://ero.zdbjq.cn

int size() const noexcept { return n_; }
来源：http://xhn.gogol.net.cn

[S53] C++：移动语义
来源：http://mjk.0kj1m.cn

std::vector<int> w = std::move(v);
来源：http://cbf.jinqigufen.top

[S54] C++：异常处理
来源：http://wxd.zdqjudy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://uey.chenzaomai.com

[S55] C++：结构化绑定
来源：http://igz.ydzc1.top

auto [a, b] = std::make_pair(1, 2);
来源：http://rjv.smart0.xyz

[S56] C++：optional
来源：http://lgk.hnxiangtu.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qfh.gogol.net.cn

[S57] C++：编译期常量
来源：http://rdt.gotoacloud.top

constexpr int N = 10;
来源：http://dxi.yj20258888.top

[S58] C++：命名空间
来源：http://ltn.dashuyun.cn

namespace ns { int f() { return 1; } }
来源：http://xbr.ctjpmb.com

[S59] C++：静态断言
来源：http://bfm.tianlin.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://msi.zdbjq.cn

[S60] C++：遍历并删除元素
来源：http://qha.dianchejie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hdu.hnqzz.top

================================================================================
来源：http://lca.dianchejie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rms.jinghuilouyu.cn

================================================================================
来源：http://utp.haohaochexian.top

[T01] Kotlin：Hello World
来源：http://ljr.zhiwuduotai.top

println("Hello")
来源：http://ere.sxryk.cn

[T02] Kotlin：变量
来源：http://mec.jinqigfzy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pui.ctjpmb.com

[T03] Kotlin：字符串模板
来源：http://ixt.pengpengdd.cyou

"值: $b"
来源：http://hhl.shzxlz.cn

[T04] Kotlin：空安全
来源：http://zkb.fanxiaobao.xyz

val n: String? = null;  n?.length
来源：http://cog.hcnkem.com

[T05] Kotlin：when 表达式
来源：http://tsk.fanxiaobao.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nkz.zycfv.cn

[T06] Kotlin：集合映射
来源：http://vkz.jlsjyb.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://asp.ydjk.org.cn

[T07] Kotlin：集合过滤
来源：http://eze.c1oappe.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://fzb.hywenlv.cn

[T08] Kotlin：数据类
来源：http://tdd.jqgfzy.top

data class User(val name: String, val age: Int)
来源：http://quf.ivvv.top

[T09] Kotlin：扩展函数
来源：http://awx.zhixingplan.top

fun String.exclaim() = this + "!"
来源：http://qis.yj20258.top

[T10] Kotlin：默认参数
来源：http://lzx.aibaodan.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://hsg.shanyushiyangtech.top

[T11] Kotlin：协程
来源：http://mrf.cdnleiting.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://gfa.fehbvm.com

[T12] Kotlin：解构声明
来源：http://zrh.sufxvd.cn

val (a, b) = Pair(1, 2)
来源：http://cyr.ctjpmb.com

[T13] Kotlin：只读 Map
来源：http://aiy.andypj.xyz

val m = mapOf("a" to 1)
来源：http://ucq.meibo888.top

[T14] Kotlin：循环
来源：http://zjj.guowangkeji.top

for (i in 1..10) println(i)
来源：http://hwp.shanyushiyangkeji.top

[T15] Kotlin：接口
来源：http://vwj.zycfv.cn

interface Shape { fun area(): Double }
来源：http://gpi.svipenyu.cn

[T16] Swift：Hello World
来源：http://ofa.ehwqpu.com

print("Hello")
来源：http://ica.fanxiaobao.xyz

[T17] Swift：变量与常量
来源：http://ppm.daxiang520.top

var a = 1;  let b = 2
来源：http://lle.hongshengwenyu.top

[T18] Swift：字符串插值
来源：http://bwr.shanyushiyangkeji.top

"值: \(b)"
来源：http://blm.guannengcc.top

[T19] Swift：可选绑定
来源：http://nix.fehbvm.com

if let n = opt { print(n) }
来源：http://pwe.hnxiangtu.top

[T20] Swift：数组操作
来源：http://ybi.jyoumei.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ywr.birdmap.top

[T21] Swift：遍历
来源：http://jfq.cdnleiting.top

for x in a { print(x) }
来源：http://gto.aizwys.cn

[T22] Swift：字典
来源：http://bzx.birdmap.top

var d = ["a": 1];  d["b"] = 2
来源：http://wjn.bbcook.cn

[T23] Swift：函数
来源：http://jog.cucudq.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ypc.tian-w.cn

[T24] Swift：闭包
来源：http://iqa.jinyuanbaomall.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://dmq.sxryk.cn

[T25] Swift：结构体
来源：http://wql.9152youxi.cn

struct P { var x: Int }
来源：http://dds.nanxinkj.top

[T26] Swift：类与重写
来源：http://vnh.jqgfzy.top

class A: Base { override func f() {} }
来源：http://rhu.shanyushiyangkeji.top

[T27] Swift：错误处理
来源：http://kmo.316326.xyz

do { try f() } catch { print(error) }
来源：http://hvz.chenjidiqi.icu

[T28] Swift：枚举
来源：http://byg.jyoumei.cn

enum Color { case red, green }
来源：http://ezh.9152youxi.cn

[T29] Swift：guard 提前返回
来源：http://cin.meibo888.top

guard let x = opt else { return }
来源：http://bpf.jinyuanbaomall.cn

[T30] Swift：协议
来源：http://msn.xziqi.cn

protocol Shape { func area() -> Double }
来源：http://cch.jyoumei.cn

[T31] Lua：Hello World
来源：http://ufu.jianghu66.top

print("Hello")
来源：http://iwt.meibo888.top

[T32] Lua：局部变量
来源：http://irz.hnqzz.top

local a = 1
来源：http://kop.9152youxi.cn

[T33] Lua：表（数组）
来源：http://yhd.tanke756.top

local t = {1, 2, 3};  t[4] = 4
来源：http://uto.cashguo.top

[T34] Lua：遍历表
来源：http://wji.shangyingyoupin.top

for i, v in ipairs(t) do print(i, v) end
来源：http://wxv.tanke756.top

[T35] Lua：字典表
来源：http://pxe.cdnleiting.top

local d = { a = 1 };  d.b = 2
来源：http://gvq.shzxlz.cn

[T36] Lua：函数
来源：http://lck.kuanghao11.cn

function add(a, b) return a + b end
来源：http://tol.mhx1999.top

[T37] Lua：字符串拼接
来源：http://fho.wangshuangyany.cn

"a" .. "b"
来源：http://mfc.wangshuangyany.cn

[T38] Lua：条件
来源：http://qci.shangyingyoupin.top

if x > 0 then print("正") end
来源：http://cbq.hfpthk.cn

[T39] Lua：模式匹配
来源：http://skk.yueranfly.top

string.find(s, "%d+")
来源：http://ozu.zdbjq.cn

[T40] Lua：元表
来源：http://edb.shuidangran.top

setmetatable({}, { __index = base })
来源：http://kiq.sxryk.cn

[T41] Perl：Hello World
来源：http://oiz.andypj.xyz

print "Hello\n";
来源：http://tig.quarkkingdee.top

[T42] Perl：变量类型
来源：http://hqw.zhijiandao.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gzb.gogol.net.cn

[T43] Perl：字符串插值
来源：http://fxj.sjlbkw.cn

"值: $a"
来源：http://zqj.yanxiufei.cn

[T44] Perl：条件
来源：http://tfn.0kj1m.cn

if ($a > 0) { print "正"; }
来源：http://zlf.shzxlz.cn

[T45] Perl：数组遍历
来源：http://lcf.sysykeji.top

for my $x (@arr) { print $x; }
来源：http://hvj.gzhubu.top

[T46] Perl：哈希操作
来源：http://iei.feifeiyinyue.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fdo.dashuyun.cn

[T47] Perl：正则捕获
来源：http://rhp.pycfn.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://afh.aibaodan.cn

[T48] Perl：正则替换
来源：http://mae.hcnkem.com

$s =~ s/old/new/g;
来源：http://aez.gzhubu.top

[T49] Perl：函数
来源：http://acp.ivvv.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xar.feifeiyinyue.top

[T50] Perl：逐行读文件
来源：http://ewa.kuanghao11.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ocm.kuanghao11.cn

while (my $line = <$fh>) { print $line; }
来源：http://fly.shangyingyoupin.top

[T51] Scala：Hello World
来源：http://pwj.cashguo.top

println("Hello")
来源：http://bxu.yj20258888.top

[T52] Scala：变量
来源：http://chh.hongshengwenyu.top

val a = 1;  var b = 2
来源：http://jbb.quarkkingdee.top

[T53] Scala：字符串插值
来源：http://eia.zhengqikj.top

s"值: $b"
来源：http://tyd.haohaochexian.top

[T54] Scala：集合映射
来源：http://qoo.bbcook.cn

List(1, 2, 3).map(_ * 2)
来源：http://tkv.feifeiyinyue.top

[T55] Scala：集合过滤
来源：http://jxk.ydzc1.top

List(1, 2, 3).filter(_ > 1)
来源：http://nft.havefunace.top

[T56] Scala：样例类
来源：http://wur.sufxvd.cn

case class User(name: String, age: Int)
来源：http://oxs.tanke756.top

[T57] Scala：模式匹配
来源：http://dww.zhongyouzk.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://vks.sjlbkw.cn

[T58] Scala：函数定义
来源：http://shw.fktsv.cn

def add(a: Int, b: Int): Int = a + b
来源：http://rlt.yangfankeji.com

[T59] Scala：循环
来源：http://kri.vqdsnc.cn

for (i <- 1 to 10) println(i)
来源：http://zsd.zdbjq.cn

[T60] Scala：折叠
来源：http://epe.mhx1999.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mmh.pycfn.com

================================================================================
来源：http://alg.sxryk.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ifh.hfpthk.cn

================================================================================
来源：http://uob.uphjek.com

[U01] Py：创建虚拟环境
来源：http://vki.9152youxi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://mje.shanyushiyangkeji.top

[U02] Py：导出 / 安装依赖
来源：http://lcw.ehwqpu.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tyc.c1oappe.top

[U03] Py：加载 .env 配置
来源：http://bjb.yj20258888.top

from dotenv import load_dotenv; load_dotenv()
来源：http://gqr.cqqwz.cn

[U04] Py：变量调试打印
来源：http://aql.redwolf501.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://byg.guannengcc.top

[U05] Py：列表去重且保序
来源：http://zyl.cucudq.cn

list(dict.fromkeys(arr))
来源：http://llx.hcnkem.com

[U06] Py：合并两个字典
来源：http://knm.sxryk.cn

{**a, **b}
来源：http://etl.feifeiyinyue.top

[U07] Py：反转字典键值
来源：http://mhs.iojbl.cn

{v: k for k, v in d.items()}
来源：http://rbo.xziqi.cn

[U08] Py：展平二维列表
来源：http://zak.ppjwa.cn

[y for x in nested for y in x]
来源：http://ntu.zdbjq.cn

[U09] Py：字典取最大值的键
来源：http://uqu.zhengqikj.top

max(d, key=d.get)
来源：http://dgq.zhixingplan.top

[U10] Py：按值排序字典
来源：http://tqq.vqdsnc.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nuh.zhoulong.xyz

[U11] Py：生成器表达式
来源：http://kti.uphjek.com

(x * 2 for x in arr)
来源：http://sfc.jinyuanbaomall.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ata.dianchejie.cn

Counter(arr).most_common(3)
来源：http://aww.birdmap.top

[U13] Py：固定长度队列
来源：http://mze.cashguo.top

deque(maxlen=10)
来源：http://lsv.gogol.net.cn

[U14] Py：分组收集到列表
来源：http://cvx.zdqjudy.top

defaultdict(list)
来源：http://vas.xylfe.cn

[U15] Py：高精度计时
来源：http://wip.jqgfzy.top

t = time.perf_counter()
来源：http://ylj.shanyushiyangkeji.top

[U16] Py：命令行参数解析
来源：http://zvn.hammf.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://och.xuanzx.com

[U17] Py：初始化日志
来源：http://ypy.yuanzhike.top

logging.basicConfig(level=logging.INFO)
来源：http://vhk.hesvh.cn

[U18] Py：预编译正则
来源：http://jok.jlsjyb.cn

pat = re.compile(r"\d+")
来源：http://mri.svipenyu.cn

[U19] Py：正则替换带回调
来源：http://myg.yvedp.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://unb.zdqjudy.top

[U20] Py：缓存函数结果
来源：http://wuu.52xcode.cn

@functools.lru_cache(maxsize=None)
来源：http://hic.chenlongwang.top

[U21] Py：自定义上下文管理器
来源：http://vxv.cheryme.top

@contextlib.contextmanager
来源：http://utz.havefunace.top

[U22] Py：矩阵转置
来源：http://iyp.nanxuanxn.top

list(zip(*m))
来源：http://tjb.xylfe.cn

[U23] Py：分块读取大文件
来源：http://ydk.9152youxi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mkd.meibo888.top

[U24] Py：路径操作
来源：http://siz.gogol.net.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pmp.shuidangran.top

[U25] Py：CSV 按字典读
来源：http://cyj.jinyuanbaomall.cn

csv.DictReader(f)
来源：http://qvb.xuanzx.com

[U26] Py：并发下载
来源：http://dgm.guannengcc.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rsz.zhongyouzk.top

[U27] Py：异步 HTTP
来源：http://dfl.andypj.xyz

aiohttp.ClientSession() 配合 async with
来源：http://utb.haohaochexian.top

[U28] Py：类型别名
来源：http://noc.smart0.xyz

UserId = int
来源：http://hkx.daria6918.cn

[U29] Py：属性校验
来源：http://vmp.chenzaomai.com

@property 与 @x.setter 配合
来源：http://qjs.hesvh.cn

[U30] Py：数据类
来源：http://jou.snrcjt.cn

@dataclass(slots=True)
来源：http://eke.pengpengdd.cyou

[U31] Py：单测
来源：http://nms.smart0.xyz

python -m pytest -q
来源：http://hba.wangdashe.top

[U32] Py：代码格式化
来源：http://tcb.hysaishi.cn

ruff format . && ruff check --fix .
来源：http://fvp.zdqjudy.top

[U33] Py：打包发布
来源：http://gqx.wangdashe.top

python -m build  （依赖 pyproject.toml）
来源：http://ojr.cucudq.cn

[U34] Py：判断编码
来源：http://nuu.cucudq.cn

chardet.detect(raw)
来源：http://flp.jqgfzy.top

[U35] Py：发送邮件
来源：http://xlt.ydjk.org.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tnc.svipenyu.cn

[U36] Py：定时任务
来源：http://zqt.tarul.cn

schedule.every(10).minutes.do(job)
来源：http://kea.daria6918.cn

[U37] Py：读写 Excel
来源：http://apx.fengsongda.top

pandas.read_excel / DataFrame.to_excel
来源：http://jdi.epnwcf.com

[U38] Py：获取脚本所在目录
来源：http://hfx.shuidangran.top

Path(__file__).resolve().parent
来源：http://qvv.hcnkem.com

[U39] Py：判断是否在交互环境
来源：http://jnd.havefunace.top

sys.stdout.isatty()
来源：http://wpc.hywenlv.cn

[U40] Py：打印到标准错误
来源：http://wqy.gaohongyu789.top

print("err", file=sys.stderr)
来源：http://yat.chenzaomai.com

[U41] PHP：初始化 Composer 项目
来源：http://zao.yvedp.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://lne.dashuyun.cn

[U42] PHP：PSR-4 自动加载
来源：http://yof.kuanghao11.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rvc.kuanghao11.cn

[U43] PHP：声明命名空间
来源：http://qwu.c1oappe.top

namespace App\Http;
来源：http://dvf.gogol.net.cn

[U44] PHP：开启严格类型
来源：http://tbj.feifeiyinyue.top

declare(strict_types=1);
来源：http://hiv.havefunace.top

[U45] PHP：类型声明与返回类型
来源：http://hvx.mhx1999.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://elx.pengpengdd.cyou

[U46] PHP：可空类型
来源：http://nrc.bjfxy.top

?string $name = null
来源：http://lqh.hnqzz.top

[U47] PHP：联合类型
来源：http://hfs.jinqigfzy.top

int|string $id
来源：http://bvh.xingfuxueyuan.xyz

[U48] PHP：纯枚举
来源：http://fyc.zhaomingkeji.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ajo.zhoulong.xyz

[U49] PHP：只读属性
来源：http://duv.gzhubu.top

public readonly string $name
来源：http://yrt.yanxiufei.cn

[U50] PHP：构造器属性提升
来源：http://xjv.xuanzx.com

public function __construct(private int $id) {}
来源：http://ixk.jinghuilouyu.cn

[U51] PHP：数组解构
来源：http://tjf.andypj.xyz

[$a, $b] = $arr;
来源：http://oiw.zhengqikj.top

[U52] PHP：箭头函数
来源：http://dzu.cashguo.top

$double = fn($x) => $x * 2;
来源：http://amq.vqdsnc.cn

[U53] PHP：空合并运算符
来源：http://zpf.andypj.xyz

$v = $a ?? $b ?? "default";
来源：http://rqg.gotoacloud.top

[U54] PHP：空安全调用
来源：http://pka.ywan-chungtsiang.top

$obj?->method()
来源：http://oko.fktsv.cn

[U55] PHP：match 表达式
来源：http://mrg.zhaomingkeji.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://pzh.ywan-chungtsiang.top

[U56] PHP：命名参数
来源：http://pmd.shzxlz.cn

f(a: 1, b: 2)
来源：http://vlt.fanxiaobao.xyz

[U57] PHP：字符串插值
来源：http://yhd.cqqwz.cn

"值: {$a}"
来源：http://bee.yueranfly.top

[U58] PHP：数组三件套
来源：http://ooo.zhixingplan.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://koh.guannengcc.top

[U59] PHP：自定义排序
来源：http://smp.yuxming.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://eex.zhongyouzk.top

[U60] PHP：JSON 编解码
来源：http://fnu.sjlbkw.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://itj.nanxuanxn.top

[U61] PHP：正则
来源：http://uzq.52xcode.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jzl.hysaishi.cn

[U62] PHP：日期对象
来源：http://zdn.shzxlz.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://soe.hysaishi.cn


<!-- 参考信息 -->