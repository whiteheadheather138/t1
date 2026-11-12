代发 wailian999

[T31] Lua：Hello World
来源：http://qdx.hysaishi.cn

print("Hello")
来源：http://hjp.gotoacloud.top

[T32] Lua：局部变量
来源：http://wbw.hnxiangtu.top

local a = 1
来源：http://nge.smart0.xyz

[T33] Lua：表（数组）
来源：http://mvn.xziqi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hyp.jinyuanbaomall.cn

[T34] Lua：遍历表
来源：http://agi.ywan-chungtsiang.top

for i, v in ipairs(t) do print(i, v) end
来源：http://duk.fengsongda.top

[T35] Lua：字典表
来源：http://kah.nwbrower.top

local d = { a = 1 };  d.b = 2
来源：http://uey.c1oappe.top

[T36] Lua：函数
来源：http://rlh.jqgufenzy.top

function add(a, b) return a + b end
来源：http://poj.xingfuxueyuan.xyz

[T37] Lua：字符串拼接
来源：http://ocs.bbcook.cn

"a" .. "b"
来源：http://qqh.nanxinkj.top

[T38] Lua：条件
来源：http://ofq.ydzc1.top

if x > 0 then print("正") end
来源：http://otl.jiagoushi.top

[T39] Lua：模式匹配
来源：http://rgu.tianlin.xyz

string.find(s, "%d+")
来源：http://jok.fktsv.cn

[T40] Lua：元表
来源：http://rej.gzhubu.top

setmetatable({}, { __index = base })
来源：http://icw.xuanzx.com

[T41] Perl：Hello World
来源：http://xwk.kuanghao11.cn

print "Hello\n";
来源：http://ndb.cdnleiting.top

[T42] Perl：变量类型
来源：http://ssq.zhijiandao.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qai.yuxming.cn

[T43] Perl：字符串插值
来源：http://fxx.sjlbkw.cn

"值: $a"
来源：http://gus.zhiwuduotai.top

[T44] Perl：条件
来源：http://yhy.fzhhl.top

if ($a > 0) { print "正"; }
来源：http://irz.wangdashe.top

[T45] Perl：数组遍历
来源：http://zkv.jiagoushi.top

for my $x (@arr) { print $x; }
来源：http://pwl.pengpengdd.cyou

[T46] Perl：哈希操作
来源：http://jvt.jinqigufen.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hak.aizwys.cn

[T47] Perl：正则捕获
来源：http://vwt.hesvh.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://xma.cheryme.top

[T48] Perl：正则替换
来源：http://dgj.jlsjyb.cn

$s =~ s/old/new/g;
来源：http://jew.mhx1999.top

[T49] Perl：函数
来源：http://kmk.yongpay.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pif.redwolf501.top

[T50] Perl：逐行读文件
来源：http://fwq.ydjk.org.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ygn.birdmap.top

while (my $line = <$fh>) { print $line; }
来源：http://etk.zhixingplan.top

[T51] Scala：Hello World
来源：http://tqm.yj20258.top

println("Hello")
来源：http://nyl.hysaishi.cn

[T52] Scala：变量
来源：http://fzr.tianlin.xyz

val a = 1;  var b = 2
来源：http://alw.epnwcf.com

[T53] Scala：字符串插值
来源：http://gur.tianlin.xyz

s"值: $b"
来源：http://gsg.xziqi.cn

[T54] Scala：集合映射
来源：http://eur.ivvv.top

List(1, 2, 3).map(_ * 2)
来源：http://glh.yanxiufei.cn

[T55] Scala：集合过滤
来源：http://dnv.smart0.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://iij.chenzaomai.com

[T56] Scala：样例类
来源：http://yxy.0kj1m.cn

case class User(name: String, age: Int)
来源：http://olm.zhijiandao.cn

[T57] Scala：模式匹配
来源：http://qhf.xziqi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://zpo.zhixingplan.top

[T58] Scala：函数定义
来源：http://yti.tianlin.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://dow.ydzc1.top

[T59] Scala：循环
来源：http://uqa.ywan-chungtsiang.top

for (i <- 1 to 10) println(i)
来源：http://kby.gaohongyu789.top

[T60] Scala：折叠
来源：http://twg.daxiang520.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bjh.zhaomingkeji.xyz

================================================================================
来源：http://eof.chenjidiqi.icu

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mac.sweek.top

================================================================================
来源：http://oeu.yangfankeji.com

[U01] Py：创建虚拟环境
来源：http://xmf.hnqzz.top

python -m venv .venv && source .venv/bin/activate
来源：http://wkb.jiagoushi.top

[U02] Py：导出 / 安装依赖
来源：http://xvy.aizwys.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tsh.hnxiangtu.top

[U03] Py：加载 .env 配置
来源：http://nvf.wangdashe.top

from dotenv import load_dotenv; load_dotenv()
来源：http://rrw.xinyue.icu

[U04] Py：变量调试打印
来源：http://hdb.hcnkem.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bce.tian-w.cn

[U05] Py：列表去重且保序
来源：http://skc.xinyue.icu

list(dict.fromkeys(arr))
来源：http://kwj.dianchejie.cn

[U06] Py：合并两个字典
来源：http://uyk.yangfankeji.com

{**a, **b}
来源：http://nja.ywan-chungtsiang.top

[U07] Py：反转字典键值
来源：http://zcc.gzhubu.top

{v: k for k, v in d.items()}
来源：http://mcd.0kj1m.cn

[U08] Py：展平二维列表
来源：http://hzi.c1oappe.top

[y for x in nested for y in x]
来源：http://zfj.sweek.top

[U09] Py：字典取最大值的键
来源：http://twf.bjfxy.top

max(d, key=d.get)
来源：http://dqr.yueranfly.top

[U10] Py：按值排序字典
来源：http://gtt.quarkkingdee.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zwo.yanxiufei.cn

[U11] Py：生成器表达式
来源：http://qvg.ppjwa.cn

(x * 2 for x in arr)
来源：http://ydq.tianlin.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://yfp.bbcook.cn

Counter(arr).most_common(3)
来源：http://jdu.dianchejie.cn

[U13] Py：固定长度队列
来源：http://zqq.guowangkeji.top

deque(maxlen=10)
来源：http://rvb.zycfv.cn

[U14] Py：分组收集到列表
来源：http://okj.yuxming.cn

defaultdict(list)
来源：http://uhl.ybcxt.top

[U15] Py：高精度计时
来源：http://ott.zhaomingkeji.xyz

t = time.perf_counter()
来源：http://yqb.kuanghao11.cn

[U16] Py：命令行参数解析
来源：http://vot.jlsjyb.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xpk.cashguo.top

[U17] Py：初始化日志
来源：http://isy.quarkkingdee.top

logging.basicConfig(level=logging.INFO)
来源：http://jog.bbcook.cn

[U18] Py：预编译正则
来源：http://wxc.hfpthk.cn

pat = re.compile(r"\d+")
来源：http://obf.aibaodan.cn

[U19] Py：正则替换带回调
来源：http://qmm.iojbl.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hxi.bjfxy.top

[U20] Py：缓存函数结果
来源：http://zdw.fanxiaobao.xyz

@functools.lru_cache(maxsize=None)
来源：http://pow.iojbl.cn

[U21] Py：自定义上下文管理器
来源：http://vnp.fktsv.cn

@contextlib.contextmanager
来源：http://auz.yfazqb.com

[U22] Py：矩阵转置
来源：http://wqp.jinyuanbaomall.cn

list(zip(*m))
来源：http://fln.zhaomingkeji.xyz

[U23] Py：分块读取大文件
来源：http://dmf.sxryk.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tmt.fehbvm.com

[U24] Py：路径操作
来源：http://wil.hywenlv.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ntq.sjlbkw.cn

[U25] Py：CSV 按字典读
来源：http://pyg.shanyushiyangtech.top

csv.DictReader(f)
来源：http://bhe.316326.xyz

[U26] Py：并发下载
来源：http://mdg.guannengcc.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://opw.fengsongda.top

[U27] Py：异步 HTTP
来源：http://jao.fanxiaobao.xyz

aiohttp.ClientSession() 配合 async with
来源：http://foa.hcnkem.com

[U28] Py：类型别名
来源：http://zfk.bbcook.cn

UserId = int
来源：http://jzx.c1oappe.top

[U29] Py：属性校验
来源：http://vxu.yueranfly.top

@property 与 @x.setter 配合
来源：http://mea.birdmap.top

[U30] Py：数据类
来源：http://sbs.jinqigufen.top

@dataclass(slots=True)
来源：http://qrc.yanxiufei.cn

[U31] Py：单测
来源：http://zqm.yongpay.top

python -m pytest -q
来源：http://wpw.hywenlv.cn

[U32] Py：代码格式化
来源：http://dae.zhijiandao.cn

ruff format . && ruff check --fix .
来源：http://uqc.fzhhl.top

[U33] Py：打包发布
来源：http://kgz.vehdjk.com

python -m build  （依赖 pyproject.toml）
来源：http://dog.52xcode.cn

[U34] Py：判断编码
来源：http://ljk.gaohongyu789.top

chardet.detect(raw)
来源：http://byc.shanyushiyangkeji.top

[U35] Py：发送邮件
来源：http://amh.ydzc1.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gcg.daria6918.cn

[U36] Py：定时任务
来源：http://ktz.feifeiyinyue.top

schedule.every(10).minutes.do(job)
来源：http://pnq.daria6918.cn

[U37] Py：读写 Excel
来源：http://law.yj202588.top

pandas.read_excel / DataFrame.to_excel
来源：http://sir.wangdashe.top

[U38] Py：获取脚本所在目录
来源：http://oni.sufxvd.cn

Path(__file__).resolve().parent
来源：http://yjp.vqdsnc.cn

[U39] Py：判断是否在交互环境
来源：http://kvm.jinghuilouyu.cn

sys.stdout.isatty()
来源：http://smp.ydjk.org.cn

[U40] Py：打印到标准错误
来源：http://gjh.daxiang520.top

print("err", file=sys.stderr)
来源：http://gpy.jinqigufen.top

[U41] PHP：初始化 Composer 项目
来源：http://wbz.sufxvd.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://pfo.nanxuanxn.top

[U42] PHP：PSR-4 自动加载
来源：http://jap.pycfn.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vfo.yvedp.cn

[U43] PHP：声明命名空间
来源：http://pax.ywan-chungtsiang.top

namespace App\Http;
来源：http://qrt.pengpengdd.cyou

[U44] PHP：开启严格类型
来源：http://gfm.andypj.xyz

declare(strict_types=1);
来源：http://zfw.hnxiangtu.top

[U45] PHP：类型声明与返回类型
来源：http://nlj.ydjk.org.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ric.jqgfzy.top

[U46] PHP：可空类型
来源：http://tlh.haohaochexian.top

?string $name = null
来源：http://ign.hysaishi.cn

[U47] PHP：联合类型
来源：http://sue.jqgufenzy.top

int|string $id
来源：http://bdi.fktsv.cn

[U48] PHP：纯枚举
来源：http://qoe.guannengcc.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tcl.yanxiufei.cn

[U49] PHP：只读属性
来源：http://bhy.guowangkeji.top

public readonly string $name
来源：http://gji.yfazqb.com

[U50] PHP：构造器属性提升
来源：http://uuk.jqgufenzy.top

public function __construct(private int $id) {}
来源：http://sbh.xingfuxueyuan.xyz

[U51] PHP：数组解构
来源：http://xxn.nanxuanxn.top

[$a, $b] = $arr;
来源：http://jeq.daxiang520.top

[U52] PHP：箭头函数
来源：http://yxz.tanke756.top

$double = fn($x) => $x * 2;
来源：http://ldp.xziqi.cn

[U53] PHP：空合并运算符
来源：http://juh.aibaodan.cn

$v = $a ?? $b ?? "default";
来源：http://fbg.havefunace.top

[U54] PHP：空安全调用
来源：http://znd.yj20258.top

$obj?->method()
来源：http://ggq.yanxiufei.cn

[U55] PHP：match 表达式
来源：http://ock.iojbl.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jnt.hywenlv.cn

[U56] PHP：命名参数
来源：http://fjl.jyoumei.cn

f(a: 1, b: 2)
来源：http://oru.svipenyu.cn

[U57] PHP：字符串插值
来源：http://msu.hesvh.cn

"值: {$a}"
来源：http://ojl.fzhhl.top

[U58] PHP：数组三件套
来源：http://mku.yueranfly.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://peu.andypj.xyz

[U59] PHP：自定义排序
来源：http://rwe.hammf.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://itr.svipenyu.cn

[U60] PHP：JSON 编解码
来源：http://tph.bbcook.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cac.jinghuilouyu.cn

[U61] PHP：正则
来源：http://lmx.hysaishi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://iry.uphjek.com

[U62] PHP：日期对象
来源：http://nwy.sufxvd.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rkx.fanxiaobao.xyz

[U63] PHP：文件读写
来源：http://gsc.hammf.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fst.c1oappe.top

[U64] PHP：目录遍历
来源：http://ocr.0kj1m.cn

glob("dir/*.php");  scandir("dir");
来源：http://udh.jqgufenzy.top

[U65] PHP：会话
来源：http://loi.fengsongda.top

session_start();  $_SESSION["uid"] = 1;
来源：http://muj.tian-w.cn

[U66] PHP：设置 Cookie
来源：http://bpj.chenjidiqi.icu

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sny.xinyue.icu

[U67] PHP：处理文件上传
来源：http://ema.jinghuilouyu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qwx.dashuyun.cn

[U68] PHP：PDO 连接
来源：http://sng.wangdashe.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xqy.jinghuilouyu.cn

[U69] PHP：PDO 预处理
来源：http://ybx.xziqi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fsq.hongshengwenyu.top

[U70] PHP：PDO 事务
来源：http://tvn.hnqzz.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://chi.snrcjt.cn

[U71] PHP：抛出异常
来源：http://yeb.wangshuangyany.cn

throw new RuntimeException("失败", 500);
来源：http://luk.daxiang520.top

[U72] PHP：写错误日志
来源：http://nyb.quarkkingdee.top

error_log("失败: " . $e->getMessage());
来源：http://gxa.smart0.xyz

[U73] PHP：读取 ini 配置
来源：http://aol.mhx1999.top

parse_ini_file("config.ini", true)
来源：http://myj.chenlongwang.top

[U74] PHP：读取环境变量
来源：http://rwe.hesvh.cn

getenv("APP_ENV") ?: "production"
来源：http://vbv.sysykeji.top

[U75] PHP：依赖注入
来源：http://yzc.hesvh.cn

composer require psr/container
来源：http://rxl.fengsongda.top

[U76] PHP：简单路由
来源：http://cum.gotoacloud.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hfj.yvedp.cn

[U77] PHP：模板渲染
来源：http://wbb.shuidangran.top

composer require twig/twig
来源：http://hbs.havefunace.top

[U78] PHP：单元测试
来源：http://xhw.quarkkingdee.top

composer require --dev phpunit/phpunit
来源：http://kmk.zhiwuduotai.top

[U79] PHP：静态分析
来源：http://xcb.yuanzhike.top

composer require --dev phpstan/phpstan
来源：http://uyb.gogol.net.cn

[U80] PHP：代码规范修复
来源：http://ymh.jyoumei.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://xuv.tanke756.top

[U81] JS：初始化项目
来源：http://yrl.kuanghao11.cn

npm init -y;  npm i express
来源：http://lbl.yueranfly.top

[U82] JS：package.json 脚本
来源：http://cgl.daxiang520.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://dty.cdnleiting.top

[U83] JS：ES Module 导入导出
来源：http://hhz.shuidangran.top

export const a = 1;  import { a } from "./m.js";
来源：http://wsr.daxiang520.top

[U84] JS：CommonJS 写法
来源：http://hgi.vehdjk.com

module.exports = { a };  const { a } = require("./m");
来源：http://lpu.fktsv.cn

[U85] JS：可选链
来源：http://scw.tanke756.top

a?.b?.c
来源：http://fhx.redwolf501.top

[U86] JS：空值合并
来源：http://zwo.shuidangran.top

a ?? b
来源：http://fbl.smart0.xyz

[U87] JS：解构默认值
来源：http://jjr.zhixingplan.top

const { a = 1, b = 2 } = obj;
来源：http://ezk.bjfxy.top

[U88] JS：对象展开合并
来源：http://mup.nanxinkj.top

{ ...a, ...b }
来源：http://xgn.yangfankeji.com

[U89] JS：数组去重
来源：http://wqd.hcnkem.com

[...new Set(arr)]
来源：http://say.feifeiyinyue.top

[U90] JS：数字数组排序
来源：http://pjm.tarul.cn

[...arr].sort((a, b) => a - b)
来源：http://dke.sjlbkw.cn

[U91] JS：对象键值遍历
来源：http://isj.hywenlv.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rvm.ctjpmb.com

[U92] JS：深拷贝
来源：http://ttl.zhiwuduotai.top

structuredClone(obj)
来源：http://snu.sufxvd.cn

[U93] JS：模板字符串
来源：http://nxf.hfpthk.cn

`共 ${n} 条`
来源：http://pkn.hysaishi.cn

[U94] JS：箭头函数
来源：http://xhz.xziqi.cn

const double = x => x * 2;
来源：http://imm.tanke756.top

[U95] JS：Promise 包装
来源：http://cas.iojbl.cn

new Promise((resolve, reject) => {})
来源：http://isy.hcnkem.com

[U96] JS：async/await 与异常
来源：http://hao.fanxiaobao.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hre.cheryme.top

[U97] JS：并发请求
来源：http://wxi.dashuyun.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://qnf.tanke756.top

[U98] JS：fetch 带 JSON
来源：http://jym.cashguo.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ojz.guannengcc.top

[U99] JS：事件监听
来源：http://azd.xylfe.cn

el.addEventListener("click", e => {})
来源：http://zll.zhijiandao.cn

[U100] JS：DOM 查询
来源：http://wqk.mhx1999.top

document.querySelector(".item")
来源：http://mvw.zhaomingkeji.xyz

[U101] JS：classList 操作
来源：http://ajm.jinyuanbaomall.cn

el.classList.toggle("active")
来源：http://cay.fanxiaobao.xyz

[U102] JS：本地存储
来源：http://hhh.guannengcc.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://qtt.hfpthk.cn

[U103] JS：定时器
来源：http://mxm.ywan-chungtsiang.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nfi.nwbrower.top

[U104] JS：防抖
来源：http://vbp.uphjek.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gqq.sweek.top

[U105] JS：节流
来源：http://dsd.cucudq.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wpj.xinyue.icu

[U106] JS：日期格式化
来源：http://ely.jqgufenzy.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://tov.yvedp.cn

[U107] JS：数字千分位
来源：http://oph.tarul.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hqa.yanxiufei.cn

[U108] JS：随机整数
来源：http://ued.nwbrower.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kyg.nwbrower.top

[U109] JS：数组分组
来源：http://bqv.ywan-chungtsiang.top

Object.groupBy(arr, x => x.type)
来源：http://six.hfpthk.cn

[U110] JS：数组分块
来源：http://slu.zhengqikj.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kfj.shangyingyoupin.top

[U111] JS：对象转 Map
来源：http://iiw.xylfe.cn

new Map(Object.entries(obj))
来源：http://zla.jinqigufen.top

[U112] JS：字符串补位
来源：http://chp.sjlbkw.cn

"7".padStart(3, "0")
来源：http://vuf.meibo888.top

[U113] JS：正则替换全部
来源：http://zmd.chenjidiqi.icu

s.replaceAll("a", "b")
来源：http://rcg.xuetiantiany.cn

[U114] JS：JSON 深比较
来源：http://cig.zhoulong.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://scu.daria6918.cn

[U115] JS：生成 UUID
来源：http://nad.zhixingplan.top

crypto.randomUUID()
来源：http://rgo.xylfe.cn

[U116] JS：类型检查（JSDoc）
来源：http://hui.andypj.xyz

/** @param {string} name */ function f(name) {}
来源：http://mgt.cdnleiting.top

[U117] JS：单元测试
来源：http://xfq.dashuyun.cn

npm i -D vitest;  npx vitest
来源：http://pwy.dashuyun.cn

[U118] JS：开发服务器
来源：http://six.ybcxt.top

npm i -D vite;  npx vite
来源：http://nhq.hnxiangtu.top


<!-- 参考信息 -->