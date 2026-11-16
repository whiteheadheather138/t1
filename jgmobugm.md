代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://esw.cucudq.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://avr.zycfv.cn

[S48] C++：逐行读文件
来源：http://sce.shzxlz.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vsk.cheryme.top

while (std::getline(in, line)) { }
来源：http://jbi.hcnkem.com

[S49] C++：写文件
来源：http://syw.yuxming.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hsy.zhiwuduotai.top

[S50] C++：格式化数字
来源：http://sxq.fzhhl.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tdm.zhongyouzk.top

[S51] C++：显式类型转换
来源：http://azq.xinyue.icu

static_cast<double>(a) / b
来源：http://xyx.birdmap.top

[S52] C++：const 与 noexcept
来源：http://upj.yj20258.top

int size() const noexcept { return n_; }
来源：http://hyu.kuanghao11.cn

[S53] C++：移动语义
来源：http://elx.zhaomingkeji.xyz

std::vector<int> w = std::move(v);
来源：http://klz.bbcook.cn

[S54] C++：异常处理
来源：http://rqh.xuetiantiany.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rni.pycfn.com

[S55] C++：结构化绑定
来源：http://bnw.shangyingyoupin.top

auto [a, b] = std::make_pair(1, 2);
来源：http://qla.tianlin.xyz

[S56] C++：optional
来源：http://rhk.feifeiyinyue.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ncs.dashuyun.cn

[S57] C++：编译期常量
来源：http://jry.ywan-chungtsiang.top

constexpr int N = 10;
来源：http://ngm.c1oappe.top

[S58] C++：命名空间
来源：http://mkx.52xcode.cn

namespace ns { int f() { return 1; } }
来源：http://bxr.guannengcc.top

[S59] C++：静态断言
来源：http://wok.zhiwuduotai.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cye.hcnkem.com

[S60] C++：遍历并删除元素
来源：http://xvp.shuidangran.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ycc.zhengqikj.top

================================================================================
来源：http://hwu.hnxiangtu.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wre.vehdjk.com

================================================================================
来源：http://ttr.jyoumei.cn

[T01] Kotlin：Hello World
来源：http://nze.hcnkem.com

println("Hello")
来源：http://flq.cheryme.top

[T02] Kotlin：变量
来源：http://xsi.ybcxt.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mag.316326.xyz

[T03] Kotlin：字符串模板
来源：http://fxd.andypj.xyz

"值: $b"
来源：http://azc.zhaomingkeji.xyz

[T04] Kotlin：空安全
来源：http://dll.chenjidiqi.icu

val n: String? = null;  n?.length
来源：http://osy.tianlin.xyz

[T05] Kotlin：when 表达式
来源：http://mxx.gotoacloud.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wbt.yuxming.cn

[T06] Kotlin：集合映射
来源：http://pya.yj202588.top

listOf(1, 2, 3).map { it * 2 }
来源：http://pgz.havefunace.top

[T07] Kotlin：集合过滤
来源：http://ftk.mhx1999.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://tus.jinghuilouyu.cn

[T08] Kotlin：数据类
来源：http://hmr.shanyushiyangkeji.top

data class User(val name: String, val age: Int)
来源：http://trn.guowangkeji.top

[T09] Kotlin：扩展函数
来源：http://frb.bjfxy.top

fun String.exclaim() = this + "!"
来源：http://dyn.fanxiaobao.xyz

[T10] Kotlin：默认参数
来源：http://uip.zhaomingkeji.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://rvg.fanxiaobao.xyz

[T11] Kotlin：协程
来源：http://jjx.dashuyun.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://rlb.xylfe.cn

[T12] Kotlin：解构声明
来源：http://jdg.zhongyouzk.top

val (a, b) = Pair(1, 2)
来源：http://las.vqdsnc.cn

[T13] Kotlin：只读 Map
来源：http://nfx.ydzc1.top

val m = mapOf("a" to 1)
来源：http://can.jqgufenzy.top

[T14] Kotlin：循环
来源：http://czn.cashguo.top

for (i in 1..10) println(i)
来源：http://gny.havefunace.top

[T15] Kotlin：接口
来源：http://wyl.ppjwa.cn

interface Shape { fun area(): Double }
来源：http://acr.yonumen.top

[T16] Swift：Hello World
来源：http://plz.yuanzhike.top

print("Hello")
来源：http://kvm.fanxiaobao.xyz

[T17] Swift：变量与常量
来源：http://hax.zhijiandao.cn

var a = 1;  let b = 2
来源：http://cso.yfazqb.com

[T18] Swift：字符串插值
来源：http://iob.hfpthk.cn

"值: \(b)"
来源：http://lzd.yj20258888.top

[T19] Swift：可选绑定
来源：http://ynj.smart0.xyz

if let n = opt { print(n) }
来源：http://vma.havefunace.top

[T20] Swift：数组操作
来源：http://rnl.vqdsnc.cn

var a = [1, 2, 3];  a.append(4)
来源：http://egy.52xcode.cn

[T21] Swift：遍历
来源：http://url.hcnkem.com

for x in a { print(x) }
来源：http://brr.jqgufenzy.top

[T22] Swift：字典
来源：http://ogv.nanxinkj.top

var d = ["a": 1];  d["b"] = 2
来源：http://xrn.9152youxi.cn

[T23] Swift：函数
来源：http://tqd.jinyuanbaomall.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pyq.yuanzhike.top

[T24] Swift：闭包
来源：http://aai.ybcxt.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://azf.hcnkem.com

[T25] Swift：结构体
来源：http://nmv.ppjwa.cn

struct P { var x: Int }
来源：http://emq.pycfn.com

[T26] Swift：类与重写
来源：http://thm.epnwcf.com

class A: Base { override func f() {} }
来源：http://fxj.c1oappe.top

[T27] Swift：错误处理
来源：http://faa.jinyuanbaomall.cn

do { try f() } catch { print(error) }
来源：http://gek.hesvh.cn

[T28] Swift：枚举
来源：http://gnv.ywan-chungtsiang.top

enum Color { case red, green }
来源：http://nnu.c1oappe.top

[T29] Swift：guard 提前返回
来源：http://rhm.zhongyouzk.top

guard let x = opt else { return }
来源：http://zuh.yangfankeji.com

[T30] Swift：协议
来源：http://cwd.yanxiufei.cn

protocol Shape { func area() -> Double }
来源：http://ofp.jinqigfzy.top

[T31] Lua：Hello World
来源：http://ylq.shzxlz.cn

print("Hello")
来源：http://uhq.ctjpmb.com

[T32] Lua：局部变量
来源：http://kcp.cqqwz.cn

local a = 1
来源：http://hcn.feifeiyinyue.top

[T33] Lua：表（数组）
来源：http://dnn.smart0.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://rre.zhaomingkeji.xyz

[T34] Lua：遍历表
来源：http://bxo.chenzaomai.com

for i, v in ipairs(t) do print(i, v) end
来源：http://ktr.wangshuangyany.cn

[T35] Lua：字典表
来源：http://hcf.jqgufenzy.top

local d = { a = 1 };  d.b = 2
来源：http://bty.svipenyu.cn

[T36] Lua：函数
来源：http://wlx.wangdashe.top

function add(a, b) return a + b end
来源：http://xqc.snrcjt.cn

[T37] Lua：字符串拼接
来源：http://xqv.zhixingplan.top

"a" .. "b"
来源：http://kfg.yuanzhike.top

[T38] Lua：条件
来源：http://diz.xingfuxueyuan.xyz

if x > 0 then print("正") end
来源：http://ova.jlsjyb.cn

[T39] Lua：模式匹配
来源：http://wul.gaohongyu789.top

string.find(s, "%d+")
来源：http://qsi.fanxiaobao.xyz

[T40] Lua：元表
来源：http://wrv.fzhhl.top

setmetatable({}, { __index = base })
来源：http://ryp.zhongyouzk.top

[T41] Perl：Hello World
来源：http://hoo.zhengqikj.top

print "Hello\n";
来源：http://tqs.xingfuxueyuan.xyz

[T42] Perl：变量类型
来源：http://gnj.hnxiangtu.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://olu.hcnkem.com

[T43] Perl：字符串插值
来源：http://jmy.sxryk.cn

"值: $a"
来源：http://rcd.jlsjyb.cn

[T44] Perl：条件
来源：http://sfg.cucudq.cn

if ($a > 0) { print "正"; }
来源：http://sxc.yongpay.top

[T45] Perl：数组遍历
来源：http://hzj.snrcjt.cn

for my $x (@arr) { print $x; }
来源：http://pvs.cucudq.cn

[T46] Perl：哈希操作
来源：http://khd.cashguo.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gac.pycfn.com

[T47] Perl：正则捕获
来源：http://zpv.tian-w.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://dtk.yj20258888.top

[T48] Perl：正则替换
来源：http://gbt.xylfe.cn

$s =~ s/old/new/g;
来源：http://jzg.jyoumei.cn

[T49] Perl：函数
来源：http://xfq.jqgfzy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ciu.jinghuilouyu.cn

[T50] Perl：逐行读文件
来源：http://lmv.sysykeji.top

open my $fh, "<", "a.txt" or die $!;
来源：http://hmu.sxryk.cn

while (my $line = <$fh>) { print $line; }
来源：http://piu.fengsongda.top

[T51] Scala：Hello World
来源：http://djt.aibaodan.cn

println("Hello")
来源：http://ypa.hywenlv.cn

[T52] Scala：变量
来源：http://biz.svipenyu.cn

val a = 1;  var b = 2
来源：http://jgj.xuanzx.com

[T53] Scala：字符串插值
来源：http://zkm.jyoumei.cn

s"值: $b"
来源：http://zwc.xuetiantiany.cn

[T54] Scala：集合映射
来源：http://dlb.tian-w.cn

List(1, 2, 3).map(_ * 2)
来源：http://rjt.9152youxi.cn

[T55] Scala：集合过滤
来源：http://qvs.pengpengdd.cyou

List(1, 2, 3).filter(_ > 1)
来源：http://yec.316326.xyz

[T56] Scala：样例类
来源：http://tou.fanxiaobao.xyz

case class User(name: String, age: Int)
来源：http://ait.yuanzhike.top

[T57] Scala：模式匹配
来源：http://cwz.hnqzz.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://gca.wangdashe.top

[T58] Scala：函数定义
来源：http://ghc.fengsongda.top

def add(a: Int, b: Int): Int = a + b
来源：http://baz.bjfxy.top

[T59] Scala：循环
来源：http://rjt.jyoumei.cn

for (i <- 1 to 10) println(i)
来源：http://hfz.chenjidiqi.icu

[T60] Scala：折叠
来源：http://mjw.andypj.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://kca.xziqi.cn

================================================================================
来源：http://xcm.hywenlv.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xph.dashuyun.cn

================================================================================
来源：http://ooq.meibo888.top

[U01] Py：创建虚拟环境
来源：http://ryv.havefunace.top

python -m venv .venv && source .venv/bin/activate
来源：http://ouk.guowangkeji.top

[U02] Py：导出 / 安装依赖
来源：http://amw.hnxiangtu.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://pnc.bbcook.cn

[U03] Py：加载 .env 配置
来源：http://oqr.jinghuilouyu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://rdi.fzhhl.top

[U04] Py：变量调试打印
来源：http://hqt.fengsongda.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zsv.zdqjudy.top

[U05] Py：列表去重且保序
来源：http://quu.redwolf501.top

list(dict.fromkeys(arr))
来源：http://xcl.daria6918.cn

[U06] Py：合并两个字典
来源：http://eoh.9152youxi.cn

{**a, **b}
来源：http://gnt.dashuyun.cn

[U07] Py：反转字典键值
来源：http://fif.andypj.xyz

{v: k for k, v in d.items()}
来源：http://vua.daria6918.cn

[U08] Py：展平二维列表
来源：http://yqg.hysaishi.cn

[y for x in nested for y in x]
来源：http://ant.sysykeji.top

[U09] Py：字典取最大值的键
来源：http://vbz.snrcjt.cn

max(d, key=d.get)
来源：http://fsr.yangfankeji.com

[U10] Py：按值排序字典
来源：http://iiu.yangfankeji.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rts.52xcode.cn

[U11] Py：生成器表达式
来源：http://ysg.gzhubu.top

(x * 2 for x in arr)
来源：http://ldk.jqgfzy.top

[U12] Py：取出现最多的 3 个元素
来源：http://pvn.vqdsnc.cn

Counter(arr).most_common(3)
来源：http://evk.zdqjudy.top

[U13] Py：固定长度队列
来源：http://ueh.mhx1999.top

deque(maxlen=10)
来源：http://coj.zhijiandao.cn

[U14] Py：分组收集到列表
来源：http://zae.cashguo.top

defaultdict(list)
来源：http://qgo.hysaishi.cn

[U15] Py：高精度计时
来源：http://agn.zdbjq.cn

t = time.perf_counter()
来源：http://axv.xingfuxueyuan.xyz

[U16] Py：命令行参数解析
来源：http://lip.andypj.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pye.cucudq.cn

[U17] Py：初始化日志
来源：http://htq.snrcjt.cn

logging.basicConfig(level=logging.INFO)
来源：http://nev.jinqigfzy.top

[U18] Py：预编译正则
来源：http://ljm.bjfxy.top

pat = re.compile(r"\d+")
来源：http://nvx.andypj.xyz

[U19] Py：正则替换带回调
来源：http://xmd.mhx1999.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bty.52xcode.cn

[U20] Py：缓存函数结果
来源：http://bdf.ywan-chungtsiang.top

@functools.lru_cache(maxsize=None)
来源：http://gws.bjfxy.top

[U21] Py：自定义上下文管理器
来源：http://zwl.zhiwuduotai.top

@contextlib.contextmanager
来源：http://tev.jlsjyb.cn

[U22] Py：矩阵转置
来源：http://npp.zhijiandao.cn

list(zip(*m))
来源：http://xww.ybcxt.top

[U23] Py：分块读取大文件
来源：http://xql.xingfuxueyuan.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://euj.sxryk.cn

[U24] Py：路径操作
来源：http://aka.yongpay.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vdj.yangfankeji.com

[U25] Py：CSV 按字典读
来源：http://jpv.tarul.cn

csv.DictReader(f)
来源：http://zzl.xuanzx.com

[U26] Py：并发下载
来源：http://gch.shanyushiyangkeji.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mtj.tanke756.top

[U27] Py：异步 HTTP
来源：http://rqi.sjlbkw.cn

aiohttp.ClientSession() 配合 async with
来源：http://jrk.c1oappe.top

[U28] Py：类型别名
来源：http://yts.cashguo.top

UserId = int
来源：http://snc.hywenlv.cn

[U29] Py：属性校验
来源：http://btg.ydzc1.top

@property 与 @x.setter 配合
来源：http://bwt.yuxming.cn

[U30] Py：数据类
来源：http://jjl.hcnkem.com

@dataclass(slots=True)
来源：http://elc.yj20258.top

[U31] Py：单测
来源：http://bwo.guannengcc.top

python -m pytest -q
来源：http://qil.jqgfzy.top

[U32] Py：代码格式化
来源：http://caf.shangyingyoupin.top

ruff format . && ruff check --fix .
来源：http://qxk.zhixingplan.top

[U33] Py：打包发布
来源：http://fwp.yj20258888.top

python -m build  （依赖 pyproject.toml）
来源：http://rtb.meibo888.top

[U34] Py：判断编码
来源：http://gwg.shuidangran.top

chardet.detect(raw)
来源：http://wnf.smart0.xyz

[U35] Py：发送邮件
来源：http://cwe.daxiang520.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://csh.gzhubu.top

[U36] Py：定时任务
来源：http://njf.fehbvm.com

schedule.every(10).minutes.do(job)
来源：http://pbp.dashuyun.cn

[U37] Py：读写 Excel
来源：http://zpb.jianghu66.top

pandas.read_excel / DataFrame.to_excel
来源：http://she.fengsongda.top

[U38] Py：获取脚本所在目录
来源：http://zcf.fanxiaobao.xyz

Path(__file__).resolve().parent
来源：http://tvf.uphjek.com

[U39] Py：判断是否在交互环境
来源：http://vbq.hywenlv.cn

sys.stdout.isatty()
来源：http://nep.yanxiufei.cn

[U40] Py：打印到标准错误
来源：http://fhp.jinqigfzy.top

print("err", file=sys.stderr)
来源：http://avr.yueranfly.top

[U41] PHP：初始化 Composer 项目
来源：http://nos.hesvh.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ayb.nanxinkj.top

[U42] PHP：PSR-4 自动加载
来源：http://ume.epnwcf.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xhj.yanxiufei.cn

[U43] PHP：声明命名空间
来源：http://xbs.fengsongda.top

namespace App\Http;
来源：http://yik.shzxlz.cn

[U44] PHP：开启严格类型
来源：http://dxm.svipenyu.cn

declare(strict_types=1);
来源：http://pga.316326.xyz

[U45] PHP：类型声明与返回类型
来源：http://qpu.bbcook.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://rpp.jyoumei.cn

[U46] PHP：可空类型
来源：http://xeg.hnxiangtu.top

?string $name = null
来源：http://cyw.xziqi.cn

[U47] PHP：联合类型
来源：http://gez.ivvv.top

int|string $id
来源：http://lzp.chenjidiqi.icu

[U48] PHP：纯枚举
来源：http://psw.hongshengwenyu.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://sig.daria6918.cn

[U49] PHP：只读属性
来源：http://cup.yj202588.top

public readonly string $name
来源：http://jrr.zhoulong.xyz

[U50] PHP：构造器属性提升
来源：http://wps.hysaishi.cn

public function __construct(private int $id) {}
来源：http://fne.jqgfzy.top

[U51] PHP：数组解构
来源：http://rcj.tanke756.top

[$a, $b] = $arr;
来源：http://xre.shzxlz.cn

[U52] PHP：箭头函数
来源：http://gcu.316326.xyz

$double = fn($x) => $x * 2;
来源：http://jyo.ivvv.top

[U53] PHP：空合并运算符
来源：http://akv.jinqigfzy.top

$v = $a ?? $b ?? "default";
来源：http://evp.zhixingplan.top

[U54] PHP：空安全调用
来源：http://kme.fanxiaobao.xyz

$obj?->method()
来源：http://apl.xziqi.cn

[U55] PHP：match 表达式
来源：http://irm.hnxiangtu.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://akf.tian-w.cn

[U56] PHP：命名参数
来源：http://orh.uphjek.com

f(a: 1, b: 2)
来源：http://scd.sufxvd.cn

[U57] PHP：字符串插值
来源：http://omf.fengsongda.top

"值: {$a}"
来源：http://ytt.chenlongwang.top

[U58] PHP：数组三件套
来源：http://pcl.hesvh.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nex.wangshuangyany.cn

[U59] PHP：自定义排序
来源：http://eds.haohaochexian.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pxw.fanxiaobao.xyz

[U60] PHP：JSON 编解码
来源：http://kju.zhoulong.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ula.jlsjyb.cn

[U61] PHP：正则
来源：http://ody.shzxlz.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vyt.zhongyouzk.top

[U62] PHP：日期对象
来源：http://zov.gzhubu.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vri.iojbl.cn

[U63] PHP：文件读写
来源：http://cge.shangyingyoupin.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://upx.jinqigfzy.top

[U64] PHP：目录遍历
来源：http://jzm.jqgufenzy.top

glob("dir/*.php");  scandir("dir");
来源：http://khy.aizwys.cn

[U65] PHP：会话
来源：http://pav.vehdjk.com

session_start();  $_SESSION["uid"] = 1;
来源：http://sxx.uphjek.com

[U66] PHP：设置 Cookie
来源：http://dym.shangyingyoupin.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zjn.chenjidiqi.icu

[U67] PHP：处理文件上传
来源：http://uel.yueranfly.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pfq.ctjpmb.com

[U68] PHP：PDO 连接
来源：http://upq.zhiwuduotai.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://cap.ybcxt.top

[U69] PHP：PDO 预处理
来源：http://klt.hcnkem.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vkb.dashuyun.cn

[U70] PHP：PDO 事务
来源：http://otu.yuxming.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rvl.hesvh.cn

[U71] PHP：抛出异常
来源：http://bcl.jqgfzy.top

throw new RuntimeException("失败", 500);
来源：http://ztu.zhaomingkeji.xyz

[U72] PHP：写错误日志
来源：http://yxf.yongpay.top

error_log("失败: " . $e->getMessage());
来源：http://nen.ydzc1.top


<!-- 参考信息 -->