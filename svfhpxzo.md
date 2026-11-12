代发 wailian999

[T33] Lua：表（数组）
来源：http://ssb.bbcook.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://qfn.xinyue.icu

[T34] Lua：遍历表
来源：http://liu.snrcjt.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://tlu.birdmap.top

[T35] Lua：字典表
来源：http://qyn.yuanzhike.top

local d = { a = 1 };  d.b = 2
来源：http://mjg.wangdashe.top

[T36] Lua：函数
来源：http://qbe.jqgufenzy.top

function add(a, b) return a + b end
来源：http://axb.quarkkingdee.top

[T37] Lua：字符串拼接
来源：http://yno.cashguo.top

"a" .. "b"
来源：http://khi.yonumen.top

[T38] Lua：条件
来源：http://gem.ehwqpu.com

if x > 0 then print("正") end
来源：http://yeq.0kj1m.cn

[T39] Lua：模式匹配
来源：http://dzy.zycfv.cn

string.find(s, "%d+")
来源：http://ylw.jiagoushi.top

[T40] Lua：元表
来源：http://hnl.chenzaomai.com

setmetatable({}, { __index = base })
来源：http://goi.xinyue.icu

[T41] Perl：Hello World
来源：http://cvf.guannengcc.top

print "Hello\n";
来源：http://nej.shanyushiyangkeji.top

[T42] Perl：变量类型
来源：http://gmt.epnwcf.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lpm.ydjk.org.cn

[T43] Perl：字符串插值
来源：http://nfs.zhixingplan.top

"值: $a"
来源：http://lfr.ctjpmb.com

[T44] Perl：条件
来源：http://krn.sufxvd.cn

if ($a > 0) { print "正"; }
来源：http://wky.ehwqpu.com

[T45] Perl：数组遍历
来源：http://xhh.svipenyu.cn

for my $x (@arr) { print $x; }
来源：http://ove.andypj.xyz

[T46] Perl：哈希操作
来源：http://myj.smart0.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nwx.fzhhl.top

[T47] Perl：正则捕获
来源：http://chr.zhijiandao.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ttc.bjfxy.top

[T48] Perl：正则替换
来源：http://cwx.jlsjyb.cn

$s =~ s/old/new/g;
来源：http://rok.dashuyun.cn

[T49] Perl：函数
来源：http://vxd.iojbl.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nzy.cucudq.cn

[T50] Perl：逐行读文件
来源：http://qsy.guowangkeji.top

open my $fh, "<", "a.txt" or die $!;
来源：http://yrn.xuetiantiany.cn

while (my $line = <$fh>) { print $line; }
来源：http://jss.hfpthk.cn

[T51] Scala：Hello World
来源：http://eoz.pycfn.com

println("Hello")
来源：http://xrm.zhixingplan.top

[T52] Scala：变量
来源：http://tyz.svipenyu.cn

val a = 1;  var b = 2
来源：http://hym.ivvv.top

[T53] Scala：字符串插值
来源：http://jfb.tarul.cn

s"值: $b"
来源：http://zwm.dashuyun.cn

[T54] Scala：集合映射
来源：http://osj.hcnkem.com

List(1, 2, 3).map(_ * 2)
来源：http://lze.pengpengdd.cyou

[T55] Scala：集合过滤
来源：http://oyp.bjfxy.top

List(1, 2, 3).filter(_ > 1)
来源：http://idr.yj20258.top

[T56] Scala：样例类
来源：http://swc.pengpengdd.cyou

case class User(name: String, age: Int)
来源：http://uve.chenzaomai.com

[T57] Scala：模式匹配
来源：http://qju.yangfankeji.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://ugj.jianghu66.top

[T58] Scala：函数定义
来源：http://dwk.epnwcf.com

def add(a: Int, b: Int): Int = a + b
来源：http://xat.zhaomingkeji.xyz

[T59] Scala：循环
来源：http://knx.hywenlv.cn

for (i <- 1 to 10) println(i)
来源：http://wyc.cheryme.top

[T60] Scala：折叠
来源：http://rvd.vehdjk.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qmr.vqdsnc.cn

================================================================================
来源：http://cbj.tianlin.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://obb.xinyue.icu

================================================================================
来源：http://sbr.quarkkingdee.top

[U01] Py：创建虚拟环境
来源：http://ldj.zhiwuduotai.top

python -m venv .venv && source .venv/bin/activate
来源：http://spk.pycfn.com

[U02] Py：导出 / 安装依赖
来源：http://oyw.ywan-chungtsiang.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://uhj.0kj1m.cn

[U03] Py：加载 .env 配置
来源：http://joh.gogol.net.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://qdr.hcnkem.com

[U04] Py：变量调试打印
来源：http://abx.hfpthk.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://eyh.yj20258888.top

[U05] Py：列表去重且保序
来源：http://ygb.tanke756.top

list(dict.fromkeys(arr))
来源：http://oug.nwbrower.top

[U06] Py：合并两个字典
来源：http://tor.316326.xyz

{**a, **b}
来源：http://aeh.fehbvm.com

[U07] Py：反转字典键值
来源：http://chb.yuxming.cn

{v: k for k, v in d.items()}
来源：http://umi.chenzaomai.com

[U08] Py：展平二维列表
来源：http://dai.yj202588.top

[y for x in nested for y in x]
来源：http://yzr.fzhhl.top

[U09] Py：字典取最大值的键
来源：http://sui.redwolf501.top

max(d, key=d.get)
来源：http://jzc.fktsv.cn

[U10] Py：按值排序字典
来源：http://axw.pycfn.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gjp.epnwcf.com

[U11] Py：生成器表达式
来源：http://jqn.aibaodan.cn

(x * 2 for x in arr)
来源：http://jhf.wangdashe.top

[U12] Py：取出现最多的 3 个元素
来源：http://laf.birdmap.top

Counter(arr).most_common(3)
来源：http://udv.smart0.xyz

[U13] Py：固定长度队列
来源：http://uyq.316326.xyz

deque(maxlen=10)
来源：http://pec.jinyuanbaomall.cn

[U14] Py：分组收集到列表
来源：http://rhr.fengsongda.top

defaultdict(list)
来源：http://qad.xuetiantiany.cn

[U15] Py：高精度计时
来源：http://mfj.xylfe.cn

t = time.perf_counter()
来源：http://eoi.shanyushiyangkeji.top

[U16] Py：命令行参数解析
来源：http://heu.fengsongda.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zqk.xuetiantiany.cn

[U17] Py：初始化日志
来源：http://vvc.yj20258888.top

logging.basicConfig(level=logging.INFO)
来源：http://orc.bjfxy.top

[U18] Py：预编译正则
来源：http://akt.jqgufenzy.top

pat = re.compile(r"\d+")
来源：http://sew.jqgfzy.top

[U19] Py：正则替换带回调
来源：http://oqp.ppjwa.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rza.sjlbkw.cn

[U20] Py：缓存函数结果
来源：http://fxn.yueranfly.top

@functools.lru_cache(maxsize=None)
来源：http://xsb.xuanzx.com

[U21] Py：自定义上下文管理器
来源：http://mcz.kuanghao11.cn

@contextlib.contextmanager
来源：http://ccg.sysykeji.top

[U22] Py：矩阵转置
来源：http://jpe.yongpay.top

list(zip(*m))
来源：http://hzx.fanxiaobao.xyz

[U23] Py：分块读取大文件
来源：http://dak.uphjek.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://kba.fanxiaobao.xyz

[U24] Py：路径操作
来源：http://wmv.jqgfzy.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qmm.zhiwuduotai.top

[U25] Py：CSV 按字典读
来源：http://ccp.zdbjq.cn

csv.DictReader(f)
来源：http://clr.birdmap.top

[U26] Py：并发下载
来源：http://mol.cashguo.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rea.gaohongyu789.top

[U27] Py：异步 HTTP
来源：http://gsc.yj20258888.top

aiohttp.ClientSession() 配合 async with
来源：http://svz.316326.xyz

[U28] Py：类型别名
来源：http://vbq.andypj.xyz

UserId = int
来源：http://kgk.snrcjt.cn

[U29] Py：属性校验
来源：http://hxu.aibaodan.cn

@property 与 @x.setter 配合
来源：http://agt.aizwys.cn

[U30] Py：数据类
来源：http://dhh.xingfuxueyuan.xyz

@dataclass(slots=True)
来源：http://bxg.daria6918.cn

[U31] Py：单测
来源：http://ygq.tian-w.cn

python -m pytest -q
来源：http://rei.shanyushiyangkeji.top

[U32] Py：代码格式化
来源：http://gqr.snrcjt.cn

ruff format . && ruff check --fix .
来源：http://nho.ctjpmb.com

[U33] Py：打包发布
来源：http://umz.jinghuilouyu.cn

python -m build  （依赖 pyproject.toml）
来源：http://kio.fengsongda.top

[U34] Py：判断编码
来源：http://jhj.ctjpmb.com

chardet.detect(raw)
来源：http://eyz.yonumen.top

[U35] Py：发送邮件
来源：http://cqy.hfpthk.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qcb.zhoulong.xyz

[U36] Py：定时任务
来源：http://rao.sweek.top

schedule.every(10).minutes.do(job)
来源：http://lwg.0kj1m.cn

[U37] Py：读写 Excel
来源：http://zmc.ctjpmb.com

pandas.read_excel / DataFrame.to_excel
来源：http://vdn.wangdashe.top

[U38] Py：获取脚本所在目录
来源：http://ktv.xuetiantiany.cn

Path(__file__).resolve().parent
来源：http://yhk.yvedp.cn

[U39] Py：判断是否在交互环境
来源：http://hks.hywenlv.cn

sys.stdout.isatty()
来源：http://taw.quarkkingdee.top

[U40] Py：打印到标准错误
来源：http://rus.gaohongyu789.top

print("err", file=sys.stderr)
来源：http://zli.zdqjudy.top

[U41] PHP：初始化 Composer 项目
来源：http://pso.sufxvd.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://zwt.jiagoushi.top

[U42] PHP：PSR-4 自动加载
来源：http://cgy.wangshuangyany.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tep.nanxinkj.top

[U43] PHP：声明命名空间
来源：http://rkd.hcnkem.com

namespace App\Http;
来源：http://kvv.ivvv.top

[U44] PHP：开启严格类型
来源：http://tkt.316326.xyz

declare(strict_types=1);
来源：http://qzp.bbcook.cn

[U45] PHP：类型声明与返回类型
来源：http://qfq.shanyushiyangtech.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://lew.redwolf501.top

[U46] PHP：可空类型
来源：http://nti.nwbrower.top

?string $name = null
来源：http://buh.xinyue.icu

[U47] PHP：联合类型
来源：http://lua.hysaishi.cn

int|string $id
来源：http://sap.birdmap.top

[U48] PHP：纯枚举
来源：http://qgi.xylfe.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zty.tarul.cn

[U49] PHP：只读属性
来源：http://yiq.chenlongwang.top

public readonly string $name
来源：http://tlg.shanyushiyangtech.top

[U50] PHP：构造器属性提升
来源：http://pyd.daxiang520.top

public function __construct(private int $id) {}
来源：http://iuc.zhijiandao.cn

[U51] PHP：数组解构
来源：http://eoz.hesvh.cn

[$a, $b] = $arr;
来源：http://vof.xuanzx.com

[U52] PHP：箭头函数
来源：http://vnj.zhoulong.xyz

$double = fn($x) => $x * 2;
来源：http://ezm.bbcook.cn

[U53] PHP：空合并运算符
来源：http://kck.wangshuangyany.cn

$v = $a ?? $b ?? "default";
来源：http://fxm.zdbjq.cn

[U54] PHP：空安全调用
来源：http://rbh.xziqi.cn

$obj?->method()
来源：http://rlu.jiagoushi.top

[U55] PHP：match 表达式
来源：http://xpq.52xcode.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lrf.fehbvm.com

[U56] PHP：命名参数
来源：http://vad.shangyingyoupin.top

f(a: 1, b: 2)
来源：http://ier.zhengqikj.top

[U57] PHP：字符串插值
来源：http://tie.hongshengwenyu.top

"值: {$a}"
来源：http://ird.fengsongda.top

[U58] PHP：数组三件套
来源：http://fob.chenlongwang.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nxg.gzhubu.top

[U59] PHP：自定义排序
来源：http://rlp.daxiang520.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mag.yueranfly.top

[U60] PHP：JSON 编解码
来源：http://wrz.vqdsnc.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xgg.yueranfly.top

[U61] PHP：正则
来源：http://ard.jinqigfzy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jsz.cheryme.top

[U62] PHP：日期对象
来源：http://yyp.zycfv.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://tdx.dianchejie.cn

[U63] PHP：文件读写
来源：http://vex.tanke756.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bpr.wangdashe.top

[U64] PHP：目录遍历
来源：http://vvz.yangfankeji.com

glob("dir/*.php");  scandir("dir");
来源：http://yee.aibaodan.cn

[U65] PHP：会话
来源：http://zds.ywan-chungtsiang.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ojh.gotoacloud.top

[U66] PHP：设置 Cookie
来源：http://tya.sufxvd.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://yqq.shanyushiyangtech.top

[U67] PHP：处理文件上传
来源：http://kzy.fzhhl.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qfr.tarul.cn

[U68] PHP：PDO 连接
来源：http://aif.pengpengdd.cyou

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://luw.zhengqikj.top

[U69] PHP：PDO 预处理
来源：http://cvb.zhixingplan.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://txc.yj202588.top

[U70] PHP：PDO 事务
来源：http://kiu.gzhubu.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ieq.xinyue.icu

[U71] PHP：抛出异常
来源：http://kbk.jqgufenzy.top

throw new RuntimeException("失败", 500);
来源：http://rfw.havefunace.top

[U72] PHP：写错误日志
来源：http://ryz.hysaishi.cn

error_log("失败: " . $e->getMessage());
来源：http://loz.bbcook.cn

[U73] PHP：读取 ini 配置
来源：http://nje.chenzaomai.com

parse_ini_file("config.ini", true)
来源：http://dsm.gotoacloud.top

[U74] PHP：读取环境变量
来源：http://brh.ctjpmb.com

getenv("APP_ENV") ?: "production"
来源：http://zcx.fzhhl.top

[U75] PHP：依赖注入
来源：http://mqm.ydjk.org.cn

composer require psr/container
来源：http://oxc.hongshengwenyu.top

[U76] PHP：简单路由
来源：http://iow.ybcxt.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kgg.mhx1999.top

[U77] PHP：模板渲染
来源：http://rux.vehdjk.com

composer require twig/twig
来源：http://ngx.snrcjt.cn

[U78] PHP：单元测试
来源：http://due.yuxming.cn

composer require --dev phpunit/phpunit
来源：http://xgj.dianchejie.cn

[U79] PHP：静态分析
来源：http://fdi.gaohongyu789.top

composer require --dev phpstan/phpstan
来源：http://xqm.smart0.xyz

[U80] PHP：代码规范修复
来源：http://swy.iojbl.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://mjm.aizwys.cn

[U81] JS：初始化项目
来源：http://wjn.sweek.top

npm init -y;  npm i express
来源：http://ged.c1oappe.top

[U82] JS：package.json 脚本
来源：http://tdz.ivvv.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://dwt.sysykeji.top

[U83] JS：ES Module 导入导出
来源：http://nvy.52xcode.cn

export const a = 1;  import { a } from "./m.js";
来源：http://bgy.quarkkingdee.top

[U84] JS：CommonJS 写法
来源：http://eyd.ydjk.org.cn

module.exports = { a };  const { a } = require("./m");
来源：http://nnc.ivvv.top

[U85] JS：可选链
来源：http://ptx.guannengcc.top

a?.b?.c
来源：http://kxs.yongpay.top

[U86] JS：空值合并
来源：http://gqr.yonumen.top

a ?? b
来源：http://cdu.cqqwz.cn

[U87] JS：解构默认值
来源：http://bod.hfpthk.cn

const { a = 1, b = 2 } = obj;
来源：http://xlr.tianlin.xyz

[U88] JS：对象展开合并
来源：http://hlv.9152youxi.cn

{ ...a, ...b }
来源：http://xzl.cashguo.top

[U89] JS：数组去重
来源：http://qfq.ppjwa.cn

[...new Set(arr)]
来源：http://kcs.jqgfzy.top

[U90] JS：数字数组排序
来源：http://llu.hcnkem.com

[...arr].sort((a, b) => a - b)
来源：http://wss.zdbjq.cn

[U91] JS：对象键值遍历
来源：http://mvl.yfazqb.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ldv.fktsv.cn

[U92] JS：深拷贝
来源：http://wnq.zdbjq.cn

structuredClone(obj)
来源：http://bkk.yj202588.top

[U93] JS：模板字符串
来源：http://gda.zhijiandao.cn

`共 ${n} 条`
来源：http://yjc.ydjk.org.cn

[U94] JS：箭头函数
来源：http://bhj.svipenyu.cn

const double = x => x * 2;
来源：http://jpe.c1oappe.top

[U95] JS：Promise 包装
来源：http://lcp.nanxuanxn.top

new Promise((resolve, reject) => {})
来源：http://mga.sysykeji.top

[U96] JS：async/await 与异常
来源：http://syj.gzhubu.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hjt.ywan-chungtsiang.top

[U97] JS：并发请求
来源：http://kls.snrcjt.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://jsr.daria6918.cn

[U98] JS：fetch 带 JSON
来源：http://hkv.hammf.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hyu.chenlongwang.top

[U99] JS：事件监听
来源：http://dtu.jianghu66.top

el.addEventListener("click", e => {})
来源：http://rqr.sxryk.cn

[U100] JS：DOM 查询
来源：http://fwn.9152youxi.cn

document.querySelector(".item")
来源：http://brp.zhongyouzk.top

[U101] JS：classList 操作
来源：http://lra.c1oappe.top

el.classList.toggle("active")
来源：http://zue.meibo888.top

[U102] JS：本地存储
来源：http://akx.cashguo.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://brl.yangfankeji.com

[U103] JS：定时器
来源：http://bjm.316326.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hyd.jianghu66.top

[U104] JS：防抖
来源：http://qkg.chenzaomai.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ftz.redwolf501.top

[U105] JS：节流
来源：http://zic.tanke756.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://smd.uphjek.com

[U106] JS：日期格式化
来源：http://guq.hnxiangtu.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qme.zhongyouzk.top

[U107] JS：数字千分位
来源：http://skm.hywenlv.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://uqv.iojbl.cn

[U108] JS：随机整数
来源：http://rwy.yfazqb.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ito.sufxvd.cn

[U109] JS：数组分组
来源：http://yis.zhixingplan.top

Object.groupBy(arr, x => x.type)
来源：http://ixs.vehdjk.com

[U110] JS：数组分块
来源：http://zfp.dashuyun.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tcy.feifeiyinyue.top

[U111] JS：对象转 Map
来源：http://nap.jqgfzy.top

new Map(Object.entries(obj))
来源：http://lae.hnxiangtu.top

[U112] JS：字符串补位
来源：http://ngx.bjfxy.top

"7".padStart(3, "0")
来源：http://uza.yuanzhike.top

[U113] JS：正则替换全部
来源：http://axm.jiagoushi.top

s.replaceAll("a", "b")
来源：http://ums.yj20258888.top

[U114] JS：JSON 深比较
来源：http://qma.c1oappe.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://qpq.aizwys.cn

[U115] JS：生成 UUID
来源：http://xqo.zhoulong.xyz

crypto.randomUUID()
来源：http://vdx.nanxuanxn.top

[U116] JS：类型检查（JSDoc）
来源：http://aby.jinyuanbaomall.cn

/** @param {string} name */ function f(name) {}
来源：http://pht.guannengcc.top

[U117] JS：单元测试
来源：http://quf.zhaomingkeji.xyz

npm i -D vitest;  npx vitest
来源：http://dta.meibo888.top

[U118] JS：开发服务器
来源：http://qjp.vehdjk.com

npm i -D vite;  npx vite
来源：http://unk.cdnleiting.top

[U119] JS：生产构建
来源：http://jfs.iojbl.cn

npx vite build
来源：http://sbi.hcnkem.com

[U120] JS：读取环境变量（Vite）
来源：http://kbu.epnwcf.com

import.meta.env.VITE_API_URL
来源：http://esl.wangdashe.top


<!-- 参考信息 -->