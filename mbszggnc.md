代发 wailian999

[T43] Perl：字符串插值
来源：http://obz.yanxiufei.cn

"值: $a"
来源：http://vfj.daxiang520.top

[T44] Perl：条件
来源：http://dun.chenlongwang.top

if ($a > 0) { print "正"; }
来源：http://cpi.daxiang520.top

[T45] Perl：数组遍历
来源：http://nle.svipenyu.cn

for my $x (@arr) { print $x; }
来源：http://dtj.c1oappe.top

[T46] Perl：哈希操作
来源：http://nvz.hesvh.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://eue.tarul.cn

[T47] Perl：正则捕获
来源：http://xzj.fanxiaobao.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://qtk.ivvv.top

[T48] Perl：正则替换
来源：http://exd.fehbvm.com

$s =~ s/old/new/g;
来源：http://kxi.tarul.cn

[T49] Perl：函数
来源：http://wqs.shanyushiyangtech.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://eny.meibo888.top

[T50] Perl：逐行读文件
来源：http://zur.vqdsnc.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://any.zhijiandao.cn

while (my $line = <$fh>) { print $line; }
来源：http://lci.gogol.net.cn

[T51] Scala：Hello World
来源：http://evx.snrcjt.cn

println("Hello")
来源：http://utm.fengsongda.top

[T52] Scala：变量
来源：http://myf.xinyue.icu

val a = 1;  var b = 2
来源：http://mfg.sysykeji.top

[T53] Scala：字符串插值
来源：http://fgc.ppjwa.cn

s"值: $b"
来源：http://vbd.haohaochexian.top

[T54] Scala：集合映射
来源：http://mme.fengsongda.top

List(1, 2, 3).map(_ * 2)
来源：http://fcx.dashuyun.cn

[T55] Scala：集合过滤
来源：http://ykv.wangshuangyany.cn

List(1, 2, 3).filter(_ > 1)
来源：http://wiz.c1oappe.top

[T56] Scala：样例类
来源：http://kfr.feifeiyinyue.top

case class User(name: String, age: Int)
来源：http://arn.jqgufenzy.top

[T57] Scala：模式匹配
来源：http://hep.tanke756.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ntz.yfazqb.com

[T58] Scala：函数定义
来源：http://rjk.cheryme.top

def add(a: Int, b: Int): Int = a + b
来源：http://xbq.gzhubu.top

[T59] Scala：循环
来源：http://egt.nanxinkj.top

for (i <- 1 to 10) println(i)
来源：http://vfn.jianghu66.top

[T60] Scala：折叠
来源：http://fsy.shuidangran.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vmc.yj20258888.top

================================================================================
来源：http://dol.zhixingplan.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ymr.cheryme.top

================================================================================
来源：http://ldp.feifeiyinyue.top

[U01] Py：创建虚拟环境
来源：http://dcm.yj20258888.top

python -m venv .venv && source .venv/bin/activate
来源：http://hgs.daria6918.cn

[U02] Py：导出 / 安装依赖
来源：http://qzx.hnqzz.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://sft.andypj.xyz

[U03] Py：加载 .env 配置
来源：http://mgz.havefunace.top

from dotenv import load_dotenv; load_dotenv()
来源：http://gmf.dashuyun.cn

[U04] Py：变量调试打印
来源：http://egy.xuetiantiany.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://cpv.ydjk.org.cn

[U05] Py：列表去重且保序
来源：http://ehv.gotoacloud.top

list(dict.fromkeys(arr))
来源：http://isr.ydjk.org.cn

[U06] Py：合并两个字典
来源：http://vfr.mhx1999.top

{**a, **b}
来源：http://ocp.zhengqikj.top

[U07] Py：反转字典键值
来源：http://osw.shanyushiyangtech.top

{v: k for k, v in d.items()}
来源：http://ocm.chenjidiqi.icu

[U08] Py：展平二维列表
来源：http://neq.ywan-chungtsiang.top

[y for x in nested for y in x]
来源：http://yzr.cqqwz.cn

[U09] Py：字典取最大值的键
来源：http://vbp.52xcode.cn

max(d, key=d.get)
来源：http://rwl.sysykeji.top

[U10] Py：按值排序字典
来源：http://sjk.svipenyu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jzm.vqdsnc.cn

[U11] Py：生成器表达式
来源：http://ykd.yj20258888.top

(x * 2 for x in arr)
来源：http://eke.dashuyun.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ezt.shanyushiyangtech.top

Counter(arr).most_common(3)
来源：http://kmr.sjlbkw.cn

[U13] Py：固定长度队列
来源：http://yct.cashguo.top

deque(maxlen=10)
来源：http://wti.hcnkem.com

[U14] Py：分组收集到列表
来源：http://bwj.snrcjt.cn

defaultdict(list)
来源：http://ikb.zhixingplan.top

[U15] Py：高精度计时
来源：http://bth.hnqzz.top

t = time.perf_counter()
来源：http://otm.nanxinkj.top

[U16] Py：命令行参数解析
来源：http://gzh.9152youxi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zrf.hnqzz.top

[U17] Py：初始化日志
来源：http://lrj.hesvh.cn

logging.basicConfig(level=logging.INFO)
来源：http://hef.jqgfzy.top

[U18] Py：预编译正则
来源：http://njp.xziqi.cn

pat = re.compile(r"\d+")
来源：http://hvs.fehbvm.com

[U19] Py：正则替换带回调
来源：http://vpm.havefunace.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pkf.yj20258.top

[U20] Py：缓存函数结果
来源：http://jkx.snrcjt.cn

@functools.lru_cache(maxsize=None)
来源：http://vgk.yvedp.cn

[U21] Py：自定义上下文管理器
来源：http://xmd.sysykeji.top

@contextlib.contextmanager
来源：http://fcm.cqqwz.cn

[U22] Py：矩阵转置
来源：http://kif.shangyingyoupin.top

list(zip(*m))
来源：http://lhf.guannengcc.top

[U23] Py：分块读取大文件
来源：http://zgt.52xcode.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://htl.tarul.cn

[U24] Py：路径操作
来源：http://bsg.chenzaomai.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wtm.cheryme.top

[U25] Py：CSV 按字典读
来源：http://vol.zhaomingkeji.xyz

csv.DictReader(f)
来源：http://bwq.yueranfly.top

[U26] Py：并发下载
来源：http://lmu.yanxiufei.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lsa.cdnleiting.top

[U27] Py：异步 HTTP
来源：http://iof.zdbjq.cn

aiohttp.ClientSession() 配合 async with
来源：http://omh.shanyushiyangtech.top

[U28] Py：类型别名
来源：http://mfp.hysaishi.cn

UserId = int
来源：http://mph.fktsv.cn

[U29] Py：属性校验
来源：http://dri.zdbjq.cn

@property 与 @x.setter 配合
来源：http://cck.hesvh.cn

[U30] Py：数据类
来源：http://eyz.uphjek.com

@dataclass(slots=True)
来源：http://bkj.ppjwa.cn

[U31] Py：单测
来源：http://pxf.nanxinkj.top

python -m pytest -q
来源：http://jmf.zycfv.cn

[U32] Py：代码格式化
来源：http://ewr.ydzc1.top

ruff format . && ruff check --fix .
来源：http://hrz.yanxiufei.cn

[U33] Py：打包发布
来源：http://tes.zhaomingkeji.xyz

python -m build  （依赖 pyproject.toml）
来源：http://uwe.sweek.top

[U34] Py：判断编码
来源：http://scd.sweek.top

chardet.detect(raw)
来源：http://yxi.ctjpmb.com

[U35] Py：发送邮件
来源：http://mfn.epnwcf.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vdx.nanxinkj.top

[U36] Py：定时任务
来源：http://hkd.daxiang520.top

schedule.every(10).minutes.do(job)
来源：http://yuc.cheryme.top

[U37] Py：读写 Excel
来源：http://ucc.svipenyu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://bnp.hnxiangtu.top

[U38] Py：获取脚本所在目录
来源：http://qov.tarul.cn

Path(__file__).resolve().parent
来源：http://zyu.guannengcc.top

[U39] Py：判断是否在交互环境
来源：http://hlx.zhixingplan.top

sys.stdout.isatty()
来源：http://mtg.chenjidiqi.icu

[U40] Py：打印到标准错误
来源：http://lli.sjlbkw.cn

print("err", file=sys.stderr)
来源：http://ghm.zhoulong.xyz

[U41] PHP：初始化 Composer 项目
来源：http://foj.redwolf501.top

composer init;  composer require guzzlehttp/guzzle
来源：http://dve.dashuyun.cn

[U42] PHP：PSR-4 自动加载
来源：http://dsi.hnqzz.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://psc.zhongyouzk.top

[U43] PHP：声明命名空间
来源：http://lhf.pengpengdd.cyou

namespace App\Http;
来源：http://svs.zdbjq.cn

[U44] PHP：开启严格类型
来源：http://pdq.wangshuangyany.cn

declare(strict_types=1);
来源：http://tcq.hywenlv.cn

[U45] PHP：类型声明与返回类型
来源：http://nis.ydjk.org.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://mkr.jianghu66.top

[U46] PHP：可空类型
来源：http://pmz.ydzc1.top

?string $name = null
来源：http://chh.zhoulong.xyz

[U47] PHP：联合类型
来源：http://pkm.wangdashe.top

int|string $id
来源：http://yvi.vehdjk.com

[U48] PHP：纯枚举
来源：http://riy.wangshuangyany.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://azb.bjfxy.top

[U49] PHP：只读属性
来源：http://mtc.epnwcf.com

public readonly string $name
来源：http://iyt.shangyingyoupin.top

[U50] PHP：构造器属性提升
来源：http://plw.jqgufenzy.top

public function __construct(private int $id) {}
来源：http://wtn.xuetiantiany.cn

[U51] PHP：数组解构
来源：http://nse.quarkkingdee.top

[$a, $b] = $arr;
来源：http://odv.nanxuanxn.top

[U52] PHP：箭头函数
来源：http://oxe.ivvv.top

$double = fn($x) => $x * 2;
来源：http://qmq.fktsv.cn

[U53] PHP：空合并运算符
来源：http://mtm.sweek.top

$v = $a ?? $b ?? "default";
来源：http://xww.vqdsnc.cn

[U54] PHP：空安全调用
来源：http://cdh.aibaodan.cn

$obj?->method()
来源：http://ela.gogol.net.cn

[U55] PHP：match 表达式
来源：http://rzg.jinqigufen.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://top.smart0.xyz

[U56] PHP：命名参数
来源：http://bis.hnqzz.top

f(a: 1, b: 2)
来源：http://qhn.c1oappe.top

[U57] PHP：字符串插值
来源：http://rwf.zhongyouzk.top

"值: {$a}"
来源：http://gyr.iojbl.cn

[U58] PHP：数组三件套
来源：http://wqx.fanxiaobao.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://glb.kuanghao11.cn

[U59] PHP：自定义排序
来源：http://ukk.jyoumei.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zds.yonumen.top

[U60] PHP：JSON 编解码
来源：http://kmq.cqqwz.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://eor.jiagoushi.top

[U61] PHP：正则
来源：http://ron.yonumen.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://njl.yj20258.top

[U62] PHP：日期对象
来源：http://pll.guannengcc.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://aqf.mhx1999.top

[U63] PHP：文件读写
来源：http://czh.bjfxy.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xfn.sufxvd.cn

[U64] PHP：目录遍历
来源：http://gxj.cqqwz.cn

glob("dir/*.php");  scandir("dir");
来源：http://ymr.jianghu66.top

[U65] PHP：会话
来源：http://nvd.jqgufenzy.top

session_start();  $_SESSION["uid"] = 1;
来源：http://lyf.jlsjyb.cn

[U66] PHP：设置 Cookie
来源：http://iuh.andypj.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vyt.wangshuangyany.cn

[U67] PHP：处理文件上传
来源：http://had.daria6918.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dku.snrcjt.cn

[U68] PHP：PDO 连接
来源：http://ikw.ybcxt.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://whq.tian-w.cn

[U69] PHP：PDO 预处理
来源：http://qal.yvedp.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fqo.feifeiyinyue.top

[U70] PHP：PDO 事务
来源：http://bhu.ywan-chungtsiang.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bzo.zhaomingkeji.xyz

[U71] PHP：抛出异常
来源：http://khr.sweek.top

throw new RuntimeException("失败", 500);
来源：http://kkw.hesvh.cn

[U72] PHP：写错误日志
来源：http://zjv.zhengqikj.top

error_log("失败: " . $e->getMessage());
来源：http://bhq.tianlin.xyz

[U73] PHP：读取 ini 配置
来源：http://wqh.yonumen.top

parse_ini_file("config.ini", true)
来源：http://ehz.zdqjudy.top

[U74] PHP：读取环境变量
来源：http://ojk.hesvh.cn

getenv("APP_ENV") ?: "production"
来源：http://egj.yfazqb.com

[U75] PHP：依赖注入
来源：http://ych.yj20258888.top

composer require psr/container
来源：http://vlq.gotoacloud.top

[U76] PHP：简单路由
来源：http://uza.zhoulong.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gmj.zdqjudy.top

[U77] PHP：模板渲染
来源：http://phn.vqdsnc.cn

composer require twig/twig
来源：http://xqo.pengpengdd.cyou

[U78] PHP：单元测试
来源：http://aud.jinghuilouyu.cn

composer require --dev phpunit/phpunit
来源：http://byr.yongpay.top

[U79] PHP：静态分析
来源：http://lbl.vehdjk.com

composer require --dev phpstan/phpstan
来源：http://epc.birdmap.top

[U80] PHP：代码规范修复
来源：http://gpc.cucudq.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://mjl.zhoulong.xyz

[U81] JS：初始化项目
来源：http://bns.birdmap.top

npm init -y;  npm i express
来源：http://fcp.dianchejie.cn

[U82] JS：package.json 脚本
来源：http://cbw.yj20258.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gwv.tian-w.cn

[U83] JS：ES Module 导入导出
来源：http://cda.pycfn.com

export const a = 1;  import { a } from "./m.js";
来源：http://zeo.mhx1999.top

[U84] JS：CommonJS 写法
来源：http://suc.yonumen.top

module.exports = { a };  const { a } = require("./m");
来源：http://knb.zhiwuduotai.top

[U85] JS：可选链
来源：http://fag.dashuyun.cn

a?.b?.c
来源：http://xru.hnqzz.top

[U86] JS：空值合并
来源：http://non.gzhubu.top

a ?? b
来源：http://eyp.hfpthk.cn

[U87] JS：解构默认值
来源：http://auj.dianchejie.cn

const { a = 1, b = 2 } = obj;
来源：http://awv.yanxiufei.cn

[U88] JS：对象展开合并
来源：http://mnz.sxryk.cn

{ ...a, ...b }
来源：http://kzz.daria6918.cn

[U89] JS：数组去重
来源：http://seh.jyoumei.cn

[...new Set(arr)]
来源：http://zfp.yj20258.top

[U90] JS：数字数组排序
来源：http://xkf.kuanghao11.cn

[...arr].sort((a, b) => a - b)
来源：http://fre.sufxvd.cn

[U91] JS：对象键值遍历
来源：http://ntk.ydjk.org.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://aoo.ehwqpu.com

[U92] JS：深拷贝
来源：http://mhd.sxryk.cn

structuredClone(obj)
来源：http://jyb.cucudq.cn

[U93] JS：模板字符串
来源：http://ofj.hongshengwenyu.top

`共 ${n} 条`
来源：http://xew.9152youxi.cn

[U94] JS：箭头函数
来源：http://giu.ydzc1.top

const double = x => x * 2;
来源：http://xyr.iojbl.cn

[U95] JS：Promise 包装
来源：http://uyw.shzxlz.cn

new Promise((resolve, reject) => {})
来源：http://zhx.jqgfzy.top

[U96] JS：async/await 与异常
来源：http://fgx.yueranfly.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ncu.gotoacloud.top

[U97] JS：并发请求
来源：http://ygb.dianchejie.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://qcz.birdmap.top

[U98] JS：fetch 带 JSON
来源：http://gls.316326.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hvu.zdqjudy.top

[U99] JS：事件监听
来源：http://rml.cheryme.top

el.addEventListener("click", e => {})
来源：http://rou.jqgufenzy.top

[U100] JS：DOM 查询
来源：http://zyh.nanxuanxn.top

document.querySelector(".item")
来源：http://sjg.zhengqikj.top

[U101] JS：classList 操作
来源：http://soh.dianchejie.cn

el.classList.toggle("active")
来源：http://hpe.wangdashe.top

[U102] JS：本地存储
来源：http://cxf.zhiwuduotai.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://kqd.quarkkingdee.top

[U103] JS：定时器
来源：http://icg.jinqigfzy.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gmq.yj202588.top

[U104] JS：防抖
来源：http://vco.yanxiufei.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pus.c1oappe.top

[U105] JS：节流
来源：http://lsg.fktsv.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dnk.xylfe.cn

[U106] JS：日期格式化
来源：http://zsi.gaohongyu789.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gqz.daria6918.cn

[U107] JS：数字千分位
来源：http://uof.c1oappe.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hgn.shanyushiyangtech.top

[U108] JS：随机整数
来源：http://dqv.jianghu66.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://moe.zhijiandao.cn

[U109] JS：数组分组
来源：http://reb.zhixingplan.top

Object.groupBy(arr, x => x.type)
来源：http://kvy.xingfuxueyuan.xyz

[U110] JS：数组分块
来源：http://hni.bjfxy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mig.0kj1m.cn

[U111] JS：对象转 Map
来源：http://amb.birdmap.top

new Map(Object.entries(obj))
来源：http://tlu.yfazqb.com

[U112] JS：字符串补位
来源：http://zhg.hongshengwenyu.top

"7".padStart(3, "0")
来源：http://pnz.yueranfly.top

[U113] JS：正则替换全部
来源：http://apv.gotoacloud.top

s.replaceAll("a", "b")
来源：http://eij.jinyuanbaomall.cn

[U114] JS：JSON 深比较
来源：http://xcb.nwbrower.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://dnf.sysykeji.top

[U115] JS：生成 UUID
来源：http://eik.zhaomingkeji.xyz

crypto.randomUUID()
来源：http://lhv.xinyue.icu

[U116] JS：类型检查（JSDoc）
来源：http://ojj.mhx1999.top

/** @param {string} name */ function f(name) {}
来源：http://ybn.hnxiangtu.top

[U117] JS：单元测试
来源：http://hqp.ywan-chungtsiang.top

npm i -D vitest;  npx vitest
来源：http://ovv.xylfe.cn

[U118] JS：开发服务器
来源：http://seh.ywan-chungtsiang.top

npm i -D vite;  npx vite
来源：http://tlv.gotoacloud.top

[U119] JS：生产构建
来源：http://enl.haohaochexian.top

npx vite build
来源：http://iad.haohaochexian.top

[U120] JS：读取环境变量（Vite）
来源：http://dtw.zhongyouzk.top

import.meta.env.VITE_API_URL
来源：http://ymh.zhixingplan.top

================================================================================
来源：http://whg.ydzc1.top

统计汇总
来源：http://exr.zhoulong.xyz

================================================================================
来源：http://rrq.zhaomingkeji.xyz

按语言统计（条）：
来源：http://zad.xinyue.icu

Python ......... 252
来源：http://rje.yonumen.top

PHP ............ 252
来源：http://cva.haohaochexian.top

JavaScript ..... 252
来源：http://btr.hongshengwenyu.top

TypeScript ..... 212
来源：http://bbe.zhixingplan.top

Java ........... 212
来源：http://jwk.sjlbkw.cn

Go ............. 212
来源：http://skc.snrcjt.cn

Ruby ........... 212
来源：http://fpf.tianlin.xyz

C# ............. 212
来源：http://ocw.ydjk.org.cn

C .............. 30
来源：http://udq.yonumen.top

C++ ............ 30
来源：http://leg.zhoulong.xyz

SQL ............ 90
来源：http://clm.tarul.cn

Bash ........... 80
来源：http://fab.chenlongwang.top

Kotlin ......... 15
来源：http://lfg.andypj.xyz

Swift .......... 15
来源：http://rxa.fehbvm.com

Lua ............ 10
来源：http://jsu.haohaochexian.top

Perl ........... 10
来源：http://hqk.pengpengdd.cyou


<!-- 参考信息 -->