代发 wailian999

[U15] Py：高精度计时
来源：http://lbg.chenjidiqi.icu

t = time.perf_counter()
来源：http://cwh.yonumen.top

[U16] Py：命令行参数解析
来源：http://jpv.xziqi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://amk.zhixingplan.top

[U17] Py：初始化日志
来源：http://xdh.zhengqikj.top

logging.basicConfig(level=logging.INFO)
来源：http://dnv.guowangkeji.top

[U18] Py：预编译正则
来源：http://ljb.ybcxt.top

pat = re.compile(r"\d+")
来源：http://wme.yonumen.top

[U19] Py：正则替换带回调
来源：http://auy.sjlbkw.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tlm.ybcxt.top

[U20] Py：缓存函数结果
来源：http://wrn.quarkkingdee.top

@functools.lru_cache(maxsize=None)
来源：http://xks.epnwcf.com

[U21] Py：自定义上下文管理器
来源：http://etc.yueranfly.top

@contextlib.contextmanager
来源：http://pva.chenlongwang.top

[U22] Py：矩阵转置
来源：http://pgh.cqqwz.cn

list(zip(*m))
来源：http://hoy.chenzaomai.com

[U23] Py：分块读取大文件
来源：http://fwm.zhengqikj.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vll.yuxming.cn

[U24] Py：路径操作
来源：http://uog.zhixingplan.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ijv.tian-w.cn

[U25] Py：CSV 按字典读
来源：http://vsy.hesvh.cn

csv.DictReader(f)
来源：http://sle.yongpay.top

[U26] Py：并发下载
来源：http://aor.hysaishi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zhg.fanxiaobao.xyz

[U27] Py：异步 HTTP
来源：http://ywq.aibaodan.cn

aiohttp.ClientSession() 配合 async with
来源：http://bdb.xziqi.cn

[U28] Py：类型别名
来源：http://lzc.ivvv.top

UserId = int
来源：http://ysa.0kj1m.cn

[U29] Py：属性校验
来源：http://jtt.ppjwa.cn

@property 与 @x.setter 配合
来源：http://qpn.daria6918.cn

[U30] Py：数据类
来源：http://gcj.hywenlv.cn

@dataclass(slots=True)
来源：http://sra.meibo888.top

[U31] Py：单测
来源：http://vno.nanxuanxn.top

python -m pytest -q
来源：http://dgy.xuanzx.com

[U32] Py：代码格式化
来源：http://anq.ydjk.org.cn

ruff format . && ruff check --fix .
来源：http://xiz.yanxiufei.cn

[U33] Py：打包发布
来源：http://mpb.jyoumei.cn

python -m build  （依赖 pyproject.toml）
来源：http://hrf.dashuyun.cn

[U34] Py：判断编码
来源：http://lwj.316326.xyz

chardet.detect(raw)
来源：http://xhb.zhongyouzk.top

[U35] Py：发送邮件
来源：http://ydd.yongpay.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qns.tian-w.cn

[U36] Py：定时任务
来源：http://xft.zhongyouzk.top

schedule.every(10).minutes.do(job)
来源：http://aee.quarkkingdee.top

[U37] Py：读写 Excel
来源：http://cpy.shangyingyoupin.top

pandas.read_excel / DataFrame.to_excel
来源：http://myb.iojbl.cn

[U38] Py：获取脚本所在目录
来源：http://zhd.mhx1999.top

Path(__file__).resolve().parent
来源：http://inv.nanxinkj.top

[U39] Py：判断是否在交互环境
来源：http://kat.zhoulong.xyz

sys.stdout.isatty()
来源：http://rvu.yj202588.top

[U40] Py：打印到标准错误
来源：http://tag.ivvv.top

print("err", file=sys.stderr)
来源：http://gci.zhongyouzk.top

[U41] PHP：初始化 Composer 项目
来源：http://qsm.jinghuilouyu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://gpp.mhx1999.top

[U42] PHP：PSR-4 自动加载
来源：http://knk.nwbrower.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yat.haohaochexian.top

[U43] PHP：声明命名空间
来源：http://rtb.9152youxi.cn

namespace App\Http;
来源：http://ief.tian-w.cn

[U44] PHP：开启严格类型
来源：http://ygq.meibo888.top

declare(strict_types=1);
来源：http://ixv.feifeiyinyue.top

[U45] PHP：类型声明与返回类型
来源：http://dxt.ydzc1.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://gcl.shzxlz.cn

[U46] PHP：可空类型
来源：http://cmi.yuxming.cn

?string $name = null
来源：http://rpa.aizwys.cn

[U47] PHP：联合类型
来源：http://znl.xinyue.icu

int|string $id
来源：http://ydi.yuxming.cn

[U48] PHP：纯枚举
来源：http://jnz.haohaochexian.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zva.meibo888.top

[U49] PHP：只读属性
来源：http://wyy.tanke756.top

public readonly string $name
来源：http://ogr.yj20258888.top

[U50] PHP：构造器属性提升
来源：http://ola.zhaomingkeji.xyz

public function __construct(private int $id) {}
来源：http://vrn.ydjk.org.cn

[U51] PHP：数组解构
来源：http://xsc.pengpengdd.cyou

[$a, $b] = $arr;
来源：http://xes.shuidangran.top

[U52] PHP：箭头函数
来源：http://hpm.fzhhl.top

$double = fn($x) => $x * 2;
来源：http://opo.ybcxt.top

[U53] PHP：空合并运算符
来源：http://spf.chenlongwang.top

$v = $a ?? $b ?? "default";
来源：http://xmb.tianlin.xyz

[U54] PHP：空安全调用
来源：http://wcs.nanxuanxn.top

$obj?->method()
来源：http://ouc.xuetiantiany.cn

[U55] PHP：match 表达式
来源：http://deb.xziqi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://iap.cucudq.cn

[U56] PHP：命名参数
来源：http://xhm.zdbjq.cn

f(a: 1, b: 2)
来源：http://mnt.shuidangran.top

[U57] PHP：字符串插值
来源：http://uze.yj202588.top

"值: {$a}"
来源：http://njt.daxiang520.top

[U58] PHP：数组三件套
来源：http://fwy.52xcode.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rjd.zhengqikj.top

[U59] PHP：自定义排序
来源：http://nuc.havefunace.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gww.zhixingplan.top

[U60] PHP：JSON 编解码
来源：http://qqj.daxiang520.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://uln.haohaochexian.top

[U61] PHP：正则
来源：http://eeo.hnqzz.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tuw.redwolf501.top

[U62] PHP：日期对象
来源：http://jtl.guowangkeji.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xvc.ydzc1.top

[U63] PHP：文件读写
来源：http://mxb.birdmap.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dyb.zhoulong.xyz

[U64] PHP：目录遍历
来源：http://civ.shzxlz.cn

glob("dir/*.php");  scandir("dir");
来源：http://cia.smart0.xyz

[U65] PHP：会话
来源：http://hja.yuanzhike.top

session_start();  $_SESSION["uid"] = 1;
来源：http://qkj.kuanghao11.cn

[U66] PHP：设置 Cookie
来源：http://syx.hongshengwenyu.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qhm.gotoacloud.top

[U67] PHP：处理文件上传
来源：http://qto.jinqigfzy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://thc.xingfuxueyuan.xyz

[U68] PHP：PDO 连接
来源：http://mff.svipenyu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jri.gzhubu.top

[U69] PHP：PDO 预处理
来源：http://knz.vqdsnc.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dtq.wangshuangyany.cn

[U70] PHP：PDO 事务
来源：http://ukq.xuanzx.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://heu.guowangkeji.top

[U71] PHP：抛出异常
来源：http://fba.hcnkem.com

throw new RuntimeException("失败", 500);
来源：http://otb.andypj.xyz

[U72] PHP：写错误日志
来源：http://gmz.xuetiantiany.cn

error_log("失败: " . $e->getMessage());
来源：http://pms.vqdsnc.cn

[U73] PHP：读取 ini 配置
来源：http://nmi.uphjek.com

parse_ini_file("config.ini", true)
来源：http://xio.aibaodan.cn

[U74] PHP：读取环境变量
来源：http://mwu.hfpthk.cn

getenv("APP_ENV") ?: "production"
来源：http://qav.tarul.cn

[U75] PHP：依赖注入
来源：http://bpy.jinqigfzy.top

composer require psr/container
来源：http://uju.xuanzx.com

[U76] PHP：简单路由
来源：http://cqe.fktsv.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xzg.xylfe.cn

[U77] PHP：模板渲染
来源：http://wfe.vehdjk.com

composer require twig/twig
来源：http://raz.yangfankeji.com

[U78] PHP：单元测试
来源：http://tkn.bbcook.cn

composer require --dev phpunit/phpunit
来源：http://kla.zhengqikj.top

[U79] PHP：静态分析
来源：http://zzu.yj20258.top

composer require --dev phpstan/phpstan
来源：http://kfm.sufxvd.cn

[U80] PHP：代码规范修复
来源：http://nbs.iojbl.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://soj.guowangkeji.top

[U81] JS：初始化项目
来源：http://srl.jyoumei.cn

npm init -y;  npm i express
来源：http://lba.sweek.top

[U82] JS：package.json 脚本
来源：http://agy.xziqi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nwu.ywan-chungtsiang.top

[U83] JS：ES Module 导入导出
来源：http://hbp.jqgfzy.top

export const a = 1;  import { a } from "./m.js";
来源：http://qmo.hammf.cn

[U84] JS：CommonJS 写法
来源：http://onf.sufxvd.cn

module.exports = { a };  const { a } = require("./m");
来源：http://jzy.bbcook.cn

[U85] JS：可选链
来源：http://gra.chenlongwang.top

a?.b?.c
来源：http://dqn.quarkkingdee.top

[U86] JS：空值合并
来源：http://wfq.xuetiantiany.cn

a ?? b
来源：http://hhx.nwbrower.top

[U87] JS：解构默认值
来源：http://sos.52xcode.cn

const { a = 1, b = 2 } = obj;
来源：http://xyj.hammf.cn

[U88] JS：对象展开合并
来源：http://fpn.ybcxt.top

{ ...a, ...b }
来源：http://qsb.wangshuangyany.cn

[U89] JS：数组去重
来源：http://asx.haohaochexian.top

[...new Set(arr)]
来源：http://lkx.kuanghao11.cn

[U90] JS：数字数组排序
来源：http://iwd.yueranfly.top

[...arr].sort((a, b) => a - b)
来源：http://fqx.ppjwa.cn

[U91] JS：对象键值遍历
来源：http://mws.jinqigufen.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ill.guowangkeji.top

[U92] JS：深拷贝
来源：http://gzm.hammf.cn

structuredClone(obj)
来源：http://tfu.sjlbkw.cn

[U93] JS：模板字符串
来源：http://szh.yuanzhike.top

`共 ${n} 条`
来源：http://naz.52xcode.cn

[U94] JS：箭头函数
来源：http://vmc.yvedp.cn

const double = x => x * 2;
来源：http://bwj.sxryk.cn

[U95] JS：Promise 包装
来源：http://tmg.hongshengwenyu.top

new Promise((resolve, reject) => {})
来源：http://usp.316326.xyz

[U96] JS：async/await 与异常
来源：http://rkk.epnwcf.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://uhw.chenlongwang.top

[U97] JS：并发请求
来源：http://uep.jianghu66.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://aaa.andypj.xyz

[U98] JS：fetch 带 JSON
来源：http://mgu.xuetiantiany.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ovw.gzhubu.top

[U99] JS：事件监听
来源：http://nhi.meibo888.top

el.addEventListener("click", e => {})
来源：http://vet.shangyingyoupin.top

[U100] JS：DOM 查询
来源：http://uwm.jyoumei.cn

document.querySelector(".item")
来源：http://qrv.52xcode.cn

[U101] JS：classList 操作
来源：http://jkz.zycfv.cn

el.classList.toggle("active")
来源：http://dym.ybcxt.top

[U102] JS：本地存储
来源：http://vdb.hnxiangtu.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://mtd.316326.xyz

[U103] JS：定时器
来源：http://dkw.smart0.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ktp.guannengcc.top

[U104] JS：防抖
来源：http://wht.hnxiangtu.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pnp.hywenlv.cn

[U105] JS：节流
来源：http://pcu.zdbjq.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bxe.quarkkingdee.top

[U106] JS：日期格式化
来源：http://udc.havefunace.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wfe.zhongyouzk.top

[U107] JS：数字千分位
来源：http://zuy.zhixingplan.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://swm.guannengcc.top

[U108] JS：随机整数
来源：http://cbl.pengpengdd.cyou

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qfl.ctjpmb.com

[U109] JS：数组分组
来源：http://pgy.aizwys.cn

Object.groupBy(arr, x => x.type)
来源：http://vjf.yonumen.top

[U110] JS：数组分块
来源：http://nhx.tanke756.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tvy.fzhhl.top

[U111] JS：对象转 Map
来源：http://qel.jinqigfzy.top

new Map(Object.entries(obj))
来源：http://bnw.zhijiandao.cn

[U112] JS：字符串补位
来源：http://acs.zhoulong.xyz

"7".padStart(3, "0")
来源：http://snk.nwbrower.top

[U113] JS：正则替换全部
来源：http://wyl.yuanzhike.top

s.replaceAll("a", "b")
来源：http://cco.guannengcc.top

[U114] JS：JSON 深比较
来源：http://qvr.ivvv.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://kuq.bjfxy.top

[U115] JS：生成 UUID
来源：http://srg.vehdjk.com

crypto.randomUUID()
来源：http://mdf.hysaishi.cn

[U116] JS：类型检查（JSDoc）
来源：http://vrq.hesvh.cn

/** @param {string} name */ function f(name) {}
来源：http://qqt.52xcode.cn

[U117] JS：单元测试
来源：http://tyx.bbcook.cn

npm i -D vitest;  npx vitest
来源：http://xeu.haohaochexian.top

[U118] JS：开发服务器
来源：http://vuo.hnqzz.top

npm i -D vite;  npx vite
来源：http://xpj.316326.xyz

[U119] JS：生产构建
来源：http://mrh.daria6918.cn

npx vite build
来源：http://qyv.aizwys.cn

[U120] JS：读取环境变量（Vite）
来源：http://gqo.tarul.cn

import.meta.env.VITE_API_URL
来源：http://dwv.bbcook.cn

================================================================================
来源：http://qnu.jiagoushi.top

统计汇总
来源：http://bra.yuxming.cn

================================================================================
来源：http://vgx.yangfankeji.com

按语言统计（条）：
来源：http://lek.daria6918.cn

Python ......... 252
来源：http://cps.316326.xyz

PHP ............ 252
来源：http://qvt.ppjwa.cn

JavaScript ..... 252
来源：http://nyt.fzhhl.top

TypeScript ..... 212
来源：http://tao.xinyue.icu

Java ........... 212
来源：http://jxl.ivvv.top

Go ............. 212
来源：http://efq.jinqigufen.top

Ruby ........... 212
来源：http://dwc.fktsv.cn

C# ............. 212
来源：http://jri.hcnkem.com

C .............. 30
来源：http://enp.aibaodan.cn

C++ ............ 30
来源：http://yoa.ctjpmb.com

SQL ............ 90
来源：http://bdr.yonumen.top

Bash ........... 80
来源：http://jjq.smart0.xyz

Kotlin ......... 15
来源：http://uxb.nanxinkj.top

Swift .......... 15
来源：http://ooy.redwolf501.top

Lua ............ 10
来源：http://kyn.fktsv.cn

Perl ........... 10
来源：http://ypt.yanxiufei.cn

Scala .......... 10
来源：http://qfd.0kj1m.cn

------------------------------------
来源：http://qlw.cashguo.top

合计 ........... 2106 条
来源：http://quy.iojbl.cn

按章节统计：
来源：http://njy.quarkkingdee.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://lvu.hnqzz.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://whx.sufxvd.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://yal.ehwqpu.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qvw.chenzaomai.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dbe.hnxiangtu.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zdn.shangyingyoupin.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zxp.vehdjk.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://pbw.c1oappe.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://foe.chenzaomai.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vvb.zhoulong.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kxq.yfazqb.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mgh.yuanzhike.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bxs.chenjidiqi.icu

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ihw.svipenyu.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zpp.sufxvd.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://zrs.hongshengwenyu.top

Q SQL 专题                              90
来源：http://kip.yj20258888.top

R Bash 专题                             80
来源：http://fdg.zhijiandao.cn

S C / C++ 专题                          60
来源：http://hjr.jlsjyb.cn

T 其他语言补充                          60
来源：http://jnr.yueranfly.top

U 高频实用片段                         120
来源：http://ick.jiagoushi.top

------------------------------------
来源：http://hxt.52xcode.cn

合计                                  2106 条
来源：http://eie.hammf.cn

--------------------------------------------------------------------------------
来源：http://ljs.fktsv.cn

使用提醒
来源：http://yvj.nanxinkj.top

--------------------------------------------------------------------------------
来源：http://chn.xylfe.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://tzc.gaohongyu789.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://oej.zhaomingkeji.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://agu.zhijiandao.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://xyw.jlsjyb.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://llq.nanxuanxn.top

—— 文件结束 ——
来源：http://jbn.yueranfly.top

================================================================================
来源：http://bgd.jyoumei.cn

程序语言常见例子速查手册（2024 版）
来源：http://cwh.birdmap.top

Common Programming Examples Cheat Book
来源：http://pdk.chenlongwang.top

================================================================================
来源：http://klw.yuxming.cn

【收录内容】
来源：http://tnq.yongpay.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ior.meibo888.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://yyk.fengsongda.top

SQL · Bash · C · C++
来源：http://xbv.cqqwz.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://bpr.smart0.xyz

【使用说明】
来源：http://bfx.pengpengdd.cyou

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://txd.ivvv.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wxd.quarkkingdee.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ztn.zycfv.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://lng.feifeiyinyue.top

Bash:  Shell         C:     C             C++:   C++
来源：http://xoy.bjfxy.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://dii.tianlin.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://xfg.jinghuilouyu.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://bti.nanxinkj.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ceb.jinghuilouyu.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jel.dianchejie.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://fdx.meibo888.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://xxc.yvedp.cn

【文件统计】
来源：http://wac.ywan-chungtsiang.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ilf.jiagoushi.top

--------------------------------------------------------------------------------
来源：http://kyy.tianlin.xyz

目  录
来源：http://ewk.52xcode.cn

--------------------------------------------------------------------------------
来源：http://xli.ydzc1.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ejm.gotoacloud.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://jlq.aizwys.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fvp.andypj.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://rfd.iojbl.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://aln.feifeiyinyue.top


<!-- 参考信息 -->