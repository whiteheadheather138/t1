代发 wailian999

[U09] Py：字典取最大值的键
来源：http://prf.haohaochexian.top

max(d, key=d.get)
来源：http://eqp.hfpthk.cn

[U10] Py：按值排序字典
来源：http://jaa.chenlongwang.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ymx.zhoulong.xyz

[U11] Py：生成器表达式
来源：http://yfs.hnqzz.top

(x * 2 for x in arr)
来源：http://bjg.daxiang520.top

[U12] Py：取出现最多的 3 个元素
来源：http://huq.sufxvd.cn

Counter(arr).most_common(3)
来源：http://ihe.fehbvm.com

[U13] Py：固定长度队列
来源：http://hso.jyoumei.cn

deque(maxlen=10)
来源：http://prk.ivvv.top

[U14] Py：分组收集到列表
来源：http://fwb.yvedp.cn

defaultdict(list)
来源：http://kgk.shanyushiyangtech.top

[U15] Py：高精度计时
来源：http://zat.daxiang520.top

t = time.perf_counter()
来源：http://vsf.gzhubu.top

[U16] Py：命令行参数解析
来源：http://xee.chenzaomai.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nmm.jinghuilouyu.cn

[U17] Py：初始化日志
来源：http://tyy.svipenyu.cn

logging.basicConfig(level=logging.INFO)
来源：http://xed.hesvh.cn

[U18] Py：预编译正则
来源：http://xwt.haohaochexian.top

pat = re.compile(r"\d+")
来源：http://ocy.hfpthk.cn

[U19] Py：正则替换带回调
来源：http://tce.xuetiantiany.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yjl.ctjpmb.com

[U20] Py：缓存函数结果
来源：http://dkk.fzhhl.top

@functools.lru_cache(maxsize=None)
来源：http://vyq.guannengcc.top

[U21] Py：自定义上下文管理器
来源：http://ovg.zhijiandao.cn

@contextlib.contextmanager
来源：http://ikb.c1oappe.top

[U22] Py：矩阵转置
来源：http://cnt.9152youxi.cn

list(zip(*m))
来源：http://sok.yvedp.cn

[U23] Py：分块读取大文件
来源：http://ero.hywenlv.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://alv.ydzc1.top

[U24] Py：路径操作
来源：http://kof.fzhhl.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://njm.svipenyu.cn

[U25] Py：CSV 按字典读
来源：http://ttk.xingfuxueyuan.xyz

csv.DictReader(f)
来源：http://rxt.sjlbkw.cn

[U26] Py：并发下载
来源：http://kcq.hywenlv.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zmv.uphjek.com

[U27] Py：异步 HTTP
来源：http://rrd.tianlin.xyz

aiohttp.ClientSession() 配合 async with
来源：http://jdd.cdnleiting.top

[U28] Py：类型别名
来源：http://qrf.daria6918.cn

UserId = int
来源：http://nin.jlsjyb.cn

[U29] Py：属性校验
来源：http://atv.fktsv.cn

@property 与 @x.setter 配合
来源：http://aay.hesvh.cn

[U30] Py：数据类
来源：http://rgw.chenzaomai.com

@dataclass(slots=True)
来源：http://chk.tanke756.top

[U31] Py：单测
来源：http://rgo.zhengqikj.top

python -m pytest -q
来源：http://qrf.shanyushiyangtech.top

[U32] Py：代码格式化
来源：http://rwi.hcnkem.com

ruff format . && ruff check --fix .
来源：http://iqq.xinyue.icu

[U33] Py：打包发布
来源：http://fok.ehwqpu.com

python -m build  （依赖 pyproject.toml）
来源：http://ccr.yj20258.top

[U34] Py：判断编码
来源：http://cjn.shanyushiyangtech.top

chardet.detect(raw)
来源：http://jye.nanxinkj.top

[U35] Py：发送邮件
来源：http://czn.jlsjyb.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mcc.xuanzx.com

[U36] Py：定时任务
来源：http://jsx.hammf.cn

schedule.every(10).minutes.do(job)
来源：http://jta.yj20258888.top

[U37] Py：读写 Excel
来源：http://gak.iojbl.cn

pandas.read_excel / DataFrame.to_excel
来源：http://igm.mhx1999.top

[U38] Py：获取脚本所在目录
来源：http://vdz.yj202588.top

Path(__file__).resolve().parent
来源：http://itf.yueranfly.top

[U39] Py：判断是否在交互环境
来源：http://sts.yuanzhike.top

sys.stdout.isatty()
来源：http://puy.jianghu66.top

[U40] Py：打印到标准错误
来源：http://uyw.meibo888.top

print("err", file=sys.stderr)
来源：http://jii.bbcook.cn

[U41] PHP：初始化 Composer 项目
来源：http://bqv.wangdashe.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ina.vqdsnc.cn

[U42] PHP：PSR-4 自动加载
来源：http://hkm.fanxiaobao.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jaa.nwbrower.top

[U43] PHP：声明命名空间
来源：http://lcc.jinqigfzy.top

namespace App\Http;
来源：http://oar.meibo888.top

[U44] PHP：开启严格类型
来源：http://pke.quarkkingdee.top

declare(strict_types=1);
来源：http://tqc.yfazqb.com

[U45] PHP：类型声明与返回类型
来源：http://yiu.havefunace.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://zuj.bjfxy.top

[U46] PHP：可空类型
来源：http://ihx.tarul.cn

?string $name = null
来源：http://jlk.52xcode.cn

[U47] PHP：联合类型
来源：http://ebz.shanyushiyangkeji.top

int|string $id
来源：http://rum.hnxiangtu.top

[U48] PHP：纯枚举
来源：http://ihz.kuanghao11.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ysl.cashguo.top

[U49] PHP：只读属性
来源：http://lkh.zhoulong.xyz

public readonly string $name
来源：http://fsh.zdbjq.cn

[U50] PHP：构造器属性提升
来源：http://fpy.jianghu66.top

public function __construct(private int $id) {}
来源：http://jah.chenjidiqi.icu

[U51] PHP：数组解构
来源：http://kxh.ctjpmb.com

[$a, $b] = $arr;
来源：http://slu.zhaomingkeji.xyz

[U52] PHP：箭头函数
来源：http://bic.yvedp.cn

$double = fn($x) => $x * 2;
来源：http://bfr.redwolf501.top

[U53] PHP：空合并运算符
来源：http://dzx.tianlin.xyz

$v = $a ?? $b ?? "default";
来源：http://vmm.shuidangran.top

[U54] PHP：空安全调用
来源：http://jks.fzhhl.top

$obj?->method()
来源：http://vqi.ivvv.top

[U55] PHP：match 表达式
来源：http://nvz.yongpay.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bfa.meibo888.top

[U56] PHP：命名参数
来源：http://itk.gaohongyu789.top

f(a: 1, b: 2)
来源：http://qxg.fanxiaobao.xyz

[U57] PHP：字符串插值
来源：http://mpq.yj202588.top

"值: {$a}"
来源：http://dxo.yj20258.top

[U58] PHP：数组三件套
来源：http://oaq.vqdsnc.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://krz.yonumen.top

[U59] PHP：自定义排序
来源：http://cil.zhoulong.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://eym.jlsjyb.cn

[U60] PHP：JSON 编解码
来源：http://qyn.vehdjk.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jdy.yj202588.top

[U61] PHP：正则
来源：http://uqv.dianchejie.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hpi.dashuyun.cn

[U62] PHP：日期对象
来源：http://mwf.hysaishi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nuo.hywenlv.cn

[U63] PHP：文件读写
来源：http://ill.tian-w.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://woh.nanxinkj.top

[U64] PHP：目录遍历
来源：http://fbh.fengsongda.top

glob("dir/*.php");  scandir("dir");
来源：http://orh.gogol.net.cn

[U65] PHP：会话
来源：http://zsv.ivvv.top

session_start();  $_SESSION["uid"] = 1;
来源：http://zui.hywenlv.cn

[U66] PHP：设置 Cookie
来源：http://auc.meibo888.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fqp.meibo888.top

[U67] PHP：处理文件上传
来源：http://lpt.shanyushiyangtech.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gol.svipenyu.cn

[U68] PHP：PDO 连接
来源：http://ftc.yuanzhike.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vwa.xingfuxueyuan.xyz

[U69] PHP：PDO 预处理
来源：http://mej.yangfankeji.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xxi.gaohongyu789.top

[U70] PHP：PDO 事务
来源：http://rtn.hesvh.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://whr.shanyushiyangkeji.top

[U71] PHP：抛出异常
来源：http://uos.xylfe.cn

throw new RuntimeException("失败", 500);
来源：http://ywu.jinghuilouyu.cn

[U72] PHP：写错误日志
来源：http://pwv.sjlbkw.cn

error_log("失败: " . $e->getMessage());
来源：http://hmj.zhongyouzk.top

[U73] PHP：读取 ini 配置
来源：http://ama.gzhubu.top

parse_ini_file("config.ini", true)
来源：http://xno.pycfn.com

[U74] PHP：读取环境变量
来源：http://mie.jlsjyb.cn

getenv("APP_ENV") ?: "production"
来源：http://tlp.jyoumei.cn

[U75] PHP：依赖注入
来源：http://gxg.shzxlz.cn

composer require psr/container
来源：http://kts.ctjpmb.com

[U76] PHP：简单路由
来源：http://oca.tarul.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://sab.jqgfzy.top

[U77] PHP：模板渲染
来源：http://hvx.yj20258.top

composer require twig/twig
来源：http://bgu.zdqjudy.top

[U78] PHP：单元测试
来源：http://tqz.epnwcf.com

composer require --dev phpunit/phpunit
来源：http://ibg.xylfe.cn

[U79] PHP：静态分析
来源：http://dou.wangdashe.top

composer require --dev phpstan/phpstan
来源：http://gxo.shuidangran.top

[U80] PHP：代码规范修复
来源：http://gwu.yuxming.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://gbh.sysykeji.top

[U81] JS：初始化项目
来源：http://hxe.yj20258888.top

npm init -y;  npm i express
来源：http://hzu.zhaomingkeji.xyz

[U82] JS：package.json 脚本
来源：http://jlj.yuanzhike.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://thj.dianchejie.cn

[U83] JS：ES Module 导入导出
来源：http://lpk.hnxiangtu.top

export const a = 1;  import { a } from "./m.js";
来源：http://ggg.jqgufenzy.top

[U84] JS：CommonJS 写法
来源：http://nmr.jinqigfzy.top

module.exports = { a };  const { a } = require("./m");
来源：http://vun.shzxlz.cn

[U85] JS：可选链
来源：http://jno.aizwys.cn

a?.b?.c
来源：http://vyv.tarul.cn

[U86] JS：空值合并
来源：http://xrs.xuanzx.com

a ?? b
来源：http://jwj.xingfuxueyuan.xyz

[U87] JS：解构默认值
来源：http://ude.epnwcf.com

const { a = 1, b = 2 } = obj;
来源：http://wlr.fzhhl.top

[U88] JS：对象展开合并
来源：http://lln.yuxming.cn

{ ...a, ...b }
来源：http://vni.cucudq.cn

[U89] JS：数组去重
来源：http://mmq.ywan-chungtsiang.top

[...new Set(arr)]
来源：http://smy.tianlin.xyz

[U90] JS：数字数组排序
来源：http://zdc.zhengqikj.top

[...arr].sort((a, b) => a - b)
来源：http://lzm.jlsjyb.cn

[U91] JS：对象键值遍历
来源：http://qck.sjlbkw.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kcr.ivvv.top

[U92] JS：深拷贝
来源：http://ozi.ydjk.org.cn

structuredClone(obj)
来源：http://spv.bjfxy.top

[U93] JS：模板字符串
来源：http://ftw.zhaomingkeji.xyz

`共 ${n} 条`
来源：http://cms.hammf.cn

[U94] JS：箭头函数
来源：http://oks.c1oappe.top

const double = x => x * 2;
来源：http://hur.mhx1999.top

[U95] JS：Promise 包装
来源：http://hdn.mhx1999.top

new Promise((resolve, reject) => {})
来源：http://cxn.xziqi.cn

[U96] JS：async/await 与异常
来源：http://dtm.nanxinkj.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://elk.cashguo.top

[U97] JS：并发请求
来源：http://aht.sysykeji.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://sim.9152youxi.cn

[U98] JS：fetch 带 JSON
来源：http://udp.hongshengwenyu.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jhb.chenlongwang.top

[U99] JS：事件监听
来源：http://nva.jinyuanbaomall.cn

el.addEventListener("click", e => {})
来源：http://fcr.fanxiaobao.xyz

[U100] JS：DOM 查询
来源：http://evm.meibo888.top

document.querySelector(".item")
来源：http://wjp.yfazqb.com

[U101] JS：classList 操作
来源：http://mvv.zdqjudy.top

el.classList.toggle("active")
来源：http://vnu.hongshengwenyu.top

[U102] JS：本地存储
来源：http://pek.cqqwz.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://lsk.jinqigufen.top

[U103] JS：定时器
来源：http://eqm.svipenyu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ogp.hnxiangtu.top

[U104] JS：防抖
来源：http://htj.aibaodan.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qiz.hywenlv.cn

[U105] JS：节流
来源：http://tai.uphjek.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gze.quarkkingdee.top

[U106] JS：日期格式化
来源：http://fno.9152youxi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xib.hongshengwenyu.top

[U107] JS：数字千分位
来源：http://piq.xuanzx.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ojs.yongpay.top

[U108] JS：随机整数
来源：http://wkd.birdmap.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ehi.yuxming.cn

[U109] JS：数组分组
来源：http://knn.aibaodan.cn

Object.groupBy(arr, x => x.type)
来源：http://mng.hywenlv.cn

[U110] JS：数组分块
来源：http://sol.yongpay.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cwy.gotoacloud.top

[U111] JS：对象转 Map
来源：http://ews.xylfe.cn

new Map(Object.entries(obj))
来源：http://yed.feifeiyinyue.top

[U112] JS：字符串补位
来源：http://oav.aibaodan.cn

"7".padStart(3, "0")
来源：http://wjl.zycfv.cn

[U113] JS：正则替换全部
来源：http://oui.jqgfzy.top

s.replaceAll("a", "b")
来源：http://xnu.aizwys.cn

[U114] JS：JSON 深比较
来源：http://xia.hammf.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://jyj.quarkkingdee.top

[U115] JS：生成 UUID
来源：http://ont.yfazqb.com

crypto.randomUUID()
来源：http://vsf.ctjpmb.com

[U116] JS：类型检查（JSDoc）
来源：http://lmj.epnwcf.com

/** @param {string} name */ function f(name) {}
来源：http://pio.fanxiaobao.xyz

[U117] JS：单元测试
来源：http://bfk.xuanzx.com

npm i -D vitest;  npx vitest
来源：http://enf.redwolf501.top

[U118] JS：开发服务器
来源：http://hqn.aibaodan.cn

npm i -D vite;  npx vite
来源：http://wqn.jianghu66.top

[U119] JS：生产构建
来源：http://sog.hongshengwenyu.top

npx vite build
来源：http://mxj.9152youxi.cn

[U120] JS：读取环境变量（Vite）
来源：http://vyr.hnqzz.top

import.meta.env.VITE_API_URL
来源：http://alc.zhixingplan.top

================================================================================
来源：http://rns.hnqzz.top

统计汇总
来源：http://tan.jlsjyb.cn

================================================================================
来源：http://ejk.zdqjudy.top

按语言统计（条）：
来源：http://ctn.birdmap.top

Python ......... 252
来源：http://myl.gogol.net.cn

PHP ............ 252
来源：http://moe.zhaomingkeji.xyz

JavaScript ..... 252
来源：http://cyh.xylfe.cn

TypeScript ..... 212
来源：http://niu.nwbrower.top

Java ........... 212
来源：http://qza.sysykeji.top

Go ............. 212
来源：http://ruk.aizwys.cn

Ruby ........... 212
来源：http://xws.ivvv.top

C# ............. 212
来源：http://nwe.andypj.xyz

C .............. 30
来源：http://eai.yj202588.top

C++ ............ 30
来源：http://gcm.tianlin.xyz

SQL ............ 90
来源：http://fed.sxryk.cn

Bash ........... 80
来源：http://nff.zhijiandao.cn

Kotlin ......... 15
来源：http://kih.shzxlz.cn

Swift .......... 15
来源：http://pfh.zhoulong.xyz

Lua ............ 10
来源：http://fdq.guannengcc.top

Perl ........... 10
来源：http://drf.jinyuanbaomall.cn

Scala .......... 10
来源：http://hwf.wangshuangyany.cn

------------------------------------
来源：http://ufk.yfazqb.com

合计 ........... 2106 条
来源：http://prm.chenlongwang.top

按章节统计：
来源：http://uih.yj20258888.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ccp.dianchejie.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://vhw.havefunace.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://acw.zhongyouzk.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vfo.52xcode.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://evy.aizwys.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vav.chenzaomai.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ces.zhijiandao.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jdv.mhx1999.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://esw.zhijiandao.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ctm.tarul.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rql.ehwqpu.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dve.tarul.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kwp.wangshuangyany.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://iat.shanyushiyangkeji.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://esy.iojbl.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://axe.zdqjudy.top

Q SQL 专题                              90
来源：http://aqr.gogol.net.cn

R Bash 专题                             80
来源：http://ydx.dashuyun.cn

S C / C++ 专题                          60
来源：http://fcv.aizwys.cn

T 其他语言补充                          60
来源：http://pwv.yj202588.top

U 高频实用片段                         120
来源：http://zjy.haohaochexian.top

------------------------------------
来源：http://pup.cdnleiting.top

合计                                  2106 条
来源：http://kla.zhoulong.xyz

--------------------------------------------------------------------------------
来源：http://suy.yanxiufei.cn

使用提醒
来源：http://ejp.chenjidiqi.icu

--------------------------------------------------------------------------------
来源：http://tdb.52xcode.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://lif.chenzaomai.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blg.fehbvm.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qzi.xylfe.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://mmu.fktsv.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://isd.52xcode.cn

—— 文件结束 ——
来源：http://rry.tarul.cn

================================================================================
来源：http://emf.wangdashe.top

程序语言常见例子速查手册（2024 版）
来源：http://gxa.feifeiyinyue.top

Common Programming Examples Cheat Book
来源：http://ytz.dianchejie.cn

================================================================================
来源：http://yjo.haohaochexian.top

【收录内容】
来源：http://wju.ydjk.org.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://cdg.haohaochexian.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://qiu.jinqigufen.top

SQL · Bash · C · C++
来源：http://eim.zhaomingkeji.xyz

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://bmm.tanke756.top

【使用说明】
来源：http://vxd.aibaodan.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vnv.ctjpmb.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://tub.ybcxt.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://cxv.sjlbkw.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://xjw.chenzaomai.com

Bash:  Shell         C:     C             C++:   C++
来源：http://rgr.xziqi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://yiu.cucudq.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://dxq.ydzc1.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vzt.ybcxt.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lav.snrcjt.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pfv.aizwys.cn


<!-- 参考信息 -->