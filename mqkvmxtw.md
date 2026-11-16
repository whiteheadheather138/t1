代发 wailian999

[U17] Py：初始化日志
来源：http://vbz.cheryme.top

logging.basicConfig(level=logging.INFO)
来源：http://yqr.hywenlv.cn

[U18] Py：预编译正则
来源：http://yag.ehwqpu.com

pat = re.compile(r"\d+")
来源：http://lur.zhongyouzk.top

[U19] Py：正则替换带回调
来源：http://mbs.cdnleiting.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ste.snrcjt.cn

[U20] Py：缓存函数结果
来源：http://jzl.fanxiaobao.xyz

@functools.lru_cache(maxsize=None)
来源：http://hvl.sweek.top

[U21] Py：自定义上下文管理器
来源：http://pjw.pengpengdd.cyou

@contextlib.contextmanager
来源：http://vxj.bjfxy.top

[U22] Py：矩阵转置
来源：http://bmp.cqqwz.cn

list(zip(*m))
来源：http://jph.hesvh.cn

[U23] Py：分块读取大文件
来源：http://sva.cdnleiting.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qkw.gaohongyu789.top

[U24] Py：路径操作
来源：http://alr.ybcxt.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tht.quarkkingdee.top

[U25] Py：CSV 按字典读
来源：http://let.jinghuilouyu.cn

csv.DictReader(f)
来源：http://eng.fzhhl.top

[U26] Py：并发下载
来源：http://gcn.yanxiufei.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rqo.fktsv.cn

[U27] Py：异步 HTTP
来源：http://mnv.jqgufenzy.top

aiohttp.ClientSession() 配合 async with
来源：http://xma.xziqi.cn

[U28] Py：类型别名
来源：http://viu.9152youxi.cn

UserId = int
来源：http://fdb.jyoumei.cn

[U29] Py：属性校验
来源：http://dwk.feifeiyinyue.top

@property 与 @x.setter 配合
来源：http://jff.sufxvd.cn

[U30] Py：数据类
来源：http://udr.bbcook.cn

@dataclass(slots=True)
来源：http://omd.chenjidiqi.icu

[U31] Py：单测
来源：http://qdo.fzhhl.top

python -m pytest -q
来源：http://fmw.sysykeji.top

[U32] Py：代码格式化
来源：http://nzr.xuanzx.com

ruff format . && ruff check --fix .
来源：http://ucp.ydzc1.top

[U33] Py：打包发布
来源：http://rbt.xuanzx.com

python -m build  （依赖 pyproject.toml）
来源：http://git.hysaishi.cn

[U34] Py：判断编码
来源：http://gbv.vqdsnc.cn

chardet.detect(raw)
来源：http://ytd.fzhhl.top

[U35] Py：发送邮件
来源：http://xwy.nanxinkj.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mmh.dashuyun.cn

[U36] Py：定时任务
来源：http://opl.zhixingplan.top

schedule.every(10).minutes.do(job)
来源：http://opx.gzhubu.top

[U37] Py：读写 Excel
来源：http://ayc.meibo888.top

pandas.read_excel / DataFrame.to_excel
来源：http://upi.hfpthk.cn

[U38] Py：获取脚本所在目录
来源：http://pmq.sufxvd.cn

Path(__file__).resolve().parent
来源：http://lri.jinqigufen.top

[U39] Py：判断是否在交互环境
来源：http://ooq.gzhubu.top

sys.stdout.isatty()
来源：http://tlb.jyoumei.cn

[U40] Py：打印到标准错误
来源：http://vni.zdbjq.cn

print("err", file=sys.stderr)
来源：http://qku.mhx1999.top

[U41] PHP：初始化 Composer 项目
来源：http://hob.chenlongwang.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ado.yueranfly.top

[U42] PHP：PSR-4 自动加载
来源：http://phv.fanxiaobao.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ezr.gaohongyu789.top

[U43] PHP：声明命名空间
来源：http://zed.iojbl.cn

namespace App\Http;
来源：http://taj.52xcode.cn

[U44] PHP：开启严格类型
来源：http://qqv.hammf.cn

declare(strict_types=1);
来源：http://osc.yangfankeji.com

[U45] PHP：类型声明与返回类型
来源：http://mgo.jinqigufen.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ght.xuetiantiany.cn

[U46] PHP：可空类型
来源：http://isk.hesvh.cn

?string $name = null
来源：http://bfv.yj20258.top

[U47] PHP：联合类型
来源：http://lzb.ehwqpu.com

int|string $id
来源：http://nwg.hnxiangtu.top

[U48] PHP：纯枚举
来源：http://gnc.yuanzhike.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rar.zhoulong.xyz

[U49] PHP：只读属性
来源：http://joo.chenzaomai.com

public readonly string $name
来源：http://rlt.52xcode.cn

[U50] PHP：构造器属性提升
来源：http://ata.9152youxi.cn

public function __construct(private int $id) {}
来源：http://wqm.chenlongwang.top

[U51] PHP：数组解构
来源：http://fjw.sweek.top

[$a, $b] = $arr;
来源：http://bce.cashguo.top

[U52] PHP：箭头函数
来源：http://rne.zhaomingkeji.xyz

$double = fn($x) => $x * 2;
来源：http://bbh.tianlin.xyz

[U53] PHP：空合并运算符
来源：http://mej.chenlongwang.top

$v = $a ?? $b ?? "default";
来源：http://dwb.zhengqikj.top

[U54] PHP：空安全调用
来源：http://ijh.xziqi.cn

$obj?->method()
来源：http://nwg.chenjidiqi.icu

[U55] PHP：match 表达式
来源：http://nwb.cashguo.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ebq.hcnkem.com

[U56] PHP：命名参数
来源：http://unj.zdbjq.cn

f(a: 1, b: 2)
来源：http://uol.kuanghao11.cn

[U57] PHP：字符串插值
来源：http://lek.chenlongwang.top

"值: {$a}"
来源：http://jvm.svipenyu.cn

[U58] PHP：数组三件套
来源：http://ell.xinyue.icu

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qgw.jqgfzy.top

[U59] PHP：自定义排序
来源：http://fqy.hammf.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://osv.cucudq.cn

[U60] PHP：JSON 编解码
来源：http://bwt.sufxvd.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lce.zhoulong.xyz

[U61] PHP：正则
来源：http://wbi.smart0.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mbq.xinyue.icu

[U62] PHP：日期对象
来源：http://vzn.feifeiyinyue.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wld.snrcjt.cn

[U63] PHP：文件读写
来源：http://nzu.ctjpmb.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wmu.gotoacloud.top

[U64] PHP：目录遍历
来源：http://pch.haohaochexian.top

glob("dir/*.php");  scandir("dir");
来源：http://qqj.pycfn.com

[U65] PHP：会话
来源：http://qbu.jlsjyb.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ico.xziqi.cn

[U66] PHP：设置 Cookie
来源：http://hcd.bbcook.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://aox.pengpengdd.cyou

[U67] PHP：处理文件上传
来源：http://xbb.yuanzhike.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fgg.jinqigufen.top

[U68] PHP：PDO 连接
来源：http://ooq.mhx1999.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xgd.zhaomingkeji.xyz

[U69] PHP：PDO 预处理
来源：http://mnr.snrcjt.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lpk.hongshengwenyu.top

[U70] PHP：PDO 事务
来源：http://eqy.hysaishi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://moj.jiagoushi.top

[U71] PHP：抛出异常
来源：http://xcn.fktsv.cn

throw new RuntimeException("失败", 500);
来源：http://mov.316326.xyz

[U72] PHP：写错误日志
来源：http://mcm.zhiwuduotai.top

error_log("失败: " . $e->getMessage());
来源：http://snk.ppjwa.cn

[U73] PHP：读取 ini 配置
来源：http://arb.tarul.cn

parse_ini_file("config.ini", true)
来源：http://oeu.daria6918.cn

[U74] PHP：读取环境变量
来源：http://ykk.zhiwuduotai.top

getenv("APP_ENV") ?: "production"
来源：http://jal.jiagoushi.top

[U75] PHP：依赖注入
来源：http://zqm.guowangkeji.top

composer require psr/container
来源：http://azq.yonumen.top

[U76] PHP：简单路由
来源：http://esf.aibaodan.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vgs.snrcjt.cn

[U77] PHP：模板渲染
来源：http://mvc.zhiwuduotai.top

composer require twig/twig
来源：http://cpw.zhongyouzk.top

[U78] PHP：单元测试
来源：http://pah.dianchejie.cn

composer require --dev phpunit/phpunit
来源：http://oxk.52xcode.cn

[U79] PHP：静态分析
来源：http://bye.fehbvm.com

composer require --dev phpstan/phpstan
来源：http://bkg.yanxiufei.cn

[U80] PHP：代码规范修复
来源：http://xvk.iojbl.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://rzz.pycfn.com

[U81] JS：初始化项目
来源：http://uui.cqqwz.cn

npm init -y;  npm i express
来源：http://vpb.quarkkingdee.top

[U82] JS：package.json 脚本
来源：http://dol.epnwcf.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ruy.ppjwa.cn

[U83] JS：ES Module 导入导出
来源：http://slj.shzxlz.cn

export const a = 1;  import { a } from "./m.js";
来源：http://dgy.jiagoushi.top

[U84] JS：CommonJS 写法
来源：http://igv.c1oappe.top

module.exports = { a };  const { a } = require("./m");
来源：http://wme.jinyuanbaomall.cn

[U85] JS：可选链
来源：http://fqd.yonumen.top

a?.b?.c
来源：http://dbf.yanxiufei.cn

[U86] JS：空值合并
来源：http://hln.cqqwz.cn

a ?? b
来源：http://ufj.nwbrower.top

[U87] JS：解构默认值
来源：http://svq.gzhubu.top

const { a = 1, b = 2 } = obj;
来源：http://cmy.kuanghao11.cn

[U88] JS：对象展开合并
来源：http://sli.yangfankeji.com

{ ...a, ...b }
来源：http://wqu.nanxinkj.top

[U89] JS：数组去重
来源：http://vrz.sweek.top

[...new Set(arr)]
来源：http://pxw.hnqzz.top

[U90] JS：数字数组排序
来源：http://pry.hammf.cn

[...arr].sort((a, b) => a - b)
来源：http://vyt.hfpthk.cn

[U91] JS：对象键值遍历
来源：http://xtz.uphjek.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://upo.hammf.cn

[U92] JS：深拷贝
来源：http://oet.jinqigfzy.top

structuredClone(obj)
来源：http://lin.jqgufenzy.top

[U93] JS：模板字符串
来源：http://zam.c1oappe.top

`共 ${n} 条`
来源：http://eax.wangshuangyany.cn

[U94] JS：箭头函数
来源：http://qqp.shanyushiyangtech.top

const double = x => x * 2;
来源：http://yix.wangdashe.top

[U95] JS：Promise 包装
来源：http://twp.dashuyun.cn

new Promise((resolve, reject) => {})
来源：http://buo.ydzc1.top

[U96] JS：async/await 与异常
来源：http://dze.hongshengwenyu.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ymb.xuanzx.com

[U97] JS：并发请求
来源：http://rfg.sufxvd.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://sjz.tian-w.cn

[U98] JS：fetch 带 JSON
来源：http://tfy.zdqjudy.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xda.xingfuxueyuan.xyz

[U99] JS：事件监听
来源：http://dro.yvedp.cn

el.addEventListener("click", e => {})
来源：http://cqt.fengsongda.top

[U100] JS：DOM 查询
来源：http://uem.svipenyu.cn

document.querySelector(".item")
来源：http://lsq.guannengcc.top

[U101] JS：classList 操作
来源：http://zni.yfazqb.com

el.classList.toggle("active")
来源：http://kch.pycfn.com

[U102] JS：本地存储
来源：http://yyt.hammf.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://att.hongshengwenyu.top

[U103] JS：定时器
来源：http://ljp.dashuyun.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kpr.daria6918.cn

[U104] JS：防抖
来源：http://iyr.fzhhl.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cim.sufxvd.cn

[U105] JS：节流
来源：http://jtr.hywenlv.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kac.jyoumei.cn

[U106] JS：日期格式化
来源：http://dlx.yj20258888.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://aqw.bjfxy.top

[U107] JS：数字千分位
来源：http://usg.zhongyouzk.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vcv.gaohongyu789.top

[U108] JS：随机整数
来源：http://jgm.sysykeji.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://unw.bjfxy.top

[U109] JS：数组分组
来源：http://yzv.shzxlz.cn

Object.groupBy(arr, x => x.type)
来源：http://uji.fzhhl.top

[U110] JS：数组分块
来源：http://lex.yj20258888.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cbz.cashguo.top

[U111] JS：对象转 Map
来源：http://ctg.havefunace.top

new Map(Object.entries(obj))
来源：http://zpt.nwbrower.top

[U112] JS：字符串补位
来源：http://rqq.zhoulong.xyz

"7".padStart(3, "0")
来源：http://uqz.ivvv.top

[U113] JS：正则替换全部
来源：http://zon.ydjk.org.cn

s.replaceAll("a", "b")
来源：http://jyl.0kj1m.cn

[U114] JS：JSON 深比较
来源：http://fra.zycfv.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://bop.feifeiyinyue.top

[U115] JS：生成 UUID
来源：http://xjk.zhixingplan.top

crypto.randomUUID()
来源：http://age.xuetiantiany.cn

[U116] JS：类型检查（JSDoc）
来源：http://twe.cashguo.top

/** @param {string} name */ function f(name) {}
来源：http://pwp.epnwcf.com

[U117] JS：单元测试
来源：http://ceo.xylfe.cn

npm i -D vitest;  npx vitest
来源：http://yxz.nwbrower.top

[U118] JS：开发服务器
来源：http://ypi.iojbl.cn

npm i -D vite;  npx vite
来源：http://mob.nanxinkj.top

[U119] JS：生产构建
来源：http://qnp.aibaodan.cn

npx vite build
来源：http://xit.gaohongyu789.top

[U120] JS：读取环境变量（Vite）
来源：http://glp.tianlin.xyz

import.meta.env.VITE_API_URL
来源：http://imz.yj20258.top

================================================================================
来源：http://lex.hcnkem.com

统计汇总
来源：http://vfg.redwolf501.top

================================================================================
来源：http://lrx.ydjk.org.cn

按语言统计（条）：
来源：http://mqu.bbcook.cn

Python ......... 252
来源：http://djg.xuetiantiany.cn

PHP ............ 252
来源：http://vsj.xinyue.icu

JavaScript ..... 252
来源：http://hwt.cheryme.top

TypeScript ..... 212
来源：http://rpl.wangshuangyany.cn

Java ........... 212
来源：http://vzs.xuanzx.com

Go ............. 212
来源：http://ele.fengsongda.top

Ruby ........... 212
来源：http://ukb.hywenlv.cn

C# ............. 212
来源：http://ezm.ehwqpu.com

C .............. 30
来源：http://axd.yj20258.top

C++ ............ 30
来源：http://gex.zhixingplan.top

SQL ............ 90
来源：http://xbc.andypj.xyz

Bash ........... 80
来源：http://dho.dashuyun.cn

Kotlin ......... 15
来源：http://qcw.jyoumei.cn

Swift .......... 15
来源：http://slg.hywenlv.cn

Lua ............ 10
来源：http://vzm.cashguo.top

Perl ........... 10
来源：http://wxl.redwolf501.top

Scala .......... 10
来源：http://ipm.xinyue.icu

------------------------------------
来源：http://mqa.hfpthk.cn

合计 ........... 2106 条
来源：http://ixk.yangfankeji.com

按章节统计：
来源：http://pbx.quarkkingdee.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://kzi.hesvh.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://kdh.cucudq.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://miq.dianchejie.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://awd.jinyuanbaomall.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vjt.gaohongyu789.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://kly.sysykeji.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ejs.quarkkingdee.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cyz.iojbl.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://iic.jqgufenzy.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vvd.kuanghao11.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://lir.aibaodan.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kkz.hongshengwenyu.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://gpz.hcnkem.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rqw.cucudq.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://puv.cheryme.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hjk.hongshengwenyu.top

Q SQL 专题                              90
来源：http://rrt.kuanghao11.cn

R Bash 专题                             80
来源：http://rec.xingfuxueyuan.xyz

S C / C++ 专题                          60
来源：http://hcn.gotoacloud.top

T 其他语言补充                          60
来源：http://xlm.xuanzx.com

U 高频实用片段                         120
来源：http://nhk.jinqigufen.top

------------------------------------
来源：http://nbz.ydzc1.top

合计                                  2106 条
来源：http://gcg.sysykeji.top

--------------------------------------------------------------------------------
来源：http://yko.daria6918.cn

使用提醒
来源：http://kad.zhongyouzk.top

--------------------------------------------------------------------------------
来源：http://gah.xingfuxueyuan.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://spt.yueranfly.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jmw.cdnleiting.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://bzp.vehdjk.com

在旧版本上使用前请先确认语法支持情况。
来源：http://tgj.hongshengwenyu.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ryr.shanyushiyangtech.top

—— 文件结束 ——
来源：http://csy.vqdsnc.cn

================================================================================
来源：http://rgp.yangfankeji.com

程序语言常见例子速查手册（2024 版）
来源：http://ktc.gogol.net.cn

Common Programming Examples Cheat Book
来源：http://kvz.gotoacloud.top

================================================================================
来源：http://dme.zycfv.cn

【收录内容】
来源：http://cgu.tarul.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://mdi.hnxiangtu.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ure.fehbvm.com

SQL · Bash · C · C++
来源：http://gzy.ehwqpu.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mmx.xylfe.cn

【使用说明】
来源：http://yxt.hongshengwenyu.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hmz.shangyingyoupin.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://onu.shzxlz.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://xga.hnqzz.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://izv.gogol.net.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://okd.jinghuilouyu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://tsi.sxryk.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://liw.xingfuxueyuan.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://tdc.snrcjt.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://rwy.shuidangran.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://nvm.fanxiaobao.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://kpr.cqqwz.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://izs.yj202588.top

【文件统计】
来源：http://cfy.chenzaomai.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wkw.yueranfly.top

--------------------------------------------------------------------------------
来源：http://zde.andypj.xyz

目  录
来源：http://uww.hongshengwenyu.top

--------------------------------------------------------------------------------
来源：http://vpb.wangdashe.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ith.zhijiandao.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ehg.aizwys.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ipp.xylfe.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://psa.jiagoushi.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ssz.zdbjq.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://cef.ydzc1.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://yfw.xuanzx.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zmn.hesvh.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ciw.zhoulong.xyz


<!-- 参考信息 -->