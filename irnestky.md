代发 wailian999

[T07] Kotlin：集合过滤
来源：http://lpx.ywan-chungtsiang.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://sxf.jlsjyb.cn

[T08] Kotlin：数据类
来源：http://xzj.xuanzx.com

data class User(val name: String, val age: Int)
来源：http://njm.zhaomingkeji.xyz

[T09] Kotlin：扩展函数
来源：http://fdb.jyoumei.cn

fun String.exclaim() = this + "!"
来源：http://ddm.epnwcf.com

[T10] Kotlin：默认参数
来源：http://zst.yangfankeji.com

fun greet(name: String = "World") = "Hi $name"
来源：http://jvo.hnqzz.top

[T11] Kotlin：协程
来源：http://uqz.zhoulong.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://uar.hysaishi.cn

[T12] Kotlin：解构声明
来源：http://xvk.fanxiaobao.xyz

val (a, b) = Pair(1, 2)
来源：http://fue.havefunace.top

[T13] Kotlin：只读 Map
来源：http://brn.zhongyouzk.top

val m = mapOf("a" to 1)
来源：http://hov.sweek.top

[T14] Kotlin：循环
来源：http://bgc.hongshengwenyu.top

for (i in 1..10) println(i)
来源：http://for.yfazqb.com

[T15] Kotlin：接口
来源：http://rmy.sjlbkw.cn

interface Shape { fun area(): Double }
来源：http://mks.hesvh.cn

[T16] Swift：Hello World
来源：http://mbl.jlsjyb.cn

print("Hello")
来源：http://tbv.hongshengwenyu.top

[T17] Swift：变量与常量
来源：http://amz.hcnkem.com

var a = 1;  let b = 2
来源：http://uls.shangyingyoupin.top

[T18] Swift：字符串插值
来源：http://acd.shuidangran.top

"值: \(b)"
来源：http://oya.yj20258.top

[T19] Swift：可选绑定
来源：http://igf.vqdsnc.cn

if let n = opt { print(n) }
来源：http://trl.aibaodan.cn

[T20] Swift：数组操作
来源：http://ypw.gotoacloud.top

var a = [1, 2, 3];  a.append(4)
来源：http://zkc.hnqzz.top

[T21] Swift：遍历
来源：http://gvg.aibaodan.cn

for x in a { print(x) }
来源：http://rim.redwolf501.top

[T22] Swift：字典
来源：http://ckb.snrcjt.cn

var d = ["a": 1];  d["b"] = 2
来源：http://lhf.xingfuxueyuan.xyz

[T23] Swift：函数
来源：http://ikf.sysykeji.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dcx.hammf.cn

[T24] Swift：闭包
来源：http://teg.gogol.net.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://iui.zhaomingkeji.xyz

[T25] Swift：结构体
来源：http://hjh.havefunace.top

struct P { var x: Int }
来源：http://kqq.pengpengdd.cyou

[T26] Swift：类与重写
来源：http://haz.fanxiaobao.xyz

class A: Base { override func f() {} }
来源：http://zeu.fehbvm.com

[T27] Swift：错误处理
来源：http://ejy.uphjek.com

do { try f() } catch { print(error) }
来源：http://abb.zdqjudy.top

[T28] Swift：枚举
来源：http://xnj.nanxinkj.top

enum Color { case red, green }
来源：http://gma.quarkkingdee.top

[T29] Swift：guard 提前返回
来源：http://zoh.ppjwa.cn

guard let x = opt else { return }
来源：http://lmz.yanxiufei.cn

[T30] Swift：协议
来源：http://ujg.nanxuanxn.top

protocol Shape { func area() -> Double }
来源：http://crb.guowangkeji.top

[T31] Lua：Hello World
来源：http://bxu.zhengqikj.top

print("Hello")
来源：http://mwh.yj20258888.top

[T32] Lua：局部变量
来源：http://knp.jinghuilouyu.cn

local a = 1
来源：http://ptn.gotoacloud.top

[T33] Lua：表（数组）
来源：http://nui.hnxiangtu.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ali.shuidangran.top

[T34] Lua：遍历表
来源：http://cxc.cdnleiting.top

for i, v in ipairs(t) do print(i, v) end
来源：http://zeh.ctjpmb.com

[T35] Lua：字典表
来源：http://coq.havefunace.top

local d = { a = 1 };  d.b = 2
来源：http://iqo.aizwys.cn

[T36] Lua：函数
来源：http://zaf.ivvv.top

function add(a, b) return a + b end
来源：http://qya.wangshuangyany.cn

[T37] Lua：字符串拼接
来源：http://ijy.xuetiantiany.cn

"a" .. "b"
来源：http://oio.meibo888.top

[T38] Lua：条件
来源：http://kgq.zhaomingkeji.xyz

if x > 0 then print("正") end
来源：http://jkm.52xcode.cn

[T39] Lua：模式匹配
来源：http://lvw.dashuyun.cn

string.find(s, "%d+")
来源：http://jcr.fehbvm.com

[T40] Lua：元表
来源：http://rmd.nanxinkj.top

setmetatable({}, { __index = base })
来源：http://fxm.uphjek.com

[T41] Perl：Hello World
来源：http://nub.gogol.net.cn

print "Hello\n";
来源：http://hnh.daria6918.cn

[T42] Perl：变量类型
来源：http://nud.shuidangran.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jhb.jianghu66.top

[T43] Perl：字符串插值
来源：http://vpc.dashuyun.cn

"值: $a"
来源：http://ikx.aizwys.cn

[T44] Perl：条件
来源：http://xep.epnwcf.com

if ($a > 0) { print "正"; }
来源：http://znx.jinghuilouyu.cn

[T45] Perl：数组遍历
来源：http://xwa.shzxlz.cn

for my $x (@arr) { print $x; }
来源：http://qiz.jlsjyb.cn

[T46] Perl：哈希操作
来源：http://rfb.hnqzz.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bob.zhoulong.xyz

[T47] Perl：正则捕获
来源：http://nfe.yongpay.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://wrw.havefunace.top

[T48] Perl：正则替换
来源：http://dse.ywan-chungtsiang.top

$s =~ s/old/new/g;
来源：http://rpi.sysykeji.top

[T49] Perl：函数
来源：http://mtw.ctjpmb.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sxf.dashuyun.cn

[T50] Perl：逐行读文件
来源：http://vhc.xuetiantiany.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://fxa.yj202588.top

while (my $line = <$fh>) { print $line; }
来源：http://jza.cheryme.top

[T51] Scala：Hello World
来源：http://oxi.xylfe.cn

println("Hello")
来源：http://dqm.tian-w.cn

[T52] Scala：变量
来源：http://viw.52xcode.cn

val a = 1;  var b = 2
来源：http://vdd.yuanzhike.top

[T53] Scala：字符串插值
来源：http://lmk.shanyushiyangkeji.top

s"值: $b"
来源：http://bcd.bbcook.cn

[T54] Scala：集合映射
来源：http://sgk.hongshengwenyu.top

List(1, 2, 3).map(_ * 2)
来源：http://wtq.zdqjudy.top

[T55] Scala：集合过滤
来源：http://qsx.ctjpmb.com

List(1, 2, 3).filter(_ > 1)
来源：http://epl.uphjek.com

[T56] Scala：样例类
来源：http://ild.fzhhl.top

case class User(name: String, age: Int)
来源：http://hev.sjlbkw.cn

[T57] Scala：模式匹配
来源：http://wod.jqgfzy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://oxj.aibaodan.cn

[T58] Scala：函数定义
来源：http://wtl.yonumen.top

def add(a: Int, b: Int): Int = a + b
来源：http://dfc.tianlin.xyz

[T59] Scala：循环
来源：http://lkg.cqqwz.cn

for (i <- 1 to 10) println(i)
来源：http://wmn.quarkkingdee.top

[T60] Scala：折叠
来源：http://reb.sufxvd.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://uff.hongshengwenyu.top

================================================================================
来源：http://xts.yuanzhike.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xvn.cdnleiting.top

================================================================================
来源：http://phu.hcnkem.com

[U01] Py：创建虚拟环境
来源：http://fwi.vqdsnc.cn

python -m venv .venv && source .venv/bin/activate
来源：http://dpn.jinyuanbaomall.cn

[U02] Py：导出 / 安装依赖
来源：http://vjf.ppjwa.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ipc.chenlongwang.top

[U03] Py：加载 .env 配置
来源：http://akp.redwolf501.top

from dotenv import load_dotenv; load_dotenv()
来源：http://dqq.hysaishi.cn

[U04] Py：变量调试打印
来源：http://wck.shanyushiyangkeji.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://swt.zycfv.cn

[U05] Py：列表去重且保序
来源：http://tvc.haohaochexian.top

list(dict.fromkeys(arr))
来源：http://vtr.cucudq.cn

[U06] Py：合并两个字典
来源：http://oex.meibo888.top

{**a, **b}
来源：http://rjt.hysaishi.cn

[U07] Py：反转字典键值
来源：http://nmr.nwbrower.top

{v: k for k, v in d.items()}
来源：http://lcs.yuanzhike.top

[U08] Py：展平二维列表
来源：http://mow.jinghuilouyu.cn

[y for x in nested for y in x]
来源：http://wer.sufxvd.cn

[U09] Py：字典取最大值的键
来源：http://sxe.ydzc1.top

max(d, key=d.get)
来源：http://cxd.tarul.cn

[U10] Py：按值排序字典
来源：http://emn.yonumen.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ekm.kuanghao11.cn

[U11] Py：生成器表达式
来源：http://rbs.yj202588.top

(x * 2 for x in arr)
来源：http://miy.havefunace.top

[U12] Py：取出现最多的 3 个元素
来源：http://wmx.sweek.top

Counter(arr).most_common(3)
来源：http://tef.shuidangran.top

[U13] Py：固定长度队列
来源：http://sgr.hongshengwenyu.top

deque(maxlen=10)
来源：http://wfh.zhengqikj.top

[U14] Py：分组收集到列表
来源：http://dzh.nanxuanxn.top

defaultdict(list)
来源：http://edu.tanke756.top

[U15] Py：高精度计时
来源：http://alk.yfazqb.com

t = time.perf_counter()
来源：http://pfq.jlsjyb.cn

[U16] Py：命令行参数解析
来源：http://iva.zycfv.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://iik.aibaodan.cn

[U17] Py：初始化日志
来源：http://wbc.jiagoushi.top

logging.basicConfig(level=logging.INFO)
来源：http://uhf.jqgufenzy.top

[U18] Py：预编译正则
来源：http://grv.dianchejie.cn

pat = re.compile(r"\d+")
来源：http://gcv.cashguo.top

[U19] Py：正则替换带回调
来源：http://oqy.snrcjt.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xyi.jlsjyb.cn

[U20] Py：缓存函数结果
来源：http://jpi.ppjwa.cn

@functools.lru_cache(maxsize=None)
来源：http://yvh.meibo888.top

[U21] Py：自定义上下文管理器
来源：http://tig.dashuyun.cn

@contextlib.contextmanager
来源：http://yss.sufxvd.cn

[U22] Py：矩阵转置
来源：http://vvb.jqgufenzy.top

list(zip(*m))
来源：http://gvl.shangyingyoupin.top

[U23] Py：分块读取大文件
来源：http://tml.ywan-chungtsiang.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pfw.yfazqb.com

[U24] Py：路径操作
来源：http://ibe.ywan-chungtsiang.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://oft.birdmap.top

[U25] Py：CSV 按字典读
来源：http://uiv.cqqwz.cn

csv.DictReader(f)
来源：http://yrp.yj202588.top

[U26] Py：并发下载
来源：http://tvh.yongpay.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://cgf.chenlongwang.top

[U27] Py：异步 HTTP
来源：http://byv.chenzaomai.com

aiohttp.ClientSession() 配合 async with
来源：http://tlv.havefunace.top

[U28] Py：类型别名
来源：http://vel.nanxinkj.top

UserId = int
来源：http://fpn.svipenyu.cn

[U29] Py：属性校验
来源：http://yyv.gotoacloud.top

@property 与 @x.setter 配合
来源：http://yvu.bbcook.cn

[U30] Py：数据类
来源：http://txb.hywenlv.cn

@dataclass(slots=True)
来源：http://hfw.jqgfzy.top

[U31] Py：单测
来源：http://lek.feifeiyinyue.top

python -m pytest -q
来源：http://uqq.yangfankeji.com

[U32] Py：代码格式化
来源：http://gaw.mhx1999.top

ruff format . && ruff check --fix .
来源：http://ptb.havefunace.top

[U33] Py：打包发布
来源：http://izf.birdmap.top

python -m build  （依赖 pyproject.toml）
来源：http://ndx.wangdashe.top

[U34] Py：判断编码
来源：http://end.pycfn.com

chardet.detect(raw)
来源：http://jhy.hammf.cn

[U35] Py：发送邮件
来源：http://gem.ywan-chungtsiang.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zvw.wangshuangyany.cn

[U36] Py：定时任务
来源：http://yjt.hnqzz.top

schedule.every(10).minutes.do(job)
来源：http://xni.cqqwz.cn

[U37] Py：读写 Excel
来源：http://jwa.zhaomingkeji.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://nxb.ehwqpu.com

[U38] Py：获取脚本所在目录
来源：http://amu.sufxvd.cn

Path(__file__).resolve().parent
来源：http://bnb.uphjek.com

[U39] Py：判断是否在交互环境
来源：http://rnz.ydjk.org.cn

sys.stdout.isatty()
来源：http://jad.quarkkingdee.top

[U40] Py：打印到标准错误
来源：http://rwa.feifeiyinyue.top

print("err", file=sys.stderr)
来源：http://rdj.yanxiufei.cn

[U41] PHP：初始化 Composer 项目
来源：http://mae.hesvh.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ufz.52xcode.cn

[U42] PHP：PSR-4 自动加载
来源：http://axw.jinqigufen.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fkd.c1oappe.top

[U43] PHP：声明命名空间
来源：http://drl.redwolf501.top

namespace App\Http;
来源：http://ogf.ydzc1.top

[U44] PHP：开启严格类型
来源：http://mfw.bbcook.cn

declare(strict_types=1);
来源：http://iqa.jlsjyb.cn

[U45] PHP：类型声明与返回类型
来源：http://sxg.hongshengwenyu.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://adl.fzhhl.top

[U46] PHP：可空类型
来源：http://wps.shangyingyoupin.top

?string $name = null
来源：http://tkz.shzxlz.cn

[U47] PHP：联合类型
来源：http://zfh.hnqzz.top

int|string $id
来源：http://sgj.kuanghao11.cn

[U48] PHP：纯枚举
来源：http://mim.zhixingplan.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://csf.ydjk.org.cn

[U49] PHP：只读属性
来源：http://rwe.shanyushiyangkeji.top

public readonly string $name
来源：http://lvi.cashguo.top

[U50] PHP：构造器属性提升
来源：http://lsp.zhixingplan.top

public function __construct(private int $id) {}
来源：http://ffj.sufxvd.cn

[U51] PHP：数组解构
来源：http://xig.havefunace.top

[$a, $b] = $arr;
来源：http://gqn.tanke756.top

[U52] PHP：箭头函数
来源：http://sgd.vehdjk.com

$double = fn($x) => $x * 2;
来源：http://mcx.dashuyun.cn

[U53] PHP：空合并运算符
来源：http://cbk.zhixingplan.top

$v = $a ?? $b ?? "default";
来源：http://qfm.zdqjudy.top

[U54] PHP：空安全调用
来源：http://bbd.dashuyun.cn

$obj?->method()
来源：http://pik.jinghuilouyu.cn

[U55] PHP：match 表达式
来源：http://drv.chenlongwang.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ohy.hcnkem.com

[U56] PHP：命名参数
来源：http://hln.fehbvm.com

f(a: 1, b: 2)
来源：http://ccx.cheryme.top

[U57] PHP：字符串插值
来源：http://yco.andypj.xyz

"值: {$a}"
来源：http://zyb.ppjwa.cn

[U58] PHP：数组三件套
来源：http://hlh.zhijiandao.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pip.cqqwz.cn

[U59] PHP：自定义排序
来源：http://ham.cashguo.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://woh.yuxming.cn

[U60] PHP：JSON 编解码
来源：http://jtr.tanke756.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://doo.iojbl.cn

[U61] PHP：正则
来源：http://wtx.nanxinkj.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jng.sweek.top

[U62] PHP：日期对象
来源：http://gxm.gogol.net.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://sxr.zhaomingkeji.xyz

[U63] PHP：文件读写
来源：http://tsr.yuanzhike.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ddg.hnxiangtu.top

[U64] PHP：目录遍历
来源：http://wev.yvedp.cn

glob("dir/*.php");  scandir("dir");
来源：http://zka.9152youxi.cn

[U65] PHP：会话
来源：http://zsa.xziqi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://kvd.yj20258.top

[U66] PHP：设置 Cookie
来源：http://jhm.xinyue.icu

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bak.hfpthk.cn

[U67] PHP：处理文件上传
来源：http://nhl.guowangkeji.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qik.nanxuanxn.top

[U68] PHP：PDO 连接
来源：http://jxf.ybcxt.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pyo.jlsjyb.cn

[U69] PHP：PDO 预处理
来源：http://dhy.epnwcf.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fod.zhixingplan.top

[U70] PHP：PDO 事务
来源：http://rcd.zhixingplan.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jyk.316326.xyz

[U71] PHP：抛出异常
来源：http://uxu.tanke756.top

throw new RuntimeException("失败", 500);
来源：http://bqe.pengpengdd.cyou

[U72] PHP：写错误日志
来源：http://nyu.zhixingplan.top

error_log("失败: " . $e->getMessage());
来源：http://ygk.zhijiandao.cn

[U73] PHP：读取 ini 配置
来源：http://ofo.svipenyu.cn

parse_ini_file("config.ini", true)
来源：http://mzc.shanyushiyangkeji.top

[U74] PHP：读取环境变量
来源：http://hkr.jyoumei.cn

getenv("APP_ENV") ?: "production"
来源：http://sex.hnqzz.top

[U75] PHP：依赖注入
来源：http://udk.shuidangran.top

composer require psr/container
来源：http://twp.jqgufenzy.top

[U76] PHP：简单路由
来源：http://mmt.jyoumei.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hth.ydzc1.top

[U77] PHP：模板渲染
来源：http://iki.jinghuilouyu.cn

composer require twig/twig
来源：http://udq.ywan-chungtsiang.top

[U78] PHP：单元测试
来源：http://leh.bjfxy.top

composer require --dev phpunit/phpunit
来源：http://gdt.316326.xyz

[U79] PHP：静态分析
来源：http://nzv.quarkkingdee.top

composer require --dev phpstan/phpstan
来源：http://mez.hammf.cn

[U80] PHP：代码规范修复
来源：http://ejf.hywenlv.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://rpk.hnxiangtu.top

[U81] JS：初始化项目
来源：http://lgj.cheryme.top

npm init -y;  npm i express
来源：http://xcz.vqdsnc.cn

[U82] JS：package.json 脚本
来源：http://myv.xuetiantiany.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lcl.zdbjq.cn

[U83] JS：ES Module 导入导出
来源：http://sww.nwbrower.top

export const a = 1;  import { a } from "./m.js";
来源：http://igt.yj20258.top

[U84] JS：CommonJS 写法
来源：http://xcd.gogol.net.cn

module.exports = { a };  const { a } = require("./m");
来源：http://wwc.yvedp.cn

[U85] JS：可选链
来源：http://rsc.xziqi.cn

a?.b?.c
来源：http://sxe.epnwcf.com

[U86] JS：空值合并
来源：http://qyk.jianghu66.top

a ?? b
来源：http://bgx.svipenyu.cn

[U87] JS：解构默认值
来源：http://xkm.snrcjt.cn

const { a = 1, b = 2 } = obj;
来源：http://oow.gzhubu.top

[U88] JS：对象展开合并
来源：http://log.iojbl.cn

{ ...a, ...b }
来源：http://fen.chenjidiqi.icu

[U89] JS：数组去重
来源：http://nak.jinyuanbaomall.cn

[...new Set(arr)]
来源：http://udp.zhixingplan.top

[U90] JS：数字数组排序
来源：http://hdl.chenzaomai.com

[...arr].sort((a, b) => a - b)
来源：http://uvi.jinghuilouyu.cn

[U91] JS：对象键值遍历
来源：http://sns.zhiwuduotai.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://oll.yanxiufei.cn

[U92] JS：深拷贝
来源：http://mwi.chenzaomai.com

structuredClone(obj)
来源：http://jrg.guannengcc.top

[U93] JS：模板字符串
来源：http://eqd.hfpthk.cn

`共 ${n} 条`
来源：http://ial.tarul.cn

[U94] JS：箭头函数
来源：http://lyn.quarkkingdee.top

const double = x => x * 2;
来源：http://pgz.pycfn.com


<!-- 参考信息 -->