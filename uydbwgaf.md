代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mgo.yonumen.top

[S51] C++：显式类型转换
来源：http://gsb.yuxming.cn

static_cast<double>(a) / b
来源：http://hag.fzhhl.top

[S52] C++：const 与 noexcept
来源：http://sbj.fengsongda.top

int size() const noexcept { return n_; }
来源：http://zgk.ctjpmb.com

[S53] C++：移动语义
来源：http://qvk.pycfn.com

std::vector<int> w = std::move(v);
来源：http://dnv.jyoumei.cn

[S54] C++：异常处理
来源：http://fge.0kj1m.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cgx.xingfuxueyuan.xyz

[S55] C++：结构化绑定
来源：http://pva.zhengqikj.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ddk.jyoumei.cn

[S56] C++：optional
来源：http://hth.fzhhl.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hse.shanyushiyangkeji.top

[S57] C++：编译期常量
来源：http://keg.jiagoushi.top

constexpr int N = 10;
来源：http://phz.fehbvm.com

[S58] C++：命名空间
来源：http://wms.guannengcc.top

namespace ns { int f() { return 1; } }
来源：http://cmv.hnxiangtu.top

[S59] C++：静态断言
来源：http://hgp.shzxlz.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nif.316326.xyz

[S60] C++：遍历并删除元素
来源：http://qbm.fzhhl.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ewz.smart0.xyz

================================================================================
来源：http://mom.guannengcc.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jmc.redwolf501.top

================================================================================
来源：http://udb.shangyingyoupin.top

[T01] Kotlin：Hello World
来源：http://xfn.0kj1m.cn

println("Hello")
来源：http://rgs.gogol.net.cn

[T02] Kotlin：变量
来源：http://uud.xinyue.icu

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yey.nanxuanxn.top

[T03] Kotlin：字符串模板
来源：http://wiw.zdbjq.cn

"值: $b"
来源：http://zzr.yj20258.top

[T04] Kotlin：空安全
来源：http://gqq.gotoacloud.top

val n: String? = null;  n?.length
来源：http://raw.cqqwz.cn

[T05] Kotlin：when 表达式
来源：http://vge.ivvv.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dia.fktsv.cn

[T06] Kotlin：集合映射
来源：http://fdw.mhx1999.top

listOf(1, 2, 3).map { it * 2 }
来源：http://hmf.sweek.top

[T07] Kotlin：集合过滤
来源：http://yda.fanxiaobao.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://gry.bbcook.cn

[T08] Kotlin：数据类
来源：http://lpd.yongpay.top

data class User(val name: String, val age: Int)
来源：http://hzf.tianlin.xyz

[T09] Kotlin：扩展函数
来源：http://ocg.wangshuangyany.cn

fun String.exclaim() = this + "!"
来源：http://nfm.jqgfzy.top

[T10] Kotlin：默认参数
来源：http://wwa.zdbjq.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://glz.ydjk.org.cn

[T11] Kotlin：协程
来源：http://via.cucudq.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://aom.xuetiantiany.cn

[T12] Kotlin：解构声明
来源：http://inq.yj20258888.top

val (a, b) = Pair(1, 2)
来源：http://dbf.ybcxt.top

[T13] Kotlin：只读 Map
来源：http://rwn.jqgufenzy.top

val m = mapOf("a" to 1)
来源：http://jnt.sweek.top

[T14] Kotlin：循环
来源：http://his.316326.xyz

for (i in 1..10) println(i)
来源：http://ica.yuxming.cn

[T15] Kotlin：接口
来源：http://xva.cucudq.cn

interface Shape { fun area(): Double }
来源：http://jlr.cheryme.top

[T16] Swift：Hello World
来源：http://siu.zhongyouzk.top

print("Hello")
来源：http://bck.jianghu66.top

[T17] Swift：变量与常量
来源：http://igu.snrcjt.cn

var a = 1;  let b = 2
来源：http://isc.mhx1999.top

[T18] Swift：字符串插值
来源：http://zat.nanxinkj.top

"值: \(b)"
来源：http://mzx.shanyushiyangkeji.top

[T19] Swift：可选绑定
来源：http://mlq.yfazqb.com

if let n = opt { print(n) }
来源：http://euk.havefunace.top

[T20] Swift：数组操作
来源：http://cnh.vqdsnc.cn

var a = [1, 2, 3];  a.append(4)
来源：http://fhh.hnxiangtu.top

[T21] Swift：遍历
来源：http://qnz.wangshuangyany.cn

for x in a { print(x) }
来源：http://nbk.shangyingyoupin.top

[T22] Swift：字典
来源：http://pop.zhongyouzk.top

var d = ["a": 1];  d["b"] = 2
来源：http://gqb.zhijiandao.cn

[T23] Swift：函数
来源：http://vqw.cucudq.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dmm.jinqigfzy.top

[T24] Swift：闭包
来源：http://xqb.zhongyouzk.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://gpl.epnwcf.com

[T25] Swift：结构体
来源：http://dlu.ydzc1.top

struct P { var x: Int }
来源：http://ruq.gogol.net.cn

[T26] Swift：类与重写
来源：http://apk.316326.xyz

class A: Base { override func f() {} }
来源：http://xud.sxryk.cn

[T27] Swift：错误处理
来源：http://klc.shzxlz.cn

do { try f() } catch { print(error) }
来源：http://qzv.fktsv.cn

[T28] Swift：枚举
来源：http://etz.uphjek.com

enum Color { case red, green }
来源：http://fbc.shzxlz.cn

[T29] Swift：guard 提前返回
来源：http://eog.dashuyun.cn

guard let x = opt else { return }
来源：http://tcq.vqdsnc.cn

[T30] Swift：协议
来源：http://ynk.gzhubu.top

protocol Shape { func area() -> Double }
来源：http://pzy.uphjek.com

[T31] Lua：Hello World
来源：http://xpp.ywan-chungtsiang.top

print("Hello")
来源：http://aip.ppjwa.cn

[T32] Lua：局部变量
来源：http://tmp.jiagoushi.top

local a = 1
来源：http://apr.ywan-chungtsiang.top

[T33] Lua：表（数组）
来源：http://alv.redwolf501.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ybl.meibo888.top

[T34] Lua：遍历表
来源：http://ire.gaohongyu789.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ljh.shzxlz.cn

[T35] Lua：字典表
来源：http://dip.yangfankeji.com

local d = { a = 1 };  d.b = 2
来源：http://tos.bbcook.cn

[T36] Lua：函数
来源：http://yfd.jinqigfzy.top

function add(a, b) return a + b end
来源：http://avh.guowangkeji.top

[T37] Lua：字符串拼接
来源：http://bmj.guannengcc.top

"a" .. "b"
来源：http://cun.guowangkeji.top

[T38] Lua：条件
来源：http://pty.bjfxy.top

if x > 0 then print("正") end
来源：http://rxt.jinyuanbaomall.cn

[T39] Lua：模式匹配
来源：http://lyb.yj202588.top

string.find(s, "%d+")
来源：http://pwe.xingfuxueyuan.xyz

[T40] Lua：元表
来源：http://bzw.iojbl.cn

setmetatable({}, { __index = base })
来源：http://vvx.yj20258.top

[T41] Perl：Hello World
来源：http://czr.xingfuxueyuan.xyz

print "Hello\n";
来源：http://bfl.ywan-chungtsiang.top

[T42] Perl：变量类型
来源：http://mde.sufxvd.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://muk.tianlin.xyz

[T43] Perl：字符串插值
来源：http://fsj.svipenyu.cn

"值: $a"
来源：http://osz.gzhubu.top

[T44] Perl：条件
来源：http://gfe.yueranfly.top

if ($a > 0) { print "正"; }
来源：http://gat.jiagoushi.top

[T45] Perl：数组遍历
来源：http://tbh.fktsv.cn

for my $x (@arr) { print $x; }
来源：http://nkm.c1oappe.top

[T46] Perl：哈希操作
来源：http://utg.nanxinkj.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ovf.hnqzz.top

[T47] Perl：正则捕获
来源：http://dvp.jinghuilouyu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://pox.ppjwa.cn

[T48] Perl：正则替换
来源：http://ffh.hnqzz.top

$s =~ s/old/new/g;
来源：http://lsj.fengsongda.top

[T49] Perl：函数
来源：http://ocm.zhongyouzk.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ncl.xingfuxueyuan.xyz

[T50] Perl：逐行读文件
来源：http://mso.jlsjyb.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qyq.yuanzhike.top

while (my $line = <$fh>) { print $line; }
来源：http://lny.shanyushiyangkeji.top

[T51] Scala：Hello World
来源：http://pcs.yuanzhike.top

println("Hello")
来源：http://hmw.meibo888.top

[T52] Scala：变量
来源：http://wal.wangdashe.top

val a = 1;  var b = 2
来源：http://fjz.daria6918.cn

[T53] Scala：字符串插值
来源：http://txs.ydjk.org.cn

s"值: $b"
来源：http://zgq.fzhhl.top

[T54] Scala：集合映射
来源：http://fhw.ybcxt.top

List(1, 2, 3).map(_ * 2)
来源：http://dnc.sjlbkw.cn

[T55] Scala：集合过滤
来源：http://rym.tian-w.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qdu.haohaochexian.top

[T56] Scala：样例类
来源：http://dcz.vqdsnc.cn

case class User(name: String, age: Int)
来源：http://omr.fehbvm.com

[T57] Scala：模式匹配
来源：http://smt.nwbrower.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://fgp.vqdsnc.cn

[T58] Scala：函数定义
来源：http://tnq.gzhubu.top

def add(a: Int, b: Int): Int = a + b
来源：http://vrt.sweek.top

[T59] Scala：循环
来源：http://gue.zhengqikj.top

for (i <- 1 to 10) println(i)
来源：http://xvv.sysykeji.top

[T60] Scala：折叠
来源：http://xlg.jlsjyb.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cpp.cqqwz.cn

================================================================================
来源：http://qqd.cashguo.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://eix.ivvv.top

================================================================================
来源：http://kfo.gogol.net.cn

[U01] Py：创建虚拟环境
来源：http://mru.shanyushiyangtech.top

python -m venv .venv && source .venv/bin/activate
来源：http://jyq.xuetiantiany.cn

[U02] Py：导出 / 安装依赖
来源：http://eah.zhaomingkeji.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bhq.zhixingplan.top

[U03] Py：加载 .env 配置
来源：http://gfz.aibaodan.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://zds.ydzc1.top

[U04] Py：变量调试打印
来源：http://gwt.chenjidiqi.icu

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://irh.iojbl.cn

[U05] Py：列表去重且保序
来源：http://hya.hfpthk.cn

list(dict.fromkeys(arr))
来源：http://kwf.tian-w.cn

[U06] Py：合并两个字典
来源：http://vax.jinqigufen.top

{**a, **b}
来源：http://nsm.tarul.cn

[U07] Py：反转字典键值
来源：http://tzf.jianghu66.top

{v: k for k, v in d.items()}
来源：http://uqg.cucudq.cn

[U08] Py：展平二维列表
来源：http://bul.shangyingyoupin.top

[y for x in nested for y in x]
来源：http://vca.hywenlv.cn

[U09] Py：字典取最大值的键
来源：http://ifg.pycfn.com

max(d, key=d.get)
来源：http://kzv.fanxiaobao.xyz

[U10] Py：按值排序字典
来源：http://hhd.jinqigufen.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ool.sweek.top

[U11] Py：生成器表达式
来源：http://loa.yongpay.top

(x * 2 for x in arr)
来源：http://qrb.feifeiyinyue.top

[U12] Py：取出现最多的 3 个元素
来源：http://pbl.xuetiantiany.cn

Counter(arr).most_common(3)
来源：http://akq.dashuyun.cn

[U13] Py：固定长度队列
来源：http://wpv.bbcook.cn

deque(maxlen=10)
来源：http://amw.yuxming.cn

[U14] Py：分组收集到列表
来源：http://mdj.dianchejie.cn

defaultdict(list)
来源：http://nug.cheryme.top

[U15] Py：高精度计时
来源：http://pra.guowangkeji.top

t = time.perf_counter()
来源：http://mzk.fanxiaobao.xyz

[U16] Py：命令行参数解析
来源：http://mgi.cheryme.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qfi.bbcook.cn

[U17] Py：初始化日志
来源：http://vba.tianlin.xyz

logging.basicConfig(level=logging.INFO)
来源：http://ehu.fehbvm.com

[U18] Py：预编译正则
来源：http://avv.svipenyu.cn

pat = re.compile(r"\d+")
来源：http://ixf.tarul.cn

[U19] Py：正则替换带回调
来源：http://nbj.ctjpmb.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wiq.yueranfly.top

[U20] Py：缓存函数结果
来源：http://tlo.chenlongwang.top

@functools.lru_cache(maxsize=None)
来源：http://ekq.jianghu66.top

[U21] Py：自定义上下文管理器
来源：http://yro.hesvh.cn

@contextlib.contextmanager
来源：http://rvc.zhongyouzk.top

[U22] Py：矩阵转置
来源：http://zka.fengsongda.top

list(zip(*m))
来源：http://cqw.xylfe.cn

[U23] Py：分块读取大文件
来源：http://gxq.fzhhl.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://btk.nanxinkj.top

[U24] Py：路径操作
来源：http://smz.fzhhl.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://udp.gzhubu.top

[U25] Py：CSV 按字典读
来源：http://zyg.hysaishi.cn

csv.DictReader(f)
来源：http://bxj.cdnleiting.top

[U26] Py：并发下载
来源：http://kxc.svipenyu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://var.ppjwa.cn

[U27] Py：异步 HTTP
来源：http://ght.ehwqpu.com

aiohttp.ClientSession() 配合 async with
来源：http://rff.yueranfly.top

[U28] Py：类型别名
来源：http://byh.ppjwa.cn

UserId = int
来源：http://lav.nwbrower.top

[U29] Py：属性校验
来源：http://hbv.yuxming.cn

@property 与 @x.setter 配合
来源：http://fti.redwolf501.top

[U30] Py：数据类
来源：http://fmk.sweek.top

@dataclass(slots=True)
来源：http://vcb.mhx1999.top

[U31] Py：单测
来源：http://ely.yj202588.top

python -m pytest -q
来源：http://ees.xziqi.cn

[U32] Py：代码格式化
来源：http://pok.vehdjk.com

ruff format . && ruff check --fix .
来源：http://ydt.meibo888.top

[U33] Py：打包发布
来源：http://udv.zycfv.cn

python -m build  （依赖 pyproject.toml）
来源：http://bmg.aibaodan.cn

[U34] Py：判断编码
来源：http://fps.nanxinkj.top

chardet.detect(raw)
来源：http://qbc.hongshengwenyu.top

[U35] Py：发送邮件
来源：http://nsb.sufxvd.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nac.cheryme.top

[U36] Py：定时任务
来源：http://wde.chenlongwang.top

schedule.every(10).minutes.do(job)
来源：http://yxs.gaohongyu789.top

[U37] Py：读写 Excel
来源：http://uzw.yfazqb.com

pandas.read_excel / DataFrame.to_excel
来源：http://hhd.ctjpmb.com

[U38] Py：获取脚本所在目录
来源：http://tpw.hesvh.cn

Path(__file__).resolve().parent
来源：http://efu.bbcook.cn

[U39] Py：判断是否在交互环境
来源：http://tht.hammf.cn

sys.stdout.isatty()
来源：http://hpj.hesvh.cn

[U40] Py：打印到标准错误
来源：http://uam.yuanzhike.top

print("err", file=sys.stderr)
来源：http://svi.yonumen.top

[U41] PHP：初始化 Composer 项目
来源：http://yxt.iojbl.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://jmp.zhixingplan.top

[U42] PHP：PSR-4 自动加载
来源：http://veb.pycfn.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dyp.yj20258888.top

[U43] PHP：声明命名空间
来源：http://mos.birdmap.top

namespace App\Http;
来源：http://ilf.jqgfzy.top

[U44] PHP：开启严格类型
来源：http://tpc.yanxiufei.cn

declare(strict_types=1);
来源：http://xqn.9152youxi.cn

[U45] PHP：类型声明与返回类型
来源：http://gnj.yj20258888.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://omq.bjfxy.top

[U46] PHP：可空类型
来源：http://ame.hnxiangtu.top

?string $name = null
来源：http://lkh.sufxvd.cn

[U47] PHP：联合类型
来源：http://viw.chenzaomai.com

int|string $id
来源：http://gyu.ywan-chungtsiang.top

[U48] PHP：纯枚举
来源：http://hwi.pengpengdd.cyou

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hab.snrcjt.cn

[U49] PHP：只读属性
来源：http://jfu.sjlbkw.cn

public readonly string $name
来源：http://rmp.nanxinkj.top

[U50] PHP：构造器属性提升
来源：http://ibc.ehwqpu.com

public function __construct(private int $id) {}
来源：http://lml.xylfe.cn

[U51] PHP：数组解构
来源：http://ngw.guowangkeji.top

[$a, $b] = $arr;
来源：http://nqf.aizwys.cn

[U52] PHP：箭头函数
来源：http://lgu.yueranfly.top

$double = fn($x) => $x * 2;
来源：http://lgk.xuetiantiany.cn

[U53] PHP：空合并运算符
来源：http://umb.redwolf501.top

$v = $a ?? $b ?? "default";
来源：http://ydg.hcnkem.com

[U54] PHP：空安全调用
来源：http://zqi.gzhubu.top

$obj?->method()
来源：http://zsx.yonumen.top

[U55] PHP：match 表达式
来源：http://tbk.shanyushiyangkeji.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vut.xinyue.icu

[U56] PHP：命名参数
来源：http://swj.xuanzx.com

f(a: 1, b: 2)
来源：http://wja.sxryk.cn

[U57] PHP：字符串插值
来源：http://upi.yangfankeji.com

"值: {$a}"
来源：http://ldl.chenzaomai.com

[U58] PHP：数组三件套
来源：http://eyd.hammf.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xgm.cashguo.top

[U59] PHP：自定义排序
来源：http://xnk.andypj.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ofb.yangfankeji.com

[U60] PHP：JSON 编解码
来源：http://ozk.daria6918.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pmu.ctjpmb.com

[U61] PHP：正则
来源：http://dft.shanyushiyangtech.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cjm.hcnkem.com

[U62] PHP：日期对象
来源：http://hqz.chenlongwang.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://kfa.tianlin.xyz

[U63] PHP：文件读写
来源：http://noc.52xcode.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fkh.fehbvm.com

[U64] PHP：目录遍历
来源：http://jcx.redwolf501.top

glob("dir/*.php");  scandir("dir");
来源：http://dvo.jyoumei.cn

[U65] PHP：会话
来源：http://yhe.yj20258888.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ftz.jianghu66.top

[U66] PHP：设置 Cookie
来源：http://rdj.hnxiangtu.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gpu.xuetiantiany.cn

[U67] PHP：处理文件上传
来源：http://mci.dashuyun.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jjy.hfpthk.cn

[U68] PHP：PDO 连接
来源：http://dbc.yfazqb.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://dpy.hysaishi.cn

[U69] PHP：PDO 预处理
来源：http://nxe.bbcook.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://azz.zhongyouzk.top

[U70] PHP：PDO 事务
来源：http://ijs.sjlbkw.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lji.iojbl.cn

[U71] PHP：抛出异常
来源：http://khw.gaohongyu789.top

throw new RuntimeException("失败", 500);
来源：http://mzz.yj202588.top

[U72] PHP：写错误日志
来源：http://bgi.dashuyun.cn

error_log("失败: " . $e->getMessage());
来源：http://zsz.ybcxt.top

[U73] PHP：读取 ini 配置
来源：http://nuv.chenjidiqi.icu

parse_ini_file("config.ini", true)
来源：http://fez.daria6918.cn

[U74] PHP：读取环境变量
来源：http://cqq.redwolf501.top

getenv("APP_ENV") ?: "production"
来源：http://tjk.fehbvm.com

[U75] PHP：依赖注入
来源：http://pxz.gaohongyu789.top

composer require psr/container
来源：http://aks.mhx1999.top

[U76] PHP：简单路由
来源：http://llp.jqgfzy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://umo.zhiwuduotai.top


<!-- 参考信息 -->