代发 wailian999

[U25] Py：CSV 按字典读
来源：http://vha.zdqjudy.top

csv.DictReader(f)
来源：http://nob.ctjpmb.com

[U26] Py：并发下载
来源：http://qhs.chenzaomai.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://liz.pengpengdd.cyou

[U27] Py：异步 HTTP
来源：http://brx.gotoacloud.top

aiohttp.ClientSession() 配合 async with
来源：http://jlp.xziqi.cn

[U28] Py：类型别名
来源：http://jot.nanxuanxn.top

UserId = int
来源：http://suj.meibo888.top

[U29] Py：属性校验
来源：http://aax.iojbl.cn

@property 与 @x.setter 配合
来源：http://xjn.jinyuanbaomall.cn

[U30] Py：数据类
来源：http://yzu.dianchejie.cn

@dataclass(slots=True)
来源：http://qhp.gzhubu.top

[U31] Py：单测
来源：http://sdb.chenzaomai.com

python -m pytest -q
来源：http://xdd.nanxuanxn.top

[U32] Py：代码格式化
来源：http://jpd.shzxlz.cn

ruff format . && ruff check --fix .
来源：http://ovv.yongpay.top

[U33] Py：打包发布
来源：http://fup.cashguo.top

python -m build  （依赖 pyproject.toml）
来源：http://jao.pengpengdd.cyou

[U34] Py：判断编码
来源：http://wyt.mhx1999.top

chardet.detect(raw)
来源：http://ifb.hammf.cn

[U35] Py：发送邮件
来源：http://sty.hywenlv.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ebl.xuetiantiany.cn

[U36] Py：定时任务
来源：http://ljs.fanxiaobao.xyz

schedule.every(10).minutes.do(job)
来源：http://ced.fengsongda.top

[U37] Py：读写 Excel
来源：http://ghb.birdmap.top

pandas.read_excel / DataFrame.to_excel
来源：http://sbu.pengpengdd.cyou

[U38] Py：获取脚本所在目录
来源：http://rlp.fktsv.cn

Path(__file__).resolve().parent
来源：http://hrz.zdqjudy.top

[U39] Py：判断是否在交互环境
来源：http://iop.c1oappe.top

sys.stdout.isatty()
来源：http://qhp.yj20258.top

[U40] Py：打印到标准错误
来源：http://bjf.fengsongda.top

print("err", file=sys.stderr)
来源：http://dyz.jiagoushi.top

[U41] PHP：初始化 Composer 项目
来源：http://ibi.shuidangran.top

composer init;  composer require guzzlehttp/guzzle
来源：http://cky.yj20258888.top

[U42] PHP：PSR-4 自动加载
来源：http://hgn.meibo888.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gnt.sjlbkw.cn

[U43] PHP：声明命名空间
来源：http://hkv.zhoulong.xyz

namespace App\Http;
来源：http://mul.hnxiangtu.top

[U44] PHP：开启严格类型
来源：http://gaa.jianghu66.top

declare(strict_types=1);
来源：http://fne.guowangkeji.top

[U45] PHP：类型声明与返回类型
来源：http://dqf.vqdsnc.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://spw.c1oappe.top

[U46] PHP：可空类型
来源：http://uol.nanxinkj.top

?string $name = null
来源：http://qsu.yonumen.top

[U47] PHP：联合类型
来源：http://iuc.yangfankeji.com

int|string $id
来源：http://ipq.bbcook.cn

[U48] PHP：纯枚举
来源：http://cnk.ivvv.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://voi.tanke756.top

[U49] PHP：只读属性
来源：http://cnx.yueranfly.top

public readonly string $name
来源：http://hns.zhongyouzk.top

[U50] PHP：构造器属性提升
来源：http://kaz.316326.xyz

public function __construct(private int $id) {}
来源：http://tpo.kuanghao11.cn

[U51] PHP：数组解构
来源：http://svt.jqgufenzy.top

[$a, $b] = $arr;
来源：http://ysh.jyoumei.cn

[U52] PHP：箭头函数
来源：http://qfp.xziqi.cn

$double = fn($x) => $x * 2;
来源：http://kja.sjlbkw.cn

[U53] PHP：空合并运算符
来源：http://rte.nanxinkj.top

$v = $a ?? $b ?? "default";
来源：http://yzg.cashguo.top

[U54] PHP：空安全调用
来源：http://sch.smart0.xyz

$obj?->method()
来源：http://jro.quarkkingdee.top

[U55] PHP：match 表达式
来源：http://qcu.cucudq.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ucq.shanyushiyangtech.top

[U56] PHP：命名参数
来源：http://yzz.zhijiandao.cn

f(a: 1, b: 2)
来源：http://zpl.zhixingplan.top

[U57] PHP：字符串插值
来源：http://vvr.yueranfly.top

"值: {$a}"
来源：http://hmg.zhoulong.xyz

[U58] PHP：数组三件套
来源：http://jjm.shangyingyoupin.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://drd.hesvh.cn

[U59] PHP：自定义排序
来源：http://hoe.cheryme.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ped.nanxinkj.top

[U60] PHP：JSON 编解码
来源：http://qtl.cucudq.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mly.c1oappe.top

[U61] PHP：正则
来源：http://wti.wangdashe.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kai.bjfxy.top

[U62] PHP：日期对象
来源：http://nvi.zhiwuduotai.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://tgq.ybcxt.top

[U63] PHP：文件读写
来源：http://sdz.sufxvd.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zly.yongpay.top

[U64] PHP：目录遍历
来源：http://eor.meibo888.top

glob("dir/*.php");  scandir("dir");
来源：http://hlt.9152youxi.cn

[U65] PHP：会话
来源：http://cce.chenlongwang.top

session_start();  $_SESSION["uid"] = 1;
来源：http://bxm.jinqigufen.top

[U66] PHP：设置 Cookie
来源：http://skh.jiagoushi.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://toa.cdnleiting.top

[U67] PHP：处理文件上传
来源：http://xgo.c1oappe.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ekf.sjlbkw.cn

[U68] PHP：PDO 连接
来源：http://rvg.kuanghao11.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://uos.shanyushiyangtech.top

[U69] PHP：PDO 预处理
来源：http://mtb.bjfxy.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nmz.wangshuangyany.cn

[U70] PHP：PDO 事务
来源：http://jhw.chenlongwang.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lel.wangshuangyany.cn

[U71] PHP：抛出异常
来源：http://xuj.chenlongwang.top

throw new RuntimeException("失败", 500);
来源：http://ibp.ybcxt.top

[U72] PHP：写错误日志
来源：http://ewr.zdbjq.cn

error_log("失败: " . $e->getMessage());
来源：http://qjo.shanyushiyangkeji.top

[U73] PHP：读取 ini 配置
来源：http://tvh.hysaishi.cn

parse_ini_file("config.ini", true)
来源：http://yev.zhoulong.xyz

[U74] PHP：读取环境变量
来源：http://iwq.ivvv.top

getenv("APP_ENV") ?: "production"
来源：http://jtk.wangdashe.top

[U75] PHP：依赖注入
来源：http://vsj.jianghu66.top

composer require psr/container
来源：http://tvz.kuanghao11.cn

[U76] PHP：简单路由
来源：http://say.yangfankeji.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mti.jqgufenzy.top

[U77] PHP：模板渲染
来源：http://qxg.cheryme.top

composer require twig/twig
来源：http://xmq.xziqi.cn

[U78] PHP：单元测试
来源：http://php.xylfe.cn

composer require --dev phpunit/phpunit
来源：http://xos.haohaochexian.top

[U79] PHP：静态分析
来源：http://qfl.316326.xyz

composer require --dev phpstan/phpstan
来源：http://vjz.yfazqb.com

[U80] PHP：代码规范修复
来源：http://hfc.wangdashe.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://drl.jiagoushi.top

[U81] JS：初始化项目
来源：http://whg.chenjidiqi.icu

npm init -y;  npm i express
来源：http://xlo.zhengqikj.top

[U82] JS：package.json 脚本
来源：http://kbt.daria6918.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jbe.bbcook.cn

[U83] JS：ES Module 导入导出
来源：http://axb.zhijiandao.cn

export const a = 1;  import { a } from "./m.js";
来源：http://nsd.cashguo.top

[U84] JS：CommonJS 写法
来源：http://gjd.hfpthk.cn

module.exports = { a };  const { a } = require("./m");
来源：http://pmr.jinqigfzy.top

[U85] JS：可选链
来源：http://tbp.daria6918.cn

a?.b?.c
来源：http://rnq.yuxming.cn

[U86] JS：空值合并
来源：http://bmn.xziqi.cn

a ?? b
来源：http://agm.fanxiaobao.xyz

[U87] JS：解构默认值
来源：http://rsf.cqqwz.cn

const { a = 1, b = 2 } = obj;
来源：http://idz.jlsjyb.cn

[U88] JS：对象展开合并
来源：http://nfk.jyoumei.cn

{ ...a, ...b }
来源：http://zuj.dianchejie.cn

[U89] JS：数组去重
来源：http://ybx.nanxuanxn.top

[...new Set(arr)]
来源：http://xub.zhengqikj.top

[U90] JS：数字数组排序
来源：http://jjr.yongpay.top

[...arr].sort((a, b) => a - b)
来源：http://vjm.9152youxi.cn

[U91] JS：对象键值遍历
来源：http://ajv.shuidangran.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lkm.yj20258.top

[U92] JS：深拷贝
来源：http://znk.bjfxy.top

structuredClone(obj)
来源：http://emc.jianghu66.top

[U93] JS：模板字符串
来源：http://odx.xingfuxueyuan.xyz

`共 ${n} 条`
来源：http://quz.xuanzx.com

[U94] JS：箭头函数
来源：http://snn.yj202588.top

const double = x => x * 2;
来源：http://kef.jinqigufen.top

[U95] JS：Promise 包装
来源：http://nin.sjlbkw.cn

new Promise((resolve, reject) => {})
来源：http://tqc.gogol.net.cn

[U96] JS：async/await 与异常
来源：http://zco.meibo888.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jhx.52xcode.cn

[U97] JS：并发请求
来源：http://vaq.hysaishi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://edn.ppjwa.cn

[U98] JS：fetch 带 JSON
来源：http://ydk.jiagoushi.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rjd.pengpengdd.cyou

[U99] JS：事件监听
来源：http://zmg.hywenlv.cn

el.addEventListener("click", e => {})
来源：http://xrx.316326.xyz

[U100] JS：DOM 查询
来源：http://ajw.xylfe.cn

document.querySelector(".item")
来源：http://bzu.gzhubu.top

[U101] JS：classList 操作
来源：http://zox.dianchejie.cn

el.classList.toggle("active")
来源：http://kwl.yvedp.cn

[U102] JS：本地存储
来源：http://ipf.ctjpmb.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://vjz.zdbjq.cn

[U103] JS：定时器
来源：http://jlg.fanxiaobao.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://asb.guowangkeji.top

[U104] JS：防抖
来源：http://vqe.shanyushiyangkeji.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eeg.epnwcf.com

[U105] JS：节流
来源：http://fcb.tanke756.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://apm.iojbl.cn

[U106] JS：日期格式化
来源：http://chl.birdmap.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pmu.sufxvd.cn

[U107] JS：数字千分位
来源：http://vjz.hysaishi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gqp.jinghuilouyu.cn

[U108] JS：随机整数
来源：http://ukz.zdbjq.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hpp.gzhubu.top

[U109] JS：数组分组
来源：http://mvh.jyoumei.cn

Object.groupBy(arr, x => x.type)
来源：http://hck.hnqzz.top

[U110] JS：数组分块
来源：http://opk.zdqjudy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ijf.havefunace.top

[U111] JS：对象转 Map
来源：http://gwu.hnxiangtu.top

new Map(Object.entries(obj))
来源：http://iii.zhijiandao.cn

[U112] JS：字符串补位
来源：http://won.52xcode.cn

"7".padStart(3, "0")
来源：http://huz.andypj.xyz

[U113] JS：正则替换全部
来源：http://dcp.sjlbkw.cn

s.replaceAll("a", "b")
来源：http://sco.fktsv.cn

[U114] JS：JSON 深比较
来源：http://khl.yuxming.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://fec.hesvh.cn

[U115] JS：生成 UUID
来源：http://svp.hnqzz.top

crypto.randomUUID()
来源：http://mpc.tarul.cn

[U116] JS：类型检查（JSDoc）
来源：http://tgx.gotoacloud.top

/** @param {string} name */ function f(name) {}
来源：http://oup.hongshengwenyu.top

[U117] JS：单元测试
来源：http://ruu.wangdashe.top

npm i -D vitest;  npx vitest
来源：http://fxh.xziqi.cn

[U118] JS：开发服务器
来源：http://caq.fehbvm.com

npm i -D vite;  npx vite
来源：http://lru.yj20258.top

[U119] JS：生产构建
来源：http://gaq.daria6918.cn

npx vite build
来源：http://qou.gotoacloud.top

[U120] JS：读取环境变量（Vite）
来源：http://ood.zhengqikj.top

import.meta.env.VITE_API_URL
来源：http://ihf.wangdashe.top

================================================================================
来源：http://lfw.xylfe.cn

统计汇总
来源：http://xzo.chenzaomai.com

================================================================================
来源：http://bdn.zhongyouzk.top

按语言统计（条）：
来源：http://tlm.zhengqikj.top

Python ......... 252
来源：http://ffy.9152youxi.cn

PHP ............ 252
来源：http://xyf.ivvv.top

JavaScript ..... 252
来源：http://zhz.havefunace.top

TypeScript ..... 212
来源：http://ixo.yonumen.top

Java ........... 212
来源：http://xmo.wangshuangyany.cn

Go ............. 212
来源：http://szp.yonumen.top

Ruby ........... 212
来源：http://jzj.hysaishi.cn

C# ............. 212
来源：http://zpc.ehwqpu.com

C .............. 30
来源：http://ngn.chenjidiqi.icu

C++ ............ 30
来源：http://our.fengsongda.top

SQL ............ 90
来源：http://dah.aizwys.cn

Bash ........... 80
来源：http://jdx.cqqwz.cn

Kotlin ......... 15
来源：http://lhz.chenlongwang.top

Swift .......... 15
来源：http://ngo.9152youxi.cn

Lua ............ 10
来源：http://hhn.ppjwa.cn

Perl ........... 10
来源：http://xqn.sufxvd.cn

Scala .......... 10
来源：http://dib.yueranfly.top

------------------------------------
来源：http://gop.nanxuanxn.top

合计 ........... 2106 条
来源：http://tfc.jinyuanbaomall.cn

按章节统计：
来源：http://opl.yonumen.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://nul.pengpengdd.cyou

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://geo.uphjek.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pcj.sufxvd.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://les.ehwqpu.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ldg.hnxiangtu.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://kfm.xingfuxueyuan.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://pee.jlsjyb.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://bxs.sysykeji.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://tcu.jqgufenzy.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://avs.andypj.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bpv.zhiwuduotai.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dew.wangdashe.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rpw.fanxiaobao.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hhq.gotoacloud.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yti.tian-w.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://gws.ppjwa.cn

Q SQL 专题                              90
来源：http://kkf.jlsjyb.cn

R Bash 专题                             80
来源：http://aut.ybcxt.top

S C / C++ 专题                          60
来源：http://amq.cqqwz.cn

T 其他语言补充                          60
来源：http://zoi.jqgfzy.top

U 高频实用片段                         120
来源：http://gyv.yueranfly.top

------------------------------------
来源：http://zrq.sxryk.cn

合计                                  2106 条
来源：http://xti.cdnleiting.top

--------------------------------------------------------------------------------
来源：http://oul.gzhubu.top

使用提醒
来源：http://cvi.hongshengwenyu.top

--------------------------------------------------------------------------------
来源：http://wfa.xuanzx.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nil.wangdashe.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://yos.fzhhl.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ooz.yvedp.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://zxe.52xcode.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://uxx.yj20258888.top

—— 文件结束 ——
来源：http://kod.gzhubu.top

================================================================================
来源：http://jlo.svipenyu.cn

程序语言常见例子速查手册（2024 版）
来源：http://iej.yj20258888.top

Common Programming Examples Cheat Book
来源：http://okt.zhengqikj.top

================================================================================
来源：http://wng.yongpay.top

【收录内容】
来源：http://jha.shzxlz.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://olc.tianlin.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://qgy.epnwcf.com

SQL · Bash · C · C++
来源：http://qef.feifeiyinyue.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hkt.cdnleiting.top

【使用说明】
来源：http://lia.zycfv.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wks.gogol.net.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hol.shanyushiyangkeji.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ruy.svipenyu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://aiz.havefunace.top

Bash:  Shell         C:     C             C++:   C++
来源：http://xec.quarkkingdee.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://eng.haohaochexian.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ylx.jianghu66.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hgz.zdqjudy.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://pen.uphjek.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://cuz.fzhhl.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hrf.jqgfzy.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://tau.meibo888.top

【文件统计】
来源：http://njm.ctjpmb.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://jhj.jyoumei.cn

--------------------------------------------------------------------------------
来源：http://nul.xuetiantiany.cn

目  录
来源：http://rfz.shuidangran.top

--------------------------------------------------------------------------------
来源：http://irq.ctjpmb.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wvg.haohaochexian.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://bpk.ppjwa.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ilh.tarul.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://tel.sysykeji.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://sox.chenlongwang.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gsr.yj20258888.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://smg.tianlin.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://pbf.aizwys.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zfj.tian-w.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://svw.yonumen.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://fjy.sjlbkw.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://uab.jianghu66.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://yxq.cqqwz.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://upr.jqgfzy.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jmv.cashguo.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rll.dianchejie.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hoo.zhoulong.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://rie.zhengqikj.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ina.ybcxt.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://sgp.yangfankeji.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://iym.sysykeji.top

================================================================================
来源：http://ypq.cheryme.top

A. 基础语法与类型
来源：http://idy.cqqwz.cn

================================================================================
来源：http://oza.yangfankeji.com

[A01] Hello World
来源：http://erg.vehdjk.com


<!-- 参考信息 -->