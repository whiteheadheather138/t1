代发 wailian999

[U23] Py：分块读取大文件
来源：http://coy.feifeiyinyue.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hid.redwolf501.top

[U24] Py：路径操作
来源：http://urt.dashuyun.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lbi.zhijiandao.cn

[U25] Py：CSV 按字典读
来源：http://pys.ppjwa.cn

csv.DictReader(f)
来源：http://jge.haohaochexian.top

[U26] Py：并发下载
来源：http://uww.ydzc1.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://cik.aizwys.cn

[U27] Py：异步 HTTP
来源：http://csy.xuetiantiany.cn

aiohttp.ClientSession() 配合 async with
来源：http://llc.bjfxy.top

[U28] Py：类型别名
来源：http://gyz.ywan-chungtsiang.top

UserId = int
来源：http://iee.nwbrower.top

[U29] Py：属性校验
来源：http://gua.zhixingplan.top

@property 与 @x.setter 配合
来源：http://twj.tanke756.top

[U30] Py：数据类
来源：http://yww.ydzc1.top

@dataclass(slots=True)
来源：http://zrj.jlsjyb.cn

[U31] Py：单测
来源：http://zrv.9152youxi.cn

python -m pytest -q
来源：http://egf.shanyushiyangkeji.top

[U32] Py：代码格式化
来源：http://aok.yueranfly.top

ruff format . && ruff check --fix .
来源：http://jba.yj20258888.top

[U33] Py：打包发布
来源：http://sfj.uphjek.com

python -m build  （依赖 pyproject.toml）
来源：http://mkt.gzhubu.top

[U34] Py：判断编码
来源：http://rpr.tarul.cn

chardet.detect(raw)
来源：http://mfn.nanxinkj.top

[U35] Py：发送邮件
来源：http://rnp.yuanzhike.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://prg.shzxlz.cn

[U36] Py：定时任务
来源：http://pqi.ctjpmb.com

schedule.every(10).minutes.do(job)
来源：http://lpa.aibaodan.cn

[U37] Py：读写 Excel
来源：http://lou.fehbvm.com

pandas.read_excel / DataFrame.to_excel
来源：http://djv.mhx1999.top

[U38] Py：获取脚本所在目录
来源：http://fed.yangfankeji.com

Path(__file__).resolve().parent
来源：http://nkv.xinyue.icu

[U39] Py：判断是否在交互环境
来源：http://ood.aibaodan.cn

sys.stdout.isatty()
来源：http://iia.ywan-chungtsiang.top

[U40] Py：打印到标准错误
来源：http://zro.shangyingyoupin.top

print("err", file=sys.stderr)
来源：http://ppg.pycfn.com

[U41] PHP：初始化 Composer 项目
来源：http://wgk.hesvh.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://dbb.hywenlv.cn

[U42] PHP：PSR-4 自动加载
来源：http://crh.wangdashe.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xjn.gogol.net.cn

[U43] PHP：声明命名空间
来源：http://vtk.chenzaomai.com

namespace App\Http;
来源：http://vwd.mhx1999.top

[U44] PHP：开启严格类型
来源：http://eng.zhixingplan.top

declare(strict_types=1);
来源：http://lpt.chenjidiqi.icu

[U45] PHP：类型声明与返回类型
来源：http://won.bbcook.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://wny.wangdashe.top

[U46] PHP：可空类型
来源：http://ohi.ydzc1.top

?string $name = null
来源：http://gql.tarul.cn

[U47] PHP：联合类型
来源：http://nsh.ydzc1.top

int|string $id
来源：http://xap.ywan-chungtsiang.top

[U48] PHP：纯枚举
来源：http://ucq.ydjk.org.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://uen.cdnleiting.top

[U49] PHP：只读属性
来源：http://pze.yonumen.top

public readonly string $name
来源：http://vxm.pengpengdd.cyou

[U50] PHP：构造器属性提升
来源：http://atg.jinqigfzy.top

public function __construct(private int $id) {}
来源：http://cpx.ydjk.org.cn

[U51] PHP：数组解构
来源：http://kal.hcnkem.com

[$a, $b] = $arr;
来源：http://ewc.smart0.xyz

[U52] PHP：箭头函数
来源：http://gof.yj20258.top

$double = fn($x) => $x * 2;
来源：http://mjq.chenjidiqi.icu

[U53] PHP：空合并运算符
来源：http://xrz.jinyuanbaomall.cn

$v = $a ?? $b ?? "default";
来源：http://nxw.daxiang520.top

[U54] PHP：空安全调用
来源：http://myd.jinghuilouyu.cn

$obj?->method()
来源：http://qph.9152youxi.cn

[U55] PHP：match 表达式
来源：http://zbx.jianghu66.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hcl.gaohongyu789.top

[U56] PHP：命名参数
来源：http://pjr.pycfn.com

f(a: 1, b: 2)
来源：http://obh.yangfankeji.com

[U57] PHP：字符串插值
来源：http://tlv.dianchejie.cn

"值: {$a}"
来源：http://kxp.aizwys.cn

[U58] PHP：数组三件套
来源：http://lgd.hnqzz.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://iou.jqgfzy.top

[U59] PHP：自定义排序
来源：http://jwk.hywenlv.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cue.tian-w.cn

[U60] PHP：JSON 编解码
来源：http://nde.gogol.net.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xjy.c1oappe.top

[U61] PHP：正则
来源：http://wki.vehdjk.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ywd.haohaochexian.top

[U62] PHP：日期对象
来源：http://iai.xziqi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mol.hnxiangtu.top

[U63] PHP：文件读写
来源：http://vjw.fktsv.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pvz.chenjidiqi.icu

[U64] PHP：目录遍历
来源：http://zfz.hesvh.cn

glob("dir/*.php");  scandir("dir");
来源：http://wcs.jinyuanbaomall.cn

[U65] PHP：会话
来源：http://jkg.quarkkingdee.top

session_start();  $_SESSION["uid"] = 1;
来源：http://cdw.ywan-chungtsiang.top

[U66] PHP：设置 Cookie
来源：http://uqz.bjfxy.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://csd.nwbrower.top

[U67] PHP：处理文件上传
来源：http://tqb.jlsjyb.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gun.havefunace.top

[U68] PHP：PDO 连接
来源：http://fog.gotoacloud.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lwy.xylfe.cn

[U69] PHP：PDO 预处理
来源：http://zrm.bbcook.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://afx.cdnleiting.top

[U70] PHP：PDO 事务
来源：http://zxp.cashguo.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wim.hesvh.cn

[U71] PHP：抛出异常
来源：http://ouh.fktsv.cn

throw new RuntimeException("失败", 500);
来源：http://gqt.jinyuanbaomall.cn

[U72] PHP：写错误日志
来源：http://nwm.guannengcc.top

error_log("失败: " . $e->getMessage());
来源：http://zdp.gzhubu.top

[U73] PHP：读取 ini 配置
来源：http://ycl.shzxlz.cn

parse_ini_file("config.ini", true)
来源：http://knl.xuanzx.com

[U74] PHP：读取环境变量
来源：http://yqv.fehbvm.com

getenv("APP_ENV") ?: "production"
来源：http://rbh.jyoumei.cn

[U75] PHP：依赖注入
来源：http://nkq.cucudq.cn

composer require psr/container
来源：http://cqm.xuetiantiany.cn

[U76] PHP：简单路由
来源：http://znd.havefunace.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://oeb.chenjidiqi.icu

[U77] PHP：模板渲染
来源：http://aul.dashuyun.cn

composer require twig/twig
来源：http://hfv.vehdjk.com

[U78] PHP：单元测试
来源：http://epq.bjfxy.top

composer require --dev phpunit/phpunit
来源：http://jpi.aizwys.cn

[U79] PHP：静态分析
来源：http://qdw.smart0.xyz

composer require --dev phpstan/phpstan
来源：http://zdk.jinyuanbaomall.cn

[U80] PHP：代码规范修复
来源：http://tvc.daria6918.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://uis.ctjpmb.com

[U81] JS：初始化项目
来源：http://req.pengpengdd.cyou

npm init -y;  npm i express
来源：http://gio.yuanzhike.top

[U82] JS：package.json 脚本
来源：http://mxi.bbcook.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://oee.xziqi.cn

[U83] JS：ES Module 导入导出
来源：http://pyn.ppjwa.cn

export const a = 1;  import { a } from "./m.js";
来源：http://lwy.gotoacloud.top

[U84] JS：CommonJS 写法
来源：http://tkx.zhaomingkeji.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://eed.tianlin.xyz

[U85] JS：可选链
来源：http://byq.kuanghao11.cn

a?.b?.c
来源：http://nkd.c1oappe.top

[U86] JS：空值合并
来源：http://rbd.bbcook.cn

a ?? b
来源：http://xpd.gogol.net.cn

[U87] JS：解构默认值
来源：http://xgf.gzhubu.top

const { a = 1, b = 2 } = obj;
来源：http://nkk.zycfv.cn

[U88] JS：对象展开合并
来源：http://fnb.cucudq.cn

{ ...a, ...b }
来源：http://nhq.gotoacloud.top

[U89] JS：数组去重
来源：http://vqu.wangshuangyany.cn

[...new Set(arr)]
来源：http://iqy.smart0.xyz

[U90] JS：数字数组排序
来源：http://dnv.zhijiandao.cn

[...arr].sort((a, b) => a - b)
来源：http://una.xziqi.cn

[U91] JS：对象键值遍历
来源：http://ngn.daria6918.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wlx.dashuyun.cn

[U92] JS：深拷贝
来源：http://diu.hnqzz.top

structuredClone(obj)
来源：http://qop.hnxiangtu.top

[U93] JS：模板字符串
来源：http://tpp.yvedp.cn

`共 ${n} 条`
来源：http://nbz.9152youxi.cn

[U94] JS：箭头函数
来源：http://wgz.jinqigufen.top

const double = x => x * 2;
来源：http://rwn.quarkkingdee.top

[U95] JS：Promise 包装
来源：http://qhr.jiagoushi.top

new Promise((resolve, reject) => {})
来源：http://azh.sweek.top

[U96] JS：async/await 与异常
来源：http://jmh.dashuyun.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lvg.zhongyouzk.top

[U97] JS：并发请求
来源：http://ttm.xuanzx.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://mbe.bbcook.cn

[U98] JS：fetch 带 JSON
来源：http://mgp.bbcook.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://lxh.zycfv.cn

[U99] JS：事件监听
来源：http://fmg.nwbrower.top

el.addEventListener("click", e => {})
来源：http://awa.chenjidiqi.icu

[U100] JS：DOM 查询
来源：http://dps.hywenlv.cn

document.querySelector(".item")
来源：http://emp.uphjek.com

[U101] JS：classList 操作
来源：http://vkz.shangyingyoupin.top

el.classList.toggle("active")
来源：http://vmu.ivvv.top

[U102] JS：本地存储
来源：http://kov.sufxvd.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://rms.cashguo.top

[U103] JS：定时器
来源：http://emv.bjfxy.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mac.wangdashe.top

[U104] JS：防抖
来源：http://oxl.wangshuangyany.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wpu.daxiang520.top

[U105] JS：节流
来源：http://enr.yangfankeji.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://eow.fktsv.cn

[U106] JS：日期格式化
来源：http://yyo.fktsv.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jjw.sufxvd.cn

[U107] JS：数字千分位
来源：http://skz.0kj1m.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pfx.bbcook.cn

[U108] JS：随机整数
来源：http://tzl.yfazqb.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://buf.dianchejie.cn

[U109] JS：数组分组
来源：http://yar.hnqzz.top

Object.groupBy(arr, x => x.type)
来源：http://lus.zhaomingkeji.xyz

[U110] JS：数组分块
来源：http://ofv.shzxlz.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fxr.sjlbkw.cn

[U111] JS：对象转 Map
来源：http://nnn.xingfuxueyuan.xyz

new Map(Object.entries(obj))
来源：http://jab.guowangkeji.top

[U112] JS：字符串补位
来源：http://cbu.nwbrower.top

"7".padStart(3, "0")
来源：http://ztv.vehdjk.com

[U113] JS：正则替换全部
来源：http://aoe.sjlbkw.cn

s.replaceAll("a", "b")
来源：http://qfo.birdmap.top

[U114] JS：JSON 深比较
来源：http://ysu.hesvh.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://zdg.cdnleiting.top

[U115] JS：生成 UUID
来源：http://sbu.nanxuanxn.top

crypto.randomUUID()
来源：http://zzh.wangdashe.top

[U116] JS：类型检查（JSDoc）
来源：http://tei.daxiang520.top

/** @param {string} name */ function f(name) {}
来源：http://sku.pycfn.com

[U117] JS：单元测试
来源：http://zec.sweek.top

npm i -D vitest;  npx vitest
来源：http://rwm.xziqi.cn

[U118] JS：开发服务器
来源：http://xpl.tanke756.top

npm i -D vite;  npx vite
来源：http://mya.feifeiyinyue.top

[U119] JS：生产构建
来源：http://won.fzhhl.top

npx vite build
来源：http://tmj.mhx1999.top

[U120] JS：读取环境变量（Vite）
来源：http://xno.gogol.net.cn

import.meta.env.VITE_API_URL
来源：http://jwj.chenlongwang.top

================================================================================
来源：http://mcw.0kj1m.cn

统计汇总
来源：http://kme.zycfv.cn

================================================================================
来源：http://slh.sysykeji.top

按语言统计（条）：
来源：http://vae.yanxiufei.cn

Python ......... 252
来源：http://uhc.haohaochexian.top

PHP ............ 252
来源：http://ouy.bbcook.cn

JavaScript ..... 252
来源：http://ews.hfpthk.cn

TypeScript ..... 212
来源：http://vil.gzhubu.top

Java ........... 212
来源：http://vst.zhengqikj.top

Go ............. 212
来源：http://xzc.yj202588.top

Ruby ........... 212
来源：http://fnd.chenjidiqi.icu

C# ............. 212
来源：http://clj.gzhubu.top

C .............. 30
来源：http://liz.cdnleiting.top

C++ ............ 30
来源：http://zda.yfazqb.com

SQL ............ 90
来源：http://bsy.yj202588.top

Bash ........... 80
来源：http://puz.zhijiandao.cn

Kotlin ......... 15
来源：http://asr.zhoulong.xyz

Swift .......... 15
来源：http://tkd.jyoumei.cn

Lua ............ 10
来源：http://qyt.jinghuilouyu.cn

Perl ........... 10
来源：http://vgg.tarul.cn

Scala .......... 10
来源：http://fxy.cqqwz.cn

------------------------------------
来源：http://hgj.andypj.xyz

合计 ........... 2106 条
来源：http://hdh.nanxuanxn.top

按章节统计：
来源：http://ftq.snrcjt.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ymm.haohaochexian.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jji.fengsongda.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://bus.jinqigufen.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://iux.uphjek.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://eml.birdmap.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bzb.xingfuxueyuan.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://sdh.sxryk.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gut.chenlongwang.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://kyp.jinyuanbaomall.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fmj.jyoumei.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hsg.chenzaomai.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nkn.hywenlv.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://xbv.shanyushiyangkeji.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://xhi.bbcook.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://tqw.wangshuangyany.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xke.0kj1m.cn

Q SQL 专题                              90
来源：http://tng.sjlbkw.cn

R Bash 专题                             80
来源：http://bjd.shangyingyoupin.top

S C / C++ 专题                          60
来源：http://xmh.daria6918.cn

T 其他语言补充                          60
来源：http://jja.dashuyun.cn

U 高频实用片段                         120
来源：http://spr.sysykeji.top

------------------------------------
来源：http://ged.hysaishi.cn

合计                                  2106 条
来源：http://mok.0kj1m.cn

--------------------------------------------------------------------------------
来源：http://pso.cucudq.cn

使用提醒
来源：http://jqm.sxryk.cn

--------------------------------------------------------------------------------
来源：http://wov.uphjek.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jyo.fzhhl.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://dzl.jlsjyb.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ywt.zhongyouzk.top

在旧版本上使用前请先确认语法支持情况。
来源：http://eeo.gzhubu.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://yau.shanyushiyangkeji.top

—— 文件结束 ——
来源：http://gen.yueranfly.top

================================================================================
来源：http://mgh.ivvv.top

程序语言常见例子速查手册（2024 版）
来源：http://eaj.meibo888.top

Common Programming Examples Cheat Book
来源：http://med.svipenyu.cn

================================================================================
来源：http://aio.0kj1m.cn

【收录内容】
来源：http://sag.hnqzz.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://vth.yanxiufei.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://upj.wangshuangyany.cn

SQL · Bash · C · C++
来源：http://uun.vehdjk.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ylm.birdmap.top

【使用说明】
来源：http://uqb.yongpay.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://sao.wangshuangyany.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://fru.nwbrower.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wna.svipenyu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qal.yfazqb.com

Bash:  Shell         C:     C             C++:   C++
来源：http://tig.yj202588.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ptv.hcnkem.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qzg.shanyushiyangtech.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vhv.chenzaomai.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hzz.c1oappe.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xvf.fanxiaobao.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qzw.hammf.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://nlt.xziqi.cn

【文件统计】
来源：http://jom.fehbvm.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://izs.chenlongwang.top

--------------------------------------------------------------------------------
来源：http://lvy.guowangkeji.top

目  录
来源：http://xix.chenzaomai.com

--------------------------------------------------------------------------------
来源：http://xqe.bbcook.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://vli.dashuyun.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://vvg.dianchejie.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hwj.yonumen.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://fwk.zhongyouzk.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ojp.dashuyun.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qme.yueranfly.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://rkm.xingfuxueyuan.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://gie.cdnleiting.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lqk.havefunace.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hla.guowangkeji.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://dcq.dianchejie.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zap.shanyushiyangtech.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://zlc.zhoulong.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://bjp.yanxiufei.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://oec.daxiang520.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://xot.hysaishi.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xch.guannengcc.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://qvh.pengpengdd.cyou

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wrq.yanxiufei.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ete.redwolf501.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://caz.yj202588.top


<!-- 参考信息 -->