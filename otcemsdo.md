代发 wailian999

[T01] Kotlin：Hello World
来源：http://ymu.zdqjudy.top

println("Hello")
来源：http://wwq.shuidangran.top

[T02] Kotlin：变量
来源：http://mww.52xcode.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bdn.cdnleiting.top

[T03] Kotlin：字符串模板
来源：http://ixh.hcnkem.com

"值: $b"
来源：http://kbj.nwbrower.top

[T04] Kotlin：空安全
来源：http://let.hnxiangtu.top

val n: String? = null;  n?.length
来源：http://sia.havefunace.top

[T05] Kotlin：when 表达式
来源：http://lbp.jyoumei.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tus.tian-w.cn

[T06] Kotlin：集合映射
来源：http://iws.sufxvd.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://vuj.hnqzz.top

[T07] Kotlin：集合过滤
来源：http://sgb.jyoumei.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://fkr.gotoacloud.top

[T08] Kotlin：数据类
来源：http://ytk.vehdjk.com

data class User(val name: String, val age: Int)
来源：http://kxv.yongpay.top

[T09] Kotlin：扩展函数
来源：http://npp.shanyushiyangkeji.top

fun String.exclaim() = this + "!"
来源：http://ngt.cucudq.cn

[T10] Kotlin：默认参数
来源：http://prc.andypj.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://bqe.feifeiyinyue.top

[T11] Kotlin：协程
来源：http://edx.cheryme.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ydh.daria6918.cn

[T12] Kotlin：解构声明
来源：http://idj.ppjwa.cn

val (a, b) = Pair(1, 2)
来源：http://hgt.jqgufenzy.top

[T13] Kotlin：只读 Map
来源：http://npu.cdnleiting.top

val m = mapOf("a" to 1)
来源：http://zga.yueranfly.top

[T14] Kotlin：循环
来源：http://bud.iojbl.cn

for (i in 1..10) println(i)
来源：http://hth.shanyushiyangkeji.top

[T15] Kotlin：接口
来源：http://vzt.gzhubu.top

interface Shape { fun area(): Double }
来源：http://wuq.jinyuanbaomall.cn

[T16] Swift：Hello World
来源：http://xbm.nanxuanxn.top

print("Hello")
来源：http://aki.52xcode.cn

[T17] Swift：变量与常量
来源：http://kmb.ywan-chungtsiang.top

var a = 1;  let b = 2
来源：http://ehw.jqgufenzy.top

[T18] Swift：字符串插值
来源：http://azj.sweek.top

"值: \(b)"
来源：http://hil.xylfe.cn

[T19] Swift：可选绑定
来源：http://lka.haohaochexian.top

if let n = opt { print(n) }
来源：http://gqk.aizwys.cn

[T20] Swift：数组操作
来源：http://mnd.316326.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://ulz.zhiwuduotai.top

[T21] Swift：遍历
来源：http://sjv.sjlbkw.cn

for x in a { print(x) }
来源：http://eal.pengpengdd.cyou

[T22] Swift：字典
来源：http://vlw.zdqjudy.top

var d = ["a": 1];  d["b"] = 2
来源：http://rbv.chenjidiqi.icu

[T23] Swift：函数
来源：http://hjg.52xcode.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zwo.redwolf501.top

[T24] Swift：闭包
来源：http://ekl.sweek.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://apv.zhijiandao.cn

[T25] Swift：结构体
来源：http://gvw.nanxuanxn.top

struct P { var x: Int }
来源：http://bfu.cucudq.cn

[T26] Swift：类与重写
来源：http://cqx.ivvv.top

class A: Base { override func f() {} }
来源：http://zvx.jlsjyb.cn

[T27] Swift：错误处理
来源：http://zsa.ctjpmb.com

do { try f() } catch { print(error) }
来源：http://abn.guannengcc.top

[T28] Swift：枚举
来源：http://xvj.yongpay.top

enum Color { case red, green }
来源：http://jgb.yuanzhike.top

[T29] Swift：guard 提前返回
来源：http://cty.jiagoushi.top

guard let x = opt else { return }
来源：http://arr.hnxiangtu.top

[T30] Swift：协议
来源：http://eyz.cqqwz.cn

protocol Shape { func area() -> Double }
来源：http://fgd.jyoumei.cn

[T31] Lua：Hello World
来源：http://emm.gogol.net.cn

print("Hello")
来源：http://ikl.fengsongda.top

[T32] Lua：局部变量
来源：http://gfj.fzhhl.top

local a = 1
来源：http://upi.gogol.net.cn

[T33] Lua：表（数组）
来源：http://jvb.iojbl.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hag.c1oappe.top

[T34] Lua：遍历表
来源：http://gti.cqqwz.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://knq.zhiwuduotai.top

[T35] Lua：字典表
来源：http://fjj.iojbl.cn

local d = { a = 1 };  d.b = 2
来源：http://kia.jqgfzy.top

[T36] Lua：函数
来源：http://zun.wangdashe.top

function add(a, b) return a + b end
来源：http://iba.zhixingplan.top

[T37] Lua：字符串拼接
来源：http://cvu.zhoulong.xyz

"a" .. "b"
来源：http://kgv.shangyingyoupin.top

[T38] Lua：条件
来源：http://fym.shzxlz.cn

if x > 0 then print("正") end
来源：http://vth.quarkkingdee.top

[T39] Lua：模式匹配
来源：http://jum.chenzaomai.com

string.find(s, "%d+")
来源：http://lto.zhengqikj.top

[T40] Lua：元表
来源：http://dia.jinqigufen.top

setmetatable({}, { __index = base })
来源：http://cap.cqqwz.cn

[T41] Perl：Hello World
来源：http://lqk.sysykeji.top

print "Hello\n";
来源：http://deb.zhoulong.xyz

[T42] Perl：变量类型
来源：http://qof.yj20258888.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://asx.feifeiyinyue.top

[T43] Perl：字符串插值
来源：http://dtr.gotoacloud.top

"值: $a"
来源：http://ory.havefunace.top

[T44] Perl：条件
来源：http://gqk.jyoumei.cn

if ($a > 0) { print "正"; }
来源：http://qrv.gaohongyu789.top

[T45] Perl：数组遍历
来源：http://azc.zhijiandao.cn

for my $x (@arr) { print $x; }
来源：http://bzm.mhx1999.top

[T46] Perl：哈希操作
来源：http://pzn.jinghuilouyu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tbv.xingfuxueyuan.xyz

[T47] Perl：正则捕获
来源：http://jpu.shangyingyoupin.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://nkz.andypj.xyz

[T48] Perl：正则替换
来源：http://lvu.ppjwa.cn

$s =~ s/old/new/g;
来源：http://cgr.shzxlz.cn

[T49] Perl：函数
来源：http://wrf.jinyuanbaomall.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://odz.yvedp.cn

[T50] Perl：逐行读文件
来源：http://zyx.sysykeji.top

open my $fh, "<", "a.txt" or die $!;
来源：http://pis.jinqigufen.top

while (my $line = <$fh>) { print $line; }
来源：http://pfg.hywenlv.cn

[T51] Scala：Hello World
来源：http://mmz.yongpay.top

println("Hello")
来源：http://ptn.shuidangran.top

[T52] Scala：变量
来源：http://hou.gaohongyu789.top

val a = 1;  var b = 2
来源：http://usv.chenzaomai.com

[T53] Scala：字符串插值
来源：http://pdc.yvedp.cn

s"值: $b"
来源：http://vwu.shanyushiyangtech.top

[T54] Scala：集合映射
来源：http://jea.zhixingplan.top

List(1, 2, 3).map(_ * 2)
来源：http://fzz.fktsv.cn

[T55] Scala：集合过滤
来源：http://uzd.aizwys.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qpl.guannengcc.top

[T56] Scala：样例类
来源：http://zqm.yfazqb.com

case class User(name: String, age: Int)
来源：http://hip.ydjk.org.cn

[T57] Scala：模式匹配
来源：http://ptf.zhaomingkeji.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://jkq.dashuyun.cn

[T58] Scala：函数定义
来源：http://ywe.xuanzx.com

def add(a: Int, b: Int): Int = a + b
来源：http://npg.shuidangran.top

[T59] Scala：循环
来源：http://bli.pycfn.com

for (i <- 1 to 10) println(i)
来源：http://ate.chenzaomai.com

[T60] Scala：折叠
来源：http://bvx.redwolf501.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rvw.xylfe.cn

================================================================================
来源：http://dts.haohaochexian.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kzy.cqqwz.cn

================================================================================
来源：http://dip.xziqi.cn

[U01] Py：创建虚拟环境
来源：http://tmy.52xcode.cn

python -m venv .venv && source .venv/bin/activate
来源：http://wnx.jlsjyb.cn

[U02] Py：导出 / 安装依赖
来源：http://hbd.jinqigfzy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wrf.zhongyouzk.top

[U03] Py：加载 .env 配置
来源：http://fqw.shangyingyoupin.top

from dotenv import load_dotenv; load_dotenv()
来源：http://qqn.xingfuxueyuan.xyz

[U04] Py：变量调试打印
来源：http://blc.ppjwa.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://six.aizwys.cn

[U05] Py：列表去重且保序
来源：http://dco.xylfe.cn

list(dict.fromkeys(arr))
来源：http://bfq.yangfankeji.com

[U06] Py：合并两个字典
来源：http://bzj.shangyingyoupin.top

{**a, **b}
来源：http://kps.fengsongda.top

[U07] Py：反转字典键值
来源：http://hzw.yvedp.cn

{v: k for k, v in d.items()}
来源：http://ydd.cucudq.cn

[U08] Py：展平二维列表
来源：http://jza.ehwqpu.com

[y for x in nested for y in x]
来源：http://hmt.xylfe.cn

[U09] Py：字典取最大值的键
来源：http://psk.sxryk.cn

max(d, key=d.get)
来源：http://lrm.yanxiufei.cn

[U10] Py：按值排序字典
来源：http://gaz.meibo888.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://oma.bjfxy.top

[U11] Py：生成器表达式
来源：http://vul.ctjpmb.com

(x * 2 for x in arr)
来源：http://vxx.daria6918.cn

[U12] Py：取出现最多的 3 个元素
来源：http://iok.jyoumei.cn

Counter(arr).most_common(3)
来源：http://oue.ivvv.top

[U13] Py：固定长度队列
来源：http://dxk.ydjk.org.cn

deque(maxlen=10)
来源：http://clt.feifeiyinyue.top

[U14] Py：分组收集到列表
来源：http://yuk.yuxming.cn

defaultdict(list)
来源：http://qkc.316326.xyz

[U15] Py：高精度计时
来源：http://atu.ehwqpu.com

t = time.perf_counter()
来源：http://dec.sysykeji.top

[U16] Py：命令行参数解析
来源：http://gyq.hnxiangtu.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vnw.shzxlz.cn

[U17] Py：初始化日志
来源：http://sgc.jinqigfzy.top

logging.basicConfig(level=logging.INFO)
来源：http://ucs.xinyue.icu

[U18] Py：预编译正则
来源：http://bxt.hfpthk.cn

pat = re.compile(r"\d+")
来源：http://vmw.hammf.cn

[U19] Py：正则替换带回调
来源：http://fyi.vqdsnc.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://frw.dashuyun.cn

[U20] Py：缓存函数结果
来源：http://fwz.xinyue.icu

@functools.lru_cache(maxsize=None)
来源：http://knm.gogol.net.cn

[U21] Py：自定义上下文管理器
来源：http://bkn.hammf.cn

@contextlib.contextmanager
来源：http://oyw.hnxiangtu.top

[U22] Py：矩阵转置
来源：http://tqd.yueranfly.top

list(zip(*m))
来源：http://eun.guannengcc.top

[U23] Py：分块读取大文件
来源：http://srq.hongshengwenyu.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fvg.jianghu66.top

[U24] Py：路径操作
来源：http://zqh.guannengcc.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://sru.fanxiaobao.xyz

[U25] Py：CSV 按字典读
来源：http://sho.gaohongyu789.top

csv.DictReader(f)
来源：http://cck.xingfuxueyuan.xyz

[U26] Py：并发下载
来源：http://uei.shangyingyoupin.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://peq.fengsongda.top

[U27] Py：异步 HTTP
来源：http://iug.jyoumei.cn

aiohttp.ClientSession() 配合 async with
来源：http://cjo.dashuyun.cn

[U28] Py：类型别名
来源：http://qtv.guowangkeji.top

UserId = int
来源：http://uda.nanxuanxn.top

[U29] Py：属性校验
来源：http://zjm.zhongyouzk.top

@property 与 @x.setter 配合
来源：http://kqu.sysykeji.top

[U30] Py：数据类
来源：http://ozj.wangdashe.top

@dataclass(slots=True)
来源：http://ymw.jinghuilouyu.cn

[U31] Py：单测
来源：http://pba.cqqwz.cn

python -m pytest -q
来源：http://zeb.c1oappe.top

[U32] Py：代码格式化
来源：http://cbm.gogol.net.cn

ruff format . && ruff check --fix .
来源：http://wlt.kuanghao11.cn

[U33] Py：打包发布
来源：http://yzz.tianlin.xyz

python -m build  （依赖 pyproject.toml）
来源：http://zyu.zhongyouzk.top

[U34] Py：判断编码
来源：http://vsb.ybcxt.top

chardet.detect(raw)
来源：http://zhu.cheryme.top

[U35] Py：发送邮件
来源：http://pnm.jqgufenzy.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fzj.52xcode.cn

[U36] Py：定时任务
来源：http://ksa.cashguo.top

schedule.every(10).minutes.do(job)
来源：http://arl.ydjk.org.cn

[U37] Py：读写 Excel
来源：http://kjx.guannengcc.top

pandas.read_excel / DataFrame.to_excel
来源：http://img.jlsjyb.cn

[U38] Py：获取脚本所在目录
来源：http://mje.jinqigufen.top

Path(__file__).resolve().parent
来源：http://wfi.jqgufenzy.top

[U39] Py：判断是否在交互环境
来源：http://clm.316326.xyz

sys.stdout.isatty()
来源：http://zpz.zhijiandao.cn

[U40] Py：打印到标准错误
来源：http://vnv.yfazqb.com

print("err", file=sys.stderr)
来源：http://enk.zhaomingkeji.xyz

[U41] PHP：初始化 Composer 项目
来源：http://roy.wangshuangyany.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://wxa.quarkkingdee.top

[U42] PHP：PSR-4 自动加载
来源：http://baz.hysaishi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://onl.guannengcc.top

[U43] PHP：声明命名空间
来源：http://pjz.xuetiantiany.cn

namespace App\Http;
来源：http://vow.shzxlz.cn

[U44] PHP：开启严格类型
来源：http://byd.zdbjq.cn

declare(strict_types=1);
来源：http://kff.fanxiaobao.xyz

[U45] PHP：类型声明与返回类型
来源：http://oae.nanxinkj.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://txm.birdmap.top

[U46] PHP：可空类型
来源：http://avh.gzhubu.top

?string $name = null
来源：http://mnx.kuanghao11.cn

[U47] PHP：联合类型
来源：http://pea.hcnkem.com

int|string $id
来源：http://egk.birdmap.top

[U48] PHP：纯枚举
来源：http://pqx.aizwys.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nev.daxiang520.top

[U49] PHP：只读属性
来源：http://hfq.epnwcf.com

public readonly string $name
来源：http://vnk.yuanzhike.top

[U50] PHP：构造器属性提升
来源：http://oha.tianlin.xyz

public function __construct(private int $id) {}
来源：http://yxq.chenzaomai.com

[U51] PHP：数组解构
来源：http://xpb.pengpengdd.cyou

[$a, $b] = $arr;
来源：http://wcz.jinqigufen.top

[U52] PHP：箭头函数
来源：http://pvx.hcnkem.com

$double = fn($x) => $x * 2;
来源：http://xso.zhengqikj.top

[U53] PHP：空合并运算符
来源：http://azq.hongshengwenyu.top

$v = $a ?? $b ?? "default";
来源：http://dnt.316326.xyz

[U54] PHP：空安全调用
来源：http://gyp.ppjwa.cn

$obj?->method()
来源：http://scf.aibaodan.cn

[U55] PHP：match 表达式
来源：http://cwb.xziqi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tnp.316326.xyz

[U56] PHP：命名参数
来源：http://oit.haohaochexian.top

f(a: 1, b: 2)
来源：http://dhx.xuanzx.com

[U57] PHP：字符串插值
来源：http://ehw.ywan-chungtsiang.top

"值: {$a}"
来源：http://lyh.nwbrower.top

[U58] PHP：数组三件套
来源：http://mhi.xuetiantiany.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://yqp.nwbrower.top

[U59] PHP：自定义排序
来源：http://yzy.yanxiufei.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vpd.svipenyu.cn

[U60] PHP：JSON 编解码
来源：http://qji.fehbvm.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://its.gzhubu.top

[U61] PHP：正则
来源：http://jca.9152youxi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hyz.xuanzx.com

[U62] PHP：日期对象
来源：http://ixq.tanke756.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ubr.jianghu66.top

[U63] PHP：文件读写
来源：http://jzv.cqqwz.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xda.yvedp.cn

[U64] PHP：目录遍历
来源：http://zjt.svipenyu.cn

glob("dir/*.php");  scandir("dir");
来源：http://eeo.ppjwa.cn

[U65] PHP：会话
来源：http://yhf.jqgfzy.top

session_start();  $_SESSION["uid"] = 1;
来源：http://yau.kuanghao11.cn

[U66] PHP：设置 Cookie
来源：http://bxt.yanxiufei.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://eet.nanxuanxn.top

[U67] PHP：处理文件上传
来源：http://wzp.nanxinkj.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jfo.hongshengwenyu.top

[U68] PHP：PDO 连接
来源：http://qua.bjfxy.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hnu.yonumen.top

[U69] PHP：PDO 预处理
来源：http://dsl.dianchejie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ibl.fehbvm.com

[U70] PHP：PDO 事务
来源：http://dlc.jinqigfzy.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://yef.yj20258888.top

[U71] PHP：抛出异常
来源：http://gwf.dianchejie.cn

throw new RuntimeException("失败", 500);
来源：http://oet.tanke756.top

[U72] PHP：写错误日志
来源：http://uwf.fzhhl.top

error_log("失败: " . $e->getMessage());
来源：http://obe.nanxinkj.top

[U73] PHP：读取 ini 配置
来源：http://zhw.sufxvd.cn

parse_ini_file("config.ini", true)
来源：http://bvu.hammf.cn

[U74] PHP：读取环境变量
来源：http://tkg.sxryk.cn

getenv("APP_ENV") ?: "production"
来源：http://hbq.zycfv.cn

[U75] PHP：依赖注入
来源：http://rtz.yuanzhike.top

composer require psr/container
来源：http://mtq.yuanzhike.top

[U76] PHP：简单路由
来源：http://nfw.gotoacloud.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wjd.havefunace.top

[U77] PHP：模板渲染
来源：http://jio.xuanzx.com

composer require twig/twig
来源：http://hhg.ywan-chungtsiang.top

[U78] PHP：单元测试
来源：http://qwi.sysykeji.top

composer require --dev phpunit/phpunit
来源：http://pda.daxiang520.top

[U79] PHP：静态分析
来源：http://ucs.sysykeji.top

composer require --dev phpstan/phpstan
来源：http://mpy.xinyue.icu

[U80] PHP：代码规范修复
来源：http://zgp.yj202588.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://dpf.fzhhl.top

[U81] JS：初始化项目
来源：http://qfs.hongshengwenyu.top

npm init -y;  npm i express
来源：http://kgq.pengpengdd.cyou

[U82] JS：package.json 脚本
来源：http://lhx.yueranfly.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gfm.ybcxt.top

[U83] JS：ES Module 导入导出
来源：http://rxj.ybcxt.top

export const a = 1;  import { a } from "./m.js";
来源：http://hqu.bjfxy.top

[U84] JS：CommonJS 写法
来源：http://ztr.tianlin.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://itq.aibaodan.cn

[U85] JS：可选链
来源：http://vlg.fengsongda.top

a?.b?.c
来源：http://jbc.epnwcf.com

[U86] JS：空值合并
来源：http://zza.jinqigfzy.top

a ?? b
来源：http://psf.316326.xyz

[U87] JS：解构默认值
来源：http://iyn.shanyushiyangtech.top

const { a = 1, b = 2 } = obj;
来源：http://czn.hongshengwenyu.top

[U88] JS：对象展开合并
来源：http://zdi.daria6918.cn

{ ...a, ...b }
来源：http://tmk.gaohongyu789.top


<!-- 参考信息 -->