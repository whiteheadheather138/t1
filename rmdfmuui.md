代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hni.xuanzx.com

[S51] C++：显式类型转换
来源：http://acc.gzhubu.top

static_cast<double>(a) / b
来源：http://fpw.tian-w.cn

[S52] C++：const 与 noexcept
来源：http://ysv.jqgufenzy.top

int size() const noexcept { return n_; }
来源：http://oxp.yj20258888.top

[S53] C++：移动语义
来源：http://kon.sjlbkw.cn

std::vector<int> w = std::move(v);
来源：http://jbk.gotoacloud.top

[S54] C++：异常处理
来源：http://dgi.shangyingyoupin.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hjq.zhoulong.xyz

[S55] C++：结构化绑定
来源：http://qpl.ywan-chungtsiang.top

auto [a, b] = std::make_pair(1, 2);
来源：http://rjd.ctjpmb.com

[S56] C++：optional
来源：http://see.shuidangran.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hzp.hfpthk.cn

[S57] C++：编译期常量
来源：http://snj.yangfankeji.com

constexpr int N = 10;
来源：http://gej.wangdashe.top

[S58] C++：命名空间
来源：http://xrl.sxryk.cn

namespace ns { int f() { return 1; } }
来源：http://pwf.zhijiandao.cn

[S59] C++：静态断言
来源：http://rvk.sweek.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://krq.bjfxy.top

[S60] C++：遍历并删除元素
来源：http://sff.fehbvm.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vuj.ywan-chungtsiang.top

================================================================================
来源：http://kfg.0kj1m.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jfk.birdmap.top

================================================================================
来源：http://ksr.wangdashe.top

[T01] Kotlin：Hello World
来源：http://jba.fanxiaobao.xyz

println("Hello")
来源：http://eux.havefunace.top

[T02] Kotlin：变量
来源：http://kor.gotoacloud.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zoa.yj20258.top

[T03] Kotlin：字符串模板
来源：http://atb.hnqzz.top

"值: $b"
来源：http://sin.shanyushiyangkeji.top

[T04] Kotlin：空安全
来源：http://jle.wangshuangyany.cn

val n: String? = null;  n?.length
来源：http://ump.chenlongwang.top

[T05] Kotlin：when 表达式
来源：http://fve.cqqwz.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://iwe.ehwqpu.com

[T06] Kotlin：集合映射
来源：http://yyd.hammf.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://jqo.316326.xyz

[T07] Kotlin：集合过滤
来源：http://qvm.ywan-chungtsiang.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://vsp.yangfankeji.com

[T08] Kotlin：数据类
来源：http://evx.shangyingyoupin.top

data class User(val name: String, val age: Int)
来源：http://ddh.xziqi.cn

[T09] Kotlin：扩展函数
来源：http://twu.fktsv.cn

fun String.exclaim() = this + "!"
来源：http://wqr.fehbvm.com

[T10] Kotlin：默认参数
来源：http://oan.haohaochexian.top

fun greet(name: String = "World") = "Hi $name"
来源：http://nfq.zycfv.cn

[T11] Kotlin：协程
来源：http://ktw.zhaomingkeji.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://muq.feifeiyinyue.top

[T12] Kotlin：解构声明
来源：http://qtm.sweek.top

val (a, b) = Pair(1, 2)
来源：http://sis.cucudq.cn

[T13] Kotlin：只读 Map
来源：http://dxo.tanke756.top

val m = mapOf("a" to 1)
来源：http://ily.pengpengdd.cyou

[T14] Kotlin：循环
来源：http://yuv.ivvv.top

for (i in 1..10) println(i)
来源：http://tsf.ppjwa.cn

[T15] Kotlin：接口
来源：http://ufz.zhaomingkeji.xyz

interface Shape { fun area(): Double }
来源：http://qvu.c1oappe.top

[T16] Swift：Hello World
来源：http://hke.cashguo.top

print("Hello")
来源：http://yvo.uphjek.com

[T17] Swift：变量与常量
来源：http://kxu.yj20258888.top

var a = 1;  let b = 2
来源：http://oyc.chenlongwang.top

[T18] Swift：字符串插值
来源：http://xxd.hcnkem.com

"值: \(b)"
来源：http://ody.jinyuanbaomall.cn

[T19] Swift：可选绑定
来源：http://wfs.zycfv.cn

if let n = opt { print(n) }
来源：http://osc.cucudq.cn

[T20] Swift：数组操作
来源：http://umf.chenzaomai.com

var a = [1, 2, 3];  a.append(4)
来源：http://gxl.chenjidiqi.icu

[T21] Swift：遍历
来源：http://zeu.zhijiandao.cn

for x in a { print(x) }
来源：http://dxu.haohaochexian.top

[T22] Swift：字典
来源：http://mlg.jlsjyb.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fyy.ivvv.top

[T23] Swift：函数
来源：http://vqo.hywenlv.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yqi.jianghu66.top

[T24] Swift：闭包
来源：http://ciq.ywan-chungtsiang.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://kwy.svipenyu.cn

[T25] Swift：结构体
来源：http://qzq.0kj1m.cn

struct P { var x: Int }
来源：http://wid.xylfe.cn

[T26] Swift：类与重写
来源：http://eel.hnxiangtu.top

class A: Base { override func f() {} }
来源：http://lel.svipenyu.cn

[T27] Swift：错误处理
来源：http://kfa.hnqzz.top

do { try f() } catch { print(error) }
来源：http://wue.jianghu66.top

[T28] Swift：枚举
来源：http://atm.c1oappe.top

enum Color { case red, green }
来源：http://hbp.yj202588.top

[T29] Swift：guard 提前返回
来源：http://dku.guowangkeji.top

guard let x = opt else { return }
来源：http://qam.zhengqikj.top

[T30] Swift：协议
来源：http://pfa.yangfankeji.com

protocol Shape { func area() -> Double }
来源：http://wbo.xylfe.cn

[T31] Lua：Hello World
来源：http://pyz.zhoulong.xyz

print("Hello")
来源：http://ofs.cqqwz.cn

[T32] Lua：局部变量
来源：http://udm.andypj.xyz

local a = 1
来源：http://ego.jyoumei.cn

[T33] Lua：表（数组）
来源：http://fxp.ywan-chungtsiang.top

local t = {1, 2, 3};  t[4] = 4
来源：http://wvz.xingfuxueyuan.xyz

[T34] Lua：遍历表
来源：http://vlf.hnqzz.top

for i, v in ipairs(t) do print(i, v) end
来源：http://pqc.cdnleiting.top

[T35] Lua：字典表
来源：http://amx.jinqigufen.top

local d = { a = 1 };  d.b = 2
来源：http://wqx.yonumen.top

[T36] Lua：函数
来源：http://nem.zhengqikj.top

function add(a, b) return a + b end
来源：http://lbl.jlsjyb.cn

[T37] Lua：字符串拼接
来源：http://her.hysaishi.cn

"a" .. "b"
来源：http://onu.tanke756.top

[T38] Lua：条件
来源：http://rsl.nanxinkj.top

if x > 0 then print("正") end
来源：http://vrh.epnwcf.com

[T39] Lua：模式匹配
来源：http://pec.smart0.xyz

string.find(s, "%d+")
来源：http://oec.yangfankeji.com

[T40] Lua：元表
来源：http://peh.c1oappe.top

setmetatable({}, { __index = base })
来源：http://msd.gzhubu.top

[T41] Perl：Hello World
来源：http://mjl.yj20258888.top

print "Hello\n";
来源：http://sqw.xuanzx.com

[T42] Perl：变量类型
来源：http://sya.chenjidiqi.icu

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qit.hywenlv.cn

[T43] Perl：字符串插值
来源：http://xag.xingfuxueyuan.xyz

"值: $a"
来源：http://awv.shanyushiyangkeji.top

[T44] Perl：条件
来源：http://lwj.jinqigufen.top

if ($a > 0) { print "正"; }
来源：http://eko.zhongyouzk.top

[T45] Perl：数组遍历
来源：http://szs.yj20258.top

for my $x (@arr) { print $x; }
来源：http://mno.0kj1m.cn

[T46] Perl：哈希操作
来源：http://ege.feifeiyinyue.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://uoo.nanxuanxn.top

[T47] Perl：正则捕获
来源：http://jxr.xziqi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://qff.cqqwz.cn

[T48] Perl：正则替换
来源：http://elz.nanxinkj.top

$s =~ s/old/new/g;
来源：http://oup.zdbjq.cn

[T49] Perl：函数
来源：http://fob.xingfuxueyuan.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://bwe.zycfv.cn

[T50] Perl：逐行读文件
来源：http://sql.xinyue.icu

open my $fh, "<", "a.txt" or die $!;
来源：http://jde.xuanzx.com

while (my $line = <$fh>) { print $line; }
来源：http://yvb.hongshengwenyu.top

[T51] Scala：Hello World
来源：http://wym.hammf.cn

println("Hello")
来源：http://lms.yuxming.cn

[T52] Scala：变量
来源：http://row.vehdjk.com

val a = 1;  var b = 2
来源：http://vkw.ivvv.top

[T53] Scala：字符串插值
来源：http://tsn.andypj.xyz

s"值: $b"
来源：http://qqh.fengsongda.top

[T54] Scala：集合映射
来源：http://drs.zhixingplan.top

List(1, 2, 3).map(_ * 2)
来源：http://ojp.zhongyouzk.top

[T55] Scala：集合过滤
来源：http://day.yongpay.top

List(1, 2, 3).filter(_ > 1)
来源：http://zpu.hywenlv.cn

[T56] Scala：样例类
来源：http://xqo.yanxiufei.cn

case class User(name: String, age: Int)
来源：http://fcl.c1oappe.top

[T57] Scala：模式匹配
来源：http://wjb.chenlongwang.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://lnz.chenzaomai.com

[T58] Scala：函数定义
来源：http://qbf.cashguo.top

def add(a: Int, b: Int): Int = a + b
来源：http://ctk.snrcjt.cn

[T59] Scala：循环
来源：http://gca.xuanzx.com

for (i <- 1 to 10) println(i)
来源：http://jch.zhongyouzk.top

[T60] Scala：折叠
来源：http://rqt.yvedp.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gzw.havefunace.top

================================================================================
来源：http://jrc.yvedp.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vng.ctjpmb.com

================================================================================
来源：http://jei.fengsongda.top

[U01] Py：创建虚拟环境
来源：http://tkd.nwbrower.top

python -m venv .venv && source .venv/bin/activate
来源：http://mrh.havefunace.top

[U02] Py：导出 / 安装依赖
来源：http://fxv.yongpay.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://caq.yj202588.top

[U03] Py：加载 .env 配置
来源：http://fnl.gogol.net.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ync.sufxvd.cn

[U04] Py：变量调试打印
来源：http://ccb.c1oappe.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wdf.fengsongda.top

[U05] Py：列表去重且保序
来源：http://vyz.yongpay.top

list(dict.fromkeys(arr))
来源：http://gmg.aizwys.cn

[U06] Py：合并两个字典
来源：http://zpu.cucudq.cn

{**a, **b}
来源：http://hin.52xcode.cn

[U07] Py：反转字典键值
来源：http://fyq.ivvv.top

{v: k for k, v in d.items()}
来源：http://xtc.0kj1m.cn

[U08] Py：展平二维列表
来源：http://glx.fanxiaobao.xyz

[y for x in nested for y in x]
来源：http://ufy.jiagoushi.top

[U09] Py：字典取最大值的键
来源：http://fdj.xingfuxueyuan.xyz

max(d, key=d.get)
来源：http://knv.hfpthk.cn

[U10] Py：按值排序字典
来源：http://prd.jinqigufen.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zlj.zdqjudy.top

[U11] Py：生成器表达式
来源：http://swz.sjlbkw.cn

(x * 2 for x in arr)
来源：http://opi.bjfxy.top

[U12] Py：取出现最多的 3 个元素
来源：http://rwg.jqgufenzy.top

Counter(arr).most_common(3)
来源：http://cpx.ctjpmb.com

[U13] Py：固定长度队列
来源：http://vqr.tanke756.top

deque(maxlen=10)
来源：http://lsk.andypj.xyz

[U14] Py：分组收集到列表
来源：http://vdv.aibaodan.cn

defaultdict(list)
来源：http://soo.zhaomingkeji.xyz

[U15] Py：高精度计时
来源：http://wuv.fktsv.cn

t = time.perf_counter()
来源：http://dzh.hammf.cn

[U16] Py：命令行参数解析
来源：http://gfj.aizwys.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://boo.cqqwz.cn

[U17] Py：初始化日志
来源：http://por.cashguo.top

logging.basicConfig(level=logging.INFO)
来源：http://lxq.xinyue.icu

[U18] Py：预编译正则
来源：http://ilt.ppjwa.cn

pat = re.compile(r"\d+")
来源：http://dmx.snrcjt.cn

[U19] Py：正则替换带回调
来源：http://pfx.quarkkingdee.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kon.gotoacloud.top

[U20] Py：缓存函数结果
来源：http://fhq.mhx1999.top

@functools.lru_cache(maxsize=None)
来源：http://wvz.iojbl.cn

[U21] Py：自定义上下文管理器
来源：http://jnu.xziqi.cn

@contextlib.contextmanager
来源：http://zre.hnxiangtu.top

[U22] Py：矩阵转置
来源：http://zgp.nanxinkj.top

list(zip(*m))
来源：http://ndq.zhoulong.xyz

[U23] Py：分块读取大文件
来源：http://igv.shanyushiyangkeji.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wit.jqgfzy.top

[U24] Py：路径操作
来源：http://uwe.vehdjk.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qam.hfpthk.cn

[U25] Py：CSV 按字典读
来源：http://myd.jqgufenzy.top

csv.DictReader(f)
来源：http://sjo.fktsv.cn

[U26] Py：并发下载
来源：http://vbe.andypj.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yzo.nwbrower.top

[U27] Py：异步 HTTP
来源：http://uou.zhaomingkeji.xyz

aiohttp.ClientSession() 配合 async with
来源：http://epa.52xcode.cn

[U28] Py：类型别名
来源：http://cim.vehdjk.com

UserId = int
来源：http://phg.ppjwa.cn

[U29] Py：属性校验
来源：http://nrw.shanyushiyangkeji.top

@property 与 @x.setter 配合
来源：http://rvg.smart0.xyz

[U30] Py：数据类
来源：http://uce.hesvh.cn

@dataclass(slots=True)
来源：http://nhc.fehbvm.com

[U31] Py：单测
来源：http://zwv.jiagoushi.top

python -m pytest -q
来源：http://lfz.yj20258888.top

[U32] Py：代码格式化
来源：http://jcm.fktsv.cn

ruff format . && ruff check --fix .
来源：http://bks.smart0.xyz

[U33] Py：打包发布
来源：http://fje.ppjwa.cn

python -m build  （依赖 pyproject.toml）
来源：http://zsu.nanxinkj.top

[U34] Py：判断编码
来源：http://pcx.jqgfzy.top

chardet.detect(raw)
来源：http://zdm.hcnkem.com

[U35] Py：发送邮件
来源：http://zqi.yj20258.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bzl.guannengcc.top

[U36] Py：定时任务
来源：http://bvc.guannengcc.top

schedule.every(10).minutes.do(job)
来源：http://skk.ppjwa.cn

[U37] Py：读写 Excel
来源：http://rwx.sufxvd.cn

pandas.read_excel / DataFrame.to_excel
来源：http://iim.pycfn.com

[U38] Py：获取脚本所在目录
来源：http://igu.fktsv.cn

Path(__file__).resolve().parent
来源：http://fjf.fzhhl.top

[U39] Py：判断是否在交互环境
来源：http://cgd.hysaishi.cn

sys.stdout.isatty()
来源：http://uvu.shanyushiyangtech.top

[U40] Py：打印到标准错误
来源：http://kdq.jyoumei.cn

print("err", file=sys.stderr)
来源：http://ait.daxiang520.top

[U41] PHP：初始化 Composer 项目
来源：http://gju.gogol.net.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://fkf.chenjidiqi.icu

[U42] PHP：PSR-4 自动加载
来源：http://omz.svipenyu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://uki.daria6918.cn

[U43] PHP：声明命名空间
来源：http://juk.cheryme.top

namespace App\Http;
来源：http://qxx.jinqigufen.top

[U44] PHP：开启严格类型
来源：http://mfa.tarul.cn

declare(strict_types=1);
来源：http://ouv.jyoumei.cn

[U45] PHP：类型声明与返回类型
来源：http://pjf.yvedp.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://mvt.xuanzx.com

[U46] PHP：可空类型
来源：http://rtk.zhengqikj.top

?string $name = null
来源：http://trg.pengpengdd.cyou

[U47] PHP：联合类型
来源：http://sgv.aibaodan.cn

int|string $id
来源：http://lvf.shzxlz.cn

[U48] PHP：纯枚举
来源：http://xky.zhixingplan.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://pla.daria6918.cn

[U49] PHP：只读属性
来源：http://tyg.zhengqikj.top

public readonly string $name
来源：http://hdv.hammf.cn

[U50] PHP：构造器属性提升
来源：http://ysb.zhixingplan.top

public function __construct(private int $id) {}
来源：http://dvq.ehwqpu.com

[U51] PHP：数组解构
来源：http://vcq.ehwqpu.com

[$a, $b] = $arr;
来源：http://vft.jianghu66.top

[U52] PHP：箭头函数
来源：http://nwn.sjlbkw.cn

$double = fn($x) => $x * 2;
来源：http://jzc.jianghu66.top

[U53] PHP：空合并运算符
来源：http://bwy.316326.xyz

$v = $a ?? $b ?? "default";
来源：http://gfi.zhoulong.xyz

[U54] PHP：空安全调用
来源：http://qkg.zhixingplan.top

$obj?->method()
来源：http://bfg.cashguo.top

[U55] PHP：match 表达式
来源：http://cwd.epnwcf.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bnv.feifeiyinyue.top

[U56] PHP：命名参数
来源：http://idt.jianghu66.top

f(a: 1, b: 2)
来源：http://chf.birdmap.top

[U57] PHP：字符串插值
来源：http://tfa.nanxinkj.top

"值: {$a}"
来源：http://yhl.aizwys.cn

[U58] PHP：数组三件套
来源：http://ntf.mhx1999.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ijn.jqgfzy.top

[U59] PHP：自定义排序
来源：http://jhe.zycfv.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qfe.ehwqpu.com

[U60] PHP：JSON 编解码
来源：http://ojz.316326.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wrp.chenlongwang.top

[U61] PHP：正则
来源：http://bkt.shanyushiyangtech.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://yjz.nanxuanxn.top

[U62] PHP：日期对象
来源：http://wzu.hysaishi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pad.yvedp.cn

[U63] PHP：文件读写
来源：http://gfx.zycfv.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hhf.jinqigufen.top

[U64] PHP：目录遍历
来源：http://vdf.vqdsnc.cn

glob("dir/*.php");  scandir("dir");
来源：http://rcs.yj20258.top

[U65] PHP：会话
来源：http://dvp.52xcode.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://bth.bbcook.cn

[U66] PHP：设置 Cookie
来源：http://xho.ehwqpu.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://tuq.jinghuilouyu.cn

[U67] PHP：处理文件上传
来源：http://lgh.yuxming.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kui.hysaishi.cn

[U68] PHP：PDO 连接
来源：http://jny.fzhhl.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ffi.fanxiaobao.xyz

[U69] PHP：PDO 预处理
来源：http://lkh.redwolf501.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gxs.pycfn.com

[U70] PHP：PDO 事务
来源：http://vwm.52xcode.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pbs.0kj1m.cn

[U71] PHP：抛出异常
来源：http://ajd.andypj.xyz

throw new RuntimeException("失败", 500);
来源：http://lax.zdbjq.cn

[U72] PHP：写错误日志
来源：http://kep.ivvv.top

error_log("失败: " . $e->getMessage());
来源：http://cln.yonumen.top

[U73] PHP：读取 ini 配置
来源：http://sdh.shanyushiyangtech.top

parse_ini_file("config.ini", true)
来源：http://iyj.wangshuangyany.cn

[U74] PHP：读取环境变量
来源：http://vol.epnwcf.com

getenv("APP_ENV") ?: "production"
来源：http://inn.xuetiantiany.cn

[U75] PHP：依赖注入
来源：http://ffc.epnwcf.com

composer require psr/container
来源：http://cky.0kj1m.cn

[U76] PHP：简单路由
来源：http://vde.redwolf501.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zax.wangdashe.top


<!-- 参考信息 -->