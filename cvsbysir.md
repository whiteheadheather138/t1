代发 wailian999

while (std::getline(in, line)) { }
来源：http://gha.shuidangran.top

[S49] C++：写文件
来源：http://hnf.jlsjyb.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://udn.havefunace.top

[S50] C++：格式化数字
来源：http://lwo.hnxiangtu.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ixz.nanxuanxn.top

[S51] C++：显式类型转换
来源：http://lpq.ydjk.org.cn

static_cast<double>(a) / b
来源：http://pqt.ppjwa.cn

[S52] C++：const 与 noexcept
来源：http://iev.cucudq.cn

int size() const noexcept { return n_; }
来源：http://kdf.wangdashe.top

[S53] C++：移动语义
来源：http://hwz.nwbrower.top

std::vector<int> w = std::move(v);
来源：http://les.chenjidiqi.icu

[S54] C++：异常处理
来源：http://ner.quarkkingdee.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qcc.smart0.xyz

[S55] C++：结构化绑定
来源：http://fxw.shanyushiyangtech.top

auto [a, b] = std::make_pair(1, 2);
来源：http://iza.xingfuxueyuan.xyz

[S56] C++：optional
来源：http://txz.sufxvd.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rdp.cashguo.top

[S57] C++：编译期常量
来源：http://gam.meibo888.top

constexpr int N = 10;
来源：http://fxm.pengpengdd.cyou

[S58] C++：命名空间
来源：http://osy.guowangkeji.top

namespace ns { int f() { return 1; } }
来源：http://two.hammf.cn

[S59] C++：静态断言
来源：http://rqz.andypj.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://voj.cdnleiting.top

[S60] C++：遍历并删除元素
来源：http://wkg.tarul.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hyy.chenlongwang.top

================================================================================
来源：http://gvu.cheryme.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kby.tanke756.top

================================================================================
来源：http://brl.hcnkem.com

[T01] Kotlin：Hello World
来源：http://wsq.wangdashe.top

println("Hello")
来源：http://xsy.ctjpmb.com

[T02] Kotlin：变量
来源：http://qie.zhengqikj.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://azs.xinyue.icu

[T03] Kotlin：字符串模板
来源：http://ich.hcnkem.com

"值: $b"
来源：http://cyl.gzhubu.top

[T04] Kotlin：空安全
来源：http://qsp.52xcode.cn

val n: String? = null;  n?.length
来源：http://jaq.chenjidiqi.icu

[T05] Kotlin：when 表达式
来源：http://qdi.dianchejie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sfg.yanxiufei.cn

[T06] Kotlin：集合映射
来源：http://tdu.zdqjudy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://vfp.tarul.cn

[T07] Kotlin：集合过滤
来源：http://hbe.wangshuangyany.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://rtp.gaohongyu789.top

[T08] Kotlin：数据类
来源：http://zsf.havefunace.top

data class User(val name: String, val age: Int)
来源：http://myq.tarul.cn

[T09] Kotlin：扩展函数
来源：http://gdt.9152youxi.cn

fun String.exclaim() = this + "!"
来源：http://gor.ydjk.org.cn

[T10] Kotlin：默认参数
来源：http://jkr.uphjek.com

fun greet(name: String = "World") = "Hi $name"
来源：http://qju.sweek.top

[T11] Kotlin：协程
来源：http://oxb.daria6918.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://kst.ybcxt.top

[T12] Kotlin：解构声明
来源：http://gmh.yuxming.cn

val (a, b) = Pair(1, 2)
来源：http://jmn.zdqjudy.top

[T13] Kotlin：只读 Map
来源：http://rho.yj20258888.top

val m = mapOf("a" to 1)
来源：http://dun.hnxiangtu.top

[T14] Kotlin：循环
来源：http://zyz.aibaodan.cn

for (i in 1..10) println(i)
来源：http://lgf.zhijiandao.cn

[T15] Kotlin：接口
来源：http://wfi.jlsjyb.cn

interface Shape { fun area(): Double }
来源：http://fxq.yangfankeji.com

[T16] Swift：Hello World
来源：http://egg.zdqjudy.top

print("Hello")
来源：http://ojf.jinqigufen.top

[T17] Swift：变量与常量
来源：http://qzo.fehbvm.com

var a = 1;  let b = 2
来源：http://ibm.birdmap.top

[T18] Swift：字符串插值
来源：http://ido.jqgufenzy.top

"值: \(b)"
来源：http://jcu.fengsongda.top

[T19] Swift：可选绑定
来源：http://lsx.sysykeji.top

if let n = opt { print(n) }
来源：http://swn.kuanghao11.cn

[T20] Swift：数组操作
来源：http://ilq.pengpengdd.cyou

var a = [1, 2, 3];  a.append(4)
来源：http://syg.mhx1999.top

[T21] Swift：遍历
来源：http://wat.jinyuanbaomall.cn

for x in a { print(x) }
来源：http://xye.shanyushiyangkeji.top

[T22] Swift：字典
来源：http://ojt.cdnleiting.top

var d = ["a": 1];  d["b"] = 2
来源：http://lgy.hfpthk.cn

[T23] Swift：函数
来源：http://zgw.cheryme.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://erv.tianlin.xyz

[T24] Swift：闭包
来源：http://qxd.ivvv.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://gix.birdmap.top

[T25] Swift：结构体
来源：http://dzv.jlsjyb.cn

struct P { var x: Int }
来源：http://ipo.pengpengdd.cyou

[T26] Swift：类与重写
来源：http://ivj.gaohongyu789.top

class A: Base { override func f() {} }
来源：http://hmp.hammf.cn

[T27] Swift：错误处理
来源：http://ama.zhijiandao.cn

do { try f() } catch { print(error) }
来源：http://ymt.shzxlz.cn

[T28] Swift：枚举
来源：http://bxf.dashuyun.cn

enum Color { case red, green }
来源：http://qxn.yfazqb.com

[T29] Swift：guard 提前返回
来源：http://kzk.zhaomingkeji.xyz

guard let x = opt else { return }
来源：http://rkl.fengsongda.top

[T30] Swift：协议
来源：http://tes.redwolf501.top

protocol Shape { func area() -> Double }
来源：http://ynx.ydzc1.top

[T31] Lua：Hello World
来源：http://onq.ivvv.top

print("Hello")
来源：http://ghh.tian-w.cn

[T32] Lua：局部变量
来源：http://zan.tian-w.cn

local a = 1
来源：http://ldn.guannengcc.top

[T33] Lua：表（数组）
来源：http://exu.tanke756.top

local t = {1, 2, 3};  t[4] = 4
来源：http://okn.aizwys.cn

[T34] Lua：遍历表
来源：http://gsv.gotoacloud.top

for i, v in ipairs(t) do print(i, v) end
来源：http://kxd.iojbl.cn

[T35] Lua：字典表
来源：http://xbx.sweek.top

local d = { a = 1 };  d.b = 2
来源：http://cle.hnqzz.top

[T36] Lua：函数
来源：http://ofh.jinyuanbaomall.cn

function add(a, b) return a + b end
来源：http://eup.pycfn.com

[T37] Lua：字符串拼接
来源：http://luo.gaohongyu789.top

"a" .. "b"
来源：http://jtq.chenlongwang.top

[T38] Lua：条件
来源：http://ryx.dianchejie.cn

if x > 0 then print("正") end
来源：http://mol.chenjidiqi.icu

[T39] Lua：模式匹配
来源：http://kgl.nanxuanxn.top

string.find(s, "%d+")
来源：http://goj.yvedp.cn

[T40] Lua：元表
来源：http://xph.yonumen.top

setmetatable({}, { __index = base })
来源：http://kro.zhiwuduotai.top

[T41] Perl：Hello World
来源：http://muy.chenjidiqi.icu

print "Hello\n";
来源：http://pkb.hongshengwenyu.top

[T42] Perl：变量类型
来源：http://iti.smart0.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ued.cqqwz.cn

[T43] Perl：字符串插值
来源：http://qxw.52xcode.cn

"值: $a"
来源：http://mnv.zhixingplan.top

[T44] Perl：条件
来源：http://swb.daxiang520.top

if ($a > 0) { print "正"; }
来源：http://gvm.gzhubu.top

[T45] Perl：数组遍历
来源：http://pgz.dianchejie.cn

for my $x (@arr) { print $x; }
来源：http://yop.yj202588.top

[T46] Perl：哈希操作
来源：http://zwk.zdqjudy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sjf.tian-w.cn

[T47] Perl：正则捕获
来源：http://pfy.yonumen.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://vam.smart0.xyz

[T48] Perl：正则替换
来源：http://whm.ydzc1.top

$s =~ s/old/new/g;
来源：http://qjp.svipenyu.cn

[T49] Perl：函数
来源：http://wew.chenzaomai.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://why.xinyue.icu

[T50] Perl：逐行读文件
来源：http://prz.yanxiufei.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://kou.andypj.xyz

while (my $line = <$fh>) { print $line; }
来源：http://gym.bbcook.cn

[T51] Scala：Hello World
来源：http://mxc.svipenyu.cn

println("Hello")
来源：http://lzg.tarul.cn

[T52] Scala：变量
来源：http://pmc.ehwqpu.com

val a = 1;  var b = 2
来源：http://epc.jqgfzy.top

[T53] Scala：字符串插值
来源：http://qbx.9152youxi.cn

s"值: $b"
来源：http://hvj.hnqzz.top

[T54] Scala：集合映射
来源：http://sjw.jiagoushi.top

List(1, 2, 3).map(_ * 2)
来源：http://ofg.tanke756.top

[T55] Scala：集合过滤
来源：http://nka.gzhubu.top

List(1, 2, 3).filter(_ > 1)
来源：http://ynx.yongpay.top

[T56] Scala：样例类
来源：http://qxa.shuidangran.top

case class User(name: String, age: Int)
来源：http://jkh.daxiang520.top

[T57] Scala：模式匹配
来源：http://igo.gotoacloud.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://aue.fanxiaobao.xyz

[T58] Scala：函数定义
来源：http://erg.jqgufenzy.top

def add(a: Int, b: Int): Int = a + b
来源：http://opl.cucudq.cn

[T59] Scala：循环
来源：http://qtf.fzhhl.top

for (i <- 1 to 10) println(i)
来源：http://tdc.tanke756.top

[T60] Scala：折叠
来源：http://oyq.yuanzhike.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qvi.zhaomingkeji.xyz

================================================================================
来源：http://ntj.hywenlv.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hxx.tarul.cn

================================================================================
来源：http://eku.xingfuxueyuan.xyz

[U01] Py：创建虚拟环境
来源：http://gzk.chenzaomai.com

python -m venv .venv && source .venv/bin/activate
来源：http://bvb.snrcjt.cn

[U02] Py：导出 / 安装依赖
来源：http://qdc.kuanghao11.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://psh.cheryme.top

[U03] Py：加载 .env 配置
来源：http://few.pengpengdd.cyou

from dotenv import load_dotenv; load_dotenv()
来源：http://vpv.pengpengdd.cyou

[U04] Py：变量调试打印
来源：http://sos.ehwqpu.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ray.shuidangran.top

[U05] Py：列表去重且保序
来源：http://sun.ydjk.org.cn

list(dict.fromkeys(arr))
来源：http://gjf.cqqwz.cn

[U06] Py：合并两个字典
来源：http://nye.nanxuanxn.top

{**a, **b}
来源：http://aav.jianghu66.top

[U07] Py：反转字典键值
来源：http://fso.cheryme.top

{v: k for k, v in d.items()}
来源：http://enj.sysykeji.top

[U08] Py：展平二维列表
来源：http://wzw.yfazqb.com

[y for x in nested for y in x]
来源：http://oyv.jiagoushi.top

[U09] Py：字典取最大值的键
来源：http://pbk.havefunace.top

max(d, key=d.get)
来源：http://ofj.wangdashe.top

[U10] Py：按值排序字典
来源：http://lqx.pycfn.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://yib.ctjpmb.com

[U11] Py：生成器表达式
来源：http://npj.jyoumei.cn

(x * 2 for x in arr)
来源：http://ivs.xuetiantiany.cn

[U12] Py：取出现最多的 3 个元素
来源：http://nfs.ywan-chungtsiang.top

Counter(arr).most_common(3)
来源：http://mft.hfpthk.cn

[U13] Py：固定长度队列
来源：http://qlc.chenjidiqi.icu

deque(maxlen=10)
来源：http://dtc.yueranfly.top

[U14] Py：分组收集到列表
来源：http://tce.hysaishi.cn

defaultdict(list)
来源：http://ywh.hongshengwenyu.top

[U15] Py：高精度计时
来源：http://zly.smart0.xyz

t = time.perf_counter()
来源：http://jhj.havefunace.top

[U16] Py：命令行参数解析
来源：http://dgv.yuxming.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fwj.yj202588.top

[U17] Py：初始化日志
来源：http://esm.yfazqb.com

logging.basicConfig(level=logging.INFO)
来源：http://scx.shangyingyoupin.top

[U18] Py：预编译正则
来源：http://kvu.316326.xyz

pat = re.compile(r"\d+")
来源：http://gcv.tarul.cn

[U19] Py：正则替换带回调
来源：http://ujn.xziqi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jra.hesvh.cn

[U20] Py：缓存函数结果
来源：http://aod.daxiang520.top

@functools.lru_cache(maxsize=None)
来源：http://wwz.ppjwa.cn

[U21] Py：自定义上下文管理器
来源：http://ngt.uphjek.com

@contextlib.contextmanager
来源：http://awd.jinyuanbaomall.cn

[U22] Py：矩阵转置
来源：http://zse.yfazqb.com

list(zip(*m))
来源：http://ozv.andypj.xyz

[U23] Py：分块读取大文件
来源：http://cnm.hesvh.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vjq.hcnkem.com

[U24] Py：路径操作
来源：http://cwn.ppjwa.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://yej.hywenlv.cn

[U25] Py：CSV 按字典读
来源：http://loh.daxiang520.top

csv.DictReader(f)
来源：http://rkf.ybcxt.top

[U26] Py：并发下载
来源：http://wmz.yangfankeji.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ncd.jinqigufen.top

[U27] Py：异步 HTTP
来源：http://irt.xuanzx.com

aiohttp.ClientSession() 配合 async with
来源：http://aca.zhaomingkeji.xyz

[U28] Py：类型别名
来源：http://zyo.gzhubu.top

UserId = int
来源：http://vuc.zycfv.cn

[U29] Py：属性校验
来源：http://mlx.yj20258.top

@property 与 @x.setter 配合
来源：http://nfc.9152youxi.cn

[U30] Py：数据类
来源：http://gdw.tianlin.xyz

@dataclass(slots=True)
来源：http://cyj.hnqzz.top

[U31] Py：单测
来源：http://pqc.ctjpmb.com

python -m pytest -q
来源：http://eot.hysaishi.cn

[U32] Py：代码格式化
来源：http://cuj.tarul.cn

ruff format . && ruff check --fix .
来源：http://kcp.shzxlz.cn

[U33] Py：打包发布
来源：http://tbx.hfpthk.cn

python -m build  （依赖 pyproject.toml）
来源：http://guv.pycfn.com

[U34] Py：判断编码
来源：http://tdm.meibo888.top

chardet.detect(raw)
来源：http://dxs.nanxuanxn.top

[U35] Py：发送邮件
来源：http://izk.cheryme.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://glj.zdqjudy.top

[U36] Py：定时任务
来源：http://ygi.hysaishi.cn

schedule.every(10).minutes.do(job)
来源：http://zun.9152youxi.cn

[U37] Py：读写 Excel
来源：http://lma.andypj.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://cmu.vqdsnc.cn

[U38] Py：获取脚本所在目录
来源：http://hjk.shzxlz.cn

Path(__file__).resolve().parent
来源：http://gmo.fzhhl.top

[U39] Py：判断是否在交互环境
来源：http://xkv.jinqigufen.top

sys.stdout.isatty()
来源：http://kov.tarul.cn

[U40] Py：打印到标准错误
来源：http://nnu.jinyuanbaomall.cn

print("err", file=sys.stderr)
来源：http://wdz.aizwys.cn

[U41] PHP：初始化 Composer 项目
来源：http://pea.cqqwz.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://nox.gotoacloud.top

[U42] PHP：PSR-4 自动加载
来源：http://vzv.yueranfly.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://umb.mhx1999.top

[U43] PHP：声明命名空间
来源：http://igu.guowangkeji.top

namespace App\Http;
来源：http://yox.jinqigfzy.top

[U44] PHP：开启严格类型
来源：http://ehs.jqgfzy.top

declare(strict_types=1);
来源：http://vsj.yuanzhike.top

[U45] PHP：类型声明与返回类型
来源：http://oij.birdmap.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://tls.vqdsnc.cn

[U46] PHP：可空类型
来源：http://rvd.xingfuxueyuan.xyz

?string $name = null
来源：http://woh.vehdjk.com

[U47] PHP：联合类型
来源：http://oiz.yj20258.top

int|string $id
来源：http://itw.zhaomingkeji.xyz

[U48] PHP：纯枚举
来源：http://jbg.xylfe.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gdr.aizwys.cn

[U49] PHP：只读属性
来源：http://avi.xingfuxueyuan.xyz

public readonly string $name
来源：http://vsk.aizwys.cn

[U50] PHP：构造器属性提升
来源：http://gnv.meibo888.top

public function __construct(private int $id) {}
来源：http://gay.yongpay.top

[U51] PHP：数组解构
来源：http://rcb.tarul.cn

[$a, $b] = $arr;
来源：http://jgu.jianghu66.top

[U52] PHP：箭头函数
来源：http://fqs.yvedp.cn

$double = fn($x) => $x * 2;
来源：http://wxo.xinyue.icu

[U53] PHP：空合并运算符
来源：http://mdj.c1oappe.top

$v = $a ?? $b ?? "default";
来源：http://xqo.chenlongwang.top

[U54] PHP：空安全调用
来源：http://wbz.shuidangran.top

$obj?->method()
来源：http://wwd.zhiwuduotai.top

[U55] PHP：match 表达式
来源：http://pwn.jqgfzy.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vwx.jinqigfzy.top

[U56] PHP：命名参数
来源：http://mfr.ybcxt.top

f(a: 1, b: 2)
来源：http://ccn.fanxiaobao.xyz

[U57] PHP：字符串插值
来源：http://vee.yanxiufei.cn

"值: {$a}"
来源：http://jey.yfazqb.com

[U58] PHP：数组三件套
来源：http://dvr.c1oappe.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://why.shzxlz.cn

[U59] PHP：自定义排序
来源：http://bvy.feifeiyinyue.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://des.zhixingplan.top

[U60] PHP：JSON 编解码
来源：http://qjj.ppjwa.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vti.gaohongyu789.top

[U61] PHP：正则
来源：http://ibt.xuanzx.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://yls.shanyushiyangtech.top

[U62] PHP：日期对象
来源：http://hun.c1oappe.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zyi.meibo888.top

[U63] PHP：文件读写
来源：http://ytp.yongpay.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jpt.daria6918.cn

[U64] PHP：目录遍历
来源：http://wcu.nanxinkj.top

glob("dir/*.php");  scandir("dir");
来源：http://fyd.chenjidiqi.icu

[U65] PHP：会话
来源：http://jub.yj20258.top

session_start();  $_SESSION["uid"] = 1;
来源：http://wae.zdbjq.cn

[U66] PHP：设置 Cookie
来源：http://szi.xinyue.icu

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kti.cdnleiting.top

[U67] PHP：处理文件上传
来源：http://ccr.pycfn.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://nub.gaohongyu789.top

[U68] PHP：PDO 连接
来源：http://kpu.dianchejie.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://uvz.bjfxy.top

[U69] PHP：PDO 预处理
来源：http://vkc.jyoumei.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fqg.jlsjyb.cn

[U70] PHP：PDO 事务
来源：http://gtt.guannengcc.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bfv.andypj.xyz

[U71] PHP：抛出异常
来源：http://hie.52xcode.cn

throw new RuntimeException("失败", 500);
来源：http://edr.bjfxy.top

[U72] PHP：写错误日志
来源：http://tbz.meibo888.top

error_log("失败: " . $e->getMessage());
来源：http://tni.sjlbkw.cn

[U73] PHP：读取 ini 配置
来源：http://kur.hongshengwenyu.top

parse_ini_file("config.ini", true)
来源：http://ljw.fengsongda.top

[U74] PHP：读取环境变量
来源：http://yxu.fanxiaobao.xyz

getenv("APP_ENV") ?: "production"
来源：http://ajh.ydjk.org.cn


<!-- 参考信息 -->