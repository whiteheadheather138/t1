代发 wailian999

[U23] Py：分块读取大文件
来源：http://zjs.guowangkeji.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://prd.sufxvd.cn

[U24] Py：路径操作
来源：http://vvh.hcnkem.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hvv.hywenlv.cn

[U25] Py：CSV 按字典读
来源：http://zbt.xingfuxueyuan.xyz

csv.DictReader(f)
来源：http://tfw.tianlin.xyz

[U26] Py：并发下载
来源：http://vjz.ehwqpu.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ltq.chenjidiqi.icu

[U27] Py：异步 HTTP
来源：http://tux.pengpengdd.cyou

aiohttp.ClientSession() 配合 async with
来源：http://nic.c1oappe.top

[U28] Py：类型别名
来源：http://low.ctjpmb.com

UserId = int
来源：http://cyu.cdnleiting.top

[U29] Py：属性校验
来源：http://sxl.jqgfzy.top

@property 与 @x.setter 配合
来源：http://pab.dianchejie.cn

[U30] Py：数据类
来源：http://iwh.snrcjt.cn

@dataclass(slots=True)
来源：http://riv.hnxiangtu.top

[U31] Py：单测
来源：http://jnf.aizwys.cn

python -m pytest -q
来源：http://fwc.gzhubu.top

[U32] Py：代码格式化
来源：http://mmc.sjlbkw.cn

ruff format . && ruff check --fix .
来源：http://fje.shanyushiyangtech.top

[U33] Py：打包发布
来源：http://uaw.hammf.cn

python -m build  （依赖 pyproject.toml）
来源：http://fee.shangyingyoupin.top

[U34] Py：判断编码
来源：http://jut.ydzc1.top

chardet.detect(raw)
来源：http://xup.0kj1m.cn

[U35] Py：发送邮件
来源：http://fze.jiagoushi.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://owu.hammf.cn

[U36] Py：定时任务
来源：http://hvp.hammf.cn

schedule.every(10).minutes.do(job)
来源：http://onl.yvedp.cn

[U37] Py：读写 Excel
来源：http://yzp.hnxiangtu.top

pandas.read_excel / DataFrame.to_excel
来源：http://fhn.haohaochexian.top

[U38] Py：获取脚本所在目录
来源：http://qfi.epnwcf.com

Path(__file__).resolve().parent
来源：http://rdl.cqqwz.cn

[U39] Py：判断是否在交互环境
来源：http://rec.c1oappe.top

sys.stdout.isatty()
来源：http://zkp.jinqigfzy.top

[U40] Py：打印到标准错误
来源：http://hxl.jqgfzy.top

print("err", file=sys.stderr)
来源：http://ily.uphjek.com

[U41] PHP：初始化 Composer 项目
来源：http://sku.hesvh.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://hib.hfpthk.cn

[U42] PHP：PSR-4 自动加载
来源：http://axi.yonumen.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xco.tianlin.xyz

[U43] PHP：声明命名空间
来源：http://gif.feifeiyinyue.top

namespace App\Http;
来源：http://mua.bjfxy.top

[U44] PHP：开启严格类型
来源：http://mag.zhongyouzk.top

declare(strict_types=1);
来源：http://spp.ybcxt.top

[U45] PHP：类型声明与返回类型
来源：http://nvc.yj20258.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://xfe.tianlin.xyz

[U46] PHP：可空类型
来源：http://dzy.birdmap.top

?string $name = null
来源：http://hcz.52xcode.cn

[U47] PHP：联合类型
来源：http://adm.pycfn.com

int|string $id
来源：http://fgk.aibaodan.cn

[U48] PHP：纯枚举
来源：http://osr.jianghu66.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://otf.tarul.cn

[U49] PHP：只读属性
来源：http://bci.uphjek.com

public readonly string $name
来源：http://zfm.wangshuangyany.cn

[U50] PHP：构造器属性提升
来源：http://rkq.xuetiantiany.cn

public function __construct(private int $id) {}
来源：http://gcn.zhengqikj.top

[U51] PHP：数组解构
来源：http://vyj.ctjpmb.com

[$a, $b] = $arr;
来源：http://znp.zdbjq.cn

[U52] PHP：箭头函数
来源：http://bty.zhengqikj.top

$double = fn($x) => $x * 2;
来源：http://afq.yanxiufei.cn

[U53] PHP：空合并运算符
来源：http://wgf.cucudq.cn

$v = $a ?? $b ?? "default";
来源：http://jni.gaohongyu789.top

[U54] PHP：空安全调用
来源：http://vuw.ydjk.org.cn

$obj?->method()
来源：http://yao.ybcxt.top

[U55] PHP：match 表达式
来源：http://kvs.aibaodan.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xte.zhoulong.xyz

[U56] PHP：命名参数
来源：http://lbb.vqdsnc.cn

f(a: 1, b: 2)
来源：http://kft.ehwqpu.com

[U57] PHP：字符串插值
来源：http://tcr.xingfuxueyuan.xyz

"值: {$a}"
来源：http://ixo.yueranfly.top

[U58] PHP：数组三件套
来源：http://ojn.sxryk.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kly.yj20258.top

[U59] PHP：自定义排序
来源：http://ypl.zhongyouzk.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gdq.birdmap.top

[U60] PHP：JSON 编解码
来源：http://hnl.iojbl.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ldz.nanxinkj.top

[U61] PHP：正则
来源：http://csz.gaohongyu789.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://urf.shanyushiyangkeji.top

[U62] PHP：日期对象
来源：http://uub.xinyue.icu

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wot.shuidangran.top

[U63] PHP：文件读写
来源：http://zzt.gzhubu.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://nzo.fzhhl.top

[U64] PHP：目录遍历
来源：http://ids.snrcjt.cn

glob("dir/*.php");  scandir("dir");
来源：http://ufj.andypj.xyz

[U65] PHP：会话
来源：http://gwp.zhixingplan.top

session_start();  $_SESSION["uid"] = 1;
来源：http://amb.9152youxi.cn

[U66] PHP：设置 Cookie
来源：http://rlg.havefunace.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xan.sxryk.cn

[U67] PHP：处理文件上传
来源：http://tyl.sjlbkw.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kti.cqqwz.cn

[U68] PHP：PDO 连接
来源：http://niv.zhoulong.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://djk.pycfn.com

[U69] PHP：PDO 预处理
来源：http://krl.fehbvm.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://pyo.smart0.xyz

[U70] PHP：PDO 事务
来源：http://muj.ehwqpu.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kqy.fehbvm.com

[U71] PHP：抛出异常
来源：http://wse.jinqigufen.top

throw new RuntimeException("失败", 500);
来源：http://fcd.ydjk.org.cn

[U72] PHP：写错误日志
来源：http://qkc.hysaishi.cn

error_log("失败: " . $e->getMessage());
来源：http://ksi.jlsjyb.cn

[U73] PHP：读取 ini 配置
来源：http://rvl.yuanzhike.top

parse_ini_file("config.ini", true)
来源：http://ytp.xziqi.cn

[U74] PHP：读取环境变量
来源：http://lzz.yj202588.top

getenv("APP_ENV") ?: "production"
来源：http://ywy.sxryk.cn

[U75] PHP：依赖注入
来源：http://mze.havefunace.top

composer require psr/container
来源：http://qyw.shanyushiyangkeji.top

[U76] PHP：简单路由
来源：http://hhr.hammf.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ylm.jqgfzy.top

[U77] PHP：模板渲染
来源：http://puq.cqqwz.cn

composer require twig/twig
来源：http://orl.bbcook.cn

[U78] PHP：单元测试
来源：http://bma.shuidangran.top

composer require --dev phpunit/phpunit
来源：http://rcq.guannengcc.top

[U79] PHP：静态分析
来源：http://cmg.jqgfzy.top

composer require --dev phpstan/phpstan
来源：http://qgn.pycfn.com

[U80] PHP：代码规范修复
来源：http://sqc.jinqigufen.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://zjl.dashuyun.cn

[U81] JS：初始化项目
来源：http://pva.wangdashe.top

npm init -y;  npm i express
来源：http://eiw.wangdashe.top

[U82] JS：package.json 脚本
来源：http://soh.nanxuanxn.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://aeh.pengpengdd.cyou

[U83] JS：ES Module 导入导出
来源：http://qqe.tarul.cn

export const a = 1;  import { a } from "./m.js";
来源：http://obq.zdqjudy.top

[U84] JS：CommonJS 写法
来源：http://ntn.svipenyu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://zjf.ctjpmb.com

[U85] JS：可选链
来源：http://pvl.sufxvd.cn

a?.b?.c
来源：http://vpu.smart0.xyz

[U86] JS：空值合并
来源：http://bwp.jinqigfzy.top

a ?? b
来源：http://azw.zhiwuduotai.top

[U87] JS：解构默认值
来源：http://psd.tarul.cn

const { a = 1, b = 2 } = obj;
来源：http://flk.fengsongda.top

[U88] JS：对象展开合并
来源：http://tes.sufxvd.cn

{ ...a, ...b }
来源：http://cim.chenlongwang.top

[U89] JS：数组去重
来源：http://fcb.ivvv.top

[...new Set(arr)]
来源：http://xel.yongpay.top

[U90] JS：数字数组排序
来源：http://sst.pengpengdd.cyou

[...arr].sort((a, b) => a - b)
来源：http://fti.xuetiantiany.cn

[U91] JS：对象键值遍历
来源：http://rtf.kuanghao11.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://yfz.hywenlv.cn

[U92] JS：深拷贝
来源：http://fpw.kuanghao11.cn

structuredClone(obj)
来源：http://nuz.chenlongwang.top

[U93] JS：模板字符串
来源：http://cil.hfpthk.cn

`共 ${n} 条`
来源：http://qxh.zhoulong.xyz

[U94] JS：箭头函数
来源：http://zme.hywenlv.cn

const double = x => x * 2;
来源：http://ehz.bjfxy.top

[U95] JS：Promise 包装
来源：http://aui.hcnkem.com

new Promise((resolve, reject) => {})
来源：http://msi.ehwqpu.com

[U96] JS：async/await 与异常
来源：http://mwh.cqqwz.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://kme.zhoulong.xyz

[U97] JS：并发请求
来源：http://ekk.jlsjyb.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://edq.shuidangran.top

[U98] JS：fetch 带 JSON
来源：http://fck.ywan-chungtsiang.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bjy.tanke756.top

[U99] JS：事件监听
来源：http://uzv.gotoacloud.top

el.addEventListener("click", e => {})
来源：http://ixs.epnwcf.com

[U100] JS：DOM 查询
来源：http://mnq.jinyuanbaomall.cn

document.querySelector(".item")
来源：http://xvn.jinghuilouyu.cn

[U101] JS：classList 操作
来源：http://rpi.zhaomingkeji.xyz

el.classList.toggle("active")
来源：http://gtg.havefunace.top

[U102] JS：本地存储
来源：http://jlz.c1oappe.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://xlf.cdnleiting.top

[U103] JS：定时器
来源：http://fgf.jqgufenzy.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://aun.andypj.xyz

[U104] JS：防抖
来源：http://pry.shanyushiyangkeji.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ffk.chenzaomai.com

[U105] JS：节流
来源：http://htc.jinqigfzy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://phk.andypj.xyz

[U106] JS：日期格式化
来源：http://rdt.shuidangran.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://uut.cashguo.top

[U107] JS：数字千分位
来源：http://yyt.jinqigufen.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zog.daxiang520.top

[U108] JS：随机整数
来源：http://ggh.zhongyouzk.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pjh.sxryk.cn

[U109] JS：数组分组
来源：http://zka.uphjek.com

Object.groupBy(arr, x => x.type)
来源：http://hlv.zhoulong.xyz

[U110] JS：数组分块
来源：http://tui.gzhubu.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zvu.zycfv.cn

[U111] JS：对象转 Map
来源：http://ays.yuanzhike.top

new Map(Object.entries(obj))
来源：http://gdi.snrcjt.cn

[U112] JS：字符串补位
来源：http://ahw.smart0.xyz

"7".padStart(3, "0")
来源：http://eid.0kj1m.cn

[U113] JS：正则替换全部
来源：http://wyw.ybcxt.top

s.replaceAll("a", "b")
来源：http://gdj.hesvh.cn

[U114] JS：JSON 深比较
来源：http://dbl.bjfxy.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://qya.zycfv.cn

[U115] JS：生成 UUID
来源：http://giq.zycfv.cn

crypto.randomUUID()
来源：http://rzt.yj20258.top

[U116] JS：类型检查（JSDoc）
来源：http://ype.hongshengwenyu.top

/** @param {string} name */ function f(name) {}
来源：http://ecf.pengpengdd.cyou

[U117] JS：单元测试
来源：http://cno.fzhhl.top

npm i -D vitest;  npx vitest
来源：http://ltm.chenzaomai.com

[U118] JS：开发服务器
来源：http://eke.iojbl.cn

npm i -D vite;  npx vite
来源：http://gyh.xuetiantiany.cn

[U119] JS：生产构建
来源：http://xgw.yuanzhike.top

npx vite build
来源：http://jfy.gzhubu.top

[U120] JS：读取环境变量（Vite）
来源：http://khw.vqdsnc.cn

import.meta.env.VITE_API_URL
来源：http://ine.xuanzx.com

================================================================================
来源：http://via.52xcode.cn

统计汇总
来源：http://duq.shuidangran.top

================================================================================
来源：http://iax.bbcook.cn

按语言统计（条）：
来源：http://mmb.jlsjyb.cn

Python ......... 252
来源：http://low.bbcook.cn

PHP ............ 252
来源：http://ywx.hesvh.cn

JavaScript ..... 252
来源：http://fvt.hesvh.cn

TypeScript ..... 212
来源：http://qli.hesvh.cn

Java ........... 212
来源：http://asm.pengpengdd.cyou

Go ............. 212
来源：http://ten.daria6918.cn

Ruby ........... 212
来源：http://kxi.hammf.cn

C# ............. 212
来源：http://buy.fengsongda.top

C .............. 30
来源：http://ojp.yj202588.top

C++ ............ 30
来源：http://jjf.sufxvd.cn

SQL ............ 90
来源：http://mhu.yj202588.top

Bash ........... 80
来源：http://hin.tian-w.cn

Kotlin ......... 15
来源：http://fsw.sufxvd.cn

Swift .......... 15
来源：http://iiz.vehdjk.com

Lua ............ 10
来源：http://hqi.zhaomingkeji.xyz

Perl ........... 10
来源：http://xjh.yuanzhike.top

Scala .......... 10
来源：http://ipi.jinqigufen.top

------------------------------------
来源：http://bbd.cqqwz.cn

合计 ........... 2106 条
来源：http://efz.hfpthk.cn

按章节统计：
来源：http://vms.0kj1m.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://yih.nanxinkj.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tdg.zhaomingkeji.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dys.jinghuilouyu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://njr.jlsjyb.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://oqj.wangdashe.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://evf.aizwys.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://scl.cheryme.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wgv.hnqzz.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xsp.gzhubu.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://lpx.quarkkingdee.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vjh.redwolf501.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://pud.zycfv.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ykm.kuanghao11.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://voc.tanke756.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wwj.ybcxt.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vug.chenzaomai.com

Q SQL 专题                              90
来源：http://mce.cheryme.top

R Bash 专题                             80
来源：http://iyd.iojbl.cn

S C / C++ 专题                          60
来源：http://bxw.gzhubu.top

T 其他语言补充                          60
来源：http://trv.jiagoushi.top

U 高频实用片段                         120
来源：http://lfm.xingfuxueyuan.xyz

------------------------------------
来源：http://guk.pengpengdd.cyou

合计                                  2106 条
来源：http://ryk.hfpthk.cn

--------------------------------------------------------------------------------
来源：http://fcj.wangshuangyany.cn

使用提醒
来源：http://njp.haohaochexian.top

--------------------------------------------------------------------------------
来源：http://vrk.fzhhl.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fsp.wangdashe.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://qsp.jqgufenzy.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://tcu.shzxlz.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ovi.xingfuxueyuan.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://dmn.zhijiandao.cn

—— 文件结束 ——
来源：http://ldh.havefunace.top

================================================================================
来源：http://jpa.tanke756.top

程序语言常见例子速查手册（2024 版）
来源：http://fxf.chenzaomai.com

Common Programming Examples Cheat Book
来源：http://tfi.jyoumei.cn

================================================================================
来源：http://mfa.bjfxy.top

【收录内容】
来源：http://zqz.aizwys.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://bxn.xuanzx.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ecw.jinqigfzy.top

SQL · Bash · C · C++
来源：http://ymf.tian-w.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qfm.9152youxi.cn

【使用说明】
来源：http://hwj.feifeiyinyue.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://fif.cqqwz.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://dgf.sxryk.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://szd.nwbrower.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hgj.hongshengwenyu.top

Bash:  Shell         C:     C             C++:   C++
来源：http://rgr.0kj1m.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://igh.hnxiangtu.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://jxf.hesvh.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ylb.yongpay.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://slx.zhijiandao.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://vvn.havefunace.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://okn.dianchejie.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zpf.haohaochexian.top

【文件统计】
来源：http://htz.andypj.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://yrc.fktsv.cn

--------------------------------------------------------------------------------
来源：http://irq.ydjk.org.cn

目  录
来源：http://lxu.nanxuanxn.top

--------------------------------------------------------------------------------
来源：http://hhu.gzhubu.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ded.yanxiufei.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://nxq.gzhubu.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://nnv.mhx1999.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://oud.feifeiyinyue.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://rmx.daria6918.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://bgd.tian-w.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mqg.hfpthk.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://jph.dianchejie.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://cjz.gogol.net.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://nsl.0kj1m.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zvm.zycfv.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://iau.xylfe.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://aph.shuidangran.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://nqp.yj20258888.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jfl.xuanzx.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ngc.zdbjq.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://rim.aizwys.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://hgs.zdqjudy.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qol.guannengcc.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://tig.0kj1m.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://pxz.haohaochexian.top


<!-- 参考信息 -->