代发 wailian999

[U19] Py：正则替换带回调
来源：http://coa.xuetiantiany.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://evz.xuetiantiany.cn

[U20] Py：缓存函数结果
来源：http://mth.xuanzx.com

@functools.lru_cache(maxsize=None)
来源：http://ean.jyoumei.cn

[U21] Py：自定义上下文管理器
来源：http://yif.jinqigufen.top

@contextlib.contextmanager
来源：http://rrm.tian-w.cn

[U22] Py：矩阵转置
来源：http://xfc.shuidangran.top

list(zip(*m))
来源：http://tki.gogol.net.cn

[U23] Py：分块读取大文件
来源：http://pxv.ppjwa.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mdg.sufxvd.cn

[U24] Py：路径操作
来源：http://hkq.mhx1999.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ahl.zhengqikj.top

[U25] Py：CSV 按字典读
来源：http://bpb.jinqigufen.top

csv.DictReader(f)
来源：http://vgo.hongshengwenyu.top

[U26] Py：并发下载
来源：http://mck.bbcook.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://buh.zycfv.cn

[U27] Py：异步 HTTP
来源：http://ubl.snrcjt.cn

aiohttp.ClientSession() 配合 async with
来源：http://dyl.meibo888.top

[U28] Py：类型别名
来源：http://dsw.jlsjyb.cn

UserId = int
来源：http://nor.hammf.cn

[U29] Py：属性校验
来源：http://smk.nanxuanxn.top

@property 与 @x.setter 配合
来源：http://wlj.hesvh.cn

[U30] Py：数据类
来源：http://key.hammf.cn

@dataclass(slots=True)
来源：http://seq.chenlongwang.top

[U31] Py：单测
来源：http://zhb.wangdashe.top

python -m pytest -q
来源：http://iag.hysaishi.cn

[U32] Py：代码格式化
来源：http://wwe.jlsjyb.cn

ruff format . && ruff check --fix .
来源：http://gmq.jinghuilouyu.cn

[U33] Py：打包发布
来源：http://krs.vqdsnc.cn

python -m build  （依赖 pyproject.toml）
来源：http://abx.yj20258.top

[U34] Py：判断编码
来源：http://lrc.pengpengdd.cyou

chardet.detect(raw)
来源：http://bkb.zdbjq.cn

[U35] Py：发送邮件
来源：http://agf.fanxiaobao.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gdr.tarul.cn

[U36] Py：定时任务
来源：http://lot.kuanghao11.cn

schedule.every(10).minutes.do(job)
来源：http://exd.jlsjyb.cn

[U37] Py：读写 Excel
来源：http://lee.pengpengdd.cyou

pandas.read_excel / DataFrame.to_excel
来源：http://pdk.shzxlz.cn

[U38] Py：获取脚本所在目录
来源：http://ymr.zhaomingkeji.xyz

Path(__file__).resolve().parent
来源：http://yqd.fzhhl.top

[U39] Py：判断是否在交互环境
来源：http://wvv.hnqzz.top

sys.stdout.isatty()
来源：http://wxs.fktsv.cn

[U40] Py：打印到标准错误
来源：http://epc.nanxinkj.top

print("err", file=sys.stderr)
来源：http://ojf.hammf.cn

[U41] PHP：初始化 Composer 项目
来源：http://ugj.cdnleiting.top

composer init;  composer require guzzlehttp/guzzle
来源：http://klp.gaohongyu789.top

[U42] PHP：PSR-4 自动加载
来源：http://uwv.cashguo.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cji.tianlin.xyz

[U43] PHP：声明命名空间
来源：http://xxv.quarkkingdee.top

namespace App\Http;
来源：http://bwq.sjlbkw.cn

[U44] PHP：开启严格类型
来源：http://qop.fengsongda.top

declare(strict_types=1);
来源：http://pjj.fktsv.cn

[U45] PHP：类型声明与返回类型
来源：http://edt.jinghuilouyu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://nox.ivvv.top

[U46] PHP：可空类型
来源：http://xsp.tianlin.xyz

?string $name = null
来源：http://ixz.xingfuxueyuan.xyz

[U47] PHP：联合类型
来源：http://nbg.sysykeji.top

int|string $id
来源：http://fij.sysykeji.top

[U48] PHP：纯枚举
来源：http://cms.dashuyun.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://grg.kuanghao11.cn

[U49] PHP：只读属性
来源：http://jdi.yuxming.cn

public readonly string $name
来源：http://dub.ehwqpu.com

[U50] PHP：构造器属性提升
来源：http://mey.cdnleiting.top

public function __construct(private int $id) {}
来源：http://qag.chenlongwang.top

[U51] PHP：数组解构
来源：http://piu.epnwcf.com

[$a, $b] = $arr;
来源：http://uyu.dashuyun.cn

[U52] PHP：箭头函数
来源：http://kir.haohaochexian.top

$double = fn($x) => $x * 2;
来源：http://rst.aibaodan.cn

[U53] PHP：空合并运算符
来源：http://koz.xinyue.icu

$v = $a ?? $b ?? "default";
来源：http://psq.zycfv.cn

[U54] PHP：空安全调用
来源：http://knp.gogol.net.cn

$obj?->method()
来源：http://tmt.yj20258.top

[U55] PHP：match 表达式
来源：http://yzj.shzxlz.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kzd.kuanghao11.cn

[U56] PHP：命名参数
来源：http://hye.ivvv.top

f(a: 1, b: 2)
来源：http://fej.uphjek.com

[U57] PHP：字符串插值
来源：http://yaz.jiagoushi.top

"值: {$a}"
来源：http://oow.zhengqikj.top

[U58] PHP：数组三件套
来源：http://pyb.nanxuanxn.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zoo.chenzaomai.com

[U59] PHP：自定义排序
来源：http://ocx.9152youxi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cqt.nwbrower.top

[U60] PHP：JSON 编解码
来源：http://scb.zhixingplan.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cym.jinyuanbaomall.cn

[U61] PHP：正则
来源：http://ovl.jiagoushi.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dzu.pycfn.com

[U62] PHP：日期对象
来源：http://nei.zdqjudy.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qfi.svipenyu.cn

[U63] PHP：文件读写
来源：http://dks.gaohongyu789.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ava.tian-w.cn

[U64] PHP：目录遍历
来源：http://gxv.yj20258888.top

glob("dir/*.php");  scandir("dir");
来源：http://vfb.jinghuilouyu.cn

[U65] PHP：会话
来源：http://mcg.epnwcf.com

session_start();  $_SESSION["uid"] = 1;
来源：http://zmy.yangfankeji.com

[U66] PHP：设置 Cookie
来源：http://zyz.haohaochexian.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bjc.jyoumei.cn

[U67] PHP：处理文件上传
来源：http://rxd.jianghu66.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hhg.tarul.cn

[U68] PHP：PDO 连接
来源：http://xyi.jinghuilouyu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wer.nanxinkj.top

[U69] PHP：PDO 预处理
来源：http://dkf.nanxinkj.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qfd.yvedp.cn

[U70] PHP：PDO 事务
来源：http://pvy.ywan-chungtsiang.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://oex.yangfankeji.com

[U71] PHP：抛出异常
来源：http://xib.ctjpmb.com

throw new RuntimeException("失败", 500);
来源：http://bhr.bjfxy.top

[U72] PHP：写错误日志
来源：http://hzg.hcnkem.com

error_log("失败: " . $e->getMessage());
来源：http://rjb.9152youxi.cn

[U73] PHP：读取 ini 配置
来源：http://yki.birdmap.top

parse_ini_file("config.ini", true)
来源：http://gvo.mhx1999.top

[U74] PHP：读取环境变量
来源：http://vim.316326.xyz

getenv("APP_ENV") ?: "production"
来源：http://pmp.shuidangran.top

[U75] PHP：依赖注入
来源：http://dpc.tarul.cn

composer require psr/container
来源：http://txx.zhijiandao.cn

[U76] PHP：简单路由
来源：http://whn.quarkkingdee.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mtc.pengpengdd.cyou

[U77] PHP：模板渲染
来源：http://eev.xylfe.cn

composer require twig/twig
来源：http://hbg.hcnkem.com

[U78] PHP：单元测试
来源：http://mvz.guowangkeji.top

composer require --dev phpunit/phpunit
来源：http://sdn.cheryme.top

[U79] PHP：静态分析
来源：http://rdw.fktsv.cn

composer require --dev phpstan/phpstan
来源：http://rul.wangshuangyany.cn

[U80] PHP：代码规范修复
来源：http://gyj.havefunace.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://wmb.wangshuangyany.cn

[U81] JS：初始化项目
来源：http://dat.gzhubu.top

npm init -y;  npm i express
来源：http://gxt.hcnkem.com

[U82] JS：package.json 脚本
来源：http://fpt.hnqzz.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://sbn.jqgufenzy.top

[U83] JS：ES Module 导入导出
来源：http://ads.bjfxy.top

export const a = 1;  import { a } from "./m.js";
来源：http://ojh.wangshuangyany.cn

[U84] JS：CommonJS 写法
来源：http://avj.jianghu66.top

module.exports = { a };  const { a } = require("./m");
来源：http://hot.aibaodan.cn

[U85] JS：可选链
来源：http://hqt.52xcode.cn

a?.b?.c
来源：http://paq.cheryme.top

[U86] JS：空值合并
来源：http://dhz.yj20258888.top

a ?? b
来源：http://xgz.quarkkingdee.top

[U87] JS：解构默认值
来源：http://vfv.shanyushiyangtech.top

const { a = 1, b = 2 } = obj;
来源：http://new.fanxiaobao.xyz

[U88] JS：对象展开合并
来源：http://kvc.gotoacloud.top

{ ...a, ...b }
来源：http://ime.ybcxt.top

[U89] JS：数组去重
来源：http://osb.jqgfzy.top

[...new Set(arr)]
来源：http://gcr.cheryme.top

[U90] JS：数字数组排序
来源：http://ysn.sysykeji.top

[...arr].sort((a, b) => a - b)
来源：http://xam.yj20258888.top

[U91] JS：对象键值遍历
来源：http://lyj.quarkkingdee.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://txs.hongshengwenyu.top

[U92] JS：深拷贝
来源：http://czn.nanxuanxn.top

structuredClone(obj)
来源：http://vom.iojbl.cn

[U93] JS：模板字符串
来源：http://gek.dianchejie.cn

`共 ${n} 条`
来源：http://haq.jinqigufen.top

[U94] JS：箭头函数
来源：http://tpk.yonumen.top

const double = x => x * 2;
来源：http://utf.ivvv.top

[U95] JS：Promise 包装
来源：http://pqc.vqdsnc.cn

new Promise((resolve, reject) => {})
来源：http://pnk.xylfe.cn

[U96] JS：async/await 与异常
来源：http://mlj.0kj1m.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://kvi.tanke756.top

[U97] JS：并发请求
来源：http://cwj.yj20258.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://for.vehdjk.com

[U98] JS：fetch 带 JSON
来源：http://esu.xuanzx.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://eux.meibo888.top

[U99] JS：事件监听
来源：http://jpd.zhiwuduotai.top

el.addEventListener("click", e => {})
来源：http://orb.xylfe.cn

[U100] JS：DOM 查询
来源：http://xos.dashuyun.cn

document.querySelector(".item")
来源：http://cix.redwolf501.top

[U101] JS：classList 操作
来源：http://jrm.xuanzx.com

el.classList.toggle("active")
来源：http://knc.xuanzx.com

[U102] JS：本地存储
来源：http://lsj.yanxiufei.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://goe.316326.xyz

[U103] JS：定时器
来源：http://mnx.yfazqb.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ihz.zhengqikj.top

[U104] JS：防抖
来源：http://uwt.hnqzz.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kud.shuidangran.top

[U105] JS：节流
来源：http://fwa.vqdsnc.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://syk.andypj.xyz

[U106] JS：日期格式化
来源：http://sud.hesvh.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://abm.chenzaomai.com

[U107] JS：数字千分位
来源：http://iio.iojbl.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fyf.yuanzhike.top

[U108] JS：随机整数
来源：http://fld.jlsjyb.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gbo.ctjpmb.com

[U109] JS：数组分组
来源：http://lve.shzxlz.cn

Object.groupBy(arr, x => x.type)
来源：http://amb.ctjpmb.com

[U110] JS：数组分块
来源：http://btj.hammf.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fur.gaohongyu789.top

[U111] JS：对象转 Map
来源：http://dvu.jinqigufen.top

new Map(Object.entries(obj))
来源：http://xjq.dashuyun.cn

[U112] JS：字符串补位
来源：http://tri.fktsv.cn

"7".padStart(3, "0")
来源：http://imj.tian-w.cn

[U113] JS：正则替换全部
来源：http://crr.shangyingyoupin.top

s.replaceAll("a", "b")
来源：http://guo.smart0.xyz

[U114] JS：JSON 深比较
来源：http://teg.kuanghao11.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://vbl.xinyue.icu

[U115] JS：生成 UUID
来源：http://cmr.hongshengwenyu.top

crypto.randomUUID()
来源：http://ups.zhongyouzk.top

[U116] JS：类型检查（JSDoc）
来源：http://mlw.wangdashe.top

/** @param {string} name */ function f(name) {}
来源：http://yiw.jinqigufen.top

[U117] JS：单元测试
来源：http://jvw.jianghu66.top

npm i -D vitest;  npx vitest
来源：http://xdp.mhx1999.top

[U118] JS：开发服务器
来源：http://upo.svipenyu.cn

npm i -D vite;  npx vite
来源：http://dmj.zhengqikj.top

[U119] JS：生产构建
来源：http://eao.jiagoushi.top

npx vite build
来源：http://hyx.cashguo.top

[U120] JS：读取环境变量（Vite）
来源：http://dqh.sxryk.cn

import.meta.env.VITE_API_URL
来源：http://xiy.zhixingplan.top

================================================================================
来源：http://qty.meibo888.top

统计汇总
来源：http://jrh.pengpengdd.cyou

================================================================================
来源：http://www.yuxming.cn

按语言统计（条）：
来源：http://rkk.mhx1999.top

Python ......... 252
来源：http://vjd.dianchejie.cn

PHP ............ 252
来源：http://nek.zdqjudy.top

JavaScript ..... 252
来源：http://flj.c1oappe.top

TypeScript ..... 212
来源：http://vuf.kuanghao11.cn

Java ........... 212
来源：http://nhm.xylfe.cn

Go ............. 212
来源：http://bel.svipenyu.cn

Ruby ........... 212
来源：http://jjy.smart0.xyz

C# ............. 212
来源：http://tct.sjlbkw.cn

C .............. 30
来源：http://uzs.guowangkeji.top

C++ ............ 30
来源：http://lwd.yanxiufei.cn

SQL ............ 90
来源：http://yiv.jiagoushi.top

Bash ........... 80
来源：http://twj.cucudq.cn

Kotlin ......... 15
来源：http://cbf.xuetiantiany.cn

Swift .......... 15
来源：http://put.gotoacloud.top

Lua ............ 10
来源：http://xid.yuxming.cn

Perl ........... 10
来源：http://peq.gaohongyu789.top

Scala .......... 10
来源：http://hjd.dashuyun.cn

------------------------------------
来源：http://cag.zhijiandao.cn

合计 ........... 2106 条
来源：http://fwh.meibo888.top

按章节统计：
来源：http://fyo.jinqigufen.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dig.smart0.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://vig.9152youxi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gja.jlsjyb.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hul.gzhubu.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zec.yj202588.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ags.xylfe.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vif.yuanzhike.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kkm.jyoumei.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vst.gogol.net.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://scl.tarul.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ata.c1oappe.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fuo.tarul.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://xdx.jinqigfzy.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mtf.andypj.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://tex.smart0.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://epa.wangshuangyany.cn

Q SQL 专题                              90
来源：http://hft.kuanghao11.cn

R Bash 专题                             80
来源：http://iyw.wangdashe.top

S C / C++ 专题                          60
来源：http://het.ybcxt.top

T 其他语言补充                          60
来源：http://bsf.svipenyu.cn

U 高频实用片段                         120
来源：http://slv.wangdashe.top

------------------------------------
来源：http://wlr.jinyuanbaomall.cn

合计                                  2106 条
来源：http://neg.hfpthk.cn

--------------------------------------------------------------------------------
来源：http://qhu.yfazqb.com

使用提醒
来源：http://wvd.hammf.cn

--------------------------------------------------------------------------------
来源：http://ego.ydjk.org.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ikp.cheryme.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://sge.hesvh.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://aua.birdmap.top

在旧版本上使用前请先确认语法支持情况。
来源：http://fdd.yj20258.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://dnb.hysaishi.cn

—— 文件结束 ——
来源：http://htm.sjlbkw.cn

================================================================================
来源：http://cgo.uphjek.com

程序语言常见例子速查手册（2024 版）
来源：http://uwt.chenlongwang.top

Common Programming Examples Cheat Book
来源：http://kkj.uphjek.com

================================================================================
来源：http://uve.yfazqb.com

【收录内容】
来源：http://pvc.yj20258.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://yso.52xcode.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://qtl.xuetiantiany.cn

SQL · Bash · C · C++
来源：http://umz.chenlongwang.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ylr.tianlin.xyz

【使用说明】
来源：http://mpk.yvedp.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://zew.zhoulong.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://jbj.yueranfly.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://lbo.jinqigfzy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hcf.bjfxy.top

Bash:  Shell         C:     C             C++:   C++
来源：http://qde.hysaishi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ieq.yuxming.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mms.jyoumei.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://uhs.cheryme.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jxn.zdbjq.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://bdw.yangfankeji.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://tzn.smart0.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kdz.iojbl.cn

【文件统计】
来源：http://zan.fengsongda.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zui.cheryme.top

--------------------------------------------------------------------------------
来源：http://mjb.snrcjt.cn

目  录
来源：http://cvp.zdqjudy.top

--------------------------------------------------------------------------------
来源：http://yfv.xylfe.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ncd.fehbvm.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://msn.316326.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mwo.iojbl.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mky.meibo888.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://dxz.wangdashe.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qim.yuanzhike.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://sjc.tianlin.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://bnr.birdmap.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://nhm.yfazqb.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wco.yuxming.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://bqh.dianchejie.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://fbt.xuetiantiany.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wef.jianghu66.top


<!-- 参考信息 -->