代发 wailian999

[U23] Py：分块读取大文件
来源：http://lnq.bjfxy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lkk.yongpay.top

[U24] Py：路径操作
来源：http://xjy.xinyue.icu

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://egx.yuxming.cn

[U25] Py：CSV 按字典读
来源：http://vqq.yj20258.top

csv.DictReader(f)
来源：http://quu.fanxiaobao.xyz

[U26] Py：并发下载
来源：http://con.yj202588.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ual.ppjwa.cn

[U27] Py：异步 HTTP
来源：http://vds.cashguo.top

aiohttp.ClientSession() 配合 async with
来源：http://zfh.tian-w.cn

[U28] Py：类型别名
来源：http://utw.daria6918.cn

UserId = int
来源：http://rzy.birdmap.top

[U29] Py：属性校验
来源：http://bdw.dashuyun.cn

@property 与 @x.setter 配合
来源：http://uvz.daria6918.cn

[U30] Py：数据类
来源：http://rsh.hnqzz.top

@dataclass(slots=True)
来源：http://hfg.ybcxt.top

[U31] Py：单测
来源：http://tgr.zdbjq.cn

python -m pytest -q
来源：http://xbb.cdnleiting.top

[U32] Py：代码格式化
来源：http://zcm.shzxlz.cn

ruff format . && ruff check --fix .
来源：http://dcs.gaohongyu789.top

[U33] Py：打包发布
来源：http://zzq.hesvh.cn

python -m build  （依赖 pyproject.toml）
来源：http://axt.zhaomingkeji.xyz

[U34] Py：判断编码
来源：http://awo.cheryme.top

chardet.detect(raw)
来源：http://aym.zhoulong.xyz

[U35] Py：发送邮件
来源：http://gpc.sysykeji.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://azq.vehdjk.com

[U36] Py：定时任务
来源：http://ktb.epnwcf.com

schedule.every(10).minutes.do(job)
来源：http://cgu.yuanzhike.top

[U37] Py：读写 Excel
来源：http://gkm.yj20258.top

pandas.read_excel / DataFrame.to_excel
来源：http://fiu.ctjpmb.com

[U38] Py：获取脚本所在目录
来源：http://zex.chenjidiqi.icu

Path(__file__).resolve().parent
来源：http://qvb.zhoulong.xyz

[U39] Py：判断是否在交互环境
来源：http://jgj.gaohongyu789.top

sys.stdout.isatty()
来源：http://wfy.zycfv.cn

[U40] Py：打印到标准错误
来源：http://hox.gogol.net.cn

print("err", file=sys.stderr)
来源：http://pus.cashguo.top

[U41] PHP：初始化 Composer 项目
来源：http://zro.jlsjyb.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://qlt.ydjk.org.cn

[U42] PHP：PSR-4 自动加载
来源：http://lub.daxiang520.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jmi.feifeiyinyue.top

[U43] PHP：声明命名空间
来源：http://azn.uphjek.com

namespace App\Http;
来源：http://byb.zhijiandao.cn

[U44] PHP：开启严格类型
来源：http://hkv.jianghu66.top

declare(strict_types=1);
来源：http://fgf.jyoumei.cn

[U45] PHP：类型声明与返回类型
来源：http://uny.gaohongyu789.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://xmm.sjlbkw.cn

[U46] PHP：可空类型
来源：http://peg.yonumen.top

?string $name = null
来源：http://hqe.yangfankeji.com

[U47] PHP：联合类型
来源：http://jbh.jqgfzy.top

int|string $id
来源：http://xbi.feifeiyinyue.top

[U48] PHP：纯枚举
来源：http://ryp.svipenyu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dhv.yanxiufei.cn

[U49] PHP：只读属性
来源：http://ktj.svipenyu.cn

public readonly string $name
来源：http://ldf.yueranfly.top

[U50] PHP：构造器属性提升
来源：http://dgk.aibaodan.cn

public function __construct(private int $id) {}
来源：http://lrg.aizwys.cn

[U51] PHP：数组解构
来源：http://ybd.shanyushiyangtech.top

[$a, $b] = $arr;
来源：http://bzb.tarul.cn

[U52] PHP：箭头函数
来源：http://zsr.yj20258.top

$double = fn($x) => $x * 2;
来源：http://tgu.cucudq.cn

[U53] PHP：空合并运算符
来源：http://nze.redwolf501.top

$v = $a ?? $b ?? "default";
来源：http://mzf.shuidangran.top

[U54] PHP：空安全调用
来源：http://veb.tianlin.xyz

$obj?->method()
来源：http://ebn.bjfxy.top

[U55] PHP：match 表达式
来源：http://eas.tarul.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qeo.hfpthk.cn

[U56] PHP：命名参数
来源：http://cav.dianchejie.cn

f(a: 1, b: 2)
来源：http://wog.jiagoushi.top

[U57] PHP：字符串插值
来源：http://wzo.kuanghao11.cn

"值: {$a}"
来源：http://grc.fehbvm.com

[U58] PHP：数组三件套
来源：http://qdv.jinghuilouyu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://skg.guannengcc.top

[U59] PHP：自定义排序
来源：http://ldf.zdqjudy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://opw.kuanghao11.cn

[U60] PHP：JSON 编解码
来源：http://jst.xziqi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wlb.316326.xyz

[U61] PHP：正则
来源：http://tux.quarkkingdee.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qjs.hfpthk.cn

[U62] PHP：日期对象
来源：http://leq.yj20258888.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://dty.yanxiufei.cn

[U63] PHP：文件读写
来源：http://xml.aibaodan.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rce.ydzc1.top

[U64] PHP：目录遍历
来源：http://ozc.kuanghao11.cn

glob("dir/*.php");  scandir("dir");
来源：http://igh.ehwqpu.com

[U65] PHP：会话
来源：http://fux.yanxiufei.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://jjn.sxryk.cn

[U66] PHP：设置 Cookie
来源：http://slo.cqqwz.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wsj.9152youxi.cn

[U67] PHP：处理文件上传
来源：http://dww.daria6918.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rca.cdnleiting.top

[U68] PHP：PDO 连接
来源：http://wdy.dianchejie.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ryl.hywenlv.cn

[U69] PHP：PDO 预处理
来源：http://ysa.dianchejie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://owh.tianlin.xyz

[U70] PHP：PDO 事务
来源：http://bji.vehdjk.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://eqy.yj20258888.top

[U71] PHP：抛出异常
来源：http://geo.xylfe.cn

throw new RuntimeException("失败", 500);
来源：http://dzx.jqgufenzy.top

[U72] PHP：写错误日志
来源：http://mdo.yfazqb.com

error_log("失败: " . $e->getMessage());
来源：http://ouq.kuanghao11.cn

[U73] PHP：读取 ini 配置
来源：http://zik.meibo888.top

parse_ini_file("config.ini", true)
来源：http://jkx.epnwcf.com

[U74] PHP：读取环境变量
来源：http://dwp.daria6918.cn

getenv("APP_ENV") ?: "production"
来源：http://bnj.daxiang520.top

[U75] PHP：依赖注入
来源：http://wbt.yuanzhike.top

composer require psr/container
来源：http://dux.xuanzx.com

[U76] PHP：简单路由
来源：http://vzq.yj20258.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zqn.xingfuxueyuan.xyz

[U77] PHP：模板渲染
来源：http://zyt.gotoacloud.top

composer require twig/twig
来源：http://gye.snrcjt.cn

[U78] PHP：单元测试
来源：http://mrp.tanke756.top

composer require --dev phpunit/phpunit
来源：http://tyh.zdqjudy.top

[U79] PHP：静态分析
来源：http://wiv.9152youxi.cn

composer require --dev phpstan/phpstan
来源：http://opi.hesvh.cn

[U80] PHP：代码规范修复
来源：http://jgr.shanyushiyangkeji.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://clq.guannengcc.top

[U81] JS：初始化项目
来源：http://ydp.hnqzz.top

npm init -y;  npm i express
来源：http://bjo.yj20258.top

[U82] JS：package.json 脚本
来源：http://muq.sxryk.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wry.jyoumei.cn

[U83] JS：ES Module 导入导出
来源：http://piu.nwbrower.top

export const a = 1;  import { a } from "./m.js";
来源：http://tiq.zdbjq.cn

[U84] JS：CommonJS 写法
来源：http://dpj.sufxvd.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ruv.yuxming.cn

[U85] JS：可选链
来源：http://mxd.jinyuanbaomall.cn

a?.b?.c
来源：http://kbh.ydjk.org.cn

[U86] JS：空值合并
来源：http://upd.wangdashe.top

a ?? b
来源：http://vrs.xziqi.cn

[U87] JS：解构默认值
来源：http://qco.shanyushiyangtech.top

const { a = 1, b = 2 } = obj;
来源：http://bov.daxiang520.top

[U88] JS：对象展开合并
来源：http://msb.hysaishi.cn

{ ...a, ...b }
来源：http://drh.svipenyu.cn

[U89] JS：数组去重
来源：http://epk.shangyingyoupin.top

[...new Set(arr)]
来源：http://jnw.bjfxy.top

[U90] JS：数字数组排序
来源：http://ykv.yongpay.top

[...arr].sort((a, b) => a - b)
来源：http://byv.wangdashe.top

[U91] JS：对象键值遍历
来源：http://tes.nwbrower.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jcl.xinyue.icu

[U92] JS：深拷贝
来源：http://fho.sxryk.cn

structuredClone(obj)
来源：http://pxw.ybcxt.top

[U93] JS：模板字符串
来源：http://oub.guowangkeji.top

`共 ${n} 条`
来源：http://lvq.shanyushiyangtech.top

[U94] JS：箭头函数
来源：http://mnm.shzxlz.cn

const double = x => x * 2;
来源：http://yvy.gzhubu.top

[U95] JS：Promise 包装
来源：http://cez.zhiwuduotai.top

new Promise((resolve, reject) => {})
来源：http://hag.fzhhl.top

[U96] JS：async/await 与异常
来源：http://jyx.cashguo.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ynf.chenzaomai.com

[U97] JS：并发请求
来源：http://mvw.yuxming.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://rax.mhx1999.top

[U98] JS：fetch 带 JSON
来源：http://peu.yuanzhike.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://yyk.shuidangran.top

[U99] JS：事件监听
来源：http://ydi.gzhubu.top

el.addEventListener("click", e => {})
来源：http://ssu.gaohongyu789.top

[U100] JS：DOM 查询
来源：http://pcu.cheryme.top

document.querySelector(".item")
来源：http://tjk.hesvh.cn

[U101] JS：classList 操作
来源：http://fco.ppjwa.cn

el.classList.toggle("active")
来源：http://ktq.cqqwz.cn

[U102] JS：本地存储
来源：http://uul.pengpengdd.cyou

localStorage.setItem("k", JSON.stringify(v))
来源：http://luf.birdmap.top

[U103] JS：定时器
来源：http://plv.jianghu66.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hwu.yj202588.top

[U104] JS：防抖
来源：http://vdx.zycfv.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wtw.yuanzhike.top

[U105] JS：节流
来源：http://xxe.fzhhl.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bys.jqgufenzy.top

[U106] JS：日期格式化
来源：http://wjk.yj20258.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://toa.andypj.xyz

[U107] JS：数字千分位
来源：http://ros.cashguo.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xeg.dashuyun.cn

[U108] JS：随机整数
来源：http://anl.zhijiandao.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://sqg.dashuyun.cn

[U109] JS：数组分组
来源：http://cwh.meibo888.top

Object.groupBy(arr, x => x.type)
来源：http://sou.ydzc1.top

[U110] JS：数组分块
来源：http://idc.zhiwuduotai.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jdh.feifeiyinyue.top

[U111] JS：对象转 Map
来源：http://pcc.hesvh.cn

new Map(Object.entries(obj))
来源：http://tmo.yvedp.cn

[U112] JS：字符串补位
来源：http://lvm.wangshuangyany.cn

"7".padStart(3, "0")
来源：http://qsl.fengsongda.top

[U113] JS：正则替换全部
来源：http://eak.cdnleiting.top

s.replaceAll("a", "b")
来源：http://nqu.316326.xyz

[U114] JS：JSON 深比较
来源：http://mhv.xingfuxueyuan.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://amw.pycfn.com

[U115] JS：生成 UUID
来源：http://hle.shzxlz.cn

crypto.randomUUID()
来源：http://bhd.smart0.xyz

[U116] JS：类型检查（JSDoc）
来源：http://tmi.sxryk.cn

/** @param {string} name */ function f(name) {}
来源：http://vgd.jiagoushi.top

[U117] JS：单元测试
来源：http://lpf.quarkkingdee.top

npm i -D vitest;  npx vitest
来源：http://bwk.nanxuanxn.top

[U118] JS：开发服务器
来源：http://aui.jinghuilouyu.cn

npm i -D vite;  npx vite
来源：http://fiy.wangshuangyany.cn

[U119] JS：生产构建
来源：http://ipc.aibaodan.cn

npx vite build
来源：http://iko.9152youxi.cn

[U120] JS：读取环境变量（Vite）
来源：http://oay.ywan-chungtsiang.top

import.meta.env.VITE_API_URL
来源：http://yot.kuanghao11.cn

================================================================================
来源：http://gjd.zhengqikj.top

统计汇总
来源：http://idr.chenzaomai.com

================================================================================
来源：http://xhm.yj20258888.top

按语言统计（条）：
来源：http://tow.yueranfly.top

Python ......... 252
来源：http://ogx.gotoacloud.top

PHP ............ 252
来源：http://rzx.jyoumei.cn

JavaScript ..... 252
来源：http://wxa.c1oappe.top

TypeScript ..... 212
来源：http://jxe.redwolf501.top

Java ........... 212
来源：http://mqi.c1oappe.top

Go ............. 212
来源：http://exe.gogol.net.cn

Ruby ........... 212
来源：http://yzb.hysaishi.cn

C# ............. 212
来源：http://xse.xuanzx.com

C .............. 30
来源：http://hrx.jinqigufen.top

C++ ............ 30
来源：http://vym.nanxuanxn.top

SQL ............ 90
来源：http://hht.yvedp.cn

Bash ........... 80
来源：http://cah.ehwqpu.com

Kotlin ......... 15
来源：http://uiz.aibaodan.cn

Swift .......... 15
来源：http://qdp.ehwqpu.com

Lua ............ 10
来源：http://dmk.uphjek.com

Perl ........... 10
来源：http://ppr.ctjpmb.com

Scala .......... 10
来源：http://rth.chenzaomai.com

------------------------------------
来源：http://rrb.guannengcc.top

合计 ........... 2106 条
来源：http://nic.mhx1999.top

按章节统计：
来源：http://uld.guowangkeji.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://had.bbcook.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lvz.tian-w.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://oox.shanyushiyangkeji.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://jir.jianghu66.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wie.cheryme.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://fwl.birdmap.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://gid.redwolf501.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://oua.jqgufenzy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xtb.hongshengwenyu.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://une.jianghu66.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fib.hcnkem.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qqt.andypj.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://yuc.sweek.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ucr.daxiang520.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://uuj.sysykeji.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wkl.yvedp.cn

Q SQL 专题                              90
来源：http://cqu.iojbl.cn

R Bash 专题                             80
来源：http://dak.ivvv.top

S C / C++ 专题                          60
来源：http://doi.hesvh.cn

T 其他语言补充                          60
来源：http://xza.jiagoushi.top

U 高频实用片段                         120
来源：http://kyp.cqqwz.cn

------------------------------------
来源：http://hwc.aizwys.cn

合计                                  2106 条
来源：http://sby.cheryme.top

--------------------------------------------------------------------------------
来源：http://dth.nanxinkj.top

使用提醒
来源：http://rzb.zhaomingkeji.xyz

--------------------------------------------------------------------------------
来源：http://mpv.wangshuangyany.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://doz.shanyushiyangkeji.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ofx.chenzaomai.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://gua.shangyingyoupin.top

在旧版本上使用前请先确认语法支持情况。
来源：http://yxo.zdqjudy.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jht.hnxiangtu.top

—— 文件结束 ——
来源：http://vpi.yj20258.top

================================================================================
来源：http://ltk.hcnkem.com

程序语言常见例子速查手册（2024 版）
来源：http://bif.andypj.xyz

Common Programming Examples Cheat Book
来源：http://vue.pengpengdd.cyou

================================================================================
来源：http://unb.chenzaomai.com

【收录内容】
来源：http://jgb.wangdashe.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://wmi.hesvh.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://rvi.ppjwa.cn

SQL · Bash · C · C++
来源：http://zbo.jinghuilouyu.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qyj.aibaodan.cn

【使用说明】
来源：http://eea.yuxming.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://aan.xuanzx.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://dqn.gotoacloud.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://bid.zhijiandao.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://bvn.nanxuanxn.top

Bash:  Shell         C:     C             C++:   C++
来源：http://icp.cucudq.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ylw.yj20258888.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://yze.gotoacloud.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://zhz.hfpthk.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://tkb.sufxvd.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ovc.jinqigfzy.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://jzy.tianlin.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://uqb.jqgufenzy.top

【文件统计】
来源：http://rgu.jqgufenzy.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ynr.jinyuanbaomall.cn

--------------------------------------------------------------------------------
来源：http://kuq.zhixingplan.top

目  录
来源：http://hht.zdbjq.cn

--------------------------------------------------------------------------------
来源：http://ekx.gaohongyu789.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xzl.shanyushiyangkeji.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tlz.gogol.net.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mxe.yuxming.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ado.xuetiantiany.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://gte.vehdjk.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://zvf.jinqigufen.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hvx.iojbl.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hwz.sysykeji.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ckg.hnqzz.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://rek.tianlin.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://slv.birdmap.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zht.tanke756.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://nml.aizwys.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ukw.shangyingyoupin.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://rgz.ybcxt.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://tzp.zhoulong.xyz

Q. SQL 专题                    （第 17 节，90 条）
来源：http://gdc.yuxming.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://lzk.pengpengdd.cyou

S. C / C++ 专题                （第 19 节，60 条）
来源：http://nen.sweek.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://npa.shzxlz.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xjq.fktsv.cn


<!-- 参考信息 -->