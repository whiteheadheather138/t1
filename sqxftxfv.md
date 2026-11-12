代发 wailian999

[T31] Lua：Hello World
来源：http://nqe.xuanzx.com

print("Hello")
来源：http://ltm.shanyushiyangkeji.top

[T32] Lua：局部变量
来源：http://anm.aibaodan.cn

local a = 1
来源：http://tid.yanxiufei.cn

[T33] Lua：表（数组）
来源：http://mjj.9152youxi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://rlw.0kj1m.cn

[T34] Lua：遍历表
来源：http://rgi.jqgfzy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://edr.uphjek.com

[T35] Lua：字典表
来源：http://nwk.zdbjq.cn

local d = { a = 1 };  d.b = 2
来源：http://tux.gogol.net.cn

[T36] Lua：函数
来源：http://rlu.ivvv.top

function add(a, b) return a + b end
来源：http://jzv.shanyushiyangkeji.top

[T37] Lua：字符串拼接
来源：http://iqp.shzxlz.cn

"a" .. "b"
来源：http://jje.jqgufenzy.top

[T38] Lua：条件
来源：http://wxm.mhx1999.top

if x > 0 then print("正") end
来源：http://egn.52xcode.cn

[T39] Lua：模式匹配
来源：http://fej.jinqigufen.top

string.find(s, "%d+")
来源：http://wiv.cucudq.cn

[T40] Lua：元表
来源：http://xxx.ybcxt.top

setmetatable({}, { __index = base })
来源：http://gbp.xuanzx.com

[T41] Perl：Hello World
来源：http://rdn.yongpay.top

print "Hello\n";
来源：http://pnd.tianlin.xyz

[T42] Perl：变量类型
来源：http://pou.xuetiantiany.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bcj.cdnleiting.top

[T43] Perl：字符串插值
来源：http://skh.jianghu66.top

"值: $a"
来源：http://qiq.quarkkingdee.top

[T44] Perl：条件
来源：http://dvv.jinqigfzy.top

if ($a > 0) { print "正"; }
来源：http://aob.shanyushiyangtech.top

[T45] Perl：数组遍历
来源：http://mwj.9152youxi.cn

for my $x (@arr) { print $x; }
来源：http://twj.shanyushiyangkeji.top

[T46] Perl：哈希操作
来源：http://qox.gaohongyu789.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rzd.zdbjq.cn

[T47] Perl：正则捕获
来源：http://tpd.9152youxi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://pfs.hongshengwenyu.top

[T48] Perl：正则替换
来源：http://bfp.yuxming.cn

$s =~ s/old/new/g;
来源：http://zpi.nwbrower.top

[T49] Perl：函数
来源：http://lku.redwolf501.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://psw.wangshuangyany.cn

[T50] Perl：逐行读文件
来源：http://moy.dianchejie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://wpt.bjfxy.top

while (my $line = <$fh>) { print $line; }
来源：http://lfv.fktsv.cn

[T51] Scala：Hello World
来源：http://cgh.nwbrower.top

println("Hello")
来源：http://due.cdnleiting.top

[T52] Scala：变量
来源：http://kpi.chenlongwang.top

val a = 1;  var b = 2
来源：http://tlh.zdbjq.cn

[T53] Scala：字符串插值
来源：http://hyl.vqdsnc.cn

s"值: $b"
来源：http://jeq.iojbl.cn

[T54] Scala：集合映射
来源：http://wze.9152youxi.cn

List(1, 2, 3).map(_ * 2)
来源：http://dry.havefunace.top

[T55] Scala：集合过滤
来源：http://scx.daria6918.cn

List(1, 2, 3).filter(_ > 1)
来源：http://bau.redwolf501.top

[T56] Scala：样例类
来源：http://tdw.sysykeji.top

case class User(name: String, age: Int)
来源：http://wpg.wangshuangyany.cn

[T57] Scala：模式匹配
来源：http://hew.iojbl.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://dsa.sjlbkw.cn

[T58] Scala：函数定义
来源：http://zuy.gotoacloud.top

def add(a: Int, b: Int): Int = a + b
来源：http://nqn.c1oappe.top

[T59] Scala：循环
来源：http://wmf.zhixingplan.top

for (i <- 1 to 10) println(i)
来源：http://byx.nanxinkj.top

[T60] Scala：折叠
来源：http://fli.zhiwuduotai.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jcq.feifeiyinyue.top

================================================================================
来源：http://jez.jinqigfzy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qmk.fengsongda.top

================================================================================
来源：http://xme.zdqjudy.top

[U01] Py：创建虚拟环境
来源：http://bva.zhaomingkeji.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://tzd.feifeiyinyue.top

[U02] Py：导出 / 安装依赖
来源：http://oxc.mhx1999.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://uej.hesvh.cn

[U03] Py：加载 .env 配置
来源：http://qpk.guannengcc.top

from dotenv import load_dotenv; load_dotenv()
来源：http://fna.vqdsnc.cn

[U04] Py：变量调试打印
来源：http://gxi.shangyingyoupin.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://thu.0kj1m.cn

[U05] Py：列表去重且保序
来源：http://vjt.jiagoushi.top

list(dict.fromkeys(arr))
来源：http://yyt.xuanzx.com

[U06] Py：合并两个字典
来源：http://ktm.guannengcc.top

{**a, **b}
来源：http://jap.ydzc1.top

[U07] Py：反转字典键值
来源：http://mog.zhixingplan.top

{v: k for k, v in d.items()}
来源：http://wmz.daria6918.cn

[U08] Py：展平二维列表
来源：http://azz.feifeiyinyue.top

[y for x in nested for y in x]
来源：http://hdu.fanxiaobao.xyz

[U09] Py：字典取最大值的键
来源：http://ldu.ybcxt.top

max(d, key=d.get)
来源：http://ltq.shzxlz.cn

[U10] Py：按值排序字典
来源：http://lym.tanke756.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mbd.zhiwuduotai.top

[U11] Py：生成器表达式
来源：http://zbk.wangshuangyany.cn

(x * 2 for x in arr)
来源：http://eis.meibo888.top

[U12] Py：取出现最多的 3 个元素
来源：http://rib.xuetiantiany.cn

Counter(arr).most_common(3)
来源：http://zwt.wangshuangyany.cn

[U13] Py：固定长度队列
来源：http://zjg.gaohongyu789.top

deque(maxlen=10)
来源：http://jnf.haohaochexian.top

[U14] Py：分组收集到列表
来源：http://cla.vqdsnc.cn

defaultdict(list)
来源：http://tuq.jlsjyb.cn

[U15] Py：高精度计时
来源：http://nxw.cqqwz.cn

t = time.perf_counter()
来源：http://kjz.bjfxy.top

[U16] Py：命令行参数解析
来源：http://ovi.sufxvd.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zmq.xingfuxueyuan.xyz

[U17] Py：初始化日志
来源：http://mrw.fanxiaobao.xyz

logging.basicConfig(level=logging.INFO)
来源：http://msr.sjlbkw.cn

[U18] Py：预编译正则
来源：http://ejw.birdmap.top

pat = re.compile(r"\d+")
来源：http://kht.xylfe.cn

[U19] Py：正则替换带回调
来源：http://ucf.cucudq.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jot.nwbrower.top

[U20] Py：缓存函数结果
来源：http://vsk.0kj1m.cn

@functools.lru_cache(maxsize=None)
来源：http://ncq.zdqjudy.top

[U21] Py：自定义上下文管理器
来源：http://qsd.cashguo.top

@contextlib.contextmanager
来源：http://wmg.kuanghao11.cn

[U22] Py：矩阵转置
来源：http://sge.yangfankeji.com

list(zip(*m))
来源：http://rdf.chenzaomai.com

[U23] Py：分块读取大文件
来源：http://zpc.epnwcf.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://box.gaohongyu789.top

[U24] Py：路径操作
来源：http://xbk.hesvh.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qhp.yueranfly.top

[U25] Py：CSV 按字典读
来源：http://val.chenjidiqi.icu

csv.DictReader(f)
来源：http://vzy.jinqigufen.top

[U26] Py：并发下载
来源：http://pfd.xingfuxueyuan.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wgq.yj202588.top

[U27] Py：异步 HTTP
来源：http://ndy.vqdsnc.cn

aiohttp.ClientSession() 配合 async with
来源：http://cwr.gaohongyu789.top

[U28] Py：类型别名
来源：http://spi.jinqigufen.top

UserId = int
来源：http://nmz.jlsjyb.cn

[U29] Py：属性校验
来源：http://opf.yfazqb.com

@property 与 @x.setter 配合
来源：http://lbb.ivvv.top

[U30] Py：数据类
来源：http://ngr.zhiwuduotai.top

@dataclass(slots=True)
来源：http://kcl.gaohongyu789.top

[U31] Py：单测
来源：http://cgh.jinqigfzy.top

python -m pytest -q
来源：http://oyt.wangshuangyany.cn

[U32] Py：代码格式化
来源：http://ayd.bbcook.cn

ruff format . && ruff check --fix .
来源：http://ens.xinyue.icu

[U33] Py：打包发布
来源：http://kjh.zdbjq.cn

python -m build  （依赖 pyproject.toml）
来源：http://vbu.yj202588.top

[U34] Py：判断编码
来源：http://zhs.yanxiufei.cn

chardet.detect(raw)
来源：http://fha.ybcxt.top

[U35] Py：发送邮件
来源：http://xbj.zhixingplan.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://aiu.yuxming.cn

[U36] Py：定时任务
来源：http://bpq.iojbl.cn

schedule.every(10).minutes.do(job)
来源：http://fhn.yj20258888.top

[U37] Py：读写 Excel
来源：http://gqy.shzxlz.cn

pandas.read_excel / DataFrame.to_excel
来源：http://xhw.cheryme.top

[U38] Py：获取脚本所在目录
来源：http://gjj.jqgufenzy.top

Path(__file__).resolve().parent
来源：http://nlg.chenjidiqi.icu

[U39] Py：判断是否在交互环境
来源：http://wfl.zhaomingkeji.xyz

sys.stdout.isatty()
来源：http://uev.fzhhl.top

[U40] Py：打印到标准错误
来源：http://hyx.redwolf501.top

print("err", file=sys.stderr)
来源：http://hzw.daria6918.cn

[U41] PHP：初始化 Composer 项目
来源：http://uzw.zhaomingkeji.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://lwg.xylfe.cn

[U42] PHP：PSR-4 自动加载
来源：http://asq.shuidangran.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vki.haohaochexian.top

[U43] PHP：声明命名空间
来源：http://zas.fanxiaobao.xyz

namespace App\Http;
来源：http://cpc.jinghuilouyu.cn

[U44] PHP：开启严格类型
来源：http://wgd.yj20258.top

declare(strict_types=1);
来源：http://trz.52xcode.cn

[U45] PHP：类型声明与返回类型
来源：http://nxp.epnwcf.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://hjp.ydzc1.top

[U46] PHP：可空类型
来源：http://sva.ybcxt.top

?string $name = null
来源：http://vqp.sufxvd.cn

[U47] PHP：联合类型
来源：http://knp.sufxvd.cn

int|string $id
来源：http://inu.cqqwz.cn

[U48] PHP：纯枚举
来源：http://ofi.xuetiantiany.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ufb.mhx1999.top

[U49] PHP：只读属性
来源：http://rbl.daxiang520.top

public readonly string $name
来源：http://rfp.zhoulong.xyz

[U50] PHP：构造器属性提升
来源：http://txd.ehwqpu.com

public function __construct(private int $id) {}
来源：http://vce.cheryme.top

[U51] PHP：数组解构
来源：http://uko.xziqi.cn

[$a, $b] = $arr;
来源：http://abr.xinyue.icu

[U52] PHP：箭头函数
来源：http://zgh.hammf.cn

$double = fn($x) => $x * 2;
来源：http://mcu.sufxvd.cn

[U53] PHP：空合并运算符
来源：http://qda.nwbrower.top

$v = $a ?? $b ?? "default";
来源：http://gxa.sweek.top

[U54] PHP：空安全调用
来源：http://pka.ybcxt.top

$obj?->method()
来源：http://xlt.bbcook.cn

[U55] PHP：match 表达式
来源：http://kjy.fanxiaobao.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rpa.jlsjyb.cn

[U56] PHP：命名参数
来源：http://rbi.9152youxi.cn

f(a: 1, b: 2)
来源：http://mzo.meibo888.top

[U57] PHP：字符串插值
来源：http://mrp.chenzaomai.com

"值: {$a}"
来源：http://spc.jinqigfzy.top

[U58] PHP：数组三件套
来源：http://smd.jqgufenzy.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://tdw.xingfuxueyuan.xyz

[U59] PHP：自定义排序
来源：http://nus.zhixingplan.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yhi.fktsv.cn

[U60] PHP：JSON 编解码
来源：http://fyd.sysykeji.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dvk.havefunace.top

[U61] PHP：正则
来源：http://sdl.nanxuanxn.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pff.cheryme.top

[U62] PHP：日期对象
来源：http://wgj.ywan-chungtsiang.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://tfc.ehwqpu.com

[U63] PHP：文件读写
来源：http://wmo.hnxiangtu.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jlx.yanxiufei.cn

[U64] PHP：目录遍历
来源：http://est.vqdsnc.cn

glob("dir/*.php");  scandir("dir");
来源：http://ixv.zhiwuduotai.top

[U65] PHP：会话
来源：http://zpc.jinghuilouyu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://geg.shanyushiyangtech.top

[U66] PHP：设置 Cookie
来源：http://ezh.svipenyu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mmm.haohaochexian.top

[U67] PHP：处理文件上传
来源：http://qnq.hcnkem.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kzf.vehdjk.com

[U68] PHP：PDO 连接
来源：http://scs.yuanzhike.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://roy.hongshengwenyu.top

[U69] PHP：PDO 预处理
来源：http://bbe.hcnkem.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qkt.dianchejie.cn

[U70] PHP：PDO 事务
来源：http://ufe.xingfuxueyuan.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bnc.fktsv.cn

[U71] PHP：抛出异常
来源：http://rxp.hcnkem.com

throw new RuntimeException("失败", 500);
来源：http://zzv.feifeiyinyue.top

[U72] PHP：写错误日志
来源：http://zoy.sxryk.cn

error_log("失败: " . $e->getMessage());
来源：http://eun.jinghuilouyu.cn

[U73] PHP：读取 ini 配置
来源：http://bpq.yj20258888.top

parse_ini_file("config.ini", true)
来源：http://uzp.yuxming.cn

[U74] PHP：读取环境变量
来源：http://nup.ehwqpu.com

getenv("APP_ENV") ?: "production"
来源：http://xkm.xuanzx.com

[U75] PHP：依赖注入
来源：http://aha.yfazqb.com

composer require psr/container
来源：http://fyn.hammf.cn

[U76] PHP：简单路由
来源：http://aey.tianlin.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ium.andypj.xyz

[U77] PHP：模板渲染
来源：http://ljz.gogol.net.cn

composer require twig/twig
来源：http://inx.c1oappe.top

[U78] PHP：单元测试
来源：http://sbj.dianchejie.cn

composer require --dev phpunit/phpunit
来源：http://ioq.shzxlz.cn

[U79] PHP：静态分析
来源：http://qps.iojbl.cn

composer require --dev phpstan/phpstan
来源：http://nlr.yonumen.top

[U80] PHP：代码规范修复
来源：http://csa.meibo888.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://eoo.yangfankeji.com

[U81] JS：初始化项目
来源：http://smp.shanyushiyangkeji.top

npm init -y;  npm i express
来源：http://uqs.shangyingyoupin.top

[U82] JS：package.json 脚本
来源：http://ein.daxiang520.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jie.hesvh.cn

[U83] JS：ES Module 导入导出
来源：http://ppg.bbcook.cn

export const a = 1;  import { a } from "./m.js";
来源：http://xme.epnwcf.com

[U84] JS：CommonJS 写法
来源：http://vdp.cqqwz.cn

module.exports = { a };  const { a } = require("./m");
来源：http://oyz.svipenyu.cn

[U85] JS：可选链
来源：http://jua.smart0.xyz

a?.b?.c
来源：http://ggy.shangyingyoupin.top

[U86] JS：空值合并
来源：http://xxw.ywan-chungtsiang.top

a ?? b
来源：http://oyi.nanxinkj.top

[U87] JS：解构默认值
来源：http://rqg.yongpay.top

const { a = 1, b = 2 } = obj;
来源：http://iig.yj20258.top

[U88] JS：对象展开合并
来源：http://ibw.fzhhl.top

{ ...a, ...b }
来源：http://tpw.jinqigufen.top

[U89] JS：数组去重
来源：http://ytc.yonumen.top

[...new Set(arr)]
来源：http://pit.jqgfzy.top

[U90] JS：数字数组排序
来源：http://zln.wangshuangyany.cn

[...arr].sort((a, b) => a - b)
来源：http://lyx.c1oappe.top

[U91] JS：对象键值遍历
来源：http://hfp.hnxiangtu.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dnh.jiagoushi.top

[U92] JS：深拷贝
来源：http://glq.yj20258888.top

structuredClone(obj)
来源：http://qwt.jqgufenzy.top

[U93] JS：模板字符串
来源：http://poe.feifeiyinyue.top

`共 ${n} 条`
来源：http://pze.yuxming.cn

[U94] JS：箭头函数
来源：http://zen.9152youxi.cn

const double = x => x * 2;
来源：http://ywi.iojbl.cn

[U95] JS：Promise 包装
来源：http://nqp.snrcjt.cn

new Promise((resolve, reject) => {})
来源：http://odh.zhongyouzk.top

[U96] JS：async/await 与异常
来源：http://tox.nanxuanxn.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://kxw.andypj.xyz

[U97] JS：并发请求
来源：http://vdc.xingfuxueyuan.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://ced.kuanghao11.cn

[U98] JS：fetch 带 JSON
来源：http://ysy.zhixingplan.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wrn.ydzc1.top

[U99] JS：事件监听
来源：http://zsx.mhx1999.top

el.addEventListener("click", e => {})
来源：http://nxw.c1oappe.top

[U100] JS：DOM 查询
来源：http://xnp.ydjk.org.cn

document.querySelector(".item")
来源：http://ful.tianlin.xyz

[U101] JS：classList 操作
来源：http://bzk.tian-w.cn

el.classList.toggle("active")
来源：http://fxb.zhijiandao.cn

[U102] JS：本地存储
来源：http://qho.pengpengdd.cyou

localStorage.setItem("k", JSON.stringify(v))
来源：http://xjw.kuanghao11.cn

[U103] JS：定时器
来源：http://xhr.dianchejie.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://osd.cdnleiting.top

[U104] JS：防抖
来源：http://njo.ctjpmb.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qya.hammf.cn

[U105] JS：节流
来源：http://bwt.nwbrower.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ydb.feifeiyinyue.top

[U106] JS：日期格式化
来源：http://yub.birdmap.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ipc.epnwcf.com

[U107] JS：数字千分位
来源：http://uwn.iojbl.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ssw.gaohongyu789.top

[U108] JS：随机整数
来源：http://gob.pengpengdd.cyou

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mmy.jinqigfzy.top

[U109] JS：数组分组
来源：http://krr.yanxiufei.cn

Object.groupBy(arr, x => x.type)
来源：http://usa.ydzc1.top

[U110] JS：数组分块
来源：http://tex.fanxiaobao.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://brq.shangyingyoupin.top

[U111] JS：对象转 Map
来源：http://hhf.ehwqpu.com

new Map(Object.entries(obj))
来源：http://bhn.fehbvm.com

[U112] JS：字符串补位
来源：http://ydl.redwolf501.top

"7".padStart(3, "0")
来源：http://urr.hywenlv.cn

[U113] JS：正则替换全部
来源：http://dzd.nwbrower.top

s.replaceAll("a", "b")
来源：http://wav.nwbrower.top

[U114] JS：JSON 深比较
来源：http://rlh.hammf.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ezb.gaohongyu789.top

[U115] JS：生成 UUID
来源：http://jgk.zdbjq.cn

crypto.randomUUID()
来源：http://rzj.ehwqpu.com

[U116] JS：类型检查（JSDoc）
来源：http://eok.cqqwz.cn

/** @param {string} name */ function f(name) {}
来源：http://gaq.hammf.cn

[U117] JS：单元测试
来源：http://rzk.hywenlv.cn

npm i -D vitest;  npx vitest
来源：http://isk.yj20258.top

[U118] JS：开发服务器
来源：http://izy.sufxvd.cn

npm i -D vite;  npx vite
来源：http://zcn.cheryme.top


<!-- 参考信息 -->