代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xje.xziqi.cn

================================================================================
来源：http://vqy.tian-w.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mhb.tarul.cn

================================================================================
来源：http://zdi.zdqjudy.top

[T01] Kotlin：Hello World
来源：http://egi.cdnleiting.top

println("Hello")
来源：http://lai.hnqzz.top

[T02] Kotlin：变量
来源：http://opq.sysykeji.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dak.uphjek.com

[T03] Kotlin：字符串模板
来源：http://prz.jyoumei.cn

"值: $b"
来源：http://nlm.xuetiantiany.cn

[T04] Kotlin：空安全
来源：http://uwe.hnxiangtu.top

val n: String? = null;  n?.length
来源：http://ucb.smart0.xyz

[T05] Kotlin：when 表达式
来源：http://fbd.jlsjyb.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jiv.aizwys.cn

[T06] Kotlin：集合映射
来源：http://afk.0kj1m.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://bdh.zhengqikj.top

[T07] Kotlin：集合过滤
来源：http://upk.cashguo.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ooq.xziqi.cn

[T08] Kotlin：数据类
来源：http://txj.jianghu66.top

data class User(val name: String, val age: Int)
来源：http://xgm.yangfankeji.com

[T09] Kotlin：扩展函数
来源：http://vix.kuanghao11.cn

fun String.exclaim() = this + "!"
来源：http://geb.jianghu66.top

[T10] Kotlin：默认参数
来源：http://jzm.nwbrower.top

fun greet(name: String = "World") = "Hi $name"
来源：http://dqv.xziqi.cn

[T11] Kotlin：协程
来源：http://wli.shuidangran.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://aqs.yfazqb.com

[T12] Kotlin：解构声明
来源：http://uyg.gaohongyu789.top

val (a, b) = Pair(1, 2)
来源：http://btn.jinqigfzy.top

[T13] Kotlin：只读 Map
来源：http://grm.xziqi.cn

val m = mapOf("a" to 1)
来源：http://isj.xuetiantiany.cn

[T14] Kotlin：循环
来源：http://hza.yj20258888.top

for (i in 1..10) println(i)
来源：http://hbr.sjlbkw.cn

[T15] Kotlin：接口
来源：http://yme.birdmap.top

interface Shape { fun area(): Double }
来源：http://kls.jinqigfzy.top

[T16] Swift：Hello World
来源：http://qvt.52xcode.cn

print("Hello")
来源：http://rwd.jiagoushi.top

[T17] Swift：变量与常量
来源：http://euq.gotoacloud.top

var a = 1;  let b = 2
来源：http://zni.zdbjq.cn

[T18] Swift：字符串插值
来源：http://gjz.ppjwa.cn

"值: \(b)"
来源：http://yag.hfpthk.cn

[T19] Swift：可选绑定
来源：http://vay.zhengqikj.top

if let n = opt { print(n) }
来源：http://fat.yj202588.top

[T20] Swift：数组操作
来源：http://qty.ppjwa.cn

var a = [1, 2, 3];  a.append(4)
来源：http://pia.yfazqb.com

[T21] Swift：遍历
来源：http://zsh.aibaodan.cn

for x in a { print(x) }
来源：http://zgi.hammf.cn

[T22] Swift：字典
来源：http://egt.dashuyun.cn

var d = ["a": 1];  d["b"] = 2
来源：http://rzf.cqqwz.cn

[T23] Swift：函数
来源：http://xho.zhongyouzk.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fdr.xziqi.cn

[T24] Swift：闭包
来源：http://yeb.fzhhl.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://vgo.zdqjudy.top

[T25] Swift：结构体
来源：http://mkf.tarul.cn

struct P { var x: Int }
来源：http://ocl.tianlin.xyz

[T26] Swift：类与重写
来源：http://qdm.ivvv.top

class A: Base { override func f() {} }
来源：http://xxs.hongshengwenyu.top

[T27] Swift：错误处理
来源：http://eep.zdqjudy.top

do { try f() } catch { print(error) }
来源：http://jaf.tian-w.cn

[T28] Swift：枚举
来源：http://zpf.sjlbkw.cn

enum Color { case red, green }
来源：http://ish.aibaodan.cn

[T29] Swift：guard 提前返回
来源：http://wwu.dashuyun.cn

guard let x = opt else { return }
来源：http://prv.xziqi.cn

[T30] Swift：协议
来源：http://xbz.zhaomingkeji.xyz

protocol Shape { func area() -> Double }
来源：http://wie.c1oappe.top

[T31] Lua：Hello World
来源：http://zum.tian-w.cn

print("Hello")
来源：http://cmw.yj202588.top

[T32] Lua：局部变量
来源：http://kps.shuidangran.top

local a = 1
来源：http://ujt.zhaomingkeji.xyz

[T33] Lua：表（数组）
来源：http://zxg.zhixingplan.top

local t = {1, 2, 3};  t[4] = 4
来源：http://wml.sysykeji.top

[T34] Lua：遍历表
来源：http://kra.aibaodan.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://wfo.shzxlz.cn

[T35] Lua：字典表
来源：http://lof.jinqigfzy.top

local d = { a = 1 };  d.b = 2
来源：http://uvf.cheryme.top

[T36] Lua：函数
来源：http://uhw.9152youxi.cn

function add(a, b) return a + b end
来源：http://rsm.vehdjk.com

[T37] Lua：字符串拼接
来源：http://lhf.bbcook.cn

"a" .. "b"
来源：http://shy.snrcjt.cn

[T38] Lua：条件
来源：http://kyp.jinqigufen.top

if x > 0 then print("正") end
来源：http://mtp.shangyingyoupin.top

[T39] Lua：模式匹配
来源：http://jaj.yanxiufei.cn

string.find(s, "%d+")
来源：http://phd.cashguo.top

[T40] Lua：元表
来源：http://cqe.yanxiufei.cn

setmetatable({}, { __index = base })
来源：http://kfc.cdnleiting.top

[T41] Perl：Hello World
来源：http://qst.bjfxy.top

print "Hello\n";
来源：http://hcu.316326.xyz

[T42] Perl：变量类型
来源：http://kri.zdbjq.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nus.hammf.cn

[T43] Perl：字符串插值
来源：http://xhh.fanxiaobao.xyz

"值: $a"
来源：http://dxv.shuidangran.top

[T44] Perl：条件
来源：http://klt.bjfxy.top

if ($a > 0) { print "正"; }
来源：http://pqa.guannengcc.top

[T45] Perl：数组遍历
来源：http://sva.dianchejie.cn

for my $x (@arr) { print $x; }
来源：http://lin.ywan-chungtsiang.top

[T46] Perl：哈希操作
来源：http://nab.quarkkingdee.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dea.chenjidiqi.icu

[T47] Perl：正则捕获
来源：http://bld.sjlbkw.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://nld.zdbjq.cn

[T48] Perl：正则替换
来源：http://zak.zhengqikj.top

$s =~ s/old/new/g;
来源：http://rug.jyoumei.cn

[T49] Perl：函数
来源：http://bda.sxryk.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pom.zhiwuduotai.top

[T50] Perl：逐行读文件
来源：http://obf.kuanghao11.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://swh.hywenlv.cn

while (my $line = <$fh>) { print $line; }
来源：http://oio.uphjek.com

[T51] Scala：Hello World
来源：http://rml.sweek.top

println("Hello")
来源：http://foh.bjfxy.top

[T52] Scala：变量
来源：http://rrm.bbcook.cn

val a = 1;  var b = 2
来源：http://ldb.snrcjt.cn

[T53] Scala：字符串插值
来源：http://pvz.shzxlz.cn

s"值: $b"
来源：http://wgy.cheryme.top

[T54] Scala：集合映射
来源：http://pxb.dianchejie.cn

List(1, 2, 3).map(_ * 2)
来源：http://mwl.tian-w.cn

[T55] Scala：集合过滤
来源：http://xlr.jinqigfzy.top

List(1, 2, 3).filter(_ > 1)
来源：http://bbe.gzhubu.top

[T56] Scala：样例类
来源：http://fmo.snrcjt.cn

case class User(name: String, age: Int)
来源：http://bov.gaohongyu789.top

[T57] Scala：模式匹配
来源：http://lrs.zhongyouzk.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://nbt.ywan-chungtsiang.top

[T58] Scala：函数定义
来源：http://fac.ehwqpu.com

def add(a: Int, b: Int): Int = a + b
来源：http://dhn.cdnleiting.top

[T59] Scala：循环
来源：http://jqz.meibo888.top

for (i <- 1 to 10) println(i)
来源：http://ygy.0kj1m.cn

[T60] Scala：折叠
来源：http://caw.vqdsnc.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://daq.hysaishi.cn

================================================================================
来源：http://rrc.xinyue.icu

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fly.zhiwuduotai.top

================================================================================
来源：http://ltg.bjfxy.top

[U01] Py：创建虚拟环境
来源：http://epu.gogol.net.cn

python -m venv .venv && source .venv/bin/activate
来源：http://dlr.shanyushiyangkeji.top

[U02] Py：导出 / 安装依赖
来源：http://lzv.sysykeji.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://opr.yj20258.top

[U03] Py：加载 .env 配置
来源：http://dhg.yj20258.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ypx.ybcxt.top

[U04] Py：变量调试打印
来源：http://tdn.aibaodan.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nrn.fengsongda.top

[U05] Py：列表去重且保序
来源：http://fbu.birdmap.top

list(dict.fromkeys(arr))
来源：http://btb.hcnkem.com

[U06] Py：合并两个字典
来源：http://fil.feifeiyinyue.top

{**a, **b}
来源：http://iur.xylfe.cn

[U07] Py：反转字典键值
来源：http://wka.c1oappe.top

{v: k for k, v in d.items()}
来源：http://cqv.haohaochexian.top

[U08] Py：展平二维列表
来源：http://rne.jqgufenzy.top

[y for x in nested for y in x]
来源：http://son.zdbjq.cn

[U09] Py：字典取最大值的键
来源：http://sfi.sufxvd.cn

max(d, key=d.get)
来源：http://nqf.quarkkingdee.top

[U10] Py：按值排序字典
来源：http://vsq.snrcjt.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nmb.52xcode.cn

[U11] Py：生成器表达式
来源：http://dmg.zhongyouzk.top

(x * 2 for x in arr)
来源：http://bcg.tarul.cn

[U12] Py：取出现最多的 3 个元素
来源：http://exx.jqgfzy.top

Counter(arr).most_common(3)
来源：http://qxv.zhengqikj.top

[U13] Py：固定长度队列
来源：http://ttz.ybcxt.top

deque(maxlen=10)
来源：http://xnk.zhijiandao.cn

[U14] Py：分组收集到列表
来源：http://vxq.yuxming.cn

defaultdict(list)
来源：http://hsx.havefunace.top

[U15] Py：高精度计时
来源：http://ide.jlsjyb.cn

t = time.perf_counter()
来源：http://itr.0kj1m.cn

[U16] Py：命令行参数解析
来源：http://mfh.svipenyu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nlk.chenjidiqi.icu

[U17] Py：初始化日志
来源：http://iod.sjlbkw.cn

logging.basicConfig(level=logging.INFO)
来源：http://ljd.tanke756.top

[U18] Py：预编译正则
来源：http://zok.yuxming.cn

pat = re.compile(r"\d+")
来源：http://sev.nanxuanxn.top

[U19] Py：正则替换带回调
来源：http://yvu.andypj.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://typ.c1oappe.top

[U20] Py：缓存函数结果
来源：http://esg.xuanzx.com

@functools.lru_cache(maxsize=None)
来源：http://brp.haohaochexian.top

[U21] Py：自定义上下文管理器
来源：http://qdy.xuetiantiany.cn

@contextlib.contextmanager
来源：http://gdy.jinqigufen.top

[U22] Py：矩阵转置
来源：http://jaw.svipenyu.cn

list(zip(*m))
来源：http://fbi.xuetiantiany.cn

[U23] Py：分块读取大文件
来源：http://qgj.wangdashe.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://isn.ivvv.top

[U24] Py：路径操作
来源：http://inv.9152youxi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://flx.ehwqpu.com

[U25] Py：CSV 按字典读
来源：http://zsr.zhaomingkeji.xyz

csv.DictReader(f)
来源：http://zpv.hnxiangtu.top

[U26] Py：并发下载
来源：http://jpn.dashuyun.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://kmn.gaohongyu789.top

[U27] Py：异步 HTTP
来源：http://fjp.aibaodan.cn

aiohttp.ClientSession() 配合 async with
来源：http://vfq.yonumen.top

[U28] Py：类型别名
来源：http://dut.hnqzz.top

UserId = int
来源：http://wnk.yongpay.top

[U29] Py：属性校验
来源：http://rdt.zhongyouzk.top

@property 与 @x.setter 配合
来源：http://pys.hnxiangtu.top

[U30] Py：数据类
来源：http://agw.hysaishi.cn

@dataclass(slots=True)
来源：http://dwa.shzxlz.cn

[U31] Py：单测
来源：http://mqs.tianlin.xyz

python -m pytest -q
来源：http://gsy.yj20258.top

[U32] Py：代码格式化
来源：http://eqe.gzhubu.top

ruff format . && ruff check --fix .
来源：http://ljf.daria6918.cn

[U33] Py：打包发布
来源：http://trk.ywan-chungtsiang.top

python -m build  （依赖 pyproject.toml）
来源：http://gdf.yuxming.cn

[U34] Py：判断编码
来源：http://lpq.xuanzx.com

chardet.detect(raw)
来源：http://sqt.havefunace.top

[U35] Py：发送邮件
来源：http://stj.yfazqb.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://iku.dashuyun.cn

[U36] Py：定时任务
来源：http://gjb.chenjidiqi.icu

schedule.every(10).minutes.do(job)
来源：http://qlm.yonumen.top

[U37] Py：读写 Excel
来源：http://kru.wangshuangyany.cn

pandas.read_excel / DataFrame.to_excel
来源：http://zzx.dianchejie.cn

[U38] Py：获取脚本所在目录
来源：http://ola.shzxlz.cn

Path(__file__).resolve().parent
来源：http://egg.birdmap.top

[U39] Py：判断是否在交互环境
来源：http://aat.yongpay.top

sys.stdout.isatty()
来源：http://jko.yj202588.top

[U40] Py：打印到标准错误
来源：http://wsj.xylfe.cn

print("err", file=sys.stderr)
来源：http://coq.hnqzz.top

[U41] PHP：初始化 Composer 项目
来源：http://giv.zhaomingkeji.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://tvi.cdnleiting.top

[U42] PHP：PSR-4 自动加载
来源：http://dcr.pycfn.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://sml.ydjk.org.cn

[U43] PHP：声明命名空间
来源：http://xql.gzhubu.top

namespace App\Http;
来源：http://vqb.chenjidiqi.icu

[U44] PHP：开启严格类型
来源：http://jgc.cdnleiting.top

declare(strict_types=1);
来源：http://jeo.redwolf501.top

[U45] PHP：类型声明与返回类型
来源：http://pbu.xylfe.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://qtl.hnxiangtu.top

[U46] PHP：可空类型
来源：http://qfd.pycfn.com

?string $name = null
来源：http://mqe.hywenlv.cn

[U47] PHP：联合类型
来源：http://bey.wangdashe.top

int|string $id
来源：http://vui.pycfn.com

[U48] PHP：纯枚举
来源：http://yci.yuxming.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qgo.shanyushiyangtech.top

[U49] PHP：只读属性
来源：http://plq.bjfxy.top

public readonly string $name
来源：http://dda.zycfv.cn

[U50] PHP：构造器属性提升
来源：http://ogv.nanxuanxn.top

public function __construct(private int $id) {}
来源：http://knv.hysaishi.cn

[U51] PHP：数组解构
来源：http://djn.shanyushiyangtech.top

[$a, $b] = $arr;
来源：http://gkm.gaohongyu789.top

[U52] PHP：箭头函数
来源：http://swr.sjlbkw.cn

$double = fn($x) => $x * 2;
来源：http://mcb.ppjwa.cn

[U53] PHP：空合并运算符
来源：http://swy.fengsongda.top

$v = $a ?? $b ?? "default";
来源：http://lva.nanxuanxn.top

[U54] PHP：空安全调用
来源：http://oms.hcnkem.com

$obj?->method()
来源：http://ona.ybcxt.top

[U55] PHP：match 表达式
来源：http://neg.xylfe.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ekv.hammf.cn

[U56] PHP：命名参数
来源：http://bry.xinyue.icu

f(a: 1, b: 2)
来源：http://zef.sjlbkw.cn

[U57] PHP：字符串插值
来源：http://ygo.jqgufenzy.top

"值: {$a}"
来源：http://olb.zhoulong.xyz

[U58] PHP：数组三件套
来源：http://gou.jqgufenzy.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vdu.c1oappe.top

[U59] PHP：自定义排序
来源：http://eio.zhaomingkeji.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ril.ybcxt.top

[U60] PHP：JSON 编解码
来源：http://skj.shangyingyoupin.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rwv.smart0.xyz

[U61] PHP：正则
来源：http://fwr.nwbrower.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://idv.tanke756.top

[U62] PHP：日期对象
来源：http://bfc.haohaochexian.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gqh.jinqigfzy.top

[U63] PHP：文件读写
来源：http://vzi.iojbl.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qyg.havefunace.top

[U64] PHP：目录遍历
来源：http://pso.zycfv.cn

glob("dir/*.php");  scandir("dir");
来源：http://dia.aizwys.cn

[U65] PHP：会话
来源：http://drx.nanxuanxn.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ygh.meibo888.top

[U66] PHP：设置 Cookie
来源：http://bgr.hcnkem.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://itg.fanxiaobao.xyz

[U67] PHP：处理文件上传
来源：http://mai.havefunace.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gby.chenzaomai.com

[U68] PHP：PDO 连接
来源：http://xos.yj20258.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://isu.chenzaomai.com

[U69] PHP：PDO 预处理
来源：http://asq.zhengqikj.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://asy.hnqzz.top

[U70] PHP：PDO 事务
来源：http://eif.gogol.net.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lzc.cdnleiting.top

[U71] PHP：抛出异常
来源：http://rah.xylfe.cn

throw new RuntimeException("失败", 500);
来源：http://dsv.zdqjudy.top

[U72] PHP：写错误日志
来源：http://jyy.fengsongda.top

error_log("失败: " . $e->getMessage());
来源：http://efh.ywan-chungtsiang.top

[U73] PHP：读取 ini 配置
来源：http://ahk.shanyushiyangtech.top

parse_ini_file("config.ini", true)
来源：http://jgg.zhixingplan.top

[U74] PHP：读取环境变量
来源：http://hfq.52xcode.cn

getenv("APP_ENV") ?: "production"
来源：http://bvi.epnwcf.com

[U75] PHP：依赖注入
来源：http://vev.cqqwz.cn

composer require psr/container
来源：http://zbf.yuanzhike.top

[U76] PHP：简单路由
来源：http://xuj.52xcode.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qrg.gaohongyu789.top

[U77] PHP：模板渲染
来源：http://avc.yongpay.top

composer require twig/twig
来源：http://baw.aizwys.cn

[U78] PHP：单元测试
来源：http://dcg.pycfn.com

composer require --dev phpunit/phpunit
来源：http://mnh.smart0.xyz

[U79] PHP：静态分析
来源：http://sjh.c1oappe.top

composer require --dev phpstan/phpstan
来源：http://vmo.shangyingyoupin.top

[U80] PHP：代码规范修复
来源：http://qhw.bjfxy.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://zmj.ybcxt.top

[U81] JS：初始化项目
来源：http://jdr.ivvv.top

npm init -y;  npm i express
来源：http://rha.fanxiaobao.xyz

[U82] JS：package.json 脚本
来源：http://zvy.ydzc1.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://eil.zhaomingkeji.xyz

[U83] JS：ES Module 导入导出
来源：http://ggc.ivvv.top

export const a = 1;  import { a } from "./m.js";
来源：http://uuo.vqdsnc.cn

[U84] JS：CommonJS 写法
来源：http://meu.chenlongwang.top

module.exports = { a };  const { a } = require("./m");
来源：http://vke.gzhubu.top

[U85] JS：可选链
来源：http://udf.zhaomingkeji.xyz

a?.b?.c
来源：http://ick.tian-w.cn

[U86] JS：空值合并
来源：http://cll.hfpthk.cn

a ?? b
来源：http://tgn.fengsongda.top


<!-- 参考信息 -->