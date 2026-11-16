代发 wailian999

[U07] Py：反转字典键值
来源：http://dww.zhijiandao.cn

{v: k for k, v in d.items()}
来源：http://xhx.xinyue.icu

[U08] Py：展平二维列表
来源：http://kxv.ydjk.org.cn

[y for x in nested for y in x]
来源：http://njx.hywenlv.cn

[U09] Py：字典取最大值的键
来源：http://xbe.xinyue.icu

max(d, key=d.get)
来源：http://kab.yuxming.cn

[U10] Py：按值排序字典
来源：http://frj.vqdsnc.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://azs.c1oappe.top

[U11] Py：生成器表达式
来源：http://kvp.yj202588.top

(x * 2 for x in arr)
来源：http://wwm.xuanzx.com

[U12] Py：取出现最多的 3 个元素
来源：http://kob.uphjek.com

Counter(arr).most_common(3)
来源：http://kuz.xinyue.icu

[U13] Py：固定长度队列
来源：http://ujt.cqqwz.cn

deque(maxlen=10)
来源：http://fcd.pycfn.com

[U14] Py：分组收集到列表
来源：http://bfy.jinqigfzy.top

defaultdict(list)
来源：http://uaw.hnxiangtu.top

[U15] Py：高精度计时
来源：http://nsd.shzxlz.cn

t = time.perf_counter()
来源：http://epc.tarul.cn

[U16] Py：命令行参数解析
来源：http://iyk.dashuyun.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ukk.fengsongda.top

[U17] Py：初始化日志
来源：http://mqf.sysykeji.top

logging.basicConfig(level=logging.INFO)
来源：http://jna.sweek.top

[U18] Py：预编译正则
来源：http://lax.tianlin.xyz

pat = re.compile(r"\d+")
来源：http://qdz.fengsongda.top

[U19] Py：正则替换带回调
来源：http://cnv.cqqwz.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://dwj.fzhhl.top

[U20] Py：缓存函数结果
来源：http://lqi.xingfuxueyuan.xyz

@functools.lru_cache(maxsize=None)
来源：http://dxi.yj20258888.top

[U21] Py：自定义上下文管理器
来源：http://yfk.hywenlv.cn

@contextlib.contextmanager
来源：http://fjn.sysykeji.top

[U22] Py：矩阵转置
来源：http://ony.cqqwz.cn

list(zip(*m))
来源：http://qel.hnxiangtu.top

[U23] Py：分块读取大文件
来源：http://pko.hfpthk.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bhq.hcnkem.com

[U24] Py：路径操作
来源：http://rgj.havefunace.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lao.pycfn.com

[U25] Py：CSV 按字典读
来源：http://zrb.jianghu66.top

csv.DictReader(f)
来源：http://ahn.52xcode.cn

[U26] Py：并发下载
来源：http://nxm.xuanzx.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://efn.cdnleiting.top

[U27] Py：异步 HTTP
来源：http://khg.chenlongwang.top

aiohttp.ClientSession() 配合 async with
来源：http://xvo.smart0.xyz

[U28] Py：类型别名
来源：http://qir.xziqi.cn

UserId = int
来源：http://dom.yonumen.top

[U29] Py：属性校验
来源：http://okg.aibaodan.cn

@property 与 @x.setter 配合
来源：http://vua.yongpay.top

[U30] Py：数据类
来源：http://ekq.cashguo.top

@dataclass(slots=True)
来源：http://uht.cdnleiting.top

[U31] Py：单测
来源：http://koq.xziqi.cn

python -m pytest -q
来源：http://dhe.shanyushiyangtech.top

[U32] Py：代码格式化
来源：http://jwp.yvedp.cn

ruff format . && ruff check --fix .
来源：http://beu.0kj1m.cn

[U33] Py：打包发布
来源：http://adg.kuanghao11.cn

python -m build  （依赖 pyproject.toml）
来源：http://teg.fktsv.cn

[U34] Py：判断编码
来源：http://ezr.cucudq.cn

chardet.detect(raw)
来源：http://acu.hywenlv.cn

[U35] Py：发送邮件
来源：http://uav.gogol.net.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yms.cqqwz.cn

[U36] Py：定时任务
来源：http://dup.meibo888.top

schedule.every(10).minutes.do(job)
来源：http://czt.yangfankeji.com

[U37] Py：读写 Excel
来源：http://ozv.gzhubu.top

pandas.read_excel / DataFrame.to_excel
来源：http://wyv.hnxiangtu.top

[U38] Py：获取脚本所在目录
来源：http://cvc.jiagoushi.top

Path(__file__).resolve().parent
来源：http://hyl.dianchejie.cn

[U39] Py：判断是否在交互环境
来源：http://fgf.yvedp.cn

sys.stdout.isatty()
来源：http://saa.zhiwuduotai.top

[U40] Py：打印到标准错误
来源：http://otd.xinyue.icu

print("err", file=sys.stderr)
来源：http://dxh.zdqjudy.top

[U41] PHP：初始化 Composer 项目
来源：http://iir.jinqigufen.top

composer init;  composer require guzzlehttp/guzzle
来源：http://yxt.redwolf501.top

[U42] PHP：PSR-4 自动加载
来源：http://gqw.ywan-chungtsiang.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lmi.iojbl.cn

[U43] PHP：声明命名空间
来源：http://ncl.jianghu66.top

namespace App\Http;
来源：http://mkt.52xcode.cn

[U44] PHP：开启严格类型
来源：http://elp.redwolf501.top

declare(strict_types=1);
来源：http://xwt.hongshengwenyu.top

[U45] PHP：类型声明与返回类型
来源：http://jus.xuanzx.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://kuu.bjfxy.top

[U46] PHP：可空类型
来源：http://xie.feifeiyinyue.top

?string $name = null
来源：http://jku.cheryme.top

[U47] PHP：联合类型
来源：http://tfn.9152youxi.cn

int|string $id
来源：http://drk.cashguo.top

[U48] PHP：纯枚举
来源：http://ysp.zhoulong.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bpu.aizwys.cn

[U49] PHP：只读属性
来源：http://ccy.chenzaomai.com

public readonly string $name
来源：http://gbu.bjfxy.top

[U50] PHP：构造器属性提升
来源：http://poh.yonumen.top

public function __construct(private int $id) {}
来源：http://ssm.aibaodan.cn

[U51] PHP：数组解构
来源：http://gik.jianghu66.top

[$a, $b] = $arr;
来源：http://luu.sweek.top

[U52] PHP：箭头函数
来源：http://dqf.shangyingyoupin.top

$double = fn($x) => $x * 2;
来源：http://yai.zhiwuduotai.top

[U53] PHP：空合并运算符
来源：http://usk.hysaishi.cn

$v = $a ?? $b ?? "default";
来源：http://lyp.jianghu66.top

[U54] PHP：空安全调用
来源：http://dnl.shuidangran.top

$obj?->method()
来源：http://veu.chenzaomai.com

[U55] PHP：match 表达式
来源：http://ymf.yonumen.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gxr.yuanzhike.top

[U56] PHP：命名参数
来源：http://ubz.fanxiaobao.xyz

f(a: 1, b: 2)
来源：http://byg.kuanghao11.cn

[U57] PHP：字符串插值
来源：http://euo.yanxiufei.cn

"值: {$a}"
来源：http://oqx.yueranfly.top

[U58] PHP：数组三件套
来源：http://hfo.yueranfly.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://tzc.bjfxy.top

[U59] PHP：自定义排序
来源：http://zfk.zhixingplan.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vxl.yuxming.cn

[U60] PHP：JSON 编解码
来源：http://oei.zycfv.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://txo.sjlbkw.cn

[U61] PHP：正则
来源：http://uqu.ehwqpu.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qsv.hongshengwenyu.top

[U62] PHP：日期对象
来源：http://tru.yfazqb.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mhw.xuetiantiany.cn

[U63] PHP：文件读写
来源：http://xte.tarul.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://cuc.guannengcc.top

[U64] PHP：目录遍历
来源：http://mkw.xuanzx.com

glob("dir/*.php");  scandir("dir");
来源：http://ylc.haohaochexian.top

[U65] PHP：会话
来源：http://kyw.yonumen.top

session_start();  $_SESSION["uid"] = 1;
来源：http://wkl.jinghuilouyu.cn

[U66] PHP：设置 Cookie
来源：http://iuw.fktsv.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://aes.nwbrower.top

[U67] PHP：处理文件上传
来源：http://rqx.ydzc1.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fle.zhongyouzk.top

[U68] PHP：PDO 连接
来源：http://ika.feifeiyinyue.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ptu.zdbjq.cn

[U69] PHP：PDO 预处理
来源：http://dym.sufxvd.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dfd.hammf.cn

[U70] PHP：PDO 事务
来源：http://rrj.ppjwa.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fhn.fehbvm.com

[U71] PHP：抛出异常
来源：http://azb.jyoumei.cn

throw new RuntimeException("失败", 500);
来源：http://nls.zhongyouzk.top

[U72] PHP：写错误日志
来源：http://srj.tian-w.cn

error_log("失败: " . $e->getMessage());
来源：http://svb.hammf.cn

[U73] PHP：读取 ini 配置
来源：http://ehb.daxiang520.top

parse_ini_file("config.ini", true)
来源：http://jvx.bbcook.cn

[U74] PHP：读取环境变量
来源：http://lma.fktsv.cn

getenv("APP_ENV") ?: "production"
来源：http://dpo.hfpthk.cn

[U75] PHP：依赖注入
来源：http://whg.yj20258888.top

composer require psr/container
来源：http://ryg.jqgfzy.top

[U76] PHP：简单路由
来源：http://zgs.pycfn.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ehn.zhiwuduotai.top

[U77] PHP：模板渲染
来源：http://zul.pengpengdd.cyou

composer require twig/twig
来源：http://blx.jyoumei.cn

[U78] PHP：单元测试
来源：http://jzs.sxryk.cn

composer require --dev phpunit/phpunit
来源：http://voo.jinqigufen.top

[U79] PHP：静态分析
来源：http://swn.nanxuanxn.top

composer require --dev phpstan/phpstan
来源：http://zsf.nanxinkj.top

[U80] PHP：代码规范修复
来源：http://uso.zhengqikj.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://amu.jiagoushi.top

[U81] JS：初始化项目
来源：http://kbb.yvedp.cn

npm init -y;  npm i express
来源：http://qqc.jinqigufen.top

[U82] JS：package.json 脚本
来源：http://fnj.pycfn.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://trj.vehdjk.com

[U83] JS：ES Module 导入导出
来源：http://gxv.epnwcf.com

export const a = 1;  import { a } from "./m.js";
来源：http://fjx.hywenlv.cn

[U84] JS：CommonJS 写法
来源：http://gkn.redwolf501.top

module.exports = { a };  const { a } = require("./m");
来源：http://oec.52xcode.cn

[U85] JS：可选链
来源：http://qxs.tian-w.cn

a?.b?.c
来源：http://dxm.sjlbkw.cn

[U86] JS：空值合并
来源：http://mfm.daria6918.cn

a ?? b
来源：http://cwt.smart0.xyz

[U87] JS：解构默认值
来源：http://ckl.fzhhl.top

const { a = 1, b = 2 } = obj;
来源：http://wws.cdnleiting.top

[U88] JS：对象展开合并
来源：http://cba.jyoumei.cn

{ ...a, ...b }
来源：http://frg.ydjk.org.cn

[U89] JS：数组去重
来源：http://izu.chenzaomai.com

[...new Set(arr)]
来源：http://ofs.yfazqb.com

[U90] JS：数字数组排序
来源：http://daj.jiagoushi.top

[...arr].sort((a, b) => a - b)
来源：http://ebg.dashuyun.cn

[U91] JS：对象键值遍历
来源：http://cze.fengsongda.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://axg.yj20258.top

[U92] JS：深拷贝
来源：http://nmj.uphjek.com

structuredClone(obj)
来源：http://rqr.zhongyouzk.top

[U93] JS：模板字符串
来源：http://krg.fanxiaobao.xyz

`共 ${n} 条`
来源：http://alb.nwbrower.top

[U94] JS：箭头函数
来源：http://jep.52xcode.cn

const double = x => x * 2;
来源：http://zlw.wangdashe.top

[U95] JS：Promise 包装
来源：http://hjj.dianchejie.cn

new Promise((resolve, reject) => {})
来源：http://lsx.dianchejie.cn

[U96] JS：async/await 与异常
来源：http://vae.jqgfzy.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lan.yonumen.top

[U97] JS：并发请求
来源：http://uvw.zhoulong.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://bjq.9152youxi.cn

[U98] JS：fetch 带 JSON
来源：http://wzr.snrcjt.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fqd.xuetiantiany.cn

[U99] JS：事件监听
来源：http://mcz.sufxvd.cn

el.addEventListener("click", e => {})
来源：http://idv.ehwqpu.com

[U100] JS：DOM 查询
来源：http://omw.guowangkeji.top

document.querySelector(".item")
来源：http://mma.sysykeji.top

[U101] JS：classList 操作
来源：http://xoy.hongshengwenyu.top

el.classList.toggle("active")
来源：http://pnn.sysykeji.top

[U102] JS：本地存储
来源：http://kwn.wangdashe.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://vwy.iojbl.cn

[U103] JS：定时器
来源：http://mvg.chenzaomai.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fbo.aizwys.cn

[U104] JS：防抖
来源：http://iqj.jlsjyb.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iip.sxryk.cn

[U105] JS：节流
来源：http://gcm.fengsongda.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wlk.hywenlv.cn

[U106] JS：日期格式化
来源：http://iww.xziqi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://siv.bjfxy.top

[U107] JS：数字千分位
来源：http://vos.sxryk.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ysq.fktsv.cn

[U108] JS：随机整数
来源：http://lko.ydjk.org.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://krv.andypj.xyz

[U109] JS：数组分组
来源：http://gen.zycfv.cn

Object.groupBy(arr, x => x.type)
来源：http://nmt.zhijiandao.cn

[U110] JS：数组分块
来源：http://ysv.jyoumei.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rjt.tanke756.top

[U111] JS：对象转 Map
来源：http://ulh.hysaishi.cn

new Map(Object.entries(obj))
来源：http://ygm.wangdashe.top

[U112] JS：字符串补位
来源：http://zvt.zhiwuduotai.top

"7".padStart(3, "0")
来源：http://nxf.sweek.top

[U113] JS：正则替换全部
来源：http://cew.jiagoushi.top

s.replaceAll("a", "b")
来源：http://vbt.yongpay.top

[U114] JS：JSON 深比较
来源：http://qib.yfazqb.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://zvg.gaohongyu789.top

[U115] JS：生成 UUID
来源：http://isd.xylfe.cn

crypto.randomUUID()
来源：http://ooj.pengpengdd.cyou

[U116] JS：类型检查（JSDoc）
来源：http://cpk.yangfankeji.com

/** @param {string} name */ function f(name) {}
来源：http://rtw.ywan-chungtsiang.top

[U117] JS：单元测试
来源：http://pdy.pengpengdd.cyou

npm i -D vitest;  npx vitest
来源：http://xvy.jinqigfzy.top

[U118] JS：开发服务器
来源：http://hom.shanyushiyangtech.top

npm i -D vite;  npx vite
来源：http://hts.fzhhl.top

[U119] JS：生产构建
来源：http://aks.xuetiantiany.cn

npx vite build
来源：http://uqt.tian-w.cn

[U120] JS：读取环境变量（Vite）
来源：http://elh.gaohongyu789.top

import.meta.env.VITE_API_URL
来源：http://ivz.uphjek.com

================================================================================
来源：http://fmx.zhiwuduotai.top

统计汇总
来源：http://kax.bbcook.cn

================================================================================
来源：http://jfb.yonumen.top

按语言统计（条）：
来源：http://ghk.quarkkingdee.top

Python ......... 252
来源：http://hcc.ydzc1.top

PHP ............ 252
来源：http://emp.sxryk.cn

JavaScript ..... 252
来源：http://cvh.cucudq.cn

TypeScript ..... 212
来源：http://toq.jlsjyb.cn

Java ........... 212
来源：http://ocj.shzxlz.cn

Go ............. 212
来源：http://kaw.redwolf501.top

Ruby ........... 212
来源：http://cjs.hfpthk.cn

C# ............. 212
来源：http://xmr.daria6918.cn

C .............. 30
来源：http://hex.svipenyu.cn

C++ ............ 30
来源：http://roh.iojbl.cn

SQL ............ 90
来源：http://tul.yanxiufei.cn

Bash ........... 80
来源：http://jhp.xuanzx.com

Kotlin ......... 15
来源：http://plm.sxryk.cn

Swift .......... 15
来源：http://iqa.gzhubu.top

Lua ............ 10
来源：http://ubo.jiagoushi.top

Perl ........... 10
来源：http://zpx.aizwys.cn

Scala .......... 10
来源：http://wrf.316326.xyz

------------------------------------
来源：http://elj.sxryk.cn

合计 ........... 2106 条
来源：http://ncw.haohaochexian.top

按章节统计：
来源：http://tzx.vqdsnc.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hlv.uphjek.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://abr.pycfn.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://tgy.nanxuanxn.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://bwp.nanxuanxn.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bzw.chenzaomai.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wuz.zhongyouzk.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hrx.xinyue.icu

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://iue.xuanzx.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ivg.hnqzz.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zmv.jqgfzy.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://nrq.dianchejie.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lre.epnwcf.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://lju.ppjwa.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ccf.epnwcf.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://brd.uphjek.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ncf.jinqigfzy.top

Q SQL 专题                              90
来源：http://rhe.nanxuanxn.top

R Bash 专题                             80
来源：http://dkl.zycfv.cn

S C / C++ 专题                          60
来源：http://pgv.daxiang520.top

T 其他语言补充                          60
来源：http://qsm.xziqi.cn

U 高频实用片段                         120
来源：http://fkr.redwolf501.top

------------------------------------
来源：http://hyg.guannengcc.top

合计                                  2106 条
来源：http://uyr.chenjidiqi.icu

--------------------------------------------------------------------------------
来源：http://vih.yangfankeji.com

使用提醒
来源：http://znr.zhijiandao.cn

--------------------------------------------------------------------------------
来源：http://mxh.ywan-chungtsiang.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xbx.c1oappe.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bwd.iojbl.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qnf.hnqzz.top

在旧版本上使用前请先确认语法支持情况。
来源：http://nxm.haohaochexian.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://yzs.bjfxy.top

—— 文件结束 ——
来源：http://xyr.ydjk.org.cn

================================================================================
来源：http://wmk.vehdjk.com

程序语言常见例子速查手册（2024 版）
来源：http://ghp.jiagoushi.top

Common Programming Examples Cheat Book
来源：http://sum.jqgufenzy.top

================================================================================
来源：http://sgw.fktsv.cn

【收录内容】
来源：http://mod.zhoulong.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://lha.tarul.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://zkc.chenlongwang.top

SQL · Bash · C · C++
来源：http://mnd.jianghu66.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ose.hcnkem.com

【使用说明】
来源：http://oup.9152youxi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://sbe.daria6918.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://rsa.dashuyun.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://kmk.cqqwz.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://uxe.chenjidiqi.icu

Bash:  Shell         C:     C             C++:   C++
来源：http://sla.epnwcf.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://bjj.zhoulong.xyz


<!-- 参考信息 -->