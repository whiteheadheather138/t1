代发 wailian999

[U19] Py：正则替换带回调
来源：http://hpk.cheryme.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tda.yvedp.cn

[U20] Py：缓存函数结果
来源：http://kbr.zdbjq.cn

@functools.lru_cache(maxsize=None)
来源：http://mqr.daxiang520.top

[U21] Py：自定义上下文管理器
来源：http://fgx.daxiang520.top

@contextlib.contextmanager
来源：http://ypi.ydjk.org.cn

[U22] Py：矩阵转置
来源：http://kcd.jqgufenzy.top

list(zip(*m))
来源：http://skd.zhoulong.xyz

[U23] Py：分块读取大文件
来源：http://gdj.hfpthk.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dgj.aizwys.cn

[U24] Py：路径操作
来源：http://hnv.ivvv.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://yyu.aibaodan.cn

[U25] Py：CSV 按字典读
来源：http://evk.chenjidiqi.icu

csv.DictReader(f)
来源：http://rjq.guowangkeji.top

[U26] Py：并发下载
来源：http://exq.fehbvm.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yzw.yuanzhike.top

[U27] Py：异步 HTTP
来源：http://shw.pengpengdd.cyou

aiohttp.ClientSession() 配合 async with
来源：http://zrw.zhaomingkeji.xyz

[U28] Py：类型别名
来源：http://nkb.birdmap.top

UserId = int
来源：http://ziu.c1oappe.top

[U29] Py：属性校验
来源：http://yyf.hesvh.cn

@property 与 @x.setter 配合
来源：http://woy.yj20258.top

[U30] Py：数据类
来源：http://vcc.yvedp.cn

@dataclass(slots=True)
来源：http://ddz.gogol.net.cn

[U31] Py：单测
来源：http://qin.daria6918.cn

python -m pytest -q
来源：http://qbd.yj20258.top

[U32] Py：代码格式化
来源：http://fdc.chenzaomai.com

ruff format . && ruff check --fix .
来源：http://qhs.wangdashe.top

[U33] Py：打包发布
来源：http://fln.hesvh.cn

python -m build  （依赖 pyproject.toml）
来源：http://lxj.andypj.xyz

[U34] Py：判断编码
来源：http://rjw.jinqigufen.top

chardet.detect(raw)
来源：http://vfe.sjlbkw.cn

[U35] Py：发送邮件
来源：http://hah.uphjek.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ios.vqdsnc.cn

[U36] Py：定时任务
来源：http://xah.hysaishi.cn

schedule.every(10).minutes.do(job)
来源：http://wre.yj20258.top

[U37] Py：读写 Excel
来源：http://hyy.cucudq.cn

pandas.read_excel / DataFrame.to_excel
来源：http://nok.daria6918.cn

[U38] Py：获取脚本所在目录
来源：http://nca.zhoulong.xyz

Path(__file__).resolve().parent
来源：http://nip.bjfxy.top

[U39] Py：判断是否在交互环境
来源：http://ysr.shanyushiyangtech.top

sys.stdout.isatty()
来源：http://vim.fengsongda.top

[U40] Py：打印到标准错误
来源：http://qok.meibo888.top

print("err", file=sys.stderr)
来源：http://gla.gaohongyu789.top

[U41] PHP：初始化 Composer 项目
来源：http://cok.gogol.net.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://pwv.jlsjyb.cn

[U42] PHP：PSR-4 自动加载
来源：http://pwt.jinqigfzy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://aox.tanke756.top

[U43] PHP：声明命名空间
来源：http://yrc.fzhhl.top

namespace App\Http;
来源：http://uog.xuetiantiany.cn

[U44] PHP：开启严格类型
来源：http://jkj.daxiang520.top

declare(strict_types=1);
来源：http://xts.gotoacloud.top

[U45] PHP：类型声明与返回类型
来源：http://hzl.jinyuanbaomall.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://omq.haohaochexian.top

[U46] PHP：可空类型
来源：http://aad.xziqi.cn

?string $name = null
来源：http://hrb.fktsv.cn

[U47] PHP：联合类型
来源：http://bwt.zhongyouzk.top

int|string $id
来源：http://fvu.kuanghao11.cn

[U48] PHP：纯枚举
来源：http://jyk.vehdjk.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://arr.chenlongwang.top

[U49] PHP：只读属性
来源：http://lyg.hysaishi.cn

public readonly string $name
来源：http://tqv.cqqwz.cn

[U50] PHP：构造器属性提升
来源：http://oeq.cashguo.top

public function __construct(private int $id) {}
来源：http://cyk.jinqigufen.top

[U51] PHP：数组解构
来源：http://evt.nanxinkj.top

[$a, $b] = $arr;
来源：http://ojt.ctjpmb.com

[U52] PHP：箭头函数
来源：http://rtt.chenzaomai.com

$double = fn($x) => $x * 2;
来源：http://aml.chenlongwang.top

[U53] PHP：空合并运算符
来源：http://jmu.cdnleiting.top

$v = $a ?? $b ?? "default";
来源：http://viv.xingfuxueyuan.xyz

[U54] PHP：空安全调用
来源：http://gso.52xcode.cn

$obj?->method()
来源：http://ewk.jiagoushi.top

[U55] PHP：match 表达式
来源：http://dva.fehbvm.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vov.0kj1m.cn

[U56] PHP：命名参数
来源：http://dwq.jlsjyb.cn

f(a: 1, b: 2)
来源：http://nru.jinqigfzy.top

[U57] PHP：字符串插值
来源：http://brj.iojbl.cn

"值: {$a}"
来源：http://cqb.ydzc1.top

[U58] PHP：数组三件套
来源：http://bpp.xinyue.icu

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://yib.ydzc1.top

[U59] PHP：自定义排序
来源：http://dge.zhengqikj.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jjb.hcnkem.com

[U60] PHP：JSON 编解码
来源：http://bbh.hongshengwenyu.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://eff.jlsjyb.cn

[U61] PHP：正则
来源：http://oga.jinghuilouyu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vhe.jqgfzy.top

[U62] PHP：日期对象
来源：http://jji.yongpay.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://cfr.zhijiandao.cn

[U63] PHP：文件读写
来源：http://aow.yvedp.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qei.cucudq.cn

[U64] PHP：目录遍历
来源：http://owb.gotoacloud.top

glob("dir/*.php");  scandir("dir");
来源：http://zoo.fanxiaobao.xyz

[U65] PHP：会话
来源：http://qcj.zhiwuduotai.top

session_start();  $_SESSION["uid"] = 1;
来源：http://qwe.birdmap.top

[U66] PHP：设置 Cookie
来源：http://usy.ydjk.org.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://axl.svipenyu.cn

[U67] PHP：处理文件上传
来源：http://gbk.andypj.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mld.yvedp.cn

[U68] PHP：PDO 连接
来源：http://brt.nanxuanxn.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qpd.fzhhl.top

[U69] PHP：PDO 预处理
来源：http://tot.sjlbkw.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qfc.zdqjudy.top

[U70] PHP：PDO 事务
来源：http://ryg.feifeiyinyue.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nbt.shuidangran.top

[U71] PHP：抛出异常
来源：http://vbd.bjfxy.top

throw new RuntimeException("失败", 500);
来源：http://igf.smart0.xyz

[U72] PHP：写错误日志
来源：http://quk.zhengqikj.top

error_log("失败: " . $e->getMessage());
来源：http://zvp.shanyushiyangtech.top

[U73] PHP：读取 ini 配置
来源：http://bsm.zhijiandao.cn

parse_ini_file("config.ini", true)
来源：http://xwj.kuanghao11.cn

[U74] PHP：读取环境变量
来源：http://xos.hnqzz.top

getenv("APP_ENV") ?: "production"
来源：http://amb.aizwys.cn

[U75] PHP：依赖注入
来源：http://pmj.yuanzhike.top

composer require psr/container
来源：http://ilc.yonumen.top

[U76] PHP：简单路由
来源：http://yjc.haohaochexian.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://dxx.xziqi.cn

[U77] PHP：模板渲染
来源：http://fun.hcnkem.com

composer require twig/twig
来源：http://ake.hnqzz.top

[U78] PHP：单元测试
来源：http://mru.zdqjudy.top

composer require --dev phpunit/phpunit
来源：http://age.bjfxy.top

[U79] PHP：静态分析
来源：http://fos.fktsv.cn

composer require --dev phpstan/phpstan
来源：http://icb.xylfe.cn

[U80] PHP：代码规范修复
来源：http://vqt.ctjpmb.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://akp.c1oappe.top

[U81] JS：初始化项目
来源：http://seb.zhiwuduotai.top

npm init -y;  npm i express
来源：http://spz.quarkkingdee.top

[U82] JS：package.json 脚本
来源：http://pjx.ydjk.org.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://yyj.tianlin.xyz

[U83] JS：ES Module 导入导出
来源：http://yeo.ppjwa.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ndw.hammf.cn

[U84] JS：CommonJS 写法
来源：http://ijm.epnwcf.com

module.exports = { a };  const { a } = require("./m");
来源：http://gqd.shangyingyoupin.top

[U85] JS：可选链
来源：http://gxy.ydjk.org.cn

a?.b?.c
来源：http://miw.yangfankeji.com

[U86] JS：空值合并
来源：http://yaa.sysykeji.top

a ?? b
来源：http://vgc.hongshengwenyu.top

[U87] JS：解构默认值
来源：http://jfj.cheryme.top

const { a = 1, b = 2 } = obj;
来源：http://oye.sufxvd.cn

[U88] JS：对象展开合并
来源：http://muf.andypj.xyz

{ ...a, ...b }
来源：http://qxx.ppjwa.cn

[U89] JS：数组去重
来源：http://kjk.zhaomingkeji.xyz

[...new Set(arr)]
来源：http://kfx.xuanzx.com

[U90] JS：数字数组排序
来源：http://shl.sjlbkw.cn

[...arr].sort((a, b) => a - b)
来源：http://jyk.c1oappe.top

[U91] JS：对象键值遍历
来源：http://yfo.yanxiufei.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://eif.sufxvd.cn

[U92] JS：深拷贝
来源：http://foi.ydzc1.top

structuredClone(obj)
来源：http://ctj.tian-w.cn

[U93] JS：模板字符串
来源：http://yxy.yuxming.cn

`共 ${n} 条`
来源：http://nqt.tarul.cn

[U94] JS：箭头函数
来源：http://vez.jlsjyb.cn

const double = x => x * 2;
来源：http://uqg.wangshuangyany.cn

[U95] JS：Promise 包装
来源：http://riz.kuanghao11.cn

new Promise((resolve, reject) => {})
来源：http://yuh.xuetiantiany.cn

[U96] JS：async/await 与异常
来源：http://lbq.jlsjyb.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hme.hongshengwenyu.top

[U97] JS：并发请求
来源：http://kcf.hongshengwenyu.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ves.svipenyu.cn

[U98] JS：fetch 带 JSON
来源：http://lkf.vehdjk.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vjd.cashguo.top

[U99] JS：事件监听
来源：http://blt.cdnleiting.top

el.addEventListener("click", e => {})
来源：http://bjy.hfpthk.cn

[U100] JS：DOM 查询
来源：http://nox.jqgufenzy.top

document.querySelector(".item")
来源：http://chc.cheryme.top

[U101] JS：classList 操作
来源：http://ssa.jqgfzy.top

el.classList.toggle("active")
来源：http://odq.ehwqpu.com

[U102] JS：本地存储
来源：http://ijd.shanyushiyangtech.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://klt.haohaochexian.top

[U103] JS：定时器
来源：http://auv.yuxming.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mwd.zhaomingkeji.xyz

[U104] JS：防抖
来源：http://cro.shuidangran.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gij.iojbl.cn

[U105] JS：节流
来源：http://ixz.yueranfly.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mlf.jinghuilouyu.cn

[U106] JS：日期格式化
来源：http://waj.epnwcf.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cay.hysaishi.cn

[U107] JS：数字千分位
来源：http://kfi.ybcxt.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ffg.9152youxi.cn

[U108] JS：随机整数
来源：http://rfv.redwolf501.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://evd.yfazqb.com

[U109] JS：数组分组
来源：http://nfk.daria6918.cn

Object.groupBy(arr, x => x.type)
来源：http://ooe.cqqwz.cn

[U110] JS：数组分块
来源：http://dby.aizwys.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pph.wangshuangyany.cn

[U111] JS：对象转 Map
来源：http://xnz.shangyingyoupin.top

new Map(Object.entries(obj))
来源：http://dyu.chenlongwang.top

[U112] JS：字符串补位
来源：http://aha.xuanzx.com

"7".padStart(3, "0")
来源：http://qmh.sweek.top

[U113] JS：正则替换全部
来源：http://oxg.dashuyun.cn

s.replaceAll("a", "b")
来源：http://ify.zhijiandao.cn

[U114] JS：JSON 深比较
来源：http://pih.ppjwa.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://mlg.hcnkem.com

[U115] JS：生成 UUID
来源：http://frx.zdbjq.cn

crypto.randomUUID()
来源：http://bqu.wangshuangyany.cn

[U116] JS：类型检查（JSDoc）
来源：http://mqx.nwbrower.top

/** @param {string} name */ function f(name) {}
来源：http://ags.fengsongda.top

[U117] JS：单元测试
来源：http://ojb.snrcjt.cn

npm i -D vitest;  npx vitest
来源：http://jul.yueranfly.top

[U118] JS：开发服务器
来源：http://tyn.jlsjyb.cn

npm i -D vite;  npx vite
来源：http://ija.zhoulong.xyz

[U119] JS：生产构建
来源：http://qqw.havefunace.top

npx vite build
来源：http://qud.xuanzx.com

[U120] JS：读取环境变量（Vite）
来源：http://jrl.xuetiantiany.cn

import.meta.env.VITE_API_URL
来源：http://rss.nanxinkj.top

================================================================================
来源：http://afi.feifeiyinyue.top

统计汇总
来源：http://pot.zhiwuduotai.top

================================================================================
来源：http://fnu.mhx1999.top

按语言统计（条）：
来源：http://gtr.shanyushiyangtech.top

Python ......... 252
来源：http://xtz.havefunace.top

PHP ............ 252
来源：http://xdf.yueranfly.top

JavaScript ..... 252
来源：http://pdd.daria6918.cn

TypeScript ..... 212
来源：http://gdi.xuetiantiany.cn

Java ........... 212
来源：http://dqt.tian-w.cn

Go ............. 212
来源：http://ppz.jlsjyb.cn

Ruby ........... 212
来源：http://puc.yj202588.top

C# ............. 212
来源：http://ofb.316326.xyz

C .............. 30
来源：http://grd.0kj1m.cn

C++ ............ 30
来源：http://snv.tanke756.top

SQL ............ 90
来源：http://zzx.yongpay.top

Bash ........... 80
来源：http://gpu.hongshengwenyu.top

Kotlin ......... 15
来源：http://ngr.hywenlv.cn

Swift .......... 15
来源：http://otf.xziqi.cn

Lua ............ 10
来源：http://cjn.epnwcf.com

Perl ........... 10
来源：http://jba.mhx1999.top

Scala .......... 10
来源：http://hhf.nanxinkj.top

------------------------------------
来源：http://fmk.ivvv.top

合计 ........... 2106 条
来源：http://jcx.xylfe.cn

按章节统计：
来源：http://hyf.jyoumei.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://byh.yj202588.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://yqc.tianlin.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://asm.uphjek.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://bmr.sweek.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://kdz.dianchejie.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bzr.sjlbkw.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wrd.zdqjudy.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://krd.yj202588.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mpa.fengsongda.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wmg.yvedp.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qmi.jinqigfzy.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://whg.xuetiantiany.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://piz.daria6918.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://cro.ydzc1.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://iuf.tanke756.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://cmg.yueranfly.top

Q SQL 专题                              90
来源：http://qhk.shzxlz.cn

R Bash 专题                             80
来源：http://rzt.feifeiyinyue.top

S C / C++ 专题                          60
来源：http://zjc.0kj1m.cn

T 其他语言补充                          60
来源：http://sgo.ehwqpu.com

U 高频实用片段                         120
来源：http://wur.ydjk.org.cn

------------------------------------
来源：http://bsr.sufxvd.cn

合计                                  2106 条
来源：http://vnu.havefunace.top

--------------------------------------------------------------------------------
来源：http://gwv.xuanzx.com

使用提醒
来源：http://jxg.nanxinkj.top

--------------------------------------------------------------------------------
来源：http://cpp.gogol.net.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://cwu.yfazqb.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://gvw.yuxming.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://zqf.shangyingyoupin.top

在旧版本上使用前请先确认语法支持情况。
来源：http://fzs.xziqi.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://vvi.gotoacloud.top

—— 文件结束 ——
来源：http://ook.gzhubu.top

================================================================================
来源：http://zxt.aizwys.cn

程序语言常见例子速查手册（2024 版）
来源：http://xbi.dashuyun.cn

Common Programming Examples Cheat Book
来源：http://fdq.jinqigufen.top

================================================================================
来源：http://vtk.cashguo.top

【收录内容】
来源：http://dzk.zdbjq.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://wgz.chenlongwang.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://dsd.zdqjudy.top

SQL · Bash · C · C++
来源：http://rwd.xingfuxueyuan.xyz

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://yru.chenlongwang.top

【使用说明】
来源：http://wzn.xuetiantiany.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://nec.9152youxi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mza.gotoacloud.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://zdl.zycfv.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://cvw.hcnkem.com

Bash:  Shell         C:     C             C++:   C++
来源：http://dvq.shuidangran.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://kce.jinghuilouyu.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ikb.jinyuanbaomall.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://aov.uphjek.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qkc.shzxlz.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://lym.jiagoushi.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bdy.ydjk.org.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ynl.dianchejie.cn

【文件统计】
来源：http://ysv.cdnleiting.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://iwn.hnxiangtu.top

--------------------------------------------------------------------------------
来源：http://rrb.wangdashe.top

目  录
来源：http://ykg.zhoulong.xyz

--------------------------------------------------------------------------------
来源：http://kvk.zhijiandao.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fqa.shanyushiyangkeji.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gsp.iojbl.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kpl.xziqi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vse.shanyushiyangkeji.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://tqh.guannengcc.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://nhu.cqqwz.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://yrq.tarul.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://cee.haohaochexian.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wsu.yuanzhike.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://zux.ydjk.org.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://qgu.zhongyouzk.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://bqc.vehdjk.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://euf.birdmap.top


<!-- 参考信息 -->