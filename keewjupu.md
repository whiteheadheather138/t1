代发 wailian999

[U19] Py：正则替换带回调
来源：http://wma.jianghu66.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fia.bjfxy.top

[U20] Py：缓存函数结果
来源：http://cvb.jianghu66.top

@functools.lru_cache(maxsize=None)
来源：http://poo.xuetiantiany.cn

[U21] Py：自定义上下文管理器
来源：http://hug.shzxlz.cn

@contextlib.contextmanager
来源：http://uxb.xuanzx.com

[U22] Py：矩阵转置
来源：http://gjk.aibaodan.cn

list(zip(*m))
来源：http://nsw.uphjek.com

[U23] Py：分块读取大文件
来源：http://ktr.nanxuanxn.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jtw.xuanzx.com

[U24] Py：路径操作
来源：http://txj.xingfuxueyuan.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ohm.hywenlv.cn

[U25] Py：CSV 按字典读
来源：http://pki.tianlin.xyz

csv.DictReader(f)
来源：http://mkl.jyoumei.cn

[U26] Py：并发下载
来源：http://pbo.hnxiangtu.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gkf.316326.xyz

[U27] Py：异步 HTTP
来源：http://qwn.zdbjq.cn

aiohttp.ClientSession() 配合 async with
来源：http://uqg.ydjk.org.cn

[U28] Py：类型别名
来源：http://uyb.smart0.xyz

UserId = int
来源：http://bvo.xuanzx.com

[U29] Py：属性校验
来源：http://ufd.c1oappe.top

@property 与 @x.setter 配合
来源：http://tty.cqqwz.cn

[U30] Py：数据类
来源：http://wxs.hfpthk.cn

@dataclass(slots=True)
来源：http://pod.epnwcf.com

[U31] Py：单测
来源：http://qho.chenjidiqi.icu

python -m pytest -q
来源：http://xvy.wangshuangyany.cn

[U32] Py：代码格式化
来源：http://bty.hywenlv.cn

ruff format . && ruff check --fix .
来源：http://rct.yfazqb.com

[U33] Py：打包发布
来源：http://fed.chenlongwang.top

python -m build  （依赖 pyproject.toml）
来源：http://loa.ydjk.org.cn

[U34] Py：判断编码
来源：http://dex.jinqigfzy.top

chardet.detect(raw)
来源：http://koq.cheryme.top

[U35] Py：发送邮件
来源：http://bdx.9152youxi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jhd.wangdashe.top

[U36] Py：定时任务
来源：http://yzz.cashguo.top

schedule.every(10).minutes.do(job)
来源：http://qed.zhoulong.xyz

[U37] Py：读写 Excel
来源：http://fij.hfpthk.cn

pandas.read_excel / DataFrame.to_excel
来源：http://owj.9152youxi.cn

[U38] Py：获取脚本所在目录
来源：http://ois.shangyingyoupin.top

Path(__file__).resolve().parent
来源：http://dup.shuidangran.top

[U39] Py：判断是否在交互环境
来源：http://irb.andypj.xyz

sys.stdout.isatty()
来源：http://xft.haohaochexian.top

[U40] Py：打印到标准错误
来源：http://ndg.cashguo.top

print("err", file=sys.stderr)
来源：http://mji.sysykeji.top

[U41] PHP：初始化 Composer 项目
来源：http://dxh.svipenyu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://pla.zdqjudy.top

[U42] PHP：PSR-4 自动加载
来源：http://jlb.yj202588.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ejm.wangdashe.top

[U43] PHP：声明命名空间
来源：http://fuh.shangyingyoupin.top

namespace App\Http;
来源：http://iey.tianlin.xyz

[U44] PHP：开启严格类型
来源：http://moc.52xcode.cn

declare(strict_types=1);
来源：http://klt.nanxuanxn.top

[U45] PHP：类型声明与返回类型
来源：http://jsk.jinqigufen.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://isa.yongpay.top

[U46] PHP：可空类型
来源：http://lgs.yangfankeji.com

?string $name = null
来源：http://kgu.birdmap.top

[U47] PHP：联合类型
来源：http://etr.smart0.xyz

int|string $id
来源：http://rvz.yj20258888.top

[U48] PHP：纯枚举
来源：http://njk.zhongyouzk.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jty.ywan-chungtsiang.top

[U49] PHP：只读属性
来源：http://gxw.hesvh.cn

public readonly string $name
来源：http://ppy.daxiang520.top

[U50] PHP：构造器属性提升
来源：http://fsh.yuanzhike.top

public function __construct(private int $id) {}
来源：http://niz.jinyuanbaomall.cn

[U51] PHP：数组解构
来源：http://zxn.meibo888.top

[$a, $b] = $arr;
来源：http://ckf.jqgfzy.top

[U52] PHP：箭头函数
来源：http://ies.xinyue.icu

$double = fn($x) => $x * 2;
来源：http://whz.shanyushiyangtech.top

[U53] PHP：空合并运算符
来源：http://dim.vqdsnc.cn

$v = $a ?? $b ?? "default";
来源：http://xek.pycfn.com

[U54] PHP：空安全调用
来源：http://nyp.fzhhl.top

$obj?->method()
来源：http://pbm.vqdsnc.cn

[U55] PHP：match 表达式
来源：http://mze.tarul.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gwr.aibaodan.cn

[U56] PHP：命名参数
来源：http://ygv.hnqzz.top

f(a: 1, b: 2)
来源：http://kds.sysykeji.top

[U57] PHP：字符串插值
来源：http://klw.52xcode.cn

"值: {$a}"
来源：http://bru.fehbvm.com

[U58] PHP：数组三件套
来源：http://jsx.hysaishi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zcw.cheryme.top

[U59] PHP：自定义排序
来源：http://viz.sysykeji.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qzz.zdqjudy.top

[U60] PHP：JSON 编解码
来源：http://ayb.jqgufenzy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rpz.fengsongda.top

[U61] PHP：正则
来源：http://hkj.hnxiangtu.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mns.hesvh.cn

[U62] PHP：日期对象
来源：http://sty.fengsongda.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fuu.xylfe.cn

[U63] PHP：文件读写
来源：http://xnj.smart0.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://heg.ppjwa.cn

[U64] PHP：目录遍历
来源：http://nag.mhx1999.top

glob("dir/*.php");  scandir("dir");
来源：http://viv.ydzc1.top

[U65] PHP：会话
来源：http://atq.cqqwz.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://nyx.cashguo.top

[U66] PHP：设置 Cookie
来源：http://bub.fehbvm.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bgp.tarul.cn

[U67] PHP：处理文件上传
来源：http://kxg.tianlin.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ajj.gogol.net.cn

[U68] PHP：PDO 连接
来源：http://lrc.hnqzz.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lkr.gotoacloud.top

[U69] PHP：PDO 预处理
来源：http://nda.sxryk.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ahl.quarkkingdee.top

[U70] PHP：PDO 事务
来源：http://gvn.jlsjyb.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mno.cucudq.cn

[U71] PHP：抛出异常
来源：http://zne.guowangkeji.top

throw new RuntimeException("失败", 500);
来源：http://ryn.jianghu66.top

[U72] PHP：写错误日志
来源：http://imw.jinyuanbaomall.cn

error_log("失败: " . $e->getMessage());
来源：http://umw.0kj1m.cn

[U73] PHP：读取 ini 配置
来源：http://vwd.fktsv.cn

parse_ini_file("config.ini", true)
来源：http://ert.nanxuanxn.top

[U74] PHP：读取环境变量
来源：http://tut.316326.xyz

getenv("APP_ENV") ?: "production"
来源：http://msb.dashuyun.cn

[U75] PHP：依赖注入
来源：http://hqm.cucudq.cn

composer require psr/container
来源：http://evy.wangdashe.top

[U76] PHP：简单路由
来源：http://pts.hywenlv.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kiy.jinghuilouyu.cn

[U77] PHP：模板渲染
来源：http://gzi.jqgfzy.top

composer require twig/twig
来源：http://dup.xuanzx.com

[U78] PHP：单元测试
来源：http://yna.shanyushiyangkeji.top

composer require --dev phpunit/phpunit
来源：http://cmk.andypj.xyz

[U79] PHP：静态分析
来源：http://tvn.birdmap.top

composer require --dev phpstan/phpstan
来源：http://nsp.jianghu66.top

[U80] PHP：代码规范修复
来源：http://ets.aibaodan.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://aef.vehdjk.com

[U81] JS：初始化项目
来源：http://reb.jinghuilouyu.cn

npm init -y;  npm i express
来源：http://gsl.gotoacloud.top

[U82] JS：package.json 脚本
来源：http://ttl.guowangkeji.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hcs.vehdjk.com

[U83] JS：ES Module 导入导出
来源：http://ron.xziqi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://fml.yuxming.cn

[U84] JS：CommonJS 写法
来源：http://onv.bjfxy.top

module.exports = { a };  const { a } = require("./m");
来源：http://ljg.zhengqikj.top

[U85] JS：可选链
来源：http://fmp.dashuyun.cn

a?.b?.c
来源：http://muj.cqqwz.cn

[U86] JS：空值合并
来源：http://yke.bbcook.cn

a ?? b
来源：http://pjv.cucudq.cn

[U87] JS：解构默认值
来源：http://iqx.yuanzhike.top

const { a = 1, b = 2 } = obj;
来源：http://qwq.tarul.cn

[U88] JS：对象展开合并
来源：http://hcp.sjlbkw.cn

{ ...a, ...b }
来源：http://blo.ydjk.org.cn

[U89] JS：数组去重
来源：http://wns.cdnleiting.top

[...new Set(arr)]
来源：http://fbu.zhengqikj.top

[U90] JS：数字数组排序
来源：http://gqp.daxiang520.top

[...arr].sort((a, b) => a - b)
来源：http://kfz.zhijiandao.cn

[U91] JS：对象键值遍历
来源：http://odl.zhongyouzk.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tgs.xuanzx.com

[U92] JS：深拷贝
来源：http://tml.ydjk.org.cn

structuredClone(obj)
来源：http://xmh.yanxiufei.cn

[U93] JS：模板字符串
来源：http://nic.aibaodan.cn

`共 ${n} 条`
来源：http://ctc.yj202588.top

[U94] JS：箭头函数
来源：http://gpd.zdqjudy.top

const double = x => x * 2;
来源：http://tch.guannengcc.top

[U95] JS：Promise 包装
来源：http://azy.ydjk.org.cn

new Promise((resolve, reject) => {})
来源：http://gmh.xziqi.cn

[U96] JS：async/await 与异常
来源：http://jtl.chenlongwang.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lsb.shanyushiyangkeji.top

[U97] JS：并发请求
来源：http://szj.zhoulong.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://hls.guowangkeji.top

[U98] JS：fetch 带 JSON
来源：http://enu.ivvv.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ruk.pengpengdd.cyou

[U99] JS：事件监听
来源：http://ffz.yvedp.cn

el.addEventListener("click", e => {})
来源：http://wxk.hnxiangtu.top

[U100] JS：DOM 查询
来源：http://ptq.chenzaomai.com

document.querySelector(".item")
来源：http://yzp.hysaishi.cn

[U101] JS：classList 操作
来源：http://iep.yueranfly.top

el.classList.toggle("active")
来源：http://siq.uphjek.com

[U102] JS：本地存储
来源：http://alf.fktsv.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://rwr.nanxinkj.top

[U103] JS：定时器
来源：http://eiv.xingfuxueyuan.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nis.hcnkem.com

[U104] JS：防抖
来源：http://krz.jqgufenzy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pjh.gotoacloud.top

[U105] JS：节流
来源：http://zpy.yj20258888.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ile.shuidangran.top

[U106] JS：日期格式化
来源：http://jbv.gaohongyu789.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mow.cdnleiting.top

[U107] JS：数字千分位
来源：http://vrb.hnqzz.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ibo.havefunace.top

[U108] JS：随机整数
来源：http://eir.ybcxt.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://syl.nanxuanxn.top

[U109] JS：数组分组
来源：http://sfh.cqqwz.cn

Object.groupBy(arr, x => x.type)
来源：http://rei.sysykeji.top

[U110] JS：数组分块
来源：http://sno.hnxiangtu.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qnk.mhx1999.top

[U111] JS：对象转 Map
来源：http://tze.andypj.xyz

new Map(Object.entries(obj))
来源：http://uyx.nanxinkj.top

[U112] JS：字符串补位
来源：http://pgr.fzhhl.top

"7".padStart(3, "0")
来源：http://xyf.yfazqb.com

[U113] JS：正则替换全部
来源：http://eqn.0kj1m.cn

s.replaceAll("a", "b")
来源：http://kim.meibo888.top

[U114] JS：JSON 深比较
来源：http://tcr.snrcjt.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://yuh.c1oappe.top

[U115] JS：生成 UUID
来源：http://prv.jqgfzy.top

crypto.randomUUID()
来源：http://wxf.jinqigufen.top

[U116] JS：类型检查（JSDoc）
来源：http://azg.fanxiaobao.xyz

/** @param {string} name */ function f(name) {}
来源：http://htx.cashguo.top

[U117] JS：单元测试
来源：http://dqg.yj20258888.top

npm i -D vitest;  npx vitest
来源：http://mbl.vqdsnc.cn

[U118] JS：开发服务器
来源：http://efm.hongshengwenyu.top

npm i -D vite;  npx vite
来源：http://wpo.zhengqikj.top

[U119] JS：生产构建
来源：http://vaw.yuxming.cn

npx vite build
来源：http://lqk.zhixingplan.top

[U120] JS：读取环境变量（Vite）
来源：http://fsa.jlsjyb.cn

import.meta.env.VITE_API_URL
来源：http://amx.xuanzx.com

================================================================================
来源：http://mlu.xuetiantiany.cn

统计汇总
来源：http://thf.yangfankeji.com

================================================================================
来源：http://uea.pengpengdd.cyou

按语言统计（条）：
来源：http://mbi.zhiwuduotai.top

Python ......... 252
来源：http://edn.dashuyun.cn

PHP ............ 252
来源：http://wpd.sweek.top

JavaScript ..... 252
来源：http://ljr.jinqigufen.top

TypeScript ..... 212
来源：http://rzx.xingfuxueyuan.xyz

Java ........... 212
来源：http://lcx.pengpengdd.cyou

Go ............. 212
来源：http://rkx.zhaomingkeji.xyz

Ruby ........... 212
来源：http://lip.kuanghao11.cn

C# ............. 212
来源：http://nki.smart0.xyz

C .............. 30
来源：http://cvq.shanyushiyangtech.top

C++ ............ 30
来源：http://eok.sjlbkw.cn

SQL ............ 90
来源：http://rjq.gotoacloud.top

Bash ........... 80
来源：http://syf.hfpthk.cn

Kotlin ......... 15
来源：http://xbi.guannengcc.top

Swift .......... 15
来源：http://wlm.nanxuanxn.top

Lua ............ 10
来源：http://ier.feifeiyinyue.top

Perl ........... 10
来源：http://wha.zhixingplan.top

Scala .......... 10
来源：http://xkm.ydzc1.top

------------------------------------
来源：http://zdq.birdmap.top

合计 ........... 2106 条
来源：http://mql.dashuyun.cn

按章节统计：
来源：http://ddh.pycfn.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qyu.ydzc1.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ths.zdbjq.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://apg.zhixingplan.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qnb.mhx1999.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ssk.hfpthk.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://sdc.cqqwz.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://lbs.zhaomingkeji.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xfx.nanxuanxn.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://pyc.zhaomingkeji.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ufb.gaohongyu789.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xnt.daxiang520.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dro.ivvv.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://xle.hnxiangtu.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://xpa.vehdjk.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vnd.ydjk.org.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xcs.yangfankeji.com

Q SQL 专题                              90
来源：http://yxq.xziqi.cn

R Bash 专题                             80
来源：http://xjw.gogol.net.cn

S C / C++ 专题                          60
来源：http://pqf.ppjwa.cn

T 其他语言补充                          60
来源：http://xoe.52xcode.cn

U 高频实用片段                         120
来源：http://szu.cheryme.top

------------------------------------
来源：http://iaa.yuxming.cn

合计                                  2106 条
来源：http://oly.snrcjt.cn

--------------------------------------------------------------------------------
来源：http://eju.quarkkingdee.top

使用提醒
来源：http://vny.gzhubu.top

--------------------------------------------------------------------------------
来源：http://zus.sysykeji.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://rsj.chenzaomai.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ssf.wangdashe.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://lvh.pengpengdd.cyou

在旧版本上使用前请先确认语法支持情况。
来源：http://tia.hywenlv.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://eub.fehbvm.com

—— 文件结束 ——
来源：http://wai.guowangkeji.top

================================================================================
来源：http://jtx.nanxuanxn.top

程序语言常见例子速查手册（2024 版）
来源：http://qgr.yuanzhike.top

Common Programming Examples Cheat Book
来源：http://ckm.ctjpmb.com

================================================================================
来源：http://vdm.zhijiandao.cn

【收录内容】
来源：http://otk.vqdsnc.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://jxm.gaohongyu789.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xyw.gzhubu.top

SQL · Bash · C · C++
来源：http://evj.jiagoushi.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://lrx.tian-w.cn

【使用说明】
来源：http://vpc.fanxiaobao.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ngd.fehbvm.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://cua.zhixingplan.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://gvv.shanyushiyangtech.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://lix.cashguo.top

Bash:  Shell         C:     C             C++:   C++
来源：http://tzv.daxiang520.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zav.wangdashe.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mkv.smart0.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xeo.svipenyu.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jbq.chenzaomai.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://eqy.kuanghao11.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vlw.ctjpmb.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wkp.c1oappe.top

【文件统计】
来源：http://bxv.shanyushiyangtech.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rev.zdqjudy.top

--------------------------------------------------------------------------------
来源：http://ukj.hysaishi.cn

目  录
来源：http://vwn.sufxvd.cn

--------------------------------------------------------------------------------
来源：http://toi.zhoulong.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://seh.hysaishi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wfd.yongpay.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ewi.sufxvd.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ryr.ydjk.org.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qbe.zhaomingkeji.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://erb.fengsongda.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hpp.haohaochexian.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://auv.yangfankeji.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wpm.kuanghao11.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://aur.yongpay.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hqx.haohaochexian.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://eep.jyoumei.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xcu.gaohongyu789.top


<!-- 参考信息 -->