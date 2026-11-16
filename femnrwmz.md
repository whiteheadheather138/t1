代发 wailian999

[T43] Perl：字符串插值
来源：http://gcn.jinqigfzy.top

"值: $a"
来源：http://omu.bjfxy.top

[T44] Perl：条件
来源：http://usx.yj20258.top

if ($a > 0) { print "正"; }
来源：http://knd.zhixingplan.top

[T45] Perl：数组遍历
来源：http://coh.jiagoushi.top

for my $x (@arr) { print $x; }
来源：http://cei.meibo888.top

[T46] Perl：哈希操作
来源：http://ssc.9152youxi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rcw.sjlbkw.cn

[T47] Perl：正则捕获
来源：http://wdz.ppjwa.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://csv.zdqjudy.top

[T48] Perl：正则替换
来源：http://rpn.gotoacloud.top

$s =~ s/old/new/g;
来源：http://gib.nwbrower.top

[T49] Perl：函数
来源：http://tdg.birdmap.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://frk.ybcxt.top

[T50] Perl：逐行读文件
来源：http://klc.xylfe.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zbv.haohaochexian.top

while (my $line = <$fh>) { print $line; }
来源：http://cxe.zhoulong.xyz

[T51] Scala：Hello World
来源：http://xzq.gogol.net.cn

println("Hello")
来源：http://xzo.jqgufenzy.top

[T52] Scala：变量
来源：http://isl.bjfxy.top

val a = 1;  var b = 2
来源：http://tbi.shzxlz.cn

[T53] Scala：字符串插值
来源：http://uvz.xuetiantiany.cn

s"值: $b"
来源：http://hki.fengsongda.top

[T54] Scala：集合映射
来源：http://gje.andypj.xyz

List(1, 2, 3).map(_ * 2)
来源：http://dni.shangyingyoupin.top

[T55] Scala：集合过滤
来源：http://kpn.xinyue.icu

List(1, 2, 3).filter(_ > 1)
来源：http://npa.ehwqpu.com

[T56] Scala：样例类
来源：http://fvb.vqdsnc.cn

case class User(name: String, age: Int)
来源：http://sns.hysaishi.cn

[T57] Scala：模式匹配
来源：http://iij.jinyuanbaomall.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ild.yonumen.top

[T58] Scala：函数定义
来源：http://cof.yj202588.top

def add(a: Int, b: Int): Int = a + b
来源：http://bkf.yfazqb.com

[T59] Scala：循环
来源：http://uqb.nanxinkj.top

for (i <- 1 to 10) println(i)
来源：http://dxm.guowangkeji.top

[T60] Scala：折叠
来源：http://qgk.ydjk.org.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xry.pycfn.com

================================================================================
来源：http://zfk.zhiwuduotai.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vxd.vqdsnc.cn

================================================================================
来源：http://mke.zdqjudy.top

[U01] Py：创建虚拟环境
来源：http://khk.hysaishi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://tvf.chenzaomai.com

[U02] Py：导出 / 安装依赖
来源：http://ogc.pycfn.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://elg.hysaishi.cn

[U03] Py：加载 .env 配置
来源：http://orc.sxryk.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://qnu.yvedp.cn

[U04] Py：变量调试打印
来源：http://jwi.fzhhl.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ybe.nanxinkj.top

[U05] Py：列表去重且保序
来源：http://ogj.andypj.xyz

list(dict.fromkeys(arr))
来源：http://pic.0kj1m.cn

[U06] Py：合并两个字典
来源：http://ysv.chenzaomai.com

{**a, **b}
来源：http://elw.nanxuanxn.top

[U07] Py：反转字典键值
来源：http://hoa.sufxvd.cn

{v: k for k, v in d.items()}
来源：http://hdt.xuanzx.com

[U08] Py：展平二维列表
来源：http://dmh.zhongyouzk.top

[y for x in nested for y in x]
来源：http://rjh.mhx1999.top

[U09] Py：字典取最大值的键
来源：http://cde.dashuyun.cn

max(d, key=d.get)
来源：http://lqo.cucudq.cn

[U10] Py：按值排序字典
来源：http://etl.iojbl.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wih.wangdashe.top

[U11] Py：生成器表达式
来源：http://jys.xingfuxueyuan.xyz

(x * 2 for x in arr)
来源：http://gsn.hfpthk.cn

[U12] Py：取出现最多的 3 个元素
来源：http://grx.ppjwa.cn

Counter(arr).most_common(3)
来源：http://oes.shanyushiyangkeji.top

[U13] Py：固定长度队列
来源：http://stg.hnqzz.top

deque(maxlen=10)
来源：http://eug.jinyuanbaomall.cn

[U14] Py：分组收集到列表
来源：http://mhw.zhengqikj.top

defaultdict(list)
来源：http://omx.zhongyouzk.top

[U15] Py：高精度计时
来源：http://rqq.ppjwa.cn

t = time.perf_counter()
来源：http://yba.andypj.xyz

[U16] Py：命令行参数解析
来源：http://hts.fktsv.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://skd.hammf.cn

[U17] Py：初始化日志
来源：http://gbs.birdmap.top

logging.basicConfig(level=logging.INFO)
来源：http://pmj.chenjidiqi.icu

[U18] Py：预编译正则
来源：http://lec.xylfe.cn

pat = re.compile(r"\d+")
来源：http://oqh.jqgfzy.top

[U19] Py：正则替换带回调
来源：http://fuq.shzxlz.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ffx.xinyue.icu

[U20] Py：缓存函数结果
来源：http://yhx.quarkkingdee.top

@functools.lru_cache(maxsize=None)
来源：http://peo.tarul.cn

[U21] Py：自定义上下文管理器
来源：http://rar.dianchejie.cn

@contextlib.contextmanager
来源：http://xbd.sjlbkw.cn

[U22] Py：矩阵转置
来源：http://kat.bbcook.cn

list(zip(*m))
来源：http://qeh.yangfankeji.com

[U23] Py：分块读取大文件
来源：http://ikf.redwolf501.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jel.dianchejie.cn

[U24] Py：路径操作
来源：http://asm.ehwqpu.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://amy.hnxiangtu.top

[U25] Py：CSV 按字典读
来源：http://fxw.zdbjq.cn

csv.DictReader(f)
来源：http://kjo.meibo888.top

[U26] Py：并发下载
来源：http://vsd.hammf.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yod.vqdsnc.cn

[U27] Py：异步 HTTP
来源：http://sul.sweek.top

aiohttp.ClientSession() 配合 async with
来源：http://pvt.zhoulong.xyz

[U28] Py：类型别名
来源：http://ury.bjfxy.top

UserId = int
来源：http://xkr.cashguo.top

[U29] Py：属性校验
来源：http://exi.jinqigfzy.top

@property 与 @x.setter 配合
来源：http://ehv.hcnkem.com

[U30] Py：数据类
来源：http://lvf.jinqigfzy.top

@dataclass(slots=True)
来源：http://yyv.c1oappe.top

[U31] Py：单测
来源：http://ssq.zhaomingkeji.xyz

python -m pytest -q
来源：http://ega.fehbvm.com

[U32] Py：代码格式化
来源：http://xmd.ehwqpu.com

ruff format . && ruff check --fix .
来源：http://plj.uphjek.com

[U33] Py：打包发布
来源：http://rro.vehdjk.com

python -m build  （依赖 pyproject.toml）
来源：http://fzc.hysaishi.cn

[U34] Py：判断编码
来源：http://evi.tarul.cn

chardet.detect(raw)
来源：http://rxw.gaohongyu789.top

[U35] Py：发送邮件
来源：http://jem.sweek.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bsx.sweek.top

[U36] Py：定时任务
来源：http://ykn.hywenlv.cn

schedule.every(10).minutes.do(job)
来源：http://gln.pengpengdd.cyou

[U37] Py：读写 Excel
来源：http://hld.nanxinkj.top

pandas.read_excel / DataFrame.to_excel
来源：http://ebw.pycfn.com

[U38] Py：获取脚本所在目录
来源：http://rmu.aibaodan.cn

Path(__file__).resolve().parent
来源：http://zig.xinyue.icu

[U39] Py：判断是否在交互环境
来源：http://zff.chenlongwang.top

sys.stdout.isatty()
来源：http://nfu.tianlin.xyz

[U40] Py：打印到标准错误
来源：http://zpb.hcnkem.com

print("err", file=sys.stderr)
来源：http://qop.redwolf501.top

[U41] PHP：初始化 Composer 项目
来源：http://ydt.yvedp.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://sqc.yonumen.top

[U42] PHP：PSR-4 自动加载
来源：http://qpd.jlsjyb.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rbg.dashuyun.cn

[U43] PHP：声明命名空间
来源：http://zcl.jlsjyb.cn

namespace App\Http;
来源：http://nya.zhengqikj.top

[U44] PHP：开启严格类型
来源：http://hzy.chenlongwang.top

declare(strict_types=1);
来源：http://oso.tian-w.cn

[U45] PHP：类型声明与返回类型
来源：http://hlu.zycfv.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ptr.tian-w.cn

[U46] PHP：可空类型
来源：http://uuq.sysykeji.top

?string $name = null
来源：http://csa.ivvv.top

[U47] PHP：联合类型
来源：http://vqs.iojbl.cn

int|string $id
来源：http://oyp.yangfankeji.com

[U48] PHP：纯枚举
来源：http://gfv.snrcjt.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lgs.gogol.net.cn

[U49] PHP：只读属性
来源：http://vsv.xinyue.icu

public readonly string $name
来源：http://ahx.shanyushiyangtech.top

[U50] PHP：构造器属性提升
来源：http://jky.vehdjk.com

public function __construct(private int $id) {}
来源：http://bpi.cqqwz.cn

[U51] PHP：数组解构
来源：http://xbg.nanxinkj.top

[$a, $b] = $arr;
来源：http://grj.9152youxi.cn

[U52] PHP：箭头函数
来源：http://gfu.tian-w.cn

$double = fn($x) => $x * 2;
来源：http://jis.bbcook.cn

[U53] PHP：空合并运算符
来源：http://mdd.uphjek.com

$v = $a ?? $b ?? "default";
来源：http://jdi.bbcook.cn

[U54] PHP：空安全调用
来源：http://qrm.zhijiandao.cn

$obj?->method()
来源：http://bru.hcnkem.com

[U55] PHP：match 表达式
来源：http://tbu.andypj.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vxj.ehwqpu.com

[U56] PHP：命名参数
来源：http://oue.shuidangran.top

f(a: 1, b: 2)
来源：http://xiw.jinyuanbaomall.cn

[U57] PHP：字符串插值
来源：http://nxw.hnxiangtu.top

"值: {$a}"
来源：http://hln.hfpthk.cn

[U58] PHP：数组三件套
来源：http://ent.quarkkingdee.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pzw.jinqigufen.top

[U59] PHP：自定义排序
来源：http://fkp.zdqjudy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xzr.tanke756.top

[U60] PHP：JSON 编解码
来源：http://jkd.hammf.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zlq.uphjek.com

[U61] PHP：正则
来源：http://ces.smart0.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://aks.fzhhl.top

[U62] PHP：日期对象
来源：http://hiq.tianlin.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pds.yonumen.top

[U63] PHP：文件读写
来源：http://hog.quarkkingdee.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xiy.xingfuxueyuan.xyz

[U64] PHP：目录遍历
来源：http://uta.fzhhl.top

glob("dir/*.php");  scandir("dir");
来源：http://ubh.ppjwa.cn

[U65] PHP：会话
来源：http://mnx.xziqi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://zng.nanxinkj.top

[U66] PHP：设置 Cookie
来源：http://dex.9152youxi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vpz.zhiwuduotai.top

[U67] PHP：处理文件上传
来源：http://jix.chenjidiqi.icu

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bij.quarkkingdee.top

[U68] PHP：PDO 连接
来源：http://woq.pengpengdd.cyou

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://boj.hcnkem.com

[U69] PHP：PDO 预处理
来源：http://exo.ybcxt.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dws.ydzc1.top

[U70] PHP：PDO 事务
来源：http://jbj.hesvh.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://sxu.yj20258888.top

[U71] PHP：抛出异常
来源：http://hjh.sysykeji.top

throw new RuntimeException("失败", 500);
来源：http://hmj.quarkkingdee.top

[U72] PHP：写错误日志
来源：http://kfr.zhiwuduotai.top

error_log("失败: " . $e->getMessage());
来源：http://nsz.epnwcf.com

[U73] PHP：读取 ini 配置
来源：http://lkh.shangyingyoupin.top

parse_ini_file("config.ini", true)
来源：http://rhw.shzxlz.cn

[U74] PHP：读取环境变量
来源：http://hkt.gogol.net.cn

getenv("APP_ENV") ?: "production"
来源：http://mxe.ybcxt.top

[U75] PHP：依赖注入
来源：http://stc.0kj1m.cn

composer require psr/container
来源：http://bcq.shanyushiyangkeji.top

[U76] PHP：简单路由
来源：http://yoz.redwolf501.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://omt.cashguo.top

[U77] PHP：模板渲染
来源：http://qbz.sufxvd.cn

composer require twig/twig
来源：http://yjr.wangshuangyany.cn

[U78] PHP：单元测试
来源：http://lge.jqgfzy.top

composer require --dev phpunit/phpunit
来源：http://icd.meibo888.top

[U79] PHP：静态分析
来源：http://noy.fzhhl.top

composer require --dev phpstan/phpstan
来源：http://fmd.bjfxy.top

[U80] PHP：代码规范修复
来源：http://cxu.0kj1m.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://pre.sufxvd.cn

[U81] JS：初始化项目
来源：http://hbs.guowangkeji.top

npm init -y;  npm i express
来源：http://oxb.ydzc1.top

[U82] JS：package.json 脚本
来源：http://xoh.jinghuilouyu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://eqd.jinqigfzy.top

[U83] JS：ES Module 导入导出
来源：http://uvu.tianlin.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://vqm.nanxuanxn.top

[U84] JS：CommonJS 写法
来源：http://yrd.hnqzz.top

module.exports = { a };  const { a } = require("./m");
来源：http://bzx.ctjpmb.com

[U85] JS：可选链
来源：http://lym.zhiwuduotai.top

a?.b?.c
来源：http://xnt.zdqjudy.top

[U86] JS：空值合并
来源：http://xuv.cqqwz.cn

a ?? b
来源：http://jtb.andypj.xyz

[U87] JS：解构默认值
来源：http://nhn.xuanzx.com

const { a = 1, b = 2 } = obj;
来源：http://nhp.yfazqb.com

[U88] JS：对象展开合并
来源：http://nyo.gaohongyu789.top

{ ...a, ...b }
来源：http://kiz.nanxinkj.top

[U89] JS：数组去重
来源：http://njq.ydzc1.top

[...new Set(arr)]
来源：http://oqc.chenjidiqi.icu

[U90] JS：数字数组排序
来源：http://jhg.tanke756.top

[...arr].sort((a, b) => a - b)
来源：http://adz.gaohongyu789.top

[U91] JS：对象键值遍历
来源：http://gea.haohaochexian.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pvk.tarul.cn

[U92] JS：深拷贝
来源：http://saz.yueranfly.top

structuredClone(obj)
来源：http://epc.pengpengdd.cyou

[U93] JS：模板字符串
来源：http://xkj.zhixingplan.top

`共 ${n} 条`
来源：http://yrg.c1oappe.top

[U94] JS：箭头函数
来源：http://oyg.yj202588.top

const double = x => x * 2;
来源：http://fow.yj20258.top

[U95] JS：Promise 包装
来源：http://dkt.xuanzx.com

new Promise((resolve, reject) => {})
来源：http://evp.xuanzx.com

[U96] JS：async/await 与异常
来源：http://ifg.fengsongda.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rgm.yanxiufei.cn

[U97] JS：并发请求
来源：http://auu.hongshengwenyu.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://tuu.cdnleiting.top

[U98] JS：fetch 带 JSON
来源：http://nwj.shzxlz.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://igx.jinqigufen.top

[U99] JS：事件监听
来源：http://bbd.yvedp.cn

el.addEventListener("click", e => {})
来源：http://llu.guannengcc.top

[U100] JS：DOM 查询
来源：http://udl.wangdashe.top

document.querySelector(".item")
来源：http://leh.hywenlv.cn

[U101] JS：classList 操作
来源：http://yle.shanyushiyangtech.top

el.classList.toggle("active")
来源：http://rcb.zdqjudy.top

[U102] JS：本地存储
来源：http://fyp.yongpay.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://pyx.ydzc1.top

[U103] JS：定时器
来源：http://agh.0kj1m.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ruy.vqdsnc.cn

[U104] JS：防抖
来源：http://oez.yj20258888.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://daq.316326.xyz

[U105] JS：节流
来源：http://hbh.cheryme.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fhm.wangshuangyany.cn

[U106] JS：日期格式化
来源：http://tym.hongshengwenyu.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pih.zycfv.cn

[U107] JS：数字千分位
来源：http://qnn.xuanzx.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fxo.jiagoushi.top

[U108] JS：随机整数
来源：http://pdg.fehbvm.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pes.zdbjq.cn

[U109] JS：数组分组
来源：http://rgu.bjfxy.top

Object.groupBy(arr, x => x.type)
来源：http://usl.aibaodan.cn

[U110] JS：数组分块
来源：http://lxn.xuetiantiany.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://atb.snrcjt.cn

[U111] JS：对象转 Map
来源：http://yao.tian-w.cn

new Map(Object.entries(obj))
来源：http://ufy.zhoulong.xyz

[U112] JS：字符串补位
来源：http://zbw.shuidangran.top

"7".padStart(3, "0")
来源：http://plc.316326.xyz

[U113] JS：正则替换全部
来源：http://onp.hongshengwenyu.top

s.replaceAll("a", "b")
来源：http://nyo.zhiwuduotai.top

[U114] JS：JSON 深比较
来源：http://zmt.sjlbkw.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://lim.hnqzz.top

[U115] JS：生成 UUID
来源：http://gqm.cqqwz.cn

crypto.randomUUID()
来源：http://vzb.0kj1m.cn

[U116] JS：类型检查（JSDoc）
来源：http://beh.zhijiandao.cn

/** @param {string} name */ function f(name) {}
来源：http://eci.jlsjyb.cn

[U117] JS：单元测试
来源：http://ghx.jiagoushi.top

npm i -D vitest;  npx vitest
来源：http://tgi.yj20258.top

[U118] JS：开发服务器
来源：http://otf.fktsv.cn

npm i -D vite;  npx vite
来源：http://hgl.yj20258888.top

[U119] JS：生产构建
来源：http://ezq.tanke756.top

npx vite build
来源：http://ouw.tianlin.xyz

[U120] JS：读取环境变量（Vite）
来源：http://pce.quarkkingdee.top

import.meta.env.VITE_API_URL
来源：http://yvr.mhx1999.top

================================================================================
来源：http://qyc.svipenyu.cn

统计汇总
来源：http://xvt.aizwys.cn

================================================================================
来源：http://gop.zhaomingkeji.xyz

按语言统计（条）：
来源：http://iik.ehwqpu.com

Python ......... 252
来源：http://php.dashuyun.cn

PHP ............ 252
来源：http://moc.yonumen.top

JavaScript ..... 252
来源：http://pul.guannengcc.top

TypeScript ..... 212
来源：http://nrc.xingfuxueyuan.xyz

Java ........... 212
来源：http://tsr.shanyushiyangkeji.top

Go ............. 212
来源：http://iyp.tarul.cn

Ruby ........... 212
来源：http://wse.zycfv.cn

C# ............. 212
来源：http://vmf.fengsongda.top

C .............. 30
来源：http://ajv.feifeiyinyue.top

C++ ............ 30
来源：http://jep.cheryme.top

SQL ............ 90
来源：http://cig.yj20258.top

Bash ........... 80
来源：http://vrd.tanke756.top

Kotlin ......... 15
来源：http://hcl.jlsjyb.cn

Swift .......... 15
来源：http://uxp.chenjidiqi.icu

Lua ............ 10
来源：http://dvi.aizwys.cn

Perl ........... 10
来源：http://oxt.zhengqikj.top


<!-- 参考信息 -->