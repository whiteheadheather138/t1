代发 wailian999

[U19] Py：正则替换带回调
来源：http://jpy.havefunace.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jfg.bjfxy.top

[U20] Py：缓存函数结果
来源：http://skl.sufxvd.cn

@functools.lru_cache(maxsize=None)
来源：http://pla.zhixingplan.top

[U21] Py：自定义上下文管理器
来源：http://ido.zhijiandao.cn

@contextlib.contextmanager
来源：http://grf.aizwys.cn

[U22] Py：矩阵转置
来源：http://inw.ctjpmb.com

list(zip(*m))
来源：http://fng.xuanzx.com

[U23] Py：分块读取大文件
来源：http://rkt.shanyushiyangtech.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gdr.ctjpmb.com

[U24] Py：路径操作
来源：http://mzq.daria6918.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nif.xuetiantiany.cn

[U25] Py：CSV 按字典读
来源：http://oav.yuanzhike.top

csv.DictReader(f)
来源：http://hxe.zhijiandao.cn

[U26] Py：并发下载
来源：http://hgf.sweek.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://kov.uphjek.com

[U27] Py：异步 HTTP
来源：http://gxn.sxryk.cn

aiohttp.ClientSession() 配合 async with
来源：http://zan.ydzc1.top

[U28] Py：类型别名
来源：http://kst.sjlbkw.cn

UserId = int
来源：http://vwd.sjlbkw.cn

[U29] Py：属性校验
来源：http://znu.xinyue.icu

@property 与 @x.setter 配合
来源：http://bgx.ehwqpu.com

[U30] Py：数据类
来源：http://zlp.guowangkeji.top

@dataclass(slots=True)
来源：http://cgz.tian-w.cn

[U31] Py：单测
来源：http://bvj.ppjwa.cn

python -m pytest -q
来源：http://tii.zhiwuduotai.top

[U32] Py：代码格式化
来源：http://lte.chenzaomai.com

ruff format . && ruff check --fix .
来源：http://hht.svipenyu.cn

[U33] Py：打包发布
来源：http://khw.ydzc1.top

python -m build  （依赖 pyproject.toml）
来源：http://dzs.jqgufenzy.top

[U34] Py：判断编码
来源：http://hfg.shanyushiyangkeji.top

chardet.detect(raw)
来源：http://jle.hywenlv.cn

[U35] Py：发送邮件
来源：http://ozc.tarul.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gmq.hywenlv.cn

[U36] Py：定时任务
来源：http://foi.sysykeji.top

schedule.every(10).minutes.do(job)
来源：http://itk.yfazqb.com

[U37] Py：读写 Excel
来源：http://wuz.sufxvd.cn

pandas.read_excel / DataFrame.to_excel
来源：http://hmo.hcnkem.com

[U38] Py：获取脚本所在目录
来源：http://wae.xingfuxueyuan.xyz

Path(__file__).resolve().parent
来源：http://qty.xingfuxueyuan.xyz

[U39] Py：判断是否在交互环境
来源：http://xqx.shangyingyoupin.top

sys.stdout.isatty()
来源：http://lio.jlsjyb.cn

[U40] Py：打印到标准错误
来源：http://cdl.sxryk.cn

print("err", file=sys.stderr)
来源：http://gfj.sjlbkw.cn

[U41] PHP：初始化 Composer 项目
来源：http://fnx.fktsv.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://kph.ppjwa.cn

[U42] PHP：PSR-4 自动加载
来源：http://ljh.zhixingplan.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cpw.yueranfly.top

[U43] PHP：声明命名空间
来源：http://scx.yongpay.top

namespace App\Http;
来源：http://mnf.sufxvd.cn

[U44] PHP：开启严格类型
来源：http://iqu.daxiang520.top

declare(strict_types=1);
来源：http://win.yfazqb.com

[U45] PHP：类型声明与返回类型
来源：http://sjh.zhoulong.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://crt.hywenlv.cn

[U46] PHP：可空类型
来源：http://cmt.hfpthk.cn

?string $name = null
来源：http://mpy.aibaodan.cn

[U47] PHP：联合类型
来源：http://jur.dashuyun.cn

int|string $id
来源：http://trv.fehbvm.com

[U48] PHP：纯枚举
来源：http://xkw.havefunace.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ydg.xuanzx.com

[U49] PHP：只读属性
来源：http://isg.0kj1m.cn

public readonly string $name
来源：http://lfc.guowangkeji.top

[U50] PHP：构造器属性提升
来源：http://hmc.daxiang520.top

public function __construct(private int $id) {}
来源：http://vke.xuetiantiany.cn

[U51] PHP：数组解构
来源：http://jaq.zhaomingkeji.xyz

[$a, $b] = $arr;
来源：http://hrl.zhiwuduotai.top

[U52] PHP：箭头函数
来源：http://srw.jinyuanbaomall.cn

$double = fn($x) => $x * 2;
来源：http://qvm.xinyue.icu

[U53] PHP：空合并运算符
来源：http://xkc.hesvh.cn

$v = $a ?? $b ?? "default";
来源：http://nbr.tarul.cn

[U54] PHP：空安全调用
来源：http://abc.meibo888.top

$obj?->method()
来源：http://lst.fzhhl.top

[U55] PHP：match 表达式
来源：http://hho.yonumen.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://iiq.shangyingyoupin.top

[U56] PHP：命名参数
来源：http://zsp.redwolf501.top

f(a: 1, b: 2)
来源：http://tee.hnqzz.top

[U57] PHP：字符串插值
来源：http://pim.fengsongda.top

"值: {$a}"
来源：http://aae.zdqjudy.top

[U58] PHP：数组三件套
来源：http://aei.shanyushiyangkeji.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fpn.wangshuangyany.cn

[U59] PHP：自定义排序
来源：http://bao.dianchejie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pya.cashguo.top

[U60] PHP：JSON 编解码
来源：http://glh.yuanzhike.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fke.hywenlv.cn

[U61] PHP：正则
来源：http://pda.haohaochexian.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kbt.ybcxt.top

[U62] PHP：日期对象
来源：http://pud.sjlbkw.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pnn.yuxming.cn

[U63] PHP：文件读写
来源：http://bmt.52xcode.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xsy.vehdjk.com

[U64] PHP：目录遍历
来源：http://jmo.nanxuanxn.top

glob("dir/*.php");  scandir("dir");
来源：http://yxs.hesvh.cn

[U65] PHP：会话
来源：http://qym.meibo888.top

session_start();  $_SESSION["uid"] = 1;
来源：http://gjv.dashuyun.cn

[U66] PHP：设置 Cookie
来源：http://emo.hnxiangtu.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wlf.chenlongwang.top

[U67] PHP：处理文件上传
来源：http://whl.jiagoushi.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rqm.sjlbkw.cn

[U68] PHP：PDO 连接
来源：http://gur.yvedp.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kyk.tian-w.cn

[U69] PHP：PDO 预处理
来源：http://rvk.dashuyun.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xba.gzhubu.top

[U70] PHP：PDO 事务
来源：http://bmk.gaohongyu789.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jro.zhengqikj.top

[U71] PHP：抛出异常
来源：http://kjy.yueranfly.top

throw new RuntimeException("失败", 500);
来源：http://gsp.cashguo.top

[U72] PHP：写错误日志
来源：http://vwk.ivvv.top

error_log("失败: " . $e->getMessage());
来源：http://uzs.fktsv.cn

[U73] PHP：读取 ini 配置
来源：http://eny.xingfuxueyuan.xyz

parse_ini_file("config.ini", true)
来源：http://upi.xuetiantiany.cn

[U74] PHP：读取环境变量
来源：http://erb.chenzaomai.com

getenv("APP_ENV") ?: "production"
来源：http://sba.jinghuilouyu.cn

[U75] PHP：依赖注入
来源：http://ryr.52xcode.cn

composer require psr/container
来源：http://rtb.hfpthk.cn

[U76] PHP：简单路由
来源：http://rho.shanyushiyangtech.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xiw.zhiwuduotai.top

[U77] PHP：模板渲染
来源：http://phx.tarul.cn

composer require twig/twig
来源：http://eir.zhaomingkeji.xyz

[U78] PHP：单元测试
来源：http://ple.chenzaomai.com

composer require --dev phpunit/phpunit
来源：http://uau.svipenyu.cn

[U79] PHP：静态分析
来源：http://qgx.feifeiyinyue.top

composer require --dev phpstan/phpstan
来源：http://dry.yonumen.top

[U80] PHP：代码规范修复
来源：http://cwy.52xcode.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://hnc.quarkkingdee.top

[U81] JS：初始化项目
来源：http://gqs.daria6918.cn

npm init -y;  npm i express
来源：http://utv.jiagoushi.top

[U82] JS：package.json 脚本
来源：http://ngy.gzhubu.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pmg.hcnkem.com

[U83] JS：ES Module 导入导出
来源：http://oqx.hywenlv.cn

export const a = 1;  import { a } from "./m.js";
来源：http://rhh.shangyingyoupin.top

[U84] JS：CommonJS 写法
来源：http://ain.cqqwz.cn

module.exports = { a };  const { a } = require("./m");
来源：http://bkh.wangdashe.top

[U85] JS：可选链
来源：http://lej.pycfn.com

a?.b?.c
来源：http://fax.yanxiufei.cn

[U86] JS：空值合并
来源：http://nxw.ivvv.top

a ?? b
来源：http://swl.yvedp.cn

[U87] JS：解构默认值
来源：http://tyh.fengsongda.top

const { a = 1, b = 2 } = obj;
来源：http://grp.hywenlv.cn

[U88] JS：对象展开合并
来源：http://ssp.cucudq.cn

{ ...a, ...b }
来源：http://bas.yueranfly.top

[U89] JS：数组去重
来源：http://amu.gaohongyu789.top

[...new Set(arr)]
来源：http://ifp.guannengcc.top

[U90] JS：数字数组排序
来源：http://oro.jinqigfzy.top

[...arr].sort((a, b) => a - b)
来源：http://zzi.cdnleiting.top

[U91] JS：对象键值遍历
来源：http://vbe.mhx1999.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nww.yanxiufei.cn

[U92] JS：深拷贝
来源：http://yvm.zdqjudy.top

structuredClone(obj)
来源：http://oes.nanxinkj.top

[U93] JS：模板字符串
来源：http://qnc.yangfankeji.com

`共 ${n} 条`
来源：http://smv.bbcook.cn

[U94] JS：箭头函数
来源：http://qkm.uphjek.com

const double = x => x * 2;
来源：http://wzg.svipenyu.cn

[U95] JS：Promise 包装
来源：http://szk.hesvh.cn

new Promise((resolve, reject) => {})
来源：http://vtb.hesvh.cn

[U96] JS：async/await 与异常
来源：http://auj.smart0.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cri.guannengcc.top

[U97] JS：并发请求
来源：http://lfr.fanxiaobao.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://axh.nanxinkj.top

[U98] JS：fetch 带 JSON
来源：http://tgs.wangdashe.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wsw.wangdashe.top

[U99] JS：事件监听
来源：http://kch.yj20258.top

el.addEventListener("click", e => {})
来源：http://nux.vqdsnc.cn

[U100] JS：DOM 查询
来源：http://riy.pengpengdd.cyou

document.querySelector(".item")
来源：http://lvu.tianlin.xyz

[U101] JS：classList 操作
来源：http://sbq.jianghu66.top

el.classList.toggle("active")
来源：http://hpl.nanxinkj.top

[U102] JS：本地存储
来源：http://bei.sysykeji.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ojn.shanyushiyangkeji.top

[U103] JS：定时器
来源：http://qnk.9152youxi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jkf.fanxiaobao.xyz

[U104] JS：防抖
来源：http://zmg.shanyushiyangtech.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hge.kuanghao11.cn

[U105] JS：节流
来源：http://gzc.xinyue.icu

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://iqj.yanxiufei.cn

[U106] JS：日期格式化
来源：http://arr.hesvh.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://eyi.zhengqikj.top

[U107] JS：数字千分位
来源：http://rrv.jianghu66.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hom.jyoumei.cn

[U108] JS：随机整数
来源：http://rfb.wangdashe.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://eto.jqgfzy.top

[U109] JS：数组分组
来源：http://jxg.ppjwa.cn

Object.groupBy(arr, x => x.type)
来源：http://rxz.yvedp.cn

[U110] JS：数组分块
来源：http://lwv.cucudq.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://viy.fanxiaobao.xyz

[U111] JS：对象转 Map
来源：http://bfl.redwolf501.top

new Map(Object.entries(obj))
来源：http://gpa.yangfankeji.com

[U112] JS：字符串补位
来源：http://nsq.vehdjk.com

"7".padStart(3, "0")
来源：http://euk.uphjek.com

[U113] JS：正则替换全部
来源：http://hml.wangshuangyany.cn

s.replaceAll("a", "b")
来源：http://jsu.zhengqikj.top

[U114] JS：JSON 深比较
来源：http://mrd.svipenyu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://fdr.vqdsnc.cn

[U115] JS：生成 UUID
来源：http://oge.hongshengwenyu.top

crypto.randomUUID()
来源：http://xme.fengsongda.top

[U116] JS：类型检查（JSDoc）
来源：http://plu.cashguo.top

/** @param {string} name */ function f(name) {}
来源：http://fmw.ybcxt.top

[U117] JS：单元测试
来源：http://zqh.daria6918.cn

npm i -D vitest;  npx vitest
来源：http://sax.feifeiyinyue.top

[U118] JS：开发服务器
来源：http://mvd.quarkkingdee.top

npm i -D vite;  npx vite
来源：http://qvj.zdqjudy.top

[U119] JS：生产构建
来源：http://kwv.ivvv.top

npx vite build
来源：http://yak.jyoumei.cn

[U120] JS：读取环境变量（Vite）
来源：http://cwa.bjfxy.top

import.meta.env.VITE_API_URL
来源：http://sta.ydzc1.top

================================================================================
来源：http://kcv.iojbl.cn

统计汇总
来源：http://gei.zhixingplan.top

================================================================================
来源：http://uok.aibaodan.cn

按语言统计（条）：
来源：http://lrm.wangdashe.top

Python ......... 252
来源：http://sio.shuidangran.top

PHP ............ 252
来源：http://jiw.zhongyouzk.top

JavaScript ..... 252
来源：http://acg.svipenyu.cn

TypeScript ..... 212
来源：http://qqp.sweek.top

Java ........... 212
来源：http://gzc.jianghu66.top

Go ............. 212
来源：http://wvt.ppjwa.cn

Ruby ........... 212
来源：http://jkc.jqgfzy.top

C# ............. 212
来源：http://nop.jyoumei.cn

C .............. 30
来源：http://wof.quarkkingdee.top

C++ ............ 30
来源：http://dwt.svipenyu.cn

SQL ............ 90
来源：http://vzb.yfazqb.com

Bash ........... 80
来源：http://tiz.hammf.cn

Kotlin ......... 15
来源：http://kum.zhoulong.xyz

Swift .......... 15
来源：http://qdf.fengsongda.top

Lua ............ 10
来源：http://tzn.guowangkeji.top

Perl ........... 10
来源：http://dor.xuanzx.com

Scala .......... 10
来源：http://cgb.gzhubu.top

------------------------------------
来源：http://yyz.316326.xyz

合计 ........... 2106 条
来源：http://fau.tarul.cn

按章节统计：
来源：http://nmo.daxiang520.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://epu.iojbl.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zml.fzhhl.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gdy.hcnkem.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xyx.guowangkeji.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fsu.shzxlz.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ufl.chenzaomai.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xgu.feifeiyinyue.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nnw.bbcook.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://dzr.yuanzhike.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yta.yj20258.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://eas.snrcjt.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cez.sufxvd.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rfg.jyoumei.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://umg.jyoumei.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://iwr.jinqigufen.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://kzg.zhixingplan.top

Q SQL 专题                              90
来源：http://kuu.fanxiaobao.xyz

R Bash 专题                             80
来源：http://ykx.xylfe.cn

S C / C++ 专题                          60
来源：http://nqi.jianghu66.top

T 其他语言补充                          60
来源：http://ikg.zhiwuduotai.top

U 高频实用片段                         120
来源：http://jox.dashuyun.cn

------------------------------------
来源：http://bgh.hysaishi.cn

合计                                  2106 条
来源：http://okf.316326.xyz

--------------------------------------------------------------------------------
来源：http://zzi.tarul.cn

使用提醒
来源：http://nfj.fengsongda.top

--------------------------------------------------------------------------------
来源：http://eno.jiagoushi.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vwx.vehdjk.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://dns.ydjk.org.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://iyv.fengsongda.top

在旧版本上使用前请先确认语法支持情况。
来源：http://lvw.hysaishi.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://fpk.wangshuangyany.cn

—— 文件结束 ——
来源：http://kpm.hysaishi.cn

================================================================================
来源：http://jvj.ybcxt.top

程序语言常见例子速查手册（2024 版）
来源：http://nkd.uphjek.com

Common Programming Examples Cheat Book
来源：http://fqd.shanyushiyangkeji.top

================================================================================
来源：http://cll.jqgfzy.top

【收录内容】
来源：http://lhe.hcnkem.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://qrm.fanxiaobao.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jps.jqgfzy.top

SQL · Bash · C · C++
来源：http://uqi.bbcook.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://pyf.xinyue.icu

【使用说明】
来源：http://nxi.yonumen.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://rdl.mhx1999.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://bam.yj20258888.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://gtl.cucudq.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vtg.yongpay.top

Bash:  Shell         C:     C             C++:   C++
来源：http://uwe.fanxiaobao.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://nbp.jqgufenzy.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://zxd.hesvh.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://bfm.ppjwa.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://tlo.shzxlz.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://amf.guowangkeji.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bky.cashguo.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://bhq.guannengcc.top

【文件统计】
来源：http://onq.sufxvd.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://pzh.guowangkeji.top

--------------------------------------------------------------------------------
来源：http://rvp.tian-w.cn

目  录
来源：http://xlo.jlsjyb.cn

--------------------------------------------------------------------------------
来源：http://ioz.xingfuxueyuan.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://vyd.wangdashe.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ylx.sysykeji.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://nrm.hammf.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://kev.yueranfly.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://kxx.zdbjq.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xdt.shangyingyoupin.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://jbp.xuetiantiany.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://dhy.sufxvd.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://irv.fehbvm.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://prj.hammf.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://idd.0kj1m.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://lky.epnwcf.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mrh.cashguo.top


<!-- 参考信息 -->