代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tgu.zycfv.cn

[S57] C++：编译期常量
来源：http://nie.jyoumei.cn

constexpr int N = 10;
来源：http://tpp.shuidangran.top

[S58] C++：命名空间
来源：http://gdm.316326.xyz

namespace ns { int f() { return 1; } }
来源：http://hgy.sysykeji.top

[S59] C++：静态断言
来源：http://nde.ctjpmb.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://prj.jinqigufen.top

[S60] C++：遍历并删除元素
来源：http://ehu.yuxming.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fsb.zycfv.cn

================================================================================
来源：http://epy.ydzc1.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://usn.xinyue.icu

================================================================================
来源：http://xla.yanxiufei.cn

[T01] Kotlin：Hello World
来源：http://kmc.fanxiaobao.xyz

println("Hello")
来源：http://xmg.wangshuangyany.cn

[T02] Kotlin：变量
来源：http://jds.xziqi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kvj.jqgfzy.top

[T03] Kotlin：字符串模板
来源：http://fow.sweek.top

"值: $b"
来源：http://tgg.guowangkeji.top

[T04] Kotlin：空安全
来源：http://qma.yj202588.top

val n: String? = null;  n?.length
来源：http://oxh.cashguo.top

[T05] Kotlin：when 表达式
来源：http://jeb.shanyushiyangkeji.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xeh.yvedp.cn

[T06] Kotlin：集合映射
来源：http://hjm.ydjk.org.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://zde.hammf.cn

[T07] Kotlin：集合过滤
来源：http://ena.hongshengwenyu.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://fyq.quarkkingdee.top

[T08] Kotlin：数据类
来源：http://mmr.hnqzz.top

data class User(val name: String, val age: Int)
来源：http://ach.aibaodan.cn

[T09] Kotlin：扩展函数
来源：http://gcg.pycfn.com

fun String.exclaim() = this + "!"
来源：http://ycf.chenzaomai.com

[T10] Kotlin：默认参数
来源：http://swd.xingfuxueyuan.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://dwc.cheryme.top

[T11] Kotlin：协程
来源：http://bxt.cashguo.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://gcc.tarul.cn

[T12] Kotlin：解构声明
来源：http://aeh.jiagoushi.top

val (a, b) = Pair(1, 2)
来源：http://nqq.dashuyun.cn

[T13] Kotlin：只读 Map
来源：http://rav.shangyingyoupin.top

val m = mapOf("a" to 1)
来源：http://vyc.vqdsnc.cn

[T14] Kotlin：循环
来源：http://buh.ehwqpu.com

for (i in 1..10) println(i)
来源：http://xcj.jinyuanbaomall.cn

[T15] Kotlin：接口
来源：http://kjh.yanxiufei.cn

interface Shape { fun area(): Double }
来源：http://smd.9152youxi.cn

[T16] Swift：Hello World
来源：http://hzw.xuanzx.com

print("Hello")
来源：http://waq.fktsv.cn

[T17] Swift：变量与常量
来源：http://yxd.ydjk.org.cn

var a = 1;  let b = 2
来源：http://fip.sjlbkw.cn

[T18] Swift：字符串插值
来源：http://fng.yfazqb.com

"值: \(b)"
来源：http://nsr.yueranfly.top

[T19] Swift：可选绑定
来源：http://hzt.yangfankeji.com

if let n = opt { print(n) }
来源：http://czs.pengpengdd.cyou

[T20] Swift：数组操作
来源：http://iks.hcnkem.com

var a = [1, 2, 3];  a.append(4)
来源：http://cdi.tianlin.xyz

[T21] Swift：遍历
来源：http://nsv.jianghu66.top

for x in a { print(x) }
来源：http://idp.pengpengdd.cyou

[T22] Swift：字典
来源：http://goi.hysaishi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ssj.tarul.cn

[T23] Swift：函数
来源：http://ujo.birdmap.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dzn.tian-w.cn

[T24] Swift：闭包
来源：http://kcr.xingfuxueyuan.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://dos.0kj1m.cn

[T25] Swift：结构体
来源：http://bgs.tianlin.xyz

struct P { var x: Int }
来源：http://jmr.hysaishi.cn

[T26] Swift：类与重写
来源：http://wuc.fengsongda.top

class A: Base { override func f() {} }
来源：http://guc.hnxiangtu.top

[T27] Swift：错误处理
来源：http://qvp.ydjk.org.cn

do { try f() } catch { print(error) }
来源：http://sba.zhoulong.xyz

[T28] Swift：枚举
来源：http://xnx.yj20258888.top

enum Color { case red, green }
来源：http://zaj.yfazqb.com

[T29] Swift：guard 提前返回
来源：http://vzd.yangfankeji.com

guard let x = opt else { return }
来源：http://aex.yanxiufei.cn

[T30] Swift：协议
来源：http://ike.shanyushiyangkeji.top

protocol Shape { func area() -> Double }
来源：http://hio.yvedp.cn

[T31] Lua：Hello World
来源：http://wek.yfazqb.com

print("Hello")
来源：http://frw.gotoacloud.top

[T32] Lua：局部变量
来源：http://khn.jlsjyb.cn

local a = 1
来源：http://ejw.andypj.xyz

[T33] Lua：表（数组）
来源：http://dxs.shuidangran.top

local t = {1, 2, 3};  t[4] = 4
来源：http://kjj.ybcxt.top

[T34] Lua：遍历表
来源：http://yth.sweek.top

for i, v in ipairs(t) do print(i, v) end
来源：http://rzb.nanxuanxn.top

[T35] Lua：字典表
来源：http://jyh.uphjek.com

local d = { a = 1 };  d.b = 2
来源：http://vhe.gaohongyu789.top

[T36] Lua：函数
来源：http://pym.jinghuilouyu.cn

function add(a, b) return a + b end
来源：http://jwq.yj202588.top

[T37] Lua：字符串拼接
来源：http://zyo.daria6918.cn

"a" .. "b"
来源：http://zuf.fehbvm.com

[T38] Lua：条件
来源：http://wcp.zhongyouzk.top

if x > 0 then print("正") end
来源：http://dsd.yj202588.top

[T39] Lua：模式匹配
来源：http://bsa.jiagoushi.top

string.find(s, "%d+")
来源：http://wxf.zhijiandao.cn

[T40] Lua：元表
来源：http://csy.pycfn.com

setmetatable({}, { __index = base })
来源：http://tfs.52xcode.cn

[T41] Perl：Hello World
来源：http://cwe.chenjidiqi.icu

print "Hello\n";
来源：http://obd.yuxming.cn

[T42] Perl：变量类型
来源：http://ywc.zhengqikj.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jsk.wangshuangyany.cn

[T43] Perl：字符串插值
来源：http://vty.yuxming.cn

"值: $a"
来源：http://bag.zdqjudy.top

[T44] Perl：条件
来源：http://vyv.jinqigufen.top

if ($a > 0) { print "正"; }
来源：http://fku.zhaomingkeji.xyz

[T45] Perl：数组遍历
来源：http://oss.ctjpmb.com

for my $x (@arr) { print $x; }
来源：http://ueb.yj20258.top

[T46] Perl：哈希操作
来源：http://pbb.yueranfly.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lwt.ybcxt.top

[T47] Perl：正则捕获
来源：http://mkl.tanke756.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://phl.haohaochexian.top

[T48] Perl：正则替换
来源：http://rau.yangfankeji.com

$s =~ s/old/new/g;
来源：http://dxy.zhixingplan.top

[T49] Perl：函数
来源：http://nte.zhiwuduotai.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xdv.fanxiaobao.xyz

[T50] Perl：逐行读文件
来源：http://vjr.cashguo.top

open my $fh, "<", "a.txt" or die $!;
来源：http://zmr.daria6918.cn

while (my $line = <$fh>) { print $line; }
来源：http://djs.yangfankeji.com

[T51] Scala：Hello World
来源：http://brb.sjlbkw.cn

println("Hello")
来源：http://xoa.hfpthk.cn

[T52] Scala：变量
来源：http://jfq.chenlongwang.top

val a = 1;  var b = 2
来源：http://pri.uphjek.com

[T53] Scala：字符串插值
来源：http://ppo.andypj.xyz

s"值: $b"
来源：http://ple.chenzaomai.com

[T54] Scala：集合映射
来源：http://muf.vehdjk.com

List(1, 2, 3).map(_ * 2)
来源：http://mpo.hfpthk.cn

[T55] Scala：集合过滤
来源：http://vln.zhiwuduotai.top

List(1, 2, 3).filter(_ > 1)
来源：http://oqr.52xcode.cn

[T56] Scala：样例类
来源：http://wqv.xuanzx.com

case class User(name: String, age: Int)
来源：http://euw.ppjwa.cn

[T57] Scala：模式匹配
来源：http://yzh.yueranfly.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://zsb.sxryk.cn

[T58] Scala：函数定义
来源：http://okg.0kj1m.cn

def add(a: Int, b: Int): Int = a + b
来源：http://buv.zhaomingkeji.xyz

[T59] Scala：循环
来源：http://ckc.gotoacloud.top

for (i <- 1 to 10) println(i)
来源：http://yuu.mhx1999.top

[T60] Scala：折叠
来源：http://vue.smart0.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://eag.yanxiufei.cn

================================================================================
来源：http://tti.c1oappe.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xzr.xziqi.cn

================================================================================
来源：http://lvt.dashuyun.cn

[U01] Py：创建虚拟环境
来源：http://afd.shzxlz.cn

python -m venv .venv && source .venv/bin/activate
来源：http://gkx.feifeiyinyue.top

[U02] Py：导出 / 安装依赖
来源：http://xkf.daxiang520.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cgp.bjfxy.top

[U03] Py：加载 .env 配置
来源：http://dpn.guannengcc.top

from dotenv import load_dotenv; load_dotenv()
来源：http://adz.shanyushiyangkeji.top

[U04] Py：变量调试打印
来源：http://ugw.yuanzhike.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://eyy.shuidangran.top

[U05] Py：列表去重且保序
来源：http://awr.shangyingyoupin.top

list(dict.fromkeys(arr))
来源：http://ens.hnqzz.top

[U06] Py：合并两个字典
来源：http://xrm.jinghuilouyu.cn

{**a, **b}
来源：http://jxt.pycfn.com

[U07] Py：反转字典键值
来源：http://ugt.jqgfzy.top

{v: k for k, v in d.items()}
来源：http://wku.daria6918.cn

[U08] Py：展平二维列表
来源：http://blv.jinqigfzy.top

[y for x in nested for y in x]
来源：http://zua.tarul.cn

[U09] Py：字典取最大值的键
来源：http://bhl.nanxinkj.top

max(d, key=d.get)
来源：http://ppu.kuanghao11.cn

[U10] Py：按值排序字典
来源：http://elz.sweek.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jox.c1oappe.top

[U11] Py：生成器表达式
来源：http://xqw.pengpengdd.cyou

(x * 2 for x in arr)
来源：http://wwj.shuidangran.top

[U12] Py：取出现最多的 3 个元素
来源：http://blp.ivvv.top

Counter(arr).most_common(3)
来源：http://fan.pycfn.com

[U13] Py：固定长度队列
来源：http://cxk.sysykeji.top

deque(maxlen=10)
来源：http://otx.daxiang520.top

[U14] Py：分组收集到列表
来源：http://ffe.zycfv.cn

defaultdict(list)
来源：http://mbd.cashguo.top

[U15] Py：高精度计时
来源：http://dwx.zdbjq.cn

t = time.perf_counter()
来源：http://jtd.52xcode.cn

[U16] Py：命令行参数解析
来源：http://hui.jqgfzy.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bfg.jianghu66.top

[U17] Py：初始化日志
来源：http://pcx.chenlongwang.top

logging.basicConfig(level=logging.INFO)
来源：http://szx.zhoulong.xyz

[U18] Py：预编译正则
来源：http://www.vqdsnc.cn

pat = re.compile(r"\d+")
来源：http://hzh.xingfuxueyuan.xyz

[U19] Py：正则替换带回调
来源：http://fwp.jqgufenzy.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jlq.birdmap.top

[U20] Py：缓存函数结果
来源：http://hff.zhijiandao.cn

@functools.lru_cache(maxsize=None)
来源：http://dpg.yj20258888.top

[U21] Py：自定义上下文管理器
来源：http://sbo.yuanzhike.top

@contextlib.contextmanager
来源：http://zyo.guowangkeji.top

[U22] Py：矩阵转置
来源：http://svf.hfpthk.cn

list(zip(*m))
来源：http://hsi.zycfv.cn

[U23] Py：分块读取大文件
来源：http://xrw.gzhubu.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dvi.yongpay.top

[U24] Py：路径操作
来源：http://mps.hesvh.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ztg.ydjk.org.cn

[U25] Py：CSV 按字典读
来源：http://jvf.hongshengwenyu.top

csv.DictReader(f)
来源：http://zmw.tarul.cn

[U26] Py：并发下载
来源：http://xhy.xinyue.icu

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://joq.jiagoushi.top

[U27] Py：异步 HTTP
来源：http://vyd.pengpengdd.cyou

aiohttp.ClientSession() 配合 async with
来源：http://mxj.zhiwuduotai.top

[U28] Py：类型别名
来源：http://slt.zdqjudy.top

UserId = int
来源：http://qaw.jlsjyb.cn

[U29] Py：属性校验
来源：http://smm.shanyushiyangtech.top

@property 与 @x.setter 配合
来源：http://qcz.iojbl.cn

[U30] Py：数据类
来源：http://gue.zhaomingkeji.xyz

@dataclass(slots=True)
来源：http://fsw.yueranfly.top

[U31] Py：单测
来源：http://hdq.snrcjt.cn

python -m pytest -q
来源：http://tfn.zdbjq.cn

[U32] Py：代码格式化
来源：http://ksd.ydjk.org.cn

ruff format . && ruff check --fix .
来源：http://tsn.gzhubu.top

[U33] Py：打包发布
来源：http://axn.cashguo.top

python -m build  （依赖 pyproject.toml）
来源：http://ffp.52xcode.cn

[U34] Py：判断编码
来源：http://zxr.ybcxt.top

chardet.detect(raw)
来源：http://ikd.jinghuilouyu.cn

[U35] Py：发送邮件
来源：http://fra.vehdjk.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ipm.shanyushiyangkeji.top

[U36] Py：定时任务
来源：http://xxq.nwbrower.top

schedule.every(10).minutes.do(job)
来源：http://xso.hnqzz.top

[U37] Py：读写 Excel
来源：http://uvm.xuetiantiany.cn

pandas.read_excel / DataFrame.to_excel
来源：http://xws.birdmap.top

[U38] Py：获取脚本所在目录
来源：http://wyi.chenlongwang.top

Path(__file__).resolve().parent
来源：http://wzt.yonumen.top

[U39] Py：判断是否在交互环境
来源：http://aoa.cheryme.top

sys.stdout.isatty()
来源：http://cqv.ppjwa.cn

[U40] Py：打印到标准错误
来源：http://pzw.fzhhl.top

print("err", file=sys.stderr)
来源：http://jza.bbcook.cn

[U41] PHP：初始化 Composer 项目
来源：http://tyu.yj20258888.top

composer init;  composer require guzzlehttp/guzzle
来源：http://pwt.yj202588.top

[U42] PHP：PSR-4 自动加载
来源：http://lda.gotoacloud.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://edl.wangdashe.top

[U43] PHP：声明命名空间
来源：http://cnc.cheryme.top

namespace App\Http;
来源：http://ybn.shuidangran.top

[U44] PHP：开启严格类型
来源：http://sad.jinqigfzy.top

declare(strict_types=1);
来源：http://dcq.zhongyouzk.top

[U45] PHP：类型声明与返回类型
来源：http://jil.pycfn.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://mzq.vehdjk.com

[U46] PHP：可空类型
来源：http://pqj.hcnkem.com

?string $name = null
来源：http://rbd.sweek.top

[U47] PHP：联合类型
来源：http://api.gogol.net.cn

int|string $id
来源：http://ygp.birdmap.top

[U48] PHP：纯枚举
来源：http://fcu.havefunace.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tpx.nanxinkj.top

[U49] PHP：只读属性
来源：http://ylg.zdbjq.cn

public readonly string $name
来源：http://hwg.jinghuilouyu.cn

[U50] PHP：构造器属性提升
来源：http://agh.svipenyu.cn

public function __construct(private int $id) {}
来源：http://lyv.sxryk.cn

[U51] PHP：数组解构
来源：http://kxd.quarkkingdee.top

[$a, $b] = $arr;
来源：http://wcj.meibo888.top

[U52] PHP：箭头函数
来源：http://fjl.ydjk.org.cn

$double = fn($x) => $x * 2;
来源：http://yzi.shanyushiyangtech.top

[U53] PHP：空合并运算符
来源：http://bhi.vqdsnc.cn

$v = $a ?? $b ?? "default";
来源：http://usc.xuetiantiany.cn

[U54] PHP：空安全调用
来源：http://ahi.gaohongyu789.top

$obj?->method()
来源：http://nas.guowangkeji.top

[U55] PHP：match 表达式
来源：http://wui.havefunace.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://oxb.hammf.cn

[U56] PHP：命名参数
来源：http://mck.svipenyu.cn

f(a: 1, b: 2)
来源：http://jax.zycfv.cn

[U57] PHP：字符串插值
来源：http://wrg.ydjk.org.cn

"值: {$a}"
来源：http://smm.tian-w.cn

[U58] PHP：数组三件套
来源：http://oun.svipenyu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fxw.hywenlv.cn

[U59] PHP：自定义排序
来源：http://zmx.wangdashe.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kkn.jyoumei.cn

[U60] PHP：JSON 编解码
来源：http://tls.yueranfly.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hxk.ppjwa.cn

[U61] PHP：正则
来源：http://cup.jqgfzy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fpx.dianchejie.cn

[U62] PHP：日期对象
来源：http://wwh.sufxvd.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://cqa.vqdsnc.cn

[U63] PHP：文件读写
来源：http://lto.hnxiangtu.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xkl.shuidangran.top

[U64] PHP：目录遍历
来源：http://jvi.hnqzz.top

glob("dir/*.php");  scandir("dir");
来源：http://kjg.epnwcf.com

[U65] PHP：会话
来源：http://kym.gogol.net.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://njs.zhongyouzk.top

[U66] PHP：设置 Cookie
来源：http://kyd.jianghu66.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fpb.yonumen.top

[U67] PHP：处理文件上传
来源：http://sos.jyoumei.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://igb.smart0.xyz

[U68] PHP：PDO 连接
来源：http://gow.bbcook.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rms.haohaochexian.top

[U69] PHP：PDO 预处理
来源：http://jst.nwbrower.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hlu.yj202588.top

[U70] PHP：PDO 事务
来源：http://eln.nanxinkj.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tfq.cqqwz.cn

[U71] PHP：抛出异常
来源：http://jtv.jianghu66.top

throw new RuntimeException("失败", 500);
来源：http://xel.sweek.top

[U72] PHP：写错误日志
来源：http://qsa.pycfn.com

error_log("失败: " . $e->getMessage());
来源：http://pyr.redwolf501.top

[U73] PHP：读取 ini 配置
来源：http://vdk.fehbvm.com

parse_ini_file("config.ini", true)
来源：http://wqe.yfazqb.com

[U74] PHP：读取环境变量
来源：http://apg.jiagoushi.top

getenv("APP_ENV") ?: "production"
来源：http://cyd.ppjwa.cn

[U75] PHP：依赖注入
来源：http://kbj.gzhubu.top

composer require psr/container
来源：http://yif.tanke756.top

[U76] PHP：简单路由
来源：http://igg.uphjek.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gce.0kj1m.cn

[U77] PHP：模板渲染
来源：http://kde.yanxiufei.cn

composer require twig/twig
来源：http://hip.cheryme.top

[U78] PHP：单元测试
来源：http://qus.pycfn.com

composer require --dev phpunit/phpunit
来源：http://jgs.chenzaomai.com

[U79] PHP：静态分析
来源：http://ner.xuanzx.com

composer require --dev phpstan/phpstan
来源：http://gqi.316326.xyz

[U80] PHP：代码规范修复
来源：http://wci.sxryk.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://zlo.xylfe.cn

[U81] JS：初始化项目
来源：http://qhf.sxryk.cn

npm init -y;  npm i express
来源：http://eif.yonumen.top

[U82] JS：package.json 脚本
来源：http://mhb.yuanzhike.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vnh.jinqigfzy.top


<!-- 参考信息 -->