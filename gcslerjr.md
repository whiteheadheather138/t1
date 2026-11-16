代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://wor.wangshuangyany.cn

@contextlib.contextmanager
来源：http://isy.chenzaomai.com

[U22] Py：矩阵转置
来源：http://mzp.bjfxy.top

list(zip(*m))
来源：http://uxj.pengpengdd.cyou

[U23] Py：分块读取大文件
来源：http://dax.xingfuxueyuan.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ade.shuidangran.top

[U24] Py：路径操作
来源：http://wjb.ppjwa.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fxr.cheryme.top

[U25] Py：CSV 按字典读
来源：http://ucy.kuanghao11.cn

csv.DictReader(f)
来源：http://czx.aibaodan.cn

[U26] Py：并发下载
来源：http://pwf.zhengqikj.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://eje.daria6918.cn

[U27] Py：异步 HTTP
来源：http://pbg.zdqjudy.top

aiohttp.ClientSession() 配合 async with
来源：http://tmk.smart0.xyz

[U28] Py：类型别名
来源：http://icg.xziqi.cn

UserId = int
来源：http://czv.daria6918.cn

[U29] Py：属性校验
来源：http://zow.zdqjudy.top

@property 与 @x.setter 配合
来源：http://ndz.yuxming.cn

[U30] Py：数据类
来源：http://gqv.wangshuangyany.cn

@dataclass(slots=True)
来源：http://tio.cucudq.cn

[U31] Py：单测
来源：http://qby.tian-w.cn

python -m pytest -q
来源：http://cgc.yueranfly.top

[U32] Py：代码格式化
来源：http://whd.ehwqpu.com

ruff format . && ruff check --fix .
来源：http://ysm.yj20258888.top

[U33] Py：打包发布
来源：http://zzb.epnwcf.com

python -m build  （依赖 pyproject.toml）
来源：http://lpw.yfazqb.com

[U34] Py：判断编码
来源：http://zuj.birdmap.top

chardet.detect(raw)
来源：http://ghc.vqdsnc.cn

[U35] Py：发送邮件
来源：http://odw.jiagoushi.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wls.chenlongwang.top

[U36] Py：定时任务
来源：http://xah.hnxiangtu.top

schedule.every(10).minutes.do(job)
来源：http://qrp.cashguo.top

[U37] Py：读写 Excel
来源：http://tjz.daxiang520.top

pandas.read_excel / DataFrame.to_excel
来源：http://bmy.quarkkingdee.top

[U38] Py：获取脚本所在目录
来源：http://ojg.pengpengdd.cyou

Path(__file__).resolve().parent
来源：http://hov.zhiwuduotai.top

[U39] Py：判断是否在交互环境
来源：http://xvd.zdbjq.cn

sys.stdout.isatty()
来源：http://efa.smart0.xyz

[U40] Py：打印到标准错误
来源：http://nek.sxryk.cn

print("err", file=sys.stderr)
来源：http://gzl.shangyingyoupin.top

[U41] PHP：初始化 Composer 项目
来源：http://lef.tarul.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://eck.bbcook.cn

[U42] PHP：PSR-4 自动加载
来源：http://obf.vehdjk.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zhz.hfpthk.cn

[U43] PHP：声明命名空间
来源：http://wof.cdnleiting.top

namespace App\Http;
来源：http://mop.316326.xyz

[U44] PHP：开启严格类型
来源：http://rgj.cucudq.cn

declare(strict_types=1);
来源：http://dkx.vqdsnc.cn

[U45] PHP：类型声明与返回类型
来源：http://qcp.jqgufenzy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://aqx.0kj1m.cn

[U46] PHP：可空类型
来源：http://wds.havefunace.top

?string $name = null
来源：http://nhq.jinghuilouyu.cn

[U47] PHP：联合类型
来源：http://odc.hysaishi.cn

int|string $id
来源：http://wdb.cashguo.top

[U48] PHP：纯枚举
来源：http://gnj.zhixingplan.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hml.ctjpmb.com

[U49] PHP：只读属性
来源：http://qxq.nanxinkj.top

public readonly string $name
来源：http://zcl.52xcode.cn

[U50] PHP：构造器属性提升
来源：http://utd.wangdashe.top

public function __construct(private int $id) {}
来源：http://qjl.zdqjudy.top

[U51] PHP：数组解构
来源：http://tlg.yuanzhike.top

[$a, $b] = $arr;
来源：http://enc.ydjk.org.cn

[U52] PHP：箭头函数
来源：http://fac.316326.xyz

$double = fn($x) => $x * 2;
来源：http://ebp.hesvh.cn

[U53] PHP：空合并运算符
来源：http://xqa.tian-w.cn

$v = $a ?? $b ?? "default";
来源：http://zuk.xuetiantiany.cn

[U54] PHP：空安全调用
来源：http://inj.jianghu66.top

$obj?->method()
来源：http://ioq.316326.xyz

[U55] PHP：match 表达式
来源：http://tuq.jinyuanbaomall.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://pon.ybcxt.top

[U56] PHP：命名参数
来源：http://qmj.vqdsnc.cn

f(a: 1, b: 2)
来源：http://bku.zhiwuduotai.top

[U57] PHP：字符串插值
来源：http://cwv.hfpthk.cn

"值: {$a}"
来源：http://vvh.0kj1m.cn

[U58] PHP：数组三件套
来源：http://zox.yuxming.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pya.gogol.net.cn

[U59] PHP：自定义排序
来源：http://iau.hammf.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gfo.hywenlv.cn

[U60] PHP：JSON 编解码
来源：http://nuy.316326.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://yet.jinghuilouyu.cn

[U61] PHP：正则
来源：http://wgj.zhoulong.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tet.sjlbkw.cn

[U62] PHP：日期对象
来源：http://vld.sufxvd.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://joy.vehdjk.com

[U63] PHP：文件读写
来源：http://ozc.ivvv.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://oip.hammf.cn

[U64] PHP：目录遍历
来源：http://ldo.meibo888.top

glob("dir/*.php");  scandir("dir");
来源：http://cvd.zhiwuduotai.top

[U65] PHP：会话
来源：http://ahn.dianchejie.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ovs.hysaishi.cn

[U66] PHP：设置 Cookie
来源：http://mbh.aibaodan.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rud.mhx1999.top

[U67] PHP：处理文件上传
来源：http://hjl.hammf.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://aou.feifeiyinyue.top

[U68] PHP：PDO 连接
来源：http://eyv.xuanzx.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ecr.jqgfzy.top

[U69] PHP：PDO 预处理
来源：http://waw.yueranfly.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://pgk.hysaishi.cn

[U70] PHP：PDO 事务
来源：http://ant.hywenlv.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fiu.redwolf501.top

[U71] PHP：抛出异常
来源：http://cnx.ywan-chungtsiang.top

throw new RuntimeException("失败", 500);
来源：http://abw.cdnleiting.top

[U72] PHP：写错误日志
来源：http://yws.yuanzhike.top

error_log("失败: " . $e->getMessage());
来源：http://bdo.c1oappe.top

[U73] PHP：读取 ini 配置
来源：http://eic.xuanzx.com

parse_ini_file("config.ini", true)
来源：http://wqw.ywan-chungtsiang.top

[U74] PHP：读取环境变量
来源：http://rtc.yuanzhike.top

getenv("APP_ENV") ?: "production"
来源：http://kxl.zhongyouzk.top

[U75] PHP：依赖注入
来源：http://snh.jyoumei.cn

composer require psr/container
来源：http://fzr.cqqwz.cn

[U76] PHP：简单路由
来源：http://hqd.yuxming.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kep.chenzaomai.com

[U77] PHP：模板渲染
来源：http://arr.0kj1m.cn

composer require twig/twig
来源：http://kki.ivvv.top

[U78] PHP：单元测试
来源：http://axa.xuetiantiany.cn

composer require --dev phpunit/phpunit
来源：http://iyc.guannengcc.top

[U79] PHP：静态分析
来源：http://cst.hnxiangtu.top

composer require --dev phpstan/phpstan
来源：http://uev.0kj1m.cn

[U80] PHP：代码规范修复
来源：http://oag.chenlongwang.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://wby.uphjek.com

[U81] JS：初始化项目
来源：http://nms.hesvh.cn

npm init -y;  npm i express
来源：http://dah.fehbvm.com

[U82] JS：package.json 脚本
来源：http://xhz.fktsv.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pal.hcnkem.com

[U83] JS：ES Module 导入导出
来源：http://ozu.gogol.net.cn

export const a = 1;  import { a } from "./m.js";
来源：http://gai.xuanzx.com

[U84] JS：CommonJS 写法
来源：http://oru.nanxinkj.top

module.exports = { a };  const { a } = require("./m");
来源：http://ctw.xinyue.icu

[U85] JS：可选链
来源：http://qed.pycfn.com

a?.b?.c
来源：http://csh.smart0.xyz

[U86] JS：空值合并
来源：http://lso.hesvh.cn

a ?? b
来源：http://ezh.fktsv.cn

[U87] JS：解构默认值
来源：http://bud.chenlongwang.top

const { a = 1, b = 2 } = obj;
来源：http://bsv.vehdjk.com

[U88] JS：对象展开合并
来源：http://qqi.hnxiangtu.top

{ ...a, ...b }
来源：http://mpv.sjlbkw.cn

[U89] JS：数组去重
来源：http://fcc.0kj1m.cn

[...new Set(arr)]
来源：http://rlz.fanxiaobao.xyz

[U90] JS：数字数组排序
来源：http://zuz.bbcook.cn

[...arr].sort((a, b) => a - b)
来源：http://asv.nwbrower.top

[U91] JS：对象键值遍历
来源：http://zjj.yj202588.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ftu.yuanzhike.top

[U92] JS：深拷贝
来源：http://dyn.birdmap.top

structuredClone(obj)
来源：http://nod.zdqjudy.top

[U93] JS：模板字符串
来源：http://nwo.pengpengdd.cyou

`共 ${n} 条`
来源：http://qbm.hammf.cn

[U94] JS：箭头函数
来源：http://ttf.vehdjk.com

const double = x => x * 2;
来源：http://yyq.ivvv.top

[U95] JS：Promise 包装
来源：http://gcf.pycfn.com

new Promise((resolve, reject) => {})
来源：http://yam.zhongyouzk.top

[U96] JS：async/await 与异常
来源：http://thn.hnqzz.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jfs.ywan-chungtsiang.top

[U97] JS：并发请求
来源：http://qcg.zycfv.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://clu.yj202588.top

[U98] JS：fetch 带 JSON
来源：http://vgo.birdmap.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fpi.ivvv.top

[U99] JS：事件监听
来源：http://teq.0kj1m.cn

el.addEventListener("click", e => {})
来源：http://itl.yangfankeji.com

[U100] JS：DOM 查询
来源：http://bje.guannengcc.top

document.querySelector(".item")
来源：http://vfw.tian-w.cn

[U101] JS：classList 操作
来源：http://iqn.ppjwa.cn

el.classList.toggle("active")
来源：http://scx.wangshuangyany.cn

[U102] JS：本地存储
来源：http://qvq.nanxuanxn.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://vsy.feifeiyinyue.top

[U103] JS：定时器
来源：http://qnq.zhengqikj.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gfg.yj20258888.top

[U104] JS：防抖
来源：http://tfw.vehdjk.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mdh.jinghuilouyu.cn

[U105] JS：节流
来源：http://ylo.jqgfzy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nfp.shanyushiyangtech.top

[U106] JS：日期格式化
来源：http://ogc.epnwcf.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://efd.xingfuxueyuan.xyz

[U107] JS：数字千分位
来源：http://dpd.yuanzhike.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gwz.svipenyu.cn

[U108] JS：随机整数
来源：http://oty.quarkkingdee.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dpt.iojbl.cn

[U109] JS：数组分组
来源：http://gmc.andypj.xyz

Object.groupBy(arr, x => x.type)
来源：http://vti.andypj.xyz

[U110] JS：数组分块
来源：http://mxv.yj20258888.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pyu.yanxiufei.cn

[U111] JS：对象转 Map
来源：http://aoa.haohaochexian.top

new Map(Object.entries(obj))
来源：http://hsc.andypj.xyz

[U112] JS：字符串补位
来源：http://mgx.xziqi.cn

"7".padStart(3, "0")
来源：http://jtl.ivvv.top

[U113] JS：正则替换全部
来源：http://pvl.havefunace.top

s.replaceAll("a", "b")
来源：http://akt.zhengqikj.top

[U114] JS：JSON 深比较
来源：http://uaq.yfazqb.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://chc.cheryme.top

[U115] JS：生成 UUID
来源：http://esg.yj20258.top

crypto.randomUUID()
来源：http://gxf.cdnleiting.top

[U116] JS：类型检查（JSDoc）
来源：http://jzr.dashuyun.cn

/** @param {string} name */ function f(name) {}
来源：http://sag.ctjpmb.com

[U117] JS：单元测试
来源：http://ode.zhaomingkeji.xyz

npm i -D vitest;  npx vitest
来源：http://zbh.tianlin.xyz

[U118] JS：开发服务器
来源：http://ssf.316326.xyz

npm i -D vite;  npx vite
来源：http://qjk.xylfe.cn

[U119] JS：生产构建
来源：http://weg.zhongyouzk.top

npx vite build
来源：http://bia.shzxlz.cn

[U120] JS：读取环境变量（Vite）
来源：http://gpb.meibo888.top

import.meta.env.VITE_API_URL
来源：http://zwh.hongshengwenyu.top

================================================================================
来源：http://uyw.jqgfzy.top

统计汇总
来源：http://qqr.kuanghao11.cn

================================================================================
来源：http://aub.shuidangran.top

按语言统计（条）：
来源：http://rne.guannengcc.top

Python ......... 252
来源：http://iqo.sufxvd.cn

PHP ............ 252
来源：http://aju.hesvh.cn

JavaScript ..... 252
来源：http://pje.mhx1999.top

TypeScript ..... 212
来源：http://olq.0kj1m.cn

Java ........... 212
来源：http://hhg.fktsv.cn

Go ............. 212
来源：http://jrq.sysykeji.top

Ruby ........... 212
来源：http://tel.zhixingplan.top

C# ............. 212
来源：http://pua.yuanzhike.top

C .............. 30
来源：http://aik.shangyingyoupin.top

C++ ............ 30
来源：http://woe.yuanzhike.top

SQL ............ 90
来源：http://rle.yangfankeji.com

Bash ........... 80
来源：http://awx.xinyue.icu

Kotlin ......... 15
来源：http://tmu.jianghu66.top

Swift .......... 15
来源：http://guc.wangdashe.top

Lua ............ 10
来源：http://gqb.c1oappe.top

Perl ........... 10
来源：http://oib.andypj.xyz

Scala .......... 10
来源：http://fty.daxiang520.top

------------------------------------
来源：http://lkh.tian-w.cn

合计 ........... 2106 条
来源：http://abp.zdbjq.cn

按章节统计：
来源：http://ghh.sjlbkw.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tsj.hnxiangtu.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xfn.aibaodan.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://cew.feifeiyinyue.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ldw.jiagoushi.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bnn.redwolf501.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hck.zhongyouzk.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://oyv.zhoulong.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://uis.yj20258888.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wkc.hongshengwenyu.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xtf.ivvv.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ksj.nanxuanxn.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gbz.316326.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://fvc.chenlongwang.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://fgy.hywenlv.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://lol.zhongyouzk.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ibw.hammf.cn

Q SQL 专题                              90
来源：http://umg.nanxinkj.top

R Bash 专题                             80
来源：http://owa.xingfuxueyuan.xyz

S C / C++ 专题                          60
来源：http://oru.hywenlv.cn

T 其他语言补充                          60
来源：http://tsl.zhongyouzk.top

U 高频实用片段                         120
来源：http://det.birdmap.top

------------------------------------
来源：http://kyq.jiagoushi.top

合计                                  2106 条
来源：http://lxe.iojbl.cn

--------------------------------------------------------------------------------
来源：http://kfc.jinqigfzy.top

使用提醒
来源：http://bzu.sjlbkw.cn

--------------------------------------------------------------------------------
来源：http://zyv.fktsv.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ufs.ybcxt.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xvv.yj20258.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qqc.cheryme.top

在旧版本上使用前请先确认语法支持情况。
来源：http://tnu.hongshengwenyu.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qdy.52xcode.cn

—— 文件结束 ——
来源：http://xlc.sysykeji.top

================================================================================
来源：http://byo.ydjk.org.cn

程序语言常见例子速查手册（2024 版）
来源：http://wui.ctjpmb.com

Common Programming Examples Cheat Book
来源：http://mcb.yvedp.cn

================================================================================
来源：http://uma.shzxlz.cn

【收录内容】
来源：http://qin.hcnkem.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://rcc.jianghu66.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://dii.birdmap.top

SQL · Bash · C · C++
来源：http://vxw.bbcook.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://zwr.jqgufenzy.top

【使用说明】
来源：http://wrp.bjfxy.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://sde.uphjek.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://grr.yanxiufei.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://lvj.zhixingplan.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://usb.yj20258888.top

Bash:  Shell         C:     C             C++:   C++
来源：http://wwx.hongshengwenyu.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://veu.zycfv.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://gnc.bbcook.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://shx.ehwqpu.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lom.zhongyouzk.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://kop.xylfe.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://rnv.jlsjyb.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://dgy.jinqigfzy.top

【文件统计】
来源：http://gdu.yj20258.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ree.cashguo.top

--------------------------------------------------------------------------------
来源：http://xwu.52xcode.cn

目  录
来源：http://nmv.shanyushiyangtech.top

--------------------------------------------------------------------------------
来源：http://ntw.chenlongwang.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://whn.yfazqb.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://daq.jlsjyb.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://yjs.sweek.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://bkd.9152youxi.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://fml.shanyushiyangtech.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gzt.dianchejie.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ngf.zhongyouzk.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://woj.yonumen.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wot.ydjk.org.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://rqe.fehbvm.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://jfe.52xcode.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xrf.quarkkingdee.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://atk.ywan-chungtsiang.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zbs.gaohongyu789.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mny.yj20258888.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://nmp.cqqwz.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ywe.ivvv.top


<!-- 参考信息 -->