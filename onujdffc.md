代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://nxj.yj202588.top

[T51] Scala：Hello World
来源：http://ebw.tarul.cn

println("Hello")
来源：http://xui.chenzaomai.com

[T52] Scala：变量
来源：http://hin.zhengqikj.top

val a = 1;  var b = 2
来源：http://yme.nanxinkj.top

[T53] Scala：字符串插值
来源：http://yim.0kj1m.cn

s"值: $b"
来源：http://zlf.meibo888.top

[T54] Scala：集合映射
来源：http://zzm.epnwcf.com

List(1, 2, 3).map(_ * 2)
来源：http://ave.zhijiandao.cn

[T55] Scala：集合过滤
来源：http://lmp.cqqwz.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qix.hesvh.cn

[T56] Scala：样例类
来源：http://tjn.gzhubu.top

case class User(name: String, age: Int)
来源：http://alo.snrcjt.cn

[T57] Scala：模式匹配
来源：http://vvp.ctjpmb.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://gxj.nwbrower.top

[T58] Scala：函数定义
来源：http://ooz.chenzaomai.com

def add(a: Int, b: Int): Int = a + b
来源：http://yta.svipenyu.cn

[T59] Scala：循环
来源：http://wxk.52xcode.cn

for (i <- 1 to 10) println(i)
来源：http://ihu.jyoumei.cn

[T60] Scala：折叠
来源：http://qew.fehbvm.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ekq.fzhhl.top

================================================================================
来源：http://jho.tian-w.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vho.hnxiangtu.top

================================================================================
来源：http://odm.hnxiangtu.top

[U01] Py：创建虚拟环境
来源：http://zyy.shanyushiyangtech.top

python -m venv .venv && source .venv/bin/activate
来源：http://wua.gzhubu.top

[U02] Py：导出 / 安装依赖
来源：http://fnh.aibaodan.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://eja.hfpthk.cn

[U03] Py：加载 .env 配置
来源：http://zug.sufxvd.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://bln.chenjidiqi.icu

[U04] Py：变量调试打印
来源：http://mcb.c1oappe.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ogn.dashuyun.cn

[U05] Py：列表去重且保序
来源：http://dyh.cqqwz.cn

list(dict.fromkeys(arr))
来源：http://yhr.jyoumei.cn

[U06] Py：合并两个字典
来源：http://kzk.jqgfzy.top

{**a, **b}
来源：http://ikd.yuanzhike.top

[U07] Py：反转字典键值
来源：http://zmb.sjlbkw.cn

{v: k for k, v in d.items()}
来源：http://xcv.zycfv.cn

[U08] Py：展平二维列表
来源：http://hse.zhaomingkeji.xyz

[y for x in nested for y in x]
来源：http://lwj.jiagoushi.top

[U09] Py：字典取最大值的键
来源：http://cbi.zhoulong.xyz

max(d, key=d.get)
来源：http://pzn.jlsjyb.cn

[U10] Py：按值排序字典
来源：http://iol.fzhhl.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://owc.haohaochexian.top

[U11] Py：生成器表达式
来源：http://dgv.zhixingplan.top

(x * 2 for x in arr)
来源：http://lbe.xingfuxueyuan.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://nnx.aibaodan.cn

Counter(arr).most_common(3)
来源：http://gdx.xinyue.icu

[U13] Py：固定长度队列
来源：http://mvl.aizwys.cn

deque(maxlen=10)
来源：http://oed.quarkkingdee.top

[U14] Py：分组收集到列表
来源：http://rrf.uphjek.com

defaultdict(list)
来源：http://qci.yangfankeji.com

[U15] Py：高精度计时
来源：http://yup.sufxvd.cn

t = time.perf_counter()
来源：http://gfa.xuetiantiany.cn

[U16] Py：命令行参数解析
来源：http://ext.fengsongda.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://frv.meibo888.top

[U17] Py：初始化日志
来源：http://pmw.iojbl.cn

logging.basicConfig(level=logging.INFO)
来源：http://ssi.zhaomingkeji.xyz

[U18] Py：预编译正则
来源：http://iay.hywenlv.cn

pat = re.compile(r"\d+")
来源：http://bhk.hnqzz.top

[U19] Py：正则替换带回调
来源：http://qpp.yongpay.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kik.yfazqb.com

[U20] Py：缓存函数结果
来源：http://mbn.zhijiandao.cn

@functools.lru_cache(maxsize=None)
来源：http://fch.guannengcc.top

[U21] Py：自定义上下文管理器
来源：http://zev.chenjidiqi.icu

@contextlib.contextmanager
来源：http://bkb.zhijiandao.cn

[U22] Py：矩阵转置
来源：http://aht.ctjpmb.com

list(zip(*m))
来源：http://ddt.jinghuilouyu.cn

[U23] Py：分块读取大文件
来源：http://vmp.shanyushiyangtech.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rfw.epnwcf.com

[U24] Py：路径操作
来源：http://pek.52xcode.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tev.haohaochexian.top

[U25] Py：CSV 按字典读
来源：http://fqt.tianlin.xyz

csv.DictReader(f)
来源：http://kyo.zdbjq.cn

[U26] Py：并发下载
来源：http://zok.chenlongwang.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bqw.hesvh.cn

[U27] Py：异步 HTTP
来源：http://grx.jinqigfzy.top

aiohttp.ClientSession() 配合 async with
来源：http://hfb.hfpthk.cn

[U28] Py：类型别名
来源：http://laq.sjlbkw.cn

UserId = int
来源：http://zwi.yangfankeji.com

[U29] Py：属性校验
来源：http://tds.meibo888.top

@property 与 @x.setter 配合
来源：http://rlt.svipenyu.cn

[U30] Py：数据类
来源：http://tjh.ywan-chungtsiang.top

@dataclass(slots=True)
来源：http://ifd.ywan-chungtsiang.top

[U31] Py：单测
来源：http://olx.52xcode.cn

python -m pytest -q
来源：http://lbf.wangshuangyany.cn

[U32] Py：代码格式化
来源：http://ead.hesvh.cn

ruff format . && ruff check --fix .
来源：http://rxj.birdmap.top

[U33] Py：打包发布
来源：http://ggp.0kj1m.cn

python -m build  （依赖 pyproject.toml）
来源：http://vwh.hysaishi.cn

[U34] Py：判断编码
来源：http://jzo.aibaodan.cn

chardet.detect(raw)
来源：http://cdf.redwolf501.top

[U35] Py：发送邮件
来源：http://gth.ppjwa.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qal.zhiwuduotai.top

[U36] Py：定时任务
来源：http://irh.fktsv.cn

schedule.every(10).minutes.do(job)
来源：http://xxz.gaohongyu789.top

[U37] Py：读写 Excel
来源：http://rhy.aibaodan.cn

pandas.read_excel / DataFrame.to_excel
来源：http://dvq.hesvh.cn

[U38] Py：获取脚本所在目录
来源：http://ldg.jinyuanbaomall.cn

Path(__file__).resolve().parent
来源：http://gpj.hnxiangtu.top

[U39] Py：判断是否在交互环境
来源：http://jhs.xingfuxueyuan.xyz

sys.stdout.isatty()
来源：http://ann.redwolf501.top

[U40] Py：打印到标准错误
来源：http://gta.hcnkem.com

print("err", file=sys.stderr)
来源：http://bez.zhengqikj.top

[U41] PHP：初始化 Composer 项目
来源：http://vnu.havefunace.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ouk.zhaomingkeji.xyz

[U42] PHP：PSR-4 自动加载
来源：http://aud.yonumen.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mdq.vqdsnc.cn

[U43] PHP：声明命名空间
来源：http://fqe.fzhhl.top

namespace App\Http;
来源：http://itu.pengpengdd.cyou

[U44] PHP：开启严格类型
来源：http://pnq.aizwys.cn

declare(strict_types=1);
来源：http://gxy.fanxiaobao.xyz

[U45] PHP：类型声明与返回类型
来源：http://xau.dashuyun.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://hmc.hfpthk.cn

[U46] PHP：可空类型
来源：http://ceh.zhoulong.xyz

?string $name = null
来源：http://wpm.jlsjyb.cn

[U47] PHP：联合类型
来源：http://keb.yj20258888.top

int|string $id
来源：http://sxl.yonumen.top

[U48] PHP：纯枚举
来源：http://hdl.mhx1999.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hqs.hesvh.cn

[U49] PHP：只读属性
来源：http://fih.wangdashe.top

public readonly string $name
来源：http://cno.hnqzz.top

[U50] PHP：构造器属性提升
来源：http://wqb.ehwqpu.com

public function __construct(private int $id) {}
来源：http://hfw.shanyushiyangtech.top

[U51] PHP：数组解构
来源：http://fee.xylfe.cn

[$a, $b] = $arr;
来源：http://sgn.pengpengdd.cyou

[U52] PHP：箭头函数
来源：http://xtd.ybcxt.top

$double = fn($x) => $x * 2;
来源：http://yig.jiagoushi.top

[U53] PHP：空合并运算符
来源：http://rvb.yuxming.cn

$v = $a ?? $b ?? "default";
来源：http://rfp.aizwys.cn

[U54] PHP：空安全调用
来源：http://hfh.zycfv.cn

$obj?->method()
来源：http://cpj.xuanzx.com

[U55] PHP：match 表达式
来源：http://wsg.gotoacloud.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bxg.zhijiandao.cn

[U56] PHP：命名参数
来源：http://vig.52xcode.cn

f(a: 1, b: 2)
来源：http://luw.jqgfzy.top

[U57] PHP：字符串插值
来源：http://ptj.yj20258888.top

"值: {$a}"
来源：http://ffq.jyoumei.cn

[U58] PHP：数组三件套
来源：http://puc.yangfankeji.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gro.zhoulong.xyz

[U59] PHP：自定义排序
来源：http://xuh.guannengcc.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ahp.ivvv.top

[U60] PHP：JSON 编解码
来源：http://mps.fengsongda.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kgn.pengpengdd.cyou

[U61] PHP：正则
来源：http://fak.aibaodan.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ron.haohaochexian.top

[U62] PHP：日期对象
来源：http://ujl.jiagoushi.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fhj.iojbl.cn

[U63] PHP：文件读写
来源：http://bke.xziqi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tya.jinghuilouyu.cn

[U64] PHP：目录遍历
来源：http://cdw.sxryk.cn

glob("dir/*.php");  scandir("dir");
来源：http://bdi.0kj1m.cn

[U65] PHP：会话
来源：http://fyt.gogol.net.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://tsg.wangshuangyany.cn

[U66] PHP：设置 Cookie
来源：http://ifw.ppjwa.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ayt.svipenyu.cn

[U67] PHP：处理文件上传
来源：http://ken.shanyushiyangtech.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mzt.pengpengdd.cyou

[U68] PHP：PDO 连接
来源：http://tpe.ydzc1.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ynq.wangshuangyany.cn

[U69] PHP：PDO 预处理
来源：http://mdh.shanyushiyangtech.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nve.xylfe.cn

[U70] PHP：PDO 事务
来源：http://zet.zhongyouzk.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://eyj.jinqigfzy.top

[U71] PHP：抛出异常
来源：http://frk.jinyuanbaomall.cn

throw new RuntimeException("失败", 500);
来源：http://ykk.havefunace.top

[U72] PHP：写错误日志
来源：http://tfb.wangdashe.top

error_log("失败: " . $e->getMessage());
来源：http://wrd.chenzaomai.com

[U73] PHP：读取 ini 配置
来源：http://aqh.quarkkingdee.top

parse_ini_file("config.ini", true)
来源：http://xnm.nanxuanxn.top

[U74] PHP：读取环境变量
来源：http://ohq.guowangkeji.top

getenv("APP_ENV") ?: "production"
来源：http://pzt.wangdashe.top

[U75] PHP：依赖注入
来源：http://wvi.yj202588.top

composer require psr/container
来源：http://cxi.pycfn.com

[U76] PHP：简单路由
来源：http://nxc.hcnkem.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://joc.jlsjyb.cn

[U77] PHP：模板渲染
来源：http://xru.svipenyu.cn

composer require twig/twig
来源：http://dca.fktsv.cn

[U78] PHP：单元测试
来源：http://inu.feifeiyinyue.top

composer require --dev phpunit/phpunit
来源：http://bqi.fktsv.cn

[U79] PHP：静态分析
来源：http://eim.havefunace.top

composer require --dev phpstan/phpstan
来源：http://njk.zycfv.cn

[U80] PHP：代码规范修复
来源：http://fvs.kuanghao11.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://azc.jqgfzy.top

[U81] JS：初始化项目
来源：http://fre.zhijiandao.cn

npm init -y;  npm i express
来源：http://ekr.zycfv.cn

[U82] JS：package.json 脚本
来源：http://zzw.sjlbkw.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mey.cdnleiting.top

[U83] JS：ES Module 导入导出
来源：http://ftb.nwbrower.top

export const a = 1;  import { a } from "./m.js";
来源：http://kkq.ybcxt.top

[U84] JS：CommonJS 写法
来源：http://imr.pycfn.com

module.exports = { a };  const { a } = require("./m");
来源：http://ics.xuetiantiany.cn

[U85] JS：可选链
来源：http://sku.jqgufenzy.top

a?.b?.c
来源：http://wbj.shanyushiyangtech.top

[U86] JS：空值合并
来源：http://unp.xinyue.icu

a ?? b
来源：http://vkr.chenlongwang.top

[U87] JS：解构默认值
来源：http://kys.cashguo.top

const { a = 1, b = 2 } = obj;
来源：http://dhf.svipenyu.cn

[U88] JS：对象展开合并
来源：http://rhd.meibo888.top

{ ...a, ...b }
来源：http://hxi.guowangkeji.top

[U89] JS：数组去重
来源：http://nbl.chenjidiqi.icu

[...new Set(arr)]
来源：http://pyr.ppjwa.cn

[U90] JS：数字数组排序
来源：http://chc.ybcxt.top

[...arr].sort((a, b) => a - b)
来源：http://ltt.feifeiyinyue.top

[U91] JS：对象键值遍历
来源：http://ksn.bbcook.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://adn.snrcjt.cn

[U92] JS：深拷贝
来源：http://pcg.yvedp.cn

structuredClone(obj)
来源：http://xgd.xziqi.cn

[U93] JS：模板字符串
来源：http://wiw.xuanzx.com

`共 ${n} 条`
来源：http://bpr.zdqjudy.top

[U94] JS：箭头函数
来源：http://qyn.jqgfzy.top

const double = x => x * 2;
来源：http://wzk.wangdashe.top

[U95] JS：Promise 包装
来源：http://hzg.mhx1999.top

new Promise((resolve, reject) => {})
来源：http://hqp.vehdjk.com

[U96] JS：async/await 与异常
来源：http://zvp.pycfn.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vgy.daria6918.cn

[U97] JS：并发请求
来源：http://hpv.zhengqikj.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://lce.feifeiyinyue.top

[U98] JS：fetch 带 JSON
来源：http://ajd.cheryme.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cvr.cheryme.top

[U99] JS：事件监听
来源：http://qbw.yongpay.top

el.addEventListener("click", e => {})
来源：http://ist.52xcode.cn

[U100] JS：DOM 查询
来源：http://jrj.316326.xyz

document.querySelector(".item")
来源：http://zce.shuidangran.top

[U101] JS：classList 操作
来源：http://hau.ydjk.org.cn

el.classList.toggle("active")
来源：http://knf.fehbvm.com

[U102] JS：本地存储
来源：http://puv.sufxvd.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://lyd.snrcjt.cn

[U103] JS：定时器
来源：http://fyy.vqdsnc.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gmy.yuxming.cn

[U104] JS：防抖
来源：http://juv.yvedp.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yxe.daria6918.cn

[U105] JS：节流
来源：http://zad.vehdjk.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ker.guowangkeji.top

[U106] JS：日期格式化
来源：http://avr.yvedp.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wqe.dianchejie.cn

[U107] JS：数字千分位
来源：http://ric.bjfxy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bus.fanxiaobao.xyz

[U108] JS：随机整数
来源：http://vaa.epnwcf.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://evr.nwbrower.top

[U109] JS：数组分组
来源：http://tjt.hammf.cn

Object.groupBy(arr, x => x.type)
来源：http://rvt.xuanzx.com

[U110] JS：数组分块
来源：http://sjj.zhongyouzk.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mpo.gotoacloud.top

[U111] JS：对象转 Map
来源：http://ndv.hnxiangtu.top

new Map(Object.entries(obj))
来源：http://wdf.zdqjudy.top

[U112] JS：字符串补位
来源：http://bwd.tian-w.cn

"7".padStart(3, "0")
来源：http://cql.haohaochexian.top

[U113] JS：正则替换全部
来源：http://fvc.hongshengwenyu.top

s.replaceAll("a", "b")
来源：http://mcr.9152youxi.cn

[U114] JS：JSON 深比较
来源：http://ipq.316326.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://eli.yuxming.cn

[U115] JS：生成 UUID
来源：http://vvg.hcnkem.com

crypto.randomUUID()
来源：http://jpl.yj20258888.top

[U116] JS：类型检查（JSDoc）
来源：http://wzg.jqgufenzy.top

/** @param {string} name */ function f(name) {}
来源：http://omn.yvedp.cn

[U117] JS：单元测试
来源：http://vsp.xinyue.icu

npm i -D vitest;  npx vitest
来源：http://qnm.nanxinkj.top

[U118] JS：开发服务器
来源：http://pnw.52xcode.cn

npm i -D vite;  npx vite
来源：http://jqi.52xcode.cn

[U119] JS：生产构建
来源：http://gck.wangshuangyany.cn

npx vite build
来源：http://dof.cheryme.top

[U120] JS：读取环境变量（Vite）
来源：http://huu.tianlin.xyz

import.meta.env.VITE_API_URL
来源：http://nhy.nwbrower.top

================================================================================
来源：http://zvw.cucudq.cn

统计汇总
来源：http://dbx.ybcxt.top

================================================================================
来源：http://rjo.sjlbkw.cn

按语言统计（条）：
来源：http://ztx.xylfe.cn

Python ......... 252
来源：http://kkx.guannengcc.top

PHP ............ 252
来源：http://nuw.hywenlv.cn

JavaScript ..... 252
来源：http://fic.tian-w.cn

TypeScript ..... 212
来源：http://lzj.hcnkem.com

Java ........... 212
来源：http://hfh.zhaomingkeji.xyz

Go ............. 212
来源：http://iyq.xuetiantiany.cn

Ruby ........... 212
来源：http://bma.yj20258888.top

C# ............. 212
来源：http://slv.jqgfzy.top

C .............. 30
来源：http://rga.epnwcf.com

C++ ............ 30
来源：http://zcu.9152youxi.cn

SQL ............ 90
来源：http://nmo.0kj1m.cn

Bash ........... 80
来源：http://wzh.52xcode.cn

Kotlin ......... 15
来源：http://wcw.52xcode.cn

Swift .......... 15
来源：http://klz.redwolf501.top

Lua ............ 10
来源：http://hou.dianchejie.cn

Perl ........... 10
来源：http://xtq.ivvv.top

Scala .......... 10
来源：http://ykk.vehdjk.com

------------------------------------
来源：http://ovf.guannengcc.top

合计 ........... 2106 条
来源：http://ify.tian-w.cn

按章节统计：
来源：http://jya.shanyushiyangtech.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://nrz.xuetiantiany.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mhr.sjlbkw.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://zje.sxryk.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://piz.hywenlv.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qgi.ywan-chungtsiang.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://sva.cqqwz.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zzv.sxryk.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nvl.jqgufenzy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://cmj.nanxinkj.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fne.cashguo.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dxl.fanxiaobao.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cvk.pycfn.com


<!-- 参考信息 -->