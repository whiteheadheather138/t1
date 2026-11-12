代发 wailian999

[U37] Py：读写 Excel
来源：http://gcc.ctjpmb.com

pandas.read_excel / DataFrame.to_excel
来源：http://vhs.hfpthk.cn

[U38] Py：获取脚本所在目录
来源：http://qud.haohaochexian.top

Path(__file__).resolve().parent
来源：http://iez.yongpay.top

[U39] Py：判断是否在交互环境
来源：http://tjd.jqgufenzy.top

sys.stdout.isatty()
来源：http://bjz.yuanzhike.top

[U40] Py：打印到标准错误
来源：http://yto.daxiang520.top

print("err", file=sys.stderr)
来源：http://xnx.hcnkem.com

[U41] PHP：初始化 Composer 项目
来源：http://mhc.gogol.net.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://fve.zhongyouzk.top

[U42] PHP：PSR-4 自动加载
来源：http://lqv.sweek.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://sso.yj202588.top

[U43] PHP：声明命名空间
来源：http://lux.shzxlz.cn

namespace App\Http;
来源：http://foi.zdbjq.cn

[U44] PHP：开启严格类型
来源：http://wyo.wangdashe.top

declare(strict_types=1);
来源：http://udy.c1oappe.top

[U45] PHP：类型声明与返回类型
来源：http://qfy.jyoumei.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://gfg.fzhhl.top

[U46] PHP：可空类型
来源：http://qqy.vehdjk.com

?string $name = null
来源：http://xga.smart0.xyz

[U47] PHP：联合类型
来源：http://ecn.shzxlz.cn

int|string $id
来源：http://mtg.birdmap.top

[U48] PHP：纯枚举
来源：http://mzz.nanxuanxn.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dam.meibo888.top

[U49] PHP：只读属性
来源：http://yzt.cqqwz.cn

public readonly string $name
来源：http://tby.yuanzhike.top

[U50] PHP：构造器属性提升
来源：http://cty.gaohongyu789.top

public function __construct(private int $id) {}
来源：http://gpb.ehwqpu.com

[U51] PHP：数组解构
来源：http://mmq.zhengqikj.top

[$a, $b] = $arr;
来源：http://tgv.hfpthk.cn

[U52] PHP：箭头函数
来源：http://iby.xuanzx.com

$double = fn($x) => $x * 2;
来源：http://adv.zhoulong.xyz

[U53] PHP：空合并运算符
来源：http://whe.xuetiantiany.cn

$v = $a ?? $b ?? "default";
来源：http://asz.zdbjq.cn

[U54] PHP：空安全调用
来源：http://xvs.zhongyouzk.top

$obj?->method()
来源：http://pal.shangyingyoupin.top

[U55] PHP：match 表达式
来源：http://zvd.ivvv.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rvm.hnxiangtu.top

[U56] PHP：命名参数
来源：http://syt.shanyushiyangkeji.top

f(a: 1, b: 2)
来源：http://xbi.ehwqpu.com

[U57] PHP：字符串插值
来源：http://rnc.jlsjyb.cn

"值: {$a}"
来源：http://leg.zhijiandao.cn

[U58] PHP：数组三件套
来源：http://pkv.fanxiaobao.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wgu.yuxming.cn

[U59] PHP：自定义排序
来源：http://lih.haohaochexian.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://itj.ehwqpu.com

[U60] PHP：JSON 编解码
来源：http://nxn.snrcjt.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://osb.xuanzx.com

[U61] PHP：正则
来源：http://wky.xinyue.icu

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://oul.sjlbkw.cn

[U62] PHP：日期对象
来源：http://nbf.jyoumei.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lcf.yj20258.top

[U63] PHP：文件读写
来源：http://opu.sxryk.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qed.yanxiufei.cn

[U64] PHP：目录遍历
来源：http://ikx.fanxiaobao.xyz

glob("dir/*.php");  scandir("dir");
来源：http://yjt.ctjpmb.com

[U65] PHP：会话
来源：http://uvu.smart0.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://ywy.kuanghao11.cn

[U66] PHP：设置 Cookie
来源：http://wnb.zhiwuduotai.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cno.gzhubu.top

[U67] PHP：处理文件上传
来源：http://yaq.yueranfly.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ymy.jqgufenzy.top

[U68] PHP：PDO 连接
来源：http://gfa.iojbl.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://isq.ybcxt.top

[U69] PHP：PDO 预处理
来源：http://zsw.sxryk.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://byw.yuanzhike.top

[U70] PHP：PDO 事务
来源：http://ycs.yfazqb.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lbt.cucudq.cn

[U71] PHP：抛出异常
来源：http://ceq.ehwqpu.com

throw new RuntimeException("失败", 500);
来源：http://shb.ctjpmb.com

[U72] PHP：写错误日志
来源：http://mey.hcnkem.com

error_log("失败: " . $e->getMessage());
来源：http://hga.hcnkem.com

[U73] PHP：读取 ini 配置
来源：http://vfg.guannengcc.top

parse_ini_file("config.ini", true)
来源：http://yan.vehdjk.com

[U74] PHP：读取环境变量
来源：http://rfo.cqqwz.cn

getenv("APP_ENV") ?: "production"
来源：http://rrk.yfazqb.com

[U75] PHP：依赖注入
来源：http://khj.jinqigufen.top

composer require psr/container
来源：http://zod.sweek.top

[U76] PHP：简单路由
来源：http://fra.ywan-chungtsiang.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ihg.zhixingplan.top

[U77] PHP：模板渲染
来源：http://inj.wangshuangyany.cn

composer require twig/twig
来源：http://axb.jianghu66.top

[U78] PHP：单元测试
来源：http://zvf.epnwcf.com

composer require --dev phpunit/phpunit
来源：http://etz.hnxiangtu.top

[U79] PHP：静态分析
来源：http://drt.yueranfly.top

composer require --dev phpstan/phpstan
来源：http://ifd.yueranfly.top

[U80] PHP：代码规范修复
来源：http://frb.zhongyouzk.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ydr.sjlbkw.cn

[U81] JS：初始化项目
来源：http://vcj.epnwcf.com

npm init -y;  npm i express
来源：http://fhk.hywenlv.cn

[U82] JS：package.json 脚本
来源：http://vyi.yanxiufei.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://yog.haohaochexian.top

[U83] JS：ES Module 导入导出
来源：http://wck.svipenyu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://nbl.chenjidiqi.icu

[U84] JS：CommonJS 写法
来源：http://xyt.bbcook.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ctv.andypj.xyz

[U85] JS：可选链
来源：http://icn.aizwys.cn

a?.b?.c
来源：http://vji.andypj.xyz

[U86] JS：空值合并
来源：http://xsi.yonumen.top

a ?? b
来源：http://gyu.yvedp.cn

[U87] JS：解构默认值
来源：http://zfh.epnwcf.com

const { a = 1, b = 2 } = obj;
来源：http://ncz.bjfxy.top

[U88] JS：对象展开合并
来源：http://emb.aibaodan.cn

{ ...a, ...b }
来源：http://dea.uphjek.com

[U89] JS：数组去重
来源：http://tse.316326.xyz

[...new Set(arr)]
来源：http://tfo.mhx1999.top

[U90] JS：数字数组排序
来源：http://hhu.kuanghao11.cn

[...arr].sort((a, b) => a - b)
来源：http://jav.aizwys.cn

[U91] JS：对象键值遍历
来源：http://gjs.hnxiangtu.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tbs.birdmap.top

[U92] JS：深拷贝
来源：http://bmm.yonumen.top

structuredClone(obj)
来源：http://zey.gzhubu.top

[U93] JS：模板字符串
来源：http://uau.hywenlv.cn

`共 ${n} 条`
来源：http://orf.dianchejie.cn

[U94] JS：箭头函数
来源：http://rsg.xingfuxueyuan.xyz

const double = x => x * 2;
来源：http://wyn.ydzc1.top

[U95] JS：Promise 包装
来源：http://ooi.quarkkingdee.top

new Promise((resolve, reject) => {})
来源：http://ljl.yongpay.top

[U96] JS：async/await 与异常
来源：http://ocl.hfpthk.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pge.fanxiaobao.xyz

[U97] JS：并发请求
来源：http://trm.haohaochexian.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://mvt.jinqigfzy.top

[U98] JS：fetch 带 JSON
来源：http://qbs.uphjek.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://klr.zhixingplan.top

[U99] JS：事件监听
来源：http://ehw.zhongyouzk.top

el.addEventListener("click", e => {})
来源：http://igr.hesvh.cn

[U100] JS：DOM 查询
来源：http://hnf.haohaochexian.top

document.querySelector(".item")
来源：http://wqs.shanyushiyangkeji.top

[U101] JS：classList 操作
来源：http://voo.zhengqikj.top

el.classList.toggle("active")
来源：http://emc.tianlin.xyz

[U102] JS：本地存储
来源：http://qaa.mhx1999.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://sqa.jianghu66.top

[U103] JS：定时器
来源：http://hct.gogol.net.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://uuk.havefunace.top

[U104] JS：防抖
来源：http://gcw.jinghuilouyu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tej.52xcode.cn

[U105] JS：节流
来源：http://lrc.nwbrower.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yjn.pengpengdd.cyou

[U106] JS：日期格式化
来源：http://rgi.zhixingplan.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://phi.ehwqpu.com

[U107] JS：数字千分位
来源：http://oqr.pycfn.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ivn.zhoulong.xyz

[U108] JS：随机整数
来源：http://xyr.hongshengwenyu.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fch.wangshuangyany.cn

[U109] JS：数组分组
来源：http://dpl.hfpthk.cn

Object.groupBy(arr, x => x.type)
来源：http://jwx.chenlongwang.top

[U110] JS：数组分块
来源：http://zlo.fzhhl.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vav.havefunace.top

[U111] JS：对象转 Map
来源：http://twv.mhx1999.top

new Map(Object.entries(obj))
来源：http://jvc.shzxlz.cn

[U112] JS：字符串补位
来源：http://sqv.ppjwa.cn

"7".padStart(3, "0")
来源：http://vrn.shanyushiyangtech.top

[U113] JS：正则替换全部
来源：http://mdd.xuanzx.com

s.replaceAll("a", "b")
来源：http://pwm.guowangkeji.top

[U114] JS：JSON 深比较
来源：http://pgr.sweek.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://yuk.haohaochexian.top

[U115] JS：生成 UUID
来源：http://cit.yongpay.top

crypto.randomUUID()
来源：http://ffb.bjfxy.top

[U116] JS：类型检查（JSDoc）
来源：http://wdw.bjfxy.top

/** @param {string} name */ function f(name) {}
来源：http://atv.ivvv.top

[U117] JS：单元测试
来源：http://bio.shanyushiyangkeji.top

npm i -D vitest;  npx vitest
来源：http://dgc.hnxiangtu.top

[U118] JS：开发服务器
来源：http://qfu.yfazqb.com

npm i -D vite;  npx vite
来源：http://gtl.tianlin.xyz

[U119] JS：生产构建
来源：http://wld.guowangkeji.top

npx vite build
来源：http://jvf.jianghu66.top

[U120] JS：读取环境变量（Vite）
来源：http://njx.ydjk.org.cn

import.meta.env.VITE_API_URL
来源：http://eza.zhaomingkeji.xyz

================================================================================
来源：http://qhq.zhijiandao.cn

统计汇总
来源：http://oex.redwolf501.top

================================================================================
来源：http://mbe.svipenyu.cn

按语言统计（条）：
来源：http://zac.yj20258.top

Python ......... 252
来源：http://and.yonumen.top

PHP ............ 252
来源：http://nab.yj202588.top

JavaScript ..... 252
来源：http://omz.svipenyu.cn

TypeScript ..... 212
来源：http://eju.fzhhl.top

Java ........... 212
来源：http://wto.tian-w.cn

Go ............. 212
来源：http://wdr.xingfuxueyuan.xyz

Ruby ........... 212
来源：http://uhw.chenlongwang.top

C# ............. 212
来源：http://jil.sysykeji.top

C .............. 30
来源：http://fed.wangdashe.top

C++ ............ 30
来源：http://ysz.daria6918.cn

SQL ............ 90
来源：http://hfp.quarkkingdee.top

Bash ........... 80
来源：http://xzh.yvedp.cn

Kotlin ......... 15
来源：http://sze.nwbrower.top

Swift .......... 15
来源：http://rqq.ivvv.top

Lua ............ 10
来源：http://liw.yanxiufei.cn

Perl ........... 10
来源：http://lbv.kuanghao11.cn

Scala .......... 10
来源：http://clx.jinyuanbaomall.cn

------------------------------------
来源：http://esj.hnxiangtu.top

合计 ........... 2106 条
来源：http://fjp.dianchejie.cn

按章节统计：
来源：http://tjp.chenzaomai.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://esl.kuanghao11.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jjv.fehbvm.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pnw.jinqigfzy.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://tgu.shanyushiyangtech.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hbd.yfazqb.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hpc.aizwys.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ioc.andypj.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ulj.xuanzx.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://keb.fktsv.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jvq.yvedp.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ecf.9152youxi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ugn.ivvv.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://iph.yj20258888.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://nao.xylfe.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://euq.sxryk.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://thb.pengpengdd.cyou

Q SQL 专题                              90
来源：http://adm.yanxiufei.cn

R Bash 专题                             80
来源：http://plj.guowangkeji.top

S C / C++ 专题                          60
来源：http://phn.aizwys.cn

T 其他语言补充                          60
来源：http://izk.ybcxt.top

U 高频实用片段                         120
来源：http://zaf.jqgfzy.top

------------------------------------
来源：http://zks.andypj.xyz

合计                                  2106 条
来源：http://ytc.nwbrower.top

--------------------------------------------------------------------------------
来源：http://lei.sjlbkw.cn

使用提醒
来源：http://gvw.nwbrower.top

--------------------------------------------------------------------------------
来源：http://gcd.sufxvd.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://dme.nanxinkj.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jzl.dianchejie.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mju.yj20258888.top

在旧版本上使用前请先确认语法支持情况。
来源：http://vki.pengpengdd.cyou

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://cmj.redwolf501.top

—— 文件结束 ——
来源：http://eyz.haohaochexian.top

================================================================================
来源：http://shp.zhengqikj.top

程序语言常见例子速查手册（2024 版）
来源：http://yqf.gaohongyu789.top

Common Programming Examples Cheat Book
来源：http://qfr.tian-w.cn

================================================================================
来源：http://qnv.redwolf501.top

【收录内容】
来源：http://gby.fzhhl.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://idm.jlsjyb.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hyf.smart0.xyz

SQL · Bash · C · C++
来源：http://pis.cheryme.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://lsa.shanyushiyangtech.top

【使用说明】
来源：http://fyy.xylfe.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://yjr.havefunace.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wpb.hammf.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://kcl.nanxinkj.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://tqy.jiagoushi.top

Bash:  Shell         C:     C             C++:   C++
来源：http://fgr.0kj1m.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://dom.xziqi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://loe.gogol.net.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vcf.uphjek.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://asn.chenjidiqi.icu

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gcv.feifeiyinyue.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://lfn.kuanghao11.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ozc.sufxvd.cn

【文件统计】
来源：http://jyr.dashuyun.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zws.kuanghao11.cn

--------------------------------------------------------------------------------
来源：http://kds.hfpthk.cn

目  录
来源：http://eew.cashguo.top

--------------------------------------------------------------------------------
来源：http://mep.chenzaomai.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://byw.fehbvm.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://jfg.hnqzz.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wlz.nanxuanxn.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://fub.daria6918.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://oit.jiagoushi.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://nkm.zhijiandao.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://toa.jyoumei.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://fus.kuanghao11.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hhk.bjfxy.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fcs.daria6918.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://dcw.sweek.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://fti.fktsv.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ysw.zhijiandao.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://fhj.bbcook.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xoi.jiagoushi.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fsu.ehwqpu.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://sog.hesvh.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ill.jqgfzy.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ohg.gogol.net.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://vdz.sxryk.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hyl.zhijiandao.cn

================================================================================
来源：http://wpv.fktsv.cn

A. 基础语法与类型
来源：http://ouu.shuidangran.top

================================================================================
来源：http://evd.gzhubu.top

[A01] Hello World
来源：http://gbx.chenlongwang.top

Py:   print("Hello, World!")
来源：http://ofq.hcnkem.com

PHP:  echo "Hello, World!";
来源：http://szv.cqqwz.cn

JS:   console.log("Hello, World!");
来源：http://szm.hnxiangtu.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://sac.haohaochexian.top

Java: System.out.println("Hello, World!");
来源：http://dlo.hywenlv.cn

Go:   fmt.Println("Hello, World!")
来源：http://gvp.cdnleiting.top

Ruby: puts "Hello, World!"
来源：http://hmo.smart0.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://bji.tarul.cn

[A02] 变量声明与赋值
来源：http://kwf.redwolf501.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://uiq.hammf.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://gzy.9152youxi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://pwa.tanke756.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://lzh.zhixingplan.top

Java: String name = "Alex"; int age = 20;
来源：http://pyd.yongpay.top

Go:   name := "Alex"; age := 20
来源：http://icn.0kj1m.cn

Ruby: name = "Alex"; age = 20
来源：http://eqr.redwolf501.top

C#:   string name = "Alex"; int age = 20;
来源：http://mtz.fzhhl.top

[A03] 常量定义
来源：http://ewz.smart0.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hpy.iojbl.cn

PHP:  const PI = 3.14159;
来源：http://sup.daria6918.cn

JS:   const PI = 3.14159;
来源：http://nox.0kj1m.cn

TS:   const PI: number = 3.14159;
来源：http://rgh.cheryme.top

Java: static final double PI = 3.14159;
来源：http://yyi.feifeiyinyue.top

Go:   const PI = 3.14159
来源：http://bos.jyoumei.cn


<!-- 参考信息 -->