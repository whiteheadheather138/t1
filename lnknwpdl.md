代发 wailian999

[U13] Py：固定长度队列
来源：http://bqo.haohaochexian.top

deque(maxlen=10)
来源：http://dzz.xuetiantiany.cn

[U14] Py：分组收集到列表
来源：http://tfm.zhoulong.xyz

defaultdict(list)
来源：http://fez.cqqwz.cn

[U15] Py：高精度计时
来源：http://uwn.9152youxi.cn

t = time.perf_counter()
来源：http://qtn.fktsv.cn

[U16] Py：命令行参数解析
来源：http://zux.zhijiandao.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ckm.9152youxi.cn

[U17] Py：初始化日志
来源：http://asz.jyoumei.cn

logging.basicConfig(level=logging.INFO)
来源：http://eaj.gaohongyu789.top

[U18] Py：预编译正则
来源：http://enr.sjlbkw.cn

pat = re.compile(r"\d+")
来源：http://nhz.vehdjk.com

[U19] Py：正则替换带回调
来源：http://hnp.wangdashe.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ebg.tanke756.top

[U20] Py：缓存函数结果
来源：http://tgx.sufxvd.cn

@functools.lru_cache(maxsize=None)
来源：http://qcj.iojbl.cn

[U21] Py：自定义上下文管理器
来源：http://fjg.ybcxt.top

@contextlib.contextmanager
来源：http://zzm.ydzc1.top

[U22] Py：矩阵转置
来源：http://hwu.nanxinkj.top

list(zip(*m))
来源：http://upb.zdbjq.cn

[U23] Py：分块读取大文件
来源：http://vxe.jlsjyb.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ufk.gotoacloud.top

[U24] Py：路径操作
来源：http://rir.sufxvd.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bwx.zhijiandao.cn

[U25] Py：CSV 按字典读
来源：http://nym.hnxiangtu.top

csv.DictReader(f)
来源：http://gpi.mhx1999.top

[U26] Py：并发下载
来源：http://aig.kuanghao11.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://glq.hesvh.cn

[U27] Py：异步 HTTP
来源：http://xxt.yueranfly.top

aiohttp.ClientSession() 配合 async with
来源：http://jcw.hysaishi.cn

[U28] Py：类型别名
来源：http://quz.zhiwuduotai.top

UserId = int
来源：http://eup.yfazqb.com

[U29] Py：属性校验
来源：http://vch.gogol.net.cn

@property 与 @x.setter 配合
来源：http://jde.chenlongwang.top

[U30] Py：数据类
来源：http://vnu.zycfv.cn

@dataclass(slots=True)
来源：http://dlu.shzxlz.cn

[U31] Py：单测
来源：http://taf.xylfe.cn

python -m pytest -q
来源：http://yxz.ybcxt.top

[U32] Py：代码格式化
来源：http://rdq.zhixingplan.top

ruff format . && ruff check --fix .
来源：http://pdg.zdbjq.cn

[U33] Py：打包发布
来源：http://kax.hongshengwenyu.top

python -m build  （依赖 pyproject.toml）
来源：http://gxi.ybcxt.top

[U34] Py：判断编码
来源：http://kjy.andypj.xyz

chardet.detect(raw)
来源：http://hgj.xylfe.cn

[U35] Py：发送邮件
来源：http://kms.sweek.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qts.hfpthk.cn

[U36] Py：定时任务
来源：http://stu.xuanzx.com

schedule.every(10).minutes.do(job)
来源：http://ivd.xingfuxueyuan.xyz

[U37] Py：读写 Excel
来源：http://aqc.xinyue.icu

pandas.read_excel / DataFrame.to_excel
来源：http://qpl.iojbl.cn

[U38] Py：获取脚本所在目录
来源：http://typ.guannengcc.top

Path(__file__).resolve().parent
来源：http://wui.shanyushiyangtech.top

[U39] Py：判断是否在交互环境
来源：http://msm.sweek.top

sys.stdout.isatty()
来源：http://kfp.hnxiangtu.top

[U40] Py：打印到标准错误
来源：http://rpo.aibaodan.cn

print("err", file=sys.stderr)
来源：http://oxm.shanyushiyangkeji.top

[U41] PHP：初始化 Composer 项目
来源：http://tfp.hnxiangtu.top

composer init;  composer require guzzlehttp/guzzle
来源：http://wgy.hywenlv.cn

[U42] PHP：PSR-4 自动加载
来源：http://aqa.cucudq.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xux.sysykeji.top

[U43] PHP：声明命名空间
来源：http://gxn.havefunace.top

namespace App\Http;
来源：http://mbr.jinqigfzy.top

[U44] PHP：开启严格类型
来源：http://mfk.jlsjyb.cn

declare(strict_types=1);
来源：http://bhz.sufxvd.cn

[U45] PHP：类型声明与返回类型
来源：http://ipm.yonumen.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://woe.cashguo.top

[U46] PHP：可空类型
来源：http://ayq.0kj1m.cn

?string $name = null
来源：http://wwp.gogol.net.cn

[U47] PHP：联合类型
来源：http://xwg.wangshuangyany.cn

int|string $id
来源：http://ejc.zdbjq.cn

[U48] PHP：纯枚举
来源：http://noq.ywan-chungtsiang.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dzu.nanxinkj.top

[U49] PHP：只读属性
来源：http://zss.guannengcc.top

public readonly string $name
来源：http://xri.bjfxy.top

[U50] PHP：构造器属性提升
来源：http://rbq.vqdsnc.cn

public function __construct(private int $id) {}
来源：http://uir.zhengqikj.top

[U51] PHP：数组解构
来源：http://nbd.nanxuanxn.top

[$a, $b] = $arr;
来源：http://qvq.gotoacloud.top

[U52] PHP：箭头函数
来源：http://tjx.fktsv.cn

$double = fn($x) => $x * 2;
来源：http://dbt.aizwys.cn

[U53] PHP：空合并运算符
来源：http://ngj.andypj.xyz

$v = $a ?? $b ?? "default";
来源：http://jpx.shanyushiyangtech.top

[U54] PHP：空安全调用
来源：http://qvf.yj202588.top

$obj?->method()
来源：http://onu.dashuyun.cn

[U55] PHP：match 表达式
来源：http://zbs.tarul.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://meu.iojbl.cn

[U56] PHP：命名参数
来源：http://uhk.xuanzx.com

f(a: 1, b: 2)
来源：http://tnj.shuidangran.top

[U57] PHP：字符串插值
来源：http://bne.cdnleiting.top

"值: {$a}"
来源：http://fia.ivvv.top

[U58] PHP：数组三件套
来源：http://ojl.yonumen.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://uwy.sufxvd.cn

[U59] PHP：自定义排序
来源：http://nxt.yj202588.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ptr.fengsongda.top

[U60] PHP：JSON 编解码
来源：http://knb.bbcook.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zmp.tian-w.cn

[U61] PHP：正则
来源：http://mio.xinyue.icu

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://szd.zdbjq.cn

[U62] PHP：日期对象
来源：http://bxy.gogol.net.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://eqo.tian-w.cn

[U63] PHP：文件读写
来源：http://wbm.yonumen.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gqp.yanxiufei.cn

[U64] PHP：目录遍历
来源：http://iec.zdbjq.cn

glob("dir/*.php");  scandir("dir");
来源：http://xlt.cheryme.top

[U65] PHP：会话
来源：http://lfv.mhx1999.top

session_start();  $_SESSION["uid"] = 1;
来源：http://nal.yfazqb.com

[U66] PHP：设置 Cookie
来源：http://qje.havefunace.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pzd.chenzaomai.com

[U67] PHP：处理文件上传
来源：http://wvn.9152youxi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hgx.zhoulong.xyz

[U68] PHP：PDO 连接
来源：http://cso.zdqjudy.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://akr.yj20258888.top

[U69] PHP：PDO 预处理
来源：http://hqy.gzhubu.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nhv.jinqigufen.top

[U70] PHP：PDO 事务
来源：http://dro.sysykeji.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://iek.jqgufenzy.top

[U71] PHP：抛出异常
来源：http://yvg.tarul.cn

throw new RuntimeException("失败", 500);
来源：http://owi.ivvv.top

[U72] PHP：写错误日志
来源：http://yey.xinyue.icu

error_log("失败: " . $e->getMessage());
来源：http://lsv.andypj.xyz

[U73] PHP：读取 ini 配置
来源：http://kdj.cashguo.top

parse_ini_file("config.ini", true)
来源：http://okx.gaohongyu789.top

[U74] PHP：读取环境变量
来源：http://cil.xziqi.cn

getenv("APP_ENV") ?: "production"
来源：http://gwj.birdmap.top

[U75] PHP：依赖注入
来源：http://bbt.tanke756.top

composer require psr/container
来源：http://fjn.zhongyouzk.top

[U76] PHP：简单路由
来源：http://gcx.dashuyun.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zow.xinyue.icu

[U77] PHP：模板渲染
来源：http://srs.zycfv.cn

composer require twig/twig
来源：http://oek.shangyingyoupin.top

[U78] PHP：单元测试
来源：http://wwx.shanyushiyangtech.top

composer require --dev phpunit/phpunit
来源：http://qel.gotoacloud.top

[U79] PHP：静态分析
来源：http://mdm.tian-w.cn

composer require --dev phpstan/phpstan
来源：http://mdv.yj20258888.top

[U80] PHP：代码规范修复
来源：http://skd.bjfxy.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://lzj.zdqjudy.top

[U81] JS：初始化项目
来源：http://zfh.cashguo.top

npm init -y;  npm i express
来源：http://bua.meibo888.top

[U82] JS：package.json 脚本
来源：http://rbd.52xcode.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mso.ydzc1.top

[U83] JS：ES Module 导入导出
来源：http://uoy.daria6918.cn

export const a = 1;  import { a } from "./m.js";
来源：http://mmj.sweek.top

[U84] JS：CommonJS 写法
来源：http://lfw.shanyushiyangtech.top

module.exports = { a };  const { a } = require("./m");
来源：http://nkd.bjfxy.top

[U85] JS：可选链
来源：http://sck.vqdsnc.cn

a?.b?.c
来源：http://ksd.kuanghao11.cn

[U86] JS：空值合并
来源：http://ugv.jinqigufen.top

a ?? b
来源：http://dnm.ehwqpu.com

[U87] JS：解构默认值
来源：http://fla.tarul.cn

const { a = 1, b = 2 } = obj;
来源：http://btl.ydjk.org.cn

[U88] JS：对象展开合并
来源：http://cfz.hnqzz.top

{ ...a, ...b }
来源：http://qbd.chenlongwang.top

[U89] JS：数组去重
来源：http://jaa.ydzc1.top

[...new Set(arr)]
来源：http://qbi.jinyuanbaomall.cn

[U90] JS：数字数组排序
来源：http://fui.fengsongda.top

[...arr].sort((a, b) => a - b)
来源：http://rub.fktsv.cn

[U91] JS：对象键值遍历
来源：http://nen.hcnkem.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://owa.cucudq.cn

[U92] JS：深拷贝
来源：http://gwd.jianghu66.top

structuredClone(obj)
来源：http://zct.yueranfly.top

[U93] JS：模板字符串
来源：http://nmw.snrcjt.cn

`共 ${n} 条`
来源：http://rns.pycfn.com

[U94] JS：箭头函数
来源：http://uyu.bbcook.cn

const double = x => x * 2;
来源：http://moa.shuidangran.top

[U95] JS：Promise 包装
来源：http://aub.hcnkem.com

new Promise((resolve, reject) => {})
来源：http://zsm.birdmap.top

[U96] JS：async/await 与异常
来源：http://mzl.cucudq.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rmt.redwolf501.top

[U97] JS：并发请求
来源：http://kma.dianchejie.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://rek.jinqigfzy.top

[U98] JS：fetch 带 JSON
来源：http://tmm.vehdjk.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://lfl.yuanzhike.top

[U99] JS：事件监听
来源：http://rvw.tian-w.cn

el.addEventListener("click", e => {})
来源：http://obw.ivvv.top

[U100] JS：DOM 查询
来源：http://uiy.zhengqikj.top

document.querySelector(".item")
来源：http://rre.jinghuilouyu.cn

[U101] JS：classList 操作
来源：http://jtm.feifeiyinyue.top

el.classList.toggle("active")
来源：http://xjn.0kj1m.cn

[U102] JS：本地存储
来源：http://knu.zhongyouzk.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://jqo.jinqigfzy.top

[U103] JS：定时器
来源：http://dhv.zhixingplan.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://onz.cdnleiting.top

[U104] JS：防抖
来源：http://pyj.fktsv.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wmw.dashuyun.cn

[U105] JS：节流
来源：http://mgl.fengsongda.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://eel.0kj1m.cn

[U106] JS：日期格式化
来源：http://ehe.cqqwz.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xzp.ppjwa.cn

[U107] JS：数字千分位
来源：http://pzk.yj20258.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jij.vehdjk.com

[U108] JS：随机整数
来源：http://wfx.wangdashe.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vkz.guowangkeji.top

[U109] JS：数组分组
来源：http://kuk.ehwqpu.com

Object.groupBy(arr, x => x.type)
来源：http://ykt.sjlbkw.cn

[U110] JS：数组分块
来源：http://ptu.jianghu66.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wix.fengsongda.top

[U111] JS：对象转 Map
来源：http://yyc.gotoacloud.top

new Map(Object.entries(obj))
来源：http://tfq.feifeiyinyue.top

[U112] JS：字符串补位
来源：http://kxt.nanxinkj.top

"7".padStart(3, "0")
来源：http://pks.hammf.cn

[U113] JS：正则替换全部
来源：http://fgl.jinghuilouyu.cn

s.replaceAll("a", "b")
来源：http://anr.52xcode.cn

[U114] JS：JSON 深比较
来源：http://gsi.ctjpmb.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://huv.9152youxi.cn

[U115] JS：生成 UUID
来源：http://aud.tian-w.cn

crypto.randomUUID()
来源：http://vrk.chenlongwang.top

[U116] JS：类型检查（JSDoc）
来源：http://tse.jinyuanbaomall.cn

/** @param {string} name */ function f(name) {}
来源：http://rti.fengsongda.top

[U117] JS：单元测试
来源：http://pyd.shzxlz.cn

npm i -D vitest;  npx vitest
来源：http://fuc.sysykeji.top

[U118] JS：开发服务器
来源：http://bxl.shangyingyoupin.top

npm i -D vite;  npx vite
来源：http://eta.sjlbkw.cn

[U119] JS：生产构建
来源：http://obb.jinghuilouyu.cn

npx vite build
来源：http://gvf.fktsv.cn

[U120] JS：读取环境变量（Vite）
来源：http://yol.hfpthk.cn

import.meta.env.VITE_API_URL
来源：http://ets.hammf.cn

================================================================================
来源：http://frw.cucudq.cn

统计汇总
来源：http://vgo.yvedp.cn

================================================================================
来源：http://lcp.jiagoushi.top

按语言统计（条）：
来源：http://pzx.zhiwuduotai.top

Python ......... 252
来源：http://wbo.xingfuxueyuan.xyz

PHP ............ 252
来源：http://fkk.xingfuxueyuan.xyz

JavaScript ..... 252
来源：http://zul.zhengqikj.top

TypeScript ..... 212
来源：http://jth.xylfe.cn

Java ........... 212
来源：http://mfd.jqgufenzy.top

Go ............. 212
来源：http://xvr.iojbl.cn

Ruby ........... 212
来源：http://rvx.uphjek.com

C# ............. 212
来源：http://vbr.gzhubu.top

C .............. 30
来源：http://vhh.hnqzz.top

C++ ............ 30
来源：http://jdi.quarkkingdee.top

SQL ............ 90
来源：http://cgn.jinqigfzy.top

Bash ........... 80
来源：http://duc.smart0.xyz

Kotlin ......... 15
来源：http://qmw.daria6918.cn

Swift .......... 15
来源：http://mbl.316326.xyz

Lua ............ 10
来源：http://dsb.tanke756.top

Perl ........... 10
来源：http://ndc.zhiwuduotai.top

Scala .......... 10
来源：http://vwh.zhixingplan.top

------------------------------------
来源：http://ekr.feifeiyinyue.top

合计 ........... 2106 条
来源：http://vlq.shangyingyoupin.top

按章节统计：
来源：http://ddn.snrcjt.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rzz.redwolf501.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://nmc.nwbrower.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fff.jqgufenzy.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xfc.hfpthk.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pqk.hnqzz.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://cbp.chenlongwang.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ioy.zdbjq.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qls.ywan-chungtsiang.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ktm.iojbl.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nik.fanxiaobao.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fsw.zdqjudy.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hzz.yvedp.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ojk.havefunace.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vmf.ppjwa.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://gdm.gogol.net.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://uxa.daria6918.cn

Q SQL 专题                              90
来源：http://lur.yuxming.cn

R Bash 专题                             80
来源：http://wqt.epnwcf.com

S C / C++ 专题                          60
来源：http://trq.wangdashe.top

T 其他语言补充                          60
来源：http://yup.shzxlz.cn

U 高频实用片段                         120
来源：http://vhy.chenlongwang.top

------------------------------------
来源：http://dgl.zycfv.cn

合计                                  2106 条
来源：http://evd.hesvh.cn

--------------------------------------------------------------------------------
来源：http://gov.gaohongyu789.top

使用提醒
来源：http://lzj.xziqi.cn

--------------------------------------------------------------------------------
来源：http://fzk.epnwcf.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://tzp.dashuyun.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ffy.haohaochexian.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://dxh.jinghuilouyu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ppn.sxryk.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mxx.ydzc1.top

—— 文件结束 ——
来源：http://mxo.shuidangran.top

================================================================================
来源：http://yjd.sysykeji.top

程序语言常见例子速查手册（2024 版）
来源：http://ppd.jyoumei.cn

Common Programming Examples Cheat Book
来源：http://wyr.guowangkeji.top

================================================================================
来源：http://kpd.c1oappe.top

【收录内容】
来源：http://led.haohaochexian.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ahh.jyoumei.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ini.tarul.cn

SQL · Bash · C · C++
来源：http://qyc.shanyushiyangtech.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://fuc.fktsv.cn

【使用说明】
来源：http://eyw.c1oappe.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qko.jqgufenzy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://rld.cdnleiting.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://onr.pengpengdd.cyou

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hya.ppjwa.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://opz.ybcxt.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://tpr.meibo888.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://asl.jyoumei.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://eeq.0kj1m.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ibf.aizwys.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mtj.ywan-chungtsiang.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://igx.fktsv.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://osr.zhiwuduotai.top

【文件统计】
来源：http://rcs.snrcjt.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://fxs.shuidangran.top

--------------------------------------------------------------------------------
来源：http://bxu.xinyue.icu

目  录
来源：http://vyg.0kj1m.cn

--------------------------------------------------------------------------------
来源：http://jyc.zhongyouzk.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qyx.cqqwz.cn


<!-- 参考信息 -->