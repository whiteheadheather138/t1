代发 wailian999

[T31] Lua：Hello World
来源：http://tdx.birdmap.top

print("Hello")
来源：http://zxb.bjfxy.top

[T32] Lua：局部变量
来源：http://wuk.52xcode.cn

local a = 1
来源：http://uvq.gogol.net.cn

[T33] Lua：表（数组）
来源：http://lbw.jianghu66.top

local t = {1, 2, 3};  t[4] = 4
来源：http://nbb.fehbvm.com

[T34] Lua：遍历表
来源：http://iut.nanxuanxn.top

for i, v in ipairs(t) do print(i, v) end
来源：http://jko.mhx1999.top

[T35] Lua：字典表
来源：http://qxa.tarul.cn

local d = { a = 1 };  d.b = 2
来源：http://hmh.hesvh.cn

[T36] Lua：函数
来源：http://fmd.guowangkeji.top

function add(a, b) return a + b end
来源：http://whj.wangdashe.top

[T37] Lua：字符串拼接
来源：http://pla.fktsv.cn

"a" .. "b"
来源：http://tna.zhixingplan.top

[T38] Lua：条件
来源：http://jas.nanxuanxn.top

if x > 0 then print("正") end
来源：http://wdc.vqdsnc.cn

[T39] Lua：模式匹配
来源：http://qrm.xinyue.icu

string.find(s, "%d+")
来源：http://urc.yueranfly.top

[T40] Lua：元表
来源：http://fct.jlsjyb.cn

setmetatable({}, { __index = base })
来源：http://jov.zhijiandao.cn

[T41] Perl：Hello World
来源：http://smi.nanxinkj.top

print "Hello\n";
来源：http://bwt.zdbjq.cn

[T42] Perl：变量类型
来源：http://eth.yanxiufei.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cew.xziqi.cn

[T43] Perl：字符串插值
来源：http://hbi.quarkkingdee.top

"值: $a"
来源：http://yfi.hnxiangtu.top

[T44] Perl：条件
来源：http://fhw.hywenlv.cn

if ($a > 0) { print "正"; }
来源：http://pim.shanyushiyangkeji.top

[T45] Perl：数组遍历
来源：http://afu.sxryk.cn

for my $x (@arr) { print $x; }
来源：http://nvp.nanxinkj.top

[T46] Perl：哈希操作
来源：http://dcm.bjfxy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://obr.shangyingyoupin.top

[T47] Perl：正则捕获
来源：http://uch.xuetiantiany.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://sfc.svipenyu.cn

[T48] Perl：正则替换
来源：http://bcg.bbcook.cn

$s =~ s/old/new/g;
来源：http://hec.bjfxy.top

[T49] Perl：函数
来源：http://yzn.yuanzhike.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tra.tianlin.xyz

[T50] Perl：逐行读文件
来源：http://hmt.aibaodan.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://azq.fzhhl.top

while (my $line = <$fh>) { print $line; }
来源：http://zaw.bjfxy.top

[T51] Scala：Hello World
来源：http://psv.jqgufenzy.top

println("Hello")
来源：http://fzn.tian-w.cn

[T52] Scala：变量
来源：http://uwn.jinqigufen.top

val a = 1;  var b = 2
来源：http://uid.xuanzx.com

[T53] Scala：字符串插值
来源：http://sdv.sjlbkw.cn

s"值: $b"
来源：http://kbx.hysaishi.cn

[T54] Scala：集合映射
来源：http://sur.sufxvd.cn

List(1, 2, 3).map(_ * 2)
来源：http://hit.yfazqb.com

[T55] Scala：集合过滤
来源：http://fug.gogol.net.cn

List(1, 2, 3).filter(_ > 1)
来源：http://zbi.jqgufenzy.top

[T56] Scala：样例类
来源：http://mli.epnwcf.com

case class User(name: String, age: Int)
来源：http://bja.uphjek.com

[T57] Scala：模式匹配
来源：http://set.hesvh.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://crl.cucudq.cn

[T58] Scala：函数定义
来源：http://lqa.iojbl.cn

def add(a: Int, b: Int): Int = a + b
来源：http://mpr.quarkkingdee.top

[T59] Scala：循环
来源：http://flu.andypj.xyz

for (i <- 1 to 10) println(i)
来源：http://yqz.feifeiyinyue.top

[T60] Scala：折叠
来源：http://mgl.shanyushiyangkeji.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zoq.cheryme.top

================================================================================
来源：http://sae.shzxlz.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kjt.birdmap.top

================================================================================
来源：http://nty.fehbvm.com

[U01] Py：创建虚拟环境
来源：http://kqk.c1oappe.top

python -m venv .venv && source .venv/bin/activate
来源：http://vqw.aibaodan.cn

[U02] Py：导出 / 安装依赖
来源：http://ykn.zhengqikj.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qdc.andypj.xyz

[U03] Py：加载 .env 配置
来源：http://eep.mhx1999.top

from dotenv import load_dotenv; load_dotenv()
来源：http://euv.mhx1999.top

[U04] Py：变量调试打印
来源：http://zrx.yuanzhike.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://avv.tianlin.xyz

[U05] Py：列表去重且保序
来源：http://btu.hongshengwenyu.top

list(dict.fromkeys(arr))
来源：http://qwm.ywan-chungtsiang.top

[U06] Py：合并两个字典
来源：http://ehd.cheryme.top

{**a, **b}
来源：http://elj.iojbl.cn

[U07] Py：反转字典键值
来源：http://jwl.ppjwa.cn

{v: k for k, v in d.items()}
来源：http://fqe.sufxvd.cn

[U08] Py：展平二维列表
来源：http://npy.zhengqikj.top

[y for x in nested for y in x]
来源：http://lfd.meibo888.top

[U09] Py：字典取最大值的键
来源：http://qos.zdqjudy.top

max(d, key=d.get)
来源：http://fil.cucudq.cn

[U10] Py：按值排序字典
来源：http://rgs.jinyuanbaomall.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://swg.pycfn.com

[U11] Py：生成器表达式
来源：http://umy.smart0.xyz

(x * 2 for x in arr)
来源：http://ker.nwbrower.top

[U12] Py：取出现最多的 3 个元素
来源：http://pqv.zhengqikj.top

Counter(arr).most_common(3)
来源：http://cnh.ivvv.top

[U13] Py：固定长度队列
来源：http://mlf.yfazqb.com

deque(maxlen=10)
来源：http://djn.wangshuangyany.cn

[U14] Py：分组收集到列表
来源：http://sro.smart0.xyz

defaultdict(list)
来源：http://rjs.yj202588.top

[U15] Py：高精度计时
来源：http://jsp.fzhhl.top

t = time.perf_counter()
来源：http://aio.tian-w.cn

[U16] Py：命令行参数解析
来源：http://ohl.hammf.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nfd.jinqigfzy.top

[U17] Py：初始化日志
来源：http://miv.aizwys.cn

logging.basicConfig(level=logging.INFO)
来源：http://jtg.meibo888.top

[U18] Py：预编译正则
来源：http://pxi.haohaochexian.top

pat = re.compile(r"\d+")
来源：http://pwc.yueranfly.top

[U19] Py：正则替换带回调
来源：http://wxo.9152youxi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ltc.nanxinkj.top

[U20] Py：缓存函数结果
来源：http://fbk.cqqwz.cn

@functools.lru_cache(maxsize=None)
来源：http://irz.shanyushiyangkeji.top

[U21] Py：自定义上下文管理器
来源：http://mno.zhengqikj.top

@contextlib.contextmanager
来源：http://hkh.yvedp.cn

[U22] Py：矩阵转置
来源：http://ltl.nwbrower.top

list(zip(*m))
来源：http://uoq.dianchejie.cn

[U23] Py：分块读取大文件
来源：http://oyq.gzhubu.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://arw.cucudq.cn

[U24] Py：路径操作
来源：http://trg.mhx1999.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pib.nanxuanxn.top

[U25] Py：CSV 按字典读
来源：http://ary.9152youxi.cn

csv.DictReader(f)
来源：http://tsp.nanxinkj.top

[U26] Py：并发下载
来源：http://qdl.fanxiaobao.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://kst.hysaishi.cn

[U27] Py：异步 HTTP
来源：http://svl.yj202588.top

aiohttp.ClientSession() 配合 async with
来源：http://wze.pycfn.com

[U28] Py：类型别名
来源：http://nlv.ctjpmb.com

UserId = int
来源：http://qog.guannengcc.top

[U29] Py：属性校验
来源：http://znv.hysaishi.cn

@property 与 @x.setter 配合
来源：http://bhs.epnwcf.com

[U30] Py：数据类
来源：http://wha.jiagoushi.top

@dataclass(slots=True)
来源：http://pia.svipenyu.cn

[U31] Py：单测
来源：http://yck.pengpengdd.cyou

python -m pytest -q
来源：http://icf.guannengcc.top

[U32] Py：代码格式化
来源：http://cle.nanxinkj.top

ruff format . && ruff check --fix .
来源：http://del.cqqwz.cn

[U33] Py：打包发布
来源：http://tls.feifeiyinyue.top

python -m build  （依赖 pyproject.toml）
来源：http://aox.jinyuanbaomall.cn

[U34] Py：判断编码
来源：http://cmq.cheryme.top

chardet.detect(raw)
来源：http://ggg.quarkkingdee.top

[U35] Py：发送邮件
来源：http://vzv.c1oappe.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://sey.shuidangran.top

[U36] Py：定时任务
来源：http://yyo.zhaomingkeji.xyz

schedule.every(10).minutes.do(job)
来源：http://qpv.jinqigufen.top

[U37] Py：读写 Excel
来源：http://byc.jyoumei.cn

pandas.read_excel / DataFrame.to_excel
来源：http://iyy.epnwcf.com

[U38] Py：获取脚本所在目录
来源：http://jlg.wangdashe.top

Path(__file__).resolve().parent
来源：http://ddb.jqgufenzy.top

[U39] Py：判断是否在交互环境
来源：http://tmo.ydjk.org.cn

sys.stdout.isatty()
来源：http://tej.aizwys.cn

[U40] Py：打印到标准错误
来源：http://waw.shzxlz.cn

print("err", file=sys.stderr)
来源：http://efg.pengpengdd.cyou

[U41] PHP：初始化 Composer 项目
来源：http://fow.hammf.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ygj.shanyushiyangkeji.top

[U42] PHP：PSR-4 自动加载
来源：http://jgo.zhengqikj.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://sct.shuidangran.top

[U43] PHP：声明命名空间
来源：http://rkw.fengsongda.top

namespace App\Http;
来源：http://guc.ywan-chungtsiang.top

[U44] PHP：开启严格类型
来源：http://bxq.jqgufenzy.top

declare(strict_types=1);
来源：http://woz.uphjek.com

[U45] PHP：类型声明与返回类型
来源：http://lzn.yfazqb.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://fug.cashguo.top

[U46] PHP：可空类型
来源：http://tdw.haohaochexian.top

?string $name = null
来源：http://tmp.ydzc1.top

[U47] PHP：联合类型
来源：http://vuj.nwbrower.top

int|string $id
来源：http://jwk.yuxming.cn

[U48] PHP：纯枚举
来源：http://eej.9152youxi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vmy.redwolf501.top

[U49] PHP：只读属性
来源：http://ehn.yueranfly.top

public readonly string $name
来源：http://ftg.ydzc1.top

[U50] PHP：构造器属性提升
来源：http://vsx.ybcxt.top

public function __construct(private int $id) {}
来源：http://vns.gaohongyu789.top

[U51] PHP：数组解构
来源：http://ern.yfazqb.com

[$a, $b] = $arr;
来源：http://gej.gaohongyu789.top

[U52] PHP：箭头函数
来源：http://tol.jyoumei.cn

$double = fn($x) => $x * 2;
来源：http://nhg.gotoacloud.top

[U53] PHP：空合并运算符
来源：http://joe.aibaodan.cn

$v = $a ?? $b ?? "default";
来源：http://zwn.jqgufenzy.top

[U54] PHP：空安全调用
来源：http://pdh.ydjk.org.cn

$obj?->method()
来源：http://uuf.iojbl.cn

[U55] PHP：match 表达式
来源：http://mbk.yangfankeji.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rmo.ctjpmb.com

[U56] PHP：命名参数
来源：http://gnk.zhongyouzk.top

f(a: 1, b: 2)
来源：http://udk.zhijiandao.cn

[U57] PHP：字符串插值
来源：http://yna.nanxuanxn.top

"值: {$a}"
来源：http://ahn.aibaodan.cn

[U58] PHP：数组三件套
来源：http://lvr.haohaochexian.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xby.zhixingplan.top

[U59] PHP：自定义排序
来源：http://zzg.nanxinkj.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aha.zhaomingkeji.xyz

[U60] PHP：JSON 编解码
来源：http://yqn.iojbl.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://nzv.bjfxy.top

[U61] PHP：正则
来源：http://pao.xuanzx.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ypy.yueranfly.top

[U62] PHP：日期对象
来源：http://lps.ehwqpu.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://sys.yanxiufei.cn

[U63] PHP：文件读写
来源：http://efu.zhijiandao.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gut.52xcode.cn

[U64] PHP：目录遍历
来源：http://pmb.guowangkeji.top

glob("dir/*.php");  scandir("dir");
来源：http://ttg.guowangkeji.top

[U65] PHP：会话
来源：http://oef.ybcxt.top

session_start();  $_SESSION["uid"] = 1;
来源：http://rtt.bbcook.cn

[U66] PHP：设置 Cookie
来源：http://tho.wangshuangyany.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://icf.zhaomingkeji.xyz

[U67] PHP：处理文件上传
来源：http://dtf.ywan-chungtsiang.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://nrq.tian-w.cn

[U68] PHP：PDO 连接
来源：http://xwf.zhengqikj.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ium.yfazqb.com

[U69] PHP：PDO 预处理
来源：http://zjr.cdnleiting.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kpr.jianghu66.top

[U70] PHP：PDO 事务
来源：http://xbj.fanxiaobao.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jtz.zycfv.cn

[U71] PHP：抛出异常
来源：http://vmo.hnqzz.top

throw new RuntimeException("失败", 500);
来源：http://xfm.yanxiufei.cn

[U72] PHP：写错误日志
来源：http://xar.ehwqpu.com

error_log("失败: " . $e->getMessage());
来源：http://xqu.hnqzz.top

[U73] PHP：读取 ini 配置
来源：http://ris.pycfn.com

parse_ini_file("config.ini", true)
来源：http://dtz.sufxvd.cn

[U74] PHP：读取环境变量
来源：http://fis.fehbvm.com

getenv("APP_ENV") ?: "production"
来源：http://mrn.dashuyun.cn

[U75] PHP：依赖注入
来源：http://pph.zhixingplan.top

composer require psr/container
来源：http://edz.zhixingplan.top

[U76] PHP：简单路由
来源：http://zsm.zhijiandao.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://aar.chenlongwang.top

[U77] PHP：模板渲染
来源：http://lzs.ivvv.top

composer require twig/twig
来源：http://ewe.fktsv.cn

[U78] PHP：单元测试
来源：http://mta.yuxming.cn

composer require --dev phpunit/phpunit
来源：http://sqr.chenlongwang.top

[U79] PHP：静态分析
来源：http://yti.sysykeji.top

composer require --dev phpstan/phpstan
来源：http://lol.cdnleiting.top

[U80] PHP：代码规范修复
来源：http://bvc.redwolf501.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://icd.jqgufenzy.top

[U81] JS：初始化项目
来源：http://tmi.xziqi.cn

npm init -y;  npm i express
来源：http://kpy.quarkkingdee.top

[U82] JS：package.json 脚本
来源：http://flz.wangdashe.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zyn.hammf.cn

[U83] JS：ES Module 导入导出
来源：http://onp.haohaochexian.top

export const a = 1;  import { a } from "./m.js";
来源：http://kai.kuanghao11.cn

[U84] JS：CommonJS 写法
来源：http://bne.yuanzhike.top

module.exports = { a };  const { a } = require("./m");
来源：http://qzl.cdnleiting.top

[U85] JS：可选链
来源：http://ncl.fehbvm.com

a?.b?.c
来源：http://zag.cdnleiting.top

[U86] JS：空值合并
来源：http://dsy.jqgufenzy.top

a ?? b
来源：http://jst.hnxiangtu.top

[U87] JS：解构默认值
来源：http://jho.svipenyu.cn

const { a = 1, b = 2 } = obj;
来源：http://gba.chenzaomai.com

[U88] JS：对象展开合并
来源：http://jtp.bbcook.cn

{ ...a, ...b }
来源：http://wbe.wangdashe.top

[U89] JS：数组去重
来源：http://bhw.xinyue.icu

[...new Set(arr)]
来源：http://glz.dianchejie.cn

[U90] JS：数字数组排序
来源：http://gzh.pycfn.com

[...arr].sort((a, b) => a - b)
来源：http://azg.zdbjq.cn

[U91] JS：对象键值遍历
来源：http://bje.zhiwuduotai.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bpt.jqgfzy.top

[U92] JS：深拷贝
来源：http://kfc.vqdsnc.cn

structuredClone(obj)
来源：http://vur.ybcxt.top

[U93] JS：模板字符串
来源：http://gpn.hongshengwenyu.top

`共 ${n} 条`
来源：http://duk.cashguo.top

[U94] JS：箭头函数
来源：http://kqh.hammf.cn

const double = x => x * 2;
来源：http://eib.ppjwa.cn

[U95] JS：Promise 包装
来源：http://tyz.guannengcc.top

new Promise((resolve, reject) => {})
来源：http://wte.yfazqb.com

[U96] JS：async/await 与异常
来源：http://oec.vehdjk.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gjx.vehdjk.com

[U97] JS：并发请求
来源：http://btr.fzhhl.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://pvv.hesvh.cn

[U98] JS：fetch 带 JSON
来源：http://rko.ppjwa.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://uln.tanke756.top

[U99] JS：事件监听
来源：http://fxg.daxiang520.top

el.addEventListener("click", e => {})
来源：http://def.yj20258.top

[U100] JS：DOM 查询
来源：http://urq.9152youxi.cn

document.querySelector(".item")
来源：http://dcf.jyoumei.cn

[U101] JS：classList 操作
来源：http://dcy.zhiwuduotai.top

el.classList.toggle("active")
来源：http://ovg.jlsjyb.cn

[U102] JS：本地存储
来源：http://oye.zhixingplan.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ynz.chenzaomai.com

[U103] JS：定时器
来源：http://szq.0kj1m.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://cus.vehdjk.com

[U104] JS：防抖
来源：http://chb.birdmap.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wwa.xuanzx.com

[U105] JS：节流
来源：http://mgj.fengsongda.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://sie.redwolf501.top

[U106] JS：日期格式化
来源：http://brl.redwolf501.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ive.tian-w.cn

[U107] JS：数字千分位
来源：http://xis.yangfankeji.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jzs.xziqi.cn

[U108] JS：随机整数
来源：http://iof.hfpthk.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://heb.cashguo.top

[U109] JS：数组分组
来源：http://iyi.yueranfly.top

Object.groupBy(arr, x => x.type)
来源：http://uqk.yuxming.cn

[U110] JS：数组分块
来源：http://cai.zhixingplan.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://toi.meibo888.top

[U111] JS：对象转 Map
来源：http://jfv.sxryk.cn

new Map(Object.entries(obj))
来源：http://gjn.iojbl.cn

[U112] JS：字符串补位
来源：http://gra.fzhhl.top

"7".padStart(3, "0")
来源：http://fox.zhijiandao.cn

[U113] JS：正则替换全部
来源：http://oor.zhiwuduotai.top

s.replaceAll("a", "b")
来源：http://bvg.gogol.net.cn

[U114] JS：JSON 深比较
来源：http://rjp.shuidangran.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://gia.zhijiandao.cn

[U115] JS：生成 UUID
来源：http://mnv.xuanzx.com

crypto.randomUUID()
来源：http://wbx.yuxming.cn

[U116] JS：类型检查（JSDoc）
来源：http://ent.yueranfly.top

/** @param {string} name */ function f(name) {}
来源：http://dcg.svipenyu.cn

[U117] JS：单元测试
来源：http://izz.wangshuangyany.cn

npm i -D vitest;  npx vitest
来源：http://idp.meibo888.top

[U118] JS：开发服务器
来源：http://jta.xziqi.cn

npm i -D vite;  npx vite
来源：http://ilq.hysaishi.cn


<!-- 参考信息 -->