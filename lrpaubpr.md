代发 wailian999

[T31] Lua：Hello World
来源：http://pgr.dashuyun.cn

print("Hello")
来源：http://swg.tian-w.cn

[T32] Lua：局部变量
来源：http://pta.sufxvd.cn

local a = 1
来源：http://ljo.cqqwz.cn

[T33] Lua：表（数组）
来源：http://miw.yangfankeji.com

local t = {1, 2, 3};  t[4] = 4
来源：http://vzc.fengsongda.top

[T34] Lua：遍历表
来源：http://kas.svipenyu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://owq.xuetiantiany.cn

[T35] Lua：字典表
来源：http://eaa.sweek.top

local d = { a = 1 };  d.b = 2
来源：http://wql.gzhubu.top

[T36] Lua：函数
来源：http://mzq.aizwys.cn

function add(a, b) return a + b end
来源：http://gkg.gotoacloud.top

[T37] Lua：字符串拼接
来源：http://dzc.yuanzhike.top

"a" .. "b"
来源：http://eoq.xuanzx.com

[T38] Lua：条件
来源：http://yxi.hnxiangtu.top

if x > 0 then print("正") end
来源：http://frr.jinyuanbaomall.cn

[T39] Lua：模式匹配
来源：http://lut.hywenlv.cn

string.find(s, "%d+")
来源：http://gyv.fktsv.cn

[T40] Lua：元表
来源：http://vue.zhaomingkeji.xyz

setmetatable({}, { __index = base })
来源：http://foa.gaohongyu789.top

[T41] Perl：Hello World
来源：http://ubp.jinqigufen.top

print "Hello\n";
来源：http://evd.xinyue.icu

[T42] Perl：变量类型
来源：http://ynv.hammf.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ygl.epnwcf.com

[T43] Perl：字符串插值
来源：http://snx.yj20258.top

"值: $a"
来源：http://ntt.aizwys.cn

[T44] Perl：条件
来源：http://zrk.nanxuanxn.top

if ($a > 0) { print "正"; }
来源：http://sog.cheryme.top

[T45] Perl：数组遍历
来源：http://yrs.gotoacloud.top

for my $x (@arr) { print $x; }
来源：http://qbx.zdbjq.cn

[T46] Perl：哈希操作
来源：http://tzz.smart0.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cxg.ydjk.org.cn

[T47] Perl：正则捕获
来源：http://vjg.hesvh.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://grj.yuanzhike.top

[T48] Perl：正则替换
来源：http://hka.gaohongyu789.top

$s =~ s/old/new/g;
来源：http://zla.shanyushiyangtech.top

[T49] Perl：函数
来源：http://sdf.gogol.net.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yse.jqgufenzy.top

[T50] Perl：逐行读文件
来源：http://ogl.gaohongyu789.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ovv.pycfn.com

while (my $line = <$fh>) { print $line; }
来源：http://efe.bbcook.cn

[T51] Scala：Hello World
来源：http://exm.vqdsnc.cn

println("Hello")
来源：http://tlh.tarul.cn

[T52] Scala：变量
来源：http://tzm.zhijiandao.cn

val a = 1;  var b = 2
来源：http://vxd.yueranfly.top

[T53] Scala：字符串插值
来源：http://qcb.cqqwz.cn

s"值: $b"
来源：http://vkd.zdqjudy.top

[T54] Scala：集合映射
来源：http://ibc.svipenyu.cn

List(1, 2, 3).map(_ * 2)
来源：http://jwj.0kj1m.cn

[T55] Scala：集合过滤
来源：http://kqi.zdqjudy.top

List(1, 2, 3).filter(_ > 1)
来源：http://bbm.shuidangran.top

[T56] Scala：样例类
来源：http://ppg.shangyingyoupin.top

case class User(name: String, age: Int)
来源：http://zdl.9152youxi.cn

[T57] Scala：模式匹配
来源：http://znx.jiagoushi.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://eua.ivvv.top

[T58] Scala：函数定义
来源：http://jwg.sjlbkw.cn

def add(a: Int, b: Int): Int = a + b
来源：http://aqn.zycfv.cn

[T59] Scala：循环
来源：http://cvd.wangshuangyany.cn

for (i <- 1 to 10) println(i)
来源：http://zvg.svipenyu.cn

[T60] Scala：折叠
来源：http://tgn.xziqi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://muv.xylfe.cn

================================================================================
来源：http://hyl.meibo888.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dtz.yj20258888.top

================================================================================
来源：http://ecg.cqqwz.cn

[U01] Py：创建虚拟环境
来源：http://icg.ywan-chungtsiang.top

python -m venv .venv && source .venv/bin/activate
来源：http://aoq.redwolf501.top

[U02] Py：导出 / 安装依赖
来源：http://tvm.cucudq.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://exe.sysykeji.top

[U03] Py：加载 .env 配置
来源：http://yjx.uphjek.com

from dotenv import load_dotenv; load_dotenv()
来源：http://iht.epnwcf.com

[U04] Py：变量调试打印
来源：http://uxs.ivvv.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://spy.cucudq.cn

[U05] Py：列表去重且保序
来源：http://enu.sxryk.cn

list(dict.fromkeys(arr))
来源：http://nqa.epnwcf.com

[U06] Py：合并两个字典
来源：http://iow.bbcook.cn

{**a, **b}
来源：http://ppp.yuanzhike.top

[U07] Py：反转字典键值
来源：http://sqi.hywenlv.cn

{v: k for k, v in d.items()}
来源：http://lbk.cqqwz.cn

[U08] Py：展平二维列表
来源：http://fia.quarkkingdee.top

[y for x in nested for y in x]
来源：http://hls.guowangkeji.top

[U09] Py：字典取最大值的键
来源：http://nqu.jiagoushi.top

max(d, key=d.get)
来源：http://mvp.shanyushiyangtech.top

[U10] Py：按值排序字典
来源：http://vqi.hfpthk.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xnq.fehbvm.com

[U11] Py：生成器表达式
来源：http://hlw.ydzc1.top

(x * 2 for x in arr)
来源：http://iof.jinqigufen.top

[U12] Py：取出现最多的 3 个元素
来源：http://cgr.yueranfly.top

Counter(arr).most_common(3)
来源：http://oxu.chenlongwang.top

[U13] Py：固定长度队列
来源：http://ief.guannengcc.top

deque(maxlen=10)
来源：http://xaj.chenzaomai.com

[U14] Py：分组收集到列表
来源：http://koj.uphjek.com

defaultdict(list)
来源：http://qzk.iojbl.cn

[U15] Py：高精度计时
来源：http://law.zhijiandao.cn

t = time.perf_counter()
来源：http://lts.cucudq.cn

[U16] Py：命令行参数解析
来源：http://rho.316326.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ysq.yj20258888.top

[U17] Py：初始化日志
来源：http://xzl.316326.xyz

logging.basicConfig(level=logging.INFO)
来源：http://ogc.ydzc1.top

[U18] Py：预编译正则
来源：http://jpo.yj20258888.top

pat = re.compile(r"\d+")
来源：http://kot.ydzc1.top

[U19] Py：正则替换带回调
来源：http://nkl.jinghuilouyu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://luu.zdbjq.cn

[U20] Py：缓存函数结果
来源：http://lil.sysykeji.top

@functools.lru_cache(maxsize=None)
来源：http://mda.iojbl.cn

[U21] Py：自定义上下文管理器
来源：http://fdc.zdbjq.cn

@contextlib.contextmanager
来源：http://kpl.hcnkem.com

[U22] Py：矩阵转置
来源：http://ysb.shanyushiyangtech.top

list(zip(*m))
来源：http://brk.sufxvd.cn

[U23] Py：分块读取大文件
来源：http://tqo.shanyushiyangkeji.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://slt.zdbjq.cn

[U24] Py：路径操作
来源：http://ewz.fengsongda.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://kqc.hnqzz.top

[U25] Py：CSV 按字典读
来源：http://nwo.sjlbkw.cn

csv.DictReader(f)
来源：http://jlh.daria6918.cn

[U26] Py：并发下载
来源：http://pzq.quarkkingdee.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jxd.redwolf501.top

[U27] Py：异步 HTTP
来源：http://kuw.gogol.net.cn

aiohttp.ClientSession() 配合 async with
来源：http://nyk.quarkkingdee.top

[U28] Py：类型别名
来源：http://myl.zhengqikj.top

UserId = int
来源：http://yvs.vehdjk.com

[U29] Py：属性校验
来源：http://dtd.guannengcc.top

@property 与 @x.setter 配合
来源：http://yzl.gaohongyu789.top

[U30] Py：数据类
来源：http://kae.yuxming.cn

@dataclass(slots=True)
来源：http://mrq.fzhhl.top

[U31] Py：单测
来源：http://znp.zhoulong.xyz

python -m pytest -q
来源：http://sku.gogol.net.cn

[U32] Py：代码格式化
来源：http://zwo.0kj1m.cn

ruff format . && ruff check --fix .
来源：http://hgp.andypj.xyz

[U33] Py：打包发布
来源：http://gnu.jinyuanbaomall.cn

python -m build  （依赖 pyproject.toml）
来源：http://iqv.zhixingplan.top

[U34] Py：判断编码
来源：http://wxj.gzhubu.top

chardet.detect(raw)
来源：http://sdk.aibaodan.cn

[U35] Py：发送邮件
来源：http://ftj.vehdjk.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://uuo.cashguo.top

[U36] Py：定时任务
来源：http://aip.yj20258.top

schedule.every(10).minutes.do(job)
来源：http://yoa.yfazqb.com

[U37] Py：读写 Excel
来源：http://ual.zhoulong.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://aqc.feifeiyinyue.top

[U38] Py：获取脚本所在目录
来源：http://rgh.yvedp.cn

Path(__file__).resolve().parent
来源：http://ubu.guowangkeji.top

[U39] Py：判断是否在交互环境
来源：http://dlf.hywenlv.cn

sys.stdout.isatty()
来源：http://egh.smart0.xyz

[U40] Py：打印到标准错误
来源：http://rnl.gaohongyu789.top

print("err", file=sys.stderr)
来源：http://gkn.zdqjudy.top

[U41] PHP：初始化 Composer 项目
来源：http://ijr.ivvv.top

composer init;  composer require guzzlehttp/guzzle
来源：http://brr.gotoacloud.top

[U42] PHP：PSR-4 自动加载
来源：http://kjv.tarul.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cpr.sweek.top

[U43] PHP：声明命名空间
来源：http://mrg.chenlongwang.top

namespace App\Http;
来源：http://fbo.52xcode.cn

[U44] PHP：开启严格类型
来源：http://abm.zhoulong.xyz

declare(strict_types=1);
来源：http://pio.yongpay.top

[U45] PHP：类型声明与返回类型
来源：http://txd.shangyingyoupin.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://byg.yuxming.cn

[U46] PHP：可空类型
来源：http://raa.nanxuanxn.top

?string $name = null
来源：http://fom.xinyue.icu

[U47] PHP：联合类型
来源：http://ofi.jianghu66.top

int|string $id
来源：http://hnq.tian-w.cn

[U48] PHP：纯枚举
来源：http://wvv.tanke756.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ngl.jyoumei.cn

[U49] PHP：只读属性
来源：http://cjy.kuanghao11.cn

public readonly string $name
来源：http://mhy.hfpthk.cn

[U50] PHP：构造器属性提升
来源：http://fac.iojbl.cn

public function __construct(private int $id) {}
来源：http://sty.birdmap.top

[U51] PHP：数组解构
来源：http://ucw.mhx1999.top

[$a, $b] = $arr;
来源：http://vox.dashuyun.cn

[U52] PHP：箭头函数
来源：http://wns.cashguo.top

$double = fn($x) => $x * 2;
来源：http://opw.fktsv.cn

[U53] PHP：空合并运算符
来源：http://kyu.ppjwa.cn

$v = $a ?? $b ?? "default";
来源：http://oci.dianchejie.cn

[U54] PHP：空安全调用
来源：http://gzn.cheryme.top

$obj?->method()
来源：http://czv.52xcode.cn

[U55] PHP：match 表达式
来源：http://ctc.redwolf501.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://onh.guannengcc.top

[U56] PHP：命名参数
来源：http://svk.yangfankeji.com

f(a: 1, b: 2)
来源：http://gua.aizwys.cn

[U57] PHP：字符串插值
来源：http://huu.yueranfly.top

"值: {$a}"
来源：http://pab.jlsjyb.cn

[U58] PHP：数组三件套
来源：http://crx.cashguo.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hhx.nwbrower.top

[U59] PHP：自定义排序
来源：http://dqi.xinyue.icu

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uah.yuanzhike.top

[U60] PHP：JSON 编解码
来源：http://niv.gaohongyu789.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qqn.zycfv.cn

[U61] PHP：正则
来源：http://qhq.gzhubu.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zza.jinqigfzy.top

[U62] PHP：日期对象
来源：http://xsr.shanyushiyangkeji.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ujr.bjfxy.top

[U63] PHP：文件读写
来源：http://clg.hysaishi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://luz.ydzc1.top

[U64] PHP：目录遍历
来源：http://fdh.cheryme.top

glob("dir/*.php");  scandir("dir");
来源：http://zeb.shuidangran.top

[U65] PHP：会话
来源：http://csh.nanxuanxn.top

session_start();  $_SESSION["uid"] = 1;
来源：http://kgx.ivvv.top

[U66] PHP：设置 Cookie
来源：http://zoo.zdbjq.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://npg.dianchejie.cn

[U67] PHP：处理文件上传
来源：http://ewd.mhx1999.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://srr.aibaodan.cn

[U68] PHP：PDO 连接
来源：http://lxa.jyoumei.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hju.c1oappe.top

[U69] PHP：PDO 预处理
来源：http://jan.cucudq.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://emk.shangyingyoupin.top

[U70] PHP：PDO 事务
来源：http://all.tanke756.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://myd.bjfxy.top

[U71] PHP：抛出异常
来源：http://yzs.tarul.cn

throw new RuntimeException("失败", 500);
来源：http://xvp.316326.xyz

[U72] PHP：写错误日志
来源：http://zwi.sweek.top

error_log("失败: " . $e->getMessage());
来源：http://jwc.sweek.top

[U73] PHP：读取 ini 配置
来源：http://ajz.wangdashe.top

parse_ini_file("config.ini", true)
来源：http://jzn.iojbl.cn

[U74] PHP：读取环境变量
来源：http://hkx.tarul.cn

getenv("APP_ENV") ?: "production"
来源：http://ezb.quarkkingdee.top

[U75] PHP：依赖注入
来源：http://czi.jqgfzy.top

composer require psr/container
来源：http://frm.hnxiangtu.top

[U76] PHP：简单路由
来源：http://tfu.smart0.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zou.pycfn.com

[U77] PHP：模板渲染
来源：http://fyy.zdbjq.cn

composer require twig/twig
来源：http://hlp.vehdjk.com

[U78] PHP：单元测试
来源：http://vzy.yj20258.top

composer require --dev phpunit/phpunit
来源：http://dbh.ydjk.org.cn

[U79] PHP：静态分析
来源：http://sdz.hammf.cn

composer require --dev phpstan/phpstan
来源：http://uml.ivvv.top

[U80] PHP：代码规范修复
来源：http://znl.sufxvd.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://xeg.kuanghao11.cn

[U81] JS：初始化项目
来源：http://lvz.jqgfzy.top

npm init -y;  npm i express
来源：http://fji.shuidangran.top

[U82] JS：package.json 脚本
来源：http://ksv.fanxiaobao.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lmt.0kj1m.cn

[U83] JS：ES Module 导入导出
来源：http://ckd.shzxlz.cn

export const a = 1;  import { a } from "./m.js";
来源：http://par.xylfe.cn

[U84] JS：CommonJS 写法
来源：http://qjc.yj202588.top

module.exports = { a };  const { a } = require("./m");
来源：http://oru.zhiwuduotai.top

[U85] JS：可选链
来源：http://wkr.jqgufenzy.top

a?.b?.c
来源：http://qsu.hongshengwenyu.top

[U86] JS：空值合并
来源：http://zdp.shzxlz.cn

a ?? b
来源：http://ykm.jyoumei.cn

[U87] JS：解构默认值
来源：http://qyn.hcnkem.com

const { a = 1, b = 2 } = obj;
来源：http://ipp.guowangkeji.top

[U88] JS：对象展开合并
来源：http://eyi.ivvv.top

{ ...a, ...b }
来源：http://nzs.xinyue.icu

[U89] JS：数组去重
来源：http://fvn.zhengqikj.top

[...new Set(arr)]
来源：http://afj.hcnkem.com

[U90] JS：数字数组排序
来源：http://cho.redwolf501.top

[...arr].sort((a, b) => a - b)
来源：http://rqc.yanxiufei.cn

[U91] JS：对象键值遍历
来源：http://xbl.xuetiantiany.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jyi.chenzaomai.com

[U92] JS：深拷贝
来源：http://uwq.jqgufenzy.top

structuredClone(obj)
来源：http://vcg.xuanzx.com

[U93] JS：模板字符串
来源：http://hsy.havefunace.top

`共 ${n} 条`
来源：http://nvl.aibaodan.cn

[U94] JS：箭头函数
来源：http://qjd.sweek.top

const double = x => x * 2;
来源：http://lff.fktsv.cn

[U95] JS：Promise 包装
来源：http://ayh.birdmap.top

new Promise((resolve, reject) => {})
来源：http://dkf.hammf.cn

[U96] JS：async/await 与异常
来源：http://llf.jinqigufen.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hto.shanyushiyangkeji.top

[U97] JS：并发请求
来源：http://mkv.yonumen.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ppb.xylfe.cn

[U98] JS：fetch 带 JSON
来源：http://ote.uphjek.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gmc.hesvh.cn

[U99] JS：事件监听
来源：http://qvr.tanke756.top

el.addEventListener("click", e => {})
来源：http://pvs.tanke756.top

[U100] JS：DOM 查询
来源：http://uok.shzxlz.cn

document.querySelector(".item")
来源：http://fld.svipenyu.cn

[U101] JS：classList 操作
来源：http://qan.ppjwa.cn

el.classList.toggle("active")
来源：http://jkd.sysykeji.top

[U102] JS：本地存储
来源：http://dnd.mhx1999.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://xpz.ehwqpu.com

[U103] JS：定时器
来源：http://aiv.ydjk.org.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kgi.epnwcf.com

[U104] JS：防抖
来源：http://uyq.meibo888.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dwh.hywenlv.cn

[U105] JS：节流
来源：http://hac.cdnleiting.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://sgy.hammf.cn

[U106] JS：日期格式化
来源：http://rfj.uphjek.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cgq.gogol.net.cn

[U107] JS：数字千分位
来源：http://tut.hnxiangtu.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://oeu.zdbjq.cn

[U108] JS：随机整数
来源：http://ulu.jyoumei.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://irx.snrcjt.cn

[U109] JS：数组分组
来源：http://adw.shanyushiyangkeji.top

Object.groupBy(arr, x => x.type)
来源：http://bov.jiagoushi.top

[U110] JS：数组分块
来源：http://iix.fengsongda.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fuf.zhaomingkeji.xyz

[U111] JS：对象转 Map
来源：http://gvj.jianghu66.top

new Map(Object.entries(obj))
来源：http://bbk.sufxvd.cn

[U112] JS：字符串补位
来源：http://hqq.hfpthk.cn

"7".padStart(3, "0")
来源：http://ymr.epnwcf.com

[U113] JS：正则替换全部
来源：http://iyz.shanyushiyangtech.top

s.replaceAll("a", "b")
来源：http://thv.cashguo.top

[U114] JS：JSON 深比较
来源：http://eev.iojbl.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://nxx.chenjidiqi.icu

[U115] JS：生成 UUID
来源：http://nau.tian-w.cn

crypto.randomUUID()
来源：http://atm.zhoulong.xyz

[U116] JS：类型检查（JSDoc）
来源：http://qcf.sjlbkw.cn

/** @param {string} name */ function f(name) {}
来源：http://idy.tanke756.top

[U117] JS：单元测试
来源：http://uid.wangdashe.top

npm i -D vitest;  npx vitest
来源：http://wkh.gzhubu.top

[U118] JS：开发服务器
来源：http://uca.zdbjq.cn

npm i -D vite;  npx vite
来源：http://xrc.ivvv.top


<!-- 参考信息 -->