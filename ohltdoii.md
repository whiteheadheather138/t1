代发 wailian999

[U23] Py：分块读取大文件
来源：http://vtv.jqgufenzy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ctg.iojbl.cn

[U24] Py：路径操作
来源：http://jwq.yongpay.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://chi.birdmap.top

[U25] Py：CSV 按字典读
来源：http://inh.shzxlz.cn

csv.DictReader(f)
来源：http://rel.chenzaomai.com

[U26] Py：并发下载
来源：http://mkj.pengpengdd.cyou

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nwc.zhongyouzk.top

[U27] Py：异步 HTTP
来源：http://ncy.wangdashe.top

aiohttp.ClientSession() 配合 async with
来源：http://dix.quarkkingdee.top

[U28] Py：类型别名
来源：http://mzo.guowangkeji.top

UserId = int
来源：http://qbf.jinqigufen.top

[U29] Py：属性校验
来源：http://gve.nanxuanxn.top

@property 与 @x.setter 配合
来源：http://nfc.gotoacloud.top

[U30] Py：数据类
来源：http://hje.9152youxi.cn

@dataclass(slots=True)
来源：http://chh.xingfuxueyuan.xyz

[U31] Py：单测
来源：http://vus.zhixingplan.top

python -m pytest -q
来源：http://rvc.zhiwuduotai.top

[U32] Py：代码格式化
来源：http://afr.xuetiantiany.cn

ruff format . && ruff check --fix .
来源：http://mrh.shanyushiyangtech.top

[U33] Py：打包发布
来源：http://cxh.cheryme.top

python -m build  （依赖 pyproject.toml）
来源：http://itn.epnwcf.com

[U34] Py：判断编码
来源：http://mst.hywenlv.cn

chardet.detect(raw)
来源：http://aqh.ppjwa.cn

[U35] Py：发送邮件
来源：http://weh.tanke756.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dra.jinqigfzy.top

[U36] Py：定时任务
来源：http://sdb.sufxvd.cn

schedule.every(10).minutes.do(job)
来源：http://hpq.jlsjyb.cn

[U37] Py：读写 Excel
来源：http://dhl.zdbjq.cn

pandas.read_excel / DataFrame.to_excel
来源：http://vrs.zhijiandao.cn

[U38] Py：获取脚本所在目录
来源：http://hqt.uphjek.com

Path(__file__).resolve().parent
来源：http://wws.xziqi.cn

[U39] Py：判断是否在交互环境
来源：http://fzn.snrcjt.cn

sys.stdout.isatty()
来源：http://qru.zhongyouzk.top

[U40] Py：打印到标准错误
来源：http://kjr.gotoacloud.top

print("err", file=sys.stderr)
来源：http://jzy.cdnleiting.top

[U41] PHP：初始化 Composer 项目
来源：http://prq.hfpthk.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://hpm.andypj.xyz

[U42] PHP：PSR-4 自动加载
来源：http://fwg.tianlin.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yls.ppjwa.cn

[U43] PHP：声明命名空间
来源：http://fni.cashguo.top

namespace App\Http;
来源：http://coi.yueranfly.top

[U44] PHP：开启严格类型
来源：http://mqi.fengsongda.top

declare(strict_types=1);
来源：http://sqc.yj202588.top

[U45] PHP：类型声明与返回类型
来源：http://jon.kuanghao11.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://hfk.ehwqpu.com

[U46] PHP：可空类型
来源：http://crv.svipenyu.cn

?string $name = null
来源：http://vfm.bbcook.cn

[U47] PHP：联合类型
来源：http://hgd.yj20258.top

int|string $id
来源：http://ygb.jyoumei.cn

[U48] PHP：纯枚举
来源：http://tas.jianghu66.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vit.zycfv.cn

[U49] PHP：只读属性
来源：http://gwn.ctjpmb.com

public readonly string $name
来源：http://fph.smart0.xyz

[U50] PHP：构造器属性提升
来源：http://aow.jqgufenzy.top

public function __construct(private int $id) {}
来源：http://ytm.chenzaomai.com

[U51] PHP：数组解构
来源：http://idv.sjlbkw.cn

[$a, $b] = $arr;
来源：http://sgd.smart0.xyz

[U52] PHP：箭头函数
来源：http://ehe.sweek.top

$double = fn($x) => $x * 2;
来源：http://ssg.shanyushiyangtech.top

[U53] PHP：空合并运算符
来源：http://ejp.jinyuanbaomall.cn

$v = $a ?? $b ?? "default";
来源：http://wpd.wangdashe.top

[U54] PHP：空安全调用
来源：http://dsf.fehbvm.com

$obj?->method()
来源：http://ien.hnqzz.top

[U55] PHP：match 表达式
来源：http://ebv.iojbl.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://axn.yj20258.top

[U56] PHP：命名参数
来源：http://vss.316326.xyz

f(a: 1, b: 2)
来源：http://eco.tanke756.top

[U57] PHP：字符串插值
来源：http://ohn.aizwys.cn

"值: {$a}"
来源：http://muw.xuetiantiany.cn

[U58] PHP：数组三件套
来源：http://vwd.jyoumei.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rae.aizwys.cn

[U59] PHP：自定义排序
来源：http://stm.uphjek.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nys.yongpay.top

[U60] PHP：JSON 编解码
来源：http://mxi.jinqigufen.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://uop.ydzc1.top

[U61] PHP：正则
来源：http://rwq.andypj.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hav.hfpthk.cn

[U62] PHP：日期对象
来源：http://kwm.havefunace.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://cvv.bjfxy.top

[U63] PHP：文件读写
来源：http://ozv.ybcxt.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ddy.yueranfly.top

[U64] PHP：目录遍历
来源：http://jcp.chenjidiqi.icu

glob("dir/*.php");  scandir("dir");
来源：http://nii.cqqwz.cn

[U65] PHP：会话
来源：http://qai.hcnkem.com

session_start();  $_SESSION["uid"] = 1;
来源：http://sci.ywan-chungtsiang.top

[U66] PHP：设置 Cookie
来源：http://tyl.tian-w.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ick.cdnleiting.top

[U67] PHP：处理文件上传
来源：http://kgu.redwolf501.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://aif.jyoumei.cn

[U68] PHP：PDO 连接
来源：http://xsp.smart0.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://dvs.hysaishi.cn

[U69] PHP：PDO 预处理
来源：http://jjb.hnqzz.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lun.ctjpmb.com

[U70] PHP：PDO 事务
来源：http://iqv.gotoacloud.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ido.yangfankeji.com

[U71] PHP：抛出异常
来源：http://pmr.yangfankeji.com

throw new RuntimeException("失败", 500);
来源：http://nxy.hammf.cn

[U72] PHP：写错误日志
来源：http://fcm.gzhubu.top

error_log("失败: " . $e->getMessage());
来源：http://jac.yj20258888.top

[U73] PHP：读取 ini 配置
来源：http://qsy.snrcjt.cn

parse_ini_file("config.ini", true)
来源：http://xwq.dashuyun.cn

[U74] PHP：读取环境变量
来源：http://tbp.ppjwa.cn

getenv("APP_ENV") ?: "production"
来源：http://vsj.wangshuangyany.cn

[U75] PHP：依赖注入
来源：http://krl.xylfe.cn

composer require psr/container
来源：http://ebw.9152youxi.cn

[U76] PHP：简单路由
来源：http://yze.epnwcf.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ebr.gogol.net.cn

[U77] PHP：模板渲染
来源：http://ktx.gzhubu.top

composer require twig/twig
来源：http://okh.andypj.xyz

[U78] PHP：单元测试
来源：http://xyw.cheryme.top

composer require --dev phpunit/phpunit
来源：http://ttm.xuanzx.com

[U79] PHP：静态分析
来源：http://wps.sxryk.cn

composer require --dev phpstan/phpstan
来源：http://mmy.nwbrower.top

[U80] PHP：代码规范修复
来源：http://amf.gaohongyu789.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://okx.chenzaomai.com

[U81] JS：初始化项目
来源：http://rrg.ppjwa.cn

npm init -y;  npm i express
来源：http://wjy.zhoulong.xyz

[U82] JS：package.json 脚本
来源：http://yep.cucudq.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kek.jyoumei.cn

[U83] JS：ES Module 导入导出
来源：http://xud.guowangkeji.top

export const a = 1;  import { a } from "./m.js";
来源：http://gik.ppjwa.cn

[U84] JS：CommonJS 写法
来源：http://cln.svipenyu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://mrg.chenlongwang.top

[U85] JS：可选链
来源：http://onq.tian-w.cn

a?.b?.c
来源：http://hvj.nanxinkj.top

[U86] JS：空值合并
来源：http://nhk.hfpthk.cn

a ?? b
来源：http://rwr.mhx1999.top

[U87] JS：解构默认值
来源：http://tfm.yueranfly.top

const { a = 1, b = 2 } = obj;
来源：http://dac.jinyuanbaomall.cn

[U88] JS：对象展开合并
来源：http://uyz.pengpengdd.cyou

{ ...a, ...b }
来源：http://kms.jianghu66.top

[U89] JS：数组去重
来源：http://tjz.ydzc1.top

[...new Set(arr)]
来源：http://fmo.bbcook.cn

[U90] JS：数字数组排序
来源：http://rzs.fktsv.cn

[...arr].sort((a, b) => a - b)
来源：http://jbv.hnqzz.top

[U91] JS：对象键值遍历
来源：http://gpq.sysykeji.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://iig.fehbvm.com

[U92] JS：深拷贝
来源：http://hqt.zdbjq.cn

structuredClone(obj)
来源：http://iga.nanxinkj.top

[U93] JS：模板字符串
来源：http://rlb.zhixingplan.top

`共 ${n} 条`
来源：http://usl.vqdsnc.cn

[U94] JS：箭头函数
来源：http://ita.yfazqb.com

const double = x => x * 2;
来源：http://pdd.quarkkingdee.top

[U95] JS：Promise 包装
来源：http://yoi.jiagoushi.top

new Promise((resolve, reject) => {})
来源：http://xxa.andypj.xyz

[U96] JS：async/await 与异常
来源：http://fvw.fengsongda.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zaw.gzhubu.top

[U97] JS：并发请求
来源：http://ozl.c1oappe.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ukm.zdqjudy.top

[U98] JS：fetch 带 JSON
来源：http://lwz.kuanghao11.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ytd.sxryk.cn

[U99] JS：事件监听
来源：http://mvw.jqgfzy.top

el.addEventListener("click", e => {})
来源：http://ece.bjfxy.top

[U100] JS：DOM 查询
来源：http://iey.hfpthk.cn

document.querySelector(".item")
来源：http://sup.fktsv.cn

[U101] JS：classList 操作
来源：http://utk.9152youxi.cn

el.classList.toggle("active")
来源：http://zvq.birdmap.top

[U102] JS：本地存储
来源：http://exz.ehwqpu.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://vqe.dashuyun.cn

[U103] JS：定时器
来源：http://vsx.xylfe.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://sec.yueranfly.top

[U104] JS：防抖
来源：http://oic.yangfankeji.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zov.shangyingyoupin.top

[U105] JS：节流
来源：http://bxt.sxryk.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://npt.wangdashe.top

[U106] JS：日期格式化
来源：http://tig.316326.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ida.zhiwuduotai.top

[U107] JS：数字千分位
来源：http://tle.xinyue.icu

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zjp.zdbjq.cn

[U108] JS：随机整数
来源：http://kvr.yueranfly.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://psh.chenjidiqi.icu

[U109] JS：数组分组
来源：http://pnx.shzxlz.cn

Object.groupBy(arr, x => x.type)
来源：http://nrg.fktsv.cn

[U110] JS：数组分块
来源：http://jjj.pengpengdd.cyou

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nct.daria6918.cn

[U111] JS：对象转 Map
来源：http://igh.shanyushiyangkeji.top

new Map(Object.entries(obj))
来源：http://job.yanxiufei.cn

[U112] JS：字符串补位
来源：http://yzw.zhengqikj.top

"7".padStart(3, "0")
来源：http://dit.aizwys.cn

[U113] JS：正则替换全部
来源：http://czx.xylfe.cn

s.replaceAll("a", "b")
来源：http://nic.52xcode.cn

[U114] JS：JSON 深比较
来源：http://vlh.nanxinkj.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://jql.xuanzx.com

[U115] JS：生成 UUID
来源：http://kal.vehdjk.com

crypto.randomUUID()
来源：http://qmm.cashguo.top

[U116] JS：类型检查（JSDoc）
来源：http://lmh.sweek.top

/** @param {string} name */ function f(name) {}
来源：http://bic.yj202588.top

[U117] JS：单元测试
来源：http://ktf.haohaochexian.top

npm i -D vitest;  npx vitest
来源：http://cls.haohaochexian.top

[U118] JS：开发服务器
来源：http://toz.fehbvm.com

npm i -D vite;  npx vite
来源：http://lbj.jinyuanbaomall.cn

[U119] JS：生产构建
来源：http://edf.zhijiandao.cn

npx vite build
来源：http://loz.shuidangran.top

[U120] JS：读取环境变量（Vite）
来源：http://gzp.quarkkingdee.top

import.meta.env.VITE_API_URL
来源：http://huf.zhaomingkeji.xyz

================================================================================
来源：http://kmr.dianchejie.cn

统计汇总
来源：http://onr.meibo888.top

================================================================================
来源：http://vqg.xuanzx.com

按语言统计（条）：
来源：http://krc.jianghu66.top

Python ......... 252
来源：http://eyh.ppjwa.cn

PHP ............ 252
来源：http://jzn.bbcook.cn

JavaScript ..... 252
来源：http://emc.yuxming.cn

TypeScript ..... 212
来源：http://lxt.bbcook.cn

Java ........... 212
来源：http://wno.jlsjyb.cn

Go ............. 212
来源：http://ple.hnqzz.top

Ruby ........... 212
来源：http://yuz.ppjwa.cn

C# ............. 212
来源：http://zme.shangyingyoupin.top

C .............. 30
来源：http://twv.fanxiaobao.xyz

C++ ............ 30
来源：http://fup.52xcode.cn

SQL ............ 90
来源：http://lws.zhixingplan.top

Bash ........... 80
来源：http://wef.hnqzz.top

Kotlin ......... 15
来源：http://gtd.jlsjyb.cn

Swift .......... 15
来源：http://jjj.yvedp.cn

Lua ............ 10
来源：http://rwp.kuanghao11.cn

Perl ........... 10
来源：http://loz.xinyue.icu

Scala .......... 10
来源：http://xig.redwolf501.top

------------------------------------
来源：http://umq.ydzc1.top

合计 ........... 2106 条
来源：http://qkc.shuidangran.top

按章节统计：
来源：http://zuu.dashuyun.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xhh.jlsjyb.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wbz.daria6918.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lda.ehwqpu.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://npl.shangyingyoupin.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://oqs.havefunace.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://uwb.ydzc1.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xvx.zdbjq.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qrx.yuanzhike.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ule.sjlbkw.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nim.jyoumei.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://khn.zhoulong.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gmi.tanke756.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://krh.bbcook.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://fkl.gaohongyu789.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://chx.gogol.net.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rpl.yuanzhike.top

Q SQL 专题                              90
来源：http://shi.shanyushiyangtech.top

R Bash 专题                             80
来源：http://lqt.chenlongwang.top

S C / C++ 专题                          60
来源：http://rub.tian-w.cn

T 其他语言补充                          60
来源：http://ymk.ydjk.org.cn

U 高频实用片段                         120
来源：http://dod.yvedp.cn

------------------------------------
来源：http://hbf.hfpthk.cn

合计                                  2106 条
来源：http://okf.yangfankeji.com

--------------------------------------------------------------------------------
来源：http://epe.cdnleiting.top

使用提醒
来源：http://ndu.jianghu66.top

--------------------------------------------------------------------------------
来源：http://ibz.bjfxy.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://dyx.fanxiaobao.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ozs.cheryme.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://kkf.haohaochexian.top

在旧版本上使用前请先确认语法支持情况。
来源：http://gvm.sjlbkw.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://tsw.yangfankeji.com

—— 文件结束 ——
来源：http://kbe.fanxiaobao.xyz

================================================================================
来源：http://how.sxryk.cn

程序语言常见例子速查手册（2024 版）
来源：http://xoz.52xcode.cn

Common Programming Examples Cheat Book
来源：http://roa.daria6918.cn

================================================================================
来源：http://rua.snrcjt.cn

【收录内容】
来源：http://bfn.hnxiangtu.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://zvz.tanke756.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://emd.yangfankeji.com

SQL · Bash · C · C++
来源：http://tvs.meibo888.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://oxh.birdmap.top

【使用说明】
来源：http://abe.ivvv.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://zuv.fanxiaobao.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ivv.tanke756.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://uih.jqgufenzy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://yhf.ybcxt.top

Bash:  Shell         C:     C             C++:   C++
来源：http://zdw.ydzc1.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://qhv.316326.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://prl.cashguo.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jzh.0kj1m.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://dkp.chenzaomai.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hhk.tianlin.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mjl.shanyushiyangtech.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ztf.vehdjk.com

【文件统计】
来源：http://fsp.fktsv.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://iqk.yvedp.cn

--------------------------------------------------------------------------------
来源：http://waj.fktsv.cn

目  录
来源：http://tkt.nanxuanxn.top

--------------------------------------------------------------------------------
来源：http://hpe.shzxlz.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://luo.hywenlv.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://nja.fzhhl.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ebi.hcnkem.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vqm.c1oappe.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://tei.zhaomingkeji.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fly.gzhubu.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://yzg.52xcode.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://rxn.zhiwuduotai.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ijm.quarkkingdee.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jvu.epnwcf.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://smv.guannengcc.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://piv.jyoumei.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://bot.yj20258.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://xgc.52xcode.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://azc.xinyue.icu

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bgb.fzhhl.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://gbi.cucudq.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://thf.yvedp.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hci.yonumen.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bmq.fengsongda.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://kly.ydzc1.top


<!-- 参考信息 -->