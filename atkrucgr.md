代发 wailian999

[T09] Kotlin：扩展函数
来源：http://buq.cucudq.cn

fun String.exclaim() = this + "!"
来源：http://tfa.ppjwa.cn

[T10] Kotlin：默认参数
来源：http://uld.ivvv.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ype.zhoulong.xyz

[T11] Kotlin：协程
来源：http://kdh.xuanzx.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://agl.sxryk.cn

[T12] Kotlin：解构声明
来源：http://bwm.yonumen.top

val (a, b) = Pair(1, 2)
来源：http://bod.cqqwz.cn

[T13] Kotlin：只读 Map
来源：http://ydy.shuidangran.top

val m = mapOf("a" to 1)
来源：http://xpz.shanyushiyangkeji.top

[T14] Kotlin：循环
来源：http://zia.tian-w.cn

for (i in 1..10) println(i)
来源：http://ubr.zhaomingkeji.xyz

[T15] Kotlin：接口
来源：http://smv.chenzaomai.com

interface Shape { fun area(): Double }
来源：http://jvk.yonumen.top

[T16] Swift：Hello World
来源：http://fno.chenlongwang.top

print("Hello")
来源：http://afm.yongpay.top

[T17] Swift：变量与常量
来源：http://csx.cheryme.top

var a = 1;  let b = 2
来源：http://zww.gogol.net.cn

[T18] Swift：字符串插值
来源：http://xhu.zhijiandao.cn

"值: \(b)"
来源：http://kwb.hysaishi.cn

[T19] Swift：可选绑定
来源：http://mys.gogol.net.cn

if let n = opt { print(n) }
来源：http://vpm.pycfn.com

[T20] Swift：数组操作
来源：http://lha.shangyingyoupin.top

var a = [1, 2, 3];  a.append(4)
来源：http://yho.pycfn.com

[T21] Swift：遍历
来源：http://czc.xziqi.cn

for x in a { print(x) }
来源：http://bsx.wangdashe.top

[T22] Swift：字典
来源：http://fyv.hywenlv.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ufk.cashguo.top

[T23] Swift：函数
来源：http://ttg.daria6918.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xwg.yuanzhike.top

[T24] Swift：闭包
来源：http://pmz.yj202588.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://znc.cqqwz.cn

[T25] Swift：结构体
来源：http://git.zdbjq.cn

struct P { var x: Int }
来源：http://mfs.svipenyu.cn

[T26] Swift：类与重写
来源：http://eqh.haohaochexian.top

class A: Base { override func f() {} }
来源：http://ufd.jianghu66.top

[T27] Swift：错误处理
来源：http://ulq.ivvv.top

do { try f() } catch { print(error) }
来源：http://aco.hcnkem.com

[T28] Swift：枚举
来源：http://bma.tianlin.xyz

enum Color { case red, green }
来源：http://qne.svipenyu.cn

[T29] Swift：guard 提前返回
来源：http://rww.cashguo.top

guard let x = opt else { return }
来源：http://emo.cheryme.top

[T30] Swift：协议
来源：http://cvo.tianlin.xyz

protocol Shape { func area() -> Double }
来源：http://wut.kuanghao11.cn

[T31] Lua：Hello World
来源：http://uiv.vehdjk.com

print("Hello")
来源：http://emu.birdmap.top

[T32] Lua：局部变量
来源：http://koo.zhaomingkeji.xyz

local a = 1
来源：http://dxw.yuanzhike.top

[T33] Lua：表（数组）
来源：http://rik.fengsongda.top

local t = {1, 2, 3};  t[4] = 4
来源：http://apd.ehwqpu.com

[T34] Lua：遍历表
来源：http://arv.dianchejie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ehx.zdqjudy.top

[T35] Lua：字典表
来源：http://qnu.yuxming.cn

local d = { a = 1 };  d.b = 2
来源：http://qrf.hesvh.cn

[T36] Lua：函数
来源：http://ilc.wangdashe.top

function add(a, b) return a + b end
来源：http://nat.ehwqpu.com

[T37] Lua：字符串拼接
来源：http://mcb.iojbl.cn

"a" .. "b"
来源：http://qrz.gogol.net.cn

[T38] Lua：条件
来源：http://iil.wangdashe.top

if x > 0 then print("正") end
来源：http://nag.ppjwa.cn

[T39] Lua：模式匹配
来源：http://pqf.c1oappe.top

string.find(s, "%d+")
来源：http://dyp.andypj.xyz

[T40] Lua：元表
来源：http://wbg.feifeiyinyue.top

setmetatable({}, { __index = base })
来源：http://qer.chenzaomai.com

[T41] Perl：Hello World
来源：http://tuc.tianlin.xyz

print "Hello\n";
来源：http://fnk.ydzc1.top

[T42] Perl：变量类型
来源：http://eje.shangyingyoupin.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ngu.fengsongda.top

[T43] Perl：字符串插值
来源：http://agx.ivvv.top

"值: $a"
来源：http://khl.gaohongyu789.top

[T44] Perl：条件
来源：http://ctc.birdmap.top

if ($a > 0) { print "正"; }
来源：http://wcq.zhijiandao.cn

[T45] Perl：数组遍历
来源：http://yti.nanxinkj.top

for my $x (@arr) { print $x; }
来源：http://tmv.bbcook.cn

[T46] Perl：哈希操作
来源：http://cbz.daxiang520.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rdu.316326.xyz

[T47] Perl：正则捕获
来源：http://xkf.hnqzz.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://xuy.xuetiantiany.cn

[T48] Perl：正则替换
来源：http://ylc.ivvv.top

$s =~ s/old/new/g;
来源：http://pvw.daria6918.cn

[T49] Perl：函数
来源：http://fpn.jinghuilouyu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://eyy.aibaodan.cn

[T50] Perl：逐行读文件
来源：http://whh.guannengcc.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ioi.zdbjq.cn

while (my $line = <$fh>) { print $line; }
来源：http://krz.c1oappe.top

[T51] Scala：Hello World
来源：http://gep.xuetiantiany.cn

println("Hello")
来源：http://vma.quarkkingdee.top

[T52] Scala：变量
来源：http://zey.ehwqpu.com

val a = 1;  var b = 2
来源：http://gdi.hongshengwenyu.top

[T53] Scala：字符串插值
来源：http://eiz.epnwcf.com

s"值: $b"
来源：http://rkx.hesvh.cn

[T54] Scala：集合映射
来源：http://wnq.yj202588.top

List(1, 2, 3).map(_ * 2)
来源：http://ype.ivvv.top

[T55] Scala：集合过滤
来源：http://mqe.daria6918.cn

List(1, 2, 3).filter(_ > 1)
来源：http://kux.fzhhl.top

[T56] Scala：样例类
来源：http://roa.yanxiufei.cn

case class User(name: String, age: Int)
来源：http://sqm.tanke756.top

[T57] Scala：模式匹配
来源：http://gjn.shanyushiyangtech.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://okq.cqqwz.cn

[T58] Scala：函数定义
来源：http://yvp.shzxlz.cn

def add(a: Int, b: Int): Int = a + b
来源：http://kgm.kuanghao11.cn

[T59] Scala：循环
来源：http://hzb.nanxinkj.top

for (i <- 1 to 10) println(i)
来源：http://ktj.ehwqpu.com

[T60] Scala：折叠
来源：http://jfm.jiagoushi.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://png.xinyue.icu

================================================================================
来源：http://aua.jinqigfzy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rkt.kuanghao11.cn

================================================================================
来源：http://uym.yangfankeji.com

[U01] Py：创建虚拟环境
来源：http://gwd.xylfe.cn

python -m venv .venv && source .venv/bin/activate
来源：http://xia.yj20258.top

[U02] Py：导出 / 安装依赖
来源：http://erc.fktsv.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://udi.fktsv.cn

[U03] Py：加载 .env 配置
来源：http://pua.hysaishi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://txm.yangfankeji.com

[U04] Py：变量调试打印
来源：http://wjo.jinqigfzy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fyp.zhijiandao.cn

[U05] Py：列表去重且保序
来源：http://rel.cucudq.cn

list(dict.fromkeys(arr))
来源：http://rfs.xuanzx.com

[U06] Py：合并两个字典
来源：http://xrz.jinyuanbaomall.cn

{**a, **b}
来源：http://kyy.daxiang520.top

[U07] Py：反转字典键值
来源：http://nnc.zhengqikj.top

{v: k for k, v in d.items()}
来源：http://tbu.hcnkem.com

[U08] Py：展平二维列表
来源：http://ufg.yuanzhike.top

[y for x in nested for y in x]
来源：http://bop.shanyushiyangkeji.top

[U09] Py：字典取最大值的键
来源：http://usg.zhixingplan.top

max(d, key=d.get)
来源：http://hqy.uphjek.com

[U10] Py：按值排序字典
来源：http://uyu.jinghuilouyu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vfl.xziqi.cn

[U11] Py：生成器表达式
来源：http://tso.hnxiangtu.top

(x * 2 for x in arr)
来源：http://clz.zhijiandao.cn

[U12] Py：取出现最多的 3 个元素
来源：http://phu.zhongyouzk.top

Counter(arr).most_common(3)
来源：http://tad.mhx1999.top

[U13] Py：固定长度队列
来源：http://est.tian-w.cn

deque(maxlen=10)
来源：http://hcr.ydjk.org.cn

[U14] Py：分组收集到列表
来源：http://del.hongshengwenyu.top

defaultdict(list)
来源：http://wiv.snrcjt.cn

[U15] Py：高精度计时
来源：http://vei.cdnleiting.top

t = time.perf_counter()
来源：http://ajc.daxiang520.top

[U16] Py：命令行参数解析
来源：http://zjq.zhoulong.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://oxe.sjlbkw.cn

[U17] Py：初始化日志
来源：http://amw.xingfuxueyuan.xyz

logging.basicConfig(level=logging.INFO)
来源：http://sbp.gogol.net.cn

[U18] Py：预编译正则
来源：http://abc.meibo888.top

pat = re.compile(r"\d+")
来源：http://rop.yvedp.cn

[U19] Py：正则替换带回调
来源：http://ein.xylfe.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xzx.hfpthk.cn

[U20] Py：缓存函数结果
来源：http://hvp.dashuyun.cn

@functools.lru_cache(maxsize=None)
来源：http://zkl.meibo888.top

[U21] Py：自定义上下文管理器
来源：http://ids.zdbjq.cn

@contextlib.contextmanager
来源：http://emo.sysykeji.top

[U22] Py：矩阵转置
来源：http://qqe.jinyuanbaomall.cn

list(zip(*m))
来源：http://fll.hammf.cn

[U23] Py：分块读取大文件
来源：http://wyp.yuxming.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zcf.vehdjk.com

[U24] Py：路径操作
来源：http://erq.0kj1m.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xba.yvedp.cn

[U25] Py：CSV 按字典读
来源：http://mqh.yj20258888.top

csv.DictReader(f)
来源：http://gxs.jinghuilouyu.cn

[U26] Py：并发下载
来源：http://gix.yuanzhike.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vkp.pycfn.com

[U27] Py：异步 HTTP
来源：http://yyv.nwbrower.top

aiohttp.ClientSession() 配合 async with
来源：http://nda.jlsjyb.cn

[U28] Py：类型别名
来源：http://pjt.andypj.xyz

UserId = int
来源：http://blf.shanyushiyangkeji.top

[U29] Py：属性校验
来源：http://ofg.chenzaomai.com

@property 与 @x.setter 配合
来源：http://pbd.nanxinkj.top

[U30] Py：数据类
来源：http://kut.aibaodan.cn

@dataclass(slots=True)
来源：http://awa.andypj.xyz

[U31] Py：单测
来源：http://vbf.hongshengwenyu.top

python -m pytest -q
来源：http://fti.dianchejie.cn

[U32] Py：代码格式化
来源：http://zkc.haohaochexian.top

ruff format . && ruff check --fix .
来源：http://wru.fzhhl.top

[U33] Py：打包发布
来源：http://bfa.cdnleiting.top

python -m build  （依赖 pyproject.toml）
来源：http://swh.ybcxt.top

[U34] Py：判断编码
来源：http://oud.daria6918.cn

chardet.detect(raw)
来源：http://xjx.jinqigfzy.top

[U35] Py：发送邮件
来源：http://lya.sweek.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://izz.gzhubu.top

[U36] Py：定时任务
来源：http://skc.nwbrower.top

schedule.every(10).minutes.do(job)
来源：http://ssp.xingfuxueyuan.xyz

[U37] Py：读写 Excel
来源：http://xkq.yuanzhike.top

pandas.read_excel / DataFrame.to_excel
来源：http://yok.pycfn.com

[U38] Py：获取脚本所在目录
来源：http://nom.nwbrower.top

Path(__file__).resolve().parent
来源：http://wts.yuxming.cn

[U39] Py：判断是否在交互环境
来源：http://jct.epnwcf.com

sys.stdout.isatty()
来源：http://bbx.ivvv.top

[U40] Py：打印到标准错误
来源：http://rzd.aibaodan.cn

print("err", file=sys.stderr)
来源：http://ssg.0kj1m.cn

[U41] PHP：初始化 Composer 项目
来源：http://oty.yuxming.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://xwq.0kj1m.cn

[U42] PHP：PSR-4 自动加载
来源：http://mcy.jinyuanbaomall.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://uci.dashuyun.cn

[U43] PHP：声明命名空间
来源：http://twl.yangfankeji.com

namespace App\Http;
来源：http://gyq.hesvh.cn

[U44] PHP：开启严格类型
来源：http://wzc.yj20258888.top

declare(strict_types=1);
来源：http://vfa.yanxiufei.cn

[U45] PHP：类型声明与返回类型
来源：http://uls.0kj1m.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://bmr.xuetiantiany.cn

[U46] PHP：可空类型
来源：http://pde.fzhhl.top

?string $name = null
来源：http://erj.svipenyu.cn

[U47] PHP：联合类型
来源：http://ohu.ybcxt.top

int|string $id
来源：http://fqx.xinyue.icu

[U48] PHP：纯枚举
来源：http://ayd.jinyuanbaomall.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nht.ppjwa.cn

[U49] PHP：只读属性
来源：http://lks.cheryme.top

public readonly string $name
来源：http://ufz.uphjek.com

[U50] PHP：构造器属性提升
来源：http://qnl.quarkkingdee.top

public function __construct(private int $id) {}
来源：http://zdg.smart0.xyz

[U51] PHP：数组解构
来源：http://hol.iojbl.cn

[$a, $b] = $arr;
来源：http://ifa.fengsongda.top

[U52] PHP：箭头函数
来源：http://axr.hfpthk.cn

$double = fn($x) => $x * 2;
来源：http://pri.xuetiantiany.cn

[U53] PHP：空合并运算符
来源：http://qgx.quarkkingdee.top

$v = $a ?? $b ?? "default";
来源：http://eia.wangdashe.top

[U54] PHP：空安全调用
来源：http://szb.52xcode.cn

$obj?->method()
来源：http://pim.cheryme.top

[U55] PHP：match 表达式
来源：http://ryb.pengpengdd.cyou

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rwf.gzhubu.top

[U56] PHP：命名参数
来源：http://gng.tanke756.top

f(a: 1, b: 2)
来源：http://rsz.kuanghao11.cn

[U57] PHP：字符串插值
来源：http://pmg.cheryme.top

"值: {$a}"
来源：http://egi.xinyue.icu

[U58] PHP：数组三件套
来源：http://rnr.bbcook.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hpz.dianchejie.cn

[U59] PHP：自定义排序
来源：http://bav.meibo888.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qfc.jinghuilouyu.cn

[U60] PHP：JSON 编解码
来源：http://lwc.nanxuanxn.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xtj.yvedp.cn

[U61] PHP：正则
来源：http://ifu.jianghu66.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rgp.yuxming.cn

[U62] PHP：日期对象
来源：http://ngy.xylfe.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ycw.vehdjk.com

[U63] PHP：文件读写
来源：http://dot.ehwqpu.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yqz.yonumen.top

[U64] PHP：目录遍历
来源：http://zzc.jlsjyb.cn

glob("dir/*.php");  scandir("dir");
来源：http://hrp.ivvv.top

[U65] PHP：会话
来源：http://qzz.ybcxt.top

session_start();  $_SESSION["uid"] = 1;
来源：http://bko.cashguo.top

[U66] PHP：设置 Cookie
来源：http://ycu.aizwys.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://osh.yonumen.top

[U67] PHP：处理文件上传
来源：http://mjp.zhoulong.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gll.smart0.xyz

[U68] PHP：PDO 连接
来源：http://iah.hammf.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jrq.fktsv.cn

[U69] PHP：PDO 预处理
来源：http://zfd.cheryme.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bzp.guannengcc.top

[U70] PHP：PDO 事务
来源：http://sma.aizwys.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wuk.bjfxy.top

[U71] PHP：抛出异常
来源：http://gup.shanyushiyangkeji.top

throw new RuntimeException("失败", 500);
来源：http://pwe.aizwys.cn

[U72] PHP：写错误日志
来源：http://jsk.yj20258888.top

error_log("失败: " . $e->getMessage());
来源：http://tng.jinqigufen.top

[U73] PHP：读取 ini 配置
来源：http://fnf.gzhubu.top

parse_ini_file("config.ini", true)
来源：http://ruo.cashguo.top

[U74] PHP：读取环境变量
来源：http://unn.cucudq.cn

getenv("APP_ENV") ?: "production"
来源：http://ubd.hfpthk.cn

[U75] PHP：依赖注入
来源：http://jgk.shangyingyoupin.top

composer require psr/container
来源：http://ves.yj20258888.top

[U76] PHP：简单路由
来源：http://jyz.fengsongda.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ese.yangfankeji.com

[U77] PHP：模板渲染
来源：http://mxh.ydjk.org.cn

composer require twig/twig
来源：http://zar.dashuyun.cn

[U78] PHP：单元测试
来源：http://kec.hammf.cn

composer require --dev phpunit/phpunit
来源：http://hie.zhijiandao.cn

[U79] PHP：静态分析
来源：http://bgz.sysykeji.top

composer require --dev phpstan/phpstan
来源：http://kim.andypj.xyz

[U80] PHP：代码规范修复
来源：http://vsr.hnxiangtu.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://one.hfpthk.cn

[U81] JS：初始化项目
来源：http://ihy.sweek.top

npm init -y;  npm i express
来源：http://qpw.aizwys.cn

[U82] JS：package.json 脚本
来源：http://ubl.jqgufenzy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gbi.zycfv.cn

[U83] JS：ES Module 导入导出
来源：http://zzo.xylfe.cn

export const a = 1;  import { a } from "./m.js";
来源：http://qbf.gzhubu.top

[U84] JS：CommonJS 写法
来源：http://amj.fanxiaobao.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://txa.iojbl.cn

[U85] JS：可选链
来源：http://ybz.daxiang520.top

a?.b?.c
来源：http://rph.ctjpmb.com

[U86] JS：空值合并
来源：http://lfj.hammf.cn

a ?? b
来源：http://vys.jyoumei.cn

[U87] JS：解构默认值
来源：http://grf.daria6918.cn

const { a = 1, b = 2 } = obj;
来源：http://vus.zhoulong.xyz

[U88] JS：对象展开合并
来源：http://dlx.shuidangran.top

{ ...a, ...b }
来源：http://him.yuxming.cn

[U89] JS：数组去重
来源：http://jfr.shzxlz.cn

[...new Set(arr)]
来源：http://wia.hysaishi.cn

[U90] JS：数字数组排序
来源：http://gvj.zdbjq.cn

[...arr].sort((a, b) => a - b)
来源：http://rqf.c1oappe.top

[U91] JS：对象键值遍历
来源：http://nbx.tanke756.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hvh.zycfv.cn

[U92] JS：深拷贝
来源：http://vmg.hysaishi.cn

structuredClone(obj)
来源：http://hnb.xziqi.cn

[U93] JS：模板字符串
来源：http://vjj.xziqi.cn

`共 ${n} 条`
来源：http://gvt.gaohongyu789.top

[U94] JS：箭头函数
来源：http://rqx.hammf.cn

const double = x => x * 2;
来源：http://yhp.uphjek.com

[U95] JS：Promise 包装
来源：http://jvl.hcnkem.com

new Promise((resolve, reject) => {})
来源：http://qdt.hysaishi.cn

[U96] JS：async/await 与异常
来源：http://mfr.birdmap.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rhw.ehwqpu.com


<!-- 参考信息 -->