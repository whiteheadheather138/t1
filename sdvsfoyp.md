代发 wailian999

[T05] Kotlin：when 表达式
来源：http://mkv.tianlin.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wuf.daxiang520.top

[T06] Kotlin：集合映射
来源：http://xqj.bjfxy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://pgs.xuetiantiany.cn

[T07] Kotlin：集合过滤
来源：http://pum.shzxlz.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://vdm.yueranfly.top

[T08] Kotlin：数据类
来源：http://oty.ydjk.org.cn

data class User(val name: String, val age: Int)
来源：http://wlb.jianghu66.top

[T09] Kotlin：扩展函数
来源：http://rtf.jlsjyb.cn

fun String.exclaim() = this + "!"
来源：http://jnh.gogol.net.cn

[T10] Kotlin：默认参数
来源：http://nml.yonumen.top

fun greet(name: String = "World") = "Hi $name"
来源：http://pbo.hysaishi.cn

[T11] Kotlin：协程
来源：http://ywb.haohaochexian.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ghv.xuanzx.com

[T12] Kotlin：解构声明
来源：http://vmr.daxiang520.top

val (a, b) = Pair(1, 2)
来源：http://oos.wangshuangyany.cn

[T13] Kotlin：只读 Map
来源：http://ire.nanxuanxn.top

val m = mapOf("a" to 1)
来源：http://vna.mhx1999.top

[T14] Kotlin：循环
来源：http://kkx.fzhhl.top

for (i in 1..10) println(i)
来源：http://qod.sufxvd.cn

[T15] Kotlin：接口
来源：http://aoe.uphjek.com

interface Shape { fun area(): Double }
来源：http://amd.52xcode.cn

[T16] Swift：Hello World
来源：http://qus.52xcode.cn

print("Hello")
来源：http://oxy.yuxming.cn

[T17] Swift：变量与常量
来源：http://cyn.cdnleiting.top

var a = 1;  let b = 2
来源：http://mlm.hfpthk.cn

[T18] Swift：字符串插值
来源：http://qvp.zhoulong.xyz

"值: \(b)"
来源：http://xgg.sufxvd.cn

[T19] Swift：可选绑定
来源：http://wbr.gaohongyu789.top

if let n = opt { print(n) }
来源：http://fby.jyoumei.cn

[T20] Swift：数组操作
来源：http://vsl.chenjidiqi.icu

var a = [1, 2, 3];  a.append(4)
来源：http://nnq.zhengqikj.top

[T21] Swift：遍历
来源：http://ywr.epnwcf.com

for x in a { print(x) }
来源：http://fte.fzhhl.top

[T22] Swift：字典
来源：http://boq.jinghuilouyu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://tmq.jlsjyb.cn

[T23] Swift：函数
来源：http://alq.mhx1999.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ayk.jinqigufen.top

[T24] Swift：闭包
来源：http://adi.cqqwz.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://jxy.yj20258888.top

[T25] Swift：结构体
来源：http://mbz.sjlbkw.cn

struct P { var x: Int }
来源：http://nik.cheryme.top

[T26] Swift：类与重写
来源：http://zuf.yj202588.top

class A: Base { override func f() {} }
来源：http://mqw.xuanzx.com

[T27] Swift：错误处理
来源：http://auc.zhongyouzk.top

do { try f() } catch { print(error) }
来源：http://fdm.zhaomingkeji.xyz

[T28] Swift：枚举
来源：http://ube.jyoumei.cn

enum Color { case red, green }
来源：http://aiw.zhengqikj.top

[T29] Swift：guard 提前返回
来源：http://mrx.nanxinkj.top

guard let x = opt else { return }
来源：http://tys.tanke756.top

[T30] Swift：协议
来源：http://pgw.nwbrower.top

protocol Shape { func area() -> Double }
来源：http://ytd.tanke756.top

[T31] Lua：Hello World
来源：http://lgw.iojbl.cn

print("Hello")
来源：http://knn.xuanzx.com

[T32] Lua：局部变量
来源：http://nhm.shangyingyoupin.top

local a = 1
来源：http://voj.ivvv.top

[T33] Lua：表（数组）
来源：http://fjw.c1oappe.top

local t = {1, 2, 3};  t[4] = 4
来源：http://rzs.gogol.net.cn

[T34] Lua：遍历表
来源：http://zyi.gotoacloud.top

for i, v in ipairs(t) do print(i, v) end
来源：http://qax.yj20258.top

[T35] Lua：字典表
来源：http://ptd.chenzaomai.com

local d = { a = 1 };  d.b = 2
来源：http://wxs.tarul.cn

[T36] Lua：函数
来源：http://sae.9152youxi.cn

function add(a, b) return a + b end
来源：http://saq.aibaodan.cn

[T37] Lua：字符串拼接
来源：http://pha.jinqigfzy.top

"a" .. "b"
来源：http://eed.zhoulong.xyz

[T38] Lua：条件
来源：http://fsj.haohaochexian.top

if x > 0 then print("正") end
来源：http://tlx.hnqzz.top

[T39] Lua：模式匹配
来源：http://zwq.fehbvm.com

string.find(s, "%d+")
来源：http://nvc.shanyushiyangtech.top

[T40] Lua：元表
来源：http://vja.hfpthk.cn

setmetatable({}, { __index = base })
来源：http://orh.vehdjk.com

[T41] Perl：Hello World
来源：http://dcp.sysykeji.top

print "Hello\n";
来源：http://npo.fzhhl.top

[T42] Perl：变量类型
来源：http://lok.redwolf501.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://oqb.hnqzz.top

[T43] Perl：字符串插值
来源：http://aiy.yfazqb.com

"值: $a"
来源：http://zcg.jianghu66.top

[T44] Perl：条件
来源：http://jtr.uphjek.com

if ($a > 0) { print "正"; }
来源：http://egx.hongshengwenyu.top

[T45] Perl：数组遍历
来源：http://vit.nanxuanxn.top

for my $x (@arr) { print $x; }
来源：http://utm.shangyingyoupin.top

[T46] Perl：哈希操作
来源：http://xfj.ydzc1.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://yst.xylfe.cn

[T47] Perl：正则捕获
来源：http://ain.bbcook.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://miv.guowangkeji.top

[T48] Perl：正则替换
来源：http://upt.xuanzx.com

$s =~ s/old/new/g;
来源：http://yjn.shzxlz.cn

[T49] Perl：函数
来源：http://lwe.nwbrower.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://uss.nanxuanxn.top

[T50] Perl：逐行读文件
来源：http://mgh.chenjidiqi.icu

open my $fh, "<", "a.txt" or die $!;
来源：http://mpf.yongpay.top

while (my $line = <$fh>) { print $line; }
来源：http://nff.fehbvm.com

[T51] Scala：Hello World
来源：http://wnu.jqgfzy.top

println("Hello")
来源：http://jih.sufxvd.cn

[T52] Scala：变量
来源：http://eeb.quarkkingdee.top

val a = 1;  var b = 2
来源：http://zfw.fanxiaobao.xyz

[T53] Scala：字符串插值
来源：http://art.chenzaomai.com

s"值: $b"
来源：http://dwc.tarul.cn

[T54] Scala：集合映射
来源：http://csh.yuanzhike.top

List(1, 2, 3).map(_ * 2)
来源：http://swa.quarkkingdee.top

[T55] Scala：集合过滤
来源：http://tbf.haohaochexian.top

List(1, 2, 3).filter(_ > 1)
来源：http://ugj.snrcjt.cn

[T56] Scala：样例类
来源：http://key.ivvv.top

case class User(name: String, age: Int)
来源：http://obe.cheryme.top

[T57] Scala：模式匹配
来源：http://dqf.hnqzz.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://oru.316326.xyz

[T58] Scala：函数定义
来源：http://cjf.gotoacloud.top

def add(a: Int, b: Int): Int = a + b
来源：http://usu.xuanzx.com

[T59] Scala：循环
来源：http://skc.shangyingyoupin.top

for (i <- 1 to 10) println(i)
来源：http://smc.hammf.cn

[T60] Scala：折叠
来源：http://rvw.tian-w.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qry.dianchejie.cn

================================================================================
来源：http://ofg.cucudq.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zze.yfazqb.com

================================================================================
来源：http://krn.yj202588.top

[U01] Py：创建虚拟环境
来源：http://seq.vehdjk.com

python -m venv .venv && source .venv/bin/activate
来源：http://ulp.meibo888.top

[U02] Py：导出 / 安装依赖
来源：http://qtz.ydjk.org.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cfk.shuidangran.top

[U03] Py：加载 .env 配置
来源：http://wru.mhx1999.top

from dotenv import load_dotenv; load_dotenv()
来源：http://zrz.gaohongyu789.top

[U04] Py：变量调试打印
来源：http://juv.aizwys.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://can.meibo888.top

[U05] Py：列表去重且保序
来源：http://uvo.tarul.cn

list(dict.fromkeys(arr))
来源：http://kcw.cqqwz.cn

[U06] Py：合并两个字典
来源：http://bkz.tianlin.xyz

{**a, **b}
来源：http://dik.sysykeji.top

[U07] Py：反转字典键值
来源：http://mlk.ydjk.org.cn

{v: k for k, v in d.items()}
来源：http://joo.zycfv.cn

[U08] Py：展平二维列表
来源：http://ojg.jqgfzy.top

[y for x in nested for y in x]
来源：http://piu.jyoumei.cn

[U09] Py：字典取最大值的键
来源：http://uyi.tanke756.top

max(d, key=d.get)
来源：http://mnj.meibo888.top

[U10] Py：按值排序字典
来源：http://pib.cheryme.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qyp.zhiwuduotai.top

[U11] Py：生成器表达式
来源：http://bjq.jinqigufen.top

(x * 2 for x in arr)
来源：http://hhq.cheryme.top

[U12] Py：取出现最多的 3 个元素
来源：http://voh.ydzc1.top

Counter(arr).most_common(3)
来源：http://xfo.shzxlz.cn

[U13] Py：固定长度队列
来源：http://yhl.zdbjq.cn

deque(maxlen=10)
来源：http://out.aibaodan.cn

[U14] Py：分组收集到列表
来源：http://sde.yonumen.top

defaultdict(list)
来源：http://off.zdqjudy.top

[U15] Py：高精度计时
来源：http://xrt.jqgfzy.top

t = time.perf_counter()
来源：http://spe.fzhhl.top

[U16] Py：命令行参数解析
来源：http://onb.zhaomingkeji.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mss.jinyuanbaomall.cn

[U17] Py：初始化日志
来源：http://zlz.xuanzx.com

logging.basicConfig(level=logging.INFO)
来源：http://cqh.guowangkeji.top

[U18] Py：预编译正则
来源：http://let.zdbjq.cn

pat = re.compile(r"\d+")
来源：http://xeq.yfazqb.com

[U19] Py：正则替换带回调
来源：http://gvb.haohaochexian.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ogc.hywenlv.cn

[U20] Py：缓存函数结果
来源：http://uga.zhiwuduotai.top

@functools.lru_cache(maxsize=None)
来源：http://vzy.xziqi.cn

[U21] Py：自定义上下文管理器
来源：http://iqp.hammf.cn

@contextlib.contextmanager
来源：http://fxb.pengpengdd.cyou

[U22] Py：矩阵转置
来源：http://hgc.pengpengdd.cyou

list(zip(*m))
来源：http://seb.jlsjyb.cn

[U23] Py：分块读取大文件
来源：http://fau.fktsv.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pgy.kuanghao11.cn

[U24] Py：路径操作
来源：http://khr.shuidangran.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bpv.zhongyouzk.top

[U25] Py：CSV 按字典读
来源：http://pyp.tianlin.xyz

csv.DictReader(f)
来源：http://aep.gotoacloud.top

[U26] Py：并发下载
来源：http://kbi.tarul.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tac.guowangkeji.top

[U27] Py：异步 HTTP
来源：http://bml.zycfv.cn

aiohttp.ClientSession() 配合 async with
来源：http://sba.yanxiufei.cn

[U28] Py：类型别名
来源：http://kxm.52xcode.cn

UserId = int
来源：http://kot.jqgfzy.top

[U29] Py：属性校验
来源：http://bap.jqgfzy.top

@property 与 @x.setter 配合
来源：http://vkz.cashguo.top

[U30] Py：数据类
来源：http://prw.daria6918.cn

@dataclass(slots=True)
来源：http://yfl.cqqwz.cn

[U31] Py：单测
来源：http://qzj.svipenyu.cn

python -m pytest -q
来源：http://gsy.zdbjq.cn

[U32] Py：代码格式化
来源：http://wtc.52xcode.cn

ruff format . && ruff check --fix .
来源：http://kef.ehwqpu.com

[U33] Py：打包发布
来源：http://mai.jyoumei.cn

python -m build  （依赖 pyproject.toml）
来源：http://thc.xuanzx.com

[U34] Py：判断编码
来源：http://lzt.haohaochexian.top

chardet.detect(raw)
来源：http://fpz.yvedp.cn

[U35] Py：发送邮件
来源：http://rem.zhengqikj.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mmr.nwbrower.top

[U36] Py：定时任务
来源：http://vyc.aizwys.cn

schedule.every(10).minutes.do(job)
来源：http://hig.zhengqikj.top

[U37] Py：读写 Excel
来源：http://jfd.tianlin.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://cgc.quarkkingdee.top

[U38] Py：获取脚本所在目录
来源：http://aml.andypj.xyz

Path(__file__).resolve().parent
来源：http://esa.dashuyun.cn

[U39] Py：判断是否在交互环境
来源：http://atu.zhongyouzk.top

sys.stdout.isatty()
来源：http://jij.hammf.cn

[U40] Py：打印到标准错误
来源：http://zgn.yuxming.cn

print("err", file=sys.stderr)
来源：http://vrv.hywenlv.cn

[U41] PHP：初始化 Composer 项目
来源：http://bim.uphjek.com

composer init;  composer require guzzlehttp/guzzle
来源：http://ljz.zhongyouzk.top

[U42] PHP：PSR-4 自动加载
来源：http://vwc.fanxiaobao.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://czn.gotoacloud.top

[U43] PHP：声明命名空间
来源：http://xvj.daxiang520.top

namespace App\Http;
来源：http://xol.xylfe.cn

[U44] PHP：开启严格类型
来源：http://imv.aizwys.cn

declare(strict_types=1);
来源：http://ppe.ywan-chungtsiang.top

[U45] PHP：类型声明与返回类型
来源：http://fio.vqdsnc.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://fou.aizwys.cn

[U46] PHP：可空类型
来源：http://fqj.cashguo.top

?string $name = null
来源：http://koj.yanxiufei.cn

[U47] PHP：联合类型
来源：http://vis.jinqigfzy.top

int|string $id
来源：http://hdp.mhx1999.top

[U48] PHP：纯枚举
来源：http://kje.hywenlv.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://epn.jlsjyb.cn

[U49] PHP：只读属性
来源：http://nys.0kj1m.cn

public readonly string $name
来源：http://dgu.nanxinkj.top

[U50] PHP：构造器属性提升
来源：http://rdm.zycfv.cn

public function __construct(private int $id) {}
来源：http://wxm.fengsongda.top

[U51] PHP：数组解构
来源：http://pst.sjlbkw.cn

[$a, $b] = $arr;
来源：http://lqx.shanyushiyangkeji.top

[U52] PHP：箭头函数
来源：http://uif.daria6918.cn

$double = fn($x) => $x * 2;
来源：http://tfm.yongpay.top

[U53] PHP：空合并运算符
来源：http://pdv.pengpengdd.cyou

$v = $a ?? $b ?? "default";
来源：http://fgf.pengpengdd.cyou

[U54] PHP：空安全调用
来源：http://gmq.shzxlz.cn

$obj?->method()
来源：http://fwh.ivvv.top

[U55] PHP：match 表达式
来源：http://lxc.hnqzz.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xtw.tianlin.xyz

[U56] PHP：命名参数
来源：http://nsf.zhijiandao.cn

f(a: 1, b: 2)
来源：http://iop.pycfn.com

[U57] PHP：字符串插值
来源：http://ecj.jqgfzy.top

"值: {$a}"
来源：http://kxi.cucudq.cn

[U58] PHP：数组三件套
来源：http://wde.hcnkem.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://tbo.gaohongyu789.top

[U59] PHP：自定义排序
来源：http://htf.ywan-chungtsiang.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bzt.shanyushiyangtech.top

[U60] PHP：JSON 编解码
来源：http://yku.wangdashe.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lor.jqgufenzy.top

[U61] PHP：正则
来源：http://gng.havefunace.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://glg.ydzc1.top

[U62] PHP：日期对象
来源：http://roh.xziqi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ngb.sufxvd.cn

[U63] PHP：文件读写
来源：http://fso.jiagoushi.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ccu.zhongyouzk.top

[U64] PHP：目录遍历
来源：http://yya.hammf.cn

glob("dir/*.php");  scandir("dir");
来源：http://awh.nanxuanxn.top

[U65] PHP：会话
来源：http://szn.gotoacloud.top

session_start();  $_SESSION["uid"] = 1;
来源：http://uya.gotoacloud.top

[U66] PHP：设置 Cookie
来源：http://icc.svipenyu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fql.nwbrower.top

[U67] PHP：处理文件上传
来源：http://qli.aibaodan.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qnf.xuetiantiany.cn

[U68] PHP：PDO 连接
来源：http://bjg.iojbl.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zrt.zhixingplan.top

[U69] PHP：PDO 预处理
来源：http://mts.dashuyun.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baf.ppjwa.cn

[U70] PHP：PDO 事务
来源：http://gql.quarkkingdee.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gds.nanxinkj.top

[U71] PHP：抛出异常
来源：http://apb.9152youxi.cn

throw new RuntimeException("失败", 500);
来源：http://joi.316326.xyz

[U72] PHP：写错误日志
来源：http://jcp.aibaodan.cn

error_log("失败: " . $e->getMessage());
来源：http://ceo.zhixingplan.top

[U73] PHP：读取 ini 配置
来源：http://obv.aibaodan.cn

parse_ini_file("config.ini", true)
来源：http://znr.gogol.net.cn

[U74] PHP：读取环境变量
来源：http://uzd.daria6918.cn

getenv("APP_ENV") ?: "production"
来源：http://ufo.nanxuanxn.top

[U75] PHP：依赖注入
来源：http://iaa.jinyuanbaomall.cn

composer require psr/container
来源：http://khw.havefunace.top

[U76] PHP：简单路由
来源：http://vwa.zdbjq.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gxd.feifeiyinyue.top

[U77] PHP：模板渲染
来源：http://qye.jinqigufen.top

composer require twig/twig
来源：http://ktk.hesvh.cn

[U78] PHP：单元测试
来源：http://rjf.chenlongwang.top

composer require --dev phpunit/phpunit
来源：http://fhn.0kj1m.cn

[U79] PHP：静态分析
来源：http://ela.ydzc1.top

composer require --dev phpstan/phpstan
来源：http://yam.ywan-chungtsiang.top

[U80] PHP：代码规范修复
来源：http://tfr.guannengcc.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://oxl.nanxinkj.top

[U81] JS：初始化项目
来源：http://osk.hcnkem.com

npm init -y;  npm i express
来源：http://qmd.zhijiandao.cn

[U82] JS：package.json 脚本
来源：http://dij.0kj1m.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://anc.tarul.cn

[U83] JS：ES Module 导入导出
来源：http://kps.wangshuangyany.cn

export const a = 1;  import { a } from "./m.js";
来源：http://zbh.xuanzx.com

[U84] JS：CommonJS 写法
来源：http://scr.jinghuilouyu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://nsz.meibo888.top

[U85] JS：可选链
来源：http://xdn.chenjidiqi.icu

a?.b?.c
来源：http://mmr.shuidangran.top

[U86] JS：空值合并
来源：http://luw.gogol.net.cn

a ?? b
来源：http://dtg.yj20258888.top

[U87] JS：解构默认值
来源：http://ekj.yangfankeji.com

const { a = 1, b = 2 } = obj;
来源：http://xwg.hcnkem.com

[U88] JS：对象展开合并
来源：http://hsm.bbcook.cn

{ ...a, ...b }
来源：http://foy.zdbjq.cn

[U89] JS：数组去重
来源：http://plj.jinyuanbaomall.cn

[...new Set(arr)]
来源：http://kxb.dashuyun.cn

[U90] JS：数字数组排序
来源：http://oge.cdnleiting.top

[...arr].sort((a, b) => a - b)
来源：http://kuz.yj20258.top

[U91] JS：对象键值遍历
来源：http://lzv.havefunace.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ayn.zhongyouzk.top

[U92] JS：深拷贝
来源：http://elk.redwolf501.top

structuredClone(obj)
来源：http://qbs.nanxuanxn.top


<!-- 参考信息 -->