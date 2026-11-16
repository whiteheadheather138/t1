代发 wailian999

[U31] Py：单测
来源：http://okv.yj20258.top

python -m pytest -q
来源：http://zwd.gaohongyu789.top

[U32] Py：代码格式化
来源：http://aks.yj20258.top

ruff format . && ruff check --fix .
来源：http://ico.chenlongwang.top

[U33] Py：打包发布
来源：http://mwl.ydjk.org.cn

python -m build  （依赖 pyproject.toml）
来源：http://gov.tian-w.cn

[U34] Py：判断编码
来源：http://tls.xingfuxueyuan.xyz

chardet.detect(raw)
来源：http://cng.daxiang520.top

[U35] Py：发送邮件
来源：http://rop.tarul.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://eqi.gzhubu.top

[U36] Py：定时任务
来源：http://eke.jinqigufen.top

schedule.every(10).minutes.do(job)
来源：http://afd.yongpay.top

[U37] Py：读写 Excel
来源：http://des.cashguo.top

pandas.read_excel / DataFrame.to_excel
来源：http://enx.ydjk.org.cn

[U38] Py：获取脚本所在目录
来源：http://mgk.c1oappe.top

Path(__file__).resolve().parent
来源：http://mra.yfazqb.com

[U39] Py：判断是否在交互环境
来源：http://tor.epnwcf.com

sys.stdout.isatty()
来源：http://xgc.zhoulong.xyz

[U40] Py：打印到标准错误
来源：http://kqt.tanke756.top

print("err", file=sys.stderr)
来源：http://nae.xinyue.icu

[U41] PHP：初始化 Composer 项目
来源：http://own.zhixingplan.top

composer init;  composer require guzzlehttp/guzzle
来源：http://tkp.jqgfzy.top

[U42] PHP：PSR-4 自动加载
来源：http://cze.hongshengwenyu.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hhl.fanxiaobao.xyz

[U43] PHP：声明命名空间
来源：http://cyd.ywan-chungtsiang.top

namespace App\Http;
来源：http://oek.shuidangran.top

[U44] PHP：开启严格类型
来源：http://eax.sjlbkw.cn

declare(strict_types=1);
来源：http://pto.bjfxy.top

[U45] PHP：类型声明与返回类型
来源：http://msf.hongshengwenyu.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://tee.havefunace.top

[U46] PHP：可空类型
来源：http://vis.jinqigfzy.top

?string $name = null
来源：http://dxs.hywenlv.cn

[U47] PHP：联合类型
来源：http://jll.ydzc1.top

int|string $id
来源：http://rcr.pengpengdd.cyou

[U48] PHP：纯枚举
来源：http://gbk.316326.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://iec.yanxiufei.cn

[U49] PHP：只读属性
来源：http://gbm.ppjwa.cn

public readonly string $name
来源：http://akl.meibo888.top

[U50] PHP：构造器属性提升
来源：http://cvf.yuxming.cn

public function __construct(private int $id) {}
来源：http://kzs.pengpengdd.cyou

[U51] PHP：数组解构
来源：http://ooe.dianchejie.cn

[$a, $b] = $arr;
来源：http://euk.hammf.cn

[U52] PHP：箭头函数
来源：http://obe.chenzaomai.com

$double = fn($x) => $x * 2;
来源：http://dva.snrcjt.cn

[U53] PHP：空合并运算符
来源：http://fia.yueranfly.top

$v = $a ?? $b ?? "default";
来源：http://gqx.uphjek.com

[U54] PHP：空安全调用
来源：http://taj.shanyushiyangkeji.top

$obj?->method()
来源：http://prp.uphjek.com

[U55] PHP：match 表达式
来源：http://dvu.tarul.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://plz.zhijiandao.cn

[U56] PHP：命名参数
来源：http://ygm.sjlbkw.cn

f(a: 1, b: 2)
来源：http://zqe.hesvh.cn

[U57] PHP：字符串插值
来源：http://bel.ywan-chungtsiang.top

"值: {$a}"
来源：http://tjk.epnwcf.com

[U58] PHP：数组三件套
来源：http://ecb.shuidangran.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fmt.yvedp.cn

[U59] PHP：自定义排序
来源：http://xsl.xziqi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ehr.sysykeji.top

[U60] PHP：JSON 编解码
来源：http://eec.dianchejie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://sca.hfpthk.cn

[U61] PHP：正则
来源：http://xci.yuanzhike.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://whh.fehbvm.com

[U62] PHP：日期对象
来源：http://rbt.shuidangran.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ibi.sxryk.cn

[U63] PHP：文件读写
来源：http://xof.pycfn.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ubh.svipenyu.cn

[U64] PHP：目录遍历
来源：http://tmj.ywan-chungtsiang.top

glob("dir/*.php");  scandir("dir");
来源：http://xnk.fktsv.cn

[U65] PHP：会话
来源：http://eww.zhaomingkeji.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://hkt.cashguo.top

[U66] PHP：设置 Cookie
来源：http://tdw.redwolf501.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kkg.hywenlv.cn

[U67] PHP：处理文件上传
来源：http://mlw.9152youxi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://uzg.sxryk.cn

[U68] PHP：PDO 连接
来源：http://pyp.svipenyu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://amr.yuxming.cn

[U69] PHP：PDO 预处理
来源：http://vsu.tianlin.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ion.52xcode.cn

[U70] PHP：PDO 事务
来源：http://yyj.xylfe.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hde.xinyue.icu

[U71] PHP：抛出异常
来源：http://onm.xinyue.icu

throw new RuntimeException("失败", 500);
来源：http://bnj.yj20258.top

[U72] PHP：写错误日志
来源：http://xzl.yangfankeji.com

error_log("失败: " . $e->getMessage());
来源：http://hwz.zhixingplan.top

[U73] PHP：读取 ini 配置
来源：http://meh.yj20258888.top

parse_ini_file("config.ini", true)
来源：http://ksf.jlsjyb.cn

[U74] PHP：读取环境变量
来源：http://vdk.havefunace.top

getenv("APP_ENV") ?: "production"
来源：http://gkw.aizwys.cn

[U75] PHP：依赖注入
来源：http://qnp.birdmap.top

composer require psr/container
来源：http://xie.yj20258888.top

[U76] PHP：简单路由
来源：http://pcu.tarul.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zen.ywan-chungtsiang.top

[U77] PHP：模板渲染
来源：http://kee.wangshuangyany.cn

composer require twig/twig
来源：http://hct.nwbrower.top

[U78] PHP：单元测试
来源：http://xhi.yongpay.top

composer require --dev phpunit/phpunit
来源：http://snm.cashguo.top

[U79] PHP：静态分析
来源：http://mqc.nanxinkj.top

composer require --dev phpstan/phpstan
来源：http://afo.guowangkeji.top

[U80] PHP：代码规范修复
来源：http://efd.yvedp.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://nuy.shangyingyoupin.top

[U81] JS：初始化项目
来源：http://gaw.52xcode.cn

npm init -y;  npm i express
来源：http://fag.cheryme.top

[U82] JS：package.json 脚本
来源：http://ire.cqqwz.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vtu.ehwqpu.com

[U83] JS：ES Module 导入导出
来源：http://gnn.ctjpmb.com

export const a = 1;  import { a } from "./m.js";
来源：http://fsa.yonumen.top

[U84] JS：CommonJS 写法
来源：http://khw.fktsv.cn

module.exports = { a };  const { a } = require("./m");
来源：http://pjt.xylfe.cn

[U85] JS：可选链
来源：http://fjt.shanyushiyangkeji.top

a?.b?.c
来源：http://yft.vqdsnc.cn

[U86] JS：空值合并
来源：http://qah.52xcode.cn

a ?? b
来源：http://rbr.gogol.net.cn

[U87] JS：解构默认值
来源：http://oia.hywenlv.cn

const { a = 1, b = 2 } = obj;
来源：http://uxi.haohaochexian.top

[U88] JS：对象展开合并
来源：http://vqz.sweek.top

{ ...a, ...b }
来源：http://edb.guannengcc.top

[U89] JS：数组去重
来源：http://eqz.sufxvd.cn

[...new Set(arr)]
来源：http://ott.zycfv.cn

[U90] JS：数字数组排序
来源：http://war.dianchejie.cn

[...arr].sort((a, b) => a - b)
来源：http://abf.yuxming.cn

[U91] JS：对象键值遍历
来源：http://sia.zhoulong.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://omq.fzhhl.top

[U92] JS：深拷贝
来源：http://ywm.shanyushiyangtech.top

structuredClone(obj)
来源：http://tfh.andypj.xyz

[U93] JS：模板字符串
来源：http://jzd.birdmap.top

`共 ${n} 条`
来源：http://anh.quarkkingdee.top

[U94] JS：箭头函数
来源：http://ktj.zdqjudy.top

const double = x => x * 2;
来源：http://frw.xinyue.icu

[U95] JS：Promise 包装
来源：http://jsd.iojbl.cn

new Promise((resolve, reject) => {})
来源：http://qhh.zhijiandao.cn

[U96] JS：async/await 与异常
来源：http://qfm.shzxlz.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://kwo.bbcook.cn

[U97] JS：并发请求
来源：http://ecr.iojbl.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://vhg.dianchejie.cn

[U98] JS：fetch 带 JSON
来源：http://wme.zhijiandao.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://elz.hesvh.cn

[U99] JS：事件监听
来源：http://thp.ctjpmb.com

el.addEventListener("click", e => {})
来源：http://hqo.ivvv.top

[U100] JS：DOM 查询
来源：http://piq.ivvv.top

document.querySelector(".item")
来源：http://fcx.c1oappe.top

[U101] JS：classList 操作
来源：http://gdv.jinyuanbaomall.cn

el.classList.toggle("active")
来源：http://mze.quarkkingdee.top

[U102] JS：本地存储
来源：http://fom.0kj1m.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://dxq.ywan-chungtsiang.top

[U103] JS：定时器
来源：http://tnb.meibo888.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://izi.zhoulong.xyz

[U104] JS：防抖
来源：http://jri.shanyushiyangkeji.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jiz.fehbvm.com

[U105] JS：节流
来源：http://cqg.cdnleiting.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://tld.ivvv.top

[U106] JS：日期格式化
来源：http://smo.yfazqb.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wwr.mhx1999.top

[U107] JS：数字千分位
来源：http://nyk.chenjidiqi.icu

new Intl.NumberFormat("en-US").format(1234567)
来源：http://dxi.shzxlz.cn

[U108] JS：随机整数
来源：http://euf.nanxinkj.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://uot.52xcode.cn

[U109] JS：数组分组
来源：http://mnv.ehwqpu.com

Object.groupBy(arr, x => x.type)
来源：http://sfu.zycfv.cn

[U110] JS：数组分块
来源：http://ytj.tian-w.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gim.fanxiaobao.xyz

[U111] JS：对象转 Map
来源：http://iec.fengsongda.top

new Map(Object.entries(obj))
来源：http://kzn.yuanzhike.top

[U112] JS：字符串补位
来源：http://adt.ydjk.org.cn

"7".padStart(3, "0")
来源：http://ggr.ydjk.org.cn

[U113] JS：正则替换全部
来源：http://ope.sysykeji.top

s.replaceAll("a", "b")
来源：http://hix.epnwcf.com

[U114] JS：JSON 深比较
来源：http://otb.mhx1999.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://voc.sufxvd.cn

[U115] JS：生成 UUID
来源：http://qsv.nanxinkj.top

crypto.randomUUID()
来源：http://vrk.cheryme.top

[U116] JS：类型检查（JSDoc）
来源：http://env.fanxiaobao.xyz

/** @param {string} name */ function f(name) {}
来源：http://bgr.ybcxt.top

[U117] JS：单元测试
来源：http://qms.yangfankeji.com

npm i -D vitest;  npx vitest
来源：http://pdy.zycfv.cn

[U118] JS：开发服务器
来源：http://irm.ybcxt.top

npm i -D vite;  npx vite
来源：http://cpp.yj20258.top

[U119] JS：生产构建
来源：http://itd.zdbjq.cn

npx vite build
来源：http://pec.guowangkeji.top

[U120] JS：读取环境变量（Vite）
来源：http://nvy.gogol.net.cn

import.meta.env.VITE_API_URL
来源：http://lqi.hnqzz.top

================================================================================
来源：http://bcw.shzxlz.cn

统计汇总
来源：http://eui.hnxiangtu.top

================================================================================
来源：http://gud.daxiang520.top

按语言统计（条）：
来源：http://wpl.fktsv.cn

Python ......... 252
来源：http://dyc.ydzc1.top

PHP ............ 252
来源：http://sov.sysykeji.top

JavaScript ..... 252
来源：http://pgx.yfazqb.com

TypeScript ..... 212
来源：http://ucy.shzxlz.cn

Java ........... 212
来源：http://zfb.sweek.top

Go ............. 212
来源：http://vsa.fengsongda.top

Ruby ........... 212
来源：http://gvf.tanke756.top

C# ............. 212
来源：http://aie.zdbjq.cn

C .............. 30
来源：http://mcb.bjfxy.top

C++ ............ 30
来源：http://sen.smart0.xyz

SQL ............ 90
来源：http://qrq.jyoumei.cn

Bash ........... 80
来源：http://cut.jyoumei.cn

Kotlin ......... 15
来源：http://cnc.kuanghao11.cn

Swift .......... 15
来源：http://tqq.ctjpmb.com

Lua ............ 10
来源：http://naa.shuidangran.top

Perl ........... 10
来源：http://emk.shzxlz.cn

Scala .......... 10
来源：http://jyq.kuanghao11.cn

------------------------------------
来源：http://hxa.cucudq.cn

合计 ........... 2106 条
来源：http://glh.ivvv.top

按章节统计：
来源：http://hda.zhijiandao.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wex.hywenlv.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gmx.gogol.net.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://sdt.ivvv.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://nyh.svipenyu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://lyj.yfazqb.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://iab.hnqzz.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zrw.hysaishi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xfm.xylfe.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://isw.zhengqikj.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wvb.xuetiantiany.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://krn.xinyue.icu

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hiw.tanke756.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://egi.cucudq.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tfw.xziqi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://llf.pengpengdd.cyou

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://nww.bjfxy.top

Q SQL 专题                              90
来源：http://gmx.meibo888.top

R Bash 专题                             80
来源：http://rkv.guowangkeji.top

S C / C++ 专题                          60
来源：http://cdf.chenlongwang.top

T 其他语言补充                          60
来源：http://kvo.zhijiandao.cn

U 高频实用片段                         120
来源：http://xnz.jinyuanbaomall.cn

------------------------------------
来源：http://tov.pycfn.com

合计                                  2106 条
来源：http://djm.jiagoushi.top

--------------------------------------------------------------------------------
来源：http://vgw.sxryk.cn

使用提醒
来源：http://sza.yj202588.top

--------------------------------------------------------------------------------
来源：http://jjn.jlsjyb.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ifq.nanxuanxn.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://nvi.sxryk.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://trg.yanxiufei.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://cwx.sjlbkw.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://lbi.sjlbkw.cn

—— 文件结束 ——
来源：http://qdb.yfazqb.com

================================================================================
来源：http://koj.fanxiaobao.xyz

程序语言常见例子速查手册（2024 版）
来源：http://mmk.yuanzhike.top

Common Programming Examples Cheat Book
来源：http://kif.zdbjq.cn

================================================================================
来源：http://yef.sysykeji.top

【收录内容】
来源：http://fio.nwbrower.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://pok.cheryme.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wgb.sysykeji.top

SQL · Bash · C · C++
来源：http://kcj.guowangkeji.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://tpm.nanxuanxn.top

【使用说明】
来源：http://mzt.wangshuangyany.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wux.feifeiyinyue.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ghz.hesvh.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pxo.cashguo.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qoo.gotoacloud.top

Bash:  Shell         C:     C             C++:   C++
来源：http://hsj.jqgufenzy.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://bwg.havefunace.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://dek.sweek.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://yin.meibo888.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wxd.xinyue.icu

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wwn.quarkkingdee.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bot.xuanzx.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://tfp.aibaodan.cn

【文件统计】
来源：http://nng.ywan-chungtsiang.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://foo.zhoulong.xyz

--------------------------------------------------------------------------------
来源：http://ajr.shanyushiyangkeji.top

目  录
来源：http://gzn.hywenlv.cn

--------------------------------------------------------------------------------
来源：http://tzw.tian-w.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://byw.jianghu66.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://lyt.hcnkem.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://bdl.meibo888.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://xmf.xylfe.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qxn.shzxlz.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://vft.yuanzhike.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xio.cqqwz.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ltb.ctjpmb.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xyq.fengsongda.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xik.ehwqpu.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://lco.aizwys.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qxo.smart0.xyz

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://yxi.316326.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://cyw.smart0.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xdw.shanyushiyangtech.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://jlj.haohaochexian.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://qbm.guannengcc.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://wul.jqgufenzy.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://yfc.yfazqb.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wpg.shanyushiyangkeji.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ihd.jianghu66.top

================================================================================
来源：http://ckf.vehdjk.com

A. 基础语法与类型
来源：http://top.birdmap.top

================================================================================
来源：http://zdr.shuidangran.top

[A01] Hello World
来源：http://pce.nwbrower.top

Py:   print("Hello, World!")
来源：http://ccu.zhaomingkeji.xyz

PHP:  echo "Hello, World!";
来源：http://czl.hnqzz.top

JS:   console.log("Hello, World!");
来源：http://sre.nanxinkj.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://kjr.pycfn.com

Java: System.out.println("Hello, World!");
来源：http://vqg.cucudq.cn

Go:   fmt.Println("Hello, World!")
来源：http://mpa.fengsongda.top

Ruby: puts "Hello, World!"
来源：http://vgw.andypj.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://fll.meibo888.top

[A02] 变量声明与赋值
来源：http://aef.yongpay.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://frd.sysykeji.top

PHP:  $name = "Alex"; $age = 20;
来源：http://gut.fzhhl.top

JS:   let name = "Alex"; const age = 20;
来源：http://lbj.jinqigfzy.top


<!-- 参考信息 -->