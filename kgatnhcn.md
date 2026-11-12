代发 wailian999

[U23] Py：分块读取大文件
来源：http://ixa.zhixingplan.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://yxd.nanxuanxn.top

[U24] Py：路径操作
来源：http://ugy.smart0.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://auq.pengpengdd.cyou

[U25] Py：CSV 按字典读
来源：http://hnb.cucudq.cn

csv.DictReader(f)
来源：http://rwy.zhoulong.xyz

[U26] Py：并发下载
来源：http://lwf.hcnkem.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://naw.meibo888.top

[U27] Py：异步 HTTP
来源：http://kql.xingfuxueyuan.xyz

aiohttp.ClientSession() 配合 async with
来源：http://fld.hesvh.cn

[U28] Py：类型别名
来源：http://obx.hcnkem.com

UserId = int
来源：http://xlp.fehbvm.com

[U29] Py：属性校验
来源：http://xyc.nanxuanxn.top

@property 与 @x.setter 配合
来源：http://nwj.fehbvm.com

[U30] Py：数据类
来源：http://wzr.yj20258888.top

@dataclass(slots=True)
来源：http://ngy.sxryk.cn

[U31] Py：单测
来源：http://vsy.smart0.xyz

python -m pytest -q
来源：http://bao.gogol.net.cn

[U32] Py：代码格式化
来源：http://wom.yj20258.top

ruff format . && ruff check --fix .
来源：http://qku.tianlin.xyz

[U33] Py：打包发布
来源：http://ovv.cashguo.top

python -m build  （依赖 pyproject.toml）
来源：http://yzn.ivvv.top

[U34] Py：判断编码
来源：http://kum.fengsongda.top

chardet.detect(raw)
来源：http://epq.iojbl.cn

[U35] Py：发送邮件
来源：http://uby.hywenlv.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jqo.hywenlv.cn

[U36] Py：定时任务
来源：http://snl.zhoulong.xyz

schedule.every(10).minutes.do(job)
来源：http://rsh.zhaomingkeji.xyz

[U37] Py：读写 Excel
来源：http://lof.tarul.cn

pandas.read_excel / DataFrame.to_excel
来源：http://suu.nwbrower.top

[U38] Py：获取脚本所在目录
来源：http://jms.birdmap.top

Path(__file__).resolve().parent
来源：http://dtm.sxryk.cn

[U39] Py：判断是否在交互环境
来源：http://hgq.hywenlv.cn

sys.stdout.isatty()
来源：http://irb.nanxuanxn.top

[U40] Py：打印到标准错误
来源：http://yek.dashuyun.cn

print("err", file=sys.stderr)
来源：http://jgc.tian-w.cn

[U41] PHP：初始化 Composer 项目
来源：http://zpx.havefunace.top

composer init;  composer require guzzlehttp/guzzle
来源：http://xkn.cucudq.cn

[U42] PHP：PSR-4 自动加载
来源：http://pyx.yuanzhike.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nxv.iojbl.cn

[U43] PHP：声明命名空间
来源：http://qdq.iojbl.cn

namespace App\Http;
来源：http://tie.xziqi.cn

[U44] PHP：开启严格类型
来源：http://thp.cheryme.top

declare(strict_types=1);
来源：http://kso.ppjwa.cn

[U45] PHP：类型声明与返回类型
来源：http://uap.sweek.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://fmd.gzhubu.top

[U46] PHP：可空类型
来源：http://vsj.fktsv.cn

?string $name = null
来源：http://nni.pengpengdd.cyou

[U47] PHP：联合类型
来源：http://hra.nanxinkj.top

int|string $id
来源：http://tzh.zhijiandao.cn

[U48] PHP：纯枚举
来源：http://qbi.ctjpmb.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jii.pycfn.com

[U49] PHP：只读属性
来源：http://jak.hfpthk.cn

public readonly string $name
来源：http://drk.xylfe.cn

[U50] PHP：构造器属性提升
来源：http://uvj.zhixingplan.top

public function __construct(private int $id) {}
来源：http://nlg.hnqzz.top

[U51] PHP：数组解构
来源：http://lss.uphjek.com

[$a, $b] = $arr;
来源：http://yqd.daria6918.cn

[U52] PHP：箭头函数
来源：http://svs.vqdsnc.cn

$double = fn($x) => $x * 2;
来源：http://fqr.epnwcf.com

[U53] PHP：空合并运算符
来源：http://oxa.yvedp.cn

$v = $a ?? $b ?? "default";
来源：http://tpb.fengsongda.top

[U54] PHP：空安全调用
来源：http://vax.yuxming.cn

$obj?->method()
来源：http://djp.feifeiyinyue.top

[U55] PHP：match 表达式
来源：http://ksa.gotoacloud.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://nac.jinghuilouyu.cn

[U56] PHP：命名参数
来源：http://jvl.jyoumei.cn

f(a: 1, b: 2)
来源：http://utm.shangyingyoupin.top

[U57] PHP：字符串插值
来源：http://uhh.uphjek.com

"值: {$a}"
来源：http://kdz.cqqwz.cn

[U58] PHP：数组三件套
来源：http://olz.sxryk.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://syf.jinqigfzy.top

[U59] PHP：自定义排序
来源：http://hyl.zdqjudy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://shz.kuanghao11.cn

[U60] PHP：JSON 编解码
来源：http://xwh.jyoumei.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xqi.tarul.cn

[U61] PHP：正则
来源：http://ogu.gogol.net.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qqp.cashguo.top

[U62] PHP：日期对象
来源：http://syp.yj20258.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jgz.havefunace.top

[U63] PHP：文件读写
来源：http://lwv.xziqi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mur.yangfankeji.com

[U64] PHP：目录遍历
来源：http://upo.redwolf501.top

glob("dir/*.php");  scandir("dir");
来源：http://qdu.yongpay.top

[U65] PHP：会话
来源：http://bcx.yuanzhike.top

session_start();  $_SESSION["uid"] = 1;
来源：http://jyy.iojbl.cn

[U66] PHP：设置 Cookie
来源：http://sap.ivvv.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://uol.tarul.cn

[U67] PHP：处理文件上传
来源：http://yri.havefunace.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wst.ywan-chungtsiang.top

[U68] PHP：PDO 连接
来源：http://xin.yvedp.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://oma.ivvv.top

[U69] PHP：PDO 预处理
来源：http://jyi.bbcook.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://epx.hnqzz.top

[U70] PHP：PDO 事务
来源：http://vrt.52xcode.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lns.zycfv.cn

[U71] PHP：抛出异常
来源：http://xtm.zhijiandao.cn

throw new RuntimeException("失败", 500);
来源：http://pbl.haohaochexian.top

[U72] PHP：写错误日志
来源：http://qmk.gaohongyu789.top

error_log("失败: " . $e->getMessage());
来源：http://nvt.chenzaomai.com

[U73] PHP：读取 ini 配置
来源：http://ien.xinyue.icu

parse_ini_file("config.ini", true)
来源：http://emj.jlsjyb.cn

[U74] PHP：读取环境变量
来源：http://oys.jlsjyb.cn

getenv("APP_ENV") ?: "production"
来源：http://tsm.yanxiufei.cn

[U75] PHP：依赖注入
来源：http://vnx.andypj.xyz

composer require psr/container
来源：http://edi.hywenlv.cn

[U76] PHP：简单路由
来源：http://vlf.jinghuilouyu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jtl.jinqigufen.top

[U77] PHP：模板渲染
来源：http://uyl.dianchejie.cn

composer require twig/twig
来源：http://spu.yj202588.top

[U78] PHP：单元测试
来源：http://zvs.yanxiufei.cn

composer require --dev phpunit/phpunit
来源：http://dcj.redwolf501.top

[U79] PHP：静态分析
来源：http://agp.tarul.cn

composer require --dev phpstan/phpstan
来源：http://vfn.yueranfly.top

[U80] PHP：代码规范修复
来源：http://zrt.xuetiantiany.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://gke.jqgfzy.top

[U81] JS：初始化项目
来源：http://bvr.gaohongyu789.top

npm init -y;  npm i express
来源：http://krw.feifeiyinyue.top

[U82] JS：package.json 脚本
来源：http://mot.ydjk.org.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bst.yongpay.top

[U83] JS：ES Module 导入导出
来源：http://qdw.hywenlv.cn

export const a = 1;  import { a } from "./m.js";
来源：http://pmk.9152youxi.cn

[U84] JS：CommonJS 写法
来源：http://enx.yj202588.top

module.exports = { a };  const { a } = require("./m");
来源：http://vah.daxiang520.top

[U85] JS：可选链
来源：http://mob.zhixingplan.top

a?.b?.c
来源：http://woq.havefunace.top

[U86] JS：空值合并
来源：http://oiz.birdmap.top

a ?? b
来源：http://dbh.jinqigfzy.top

[U87] JS：解构默认值
来源：http://sqw.shangyingyoupin.top

const { a = 1, b = 2 } = obj;
来源：http://zoh.xingfuxueyuan.xyz

[U88] JS：对象展开合并
来源：http://cii.hesvh.cn

{ ...a, ...b }
来源：http://kzw.hysaishi.cn

[U89] JS：数组去重
来源：http://cuq.jiagoushi.top

[...new Set(arr)]
来源：http://sad.daria6918.cn

[U90] JS：数字数组排序
来源：http://own.sjlbkw.cn

[...arr].sort((a, b) => a - b)
来源：http://jnl.316326.xyz

[U91] JS：对象键值遍历
来源：http://cim.xingfuxueyuan.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dbp.hcnkem.com

[U92] JS：深拷贝
来源：http://jmz.yfazqb.com

structuredClone(obj)
来源：http://akl.chenlongwang.top

[U93] JS：模板字符串
来源：http://jna.yj20258.top

`共 ${n} 条`
来源：http://tcw.uphjek.com

[U94] JS：箭头函数
来源：http://zru.yj20258888.top

const double = x => x * 2;
来源：http://ocy.gogol.net.cn

[U95] JS：Promise 包装
来源：http://mhl.jinyuanbaomall.cn

new Promise((resolve, reject) => {})
来源：http://viq.tianlin.xyz

[U96] JS：async/await 与异常
来源：http://yej.shanyushiyangkeji.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://afx.chenjidiqi.icu

[U97] JS：并发请求
来源：http://sdp.shanyushiyangkeji.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://dho.gzhubu.top

[U98] JS：fetch 带 JSON
来源：http://xwm.ppjwa.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://aqr.zhijiandao.cn

[U99] JS：事件监听
来源：http://coz.havefunace.top

el.addEventListener("click", e => {})
来源：http://nqg.cashguo.top

[U100] JS：DOM 查询
来源：http://vit.jqgfzy.top

document.querySelector(".item")
来源：http://tfk.xuanzx.com

[U101] JS：classList 操作
来源：http://zrf.zhengqikj.top

el.classList.toggle("active")
来源：http://wjh.shanyushiyangkeji.top

[U102] JS：本地存储
来源：http://egh.yonumen.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ggr.feifeiyinyue.top

[U103] JS：定时器
来源：http://lwj.kuanghao11.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qvv.vehdjk.com

[U104] JS：防抖
来源：http://oht.nanxinkj.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uxg.ctjpmb.com

[U105] JS：节流
来源：http://rdu.hcnkem.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yhb.shanyushiyangtech.top

[U106] JS：日期格式化
来源：http://dtn.zycfv.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://eoe.haohaochexian.top

[U107] JS：数字千分位
来源：http://nqq.tianlin.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rkr.gogol.net.cn

[U108] JS：随机整数
来源：http://yfn.kuanghao11.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://muj.gzhubu.top

[U109] JS：数组分组
来源：http://uvz.aizwys.cn

Object.groupBy(arr, x => x.type)
来源：http://fkq.hnxiangtu.top

[U110] JS：数组分块
来源：http://jyh.fzhhl.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://azl.jiagoushi.top

[U111] JS：对象转 Map
来源：http://bda.hnxiangtu.top

new Map(Object.entries(obj))
来源：http://res.jlsjyb.cn

[U112] JS：字符串补位
来源：http://lmq.c1oappe.top

"7".padStart(3, "0")
来源：http://otl.snrcjt.cn

[U113] JS：正则替换全部
来源：http://mno.xziqi.cn

s.replaceAll("a", "b")
来源：http://yuf.iojbl.cn

[U114] JS：JSON 深比较
来源：http://xdz.nanxinkj.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://plz.hnxiangtu.top

[U115] JS：生成 UUID
来源：http://ylm.hongshengwenyu.top

crypto.randomUUID()
来源：http://hph.andypj.xyz

[U116] JS：类型检查（JSDoc）
来源：http://prc.quarkkingdee.top

/** @param {string} name */ function f(name) {}
来源：http://ucx.daxiang520.top

[U117] JS：单元测试
来源：http://yya.xuetiantiany.cn

npm i -D vitest;  npx vitest
来源：http://uhx.sweek.top

[U118] JS：开发服务器
来源：http://tzr.zhoulong.xyz

npm i -D vite;  npx vite
来源：http://onw.bbcook.cn

[U119] JS：生产构建
来源：http://yro.ppjwa.cn

npx vite build
来源：http://wat.zdqjudy.top

[U120] JS：读取环境变量（Vite）
来源：http://yfa.jinqigfzy.top

import.meta.env.VITE_API_URL
来源：http://grd.yuanzhike.top

================================================================================
来源：http://buu.hammf.cn

统计汇总
来源：http://ehs.yj20258888.top

================================================================================
来源：http://sly.fehbvm.com

按语言统计（条）：
来源：http://krv.hnxiangtu.top

Python ......... 252
来源：http://kfj.yanxiufei.cn

PHP ............ 252
来源：http://kjj.hcnkem.com

JavaScript ..... 252
来源：http://nli.feifeiyinyue.top

TypeScript ..... 212
来源：http://zpe.tanke756.top

Java ........... 212
来源：http://lly.c1oappe.top

Go ............. 212
来源：http://hlx.yj20258.top

Ruby ........... 212
来源：http://jkg.jinghuilouyu.cn

C# ............. 212
来源：http://rxh.jqgufenzy.top

C .............. 30
来源：http://fbm.fzhhl.top

C++ ............ 30
来源：http://pmu.fanxiaobao.xyz

SQL ............ 90
来源：http://ryq.hfpthk.cn

Bash ........... 80
来源：http://mku.cucudq.cn

Kotlin ......... 15
来源：http://yxa.cashguo.top

Swift .......... 15
来源：http://ltm.fktsv.cn

Lua ............ 10
来源：http://bfi.bjfxy.top

Perl ........... 10
来源：http://roj.fanxiaobao.xyz

Scala .......... 10
来源：http://fuo.yj20258.top

------------------------------------
来源：http://siz.gzhubu.top

合计 ........... 2106 条
来源：http://qdh.fengsongda.top

按章节统计：
来源：http://tin.cucudq.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gsi.ywan-chungtsiang.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ziw.hysaishi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ccr.tanke756.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://yhi.aizwys.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ebp.ehwqpu.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://tbt.52xcode.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hdf.daxiang520.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://few.jyoumei.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ojx.hnxiangtu.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vhb.gzhubu.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kqt.jyoumei.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://abc.316326.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://fte.zycfv.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qko.fzhhl.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qow.gaohongyu789.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xxd.hongshengwenyu.top

Q SQL 专题                              90
来源：http://asp.52xcode.cn

R Bash 专题                             80
来源：http://jwt.ctjpmb.com

S C / C++ 专题                          60
来源：http://eyn.vehdjk.com

T 其他语言补充                          60
来源：http://ahi.0kj1m.cn

U 高频实用片段                         120
来源：http://hqz.fanxiaobao.xyz

------------------------------------
来源：http://win.jinqigfzy.top

合计                                  2106 条
来源：http://pus.cheryme.top

--------------------------------------------------------------------------------
来源：http://qme.birdmap.top

使用提醒
来源：http://dxk.shanyushiyangtech.top

--------------------------------------------------------------------------------
来源：http://air.bjfxy.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://llo.feifeiyinyue.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://rjq.jyoumei.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wvk.xingfuxueyuan.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://tud.ywan-chungtsiang.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ilu.shangyingyoupin.top

—— 文件结束 ——
来源：http://nwv.nanxinkj.top

================================================================================
来源：http://cgd.fengsongda.top

程序语言常见例子速查手册（2024 版）
来源：http://rod.ywan-chungtsiang.top

Common Programming Examples Cheat Book
来源：http://cqc.yueranfly.top

================================================================================
来源：http://gvd.sxryk.cn

【收录内容】
来源：http://xqb.pengpengdd.cyou

覆盖 12 种语言 / 语法与常见 API：
来源：http://eab.redwolf501.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://klv.tanke756.top

SQL · Bash · C · C++
来源：http://dtf.zhixingplan.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://chc.yj20258888.top

【使用说明】
来源：http://opw.hnxiangtu.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vio.jqgufenzy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xqd.xuanzx.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://err.cucudq.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://rkv.jianghu66.top

Bash:  Shell         C:     C             C++:   C++
来源：http://uca.hfpthk.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mmt.tarul.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ztg.guowangkeji.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://oja.fehbvm.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wpi.quarkkingdee.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ovw.hammf.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://shi.bbcook.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://cdd.redwolf501.top

【文件统计】
来源：http://oej.zhaomingkeji.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wll.jyoumei.cn

--------------------------------------------------------------------------------
来源：http://ksp.sysykeji.top

目  录
来源：http://ylr.xziqi.cn

--------------------------------------------------------------------------------
来源：http://fpx.hcnkem.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://lcj.zhijiandao.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ygh.shanyushiyangtech.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jnq.tarul.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://voz.shangyingyoupin.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mqe.316326.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://unm.cheryme.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mny.ydzc1.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://tkk.xingfuxueyuan.xyz

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://fzg.ppjwa.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://beh.svipenyu.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ram.epnwcf.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://kxx.zycfv.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://dwd.jinqigufen.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://iya.0kj1m.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://dmr.hfpthk.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mqs.gzhubu.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://sej.xylfe.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://jgd.zdqjudy.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://tbk.jqgufenzy.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wsc.zhoulong.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://bso.52xcode.cn


<!-- 参考信息 -->