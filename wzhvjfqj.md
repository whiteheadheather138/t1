代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://dzd.shanyushiyangtech.top

@contextlib.contextmanager
来源：http://cox.jiagoushi.top

[U22] Py：矩阵转置
来源：http://ojt.ydzc1.top

list(zip(*m))
来源：http://mxk.jiagoushi.top

[U23] Py：分块读取大文件
来源：http://zgt.birdmap.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bbt.c1oappe.top

[U24] Py：路径操作
来源：http://uka.ehwqpu.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://agn.bbcook.cn

[U25] Py：CSV 按字典读
来源：http://doz.uphjek.com

csv.DictReader(f)
来源：http://qeo.yj202588.top

[U26] Py：并发下载
来源：http://hgw.pengpengdd.cyou

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hfw.aibaodan.cn

[U27] Py：异步 HTTP
来源：http://qan.smart0.xyz

aiohttp.ClientSession() 配合 async with
来源：http://hvd.gaohongyu789.top

[U28] Py：类型别名
来源：http://zlf.jinyuanbaomall.cn

UserId = int
来源：http://uqq.ydjk.org.cn

[U29] Py：属性校验
来源：http://xwi.sysykeji.top

@property 与 @x.setter 配合
来源：http://dzm.zhaomingkeji.xyz

[U30] Py：数据类
来源：http://zuw.shuidangran.top

@dataclass(slots=True)
来源：http://gzt.guannengcc.top

[U31] Py：单测
来源：http://vjo.dashuyun.cn

python -m pytest -q
来源：http://ihu.shzxlz.cn

[U32] Py：代码格式化
来源：http://zhs.vqdsnc.cn

ruff format . && ruff check --fix .
来源：http://wzw.fehbvm.com

[U33] Py：打包发布
来源：http://bts.snrcjt.cn

python -m build  （依赖 pyproject.toml）
来源：http://voh.aibaodan.cn

[U34] Py：判断编码
来源：http://wmw.guannengcc.top

chardet.detect(raw)
来源：http://dow.yuxming.cn

[U35] Py：发送邮件
来源：http://wtx.wangdashe.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xhs.fengsongda.top

[U36] Py：定时任务
来源：http://fgx.zhijiandao.cn

schedule.every(10).minutes.do(job)
来源：http://czy.gaohongyu789.top

[U37] Py：读写 Excel
来源：http://ibu.hnqzz.top

pandas.read_excel / DataFrame.to_excel
来源：http://luk.gotoacloud.top

[U38] Py：获取脚本所在目录
来源：http://uxg.hnqzz.top

Path(__file__).resolve().parent
来源：http://crf.ehwqpu.com

[U39] Py：判断是否在交互环境
来源：http://jdu.fzhhl.top

sys.stdout.isatty()
来源：http://ibu.316326.xyz

[U40] Py：打印到标准错误
来源：http://myu.cheryme.top

print("err", file=sys.stderr)
来源：http://pvt.cheryme.top

[U41] PHP：初始化 Composer 项目
来源：http://hzp.52xcode.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://gvd.hcnkem.com

[U42] PHP：PSR-4 自动加载
来源：http://qbl.jinqigfzy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ujf.zhaomingkeji.xyz

[U43] PHP：声明命名空间
来源：http://mdo.xylfe.cn

namespace App\Http;
来源：http://kfi.52xcode.cn

[U44] PHP：开启严格类型
来源：http://mur.fktsv.cn

declare(strict_types=1);
来源：http://svz.zhixingplan.top

[U45] PHP：类型声明与返回类型
来源：http://igl.nanxuanxn.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://yov.aizwys.cn

[U46] PHP：可空类型
来源：http://rhz.xuetiantiany.cn

?string $name = null
来源：http://nan.c1oappe.top

[U47] PHP：联合类型
来源：http://gsn.ydzc1.top

int|string $id
来源：http://bai.tian-w.cn

[U48] PHP：纯枚举
来源：http://xir.0kj1m.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://sck.ywan-chungtsiang.top

[U49] PHP：只读属性
来源：http://dog.vehdjk.com

public readonly string $name
来源：http://vmu.xuetiantiany.cn

[U50] PHP：构造器属性提升
来源：http://xww.andypj.xyz

public function __construct(private int $id) {}
来源：http://bag.zhoulong.xyz

[U51] PHP：数组解构
来源：http://krf.epnwcf.com

[$a, $b] = $arr;
来源：http://nfg.yanxiufei.cn

[U52] PHP：箭头函数
来源：http://oia.iojbl.cn

$double = fn($x) => $x * 2;
来源：http://tvd.shzxlz.cn

[U53] PHP：空合并运算符
来源：http://bme.jqgfzy.top

$v = $a ?? $b ?? "default";
来源：http://cso.jqgufenzy.top

[U54] PHP：空安全调用
来源：http://uxm.shanyushiyangkeji.top

$obj?->method()
来源：http://aqr.xylfe.cn

[U55] PHP：match 表达式
来源：http://jlc.chenlongwang.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zfd.wangshuangyany.cn

[U56] PHP：命名参数
来源：http://ava.zhixingplan.top

f(a: 1, b: 2)
来源：http://fyh.iojbl.cn

[U57] PHP：字符串插值
来源：http://eqp.shangyingyoupin.top

"值: {$a}"
来源：http://kco.hfpthk.cn

[U58] PHP：数组三件套
来源：http://qev.52xcode.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kkc.yongpay.top

[U59] PHP：自定义排序
来源：http://htz.zhijiandao.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nry.chenjidiqi.icu

[U60] PHP：JSON 编解码
来源：http://pwx.vehdjk.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jjh.sufxvd.cn

[U61] PHP：正则
来源：http://gkt.xuetiantiany.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://roh.pengpengdd.cyou

[U62] PHP：日期对象
来源：http://pca.jinghuilouyu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vme.zycfv.cn

[U63] PHP：文件读写
来源：http://clh.ppjwa.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hbf.chenlongwang.top

[U64] PHP：目录遍历
来源：http://kwh.nanxuanxn.top

glob("dir/*.php");  scandir("dir");
来源：http://tuq.zycfv.cn

[U65] PHP：会话
来源：http://ege.yj20258.top

session_start();  $_SESSION["uid"] = 1;
来源：http://sef.jinghuilouyu.cn

[U66] PHP：设置 Cookie
来源：http://eqr.jlsjyb.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hoe.yj20258.top

[U67] PHP：处理文件上传
来源：http://lis.meibo888.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://cbd.ehwqpu.com

[U68] PHP：PDO 连接
来源：http://wuc.jiagoushi.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://tvt.zhongyouzk.top

[U69] PHP：PDO 预处理
来源：http://rht.cdnleiting.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nvb.gaohongyu789.top

[U70] PHP：PDO 事务
来源：http://jdh.jinqigufen.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://cnk.yongpay.top

[U71] PHP：抛出异常
来源：http://ens.zhoulong.xyz

throw new RuntimeException("失败", 500);
来源：http://uoi.zhongyouzk.top

[U72] PHP：写错误日志
来源：http://wmz.cucudq.cn

error_log("失败: " . $e->getMessage());
来源：http://wfq.yfazqb.com

[U73] PHP：读取 ini 配置
来源：http://iln.ehwqpu.com

parse_ini_file("config.ini", true)
来源：http://wix.yonumen.top

[U74] PHP：读取环境变量
来源：http://vme.guowangkeji.top

getenv("APP_ENV") ?: "production"
来源：http://rhr.shanyushiyangkeji.top

[U75] PHP：依赖注入
来源：http://tco.smart0.xyz

composer require psr/container
来源：http://myn.jinyuanbaomall.cn

[U76] PHP：简单路由
来源：http://fkh.snrcjt.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://sqm.quarkkingdee.top

[U77] PHP：模板渲染
来源：http://spr.zhiwuduotai.top

composer require twig/twig
来源：http://isp.uphjek.com

[U78] PHP：单元测试
来源：http://mnr.bbcook.cn

composer require --dev phpunit/phpunit
来源：http://srk.yfazqb.com

[U79] PHP：静态分析
来源：http://ubb.zhijiandao.cn

composer require --dev phpstan/phpstan
来源：http://ysc.gogol.net.cn

[U80] PHP：代码规范修复
来源：http://sql.jqgfzy.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://pec.feifeiyinyue.top

[U81] JS：初始化项目
来源：http://nvv.jinghuilouyu.cn

npm init -y;  npm i express
来源：http://cuw.yfazqb.com

[U82] JS：package.json 脚本
来源：http://nfo.sysykeji.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nif.ybcxt.top

[U83] JS：ES Module 导入导出
来源：http://kdg.hysaishi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ong.yanxiufei.cn

[U84] JS：CommonJS 写法
来源：http://dlo.hysaishi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://xby.hongshengwenyu.top

[U85] JS：可选链
来源：http://zcw.haohaochexian.top

a?.b?.c
来源：http://wcd.zhengqikj.top

[U86] JS：空值合并
来源：http://sxw.bjfxy.top

a ?? b
来源：http://egt.tanke756.top

[U87] JS：解构默认值
来源：http://otz.jiagoushi.top

const { a = 1, b = 2 } = obj;
来源：http://eeb.jqgfzy.top

[U88] JS：对象展开合并
来源：http://pna.gotoacloud.top

{ ...a, ...b }
来源：http://enc.cdnleiting.top

[U89] JS：数组去重
来源：http://zil.ivvv.top

[...new Set(arr)]
来源：http://plp.yonumen.top

[U90] JS：数字数组排序
来源：http://pqi.yvedp.cn

[...arr].sort((a, b) => a - b)
来源：http://sxy.guannengcc.top

[U91] JS：对象键值遍历
来源：http://yul.hysaishi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bzz.ydzc1.top

[U92] JS：深拷贝
来源：http://oqw.kuanghao11.cn

structuredClone(obj)
来源：http://lzm.52xcode.cn

[U93] JS：模板字符串
来源：http://fih.gzhubu.top

`共 ${n} 条`
来源：http://iky.vehdjk.com

[U94] JS：箭头函数
来源：http://waz.zhixingplan.top

const double = x => x * 2;
来源：http://ekg.xuanzx.com

[U95] JS：Promise 包装
来源：http://llx.hcnkem.com

new Promise((resolve, reject) => {})
来源：http://ybx.yonumen.top

[U96] JS：async/await 与异常
来源：http://rlf.kuanghao11.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ifi.yuxming.cn

[U97] JS：并发请求
来源：http://yoc.shuidangran.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://frz.mhx1999.top

[U98] JS：fetch 带 JSON
来源：http://fyp.xziqi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mzv.zhixingplan.top

[U99] JS：事件监听
来源：http://gid.epnwcf.com

el.addEventListener("click", e => {})
来源：http://wdu.zhiwuduotai.top

[U100] JS：DOM 查询
来源：http://ywb.shuidangran.top

document.querySelector(".item")
来源：http://uwa.zhixingplan.top

[U101] JS：classList 操作
来源：http://glg.zhixingplan.top

el.classList.toggle("active")
来源：http://yok.hysaishi.cn

[U102] JS：本地存储
来源：http://btz.chenzaomai.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://vjq.wangdashe.top

[U103] JS：定时器
来源：http://xii.svipenyu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://roq.hongshengwenyu.top

[U104] JS：防抖
来源：http://igd.zhaomingkeji.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ahh.cucudq.cn

[U105] JS：节流
来源：http://qtg.cheryme.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ptl.shanyushiyangkeji.top

[U106] JS：日期格式化
来源：http://tyh.zhijiandao.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wpv.tarul.cn

[U107] JS：数字千分位
来源：http://wlo.zhengqikj.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yli.zdbjq.cn

[U108] JS：随机整数
来源：http://rrb.cucudq.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vfk.jiagoushi.top

[U109] JS：数组分组
来源：http://qge.316326.xyz

Object.groupBy(arr, x => x.type)
来源：http://hrg.hnxiangtu.top

[U110] JS：数组分块
来源：http://hop.fehbvm.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gpo.hcnkem.com

[U111] JS：对象转 Map
来源：http://bst.tarul.cn

new Map(Object.entries(obj))
来源：http://fnk.sysykeji.top

[U112] JS：字符串补位
来源：http://nqw.aibaodan.cn

"7".padStart(3, "0")
来源：http://wyk.nanxuanxn.top

[U113] JS：正则替换全部
来源：http://ast.yfazqb.com

s.replaceAll("a", "b")
来源：http://skr.yuanzhike.top

[U114] JS：JSON 深比较
来源：http://rlg.wangdashe.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://sdv.xuanzx.com

[U115] JS：生成 UUID
来源：http://fjs.ybcxt.top

crypto.randomUUID()
来源：http://mgf.feifeiyinyue.top

[U116] JS：类型检查（JSDoc）
来源：http://vah.guowangkeji.top

/** @param {string} name */ function f(name) {}
来源：http://lvr.c1oappe.top

[U117] JS：单元测试
来源：http://rsl.xziqi.cn

npm i -D vitest;  npx vitest
来源：http://ybi.feifeiyinyue.top

[U118] JS：开发服务器
来源：http://ycp.tanke756.top

npm i -D vite;  npx vite
来源：http://odl.nwbrower.top

[U119] JS：生产构建
来源：http://yzs.nanxuanxn.top

npx vite build
来源：http://kbj.yuxming.cn

[U120] JS：读取环境变量（Vite）
来源：http://ctr.dianchejie.cn

import.meta.env.VITE_API_URL
来源：http://poc.jqgfzy.top

================================================================================
来源：http://wsu.xuetiantiany.cn

统计汇总
来源：http://bix.cashguo.top

================================================================================
来源：http://sty.hnxiangtu.top

按语言统计（条）：
来源：http://pnv.kuanghao11.cn

Python ......... 252
来源：http://wcz.9152youxi.cn

PHP ............ 252
来源：http://gmj.zhiwuduotai.top

JavaScript ..... 252
来源：http://lcy.ydzc1.top

TypeScript ..... 212
来源：http://sqt.xuanzx.com

Java ........... 212
来源：http://avz.aibaodan.cn

Go ............. 212
来源：http://dtf.ppjwa.cn

Ruby ........... 212
来源：http://pio.gotoacloud.top

C# ............. 212
来源：http://sjg.yanxiufei.cn

C .............. 30
来源：http://cdp.tian-w.cn

C++ ............ 30
来源：http://gml.zdqjudy.top

SQL ............ 90
来源：http://nzx.wangdashe.top

Bash ........... 80
来源：http://rtm.jianghu66.top

Kotlin ......... 15
来源：http://mar.0kj1m.cn

Swift .......... 15
来源：http://wnq.sxryk.cn

Lua ............ 10
来源：http://ihj.xylfe.cn

Perl ........... 10
来源：http://peu.gotoacloud.top

Scala .......... 10
来源：http://lfl.yj20258888.top

------------------------------------
来源：http://vca.jinqigufen.top

合计 ........... 2106 条
来源：http://yao.shuidangran.top

按章节统计：
来源：http://kej.nwbrower.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xhe.birdmap.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://iaa.smart0.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://liq.gzhubu.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://bve.hesvh.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hkk.chenjidiqi.icu

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://teq.chenzaomai.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://maj.fengsongda.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ggx.jinqigufen.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ald.nanxinkj.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rri.hysaishi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://src.jqgfzy.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dmp.guowangkeji.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://exa.zhixingplan.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://exr.shzxlz.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://lkg.c1oappe.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://fga.vehdjk.com

Q SQL 专题                              90
来源：http://hpr.dianchejie.cn

R Bash 专题                             80
来源：http://udc.vqdsnc.cn

S C / C++ 专题                          60
来源：http://gdl.jianghu66.top

T 其他语言补充                          60
来源：http://ckv.jinqigufen.top

U 高频实用片段                         120
来源：http://hjk.quarkkingdee.top

------------------------------------
来源：http://njr.shanyushiyangkeji.top

合计                                  2106 条
来源：http://hbm.epnwcf.com

--------------------------------------------------------------------------------
来源：http://ile.jinyuanbaomall.cn

使用提醒
来源：http://qcu.iojbl.cn

--------------------------------------------------------------------------------
来源：http://apq.fehbvm.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jie.sxryk.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://evz.fktsv.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qti.jyoumei.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://xpd.jinghuilouyu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://lcr.cheryme.top

—— 文件结束 ——
来源：http://uno.zhongyouzk.top

================================================================================
来源：http://fki.sjlbkw.cn

程序语言常见例子速查手册（2024 版）
来源：http://ruu.sufxvd.cn

Common Programming Examples Cheat Book
来源：http://huk.zhongyouzk.top

================================================================================
来源：http://tev.hesvh.cn

【收录内容】
来源：http://vtz.jianghu66.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://qzk.fehbvm.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hwx.yuanzhike.top

SQL · Bash · C · C++
来源：http://ryt.zhongyouzk.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://vuw.gogol.net.cn

【使用说明】
来源：http://osn.jqgufenzy.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://iuk.yuanzhike.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://lpt.quarkkingdee.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ebn.vqdsnc.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://tum.xuetiantiany.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://idb.shanyushiyangkeji.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://rbf.redwolf501.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ybi.ctjpmb.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ads.yj20258888.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://cmf.quarkkingdee.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://vrb.fanxiaobao.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://zyi.52xcode.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://nyy.chenjidiqi.icu

【文件统计】
来源：http://jjk.dashuyun.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hni.smart0.xyz

--------------------------------------------------------------------------------
来源：http://ckd.hcnkem.com

目  录
来源：http://azf.jinghuilouyu.cn

--------------------------------------------------------------------------------
来源：http://vae.gotoacloud.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://lzm.52xcode.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://era.yuxming.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://nps.hnqzz.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://pnt.jinqigfzy.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://lfc.tarul.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://sik.chenzaomai.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ugv.redwolf501.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wns.xziqi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ajt.hcnkem.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xio.tarul.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ups.cucudq.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://tsi.zhiwuduotai.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mqx.52xcode.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://auw.pengpengdd.cyou

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lvy.meibo888.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://jpf.xylfe.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://izx.aizwys.cn


<!-- 参考信息 -->