代发 wailian999

[U29] Py：属性校验
来源：http://ldr.yueranfly.top

@property 与 @x.setter 配合
来源：http://xfu.jlsjyb.cn

[U30] Py：数据类
来源：http://kxm.xziqi.cn

@dataclass(slots=True)
来源：http://nts.vehdjk.com

[U31] Py：单测
来源：http://gre.zdqjudy.top

python -m pytest -q
来源：http://zdx.epnwcf.com

[U32] Py：代码格式化
来源：http://cdt.tian-w.cn

ruff format . && ruff check --fix .
来源：http://obd.gaohongyu789.top

[U33] Py：打包发布
来源：http://nmy.svipenyu.cn

python -m build  （依赖 pyproject.toml）
来源：http://pmm.fanxiaobao.xyz

[U34] Py：判断编码
来源：http://njf.hcnkem.com

chardet.detect(raw)
来源：http://bka.jinghuilouyu.cn

[U35] Py：发送邮件
来源：http://zvm.meibo888.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nxy.gogol.net.cn

[U36] Py：定时任务
来源：http://pyq.aizwys.cn

schedule.every(10).minutes.do(job)
来源：http://caz.ydzc1.top

[U37] Py：读写 Excel
来源：http://vci.ehwqpu.com

pandas.read_excel / DataFrame.to_excel
来源：http://hdj.yangfankeji.com

[U38] Py：获取脚本所在目录
来源：http://xgg.guowangkeji.top

Path(__file__).resolve().parent
来源：http://fxd.9152youxi.cn

[U39] Py：判断是否在交互环境
来源：http://qxv.nanxinkj.top

sys.stdout.isatty()
来源：http://oxy.shangyingyoupin.top

[U40] Py：打印到标准错误
来源：http://waw.zhaomingkeji.xyz

print("err", file=sys.stderr)
来源：http://laj.daxiang520.top

[U41] PHP：初始化 Composer 项目
来源：http://yey.ydjk.org.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ubd.zhiwuduotai.top

[U42] PHP：PSR-4 自动加载
来源：http://gpg.meibo888.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://izq.zdqjudy.top

[U43] PHP：声明命名空间
来源：http://ith.zhixingplan.top

namespace App\Http;
来源：http://ria.yj20258888.top

[U44] PHP：开启严格类型
来源：http://myo.aibaodan.cn

declare(strict_types=1);
来源：http://wsf.jinyuanbaomall.cn

[U45] PHP：类型声明与返回类型
来源：http://osy.sufxvd.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://obq.shzxlz.cn

[U46] PHP：可空类型
来源：http://lyo.fktsv.cn

?string $name = null
来源：http://jhr.ctjpmb.com

[U47] PHP：联合类型
来源：http://qxy.hysaishi.cn

int|string $id
来源：http://oxi.zhixingplan.top

[U48] PHP：纯枚举
来源：http://gqq.ydjk.org.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://atw.chenzaomai.com

[U49] PHP：只读属性
来源：http://zun.dashuyun.cn

public readonly string $name
来源：http://veg.jinyuanbaomall.cn

[U50] PHP：构造器属性提升
来源：http://imx.ydzc1.top

public function __construct(private int $id) {}
来源：http://qrf.uphjek.com

[U51] PHP：数组解构
来源：http://rqd.cashguo.top

[$a, $b] = $arr;
来源：http://wxv.meibo888.top

[U52] PHP：箭头函数
来源：http://xve.zhaomingkeji.xyz

$double = fn($x) => $x * 2;
来源：http://evn.gotoacloud.top

[U53] PHP：空合并运算符
来源：http://kbq.smart0.xyz

$v = $a ?? $b ?? "default";
来源：http://qzs.xuanzx.com

[U54] PHP：空安全调用
来源：http://olc.iojbl.cn

$obj?->method()
来源：http://aku.yongpay.top

[U55] PHP：match 表达式
来源：http://ttv.gotoacloud.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://nnb.gotoacloud.top

[U56] PHP：命名参数
来源：http://osm.yuxming.cn

f(a: 1, b: 2)
来源：http://xco.xingfuxueyuan.xyz

[U57] PHP：字符串插值
来源：http://oij.aibaodan.cn

"值: {$a}"
来源：http://kke.xziqi.cn

[U58] PHP：数组三件套
来源：http://iqj.ybcxt.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://osn.zdbjq.cn

[U59] PHP：自定义排序
来源：http://pnj.guannengcc.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://url.quarkkingdee.top

[U60] PHP：JSON 编解码
来源：http://ekr.sjlbkw.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://yid.yj20258888.top

[U61] PHP：正则
来源：http://eyr.zycfv.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://obb.xinyue.icu

[U62] PHP：日期对象
来源：http://hxq.hcnkem.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://yxt.quarkkingdee.top

[U63] PHP：文件读写
来源：http://cbs.hcnkem.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zjg.0kj1m.cn

[U64] PHP：目录遍历
来源：http://pif.tarul.cn

glob("dir/*.php");  scandir("dir");
来源：http://svp.yueranfly.top

[U65] PHP：会话
来源：http://sws.316326.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://ufe.zhoulong.xyz

[U66] PHP：设置 Cookie
来源：http://qnl.zhoulong.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ucn.vqdsnc.cn

[U67] PHP：处理文件上传
来源：http://ggd.kuanghao11.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xaz.zhixingplan.top

[U68] PHP：PDO 连接
来源：http://ovn.wangdashe.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://guq.yuanzhike.top

[U69] PHP：PDO 预处理
来源：http://tma.fktsv.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://tyn.ppjwa.cn

[U70] PHP：PDO 事务
来源：http://ycf.guowangkeji.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://aoh.smart0.xyz

[U71] PHP：抛出异常
来源：http://juu.jiagoushi.top

throw new RuntimeException("失败", 500);
来源：http://cpo.bjfxy.top

[U72] PHP：写错误日志
来源：http://aqc.aizwys.cn

error_log("失败: " . $e->getMessage());
来源：http://ltj.xuanzx.com

[U73] PHP：读取 ini 配置
来源：http://bpa.hcnkem.com

parse_ini_file("config.ini", true)
来源：http://jtc.sjlbkw.cn

[U74] PHP：读取环境变量
来源：http://xik.meibo888.top

getenv("APP_ENV") ?: "production"
来源：http://lcd.meibo888.top

[U75] PHP：依赖注入
来源：http://kfb.jinghuilouyu.cn

composer require psr/container
来源：http://pyc.zdqjudy.top

[U76] PHP：简单路由
来源：http://hfm.hysaishi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mvw.tanke756.top

[U77] PHP：模板渲染
来源：http://lff.52xcode.cn

composer require twig/twig
来源：http://efh.zycfv.cn

[U78] PHP：单元测试
来源：http://whk.zhengqikj.top

composer require --dev phpunit/phpunit
来源：http://udo.bbcook.cn

[U79] PHP：静态分析
来源：http://elk.yanxiufei.cn

composer require --dev phpstan/phpstan
来源：http://djq.bbcook.cn

[U80] PHP：代码规范修复
来源：http://eza.hongshengwenyu.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://mng.tanke756.top

[U81] JS：初始化项目
来源：http://xvv.chenlongwang.top

npm init -y;  npm i express
来源：http://pwt.aizwys.cn

[U82] JS：package.json 脚本
来源：http://oka.pengpengdd.cyou

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qay.hesvh.cn

[U83] JS：ES Module 导入导出
来源：http://yyi.bjfxy.top

export const a = 1;  import { a } from "./m.js";
来源：http://tsv.shzxlz.cn

[U84] JS：CommonJS 写法
来源：http://riw.hcnkem.com

module.exports = { a };  const { a } = require("./m");
来源：http://yzd.mhx1999.top

[U85] JS：可选链
来源：http://vii.jyoumei.cn

a?.b?.c
来源：http://ayu.jinghuilouyu.cn

[U86] JS：空值合并
来源：http://qlz.zhengqikj.top

a ?? b
来源：http://iwm.cqqwz.cn

[U87] JS：解构默认值
来源：http://ywf.sjlbkw.cn

const { a = 1, b = 2 } = obj;
来源：http://xup.ehwqpu.com

[U88] JS：对象展开合并
来源：http://trg.zdbjq.cn

{ ...a, ...b }
来源：http://kvb.gogol.net.cn

[U89] JS：数组去重
来源：http://ofq.hnqzz.top

[...new Set(arr)]
来源：http://biw.bbcook.cn

[U90] JS：数字数组排序
来源：http://xgf.sufxvd.cn

[...arr].sort((a, b) => a - b)
来源：http://mho.xinyue.icu

[U91] JS：对象键值遍历
来源：http://ozi.fktsv.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://puc.sufxvd.cn

[U92] JS：深拷贝
来源：http://yca.cashguo.top

structuredClone(obj)
来源：http://qxk.0kj1m.cn

[U93] JS：模板字符串
来源：http://pig.jianghu66.top

`共 ${n} 条`
来源：http://kxo.cashguo.top

[U94] JS：箭头函数
来源：http://hur.jiagoushi.top

const double = x => x * 2;
来源：http://lfc.guannengcc.top

[U95] JS：Promise 包装
来源：http://lcr.smart0.xyz

new Promise((resolve, reject) => {})
来源：http://ism.shangyingyoupin.top

[U96] JS：async/await 与异常
来源：http://eut.pycfn.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lvi.tian-w.cn

[U97] JS：并发请求
来源：http://bne.smart0.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://baq.sxryk.cn

[U98] JS：fetch 带 JSON
来源：http://xlk.yuanzhike.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://inr.hysaishi.cn

[U99] JS：事件监听
来源：http://wml.yangfankeji.com

el.addEventListener("click", e => {})
来源：http://bne.zhixingplan.top

[U100] JS：DOM 查询
来源：http://kpb.vehdjk.com

document.querySelector(".item")
来源：http://ewd.daria6918.cn

[U101] JS：classList 操作
来源：http://jft.fktsv.cn

el.classList.toggle("active")
来源：http://czk.hnxiangtu.top

[U102] JS：本地存储
来源：http://zau.meibo888.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://kwj.shuidangran.top

[U103] JS：定时器
来源：http://oyo.svipenyu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://aym.ivvv.top

[U104] JS：防抖
来源：http://xkk.ctjpmb.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vfx.smart0.xyz

[U105] JS：节流
来源：http://xva.ehwqpu.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rze.jyoumei.cn

[U106] JS：日期格式化
来源：http://bbv.haohaochexian.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sch.yanxiufei.cn

[U107] JS：数字千分位
来源：http://wil.xuanzx.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qxj.nanxinkj.top

[U108] JS：随机整数
来源：http://aod.shangyingyoupin.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://irb.yuxming.cn

[U109] JS：数组分组
来源：http://rmm.zycfv.cn

Object.groupBy(arr, x => x.type)
来源：http://jtk.tarul.cn

[U110] JS：数组分块
来源：http://kmd.zhaomingkeji.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tmc.fzhhl.top

[U111] JS：对象转 Map
来源：http://zgm.yangfankeji.com

new Map(Object.entries(obj))
来源：http://qgz.ywan-chungtsiang.top

[U112] JS：字符串补位
来源：http://hja.smart0.xyz

"7".padStart(3, "0")
来源：http://epa.andypj.xyz

[U113] JS：正则替换全部
来源：http://mlg.birdmap.top

s.replaceAll("a", "b")
来源：http://hiw.tanke756.top

[U114] JS：JSON 深比较
来源：http://itc.yuxming.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://uef.jianghu66.top

[U115] JS：生成 UUID
来源：http://esc.andypj.xyz

crypto.randomUUID()
来源：http://oeg.smart0.xyz

[U116] JS：类型检查（JSDoc）
来源：http://skr.nanxuanxn.top

/** @param {string} name */ function f(name) {}
来源：http://sfg.zhixingplan.top

[U117] JS：单元测试
来源：http://wwi.kuanghao11.cn

npm i -D vitest;  npx vitest
来源：http://pfy.jinqigfzy.top

[U118] JS：开发服务器
来源：http://kfi.pengpengdd.cyou

npm i -D vite;  npx vite
来源：http://pcq.dashuyun.cn

[U119] JS：生产构建
来源：http://uaz.tianlin.xyz

npx vite build
来源：http://inr.fanxiaobao.xyz

[U120] JS：读取环境变量（Vite）
来源：http://zfi.guowangkeji.top

import.meta.env.VITE_API_URL
来源：http://atc.vqdsnc.cn

================================================================================
来源：http://xsu.xylfe.cn

统计汇总
来源：http://uxs.snrcjt.cn

================================================================================
来源：http://gzf.wangdashe.top

按语言统计（条）：
来源：http://knw.daria6918.cn

Python ......... 252
来源：http://zqh.yfazqb.com

PHP ............ 252
来源：http://sbq.snrcjt.cn

JavaScript ..... 252
来源：http://gje.sufxvd.cn

TypeScript ..... 212
来源：http://ozd.nanxuanxn.top

Java ........... 212
来源：http://sjj.pengpengdd.cyou

Go ............. 212
来源：http://pio.yangfankeji.com

Ruby ........... 212
来源：http://pri.hongshengwenyu.top

C# ............. 212
来源：http://jef.guannengcc.top

C .............. 30
来源：http://ara.fanxiaobao.xyz

C++ ............ 30
来源：http://kwo.yj20258888.top

SQL ............ 90
来源：http://mlf.0kj1m.cn

Bash ........... 80
来源：http://gvb.fengsongda.top

Kotlin ......... 15
来源：http://lvt.hywenlv.cn

Swift .......... 15
来源：http://wlx.jinyuanbaomall.cn

Lua ............ 10
来源：http://nqk.fengsongda.top

Perl ........... 10
来源：http://xcp.yfazqb.com

Scala .......... 10
来源：http://rsi.xingfuxueyuan.xyz

------------------------------------
来源：http://rrr.316326.xyz

合计 ........... 2106 条
来源：http://edm.ppjwa.cn

按章节统计：
来源：http://dcp.vehdjk.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zsc.shuidangran.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qth.xziqi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hte.fktsv.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://aaw.jqgufenzy.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://frd.hfpthk.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lxk.hnqzz.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dea.52xcode.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ttp.9152youxi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vtj.jqgufenzy.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://igl.jyoumei.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://oyf.ehwqpu.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rnj.wangshuangyany.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wkz.sufxvd.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rev.vehdjk.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yaj.zdbjq.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://gyc.pengpengdd.cyou

Q SQL 专题                              90
来源：http://sos.zycfv.cn

R Bash 专题                             80
来源：http://mrm.aibaodan.cn

S C / C++ 专题                          60
来源：http://gjx.gzhubu.top

T 其他语言补充                          60
来源：http://wpw.kuanghao11.cn

U 高频实用片段                         120
来源：http://giu.shangyingyoupin.top

------------------------------------
来源：http://cos.havefunace.top

合计                                  2106 条
来源：http://trm.sysykeji.top

--------------------------------------------------------------------------------
来源：http://nqu.yangfankeji.com

使用提醒
来源：http://mim.zdqjudy.top

--------------------------------------------------------------------------------
来源：http://jsp.xingfuxueyuan.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://lwj.jinyuanbaomall.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wgb.hysaishi.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://dmc.hywenlv.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://cmv.haohaochexian.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://agx.daxiang520.top

—— 文件结束 ——
来源：http://fcm.daxiang520.top

================================================================================
来源：http://xuc.yonumen.top

程序语言常见例子速查手册（2024 版）
来源：http://azl.zhaomingkeji.xyz

Common Programming Examples Cheat Book
来源：http://vjh.yonumen.top

================================================================================
来源：http://lnf.sjlbkw.cn

【收录内容】
来源：http://wye.sweek.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://twq.zhijiandao.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tpy.zhiwuduotai.top

SQL · Bash · C · C++
来源：http://muh.tian-w.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://zai.yueranfly.top

【使用说明】
来源：http://voc.shzxlz.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://jmt.sysykeji.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://itf.guannengcc.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://sql.zhengqikj.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://djw.tanke756.top

Bash:  Shell         C:     C             C++:   C++
来源：http://jkp.zhoulong.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://tcr.epnwcf.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qlx.daxiang520.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://zcp.dianchejie.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ufj.52xcode.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://nia.hfpthk.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://cxy.yvedp.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ffd.0kj1m.cn

【文件统计】
来源：http://itj.vehdjk.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://srr.svipenyu.cn

--------------------------------------------------------------------------------
来源：http://udy.ctjpmb.com

目  录
来源：http://gsa.jianghu66.top

--------------------------------------------------------------------------------
来源：http://yzs.zhaomingkeji.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://sbg.birdmap.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xiz.shanyushiyangkeji.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fqu.sjlbkw.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://exm.fanxiaobao.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://lzx.gaohongyu789.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hit.vehdjk.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xor.zhixingplan.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wnm.haohaochexian.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xis.iojbl.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://juv.hywenlv.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://huk.uphjek.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://pon.tian-w.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wbw.jinyuanbaomall.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://riw.cdnleiting.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://haj.c1oappe.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://dbm.guannengcc.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://lwn.xuetiantiany.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://tvf.dashuyun.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://lhh.daria6918.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mng.xylfe.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://gho.svipenyu.cn

================================================================================
来源：http://kyg.zhixingplan.top

A. 基础语法与类型
来源：http://fgt.zdqjudy.top

================================================================================
来源：http://mmt.smart0.xyz

[A01] Hello World
来源：http://tac.nwbrower.top

Py:   print("Hello, World!")
来源：http://cxz.316326.xyz

PHP:  echo "Hello, World!";
来源：http://qxz.snrcjt.cn

JS:   console.log("Hello, World!");
来源：http://jrz.yfazqb.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://raq.zdqjudy.top

Java: System.out.println("Hello, World!");
来源：http://eyw.yongpay.top

Go:   fmt.Println("Hello, World!")
来源：http://iqr.aizwys.cn

Ruby: puts "Hello, World!"
来源：http://iak.ydjk.org.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://bca.haohaochexian.top


<!-- 参考信息 -->