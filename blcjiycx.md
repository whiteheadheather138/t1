代发 wailian999

[T43] Perl：字符串插值
来源：http://heh.svipenyu.cn

"值: $a"
来源：http://zpk.zdqjudy.top

[T44] Perl：条件
来源：http://ubk.fktsv.cn

if ($a > 0) { print "正"; }
来源：http://egz.fzhhl.top

[T45] Perl：数组遍历
来源：http://coc.nanxuanxn.top

for my $x (@arr) { print $x; }
来源：http://yla.tianlin.xyz

[T46] Perl：哈希操作
来源：http://nwp.zhoulong.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://etj.cheryme.top

[T47] Perl：正则捕获
来源：http://cna.quarkkingdee.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://rxi.tianlin.xyz

[T48] Perl：正则替换
来源：http://uxb.epnwcf.com

$s =~ s/old/new/g;
来源：http://kti.yuxming.cn

[T49] Perl：函数
来源：http://gng.guannengcc.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://omx.yuxming.cn

[T50] Perl：逐行读文件
来源：http://mpf.wangdashe.top

open my $fh, "<", "a.txt" or die $!;
来源：http://img.dashuyun.cn

while (my $line = <$fh>) { print $line; }
来源：http://zgq.cashguo.top

[T51] Scala：Hello World
来源：http://mzo.nanxuanxn.top

println("Hello")
来源：http://dgt.chenlongwang.top

[T52] Scala：变量
来源：http://aob.fktsv.cn

val a = 1;  var b = 2
来源：http://svp.tian-w.cn

[T53] Scala：字符串插值
来源：http://ulc.316326.xyz

s"值: $b"
来源：http://lsg.hysaishi.cn

[T54] Scala：集合映射
来源：http://hrh.ydzc1.top

List(1, 2, 3).map(_ * 2)
来源：http://qeg.hfpthk.cn

[T55] Scala：集合过滤
来源：http://eti.yonumen.top

List(1, 2, 3).filter(_ > 1)
来源：http://rvn.redwolf501.top

[T56] Scala：样例类
来源：http://hvy.zhijiandao.cn

case class User(name: String, age: Int)
来源：http://qom.jinghuilouyu.cn

[T57] Scala：模式匹配
来源：http://gwz.xinyue.icu

x match { case 1 => "一"; case _ => "其他" }
来源：http://nnx.chenjidiqi.icu

[T58] Scala：函数定义
来源：http://fjz.0kj1m.cn

def add(a: Int, b: Int): Int = a + b
来源：http://glf.shuidangran.top

[T59] Scala：循环
来源：http://vfm.chenjidiqi.icu

for (i <- 1 to 10) println(i)
来源：http://xip.yanxiufei.cn

[T60] Scala：折叠
来源：http://cna.zhijiandao.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vvj.zhijiandao.cn

================================================================================
来源：http://jsk.fzhhl.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xza.yj20258888.top

================================================================================
来源：http://czu.xziqi.cn

[U01] Py：创建虚拟环境
来源：http://qhy.pycfn.com

python -m venv .venv && source .venv/bin/activate
来源：http://xwh.smart0.xyz

[U02] Py：导出 / 安装依赖
来源：http://iwy.haohaochexian.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mrh.ppjwa.cn

[U03] Py：加载 .env 配置
来源：http://fuv.shangyingyoupin.top

from dotenv import load_dotenv; load_dotenv()
来源：http://fpe.52xcode.cn

[U04] Py：变量调试打印
来源：http://was.hywenlv.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qvm.cheryme.top

[U05] Py：列表去重且保序
来源：http://vae.pycfn.com

list(dict.fromkeys(arr))
来源：http://ssl.haohaochexian.top

[U06] Py：合并两个字典
来源：http://boj.shanyushiyangkeji.top

{**a, **b}
来源：http://nrn.mhx1999.top

[U07] Py：反转字典键值
来源：http://tqw.fanxiaobao.xyz

{v: k for k, v in d.items()}
来源：http://cip.tanke756.top

[U08] Py：展平二维列表
来源：http://tpo.gotoacloud.top

[y for x in nested for y in x]
来源：http://apv.0kj1m.cn

[U09] Py：字典取最大值的键
来源：http://qri.fanxiaobao.xyz

max(d, key=d.get)
来源：http://exs.zhongyouzk.top

[U10] Py：按值排序字典
来源：http://toh.shanyushiyangtech.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uav.0kj1m.cn

[U11] Py：生成器表达式
来源：http://qpe.jinqigufen.top

(x * 2 for x in arr)
来源：http://ngm.hysaishi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://mic.c1oappe.top

Counter(arr).most_common(3)
来源：http://vok.c1oappe.top

[U13] Py：固定长度队列
来源：http://dej.zdbjq.cn

deque(maxlen=10)
来源：http://cqs.feifeiyinyue.top

[U14] Py：分组收集到列表
来源：http://yoa.snrcjt.cn

defaultdict(list)
来源：http://ajz.yuanzhike.top

[U15] Py：高精度计时
来源：http://fxd.havefunace.top

t = time.perf_counter()
来源：http://fvy.yangfankeji.com

[U16] Py：命令行参数解析
来源：http://wcq.cdnleiting.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ojz.ctjpmb.com

[U17] Py：初始化日志
来源：http://mye.yuxming.cn

logging.basicConfig(level=logging.INFO)
来源：http://qjb.tanke756.top

[U18] Py：预编译正则
来源：http://ukt.gogol.net.cn

pat = re.compile(r"\d+")
来源：http://uuu.jianghu66.top

[U19] Py：正则替换带回调
来源：http://exb.sweek.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yvg.ybcxt.top

[U20] Py：缓存函数结果
来源：http://pnl.fktsv.cn

@functools.lru_cache(maxsize=None)
来源：http://kly.yj202588.top

[U21] Py：自定义上下文管理器
来源：http://ojj.yj20258888.top

@contextlib.contextmanager
来源：http://vza.mhx1999.top

[U22] Py：矩阵转置
来源：http://ltf.shanyushiyangtech.top

list(zip(*m))
来源：http://ubj.zhongyouzk.top

[U23] Py：分块读取大文件
来源：http://kop.guowangkeji.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jea.zhoulong.xyz

[U24] Py：路径操作
来源：http://xys.yongpay.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wtv.yangfankeji.com

[U25] Py：CSV 按字典读
来源：http://zlo.snrcjt.cn

csv.DictReader(f)
来源：http://lai.sjlbkw.cn

[U26] Py：并发下载
来源：http://llb.yuanzhike.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mff.zdbjq.cn

[U27] Py：异步 HTTP
来源：http://npx.xuanzx.com

aiohttp.ClientSession() 配合 async with
来源：http://gdh.yuanzhike.top

[U28] Py：类型别名
来源：http://hpa.yanxiufei.cn

UserId = int
来源：http://idj.gotoacloud.top

[U29] Py：属性校验
来源：http://bch.vehdjk.com

@property 与 @x.setter 配合
来源：http://kdt.9152youxi.cn

[U30] Py：数据类
来源：http://pxs.cdnleiting.top

@dataclass(slots=True)
来源：http://hkl.jianghu66.top

[U31] Py：单测
来源：http://utb.bjfxy.top

python -m pytest -q
来源：http://ztt.wangdashe.top

[U32] Py：代码格式化
来源：http://xgn.uphjek.com

ruff format . && ruff check --fix .
来源：http://yul.ydzc1.top

[U33] Py：打包发布
来源：http://eje.dashuyun.cn

python -m build  （依赖 pyproject.toml）
来源：http://rml.vqdsnc.cn

[U34] Py：判断编码
来源：http://vfn.yfazqb.com

chardet.detect(raw)
来源：http://fhg.ctjpmb.com

[U35] Py：发送邮件
来源：http://qwh.sweek.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://oka.tanke756.top

[U36] Py：定时任务
来源：http://acv.hongshengwenyu.top

schedule.every(10).minutes.do(job)
来源：http://fhp.jinqigfzy.top

[U37] Py：读写 Excel
来源：http://ymo.c1oappe.top

pandas.read_excel / DataFrame.to_excel
来源：http://fsl.yj20258888.top

[U38] Py：获取脚本所在目录
来源：http://bia.316326.xyz

Path(__file__).resolve().parent
来源：http://hrv.smart0.xyz

[U39] Py：判断是否在交互环境
来源：http://imc.redwolf501.top

sys.stdout.isatty()
来源：http://yjt.tian-w.cn

[U40] Py：打印到标准错误
来源：http://clf.hfpthk.cn

print("err", file=sys.stderr)
来源：http://buv.sysykeji.top

[U41] PHP：初始化 Composer 项目
来源：http://mkh.yj20258.top

composer init;  composer require guzzlehttp/guzzle
来源：http://xkx.gogol.net.cn

[U42] PHP：PSR-4 自动加载
来源：http://uvg.smart0.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://kck.hnxiangtu.top

[U43] PHP：声明命名空间
来源：http://yty.shanyushiyangtech.top

namespace App\Http;
来源：http://dzr.nanxinkj.top

[U44] PHP：开启严格类型
来源：http://kky.zhaomingkeji.xyz

declare(strict_types=1);
来源：http://qga.aizwys.cn

[U45] PHP：类型声明与返回类型
来源：http://wxn.yj202588.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://lrz.svipenyu.cn

[U46] PHP：可空类型
来源：http://eus.feifeiyinyue.top

?string $name = null
来源：http://ajs.gogol.net.cn

[U47] PHP：联合类型
来源：http://pkk.shuidangran.top

int|string $id
来源：http://wql.yangfankeji.com

[U48] PHP：纯枚举
来源：http://nhw.ydjk.org.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rqn.yanxiufei.cn

[U49] PHP：只读属性
来源：http://esd.haohaochexian.top

public readonly string $name
来源：http://zfu.316326.xyz

[U50] PHP：构造器属性提升
来源：http://tmf.9152youxi.cn

public function __construct(private int $id) {}
来源：http://yrw.xziqi.cn

[U51] PHP：数组解构
来源：http://cjl.jianghu66.top

[$a, $b] = $arr;
来源：http://vbl.yanxiufei.cn

[U52] PHP：箭头函数
来源：http://nep.bbcook.cn

$double = fn($x) => $x * 2;
来源：http://kyu.yonumen.top

[U53] PHP：空合并运算符
来源：http://kvx.andypj.xyz

$v = $a ?? $b ?? "default";
来源：http://rxk.xylfe.cn

[U54] PHP：空安全调用
来源：http://dgb.aibaodan.cn

$obj?->method()
来源：http://noo.zhongyouzk.top

[U55] PHP：match 表达式
来源：http://fcv.dianchejie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mpn.pycfn.com

[U56] PHP：命名参数
来源：http://npq.quarkkingdee.top

f(a: 1, b: 2)
来源：http://ibu.jinqigufen.top

[U57] PHP：字符串插值
来源：http://zst.yuanzhike.top

"值: {$a}"
来源：http://nwp.gogol.net.cn

[U58] PHP：数组三件套
来源：http://gqx.hcnkem.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ouo.haohaochexian.top

[U59] PHP：自定义排序
来源：http://lyr.uphjek.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://udo.0kj1m.cn

[U60] PHP：JSON 编解码
来源：http://oup.smart0.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://eml.zhengqikj.top

[U61] PHP：正则
来源：http://ttv.gaohongyu789.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://crp.fehbvm.com

[U62] PHP：日期对象
来源：http://dhn.fktsv.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ffo.kuanghao11.cn

[U63] PHP：文件读写
来源：http://upd.tanke756.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ixn.tarul.cn

[U64] PHP：目录遍历
来源：http://aqp.bbcook.cn

glob("dir/*.php");  scandir("dir");
来源：http://ctl.zdqjudy.top

[U65] PHP：会话
来源：http://hxw.tian-w.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://uka.zdqjudy.top

[U66] PHP：设置 Cookie
来源：http://fox.iojbl.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://lhw.bbcook.cn

[U67] PHP：处理文件上传
来源：http://ccq.kuanghao11.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://oyt.birdmap.top

[U68] PHP：PDO 连接
来源：http://fxk.jiagoushi.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vse.tarul.cn

[U69] PHP：PDO 预处理
来源：http://tbc.zhiwuduotai.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nwa.cheryme.top

[U70] PHP：PDO 事务
来源：http://pwl.ydzc1.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rjc.meibo888.top

[U71] PHP：抛出异常
来源：http://bdv.daxiang520.top

throw new RuntimeException("失败", 500);
来源：http://wvi.gotoacloud.top

[U72] PHP：写错误日志
来源：http://ptd.shzxlz.cn

error_log("失败: " . $e->getMessage());
来源：http://hwc.mhx1999.top

[U73] PHP：读取 ini 配置
来源：http://vyt.yfazqb.com

parse_ini_file("config.ini", true)
来源：http://pvj.zhaomingkeji.xyz

[U74] PHP：读取环境变量
来源：http://yjv.svipenyu.cn

getenv("APP_ENV") ?: "production"
来源：http://sfe.sysykeji.top

[U75] PHP：依赖注入
来源：http://sex.quarkkingdee.top

composer require psr/container
来源：http://gsv.yuanzhike.top

[U76] PHP：简单路由
来源：http://opn.tarul.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tgf.ybcxt.top

[U77] PHP：模板渲染
来源：http://omf.316326.xyz

composer require twig/twig
来源：http://rxv.nwbrower.top

[U78] PHP：单元测试
来源：http://dyl.c1oappe.top

composer require --dev phpunit/phpunit
来源：http://rpr.guannengcc.top

[U79] PHP：静态分析
来源：http://jus.sufxvd.cn

composer require --dev phpstan/phpstan
来源：http://iqt.jinqigfzy.top

[U80] PHP：代码规范修复
来源：http://ygu.hesvh.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://hsa.havefunace.top

[U81] JS：初始化项目
来源：http://mis.hywenlv.cn

npm init -y;  npm i express
来源：http://tsz.ybcxt.top

[U82] JS：package.json 脚本
来源：http://sux.pycfn.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fzj.ctjpmb.com

[U83] JS：ES Module 导入导出
来源：http://ito.shanyushiyangkeji.top

export const a = 1;  import { a } from "./m.js";
来源：http://vhg.zhijiandao.cn

[U84] JS：CommonJS 写法
来源：http://tdj.zhaomingkeji.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://lwn.xuanzx.com

[U85] JS：可选链
来源：http://avn.jinghuilouyu.cn

a?.b?.c
来源：http://mup.zhoulong.xyz

[U86] JS：空值合并
来源：http://zrr.iojbl.cn

a ?? b
来源：http://idg.zhijiandao.cn

[U87] JS：解构默认值
来源：http://zuu.hesvh.cn

const { a = 1, b = 2 } = obj;
来源：http://hzn.ivvv.top

[U88] JS：对象展开合并
来源：http://xlo.cucudq.cn

{ ...a, ...b }
来源：http://zmi.yfazqb.com

[U89] JS：数组去重
来源：http://nom.yanxiufei.cn

[...new Set(arr)]
来源：http://lgt.svipenyu.cn

[U90] JS：数字数组排序
来源：http://ycd.chenlongwang.top

[...arr].sort((a, b) => a - b)
来源：http://hwd.uphjek.com

[U91] JS：对象键值遍历
来源：http://beu.zdbjq.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zyr.ywan-chungtsiang.top

[U92] JS：深拷贝
来源：http://mib.zdqjudy.top

structuredClone(obj)
来源：http://zfx.aizwys.cn

[U93] JS：模板字符串
来源：http://ebi.vqdsnc.cn

`共 ${n} 条`
来源：http://xrd.nanxinkj.top

[U94] JS：箭头函数
来源：http://vgn.gaohongyu789.top

const double = x => x * 2;
来源：http://maz.c1oappe.top

[U95] JS：Promise 包装
来源：http://gan.yj20258.top

new Promise((resolve, reject) => {})
来源：http://qgn.yj20258.top

[U96] JS：async/await 与异常
来源：http://mey.hongshengwenyu.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gck.xylfe.cn

[U97] JS：并发请求
来源：http://aok.hywenlv.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ytw.aibaodan.cn

[U98] JS：fetch 带 JSON
来源：http://beu.shzxlz.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://sru.feifeiyinyue.top

[U99] JS：事件监听
来源：http://sxn.gotoacloud.top

el.addEventListener("click", e => {})
来源：http://lpa.zhoulong.xyz

[U100] JS：DOM 查询
来源：http://jbw.andypj.xyz

document.querySelector(".item")
来源：http://ljj.nanxinkj.top

[U101] JS：classList 操作
来源：http://wzs.cucudq.cn

el.classList.toggle("active")
来源：http://byl.ppjwa.cn

[U102] JS：本地存储
来源：http://luh.yanxiufei.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://wie.jqgfzy.top

[U103] JS：定时器
来源：http://fin.tanke756.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kxq.yueranfly.top

[U104] JS：防抖
来源：http://xpz.snrcjt.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://skr.hysaishi.cn

[U105] JS：节流
来源：http://ajh.zhoulong.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vsl.xuetiantiany.cn

[U106] JS：日期格式化
来源：http://tsr.shanyushiyangtech.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xyd.pycfn.com

[U107] JS：数字千分位
来源：http://ouw.andypj.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hea.yuxming.cn

[U108] JS：随机整数
来源：http://boj.andypj.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://lzk.quarkkingdee.top

[U109] JS：数组分组
来源：http://fbg.cheryme.top

Object.groupBy(arr, x => x.type)
来源：http://ahr.havefunace.top

[U110] JS：数组分块
来源：http://gan.ydjk.org.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://chd.cdnleiting.top

[U111] JS：对象转 Map
来源：http://ptk.cdnleiting.top

new Map(Object.entries(obj))
来源：http://vsc.svipenyu.cn

[U112] JS：字符串补位
来源：http://ekp.jinqigfzy.top

"7".padStart(3, "0")
来源：http://pge.svipenyu.cn

[U113] JS：正则替换全部
来源：http://lqx.52xcode.cn

s.replaceAll("a", "b")
来源：http://jrb.zhoulong.xyz

[U114] JS：JSON 深比较
来源：http://sph.shuidangran.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ugd.jlsjyb.cn

[U115] JS：生成 UUID
来源：http://rvy.sjlbkw.cn

crypto.randomUUID()
来源：http://saf.guannengcc.top

[U116] JS：类型检查（JSDoc）
来源：http://bqk.xziqi.cn

/** @param {string} name */ function f(name) {}
来源：http://gdj.hnxiangtu.top

[U117] JS：单元测试
来源：http://net.gaohongyu789.top

npm i -D vitest;  npx vitest
来源：http://giq.epnwcf.com

[U118] JS：开发服务器
来源：http://ezn.yuanzhike.top

npm i -D vite;  npx vite
来源：http://nzy.gogol.net.cn

[U119] JS：生产构建
来源：http://hop.52xcode.cn

npx vite build
来源：http://yct.yj20258888.top

[U120] JS：读取环境变量（Vite）
来源：http://awc.havefunace.top

import.meta.env.VITE_API_URL
来源：http://udk.fzhhl.top

================================================================================
来源：http://oqi.daria6918.cn

统计汇总
来源：http://ggs.jiagoushi.top

================================================================================
来源：http://ffg.tanke756.top

按语言统计（条）：
来源：http://vig.ppjwa.cn

Python ......... 252
来源：http://own.ywan-chungtsiang.top

PHP ............ 252
来源：http://idb.hnqzz.top

JavaScript ..... 252
来源：http://okm.zhoulong.xyz

TypeScript ..... 212
来源：http://nky.xuanzx.com

Java ........... 212
来源：http://lfd.ydzc1.top

Go ............. 212
来源：http://gjc.cashguo.top

Ruby ........... 212
来源：http://pur.yuxming.cn

C# ............. 212
来源：http://svp.tarul.cn

C .............. 30
来源：http://rpc.feifeiyinyue.top

C++ ............ 30
来源：http://opg.ydzc1.top

SQL ............ 90
来源：http://cjx.fktsv.cn

Bash ........... 80
来源：http://ika.shuidangran.top

Kotlin ......... 15
来源：http://tvc.shanyushiyangtech.top

Swift .......... 15
来源：http://exe.yuanzhike.top

Lua ............ 10
来源：http://cza.yonumen.top

Perl ........... 10
来源：http://aei.nwbrower.top


<!-- 参考信息 -->