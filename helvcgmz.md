代发 wailian999

[U23] Py：分块读取大文件
来源：http://bxi.havefunace.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://sdc.hesvh.cn

[U24] Py：路径操作
来源：http://ksm.birdmap.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bhg.yongpay.top

[U25] Py：CSV 按字典读
来源：http://cjw.yfazqb.com

csv.DictReader(f)
来源：http://nel.yvedp.cn

[U26] Py：并发下载
来源：http://lns.hammf.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jpq.iojbl.cn

[U27] Py：异步 HTTP
来源：http://vqb.sufxvd.cn

aiohttp.ClientSession() 配合 async with
来源：http://xob.52xcode.cn

[U28] Py：类型别名
来源：http://wlz.ydjk.org.cn

UserId = int
来源：http://ysq.sufxvd.cn

[U29] Py：属性校验
来源：http://gwo.hesvh.cn

@property 与 @x.setter 配合
来源：http://ctc.gotoacloud.top

[U30] Py：数据类
来源：http://fsw.svipenyu.cn

@dataclass(slots=True)
来源：http://gaj.haohaochexian.top

[U31] Py：单测
来源：http://jcp.hnqzz.top

python -m pytest -q
来源：http://yzy.ydjk.org.cn

[U32] Py：代码格式化
来源：http://ecs.gotoacloud.top

ruff format . && ruff check --fix .
来源：http://dkc.jyoumei.cn

[U33] Py：打包发布
来源：http://dbw.zhoulong.xyz

python -m build  （依赖 pyproject.toml）
来源：http://cou.chenzaomai.com

[U34] Py：判断编码
来源：http://wxv.yongpay.top

chardet.detect(raw)
来源：http://rhh.zhiwuduotai.top

[U35] Py：发送邮件
来源：http://ykt.aizwys.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fii.tianlin.xyz

[U36] Py：定时任务
来源：http://vtm.pycfn.com

schedule.every(10).minutes.do(job)
来源：http://csn.9152youxi.cn

[U37] Py：读写 Excel
来源：http://goj.kuanghao11.cn

pandas.read_excel / DataFrame.to_excel
来源：http://lta.pengpengdd.cyou

[U38] Py：获取脚本所在目录
来源：http://mhp.xziqi.cn

Path(__file__).resolve().parent
来源：http://rfd.jinyuanbaomall.cn

[U39] Py：判断是否在交互环境
来源：http://shj.cqqwz.cn

sys.stdout.isatty()
来源：http://utu.c1oappe.top

[U40] Py：打印到标准错误
来源：http://myq.shzxlz.cn

print("err", file=sys.stderr)
来源：http://qqv.yonumen.top

[U41] PHP：初始化 Composer 项目
来源：http://qnz.yanxiufei.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://oit.dianchejie.cn

[U42] PHP：PSR-4 自动加载
来源：http://cta.ctjpmb.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mgg.0kj1m.cn

[U43] PHP：声明命名空间
来源：http://wkd.fengsongda.top

namespace App\Http;
来源：http://qtv.fktsv.cn

[U44] PHP：开启严格类型
来源：http://mqi.tarul.cn

declare(strict_types=1);
来源：http://lyw.cqqwz.cn

[U45] PHP：类型声明与返回类型
来源：http://ily.sysykeji.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://xwx.nanxinkj.top

[U46] PHP：可空类型
来源：http://jeg.52xcode.cn

?string $name = null
来源：http://bgv.xuetiantiany.cn

[U47] PHP：联合类型
来源：http://hjq.xylfe.cn

int|string $id
来源：http://wzn.ivvv.top

[U48] PHP：纯枚举
来源：http://yid.hongshengwenyu.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cwu.hesvh.cn

[U49] PHP：只读属性
来源：http://irj.shzxlz.cn

public readonly string $name
来源：http://bbt.chenlongwang.top

[U50] PHP：构造器属性提升
来源：http://ogk.guannengcc.top

public function __construct(private int $id) {}
来源：http://azl.sufxvd.cn

[U51] PHP：数组解构
来源：http://mxf.shzxlz.cn

[$a, $b] = $arr;
来源：http://xgy.jinghuilouyu.cn

[U52] PHP：箭头函数
来源：http://nlm.hysaishi.cn

$double = fn($x) => $x * 2;
来源：http://dco.shzxlz.cn

[U53] PHP：空合并运算符
来源：http://hpe.jinghuilouyu.cn

$v = $a ?? $b ?? "default";
来源：http://bql.jinyuanbaomall.cn

[U54] PHP：空安全调用
来源：http://iec.svipenyu.cn

$obj?->method()
来源：http://ddw.shuidangran.top

[U55] PHP：match 表达式
来源：http://agz.ybcxt.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://adb.guannengcc.top

[U56] PHP：命名参数
来源：http://goc.xingfuxueyuan.xyz

f(a: 1, b: 2)
来源：http://ofj.sufxvd.cn

[U57] PHP：字符串插值
来源：http://wjf.hysaishi.cn

"值: {$a}"
来源：http://brg.sweek.top

[U58] PHP：数组三件套
来源：http://yoy.hcnkem.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://unx.xingfuxueyuan.xyz

[U59] PHP：自定义排序
来源：http://yss.ydjk.org.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fka.vqdsnc.cn

[U60] PHP：JSON 编解码
来源：http://qik.havefunace.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xdv.ydjk.org.cn

[U61] PHP：正则
来源：http://whv.wangdashe.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://psa.fehbvm.com

[U62] PHP：日期对象
来源：http://jvf.chenjidiqi.icu

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nsj.cqqwz.cn

[U63] PHP：文件读写
来源：http://tqf.9152youxi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hhd.birdmap.top

[U64] PHP：目录遍历
来源：http://ftr.sjlbkw.cn

glob("dir/*.php");  scandir("dir");
来源：http://fus.gotoacloud.top

[U65] PHP：会话
来源：http://ugo.zhongyouzk.top

session_start();  $_SESSION["uid"] = 1;
来源：http://qsq.zhijiandao.cn

[U66] PHP：设置 Cookie
来源：http://ilj.fzhhl.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kog.yuanzhike.top

[U67] PHP：处理文件上传
来源：http://tdc.hcnkem.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dgf.zhoulong.xyz

[U68] PHP：PDO 连接
来源：http://auh.guowangkeji.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pqt.xziqi.cn

[U69] PHP：PDO 预处理
来源：http://wug.svipenyu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://uyf.guowangkeji.top

[U70] PHP：PDO 事务
来源：http://waf.yangfankeji.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bpw.shangyingyoupin.top

[U71] PHP：抛出异常
来源：http://pir.nanxinkj.top

throw new RuntimeException("失败", 500);
来源：http://xsn.tianlin.xyz

[U72] PHP：写错误日志
来源：http://dhu.fengsongda.top

error_log("失败: " . $e->getMessage());
来源：http://ghq.nanxuanxn.top

[U73] PHP：读取 ini 配置
来源：http://mht.hywenlv.cn

parse_ini_file("config.ini", true)
来源：http://odo.aizwys.cn

[U74] PHP：读取环境变量
来源：http://nmx.nwbrower.top

getenv("APP_ENV") ?: "production"
来源：http://igb.tian-w.cn

[U75] PHP：依赖注入
来源：http://mfi.birdmap.top

composer require psr/container
来源：http://yrm.yj202588.top

[U76] PHP：简单路由
来源：http://okp.yangfankeji.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wcd.zhixingplan.top

[U77] PHP：模板渲染
来源：http://qcb.zhoulong.xyz

composer require twig/twig
来源：http://yko.yanxiufei.cn

[U78] PHP：单元测试
来源：http://zkh.sxryk.cn

composer require --dev phpunit/phpunit
来源：http://nug.yueranfly.top

[U79] PHP：静态分析
来源：http://utn.tian-w.cn

composer require --dev phpstan/phpstan
来源：http://ejg.meibo888.top

[U80] PHP：代码规范修复
来源：http://mgr.zhengqikj.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://xfo.sweek.top

[U81] JS：初始化项目
来源：http://tiv.hysaishi.cn

npm init -y;  npm i express
来源：http://son.tian-w.cn

[U82] JS：package.json 脚本
来源：http://mut.jyoumei.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://tpf.yanxiufei.cn

[U83] JS：ES Module 导入导出
来源：http://ixn.yuxming.cn

export const a = 1;  import { a } from "./m.js";
来源：http://oqe.feifeiyinyue.top

[U84] JS：CommonJS 写法
来源：http://aqg.hammf.cn

module.exports = { a };  const { a } = require("./m");
来源：http://tlh.fanxiaobao.xyz

[U85] JS：可选链
来源：http://rwz.jinqigufen.top

a?.b?.c
来源：http://bhb.hesvh.cn

[U86] JS：空值合并
来源：http://rut.zhaomingkeji.xyz

a ?? b
来源：http://hyg.andypj.xyz

[U87] JS：解构默认值
来源：http://wrh.jianghu66.top

const { a = 1, b = 2 } = obj;
来源：http://zsh.ydzc1.top

[U88] JS：对象展开合并
来源：http://jeg.tianlin.xyz

{ ...a, ...b }
来源：http://bbv.tarul.cn

[U89] JS：数组去重
来源：http://jep.yj202588.top

[...new Set(arr)]
来源：http://nxe.zhongyouzk.top

[U90] JS：数字数组排序
来源：http://gvb.zdqjudy.top

[...arr].sort((a, b) => a - b)
来源：http://vit.gzhubu.top

[U91] JS：对象键值遍历
来源：http://nfd.xingfuxueyuan.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kna.zycfv.cn

[U92] JS：深拷贝
来源：http://eus.guowangkeji.top

structuredClone(obj)
来源：http://tam.xylfe.cn

[U93] JS：模板字符串
来源：http://ogu.xingfuxueyuan.xyz

`共 ${n} 条`
来源：http://rmm.zhiwuduotai.top

[U94] JS：箭头函数
来源：http://xvg.jianghu66.top

const double = x => x * 2;
来源：http://llk.tarul.cn

[U95] JS：Promise 包装
来源：http://kxe.zycfv.cn

new Promise((resolve, reject) => {})
来源：http://qqu.xinyue.icu

[U96] JS：async/await 与异常
来源：http://mgj.shanyushiyangkeji.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://aet.aibaodan.cn

[U97] JS：并发请求
来源：http://dhe.tian-w.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://beq.haohaochexian.top

[U98] JS：fetch 带 JSON
来源：http://qhd.guowangkeji.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vkp.svipenyu.cn

[U99] JS：事件监听
来源：http://rid.ybcxt.top

el.addEventListener("click", e => {})
来源：http://gqm.ybcxt.top

[U100] JS：DOM 查询
来源：http://ung.gotoacloud.top

document.querySelector(".item")
来源：http://bru.sjlbkw.cn

[U101] JS：classList 操作
来源：http://elv.hywenlv.cn

el.classList.toggle("active")
来源：http://htv.zhijiandao.cn

[U102] JS：本地存储
来源：http://krd.bjfxy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://oli.yongpay.top

[U103] JS：定时器
来源：http://uov.xingfuxueyuan.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ybx.zhaomingkeji.xyz

[U104] JS：防抖
来源：http://nax.xinyue.icu

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tez.gotoacloud.top

[U105] JS：节流
来源：http://cpo.shanyushiyangkeji.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://faz.jlsjyb.cn

[U106] JS：日期格式化
来源：http://bje.jlsjyb.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://eix.jlsjyb.cn

[U107] JS：数字千分位
来源：http://ept.zhiwuduotai.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yjp.aizwys.cn

[U108] JS：随机整数
来源：http://flu.xuetiantiany.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://sdu.ybcxt.top

[U109] JS：数组分组
来源：http://fot.gotoacloud.top

Object.groupBy(arr, x => x.type)
来源：http://rdr.jiagoushi.top

[U110] JS：数组分块
来源：http://qio.yonumen.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wxg.nanxuanxn.top

[U111] JS：对象转 Map
来源：http://aho.kuanghao11.cn

new Map(Object.entries(obj))
来源：http://dlf.sxryk.cn

[U112] JS：字符串补位
来源：http://eam.chenjidiqi.icu

"7".padStart(3, "0")
来源：http://ywl.haohaochexian.top

[U113] JS：正则替换全部
来源：http://cwx.dashuyun.cn

s.replaceAll("a", "b")
来源：http://hlr.hesvh.cn

[U114] JS：JSON 深比较
来源：http://qgs.hnqzz.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://adr.cheryme.top

[U115] JS：生成 UUID
来源：http://kaf.hammf.cn

crypto.randomUUID()
来源：http://uls.hysaishi.cn

[U116] JS：类型检查（JSDoc）
来源：http://sfv.hnxiangtu.top

/** @param {string} name */ function f(name) {}
来源：http://pni.gogol.net.cn

[U117] JS：单元测试
来源：http://gib.ivvv.top

npm i -D vitest;  npx vitest
来源：http://irn.gzhubu.top

[U118] JS：开发服务器
来源：http://ylh.uphjek.com

npm i -D vite;  npx vite
来源：http://hyw.hnqzz.top

[U119] JS：生产构建
来源：http://ctt.havefunace.top

npx vite build
来源：http://grr.dianchejie.cn

[U120] JS：读取环境变量（Vite）
来源：http://nxe.birdmap.top

import.meta.env.VITE_API_URL
来源：http://eri.gaohongyu789.top

================================================================================
来源：http://psk.zhiwuduotai.top

统计汇总
来源：http://erx.yj20258.top

================================================================================
来源：http://kpc.jyoumei.cn

按语言统计（条）：
来源：http://tan.gaohongyu789.top

Python ......... 252
来源：http://prq.yuanzhike.top

PHP ............ 252
来源：http://gmw.feifeiyinyue.top

JavaScript ..... 252
来源：http://isc.dianchejie.cn

TypeScript ..... 212
来源：http://zjo.xuetiantiany.cn

Java ........... 212
来源：http://vzg.zhoulong.xyz

Go ............. 212
来源：http://xxi.ctjpmb.com

Ruby ........... 212
来源：http://sva.mhx1999.top

C# ............. 212
来源：http://fey.wangshuangyany.cn

C .............. 30
来源：http://awq.jiagoushi.top

C++ ............ 30
来源：http://buj.meibo888.top

SQL ............ 90
来源：http://vxl.jyoumei.cn

Bash ........... 80
来源：http://ayf.hysaishi.cn

Kotlin ......... 15
来源：http://cop.feifeiyinyue.top

Swift .......... 15
来源：http://fxc.gaohongyu789.top

Lua ............ 10
来源：http://kkj.jqgufenzy.top

Perl ........... 10
来源：http://taf.sufxvd.cn

Scala .......... 10
来源：http://xeh.yuanzhike.top

------------------------------------
来源：http://qii.xylfe.cn

合计 ........... 2106 条
来源：http://wuk.andypj.xyz

按章节统计：
来源：http://xhi.ehwqpu.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wsi.wangshuangyany.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://fuw.feifeiyinyue.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://uku.jianghu66.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fek.xingfuxueyuan.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://smm.jqgfzy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qvr.quarkkingdee.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hjm.gzhubu.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://dvx.yuanzhike.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://tdm.shanyushiyangkeji.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://pdn.yj202588.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ffz.ivvv.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ubs.tianlin.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jgi.hywenlv.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wwh.hongshengwenyu.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qau.sysykeji.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://oul.shanyushiyangtech.top

Q SQL 专题                              90
来源：http://sgc.xuanzx.com

R Bash 专题                             80
来源：http://lir.vqdsnc.cn

S C / C++ 专题                          60
来源：http://leh.wangshuangyany.cn

T 其他语言补充                          60
来源：http://nly.jiagoushi.top

U 高频实用片段                         120
来源：http://uux.jlsjyb.cn

------------------------------------
来源：http://fmc.zhixingplan.top

合计                                  2106 条
来源：http://yvo.havefunace.top

--------------------------------------------------------------------------------
来源：http://enh.smart0.xyz

使用提醒
来源：http://nck.mhx1999.top

--------------------------------------------------------------------------------
来源：http://okt.ehwqpu.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://odp.cheryme.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://oac.ivvv.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rub.yangfankeji.com

在旧版本上使用前请先确认语法支持情况。
来源：http://otx.andypj.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zyo.zhixingplan.top

—— 文件结束 ——
来源：http://vdq.hnxiangtu.top

================================================================================
来源：http://qja.c1oappe.top

程序语言常见例子速查手册（2024 版）
来源：http://gpy.yj202588.top

Common Programming Examples Cheat Book
来源：http://gux.fehbvm.com

================================================================================
来源：http://azr.nwbrower.top

【收录内容】
来源：http://lin.pycfn.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://qpv.yanxiufei.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wif.zdbjq.cn

SQL · Bash · C · C++
来源：http://rqi.smart0.xyz

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hal.aizwys.cn

【使用说明】
来源：http://wta.jqgufenzy.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ngc.yuxming.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://oed.jinqigufen.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://sie.cashguo.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zko.cheryme.top

Bash:  Shell         C:     C             C++:   C++
来源：http://dnz.wangshuangyany.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://lyl.ppjwa.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mbn.ctjpmb.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://oat.tian-w.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://gcd.316326.xyz

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gab.smart0.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wxh.shanyushiyangtech.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kee.sufxvd.cn

【文件统计】
来源：http://yzj.ivvv.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://yxc.hfpthk.cn

--------------------------------------------------------------------------------
来源：http://shm.gogol.net.cn

目  录
来源：http://ste.yuxming.cn

--------------------------------------------------------------------------------
来源：http://soy.jlsjyb.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ebf.yj202588.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ihu.birdmap.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://pbt.zhixingplan.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://kov.jqgfzy.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://plq.cashguo.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xwk.zhengqikj.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gpg.cucudq.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://tjs.yongpay.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zpl.9152youxi.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://khc.yonumen.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://fex.meibo888.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://tpu.sysykeji.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://txx.cashguo.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://kwo.yonumen.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://pfi.daria6918.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://jkg.feifeiyinyue.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://evq.bjfxy.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://kfh.hnxiangtu.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://lun.hcnkem.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bbh.ivvv.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://gix.aizwys.cn


<!-- 参考信息 -->