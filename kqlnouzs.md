代发 wailian999

[U07] Py：反转字典键值
来源：http://rbi.yj20258.top

{v: k for k, v in d.items()}
来源：http://jyy.vqdsnc.cn

[U08] Py：展平二维列表
来源：http://mmf.jyoumei.cn

[y for x in nested for y in x]
来源：http://god.gotoacloud.top

[U09] Py：字典取最大值的键
来源：http://ulg.gotoacloud.top

max(d, key=d.get)
来源：http://joy.52xcode.cn

[U10] Py：按值排序字典
来源：http://zgj.fktsv.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ckk.ywan-chungtsiang.top

[U11] Py：生成器表达式
来源：http://tjb.316326.xyz

(x * 2 for x in arr)
来源：http://edm.nwbrower.top

[U12] Py：取出现最多的 3 个元素
来源：http://yql.iojbl.cn

Counter(arr).most_common(3)
来源：http://ykv.cucudq.cn

[U13] Py：固定长度队列
来源：http://qwf.yongpay.top

deque(maxlen=10)
来源：http://ucw.feifeiyinyue.top

[U14] Py：分组收集到列表
来源：http://gyu.ydjk.org.cn

defaultdict(list)
来源：http://evj.snrcjt.cn

[U15] Py：高精度计时
来源：http://drl.nwbrower.top

t = time.perf_counter()
来源：http://zqz.hnxiangtu.top

[U16] Py：命令行参数解析
来源：http://evy.quarkkingdee.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://agj.yj20258888.top

[U17] Py：初始化日志
来源：http://ivy.ydzc1.top

logging.basicConfig(level=logging.INFO)
来源：http://zyt.chenjidiqi.icu

[U18] Py：预编译正则
来源：http://bwr.aizwys.cn

pat = re.compile(r"\d+")
来源：http://sxs.fehbvm.com

[U19] Py：正则替换带回调
来源：http://ijk.hnqzz.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wng.nwbrower.top

[U20] Py：缓存函数结果
来源：http://his.iojbl.cn

@functools.lru_cache(maxsize=None)
来源：http://qbs.yvedp.cn

[U21] Py：自定义上下文管理器
来源：http://vuz.jiagoushi.top

@contextlib.contextmanager
来源：http://lkr.aibaodan.cn

[U22] Py：矩阵转置
来源：http://mga.wangdashe.top

list(zip(*m))
来源：http://ysi.snrcjt.cn

[U23] Py：分块读取大文件
来源：http://obw.hnqzz.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ytc.birdmap.top

[U24] Py：路径操作
来源：http://ogc.daxiang520.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hyo.zdbjq.cn

[U25] Py：CSV 按字典读
来源：http://ald.zhixingplan.top

csv.DictReader(f)
来源：http://lgq.yj202588.top

[U26] Py：并发下载
来源：http://tzl.yfazqb.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qjt.zhaomingkeji.xyz

[U27] Py：异步 HTTP
来源：http://tdy.smart0.xyz

aiohttp.ClientSession() 配合 async with
来源：http://etn.meibo888.top

[U28] Py：类型别名
来源：http://ofm.sjlbkw.cn

UserId = int
来源：http://tzh.vehdjk.com

[U29] Py：属性校验
来源：http://esf.fktsv.cn

@property 与 @x.setter 配合
来源：http://ptz.aibaodan.cn

[U30] Py：数据类
来源：http://lxf.gaohongyu789.top

@dataclass(slots=True)
来源：http://tjo.chenzaomai.com

[U31] Py：单测
来源：http://grk.jinqigfzy.top

python -m pytest -q
来源：http://eix.xuetiantiany.cn

[U32] Py：代码格式化
来源：http://tki.chenjidiqi.icu

ruff format . && ruff check --fix .
来源：http://uea.xuanzx.com

[U33] Py：打包发布
来源：http://qvt.hywenlv.cn

python -m build  （依赖 pyproject.toml）
来源：http://urw.tanke756.top

[U34] Py：判断编码
来源：http://qui.pycfn.com

chardet.detect(raw)
来源：http://lrc.epnwcf.com

[U35] Py：发送邮件
来源：http://irh.cqqwz.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://lvx.wangshuangyany.cn

[U36] Py：定时任务
来源：http://yoa.shanyushiyangtech.top

schedule.every(10).minutes.do(job)
来源：http://tic.smart0.xyz

[U37] Py：读写 Excel
来源：http://fnl.jianghu66.top

pandas.read_excel / DataFrame.to_excel
来源：http://edr.cheryme.top

[U38] Py：获取脚本所在目录
来源：http://kiw.jqgufenzy.top

Path(__file__).resolve().parent
来源：http://wba.jianghu66.top

[U39] Py：判断是否在交互环境
来源：http://ens.jiagoushi.top

sys.stdout.isatty()
来源：http://pfd.hesvh.cn

[U40] Py：打印到标准错误
来源：http://pei.snrcjt.cn

print("err", file=sys.stderr)
来源：http://pvp.redwolf501.top

[U41] PHP：初始化 Composer 项目
来源：http://vzq.hfpthk.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://vaw.nanxuanxn.top

[U42] PHP：PSR-4 自动加载
来源：http://ujw.tanke756.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dlx.sysykeji.top

[U43] PHP：声明命名空间
来源：http://uks.redwolf501.top

namespace App\Http;
来源：http://igz.zhaomingkeji.xyz

[U44] PHP：开启严格类型
来源：http://ozk.ydjk.org.cn

declare(strict_types=1);
来源：http://wfj.jinyuanbaomall.cn

[U45] PHP：类型声明与返回类型
来源：http://rkf.chenjidiqi.icu

function add(int $a, int $b): int { return $a + $b; }
来源：http://lwa.chenzaomai.com

[U46] PHP：可空类型
来源：http://ezi.xylfe.cn

?string $name = null
来源：http://wmi.zhengqikj.top

[U47] PHP：联合类型
来源：http://tum.hongshengwenyu.top

int|string $id
来源：http://yvi.tianlin.xyz

[U48] PHP：纯枚举
来源：http://rps.tianlin.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jsh.bjfxy.top

[U49] PHP：只读属性
来源：http://fwy.9152youxi.cn

public readonly string $name
来源：http://fkl.sysykeji.top

[U50] PHP：构造器属性提升
来源：http://fuv.nanxinkj.top

public function __construct(private int $id) {}
来源：http://ijm.tarul.cn

[U51] PHP：数组解构
来源：http://ldj.ctjpmb.com

[$a, $b] = $arr;
来源：http://gem.tarul.cn

[U52] PHP：箭头函数
来源：http://uqs.xuanzx.com

$double = fn($x) => $x * 2;
来源：http://oym.jianghu66.top

[U53] PHP：空合并运算符
来源：http://ela.kuanghao11.cn

$v = $a ?? $b ?? "default";
来源：http://qpk.tanke756.top

[U54] PHP：空安全调用
来源：http://cxj.yj20258.top

$obj?->method()
来源：http://gjy.jiagoushi.top

[U55] PHP：match 表达式
来源：http://nfs.shanyushiyangtech.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://whz.jyoumei.cn

[U56] PHP：命名参数
来源：http://ukr.haohaochexian.top

f(a: 1, b: 2)
来源：http://mtz.ivvv.top

[U57] PHP：字符串插值
来源：http://wex.dianchejie.cn

"值: {$a}"
来源：http://qwi.bjfxy.top

[U58] PHP：数组三件套
来源：http://ajh.zhijiandao.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vjv.zhixingplan.top

[U59] PHP：自定义排序
来源：http://bod.zhixingplan.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sca.hysaishi.cn

[U60] PHP：JSON 编解码
来源：http://rdj.wangdashe.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ujm.cheryme.top

[U61] PHP：正则
来源：http://nvc.hesvh.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xmj.xuanzx.com

[U62] PHP：日期对象
来源：http://cmu.shangyingyoupin.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zlq.zycfv.cn

[U63] PHP：文件读写
来源：http://jnk.zhixingplan.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://eae.jqgfzy.top

[U64] PHP：目录遍历
来源：http://foq.hammf.cn

glob("dir/*.php");  scandir("dir");
来源：http://ffc.52xcode.cn

[U65] PHP：会话
来源：http://kyb.nanxinkj.top

session_start();  $_SESSION["uid"] = 1;
来源：http://opg.chenlongwang.top

[U66] PHP：设置 Cookie
来源：http://pyh.shuidangran.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zhj.nanxinkj.top

[U67] PHP：处理文件上传
来源：http://ijw.shuidangran.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ctt.yonumen.top

[U68] PHP：PDO 连接
来源：http://jur.gogol.net.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://yyd.hnqzz.top

[U69] PHP：PDO 预处理
来源：http://lsz.uphjek.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://uqx.yvedp.cn

[U70] PHP：PDO 事务
来源：http://kfi.zhijiandao.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://uee.hcnkem.com

[U71] PHP：抛出异常
来源：http://csd.hnxiangtu.top

throw new RuntimeException("失败", 500);
来源：http://hhw.zhixingplan.top

[U72] PHP：写错误日志
来源：http://ooc.hfpthk.cn

error_log("失败: " . $e->getMessage());
来源：http://wvo.xziqi.cn

[U73] PHP：读取 ini 配置
来源：http://pjf.yj202588.top

parse_ini_file("config.ini", true)
来源：http://umo.ppjwa.cn

[U74] PHP：读取环境变量
来源：http://sgk.haohaochexian.top

getenv("APP_ENV") ?: "production"
来源：http://rsh.smart0.xyz

[U75] PHP：依赖注入
来源：http://hsd.zhixingplan.top

composer require psr/container
来源：http://pnf.pycfn.com

[U76] PHP：简单路由
来源：http://oxo.iojbl.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://clv.316326.xyz

[U77] PHP：模板渲染
来源：http://fgz.316326.xyz

composer require twig/twig
来源：http://otp.yj20258888.top

[U78] PHP：单元测试
来源：http://fgf.wangshuangyany.cn

composer require --dev phpunit/phpunit
来源：http://tkj.xziqi.cn

[U79] PHP：静态分析
来源：http://eak.hcnkem.com

composer require --dev phpstan/phpstan
来源：http://sry.jqgfzy.top

[U80] PHP：代码规范修复
来源：http://ucj.guowangkeji.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://tco.hnqzz.top

[U81] JS：初始化项目
来源：http://fta.havefunace.top

npm init -y;  npm i express
来源：http://zvu.kuanghao11.cn

[U82] JS：package.json 脚本
来源：http://ith.yj20258888.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kis.pycfn.com

[U83] JS：ES Module 导入导出
来源：http://boo.hnxiangtu.top

export const a = 1;  import { a } from "./m.js";
来源：http://ilu.dianchejie.cn

[U84] JS：CommonJS 写法
来源：http://jju.vqdsnc.cn

module.exports = { a };  const { a } = require("./m");
来源：http://shb.fktsv.cn

[U85] JS：可选链
来源：http://buw.zhiwuduotai.top

a?.b?.c
来源：http://ric.jqgfzy.top

[U86] JS：空值合并
来源：http://agp.316326.xyz

a ?? b
来源：http://akj.xuanzx.com

[U87] JS：解构默认值
来源：http://inw.ivvv.top

const { a = 1, b = 2 } = obj;
来源：http://xry.shanyushiyangtech.top

[U88] JS：对象展开合并
来源：http://jvx.xziqi.cn

{ ...a, ...b }
来源：http://uxc.smart0.xyz

[U89] JS：数组去重
来源：http://heu.hcnkem.com

[...new Set(arr)]
来源：http://rju.feifeiyinyue.top

[U90] JS：数字数组排序
来源：http://mvq.jinghuilouyu.cn

[...arr].sort((a, b) => a - b)
来源：http://rmq.ppjwa.cn

[U91] JS：对象键值遍历
来源：http://jmj.yj20258888.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gpk.fktsv.cn

[U92] JS：深拷贝
来源：http://nbf.jinqigfzy.top

structuredClone(obj)
来源：http://ibn.jinqigfzy.top

[U93] JS：模板字符串
来源：http://gjk.zycfv.cn

`共 ${n} 条`
来源：http://vfm.ywan-chungtsiang.top

[U94] JS：箭头函数
来源：http://mqp.shangyingyoupin.top

const double = x => x * 2;
来源：http://fcy.ydzc1.top

[U95] JS：Promise 包装
来源：http://rws.zhengqikj.top

new Promise((resolve, reject) => {})
来源：http://khd.zhengqikj.top

[U96] JS：async/await 与异常
来源：http://mkq.quarkkingdee.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hby.jiagoushi.top

[U97] JS：并发请求
来源：http://mou.cheryme.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://mic.shzxlz.cn

[U98] JS：fetch 带 JSON
来源：http://rma.nanxinkj.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ell.bjfxy.top

[U99] JS：事件监听
来源：http://zla.svipenyu.cn

el.addEventListener("click", e => {})
来源：http://xag.gzhubu.top

[U100] JS：DOM 查询
来源：http://bit.xuanzx.com

document.querySelector(".item")
来源：http://bqz.yangfankeji.com

[U101] JS：classList 操作
来源：http://bzi.wangshuangyany.cn

el.classList.toggle("active")
来源：http://vro.bjfxy.top

[U102] JS：本地存储
来源：http://ioq.zdqjudy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://utw.fehbvm.com

[U103] JS：定时器
来源：http://jtg.jyoumei.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://oen.cqqwz.cn

[U104] JS：防抖
来源：http://rea.hongshengwenyu.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hyp.gzhubu.top

[U105] JS：节流
来源：http://gkg.hammf.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cgt.tanke756.top

[U106] JS：日期格式化
来源：http://yml.cdnleiting.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nit.cucudq.cn

[U107] JS：数字千分位
来源：http://qop.fengsongda.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rsx.kuanghao11.cn

[U108] JS：随机整数
来源：http://egj.hysaishi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hhx.yfazqb.com

[U109] JS：数组分组
来源：http://ubw.vqdsnc.cn

Object.groupBy(arr, x => x.type)
来源：http://psv.ywan-chungtsiang.top

[U110] JS：数组分块
来源：http://bhn.vqdsnc.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pme.hnxiangtu.top

[U111] JS：对象转 Map
来源：http://nuv.yj20258.top

new Map(Object.entries(obj))
来源：http://aqd.bbcook.cn

[U112] JS：字符串补位
来源：http://buf.yvedp.cn

"7".padStart(3, "0")
来源：http://ltk.wangshuangyany.cn

[U113] JS：正则替换全部
来源：http://jdc.sxryk.cn

s.replaceAll("a", "b")
来源：http://urq.guowangkeji.top

[U114] JS：JSON 深比较
来源：http://mir.fengsongda.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://mmi.shuidangran.top

[U115] JS：生成 UUID
来源：http://zry.zycfv.cn

crypto.randomUUID()
来源：http://klr.redwolf501.top

[U116] JS：类型检查（JSDoc）
来源：http://fql.yuanzhike.top

/** @param {string} name */ function f(name) {}
来源：http://lee.zdqjudy.top

[U117] JS：单元测试
来源：http://mog.ctjpmb.com

npm i -D vitest;  npx vitest
来源：http://kzo.guannengcc.top

[U118] JS：开发服务器
来源：http://ubc.fehbvm.com

npm i -D vite;  npx vite
来源：http://dww.ivvv.top

[U119] JS：生产构建
来源：http://ity.gzhubu.top

npx vite build
来源：http://car.jiagoushi.top

[U120] JS：读取环境变量（Vite）
来源：http://qav.zhoulong.xyz

import.meta.env.VITE_API_URL
来源：http://rox.sjlbkw.cn

================================================================================
来源：http://hzq.jinyuanbaomall.cn

统计汇总
来源：http://wwk.zhixingplan.top

================================================================================
来源：http://hqj.shuidangran.top

按语言统计（条）：
来源：http://jvy.aizwys.cn

Python ......... 252
来源：http://pol.zhiwuduotai.top

PHP ............ 252
来源：http://fdr.c1oappe.top

JavaScript ..... 252
来源：http://lzc.havefunace.top

TypeScript ..... 212
来源：http://hgx.hnqzz.top

Java ........... 212
来源：http://lgi.snrcjt.cn

Go ............. 212
来源：http://ebj.zdbjq.cn

Ruby ........... 212
来源：http://ewm.jqgufenzy.top

C# ............. 212
来源：http://hng.sxryk.cn

C .............. 30
来源：http://xmc.hesvh.cn

C++ ............ 30
来源：http://atk.yuanzhike.top

SQL ............ 90
来源：http://vat.cucudq.cn

Bash ........... 80
来源：http://iae.zhiwuduotai.top

Kotlin ......... 15
来源：http://xgc.smart0.xyz

Swift .......... 15
来源：http://pic.gogol.net.cn

Lua ............ 10
来源：http://pih.andypj.xyz

Perl ........... 10
来源：http://wsm.hnxiangtu.top

Scala .......... 10
来源：http://cic.zycfv.cn

------------------------------------
来源：http://jyo.zhiwuduotai.top

合计 ........... 2106 条
来源：http://hea.xuanzx.com

按章节统计：
来源：http://byz.zycfv.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fkf.zhixingplan.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jhk.redwolf501.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hmp.zhoulong.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fwn.aizwys.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://deh.yfazqb.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vay.chenzaomai.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://szg.feifeiyinyue.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://njg.fehbvm.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mhl.sufxvd.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://uxb.bbcook.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://cyy.svipenyu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zpp.jianghu66.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bxs.zdbjq.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ubb.andypj.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://pwq.0kj1m.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vcv.tanke756.top

Q SQL 专题                              90
来源：http://rdv.jyoumei.cn

R Bash 专题                             80
来源：http://twy.shanyushiyangtech.top

S C / C++ 专题                          60
来源：http://agv.tianlin.xyz

T 其他语言补充                          60
来源：http://vbw.316326.xyz

U 高频实用片段                         120
来源：http://zec.yuxming.cn

------------------------------------
来源：http://xpz.zhijiandao.cn

合计                                  2106 条
来源：http://zmv.birdmap.top

--------------------------------------------------------------------------------
来源：http://hzi.shanyushiyangkeji.top

使用提醒
来源：http://ynb.jlsjyb.cn

--------------------------------------------------------------------------------
来源：http://sim.hongshengwenyu.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ixw.hywenlv.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wis.mhx1999.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://gil.tianlin.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://fmj.bjfxy.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://tmk.gzhubu.top

—— 文件结束 ——
来源：http://gkt.bjfxy.top

================================================================================
来源：http://nxn.nanxuanxn.top

程序语言常见例子速查手册（2024 版）
来源：http://vjz.xziqi.cn

Common Programming Examples Cheat Book
来源：http://qpz.xylfe.cn

================================================================================
来源：http://ytb.aizwys.cn

【收录内容】
来源：http://yyb.nwbrower.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://lev.0kj1m.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tbn.birdmap.top

SQL · Bash · C · C++
来源：http://jlt.vqdsnc.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ngv.jqgufenzy.top

【使用说明】
来源：http://kmk.quarkkingdee.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mnk.tarul.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vhh.pycfn.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://dea.sufxvd.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ufj.zhiwuduotai.top

Bash:  Shell         C:     C             C++:   C++
来源：http://fql.xingfuxueyuan.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://eyw.zhengqikj.top


<!-- 参考信息 -->