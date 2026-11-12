代发 wailian999

[U23] Py：分块读取大文件
来源：http://ftg.cheryme.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ywh.dianchejie.cn

[U24] Py：路径操作
来源：http://gem.snrcjt.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xyi.tian-w.cn

[U25] Py：CSV 按字典读
来源：http://xid.quarkkingdee.top

csv.DictReader(f)
来源：http://jfj.guannengcc.top

[U26] Py：并发下载
来源：http://iuq.yongpay.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ndi.jianghu66.top

[U27] Py：异步 HTTP
来源：http://owv.jiagoushi.top

aiohttp.ClientSession() 配合 async with
来源：http://dnv.quarkkingdee.top

[U28] Py：类型别名
来源：http://hug.sysykeji.top

UserId = int
来源：http://obg.nanxuanxn.top

[U29] Py：属性校验
来源：http://txb.jinghuilouyu.cn

@property 与 @x.setter 配合
来源：http://jci.nanxinkj.top

[U30] Py：数据类
来源：http://pik.cashguo.top

@dataclass(slots=True)
来源：http://hwr.ydjk.org.cn

[U31] Py：单测
来源：http://awl.bbcook.cn

python -m pytest -q
来源：http://alp.jinqigfzy.top

[U32] Py：代码格式化
来源：http://ste.sweek.top

ruff format . && ruff check --fix .
来源：http://mxt.zycfv.cn

[U33] Py：打包发布
来源：http://thq.zycfv.cn

python -m build  （依赖 pyproject.toml）
来源：http://pdu.meibo888.top

[U34] Py：判断编码
来源：http://tsy.xuanzx.com

chardet.detect(raw)
来源：http://bxz.aibaodan.cn

[U35] Py：发送邮件
来源：http://xmr.daria6918.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://lhw.xuanzx.com

[U36] Py：定时任务
来源：http://ici.52xcode.cn

schedule.every(10).minutes.do(job)
来源：http://ifv.c1oappe.top

[U37] Py：读写 Excel
来源：http://oxy.xingfuxueyuan.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://qqj.vqdsnc.cn

[U38] Py：获取脚本所在目录
来源：http://gmx.wangdashe.top

Path(__file__).resolve().parent
来源：http://ndm.jinqigfzy.top

[U39] Py：判断是否在交互环境
来源：http://lmi.gzhubu.top

sys.stdout.isatty()
来源：http://rtr.hammf.cn

[U40] Py：打印到标准错误
来源：http://hjc.52xcode.cn

print("err", file=sys.stderr)
来源：http://aym.fehbvm.com

[U41] PHP：初始化 Composer 项目
来源：http://twf.cashguo.top

composer init;  composer require guzzlehttp/guzzle
来源：http://zvl.snrcjt.cn

[U42] PHP：PSR-4 自动加载
来源：http://vbt.snrcjt.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jvp.jiagoushi.top

[U43] PHP：声明命名空间
来源：http://ahw.bbcook.cn

namespace App\Http;
来源：http://yvj.nanxuanxn.top

[U44] PHP：开启严格类型
来源：http://btb.zhoulong.xyz

declare(strict_types=1);
来源：http://qcd.yj202588.top

[U45] PHP：类型声明与返回类型
来源：http://cqo.jqgfzy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://sjm.mhx1999.top

[U46] PHP：可空类型
来源：http://yaq.cdnleiting.top

?string $name = null
来源：http://qwg.yangfankeji.com

[U47] PHP：联合类型
来源：http://lbc.shangyingyoupin.top

int|string $id
来源：http://ome.fanxiaobao.xyz

[U48] PHP：纯枚举
来源：http://ydv.shangyingyoupin.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://klq.tian-w.cn

[U49] PHP：只读属性
来源：http://yni.ybcxt.top

public readonly string $name
来源：http://bil.vqdsnc.cn

[U50] PHP：构造器属性提升
来源：http://xco.epnwcf.com

public function __construct(private int $id) {}
来源：http://dwj.tarul.cn

[U51] PHP：数组解构
来源：http://ovw.shanyushiyangtech.top

[$a, $b] = $arr;
来源：http://icz.sweek.top

[U52] PHP：箭头函数
来源：http://ife.yangfankeji.com

$double = fn($x) => $x * 2;
来源：http://hwh.haohaochexian.top

[U53] PHP：空合并运算符
来源：http://nxi.hysaishi.cn

$v = $a ?? $b ?? "default";
来源：http://goo.meibo888.top

[U54] PHP：空安全调用
来源：http://aiw.cucudq.cn

$obj?->method()
来源：http://zmd.shanyushiyangkeji.top

[U55] PHP：match 表达式
来源：http://srn.cdnleiting.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ibf.jqgufenzy.top

[U56] PHP：命名参数
来源：http://atj.svipenyu.cn

f(a: 1, b: 2)
来源：http://ycw.fanxiaobao.xyz

[U57] PHP：字符串插值
来源：http://act.vqdsnc.cn

"值: {$a}"
来源：http://aym.havefunace.top

[U58] PHP：数组三件套
来源：http://tem.andypj.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rzy.snrcjt.cn

[U59] PHP：自定义排序
来源：http://yrj.shanyushiyangtech.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wzl.jinghuilouyu.cn

[U60] PHP：JSON 编解码
来源：http://lkf.aibaodan.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qqa.mhx1999.top

[U61] PHP：正则
来源：http://szt.jianghu66.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://yeq.xingfuxueyuan.xyz

[U62] PHP：日期对象
来源：http://uph.zhengqikj.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://kwc.gaohongyu789.top

[U63] PHP：文件读写
来源：http://pey.meibo888.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ykx.sufxvd.cn

[U64] PHP：目录遍历
来源：http://sfr.feifeiyinyue.top

glob("dir/*.php");  scandir("dir");
来源：http://ksn.jqgufenzy.top

[U65] PHP：会话
来源：http://mqi.yueranfly.top

session_start();  $_SESSION["uid"] = 1;
来源：http://pyc.tanke756.top

[U66] PHP：设置 Cookie
来源：http://vtb.yonumen.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://syu.shangyingyoupin.top

[U67] PHP：处理文件上传
来源：http://sjn.fengsongda.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://sbn.cheryme.top

[U68] PHP：PDO 连接
来源：http://gae.yj202588.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nzr.yj20258.top

[U69] PHP：PDO 预处理
来源：http://fzp.hnqzz.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wog.tian-w.cn

[U70] PHP：PDO 事务
来源：http://rzp.daxiang520.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ffd.yj202588.top

[U71] PHP：抛出异常
来源：http://jzb.hysaishi.cn

throw new RuntimeException("失败", 500);
来源：http://sei.ydjk.org.cn

[U72] PHP：写错误日志
来源：http://oel.daxiang520.top

error_log("失败: " . $e->getMessage());
来源：http://axy.zdqjudy.top

[U73] PHP：读取 ini 配置
来源：http://mdp.vehdjk.com

parse_ini_file("config.ini", true)
来源：http://wbw.xuanzx.com

[U74] PHP：读取环境变量
来源：http://xxj.yongpay.top

getenv("APP_ENV") ?: "production"
来源：http://urr.mhx1999.top

[U75] PHP：依赖注入
来源：http://rjs.jinqigufen.top

composer require psr/container
来源：http://uyy.yueranfly.top

[U76] PHP：简单路由
来源：http://pxb.yongpay.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://utv.sufxvd.cn

[U77] PHP：模板渲染
来源：http://gol.jinqigufen.top

composer require twig/twig
来源：http://eek.zhengqikj.top

[U78] PHP：单元测试
来源：http://ajo.chenzaomai.com

composer require --dev phpunit/phpunit
来源：http://unn.zhijiandao.cn

[U79] PHP：静态分析
来源：http://vtn.jqgufenzy.top

composer require --dev phpstan/phpstan
来源：http://vsh.yanxiufei.cn

[U80] PHP：代码规范修复
来源：http://qdh.aizwys.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://axh.jinqigufen.top

[U81] JS：初始化项目
来源：http://hvo.smart0.xyz

npm init -y;  npm i express
来源：http://rhy.jianghu66.top

[U82] JS：package.json 脚本
来源：http://khh.jinqigfzy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qcv.ppjwa.cn

[U83] JS：ES Module 导入导出
来源：http://qta.ctjpmb.com

export const a = 1;  import { a } from "./m.js";
来源：http://xnn.fanxiaobao.xyz

[U84] JS：CommonJS 写法
来源：http://qdq.sufxvd.cn

module.exports = { a };  const { a } = require("./m");
来源：http://woe.nanxuanxn.top

[U85] JS：可选链
来源：http://cap.cqqwz.cn

a?.b?.c
来源：http://cbc.feifeiyinyue.top

[U86] JS：空值合并
来源：http://ipv.dashuyun.cn

a ?? b
来源：http://rqu.sjlbkw.cn

[U87] JS：解构默认值
来源：http://hdu.bbcook.cn

const { a = 1, b = 2 } = obj;
来源：http://nyh.dashuyun.cn

[U88] JS：对象展开合并
来源：http://ygx.ppjwa.cn

{ ...a, ...b }
来源：http://uqv.yuanzhike.top

[U89] JS：数组去重
来源：http://cvl.hnxiangtu.top

[...new Set(arr)]
来源：http://dfm.hysaishi.cn

[U90] JS：数字数组排序
来源：http://ijl.andypj.xyz

[...arr].sort((a, b) => a - b)
来源：http://otq.epnwcf.com

[U91] JS：对象键值遍历
来源：http://xym.hammf.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://thl.yuanzhike.top

[U92] JS：深拷贝
来源：http://ngt.nanxinkj.top

structuredClone(obj)
来源：http://cqb.hfpthk.cn

[U93] JS：模板字符串
来源：http://fbk.tian-w.cn

`共 ${n} 条`
来源：http://nuh.cdnleiting.top

[U94] JS：箭头函数
来源：http://lag.epnwcf.com

const double = x => x * 2;
来源：http://nqq.redwolf501.top

[U95] JS：Promise 包装
来源：http://oif.52xcode.cn

new Promise((resolve, reject) => {})
来源：http://slb.jqgufenzy.top

[U96] JS：async/await 与异常
来源：http://bfp.daxiang520.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xmo.52xcode.cn

[U97] JS：并发请求
来源：http://akt.cashguo.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://nch.9152youxi.cn

[U98] JS：fetch 带 JSON
来源：http://fjq.gaohongyu789.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fib.shzxlz.cn

[U99] JS：事件监听
来源：http://teq.xinyue.icu

el.addEventListener("click", e => {})
来源：http://ujg.tian-w.cn

[U100] JS：DOM 查询
来源：http://hmd.kuanghao11.cn

document.querySelector(".item")
来源：http://dlx.haohaochexian.top

[U101] JS：classList 操作
来源：http://xhz.xuanzx.com

el.classList.toggle("active")
来源：http://hkd.hnxiangtu.top

[U102] JS：本地存储
来源：http://efv.hywenlv.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://uap.zdbjq.cn

[U103] JS：定时器
来源：http://jny.xinyue.icu

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tgs.fehbvm.com

[U104] JS：防抖
来源：http://vks.0kj1m.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://imn.wangshuangyany.cn

[U105] JS：节流
来源：http://ozz.c1oappe.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vil.sysykeji.top

[U106] JS：日期格式化
来源：http://usd.fanxiaobao.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rma.yangfankeji.com

[U107] JS：数字千分位
来源：http://sms.tianlin.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ntz.nwbrower.top

[U108] JS：随机整数
来源：http://sjp.shuidangran.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ozt.xuanzx.com

[U109] JS：数组分组
来源：http://vhp.yj202588.top

Object.groupBy(arr, x => x.type)
来源：http://cmv.ivvv.top

[U110] JS：数组分块
来源：http://qni.ydzc1.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lto.cheryme.top

[U111] JS：对象转 Map
来源：http://kii.hammf.cn

new Map(Object.entries(obj))
来源：http://noe.jlsjyb.cn

[U112] JS：字符串补位
来源：http://mdt.nwbrower.top

"7".padStart(3, "0")
来源：http://sai.gotoacloud.top

[U113] JS：正则替换全部
来源：http://zse.cqqwz.cn

s.replaceAll("a", "b")
来源：http://gue.gzhubu.top

[U114] JS：JSON 深比较
来源：http://mzr.fzhhl.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ryl.ybcxt.top

[U115] JS：生成 UUID
来源：http://tfd.ydjk.org.cn

crypto.randomUUID()
来源：http://lwc.sysykeji.top

[U116] JS：类型检查（JSDoc）
来源：http://ojt.9152youxi.cn

/** @param {string} name */ function f(name) {}
来源：http://oru.zdqjudy.top

[U117] JS：单元测试
来源：http://hhn.hesvh.cn

npm i -D vitest;  npx vitest
来源：http://rxf.jiagoushi.top

[U118] JS：开发服务器
来源：http://ubd.daria6918.cn

npm i -D vite;  npx vite
来源：http://ayn.sysykeji.top

[U119] JS：生产构建
来源：http://tzq.hcnkem.com

npx vite build
来源：http://pus.dianchejie.cn

[U120] JS：读取环境变量（Vite）
来源：http://yil.yonumen.top

import.meta.env.VITE_API_URL
来源：http://vbl.xylfe.cn

================================================================================
来源：http://sjt.yj20258.top

统计汇总
来源：http://xez.fanxiaobao.xyz

================================================================================
来源：http://acx.gogol.net.cn

按语言统计（条）：
来源：http://jcf.yueranfly.top

Python ......... 252
来源：http://gsz.vqdsnc.cn

PHP ............ 252
来源：http://ajd.jinqigfzy.top

JavaScript ..... 252
来源：http://nhx.jqgfzy.top

TypeScript ..... 212
来源：http://kcj.cashguo.top

Java ........... 212
来源：http://dcw.zycfv.cn

Go ............. 212
来源：http://vdk.vehdjk.com

Ruby ........... 212
来源：http://dgy.zhoulong.xyz

C# ............. 212
来源：http://qgp.snrcjt.cn

C .............. 30
来源：http://hlv.jinqigfzy.top

C++ ............ 30
来源：http://wtb.hysaishi.cn

SQL ............ 90
来源：http://vhy.yj20258888.top

Bash ........... 80
来源：http://vvn.yuxming.cn

Kotlin ......... 15
来源：http://ybv.cucudq.cn

Swift .......... 15
来源：http://tiv.ivvv.top

Lua ............ 10
来源：http://hhh.bbcook.cn

Perl ........... 10
来源：http://rlw.tian-w.cn

Scala .......... 10
来源：http://kyb.yj202588.top

------------------------------------
来源：http://ezq.gaohongyu789.top

合计 ........... 2106 条
来源：http://wux.redwolf501.top

按章节统计：
来源：http://yuw.shzxlz.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://cud.9152youxi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mum.guannengcc.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://kud.svipenyu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://cho.cucudq.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jfi.guannengcc.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dmq.jianghu66.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kju.jqgfzy.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://bew.yuxming.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://dar.kuanghao11.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zgg.sjlbkw.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://whs.xuetiantiany.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://duy.jinqigfzy.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mbc.sufxvd.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://yhb.jiagoushi.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ibx.xuanzx.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wck.quarkkingdee.top

Q SQL 专题                              90
来源：http://wgr.daria6918.cn

R Bash 专题                             80
来源：http://gqz.ybcxt.top

S C / C++ 专题                          60
来源：http://ubd.xylfe.cn

T 其他语言补充                          60
来源：http://tef.nanxinkj.top

U 高频实用片段                         120
来源：http://fkz.xuanzx.com

------------------------------------
来源：http://ktu.iojbl.cn

合计                                  2106 条
来源：http://uys.jinyuanbaomall.cn

--------------------------------------------------------------------------------
来源：http://amm.yongpay.top

使用提醒
来源：http://jjy.shanyushiyangkeji.top

--------------------------------------------------------------------------------
来源：http://mgk.zhengqikj.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://scs.zhijiandao.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xwp.yfazqb.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fej.sxryk.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://tof.tian-w.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://fin.zhijiandao.cn

—— 文件结束 ——
来源：http://vin.jinqigufen.top

================================================================================
来源：http://gsb.ybcxt.top

程序语言常见例子速查手册（2024 版）
来源：http://cdu.tian-w.cn

Common Programming Examples Cheat Book
来源：http://ecz.cqqwz.cn

================================================================================
来源：http://zgz.tarul.cn

【收录内容】
来源：http://nhp.dianchejie.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ytp.jqgufenzy.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://dzz.cashguo.top

SQL · Bash · C · C++
来源：http://xdu.zhoulong.xyz

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://usr.andypj.xyz

【使用说明】
来源：http://apd.haohaochexian.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cek.cheryme.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://oms.ehwqpu.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://tyx.xinyue.icu

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zmi.ydzc1.top

Bash:  Shell         C:     C             C++:   C++
来源：http://axu.iojbl.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zwk.snrcjt.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://asr.birdmap.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jjp.gzhubu.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://zqs.nanxuanxn.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://aor.hywenlv.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://zbh.jqgufenzy.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vcs.shangyingyoupin.top

【文件统计】
来源：http://xaz.yfazqb.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cyb.sysykeji.top

--------------------------------------------------------------------------------
来源：http://xdi.mhx1999.top

目  录
来源：http://qzz.uphjek.com

--------------------------------------------------------------------------------
来源：http://wwa.vqdsnc.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://uxn.daxiang520.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://vhh.gotoacloud.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://xss.kuanghao11.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://tpq.pycfn.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://dqf.vehdjk.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://cdm.kuanghao11.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mrt.jinqigufen.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://uea.hnxiangtu.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://cva.bjfxy.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fss.nanxinkj.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zpi.chenjidiqi.icu

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://caz.cheryme.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://kub.yj202588.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://tqq.sxryk.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lno.yangfankeji.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://dxs.ydjk.org.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mzg.kuanghao11.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://boj.wangshuangyany.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ggq.316326.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://zgn.aibaodan.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://sjw.jqgufenzy.top


<!-- 参考信息 -->