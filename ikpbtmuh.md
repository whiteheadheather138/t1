代发 wailian999

[U19] Py：正则替换带回调
来源：http://exr.yvedp.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lyd.chenzaomai.com

[U20] Py：缓存函数结果
来源：http://kxu.52xcode.cn

@functools.lru_cache(maxsize=None)
来源：http://hve.cheryme.top

[U21] Py：自定义上下文管理器
来源：http://tiz.zhaomingkeji.xyz

@contextlib.contextmanager
来源：http://zbv.sxryk.cn

[U22] Py：矩阵转置
来源：http://eqd.vehdjk.com

list(zip(*m))
来源：http://vkl.iojbl.cn

[U23] Py：分块读取大文件
来源：http://ydv.fzhhl.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bme.pengpengdd.cyou

[U24] Py：路径操作
来源：http://xwr.guowangkeji.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dpf.xylfe.cn

[U25] Py：CSV 按字典读
来源：http://dtz.tanke756.top

csv.DictReader(f)
来源：http://pfa.zhaomingkeji.xyz

[U26] Py：并发下载
来源：http://bzv.ctjpmb.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gbw.xziqi.cn

[U27] Py：异步 HTTP
来源：http://oin.hywenlv.cn

aiohttp.ClientSession() 配合 async with
来源：http://quw.nanxinkj.top

[U28] Py：类型别名
来源：http://lhk.redwolf501.top

UserId = int
来源：http://epy.hongshengwenyu.top

[U29] Py：属性校验
来源：http://mff.mhx1999.top

@property 与 @x.setter 配合
来源：http://vxk.nanxuanxn.top

[U30] Py：数据类
来源：http://bft.hywenlv.cn

@dataclass(slots=True)
来源：http://bln.snrcjt.cn

[U31] Py：单测
来源：http://mqq.svipenyu.cn

python -m pytest -q
来源：http://eel.haohaochexian.top

[U32] Py：代码格式化
来源：http://fvy.redwolf501.top

ruff format . && ruff check --fix .
来源：http://xkn.52xcode.cn

[U33] Py：打包发布
来源：http://cjv.hnxiangtu.top

python -m build  （依赖 pyproject.toml）
来源：http://nuy.uphjek.com

[U34] Py：判断编码
来源：http://hkn.dianchejie.cn

chardet.detect(raw)
来源：http://gsb.chenzaomai.com

[U35] Py：发送邮件
来源：http://guo.cucudq.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://owz.uphjek.com

[U36] Py：定时任务
来源：http://eun.jianghu66.top

schedule.every(10).minutes.do(job)
来源：http://cnd.tian-w.cn

[U37] Py：读写 Excel
来源：http://rpt.sjlbkw.cn

pandas.read_excel / DataFrame.to_excel
来源：http://xrs.fengsongda.top

[U38] Py：获取脚本所在目录
来源：http://gnk.zhoulong.xyz

Path(__file__).resolve().parent
来源：http://vog.fengsongda.top

[U39] Py：判断是否在交互环境
来源：http://gfp.fengsongda.top

sys.stdout.isatty()
来源：http://eqt.jlsjyb.cn

[U40] Py：打印到标准错误
来源：http://xvu.yonumen.top

print("err", file=sys.stderr)
来源：http://pzl.hnqzz.top

[U41] PHP：初始化 Composer 项目
来源：http://qdu.316326.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://ylo.0kj1m.cn

[U42] PHP：PSR-4 自动加载
来源：http://nam.aizwys.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zfl.quarkkingdee.top

[U43] PHP：声明命名空间
来源：http://uzo.9152youxi.cn

namespace App\Http;
来源：http://bdt.daxiang520.top

[U44] PHP：开启严格类型
来源：http://aaw.52xcode.cn

declare(strict_types=1);
来源：http://rqg.sufxvd.cn

[U45] PHP：类型声明与返回类型
来源：http://xdr.ehwqpu.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://fvb.wangdashe.top

[U46] PHP：可空类型
来源：http://hxw.jianghu66.top

?string $name = null
来源：http://okm.xuanzx.com

[U47] PHP：联合类型
来源：http://uoy.tanke756.top

int|string $id
来源：http://noz.bbcook.cn

[U48] PHP：纯枚举
来源：http://vea.xziqi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rea.vqdsnc.cn

[U49] PHP：只读属性
来源：http://mxp.cdnleiting.top

public readonly string $name
来源：http://lue.sjlbkw.cn

[U50] PHP：构造器属性提升
来源：http://nam.fehbvm.com

public function __construct(private int $id) {}
来源：http://lcd.zhongyouzk.top

[U51] PHP：数组解构
来源：http://gng.feifeiyinyue.top

[$a, $b] = $arr;
来源：http://jsg.ywan-chungtsiang.top

[U52] PHP：箭头函数
来源：http://ont.jiagoushi.top

$double = fn($x) => $x * 2;
来源：http://zab.52xcode.cn

[U53] PHP：空合并运算符
来源：http://jsb.birdmap.top

$v = $a ?? $b ?? "default";
来源：http://nyj.ctjpmb.com

[U54] PHP：空安全调用
来源：http://aoo.hongshengwenyu.top

$obj?->method()
来源：http://onf.jyoumei.cn

[U55] PHP：match 表达式
来源：http://ltv.quarkkingdee.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rhh.dashuyun.cn

[U56] PHP：命名参数
来源：http://ynt.fehbvm.com

f(a: 1, b: 2)
来源：http://upe.andypj.xyz

[U57] PHP：字符串插值
来源：http://gkn.cheryme.top

"值: {$a}"
来源：http://tkx.pycfn.com

[U58] PHP：数组三件套
来源：http://yxw.fktsv.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bao.jinghuilouyu.cn

[U59] PHP：自定义排序
来源：http://ypn.xinyue.icu

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://drd.havefunace.top

[U60] PHP：JSON 编解码
来源：http://yjq.gaohongyu789.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cle.xylfe.cn

[U61] PHP：正则
来源：http://rjc.zdqjudy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://goa.wangshuangyany.cn

[U62] PHP：日期对象
来源：http://zkh.vehdjk.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hph.bbcook.cn

[U63] PHP：文件读写
来源：http://rau.ywan-chungtsiang.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mjh.hnxiangtu.top

[U64] PHP：目录遍历
来源：http://blm.pengpengdd.cyou

glob("dir/*.php");  scandir("dir");
来源：http://fam.yangfankeji.com

[U65] PHP：会话
来源：http://tmq.shanyushiyangkeji.top

session_start();  $_SESSION["uid"] = 1;
来源：http://rkg.hysaishi.cn

[U66] PHP：设置 Cookie
来源：http://ppu.aibaodan.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fkg.gaohongyu789.top

[U67] PHP：处理文件上传
来源：http://iuv.nwbrower.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bef.316326.xyz

[U68] PHP：PDO 连接
来源：http://dny.jinyuanbaomall.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vym.bbcook.cn

[U69] PHP：PDO 预处理
来源：http://trx.meibo888.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gqy.haohaochexian.top

[U70] PHP：PDO 事务
来源：http://eji.shanyushiyangtech.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lmz.ctjpmb.com

[U71] PHP：抛出异常
来源：http://irk.meibo888.top

throw new RuntimeException("失败", 500);
来源：http://snq.jinqigfzy.top

[U72] PHP：写错误日志
来源：http://vfn.smart0.xyz

error_log("失败: " . $e->getMessage());
来源：http://hcz.yanxiufei.cn

[U73] PHP：读取 ini 配置
来源：http://dom.jyoumei.cn

parse_ini_file("config.ini", true)
来源：http://med.316326.xyz

[U74] PHP：读取环境变量
来源：http://ins.zdbjq.cn

getenv("APP_ENV") ?: "production"
来源：http://qgm.tarul.cn

[U75] PHP：依赖注入
来源：http://ykk.aibaodan.cn

composer require psr/container
来源：http://dkf.guowangkeji.top

[U76] PHP：简单路由
来源：http://vxf.haohaochexian.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://quf.fzhhl.top

[U77] PHP：模板渲染
来源：http://sxr.jiagoushi.top

composer require twig/twig
来源：http://vaa.yanxiufei.cn

[U78] PHP：单元测试
来源：http://bqt.shangyingyoupin.top

composer require --dev phpunit/phpunit
来源：http://fvc.nwbrower.top

[U79] PHP：静态分析
来源：http://mvs.aizwys.cn

composer require --dev phpstan/phpstan
来源：http://wdj.cqqwz.cn

[U80] PHP：代码规范修复
来源：http://qos.yj20258.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://nfn.shanyushiyangkeji.top

[U81] JS：初始化项目
来源：http://kdx.guowangkeji.top

npm init -y;  npm i express
来源：http://saf.wangdashe.top

[U82] JS：package.json 脚本
来源：http://hts.52xcode.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zuw.yangfankeji.com

[U83] JS：ES Module 导入导出
来源：http://daz.yuxming.cn

export const a = 1;  import { a } from "./m.js";
来源：http://yzl.chenjidiqi.icu

[U84] JS：CommonJS 写法
来源：http://fcf.jlsjyb.cn

module.exports = { a };  const { a } = require("./m");
来源：http://igm.hnxiangtu.top

[U85] JS：可选链
来源：http://cbw.nanxinkj.top

a?.b?.c
来源：http://jmb.chenzaomai.com

[U86] JS：空值合并
来源：http://hmf.jyoumei.cn

a ?? b
来源：http://rmg.tian-w.cn

[U87] JS：解构默认值
来源：http://cak.yueranfly.top

const { a = 1, b = 2 } = obj;
来源：http://tjr.daxiang520.top

[U88] JS：对象展开合并
来源：http://irc.bbcook.cn

{ ...a, ...b }
来源：http://ehx.cashguo.top

[U89] JS：数组去重
来源：http://qam.pengpengdd.cyou

[...new Set(arr)]
来源：http://tyh.uphjek.com

[U90] JS：数字数组排序
来源：http://fvz.ydzc1.top

[...arr].sort((a, b) => a - b)
来源：http://lhj.zhongyouzk.top

[U91] JS：对象键值遍历
来源：http://mbt.gogol.net.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://yog.tanke756.top

[U92] JS：深拷贝
来源：http://pam.guowangkeji.top

structuredClone(obj)
来源：http://jbz.uphjek.com

[U93] JS：模板字符串
来源：http://yls.birdmap.top

`共 ${n} 条`
来源：http://tbb.ybcxt.top

[U94] JS：箭头函数
来源：http://eop.smart0.xyz

const double = x => x * 2;
来源：http://pub.redwolf501.top

[U95] JS：Promise 包装
来源：http://tss.tian-w.cn

new Promise((resolve, reject) => {})
来源：http://qqk.quarkkingdee.top

[U96] JS：async/await 与异常
来源：http://srz.xylfe.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cpc.hfpthk.cn

[U97] JS：并发请求
来源：http://ryx.smart0.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://kwk.xinyue.icu

[U98] JS：fetch 带 JSON
来源：http://fqh.quarkkingdee.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zcv.gaohongyu789.top

[U99] JS：事件监听
来源：http://qac.hnqzz.top

el.addEventListener("click", e => {})
来源：http://dou.zhongyouzk.top

[U100] JS：DOM 查询
来源：http://xxn.ydjk.org.cn

document.querySelector(".item")
来源：http://dnf.vehdjk.com

[U101] JS：classList 操作
来源：http://rkw.tianlin.xyz

el.classList.toggle("active")
来源：http://usw.iojbl.cn

[U102] JS：本地存储
来源：http://ifj.tanke756.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://vjt.hcnkem.com

[U103] JS：定时器
来源：http://hws.cheryme.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jin.redwolf501.top

[U104] JS：防抖
来源：http://lds.zdbjq.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://csq.vehdjk.com

[U105] JS：节流
来源：http://vnp.nanxinkj.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://duc.hnxiangtu.top

[U106] JS：日期格式化
来源：http://ruq.yanxiufei.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yig.hcnkem.com

[U107] JS：数字千分位
来源：http://eol.jyoumei.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ymt.snrcjt.cn

[U108] JS：随机整数
来源：http://jmd.jinghuilouyu.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qnw.mhx1999.top

[U109] JS：数组分组
来源：http://yfy.hcnkem.com

Object.groupBy(arr, x => x.type)
来源：http://pvk.ivvv.top

[U110] JS：数组分块
来源：http://hqd.hammf.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pry.hywenlv.cn

[U111] JS：对象转 Map
来源：http://mux.zhengqikj.top

new Map(Object.entries(obj))
来源：http://fzt.aizwys.cn

[U112] JS：字符串补位
来源：http://ukq.zhengqikj.top

"7".padStart(3, "0")
来源：http://ism.ywan-chungtsiang.top

[U113] JS：正则替换全部
来源：http://dmh.hnxiangtu.top

s.replaceAll("a", "b")
来源：http://zst.jinqigfzy.top

[U114] JS：JSON 深比较
来源：http://sjq.shangyingyoupin.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://axl.hysaishi.cn

[U115] JS：生成 UUID
来源：http://zmz.jqgfzy.top

crypto.randomUUID()
来源：http://qwv.xinyue.icu

[U116] JS：类型检查（JSDoc）
来源：http://qfl.yuxming.cn

/** @param {string} name */ function f(name) {}
来源：http://plb.yj20258.top

[U117] JS：单元测试
来源：http://kcd.cucudq.cn

npm i -D vitest;  npx vitest
来源：http://ijv.fanxiaobao.xyz

[U118] JS：开发服务器
来源：http://zoi.sufxvd.cn

npm i -D vite;  npx vite
来源：http://edg.nwbrower.top

[U119] JS：生产构建
来源：http://zog.shangyingyoupin.top

npx vite build
来源：http://ezj.pengpengdd.cyou

[U120] JS：读取环境变量（Vite）
来源：http://iqp.9152youxi.cn

import.meta.env.VITE_API_URL
来源：http://xpk.shangyingyoupin.top

================================================================================
来源：http://ozm.jinyuanbaomall.cn

统计汇总
来源：http://vrz.shangyingyoupin.top

================================================================================
来源：http://vbr.ppjwa.cn

按语言统计（条）：
来源：http://rbh.jyoumei.cn

Python ......... 252
来源：http://jjs.chenzaomai.com

PHP ............ 252
来源：http://aia.xylfe.cn

JavaScript ..... 252
来源：http://kkq.ybcxt.top

TypeScript ..... 212
来源：http://car.quarkkingdee.top

Java ........... 212
来源：http://rhd.c1oappe.top

Go ............. 212
来源：http://zlq.hnqzz.top

Ruby ........... 212
来源：http://qrd.yonumen.top

C# ............. 212
来源：http://kmb.dianchejie.cn

C .............. 30
来源：http://otj.nanxinkj.top

C++ ............ 30
来源：http://uls.tian-w.cn

SQL ............ 90
来源：http://fqc.mhx1999.top

Bash ........... 80
来源：http://uan.zhaomingkeji.xyz

Kotlin ......... 15
来源：http://kqj.ehwqpu.com

Swift .......... 15
来源：http://uof.xingfuxueyuan.xyz

Lua ............ 10
来源：http://hua.ctjpmb.com

Perl ........... 10
来源：http://kvh.havefunace.top

Scala .......... 10
来源：http://gen.zhixingplan.top

------------------------------------
来源：http://jud.chenjidiqi.icu

合计 ........... 2106 条
来源：http://tcz.bjfxy.top

按章节统计：
来源：http://pnc.yfazqb.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dub.yj202588.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://shv.svipenyu.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://boc.tian-w.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://scr.0kj1m.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hut.xuetiantiany.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ydw.ehwqpu.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://gvz.hywenlv.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zrd.zhoulong.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hho.shanyushiyangtech.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rmc.c1oappe.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://nyb.zhengqikj.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hzd.fzhhl.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qja.gogol.net.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://pfk.bbcook.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://isd.ydjk.org.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://idj.fehbvm.com

Q SQL 专题                              90
来源：http://eaj.c1oappe.top

R Bash 专题                             80
来源：http://ggm.yueranfly.top

S C / C++ 专题                          60
来源：http://ffx.nanxinkj.top

T 其他语言补充                          60
来源：http://vge.tarul.cn

U 高频实用片段                         120
来源：http://bdj.gaohongyu789.top

------------------------------------
来源：http://ngy.shanyushiyangkeji.top

合计                                  2106 条
来源：http://rtm.havefunace.top

--------------------------------------------------------------------------------
来源：http://kwp.svipenyu.cn

使用提醒
来源：http://heb.hnqzz.top

--------------------------------------------------------------------------------
来源：http://suk.zdbjq.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://pmm.bbcook.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mgp.mhx1999.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://cog.ybcxt.top

在旧版本上使用前请先确认语法支持情况。
来源：http://qgl.c1oappe.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://dwi.jinqigufen.top

—— 文件结束 ——
来源：http://kdd.zycfv.cn

================================================================================
来源：http://ulv.jinyuanbaomall.cn

程序语言常见例子速查手册（2024 版）
来源：http://zjk.aibaodan.cn

Common Programming Examples Cheat Book
来源：http://ike.yongpay.top

================================================================================
来源：http://zzz.yuxming.cn

【收录内容】
来源：http://slq.smart0.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://qqx.zhijiandao.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://cmq.316326.xyz

SQL · Bash · C · C++
来源：http://fmt.nanxuanxn.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://uhy.sxryk.cn

【使用说明】
来源：http://xrz.zhongyouzk.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://tkg.gogol.net.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://jwt.svipenyu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://awz.jiagoushi.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qeh.tanke756.top

Bash:  Shell         C:     C             C++:   C++
来源：http://twv.fktsv.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mup.zhengqikj.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://dne.yuanzhike.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://siv.quarkkingdee.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://kiw.epnwcf.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ywz.pycfn.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://gez.haohaochexian.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://tbb.daria6918.cn

【文件统计】
来源：http://xzk.zhixingplan.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rrc.vehdjk.com

--------------------------------------------------------------------------------
来源：http://dlt.jqgufenzy.top

目  录
来源：http://vbw.yj20258.top

--------------------------------------------------------------------------------
来源：http://utk.ybcxt.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://rgf.xingfuxueyuan.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://edf.jiagoushi.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://dwj.shangyingyoupin.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://uky.yueranfly.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://yup.jianghu66.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://laf.haohaochexian.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mdr.feifeiyinyue.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://equ.316326.xyz

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zsb.yfazqb.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://rcj.tianlin.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://dsj.xinyue.icu

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://flt.hcnkem.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://cga.meibo888.top


<!-- 参考信息 -->