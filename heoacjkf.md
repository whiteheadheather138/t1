代发 wailian999

[T39] Lua：模式匹配
来源：http://wky.epnwcf.com

string.find(s, "%d+")
来源：http://vse.xinyue.icu

[T40] Lua：元表
来源：http://wku.fengsongda.top

setmetatable({}, { __index = base })
来源：http://aep.quarkkingdee.top

[T41] Perl：Hello World
来源：http://cdf.yuxming.cn

print "Hello\n";
来源：http://ujr.hesvh.cn

[T42] Perl：变量类型
来源：http://how.sufxvd.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tmq.shangyingyoupin.top

[T43] Perl：字符串插值
来源：http://qxf.vqdsnc.cn

"值: $a"
来源：http://xtc.svipenyu.cn

[T44] Perl：条件
来源：http://uah.yj20258.top

if ($a > 0) { print "正"; }
来源：http://ond.jyoumei.cn

[T45] Perl：数组遍历
来源：http://otg.aizwys.cn

for my $x (@arr) { print $x; }
来源：http://uhs.pengpengdd.cyou

[T46] Perl：哈希操作
来源：http://jqd.jinqigfzy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://neo.c1oappe.top

[T47] Perl：正则捕获
来源：http://xjp.zhijiandao.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://jhp.jyoumei.cn

[T48] Perl：正则替换
来源：http://lfw.nanxinkj.top

$s =~ s/old/new/g;
来源：http://jku.zhiwuduotai.top

[T49] Perl：函数
来源：http://tlc.ehwqpu.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wah.gogol.net.cn

[T50] Perl：逐行读文件
来源：http://adg.nanxinkj.top

open my $fh, "<", "a.txt" or die $!;
来源：http://hlv.9152youxi.cn

while (my $line = <$fh>) { print $line; }
来源：http://rhn.sufxvd.cn

[T51] Scala：Hello World
来源：http://ekz.xingfuxueyuan.xyz

println("Hello")
来源：http://fsc.tanke756.top

[T52] Scala：变量
来源：http://wxo.yj20258888.top

val a = 1;  var b = 2
来源：http://nbs.fanxiaobao.xyz

[T53] Scala：字符串插值
来源：http://ifs.chenjidiqi.icu

s"值: $b"
来源：http://udk.snrcjt.cn

[T54] Scala：集合映射
来源：http://xom.fengsongda.top

List(1, 2, 3).map(_ * 2)
来源：http://ohl.snrcjt.cn

[T55] Scala：集合过滤
来源：http://fty.cdnleiting.top

List(1, 2, 3).filter(_ > 1)
来源：http://loq.zhongyouzk.top

[T56] Scala：样例类
来源：http://dhg.yfazqb.com

case class User(name: String, age: Int)
来源：http://grt.fanxiaobao.xyz

[T57] Scala：模式匹配
来源：http://dcv.nanxuanxn.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://zhf.snrcjt.cn

[T58] Scala：函数定义
来源：http://jtg.9152youxi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://tkp.shanyushiyangtech.top

[T59] Scala：循环
来源：http://lgx.yanxiufei.cn

for (i <- 1 to 10) println(i)
来源：http://pyu.sweek.top

[T60] Scala：折叠
来源：http://fgd.hammf.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://eig.aizwys.cn

================================================================================
来源：http://xdn.jyoumei.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ubw.uphjek.com

================================================================================
来源：http://ocq.hongshengwenyu.top

[U01] Py：创建虚拟环境
来源：http://uvc.sufxvd.cn

python -m venv .venv && source .venv/bin/activate
来源：http://spx.nwbrower.top

[U02] Py：导出 / 安装依赖
来源：http://amw.shangyingyoupin.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fjy.feifeiyinyue.top

[U03] Py：加载 .env 配置
来源：http://koy.feifeiyinyue.top

from dotenv import load_dotenv; load_dotenv()
来源：http://sqo.uphjek.com

[U04] Py：变量调试打印
来源：http://dym.yfazqb.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jhq.hnqzz.top

[U05] Py：列表去重且保序
来源：http://okg.gotoacloud.top

list(dict.fromkeys(arr))
来源：http://pli.snrcjt.cn

[U06] Py：合并两个字典
来源：http://qmn.ctjpmb.com

{**a, **b}
来源：http://afp.pycfn.com

[U07] Py：反转字典键值
来源：http://ylc.hongshengwenyu.top

{v: k for k, v in d.items()}
来源：http://jyp.hywenlv.cn

[U08] Py：展平二维列表
来源：http://hju.yj20258888.top

[y for x in nested for y in x]
来源：http://zub.ybcxt.top

[U09] Py：字典取最大值的键
来源：http://rwu.hnxiangtu.top

max(d, key=d.get)
来源：http://eie.jinqigufen.top

[U10] Py：按值排序字典
来源：http://ddh.gaohongyu789.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qmp.ydjk.org.cn

[U11] Py：生成器表达式
来源：http://gnr.hnxiangtu.top

(x * 2 for x in arr)
来源：http://oog.daria6918.cn

[U12] Py：取出现最多的 3 个元素
来源：http://dnr.yangfankeji.com

Counter(arr).most_common(3)
来源：http://vll.yongpay.top

[U13] Py：固定长度队列
来源：http://vdj.daxiang520.top

deque(maxlen=10)
来源：http://lob.jyoumei.cn

[U14] Py：分组收集到列表
来源：http://vhr.guowangkeji.top

defaultdict(list)
来源：http://ywd.hnxiangtu.top

[U15] Py：高精度计时
来源：http://qnv.shangyingyoupin.top

t = time.perf_counter()
来源：http://ewh.redwolf501.top

[U16] Py：命令行参数解析
来源：http://eze.sweek.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ijs.yj202588.top

[U17] Py：初始化日志
来源：http://xkr.guowangkeji.top

logging.basicConfig(level=logging.INFO)
来源：http://rev.pengpengdd.cyou

[U18] Py：预编译正则
来源：http://iol.jiagoushi.top

pat = re.compile(r"\d+")
来源：http://qpm.iojbl.cn

[U19] Py：正则替换带回调
来源：http://iqz.haohaochexian.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wkz.tianlin.xyz

[U20] Py：缓存函数结果
来源：http://jeo.epnwcf.com

@functools.lru_cache(maxsize=None)
来源：http://gch.sxryk.cn

[U21] Py：自定义上下文管理器
来源：http://wyb.yvedp.cn

@contextlib.contextmanager
来源：http://mye.pycfn.com

[U22] Py：矩阵转置
来源：http://nqy.316326.xyz

list(zip(*m))
来源：http://uam.316326.xyz

[U23] Py：分块读取大文件
来源：http://aex.zdqjudy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://djm.wangdashe.top

[U24] Py：路径操作
来源：http://fjh.bbcook.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rrl.xuetiantiany.cn

[U25] Py：CSV 按字典读
来源：http://ajp.zhengqikj.top

csv.DictReader(f)
来源：http://htf.9152youxi.cn

[U26] Py：并发下载
来源：http://vlk.gogol.net.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://eds.zhiwuduotai.top

[U27] Py：异步 HTTP
来源：http://jqn.smart0.xyz

aiohttp.ClientSession() 配合 async with
来源：http://tji.nwbrower.top

[U28] Py：类型别名
来源：http://hcu.shanyushiyangkeji.top

UserId = int
来源：http://phr.yj202588.top

[U29] Py：属性校验
来源：http://vtb.bbcook.cn

@property 与 @x.setter 配合
来源：http://wfq.nanxinkj.top

[U30] Py：数据类
来源：http://nzk.jinyuanbaomall.cn

@dataclass(slots=True)
来源：http://tot.svipenyu.cn

[U31] Py：单测
来源：http://xej.sufxvd.cn

python -m pytest -q
来源：http://jme.havefunace.top

[U32] Py：代码格式化
来源：http://uiw.sxryk.cn

ruff format . && ruff check --fix .
来源：http://ywa.ehwqpu.com

[U33] Py：打包发布
来源：http://osi.zdbjq.cn

python -m build  （依赖 pyproject.toml）
来源：http://nqv.jqgfzy.top

[U34] Py：判断编码
来源：http://qzz.kuanghao11.cn

chardet.detect(raw)
来源：http://ivz.ivvv.top

[U35] Py：发送邮件
来源：http://ymp.meibo888.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gsc.yongpay.top

[U36] Py：定时任务
来源：http://mvm.ivvv.top

schedule.every(10).minutes.do(job)
来源：http://mht.bbcook.cn

[U37] Py：读写 Excel
来源：http://jkp.smart0.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://mzq.gotoacloud.top

[U38] Py：获取脚本所在目录
来源：http://lxy.chenjidiqi.icu

Path(__file__).resolve().parent
来源：http://yni.chenlongwang.top

[U39] Py：判断是否在交互环境
来源：http://ddx.shangyingyoupin.top

sys.stdout.isatty()
来源：http://rux.nanxuanxn.top

[U40] Py：打印到标准错误
来源：http://guv.cqqwz.cn

print("err", file=sys.stderr)
来源：http://jrx.nanxuanxn.top

[U41] PHP：初始化 Composer 项目
来源：http://tfp.jlsjyb.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://zzl.jinqigfzy.top

[U42] PHP：PSR-4 自动加载
来源：http://odg.zhaomingkeji.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://weo.yuxming.cn

[U43] PHP：声明命名空间
来源：http://mth.vehdjk.com

namespace App\Http;
来源：http://apt.sufxvd.cn

[U44] PHP：开启严格类型
来源：http://vvy.zhaomingkeji.xyz

declare(strict_types=1);
来源：http://wzj.jqgfzy.top

[U45] PHP：类型声明与返回类型
来源：http://glc.andypj.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://lgb.iojbl.cn

[U46] PHP：可空类型
来源：http://tcr.zycfv.cn

?string $name = null
来源：http://llw.zdqjudy.top

[U47] PHP：联合类型
来源：http://fml.cdnleiting.top

int|string $id
来源：http://ivo.ydjk.org.cn

[U48] PHP：纯枚举
来源：http://ygw.ehwqpu.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wgg.pycfn.com

[U49] PHP：只读属性
来源：http://wjm.aibaodan.cn

public readonly string $name
来源：http://zjn.c1oappe.top

[U50] PHP：构造器属性提升
来源：http://fgj.tanke756.top

public function __construct(private int $id) {}
来源：http://dhz.tanke756.top

[U51] PHP：数组解构
来源：http://vqh.gogol.net.cn

[$a, $b] = $arr;
来源：http://obu.jqgfzy.top

[U52] PHP：箭头函数
来源：http://vqy.cucudq.cn

$double = fn($x) => $x * 2;
来源：http://oox.mhx1999.top

[U53] PHP：空合并运算符
来源：http://btc.gogol.net.cn

$v = $a ?? $b ?? "default";
来源：http://aol.hammf.cn

[U54] PHP：空安全调用
来源：http://ljg.xuanzx.com

$obj?->method()
来源：http://nns.jqgfzy.top

[U55] PHP：match 表达式
来源：http://vok.gzhubu.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rsa.yangfankeji.com

[U56] PHP：命名参数
来源：http://jmw.nanxinkj.top

f(a: 1, b: 2)
来源：http://mfh.c1oappe.top

[U57] PHP：字符串插值
来源：http://oyb.cqqwz.cn

"值: {$a}"
来源：http://ciu.zdbjq.cn

[U58] PHP：数组三件套
来源：http://tzt.mhx1999.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ygg.zhiwuduotai.top

[U59] PHP：自定义排序
来源：http://pqt.ehwqpu.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bum.bbcook.cn

[U60] PHP：JSON 编解码
来源：http://njf.fktsv.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ebz.sjlbkw.cn

[U61] PHP：正则
来源：http://oip.ywan-chungtsiang.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ujb.guannengcc.top

[U62] PHP：日期对象
来源：http://gmj.yanxiufei.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pvq.yj20258.top

[U63] PHP：文件读写
来源：http://fvg.cucudq.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://cab.cqqwz.cn

[U64] PHP：目录遍历
来源：http://rgk.xingfuxueyuan.xyz

glob("dir/*.php");  scandir("dir");
来源：http://ugj.jqgfzy.top

[U65] PHP：会话
来源：http://mxl.hcnkem.com

session_start();  $_SESSION["uid"] = 1;
来源：http://rjb.yuanzhike.top

[U66] PHP：设置 Cookie
来源：http://rsx.zycfv.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mpn.shanyushiyangtech.top

[U67] PHP：处理文件上传
来源：http://ynl.ehwqpu.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ndh.tian-w.cn

[U68] PHP：PDO 连接
来源：http://mpe.feifeiyinyue.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rvf.52xcode.cn

[U69] PHP：PDO 预处理
来源：http://alp.jqgufenzy.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qzc.bbcook.cn

[U70] PHP：PDO 事务
来源：http://dgd.daria6918.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ljo.chenjidiqi.icu

[U71] PHP：抛出异常
来源：http://qmw.52xcode.cn

throw new RuntimeException("失败", 500);
来源：http://ptl.svipenyu.cn

[U72] PHP：写错误日志
来源：http://oho.yongpay.top

error_log("失败: " . $e->getMessage());
来源：http://spr.9152youxi.cn

[U73] PHP：读取 ini 配置
来源：http://urd.fktsv.cn

parse_ini_file("config.ini", true)
来源：http://opz.bbcook.cn

[U74] PHP：读取环境变量
来源：http://sch.jqgufenzy.top

getenv("APP_ENV") ?: "production"
来源：http://rnf.smart0.xyz

[U75] PHP：依赖注入
来源：http://vrn.nwbrower.top

composer require psr/container
来源：http://lew.tanke756.top

[U76] PHP：简单路由
来源：http://dir.hysaishi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://swx.nanxuanxn.top

[U77] PHP：模板渲染
来源：http://jpf.quarkkingdee.top

composer require twig/twig
来源：http://ppn.jinqigufen.top

[U78] PHP：单元测试
来源：http://jsw.fzhhl.top

composer require --dev phpunit/phpunit
来源：http://rog.shanyushiyangkeji.top

[U79] PHP：静态分析
来源：http://vlc.cheryme.top

composer require --dev phpstan/phpstan
来源：http://czf.fanxiaobao.xyz

[U80] PHP：代码规范修复
来源：http://yvf.jinqigfzy.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://jhd.yonumen.top

[U81] JS：初始化项目
来源：http://zdu.epnwcf.com

npm init -y;  npm i express
来源：http://eeu.gotoacloud.top

[U82] JS：package.json 脚本
来源：http://lqg.guannengcc.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fnp.feifeiyinyue.top

[U83] JS：ES Module 导入导出
来源：http://jlg.zdbjq.cn

export const a = 1;  import { a } from "./m.js";
来源：http://agl.316326.xyz

[U84] JS：CommonJS 写法
来源：http://jrg.cqqwz.cn

module.exports = { a };  const { a } = require("./m");
来源：http://jnt.tanke756.top

[U85] JS：可选链
来源：http://btp.ctjpmb.com

a?.b?.c
来源：http://ran.dashuyun.cn

[U86] JS：空值合并
来源：http://yeb.smart0.xyz

a ?? b
来源：http://pkg.cdnleiting.top

[U87] JS：解构默认值
来源：http://eso.jqgfzy.top

const { a = 1, b = 2 } = obj;
来源：http://mtf.yangfankeji.com

[U88] JS：对象展开合并
来源：http://wkm.daxiang520.top

{ ...a, ...b }
来源：http://new.zdbjq.cn

[U89] JS：数组去重
来源：http://dng.mhx1999.top

[...new Set(arr)]
来源：http://voe.bbcook.cn

[U90] JS：数字数组排序
来源：http://nwh.fzhhl.top

[...arr].sort((a, b) => a - b)
来源：http://qsa.shuidangran.top

[U91] JS：对象键值遍历
来源：http://cyt.jinqigfzy.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gie.gaohongyu789.top

[U92] JS：深拷贝
来源：http://kxr.hammf.cn

structuredClone(obj)
来源：http://xhb.daria6918.cn

[U93] JS：模板字符串
来源：http://lqq.dianchejie.cn

`共 ${n} 条`
来源：http://plv.vqdsnc.cn

[U94] JS：箭头函数
来源：http://xkf.daxiang520.top

const double = x => x * 2;
来源：http://zcr.snrcjt.cn

[U95] JS：Promise 包装
来源：http://oyf.xinyue.icu

new Promise((resolve, reject) => {})
来源：http://bqk.xziqi.cn

[U96] JS：async/await 与异常
来源：http://poa.ydzc1.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qiy.yuanzhike.top

[U97] JS：并发请求
来源：http://cpd.zhixingplan.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ybw.yueranfly.top

[U98] JS：fetch 带 JSON
来源：http://mdv.guowangkeji.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cya.chenzaomai.com

[U99] JS：事件监听
来源：http://ywv.shanyushiyangtech.top

el.addEventListener("click", e => {})
来源：http://xfb.xuetiantiany.cn

[U100] JS：DOM 查询
来源：http://erm.fktsv.cn

document.querySelector(".item")
来源：http://njj.cucudq.cn

[U101] JS：classList 操作
来源：http://mfk.gaohongyu789.top

el.classList.toggle("active")
来源：http://bpy.andypj.xyz

[U102] JS：本地存储
来源：http://hpi.cucudq.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://lpy.fktsv.cn

[U103] JS：定时器
来源：http://pmb.ctjpmb.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lwh.zhiwuduotai.top

[U104] JS：防抖
来源：http://yqn.shanyushiyangkeji.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dke.fktsv.cn

[U105] JS：节流
来源：http://wns.yvedp.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://knb.zhijiandao.cn

[U106] JS：日期格式化
来源：http://itw.cucudq.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://trs.xziqi.cn

[U107] JS：数字千分位
来源：http://lbg.shuidangran.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ekh.c1oappe.top

[U108] JS：随机整数
来源：http://tbf.jlsjyb.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ble.andypj.xyz

[U109] JS：数组分组
来源：http://kef.yj20258.top

Object.groupBy(arr, x => x.type)
来源：http://wxo.yonumen.top

[U110] JS：数组分块
来源：http://qjz.cdnleiting.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://uwu.tanke756.top

[U111] JS：对象转 Map
来源：http://bub.mhx1999.top

new Map(Object.entries(obj))
来源：http://jty.ydzc1.top

[U112] JS：字符串补位
来源：http://reb.shanyushiyangkeji.top

"7".padStart(3, "0")
来源：http://wmf.52xcode.cn

[U113] JS：正则替换全部
来源：http://aks.aizwys.cn

s.replaceAll("a", "b")
来源：http://myx.zhaomingkeji.xyz

[U114] JS：JSON 深比较
来源：http://spy.shangyingyoupin.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://shx.ctjpmb.com

[U115] JS：生成 UUID
来源：http://swz.yongpay.top

crypto.randomUUID()
来源：http://yii.hysaishi.cn

[U116] JS：类型检查（JSDoc）
来源：http://phw.shuidangran.top

/** @param {string} name */ function f(name) {}
来源：http://mzv.redwolf501.top

[U117] JS：单元测试
来源：http://hsz.hnxiangtu.top

npm i -D vitest;  npx vitest
来源：http://hfc.cdnleiting.top

[U118] JS：开发服务器
来源：http://efv.cdnleiting.top

npm i -D vite;  npx vite
来源：http://tgj.ivvv.top

[U119] JS：生产构建
来源：http://djr.hysaishi.cn

npx vite build
来源：http://smk.guowangkeji.top

[U120] JS：读取环境变量（Vite）
来源：http://flr.yj202588.top

import.meta.env.VITE_API_URL
来源：http://ptf.jinqigufen.top

================================================================================
来源：http://zhm.gaohongyu789.top

统计汇总
来源：http://dwj.wangdashe.top

================================================================================
来源：http://yhl.yongpay.top

按语言统计（条）：
来源：http://unx.sweek.top

Python ......... 252
来源：http://xwd.jinghuilouyu.cn

PHP ............ 252
来源：http://ugy.ehwqpu.com

JavaScript ..... 252
来源：http://tyx.cqqwz.cn

TypeScript ..... 212
来源：http://tgy.fehbvm.com

Java ........... 212
来源：http://gws.tianlin.xyz

Go ............. 212
来源：http://ztj.iojbl.cn

Ruby ........... 212
来源：http://xlc.andypj.xyz

C# ............. 212
来源：http://fah.nanxuanxn.top


<!-- 参考信息 -->