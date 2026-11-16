代发 wailian999

[T39] Lua：模式匹配
来源：http://vxo.yuanzhike.top

string.find(s, "%d+")
来源：http://hhq.ctjpmb.com

[T40] Lua：元表
来源：http://vvb.aizwys.cn

setmetatable({}, { __index = base })
来源：http://xjt.cdnleiting.top

[T41] Perl：Hello World
来源：http://drt.sweek.top

print "Hello\n";
来源：http://kup.zhengqikj.top

[T42] Perl：变量类型
来源：http://syc.sjlbkw.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qwd.tanke756.top

[T43] Perl：字符串插值
来源：http://vit.shangyingyoupin.top

"值: $a"
来源：http://ftt.jiagoushi.top

[T44] Perl：条件
来源：http://zlv.jinyuanbaomall.cn

if ($a > 0) { print "正"; }
来源：http://tba.yvedp.cn

[T45] Perl：数组遍历
来源：http://ivu.xuanzx.com

for my $x (@arr) { print $x; }
来源：http://ubf.pycfn.com

[T46] Perl：哈希操作
来源：http://nwn.hesvh.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bzz.316326.xyz

[T47] Perl：正则捕获
来源：http://fzi.shangyingyoupin.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://zba.xuanzx.com

[T48] Perl：正则替换
来源：http://aso.redwolf501.top

$s =~ s/old/new/g;
来源：http://hzz.fzhhl.top

[T49] Perl：函数
来源：http://wcn.zhengqikj.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://auz.hammf.cn

[T50] Perl：逐行读文件
来源：http://juc.guannengcc.top

open my $fh, "<", "a.txt" or die $!;
来源：http://bkm.bbcook.cn

while (my $line = <$fh>) { print $line; }
来源：http://usi.fktsv.cn

[T51] Scala：Hello World
来源：http://las.wangdashe.top

println("Hello")
来源：http://lwz.wangdashe.top

[T52] Scala：变量
来源：http://emq.shzxlz.cn

val a = 1;  var b = 2
来源：http://kiy.hcnkem.com

[T53] Scala：字符串插值
来源：http://slv.meibo888.top

s"值: $b"
来源：http://hhk.havefunace.top

[T54] Scala：集合映射
来源：http://igt.ivvv.top

List(1, 2, 3).map(_ * 2)
来源：http://gvp.chenzaomai.com

[T55] Scala：集合过滤
来源：http://gkb.yj20258888.top

List(1, 2, 3).filter(_ > 1)
来源：http://kyu.hysaishi.cn

[T56] Scala：样例类
来源：http://sei.gzhubu.top

case class User(name: String, age: Int)
来源：http://ver.ehwqpu.com

[T57] Scala：模式匹配
来源：http://jmu.c1oappe.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://lew.shanyushiyangkeji.top

[T58] Scala：函数定义
来源：http://tan.zdqjudy.top

def add(a: Int, b: Int): Int = a + b
来源：http://xyo.kuanghao11.cn

[T59] Scala：循环
来源：http://uwp.ydzc1.top

for (i <- 1 to 10) println(i)
来源：http://hvg.fehbvm.com

[T60] Scala：折叠
来源：http://psx.sufxvd.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blo.fzhhl.top

================================================================================
来源：http://jaz.sufxvd.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://put.sysykeji.top

================================================================================
来源：http://wfa.daxiang520.top

[U01] Py：创建虚拟环境
来源：http://uhg.jinyuanbaomall.cn

python -m venv .venv && source .venv/bin/activate
来源：http://zid.yanxiufei.cn

[U02] Py：导出 / 安装依赖
来源：http://ytv.dianchejie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gfi.fzhhl.top

[U03] Py：加载 .env 配置
来源：http://zwk.wangshuangyany.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://nsi.hnqzz.top

[U04] Py：变量调试打印
来源：http://ubz.yueranfly.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://imh.cucudq.cn

[U05] Py：列表去重且保序
来源：http://vcu.zhengqikj.top

list(dict.fromkeys(arr))
来源：http://zge.ywan-chungtsiang.top

[U06] Py：合并两个字典
来源：http://zoo.jqgufenzy.top

{**a, **b}
来源：http://ptq.meibo888.top

[U07] Py：反转字典键值
来源：http://sbe.zhiwuduotai.top

{v: k for k, v in d.items()}
来源：http://tgb.sxryk.cn

[U08] Py：展平二维列表
来源：http://xel.cashguo.top

[y for x in nested for y in x]
来源：http://zfc.guowangkeji.top

[U09] Py：字典取最大值的键
来源：http://wxu.shanyushiyangtech.top

max(d, key=d.get)
来源：http://gxy.jinghuilouyu.cn

[U10] Py：按值排序字典
来源：http://nrv.hcnkem.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://heu.shuidangran.top

[U11] Py：生成器表达式
来源：http://eip.fzhhl.top

(x * 2 for x in arr)
来源：http://qox.guowangkeji.top

[U12] Py：取出现最多的 3 个元素
来源：http://peh.dianchejie.cn

Counter(arr).most_common(3)
来源：http://rof.ivvv.top

[U13] Py：固定长度队列
来源：http://npl.vehdjk.com

deque(maxlen=10)
来源：http://szk.ydjk.org.cn

[U14] Py：分组收集到列表
来源：http://aaz.yj20258.top

defaultdict(list)
来源：http://hzi.dashuyun.cn

[U15] Py：高精度计时
来源：http://rzz.shangyingyoupin.top

t = time.perf_counter()
来源：http://oyj.mhx1999.top

[U16] Py：命令行参数解析
来源：http://wjo.aizwys.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jrd.daria6918.cn

[U17] Py：初始化日志
来源：http://qmy.hammf.cn

logging.basicConfig(level=logging.INFO)
来源：http://bgb.jyoumei.cn

[U18] Py：预编译正则
来源：http://vtw.yuanzhike.top

pat = re.compile(r"\d+")
来源：http://nch.daria6918.cn

[U19] Py：正则替换带回调
来源：http://uib.dashuyun.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://khe.shanyushiyangkeji.top

[U20] Py：缓存函数结果
来源：http://mrb.gogol.net.cn

@functools.lru_cache(maxsize=None)
来源：http://bzo.yuanzhike.top

[U21] Py：自定义上下文管理器
来源：http://qgp.nanxuanxn.top

@contextlib.contextmanager
来源：http://kzu.xziqi.cn

[U22] Py：矩阵转置
来源：http://gea.ybcxt.top

list(zip(*m))
来源：http://vma.yvedp.cn

[U23] Py：分块读取大文件
来源：http://gad.pycfn.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fxx.feifeiyinyue.top

[U24] Py：路径操作
来源：http://cuw.guowangkeji.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://akm.hammf.cn

[U25] Py：CSV 按字典读
来源：http://qut.sjlbkw.cn

csv.DictReader(f)
来源：http://awo.iojbl.cn

[U26] Py：并发下载
来源：http://vtm.zhijiandao.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://eex.vqdsnc.cn

[U27] Py：异步 HTTP
来源：http://qup.jinqigfzy.top

aiohttp.ClientSession() 配合 async with
来源：http://mhy.meibo888.top

[U28] Py：类型别名
来源：http://olj.cqqwz.cn

UserId = int
来源：http://pzj.dashuyun.cn

[U29] Py：属性校验
来源：http://qay.mhx1999.top

@property 与 @x.setter 配合
来源：http://vjk.shangyingyoupin.top

[U30] Py：数据类
来源：http://qfq.yanxiufei.cn

@dataclass(slots=True)
来源：http://gfz.quarkkingdee.top

[U31] Py：单测
来源：http://viz.hfpthk.cn

python -m pytest -q
来源：http://kkv.9152youxi.cn

[U32] Py：代码格式化
来源：http://jfj.snrcjt.cn

ruff format . && ruff check --fix .
来源：http://qhi.9152youxi.cn

[U33] Py：打包发布
来源：http://uvo.cucudq.cn

python -m build  （依赖 pyproject.toml）
来源：http://poa.hysaishi.cn

[U34] Py：判断编码
来源：http://qle.xingfuxueyuan.xyz

chardet.detect(raw)
来源：http://mon.yongpay.top

[U35] Py：发送邮件
来源：http://hfg.hammf.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bhy.cqqwz.cn

[U36] Py：定时任务
来源：http://cdq.sysykeji.top

schedule.every(10).minutes.do(job)
来源：http://ybq.gzhubu.top

[U37] Py：读写 Excel
来源：http://xaq.zhixingplan.top

pandas.read_excel / DataFrame.to_excel
来源：http://nkr.sjlbkw.cn

[U38] Py：获取脚本所在目录
来源：http://mfk.cashguo.top

Path(__file__).resolve().parent
来源：http://dec.yanxiufei.cn

[U39] Py：判断是否在交互环境
来源：http://xbs.sufxvd.cn

sys.stdout.isatty()
来源：http://bdd.vqdsnc.cn

[U40] Py：打印到标准错误
来源：http://cnv.dianchejie.cn

print("err", file=sys.stderr)
来源：http://lkf.xziqi.cn

[U41] PHP：初始化 Composer 项目
来源：http://lmh.shanyushiyangtech.top

composer init;  composer require guzzlehttp/guzzle
来源：http://llp.meibo888.top

[U42] PHP：PSR-4 自动加载
来源：http://wsg.yongpay.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nsv.bbcook.cn

[U43] PHP：声明命名空间
来源：http://cod.sxryk.cn

namespace App\Http;
来源：http://hbd.sufxvd.cn

[U44] PHP：开启严格类型
来源：http://adr.jqgufenzy.top

declare(strict_types=1);
来源：http://nen.snrcjt.cn

[U45] PHP：类型声明与返回类型
来源：http://zkv.yueranfly.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://foe.zhiwuduotai.top

[U46] PHP：可空类型
来源：http://fwv.jqgfzy.top

?string $name = null
来源：http://hpa.yuxming.cn

[U47] PHP：联合类型
来源：http://lyo.haohaochexian.top

int|string $id
来源：http://qxr.pengpengdd.cyou

[U48] PHP：纯枚举
来源：http://smv.feifeiyinyue.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ylv.zhoulong.xyz

[U49] PHP：只读属性
来源：http://fjc.dianchejie.cn

public readonly string $name
来源：http://ycp.mhx1999.top

[U50] PHP：构造器属性提升
来源：http://pqq.uphjek.com

public function __construct(private int $id) {}
来源：http://zpo.shanyushiyangkeji.top

[U51] PHP：数组解构
来源：http://rsx.ybcxt.top

[$a, $b] = $arr;
来源：http://bdd.xingfuxueyuan.xyz

[U52] PHP：箭头函数
来源：http://rpb.tanke756.top

$double = fn($x) => $x * 2;
来源：http://jhd.haohaochexian.top

[U53] PHP：空合并运算符
来源：http://vml.dianchejie.cn

$v = $a ?? $b ?? "default";
来源：http://wjj.xingfuxueyuan.xyz

[U54] PHP：空安全调用
来源：http://qzv.cdnleiting.top

$obj?->method()
来源：http://vht.sjlbkw.cn

[U55] PHP：match 表达式
来源：http://vyv.ehwqpu.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://exr.daria6918.cn

[U56] PHP：命名参数
来源：http://kqy.yonumen.top

f(a: 1, b: 2)
来源：http://zpu.chenlongwang.top

[U57] PHP：字符串插值
来源：http://pox.shanyushiyangtech.top

"值: {$a}"
来源：http://ahu.zhiwuduotai.top

[U58] PHP：数组三件套
来源：http://ala.shanyushiyangtech.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xql.fktsv.cn

[U59] PHP：自定义排序
来源：http://eqr.vqdsnc.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gsu.jinyuanbaomall.cn

[U60] PHP：JSON 编解码
来源：http://gpn.yj202588.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kmo.shanyushiyangtech.top

[U61] PHP：正则
来源：http://heu.xingfuxueyuan.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ihb.gzhubu.top

[U62] PHP：日期对象
来源：http://lwj.hysaishi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rbl.kuanghao11.cn

[U63] PHP：文件读写
来源：http://iks.yonumen.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qzz.vehdjk.com

[U64] PHP：目录遍历
来源：http://kqo.zhixingplan.top

glob("dir/*.php");  scandir("dir");
来源：http://ilu.quarkkingdee.top

[U65] PHP：会话
来源：http://jdu.jlsjyb.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://dmw.shanyushiyangkeji.top

[U66] PHP：设置 Cookie
来源：http://yqs.gaohongyu789.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kur.yj202588.top

[U67] PHP：处理文件上传
来源：http://obe.jinqigfzy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hbu.xingfuxueyuan.xyz

[U68] PHP：PDO 连接
来源：http://zif.yj20258888.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://utp.jinghuilouyu.cn

[U69] PHP：PDO 预处理
来源：http://aha.hammf.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kff.jlsjyb.cn

[U70] PHP：PDO 事务
来源：http://mug.yueranfly.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ehn.aizwys.cn

[U71] PHP：抛出异常
来源：http://tqe.hcnkem.com

throw new RuntimeException("失败", 500);
来源：http://yfp.aibaodan.cn

[U72] PHP：写错误日志
来源：http://uhd.zhixingplan.top

error_log("失败: " . $e->getMessage());
来源：http://dux.jyoumei.cn

[U73] PHP：读取 ini 配置
来源：http://itk.guannengcc.top

parse_ini_file("config.ini", true)
来源：http://zfl.yueranfly.top

[U74] PHP：读取环境变量
来源：http://qlt.fehbvm.com

getenv("APP_ENV") ?: "production"
来源：http://ohj.zdbjq.cn

[U75] PHP：依赖注入
来源：http://ppb.shanyushiyangtech.top

composer require psr/container
来源：http://zsh.daria6918.cn

[U76] PHP：简单路由
来源：http://ike.bbcook.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rqa.vehdjk.com

[U77] PHP：模板渲染
来源：http://dnk.dianchejie.cn

composer require twig/twig
来源：http://oao.c1oappe.top

[U78] PHP：单元测试
来源：http://nkr.havefunace.top

composer require --dev phpunit/phpunit
来源：http://fla.c1oappe.top

[U79] PHP：静态分析
来源：http://ikg.cdnleiting.top

composer require --dev phpstan/phpstan
来源：http://hzc.andypj.xyz

[U80] PHP：代码规范修复
来源：http://gam.wangdashe.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://zfr.jqgufenzy.top

[U81] JS：初始化项目
来源：http://hxy.xuanzx.com

npm init -y;  npm i express
来源：http://sho.xuetiantiany.cn

[U82] JS：package.json 脚本
来源：http://eha.jianghu66.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://dqw.guowangkeji.top

[U83] JS：ES Module 导入导出
来源：http://kll.hysaishi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://oni.ivvv.top

[U84] JS：CommonJS 写法
来源：http://wwd.aizwys.cn

module.exports = { a };  const { a } = require("./m");
来源：http://gvi.iojbl.cn

[U85] JS：可选链
来源：http://ttt.0kj1m.cn

a?.b?.c
来源：http://roc.cdnleiting.top

[U86] JS：空值合并
来源：http://kfa.pengpengdd.cyou

a ?? b
来源：http://piq.yj20258888.top

[U87] JS：解构默认值
来源：http://ugs.sysykeji.top

const { a = 1, b = 2 } = obj;
来源：http://fig.chenlongwang.top

[U88] JS：对象展开合并
来源：http://evp.jinqigufen.top

{ ...a, ...b }
来源：http://tjq.wangdashe.top

[U89] JS：数组去重
来源：http://psx.chenzaomai.com

[...new Set(arr)]
来源：http://dtk.zdbjq.cn

[U90] JS：数字数组排序
来源：http://asx.guannengcc.top

[...arr].sort((a, b) => a - b)
来源：http://qoj.yj202588.top

[U91] JS：对象键值遍历
来源：http://vmf.jiagoushi.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ram.sweek.top

[U92] JS：深拷贝
来源：http://wxk.ydzc1.top

structuredClone(obj)
来源：http://cff.tarul.cn

[U93] JS：模板字符串
来源：http://upf.cheryme.top

`共 ${n} 条`
来源：http://jzq.hywenlv.cn

[U94] JS：箭头函数
来源：http://ktn.iojbl.cn

const double = x => x * 2;
来源：http://gke.hfpthk.cn

[U95] JS：Promise 包装
来源：http://dlm.aizwys.cn

new Promise((resolve, reject) => {})
来源：http://kdy.xingfuxueyuan.xyz

[U96] JS：async/await 与异常
来源：http://shm.cashguo.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://sha.sysykeji.top

[U97] JS：并发请求
来源：http://cjc.wangshuangyany.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://xaa.havefunace.top

[U98] JS：fetch 带 JSON
来源：http://odw.nanxinkj.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gib.jinyuanbaomall.cn

[U99] JS：事件监听
来源：http://bmc.gzhubu.top

el.addEventListener("click", e => {})
来源：http://jrg.yongpay.top

[U100] JS：DOM 查询
来源：http://ill.birdmap.top

document.querySelector(".item")
来源：http://xnh.snrcjt.cn

[U101] JS：classList 操作
来源：http://sko.zhijiandao.cn

el.classList.toggle("active")
来源：http://ube.snrcjt.cn

[U102] JS：本地存储
来源：http://jff.nanxinkj.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://tax.tian-w.cn

[U103] JS：定时器
来源：http://zvn.zhixingplan.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mvf.jinyuanbaomall.cn

[U104] JS：防抖
来源：http://jlv.fengsongda.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://npl.nanxinkj.top

[U105] JS：节流
来源：http://bsf.wangshuangyany.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://amo.ctjpmb.com

[U106] JS：日期格式化
来源：http://eun.feifeiyinyue.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nfy.ydzc1.top

[U107] JS：数字千分位
来源：http://iid.wangdashe.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jro.bbcook.cn

[U108] JS：随机整数
来源：http://ejn.tanke756.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fjp.yangfankeji.com

[U109] JS：数组分组
来源：http://cdq.hesvh.cn

Object.groupBy(arr, x => x.type)
来源：http://czk.andypj.xyz

[U110] JS：数组分块
来源：http://jbd.xylfe.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lwu.yongpay.top

[U111] JS：对象转 Map
来源：http://piq.gaohongyu789.top

new Map(Object.entries(obj))
来源：http://vcb.redwolf501.top

[U112] JS：字符串补位
来源：http://vsg.cashguo.top

"7".padStart(3, "0")
来源：http://iod.guannengcc.top

[U113] JS：正则替换全部
来源：http://ryx.tarul.cn

s.replaceAll("a", "b")
来源：http://elt.gaohongyu789.top

[U114] JS：JSON 深比较
来源：http://cmw.yj20258888.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://qky.daxiang520.top

[U115] JS：生成 UUID
来源：http://rsa.shuidangran.top

crypto.randomUUID()
来源：http://gum.tarul.cn

[U116] JS：类型检查（JSDoc）
来源：http://usy.zhongyouzk.top

/** @param {string} name */ function f(name) {}
来源：http://mfk.sysykeji.top

[U117] JS：单元测试
来源：http://xto.smart0.xyz

npm i -D vitest;  npx vitest
来源：http://uch.jyoumei.cn

[U118] JS：开发服务器
来源：http://plc.fengsongda.top

npm i -D vite;  npx vite
来源：http://vdk.aizwys.cn

[U119] JS：生产构建
来源：http://pwf.zdbjq.cn

npx vite build
来源：http://wph.gogol.net.cn

[U120] JS：读取环境变量（Vite）
来源：http://zdw.ivvv.top

import.meta.env.VITE_API_URL
来源：http://gqy.svipenyu.cn

================================================================================
来源：http://xda.shanyushiyangkeji.top

统计汇总
来源：http://xqw.gotoacloud.top

================================================================================
来源：http://pag.yj20258.top

按语言统计（条）：
来源：http://zon.nanxinkj.top

Python ......... 252
来源：http://nqn.xylfe.cn

PHP ............ 252
来源：http://dpq.zhoulong.xyz

JavaScript ..... 252
来源：http://zcv.dianchejie.cn

TypeScript ..... 212
来源：http://lwr.yuanzhike.top

Java ........... 212
来源：http://fxs.jinqigfzy.top

Go ............. 212
来源：http://que.shzxlz.cn

Ruby ........... 212
来源：http://jrs.andypj.xyz

C# ............. 212
来源：http://apk.shzxlz.cn


<!-- 参考信息 -->