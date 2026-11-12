代发 wailian999

[U27] Py：异步 HTTP
来源：http://xki.iojbl.cn

aiohttp.ClientSession() 配合 async with
来源：http://fyo.fanxiaobao.xyz

[U28] Py：类型别名
来源：http://mns.chenzaomai.com

UserId = int
来源：http://bka.yueranfly.top

[U29] Py：属性校验
来源：http://hqd.hnxiangtu.top

@property 与 @x.setter 配合
来源：http://vug.bjfxy.top

[U30] Py：数据类
来源：http://fdp.yonumen.top

@dataclass(slots=True)
来源：http://xvm.nanxuanxn.top

[U31] Py：单测
来源：http://ofq.fehbvm.com

python -m pytest -q
来源：http://naf.c1oappe.top

[U32] Py：代码格式化
来源：http://qkv.9152youxi.cn

ruff format . && ruff check --fix .
来源：http://kdz.ppjwa.cn

[U33] Py：打包发布
来源：http://uri.aizwys.cn

python -m build  （依赖 pyproject.toml）
来源：http://shr.redwolf501.top

[U34] Py：判断编码
来源：http://nzh.vqdsnc.cn

chardet.detect(raw)
来源：http://dlo.uphjek.com

[U35] Py：发送邮件
来源：http://hws.xuetiantiany.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://oys.pycfn.com

[U36] Py：定时任务
来源：http://swr.smart0.xyz

schedule.every(10).minutes.do(job)
来源：http://pof.sxryk.cn

[U37] Py：读写 Excel
来源：http://qup.ppjwa.cn

pandas.read_excel / DataFrame.to_excel
来源：http://eii.nanxuanxn.top

[U38] Py：获取脚本所在目录
来源：http://prs.dianchejie.cn

Path(__file__).resolve().parent
来源：http://mcx.uphjek.com

[U39] Py：判断是否在交互环境
来源：http://svz.gogol.net.cn

sys.stdout.isatty()
来源：http://vej.zycfv.cn

[U40] Py：打印到标准错误
来源：http://klv.yj20258.top

print("err", file=sys.stderr)
来源：http://aox.xylfe.cn

[U41] PHP：初始化 Composer 项目
来源：http://kpi.c1oappe.top

composer init;  composer require guzzlehttp/guzzle
来源：http://vye.aizwys.cn

[U42] PHP：PSR-4 自动加载
来源：http://nzu.hcnkem.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ona.cdnleiting.top

[U43] PHP：声明命名空间
来源：http://kor.cucudq.cn

namespace App\Http;
来源：http://wrd.pengpengdd.cyou

[U44] PHP：开启严格类型
来源：http://qpl.jlsjyb.cn

declare(strict_types=1);
来源：http://cqb.ydzc1.top

[U45] PHP：类型声明与返回类型
来源：http://kuj.havefunace.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://swu.aibaodan.cn

[U46] PHP：可空类型
来源：http://mtb.0kj1m.cn

?string $name = null
来源：http://ael.zdbjq.cn

[U47] PHP：联合类型
来源：http://jad.mhx1999.top

int|string $id
来源：http://dxb.meibo888.top

[U48] PHP：纯枚举
来源：http://xmr.jinqigfzy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zpg.jqgufenzy.top

[U49] PHP：只读属性
来源：http://zee.andypj.xyz

public readonly string $name
来源：http://noa.jqgufenzy.top

[U50] PHP：构造器属性提升
来源：http://lpc.9152youxi.cn

public function __construct(private int $id) {}
来源：http://tvt.jqgufenzy.top

[U51] PHP：数组解构
来源：http://ztq.fzhhl.top

[$a, $b] = $arr;
来源：http://cdv.yangfankeji.com

[U52] PHP：箭头函数
来源：http://zyp.chenjidiqi.icu

$double = fn($x) => $x * 2;
来源：http://hzs.wangdashe.top

[U53] PHP：空合并运算符
来源：http://mbj.aibaodan.cn

$v = $a ?? $b ?? "default";
来源：http://lyh.zhaomingkeji.xyz

[U54] PHP：空安全调用
来源：http://bvb.hnqzz.top

$obj?->method()
来源：http://ljd.chenzaomai.com

[U55] PHP：match 表达式
来源：http://ena.chenzaomai.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://snf.sufxvd.cn

[U56] PHP：命名参数
来源：http://tro.birdmap.top

f(a: 1, b: 2)
来源：http://qac.hesvh.cn

[U57] PHP：字符串插值
来源：http://dsz.xingfuxueyuan.xyz

"值: {$a}"
来源：http://ntv.yuxming.cn

[U58] PHP：数组三件套
来源：http://cxx.shangyingyoupin.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kei.ehwqpu.com

[U59] PHP：自定义排序
来源：http://tvr.xuanzx.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://eeb.cdnleiting.top

[U60] PHP：JSON 编解码
来源：http://ulg.jiagoushi.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pci.jqgfzy.top

[U61] PHP：正则
来源：http://kfh.zycfv.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pqp.hywenlv.cn

[U62] PHP：日期对象
来源：http://szj.ctjpmb.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xxy.xylfe.cn

[U63] PHP：文件读写
来源：http://tya.yueranfly.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bjo.gogol.net.cn

[U64] PHP：目录遍历
来源：http://lgo.zdbjq.cn

glob("dir/*.php");  scandir("dir");
来源：http://gpj.yueranfly.top

[U65] PHP：会话
来源：http://vlt.hysaishi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://cmr.chenzaomai.com

[U66] PHP：设置 Cookie
来源：http://gpk.vqdsnc.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kqa.sysykeji.top

[U67] PHP：处理文件上传
来源：http://ndx.iojbl.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vmb.fanxiaobao.xyz

[U68] PHP：PDO 连接
来源：http://wgg.daria6918.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rjm.nanxuanxn.top

[U69] PHP：PDO 预处理
来源：http://izw.daria6918.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wdo.hnxiangtu.top

[U70] PHP：PDO 事务
来源：http://are.tarul.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gpq.jinghuilouyu.cn

[U71] PHP：抛出异常
来源：http://xpn.yonumen.top

throw new RuntimeException("失败", 500);
来源：http://uxm.cucudq.cn

[U72] PHP：写错误日志
来源：http://pzx.havefunace.top

error_log("失败: " . $e->getMessage());
来源：http://zdw.jinqigfzy.top

[U73] PHP：读取 ini 配置
来源：http://xvk.shanyushiyangkeji.top

parse_ini_file("config.ini", true)
来源：http://ned.vqdsnc.cn

[U74] PHP：读取环境变量
来源：http://zbi.yanxiufei.cn

getenv("APP_ENV") ?: "production"
来源：http://gtz.sysykeji.top

[U75] PHP：依赖注入
来源：http://kfl.daria6918.cn

composer require psr/container
来源：http://sqa.ivvv.top

[U76] PHP：简单路由
来源：http://nfc.birdmap.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://stj.mhx1999.top

[U77] PHP：模板渲染
来源：http://uxk.fktsv.cn

composer require twig/twig
来源：http://qbp.ppjwa.cn

[U78] PHP：单元测试
来源：http://giq.daria6918.cn

composer require --dev phpunit/phpunit
来源：http://cfo.yongpay.top

[U79] PHP：静态分析
来源：http://abs.yj20258888.top

composer require --dev phpstan/phpstan
来源：http://qih.jinqigfzy.top

[U80] PHP：代码规范修复
来源：http://pep.gzhubu.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://rfe.shzxlz.cn

[U81] JS：初始化项目
来源：http://tjh.xingfuxueyuan.xyz

npm init -y;  npm i express
来源：http://zcx.gaohongyu789.top

[U82] JS：package.json 脚本
来源：http://jiy.shangyingyoupin.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jgf.yongpay.top

[U83] JS：ES Module 导入导出
来源：http://hkv.9152youxi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://xns.yj20258888.top

[U84] JS：CommonJS 写法
来源：http://bnh.9152youxi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://psm.jqgufenzy.top

[U85] JS：可选链
来源：http://tdg.hongshengwenyu.top

a?.b?.c
来源：http://qcl.9152youxi.cn

[U86] JS：空值合并
来源：http://qqg.iojbl.cn

a ?? b
来源：http://ujh.gaohongyu789.top

[U87] JS：解构默认值
来源：http://xqm.ybcxt.top

const { a = 1, b = 2 } = obj;
来源：http://mqw.fehbvm.com

[U88] JS：对象展开合并
来源：http://bgw.haohaochexian.top

{ ...a, ...b }
来源：http://nmf.hfpthk.cn

[U89] JS：数组去重
来源：http://hsq.bjfxy.top

[...new Set(arr)]
来源：http://lfm.9152youxi.cn

[U90] JS：数字数组排序
来源：http://uel.redwolf501.top

[...arr].sort((a, b) => a - b)
来源：http://lis.hcnkem.com

[U91] JS：对象键值遍历
来源：http://hwn.jinyuanbaomall.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mam.sjlbkw.cn

[U92] JS：深拷贝
来源：http://ivb.iojbl.cn

structuredClone(obj)
来源：http://aup.shanyushiyangkeji.top

[U93] JS：模板字符串
来源：http://ojw.ydzc1.top

`共 ${n} 条`
来源：http://mzt.shanyushiyangtech.top

[U94] JS：箭头函数
来源：http://cvk.nanxinkj.top

const double = x => x * 2;
来源：http://txj.sweek.top

[U95] JS：Promise 包装
来源：http://qrp.shanyushiyangtech.top

new Promise((resolve, reject) => {})
来源：http://gjw.jyoumei.cn

[U96] JS：async/await 与异常
来源：http://auh.zhengqikj.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://utj.chenjidiqi.icu

[U97] JS：并发请求
来源：http://hsq.sxryk.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://aqj.jlsjyb.cn

[U98] JS：fetch 带 JSON
来源：http://sik.shzxlz.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fwa.mhx1999.top

[U99] JS：事件监听
来源：http://rxs.fktsv.cn

el.addEventListener("click", e => {})
来源：http://aan.sysykeji.top

[U100] JS：DOM 查询
来源：http://oyk.jianghu66.top

document.querySelector(".item")
来源：http://gsk.sysykeji.top

[U101] JS：classList 操作
来源：http://bcr.gogol.net.cn

el.classList.toggle("active")
来源：http://hgs.0kj1m.cn

[U102] JS：本地存储
来源：http://plq.xuanzx.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://ctj.hongshengwenyu.top

[U103] JS：定时器
来源：http://tdd.ywan-chungtsiang.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ake.zhixingplan.top

[U104] JS：防抖
来源：http://pzz.yj20258.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wag.hesvh.cn

[U105] JS：节流
来源：http://vhq.wangshuangyany.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yci.kuanghao11.cn

[U106] JS：日期格式化
来源：http://fzb.zdqjudy.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://iua.tian-w.cn

[U107] JS：数字千分位
来源：http://egr.sxryk.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://eqg.havefunace.top

[U108] JS：随机整数
来源：http://god.sufxvd.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bhf.fzhhl.top

[U109] JS：数组分组
来源：http://wih.aibaodan.cn

Object.groupBy(arr, x => x.type)
来源：http://rjv.yueranfly.top

[U110] JS：数组分块
来源：http://kll.dianchejie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pcr.jiagoushi.top

[U111] JS：对象转 Map
来源：http://nph.kuanghao11.cn

new Map(Object.entries(obj))
来源：http://lij.zhoulong.xyz

[U112] JS：字符串补位
来源：http://qhk.vqdsnc.cn

"7".padStart(3, "0")
来源：http://fdi.hywenlv.cn

[U113] JS：正则替换全部
来源：http://njs.ywan-chungtsiang.top

s.replaceAll("a", "b")
来源：http://duu.tanke756.top

[U114] JS：JSON 深比较
来源：http://wxl.zdqjudy.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://hgd.ivvv.top

[U115] JS：生成 UUID
来源：http://xna.guannengcc.top

crypto.randomUUID()
来源：http://obq.nwbrower.top

[U116] JS：类型检查（JSDoc）
来源：http://mzx.dashuyun.cn

/** @param {string} name */ function f(name) {}
来源：http://elv.haohaochexian.top

[U117] JS：单元测试
来源：http://crc.xuanzx.com

npm i -D vitest;  npx vitest
来源：http://zqh.snrcjt.cn

[U118] JS：开发服务器
来源：http://bdx.zycfv.cn

npm i -D vite;  npx vite
来源：http://ogb.yj20258888.top

[U119] JS：生产构建
来源：http://umm.guannengcc.top

npx vite build
来源：http://emv.nwbrower.top

[U120] JS：读取环境变量（Vite）
来源：http://mlp.jianghu66.top

import.meta.env.VITE_API_URL
来源：http://ecb.cheryme.top

================================================================================
来源：http://znx.fktsv.cn

统计汇总
来源：http://eiw.tian-w.cn

================================================================================
来源：http://bfa.zhiwuduotai.top

按语言统计（条）：
来源：http://gvz.shangyingyoupin.top

Python ......... 252
来源：http://lif.zhoulong.xyz

PHP ............ 252
来源：http://eby.jinyuanbaomall.cn

JavaScript ..... 252
来源：http://cya.yfazqb.com

TypeScript ..... 212
来源：http://wqb.jianghu66.top

Java ........... 212
来源：http://grr.xziqi.cn

Go ............. 212
来源：http://pjn.cashguo.top

Ruby ........... 212
来源：http://rcv.yangfankeji.com

C# ............. 212
来源：http://ysv.yangfankeji.com

C .............. 30
来源：http://tqw.jianghu66.top

C++ ............ 30
来源：http://hka.fktsv.cn

SQL ............ 90
来源：http://sui.pycfn.com

Bash ........... 80
来源：http://mmd.redwolf501.top

Kotlin ......... 15
来源：http://ofc.quarkkingdee.top

Swift .......... 15
来源：http://pjn.yanxiufei.cn

Lua ............ 10
来源：http://msx.xuanzx.com

Perl ........... 10
来源：http://kpx.dashuyun.cn

Scala .......... 10
来源：http://mbu.zdqjudy.top

------------------------------------
来源：http://mqq.uphjek.com

合计 ........... 2106 条
来源：http://brz.uphjek.com

按章节统计：
来源：http://pcd.yangfankeji.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://okx.dashuyun.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://llw.havefunace.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://afg.mhx1999.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rgw.guannengcc.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qte.yuxming.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://obf.fehbvm.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://gbp.nanxuanxn.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://lch.shangyingyoupin.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jfw.yuanzhike.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vef.zhongyouzk.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://sco.snrcjt.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://pcj.gogol.net.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kli.hfpthk.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://gwi.aizwys.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dzq.pycfn.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://agj.xylfe.cn

Q SQL 专题                              90
来源：http://cny.yongpay.top

R Bash 专题                             80
来源：http://wcf.jinqigufen.top

S C / C++ 专题                          60
来源：http://kpy.shzxlz.cn

T 其他语言补充                          60
来源：http://bub.svipenyu.cn

U 高频实用片段                         120
来源：http://fzz.jiagoushi.top

------------------------------------
来源：http://ezk.pengpengdd.cyou

合计                                  2106 条
来源：http://gto.zhaomingkeji.xyz

--------------------------------------------------------------------------------
来源：http://upj.tarul.cn

使用提醒
来源：http://mgs.jqgufenzy.top

--------------------------------------------------------------------------------
来源：http://wed.yongpay.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ykh.sysykeji.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://eck.ivvv.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://jlp.hnqzz.top

在旧版本上使用前请先确认语法支持情况。
来源：http://nje.yuanzhike.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://inq.haohaochexian.top

—— 文件结束 ——
来源：http://zpe.vehdjk.com

================================================================================
来源：http://kmf.yvedp.cn

程序语言常见例子速查手册（2024 版）
来源：http://pjj.snrcjt.cn

Common Programming Examples Cheat Book
来源：http://mxv.hammf.cn

================================================================================
来源：http://sry.meibo888.top

【收录内容】
来源：http://vgt.fengsongda.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ifl.sysykeji.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://qrg.52xcode.cn

SQL · Bash · C · C++
来源：http://xca.daria6918.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://sxl.zdqjudy.top

【使用说明】
来源：http://zbm.ybcxt.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://tsf.pengpengdd.cyou

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://jsk.jinqigufen.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://snb.guowangkeji.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://asq.zycfv.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://hwo.cqqwz.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://okl.xuetiantiany.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://gds.nanxuanxn.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://lsa.fehbvm.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://dqr.aizwys.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://bcj.bbcook.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hnr.hesvh.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://yyp.guannengcc.top

【文件统计】
来源：http://pkw.xylfe.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ngz.cashguo.top

--------------------------------------------------------------------------------
来源：http://nod.wangdashe.top

目  录
来源：http://jca.tian-w.cn

--------------------------------------------------------------------------------
来源：http://ser.xziqi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://whs.redwolf501.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://lcy.dianchejie.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fuq.hongshengwenyu.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://miv.jinyuanbaomall.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qvs.ybcxt.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://sfm.zdbjq.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://fpq.9152youxi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ryn.jianghu66.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://okn.nanxinkj.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mug.xinyue.icu

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://btd.epnwcf.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wyl.fzhhl.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://pgw.jinqigfzy.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gfr.zhaomingkeji.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ssd.yonumen.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://dte.hcnkem.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jks.cashguo.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://nnt.ehwqpu.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rik.gotoacloud.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://jvc.pycfn.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://pbw.yvedp.cn

================================================================================
来源：http://vma.jqgfzy.top

A. 基础语法与类型
来源：http://thw.iojbl.cn

================================================================================
来源：http://gpm.xuanzx.com

[A01] Hello World
来源：http://jqb.gzhubu.top

Py:   print("Hello, World!")
来源：http://czr.zhaomingkeji.xyz

PHP:  echo "Hello, World!";
来源：http://xkx.vehdjk.com

JS:   console.log("Hello, World!");
来源：http://rxh.cashguo.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://gmc.aizwys.cn


<!-- 参考信息 -->