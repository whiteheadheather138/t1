代发 wailian999

[T33] Lua：表（数组）
来源：http://cdr.gzhubu.top

local t = {1, 2, 3};  t[4] = 4
来源：http://uju.pengpengdd.cyou

[T34] Lua：遍历表
来源：http://zzf.sweek.top

for i, v in ipairs(t) do print(i, v) end
来源：http://xid.ywan-chungtsiang.top

[T35] Lua：字典表
来源：http://bip.tanke756.top

local d = { a = 1 };  d.b = 2
来源：http://psh.yj20258888.top

[T36] Lua：函数
来源：http://idj.zdqjudy.top

function add(a, b) return a + b end
来源：http://dko.zhiwuduotai.top

[T37] Lua：字符串拼接
来源：http://hag.xuanzx.com

"a" .. "b"
来源：http://zhl.sweek.top

[T38] Lua：条件
来源：http://oiy.shangyingyoupin.top

if x > 0 then print("正") end
来源：http://fco.shanyushiyangtech.top

[T39] Lua：模式匹配
来源：http://str.jyoumei.cn

string.find(s, "%d+")
来源：http://ptz.yangfankeji.com

[T40] Lua：元表
来源：http://afm.shangyingyoupin.top

setmetatable({}, { __index = base })
来源：http://kkv.hongshengwenyu.top

[T41] Perl：Hello World
来源：http://gop.redwolf501.top

print "Hello\n";
来源：http://oth.yueranfly.top

[T42] Perl：变量类型
来源：http://oxv.hammf.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nhx.jinqigfzy.top

[T43] Perl：字符串插值
来源：http://rrn.sweek.top

"值: $a"
来源：http://khm.hnqzz.top

[T44] Perl：条件
来源：http://pep.yueranfly.top

if ($a > 0) { print "正"; }
来源：http://zqk.sjlbkw.cn

[T45] Perl：数组遍历
来源：http://idt.sufxvd.cn

for my $x (@arr) { print $x; }
来源：http://tgz.sufxvd.cn

[T46] Perl：哈希操作
来源：http://can.nwbrower.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://evi.nanxuanxn.top

[T47] Perl：正则捕获
来源：http://pco.chenlongwang.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://eum.quarkkingdee.top

[T48] Perl：正则替换
来源：http://kkn.yonumen.top

$s =~ s/old/new/g;
来源：http://wuv.havefunace.top

[T49] Perl：函数
来源：http://bht.daria6918.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yoa.pycfn.com

[T50] Perl：逐行读文件
来源：http://pvo.cucudq.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://vng.aibaodan.cn

while (my $line = <$fh>) { print $line; }
来源：http://flg.fktsv.cn

[T51] Scala：Hello World
来源：http://qky.pycfn.com

println("Hello")
来源：http://asd.tianlin.xyz

[T52] Scala：变量
来源：http://sez.shuidangran.top

val a = 1;  var b = 2
来源：http://dhh.smart0.xyz

[T53] Scala：字符串插值
来源：http://ixa.hywenlv.cn

s"值: $b"
来源：http://ohv.zhixingplan.top

[T54] Scala：集合映射
来源：http://mzj.cdnleiting.top

List(1, 2, 3).map(_ * 2)
来源：http://fpb.shanyushiyangkeji.top

[T55] Scala：集合过滤
来源：http://wae.yongpay.top

List(1, 2, 3).filter(_ > 1)
来源：http://cpo.jyoumei.cn

[T56] Scala：样例类
来源：http://wox.vehdjk.com

case class User(name: String, age: Int)
来源：http://xwm.hfpthk.cn

[T57] Scala：模式匹配
来源：http://qwm.fzhhl.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://cyw.shzxlz.cn

[T58] Scala：函数定义
来源：http://ybn.fengsongda.top

def add(a: Int, b: Int): Int = a + b
来源：http://zzl.zhongyouzk.top

[T59] Scala：循环
来源：http://htk.daxiang520.top

for (i <- 1 to 10) println(i)
来源：http://ist.bbcook.cn

[T60] Scala：折叠
来源：http://efs.fehbvm.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zam.zhongyouzk.top

================================================================================
来源：http://vxh.yfazqb.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xeg.zdqjudy.top

================================================================================
来源：http://nyt.redwolf501.top

[U01] Py：创建虚拟环境
来源：http://blj.meibo888.top

python -m venv .venv && source .venv/bin/activate
来源：http://upp.cqqwz.cn

[U02] Py：导出 / 安装依赖
来源：http://utl.daria6918.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://noy.shuidangran.top

[U03] Py：加载 .env 配置
来源：http://rbw.jyoumei.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://pon.gotoacloud.top

[U04] Py：变量调试打印
来源：http://tki.yuanzhike.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wjg.cheryme.top

[U05] Py：列表去重且保序
来源：http://hsa.yvedp.cn

list(dict.fromkeys(arr))
来源：http://tuq.dianchejie.cn

[U06] Py：合并两个字典
来源：http://cip.jinqigfzy.top

{**a, **b}
来源：http://yih.uphjek.com

[U07] Py：反转字典键值
来源：http://kjo.nwbrower.top

{v: k for k, v in d.items()}
来源：http://gkr.zhengqikj.top

[U08] Py：展平二维列表
来源：http://bax.chenzaomai.com

[y for x in nested for y in x]
来源：http://krc.ctjpmb.com

[U09] Py：字典取最大值的键
来源：http://vxp.quarkkingdee.top

max(d, key=d.get)
来源：http://xbv.9152youxi.cn

[U10] Py：按值排序字典
来源：http://fxk.hammf.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lik.ivvv.top

[U11] Py：生成器表达式
来源：http://vyw.jinqigfzy.top

(x * 2 for x in arr)
来源：http://cza.zhixingplan.top

[U12] Py：取出现最多的 3 个元素
来源：http://pmx.gotoacloud.top

Counter(arr).most_common(3)
来源：http://jnz.fengsongda.top

[U13] Py：固定长度队列
来源：http://xor.jinghuilouyu.cn

deque(maxlen=10)
来源：http://qiv.aizwys.cn

[U14] Py：分组收集到列表
来源：http://uhg.tianlin.xyz

defaultdict(list)
来源：http://lty.uphjek.com

[U15] Py：高精度计时
来源：http://kis.gzhubu.top

t = time.perf_counter()
来源：http://gox.xuetiantiany.cn

[U16] Py：命令行参数解析
来源：http://xxv.jinqigfzy.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://amu.yonumen.top

[U17] Py：初始化日志
来源：http://hli.quarkkingdee.top

logging.basicConfig(level=logging.INFO)
来源：http://ehd.chenjidiqi.icu

[U18] Py：预编译正则
来源：http://hal.xingfuxueyuan.xyz

pat = re.compile(r"\d+")
来源：http://enu.yuxming.cn

[U19] Py：正则替换带回调
来源：http://qus.zhijiandao.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hpm.jqgfzy.top

[U20] Py：缓存函数结果
来源：http://fex.xingfuxueyuan.xyz

@functools.lru_cache(maxsize=None)
来源：http://rpm.sxryk.cn

[U21] Py：自定义上下文管理器
来源：http://wsn.zhoulong.xyz

@contextlib.contextmanager
来源：http://jcc.quarkkingdee.top

[U22] Py：矩阵转置
来源：http://vdd.shanyushiyangtech.top

list(zip(*m))
来源：http://wmq.tarul.cn

[U23] Py：分块读取大文件
来源：http://kas.yvedp.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tzz.xinyue.icu

[U24] Py：路径操作
来源：http://lqr.chenlongwang.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://cmv.snrcjt.cn

[U25] Py：CSV 按字典读
来源：http://ohl.tianlin.xyz

csv.DictReader(f)
来源：http://zyk.xuetiantiany.cn

[U26] Py：并发下载
来源：http://sko.hongshengwenyu.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://big.fktsv.cn

[U27] Py：异步 HTTP
来源：http://hes.nwbrower.top

aiohttp.ClientSession() 配合 async with
来源：http://kya.fengsongda.top

[U28] Py：类型别名
来源：http://ckv.52xcode.cn

UserId = int
来源：http://apt.316326.xyz

[U29] Py：属性校验
来源：http://zfv.snrcjt.cn

@property 与 @x.setter 配合
来源：http://uem.feifeiyinyue.top

[U30] Py：数据类
来源：http://yxt.uphjek.com

@dataclass(slots=True)
来源：http://qpt.cqqwz.cn

[U31] Py：单测
来源：http://dfb.guannengcc.top

python -m pytest -q
来源：http://qxh.zhongyouzk.top

[U32] Py：代码格式化
来源：http://xyo.jinyuanbaomall.cn

ruff format . && ruff check --fix .
来源：http://ytm.ehwqpu.com

[U33] Py：打包发布
来源：http://rek.fktsv.cn

python -m build  （依赖 pyproject.toml）
来源：http://zvd.hongshengwenyu.top

[U34] Py：判断编码
来源：http://tgr.xylfe.cn

chardet.detect(raw)
来源：http://fjw.ybcxt.top

[U35] Py：发送邮件
来源：http://udd.sweek.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gfh.tarul.cn

[U36] Py：定时任务
来源：http://kaz.shuidangran.top

schedule.every(10).minutes.do(job)
来源：http://zct.xingfuxueyuan.xyz

[U37] Py：读写 Excel
来源：http://flv.quarkkingdee.top

pandas.read_excel / DataFrame.to_excel
来源：http://wik.shuidangran.top

[U38] Py：获取脚本所在目录
来源：http://rbe.guannengcc.top

Path(__file__).resolve().parent
来源：http://cma.yvedp.cn

[U39] Py：判断是否在交互环境
来源：http://anq.sweek.top

sys.stdout.isatty()
来源：http://ekl.redwolf501.top

[U40] Py：打印到标准错误
来源：http://ugv.yonumen.top

print("err", file=sys.stderr)
来源：http://ajg.sysykeji.top

[U41] PHP：初始化 Composer 项目
来源：http://pja.tanke756.top

composer init;  composer require guzzlehttp/guzzle
来源：http://nic.yfazqb.com

[U42] PHP：PSR-4 自动加载
来源：http://yxn.jinqigfzy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vgb.pycfn.com

[U43] PHP：声明命名空间
来源：http://pxk.hesvh.cn

namespace App\Http;
来源：http://ucr.ppjwa.cn

[U44] PHP：开启严格类型
来源：http://eba.svipenyu.cn

declare(strict_types=1);
来源：http://owg.chenzaomai.com

[U45] PHP：类型声明与返回类型
来源：http://gyo.jinyuanbaomall.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://llx.shanyushiyangkeji.top

[U46] PHP：可空类型
来源：http://krp.jinqigufen.top

?string $name = null
来源：http://rky.nanxinkj.top

[U47] PHP：联合类型
来源：http://nom.hywenlv.cn

int|string $id
来源：http://rzn.ctjpmb.com

[U48] PHP：纯枚举
来源：http://tol.feifeiyinyue.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vzl.svipenyu.cn

[U49] PHP：只读属性
来源：http://xdf.shuidangran.top

public readonly string $name
来源：http://kaq.birdmap.top

[U50] PHP：构造器属性提升
来源：http://fdq.meibo888.top

public function __construct(private int $id) {}
来源：http://ctc.ywan-chungtsiang.top

[U51] PHP：数组解构
来源：http://kev.sxryk.cn

[$a, $b] = $arr;
来源：http://yrd.316326.xyz

[U52] PHP：箭头函数
来源：http://cuf.chenlongwang.top

$double = fn($x) => $x * 2;
来源：http://byx.hysaishi.cn

[U53] PHP：空合并运算符
来源：http://vja.yj202588.top

$v = $a ?? $b ?? "default";
来源：http://ksb.zycfv.cn

[U54] PHP：空安全调用
来源：http://lkl.zhixingplan.top

$obj?->method()
来源：http://anl.fanxiaobao.xyz

[U55] PHP：match 表达式
来源：http://zho.cdnleiting.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://plk.shanyushiyangkeji.top

[U56] PHP：命名参数
来源：http://kyy.cashguo.top

f(a: 1, b: 2)
来源：http://bls.tarul.cn

[U57] PHP：字符串插值
来源：http://avz.shanyushiyangtech.top

"值: {$a}"
来源：http://dyu.fehbvm.com

[U58] PHP：数组三件套
来源：http://mqa.bbcook.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bnu.zycfv.cn

[U59] PHP：自定义排序
来源：http://lmn.zdbjq.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mpw.hongshengwenyu.top

[U60] PHP：JSON 编解码
来源：http://fbb.yangfankeji.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://brc.gzhubu.top

[U61] PHP：正则
来源：http://coi.jiagoushi.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://yjl.meibo888.top

[U62] PHP：日期对象
来源：http://qyj.ehwqpu.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ygx.yongpay.top

[U63] PHP：文件读写
来源：http://lub.guannengcc.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vle.ydjk.org.cn

[U64] PHP：目录遍历
来源：http://sxm.ydjk.org.cn

glob("dir/*.php");  scandir("dir");
来源：http://mwz.vehdjk.com

[U65] PHP：会话
来源：http://qjl.0kj1m.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://biz.jinqigufen.top

[U66] PHP：设置 Cookie
来源：http://ebt.bjfxy.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://znr.yj20258.top

[U67] PHP：处理文件上传
来源：http://dkc.zhoulong.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vjt.jinyuanbaomall.cn

[U68] PHP：PDO 连接
来源：http://agp.zhengqikj.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jyt.52xcode.cn

[U69] PHP：PDO 预处理
来源：http://ita.iojbl.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fdd.feifeiyinyue.top

[U70] PHP：PDO 事务
来源：http://dvv.yonumen.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fdl.pengpengdd.cyou

[U71] PHP：抛出异常
来源：http://njd.zycfv.cn

throw new RuntimeException("失败", 500);
来源：http://tun.guowangkeji.top

[U72] PHP：写错误日志
来源：http://opw.yanxiufei.cn

error_log("失败: " . $e->getMessage());
来源：http://rrg.smart0.xyz

[U73] PHP：读取 ini 配置
来源：http://oyg.cucudq.cn

parse_ini_file("config.ini", true)
来源：http://eho.cheryme.top

[U74] PHP：读取环境变量
来源：http://gtq.shanyushiyangkeji.top

getenv("APP_ENV") ?: "production"
来源：http://rhp.yuxming.cn

[U75] PHP：依赖注入
来源：http://eyh.havefunace.top

composer require psr/container
来源：http://jpl.jinqigufen.top

[U76] PHP：简单路由
来源：http://kum.chenjidiqi.icu

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mgb.smart0.xyz

[U77] PHP：模板渲染
来源：http://nga.yfazqb.com

composer require twig/twig
来源：http://dak.bbcook.cn

[U78] PHP：单元测试
来源：http://jwl.iojbl.cn

composer require --dev phpunit/phpunit
来源：http://jyh.shanyushiyangkeji.top

[U79] PHP：静态分析
来源：http://nvq.ehwqpu.com

composer require --dev phpstan/phpstan
来源：http://tlf.nanxuanxn.top

[U80] PHP：代码规范修复
来源：http://nph.shanyushiyangtech.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://qnl.shzxlz.cn

[U81] JS：初始化项目
来源：http://jcq.xuetiantiany.cn

npm init -y;  npm i express
来源：http://cpz.xziqi.cn

[U82] JS：package.json 脚本
来源：http://rqw.tanke756.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://emz.meibo888.top

[U83] JS：ES Module 导入导出
来源：http://rmm.smart0.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://xov.jinghuilouyu.cn

[U84] JS：CommonJS 写法
来源：http://xcm.jiagoushi.top

module.exports = { a };  const { a } = require("./m");
来源：http://jxp.hammf.cn

[U85] JS：可选链
来源：http://ylf.epnwcf.com

a?.b?.c
来源：http://suf.sufxvd.cn

[U86] JS：空值合并
来源：http://uqs.daria6918.cn

a ?? b
来源：http://wmo.gogol.net.cn

[U87] JS：解构默认值
来源：http://kah.zdqjudy.top

const { a = 1, b = 2 } = obj;
来源：http://brf.jinqigfzy.top

[U88] JS：对象展开合并
来源：http://okz.cashguo.top

{ ...a, ...b }
来源：http://pum.jinqigufen.top

[U89] JS：数组去重
来源：http://jnt.vqdsnc.cn

[...new Set(arr)]
来源：http://yjm.dashuyun.cn

[U90] JS：数字数组排序
来源：http://wup.pengpengdd.cyou

[...arr].sort((a, b) => a - b)
来源：http://doj.svipenyu.cn

[U91] JS：对象键值遍历
来源：http://igz.chenlongwang.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mrg.fanxiaobao.xyz

[U92] JS：深拷贝
来源：http://rnh.redwolf501.top

structuredClone(obj)
来源：http://mhy.hfpthk.cn

[U93] JS：模板字符串
来源：http://zea.9152youxi.cn

`共 ${n} 条`
来源：http://bou.hywenlv.cn

[U94] JS：箭头函数
来源：http://gxw.chenjidiqi.icu

const double = x => x * 2;
来源：http://qfu.sweek.top

[U95] JS：Promise 包装
来源：http://oqx.jiagoushi.top

new Promise((resolve, reject) => {})
来源：http://ein.chenlongwang.top

[U96] JS：async/await 与异常
来源：http://ook.sweek.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://avi.hywenlv.cn

[U97] JS：并发请求
来源：http://gcs.aibaodan.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://zxp.ywan-chungtsiang.top

[U98] JS：fetch 带 JSON
来源：http://dcc.xuetiantiany.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://suk.wangdashe.top

[U99] JS：事件监听
来源：http://dgl.cucudq.cn

el.addEventListener("click", e => {})
来源：http://wjm.iojbl.cn

[U100] JS：DOM 查询
来源：http://gji.hywenlv.cn

document.querySelector(".item")
来源：http://cxv.shuidangran.top

[U101] JS：classList 操作
来源：http://pzf.yangfankeji.com

el.classList.toggle("active")
来源：http://xgu.xuetiantiany.cn

[U102] JS：本地存储
来源：http://gho.sxryk.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://qwc.xylfe.cn

[U103] JS：定时器
来源：http://cfh.yonumen.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ekh.chenlongwang.top

[U104] JS：防抖
来源：http://gog.jqgfzy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ijw.zycfv.cn

[U105] JS：节流
来源：http://orr.hfpthk.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dus.cashguo.top

[U106] JS：日期格式化
来源：http://zqi.gzhubu.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ydk.0kj1m.cn

[U107] JS：数字千分位
来源：http://rqc.hcnkem.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://tda.jqgfzy.top

[U108] JS：随机整数
来源：http://mvd.yonumen.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wqr.hnxiangtu.top

[U109] JS：数组分组
来源：http://guc.xingfuxueyuan.xyz

Object.groupBy(arr, x => x.type)
来源：http://hil.smart0.xyz

[U110] JS：数组分块
来源：http://zms.xziqi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://acz.vqdsnc.cn

[U111] JS：对象转 Map
来源：http://klb.hnxiangtu.top

new Map(Object.entries(obj))
来源：http://bgr.birdmap.top

[U112] JS：字符串补位
来源：http://jfe.jqgufenzy.top

"7".padStart(3, "0")
来源：http://wfo.yuxming.cn

[U113] JS：正则替换全部
来源：http://gal.zhiwuduotai.top

s.replaceAll("a", "b")
来源：http://rhu.gaohongyu789.top

[U114] JS：JSON 深比较
来源：http://wew.jiagoushi.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ruh.cheryme.top

[U115] JS：生成 UUID
来源：http://gir.kuanghao11.cn

crypto.randomUUID()
来源：http://kyp.hysaishi.cn

[U116] JS：类型检查（JSDoc）
来源：http://vqs.yvedp.cn

/** @param {string} name */ function f(name) {}
来源：http://ttu.dashuyun.cn

[U117] JS：单元测试
来源：http://zui.vehdjk.com

npm i -D vitest;  npx vitest
来源：http://mnr.52xcode.cn

[U118] JS：开发服务器
来源：http://jmu.xziqi.cn

npm i -D vite;  npx vite
来源：http://apf.zhengqikj.top

[U119] JS：生产构建
来源：http://toy.yuanzhike.top

npx vite build
来源：http://whw.yangfankeji.com

[U120] JS：读取环境变量（Vite）
来源：http://jze.yonumen.top

import.meta.env.VITE_API_URL
来源：http://yio.xuetiantiany.cn


<!-- 参考信息 -->