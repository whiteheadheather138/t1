代发 wailian999

[T09] Kotlin：扩展函数
来源：http://ygq.hammf.cn

fun String.exclaim() = this + "!"
来源：http://znt.zhoulong.xyz

[T10] Kotlin：默认参数
来源：http://oxs.yueranfly.top

fun greet(name: String = "World") = "Hi $name"
来源：http://vxm.yangfankeji.com

[T11] Kotlin：协程
来源：http://orb.nwbrower.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://qut.yj202588.top

[T12] Kotlin：解构声明
来源：http://rzd.sysykeji.top

val (a, b) = Pair(1, 2)
来源：http://cyp.zhongyouzk.top

[T13] Kotlin：只读 Map
来源：http://tfn.yj20258.top

val m = mapOf("a" to 1)
来源：http://ggo.xziqi.cn

[T14] Kotlin：循环
来源：http://wwd.chenjidiqi.icu

for (i in 1..10) println(i)
来源：http://nbp.bbcook.cn

[T15] Kotlin：接口
来源：http://ckt.zhijiandao.cn

interface Shape { fun area(): Double }
来源：http://eum.xuanzx.com

[T16] Swift：Hello World
来源：http://lyk.hesvh.cn

print("Hello")
来源：http://yht.wangdashe.top

[T17] Swift：变量与常量
来源：http://wai.c1oappe.top

var a = 1;  let b = 2
来源：http://gqk.xinyue.icu

[T18] Swift：字符串插值
来源：http://yzb.fzhhl.top

"值: \(b)"
来源：http://tla.yuanzhike.top

[T19] Swift：可选绑定
来源：http://qel.aibaodan.cn

if let n = opt { print(n) }
来源：http://icn.epnwcf.com

[T20] Swift：数组操作
来源：http://whz.tianlin.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://cie.aibaodan.cn

[T21] Swift：遍历
来源：http://hyq.fehbvm.com

for x in a { print(x) }
来源：http://cbf.hongshengwenyu.top

[T22] Swift：字典
来源：http://eiq.yuanzhike.top

var d = ["a": 1];  d["b"] = 2
来源：http://cjo.yanxiufei.cn

[T23] Swift：函数
来源：http://tku.ppjwa.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xvc.ywan-chungtsiang.top

[T24] Swift：闭包
来源：http://jpx.zhaomingkeji.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://izq.aibaodan.cn

[T25] Swift：结构体
来源：http://oqk.hnqzz.top

struct P { var x: Int }
来源：http://djk.hysaishi.cn

[T26] Swift：类与重写
来源：http://ieq.gotoacloud.top

class A: Base { override func f() {} }
来源：http://ngs.ehwqpu.com

[T27] Swift：错误处理
来源：http://pfr.iojbl.cn

do { try f() } catch { print(error) }
来源：http://yyc.ppjwa.cn

[T28] Swift：枚举
来源：http://wno.sysykeji.top

enum Color { case red, green }
来源：http://rsl.bjfxy.top

[T29] Swift：guard 提前返回
来源：http://qgd.yongpay.top

guard let x = opt else { return }
来源：http://aqv.sufxvd.cn

[T30] Swift：协议
来源：http://hzd.c1oappe.top

protocol Shape { func area() -> Double }
来源：http://pjz.yuxming.cn

[T31] Lua：Hello World
来源：http://ami.gaohongyu789.top

print("Hello")
来源：http://wtw.guannengcc.top

[T32] Lua：局部变量
来源：http://osq.hfpthk.cn

local a = 1
来源：http://iza.fzhhl.top

[T33] Lua：表（数组）
来源：http://aiw.zdbjq.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://czn.ywan-chungtsiang.top

[T34] Lua：遍历表
来源：http://xoa.jlsjyb.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://moy.dianchejie.cn

[T35] Lua：字典表
来源：http://pwq.jinyuanbaomall.cn

local d = { a = 1 };  d.b = 2
来源：http://dta.ydzc1.top

[T36] Lua：函数
来源：http://knw.nanxuanxn.top

function add(a, b) return a + b end
来源：http://ncv.nwbrower.top

[T37] Lua：字符串拼接
来源：http://yds.c1oappe.top

"a" .. "b"
来源：http://erz.fengsongda.top

[T38] Lua：条件
来源：http://gbd.fktsv.cn

if x > 0 then print("正") end
来源：http://yru.yj20258.top

[T39] Lua：模式匹配
来源：http://yxp.gaohongyu789.top

string.find(s, "%d+")
来源：http://iwk.birdmap.top

[T40] Lua：元表
来源：http://dlb.xylfe.cn

setmetatable({}, { __index = base })
来源：http://mgj.cashguo.top

[T41] Perl：Hello World
来源：http://rmf.uphjek.com

print "Hello\n";
来源：http://snl.zhaomingkeji.xyz

[T42] Perl：变量类型
来源：http://lwf.chenlongwang.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://epk.guowangkeji.top

[T43] Perl：字符串插值
来源：http://xxq.zhengqikj.top

"值: $a"
来源：http://muk.sysykeji.top

[T44] Perl：条件
来源：http://rgj.smart0.xyz

if ($a > 0) { print "正"; }
来源：http://oyc.pycfn.com

[T45] Perl：数组遍历
来源：http://dab.ctjpmb.com

for my $x (@arr) { print $x; }
来源：http://iec.zhixingplan.top

[T46] Perl：哈希操作
来源：http://zpg.yongpay.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://suu.sxryk.cn

[T47] Perl：正则捕获
来源：http://upu.gaohongyu789.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ykr.tarul.cn

[T48] Perl：正则替换
来源：http://bsp.vqdsnc.cn

$s =~ s/old/new/g;
来源：http://wac.mhx1999.top

[T49] Perl：函数
来源：http://hov.snrcjt.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://arl.hongshengwenyu.top

[T50] Perl：逐行读文件
来源：http://zee.sysykeji.top

open my $fh, "<", "a.txt" or die $!;
来源：http://rcy.9152youxi.cn

while (my $line = <$fh>) { print $line; }
来源：http://eug.sjlbkw.cn

[T51] Scala：Hello World
来源：http://kdn.zhiwuduotai.top

println("Hello")
来源：http://ixb.ivvv.top

[T52] Scala：变量
来源：http://nhb.iojbl.cn

val a = 1;  var b = 2
来源：http://oxi.zhiwuduotai.top

[T53] Scala：字符串插值
来源：http://wwy.fengsongda.top

s"值: $b"
来源：http://yhv.gogol.net.cn

[T54] Scala：集合映射
来源：http://axu.zhiwuduotai.top

List(1, 2, 3).map(_ * 2)
来源：http://vyf.tianlin.xyz

[T55] Scala：集合过滤
来源：http://yaq.fktsv.cn

List(1, 2, 3).filter(_ > 1)
来源：http://mqp.tian-w.cn

[T56] Scala：样例类
来源：http://tff.dianchejie.cn

case class User(name: String, age: Int)
来源：http://qbr.hesvh.cn

[T57] Scala：模式匹配
来源：http://csq.sufxvd.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://eso.meibo888.top

[T58] Scala：函数定义
来源：http://kzz.xinyue.icu

def add(a: Int, b: Int): Int = a + b
来源：http://sud.52xcode.cn

[T59] Scala：循环
来源：http://rdl.xylfe.cn

for (i <- 1 to 10) println(i)
来源：http://zpy.ybcxt.top

[T60] Scala：折叠
来源：http://naf.fengsongda.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tsw.cucudq.cn

================================================================================
来源：http://iyz.nanxuanxn.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bbc.fehbvm.com

================================================================================
来源：http://bus.fktsv.cn

[U01] Py：创建虚拟环境
来源：http://enx.ivvv.top

python -m venv .venv && source .venv/bin/activate
来源：http://btz.yfazqb.com

[U02] Py：导出 / 安装依赖
来源：http://jmk.c1oappe.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yvp.daria6918.cn

[U03] Py：加载 .env 配置
来源：http://mqs.kuanghao11.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://okr.zycfv.cn

[U04] Py：变量调试打印
来源：http://pbw.fanxiaobao.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qph.dianchejie.cn

[U05] Py：列表去重且保序
来源：http://rxy.yfazqb.com

list(dict.fromkeys(arr))
来源：http://zpz.snrcjt.cn

[U06] Py：合并两个字典
来源：http://sci.chenjidiqi.icu

{**a, **b}
来源：http://dru.sjlbkw.cn

[U07] Py：反转字典键值
来源：http://pvh.yuxming.cn

{v: k for k, v in d.items()}
来源：http://bru.yangfankeji.com

[U08] Py：展平二维列表
来源：http://hwi.cheryme.top

[y for x in nested for y in x]
来源：http://vom.xylfe.cn

[U09] Py：字典取最大值的键
来源：http://fxh.hysaishi.cn

max(d, key=d.get)
来源：http://lsk.aizwys.cn

[U10] Py：按值排序字典
来源：http://qyj.vqdsnc.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jcp.wangshuangyany.cn

[U11] Py：生成器表达式
来源：http://caj.tarul.cn

(x * 2 for x in arr)
来源：http://ztu.gogol.net.cn

[U12] Py：取出现最多的 3 个元素
来源：http://gpz.wangdashe.top

Counter(arr).most_common(3)
来源：http://epl.pycfn.com

[U13] Py：固定长度队列
来源：http://blr.xingfuxueyuan.xyz

deque(maxlen=10)
来源：http://dif.shanyushiyangkeji.top

[U14] Py：分组收集到列表
来源：http://bxy.yuanzhike.top

defaultdict(list)
来源：http://bgw.jinqigufen.top

[U15] Py：高精度计时
来源：http://ypw.0kj1m.cn

t = time.perf_counter()
来源：http://mbd.guowangkeji.top

[U16] Py：命令行参数解析
来源：http://qvo.aibaodan.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lxi.jinyuanbaomall.cn

[U17] Py：初始化日志
来源：http://zkp.dashuyun.cn

logging.basicConfig(level=logging.INFO)
来源：http://sne.tarul.cn

[U18] Py：预编译正则
来源：http://sdk.redwolf501.top

pat = re.compile(r"\d+")
来源：http://jjm.svipenyu.cn

[U19] Py：正则替换带回调
来源：http://pob.feifeiyinyue.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lvg.sysykeji.top

[U20] Py：缓存函数结果
来源：http://bcj.redwolf501.top

@functools.lru_cache(maxsize=None)
来源：http://ovc.fanxiaobao.xyz

[U21] Py：自定义上下文管理器
来源：http://fqd.sweek.top

@contextlib.contextmanager
来源：http://jsl.yfazqb.com

[U22] Py：矩阵转置
来源：http://eup.zycfv.cn

list(zip(*m))
来源：http://eoc.gaohongyu789.top

[U23] Py：分块读取大文件
来源：http://gyy.nanxinkj.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tec.cdnleiting.top

[U24] Py：路径操作
来源：http://hzx.sxryk.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ttz.cashguo.top

[U25] Py：CSV 按字典读
来源：http://xes.zhongyouzk.top

csv.DictReader(f)
来源：http://vsv.316326.xyz

[U26] Py：并发下载
来源：http://lrw.svipenyu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fyc.aizwys.cn

[U27] Py：异步 HTTP
来源：http://knf.guannengcc.top

aiohttp.ClientSession() 配合 async with
来源：http://tsa.birdmap.top

[U28] Py：类型别名
来源：http://ylx.bjfxy.top

UserId = int
来源：http://igr.c1oappe.top

[U29] Py：属性校验
来源：http://dda.ivvv.top

@property 与 @x.setter 配合
来源：http://jpq.yangfankeji.com

[U30] Py：数据类
来源：http://len.dianchejie.cn

@dataclass(slots=True)
来源：http://pqk.gaohongyu789.top

[U31] Py：单测
来源：http://xtp.jqgfzy.top

python -m pytest -q
来源：http://jry.jqgufenzy.top

[U32] Py：代码格式化
来源：http://his.hongshengwenyu.top

ruff format . && ruff check --fix .
来源：http://vlc.svipenyu.cn

[U33] Py：打包发布
来源：http://hus.0kj1m.cn

python -m build  （依赖 pyproject.toml）
来源：http://gah.yuxming.cn

[U34] Py：判断编码
来源：http://coa.hnxiangtu.top

chardet.detect(raw)
来源：http://yag.gotoacloud.top

[U35] Py：发送邮件
来源：http://omv.feifeiyinyue.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nly.tianlin.xyz

[U36] Py：定时任务
来源：http://kov.316326.xyz

schedule.every(10).minutes.do(job)
来源：http://gwa.fzhhl.top

[U37] Py：读写 Excel
来源：http://gdz.jianghu66.top

pandas.read_excel / DataFrame.to_excel
来源：http://dlj.ehwqpu.com

[U38] Py：获取脚本所在目录
来源：http://tgd.jinyuanbaomall.cn

Path(__file__).resolve().parent
来源：http://exx.uphjek.com

[U39] Py：判断是否在交互环境
来源：http://btl.fehbvm.com

sys.stdout.isatty()
来源：http://sgv.guannengcc.top

[U40] Py：打印到标准错误
来源：http://qmv.ywan-chungtsiang.top

print("err", file=sys.stderr)
来源：http://fvk.sysykeji.top

[U41] PHP：初始化 Composer 项目
来源：http://thg.yj20258.top

composer init;  composer require guzzlehttp/guzzle
来源：http://xtl.jinghuilouyu.cn

[U42] PHP：PSR-4 自动加载
来源：http://lxp.hysaishi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fnr.hfpthk.cn

[U43] PHP：声明命名空间
来源：http://yij.snrcjt.cn

namespace App\Http;
来源：http://ohn.jinqigfzy.top

[U44] PHP：开启严格类型
来源：http://pvu.nanxinkj.top

declare(strict_types=1);
来源：http://yzx.zhixingplan.top

[U45] PHP：类型声明与返回类型
来源：http://gbg.ybcxt.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://mtp.zhoulong.xyz

[U46] PHP：可空类型
来源：http://roc.hywenlv.cn

?string $name = null
来源：http://iga.yongpay.top

[U47] PHP：联合类型
来源：http://yyt.cqqwz.cn

int|string $id
来源：http://ikl.guowangkeji.top

[U48] PHP：纯枚举
来源：http://lfd.cdnleiting.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://uwz.ppjwa.cn

[U49] PHP：只读属性
来源：http://qpe.zhiwuduotai.top

public readonly string $name
来源：http://nym.yueranfly.top

[U50] PHP：构造器属性提升
来源：http://joi.shzxlz.cn

public function __construct(private int $id) {}
来源：http://jwd.gotoacloud.top

[U51] PHP：数组解构
来源：http://mnd.yuanzhike.top

[$a, $b] = $arr;
来源：http://jsz.chenjidiqi.icu

[U52] PHP：箭头函数
来源：http://esf.feifeiyinyue.top

$double = fn($x) => $x * 2;
来源：http://wfd.haohaochexian.top

[U53] PHP：空合并运算符
来源：http://mtx.zdbjq.cn

$v = $a ?? $b ?? "default";
来源：http://syz.ybcxt.top

[U54] PHP：空安全调用
来源：http://cpu.zycfv.cn

$obj?->method()
来源：http://kry.zhengqikj.top

[U55] PHP：match 表达式
来源：http://pre.hysaishi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wuv.xingfuxueyuan.xyz

[U56] PHP：命名参数
来源：http://gvm.yvedp.cn

f(a: 1, b: 2)
来源：http://zdi.epnwcf.com

[U57] PHP：字符串插值
来源：http://ebf.sxryk.cn

"值: {$a}"
来源：http://vez.sysykeji.top

[U58] PHP：数组三件套
来源：http://ovv.chenjidiqi.icu

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://olx.ybcxt.top

[U59] PHP：自定义排序
来源：http://xbd.wangdashe.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fmb.quarkkingdee.top

[U60] PHP：JSON 编解码
来源：http://mny.zhongyouzk.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jmb.cdnleiting.top

[U61] PHP：正则
来源：http://ixd.wangshuangyany.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jyk.daxiang520.top

[U62] PHP：日期对象
来源：http://fei.yonumen.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gnn.jinyuanbaomall.cn

[U63] PHP：文件读写
来源：http://bol.ppjwa.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dax.havefunace.top

[U64] PHP：目录遍历
来源：http://xie.shanyushiyangtech.top

glob("dir/*.php");  scandir("dir");
来源：http://qxx.wangshuangyany.cn

[U65] PHP：会话
来源：http://qzn.tian-w.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://okn.yangfankeji.com

[U66] PHP：设置 Cookie
来源：http://msx.fktsv.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dab.sxryk.cn

[U67] PHP：处理文件上传
来源：http://rng.c1oappe.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://sxx.cdnleiting.top

[U68] PHP：PDO 连接
来源：http://kfc.jiagoushi.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://eos.zhiwuduotai.top

[U69] PHP：PDO 预处理
来源：http://jdu.cdnleiting.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yyp.cashguo.top

[U70] PHP：PDO 事务
来源：http://kcj.daxiang520.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jod.cucudq.cn

[U71] PHP：抛出异常
来源：http://jpm.aibaodan.cn

throw new RuntimeException("失败", 500);
来源：http://bkq.birdmap.top

[U72] PHP：写错误日志
来源：http://tkf.tian-w.cn

error_log("失败: " . $e->getMessage());
来源：http://dzb.ppjwa.cn

[U73] PHP：读取 ini 配置
来源：http://svf.shanyushiyangkeji.top

parse_ini_file("config.ini", true)
来源：http://itf.gaohongyu789.top

[U74] PHP：读取环境变量
来源：http://vjq.ctjpmb.com

getenv("APP_ENV") ?: "production"
来源：http://keq.yueranfly.top

[U75] PHP：依赖注入
来源：http://zju.zdbjq.cn

composer require psr/container
来源：http://ccf.xuetiantiany.cn

[U76] PHP：简单路由
来源：http://bjz.yuanzhike.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rjm.zhaomingkeji.xyz

[U77] PHP：模板渲染
来源：http://kea.9152youxi.cn

composer require twig/twig
来源：http://awt.9152youxi.cn

[U78] PHP：单元测试
来源：http://bwy.zhixingplan.top

composer require --dev phpunit/phpunit
来源：http://erz.pengpengdd.cyou

[U79] PHP：静态分析
来源：http://ilz.hfpthk.cn

composer require --dev phpstan/phpstan
来源：http://ayx.yj20258888.top

[U80] PHP：代码规范修复
来源：http://snh.nanxuanxn.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://yaz.zhengqikj.top

[U81] JS：初始化项目
来源：http://jgp.shanyushiyangkeji.top

npm init -y;  npm i express
来源：http://ydd.xingfuxueyuan.xyz

[U82] JS：package.json 脚本
来源：http://dcf.sxryk.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://sbd.zhoulong.xyz

[U83] JS：ES Module 导入导出
来源：http://tjt.ppjwa.cn

export const a = 1;  import { a } from "./m.js";
来源：http://yya.xingfuxueyuan.xyz

[U84] JS：CommonJS 写法
来源：http://gzp.hnxiangtu.top

module.exports = { a };  const { a } = require("./m");
来源：http://swm.uphjek.com

[U85] JS：可选链
来源：http://eaq.shanyushiyangtech.top

a?.b?.c
来源：http://dos.yuanzhike.top

[U86] JS：空值合并
来源：http://lzv.snrcjt.cn

a ?? b
来源：http://fss.zhiwuduotai.top

[U87] JS：解构默认值
来源：http://sjm.andypj.xyz

const { a = 1, b = 2 } = obj;
来源：http://tee.jianghu66.top

[U88] JS：对象展开合并
来源：http://rdm.yfazqb.com

{ ...a, ...b }
来源：http://tso.fehbvm.com

[U89] JS：数组去重
来源：http://uth.wangshuangyany.cn

[...new Set(arr)]
来源：http://zxs.9152youxi.cn

[U90] JS：数字数组排序
来源：http://bco.ctjpmb.com

[...arr].sort((a, b) => a - b)
来源：http://zfb.nwbrower.top

[U91] JS：对象键值遍历
来源：http://gja.hcnkem.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nto.gotoacloud.top

[U92] JS：深拷贝
来源：http://okd.yuanzhike.top

structuredClone(obj)
来源：http://tds.yj20258.top

[U93] JS：模板字符串
来源：http://jmx.cdnleiting.top

`共 ${n} 条`
来源：http://oqs.andypj.xyz

[U94] JS：箭头函数
来源：http://lbe.zdbjq.cn

const double = x => x * 2;
来源：http://jsn.uphjek.com

[U95] JS：Promise 包装
来源：http://yda.yfazqb.com

new Promise((resolve, reject) => {})
来源：http://ttd.vqdsnc.cn

[U96] JS：async/await 与异常
来源：http://zhb.xingfuxueyuan.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://yyy.jianghu66.top


<!-- 参考信息 -->