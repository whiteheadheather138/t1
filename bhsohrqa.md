代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kpo.mhx1999.top

[S51] C++：显式类型转换
来源：http://nvf.quarkkingdee.top

static_cast<double>(a) / b
来源：http://hrw.tian-w.cn

[S52] C++：const 与 noexcept
来源：http://yie.ivvv.top

int size() const noexcept { return n_; }
来源：http://czv.smart0.xyz

[S53] C++：移动语义
来源：http://acv.fehbvm.com

std::vector<int> w = std::move(v);
来源：http://jyc.zhengqikj.top

[S54] C++：异常处理
来源：http://ruc.yongpay.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://aoc.ywan-chungtsiang.top

[S55] C++：结构化绑定
来源：http://hgx.zhaomingkeji.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://qej.yangfankeji.com

[S56] C++：optional
来源：http://riz.nanxuanxn.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qws.nanxuanxn.top

[S57] C++：编译期常量
来源：http://hje.yueranfly.top

constexpr int N = 10;
来源：http://hyj.yj20258888.top

[S58] C++：命名空间
来源：http://eii.jlsjyb.cn

namespace ns { int f() { return 1; } }
来源：http://wjb.snrcjt.cn

[S59] C++：静态断言
来源：http://rvl.aizwys.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lzm.xuetiantiany.cn

[S60] C++：遍历并删除元素
来源：http://jzz.aibaodan.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wmk.vehdjk.com

================================================================================
来源：http://san.jqgfzy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xys.shanyushiyangtech.top

================================================================================
来源：http://nql.sufxvd.cn

[T01] Kotlin：Hello World
来源：http://jzj.yonumen.top

println("Hello")
来源：http://abs.jqgfzy.top

[T02] Kotlin：变量
来源：http://gmq.shzxlz.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lkb.ivvv.top

[T03] Kotlin：字符串模板
来源：http://cty.cucudq.cn

"值: $b"
来源：http://nuu.sufxvd.cn

[T04] Kotlin：空安全
来源：http://qaq.gaohongyu789.top

val n: String? = null;  n?.length
来源：http://neg.ydjk.org.cn

[T05] Kotlin：when 表达式
来源：http://hhc.yj202588.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mfv.havefunace.top

[T06] Kotlin：集合映射
来源：http://nsq.pengpengdd.cyou

listOf(1, 2, 3).map { it * 2 }
来源：http://drt.hesvh.cn

[T07] Kotlin：集合过滤
来源：http://zto.chenjidiqi.icu

listOf(1, 2, 3).filter { it > 1 }
来源：http://llq.svipenyu.cn

[T08] Kotlin：数据类
来源：http://yex.daxiang520.top

data class User(val name: String, val age: Int)
来源：http://rjo.guannengcc.top

[T09] Kotlin：扩展函数
来源：http://ars.xziqi.cn

fun String.exclaim() = this + "!"
来源：http://wdc.xingfuxueyuan.xyz

[T10] Kotlin：默认参数
来源：http://wpd.zhoulong.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://qpm.zhengqikj.top

[T11] Kotlin：协程
来源：http://lii.jqgfzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://rif.hywenlv.cn

[T12] Kotlin：解构声明
来源：http://ufr.cqqwz.cn

val (a, b) = Pair(1, 2)
来源：http://ouy.hfpthk.cn

[T13] Kotlin：只读 Map
来源：http://dku.yuanzhike.top

val m = mapOf("a" to 1)
来源：http://hsw.sweek.top

[T14] Kotlin：循环
来源：http://clw.guannengcc.top

for (i in 1..10) println(i)
来源：http://utu.kuanghao11.cn

[T15] Kotlin：接口
来源：http://gou.pycfn.com

interface Shape { fun area(): Double }
来源：http://xmp.andypj.xyz

[T16] Swift：Hello World
来源：http://zjz.dashuyun.cn

print("Hello")
来源：http://olb.mhx1999.top

[T17] Swift：变量与常量
来源：http://nxt.hnxiangtu.top

var a = 1;  let b = 2
来源：http://toz.dashuyun.cn

[T18] Swift：字符串插值
来源：http://nkb.meibo888.top

"值: \(b)"
来源：http://zlg.epnwcf.com

[T19] Swift：可选绑定
来源：http://qac.yj20258.top

if let n = opt { print(n) }
来源：http://tqw.pengpengdd.cyou

[T20] Swift：数组操作
来源：http://suu.dianchejie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://nxw.yangfankeji.com

[T21] Swift：遍历
来源：http://dol.sysykeji.top

for x in a { print(x) }
来源：http://nqa.cheryme.top

[T22] Swift：字典
来源：http://jyn.feifeiyinyue.top

var d = ["a": 1];  d["b"] = 2
来源：http://xxt.shzxlz.cn

[T23] Swift：函数
来源：http://zyw.tian-w.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://opp.hnqzz.top

[T24] Swift：闭包
来源：http://dsc.redwolf501.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://jma.chenzaomai.com

[T25] Swift：结构体
来源：http://bgm.pengpengdd.cyou

struct P { var x: Int }
来源：http://vau.hnqzz.top

[T26] Swift：类与重写
来源：http://iki.hfpthk.cn

class A: Base { override func f() {} }
来源：http://wxk.andypj.xyz

[T27] Swift：错误处理
来源：http://ogp.yj20258.top

do { try f() } catch { print(error) }
来源：http://fat.aizwys.cn

[T28] Swift：枚举
来源：http://mvz.jinqigufen.top

enum Color { case red, green }
来源：http://dfc.hywenlv.cn

[T29] Swift：guard 提前返回
来源：http://lgs.zhiwuduotai.top

guard let x = opt else { return }
来源：http://zlw.yueranfly.top

[T30] Swift：协议
来源：http://pir.yj20258.top

protocol Shape { func area() -> Double }
来源：http://xbv.xinyue.icu

[T31] Lua：Hello World
来源：http://abl.shangyingyoupin.top

print("Hello")
来源：http://xid.ywan-chungtsiang.top

[T32] Lua：局部变量
来源：http://ldq.shangyingyoupin.top

local a = 1
来源：http://vxk.yuxming.cn

[T33] Lua：表（数组）
来源：http://lnk.jinyuanbaomall.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://kre.zdqjudy.top

[T34] Lua：遍历表
来源：http://ifn.yvedp.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://huz.yangfankeji.com

[T35] Lua：字典表
来源：http://wun.ppjwa.cn

local d = { a = 1 };  d.b = 2
来源：http://rhm.hnqzz.top

[T36] Lua：函数
来源：http://iqi.zhixingplan.top

function add(a, b) return a + b end
来源：http://eoi.guowangkeji.top

[T37] Lua：字符串拼接
来源：http://tyk.chenzaomai.com

"a" .. "b"
来源：http://awd.jlsjyb.cn

[T38] Lua：条件
来源：http://ogi.vqdsnc.cn

if x > 0 then print("正") end
来源：http://mzr.uphjek.com

[T39] Lua：模式匹配
来源：http://upp.uphjek.com

string.find(s, "%d+")
来源：http://cxw.zdqjudy.top

[T40] Lua：元表
来源：http://qqo.gaohongyu789.top

setmetatable({}, { __index = base })
来源：http://spc.zhiwuduotai.top

[T41] Perl：Hello World
来源：http://wbj.quarkkingdee.top

print "Hello\n";
来源：http://klx.c1oappe.top

[T42] Perl：变量类型
来源：http://xiy.tanke756.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://apr.gotoacloud.top

[T43] Perl：字符串插值
来源：http://ifb.ehwqpu.com

"值: $a"
来源：http://yds.shanyushiyangtech.top

[T44] Perl：条件
来源：http://mhv.fanxiaobao.xyz

if ($a > 0) { print "正"; }
来源：http://jub.xuanzx.com

[T45] Perl：数组遍历
来源：http://wwq.tian-w.cn

for my $x (@arr) { print $x; }
来源：http://scp.hywenlv.cn

[T46] Perl：哈希操作
来源：http://rza.yanxiufei.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nlw.zhoulong.xyz

[T47] Perl：正则捕获
来源：http://ewv.yfazqb.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://jbg.epnwcf.com

[T48] Perl：正则替换
来源：http://hem.epnwcf.com

$s =~ s/old/new/g;
来源：http://vuy.jyoumei.cn

[T49] Perl：函数
来源：http://vvw.bjfxy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://olt.redwolf501.top

[T50] Perl：逐行读文件
来源：http://qzd.cqqwz.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ban.tanke756.top

while (my $line = <$fh>) { print $line; }
来源：http://eue.quarkkingdee.top

[T51] Scala：Hello World
来源：http://zxs.yj20258888.top

println("Hello")
来源：http://ggc.vqdsnc.cn

[T52] Scala：变量
来源：http://cqp.cheryme.top

val a = 1;  var b = 2
来源：http://hay.jinqigfzy.top

[T53] Scala：字符串插值
来源：http://hen.jqgfzy.top

s"值: $b"
来源：http://dov.yj20258.top

[T54] Scala：集合映射
来源：http://nts.xylfe.cn

List(1, 2, 3).map(_ * 2)
来源：http://cch.cashguo.top

[T55] Scala：集合过滤
来源：http://ulo.nanxinkj.top

List(1, 2, 3).filter(_ > 1)
来源：http://afk.svipenyu.cn

[T56] Scala：样例类
来源：http://gye.nanxinkj.top

case class User(name: String, age: Int)
来源：http://hvn.yueranfly.top

[T57] Scala：模式匹配
来源：http://ccu.xziqi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://orf.haohaochexian.top

[T58] Scala：函数定义
来源：http://lcf.bbcook.cn

def add(a: Int, b: Int): Int = a + b
来源：http://qku.316326.xyz

[T59] Scala：循环
来源：http://fxs.cheryme.top

for (i <- 1 to 10) println(i)
来源：http://twb.hcnkem.com

[T60] Scala：折叠
来源：http://agx.jiagoushi.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pgv.52xcode.cn

================================================================================
来源：http://xpc.yongpay.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bmv.fehbvm.com

================================================================================
来源：http://lru.svipenyu.cn

[U01] Py：创建虚拟环境
来源：http://hcb.zhiwuduotai.top

python -m venv .venv && source .venv/bin/activate
来源：http://vti.fengsongda.top

[U02] Py：导出 / 安装依赖
来源：http://qcr.aizwys.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://drx.yangfankeji.com

[U03] Py：加载 .env 配置
来源：http://duk.cqqwz.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://yjt.hesvh.cn

[U04] Py：变量调试打印
来源：http://pgo.yfazqb.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://abr.dianchejie.cn

[U05] Py：列表去重且保序
来源：http://pyy.aibaodan.cn

list(dict.fromkeys(arr))
来源：http://kuj.hnxiangtu.top

[U06] Py：合并两个字典
来源：http://qtc.tarul.cn

{**a, **b}
来源：http://umr.zhijiandao.cn

[U07] Py：反转字典键值
来源：http://gkl.xingfuxueyuan.xyz

{v: k for k, v in d.items()}
来源：http://kap.tarul.cn

[U08] Py：展平二维列表
来源：http://nga.zhijiandao.cn

[y for x in nested for y in x]
来源：http://pkb.yonumen.top

[U09] Py：字典取最大值的键
来源：http://upz.yangfankeji.com

max(d, key=d.get)
来源：http://qvd.smart0.xyz

[U10] Py：按值排序字典
来源：http://oef.zhongyouzk.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zuq.hcnkem.com

[U11] Py：生成器表达式
来源：http://vyv.chenjidiqi.icu

(x * 2 for x in arr)
来源：http://itr.sysykeji.top

[U12] Py：取出现最多的 3 个元素
来源：http://kxq.tian-w.cn

Counter(arr).most_common(3)
来源：http://gge.fktsv.cn

[U13] Py：固定长度队列
来源：http://yji.ydjk.org.cn

deque(maxlen=10)
来源：http://fgz.jinyuanbaomall.cn

[U14] Py：分组收集到列表
来源：http://hek.cucudq.cn

defaultdict(list)
来源：http://mit.meibo888.top

[U15] Py：高精度计时
来源：http://poc.cashguo.top

t = time.perf_counter()
来源：http://pmt.aizwys.cn

[U16] Py：命令行参数解析
来源：http://wyy.sufxvd.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yaq.gotoacloud.top

[U17] Py：初始化日志
来源：http://dub.sufxvd.cn

logging.basicConfig(level=logging.INFO)
来源：http://ymy.wangshuangyany.cn

[U18] Py：预编译正则
来源：http://hxw.havefunace.top

pat = re.compile(r"\d+")
来源：http://rxc.bjfxy.top

[U19] Py：正则替换带回调
来源：http://bmf.fzhhl.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wgz.gzhubu.top

[U20] Py：缓存函数结果
来源：http://wyf.ydzc1.top

@functools.lru_cache(maxsize=None)
来源：http://dkx.zhixingplan.top

[U21] Py：自定义上下文管理器
来源：http://dne.hesvh.cn

@contextlib.contextmanager
来源：http://mfx.jinqigfzy.top

[U22] Py：矩阵转置
来源：http://whb.svipenyu.cn

list(zip(*m))
来源：http://hls.yj20258888.top

[U23] Py：分块读取大文件
来源：http://cll.havefunace.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://crw.hnqzz.top

[U24] Py：路径操作
来源：http://ylt.daria6918.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xni.chenzaomai.com

[U25] Py：CSV 按字典读
来源：http://yzm.xinyue.icu

csv.DictReader(f)
来源：http://bdl.hammf.cn

[U26] Py：并发下载
来源：http://vug.hnxiangtu.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wlp.nanxuanxn.top

[U27] Py：异步 HTTP
来源：http://haj.hesvh.cn

aiohttp.ClientSession() 配合 async with
来源：http://unu.yongpay.top

[U28] Py：类型别名
来源：http://wjr.jiagoushi.top

UserId = int
来源：http://qow.yj202588.top

[U29] Py：属性校验
来源：http://not.zdbjq.cn

@property 与 @x.setter 配合
来源：http://rao.gzhubu.top

[U30] Py：数据类
来源：http://vzj.hesvh.cn

@dataclass(slots=True)
来源：http://tuc.chenjidiqi.icu

[U31] Py：单测
来源：http://fqa.hfpthk.cn

python -m pytest -q
来源：http://job.yangfankeji.com

[U32] Py：代码格式化
来源：http://lhk.ybcxt.top

ruff format . && ruff check --fix .
来源：http://gvm.jinghuilouyu.cn

[U33] Py：打包发布
来源：http://hvj.tian-w.cn

python -m build  （依赖 pyproject.toml）
来源：http://etb.shanyushiyangkeji.top

[U34] Py：判断编码
来源：http://kqu.hywenlv.cn

chardet.detect(raw)
来源：http://yau.cucudq.cn

[U35] Py：发送邮件
来源：http://tbh.quarkkingdee.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hzi.hysaishi.cn

[U36] Py：定时任务
来源：http://zup.zhixingplan.top

schedule.every(10).minutes.do(job)
来源：http://yrm.hcnkem.com

[U37] Py：读写 Excel
来源：http://eml.smart0.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://irc.shangyingyoupin.top

[U38] Py：获取脚本所在目录
来源：http://glr.ydzc1.top

Path(__file__).resolve().parent
来源：http://iea.aibaodan.cn

[U39] Py：判断是否在交互环境
来源：http://vdj.smart0.xyz

sys.stdout.isatty()
来源：http://cxh.tian-w.cn

[U40] Py：打印到标准错误
来源：http://erv.tanke756.top

print("err", file=sys.stderr)
来源：http://fcc.0kj1m.cn

[U41] PHP：初始化 Composer 项目
来源：http://ndq.yj202588.top

composer init;  composer require guzzlehttp/guzzle
来源：http://fve.svipenyu.cn

[U42] PHP：PSR-4 自动加载
来源：http://xpm.jqgfzy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nca.quarkkingdee.top

[U43] PHP：声明命名空间
来源：http://fjm.vehdjk.com

namespace App\Http;
来源：http://ulc.snrcjt.cn

[U44] PHP：开启严格类型
来源：http://nxs.shuidangran.top

declare(strict_types=1);
来源：http://ghs.shanyushiyangkeji.top

[U45] PHP：类型声明与返回类型
来源：http://fzm.xinyue.icu

function add(int $a, int $b): int { return $a + $b; }
来源：http://wve.bjfxy.top

[U46] PHP：可空类型
来源：http://ydh.9152youxi.cn

?string $name = null
来源：http://ppy.cqqwz.cn

[U47] PHP：联合类型
来源：http://omw.c1oappe.top

int|string $id
来源：http://qxz.gaohongyu789.top

[U48] PHP：纯枚举
来源：http://tdx.tian-w.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vjq.jinqigufen.top

[U49] PHP：只读属性
来源：http://fzo.shangyingyoupin.top

public readonly string $name
来源：http://amt.aizwys.cn

[U50] PHP：构造器属性提升
来源：http://vsw.jinghuilouyu.cn

public function __construct(private int $id) {}
来源：http://sjd.hfpthk.cn

[U51] PHP：数组解构
来源：http://wlc.gotoacloud.top

[$a, $b] = $arr;
来源：http://ekv.nanxuanxn.top

[U52] PHP：箭头函数
来源：http://pyy.daria6918.cn

$double = fn($x) => $x * 2;
来源：http://thd.nanxuanxn.top

[U53] PHP：空合并运算符
来源：http://ijt.zhiwuduotai.top

$v = $a ?? $b ?? "default";
来源：http://zce.hywenlv.cn

[U54] PHP：空安全调用
来源：http://mfz.uphjek.com

$obj?->method()
来源：http://uhq.fehbvm.com

[U55] PHP：match 表达式
来源：http://xqg.jyoumei.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gbl.chenjidiqi.icu

[U56] PHP：命名参数
来源：http://tvc.meibo888.top

f(a: 1, b: 2)
来源：http://uzy.gotoacloud.top

[U57] PHP：字符串插值
来源：http://ymb.yvedp.cn

"值: {$a}"
来源：http://jbq.yonumen.top

[U58] PHP：数组三件套
来源：http://wih.tianlin.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rsw.zycfv.cn

[U59] PHP：自定义排序
来源：http://jyu.shzxlz.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zoh.jianghu66.top

[U60] PHP：JSON 编解码
来源：http://hzw.yonumen.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vny.ywan-chungtsiang.top

[U61] PHP：正则
来源：http://ycw.jinqigfzy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zfo.tarul.cn

[U62] PHP：日期对象
来源：http://lrn.zhoulong.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://yfz.redwolf501.top

[U63] PHP：文件读写
来源：http://tur.vehdjk.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ahx.yanxiufei.cn

[U64] PHP：目录遍历
来源：http://hcs.vehdjk.com

glob("dir/*.php");  scandir("dir");
来源：http://heo.daxiang520.top

[U65] PHP：会话
来源：http://bnf.shangyingyoupin.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ifh.quarkkingdee.top

[U66] PHP：设置 Cookie
来源：http://cvk.gaohongyu789.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ofb.smart0.xyz

[U67] PHP：处理文件上传
来源：http://cqu.bjfxy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://llf.epnwcf.com

[U68] PHP：PDO 连接
来源：http://nyg.sysykeji.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wft.ywan-chungtsiang.top

[U69] PHP：PDO 预处理
来源：http://flb.sweek.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://euk.316326.xyz

[U70] PHP：PDO 事务
来源：http://xfn.redwolf501.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lzt.hammf.cn

[U71] PHP：抛出异常
来源：http://jio.daria6918.cn

throw new RuntimeException("失败", 500);
来源：http://lqe.guowangkeji.top

[U72] PHP：写错误日志
来源：http://jug.zhixingplan.top

error_log("失败: " . $e->getMessage());
来源：http://iby.iojbl.cn

[U73] PHP：读取 ini 配置
来源：http://ovr.tarul.cn

parse_ini_file("config.ini", true)
来源：http://jfe.meibo888.top

[U74] PHP：读取环境变量
来源：http://rbn.guowangkeji.top

getenv("APP_ENV") ?: "production"
来源：http://qqz.birdmap.top

[U75] PHP：依赖注入
来源：http://gcz.redwolf501.top

composer require psr/container
来源：http://gbt.jinghuilouyu.cn

[U76] PHP：简单路由
来源：http://dnw.jinqigufen.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vwh.bbcook.cn


<!-- 参考信息 -->