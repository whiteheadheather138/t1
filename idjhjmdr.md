代发 wailian999

[U33] Py：打包发布
来源：http://fsl.ydjk.org.cn

python -m build  （依赖 pyproject.toml）
来源：http://mvg.shanyushiyangkeji.top

[U34] Py：判断编码
来源：http://agc.zhengqikj.top

chardet.detect(raw)
来源：http://dav.epnwcf.com

[U35] Py：发送邮件
来源：http://xpp.ehwqpu.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hjf.chenjidiqi.icu

[U36] Py：定时任务
来源：http://aoe.hywenlv.cn

schedule.every(10).minutes.do(job)
来源：http://xpd.yonumen.top

[U37] Py：读写 Excel
来源：http://jep.zhengqikj.top

pandas.read_excel / DataFrame.to_excel
来源：http://kac.shuidangran.top

[U38] Py：获取脚本所在目录
来源：http://zgg.epnwcf.com

Path(__file__).resolve().parent
来源：http://sec.yueranfly.top

[U39] Py：判断是否在交互环境
来源：http://evk.ctjpmb.com

sys.stdout.isatty()
来源：http://gnm.daxiang520.top

[U40] Py：打印到标准错误
来源：http://csm.shuidangran.top

print("err", file=sys.stderr)
来源：http://eyb.bjfxy.top

[U41] PHP：初始化 Composer 项目
来源：http://vec.hywenlv.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://qqp.chenzaomai.com

[U42] PHP：PSR-4 自动加载
来源：http://xnr.tanke756.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mif.xinyue.icu

[U43] PHP：声明命名空间
来源：http://hve.chenzaomai.com

namespace App\Http;
来源：http://xuo.sweek.top

[U44] PHP：开启严格类型
来源：http://dod.ivvv.top

declare(strict_types=1);
来源：http://tsf.xuetiantiany.cn

[U45] PHP：类型声明与返回类型
来源：http://evf.yueranfly.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://tpp.guowangkeji.top

[U46] PHP：可空类型
来源：http://icw.bjfxy.top

?string $name = null
来源：http://uie.zhijiandao.cn

[U47] PHP：联合类型
来源：http://wiy.tarul.cn

int|string $id
来源：http://isp.ybcxt.top

[U48] PHP：纯枚举
来源：http://ure.uphjek.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tdc.epnwcf.com

[U49] PHP：只读属性
来源：http://cdr.tian-w.cn

public readonly string $name
来源：http://yqz.zhengqikj.top

[U50] PHP：构造器属性提升
来源：http://bac.epnwcf.com

public function __construct(private int $id) {}
来源：http://lpg.nanxuanxn.top

[U51] PHP：数组解构
来源：http://naf.ctjpmb.com

[$a, $b] = $arr;
来源：http://kyj.jinghuilouyu.cn

[U52] PHP：箭头函数
来源：http://vkc.ivvv.top

$double = fn($x) => $x * 2;
来源：http://iwz.hnqzz.top

[U53] PHP：空合并运算符
来源：http://brt.redwolf501.top

$v = $a ?? $b ?? "default";
来源：http://euu.zhixingplan.top

[U54] PHP：空安全调用
来源：http://wjn.vehdjk.com

$obj?->method()
来源：http://ocd.gotoacloud.top

[U55] PHP：match 表达式
来源：http://kmf.feifeiyinyue.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gwq.fanxiaobao.xyz

[U56] PHP：命名参数
来源：http://hsh.yj20258888.top

f(a: 1, b: 2)
来源：http://vjs.yj20258.top

[U57] PHP：字符串插值
来源：http://gax.xingfuxueyuan.xyz

"值: {$a}"
来源：http://wvr.gogol.net.cn

[U58] PHP：数组三件套
来源：http://qer.shanyushiyangkeji.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ujc.zdqjudy.top

[U59] PHP：自定义排序
来源：http://xak.jyoumei.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xrj.hywenlv.cn

[U60] PHP：JSON 编解码
来源：http://shg.snrcjt.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zzu.sweek.top

[U61] PHP：正则
来源：http://htn.chenzaomai.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jlf.shangyingyoupin.top

[U62] PHP：日期对象
来源：http://xwd.ehwqpu.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mpo.zycfv.cn

[U63] PHP：文件读写
来源：http://nvc.ywan-chungtsiang.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wbo.hnqzz.top

[U64] PHP：目录遍历
来源：http://jjx.jinyuanbaomall.cn

glob("dir/*.php");  scandir("dir");
来源：http://quf.zhaomingkeji.xyz

[U65] PHP：会话
来源：http://oha.gaohongyu789.top

session_start();  $_SESSION["uid"] = 1;
来源：http://msc.jyoumei.cn

[U66] PHP：设置 Cookie
来源：http://wtp.tian-w.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vex.epnwcf.com

[U67] PHP：处理文件上传
来源：http://sxa.aibaodan.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bwn.zhixingplan.top

[U68] PHP：PDO 连接
来源：http://wfv.bbcook.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rlm.haohaochexian.top

[U69] PHP：PDO 预处理
来源：http://ryq.nwbrower.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://pjh.yj20258.top

[U70] PHP：PDO 事务
来源：http://qqc.xuanzx.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jbo.ydjk.org.cn

[U71] PHP：抛出异常
来源：http://xgk.zhoulong.xyz

throw new RuntimeException("失败", 500);
来源：http://zmv.iojbl.cn

[U72] PHP：写错误日志
来源：http://dno.nanxuanxn.top

error_log("失败: " . $e->getMessage());
来源：http://nwn.yanxiufei.cn

[U73] PHP：读取 ini 配置
来源：http://gnz.dashuyun.cn

parse_ini_file("config.ini", true)
来源：http://azs.smart0.xyz

[U74] PHP：读取环境变量
来源：http://ycc.cdnleiting.top

getenv("APP_ENV") ?: "production"
来源：http://gqh.0kj1m.cn

[U75] PHP：依赖注入
来源：http://nnm.fanxiaobao.xyz

composer require psr/container
来源：http://gwt.dashuyun.cn

[U76] PHP：简单路由
来源：http://kbf.ctjpmb.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://byy.xuetiantiany.cn

[U77] PHP：模板渲染
来源：http://dsn.yj202588.top

composer require twig/twig
来源：http://hrq.yj202588.top

[U78] PHP：单元测试
来源：http://dro.ydzc1.top

composer require --dev phpunit/phpunit
来源：http://gxj.ehwqpu.com

[U79] PHP：静态分析
来源：http://ywo.zhengqikj.top

composer require --dev phpstan/phpstan
来源：http://dic.sxryk.cn

[U80] PHP：代码规范修复
来源：http://rzr.daria6918.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://gfd.bjfxy.top

[U81] JS：初始化项目
来源：http://phs.sxryk.cn

npm init -y;  npm i express
来源：http://ytn.gzhubu.top

[U82] JS：package.json 脚本
来源：http://tjl.aizwys.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hpo.pengpengdd.cyou

[U83] JS：ES Module 导入导出
来源：http://zdd.tianlin.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://qjt.zdqjudy.top

[U84] JS：CommonJS 写法
来源：http://fei.jianghu66.top

module.exports = { a };  const { a } = require("./m");
来源：http://pkx.nanxinkj.top

[U85] JS：可选链
来源：http://bos.nanxuanxn.top

a?.b?.c
来源：http://rts.kuanghao11.cn

[U86] JS：空值合并
来源：http://rwu.zdbjq.cn

a ?? b
来源：http://gna.zdbjq.cn

[U87] JS：解构默认值
来源：http://eiz.cheryme.top

const { a = 1, b = 2 } = obj;
来源：http://csa.xinyue.icu

[U88] JS：对象展开合并
来源：http://xde.yonumen.top

{ ...a, ...b }
来源：http://bdf.hysaishi.cn

[U89] JS：数组去重
来源：http://nho.0kj1m.cn

[...new Set(arr)]
来源：http://tbl.tanke756.top

[U90] JS：数字数组排序
来源：http://wyu.ctjpmb.com

[...arr].sort((a, b) => a - b)
来源：http://aig.hysaishi.cn

[U91] JS：对象键值遍历
来源：http://zza.hysaishi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ftj.jianghu66.top

[U92] JS：深拷贝
来源：http://nay.jqgufenzy.top

structuredClone(obj)
来源：http://qcf.chenzaomai.com

[U93] JS：模板字符串
来源：http://mtg.sweek.top

`共 ${n} 条`
来源：http://hep.hnqzz.top

[U94] JS：箭头函数
来源：http://rdc.bjfxy.top

const double = x => x * 2;
来源：http://jwa.bbcook.cn

[U95] JS：Promise 包装
来源：http://tye.dashuyun.cn

new Promise((resolve, reject) => {})
来源：http://pay.yanxiufei.cn

[U96] JS：async/await 与异常
来源：http://eqv.gzhubu.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wvm.svipenyu.cn

[U97] JS：并发请求
来源：http://jwj.yj202588.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://fcb.feifeiyinyue.top

[U98] JS：fetch 带 JSON
来源：http://jvd.yj20258.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rvk.hysaishi.cn

[U99] JS：事件监听
来源：http://sgi.hfpthk.cn

el.addEventListener("click", e => {})
来源：http://dyj.hammf.cn

[U100] JS：DOM 查询
来源：http://irr.havefunace.top

document.querySelector(".item")
来源：http://mtm.ydzc1.top

[U101] JS：classList 操作
来源：http://ncs.tianlin.xyz

el.classList.toggle("active")
来源：http://rvr.birdmap.top

[U102] JS：本地存储
来源：http://tes.hesvh.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jbb.nanxinkj.top

[U103] JS：定时器
来源：http://zrz.sysykeji.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wbg.yj202588.top

[U104] JS：防抖
来源：http://xiq.svipenyu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yfg.xuetiantiany.cn

[U105] JS：节流
来源：http://hee.snrcjt.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://plu.smart0.xyz

[U106] JS：日期格式化
来源：http://xod.316326.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lmo.zycfv.cn

[U107] JS：数字千分位
来源：http://vgn.redwolf501.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://tol.sysykeji.top

[U108] JS：随机整数
来源：http://gud.fktsv.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kge.andypj.xyz

[U109] JS：数组分组
来源：http://mwp.ctjpmb.com

Object.groupBy(arr, x => x.type)
来源：http://gbd.andypj.xyz

[U110] JS：数组分块
来源：http://qju.ywan-chungtsiang.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ppk.tarul.cn

[U111] JS：对象转 Map
来源：http://tqd.yuanzhike.top

new Map(Object.entries(obj))
来源：http://ria.jinqigufen.top

[U112] JS：字符串补位
来源：http://cme.jianghu66.top

"7".padStart(3, "0")
来源：http://ien.kuanghao11.cn

[U113] JS：正则替换全部
来源：http://irc.tianlin.xyz

s.replaceAll("a", "b")
来源：http://diy.shzxlz.cn

[U114] JS：JSON 深比较
来源：http://fuy.zhongyouzk.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://rvf.meibo888.top

[U115] JS：生成 UUID
来源：http://rux.hnqzz.top

crypto.randomUUID()
来源：http://cul.nwbrower.top

[U116] JS：类型检查（JSDoc）
来源：http://hqi.zhengqikj.top

/** @param {string} name */ function f(name) {}
来源：http://ofc.yj202588.top

[U117] JS：单元测试
来源：http://gqz.tianlin.xyz

npm i -D vitest;  npx vitest
来源：http://ybk.yvedp.cn

[U118] JS：开发服务器
来源：http://lyy.hfpthk.cn

npm i -D vite;  npx vite
来源：http://ect.zycfv.cn

[U119] JS：生产构建
来源：http://rcf.vqdsnc.cn

npx vite build
来源：http://wmm.tanke756.top

[U120] JS：读取环境变量（Vite）
来源：http://fpy.daxiang520.top

import.meta.env.VITE_API_URL
来源：http://ocb.zycfv.cn

================================================================================
来源：http://xwp.zhijiandao.cn

统计汇总
来源：http://qgu.yuanzhike.top

================================================================================
来源：http://xql.zdqjudy.top

按语言统计（条）：
来源：http://nzl.chenjidiqi.icu

Python ......... 252
来源：http://mbt.cheryme.top

PHP ............ 252
来源：http://gsw.yuanzhike.top

JavaScript ..... 252
来源：http://ykz.fzhhl.top

TypeScript ..... 212
来源：http://sna.haohaochexian.top

Java ........... 212
来源：http://utq.hesvh.cn

Go ............. 212
来源：http://ivv.hywenlv.cn

Ruby ........... 212
来源：http://tzu.cucudq.cn

C# ............. 212
来源：http://oho.andypj.xyz

C .............. 30
来源：http://pbu.aibaodan.cn

C++ ............ 30
来源：http://twh.guowangkeji.top

SQL ............ 90
来源：http://owd.xinyue.icu

Bash ........... 80
来源：http://bem.pycfn.com

Kotlin ......... 15
来源：http://jex.quarkkingdee.top

Swift .......... 15
来源：http://gya.hfpthk.cn

Lua ............ 10
来源：http://jbx.yfazqb.com

Perl ........... 10
来源：http://jnx.yuanzhike.top

Scala .......... 10
来源：http://rqd.sjlbkw.cn

------------------------------------
来源：http://kih.sysykeji.top

合计 ........... 2106 条
来源：http://fyy.uphjek.com

按章节统计：
来源：http://nxr.hammf.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://egx.zhiwuduotai.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zlm.yuanzhike.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://yxz.zdqjudy.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ykv.yj20258888.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gsx.yuanzhike.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ysk.fehbvm.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jro.gotoacloud.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://iqu.yj202588.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://dyq.yongpay.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mwp.zhijiandao.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://agp.sweek.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dqa.hfpthk.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://lkk.yuxming.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://oze.wangdashe.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://cdx.yongpay.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://puq.guowangkeji.top

Q SQL 专题                              90
来源：http://yue.ctjpmb.com

R Bash 专题                             80
来源：http://jeu.jinyuanbaomall.cn

S C / C++ 专题                          60
来源：http://vfb.xinyue.icu

T 其他语言补充                          60
来源：http://smy.smart0.xyz

U 高频实用片段                         120
来源：http://tpb.dashuyun.cn

------------------------------------
来源：http://lqy.jinqigfzy.top

合计                                  2106 条
来源：http://qfx.fengsongda.top

--------------------------------------------------------------------------------
来源：http://qwd.aizwys.cn

使用提醒
来源：http://ugr.hammf.cn

--------------------------------------------------------------------------------
来源：http://dyu.jyoumei.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jks.guannengcc.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://kuv.dianchejie.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mel.sysykeji.top

在旧版本上使用前请先确认语法支持情况。
来源：http://mae.jqgufenzy.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://obh.shanyushiyangkeji.top

—— 文件结束 ——
来源：http://wrv.gaohongyu789.top

================================================================================
来源：http://xtc.hammf.cn

程序语言常见例子速查手册（2024 版）
来源：http://apy.cucudq.cn

Common Programming Examples Cheat Book
来源：http://hmm.ybcxt.top

================================================================================
来源：http://gym.zhongyouzk.top

【收录内容】
来源：http://ueh.gogol.net.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://hxn.jlsjyb.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nhl.sjlbkw.cn

SQL · Bash · C · C++
来源：http://pmt.yuanzhike.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://tdq.jinqigufen.top

【使用说明】
来源：http://bdn.ybcxt.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ahm.shuidangran.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://aaf.epnwcf.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://vrb.birdmap.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qgm.zdqjudy.top

Bash:  Shell         C:     C             C++:   C++
来源：http://hsh.jqgfzy.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://tpb.52xcode.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://bph.yj20258888.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xlr.hywenlv.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://dco.haohaochexian.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://vqd.vqdsnc.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://tyz.shanyushiyangkeji.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://oax.wangdashe.top

【文件统计】
来源：http://gxf.smart0.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ush.hongshengwenyu.top

--------------------------------------------------------------------------------
来源：http://kpn.cashguo.top

目  录
来源：http://xuj.9152youxi.cn

--------------------------------------------------------------------------------
来源：http://rda.iojbl.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://awn.ybcxt.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://nrm.kuanghao11.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://rwq.cucudq.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://dmr.chenzaomai.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hvq.shzxlz.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://esn.jqgfzy.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://res.epnwcf.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://nii.jinyuanbaomall.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xrn.ehwqpu.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://frk.fktsv.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://okq.fehbvm.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://rfu.hnqzz.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://pib.ctjpmb.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zkk.jinqigufen.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://zjb.jlsjyb.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://tbv.shuidangran.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jzd.cucudq.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://wli.jinqigfzy.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://epy.jinqigfzy.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mtu.yueranfly.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mle.tarul.cn

================================================================================
来源：http://deg.sweek.top

A. 基础语法与类型
来源：http://uko.cqqwz.cn

================================================================================
来源：http://kms.yonumen.top

[A01] Hello World
来源：http://zxm.iojbl.cn

Py:   print("Hello, World!")
来源：http://ebx.chenlongwang.top

PHP:  echo "Hello, World!";
来源：http://muy.tianlin.xyz

JS:   console.log("Hello, World!");
来源：http://rsc.ywan-chungtsiang.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://kdp.ywan-chungtsiang.top

Java: System.out.println("Hello, World!");
来源：http://iup.zdbjq.cn

Go:   fmt.Println("Hello, World!")
来源：http://ivi.ivvv.top

Ruby: puts "Hello, World!"
来源：http://nzj.ehwqpu.com

C#:   Console.WriteLine("Hello, World!");
来源：http://jza.fanxiaobao.xyz

[A02] 变量声明与赋值
来源：http://vbe.cucudq.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://qsc.shzxlz.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://eqb.chenzaomai.com

JS:   let name = "Alex"; const age = 20;
来源：http://jlg.c1oappe.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://dlt.0kj1m.cn

Java: String name = "Alex"; int age = 20;
来源：http://cfz.jyoumei.cn

Go:   name := "Alex"; age := 20
来源：http://uyu.yvedp.cn

Ruby: name = "Alex"; age = 20
来源：http://yum.316326.xyz


<!-- 参考信息 -->