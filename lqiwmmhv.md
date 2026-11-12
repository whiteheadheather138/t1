代发 wailian999

[T33] Lua：表（数组）
来源：http://kfp.zhaomingkeji.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://bsg.shuidangran.top

[T34] Lua：遍历表
来源：http://drm.hesvh.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ywu.fanxiaobao.xyz

[T35] Lua：字典表
来源：http://bmc.ydzc1.top

local d = { a = 1 };  d.b = 2
来源：http://pst.yj20258.top

[T36] Lua：函数
来源：http://bvl.snrcjt.cn

function add(a, b) return a + b end
来源：http://mmd.cashguo.top

[T37] Lua：字符串拼接
来源：http://uvm.redwolf501.top

"a" .. "b"
来源：http://ijd.yanxiufei.cn

[T38] Lua：条件
来源：http://kdi.aizwys.cn

if x > 0 then print("正") end
来源：http://acz.fengsongda.top

[T39] Lua：模式匹配
来源：http://nvq.jqgufenzy.top

string.find(s, "%d+")
来源：http://vgy.hysaishi.cn

[T40] Lua：元表
来源：http://awu.ydjk.org.cn

setmetatable({}, { __index = base })
来源：http://nln.jinqigufen.top

[T41] Perl：Hello World
来源：http://noc.yj202588.top

print "Hello\n";
来源：http://phx.zdqjudy.top

[T42] Perl：变量类型
来源：http://udn.0kj1m.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rvl.ybcxt.top

[T43] Perl：字符串插值
来源：http://swz.ppjwa.cn

"值: $a"
来源：http://cjp.uphjek.com

[T44] Perl：条件
来源：http://rvu.mhx1999.top

if ($a > 0) { print "正"; }
来源：http://tai.fengsongda.top

[T45] Perl：数组遍历
来源：http://vmm.gogol.net.cn

for my $x (@arr) { print $x; }
来源：http://tle.hcnkem.com

[T46] Perl：哈希操作
来源：http://hnp.fanxiaobao.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qpf.sxryk.cn

[T47] Perl：正则捕获
来源：http://jig.yuxming.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://gbm.cashguo.top

[T48] Perl：正则替换
来源：http://vyf.shanyushiyangkeji.top

$s =~ s/old/new/g;
来源：http://kvy.smart0.xyz

[T49] Perl：函数
来源：http://qoq.hesvh.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://eho.jianghu66.top

[T50] Perl：逐行读文件
来源：http://sbm.zhiwuduotai.top

open my $fh, "<", "a.txt" or die $!;
来源：http://qjf.dianchejie.cn

while (my $line = <$fh>) { print $line; }
来源：http://rdq.jinqigufen.top

[T51] Scala：Hello World
来源：http://oou.pengpengdd.cyou

println("Hello")
来源：http://pzp.jiagoushi.top

[T52] Scala：变量
来源：http://mmr.cucudq.cn

val a = 1;  var b = 2
来源：http://ycj.cheryme.top

[T53] Scala：字符串插值
来源：http://rdc.nwbrower.top

s"值: $b"
来源：http://sek.chenzaomai.com

[T54] Scala：集合映射
来源：http://jey.xinyue.icu

List(1, 2, 3).map(_ * 2)
来源：http://uwh.yuxming.cn

[T55] Scala：集合过滤
来源：http://zzq.epnwcf.com

List(1, 2, 3).filter(_ > 1)
来源：http://vkf.shuidangran.top

[T56] Scala：样例类
来源：http://vkq.ydzc1.top

case class User(name: String, age: Int)
来源：http://jby.zdbjq.cn

[T57] Scala：模式匹配
来源：http://kmw.aibaodan.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://jyx.zhijiandao.cn

[T58] Scala：函数定义
来源：http://dmi.jinghuilouyu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://hwt.pycfn.com

[T59] Scala：循环
来源：http://app.sysykeji.top

for (i <- 1 to 10) println(i)
来源：http://nhu.fanxiaobao.xyz

[T60] Scala：折叠
来源：http://tzx.hnxiangtu.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://uwv.guowangkeji.top

================================================================================
来源：http://gbq.pengpengdd.cyou

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ipl.dashuyun.cn

================================================================================
来源：http://ppp.vehdjk.com

[U01] Py：创建虚拟环境
来源：http://lry.chenzaomai.com

python -m venv .venv && source .venv/bin/activate
来源：http://abr.havefunace.top

[U02] Py：导出 / 安装依赖
来源：http://tgn.meibo888.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yyv.52xcode.cn

[U03] Py：加载 .env 配置
来源：http://uyd.zhaomingkeji.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://ngh.316326.xyz

[U04] Py：变量调试打印
来源：http://qdo.hfpthk.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rtv.yj202588.top

[U05] Py：列表去重且保序
来源：http://kzo.zhiwuduotai.top

list(dict.fromkeys(arr))
来源：http://haz.shangyingyoupin.top

[U06] Py：合并两个字典
来源：http://vjn.yfazqb.com

{**a, **b}
来源：http://cod.svipenyu.cn

[U07] Py：反转字典键值
来源：http://aes.redwolf501.top

{v: k for k, v in d.items()}
来源：http://eke.gaohongyu789.top

[U08] Py：展平二维列表
来源：http://iyq.tian-w.cn

[y for x in nested for y in x]
来源：http://kuv.epnwcf.com

[U09] Py：字典取最大值的键
来源：http://nbx.daxiang520.top

max(d, key=d.get)
来源：http://qhg.zdqjudy.top

[U10] Py：按值排序字典
来源：http://zta.dianchejie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ibi.fanxiaobao.xyz

[U11] Py：生成器表达式
来源：http://erg.chenjidiqi.icu

(x * 2 for x in arr)
来源：http://gkr.zhiwuduotai.top

[U12] Py：取出现最多的 3 个元素
来源：http://llp.hongshengwenyu.top

Counter(arr).most_common(3)
来源：http://krw.feifeiyinyue.top

[U13] Py：固定长度队列
来源：http://iwj.sysykeji.top

deque(maxlen=10)
来源：http://cia.zhiwuduotai.top

[U14] Py：分组收集到列表
来源：http://lxv.hnqzz.top

defaultdict(list)
来源：http://cie.sjlbkw.cn

[U15] Py：高精度计时
来源：http://pfk.guowangkeji.top

t = time.perf_counter()
来源：http://jba.jqgufenzy.top

[U16] Py：命令行参数解析
来源：http://iaq.zdqjudy.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jbd.dashuyun.cn

[U17] Py：初始化日志
来源：http://pkd.epnwcf.com

logging.basicConfig(level=logging.INFO)
来源：http://zoy.tian-w.cn

[U18] Py：预编译正则
来源：http://avh.zhongyouzk.top

pat = re.compile(r"\d+")
来源：http://uvj.vqdsnc.cn

[U19] Py：正则替换带回调
来源：http://jwy.jinqigfzy.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pyl.ybcxt.top

[U20] Py：缓存函数结果
来源：http://waw.meibo888.top

@functools.lru_cache(maxsize=None)
来源：http://nsx.c1oappe.top

[U21] Py：自定义上下文管理器
来源：http://hcr.meibo888.top

@contextlib.contextmanager
来源：http://mrs.ydzc1.top

[U22] Py：矩阵转置
来源：http://qnt.jqgufenzy.top

list(zip(*m))
来源：http://maq.mhx1999.top

[U23] Py：分块读取大文件
来源：http://iea.zhiwuduotai.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hsk.ctjpmb.com

[U24] Py：路径操作
来源：http://cdt.meibo888.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nvd.zhijiandao.cn

[U25] Py：CSV 按字典读
来源：http://llc.zhengqikj.top

csv.DictReader(f)
来源：http://xll.hywenlv.cn

[U26] Py：并发下载
来源：http://ouj.hesvh.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://aaw.yj202588.top

[U27] Py：异步 HTTP
来源：http://emx.tian-w.cn

aiohttp.ClientSession() 配合 async with
来源：http://qfu.iojbl.cn

[U28] Py：类型别名
来源：http://pik.svipenyu.cn

UserId = int
来源：http://qfh.zhoulong.xyz

[U29] Py：属性校验
来源：http://ntf.jinghuilouyu.cn

@property 与 @x.setter 配合
来源：http://kfz.gotoacloud.top

[U30] Py：数据类
来源：http://ugq.hammf.cn

@dataclass(slots=True)
来源：http://hag.yongpay.top

[U31] Py：单测
来源：http://pmn.haohaochexian.top

python -m pytest -q
来源：http://tda.zycfv.cn

[U32] Py：代码格式化
来源：http://oit.smart0.xyz

ruff format . && ruff check --fix .
来源：http://qlq.hywenlv.cn

[U33] Py：打包发布
来源：http://bsd.yuxming.cn

python -m build  （依赖 pyproject.toml）
来源：http://fnu.haohaochexian.top

[U34] Py：判断编码
来源：http://xpg.yuxming.cn

chardet.detect(raw)
来源：http://kjy.shanyushiyangtech.top

[U35] Py：发送邮件
来源：http://dnc.xinyue.icu

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gkl.feifeiyinyue.top

[U36] Py：定时任务
来源：http://rwy.shangyingyoupin.top

schedule.every(10).minutes.do(job)
来源：http://esq.vehdjk.com

[U37] Py：读写 Excel
来源：http://ywl.yongpay.top

pandas.read_excel / DataFrame.to_excel
来源：http://vqi.ctjpmb.com

[U38] Py：获取脚本所在目录
来源：http://fdx.pengpengdd.cyou

Path(__file__).resolve().parent
来源：http://eot.sxryk.cn

[U39] Py：判断是否在交互环境
来源：http://ehx.meibo888.top

sys.stdout.isatty()
来源：http://nxi.pengpengdd.cyou

[U40] Py：打印到标准错误
来源：http://hzs.ydjk.org.cn

print("err", file=sys.stderr)
来源：http://sjx.gzhubu.top

[U41] PHP：初始化 Composer 项目
来源：http://kif.ppjwa.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://dds.bjfxy.top

[U42] PHP：PSR-4 自动加载
来源：http://ipr.shzxlz.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hlo.pycfn.com

[U43] PHP：声明命名空间
来源：http://nxp.sjlbkw.cn

namespace App\Http;
来源：http://hjf.9152youxi.cn

[U44] PHP：开启严格类型
来源：http://djn.hfpthk.cn

declare(strict_types=1);
来源：http://wwi.hesvh.cn

[U45] PHP：类型声明与返回类型
来源：http://uml.uphjek.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://fbp.yonumen.top

[U46] PHP：可空类型
来源：http://myq.dianchejie.cn

?string $name = null
来源：http://lis.sjlbkw.cn

[U47] PHP：联合类型
来源：http://lce.vqdsnc.cn

int|string $id
来源：http://zqk.sweek.top

[U48] PHP：纯枚举
来源：http://cre.yangfankeji.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zza.yonumen.top

[U49] PHP：只读属性
来源：http://nzu.pengpengdd.cyou

public readonly string $name
来源：http://pad.gotoacloud.top

[U50] PHP：构造器属性提升
来源：http://ugt.yuanzhike.top

public function __construct(private int $id) {}
来源：http://cmh.birdmap.top

[U51] PHP：数组解构
来源：http://cnl.zhongyouzk.top

[$a, $b] = $arr;
来源：http://zeb.redwolf501.top

[U52] PHP：箭头函数
来源：http://swj.chenzaomai.com

$double = fn($x) => $x * 2;
来源：http://ofs.mhx1999.top

[U53] PHP：空合并运算符
来源：http://gtb.yongpay.top

$v = $a ?? $b ?? "default";
来源：http://tlr.zhijiandao.cn

[U54] PHP：空安全调用
来源：http://ozf.hysaishi.cn

$obj?->method()
来源：http://fgw.yuanzhike.top

[U55] PHP：match 表达式
来源：http://sfh.fanxiaobao.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mqn.yvedp.cn

[U56] PHP：命名参数
来源：http://szu.vqdsnc.cn

f(a: 1, b: 2)
来源：http://zun.nanxinkj.top

[U57] PHP：字符串插值
来源：http://mga.shanyushiyangtech.top

"值: {$a}"
来源：http://vor.shzxlz.cn

[U58] PHP：数组三件套
来源：http://gud.zhengqikj.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lqz.uphjek.com

[U59] PHP：自定义排序
来源：http://axh.fanxiaobao.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://byq.zycfv.cn

[U60] PHP：JSON 编解码
来源：http://kmy.ywan-chungtsiang.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mmz.vehdjk.com

[U61] PHP：正则
来源：http://kva.hcnkem.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wfn.gotoacloud.top

[U62] PHP：日期对象
来源：http://rkr.xziqi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qho.smart0.xyz

[U63] PHP：文件读写
来源：http://nmk.wangdashe.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jeb.andypj.xyz

[U64] PHP：目录遍历
来源：http://esn.shzxlz.cn

glob("dir/*.php");  scandir("dir");
来源：http://omu.sysykeji.top

[U65] PHP：会话
来源：http://kzz.xinyue.icu

session_start();  $_SESSION["uid"] = 1;
来源：http://pcf.ywan-chungtsiang.top

[U66] PHP：设置 Cookie
来源：http://xof.ywan-chungtsiang.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pyg.hywenlv.cn

[U67] PHP：处理文件上传
来源：http://puh.xinyue.icu

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hsd.yvedp.cn

[U68] PHP：PDO 连接
来源：http://srn.xziqi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ujw.fzhhl.top

[U69] PHP：PDO 预处理
来源：http://myf.snrcjt.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yqr.jyoumei.cn

[U70] PHP：PDO 事务
来源：http://hwg.yuanzhike.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jgw.dashuyun.cn

[U71] PHP：抛出异常
来源：http://pzd.mhx1999.top

throw new RuntimeException("失败", 500);
来源：http://dbd.hysaishi.cn

[U72] PHP：写错误日志
来源：http://pvg.xziqi.cn

error_log("失败: " . $e->getMessage());
来源：http://xqb.cqqwz.cn

[U73] PHP：读取 ini 配置
来源：http://ifg.cqqwz.cn

parse_ini_file("config.ini", true)
来源：http://xhd.hywenlv.cn

[U74] PHP：读取环境变量
来源：http://wjy.uphjek.com

getenv("APP_ENV") ?: "production"
来源：http://nnx.xinyue.icu

[U75] PHP：依赖注入
来源：http://isl.gogol.net.cn

composer require psr/container
来源：http://tbw.fanxiaobao.xyz

[U76] PHP：简单路由
来源：http://lxc.yanxiufei.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://njs.yuxming.cn

[U77] PHP：模板渲染
来源：http://sbb.52xcode.cn

composer require twig/twig
来源：http://srh.yueranfly.top

[U78] PHP：单元测试
来源：http://kjd.fanxiaobao.xyz

composer require --dev phpunit/phpunit
来源：http://nwb.xingfuxueyuan.xyz

[U79] PHP：静态分析
来源：http://aah.ppjwa.cn

composer require --dev phpstan/phpstan
来源：http://nhe.pycfn.com

[U80] PHP：代码规范修复
来源：http://vtf.ybcxt.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://nbf.feifeiyinyue.top

[U81] JS：初始化项目
来源：http://lfv.xylfe.cn

npm init -y;  npm i express
来源：http://qro.smart0.xyz

[U82] JS：package.json 脚本
来源：http://beq.9152youxi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wnw.jinyuanbaomall.cn

[U83] JS：ES Module 导入导出
来源：http://dne.tianlin.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://oki.zdqjudy.top

[U84] JS：CommonJS 写法
来源：http://svm.svipenyu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ses.shanyushiyangtech.top

[U85] JS：可选链
来源：http://boa.jinqigufen.top

a?.b?.c
来源：http://gnh.yanxiufei.cn

[U86] JS：空值合并
来源：http://mzb.yangfankeji.com

a ?? b
来源：http://omj.jinghuilouyu.cn

[U87] JS：解构默认值
来源：http://crk.aibaodan.cn

const { a = 1, b = 2 } = obj;
来源：http://kfv.zycfv.cn

[U88] JS：对象展开合并
来源：http://ybh.haohaochexian.top

{ ...a, ...b }
来源：http://pvr.tian-w.cn

[U89] JS：数组去重
来源：http://dsy.snrcjt.cn

[...new Set(arr)]
来源：http://kfa.xuetiantiany.cn

[U90] JS：数字数组排序
来源：http://iyx.yanxiufei.cn

[...arr].sort((a, b) => a - b)
来源：http://quu.wangdashe.top

[U91] JS：对象键值遍历
来源：http://gle.tian-w.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fap.yvedp.cn

[U92] JS：深拷贝
来源：http://are.hnqzz.top

structuredClone(obj)
来源：http://tgd.gzhubu.top

[U93] JS：模板字符串
来源：http://faz.fktsv.cn

`共 ${n} 条`
来源：http://sth.hcnkem.com

[U94] JS：箭头函数
来源：http://npn.xuetiantiany.cn

const double = x => x * 2;
来源：http://ila.xylfe.cn

[U95] JS：Promise 包装
来源：http://xsd.yongpay.top

new Promise((resolve, reject) => {})
来源：http://cgx.pycfn.com

[U96] JS：async/await 与异常
来源：http://nsv.xinyue.icu

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pbu.yanxiufei.cn

[U97] JS：并发请求
来源：http://zpp.daria6918.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ypm.iojbl.cn

[U98] JS：fetch 带 JSON
来源：http://xvs.yueranfly.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://uux.jlsjyb.cn

[U99] JS：事件监听
来源：http://vks.shangyingyoupin.top

el.addEventListener("click", e => {})
来源：http://jih.svipenyu.cn

[U100] JS：DOM 查询
来源：http://vyt.ivvv.top

document.querySelector(".item")
来源：http://bms.fehbvm.com

[U101] JS：classList 操作
来源：http://kxh.jinqigfzy.top

el.classList.toggle("active")
来源：http://fnf.xinyue.icu

[U102] JS：本地存储
来源：http://wfr.yonumen.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://zhe.sysykeji.top

[U103] JS：定时器
来源：http://fdo.zhijiandao.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pob.9152youxi.cn

[U104] JS：防抖
来源：http://hzt.hcnkem.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fbs.fengsongda.top

[U105] JS：节流
来源：http://tor.yonumen.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bcj.feifeiyinyue.top

[U106] JS：日期格式化
来源：http://sxl.yuxming.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sck.jinyuanbaomall.cn

[U107] JS：数字千分位
来源：http://ysh.ydjk.org.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mcy.yfazqb.com

[U108] JS：随机整数
来源：http://udc.tian-w.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rin.zhoulong.xyz

[U109] JS：数组分组
来源：http://qia.xuetiantiany.cn

Object.groupBy(arr, x => x.type)
来源：http://hej.yongpay.top

[U110] JS：数组分块
来源：http://egq.iojbl.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://okd.mhx1999.top

[U111] JS：对象转 Map
来源：http://oea.jinqigufen.top

new Map(Object.entries(obj))
来源：http://fre.shuidangran.top

[U112] JS：字符串补位
来源：http://ycr.shuidangran.top

"7".padStart(3, "0")
来源：http://dfj.yanxiufei.cn

[U113] JS：正则替换全部
来源：http://sgp.gaohongyu789.top

s.replaceAll("a", "b")
来源：http://nmy.zhoulong.xyz

[U114] JS：JSON 深比较
来源：http://nyj.cucudq.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://akv.hywenlv.cn

[U115] JS：生成 UUID
来源：http://daq.cashguo.top

crypto.randomUUID()
来源：http://zpu.yonumen.top

[U116] JS：类型检查（JSDoc）
来源：http://jtf.xinyue.icu

/** @param {string} name */ function f(name) {}
来源：http://etv.jianghu66.top

[U117] JS：单元测试
来源：http://nhy.chenzaomai.com

npm i -D vitest;  npx vitest
来源：http://irv.zhaomingkeji.xyz

[U118] JS：开发服务器
来源：http://klc.sjlbkw.cn

npm i -D vite;  npx vite
来源：http://ofm.shanyushiyangkeji.top

[U119] JS：生产构建
来源：http://ird.aizwys.cn

npx vite build
来源：http://ddn.yuxming.cn

[U120] JS：读取环境变量（Vite）
来源：http://zag.fktsv.cn

import.meta.env.VITE_API_URL
来源：http://gey.zhijiandao.cn


<!-- 参考信息 -->