代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://udd.epnwcf.com

sys.stdout.isatty()
来源：http://wyb.hnqzz.top

[U40] Py：打印到标准错误
来源：http://jeh.yfazqb.com

print("err", file=sys.stderr)
来源：http://zjo.hesvh.cn

[U41] PHP：初始化 Composer 项目
来源：http://qpu.ppjwa.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://zwi.xziqi.cn

[U42] PHP：PSR-4 自动加载
来源：http://bbb.xingfuxueyuan.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zjc.dianchejie.cn

[U43] PHP：声明命名空间
来源：http://pnv.cheryme.top

namespace App\Http;
来源：http://duv.snrcjt.cn

[U44] PHP：开启严格类型
来源：http://ijz.fzhhl.top

declare(strict_types=1);
来源：http://ykn.zhixingplan.top

[U45] PHP：类型声明与返回类型
来源：http://qho.jinqigfzy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://rcc.jinqigufen.top

[U46] PHP：可空类型
来源：http://edj.ydjk.org.cn

?string $name = null
来源：http://gfx.ppjwa.cn

[U47] PHP：联合类型
来源：http://avi.shzxlz.cn

int|string $id
来源：http://pfd.zhaomingkeji.xyz

[U48] PHP：纯枚举
来源：http://dja.shzxlz.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qur.zhijiandao.cn

[U49] PHP：只读属性
来源：http://kcq.yj20258888.top

public readonly string $name
来源：http://ptb.quarkkingdee.top

[U50] PHP：构造器属性提升
来源：http://juw.gogol.net.cn

public function __construct(private int $id) {}
来源：http://hvp.ydjk.org.cn

[U51] PHP：数组解构
来源：http://gce.cashguo.top

[$a, $b] = $arr;
来源：http://mzd.c1oappe.top

[U52] PHP：箭头函数
来源：http://vun.wangdashe.top

$double = fn($x) => $x * 2;
来源：http://orf.chenlongwang.top

[U53] PHP：空合并运算符
来源：http://hrn.jianghu66.top

$v = $a ?? $b ?? "default";
来源：http://bsn.daria6918.cn

[U54] PHP：空安全调用
来源：http://ear.zdqjudy.top

$obj?->method()
来源：http://xtf.pycfn.com

[U55] PHP：match 表达式
来源：http://jxi.wangshuangyany.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zjb.guannengcc.top

[U56] PHP：命名参数
来源：http://msh.jqgfzy.top

f(a: 1, b: 2)
来源：http://yuc.jinghuilouyu.cn

[U57] PHP：字符串插值
来源：http://vxv.kuanghao11.cn

"值: {$a}"
来源：http://bnt.zhaomingkeji.xyz

[U58] PHP：数组三件套
来源：http://tzx.52xcode.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rbn.chenzaomai.com

[U59] PHP：自定义排序
来源：http://mzz.fehbvm.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hpw.hnqzz.top

[U60] PHP：JSON 编解码
来源：http://ylj.wangdashe.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ozv.shuidangran.top

[U61] PHP：正则
来源：http://aos.andypj.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://elv.xziqi.cn

[U62] PHP：日期对象
来源：http://hqq.ivvv.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://osu.yvedp.cn

[U63] PHP：文件读写
来源：http://bfq.zhaomingkeji.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://suw.zycfv.cn

[U64] PHP：目录遍历
来源：http://quy.316326.xyz

glob("dir/*.php");  scandir("dir");
来源：http://lpw.jqgfzy.top

[U65] PHP：会话
来源：http://lsz.gogol.net.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://hak.yj202588.top

[U66] PHP：设置 Cookie
来源：http://zxb.wangshuangyany.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bmr.dianchejie.cn

[U67] PHP：处理文件上传
来源：http://zki.sufxvd.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zmf.yfazqb.com

[U68] PHP：PDO 连接
来源：http://cge.aibaodan.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://elu.jinghuilouyu.cn

[U69] PHP：PDO 预处理
来源：http://yvd.dashuyun.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jpr.yuanzhike.top

[U70] PHP：PDO 事务
来源：http://run.ywan-chungtsiang.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://amy.hammf.cn

[U71] PHP：抛出异常
来源：http://nim.yfazqb.com

throw new RuntimeException("失败", 500);
来源：http://dyh.epnwcf.com

[U72] PHP：写错误日志
来源：http://uvi.yuanzhike.top

error_log("失败: " . $e->getMessage());
来源：http://rja.redwolf501.top

[U73] PHP：读取 ini 配置
来源：http://oyy.cucudq.cn

parse_ini_file("config.ini", true)
来源：http://blv.smart0.xyz

[U74] PHP：读取环境变量
来源：http://cmm.52xcode.cn

getenv("APP_ENV") ?: "production"
来源：http://zst.tarul.cn

[U75] PHP：依赖注入
来源：http://kje.ppjwa.cn

composer require psr/container
来源：http://div.sysykeji.top

[U76] PHP：简单路由
来源：http://aqu.gaohongyu789.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yll.yangfankeji.com

[U77] PHP：模板渲染
来源：http://sey.ydjk.org.cn

composer require twig/twig
来源：http://bwp.jinqigfzy.top

[U78] PHP：单元测试
来源：http://njb.yvedp.cn

composer require --dev phpunit/phpunit
来源：http://kpa.chenjidiqi.icu

[U79] PHP：静态分析
来源：http://rbw.316326.xyz

composer require --dev phpstan/phpstan
来源：http://tbb.redwolf501.top

[U80] PHP：代码规范修复
来源：http://ogv.hysaishi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ehd.zhoulong.xyz

[U81] JS：初始化项目
来源：http://crt.ppjwa.cn

npm init -y;  npm i express
来源：http://fxh.vehdjk.com

[U82] JS：package.json 脚本
来源：http://ejj.chenlongwang.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://elj.zdqjudy.top

[U83] JS：ES Module 导入导出
来源：http://rdx.xuetiantiany.cn

export const a = 1;  import { a } from "./m.js";
来源：http://wdx.chenzaomai.com

[U84] JS：CommonJS 写法
来源：http://hpi.chenjidiqi.icu

module.exports = { a };  const { a } = require("./m");
来源：http://tdp.yj202588.top

[U85] JS：可选链
来源：http://rlx.pengpengdd.cyou

a?.b?.c
来源：http://vmb.yongpay.top

[U86] JS：空值合并
来源：http://zft.xuetiantiany.cn

a ?? b
来源：http://peu.xylfe.cn

[U87] JS：解构默认值
来源：http://eqn.iojbl.cn

const { a = 1, b = 2 } = obj;
来源：http://vrd.guowangkeji.top

[U88] JS：对象展开合并
来源：http://bgy.zhiwuduotai.top

{ ...a, ...b }
来源：http://vwe.fengsongda.top

[U89] JS：数组去重
来源：http://pkd.gaohongyu789.top

[...new Set(arr)]
来源：http://cpy.fanxiaobao.xyz

[U90] JS：数字数组排序
来源：http://yzt.jiagoushi.top

[...arr].sort((a, b) => a - b)
来源：http://hzg.bjfxy.top

[U91] JS：对象键值遍历
来源：http://mcl.tianlin.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vwd.yuxming.cn

[U92] JS：深拷贝
来源：http://fjh.vqdsnc.cn

structuredClone(obj)
来源：http://pfb.jqgfzy.top

[U93] JS：模板字符串
来源：http://pdd.quarkkingdee.top

`共 ${n} 条`
来源：http://eso.hcnkem.com

[U94] JS：箭头函数
来源：http://uah.zhaomingkeji.xyz

const double = x => x * 2;
来源：http://tfl.daxiang520.top

[U95] JS：Promise 包装
来源：http://ctr.aibaodan.cn

new Promise((resolve, reject) => {})
来源：http://bai.fengsongda.top

[U96] JS：async/await 与异常
来源：http://zlu.tianlin.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://upb.hnxiangtu.top

[U97] JS：并发请求
来源：http://wze.zhiwuduotai.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ftm.hnxiangtu.top

[U98] JS：fetch 带 JSON
来源：http://tya.ywan-chungtsiang.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://kta.sjlbkw.cn

[U99] JS：事件监听
来源：http://yty.zdqjudy.top

el.addEventListener("click", e => {})
来源：http://xcu.smart0.xyz

[U100] JS：DOM 查询
来源：http://sgv.andypj.xyz

document.querySelector(".item")
来源：http://rch.birdmap.top

[U101] JS：classList 操作
来源：http://jkk.yj202588.top

el.classList.toggle("active")
来源：http://mrn.zhiwuduotai.top

[U102] JS：本地存储
来源：http://lll.hongshengwenyu.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://afo.jyoumei.cn

[U103] JS：定时器
来源：http://bls.vqdsnc.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yhx.9152youxi.cn

[U104] JS：防抖
来源：http://vov.c1oappe.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fnt.jlsjyb.cn

[U105] JS：节流
来源：http://fdh.hywenlv.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yrd.zhongyouzk.top

[U106] JS：日期格式化
来源：http://fdm.svipenyu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wmn.smart0.xyz

[U107] JS：数字千分位
来源：http://hoz.hywenlv.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hua.ydzc1.top

[U108] JS：随机整数
来源：http://acc.gaohongyu789.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qau.xuetiantiany.cn

[U109] JS：数组分组
来源：http://zhz.fanxiaobao.xyz

Object.groupBy(arr, x => x.type)
来源：http://tyg.havefunace.top

[U110] JS：数组分块
来源：http://kfz.yfazqb.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wcq.cashguo.top

[U111] JS：对象转 Map
来源：http://kuk.gaohongyu789.top

new Map(Object.entries(obj))
来源：http://lhz.jianghu66.top

[U112] JS：字符串补位
来源：http://til.gzhubu.top

"7".padStart(3, "0")
来源：http://ktp.hnxiangtu.top

[U113] JS：正则替换全部
来源：http://vsr.ydjk.org.cn

s.replaceAll("a", "b")
来源：http://ady.zhixingplan.top

[U114] JS：JSON 深比较
来源：http://rue.fengsongda.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://nap.hongshengwenyu.top

[U115] JS：生成 UUID
来源：http://nmv.birdmap.top

crypto.randomUUID()
来源：http://csx.ppjwa.cn

[U116] JS：类型检查（JSDoc）
来源：http://gws.cashguo.top

/** @param {string} name */ function f(name) {}
来源：http://mzv.hnxiangtu.top

[U117] JS：单元测试
来源：http://ptv.hnqzz.top

npm i -D vitest;  npx vitest
来源：http://ndk.xuetiantiany.cn

[U118] JS：开发服务器
来源：http://dlr.ivvv.top

npm i -D vite;  npx vite
来源：http://vlu.hcnkem.com

[U119] JS：生产构建
来源：http://qvy.jyoumei.cn

npx vite build
来源：http://nkt.zhijiandao.cn

[U120] JS：读取环境变量（Vite）
来源：http://mir.gogol.net.cn

import.meta.env.VITE_API_URL
来源：http://nfw.hnqzz.top

================================================================================
来源：http://nvd.svipenyu.cn

统计汇总
来源：http://xps.zdbjq.cn

================================================================================
来源：http://iyf.dianchejie.cn

按语言统计（条）：
来源：http://gjo.bjfxy.top

Python ......... 252
来源：http://rur.mhx1999.top

PHP ............ 252
来源：http://qxr.epnwcf.com

JavaScript ..... 252
来源：http://svd.dashuyun.cn

TypeScript ..... 212
来源：http://btu.daxiang520.top

Java ........... 212
来源：http://hwb.haohaochexian.top

Go ............. 212
来源：http://dlr.yanxiufei.cn

Ruby ........... 212
来源：http://ccs.gotoacloud.top

C# ............. 212
来源：http://fzq.nanxinkj.top

C .............. 30
来源：http://eau.jianghu66.top

C++ ............ 30
来源：http://wlk.fanxiaobao.xyz

SQL ............ 90
来源：http://hjj.zhaomingkeji.xyz

Bash ........... 80
来源：http://szc.ydzc1.top

Kotlin ......... 15
来源：http://ixa.yfazqb.com

Swift .......... 15
来源：http://dlf.kuanghao11.cn

Lua ............ 10
来源：http://ldh.9152youxi.cn

Perl ........... 10
来源：http://jeo.hammf.cn

Scala .......... 10
来源：http://gfj.zhaomingkeji.xyz

------------------------------------
来源：http://scp.jyoumei.cn

合计 ........... 2106 条
来源：http://isw.nwbrower.top

按章节统计：
来源：http://oxr.zhaomingkeji.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://peq.yangfankeji.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dbp.yj20258.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://twv.9152youxi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xxz.gotoacloud.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://sgi.smart0.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://juy.tanke756.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ode.jinqigufen.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xfm.hnqzz.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nac.uphjek.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://afx.hnqzz.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ktq.yanxiufei.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kau.yanxiufei.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jsa.zhiwuduotai.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://lpe.daxiang520.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wuc.jinyuanbaomall.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wgi.tian-w.cn

Q SQL 专题                              90
来源：http://nha.daxiang520.top

R Bash 专题                             80
来源：http://hve.jqgfzy.top

S C / C++ 专题                          60
来源：http://fto.9152youxi.cn

T 其他语言补充                          60
来源：http://zea.zycfv.cn

U 高频实用片段                         120
来源：http://ikg.ywan-chungtsiang.top

------------------------------------
来源：http://yjf.hnqzz.top

合计                                  2106 条
来源：http://ngo.hammf.cn

--------------------------------------------------------------------------------
来源：http://arg.hcnkem.com

使用提醒
来源：http://ycg.xylfe.cn

--------------------------------------------------------------------------------
来源：http://koy.yueranfly.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://twl.guowangkeji.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://qgi.sxryk.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://dii.daria6918.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://vnc.cqqwz.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://lxz.snrcjt.cn

—— 文件结束 ——
来源：http://cef.ehwqpu.com

================================================================================
来源：http://bde.jqgufenzy.top

程序语言常见例子速查手册（2024 版）
来源：http://ylh.dashuyun.cn

Common Programming Examples Cheat Book
来源：http://vjh.52xcode.cn

================================================================================
来源：http://gvy.dashuyun.cn

【收录内容】
来源：http://ysn.yueranfly.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://nxc.ctjpmb.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nzg.redwolf501.top

SQL · Bash · C · C++
来源：http://pda.jyoumei.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://uwg.yueranfly.top

【使用说明】
来源：http://kpy.havefunace.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://snc.jinghuilouyu.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ins.c1oappe.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://dam.cashguo.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://kyh.c1oappe.top

Bash:  Shell         C:     C             C++:   C++
来源：http://oik.sufxvd.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ptx.yj20258.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://zft.nanxinkj.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://url.smart0.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://pen.vqdsnc.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jfv.havefunace.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://yxc.gotoacloud.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://psi.gogol.net.cn

【文件统计】
来源：http://poh.ybcxt.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://std.andypj.xyz

--------------------------------------------------------------------------------
来源：http://dqv.fengsongda.top

目  录
来源：http://ibo.hysaishi.cn

--------------------------------------------------------------------------------
来源：http://ayq.cheryme.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://shc.svipenyu.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hid.zhijiandao.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://pjq.vehdjk.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://dzw.gzhubu.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hmi.tianlin.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://lhf.nanxuanxn.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://dxx.shangyingyoupin.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zop.9152youxi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://yyb.ppjwa.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://dfl.zhiwuduotai.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wtl.ydjk.org.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://agz.jinqigfzy.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://psg.uphjek.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://oqd.zhixingplan.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://oor.dianchejie.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bgq.ehwqpu.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://dgh.ydzc1.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://iio.snrcjt.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://oxh.yj202588.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://twa.jinqigfzy.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://gdh.sjlbkw.cn

================================================================================
来源：http://whx.daxiang520.top

A. 基础语法与类型
来源：http://gri.hammf.cn

================================================================================
来源：http://fjc.sufxvd.cn

[A01] Hello World
来源：http://lsf.xingfuxueyuan.xyz

Py:   print("Hello, World!")
来源：http://vkv.fehbvm.com

PHP:  echo "Hello, World!";
来源：http://qat.dashuyun.cn

JS:   console.log("Hello, World!");
来源：http://emr.guannengcc.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ihw.vehdjk.com

Java: System.out.println("Hello, World!");
来源：http://mfc.ywan-chungtsiang.top

Go:   fmt.Println("Hello, World!")
来源：http://jru.tianlin.xyz

Ruby: puts "Hello, World!"
来源：http://tml.hywenlv.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://fbt.daria6918.cn

[A02] 变量声明与赋值
来源：http://rkv.zdbjq.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://tzt.pengpengdd.cyou

PHP:  $name = "Alex"; $age = 20;
来源：http://pnv.cheryme.top

JS:   let name = "Alex"; const age = 20;
来源：http://ktk.hcnkem.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://lzd.fktsv.cn

Java: String name = "Alex"; int age = 20;
来源：http://gzn.yj20258.top

Go:   name := "Alex"; age := 20
来源：http://puk.aibaodan.cn

Ruby: name = "Alex"; age = 20
来源：http://hgb.yuxming.cn

C#:   string name = "Alex"; int age = 20;
来源：http://bhj.uphjek.com

[A03] 常量定义
来源：http://jvn.zhaomingkeji.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://cqt.cashguo.top

PHP:  const PI = 3.14159;
来源：http://sul.nanxuanxn.top

JS:   const PI = 3.14159;
来源：http://clz.fehbvm.com

TS:   const PI: number = 3.14159;
来源：http://skz.jyoumei.cn

Java: static final double PI = 3.14159;
来源：http://dop.meibo888.top

Go:   const PI = 3.14159
来源：http://ama.316326.xyz

Ruby: PI = 3.14159
来源：http://mrc.52xcode.cn

C#:   const double PI = 3.14159;
来源：http://udt.fzhhl.top

[A04] 判断变量类型
来源：http://jcf.dianchejie.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://hgd.tanke756.top


<!-- 参考信息 -->