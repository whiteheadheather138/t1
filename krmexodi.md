代发 wailian999

[U33] Py：打包发布
来源：http://gat.meibo888.top

python -m build  （依赖 pyproject.toml）
来源：http://nsr.tarul.cn

[U34] Py：判断编码
来源：http://vpc.9152youxi.cn

chardet.detect(raw)
来源：http://lty.aibaodan.cn

[U35] Py：发送邮件
来源：http://pjq.jianghu66.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pbe.xuetiantiany.cn

[U36] Py：定时任务
来源：http://tdm.shanyushiyangtech.top

schedule.every(10).minutes.do(job)
来源：http://jbr.guowangkeji.top

[U37] Py：读写 Excel
来源：http://xxl.sweek.top

pandas.read_excel / DataFrame.to_excel
来源：http://csk.zhijiandao.cn

[U38] Py：获取脚本所在目录
来源：http://wnh.havefunace.top

Path(__file__).resolve().parent
来源：http://rwa.mhx1999.top

[U39] Py：判断是否在交互环境
来源：http://aat.ywan-chungtsiang.top

sys.stdout.isatty()
来源：http://xep.birdmap.top

[U40] Py：打印到标准错误
来源：http://rsm.hysaishi.cn

print("err", file=sys.stderr)
来源：http://gdn.fehbvm.com

[U41] PHP：初始化 Composer 项目
来源：http://ndu.ppjwa.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://tfr.zhixingplan.top

[U42] PHP：PSR-4 自动加载
来源：http://ubj.zycfv.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://okq.daria6918.cn

[U43] PHP：声明命名空间
来源：http://mwv.guowangkeji.top

namespace App\Http;
来源：http://szs.yanxiufei.cn

[U44] PHP：开启严格类型
来源：http://ytx.fzhhl.top

declare(strict_types=1);
来源：http://uht.xziqi.cn

[U45] PHP：类型声明与返回类型
来源：http://vko.jiagoushi.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://oys.xylfe.cn

[U46] PHP：可空类型
来源：http://trw.andypj.xyz

?string $name = null
来源：http://fxc.cashguo.top

[U47] PHP：联合类型
来源：http://ugm.iojbl.cn

int|string $id
来源：http://qgr.bbcook.cn

[U48] PHP：纯枚举
来源：http://lfj.xziqi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hgo.xinyue.icu

[U49] PHP：只读属性
来源：http://opi.tanke756.top

public readonly string $name
来源：http://mtv.yanxiufei.cn

[U50] PHP：构造器属性提升
来源：http://jor.svipenyu.cn

public function __construct(private int $id) {}
来源：http://rad.jiagoushi.top

[U51] PHP：数组解构
来源：http://abb.andypj.xyz

[$a, $b] = $arr;
来源：http://vng.zdqjudy.top

[U52] PHP：箭头函数
来源：http://oni.xinyue.icu

$double = fn($x) => $x * 2;
来源：http://mok.yangfankeji.com

[U53] PHP：空合并运算符
来源：http://meo.uphjek.com

$v = $a ?? $b ?? "default";
来源：http://rrv.epnwcf.com

[U54] PHP：空安全调用
来源：http://ach.yuxming.cn

$obj?->method()
来源：http://onj.zhoulong.xyz

[U55] PHP：match 表达式
来源：http://zqg.quarkkingdee.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://drx.yj20258888.top

[U56] PHP：命名参数
来源：http://pac.zhijiandao.cn

f(a: 1, b: 2)
来源：http://pua.zhijiandao.cn

[U57] PHP：字符串插值
来源：http://kwn.shanyushiyangkeji.top

"值: {$a}"
来源：http://pip.ehwqpu.com

[U58] PHP：数组三件套
来源：http://his.ehwqpu.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://imx.havefunace.top

[U59] PHP：自定义排序
来源：http://uoz.feifeiyinyue.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rgy.yongpay.top

[U60] PHP：JSON 编解码
来源：http://ryd.tianlin.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://nqz.hammf.cn

[U61] PHP：正则
来源：http://hoe.xziqi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jsd.cdnleiting.top

[U62] PHP：日期对象
来源：http://cmj.xuetiantiany.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jjp.sweek.top

[U63] PHP：文件读写
来源：http://vtc.jlsjyb.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ybt.ivvv.top

[U64] PHP：目录遍历
来源：http://adc.yueranfly.top

glob("dir/*.php");  scandir("dir");
来源：http://mlp.0kj1m.cn

[U65] PHP：会话
来源：http://jgs.zdbjq.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://awy.quarkkingdee.top

[U66] PHP：设置 Cookie
来源：http://uxe.hongshengwenyu.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qll.hfpthk.cn

[U67] PHP：处理文件上传
来源：http://xjo.hongshengwenyu.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rwv.yangfankeji.com

[U68] PHP：PDO 连接
来源：http://wxg.zhoulong.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://oln.zycfv.cn

[U69] PHP：PDO 预处理
来源：http://dbd.ppjwa.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qmy.hnqzz.top

[U70] PHP：PDO 事务
来源：http://anu.ivvv.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bes.zhoulong.xyz

[U71] PHP：抛出异常
来源：http://bhl.iojbl.cn

throw new RuntimeException("失败", 500);
来源：http://jes.yj20258.top

[U72] PHP：写错误日志
来源：http://sxd.yangfankeji.com

error_log("失败: " . $e->getMessage());
来源：http://dbb.xuetiantiany.cn

[U73] PHP：读取 ini 配置
来源：http://zmm.sweek.top

parse_ini_file("config.ini", true)
来源：http://irp.guannengcc.top

[U74] PHP：读取环境变量
来源：http://fsc.jqgfzy.top

getenv("APP_ENV") ?: "production"
来源：http://vng.ybcxt.top

[U75] PHP：依赖注入
来源：http://gnv.xinyue.icu

composer require psr/container
来源：http://hmc.fzhhl.top

[U76] PHP：简单路由
来源：http://spl.redwolf501.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://axl.cheryme.top

[U77] PHP：模板渲染
来源：http://pjc.ybcxt.top

composer require twig/twig
来源：http://fdg.gaohongyu789.top

[U78] PHP：单元测试
来源：http://ckc.guannengcc.top

composer require --dev phpunit/phpunit
来源：http://zuj.xuetiantiany.cn

[U79] PHP：静态分析
来源：http://vba.mhx1999.top

composer require --dev phpstan/phpstan
来源：http://vzu.0kj1m.cn

[U80] PHP：代码规范修复
来源：http://zgs.zhiwuduotai.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://chg.andypj.xyz

[U81] JS：初始化项目
来源：http://xzv.yj202588.top

npm init -y;  npm i express
来源：http://zzs.gotoacloud.top

[U82] JS：package.json 脚本
来源：http://tcx.xinyue.icu

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://idp.pengpengdd.cyou

[U83] JS：ES Module 导入导出
来源：http://bpv.daria6918.cn

export const a = 1;  import { a } from "./m.js";
来源：http://nva.chenjidiqi.icu

[U84] JS：CommonJS 写法
来源：http://oyl.sjlbkw.cn

module.exports = { a };  const { a } = require("./m");
来源：http://mky.hnqzz.top

[U85] JS：可选链
来源：http://gyy.feifeiyinyue.top

a?.b?.c
来源：http://ady.haohaochexian.top

[U86] JS：空值合并
来源：http://nzm.dianchejie.cn

a ?? b
来源：http://ypv.c1oappe.top

[U87] JS：解构默认值
来源：http://myi.yuanzhike.top

const { a = 1, b = 2 } = obj;
来源：http://zrt.dianchejie.cn

[U88] JS：对象展开合并
来源：http://ujn.guannengcc.top

{ ...a, ...b }
来源：http://qql.shzxlz.cn

[U89] JS：数组去重
来源：http://feb.ydjk.org.cn

[...new Set(arr)]
来源：http://nhi.zhaomingkeji.xyz

[U90] JS：数字数组排序
来源：http://kon.aizwys.cn

[...arr].sort((a, b) => a - b)
来源：http://dds.xuanzx.com

[U91] JS：对象键值遍历
来源：http://epo.yfazqb.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hnn.cqqwz.cn

[U92] JS：深拷贝
来源：http://xky.chenzaomai.com

structuredClone(obj)
来源：http://cxz.svipenyu.cn

[U93] JS：模板字符串
来源：http://gww.kuanghao11.cn

`共 ${n} 条`
来源：http://umj.jinqigufen.top

[U94] JS：箭头函数
来源：http://eqk.nwbrower.top

const double = x => x * 2;
来源：http://sai.fengsongda.top

[U95] JS：Promise 包装
来源：http://fjh.jiagoushi.top

new Promise((resolve, reject) => {})
来源：http://mhq.yangfankeji.com

[U96] JS：async/await 与异常
来源：http://gkl.hywenlv.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fcy.yongpay.top

[U97] JS：并发请求
来源：http://wrm.316326.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://ipg.jinqigufen.top

[U98] JS：fetch 带 JSON
来源：http://fzy.daria6918.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nks.hnqzz.top

[U99] JS：事件监听
来源：http://ytq.aibaodan.cn

el.addEventListener("click", e => {})
来源：http://grd.fehbvm.com

[U100] JS：DOM 查询
来源：http://cdt.ybcxt.top

document.querySelector(".item")
来源：http://ovw.fzhhl.top

[U101] JS：classList 操作
来源：http://hay.xingfuxueyuan.xyz

el.classList.toggle("active")
来源：http://ykc.xylfe.cn

[U102] JS：本地存储
来源：http://cxc.guannengcc.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://tpy.shuidangran.top

[U103] JS：定时器
来源：http://yun.shuidangran.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ygg.tanke756.top

[U104] JS：防抖
来源：http://hvn.guowangkeji.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hum.hnqzz.top

[U105] JS：节流
来源：http://zqm.wangdashe.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mzs.jqgufenzy.top

[U106] JS：日期格式化
来源：http://ysl.xziqi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ztk.jianghu66.top

[U107] JS：数字千分位
来源：http://qdj.ydzc1.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nmb.zdbjq.cn

[U108] JS：随机整数
来源：http://lug.jyoumei.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wad.shuidangran.top

[U109] JS：数组分组
来源：http://muo.xinyue.icu

Object.groupBy(arr, x => x.type)
来源：http://nox.zhixingplan.top

[U110] JS：数组分块
来源：http://mno.sweek.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hap.hnqzz.top

[U111] JS：对象转 Map
来源：http://vnb.sjlbkw.cn

new Map(Object.entries(obj))
来源：http://mxf.ydjk.org.cn

[U112] JS：字符串补位
来源：http://twm.pycfn.com

"7".padStart(3, "0")
来源：http://lue.snrcjt.cn

[U113] JS：正则替换全部
来源：http://cwa.zhaomingkeji.xyz

s.replaceAll("a", "b")
来源：http://vkm.hywenlv.cn

[U114] JS：JSON 深比较
来源：http://mcs.aibaodan.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://nos.feifeiyinyue.top

[U115] JS：生成 UUID
来源：http://jgs.daxiang520.top

crypto.randomUUID()
来源：http://mxb.xziqi.cn

[U116] JS：类型检查（JSDoc）
来源：http://pmz.zhongyouzk.top

/** @param {string} name */ function f(name) {}
来源：http://fhk.shangyingyoupin.top

[U117] JS：单元测试
来源：http://uvr.shuidangran.top

npm i -D vitest;  npx vitest
来源：http://ttg.fktsv.cn

[U118] JS：开发服务器
来源：http://kpl.316326.xyz

npm i -D vite;  npx vite
来源：http://ovy.smart0.xyz

[U119] JS：生产构建
来源：http://cbm.tarul.cn

npx vite build
来源：http://jyj.sjlbkw.cn

[U120] JS：读取环境变量（Vite）
来源：http://xyp.birdmap.top

import.meta.env.VITE_API_URL
来源：http://whu.fanxiaobao.xyz

================================================================================
来源：http://qno.dianchejie.cn

统计汇总
来源：http://lxe.smart0.xyz

================================================================================
来源：http://loh.vehdjk.com

按语言统计（条）：
来源：http://aqf.yanxiufei.cn

Python ......... 252
来源：http://kag.meibo888.top

PHP ............ 252
来源：http://mvy.zhongyouzk.top

JavaScript ..... 252
来源：http://xkh.fengsongda.top

TypeScript ..... 212
来源：http://eey.jlsjyb.cn

Java ........... 212
来源：http://jfo.hnxiangtu.top

Go ............. 212
来源：http://oeh.hysaishi.cn

Ruby ........... 212
来源：http://vzc.yanxiufei.cn

C# ............. 212
来源：http://eju.birdmap.top

C .............. 30
来源：http://kwa.jianghu66.top

C++ ............ 30
来源：http://ggj.jyoumei.cn

SQL ............ 90
来源：http://npx.yangfankeji.com

Bash ........... 80
来源：http://vbe.sxryk.cn

Kotlin ......... 15
来源：http://zgq.hfpthk.cn

Swift .......... 15
来源：http://upx.yueranfly.top

Lua ............ 10
来源：http://yaj.birdmap.top

Perl ........... 10
来源：http://dxs.ehwqpu.com

Scala .......... 10
来源：http://nde.smart0.xyz

------------------------------------
来源：http://zkt.chenzaomai.com

合计 ........... 2106 条
来源：http://ejb.yueranfly.top

按章节统计：
来源：http://zuw.snrcjt.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jzu.chenzaomai.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mvw.fehbvm.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://biv.hongshengwenyu.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://buh.zhengqikj.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://txl.ppjwa.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://agg.bbcook.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://rih.52xcode.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tzn.zdbjq.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wsh.xuanzx.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yql.zhoulong.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://oto.wangshuangyany.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cgw.shanyushiyangtech.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://trs.c1oappe.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://lpt.cashguo.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wrp.shanyushiyangtech.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://gwo.daria6918.cn

Q SQL 专题                              90
来源：http://xeb.jlsjyb.cn

R Bash 专题                             80
来源：http://qoz.dashuyun.cn

S C / C++ 专题                          60
来源：http://wrn.hesvh.cn

T 其他语言补充                          60
来源：http://kyq.nanxuanxn.top

U 高频实用片段                         120
来源：http://kjg.zdqjudy.top

------------------------------------
来源：http://ixm.guannengcc.top

合计                                  2106 条
来源：http://nbe.sysykeji.top

--------------------------------------------------------------------------------
来源：http://yrm.c1oappe.top

使用提醒
来源：http://pkr.shzxlz.cn

--------------------------------------------------------------------------------
来源：http://myr.shzxlz.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://woz.zhiwuduotai.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://gkx.snrcjt.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://eee.ydjk.org.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://nkr.fzhhl.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bjz.hfpthk.cn

—— 文件结束 ——
来源：http://fjk.yvedp.cn

================================================================================
来源：http://xwf.ctjpmb.com

程序语言常见例子速查手册（2024 版）
来源：http://tvi.nwbrower.top

Common Programming Examples Cheat Book
来源：http://kei.zhoulong.xyz

================================================================================
来源：http://vwa.snrcjt.cn

【收录内容】
来源：http://kae.bbcook.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ypy.cdnleiting.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://yud.bbcook.cn

SQL · Bash · C · C++
来源：http://xsq.fzhhl.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://vxm.chenzaomai.com

【使用说明】
来源：http://xko.hnxiangtu.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mao.ybcxt.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qcz.vehdjk.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://xgo.yj202588.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://nvv.zdbjq.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://wid.yangfankeji.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://kgo.cdnleiting.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ldj.mhx1999.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://nhv.jiagoushi.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://bxp.hywenlv.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://zzr.mhx1999.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://cyi.yueranfly.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://cdu.daria6918.cn

【文件统计】
来源：http://szn.hnqzz.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ond.xziqi.cn

--------------------------------------------------------------------------------
来源：http://dyd.c1oappe.top

目  录
来源：http://yja.zhijiandao.cn

--------------------------------------------------------------------------------
来源：http://jeb.bjfxy.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://skc.fehbvm.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://isg.pengpengdd.cyou

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://glo.zhixingplan.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mmp.zhongyouzk.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://yjv.shanyushiyangkeji.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ydy.ppjwa.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://cfw.hnqzz.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ecy.jyoumei.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://eqg.daria6918.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://tzq.ywan-chungtsiang.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://gdw.sufxvd.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://moq.ybcxt.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://zxr.zhaomingkeji.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hoa.shzxlz.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://csu.hywenlv.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ahz.gzhubu.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://smm.aizwys.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://tvz.smart0.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://axz.tarul.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wvf.chenzaomai.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://vxm.jlsjyb.cn

================================================================================
来源：http://vva.hnqzz.top

A. 基础语法与类型
来源：http://ipt.zhengqikj.top

================================================================================
来源：http://mpm.pycfn.com

[A01] Hello World
来源：http://irx.ppjwa.cn

Py:   print("Hello, World!")
来源：http://gag.guannengcc.top

PHP:  echo "Hello, World!";
来源：http://kzx.zycfv.cn

JS:   console.log("Hello, World!");
来源：http://qck.zdqjudy.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ypm.quarkkingdee.top

Java: System.out.println("Hello, World!");
来源：http://cho.cucudq.cn

Go:   fmt.Println("Hello, World!")
来源：http://uwn.ctjpmb.com

Ruby: puts "Hello, World!"
来源：http://vmf.sweek.top

C#:   Console.WriteLine("Hello, World!");
来源：http://aew.gzhubu.top

[A02] 变量声明与赋值
来源：http://oof.xziqi.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wqd.gotoacloud.top

PHP:  $name = "Alex"; $age = 20;
来源：http://kol.ydzc1.top

JS:   let name = "Alex"; const age = 20;
来源：http://jxd.yueranfly.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vkl.smart0.xyz

Java: String name = "Alex"; int age = 20;
来源：http://qnh.sweek.top

Go:   name := "Alex"; age := 20
来源：http://dwx.jinghuilouyu.cn

Ruby: name = "Alex"; age = 20
来源：http://slj.feifeiyinyue.top


<!-- 参考信息 -->