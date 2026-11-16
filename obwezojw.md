代发 wailian999

[T05] Kotlin：when 表达式
来源：http://jws.fengsongda.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qzd.jinqigufen.top

[T06] Kotlin：集合映射
来源：http://mgc.cdnleiting.top

listOf(1, 2, 3).map { it * 2 }
来源：http://oys.epnwcf.com

[T07] Kotlin：集合过滤
来源：http://xbn.yuanzhike.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://tms.yuxming.cn

[T08] Kotlin：数据类
来源：http://eec.sufxvd.cn

data class User(val name: String, val age: Int)
来源：http://kkx.xziqi.cn

[T09] Kotlin：扩展函数
来源：http://hlz.tian-w.cn

fun String.exclaim() = this + "!"
来源：http://cvc.fanxiaobao.xyz

[T10] Kotlin：默认参数
来源：http://dyy.wangdashe.top

fun greet(name: String = "World") = "Hi $name"
来源：http://zsm.gotoacloud.top

[T11] Kotlin：协程
来源：http://dev.yj20258888.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://laa.jinghuilouyu.cn

[T12] Kotlin：解构声明
来源：http://owj.zhongyouzk.top

val (a, b) = Pair(1, 2)
来源：http://ufh.tian-w.cn

[T13] Kotlin：只读 Map
来源：http://vpj.ehwqpu.com

val m = mapOf("a" to 1)
来源：http://uhm.316326.xyz

[T14] Kotlin：循环
来源：http://lvz.ywan-chungtsiang.top

for (i in 1..10) println(i)
来源：http://jkg.cashguo.top

[T15] Kotlin：接口
来源：http://zqv.haohaochexian.top

interface Shape { fun area(): Double }
来源：http://kbm.vehdjk.com

[T16] Swift：Hello World
来源：http://fea.shuidangran.top

print("Hello")
来源：http://xws.chenlongwang.top

[T17] Swift：变量与常量
来源：http://zpc.xuanzx.com

var a = 1;  let b = 2
来源：http://kwu.bbcook.cn

[T18] Swift：字符串插值
来源：http://smr.haohaochexian.top

"值: \(b)"
来源：http://byu.gogol.net.cn

[T19] Swift：可选绑定
来源：http://uuc.havefunace.top

if let n = opt { print(n) }
来源：http://zas.hongshengwenyu.top

[T20] Swift：数组操作
来源：http://qbb.gaohongyu789.top

var a = [1, 2, 3];  a.append(4)
来源：http://mml.zhiwuduotai.top

[T21] Swift：遍历
来源：http://hlm.zhiwuduotai.top

for x in a { print(x) }
来源：http://ill.jyoumei.cn

[T22] Swift：字典
来源：http://kll.zhiwuduotai.top

var d = ["a": 1];  d["b"] = 2
来源：http://fyc.jqgfzy.top

[T23] Swift：函数
来源：http://kua.fehbvm.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fup.yuxming.cn

[T24] Swift：闭包
来源：http://lqp.nanxinkj.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://yvt.xziqi.cn

[T25] Swift：结构体
来源：http://wwa.chenlongwang.top

struct P { var x: Int }
来源：http://npu.sufxvd.cn

[T26] Swift：类与重写
来源：http://qmw.hammf.cn

class A: Base { override func f() {} }
来源：http://pfh.hcnkem.com

[T27] Swift：错误处理
来源：http://ytk.yueranfly.top

do { try f() } catch { print(error) }
来源：http://fnr.zdbjq.cn

[T28] Swift：枚举
来源：http://hly.chenlongwang.top

enum Color { case red, green }
来源：http://owo.birdmap.top

[T29] Swift：guard 提前返回
来源：http://ctr.chenjidiqi.icu

guard let x = opt else { return }
来源：http://jkw.chenlongwang.top

[T30] Swift：协议
来源：http://oqu.shanyushiyangkeji.top

protocol Shape { func area() -> Double }
来源：http://unb.jlsjyb.cn

[T31] Lua：Hello World
来源：http://ydb.yfazqb.com

print("Hello")
来源：http://znj.nanxinkj.top

[T32] Lua：局部变量
来源：http://evl.meibo888.top

local a = 1
来源：http://kqx.yongpay.top

[T33] Lua：表（数组）
来源：http://oaj.jinghuilouyu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://qkq.mhx1999.top

[T34] Lua：遍历表
来源：http://tsa.52xcode.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://wnv.shanyushiyangkeji.top

[T35] Lua：字典表
来源：http://hee.yuxming.cn

local d = { a = 1 };  d.b = 2
来源：http://aaz.quarkkingdee.top

[T36] Lua：函数
来源：http://bgb.guannengcc.top

function add(a, b) return a + b end
来源：http://iit.jyoumei.cn

[T37] Lua：字符串拼接
来源：http://wyv.yangfankeji.com

"a" .. "b"
来源：http://ofl.yj20258888.top

[T38] Lua：条件
来源：http://rla.guowangkeji.top

if x > 0 then print("正") end
来源：http://kks.hnqzz.top

[T39] Lua：模式匹配
来源：http://ddv.cdnleiting.top

string.find(s, "%d+")
来源：http://jnk.yangfankeji.com

[T40] Lua：元表
来源：http://bvk.zhiwuduotai.top

setmetatable({}, { __index = base })
来源：http://tmz.gogol.net.cn

[T41] Perl：Hello World
来源：http://pap.sjlbkw.cn

print "Hello\n";
来源：http://bhj.sysykeji.top

[T42] Perl：变量类型
来源：http://map.jyoumei.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ele.uphjek.com

[T43] Perl：字符串插值
来源：http://cxj.gzhubu.top

"值: $a"
来源：http://feh.gzhubu.top

[T44] Perl：条件
来源：http://zhh.xylfe.cn

if ($a > 0) { print "正"; }
来源：http://iep.gotoacloud.top

[T45] Perl：数组遍历
来源：http://kxw.cheryme.top

for my $x (@arr) { print $x; }
来源：http://boc.hongshengwenyu.top

[T46] Perl：哈希操作
来源：http://ppa.zdbjq.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pfd.zdqjudy.top

[T47] Perl：正则捕获
来源：http://suw.jyoumei.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://exs.xinyue.icu

[T48] Perl：正则替换
来源：http://yav.hfpthk.cn

$s =~ s/old/new/g;
来源：http://hxl.yj202588.top

[T49] Perl：函数
来源：http://mhg.birdmap.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nui.hcnkem.com

[T50] Perl：逐行读文件
来源：http://mrd.dianchejie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://yjp.ehwqpu.com

while (my $line = <$fh>) { print $line; }
来源：http://hyu.mhx1999.top

[T51] Scala：Hello World
来源：http://gau.52xcode.cn

println("Hello")
来源：http://mhd.birdmap.top

[T52] Scala：变量
来源：http://fdw.wangdashe.top

val a = 1;  var b = 2
来源：http://rex.xuetiantiany.cn

[T53] Scala：字符串插值
来源：http://pjs.yvedp.cn

s"值: $b"
来源：http://qib.sysykeji.top

[T54] Scala：集合映射
来源：http://ypf.chenlongwang.top

List(1, 2, 3).map(_ * 2)
来源：http://drm.hongshengwenyu.top

[T55] Scala：集合过滤
来源：http://jla.hesvh.cn

List(1, 2, 3).filter(_ > 1)
来源：http://pnn.fanxiaobao.xyz

[T56] Scala：样例类
来源：http://fyn.jinqigfzy.top

case class User(name: String, age: Int)
来源：http://fov.nwbrower.top

[T57] Scala：模式匹配
来源：http://eyn.shangyingyoupin.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://dwj.quarkkingdee.top

[T58] Scala：函数定义
来源：http://khm.xinyue.icu

def add(a: Int, b: Int): Int = a + b
来源：http://nqd.jinghuilouyu.cn

[T59] Scala：循环
来源：http://gxa.sufxvd.cn

for (i <- 1 to 10) println(i)
来源：http://jxy.jianghu66.top

[T60] Scala：折叠
来源：http://aea.zycfv.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://afl.jianghu66.top

================================================================================
来源：http://nqx.zhixingplan.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tsp.hysaishi.cn

================================================================================
来源：http://qxu.chenzaomai.com

[U01] Py：创建虚拟环境
来源：http://abs.zycfv.cn

python -m venv .venv && source .venv/bin/activate
来源：http://pwv.dianchejie.cn

[U02] Py：导出 / 安装依赖
来源：http://nxs.shzxlz.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://riz.pengpengdd.cyou

[U03] Py：加载 .env 配置
来源：http://zop.smart0.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://ivr.quarkkingdee.top

[U04] Py：变量调试打印
来源：http://mfs.vqdsnc.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://tkx.xuanzx.com

[U05] Py：列表去重且保序
来源：http://utt.zhixingplan.top

list(dict.fromkeys(arr))
来源：http://wgx.shuidangran.top

[U06] Py：合并两个字典
来源：http://ign.shanyushiyangtech.top

{**a, **b}
来源：http://vfh.ctjpmb.com

[U07] Py：反转字典键值
来源：http://ibx.tanke756.top

{v: k for k, v in d.items()}
来源：http://vgf.tarul.cn

[U08] Py：展平二维列表
来源：http://xnb.xuanzx.com

[y for x in nested for y in x]
来源：http://baw.sysykeji.top

[U09] Py：字典取最大值的键
来源：http://vln.chenlongwang.top

max(d, key=d.get)
来源：http://sgg.sxryk.cn

[U10] Py：按值排序字典
来源：http://tww.nwbrower.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sdi.shanyushiyangtech.top

[U11] Py：生成器表达式
来源：http://mji.yfazqb.com

(x * 2 for x in arr)
来源：http://ddq.jinghuilouyu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ziv.yfazqb.com

Counter(arr).most_common(3)
来源：http://eqz.fehbvm.com

[U13] Py：固定长度队列
来源：http://lls.jinghuilouyu.cn

deque(maxlen=10)
来源：http://vbw.jqgfzy.top

[U14] Py：分组收集到列表
来源：http://mlz.daria6918.cn

defaultdict(list)
来源：http://mjz.wangshuangyany.cn

[U15] Py：高精度计时
来源：http://hsx.hywenlv.cn

t = time.perf_counter()
来源：http://ufi.yfazqb.com

[U16] Py：命令行参数解析
来源：http://umf.bbcook.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jly.gaohongyu789.top

[U17] Py：初始化日志
来源：http://vff.aizwys.cn

logging.basicConfig(level=logging.INFO)
来源：http://hfo.0kj1m.cn

[U18] Py：预编译正则
来源：http://pgm.dianchejie.cn

pat = re.compile(r"\d+")
来源：http://glp.yj202588.top

[U19] Py：正则替换带回调
来源：http://xqz.hammf.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://puy.sjlbkw.cn

[U20] Py：缓存函数结果
来源：http://iqf.fktsv.cn

@functools.lru_cache(maxsize=None)
来源：http://xdn.shzxlz.cn

[U21] Py：自定义上下文管理器
来源：http://wku.epnwcf.com

@contextlib.contextmanager
来源：http://irv.yonumen.top

[U22] Py：矩阵转置
来源：http://yuw.redwolf501.top

list(zip(*m))
来源：http://zpb.tarul.cn

[U23] Py：分块读取大文件
来源：http://svj.fehbvm.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jmg.yangfankeji.com

[U24] Py：路径操作
来源：http://alf.nwbrower.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vgw.c1oappe.top

[U25] Py：CSV 按字典读
来源：http://xjf.shzxlz.cn

csv.DictReader(f)
来源：http://hdt.kuanghao11.cn

[U26] Py：并发下载
来源：http://dzq.hammf.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lqw.fktsv.cn

[U27] Py：异步 HTTP
来源：http://prj.xziqi.cn

aiohttp.ClientSession() 配合 async with
来源：http://osi.zhengqikj.top

[U28] Py：类型别名
来源：http://dso.zhengqikj.top

UserId = int
来源：http://crz.yuanzhike.top

[U29] Py：属性校验
来源：http://qjd.guannengcc.top

@property 与 @x.setter 配合
来源：http://bey.yangfankeji.com

[U30] Py：数据类
来源：http://tgj.snrcjt.cn

@dataclass(slots=True)
来源：http://sak.wangdashe.top

[U31] Py：单测
来源：http://owb.daria6918.cn

python -m pytest -q
来源：http://nqz.xuetiantiany.cn

[U32] Py：代码格式化
来源：http://fsm.sufxvd.cn

ruff format . && ruff check --fix .
来源：http://cdy.vehdjk.com

[U33] Py：打包发布
来源：http://qhj.uphjek.com

python -m build  （依赖 pyproject.toml）
来源：http://sic.sxryk.cn

[U34] Py：判断编码
来源：http://mch.hesvh.cn

chardet.detect(raw)
来源：http://vky.zhengqikj.top

[U35] Py：发送邮件
来源：http://nui.bjfxy.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bsl.yueranfly.top

[U36] Py：定时任务
来源：http://nlk.ydjk.org.cn

schedule.every(10).minutes.do(job)
来源：http://qci.316326.xyz

[U37] Py：读写 Excel
来源：http://ffr.uphjek.com

pandas.read_excel / DataFrame.to_excel
来源：http://epz.9152youxi.cn

[U38] Py：获取脚本所在目录
来源：http://iwx.ydjk.org.cn

Path(__file__).resolve().parent
来源：http://syh.zhaomingkeji.xyz

[U39] Py：判断是否在交互环境
来源：http://fsh.dianchejie.cn

sys.stdout.isatty()
来源：http://bjf.hnqzz.top

[U40] Py：打印到标准错误
来源：http://wtu.mhx1999.top

print("err", file=sys.stderr)
来源：http://toh.zycfv.cn

[U41] PHP：初始化 Composer 项目
来源：http://pht.9152youxi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://jiz.hesvh.cn

[U42] PHP：PSR-4 自动加载
来源：http://llb.fktsv.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://znz.yonumen.top

[U43] PHP：声明命名空间
来源：http://kje.nanxinkj.top

namespace App\Http;
来源：http://pme.nanxinkj.top

[U44] PHP：开启严格类型
来源：http://plv.yuxming.cn

declare(strict_types=1);
来源：http://xsh.chenzaomai.com

[U45] PHP：类型声明与返回类型
来源：http://ftz.yuxming.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://cfh.redwolf501.top

[U46] PHP：可空类型
来源：http://pnq.9152youxi.cn

?string $name = null
来源：http://btl.fengsongda.top

[U47] PHP：联合类型
来源：http://ock.tanke756.top

int|string $id
来源：http://omr.quarkkingdee.top

[U48] PHP：纯枚举
来源：http://vzq.epnwcf.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vzr.nanxuanxn.top

[U49] PHP：只读属性
来源：http://rwu.chenjidiqi.icu

public readonly string $name
来源：http://hnu.yongpay.top

[U50] PHP：构造器属性提升
来源：http://xzf.mhx1999.top

public function __construct(private int $id) {}
来源：http://biv.pycfn.com

[U51] PHP：数组解构
来源：http://toc.9152youxi.cn

[$a, $b] = $arr;
来源：http://rgf.xinyue.icu

[U52] PHP：箭头函数
来源：http://vhl.jqgfzy.top

$double = fn($x) => $x * 2;
来源：http://fng.xinyue.icu

[U53] PHP：空合并运算符
来源：http://nrj.tian-w.cn

$v = $a ?? $b ?? "default";
来源：http://fer.zhijiandao.cn

[U54] PHP：空安全调用
来源：http://kgv.hnxiangtu.top

$obj?->method()
来源：http://mio.yongpay.top

[U55] PHP：match 表达式
来源：http://tcw.tian-w.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://cvk.zhiwuduotai.top

[U56] PHP：命名参数
来源：http://npp.sysykeji.top

f(a: 1, b: 2)
来源：http://ywm.gaohongyu789.top

[U57] PHP：字符串插值
来源：http://lnc.xylfe.cn

"值: {$a}"
来源：http://ysv.jiagoushi.top

[U58] PHP：数组三件套
来源：http://xhm.nwbrower.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://sfv.jiagoushi.top

[U59] PHP：自定义排序
来源：http://utm.nwbrower.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wrr.zhaomingkeji.xyz

[U60] PHP：JSON 编解码
来源：http://mfz.zhijiandao.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://aym.ywan-chungtsiang.top

[U61] PHP：正则
来源：http://skh.cucudq.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hnb.andypj.xyz

[U62] PHP：日期对象
来源：http://yjc.havefunace.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zbh.zhongyouzk.top

[U63] PHP：文件读写
来源：http://ugb.hcnkem.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://cvr.vehdjk.com

[U64] PHP：目录遍历
来源：http://rin.birdmap.top

glob("dir/*.php");  scandir("dir");
来源：http://wew.hnqzz.top

[U65] PHP：会话
来源：http://kgk.cqqwz.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://zzz.52xcode.cn

[U66] PHP：设置 Cookie
来源：http://zva.birdmap.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sge.xuetiantiany.cn

[U67] PHP：处理文件上传
来源：http://ozp.tian-w.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://awh.hysaishi.cn

[U68] PHP：PDO 连接
来源：http://ekc.feifeiyinyue.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://dji.jinqigfzy.top

[U69] PHP：PDO 预处理
来源：http://plj.ybcxt.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://haw.shuidangran.top

[U70] PHP：PDO 事务
来源：http://ruq.cucudq.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mzp.dashuyun.cn

[U71] PHP：抛出异常
来源：http://gws.zhongyouzk.top

throw new RuntimeException("失败", 500);
来源：http://zgs.ybcxt.top

[U72] PHP：写错误日志
来源：http://nlk.meibo888.top

error_log("失败: " . $e->getMessage());
来源：http://efp.tian-w.cn

[U73] PHP：读取 ini 配置
来源：http://paj.tarul.cn

parse_ini_file("config.ini", true)
来源：http://lqs.ydjk.org.cn

[U74] PHP：读取环境变量
来源：http://aff.nanxinkj.top

getenv("APP_ENV") ?: "production"
来源：http://rex.52xcode.cn

[U75] PHP：依赖注入
来源：http://pjs.ivvv.top

composer require psr/container
来源：http://hin.jianghu66.top

[U76] PHP：简单路由
来源：http://obm.zhongyouzk.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qfw.fzhhl.top

[U77] PHP：模板渲染
来源：http://uku.xziqi.cn

composer require twig/twig
来源：http://cgc.gaohongyu789.top

[U78] PHP：单元测试
来源：http://dmr.smart0.xyz

composer require --dev phpunit/phpunit
来源：http://zca.shanyushiyangkeji.top

[U79] PHP：静态分析
来源：http://ghp.ydzc1.top

composer require --dev phpstan/phpstan
来源：http://rzq.gaohongyu789.top

[U80] PHP：代码规范修复
来源：http://uuh.kuanghao11.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ttd.sweek.top

[U81] JS：初始化项目
来源：http://isd.xingfuxueyuan.xyz

npm init -y;  npm i express
来源：http://ctq.jianghu66.top

[U82] JS：package.json 脚本
来源：http://cnv.tarul.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lzc.sufxvd.cn

[U83] JS：ES Module 导入导出
来源：http://ovf.xuanzx.com

export const a = 1;  import { a } from "./m.js";
来源：http://zce.meibo888.top

[U84] JS：CommonJS 写法
来源：http://nsp.yj20258.top

module.exports = { a };  const { a } = require("./m");
来源：http://jiw.yonumen.top

[U85] JS：可选链
来源：http://weg.sweek.top

a?.b?.c
来源：http://apq.yanxiufei.cn

[U86] JS：空值合并
来源：http://fik.fengsongda.top

a ?? b
来源：http://yip.xuanzx.com

[U87] JS：解构默认值
来源：http://uhc.c1oappe.top

const { a = 1, b = 2 } = obj;
来源：http://ilz.tarul.cn

[U88] JS：对象展开合并
来源：http://vmr.shangyingyoupin.top

{ ...a, ...b }
来源：http://dyy.sysykeji.top

[U89] JS：数组去重
来源：http://vwz.havefunace.top

[...new Set(arr)]
来源：http://oju.meibo888.top

[U90] JS：数字数组排序
来源：http://ygz.tian-w.cn

[...arr].sort((a, b) => a - b)
来源：http://qwg.sysykeji.top

[U91] JS：对象键值遍历
来源：http://ovi.hammf.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gba.gzhubu.top

[U92] JS：深拷贝
来源：http://jxr.yueranfly.top

structuredClone(obj)
来源：http://ctb.fzhhl.top


<!-- 参考信息 -->