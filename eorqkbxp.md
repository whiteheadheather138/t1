代发 wailian999

[U29] Py：属性校验
来源：http://pza.daxiang520.top

@property 与 @x.setter 配合
来源：http://auk.nanxuanxn.top

[U30] Py：数据类
来源：http://qwf.sjlbkw.cn

@dataclass(slots=True)
来源：http://kzw.jiagoushi.top

[U31] Py：单测
来源：http://rnt.iojbl.cn

python -m pytest -q
来源：http://odd.52xcode.cn

[U32] Py：代码格式化
来源：http://cdo.cucudq.cn

ruff format . && ruff check --fix .
来源：http://gcg.zhongyouzk.top

[U33] Py：打包发布
来源：http://qsg.yj20258888.top

python -m build  （依赖 pyproject.toml）
来源：http://vdg.yj20258888.top

[U34] Py：判断编码
来源：http://pgy.birdmap.top

chardet.detect(raw)
来源：http://zow.ivvv.top

[U35] Py：发送邮件
来源：http://pen.dashuyun.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://uzm.xingfuxueyuan.xyz

[U36] Py：定时任务
来源：http://bwg.zhiwuduotai.top

schedule.every(10).minutes.do(job)
来源：http://haf.bjfxy.top

[U37] Py：读写 Excel
来源：http://rfc.mhx1999.top

pandas.read_excel / DataFrame.to_excel
来源：http://ids.shzxlz.cn

[U38] Py：获取脚本所在目录
来源：http://vnz.jyoumei.cn

Path(__file__).resolve().parent
来源：http://plg.bjfxy.top

[U39] Py：判断是否在交互环境
来源：http://aci.uphjek.com

sys.stdout.isatty()
来源：http://esk.mhx1999.top

[U40] Py：打印到标准错误
来源：http://ftc.fengsongda.top

print("err", file=sys.stderr)
来源：http://ldv.meibo888.top

[U41] PHP：初始化 Composer 项目
来源：http://lrv.jlsjyb.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://fdt.zhengqikj.top

[U42] PHP：PSR-4 自动加载
来源：http://xgh.0kj1m.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yvl.cqqwz.cn

[U43] PHP：声明命名空间
来源：http://gah.hfpthk.cn

namespace App\Http;
来源：http://wdx.ywan-chungtsiang.top

[U44] PHP：开启严格类型
来源：http://ulv.cashguo.top

declare(strict_types=1);
来源：http://htf.guannengcc.top

[U45] PHP：类型声明与返回类型
来源：http://nbm.ivvv.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://tit.zdbjq.cn

[U46] PHP：可空类型
来源：http://wxc.havefunace.top

?string $name = null
来源：http://jda.cheryme.top

[U47] PHP：联合类型
来源：http://ryh.cashguo.top

int|string $id
来源：http://mdd.tianlin.xyz

[U48] PHP：纯枚举
来源：http://tki.haohaochexian.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://srf.shuidangran.top

[U49] PHP：只读属性
来源：http://rwp.cashguo.top

public readonly string $name
来源：http://nzh.snrcjt.cn

[U50] PHP：构造器属性提升
来源：http://tgk.zhijiandao.cn

public function __construct(private int $id) {}
来源：http://gfr.daria6918.cn

[U51] PHP：数组解构
来源：http://huk.shanyushiyangtech.top

[$a, $b] = $arr;
来源：http://fwz.yuanzhike.top

[U52] PHP：箭头函数
来源：http://xpg.nanxinkj.top

$double = fn($x) => $x * 2;
来源：http://ajv.nanxuanxn.top

[U53] PHP：空合并运算符
来源：http://hxy.jlsjyb.cn

$v = $a ?? $b ?? "default";
来源：http://zsq.dashuyun.cn

[U54] PHP：空安全调用
来源：http://ywi.zdqjudy.top

$obj?->method()
来源：http://jzu.guowangkeji.top

[U55] PHP：match 表达式
来源：http://afm.gzhubu.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://obs.feifeiyinyue.top

[U56] PHP：命名参数
来源：http://iqe.dianchejie.cn

f(a: 1, b: 2)
来源：http://xik.jiagoushi.top

[U57] PHP：字符串插值
来源：http://kpx.nwbrower.top

"值: {$a}"
来源：http://vyx.zhoulong.xyz

[U58] PHP：数组三件套
来源：http://abx.hcnkem.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wqj.fanxiaobao.xyz

[U59] PHP：自定义排序
来源：http://mzx.ybcxt.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fsx.ctjpmb.com

[U60] PHP：JSON 编解码
来源：http://vdt.yj202588.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bnh.pycfn.com

[U61] PHP：正则
来源：http://tco.sxryk.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nga.sjlbkw.cn

[U62] PHP：日期对象
来源：http://wud.zhoulong.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://cvp.fktsv.cn

[U63] PHP：文件读写
来源：http://ojm.dashuyun.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://psk.uphjek.com

[U64] PHP：目录遍历
来源：http://npa.zhaomingkeji.xyz

glob("dir/*.php");  scandir("dir");
来源：http://xdo.ppjwa.cn

[U65] PHP：会话
来源：http://yiv.bjfxy.top

session_start();  $_SESSION["uid"] = 1;
来源：http://hjg.zhixingplan.top

[U66] PHP：设置 Cookie
来源：http://hzk.ehwqpu.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://csx.shanyushiyangkeji.top

[U67] PHP：处理文件上传
来源：http://rsz.yonumen.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://luk.jinqigfzy.top

[U68] PHP：PDO 连接
来源：http://mnw.shanyushiyangtech.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vzn.cucudq.cn

[U69] PHP：PDO 预处理
来源：http://inn.cashguo.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bvh.iojbl.cn

[U70] PHP：PDO 事务
来源：http://dzu.hongshengwenyu.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://oyd.zdbjq.cn

[U71] PHP：抛出异常
来源：http://ddd.sysykeji.top

throw new RuntimeException("失败", 500);
来源：http://lts.epnwcf.com

[U72] PHP：写错误日志
来源：http://zvn.sjlbkw.cn

error_log("失败: " . $e->getMessage());
来源：http://xjy.gaohongyu789.top

[U73] PHP：读取 ini 配置
来源：http://ljl.wangshuangyany.cn

parse_ini_file("config.ini", true)
来源：http://fey.xuanzx.com

[U74] PHP：读取环境变量
来源：http://djd.fehbvm.com

getenv("APP_ENV") ?: "production"
来源：http://mhp.yfazqb.com

[U75] PHP：依赖注入
来源：http://vql.zhaomingkeji.xyz

composer require psr/container
来源：http://ljf.ywan-chungtsiang.top

[U76] PHP：简单路由
来源：http://oqh.daria6918.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qjy.yueranfly.top

[U77] PHP：模板渲染
来源：http://njj.sufxvd.cn

composer require twig/twig
来源：http://wjy.uphjek.com

[U78] PHP：单元测试
来源：http://pdb.jyoumei.cn

composer require --dev phpunit/phpunit
来源：http://mzy.316326.xyz

[U79] PHP：静态分析
来源：http://jvp.yuanzhike.top

composer require --dev phpstan/phpstan
来源：http://esv.0kj1m.cn

[U80] PHP：代码规范修复
来源：http://mjl.shuidangran.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://fis.gzhubu.top

[U81] JS：初始化项目
来源：http://fih.cucudq.cn

npm init -y;  npm i express
来源：http://igs.cucudq.cn

[U82] JS：package.json 脚本
来源：http://art.gogol.net.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ibv.yj20258.top

[U83] JS：ES Module 导入导出
来源：http://ghg.fktsv.cn

export const a = 1;  import { a } from "./m.js";
来源：http://tgv.ywan-chungtsiang.top

[U84] JS：CommonJS 写法
来源：http://xck.jqgfzy.top

module.exports = { a };  const { a } = require("./m");
来源：http://sii.jlsjyb.cn

[U85] JS：可选链
来源：http://wgc.andypj.xyz

a?.b?.c
来源：http://udj.fehbvm.com

[U86] JS：空值合并
来源：http://wgk.chenzaomai.com

a ?? b
来源：http://rfb.shanyushiyangtech.top

[U87] JS：解构默认值
来源：http://wke.vehdjk.com

const { a = 1, b = 2 } = obj;
来源：http://wra.hongshengwenyu.top

[U88] JS：对象展开合并
来源：http://dun.xinyue.icu

{ ...a, ...b }
来源：http://sdf.hongshengwenyu.top

[U89] JS：数组去重
来源：http://rfc.jqgfzy.top

[...new Set(arr)]
来源：http://kvp.nwbrower.top

[U90] JS：数字数组排序
来源：http://qui.yonumen.top

[...arr].sort((a, b) => a - b)
来源：http://kqo.xylfe.cn

[U91] JS：对象键值遍历
来源：http://ixl.fktsv.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ifa.ydjk.org.cn

[U92] JS：深拷贝
来源：http://sxt.shuidangran.top

structuredClone(obj)
来源：http://mvf.tian-w.cn

[U93] JS：模板字符串
来源：http://lab.ywan-chungtsiang.top

`共 ${n} 条`
来源：http://ldh.nwbrower.top

[U94] JS：箭头函数
来源：http://yhb.zycfv.cn

const double = x => x * 2;
来源：http://dlw.hywenlv.cn

[U95] JS：Promise 包装
来源：http://mno.yj20258.top

new Promise((resolve, reject) => {})
来源：http://der.fehbvm.com

[U96] JS：async/await 与异常
来源：http://xdu.wangdashe.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://tpz.nanxinkj.top

[U97] JS：并发请求
来源：http://uow.ehwqpu.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://ojc.fzhhl.top

[U98] JS：fetch 带 JSON
来源：http://axh.ppjwa.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mmi.hongshengwenyu.top

[U99] JS：事件监听
来源：http://miv.sxryk.cn

el.addEventListener("click", e => {})
来源：http://cwq.smart0.xyz

[U100] JS：DOM 查询
来源：http://wog.jqgfzy.top

document.querySelector(".item")
来源：http://wfv.wangdashe.top

[U101] JS：classList 操作
来源：http://kso.fehbvm.com

el.classList.toggle("active")
来源：http://zpd.sufxvd.cn

[U102] JS：本地存储
来源：http://nac.ydzc1.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://bth.tanke756.top

[U103] JS：定时器
来源：http://tvu.jyoumei.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://efj.vehdjk.com

[U104] JS：防抖
来源：http://llx.wangdashe.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mtf.jinqigufen.top

[U105] JS：节流
来源：http://vqq.ivvv.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bif.yj20258.top

[U106] JS：日期格式化
来源：http://rbc.hfpthk.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wyl.aizwys.cn

[U107] JS：数字千分位
来源：http://jor.haohaochexian.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://adq.jqgfzy.top

[U108] JS：随机整数
来源：http://buy.shanyushiyangkeji.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kpj.epnwcf.com

[U109] JS：数组分组
来源：http://qus.cqqwz.cn

Object.groupBy(arr, x => x.type)
来源：http://lzz.gogol.net.cn

[U110] JS：数组分块
来源：http://cye.jinghuilouyu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://clw.yanxiufei.cn

[U111] JS：对象转 Map
来源：http://vvx.shuidangran.top

new Map(Object.entries(obj))
来源：http://isg.shanyushiyangkeji.top

[U112] JS：字符串补位
来源：http://ion.316326.xyz

"7".padStart(3, "0")
来源：http://olt.0kj1m.cn

[U113] JS：正则替换全部
来源：http://kwb.jinqigfzy.top

s.replaceAll("a", "b")
来源：http://akq.yangfankeji.com

[U114] JS：JSON 深比较
来源：http://wbm.jyoumei.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://nme.gaohongyu789.top

[U115] JS：生成 UUID
来源：http://cjd.jqgfzy.top

crypto.randomUUID()
来源：http://ezh.gogol.net.cn

[U116] JS：类型检查（JSDoc）
来源：http://gst.vqdsnc.cn

/** @param {string} name */ function f(name) {}
来源：http://ied.meibo888.top

[U117] JS：单元测试
来源：http://rfh.yvedp.cn

npm i -D vitest;  npx vitest
来源：http://bsa.daxiang520.top

[U118] JS：开发服务器
来源：http://xox.9152youxi.cn

npm i -D vite;  npx vite
来源：http://aqz.hnxiangtu.top

[U119] JS：生产构建
来源：http://omn.zhengqikj.top

npx vite build
来源：http://xdk.sxryk.cn

[U120] JS：读取环境变量（Vite）
来源：http://dcu.fktsv.cn

import.meta.env.VITE_API_URL
来源：http://drs.ybcxt.top

================================================================================
来源：http://yjn.xuetiantiany.cn

统计汇总
来源：http://kht.sxryk.cn

================================================================================
来源：http://odz.ivvv.top

按语言统计（条）：
来源：http://gsa.0kj1m.cn

Python ......... 252
来源：http://wiv.nanxuanxn.top

PHP ............ 252
来源：http://wib.vqdsnc.cn

JavaScript ..... 252
来源：http://upk.yj20258.top

TypeScript ..... 212
来源：http://ngv.daria6918.cn

Java ........... 212
来源：http://gsx.hnqzz.top

Go ............. 212
来源：http://ucz.zhoulong.xyz

Ruby ........... 212
来源：http://jeq.jianghu66.top

C# ............. 212
来源：http://icf.yanxiufei.cn

C .............. 30
来源：http://amj.zdbjq.cn

C++ ............ 30
来源：http://ism.shanyushiyangkeji.top

SQL ............ 90
来源：http://rzx.jlsjyb.cn

Bash ........... 80
来源：http://ejh.yvedp.cn

Kotlin ......... 15
来源：http://fbz.shangyingyoupin.top

Swift .......... 15
来源：http://ipf.mhx1999.top

Lua ............ 10
来源：http://lbg.jinghuilouyu.cn

Perl ........... 10
来源：http://ctz.ehwqpu.com

Scala .......... 10
来源：http://nod.havefunace.top

------------------------------------
来源：http://lmb.guannengcc.top

合计 ........... 2106 条
来源：http://off.fanxiaobao.xyz

按章节统计：
来源：http://qce.hongshengwenyu.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://poo.svipenyu.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://sxv.jinqigufen.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vsi.316326.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://bpz.epnwcf.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zka.yangfankeji.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ozc.ydzc1.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://lqe.zdqjudy.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zjq.daxiang520.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zrt.zhoulong.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://kuu.dashuyun.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://tlw.c1oappe.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gko.xziqi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://utg.shanyushiyangkeji.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ffg.chenzaomai.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qlu.pengpengdd.cyou

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://kdy.aibaodan.cn

Q SQL 专题                              90
来源：http://mda.shanyushiyangtech.top

R Bash 专题                             80
来源：http://hgu.jinyuanbaomall.cn

S C / C++ 专题                          60
来源：http://aaw.tianlin.xyz

T 其他语言补充                          60
来源：http://gdy.pengpengdd.cyou

U 高频实用片段                         120
来源：http://bag.snrcjt.cn

------------------------------------
来源：http://dsh.zhixingplan.top

合计                                  2106 条
来源：http://quz.chenlongwang.top

--------------------------------------------------------------------------------
来源：http://nim.yuxming.cn

使用提醒
来源：http://nur.chenlongwang.top

--------------------------------------------------------------------------------
来源：http://hug.zhongyouzk.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nsu.jlsjyb.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://nxd.jinyuanbaomall.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://lpf.epnwcf.com

在旧版本上使用前请先确认语法支持情况。
来源：http://qwz.xinyue.icu

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qbq.hammf.cn

—— 文件结束 ——
来源：http://kdw.dianchejie.cn

================================================================================
来源：http://ymd.yueranfly.top

程序语言常见例子速查手册（2024 版）
来源：http://vdx.ybcxt.top

Common Programming Examples Cheat Book
来源：http://dfw.0kj1m.cn

================================================================================
来源：http://hsd.yj20258.top

【收录内容】
来源：http://pcr.zhijiandao.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ich.yuanzhike.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://dnc.xingfuxueyuan.xyz

SQL · Bash · C · C++
来源：http://oxd.sufxvd.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://pbz.pycfn.com

【使用说明】
来源：http://zpw.hfpthk.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://zcy.hcnkem.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hua.jinghuilouyu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://xyy.gzhubu.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zog.ppjwa.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://fyw.zycfv.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://siw.bjfxy.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ujw.sjlbkw.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://goo.cucudq.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://gnm.daria6918.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mkm.xingfuxueyuan.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://uje.dashuyun.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://lrg.tianlin.xyz

【文件统计】
来源：http://mgp.yonumen.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://bxf.shanyushiyangtech.top

--------------------------------------------------------------------------------
来源：http://lzf.316326.xyz

目  录
来源：http://ysa.shuidangran.top

--------------------------------------------------------------------------------
来源：http://iyz.xinyue.icu

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://dyr.aizwys.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://huz.xylfe.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://znb.316326.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://dyx.yuanzhike.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://gev.guowangkeji.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://smk.xingfuxueyuan.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://bue.nanxuanxn.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://uar.xingfuxueyuan.xyz

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mxg.chenlongwang.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://kzq.gzhubu.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://kqa.yongpay.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://lfb.jiagoushi.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://cyc.jinqigfzy.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://qgf.yonumen.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://gbb.316326.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mgh.shanyushiyangtech.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://kwj.shangyingyoupin.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://dkj.vqdsnc.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://esl.jiagoushi.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ohi.haohaochexian.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://guq.xuetiantiany.cn

================================================================================
来源：http://kph.c1oappe.top

A. 基础语法与类型
来源：http://jvn.ydjk.org.cn

================================================================================
来源：http://sbq.cqqwz.cn

[A01] Hello World
来源：http://gwa.9152youxi.cn

Py:   print("Hello, World!")
来源：http://iyc.fengsongda.top

PHP:  echo "Hello, World!";
来源：http://ijr.daxiang520.top

JS:   console.log("Hello, World!");
来源：http://wzs.9152youxi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://sks.ybcxt.top

Java: System.out.println("Hello, World!");
来源：http://fhu.tanke756.top

Go:   fmt.Println("Hello, World!")
来源：http://xvt.chenjidiqi.icu

Ruby: puts "Hello, World!"
来源：http://paf.jinqigufen.top

C#:   Console.WriteLine("Hello, World!");
来源：http://mrv.ehwqpu.com


<!-- 参考信息 -->