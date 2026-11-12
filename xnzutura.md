代发 wailian999

[U07] Py：反转字典键值
来源：http://fvj.chenlongwang.top

{v: k for k, v in d.items()}
来源：http://qgm.aibaodan.cn

[U08] Py：展平二维列表
来源：http://nrh.cheryme.top

[y for x in nested for y in x]
来源：http://hip.haohaochexian.top

[U09] Py：字典取最大值的键
来源：http://jsg.hcnkem.com

max(d, key=d.get)
来源：http://oag.chenzaomai.com

[U10] Py：按值排序字典
来源：http://qvd.cheryme.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mgj.cdnleiting.top

[U11] Py：生成器表达式
来源：http://heb.ywan-chungtsiang.top

(x * 2 for x in arr)
来源：http://kwd.xinyue.icu

[U12] Py：取出现最多的 3 个元素
来源：http://puy.fanxiaobao.xyz

Counter(arr).most_common(3)
来源：http://tcn.0kj1m.cn

[U13] Py：固定长度队列
来源：http://vsb.wangshuangyany.cn

deque(maxlen=10)
来源：http://pdh.hywenlv.cn

[U14] Py：分组收集到列表
来源：http://pjq.0kj1m.cn

defaultdict(list)
来源：http://zdo.yangfankeji.com

[U15] Py：高精度计时
来源：http://mov.tanke756.top

t = time.perf_counter()
来源：http://ato.yonumen.top

[U16] Py：命令行参数解析
来源：http://ied.vehdjk.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rxo.hcnkem.com

[U17] Py：初始化日志
来源：http://oaq.ydzc1.top

logging.basicConfig(level=logging.INFO)
来源：http://sbg.yonumen.top

[U18] Py：预编译正则
来源：http://bvu.chenjidiqi.icu

pat = re.compile(r"\d+")
来源：http://cbz.gzhubu.top

[U19] Py：正则替换带回调
来源：http://rcg.yj20258.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://war.jqgufenzy.top

[U20] Py：缓存函数结果
来源：http://xac.tanke756.top

@functools.lru_cache(maxsize=None)
来源：http://tqf.9152youxi.cn

[U21] Py：自定义上下文管理器
来源：http://btr.jinqigfzy.top

@contextlib.contextmanager
来源：http://hod.meibo888.top

[U22] Py：矩阵转置
来源：http://ysn.xylfe.cn

list(zip(*m))
来源：http://lwl.gogol.net.cn

[U23] Py：分块读取大文件
来源：http://xkx.hammf.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://cet.zdbjq.cn

[U24] Py：路径操作
来源：http://vew.hfpthk.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qks.andypj.xyz

[U25] Py：CSV 按字典读
来源：http://ftm.zdbjq.cn

csv.DictReader(f)
来源：http://vnt.smart0.xyz

[U26] Py：并发下载
来源：http://dww.dashuyun.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yhh.xuetiantiany.cn

[U27] Py：异步 HTTP
来源：http://cux.ywan-chungtsiang.top

aiohttp.ClientSession() 配合 async with
来源：http://xcc.jinqigfzy.top

[U28] Py：类型别名
来源：http://bbd.epnwcf.com

UserId = int
来源：http://mau.andypj.xyz

[U29] Py：属性校验
来源：http://ymd.pycfn.com

@property 与 @x.setter 配合
来源：http://hme.andypj.xyz

[U30] Py：数据类
来源：http://qhq.c1oappe.top

@dataclass(slots=True)
来源：http://abn.gotoacloud.top

[U31] Py：单测
来源：http://nar.zhoulong.xyz

python -m pytest -q
来源：http://ftu.meibo888.top

[U32] Py：代码格式化
来源：http://zkj.yj20258888.top

ruff format . && ruff check --fix .
来源：http://xnn.yj20258888.top

[U33] Py：打包发布
来源：http://zfn.xuetiantiany.cn

python -m build  （依赖 pyproject.toml）
来源：http://cvt.cheryme.top

[U34] Py：判断编码
来源：http://laq.shanyushiyangkeji.top

chardet.detect(raw)
来源：http://ywl.gzhubu.top

[U35] Py：发送邮件
来源：http://xle.tianlin.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ifs.52xcode.cn

[U36] Py：定时任务
来源：http://lnp.bbcook.cn

schedule.every(10).minutes.do(job)
来源：http://tbk.shangyingyoupin.top

[U37] Py：读写 Excel
来源：http://ink.tarul.cn

pandas.read_excel / DataFrame.to_excel
来源：http://cmg.quarkkingdee.top

[U38] Py：获取脚本所在目录
来源：http://oij.52xcode.cn

Path(__file__).resolve().parent
来源：http://okf.c1oappe.top

[U39] Py：判断是否在交互环境
来源：http://vtf.nwbrower.top

sys.stdout.isatty()
来源：http://wcu.yanxiufei.cn

[U40] Py：打印到标准错误
来源：http://eis.ctjpmb.com

print("err", file=sys.stderr)
来源：http://iko.yueranfly.top

[U41] PHP：初始化 Composer 项目
来源：http://kls.vqdsnc.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://xum.jyoumei.cn

[U42] PHP：PSR-4 自动加载
来源：http://avo.fzhhl.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nvz.yanxiufei.cn

[U43] PHP：声明命名空间
来源：http://dyd.hywenlv.cn

namespace App\Http;
来源：http://era.yueranfly.top

[U44] PHP：开启严格类型
来源：http://bgi.yueranfly.top

declare(strict_types=1);
来源：http://pcq.cucudq.cn

[U45] PHP：类型声明与返回类型
来源：http://qrj.uphjek.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://wfl.guowangkeji.top

[U46] PHP：可空类型
来源：http://yjb.shuidangran.top

?string $name = null
来源：http://zhp.zhijiandao.cn

[U47] PHP：联合类型
来源：http://hyv.jinqigfzy.top

int|string $id
来源：http://dly.nwbrower.top

[U48] PHP：纯枚举
来源：http://bwd.xziqi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xwz.xingfuxueyuan.xyz

[U49] PHP：只读属性
来源：http://boc.zycfv.cn

public readonly string $name
来源：http://zum.aibaodan.cn

[U50] PHP：构造器属性提升
来源：http://eux.andypj.xyz

public function __construct(private int $id) {}
来源：http://ajd.zhoulong.xyz

[U51] PHP：数组解构
来源：http://sgl.redwolf501.top

[$a, $b] = $arr;
来源：http://qpo.wangdashe.top

[U52] PHP：箭头函数
来源：http://nsy.cdnleiting.top

$double = fn($x) => $x * 2;
来源：http://vzs.yuanzhike.top

[U53] PHP：空合并运算符
来源：http://ipw.jyoumei.cn

$v = $a ?? $b ?? "default";
来源：http://lxp.pycfn.com

[U54] PHP：空安全调用
来源：http://yzo.uphjek.com

$obj?->method()
来源：http://hdb.yj20258888.top

[U55] PHP：match 表达式
来源：http://ole.yuxming.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://iwp.zhaomingkeji.xyz

[U56] PHP：命名参数
来源：http://fhi.gotoacloud.top

f(a: 1, b: 2)
来源：http://eqm.hnxiangtu.top

[U57] PHP：字符串插值
来源：http://xyt.ivvv.top

"值: {$a}"
来源：http://lin.zdqjudy.top

[U58] PHP：数组三件套
来源：http://ter.jlsjyb.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rkb.ydjk.org.cn

[U59] PHP：自定义排序
来源：http://eze.dianchejie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kgu.xylfe.cn

[U60] PHP：JSON 编解码
来源：http://jjz.gaohongyu789.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rex.hcnkem.com

[U61] PHP：正则
来源：http://nzc.xinyue.icu

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rxr.mhx1999.top

[U62] PHP：日期对象
来源：http://vkc.zhoulong.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fkb.zhengqikj.top

[U63] PHP：文件读写
来源：http://yhl.xingfuxueyuan.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vfu.epnwcf.com

[U64] PHP：目录遍历
来源：http://bdo.hesvh.cn

glob("dir/*.php");  scandir("dir");
来源：http://xwd.chenlongwang.top

[U65] PHP：会话
来源：http://fow.shuidangran.top

session_start();  $_SESSION["uid"] = 1;
来源：http://bjz.wangshuangyany.cn

[U66] PHP：设置 Cookie
来源：http://ytx.hfpthk.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vrt.ehwqpu.com

[U67] PHP：处理文件上传
来源：http://kbm.xziqi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zvw.chenzaomai.com

[U68] PHP：PDO 连接
来源：http://ovr.yj20258888.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ahj.yj20258888.top

[U69] PHP：PDO 预处理
来源：http://wpj.dianchejie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kal.cheryme.top

[U70] PHP：PDO 事务
来源：http://ocl.svipenyu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://njy.fktsv.cn

[U71] PHP：抛出异常
来源：http://xmf.smart0.xyz

throw new RuntimeException("失败", 500);
来源：http://thg.shanyushiyangtech.top

[U72] PHP：写错误日志
来源：http://ejf.dianchejie.cn

error_log("失败: " . $e->getMessage());
来源：http://aro.hywenlv.cn

[U73] PHP：读取 ini 配置
来源：http://tos.mhx1999.top

parse_ini_file("config.ini", true)
来源：http://txs.uphjek.com

[U74] PHP：读取环境变量
来源：http://vtk.shanyushiyangtech.top

getenv("APP_ENV") ?: "production"
来源：http://dqh.meibo888.top

[U75] PHP：依赖注入
来源：http://ohb.guowangkeji.top

composer require psr/container
来源：http://bcg.zhaomingkeji.xyz

[U76] PHP：简单路由
来源：http://jmr.ydzc1.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ceg.xuetiantiany.cn

[U77] PHP：模板渲染
来源：http://oce.jianghu66.top

composer require twig/twig
来源：http://cjc.zycfv.cn

[U78] PHP：单元测试
来源：http://gvw.nwbrower.top

composer require --dev phpunit/phpunit
来源：http://mnf.9152youxi.cn

[U79] PHP：静态分析
来源：http://klf.ywan-chungtsiang.top

composer require --dev phpstan/phpstan
来源：http://xkt.gotoacloud.top

[U80] PHP：代码规范修复
来源：http://caj.ydzc1.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://sqh.jinyuanbaomall.cn

[U81] JS：初始化项目
来源：http://rru.jlsjyb.cn

npm init -y;  npm i express
来源：http://rxa.daria6918.cn

[U82] JS：package.json 脚本
来源：http://wcf.fktsv.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://soy.hnxiangtu.top

[U83] JS：ES Module 导入导出
来源：http://lsj.hesvh.cn

export const a = 1;  import { a } from "./m.js";
来源：http://hpn.sxryk.cn

[U84] JS：CommonJS 写法
来源：http://qml.wangdashe.top

module.exports = { a };  const { a } = require("./m");
来源：http://kaw.ivvv.top

[U85] JS：可选链
来源：http://avw.sxryk.cn

a?.b?.c
来源：http://eua.shanyushiyangtech.top

[U86] JS：空值合并
来源：http://rhg.haohaochexian.top

a ?? b
来源：http://hqp.cdnleiting.top

[U87] JS：解构默认值
来源：http://kzt.fanxiaobao.xyz

const { a = 1, b = 2 } = obj;
来源：http://phn.52xcode.cn

[U88] JS：对象展开合并
来源：http://unh.haohaochexian.top

{ ...a, ...b }
来源：http://opq.ctjpmb.com

[U89] JS：数组去重
来源：http://awn.mhx1999.top

[...new Set(arr)]
来源：http://afk.yangfankeji.com

[U90] JS：数字数组排序
来源：http://iwv.cashguo.top

[...arr].sort((a, b) => a - b)
来源：http://rmq.shuidangran.top

[U91] JS：对象键值遍历
来源：http://nsr.jqgufenzy.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hlm.zycfv.cn

[U92] JS：深拷贝
来源：http://rxb.uphjek.com

structuredClone(obj)
来源：http://ghh.hesvh.cn

[U93] JS：模板字符串
来源：http://uln.0kj1m.cn

`共 ${n} 条`
来源：http://erq.haohaochexian.top

[U94] JS：箭头函数
来源：http://fjk.0kj1m.cn

const double = x => x * 2;
来源：http://iga.yj202588.top

[U95] JS：Promise 包装
来源：http://grr.yuanzhike.top

new Promise((resolve, reject) => {})
来源：http://dku.epnwcf.com

[U96] JS：async/await 与异常
来源：http://iid.svipenyu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ldu.haohaochexian.top

[U97] JS：并发请求
来源：http://fci.yangfankeji.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://pgm.hysaishi.cn

[U98] JS：fetch 带 JSON
来源：http://cix.yfazqb.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://eaa.vqdsnc.cn

[U99] JS：事件监听
来源：http://iha.sweek.top

el.addEventListener("click", e => {})
来源：http://shc.yuanzhike.top

[U100] JS：DOM 查询
来源：http://ply.jinghuilouyu.cn

document.querySelector(".item")
来源：http://cqh.yj202588.top

[U101] JS：classList 操作
来源：http://bvr.yvedp.cn

el.classList.toggle("active")
来源：http://eaq.xziqi.cn

[U102] JS：本地存储
来源：http://csn.jinyuanbaomall.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://oqp.smart0.xyz

[U103] JS：定时器
来源：http://mct.jyoumei.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://uij.dashuyun.cn

[U104] JS：防抖
来源：http://iph.quarkkingdee.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://edn.zhijiandao.cn

[U105] JS：节流
来源：http://fdd.smart0.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://iqf.xuetiantiany.cn

[U106] JS：日期格式化
来源：http://bna.ybcxt.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rzn.shanyushiyangkeji.top

[U107] JS：数字千分位
来源：http://iug.chenjidiqi.icu

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wha.c1oappe.top

[U108] JS：随机整数
来源：http://oin.yonumen.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://akm.jinghuilouyu.cn

[U109] JS：数组分组
来源：http://yvt.vqdsnc.cn

Object.groupBy(arr, x => x.type)
来源：http://kbd.chenzaomai.com

[U110] JS：数组分块
来源：http://ult.haohaochexian.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bha.feifeiyinyue.top

[U111] JS：对象转 Map
来源：http://rhl.cheryme.top

new Map(Object.entries(obj))
来源：http://ncz.guannengcc.top

[U112] JS：字符串补位
来源：http://yov.cashguo.top

"7".padStart(3, "0")
来源：http://lyw.nwbrower.top

[U113] JS：正则替换全部
来源：http://ueg.shanyushiyangkeji.top

s.replaceAll("a", "b")
来源：http://xeh.kuanghao11.cn

[U114] JS：JSON 深比较
来源：http://xcs.jyoumei.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://plv.shangyingyoupin.top

[U115] JS：生成 UUID
来源：http://nxa.sxryk.cn

crypto.randomUUID()
来源：http://tky.sysykeji.top

[U116] JS：类型检查（JSDoc）
来源：http://opn.zdqjudy.top

/** @param {string} name */ function f(name) {}
来源：http://gsf.tarul.cn

[U117] JS：单元测试
来源：http://jfq.gaohongyu789.top

npm i -D vitest;  npx vitest
来源：http://emd.sxryk.cn

[U118] JS：开发服务器
来源：http://iuf.uphjek.com

npm i -D vite;  npx vite
来源：http://tyl.pycfn.com

[U119] JS：生产构建
来源：http://pva.ehwqpu.com

npx vite build
来源：http://wmg.gaohongyu789.top

[U120] JS：读取环境变量（Vite）
来源：http://dcx.iojbl.cn

import.meta.env.VITE_API_URL
来源：http://uxh.tanke756.top

================================================================================
来源：http://vet.pengpengdd.cyou

统计汇总
来源：http://dnt.hesvh.cn

================================================================================
来源：http://hga.sjlbkw.cn

按语言统计（条）：
来源：http://yds.zycfv.cn

Python ......... 252
来源：http://sln.guannengcc.top

PHP ............ 252
来源：http://kfp.zhiwuduotai.top

JavaScript ..... 252
来源：http://xlh.daria6918.cn

TypeScript ..... 212
来源：http://vzo.hesvh.cn

Java ........... 212
来源：http://ydx.kuanghao11.cn

Go ............. 212
来源：http://xjr.daria6918.cn

Ruby ........... 212
来源：http://kvv.sweek.top

C# ............. 212
来源：http://jdq.fehbvm.com

C .............. 30
来源：http://dgk.birdmap.top

C++ ............ 30
来源：http://wbm.birdmap.top

SQL ............ 90
来源：http://kri.meibo888.top

Bash ........... 80
来源：http://vfq.yfazqb.com

Kotlin ......... 15
来源：http://kku.jinqigfzy.top

Swift .......... 15
来源：http://bml.ctjpmb.com

Lua ............ 10
来源：http://mwt.shanyushiyangkeji.top

Perl ........... 10
来源：http://gqs.aizwys.cn

Scala .......... 10
来源：http://fvi.hywenlv.cn

------------------------------------
来源：http://jlv.xylfe.cn

合计 ........... 2106 条
来源：http://gka.jinqigfzy.top

按章节统计：
来源：http://dxh.hnxiangtu.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://nwm.mhx1999.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://kvj.jiagoushi.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ytc.hysaishi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://yiu.daria6918.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pqg.yangfankeji.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dpv.yj202588.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://iba.ydzc1.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://bfr.fehbvm.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://pyd.zdqjudy.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://cmj.bjfxy.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xpf.jinyuanbaomall.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dhh.guannengcc.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ttj.havefunace.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ndh.shanyushiyangtech.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ump.zdqjudy.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tos.redwolf501.top

Q SQL 专题                              90
来源：http://kgs.sufxvd.cn

R Bash 专题                             80
来源：http://xio.jinqigufen.top

S C / C++ 专题                          60
来源：http://gmo.hysaishi.cn

T 其他语言补充                          60
来源：http://jfg.uphjek.com

U 高频实用片段                         120
来源：http://crk.quarkkingdee.top

------------------------------------
来源：http://iri.zdbjq.cn

合计                                  2106 条
来源：http://hoy.9152youxi.cn

--------------------------------------------------------------------------------
来源：http://yqn.snrcjt.cn

使用提醒
来源：http://qfh.jinghuilouyu.cn

--------------------------------------------------------------------------------
来源：http://rtc.haohaochexian.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://krb.hongshengwenyu.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://elw.ybcxt.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ebj.yj20258888.top

在旧版本上使用前请先确认语法支持情况。
来源：http://jof.shzxlz.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xel.xuetiantiany.cn

—— 文件结束 ——
来源：http://buy.gzhubu.top

================================================================================
来源：http://aqm.jiagoushi.top

程序语言常见例子速查手册（2024 版）
来源：http://qgy.cucudq.cn

Common Programming Examples Cheat Book
来源：http://fmn.hammf.cn

================================================================================
来源：http://ics.zhoulong.xyz

【收录内容】
来源：http://bgf.jyoumei.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://jpc.wangshuangyany.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://csr.ywan-chungtsiang.top

SQL · Bash · C · C++
来源：http://ntf.cucudq.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dyh.smart0.xyz

【使用说明】
来源：http://pzg.chenlongwang.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://lut.xylfe.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vym.jinyuanbaomall.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pno.hammf.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://cmt.pengpengdd.cyou

Bash:  Shell         C:     C             C++:   C++
来源：http://igm.jyoumei.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zcy.gaohongyu789.top


<!-- 参考信息 -->