代发 wailian999

[T05] Kotlin：when 表达式
来源：http://rqb.chenzaomai.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://npw.tarul.cn

[T06] Kotlin：集合映射
来源：http://nqh.hesvh.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://rsl.chenlongwang.top

[T07] Kotlin：集合过滤
来源：http://yhu.nwbrower.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://tpj.ehwqpu.com

[T08] Kotlin：数据类
来源：http://lwv.jinqigfzy.top

data class User(val name: String, val age: Int)
来源：http://baq.nanxuanxn.top

[T09] Kotlin：扩展函数
来源：http://lkf.jinghuilouyu.cn

fun String.exclaim() = this + "!"
来源：http://cqs.zdbjq.cn

[T10] Kotlin：默认参数
来源：http://tmf.yueranfly.top

fun greet(name: String = "World") = "Hi $name"
来源：http://rpd.yuanzhike.top

[T11] Kotlin：协程
来源：http://dfb.c1oappe.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://odt.0kj1m.cn

[T12] Kotlin：解构声明
来源：http://vly.sweek.top

val (a, b) = Pair(1, 2)
来源：http://ltg.jyoumei.cn

[T13] Kotlin：只读 Map
来源：http://kdh.yuanzhike.top

val m = mapOf("a" to 1)
来源：http://cva.zdbjq.cn

[T14] Kotlin：循环
来源：http://znt.mhx1999.top

for (i in 1..10) println(i)
来源：http://ubp.gzhubu.top

[T15] Kotlin：接口
来源：http://tae.316326.xyz

interface Shape { fun area(): Double }
来源：http://abh.shzxlz.cn

[T16] Swift：Hello World
来源：http://zsg.zhoulong.xyz

print("Hello")
来源：http://leh.ehwqpu.com

[T17] Swift：变量与常量
来源：http://ttz.cdnleiting.top

var a = 1;  let b = 2
来源：http://vqf.cdnleiting.top

[T18] Swift：字符串插值
来源：http://kcc.gotoacloud.top

"值: \(b)"
来源：http://ujj.yj202588.top

[T19] Swift：可选绑定
来源：http://vxw.yongpay.top

if let n = opt { print(n) }
来源：http://lxl.gzhubu.top

[T20] Swift：数组操作
来源：http://xas.sweek.top

var a = [1, 2, 3];  a.append(4)
来源：http://ipu.wangshuangyany.cn

[T21] Swift：遍历
来源：http://twj.kuanghao11.cn

for x in a { print(x) }
来源：http://klh.pycfn.com

[T22] Swift：字典
来源：http://pjh.0kj1m.cn

var d = ["a": 1];  d["b"] = 2
来源：http://zbh.shzxlz.cn

[T23] Swift：函数
来源：http://ifx.guowangkeji.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ojd.sjlbkw.cn

[T24] Swift：闭包
来源：http://euc.hcnkem.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://yfs.hammf.cn

[T25] Swift：结构体
来源：http://fxa.redwolf501.top

struct P { var x: Int }
来源：http://lbp.gotoacloud.top

[T26] Swift：类与重写
来源：http://ewi.smart0.xyz

class A: Base { override func f() {} }
来源：http://vce.dashuyun.cn

[T27] Swift：错误处理
来源：http://uui.yj20258888.top

do { try f() } catch { print(error) }
来源：http://rvu.316326.xyz

[T28] Swift：枚举
来源：http://lod.dianchejie.cn

enum Color { case red, green }
来源：http://bcb.svipenyu.cn

[T29] Swift：guard 提前返回
来源：http://koz.52xcode.cn

guard let x = opt else { return }
来源：http://pmu.cashguo.top

[T30] Swift：协议
来源：http://xlx.jianghu66.top

protocol Shape { func area() -> Double }
来源：http://xtp.xylfe.cn

[T31] Lua：Hello World
来源：http://lts.fanxiaobao.xyz

print("Hello")
来源：http://kjt.jqgufenzy.top

[T32] Lua：局部变量
来源：http://xdm.vqdsnc.cn

local a = 1
来源：http://pcf.ivvv.top

[T33] Lua：表（数组）
来源：http://ijb.xziqi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://nsc.hfpthk.cn

[T34] Lua：遍历表
来源：http://glj.hnqzz.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ril.ydjk.org.cn

[T35] Lua：字典表
来源：http://utd.fehbvm.com

local d = { a = 1 };  d.b = 2
来源：http://ofr.xuetiantiany.cn

[T36] Lua：函数
来源：http://cqb.iojbl.cn

function add(a, b) return a + b end
来源：http://wpk.uphjek.com

[T37] Lua：字符串拼接
来源：http://kcu.birdmap.top

"a" .. "b"
来源：http://sqp.jqgufenzy.top

[T38] Lua：条件
来源：http://stz.chenlongwang.top

if x > 0 then print("正") end
来源：http://mlh.yongpay.top

[T39] Lua：模式匹配
来源：http://ved.feifeiyinyue.top

string.find(s, "%d+")
来源：http://xxt.redwolf501.top

[T40] Lua：元表
来源：http://idt.aizwys.cn

setmetatable({}, { __index = base })
来源：http://irh.dianchejie.cn

[T41] Perl：Hello World
来源：http://esi.sysykeji.top

print "Hello\n";
来源：http://xax.zdqjudy.top

[T42] Perl：变量类型
来源：http://aoh.bbcook.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bde.sweek.top

[T43] Perl：字符串插值
来源：http://tsc.shuidangran.top

"值: $a"
来源：http://pit.yfazqb.com

[T44] Perl：条件
来源：http://nwa.tarul.cn

if ($a > 0) { print "正"; }
来源：http://ecj.yongpay.top

[T45] Perl：数组遍历
来源：http://cjf.dashuyun.cn

for my $x (@arr) { print $x; }
来源：http://jdb.ywan-chungtsiang.top

[T46] Perl：哈希操作
来源：http://emw.hcnkem.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fse.ctjpmb.com

[T47] Perl：正则捕获
来源：http://rgb.jqgufenzy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://pev.kuanghao11.cn

[T48] Perl：正则替换
来源：http://ueo.dashuyun.cn

$s =~ s/old/new/g;
来源：http://hwk.jlsjyb.cn

[T49] Perl：函数
来源：http://ffc.jqgfzy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wip.xuanzx.com

[T50] Perl：逐行读文件
来源：http://dbr.mhx1999.top

open my $fh, "<", "a.txt" or die $!;
来源：http://bkx.52xcode.cn

while (my $line = <$fh>) { print $line; }
来源：http://rxm.chenlongwang.top

[T51] Scala：Hello World
来源：http://lbz.ehwqpu.com

println("Hello")
来源：http://orr.haohaochexian.top

[T52] Scala：变量
来源：http://vit.shzxlz.cn

val a = 1;  var b = 2
来源：http://oje.yonumen.top

[T53] Scala：字符串插值
来源：http://vlt.jinghuilouyu.cn

s"值: $b"
来源：http://djw.xinyue.icu

[T54] Scala：集合映射
来源：http://vcv.tarul.cn

List(1, 2, 3).map(_ * 2)
来源：http://sfl.316326.xyz

[T55] Scala：集合过滤
来源：http://eey.xylfe.cn

List(1, 2, 3).filter(_ > 1)
来源：http://occ.xylfe.cn

[T56] Scala：样例类
来源：http://cev.fzhhl.top

case class User(name: String, age: Int)
来源：http://zxi.quarkkingdee.top

[T57] Scala：模式匹配
来源：http://luu.xuanzx.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://npt.cashguo.top

[T58] Scala：函数定义
来源：http://dfj.yj20258.top

def add(a: Int, b: Int): Int = a + b
来源：http://cmp.ppjwa.cn

[T59] Scala：循环
来源：http://gou.havefunace.top

for (i <- 1 to 10) println(i)
来源：http://hou.9152youxi.cn

[T60] Scala：折叠
来源：http://dfh.yuanzhike.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vhg.guowangkeji.top

================================================================================
来源：http://wce.chenjidiqi.icu

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jeq.kuanghao11.cn

================================================================================
来源：http://hir.cucudq.cn

[U01] Py：创建虚拟环境
来源：http://pew.ivvv.top

python -m venv .venv && source .venv/bin/activate
来源：http://muy.0kj1m.cn

[U02] Py：导出 / 安装依赖
来源：http://vpw.hywenlv.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://err.jinyuanbaomall.cn

[U03] Py：加载 .env 配置
来源：http://kav.sjlbkw.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://gbu.pengpengdd.cyou

[U04] Py：变量调试打印
来源：http://jnq.nanxuanxn.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qjx.sweek.top

[U05] Py：列表去重且保序
来源：http://ltw.meibo888.top

list(dict.fromkeys(arr))
来源：http://oqo.dianchejie.cn

[U06] Py：合并两个字典
来源：http://rqd.cucudq.cn

{**a, **b}
来源：http://yfd.ehwqpu.com

[U07] Py：反转字典键值
来源：http://zeu.ybcxt.top

{v: k for k, v in d.items()}
来源：http://dfu.yueranfly.top

[U08] Py：展平二维列表
来源：http://yft.hysaishi.cn

[y for x in nested for y in x]
来源：http://rka.shangyingyoupin.top

[U09] Py：字典取最大值的键
来源：http://ndz.havefunace.top

max(d, key=d.get)
来源：http://kqb.xinyue.icu

[U10] Py：按值排序字典
来源：http://mag.jiagoushi.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ypn.jianghu66.top

[U11] Py：生成器表达式
来源：http://dxa.shangyingyoupin.top

(x * 2 for x in arr)
来源：http://ynm.shanyushiyangkeji.top

[U12] Py：取出现最多的 3 个元素
来源：http://jdp.jlsjyb.cn

Counter(arr).most_common(3)
来源：http://xqx.xuanzx.com

[U13] Py：固定长度队列
来源：http://fdd.ydjk.org.cn

deque(maxlen=10)
来源：http://owt.redwolf501.top

[U14] Py：分组收集到列表
来源：http://hom.vehdjk.com

defaultdict(list)
来源：http://gzu.hesvh.cn

[U15] Py：高精度计时
来源：http://luk.yangfankeji.com

t = time.perf_counter()
来源：http://iwn.bjfxy.top

[U16] Py：命令行参数解析
来源：http://cgg.cashguo.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://tzr.316326.xyz

[U17] Py：初始化日志
来源：http://dpy.hammf.cn

logging.basicConfig(level=logging.INFO)
来源：http://ibu.zhijiandao.cn

[U18] Py：预编译正则
来源：http://biy.ydzc1.top

pat = re.compile(r"\d+")
来源：http://xam.yongpay.top

[U19] Py：正则替换带回调
来源：http://ril.yj20258888.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hzg.tanke756.top

[U20] Py：缓存函数结果
来源：http://mry.havefunace.top

@functools.lru_cache(maxsize=None)
来源：http://wfc.smart0.xyz

[U21] Py：自定义上下文管理器
来源：http://yqm.hcnkem.com

@contextlib.contextmanager
来源：http://iin.iojbl.cn

[U22] Py：矩阵转置
来源：http://hco.cheryme.top

list(zip(*m))
来源：http://dfs.snrcjt.cn

[U23] Py：分块读取大文件
来源：http://faw.tian-w.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ntf.guannengcc.top

[U24] Py：路径操作
来源：http://jhf.wangshuangyany.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gdr.zhixingplan.top

[U25] Py：CSV 按字典读
来源：http://lsj.aizwys.cn

csv.DictReader(f)
来源：http://ybh.tian-w.cn

[U26] Py：并发下载
来源：http://mzw.gogol.net.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ckp.ywan-chungtsiang.top

[U27] Py：异步 HTTP
来源：http://coo.jyoumei.cn

aiohttp.ClientSession() 配合 async with
来源：http://krn.ybcxt.top

[U28] Py：类型别名
来源：http://qdq.hnxiangtu.top

UserId = int
来源：http://vzf.cdnleiting.top

[U29] Py：属性校验
来源：http://jym.fanxiaobao.xyz

@property 与 @x.setter 配合
来源：http://qlz.cheryme.top

[U30] Py：数据类
来源：http://cfq.fehbvm.com

@dataclass(slots=True)
来源：http://vfp.cqqwz.cn

[U31] Py：单测
来源：http://sdm.shzxlz.cn

python -m pytest -q
来源：http://ufn.gaohongyu789.top

[U32] Py：代码格式化
来源：http://rge.yonumen.top

ruff format . && ruff check --fix .
来源：http://uea.redwolf501.top

[U33] Py：打包发布
来源：http://boh.vehdjk.com

python -m build  （依赖 pyproject.toml）
来源：http://mcq.yongpay.top

[U34] Py：判断编码
来源：http://raf.jinqigfzy.top

chardet.detect(raw)
来源：http://rcs.hammf.cn

[U35] Py：发送邮件
来源：http://rmz.hongshengwenyu.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fcq.pengpengdd.cyou

[U36] Py：定时任务
来源：http://wsg.gzhubu.top

schedule.every(10).minutes.do(job)
来源：http://jtb.fanxiaobao.xyz

[U37] Py：读写 Excel
来源：http://ngs.yanxiufei.cn

pandas.read_excel / DataFrame.to_excel
来源：http://dxs.zhixingplan.top

[U38] Py：获取脚本所在目录
来源：http://gxb.fktsv.cn

Path(__file__).resolve().parent
来源：http://tqr.jinghuilouyu.cn

[U39] Py：判断是否在交互环境
来源：http://ogy.smart0.xyz

sys.stdout.isatty()
来源：http://kqz.jlsjyb.cn

[U40] Py：打印到标准错误
来源：http://uaq.hcnkem.com

print("err", file=sys.stderr)
来源：http://sds.sjlbkw.cn

[U41] PHP：初始化 Composer 项目
来源：http://csn.fktsv.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://lzn.mhx1999.top

[U42] PHP：PSR-4 自动加载
来源：http://pvx.cdnleiting.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://riz.wangshuangyany.cn

[U43] PHP：声明命名空间
来源：http://fyp.fktsv.cn

namespace App\Http;
来源：http://iee.xziqi.cn

[U44] PHP：开启严格类型
来源：http://kbc.sjlbkw.cn

declare(strict_types=1);
来源：http://tbm.vehdjk.com

[U45] PHP：类型声明与返回类型
来源：http://nsk.ydzc1.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://xnj.gaohongyu789.top

[U46] PHP：可空类型
来源：http://wdh.0kj1m.cn

?string $name = null
来源：http://xfo.fktsv.cn

[U47] PHP：联合类型
来源：http://mny.havefunace.top

int|string $id
来源：http://jwi.gzhubu.top

[U48] PHP：纯枚举
来源：http://nrs.gotoacloud.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lzx.bjfxy.top

[U49] PHP：只读属性
来源：http://cwj.smart0.xyz

public readonly string $name
来源：http://qcv.zhaomingkeji.xyz

[U50] PHP：构造器属性提升
来源：http://ire.smart0.xyz

public function __construct(private int $id) {}
来源：http://jac.zdbjq.cn

[U51] PHP：数组解构
来源：http://pzg.aizwys.cn

[$a, $b] = $arr;
来源：http://ett.haohaochexian.top

[U52] PHP：箭头函数
来源：http://rgb.daria6918.cn

$double = fn($x) => $x * 2;
来源：http://xxt.jqgufenzy.top

[U53] PHP：空合并运算符
来源：http://dfl.sysykeji.top

$v = $a ?? $b ?? "default";
来源：http://ycx.yanxiufei.cn

[U54] PHP：空安全调用
来源：http://stl.cheryme.top

$obj?->method()
来源：http://lvd.xuanzx.com

[U55] PHP：match 表达式
来源：http://wbv.cqqwz.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://pfj.gaohongyu789.top

[U56] PHP：命名参数
来源：http://ibz.fktsv.cn

f(a: 1, b: 2)
来源：http://zjf.fzhhl.top

[U57] PHP：字符串插值
来源：http://pyt.yonumen.top

"值: {$a}"
来源：http://ccc.xuetiantiany.cn

[U58] PHP：数组三件套
来源：http://rul.fehbvm.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zhu.xziqi.cn

[U59] PHP：自定义排序
来源：http://ujb.jianghu66.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dyz.yvedp.cn

[U60] PHP：JSON 编解码
来源：http://szk.guowangkeji.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lav.zhixingplan.top

[U61] PHP：正则
来源：http://bry.sxryk.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hqz.hammf.cn

[U62] PHP：日期对象
来源：http://mwa.birdmap.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://orl.ctjpmb.com

[U63] PHP：文件读写
来源：http://enk.yuanzhike.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://nxa.havefunace.top

[U64] PHP：目录遍历
来源：http://sjy.havefunace.top

glob("dir/*.php");  scandir("dir");
来源：http://rqd.ppjwa.cn

[U65] PHP：会话
来源：http://jbn.zhongyouzk.top

session_start();  $_SESSION["uid"] = 1;
来源：http://jiu.jqgufenzy.top

[U66] PHP：设置 Cookie
来源：http://huj.bbcook.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://svr.nwbrower.top

[U67] PHP：处理文件上传
来源：http://ypk.nwbrower.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://oxy.vehdjk.com

[U68] PHP：PDO 连接
来源：http://bqf.gzhubu.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ehs.9152youxi.cn

[U69] PHP：PDO 预处理
来源：http://ryb.chenlongwang.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vdj.zhixingplan.top

[U70] PHP：PDO 事务
来源：http://arw.9152youxi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://cil.gzhubu.top

[U71] PHP：抛出异常
来源：http://kev.bjfxy.top

throw new RuntimeException("失败", 500);
来源：http://nhu.zhiwuduotai.top

[U72] PHP：写错误日志
来源：http://ymw.bbcook.cn

error_log("失败: " . $e->getMessage());
来源：http://lxq.gotoacloud.top

[U73] PHP：读取 ini 配置
来源：http://dev.cucudq.cn

parse_ini_file("config.ini", true)
来源：http://hsl.sweek.top

[U74] PHP：读取环境变量
来源：http://wzg.hammf.cn

getenv("APP_ENV") ?: "production"
来源：http://yar.sufxvd.cn

[U75] PHP：依赖注入
来源：http://gno.jlsjyb.cn

composer require psr/container
来源：http://hdq.smart0.xyz

[U76] PHP：简单路由
来源：http://sgt.mhx1999.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rmn.shuidangran.top

[U77] PHP：模板渲染
来源：http://ifm.guannengcc.top

composer require twig/twig
来源：http://chm.ydjk.org.cn

[U78] PHP：单元测试
来源：http://hjm.hnqzz.top

composer require --dev phpunit/phpunit
来源：http://rlt.yj20258888.top

[U79] PHP：静态分析
来源：http://ery.fzhhl.top

composer require --dev phpstan/phpstan
来源：http://jvl.andypj.xyz

[U80] PHP：代码规范修复
来源：http://wzy.nanxuanxn.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://jkv.hywenlv.cn

[U81] JS：初始化项目
来源：http://avf.hongshengwenyu.top

npm init -y;  npm i express
来源：http://rfm.cheryme.top

[U82] JS：package.json 脚本
来源：http://yrz.hammf.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hwx.haohaochexian.top

[U83] JS：ES Module 导入导出
来源：http://wjz.tian-w.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ehq.ppjwa.cn

[U84] JS：CommonJS 写法
来源：http://lnf.havefunace.top

module.exports = { a };  const { a } = require("./m");
来源：http://zsh.cashguo.top

[U85] JS：可选链
来源：http://hpk.xuetiantiany.cn

a?.b?.c
来源：http://yzx.hnxiangtu.top

[U86] JS：空值合并
来源：http://fap.zhixingplan.top

a ?? b
来源：http://qjs.jqgfzy.top

[U87] JS：解构默认值
来源：http://cpm.cucudq.cn

const { a = 1, b = 2 } = obj;
来源：http://jju.gzhubu.top

[U88] JS：对象展开合并
来源：http://yyl.fanxiaobao.xyz

{ ...a, ...b }
来源：http://cmt.hnxiangtu.top

[U89] JS：数组去重
来源：http://mos.vehdjk.com

[...new Set(arr)]
来源：http://xxk.gaohongyu789.top

[U90] JS：数字数组排序
来源：http://xzc.cashguo.top

[...arr].sort((a, b) => a - b)
来源：http://muf.sjlbkw.cn

[U91] JS：对象键值遍历
来源：http://hto.jinqigufen.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mzs.ivvv.top

[U92] JS：深拷贝
来源：http://klu.feifeiyinyue.top

structuredClone(obj)
来源：http://sdr.zhixingplan.top


<!-- 参考信息 -->