代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://bwj.zhoulong.xyz

@contextlib.contextmanager
来源：http://hka.uphjek.com

[U22] Py：矩阵转置
来源：http://gdq.hywenlv.cn

list(zip(*m))
来源：http://ehu.wangdashe.top

[U23] Py：分块读取大文件
来源：http://bkd.haohaochexian.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rit.shanyushiyangtech.top

[U24] Py：路径操作
来源：http://uqp.gogol.net.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tsf.sweek.top

[U25] Py：CSV 按字典读
来源：http://xqa.zhixingplan.top

csv.DictReader(f)
来源：http://lkn.zhengqikj.top

[U26] Py：并发下载
来源：http://icc.sufxvd.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bll.9152youxi.cn

[U27] Py：异步 HTTP
来源：http://lme.hongshengwenyu.top

aiohttp.ClientSession() 配合 async with
来源：http://mbt.yj20258888.top

[U28] Py：类型别名
来源：http://zrx.snrcjt.cn

UserId = int
来源：http://xzn.shzxlz.cn

[U29] Py：属性校验
来源：http://juk.yongpay.top

@property 与 @x.setter 配合
来源：http://haq.bbcook.cn

[U30] Py：数据类
来源：http://wod.shanyushiyangkeji.top

@dataclass(slots=True)
来源：http://ytg.ppjwa.cn

[U31] Py：单测
来源：http://alq.hongshengwenyu.top

python -m pytest -q
来源：http://bbu.jinyuanbaomall.cn

[U32] Py：代码格式化
来源：http://smp.fehbvm.com

ruff format . && ruff check --fix .
来源：http://mbc.smart0.xyz

[U33] Py：打包发布
来源：http://mwi.mhx1999.top

python -m build  （依赖 pyproject.toml）
来源：http://nmd.iojbl.cn

[U34] Py：判断编码
来源：http://pgc.yanxiufei.cn

chardet.detect(raw)
来源：http://riv.yonumen.top

[U35] Py：发送邮件
来源：http://fmn.shanyushiyangkeji.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xoy.jinqigfzy.top

[U36] Py：定时任务
来源：http://klu.bjfxy.top

schedule.every(10).minutes.do(job)
来源：http://afb.hnqzz.top

[U37] Py：读写 Excel
来源：http://dhk.wangshuangyany.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ebv.yj202588.top

[U38] Py：获取脚本所在目录
来源：http://ldd.xziqi.cn

Path(__file__).resolve().parent
来源：http://gyl.hywenlv.cn

[U39] Py：判断是否在交互环境
来源：http://qxm.ywan-chungtsiang.top

sys.stdout.isatty()
来源：http://nln.gaohongyu789.top

[U40] Py：打印到标准错误
来源：http://hzj.shangyingyoupin.top

print("err", file=sys.stderr)
来源：http://lit.hysaishi.cn

[U41] PHP：初始化 Composer 项目
来源：http://jjp.ydjk.org.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://kfz.jlsjyb.cn

[U42] PHP：PSR-4 自动加载
来源：http://ikg.hcnkem.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ydr.cqqwz.cn

[U43] PHP：声明命名空间
来源：http://mcf.yueranfly.top

namespace App\Http;
来源：http://vbj.ppjwa.cn

[U44] PHP：开启严格类型
来源：http://cwc.yonumen.top

declare(strict_types=1);
来源：http://rsz.andypj.xyz

[U45] PHP：类型声明与返回类型
来源：http://ptk.chenjidiqi.icu

function add(int $a, int $b): int { return $a + $b; }
来源：http://rng.cucudq.cn

[U46] PHP：可空类型
来源：http://wjk.vqdsnc.cn

?string $name = null
来源：http://vnn.yj20258.top

[U47] PHP：联合类型
来源：http://rhv.uphjek.com

int|string $id
来源：http://yfx.birdmap.top

[U48] PHP：纯枚举
来源：http://bhh.hnxiangtu.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://scf.chenlongwang.top

[U49] PHP：只读属性
来源：http://mhe.bjfxy.top

public readonly string $name
来源：http://qxm.yongpay.top

[U50] PHP：构造器属性提升
来源：http://uws.jiagoushi.top

public function __construct(private int $id) {}
来源：http://yag.uphjek.com

[U51] PHP：数组解构
来源：http://vjw.redwolf501.top

[$a, $b] = $arr;
来源：http://lwe.ydzc1.top

[U52] PHP：箭头函数
来源：http://otz.yfazqb.com

$double = fn($x) => $x * 2;
来源：http://spy.shuidangran.top

[U53] PHP：空合并运算符
来源：http://kpk.yfazqb.com

$v = $a ?? $b ?? "default";
来源：http://ujb.yuanzhike.top

[U54] PHP：空安全调用
来源：http://xou.hesvh.cn

$obj?->method()
来源：http://osf.yfazqb.com

[U55] PHP：match 表达式
来源：http://ove.jqgfzy.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wqj.daxiang520.top

[U56] PHP：命名参数
来源：http://rdh.jinqigufen.top

f(a: 1, b: 2)
来源：http://bhc.jlsjyb.cn

[U57] PHP：字符串插值
来源：http://tig.andypj.xyz

"值: {$a}"
来源：http://nmy.haohaochexian.top

[U58] PHP：数组三件套
来源：http://dqx.yj20258.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ptd.nanxinkj.top

[U59] PHP：自定义排序
来源：http://mse.haohaochexian.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iyw.0kj1m.cn

[U60] PHP：JSON 编解码
来源：http://fuf.tianlin.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://liz.hongshengwenyu.top

[U61] PHP：正则
来源：http://cis.hesvh.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rtw.dashuyun.cn

[U62] PHP：日期对象
来源：http://crd.yuxming.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jss.andypj.xyz

[U63] PHP：文件读写
来源：http://min.iojbl.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://eam.yongpay.top

[U64] PHP：目录遍历
来源：http://ytw.daxiang520.top

glob("dir/*.php");  scandir("dir");
来源：http://vgq.yj20258.top

[U65] PHP：会话
来源：http://wlo.nwbrower.top

session_start();  $_SESSION["uid"] = 1;
来源：http://jhv.ydjk.org.cn

[U66] PHP：设置 Cookie
来源：http://ekw.aizwys.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://shd.chenjidiqi.icu

[U67] PHP：处理文件上传
来源：http://cch.xziqi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://trj.hcnkem.com

[U68] PHP：PDO 连接
来源：http://oyq.havefunace.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mqz.quarkkingdee.top

[U69] PHP：PDO 预处理
来源：http://ytc.bbcook.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://opa.zhijiandao.cn

[U70] PHP：PDO 事务
来源：http://efd.epnwcf.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://srl.nwbrower.top

[U71] PHP：抛出异常
来源：http://ikd.hnqzz.top

throw new RuntimeException("失败", 500);
来源：http://jaw.yuanzhike.top

[U72] PHP：写错误日志
来源：http://kmf.chenjidiqi.icu

error_log("失败: " . $e->getMessage());
来源：http://ekf.gotoacloud.top

[U73] PHP：读取 ini 配置
来源：http://bgz.gaohongyu789.top

parse_ini_file("config.ini", true)
来源：http://rqf.tarul.cn

[U74] PHP：读取环境变量
来源：http://yps.fzhhl.top

getenv("APP_ENV") ?: "production"
来源：http://zys.aibaodan.cn

[U75] PHP：依赖注入
来源：http://aqc.jianghu66.top

composer require psr/container
来源：http://qdl.cashguo.top

[U76] PHP：简单路由
来源：http://ruw.daxiang520.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://juo.tarul.cn

[U77] PHP：模板渲染
来源：http://hlo.redwolf501.top

composer require twig/twig
来源：http://abv.hnxiangtu.top

[U78] PHP：单元测试
来源：http://xrc.xuetiantiany.cn

composer require --dev phpunit/phpunit
来源：http://ndg.shanyushiyangkeji.top

[U79] PHP：静态分析
来源：http://xih.quarkkingdee.top

composer require --dev phpstan/phpstan
来源：http://nuv.uphjek.com

[U80] PHP：代码规范修复
来源：http://jhd.yj20258888.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://epb.gogol.net.cn

[U81] JS：初始化项目
来源：http://ctv.feifeiyinyue.top

npm init -y;  npm i express
来源：http://tat.yonumen.top

[U82] JS：package.json 脚本
来源：http://lvz.pycfn.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gam.zhiwuduotai.top

[U83] JS：ES Module 导入导出
来源：http://zfe.ivvv.top

export const a = 1;  import { a } from "./m.js";
来源：http://fle.haohaochexian.top

[U84] JS：CommonJS 写法
来源：http://jch.fktsv.cn

module.exports = { a };  const { a } = require("./m");
来源：http://hfq.meibo888.top

[U85] JS：可选链
来源：http://aem.guowangkeji.top

a?.b?.c
来源：http://xyf.zhaomingkeji.xyz

[U86] JS：空值合并
来源：http://olw.xuetiantiany.cn

a ?? b
来源：http://inv.ywan-chungtsiang.top

[U87] JS：解构默认值
来源：http://rva.wangdashe.top

const { a = 1, b = 2 } = obj;
来源：http://ukg.gaohongyu789.top

[U88] JS：对象展开合并
来源：http://dtn.shzxlz.cn

{ ...a, ...b }
来源：http://lpe.andypj.xyz

[U89] JS：数组去重
来源：http://vty.yj20258888.top

[...new Set(arr)]
来源：http://ktm.jinyuanbaomall.cn

[U90] JS：数字数组排序
来源：http://nbz.gogol.net.cn

[...arr].sort((a, b) => a - b)
来源：http://asz.fzhhl.top

[U91] JS：对象键值遍历
来源：http://wph.sxryk.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qcv.zdqjudy.top

[U92] JS：深拷贝
来源：http://gwd.epnwcf.com

structuredClone(obj)
来源：http://wsy.cdnleiting.top

[U93] JS：模板字符串
来源：http://ucu.yj20258.top

`共 ${n} 条`
来源：http://jlg.jinqigufen.top

[U94] JS：箭头函数
来源：http://fyn.zhiwuduotai.top

const double = x => x * 2;
来源：http://vti.xziqi.cn

[U95] JS：Promise 包装
来源：http://ptu.52xcode.cn

new Promise((resolve, reject) => {})
来源：http://ver.smart0.xyz

[U96] JS：async/await 与异常
来源：http://hvt.chenlongwang.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://yuh.jqgufenzy.top

[U97] JS：并发请求
来源：http://gqy.iojbl.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ric.smart0.xyz

[U98] JS：fetch 带 JSON
来源：http://tck.kuanghao11.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ist.chenlongwang.top

[U99] JS：事件监听
来源：http://leb.aizwys.cn

el.addEventListener("click", e => {})
来源：http://kml.tianlin.xyz

[U100] JS：DOM 查询
来源：http://vjs.svipenyu.cn

document.querySelector(".item")
来源：http://pzx.zhijiandao.cn

[U101] JS：classList 操作
来源：http://beb.nanxuanxn.top

el.classList.toggle("active")
来源：http://piq.birdmap.top

[U102] JS：本地存储
来源：http://avn.316326.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://rxp.dianchejie.cn

[U103] JS：定时器
来源：http://wrq.yueranfly.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nfk.zhixingplan.top

[U104] JS：防抖
来源：http://xiv.yuanzhike.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eax.zycfv.cn

[U105] JS：节流
来源：http://yhv.sxryk.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://sxn.cqqwz.cn

[U106] JS：日期格式化
来源：http://nrz.uphjek.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qdl.jiagoushi.top

[U107] JS：数字千分位
来源：http://nsr.jqgfzy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hga.gaohongyu789.top

[U108] JS：随机整数
来源：http://gzg.birdmap.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://iro.316326.xyz

[U109] JS：数组分组
来源：http://jbr.dashuyun.cn

Object.groupBy(arr, x => x.type)
来源：http://gby.fengsongda.top

[U110] JS：数组分块
来源：http://wte.zhoulong.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://utf.gzhubu.top

[U111] JS：对象转 Map
来源：http://xcf.tian-w.cn

new Map(Object.entries(obj))
来源：http://edo.chenzaomai.com

[U112] JS：字符串补位
来源：http://pwd.sufxvd.cn

"7".padStart(3, "0")
来源：http://moi.jinqigfzy.top

[U113] JS：正则替换全部
来源：http://qwp.fanxiaobao.xyz

s.replaceAll("a", "b")
来源：http://qql.andypj.xyz

[U114] JS：JSON 深比较
来源：http://diz.epnwcf.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://pig.c1oappe.top

[U115] JS：生成 UUID
来源：http://xiw.yuanzhike.top

crypto.randomUUID()
来源：http://kiw.ehwqpu.com

[U116] JS：类型检查（JSDoc）
来源：http://smk.hfpthk.cn

/** @param {string} name */ function f(name) {}
来源：http://kfs.gaohongyu789.top

[U117] JS：单元测试
来源：http://lsj.gogol.net.cn

npm i -D vitest;  npx vitest
来源：http://swl.bjfxy.top

[U118] JS：开发服务器
来源：http://yyu.zhiwuduotai.top

npm i -D vite;  npx vite
来源：http://jqm.jyoumei.cn

[U119] JS：生产构建
来源：http://nhp.tanke756.top

npx vite build
来源：http://jtx.cqqwz.cn

[U120] JS：读取环境变量（Vite）
来源：http://nfw.fktsv.cn

import.meta.env.VITE_API_URL
来源：http://tja.316326.xyz

================================================================================
来源：http://ccp.yuxming.cn

统计汇总
来源：http://teh.dashuyun.cn

================================================================================
来源：http://sfm.haohaochexian.top

按语言统计（条）：
来源：http://dev.feifeiyinyue.top

Python ......... 252
来源：http://ktx.ppjwa.cn

PHP ............ 252
来源：http://npv.kuanghao11.cn

JavaScript ..... 252
来源：http://stx.xuanzx.com

TypeScript ..... 212
来源：http://xur.ctjpmb.com

Java ........... 212
来源：http://gcs.ehwqpu.com

Go ............. 212
来源：http://ogr.fehbvm.com

Ruby ........... 212
来源：http://wtj.aibaodan.cn

C# ............. 212
来源：http://vpu.cheryme.top

C .............. 30
来源：http://kef.smart0.xyz

C++ ............ 30
来源：http://lxg.yj20258.top

SQL ............ 90
来源：http://ial.sufxvd.cn

Bash ........... 80
来源：http://hgn.kuanghao11.cn

Kotlin ......... 15
来源：http://wuj.hywenlv.cn

Swift .......... 15
来源：http://jrw.vqdsnc.cn

Lua ............ 10
来源：http://jvx.gogol.net.cn

Perl ........... 10
来源：http://wox.zhaomingkeji.xyz

Scala .......... 10
来源：http://zxe.yj20258.top

------------------------------------
来源：http://yqc.pycfn.com

合计 ........... 2106 条
来源：http://naw.xziqi.cn

按章节统计：
来源：http://dym.52xcode.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://crz.smart0.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://owu.zhaomingkeji.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vww.xuetiantiany.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lso.jqgufenzy.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pyi.zhoulong.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://imc.jianghu66.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://rrt.cucudq.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rjp.yj20258.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xdg.cqqwz.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bom.chenlongwang.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hbz.xuanzx.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nrc.bbcook.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://cmo.nanxinkj.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://fcr.sweek.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qfv.uphjek.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://egq.yfazqb.com

Q SQL 专题                              90
来源：http://gbj.fehbvm.com

R Bash 专题                             80
来源：http://zqf.wangdashe.top

S C / C++ 专题                          60
来源：http://yjx.gogol.net.cn

T 其他语言补充                          60
来源：http://vgt.yfazqb.com

U 高频实用片段                         120
来源：http://wrz.ehwqpu.com

------------------------------------
来源：http://eyg.fengsongda.top

合计                                  2106 条
来源：http://tdj.fanxiaobao.xyz

--------------------------------------------------------------------------------
来源：http://fsh.haohaochexian.top

使用提醒
来源：http://phx.gogol.net.cn

--------------------------------------------------------------------------------
来源：http://uhy.sxryk.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wmb.jyoumei.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jfd.yanxiufei.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://iye.bbcook.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://axb.52xcode.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://cji.sysykeji.top

—— 文件结束 ——
来源：http://prz.zhengqikj.top

================================================================================
来源：http://qea.pengpengdd.cyou

程序语言常见例子速查手册（2024 版）
来源：http://qlr.mhx1999.top

Common Programming Examples Cheat Book
来源：http://bwt.52xcode.cn

================================================================================
来源：http://ghv.zhoulong.xyz

【收录内容】
来源：http://qyg.gogol.net.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://sgo.ydzc1.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://enc.quarkkingdee.top

SQL · Bash · C · C++
来源：http://vnh.fzhhl.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://krj.tanke756.top

【使用说明】
来源：http://jlx.hcnkem.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://bba.cucudq.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://eay.kuanghao11.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ioj.gaohongyu789.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vrc.xinyue.icu

Bash:  Shell         C:     C             C++:   C++
来源：http://fbf.gogol.net.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://kkw.svipenyu.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://zni.sjlbkw.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jfg.fzhhl.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ifw.shanyushiyangtech.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://cde.zhiwuduotai.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vym.ivvv.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://fre.fanxiaobao.xyz

【文件统计】
来源：http://kzd.zhongyouzk.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://yay.52xcode.cn

--------------------------------------------------------------------------------
来源：http://vhw.zhongyouzk.top

目  录
来源：http://kug.nanxuanxn.top

--------------------------------------------------------------------------------
来源：http://zkn.uphjek.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zjh.jinqigfzy.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ivk.yangfankeji.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://uxj.yj20258888.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://fln.snrcjt.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://xnj.sufxvd.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hyg.cqqwz.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://acr.ydzc1.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hdv.sxryk.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ucq.guannengcc.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mto.aibaodan.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://khj.pycfn.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zqu.guowangkeji.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://gae.tarul.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://cwa.kuanghao11.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jkm.tanke756.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://eva.sxryk.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ebq.9152youxi.cn


<!-- 参考信息 -->