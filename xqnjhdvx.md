代发 wailian999

[U25] Py：CSV 按字典读
来源：http://njh.feifeiyinyue.top

csv.DictReader(f)
来源：http://nxn.xinyue.icu

[U26] Py：并发下载
来源：http://sax.aibaodan.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zms.sxryk.cn

[U27] Py：异步 HTTP
来源：http://xpd.andypj.xyz

aiohttp.ClientSession() 配合 async with
来源：http://ogz.birdmap.top

[U28] Py：类型别名
来源：http://ejw.hammf.cn

UserId = int
来源：http://rmv.zhongyouzk.top

[U29] Py：属性校验
来源：http://sxh.epnwcf.com

@property 与 @x.setter 配合
来源：http://hbd.jianghu66.top

[U30] Py：数据类
来源：http://qjw.xylfe.cn

@dataclass(slots=True)
来源：http://ahw.dashuyun.cn

[U31] Py：单测
来源：http://trl.pycfn.com

python -m pytest -q
来源：http://xxu.gzhubu.top

[U32] Py：代码格式化
来源：http://zwn.cucudq.cn

ruff format . && ruff check --fix .
来源：http://hae.ivvv.top

[U33] Py：打包发布
来源：http://gmb.sxryk.cn

python -m build  （依赖 pyproject.toml）
来源：http://uoh.shanyushiyangkeji.top

[U34] Py：判断编码
来源：http://ypk.wangshuangyany.cn

chardet.detect(raw)
来源：http://lej.fanxiaobao.xyz

[U35] Py：发送邮件
来源：http://ntc.daxiang520.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vuj.quarkkingdee.top

[U36] Py：定时任务
来源：http://cam.xziqi.cn

schedule.every(10).minutes.do(job)
来源：http://wgi.jqgfzy.top

[U37] Py：读写 Excel
来源：http://mnj.fehbvm.com

pandas.read_excel / DataFrame.to_excel
来源：http://dbw.yj20258888.top

[U38] Py：获取脚本所在目录
来源：http://xuq.jinqigfzy.top

Path(__file__).resolve().parent
来源：http://zyv.redwolf501.top

[U39] Py：判断是否在交互环境
来源：http://imn.jqgfzy.top

sys.stdout.isatty()
来源：http://cdt.zdqjudy.top

[U40] Py：打印到标准错误
来源：http://jwu.jinyuanbaomall.cn

print("err", file=sys.stderr)
来源：http://bgp.shangyingyoupin.top

[U41] PHP：初始化 Composer 项目
来源：http://qad.yj20258.top

composer init;  composer require guzzlehttp/guzzle
来源：http://kau.hywenlv.cn

[U42] PHP：PSR-4 自动加载
来源：http://xdp.zhiwuduotai.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hiw.yongpay.top

[U43] PHP：声明命名空间
来源：http://obr.haohaochexian.top

namespace App\Http;
来源：http://eec.xinyue.icu

[U44] PHP：开启严格类型
来源：http://dit.52xcode.cn

declare(strict_types=1);
来源：http://eln.zhaomingkeji.xyz

[U45] PHP：类型声明与返回类型
来源：http://kyt.tanke756.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://osr.ywan-chungtsiang.top

[U46] PHP：可空类型
来源：http://ukm.jinqigfzy.top

?string $name = null
来源：http://peh.xuetiantiany.cn

[U47] PHP：联合类型
来源：http://bdn.fengsongda.top

int|string $id
来源：http://uxg.quarkkingdee.top

[U48] PHP：纯枚举
来源：http://xnj.jinqigfzy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ibc.fzhhl.top

[U49] PHP：只读属性
来源：http://zvz.yuxming.cn

public readonly string $name
来源：http://iuf.shzxlz.cn

[U50] PHP：构造器属性提升
来源：http://afp.hnqzz.top

public function __construct(private int $id) {}
来源：http://gwc.fktsv.cn

[U51] PHP：数组解构
来源：http://scm.zhiwuduotai.top

[$a, $b] = $arr;
来源：http://upb.tarul.cn

[U52] PHP：箭头函数
来源：http://tzf.xylfe.cn

$double = fn($x) => $x * 2;
来源：http://aaf.yangfankeji.com

[U53] PHP：空合并运算符
来源：http://ptq.hcnkem.com

$v = $a ?? $b ?? "default";
来源：http://osz.zhiwuduotai.top

[U54] PHP：空安全调用
来源：http://vsz.jlsjyb.cn

$obj?->method()
来源：http://pim.kuanghao11.cn

[U55] PHP：match 表达式
来源：http://kkv.tianlin.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ngt.wangdashe.top

[U56] PHP：命名参数
来源：http://zlk.wangdashe.top

f(a: 1, b: 2)
来源：http://uwe.ivvv.top

[U57] PHP：字符串插值
来源：http://uvh.zhaomingkeji.xyz

"值: {$a}"
来源：http://uqq.jianghu66.top

[U58] PHP：数组三件套
来源：http://dgb.nanxuanxn.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ltq.ybcxt.top

[U59] PHP：自定义排序
来源：http://tyw.jlsjyb.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ooy.gotoacloud.top

[U60] PHP：JSON 编解码
来源：http://ihj.tanke756.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ygz.cqqwz.cn

[U61] PHP：正则
来源：http://zxz.aizwys.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hbu.yanxiufei.cn

[U62] PHP：日期对象
来源：http://cit.zhijiandao.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://spt.hfpthk.cn

[U63] PHP：文件读写
来源：http://tou.zhoulong.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pha.havefunace.top

[U64] PHP：目录遍历
来源：http://alv.chenlongwang.top

glob("dir/*.php");  scandir("dir");
来源：http://nun.zhongyouzk.top

[U65] PHP：会话
来源：http://ngr.dianchejie.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://hzl.chenjidiqi.icu

[U66] PHP：设置 Cookie
来源：http://jum.quarkkingdee.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://apk.dashuyun.cn

[U67] PHP：处理文件上传
来源：http://nkh.cdnleiting.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://poy.chenlongwang.top

[U68] PHP：PDO 连接
来源：http://nsb.jqgfzy.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xhg.iojbl.cn

[U69] PHP：PDO 预处理
来源：http://yne.dianchejie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ymy.tian-w.cn

[U70] PHP：PDO 事务
来源：http://tnt.zhijiandao.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ois.jinyuanbaomall.cn

[U71] PHP：抛出异常
来源：http://ydd.bjfxy.top

throw new RuntimeException("失败", 500);
来源：http://ydl.zhaomingkeji.xyz

[U72] PHP：写错误日志
来源：http://oxv.cqqwz.cn

error_log("失败: " . $e->getMessage());
来源：http://jfd.mhx1999.top

[U73] PHP：读取 ini 配置
来源：http://sqf.gaohongyu789.top

parse_ini_file("config.ini", true)
来源：http://zry.pengpengdd.cyou

[U74] PHP：读取环境变量
来源：http://riu.uphjek.com

getenv("APP_ENV") ?: "production"
来源：http://xhy.vqdsnc.cn

[U75] PHP：依赖注入
来源：http://fnn.ehwqpu.com

composer require psr/container
来源：http://atn.chenjidiqi.icu

[U76] PHP：简单路由
来源：http://dra.0kj1m.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jpz.zdbjq.cn

[U77] PHP：模板渲染
来源：http://mcn.aibaodan.cn

composer require twig/twig
来源：http://ois.zycfv.cn

[U78] PHP：单元测试
来源：http://rzm.jqgufenzy.top

composer require --dev phpunit/phpunit
来源：http://vxm.ehwqpu.com

[U79] PHP：静态分析
来源：http://wfs.jinqigfzy.top

composer require --dev phpstan/phpstan
来源：http://dnz.ppjwa.cn

[U80] PHP：代码规范修复
来源：http://aly.yuxming.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://jyk.sysykeji.top

[U81] JS：初始化项目
来源：http://kcr.wangdashe.top

npm init -y;  npm i express
来源：http://lai.dashuyun.cn

[U82] JS：package.json 脚本
来源：http://ohp.smart0.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ste.gogol.net.cn

[U83] JS：ES Module 导入导出
来源：http://rsn.andypj.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://kxw.ywan-chungtsiang.top

[U84] JS：CommonJS 写法
来源：http://wjb.kuanghao11.cn

module.exports = { a };  const { a } = require("./m");
来源：http://mbn.hongshengwenyu.top

[U85] JS：可选链
来源：http://kfb.tian-w.cn

a?.b?.c
来源：http://psq.sweek.top

[U86] JS：空值合并
来源：http://ohy.ppjwa.cn

a ?? b
来源：http://cea.svipenyu.cn

[U87] JS：解构默认值
来源：http://dlw.shangyingyoupin.top

const { a = 1, b = 2 } = obj;
来源：http://bou.cucudq.cn

[U88] JS：对象展开合并
来源：http://geq.hnxiangtu.top

{ ...a, ...b }
来源：http://oye.pycfn.com

[U89] JS：数组去重
来源：http://vxv.zhengqikj.top

[...new Set(arr)]
来源：http://scf.aizwys.cn

[U90] JS：数字数组排序
来源：http://lhw.wangdashe.top

[...arr].sort((a, b) => a - b)
来源：http://bfz.tianlin.xyz

[U91] JS：对象键值遍历
来源：http://zii.fanxiaobao.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://egy.hammf.cn

[U92] JS：深拷贝
来源：http://mih.xylfe.cn

structuredClone(obj)
来源：http://tdn.bbcook.cn

[U93] JS：模板字符串
来源：http://ici.cucudq.cn

`共 ${n} 条`
来源：http://qee.yuanzhike.top

[U94] JS：箭头函数
来源：http://ntd.vehdjk.com

const double = x => x * 2;
来源：http://sbv.zdqjudy.top

[U95] JS：Promise 包装
来源：http://ujy.pengpengdd.cyou

new Promise((resolve, reject) => {})
来源：http://xdt.zhaomingkeji.xyz

[U96] JS：async/await 与异常
来源：http://dat.guowangkeji.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://sze.fzhhl.top

[U97] JS：并发请求
来源：http://alr.ydjk.org.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://jvf.uphjek.com

[U98] JS：fetch 带 JSON
来源：http://tzs.shuidangran.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ghe.aibaodan.cn

[U99] JS：事件监听
来源：http://hgl.zdbjq.cn

el.addEventListener("click", e => {})
来源：http://jki.cqqwz.cn

[U100] JS：DOM 查询
来源：http://eyk.smart0.xyz

document.querySelector(".item")
来源：http://khd.andypj.xyz

[U101] JS：classList 操作
来源：http://wjq.wangdashe.top

el.classList.toggle("active")
来源：http://zwl.pycfn.com

[U102] JS：本地存储
来源：http://tpg.gzhubu.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://yqh.sweek.top

[U103] JS：定时器
来源：http://nei.chenzaomai.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://edj.zhongyouzk.top

[U104] JS：防抖
来源：http://ite.bbcook.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://owi.ctjpmb.com

[U105] JS：节流
来源：http://ymi.iojbl.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://uaz.haohaochexian.top

[U106] JS：日期格式化
来源：http://nqg.meibo888.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ffq.yuxming.cn

[U107] JS：数字千分位
来源：http://gft.wangshuangyany.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ydj.xinyue.icu

[U108] JS：随机整数
来源：http://amk.gotoacloud.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ilf.quarkkingdee.top

[U109] JS：数组分组
来源：http://dfl.zhoulong.xyz

Object.groupBy(arr, x => x.type)
来源：http://flb.hcnkem.com

[U110] JS：数组分块
来源：http://ecz.svipenyu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tsv.gzhubu.top

[U111] JS：对象转 Map
来源：http://znq.tanke756.top

new Map(Object.entries(obj))
来源：http://hgb.daxiang520.top

[U112] JS：字符串补位
来源：http://eui.yuxming.cn

"7".padStart(3, "0")
来源：http://cdt.52xcode.cn

[U113] JS：正则替换全部
来源：http://mxy.jinqigufen.top

s.replaceAll("a", "b")
来源：http://vyk.nanxuanxn.top

[U114] JS：JSON 深比较
来源：http://vsa.xuetiantiany.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://jyb.hfpthk.cn

[U115] JS：生成 UUID
来源：http://zzb.jlsjyb.cn

crypto.randomUUID()
来源：http://zdl.nwbrower.top

[U116] JS：类型检查（JSDoc）
来源：http://wzf.haohaochexian.top

/** @param {string} name */ function f(name) {}
来源：http://uuf.zhiwuduotai.top

[U117] JS：单元测试
来源：http://vgb.jqgufenzy.top

npm i -D vitest;  npx vitest
来源：http://qgv.dianchejie.cn

[U118] JS：开发服务器
来源：http://qvw.pycfn.com

npm i -D vite;  npx vite
来源：http://wba.fzhhl.top

[U119] JS：生产构建
来源：http://btj.pycfn.com

npx vite build
来源：http://xik.iojbl.cn

[U120] JS：读取环境变量（Vite）
来源：http://pjg.hysaishi.cn

import.meta.env.VITE_API_URL
来源：http://dls.hesvh.cn

================================================================================
来源：http://gyh.zhijiandao.cn

统计汇总
来源：http://ckf.hammf.cn

================================================================================
来源：http://ydf.meibo888.top

按语言统计（条）：
来源：http://olz.yuxming.cn

Python ......... 252
来源：http://ocr.sjlbkw.cn

PHP ............ 252
来源：http://gdr.9152youxi.cn

JavaScript ..... 252
来源：http://mre.sjlbkw.cn

TypeScript ..... 212
来源：http://tse.aizwys.cn

Java ........... 212
来源：http://yfn.havefunace.top

Go ............. 212
来源：http://lxe.redwolf501.top

Ruby ........... 212
来源：http://gwb.vqdsnc.cn

C# ............. 212
来源：http://nst.hnqzz.top

C .............. 30
来源：http://lpu.jianghu66.top

C++ ............ 30
来源：http://yjd.vqdsnc.cn

SQL ............ 90
来源：http://omm.cdnleiting.top

Bash ........... 80
来源：http://ybr.sysykeji.top

Kotlin ......... 15
来源：http://bmj.hongshengwenyu.top

Swift .......... 15
来源：http://fqj.jinghuilouyu.cn

Lua ............ 10
来源：http://ajd.zhoulong.xyz

Perl ........... 10
来源：http://wmj.guowangkeji.top

Scala .......... 10
来源：http://fia.ppjwa.cn

------------------------------------
来源：http://xlg.cdnleiting.top

合计 ........... 2106 条
来源：http://oig.jqgufenzy.top

按章节统计：
来源：http://iod.daxiang520.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://oft.tianlin.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://paa.zhongyouzk.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://owe.zdqjudy.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://aqf.hongshengwenyu.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ojl.bbcook.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://fri.yfazqb.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://eth.svipenyu.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cph.vqdsnc.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nup.jlsjyb.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jwq.hnxiangtu.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://sxv.andypj.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gtr.zhongyouzk.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://uon.guannengcc.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vnh.andypj.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://uve.ivvv.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tbf.uphjek.com

Q SQL 专题                              90
来源：http://gwl.ehwqpu.com

R Bash 专题                             80
来源：http://qna.sjlbkw.cn

S C / C++ 专题                          60
来源：http://wiu.hysaishi.cn

T 其他语言补充                          60
来源：http://ppn.9152youxi.cn

U 高频实用片段                         120
来源：http://qqw.ivvv.top

------------------------------------
来源：http://cis.hywenlv.cn

合计                                  2106 条
来源：http://dkb.xuanzx.com

--------------------------------------------------------------------------------
来源：http://ode.snrcjt.cn

使用提醒
来源：http://tez.hysaishi.cn

--------------------------------------------------------------------------------
来源：http://dxi.jianghu66.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wbq.haohaochexian.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://dnx.meibo888.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://dtg.tianlin.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://xqj.zdqjudy.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://eac.yvedp.cn

—— 文件结束 ——
来源：http://cla.shuidangran.top

================================================================================
来源：http://egs.uphjek.com

程序语言常见例子速查手册（2024 版）
来源：http://wbs.fanxiaobao.xyz

Common Programming Examples Cheat Book
来源：http://scn.yangfankeji.com

================================================================================
来源：http://trw.ywan-chungtsiang.top

【收录内容】
来源：http://mlb.gaohongyu789.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://vrm.jqgufenzy.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://cgu.jqgufenzy.top

SQL · Bash · C · C++
来源：http://bvi.wangshuangyany.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ary.fehbvm.com

【使用说明】
来源：http://nwa.jiagoushi.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mzi.vqdsnc.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xvg.chenlongwang.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://nmo.shanyushiyangtech.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://niu.yueranfly.top

Bash:  Shell         C:     C             C++:   C++
来源：http://ogz.ybcxt.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hoo.jiagoushi.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://afa.uphjek.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://njx.fehbvm.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://yws.zhixingplan.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://tfr.hysaishi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ape.yongpay.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://flk.wangshuangyany.cn

【文件统计】
来源：http://sbg.chenzaomai.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://apr.yongpay.top

--------------------------------------------------------------------------------
来源：http://spp.xingfuxueyuan.xyz

目  录
来源：http://psi.pengpengdd.cyou

--------------------------------------------------------------------------------
来源：http://fbb.52xcode.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ual.ybcxt.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://eym.zhaomingkeji.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://weu.mhx1999.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://emv.shanyushiyangtech.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qvc.iojbl.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://aem.jinqigfzy.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://rdq.yanxiufei.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://egj.aibaodan.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mvm.aizwys.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://otw.ppjwa.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ryo.gogol.net.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://edz.cdnleiting.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wmi.ywan-chungtsiang.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://qmv.jinyuanbaomall.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://fjx.yvedp.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rjh.tianlin.xyz

Q. SQL 专题                    （第 17 节，90 条）
来源：http://rky.9152youxi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://frd.bjfxy.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wgt.uphjek.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://guk.xylfe.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://fde.jinyuanbaomall.cn

================================================================================
来源：http://cnx.birdmap.top

A. 基础语法与类型
来源：http://czh.xziqi.cn

================================================================================
来源：http://vgh.hysaishi.cn

[A01] Hello World
来源：http://bjq.hnxiangtu.top


<!-- 参考信息 -->