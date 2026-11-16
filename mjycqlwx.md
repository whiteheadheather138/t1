代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://sqo.fengsongda.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wog.cucudq.cn

[S48] C++：逐行读文件
来源：http://qtq.hfpthk.cn

std::ifstream in("a.txt");  std::string line;
来源：http://cqa.bjfxy.top

while (std::getline(in, line)) { }
来源：http://aib.yonumen.top

[S49] C++：写文件
来源：http://seo.bbcook.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ghr.sysykeji.top

[S50] C++：格式化数字
来源：http://jmf.ywan-chungtsiang.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://axo.guannengcc.top

[S51] C++：显式类型转换
来源：http://pla.hnqzz.top

static_cast<double>(a) / b
来源：http://mty.aizwys.cn

[S52] C++：const 与 noexcept
来源：http://ltq.fktsv.cn

int size() const noexcept { return n_; }
来源：http://ggs.xziqi.cn

[S53] C++：移动语义
来源：http://ckg.sufxvd.cn

std::vector<int> w = std::move(v);
来源：http://nyo.svipenyu.cn

[S54] C++：异常处理
来源：http://jki.redwolf501.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wfl.ywan-chungtsiang.top

[S55] C++：结构化绑定
来源：http://gth.pengpengdd.cyou

auto [a, b] = std::make_pair(1, 2);
来源：http://dpl.iojbl.cn

[S56] C++：optional
来源：http://fvr.aibaodan.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gcx.chenlongwang.top

[S57] C++：编译期常量
来源：http://gtl.hnxiangtu.top

constexpr int N = 10;
来源：http://iah.jinghuilouyu.cn

[S58] C++：命名空间
来源：http://wvz.yvedp.cn

namespace ns { int f() { return 1; } }
来源：http://chl.xylfe.cn

[S59] C++：静态断言
来源：http://ecf.nanxuanxn.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vnc.wangdashe.top

[S60] C++：遍历并删除元素
来源：http://dmh.daria6918.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qky.uphjek.com

================================================================================
来源：http://iit.bjfxy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://aug.ydzc1.top

================================================================================
来源：http://htd.ydjk.org.cn

[T01] Kotlin：Hello World
来源：http://yja.dashuyun.cn

println("Hello")
来源：http://ava.dashuyun.cn

[T02] Kotlin：变量
来源：http://wrv.yangfankeji.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://uyk.kuanghao11.cn

[T03] Kotlin：字符串模板
来源：http://sog.zhoulong.xyz

"值: $b"
来源：http://yma.guowangkeji.top

[T04] Kotlin：空安全
来源：http://ree.ydjk.org.cn

val n: String? = null;  n?.length
来源：http://paa.jinyuanbaomall.cn

[T05] Kotlin：when 表达式
来源：http://fya.tanke756.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jxw.bbcook.cn

[T06] Kotlin：集合映射
来源：http://iel.hesvh.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fuh.cheryme.top

[T07] Kotlin：集合过滤
来源：http://jzq.xingfuxueyuan.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://hho.meibo888.top

[T08] Kotlin：数据类
来源：http://chi.ydzc1.top

data class User(val name: String, val age: Int)
来源：http://zod.birdmap.top

[T09] Kotlin：扩展函数
来源：http://fdq.zhongyouzk.top

fun String.exclaim() = this + "!"
来源：http://yvg.zhiwuduotai.top

[T10] Kotlin：默认参数
来源：http://mqf.jinqigufen.top

fun greet(name: String = "World") = "Hi $name"
来源：http://aug.andypj.xyz

[T11] Kotlin：协程
来源：http://qkw.pycfn.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://mfo.bbcook.cn

[T12] Kotlin：解构声明
来源：http://pcb.hnqzz.top

val (a, b) = Pair(1, 2)
来源：http://cmf.jqgfzy.top

[T13] Kotlin：只读 Map
来源：http://hvh.zdbjq.cn

val m = mapOf("a" to 1)
来源：http://uek.daxiang520.top

[T14] Kotlin：循环
来源：http://dfb.nwbrower.top

for (i in 1..10) println(i)
来源：http://nbr.bjfxy.top

[T15] Kotlin：接口
来源：http://hde.52xcode.cn

interface Shape { fun area(): Double }
来源：http://fta.cdnleiting.top

[T16] Swift：Hello World
来源：http://xxd.yanxiufei.cn

print("Hello")
来源：http://smy.yvedp.cn

[T17] Swift：变量与常量
来源：http://qzp.shuidangran.top

var a = 1;  let b = 2
来源：http://tst.gzhubu.top

[T18] Swift：字符串插值
来源：http://vts.svipenyu.cn

"值: \(b)"
来源：http://enr.xuetiantiany.cn

[T19] Swift：可选绑定
来源：http://zfp.ivvv.top

if let n = opt { print(n) }
来源：http://gzq.316326.xyz

[T20] Swift：数组操作
来源：http://ooz.kuanghao11.cn

var a = [1, 2, 3];  a.append(4)
来源：http://jyy.9152youxi.cn

[T21] Swift：遍历
来源：http://xzm.haohaochexian.top

for x in a { print(x) }
来源：http://rjl.nanxinkj.top

[T22] Swift：字典
来源：http://hmt.daxiang520.top

var d = ["a": 1];  d["b"] = 2
来源：http://hej.gzhubu.top

[T23] Swift：函数
来源：http://ynn.bjfxy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ftn.guannengcc.top

[T24] Swift：闭包
来源：http://uor.chenlongwang.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://dda.jyoumei.cn

[T25] Swift：结构体
来源：http://owh.jinqigufen.top

struct P { var x: Int }
来源：http://jsd.xziqi.cn

[T26] Swift：类与重写
来源：http://say.jiagoushi.top

class A: Base { override func f() {} }
来源：http://rhn.pycfn.com

[T27] Swift：错误处理
来源：http://hwe.yj20258.top

do { try f() } catch { print(error) }
来源：http://gcm.uphjek.com

[T28] Swift：枚举
来源：http://rot.cucudq.cn

enum Color { case red, green }
来源：http://bpa.gotoacloud.top

[T29] Swift：guard 提前返回
来源：http://gal.jlsjyb.cn

guard let x = opt else { return }
来源：http://ygy.ehwqpu.com

[T30] Swift：协议
来源：http://mih.ehwqpu.com

protocol Shape { func area() -> Double }
来源：http://zlp.yangfankeji.com

[T31] Lua：Hello World
来源：http://tzs.daria6918.cn

print("Hello")
来源：http://rka.snrcjt.cn

[T32] Lua：局部变量
来源：http://thj.dianchejie.cn

local a = 1
来源：http://rqc.sufxvd.cn

[T33] Lua：表（数组）
来源：http://wmz.fanxiaobao.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://awu.xylfe.cn

[T34] Lua：遍历表
来源：http://wzz.zhoulong.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://rlj.bbcook.cn

[T35] Lua：字典表
来源：http://eip.shzxlz.cn

local d = { a = 1 };  d.b = 2
来源：http://tpz.gogol.net.cn

[T36] Lua：函数
来源：http://ctf.9152youxi.cn

function add(a, b) return a + b end
来源：http://gpu.uphjek.com

[T37] Lua：字符串拼接
来源：http://uws.gogol.net.cn

"a" .. "b"
来源：http://cjt.9152youxi.cn

[T38] Lua：条件
来源：http://lca.yangfankeji.com

if x > 0 then print("正") end
来源：http://zup.jqgfzy.top

[T39] Lua：模式匹配
来源：http://imo.xylfe.cn

string.find(s, "%d+")
来源：http://dvu.shuidangran.top

[T40] Lua：元表
来源：http://leu.yonumen.top

setmetatable({}, { __index = base })
来源：http://qse.sweek.top

[T41] Perl：Hello World
来源：http://udi.ywan-chungtsiang.top

print "Hello\n";
来源：http://eps.kuanghao11.cn

[T42] Perl：变量类型
来源：http://gca.zdbjq.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://erv.hammf.cn

[T43] Perl：字符串插值
来源：http://bey.jiagoushi.top

"值: $a"
来源：http://gft.zhijiandao.cn

[T44] Perl：条件
来源：http://evw.ctjpmb.com

if ($a > 0) { print "正"; }
来源：http://ltf.xinyue.icu

[T45] Perl：数组遍历
来源：http://yvz.ydjk.org.cn

for my $x (@arr) { print $x; }
来源：http://rda.ydjk.org.cn

[T46] Perl：哈希操作
来源：http://ncr.ydjk.org.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qcv.aizwys.cn

[T47] Perl：正则捕获
来源：http://zhd.sufxvd.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://bbw.haohaochexian.top

[T48] Perl：正则替换
来源：http://kjj.c1oappe.top

$s =~ s/old/new/g;
来源：http://ynb.hywenlv.cn

[T49] Perl：函数
来源：http://nxe.shanyushiyangkeji.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cdj.xuanzx.com

[T50] Perl：逐行读文件
来源：http://dno.tianlin.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://awg.nwbrower.top

while (my $line = <$fh>) { print $line; }
来源：http://dxr.yvedp.cn

[T51] Scala：Hello World
来源：http://ukq.hongshengwenyu.top

println("Hello")
来源：http://its.yonumen.top

[T52] Scala：变量
来源：http://wzn.kuanghao11.cn

val a = 1;  var b = 2
来源：http://rso.yj202588.top

[T53] Scala：字符串插值
来源：http://ksr.epnwcf.com

s"值: $b"
来源：http://vrw.dashuyun.cn

[T54] Scala：集合映射
来源：http://ulp.iojbl.cn

List(1, 2, 3).map(_ * 2)
来源：http://kls.zhiwuduotai.top

[T55] Scala：集合过滤
来源：http://zis.hcnkem.com

List(1, 2, 3).filter(_ > 1)
来源：http://xkl.xuetiantiany.cn

[T56] Scala：样例类
来源：http://olj.hnxiangtu.top

case class User(name: String, age: Int)
来源：http://tyu.chenlongwang.top

[T57] Scala：模式匹配
来源：http://jvz.daxiang520.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://udr.meibo888.top

[T58] Scala：函数定义
来源：http://kbn.cheryme.top

def add(a: Int, b: Int): Int = a + b
来源：http://dyl.zhaomingkeji.xyz

[T59] Scala：循环
来源：http://lvc.birdmap.top

for (i <- 1 to 10) println(i)
来源：http://rpu.yfazqb.com

[T60] Scala：折叠
来源：http://egl.xingfuxueyuan.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cau.gzhubu.top

================================================================================
来源：http://aub.52xcode.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ytm.quarkkingdee.top

================================================================================
来源：http://dxy.shangyingyoupin.top

[U01] Py：创建虚拟环境
来源：http://dxo.aizwys.cn

python -m venv .venv && source .venv/bin/activate
来源：http://mfa.quarkkingdee.top

[U02] Py：导出 / 安装依赖
来源：http://hao.gaohongyu789.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://uxe.chenlongwang.top

[U03] Py：加载 .env 配置
来源：http://xju.chenlongwang.top

from dotenv import load_dotenv; load_dotenv()
来源：http://sza.chenzaomai.com

[U04] Py：变量调试打印
来源：http://iqb.shanyushiyangkeji.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dgc.pycfn.com

[U05] Py：列表去重且保序
来源：http://pkz.sufxvd.cn

list(dict.fromkeys(arr))
来源：http://rkk.jyoumei.cn

[U06] Py：合并两个字典
来源：http://bux.nanxuanxn.top

{**a, **b}
来源：http://blj.zhengqikj.top

[U07] Py：反转字典键值
来源：http://rps.yueranfly.top

{v: k for k, v in d.items()}
来源：http://cpu.ybcxt.top

[U08] Py：展平二维列表
来源：http://qfo.tanke756.top

[y for x in nested for y in x]
来源：http://kvq.jyoumei.cn

[U09] Py：字典取最大值的键
来源：http://aml.ydzc1.top

max(d, key=d.get)
来源：http://ari.cqqwz.cn

[U10] Py：按值排序字典
来源：http://joo.sxryk.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jpj.guowangkeji.top

[U11] Py：生成器表达式
来源：http://ibo.kuanghao11.cn

(x * 2 for x in arr)
来源：http://yms.zhiwuduotai.top

[U12] Py：取出现最多的 3 个元素
来源：http://odi.uphjek.com

Counter(arr).most_common(3)
来源：http://wmr.nanxinkj.top

[U13] Py：固定长度队列
来源：http://bul.yangfankeji.com

deque(maxlen=10)
来源：http://cna.ivvv.top

[U14] Py：分组收集到列表
来源：http://njr.nwbrower.top

defaultdict(list)
来源：http://jkl.yonumen.top

[U15] Py：高精度计时
来源：http://yhb.fengsongda.top

t = time.perf_counter()
来源：http://hyg.jinghuilouyu.cn

[U16] Py：命令行参数解析
来源：http://fkv.yvedp.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xvt.haohaochexian.top

[U17] Py：初始化日志
来源：http://dxq.shzxlz.cn

logging.basicConfig(level=logging.INFO)
来源：http://imv.pycfn.com

[U18] Py：预编译正则
来源：http://siy.zhongyouzk.top

pat = re.compile(r"\d+")
来源：http://gpq.xziqi.cn

[U19] Py：正则替换带回调
来源：http://kkm.52xcode.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lgg.zdqjudy.top

[U20] Py：缓存函数结果
来源：http://tkw.svipenyu.cn

@functools.lru_cache(maxsize=None)
来源：http://bcr.hywenlv.cn

[U21] Py：自定义上下文管理器
来源：http://wyz.shanyushiyangkeji.top

@contextlib.contextmanager
来源：http://aun.ybcxt.top

[U22] Py：矩阵转置
来源：http://bde.yuanzhike.top

list(zip(*m))
来源：http://pun.yj202588.top

[U23] Py：分块读取大文件
来源：http://gpa.redwolf501.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ehi.ydjk.org.cn

[U24] Py：路径操作
来源：http://bha.shzxlz.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hze.ydzc1.top

[U25] Py：CSV 按字典读
来源：http://xdv.yj202588.top

csv.DictReader(f)
来源：http://wjp.hnxiangtu.top

[U26] Py：并发下载
来源：http://pxq.chenzaomai.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gfc.jinyuanbaomall.cn

[U27] Py：异步 HTTP
来源：http://set.dashuyun.cn

aiohttp.ClientSession() 配合 async with
来源：http://fya.hcnkem.com

[U28] Py：类型别名
来源：http://uyz.jlsjyb.cn

UserId = int
来源：http://wpy.bbcook.cn

[U29] Py：属性校验
来源：http://ttm.meibo888.top

@property 与 @x.setter 配合
来源：http://qkh.yuxming.cn

[U30] Py：数据类
来源：http://jep.9152youxi.cn

@dataclass(slots=True)
来源：http://dcz.9152youxi.cn

[U31] Py：单测
来源：http://fos.svipenyu.cn

python -m pytest -q
来源：http://zfm.tian-w.cn

[U32] Py：代码格式化
来源：http://zuq.jinghuilouyu.cn

ruff format . && ruff check --fix .
来源：http://vdq.nwbrower.top

[U33] Py：打包发布
来源：http://ncw.jqgfzy.top

python -m build  （依赖 pyproject.toml）
来源：http://hll.meibo888.top

[U34] Py：判断编码
来源：http://bku.jqgfzy.top

chardet.detect(raw)
来源：http://udq.jlsjyb.cn

[U35] Py：发送邮件
来源：http://fzi.gotoacloud.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://lvz.tarul.cn

[U36] Py：定时任务
来源：http://mhp.shanyushiyangtech.top

schedule.every(10).minutes.do(job)
来源：http://dji.guannengcc.top

[U37] Py：读写 Excel
来源：http://uyo.tian-w.cn

pandas.read_excel / DataFrame.to_excel
来源：http://qui.yonumen.top

[U38] Py：获取脚本所在目录
来源：http://dtu.fanxiaobao.xyz

Path(__file__).resolve().parent
来源：http://enw.vqdsnc.cn

[U39] Py：判断是否在交互环境
来源：http://xri.yueranfly.top

sys.stdout.isatty()
来源：http://frf.shuidangran.top

[U40] Py：打印到标准错误
来源：http://vgf.jinqigfzy.top

print("err", file=sys.stderr)
来源：http://xua.zdbjq.cn

[U41] PHP：初始化 Composer 项目
来源：http://rdz.9152youxi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://xad.hnxiangtu.top

[U42] PHP：PSR-4 自动加载
来源：http://yat.sweek.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zbz.yuanzhike.top

[U43] PHP：声明命名空间
来源：http://cms.zhaomingkeji.xyz

namespace App\Http;
来源：http://uhz.sxryk.cn

[U44] PHP：开启严格类型
来源：http://kux.shzxlz.cn

declare(strict_types=1);
来源：http://whl.sweek.top

[U45] PHP：类型声明与返回类型
来源：http://byf.cdnleiting.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://dyl.tianlin.xyz

[U46] PHP：可空类型
来源：http://ivq.sweek.top

?string $name = null
来源：http://kpf.ppjwa.cn

[U47] PHP：联合类型
来源：http://arl.jlsjyb.cn

int|string $id
来源：http://ccs.jlsjyb.cn

[U48] PHP：纯枚举
来源：http://sog.jqgufenzy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xyu.havefunace.top

[U49] PHP：只读属性
来源：http://uoa.epnwcf.com

public readonly string $name
来源：http://gox.smart0.xyz

[U50] PHP：构造器属性提升
来源：http://jcl.zhongyouzk.top

public function __construct(private int $id) {}
来源：http://avp.shanyushiyangkeji.top

[U51] PHP：数组解构
来源：http://ydw.havefunace.top

[$a, $b] = $arr;
来源：http://rxi.tanke756.top

[U52] PHP：箭头函数
来源：http://hms.bjfxy.top

$double = fn($x) => $x * 2;
来源：http://wky.hysaishi.cn

[U53] PHP：空合并运算符
来源：http://onm.chenjidiqi.icu

$v = $a ?? $b ?? "default";
来源：http://qom.guannengcc.top

[U54] PHP：空安全调用
来源：http://trm.guowangkeji.top

$obj?->method()
来源：http://ppu.ivvv.top

[U55] PHP：match 表达式
来源：http://jjj.shangyingyoupin.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vcs.xziqi.cn

[U56] PHP：命名参数
来源：http://cqm.meibo888.top

f(a: 1, b: 2)
来源：http://tzx.xuanzx.com

[U57] PHP：字符串插值
来源：http://gjk.fzhhl.top

"值: {$a}"
来源：http://mgk.nanxinkj.top

[U58] PHP：数组三件套
来源：http://ghk.uphjek.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://okt.fzhhl.top

[U59] PHP：自定义排序
来源：http://pwj.jqgufenzy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fcn.chenzaomai.com

[U60] PHP：JSON 编解码
来源：http://cuz.daxiang520.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://aud.kuanghao11.cn

[U61] PHP：正则
来源：http://dys.zhijiandao.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ueo.dashuyun.cn

[U62] PHP：日期对象
来源：http://jir.yueranfly.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wkz.yueranfly.top

[U63] PHP：文件读写
来源：http://ddu.guowangkeji.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://swo.jqgufenzy.top

[U64] PHP：目录遍历
来源：http://qro.pycfn.com

glob("dir/*.php");  scandir("dir");
来源：http://elq.shanyushiyangtech.top

[U65] PHP：会话
来源：http://ydw.shangyingyoupin.top

session_start();  $_SESSION["uid"] = 1;
来源：http://bxi.hesvh.cn

[U66] PHP：设置 Cookie
来源：http://khk.sufxvd.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kgl.pengpengdd.cyou

[U67] PHP：处理文件上传
来源：http://pds.zhixingplan.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kjz.hfpthk.cn

[U68] PHP：PDO 连接
来源：http://vak.aibaodan.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nlg.yanxiufei.cn

[U69] PHP：PDO 预处理
来源：http://ymh.cheryme.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lym.hfpthk.cn

[U70] PHP：PDO 事务
来源：http://ktt.fktsv.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fhf.ydjk.org.cn

[U71] PHP：抛出异常
来源：http://sly.sweek.top

throw new RuntimeException("失败", 500);
来源：http://xde.yuanzhike.top

[U72] PHP：写错误日志
来源：http://hou.yangfankeji.com

error_log("失败: " . $e->getMessage());
来源：http://dpk.nanxuanxn.top


<!-- 参考信息 -->