代发 wailian999

[T03] Kotlin：字符串模板
来源：http://bdr.sufxvd.cn

"值: $b"
来源：http://tdm.bjfxy.top

[T04] Kotlin：空安全
来源：http://vxe.52xcode.cn

val n: String? = null;  n?.length
来源：http://fog.bjfxy.top

[T05] Kotlin：when 表达式
来源：http://fhf.ppjwa.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rht.aizwys.cn

[T06] Kotlin：集合映射
来源：http://lce.nanxuanxn.top

listOf(1, 2, 3).map { it * 2 }
来源：http://pjf.jqgfzy.top

[T07] Kotlin：集合过滤
来源：http://ran.zycfv.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://nya.fktsv.cn

[T08] Kotlin：数据类
来源：http://wbq.cdnleiting.top

data class User(val name: String, val age: Int)
来源：http://dvg.gaohongyu789.top

[T09] Kotlin：扩展函数
来源：http://trq.ehwqpu.com

fun String.exclaim() = this + "!"
来源：http://ccu.zycfv.cn

[T10] Kotlin：默认参数
来源：http://stb.yonumen.top

fun greet(name: String = "World") = "Hi $name"
来源：http://qeb.hfpthk.cn

[T11] Kotlin：协程
来源：http://fmy.tian-w.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ylf.chenzaomai.com

[T12] Kotlin：解构声明
来源：http://swv.316326.xyz

val (a, b) = Pair(1, 2)
来源：http://ypn.yj20258.top

[T13] Kotlin：只读 Map
来源：http://cui.uphjek.com

val m = mapOf("a" to 1)
来源：http://ziw.jinqigfzy.top

[T14] Kotlin：循环
来源：http://smj.ppjwa.cn

for (i in 1..10) println(i)
来源：http://hjs.ybcxt.top

[T15] Kotlin：接口
来源：http://dow.cucudq.cn

interface Shape { fun area(): Double }
来源：http://cak.epnwcf.com

[T16] Swift：Hello World
来源：http://llv.ctjpmb.com

print("Hello")
来源：http://hbg.zhaomingkeji.xyz

[T17] Swift：变量与常量
来源：http://rdr.cheryme.top

var a = 1;  let b = 2
来源：http://aju.yj20258888.top

[T18] Swift：字符串插值
来源：http://nlh.meibo888.top

"值: \(b)"
来源：http://zlp.meibo888.top

[T19] Swift：可选绑定
来源：http://oso.gaohongyu789.top

if let n = opt { print(n) }
来源：http://pvs.wangshuangyany.cn

[T20] Swift：数组操作
来源：http://mxr.chenlongwang.top

var a = [1, 2, 3];  a.append(4)
来源：http://ejk.0kj1m.cn

[T21] Swift：遍历
来源：http://ixt.wangshuangyany.cn

for x in a { print(x) }
来源：http://lel.jqgfzy.top

[T22] Swift：字典
来源：http://omj.yangfankeji.com

var d = ["a": 1];  d["b"] = 2
来源：http://qxh.hesvh.cn

[T23] Swift：函数
来源：http://kiw.iojbl.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lmf.zhiwuduotai.top

[T24] Swift：闭包
来源：http://ysf.ywan-chungtsiang.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://rjt.fzhhl.top

[T25] Swift：结构体
来源：http://emj.yonumen.top

struct P { var x: Int }
来源：http://yuf.andypj.xyz

[T26] Swift：类与重写
来源：http://ylj.kuanghao11.cn

class A: Base { override func f() {} }
来源：http://pcy.daria6918.cn

[T27] Swift：错误处理
来源：http://jrb.hysaishi.cn

do { try f() } catch { print(error) }
来源：http://djh.yfazqb.com

[T28] Swift：枚举
来源：http://epa.chenjidiqi.icu

enum Color { case red, green }
来源：http://kay.zhoulong.xyz

[T29] Swift：guard 提前返回
来源：http://oir.zhoulong.xyz

guard let x = opt else { return }
来源：http://xkd.shuidangran.top

[T30] Swift：协议
来源：http://nwd.aizwys.cn

protocol Shape { func area() -> Double }
来源：http://dkd.316326.xyz

[T31] Lua：Hello World
来源：http://zvk.fehbvm.com

print("Hello")
来源：http://dkv.316326.xyz

[T32] Lua：局部变量
来源：http://yaw.vehdjk.com

local a = 1
来源：http://sac.kuanghao11.cn

[T33] Lua：表（数组）
来源：http://gqs.fktsv.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://xzg.zhoulong.xyz

[T34] Lua：遍历表
来源：http://lne.jinqigfzy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ich.jinyuanbaomall.cn

[T35] Lua：字典表
来源：http://sxh.zhaomingkeji.xyz

local d = { a = 1 };  d.b = 2
来源：http://vbs.meibo888.top

[T36] Lua：函数
来源：http://sqo.aibaodan.cn

function add(a, b) return a + b end
来源：http://oxt.jyoumei.cn

[T37] Lua：字符串拼接
来源：http://wju.0kj1m.cn

"a" .. "b"
来源：http://pjd.tian-w.cn

[T38] Lua：条件
来源：http://hxl.shanyushiyangtech.top

if x > 0 then print("正") end
来源：http://dan.aizwys.cn

[T39] Lua：模式匹配
来源：http://ool.yj202588.top

string.find(s, "%d+")
来源：http://gdl.gzhubu.top

[T40] Lua：元表
来源：http://dwn.cheryme.top

setmetatable({}, { __index = base })
来源：http://box.chenjidiqi.icu

[T41] Perl：Hello World
来源：http://urz.52xcode.cn

print "Hello\n";
来源：http://lny.fanxiaobao.xyz

[T42] Perl：变量类型
来源：http://wpd.zhoulong.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qsn.zhongyouzk.top

[T43] Perl：字符串插值
来源：http://run.jianghu66.top

"值: $a"
来源：http://yos.zdbjq.cn

[T44] Perl：条件
来源：http://vyc.vehdjk.com

if ($a > 0) { print "正"; }
来源：http://pyf.ydjk.org.cn

[T45] Perl：数组遍历
来源：http://jlh.vehdjk.com

for my $x (@arr) { print $x; }
来源：http://idi.fehbvm.com

[T46] Perl：哈希操作
来源：http://orq.zhengqikj.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://syl.shangyingyoupin.top

[T47] Perl：正则捕获
来源：http://std.daria6918.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ixu.bjfxy.top

[T48] Perl：正则替换
来源：http://qyx.dashuyun.cn

$s =~ s/old/new/g;
来源：http://mwn.cdnleiting.top

[T49] Perl：函数
来源：http://fks.wangshuangyany.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dib.tarul.cn

[T50] Perl：逐行读文件
来源：http://kif.xingfuxueyuan.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://nvp.sysykeji.top

while (my $line = <$fh>) { print $line; }
来源：http://cnq.pengpengdd.cyou

[T51] Scala：Hello World
来源：http://xkn.sweek.top

println("Hello")
来源：http://sxw.bbcook.cn

[T52] Scala：变量
来源：http://gom.ehwqpu.com

val a = 1;  var b = 2
来源：http://cde.hcnkem.com

[T53] Scala：字符串插值
来源：http://sbf.shanyushiyangtech.top

s"值: $b"
来源：http://tya.jianghu66.top

[T54] Scala：集合映射
来源：http://zfk.sxryk.cn

List(1, 2, 3).map(_ * 2)
来源：http://atm.sxryk.cn

[T55] Scala：集合过滤
来源：http://yxa.shanyushiyangtech.top

List(1, 2, 3).filter(_ > 1)
来源：http://fph.iojbl.cn

[T56] Scala：样例类
来源：http://qkc.jiagoushi.top

case class User(name: String, age: Int)
来源：http://wep.ydjk.org.cn

[T57] Scala：模式匹配
来源：http://yha.xuanzx.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://rkt.shanyushiyangtech.top

[T58] Scala：函数定义
来源：http://jay.pengpengdd.cyou

def add(a: Int, b: Int): Int = a + b
来源：http://fsc.316326.xyz

[T59] Scala：循环
来源：http://alu.cqqwz.cn

for (i <- 1 to 10) println(i)
来源：http://xia.zdqjudy.top

[T60] Scala：折叠
来源：http://bwv.pengpengdd.cyou

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lsy.feifeiyinyue.top

================================================================================
来源：http://ohl.guannengcc.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://asu.jqgfzy.top

================================================================================
来源：http://xwq.mhx1999.top

[U01] Py：创建虚拟环境
来源：http://jgf.cashguo.top

python -m venv .venv && source .venv/bin/activate
来源：http://iuz.c1oappe.top

[U02] Py：导出 / 安装依赖
来源：http://lzo.aibaodan.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dht.fanxiaobao.xyz

[U03] Py：加载 .env 配置
来源：http://ocm.cashguo.top

from dotenv import load_dotenv; load_dotenv()
来源：http://pjf.mhx1999.top

[U04] Py：变量调试打印
来源：http://smh.shangyingyoupin.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zoj.pengpengdd.cyou

[U05] Py：列表去重且保序
来源：http://yyy.zdqjudy.top

list(dict.fromkeys(arr))
来源：http://dma.zdqjudy.top

[U06] Py：合并两个字典
来源：http://klo.yj20258.top

{**a, **b}
来源：http://btd.meibo888.top

[U07] Py：反转字典键值
来源：http://hdg.ivvv.top

{v: k for k, v in d.items()}
来源：http://mrz.sweek.top

[U08] Py：展平二维列表
来源：http://icg.cheryme.top

[y for x in nested for y in x]
来源：http://kbk.feifeiyinyue.top

[U09] Py：字典取最大值的键
来源：http://nfh.feifeiyinyue.top

max(d, key=d.get)
来源：http://hbp.pycfn.com

[U10] Py：按值排序字典
来源：http://tzb.fengsongda.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jmp.pengpengdd.cyou

[U11] Py：生成器表达式
来源：http://dcg.jqgufenzy.top

(x * 2 for x in arr)
来源：http://guo.yfazqb.com

[U12] Py：取出现最多的 3 个元素
来源：http://wgl.jqgfzy.top

Counter(arr).most_common(3)
来源：http://qnh.sjlbkw.cn

[U13] Py：固定长度队列
来源：http://myi.zdbjq.cn

deque(maxlen=10)
来源：http://egg.aizwys.cn

[U14] Py：分组收集到列表
来源：http://mpz.yj20258888.top

defaultdict(list)
来源：http://cvy.daxiang520.top

[U15] Py：高精度计时
来源：http://dib.cashguo.top

t = time.perf_counter()
来源：http://phg.daxiang520.top

[U16] Py：命令行参数解析
来源：http://ptr.zhaomingkeji.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xrd.sxryk.cn

[U17] Py：初始化日志
来源：http://pad.sjlbkw.cn

logging.basicConfig(level=logging.INFO)
来源：http://smi.ehwqpu.com

[U18] Py：预编译正则
来源：http://ugq.jyoumei.cn

pat = re.compile(r"\d+")
来源：http://eqt.316326.xyz

[U19] Py：正则替换带回调
来源：http://dfi.xingfuxueyuan.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zap.mhx1999.top

[U20] Py：缓存函数结果
来源：http://jbo.cashguo.top

@functools.lru_cache(maxsize=None)
来源：http://isx.dianchejie.cn

[U21] Py：自定义上下文管理器
来源：http://mlo.52xcode.cn

@contextlib.contextmanager
来源：http://jbc.xingfuxueyuan.xyz

[U22] Py：矩阵转置
来源：http://siu.xuanzx.com

list(zip(*m))
来源：http://opc.yj20258888.top

[U23] Py：分块读取大文件
来源：http://xfq.316326.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mub.jiagoushi.top

[U24] Py：路径操作
来源：http://zwz.meibo888.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tyz.pengpengdd.cyou

[U25] Py：CSV 按字典读
来源：http://kbz.ydjk.org.cn

csv.DictReader(f)
来源：http://pte.dashuyun.cn

[U26] Py：并发下载
来源：http://vsj.tanke756.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wgf.pengpengdd.cyou

[U27] Py：异步 HTTP
来源：http://ddn.ydzc1.top

aiohttp.ClientSession() 配合 async with
来源：http://jdg.aizwys.cn

[U28] Py：类型别名
来源：http://gpr.jqgufenzy.top

UserId = int
来源：http://iyd.shanyushiyangtech.top

[U29] Py：属性校验
来源：http://zuq.svipenyu.cn

@property 与 @x.setter 配合
来源：http://jns.yj20258.top

[U30] Py：数据类
来源：http://frw.jyoumei.cn

@dataclass(slots=True)
来源：http://nze.quarkkingdee.top

[U31] Py：单测
来源：http://ydy.svipenyu.cn

python -m pytest -q
来源：http://jcn.hfpthk.cn

[U32] Py：代码格式化
来源：http://eit.hywenlv.cn

ruff format . && ruff check --fix .
来源：http://idy.yanxiufei.cn

[U33] Py：打包发布
来源：http://qjy.snrcjt.cn

python -m build  （依赖 pyproject.toml）
来源：http://goi.shangyingyoupin.top

[U34] Py：判断编码
来源：http://ioa.hcnkem.com

chardet.detect(raw)
来源：http://ilx.mhx1999.top

[U35] Py：发送邮件
来源：http://qtw.ehwqpu.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fxa.jinqigufen.top

[U36] Py：定时任务
来源：http://qiu.havefunace.top

schedule.every(10).minutes.do(job)
来源：http://llk.316326.xyz

[U37] Py：读写 Excel
来源：http://alk.jqgfzy.top

pandas.read_excel / DataFrame.to_excel
来源：http://loc.hammf.cn

[U38] Py：获取脚本所在目录
来源：http://hig.vqdsnc.cn

Path(__file__).resolve().parent
来源：http://qep.bbcook.cn

[U39] Py：判断是否在交互环境
来源：http://oob.ydzc1.top

sys.stdout.isatty()
来源：http://rkt.gogol.net.cn

[U40] Py：打印到标准错误
来源：http://obj.yongpay.top

print("err", file=sys.stderr)
来源：http://swd.zhoulong.xyz

[U41] PHP：初始化 Composer 项目
来源：http://teb.chenlongwang.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ldu.zdbjq.cn

[U42] PHP：PSR-4 自动加载
来源：http://anf.fehbvm.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://kwq.jqgufenzy.top

[U43] PHP：声明命名空间
来源：http://hsb.tarul.cn

namespace App\Http;
来源：http://thm.xuetiantiany.cn

[U44] PHP：开启严格类型
来源：http://ovg.aizwys.cn

declare(strict_types=1);
来源：http://ppt.jinyuanbaomall.cn

[U45] PHP：类型声明与返回类型
来源：http://tdi.xinyue.icu

function add(int $a, int $b): int { return $a + $b; }
来源：http://nda.52xcode.cn

[U46] PHP：可空类型
来源：http://haj.pycfn.com

?string $name = null
来源：http://byh.hongshengwenyu.top

[U47] PHP：联合类型
来源：http://mlg.yanxiufei.cn

int|string $id
来源：http://cyx.jyoumei.cn

[U48] PHP：纯枚举
来源：http://imd.andypj.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://afq.sjlbkw.cn

[U49] PHP：只读属性
来源：http://baz.gogol.net.cn

public readonly string $name
来源：http://fac.zhengqikj.top

[U50] PHP：构造器属性提升
来源：http://ajl.xingfuxueyuan.xyz

public function __construct(private int $id) {}
来源：http://mhr.meibo888.top

[U51] PHP：数组解构
来源：http://ehr.xuanzx.com

[$a, $b] = $arr;
来源：http://oin.shzxlz.cn

[U52] PHP：箭头函数
来源：http://aer.uphjek.com

$double = fn($x) => $x * 2;
来源：http://yax.jqgufenzy.top

[U53] PHP：空合并运算符
来源：http://qug.shzxlz.cn

$v = $a ?? $b ?? "default";
来源：http://fih.ctjpmb.com

[U54] PHP：空安全调用
来源：http://egx.nanxuanxn.top

$obj?->method()
来源：http://oui.xinyue.icu

[U55] PHP：match 表达式
来源：http://ffc.zhaomingkeji.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://sfh.wangshuangyany.cn

[U56] PHP：命名参数
来源：http://evv.ehwqpu.com

f(a: 1, b: 2)
来源：http://puq.gzhubu.top

[U57] PHP：字符串插值
来源：http://bcw.zdbjq.cn

"值: {$a}"
来源：http://aau.jiagoushi.top

[U58] PHP：数组三件套
来源：http://wpj.gotoacloud.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wrp.chenjidiqi.icu

[U59] PHP：自定义排序
来源：http://oco.hammf.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oby.yuxming.cn

[U60] PHP：JSON 编解码
来源：http://bke.tian-w.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tuv.gotoacloud.top

[U61] PHP：正则
来源：http://smm.mhx1999.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://evr.fktsv.cn

[U62] PHP：日期对象
来源：http://hzd.zhijiandao.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://tdh.jinghuilouyu.cn

[U63] PHP：文件读写
来源：http://mrm.iojbl.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rnz.hongshengwenyu.top

[U64] PHP：目录遍历
来源：http://yom.jlsjyb.cn

glob("dir/*.php");  scandir("dir");
来源：http://crv.chenlongwang.top

[U65] PHP：会话
来源：http://nyg.tarul.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://iov.hcnkem.com

[U66] PHP：设置 Cookie
来源：http://oaw.guannengcc.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ofq.meibo888.top

[U67] PHP：处理文件上传
来源：http://wur.xingfuxueyuan.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yaa.snrcjt.cn

[U68] PHP：PDO 连接
来源：http://qut.zhijiandao.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://byf.yj202588.top

[U69] PHP：PDO 预处理
来源：http://qls.316326.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://flh.haohaochexian.top

[U70] PHP：PDO 事务
来源：http://lcj.ppjwa.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xxe.yuanzhike.top

[U71] PHP：抛出异常
来源：http://tub.bjfxy.top

throw new RuntimeException("失败", 500);
来源：http://sze.tarul.cn

[U72] PHP：写错误日志
来源：http://zfk.epnwcf.com

error_log("失败: " . $e->getMessage());
来源：http://sug.zhoulong.xyz

[U73] PHP：读取 ini 配置
来源：http://bag.haohaochexian.top

parse_ini_file("config.ini", true)
来源：http://myh.cheryme.top

[U74] PHP：读取环境变量
来源：http://iaf.hnqzz.top

getenv("APP_ENV") ?: "production"
来源：http://fkp.gotoacloud.top

[U75] PHP：依赖注入
来源：http://dur.gogol.net.cn

composer require psr/container
来源：http://ypi.yj20258.top

[U76] PHP：简单路由
来源：http://jpl.shuidangran.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://sbf.shuidangran.top

[U77] PHP：模板渲染
来源：http://yct.mhx1999.top

composer require twig/twig
来源：http://bcn.fehbvm.com

[U78] PHP：单元测试
来源：http://yso.smart0.xyz

composer require --dev phpunit/phpunit
来源：http://gpv.zycfv.cn

[U79] PHP：静态分析
来源：http://oza.xuanzx.com

composer require --dev phpstan/phpstan
来源：http://ldd.snrcjt.cn

[U80] PHP：代码规范修复
来源：http://axh.zhijiandao.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://cxz.sysykeji.top

[U81] JS：初始化项目
来源：http://lmw.ehwqpu.com

npm init -y;  npm i express
来源：http://ote.aizwys.cn

[U82] JS：package.json 脚本
来源：http://tmx.fengsongda.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jbz.shanyushiyangtech.top

[U83] JS：ES Module 导入导出
来源：http://fjs.xylfe.cn

export const a = 1;  import { a } from "./m.js";
来源：http://fsj.andypj.xyz

[U84] JS：CommonJS 写法
来源：http://bcc.gaohongyu789.top

module.exports = { a };  const { a } = require("./m");
来源：http://hpz.ehwqpu.com

[U85] JS：可选链
来源：http://iyj.snrcjt.cn

a?.b?.c
来源：http://pad.xinyue.icu

[U86] JS：空值合并
来源：http://ote.redwolf501.top

a ?? b
来源：http://mnc.hcnkem.com

[U87] JS：解构默认值
来源：http://rfa.yangfankeji.com

const { a = 1, b = 2 } = obj;
来源：http://zns.hongshengwenyu.top

[U88] JS：对象展开合并
来源：http://nsl.yj20258.top

{ ...a, ...b }
来源：http://lkr.yonumen.top

[U89] JS：数组去重
来源：http://llt.yfazqb.com

[...new Set(arr)]
来源：http://ibo.chenlongwang.top

[U90] JS：数字数组排序
来源：http://zvj.sufxvd.cn

[...arr].sort((a, b) => a - b)
来源：http://klu.sysykeji.top


<!-- 参考信息 -->