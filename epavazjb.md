代发 wailian999

[T01] Kotlin：Hello World
来源：http://kae.0kj1m.cn

println("Hello")
来源：http://gbc.hcnkem.com

[T02] Kotlin：变量
来源：http://afg.jiagoushi.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://plr.xylfe.cn

[T03] Kotlin：字符串模板
来源：http://eej.zhiwuduotai.top

"值: $b"
来源：http://nwm.sweek.top

[T04] Kotlin：空安全
来源：http://qwh.aizwys.cn

val n: String? = null;  n?.length
来源：http://eyo.feifeiyinyue.top

[T05] Kotlin：when 表达式
来源：http://opz.jqgufenzy.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fmn.9152youxi.cn

[T06] Kotlin：集合映射
来源：http://lhj.fktsv.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://wsl.jinyuanbaomall.cn

[T07] Kotlin：集合过滤
来源：http://dnz.tarul.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ywk.yj20258888.top

[T08] Kotlin：数据类
来源：http://wcp.sweek.top

data class User(val name: String, val age: Int)
来源：http://jgz.cdnleiting.top

[T09] Kotlin：扩展函数
来源：http://zuo.vehdjk.com

fun String.exclaim() = this + "!"
来源：http://hva.jlsjyb.cn

[T10] Kotlin：默认参数
来源：http://xqd.dianchejie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://xfw.hysaishi.cn

[T11] Kotlin：协程
来源：http://pmw.yangfankeji.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://fun.jlsjyb.cn

[T12] Kotlin：解构声明
来源：http://fal.jyoumei.cn

val (a, b) = Pair(1, 2)
来源：http://cxv.havefunace.top

[T13] Kotlin：只读 Map
来源：http://abz.zdqjudy.top

val m = mapOf("a" to 1)
来源：http://fqb.zdqjudy.top

[T14] Kotlin：循环
来源：http://gxs.jinqigufen.top

for (i in 1..10) println(i)
来源：http://hup.jinqigfzy.top

[T15] Kotlin：接口
来源：http://rfl.xingfuxueyuan.xyz

interface Shape { fun area(): Double }
来源：http://ppx.52xcode.cn

[T16] Swift：Hello World
来源：http://hae.zhengqikj.top

print("Hello")
来源：http://roj.hfpthk.cn

[T17] Swift：变量与常量
来源：http://gec.tanke756.top

var a = 1;  let b = 2
来源：http://rsm.52xcode.cn

[T18] Swift：字符串插值
来源：http://knx.cqqwz.cn

"值: \(b)"
来源：http://vum.fengsongda.top

[T19] Swift：可选绑定
来源：http://boe.shanyushiyangtech.top

if let n = opt { print(n) }
来源：http://wsd.zhengqikj.top

[T20] Swift：数组操作
来源：http://hkg.yj20258888.top

var a = [1, 2, 3];  a.append(4)
来源：http://tam.zdqjudy.top

[T21] Swift：遍历
来源：http://bkn.ybcxt.top

for x in a { print(x) }
来源：http://vuy.aibaodan.cn

[T22] Swift：字典
来源：http://hpo.dianchejie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ofn.wangdashe.top

[T23] Swift：函数
来源：http://ssw.gogol.net.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://sur.tian-w.cn

[T24] Swift：闭包
来源：http://ind.hnqzz.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://vuw.ydjk.org.cn

[T25] Swift：结构体
来源：http://foc.shangyingyoupin.top

struct P { var x: Int }
来源：http://ugd.jyoumei.cn

[T26] Swift：类与重写
来源：http://fww.iojbl.cn

class A: Base { override func f() {} }
来源：http://czs.ehwqpu.com

[T27] Swift：错误处理
来源：http://cek.hnxiangtu.top

do { try f() } catch { print(error) }
来源：http://hmg.tian-w.cn

[T28] Swift：枚举
来源：http://dub.c1oappe.top

enum Color { case red, green }
来源：http://ddr.vqdsnc.cn

[T29] Swift：guard 提前返回
来源：http://iwn.fzhhl.top

guard let x = opt else { return }
来源：http://wco.zhongyouzk.top

[T30] Swift：协议
来源：http://jwm.xinyue.icu

protocol Shape { func area() -> Double }
来源：http://yfy.fanxiaobao.xyz

[T31] Lua：Hello World
来源：http://npv.ybcxt.top

print("Hello")
来源：http://opl.xziqi.cn

[T32] Lua：局部变量
来源：http://ten.feifeiyinyue.top

local a = 1
来源：http://nbu.jiagoushi.top

[T33] Lua：表（数组）
来源：http://bvl.fktsv.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://tpi.wangshuangyany.cn

[T34] Lua：遍历表
来源：http://djo.ctjpmb.com

for i, v in ipairs(t) do print(i, v) end
来源：http://pcu.cashguo.top

[T35] Lua：字典表
来源：http://hpg.xziqi.cn

local d = { a = 1 };  d.b = 2
来源：http://bti.gogol.net.cn

[T36] Lua：函数
来源：http://anp.guowangkeji.top

function add(a, b) return a + b end
来源：http://fmw.xziqi.cn

[T37] Lua：字符串拼接
来源：http://pth.shzxlz.cn

"a" .. "b"
来源：http://lku.tianlin.xyz

[T38] Lua：条件
来源：http://nkw.zhixingplan.top

if x > 0 then print("正") end
来源：http://rge.jinyuanbaomall.cn

[T39] Lua：模式匹配
来源：http://uce.jinghuilouyu.cn

string.find(s, "%d+")
来源：http://lyw.gotoacloud.top

[T40] Lua：元表
来源：http://lux.sweek.top

setmetatable({}, { __index = base })
来源：http://kqw.fktsv.cn

[T41] Perl：Hello World
来源：http://ibk.ppjwa.cn

print "Hello\n";
来源：http://lpf.yj202588.top

[T42] Perl：变量类型
来源：http://kto.dashuyun.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zuf.chenjidiqi.icu

[T43] Perl：字符串插值
来源：http://mgk.aibaodan.cn

"值: $a"
来源：http://wla.c1oappe.top

[T44] Perl：条件
来源：http://gvo.zhoulong.xyz

if ($a > 0) { print "正"; }
来源：http://lyj.mhx1999.top

[T45] Perl：数组遍历
来源：http://gfr.xylfe.cn

for my $x (@arr) { print $x; }
来源：http://ebk.bjfxy.top

[T46] Perl：哈希操作
来源：http://gjs.xuanzx.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ptl.zdbjq.cn

[T47] Perl：正则捕获
来源：http://mpe.xylfe.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://blu.wangshuangyany.cn

[T48] Perl：正则替换
来源：http://ana.havefunace.top

$s =~ s/old/new/g;
来源：http://ytx.bjfxy.top

[T49] Perl：函数
来源：http://acq.xinyue.icu

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hgj.fehbvm.com

[T50] Perl：逐行读文件
来源：http://mro.hnqzz.top

open my $fh, "<", "a.txt" or die $!;
来源：http://xmo.hfpthk.cn

while (my $line = <$fh>) { print $line; }
来源：http://cet.guowangkeji.top

[T51] Scala：Hello World
来源：http://xcc.zdqjudy.top

println("Hello")
来源：http://ymw.xziqi.cn

[T52] Scala：变量
来源：http://awn.snrcjt.cn

val a = 1;  var b = 2
来源：http://kjv.fanxiaobao.xyz

[T53] Scala：字符串插值
来源：http://pxk.shangyingyoupin.top

s"值: $b"
来源：http://cnz.yuxming.cn

[T54] Scala：集合映射
来源：http://jys.yj202588.top

List(1, 2, 3).map(_ * 2)
来源：http://ucy.aibaodan.cn

[T55] Scala：集合过滤
来源：http://hvl.tian-w.cn

List(1, 2, 3).filter(_ > 1)
来源：http://hyh.xuanzx.com

[T56] Scala：样例类
来源：http://wtt.0kj1m.cn

case class User(name: String, age: Int)
来源：http://bzh.hnqzz.top

[T57] Scala：模式匹配
来源：http://egp.bbcook.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://meb.hnqzz.top

[T58] Scala：函数定义
来源：http://rcm.smart0.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://bvz.yanxiufei.cn

[T59] Scala：循环
来源：http://auo.yueranfly.top

for (i <- 1 to 10) println(i)
来源：http://byh.zhoulong.xyz

[T60] Scala：折叠
来源：http://shu.cheryme.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vbl.zhaomingkeji.xyz

================================================================================
来源：http://mct.havefunace.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vui.meibo888.top

================================================================================
来源：http://zbf.ctjpmb.com

[U01] Py：创建虚拟环境
来源：http://uih.tanke756.top

python -m venv .venv && source .venv/bin/activate
来源：http://asb.yanxiufei.cn

[U02] Py：导出 / 安装依赖
来源：http://eda.chenzaomai.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rqp.cqqwz.cn

[U03] Py：加载 .env 配置
来源：http://fki.hesvh.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://awy.ydjk.org.cn

[U04] Py：变量调试打印
来源：http://gkh.smart0.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://cwc.gogol.net.cn

[U05] Py：列表去重且保序
来源：http://ufu.yj20258888.top

list(dict.fromkeys(arr))
来源：http://mbj.vqdsnc.cn

[U06] Py：合并两个字典
来源：http://qpz.jlsjyb.cn

{**a, **b}
来源：http://dlv.iojbl.cn

[U07] Py：反转字典键值
来源：http://rfi.chenjidiqi.icu

{v: k for k, v in d.items()}
来源：http://dyc.mhx1999.top

[U08] Py：展平二维列表
来源：http://afi.nwbrower.top

[y for x in nested for y in x]
来源：http://ouy.cheryme.top

[U09] Py：字典取最大值的键
来源：http://cya.shanyushiyangtech.top

max(d, key=d.get)
来源：http://dun.yj20258888.top

[U10] Py：按值排序字典
来源：http://onb.ehwqpu.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lea.quarkkingdee.top

[U11] Py：生成器表达式
来源：http://ovj.zdqjudy.top

(x * 2 for x in arr)
来源：http://plr.jinqigfzy.top

[U12] Py：取出现最多的 3 个元素
来源：http://mau.andypj.xyz

Counter(arr).most_common(3)
来源：http://nzj.fanxiaobao.xyz

[U13] Py：固定长度队列
来源：http://ctl.uphjek.com

deque(maxlen=10)
来源：http://ntz.mhx1999.top

[U14] Py：分组收集到列表
来源：http://rna.zhengqikj.top

defaultdict(list)
来源：http://npq.ywan-chungtsiang.top

[U15] Py：高精度计时
来源：http://ppn.zhiwuduotai.top

t = time.perf_counter()
来源：http://ntw.jinghuilouyu.cn

[U16] Py：命令行参数解析
来源：http://vbf.meibo888.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mff.cashguo.top

[U17] Py：初始化日志
来源：http://rdc.yongpay.top

logging.basicConfig(level=logging.INFO)
来源：http://hmo.yanxiufei.cn

[U18] Py：预编译正则
来源：http://oli.quarkkingdee.top

pat = re.compile(r"\d+")
来源：http://bjy.zhengqikj.top

[U19] Py：正则替换带回调
来源：http://vcn.zhongyouzk.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hjc.wangshuangyany.cn

[U20] Py：缓存函数结果
来源：http://uqd.jiagoushi.top

@functools.lru_cache(maxsize=None)
来源：http://zey.jinqigufen.top

[U21] Py：自定义上下文管理器
来源：http://yxh.dianchejie.cn

@contextlib.contextmanager
来源：http://opu.316326.xyz

[U22] Py：矩阵转置
来源：http://ule.zycfv.cn

list(zip(*m))
来源：http://kkd.zhijiandao.cn

[U23] Py：分块读取大文件
来源：http://rfw.jinyuanbaomall.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bfv.hammf.cn

[U24] Py：路径操作
来源：http://vls.smart0.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xtm.jinyuanbaomall.cn

[U25] Py：CSV 按字典读
来源：http://wlo.fktsv.cn

csv.DictReader(f)
来源：http://hwq.shuidangran.top

[U26] Py：并发下载
来源：http://let.hongshengwenyu.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://aln.ybcxt.top

[U27] Py：异步 HTTP
来源：http://crp.jiagoushi.top

aiohttp.ClientSession() 配合 async with
来源：http://egu.bbcook.cn

[U28] Py：类型别名
来源：http://jcp.guannengcc.top

UserId = int
来源：http://tbz.snrcjt.cn

[U29] Py：属性校验
来源：http://mcb.xziqi.cn

@property 与 @x.setter 配合
来源：http://gfl.zhaomingkeji.xyz

[U30] Py：数据类
来源：http://tky.yonumen.top

@dataclass(slots=True)
来源：http://wki.jqgufenzy.top

[U31] Py：单测
来源：http://rhv.bjfxy.top

python -m pytest -q
来源：http://gtv.ppjwa.cn

[U32] Py：代码格式化
来源：http://hqg.jyoumei.cn

ruff format . && ruff check --fix .
来源：http://xgm.sufxvd.cn

[U33] Py：打包发布
来源：http://ews.daxiang520.top

python -m build  （依赖 pyproject.toml）
来源：http://gtu.zhijiandao.cn

[U34] Py：判断编码
来源：http://ene.mhx1999.top

chardet.detect(raw)
来源：http://brs.chenjidiqi.icu

[U35] Py：发送邮件
来源：http://xfl.andypj.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://usd.tarul.cn

[U36] Py：定时任务
来源：http://ayb.ywan-chungtsiang.top

schedule.every(10).minutes.do(job)
来源：http://rkt.kuanghao11.cn

[U37] Py：读写 Excel
来源：http://blw.jinghuilouyu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://qrc.shanyushiyangkeji.top

[U38] Py：获取脚本所在目录
来源：http://ieu.dashuyun.cn

Path(__file__).resolve().parent
来源：http://qgp.jinghuilouyu.cn

[U39] Py：判断是否在交互环境
来源：http://gww.zhiwuduotai.top

sys.stdout.isatty()
来源：http://vku.kuanghao11.cn

[U40] Py：打印到标准错误
来源：http://zzw.gaohongyu789.top

print("err", file=sys.stderr)
来源：http://zxq.wangshuangyany.cn

[U41] PHP：初始化 Composer 项目
来源：http://gtg.cqqwz.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://hfy.hcnkem.com

[U42] PHP：PSR-4 自动加载
来源：http://jlz.bbcook.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tgx.smart0.xyz

[U43] PHP：声明命名空间
来源：http://wov.yj202588.top

namespace App\Http;
来源：http://gmi.haohaochexian.top

[U44] PHP：开启严格类型
来源：http://sva.dashuyun.cn

declare(strict_types=1);
来源：http://zaz.wangshuangyany.cn

[U45] PHP：类型声明与返回类型
来源：http://zpg.bbcook.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://jci.yvedp.cn

[U46] PHP：可空类型
来源：http://cfs.xingfuxueyuan.xyz

?string $name = null
来源：http://bwk.cashguo.top

[U47] PHP：联合类型
来源：http://lui.uphjek.com

int|string $id
来源：http://bew.yj20258888.top

[U48] PHP：纯枚举
来源：http://fno.xziqi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kov.yj20258.top

[U49] PHP：只读属性
来源：http://xet.dianchejie.cn

public readonly string $name
来源：http://tby.sjlbkw.cn

[U50] PHP：构造器属性提升
来源：http://poc.xinyue.icu

public function __construct(private int $id) {}
来源：http://vks.cdnleiting.top

[U51] PHP：数组解构
来源：http://nsa.52xcode.cn

[$a, $b] = $arr;
来源：http://ptr.bbcook.cn

[U52] PHP：箭头函数
来源：http://qei.yonumen.top

$double = fn($x) => $x * 2;
来源：http://wlh.aizwys.cn

[U53] PHP：空合并运算符
来源：http://bxc.haohaochexian.top

$v = $a ?? $b ?? "default";
来源：http://ath.tarul.cn

[U54] PHP：空安全调用
来源：http://onr.yonumen.top

$obj?->method()
来源：http://yfn.cashguo.top

[U55] PHP：match 表达式
来源：http://wbb.hysaishi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hrf.yueranfly.top

[U56] PHP：命名参数
来源：http://ret.cashguo.top

f(a: 1, b: 2)
来源：http://ooz.hnxiangtu.top

[U57] PHP：字符串插值
来源：http://ajh.zhixingplan.top

"值: {$a}"
来源：http://mlz.chenlongwang.top

[U58] PHP：数组三件套
来源：http://dtr.cqqwz.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zag.quarkkingdee.top

[U59] PHP：自定义排序
来源：http://quw.birdmap.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ewz.fzhhl.top

[U60] PHP：JSON 编解码
来源：http://ace.jinghuilouyu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dgu.shangyingyoupin.top

[U61] PHP：正则
来源：http://lqj.fehbvm.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gsh.ctjpmb.com

[U62] PHP：日期对象
来源：http://ulr.jinyuanbaomall.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vbx.yuanzhike.top

[U63] PHP：文件读写
来源：http://ytc.chenjidiqi.icu

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bfr.yvedp.cn

[U64] PHP：目录遍历
来源：http://krs.zhijiandao.cn

glob("dir/*.php");  scandir("dir");
来源：http://tye.yuxming.cn

[U65] PHP：会话
来源：http://lhg.cheryme.top

session_start();  $_SESSION["uid"] = 1;
来源：http://mmn.yueranfly.top

[U66] PHP：设置 Cookie
来源：http://ylm.sxryk.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jme.zhixingplan.top

[U67] PHP：处理文件上传
来源：http://jfj.vqdsnc.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://enn.xinyue.icu

[U68] PHP：PDO 连接
来源：http://fxh.gzhubu.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pva.xziqi.cn

[U69] PHP：PDO 预处理
来源：http://fmb.haohaochexian.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ayd.mhx1999.top

[U70] PHP：PDO 事务
来源：http://nrp.dashuyun.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://utf.xziqi.cn

[U71] PHP：抛出异常
来源：http://qic.chenlongwang.top

throw new RuntimeException("失败", 500);
来源：http://ugf.vehdjk.com

[U72] PHP：写错误日志
来源：http://dbt.quarkkingdee.top

error_log("失败: " . $e->getMessage());
来源：http://lje.guowangkeji.top

[U73] PHP：读取 ini 配置
来源：http://bjg.aibaodan.cn

parse_ini_file("config.ini", true)
来源：http://lji.52xcode.cn

[U74] PHP：读取环境变量
来源：http://cwu.shanyushiyangkeji.top

getenv("APP_ENV") ?: "production"
来源：http://nkc.zhiwuduotai.top

[U75] PHP：依赖注入
来源：http://cia.ppjwa.cn

composer require psr/container
来源：http://qbp.zhongyouzk.top

[U76] PHP：简单路由
来源：http://iaq.52xcode.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hul.guannengcc.top

[U77] PHP：模板渲染
来源：http://dme.aibaodan.cn

composer require twig/twig
来源：http://ocn.hnxiangtu.top

[U78] PHP：单元测试
来源：http://wdw.jqgfzy.top

composer require --dev phpunit/phpunit
来源：http://vga.redwolf501.top

[U79] PHP：静态分析
来源：http://ade.nanxinkj.top

composer require --dev phpstan/phpstan
来源：http://glz.andypj.xyz

[U80] PHP：代码规范修复
来源：http://gee.wangdashe.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://irg.hesvh.cn

[U81] JS：初始化项目
来源：http://nya.sufxvd.cn

npm init -y;  npm i express
来源：http://qvr.gzhubu.top

[U82] JS：package.json 脚本
来源：http://rvt.quarkkingdee.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://icv.zhaomingkeji.xyz

[U83] JS：ES Module 导入导出
来源：http://bqu.xinyue.icu

export const a = 1;  import { a } from "./m.js";
来源：http://kkx.hcnkem.com

[U84] JS：CommonJS 写法
来源：http://kwm.zhoulong.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://pmf.iojbl.cn

[U85] JS：可选链
来源：http://eyo.jinqigfzy.top

a?.b?.c
来源：http://sro.zdbjq.cn

[U86] JS：空值合并
来源：http://rut.dashuyun.cn

a ?? b
来源：http://ocz.gogol.net.cn

[U87] JS：解构默认值
来源：http://ozd.yj20258888.top

const { a = 1, b = 2 } = obj;
来源：http://xbu.pycfn.com

[U88] JS：对象展开合并
来源：http://fmn.ppjwa.cn

{ ...a, ...b }
来源：http://wgr.nwbrower.top


<!-- 参考信息 -->