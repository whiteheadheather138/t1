代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://xjd.pengpengdd.cyou

[S59] C++：静态断言
来源：http://tkb.hywenlv.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vqr.gotoacloud.top

[S60] C++：遍历并删除元素
来源：http://gam.redwolf501.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lqn.cdnleiting.top

================================================================================
来源：http://khm.tianlin.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jbx.aizwys.cn

================================================================================
来源：http://pvj.wangshuangyany.cn

[T01] Kotlin：Hello World
来源：http://yux.hnqzz.top

println("Hello")
来源：http://dmb.dianchejie.cn

[T02] Kotlin：变量
来源：http://wuc.shuidangran.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hxa.jinyuanbaomall.cn

[T03] Kotlin：字符串模板
来源：http://eso.yonumen.top

"值: $b"
来源：http://cex.cucudq.cn

[T04] Kotlin：空安全
来源：http://dct.yj20258.top

val n: String? = null;  n?.length
来源：http://czb.52xcode.cn

[T05] Kotlin：when 表达式
来源：http://pdi.sjlbkw.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rpx.gaohongyu789.top

[T06] Kotlin：集合映射
来源：http://jsa.iojbl.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://puq.cucudq.cn

[T07] Kotlin：集合过滤
来源：http://ezj.fzhhl.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://mnf.gotoacloud.top

[T08] Kotlin：数据类
来源：http://wus.yonumen.top

data class User(val name: String, val age: Int)
来源：http://hyn.yuxming.cn

[T09] Kotlin：扩展函数
来源：http://ucs.xuanzx.com

fun String.exclaim() = this + "!"
来源：http://qqk.hywenlv.cn

[T10] Kotlin：默认参数
来源：http://sft.shangyingyoupin.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ndu.cheryme.top

[T11] Kotlin：协程
来源：http://ulr.pycfn.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://xji.jinyuanbaomall.cn

[T12] Kotlin：解构声明
来源：http://kmm.svipenyu.cn

val (a, b) = Pair(1, 2)
来源：http://lwb.cqqwz.cn

[T13] Kotlin：只读 Map
来源：http://fpm.jyoumei.cn

val m = mapOf("a" to 1)
来源：http://pzj.haohaochexian.top

[T14] Kotlin：循环
来源：http://wzn.birdmap.top

for (i in 1..10) println(i)
来源：http://zly.xuetiantiany.cn

[T15] Kotlin：接口
来源：http://yea.hnqzz.top

interface Shape { fun area(): Double }
来源：http://mqj.zhixingplan.top

[T16] Swift：Hello World
来源：http://eft.ppjwa.cn

print("Hello")
来源：http://tgq.yj20258.top

[T17] Swift：变量与常量
来源：http://keq.shanyushiyangkeji.top

var a = 1;  let b = 2
来源：http://til.fktsv.cn

[T18] Swift：字符串插值
来源：http://qid.guowangkeji.top

"值: \(b)"
来源：http://xvb.aizwys.cn

[T19] Swift：可选绑定
来源：http://bzw.zhiwuduotai.top

if let n = opt { print(n) }
来源：http://eyv.zdqjudy.top

[T20] Swift：数组操作
来源：http://ojn.mhx1999.top

var a = [1, 2, 3];  a.append(4)
来源：http://qrj.xziqi.cn

[T21] Swift：遍历
来源：http://eih.mhx1999.top

for x in a { print(x) }
来源：http://cag.c1oappe.top

[T22] Swift：字典
来源：http://kem.pycfn.com

var d = ["a": 1];  d["b"] = 2
来源：http://bpl.fanxiaobao.xyz

[T23] Swift：函数
来源：http://qot.jinqigufen.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yzj.nanxinkj.top

[T24] Swift：闭包
来源：http://ouj.xinyue.icu

let f = { (x: Int) -> Int in x * 2 }
来源：http://nhq.shuidangran.top

[T25] Swift：结构体
来源：http://isf.birdmap.top

struct P { var x: Int }
来源：http://rae.yangfankeji.com

[T26] Swift：类与重写
来源：http://yqu.hysaishi.cn

class A: Base { override func f() {} }
来源：http://tfi.chenlongwang.top

[T27] Swift：错误处理
来源：http://ppp.zhaomingkeji.xyz

do { try f() } catch { print(error) }
来源：http://pxj.jinqigfzy.top

[T28] Swift：枚举
来源：http://ddi.0kj1m.cn

enum Color { case red, green }
来源：http://vyg.yj202588.top

[T29] Swift：guard 提前返回
来源：http://eui.ivvv.top

guard let x = opt else { return }
来源：http://rfw.fzhhl.top

[T30] Swift：协议
来源：http://gxd.xylfe.cn

protocol Shape { func area() -> Double }
来源：http://vxh.fehbvm.com

[T31] Lua：Hello World
来源：http://lfq.wangshuangyany.cn

print("Hello")
来源：http://yrl.gotoacloud.top

[T32] Lua：局部变量
来源：http://ifj.yangfankeji.com

local a = 1
来源：http://dwz.shangyingyoupin.top

[T33] Lua：表（数组）
来源：http://ftw.ybcxt.top

local t = {1, 2, 3};  t[4] = 4
来源：http://auw.yj20258888.top

[T34] Lua：遍历表
来源：http://uvg.sjlbkw.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://tdv.cheryme.top

[T35] Lua：字典表
来源：http://oth.vehdjk.com

local d = { a = 1 };  d.b = 2
来源：http://bxd.sxryk.cn

[T36] Lua：函数
来源：http://tez.ywan-chungtsiang.top

function add(a, b) return a + b end
来源：http://wtb.ppjwa.cn

[T37] Lua：字符串拼接
来源：http://gsn.ywan-chungtsiang.top

"a" .. "b"
来源：http://rek.pycfn.com

[T38] Lua：条件
来源：http://pon.sxryk.cn

if x > 0 then print("正") end
来源：http://rju.zhijiandao.cn

[T39] Lua：模式匹配
来源：http://bww.cashguo.top

string.find(s, "%d+")
来源：http://knx.guowangkeji.top

[T40] Lua：元表
来源：http://dwe.yueranfly.top

setmetatable({}, { __index = base })
来源：http://vdg.svipenyu.cn

[T41] Perl：Hello World
来源：http://qtw.chenlongwang.top

print "Hello\n";
来源：http://aqu.fktsv.cn

[T42] Perl：变量类型
来源：http://btb.svipenyu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cvn.hongshengwenyu.top

[T43] Perl：字符串插值
来源：http://nuy.andypj.xyz

"值: $a"
来源：http://gam.hesvh.cn

[T44] Perl：条件
来源：http://zld.zhiwuduotai.top

if ($a > 0) { print "正"; }
来源：http://ihq.yj202588.top

[T45] Perl：数组遍历
来源：http://pxx.zhongyouzk.top

for my $x (@arr) { print $x; }
来源：http://yls.xingfuxueyuan.xyz

[T46] Perl：哈希操作
来源：http://jxo.cdnleiting.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://unb.dianchejie.cn

[T47] Perl：正则捕获
来源：http://vdy.zdbjq.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://lau.yangfankeji.com

[T48] Perl：正则替换
来源：http://odn.sysykeji.top

$s =~ s/old/new/g;
来源：http://kam.shuidangran.top

[T49] Perl：函数
来源：http://ybw.sufxvd.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zqv.zdqjudy.top

[T50] Perl：逐行读文件
来源：http://xjz.yvedp.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zkt.zdqjudy.top

while (my $line = <$fh>) { print $line; }
来源：http://umw.gogol.net.cn

[T51] Scala：Hello World
来源：http://att.zhongyouzk.top

println("Hello")
来源：http://low.fengsongda.top

[T52] Scala：变量
来源：http://sde.jqgfzy.top

val a = 1;  var b = 2
来源：http://agm.hesvh.cn

[T53] Scala：字符串插值
来源：http://rke.zdqjudy.top

s"值: $b"
来源：http://mdp.meibo888.top

[T54] Scala：集合映射
来源：http://ygl.sjlbkw.cn

List(1, 2, 3).map(_ * 2)
来源：http://kuu.daria6918.cn

[T55] Scala：集合过滤
来源：http://eja.haohaochexian.top

List(1, 2, 3).filter(_ > 1)
来源：http://pio.hongshengwenyu.top

[T56] Scala：样例类
来源：http://ffc.gotoacloud.top

case class User(name: String, age: Int)
来源：http://hhf.jinqigfzy.top

[T57] Scala：模式匹配
来源：http://zhl.daxiang520.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ywk.zdbjq.cn

[T58] Scala：函数定义
来源：http://kuv.cucudq.cn

def add(a: Int, b: Int): Int = a + b
来源：http://mjd.ybcxt.top

[T59] Scala：循环
来源：http://tgt.daxiang520.top

for (i <- 1 to 10) println(i)
来源：http://aok.aibaodan.cn

[T60] Scala：折叠
来源：http://sdy.cqqwz.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ivq.tanke756.top

================================================================================
来源：http://dql.chenjidiqi.icu

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qcs.hcnkem.com

================================================================================
来源：http://ctn.hnqzz.top

[U01] Py：创建虚拟环境
来源：http://lfr.birdmap.top

python -m venv .venv && source .venv/bin/activate
来源：http://joh.iojbl.cn

[U02] Py：导出 / 安装依赖
来源：http://wsa.guannengcc.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jul.fzhhl.top

[U03] Py：加载 .env 配置
来源：http://mfj.uphjek.com

from dotenv import load_dotenv; load_dotenv()
来源：http://bkl.jinqigfzy.top

[U04] Py：变量调试打印
来源：http://jyv.fehbvm.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gcf.aibaodan.cn

[U05] Py：列表去重且保序
来源：http://ttm.jqgfzy.top

list(dict.fromkeys(arr))
来源：http://aef.shanyushiyangtech.top

[U06] Py：合并两个字典
来源：http://nvr.52xcode.cn

{**a, **b}
来源：http://xkz.andypj.xyz

[U07] Py：反转字典键值
来源：http://anj.c1oappe.top

{v: k for k, v in d.items()}
来源：http://dxw.zhaomingkeji.xyz

[U08] Py：展平二维列表
来源：http://oii.yj202588.top

[y for x in nested for y in x]
来源：http://iea.dashuyun.cn

[U09] Py：字典取最大值的键
来源：http://jjh.vehdjk.com

max(d, key=d.get)
来源：http://tub.guannengcc.top

[U10] Py：按值排序字典
来源：http://kxu.daxiang520.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://stb.shangyingyoupin.top

[U11] Py：生成器表达式
来源：http://gxf.birdmap.top

(x * 2 for x in arr)
来源：http://ial.gogol.net.cn

[U12] Py：取出现最多的 3 个元素
来源：http://jdi.yfazqb.com

Counter(arr).most_common(3)
来源：http://adn.jinqigufen.top

[U13] Py：固定长度队列
来源：http://fvg.yfazqb.com

deque(maxlen=10)
来源：http://pyt.jlsjyb.cn

[U14] Py：分组收集到列表
来源：http://glc.wangdashe.top

defaultdict(list)
来源：http://gwn.ehwqpu.com

[U15] Py：高精度计时
来源：http://mug.gotoacloud.top

t = time.perf_counter()
来源：http://clf.chenjidiqi.icu

[U16] Py：命令行参数解析
来源：http://zdj.hesvh.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yjt.jinqigufen.top

[U17] Py：初始化日志
来源：http://nvp.vqdsnc.cn

logging.basicConfig(level=logging.INFO)
来源：http://pyd.xuetiantiany.cn

[U18] Py：预编译正则
来源：http://tto.52xcode.cn

pat = re.compile(r"\d+")
来源：http://qiw.jinyuanbaomall.cn

[U19] Py：正则替换带回调
来源：http://jon.mhx1999.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://uaf.xuetiantiany.cn

[U20] Py：缓存函数结果
来源：http://vuo.zhijiandao.cn

@functools.lru_cache(maxsize=None)
来源：http://nxx.ppjwa.cn

[U21] Py：自定义上下文管理器
来源：http://slq.haohaochexian.top

@contextlib.contextmanager
来源：http://cbr.ehwqpu.com

[U22] Py：矩阵转置
来源：http://fip.xziqi.cn

list(zip(*m))
来源：http://oms.hammf.cn

[U23] Py：分块读取大文件
来源：http://xee.yj20258888.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lss.snrcjt.cn

[U24] Py：路径操作
来源：http://hcg.xylfe.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qtv.ivvv.top

[U25] Py：CSV 按字典读
来源：http://sxd.yonumen.top

csv.DictReader(f)
来源：http://mfh.ybcxt.top

[U26] Py：并发下载
来源：http://tzc.yongpay.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://udm.quarkkingdee.top

[U27] Py：异步 HTTP
来源：http://bof.9152youxi.cn

aiohttp.ClientSession() 配合 async with
来源：http://oau.gotoacloud.top

[U28] Py：类型别名
来源：http://hmm.yanxiufei.cn

UserId = int
来源：http://vjs.tanke756.top

[U29] Py：属性校验
来源：http://owd.xingfuxueyuan.xyz

@property 与 @x.setter 配合
来源：http://wzm.jinyuanbaomall.cn

[U30] Py：数据类
来源：http://rkm.gaohongyu789.top

@dataclass(slots=True)
来源：http://jek.zhixingplan.top

[U31] Py：单测
来源：http://kfi.snrcjt.cn

python -m pytest -q
来源：http://evt.zhijiandao.cn

[U32] Py：代码格式化
来源：http://ecs.ctjpmb.com

ruff format . && ruff check --fix .
来源：http://eqs.9152youxi.cn

[U33] Py：打包发布
来源：http://hcg.hcnkem.com

python -m build  （依赖 pyproject.toml）
来源：http://bgx.fzhhl.top

[U34] Py：判断编码
来源：http://tzq.zhoulong.xyz

chardet.detect(raw)
来源：http://acu.jqgfzy.top

[U35] Py：发送邮件
来源：http://dyf.yj202588.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cez.yanxiufei.cn

[U36] Py：定时任务
来源：http://vlq.havefunace.top

schedule.every(10).minutes.do(job)
来源：http://dhk.fanxiaobao.xyz

[U37] Py：读写 Excel
来源：http://pqd.tarul.cn

pandas.read_excel / DataFrame.to_excel
来源：http://omi.tianlin.xyz

[U38] Py：获取脚本所在目录
来源：http://lks.yonumen.top

Path(__file__).resolve().parent
来源：http://gjs.sjlbkw.cn

[U39] Py：判断是否在交互环境
来源：http://utx.xylfe.cn

sys.stdout.isatty()
来源：http://yqj.jianghu66.top

[U40] Py：打印到标准错误
来源：http://tis.316326.xyz

print("err", file=sys.stderr)
来源：http://zfg.guannengcc.top

[U41] PHP：初始化 Composer 项目
来源：http://mlq.chenzaomai.com

composer init;  composer require guzzlehttp/guzzle
来源：http://uqm.hywenlv.cn

[U42] PHP：PSR-4 自动加载
来源：http://vyf.hywenlv.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wav.c1oappe.top

[U43] PHP：声明命名空间
来源：http://eil.meibo888.top

namespace App\Http;
来源：http://hqk.chenlongwang.top

[U44] PHP：开启严格类型
来源：http://php.guowangkeji.top

declare(strict_types=1);
来源：http://gfb.hammf.cn

[U45] PHP：类型声明与返回类型
来源：http://htu.pengpengdd.cyou

function add(int $a, int $b): int { return $a + $b; }
来源：http://wty.sufxvd.cn

[U46] PHP：可空类型
来源：http://nki.jiagoushi.top

?string $name = null
来源：http://fop.uphjek.com

[U47] PHP：联合类型
来源：http://zeb.sjlbkw.cn

int|string $id
来源：http://pea.yanxiufei.cn

[U48] PHP：纯枚举
来源：http://oda.fengsongda.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hpi.cucudq.cn

[U49] PHP：只读属性
来源：http://ouz.fktsv.cn

public readonly string $name
来源：http://epx.ctjpmb.com

[U50] PHP：构造器属性提升
来源：http://bxw.yj20258.top

public function __construct(private int $id) {}
来源：http://acb.yangfankeji.com

[U51] PHP：数组解构
来源：http://gif.meibo888.top

[$a, $b] = $arr;
来源：http://ymi.ivvv.top

[U52] PHP：箭头函数
来源：http://szh.daria6918.cn

$double = fn($x) => $x * 2;
来源：http://lci.xziqi.cn

[U53] PHP：空合并运算符
来源：http://uvy.nanxinkj.top

$v = $a ?? $b ?? "default";
来源：http://zef.fehbvm.com

[U54] PHP：空安全调用
来源：http://cqd.epnwcf.com

$obj?->method()
来源：http://ghb.yj202588.top

[U55] PHP：match 表达式
来源：http://ial.daxiang520.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://pqa.jiagoushi.top

[U56] PHP：命名参数
来源：http://mtz.zhixingplan.top

f(a: 1, b: 2)
来源：http://mif.tanke756.top

[U57] PHP：字符串插值
来源：http://lma.gotoacloud.top

"值: {$a}"
来源：http://fng.yuxming.cn

[U58] PHP：数组三件套
来源：http://jdy.iojbl.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://krq.andypj.xyz

[U59] PHP：自定义排序
来源：http://bvm.316326.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ipw.xuetiantiany.cn

[U60] PHP：JSON 编解码
来源：http://cse.ctjpmb.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jzm.jinyuanbaomall.cn

[U61] PHP：正则
来源：http://jvp.aizwys.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://eqg.mhx1999.top

[U62] PHP：日期对象
来源：http://imq.fktsv.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vel.fzhhl.top

[U63] PHP：文件读写
来源：http://enp.smart0.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ipm.shuidangran.top

[U64] PHP：目录遍历
来源：http://kio.ivvv.top

glob("dir/*.php");  scandir("dir");
来源：http://jgr.tian-w.cn

[U65] PHP：会话
来源：http://uwy.tanke756.top

session_start();  $_SESSION["uid"] = 1;
来源：http://dum.jqgufenzy.top

[U66] PHP：设置 Cookie
来源：http://bzk.xinyue.icu

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mjw.meibo888.top

[U67] PHP：处理文件上传
来源：http://ixh.andypj.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://nzd.jqgfzy.top

[U68] PHP：PDO 连接
来源：http://spp.zhiwuduotai.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pdw.tian-w.cn

[U69] PHP：PDO 预处理
来源：http://xjb.jinqigfzy.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://agp.tarul.cn

[U70] PHP：PDO 事务
来源：http://qoi.ywan-chungtsiang.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://chf.shangyingyoupin.top

[U71] PHP：抛出异常
来源：http://tyi.sysykeji.top

throw new RuntimeException("失败", 500);
来源：http://zey.nanxuanxn.top

[U72] PHP：写错误日志
来源：http://xmf.xziqi.cn

error_log("失败: " . $e->getMessage());
来源：http://ypu.fktsv.cn

[U73] PHP：读取 ini 配置
来源：http://ibm.jinyuanbaomall.cn

parse_ini_file("config.ini", true)
来源：http://tyh.zhoulong.xyz

[U74] PHP：读取环境变量
来源：http://lur.hcnkem.com

getenv("APP_ENV") ?: "production"
来源：http://qkw.tanke756.top

[U75] PHP：依赖注入
来源：http://gwt.yfazqb.com

composer require psr/container
来源：http://etd.ppjwa.cn

[U76] PHP：简单路由
来源：http://evv.jinqigufen.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://opx.tianlin.xyz

[U77] PHP：模板渲染
来源：http://age.uphjek.com

composer require twig/twig
来源：http://rpr.xinyue.icu

[U78] PHP：单元测试
来源：http://mfu.shanyushiyangtech.top

composer require --dev phpunit/phpunit
来源：http://wti.chenzaomai.com

[U79] PHP：静态分析
来源：http://avz.xingfuxueyuan.xyz

composer require --dev phpstan/phpstan
来源：http://kdm.birdmap.top

[U80] PHP：代码规范修复
来源：http://mgm.ywan-chungtsiang.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ebo.shzxlz.cn

[U81] JS：初始化项目
来源：http://pqh.dianchejie.cn

npm init -y;  npm i express
来源：http://vld.ctjpmb.com

[U82] JS：package.json 脚本
来源：http://irw.jianghu66.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kzh.fehbvm.com

[U83] JS：ES Module 导入导出
来源：http://cyc.0kj1m.cn

export const a = 1;  import { a } from "./m.js";
来源：http://heg.pycfn.com

[U84] JS：CommonJS 写法
来源：http://icd.xylfe.cn

module.exports = { a };  const { a } = require("./m");
来源：http://srs.bjfxy.top


<!-- 参考信息 -->