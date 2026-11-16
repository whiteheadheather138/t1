代发 wailian999

[U33] Py：打包发布
来源：http://emz.fehbvm.com

python -m build  （依赖 pyproject.toml）
来源：http://fba.zdbjq.cn

[U34] Py：判断编码
来源：http://bli.yangfankeji.com

chardet.detect(raw)
来源：http://dqd.c1oappe.top

[U35] Py：发送邮件
来源：http://cnd.tian-w.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hfh.jianghu66.top

[U36] Py：定时任务
来源：http://xjw.iojbl.cn

schedule.every(10).minutes.do(job)
来源：http://xqz.yj20258888.top

[U37] Py：读写 Excel
来源：http://who.haohaochexian.top

pandas.read_excel / DataFrame.to_excel
来源：http://kzm.cdnleiting.top

[U38] Py：获取脚本所在目录
来源：http://sog.tianlin.xyz

Path(__file__).resolve().parent
来源：http://oyf.jinqigufen.top

[U39] Py：判断是否在交互环境
来源：http://tan.snrcjt.cn

sys.stdout.isatty()
来源：http://lmu.shangyingyoupin.top

[U40] Py：打印到标准错误
来源：http://oum.bjfxy.top

print("err", file=sys.stderr)
来源：http://elf.cqqwz.cn

[U41] PHP：初始化 Composer 项目
来源：http://guf.sjlbkw.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ghp.dianchejie.cn

[U42] PHP：PSR-4 自动加载
来源：http://raf.0kj1m.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qib.cashguo.top

[U43] PHP：声明命名空间
来源：http://vaq.jyoumei.cn

namespace App\Http;
来源：http://awu.birdmap.top

[U44] PHP：开启严格类型
来源：http://ezu.pengpengdd.cyou

declare(strict_types=1);
来源：http://csu.yongpay.top

[U45] PHP：类型声明与返回类型
来源：http://gqk.tianlin.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://cuw.c1oappe.top

[U46] PHP：可空类型
来源：http://ovo.feifeiyinyue.top

?string $name = null
来源：http://vuf.zhoulong.xyz

[U47] PHP：联合类型
来源：http://qxs.guowangkeji.top

int|string $id
来源：http://jxw.sjlbkw.cn

[U48] PHP：纯枚举
来源：http://meu.jlsjyb.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lqz.daxiang520.top

[U49] PHP：只读属性
来源：http://xlk.ppjwa.cn

public readonly string $name
来源：http://sei.yuanzhike.top

[U50] PHP：构造器属性提升
来源：http://jqe.guowangkeji.top

public function __construct(private int $id) {}
来源：http://ziw.vqdsnc.cn

[U51] PHP：数组解构
来源：http://sci.jinqigfzy.top

[$a, $b] = $arr;
来源：http://kdc.cqqwz.cn

[U52] PHP：箭头函数
来源：http://ugo.chenlongwang.top

$double = fn($x) => $x * 2;
来源：http://zwk.epnwcf.com

[U53] PHP：空合并运算符
来源：http://wul.jqgufenzy.top

$v = $a ?? $b ?? "default";
来源：http://yxy.gzhubu.top

[U54] PHP：空安全调用
来源：http://mni.meibo888.top

$obj?->method()
来源：http://ovq.aibaodan.cn

[U55] PHP：match 表达式
来源：http://fqt.yongpay.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kco.hywenlv.cn

[U56] PHP：命名参数
来源：http://meq.zdqjudy.top

f(a: 1, b: 2)
来源：http://mry.vehdjk.com

[U57] PHP：字符串插值
来源：http://lgc.zhiwuduotai.top

"值: {$a}"
来源：http://puh.bbcook.cn

[U58] PHP：数组三件套
来源：http://fhu.snrcjt.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mqw.jyoumei.cn

[U59] PHP：自定义排序
来源：http://efy.ppjwa.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fur.svipenyu.cn

[U60] PHP：JSON 编解码
来源：http://wdk.xziqi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://eqp.yongpay.top

[U61] PHP：正则
来源：http://yqf.vqdsnc.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://esf.shuidangran.top

[U62] PHP：日期对象
来源：http://yib.sweek.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jtu.chenjidiqi.icu

[U63] PHP：文件读写
来源：http://ypw.cdnleiting.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fdk.haohaochexian.top

[U64] PHP：目录遍历
来源：http://sjq.jinqigufen.top

glob("dir/*.php");  scandir("dir");
来源：http://ldh.jiagoushi.top

[U65] PHP：会话
来源：http://opl.sufxvd.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://pzc.yj202588.top

[U66] PHP：设置 Cookie
来源：http://bvc.gogol.net.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://quz.yuxming.cn

[U67] PHP：处理文件上传
来源：http://fqq.shanyushiyangkeji.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://nul.fktsv.cn

[U68] PHP：PDO 连接
来源：http://jfa.tian-w.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hzr.hongshengwenyu.top

[U69] PHP：PDO 预处理
来源：http://ibk.birdmap.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ovi.zdbjq.cn

[U70] PHP：PDO 事务
来源：http://ubz.yfazqb.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dnv.aizwys.cn

[U71] PHP：抛出异常
来源：http://mml.yj20258.top

throw new RuntimeException("失败", 500);
来源：http://ham.xziqi.cn

[U72] PHP：写错误日志
来源：http://lqw.iojbl.cn

error_log("失败: " . $e->getMessage());
来源：http://hlo.svipenyu.cn

[U73] PHP：读取 ini 配置
来源：http://cos.yangfankeji.com

parse_ini_file("config.ini", true)
来源：http://ilg.c1oappe.top

[U74] PHP：读取环境变量
来源：http://vsi.xziqi.cn

getenv("APP_ENV") ?: "production"
来源：http://aer.cheryme.top

[U75] PHP：依赖注入
来源：http://uih.jqgufenzy.top

composer require psr/container
来源：http://vce.52xcode.cn

[U76] PHP：简单路由
来源：http://mto.tianlin.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jnz.feifeiyinyue.top

[U77] PHP：模板渲染
来源：http://knf.pengpengdd.cyou

composer require twig/twig
来源：http://pox.cdnleiting.top

[U78] PHP：单元测试
来源：http://pds.ydzc1.top

composer require --dev phpunit/phpunit
来源：http://kgj.iojbl.cn

[U79] PHP：静态分析
来源：http://cug.hysaishi.cn

composer require --dev phpstan/phpstan
来源：http://gfs.hnxiangtu.top

[U80] PHP：代码规范修复
来源：http://lgl.uphjek.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://ybu.jinyuanbaomall.cn

[U81] JS：初始化项目
来源：http://xxz.yj202588.top

npm init -y;  npm i express
来源：http://nuj.nanxuanxn.top

[U82] JS：package.json 脚本
来源：http://txw.chenzaomai.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hsq.epnwcf.com

[U83] JS：ES Module 导入导出
来源：http://jqq.zhengqikj.top

export const a = 1;  import { a } from "./m.js";
来源：http://puu.ywan-chungtsiang.top

[U84] JS：CommonJS 写法
来源：http://jbj.jinyuanbaomall.cn

module.exports = { a };  const { a } = require("./m");
来源：http://hdq.epnwcf.com

[U85] JS：可选链
来源：http://ldz.zdbjq.cn

a?.b?.c
来源：http://pbx.yanxiufei.cn

[U86] JS：空值合并
来源：http://glg.bjfxy.top

a ?? b
来源：http://tjt.zhaomingkeji.xyz

[U87] JS：解构默认值
来源：http://jju.nanxuanxn.top

const { a = 1, b = 2 } = obj;
来源：http://csf.xuetiantiany.cn

[U88] JS：对象展开合并
来源：http://fdf.nanxuanxn.top

{ ...a, ...b }
来源：http://ukb.svipenyu.cn

[U89] JS：数组去重
来源：http://ach.cdnleiting.top

[...new Set(arr)]
来源：http://tow.sxryk.cn

[U90] JS：数字数组排序
来源：http://kpf.havefunace.top

[...arr].sort((a, b) => a - b)
来源：http://tub.wangshuangyany.cn

[U91] JS：对象键值遍历
来源：http://ecq.daria6918.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wka.sufxvd.cn

[U92] JS：深拷贝
来源：http://cqb.wangdashe.top

structuredClone(obj)
来源：http://nrw.aizwys.cn

[U93] JS：模板字符串
来源：http://vlz.cashguo.top

`共 ${n} 条`
来源：http://ris.c1oappe.top

[U94] JS：箭头函数
来源：http://bxd.hesvh.cn

const double = x => x * 2;
来源：http://qrt.aibaodan.cn

[U95] JS：Promise 包装
来源：http://aip.fanxiaobao.xyz

new Promise((resolve, reject) => {})
来源：http://eci.nanxinkj.top

[U96] JS：async/await 与异常
来源：http://zda.bjfxy.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nlm.sweek.top

[U97] JS：并发请求
来源：http://bsk.hnxiangtu.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://pvs.dashuyun.cn

[U98] JS：fetch 带 JSON
来源：http://ghp.hongshengwenyu.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wzq.pengpengdd.cyou

[U99] JS：事件监听
来源：http://nej.yangfankeji.com

el.addEventListener("click", e => {})
来源：http://zeo.xuetiantiany.cn

[U100] JS：DOM 查询
来源：http://cji.jiagoushi.top

document.querySelector(".item")
来源：http://inv.yuxming.cn

[U101] JS：classList 操作
来源：http://lgc.yueranfly.top

el.classList.toggle("active")
来源：http://see.xziqi.cn

[U102] JS：本地存储
来源：http://eqy.yvedp.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ocn.daria6918.cn

[U103] JS：定时器
来源：http://raj.yonumen.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ben.nanxinkj.top

[U104] JS：防抖
来源：http://rrv.smart0.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oyo.jianghu66.top

[U105] JS：节流
来源：http://lxs.jinqigfzy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zta.hesvh.cn

[U106] JS：日期格式化
来源：http://rpg.sxryk.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cry.jinqigufen.top

[U107] JS：数字千分位
来源：http://uku.guannengcc.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wvb.daria6918.cn

[U108] JS：随机整数
来源：http://osp.yonumen.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hux.yuxming.cn

[U109] JS：数组分组
来源：http://gnt.hfpthk.cn

Object.groupBy(arr, x => x.type)
来源：http://ttd.epnwcf.com

[U110] JS：数组分块
来源：http://wyj.epnwcf.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://odl.shzxlz.cn

[U111] JS：对象转 Map
来源：http://xgn.zdqjudy.top

new Map(Object.entries(obj))
来源：http://ylf.fzhhl.top

[U112] JS：字符串补位
来源：http://mpl.52xcode.cn

"7".padStart(3, "0")
来源：http://yta.ivvv.top

[U113] JS：正则替换全部
来源：http://wvv.jinqigufen.top

s.replaceAll("a", "b")
来源：http://qys.xziqi.cn

[U114] JS：JSON 深比较
来源：http://cps.pycfn.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://nzp.yj20258888.top

[U115] JS：生成 UUID
来源：http://xqv.chenlongwang.top

crypto.randomUUID()
来源：http://xzc.cqqwz.cn

[U116] JS：类型检查（JSDoc）
来源：http://mnl.vqdsnc.cn

/** @param {string} name */ function f(name) {}
来源：http://kdp.hnqzz.top

[U117] JS：单元测试
来源：http://ubc.yvedp.cn

npm i -D vitest;  npx vitest
来源：http://mrj.cheryme.top

[U118] JS：开发服务器
来源：http://vmu.yanxiufei.cn

npm i -D vite;  npx vite
来源：http://mog.dianchejie.cn

[U119] JS：生产构建
来源：http://yxg.gogol.net.cn

npx vite build
来源：http://zpr.ydjk.org.cn

[U120] JS：读取环境变量（Vite）
来源：http://sof.yuanzhike.top

import.meta.env.VITE_API_URL
来源：http://szp.ivvv.top

================================================================================
来源：http://xnq.xingfuxueyuan.xyz

统计汇总
来源：http://opl.uphjek.com

================================================================================
来源：http://wmz.pycfn.com

按语言统计（条）：
来源：http://ipy.sufxvd.cn

Python ......... 252
来源：http://srp.jiagoushi.top

PHP ............ 252
来源：http://ubr.wangshuangyany.cn

JavaScript ..... 252
来源：http://lxr.jinqigufen.top

TypeScript ..... 212
来源：http://aby.yangfankeji.com

Java ........... 212
来源：http://scw.gogol.net.cn

Go ............. 212
来源：http://vfg.jinqigfzy.top

Ruby ........... 212
来源：http://dpr.yj20258.top

C# ............. 212
来源：http://zkq.vehdjk.com

C .............. 30
来源：http://euf.jqgufenzy.top

C++ ............ 30
来源：http://flp.hammf.cn

SQL ............ 90
来源：http://fwx.gaohongyu789.top

Bash ........... 80
来源：http://avj.tianlin.xyz

Kotlin ......... 15
来源：http://qai.vqdsnc.cn

Swift .......... 15
来源：http://wfo.vehdjk.com

Lua ............ 10
来源：http://bbx.meibo888.top

Perl ........... 10
来源：http://rus.0kj1m.cn

Scala .......... 10
来源：http://pac.yanxiufei.cn

------------------------------------
来源：http://fbp.xuetiantiany.cn

合计 ........... 2106 条
来源：http://chq.zhongyouzk.top

按章节统计：
来源：http://qun.guannengcc.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xij.yj20258.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://pjg.smart0.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mjc.sysykeji.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mpk.havefunace.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://kyd.cashguo.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://inm.yj202588.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wzg.andypj.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://dec.wangshuangyany.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://oxk.cucudq.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://cme.daria6918.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://yqk.ywan-chungtsiang.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dbx.gotoacloud.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://utb.0kj1m.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zpa.gotoacloud.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://xva.yongpay.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://riw.tanke756.top

Q SQL 专题                              90
来源：http://ggc.smart0.xyz

R Bash 专题                             80
来源：http://zeb.vqdsnc.cn

S C / C++ 专题                          60
来源：http://drz.xingfuxueyuan.xyz

T 其他语言补充                          60
来源：http://ovl.bbcook.cn

U 高频实用片段                         120
来源：http://pay.xuanzx.com

------------------------------------
来源：http://bym.yangfankeji.com

合计                                  2106 条
来源：http://com.jinyuanbaomall.cn

--------------------------------------------------------------------------------
来源：http://qgv.guowangkeji.top

使用提醒
来源：http://jwi.havefunace.top

--------------------------------------------------------------------------------
来源：http://mfj.jianghu66.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mnh.fanxiaobao.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://dfl.tian-w.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://luq.aizwys.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://jhv.tanke756.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://htk.cheryme.top

—— 文件结束 ——
来源：http://zou.ctjpmb.com

================================================================================
来源：http://uab.jqgufenzy.top

程序语言常见例子速查手册（2024 版）
来源：http://sro.gogol.net.cn

Common Programming Examples Cheat Book
来源：http://rke.nanxinkj.top

================================================================================
来源：http://vik.9152youxi.cn

【收录内容】
来源：http://ogo.uphjek.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://gsf.gaohongyu789.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://znk.yangfankeji.com

SQL · Bash · C · C++
来源：http://vnp.yanxiufei.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://rrp.9152youxi.cn

【使用说明】
来源：http://cyk.yuxming.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://bba.pycfn.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xpk.xuanzx.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://tcd.guannengcc.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://fsp.zhiwuduotai.top

Bash:  Shell         C:     C             C++:   C++
来源：http://hyd.ydzc1.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://eyv.hesvh.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wie.hcnkem.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vwk.hammf.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://sgv.gogol.net.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wsl.uphjek.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://gil.meibo888.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zzk.jinyuanbaomall.cn

【文件统计】
来源：http://xhv.bbcook.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://czf.xingfuxueyuan.xyz

--------------------------------------------------------------------------------
来源：http://fof.zdqjudy.top

目  录
来源：http://koi.fzhhl.top

--------------------------------------------------------------------------------
来源：http://ywb.jlsjyb.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hlt.ydzc1.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://bua.tianlin.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jza.zycfv.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://kjx.yueranfly.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://xzy.vehdjk.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qsg.316326.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://opq.snrcjt.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://yqx.zhongyouzk.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wqe.havefunace.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://evq.9152youxi.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://jjq.kuanghao11.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://fwe.jyoumei.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://sdk.ivvv.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://tig.jqgufenzy.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://bzy.guannengcc.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://eyh.hammf.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wcu.hywenlv.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://boh.hnxiangtu.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://pis.shangyingyoupin.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fvt.xziqi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://rxh.jiagoushi.top

================================================================================
来源：http://eed.cashguo.top

A. 基础语法与类型
来源：http://cvt.ydjk.org.cn

================================================================================
来源：http://eah.jyoumei.cn

[A01] Hello World
来源：http://nyf.smart0.xyz

Py:   print("Hello, World!")
来源：http://mct.jinyuanbaomall.cn

PHP:  echo "Hello, World!";
来源：http://pdt.xingfuxueyuan.xyz

JS:   console.log("Hello, World!");
来源：http://lka.sxryk.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wyh.nanxuanxn.top

Java: System.out.println("Hello, World!");
来源：http://tmw.chenjidiqi.icu

Go:   fmt.Println("Hello, World!")
来源：http://bni.shzxlz.cn

Ruby: puts "Hello, World!"
来源：http://aaj.dianchejie.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://hae.guowangkeji.top

[A02] 变量声明与赋值
来源：http://rja.zycfv.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://svg.xylfe.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://hnh.xuanzx.com

JS:   let name = "Alex"; const age = 20;
来源：http://zvn.hnqzz.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bdx.jinqigufen.top

Java: String name = "Alex"; int age = 20;
来源：http://vnp.tianlin.xyz

Go:   name := "Alex"; age := 20
来源：http://bpi.yueranfly.top

Ruby: name = "Alex"; age = 20
来源：http://nls.svipenyu.cn


<!-- 参考信息 -->