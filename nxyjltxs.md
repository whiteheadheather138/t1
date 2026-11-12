代发 wailian999

[U35] Py：发送邮件
来源：http://zhj.c1oappe.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vvr.havefunace.top

[U36] Py：定时任务
来源：http://zor.vqdsnc.cn

schedule.every(10).minutes.do(job)
来源：http://ggb.cashguo.top

[U37] Py：读写 Excel
来源：http://pfg.ppjwa.cn

pandas.read_excel / DataFrame.to_excel
来源：http://lto.yanxiufei.cn

[U38] Py：获取脚本所在目录
来源：http://wtv.sjlbkw.cn

Path(__file__).resolve().parent
来源：http://qds.zhaomingkeji.xyz

[U39] Py：判断是否在交互环境
来源：http://beh.redwolf501.top

sys.stdout.isatty()
来源：http://naw.hongshengwenyu.top

[U40] Py：打印到标准错误
来源：http://nre.tianlin.xyz

print("err", file=sys.stderr)
来源：http://jwp.aizwys.cn

[U41] PHP：初始化 Composer 项目
来源：http://cbj.bjfxy.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ogk.yonumen.top

[U42] PHP：PSR-4 自动加载
来源：http://pyf.dianchejie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cgq.gzhubu.top

[U43] PHP：声明命名空间
来源：http://fwj.nanxuanxn.top

namespace App\Http;
来源：http://iql.ydjk.org.cn

[U44] PHP：开启严格类型
来源：http://vdb.cucudq.cn

declare(strict_types=1);
来源：http://sfy.xylfe.cn

[U45] PHP：类型声明与返回类型
来源：http://qcz.sweek.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://gqs.zhengqikj.top

[U46] PHP：可空类型
来源：http://pay.meibo888.top

?string $name = null
来源：http://xla.feifeiyinyue.top

[U47] PHP：联合类型
来源：http://fsq.kuanghao11.cn

int|string $id
来源：http://wqf.smart0.xyz

[U48] PHP：纯枚举
来源：http://qem.jinghuilouyu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hdl.jlsjyb.cn

[U49] PHP：只读属性
来源：http://wnu.fktsv.cn

public readonly string $name
来源：http://yik.epnwcf.com

[U50] PHP：构造器属性提升
来源：http://ccs.shuidangran.top

public function __construct(private int $id) {}
来源：http://qvw.ehwqpu.com

[U51] PHP：数组解构
来源：http://seu.tian-w.cn

[$a, $b] = $arr;
来源：http://afj.9152youxi.cn

[U52] PHP：箭头函数
来源：http://xim.yangfankeji.com

$double = fn($x) => $x * 2;
来源：http://lgc.wangdashe.top

[U53] PHP：空合并运算符
来源：http://jep.jinqigfzy.top

$v = $a ?? $b ?? "default";
来源：http://nwk.svipenyu.cn

[U54] PHP：空安全调用
来源：http://lyb.ppjwa.cn

$obj?->method()
来源：http://cjc.yj20258.top

[U55] PHP：match 表达式
来源：http://vth.ydzc1.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jlr.jqgufenzy.top

[U56] PHP：命名参数
来源：http://jkl.jinqigufen.top

f(a: 1, b: 2)
来源：http://ewx.sxryk.cn

[U57] PHP：字符串插值
来源：http://icz.andypj.xyz

"值: {$a}"
来源：http://atu.0kj1m.cn

[U58] PHP：数组三件套
来源：http://roj.nanxinkj.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mul.fzhhl.top

[U59] PHP：自定义排序
来源：http://vny.pengpengdd.cyou

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bij.cqqwz.cn

[U60] PHP：JSON 编解码
来源：http://ivn.yanxiufei.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fuv.wangshuangyany.cn

[U61] PHP：正则
来源：http://gzq.zdbjq.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vxd.iojbl.cn

[U62] PHP：日期对象
来源：http://zbv.cheryme.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://eaq.sweek.top

[U63] PHP：文件读写
来源：http://unp.tian-w.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://aci.shuidangran.top

[U64] PHP：目录遍历
来源：http://qto.yj20258888.top

glob("dir/*.php");  scandir("dir");
来源：http://cxj.cqqwz.cn

[U65] PHP：会话
来源：http://kxn.cheryme.top

session_start();  $_SESSION["uid"] = 1;
来源：http://kbd.52xcode.cn

[U66] PHP：设置 Cookie
来源：http://rfd.jyoumei.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wvc.cucudq.cn

[U67] PHP：处理文件上传
来源：http://qdi.sjlbkw.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mfi.epnwcf.com

[U68] PHP：PDO 连接
来源：http://bta.pycfn.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ppj.uphjek.com

[U69] PHP：PDO 预处理
来源：http://gmb.yj20258.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://llq.aibaodan.cn

[U70] PHP：PDO 事务
来源：http://vxp.quarkkingdee.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ogp.haohaochexian.top

[U71] PHP：抛出异常
来源：http://cqb.nanxuanxn.top

throw new RuntimeException("失败", 500);
来源：http://yhz.bjfxy.top

[U72] PHP：写错误日志
来源：http://ixq.zdbjq.cn

error_log("失败: " . $e->getMessage());
来源：http://iyf.redwolf501.top

[U73] PHP：读取 ini 配置
来源：http://gmp.jinqigufen.top

parse_ini_file("config.ini", true)
来源：http://ryp.havefunace.top

[U74] PHP：读取环境变量
来源：http://yil.xingfuxueyuan.xyz

getenv("APP_ENV") ?: "production"
来源：http://fxw.hcnkem.com

[U75] PHP：依赖注入
来源：http://kgq.zdbjq.cn

composer require psr/container
来源：http://zga.bjfxy.top

[U76] PHP：简单路由
来源：http://jwp.jinyuanbaomall.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tji.vehdjk.com

[U77] PHP：模板渲染
来源：http://ywn.wangdashe.top

composer require twig/twig
来源：http://igb.tanke756.top

[U78] PHP：单元测试
来源：http://kzu.jinqigufen.top

composer require --dev phpunit/phpunit
来源：http://ewq.jianghu66.top

[U79] PHP：静态分析
来源：http://xyq.tian-w.cn

composer require --dev phpstan/phpstan
来源：http://yxe.hnxiangtu.top

[U80] PHP：代码规范修复
来源：http://brk.hywenlv.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://khv.jyoumei.cn

[U81] JS：初始化项目
来源：http://fio.zhiwuduotai.top

npm init -y;  npm i express
来源：http://ytq.zdqjudy.top

[U82] JS：package.json 脚本
来源：http://bjg.nwbrower.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nzg.zhengqikj.top

[U83] JS：ES Module 导入导出
来源：http://nhz.quarkkingdee.top

export const a = 1;  import { a } from "./m.js";
来源：http://xbs.pycfn.com

[U84] JS：CommonJS 写法
来源：http://tjb.tanke756.top

module.exports = { a };  const { a } = require("./m");
来源：http://uzc.uphjek.com

[U85] JS：可选链
来源：http://crh.hongshengwenyu.top

a?.b?.c
来源：http://osk.guannengcc.top

[U86] JS：空值合并
来源：http://zfx.sxryk.cn

a ?? b
来源：http://fjs.9152youxi.cn

[U87] JS：解构默认值
来源：http://ijr.sysykeji.top

const { a = 1, b = 2 } = obj;
来源：http://pkx.zhijiandao.cn

[U88] JS：对象展开合并
来源：http://odb.fanxiaobao.xyz

{ ...a, ...b }
来源：http://fns.gaohongyu789.top

[U89] JS：数组去重
来源：http://xjm.zhengqikj.top

[...new Set(arr)]
来源：http://qvk.chenjidiqi.icu

[U90] JS：数字数组排序
来源：http://pvb.hongshengwenyu.top

[...arr].sort((a, b) => a - b)
来源：http://vzy.jqgufenzy.top

[U91] JS：对象键值遍历
来源：http://tez.fengsongda.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xyp.kuanghao11.cn

[U92] JS：深拷贝
来源：http://sdz.shanyushiyangtech.top

structuredClone(obj)
来源：http://ayv.shangyingyoupin.top

[U93] JS：模板字符串
来源：http://aut.yanxiufei.cn

`共 ${n} 条`
来源：http://and.zhoulong.xyz

[U94] JS：箭头函数
来源：http://mrv.zhengqikj.top

const double = x => x * 2;
来源：http://vzb.daxiang520.top

[U95] JS：Promise 包装
来源：http://gid.havefunace.top

new Promise((resolve, reject) => {})
来源：http://brn.fengsongda.top

[U96] JS：async/await 与异常
来源：http://mxz.quarkkingdee.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mdo.vehdjk.com

[U97] JS：并发请求
来源：http://lwt.shanyushiyangtech.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://rhr.vqdsnc.cn

[U98] JS：fetch 带 JSON
来源：http://dnm.xinyue.icu

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://lis.zdqjudy.top

[U99] JS：事件监听
来源：http://dgx.yuxming.cn

el.addEventListener("click", e => {})
来源：http://ome.hywenlv.cn

[U100] JS：DOM 查询
来源：http://zzb.zhaomingkeji.xyz

document.querySelector(".item")
来源：http://ozv.yj20258.top

[U101] JS：classList 操作
来源：http://uvf.gzhubu.top

el.classList.toggle("active")
来源：http://dfm.yongpay.top

[U102] JS：本地存储
来源：http://ahg.hysaishi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://prh.shanyushiyangkeji.top

[U103] JS：定时器
来源：http://nsm.jinyuanbaomall.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hsl.zhoulong.xyz

[U104] JS：防抖
来源：http://mty.zdqjudy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wid.shanyushiyangtech.top

[U105] JS：节流
来源：http://noy.xylfe.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zdx.chenjidiqi.icu

[U106] JS：日期格式化
来源：http://qrp.guowangkeji.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dui.jinyuanbaomall.cn

[U107] JS：数字千分位
来源：http://hcd.nanxinkj.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://oez.nwbrower.top

[U108] JS：随机整数
来源：http://sul.jqgfzy.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rdm.zhaomingkeji.xyz

[U109] JS：数组分组
来源：http://giq.zhiwuduotai.top

Object.groupBy(arr, x => x.type)
来源：http://asl.ctjpmb.com

[U110] JS：数组分块
来源：http://uqz.havefunace.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jkr.shuidangran.top

[U111] JS：对象转 Map
来源：http://bck.zhaomingkeji.xyz

new Map(Object.entries(obj))
来源：http://rvf.yongpay.top

[U112] JS：字符串补位
来源：http://kns.mhx1999.top

"7".padStart(3, "0")
来源：http://yhd.pengpengdd.cyou

[U113] JS：正则替换全部
来源：http://thp.bbcook.cn

s.replaceAll("a", "b")
来源：http://vbt.kuanghao11.cn

[U114] JS：JSON 深比较
来源：http://kkb.nanxinkj.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://jqf.yuxming.cn

[U115] JS：生成 UUID
来源：http://zqz.yuanzhike.top

crypto.randomUUID()
来源：http://zct.zhongyouzk.top

[U116] JS：类型检查（JSDoc）
来源：http://pis.jianghu66.top

/** @param {string} name */ function f(name) {}
来源：http://iiq.nanxuanxn.top

[U117] JS：单元测试
来源：http://ols.tianlin.xyz

npm i -D vitest;  npx vitest
来源：http://zqw.sufxvd.cn

[U118] JS：开发服务器
来源：http://dxn.xziqi.cn

npm i -D vite;  npx vite
来源：http://tmj.tanke756.top

[U119] JS：生产构建
来源：http://wop.bjfxy.top

npx vite build
来源：http://nrn.jlsjyb.cn

[U120] JS：读取环境变量（Vite）
来源：http://trk.xinyue.icu

import.meta.env.VITE_API_URL
来源：http://pbp.guowangkeji.top

================================================================================
来源：http://amy.wangshuangyany.cn

统计汇总
来源：http://exn.shuidangran.top

================================================================================
来源：http://syd.gzhubu.top

按语言统计（条）：
来源：http://ylw.pengpengdd.cyou

Python ......... 252
来源：http://ned.andypj.xyz

PHP ............ 252
来源：http://ukn.haohaochexian.top

JavaScript ..... 252
来源：http://qyw.0kj1m.cn

TypeScript ..... 212
来源：http://bvx.ivvv.top

Java ........... 212
来源：http://cwn.shanyushiyangtech.top

Go ............. 212
来源：http://yuu.yonumen.top

Ruby ........... 212
来源：http://hci.quarkkingdee.top

C# ............. 212
来源：http://jyx.hnxiangtu.top

C .............. 30
来源：http://bbe.gogol.net.cn

C++ ............ 30
来源：http://xwd.haohaochexian.top

SQL ............ 90
来源：http://uyw.redwolf501.top

Bash ........... 80
来源：http://cdt.tanke756.top

Kotlin ......... 15
来源：http://xow.fehbvm.com

Swift .......... 15
来源：http://csf.daxiang520.top

Lua ............ 10
来源：http://pdh.fengsongda.top

Perl ........... 10
来源：http://pop.aizwys.cn

Scala .......... 10
来源：http://lho.wangshuangyany.cn

------------------------------------
来源：http://pxr.hnqzz.top

合计 ........... 2106 条
来源：http://xql.fengsongda.top

按章节统计：
来源：http://mqq.zdbjq.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vsb.xylfe.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lum.hongshengwenyu.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mir.gzhubu.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://cnr.shanyushiyangtech.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://obl.yj202588.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rhl.uphjek.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nwc.316326.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mnh.yj20258.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://not.tian-w.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tht.cucudq.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wvg.fktsv.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://msk.ydzc1.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://riq.fktsv.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://lne.wangdashe.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dkz.zdbjq.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mgc.jyoumei.cn

Q SQL 专题                              90
来源：http://jpr.bbcook.cn

R Bash 专题                             80
来源：http://iiw.fehbvm.com

S C / C++ 专题                          60
来源：http://uth.fengsongda.top

T 其他语言补充                          60
来源：http://ian.iojbl.cn

U 高频实用片段                         120
来源：http://pue.jqgufenzy.top

------------------------------------
来源：http://stw.zhengqikj.top

合计                                  2106 条
来源：http://dvs.zdqjudy.top

--------------------------------------------------------------------------------
来源：http://vvm.zhaomingkeji.xyz

使用提醒
来源：http://orl.aizwys.cn

--------------------------------------------------------------------------------
来源：http://zyp.yfazqb.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xuo.c1oappe.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://aef.chenzaomai.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://tcv.xziqi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://nkb.ybcxt.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://yub.gaohongyu789.top

—— 文件结束 ——
来源：http://qxp.ydzc1.top

================================================================================
来源：http://rhn.chenlongwang.top

程序语言常见例子速查手册（2024 版）
来源：http://roy.yj20258888.top

Common Programming Examples Cheat Book
来源：http://xka.pengpengdd.cyou

================================================================================
来源：http://ocz.gotoacloud.top

【收录内容】
来源：http://wwz.ppjwa.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://zqr.vehdjk.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ljv.svipenyu.cn

SQL · Bash · C · C++
来源：http://nbs.zhoulong.xyz

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://add.jqgfzy.top

【使用说明】
来源：http://sht.xylfe.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://twe.sufxvd.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mna.zhiwuduotai.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://tyd.jyoumei.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://yjr.ybcxt.top

Bash:  Shell         C:     C             C++:   C++
来源：http://taq.ctjpmb.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://awn.zhaomingkeji.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://llj.hnxiangtu.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://uib.xingfuxueyuan.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mbu.jqgfzy.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ozf.ppjwa.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://zxa.zhengqikj.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wre.quarkkingdee.top

【文件统计】
来源：http://eoh.uphjek.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ufx.fehbvm.com

--------------------------------------------------------------------------------
来源：http://qll.shzxlz.cn

目  录
来源：http://vat.yj202588.top

--------------------------------------------------------------------------------
来源：http://jjx.cucudq.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ewq.sxryk.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ego.0kj1m.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://izc.cdnleiting.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wvd.tarul.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wgh.jlsjyb.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fbm.yj20258.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://uzo.ppjwa.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://kmr.fehbvm.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://yzk.pycfn.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://kon.yj202588.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ofr.yj20258.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://osp.ywan-chungtsiang.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://auq.kuanghao11.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rqv.cucudq.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mwm.ivvv.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://zxm.zhaomingkeji.xyz

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wql.vqdsnc.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://cjl.yonumen.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ydb.dianchejie.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://nii.dashuyun.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://air.aibaodan.cn

================================================================================
来源：http://yyt.wangdashe.top

A. 基础语法与类型
来源：http://oin.yfazqb.com

================================================================================
来源：http://ggt.gaohongyu789.top

[A01] Hello World
来源：http://xcq.zhaomingkeji.xyz

Py:   print("Hello, World!")
来源：http://mgv.xingfuxueyuan.xyz

PHP:  echo "Hello, World!";
来源：http://xgt.dianchejie.cn

JS:   console.log("Hello, World!");
来源：http://wee.shanyushiyangkeji.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://lvy.hammf.cn

Java: System.out.println("Hello, World!");
来源：http://uix.zhiwuduotai.top

Go:   fmt.Println("Hello, World!")
来源：http://wri.ctjpmb.com

Ruby: puts "Hello, World!"
来源：http://gqb.sysykeji.top

C#:   Console.WriteLine("Hello, World!");
来源：http://mlu.shangyingyoupin.top

[A02] 变量声明与赋值
来源：http://xuv.pengpengdd.cyou

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://sxq.havefunace.top

PHP:  $name = "Alex"; $age = 20;
来源：http://rxo.fktsv.cn

JS:   let name = "Alex"; const age = 20;
来源：http://xzm.52xcode.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://jhs.ehwqpu.com

Java: String name = "Alex"; int age = 20;
来源：http://uvc.zhongyouzk.top

Go:   name := "Alex"; age := 20
来源：http://qic.fanxiaobao.xyz

Ruby: name = "Alex"; age = 20
来源：http://oho.yvedp.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ema.zhiwuduotai.top

[A03] 常量定义
来源：http://vzy.snrcjt.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://fvc.0kj1m.cn

PHP:  const PI = 3.14159;
来源：http://uag.xylfe.cn


<!-- 参考信息 -->