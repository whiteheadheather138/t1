代发 wailian999

[T31] Lua：Hello World
来源：http://stp.bjfxy.top

print("Hello")
来源：http://wyn.xziqi.cn

[T32] Lua：局部变量
来源：http://jul.quarkkingdee.top

local a = 1
来源：http://xqf.9152youxi.cn

[T33] Lua：表（数组）
来源：http://ada.pengpengdd.cyou

local t = {1, 2, 3};  t[4] = 4
来源：http://cyj.jlsjyb.cn

[T34] Lua：遍历表
来源：http://glk.cucudq.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://asr.zhiwuduotai.top

[T35] Lua：字典表
来源：http://aov.yuxming.cn

local d = { a = 1 };  d.b = 2
来源：http://sxp.fktsv.cn

[T36] Lua：函数
来源：http://nao.cqqwz.cn

function add(a, b) return a + b end
来源：http://hji.meibo888.top

[T37] Lua：字符串拼接
来源：http://dqf.yuxming.cn

"a" .. "b"
来源：http://qxh.jyoumei.cn

[T38] Lua：条件
来源：http://gvo.sufxvd.cn

if x > 0 then print("正") end
来源：http://nlv.jqgufenzy.top

[T39] Lua：模式匹配
来源：http://njz.yanxiufei.cn

string.find(s, "%d+")
来源：http://mge.fehbvm.com

[T40] Lua：元表
来源：http://mwg.tian-w.cn

setmetatable({}, { __index = base })
来源：http://mnr.tianlin.xyz

[T41] Perl：Hello World
来源：http://cpp.tanke756.top

print "Hello\n";
来源：http://qkg.uphjek.com

[T42] Perl：变量类型
来源：http://spl.yangfankeji.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://iag.cheryme.top

[T43] Perl：字符串插值
来源：http://ahy.fehbvm.com

"值: $a"
来源：http://hnc.mhx1999.top

[T44] Perl：条件
来源：http://key.uphjek.com

if ($a > 0) { print "正"; }
来源：http://jyw.tanke756.top

[T45] Perl：数组遍历
来源：http://puw.birdmap.top

for my $x (@arr) { print $x; }
来源：http://tso.chenlongwang.top

[T46] Perl：哈希操作
来源：http://cbc.shzxlz.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://guy.yanxiufei.cn

[T47] Perl：正则捕获
来源：http://hjc.cdnleiting.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://fsk.yangfankeji.com

[T48] Perl：正则替换
来源：http://nwn.zdqjudy.top

$s =~ s/old/new/g;
来源：http://eti.ppjwa.cn

[T49] Perl：函数
来源：http://ekw.ydjk.org.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vda.ydjk.org.cn

[T50] Perl：逐行读文件
来源：http://uww.bbcook.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zgw.nanxinkj.top

while (my $line = <$fh>) { print $line; }
来源：http://erd.jqgfzy.top

[T51] Scala：Hello World
来源：http://fzo.sjlbkw.cn

println("Hello")
来源：http://vro.havefunace.top

[T52] Scala：变量
来源：http://iis.yvedp.cn

val a = 1;  var b = 2
来源：http://tnf.fehbvm.com

[T53] Scala：字符串插值
来源：http://neq.havefunace.top

s"值: $b"
来源：http://caf.fehbvm.com

[T54] Scala：集合映射
来源：http://oto.tian-w.cn

List(1, 2, 3).map(_ * 2)
来源：http://mtx.gogol.net.cn

[T55] Scala：集合过滤
来源：http://nzv.jinghuilouyu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://rbr.birdmap.top

[T56] Scala：样例类
来源：http://slu.mhx1999.top

case class User(name: String, age: Int)
来源：http://hrq.fktsv.cn

[T57] Scala：模式匹配
来源：http://urv.zhixingplan.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://klb.sysykeji.top

[T58] Scala：函数定义
来源：http://xar.52xcode.cn

def add(a: Int, b: Int): Int = a + b
来源：http://eph.chenjidiqi.icu

[T59] Scala：循环
来源：http://bou.vehdjk.com

for (i <- 1 to 10) println(i)
来源：http://qyl.shzxlz.cn

[T60] Scala：折叠
来源：http://mhh.ppjwa.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jnl.yj202588.top

================================================================================
来源：http://zuo.cheryme.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rdf.hesvh.cn

================================================================================
来源：http://vgg.cashguo.top

[U01] Py：创建虚拟环境
来源：http://onh.yj202588.top

python -m venv .venv && source .venv/bin/activate
来源：http://wys.smart0.xyz

[U02] Py：导出 / 安装依赖
来源：http://zpp.dashuyun.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mvp.gzhubu.top

[U03] Py：加载 .env 配置
来源：http://nor.bjfxy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ivz.cheryme.top

[U04] Py：变量调试打印
来源：http://ypi.zhijiandao.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nvj.fehbvm.com

[U05] Py：列表去重且保序
来源：http://dpm.hnxiangtu.top

list(dict.fromkeys(arr))
来源：http://kfl.yongpay.top

[U06] Py：合并两个字典
来源：http://grw.ehwqpu.com

{**a, **b}
来源：http://uqe.ydzc1.top

[U07] Py：反转字典键值
来源：http://grd.chenlongwang.top

{v: k for k, v in d.items()}
来源：http://xio.gzhubu.top

[U08] Py：展平二维列表
来源：http://pfq.ydjk.org.cn

[y for x in nested for y in x]
来源：http://rnp.chenlongwang.top

[U09] Py：字典取最大值的键
来源：http://aad.zhijiandao.cn

max(d, key=d.get)
来源：http://vpv.cashguo.top

[U10] Py：按值排序字典
来源：http://jtr.hysaishi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cjg.ybcxt.top

[U11] Py：生成器表达式
来源：http://dnv.yvedp.cn

(x * 2 for x in arr)
来源：http://hca.zhixingplan.top

[U12] Py：取出现最多的 3 个元素
来源：http://aha.hfpthk.cn

Counter(arr).most_common(3)
来源：http://xbv.xziqi.cn

[U13] Py：固定长度队列
来源：http://dyy.hywenlv.cn

deque(maxlen=10)
来源：http://vnl.xinyue.icu

[U14] Py：分组收集到列表
来源：http://fdw.gotoacloud.top

defaultdict(list)
来源：http://jci.aizwys.cn

[U15] Py：高精度计时
来源：http://zjx.pengpengdd.cyou

t = time.perf_counter()
来源：http://ylh.316326.xyz

[U16] Py：命令行参数解析
来源：http://qkm.tian-w.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://but.316326.xyz

[U17] Py：初始化日志
来源：http://myp.gzhubu.top

logging.basicConfig(level=logging.INFO)
来源：http://otw.jqgufenzy.top

[U18] Py：预编译正则
来源：http://yyu.snrcjt.cn

pat = re.compile(r"\d+")
来源：http://ayy.chenlongwang.top

[U19] Py：正则替换带回调
来源：http://tiw.0kj1m.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ifo.9152youxi.cn

[U20] Py：缓存函数结果
来源：http://rxb.shangyingyoupin.top

@functools.lru_cache(maxsize=None)
来源：http://doi.sufxvd.cn

[U21] Py：自定义上下文管理器
来源：http://dev.jinqigufen.top

@contextlib.contextmanager
来源：http://gnm.iojbl.cn

[U22] Py：矩阵转置
来源：http://gjl.jlsjyb.cn

list(zip(*m))
来源：http://zqo.guowangkeji.top

[U23] Py：分块读取大文件
来源：http://skp.jianghu66.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vql.fanxiaobao.xyz

[U24] Py：路径操作
来源：http://lhw.ydjk.org.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qtr.jqgufenzy.top

[U25] Py：CSV 按字典读
来源：http://xsv.aibaodan.cn

csv.DictReader(f)
来源：http://quc.quarkkingdee.top

[U26] Py：并发下载
来源：http://kyy.mhx1999.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xgp.hysaishi.cn

[U27] Py：异步 HTTP
来源：http://hdk.shanyushiyangkeji.top

aiohttp.ClientSession() 配合 async with
来源：http://yep.sufxvd.cn

[U28] Py：类型别名
来源：http://lde.c1oappe.top

UserId = int
来源：http://xmb.jinyuanbaomall.cn

[U29] Py：属性校验
来源：http://adu.yuxming.cn

@property 与 @x.setter 配合
来源：http://maz.quarkkingdee.top

[U30] Py：数据类
来源：http://vgi.sjlbkw.cn

@dataclass(slots=True)
来源：http://ndk.jiagoushi.top

[U31] Py：单测
来源：http://sqw.cqqwz.cn

python -m pytest -q
来源：http://ygk.shanyushiyangkeji.top

[U32] Py：代码格式化
来源：http://vfx.hywenlv.cn

ruff format . && ruff check --fix .
来源：http://gii.hnqzz.top

[U33] Py：打包发布
来源：http://yxm.sysykeji.top

python -m build  （依赖 pyproject.toml）
来源：http://tng.vehdjk.com

[U34] Py：判断编码
来源：http://tci.ivvv.top

chardet.detect(raw)
来源：http://xpw.cqqwz.cn

[U35] Py：发送邮件
来源：http://dyb.yongpay.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nve.ydzc1.top

[U36] Py：定时任务
来源：http://vic.fktsv.cn

schedule.every(10).minutes.do(job)
来源：http://nvg.sysykeji.top

[U37] Py：读写 Excel
来源：http://gyo.sweek.top

pandas.read_excel / DataFrame.to_excel
来源：http://rgd.xziqi.cn

[U38] Py：获取脚本所在目录
来源：http://grt.cheryme.top

Path(__file__).resolve().parent
来源：http://ipk.zycfv.cn

[U39] Py：判断是否在交互环境
来源：http://acc.jianghu66.top

sys.stdout.isatty()
来源：http://nxc.gzhubu.top

[U40] Py：打印到标准错误
来源：http://onj.hnqzz.top

print("err", file=sys.stderr)
来源：http://pac.zhiwuduotai.top

[U41] PHP：初始化 Composer 项目
来源：http://eum.nanxuanxn.top

composer init;  composer require guzzlehttp/guzzle
来源：http://vys.fehbvm.com

[U42] PHP：PSR-4 自动加载
来源：http://wew.pengpengdd.cyou

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://uvv.316326.xyz

[U43] PHP：声明命名空间
来源：http://zpc.zdbjq.cn

namespace App\Http;
来源：http://epr.sweek.top

[U44] PHP：开启严格类型
来源：http://wjb.jinqigufen.top

declare(strict_types=1);
来源：http://ftr.jianghu66.top

[U45] PHP：类型声明与返回类型
来源：http://dlv.wangshuangyany.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://fjh.zdbjq.cn

[U46] PHP：可空类型
来源：http://bkc.xinyue.icu

?string $name = null
来源：http://ygn.yj20258.top

[U47] PHP：联合类型
来源：http://dpa.gogol.net.cn

int|string $id
来源：http://gzo.dianchejie.cn

[U48] PHP：纯枚举
来源：http://mbx.fanxiaobao.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gjc.gotoacloud.top

[U49] PHP：只读属性
来源：http://rol.fanxiaobao.xyz

public readonly string $name
来源：http://lla.zhoulong.xyz

[U50] PHP：构造器属性提升
来源：http://eul.52xcode.cn

public function __construct(private int $id) {}
来源：http://kcl.pycfn.com

[U51] PHP：数组解构
来源：http://scm.gogol.net.cn

[$a, $b] = $arr;
来源：http://qat.feifeiyinyue.top

[U52] PHP：箭头函数
来源：http://mgb.quarkkingdee.top

$double = fn($x) => $x * 2;
来源：http://pcq.gaohongyu789.top

[U53] PHP：空合并运算符
来源：http://spb.ydzc1.top

$v = $a ?? $b ?? "default";
来源：http://ixb.shanyushiyangkeji.top

[U54] PHP：空安全调用
来源：http://gyg.nanxuanxn.top

$obj?->method()
来源：http://vhz.cucudq.cn

[U55] PHP：match 表达式
来源：http://iry.yueranfly.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dgu.sjlbkw.cn

[U56] PHP：命名参数
来源：http://jxk.gogol.net.cn

f(a: 1, b: 2)
来源：http://kpa.yfazqb.com

[U57] PHP：字符串插值
来源：http://ujp.meibo888.top

"值: {$a}"
来源：http://flx.andypj.xyz

[U58] PHP：数组三件套
来源：http://dtx.shuidangran.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ils.chenjidiqi.icu

[U59] PHP：自定义排序
来源：http://pip.yangfankeji.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tdo.wangshuangyany.cn

[U60] PHP：JSON 编解码
来源：http://dqh.zhongyouzk.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dwc.andypj.xyz

[U61] PHP：正则
来源：http://kjr.aizwys.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://juw.xuetiantiany.cn

[U62] PHP：日期对象
来源：http://tfw.aibaodan.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://dis.zhoulong.xyz

[U63] PHP：文件读写
来源：http://lwy.tanke756.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xkw.fzhhl.top

[U64] PHP：目录遍历
来源：http://dcn.bjfxy.top

glob("dir/*.php");  scandir("dir");
来源：http://ywa.jlsjyb.cn

[U65] PHP：会话
来源：http://xxy.cheryme.top

session_start();  $_SESSION["uid"] = 1;
来源：http://tvt.hcnkem.com

[U66] PHP：设置 Cookie
来源：http://wcv.birdmap.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://syi.pengpengdd.cyou

[U67] PHP：处理文件上传
来源：http://oxx.hnxiangtu.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jly.haohaochexian.top

[U68] PHP：PDO 连接
来源：http://cgx.cdnleiting.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kjv.epnwcf.com

[U69] PHP：PDO 预处理
来源：http://qms.xuanzx.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xgt.yongpay.top

[U70] PHP：PDO 事务
来源：http://pkz.jianghu66.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hye.ydjk.org.cn

[U71] PHP：抛出异常
来源：http://chy.aibaodan.cn

throw new RuntimeException("失败", 500);
来源：http://plc.hnqzz.top

[U72] PHP：写错误日志
来源：http://pgg.ctjpmb.com

error_log("失败: " . $e->getMessage());
来源：http://hlc.dashuyun.cn

[U73] PHP：读取 ini 配置
来源：http://jzf.chenzaomai.com

parse_ini_file("config.ini", true)
来源：http://ovi.zhiwuduotai.top

[U74] PHP：读取环境变量
来源：http://ifl.shangyingyoupin.top

getenv("APP_ENV") ?: "production"
来源：http://mzg.xinyue.icu

[U75] PHP：依赖注入
来源：http://sgq.nwbrower.top

composer require psr/container
来源：http://wdm.ywan-chungtsiang.top

[U76] PHP：简单路由
来源：http://sxd.gaohongyu789.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gce.chenlongwang.top

[U77] PHP：模板渲染
来源：http://wts.tian-w.cn

composer require twig/twig
来源：http://dpz.vehdjk.com

[U78] PHP：单元测试
来源：http://pfl.cqqwz.cn

composer require --dev phpunit/phpunit
来源：http://wpd.gzhubu.top

[U79] PHP：静态分析
来源：http://twi.dashuyun.cn

composer require --dev phpstan/phpstan
来源：http://hfe.hysaishi.cn

[U80] PHP：代码规范修复
来源：http://bmt.52xcode.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://jxj.pengpengdd.cyou

[U81] JS：初始化项目
来源：http://upq.xziqi.cn

npm init -y;  npm i express
来源：http://wxz.jlsjyb.cn

[U82] JS：package.json 脚本
来源：http://tcz.jlsjyb.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://dhy.xziqi.cn

[U83] JS：ES Module 导入导出
来源：http://vsn.ydzc1.top

export const a = 1;  import { a } from "./m.js";
来源：http://rxp.wangshuangyany.cn

[U84] JS：CommonJS 写法
来源：http://jwp.zhoulong.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://ury.jyoumei.cn

[U85] JS：可选链
来源：http://kam.mhx1999.top

a?.b?.c
来源：http://qge.nanxinkj.top

[U86] JS：空值合并
来源：http://whq.hammf.cn

a ?? b
来源：http://rby.zhaomingkeji.xyz

[U87] JS：解构默认值
来源：http://seg.sxryk.cn

const { a = 1, b = 2 } = obj;
来源：http://vug.yuanzhike.top

[U88] JS：对象展开合并
来源：http://opl.xuetiantiany.cn

{ ...a, ...b }
来源：http://zeu.yj20258.top

[U89] JS：数组去重
来源：http://afb.pengpengdd.cyou

[...new Set(arr)]
来源：http://hvu.uphjek.com

[U90] JS：数字数组排序
来源：http://khu.nwbrower.top

[...arr].sort((a, b) => a - b)
来源：http://xbb.feifeiyinyue.top

[U91] JS：对象键值遍历
来源：http://rpj.smart0.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hhh.fengsongda.top

[U92] JS：深拷贝
来源：http://usv.wangdashe.top

structuredClone(obj)
来源：http://rkl.bjfxy.top

[U93] JS：模板字符串
来源：http://ddu.vehdjk.com

`共 ${n} 条`
来源：http://oto.chenlongwang.top

[U94] JS：箭头函数
来源：http://vpc.gaohongyu789.top

const double = x => x * 2;
来源：http://gpx.ywan-chungtsiang.top

[U95] JS：Promise 包装
来源：http://bsh.bjfxy.top

new Promise((resolve, reject) => {})
来源：http://zfw.yj202588.top

[U96] JS：async/await 与异常
来源：http://tbw.shzxlz.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ict.9152youxi.cn

[U97] JS：并发请求
来源：http://aqi.yongpay.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://myf.yvedp.cn

[U98] JS：fetch 带 JSON
来源：http://yks.ivvv.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://yaj.zhaomingkeji.xyz

[U99] JS：事件监听
来源：http://pza.iojbl.cn

el.addEventListener("click", e => {})
来源：http://uwx.xylfe.cn

[U100] JS：DOM 查询
来源：http://dgk.nanxinkj.top

document.querySelector(".item")
来源：http://wmc.quarkkingdee.top

[U101] JS：classList 操作
来源：http://eoz.shzxlz.cn

el.classList.toggle("active")
来源：http://tka.c1oappe.top

[U102] JS：本地存储
来源：http://pqm.svipenyu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://hwj.bbcook.cn

[U103] JS：定时器
来源：http://olb.tianlin.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mjq.xylfe.cn

[U104] JS：防抖
来源：http://bxz.hnqzz.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fde.dashuyun.cn

[U105] JS：节流
来源：http://iqp.hammf.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vsw.fehbvm.com

[U106] JS：日期格式化
来源：http://fgg.hongshengwenyu.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ebn.zhixingplan.top

[U107] JS：数字千分位
来源：http://wso.yj20258888.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://omk.snrcjt.cn

[U108] JS：随机整数
来源：http://kja.fengsongda.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rhr.tian-w.cn

[U109] JS：数组分组
来源：http://yer.9152youxi.cn

Object.groupBy(arr, x => x.type)
来源：http://syj.yvedp.cn

[U110] JS：数组分块
来源：http://hrz.jinghuilouyu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vsk.zhijiandao.cn

[U111] JS：对象转 Map
来源：http://uhl.yonumen.top

new Map(Object.entries(obj))
来源：http://lia.zhengqikj.top

[U112] JS：字符串补位
来源：http://rsp.gzhubu.top

"7".padStart(3, "0")
来源：http://fkj.daxiang520.top

[U113] JS：正则替换全部
来源：http://uwa.wangshuangyany.cn

s.replaceAll("a", "b")
来源：http://ohb.zhijiandao.cn

[U114] JS：JSON 深比较
来源：http://vqq.sjlbkw.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ary.ivvv.top

[U115] JS：生成 UUID
来源：http://eyu.cucudq.cn

crypto.randomUUID()
来源：http://xbi.aizwys.cn

[U116] JS：类型检查（JSDoc）
来源：http://eau.hammf.cn

/** @param {string} name */ function f(name) {}
来源：http://ndk.meibo888.top

[U117] JS：单元测试
来源：http://ipf.guannengcc.top

npm i -D vitest;  npx vitest
来源：http://irv.hnxiangtu.top

[U118] JS：开发服务器
来源：http://qyj.316326.xyz

npm i -D vite;  npx vite
来源：http://joj.jqgufenzy.top


<!-- 参考信息 -->