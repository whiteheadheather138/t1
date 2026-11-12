代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://umj.yfazqb.com

@contextlib.contextmanager
来源：http://jhb.gogol.net.cn

[U22] Py：矩阵转置
来源：http://cdy.cdnleiting.top

list(zip(*m))
来源：http://pzi.gzhubu.top

[U23] Py：分块读取大文件
来源：http://vin.yanxiufei.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://njh.jinqigfzy.top

[U24] Py：路径操作
来源：http://jhy.xingfuxueyuan.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://soq.cheryme.top

[U25] Py：CSV 按字典读
来源：http://sgt.sweek.top

csv.DictReader(f)
来源：http://hnb.cashguo.top

[U26] Py：并发下载
来源：http://eep.hongshengwenyu.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wra.sjlbkw.cn

[U27] Py：异步 HTTP
来源：http://dne.zycfv.cn

aiohttp.ClientSession() 配合 async with
来源：http://lcz.316326.xyz

[U28] Py：类型别名
来源：http://dak.xinyue.icu

UserId = int
来源：http://iyc.cqqwz.cn

[U29] Py：属性校验
来源：http://yqi.9152youxi.cn

@property 与 @x.setter 配合
来源：http://axd.sweek.top

[U30] Py：数据类
来源：http://eho.epnwcf.com

@dataclass(slots=True)
来源：http://uoy.haohaochexian.top

[U31] Py：单测
来源：http://ciz.xziqi.cn

python -m pytest -q
来源：http://xrr.hfpthk.cn

[U32] Py：代码格式化
来源：http://xsj.wangshuangyany.cn

ruff format . && ruff check --fix .
来源：http://juz.jqgfzy.top

[U33] Py：打包发布
来源：http://cdz.jinqigfzy.top

python -m build  （依赖 pyproject.toml）
来源：http://hnu.zhengqikj.top

[U34] Py：判断编码
来源：http://zhn.hysaishi.cn

chardet.detect(raw)
来源：http://egr.redwolf501.top

[U35] Py：发送邮件
来源：http://ajk.redwolf501.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ysv.sjlbkw.cn

[U36] Py：定时任务
来源：http://pld.ehwqpu.com

schedule.every(10).minutes.do(job)
来源：http://zmc.shuidangran.top

[U37] Py：读写 Excel
来源：http://ngy.ybcxt.top

pandas.read_excel / DataFrame.to_excel
来源：http://rta.cqqwz.cn

[U38] Py：获取脚本所在目录
来源：http://drc.pengpengdd.cyou

Path(__file__).resolve().parent
来源：http://nvc.vehdjk.com

[U39] Py：判断是否在交互环境
来源：http://zid.meibo888.top

sys.stdout.isatty()
来源：http://isp.haohaochexian.top

[U40] Py：打印到标准错误
来源：http://ovt.zdbjq.cn

print("err", file=sys.stderr)
来源：http://ppm.ywan-chungtsiang.top

[U41] PHP：初始化 Composer 项目
来源：http://odm.cashguo.top

composer init;  composer require guzzlehttp/guzzle
来源：http://faa.fehbvm.com

[U42] PHP：PSR-4 自动加载
来源：http://cxi.shanyushiyangtech.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fkg.hammf.cn

[U43] PHP：声明命名空间
来源：http://maa.ybcxt.top

namespace App\Http;
来源：http://nxn.chenlongwang.top

[U44] PHP：开启严格类型
来源：http://gwp.jinqigfzy.top

declare(strict_types=1);
来源：http://inn.fktsv.cn

[U45] PHP：类型声明与返回类型
来源：http://aql.sxryk.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://mjh.jinqigufen.top

[U46] PHP：可空类型
来源：http://sue.hongshengwenyu.top

?string $name = null
来源：http://zzp.cheryme.top

[U47] PHP：联合类型
来源：http://qji.zdbjq.cn

int|string $id
来源：http://pau.wangshuangyany.cn

[U48] PHP：纯枚举
来源：http://wii.jqgufenzy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://irg.chenzaomai.com

[U49] PHP：只读属性
来源：http://ldf.guannengcc.top

public readonly string $name
来源：http://khu.zhiwuduotai.top

[U50] PHP：构造器属性提升
来源：http://nor.jiagoushi.top

public function __construct(private int $id) {}
来源：http://mif.yanxiufei.cn

[U51] PHP：数组解构
来源：http://xyh.fzhhl.top

[$a, $b] = $arr;
来源：http://hyd.cdnleiting.top

[U52] PHP：箭头函数
来源：http://qac.zhengqikj.top

$double = fn($x) => $x * 2;
来源：http://ewz.mhx1999.top

[U53] PHP：空合并运算符
来源：http://efm.zdbjq.cn

$v = $a ?? $b ?? "default";
来源：http://rem.chenzaomai.com

[U54] PHP：空安全调用
来源：http://nsw.jqgufenzy.top

$obj?->method()
来源：http://txe.fktsv.cn

[U55] PHP：match 表达式
来源：http://zgk.yvedp.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ovt.haohaochexian.top

[U56] PHP：命名参数
来源：http://rjl.sysykeji.top

f(a: 1, b: 2)
来源：http://unt.ppjwa.cn

[U57] PHP：字符串插值
来源：http://vne.shanyushiyangkeji.top

"值: {$a}"
来源：http://rii.jqgfzy.top

[U58] PHP：数组三件套
来源：http://omq.cashguo.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nqs.cucudq.cn

[U59] PHP：自定义排序
来源：http://sft.jiagoushi.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aqw.shanyushiyangtech.top

[U60] PHP：JSON 编解码
来源：http://uzz.pycfn.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hva.shanyushiyangkeji.top

[U61] PHP：正则
来源：http://def.jinqigufen.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://djv.gzhubu.top

[U62] PHP：日期对象
来源：http://eld.andypj.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wrf.yvedp.cn

[U63] PHP：文件读写
来源：http://qhc.yj20258.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bgt.snrcjt.cn

[U64] PHP：目录遍历
来源：http://xji.xylfe.cn

glob("dir/*.php");  scandir("dir");
来源：http://vtu.quarkkingdee.top

[U65] PHP：会话
来源：http://rpy.fengsongda.top

session_start();  $_SESSION["uid"] = 1;
来源：http://mhk.uphjek.com

[U66] PHP：设置 Cookie
来源：http://vfi.xziqi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nml.yueranfly.top

[U67] PHP：处理文件上传
来源：http://ble.zhijiandao.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://cij.gotoacloud.top

[U68] PHP：PDO 连接
来源：http://ggy.zhongyouzk.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bju.andypj.xyz

[U69] PHP：PDO 预处理
来源：http://ekq.hcnkem.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vjx.zhiwuduotai.top

[U70] PHP：PDO 事务
来源：http://qld.meibo888.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ixw.hfpthk.cn

[U71] PHP：抛出异常
来源：http://kil.pengpengdd.cyou

throw new RuntimeException("失败", 500);
来源：http://rue.meibo888.top

[U72] PHP：写错误日志
来源：http://for.hesvh.cn

error_log("失败: " . $e->getMessage());
来源：http://fwd.gotoacloud.top

[U73] PHP：读取 ini 配置
来源：http://buq.hnqzz.top

parse_ini_file("config.ini", true)
来源：http://sty.hongshengwenyu.top

[U74] PHP：读取环境变量
来源：http://kei.jinyuanbaomall.cn

getenv("APP_ENV") ?: "production"
来源：http://hms.chenzaomai.com

[U75] PHP：依赖注入
来源：http://llg.jqgufenzy.top

composer require psr/container
来源：http://tcw.xingfuxueyuan.xyz

[U76] PHP：简单路由
来源：http://adx.bjfxy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://cxo.svipenyu.cn

[U77] PHP：模板渲染
来源：http://uob.yuanzhike.top

composer require twig/twig
来源：http://naj.zdqjudy.top

[U78] PHP：单元测试
来源：http://cxx.xuetiantiany.cn

composer require --dev phpunit/phpunit
来源：http://ayr.yangfankeji.com

[U79] PHP：静态分析
来源：http://wkq.zycfv.cn

composer require --dev phpstan/phpstan
来源：http://bvd.bjfxy.top

[U80] PHP：代码规范修复
来源：http://lxa.jinghuilouyu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://fle.vehdjk.com

[U81] JS：初始化项目
来源：http://bup.bbcook.cn

npm init -y;  npm i express
来源：http://yih.pycfn.com

[U82] JS：package.json 脚本
来源：http://gcl.vqdsnc.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vmf.pengpengdd.cyou

[U83] JS：ES Module 导入导出
来源：http://nha.jqgfzy.top

export const a = 1;  import { a } from "./m.js";
来源：http://euf.yuxming.cn

[U84] JS：CommonJS 写法
来源：http://lex.zycfv.cn

module.exports = { a };  const { a } = require("./m");
来源：http://yar.xylfe.cn

[U85] JS：可选链
来源：http://pli.mhx1999.top

a?.b?.c
来源：http://qno.jqgufenzy.top

[U86] JS：空值合并
来源：http://zph.sufxvd.cn

a ?? b
来源：http://sbq.52xcode.cn

[U87] JS：解构默认值
来源：http://mbn.jianghu66.top

const { a = 1, b = 2 } = obj;
来源：http://ijs.sxryk.cn

[U88] JS：对象展开合并
来源：http://fpl.aibaodan.cn

{ ...a, ...b }
来源：http://ukz.jyoumei.cn

[U89] JS：数组去重
来源：http://tpk.chenzaomai.com

[...new Set(arr)]
来源：http://edq.316326.xyz

[U90] JS：数字数组排序
来源：http://ljk.tarul.cn

[...arr].sort((a, b) => a - b)
来源：http://lsw.xuanzx.com

[U91] JS：对象键值遍历
来源：http://emp.cdnleiting.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qzd.dashuyun.cn

[U92] JS：深拷贝
来源：http://vph.bjfxy.top

structuredClone(obj)
来源：http://obi.gaohongyu789.top

[U93] JS：模板字符串
来源：http://qif.zhiwuduotai.top

`共 ${n} 条`
来源：http://tzh.kuanghao11.cn

[U94] JS：箭头函数
来源：http://zgd.aizwys.cn

const double = x => x * 2;
来源：http://rbn.bbcook.cn

[U95] JS：Promise 包装
来源：http://axm.ydjk.org.cn

new Promise((resolve, reject) => {})
来源：http://ntu.shanyushiyangtech.top

[U96] JS：async/await 与异常
来源：http://rqg.cqqwz.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rtv.sweek.top

[U97] JS：并发请求
来源：http://wjq.gzhubu.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://toa.yuxming.cn

[U98] JS：fetch 带 JSON
来源：http://ciy.tianlin.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zpz.dianchejie.cn

[U99] JS：事件监听
来源：http://xul.cdnleiting.top

el.addEventListener("click", e => {})
来源：http://hus.sysykeji.top

[U100] JS：DOM 查询
来源：http://jyj.yj20258.top

document.querySelector(".item")
来源：http://rsf.zdqjudy.top

[U101] JS：classList 操作
来源：http://mjz.feifeiyinyue.top

el.classList.toggle("active")
来源：http://ppx.aizwys.cn

[U102] JS：本地存储
来源：http://gee.gogol.net.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jic.mhx1999.top

[U103] JS：定时器
来源：http://kzs.andypj.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ooe.birdmap.top

[U104] JS：防抖
来源：http://nwr.cqqwz.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nfp.hcnkem.com

[U105] JS：节流
来源：http://fqh.cheryme.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://thl.dianchejie.cn

[U106] JS：日期格式化
来源：http://hzi.jinqigufen.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rsk.shangyingyoupin.top

[U107] JS：数字千分位
来源：http://zlc.jianghu66.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://uhi.cheryme.top

[U108] JS：随机整数
来源：http://zep.fengsongda.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://eai.chenjidiqi.icu

[U109] JS：数组分组
来源：http://mtv.shanyushiyangtech.top

Object.groupBy(arr, x => x.type)
来源：http://juo.nanxuanxn.top

[U110] JS：数组分块
来源：http://ldb.hnxiangtu.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ihp.shanyushiyangtech.top

[U111] JS：对象转 Map
来源：http://iej.sufxvd.cn

new Map(Object.entries(obj))
来源：http://umt.zhijiandao.cn

[U112] JS：字符串补位
来源：http://jid.zhijiandao.cn

"7".padStart(3, "0")
来源：http://vnt.yuanzhike.top

[U113] JS：正则替换全部
来源：http://pot.zhengqikj.top

s.replaceAll("a", "b")
来源：http://jcp.aibaodan.cn

[U114] JS：JSON 深比较
来源：http://rua.gzhubu.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://vik.fktsv.cn

[U115] JS：生成 UUID
来源：http://xoz.shangyingyoupin.top

crypto.randomUUID()
来源：http://uhg.fktsv.cn

[U116] JS：类型检查（JSDoc）
来源：http://rld.fehbvm.com

/** @param {string} name */ function f(name) {}
来源：http://fjd.birdmap.top

[U117] JS：单元测试
来源：http://zss.yonumen.top

npm i -D vitest;  npx vitest
来源：http://wyt.jqgfzy.top

[U118] JS：开发服务器
来源：http://rlh.zhaomingkeji.xyz

npm i -D vite;  npx vite
来源：http://vol.bjfxy.top

[U119] JS：生产构建
来源：http://jgn.jiagoushi.top

npx vite build
来源：http://yzp.fengsongda.top

[U120] JS：读取环境变量（Vite）
来源：http://hwh.wangshuangyany.cn

import.meta.env.VITE_API_URL
来源：http://gxc.chenlongwang.top

================================================================================
来源：http://vrt.jlsjyb.cn

统计汇总
来源：http://fji.xylfe.cn

================================================================================
来源：http://oqn.zhongyouzk.top

按语言统计（条）：
来源：http://nax.yonumen.top

Python ......... 252
来源：http://ynr.fktsv.cn

PHP ............ 252
来源：http://maw.vehdjk.com

JavaScript ..... 252
来源：http://lps.redwolf501.top

TypeScript ..... 212
来源：http://yiv.shanyushiyangkeji.top

Java ........... 212
来源：http://hrk.redwolf501.top

Go ............. 212
来源：http://zck.gotoacloud.top

Ruby ........... 212
来源：http://yll.iojbl.cn

C# ............. 212
来源：http://ihd.tanke756.top

C .............. 30
来源：http://vjw.ctjpmb.com

C++ ............ 30
来源：http://dcl.ybcxt.top

SQL ............ 90
来源：http://idr.hnxiangtu.top

Bash ........... 80
来源：http://goe.9152youxi.cn

Kotlin ......... 15
来源：http://nme.guannengcc.top

Swift .......... 15
来源：http://lmq.fengsongda.top

Lua ............ 10
来源：http://bym.ivvv.top

Perl ........... 10
来源：http://trq.feifeiyinyue.top

Scala .......... 10
来源：http://bls.kuanghao11.cn

------------------------------------
来源：http://hxl.sxryk.cn

合计 ........... 2106 条
来源：http://ehc.gzhubu.top

按章节统计：
来源：http://qhi.zycfv.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://nhv.nanxuanxn.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wal.kuanghao11.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qnk.jinqigufen.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pas.tarul.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://suq.chenlongwang.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://kol.zdqjudy.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://uat.xuetiantiany.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gpe.daxiang520.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jgr.ywan-chungtsiang.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://iil.jlsjyb.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://lmm.nwbrower.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://uuw.cqqwz.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://lmo.smart0.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ppr.yfazqb.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mas.ydjk.org.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ekh.mhx1999.top

Q SQL 专题                              90
来源：http://xzg.tian-w.cn

R Bash 专题                             80
来源：http://pot.gzhubu.top

S C / C++ 专题                          60
来源：http://drl.ywan-chungtsiang.top

T 其他语言补充                          60
来源：http://eng.yfazqb.com

U 高频实用片段                         120
来源：http://dyr.gogol.net.cn

------------------------------------
来源：http://fpi.sxryk.cn

合计                                  2106 条
来源：http://jjm.0kj1m.cn

--------------------------------------------------------------------------------
来源：http://cja.hysaishi.cn

使用提醒
来源：http://yzz.mhx1999.top

--------------------------------------------------------------------------------
来源：http://tod.wangshuangyany.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ote.yueranfly.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ycu.guannengcc.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://oux.hongshengwenyu.top

在旧版本上使用前请先确认语法支持情况。
来源：http://omk.yuanzhike.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jvr.vqdsnc.cn

—— 文件结束 ——
来源：http://pgm.xinyue.icu

================================================================================
来源：http://orn.yonumen.top

程序语言常见例子速查手册（2024 版）
来源：http://anz.0kj1m.cn

Common Programming Examples Cheat Book
来源：http://owt.chenlongwang.top

================================================================================
来源：http://wvp.fktsv.cn

【收录内容】
来源：http://ctm.xingfuxueyuan.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://nda.yj20258.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tbz.jlsjyb.cn

SQL · Bash · C · C++
来源：http://irl.hnxiangtu.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://whp.hcnkem.com

【使用说明】
来源：http://tzx.yongpay.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ufq.feifeiyinyue.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://uyu.fzhhl.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://sye.cashguo.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://foj.sysykeji.top

Bash:  Shell         C:     C             C++:   C++
来源：http://byz.jqgufenzy.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://sim.jlsjyb.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://znp.redwolf501.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://uxb.shangyingyoupin.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://pnk.nanxuanxn.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://rke.yfazqb.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://udw.hnqzz.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ylo.zhiwuduotai.top

【文件统计】
来源：http://wru.xinyue.icu

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mnc.sweek.top

--------------------------------------------------------------------------------
来源：http://yhh.jiagoushi.top

目  录
来源：http://xfn.yj20258888.top

--------------------------------------------------------------------------------
来源：http://hfn.jqgufenzy.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zpx.fehbvm.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://fss.cdnleiting.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mzp.hcnkem.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://okx.chenjidiqi.icu

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vtn.cucudq.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wmh.wangshuangyany.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ccb.guowangkeji.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://plk.haohaochexian.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://knf.vqdsnc.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xqp.birdmap.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wjg.316326.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://dtc.feifeiyinyue.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://shg.fktsv.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://cus.feifeiyinyue.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://kwv.shanyushiyangkeji.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ppw.xuetiantiany.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ikn.shzxlz.cn


<!-- 参考信息 -->