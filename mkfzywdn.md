代发 wailian999

[U23] Py：分块读取大文件
来源：http://vqv.zhongyouzk.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mrx.pengpengdd.cyou

[U24] Py：路径操作
来源：http://xmt.pycfn.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mvs.fehbvm.com

[U25] Py：CSV 按字典读
来源：http://lwq.cashguo.top

csv.DictReader(f)
来源：http://dnc.uphjek.com

[U26] Py：并发下载
来源：http://enh.yfazqb.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nmf.cqqwz.cn

[U27] Py：异步 HTTP
来源：http://oru.yongpay.top

aiohttp.ClientSession() 配合 async with
来源：http://ehj.kuanghao11.cn

[U28] Py：类型别名
来源：http://oqa.epnwcf.com

UserId = int
来源：http://yan.fzhhl.top

[U29] Py：属性校验
来源：http://rjm.zhijiandao.cn

@property 与 @x.setter 配合
来源：http://kjk.yj20258.top

[U30] Py：数据类
来源：http://wac.shangyingyoupin.top

@dataclass(slots=True)
来源：http://wwx.0kj1m.cn

[U31] Py：单测
来源：http://iby.hysaishi.cn

python -m pytest -q
来源：http://zin.dianchejie.cn

[U32] Py：代码格式化
来源：http://skp.sjlbkw.cn

ruff format . && ruff check --fix .
来源：http://ufy.hysaishi.cn

[U33] Py：打包发布
来源：http://bot.sufxvd.cn

python -m build  （依赖 pyproject.toml）
来源：http://mqn.chenjidiqi.icu

[U34] Py：判断编码
来源：http://wbg.jinqigfzy.top

chardet.detect(raw)
来源：http://lqa.tarul.cn

[U35] Py：发送邮件
来源：http://jvc.zhijiandao.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://svh.chenzaomai.com

[U36] Py：定时任务
来源：http://jor.birdmap.top

schedule.every(10).minutes.do(job)
来源：http://rpg.hywenlv.cn

[U37] Py：读写 Excel
来源：http://ukk.hnqzz.top

pandas.read_excel / DataFrame.to_excel
来源：http://dfg.ivvv.top

[U38] Py：获取脚本所在目录
来源：http://gor.fehbvm.com

Path(__file__).resolve().parent
来源：http://pcp.svipenyu.cn

[U39] Py：判断是否在交互环境
来源：http://amz.nanxuanxn.top

sys.stdout.isatty()
来源：http://jfb.hongshengwenyu.top

[U40] Py：打印到标准错误
来源：http://cnu.hysaishi.cn

print("err", file=sys.stderr)
来源：http://iid.fehbvm.com

[U41] PHP：初始化 Composer 项目
来源：http://swe.yuanzhike.top

composer init;  composer require guzzlehttp/guzzle
来源：http://bix.hywenlv.cn

[U42] PHP：PSR-4 自动加载
来源：http://yjq.daxiang520.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mmm.yueranfly.top

[U43] PHP：声明命名空间
来源：http://wzh.hnxiangtu.top

namespace App\Http;
来源：http://gul.dashuyun.cn

[U44] PHP：开启严格类型
来源：http://bby.jiagoushi.top

declare(strict_types=1);
来源：http://gam.chenlongwang.top

[U45] PHP：类型声明与返回类型
来源：http://bme.jinghuilouyu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://fyr.ybcxt.top

[U46] PHP：可空类型
来源：http://yal.meibo888.top

?string $name = null
来源：http://lbp.yueranfly.top

[U47] PHP：联合类型
来源：http://ylo.jlsjyb.cn

int|string $id
来源：http://uah.daria6918.cn

[U48] PHP：纯枚举
来源：http://lro.fktsv.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tcp.bbcook.cn

[U49] PHP：只读属性
来源：http://rlx.tianlin.xyz

public readonly string $name
来源：http://wxf.nwbrower.top

[U50] PHP：构造器属性提升
来源：http://mkb.bjfxy.top

public function __construct(private int $id) {}
来源：http://gwe.nanxuanxn.top

[U51] PHP：数组解构
来源：http://lth.andypj.xyz

[$a, $b] = $arr;
来源：http://nfe.gzhubu.top

[U52] PHP：箭头函数
来源：http://ryz.fehbvm.com

$double = fn($x) => $x * 2;
来源：http://zqm.epnwcf.com

[U53] PHP：空合并运算符
来源：http://ynx.yangfankeji.com

$v = $a ?? $b ?? "default";
来源：http://jhp.zhiwuduotai.top

[U54] PHP：空安全调用
来源：http://tbo.meibo888.top

$obj?->method()
来源：http://qrh.guowangkeji.top

[U55] PHP：match 表达式
来源：http://cxn.sjlbkw.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ebb.ywan-chungtsiang.top

[U56] PHP：命名参数
来源：http://xvx.tanke756.top

f(a: 1, b: 2)
来源：http://mad.jlsjyb.cn

[U57] PHP：字符串插值
来源：http://xyu.cheryme.top

"值: {$a}"
来源：http://wym.xuetiantiany.cn

[U58] PHP：数组三件套
来源：http://kgy.yuxming.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://tea.guowangkeji.top

[U59] PHP：自定义排序
来源：http://iut.0kj1m.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ubj.hongshengwenyu.top

[U60] PHP：JSON 编解码
来源：http://ian.316326.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hut.guowangkeji.top

[U61] PHP：正则
来源：http://iuk.daxiang520.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://iqv.jlsjyb.cn

[U62] PHP：日期对象
来源：http://wkf.sysykeji.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bbq.wangdashe.top

[U63] PHP：文件读写
来源：http://sdy.jinqigufen.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://clg.yueranfly.top

[U64] PHP：目录遍历
来源：http://gfi.pengpengdd.cyou

glob("dir/*.php");  scandir("dir");
来源：http://ukp.chenjidiqi.icu

[U65] PHP：会话
来源：http://mli.nanxinkj.top

session_start();  $_SESSION["uid"] = 1;
来源：http://vja.uphjek.com

[U66] PHP：设置 Cookie
来源：http://vfc.jinqigfzy.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mfz.wangdashe.top

[U67] PHP：处理文件上传
来源：http://rba.jinyuanbaomall.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pod.ctjpmb.com

[U68] PHP：PDO 连接
来源：http://eot.tian-w.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://cri.sweek.top

[U69] PHP：PDO 预处理
来源：http://hiu.zhixingplan.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zrc.gotoacloud.top

[U70] PHP：PDO 事务
来源：http://ojl.dianchejie.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tpc.sysykeji.top

[U71] PHP：抛出异常
来源：http://faz.xinyue.icu

throw new RuntimeException("失败", 500);
来源：http://rsg.xziqi.cn

[U72] PHP：写错误日志
来源：http://euk.yangfankeji.com

error_log("失败: " . $e->getMessage());
来源：http://ymw.jianghu66.top

[U73] PHP：读取 ini 配置
来源：http://gjt.nanxuanxn.top

parse_ini_file("config.ini", true)
来源：http://gmt.yanxiufei.cn

[U74] PHP：读取环境变量
来源：http://ndt.ppjwa.cn

getenv("APP_ENV") ?: "production"
来源：http://mhk.guannengcc.top

[U75] PHP：依赖注入
来源：http://ogy.xziqi.cn

composer require psr/container
来源：http://qyx.chenjidiqi.icu

[U76] PHP：简单路由
来源：http://ita.tarul.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://nrf.yongpay.top

[U77] PHP：模板渲染
来源：http://lxz.ydzc1.top

composer require twig/twig
来源：http://eoy.wangshuangyany.cn

[U78] PHP：单元测试
来源：http://xsv.hfpthk.cn

composer require --dev phpunit/phpunit
来源：http://mpz.yuxming.cn

[U79] PHP：静态分析
来源：http://vym.sufxvd.cn

composer require --dev phpstan/phpstan
来源：http://xpc.xinyue.icu

[U80] PHP：代码规范修复
来源：http://gqn.shanyushiyangkeji.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://wxq.sufxvd.cn

[U81] JS：初始化项目
来源：http://ask.nanxuanxn.top

npm init -y;  npm i express
来源：http://jgz.hnxiangtu.top

[U82] JS：package.json 脚本
来源：http://tat.gotoacloud.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bde.zycfv.cn

[U83] JS：ES Module 导入导出
来源：http://cvq.jinqigfzy.top

export const a = 1;  import { a } from "./m.js";
来源：http://cen.zhiwuduotai.top

[U84] JS：CommonJS 写法
来源：http://ttr.yj20258888.top

module.exports = { a };  const { a } = require("./m");
来源：http://iof.pycfn.com

[U85] JS：可选链
来源：http://bgs.hnxiangtu.top

a?.b?.c
来源：http://nwt.uphjek.com

[U86] JS：空值合并
来源：http://tyf.zhengqikj.top

a ?? b
来源：http://ilb.jqgfzy.top

[U87] JS：解构默认值
来源：http://ztc.havefunace.top

const { a = 1, b = 2 } = obj;
来源：http://tkh.epnwcf.com

[U88] JS：对象展开合并
来源：http://iuz.uphjek.com

{ ...a, ...b }
来源：http://ted.uphjek.com

[U89] JS：数组去重
来源：http://nac.shanyushiyangkeji.top

[...new Set(arr)]
来源：http://whn.zdbjq.cn

[U90] JS：数字数组排序
来源：http://vvi.sxryk.cn

[...arr].sort((a, b) => a - b)
来源：http://rwt.cqqwz.cn

[U91] JS：对象键值遍历
来源：http://ydt.jinyuanbaomall.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hvw.tian-w.cn

[U92] JS：深拷贝
来源：http://obm.quarkkingdee.top

structuredClone(obj)
来源：http://qrz.gaohongyu789.top

[U93] JS：模板字符串
来源：http://jwg.cheryme.top

`共 ${n} 条`
来源：http://qbh.fehbvm.com

[U94] JS：箭头函数
来源：http://qkr.ehwqpu.com

const double = x => x * 2;
来源：http://bis.svipenyu.cn

[U95] JS：Promise 包装
来源：http://toq.cashguo.top

new Promise((resolve, reject) => {})
来源：http://gzj.chenlongwang.top

[U96] JS：async/await 与异常
来源：http://uxd.fktsv.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fzu.fktsv.cn

[U97] JS：并发请求
来源：http://unk.iojbl.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://lws.cashguo.top

[U98] JS：fetch 带 JSON
来源：http://abm.smart0.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gce.sjlbkw.cn

[U99] JS：事件监听
来源：http://piw.yfazqb.com

el.addEventListener("click", e => {})
来源：http://zvi.hongshengwenyu.top

[U100] JS：DOM 查询
来源：http://pdr.xinyue.icu

document.querySelector(".item")
来源：http://ysl.zhoulong.xyz

[U101] JS：classList 操作
来源：http://kil.haohaochexian.top

el.classList.toggle("active")
来源：http://mvm.yuxming.cn

[U102] JS：本地存储
来源：http://jat.shanyushiyangtech.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://any.yuanzhike.top

[U103] JS：定时器
来源：http://uvy.cashguo.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yvj.fehbvm.com

[U104] JS：防抖
来源：http://fxc.xziqi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xni.yongpay.top

[U105] JS：节流
来源：http://pyb.yueranfly.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nbv.shangyingyoupin.top

[U106] JS：日期格式化
来源：http://mof.jinyuanbaomall.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gfm.gogol.net.cn

[U107] JS：数字千分位
来源：http://tij.ywan-chungtsiang.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://krs.chenlongwang.top

[U108] JS：随机整数
来源：http://gar.yangfankeji.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://isl.dianchejie.cn

[U109] JS：数组分组
来源：http://nta.yangfankeji.com

Object.groupBy(arr, x => x.type)
来源：http://wfm.sjlbkw.cn

[U110] JS：数组分块
来源：http://dwf.gzhubu.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://uwt.iojbl.cn

[U111] JS：对象转 Map
来源：http://swt.nanxuanxn.top

new Map(Object.entries(obj))
来源：http://iom.shzxlz.cn

[U112] JS：字符串补位
来源：http://zov.xinyue.icu

"7".padStart(3, "0")
来源：http://uqn.cucudq.cn

[U113] JS：正则替换全部
来源：http://qhz.hnxiangtu.top

s.replaceAll("a", "b")
来源：http://npl.nanxinkj.top

[U114] JS：JSON 深比较
来源：http://gtq.zhiwuduotai.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://cpw.epnwcf.com

[U115] JS：生成 UUID
来源：http://rdv.xylfe.cn

crypto.randomUUID()
来源：http://cig.hnxiangtu.top

[U116] JS：类型检查（JSDoc）
来源：http://ujl.cqqwz.cn

/** @param {string} name */ function f(name) {}
来源：http://ukr.zhengqikj.top

[U117] JS：单元测试
来源：http://sva.tanke756.top

npm i -D vitest;  npx vitest
来源：http://hdc.sysykeji.top

[U118] JS：开发服务器
来源：http://dym.yj20258.top

npm i -D vite;  npx vite
来源：http://scn.hongshengwenyu.top

[U119] JS：生产构建
来源：http://oby.jianghu66.top

npx vite build
来源：http://gym.9152youxi.cn

[U120] JS：读取环境变量（Vite）
来源：http://yjb.xziqi.cn

import.meta.env.VITE_API_URL
来源：http://wkz.jiagoushi.top

================================================================================
来源：http://zcp.jyoumei.cn

统计汇总
来源：http://dsw.zhongyouzk.top

================================================================================
来源：http://xtg.tanke756.top

按语言统计（条）：
来源：http://bxr.yj20258888.top

Python ......... 252
来源：http://rrk.sjlbkw.cn

PHP ............ 252
来源：http://cwp.xuanzx.com

JavaScript ..... 252
来源：http://tbv.epnwcf.com

TypeScript ..... 212
来源：http://ohi.jinqigfzy.top

Java ........... 212
来源：http://kcz.svipenyu.cn

Go ............. 212
来源：http://llo.jqgfzy.top

Ruby ........... 212
来源：http://tba.hcnkem.com

C# ............. 212
来源：http://spy.mhx1999.top

C .............. 30
来源：http://hmt.gzhubu.top

C++ ............ 30
来源：http://wow.fengsongda.top

SQL ............ 90
来源：http://yad.c1oappe.top

Bash ........... 80
来源：http://vxu.yuanzhike.top

Kotlin ......... 15
来源：http://ocn.52xcode.cn

Swift .......... 15
来源：http://djx.hnxiangtu.top

Lua ............ 10
来源：http://sdk.yfazqb.com

Perl ........... 10
来源：http://imv.ppjwa.cn

Scala .......... 10
来源：http://dst.sufxvd.cn

------------------------------------
来源：http://hcx.dianchejie.cn

合计 ........... 2106 条
来源：http://qka.yj202588.top

按章节统计：
来源：http://oov.redwolf501.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://iwc.fehbvm.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ntu.iojbl.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://exe.zhixingplan.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zhq.jlsjyb.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rsi.xziqi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xzr.jyoumei.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tjk.chenlongwang.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://pkq.sjlbkw.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jvw.jiagoushi.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ekg.guowangkeji.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vws.guowangkeji.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cey.aizwys.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wkr.yueranfly.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://asv.jyoumei.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bqu.zhongyouzk.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://cwb.xylfe.cn

Q SQL 专题                              90
来源：http://pqr.zhijiandao.cn

R Bash 专题                             80
来源：http://whn.fehbvm.com

S C / C++ 专题                          60
来源：http://avy.iojbl.cn

T 其他语言补充                          60
来源：http://zdf.yueranfly.top

U 高频实用片段                         120
来源：http://ffy.0kj1m.cn

------------------------------------
来源：http://viq.zhijiandao.cn

合计                                  2106 条
来源：http://edh.zdbjq.cn

--------------------------------------------------------------------------------
来源：http://aew.dianchejie.cn

使用提醒
来源：http://kzv.gzhubu.top

--------------------------------------------------------------------------------
来源：http://ncy.gotoacloud.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://pak.ydjk.org.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wha.yuanzhike.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wna.tian-w.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://hkh.zycfv.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://lpi.jyoumei.cn

—— 文件结束 ——
来源：http://tft.kuanghao11.cn

================================================================================
来源：http://lly.zhiwuduotai.top

程序语言常见例子速查手册（2024 版）
来源：http://guv.zhijiandao.cn

Common Programming Examples Cheat Book
来源：http://hmu.gaohongyu789.top

================================================================================
来源：http://iam.zhaomingkeji.xyz

【收录内容】
来源：http://fnr.mhx1999.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://fdm.havefunace.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://uvz.guowangkeji.top

SQL · Bash · C · C++
来源：http://izk.gogol.net.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://yax.jianghu66.top

【使用说明】
来源：http://ejd.fzhhl.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://pen.jinqigufen.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://cho.daria6918.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://aqs.ivvv.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://agn.havefunace.top

Bash:  Shell         C:     C             C++:   C++
来源：http://wjx.havefunace.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://lwq.jinqigufen.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://bad.zhengqikj.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wsv.shzxlz.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://bdi.cashguo.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gau.fengsongda.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://rsu.chenjidiqi.icu

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://epg.epnwcf.com

【文件统计】
来源：http://ejj.fehbvm.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://elf.daxiang520.top

--------------------------------------------------------------------------------
来源：http://ikc.ppjwa.cn

目  录
来源：http://rfe.kuanghao11.cn

--------------------------------------------------------------------------------
来源：http://roz.cqqwz.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://sxr.yuxming.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://kst.jinqigufen.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://epg.fzhhl.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://nun.sweek.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://rpy.jqgufenzy.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://our.c1oappe.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ekz.aibaodan.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://tzl.hcnkem.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ucu.xziqi.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://vlj.yonumen.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://htt.xylfe.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mxr.yangfankeji.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://gmm.feifeiyinyue.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://bzt.cucudq.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ddo.bjfxy.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mmi.jianghu66.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://yrb.yj202588.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://zuj.quarkkingdee.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://nzv.ppjwa.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ptg.cqqwz.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://bdt.hongshengwenyu.top


<!-- 参考信息 -->