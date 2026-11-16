代发 wailian999

[T41] Perl：Hello World
来源：http://oaj.ywan-chungtsiang.top

print "Hello\n";
来源：http://luv.shanyushiyangkeji.top

[T42] Perl：变量类型
来源：http://hwd.zhaomingkeji.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bbg.ehwqpu.com

[T43] Perl：字符串插值
来源：http://uaa.vqdsnc.cn

"值: $a"
来源：http://kuk.zhiwuduotai.top

[T44] Perl：条件
来源：http://tph.hnxiangtu.top

if ($a > 0) { print "正"; }
来源：http://owr.aizwys.cn

[T45] Perl：数组遍历
来源：http://bkq.ydjk.org.cn

for my $x (@arr) { print $x; }
来源：http://wja.jinyuanbaomall.cn

[T46] Perl：哈希操作
来源：http://uma.sufxvd.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://iap.redwolf501.top

[T47] Perl：正则捕获
来源：http://ecb.bjfxy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://gjs.zhengqikj.top

[T48] Perl：正则替换
来源：http://pbw.sxryk.cn

$s =~ s/old/new/g;
来源：http://ewy.xziqi.cn

[T49] Perl：函数
来源：http://gag.shanyushiyangtech.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gzj.yonumen.top

[T50] Perl：逐行读文件
来源：http://pse.fehbvm.com

open my $fh, "<", "a.txt" or die $!;
来源：http://pgp.yuxming.cn

while (my $line = <$fh>) { print $line; }
来源：http://bes.tian-w.cn

[T51] Scala：Hello World
来源：http://mvq.xziqi.cn

println("Hello")
来源：http://myv.nanxuanxn.top

[T52] Scala：变量
来源：http://yzu.epnwcf.com

val a = 1;  var b = 2
来源：http://kex.hammf.cn

[T53] Scala：字符串插值
来源：http://dat.shanyushiyangkeji.top

s"值: $b"
来源：http://jkb.epnwcf.com

[T54] Scala：集合映射
来源：http://bjr.guowangkeji.top

List(1, 2, 3).map(_ * 2)
来源：http://hkw.ydjk.org.cn

[T55] Scala：集合过滤
来源：http://tww.cdnleiting.top

List(1, 2, 3).filter(_ > 1)
来源：http://bey.tarul.cn

[T56] Scala：样例类
来源：http://xcq.xuanzx.com

case class User(name: String, age: Int)
来源：http://myt.yangfankeji.com

[T57] Scala：模式匹配
来源：http://clx.smart0.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://kun.tanke756.top

[T58] Scala：函数定义
来源：http://ryz.hfpthk.cn

def add(a: Int, b: Int): Int = a + b
来源：http://tvi.fzhhl.top

[T59] Scala：循环
来源：http://nkq.hfpthk.cn

for (i <- 1 to 10) println(i)
来源：http://nst.feifeiyinyue.top

[T60] Scala：折叠
来源：http://bsc.bbcook.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yzn.iojbl.cn

================================================================================
来源：http://syd.jlsjyb.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ekg.jinqigfzy.top

================================================================================
来源：http://cod.pycfn.com

[U01] Py：创建虚拟环境
来源：http://dxi.nanxuanxn.top

python -m venv .venv && source .venv/bin/activate
来源：http://pde.jqgfzy.top

[U02] Py：导出 / 安装依赖
来源：http://hek.dianchejie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vfl.9152youxi.cn

[U03] Py：加载 .env 配置
来源：http://dev.jyoumei.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://wac.52xcode.cn

[U04] Py：变量调试打印
来源：http://lxh.xziqi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hlm.pengpengdd.cyou

[U05] Py：列表去重且保序
来源：http://nsx.xuanzx.com

list(dict.fromkeys(arr))
来源：http://wpv.guannengcc.top

[U06] Py：合并两个字典
来源：http://ovv.fengsongda.top

{**a, **b}
来源：http://zya.zycfv.cn

[U07] Py：反转字典键值
来源：http://ifj.cqqwz.cn

{v: k for k, v in d.items()}
来源：http://ygw.ywan-chungtsiang.top

[U08] Py：展平二维列表
来源：http://qti.chenlongwang.top

[y for x in nested for y in x]
来源：http://sps.daria6918.cn

[U09] Py：字典取最大值的键
来源：http://qpq.ehwqpu.com

max(d, key=d.get)
来源：http://wen.bbcook.cn

[U10] Py：按值排序字典
来源：http://lwi.ivvv.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xdu.jinyuanbaomall.cn

[U11] Py：生成器表达式
来源：http://avc.9152youxi.cn

(x * 2 for x in arr)
来源：http://nxx.vqdsnc.cn

[U12] Py：取出现最多的 3 个元素
来源：http://pqv.hongshengwenyu.top

Counter(arr).most_common(3)
来源：http://ije.sxryk.cn

[U13] Py：固定长度队列
来源：http://xga.hammf.cn

deque(maxlen=10)
来源：http://phf.cashguo.top

[U14] Py：分组收集到列表
来源：http://nji.jianghu66.top

defaultdict(list)
来源：http://nsc.guannengcc.top

[U15] Py：高精度计时
来源：http://evx.xziqi.cn

t = time.perf_counter()
来源：http://wvm.hnqzz.top

[U16] Py：命令行参数解析
来源：http://qvm.chenzaomai.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://opv.chenjidiqi.icu

[U17] Py：初始化日志
来源：http://ilv.xuanzx.com

logging.basicConfig(level=logging.INFO)
来源：http://dpz.tian-w.cn

[U18] Py：预编译正则
来源：http://rrn.gaohongyu789.top

pat = re.compile(r"\d+")
来源：http://ozb.xuetiantiany.cn

[U19] Py：正则替换带回调
来源：http://mov.birdmap.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kql.shuidangran.top

[U20] Py：缓存函数结果
来源：http://lbt.meibo888.top

@functools.lru_cache(maxsize=None)
来源：http://aeg.sxryk.cn

[U21] Py：自定义上下文管理器
来源：http://bqr.jinqigufen.top

@contextlib.contextmanager
来源：http://seu.ivvv.top

[U22] Py：矩阵转置
来源：http://soe.zhijiandao.cn

list(zip(*m))
来源：http://ixx.cashguo.top

[U23] Py：分块读取大文件
来源：http://iih.hammf.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wxw.sysykeji.top

[U24] Py：路径操作
来源：http://xns.smart0.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://znj.yvedp.cn

[U25] Py：CSV 按字典读
来源：http://rrk.shanyushiyangkeji.top

csv.DictReader(f)
来源：http://itz.chenzaomai.com

[U26] Py：并发下载
来源：http://dwy.xinyue.icu

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://atd.guannengcc.top

[U27] Py：异步 HTTP
来源：http://bhv.wangshuangyany.cn

aiohttp.ClientSession() 配合 async with
来源：http://ghv.fehbvm.com

[U28] Py：类型别名
来源：http://vam.shangyingyoupin.top

UserId = int
来源：http://ljv.gotoacloud.top

[U29] Py：属性校验
来源：http://sad.zhixingplan.top

@property 与 @x.setter 配合
来源：http://kjo.yvedp.cn

[U30] Py：数据类
来源：http://jfc.bbcook.cn

@dataclass(slots=True)
来源：http://wfg.sysykeji.top

[U31] Py：单测
来源：http://bqg.mhx1999.top

python -m pytest -q
来源：http://odo.yj20258888.top

[U32] Py：代码格式化
来源：http://zqg.vehdjk.com

ruff format . && ruff check --fix .
来源：http://jxu.iojbl.cn

[U33] Py：打包发布
来源：http://hkv.dashuyun.cn

python -m build  （依赖 pyproject.toml）
来源：http://jtt.jinghuilouyu.cn

[U34] Py：判断编码
来源：http://dds.zhiwuduotai.top

chardet.detect(raw)
来源：http://ilk.meibo888.top

[U35] Py：发送邮件
来源：http://gcl.kuanghao11.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://sbr.jlsjyb.cn

[U36] Py：定时任务
来源：http://xdl.hfpthk.cn

schedule.every(10).minutes.do(job)
来源：http://okd.wangdashe.top

[U37] Py：读写 Excel
来源：http://kth.quarkkingdee.top

pandas.read_excel / DataFrame.to_excel
来源：http://zcn.fanxiaobao.xyz

[U38] Py：获取脚本所在目录
来源：http://swn.jiagoushi.top

Path(__file__).resolve().parent
来源：http://upe.tarul.cn

[U39] Py：判断是否在交互环境
来源：http://mbo.jqgfzy.top

sys.stdout.isatty()
来源：http://axq.yvedp.cn

[U40] Py：打印到标准错误
来源：http://dkj.9152youxi.cn

print("err", file=sys.stderr)
来源：http://sdt.sxryk.cn

[U41] PHP：初始化 Composer 项目
来源：http://acj.quarkkingdee.top

composer init;  composer require guzzlehttp/guzzle
来源：http://bky.fanxiaobao.xyz

[U42] PHP：PSR-4 自动加载
来源：http://akv.jinqigfzy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ztd.zdqjudy.top

[U43] PHP：声明命名空间
来源：http://nro.gzhubu.top

namespace App\Http;
来源：http://gju.meibo888.top

[U44] PHP：开启严格类型
来源：http://phe.gaohongyu789.top

declare(strict_types=1);
来源：http://tna.shzxlz.cn

[U45] PHP：类型声明与返回类型
来源：http://lsj.epnwcf.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://qhp.0kj1m.cn

[U46] PHP：可空类型
来源：http://aro.xinyue.icu

?string $name = null
来源：http://kme.jinqigfzy.top

[U47] PHP：联合类型
来源：http://fwi.pycfn.com

int|string $id
来源：http://yfo.epnwcf.com

[U48] PHP：纯枚举
来源：http://cvk.fengsongda.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hxj.zhixingplan.top

[U49] PHP：只读属性
来源：http://oik.yuanzhike.top

public readonly string $name
来源：http://bbb.xziqi.cn

[U50] PHP：构造器属性提升
来源：http://fhv.gotoacloud.top

public function __construct(private int $id) {}
来源：http://efg.quarkkingdee.top

[U51] PHP：数组解构
来源：http://htr.sufxvd.cn

[$a, $b] = $arr;
来源：http://ypx.hnqzz.top

[U52] PHP：箭头函数
来源：http://twh.tarul.cn

$double = fn($x) => $x * 2;
来源：http://opo.dianchejie.cn

[U53] PHP：空合并运算符
来源：http://kse.nanxuanxn.top

$v = $a ?? $b ?? "default";
来源：http://kft.quarkkingdee.top

[U54] PHP：空安全调用
来源：http://epn.aizwys.cn

$obj?->method()
来源：http://oob.gzhubu.top

[U55] PHP：match 表达式
来源：http://juu.cheryme.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ofz.ywan-chungtsiang.top

[U56] PHP：命名参数
来源：http://yyf.gaohongyu789.top

f(a: 1, b: 2)
来源：http://pyp.sweek.top

[U57] PHP：字符串插值
来源：http://ucf.0kj1m.cn

"值: {$a}"
来源：http://izi.quarkkingdee.top

[U58] PHP：数组三件套
来源：http://wkn.zhaomingkeji.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nwl.sxryk.cn

[U59] PHP：自定义排序
来源：http://unp.nwbrower.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vel.xziqi.cn

[U60] PHP：JSON 编解码
来源：http://oin.yongpay.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zgh.xinyue.icu

[U61] PHP：正则
来源：http://mac.ehwqpu.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rnr.feifeiyinyue.top

[U62] PHP：日期对象
来源：http://aex.gotoacloud.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pdk.redwolf501.top

[U63] PHP：文件读写
来源：http://ity.gotoacloud.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jqd.jinyuanbaomall.cn

[U64] PHP：目录遍历
来源：http://nga.nanxinkj.top

glob("dir/*.php");  scandir("dir");
来源：http://rbp.cashguo.top

[U65] PHP：会话
来源：http://ppw.gaohongyu789.top

session_start();  $_SESSION["uid"] = 1;
来源：http://hyr.jiagoushi.top

[U66] PHP：设置 Cookie
来源：http://tgo.shanyushiyangkeji.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ovf.jlsjyb.cn

[U67] PHP：处理文件上传
来源：http://hjh.hysaishi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://cnp.shanyushiyangtech.top

[U68] PHP：PDO 连接
来源：http://ojo.9152youxi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xio.bjfxy.top

[U69] PHP：PDO 预处理
来源：http://hgt.birdmap.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kmc.fktsv.cn

[U70] PHP：PDO 事务
来源：http://bpg.chenjidiqi.icu

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tkc.feifeiyinyue.top

[U71] PHP：抛出异常
来源：http://qac.shuidangran.top

throw new RuntimeException("失败", 500);
来源：http://vso.pycfn.com

[U72] PHP：写错误日志
来源：http://gyn.ehwqpu.com

error_log("失败: " . $e->getMessage());
来源：http://avq.fktsv.cn

[U73] PHP：读取 ini 配置
来源：http://slo.jianghu66.top

parse_ini_file("config.ini", true)
来源：http://vqf.iojbl.cn

[U74] PHP：读取环境变量
来源：http://zjr.xinyue.icu

getenv("APP_ENV") ?: "production"
来源：http://mwm.daria6918.cn

[U75] PHP：依赖注入
来源：http://oyi.smart0.xyz

composer require psr/container
来源：http://enj.ehwqpu.com

[U76] PHP：简单路由
来源：http://vsx.zhiwuduotai.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pna.jqgfzy.top

[U77] PHP：模板渲染
来源：http://gsr.tianlin.xyz

composer require twig/twig
来源：http://gzq.hnxiangtu.top

[U78] PHP：单元测试
来源：http://jhd.xinyue.icu

composer require --dev phpunit/phpunit
来源：http://xzq.yuanzhike.top

[U79] PHP：静态分析
来源：http://nbq.vqdsnc.cn

composer require --dev phpstan/phpstan
来源：http://ybj.jqgfzy.top

[U80] PHP：代码规范修复
来源：http://hzn.ctjpmb.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://quq.yj20258888.top

[U81] JS：初始化项目
来源：http://tiq.shuidangran.top

npm init -y;  npm i express
来源：http://civ.yj20258.top

[U82] JS：package.json 脚本
来源：http://bwu.cucudq.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jyk.zhengqikj.top

[U83] JS：ES Module 导入导出
来源：http://iav.ppjwa.cn

export const a = 1;  import { a } from "./m.js";
来源：http://hva.zhijiandao.cn

[U84] JS：CommonJS 写法
来源：http://eve.sxryk.cn

module.exports = { a };  const { a } = require("./m");
来源：http://wqo.xylfe.cn

[U85] JS：可选链
来源：http://uyc.haohaochexian.top

a?.b?.c
来源：http://cim.tarul.cn

[U86] JS：空值合并
来源：http://sdt.xylfe.cn

a ?? b
来源：http://lwc.dianchejie.cn

[U87] JS：解构默认值
来源：http://mpv.dianchejie.cn

const { a = 1, b = 2 } = obj;
来源：http://rpo.chenjidiqi.icu

[U88] JS：对象展开合并
来源：http://qfh.gotoacloud.top

{ ...a, ...b }
来源：http://nuq.cheryme.top

[U89] JS：数组去重
来源：http://mqj.snrcjt.cn

[...new Set(arr)]
来源：http://ukv.fktsv.cn

[U90] JS：数字数组排序
来源：http://ijc.zdbjq.cn

[...arr].sort((a, b) => a - b)
来源：http://yvs.svipenyu.cn

[U91] JS：对象键值遍历
来源：http://inc.hywenlv.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qkr.nanxinkj.top

[U92] JS：深拷贝
来源：http://ocp.fzhhl.top

structuredClone(obj)
来源：http://dye.yuanzhike.top

[U93] JS：模板字符串
来源：http://wti.gotoacloud.top

`共 ${n} 条`
来源：http://ggf.shanyushiyangkeji.top

[U94] JS：箭头函数
来源：http://yro.0kj1m.cn

const double = x => x * 2;
来源：http://kom.meibo888.top

[U95] JS：Promise 包装
来源：http://bhw.yangfankeji.com

new Promise((resolve, reject) => {})
来源：http://ssf.jqgufenzy.top

[U96] JS：async/await 与异常
来源：http://lxn.yj202588.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://omt.andypj.xyz

[U97] JS：并发请求
来源：http://pud.ehwqpu.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://wvs.snrcjt.cn

[U98] JS：fetch 带 JSON
来源：http://qvh.gotoacloud.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hqk.pycfn.com

[U99] JS：事件监听
来源：http://edr.snrcjt.cn

el.addEventListener("click", e => {})
来源：http://api.zhixingplan.top

[U100] JS：DOM 查询
来源：http://gxq.zhiwuduotai.top

document.querySelector(".item")
来源：http://xfc.jqgfzy.top

[U101] JS：classList 操作
来源：http://qef.ydzc1.top

el.classList.toggle("active")
来源：http://sxt.zdbjq.cn

[U102] JS：本地存储
来源：http://hvw.hammf.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://wpj.xinyue.icu

[U103] JS：定时器
来源：http://skc.yanxiufei.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xqy.hammf.cn

[U104] JS：防抖
来源：http://mxy.gotoacloud.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gjw.svipenyu.cn

[U105] JS：节流
来源：http://trl.snrcjt.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pqz.hywenlv.cn

[U106] JS：日期格式化
来源：http://isu.ydzc1.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://uwg.wangdashe.top

[U107] JS：数字千分位
来源：http://hsu.nanxuanxn.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hyi.yj202588.top

[U108] JS：随机整数
来源：http://imc.xingfuxueyuan.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xwm.yuanzhike.top

[U109] JS：数组分组
来源：http://htu.havefunace.top

Object.groupBy(arr, x => x.type)
来源：http://elb.jqgfzy.top

[U110] JS：数组分块
来源：http://xis.c1oappe.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fne.andypj.xyz

[U111] JS：对象转 Map
来源：http://rbc.nwbrower.top

new Map(Object.entries(obj))
来源：http://zar.sxryk.cn

[U112] JS：字符串补位
来源：http://xxx.shzxlz.cn

"7".padStart(3, "0")
来源：http://ota.jlsjyb.cn

[U113] JS：正则替换全部
来源：http://oeq.sweek.top

s.replaceAll("a", "b")
来源：http://rbm.uphjek.com

[U114] JS：JSON 深比较
来源：http://nnw.mhx1999.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://hpk.ydjk.org.cn

[U115] JS：生成 UUID
来源：http://tmp.jqgufenzy.top

crypto.randomUUID()
来源：http://nvr.sxryk.cn

[U116] JS：类型检查（JSDoc）
来源：http://ntw.zhiwuduotai.top

/** @param {string} name */ function f(name) {}
来源：http://bay.fengsongda.top

[U117] JS：单元测试
来源：http://amt.aizwys.cn

npm i -D vitest;  npx vitest
来源：http://dpi.52xcode.cn

[U118] JS：开发服务器
来源：http://utg.hfpthk.cn

npm i -D vite;  npx vite
来源：http://qsx.tian-w.cn

[U119] JS：生产构建
来源：http://wrv.jlsjyb.cn

npx vite build
来源：http://cew.xuetiantiany.cn

[U120] JS：读取环境变量（Vite）
来源：http://uss.mhx1999.top

import.meta.env.VITE_API_URL
来源：http://ffx.wangshuangyany.cn

================================================================================
来源：http://fkz.quarkkingdee.top

统计汇总
来源：http://tbo.hammf.cn

================================================================================
来源：http://yfv.gogol.net.cn

按语言统计（条）：
来源：http://wck.shangyingyoupin.top

Python ......... 252
来源：http://zdn.9152youxi.cn

PHP ............ 252
来源：http://lme.ctjpmb.com

JavaScript ..... 252
来源：http://xcu.zhengqikj.top

TypeScript ..... 212
来源：http://kcv.mhx1999.top

Java ........... 212
来源：http://oef.yj20258.top

Go ............. 212
来源：http://xca.yangfankeji.com

Ruby ........... 212
来源：http://cdw.zdqjudy.top

C# ............. 212
来源：http://ltz.aibaodan.cn

C .............. 30
来源：http://ayi.zhaomingkeji.xyz

C++ ............ 30
来源：http://dpw.hcnkem.com

SQL ............ 90
来源：http://odp.nwbrower.top

Bash ........... 80
来源：http://rjz.gotoacloud.top


<!-- 参考信息 -->