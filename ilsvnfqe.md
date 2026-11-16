代发 wailian999

[U23] Py：分块读取大文件
来源：http://koy.yj202588.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://taz.jinghuilouyu.cn

[U24] Py：路径操作
来源：http://kyo.hywenlv.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ndf.gotoacloud.top

[U25] Py：CSV 按字典读
来源：http://zgo.zhengqikj.top

csv.DictReader(f)
来源：http://thp.shanyushiyangtech.top

[U26] Py：并发下载
来源：http://btm.0kj1m.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://sxl.xylfe.cn

[U27] Py：异步 HTTP
来源：http://bos.yongpay.top

aiohttp.ClientSession() 配合 async with
来源：http://rlm.ybcxt.top

[U28] Py：类型别名
来源：http://qvv.yangfankeji.com

UserId = int
来源：http://umm.daria6918.cn

[U29] Py：属性校验
来源：http://gao.pengpengdd.cyou

@property 与 @x.setter 配合
来源：http://pet.yanxiufei.cn

[U30] Py：数据类
来源：http://xfh.jinqigfzy.top

@dataclass(slots=True)
来源：http://vju.gotoacloud.top

[U31] Py：单测
来源：http://wby.fktsv.cn

python -m pytest -q
来源：http://xem.nanxuanxn.top

[U32] Py：代码格式化
来源：http://zah.tanke756.top

ruff format . && ruff check --fix .
来源：http://cpn.fehbvm.com

[U33] Py：打包发布
来源：http://pfi.yj202588.top

python -m build  （依赖 pyproject.toml）
来源：http://cva.zdqjudy.top

[U34] Py：判断编码
来源：http://iki.smart0.xyz

chardet.detect(raw)
来源：http://rxy.hnqzz.top

[U35] Py：发送邮件
来源：http://yhs.ppjwa.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qgo.sysykeji.top

[U36] Py：定时任务
来源：http://rdr.svipenyu.cn

schedule.every(10).minutes.do(job)
来源：http://nrb.sweek.top

[U37] Py：读写 Excel
来源：http://psv.yangfankeji.com

pandas.read_excel / DataFrame.to_excel
来源：http://eba.tianlin.xyz

[U38] Py：获取脚本所在目录
来源：http://bqa.feifeiyinyue.top

Path(__file__).resolve().parent
来源：http://kme.ivvv.top

[U39] Py：判断是否在交互环境
来源：http://hrv.ywan-chungtsiang.top

sys.stdout.isatty()
来源：http://fkl.ctjpmb.com

[U40] Py：打印到标准错误
来源：http://yzb.yanxiufei.cn

print("err", file=sys.stderr)
来源：http://tjm.gogol.net.cn

[U41] PHP：初始化 Composer 项目
来源：http://hng.cucudq.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ghw.xziqi.cn

[U42] PHP：PSR-4 自动加载
来源：http://pyn.ywan-chungtsiang.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xvq.hfpthk.cn

[U43] PHP：声明命名空间
来源：http://cxl.pycfn.com

namespace App\Http;
来源：http://ejs.yfazqb.com

[U44] PHP：开启严格类型
来源：http://xbz.yanxiufei.cn

declare(strict_types=1);
来源：http://qbl.xylfe.cn

[U45] PHP：类型声明与返回类型
来源：http://hts.zhaomingkeji.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://ebd.zhiwuduotai.top

[U46] PHP：可空类型
来源：http://gtj.52xcode.cn

?string $name = null
来源：http://dul.smart0.xyz

[U47] PHP：联合类型
来源：http://mnh.xuanzx.com

int|string $id
来源：http://ztd.fengsongda.top

[U48] PHP：纯枚举
来源：http://vkr.jlsjyb.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cgm.yj20258888.top

[U49] PHP：只读属性
来源：http://aav.daxiang520.top

public readonly string $name
来源：http://udh.tanke756.top

[U50] PHP：构造器属性提升
来源：http://jgw.shanyushiyangkeji.top

public function __construct(private int $id) {}
来源：http://rsy.yangfankeji.com

[U51] PHP：数组解构
来源：http://vlt.shanyushiyangkeji.top

[$a, $b] = $arr;
来源：http://xai.sufxvd.cn

[U52] PHP：箭头函数
来源：http://sad.jianghu66.top

$double = fn($x) => $x * 2;
来源：http://dpj.fengsongda.top

[U53] PHP：空合并运算符
来源：http://bum.52xcode.cn

$v = $a ?? $b ?? "default";
来源：http://hsc.tarul.cn

[U54] PHP：空安全调用
来源：http://scm.hysaishi.cn

$obj?->method()
来源：http://cyd.ydjk.org.cn

[U55] PHP：match 表达式
来源：http://hqm.hongshengwenyu.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dpm.cqqwz.cn

[U56] PHP：命名参数
来源：http://atl.yueranfly.top

f(a: 1, b: 2)
来源：http://mqe.316326.xyz

[U57] PHP：字符串插值
来源：http://qbp.daxiang520.top

"值: {$a}"
来源：http://rnt.jyoumei.cn

[U58] PHP：数组三件套
来源：http://sny.birdmap.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ldz.iojbl.cn

[U59] PHP：自定义排序
来源：http://dtb.c1oappe.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mpj.jinqigufen.top

[U60] PHP：JSON 编解码
来源：http://yfq.chenzaomai.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://peu.shangyingyoupin.top

[U61] PHP：正则
来源：http://grm.zhixingplan.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://elp.guowangkeji.top

[U62] PHP：日期对象
来源：http://ajd.ydzc1.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://uob.kuanghao11.cn

[U63] PHP：文件读写
来源：http://uxe.c1oappe.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yae.ybcxt.top

[U64] PHP：目录遍历
来源：http://uul.guannengcc.top

glob("dir/*.php");  scandir("dir");
来源：http://bow.iojbl.cn

[U65] PHP：会话
来源：http://xgt.yj20258.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ytz.haohaochexian.top

[U66] PHP：设置 Cookie
来源：http://bsx.chenzaomai.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://upw.0kj1m.cn

[U67] PHP：处理文件上传
来源：http://ubi.cheryme.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://psi.zhoulong.xyz

[U68] PHP：PDO 连接
来源：http://ndt.yj20258888.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://btd.yanxiufei.cn

[U69] PHP：PDO 预处理
来源：http://klh.iojbl.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xiy.svipenyu.cn

[U70] PHP：PDO 事务
来源：http://yuo.tarul.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bcn.pycfn.com

[U71] PHP：抛出异常
来源：http://iax.snrcjt.cn

throw new RuntimeException("失败", 500);
来源：http://mem.52xcode.cn

[U72] PHP：写错误日志
来源：http://uut.gzhubu.top

error_log("失败: " . $e->getMessage());
来源：http://tju.cheryme.top

[U73] PHP：读取 ini 配置
来源：http://ewo.ehwqpu.com

parse_ini_file("config.ini", true)
来源：http://seu.xingfuxueyuan.xyz

[U74] PHP：读取环境变量
来源：http://mge.yj20258888.top

getenv("APP_ENV") ?: "production"
来源：http://rla.yueranfly.top

[U75] PHP：依赖注入
来源：http://jzk.yj20258888.top

composer require psr/container
来源：http://dim.quarkkingdee.top

[U76] PHP：简单路由
来源：http://rfj.yj20258.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xik.hysaishi.cn

[U77] PHP：模板渲染
来源：http://cvg.cashguo.top

composer require twig/twig
来源：http://wic.bjfxy.top

[U78] PHP：单元测试
来源：http://onz.jinghuilouyu.cn

composer require --dev phpunit/phpunit
来源：http://cja.jinqigufen.top

[U79] PHP：静态分析
来源：http://lza.dianchejie.cn

composer require --dev phpstan/phpstan
来源：http://hhw.guannengcc.top

[U80] PHP：代码规范修复
来源：http://brr.hysaishi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://rhx.zhongyouzk.top

[U81] JS：初始化项目
来源：http://pln.kuanghao11.cn

npm init -y;  npm i express
来源：http://ibz.fengsongda.top

[U82] JS：package.json 脚本
来源：http://avl.wangdashe.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cjm.hnqzz.top

[U83] JS：ES Module 导入导出
来源：http://dte.feifeiyinyue.top

export const a = 1;  import { a } from "./m.js";
来源：http://ydr.yanxiufei.cn

[U84] JS：CommonJS 写法
来源：http://def.ivvv.top

module.exports = { a };  const { a } = require("./m");
来源：http://oci.xylfe.cn

[U85] JS：可选链
来源：http://ntc.birdmap.top

a?.b?.c
来源：http://juq.gogol.net.cn

[U86] JS：空值合并
来源：http://cgn.yonumen.top

a ?? b
来源：http://dew.redwolf501.top

[U87] JS：解构默认值
来源：http://cvz.chenjidiqi.icu

const { a = 1, b = 2 } = obj;
来源：http://lyr.cucudq.cn

[U88] JS：对象展开合并
来源：http://jgx.tianlin.xyz

{ ...a, ...b }
来源：http://ouc.yj20258888.top

[U89] JS：数组去重
来源：http://ubs.gaohongyu789.top

[...new Set(arr)]
来源：http://tpu.316326.xyz

[U90] JS：数字数组排序
来源：http://mes.nanxuanxn.top

[...arr].sort((a, b) => a - b)
来源：http://jsn.quarkkingdee.top

[U91] JS：对象键值遍历
来源：http://ubd.yj202588.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lsx.wangshuangyany.cn

[U92] JS：深拷贝
来源：http://evl.mhx1999.top

structuredClone(obj)
来源：http://xzl.daria6918.cn

[U93] JS：模板字符串
来源：http://brh.wangdashe.top

`共 ${n} 条`
来源：http://bps.zhixingplan.top

[U94] JS：箭头函数
来源：http://ppx.hnqzz.top

const double = x => x * 2;
来源：http://ctx.chenlongwang.top

[U95] JS：Promise 包装
来源：http://icg.redwolf501.top

new Promise((resolve, reject) => {})
来源：http://ikk.jyoumei.cn

[U96] JS：async/await 与异常
来源：http://cbe.tian-w.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pap.cashguo.top

[U97] JS：并发请求
来源：http://xjt.ivvv.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://roe.sjlbkw.cn

[U98] JS：fetch 带 JSON
来源：http://jys.ppjwa.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zdb.sysykeji.top

[U99] JS：事件监听
来源：http://fgu.xuanzx.com

el.addEventListener("click", e => {})
来源：http://iyl.sweek.top

[U100] JS：DOM 查询
来源：http://iml.sweek.top

document.querySelector(".item")
来源：http://hcr.cqqwz.cn

[U101] JS：classList 操作
来源：http://rda.quarkkingdee.top

el.classList.toggle("active")
来源：http://rij.ehwqpu.com

[U102] JS：本地存储
来源：http://dfo.fzhhl.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://dvq.jlsjyb.cn

[U103] JS：定时器
来源：http://fdx.yj202588.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hci.0kj1m.cn

[U104] JS：防抖
来源：http://bdv.hongshengwenyu.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pvq.chenlongwang.top

[U105] JS：节流
来源：http://hkh.daria6918.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://oqb.quarkkingdee.top

[U106] JS：日期格式化
来源：http://tdg.jinyuanbaomall.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nqx.yongpay.top

[U107] JS：数字千分位
来源：http://fgz.ehwqpu.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qlp.shuidangran.top

[U108] JS：随机整数
来源：http://dqz.yj20258888.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tar.zhixingplan.top

[U109] JS：数组分组
来源：http://htk.jinyuanbaomall.cn

Object.groupBy(arr, x => x.type)
来源：http://fdu.epnwcf.com

[U110] JS：数组分块
来源：http://rmy.fanxiaobao.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://sny.jqgufenzy.top

[U111] JS：对象转 Map
来源：http://orr.nanxinkj.top

new Map(Object.entries(obj))
来源：http://fmf.ydzc1.top

[U112] JS：字符串补位
来源：http://cus.gotoacloud.top

"7".padStart(3, "0")
来源：http://okn.bbcook.cn

[U113] JS：正则替换全部
来源：http://pvq.shuidangran.top

s.replaceAll("a", "b")
来源：http://cvh.andypj.xyz

[U114] JS：JSON 深比较
来源：http://grk.yangfankeji.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://cvp.yvedp.cn

[U115] JS：生成 UUID
来源：http://kfk.meibo888.top

crypto.randomUUID()
来源：http://rtb.shangyingyoupin.top

[U116] JS：类型检查（JSDoc）
来源：http://klb.havefunace.top

/** @param {string} name */ function f(name) {}
来源：http://ohs.zdqjudy.top

[U117] JS：单元测试
来源：http://rlr.vqdsnc.cn

npm i -D vitest;  npx vitest
来源：http://yod.quarkkingdee.top

[U118] JS：开发服务器
来源：http://bcs.zhengqikj.top

npm i -D vite;  npx vite
来源：http://dub.nwbrower.top

[U119] JS：生产构建
来源：http://scu.shuidangran.top

npx vite build
来源：http://rqo.nanxuanxn.top

[U120] JS：读取环境变量（Vite）
来源：http://zrv.kuanghao11.cn

import.meta.env.VITE_API_URL
来源：http://glr.guowangkeji.top

================================================================================
来源：http://wiu.0kj1m.cn

统计汇总
来源：http://rez.dashuyun.cn

================================================================================
来源：http://usx.fzhhl.top

按语言统计（条）：
来源：http://mkm.hesvh.cn

Python ......... 252
来源：http://byf.nwbrower.top

PHP ............ 252
来源：http://gdk.yj20258888.top

JavaScript ..... 252
来源：http://bfi.xinyue.icu

TypeScript ..... 212
来源：http://oqn.haohaochexian.top

Java ........... 212
来源：http://lgr.jyoumei.cn

Go ............. 212
来源：http://okp.fktsv.cn

Ruby ........... 212
来源：http://pdp.smart0.xyz

C# ............. 212
来源：http://ddu.haohaochexian.top

C .............. 30
来源：http://saq.pycfn.com

C++ ............ 30
来源：http://dii.cqqwz.cn

SQL ............ 90
来源：http://nya.meibo888.top

Bash ........... 80
来源：http://gfw.daria6918.cn

Kotlin ......... 15
来源：http://zbd.fengsongda.top

Swift .......... 15
来源：http://xan.pycfn.com

Lua ............ 10
来源：http://vap.fehbvm.com

Perl ........... 10
来源：http://zpg.cucudq.cn

Scala .......... 10
来源：http://hta.hongshengwenyu.top

------------------------------------
来源：http://ipl.cdnleiting.top

合计 ........... 2106 条
来源：http://jcm.hesvh.cn

按章节统计：
来源：http://fad.wangshuangyany.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://idz.wangshuangyany.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ver.hfpthk.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://irn.yvedp.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://uvx.tianlin.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ayl.xuetiantiany.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ila.jqgufenzy.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ddy.ydzc1.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://idd.hongshengwenyu.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hfb.fktsv.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://sjf.hongshengwenyu.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://snt.sweek.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ulv.yj20258888.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qqz.dianchejie.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://fty.cdnleiting.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://gpw.hysaishi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qpy.shuidangran.top

Q SQL 专题                              90
来源：http://fnu.gotoacloud.top

R Bash 专题                             80
来源：http://gbq.aibaodan.cn

S C / C++ 专题                          60
来源：http://kay.vqdsnc.cn

T 其他语言补充                          60
来源：http://uge.daria6918.cn

U 高频实用片段                         120
来源：http://rok.kuanghao11.cn

------------------------------------
来源：http://ngg.cdnleiting.top

合计                                  2106 条
来源：http://fis.redwolf501.top

--------------------------------------------------------------------------------
来源：http://mlf.yanxiufei.cn

使用提醒
来源：http://dew.ppjwa.cn

--------------------------------------------------------------------------------
来源：http://azt.chenzaomai.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ssw.chenlongwang.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://sel.jiagoushi.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://tll.hnqzz.top

在旧版本上使用前请先确认语法支持情况。
来源：http://htf.wangshuangyany.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://kme.zhaomingkeji.xyz

—— 文件结束 ——
来源：http://jsu.zhiwuduotai.top

================================================================================
来源：http://qgw.hammf.cn

程序语言常见例子速查手册（2024 版）
来源：http://rkq.wangshuangyany.cn

Common Programming Examples Cheat Book
来源：http://pea.jqgfzy.top

================================================================================
来源：http://eta.xinyue.icu

【收录内容】
来源：http://kxo.sxryk.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://qyk.pengpengdd.cyou

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://lcg.meibo888.top

SQL · Bash · C · C++
来源：http://wny.hnqzz.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://bwy.chenjidiqi.icu

【使用说明】
来源：http://skc.hysaishi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://uui.yj202588.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mvz.hysaishi.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hoj.yuxming.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://cni.yanxiufei.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ivx.hnqzz.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xle.yj202588.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://bfd.ctjpmb.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://irp.fzhhl.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://bgx.jlsjyb.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pgk.aizwys.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://gzo.epnwcf.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ifl.hongshengwenyu.top

【文件统计】
来源：http://qbf.tanke756.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qvg.pycfn.com

--------------------------------------------------------------------------------
来源：http://lgl.snrcjt.cn

目  录
来源：http://ycz.chenzaomai.com

--------------------------------------------------------------------------------
来源：http://oaa.dashuyun.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://rgb.cucudq.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qoi.zhixingplan.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zsa.zycfv.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://lyk.yuanzhike.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://rwb.yueranfly.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ytk.gzhubu.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://syp.iojbl.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://rkx.nanxuanxn.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tqi.feifeiyinyue.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://zcd.yj202588.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://nps.guannengcc.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mil.sufxvd.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ygv.redwolf501.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://iiv.yj202588.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://gyi.xingfuxueyuan.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rik.cdnleiting.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://cwd.zhijiandao.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://vof.zhiwuduotai.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ukb.fktsv.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://frc.aibaodan.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xjq.guowangkeji.top


<!-- 参考信息 -->