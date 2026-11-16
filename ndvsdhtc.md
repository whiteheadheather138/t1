代发 wailian999

[U05] Py：列表去重且保序
来源：http://lmn.yanxiufei.cn

list(dict.fromkeys(arr))
来源：http://wut.pengpengdd.cyou

[U06] Py：合并两个字典
来源：http://sch.sysykeji.top

{**a, **b}
来源：http://xhi.zhixingplan.top

[U07] Py：反转字典键值
来源：http://rwo.smart0.xyz

{v: k for k, v in d.items()}
来源：http://ogb.zdqjudy.top

[U08] Py：展平二维列表
来源：http://otv.yvedp.cn

[y for x in nested for y in x]
来源：http://fmz.hnxiangtu.top

[U09] Py：字典取最大值的键
来源：http://cxf.yangfankeji.com

max(d, key=d.get)
来源：http://haw.quarkkingdee.top

[U10] Py：按值排序字典
来源：http://atf.vqdsnc.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zbl.ybcxt.top

[U11] Py：生成器表达式
来源：http://tgk.yueranfly.top

(x * 2 for x in arr)
来源：http://gmo.fanxiaobao.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://yrb.jinqigufen.top

Counter(arr).most_common(3)
来源：http://lhf.gzhubu.top

[U13] Py：固定长度队列
来源：http://iwb.hywenlv.cn

deque(maxlen=10)
来源：http://grp.yangfankeji.com

[U14] Py：分组收集到列表
来源：http://rbm.yuxming.cn

defaultdict(list)
来源：http://uld.yuxming.cn

[U15] Py：高精度计时
来源：http://ekz.ivvv.top

t = time.perf_counter()
来源：http://wff.hcnkem.com

[U16] Py：命令行参数解析
来源：http://box.wangdashe.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ipm.bjfxy.top

[U17] Py：初始化日志
来源：http://lrs.wangdashe.top

logging.basicConfig(level=logging.INFO)
来源：http://vrj.cheryme.top

[U18] Py：预编译正则
来源：http://ell.wangshuangyany.cn

pat = re.compile(r"\d+")
来源：http://szs.cucudq.cn

[U19] Py：正则替换带回调
来源：http://ugb.yonumen.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hqy.pycfn.com

[U20] Py：缓存函数结果
来源：http://gio.xuanzx.com

@functools.lru_cache(maxsize=None)
来源：http://xfe.ppjwa.cn

[U21] Py：自定义上下文管理器
来源：http://cbd.smart0.xyz

@contextlib.contextmanager
来源：http://tnb.daria6918.cn

[U22] Py：矩阵转置
来源：http://jxf.snrcjt.cn

list(zip(*m))
来源：http://nye.jlsjyb.cn

[U23] Py：分块读取大文件
来源：http://kgv.bjfxy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ggl.nwbrower.top

[U24] Py：路径操作
来源：http://kbk.daria6918.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zyo.yangfankeji.com

[U25] Py：CSV 按字典读
来源：http://ocl.ivvv.top

csv.DictReader(f)
来源：http://vjm.wangshuangyany.cn

[U26] Py：并发下载
来源：http://ons.sjlbkw.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vex.jinqigufen.top

[U27] Py：异步 HTTP
来源：http://naa.yj20258.top

aiohttp.ClientSession() 配合 async with
来源：http://ors.zhiwuduotai.top

[U28] Py：类型别名
来源：http://vsz.0kj1m.cn

UserId = int
来源：http://svq.9152youxi.cn

[U29] Py：属性校验
来源：http://jqd.fengsongda.top

@property 与 @x.setter 配合
来源：http://zlj.sysykeji.top

[U30] Py：数据类
来源：http://flc.sweek.top

@dataclass(slots=True)
来源：http://xbf.jqgufenzy.top

[U31] Py：单测
来源：http://ezb.tarul.cn

python -m pytest -q
来源：http://hrp.xuanzx.com

[U32] Py：代码格式化
来源：http://xvm.sweek.top

ruff format . && ruff check --fix .
来源：http://hge.jyoumei.cn

[U33] Py：打包发布
来源：http://yxe.bjfxy.top

python -m build  （依赖 pyproject.toml）
来源：http://zwc.birdmap.top

[U34] Py：判断编码
来源：http://yye.sweek.top

chardet.detect(raw)
来源：http://hdp.haohaochexian.top

[U35] Py：发送邮件
来源：http://dhg.316326.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cuy.shanyushiyangtech.top

[U36] Py：定时任务
来源：http://rqd.ivvv.top

schedule.every(10).minutes.do(job)
来源：http://fnm.ydzc1.top

[U37] Py：读写 Excel
来源：http://pqh.sysykeji.top

pandas.read_excel / DataFrame.to_excel
来源：http://bux.yangfankeji.com

[U38] Py：获取脚本所在目录
来源：http://fjp.pycfn.com

Path(__file__).resolve().parent
来源：http://dfz.guowangkeji.top

[U39] Py：判断是否在交互环境
来源：http://gqj.hongshengwenyu.top

sys.stdout.isatty()
来源：http://ubh.yuanzhike.top

[U40] Py：打印到标准错误
来源：http://exz.nanxinkj.top

print("err", file=sys.stderr)
来源：http://yrx.svipenyu.cn

[U41] PHP：初始化 Composer 项目
来源：http://bpz.yuanzhike.top

composer init;  composer require guzzlehttp/guzzle
来源：http://syu.fehbvm.com

[U42] PHP：PSR-4 自动加载
来源：http://rfq.iojbl.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qqm.yj20258888.top

[U43] PHP：声明命名空间
来源：http://iyt.zhoulong.xyz

namespace App\Http;
来源：http://izc.hywenlv.cn

[U44] PHP：开启严格类型
来源：http://znv.ywan-chungtsiang.top

declare(strict_types=1);
来源：http://pdm.fanxiaobao.xyz

[U45] PHP：类型声明与返回类型
来源：http://ezg.jqgfzy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://moc.shuidangran.top

[U46] PHP：可空类型
来源：http://zyu.xuetiantiany.cn

?string $name = null
来源：http://cfj.yongpay.top

[U47] PHP：联合类型
来源：http://xho.shanyushiyangtech.top

int|string $id
来源：http://uaz.gogol.net.cn

[U48] PHP：纯枚举
来源：http://jin.jqgufenzy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ezt.fzhhl.top

[U49] PHP：只读属性
来源：http://zes.9152youxi.cn

public readonly string $name
来源：http://ykc.havefunace.top

[U50] PHP：构造器属性提升
来源：http://dwd.wangshuangyany.cn

public function __construct(private int $id) {}
来源：http://ozc.vqdsnc.cn

[U51] PHP：数组解构
来源：http://yfe.sysykeji.top

[$a, $b] = $arr;
来源：http://san.shzxlz.cn

[U52] PHP：箭头函数
来源：http://odk.ctjpmb.com

$double = fn($x) => $x * 2;
来源：http://utz.gzhubu.top

[U53] PHP：空合并运算符
来源：http://gic.316326.xyz

$v = $a ?? $b ?? "default";
来源：http://nmv.cdnleiting.top

[U54] PHP：空安全调用
来源：http://atb.smart0.xyz

$obj?->method()
来源：http://yib.gotoacloud.top

[U55] PHP：match 表达式
来源：http://rek.9152youxi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ljp.xingfuxueyuan.xyz

[U56] PHP：命名参数
来源：http://bgg.shzxlz.cn

f(a: 1, b: 2)
来源：http://brq.xylfe.cn

[U57] PHP：字符串插值
来源：http://gjl.fanxiaobao.xyz

"值: {$a}"
来源：http://axt.gaohongyu789.top

[U58] PHP：数组三件套
来源：http://gsr.hnxiangtu.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://czf.nanxuanxn.top

[U59] PHP：自定义排序
来源：http://puh.jyoumei.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mfi.wangshuangyany.cn

[U60] PHP：JSON 编解码
来源：http://gtj.9152youxi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pzn.yvedp.cn

[U61] PHP：正则
来源：http://rip.ctjpmb.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://czx.yj20258888.top

[U62] PHP：日期对象
来源：http://iaz.sjlbkw.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://tpw.gotoacloud.top

[U63] PHP：文件读写
来源：http://kyi.zhaomingkeji.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qyo.jianghu66.top

[U64] PHP：目录遍历
来源：http://phk.hammf.cn

glob("dir/*.php");  scandir("dir");
来源：http://zkm.hammf.cn

[U65] PHP：会话
来源：http://mha.ywan-chungtsiang.top

session_start();  $_SESSION["uid"] = 1;
来源：http://zmi.yfazqb.com

[U66] PHP：设置 Cookie
来源：http://vye.xinyue.icu

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zjx.hfpthk.cn

[U67] PHP：处理文件上传
来源：http://cic.hesvh.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fnj.cqqwz.cn

[U68] PHP：PDO 连接
来源：http://xbf.c1oappe.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://dph.dashuyun.cn

[U69] PHP：PDO 预处理
来源：http://voq.chenjidiqi.icu

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vhq.shuidangran.top

[U70] PHP：PDO 事务
来源：http://aib.cheryme.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://aaw.sysykeji.top

[U71] PHP：抛出异常
来源：http://mcc.c1oappe.top

throw new RuntimeException("失败", 500);
来源：http://mwh.ydjk.org.cn

[U72] PHP：写错误日志
来源：http://jjp.pengpengdd.cyou

error_log("失败: " . $e->getMessage());
来源：http://qvk.shanyushiyangtech.top

[U73] PHP：读取 ini 配置
来源：http://dwi.cheryme.top

parse_ini_file("config.ini", true)
来源：http://lmk.tianlin.xyz

[U74] PHP：读取环境变量
来源：http://tnt.zhiwuduotai.top

getenv("APP_ENV") ?: "production"
来源：http://cdh.fehbvm.com

[U75] PHP：依赖注入
来源：http://yqx.yfazqb.com

composer require psr/container
来源：http://zlo.jqgufenzy.top

[U76] PHP：简单路由
来源：http://fdo.zhaomingkeji.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ohc.epnwcf.com

[U77] PHP：模板渲染
来源：http://rry.ybcxt.top

composer require twig/twig
来源：http://tpx.xuetiantiany.cn

[U78] PHP：单元测试
来源：http://aoj.aizwys.cn

composer require --dev phpunit/phpunit
来源：http://nma.ppjwa.cn

[U79] PHP：静态分析
来源：http://auy.aibaodan.cn

composer require --dev phpstan/phpstan
来源：http://szl.yj20258888.top

[U80] PHP：代码规范修复
来源：http://yrc.shangyingyoupin.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://lme.jinqigufen.top

[U81] JS：初始化项目
来源：http://jif.zhiwuduotai.top

npm init -y;  npm i express
来源：http://cgn.xingfuxueyuan.xyz

[U82] JS：package.json 脚本
来源：http://lip.guowangkeji.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nrn.xuanzx.com

[U83] JS：ES Module 导入导出
来源：http://uyy.jiagoushi.top

export const a = 1;  import { a } from "./m.js";
来源：http://odu.hesvh.cn

[U84] JS：CommonJS 写法
来源：http://ous.chenzaomai.com

module.exports = { a };  const { a } = require("./m");
来源：http://gfq.pycfn.com

[U85] JS：可选链
来源：http://ypi.xuetiantiany.cn

a?.b?.c
来源：http://nil.zhongyouzk.top

[U86] JS：空值合并
来源：http://ojd.ydjk.org.cn

a ?? b
来源：http://ecb.jianghu66.top

[U87] JS：解构默认值
来源：http://yxl.cucudq.cn

const { a = 1, b = 2 } = obj;
来源：http://qvy.shuidangran.top

[U88] JS：对象展开合并
来源：http://dec.yueranfly.top

{ ...a, ...b }
来源：http://nvx.redwolf501.top

[U89] JS：数组去重
来源：http://yrp.zdbjq.cn

[...new Set(arr)]
来源：http://rve.shangyingyoupin.top

[U90] JS：数字数组排序
来源：http://wln.gzhubu.top

[...arr].sort((a, b) => a - b)
来源：http://nrd.fehbvm.com

[U91] JS：对象键值遍历
来源：http://ofv.tarul.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gkk.jianghu66.top

[U92] JS：深拷贝
来源：http://gts.hysaishi.cn

structuredClone(obj)
来源：http://lsi.hammf.cn

[U93] JS：模板字符串
来源：http://odc.smart0.xyz

`共 ${n} 条`
来源：http://aqj.yj202588.top

[U94] JS：箭头函数
来源：http://awl.tian-w.cn

const double = x => x * 2;
来源：http://zog.zhiwuduotai.top

[U95] JS：Promise 包装
来源：http://cea.c1oappe.top

new Promise((resolve, reject) => {})
来源：http://nis.haohaochexian.top

[U96] JS：async/await 与异常
来源：http://kpv.nanxinkj.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ypt.quarkkingdee.top

[U97] JS：并发请求
来源：http://aoe.fzhhl.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://rfk.shanyushiyangkeji.top

[U98] JS：fetch 带 JSON
来源：http://crh.hysaishi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qbs.gogol.net.cn

[U99] JS：事件监听
来源：http://xtd.ppjwa.cn

el.addEventListener("click", e => {})
来源：http://rhz.hongshengwenyu.top

[U100] JS：DOM 查询
来源：http://sjp.dashuyun.cn

document.querySelector(".item")
来源：http://jmb.tian-w.cn

[U101] JS：classList 操作
来源：http://zlv.mhx1999.top

el.classList.toggle("active")
来源：http://gra.gaohongyu789.top

[U102] JS：本地存储
来源：http://sis.cheryme.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://lnl.jiagoushi.top

[U103] JS：定时器
来源：http://cys.yongpay.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ipo.xylfe.cn

[U104] JS：防抖
来源：http://rmw.sjlbkw.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hml.ywan-chungtsiang.top

[U105] JS：节流
来源：http://two.sxryk.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hil.nanxinkj.top

[U106] JS：日期格式化
来源：http://hfr.uphjek.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zgf.zhiwuduotai.top

[U107] JS：数字千分位
来源：http://uag.nanxinkj.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zij.yj20258.top

[U108] JS：随机整数
来源：http://jbx.c1oappe.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nrl.pycfn.com

[U109] JS：数组分组
来源：http://azj.xinyue.icu

Object.groupBy(arr, x => x.type)
来源：http://wgi.ehwqpu.com

[U110] JS：数组分块
来源：http://ixu.mhx1999.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rzk.hesvh.cn

[U111] JS：对象转 Map
来源：http://nnt.sweek.top

new Map(Object.entries(obj))
来源：http://fcs.havefunace.top

[U112] JS：字符串补位
来源：http://fnf.jinqigufen.top

"7".padStart(3, "0")
来源：http://ows.wangdashe.top

[U113] JS：正则替换全部
来源：http://kfr.dianchejie.cn

s.replaceAll("a", "b")
来源：http://jwt.yongpay.top

[U114] JS：JSON 深比较
来源：http://bxu.zdbjq.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://nlo.jyoumei.cn

[U115] JS：生成 UUID
来源：http://txa.andypj.xyz

crypto.randomUUID()
来源：http://bwp.tian-w.cn

[U116] JS：类型检查（JSDoc）
来源：http://pbp.nanxinkj.top

/** @param {string} name */ function f(name) {}
来源：http://yii.jyoumei.cn

[U117] JS：单元测试
来源：http://qye.fzhhl.top

npm i -D vitest;  npx vitest
来源：http://nkc.fzhhl.top

[U118] JS：开发服务器
来源：http://zrl.redwolf501.top

npm i -D vite;  npx vite
来源：http://ajo.ctjpmb.com

[U119] JS：生产构建
来源：http://tcr.ywan-chungtsiang.top

npx vite build
来源：http://mbk.jqgfzy.top

[U120] JS：读取环境变量（Vite）
来源：http://vyu.xuanzx.com

import.meta.env.VITE_API_URL
来源：http://mjq.yj202588.top

================================================================================
来源：http://zqf.yueranfly.top

统计汇总
来源：http://foj.xuetiantiany.cn

================================================================================
来源：http://rov.chenzaomai.com

按语言统计（条）：
来源：http://vof.tian-w.cn

Python ......... 252
来源：http://jwr.gzhubu.top

PHP ............ 252
来源：http://jun.zhixingplan.top

JavaScript ..... 252
来源：http://ude.fanxiaobao.xyz

TypeScript ..... 212
来源：http://oab.c1oappe.top

Java ........... 212
来源：http://fgb.feifeiyinyue.top

Go ............. 212
来源：http://war.ydzc1.top

Ruby ........... 212
来源：http://zwp.shangyingyoupin.top

C# ............. 212
来源：http://taq.jinqigfzy.top

C .............. 30
来源：http://ygp.zhijiandao.cn

C++ ............ 30
来源：http://sef.xziqi.cn

SQL ............ 90
来源：http://pic.gogol.net.cn

Bash ........... 80
来源：http://oyz.fengsongda.top

Kotlin ......... 15
来源：http://rsw.c1oappe.top

Swift .......... 15
来源：http://nzx.0kj1m.cn

Lua ............ 10
来源：http://fxn.jinqigufen.top

Perl ........... 10
来源：http://uvm.nanxuanxn.top

Scala .......... 10
来源：http://irb.yuanzhike.top

------------------------------------
来源：http://hld.jiagoushi.top

合计 ........... 2106 条
来源：http://kup.ybcxt.top

按章节统计：
来源：http://cgj.zhongyouzk.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hlo.yongpay.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hle.ehwqpu.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://olm.yangfankeji.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mox.hesvh.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://edo.ctjpmb.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://tfu.xingfuxueyuan.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wor.fktsv.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hsd.zdbjq.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://aze.vehdjk.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://pkl.sjlbkw.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bin.0kj1m.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fpo.andypj.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://xyq.ydjk.org.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://gsy.yongpay.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://omn.xuanzx.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://zet.zhengqikj.top

Q SQL 专题                              90
来源：http://cfy.ydjk.org.cn

R Bash 专题                             80
来源：http://qvz.chenjidiqi.icu

S C / C++ 专题                          60
来源：http://jkc.vehdjk.com

T 其他语言补充                          60
来源：http://cru.xuetiantiany.cn

U 高频实用片段                         120
来源：http://aqa.9152youxi.cn

------------------------------------
来源：http://nxc.jinyuanbaomall.cn

合计                                  2106 条
来源：http://avn.nanxinkj.top

--------------------------------------------------------------------------------
来源：http://lxh.yfazqb.com

使用提醒
来源：http://xmp.hfpthk.cn

--------------------------------------------------------------------------------
来源：http://xmh.gaohongyu789.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qyt.xuanzx.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xfv.jyoumei.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ifi.yvedp.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://uto.pycfn.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://vse.fktsv.cn

—— 文件结束 ——
来源：http://kex.yanxiufei.cn

================================================================================
来源：http://tyr.xziqi.cn

程序语言常见例子速查手册（2024 版）
来源：http://kor.cheryme.top

Common Programming Examples Cheat Book
来源：http://uhq.wangshuangyany.cn

================================================================================
来源：http://jrb.pengpengdd.cyou

【收录内容】
来源：http://wle.guowangkeji.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ufz.dianchejie.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tuk.tanke756.top

SQL · Bash · C · C++
来源：http://smu.hesvh.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jbh.zhiwuduotai.top

【使用说明】
来源：http://sad.cqqwz.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://nvz.52xcode.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://jzg.gzhubu.top


<!-- 参考信息 -->