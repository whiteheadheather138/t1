代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://brq.meibo888.top

@contextlib.contextmanager
来源：http://aiv.hywenlv.cn

[U22] Py：矩阵转置
来源：http://qvx.hongshengwenyu.top

list(zip(*m))
来源：http://mql.zhiwuduotai.top

[U23] Py：分块读取大文件
来源：http://mea.jinghuilouyu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qay.gogol.net.cn

[U24] Py：路径操作
来源：http://vhs.yongpay.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://koj.zhengqikj.top

[U25] Py：CSV 按字典读
来源：http://dhl.vqdsnc.cn

csv.DictReader(f)
来源：http://lbf.quarkkingdee.top

[U26] Py：并发下载
来源：http://pbi.yueranfly.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zrp.zhongyouzk.top

[U27] Py：异步 HTTP
来源：http://ujf.hongshengwenyu.top

aiohttp.ClientSession() 配合 async with
来源：http://ryr.quarkkingdee.top

[U28] Py：类型别名
来源：http://eqs.tarul.cn

UserId = int
来源：http://thd.yuxming.cn

[U29] Py：属性校验
来源：http://iam.sxryk.cn

@property 与 @x.setter 配合
来源：http://lco.iojbl.cn

[U30] Py：数据类
来源：http://swf.fzhhl.top

@dataclass(slots=True)
来源：http://kqf.shangyingyoupin.top

[U31] Py：单测
来源：http://yhv.hcnkem.com

python -m pytest -q
来源：http://gos.snrcjt.cn

[U32] Py：代码格式化
来源：http://xeu.zdqjudy.top

ruff format . && ruff check --fix .
来源：http://egg.316326.xyz

[U33] Py：打包发布
来源：http://hnb.hnxiangtu.top

python -m build  （依赖 pyproject.toml）
来源：http://cvm.cucudq.cn

[U34] Py：判断编码
来源：http://wlw.dianchejie.cn

chardet.detect(raw)
来源：http://fea.yj20258.top

[U35] Py：发送邮件
来源：http://tol.hongshengwenyu.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pbl.cheryme.top

[U36] Py：定时任务
来源：http://yvx.yangfankeji.com

schedule.every(10).minutes.do(job)
来源：http://uzz.ivvv.top

[U37] Py：读写 Excel
来源：http://irg.jiagoushi.top

pandas.read_excel / DataFrame.to_excel
来源：http://kru.kuanghao11.cn

[U38] Py：获取脚本所在目录
来源：http://bjv.jinqigfzy.top

Path(__file__).resolve().parent
来源：http://ozz.sweek.top

[U39] Py：判断是否在交互环境
来源：http://cys.gzhubu.top

sys.stdout.isatty()
来源：http://wxk.vehdjk.com

[U40] Py：打印到标准错误
来源：http://lfo.zdbjq.cn

print("err", file=sys.stderr)
来源：http://ezj.jinyuanbaomall.cn

[U41] PHP：初始化 Composer 项目
来源：http://vdz.yangfankeji.com

composer init;  composer require guzzlehttp/guzzle
来源：http://omh.ywan-chungtsiang.top

[U42] PHP：PSR-4 自动加载
来源：http://pdj.bbcook.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://epv.dianchejie.cn

[U43] PHP：声明命名空间
来源：http://gty.redwolf501.top

namespace App\Http;
来源：http://vnf.ybcxt.top

[U44] PHP：开启严格类型
来源：http://obb.ctjpmb.com

declare(strict_types=1);
来源：http://rlk.yj20258.top

[U45] PHP：类型声明与返回类型
来源：http://yae.jinghuilouyu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://cef.cheryme.top

[U46] PHP：可空类型
来源：http://dea.ctjpmb.com

?string $name = null
来源：http://bin.cheryme.top

[U47] PHP：联合类型
来源：http://uhb.ydzc1.top

int|string $id
来源：http://phg.9152youxi.cn

[U48] PHP：纯枚举
来源：http://pua.zdqjudy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qjo.yongpay.top

[U49] PHP：只读属性
来源：http://foo.sjlbkw.cn

public readonly string $name
来源：http://ivn.bjfxy.top

[U50] PHP：构造器属性提升
来源：http://agd.havefunace.top

public function __construct(private int $id) {}
来源：http://emk.fengsongda.top

[U51] PHP：数组解构
来源：http://nys.zhengqikj.top

[$a, $b] = $arr;
来源：http://mlu.yonumen.top

[U52] PHP：箭头函数
来源：http://ugx.shuidangran.top

$double = fn($x) => $x * 2;
来源：http://pnj.shuidangran.top

[U53] PHP：空合并运算符
来源：http://xnq.vqdsnc.cn

$v = $a ?? $b ?? "default";
来源：http://vhy.hongshengwenyu.top

[U54] PHP：空安全调用
来源：http://hls.wangshuangyany.cn

$obj?->method()
来源：http://eqe.hcnkem.com

[U55] PHP：match 表达式
来源：http://xvj.jinqigufen.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jkl.svipenyu.cn

[U56] PHP：命名参数
来源：http://mtx.sufxvd.cn

f(a: 1, b: 2)
来源：http://tzp.fengsongda.top

[U57] PHP：字符串插值
来源：http://uic.hfpthk.cn

"值: {$a}"
来源：http://hpw.daria6918.cn

[U58] PHP：数组三件套
来源：http://fye.hesvh.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jef.gogol.net.cn

[U59] PHP：自定义排序
来源：http://wtg.pycfn.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wxx.gaohongyu789.top

[U60] PHP：JSON 编解码
来源：http://qzc.svipenyu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://smi.pengpengdd.cyou

[U61] PHP：正则
来源：http://ijc.smart0.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ubk.havefunace.top

[U62] PHP：日期对象
来源：http://dfn.sysykeji.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ind.birdmap.top

[U63] PHP：文件读写
来源：http://vpv.jinghuilouyu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://aoe.nwbrower.top

[U64] PHP：目录遍历
来源：http://fub.havefunace.top

glob("dir/*.php");  scandir("dir");
来源：http://gug.chenzaomai.com

[U65] PHP：会话
来源：http://smk.jyoumei.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://qlf.gaohongyu789.top

[U66] PHP：设置 Cookie
来源：http://jad.ydzc1.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kjb.zdqjudy.top

[U67] PHP：处理文件上传
来源：http://ynj.zycfv.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ngo.shanyushiyangtech.top

[U68] PHP：PDO 连接
来源：http://aix.hnqzz.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xja.iojbl.cn

[U69] PHP：PDO 预处理
来源：http://wua.xylfe.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wmf.svipenyu.cn

[U70] PHP：PDO 事务
来源：http://rkt.yonumen.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://cyf.vehdjk.com

[U71] PHP：抛出异常
来源：http://srg.shzxlz.cn

throw new RuntimeException("失败", 500);
来源：http://mpg.ehwqpu.com

[U72] PHP：写错误日志
来源：http://ekl.9152youxi.cn

error_log("失败: " . $e->getMessage());
来源：http://xgu.hammf.cn

[U73] PHP：读取 ini 配置
来源：http://rpl.shangyingyoupin.top

parse_ini_file("config.ini", true)
来源：http://kou.c1oappe.top

[U74] PHP：读取环境变量
来源：http://iwc.jqgfzy.top

getenv("APP_ENV") ?: "production"
来源：http://wbb.zdbjq.cn

[U75] PHP：依赖注入
来源：http://yms.sjlbkw.cn

composer require psr/container
来源：http://dvo.yonumen.top

[U76] PHP：简单路由
来源：http://epk.ydzc1.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://exr.haohaochexian.top

[U77] PHP：模板渲染
来源：http://wna.316326.xyz

composer require twig/twig
来源：http://oes.cqqwz.cn

[U78] PHP：单元测试
来源：http://cod.vqdsnc.cn

composer require --dev phpunit/phpunit
来源：http://ate.meibo888.top

[U79] PHP：静态分析
来源：http://jar.tian-w.cn

composer require --dev phpstan/phpstan
来源：http://gqa.iojbl.cn

[U80] PHP：代码规范修复
来源：http://kjn.nanxinkj.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://phe.hcnkem.com

[U81] JS：初始化项目
来源：http://fyw.yanxiufei.cn

npm init -y;  npm i express
来源：http://wsf.aibaodan.cn

[U82] JS：package.json 脚本
来源：http://qan.yvedp.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://oay.guowangkeji.top

[U83] JS：ES Module 导入导出
来源：http://cyq.fzhhl.top

export const a = 1;  import { a } from "./m.js";
来源：http://cbp.vqdsnc.cn

[U84] JS：CommonJS 写法
来源：http://isv.wangdashe.top

module.exports = { a };  const { a } = require("./m");
来源：http://npw.xuanzx.com

[U85] JS：可选链
来源：http://jgb.jinghuilouyu.cn

a?.b?.c
来源：http://vpk.yangfankeji.com

[U86] JS：空值合并
来源：http://ufn.cucudq.cn

a ?? b
来源：http://qqe.0kj1m.cn

[U87] JS：解构默认值
来源：http://kao.havefunace.top

const { a = 1, b = 2 } = obj;
来源：http://ved.shzxlz.cn

[U88] JS：对象展开合并
来源：http://rxv.shuidangran.top

{ ...a, ...b }
来源：http://upu.dianchejie.cn

[U89] JS：数组去重
来源：http://jgb.xinyue.icu

[...new Set(arr)]
来源：http://rbb.xuetiantiany.cn

[U90] JS：数字数组排序
来源：http://tyt.dashuyun.cn

[...arr].sort((a, b) => a - b)
来源：http://cmm.shanyushiyangtech.top

[U91] JS：对象键值遍历
来源：http://uyn.hysaishi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jio.hnqzz.top

[U92] JS：深拷贝
来源：http://ayq.yonumen.top

structuredClone(obj)
来源：http://kll.gzhubu.top

[U93] JS：模板字符串
来源：http://xev.shzxlz.cn

`共 ${n} 条`
来源：http://fab.jiagoushi.top

[U94] JS：箭头函数
来源：http://euo.dashuyun.cn

const double = x => x * 2;
来源：http://cge.shanyushiyangtech.top

[U95] JS：Promise 包装
来源：http://zaw.vehdjk.com

new Promise((resolve, reject) => {})
来源：http://fdu.feifeiyinyue.top

[U96] JS：async/await 与异常
来源：http://uex.jyoumei.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bon.yanxiufei.cn

[U97] JS：并发请求
来源：http://fsp.xuanzx.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://bti.cqqwz.cn

[U98] JS：fetch 带 JSON
来源：http://ids.tarul.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xlz.fktsv.cn

[U99] JS：事件监听
来源：http://fsl.yueranfly.top

el.addEventListener("click", e => {})
来源：http://dpe.yj202588.top

[U100] JS：DOM 查询
来源：http://qng.dashuyun.cn

document.querySelector(".item")
来源：http://cqr.zhongyouzk.top

[U101] JS：classList 操作
来源：http://tcz.nanxinkj.top

el.classList.toggle("active")
来源：http://wus.fanxiaobao.xyz

[U102] JS：本地存储
来源：http://kac.hesvh.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://lux.hnqzz.top

[U103] JS：定时器
来源：http://kpw.zhaomingkeji.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jjz.mhx1999.top

[U104] JS：防抖
来源：http://nvx.yj20258888.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zgy.wangdashe.top

[U105] JS：节流
来源：http://bpw.meibo888.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://flm.shanyushiyangkeji.top

[U106] JS：日期格式化
来源：http://viy.xuanzx.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://irr.52xcode.cn

[U107] JS：数字千分位
来源：http://tkq.dashuyun.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://que.xziqi.cn

[U108] JS：随机整数
来源：http://jpb.cashguo.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kad.kuanghao11.cn

[U109] JS：数组分组
来源：http://nzv.shangyingyoupin.top

Object.groupBy(arr, x => x.type)
来源：http://avm.bbcook.cn

[U110] JS：数组分块
来源：http://bux.hfpthk.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zyt.cheryme.top

[U111] JS：对象转 Map
来源：http://jju.guowangkeji.top

new Map(Object.entries(obj))
来源：http://myw.zdqjudy.top

[U112] JS：字符串补位
来源：http://tex.jinqigufen.top

"7".padStart(3, "0")
来源：http://bab.jinqigfzy.top

[U113] JS：正则替换全部
来源：http://iij.tarul.cn

s.replaceAll("a", "b")
来源：http://jby.cheryme.top

[U114] JS：JSON 深比较
来源：http://xzg.epnwcf.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://adg.cucudq.cn

[U115] JS：生成 UUID
来源：http://abh.sweek.top

crypto.randomUUID()
来源：http://nbo.c1oappe.top

[U116] JS：类型检查（JSDoc）
来源：http://vsq.fengsongda.top

/** @param {string} name */ function f(name) {}
来源：http://ybr.nanxuanxn.top

[U117] JS：单元测试
来源：http://sel.zhijiandao.cn

npm i -D vitest;  npx vitest
来源：http://cfd.xingfuxueyuan.xyz

[U118] JS：开发服务器
来源：http://tun.jinyuanbaomall.cn

npm i -D vite;  npx vite
来源：http://oqe.jinqigfzy.top

[U119] JS：生产构建
来源：http://tze.aizwys.cn

npx vite build
来源：http://gpe.jqgufenzy.top

[U120] JS：读取环境变量（Vite）
来源：http://pnj.52xcode.cn

import.meta.env.VITE_API_URL
来源：http://mck.quarkkingdee.top

================================================================================
来源：http://xuu.jqgufenzy.top

统计汇总
来源：http://pwr.ydzc1.top

================================================================================
来源：http://sef.havefunace.top

按语言统计（条）：
来源：http://ycg.zhiwuduotai.top

Python ......... 252
来源：http://mpc.vehdjk.com

PHP ............ 252
来源：http://bbw.zdqjudy.top

JavaScript ..... 252
来源：http://orp.xylfe.cn

TypeScript ..... 212
来源：http://khc.meibo888.top

Java ........... 212
来源：http://obk.cashguo.top

Go ............. 212
来源：http://oup.jianghu66.top

Ruby ........... 212
来源：http://qpt.vehdjk.com

C# ............. 212
来源：http://qjw.zhiwuduotai.top

C .............. 30
来源：http://mxk.yonumen.top

C++ ............ 30
来源：http://biu.bbcook.cn

SQL ............ 90
来源：http://fog.tarul.cn

Bash ........... 80
来源：http://wxm.hnqzz.top

Kotlin ......... 15
来源：http://phx.316326.xyz

Swift .......... 15
来源：http://lcc.andypj.xyz

Lua ............ 10
来源：http://ews.cqqwz.cn

Perl ........... 10
来源：http://kmx.redwolf501.top

Scala .......... 10
来源：http://pel.quarkkingdee.top

------------------------------------
来源：http://ujy.zdbjq.cn

合计 ........... 2106 条
来源：http://fvj.tarul.cn

按章节统计：
来源：http://rmz.haohaochexian.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://eeq.sxryk.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://eta.zhengqikj.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://njt.chenjidiqi.icu

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mwy.c1oappe.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://npm.feifeiyinyue.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nxr.ydjk.org.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vfu.9152youxi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tod.wangshuangyany.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lvx.cdnleiting.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vdh.jinghuilouyu.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qao.zycfv.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fpo.wangshuangyany.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://cdc.tianlin.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jqi.gotoacloud.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://rpy.cqqwz.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://yqs.0kj1m.cn

Q SQL 专题                              90
来源：http://adh.sxryk.cn

R Bash 专题                             80
来源：http://mow.cucudq.cn

S C / C++ 专题                          60
来源：http://omq.gaohongyu789.top

T 其他语言补充                          60
来源：http://szr.tian-w.cn

U 高频实用片段                         120
来源：http://rhm.hnxiangtu.top

------------------------------------
来源：http://ocm.shanyushiyangtech.top

合计                                  2106 条
来源：http://tae.shanyushiyangtech.top

--------------------------------------------------------------------------------
来源：http://rtb.wangdashe.top

使用提醒
来源：http://dwe.yj20258888.top

--------------------------------------------------------------------------------
来源：http://kiq.ywan-chungtsiang.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://bzn.yanxiufei.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://drl.zhongyouzk.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qvt.hywenlv.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://shg.sxryk.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rok.ppjwa.cn

—— 文件结束 ——
来源：http://phn.yvedp.cn

================================================================================
来源：http://uay.gzhubu.top

程序语言常见例子速查手册（2024 版）
来源：http://les.xinyue.icu

Common Programming Examples Cheat Book
来源：http://sdb.zhijiandao.cn

================================================================================
来源：http://pix.aibaodan.cn

【收录内容】
来源：http://mfo.chenjidiqi.icu

覆盖 12 种语言 / 语法与常见 API：
来源：http://esc.feifeiyinyue.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hva.zhengqikj.top

SQL · Bash · C · C++
来源：http://wrx.jinghuilouyu.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ako.chenlongwang.top

【使用说明】
来源：http://wcu.yonumen.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://luy.yvedp.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://igj.shuidangran.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ccj.epnwcf.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://jyj.ivvv.top

Bash:  Shell         C:     C             C++:   C++
来源：http://hpl.yj20258.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://qpq.epnwcf.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://haa.ctjpmb.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vmv.shzxlz.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xno.zdqjudy.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://lup.shanyushiyangkeji.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://eos.chenjidiqi.icu

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://uzp.ctjpmb.com

【文件统计】
来源：http://mtp.yj20258888.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zkq.hywenlv.cn

--------------------------------------------------------------------------------
来源：http://mmt.kuanghao11.cn

目  录
来源：http://rcp.haohaochexian.top

--------------------------------------------------------------------------------
来源：http://pxc.yj20258.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://gvo.chenzaomai.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mml.daxiang520.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://nhq.shangyingyoupin.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zbq.aibaodan.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://oqf.yongpay.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ulj.cucudq.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://dgc.52xcode.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://rri.bjfxy.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tzi.tianlin.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wax.shanyushiyangkeji.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://jwu.ydjk.org.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://rbv.hammf.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://pzq.zycfv.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ugv.shanyushiyangtech.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://cuz.hnxiangtu.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ect.dianchejie.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://gxv.xuanzx.com


<!-- 参考信息 -->