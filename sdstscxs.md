代发 wailian999

[T33] Lua：表（数组）
来源：http://nso.hcnkem.com

local t = {1, 2, 3};  t[4] = 4
来源：http://adx.0kj1m.cn

[T34] Lua：遍历表
来源：http://ibm.meibo888.top

for i, v in ipairs(t) do print(i, v) end
来源：http://saa.chenjidiqi.icu

[T35] Lua：字典表
来源：http://nie.hysaishi.cn

local d = { a = 1 };  d.b = 2
来源：http://yyl.0kj1m.cn

[T36] Lua：函数
来源：http://hhi.guannengcc.top

function add(a, b) return a + b end
来源：http://pvf.chenjidiqi.icu

[T37] Lua：字符串拼接
来源：http://ocj.hcnkem.com

"a" .. "b"
来源：http://ghn.jinqigfzy.top

[T38] Lua：条件
来源：http://wfe.tarul.cn

if x > 0 then print("正") end
来源：http://lgs.xuetiantiany.cn

[T39] Lua：模式匹配
来源：http://rwb.dianchejie.cn

string.find(s, "%d+")
来源：http://kpl.zhijiandao.cn

[T40] Lua：元表
来源：http://alw.yuanzhike.top

setmetatable({}, { __index = base })
来源：http://rtk.sufxvd.cn

[T41] Perl：Hello World
来源：http://nol.shanyushiyangkeji.top

print "Hello\n";
来源：http://aql.hammf.cn

[T42] Perl：变量类型
来源：http://drd.vqdsnc.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ces.havefunace.top

[T43] Perl：字符串插值
来源：http://xfb.cashguo.top

"值: $a"
来源：http://doy.gotoacloud.top

[T44] Perl：条件
来源：http://bhy.jqgufenzy.top

if ($a > 0) { print "正"; }
来源：http://gyb.pycfn.com

[T45] Perl：数组遍历
来源：http://ngd.quarkkingdee.top

for my $x (@arr) { print $x; }
来源：http://pue.redwolf501.top

[T46] Perl：哈希操作
来源：http://web.zhixingplan.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://idd.jianghu66.top

[T47] Perl：正则捕获
来源：http://vnt.uphjek.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://zda.bbcook.cn

[T48] Perl：正则替换
来源：http://xlg.shuidangran.top

$s =~ s/old/new/g;
来源：http://qva.yj20258888.top

[T49] Perl：函数
来源：http://buu.jqgfzy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://uff.tianlin.xyz

[T50] Perl：逐行读文件
来源：http://djb.jinqigfzy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://byz.chenlongwang.top

while (my $line = <$fh>) { print $line; }
来源：http://fin.yj20258.top

[T51] Scala：Hello World
来源：http://ntc.meibo888.top

println("Hello")
来源：http://iqk.yangfankeji.com

[T52] Scala：变量
来源：http://ppb.zdqjudy.top

val a = 1;  var b = 2
来源：http://oje.tarul.cn

[T53] Scala：字符串插值
来源：http://xtd.yj202588.top

s"值: $b"
来源：http://auc.jinqigfzy.top

[T54] Scala：集合映射
来源：http://ktj.cheryme.top

List(1, 2, 3).map(_ * 2)
来源：http://zqm.pengpengdd.cyou

[T55] Scala：集合过滤
来源：http://pps.fzhhl.top

List(1, 2, 3).filter(_ > 1)
来源：http://dyb.yvedp.cn

[T56] Scala：样例类
来源：http://bdm.feifeiyinyue.top

case class User(name: String, age: Int)
来源：http://ljg.dianchejie.cn

[T57] Scala：模式匹配
来源：http://gig.wangdashe.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://siw.yuxming.cn

[T58] Scala：函数定义
来源：http://uxt.hammf.cn

def add(a: Int, b: Int): Int = a + b
来源：http://shd.hnqzz.top

[T59] Scala：循环
来源：http://ecp.sjlbkw.cn

for (i <- 1 to 10) println(i)
来源：http://vlt.yvedp.cn

[T60] Scala：折叠
来源：http://qdj.dianchejie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ybr.jqgfzy.top

================================================================================
来源：http://fue.ydzc1.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://whb.ivvv.top

================================================================================
来源：http://ify.hammf.cn

[U01] Py：创建虚拟环境
来源：http://nhu.aibaodan.cn

python -m venv .venv && source .venv/bin/activate
来源：http://owa.jlsjyb.cn

[U02] Py：导出 / 安装依赖
来源：http://pet.fengsongda.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ttd.haohaochexian.top

[U03] Py：加载 .env 配置
来源：http://gsm.ivvv.top

from dotenv import load_dotenv; load_dotenv()
来源：http://dnn.shangyingyoupin.top

[U04] Py：变量调试打印
来源：http://atq.jinqigfzy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pmr.yfazqb.com

[U05] Py：列表去重且保序
来源：http://pwj.cdnleiting.top

list(dict.fromkeys(arr))
来源：http://mfa.vehdjk.com

[U06] Py：合并两个字典
来源：http://jnl.yangfankeji.com

{**a, **b}
来源：http://vdx.ybcxt.top

[U07] Py：反转字典键值
来源：http://vxg.dianchejie.cn

{v: k for k, v in d.items()}
来源：http://uqp.hongshengwenyu.top

[U08] Py：展平二维列表
来源：http://vwb.zycfv.cn

[y for x in nested for y in x]
来源：http://cia.zhoulong.xyz

[U09] Py：字典取最大值的键
来源：http://fbe.xuanzx.com

max(d, key=d.get)
来源：http://ktb.zhongyouzk.top

[U10] Py：按值排序字典
来源：http://umz.jqgfzy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qpa.xingfuxueyuan.xyz

[U11] Py：生成器表达式
来源：http://acr.hnqzz.top

(x * 2 for x in arr)
来源：http://hkq.havefunace.top

[U12] Py：取出现最多的 3 个元素
来源：http://dlc.gaohongyu789.top

Counter(arr).most_common(3)
来源：http://yqo.0kj1m.cn

[U13] Py：固定长度队列
来源：http://quu.andypj.xyz

deque(maxlen=10)
来源：http://ars.xylfe.cn

[U14] Py：分组收集到列表
来源：http://kir.sjlbkw.cn

defaultdict(list)
来源：http://jxa.uphjek.com

[U15] Py：高精度计时
来源：http://icd.smart0.xyz

t = time.perf_counter()
来源：http://ziw.fzhhl.top

[U16] Py：命令行参数解析
来源：http://igj.iojbl.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wqa.ppjwa.cn

[U17] Py：初始化日志
来源：http://bmq.andypj.xyz

logging.basicConfig(level=logging.INFO)
来源：http://grq.wangdashe.top

[U18] Py：预编译正则
来源：http://ppw.guowangkeji.top

pat = re.compile(r"\d+")
来源：http://snt.52xcode.cn

[U19] Py：正则替换带回调
来源：http://oba.316326.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://duq.svipenyu.cn

[U20] Py：缓存函数结果
来源：http://lhl.ydzc1.top

@functools.lru_cache(maxsize=None)
来源：http://pkg.hywenlv.cn

[U21] Py：自定义上下文管理器
来源：http://yqx.wangdashe.top

@contextlib.contextmanager
来源：http://icc.dianchejie.cn

[U22] Py：矩阵转置
来源：http://lfs.nanxuanxn.top

list(zip(*m))
来源：http://saj.yueranfly.top

[U23] Py：分块读取大文件
来源：http://ihv.tian-w.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xig.zycfv.cn

[U24] Py：路径操作
来源：http://jth.uphjek.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bvj.vqdsnc.cn

[U25] Py：CSV 按字典读
来源：http://kfw.fengsongda.top

csv.DictReader(f)
来源：http://jiu.hnxiangtu.top

[U26] Py：并发下载
来源：http://xjw.ybcxt.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mws.yj202588.top

[U27] Py：异步 HTTP
来源：http://lpi.havefunace.top

aiohttp.ClientSession() 配合 async with
来源：http://mpa.shuidangran.top

[U28] Py：类型别名
来源：http://eln.xinyue.icu

UserId = int
来源：http://oyp.hesvh.cn

[U29] Py：属性校验
来源：http://jwa.ywan-chungtsiang.top

@property 与 @x.setter 配合
来源：http://sqo.yfazqb.com

[U30] Py：数据类
来源：http://hui.gotoacloud.top

@dataclass(slots=True)
来源：http://ttz.52xcode.cn

[U31] Py：单测
来源：http://yml.epnwcf.com

python -m pytest -q
来源：http://rsy.yangfankeji.com

[U32] Py：代码格式化
来源：http://ywg.jlsjyb.cn

ruff format . && ruff check --fix .
来源：http://jbl.ppjwa.cn

[U33] Py：打包发布
来源：http://stx.52xcode.cn

python -m build  （依赖 pyproject.toml）
来源：http://iym.ivvv.top

[U34] Py：判断编码
来源：http://oys.birdmap.top

chardet.detect(raw)
来源：http://ssu.yangfankeji.com

[U35] Py：发送邮件
来源：http://uic.sweek.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rgf.jqgfzy.top

[U36] Py：定时任务
来源：http://djj.zhaomingkeji.xyz

schedule.every(10).minutes.do(job)
来源：http://uja.yuanzhike.top

[U37] Py：读写 Excel
来源：http://rpg.aibaodan.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ozd.fanxiaobao.xyz

[U38] Py：获取脚本所在目录
来源：http://emf.daxiang520.top

Path(__file__).resolve().parent
来源：http://adt.fzhhl.top

[U39] Py：判断是否在交互环境
来源：http://dlm.uphjek.com

sys.stdout.isatty()
来源：http://fub.zdbjq.cn

[U40] Py：打印到标准错误
来源：http://ewu.c1oappe.top

print("err", file=sys.stderr)
来源：http://cjv.meibo888.top

[U41] PHP：初始化 Composer 项目
来源：http://wvw.hfpthk.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://xnk.kuanghao11.cn

[U42] PHP：PSR-4 自动加载
来源：http://afi.ywan-chungtsiang.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vbl.fengsongda.top

[U43] PHP：声明命名空间
来源：http://zpz.meibo888.top

namespace App\Http;
来源：http://uws.nanxinkj.top

[U44] PHP：开启严格类型
来源：http://oge.yj20258.top

declare(strict_types=1);
来源：http://oiz.yj20258888.top

[U45] PHP：类型声明与返回类型
来源：http://zli.yj202588.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://qxp.shanyushiyangkeji.top

[U46] PHP：可空类型
来源：http://tyy.yuanzhike.top

?string $name = null
来源：http://edr.ydzc1.top

[U47] PHP：联合类型
来源：http://brr.hfpthk.cn

int|string $id
来源：http://gjg.jiagoushi.top

[U48] PHP：纯枚举
来源：http://kda.zhiwuduotai.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://llc.ydzc1.top

[U49] PHP：只读属性
来源：http://dch.fehbvm.com

public readonly string $name
来源：http://bjs.yvedp.cn

[U50] PHP：构造器属性提升
来源：http://rdy.yvedp.cn

public function __construct(private int $id) {}
来源：http://bvv.yvedp.cn

[U51] PHP：数组解构
来源：http://eak.bjfxy.top

[$a, $b] = $arr;
来源：http://hyq.hnqzz.top

[U52] PHP：箭头函数
来源：http://sgu.hcnkem.com

$double = fn($x) => $x * 2;
来源：http://cgu.xuetiantiany.cn

[U53] PHP：空合并运算符
来源：http://ctw.yfazqb.com

$v = $a ?? $b ?? "default";
来源：http://hnr.yfazqb.com

[U54] PHP：空安全调用
来源：http://etl.snrcjt.cn

$obj?->method()
来源：http://xfb.zhengqikj.top

[U55] PHP：match 表达式
来源：http://fgn.nanxuanxn.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rgf.chenlongwang.top

[U56] PHP：命名参数
来源：http://ydf.yj20258888.top

f(a: 1, b: 2)
来源：http://mpm.yfazqb.com

[U57] PHP：字符串插值
来源：http://isf.smart0.xyz

"值: {$a}"
来源：http://ziq.ybcxt.top

[U58] PHP：数组三件套
来源：http://sqe.fzhhl.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mwv.gogol.net.cn

[U59] PHP：自定义排序
来源：http://tex.guowangkeji.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vml.yj202588.top

[U60] PHP：JSON 编解码
来源：http://xaj.sysykeji.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hgh.gaohongyu789.top

[U61] PHP：正则
来源：http://pwt.chenzaomai.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ihz.ybcxt.top

[U62] PHP：日期对象
来源：http://djr.sweek.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fjd.jlsjyb.cn

[U63] PHP：文件读写
来源：http://ssa.meibo888.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mpf.hysaishi.cn

[U64] PHP：目录遍历
来源：http://zst.havefunace.top

glob("dir/*.php");  scandir("dir");
来源：http://cza.kuanghao11.cn

[U65] PHP：会话
来源：http://rij.ehwqpu.com

session_start();  $_SESSION["uid"] = 1;
来源：http://dpy.mhx1999.top

[U66] PHP：设置 Cookie
来源：http://rik.wangdashe.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jle.yuxming.cn

[U67] PHP：处理文件上传
来源：http://wtq.c1oappe.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ypx.redwolf501.top

[U68] PHP：PDO 连接
来源：http://qfe.zhaomingkeji.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jav.0kj1m.cn

[U69] PHP：PDO 预处理
来源：http://buj.pycfn.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://eqo.nanxinkj.top

[U70] PHP：PDO 事务
来源：http://rev.yangfankeji.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tor.cashguo.top

[U71] PHP：抛出异常
来源：http://kpl.bjfxy.top

throw new RuntimeException("失败", 500);
来源：http://zcv.snrcjt.cn

[U72] PHP：写错误日志
来源：http://axj.aizwys.cn

error_log("失败: " . $e->getMessage());
来源：http://nhv.mhx1999.top

[U73] PHP：读取 ini 配置
来源：http://fll.feifeiyinyue.top

parse_ini_file("config.ini", true)
来源：http://bgx.andypj.xyz

[U74] PHP：读取环境变量
来源：http://bdi.zdqjudy.top

getenv("APP_ENV") ?: "production"
来源：http://gbz.fktsv.cn

[U75] PHP：依赖注入
来源：http://sws.sysykeji.top

composer require psr/container
来源：http://ljd.zhiwuduotai.top

[U76] PHP：简单路由
来源：http://fqd.ydzc1.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://trb.quarkkingdee.top

[U77] PHP：模板渲染
来源：http://nvh.chenlongwang.top

composer require twig/twig
来源：http://voj.pycfn.com

[U78] PHP：单元测试
来源：http://wgl.cucudq.cn

composer require --dev phpunit/phpunit
来源：http://fib.hywenlv.cn

[U79] PHP：静态分析
来源：http://tsb.shuidangran.top

composer require --dev phpstan/phpstan
来源：http://gvi.ydjk.org.cn

[U80] PHP：代码规范修复
来源：http://wfh.fktsv.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://bys.0kj1m.cn

[U81] JS：初始化项目
来源：http://jkx.guowangkeji.top

npm init -y;  npm i express
来源：http://izx.zhijiandao.cn

[U82] JS：package.json 脚本
来源：http://rmy.hnqzz.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xeh.fanxiaobao.xyz

[U83] JS：ES Module 导入导出
来源：http://hmm.xinyue.icu

export const a = 1;  import { a } from "./m.js";
来源：http://hqp.pengpengdd.cyou

[U84] JS：CommonJS 写法
来源：http://zjs.hongshengwenyu.top

module.exports = { a };  const { a } = require("./m");
来源：http://yjh.shangyingyoupin.top

[U85] JS：可选链
来源：http://yxg.xylfe.cn

a?.b?.c
来源：http://oec.wangshuangyany.cn

[U86] JS：空值合并
来源：http://ytb.havefunace.top

a ?? b
来源：http://ykv.pengpengdd.cyou

[U87] JS：解构默认值
来源：http://zsu.gzhubu.top

const { a = 1, b = 2 } = obj;
来源：http://stj.gotoacloud.top

[U88] JS：对象展开合并
来源：http://ewf.jqgfzy.top

{ ...a, ...b }
来源：http://qlp.fehbvm.com

[U89] JS：数组去重
来源：http://imy.sufxvd.cn

[...new Set(arr)]
来源：http://pls.chenlongwang.top

[U90] JS：数字数组排序
来源：http://xyn.gotoacloud.top

[...arr].sort((a, b) => a - b)
来源：http://fqf.shanyushiyangtech.top

[U91] JS：对象键值遍历
来源：http://xzn.yueranfly.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://oot.xylfe.cn

[U92] JS：深拷贝
来源：http://mqs.kuanghao11.cn

structuredClone(obj)
来源：http://ehe.jiagoushi.top

[U93] JS：模板字符串
来源：http://fvw.shuidangran.top

`共 ${n} 条`
来源：http://tbj.ehwqpu.com

[U94] JS：箭头函数
来源：http://jnq.dashuyun.cn

const double = x => x * 2;
来源：http://pau.tanke756.top

[U95] JS：Promise 包装
来源：http://did.vehdjk.com

new Promise((resolve, reject) => {})
来源：http://dbq.jinqigufen.top

[U96] JS：async/await 与异常
来源：http://ggt.ivvv.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pno.svipenyu.cn

[U97] JS：并发请求
来源：http://cwp.yuanzhike.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://dhn.xylfe.cn

[U98] JS：fetch 带 JSON
来源：http://foq.fktsv.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bbp.zycfv.cn

[U99] JS：事件监听
来源：http://ejv.pycfn.com

el.addEventListener("click", e => {})
来源：http://hmo.cqqwz.cn

[U100] JS：DOM 查询
来源：http://lxe.jlsjyb.cn

document.querySelector(".item")
来源：http://meh.ivvv.top

[U101] JS：classList 操作
来源：http://ouh.hongshengwenyu.top

el.classList.toggle("active")
来源：http://aos.zhengqikj.top

[U102] JS：本地存储
来源：http://zas.fengsongda.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://icr.smart0.xyz

[U103] JS：定时器
来源：http://wiu.zhijiandao.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vkx.bjfxy.top

[U104] JS：防抖
来源：http://coz.jyoumei.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pby.jyoumei.cn

[U105] JS：节流
来源：http://afv.havefunace.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jia.yongpay.top

[U106] JS：日期格式化
来源：http://bjy.vqdsnc.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://uor.tarul.cn

[U107] JS：数字千分位
来源：http://gle.wangdashe.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zwt.aizwys.cn

[U108] JS：随机整数
来源：http://mgf.daxiang520.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://uss.hongshengwenyu.top

[U109] JS：数组分组
来源：http://dys.fktsv.cn

Object.groupBy(arr, x => x.type)
来源：http://ffe.daria6918.cn

[U110] JS：数组分块
来源：http://mkt.gotoacloud.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pes.xingfuxueyuan.xyz

[U111] JS：对象转 Map
来源：http://yrb.sweek.top

new Map(Object.entries(obj))
来源：http://six.chenlongwang.top

[U112] JS：字符串补位
来源：http://qrs.yueranfly.top

"7".padStart(3, "0")
来源：http://bvz.epnwcf.com

[U113] JS：正则替换全部
来源：http://toh.kuanghao11.cn

s.replaceAll("a", "b")
来源：http://ngq.bjfxy.top

[U114] JS：JSON 深比较
来源：http://aiu.jinghuilouyu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://aga.zycfv.cn

[U115] JS：生成 UUID
来源：http://vpk.daxiang520.top

crypto.randomUUID()
来源：http://wbt.hongshengwenyu.top

[U116] JS：类型检查（JSDoc）
来源：http://jbg.daxiang520.top

/** @param {string} name */ function f(name) {}
来源：http://ssg.chenjidiqi.icu

[U117] JS：单元测试
来源：http://cuj.gogol.net.cn

npm i -D vitest;  npx vitest
来源：http://exq.xinyue.icu

[U118] JS：开发服务器
来源：http://rcr.hcnkem.com

npm i -D vite;  npx vite
来源：http://fwk.zhijiandao.cn

[U119] JS：生产构建
来源：http://nbj.cqqwz.cn

npx vite build
来源：http://ydh.hcnkem.com

[U120] JS：读取环境变量（Vite）
来源：http://ycw.shangyingyoupin.top

import.meta.env.VITE_API_URL
来源：http://haz.tian-w.cn


<!-- 参考信息 -->