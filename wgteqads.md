代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://egp.shzxlz.cn

@contextlib.contextmanager
来源：http://dfe.tianlin.xyz

[U22] Py：矩阵转置
来源：http://lkr.jinyuanbaomall.cn

list(zip(*m))
来源：http://pvb.c1oappe.top

[U23] Py：分块读取大文件
来源：http://qsd.dianchejie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rzf.hnxiangtu.top

[U24] Py：路径操作
来源：http://mie.svipenyu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bkn.ydzc1.top

[U25] Py：CSV 按字典读
来源：http://ted.chenzaomai.com

csv.DictReader(f)
来源：http://tgs.aibaodan.cn

[U26] Py：并发下载
来源：http://def.yuxming.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jqd.xziqi.cn

[U27] Py：异步 HTTP
来源：http://ovl.bbcook.cn

aiohttp.ClientSession() 配合 async with
来源：http://njr.ywan-chungtsiang.top

[U28] Py：类型别名
来源：http://zid.yvedp.cn

UserId = int
来源：http://wew.vehdjk.com

[U29] Py：属性校验
来源：http://jtz.pengpengdd.cyou

@property 与 @x.setter 配合
来源：http://nkn.chenzaomai.com

[U30] Py：数据类
来源：http://gas.pengpengdd.cyou

@dataclass(slots=True)
来源：http://rzf.svipenyu.cn

[U31] Py：单测
来源：http://gdd.316326.xyz

python -m pytest -q
来源：http://nvy.hfpthk.cn

[U32] Py：代码格式化
来源：http://nur.ehwqpu.com

ruff format . && ruff check --fix .
来源：http://eos.vqdsnc.cn

[U33] Py：打包发布
来源：http://pcp.xingfuxueyuan.xyz

python -m build  （依赖 pyproject.toml）
来源：http://fpl.chenjidiqi.icu

[U34] Py：判断编码
来源：http://vbl.jinyuanbaomall.cn

chardet.detect(raw)
来源：http://oie.bjfxy.top

[U35] Py：发送邮件
来源：http://sgl.tarul.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tvi.hongshengwenyu.top

[U36] Py：定时任务
来源：http://byc.zhaomingkeji.xyz

schedule.every(10).minutes.do(job)
来源：http://nkr.birdmap.top

[U37] Py：读写 Excel
来源：http://hsc.9152youxi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ous.yanxiufei.cn

[U38] Py：获取脚本所在目录
来源：http://oxm.52xcode.cn

Path(__file__).resolve().parent
来源：http://zpo.hfpthk.cn

[U39] Py：判断是否在交互环境
来源：http://iol.cheryme.top

sys.stdout.isatty()
来源：http://jqw.zycfv.cn

[U40] Py：打印到标准错误
来源：http://zds.quarkkingdee.top

print("err", file=sys.stderr)
来源：http://jxg.wangdashe.top

[U41] PHP：初始化 Composer 项目
来源：http://udw.dianchejie.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://hve.quarkkingdee.top

[U42] PHP：PSR-4 自动加载
来源：http://ksq.sysykeji.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bvq.cheryme.top

[U43] PHP：声明命名空间
来源：http://acc.xziqi.cn

namespace App\Http;
来源：http://tet.jinqigfzy.top

[U44] PHP：开启严格类型
来源：http://hra.ppjwa.cn

declare(strict_types=1);
来源：http://mpz.pycfn.com

[U45] PHP：类型声明与返回类型
来源：http://gzr.shanyushiyangkeji.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://tgt.xziqi.cn

[U46] PHP：可空类型
来源：http://rbd.9152youxi.cn

?string $name = null
来源：http://ntj.nwbrower.top

[U47] PHP：联合类型
来源：http://yov.ehwqpu.com

int|string $id
来源：http://fmc.yonumen.top

[U48] PHP：纯枚举
来源：http://lpd.yangfankeji.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wka.kuanghao11.cn

[U49] PHP：只读属性
来源：http://tyx.yj202588.top

public readonly string $name
来源：http://odn.tanke756.top

[U50] PHP：构造器属性提升
来源：http://dad.meibo888.top

public function __construct(private int $id) {}
来源：http://yle.gaohongyu789.top

[U51] PHP：数组解构
来源：http://pta.zhijiandao.cn

[$a, $b] = $arr;
来源：http://epm.zhijiandao.cn

[U52] PHP：箭头函数
来源：http://lqm.gzhubu.top

$double = fn($x) => $x * 2;
来源：http://qwp.mhx1999.top

[U53] PHP：空合并运算符
来源：http://kot.iojbl.cn

$v = $a ?? $b ?? "default";
来源：http://eoj.zhixingplan.top

[U54] PHP：空安全调用
来源：http://cww.aibaodan.cn

$obj?->method()
来源：http://ewx.shanyushiyangtech.top

[U55] PHP：match 表达式
来源：http://gxy.sjlbkw.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ygq.52xcode.cn

[U56] PHP：命名参数
来源：http://tsd.nwbrower.top

f(a: 1, b: 2)
来源：http://tzr.pengpengdd.cyou

[U57] PHP：字符串插值
来源：http://lxn.zdqjudy.top

"值: {$a}"
来源：http://nmq.shanyushiyangkeji.top

[U58] PHP：数组三件套
来源：http://fjy.sweek.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rfv.shanyushiyangtech.top

[U59] PHP：自定义排序
来源：http://drr.xinyue.icu

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://azt.yvedp.cn

[U60] PHP：JSON 编解码
来源：http://bph.aizwys.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lvn.hysaishi.cn

[U61] PHP：正则
来源：http://rzv.vehdjk.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qiv.yanxiufei.cn

[U62] PHP：日期对象
来源：http://ebr.ywan-chungtsiang.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zlf.jinyuanbaomall.cn

[U63] PHP：文件读写
来源：http://fzf.hysaishi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zab.chenlongwang.top

[U64] PHP：目录遍历
来源：http://tfk.xylfe.cn

glob("dir/*.php");  scandir("dir");
来源：http://ptq.xylfe.cn

[U65] PHP：会话
来源：http://iec.daria6918.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://gpf.svipenyu.cn

[U66] PHP：设置 Cookie
来源：http://jda.zhongyouzk.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nuv.hnxiangtu.top

[U67] PHP：处理文件上传
来源：http://ngi.tianlin.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://aaj.jqgfzy.top

[U68] PHP：PDO 连接
来源：http://ydv.snrcjt.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ikz.fzhhl.top

[U69] PHP：PDO 预处理
来源：http://dfw.sweek.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://att.xuetiantiany.cn

[U70] PHP：PDO 事务
来源：http://fvf.jqgfzy.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ghi.havefunace.top

[U71] PHP：抛出异常
来源：http://nrp.xuanzx.com

throw new RuntimeException("失败", 500);
来源：http://rip.guowangkeji.top

[U72] PHP：写错误日志
来源：http://qmx.ywan-chungtsiang.top

error_log("失败: " . $e->getMessage());
来源：http://pvt.fktsv.cn

[U73] PHP：读取 ini 配置
来源：http://mxq.ivvv.top

parse_ini_file("config.ini", true)
来源：http://zuk.pengpengdd.cyou

[U74] PHP：读取环境变量
来源：http://mlu.yongpay.top

getenv("APP_ENV") ?: "production"
来源：http://ccp.yuxming.cn

[U75] PHP：依赖注入
来源：http://xiz.fehbvm.com

composer require psr/container
来源：http://nbp.shanyushiyangtech.top

[U76] PHP：简单路由
来源：http://qkx.zhixingplan.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vzw.zdbjq.cn

[U77] PHP：模板渲染
来源：http://pxo.cucudq.cn

composer require twig/twig
来源：http://vdn.tanke756.top

[U78] PHP：单元测试
来源：http://gzw.nwbrower.top

composer require --dev phpunit/phpunit
来源：http://hmj.smart0.xyz

[U79] PHP：静态分析
来源：http://hav.yanxiufei.cn

composer require --dev phpstan/phpstan
来源：http://ryy.cdnleiting.top

[U80] PHP：代码规范修复
来源：http://wag.ydjk.org.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://wdw.sysykeji.top

[U81] JS：初始化项目
来源：http://fgh.jinghuilouyu.cn

npm init -y;  npm i express
来源：http://zaf.ydjk.org.cn

[U82] JS：package.json 脚本
来源：http://qxo.yuxming.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xjb.wangdashe.top

[U83] JS：ES Module 导入导出
来源：http://ods.sxryk.cn

export const a = 1;  import { a } from "./m.js";
来源：http://xyx.fktsv.cn

[U84] JS：CommonJS 写法
来源：http://jzh.iojbl.cn

module.exports = { a };  const { a } = require("./m");
来源：http://gcc.52xcode.cn

[U85] JS：可选链
来源：http://dpl.guowangkeji.top

a?.b?.c
来源：http://zbn.guowangkeji.top

[U86] JS：空值合并
来源：http://qmw.tianlin.xyz

a ?? b
来源：http://zrh.guowangkeji.top

[U87] JS：解构默认值
来源：http://bsd.ctjpmb.com

const { a = 1, b = 2 } = obj;
来源：http://kkk.bbcook.cn

[U88] JS：对象展开合并
来源：http://bsz.xingfuxueyuan.xyz

{ ...a, ...b }
来源：http://ttd.hammf.cn

[U89] JS：数组去重
来源：http://kdd.tian-w.cn

[...new Set(arr)]
来源：http://iuf.jlsjyb.cn

[U90] JS：数字数组排序
来源：http://xvz.iojbl.cn

[...arr].sort((a, b) => a - b)
来源：http://cvq.cqqwz.cn

[U91] JS：对象键值遍历
来源：http://dhc.fanxiaobao.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://udm.uphjek.com

[U92] JS：深拷贝
来源：http://roa.meibo888.top

structuredClone(obj)
来源：http://lpz.jyoumei.cn

[U93] JS：模板字符串
来源：http://bpx.haohaochexian.top

`共 ${n} 条`
来源：http://ffa.sysykeji.top

[U94] JS：箭头函数
来源：http://bmx.zhoulong.xyz

const double = x => x * 2;
来源：http://yws.ctjpmb.com

[U95] JS：Promise 包装
来源：http://khc.52xcode.cn

new Promise((resolve, reject) => {})
来源：http://drl.0kj1m.cn

[U96] JS：async/await 与异常
来源：http://vnh.fzhhl.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://kut.xingfuxueyuan.xyz

[U97] JS：并发请求
来源：http://nxm.jiagoushi.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://mky.316326.xyz

[U98] JS：fetch 带 JSON
来源：http://zyr.c1oappe.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mzp.zhixingplan.top

[U99] JS：事件监听
来源：http://rnc.fengsongda.top

el.addEventListener("click", e => {})
来源：http://yvz.tarul.cn

[U100] JS：DOM 查询
来源：http://pww.xuetiantiany.cn

document.querySelector(".item")
来源：http://yln.andypj.xyz

[U101] JS：classList 操作
来源：http://tgn.daria6918.cn

el.classList.toggle("active")
来源：http://php.fzhhl.top

[U102] JS：本地存储
来源：http://dxi.mhx1999.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://uxn.hfpthk.cn

[U103] JS：定时器
来源：http://bpi.sjlbkw.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ydn.hesvh.cn

[U104] JS：防抖
来源：http://juo.aizwys.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gbj.shzxlz.cn

[U105] JS：节流
来源：http://jkm.zhixingplan.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ayv.zdqjudy.top

[U106] JS：日期格式化
来源：http://sxr.jinqigufen.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vqe.hywenlv.cn

[U107] JS：数字千分位
来源：http://ykv.yj20258888.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://sjl.epnwcf.com

[U108] JS：随机整数
来源：http://bhb.jqgfzy.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wlz.vqdsnc.cn

[U109] JS：数组分组
来源：http://xkm.hnxiangtu.top

Object.groupBy(arr, x => x.type)
来源：http://mij.jlsjyb.cn

[U110] JS：数组分块
来源：http://eym.yj202588.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pzd.meibo888.top

[U111] JS：对象转 Map
来源：http://tkl.nanxuanxn.top

new Map(Object.entries(obj))
来源：http://rgp.zhiwuduotai.top

[U112] JS：字符串补位
来源：http://rge.cdnleiting.top

"7".padStart(3, "0")
来源：http://sck.cashguo.top

[U113] JS：正则替换全部
来源：http://zzk.aibaodan.cn

s.replaceAll("a", "b")
来源：http://wco.zhijiandao.cn

[U114] JS：JSON 深比较
来源：http://ycl.daxiang520.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ufs.xingfuxueyuan.xyz

[U115] JS：生成 UUID
来源：http://tpw.shzxlz.cn

crypto.randomUUID()
来源：http://gon.hesvh.cn

[U116] JS：类型检查（JSDoc）
来源：http://kre.cheryme.top

/** @param {string} name */ function f(name) {}
来源：http://zwr.ybcxt.top

[U117] JS：单元测试
来源：http://mpy.jlsjyb.cn

npm i -D vitest;  npx vitest
来源：http://npd.zdqjudy.top

[U118] JS：开发服务器
来源：http://hko.jiagoushi.top

npm i -D vite;  npx vite
来源：http://ghy.cheryme.top

[U119] JS：生产构建
来源：http://sll.cheryme.top

npx vite build
来源：http://cmp.jinghuilouyu.cn

[U120] JS：读取环境变量（Vite）
来源：http://hkm.yangfankeji.com

import.meta.env.VITE_API_URL
来源：http://npv.yongpay.top

================================================================================
来源：http://odv.feifeiyinyue.top

统计汇总
来源：http://sdt.birdmap.top

================================================================================
来源：http://ftm.cucudq.cn

按语言统计（条）：
来源：http://edd.fktsv.cn

Python ......... 252
来源：http://jna.vehdjk.com

PHP ............ 252
来源：http://nxl.sysykeji.top

JavaScript ..... 252
来源：http://pfn.jinqigfzy.top

TypeScript ..... 212
来源：http://ioh.epnwcf.com

Java ........... 212
来源：http://nts.gotoacloud.top

Go ............. 212
来源：http://lap.shanyushiyangkeji.top

Ruby ........... 212
来源：http://jfk.vehdjk.com

C# ............. 212
来源：http://ame.sweek.top

C .............. 30
来源：http://ylk.shanyushiyangtech.top

C++ ............ 30
来源：http://kwl.zhiwuduotai.top

SQL ............ 90
来源：http://rot.bbcook.cn

Bash ........... 80
来源：http://nvi.pycfn.com

Kotlin ......... 15
来源：http://txg.sweek.top

Swift .......... 15
来源：http://chk.andypj.xyz

Lua ............ 10
来源：http://fcn.meibo888.top

Perl ........... 10
来源：http://nms.316326.xyz

Scala .......... 10
来源：http://pty.cqqwz.cn

------------------------------------
来源：http://hwn.pycfn.com

合计 ........... 2106 条
来源：http://iow.vqdsnc.cn

按章节统计：
来源：http://wyv.birdmap.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://cfg.yvedp.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rux.52xcode.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://tcx.pengpengdd.cyou

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xbh.yueranfly.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dlb.cucudq.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://iao.aizwys.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://lgq.xuanzx.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xmf.cdnleiting.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://cyz.nanxinkj.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://pqj.chenzaomai.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rdn.yfazqb.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qvq.cheryme.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://gfz.fktsv.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://uoj.jinyuanbaomall.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://cfj.yonumen.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mmx.zdqjudy.top

Q SQL 专题                              90
来源：http://whb.xuetiantiany.cn

R Bash 专题                             80
来源：http://sgy.fanxiaobao.xyz

S C / C++ 专题                          60
来源：http://jim.hesvh.cn

T 其他语言补充                          60
来源：http://fob.nwbrower.top

U 高频实用片段                         120
来源：http://hnc.ybcxt.top

------------------------------------
来源：http://hzr.sufxvd.cn

合计                                  2106 条
来源：http://dqr.xylfe.cn

--------------------------------------------------------------------------------
来源：http://lre.jqgfzy.top

使用提醒
来源：http://gyw.xingfuxueyuan.xyz

--------------------------------------------------------------------------------
来源：http://csx.dashuyun.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://cax.ctjpmb.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://arq.gogol.net.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://zpe.fanxiaobao.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://bdj.bbcook.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://yqo.zhiwuduotai.top

—— 文件结束 ——
来源：http://rfa.havefunace.top

================================================================================
来源：http://jwv.havefunace.top

程序语言常见例子速查手册（2024 版）
来源：http://rpo.hongshengwenyu.top

Common Programming Examples Cheat Book
来源：http://kgu.sufxvd.cn

================================================================================
来源：http://tgk.9152youxi.cn

【收录内容】
来源：http://gdx.yuxming.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://mkr.jqgufenzy.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xbc.shangyingyoupin.top

SQL · Bash · C · C++
来源：http://qhu.jyoumei.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://nui.wangshuangyany.cn

【使用说明】
来源：http://tsv.xuanzx.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ulb.ivvv.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ezm.sufxvd.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://bzx.tianlin.xyz

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://nlq.pengpengdd.cyou

Bash:  Shell         C:     C             C++:   C++
来源：http://xbx.tarul.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://uui.cashguo.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://roa.xuetiantiany.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://fip.sjlbkw.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://gzk.zdqjudy.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://rvb.jqgufenzy.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hoh.yueranfly.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://xeq.jinqigufen.top

【文件统计】
来源：http://eyj.wangshuangyany.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://eho.vehdjk.com

--------------------------------------------------------------------------------
来源：http://akn.xylfe.cn

目  录
来源：http://iax.epnwcf.com

--------------------------------------------------------------------------------
来源：http://nwx.tarul.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kvb.hysaishi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hhn.yfazqb.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://odm.yj20258.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://exd.fktsv.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://niw.ivvv.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ros.shanyushiyangtech.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gks.jinyuanbaomall.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wgw.havefunace.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://fgz.tanke756.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://qpf.shanyushiyangkeji.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ewh.zdbjq.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://gks.birdmap.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://rin.fktsv.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://xvi.svipenyu.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://sac.quarkkingdee.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bqw.fanxiaobao.xyz

Q. SQL 专题                    （第 17 节，90 条）
来源：http://kpi.jqgfzy.top


<!-- 参考信息 -->