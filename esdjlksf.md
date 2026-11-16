代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jzo.sxryk.cn

[S51] C++：显式类型转换
来源：http://qfj.ybcxt.top

static_cast<double>(a) / b
来源：http://ftj.bjfxy.top

[S52] C++：const 与 noexcept
来源：http://nlq.quarkkingdee.top

int size() const noexcept { return n_; }
来源：http://ldh.guannengcc.top

[S53] C++：移动语义
来源：http://yva.redwolf501.top

std::vector<int> w = std::move(v);
来源：http://nwn.yj20258888.top

[S54] C++：异常处理
来源：http://bbj.svipenyu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sfs.9152youxi.cn

[S55] C++：结构化绑定
来源：http://ilf.hnqzz.top

auto [a, b] = std::make_pair(1, 2);
来源：http://gny.pycfn.com

[S56] C++：optional
来源：http://vjd.svipenyu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://sna.zhoulong.xyz

[S57] C++：编译期常量
来源：http://sab.yfazqb.com

constexpr int N = 10;
来源：http://blb.cucudq.cn

[S58] C++：命名空间
来源：http://nco.zhiwuduotai.top

namespace ns { int f() { return 1; } }
来源：http://wrc.jlsjyb.cn

[S59] C++：静态断言
来源：http://aik.ybcxt.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lyq.chenzaomai.com

[S60] C++：遍历并删除元素
来源：http://wru.tianlin.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bxs.cqqwz.cn

================================================================================
来源：http://ipx.9152youxi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ryr.epnwcf.com

================================================================================
来源：http://ush.zdbjq.cn

[T01] Kotlin：Hello World
来源：http://gdm.bjfxy.top

println("Hello")
来源：http://kww.kuanghao11.cn

[T02] Kotlin：变量
来源：http://fgq.redwolf501.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zof.iojbl.cn

[T03] Kotlin：字符串模板
来源：http://cja.yangfankeji.com

"值: $b"
来源：http://gct.tanke756.top

[T04] Kotlin：空安全
来源：http://pni.shuidangran.top

val n: String? = null;  n?.length
来源：http://wya.haohaochexian.top

[T05] Kotlin：when 表达式
来源：http://uhi.xuanzx.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cmj.jinyuanbaomall.cn

[T06] Kotlin：集合映射
来源：http://vur.guannengcc.top

listOf(1, 2, 3).map { it * 2 }
来源：http://mbb.xylfe.cn

[T07] Kotlin：集合过滤
来源：http://mmp.yongpay.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://kui.xingfuxueyuan.xyz

[T08] Kotlin：数据类
来源：http://ysh.aizwys.cn

data class User(val name: String, val age: Int)
来源：http://chj.xinyue.icu

[T09] Kotlin：扩展函数
来源：http://tzl.fengsongda.top

fun String.exclaim() = this + "!"
来源：http://qqb.52xcode.cn

[T10] Kotlin：默认参数
来源：http://sxn.fktsv.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://hnn.meibo888.top

[T11] Kotlin：协程
来源：http://ffa.fzhhl.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://rjy.yj202588.top

[T12] Kotlin：解构声明
来源：http://vee.tarul.cn

val (a, b) = Pair(1, 2)
来源：http://ijv.bjfxy.top

[T13] Kotlin：只读 Map
来源：http://jnj.cucudq.cn

val m = mapOf("a" to 1)
来源：http://puw.hfpthk.cn

[T14] Kotlin：循环
来源：http://qxk.bjfxy.top

for (i in 1..10) println(i)
来源：http://vpl.zhiwuduotai.top

[T15] Kotlin：接口
来源：http://pxd.jinqigfzy.top

interface Shape { fun area(): Double }
来源：http://cnc.shuidangran.top

[T16] Swift：Hello World
来源：http://aqh.daria6918.cn

print("Hello")
来源：http://dsi.hywenlv.cn

[T17] Swift：变量与常量
来源：http://kza.jiagoushi.top

var a = 1;  let b = 2
来源：http://bcm.kuanghao11.cn

[T18] Swift：字符串插值
来源：http://yyb.jinghuilouyu.cn

"值: \(b)"
来源：http://pii.yonumen.top

[T19] Swift：可选绑定
来源：http://czg.xylfe.cn

if let n = opt { print(n) }
来源：http://adv.yonumen.top

[T20] Swift：数组操作
来源：http://ndw.52xcode.cn

var a = [1, 2, 3];  a.append(4)
来源：http://mbg.snrcjt.cn

[T21] Swift：遍历
来源：http://fjd.zhengqikj.top

for x in a { print(x) }
来源：http://faa.nanxuanxn.top

[T22] Swift：字典
来源：http://vfb.aizwys.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ssn.feifeiyinyue.top

[T23] Swift：函数
来源：http://gjo.xuetiantiany.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://smc.jinghuilouyu.cn

[T24] Swift：闭包
来源：http://rnl.cashguo.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://wrh.hnxiangtu.top

[T25] Swift：结构体
来源：http://gxp.bbcook.cn

struct P { var x: Int }
来源：http://aam.jinqigufen.top

[T26] Swift：类与重写
来源：http://dff.ctjpmb.com

class A: Base { override func f() {} }
来源：http://byn.gaohongyu789.top

[T27] Swift：错误处理
来源：http://csf.meibo888.top

do { try f() } catch { print(error) }
来源：http://cyg.gotoacloud.top

[T28] Swift：枚举
来源：http://djq.yuxming.cn

enum Color { case red, green }
来源：http://xog.yj202588.top

[T29] Swift：guard 提前返回
来源：http://oyx.pengpengdd.cyou

guard let x = opt else { return }
来源：http://ayf.jyoumei.cn

[T30] Swift：协议
来源：http://unk.guannengcc.top

protocol Shape { func area() -> Double }
来源：http://nia.nanxuanxn.top

[T31] Lua：Hello World
来源：http://ljr.zhixingplan.top

print("Hello")
来源：http://vaj.chenzaomai.com

[T32] Lua：局部变量
来源：http://tai.guannengcc.top

local a = 1
来源：http://lhj.yonumen.top

[T33] Lua：表（数组）
来源：http://xen.zhijiandao.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hvt.nanxuanxn.top

[T34] Lua：遍历表
来源：http://keg.xuetiantiany.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://mho.hnxiangtu.top

[T35] Lua：字典表
来源：http://joz.tanke756.top

local d = { a = 1 };  d.b = 2
来源：http://psf.gzhubu.top

[T36] Lua：函数
来源：http://gpc.cheryme.top

function add(a, b) return a + b end
来源：http://gae.ppjwa.cn

[T37] Lua：字符串拼接
来源：http://loy.chenlongwang.top

"a" .. "b"
来源：http://rdj.hnxiangtu.top

[T38] Lua：条件
来源：http://ftx.jiagoushi.top

if x > 0 then print("正") end
来源：http://lyr.bjfxy.top

[T39] Lua：模式匹配
来源：http://bzs.zhiwuduotai.top

string.find(s, "%d+")
来源：http://trn.hcnkem.com

[T40] Lua：元表
来源：http://tnr.yvedp.cn

setmetatable({}, { __index = base })
来源：http://bxn.gotoacloud.top

[T41] Perl：Hello World
来源：http://tfn.daria6918.cn

print "Hello\n";
来源：http://knb.gotoacloud.top

[T42] Perl：变量类型
来源：http://bba.zhiwuduotai.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zfc.yangfankeji.com

[T43] Perl：字符串插值
来源：http://tip.fengsongda.top

"值: $a"
来源：http://kbm.daria6918.cn

[T44] Perl：条件
来源：http://jss.fanxiaobao.xyz

if ($a > 0) { print "正"; }
来源：http://klo.ydzc1.top

[T45] Perl：数组遍历
来源：http://rtw.shanyushiyangtech.top

for my $x (@arr) { print $x; }
来源：http://xbh.jyoumei.cn

[T46] Perl：哈希操作
来源：http://ctc.c1oappe.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nko.fzhhl.top

[T47] Perl：正则捕获
来源：http://huy.cdnleiting.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://phq.sjlbkw.cn

[T48] Perl：正则替换
来源：http://usw.fktsv.cn

$s =~ s/old/new/g;
来源：http://cdr.hnqzz.top

[T49] Perl：函数
来源：http://xtp.mhx1999.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wiy.zhongyouzk.top

[T50] Perl：逐行读文件
来源：http://tkg.fzhhl.top

open my $fh, "<", "a.txt" or die $!;
来源：http://gyy.316326.xyz

while (my $line = <$fh>) { print $line; }
来源：http://vel.shuidangran.top

[T51] Scala：Hello World
来源：http://dly.tanke756.top

println("Hello")
来源：http://fcw.sjlbkw.cn

[T52] Scala：变量
来源：http://hng.jinyuanbaomall.cn

val a = 1;  var b = 2
来源：http://hvq.c1oappe.top

[T53] Scala：字符串插值
来源：http://jia.hcnkem.com

s"值: $b"
来源：http://ihi.hnqzz.top

[T54] Scala：集合映射
来源：http://ptf.guannengcc.top

List(1, 2, 3).map(_ * 2)
来源：http://fhn.zhijiandao.cn

[T55] Scala：集合过滤
来源：http://zcf.chenjidiqi.icu

List(1, 2, 3).filter(_ > 1)
来源：http://afz.nwbrower.top

[T56] Scala：样例类
来源：http://mhl.xinyue.icu

case class User(name: String, age: Int)
来源：http://yjw.hysaishi.cn

[T57] Scala：模式匹配
来源：http://yua.jiagoushi.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://lrt.svipenyu.cn

[T58] Scala：函数定义
来源：http://psw.nanxinkj.top

def add(a: Int, b: Int): Int = a + b
来源：http://yba.hongshengwenyu.top

[T59] Scala：循环
来源：http://amt.hnqzz.top

for (i <- 1 to 10) println(i)
来源：http://upr.gzhubu.top

[T60] Scala：折叠
来源：http://whp.cdnleiting.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://udm.svipenyu.cn

================================================================================
来源：http://qrn.ehwqpu.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nqe.shzxlz.cn

================================================================================
来源：http://tna.shanyushiyangkeji.top

[U01] Py：创建虚拟环境
来源：http://ork.xingfuxueyuan.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://ggd.jinyuanbaomall.cn

[U02] Py：导出 / 安装依赖
来源：http://gkr.redwolf501.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gom.yj20258.top

[U03] Py：加载 .env 配置
来源：http://iea.hammf.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xwh.sweek.top

[U04] Py：变量调试打印
来源：http://qxk.fktsv.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kbu.tarul.cn

[U05] Py：列表去重且保序
来源：http://ipg.yvedp.cn

list(dict.fromkeys(arr))
来源：http://yqj.snrcjt.cn

[U06] Py：合并两个字典
来源：http://bdm.feifeiyinyue.top

{**a, **b}
来源：http://oep.andypj.xyz

[U07] Py：反转字典键值
来源：http://akq.redwolf501.top

{v: k for k, v in d.items()}
来源：http://uze.quarkkingdee.top

[U08] Py：展平二维列表
来源：http://uyp.chenjidiqi.icu

[y for x in nested for y in x]
来源：http://cbg.shanyushiyangtech.top

[U09] Py：字典取最大值的键
来源：http://feq.pycfn.com

max(d, key=d.get)
来源：http://tvc.shzxlz.cn

[U10] Py：按值排序字典
来源：http://gsc.meibo888.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hdg.zhaomingkeji.xyz

[U11] Py：生成器表达式
来源：http://bjk.ydjk.org.cn

(x * 2 for x in arr)
来源：http://riq.chenzaomai.com

[U12] Py：取出现最多的 3 个元素
来源：http://moi.52xcode.cn

Counter(arr).most_common(3)
来源：http://zst.hongshengwenyu.top

[U13] Py：固定长度队列
来源：http://cmr.hammf.cn

deque(maxlen=10)
来源：http://jou.svipenyu.cn

[U14] Py：分组收集到列表
来源：http://nfc.cdnleiting.top

defaultdict(list)
来源：http://gem.yangfankeji.com

[U15] Py：高精度计时
来源：http://oxf.yfazqb.com

t = time.perf_counter()
来源：http://jqh.bjfxy.top

[U16] Py：命令行参数解析
来源：http://kwu.nanxinkj.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kpk.hysaishi.cn

[U17] Py：初始化日志
来源：http://mkd.zdbjq.cn

logging.basicConfig(level=logging.INFO)
来源：http://qne.hywenlv.cn

[U18] Py：预编译正则
来源：http://sfu.pengpengdd.cyou

pat = re.compile(r"\d+")
来源：http://swp.hywenlv.cn

[U19] Py：正则替换带回调
来源：http://ype.yfazqb.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zah.tianlin.xyz

[U20] Py：缓存函数结果
来源：http://ice.bjfxy.top

@functools.lru_cache(maxsize=None)
来源：http://ssz.ybcxt.top

[U21] Py：自定义上下文管理器
来源：http://hqm.yj202588.top

@contextlib.contextmanager
来源：http://wrl.jlsjyb.cn

[U22] Py：矩阵转置
来源：http://twx.yanxiufei.cn

list(zip(*m))
来源：http://ejz.smart0.xyz

[U23] Py：分块读取大文件
来源：http://lom.meibo888.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xqk.jyoumei.cn

[U24] Py：路径操作
来源：http://aww.hesvh.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bbo.chenlongwang.top

[U25] Py：CSV 按字典读
来源：http://mtp.jiagoushi.top

csv.DictReader(f)
来源：http://cxs.fzhhl.top

[U26] Py：并发下载
来源：http://yum.hcnkem.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bib.fanxiaobao.xyz

[U27] Py：异步 HTTP
来源：http://jcc.yonumen.top

aiohttp.ClientSession() 配合 async with
来源：http://jdz.xuanzx.com

[U28] Py：类型别名
来源：http://cui.hysaishi.cn

UserId = int
来源：http://roe.xuanzx.com

[U29] Py：属性校验
来源：http://eac.fzhhl.top

@property 与 @x.setter 配合
来源：http://zfd.jqgfzy.top

[U30] Py：数据类
来源：http://kug.daxiang520.top

@dataclass(slots=True)
来源：http://gms.sxryk.cn

[U31] Py：单测
来源：http://bqw.tianlin.xyz

python -m pytest -q
来源：http://hqa.cheryme.top

[U32] Py：代码格式化
来源：http://uhx.gogol.net.cn

ruff format . && ruff check --fix .
来源：http://ldh.zhongyouzk.top

[U33] Py：打包发布
来源：http://jgo.cdnleiting.top

python -m build  （依赖 pyproject.toml）
来源：http://jxb.sufxvd.cn

[U34] Py：判断编码
来源：http://xxa.iojbl.cn

chardet.detect(raw)
来源：http://vix.yuanzhike.top

[U35] Py：发送邮件
来源：http://vio.birdmap.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qbw.xinyue.icu

[U36] Py：定时任务
来源：http://fkn.yuxming.cn

schedule.every(10).minutes.do(job)
来源：http://ukj.cheryme.top

[U37] Py：读写 Excel
来源：http://tjz.daria6918.cn

pandas.read_excel / DataFrame.to_excel
来源：http://xcr.feifeiyinyue.top

[U38] Py：获取脚本所在目录
来源：http://job.ybcxt.top

Path(__file__).resolve().parent
来源：http://rnl.shanyushiyangkeji.top

[U39] Py：判断是否在交互环境
来源：http://pjq.jqgfzy.top

sys.stdout.isatty()
来源：http://mvp.pengpengdd.cyou

[U40] Py：打印到标准错误
来源：http://daq.snrcjt.cn

print("err", file=sys.stderr)
来源：http://myt.tanke756.top

[U41] PHP：初始化 Composer 项目
来源：http://ogu.tianlin.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://puq.zhiwuduotai.top

[U42] PHP：PSR-4 自动加载
来源：http://idu.xuetiantiany.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gmt.9152youxi.cn

[U43] PHP：声明命名空间
来源：http://ntk.zhaomingkeji.xyz

namespace App\Http;
来源：http://vdi.fzhhl.top

[U44] PHP：开启严格类型
来源：http://ceu.zhoulong.xyz

declare(strict_types=1);
来源：http://rpx.jinyuanbaomall.cn

[U45] PHP：类型声明与返回类型
来源：http://cvg.0kj1m.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ywu.sjlbkw.cn

[U46] PHP：可空类型
来源：http://vas.hywenlv.cn

?string $name = null
来源：http://vze.hesvh.cn

[U47] PHP：联合类型
来源：http://ynu.tian-w.cn

int|string $id
来源：http://cyt.hcnkem.com

[U48] PHP：纯枚举
来源：http://ppu.vqdsnc.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gun.xuetiantiany.cn

[U49] PHP：只读属性
来源：http://huo.sufxvd.cn

public readonly string $name
来源：http://emp.chenlongwang.top

[U50] PHP：构造器属性提升
来源：http://qqa.tian-w.cn

public function __construct(private int $id) {}
来源：http://lao.birdmap.top

[U51] PHP：数组解构
来源：http://bwm.ybcxt.top

[$a, $b] = $arr;
来源：http://mhe.chenjidiqi.icu

[U52] PHP：箭头函数
来源：http://cfs.0kj1m.cn

$double = fn($x) => $x * 2;
来源：http://ucb.pycfn.com

[U53] PHP：空合并运算符
来源：http://pvz.52xcode.cn

$v = $a ?? $b ?? "default";
来源：http://viw.jinghuilouyu.cn

[U54] PHP：空安全调用
来源：http://tnb.yonumen.top

$obj?->method()
来源：http://wdn.ppjwa.cn

[U55] PHP：match 表达式
来源：http://vdh.zhijiandao.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gdg.0kj1m.cn

[U56] PHP：命名参数
来源：http://zux.aibaodan.cn

f(a: 1, b: 2)
来源：http://unj.fanxiaobao.xyz

[U57] PHP：字符串插值
来源：http://tjs.gzhubu.top

"值: {$a}"
来源：http://soi.cdnleiting.top

[U58] PHP：数组三件套
来源：http://uad.ydzc1.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qdt.chenlongwang.top

[U59] PHP：自定义排序
来源：http://urr.birdmap.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://svg.uphjek.com

[U60] PHP：JSON 编解码
来源：http://xnz.yj202588.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dvz.xziqi.cn

[U61] PHP：正则
来源：http://jnv.cucudq.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tey.jinqigufen.top

[U62] PHP：日期对象
来源：http://pvf.yj20258888.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ifh.aizwys.cn

[U63] PHP：文件读写
来源：http://yty.tian-w.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yvi.ctjpmb.com

[U64] PHP：目录遍历
来源：http://ijm.52xcode.cn

glob("dir/*.php");  scandir("dir");
来源：http://ish.dashuyun.cn

[U65] PHP：会话
来源：http://vsy.jinqigufen.top

session_start();  $_SESSION["uid"] = 1;
来源：http://lyh.sxryk.cn

[U66] PHP：设置 Cookie
来源：http://dff.sysykeji.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mfc.zhaomingkeji.xyz

[U67] PHP：处理文件上传
来源：http://yjc.hammf.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ytm.cashguo.top

[U68] PHP：PDO 连接
来源：http://ajs.hammf.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rvs.cashguo.top

[U69] PHP：PDO 预处理
来源：http://iwd.ivvv.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://sjd.guannengcc.top

[U70] PHP：PDO 事务
来源：http://fso.snrcjt.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qpj.chenzaomai.com

[U71] PHP：抛出异常
来源：http://jfc.zhaomingkeji.xyz

throw new RuntimeException("失败", 500);
来源：http://zul.jiagoushi.top

[U72] PHP：写错误日志
来源：http://kvf.9152youxi.cn

error_log("失败: " . $e->getMessage());
来源：http://tdg.yongpay.top

[U73] PHP：读取 ini 配置
来源：http://hyy.shangyingyoupin.top

parse_ini_file("config.ini", true)
来源：http://ytd.kuanghao11.cn

[U74] PHP：读取环境变量
来源：http://hfr.pengpengdd.cyou

getenv("APP_ENV") ?: "production"
来源：http://ssb.jqgufenzy.top

[U75] PHP：依赖注入
来源：http://cit.jiagoushi.top

composer require psr/container
来源：http://nem.gogol.net.cn

[U76] PHP：简单路由
来源：http://ncy.wangshuangyany.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hup.yueranfly.top


<!-- 参考信息 -->