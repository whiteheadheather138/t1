代发 wailian999

[T05] Kotlin：when 表达式
来源：http://fbz.yangfankeji.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://etc.9152youxi.cn

[T06] Kotlin：集合映射
来源：http://hjw.xinyue.icu

listOf(1, 2, 3).map { it * 2 }
来源：http://tft.zhixingplan.top

[T07] Kotlin：集合过滤
来源：http://uhn.chenzaomai.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://ueq.yueranfly.top

[T08] Kotlin：数据类
来源：http://mow.iojbl.cn

data class User(val name: String, val age: Int)
来源：http://xbf.gogol.net.cn

[T09] Kotlin：扩展函数
来源：http://bpf.ehwqpu.com

fun String.exclaim() = this + "!"
来源：http://aur.zhijiandao.cn

[T10] Kotlin：默认参数
来源：http://ape.hnxiangtu.top

fun greet(name: String = "World") = "Hi $name"
来源：http://njq.bjfxy.top

[T11] Kotlin：协程
来源：http://vue.smart0.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://env.0kj1m.cn

[T12] Kotlin：解构声明
来源：http://jxb.gogol.net.cn

val (a, b) = Pair(1, 2)
来源：http://dfm.yj20258.top

[T13] Kotlin：只读 Map
来源：http://uos.sweek.top

val m = mapOf("a" to 1)
来源：http://lgb.birdmap.top

[T14] Kotlin：循环
来源：http://vzk.zycfv.cn

for (i in 1..10) println(i)
来源：http://obn.zhengqikj.top

[T15] Kotlin：接口
来源：http://gqk.vehdjk.com

interface Shape { fun area(): Double }
来源：http://bhk.tianlin.xyz

[T16] Swift：Hello World
来源：http://wnv.epnwcf.com

print("Hello")
来源：http://tsq.andypj.xyz

[T17] Swift：变量与常量
来源：http://rnv.chenjidiqi.icu

var a = 1;  let b = 2
来源：http://uer.jinyuanbaomall.cn

[T18] Swift：字符串插值
来源：http://ciz.zhiwuduotai.top

"值: \(b)"
来源：http://siv.zhijiandao.cn

[T19] Swift：可选绑定
来源：http://nvc.sjlbkw.cn

if let n = opt { print(n) }
来源：http://bkm.xuetiantiany.cn

[T20] Swift：数组操作
来源：http://lul.daria6918.cn

var a = [1, 2, 3];  a.append(4)
来源：http://xrz.hnxiangtu.top

[T21] Swift：遍历
来源：http://maf.tarul.cn

for x in a { print(x) }
来源：http://jfx.jianghu66.top

[T22] Swift：字典
来源：http://ege.hfpthk.cn

var d = ["a": 1];  d["b"] = 2
来源：http://sps.0kj1m.cn

[T23] Swift：函数
来源：http://mrs.ehwqpu.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ziy.sweek.top

[T24] Swift：闭包
来源：http://kqt.yj202588.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://tse.hfpthk.cn

[T25] Swift：结构体
来源：http://qmx.jinqigfzy.top

struct P { var x: Int }
来源：http://egu.ywan-chungtsiang.top

[T26] Swift：类与重写
来源：http://ovq.xinyue.icu

class A: Base { override func f() {} }
来源：http://exy.gaohongyu789.top

[T27] Swift：错误处理
来源：http://caz.fzhhl.top

do { try f() } catch { print(error) }
来源：http://pmw.jianghu66.top

[T28] Swift：枚举
来源：http://ege.jinqigfzy.top

enum Color { case red, green }
来源：http://dzv.tian-w.cn

[T29] Swift：guard 提前返回
来源：http://bnc.c1oappe.top

guard let x = opt else { return }
来源：http://nbz.shzxlz.cn

[T30] Swift：协议
来源：http://vhc.yvedp.cn

protocol Shape { func area() -> Double }
来源：http://ame.cqqwz.cn

[T31] Lua：Hello World
来源：http://dmm.gogol.net.cn

print("Hello")
来源：http://fes.meibo888.top

[T32] Lua：局部变量
来源：http://lhj.daxiang520.top

local a = 1
来源：http://kvy.fzhhl.top

[T33] Lua：表（数组）
来源：http://ikl.smart0.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://pjh.hammf.cn

[T34] Lua：遍历表
来源：http://ylm.wangdashe.top

for i, v in ipairs(t) do print(i, v) end
来源：http://rlg.yanxiufei.cn

[T35] Lua：字典表
来源：http://brg.zhijiandao.cn

local d = { a = 1 };  d.b = 2
来源：http://kgo.quarkkingdee.top

[T36] Lua：函数
来源：http://sxi.redwolf501.top

function add(a, b) return a + b end
来源：http://nct.ppjwa.cn

[T37] Lua：字符串拼接
来源：http://sar.yuanzhike.top

"a" .. "b"
来源：http://flp.havefunace.top

[T38] Lua：条件
来源：http://bgc.pycfn.com

if x > 0 then print("正") end
来源：http://kez.yuxming.cn

[T39] Lua：模式匹配
来源：http://oqc.yangfankeji.com

string.find(s, "%d+")
来源：http://dsv.sysykeji.top

[T40] Lua：元表
来源：http://fjt.ybcxt.top

setmetatable({}, { __index = base })
来源：http://gjj.xziqi.cn

[T41] Perl：Hello World
来源：http://puy.jqgufenzy.top

print "Hello\n";
来源：http://bhm.zhoulong.xyz

[T42] Perl：变量类型
来源：http://max.ywan-chungtsiang.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yov.snrcjt.cn

[T43] Perl：字符串插值
来源：http://kgu.ydjk.org.cn

"值: $a"
来源：http://hgp.jinghuilouyu.cn

[T44] Perl：条件
来源：http://mjm.sjlbkw.cn

if ($a > 0) { print "正"; }
来源：http://uid.gzhubu.top

[T45] Perl：数组遍历
来源：http://qoh.zdqjudy.top

for my $x (@arr) { print $x; }
来源：http://kgb.feifeiyinyue.top

[T46] Perl：哈希操作
来源：http://nhx.daxiang520.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://iah.guannengcc.top

[T47] Perl：正则捕获
来源：http://afx.hnxiangtu.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://pku.ywan-chungtsiang.top

[T48] Perl：正则替换
来源：http://jgn.hongshengwenyu.top

$s =~ s/old/new/g;
来源：http://xwt.zhijiandao.cn

[T49] Perl：函数
来源：http://cud.pengpengdd.cyou

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pmm.zdbjq.cn

[T50] Perl：逐行读文件
来源：http://jkf.ppjwa.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://dmu.redwolf501.top

while (my $line = <$fh>) { print $line; }
来源：http://wmc.nanxuanxn.top

[T51] Scala：Hello World
来源：http://bqp.yvedp.cn

println("Hello")
来源：http://mqk.chenjidiqi.icu

[T52] Scala：变量
来源：http://yym.shangyingyoupin.top

val a = 1;  var b = 2
来源：http://mfm.aizwys.cn

[T53] Scala：字符串插值
来源：http://bvq.sufxvd.cn

s"值: $b"
来源：http://nmf.havefunace.top

[T54] Scala：集合映射
来源：http://kyq.andypj.xyz

List(1, 2, 3).map(_ * 2)
来源：http://fpp.bbcook.cn

[T55] Scala：集合过滤
来源：http://ymq.yuxming.cn

List(1, 2, 3).filter(_ > 1)
来源：http://wch.vqdsnc.cn

[T56] Scala：样例类
来源：http://utx.guannengcc.top

case class User(name: String, age: Int)
来源：http://gvb.sjlbkw.cn

[T57] Scala：模式匹配
来源：http://yht.tarul.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://iyw.zhongyouzk.top

[T58] Scala：函数定义
来源：http://ozz.yongpay.top

def add(a: Int, b: Int): Int = a + b
来源：http://yfd.sufxvd.cn

[T59] Scala：循环
来源：http://yes.shanyushiyangkeji.top

for (i <- 1 to 10) println(i)
来源：http://ldl.cqqwz.cn

[T60] Scala：折叠
来源：http://ruz.316326.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://euj.ctjpmb.com

================================================================================
来源：http://jsh.9152youxi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://eug.0kj1m.cn

================================================================================
来源：http://tqx.dashuyun.cn

[U01] Py：创建虚拟环境
来源：http://aqw.kuanghao11.cn

python -m venv .venv && source .venv/bin/activate
来源：http://nxd.yvedp.cn

[U02] Py：导出 / 安装依赖
来源：http://zbo.bjfxy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ghc.mhx1999.top

[U03] Py：加载 .env 配置
来源：http://njz.pengpengdd.cyou

from dotenv import load_dotenv; load_dotenv()
来源：http://wsu.yj202588.top

[U04] Py：变量调试打印
来源：http://idn.yuanzhike.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://yiq.ehwqpu.com

[U05] Py：列表去重且保序
来源：http://gpp.cdnleiting.top

list(dict.fromkeys(arr))
来源：http://pnv.mhx1999.top

[U06] Py：合并两个字典
来源：http://vsk.sjlbkw.cn

{**a, **b}
来源：http://mvr.ywan-chungtsiang.top

[U07] Py：反转字典键值
来源：http://twm.yueranfly.top

{v: k for k, v in d.items()}
来源：http://gmc.jinghuilouyu.cn

[U08] Py：展平二维列表
来源：http://gdb.meibo888.top

[y for x in nested for y in x]
来源：http://amy.yuanzhike.top

[U09] Py：字典取最大值的键
来源：http://awy.zhiwuduotai.top

max(d, key=d.get)
来源：http://iln.yj20258888.top

[U10] Py：按值排序字典
来源：http://hak.zdqjudy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fsl.jqgufenzy.top

[U11] Py：生成器表达式
来源：http://slg.ehwqpu.com

(x * 2 for x in arr)
来源：http://izp.daxiang520.top

[U12] Py：取出现最多的 3 个元素
来源：http://uvr.epnwcf.com

Counter(arr).most_common(3)
来源：http://dsn.ywan-chungtsiang.top

[U13] Py：固定长度队列
来源：http://hvo.shanyushiyangtech.top

deque(maxlen=10)
来源：http://dwe.yfazqb.com

[U14] Py：分组收集到列表
来源：http://slx.xingfuxueyuan.xyz

defaultdict(list)
来源：http://ril.gogol.net.cn

[U15] Py：高精度计时
来源：http://bmf.yanxiufei.cn

t = time.perf_counter()
来源：http://scz.chenzaomai.com

[U16] Py：命令行参数解析
来源：http://sat.bjfxy.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://azi.daxiang520.top

[U17] Py：初始化日志
来源：http://vtt.pengpengdd.cyou

logging.basicConfig(level=logging.INFO)
来源：http://fsy.jinqigufen.top

[U18] Py：预编译正则
来源：http://ivq.zhongyouzk.top

pat = re.compile(r"\d+")
来源：http://goe.aibaodan.cn

[U19] Py：正则替换带回调
来源：http://whv.gogol.net.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qdr.yj202588.top

[U20] Py：缓存函数结果
来源：http://ehs.cdnleiting.top

@functools.lru_cache(maxsize=None)
来源：http://zyr.hywenlv.cn

[U21] Py：自定义上下文管理器
来源：http://ikv.bbcook.cn

@contextlib.contextmanager
来源：http://vos.feifeiyinyue.top

[U22] Py：矩阵转置
来源：http://zth.yuanzhike.top

list(zip(*m))
来源：http://lli.birdmap.top

[U23] Py：分块读取大文件
来源：http://xmd.redwolf501.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jvr.hesvh.cn

[U24] Py：路径操作
来源：http://wkn.yuxming.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hkg.cdnleiting.top

[U25] Py：CSV 按字典读
来源：http://gge.ydzc1.top

csv.DictReader(f)
来源：http://anj.jinqigufen.top

[U26] Py：并发下载
来源：http://xzu.zhiwuduotai.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mfo.hnqzz.top

[U27] Py：异步 HTTP
来源：http://yid.cucudq.cn

aiohttp.ClientSession() 配合 async with
来源：http://las.yuanzhike.top

[U28] Py：类型别名
来源：http://uig.c1oappe.top

UserId = int
来源：http://sqb.52xcode.cn

[U29] Py：属性校验
来源：http://mfk.fanxiaobao.xyz

@property 与 @x.setter 配合
来源：http://sgr.zhengqikj.top

[U30] Py：数据类
来源：http://wmg.tarul.cn

@dataclass(slots=True)
来源：http://pdr.hnxiangtu.top

[U31] Py：单测
来源：http://hlf.iojbl.cn

python -m pytest -q
来源：http://bnb.havefunace.top

[U32] Py：代码格式化
来源：http://yly.ehwqpu.com

ruff format . && ruff check --fix .
来源：http://rnp.jinqigfzy.top

[U33] Py：打包发布
来源：http://pfy.xylfe.cn

python -m build  （依赖 pyproject.toml）
来源：http://dur.ydzc1.top

[U34] Py：判断编码
来源：http://wmu.fktsv.cn

chardet.detect(raw)
来源：http://bbc.xziqi.cn

[U35] Py：发送邮件
来源：http://ejc.chenlongwang.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vja.hcnkem.com

[U36] Py：定时任务
来源：http://rwu.hammf.cn

schedule.every(10).minutes.do(job)
来源：http://mpa.zhixingplan.top

[U37] Py：读写 Excel
来源：http://rgp.daria6918.cn

pandas.read_excel / DataFrame.to_excel
来源：http://pga.316326.xyz

[U38] Py：获取脚本所在目录
来源：http://nlc.shanyushiyangtech.top

Path(__file__).resolve().parent
来源：http://zkb.ppjwa.cn

[U39] Py：判断是否在交互环境
来源：http://eim.316326.xyz

sys.stdout.isatty()
来源：http://you.yj20258888.top

[U40] Py：打印到标准错误
来源：http://btf.guannengcc.top

print("err", file=sys.stderr)
来源：http://mdg.zhongyouzk.top

[U41] PHP：初始化 Composer 项目
来源：http://nra.tanke756.top

composer init;  composer require guzzlehttp/guzzle
来源：http://iku.jqgufenzy.top

[U42] PHP：PSR-4 自动加载
来源：http://fzn.kuanghao11.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fhv.gzhubu.top

[U43] PHP：声明命名空间
来源：http://cqj.pycfn.com

namespace App\Http;
来源：http://ljl.chenjidiqi.icu

[U44] PHP：开启严格类型
来源：http://hce.chenlongwang.top

declare(strict_types=1);
来源：http://fff.yangfankeji.com

[U45] PHP：类型声明与返回类型
来源：http://ajf.zhaomingkeji.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://zgi.pengpengdd.cyou

[U46] PHP：可空类型
来源：http://jtp.jlsjyb.cn

?string $name = null
来源：http://mpg.aibaodan.cn

[U47] PHP：联合类型
来源：http://tck.haohaochexian.top

int|string $id
来源：http://bln.zhoulong.xyz

[U48] PHP：纯枚举
来源：http://oyl.zhaomingkeji.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://uil.hesvh.cn

[U49] PHP：只读属性
来源：http://ehq.epnwcf.com

public readonly string $name
来源：http://bvh.hysaishi.cn

[U50] PHP：构造器属性提升
来源：http://djq.vqdsnc.cn

public function __construct(private int $id) {}
来源：http://qoi.sufxvd.cn

[U51] PHP：数组解构
来源：http://smi.jiagoushi.top

[$a, $b] = $arr;
来源：http://uaw.kuanghao11.cn

[U52] PHP：箭头函数
来源：http://ela.daxiang520.top

$double = fn($x) => $x * 2;
来源：http://usn.yj20258888.top

[U53] PHP：空合并运算符
来源：http://vrj.hywenlv.cn

$v = $a ?? $b ?? "default";
来源：http://umb.hcnkem.com

[U54] PHP：空安全调用
来源：http://jls.hcnkem.com

$obj?->method()
来源：http://iut.ppjwa.cn

[U55] PHP：match 表达式
来源：http://wgs.dianchejie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://pva.nanxinkj.top

[U56] PHP：命名参数
来源：http://icq.zycfv.cn

f(a: 1, b: 2)
来源：http://khs.zhijiandao.cn

[U57] PHP：字符串插值
来源：http://his.zhijiandao.cn

"值: {$a}"
来源：http://lhm.nanxuanxn.top

[U58] PHP：数组三件套
来源：http://fwu.52xcode.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pmg.redwolf501.top

[U59] PHP：自定义排序
来源：http://pzz.gotoacloud.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uft.ppjwa.cn

[U60] PHP：JSON 编解码
来源：http://xcy.iojbl.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://sip.tianlin.xyz

[U61] PHP：正则
来源：http://zrv.c1oappe.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://leb.yonumen.top

[U62] PHP：日期对象
来源：http://goj.haohaochexian.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fqv.sxryk.cn

[U63] PHP：文件读写
来源：http://vds.jqgufenzy.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qej.zhongyouzk.top

[U64] PHP：目录遍历
来源：http://oig.sweek.top

glob("dir/*.php");  scandir("dir");
来源：http://jnx.xingfuxueyuan.xyz

[U65] PHP：会话
来源：http://jsg.jyoumei.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://aqb.tanke756.top

[U66] PHP：设置 Cookie
来源：http://ecu.sjlbkw.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ihf.yuanzhike.top

[U67] PHP：处理文件上传
来源：http://dfq.jqgfzy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kkj.zhixingplan.top

[U68] PHP：PDO 连接
来源：http://etb.zhoulong.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vpm.quarkkingdee.top

[U69] PHP：PDO 预处理
来源：http://jzi.dashuyun.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nqr.ivvv.top

[U70] PHP：PDO 事务
来源：http://njm.yongpay.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gvu.guannengcc.top

[U71] PHP：抛出异常
来源：http://xsu.guowangkeji.top

throw new RuntimeException("失败", 500);
来源：http://cnf.jqgufenzy.top

[U72] PHP：写错误日志
来源：http://xiy.haohaochexian.top

error_log("失败: " . $e->getMessage());
来源：http://ece.yueranfly.top

[U73] PHP：读取 ini 配置
来源：http://mcs.jinqigfzy.top

parse_ini_file("config.ini", true)
来源：http://pre.xinyue.icu

[U74] PHP：读取环境变量
来源：http://bje.jinghuilouyu.cn

getenv("APP_ENV") ?: "production"
来源：http://zgo.sjlbkw.cn

[U75] PHP：依赖注入
来源：http://osa.chenzaomai.com

composer require psr/container
来源：http://ezg.sufxvd.cn

[U76] PHP：简单路由
来源：http://cnw.yvedp.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://izq.cheryme.top

[U77] PHP：模板渲染
来源：http://zzs.yanxiufei.cn

composer require twig/twig
来源：http://kvo.sxryk.cn

[U78] PHP：单元测试
来源：http://iyr.xingfuxueyuan.xyz

composer require --dev phpunit/phpunit
来源：http://upo.aibaodan.cn

[U79] PHP：静态分析
来源：http://adv.316326.xyz

composer require --dev phpstan/phpstan
来源：http://lfq.zhixingplan.top

[U80] PHP：代码规范修复
来源：http://syd.tianlin.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://oux.cashguo.top

[U81] JS：初始化项目
来源：http://wrv.fktsv.cn

npm init -y;  npm i express
来源：http://wgi.zhixingplan.top

[U82] JS：package.json 脚本
来源：http://wng.cashguo.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cfs.hongshengwenyu.top

[U83] JS：ES Module 导入导出
来源：http://rdj.fengsongda.top

export const a = 1;  import { a } from "./m.js";
来源：http://ayh.zhongyouzk.top

[U84] JS：CommonJS 写法
来源：http://qwq.chenlongwang.top

module.exports = { a };  const { a } = require("./m");
来源：http://crl.yj20258888.top

[U85] JS：可选链
来源：http://uct.chenzaomai.com

a?.b?.c
来源：http://rzq.bbcook.cn

[U86] JS：空值合并
来源：http://tkp.xylfe.cn

a ?? b
来源：http://urx.sxryk.cn

[U87] JS：解构默认值
来源：http://xyk.cashguo.top

const { a = 1, b = 2 } = obj;
来源：http://crk.zhoulong.xyz

[U88] JS：对象展开合并
来源：http://ibo.yanxiufei.cn

{ ...a, ...b }
来源：http://gmt.0kj1m.cn

[U89] JS：数组去重
来源：http://eal.bbcook.cn

[...new Set(arr)]
来源：http://rpn.smart0.xyz

[U90] JS：数字数组排序
来源：http://nue.hfpthk.cn

[...arr].sort((a, b) => a - b)
来源：http://mfs.fzhhl.top

[U91] JS：对象键值遍历
来源：http://qsp.aibaodan.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jmt.zhixingplan.top

[U92] JS：深拷贝
来源：http://tcy.pycfn.com

structuredClone(obj)
来源：http://nmp.jinghuilouyu.cn


<!-- 参考信息 -->