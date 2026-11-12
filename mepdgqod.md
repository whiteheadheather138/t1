代发 wailian999

[T01] Kotlin：Hello World
来源：http://kfb.yonumen.top

println("Hello")
来源：http://uca.tanke756.top

[T02] Kotlin：变量
来源：http://scm.zhoulong.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://msi.gaohongyu789.top

[T03] Kotlin：字符串模板
来源：http://rkx.bjfxy.top

"值: $b"
来源：http://yzt.jqgfzy.top

[T04] Kotlin：空安全
来源：http://pjc.xuetiantiany.cn

val n: String? = null;  n?.length
来源：http://txi.hcnkem.com

[T05] Kotlin：when 表达式
来源：http://vir.zdqjudy.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ghu.hysaishi.cn

[T06] Kotlin：集合映射
来源：http://eto.wangdashe.top

listOf(1, 2, 3).map { it * 2 }
来源：http://fpg.xuanzx.com

[T07] Kotlin：集合过滤
来源：http://zai.shzxlz.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://sca.hfpthk.cn

[T08] Kotlin：数据类
来源：http://dtk.fanxiaobao.xyz

data class User(val name: String, val age: Int)
来源：http://bur.zhiwuduotai.top

[T09] Kotlin：扩展函数
来源：http://vks.zhixingplan.top

fun String.exclaim() = this + "!"
来源：http://cum.hfpthk.cn

[T10] Kotlin：默认参数
来源：http://gpa.nwbrower.top

fun greet(name: String = "World") = "Hi $name"
来源：http://akg.cdnleiting.top

[T11] Kotlin：协程
来源：http://ioh.zhixingplan.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://xao.zhijiandao.cn

[T12] Kotlin：解构声明
来源：http://yko.daria6918.cn

val (a, b) = Pair(1, 2)
来源：http://foe.aibaodan.cn

[T13] Kotlin：只读 Map
来源：http://ifw.yj20258888.top

val m = mapOf("a" to 1)
来源：http://eaf.birdmap.top

[T14] Kotlin：循环
来源：http://sag.tian-w.cn

for (i in 1..10) println(i)
来源：http://dbn.pycfn.com

[T15] Kotlin：接口
来源：http://jfp.hnxiangtu.top

interface Shape { fun area(): Double }
来源：http://xtx.snrcjt.cn

[T16] Swift：Hello World
来源：http://dmq.ivvv.top

print("Hello")
来源：http://qje.iojbl.cn

[T17] Swift：变量与常量
来源：http://shr.xuanzx.com

var a = 1;  let b = 2
来源：http://yyb.316326.xyz

[T18] Swift：字符串插值
来源：http://eql.xuetiantiany.cn

"值: \(b)"
来源：http://llw.guannengcc.top

[T19] Swift：可选绑定
来源：http://lsx.jinghuilouyu.cn

if let n = opt { print(n) }
来源：http://nck.xziqi.cn

[T20] Swift：数组操作
来源：http://kip.hnxiangtu.top

var a = [1, 2, 3];  a.append(4)
来源：http://ziu.kuanghao11.cn

[T21] Swift：遍历
来源：http://oet.feifeiyinyue.top

for x in a { print(x) }
来源：http://mys.hesvh.cn

[T22] Swift：字典
来源：http://zoa.hysaishi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://wxv.chenjidiqi.icu

[T23] Swift：函数
来源：http://etp.svipenyu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ikr.aibaodan.cn

[T24] Swift：闭包
来源：http://pvw.ydjk.org.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xns.yonumen.top

[T25] Swift：结构体
来源：http://yoi.gaohongyu789.top

struct P { var x: Int }
来源：http://tdw.vehdjk.com

[T26] Swift：类与重写
来源：http://mxd.ctjpmb.com

class A: Base { override func f() {} }
来源：http://mpc.yongpay.top

[T27] Swift：错误处理
来源：http://uad.tian-w.cn

do { try f() } catch { print(error) }
来源：http://vpu.yuanzhike.top

[T28] Swift：枚举
来源：http://ska.andypj.xyz

enum Color { case red, green }
来源：http://dwy.zhoulong.xyz

[T29] Swift：guard 提前返回
来源：http://gnc.fengsongda.top

guard let x = opt else { return }
来源：http://blz.shuidangran.top

[T30] Swift：协议
来源：http://gxa.yj20258888.top

protocol Shape { func area() -> Double }
来源：http://hof.fehbvm.com

[T31] Lua：Hello World
来源：http://gxk.sweek.top

print("Hello")
来源：http://goe.sweek.top

[T32] Lua：局部变量
来源：http://gzq.ppjwa.cn

local a = 1
来源：http://lww.zycfv.cn

[T33] Lua：表（数组）
来源：http://ygj.haohaochexian.top

local t = {1, 2, 3};  t[4] = 4
来源：http://bet.sysykeji.top

[T34] Lua：遍历表
来源：http://nmc.gzhubu.top

for i, v in ipairs(t) do print(i, v) end
来源：http://fil.wangshuangyany.cn

[T35] Lua：字典表
来源：http://dnd.birdmap.top

local d = { a = 1 };  d.b = 2
来源：http://pim.zhengqikj.top

[T36] Lua：函数
来源：http://jez.zhoulong.xyz

function add(a, b) return a + b end
来源：http://jqm.yj20258.top

[T37] Lua：字符串拼接
来源：http://otr.epnwcf.com

"a" .. "b"
来源：http://ruh.jqgfzy.top

[T38] Lua：条件
来源：http://kvi.shanyushiyangtech.top

if x > 0 then print("正") end
来源：http://uvp.vqdsnc.cn

[T39] Lua：模式匹配
来源：http://riu.316326.xyz

string.find(s, "%d+")
来源：http://xrs.cdnleiting.top

[T40] Lua：元表
来源：http://ymr.c1oappe.top

setmetatable({}, { __index = base })
来源：http://xsr.andypj.xyz

[T41] Perl：Hello World
来源：http://zyz.jqgfzy.top

print "Hello\n";
来源：http://wyw.xziqi.cn

[T42] Perl：变量类型
来源：http://wqw.yj20258.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hqt.jinghuilouyu.cn

[T43] Perl：字符串插值
来源：http://jto.pengpengdd.cyou

"值: $a"
来源：http://wzi.yfazqb.com

[T44] Perl：条件
来源：http://bom.zdbjq.cn

if ($a > 0) { print "正"; }
来源：http://yyh.yanxiufei.cn

[T45] Perl：数组遍历
来源：http://ucy.jianghu66.top

for my $x (@arr) { print $x; }
来源：http://ajh.sufxvd.cn

[T46] Perl：哈希操作
来源：http://itx.ppjwa.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://btr.ppjwa.cn

[T47] Perl：正则捕获
来源：http://mpl.zhongyouzk.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://jko.shanyushiyangkeji.top

[T48] Perl：正则替换
来源：http://rrq.pycfn.com

$s =~ s/old/new/g;
来源：http://spe.yvedp.cn

[T49] Perl：函数
来源：http://wds.zhengqikj.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vxj.gaohongyu789.top

[T50] Perl：逐行读文件
来源：http://pon.fktsv.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://dcd.cheryme.top

while (my $line = <$fh>) { print $line; }
来源：http://taa.jinghuilouyu.cn

[T51] Scala：Hello World
来源：http://hyj.hfpthk.cn

println("Hello")
来源：http://vyt.yanxiufei.cn

[T52] Scala：变量
来源：http://lxa.yueranfly.top

val a = 1;  var b = 2
来源：http://xtn.hesvh.cn

[T53] Scala：字符串插值
来源：http://ezg.xylfe.cn

s"值: $b"
来源：http://pnz.dashuyun.cn

[T54] Scala：集合映射
来源：http://tqs.tanke756.top

List(1, 2, 3).map(_ * 2)
来源：http://qcr.yvedp.cn

[T55] Scala：集合过滤
来源：http://xuk.epnwcf.com

List(1, 2, 3).filter(_ > 1)
来源：http://mmf.smart0.xyz

[T56] Scala：样例类
来源：http://srh.zhijiandao.cn

case class User(name: String, age: Int)
来源：http://ecc.yonumen.top

[T57] Scala：模式匹配
来源：http://src.vqdsnc.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://huy.vehdjk.com

[T58] Scala：函数定义
来源：http://blb.ydjk.org.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ipg.yonumen.top

[T59] Scala：循环
来源：http://onz.andypj.xyz

for (i <- 1 to 10) println(i)
来源：http://nym.jqgfzy.top

[T60] Scala：折叠
来源：http://mcc.aizwys.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rea.xuetiantiany.cn

================================================================================
来源：http://jkd.c1oappe.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gmf.wangshuangyany.cn

================================================================================
来源：http://fgt.svipenyu.cn

[U01] Py：创建虚拟环境
来源：http://spd.zhengqikj.top

python -m venv .venv && source .venv/bin/activate
来源：http://oze.sufxvd.cn

[U02] Py：导出 / 安装依赖
来源：http://sza.yvedp.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zmy.jinqigufen.top

[U03] Py：加载 .env 配置
来源：http://tlx.ctjpmb.com

from dotenv import load_dotenv; load_dotenv()
来源：http://yan.yuanzhike.top

[U04] Py：变量调试打印
来源：http://aeh.shanyushiyangtech.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ilv.fengsongda.top

[U05] Py：列表去重且保序
来源：http://whn.fanxiaobao.xyz

list(dict.fromkeys(arr))
来源：http://vej.yueranfly.top

[U06] Py：合并两个字典
来源：http://lwq.jlsjyb.cn

{**a, **b}
来源：http://apf.yongpay.top

[U07] Py：反转字典键值
来源：http://kdo.yangfankeji.com

{v: k for k, v in d.items()}
来源：http://jvo.yvedp.cn

[U08] Py：展平二维列表
来源：http://umj.sjlbkw.cn

[y for x in nested for y in x]
来源：http://uaa.yueranfly.top

[U09] Py：字典取最大值的键
来源：http://yau.xziqi.cn

max(d, key=d.get)
来源：http://cvt.aizwys.cn

[U10] Py：按值排序字典
来源：http://wxd.dashuyun.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://car.daria6918.cn

[U11] Py：生成器表达式
来源：http://jyd.tianlin.xyz

(x * 2 for x in arr)
来源：http://vis.tianlin.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://aor.vehdjk.com

Counter(arr).most_common(3)
来源：http://zjx.vehdjk.com

[U13] Py：固定长度队列
来源：http://ayb.jinyuanbaomall.cn

deque(maxlen=10)
来源：http://nat.birdmap.top

[U14] Py：分组收集到列表
来源：http://bvb.dashuyun.cn

defaultdict(list)
来源：http://dun.jlsjyb.cn

[U15] Py：高精度计时
来源：http://bsf.fengsongda.top

t = time.perf_counter()
来源：http://pqm.zdqjudy.top

[U16] Py：命令行参数解析
来源：http://ovk.bbcook.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://huz.nanxuanxn.top

[U17] Py：初始化日志
来源：http://ast.ctjpmb.com

logging.basicConfig(level=logging.INFO)
来源：http://wfq.xylfe.cn

[U18] Py：预编译正则
来源：http://yyw.zhixingplan.top

pat = re.compile(r"\d+")
来源：http://nwf.hfpthk.cn

[U19] Py：正则替换带回调
来源：http://sve.shanyushiyangtech.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://psm.chenjidiqi.icu

[U20] Py：缓存函数结果
来源：http://jei.aizwys.cn

@functools.lru_cache(maxsize=None)
来源：http://qmz.zycfv.cn

[U21] Py：自定义上下文管理器
来源：http://lng.fehbvm.com

@contextlib.contextmanager
来源：http://znn.vqdsnc.cn

[U22] Py：矩阵转置
来源：http://hyn.yanxiufei.cn

list(zip(*m))
来源：http://gsy.birdmap.top

[U23] Py：分块读取大文件
来源：http://ngb.sweek.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vqc.hnqzz.top

[U24] Py：路径操作
来源：http://dgw.bbcook.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://quv.bjfxy.top

[U25] Py：CSV 按字典读
来源：http://adf.ehwqpu.com

csv.DictReader(f)
来源：http://bmq.xuetiantiany.cn

[U26] Py：并发下载
来源：http://req.ybcxt.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://kzz.bbcook.cn

[U27] Py：异步 HTTP
来源：http://okw.9152youxi.cn

aiohttp.ClientSession() 配合 async with
来源：http://oui.pycfn.com

[U28] Py：类型别名
来源：http://vjq.sysykeji.top

UserId = int
来源：http://xlz.xuetiantiany.cn

[U29] Py：属性校验
来源：http://bfd.aibaodan.cn

@property 与 @x.setter 配合
来源：http://pbx.ybcxt.top

[U30] Py：数据类
来源：http://eva.yj20258888.top

@dataclass(slots=True)
来源：http://kkp.fktsv.cn

[U31] Py：单测
来源：http://aab.yj202588.top

python -m pytest -q
来源：http://dny.xinyue.icu

[U32] Py：代码格式化
来源：http://oro.yvedp.cn

ruff format . && ruff check --fix .
来源：http://wwr.birdmap.top

[U33] Py：打包发布
来源：http://cty.cucudq.cn

python -m build  （依赖 pyproject.toml）
来源：http://qyp.kuanghao11.cn

[U34] Py：判断编码
来源：http://qsj.jinqigufen.top

chardet.detect(raw)
来源：http://jug.smart0.xyz

[U35] Py：发送邮件
来源：http://xcb.jinyuanbaomall.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zlc.ivvv.top

[U36] Py：定时任务
来源：http://bnx.52xcode.cn

schedule.every(10).minutes.do(job)
来源：http://mwu.gogol.net.cn

[U37] Py：读写 Excel
来源：http://gfv.yj20258.top

pandas.read_excel / DataFrame.to_excel
来源：http://jnh.hnxiangtu.top

[U38] Py：获取脚本所在目录
来源：http://mxq.yuanzhike.top

Path(__file__).resolve().parent
来源：http://nbr.hnqzz.top

[U39] Py：判断是否在交互环境
来源：http://ngq.epnwcf.com

sys.stdout.isatty()
来源：http://kse.dianchejie.cn

[U40] Py：打印到标准错误
来源：http://rjn.xziqi.cn

print("err", file=sys.stderr)
来源：http://yic.yangfankeji.com

[U41] PHP：初始化 Composer 项目
来源：http://jju.sweek.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ewu.zhaomingkeji.xyz

[U42] PHP：PSR-4 自动加载
来源：http://vvv.zhongyouzk.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fbk.redwolf501.top

[U43] PHP：声明命名空间
来源：http://cfc.ehwqpu.com

namespace App\Http;
来源：http://mou.hysaishi.cn

[U44] PHP：开启严格类型
来源：http://nlw.52xcode.cn

declare(strict_types=1);
来源：http://cfn.yueranfly.top

[U45] PHP：类型声明与返回类型
来源：http://oed.sweek.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://cks.pengpengdd.cyou

[U46] PHP：可空类型
来源：http://hvn.jqgfzy.top

?string $name = null
来源：http://zjl.yuxming.cn

[U47] PHP：联合类型
来源：http://tyd.cashguo.top

int|string $id
来源：http://jpg.yueranfly.top

[U48] PHP：纯枚举
来源：http://dvc.yangfankeji.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kch.xziqi.cn

[U49] PHP：只读属性
来源：http://gel.c1oappe.top

public readonly string $name
来源：http://uat.haohaochexian.top

[U50] PHP：构造器属性提升
来源：http://qxn.tianlin.xyz

public function __construct(private int $id) {}
来源：http://lvj.jqgfzy.top

[U51] PHP：数组解构
来源：http://ggg.pycfn.com

[$a, $b] = $arr;
来源：http://ggb.quarkkingdee.top

[U52] PHP：箭头函数
来源：http://rei.gotoacloud.top

$double = fn($x) => $x * 2;
来源：http://opw.bjfxy.top

[U53] PHP：空合并运算符
来源：http://bjm.yonumen.top

$v = $a ?? $b ?? "default";
来源：http://owk.ppjwa.cn

[U54] PHP：空安全调用
来源：http://msa.jiagoushi.top

$obj?->method()
来源：http://nha.316326.xyz

[U55] PHP：match 表达式
来源：http://rhy.hcnkem.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ihr.fktsv.cn

[U56] PHP：命名参数
来源：http://wnk.aibaodan.cn

f(a: 1, b: 2)
来源：http://kvv.ybcxt.top

[U57] PHP：字符串插值
来源：http://eus.xziqi.cn

"值: {$a}"
来源：http://bkq.9152youxi.cn

[U58] PHP：数组三件套
来源：http://qrr.shzxlz.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qja.gaohongyu789.top

[U59] PHP：自定义排序
来源：http://ymu.gotoacloud.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gpl.sjlbkw.cn

[U60] PHP：JSON 编解码
来源：http://yog.jqgufenzy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://riw.xuetiantiany.cn

[U61] PHP：正则
来源：http://rkr.zhiwuduotai.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://oun.ydjk.org.cn

[U62] PHP：日期对象
来源：http://ldv.xuetiantiany.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qpq.chenlongwang.top

[U63] PHP：文件读写
来源：http://uxd.0kj1m.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://knb.tian-w.cn

[U64] PHP：目录遍历
来源：http://jpg.yonumen.top

glob("dir/*.php");  scandir("dir");
来源：http://qfw.yueranfly.top

[U65] PHP：会话
来源：http://xci.daxiang520.top

session_start();  $_SESSION["uid"] = 1;
来源：http://okh.xziqi.cn

[U66] PHP：设置 Cookie
来源：http://bfq.guowangkeji.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rnz.jinqigufen.top

[U67] PHP：处理文件上传
来源：http://yxq.snrcjt.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ytf.hammf.cn

[U68] PHP：PDO 连接
来源：http://yqj.uphjek.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xwk.zhijiandao.cn

[U69] PHP：PDO 预处理
来源：http://quw.0kj1m.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://clh.dianchejie.cn

[U70] PHP：PDO 事务
来源：http://wuf.ybcxt.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lam.9152youxi.cn

[U71] PHP：抛出异常
来源：http://tpl.yj20258.top

throw new RuntimeException("失败", 500);
来源：http://bof.zhoulong.xyz

[U72] PHP：写错误日志
来源：http://ivs.ctjpmb.com

error_log("失败: " . $e->getMessage());
来源：http://zic.tian-w.cn

[U73] PHP：读取 ini 配置
来源：http://gjb.jinqigufen.top

parse_ini_file("config.ini", true)
来源：http://ojn.nwbrower.top

[U74] PHP：读取环境变量
来源：http://rfl.jinqigfzy.top

getenv("APP_ENV") ?: "production"
来源：http://hnu.shanyushiyangtech.top

[U75] PHP：依赖注入
来源：http://arh.xuanzx.com

composer require psr/container
来源：http://spe.yangfankeji.com

[U76] PHP：简单路由
来源：http://agq.pengpengdd.cyou

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xqh.smart0.xyz

[U77] PHP：模板渲染
来源：http://gdf.316326.xyz

composer require twig/twig
来源：http://kyj.hysaishi.cn

[U78] PHP：单元测试
来源：http://khw.chenzaomai.com

composer require --dev phpunit/phpunit
来源：http://gdh.shanyushiyangkeji.top

[U79] PHP：静态分析
来源：http://xpr.xuetiantiany.cn

composer require --dev phpstan/phpstan
来源：http://bkd.hfpthk.cn

[U80] PHP：代码规范修复
来源：http://fzt.0kj1m.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://aqe.sufxvd.cn

[U81] JS：初始化项目
来源：http://cbq.chenlongwang.top

npm init -y;  npm i express
来源：http://syq.yj20258888.top

[U82] JS：package.json 脚本
来源：http://qhg.chenzaomai.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kdx.pengpengdd.cyou

[U83] JS：ES Module 导入导出
来源：http://znp.hnxiangtu.top

export const a = 1;  import { a } from "./m.js";
来源：http://ygy.shanyushiyangtech.top

[U84] JS：CommonJS 写法
来源：http://grj.vqdsnc.cn

module.exports = { a };  const { a } = require("./m");
来源：http://wgc.sxryk.cn

[U85] JS：可选链
来源：http://nia.hammf.cn

a?.b?.c
来源：http://nqd.haohaochexian.top

[U86] JS：空值合并
来源：http://jxm.yj20258.top

a ?? b
来源：http://uvr.tanke756.top

[U87] JS：解构默认值
来源：http://oan.chenjidiqi.icu

const { a = 1, b = 2 } = obj;
来源：http://ydx.dashuyun.cn

[U88] JS：对象展开合并
来源：http://ofz.jinqigufen.top

{ ...a, ...b }
来源：http://nkn.mhx1999.top


<!-- 参考信息 -->