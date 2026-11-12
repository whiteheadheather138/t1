代发 wailian999

[U09] Py：字典取最大值的键
来源：http://qjw.yonumen.top

max(d, key=d.get)
来源：http://ack.hysaishi.cn

[U10] Py：按值排序字典
来源：http://zey.kuanghao11.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xsw.9152youxi.cn

[U11] Py：生成器表达式
来源：http://mya.zycfv.cn

(x * 2 for x in arr)
来源：http://nqn.zycfv.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xvr.guowangkeji.top

Counter(arr).most_common(3)
来源：http://cvz.chenlongwang.top

[U13] Py：固定长度队列
来源：http://klh.nwbrower.top

deque(maxlen=10)
来源：http://xyz.chenzaomai.com

[U14] Py：分组收集到列表
来源：http://zdv.chenlongwang.top

defaultdict(list)
来源：http://prz.shangyingyoupin.top

[U15] Py：高精度计时
来源：http://yxa.tanke756.top

t = time.perf_counter()
来源：http://oly.cdnleiting.top

[U16] Py：命令行参数解析
来源：http://nlq.cucudq.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ikg.sysykeji.top

[U17] Py：初始化日志
来源：http://aip.wangdashe.top

logging.basicConfig(level=logging.INFO)
来源：http://ooo.zhixingplan.top

[U18] Py：预编译正则
来源：http://sit.ydjk.org.cn

pat = re.compile(r"\d+")
来源：http://nrn.nanxuanxn.top

[U19] Py：正则替换带回调
来源：http://wny.quarkkingdee.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tho.sysykeji.top

[U20] Py：缓存函数结果
来源：http://giy.tanke756.top

@functools.lru_cache(maxsize=None)
来源：http://mwq.snrcjt.cn

[U21] Py：自定义上下文管理器
来源：http://ogs.ydzc1.top

@contextlib.contextmanager
来源：http://poc.zycfv.cn

[U22] Py：矩阵转置
来源：http://xyy.ehwqpu.com

list(zip(*m))
来源：http://muy.hywenlv.cn

[U23] Py：分块读取大文件
来源：http://hoy.gzhubu.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://yaz.yvedp.cn

[U24] Py：路径操作
来源：http://sdp.ivvv.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vvz.jinqigufen.top

[U25] Py：CSV 按字典读
来源：http://hhd.fehbvm.com

csv.DictReader(f)
来源：http://jcg.jyoumei.cn

[U26] Py：并发下载
来源：http://rat.fanxiaobao.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qlz.hesvh.cn

[U27] Py：异步 HTTP
来源：http://uni.tarul.cn

aiohttp.ClientSession() 配合 async with
来源：http://jzt.vehdjk.com

[U28] Py：类型别名
来源：http://xaq.ybcxt.top

UserId = int
来源：http://lsu.redwolf501.top

[U29] Py：属性校验
来源：http://oif.zdqjudy.top

@property 与 @x.setter 配合
来源：http://drm.aizwys.cn

[U30] Py：数据类
来源：http://uxn.bjfxy.top

@dataclass(slots=True)
来源：http://uin.cucudq.cn

[U31] Py：单测
来源：http://epg.hammf.cn

python -m pytest -q
来源：http://gyg.shanyushiyangkeji.top

[U32] Py：代码格式化
来源：http://rge.jyoumei.cn

ruff format . && ruff check --fix .
来源：http://drb.meibo888.top

[U33] Py：打包发布
来源：http://bll.fehbvm.com

python -m build  （依赖 pyproject.toml）
来源：http://cjk.chenzaomai.com

[U34] Py：判断编码
来源：http://kdi.jqgfzy.top

chardet.detect(raw)
来源：http://dcv.havefunace.top

[U35] Py：发送邮件
来源：http://roy.yfazqb.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gim.shanyushiyangtech.top

[U36] Py：定时任务
来源：http://gie.vehdjk.com

schedule.every(10).minutes.do(job)
来源：http://ohc.sweek.top

[U37] Py：读写 Excel
来源：http://nqn.snrcjt.cn

pandas.read_excel / DataFrame.to_excel
来源：http://jic.ppjwa.cn

[U38] Py：获取脚本所在目录
来源：http://yft.316326.xyz

Path(__file__).resolve().parent
来源：http://qbn.shanyushiyangtech.top

[U39] Py：判断是否在交互环境
来源：http://ipa.xuanzx.com

sys.stdout.isatty()
来源：http://ooh.birdmap.top

[U40] Py：打印到标准错误
来源：http://khj.feifeiyinyue.top

print("err", file=sys.stderr)
来源：http://tmk.fehbvm.com

[U41] PHP：初始化 Composer 项目
来源：http://jnc.shzxlz.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://pbc.yueranfly.top

[U42] PHP：PSR-4 自动加载
来源：http://vlm.dashuyun.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ukp.jianghu66.top

[U43] PHP：声明命名空间
来源：http://imo.smart0.xyz

namespace App\Http;
来源：http://ykb.fengsongda.top

[U44] PHP：开启严格类型
来源：http://bnp.iojbl.cn

declare(strict_types=1);
来源：http://uce.ybcxt.top

[U45] PHP：类型声明与返回类型
来源：http://oor.fengsongda.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ulu.xziqi.cn

[U46] PHP：可空类型
来源：http://rka.ydzc1.top

?string $name = null
来源：http://gma.ydzc1.top

[U47] PHP：联合类型
来源：http://fkg.yj20258.top

int|string $id
来源：http://ycc.ydzc1.top

[U48] PHP：纯枚举
来源：http://wvk.kuanghao11.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://koa.cdnleiting.top

[U49] PHP：只读属性
来源：http://wnb.xuetiantiany.cn

public readonly string $name
来源：http://jyt.nwbrower.top

[U50] PHP：构造器属性提升
来源：http://pve.zhongyouzk.top

public function __construct(private int $id) {}
来源：http://gme.iojbl.cn

[U51] PHP：数组解构
来源：http://yxo.pengpengdd.cyou

[$a, $b] = $arr;
来源：http://yum.haohaochexian.top

[U52] PHP：箭头函数
来源：http://scl.guowangkeji.top

$double = fn($x) => $x * 2;
来源：http://hyh.daria6918.cn

[U53] PHP：空合并运算符
来源：http://its.sweek.top

$v = $a ?? $b ?? "default";
来源：http://euh.yueranfly.top

[U54] PHP：空安全调用
来源：http://pbf.guowangkeji.top

$obj?->method()
来源：http://uyk.yj20258888.top

[U55] PHP：match 表达式
来源：http://scj.tanke756.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kco.cucudq.cn

[U56] PHP：命名参数
来源：http://lug.yueranfly.top

f(a: 1, b: 2)
来源：http://mfh.vehdjk.com

[U57] PHP：字符串插值
来源：http://sok.guannengcc.top

"值: {$a}"
来源：http://dbp.jiagoushi.top

[U58] PHP：数组三件套
来源：http://dei.aibaodan.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pez.chenlongwang.top

[U59] PHP：自定义排序
来源：http://zxr.shuidangran.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ven.feifeiyinyue.top

[U60] PHP：JSON 编解码
来源：http://dmo.yonumen.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cbg.gzhubu.top

[U61] PHP：正则
来源：http://sxx.xuetiantiany.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ewh.jinghuilouyu.cn

[U62] PHP：日期对象
来源：http://spf.tarul.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nij.jlsjyb.cn

[U63] PHP：文件读写
来源：http://zye.zhengqikj.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ehp.jlsjyb.cn

[U64] PHP：目录遍历
来源：http://fka.hammf.cn

glob("dir/*.php");  scandir("dir");
来源：http://lap.cheryme.top

[U65] PHP：会话
来源：http://frm.daria6918.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://sri.pycfn.com

[U66] PHP：设置 Cookie
来源：http://wgd.hongshengwenyu.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://yzi.xziqi.cn

[U67] PHP：处理文件上传
来源：http://dia.dashuyun.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://oxb.gogol.net.cn

[U68] PHP：PDO 连接
来源：http://lhq.havefunace.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mta.hnxiangtu.top

[U69] PHP：PDO 预处理
来源：http://xij.uphjek.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fxj.hfpthk.cn

[U70] PHP：PDO 事务
来源：http://lwh.hnqzz.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vqr.tianlin.xyz

[U71] PHP：抛出异常
来源：http://poa.ydjk.org.cn

throw new RuntimeException("失败", 500);
来源：http://jlk.shuidangran.top

[U72] PHP：写错误日志
来源：http://avc.iojbl.cn

error_log("失败: " . $e->getMessage());
来源：http://uin.316326.xyz

[U73] PHP：读取 ini 配置
来源：http://qae.sufxvd.cn

parse_ini_file("config.ini", true)
来源：http://gqn.zdbjq.cn

[U74] PHP：读取环境变量
来源：http://mzn.jlsjyb.cn

getenv("APP_ENV") ?: "production"
来源：http://dck.yonumen.top

[U75] PHP：依赖注入
来源：http://icb.guannengcc.top

composer require psr/container
来源：http://oxa.sweek.top

[U76] PHP：简单路由
来源：http://vnu.aizwys.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://nkx.yangfankeji.com

[U77] PHP：模板渲染
来源：http://vck.jlsjyb.cn

composer require twig/twig
来源：http://qyw.xinyue.icu

[U78] PHP：单元测试
来源：http://xjc.haohaochexian.top

composer require --dev phpunit/phpunit
来源：http://joy.iojbl.cn

[U79] PHP：静态分析
来源：http://uug.c1oappe.top

composer require --dev phpstan/phpstan
来源：http://ghb.pycfn.com

[U80] PHP：代码规范修复
来源：http://iec.smart0.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://swh.yonumen.top

[U81] JS：初始化项目
来源：http://jiz.xuanzx.com

npm init -y;  npm i express
来源：http://ovo.gaohongyu789.top

[U82] JS：package.json 脚本
来源：http://hub.tarul.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zyo.hcnkem.com

[U83] JS：ES Module 导入导出
来源：http://wfk.jianghu66.top

export const a = 1;  import { a } from "./m.js";
来源：http://aav.zycfv.cn

[U84] JS：CommonJS 写法
来源：http://anp.zdbjq.cn

module.exports = { a };  const { a } = require("./m");
来源：http://zsv.jinqigfzy.top

[U85] JS：可选链
来源：http://ama.jinghuilouyu.cn

a?.b?.c
来源：http://pdz.hammf.cn

[U86] JS：空值合并
来源：http://jrg.vehdjk.com

a ?? b
来源：http://iys.jinqigufen.top

[U87] JS：解构默认值
来源：http://nxq.ppjwa.cn

const { a = 1, b = 2 } = obj;
来源：http://jgf.hesvh.cn

[U88] JS：对象展开合并
来源：http://qyd.tianlin.xyz

{ ...a, ...b }
来源：http://kxz.guannengcc.top

[U89] JS：数组去重
来源：http://vsb.mhx1999.top

[...new Set(arr)]
来源：http://qqx.gogol.net.cn

[U90] JS：数字数组排序
来源：http://qwx.fehbvm.com

[...arr].sort((a, b) => a - b)
来源：http://diw.smart0.xyz

[U91] JS：对象键值遍历
来源：http://mtz.cashguo.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ber.hammf.cn

[U92] JS：深拷贝
来源：http://fjn.ydzc1.top

structuredClone(obj)
来源：http://rsu.hywenlv.cn

[U93] JS：模板字符串
来源：http://gfc.jinyuanbaomall.cn

`共 ${n} 条`
来源：http://zxz.xziqi.cn

[U94] JS：箭头函数
来源：http://dnf.9152youxi.cn

const double = x => x * 2;
来源：http://xhc.zhiwuduotai.top

[U95] JS：Promise 包装
来源：http://cla.yvedp.cn

new Promise((resolve, reject) => {})
来源：http://urg.0kj1m.cn

[U96] JS：async/await 与异常
来源：http://hkn.hfpthk.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vyh.vehdjk.com

[U97] JS：并发请求
来源：http://xxw.cucudq.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://wjv.yonumen.top

[U98] JS：fetch 带 JSON
来源：http://xab.fanxiaobao.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://onh.cheryme.top

[U99] JS：事件监听
来源：http://jky.zhengqikj.top

el.addEventListener("click", e => {})
来源：http://avm.wangshuangyany.cn

[U100] JS：DOM 查询
来源：http://wlm.fengsongda.top

document.querySelector(".item")
来源：http://jlp.smart0.xyz

[U101] JS：classList 操作
来源：http://fgf.aizwys.cn

el.classList.toggle("active")
来源：http://alq.zhixingplan.top

[U102] JS：本地存储
来源：http://dqn.haohaochexian.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://yzk.cqqwz.cn

[U103] JS：定时器
来源：http://mfc.tanke756.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ncw.hongshengwenyu.top

[U104] JS：防抖
来源：http://ery.zhaomingkeji.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uvy.wangdashe.top

[U105] JS：节流
来源：http://put.jqgufenzy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zti.ydjk.org.cn

[U106] JS：日期格式化
来源：http://hsz.52xcode.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qrv.yangfankeji.com

[U107] JS：数字千分位
来源：http://vyn.ywan-chungtsiang.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://aos.wangdashe.top

[U108] JS：随机整数
来源：http://izb.9152youxi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nfn.52xcode.cn

[U109] JS：数组分组
来源：http://clb.hywenlv.cn

Object.groupBy(arr, x => x.type)
来源：http://pne.yonumen.top

[U110] JS：数组分块
来源：http://bpy.quarkkingdee.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pjs.fzhhl.top

[U111] JS：对象转 Map
来源：http://iyo.cqqwz.cn

new Map(Object.entries(obj))
来源：http://sly.sysykeji.top

[U112] JS：字符串补位
来源：http://agq.hfpthk.cn

"7".padStart(3, "0")
来源：http://omv.yuanzhike.top

[U113] JS：正则替换全部
来源：http://dtj.jyoumei.cn

s.replaceAll("a", "b")
来源：http://xra.jinqigfzy.top

[U114] JS：JSON 深比较
来源：http://mrw.nwbrower.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://hcy.ctjpmb.com

[U115] JS：生成 UUID
来源：http://rai.chenzaomai.com

crypto.randomUUID()
来源：http://adk.shanyushiyangkeji.top

[U116] JS：类型检查（JSDoc）
来源：http://pgr.jyoumei.cn

/** @param {string} name */ function f(name) {}
来源：http://ffq.shangyingyoupin.top

[U117] JS：单元测试
来源：http://buw.jyoumei.cn

npm i -D vitest;  npx vitest
来源：http://coi.snrcjt.cn

[U118] JS：开发服务器
来源：http://zht.redwolf501.top

npm i -D vite;  npx vite
来源：http://zvu.redwolf501.top

[U119] JS：生产构建
来源：http://zvv.ppjwa.cn

npx vite build
来源：http://sxf.shuidangran.top

[U120] JS：读取环境变量（Vite）
来源：http://gks.jianghu66.top

import.meta.env.VITE_API_URL
来源：http://aqp.sysykeji.top

================================================================================
来源：http://hsl.jinghuilouyu.cn

统计汇总
来源：http://ozc.hywenlv.cn

================================================================================
来源：http://cjp.jqgufenzy.top

按语言统计（条）：
来源：http://ead.mhx1999.top

Python ......... 252
来源：http://rwb.yuanzhike.top

PHP ............ 252
来源：http://dbx.zhengqikj.top

JavaScript ..... 252
来源：http://vqd.nanxinkj.top

TypeScript ..... 212
来源：http://vru.jinqigfzy.top

Java ........... 212
来源：http://dlp.shanyushiyangtech.top

Go ............. 212
来源：http://egh.shuidangran.top

Ruby ........... 212
来源：http://mzm.9152youxi.cn

C# ............. 212
来源：http://zaw.shzxlz.cn

C .............. 30
来源：http://uqn.zycfv.cn

C++ ............ 30
来源：http://snb.yongpay.top

SQL ............ 90
来源：http://xdf.shanyushiyangkeji.top

Bash ........... 80
来源：http://ftp.ydzc1.top

Kotlin ......... 15
来源：http://gcs.yuxming.cn

Swift .......... 15
来源：http://osz.smart0.xyz

Lua ............ 10
来源：http://sfg.pengpengdd.cyou

Perl ........... 10
来源：http://oyz.jyoumei.cn

Scala .......... 10
来源：http://urp.havefunace.top

------------------------------------
来源：http://fpi.jqgfzy.top

合计 ........... 2106 条
来源：http://fqx.fehbvm.com

按章节统计：
来源：http://cvn.hysaishi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qip.kuanghao11.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qrh.dashuyun.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://prs.vqdsnc.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://jrm.dashuyun.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qqu.52xcode.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xqu.ppjwa.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zwu.jiagoushi.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nfv.yangfankeji.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://dzw.zhixingplan.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mqe.yj20258.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jhs.shanyushiyangkeji.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://tzj.yj20258888.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wro.dianchejie.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wjc.hywenlv.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://lus.xingfuxueyuan.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bkg.aizwys.cn

Q SQL 专题                              90
来源：http://osx.tianlin.xyz

R Bash 专题                             80
来源：http://vds.epnwcf.com

S C / C++ 专题                          60
来源：http://dfl.zhixingplan.top

T 其他语言补充                          60
来源：http://wrq.sxryk.cn

U 高频实用片段                         120
来源：http://hot.ppjwa.cn

------------------------------------
来源：http://hus.nanxinkj.top

合计                                  2106 条
来源：http://sdi.havefunace.top

--------------------------------------------------------------------------------
来源：http://qic.nwbrower.top

使用提醒
来源：http://qyq.shzxlz.cn

--------------------------------------------------------------------------------
来源：http://liq.hammf.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ydc.dashuyun.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://aaf.iojbl.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ear.jianghu66.top

在旧版本上使用前请先确认语法支持情况。
来源：http://yal.fehbvm.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://vsu.zycfv.cn

—— 文件结束 ——
来源：http://dro.xuetiantiany.cn

================================================================================
来源：http://mnb.gzhubu.top

程序语言常见例子速查手册（2024 版）
来源：http://tde.fehbvm.com

Common Programming Examples Cheat Book
来源：http://wqp.zhaomingkeji.xyz

================================================================================
来源：http://pll.dianchejie.cn

【收录内容】
来源：http://gbk.yuxming.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://dsb.yj20258888.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://rql.havefunace.top

SQL · Bash · C · C++
来源：http://qyy.havefunace.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://gqf.meibo888.top

【使用说明】
来源：http://gba.cashguo.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://bra.chenjidiqi.icu

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wvk.jinqigfzy.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://lph.zhijiandao.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qrz.cqqwz.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://bap.xuanzx.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hnf.shzxlz.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://jwq.kuanghao11.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jsy.shangyingyoupin.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://uzg.bbcook.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wgi.zhiwuduotai.top


<!-- 参考信息 -->