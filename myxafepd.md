代发 wailian999

val a = 1;  var b = 2
来源：http://wrg.xingfuxueyuan.xyz

[T53] Scala：字符串插值
来源：http://yob.hnqzz.top

s"值: $b"
来源：http://fzy.jinyuanbaomall.cn

[T54] Scala：集合映射
来源：http://lxd.tanke756.top

List(1, 2, 3).map(_ * 2)
来源：http://yuv.smart0.xyz

[T55] Scala：集合过滤
来源：http://rkp.wangdashe.top

List(1, 2, 3).filter(_ > 1)
来源：http://bxw.fehbvm.com

[T56] Scala：样例类
来源：http://jsb.hammf.cn

case class User(name: String, age: Int)
来源：http://yqo.jinyuanbaomall.cn

[T57] Scala：模式匹配
来源：http://edm.zhengqikj.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://trx.ehwqpu.com

[T58] Scala：函数定义
来源：http://lme.cqqwz.cn

def add(a: Int, b: Int): Int = a + b
来源：http://cfq.yvedp.cn

[T59] Scala：循环
来源：http://jjv.zhongyouzk.top

for (i <- 1 to 10) println(i)
来源：http://ffk.fktsv.cn

[T60] Scala：折叠
来源：http://ekp.andypj.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hib.hysaishi.cn

================================================================================
来源：http://fnk.sjlbkw.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yey.nwbrower.top

================================================================================
来源：http://gtk.shzxlz.cn

[U01] Py：创建虚拟环境
来源：http://ssm.yangfankeji.com

python -m venv .venv && source .venv/bin/activate
来源：http://uqp.ydjk.org.cn

[U02] Py：导出 / 安装依赖
来源：http://obs.vqdsnc.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zlu.sufxvd.cn

[U03] Py：加载 .env 配置
来源：http://dku.jinghuilouyu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://lpo.meibo888.top

[U04] Py：变量调试打印
来源：http://nof.yvedp.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://oyz.guowangkeji.top

[U05] Py：列表去重且保序
来源：http://lhz.havefunace.top

list(dict.fromkeys(arr))
来源：http://ycx.vqdsnc.cn

[U06] Py：合并两个字典
来源：http://egc.ppjwa.cn

{**a, **b}
来源：http://rjb.dianchejie.cn

[U07] Py：反转字典键值
来源：http://mzw.yueranfly.top

{v: k for k, v in d.items()}
来源：http://zms.jinqigfzy.top

[U08] Py：展平二维列表
来源：http://kbq.yfazqb.com

[y for x in nested for y in x]
来源：http://hdd.cashguo.top

[U09] Py：字典取最大值的键
来源：http://jyn.gzhubu.top

max(d, key=d.get)
来源：http://hlr.zhongyouzk.top

[U10] Py：按值排序字典
来源：http://utb.xingfuxueyuan.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://meg.yangfankeji.com

[U11] Py：生成器表达式
来源：http://qjx.hongshengwenyu.top

(x * 2 for x in arr)
来源：http://oxl.tian-w.cn

[U12] Py：取出现最多的 3 个元素
来源：http://vsu.52xcode.cn

Counter(arr).most_common(3)
来源：http://uor.zdqjudy.top

[U13] Py：固定长度队列
来源：http://znn.daxiang520.top

deque(maxlen=10)
来源：http://ihz.cqqwz.cn

[U14] Py：分组收集到列表
来源：http://aoe.sufxvd.cn

defaultdict(list)
来源：http://sms.hongshengwenyu.top

[U15] Py：高精度计时
来源：http://qzz.gaohongyu789.top

t = time.perf_counter()
来源：http://gwq.cqqwz.cn

[U16] Py：命令行参数解析
来源：http://rnb.havefunace.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dcn.shanyushiyangtech.top

[U17] Py：初始化日志
来源：http://lwl.xinyue.icu

logging.basicConfig(level=logging.INFO)
来源：http://mqp.316326.xyz

[U18] Py：预编译正则
来源：http://del.fehbvm.com

pat = re.compile(r"\d+")
来源：http://mma.cashguo.top

[U19] Py：正则替换带回调
来源：http://jzy.pycfn.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mvr.zhijiandao.cn

[U20] Py：缓存函数结果
来源：http://ltx.xylfe.cn

@functools.lru_cache(maxsize=None)
来源：http://fnk.nwbrower.top

[U21] Py：自定义上下文管理器
来源：http://vif.wangshuangyany.cn

@contextlib.contextmanager
来源：http://ikn.haohaochexian.top

[U22] Py：矩阵转置
来源：http://pzc.tian-w.cn

list(zip(*m))
来源：http://hnc.hywenlv.cn

[U23] Py：分块读取大文件
来源：http://lve.cqqwz.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://avr.ppjwa.cn

[U24] Py：路径操作
来源：http://faj.smart0.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tqg.gotoacloud.top

[U25] Py：CSV 按字典读
来源：http://akp.shzxlz.cn

csv.DictReader(f)
来源：http://rhm.ywan-chungtsiang.top

[U26] Py：并发下载
来源：http://hzd.chenzaomai.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://exr.meibo888.top

[U27] Py：异步 HTTP
来源：http://ucb.jinqigufen.top

aiohttp.ClientSession() 配合 async with
来源：http://fbe.yj20258.top

[U28] Py：类型别名
来源：http://bwk.hesvh.cn

UserId = int
来源：http://rkc.yueranfly.top

[U29] Py：属性校验
来源：http://qbh.sjlbkw.cn

@property 与 @x.setter 配合
来源：http://hts.daxiang520.top

[U30] Py：数据类
来源：http://xdl.feifeiyinyue.top

@dataclass(slots=True)
来源：http://jvv.cucudq.cn

[U31] Py：单测
来源：http://ttv.bjfxy.top

python -m pytest -q
来源：http://ctk.ivvv.top

[U32] Py：代码格式化
来源：http://uto.jqgufenzy.top

ruff format . && ruff check --fix .
来源：http://ibq.nanxinkj.top

[U33] Py：打包发布
来源：http://npn.feifeiyinyue.top

python -m build  （依赖 pyproject.toml）
来源：http://tgy.birdmap.top

[U34] Py：判断编码
来源：http://mqr.ppjwa.cn

chardet.detect(raw)
来源：http://wvm.316326.xyz

[U35] Py：发送邮件
来源：http://jbw.zhaomingkeji.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gdm.yueranfly.top

[U36] Py：定时任务
来源：http://sqd.zhijiandao.cn

schedule.every(10).minutes.do(job)
来源：http://pas.xuetiantiany.cn

[U37] Py：读写 Excel
来源：http://acu.mhx1999.top

pandas.read_excel / DataFrame.to_excel
来源：http://kuv.xinyue.icu

[U38] Py：获取脚本所在目录
来源：http://sby.ivvv.top

Path(__file__).resolve().parent
来源：http://gjh.cheryme.top

[U39] Py：判断是否在交互环境
来源：http://tqm.yangfankeji.com

sys.stdout.isatty()
来源：http://kor.wangdashe.top

[U40] Py：打印到标准错误
来源：http://hzb.fktsv.cn

print("err", file=sys.stderr)
来源：http://acd.yonumen.top

[U41] PHP：初始化 Composer 项目
来源：http://tsq.bbcook.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://xtv.xinyue.icu

[U42] PHP：PSR-4 自动加载
来源：http://tjt.ydzc1.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tzb.jqgfzy.top

[U43] PHP：声明命名空间
来源：http://ynk.zycfv.cn

namespace App\Http;
来源：http://hcg.fktsv.cn

[U44] PHP：开启严格类型
来源：http://fos.zhaomingkeji.xyz

declare(strict_types=1);
来源：http://gyb.yanxiufei.cn

[U45] PHP：类型声明与返回类型
来源：http://akz.zdbjq.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://vno.daxiang520.top

[U46] PHP：可空类型
来源：http://wmv.bbcook.cn

?string $name = null
来源：http://boe.zdqjudy.top

[U47] PHP：联合类型
来源：http://ieu.daxiang520.top

int|string $id
来源：http://nte.nanxinkj.top

[U48] PHP：纯枚举
来源：http://xfz.jqgufenzy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://epf.zycfv.cn

[U49] PHP：只读属性
来源：http://lua.tianlin.xyz

public readonly string $name
来源：http://hub.hesvh.cn

[U50] PHP：构造器属性提升
来源：http://nnc.aibaodan.cn

public function __construct(private int $id) {}
来源：http://trs.bbcook.cn

[U51] PHP：数组解构
来源：http://vof.yvedp.cn

[$a, $b] = $arr;
来源：http://vic.chenjidiqi.icu

[U52] PHP：箭头函数
来源：http://tyk.zhixingplan.top

$double = fn($x) => $x * 2;
来源：http://eaa.quarkkingdee.top

[U53] PHP：空合并运算符
来源：http://cwe.jinyuanbaomall.cn

$v = $a ?? $b ?? "default";
来源：http://hrb.jiagoushi.top

[U54] PHP：空安全调用
来源：http://fzb.shanyushiyangtech.top

$obj?->method()
来源：http://pjv.gogol.net.cn

[U55] PHP：match 表达式
来源：http://bms.hcnkem.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://nnr.jqgufenzy.top

[U56] PHP：命名参数
来源：http://baf.tian-w.cn

f(a: 1, b: 2)
来源：http://zuo.hywenlv.cn

[U57] PHP：字符串插值
来源：http://huf.xuanzx.com

"值: {$a}"
来源：http://oyo.chenjidiqi.icu

[U58] PHP：数组三件套
来源：http://eco.guowangkeji.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qad.shangyingyoupin.top

[U59] PHP：自定义排序
来源：http://htg.snrcjt.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hyy.daxiang520.top

[U60] PHP：JSON 编解码
来源：http://jxc.gzhubu.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fic.epnwcf.com

[U61] PHP：正则
来源：http://akc.xylfe.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nzi.tarul.cn

[U62] PHP：日期对象
来源：http://ngo.hcnkem.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://efs.ydjk.org.cn

[U63] PHP：文件读写
来源：http://rzi.xylfe.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hdz.yfazqb.com

[U64] PHP：目录遍历
来源：http://rgb.aibaodan.cn

glob("dir/*.php");  scandir("dir");
来源：http://hfe.hfpthk.cn

[U65] PHP：会话
来源：http://jnm.xylfe.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://zkj.cqqwz.cn

[U66] PHP：设置 Cookie
来源：http://hgm.tianlin.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pue.zdqjudy.top

[U67] PHP：处理文件上传
来源：http://yqd.kuanghao11.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://geq.tarul.cn

[U68] PHP：PDO 连接
来源：http://hcn.316326.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rgf.birdmap.top

[U69] PHP：PDO 预处理
来源：http://zji.pengpengdd.cyou

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://tdw.snrcjt.cn

[U70] PHP：PDO 事务
来源：http://lxs.hysaishi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mdv.gotoacloud.top

[U71] PHP：抛出异常
来源：http://cgs.jianghu66.top

throw new RuntimeException("失败", 500);
来源：http://gqc.shuidangran.top

[U72] PHP：写错误日志
来源：http://aqh.hcnkem.com

error_log("失败: " . $e->getMessage());
来源：http://dfz.daria6918.cn

[U73] PHP：读取 ini 配置
来源：http://wgf.shuidangran.top

parse_ini_file("config.ini", true)
来源：http://jeb.feifeiyinyue.top

[U74] PHP：读取环境变量
来源：http://abm.nanxuanxn.top

getenv("APP_ENV") ?: "production"
来源：http://ktt.havefunace.top

[U75] PHP：依赖注入
来源：http://zug.316326.xyz

composer require psr/container
来源：http://rex.xylfe.cn

[U76] PHP：简单路由
来源：http://wpg.cashguo.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gmm.0kj1m.cn

[U77] PHP：模板渲染
来源：http://htu.ydzc1.top

composer require twig/twig
来源：http://oaf.zhixingplan.top

[U78] PHP：单元测试
来源：http://kcl.fzhhl.top

composer require --dev phpunit/phpunit
来源：http://foe.kuanghao11.cn

[U79] PHP：静态分析
来源：http://rmn.daria6918.cn

composer require --dev phpstan/phpstan
来源：http://xdh.snrcjt.cn

[U80] PHP：代码规范修复
来源：http://sls.pycfn.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://mhb.zhongyouzk.top

[U81] JS：初始化项目
来源：http://khd.iojbl.cn

npm init -y;  npm i express
来源：http://zfz.kuanghao11.cn

[U82] JS：package.json 脚本
来源：http://jeu.c1oappe.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://syq.nanxuanxn.top

[U83] JS：ES Module 导入导出
来源：http://rbs.yanxiufei.cn

export const a = 1;  import { a } from "./m.js";
来源：http://buo.hesvh.cn

[U84] JS：CommonJS 写法
来源：http://cfp.aibaodan.cn

module.exports = { a };  const { a } = require("./m");
来源：http://udq.ydzc1.top

[U85] JS：可选链
来源：http://gjr.uphjek.com

a?.b?.c
来源：http://dbc.xuetiantiany.cn

[U86] JS：空值合并
来源：http://vas.yj20258888.top

a ?? b
来源：http://arh.xylfe.cn

[U87] JS：解构默认值
来源：http://ycy.daxiang520.top

const { a = 1, b = 2 } = obj;
来源：http://ezd.xziqi.cn

[U88] JS：对象展开合并
来源：http://yqs.jinqigufen.top

{ ...a, ...b }
来源：http://idv.fehbvm.com

[U89] JS：数组去重
来源：http://vea.iojbl.cn

[...new Set(arr)]
来源：http://ast.ehwqpu.com

[U90] JS：数字数组排序
来源：http://hsp.zhengqikj.top

[...arr].sort((a, b) => a - b)
来源：http://imk.fengsongda.top

[U91] JS：对象键值遍历
来源：http://eft.gogol.net.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://elp.yj20258.top

[U92] JS：深拷贝
来源：http://gnb.vehdjk.com

structuredClone(obj)
来源：http://kai.zhiwuduotai.top

[U93] JS：模板字符串
来源：http://jyq.chenjidiqi.icu

`共 ${n} 条`
来源：http://zji.yuxming.cn

[U94] JS：箭头函数
来源：http://wey.havefunace.top

const double = x => x * 2;
来源：http://mba.c1oappe.top

[U95] JS：Promise 包装
来源：http://xwt.jianghu66.top

new Promise((resolve, reject) => {})
来源：http://jqr.chenjidiqi.icu

[U96] JS：async/await 与异常
来源：http://tyo.dashuyun.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://iyi.jyoumei.cn

[U97] JS：并发请求
来源：http://ylp.yangfankeji.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://mjo.birdmap.top

[U98] JS：fetch 带 JSON
来源：http://cxw.shangyingyoupin.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pga.hcnkem.com

[U99] JS：事件监听
来源：http://inl.cqqwz.cn

el.addEventListener("click", e => {})
来源：http://kpv.cdnleiting.top

[U100] JS：DOM 查询
来源：http://inj.epnwcf.com

document.querySelector(".item")
来源：http://kld.bbcook.cn

[U101] JS：classList 操作
来源：http://wtw.cashguo.top

el.classList.toggle("active")
来源：http://jyt.pycfn.com

[U102] JS：本地存储
来源：http://aeo.chenjidiqi.icu

localStorage.setItem("k", JSON.stringify(v))
来源：http://ukw.birdmap.top

[U103] JS：定时器
来源：http://hbc.zhiwuduotai.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zuf.fanxiaobao.xyz

[U104] JS：防抖
来源：http://dcx.havefunace.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wor.sysykeji.top

[U105] JS：节流
来源：http://ctr.chenlongwang.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gve.kuanghao11.cn

[U106] JS：日期格式化
来源：http://viy.smart0.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://opc.jqgfzy.top

[U107] JS：数字千分位
来源：http://sqa.ehwqpu.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zor.ydzc1.top

[U108] JS：随机整数
来源：http://lsp.ybcxt.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hqq.sweek.top

[U109] JS：数组分组
来源：http://lfj.shuidangran.top

Object.groupBy(arr, x => x.type)
来源：http://qzf.dashuyun.cn

[U110] JS：数组分块
来源：http://kuf.c1oappe.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vjm.sufxvd.cn

[U111] JS：对象转 Map
来源：http://wnd.jqgfzy.top

new Map(Object.entries(obj))
来源：http://iqc.ydjk.org.cn

[U112] JS：字符串补位
来源：http://dly.shzxlz.cn

"7".padStart(3, "0")
来源：http://vxw.ydzc1.top

[U113] JS：正则替换全部
来源：http://kyw.jinghuilouyu.cn

s.replaceAll("a", "b")
来源：http://qrg.birdmap.top

[U114] JS：JSON 深比较
来源：http://esd.daria6918.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ssp.jinqigufen.top

[U115] JS：生成 UUID
来源：http://fyj.jinyuanbaomall.cn

crypto.randomUUID()
来源：http://swp.nwbrower.top

[U116] JS：类型检查（JSDoc）
来源：http://plx.jiagoushi.top

/** @param {string} name */ function f(name) {}
来源：http://fbp.xuetiantiany.cn

[U117] JS：单元测试
来源：http://xds.sufxvd.cn

npm i -D vitest;  npx vitest
来源：http://vga.aizwys.cn

[U118] JS：开发服务器
来源：http://ccf.yangfankeji.com

npm i -D vite;  npx vite
来源：http://ocx.yueranfly.top

[U119] JS：生产构建
来源：http://eyh.fzhhl.top

npx vite build
来源：http://xgz.dianchejie.cn

[U120] JS：读取环境变量（Vite）
来源：http://yxy.quarkkingdee.top

import.meta.env.VITE_API_URL
来源：http://hnp.yj20258.top

================================================================================
来源：http://xdx.jiagoushi.top

统计汇总
来源：http://oev.hysaishi.cn

================================================================================
来源：http://rve.cdnleiting.top

按语言统计（条）：
来源：http://oaq.jinyuanbaomall.cn

Python ......... 252
来源：http://vzn.jianghu66.top

PHP ............ 252
来源：http://ebu.yj20258.top

JavaScript ..... 252
来源：http://xke.ivvv.top

TypeScript ..... 212
来源：http://svw.c1oappe.top

Java ........... 212
来源：http://gcm.yangfankeji.com

Go ............. 212
来源：http://ead.ctjpmb.com

Ruby ........... 212
来源：http://cqi.hnxiangtu.top

C# ............. 212
来源：http://nfc.hywenlv.cn

C .............. 30
来源：http://ygs.xuanzx.com

C++ ............ 30
来源：http://unh.fengsongda.top

SQL ............ 90
来源：http://igw.ehwqpu.com

Bash ........... 80
来源：http://ryu.zhengqikj.top

Kotlin ......... 15
来源：http://tho.zdbjq.cn

Swift .......... 15
来源：http://rxs.hongshengwenyu.top

Lua ............ 10
来源：http://gki.guowangkeji.top

Perl ........... 10
来源：http://kvx.zdqjudy.top

Scala .......... 10
来源：http://imz.havefunace.top

------------------------------------
来源：http://ipg.cashguo.top

合计 ........... 2106 条
来源：http://btd.cheryme.top

按章节统计：
来源：http://mdw.ehwqpu.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gpy.redwolf501.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://pwt.guowangkeji.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://usc.ivvv.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rkv.yuxming.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gvz.meibo888.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://kfs.jinyuanbaomall.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://gfq.vqdsnc.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://bsm.tanke756.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://cra.tanke756.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xfi.chenzaomai.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vuz.tianlin.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://sym.aibaodan.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://lpu.xziqi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ppp.aibaodan.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://sbe.yj202588.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://inb.jinqigufen.top


<!-- 参考信息 -->