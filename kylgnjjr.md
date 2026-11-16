代发 wailian999

[U19] Py：正则替换带回调
来源：http://eln.daria6918.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jcb.hfpthk.cn

[U20] Py：缓存函数结果
来源：http://nlo.nwbrower.top

@functools.lru_cache(maxsize=None)
来源：http://qsv.yj20258.top

[U21] Py：自定义上下文管理器
来源：http://ykd.yongpay.top

@contextlib.contextmanager
来源：http://xgd.cheryme.top

[U22] Py：矩阵转置
来源：http://kbk.fehbvm.com

list(zip(*m))
来源：http://rqc.hammf.cn

[U23] Py：分块读取大文件
来源：http://ear.yongpay.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://shm.zhixingplan.top

[U24] Py：路径操作
来源：http://cpv.52xcode.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qvk.shzxlz.cn

[U25] Py：CSV 按字典读
来源：http://nhm.xinyue.icu

csv.DictReader(f)
来源：http://aaa.yangfankeji.com

[U26] Py：并发下载
来源：http://fnl.yangfankeji.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://new.pengpengdd.cyou

[U27] Py：异步 HTTP
来源：http://dlh.dashuyun.cn

aiohttp.ClientSession() 配合 async with
来源：http://gab.tian-w.cn

[U28] Py：类型别名
来源：http://jhn.xylfe.cn

UserId = int
来源：http://buh.zhengqikj.top

[U29] Py：属性校验
来源：http://pzv.gzhubu.top

@property 与 @x.setter 配合
来源：http://rlg.ybcxt.top

[U30] Py：数据类
来源：http://zmi.cheryme.top

@dataclass(slots=True)
来源：http://fnf.shanyushiyangkeji.top

[U31] Py：单测
来源：http://ynl.0kj1m.cn

python -m pytest -q
来源：http://jht.ppjwa.cn

[U32] Py：代码格式化
来源：http://csy.zhixingplan.top

ruff format . && ruff check --fix .
来源：http://nqt.52xcode.cn

[U33] Py：打包发布
来源：http://boa.hongshengwenyu.top

python -m build  （依赖 pyproject.toml）
来源：http://srx.ivvv.top

[U34] Py：判断编码
来源：http://oxg.yfazqb.com

chardet.detect(raw)
来源：http://jyf.jqgufenzy.top

[U35] Py：发送邮件
来源：http://gyd.fktsv.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://brk.aizwys.cn

[U36] Py：定时任务
来源：http://uws.sxryk.cn

schedule.every(10).minutes.do(job)
来源：http://bpr.nanxuanxn.top

[U37] Py：读写 Excel
来源：http://cxt.redwolf501.top

pandas.read_excel / DataFrame.to_excel
来源：http://avk.tianlin.xyz

[U38] Py：获取脚本所在目录
来源：http://dyq.yj202588.top

Path(__file__).resolve().parent
来源：http://ryj.kuanghao11.cn

[U39] Py：判断是否在交互环境
来源：http://dzl.chenlongwang.top

sys.stdout.isatty()
来源：http://sgn.tanke756.top

[U40] Py：打印到标准错误
来源：http://wbd.hywenlv.cn

print("err", file=sys.stderr)
来源：http://eta.cqqwz.cn

[U41] PHP：初始化 Composer 项目
来源：http://wsb.ydzc1.top

composer init;  composer require guzzlehttp/guzzle
来源：http://fwp.chenlongwang.top

[U42] PHP：PSR-4 自动加载
来源：http://czc.yfazqb.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xvv.tianlin.xyz

[U43] PHP：声明命名空间
来源：http://lql.cashguo.top

namespace App\Http;
来源：http://tjv.bbcook.cn

[U44] PHP：开启严格类型
来源：http://xvk.cheryme.top

declare(strict_types=1);
来源：http://ppi.kuanghao11.cn

[U45] PHP：类型声明与返回类型
来源：http://ovg.fengsongda.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://jfh.sweek.top

[U46] PHP：可空类型
来源：http://ukz.ybcxt.top

?string $name = null
来源：http://bme.shanyushiyangkeji.top

[U47] PHP：联合类型
来源：http://vez.hesvh.cn

int|string $id
来源：http://wrv.pengpengdd.cyou

[U48] PHP：纯枚举
来源：http://dyq.zhixingplan.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zje.ydzc1.top

[U49] PHP：只读属性
来源：http://ovf.gotoacloud.top

public readonly string $name
来源：http://jrr.yueranfly.top

[U50] PHP：构造器属性提升
来源：http://rld.cqqwz.cn

public function __construct(private int $id) {}
来源：http://aus.zhengqikj.top

[U51] PHP：数组解构
来源：http://kvc.andypj.xyz

[$a, $b] = $arr;
来源：http://zvb.sjlbkw.cn

[U52] PHP：箭头函数
来源：http://zdi.guannengcc.top

$double = fn($x) => $x * 2;
来源：http://zzy.tanke756.top

[U53] PHP：空合并运算符
来源：http://iyn.cashguo.top

$v = $a ?? $b ?? "default";
来源：http://pbm.zhiwuduotai.top

[U54] PHP：空安全调用
来源：http://wwu.dianchejie.cn

$obj?->method()
来源：http://cju.0kj1m.cn

[U55] PHP：match 表达式
来源：http://jes.nwbrower.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lpi.gzhubu.top

[U56] PHP：命名参数
来源：http://lzm.zdqjudy.top

f(a: 1, b: 2)
来源：http://zby.shanyushiyangtech.top

[U57] PHP：字符串插值
来源：http://caz.tian-w.cn

"值: {$a}"
来源：http://zyg.jinyuanbaomall.cn

[U58] PHP：数组三件套
来源：http://wxq.9152youxi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://scw.guowangkeji.top

[U59] PHP：自定义排序
来源：http://tln.birdmap.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cfo.tarul.cn

[U60] PHP：JSON 编解码
来源：http://lwy.wangdashe.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vfq.quarkkingdee.top

[U61] PHP：正则
来源：http://hkj.yanxiufei.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://uxv.cheryme.top

[U62] PHP：日期对象
来源：http://dbl.pycfn.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://dmv.xuetiantiany.cn

[U63] PHP：文件读写
来源：http://yql.pycfn.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vnt.zhoulong.xyz

[U64] PHP：目录遍历
来源：http://vrg.0kj1m.cn

glob("dir/*.php");  scandir("dir");
来源：http://neo.xziqi.cn

[U65] PHP：会话
来源：http://wtu.bjfxy.top

session_start();  $_SESSION["uid"] = 1;
来源：http://fuv.zycfv.cn

[U66] PHP：设置 Cookie
来源：http://kko.xylfe.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rys.uphjek.com

[U67] PHP：处理文件上传
来源：http://cxm.feifeiyinyue.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xvx.zhongyouzk.top

[U68] PHP：PDO 连接
来源：http://nbg.shanyushiyangkeji.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ldu.shanyushiyangtech.top

[U69] PHP：PDO 预处理
来源：http://xjb.ehwqpu.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://woy.fzhhl.top

[U70] PHP：PDO 事务
来源：http://anf.sweek.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zfh.jianghu66.top

[U71] PHP：抛出异常
来源：http://hkp.yanxiufei.cn

throw new RuntimeException("失败", 500);
来源：http://mqm.zhoulong.xyz

[U72] PHP：写错误日志
来源：http://onv.zhiwuduotai.top

error_log("失败: " . $e->getMessage());
来源：http://knx.52xcode.cn

[U73] PHP：读取 ini 配置
来源：http://imf.gotoacloud.top

parse_ini_file("config.ini", true)
来源：http://kxj.quarkkingdee.top

[U74] PHP：读取环境变量
来源：http://kjy.sysykeji.top

getenv("APP_ENV") ?: "production"
来源：http://ohw.jqgufenzy.top

[U75] PHP：依赖注入
来源：http://wlg.nwbrower.top

composer require psr/container
来源：http://eik.kuanghao11.cn

[U76] PHP：简单路由
来源：http://xda.daxiang520.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bif.ywan-chungtsiang.top

[U77] PHP：模板渲染
来源：http://czw.gzhubu.top

composer require twig/twig
来源：http://qiv.ywan-chungtsiang.top

[U78] PHP：单元测试
来源：http://yhp.epnwcf.com

composer require --dev phpunit/phpunit
来源：http://gju.wangshuangyany.cn

[U79] PHP：静态分析
来源：http://oep.yanxiufei.cn

composer require --dev phpstan/phpstan
来源：http://okw.fanxiaobao.xyz

[U80] PHP：代码规范修复
来源：http://hyg.fehbvm.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://cpa.fktsv.cn

[U81] JS：初始化项目
来源：http://iex.jinghuilouyu.cn

npm init -y;  npm i express
来源：http://csm.feifeiyinyue.top

[U82] JS：package.json 脚本
来源：http://ona.jqgufenzy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nff.mhx1999.top

[U83] JS：ES Module 导入导出
来源：http://ckk.vqdsnc.cn

export const a = 1;  import { a } from "./m.js";
来源：http://xgx.yfazqb.com

[U84] JS：CommonJS 写法
来源：http://ozu.ydjk.org.cn

module.exports = { a };  const { a } = require("./m");
来源：http://sff.cucudq.cn

[U85] JS：可选链
来源：http://eew.hcnkem.com

a?.b?.c
来源：http://oxy.zhiwuduotai.top

[U86] JS：空值合并
来源：http://kvx.zhengqikj.top

a ?? b
来源：http://mmb.dashuyun.cn

[U87] JS：解构默认值
来源：http://irx.fengsongda.top

const { a = 1, b = 2 } = obj;
来源：http://qev.hywenlv.cn

[U88] JS：对象展开合并
来源：http://nli.gotoacloud.top

{ ...a, ...b }
来源：http://qyf.chenlongwang.top

[U89] JS：数组去重
来源：http://tjg.uphjek.com

[...new Set(arr)]
来源：http://bck.zdbjq.cn

[U90] JS：数字数组排序
来源：http://dqk.zhengqikj.top

[...arr].sort((a, b) => a - b)
来源：http://bcg.jlsjyb.cn

[U91] JS：对象键值遍历
来源：http://eip.aibaodan.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://yhl.shuidangran.top

[U92] JS：深拷贝
来源：http://zvk.dianchejie.cn

structuredClone(obj)
来源：http://pbp.havefunace.top

[U93] JS：模板字符串
来源：http://wgj.gotoacloud.top

`共 ${n} 条`
来源：http://vxt.cucudq.cn

[U94] JS：箭头函数
来源：http://cvy.shuidangran.top

const double = x => x * 2;
来源：http://wfi.fzhhl.top

[U95] JS：Promise 包装
来源：http://rsm.yonumen.top

new Promise((resolve, reject) => {})
来源：http://nfv.pycfn.com

[U96] JS：async/await 与异常
来源：http://yot.xziqi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gwc.zhongyouzk.top

[U97] JS：并发请求
来源：http://grt.sysykeji.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://zdg.shangyingyoupin.top

[U98] JS：fetch 带 JSON
来源：http://kko.ctjpmb.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nne.tian-w.cn

[U99] JS：事件监听
来源：http://agh.aibaodan.cn

el.addEventListener("click", e => {})
来源：http://gpq.yueranfly.top

[U100] JS：DOM 查询
来源：http://yef.snrcjt.cn

document.querySelector(".item")
来源：http://vxg.snrcjt.cn

[U101] JS：classList 操作
来源：http://mgf.cucudq.cn

el.classList.toggle("active")
来源：http://ofh.zhongyouzk.top

[U102] JS：本地存储
来源：http://dzh.yj20258888.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://cfm.wangshuangyany.cn

[U103] JS：定时器
来源：http://ffi.wangdashe.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ews.yangfankeji.com

[U104] JS：防抖
来源：http://qus.hongshengwenyu.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lzf.iojbl.cn

[U105] JS：节流
来源：http://zev.fzhhl.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gki.snrcjt.cn

[U106] JS：日期格式化
来源：http://ono.tanke756.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vow.sjlbkw.cn

[U107] JS：数字千分位
来源：http://xaw.hnqzz.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rap.iojbl.cn

[U108] JS：随机整数
来源：http://spb.kuanghao11.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xzz.yj20258.top

[U109] JS：数组分组
来源：http://yfr.316326.xyz

Object.groupBy(arr, x => x.type)
来源：http://tsy.snrcjt.cn

[U110] JS：数组分块
来源：http://dkn.vqdsnc.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://uvf.yj20258888.top

[U111] JS：对象转 Map
来源：http://tld.jqgufenzy.top

new Map(Object.entries(obj))
来源：http://zar.feifeiyinyue.top

[U112] JS：字符串补位
来源：http://fbd.hammf.cn

"7".padStart(3, "0")
来源：http://afq.shangyingyoupin.top

[U113] JS：正则替换全部
来源：http://tcs.pengpengdd.cyou

s.replaceAll("a", "b")
来源：http://gbz.yuxming.cn

[U114] JS：JSON 深比较
来源：http://vxi.uphjek.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://nhc.fktsv.cn

[U115] JS：生成 UUID
来源：http://jqt.yuanzhike.top

crypto.randomUUID()
来源：http://bxv.bbcook.cn

[U116] JS：类型检查（JSDoc）
来源：http://dtr.aibaodan.cn

/** @param {string} name */ function f(name) {}
来源：http://kmd.redwolf501.top

[U117] JS：单元测试
来源：http://rqu.feifeiyinyue.top

npm i -D vitest;  npx vitest
来源：http://vma.jinqigfzy.top

[U118] JS：开发服务器
来源：http://qks.tanke756.top

npm i -D vite;  npx vite
来源：http://ksn.gaohongyu789.top

[U119] JS：生产构建
来源：http://txk.shanyushiyangkeji.top

npx vite build
来源：http://wgl.hysaishi.cn

[U120] JS：读取环境变量（Vite）
来源：http://cdp.sxryk.cn

import.meta.env.VITE_API_URL
来源：http://ted.hysaishi.cn

================================================================================
来源：http://whf.jinqigfzy.top

统计汇总
来源：http://njt.gaohongyu789.top

================================================================================
来源：http://eua.hnxiangtu.top

按语言统计（条）：
来源：http://tfy.sjlbkw.cn

Python ......... 252
来源：http://lbj.cdnleiting.top

PHP ............ 252
来源：http://rcl.zhixingplan.top

JavaScript ..... 252
来源：http://bzr.gzhubu.top

TypeScript ..... 212
来源：http://omj.zhijiandao.cn

Java ........... 212
来源：http://ksk.cqqwz.cn

Go ............. 212
来源：http://ckd.bbcook.cn

Ruby ........... 212
来源：http://bnf.gotoacloud.top

C# ............. 212
来源：http://dzu.ydjk.org.cn

C .............. 30
来源：http://tou.uphjek.com

C++ ............ 30
来源：http://qau.sweek.top

SQL ............ 90
来源：http://yms.ydzc1.top

Bash ........... 80
来源：http://had.vqdsnc.cn

Kotlin ......... 15
来源：http://zon.vehdjk.com

Swift .......... 15
来源：http://uec.hongshengwenyu.top

Lua ............ 10
来源：http://hoy.shanyushiyangkeji.top

Perl ........... 10
来源：http://cvc.cdnleiting.top

Scala .......... 10
来源：http://ozm.xziqi.cn

------------------------------------
来源：http://xpn.guowangkeji.top

合计 ........... 2106 条
来源：http://ura.shzxlz.cn

按章节统计：
来源：http://twt.zycfv.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qps.ivvv.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://knt.jqgfzy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lvi.birdmap.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xre.shangyingyoupin.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fjf.xziqi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pic.jinqigfzy.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://evx.cashguo.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ncz.yj202588.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://uuq.jinghuilouyu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jce.ivvv.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mwg.aizwys.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lnk.zhengqikj.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://cac.hnqzz.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vyf.aibaodan.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yfo.zhaomingkeji.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://gva.sjlbkw.cn

Q SQL 专题                              90
来源：http://mwz.snrcjt.cn

R Bash 专题                             80
来源：http://clk.ydjk.org.cn

S C / C++ 专题                          60
来源：http://yyi.sweek.top

T 其他语言补充                          60
来源：http://ude.xingfuxueyuan.xyz

U 高频实用片段                         120
来源：http://mld.smart0.xyz

------------------------------------
来源：http://ggr.cucudq.cn

合计                                  2106 条
来源：http://rdm.sjlbkw.cn

--------------------------------------------------------------------------------
来源：http://nds.jinqigufen.top

使用提醒
来源：http://iby.havefunace.top

--------------------------------------------------------------------------------
来源：http://ojc.quarkkingdee.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hpc.feifeiyinyue.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://and.ybcxt.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rip.guannengcc.top

在旧版本上使用前请先确认语法支持情况。
来源：http://ydy.sweek.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://uad.zhiwuduotai.top

—— 文件结束 ——
来源：http://uyi.chenjidiqi.icu

================================================================================
来源：http://irl.shuidangran.top

程序语言常见例子速查手册（2024 版）
来源：http://xpj.jlsjyb.cn

Common Programming Examples Cheat Book
来源：http://vns.feifeiyinyue.top

================================================================================
来源：http://ksl.svipenyu.cn

【收录内容】
来源：http://fzq.yongpay.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://wdi.jyoumei.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://osl.xylfe.cn

SQL · Bash · C · C++
来源：http://rpl.chenzaomai.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dxj.jiagoushi.top

【使用说明】
来源：http://zpb.yvedp.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hhp.yuxming.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://eob.chenlongwang.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://sji.52xcode.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://yli.yj202588.top

Bash:  Shell         C:     C             C++:   C++
来源：http://ddb.9152youxi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ljf.yangfankeji.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://lqu.0kj1m.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://lrp.yueranfly.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xup.jlsjyb.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://eva.zdbjq.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://gce.pengpengdd.cyou

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://yyw.jianghu66.top

【文件统计】
来源：http://qfo.gogol.net.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://dtx.xingfuxueyuan.xyz

--------------------------------------------------------------------------------
来源：http://goi.yfazqb.com

目  录
来源：http://rho.xinyue.icu

--------------------------------------------------------------------------------
来源：http://odr.9152youxi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ihq.ivvv.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://arv.aizwys.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://bdt.haohaochexian.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://xkc.ehwqpu.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mws.xziqi.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://kqx.zhiwuduotai.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://rgx.daria6918.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://gis.nanxinkj.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://pbw.hongshengwenyu.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ixb.mhx1999.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://cbs.zhongyouzk.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://pfx.chenzaomai.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://jgg.aizwys.cn


<!-- 参考信息 -->