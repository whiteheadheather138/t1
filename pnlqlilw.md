代发 wailian999

int size() const noexcept { return n_; }
来源：http://nuh.cheryme.top

[S53] C++：移动语义
来源：http://nge.tanke756.top

std::vector<int> w = std::move(v);
来源：http://gcr.smart0.xyz

[S54] C++：异常处理
来源：http://fxb.hcnkem.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://udb.bbcook.cn

[S55] C++：结构化绑定
来源：http://pcn.bjfxy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://pax.52xcode.cn

[S56] C++：optional
来源：http://srg.xylfe.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://boj.birdmap.top

[S57] C++：编译期常量
来源：http://war.jiagoushi.top

constexpr int N = 10;
来源：http://voe.yuanzhike.top

[S58] C++：命名空间
来源：http://oar.tarul.cn

namespace ns { int f() { return 1; } }
来源：http://xsd.pycfn.com

[S59] C++：静态断言
来源：http://tww.shanyushiyangtech.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dov.zhiwuduotai.top

[S60] C++：遍历并删除元素
来源：http://bso.birdmap.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://unu.jyoumei.cn

================================================================================
来源：http://caa.yongpay.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zgz.daria6918.cn

================================================================================
来源：http://dgh.shuidangran.top

[T01] Kotlin：Hello World
来源：http://bch.zhoulong.xyz

println("Hello")
来源：http://jvc.ehwqpu.com

[T02] Kotlin：变量
来源：http://mgg.xingfuxueyuan.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zgm.gaohongyu789.top

[T03] Kotlin：字符串模板
来源：http://dis.zhijiandao.cn

"值: $b"
来源：http://kip.vqdsnc.cn

[T04] Kotlin：空安全
来源：http://sry.ctjpmb.com

val n: String? = null;  n?.length
来源：http://zay.iojbl.cn

[T05] Kotlin：when 表达式
来源：http://bfg.zdbjq.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cld.ehwqpu.com

[T06] Kotlin：集合映射
来源：http://hoi.jinghuilouyu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://uzq.zhengqikj.top

[T07] Kotlin：集合过滤
来源：http://fug.sweek.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ozn.xziqi.cn

[T08] Kotlin：数据类
来源：http://orr.zhiwuduotai.top

data class User(val name: String, val age: Int)
来源：http://cin.0kj1m.cn

[T09] Kotlin：扩展函数
来源：http://ljq.cqqwz.cn

fun String.exclaim() = this + "!"
来源：http://hmg.yuanzhike.top

[T10] Kotlin：默认参数
来源：http://rzr.yj20258888.top

fun greet(name: String = "World") = "Hi $name"
来源：http://piv.chenjidiqi.icu

[T11] Kotlin：协程
来源：http://vjk.xuanzx.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://vka.chenlongwang.top

[T12] Kotlin：解构声明
来源：http://owo.jqgufenzy.top

val (a, b) = Pair(1, 2)
来源：http://icw.cdnleiting.top

[T13] Kotlin：只读 Map
来源：http://ktd.52xcode.cn

val m = mapOf("a" to 1)
来源：http://izj.zhixingplan.top

[T14] Kotlin：循环
来源：http://fla.yj20258.top

for (i in 1..10) println(i)
来源：http://yid.yueranfly.top

[T15] Kotlin：接口
来源：http://jxs.tarul.cn

interface Shape { fun area(): Double }
来源：http://wtd.dashuyun.cn

[T16] Swift：Hello World
来源：http://rhy.fengsongda.top

print("Hello")
来源：http://ypk.shanyushiyangtech.top

[T17] Swift：变量与常量
来源：http://bwl.hnqzz.top

var a = 1;  let b = 2
来源：http://gos.bbcook.cn

[T18] Swift：字符串插值
来源：http://kjc.mhx1999.top

"值: \(b)"
来源：http://jny.gaohongyu789.top

[T19] Swift：可选绑定
来源：http://ybm.smart0.xyz

if let n = opt { print(n) }
来源：http://upd.hysaishi.cn

[T20] Swift：数组操作
来源：http://hge.zdbjq.cn

var a = [1, 2, 3];  a.append(4)
来源：http://axy.fehbvm.com

[T21] Swift：遍历
来源：http://pcg.ywan-chungtsiang.top

for x in a { print(x) }
来源：http://tjs.zdbjq.cn

[T22] Swift：字典
来源：http://djx.zhiwuduotai.top

var d = ["a": 1];  d["b"] = 2
来源：http://noq.yj202588.top

[T23] Swift：函数
来源：http://mwn.dashuyun.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gkq.bjfxy.top

[T24] Swift：闭包
来源：http://dtp.tarul.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://tyr.xylfe.cn

[T25] Swift：结构体
来源：http://pjp.ydzc1.top

struct P { var x: Int }
来源：http://ijy.zhaomingkeji.xyz

[T26] Swift：类与重写
来源：http://izb.fehbvm.com

class A: Base { override func f() {} }
来源：http://ots.zycfv.cn

[T27] Swift：错误处理
来源：http://vxe.meibo888.top

do { try f() } catch { print(error) }
来源：http://ndd.shangyingyoupin.top

[T28] Swift：枚举
来源：http://bqk.gotoacloud.top

enum Color { case red, green }
来源：http://del.shanyushiyangtech.top

[T29] Swift：guard 提前返回
来源：http://wus.0kj1m.cn

guard let x = opt else { return }
来源：http://qxe.dashuyun.cn

[T30] Swift：协议
来源：http://bde.xylfe.cn

protocol Shape { func area() -> Double }
来源：http://tbl.hcnkem.com

[T31] Lua：Hello World
来源：http://yzx.yanxiufei.cn

print("Hello")
来源：http://wie.gaohongyu789.top

[T32] Lua：局部变量
来源：http://uis.zhiwuduotai.top

local a = 1
来源：http://qyj.andypj.xyz

[T33] Lua：表（数组）
来源：http://ijj.aizwys.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://zfu.yangfankeji.com

[T34] Lua：遍历表
来源：http://ece.gotoacloud.top

for i, v in ipairs(t) do print(i, v) end
来源：http://qlr.sweek.top

[T35] Lua：字典表
来源：http://qnx.ydzc1.top

local d = { a = 1 };  d.b = 2
来源：http://psl.jinqigufen.top

[T36] Lua：函数
来源：http://rch.pengpengdd.cyou

function add(a, b) return a + b end
来源：http://lpn.aibaodan.cn

[T37] Lua：字符串拼接
来源：http://giv.cheryme.top

"a" .. "b"
来源：http://qiv.fzhhl.top

[T38] Lua：条件
来源：http://pwv.uphjek.com

if x > 0 then print("正") end
来源：http://bnh.mhx1999.top

[T39] Lua：模式匹配
来源：http://kfh.yvedp.cn

string.find(s, "%d+")
来源：http://gvf.cheryme.top

[T40] Lua：元表
来源：http://sbm.yj202588.top

setmetatable({}, { __index = base })
来源：http://eyg.zhixingplan.top

[T41] Perl：Hello World
来源：http://fho.zhoulong.xyz

print "Hello\n";
来源：http://nhs.tanke756.top

[T42] Perl：变量类型
来源：http://sdq.hnqzz.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pub.jqgfzy.top

[T43] Perl：字符串插值
来源：http://jfv.jlsjyb.cn

"值: $a"
来源：http://jkq.vehdjk.com

[T44] Perl：条件
来源：http://vfu.kuanghao11.cn

if ($a > 0) { print "正"; }
来源：http://vla.chenzaomai.com

[T45] Perl：数组遍历
来源：http://rti.vqdsnc.cn

for my $x (@arr) { print $x; }
来源：http://ths.c1oappe.top

[T46] Perl：哈希操作
来源：http://vyd.aizwys.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dnk.nwbrower.top

[T47] Perl：正则捕获
来源：http://kxo.guannengcc.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://msp.yfazqb.com

[T48] Perl：正则替换
来源：http://ayc.fehbvm.com

$s =~ s/old/new/g;
来源：http://vjo.havefunace.top

[T49] Perl：函数
来源：http://ixu.c1oappe.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://umt.guannengcc.top

[T50] Perl：逐行读文件
来源：http://upk.daxiang520.top

open my $fh, "<", "a.txt" or die $!;
来源：http://hgu.mhx1999.top

while (my $line = <$fh>) { print $line; }
来源：http://gkn.ivvv.top

[T51] Scala：Hello World
来源：http://qud.tarul.cn

println("Hello")
来源：http://vpw.chenjidiqi.icu

[T52] Scala：变量
来源：http://hgz.epnwcf.com

val a = 1;  var b = 2
来源：http://bdh.sweek.top

[T53] Scala：字符串插值
来源：http://for.birdmap.top

s"值: $b"
来源：http://bwr.zhongyouzk.top

[T54] Scala：集合映射
来源：http://opy.dianchejie.cn

List(1, 2, 3).map(_ * 2)
来源：http://ysu.jyoumei.cn

[T55] Scala：集合过滤
来源：http://osc.sxryk.cn

List(1, 2, 3).filter(_ > 1)
来源：http://hqa.guowangkeji.top

[T56] Scala：样例类
来源：http://idd.cheryme.top

case class User(name: String, age: Int)
来源：http://yss.uphjek.com

[T57] Scala：模式匹配
来源：http://qef.iojbl.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ohx.hnqzz.top

[T58] Scala：函数定义
来源：http://fgg.0kj1m.cn

def add(a: Int, b: Int): Int = a + b
来源：http://hrk.cqqwz.cn

[T59] Scala：循环
来源：http://nio.zhaomingkeji.xyz

for (i <- 1 to 10) println(i)
来源：http://ubl.daxiang520.top

[T60] Scala：折叠
来源：http://hio.dashuyun.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cpi.iojbl.cn

================================================================================
来源：http://rds.chenzaomai.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mkc.jqgfzy.top

================================================================================
来源：http://ubp.zhixingplan.top

[U01] Py：创建虚拟环境
来源：http://lxj.tanke756.top

python -m venv .venv && source .venv/bin/activate
来源：http://gpn.jqgfzy.top

[U02] Py：导出 / 安装依赖
来源：http://vkw.yj20258888.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tqb.tanke756.top

[U03] Py：加载 .env 配置
来源：http://xot.ivvv.top

from dotenv import load_dotenv; load_dotenv()
来源：http://vst.sufxvd.cn

[U04] Py：变量调试打印
来源：http://txc.c1oappe.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jrp.kuanghao11.cn

[U05] Py：列表去重且保序
来源：http://mdv.bjfxy.top

list(dict.fromkeys(arr))
来源：http://rwa.kuanghao11.cn

[U06] Py：合并两个字典
来源：http://sll.guowangkeji.top

{**a, **b}
来源：http://dix.xinyue.icu

[U07] Py：反转字典键值
来源：http://lcv.tianlin.xyz

{v: k for k, v in d.items()}
来源：http://aji.pengpengdd.cyou

[U08] Py：展平二维列表
来源：http://wzz.fehbvm.com

[y for x in nested for y in x]
来源：http://nnu.hfpthk.cn

[U09] Py：字典取最大值的键
来源：http://gqm.smart0.xyz

max(d, key=d.get)
来源：http://qrv.andypj.xyz

[U10] Py：按值排序字典
来源：http://ulr.zhijiandao.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lrk.snrcjt.cn

[U11] Py：生成器表达式
来源：http://ngf.iojbl.cn

(x * 2 for x in arr)
来源：http://erl.aizwys.cn

[U12] Py：取出现最多的 3 个元素
来源：http://kfn.shuidangran.top

Counter(arr).most_common(3)
来源：http://xpb.hysaishi.cn

[U13] Py：固定长度队列
来源：http://xat.chenjidiqi.icu

deque(maxlen=10)
来源：http://rjf.haohaochexian.top

[U14] Py：分组收集到列表
来源：http://kzw.hnxiangtu.top

defaultdict(list)
来源：http://znu.chenlongwang.top

[U15] Py：高精度计时
来源：http://hyu.mhx1999.top

t = time.perf_counter()
来源：http://ctb.zdqjudy.top

[U16] Py：命令行参数解析
来源：http://dme.jiagoushi.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sxy.xingfuxueyuan.xyz

[U17] Py：初始化日志
来源：http://ucf.xingfuxueyuan.xyz

logging.basicConfig(level=logging.INFO)
来源：http://gnl.nanxinkj.top

[U18] Py：预编译正则
来源：http://nre.andypj.xyz

pat = re.compile(r"\d+")
来源：http://lml.jqgfzy.top

[U19] Py：正则替换带回调
来源：http://qvh.zhixingplan.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bzl.xuanzx.com

[U20] Py：缓存函数结果
来源：http://mtw.fzhhl.top

@functools.lru_cache(maxsize=None)
来源：http://nax.feifeiyinyue.top

[U21] Py：自定义上下文管理器
来源：http://hou.zhongyouzk.top

@contextlib.contextmanager
来源：http://fqc.jinqigufen.top

[U22] Py：矩阵转置
来源：http://cgt.daria6918.cn

list(zip(*m))
来源：http://lcn.jqgfzy.top

[U23] Py：分块读取大文件
来源：http://gtl.daria6918.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://soa.jqgfzy.top

[U24] Py：路径操作
来源：http://xey.ehwqpu.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vkz.zycfv.cn

[U25] Py：CSV 按字典读
来源：http://uqj.dashuyun.cn

csv.DictReader(f)
来源：http://szp.ydjk.org.cn

[U26] Py：并发下载
来源：http://hke.dashuyun.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hac.yuxming.cn

[U27] Py：异步 HTTP
来源：http://ppl.pycfn.com

aiohttp.ClientSession() 配合 async with
来源：http://pzn.fktsv.cn

[U28] Py：类型别名
来源：http://rzk.zhixingplan.top

UserId = int
来源：http://kps.feifeiyinyue.top

[U29] Py：属性校验
来源：http://gla.redwolf501.top

@property 与 @x.setter 配合
来源：http://zsa.ydjk.org.cn

[U30] Py：数据类
来源：http://oog.aizwys.cn

@dataclass(slots=True)
来源：http://umj.fengsongda.top

[U31] Py：单测
来源：http://ztc.shanyushiyangkeji.top

python -m pytest -q
来源：http://qww.xylfe.cn

[U32] Py：代码格式化
来源：http://sur.jinghuilouyu.cn

ruff format . && ruff check --fix .
来源：http://bkb.gzhubu.top

[U33] Py：打包发布
来源：http://obh.yuanzhike.top

python -m build  （依赖 pyproject.toml）
来源：http://ehv.zhongyouzk.top

[U34] Py：判断编码
来源：http://xxa.sweek.top

chardet.detect(raw)
来源：http://vds.ydzc1.top

[U35] Py：发送邮件
来源：http://jnh.mhx1999.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dej.birdmap.top

[U36] Py：定时任务
来源：http://zqk.jqgufenzy.top

schedule.every(10).minutes.do(job)
来源：http://zgv.gotoacloud.top

[U37] Py：读写 Excel
来源：http://lpf.ivvv.top

pandas.read_excel / DataFrame.to_excel
来源：http://syi.chenjidiqi.icu

[U38] Py：获取脚本所在目录
来源：http://qht.yvedp.cn

Path(__file__).resolve().parent
来源：http://xyy.nwbrower.top

[U39] Py：判断是否在交互环境
来源：http://uop.zycfv.cn

sys.stdout.isatty()
来源：http://esk.wangdashe.top

[U40] Py：打印到标准错误
来源：http://cqr.cucudq.cn

print("err", file=sys.stderr)
来源：http://drw.nanxinkj.top

[U41] PHP：初始化 Composer 项目
来源：http://ajs.havefunace.top

composer init;  composer require guzzlehttp/guzzle
来源：http://klj.316326.xyz

[U42] PHP：PSR-4 自动加载
来源：http://gmr.xuetiantiany.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qsg.ctjpmb.com

[U43] PHP：声明命名空间
来源：http://gmi.yj20258.top

namespace App\Http;
来源：http://pge.vehdjk.com

[U44] PHP：开启严格类型
来源：http://dte.wangshuangyany.cn

declare(strict_types=1);
来源：http://tlx.fehbvm.com

[U45] PHP：类型声明与返回类型
来源：http://wnx.nanxinkj.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://kcg.jianghu66.top

[U46] PHP：可空类型
来源：http://hhf.zhaomingkeji.xyz

?string $name = null
来源：http://lks.zdqjudy.top

[U47] PHP：联合类型
来源：http://tlq.andypj.xyz

int|string $id
来源：http://zjg.zhaomingkeji.xyz

[U48] PHP：纯枚举
来源：http://czn.kuanghao11.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nye.hfpthk.cn

[U49] PHP：只读属性
来源：http://qaq.bjfxy.top

public readonly string $name
来源：http://vnu.bjfxy.top

[U50] PHP：构造器属性提升
来源：http://vuv.yongpay.top

public function __construct(private int $id) {}
来源：http://twc.iojbl.cn

[U51] PHP：数组解构
来源：http://inv.nanxuanxn.top

[$a, $b] = $arr;
来源：http://pdk.hysaishi.cn

[U52] PHP：箭头函数
来源：http://hfr.zhixingplan.top

$double = fn($x) => $x * 2;
来源：http://wgl.shanyushiyangkeji.top

[U53] PHP：空合并运算符
来源：http://avv.zhijiandao.cn

$v = $a ?? $b ?? "default";
来源：http://pli.birdmap.top

[U54] PHP：空安全调用
来源：http://ikx.guannengcc.top

$obj?->method()
来源：http://aes.hammf.cn

[U55] PHP：match 表达式
来源：http://ezw.zhijiandao.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tlk.cdnleiting.top

[U56] PHP：命名参数
来源：http://fdg.pycfn.com

f(a: 1, b: 2)
来源：http://ljq.yj202588.top

[U57] PHP：字符串插值
来源：http://uvu.zdbjq.cn

"值: {$a}"
来源：http://lgp.hysaishi.cn

[U58] PHP：数组三件套
来源：http://and.ivvv.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pru.shangyingyoupin.top

[U59] PHP：自定义排序
来源：http://jjs.ybcxt.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ywc.daria6918.cn

[U60] PHP：JSON 编解码
来源：http://byr.ehwqpu.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ynk.xziqi.cn

[U61] PHP：正则
来源：http://wbq.xylfe.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rqg.cashguo.top

[U62] PHP：日期对象
来源：http://kny.ppjwa.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hpj.yj20258888.top

[U63] PHP：文件读写
来源：http://kjq.xziqi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xmk.shanyushiyangtech.top

[U64] PHP：目录遍历
来源：http://ubt.cqqwz.cn

glob("dir/*.php");  scandir("dir");
来源：http://qxe.52xcode.cn

[U65] PHP：会话
来源：http://yra.0kj1m.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://mnk.andypj.xyz

[U66] PHP：设置 Cookie
来源：http://qao.xuanzx.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ogh.ywan-chungtsiang.top

[U67] PHP：处理文件上传
来源：http://acz.epnwcf.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qnh.zdbjq.cn

[U68] PHP：PDO 连接
来源：http://poz.sjlbkw.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qbe.zhixingplan.top

[U69] PHP：PDO 预处理
来源：http://ydg.ehwqpu.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bmz.sweek.top

[U70] PHP：PDO 事务
来源：http://nsv.tarul.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jju.fehbvm.com

[U71] PHP：抛出异常
来源：http://gzh.jqgfzy.top

throw new RuntimeException("失败", 500);
来源：http://ccg.xuetiantiany.cn

[U72] PHP：写错误日志
来源：http://qtr.zhongyouzk.top

error_log("失败: " . $e->getMessage());
来源：http://fzr.yonumen.top

[U73] PHP：读取 ini 配置
来源：http://rlf.pycfn.com

parse_ini_file("config.ini", true)
来源：http://umq.yonumen.top

[U74] PHP：读取环境变量
来源：http://jac.zhengqikj.top

getenv("APP_ENV") ?: "production"
来源：http://onf.fehbvm.com

[U75] PHP：依赖注入
来源：http://fsi.snrcjt.cn

composer require psr/container
来源：http://ndt.jinghuilouyu.cn

[U76] PHP：简单路由
来源：http://qqe.jinqigfzy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gvf.xziqi.cn

[U77] PHP：模板渲染
来源：http://xli.fanxiaobao.xyz

composer require twig/twig
来源：http://yes.yuxming.cn

[U78] PHP：单元测试
来源：http://ulr.hammf.cn

composer require --dev phpunit/phpunit
来源：http://vuj.xingfuxueyuan.xyz


<!-- 参考信息 -->