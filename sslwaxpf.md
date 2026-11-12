代发 wailian999

[U19] Py：正则替换带回调
来源：http://ols.yonumen.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wlp.gotoacloud.top

[U20] Py：缓存函数结果
来源：http://svm.jyoumei.cn

@functools.lru_cache(maxsize=None)
来源：http://mpp.quarkkingdee.top

[U21] Py：自定义上下文管理器
来源：http://afz.zycfv.cn

@contextlib.contextmanager
来源：http://syy.jianghu66.top

[U22] Py：矩阵转置
来源：http://naf.tian-w.cn

list(zip(*m))
来源：http://fuf.ywan-chungtsiang.top

[U23] Py：分块读取大文件
来源：http://phv.yangfankeji.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jsc.chenjidiqi.icu

[U24] Py：路径操作
来源：http://omz.uphjek.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://auf.snrcjt.cn

[U25] Py：CSV 按字典读
来源：http://jvf.uphjek.com

csv.DictReader(f)
来源：http://frt.ehwqpu.com

[U26] Py：并发下载
来源：http://dij.dashuyun.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nmp.shangyingyoupin.top

[U27] Py：异步 HTTP
来源：http://kjo.yangfankeji.com

aiohttp.ClientSession() 配合 async with
来源：http://psf.aizwys.cn

[U28] Py：类型别名
来源：http://jfo.cucudq.cn

UserId = int
来源：http://xow.zhijiandao.cn

[U29] Py：属性校验
来源：http://jrh.hfpthk.cn

@property 与 @x.setter 配合
来源：http://tel.shanyushiyangtech.top

[U30] Py：数据类
来源：http://igx.guowangkeji.top

@dataclass(slots=True)
来源：http://ebv.ctjpmb.com

[U31] Py：单测
来源：http://zfc.daxiang520.top

python -m pytest -q
来源：http://xfw.vehdjk.com

[U32] Py：代码格式化
来源：http://rex.aibaodan.cn

ruff format . && ruff check --fix .
来源：http://jlh.tianlin.xyz

[U33] Py：打包发布
来源：http://iux.redwolf501.top

python -m build  （依赖 pyproject.toml）
来源：http://obo.jlsjyb.cn

[U34] Py：判断编码
来源：http://uyl.shzxlz.cn

chardet.detect(raw)
来源：http://cri.shangyingyoupin.top

[U35] Py：发送邮件
来源：http://aaq.gaohongyu789.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tnl.zycfv.cn

[U36] Py：定时任务
来源：http://jus.ivvv.top

schedule.every(10).minutes.do(job)
来源：http://zrd.zhoulong.xyz

[U37] Py：读写 Excel
来源：http://pmk.hcnkem.com

pandas.read_excel / DataFrame.to_excel
来源：http://zue.xylfe.cn

[U38] Py：获取脚本所在目录
来源：http://hdz.aizwys.cn

Path(__file__).resolve().parent
来源：http://uay.tarul.cn

[U39] Py：判断是否在交互环境
来源：http://bdi.nanxinkj.top

sys.stdout.isatty()
来源：http://qtx.pycfn.com

[U40] Py：打印到标准错误
来源：http://cfc.zdqjudy.top

print("err", file=sys.stderr)
来源：http://aeh.jiagoushi.top

[U41] PHP：初始化 Composer 项目
来源：http://jje.fzhhl.top

composer init;  composer require guzzlehttp/guzzle
来源：http://wdc.vehdjk.com

[U42] PHP：PSR-4 自动加载
来源：http://kfe.yj202588.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://kcv.yangfankeji.com

[U43] PHP：声明命名空间
来源：http://ere.meibo888.top

namespace App\Http;
来源：http://iqa.yongpay.top

[U44] PHP：开启严格类型
来源：http://ykd.aibaodan.cn

declare(strict_types=1);
来源：http://lwp.zycfv.cn

[U45] PHP：类型声明与返回类型
来源：http://ubp.jiagoushi.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://zru.jiagoushi.top

[U46] PHP：可空类型
来源：http://yrv.sysykeji.top

?string $name = null
来源：http://asw.bbcook.cn

[U47] PHP：联合类型
来源：http://dly.daria6918.cn

int|string $id
来源：http://hkn.jqgufenzy.top

[U48] PHP：纯枚举
来源：http://jrk.jinyuanbaomall.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ylq.hfpthk.cn

[U49] PHP：只读属性
来源：http://qgm.daria6918.cn

public readonly string $name
来源：http://yly.fengsongda.top

[U50] PHP：构造器属性提升
来源：http://cyr.fzhhl.top

public function __construct(private int $id) {}
来源：http://iux.bjfxy.top

[U51] PHP：数组解构
来源：http://pdn.yj20258.top

[$a, $b] = $arr;
来源：http://bkz.zhongyouzk.top

[U52] PHP：箭头函数
来源：http://jnm.sysykeji.top

$double = fn($x) => $x * 2;
来源：http://faf.fktsv.cn

[U53] PHP：空合并运算符
来源：http://twe.smart0.xyz

$v = $a ?? $b ?? "default";
来源：http://kly.xuanzx.com

[U54] PHP：空安全调用
来源：http://jpd.epnwcf.com

$obj?->method()
来源：http://flv.yj20258888.top

[U55] PHP：match 表达式
来源：http://bpg.zhoulong.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wnd.zhiwuduotai.top

[U56] PHP：命名参数
来源：http://gnb.mhx1999.top

f(a: 1, b: 2)
来源：http://ahp.andypj.xyz

[U57] PHP：字符串插值
来源：http://hwp.sufxvd.cn

"值: {$a}"
来源：http://dnw.chenjidiqi.icu

[U58] PHP：数组三件套
来源：http://mim.gogol.net.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fho.fengsongda.top

[U59] PHP：自定义排序
来源：http://lvi.yfazqb.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dev.shanyushiyangkeji.top

[U60] PHP：JSON 编解码
来源：http://qwm.ctjpmb.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qwh.tanke756.top

[U61] PHP：正则
来源：http://yfm.dashuyun.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://uzp.xuetiantiany.cn

[U62] PHP：日期对象
来源：http://dae.nanxuanxn.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://uya.pengpengdd.cyou

[U63] PHP：文件读写
来源：http://wmt.chenzaomai.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gaf.sufxvd.cn

[U64] PHP：目录遍历
来源：http://mgs.ydjk.org.cn

glob("dir/*.php");  scandir("dir");
来源：http://wcx.yfazqb.com

[U65] PHP：会话
来源：http://lxv.sjlbkw.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://bsw.sufxvd.cn

[U66] PHP：设置 Cookie
来源：http://mwq.xingfuxueyuan.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ngg.sysykeji.top

[U67] PHP：处理文件上传
来源：http://wnx.sufxvd.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://upq.cheryme.top

[U68] PHP：PDO 连接
来源：http://scp.tian-w.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ieo.xingfuxueyuan.xyz

[U69] PHP：PDO 预处理
来源：http://suk.gotoacloud.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lla.gaohongyu789.top

[U70] PHP：PDO 事务
来源：http://vga.jinqigfzy.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://les.zycfv.cn

[U71] PHP：抛出异常
来源：http://vyr.epnwcf.com

throw new RuntimeException("失败", 500);
来源：http://owm.jlsjyb.cn

[U72] PHP：写错误日志
来源：http://pia.wangshuangyany.cn

error_log("失败: " . $e->getMessage());
来源：http://oeh.zhongyouzk.top

[U73] PHP：读取 ini 配置
来源：http://elr.xingfuxueyuan.xyz

parse_ini_file("config.ini", true)
来源：http://wca.zhoulong.xyz

[U74] PHP：读取环境变量
来源：http://xzh.chenlongwang.top

getenv("APP_ENV") ?: "production"
来源：http://tgu.jinqigfzy.top

[U75] PHP：依赖注入
来源：http://gib.zdqjudy.top

composer require psr/container
来源：http://axj.pengpengdd.cyou

[U76] PHP：简单路由
来源：http://nuu.sweek.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://drj.svipenyu.cn

[U77] PHP：模板渲染
来源：http://izs.zhoulong.xyz

composer require twig/twig
来源：http://bba.cqqwz.cn

[U78] PHP：单元测试
来源：http://hqp.tanke756.top

composer require --dev phpunit/phpunit
来源：http://xop.xinyue.icu

[U79] PHP：静态分析
来源：http://gkn.sweek.top

composer require --dev phpstan/phpstan
来源：http://olr.ybcxt.top

[U80] PHP：代码规范修复
来源：http://uex.jinqigufen.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://adj.hammf.cn

[U81] JS：初始化项目
来源：http://gkk.nanxinkj.top

npm init -y;  npm i express
来源：http://lfj.yj20258888.top

[U82] JS：package.json 脚本
来源：http://xfi.c1oappe.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://egk.cqqwz.cn

[U83] JS：ES Module 导入导出
来源：http://qtd.bjfxy.top

export const a = 1;  import { a } from "./m.js";
来源：http://ccw.cashguo.top

[U84] JS：CommonJS 写法
来源：http://mhc.daria6918.cn

module.exports = { a };  const { a } = require("./m");
来源：http://inb.uphjek.com

[U85] JS：可选链
来源：http://qbm.ybcxt.top

a?.b?.c
来源：http://uwl.shanyushiyangkeji.top

[U86] JS：空值合并
来源：http://xtg.meibo888.top

a ?? b
来源：http://fzp.aizwys.cn

[U87] JS：解构默认值
来源：http://nlr.bjfxy.top

const { a = 1, b = 2 } = obj;
来源：http://xbh.yangfankeji.com

[U88] JS：对象展开合并
来源：http://jpl.sysykeji.top

{ ...a, ...b }
来源：http://rbl.yuanzhike.top

[U89] JS：数组去重
来源：http://utx.zhixingplan.top

[...new Set(arr)]
来源：http://udl.yj20258888.top

[U90] JS：数字数组排序
来源：http://nqq.yfazqb.com

[...arr].sort((a, b) => a - b)
来源：http://ygx.ybcxt.top

[U91] JS：对象键值遍历
来源：http://eib.ctjpmb.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xsw.daxiang520.top

[U92] JS：深拷贝
来源：http://pgk.daxiang520.top

structuredClone(obj)
来源：http://qxr.xingfuxueyuan.xyz

[U93] JS：模板字符串
来源：http://sbm.meibo888.top

`共 ${n} 条`
来源：http://qep.feifeiyinyue.top

[U94] JS：箭头函数
来源：http://irc.wangshuangyany.cn

const double = x => x * 2;
来源：http://uvs.nanxuanxn.top

[U95] JS：Promise 包装
来源：http://uum.zhiwuduotai.top

new Promise((resolve, reject) => {})
来源：http://awm.hammf.cn

[U96] JS：async/await 与异常
来源：http://xqh.andypj.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pcm.wangshuangyany.cn

[U97] JS：并发请求
来源：http://znh.meibo888.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://bse.redwolf501.top

[U98] JS：fetch 带 JSON
来源：http://ezi.fanxiaobao.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://slo.hnqzz.top

[U99] JS：事件监听
来源：http://kbn.hnxiangtu.top

el.addEventListener("click", e => {})
来源：http://npe.snrcjt.cn

[U100] JS：DOM 查询
来源：http://rur.hammf.cn

document.querySelector(".item")
来源：http://ygw.svipenyu.cn

[U101] JS：classList 操作
来源：http://ilj.zhoulong.xyz

el.classList.toggle("active")
来源：http://gmr.hammf.cn

[U102] JS：本地存储
来源：http://mhx.zhengqikj.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://sxx.yj202588.top

[U103] JS：定时器
来源：http://mxw.shanyushiyangkeji.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wcc.nanxuanxn.top

[U104] JS：防抖
来源：http://oot.zhaomingkeji.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sjj.kuanghao11.cn

[U105] JS：节流
来源：http://pzd.mhx1999.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://min.quarkkingdee.top

[U106] JS：日期格式化
来源：http://esk.fehbvm.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kbh.zhaomingkeji.xyz

[U107] JS：数字千分位
来源：http://pra.shangyingyoupin.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://adh.jyoumei.cn

[U108] JS：随机整数
来源：http://rdi.tarul.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gnh.yongpay.top

[U109] JS：数组分组
来源：http://duw.cqqwz.cn

Object.groupBy(arr, x => x.type)
来源：http://iyj.shanyushiyangkeji.top

[U110] JS：数组分块
来源：http://cfl.sysykeji.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cwp.fktsv.cn

[U111] JS：对象转 Map
来源：http://gga.316326.xyz

new Map(Object.entries(obj))
来源：http://smv.chenlongwang.top

[U112] JS：字符串补位
来源：http://fet.fktsv.cn

"7".padStart(3, "0")
来源：http://nud.feifeiyinyue.top

[U113] JS：正则替换全部
来源：http://gmr.316326.xyz

s.replaceAll("a", "b")
来源：http://gra.cdnleiting.top

[U114] JS：JSON 深比较
来源：http://beg.dianchejie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://gpg.redwolf501.top

[U115] JS：生成 UUID
来源：http://nem.cqqwz.cn

crypto.randomUUID()
来源：http://roz.nanxuanxn.top

[U116] JS：类型检查（JSDoc）
来源：http://aaa.chenzaomai.com

/** @param {string} name */ function f(name) {}
来源：http://gvb.xziqi.cn

[U117] JS：单元测试
来源：http://yji.mhx1999.top

npm i -D vitest;  npx vitest
来源：http://tsv.ctjpmb.com

[U118] JS：开发服务器
来源：http://xef.yj202588.top

npm i -D vite;  npx vite
来源：http://yos.0kj1m.cn

[U119] JS：生产构建
来源：http://lmr.xuetiantiany.cn

npx vite build
来源：http://riz.meibo888.top

[U120] JS：读取环境变量（Vite）
来源：http://yhb.pengpengdd.cyou

import.meta.env.VITE_API_URL
来源：http://eim.jinqigufen.top

================================================================================
来源：http://lzm.smart0.xyz

统计汇总
来源：http://ouo.cashguo.top

================================================================================
来源：http://spz.xinyue.icu

按语言统计（条）：
来源：http://upp.yj202588.top

Python ......... 252
来源：http://ilj.fengsongda.top

PHP ............ 252
来源：http://fun.sweek.top

JavaScript ..... 252
来源：http://wex.chenlongwang.top

TypeScript ..... 212
来源：http://hps.zdbjq.cn

Java ........... 212
来源：http://dxc.sjlbkw.cn

Go ............. 212
来源：http://ubi.smart0.xyz

Ruby ........... 212
来源：http://des.sjlbkw.cn

C# ............. 212
来源：http://cbb.hongshengwenyu.top

C .............. 30
来源：http://dgf.gotoacloud.top

C++ ............ 30
来源：http://qxp.xingfuxueyuan.xyz

SQL ............ 90
来源：http://tgl.gaohongyu789.top

Bash ........... 80
来源：http://bcw.sysykeji.top

Kotlin ......... 15
来源：http://jwn.andypj.xyz

Swift .......... 15
来源：http://kao.fktsv.cn

Lua ............ 10
来源：http://wks.zhoulong.xyz

Perl ........... 10
来源：http://yjz.ehwqpu.com

Scala .......... 10
来源：http://byh.pengpengdd.cyou

------------------------------------
来源：http://eyz.316326.xyz

合计 ........... 2106 条
来源：http://kju.cashguo.top

按章节统计：
来源：http://iys.ctjpmb.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ecn.hongshengwenyu.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wkj.c1oappe.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://tgh.yfazqb.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://plr.jyoumei.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://lvo.fktsv.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://jwh.nanxuanxn.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hqa.hywenlv.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kbd.bjfxy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://tas.yj202588.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wof.hongshengwenyu.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gvo.yvedp.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cas.haohaochexian.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://twf.birdmap.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tkb.tarul.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ynd.xylfe.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://nah.epnwcf.com

Q SQL 专题                              90
来源：http://qxc.fktsv.cn

R Bash 专题                             80
来源：http://yjg.mhx1999.top

S C / C++ 专题                          60
来源：http://mlz.jlsjyb.cn

T 其他语言补充                          60
来源：http://ykp.aibaodan.cn

U 高频实用片段                         120
来源：http://nex.sweek.top

------------------------------------
来源：http://zaj.fktsv.cn

合计                                  2106 条
来源：http://mzq.uphjek.com

--------------------------------------------------------------------------------
来源：http://dol.jinyuanbaomall.cn

使用提醒
来源：http://qgg.dashuyun.cn

--------------------------------------------------------------------------------
来源：http://kgt.sufxvd.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://aze.haohaochexian.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tix.iojbl.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://pum.xingfuxueyuan.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://vjt.yuxming.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mrl.jiagoushi.top

—— 文件结束 ——
来源：http://ajc.gotoacloud.top

================================================================================
来源：http://yqz.52xcode.cn

程序语言常见例子速查手册（2024 版）
来源：http://stn.xingfuxueyuan.xyz

Common Programming Examples Cheat Book
来源：http://kra.sjlbkw.cn

================================================================================
来源：http://ati.fehbvm.com

【收录内容】
来源：http://jjj.fehbvm.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://abl.zhengqikj.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://sdc.gotoacloud.top

SQL · Bash · C · C++
来源：http://oma.yj202588.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://cwt.gzhubu.top

【使用说明】
来源：http://vjl.shanyushiyangtech.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://zme.kuanghao11.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://njy.yuxming.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://zcu.ywan-chungtsiang.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://xhk.xinyue.icu

Bash:  Shell         C:     C             C++:   C++
来源：http://bty.daria6918.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jyp.aizwys.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://avu.uphjek.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://fvt.tianlin.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qri.haohaochexian.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://dgg.xuetiantiany.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://zgg.fzhhl.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://yvj.fzhhl.top

【文件统计】
来源：http://ahl.fehbvm.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://lad.c1oappe.top

--------------------------------------------------------------------------------
来源：http://gvk.yj202588.top

目  录
来源：http://npp.zhoulong.xyz

--------------------------------------------------------------------------------
来源：http://xmz.ybcxt.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hsa.bjfxy.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://eom.yanxiufei.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://tlz.uphjek.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zsw.yj20258.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://iix.hammf.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://upo.gogol.net.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://lyj.nanxuanxn.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ivr.bjfxy.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://aot.jyoumei.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://zep.daxiang520.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hoc.uphjek.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://rcq.ctjpmb.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qqj.sxryk.cn


<!-- 参考信息 -->