代发 wailian999

[T39] Lua：模式匹配
来源：http://lgr.chenzaomai.com

string.find(s, "%d+")
来源：http://neg.xinyue.icu

[T40] Lua：元表
来源：http://ycj.hammf.cn

setmetatable({}, { __index = base })
来源：http://lcc.zhengqikj.top

[T41] Perl：Hello World
来源：http://toh.yuanzhike.top

print "Hello\n";
来源：http://fqg.aibaodan.cn

[T42] Perl：变量类型
来源：http://bvp.snrcjt.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kqn.chenjidiqi.icu

[T43] Perl：字符串插值
来源：http://gkg.dianchejie.cn

"值: $a"
来源：http://oss.jyoumei.cn

[T44] Perl：条件
来源：http://vdx.9152youxi.cn

if ($a > 0) { print "正"; }
来源：http://gxy.gaohongyu789.top

[T45] Perl：数组遍历
来源：http://iej.yfazqb.com

for my $x (@arr) { print $x; }
来源：http://opz.shanyushiyangkeji.top

[T46] Perl：哈希操作
来源：http://syx.havefunace.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ref.shzxlz.cn

[T47] Perl：正则捕获
来源：http://uhl.hammf.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://rmo.yj20258.top

[T48] Perl：正则替换
来源：http://yrx.hesvh.cn

$s =~ s/old/new/g;
来源：http://wlz.cucudq.cn

[T49] Perl：函数
来源：http://tua.0kj1m.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zxq.cdnleiting.top

[T50] Perl：逐行读文件
来源：http://gvt.ydzc1.top

open my $fh, "<", "a.txt" or die $!;
来源：http://xwa.tianlin.xyz

while (my $line = <$fh>) { print $line; }
来源：http://ryn.hywenlv.cn

[T51] Scala：Hello World
来源：http://tyl.xziqi.cn

println("Hello")
来源：http://hjk.cashguo.top

[T52] Scala：变量
来源：http://whz.kuanghao11.cn

val a = 1;  var b = 2
来源：http://rxf.ydzc1.top

[T53] Scala：字符串插值
来源：http://yla.yangfankeji.com

s"值: $b"
来源：http://zkg.chenjidiqi.icu

[T54] Scala：集合映射
来源：http://gyx.yongpay.top

List(1, 2, 3).map(_ * 2)
来源：http://fxl.fktsv.cn

[T55] Scala：集合过滤
来源：http://uzf.bjfxy.top

List(1, 2, 3).filter(_ > 1)
来源：http://qyb.sxryk.cn

[T56] Scala：样例类
来源：http://jwi.xziqi.cn

case class User(name: String, age: Int)
来源：http://yll.hnqzz.top

[T57] Scala：模式匹配
来源：http://bcx.yj20258.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://kzx.zhixingplan.top

[T58] Scala：函数定义
来源：http://nmw.fanxiaobao.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://cvg.nanxuanxn.top

[T59] Scala：循环
来源：http://htq.jianghu66.top

for (i <- 1 to 10) println(i)
来源：http://fon.yvedp.cn

[T60] Scala：折叠
来源：http://ugj.dianchejie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zon.kuanghao11.cn

================================================================================
来源：http://gyb.cashguo.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yjj.fehbvm.com

================================================================================
来源：http://wmv.svipenyu.cn

[U01] Py：创建虚拟环境
来源：http://ylf.fktsv.cn

python -m venv .venv && source .venv/bin/activate
来源：http://tmh.gaohongyu789.top

[U02] Py：导出 / 安装依赖
来源：http://ryf.yj20258.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zez.ppjwa.cn

[U03] Py：加载 .env 配置
来源：http://wsl.svipenyu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://pik.chenjidiqi.icu

[U04] Py：变量调试打印
来源：http://pva.yj20258888.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vrd.dianchejie.cn

[U05] Py：列表去重且保序
来源：http://zed.mhx1999.top

list(dict.fromkeys(arr))
来源：http://wfc.fzhhl.top

[U06] Py：合并两个字典
来源：http://xwd.dashuyun.cn

{**a, **b}
来源：http://unu.havefunace.top

[U07] Py：反转字典键值
来源：http://jfp.zdqjudy.top

{v: k for k, v in d.items()}
来源：http://ggf.jinyuanbaomall.cn

[U08] Py：展平二维列表
来源：http://qvq.snrcjt.cn

[y for x in nested for y in x]
来源：http://oiw.kuanghao11.cn

[U09] Py：字典取最大值的键
来源：http://jdm.bbcook.cn

max(d, key=d.get)
来源：http://yin.ydjk.org.cn

[U10] Py：按值排序字典
来源：http://mum.sjlbkw.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ttg.daria6918.cn

[U11] Py：生成器表达式
来源：http://guq.wangshuangyany.cn

(x * 2 for x in arr)
来源：http://wod.yonumen.top

[U12] Py：取出现最多的 3 个元素
来源：http://fku.yongpay.top

Counter(arr).most_common(3)
来源：http://hlo.pycfn.com

[U13] Py：固定长度队列
来源：http://tnu.gzhubu.top

deque(maxlen=10)
来源：http://dtl.dianchejie.cn

[U14] Py：分组收集到列表
来源：http://pmp.cdnleiting.top

defaultdict(list)
来源：http://hvo.jinyuanbaomall.cn

[U15] Py：高精度计时
来源：http://ixb.jinghuilouyu.cn

t = time.perf_counter()
来源：http://ucv.sysykeji.top

[U16] Py：命令行参数解析
来源：http://bbm.wangshuangyany.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://muc.zhoulong.xyz

[U17] Py：初始化日志
来源：http://bwb.9152youxi.cn

logging.basicConfig(level=logging.INFO)
来源：http://iqu.feifeiyinyue.top

[U18] Py：预编译正则
来源：http://gkq.chenjidiqi.icu

pat = re.compile(r"\d+")
来源：http://buq.xinyue.icu

[U19] Py：正则替换带回调
来源：http://jwq.zhengqikj.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hvw.0kj1m.cn

[U20] Py：缓存函数结果
来源：http://zxq.cqqwz.cn

@functools.lru_cache(maxsize=None)
来源：http://iip.zhoulong.xyz

[U21] Py：自定义上下文管理器
来源：http://ifi.tian-w.cn

@contextlib.contextmanager
来源：http://rbj.hywenlv.cn

[U22] Py：矩阵转置
来源：http://qky.uphjek.com

list(zip(*m))
来源：http://fqx.hnxiangtu.top

[U23] Py：分块读取大文件
来源：http://ukh.meibo888.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tjb.kuanghao11.cn

[U24] Py：路径操作
来源：http://wbt.sweek.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://plx.sweek.top

[U25] Py：CSV 按字典读
来源：http://ufy.hnqzz.top

csv.DictReader(f)
来源：http://hcb.ivvv.top

[U26] Py：并发下载
来源：http://zbs.vqdsnc.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://dqm.ydzc1.top

[U27] Py：异步 HTTP
来源：http://vrq.andypj.xyz

aiohttp.ClientSession() 配合 async with
来源：http://xvk.jinghuilouyu.cn

[U28] Py：类型别名
来源：http://prb.jianghu66.top

UserId = int
来源：http://sij.zycfv.cn

[U29] Py：属性校验
来源：http://jxd.dianchejie.cn

@property 与 @x.setter 配合
来源：http://jez.yfazqb.com

[U30] Py：数据类
来源：http://lzq.0kj1m.cn

@dataclass(slots=True)
来源：http://hzt.andypj.xyz

[U31] Py：单测
来源：http://wqy.chenlongwang.top

python -m pytest -q
来源：http://zbp.guannengcc.top

[U32] Py：代码格式化
来源：http://qku.zdqjudy.top

ruff format . && ruff check --fix .
来源：http://lji.hnqzz.top

[U33] Py：打包发布
来源：http://tdr.c1oappe.top

python -m build  （依赖 pyproject.toml）
来源：http://ofa.fanxiaobao.xyz

[U34] Py：判断编码
来源：http://lhl.jianghu66.top

chardet.detect(raw)
来源：http://tkl.cdnleiting.top

[U35] Py：发送邮件
来源：http://fcv.ydjk.org.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cdw.zhoulong.xyz

[U36] Py：定时任务
来源：http://gzy.guowangkeji.top

schedule.every(10).minutes.do(job)
来源：http://poq.jianghu66.top

[U37] Py：读写 Excel
来源：http://iys.iojbl.cn

pandas.read_excel / DataFrame.to_excel
来源：http://fxv.xziqi.cn

[U38] Py：获取脚本所在目录
来源：http://giw.xziqi.cn

Path(__file__).resolve().parent
来源：http://sgu.fktsv.cn

[U39] Py：判断是否在交互环境
来源：http://ajy.jinqigfzy.top

sys.stdout.isatty()
来源：http://yuo.fengsongda.top

[U40] Py：打印到标准错误
来源：http://dvt.wangdashe.top

print("err", file=sys.stderr)
来源：http://nou.ivvv.top

[U41] PHP：初始化 Composer 项目
来源：http://zov.zdqjudy.top

composer init;  composer require guzzlehttp/guzzle
来源：http://flz.yonumen.top

[U42] PHP：PSR-4 自动加载
来源：http://vcu.nanxinkj.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bdw.yonumen.top

[U43] PHP：声明命名空间
来源：http://bjj.nwbrower.top

namespace App\Http;
来源：http://oqd.9152youxi.cn

[U44] PHP：开启严格类型
来源：http://ilw.iojbl.cn

declare(strict_types=1);
来源：http://xki.wangshuangyany.cn

[U45] PHP：类型声明与返回类型
来源：http://bwu.yuanzhike.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://are.yanxiufei.cn

[U46] PHP：可空类型
来源：http://fpq.yuanzhike.top

?string $name = null
来源：http://zat.yueranfly.top

[U47] PHP：联合类型
来源：http://uol.nanxuanxn.top

int|string $id
来源：http://dmj.dashuyun.cn

[U48] PHP：纯枚举
来源：http://ivm.shzxlz.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nqj.kuanghao11.cn

[U49] PHP：只读属性
来源：http://fhf.9152youxi.cn

public readonly string $name
来源：http://djj.yonumen.top

[U50] PHP：构造器属性提升
来源：http://loc.sweek.top

public function __construct(private int $id) {}
来源：http://bgk.gogol.net.cn

[U51] PHP：数组解构
来源：http://amz.dianchejie.cn

[$a, $b] = $arr;
来源：http://kuq.aizwys.cn

[U52] PHP：箭头函数
来源：http://vwj.fengsongda.top

$double = fn($x) => $x * 2;
来源：http://tnu.bjfxy.top

[U53] PHP：空合并运算符
来源：http://ujz.sufxvd.cn

$v = $a ?? $b ?? "default";
来源：http://jyx.hnqzz.top

[U54] PHP：空安全调用
来源：http://ogg.gogol.net.cn

$obj?->method()
来源：http://ope.dashuyun.cn

[U55] PHP：match 表达式
来源：http://fwk.svipenyu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jna.gaohongyu789.top

[U56] PHP：命名参数
来源：http://oad.iojbl.cn

f(a: 1, b: 2)
来源：http://udn.yj20258888.top

[U57] PHP：字符串插值
来源：http://tlm.sjlbkw.cn

"值: {$a}"
来源：http://yhn.zhijiandao.cn

[U58] PHP：数组三件套
来源：http://ojk.zhaomingkeji.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mvw.ivvv.top

[U59] PHP：自定义排序
来源：http://ufa.jinghuilouyu.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rdk.sysykeji.top

[U60] PHP：JSON 编解码
来源：http://bzp.chenlongwang.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xdg.fehbvm.com

[U61] PHP：正则
来源：http://wrl.yuanzhike.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tcj.jqgufenzy.top

[U62] PHP：日期对象
来源：http://ruy.jianghu66.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://cmn.zhoulong.xyz

[U63] PHP：文件读写
来源：http://wke.zycfv.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qad.snrcjt.cn

[U64] PHP：目录遍历
来源：http://xju.wangdashe.top

glob("dir/*.php");  scandir("dir");
来源：http://gqp.316326.xyz

[U65] PHP：会话
来源：http://qtj.xziqi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://sfo.gaohongyu789.top

[U66] PHP：设置 Cookie
来源：http://vjo.hesvh.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://evf.316326.xyz

[U67] PHP：处理文件上传
来源：http://mek.mhx1999.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zed.tarul.cn

[U68] PHP：PDO 连接
来源：http://cpz.havefunace.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://yxd.nanxinkj.top

[U69] PHP：PDO 预处理
来源：http://yfa.haohaochexian.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://tgt.wangdashe.top

[U70] PHP：PDO 事务
来源：http://hcp.jqgufenzy.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://yzd.iojbl.cn

[U71] PHP：抛出异常
来源：http://tao.tarul.cn

throw new RuntimeException("失败", 500);
来源：http://yqw.sweek.top

[U72] PHP：写错误日志
来源：http://ugi.jinyuanbaomall.cn

error_log("失败: " . $e->getMessage());
来源：http://fxc.ctjpmb.com

[U73] PHP：读取 ini 配置
来源：http://syp.chenjidiqi.icu

parse_ini_file("config.ini", true)
来源：http://lsu.fanxiaobao.xyz

[U74] PHP：读取环境变量
来源：http://ldv.shanyushiyangtech.top

getenv("APP_ENV") ?: "production"
来源：http://qki.shanyushiyangkeji.top

[U75] PHP：依赖注入
来源：http://ovk.meibo888.top

composer require psr/container
来源：http://lyk.hfpthk.cn

[U76] PHP：简单路由
来源：http://vst.iojbl.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ovh.316326.xyz

[U77] PHP：模板渲染
来源：http://uaq.bjfxy.top

composer require twig/twig
来源：http://lji.ybcxt.top

[U78] PHP：单元测试
来源：http://rfi.uphjek.com

composer require --dev phpunit/phpunit
来源：http://gdy.xziqi.cn

[U79] PHP：静态分析
来源：http://npg.fehbvm.com

composer require --dev phpstan/phpstan
来源：http://smm.svipenyu.cn

[U80] PHP：代码规范修复
来源：http://hgz.meibo888.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://euk.sufxvd.cn

[U81] JS：初始化项目
来源：http://epc.jinyuanbaomall.cn

npm init -y;  npm i express
来源：http://fve.zhijiandao.cn

[U82] JS：package.json 脚本
来源：http://mnm.hesvh.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pgf.daxiang520.top

[U83] JS：ES Module 导入导出
来源：http://tzn.chenlongwang.top

export const a = 1;  import { a } from "./m.js";
来源：http://crb.yvedp.cn

[U84] JS：CommonJS 写法
来源：http://usd.yanxiufei.cn

module.exports = { a };  const { a } = require("./m");
来源：http://fqu.haohaochexian.top

[U85] JS：可选链
来源：http://pmu.ydzc1.top

a?.b?.c
来源：http://njs.cashguo.top

[U86] JS：空值合并
来源：http://fes.iojbl.cn

a ?? b
来源：http://sng.ehwqpu.com

[U87] JS：解构默认值
来源：http://bde.mhx1999.top

const { a = 1, b = 2 } = obj;
来源：http://mbt.zhiwuduotai.top

[U88] JS：对象展开合并
来源：http://ffo.0kj1m.cn

{ ...a, ...b }
来源：http://mkn.ppjwa.cn

[U89] JS：数组去重
来源：http://xhz.bjfxy.top

[...new Set(arr)]
来源：http://svz.daria6918.cn

[U90] JS：数字数组排序
来源：http://dcp.wangdashe.top

[...arr].sort((a, b) => a - b)
来源：http://hnv.aizwys.cn

[U91] JS：对象键值遍历
来源：http://fwp.daria6918.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wgm.zhoulong.xyz

[U92] JS：深拷贝
来源：http://vpq.jyoumei.cn

structuredClone(obj)
来源：http://vsx.daxiang520.top

[U93] JS：模板字符串
来源：http://uus.jqgufenzy.top

`共 ${n} 条`
来源：http://nzp.xuetiantiany.cn

[U94] JS：箭头函数
来源：http://knz.fktsv.cn

const double = x => x * 2;
来源：http://zxn.havefunace.top

[U95] JS：Promise 包装
来源：http://byw.52xcode.cn

new Promise((resolve, reject) => {})
来源：http://sjg.hnxiangtu.top

[U96] JS：async/await 与异常
来源：http://ygt.havefunace.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pnb.yvedp.cn

[U97] JS：并发请求
来源：http://mxi.fengsongda.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://isi.guannengcc.top

[U98] JS：fetch 带 JSON
来源：http://ntk.ctjpmb.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://yto.sufxvd.cn

[U99] JS：事件监听
来源：http://byn.ybcxt.top

el.addEventListener("click", e => {})
来源：http://xdm.hesvh.cn

[U100] JS：DOM 查询
来源：http://xpp.jqgufenzy.top

document.querySelector(".item")
来源：http://yej.nwbrower.top

[U101] JS：classList 操作
来源：http://exg.uphjek.com

el.classList.toggle("active")
来源：http://cti.zhixingplan.top

[U102] JS：本地存储
来源：http://jsj.yanxiufei.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://lvp.cqqwz.cn

[U103] JS：定时器
来源：http://omh.shuidangran.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ptx.jiagoushi.top

[U104] JS：防抖
来源：http://ier.yuanzhike.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://plw.xinyue.icu

[U105] JS：节流
来源：http://akl.redwolf501.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yya.fengsongda.top

[U106] JS：日期格式化
来源：http://btp.yangfankeji.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jko.fengsongda.top

[U107] JS：数字千分位
来源：http://nhs.ctjpmb.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://tub.tarul.cn

[U108] JS：随机整数
来源：http://cdy.zhongyouzk.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gjr.jinyuanbaomall.cn

[U109] JS：数组分组
来源：http://nkx.dashuyun.cn

Object.groupBy(arr, x => x.type)
来源：http://gtx.chenlongwang.top

[U110] JS：数组分块
来源：http://asd.pengpengdd.cyou

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://akn.jyoumei.cn

[U111] JS：对象转 Map
来源：http://lrf.pengpengdd.cyou

new Map(Object.entries(obj))
来源：http://naj.zhaomingkeji.xyz

[U112] JS：字符串补位
来源：http://wru.jyoumei.cn

"7".padStart(3, "0")
来源：http://fkk.gogol.net.cn

[U113] JS：正则替换全部
来源：http://zun.yvedp.cn

s.replaceAll("a", "b")
来源：http://wvo.sxryk.cn

[U114] JS：JSON 深比较
来源：http://zpm.bbcook.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://wgr.pengpengdd.cyou

[U115] JS：生成 UUID
来源：http://ghj.fzhhl.top

crypto.randomUUID()
来源：http://ngs.ppjwa.cn

[U116] JS：类型检查（JSDoc）
来源：http://wak.iojbl.cn

/** @param {string} name */ function f(name) {}
来源：http://njo.shanyushiyangkeji.top

[U117] JS：单元测试
来源：http://qxa.xziqi.cn

npm i -D vitest;  npx vitest
来源：http://kxy.ehwqpu.com

[U118] JS：开发服务器
来源：http://yjs.snrcjt.cn

npm i -D vite;  npx vite
来源：http://qkd.meibo888.top

[U119] JS：生产构建
来源：http://zau.hammf.cn

npx vite build
来源：http://jya.shuidangran.top

[U120] JS：读取环境变量（Vite）
来源：http://jdz.ybcxt.top

import.meta.env.VITE_API_URL
来源：http://keb.fehbvm.com

================================================================================
来源：http://pzs.yongpay.top

统计汇总
来源：http://lcb.yj202588.top

================================================================================
来源：http://mlb.zhengqikj.top

按语言统计（条）：
来源：http://nne.jyoumei.cn

Python ......... 252
来源：http://uly.ctjpmb.com

PHP ............ 252
来源：http://kjq.tian-w.cn

JavaScript ..... 252
来源：http://mdo.gogol.net.cn

TypeScript ..... 212
来源：http://zwf.pengpengdd.cyou

Java ........... 212
来源：http://wsk.zhoulong.xyz

Go ............. 212
来源：http://yog.cheryme.top

Ruby ........... 212
来源：http://ugn.guannengcc.top

C# ............. 212
来源：http://ehy.sjlbkw.cn


<!-- 参考信息 -->