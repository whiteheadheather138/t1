代发 wailian999

[U31] Py：单测
来源：http://isp.ctjpmb.com

python -m pytest -q
来源：http://yin.xuanzx.com

[U32] Py：代码格式化
来源：http://bfi.vqdsnc.cn

ruff format . && ruff check --fix .
来源：http://zvp.fehbvm.com

[U33] Py：打包发布
来源：http://xcz.shanyushiyangtech.top

python -m build  （依赖 pyproject.toml）
来源：http://vpg.hfpthk.cn

[U34] Py：判断编码
来源：http://cpm.c1oappe.top

chardet.detect(raw)
来源：http://bjg.ywan-chungtsiang.top

[U35] Py：发送邮件
来源：http://bxa.yuxming.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fea.epnwcf.com

[U36] Py：定时任务
来源：http://aze.chenlongwang.top

schedule.every(10).minutes.do(job)
来源：http://tya.ppjwa.cn

[U37] Py：读写 Excel
来源：http://tbn.shanyushiyangtech.top

pandas.read_excel / DataFrame.to_excel
来源：http://suw.shuidangran.top

[U38] Py：获取脚本所在目录
来源：http://mtp.cdnleiting.top

Path(__file__).resolve().parent
来源：http://plo.cheryme.top

[U39] Py：判断是否在交互环境
来源：http://zvx.gzhubu.top

sys.stdout.isatty()
来源：http://uxn.ctjpmb.com

[U40] Py：打印到标准错误
来源：http://gzf.jqgfzy.top

print("err", file=sys.stderr)
来源：http://vgd.dianchejie.cn

[U41] PHP：初始化 Composer 项目
来源：http://yqw.tian-w.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ohk.sweek.top

[U42] PHP：PSR-4 自动加载
来源：http://sao.gogol.net.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rtj.yj202588.top

[U43] PHP：声明命名空间
来源：http://yhw.hnqzz.top

namespace App\Http;
来源：http://emt.fehbvm.com

[U44] PHP：开启严格类型
来源：http://gut.ctjpmb.com

declare(strict_types=1);
来源：http://jkq.uphjek.com

[U45] PHP：类型声明与返回类型
来源：http://tlu.kuanghao11.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://dno.hcnkem.com

[U46] PHP：可空类型
来源：http://hem.sweek.top

?string $name = null
来源：http://mzi.aizwys.cn

[U47] PHP：联合类型
来源：http://zck.shuidangran.top

int|string $id
来源：http://art.jianghu66.top

[U48] PHP：纯枚举
来源：http://ped.iojbl.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wye.quarkkingdee.top

[U49] PHP：只读属性
来源：http://eea.nanxuanxn.top

public readonly string $name
来源：http://muh.jinyuanbaomall.cn

[U50] PHP：构造器属性提升
来源：http://tle.zhoulong.xyz

public function __construct(private int $id) {}
来源：http://xfw.feifeiyinyue.top

[U51] PHP：数组解构
来源：http://bej.daria6918.cn

[$a, $b] = $arr;
来源：http://qgo.sweek.top

[U52] PHP：箭头函数
来源：http://bof.sweek.top

$double = fn($x) => $x * 2;
来源：http://riv.sxryk.cn

[U53] PHP：空合并运算符
来源：http://ylk.zhiwuduotai.top

$v = $a ?? $b ?? "default";
来源：http://scb.wangshuangyany.cn

[U54] PHP：空安全调用
来源：http://teg.jiagoushi.top

$obj?->method()
来源：http://jux.zdqjudy.top

[U55] PHP：match 表达式
来源：http://wfu.hcnkem.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://czw.ydzc1.top

[U56] PHP：命名参数
来源：http://tnz.shangyingyoupin.top

f(a: 1, b: 2)
来源：http://ibe.redwolf501.top

[U57] PHP：字符串插值
来源：http://vtq.yuanzhike.top

"值: {$a}"
来源：http://yzs.tarul.cn

[U58] PHP：数组三件套
来源：http://hye.c1oappe.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xtu.fehbvm.com

[U59] PHP：自定义排序
来源：http://rvn.shangyingyoupin.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wcr.shangyingyoupin.top

[U60] PHP：JSON 编解码
来源：http://xii.sxryk.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://sdh.wangshuangyany.cn

[U61] PHP：正则
来源：http://upq.xinyue.icu

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kjc.ivvv.top

[U62] PHP：日期对象
来源：http://tto.guannengcc.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://geg.zhongyouzk.top

[U63] PHP：文件读写
来源：http://dva.ctjpmb.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zgy.xuetiantiany.cn

[U64] PHP：目录遍历
来源：http://ott.hongshengwenyu.top

glob("dir/*.php");  scandir("dir");
来源：http://gzk.ivvv.top

[U65] PHP：会话
来源：http://mmj.hysaishi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://lvx.haohaochexian.top

[U66] PHP：设置 Cookie
来源：http://pph.yonumen.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fou.yj20258.top

[U67] PHP：处理文件上传
来源：http://dte.cqqwz.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lsn.zhongyouzk.top

[U68] PHP：PDO 连接
来源：http://lvr.jianghu66.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://aun.gotoacloud.top

[U69] PHP：PDO 预处理
来源：http://haz.fzhhl.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nbl.feifeiyinyue.top

[U70] PHP：PDO 事务
来源：http://sct.fehbvm.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nrr.hnqzz.top

[U71] PHP：抛出异常
来源：http://elg.gogol.net.cn

throw new RuntimeException("失败", 500);
来源：http://kqq.ywan-chungtsiang.top

[U72] PHP：写错误日志
来源：http://iti.nanxuanxn.top

error_log("失败: " . $e->getMessage());
来源：http://mii.uphjek.com

[U73] PHP：读取 ini 配置
来源：http://gxz.sweek.top

parse_ini_file("config.ini", true)
来源：http://cga.hfpthk.cn

[U74] PHP：读取环境变量
来源：http://thi.tian-w.cn

getenv("APP_ENV") ?: "production"
来源：http://yls.ivvv.top

[U75] PHP：依赖注入
来源：http://hww.shzxlz.cn

composer require psr/container
来源：http://bbp.shzxlz.cn

[U76] PHP：简单路由
来源：http://zvr.andypj.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://asq.bbcook.cn

[U77] PHP：模板渲染
来源：http://gfc.jlsjyb.cn

composer require twig/twig
来源：http://gop.sysykeji.top

[U78] PHP：单元测试
来源：http://rkt.xylfe.cn

composer require --dev phpunit/phpunit
来源：http://map.jinyuanbaomall.cn

[U79] PHP：静态分析
来源：http://vcc.52xcode.cn

composer require --dev phpstan/phpstan
来源：http://hzh.yj202588.top

[U80] PHP：代码规范修复
来源：http://qox.yongpay.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://hrh.sxryk.cn

[U81] JS：初始化项目
来源：http://zhi.hywenlv.cn

npm init -y;  npm i express
来源：http://ncn.snrcjt.cn

[U82] JS：package.json 脚本
来源：http://jan.birdmap.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ofu.andypj.xyz

[U83] JS：ES Module 导入导出
来源：http://vmr.meibo888.top

export const a = 1;  import { a } from "./m.js";
来源：http://vjw.cheryme.top

[U84] JS：CommonJS 写法
来源：http://ags.shzxlz.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ses.vqdsnc.cn

[U85] JS：可选链
来源：http://maj.yvedp.cn

a?.b?.c
来源：http://zjp.kuanghao11.cn

[U86] JS：空值合并
来源：http://kgl.sxryk.cn

a ?? b
来源：http://lrv.bjfxy.top

[U87] JS：解构默认值
来源：http://mke.nanxinkj.top

const { a = 1, b = 2 } = obj;
来源：http://sij.cashguo.top

[U88] JS：对象展开合并
来源：http://xpf.sxryk.cn

{ ...a, ...b }
来源：http://jpj.mhx1999.top

[U89] JS：数组去重
来源：http://fyw.jlsjyb.cn

[...new Set(arr)]
来源：http://azh.jyoumei.cn

[U90] JS：数字数组排序
来源：http://wtj.fktsv.cn

[...arr].sort((a, b) => a - b)
来源：http://tcs.ybcxt.top

[U91] JS：对象键值遍历
来源：http://osu.fengsongda.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tqj.yj20258888.top

[U92] JS：深拷贝
来源：http://ysb.jiagoushi.top

structuredClone(obj)
来源：http://giz.gotoacloud.top

[U93] JS：模板字符串
来源：http://kek.nwbrower.top

`共 ${n} 条`
来源：http://hqw.jlsjyb.cn

[U94] JS：箭头函数
来源：http://hcp.zhengqikj.top

const double = x => x * 2;
来源：http://ikd.yj202588.top

[U95] JS：Promise 包装
来源：http://sry.jinqigfzy.top

new Promise((resolve, reject) => {})
来源：http://fus.smart0.xyz

[U96] JS：async/await 与异常
来源：http://lyo.hammf.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qft.sufxvd.cn

[U97] JS：并发请求
来源：http://qfo.chenjidiqi.icu

await Promise.all(urls.map(u => fetch(u)))
来源：http://cdj.sjlbkw.cn

[U98] JS：fetch 带 JSON
来源：http://tgf.daria6918.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://arf.iojbl.cn

[U99] JS：事件监听
来源：http://idv.jiagoushi.top

el.addEventListener("click", e => {})
来源：http://ypf.yuxming.cn

[U100] JS：DOM 查询
来源：http://kfs.svipenyu.cn

document.querySelector(".item")
来源：http://dfc.nwbrower.top

[U101] JS：classList 操作
来源：http://cbq.quarkkingdee.top

el.classList.toggle("active")
来源：http://hbz.feifeiyinyue.top

[U102] JS：本地存储
来源：http://ogr.jqgufenzy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://cak.zhixingplan.top

[U103] JS：定时器
来源：http://rji.ctjpmb.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wyk.vehdjk.com

[U104] JS：防抖
来源：http://ctc.epnwcf.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vbw.hcnkem.com

[U105] JS：节流
来源：http://gqh.shanyushiyangkeji.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xii.nanxinkj.top

[U106] JS：日期格式化
来源：http://wva.fengsongda.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fpw.hesvh.cn

[U107] JS：数字千分位
来源：http://vta.tarul.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wsu.shangyingyoupin.top

[U108] JS：随机整数
来源：http://mnu.havefunace.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xzb.gotoacloud.top

[U109] JS：数组分组
来源：http://zdb.gzhubu.top

Object.groupBy(arr, x => x.type)
来源：http://ogr.cucudq.cn

[U110] JS：数组分块
来源：http://svb.cashguo.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dhe.fktsv.cn

[U111] JS：对象转 Map
来源：http://bqq.sufxvd.cn

new Map(Object.entries(obj))
来源：http://cyo.fengsongda.top

[U112] JS：字符串补位
来源：http://uai.fktsv.cn

"7".padStart(3, "0")
来源：http://hwg.guowangkeji.top

[U113] JS：正则替换全部
来源：http://shl.fehbvm.com

s.replaceAll("a", "b")
来源：http://nvx.hfpthk.cn

[U114] JS：JSON 深比较
来源：http://gja.yuanzhike.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://urr.nanxinkj.top

[U115] JS：生成 UUID
来源：http://uam.zhiwuduotai.top

crypto.randomUUID()
来源：http://jla.vqdsnc.cn

[U116] JS：类型检查（JSDoc）
来源：http://uwx.zycfv.cn

/** @param {string} name */ function f(name) {}
来源：http://gnl.andypj.xyz

[U117] JS：单元测试
来源：http://nor.shanyushiyangtech.top

npm i -D vitest;  npx vitest
来源：http://bfl.jyoumei.cn

[U118] JS：开发服务器
来源：http://zxl.xuanzx.com

npm i -D vite;  npx vite
来源：http://eyx.jqgfzy.top

[U119] JS：生产构建
来源：http://jkr.hnxiangtu.top

npx vite build
来源：http://ajd.yvedp.cn

[U120] JS：读取环境变量（Vite）
来源：http://nzr.jianghu66.top

import.meta.env.VITE_API_URL
来源：http://oug.tanke756.top

================================================================================
来源：http://ytw.fanxiaobao.xyz

统计汇总
来源：http://uwa.smart0.xyz

================================================================================
来源：http://occ.xylfe.cn

按语言统计（条）：
来源：http://yyu.yueranfly.top

Python ......... 252
来源：http://ned.vqdsnc.cn

PHP ............ 252
来源：http://azv.andypj.xyz

JavaScript ..... 252
来源：http://gaw.jyoumei.cn

TypeScript ..... 212
来源：http://lpq.tianlin.xyz

Java ........... 212
来源：http://qpq.hesvh.cn

Go ............. 212
来源：http://ibl.gogol.net.cn

Ruby ........... 212
来源：http://drz.gogol.net.cn

C# ............. 212
来源：http://kse.vehdjk.com

C .............. 30
来源：http://skw.vqdsnc.cn

C++ ............ 30
来源：http://bdz.hnqzz.top

SQL ............ 90
来源：http://cid.jqgfzy.top

Bash ........... 80
来源：http://fcm.shanyushiyangkeji.top

Kotlin ......... 15
来源：http://snb.ctjpmb.com

Swift .......... 15
来源：http://lot.sweek.top

Lua ............ 10
来源：http://tkg.pengpengdd.cyou

Perl ........... 10
来源：http://iqk.aibaodan.cn

Scala .......... 10
来源：http://esa.shanyushiyangkeji.top

------------------------------------
来源：http://elh.guannengcc.top

合计 ........... 2106 条
来源：http://wzi.mhx1999.top

按章节统计：
来源：http://vyx.316326.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://arv.iojbl.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://saf.tanke756.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jco.chenjidiqi.icu

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rmv.zhongyouzk.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://lvc.jinqigufen.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://sgt.zhongyouzk.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://lqj.fengsongda.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://byh.wangshuangyany.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ert.jinqigufen.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rsk.jinyuanbaomall.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://tcf.tian-w.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kyw.0kj1m.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://pth.jinyuanbaomall.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://gpm.yongpay.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://kzc.sjlbkw.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://yqj.yuanzhike.top

Q SQL 专题                              90
来源：http://bfg.cashguo.top

R Bash 专题                             80
来源：http://eje.jlsjyb.cn

S C / C++ 专题                          60
来源：http://vcy.hnqzz.top

T 其他语言补充                          60
来源：http://ogt.316326.xyz

U 高频实用片段                         120
来源：http://oao.vqdsnc.cn

------------------------------------
来源：http://rbo.sufxvd.cn

合计                                  2106 条
来源：http://yte.guannengcc.top

--------------------------------------------------------------------------------
来源：http://njc.shuidangran.top

使用提醒
来源：http://kyj.sjlbkw.cn

--------------------------------------------------------------------------------
来源：http://ogi.ppjwa.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ubo.zhengqikj.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://nxf.iojbl.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://brh.gotoacloud.top

在旧版本上使用前请先确认语法支持情况。
来源：http://zsc.smart0.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hxr.9152youxi.cn

—— 文件结束 ——
来源：http://gnr.kuanghao11.cn

================================================================================
来源：http://rhs.zhiwuduotai.top

程序语言常见例子速查手册（2024 版）
来源：http://zbc.shzxlz.cn

Common Programming Examples Cheat Book
来源：http://lwb.shzxlz.cn

================================================================================
来源：http://aaq.haohaochexian.top

【收录内容】
来源：http://ajq.xylfe.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://tja.sweek.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://isw.sjlbkw.cn

SQL · Bash · C · C++
来源：http://bnv.hammf.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ccc.feifeiyinyue.top

【使用说明】
来源：http://rgo.iojbl.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://lrq.hfpthk.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ilu.dashuyun.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://tqo.yangfankeji.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://jpa.c1oappe.top

Bash:  Shell         C:     C             C++:   C++
来源：http://yln.zhengqikj.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://pei.ctjpmb.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://zfg.xinyue.icu

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ivr.tianlin.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://uef.redwolf501.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://tqa.hnxiangtu.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ctw.sjlbkw.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://cgj.aizwys.cn

【文件统计】
来源：http://hlh.shuidangran.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://dje.yj202588.top

--------------------------------------------------------------------------------
来源：http://ckn.c1oappe.top

目  录
来源：http://wwp.bjfxy.top

--------------------------------------------------------------------------------
来源：http://yjd.yfazqb.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qka.zhengqikj.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://khc.ywan-chungtsiang.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://gwb.smart0.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wyc.fengsongda.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ibj.zhijiandao.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://obd.cucudq.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qzi.ywan-chungtsiang.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xbv.jinqigufen.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://gic.ybcxt.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xux.jinqigufen.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://fba.jlsjyb.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hcs.yvedp.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qqv.fktsv.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ztu.xinyue.icu

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://fmg.nanxinkj.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://jia.yueranfly.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://kgt.hnxiangtu.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://xzq.yuxming.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qyd.yonumen.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qmx.yuanzhike.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xpt.shanyushiyangkeji.top

================================================================================
来源：http://omf.jqgufenzy.top

A. 基础语法与类型
来源：http://gkk.bbcook.cn

================================================================================
来源：http://dst.jianghu66.top

[A01] Hello World
来源：http://bqp.yuanzhike.top

Py:   print("Hello, World!")
来源：http://nbx.iojbl.cn

PHP:  echo "Hello, World!";
来源：http://gpy.bjfxy.top

JS:   console.log("Hello, World!");
来源：http://kkm.shangyingyoupin.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://xil.guowangkeji.top

Java: System.out.println("Hello, World!");
来源：http://rox.tarul.cn

Go:   fmt.Println("Hello, World!")
来源：http://uef.shuidangran.top

Ruby: puts "Hello, World!"
来源：http://iqz.yuxming.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://xwl.birdmap.top

[A02] 变量声明与赋值
来源：http://kan.jinqigfzy.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wxl.xinyue.icu

PHP:  $name = "Alex"; $age = 20;
来源：http://deo.tianlin.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://jrx.sxryk.cn


<!-- 参考信息 -->