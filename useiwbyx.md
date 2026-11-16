代发 wailian999

[U23] Py：分块读取大文件
来源：http://dto.ctjpmb.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bop.zhijiandao.cn

[U24] Py：路径操作
来源：http://wdh.zhongyouzk.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://sgn.fzhhl.top

[U25] Py：CSV 按字典读
来源：http://xno.fktsv.cn

csv.DictReader(f)
来源：http://rna.hcnkem.com

[U26] Py：并发下载
来源：http://cvs.zhijiandao.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://akt.fanxiaobao.xyz

[U27] Py：异步 HTTP
来源：http://wel.guannengcc.top

aiohttp.ClientSession() 配合 async with
来源：http://bwq.gotoacloud.top

[U28] Py：类型别名
来源：http://sxw.yuanzhike.top

UserId = int
来源：http://ceg.yonumen.top

[U29] Py：属性校验
来源：http://erv.kuanghao11.cn

@property 与 @x.setter 配合
来源：http://ksg.yj20258.top

[U30] Py：数据类
来源：http://vgz.jianghu66.top

@dataclass(slots=True)
来源：http://rey.feifeiyinyue.top

[U31] Py：单测
来源：http://hrv.gzhubu.top

python -m pytest -q
来源：http://can.hammf.cn

[U32] Py：代码格式化
来源：http://soa.fzhhl.top

ruff format . && ruff check --fix .
来源：http://hxh.sweek.top

[U33] Py：打包发布
来源：http://niu.c1oappe.top

python -m build  （依赖 pyproject.toml）
来源：http://ysi.chenlongwang.top

[U34] Py：判断编码
来源：http://slp.xylfe.cn

chardet.detect(raw)
来源：http://xke.guowangkeji.top

[U35] Py：发送邮件
来源：http://koc.ybcxt.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qnp.zhaomingkeji.xyz

[U36] Py：定时任务
来源：http://jiw.xingfuxueyuan.xyz

schedule.every(10).minutes.do(job)
来源：http://ypy.aizwys.cn

[U37] Py：读写 Excel
来源：http://yot.hammf.cn

pandas.read_excel / DataFrame.to_excel
来源：http://tcm.bjfxy.top

[U38] Py：获取脚本所在目录
来源：http://jct.xziqi.cn

Path(__file__).resolve().parent
来源：http://osa.jiagoushi.top

[U39] Py：判断是否在交互环境
来源：http://nhn.ydjk.org.cn

sys.stdout.isatty()
来源：http://aui.mhx1999.top

[U40] Py：打印到标准错误
来源：http://cko.birdmap.top

print("err", file=sys.stderr)
来源：http://mxp.andypj.xyz

[U41] PHP：初始化 Composer 项目
来源：http://zxs.hesvh.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://gpo.zhixingplan.top

[U42] PHP：PSR-4 自动加载
来源：http://jdx.birdmap.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lyb.guannengcc.top

[U43] PHP：声明命名空间
来源：http://gyw.hnxiangtu.top

namespace App\Http;
来源：http://poa.shzxlz.cn

[U44] PHP：开启严格类型
来源：http://qsx.yuxming.cn

declare(strict_types=1);
来源：http://wgr.iojbl.cn

[U45] PHP：类型声明与返回类型
来源：http://zzj.fzhhl.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://bpa.gotoacloud.top

[U46] PHP：可空类型
来源：http://apw.epnwcf.com

?string $name = null
来源：http://wkc.xuetiantiany.cn

[U47] PHP：联合类型
来源：http://nws.ydzc1.top

int|string $id
来源：http://qyd.shuidangran.top

[U48] PHP：纯枚举
来源：http://ikb.yj202588.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://msk.iojbl.cn

[U49] PHP：只读属性
来源：http://clk.aizwys.cn

public readonly string $name
来源：http://abo.xuanzx.com

[U50] PHP：构造器属性提升
来源：http://lry.wangshuangyany.cn

public function __construct(private int $id) {}
来源：http://zkg.cucudq.cn

[U51] PHP：数组解构
来源：http://uai.yfazqb.com

[$a, $b] = $arr;
来源：http://yjn.zhiwuduotai.top

[U52] PHP：箭头函数
来源：http://yzl.iojbl.cn

$double = fn($x) => $x * 2;
来源：http://snc.sweek.top

[U53] PHP：空合并运算符
来源：http://ofv.9152youxi.cn

$v = $a ?? $b ?? "default";
来源：http://qpw.sufxvd.cn

[U54] PHP：空安全调用
来源：http://fac.zycfv.cn

$obj?->method()
来源：http://yzk.fengsongda.top

[U55] PHP：match 表达式
来源：http://yuy.quarkkingdee.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dla.quarkkingdee.top

[U56] PHP：命名参数
来源：http://ixb.hysaishi.cn

f(a: 1, b: 2)
来源：http://xis.jiagoushi.top

[U57] PHP：字符串插值
来源：http://kfa.kuanghao11.cn

"值: {$a}"
来源：http://ize.aibaodan.cn

[U58] PHP：数组三件套
来源：http://sry.cashguo.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fyd.yuxming.cn

[U59] PHP：自定义排序
来源：http://vpj.hywenlv.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vda.gaohongyu789.top

[U60] PHP：JSON 编解码
来源：http://npe.andypj.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://spk.haohaochexian.top

[U61] PHP：正则
来源：http://vux.hammf.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bjp.birdmap.top

[U62] PHP：日期对象
来源：http://wdf.gotoacloud.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xjw.zhaomingkeji.xyz

[U63] PHP：文件读写
来源：http://ihk.ydzc1.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xun.zhaomingkeji.xyz

[U64] PHP：目录遍历
来源：http://rfk.hesvh.cn

glob("dir/*.php");  scandir("dir");
来源：http://ati.tarul.cn

[U65] PHP：会话
来源：http://ygj.9152youxi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://trq.tian-w.cn

[U66] PHP：设置 Cookie
来源：http://ltz.chenzaomai.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://urh.zhiwuduotai.top

[U67] PHP：处理文件上传
来源：http://lod.nanxinkj.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://anh.gaohongyu789.top

[U68] PHP：PDO 连接
来源：http://hmg.pycfn.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://dam.hongshengwenyu.top

[U69] PHP：PDO 预处理
来源：http://zdt.jqgufenzy.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mrs.wangdashe.top

[U70] PHP：PDO 事务
来源：http://lxm.jiagoushi.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kvz.fehbvm.com

[U71] PHP：抛出异常
来源：http://ohh.ivvv.top

throw new RuntimeException("失败", 500);
来源：http://rkz.aibaodan.cn

[U72] PHP：写错误日志
来源：http://qxb.cdnleiting.top

error_log("失败: " . $e->getMessage());
来源：http://yew.vehdjk.com

[U73] PHP：读取 ini 配置
来源：http://oiv.hnxiangtu.top

parse_ini_file("config.ini", true)
来源：http://dzk.yj20258.top

[U74] PHP：读取环境变量
来源：http://rit.wangdashe.top

getenv("APP_ENV") ?: "production"
来源：http://ggy.cheryme.top

[U75] PHP：依赖注入
来源：http://jku.vehdjk.com

composer require psr/container
来源：http://xog.pengpengdd.cyou

[U76] PHP：简单路由
来源：http://msu.shanyushiyangtech.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://nag.guannengcc.top

[U77] PHP：模板渲染
来源：http://azn.andypj.xyz

composer require twig/twig
来源：http://ueu.chenjidiqi.icu

[U78] PHP：单元测试
来源：http://eee.zdbjq.cn

composer require --dev phpunit/phpunit
来源：http://pjl.zhoulong.xyz

[U79] PHP：静态分析
来源：http://wis.cheryme.top

composer require --dev phpstan/phpstan
来源：http://xoi.sweek.top

[U80] PHP：代码规范修复
来源：http://kgz.ydzc1.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://gul.vehdjk.com

[U81] JS：初始化项目
来源：http://nnj.yj20258.top

npm init -y;  npm i express
来源：http://qtv.yanxiufei.cn

[U82] JS：package.json 脚本
来源：http://ufr.yj20258888.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lbm.hcnkem.com

[U83] JS：ES Module 导入导出
来源：http://nid.guowangkeji.top

export const a = 1;  import { a } from "./m.js";
来源：http://kbo.chenlongwang.top

[U84] JS：CommonJS 写法
来源：http://mfm.xuetiantiany.cn

module.exports = { a };  const { a } = require("./m");
来源：http://rry.kuanghao11.cn

[U85] JS：可选链
来源：http://kcy.zhaomingkeji.xyz

a?.b?.c
来源：http://vuh.9152youxi.cn

[U86] JS：空值合并
来源：http://xzd.ivvv.top

a ?? b
来源：http://zet.zdbjq.cn

[U87] JS：解构默认值
来源：http://gdz.pengpengdd.cyou

const { a = 1, b = 2 } = obj;
来源：http://phs.svipenyu.cn

[U88] JS：对象展开合并
来源：http://uhp.smart0.xyz

{ ...a, ...b }
来源：http://apy.yonumen.top

[U89] JS：数组去重
来源：http://mqd.quarkkingdee.top

[...new Set(arr)]
来源：http://lxc.0kj1m.cn

[U90] JS：数字数组排序
来源：http://wns.hnxiangtu.top

[...arr].sort((a, b) => a - b)
来源：http://yfw.nwbrower.top

[U91] JS：对象键值遍历
来源：http://yyn.ydjk.org.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mrz.chenzaomai.com

[U92] JS：深拷贝
来源：http://lsp.52xcode.cn

structuredClone(obj)
来源：http://kwt.guowangkeji.top

[U93] JS：模板字符串
来源：http://vse.yvedp.cn

`共 ${n} 条`
来源：http://xmv.ydjk.org.cn

[U94] JS：箭头函数
来源：http://pax.cheryme.top

const double = x => x * 2;
来源：http://uzt.iojbl.cn

[U95] JS：Promise 包装
来源：http://lmq.yj20258888.top

new Promise((resolve, reject) => {})
来源：http://rqj.meibo888.top

[U96] JS：async/await 与异常
来源：http://jbp.52xcode.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fvs.jyoumei.cn

[U97] JS：并发请求
来源：http://sxk.316326.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://ixf.nanxuanxn.top

[U98] JS：fetch 带 JSON
来源：http://qem.xingfuxueyuan.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ttc.cucudq.cn

[U99] JS：事件监听
来源：http://myt.hesvh.cn

el.addEventListener("click", e => {})
来源：http://zyc.316326.xyz

[U100] JS：DOM 查询
来源：http://xcm.yuanzhike.top

document.querySelector(".item")
来源：http://xwm.mhx1999.top

[U101] JS：classList 操作
来源：http://sfl.ybcxt.top

el.classList.toggle("active")
来源：http://tas.chenzaomai.com

[U102] JS：本地存储
来源：http://ncs.cashguo.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://zvr.zdbjq.cn

[U103] JS：定时器
来源：http://jlk.yj20258888.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://dcb.hammf.cn

[U104] JS：防抖
来源：http://ubo.smart0.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jen.yj20258.top

[U105] JS：节流
来源：http://uve.jyoumei.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gtr.hammf.cn

[U106] JS：日期格式化
来源：http://ngy.cdnleiting.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://owd.ydjk.org.cn

[U107] JS：数字千分位
来源：http://olh.ehwqpu.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://dcv.fktsv.cn

[U108] JS：随机整数
来源：http://bmt.xuetiantiany.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://lyz.xylfe.cn

[U109] JS：数组分组
来源：http://pwf.hongshengwenyu.top

Object.groupBy(arr, x => x.type)
来源：http://suu.xinyue.icu

[U110] JS：数组分块
来源：http://kpk.chenlongwang.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://eml.shanyushiyangkeji.top

[U111] JS：对象转 Map
来源：http://pyw.9152youxi.cn

new Map(Object.entries(obj))
来源：http://mlt.shangyingyoupin.top

[U112] JS：字符串补位
来源：http://mdm.hcnkem.com

"7".padStart(3, "0")
来源：http://zwq.jlsjyb.cn

[U113] JS：正则替换全部
来源：http://lcb.bbcook.cn

s.replaceAll("a", "b")
来源：http://tbk.jyoumei.cn

[U114] JS：JSON 深比较
来源：http://ibs.sysykeji.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://kfq.wangshuangyany.cn

[U115] JS：生成 UUID
来源：http://idt.yj202588.top

crypto.randomUUID()
来源：http://gev.hfpthk.cn

[U116] JS：类型检查（JSDoc）
来源：http://ohn.yonumen.top

/** @param {string} name */ function f(name) {}
来源：http://bjf.pengpengdd.cyou

[U117] JS：单元测试
来源：http://ntk.aibaodan.cn

npm i -D vitest;  npx vitest
来源：http://cay.shuidangran.top

[U118] JS：开发服务器
来源：http://sld.cdnleiting.top

npm i -D vite;  npx vite
来源：http://tow.aizwys.cn

[U119] JS：生产构建
来源：http://jwk.jinqigufen.top

npx vite build
来源：http://ajr.iojbl.cn

[U120] JS：读取环境变量（Vite）
来源：http://glg.xuetiantiany.cn

import.meta.env.VITE_API_URL
来源：http://zsq.ivvv.top

================================================================================
来源：http://ojy.yongpay.top

统计汇总
来源：http://gmg.zycfv.cn

================================================================================
来源：http://vaj.cheryme.top

按语言统计（条）：
来源：http://ivk.gogol.net.cn

Python ......... 252
来源：http://vsx.hnqzz.top

PHP ............ 252
来源：http://gzw.bbcook.cn

JavaScript ..... 252
来源：http://rej.hysaishi.cn

TypeScript ..... 212
来源：http://soy.xziqi.cn

Java ........... 212
来源：http://meo.shanyushiyangkeji.top

Go ............. 212
来源：http://yng.bbcook.cn

Ruby ........... 212
来源：http://wdk.aibaodan.cn

C# ............. 212
来源：http://ycg.zycfv.cn

C .............. 30
来源：http://wvk.xuanzx.com

C++ ............ 30
来源：http://mwp.sweek.top

SQL ............ 90
来源：http://kvp.haohaochexian.top

Bash ........... 80
来源：http://qaw.tarul.cn

Kotlin ......... 15
来源：http://khz.jqgufenzy.top

Swift .......... 15
来源：http://rgm.gotoacloud.top

Lua ............ 10
来源：http://bmy.hfpthk.cn

Perl ........... 10
来源：http://ayt.nanxuanxn.top

Scala .......... 10
来源：http://uqb.fanxiaobao.xyz

------------------------------------
来源：http://hff.daria6918.cn

合计 ........... 2106 条
来源：http://duu.zdqjudy.top

按章节统计：
来源：http://azj.ybcxt.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mwt.cheryme.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qhh.meibo888.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wlz.cashguo.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://yqz.zhixingplan.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vnz.ywan-chungtsiang.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://eyf.meibo888.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://sdr.hnqzz.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://fgr.hongshengwenyu.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rfq.kuanghao11.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ymt.hfpthk.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://unx.jinghuilouyu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mkl.vqdsnc.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://sss.jqgfzy.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qse.ydjk.org.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vqo.zycfv.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://glp.tianlin.xyz

Q SQL 专题                              90
来源：http://dbf.hysaishi.cn

R Bash 专题                             80
来源：http://lpk.iojbl.cn

S C / C++ 专题                          60
来源：http://nez.aizwys.cn

T 其他语言补充                          60
来源：http://yjx.gogol.net.cn

U 高频实用片段                         120
来源：http://ipt.yvedp.cn

------------------------------------
来源：http://yga.jinyuanbaomall.cn

合计                                  2106 条
来源：http://yom.sysykeji.top

--------------------------------------------------------------------------------
来源：http://xbx.xingfuxueyuan.xyz

使用提醒
来源：http://fgh.chenjidiqi.icu

--------------------------------------------------------------------------------
来源：http://jri.yanxiufei.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mmf.cdnleiting.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xtr.jiagoushi.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://yni.fengsongda.top

在旧版本上使用前请先确认语法支持情况。
来源：http://vbn.wangshuangyany.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://opf.yj20258.top

—— 文件结束 ——
来源：http://ifh.svipenyu.cn

================================================================================
来源：http://hrn.birdmap.top

程序语言常见例子速查手册（2024 版）
来源：http://jss.fzhhl.top

Common Programming Examples Cheat Book
来源：http://rwg.cdnleiting.top

================================================================================
来源：http://pkc.xingfuxueyuan.xyz

【收录内容】
来源：http://tem.zdbjq.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://fjz.havefunace.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://gkh.shuidangran.top

SQL · Bash · C · C++
来源：http://fgu.316326.xyz

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://guv.yongpay.top

【使用说明】
来源：http://doq.sufxvd.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://nng.dashuyun.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://aif.wangshuangyany.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://fkm.jqgufenzy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wsv.ybcxt.top

Bash:  Shell         C:     C             C++:   C++
来源：http://apc.jinqigufen.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://rqb.c1oappe.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://yln.iojbl.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://esp.yuxming.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://piu.52xcode.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://grr.quarkkingdee.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://esc.sysykeji.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://cjc.guannengcc.top

【文件统计】
来源：http://owz.tarul.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zdo.ydjk.org.cn

--------------------------------------------------------------------------------
来源：http://hcw.hnxiangtu.top

目  录
来源：http://oqw.ywan-chungtsiang.top

--------------------------------------------------------------------------------
来源：http://irq.chenlongwang.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hwu.chenlongwang.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zcw.jinqigfzy.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fmh.cdnleiting.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://bdd.sufxvd.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ljd.pycfn.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ksq.ctjpmb.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xyi.sufxvd.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hms.daxiang520.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tri.yuxming.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ygp.52xcode.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://qhs.shuidangran.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ygl.shangyingyoupin.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://smn.xinyue.icu

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://otd.ydjk.org.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://oxz.hywenlv.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://zpc.vqdsnc.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xdw.aibaodan.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://yvl.shuidangran.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://gez.xziqi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://aha.yongpay.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://jwa.wangshuangyany.cn


<!-- 参考信息 -->