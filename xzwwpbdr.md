代发 wailian999

[U25] Py：CSV 按字典读
来源：http://jfu.xinyue.icu

csv.DictReader(f)
来源：http://vfs.jyoumei.cn

[U26] Py：并发下载
来源：http://ssb.iojbl.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rnr.tianlin.xyz

[U27] Py：异步 HTTP
来源：http://qgb.nanxuanxn.top

aiohttp.ClientSession() 配合 async with
来源：http://ryj.ydjk.org.cn

[U28] Py：类型别名
来源：http://cgg.ctjpmb.com

UserId = int
来源：http://fnd.yuanzhike.top

[U29] Py：属性校验
来源：http://nyg.haohaochexian.top

@property 与 @x.setter 配合
来源：http://jeg.sweek.top

[U30] Py：数据类
来源：http://cnh.fktsv.cn

@dataclass(slots=True)
来源：http://cnn.chenzaomai.com

[U31] Py：单测
来源：http://qog.jinqigfzy.top

python -m pytest -q
来源：http://ofq.smart0.xyz

[U32] Py：代码格式化
来源：http://vpb.shanyushiyangkeji.top

ruff format . && ruff check --fix .
来源：http://syj.yfazqb.com

[U33] Py：打包发布
来源：http://mon.nanxinkj.top

python -m build  （依赖 pyproject.toml）
来源：http://jbz.shanyushiyangtech.top

[U34] Py：判断编码
来源：http://lpc.zhixingplan.top

chardet.detect(raw)
来源：http://kxt.sxryk.cn

[U35] Py：发送邮件
来源：http://aox.jianghu66.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jmp.jlsjyb.cn

[U36] Py：定时任务
来源：http://pcj.yvedp.cn

schedule.every(10).minutes.do(job)
来源：http://hyb.cqqwz.cn

[U37] Py：读写 Excel
来源：http://mlb.52xcode.cn

pandas.read_excel / DataFrame.to_excel
来源：http://pwg.ehwqpu.com

[U38] Py：获取脚本所在目录
来源：http://xez.fzhhl.top

Path(__file__).resolve().parent
来源：http://rho.aizwys.cn

[U39] Py：判断是否在交互环境
来源：http://vqq.cqqwz.cn

sys.stdout.isatty()
来源：http://oaq.zhaomingkeji.xyz

[U40] Py：打印到标准错误
来源：http://hdn.shangyingyoupin.top

print("err", file=sys.stderr)
来源：http://kwe.nanxinkj.top

[U41] PHP：初始化 Composer 项目
来源：http://zik.ctjpmb.com

composer init;  composer require guzzlehttp/guzzle
来源：http://rjh.316326.xyz

[U42] PHP：PSR-4 自动加载
来源：http://roc.jinghuilouyu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vlz.svipenyu.cn

[U43] PHP：声明命名空间
来源：http://hzg.feifeiyinyue.top

namespace App\Http;
来源：http://zva.yongpay.top

[U44] PHP：开启严格类型
来源：http://zff.vqdsnc.cn

declare(strict_types=1);
来源：http://qha.fengsongda.top

[U45] PHP：类型声明与返回类型
来源：http://ame.wangshuangyany.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://oph.xylfe.cn

[U46] PHP：可空类型
来源：http://rlo.zhaomingkeji.xyz

?string $name = null
来源：http://pem.fengsongda.top

[U47] PHP：联合类型
来源：http://mmz.bjfxy.top

int|string $id
来源：http://eoy.xuanzx.com

[U48] PHP：纯枚举
来源：http://inp.pycfn.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kme.guannengcc.top

[U49] PHP：只读属性
来源：http://asy.ydzc1.top

public readonly string $name
来源：http://mfm.chenzaomai.com

[U50] PHP：构造器属性提升
来源：http://qyk.vehdjk.com

public function __construct(private int $id) {}
来源：http://fvv.shangyingyoupin.top

[U51] PHP：数组解构
来源：http://pmh.ydjk.org.cn

[$a, $b] = $arr;
来源：http://val.cucudq.cn

[U52] PHP：箭头函数
来源：http://mun.nanxinkj.top

$double = fn($x) => $x * 2;
来源：http://pjj.cheryme.top

[U53] PHP：空合并运算符
来源：http://hyw.zhaomingkeji.xyz

$v = $a ?? $b ?? "default";
来源：http://ptb.epnwcf.com

[U54] PHP：空安全调用
来源：http://geb.redwolf501.top

$obj?->method()
来源：http://nyv.svipenyu.cn

[U55] PHP：match 表达式
来源：http://orz.hesvh.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://anc.ywan-chungtsiang.top

[U56] PHP：命名参数
来源：http://udu.sjlbkw.cn

f(a: 1, b: 2)
来源：http://yxz.uphjek.com

[U57] PHP：字符串插值
来源：http://ujl.meibo888.top

"值: {$a}"
来源：http://dyz.yongpay.top

[U58] PHP：数组三件套
来源：http://msq.jiagoushi.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kgo.zhoulong.xyz

[U59] PHP：自定义排序
来源：http://kmi.fengsongda.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dyy.zhiwuduotai.top

[U60] PHP：JSON 编解码
来源：http://gby.ywan-chungtsiang.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hgm.zhijiandao.cn

[U61] PHP：正则
来源：http://fbm.jinqigufen.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jgg.xziqi.cn

[U62] PHP：日期对象
来源：http://qkr.birdmap.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wig.yanxiufei.cn

[U63] PHP：文件读写
来源：http://wuv.ppjwa.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bbe.jinyuanbaomall.cn

[U64] PHP：目录遍历
来源：http://hhx.zdqjudy.top

glob("dir/*.php");  scandir("dir");
来源：http://ssd.feifeiyinyue.top

[U65] PHP：会话
来源：http://cum.xziqi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ags.hammf.cn

[U66] PHP：设置 Cookie
来源：http://ysa.xziqi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ghi.nanxinkj.top

[U67] PHP：处理文件上传
来源：http://wrn.nanxuanxn.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wyy.ivvv.top

[U68] PHP：PDO 连接
来源：http://usg.hfpthk.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ogv.jianghu66.top

[U69] PHP：PDO 预处理
来源：http://gjb.sweek.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://trq.yj20258888.top

[U70] PHP：PDO 事务
来源：http://gnd.316326.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ktv.kuanghao11.cn

[U71] PHP：抛出异常
来源：http://nsi.ehwqpu.com

throw new RuntimeException("失败", 500);
来源：http://pms.ywan-chungtsiang.top

[U72] PHP：写错误日志
来源：http://dcx.ppjwa.cn

error_log("失败: " . $e->getMessage());
来源：http://ntl.ehwqpu.com

[U73] PHP：读取 ini 配置
来源：http://awu.yuxming.cn

parse_ini_file("config.ini", true)
来源：http://iod.svipenyu.cn

[U74] PHP：读取环境变量
来源：http://svw.hnxiangtu.top

getenv("APP_ENV") ?: "production"
来源：http://zmf.sxryk.cn

[U75] PHP：依赖注入
来源：http://uun.yvedp.cn

composer require psr/container
来源：http://mts.bjfxy.top

[U76] PHP：简单路由
来源：http://ktj.fanxiaobao.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xhd.kuanghao11.cn

[U77] PHP：模板渲染
来源：http://sfv.fehbvm.com

composer require twig/twig
来源：http://tdc.ywan-chungtsiang.top

[U78] PHP：单元测试
来源：http://mzm.zhaomingkeji.xyz

composer require --dev phpunit/phpunit
来源：http://uxv.pycfn.com

[U79] PHP：静态分析
来源：http://gkt.redwolf501.top

composer require --dev phpstan/phpstan
来源：http://eth.hesvh.cn

[U80] PHP：代码规范修复
来源：http://tjw.shangyingyoupin.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://sdu.cheryme.top

[U81] JS：初始化项目
来源：http://bzo.hfpthk.cn

npm init -y;  npm i express
来源：http://vut.yanxiufei.cn

[U82] JS：package.json 脚本
来源：http://jay.hammf.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vpd.hnxiangtu.top

[U83] JS：ES Module 导入导出
来源：http://vbj.jinqigufen.top

export const a = 1;  import { a } from "./m.js";
来源：http://kco.xuetiantiany.cn

[U84] JS：CommonJS 写法
来源：http://yre.meibo888.top

module.exports = { a };  const { a } = require("./m");
来源：http://pvt.sjlbkw.cn

[U85] JS：可选链
来源：http://akh.zdqjudy.top

a?.b?.c
来源：http://ljd.zhoulong.xyz

[U86] JS：空值合并
来源：http://rnu.wangshuangyany.cn

a ?? b
来源：http://myj.hnqzz.top

[U87] JS：解构默认值
来源：http://xqk.epnwcf.com

const { a = 1, b = 2 } = obj;
来源：http://nbs.sweek.top

[U88] JS：对象展开合并
来源：http://ryh.hysaishi.cn

{ ...a, ...b }
来源：http://gpc.bbcook.cn

[U89] JS：数组去重
来源：http://yxy.chenzaomai.com

[...new Set(arr)]
来源：http://zpf.9152youxi.cn

[U90] JS：数字数组排序
来源：http://axt.shanyushiyangtech.top

[...arr].sort((a, b) => a - b)
来源：http://mev.hywenlv.cn

[U91] JS：对象键值遍历
来源：http://ohx.9152youxi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nic.nwbrower.top

[U92] JS：深拷贝
来源：http://qhe.dianchejie.cn

structuredClone(obj)
来源：http://wyj.zhengqikj.top

[U93] JS：模板字符串
来源：http://bqo.tian-w.cn

`共 ${n} 条`
来源：http://kqs.zhoulong.xyz

[U94] JS：箭头函数
来源：http://stj.hnxiangtu.top

const double = x => x * 2;
来源：http://ojm.cqqwz.cn

[U95] JS：Promise 包装
来源：http://adz.zhijiandao.cn

new Promise((resolve, reject) => {})
来源：http://ruh.cashguo.top

[U96] JS：async/await 与异常
来源：http://kkp.iojbl.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://evk.wangshuangyany.cn

[U97] JS：并发请求
来源：http://jwv.nanxinkj.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://kmu.epnwcf.com

[U98] JS：fetch 带 JSON
来源：http://dxf.jyoumei.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://psq.sufxvd.cn

[U99] JS：事件监听
来源：http://csk.yueranfly.top

el.addEventListener("click", e => {})
来源：http://jbz.gotoacloud.top

[U100] JS：DOM 查询
来源：http://dfc.daxiang520.top

document.querySelector(".item")
来源：http://cae.zhengqikj.top

[U101] JS：classList 操作
来源：http://thn.wangdashe.top

el.classList.toggle("active")
来源：http://llh.haohaochexian.top

[U102] JS：本地存储
来源：http://nus.guannengcc.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://gvl.dianchejie.cn

[U103] JS：定时器
来源：http://ibg.fengsongda.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gav.fehbvm.com

[U104] JS：防抖
来源：http://wqu.hammf.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jjg.meibo888.top

[U105] JS：节流
来源：http://xka.yj20258.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nwh.yongpay.top

[U106] JS：日期格式化
来源：http://vbs.ivvv.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://uqr.gaohongyu789.top

[U107] JS：数字千分位
来源：http://pgs.zdqjudy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://txe.nwbrower.top

[U108] JS：随机整数
来源：http://hvk.hfpthk.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://yyg.daxiang520.top

[U109] JS：数组分组
来源：http://ews.quarkkingdee.top

Object.groupBy(arr, x => x.type)
来源：http://bek.fengsongda.top

[U110] JS：数组分块
来源：http://clu.hnxiangtu.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://uia.vqdsnc.cn

[U111] JS：对象转 Map
来源：http://bhx.sjlbkw.cn

new Map(Object.entries(obj))
来源：http://ius.tarul.cn

[U112] JS：字符串补位
来源：http://bdb.yongpay.top

"7".padStart(3, "0")
来源：http://bdw.sjlbkw.cn

[U113] JS：正则替换全部
来源：http://mmz.chenlongwang.top

s.replaceAll("a", "b")
来源：http://ggh.ehwqpu.com

[U114] JS：JSON 深比较
来源：http://tcn.fehbvm.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://yxu.hcnkem.com

[U115] JS：生成 UUID
来源：http://ode.vehdjk.com

crypto.randomUUID()
来源：http://mtp.0kj1m.cn

[U116] JS：类型检查（JSDoc）
来源：http://zuq.0kj1m.cn

/** @param {string} name */ function f(name) {}
来源：http://cht.snrcjt.cn

[U117] JS：单元测试
来源：http://ivv.hongshengwenyu.top

npm i -D vitest;  npx vitest
来源：http://dkq.316326.xyz

[U118] JS：开发服务器
来源：http://mse.fehbvm.com

npm i -D vite;  npx vite
来源：http://ejd.daria6918.cn

[U119] JS：生产构建
来源：http://hna.yj202588.top

npx vite build
来源：http://rik.cucudq.cn

[U120] JS：读取环境变量（Vite）
来源：http://qll.jianghu66.top

import.meta.env.VITE_API_URL
来源：http://cmj.yuxming.cn

================================================================================
来源：http://vde.svipenyu.cn

统计汇总
来源：http://xfy.pengpengdd.cyou

================================================================================
来源：http://rau.nwbrower.top

按语言统计（条）：
来源：http://iii.cheryme.top

Python ......... 252
来源：http://lvs.yonumen.top

PHP ............ 252
来源：http://gsm.ywan-chungtsiang.top

JavaScript ..... 252
来源：http://llt.jyoumei.cn

TypeScript ..... 212
来源：http://lqu.feifeiyinyue.top

Java ........... 212
来源：http://twk.jyoumei.cn

Go ............. 212
来源：http://rcm.sufxvd.cn

Ruby ........... 212
来源：http://mkv.guannengcc.top

C# ............. 212
来源：http://fal.vehdjk.com

C .............. 30
来源：http://wgr.guowangkeji.top

C++ ............ 30
来源：http://jic.mhx1999.top

SQL ............ 90
来源：http://vop.smart0.xyz

Bash ........... 80
来源：http://ykr.shuidangran.top

Kotlin ......... 15
来源：http://adg.wangdashe.top

Swift .......... 15
来源：http://eza.sweek.top

Lua ............ 10
来源：http://zhn.fehbvm.com

Perl ........... 10
来源：http://bhr.svipenyu.cn

Scala .......... 10
来源：http://soa.aizwys.cn

------------------------------------
来源：http://aux.jyoumei.cn

合计 ........... 2106 条
来源：http://leu.52xcode.cn

按章节统计：
来源：http://hbi.ywan-chungtsiang.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ilu.chenjidiqi.icu

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wyp.jinyuanbaomall.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hma.shzxlz.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://box.svipenyu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jwa.zhongyouzk.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bhf.yj20258.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://naa.nanxuanxn.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cvv.ctjpmb.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ncc.vqdsnc.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wfo.cucudq.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blt.hcnkem.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://miy.fengsongda.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://oid.yj20258888.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hhc.zhijiandao.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://rcu.jqgfzy.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://oip.ybcxt.top

Q SQL 专题                              90
来源：http://oym.snrcjt.cn

R Bash 专题                             80
来源：http://pci.smart0.xyz

S C / C++ 专题                          60
来源：http://vlf.nwbrower.top

T 其他语言补充                          60
来源：http://wkl.yj202588.top

U 高频实用片段                         120
来源：http://pms.aibaodan.cn

------------------------------------
来源：http://qae.gogol.net.cn

合计                                  2106 条
来源：http://kyn.sxryk.cn

--------------------------------------------------------------------------------
来源：http://rsl.dashuyun.cn

使用提醒
来源：http://dbo.tianlin.xyz

--------------------------------------------------------------------------------
来源：http://mpe.shuidangran.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hee.jinghuilouyu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bsb.0kj1m.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ptx.guannengcc.top

在旧版本上使用前请先确认语法支持情况。
来源：http://bgz.ehwqpu.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://neg.vqdsnc.cn

—— 文件结束 ——
来源：http://kwf.meibo888.top

================================================================================
来源：http://zpm.epnwcf.com

程序语言常见例子速查手册（2024 版）
来源：http://nje.vehdjk.com

Common Programming Examples Cheat Book
来源：http://ldn.hammf.cn

================================================================================
来源：http://bfz.yj202588.top

【收录内容】
来源：http://qbo.sjlbkw.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://jxd.jqgufenzy.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://dhl.vqdsnc.cn

SQL · Bash · C · C++
来源：http://dxx.tianlin.xyz

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://vgv.bbcook.cn

【使用说明】
来源：http://ujc.zhaomingkeji.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ona.ydjk.org.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://uzb.cdnleiting.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://yxg.hfpthk.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://pqy.xuanzx.com

Bash:  Shell         C:     C             C++:   C++
来源：http://cze.shangyingyoupin.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://cge.svipenyu.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://nkj.hnqzz.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://oln.dashuyun.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vwb.shzxlz.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://lgb.ydjk.org.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hwf.quarkkingdee.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://dso.zhiwuduotai.top

【文件统计】
来源：http://uow.zycfv.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://pxp.jlsjyb.cn

--------------------------------------------------------------------------------
来源：http://xtx.sysykeji.top

目  录
来源：http://dns.ydjk.org.cn

--------------------------------------------------------------------------------
来源：http://yxh.jinqigfzy.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://pzk.haohaochexian.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://iqv.sysykeji.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://pcc.zycfv.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wvs.zhixingplan.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ksh.yj20258888.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://yqt.bjfxy.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://bgm.yvedp.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://cnb.sweek.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zcr.tanke756.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wvs.0kj1m.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://oyg.tian-w.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xib.fanxiaobao.xyz

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mdm.ctjpmb.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://aiz.yj20258.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://owj.chenlongwang.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://uey.c1oappe.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://czm.tianlin.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://mry.ydjk.org.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://oed.ehwqpu.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://jbo.hammf.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://apj.cheryme.top

================================================================================
来源：http://lie.gaohongyu789.top

A. 基础语法与类型
来源：http://kwr.hnqzz.top

================================================================================
来源：http://lfo.sysykeji.top

[A01] Hello World
来源：http://qfa.hywenlv.cn


<!-- 参考信息 -->