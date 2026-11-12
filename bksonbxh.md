代发 wailian999

[U23] Py：分块读取大文件
来源：http://bxm.0kj1m.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vpp.ydjk.org.cn

[U24] Py：路径操作
来源：http://rro.sysykeji.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jmv.xuanzx.com

[U25] Py：CSV 按字典读
来源：http://wbb.xuanzx.com

csv.DictReader(f)
来源：http://eac.smart0.xyz

[U26] Py：并发下载
来源：http://xxg.bjfxy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zqy.shangyingyoupin.top

[U27] Py：异步 HTTP
来源：http://yhg.guannengcc.top

aiohttp.ClientSession() 配合 async with
来源：http://xlk.pycfn.com

[U28] Py：类型别名
来源：http://frw.andypj.xyz

UserId = int
来源：http://bgz.vqdsnc.cn

[U29] Py：属性校验
来源：http://upa.dianchejie.cn

@property 与 @x.setter 配合
来源：http://hbr.havefunace.top

[U30] Py：数据类
来源：http://okj.hcnkem.com

@dataclass(slots=True)
来源：http://ony.zhixingplan.top

[U31] Py：单测
来源：http://sbj.ppjwa.cn

python -m pytest -q
来源：http://qna.dashuyun.cn

[U32] Py：代码格式化
来源：http://dru.tarul.cn

ruff format . && ruff check --fix .
来源：http://cia.mhx1999.top

[U33] Py：打包发布
来源：http://ewb.xingfuxueyuan.xyz

python -m build  （依赖 pyproject.toml）
来源：http://jgs.feifeiyinyue.top

[U34] Py：判断编码
来源：http://yku.andypj.xyz

chardet.detect(raw)
来源：http://phl.yonumen.top

[U35] Py：发送邮件
来源：http://kwg.ppjwa.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jxf.sufxvd.cn

[U36] Py：定时任务
来源：http://qxj.cashguo.top

schedule.every(10).minutes.do(job)
来源：http://okd.zhixingplan.top

[U37] Py：读写 Excel
来源：http://cuo.zycfv.cn

pandas.read_excel / DataFrame.to_excel
来源：http://kir.zdbjq.cn

[U38] Py：获取脚本所在目录
来源：http://vgu.c1oappe.top

Path(__file__).resolve().parent
来源：http://mco.fzhhl.top

[U39] Py：判断是否在交互环境
来源：http://bfw.sysykeji.top

sys.stdout.isatty()
来源：http://nmv.hfpthk.cn

[U40] Py：打印到标准错误
来源：http://qsb.shzxlz.cn

print("err", file=sys.stderr)
来源：http://zfr.zhoulong.xyz

[U41] PHP：初始化 Composer 项目
来源：http://vrn.fzhhl.top

composer init;  composer require guzzlehttp/guzzle
来源：http://cmq.yongpay.top

[U42] PHP：PSR-4 自动加载
来源：http://bsc.yuxming.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mrk.cqqwz.cn

[U43] PHP：声明命名空间
来源：http://nbj.ybcxt.top

namespace App\Http;
来源：http://waf.yangfankeji.com

[U44] PHP：开启严格类型
来源：http://smh.svipenyu.cn

declare(strict_types=1);
来源：http://sob.ppjwa.cn

[U45] PHP：类型声明与返回类型
来源：http://ktj.hammf.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://qra.fengsongda.top

[U46] PHP：可空类型
来源：http://nra.yj202588.top

?string $name = null
来源：http://dzs.sxryk.cn

[U47] PHP：联合类型
来源：http://xsn.zhongyouzk.top

int|string $id
来源：http://izp.hysaishi.cn

[U48] PHP：纯枚举
来源：http://cnc.yvedp.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://oir.nanxuanxn.top

[U49] PHP：只读属性
来源：http://okw.aizwys.cn

public readonly string $name
来源：http://mho.yongpay.top

[U50] PHP：构造器属性提升
来源：http://atw.andypj.xyz

public function __construct(private int $id) {}
来源：http://zoo.316326.xyz

[U51] PHP：数组解构
来源：http://prv.havefunace.top

[$a, $b] = $arr;
来源：http://jos.gotoacloud.top

[U52] PHP：箭头函数
来源：http://mky.ydjk.org.cn

$double = fn($x) => $x * 2;
来源：http://eot.yongpay.top

[U53] PHP：空合并运算符
来源：http://cxp.aibaodan.cn

$v = $a ?? $b ?? "default";
来源：http://sqj.xinyue.icu

[U54] PHP：空安全调用
来源：http://eos.aibaodan.cn

$obj?->method()
来源：http://jhp.cheryme.top

[U55] PHP：match 表达式
来源：http://cnx.hcnkem.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://byv.xziqi.cn

[U56] PHP：命名参数
来源：http://lsb.yongpay.top

f(a: 1, b: 2)
来源：http://xxv.hcnkem.com

[U57] PHP：字符串插值
来源：http://qjn.pengpengdd.cyou

"值: {$a}"
来源：http://fjy.yangfankeji.com

[U58] PHP：数组三件套
来源：http://ocl.haohaochexian.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vgb.jlsjyb.cn

[U59] PHP：自定义排序
来源：http://sir.guowangkeji.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xjp.bbcook.cn

[U60] PHP：JSON 编解码
来源：http://seo.tanke756.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://anb.xuetiantiany.cn

[U61] PHP：正则
来源：http://mkm.zhaomingkeji.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ych.hesvh.cn

[U62] PHP：日期对象
来源：http://zcq.316326.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://awv.xylfe.cn

[U63] PHP：文件读写
来源：http://awk.ydzc1.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://llh.vehdjk.com

[U64] PHP：目录遍历
来源：http://vxc.hammf.cn

glob("dir/*.php");  scandir("dir");
来源：http://rxn.svipenyu.cn

[U65] PHP：会话
来源：http://xxr.hysaishi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://lxg.sxryk.cn

[U66] PHP：设置 Cookie
来源：http://eml.shuidangran.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wyt.quarkkingdee.top

[U67] PHP：处理文件上传
来源：http://ndo.andypj.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://opv.haohaochexian.top

[U68] PHP：PDO 连接
来源：http://nmm.cucudq.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ckl.dianchejie.cn

[U69] PHP：PDO 预处理
来源：http://bph.birdmap.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fzz.andypj.xyz

[U70] PHP：PDO 事务
来源：http://mlu.ydjk.org.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://khd.bbcook.cn

[U71] PHP：抛出异常
来源：http://ook.cheryme.top

throw new RuntimeException("失败", 500);
来源：http://rqr.bbcook.cn

[U72] PHP：写错误日志
来源：http://hgp.xziqi.cn

error_log("失败: " . $e->getMessage());
来源：http://fgt.daxiang520.top

[U73] PHP：读取 ini 配置
来源：http://zqj.ehwqpu.com

parse_ini_file("config.ini", true)
来源：http://aiu.zhiwuduotai.top

[U74] PHP：读取环境变量
来源：http://uth.zdqjudy.top

getenv("APP_ENV") ?: "production"
来源：http://gyn.hnqzz.top

[U75] PHP：依赖注入
来源：http://mea.redwolf501.top

composer require psr/container
来源：http://ncz.daxiang520.top

[U76] PHP：简单路由
来源：http://cjf.zhengqikj.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qkf.yj20258888.top

[U77] PHP：模板渲染
来源：http://fex.mhx1999.top

composer require twig/twig
来源：http://dhn.quarkkingdee.top

[U78] PHP：单元测试
来源：http://qdm.snrcjt.cn

composer require --dev phpunit/phpunit
来源：http://oiv.yvedp.cn

[U79] PHP：静态分析
来源：http://yrg.guowangkeji.top

composer require --dev phpstan/phpstan
来源：http://nhx.xylfe.cn

[U80] PHP：代码规范修复
来源：http://gvw.pengpengdd.cyou

composer require --dev friendsofphp/php-cs-fixer
来源：http://fkr.guowangkeji.top

[U81] JS：初始化项目
来源：http://fpu.dashuyun.cn

npm init -y;  npm i express
来源：http://xjz.zdqjudy.top

[U82] JS：package.json 脚本
来源：http://eim.zhaomingkeji.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fju.shangyingyoupin.top

[U83] JS：ES Module 导入导出
来源：http://mxm.fehbvm.com

export const a = 1;  import { a } from "./m.js";
来源：http://wpv.0kj1m.cn

[U84] JS：CommonJS 写法
来源：http://eav.ybcxt.top

module.exports = { a };  const { a } = require("./m");
来源：http://zum.yonumen.top

[U85] JS：可选链
来源：http://fhx.hesvh.cn

a?.b?.c
来源：http://uoh.chenjidiqi.icu

[U86] JS：空值合并
来源：http://hmd.fengsongda.top

a ?? b
来源：http://cua.havefunace.top

[U87] JS：解构默认值
来源：http://mgz.vehdjk.com

const { a = 1, b = 2 } = obj;
来源：http://waj.gotoacloud.top

[U88] JS：对象展开合并
来源：http://rfn.pycfn.com

{ ...a, ...b }
来源：http://hnm.ydzc1.top

[U89] JS：数组去重
来源：http://wgd.ydjk.org.cn

[...new Set(arr)]
来源：http://klb.ydzc1.top

[U90] JS：数字数组排序
来源：http://ktx.bbcook.cn

[...arr].sort((a, b) => a - b)
来源：http://vjt.epnwcf.com

[U91] JS：对象键值遍历
来源：http://okr.aizwys.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xhb.snrcjt.cn

[U92] JS：深拷贝
来源：http://pss.vehdjk.com

structuredClone(obj)
来源：http://wmx.smart0.xyz

[U93] JS：模板字符串
来源：http://oyj.shzxlz.cn

`共 ${n} 条`
来源：http://nzz.tian-w.cn

[U94] JS：箭头函数
来源：http://cbx.gotoacloud.top

const double = x => x * 2;
来源：http://xtz.xuetiantiany.cn

[U95] JS：Promise 包装
来源：http://tbc.zhongyouzk.top

new Promise((resolve, reject) => {})
来源：http://kuw.yj202588.top

[U96] JS：async/await 与异常
来源：http://tbm.sufxvd.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jbd.smart0.xyz

[U97] JS：并发请求
来源：http://vbg.hongshengwenyu.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://lei.52xcode.cn

[U98] JS：fetch 带 JSON
来源：http://xvk.zhiwuduotai.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qzb.xingfuxueyuan.xyz

[U99] JS：事件监听
来源：http://lmp.xuanzx.com

el.addEventListener("click", e => {})
来源：http://izp.xinyue.icu

[U100] JS：DOM 查询
来源：http://bti.sjlbkw.cn

document.querySelector(".item")
来源：http://wem.jyoumei.cn

[U101] JS：classList 操作
来源：http://obe.yonumen.top

el.classList.toggle("active")
来源：http://apj.jinghuilouyu.cn

[U102] JS：本地存储
来源：http://gci.chenjidiqi.icu

localStorage.setItem("k", JSON.stringify(v))
来源：http://xaf.hfpthk.cn

[U103] JS：定时器
来源：http://att.fktsv.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://puc.aibaodan.cn

[U104] JS：防抖
来源：http://vvy.jqgfzy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fzp.yj20258.top

[U105] JS：节流
来源：http://xsn.xinyue.icu

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://aet.smart0.xyz

[U106] JS：日期格式化
来源：http://uub.cashguo.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wuf.ctjpmb.com

[U107] JS：数字千分位
来源：http://trl.yfazqb.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rgn.0kj1m.cn

[U108] JS：随机整数
来源：http://yvv.bbcook.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cir.cqqwz.cn

[U109] JS：数组分组
来源：http://mzn.iojbl.cn

Object.groupBy(arr, x => x.type)
来源：http://cju.kuanghao11.cn

[U110] JS：数组分块
来源：http://wtd.quarkkingdee.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pjt.yj20258.top

[U111] JS：对象转 Map
来源：http://rvt.chenlongwang.top

new Map(Object.entries(obj))
来源：http://pjm.jinqigfzy.top

[U112] JS：字符串补位
来源：http://ejn.yongpay.top

"7".padStart(3, "0")
来源：http://zyj.zdqjudy.top

[U113] JS：正则替换全部
来源：http://oru.cheryme.top

s.replaceAll("a", "b")
来源：http://djs.feifeiyinyue.top

[U114] JS：JSON 深比较
来源：http://qgw.sxryk.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://idu.fehbvm.com

[U115] JS：生成 UUID
来源：http://hky.ehwqpu.com

crypto.randomUUID()
来源：http://muw.shuidangran.top

[U116] JS：类型检查（JSDoc）
来源：http://unk.yj202588.top

/** @param {string} name */ function f(name) {}
来源：http://ukl.havefunace.top

[U117] JS：单元测试
来源：http://xxk.jyoumei.cn

npm i -D vitest;  npx vitest
来源：http://piu.guannengcc.top

[U118] JS：开发服务器
来源：http://odt.gaohongyu789.top

npm i -D vite;  npx vite
来源：http://lsg.hammf.cn

[U119] JS：生产构建
来源：http://dzs.vehdjk.com

npx vite build
来源：http://knh.xziqi.cn

[U120] JS：读取环境变量（Vite）
来源：http://yko.cheryme.top

import.meta.env.VITE_API_URL
来源：http://fzl.kuanghao11.cn

================================================================================
来源：http://lkd.sweek.top

统计汇总
来源：http://aws.zhaomingkeji.xyz

================================================================================
来源：http://cnt.guannengcc.top

按语言统计（条）：
来源：http://pvx.ivvv.top

Python ......... 252
来源：http://bsl.tarul.cn

PHP ............ 252
来源：http://vwr.xuetiantiany.cn

JavaScript ..... 252
来源：http://qeh.dianchejie.cn

TypeScript ..... 212
来源：http://mmq.bbcook.cn

Java ........... 212
来源：http://lyu.gaohongyu789.top

Go ............. 212
来源：http://ryq.zhongyouzk.top

Ruby ........... 212
来源：http://fiy.haohaochexian.top

C# ............. 212
来源：http://zbd.yonumen.top

C .............. 30
来源：http://qqz.cqqwz.cn

C++ ............ 30
来源：http://sti.yanxiufei.cn

SQL ............ 90
来源：http://aqz.guannengcc.top

Bash ........... 80
来源：http://vom.iojbl.cn

Kotlin ......... 15
来源：http://ljo.vehdjk.com

Swift .......... 15
来源：http://wyr.redwolf501.top

Lua ............ 10
来源：http://csp.uphjek.com

Perl ........... 10
来源：http://rco.aibaodan.cn

Scala .......... 10
来源：http://upz.redwolf501.top

------------------------------------
来源：http://bmj.xylfe.cn

合计 ........... 2106 条
来源：http://nll.xylfe.cn

按章节统计：
来源：http://qgx.yanxiufei.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ats.tarul.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ilw.pycfn.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://cvc.daxiang520.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mxc.zhiwuduotai.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fts.redwolf501.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gpy.yonumen.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vyp.yanxiufei.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://afp.hfpthk.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://tyh.yueranfly.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jkn.jinqigufen.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wpg.jinghuilouyu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jky.daria6918.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bol.ybcxt.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qtt.shuidangran.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yvh.yangfankeji.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hkn.yonumen.top

Q SQL 专题                              90
来源：http://dut.ivvv.top

R Bash 专题                             80
来源：http://fcp.0kj1m.cn

S C / C++ 专题                          60
来源：http://uei.316326.xyz

T 其他语言补充                          60
来源：http://ftc.snrcjt.cn

U 高频实用片段                         120
来源：http://wpq.nwbrower.top

------------------------------------
来源：http://axu.fehbvm.com

合计                                  2106 条
来源：http://xlh.daxiang520.top

--------------------------------------------------------------------------------
来源：http://pff.cqqwz.cn

使用提醒
来源：http://lhc.sweek.top

--------------------------------------------------------------------------------
来源：http://xna.zhaomingkeji.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://cmt.sjlbkw.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zac.dianchejie.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://nam.zhaomingkeji.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://vtu.jiagoushi.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://vun.yongpay.top

—— 文件结束 ——
来源：http://iwa.quarkkingdee.top

================================================================================
来源：http://jjd.jianghu66.top

程序语言常见例子速查手册（2024 版）
来源：http://lzr.bjfxy.top

Common Programming Examples Cheat Book
来源：http://ptc.andypj.xyz

================================================================================
来源：http://fcp.zycfv.cn

【收录内容】
来源：http://ldl.fanxiaobao.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://qtj.hfpthk.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://llp.xylfe.cn

SQL · Bash · C · C++
来源：http://sun.fanxiaobao.xyz

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://kqa.wangdashe.top

【使用说明】
来源：http://gex.xingfuxueyuan.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://des.ydjk.org.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wjh.xingfuxueyuan.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://cgs.hywenlv.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://yva.xinyue.icu

Bash:  Shell         C:     C             C++:   C++
来源：http://gsc.zhiwuduotai.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://vvd.jyoumei.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vbg.uphjek.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://obh.pycfn.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ndg.9152youxi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://rnr.sjlbkw.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wdt.zhixingplan.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mqr.yj20258888.top

【文件统计】
来源：http://bsa.pengpengdd.cyou

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://bxu.ywan-chungtsiang.top

--------------------------------------------------------------------------------
来源：http://aov.tianlin.xyz

目  录
来源：http://kjf.daria6918.cn

--------------------------------------------------------------------------------
来源：http://btw.shzxlz.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xoa.gaohongyu789.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://oma.52xcode.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://uae.yfazqb.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://pfm.jqgufenzy.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://oyj.wangdashe.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://roa.yvedp.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xar.zhengqikj.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://akd.zdqjudy.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://nvn.sxryk.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://kdu.gotoacloud.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://cgj.hnqzz.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://brl.hesvh.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://obk.fehbvm.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ocd.guannengcc.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://vex.wangshuangyany.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://vto.aibaodan.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hdb.sysykeji.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://jvh.wangdashe.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rfp.yuanzhike.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wum.vehdjk.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://vzu.dashuyun.cn


<!-- 参考信息 -->