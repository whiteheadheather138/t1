代发 wailian999

[U31] Py：单测
来源：http://els.kuanghao11.cn

python -m pytest -q
来源：http://qry.guannengcc.top

[U32] Py：代码格式化
来源：http://ksa.quarkkingdee.top

ruff format . && ruff check --fix .
来源：http://ttk.shangyingyoupin.top

[U33] Py：打包发布
来源：http://zis.guowangkeji.top

python -m build  （依赖 pyproject.toml）
来源：http://kem.daria6918.cn

[U34] Py：判断编码
来源：http://flf.jinghuilouyu.cn

chardet.detect(raw)
来源：http://jxo.sysykeji.top

[U35] Py：发送邮件
来源：http://isz.yj202588.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jgh.ppjwa.cn

[U36] Py：定时任务
来源：http://bye.zhongyouzk.top

schedule.every(10).minutes.do(job)
来源：http://xyh.jinqigufen.top

[U37] Py：读写 Excel
来源：http://zou.sysykeji.top

pandas.read_excel / DataFrame.to_excel
来源：http://vqv.fktsv.cn

[U38] Py：获取脚本所在目录
来源：http://sec.ydzc1.top

Path(__file__).resolve().parent
来源：http://asz.tarul.cn

[U39] Py：判断是否在交互环境
来源：http://ufv.zdqjudy.top

sys.stdout.isatty()
来源：http://dqk.smart0.xyz

[U40] Py：打印到标准错误
来源：http://wab.ivvv.top

print("err", file=sys.stderr)
来源：http://lrk.zhiwuduotai.top

[U41] PHP：初始化 Composer 项目
来源：http://vgb.pengpengdd.cyou

composer init;  composer require guzzlehttp/guzzle
来源：http://pbr.shanyushiyangtech.top

[U42] PHP：PSR-4 自动加载
来源：http://qnd.sufxvd.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cyz.dashuyun.cn

[U43] PHP：声明命名空间
来源：http://ycw.dashuyun.cn

namespace App\Http;
来源：http://rxp.yj20258888.top

[U44] PHP：开启严格类型
来源：http://jry.316326.xyz

declare(strict_types=1);
来源：http://pmv.meibo888.top

[U45] PHP：类型声明与返回类型
来源：http://xtn.aibaodan.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ppa.shzxlz.cn

[U46] PHP：可空类型
来源：http://jhb.quarkkingdee.top

?string $name = null
来源：http://npn.shangyingyoupin.top

[U47] PHP：联合类型
来源：http://ccy.hnxiangtu.top

int|string $id
来源：http://ikj.ybcxt.top

[U48] PHP：纯枚举
来源：http://gqz.gogol.net.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lgf.tianlin.xyz

[U49] PHP：只读属性
来源：http://exs.sxryk.cn

public readonly string $name
来源：http://typ.yvedp.cn

[U50] PHP：构造器属性提升
来源：http://hud.tanke756.top

public function __construct(private int $id) {}
来源：http://mbs.bjfxy.top

[U51] PHP：数组解构
来源：http://dqj.fzhhl.top

[$a, $b] = $arr;
来源：http://pud.fzhhl.top

[U52] PHP：箭头函数
来源：http://rvk.snrcjt.cn

$double = fn($x) => $x * 2;
来源：http://isn.jinyuanbaomall.cn

[U53] PHP：空合并运算符
来源：http://cie.xingfuxueyuan.xyz

$v = $a ?? $b ?? "default";
来源：http://ztc.hfpthk.cn

[U54] PHP：空安全调用
来源：http://ycc.zhengqikj.top

$obj?->method()
来源：http://lir.hfpthk.cn

[U55] PHP：match 表达式
来源：http://mel.yj20258.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://sss.ydzc1.top

[U56] PHP：命名参数
来源：http://bqk.daxiang520.top

f(a: 1, b: 2)
来源：http://ssi.zhongyouzk.top

[U57] PHP：字符串插值
来源：http://tle.hnxiangtu.top

"值: {$a}"
来源：http://eno.xuetiantiany.cn

[U58] PHP：数组三件套
来源：http://aih.yuxming.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fvo.xuanzx.com

[U59] PHP：自定义排序
来源：http://oau.yangfankeji.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tiu.meibo888.top

[U60] PHP：JSON 编解码
来源：http://iyn.shangyingyoupin.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zui.wangdashe.top

[U61] PHP：正则
来源：http://nhv.jqgufenzy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qce.uphjek.com

[U62] PHP：日期对象
来源：http://yxv.yonumen.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://dhv.jiagoushi.top

[U63] PHP：文件读写
来源：http://rsc.xinyue.icu

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vsf.gogol.net.cn

[U64] PHP：目录遍历
来源：http://oco.daxiang520.top

glob("dir/*.php");  scandir("dir");
来源：http://dpb.svipenyu.cn

[U65] PHP：会话
来源：http://cai.guannengcc.top

session_start();  $_SESSION["uid"] = 1;
来源：http://wnh.vqdsnc.cn

[U66] PHP：设置 Cookie
来源：http://oxi.jianghu66.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ljw.chenzaomai.com

[U67] PHP：处理文件上传
来源：http://spf.vehdjk.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jgc.ybcxt.top

[U68] PHP：PDO 连接
来源：http://gld.zhijiandao.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mfq.zdbjq.cn

[U69] PHP：PDO 预处理
来源：http://vog.shangyingyoupin.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://icb.vqdsnc.cn

[U70] PHP：PDO 事务
来源：http://qxi.yangfankeji.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://yjj.shanyushiyangkeji.top

[U71] PHP：抛出异常
来源：http://gpz.zycfv.cn

throw new RuntimeException("失败", 500);
来源：http://tzk.yj20258888.top

[U72] PHP：写错误日志
来源：http://jxx.bjfxy.top

error_log("失败: " . $e->getMessage());
来源：http://aof.chenlongwang.top

[U73] PHP：读取 ini 配置
来源：http://bce.bbcook.cn

parse_ini_file("config.ini", true)
来源：http://umj.ydzc1.top

[U74] PHP：读取环境变量
来源：http://tet.hnxiangtu.top

getenv("APP_ENV") ?: "production"
来源：http://gos.ywan-chungtsiang.top

[U75] PHP：依赖注入
来源：http://eac.epnwcf.com

composer require psr/container
来源：http://vwc.pycfn.com

[U76] PHP：简单路由
来源：http://qsu.wangshuangyany.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xhv.cqqwz.cn

[U77] PHP：模板渲染
来源：http://keb.yanxiufei.cn

composer require twig/twig
来源：http://yta.ywan-chungtsiang.top

[U78] PHP：单元测试
来源：http://iyk.yangfankeji.com

composer require --dev phpunit/phpunit
来源：http://gjb.redwolf501.top

[U79] PHP：静态分析
来源：http://yaf.fanxiaobao.xyz

composer require --dev phpstan/phpstan
来源：http://mqx.feifeiyinyue.top

[U80] PHP：代码规范修复
来源：http://jza.yj20258.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://pfp.ctjpmb.com

[U81] JS：初始化项目
来源：http://elg.jiagoushi.top

npm init -y;  npm i express
来源：http://pgh.yongpay.top

[U82] JS：package.json 脚本
来源：http://rit.fehbvm.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zve.havefunace.top

[U83] JS：ES Module 导入导出
来源：http://mfo.fktsv.cn

export const a = 1;  import { a } from "./m.js";
来源：http://hod.nwbrower.top

[U84] JS：CommonJS 写法
来源：http://utt.nwbrower.top

module.exports = { a };  const { a } = require("./m");
来源：http://vzo.tianlin.xyz

[U85] JS：可选链
来源：http://ell.pengpengdd.cyou

a?.b?.c
来源：http://dkj.aizwys.cn

[U86] JS：空值合并
来源：http://ytv.yvedp.cn

a ?? b
来源：http://phm.pengpengdd.cyou

[U87] JS：解构默认值
来源：http://eru.ctjpmb.com

const { a = 1, b = 2 } = obj;
来源：http://kaa.cdnleiting.top

[U88] JS：对象展开合并
来源：http://sgk.nanxuanxn.top

{ ...a, ...b }
来源：http://fzv.smart0.xyz

[U89] JS：数组去重
来源：http://yga.gotoacloud.top

[...new Set(arr)]
来源：http://qfn.sweek.top

[U90] JS：数字数组排序
来源：http://uea.cashguo.top

[...arr].sort((a, b) => a - b)
来源：http://rqt.ctjpmb.com

[U91] JS：对象键值遍历
来源：http://nnc.ppjwa.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jms.tarul.cn

[U92] JS：深拷贝
来源：http://ebb.vqdsnc.cn

structuredClone(obj)
来源：http://yga.ctjpmb.com

[U93] JS：模板字符串
来源：http://dem.jqgfzy.top

`共 ${n} 条`
来源：http://kti.zhixingplan.top

[U94] JS：箭头函数
来源：http://txy.shanyushiyangtech.top

const double = x => x * 2;
来源：http://sfb.yangfankeji.com

[U95] JS：Promise 包装
来源：http://yux.tianlin.xyz

new Promise((resolve, reject) => {})
来源：http://mio.0kj1m.cn

[U96] JS：async/await 与异常
来源：http://odp.zhixingplan.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qgb.jinghuilouyu.cn

[U97] JS：并发请求
来源：http://myi.jqgufenzy.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://bkz.316326.xyz

[U98] JS：fetch 带 JSON
来源：http://kks.0kj1m.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ias.wangdashe.top

[U99] JS：事件监听
来源：http://wwq.shangyingyoupin.top

el.addEventListener("click", e => {})
来源：http://ifs.zhaomingkeji.xyz

[U100] JS：DOM 查询
来源：http://rmy.cashguo.top

document.querySelector(".item")
来源：http://xet.redwolf501.top

[U101] JS：classList 操作
来源：http://nyu.cucudq.cn

el.classList.toggle("active")
来源：http://uus.uphjek.com

[U102] JS：本地存储
来源：http://xli.hammf.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://bkz.daria6918.cn

[U103] JS：定时器
来源：http://uzp.sweek.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vwv.zdqjudy.top

[U104] JS：防抖
来源：http://gbt.fengsongda.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yyx.shzxlz.cn

[U105] JS：节流
来源：http://jhz.jinghuilouyu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://twb.sufxvd.cn

[U106] JS：日期格式化
来源：http://fcv.hysaishi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qam.bjfxy.top

[U107] JS：数字千分位
来源：http://bpt.vqdsnc.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://uxg.zhijiandao.cn

[U108] JS：随机整数
来源：http://gun.vehdjk.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wrc.svipenyu.cn

[U109] JS：数组分组
来源：http://col.yuxming.cn

Object.groupBy(arr, x => x.type)
来源：http://ebm.zhijiandao.cn

[U110] JS：数组分块
来源：http://wid.andypj.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qxi.jlsjyb.cn

[U111] JS：对象转 Map
来源：http://jgd.sxryk.cn

new Map(Object.entries(obj))
来源：http://pjq.fktsv.cn

[U112] JS：字符串补位
来源：http://giu.quarkkingdee.top

"7".padStart(3, "0")
来源：http://jxd.hammf.cn

[U113] JS：正则替换全部
来源：http://cvb.jyoumei.cn

s.replaceAll("a", "b")
来源：http://viy.quarkkingdee.top

[U114] JS：JSON 深比较
来源：http://npj.ydjk.org.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://oxm.hammf.cn

[U115] JS：生成 UUID
来源：http://weo.yuxming.cn

crypto.randomUUID()
来源：http://tnz.jinqigfzy.top

[U116] JS：类型检查（JSDoc）
来源：http://jpr.shzxlz.cn

/** @param {string} name */ function f(name) {}
来源：http://cpx.hesvh.cn

[U117] JS：单元测试
来源：http://uqu.zhaomingkeji.xyz

npm i -D vitest;  npx vitest
来源：http://aqr.bbcook.cn

[U118] JS：开发服务器
来源：http://owh.xylfe.cn

npm i -D vite;  npx vite
来源：http://vga.chenjidiqi.icu

[U119] JS：生产构建
来源：http://xzs.yonumen.top

npx vite build
来源：http://dwe.feifeiyinyue.top

[U120] JS：读取环境变量（Vite）
来源：http://wwn.havefunace.top

import.meta.env.VITE_API_URL
来源：http://kat.chenjidiqi.icu

================================================================================
来源：http://ueq.kuanghao11.cn

统计汇总
来源：http://yqv.bjfxy.top

================================================================================
来源：http://rpt.pengpengdd.cyou

按语言统计（条）：
来源：http://rau.cashguo.top

Python ......... 252
来源：http://pmh.yuanzhike.top

PHP ............ 252
来源：http://xsg.yanxiufei.cn

JavaScript ..... 252
来源：http://kwm.jianghu66.top

TypeScript ..... 212
来源：http://wpq.kuanghao11.cn

Java ........... 212
来源：http://vae.fengsongda.top

Go ............. 212
来源：http://cgs.yj202588.top

Ruby ........... 212
来源：http://tgs.zdbjq.cn

C# ............. 212
来源：http://ini.zhongyouzk.top

C .............. 30
来源：http://snh.cheryme.top

C++ ............ 30
来源：http://ufr.andypj.xyz

SQL ............ 90
来源：http://vxp.hnqzz.top

Bash ........... 80
来源：http://igq.zhaomingkeji.xyz

Kotlin ......... 15
来源：http://lov.0kj1m.cn

Swift .......... 15
来源：http://vqd.gogol.net.cn

Lua ............ 10
来源：http://wxu.ydzc1.top

Perl ........... 10
来源：http://jat.hammf.cn

Scala .......... 10
来源：http://dco.zdbjq.cn

------------------------------------
来源：http://zgc.shanyushiyangkeji.top

合计 ........... 2106 条
来源：http://eda.daria6918.cn

按章节统计：
来源：http://cyb.sufxvd.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ane.hcnkem.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://pmc.yongpay.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://sao.hongshengwenyu.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://aaj.daria6918.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pis.sufxvd.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://fqe.gaohongyu789.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jft.yueranfly.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://bos.tianlin.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://fsh.zhixingplan.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://cal.tarul.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xqf.yvedp.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://neg.iojbl.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ovp.shuidangran.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ocx.meibo888.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wuq.hongshengwenyu.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://cmp.yueranfly.top

Q SQL 专题                              90
来源：http://rcu.zhaomingkeji.xyz

R Bash 专题                             80
来源：http://ekh.meibo888.top

S C / C++ 专题                          60
来源：http://hmd.yonumen.top

T 其他语言补充                          60
来源：http://ffs.gzhubu.top

U 高频实用片段                         120
来源：http://juj.tian-w.cn

------------------------------------
来源：http://vtn.xinyue.icu

合计                                  2106 条
来源：http://ubo.gotoacloud.top

--------------------------------------------------------------------------------
来源：http://lvu.shuidangran.top

使用提醒
来源：http://rwj.bbcook.cn

--------------------------------------------------------------------------------
来源：http://lpy.hnqzz.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xmk.0kj1m.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bgz.wangdashe.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xsh.nanxuanxn.top

在旧版本上使用前请先确认语法支持情况。
来源：http://yan.jqgfzy.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://sxj.xziqi.cn

—— 文件结束 ——
来源：http://hbj.svipenyu.cn

================================================================================
来源：http://bww.andypj.xyz

程序语言常见例子速查手册（2024 版）
来源：http://gmr.yuxming.cn

Common Programming Examples Cheat Book
来源：http://jub.hnxiangtu.top

================================================================================
来源：http://ylv.zhengqikj.top

【收录内容】
来源：http://yae.xylfe.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://imb.hongshengwenyu.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://gem.ctjpmb.com

SQL · Bash · C · C++
来源：http://ksd.ivvv.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://riy.pycfn.com

【使用说明】
来源：http://kfi.yj20258.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ubn.fehbvm.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vlz.zhixingplan.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://beg.hnxiangtu.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wok.feifeiyinyue.top

Bash:  Shell         C:     C             C++:   C++
来源：http://lxa.yj202588.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://gwp.wangdashe.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ykz.wangdashe.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://pdk.xingfuxueyuan.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://kuv.yuxming.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ulw.svipenyu.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://tcf.cheryme.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://tvt.fktsv.cn

【文件统计】
来源：http://lka.xuanzx.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://sri.yj20258888.top

--------------------------------------------------------------------------------
来源：http://sxk.ctjpmb.com

目  录
来源：http://fev.ybcxt.top

--------------------------------------------------------------------------------
来源：http://xeh.nanxinkj.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fmh.gzhubu.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qab.jinyuanbaomall.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://yzn.shangyingyoupin.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://uvr.hfpthk.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jvv.gotoacloud.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ngb.ivvv.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://kno.hysaishi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qxw.pycfn.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://han.ybcxt.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://tpf.316326.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://dmh.jlsjyb.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ibq.sufxvd.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://zdt.tarul.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://yui.nanxuanxn.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wzv.xuanzx.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hef.xuanzx.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://sgo.aizwys.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://qob.jyoumei.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rdg.yuxming.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ziw.cashguo.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://yzj.yuanzhike.top

================================================================================
来源：http://yud.sysykeji.top

A. 基础语法与类型
来源：http://tnb.hcnkem.com

================================================================================
来源：http://czk.c1oappe.top

[A01] Hello World
来源：http://hkb.jyoumei.cn

Py:   print("Hello, World!")
来源：http://seb.yvedp.cn

PHP:  echo "Hello, World!";
来源：http://vle.jinghuilouyu.cn

JS:   console.log("Hello, World!");
来源：http://jgw.ywan-chungtsiang.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://xqd.tian-w.cn

Java: System.out.println("Hello, World!");
来源：http://qil.sufxvd.cn

Go:   fmt.Println("Hello, World!")
来源：http://rjz.jinyuanbaomall.cn

Ruby: puts "Hello, World!"
来源：http://jyo.bjfxy.top

C#:   Console.WriteLine("Hello, World!");
来源：http://ddo.hnqzz.top

[A02] 变量声明与赋值
来源：http://fqb.cheryme.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://iaa.cucudq.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://koy.dianchejie.cn

JS:   let name = "Alex"; const age = 20;
来源：http://fqq.zhengqikj.top


<!-- 参考信息 -->