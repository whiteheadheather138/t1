代发 wailian999

[U29] Py：属性校验
来源：http://adb.quarkkingdee.top

@property 与 @x.setter 配合
来源：http://hxm.zycfv.cn

[U30] Py：数据类
来源：http://eis.fanxiaobao.xyz

@dataclass(slots=True)
来源：http://jts.ppjwa.cn

[U31] Py：单测
来源：http://aoc.snrcjt.cn

python -m pytest -q
来源：http://ksi.sufxvd.cn

[U32] Py：代码格式化
来源：http://giy.cheryme.top

ruff format . && ruff check --fix .
来源：http://xii.quarkkingdee.top

[U33] Py：打包发布
来源：http://pxl.cdnleiting.top

python -m build  （依赖 pyproject.toml）
来源：http://pir.0kj1m.cn

[U34] Py：判断编码
来源：http://hgi.chenlongwang.top

chardet.detect(raw)
来源：http://ujt.wangshuangyany.cn

[U35] Py：发送邮件
来源：http://jvv.vqdsnc.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://stp.vqdsnc.cn

[U36] Py：定时任务
来源：http://yuv.yj202588.top

schedule.every(10).minutes.do(job)
来源：http://lav.zhongyouzk.top

[U37] Py：读写 Excel
来源：http://pws.guannengcc.top

pandas.read_excel / DataFrame.to_excel
来源：http://wab.dianchejie.cn

[U38] Py：获取脚本所在目录
来源：http://amj.zdbjq.cn

Path(__file__).resolve().parent
来源：http://tuk.zycfv.cn

[U39] Py：判断是否在交互环境
来源：http://wdq.yuanzhike.top

sys.stdout.isatty()
来源：http://wyg.sjlbkw.cn

[U40] Py：打印到标准错误
来源：http://xec.hcnkem.com

print("err", file=sys.stderr)
来源：http://zrl.nwbrower.top

[U41] PHP：初始化 Composer 项目
来源：http://eco.9152youxi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://qfh.gzhubu.top

[U42] PHP：PSR-4 自动加载
来源：http://gek.smart0.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zgq.zdqjudy.top

[U43] PHP：声明命名空间
来源：http://vdr.hcnkem.com

namespace App\Http;
来源：http://ycg.mhx1999.top

[U44] PHP：开启严格类型
来源：http://ttc.xuanzx.com

declare(strict_types=1);
来源：http://lhf.gzhubu.top

[U45] PHP：类型声明与返回类型
来源：http://rrh.birdmap.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://qrb.gogol.net.cn

[U46] PHP：可空类型
来源：http://wqf.jqgufenzy.top

?string $name = null
来源：http://osz.jinyuanbaomall.cn

[U47] PHP：联合类型
来源：http://eni.jianghu66.top

int|string $id
来源：http://ame.smart0.xyz

[U48] PHP：纯枚举
来源：http://qgz.yj20258.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://csx.zdqjudy.top

[U49] PHP：只读属性
来源：http://dnf.sysykeji.top

public readonly string $name
来源：http://hyh.fengsongda.top

[U50] PHP：构造器属性提升
来源：http://ori.yueranfly.top

public function __construct(private int $id) {}
来源：http://vcy.hammf.cn

[U51] PHP：数组解构
来源：http://igm.shangyingyoupin.top

[$a, $b] = $arr;
来源：http://kyh.jiagoushi.top

[U52] PHP：箭头函数
来源：http://xbz.shuidangran.top

$double = fn($x) => $x * 2;
来源：http://ods.vehdjk.com

[U53] PHP：空合并运算符
来源：http://zgb.feifeiyinyue.top

$v = $a ?? $b ?? "default";
来源：http://hlw.fanxiaobao.xyz

[U54] PHP：空安全调用
来源：http://pfe.jinqigfzy.top

$obj?->method()
来源：http://xhd.hywenlv.cn

[U55] PHP：match 表达式
来源：http://dab.kuanghao11.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://keo.zdqjudy.top

[U56] PHP：命名参数
来源：http://evg.daria6918.cn

f(a: 1, b: 2)
来源：http://inv.wangdashe.top

[U57] PHP：字符串插值
来源：http://pwd.vehdjk.com

"值: {$a}"
来源：http://ucy.hesvh.cn

[U58] PHP：数组三件套
来源：http://avy.chenjidiqi.icu

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rdc.nanxinkj.top

[U59] PHP：自定义排序
来源：http://uhs.quarkkingdee.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://anx.smart0.xyz

[U60] PHP：JSON 编解码
来源：http://wge.hcnkem.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ric.fanxiaobao.xyz

[U61] PHP：正则
来源：http://yzr.hnqzz.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://oxo.haohaochexian.top

[U62] PHP：日期对象
来源：http://omi.zhengqikj.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vyp.shangyingyoupin.top

[U63] PHP：文件读写
来源：http://hnj.jyoumei.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://unb.yuxming.cn

[U64] PHP：目录遍历
来源：http://khg.chenlongwang.top

glob("dir/*.php");  scandir("dir");
来源：http://tcj.guannengcc.top

[U65] PHP：会话
来源：http://vgp.52xcode.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://dyv.xuetiantiany.cn

[U66] PHP：设置 Cookie
来源：http://qhc.zhaomingkeji.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ltd.zhiwuduotai.top

[U67] PHP：处理文件上传
来源：http://kkk.ybcxt.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ztv.zdqjudy.top

[U68] PHP：PDO 连接
来源：http://ksz.yfazqb.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gvu.chenjidiqi.icu

[U69] PHP：PDO 预处理
来源：http://gme.wangdashe.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jhp.gzhubu.top

[U70] PHP：PDO 事务
来源：http://cmy.hysaishi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ptq.hnqzz.top

[U71] PHP：抛出异常
来源：http://off.wangshuangyany.cn

throw new RuntimeException("失败", 500);
来源：http://xvk.fktsv.cn

[U72] PHP：写错误日志
来源：http://trm.zhijiandao.cn

error_log("失败: " . $e->getMessage());
来源：http://zbz.xziqi.cn

[U73] PHP：读取 ini 配置
来源：http://whq.xingfuxueyuan.xyz

parse_ini_file("config.ini", true)
来源：http://exn.zhaomingkeji.xyz

[U74] PHP：读取环境变量
来源：http://bpi.shanyushiyangkeji.top

getenv("APP_ENV") ?: "production"
来源：http://pvd.feifeiyinyue.top

[U75] PHP：依赖注入
来源：http://qjt.hongshengwenyu.top

composer require psr/container
来源：http://pkm.fanxiaobao.xyz

[U76] PHP：简单路由
来源：http://pez.cheryme.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://anx.snrcjt.cn

[U77] PHP：模板渲染
来源：http://aqf.wangdashe.top

composer require twig/twig
来源：http://bkc.hongshengwenyu.top

[U78] PHP：单元测试
来源：http://ivi.zycfv.cn

composer require --dev phpunit/phpunit
来源：http://hfy.tanke756.top

[U79] PHP：静态分析
来源：http://brl.guowangkeji.top

composer require --dev phpstan/phpstan
来源：http://yxf.nwbrower.top

[U80] PHP：代码规范修复
来源：http://ypp.yanxiufei.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://niy.jinqigufen.top

[U81] JS：初始化项目
来源：http://ezt.gzhubu.top

npm init -y;  npm i express
来源：http://dko.feifeiyinyue.top

[U82] JS：package.json 脚本
来源：http://axe.xinyue.icu

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nyq.aibaodan.cn

[U83] JS：ES Module 导入导出
来源：http://zca.sweek.top

export const a = 1;  import { a } from "./m.js";
来源：http://hgl.fehbvm.com

[U84] JS：CommonJS 写法
来源：http://aha.ywan-chungtsiang.top

module.exports = { a };  const { a } = require("./m");
来源：http://thk.meibo888.top

[U85] JS：可选链
来源：http://jlb.shzxlz.cn

a?.b?.c
来源：http://aww.gaohongyu789.top

[U86] JS：空值合并
来源：http://trl.zhiwuduotai.top

a ?? b
来源：http://kkj.c1oappe.top

[U87] JS：解构默认值
来源：http://caa.gogol.net.cn

const { a = 1, b = 2 } = obj;
来源：http://pqj.kuanghao11.cn

[U88] JS：对象展开合并
来源：http://cdz.cdnleiting.top

{ ...a, ...b }
来源：http://cea.ppjwa.cn

[U89] JS：数组去重
来源：http://gni.haohaochexian.top

[...new Set(arr)]
来源：http://uwg.cucudq.cn

[U90] JS：数字数组排序
来源：http://uth.ydzc1.top

[...arr].sort((a, b) => a - b)
来源：http://hgl.guowangkeji.top

[U91] JS：对象键值遍历
来源：http://tba.tian-w.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://loq.haohaochexian.top

[U92] JS：深拷贝
来源：http://prx.ydjk.org.cn

structuredClone(obj)
来源：http://bfx.xinyue.icu

[U93] JS：模板字符串
来源：http://kcl.ydjk.org.cn

`共 ${n} 条`
来源：http://cdi.shzxlz.cn

[U94] JS：箭头函数
来源：http://kly.daxiang520.top

const double = x => x * 2;
来源：http://irg.jianghu66.top

[U95] JS：Promise 包装
来源：http://bni.sxryk.cn

new Promise((resolve, reject) => {})
来源：http://koz.vqdsnc.cn

[U96] JS：async/await 与异常
来源：http://gpn.hongshengwenyu.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://yje.c1oappe.top

[U97] JS：并发请求
来源：http://xvn.cashguo.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://okh.fktsv.cn

[U98] JS：fetch 带 JSON
来源：http://wvo.feifeiyinyue.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ici.zdbjq.cn

[U99] JS：事件监听
来源：http://upa.sufxvd.cn

el.addEventListener("click", e => {})
来源：http://jco.yj20258.top

[U100] JS：DOM 查询
来源：http://xal.zdbjq.cn

document.querySelector(".item")
来源：http://ofw.bjfxy.top

[U101] JS：classList 操作
来源：http://zcw.kuanghao11.cn

el.classList.toggle("active")
来源：http://idk.52xcode.cn

[U102] JS：本地存储
来源：http://tne.ydjk.org.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://hnp.nwbrower.top

[U103] JS：定时器
来源：http://tld.dianchejie.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xtr.c1oappe.top

[U104] JS：防抖
来源：http://dtj.gaohongyu789.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nyb.zhijiandao.cn

[U105] JS：节流
来源：http://itx.snrcjt.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hhg.cdnleiting.top

[U106] JS：日期格式化
来源：http://cpg.yueranfly.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rtj.wangdashe.top

[U107] JS：数字千分位
来源：http://yif.yanxiufei.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://med.zhengqikj.top

[U108] JS：随机整数
来源：http://nab.9152youxi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tzo.gogol.net.cn

[U109] JS：数组分组
来源：http://smo.ybcxt.top

Object.groupBy(arr, x => x.type)
来源：http://jmr.zhixingplan.top

[U110] JS：数组分块
来源：http://vun.meibo888.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ino.jqgfzy.top

[U111] JS：对象转 Map
来源：http://sxt.jiagoushi.top

new Map(Object.entries(obj))
来源：http://ukr.wangshuangyany.cn

[U112] JS：字符串补位
来源：http://cvr.wangshuangyany.cn

"7".padStart(3, "0")
来源：http://apc.pengpengdd.cyou

[U113] JS：正则替换全部
来源：http://gor.yongpay.top

s.replaceAll("a", "b")
来源：http://waj.zdqjudy.top

[U114] JS：JSON 深比较
来源：http://iqe.cucudq.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://yrw.dianchejie.cn

[U115] JS：生成 UUID
来源：http://phf.yj20258888.top

crypto.randomUUID()
来源：http://gjs.andypj.xyz

[U116] JS：类型检查（JSDoc）
来源：http://reg.zhongyouzk.top

/** @param {string} name */ function f(name) {}
来源：http://hhy.meibo888.top

[U117] JS：单元测试
来源：http://boz.yongpay.top

npm i -D vitest;  npx vitest
来源：http://zwa.gogol.net.cn

[U118] JS：开发服务器
来源：http://qco.sxryk.cn

npm i -D vite;  npx vite
来源：http://pvc.316326.xyz

[U119] JS：生产构建
来源：http://rwf.gogol.net.cn

npx vite build
来源：http://dod.uphjek.com

[U120] JS：读取环境变量（Vite）
来源：http://qrm.zhengqikj.top

import.meta.env.VITE_API_URL
来源：http://cth.vqdsnc.cn

================================================================================
来源：http://tgv.jiagoushi.top

统计汇总
来源：http://ods.tianlin.xyz

================================================================================
来源：http://dwy.sysykeji.top

按语言统计（条）：
来源：http://bdn.9152youxi.cn

Python ......... 252
来源：http://elu.yueranfly.top

PHP ............ 252
来源：http://rfe.ppjwa.cn

JavaScript ..... 252
来源：http://owm.yongpay.top

TypeScript ..... 212
来源：http://zhz.ydzc1.top

Java ........... 212
来源：http://ajs.yj20258888.top

Go ............. 212
来源：http://rqh.chenlongwang.top

Ruby ........... 212
来源：http://oeb.yvedp.cn

C# ............. 212
来源：http://cxx.jinqigufen.top

C .............. 30
来源：http://sly.hcnkem.com

C++ ............ 30
来源：http://uei.wangshuangyany.cn

SQL ............ 90
来源：http://ffn.jqgfzy.top

Bash ........... 80
来源：http://mfi.chenzaomai.com

Kotlin ......... 15
来源：http://pic.jinqigufen.top

Swift .......... 15
来源：http://cmy.zhongyouzk.top

Lua ............ 10
来源：http://yru.jianghu66.top

Perl ........... 10
来源：http://cnv.haohaochexian.top

Scala .......... 10
来源：http://wnw.fanxiaobao.xyz

------------------------------------
来源：http://nuo.daxiang520.top

合计 ........... 2106 条
来源：http://mjy.52xcode.cn

按章节统计：
来源：http://glf.shzxlz.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ayl.redwolf501.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://sqi.gzhubu.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://upy.aibaodan.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qhr.ywan-chungtsiang.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xoo.chenzaomai.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://odi.birdmap.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://edg.chenjidiqi.icu

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vlj.nanxuanxn.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hxr.cashguo.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ham.fanxiaobao.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://coj.yonumen.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hpz.mhx1999.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ljx.yuanzhike.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ntu.jlsjyb.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://tqv.chenjidiqi.icu

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://zel.zhoulong.xyz

Q SQL 专题                              90
来源：http://uxf.vqdsnc.cn

R Bash 专题                             80
来源：http://lic.birdmap.top

S C / C++ 专题                          60
来源：http://spg.jqgufenzy.top

T 其他语言补充                          60
来源：http://gxf.birdmap.top

U 高频实用片段                         120
来源：http://rsj.jqgfzy.top

------------------------------------
来源：http://ukb.cucudq.cn

合计                                  2106 条
来源：http://wlk.c1oappe.top

--------------------------------------------------------------------------------
来源：http://tdn.hnqzz.top

使用提醒
来源：http://npm.havefunace.top

--------------------------------------------------------------------------------
来源：http://nuq.zhijiandao.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://amc.vehdjk.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://sir.zhoulong.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://zpw.xziqi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://xnd.yuanzhike.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wcl.shzxlz.cn

—— 文件结束 ——
来源：http://ovo.hesvh.cn

================================================================================
来源：http://hmt.fzhhl.top

程序语言常见例子速查手册（2024 版）
来源：http://gew.jlsjyb.cn

Common Programming Examples Cheat Book
来源：http://vrb.fzhhl.top

================================================================================
来源：http://nyv.0kj1m.cn

【收录内容】
来源：http://qda.cheryme.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://fgm.dianchejie.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://pbl.jyoumei.cn

SQL · Bash · C · C++
来源：http://imc.chenjidiqi.icu

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ukv.yj20258888.top

【使用说明】
来源：http://dne.sysykeji.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://oku.jqgfzy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wrc.hysaishi.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://cxu.havefunace.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://yys.fanxiaobao.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://skd.hysaishi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://qfq.snrcjt.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://oty.guowangkeji.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ghc.xuetiantiany.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://aji.dianchejie.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gpk.chenjidiqi.icu

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://xeb.sxryk.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://cah.daxiang520.top

【文件统计】
来源：http://sjp.hnxiangtu.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://tgc.cucudq.cn

--------------------------------------------------------------------------------
来源：http://hka.bjfxy.top

目  录
来源：http://lwb.pycfn.com

--------------------------------------------------------------------------------
来源：http://xkn.sysykeji.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mef.bjfxy.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://swd.cashguo.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://aek.epnwcf.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://fyt.ivvv.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://yyo.hongshengwenyu.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ucq.sweek.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ztv.havefunace.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://pci.cdnleiting.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://msa.yj20258888.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://udf.dashuyun.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://nto.hysaishi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://yjf.yvedp.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://rup.fanxiaobao.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://woa.jinqigfzy.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://iuf.ppjwa.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wla.xingfuxueyuan.xyz

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wuk.shuidangran.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://csf.shuidangran.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://nbu.dianchejie.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hkq.svipenyu.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://iml.fktsv.cn

================================================================================
来源：http://cbl.chenlongwang.top

A. 基础语法与类型
来源：http://afp.birdmap.top

================================================================================
来源：http://tmi.hcnkem.com

[A01] Hello World
来源：http://jog.chenjidiqi.icu

Py:   print("Hello, World!")
来源：http://zhx.316326.xyz

PHP:  echo "Hello, World!";
来源：http://jot.jianghu66.top

JS:   console.log("Hello, World!");
来源：http://vdz.fengsongda.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://gby.fanxiaobao.xyz

Java: System.out.println("Hello, World!");
来源：http://dxy.zdbjq.cn

Go:   fmt.Println("Hello, World!")
来源：http://htr.jqgfzy.top

Ruby: puts "Hello, World!"
来源：http://qlg.dashuyun.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://bmn.yongpay.top


<!-- 参考信息 -->