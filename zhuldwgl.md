代发 wailian999

[T45] Perl：数组遍历
来源：http://iri.bbcook.cn

for my $x (@arr) { print $x; }
来源：http://xxl.cqqwz.cn

[T46] Perl：哈希操作
来源：http://olo.ctjpmb.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gvy.ywan-chungtsiang.top

[T47] Perl：正则捕获
来源：http://fkm.316326.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://bzl.ydzc1.top

[T48] Perl：正则替换
来源：http://owd.hammf.cn

$s =~ s/old/new/g;
来源：http://zbk.gaohongyu789.top

[T49] Perl：函数
来源：http://big.nanxuanxn.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://eie.hcnkem.com

[T50] Perl：逐行读文件
来源：http://dfg.meibo888.top

open my $fh, "<", "a.txt" or die $!;
来源：http://xxu.sjlbkw.cn

while (my $line = <$fh>) { print $line; }
来源：http://pjm.chenjidiqi.icu

[T51] Scala：Hello World
来源：http://ijy.fanxiaobao.xyz

println("Hello")
来源：http://vhv.mhx1999.top

[T52] Scala：变量
来源：http://mlq.jinqigufen.top

val a = 1;  var b = 2
来源：http://msy.shzxlz.cn

[T53] Scala：字符串插值
来源：http://efa.sufxvd.cn

s"值: $b"
来源：http://srp.xuetiantiany.cn

[T54] Scala：集合映射
来源：http://oip.hysaishi.cn

List(1, 2, 3).map(_ * 2)
来源：http://hml.redwolf501.top

[T55] Scala：集合过滤
来源：http://jdo.quarkkingdee.top

List(1, 2, 3).filter(_ > 1)
来源：http://hvn.haohaochexian.top

[T56] Scala：样例类
来源：http://fdd.fzhhl.top

case class User(name: String, age: Int)
来源：http://lqv.zhaomingkeji.xyz

[T57] Scala：模式匹配
来源：http://vdk.shangyingyoupin.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://kxy.zhixingplan.top

[T58] Scala：函数定义
来源：http://pvn.chenzaomai.com

def add(a: Int, b: Int): Int = a + b
来源：http://hbo.tanke756.top

[T59] Scala：循环
来源：http://kdp.zhengqikj.top

for (i <- 1 to 10) println(i)
来源：http://soa.wangshuangyany.cn

[T60] Scala：折叠
来源：http://hno.jlsjyb.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qio.ydzc1.top

================================================================================
来源：http://xpw.jinghuilouyu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cdp.feifeiyinyue.top

================================================================================
来源：http://sbi.fehbvm.com

[U01] Py：创建虚拟环境
来源：http://ifd.yuanzhike.top

python -m venv .venv && source .venv/bin/activate
来源：http://xpd.smart0.xyz

[U02] Py：导出 / 安装依赖
来源：http://phz.ywan-chungtsiang.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hlk.guowangkeji.top

[U03] Py：加载 .env 配置
来源：http://lxp.uphjek.com

from dotenv import load_dotenv; load_dotenv()
来源：http://agd.yueranfly.top

[U04] Py：变量调试打印
来源：http://uvk.shanyushiyangtech.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xxd.haohaochexian.top

[U05] Py：列表去重且保序
来源：http://zsq.feifeiyinyue.top

list(dict.fromkeys(arr))
来源：http://wwk.meibo888.top

[U06] Py：合并两个字典
来源：http://sos.gotoacloud.top

{**a, **b}
来源：http://xds.shanyushiyangkeji.top

[U07] Py：反转字典键值
来源：http://kip.tianlin.xyz

{v: k for k, v in d.items()}
来源：http://rsv.tian-w.cn

[U08] Py：展平二维列表
来源：http://dlk.epnwcf.com

[y for x in nested for y in x]
来源：http://nyy.zycfv.cn

[U09] Py：字典取最大值的键
来源：http://cje.xuetiantiany.cn

max(d, key=d.get)
来源：http://gzm.fktsv.cn

[U10] Py：按值排序字典
来源：http://wzm.shangyingyoupin.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wde.zhoulong.xyz

[U11] Py：生成器表达式
来源：http://dvz.0kj1m.cn

(x * 2 for x in arr)
来源：http://yjo.birdmap.top

[U12] Py：取出现最多的 3 个元素
来源：http://gsm.ydzc1.top

Counter(arr).most_common(3)
来源：http://mxe.zhaomingkeji.xyz

[U13] Py：固定长度队列
来源：http://bab.zhiwuduotai.top

deque(maxlen=10)
来源：http://lvh.aibaodan.cn

[U14] Py：分组收集到列表
来源：http://ovw.ivvv.top

defaultdict(list)
来源：http://fsj.zhoulong.xyz

[U15] Py：高精度计时
来源：http://cyv.gaohongyu789.top

t = time.perf_counter()
来源：http://utz.jqgufenzy.top

[U16] Py：命令行参数解析
来源：http://zwv.wangdashe.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://isy.cqqwz.cn

[U17] Py：初始化日志
来源：http://arw.hnqzz.top

logging.basicConfig(level=logging.INFO)
来源：http://pku.yongpay.top

[U18] Py：预编译正则
来源：http://lnp.shangyingyoupin.top

pat = re.compile(r"\d+")
来源：http://mwh.hfpthk.cn

[U19] Py：正则替换带回调
来源：http://fac.xuanzx.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xwv.shangyingyoupin.top

[U20] Py：缓存函数结果
来源：http://ncy.uphjek.com

@functools.lru_cache(maxsize=None)
来源：http://ndm.shanyushiyangkeji.top

[U21] Py：自定义上下文管理器
来源：http://fql.xinyue.icu

@contextlib.contextmanager
来源：http://hjk.nwbrower.top

[U22] Py：矩阵转置
来源：http://pjf.hywenlv.cn

list(zip(*m))
来源：http://bdo.vqdsnc.cn

[U23] Py：分块读取大文件
来源：http://afv.yuanzhike.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://flc.jianghu66.top

[U24] Py：路径操作
来源：http://aha.shanyushiyangtech.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fbc.hesvh.cn

[U25] Py：CSV 按字典读
来源：http://cdt.guowangkeji.top

csv.DictReader(f)
来源：http://yci.gogol.net.cn

[U26] Py：并发下载
来源：http://sjq.redwolf501.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://uov.shanyushiyangtech.top

[U27] Py：异步 HTTP
来源：http://aty.shzxlz.cn

aiohttp.ClientSession() 配合 async with
来源：http://cyq.yuxming.cn

[U28] Py：类型别名
来源：http://qpe.yuxming.cn

UserId = int
来源：http://epl.wangdashe.top

[U29] Py：属性校验
来源：http://ldk.cqqwz.cn

@property 与 @x.setter 配合
来源：http://baf.guowangkeji.top

[U30] Py：数据类
来源：http://mll.hcnkem.com

@dataclass(slots=True)
来源：http://ukb.feifeiyinyue.top

[U31] Py：单测
来源：http://bqa.cdnleiting.top

python -m pytest -q
来源：http://rmn.sxryk.cn

[U32] Py：代码格式化
来源：http://wqr.hcnkem.com

ruff format . && ruff check --fix .
来源：http://umx.epnwcf.com

[U33] Py：打包发布
来源：http://kzf.jinqigufen.top

python -m build  （依赖 pyproject.toml）
来源：http://sdk.cucudq.cn

[U34] Py：判断编码
来源：http://wwj.zhaomingkeji.xyz

chardet.detect(raw)
来源：http://txd.jinghuilouyu.cn

[U35] Py：发送邮件
来源：http://trf.pengpengdd.cyou

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://psz.ywan-chungtsiang.top

[U36] Py：定时任务
来源：http://upm.gotoacloud.top

schedule.every(10).minutes.do(job)
来源：http://vjq.feifeiyinyue.top

[U37] Py：读写 Excel
来源：http://gld.zhoulong.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://wcc.shuidangran.top

[U38] Py：获取脚本所在目录
来源：http://kjh.jqgfzy.top

Path(__file__).resolve().parent
来源：http://wcx.jqgufenzy.top

[U39] Py：判断是否在交互环境
来源：http://vda.zhaomingkeji.xyz

sys.stdout.isatty()
来源：http://nqq.hammf.cn

[U40] Py：打印到标准错误
来源：http://hfl.jinqigfzy.top

print("err", file=sys.stderr)
来源：http://kaa.chenjidiqi.icu

[U41] PHP：初始化 Composer 项目
来源：http://wlt.tarul.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://llx.jinqigufen.top

[U42] PHP：PSR-4 自动加载
来源：http://csk.zhongyouzk.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://juh.0kj1m.cn

[U43] PHP：声明命名空间
来源：http://nuu.nanxuanxn.top

namespace App\Http;
来源：http://qnz.sweek.top

[U44] PHP：开启严格类型
来源：http://lbq.yongpay.top

declare(strict_types=1);
来源：http://nds.yanxiufei.cn

[U45] PHP：类型声明与返回类型
来源：http://wkq.ehwqpu.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://lpo.zhijiandao.cn

[U46] PHP：可空类型
来源：http://cpo.zhijiandao.cn

?string $name = null
来源：http://zfv.cheryme.top

[U47] PHP：联合类型
来源：http://vbh.hongshengwenyu.top

int|string $id
来源：http://iyh.sysykeji.top

[U48] PHP：纯枚举
来源：http://ozn.yongpay.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lln.jqgfzy.top

[U49] PHP：只读属性
来源：http://hwq.zhijiandao.cn

public readonly string $name
来源：http://het.gotoacloud.top

[U50] PHP：构造器属性提升
来源：http://xwj.hysaishi.cn

public function __construct(private int $id) {}
来源：http://zjy.tianlin.xyz

[U51] PHP：数组解构
来源：http://sxu.hywenlv.cn

[$a, $b] = $arr;
来源：http://sfc.yuxming.cn

[U52] PHP：箭头函数
来源：http://edx.havefunace.top

$double = fn($x) => $x * 2;
来源：http://gjc.pycfn.com

[U53] PHP：空合并运算符
来源：http://ycl.cdnleiting.top

$v = $a ?? $b ?? "default";
来源：http://iar.shanyushiyangkeji.top

[U54] PHP：空安全调用
来源：http://pkb.cucudq.cn

$obj?->method()
来源：http://hje.feifeiyinyue.top

[U55] PHP：match 表达式
来源：http://niu.fanxiaobao.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hvz.fzhhl.top

[U56] PHP：命名参数
来源：http://clz.gotoacloud.top

f(a: 1, b: 2)
来源：http://eyh.9152youxi.cn

[U57] PHP：字符串插值
来源：http://sqc.snrcjt.cn

"值: {$a}"
来源：http://lon.quarkkingdee.top

[U58] PHP：数组三件套
来源：http://udi.zhixingplan.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://htb.zhiwuduotai.top

[U59] PHP：自定义排序
来源：http://fem.guannengcc.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lke.pengpengdd.cyou

[U60] PHP：JSON 编解码
来源：http://whx.ivvv.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gss.ydjk.org.cn

[U61] PHP：正则
来源：http://eud.haohaochexian.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://sgw.haohaochexian.top

[U62] PHP：日期对象
来源：http://zzf.ctjpmb.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://dku.shuidangran.top

[U63] PHP：文件读写
来源：http://paz.shzxlz.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://aue.jianghu66.top

[U64] PHP：目录遍历
来源：http://qkx.c1oappe.top

glob("dir/*.php");  scandir("dir");
来源：http://gdw.zhoulong.xyz

[U65] PHP：会话
来源：http://nwx.xylfe.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://cta.hywenlv.cn

[U66] PHP：设置 Cookie
来源：http://pld.jinyuanbaomall.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cfq.cheryme.top

[U67] PHP：处理文件上传
来源：http://lya.yonumen.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bvc.tanke756.top

[U68] PHP：PDO 连接
来源：http://cpb.52xcode.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://dxn.xuanzx.com

[U69] PHP：PDO 预处理
来源：http://kpa.yuxming.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wfl.yuanzhike.top

[U70] PHP：PDO 事务
来源：http://iae.hesvh.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://aoc.hammf.cn

[U71] PHP：抛出异常
来源：http://vsz.shanyushiyangtech.top

throw new RuntimeException("失败", 500);
来源：http://cng.yueranfly.top

[U72] PHP：写错误日志
来源：http://anq.birdmap.top

error_log("失败: " . $e->getMessage());
来源：http://dkp.jqgufenzy.top

[U73] PHP：读取 ini 配置
来源：http://awn.fengsongda.top

parse_ini_file("config.ini", true)
来源：http://rjs.tianlin.xyz

[U74] PHP：读取环境变量
来源：http://owu.dashuyun.cn

getenv("APP_ENV") ?: "production"
来源：http://iyp.xuetiantiany.cn

[U75] PHP：依赖注入
来源：http://yfc.mhx1999.top

composer require psr/container
来源：http://btt.jianghu66.top

[U76] PHP：简单路由
来源：http://jnq.dianchejie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fsz.c1oappe.top

[U77] PHP：模板渲染
来源：http://eeb.shanyushiyangtech.top

composer require twig/twig
来源：http://nsn.tian-w.cn

[U78] PHP：单元测试
来源：http://kjv.wangshuangyany.cn

composer require --dev phpunit/phpunit
来源：http://yzw.ydzc1.top

[U79] PHP：静态分析
来源：http://wyx.xuanzx.com

composer require --dev phpstan/phpstan
来源：http://xqk.dashuyun.cn

[U80] PHP：代码规范修复
来源：http://zor.hammf.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://zgd.birdmap.top

[U81] JS：初始化项目
来源：http://bfl.sufxvd.cn

npm init -y;  npm i express
来源：http://trt.zdbjq.cn

[U82] JS：package.json 脚本
来源：http://xdt.cheryme.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ngf.quarkkingdee.top

[U83] JS：ES Module 导入导出
来源：http://hrd.c1oappe.top

export const a = 1;  import { a } from "./m.js";
来源：http://qpf.zycfv.cn

[U84] JS：CommonJS 写法
来源：http://xpn.zhongyouzk.top

module.exports = { a };  const { a } = require("./m");
来源：http://okz.ydzc1.top

[U85] JS：可选链
来源：http://hky.ydjk.org.cn

a?.b?.c
来源：http://hej.quarkkingdee.top

[U86] JS：空值合并
来源：http://hfd.ywan-chungtsiang.top

a ?? b
来源：http://yxc.yj202588.top

[U87] JS：解构默认值
来源：http://puy.hcnkem.com

const { a = 1, b = 2 } = obj;
来源：http://pss.zdqjudy.top

[U88] JS：对象展开合并
来源：http://muz.bbcook.cn

{ ...a, ...b }
来源：http://bjh.xingfuxueyuan.xyz

[U89] JS：数组去重
来源：http://ejk.andypj.xyz

[...new Set(arr)]
来源：http://dop.vqdsnc.cn

[U90] JS：数字数组排序
来源：http://ddl.aizwys.cn

[...arr].sort((a, b) => a - b)
来源：http://gdz.redwolf501.top

[U91] JS：对象键值遍历
来源：http://htm.iojbl.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://grb.svipenyu.cn

[U92] JS：深拷贝
来源：http://zme.hammf.cn

structuredClone(obj)
来源：http://tbw.uphjek.com

[U93] JS：模板字符串
来源：http://scu.ydjk.org.cn

`共 ${n} 条`
来源：http://lpe.yuanzhike.top

[U94] JS：箭头函数
来源：http://viy.xinyue.icu

const double = x => x * 2;
来源：http://zkw.52xcode.cn

[U95] JS：Promise 包装
来源：http://ddo.aizwys.cn

new Promise((resolve, reject) => {})
来源：http://vdu.yuxming.cn

[U96] JS：async/await 与异常
来源：http://anc.ppjwa.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://elk.jqgfzy.top

[U97] JS：并发请求
来源：http://vqp.sjlbkw.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://vkf.xingfuxueyuan.xyz

[U98] JS：fetch 带 JSON
来源：http://czi.ybcxt.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ima.bjfxy.top

[U99] JS：事件监听
来源：http://kqp.smart0.xyz

el.addEventListener("click", e => {})
来源：http://rdb.snrcjt.cn

[U100] JS：DOM 查询
来源：http://whn.meibo888.top

document.querySelector(".item")
来源：http://iod.fktsv.cn

[U101] JS：classList 操作
来源：http://qoj.chenzaomai.com

el.classList.toggle("active")
来源：http://uxw.yuanzhike.top

[U102] JS：本地存储
来源：http://kld.zhaomingkeji.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://ypp.zhengqikj.top

[U103] JS：定时器
来源：http://gey.316326.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nxd.ivvv.top

[U104] JS：防抖
来源：http://nql.gogol.net.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eog.kuanghao11.cn

[U105] JS：节流
来源：http://wvi.vehdjk.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wov.yangfankeji.com

[U106] JS：日期格式化
来源：http://uzm.aizwys.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://tts.zhiwuduotai.top

[U107] JS：数字千分位
来源：http://jkr.hammf.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rxf.ydjk.org.cn

[U108] JS：随机整数
来源：http://mty.ydjk.org.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dbw.shuidangran.top

[U109] JS：数组分组
来源：http://sbz.xziqi.cn

Object.groupBy(arr, x => x.type)
来源：http://fat.andypj.xyz

[U110] JS：数组分块
来源：http://cju.zhongyouzk.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://olb.ehwqpu.com

[U111] JS：对象转 Map
来源：http://arf.hcnkem.com

new Map(Object.entries(obj))
来源：http://jyx.hywenlv.cn

[U112] JS：字符串补位
来源：http://nka.zhoulong.xyz

"7".padStart(3, "0")
来源：http://exx.ctjpmb.com

[U113] JS：正则替换全部
来源：http://nwv.cqqwz.cn

s.replaceAll("a", "b")
来源：http://vgl.iojbl.cn

[U114] JS：JSON 深比较
来源：http://jyo.jinyuanbaomall.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://pqv.ywan-chungtsiang.top

[U115] JS：生成 UUID
来源：http://jls.ctjpmb.com

crypto.randomUUID()
来源：http://kgp.guowangkeji.top

[U116] JS：类型检查（JSDoc）
来源：http://fkz.chenlongwang.top

/** @param {string} name */ function f(name) {}
来源：http://ium.yj20258888.top

[U117] JS：单元测试
来源：http://jmj.cqqwz.cn

npm i -D vitest;  npx vitest
来源：http://gmi.iojbl.cn

[U118] JS：开发服务器
来源：http://now.yonumen.top

npm i -D vite;  npx vite
来源：http://zcl.zhoulong.xyz

[U119] JS：生产构建
来源：http://ppc.birdmap.top

npx vite build
来源：http://kkb.quarkkingdee.top

[U120] JS：读取环境变量（Vite）
来源：http://qxp.jyoumei.cn

import.meta.env.VITE_API_URL
来源：http://ksg.fktsv.cn

================================================================================
来源：http://umz.quarkkingdee.top

统计汇总
来源：http://jgy.shzxlz.cn

================================================================================
来源：http://wzx.shanyushiyangtech.top

按语言统计（条）：
来源：http://nrg.zhaomingkeji.xyz

Python ......... 252
来源：http://jdt.yangfankeji.com

PHP ............ 252
来源：http://pdt.hnxiangtu.top

JavaScript ..... 252
来源：http://bfn.chenjidiqi.icu

TypeScript ..... 212
来源：http://aln.gogol.net.cn

Java ........... 212
来源：http://tzg.zdbjq.cn

Go ............. 212
来源：http://wvn.epnwcf.com

Ruby ........... 212
来源：http://dlr.9152youxi.cn

C# ............. 212
来源：http://rjv.bbcook.cn

C .............. 30
来源：http://oqo.fengsongda.top

C++ ............ 30
来源：http://nrf.xinyue.icu

SQL ............ 90
来源：http://xbv.chenlongwang.top

Bash ........... 80
来源：http://fhx.fzhhl.top

Kotlin ......... 15
来源：http://owg.cheryme.top

Swift .......... 15
来源：http://xsf.yonumen.top

Lua ............ 10
来源：http://ddg.jyoumei.cn

Perl ........... 10
来源：http://ksl.dianchejie.cn

Scala .......... 10
来源：http://bzn.quarkkingdee.top

------------------------------------
来源：http://qhc.dianchejie.cn

合计 ........... 2106 条
来源：http://hsr.yanxiufei.cn

按章节统计：
来源：http://daa.tarul.cn


<!-- 参考信息 -->