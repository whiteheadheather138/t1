代发 wailian999

[T47] Perl：正则捕获
来源：http://ulk.xuanzx.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://rqf.tianlin.xyz

[T48] Perl：正则替换
来源：http://ppg.tian-w.cn

$s =~ s/old/new/g;
来源：http://sku.mhx1999.top

[T49] Perl：函数
来源：http://tli.haohaochexian.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://amx.jinyuanbaomall.cn

[T50] Perl：逐行读文件
来源：http://pvg.guannengcc.top

open my $fh, "<", "a.txt" or die $!;
来源：http://bxk.ctjpmb.com

while (my $line = <$fh>) { print $line; }
来源：http://hlh.sufxvd.cn

[T51] Scala：Hello World
来源：http://oqf.jyoumei.cn

println("Hello")
来源：http://nme.guowangkeji.top

[T52] Scala：变量
来源：http://aee.tarul.cn

val a = 1;  var b = 2
来源：http://fij.dianchejie.cn

[T53] Scala：字符串插值
来源：http://pgm.sjlbkw.cn

s"值: $b"
来源：http://ehd.svipenyu.cn

[T54] Scala：集合映射
来源：http://hbd.zhengqikj.top

List(1, 2, 3).map(_ * 2)
来源：http://evz.zhongyouzk.top

[T55] Scala：集合过滤
来源：http://wgq.gotoacloud.top

List(1, 2, 3).filter(_ > 1)
来源：http://gwz.sysykeji.top

[T56] Scala：样例类
来源：http://zmj.zycfv.cn

case class User(name: String, age: Int)
来源：http://tcy.shanyushiyangkeji.top

[T57] Scala：模式匹配
来源：http://zys.haohaochexian.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ljb.sufxvd.cn

[T58] Scala：函数定义
来源：http://moj.zhongyouzk.top

def add(a: Int, b: Int): Int = a + b
来源：http://zvh.guowangkeji.top

[T59] Scala：循环
来源：http://hit.hysaishi.cn

for (i <- 1 to 10) println(i)
来源：http://per.jinyuanbaomall.cn

[T60] Scala：折叠
来源：http://kix.52xcode.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://omf.xylfe.cn

================================================================================
来源：http://nxj.ehwqpu.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vcs.sxryk.cn

================================================================================
来源：http://jbs.yj20258888.top

[U01] Py：创建虚拟环境
来源：http://xgx.tarul.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qnz.chenjidiqi.icu

[U02] Py：导出 / 安装依赖
来源：http://uax.yj20258888.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fmq.yuxming.cn

[U03] Py：加载 .env 配置
来源：http://epj.epnwcf.com

from dotenv import load_dotenv; load_dotenv()
来源：http://atc.wangshuangyany.cn

[U04] Py：变量调试打印
来源：http://enx.zhiwuduotai.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://csw.gotoacloud.top

[U05] Py：列表去重且保序
来源：http://bos.aibaodan.cn

list(dict.fromkeys(arr))
来源：http://gqa.yj20258.top

[U06] Py：合并两个字典
来源：http://wcu.nwbrower.top

{**a, **b}
来源：http://acb.shuidangran.top

[U07] Py：反转字典键值
来源：http://nqi.jianghu66.top

{v: k for k, v in d.items()}
来源：http://jzk.chenjidiqi.icu

[U08] Py：展平二维列表
来源：http://blm.ywan-chungtsiang.top

[y for x in nested for y in x]
来源：http://xrd.zhoulong.xyz

[U09] Py：字典取最大值的键
来源：http://wvq.ybcxt.top

max(d, key=d.get)
来源：http://jgn.uphjek.com

[U10] Py：按值排序字典
来源：http://cbu.ybcxt.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gpb.zdqjudy.top

[U11] Py：生成器表达式
来源：http://lkp.yj202588.top

(x * 2 for x in arr)
来源：http://cgs.hfpthk.cn

[U12] Py：取出现最多的 3 个元素
来源：http://tac.feifeiyinyue.top

Counter(arr).most_common(3)
来源：http://zuq.9152youxi.cn

[U13] Py：固定长度队列
来源：http://ljh.aizwys.cn

deque(maxlen=10)
来源：http://dvz.jlsjyb.cn

[U14] Py：分组收集到列表
来源：http://ixm.yuxming.cn

defaultdict(list)
来源：http://pqt.daxiang520.top

[U15] Py：高精度计时
来源：http://niu.ppjwa.cn

t = time.perf_counter()
来源：http://rot.tianlin.xyz

[U16] Py：命令行参数解析
来源：http://reo.feifeiyinyue.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pyg.chenlongwang.top

[U17] Py：初始化日志
来源：http://dzq.sysykeji.top

logging.basicConfig(level=logging.INFO)
来源：http://qdn.nwbrower.top

[U18] Py：预编译正则
来源：http://itc.fzhhl.top

pat = re.compile(r"\d+")
来源：http://aky.zycfv.cn

[U19] Py：正则替换带回调
来源：http://bdy.xingfuxueyuan.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://olc.jinqigufen.top

[U20] Py：缓存函数结果
来源：http://tin.ybcxt.top

@functools.lru_cache(maxsize=None)
来源：http://cqb.yangfankeji.com

[U21] Py：自定义上下文管理器
来源：http://vtz.shanyushiyangkeji.top

@contextlib.contextmanager
来源：http://uqu.tarul.cn

[U22] Py：矩阵转置
来源：http://bgf.yangfankeji.com

list(zip(*m))
来源：http://stq.birdmap.top

[U23] Py：分块读取大文件
来源：http://xjr.aibaodan.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qpt.yuanzhike.top

[U24] Py：路径操作
来源：http://vyr.shangyingyoupin.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://aeo.cheryme.top

[U25] Py：CSV 按字典读
来源：http://zgn.sweek.top

csv.DictReader(f)
来源：http://nub.zhijiandao.cn

[U26] Py：并发下载
来源：http://dbn.vehdjk.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xwi.gzhubu.top

[U27] Py：异步 HTTP
来源：http://cih.jinqigufen.top

aiohttp.ClientSession() 配合 async with
来源：http://exm.zhaomingkeji.xyz

[U28] Py：类型别名
来源：http://gxo.chenzaomai.com

UserId = int
来源：http://nox.mhx1999.top

[U29] Py：属性校验
来源：http://mft.jinghuilouyu.cn

@property 与 @x.setter 配合
来源：http://isb.redwolf501.top

[U30] Py：数据类
来源：http://drp.wangshuangyany.cn

@dataclass(slots=True)
来源：http://wly.c1oappe.top

[U31] Py：单测
来源：http://wov.ctjpmb.com

python -m pytest -q
来源：http://ral.cashguo.top

[U32] Py：代码格式化
来源：http://skv.smart0.xyz

ruff format . && ruff check --fix .
来源：http://tel.shzxlz.cn

[U33] Py：打包发布
来源：http://gow.zycfv.cn

python -m build  （依赖 pyproject.toml）
来源：http://vnb.xinyue.icu

[U34] Py：判断编码
来源：http://edl.hnxiangtu.top

chardet.detect(raw)
来源：http://syh.sweek.top

[U35] Py：发送邮件
来源：http://wip.zhijiandao.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mix.chenzaomai.com

[U36] Py：定时任务
来源：http://rgo.bbcook.cn

schedule.every(10).minutes.do(job)
来源：http://npj.zhiwuduotai.top

[U37] Py：读写 Excel
来源：http://bxd.jianghu66.top

pandas.read_excel / DataFrame.to_excel
来源：http://abv.nanxinkj.top

[U38] Py：获取脚本所在目录
来源：http://ghb.xylfe.cn

Path(__file__).resolve().parent
来源：http://pzv.nwbrower.top

[U39] Py：判断是否在交互环境
来源：http://wti.cqqwz.cn

sys.stdout.isatty()
来源：http://wjp.aibaodan.cn

[U40] Py：打印到标准错误
来源：http://kib.zdqjudy.top

print("err", file=sys.stderr)
来源：http://rrm.zdqjudy.top

[U41] PHP：初始化 Composer 项目
来源：http://dni.jiagoushi.top

composer init;  composer require guzzlehttp/guzzle
来源：http://glb.tanke756.top

[U42] PHP：PSR-4 自动加载
来源：http://iod.shuidangran.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ctx.gotoacloud.top

[U43] PHP：声明命名空间
来源：http://wmm.gaohongyu789.top

namespace App\Http;
来源：http://agy.fanxiaobao.xyz

[U44] PHP：开启严格类型
来源：http://tfo.andypj.xyz

declare(strict_types=1);
来源：http://vyb.dashuyun.cn

[U45] PHP：类型声明与返回类型
来源：http://ecy.hysaishi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://mva.ydzc1.top

[U46] PHP：可空类型
来源：http://mvh.jinqigfzy.top

?string $name = null
来源：http://jsg.fzhhl.top

[U47] PHP：联合类型
来源：http://kmn.jqgfzy.top

int|string $id
来源：http://fhr.cucudq.cn

[U48] PHP：纯枚举
来源：http://jic.hnxiangtu.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bua.zhiwuduotai.top

[U49] PHP：只读属性
来源：http://fqn.xylfe.cn

public readonly string $name
来源：http://acs.fengsongda.top

[U50] PHP：构造器属性提升
来源：http://mug.hysaishi.cn

public function __construct(private int $id) {}
来源：http://qlf.jyoumei.cn

[U51] PHP：数组解构
来源：http://rza.316326.xyz

[$a, $b] = $arr;
来源：http://bnx.hysaishi.cn

[U52] PHP：箭头函数
来源：http://moa.pycfn.com

$double = fn($x) => $x * 2;
来源：http://oov.ywan-chungtsiang.top

[U53] PHP：空合并运算符
来源：http://swc.jqgfzy.top

$v = $a ?? $b ?? "default";
来源：http://dmd.dashuyun.cn

[U54] PHP：空安全调用
来源：http://tje.jqgufenzy.top

$obj?->method()
来源：http://ofk.zhijiandao.cn

[U55] PHP：match 表达式
来源：http://eqp.aibaodan.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jyq.jinyuanbaomall.cn

[U56] PHP：命名参数
来源：http://wff.ctjpmb.com

f(a: 1, b: 2)
来源：http://bif.shanyushiyangtech.top

[U57] PHP：字符串插值
来源：http://acj.316326.xyz

"值: {$a}"
来源：http://exb.tarul.cn

[U58] PHP：数组三件套
来源：http://vho.aizwys.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xsr.epnwcf.com

[U59] PHP：自定义排序
来源：http://yrs.pycfn.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mzz.shuidangran.top

[U60] PHP：JSON 编解码
来源：http://iyr.ybcxt.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gmq.birdmap.top

[U61] PHP：正则
来源：http://wix.snrcjt.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wxl.52xcode.cn

[U62] PHP：日期对象
来源：http://tre.hysaishi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fio.sxryk.cn

[U63] PHP：文件读写
来源：http://car.redwolf501.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bld.cdnleiting.top

[U64] PHP：目录遍历
来源：http://ozw.c1oappe.top

glob("dir/*.php");  scandir("dir");
来源：http://xka.jqgfzy.top

[U65] PHP：会话
来源：http://rhc.jinqigfzy.top

session_start();  $_SESSION["uid"] = 1;
来源：http://pzq.haohaochexian.top

[U66] PHP：设置 Cookie
来源：http://xpr.yuxming.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zef.zhaomingkeji.xyz

[U67] PHP：处理文件上传
来源：http://oku.cdnleiting.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mia.sufxvd.cn

[U68] PHP：PDO 连接
来源：http://uwu.haohaochexian.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qsu.jqgfzy.top

[U69] PHP：PDO 预处理
来源：http://zkq.tian-w.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lle.chenzaomai.com

[U70] PHP：PDO 事务
来源：http://gim.meibo888.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kkr.sxryk.cn

[U71] PHP：抛出异常
来源：http://dse.cheryme.top

throw new RuntimeException("失败", 500);
来源：http://jxt.yj202588.top

[U72] PHP：写错误日志
来源：http://mpn.jianghu66.top

error_log("失败: " . $e->getMessage());
来源：http://bci.tianlin.xyz

[U73] PHP：读取 ini 配置
来源：http://nal.cdnleiting.top

parse_ini_file("config.ini", true)
来源：http://vsa.zhaomingkeji.xyz

[U74] PHP：读取环境变量
来源：http://uft.andypj.xyz

getenv("APP_ENV") ?: "production"
来源：http://qdy.0kj1m.cn

[U75] PHP：依赖注入
来源：http://uzw.hongshengwenyu.top

composer require psr/container
来源：http://cfz.xingfuxueyuan.xyz

[U76] PHP：简单路由
来源：http://amv.zhengqikj.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vam.xingfuxueyuan.xyz

[U77] PHP：模板渲染
来源：http://mvv.yongpay.top

composer require twig/twig
来源：http://mmv.zhijiandao.cn

[U78] PHP：单元测试
来源：http://yca.cdnleiting.top

composer require --dev phpunit/phpunit
来源：http://rds.ctjpmb.com

[U79] PHP：静态分析
来源：http://crd.birdmap.top

composer require --dev phpstan/phpstan
来源：http://etk.chenjidiqi.icu

[U80] PHP：代码规范修复
来源：http://mrw.ydjk.org.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://rfb.shangyingyoupin.top

[U81] JS：初始化项目
来源：http://zkm.jqgufenzy.top

npm init -y;  npm i express
来源：http://dub.daria6918.cn

[U82] JS：package.json 脚本
来源：http://jei.sysykeji.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gzo.jinghuilouyu.cn

[U83] JS：ES Module 导入导出
来源：http://owc.shuidangran.top

export const a = 1;  import { a } from "./m.js";
来源：http://gzn.wangdashe.top

[U84] JS：CommonJS 写法
来源：http://sxb.zhoulong.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://xnl.bbcook.cn

[U85] JS：可选链
来源：http://mwb.nanxinkj.top

a?.b?.c
来源：http://whw.ydzc1.top

[U86] JS：空值合并
来源：http://aco.cheryme.top

a ?? b
来源：http://uiz.hcnkem.com

[U87] JS：解构默认值
来源：http://yxk.ivvv.top

const { a = 1, b = 2 } = obj;
来源：http://jbj.fehbvm.com

[U88] JS：对象展开合并
来源：http://noz.havefunace.top

{ ...a, ...b }
来源：http://kaw.ehwqpu.com

[U89] JS：数组去重
来源：http://ztc.xuetiantiany.cn

[...new Set(arr)]
来源：http://izn.fzhhl.top

[U90] JS：数字数组排序
来源：http://npz.haohaochexian.top

[...arr].sort((a, b) => a - b)
来源：http://ivq.jinyuanbaomall.cn

[U91] JS：对象键值遍历
来源：http://cgt.gaohongyu789.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ept.meibo888.top

[U92] JS：深拷贝
来源：http://zsy.zhengqikj.top

structuredClone(obj)
来源：http://ykv.ywan-chungtsiang.top

[U93] JS：模板字符串
来源：http://cja.xylfe.cn

`共 ${n} 条`
来源：http://rcp.epnwcf.com

[U94] JS：箭头函数
来源：http://nim.nwbrower.top

const double = x => x * 2;
来源：http://lmx.tarul.cn

[U95] JS：Promise 包装
来源：http://uxs.jiagoushi.top

new Promise((resolve, reject) => {})
来源：http://hdv.svipenyu.cn

[U96] JS：async/await 与异常
来源：http://okp.birdmap.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rja.jiagoushi.top

[U97] JS：并发请求
来源：http://ldd.316326.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://cow.shanyushiyangtech.top

[U98] JS：fetch 带 JSON
来源：http://fkt.9152youxi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gfi.tanke756.top

[U99] JS：事件监听
来源：http://vnf.ppjwa.cn

el.addEventListener("click", e => {})
来源：http://yug.ybcxt.top

[U100] JS：DOM 查询
来源：http://uqw.zycfv.cn

document.querySelector(".item")
来源：http://xhz.cashguo.top

[U101] JS：classList 操作
来源：http://yjc.vehdjk.com

el.classList.toggle("active")
来源：http://zpt.hesvh.cn

[U102] JS：本地存储
来源：http://cwv.ydzc1.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://rom.yanxiufei.cn

[U103] JS：定时器
来源：http://ijg.ydjk.org.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://cnx.tian-w.cn

[U104] JS：防抖
来源：http://fde.nanxinkj.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tab.wangshuangyany.cn

[U105] JS：节流
来源：http://nyt.xinyue.icu

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://oxy.xziqi.cn

[U106] JS：日期格式化
来源：http://ywk.vehdjk.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://azg.9152youxi.cn

[U107] JS：数字千分位
来源：http://vqk.hywenlv.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://oxu.ctjpmb.com

[U108] JS：随机整数
来源：http://mrx.c1oappe.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tjc.epnwcf.com

[U109] JS：数组分组
来源：http://cve.zhoulong.xyz

Object.groupBy(arr, x => x.type)
来源：http://ike.haohaochexian.top

[U110] JS：数组分块
来源：http://ogd.fehbvm.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yst.jyoumei.cn

[U111] JS：对象转 Map
来源：http://ogm.zhiwuduotai.top

new Map(Object.entries(obj))
来源：http://svw.quarkkingdee.top

[U112] JS：字符串补位
来源：http://msf.guowangkeji.top

"7".padStart(3, "0")
来源：http://mcc.birdmap.top

[U113] JS：正则替换全部
来源：http://lii.gaohongyu789.top

s.replaceAll("a", "b")
来源：http://hmn.ehwqpu.com

[U114] JS：JSON 深比较
来源：http://why.jianghu66.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://uqe.uphjek.com

[U115] JS：生成 UUID
来源：http://cpi.yanxiufei.cn

crypto.randomUUID()
来源：http://tih.uphjek.com

[U116] JS：类型检查（JSDoc）
来源：http://rld.gzhubu.top

/** @param {string} name */ function f(name) {}
来源：http://qzn.yanxiufei.cn

[U117] JS：单元测试
来源：http://fdg.guowangkeji.top

npm i -D vitest;  npx vitest
来源：http://lgs.nanxuanxn.top

[U118] JS：开发服务器
来源：http://gjn.fktsv.cn

npm i -D vite;  npx vite
来源：http://cwd.shuidangran.top

[U119] JS：生产构建
来源：http://mhd.zdqjudy.top

npx vite build
来源：http://vzt.ehwqpu.com

[U120] JS：读取环境变量（Vite）
来源：http://msc.yj202588.top

import.meta.env.VITE_API_URL
来源：http://kmf.vehdjk.com

================================================================================
来源：http://koa.hongshengwenyu.top

统计汇总
来源：http://cfe.jinqigufen.top

================================================================================
来源：http://eps.gotoacloud.top

按语言统计（条）：
来源：http://kuf.c1oappe.top

Python ......... 252
来源：http://xqb.jinghuilouyu.cn

PHP ............ 252
来源：http://qbe.smart0.xyz

JavaScript ..... 252
来源：http://epq.zhaomingkeji.xyz

TypeScript ..... 212
来源：http://zuu.zhijiandao.cn

Java ........... 212
来源：http://eed.nwbrower.top

Go ............. 212
来源：http://yzs.jianghu66.top

Ruby ........... 212
来源：http://amy.kuanghao11.cn

C# ............. 212
来源：http://yho.chenjidiqi.icu

C .............. 30
来源：http://lej.aizwys.cn

C++ ............ 30
来源：http://zxq.nanxinkj.top

SQL ............ 90
来源：http://wdx.hysaishi.cn

Bash ........... 80
来源：http://jbi.yj20258.top

Kotlin ......... 15
来源：http://rgo.yj202588.top

Swift .......... 15
来源：http://thu.yj202588.top

Lua ............ 10
来源：http://wpq.dashuyun.cn

Perl ........... 10
来源：http://avy.zhiwuduotai.top

Scala .......... 10
来源：http://idt.aizwys.cn

------------------------------------
来源：http://siq.xziqi.cn

合计 ........... 2106 条
来源：http://ccj.daria6918.cn

按章节统计：
来源：http://pvo.bbcook.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://htz.sjlbkw.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://epn.chenzaomai.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://axp.haohaochexian.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://oep.gotoacloud.top


<!-- 参考信息 -->