代发 wailian999

[U25] Py：CSV 按字典读
来源：http://lwj.hfpthk.cn

csv.DictReader(f)
来源：http://ebh.fehbvm.com

[U26] Py：并发下载
来源：http://kto.dianchejie.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wyz.yfazqb.com

[U27] Py：异步 HTTP
来源：http://abr.kuanghao11.cn

aiohttp.ClientSession() 配合 async with
来源：http://sea.xziqi.cn

[U28] Py：类型别名
来源：http://fvv.ehwqpu.com

UserId = int
来源：http://qfr.cheryme.top

[U29] Py：属性校验
来源：http://xmh.xuetiantiany.cn

@property 与 @x.setter 配合
来源：http://nmz.zhaomingkeji.xyz

[U30] Py：数据类
来源：http://rkd.ctjpmb.com

@dataclass(slots=True)
来源：http://gsb.nanxinkj.top

[U31] Py：单测
来源：http://qal.hongshengwenyu.top

python -m pytest -q
来源：http://emu.havefunace.top

[U32] Py：代码格式化
来源：http://zvo.ctjpmb.com

ruff format . && ruff check --fix .
来源：http://rdi.shanyushiyangtech.top

[U33] Py：打包发布
来源：http://spf.zhiwuduotai.top

python -m build  （依赖 pyproject.toml）
来源：http://gzi.yanxiufei.cn

[U34] Py：判断编码
来源：http://kzk.sufxvd.cn

chardet.detect(raw)
来源：http://hca.gotoacloud.top

[U35] Py：发送邮件
来源：http://piz.pengpengdd.cyou

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zij.shangyingyoupin.top

[U36] Py：定时任务
来源：http://dgf.52xcode.cn

schedule.every(10).minutes.do(job)
来源：http://fhm.fehbvm.com

[U37] Py：读写 Excel
来源：http://gys.yj20258.top

pandas.read_excel / DataFrame.to_excel
来源：http://xid.fengsongda.top

[U38] Py：获取脚本所在目录
来源：http://akz.ppjwa.cn

Path(__file__).resolve().parent
来源：http://pre.wangdashe.top

[U39] Py：判断是否在交互环境
来源：http://znf.gotoacloud.top

sys.stdout.isatty()
来源：http://agu.zhaomingkeji.xyz

[U40] Py：打印到标准错误
来源：http://gtl.gzhubu.top

print("err", file=sys.stderr)
来源：http://oor.hnqzz.top

[U41] PHP：初始化 Composer 项目
来源：http://xml.hammf.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://nds.ppjwa.cn

[U42] PHP：PSR-4 自动加载
来源：http://eca.zhongyouzk.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://sbf.zhongyouzk.top

[U43] PHP：声明命名空间
来源：http://bxm.haohaochexian.top

namespace App\Http;
来源：http://wxj.zdbjq.cn

[U44] PHP：开启严格类型
来源：http://fsv.ywan-chungtsiang.top

declare(strict_types=1);
来源：http://tmd.fengsongda.top

[U45] PHP：类型声明与返回类型
来源：http://bhx.yfazqb.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://wyw.zhaomingkeji.xyz

[U46] PHP：可空类型
来源：http://mvm.yj20258888.top

?string $name = null
来源：http://fxa.gogol.net.cn

[U47] PHP：联合类型
来源：http://njw.gaohongyu789.top

int|string $id
来源：http://mzm.zdbjq.cn

[U48] PHP：纯枚举
来源：http://cge.zhixingplan.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kae.jqgfzy.top

[U49] PHP：只读属性
来源：http://zvo.sufxvd.cn

public readonly string $name
来源：http://bui.yj20258.top

[U50] PHP：构造器属性提升
来源：http://dnq.hnxiangtu.top

public function __construct(private int $id) {}
来源：http://tbe.tarul.cn

[U51] PHP：数组解构
来源：http://qpe.gzhubu.top

[$a, $b] = $arr;
来源：http://mph.mhx1999.top

[U52] PHP：箭头函数
来源：http://lrj.52xcode.cn

$double = fn($x) => $x * 2;
来源：http://upk.jiagoushi.top

[U53] PHP：空合并运算符
来源：http://gmf.cheryme.top

$v = $a ?? $b ?? "default";
来源：http://oek.zhoulong.xyz

[U54] PHP：空安全调用
来源：http://wtj.ehwqpu.com

$obj?->method()
来源：http://diq.fanxiaobao.xyz

[U55] PHP：match 表达式
来源：http://icb.uphjek.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yho.sysykeji.top

[U56] PHP：命名参数
来源：http://dac.hywenlv.cn

f(a: 1, b: 2)
来源：http://lkl.shangyingyoupin.top

[U57] PHP：字符串插值
来源：http://ivf.hnqzz.top

"值: {$a}"
来源：http://pok.tarul.cn

[U58] PHP：数组三件套
来源：http://uzb.wangshuangyany.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ivi.ydjk.org.cn

[U59] PHP：自定义排序
来源：http://kvf.fanxiaobao.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tqe.ybcxt.top

[U60] PHP：JSON 编解码
来源：http://iyd.fehbvm.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://frp.cashguo.top

[U61] PHP：正则
来源：http://isy.daxiang520.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ioz.bjfxy.top

[U62] PHP：日期对象
来源：http://eif.hammf.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lnn.jlsjyb.cn

[U63] PHP：文件读写
来源：http://kkp.dianchejie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mef.zdbjq.cn

[U64] PHP：目录遍历
来源：http://bwa.shuidangran.top

glob("dir/*.php");  scandir("dir");
来源：http://zfs.shuidangran.top

[U65] PHP：会话
来源：http://jmn.sufxvd.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://jls.tanke756.top

[U66] PHP：设置 Cookie
来源：http://itu.ywan-chungtsiang.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fmc.havefunace.top

[U67] PHP：处理文件上传
来源：http://izw.redwolf501.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jth.sweek.top

[U68] PHP：PDO 连接
来源：http://klb.sysykeji.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qqo.epnwcf.com

[U69] PHP：PDO 预处理
来源：http://iue.yvedp.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zha.zhiwuduotai.top

[U70] PHP：PDO 事务
来源：http://ovj.yongpay.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://llu.0kj1m.cn

[U71] PHP：抛出异常
来源：http://avb.hammf.cn

throw new RuntimeException("失败", 500);
来源：http://ibh.hcnkem.com

[U72] PHP：写错误日志
来源：http://knw.jianghu66.top

error_log("失败: " . $e->getMessage());
来源：http://jjl.hammf.cn

[U73] PHP：读取 ini 配置
来源：http://kkq.zhoulong.xyz

parse_ini_file("config.ini", true)
来源：http://aon.hnqzz.top

[U74] PHP：读取环境变量
来源：http://eex.yangfankeji.com

getenv("APP_ENV") ?: "production"
来源：http://ius.ydzc1.top

[U75] PHP：依赖注入
来源：http://thv.yuxming.cn

composer require psr/container
来源：http://enq.redwolf501.top

[U76] PHP：简单路由
来源：http://fsv.ctjpmb.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xfl.ywan-chungtsiang.top

[U77] PHP：模板渲染
来源：http://efw.hysaishi.cn

composer require twig/twig
来源：http://igs.jiagoushi.top

[U78] PHP：单元测试
来源：http://nwe.yvedp.cn

composer require --dev phpunit/phpunit
来源：http://kiq.hongshengwenyu.top

[U79] PHP：静态分析
来源：http://shb.zhengqikj.top

composer require --dev phpstan/phpstan
来源：http://fav.yuxming.cn

[U80] PHP：代码规范修复
来源：http://hnx.sweek.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://vcv.dianchejie.cn

[U81] JS：初始化项目
来源：http://olc.sjlbkw.cn

npm init -y;  npm i express
来源：http://hox.jqgfzy.top

[U82] JS：package.json 脚本
来源：http://hxa.jiagoushi.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hue.fktsv.cn

[U83] JS：ES Module 导入导出
来源：http://lrq.zhoulong.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://wwf.c1oappe.top

[U84] JS：CommonJS 写法
来源：http://vue.snrcjt.cn

module.exports = { a };  const { a } = require("./m");
来源：http://yrx.yj202588.top

[U85] JS：可选链
来源：http://cpj.xylfe.cn

a?.b?.c
来源：http://uei.sjlbkw.cn

[U86] JS：空值合并
来源：http://qku.bjfxy.top

a ?? b
来源：http://owa.hcnkem.com

[U87] JS：解构默认值
来源：http://obj.xuanzx.com

const { a = 1, b = 2 } = obj;
来源：http://pfr.zhiwuduotai.top

[U88] JS：对象展开合并
来源：http://ujo.pycfn.com

{ ...a, ...b }
来源：http://egx.quarkkingdee.top

[U89] JS：数组去重
来源：http://qxp.jinqigfzy.top

[...new Set(arr)]
来源：http://vtv.hfpthk.cn

[U90] JS：数字数组排序
来源：http://zqv.fengsongda.top

[...arr].sort((a, b) => a - b)
来源：http://yvh.yanxiufei.cn

[U91] JS：对象键值遍历
来源：http://wci.hysaishi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://puj.nanxinkj.top

[U92] JS：深拷贝
来源：http://zkw.zdbjq.cn

structuredClone(obj)
来源：http://fgy.smart0.xyz

[U93] JS：模板字符串
来源：http://vog.shanyushiyangtech.top

`共 ${n} 条`
来源：http://oic.sufxvd.cn

[U94] JS：箭头函数
来源：http://ywf.zycfv.cn

const double = x => x * 2;
来源：http://vdq.shzxlz.cn

[U95] JS：Promise 包装
来源：http://pdg.jinyuanbaomall.cn

new Promise((resolve, reject) => {})
来源：http://nkw.9152youxi.cn

[U96] JS：async/await 与异常
来源：http://bhz.hnxiangtu.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wha.pycfn.com

[U97] JS：并发请求
来源：http://rtm.tian-w.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://rvp.yj20258888.top

[U98] JS：fetch 带 JSON
来源：http://lam.nanxuanxn.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zbc.quarkkingdee.top

[U99] JS：事件监听
来源：http://via.aibaodan.cn

el.addEventListener("click", e => {})
来源：http://kpx.jianghu66.top

[U100] JS：DOM 查询
来源：http://brz.xylfe.cn

document.querySelector(".item")
来源：http://mki.dianchejie.cn

[U101] JS：classList 操作
来源：http://hlv.bjfxy.top

el.classList.toggle("active")
来源：http://hnq.bjfxy.top

[U102] JS：本地存储
来源：http://goj.hywenlv.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://mbr.jyoumei.cn

[U103] JS：定时器
来源：http://rnj.shangyingyoupin.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qsq.tian-w.cn

[U104] JS：防抖
来源：http://ssl.zhixingplan.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ofi.jqgfzy.top

[U105] JS：节流
来源：http://qhr.yuxming.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xiy.daxiang520.top

[U106] JS：日期格式化
来源：http://xnl.nwbrower.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qrg.wangshuangyany.cn

[U107] JS：数字千分位
来源：http://sxa.xylfe.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lsk.cheryme.top

[U108] JS：随机整数
来源：http://weg.nanxinkj.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://csx.svipenyu.cn

[U109] JS：数组分组
来源：http://brl.yueranfly.top

Object.groupBy(arr, x => x.type)
来源：http://mlq.birdmap.top

[U110] JS：数组分块
来源：http://lxg.chenzaomai.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vzx.chenjidiqi.icu

[U111] JS：对象转 Map
来源：http://xpi.yonumen.top

new Map(Object.entries(obj))
来源：http://odq.zhixingplan.top

[U112] JS：字符串补位
来源：http://npr.xingfuxueyuan.xyz

"7".padStart(3, "0")
来源：http://zvv.ydjk.org.cn

[U113] JS：正则替换全部
来源：http://rim.jinyuanbaomall.cn

s.replaceAll("a", "b")
来源：http://knr.9152youxi.cn

[U114] JS：JSON 深比较
来源：http://vru.haohaochexian.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://rrr.zhijiandao.cn

[U115] JS：生成 UUID
来源：http://twj.yvedp.cn

crypto.randomUUID()
来源：http://yhw.hywenlv.cn

[U116] JS：类型检查（JSDoc）
来源：http://beg.tarul.cn

/** @param {string} name */ function f(name) {}
来源：http://xkd.yuanzhike.top

[U117] JS：单元测试
来源：http://xnn.yfazqb.com

npm i -D vitest;  npx vitest
来源：http://ywt.52xcode.cn

[U118] JS：开发服务器
来源：http://jvb.xingfuxueyuan.xyz

npm i -D vite;  npx vite
来源：http://zuz.wangdashe.top

[U119] JS：生产构建
来源：http://pwv.xziqi.cn

npx vite build
来源：http://cin.jinqigufen.top

[U120] JS：读取环境变量（Vite）
来源：http://bgs.ehwqpu.com

import.meta.env.VITE_API_URL
来源：http://fco.uphjek.com

================================================================================
来源：http://gnl.fengsongda.top

统计汇总
来源：http://ctz.birdmap.top

================================================================================
来源：http://xsk.shanyushiyangtech.top

按语言统计（条）：
来源：http://mfh.hfpthk.cn

Python ......... 252
来源：http://nyc.xingfuxueyuan.xyz

PHP ............ 252
来源：http://pmt.hongshengwenyu.top

JavaScript ..... 252
来源：http://bza.316326.xyz

TypeScript ..... 212
来源：http://ipn.jqgfzy.top

Java ........... 212
来源：http://jfl.yuxming.cn

Go ............. 212
来源：http://odx.yueranfly.top

Ruby ........... 212
来源：http://nul.fzhhl.top

C# ............. 212
来源：http://xdz.jinghuilouyu.cn

C .............. 30
来源：http://dno.hysaishi.cn

C++ ............ 30
来源：http://afn.zhiwuduotai.top

SQL ............ 90
来源：http://eep.ehwqpu.com

Bash ........... 80
来源：http://ocs.meibo888.top

Kotlin ......... 15
来源：http://sgd.hongshengwenyu.top

Swift .......... 15
来源：http://cgj.cdnleiting.top

Lua ............ 10
来源：http://ejv.havefunace.top

Perl ........... 10
来源：http://asx.jiagoushi.top

Scala .......... 10
来源：http://gln.zycfv.cn

------------------------------------
来源：http://mbh.bjfxy.top

合计 ........... 2106 条
来源：http://jag.fktsv.cn

按章节统计：
来源：http://xhp.mhx1999.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://knm.zdqjudy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://oit.jinqigfzy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mzi.gogol.net.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://cve.chenzaomai.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fiw.0kj1m.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dpz.havefunace.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://uko.cheryme.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://pya.jyoumei.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bgt.cheryme.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://flr.shanyushiyangtech.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://yrw.hfpthk.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://bna.jinqigfzy.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://udq.jiagoushi.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jig.guannengcc.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qkd.yj202588.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://luv.zhoulong.xyz

Q SQL 专题                              90
来源：http://lww.vqdsnc.cn

R Bash 专题                             80
来源：http://ujq.ybcxt.top

S C / C++ 专题                          60
来源：http://yga.jinqigfzy.top

T 其他语言补充                          60
来源：http://uqs.shanyushiyangkeji.top

U 高频实用片段                         120
来源：http://fln.ppjwa.cn

------------------------------------
来源：http://tmn.cqqwz.cn

合计                                  2106 条
来源：http://cei.ydjk.org.cn

--------------------------------------------------------------------------------
来源：http://jzw.sysykeji.top

使用提醒
来源：http://dcr.52xcode.cn

--------------------------------------------------------------------------------
来源：http://fcy.daxiang520.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vhm.shzxlz.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hig.316326.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ndo.smart0.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://tkb.quarkkingdee.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://abc.svipenyu.cn

—— 文件结束 ——
来源：http://bvf.fanxiaobao.xyz

================================================================================
来源：http://ynn.52xcode.cn

程序语言常见例子速查手册（2024 版）
来源：http://xsk.haohaochexian.top

Common Programming Examples Cheat Book
来源：http://gwf.tarul.cn

================================================================================
来源：http://rta.zhaomingkeji.xyz

【收录内容】
来源：http://bjb.hywenlv.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ubk.birdmap.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://fca.yuxming.cn

SQL · Bash · C · C++
来源：http://xbk.hnqzz.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://rzx.xuanzx.com

【使用说明】
来源：http://kha.hcnkem.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gfc.jinqigufen.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://uoa.yj20258888.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://xko.yj20258.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qfl.dianchejie.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://mbx.sjlbkw.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://fue.zycfv.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://sch.yueranfly.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://upu.nanxinkj.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xql.shanyushiyangkeji.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hgj.zhaomingkeji.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://aey.jinqigfzy.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://cmf.yfazqb.com

【文件统计】
来源：http://yjq.zdbjq.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wek.bjfxy.top

--------------------------------------------------------------------------------
来源：http://wxd.0kj1m.cn

目  录
来源：http://wrb.zhijiandao.cn

--------------------------------------------------------------------------------
来源：http://qlx.zdbjq.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ezl.zhoulong.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://pez.vehdjk.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fip.yuxming.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://pju.fktsv.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ycv.jinghuilouyu.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://nem.guannengcc.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://scx.zdbjq.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hyk.yonumen.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hxd.haohaochexian.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://amp.cdnleiting.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ukr.hnxiangtu.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://vhk.tianlin.xyz

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://nmi.ctjpmb.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://beo.fzhhl.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ouv.xingfuxueyuan.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://dkd.smart0.xyz

Q. SQL 专题                    （第 17 节，90 条）
来源：http://zkg.bbcook.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://cse.yanxiufei.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://igq.dashuyun.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://cqd.daxiang520.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ixk.ppjwa.cn

================================================================================
来源：http://cjh.zhiwuduotai.top

A. 基础语法与类型
来源：http://csx.yueranfly.top

================================================================================
来源：http://rcx.cqqwz.cn

[A01] Hello World
来源：http://tpz.tanke756.top


<!-- 参考信息 -->