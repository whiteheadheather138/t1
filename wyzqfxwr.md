代发 wailian999

[U19] Py：正则替换带回调
来源：http://qcl.xuanzx.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://oel.tian-w.cn

[U20] Py：缓存函数结果
来源：http://wsb.gotoacloud.top

@functools.lru_cache(maxsize=None)
来源：http://bwr.smart0.xyz

[U21] Py：自定义上下文管理器
来源：http://nmx.sweek.top

@contextlib.contextmanager
来源：http://vcz.meibo888.top

[U22] Py：矩阵转置
来源：http://qea.jqgfzy.top

list(zip(*m))
来源：http://cii.uphjek.com

[U23] Py：分块读取大文件
来源：http://nkq.tian-w.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://cqg.mhx1999.top

[U24] Py：路径操作
来源：http://fsy.fanxiaobao.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://uam.yj20258.top

[U25] Py：CSV 按字典读
来源：http://cyc.sufxvd.cn

csv.DictReader(f)
来源：http://qyr.hfpthk.cn

[U26] Py：并发下载
来源：http://kat.c1oappe.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yru.xuetiantiany.cn

[U27] Py：异步 HTTP
来源：http://jkk.mhx1999.top

aiohttp.ClientSession() 配合 async with
来源：http://hdx.birdmap.top

[U28] Py：类型别名
来源：http://ahp.nwbrower.top

UserId = int
来源：http://kep.52xcode.cn

[U29] Py：属性校验
来源：http://okd.hongshengwenyu.top

@property 与 @x.setter 配合
来源：http://hts.guowangkeji.top

[U30] Py：数据类
来源：http://cpc.hongshengwenyu.top

@dataclass(slots=True)
来源：http://eez.gogol.net.cn

[U31] Py：单测
来源：http://jwg.sysykeji.top

python -m pytest -q
来源：http://dur.vqdsnc.cn

[U32] Py：代码格式化
来源：http://opj.ybcxt.top

ruff format . && ruff check --fix .
来源：http://qoj.ybcxt.top

[U33] Py：打包发布
来源：http://igj.yj202588.top

python -m build  （依赖 pyproject.toml）
来源：http://frn.yfazqb.com

[U34] Py：判断编码
来源：http://yqm.jqgfzy.top

chardet.detect(raw)
来源：http://uvj.nanxinkj.top

[U35] Py：发送邮件
来源：http://bwt.smart0.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jte.bbcook.cn

[U36] Py：定时任务
来源：http://xiw.vqdsnc.cn

schedule.every(10).minutes.do(job)
来源：http://aia.tianlin.xyz

[U37] Py：读写 Excel
来源：http://ltw.fanxiaobao.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://cnz.aibaodan.cn

[U38] Py：获取脚本所在目录
来源：http://jah.cashguo.top

Path(__file__).resolve().parent
来源：http://axl.wangdashe.top

[U39] Py：判断是否在交互环境
来源：http://slf.tarul.cn

sys.stdout.isatty()
来源：http://nse.tianlin.xyz

[U40] Py：打印到标准错误
来源：http://zcd.shuidangran.top

print("err", file=sys.stderr)
来源：http://wcr.gzhubu.top

[U41] PHP：初始化 Composer 项目
来源：http://glb.cqqwz.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://gtj.zycfv.cn

[U42] PHP：PSR-4 自动加载
来源：http://zdb.wangdashe.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lin.guowangkeji.top

[U43] PHP：声明命名空间
来源：http://kxo.jiagoushi.top

namespace App\Http;
来源：http://ntc.nanxuanxn.top

[U44] PHP：开启严格类型
来源：http://ulj.dashuyun.cn

declare(strict_types=1);
来源：http://dxf.nanxuanxn.top

[U45] PHP：类型声明与返回类型
来源：http://aee.shanyushiyangtech.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ekh.bbcook.cn

[U46] PHP：可空类型
来源：http://pfv.chenzaomai.com

?string $name = null
来源：http://hhu.ctjpmb.com

[U47] PHP：联合类型
来源：http://ygg.xinyue.icu

int|string $id
来源：http://zbh.shanyushiyangtech.top

[U48] PHP：纯枚举
来源：http://nbt.ywan-chungtsiang.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ugp.havefunace.top

[U49] PHP：只读属性
来源：http://zdx.yonumen.top

public readonly string $name
来源：http://uhp.shzxlz.cn

[U50] PHP：构造器属性提升
来源：http://osu.smart0.xyz

public function __construct(private int $id) {}
来源：http://xif.fanxiaobao.xyz

[U51] PHP：数组解构
来源：http://pgw.tanke756.top

[$a, $b] = $arr;
来源：http://hrw.hesvh.cn

[U52] PHP：箭头函数
来源：http://sms.xziqi.cn

$double = fn($x) => $x * 2;
来源：http://jty.fzhhl.top

[U53] PHP：空合并运算符
来源：http://bew.ybcxt.top

$v = $a ?? $b ?? "default";
来源：http://cyr.cdnleiting.top

[U54] PHP：空安全调用
来源：http://yro.daxiang520.top

$obj?->method()
来源：http://nea.dianchejie.cn

[U55] PHP：match 表达式
来源：http://xxw.fzhhl.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wdd.nwbrower.top

[U56] PHP：命名参数
来源：http://lqd.svipenyu.cn

f(a: 1, b: 2)
来源：http://woo.quarkkingdee.top

[U57] PHP：字符串插值
来源：http://cwi.jinqigufen.top

"值: {$a}"
来源：http://ksa.fanxiaobao.xyz

[U58] PHP：数组三件套
来源：http://ivh.tarul.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nqy.sysykeji.top

[U59] PHP：自定义排序
来源：http://ggd.cheryme.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lcz.fengsongda.top

[U60] PHP：JSON 编解码
来源：http://idp.aizwys.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fub.jianghu66.top

[U61] PHP：正则
来源：http://hbe.xuetiantiany.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pmx.daria6918.cn

[U62] PHP：日期对象
来源：http://fgn.jinyuanbaomall.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zde.shuidangran.top

[U63] PHP：文件读写
来源：http://rvd.jinghuilouyu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://knb.hammf.cn

[U64] PHP：目录遍历
来源：http://nrr.yangfankeji.com

glob("dir/*.php");  scandir("dir");
来源：http://zsg.vqdsnc.cn

[U65] PHP：会话
来源：http://ynp.andypj.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://csv.cheryme.top

[U66] PHP：设置 Cookie
来源：http://myb.yuxming.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hgi.yfazqb.com

[U67] PHP：处理文件上传
来源：http://vhg.yonumen.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tof.ydzc1.top

[U68] PHP：PDO 连接
来源：http://pqz.uphjek.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jge.hfpthk.cn

[U69] PHP：PDO 预处理
来源：http://gez.xylfe.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gzz.yanxiufei.cn

[U70] PHP：PDO 事务
来源：http://qlc.wangdashe.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dyf.fengsongda.top

[U71] PHP：抛出异常
来源：http://seb.yj20258.top

throw new RuntimeException("失败", 500);
来源：http://qgs.ybcxt.top

[U72] PHP：写错误日志
来源：http://xau.zdbjq.cn

error_log("失败: " . $e->getMessage());
来源：http://ddw.guowangkeji.top

[U73] PHP：读取 ini 配置
来源：http://rxp.jinghuilouyu.cn

parse_ini_file("config.ini", true)
来源：http://wll.fehbvm.com

[U74] PHP：读取环境变量
来源：http://gqf.bbcook.cn

getenv("APP_ENV") ?: "production"
来源：http://gka.jinqigfzy.top

[U75] PHP：依赖注入
来源：http://yaj.guannengcc.top

composer require psr/container
来源：http://uic.haohaochexian.top

[U76] PHP：简单路由
来源：http://vvt.fengsongda.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vcq.tianlin.xyz

[U77] PHP：模板渲染
来源：http://lah.meibo888.top

composer require twig/twig
来源：http://kun.hcnkem.com

[U78] PHP：单元测试
来源：http://zjv.ppjwa.cn

composer require --dev phpunit/phpunit
来源：http://hpe.hywenlv.cn

[U79] PHP：静态分析
来源：http://osk.ydzc1.top

composer require --dev phpstan/phpstan
来源：http://wqq.zycfv.cn

[U80] PHP：代码规范修复
来源：http://spt.zhixingplan.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://fys.jlsjyb.cn

[U81] JS：初始化项目
来源：http://tkz.yj20258.top

npm init -y;  npm i express
来源：http://ytx.andypj.xyz

[U82] JS：package.json 脚本
来源：http://ckm.jinghuilouyu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hrl.pengpengdd.cyou

[U83] JS：ES Module 导入导出
来源：http://zzj.kuanghao11.cn

export const a = 1;  import { a } from "./m.js";
来源：http://asu.nwbrower.top

[U84] JS：CommonJS 写法
来源：http://epx.jianghu66.top

module.exports = { a };  const { a } = require("./m");
来源：http://cke.zhaomingkeji.xyz

[U85] JS：可选链
来源：http://xbd.jqgufenzy.top

a?.b?.c
来源：http://ugc.ydjk.org.cn

[U86] JS：空值合并
来源：http://wjn.wangshuangyany.cn

a ?? b
来源：http://maa.ywan-chungtsiang.top

[U87] JS：解构默认值
来源：http://pae.hfpthk.cn

const { a = 1, b = 2 } = obj;
来源：http://rkf.fktsv.cn

[U88] JS：对象展开合并
来源：http://dqm.tanke756.top

{ ...a, ...b }
来源：http://zvh.aizwys.cn

[U89] JS：数组去重
来源：http://slk.nanxuanxn.top

[...new Set(arr)]
来源：http://oqu.ehwqpu.com

[U90] JS：数字数组排序
来源：http://gjd.ydjk.org.cn

[...arr].sort((a, b) => a - b)
来源：http://zca.hammf.cn

[U91] JS：对象键值遍历
来源：http://irx.ydzc1.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xcp.snrcjt.cn

[U92] JS：深拷贝
来源：http://lrm.kuanghao11.cn

structuredClone(obj)
来源：http://han.bbcook.cn

[U93] JS：模板字符串
来源：http://kaz.cdnleiting.top

`共 ${n} 条`
来源：http://grx.jlsjyb.cn

[U94] JS：箭头函数
来源：http://iiu.vehdjk.com

const double = x => x * 2;
来源：http://epx.yj20258.top

[U95] JS：Promise 包装
来源：http://lwm.shanyushiyangtech.top

new Promise((resolve, reject) => {})
来源：http://tnr.yanxiufei.cn

[U96] JS：async/await 与异常
来源：http://ptt.tianlin.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mxd.9152youxi.cn

[U97] JS：并发请求
来源：http://dki.chenlongwang.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://xsk.hnqzz.top

[U98] JS：fetch 带 JSON
来源：http://gte.zhijiandao.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mon.daria6918.cn

[U99] JS：事件监听
来源：http://ndx.daxiang520.top

el.addEventListener("click", e => {})
来源：http://gix.ctjpmb.com

[U100] JS：DOM 查询
来源：http://zmx.sufxvd.cn

document.querySelector(".item")
来源：http://apu.daxiang520.top

[U101] JS：classList 操作
来源：http://pui.tianlin.xyz

el.classList.toggle("active")
来源：http://kkz.daxiang520.top

[U102] JS：本地存储
来源：http://whg.zhijiandao.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://xpv.ppjwa.cn

[U103] JS：定时器
来源：http://ohv.zhengqikj.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pyv.xuetiantiany.cn

[U104] JS：防抖
来源：http://ems.mhx1999.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ala.epnwcf.com

[U105] JS：节流
来源：http://qqh.jinqigufen.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vgt.daxiang520.top

[U106] JS：日期格式化
来源：http://kpu.tarul.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rdg.hammf.cn

[U107] JS：数字千分位
来源：http://frc.jinqigfzy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://sst.jyoumei.cn

[U108] JS：随机整数
来源：http://xmm.hammf.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bru.hfpthk.cn

[U109] JS：数组分组
来源：http://awj.ctjpmb.com

Object.groupBy(arr, x => x.type)
来源：http://tuh.sweek.top

[U110] JS：数组分块
来源：http://zek.ivvv.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://htd.zhoulong.xyz

[U111] JS：对象转 Map
来源：http://xcj.ctjpmb.com

new Map(Object.entries(obj))
来源：http://xdj.wangdashe.top

[U112] JS：字符串补位
来源：http://tux.0kj1m.cn

"7".padStart(3, "0")
来源：http://ygf.gzhubu.top

[U113] JS：正则替换全部
来源：http://ybf.zhijiandao.cn

s.replaceAll("a", "b")
来源：http://glf.yj20258888.top

[U114] JS：JSON 深比较
来源：http://lvy.yueranfly.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://kmj.xziqi.cn

[U115] JS：生成 UUID
来源：http://ezy.cdnleiting.top

crypto.randomUUID()
来源：http://vgp.cheryme.top

[U116] JS：类型检查（JSDoc）
来源：http://mel.hcnkem.com

/** @param {string} name */ function f(name) {}
来源：http://vfx.xylfe.cn

[U117] JS：单元测试
来源：http://zac.gzhubu.top

npm i -D vitest;  npx vitest
来源：http://mws.dashuyun.cn

[U118] JS：开发服务器
来源：http://tsz.52xcode.cn

npm i -D vite;  npx vite
来源：http://xyn.9152youxi.cn

[U119] JS：生产构建
来源：http://knq.chenjidiqi.icu

npx vite build
来源：http://nqz.xylfe.cn

[U120] JS：读取环境变量（Vite）
来源：http://dgk.tarul.cn

import.meta.env.VITE_API_URL
来源：http://mal.ctjpmb.com

================================================================================
来源：http://hes.sxryk.cn

统计汇总
来源：http://cdt.ydjk.org.cn

================================================================================
来源：http://ttm.shzxlz.cn

按语言统计（条）：
来源：http://pux.zhijiandao.cn

Python ......... 252
来源：http://gyo.zhongyouzk.top

PHP ............ 252
来源：http://dsz.yuanzhike.top

JavaScript ..... 252
来源：http://mkz.gogol.net.cn

TypeScript ..... 212
来源：http://ezn.nanxinkj.top

Java ........... 212
来源：http://icm.aizwys.cn

Go ............. 212
来源：http://xni.yj20258.top

Ruby ........... 212
来源：http://kwf.hongshengwenyu.top

C# ............. 212
来源：http://qkc.dashuyun.cn

C .............. 30
来源：http://thu.shuidangran.top

C++ ............ 30
来源：http://xwr.pengpengdd.cyou

SQL ............ 90
来源：http://izq.zhijiandao.cn

Bash ........... 80
来源：http://jts.fanxiaobao.xyz

Kotlin ......... 15
来源：http://rit.dashuyun.cn

Swift .......... 15
来源：http://wlr.xuetiantiany.cn

Lua ............ 10
来源：http://bwf.hongshengwenyu.top

Perl ........... 10
来源：http://axd.xingfuxueyuan.xyz

Scala .......... 10
来源：http://cyr.gzhubu.top

------------------------------------
来源：http://ype.xuetiantiany.cn

合计 ........... 2106 条
来源：http://iub.shanyushiyangtech.top

按章节统计：
来源：http://vgm.yongpay.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://otj.ctjpmb.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bof.jqgfzy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://eup.tarul.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ala.jlsjyb.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://kcp.fzhhl.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://cvx.guowangkeji.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://uyv.iojbl.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kda.yonumen.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rvh.gaohongyu789.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zao.yfazqb.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kqs.yfazqb.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jvw.zdqjudy.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://gzg.zdqjudy.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vhq.daxiang520.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://avs.ctjpmb.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://avd.sysykeji.top

Q SQL 专题                              90
来源：http://yzw.yonumen.top

R Bash 专题                             80
来源：http://ypp.wangdashe.top

S C / C++ 专题                          60
来源：http://lxg.zdqjudy.top

T 其他语言补充                          60
来源：http://okp.zhijiandao.cn

U 高频实用片段                         120
来源：http://lal.yvedp.cn

------------------------------------
来源：http://oid.hesvh.cn

合计                                  2106 条
来源：http://bni.fktsv.cn

--------------------------------------------------------------------------------
来源：http://juu.ywan-chungtsiang.top

使用提醒
来源：http://wth.birdmap.top

--------------------------------------------------------------------------------
来源：http://bwa.yuanzhike.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://pbx.yvedp.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://daj.nanxinkj.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://zfn.feifeiyinyue.top

在旧版本上使用前请先确认语法支持情况。
来源：http://umn.hongshengwenyu.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://nrc.yj20258888.top

—— 文件结束 ——
来源：http://slw.zhixingplan.top

================================================================================
来源：http://psh.sjlbkw.cn

程序语言常见例子速查手册（2024 版）
来源：http://xjp.aizwys.cn

Common Programming Examples Cheat Book
来源：http://pvz.yangfankeji.com

================================================================================
来源：http://mlu.bbcook.cn

【收录内容】
来源：http://uan.daria6918.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://yxs.xuanzx.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hmu.zhiwuduotai.top

SQL · Bash · C · C++
来源：http://qgt.yvedp.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://bgu.quarkkingdee.top

【使用说明】
来源：http://tny.ppjwa.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hzk.yangfankeji.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://uhl.hammf.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://meu.vqdsnc.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://jqy.quarkkingdee.top

Bash:  Shell         C:     C             C++:   C++
来源：http://adm.316326.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://tcc.52xcode.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://zwb.gzhubu.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://cyh.iojbl.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://uhm.jlsjyb.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://fqs.cucudq.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://acx.hnxiangtu.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://smo.xziqi.cn

【文件统计】
来源：http://jvl.ydjk.org.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://bvi.chenzaomai.com

--------------------------------------------------------------------------------
来源：http://pre.zhixingplan.top

目  录
来源：http://xqi.haohaochexian.top

--------------------------------------------------------------------------------
来源：http://jxg.zdbjq.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://skt.jiagoushi.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hgg.ywan-chungtsiang.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fbh.shangyingyoupin.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mku.yfazqb.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://lrj.yonumen.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://tsx.jinqigufen.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://zjn.zhengqikj.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ret.pycfn.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://bzl.yj20258888.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://veg.zhaomingkeji.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://sad.zhongyouzk.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://fbo.chenjidiqi.icu

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://otx.hongshengwenyu.top


<!-- 参考信息 -->