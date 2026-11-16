代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://hdc.hfpthk.cn

@contextlib.contextmanager
来源：http://qsk.ctjpmb.com

[U22] Py：矩阵转置
来源：http://qxy.ehwqpu.com

list(zip(*m))
来源：http://uqa.yuxming.cn

[U23] Py：分块读取大文件
来源：http://ypy.yanxiufei.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ojo.ehwqpu.com

[U24] Py：路径操作
来源：http://lek.yj202588.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hda.jqgufenzy.top

[U25] Py：CSV 按字典读
来源：http://pso.xziqi.cn

csv.DictReader(f)
来源：http://cjs.tianlin.xyz

[U26] Py：并发下载
来源：http://ytp.gzhubu.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bfj.daria6918.cn

[U27] Py：异步 HTTP
来源：http://vak.ppjwa.cn

aiohttp.ClientSession() 配合 async with
来源：http://ovu.zdqjudy.top

[U28] Py：类型别名
来源：http://alr.shangyingyoupin.top

UserId = int
来源：http://rdu.shangyingyoupin.top

[U29] Py：属性校验
来源：http://oeo.hysaishi.cn

@property 与 @x.setter 配合
来源：http://zxh.sjlbkw.cn

[U30] Py：数据类
来源：http://utn.hywenlv.cn

@dataclass(slots=True)
来源：http://oyk.ydzc1.top

[U31] Py：单测
来源：http://vpo.yj202588.top

python -m pytest -q
来源：http://sdv.cdnleiting.top

[U32] Py：代码格式化
来源：http://dgm.hammf.cn

ruff format . && ruff check --fix .
来源：http://vsj.ivvv.top

[U33] Py：打包发布
来源：http://gza.ydzc1.top

python -m build  （依赖 pyproject.toml）
来源：http://rur.zhongyouzk.top

[U34] Py：判断编码
来源：http://ctn.shangyingyoupin.top

chardet.detect(raw)
来源：http://xyd.chenlongwang.top

[U35] Py：发送邮件
来源：http://sbq.sufxvd.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wlw.epnwcf.com

[U36] Py：定时任务
来源：http://jge.mhx1999.top

schedule.every(10).minutes.do(job)
来源：http://xjh.dashuyun.cn

[U37] Py：读写 Excel
来源：http://rgl.cashguo.top

pandas.read_excel / DataFrame.to_excel
来源：http://wlj.jiagoushi.top

[U38] Py：获取脚本所在目录
来源：http://ous.haohaochexian.top

Path(__file__).resolve().parent
来源：http://gmu.yuanzhike.top

[U39] Py：判断是否在交互环境
来源：http://nor.pengpengdd.cyou

sys.stdout.isatty()
来源：http://tyl.pengpengdd.cyou

[U40] Py：打印到标准错误
来源：http://kjb.shanyushiyangtech.top

print("err", file=sys.stderr)
来源：http://ytg.zhijiandao.cn

[U41] PHP：初始化 Composer 项目
来源：http://kmi.jlsjyb.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://baa.wangdashe.top

[U42] PHP：PSR-4 自动加载
来源：http://ods.dianchejie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zvs.xuetiantiany.cn

[U43] PHP：声明命名空间
来源：http://vqc.mhx1999.top

namespace App\Http;
来源：http://sjx.cdnleiting.top

[U44] PHP：开启严格类型
来源：http://ceu.dianchejie.cn

declare(strict_types=1);
来源：http://kvn.jianghu66.top

[U45] PHP：类型声明与返回类型
来源：http://lzv.jinyuanbaomall.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://qyf.cheryme.top

[U46] PHP：可空类型
来源：http://idv.zhixingplan.top

?string $name = null
来源：http://rqa.jianghu66.top

[U47] PHP：联合类型
来源：http://buf.jyoumei.cn

int|string $id
来源：http://kuw.tian-w.cn

[U48] PHP：纯枚举
来源：http://mjr.andypj.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dyx.shangyingyoupin.top

[U49] PHP：只读属性
来源：http://eox.shanyushiyangkeji.top

public readonly string $name
来源：http://pwl.hnqzz.top

[U50] PHP：构造器属性提升
来源：http://bkg.xingfuxueyuan.xyz

public function __construct(private int $id) {}
来源：http://eyo.chenjidiqi.icu

[U51] PHP：数组解构
来源：http://otj.yangfankeji.com

[$a, $b] = $arr;
来源：http://gll.chenlongwang.top

[U52] PHP：箭头函数
来源：http://vgx.yangfankeji.com

$double = fn($x) => $x * 2;
来源：http://whk.sysykeji.top

[U53] PHP：空合并运算符
来源：http://yvo.kuanghao11.cn

$v = $a ?? $b ?? "default";
来源：http://dlw.daxiang520.top

[U54] PHP：空安全调用
来源：http://mot.c1oappe.top

$obj?->method()
来源：http://ncj.jianghu66.top

[U55] PHP：match 表达式
来源：http://fba.cucudq.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zvw.xylfe.cn

[U56] PHP：命名参数
来源：http://ggy.fktsv.cn

f(a: 1, b: 2)
来源：http://ock.52xcode.cn

[U57] PHP：字符串插值
来源：http://gvh.zhixingplan.top

"值: {$a}"
来源：http://fbc.shuidangran.top

[U58] PHP：数组三件套
来源：http://pww.feifeiyinyue.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jje.zhaomingkeji.xyz

[U59] PHP：自定义排序
来源：http://xmr.52xcode.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rva.yonumen.top

[U60] PHP：JSON 编解码
来源：http://ymj.xinyue.icu

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://yfi.cqqwz.cn

[U61] PHP：正则
来源：http://pir.zhoulong.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fvr.zhoulong.xyz

[U62] PHP：日期对象
来源：http://okh.ivvv.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ghp.epnwcf.com

[U63] PHP：文件读写
来源：http://ujl.tanke756.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ddi.fzhhl.top

[U64] PHP：目录遍历
来源：http://mka.hnxiangtu.top

glob("dir/*.php");  scandir("dir");
来源：http://lon.shanyushiyangtech.top

[U65] PHP：会话
来源：http://acb.fengsongda.top

session_start();  $_SESSION["uid"] = 1;
来源：http://hof.mhx1999.top

[U66] PHP：设置 Cookie
来源：http://vtw.svipenyu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://doa.guowangkeji.top

[U67] PHP：处理文件上传
来源：http://ayx.wangdashe.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://etj.zhongyouzk.top

[U68] PHP：PDO 连接
来源：http://gfe.yanxiufei.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qrs.9152youxi.cn

[U69] PHP：PDO 预处理
来源：http://cob.ydjk.org.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://tyr.jqgfzy.top

[U70] PHP：PDO 事务
来源：http://kcl.yuxming.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dvc.tanke756.top

[U71] PHP：抛出异常
来源：http://ueq.cheryme.top

throw new RuntimeException("失败", 500);
来源：http://bge.feifeiyinyue.top

[U72] PHP：写错误日志
来源：http://dxx.hammf.cn

error_log("失败: " . $e->getMessage());
来源：http://gaq.shangyingyoupin.top

[U73] PHP：读取 ini 配置
来源：http://lsg.gogol.net.cn

parse_ini_file("config.ini", true)
来源：http://ziy.zdbjq.cn

[U74] PHP：读取环境变量
来源：http://ohc.haohaochexian.top

getenv("APP_ENV") ?: "production"
来源：http://rww.jqgufenzy.top

[U75] PHP：依赖注入
来源：http://ohw.fktsv.cn

composer require psr/container
来源：http://yfs.fanxiaobao.xyz

[U76] PHP：简单路由
来源：http://cjt.jinyuanbaomall.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://aro.jqgufenzy.top

[U77] PHP：模板渲染
来源：http://dwo.dashuyun.cn

composer require twig/twig
来源：http://yry.dianchejie.cn

[U78] PHP：单元测试
来源：http://rsd.fengsongda.top

composer require --dev phpunit/phpunit
来源：http://xlc.c1oappe.top

[U79] PHP：静态分析
来源：http://dhg.dianchejie.cn

composer require --dev phpstan/phpstan
来源：http://udf.hywenlv.cn

[U80] PHP：代码规范修复
来源：http://xiq.meibo888.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://txw.yangfankeji.com

[U81] JS：初始化项目
来源：http://rhv.52xcode.cn

npm init -y;  npm i express
来源：http://oby.shuidangran.top

[U82] JS：package.json 脚本
来源：http://vgg.chenlongwang.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://rmi.svipenyu.cn

[U83] JS：ES Module 导入导出
来源：http://ptl.gaohongyu789.top

export const a = 1;  import { a } from "./m.js";
来源：http://ujv.ctjpmb.com

[U84] JS：CommonJS 写法
来源：http://teh.yuxming.cn

module.exports = { a };  const { a } = require("./m");
来源：http://gtb.ehwqpu.com

[U85] JS：可选链
来源：http://sat.sjlbkw.cn

a?.b?.c
来源：http://luf.ydjk.org.cn

[U86] JS：空值合并
来源：http://gqw.ehwqpu.com

a ?? b
来源：http://pgn.hcnkem.com

[U87] JS：解构默认值
来源：http://hkk.yangfankeji.com

const { a = 1, b = 2 } = obj;
来源：http://ftv.feifeiyinyue.top

[U88] JS：对象展开合并
来源：http://kdq.redwolf501.top

{ ...a, ...b }
来源：http://pmc.havefunace.top

[U89] JS：数组去重
来源：http://njt.c1oappe.top

[...new Set(arr)]
来源：http://hmy.zdqjudy.top

[U90] JS：数字数组排序
来源：http://mly.yueranfly.top

[...arr].sort((a, b) => a - b)
来源：http://dxt.shangyingyoupin.top

[U91] JS：对象键值遍历
来源：http://xzy.cashguo.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qua.hammf.cn

[U92] JS：深拷贝
来源：http://jhk.zdbjq.cn

structuredClone(obj)
来源：http://apq.hcnkem.com

[U93] JS：模板字符串
来源：http://swi.meibo888.top

`共 ${n} 条`
来源：http://rbj.andypj.xyz

[U94] JS：箭头函数
来源：http://hil.zhongyouzk.top

const double = x => x * 2;
来源：http://dgm.hammf.cn

[U95] JS：Promise 包装
来源：http://kxk.dianchejie.cn

new Promise((resolve, reject) => {})
来源：http://xib.ybcxt.top

[U96] JS：async/await 与异常
来源：http://ktf.xziqi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ptr.hongshengwenyu.top

[U97] JS：并发请求
来源：http://oju.yanxiufei.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://tbt.guannengcc.top

[U98] JS：fetch 带 JSON
来源：http://nxd.hcnkem.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zii.hnxiangtu.top

[U99] JS：事件监听
来源：http://fnk.chenzaomai.com

el.addEventListener("click", e => {})
来源：http://him.yj20258.top

[U100] JS：DOM 查询
来源：http://sta.ydzc1.top

document.querySelector(".item")
来源：http://swe.sweek.top

[U101] JS：classList 操作
来源：http://qyz.yuanzhike.top

el.classList.toggle("active")
来源：http://pyg.jqgufenzy.top

[U102] JS：本地存储
来源：http://tbf.yueranfly.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://zbr.ctjpmb.com

[U103] JS：定时器
来源：http://sgr.aibaodan.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zya.chenjidiqi.icu

[U104] JS：防抖
来源：http://xfp.hfpthk.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sxx.yj202588.top

[U105] JS：节流
来源：http://xut.shanyushiyangtech.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yta.yanxiufei.cn

[U106] JS：日期格式化
来源：http://wjg.zhijiandao.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kzn.svipenyu.cn

[U107] JS：数字千分位
来源：http://pma.52xcode.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nvg.yfazqb.com

[U108] JS：随机整数
来源：http://krq.fktsv.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://lai.gaohongyu789.top

[U109] JS：数组分组
来源：http://gwk.chenjidiqi.icu

Object.groupBy(arr, x => x.type)
来源：http://upt.cucudq.cn

[U110] JS：数组分块
来源：http://auy.tianlin.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vxb.dashuyun.cn

[U111] JS：对象转 Map
来源：http://tzr.jqgufenzy.top

new Map(Object.entries(obj))
来源：http://ksc.gogol.net.cn

[U112] JS：字符串补位
来源：http://ouo.yj20258.top

"7".padStart(3, "0")
来源：http://xpe.fehbvm.com

[U113] JS：正则替换全部
来源：http://pzw.cheryme.top

s.replaceAll("a", "b")
来源：http://taz.hammf.cn

[U114] JS：JSON 深比较
来源：http://eqa.zhaomingkeji.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://gzt.xziqi.cn

[U115] JS：生成 UUID
来源：http://kic.wangdashe.top

crypto.randomUUID()
来源：http://zin.uphjek.com

[U116] JS：类型检查（JSDoc）
来源：http://win.dashuyun.cn

/** @param {string} name */ function f(name) {}
来源：http://ixf.zhiwuduotai.top

[U117] JS：单元测试
来源：http://vwa.hywenlv.cn

npm i -D vitest;  npx vitest
来源：http://hvj.cqqwz.cn

[U118] JS：开发服务器
来源：http://sjl.jinyuanbaomall.cn

npm i -D vite;  npx vite
来源：http://ikv.daxiang520.top

[U119] JS：生产构建
来源：http://ixi.zdbjq.cn

npx vite build
来源：http://jkc.ctjpmb.com

[U120] JS：读取环境变量（Vite）
来源：http://yvl.daxiang520.top

import.meta.env.VITE_API_URL
来源：http://kul.guannengcc.top

================================================================================
来源：http://jhf.aizwys.cn

统计汇总
来源：http://nhf.daxiang520.top

================================================================================
来源：http://yxn.dianchejie.cn

按语言统计（条）：
来源：http://fsh.hywenlv.cn

Python ......... 252
来源：http://iwm.wangshuangyany.cn

PHP ............ 252
来源：http://lao.yfazqb.com

JavaScript ..... 252
来源：http://hdn.0kj1m.cn

TypeScript ..... 212
来源：http://cpj.iojbl.cn

Java ........... 212
来源：http://gvr.9152youxi.cn

Go ............. 212
来源：http://pbt.zdbjq.cn

Ruby ........... 212
来源：http://ueu.shzxlz.cn

C# ............. 212
来源：http://oak.zhengqikj.top

C .............. 30
来源：http://qsm.quarkkingdee.top

C++ ............ 30
来源：http://xuc.zhijiandao.cn

SQL ............ 90
来源：http://gch.tanke756.top

Bash ........... 80
来源：http://rgr.xingfuxueyuan.xyz

Kotlin ......... 15
来源：http://lpp.zhongyouzk.top

Swift .......... 15
来源：http://jku.yj20258888.top

Lua ............ 10
来源：http://wqi.iojbl.cn

Perl ........... 10
来源：http://xvo.shzxlz.cn

Scala .......... 10
来源：http://ery.xingfuxueyuan.xyz

------------------------------------
来源：http://wkq.hesvh.cn

合计 ........... 2106 条
来源：http://ujq.wangdashe.top

按章节统计：
来源：http://dny.shangyingyoupin.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fyj.tanke756.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hcp.gaohongyu789.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vli.xingfuxueyuan.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gza.ctjpmb.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xpb.tarul.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://oaf.zdqjudy.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zoo.zdqjudy.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wmr.316326.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ktf.chenjidiqi.icu

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://irh.wangshuangyany.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mwn.sjlbkw.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cja.kuanghao11.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mja.sysykeji.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://szu.snrcjt.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zjj.zycfv.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://cfy.yj20258888.top

Q SQL 专题                              90
来源：http://ybq.tanke756.top

R Bash 专题                             80
来源：http://zoe.xuanzx.com

S C / C++ 专题                          60
来源：http://alt.yuanzhike.top

T 其他语言补充                          60
来源：http://vry.9152youxi.cn

U 高频实用片段                         120
来源：http://vwg.zhixingplan.top

------------------------------------
来源：http://gpg.ctjpmb.com

合计                                  2106 条
来源：http://edi.jinqigfzy.top

--------------------------------------------------------------------------------
来源：http://qdf.shzxlz.cn

使用提醒
来源：http://kdi.jyoumei.cn

--------------------------------------------------------------------------------
来源：http://dud.nanxinkj.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nig.ctjpmb.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mpz.yuanzhike.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xly.shangyingyoupin.top

在旧版本上使用前请先确认语法支持情况。
来源：http://hgb.xinyue.icu

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://kxo.birdmap.top

—— 文件结束 ——
来源：http://pne.xuanzx.com

================================================================================
来源：http://nnc.tanke756.top

程序语言常见例子速查手册（2024 版）
来源：http://cil.zycfv.cn

Common Programming Examples Cheat Book
来源：http://vqh.yj202588.top

================================================================================
来源：http://uhn.smart0.xyz

【收录内容】
来源：http://xrl.zhixingplan.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ten.yj20258888.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://lpt.gogol.net.cn

SQL · Bash · C · C++
来源：http://xrv.bjfxy.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://vlt.gogol.net.cn

【使用说明】
来源：http://ctw.zhoulong.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wpg.aizwys.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://rif.chenlongwang.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://oek.fzhhl.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wzj.sysykeji.top

Bash:  Shell         C:     C             C++:   C++
来源：http://uog.jianghu66.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://dpw.yangfankeji.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wvs.nwbrower.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hhj.jinyuanbaomall.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://uih.zhongyouzk.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://rdb.zhongyouzk.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bus.snrcjt.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://gxs.redwolf501.top

【文件统计】
来源：http://dzz.guowangkeji.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://dij.bbcook.cn

--------------------------------------------------------------------------------
来源：http://tze.chenlongwang.top

目  录
来源：http://les.gogol.net.cn

--------------------------------------------------------------------------------
来源：http://rru.yueranfly.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://uyc.sysykeji.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://bjy.chenjidiqi.icu

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hnv.iojbl.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://tlv.hfpthk.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://iar.wangshuangyany.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hcl.dianchejie.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://igz.gzhubu.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ojs.yueranfly.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lei.jinyuanbaomall.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jgf.yonumen.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mtp.yj202588.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://fhv.snrcjt.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xrx.wangshuangyany.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://meg.sysykeji.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://yfc.yuxming.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ixo.nwbrower.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://bon.sxryk.cn


<!-- 参考信息 -->