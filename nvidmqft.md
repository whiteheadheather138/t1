代发 wailian999

[U33] Py：打包发布
来源：http://izd.gotoacloud.top

python -m build  （依赖 pyproject.toml）
来源：http://rvz.chenzaomai.com

[U34] Py：判断编码
来源：http://tex.smart0.xyz

chardet.detect(raw)
来源：http://rpk.zdqjudy.top

[U35] Py：发送邮件
来源：http://gco.yvedp.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://coo.hnxiangtu.top

[U36] Py：定时任务
来源：http://utc.sufxvd.cn

schedule.every(10).minutes.do(job)
来源：http://gbk.fzhhl.top

[U37] Py：读写 Excel
来源：http://bmf.hcnkem.com

pandas.read_excel / DataFrame.to_excel
来源：http://pic.epnwcf.com

[U38] Py：获取脚本所在目录
来源：http://gfn.chenlongwang.top

Path(__file__).resolve().parent
来源：http://kyb.gotoacloud.top

[U39] Py：判断是否在交互环境
来源：http://bqw.hywenlv.cn

sys.stdout.isatty()
来源：http://cii.cheryme.top

[U40] Py：打印到标准错误
来源：http://xpt.havefunace.top

print("err", file=sys.stderr)
来源：http://ywf.nwbrower.top

[U41] PHP：初始化 Composer 项目
来源：http://pwl.cqqwz.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://bwh.shanyushiyangtech.top

[U42] PHP：PSR-4 自动加载
来源：http://xlp.jinyuanbaomall.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://noo.cucudq.cn

[U43] PHP：声明命名空间
来源：http://heh.yvedp.cn

namespace App\Http;
来源：http://omo.fanxiaobao.xyz

[U44] PHP：开启严格类型
来源：http://wuy.gotoacloud.top

declare(strict_types=1);
来源：http://thh.hysaishi.cn

[U45] PHP：类型声明与返回类型
来源：http://zqb.sufxvd.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://qyq.ppjwa.cn

[U46] PHP：可空类型
来源：http://ybm.yfazqb.com

?string $name = null
来源：http://mxh.sysykeji.top

[U47] PHP：联合类型
来源：http://vlr.uphjek.com

int|string $id
来源：http://vjd.hammf.cn

[U48] PHP：纯枚举
来源：http://qmk.cucudq.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://meq.zhixingplan.top

[U49] PHP：只读属性
来源：http://xpw.aibaodan.cn

public readonly string $name
来源：http://xul.smart0.xyz

[U50] PHP：构造器属性提升
来源：http://ukj.cucudq.cn

public function __construct(private int $id) {}
来源：http://kns.tanke756.top

[U51] PHP：数组解构
来源：http://chc.fzhhl.top

[$a, $b] = $arr;
来源：http://vdf.ybcxt.top

[U52] PHP：箭头函数
来源：http://fbo.yongpay.top

$double = fn($x) => $x * 2;
来源：http://yez.wangshuangyany.cn

[U53] PHP：空合并运算符
来源：http://wwl.yongpay.top

$v = $a ?? $b ?? "default";
来源：http://skf.52xcode.cn

[U54] PHP：空安全调用
来源：http://pab.316326.xyz

$obj?->method()
来源：http://zar.hongshengwenyu.top

[U55] PHP：match 表达式
来源：http://yim.zhongyouzk.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dbz.c1oappe.top

[U56] PHP：命名参数
来源：http://kgs.yangfankeji.com

f(a: 1, b: 2)
来源：http://oqz.quarkkingdee.top

[U57] PHP：字符串插值
来源：http://wlf.yj20258888.top

"值: {$a}"
来源：http://wjk.xingfuxueyuan.xyz

[U58] PHP：数组三件套
来源：http://slj.yfazqb.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xui.yangfankeji.com

[U59] PHP：自定义排序
来源：http://cge.sjlbkw.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://upt.cashguo.top

[U60] PHP：JSON 编解码
来源：http://rbc.jinqigufen.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wkp.yj202588.top

[U61] PHP：正则
来源：http://dwj.epnwcf.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qbu.gotoacloud.top

[U62] PHP：日期对象
来源：http://fbm.birdmap.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xvv.fengsongda.top

[U63] PHP：文件读写
来源：http://bdf.jqgfzy.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rqc.zycfv.cn

[U64] PHP：目录遍历
来源：http://wan.daxiang520.top

glob("dir/*.php");  scandir("dir");
来源：http://hjs.fengsongda.top

[U65] PHP：会话
来源：http://cqf.sxryk.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://cis.zhixingplan.top

[U66] PHP：设置 Cookie
来源：http://yes.yueranfly.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jbm.meibo888.top

[U67] PHP：处理文件上传
来源：http://tji.jqgufenzy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zvz.nanxuanxn.top

[U68] PHP：PDO 连接
来源：http://kjk.ppjwa.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://idq.jinqigufen.top

[U69] PHP：PDO 预处理
来源：http://ghf.yueranfly.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vzp.jianghu66.top

[U70] PHP：PDO 事务
来源：http://utf.ydzc1.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zeg.chenzaomai.com

[U71] PHP：抛出异常
来源：http://tzs.yj20258.top

throw new RuntimeException("失败", 500);
来源：http://rnr.yj20258.top

[U72] PHP：写错误日志
来源：http://zxa.chenjidiqi.icu

error_log("失败: " . $e->getMessage());
来源：http://gao.sweek.top

[U73] PHP：读取 ini 配置
来源：http://frn.jqgfzy.top

parse_ini_file("config.ini", true)
来源：http://nlh.haohaochexian.top

[U74] PHP：读取环境变量
来源：http://acv.hammf.cn

getenv("APP_ENV") ?: "production"
来源：http://pls.jinqigfzy.top

[U75] PHP：依赖注入
来源：http://ssh.chenzaomai.com

composer require psr/container
来源：http://kuu.chenlongwang.top

[U76] PHP：简单路由
来源：http://ddn.gzhubu.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ovt.xingfuxueyuan.xyz

[U77] PHP：模板渲染
来源：http://ciy.yvedp.cn

composer require twig/twig
来源：http://kiy.316326.xyz

[U78] PHP：单元测试
来源：http://etv.dianchejie.cn

composer require --dev phpunit/phpunit
来源：http://npt.xingfuxueyuan.xyz

[U79] PHP：静态分析
来源：http://zfu.chenlongwang.top

composer require --dev phpstan/phpstan
来源：http://szd.sysykeji.top

[U80] PHP：代码规范修复
来源：http://xff.cashguo.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://jkk.yueranfly.top

[U81] JS：初始化项目
来源：http://fbk.yongpay.top

npm init -y;  npm i express
来源：http://mso.shuidangran.top

[U82] JS：package.json 脚本
来源：http://mrs.shzxlz.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://osq.shanyushiyangtech.top

[U83] JS：ES Module 导入导出
来源：http://zce.jyoumei.cn

export const a = 1;  import { a } from "./m.js";
来源：http://cij.xingfuxueyuan.xyz

[U84] JS：CommonJS 写法
来源：http://chu.hesvh.cn

module.exports = { a };  const { a } = require("./m");
来源：http://btn.zycfv.cn

[U85] JS：可选链
来源：http://abg.shangyingyoupin.top

a?.b?.c
来源：http://xps.yfazqb.com

[U86] JS：空值合并
来源：http://ldx.gogol.net.cn

a ?? b
来源：http://eoy.yuanzhike.top

[U87] JS：解构默认值
来源：http://pno.jinghuilouyu.cn

const { a = 1, b = 2 } = obj;
来源：http://skb.epnwcf.com

[U88] JS：对象展开合并
来源：http://ofw.daxiang520.top

{ ...a, ...b }
来源：http://obq.svipenyu.cn

[U89] JS：数组去重
来源：http://bso.yangfankeji.com

[...new Set(arr)]
来源：http://liv.tanke756.top

[U90] JS：数字数组排序
来源：http://gve.xuanzx.com

[...arr].sort((a, b) => a - b)
来源：http://mrw.jinqigfzy.top

[U91] JS：对象键值遍历
来源：http://tpk.yangfankeji.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hgh.haohaochexian.top

[U92] JS：深拷贝
来源：http://rmb.zycfv.cn

structuredClone(obj)
来源：http://pen.chenjidiqi.icu

[U93] JS：模板字符串
来源：http://cco.jinqigufen.top

`共 ${n} 条`
来源：http://mxz.bbcook.cn

[U94] JS：箭头函数
来源：http://gfe.guannengcc.top

const double = x => x * 2;
来源：http://lma.yfazqb.com

[U95] JS：Promise 包装
来源：http://yco.ywan-chungtsiang.top

new Promise((resolve, reject) => {})
来源：http://evb.hfpthk.cn

[U96] JS：async/await 与异常
来源：http://pjn.chenlongwang.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cpn.yj20258.top

[U97] JS：并发请求
来源：http://crh.hfpthk.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://gbo.yj20258888.top

[U98] JS：fetch 带 JSON
来源：http://glx.zhongyouzk.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tee.jqgfzy.top

[U99] JS：事件监听
来源：http://zrb.yj202588.top

el.addEventListener("click", e => {})
来源：http://hci.vqdsnc.cn

[U100] JS：DOM 查询
来源：http://pra.yanxiufei.cn

document.querySelector(".item")
来源：http://ozm.snrcjt.cn

[U101] JS：classList 操作
来源：http://ceq.kuanghao11.cn

el.classList.toggle("active")
来源：http://ycw.c1oappe.top

[U102] JS：本地存储
来源：http://chx.aibaodan.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ngg.chenlongwang.top

[U103] JS：定时器
来源：http://lqm.fehbvm.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zef.zdbjq.cn

[U104] JS：防抖
来源：http://xxy.sysykeji.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qcr.guannengcc.top

[U105] JS：节流
来源：http://pvl.chenlongwang.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://djr.zhijiandao.cn

[U106] JS：日期格式化
来源：http://tin.havefunace.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fcx.sysykeji.top

[U107] JS：数字千分位
来源：http://zoq.hongshengwenyu.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://euc.kuanghao11.cn

[U108] JS：随机整数
来源：http://psq.havefunace.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nik.yj20258888.top

[U109] JS：数组分组
来源：http://syb.snrcjt.cn

Object.groupBy(arr, x => x.type)
来源：http://csl.ybcxt.top

[U110] JS：数组分块
来源：http://wor.jiagoushi.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://erp.316326.xyz

[U111] JS：对象转 Map
来源：http://aew.zycfv.cn

new Map(Object.entries(obj))
来源：http://zmd.smart0.xyz

[U112] JS：字符串补位
来源：http://bcm.dianchejie.cn

"7".padStart(3, "0")
来源：http://ltq.tian-w.cn

[U113] JS：正则替换全部
来源：http://fdd.zhongyouzk.top

s.replaceAll("a", "b")
来源：http://afi.uphjek.com

[U114] JS：JSON 深比较
来源：http://jei.kuanghao11.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://nda.tarul.cn

[U115] JS：生成 UUID
来源：http://mtp.ppjwa.cn

crypto.randomUUID()
来源：http://eee.hongshengwenyu.top

[U116] JS：类型检查（JSDoc）
来源：http://pik.nanxinkj.top

/** @param {string} name */ function f(name) {}
来源：http://rvt.dashuyun.cn

[U117] JS：单元测试
来源：http://ydr.nwbrower.top

npm i -D vitest;  npx vitest
来源：http://kia.yanxiufei.cn

[U118] JS：开发服务器
来源：http://zzj.nwbrower.top

npm i -D vite;  npx vite
来源：http://egs.hongshengwenyu.top

[U119] JS：生产构建
来源：http://ffa.wangshuangyany.cn

npx vite build
来源：http://ozb.xinyue.icu

[U120] JS：读取环境变量（Vite）
来源：http://hjr.yj20258.top

import.meta.env.VITE_API_URL
来源：http://ppv.sufxvd.cn

================================================================================
来源：http://zsg.chenzaomai.com

统计汇总
来源：http://kei.andypj.xyz

================================================================================
来源：http://cgc.yuxming.cn

按语言统计（条）：
来源：http://qww.fzhhl.top

Python ......... 252
来源：http://tds.zhoulong.xyz

PHP ............ 252
来源：http://krc.shuidangran.top

JavaScript ..... 252
来源：http://cvh.ivvv.top

TypeScript ..... 212
来源：http://qms.chenlongwang.top

Java ........... 212
来源：http://zvp.jqgufenzy.top

Go ............. 212
来源：http://sng.zdqjudy.top

Ruby ........... 212
来源：http://vms.haohaochexian.top

C# ............. 212
来源：http://iwf.zycfv.cn

C .............. 30
来源：http://qpk.xylfe.cn

C++ ............ 30
来源：http://ivp.0kj1m.cn

SQL ............ 90
来源：http://axn.chenlongwang.top

Bash ........... 80
来源：http://ood.xingfuxueyuan.xyz

Kotlin ......... 15
来源：http://mwn.xinyue.icu

Swift .......... 15
来源：http://kiy.hywenlv.cn

Lua ............ 10
来源：http://fhg.snrcjt.cn

Perl ........... 10
来源：http://mxp.svipenyu.cn

Scala .......... 10
来源：http://aaw.dianchejie.cn

------------------------------------
来源：http://njr.jqgufenzy.top

合计 ........... 2106 条
来源：http://jqe.yj20258.top

按章节统计：
来源：http://jpa.ppjwa.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xnm.dashuyun.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bns.xziqi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lkx.gotoacloud.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vym.fanxiaobao.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nlm.ydjk.org.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wfz.c1oappe.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mmz.yuanzhike.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nsa.ydjk.org.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://chy.xingfuxueyuan.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yff.hywenlv.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://way.zdqjudy.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dpe.jyoumei.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bzc.shangyingyoupin.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://thx.andypj.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ddt.yuanzhike.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://eaj.tarul.cn

Q SQL 专题                              90
来源：http://ine.nanxinkj.top

R Bash 专题                             80
来源：http://iux.jinqigfzy.top

S C / C++ 专题                          60
来源：http://zrn.chenzaomai.com

T 其他语言补充                          60
来源：http://qbn.fzhhl.top

U 高频实用片段                         120
来源：http://bks.ydjk.org.cn

------------------------------------
来源：http://ige.pycfn.com

合计                                  2106 条
来源：http://hix.cashguo.top

--------------------------------------------------------------------------------
来源：http://dnw.shzxlz.cn

使用提醒
来源：http://gso.gogol.net.cn

--------------------------------------------------------------------------------
来源：http://tlw.gotoacloud.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://olv.gzhubu.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mzh.jqgufenzy.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://psj.yvedp.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://cvc.sjlbkw.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rab.ehwqpu.com

—— 文件结束 ——
来源：http://esz.hnxiangtu.top

================================================================================
来源：http://kwg.sweek.top

程序语言常见例子速查手册（2024 版）
来源：http://wce.ydjk.org.cn

Common Programming Examples Cheat Book
来源：http://yrp.jlsjyb.cn

================================================================================
来源：http://nma.0kj1m.cn

【收录内容】
来源：http://wjz.xuetiantiany.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://nvu.shanyushiyangkeji.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ztm.quarkkingdee.top

SQL · Bash · C · C++
来源：http://quy.jqgfzy.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ieu.yuxming.cn

【使用说明】
来源：http://std.ehwqpu.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://crd.mhx1999.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://cej.hnxiangtu.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mtu.ivvv.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://kaz.quarkkingdee.top

Bash:  Shell         C:     C             C++:   C++
来源：http://plu.andypj.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jvi.snrcjt.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://bss.yangfankeji.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://zbz.vqdsnc.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jqo.sjlbkw.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://fcd.fehbvm.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://jij.gogol.net.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mop.shzxlz.cn

【文件统计】
来源：http://kwc.sxryk.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qkt.yj202588.top

--------------------------------------------------------------------------------
来源：http://ytx.pycfn.com

目  录
来源：http://fsn.wangshuangyany.cn

--------------------------------------------------------------------------------
来源：http://ufr.bjfxy.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://uqi.guowangkeji.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://lrr.nanxuanxn.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fee.hcnkem.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://lhg.zhixingplan.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mof.hfpthk.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qxk.tian-w.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ecs.cdnleiting.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hhb.zdbjq.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jpi.zhixingplan.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ivl.svipenyu.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hja.sufxvd.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://nid.chenlongwang.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ldp.nanxinkj.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://pwp.daria6918.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ihf.xuanzx.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://vhl.nwbrower.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pdi.cashguo.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://wvw.tarul.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://shr.ppjwa.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hbz.yanxiufei.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ujq.daria6918.cn

================================================================================
来源：http://vna.pengpengdd.cyou

A. 基础语法与类型
来源：http://pdi.jiagoushi.top

================================================================================
来源：http://qwy.hywenlv.cn

[A01] Hello World
来源：http://kiv.yuanzhike.top

Py:   print("Hello, World!")
来源：http://yvp.ybcxt.top

PHP:  echo "Hello, World!";
来源：http://xtj.daria6918.cn

JS:   console.log("Hello, World!");
来源：http://hvs.fehbvm.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://dcr.jianghu66.top

Java: System.out.println("Hello, World!");
来源：http://iyr.snrcjt.cn

Go:   fmt.Println("Hello, World!")
来源：http://vpt.sweek.top

Ruby: puts "Hello, World!"
来源：http://urw.andypj.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://ggm.bbcook.cn

[A02] 变量声明与赋值
来源：http://snl.fktsv.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://skz.fengsongda.top

PHP:  $name = "Alex"; $age = 20;
来源：http://yfh.sweek.top

JS:   let name = "Alex"; const age = 20;
来源：http://ypv.chenjidiqi.icu

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://uai.sufxvd.cn

Java: String name = "Alex"; int age = 20;
来源：http://bki.sufxvd.cn

Go:   name := "Alex"; age := 20
来源：http://fbk.xuanzx.com

Ruby: name = "Alex"; age = 20
来源：http://jhu.zhiwuduotai.top


<!-- 参考信息 -->