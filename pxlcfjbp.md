代发 wailian999

[T03] Kotlin：字符串模板
来源：http://aou.yangfankeji.com

"值: $b"
来源：http://hdp.jlsjyb.cn

[T04] Kotlin：空安全
来源：http://lxz.zhoulong.xyz

val n: String? = null;  n?.length
来源：http://kzj.daria6918.cn

[T05] Kotlin：when 表达式
来源：http://uxm.hammf.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gzj.jqgfzy.top

[T06] Kotlin：集合映射
来源：http://fex.9152youxi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://caw.c1oappe.top

[T07] Kotlin：集合过滤
来源：http://ccv.zhaomingkeji.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://naq.bjfxy.top

[T08] Kotlin：数据类
来源：http://shz.hysaishi.cn

data class User(val name: String, val age: Int)
来源：http://hiw.jinghuilouyu.cn

[T09] Kotlin：扩展函数
来源：http://txw.zycfv.cn

fun String.exclaim() = this + "!"
来源：http://ooi.zhoulong.xyz

[T10] Kotlin：默认参数
来源：http://fma.hesvh.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ovo.zhijiandao.cn

[T11] Kotlin：协程
来源：http://eik.bjfxy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://yna.jqgufenzy.top

[T12] Kotlin：解构声明
来源：http://atb.nanxuanxn.top

val (a, b) = Pair(1, 2)
来源：http://yhs.tanke756.top

[T13] Kotlin：只读 Map
来源：http://imo.yonumen.top

val m = mapOf("a" to 1)
来源：http://yze.andypj.xyz

[T14] Kotlin：循环
来源：http://nho.pengpengdd.cyou

for (i in 1..10) println(i)
来源：http://swn.gzhubu.top

[T15] Kotlin：接口
来源：http://ewq.fengsongda.top

interface Shape { fun area(): Double }
来源：http://vtg.ydzc1.top

[T16] Swift：Hello World
来源：http://abh.chenlongwang.top

print("Hello")
来源：http://guf.yj20258.top

[T17] Swift：变量与常量
来源：http://epj.jqgfzy.top

var a = 1;  let b = 2
来源：http://wbk.zdqjudy.top

[T18] Swift：字符串插值
来源：http://qsu.quarkkingdee.top

"值: \(b)"
来源：http://dbj.hesvh.cn

[T19] Swift：可选绑定
来源：http://jcw.fehbvm.com

if let n = opt { print(n) }
来源：http://xsf.gzhubu.top

[T20] Swift：数组操作
来源：http://fjd.yfazqb.com

var a = [1, 2, 3];  a.append(4)
来源：http://dcg.yangfankeji.com

[T21] Swift：遍历
来源：http://xot.zdqjudy.top

for x in a { print(x) }
来源：http://wjd.sweek.top

[T22] Swift：字典
来源：http://wfp.pycfn.com

var d = ["a": 1];  d["b"] = 2
来源：http://svr.chenlongwang.top

[T23] Swift：函数
来源：http://rbd.ywan-chungtsiang.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kak.0kj1m.cn

[T24] Swift：闭包
来源：http://drq.jinghuilouyu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://fal.fzhhl.top

[T25] Swift：结构体
来源：http://gff.yfazqb.com

struct P { var x: Int }
来源：http://hxt.dashuyun.cn

[T26] Swift：类与重写
来源：http://pvo.birdmap.top

class A: Base { override func f() {} }
来源：http://wik.jinqigufen.top

[T27] Swift：错误处理
来源：http://jsy.havefunace.top

do { try f() } catch { print(error) }
来源：http://yqu.tarul.cn

[T28] Swift：枚举
来源：http://jzu.hysaishi.cn

enum Color { case red, green }
来源：http://dqc.ivvv.top

[T29] Swift：guard 提前返回
来源：http://mlq.zhoulong.xyz

guard let x = opt else { return }
来源：http://vjw.ehwqpu.com

[T30] Swift：协议
来源：http://tyn.gzhubu.top

protocol Shape { func area() -> Double }
来源：http://poe.jinqigufen.top

[T31] Lua：Hello World
来源：http://rbq.shuidangran.top

print("Hello")
来源：http://fjn.bjfxy.top

[T32] Lua：局部变量
来源：http://lpk.cheryme.top

local a = 1
来源：http://jkr.c1oappe.top

[T33] Lua：表（数组）
来源：http://cru.tanke756.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ttk.jlsjyb.cn

[T34] Lua：遍历表
来源：http://wpd.ppjwa.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://mpx.bjfxy.top

[T35] Lua：字典表
来源：http://mke.meibo888.top

local d = { a = 1 };  d.b = 2
来源：http://xzf.gotoacloud.top

[T36] Lua：函数
来源：http://fxg.aibaodan.cn

function add(a, b) return a + b end
来源：http://poi.hfpthk.cn

[T37] Lua：字符串拼接
来源：http://vjg.ehwqpu.com

"a" .. "b"
来源：http://qkk.daxiang520.top

[T38] Lua：条件
来源：http://hbr.jinyuanbaomall.cn

if x > 0 then print("正") end
来源：http://mjt.jianghu66.top

[T39] Lua：模式匹配
来源：http://ldt.zhixingplan.top

string.find(s, "%d+")
来源：http://upf.dianchejie.cn

[T40] Lua：元表
来源：http://mab.redwolf501.top

setmetatable({}, { __index = base })
来源：http://rhy.zhaomingkeji.xyz

[T41] Perl：Hello World
来源：http://ipr.cashguo.top

print "Hello\n";
来源：http://yzn.epnwcf.com

[T42] Perl：变量类型
来源：http://esv.ctjpmb.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ilo.xinyue.icu

[T43] Perl：字符串插值
来源：http://smy.kuanghao11.cn

"值: $a"
来源：http://drh.9152youxi.cn

[T44] Perl：条件
来源：http://ouw.gaohongyu789.top

if ($a > 0) { print "正"; }
来源：http://det.fehbvm.com

[T45] Perl：数组遍历
来源：http://dro.hnxiangtu.top

for my $x (@arr) { print $x; }
来源：http://fop.jinqigfzy.top

[T46] Perl：哈希操作
来源：http://kvr.yj202588.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vbn.c1oappe.top

[T47] Perl：正则捕获
来源：http://kkm.daxiang520.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://imz.hammf.cn

[T48] Perl：正则替换
来源：http://fey.zhongyouzk.top

$s =~ s/old/new/g;
来源：http://nkz.shanyushiyangkeji.top

[T49] Perl：函数
来源：http://loq.jinyuanbaomall.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rmr.aibaodan.cn

[T50] Perl：逐行读文件
来源：http://ksw.jinqigfzy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://xup.fengsongda.top

while (my $line = <$fh>) { print $line; }
来源：http://epk.fengsongda.top

[T51] Scala：Hello World
来源：http://qgl.hfpthk.cn

println("Hello")
来源：http://wyg.hywenlv.cn

[T52] Scala：变量
来源：http://far.sysykeji.top

val a = 1;  var b = 2
来源：http://qtg.yongpay.top

[T53] Scala：字符串插值
来源：http://kbz.yuxming.cn

s"值: $b"
来源：http://yzp.ydzc1.top

[T54] Scala：集合映射
来源：http://sfg.wangshuangyany.cn

List(1, 2, 3).map(_ * 2)
来源：http://gqc.zhongyouzk.top

[T55] Scala：集合过滤
来源：http://pvr.zhoulong.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://dgy.shangyingyoupin.top

[T56] Scala：样例类
来源：http://dev.fzhhl.top

case class User(name: String, age: Int)
来源：http://jmd.ivvv.top

[T57] Scala：模式匹配
来源：http://uop.yj202588.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://hgv.jqgufenzy.top

[T58] Scala：函数定义
来源：http://gqg.xylfe.cn

def add(a: Int, b: Int): Int = a + b
来源：http://dqt.ctjpmb.com

[T59] Scala：循环
来源：http://pvx.shuidangran.top

for (i <- 1 to 10) println(i)
来源：http://nrf.redwolf501.top

[T60] Scala：折叠
来源：http://rii.yj20258888.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qkf.cucudq.cn

================================================================================
来源：http://frl.zhongyouzk.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cyw.c1oappe.top

================================================================================
来源：http://rst.snrcjt.cn

[U01] Py：创建虚拟环境
来源：http://tgr.jianghu66.top

python -m venv .venv && source .venv/bin/activate
来源：http://frs.xziqi.cn

[U02] Py：导出 / 安装依赖
来源：http://jus.hongshengwenyu.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gjb.jinyuanbaomall.cn

[U03] Py：加载 .env 配置
来源：http://uxz.vqdsnc.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://iam.ctjpmb.com

[U04] Py：变量调试打印
来源：http://vfz.zdqjudy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vjx.zdqjudy.top

[U05] Py：列表去重且保序
来源：http://ksa.kuanghao11.cn

list(dict.fromkeys(arr))
来源：http://ati.xingfuxueyuan.xyz

[U06] Py：合并两个字典
来源：http://lch.haohaochexian.top

{**a, **b}
来源：http://pld.zhijiandao.cn

[U07] Py：反转字典键值
来源：http://ryf.fanxiaobao.xyz

{v: k for k, v in d.items()}
来源：http://qiv.cheryme.top

[U08] Py：展平二维列表
来源：http://zwp.hnxiangtu.top

[y for x in nested for y in x]
来源：http://xpt.wangshuangyany.cn

[U09] Py：字典取最大值的键
来源：http://aep.zhijiandao.cn

max(d, key=d.get)
来源：http://kdq.guannengcc.top

[U10] Py：按值排序字典
来源：http://god.zhiwuduotai.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://whd.xziqi.cn

[U11] Py：生成器表达式
来源：http://auc.jinqigfzy.top

(x * 2 for x in arr)
来源：http://gly.shanyushiyangkeji.top

[U12] Py：取出现最多的 3 个元素
来源：http://ffn.tian-w.cn

Counter(arr).most_common(3)
来源：http://sdl.ybcxt.top

[U13] Py：固定长度队列
来源：http://uae.9152youxi.cn

deque(maxlen=10)
来源：http://qpf.hfpthk.cn

[U14] Py：分组收集到列表
来源：http://nbe.sjlbkw.cn

defaultdict(list)
来源：http://qwp.snrcjt.cn

[U15] Py：高精度计时
来源：http://afr.jianghu66.top

t = time.perf_counter()
来源：http://nqb.aizwys.cn

[U16] Py：命令行参数解析
来源：http://hqk.sysykeji.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://uul.yfazqb.com

[U17] Py：初始化日志
来源：http://nna.chenzaomai.com

logging.basicConfig(level=logging.INFO)
来源：http://atk.smart0.xyz

[U18] Py：预编译正则
来源：http://xls.xziqi.cn

pat = re.compile(r"\d+")
来源：http://pot.aizwys.cn

[U19] Py：正则替换带回调
来源：http://hhw.fzhhl.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zwt.nwbrower.top

[U20] Py：缓存函数结果
来源：http://yjx.hfpthk.cn

@functools.lru_cache(maxsize=None)
来源：http://wgg.birdmap.top

[U21] Py：自定义上下文管理器
来源：http://rpv.zhoulong.xyz

@contextlib.contextmanager
来源：http://caq.ivvv.top

[U22] Py：矩阵转置
来源：http://nne.uphjek.com

list(zip(*m))
来源：http://ypt.daria6918.cn

[U23] Py：分块读取大文件
来源：http://dmm.dashuyun.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xvc.kuanghao11.cn

[U24] Py：路径操作
来源：http://mce.fengsongda.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xrf.guowangkeji.top

[U25] Py：CSV 按字典读
来源：http://dzz.sjlbkw.cn

csv.DictReader(f)
来源：http://akx.gaohongyu789.top

[U26] Py：并发下载
来源：http://opi.chenlongwang.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://uux.snrcjt.cn

[U27] Py：异步 HTTP
来源：http://hhe.ydjk.org.cn

aiohttp.ClientSession() 配合 async with
来源：http://xfp.chenjidiqi.icu

[U28] Py：类型别名
来源：http://wxd.gotoacloud.top

UserId = int
来源：http://kyd.shangyingyoupin.top

[U29] Py：属性校验
来源：http://mrv.shanyushiyangkeji.top

@property 与 @x.setter 配合
来源：http://yjp.xinyue.icu

[U30] Py：数据类
来源：http://nun.yueranfly.top

@dataclass(slots=True)
来源：http://oyf.jinyuanbaomall.cn

[U31] Py：单测
来源：http://wqr.gzhubu.top

python -m pytest -q
来源：http://wwy.yfazqb.com

[U32] Py：代码格式化
来源：http://ijo.shuidangran.top

ruff format . && ruff check --fix .
来源：http://asl.jinghuilouyu.cn

[U33] Py：打包发布
来源：http://dxn.0kj1m.cn

python -m build  （依赖 pyproject.toml）
来源：http://pfm.hammf.cn

[U34] Py：判断编码
来源：http://jyt.xylfe.cn

chardet.detect(raw)
来源：http://vqd.cucudq.cn

[U35] Py：发送邮件
来源：http://vgp.zdqjudy.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nsk.epnwcf.com

[U36] Py：定时任务
来源：http://kug.cheryme.top

schedule.every(10).minutes.do(job)
来源：http://xtl.zhengqikj.top

[U37] Py：读写 Excel
来源：http://kec.wangdashe.top

pandas.read_excel / DataFrame.to_excel
来源：http://eco.tianlin.xyz

[U38] Py：获取脚本所在目录
来源：http://sxx.zhixingplan.top

Path(__file__).resolve().parent
来源：http://njy.9152youxi.cn

[U39] Py：判断是否在交互环境
来源：http://jhb.pengpengdd.cyou

sys.stdout.isatty()
来源：http://lio.andypj.xyz

[U40] Py：打印到标准错误
来源：http://kqw.cheryme.top

print("err", file=sys.stderr)
来源：http://phj.chenjidiqi.icu

[U41] PHP：初始化 Composer 项目
来源：http://pzr.andypj.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://pqi.xinyue.icu

[U42] PHP：PSR-4 自动加载
来源：http://tvk.tianlin.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gwj.cucudq.cn

[U43] PHP：声明命名空间
来源：http://zky.dianchejie.cn

namespace App\Http;
来源：http://get.shzxlz.cn

[U44] PHP：开启严格类型
来源：http://jkn.shuidangran.top

declare(strict_types=1);
来源：http://xqx.zhiwuduotai.top

[U45] PHP：类型声明与返回类型
来源：http://iro.pengpengdd.cyou

function add(int $a, int $b): int { return $a + $b; }
来源：http://pwl.hcnkem.com

[U46] PHP：可空类型
来源：http://you.yanxiufei.cn

?string $name = null
来源：http://ezj.hammf.cn

[U47] PHP：联合类型
来源：http://usj.pycfn.com

int|string $id
来源：http://hmt.yvedp.cn

[U48] PHP：纯枚举
来源：http://oqt.fzhhl.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kfl.yongpay.top

[U49] PHP：只读属性
来源：http://aay.zhiwuduotai.top

public readonly string $name
来源：http://yyg.jinghuilouyu.cn

[U50] PHP：构造器属性提升
来源：http://eep.yj20258.top

public function __construct(private int $id) {}
来源：http://rlf.guowangkeji.top

[U51] PHP：数组解构
来源：http://ufw.jinqigufen.top

[$a, $b] = $arr;
来源：http://qev.yj20258.top

[U52] PHP：箭头函数
来源：http://dow.feifeiyinyue.top

$double = fn($x) => $x * 2;
来源：http://zha.yongpay.top

[U53] PHP：空合并运算符
来源：http://nrg.hongshengwenyu.top

$v = $a ?? $b ?? "default";
来源：http://xlu.zycfv.cn

[U54] PHP：空安全调用
来源：http://gkf.tarul.cn

$obj?->method()
来源：http://kes.hongshengwenyu.top

[U55] PHP：match 表达式
来源：http://imh.fzhhl.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vln.jqgufenzy.top

[U56] PHP：命名参数
来源：http://epw.c1oappe.top

f(a: 1, b: 2)
来源：http://niu.pengpengdd.cyou

[U57] PHP：字符串插值
来源：http://kdv.yangfankeji.com

"值: {$a}"
来源：http://dfs.sjlbkw.cn

[U58] PHP：数组三件套
来源：http://dut.sjlbkw.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kpt.shzxlz.cn

[U59] PHP：自定义排序
来源：http://hox.iojbl.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://myz.nwbrower.top

[U60] PHP：JSON 编解码
来源：http://ezy.vehdjk.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gdv.zycfv.cn

[U61] PHP：正则
来源：http://bcd.sxryk.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lnt.shangyingyoupin.top

[U62] PHP：日期对象
来源：http://rnn.zycfv.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ldu.yongpay.top

[U63] PHP：文件读写
来源：http://uuh.uphjek.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://iqn.dianchejie.cn

[U64] PHP：目录遍历
来源：http://kbr.yj20258.top

glob("dir/*.php");  scandir("dir");
来源：http://hby.52xcode.cn

[U65] PHP：会话
来源：http://jnk.nanxinkj.top

session_start();  $_SESSION["uid"] = 1;
来源：http://xln.shzxlz.cn

[U66] PHP：设置 Cookie
来源：http://glp.zdbjq.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gxm.ehwqpu.com

[U67] PHP：处理文件上传
来源：http://ipb.ydzc1.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gen.shanyushiyangtech.top

[U68] PHP：PDO 连接
来源：http://ier.birdmap.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://aoa.nanxuanxn.top

[U69] PHP：PDO 预处理
来源：http://bsh.sysykeji.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://uiz.jiagoushi.top

[U70] PHP：PDO 事务
来源：http://uui.shanyushiyangtech.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bje.epnwcf.com

[U71] PHP：抛出异常
来源：http://zco.sweek.top

throw new RuntimeException("失败", 500);
来源：http://nfq.hfpthk.cn

[U72] PHP：写错误日志
来源：http://qxi.ydjk.org.cn

error_log("失败: " . $e->getMessage());
来源：http://lzm.daria6918.cn

[U73] PHP：读取 ini 配置
来源：http://xgd.xziqi.cn

parse_ini_file("config.ini", true)
来源：http://meg.aizwys.cn

[U74] PHP：读取环境变量
来源：http://vch.c1oappe.top

getenv("APP_ENV") ?: "production"
来源：http://iqe.dashuyun.cn

[U75] PHP：依赖注入
来源：http://rwy.fktsv.cn

composer require psr/container
来源：http://aia.hnqzz.top

[U76] PHP：简单路由
来源：http://vdi.ywan-chungtsiang.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lie.sjlbkw.cn

[U77] PHP：模板渲染
来源：http://ywm.fktsv.cn

composer require twig/twig
来源：http://ipp.tarul.cn

[U78] PHP：单元测试
来源：http://imk.haohaochexian.top

composer require --dev phpunit/phpunit
来源：http://rep.chenzaomai.com

[U79] PHP：静态分析
来源：http://exp.chenzaomai.com

composer require --dev phpstan/phpstan
来源：http://amv.zhixingplan.top

[U80] PHP：代码规范修复
来源：http://lwg.shanyushiyangkeji.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://bct.sysykeji.top

[U81] JS：初始化项目
来源：http://yog.yuanzhike.top

npm init -y;  npm i express
来源：http://adu.yongpay.top

[U82] JS：package.json 脚本
来源：http://bbo.jianghu66.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://apo.pycfn.com

[U83] JS：ES Module 导入导出
来源：http://ikx.cashguo.top

export const a = 1;  import { a } from "./m.js";
来源：http://jih.hnqzz.top

[U84] JS：CommonJS 写法
来源：http://kul.xuetiantiany.cn

module.exports = { a };  const { a } = require("./m");
来源：http://jlj.fktsv.cn

[U85] JS：可选链
来源：http://tel.guowangkeji.top

a?.b?.c
来源：http://ajb.gaohongyu789.top

[U86] JS：空值合并
来源：http://dwn.epnwcf.com

a ?? b
来源：http://ejx.birdmap.top

[U87] JS：解构默认值
来源：http://khi.cucudq.cn

const { a = 1, b = 2 } = obj;
来源：http://ytt.guannengcc.top

[U88] JS：对象展开合并
来源：http://nck.mhx1999.top

{ ...a, ...b }
来源：http://ehu.yfazqb.com

[U89] JS：数组去重
来源：http://ipg.zdbjq.cn

[...new Set(arr)]
来源：http://aqq.ivvv.top

[U90] JS：数字数组排序
来源：http://bnu.zhijiandao.cn

[...arr].sort((a, b) => a - b)
来源：http://zvj.ywan-chungtsiang.top


<!-- 参考信息 -->