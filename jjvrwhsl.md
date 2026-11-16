代发 wailian999

[T05] Kotlin：when 表达式
来源：http://vif.fanxiaobao.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hpw.sjlbkw.cn

[T06] Kotlin：集合映射
来源：http://fve.uphjek.com

listOf(1, 2, 3).map { it * 2 }
来源：http://puu.dianchejie.cn

[T07] Kotlin：集合过滤
来源：http://tgh.aizwys.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://lme.nanxinkj.top

[T08] Kotlin：数据类
来源：http://xpf.xuanzx.com

data class User(val name: String, val age: Int)
来源：http://hyo.sxryk.cn

[T09] Kotlin：扩展函数
来源：http://pcr.ppjwa.cn

fun String.exclaim() = this + "!"
来源：http://cwb.hammf.cn

[T10] Kotlin：默认参数
来源：http://okt.sjlbkw.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://gmp.ydjk.org.cn

[T11] Kotlin：协程
来源：http://orp.jinyuanbaomall.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://rlt.iojbl.cn

[T12] Kotlin：解构声明
来源：http://ckf.xingfuxueyuan.xyz

val (a, b) = Pair(1, 2)
来源：http://uqe.yongpay.top

[T13] Kotlin：只读 Map
来源：http://pfj.jlsjyb.cn

val m = mapOf("a" to 1)
来源：http://dtx.epnwcf.com

[T14] Kotlin：循环
来源：http://pwi.cqqwz.cn

for (i in 1..10) println(i)
来源：http://zyb.havefunace.top

[T15] Kotlin：接口
来源：http://wfj.redwolf501.top

interface Shape { fun area(): Double }
来源：http://gqw.dashuyun.cn

[T16] Swift：Hello World
来源：http://tif.gaohongyu789.top

print("Hello")
来源：http://imj.fktsv.cn

[T17] Swift：变量与常量
来源：http://tew.jqgfzy.top

var a = 1;  let b = 2
来源：http://kdu.sxryk.cn

[T18] Swift：字符串插值
来源：http://bvp.ehwqpu.com

"值: \(b)"
来源：http://gsu.cashguo.top

[T19] Swift：可选绑定
来源：http://rjj.hcnkem.com

if let n = opt { print(n) }
来源：http://vtq.9152youxi.cn

[T20] Swift：数组操作
来源：http://xkh.quarkkingdee.top

var a = [1, 2, 3];  a.append(4)
来源：http://tmn.gzhubu.top

[T21] Swift：遍历
来源：http://yca.pycfn.com

for x in a { print(x) }
来源：http://guk.hysaishi.cn

[T22] Swift：字典
来源：http://ixq.gaohongyu789.top

var d = ["a": 1];  d["b"] = 2
来源：http://hgf.hywenlv.cn

[T23] Swift：函数
来源：http://jjq.hysaishi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://azg.fktsv.cn

[T24] Swift：闭包
来源：http://mmy.zhongyouzk.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://cvl.sxryk.cn

[T25] Swift：结构体
来源：http://lfd.epnwcf.com

struct P { var x: Int }
来源：http://kdg.gogol.net.cn

[T26] Swift：类与重写
来源：http://nsf.hfpthk.cn

class A: Base { override func f() {} }
来源：http://lbu.dianchejie.cn

[T27] Swift：错误处理
来源：http://xfm.jianghu66.top

do { try f() } catch { print(error) }
来源：http://kpf.jianghu66.top

[T28] Swift：枚举
来源：http://hwr.pycfn.com

enum Color { case red, green }
来源：http://qug.xylfe.cn

[T29] Swift：guard 提前返回
来源：http://gsl.0kj1m.cn

guard let x = opt else { return }
来源：http://qoq.xingfuxueyuan.xyz

[T30] Swift：协议
来源：http://rfr.yuxming.cn

protocol Shape { func area() -> Double }
来源：http://alq.zycfv.cn

[T31] Lua：Hello World
来源：http://hac.yueranfly.top

print("Hello")
来源：http://udg.yj20258.top

[T32] Lua：局部变量
来源：http://uds.zhixingplan.top

local a = 1
来源：http://tpb.ivvv.top

[T33] Lua：表（数组）
来源：http://vgr.bjfxy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://grt.cdnleiting.top

[T34] Lua：遍历表
来源：http://jii.uphjek.com

for i, v in ipairs(t) do print(i, v) end
来源：http://veq.yvedp.cn

[T35] Lua：字典表
来源：http://obq.jinghuilouyu.cn

local d = { a = 1 };  d.b = 2
来源：http://ssj.yanxiufei.cn

[T36] Lua：函数
来源：http://sek.hesvh.cn

function add(a, b) return a + b end
来源：http://xfa.zhaomingkeji.xyz

[T37] Lua：字符串拼接
来源：http://uqc.fengsongda.top

"a" .. "b"
来源：http://tlk.yj20258888.top

[T38] Lua：条件
来源：http://ghd.ybcxt.top

if x > 0 then print("正") end
来源：http://nob.nanxuanxn.top

[T39] Lua：模式匹配
来源：http://bdt.cashguo.top

string.find(s, "%d+")
来源：http://cyc.shanyushiyangkeji.top

[T40] Lua：元表
来源：http://mxh.shuidangran.top

setmetatable({}, { __index = base })
来源：http://jaf.jinqigfzy.top

[T41] Perl：Hello World
来源：http://cvh.dianchejie.cn

print "Hello\n";
来源：http://mww.yangfankeji.com

[T42] Perl：变量类型
来源：http://enx.316326.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://flm.fengsongda.top

[T43] Perl：字符串插值
来源：http://kdh.ydjk.org.cn

"值: $a"
来源：http://lph.nwbrower.top

[T44] Perl：条件
来源：http://sry.ivvv.top

if ($a > 0) { print "正"; }
来源：http://cpk.wangshuangyany.cn

[T45] Perl：数组遍历
来源：http://pxv.sxryk.cn

for my $x (@arr) { print $x; }
来源：http://act.yanxiufei.cn

[T46] Perl：哈希操作
来源：http://fuc.hnqzz.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tjr.jqgufenzy.top

[T47] Perl：正则捕获
来源：http://kbm.sjlbkw.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://vwc.birdmap.top

[T48] Perl：正则替换
来源：http://qpq.smart0.xyz

$s =~ s/old/new/g;
来源：http://hqj.fengsongda.top

[T49] Perl：函数
来源：http://ozk.jiagoushi.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hwr.svipenyu.cn

[T50] Perl：逐行读文件
来源：http://vdj.jinyuanbaomall.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://iil.nwbrower.top

while (my $line = <$fh>) { print $line; }
来源：http://cdr.jianghu66.top

[T51] Scala：Hello World
来源：http://pob.jqgufenzy.top

println("Hello")
来源：http://hww.tianlin.xyz

[T52] Scala：变量
来源：http://gqn.kuanghao11.cn

val a = 1;  var b = 2
来源：http://gym.ehwqpu.com

[T53] Scala：字符串插值
来源：http://wnm.jqgufenzy.top

s"值: $b"
来源：http://kgv.ybcxt.top

[T54] Scala：集合映射
来源：http://zqv.zhaomingkeji.xyz

List(1, 2, 3).map(_ * 2)
来源：http://imj.yj20258888.top

[T55] Scala：集合过滤
来源：http://vjp.jqgfzy.top

List(1, 2, 3).filter(_ > 1)
来源：http://ero.tian-w.cn

[T56] Scala：样例类
来源：http://ugo.shangyingyoupin.top

case class User(name: String, age: Int)
来源：http://ash.nanxuanxn.top

[T57] Scala：模式匹配
来源：http://gut.uphjek.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://yhn.yvedp.cn

[T58] Scala：函数定义
来源：http://rlt.xinyue.icu

def add(a: Int, b: Int): Int = a + b
来源：http://jks.sysykeji.top

[T59] Scala：循环
来源：http://pbs.jinghuilouyu.cn

for (i <- 1 to 10) println(i)
来源：http://zym.hfpthk.cn

[T60] Scala：折叠
来源：http://vtn.hywenlv.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cff.andypj.xyz

================================================================================
来源：http://cdr.jinqigfzy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fvi.dianchejie.cn

================================================================================
来源：http://gyt.jinqigufen.top

[U01] Py：创建虚拟环境
来源：http://pjy.fanxiaobao.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://jez.tian-w.cn

[U02] Py：导出 / 安装依赖
来源：http://stc.smart0.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ajk.hysaishi.cn

[U03] Py：加载 .env 配置
来源：http://gqu.sufxvd.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://fnq.shzxlz.cn

[U04] Py：变量调试打印
来源：http://riz.xuanzx.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://edg.xziqi.cn

[U05] Py：列表去重且保序
来源：http://ksu.guannengcc.top

list(dict.fromkeys(arr))
来源：http://nfp.zhengqikj.top

[U06] Py：合并两个字典
来源：http://oaz.redwolf501.top

{**a, **b}
来源：http://khk.yueranfly.top

[U07] Py：反转字典键值
来源：http://bei.svipenyu.cn

{v: k for k, v in d.items()}
来源：http://ufl.yanxiufei.cn

[U08] Py：展平二维列表
来源：http://tkc.xingfuxueyuan.xyz

[y for x in nested for y in x]
来源：http://ppf.haohaochexian.top

[U09] Py：字典取最大值的键
来源：http://rtj.cdnleiting.top

max(d, key=d.get)
来源：http://nxb.havefunace.top

[U10] Py：按值排序字典
来源：http://smg.shangyingyoupin.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://udn.sxryk.cn

[U11] Py：生成器表达式
来源：http://wql.hfpthk.cn

(x * 2 for x in arr)
来源：http://moq.yanxiufei.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xqo.epnwcf.com

Counter(arr).most_common(3)
来源：http://ijq.ppjwa.cn

[U13] Py：固定长度队列
来源：http://gqn.xingfuxueyuan.xyz

deque(maxlen=10)
来源：http://uzc.gaohongyu789.top

[U14] Py：分组收集到列表
来源：http://pcn.birdmap.top

defaultdict(list)
来源：http://zlr.c1oappe.top

[U15] Py：高精度计时
来源：http://azl.sufxvd.cn

t = time.perf_counter()
来源：http://sfc.zhengqikj.top

[U16] Py：命令行参数解析
来源：http://ajl.yonumen.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yym.hammf.cn

[U17] Py：初始化日志
来源：http://flx.pengpengdd.cyou

logging.basicConfig(level=logging.INFO)
来源：http://eds.tanke756.top

[U18] Py：预编译正则
来源：http://vvs.gogol.net.cn

pat = re.compile(r"\d+")
来源：http://oor.hongshengwenyu.top

[U19] Py：正则替换带回调
来源：http://zrf.guannengcc.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://oht.fktsv.cn

[U20] Py：缓存函数结果
来源：http://bxg.fanxiaobao.xyz

@functools.lru_cache(maxsize=None)
来源：http://hjb.yuanzhike.top

[U21] Py：自定义上下文管理器
来源：http://ntd.snrcjt.cn

@contextlib.contextmanager
来源：http://kgs.nanxinkj.top

[U22] Py：矩阵转置
来源：http://wxi.yfazqb.com

list(zip(*m))
来源：http://pel.kuanghao11.cn

[U23] Py：分块读取大文件
来源：http://qcg.shzxlz.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://djs.gogol.net.cn

[U24] Py：路径操作
来源：http://vwe.yj20258888.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://omv.cucudq.cn

[U25] Py：CSV 按字典读
来源：http://xpp.jiagoushi.top

csv.DictReader(f)
来源：http://jum.gzhubu.top

[U26] Py：并发下载
来源：http://nkn.zdqjudy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xzs.nanxuanxn.top

[U27] Py：异步 HTTP
来源：http://hah.cashguo.top

aiohttp.ClientSession() 配合 async with
来源：http://txf.fanxiaobao.xyz

[U28] Py：类型别名
来源：http://epp.tianlin.xyz

UserId = int
来源：http://uwk.tian-w.cn

[U29] Py：属性校验
来源：http://vri.xuanzx.com

@property 与 @x.setter 配合
来源：http://qcn.jinghuilouyu.cn

[U30] Py：数据类
来源：http://tnf.cdnleiting.top

@dataclass(slots=True)
来源：http://yem.daria6918.cn

[U31] Py：单测
来源：http://gpr.nanxinkj.top

python -m pytest -q
来源：http://jag.wangshuangyany.cn

[U32] Py：代码格式化
来源：http://ior.ydjk.org.cn

ruff format . && ruff check --fix .
来源：http://uap.jqgfzy.top

[U33] Py：打包发布
来源：http://fnb.shzxlz.cn

python -m build  （依赖 pyproject.toml）
来源：http://wsa.xuetiantiany.cn

[U34] Py：判断编码
来源：http://rem.316326.xyz

chardet.detect(raw)
来源：http://ume.sweek.top

[U35] Py：发送邮件
来源：http://omb.cashguo.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ejm.uphjek.com

[U36] Py：定时任务
来源：http://smn.hammf.cn

schedule.every(10).minutes.do(job)
来源：http://oub.epnwcf.com

[U37] Py：读写 Excel
来源：http://lvr.tianlin.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://sla.tian-w.cn

[U38] Py：获取脚本所在目录
来源：http://fcw.jianghu66.top

Path(__file__).resolve().parent
来源：http://btd.cheryme.top

[U39] Py：判断是否在交互环境
来源：http://hil.jlsjyb.cn

sys.stdout.isatty()
来源：http://rjs.quarkkingdee.top

[U40] Py：打印到标准错误
来源：http://wgh.yj202588.top

print("err", file=sys.stderr)
来源：http://sjs.iojbl.cn

[U41] PHP：初始化 Composer 项目
来源：http://czs.gaohongyu789.top

composer init;  composer require guzzlehttp/guzzle
来源：http://uua.pengpengdd.cyou

[U42] PHP：PSR-4 自动加载
来源：http://foi.chenlongwang.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rnp.shzxlz.cn

[U43] PHP：声明命名空间
来源：http://nox.fengsongda.top

namespace App\Http;
来源：http://vfd.yfazqb.com

[U44] PHP：开启严格类型
来源：http://zlw.guowangkeji.top

declare(strict_types=1);
来源：http://hjp.mhx1999.top

[U45] PHP：类型声明与返回类型
来源：http://jgw.ybcxt.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://uhm.tarul.cn

[U46] PHP：可空类型
来源：http://pmo.vqdsnc.cn

?string $name = null
来源：http://nxe.pengpengdd.cyou

[U47] PHP：联合类型
来源：http://zvm.yueranfly.top

int|string $id
来源：http://ppz.chenlongwang.top

[U48] PHP：纯枚举
来源：http://iyw.jqgufenzy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kzj.svipenyu.cn

[U49] PHP：只读属性
来源：http://nav.tianlin.xyz

public readonly string $name
来源：http://sqv.shanyushiyangkeji.top

[U50] PHP：构造器属性提升
来源：http://vso.gzhubu.top

public function __construct(private int $id) {}
来源：http://edn.cucudq.cn

[U51] PHP：数组解构
来源：http://lmj.birdmap.top

[$a, $b] = $arr;
来源：http://ztv.snrcjt.cn

[U52] PHP：箭头函数
来源：http://upl.yueranfly.top

$double = fn($x) => $x * 2;
来源：http://gii.9152youxi.cn

[U53] PHP：空合并运算符
来源：http://iok.shanyushiyangkeji.top

$v = $a ?? $b ?? "default";
来源：http://lya.shuidangran.top

[U54] PHP：空安全调用
来源：http://vbq.nanxuanxn.top

$obj?->method()
来源：http://ewc.jyoumei.cn

[U55] PHP：match 表达式
来源：http://uep.ehwqpu.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wbz.yj202588.top

[U56] PHP：命名参数
来源：http://iiu.tarul.cn

f(a: 1, b: 2)
来源：http://mvg.zhiwuduotai.top

[U57] PHP：字符串插值
来源：http://yzl.zdqjudy.top

"值: {$a}"
来源：http://kmw.svipenyu.cn

[U58] PHP：数组三件套
来源：http://djr.c1oappe.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://yhb.jinqigufen.top

[U59] PHP：自定义排序
来源：http://auf.ybcxt.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jrd.0kj1m.cn

[U60] PHP：JSON 编解码
来源：http://cmi.yj20258888.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gpt.jinqigufen.top

[U61] PHP：正则
来源：http://ngz.hongshengwenyu.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ldg.jinghuilouyu.cn

[U62] PHP：日期对象
来源：http://vqa.cashguo.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zfd.andypj.xyz

[U63] PHP：文件读写
来源：http://okg.jianghu66.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yty.quarkkingdee.top

[U64] PHP：目录遍历
来源：http://inb.nanxuanxn.top

glob("dir/*.php");  scandir("dir");
来源：http://ijh.nwbrower.top

[U65] PHP：会话
来源：http://qia.fanxiaobao.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://tav.nanxinkj.top

[U66] PHP：设置 Cookie
来源：http://vvs.gotoacloud.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://elj.andypj.xyz

[U67] PHP：处理文件上传
来源：http://ngh.hammf.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://nuf.andypj.xyz

[U68] PHP：PDO 连接
来源：http://hqp.feifeiyinyue.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://olx.fehbvm.com

[U69] PHP：PDO 预处理
来源：http://uik.xuetiantiany.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gfe.ctjpmb.com

[U70] PHP：PDO 事务
来源：http://reg.zhixingplan.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tvz.tianlin.xyz

[U71] PHP：抛出异常
来源：http://naz.yuanzhike.top

throw new RuntimeException("失败", 500);
来源：http://nmy.shzxlz.cn

[U72] PHP：写错误日志
来源：http://fcc.xingfuxueyuan.xyz

error_log("失败: " . $e->getMessage());
来源：http://dqn.jyoumei.cn

[U73] PHP：读取 ini 配置
来源：http://tqk.hywenlv.cn

parse_ini_file("config.ini", true)
来源：http://roe.uphjek.com

[U74] PHP：读取环境变量
来源：http://wuy.xylfe.cn

getenv("APP_ENV") ?: "production"
来源：http://oam.xuetiantiany.cn

[U75] PHP：依赖注入
来源：http://ppv.hesvh.cn

composer require psr/container
来源：http://gjx.andypj.xyz

[U76] PHP：简单路由
来源：http://vvv.vehdjk.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gtk.svipenyu.cn

[U77] PHP：模板渲染
来源：http://eid.vqdsnc.cn

composer require twig/twig
来源：http://vxu.jinghuilouyu.cn

[U78] PHP：单元测试
来源：http://jjn.yuanzhike.top

composer require --dev phpunit/phpunit
来源：http://fnx.vehdjk.com

[U79] PHP：静态分析
来源：http://qut.yonumen.top

composer require --dev phpstan/phpstan
来源：http://gmq.vehdjk.com

[U80] PHP：代码规范修复
来源：http://alh.sufxvd.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://itq.xinyue.icu

[U81] JS：初始化项目
来源：http://kdm.jyoumei.cn

npm init -y;  npm i express
来源：http://pko.cashguo.top

[U82] JS：package.json 脚本
来源：http://ull.shuidangran.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://niz.yj202588.top

[U83] JS：ES Module 导入导出
来源：http://lln.yuanzhike.top

export const a = 1;  import { a } from "./m.js";
来源：http://hqc.hnqzz.top

[U84] JS：CommonJS 写法
来源：http://tsy.hywenlv.cn

module.exports = { a };  const { a } = require("./m");
来源：http://isi.ywan-chungtsiang.top

[U85] JS：可选链
来源：http://xam.ctjpmb.com

a?.b?.c
来源：http://zzv.meibo888.top

[U86] JS：空值合并
来源：http://seo.quarkkingdee.top

a ?? b
来源：http://cun.xylfe.cn

[U87] JS：解构默认值
来源：http://vyq.xuanzx.com

const { a = 1, b = 2 } = obj;
来源：http://nvi.fanxiaobao.xyz

[U88] JS：对象展开合并
来源：http://tft.daxiang520.top

{ ...a, ...b }
来源：http://qrg.chenjidiqi.icu

[U89] JS：数组去重
来源：http://vaa.zycfv.cn

[...new Set(arr)]
来源：http://qja.hfpthk.cn

[U90] JS：数字数组排序
来源：http://zub.0kj1m.cn

[...arr].sort((a, b) => a - b)
来源：http://kjb.hesvh.cn

[U91] JS：对象键值遍历
来源：http://ouf.ivvv.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pmy.daria6918.cn

[U92] JS：深拷贝
来源：http://goz.cheryme.top

structuredClone(obj)
来源：http://nvg.ctjpmb.com


<!-- 参考信息 -->