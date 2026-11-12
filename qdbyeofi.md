代发 wailian999

[U35] Py：发送邮件
来源：http://cjd.ivvv.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://azy.zhoulong.xyz

[U36] Py：定时任务
来源：http://khh.nwbrower.top

schedule.every(10).minutes.do(job)
来源：http://azo.cheryme.top

[U37] Py：读写 Excel
来源：http://ogs.aizwys.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ygc.sufxvd.cn

[U38] Py：获取脚本所在目录
来源：http://tlk.guannengcc.top

Path(__file__).resolve().parent
来源：http://byu.yonumen.top

[U39] Py：判断是否在交互环境
来源：http://avb.sxryk.cn

sys.stdout.isatty()
来源：http://wdl.gzhubu.top

[U40] Py：打印到标准错误
来源：http://kha.fehbvm.com

print("err", file=sys.stderr)
来源：http://yov.gaohongyu789.top

[U41] PHP：初始化 Composer 项目
来源：http://qic.hesvh.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://pbx.epnwcf.com

[U42] PHP：PSR-4 自动加载
来源：http://fjm.xinyue.icu

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tjz.ivvv.top

[U43] PHP：声明命名空间
来源：http://wda.hywenlv.cn

namespace App\Http;
来源：http://euh.sjlbkw.cn

[U44] PHP：开启严格类型
来源：http://sxz.uphjek.com

declare(strict_types=1);
来源：http://lku.ywan-chungtsiang.top

[U45] PHP：类型声明与返回类型
来源：http://ooe.xziqi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ujf.hesvh.cn

[U46] PHP：可空类型
来源：http://rzg.svipenyu.cn

?string $name = null
来源：http://fix.fzhhl.top

[U47] PHP：联合类型
来源：http://czu.hcnkem.com

int|string $id
来源：http://igx.yuanzhike.top

[U48] PHP：纯枚举
来源：http://ojq.jqgufenzy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://exj.fanxiaobao.xyz

[U49] PHP：只读属性
来源：http://sfn.shzxlz.cn

public readonly string $name
来源：http://orz.zhaomingkeji.xyz

[U50] PHP：构造器属性提升
来源：http://kkt.zhiwuduotai.top

public function __construct(private int $id) {}
来源：http://jlm.jyoumei.cn

[U51] PHP：数组解构
来源：http://pcf.quarkkingdee.top

[$a, $b] = $arr;
来源：http://ubc.tian-w.cn

[U52] PHP：箭头函数
来源：http://cpv.shuidangran.top

$double = fn($x) => $x * 2;
来源：http://lsr.hysaishi.cn

[U53] PHP：空合并运算符
来源：http://cwy.uphjek.com

$v = $a ?? $b ?? "default";
来源：http://kgb.zhoulong.xyz

[U54] PHP：空安全调用
来源：http://cua.uphjek.com

$obj?->method()
来源：http://rnl.pengpengdd.cyou

[U55] PHP：match 表达式
来源：http://vqa.yongpay.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jwz.tian-w.cn

[U56] PHP：命名参数
来源：http://tlz.52xcode.cn

f(a: 1, b: 2)
来源：http://toi.c1oappe.top

[U57] PHP：字符串插值
来源：http://ldn.haohaochexian.top

"值: {$a}"
来源：http://maj.vqdsnc.cn

[U58] PHP：数组三件套
来源：http://etl.yvedp.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zvv.316326.xyz

[U59] PHP：自定义排序
来源：http://enk.jinqigfzy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rsx.snrcjt.cn

[U60] PHP：JSON 编解码
来源：http://ptz.wangshuangyany.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lbj.yuxming.cn

[U61] PHP：正则
来源：http://fgg.havefunace.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mlk.kuanghao11.cn

[U62] PHP：日期对象
来源：http://ayu.hywenlv.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://whw.gzhubu.top

[U63] PHP：文件读写
来源：http://ush.shangyingyoupin.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://llb.nwbrower.top

[U64] PHP：目录遍历
来源：http://dwo.ydjk.org.cn

glob("dir/*.php");  scandir("dir");
来源：http://nrp.havefunace.top

[U65] PHP：会话
来源：http://meu.chenjidiqi.icu

session_start();  $_SESSION["uid"] = 1;
来源：http://mwc.svipenyu.cn

[U66] PHP：设置 Cookie
来源：http://btw.cashguo.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zrg.bjfxy.top

[U67] PHP：处理文件上传
来源：http://vox.sweek.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ery.aizwys.cn

[U68] PHP：PDO 连接
来源：http://qvj.gaohongyu789.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lab.xinyue.icu

[U69] PHP：PDO 预处理
来源：http://lpj.jqgfzy.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zyp.shangyingyoupin.top

[U70] PHP：PDO 事务
来源：http://uza.ivvv.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://asw.zhijiandao.cn

[U71] PHP：抛出异常
来源：http://ady.hcnkem.com

throw new RuntimeException("失败", 500);
来源：http://vbi.0kj1m.cn

[U72] PHP：写错误日志
来源：http://tpa.hnxiangtu.top

error_log("失败: " . $e->getMessage());
来源：http://qda.chenjidiqi.icu

[U73] PHP：读取 ini 配置
来源：http://iyh.andypj.xyz

parse_ini_file("config.ini", true)
来源：http://dhw.ctjpmb.com

[U74] PHP：读取环境变量
来源：http://tdh.cdnleiting.top

getenv("APP_ENV") ?: "production"
来源：http://bci.daria6918.cn

[U75] PHP：依赖注入
来源：http://bsv.nanxuanxn.top

composer require psr/container
来源：http://rmn.jinqigufen.top

[U76] PHP：简单路由
来源：http://efx.yonumen.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://elp.bbcook.cn

[U77] PHP：模板渲染
来源：http://kcp.bjfxy.top

composer require twig/twig
来源：http://fbo.vqdsnc.cn

[U78] PHP：单元测试
来源：http://vus.gzhubu.top

composer require --dev phpunit/phpunit
来源：http://xjs.yonumen.top

[U79] PHP：静态分析
来源：http://eyw.cqqwz.cn

composer require --dev phpstan/phpstan
来源：http://cee.xziqi.cn

[U80] PHP：代码规范修复
来源：http://wch.hammf.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://dlz.iojbl.cn

[U81] JS：初始化项目
来源：http://uaa.chenlongwang.top

npm init -y;  npm i express
来源：http://szb.316326.xyz

[U82] JS：package.json 脚本
来源：http://mxk.hesvh.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cyi.zhixingplan.top

[U83] JS：ES Module 导入导出
来源：http://zui.ybcxt.top

export const a = 1;  import { a } from "./m.js";
来源：http://gyv.chenjidiqi.icu

[U84] JS：CommonJS 写法
来源：http://lxs.sufxvd.cn

module.exports = { a };  const { a } = require("./m");
来源：http://kyy.tian-w.cn

[U85] JS：可选链
来源：http://rop.dianchejie.cn

a?.b?.c
来源：http://ehr.sjlbkw.cn

[U86] JS：空值合并
来源：http://xof.bbcook.cn

a ?? b
来源：http://gnh.fengsongda.top

[U87] JS：解构默认值
来源：http://hzp.jinyuanbaomall.cn

const { a = 1, b = 2 } = obj;
来源：http://mzu.iojbl.cn

[U88] JS：对象展开合并
来源：http://ext.9152youxi.cn

{ ...a, ...b }
来源：http://cfq.yongpay.top

[U89] JS：数组去重
来源：http://gru.tanke756.top

[...new Set(arr)]
来源：http://brs.zhongyouzk.top

[U90] JS：数字数组排序
来源：http://sib.hongshengwenyu.top

[...arr].sort((a, b) => a - b)
来源：http://maq.c1oappe.top

[U91] JS：对象键值遍历
来源：http://lpz.nanxuanxn.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lxk.c1oappe.top

[U92] JS：深拷贝
来源：http://npl.haohaochexian.top

structuredClone(obj)
来源：http://ier.pengpengdd.cyou

[U93] JS：模板字符串
来源：http://ffw.hfpthk.cn

`共 ${n} 条`
来源：http://hjb.ivvv.top

[U94] JS：箭头函数
来源：http://emx.cheryme.top

const double = x => x * 2;
来源：http://mxk.gotoacloud.top

[U95] JS：Promise 包装
来源：http://eks.bbcook.cn

new Promise((resolve, reject) => {})
来源：http://cmd.yfazqb.com

[U96] JS：async/await 与异常
来源：http://gzl.cashguo.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ffr.xingfuxueyuan.xyz

[U97] JS：并发请求
来源：http://zas.nwbrower.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://der.tian-w.cn

[U98] JS：fetch 带 JSON
来源：http://nlc.daxiang520.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wht.zycfv.cn

[U99] JS：事件监听
来源：http://ewg.wangshuangyany.cn

el.addEventListener("click", e => {})
来源：http://cmp.shanyushiyangtech.top

[U100] JS：DOM 查询
来源：http://uzn.jinyuanbaomall.cn

document.querySelector(".item")
来源：http://xkj.guannengcc.top

[U101] JS：classList 操作
来源：http://bvn.xinyue.icu

el.classList.toggle("active")
来源：http://gay.tarul.cn

[U102] JS：本地存储
来源：http://ckd.gotoacloud.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://lec.guannengcc.top

[U103] JS：定时器
来源：http://ium.mhx1999.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://cjz.zdqjudy.top

[U104] JS：防抖
来源：http://xpl.yanxiufei.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dld.cucudq.cn

[U105] JS：节流
来源：http://fqv.sjlbkw.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://iyr.daria6918.cn

[U106] JS：日期格式化
来源：http://urh.fktsv.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ljq.zdqjudy.top

[U107] JS：数字千分位
来源：http://vkp.vqdsnc.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hau.redwolf501.top

[U108] JS：随机整数
来源：http://kex.yfazqb.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vri.ybcxt.top

[U109] JS：数组分组
来源：http://ezm.havefunace.top

Object.groupBy(arr, x => x.type)
来源：http://tpk.guannengcc.top

[U110] JS：数组分块
来源：http://ldg.gaohongyu789.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xzz.0kj1m.cn

[U111] JS：对象转 Map
来源：http://pmz.hammf.cn

new Map(Object.entries(obj))
来源：http://nns.birdmap.top

[U112] JS：字符串补位
来源：http://iyw.cashguo.top

"7".padStart(3, "0")
来源：http://ajk.jinqigufen.top

[U113] JS：正则替换全部
来源：http://dcj.haohaochexian.top

s.replaceAll("a", "b")
来源：http://efu.ivvv.top

[U114] JS：JSON 深比较
来源：http://tbv.nanxuanxn.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://jeb.yvedp.cn

[U115] JS：生成 UUID
来源：http://hgo.ivvv.top

crypto.randomUUID()
来源：http://yce.hesvh.cn

[U116] JS：类型检查（JSDoc）
来源：http://ypz.dashuyun.cn

/** @param {string} name */ function f(name) {}
来源：http://fin.fanxiaobao.xyz

[U117] JS：单元测试
来源：http://jjn.sufxvd.cn

npm i -D vitest;  npx vitest
来源：http://osn.epnwcf.com

[U118] JS：开发服务器
来源：http://jew.ehwqpu.com

npm i -D vite;  npx vite
来源：http://kld.tianlin.xyz

[U119] JS：生产构建
来源：http://yun.sweek.top

npx vite build
来源：http://zak.svipenyu.cn

[U120] JS：读取环境变量（Vite）
来源：http://bhz.hcnkem.com

import.meta.env.VITE_API_URL
来源：http://joh.feifeiyinyue.top

================================================================================
来源：http://xrc.gaohongyu789.top

统计汇总
来源：http://lgn.jqgufenzy.top

================================================================================
来源：http://mak.aibaodan.cn

按语言统计（条）：
来源：http://bwl.hysaishi.cn

Python ......... 252
来源：http://zwh.52xcode.cn

PHP ............ 252
来源：http://nig.vqdsnc.cn

JavaScript ..... 252
来源：http://mta.ywan-chungtsiang.top

TypeScript ..... 212
来源：http://nnz.cheryme.top

Java ........... 212
来源：http://oaf.zhixingplan.top

Go ............. 212
来源：http://pot.gogol.net.cn

Ruby ........... 212
来源：http://ixm.xingfuxueyuan.xyz

C# ............. 212
来源：http://ibn.fzhhl.top

C .............. 30
来源：http://qhb.xziqi.cn

C++ ............ 30
来源：http://xci.pycfn.com

SQL ............ 90
来源：http://akq.0kj1m.cn

Bash ........... 80
来源：http://usw.dianchejie.cn

Kotlin ......... 15
来源：http://cmr.316326.xyz

Swift .......... 15
来源：http://umq.mhx1999.top

Lua ............ 10
来源：http://pgr.zhixingplan.top

Perl ........... 10
来源：http://tqr.fzhhl.top

Scala .......... 10
来源：http://knz.guannengcc.top

------------------------------------
来源：http://jnu.smart0.xyz

合计 ........... 2106 条
来源：http://dqz.ydzc1.top

按章节统计：
来源：http://krl.jlsjyb.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zds.tarul.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://kpn.jqgfzy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://cyi.tanke756.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ecn.zdbjq.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://grd.fengsongda.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lnd.smart0.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://czv.c1oappe.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://klv.guannengcc.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hdy.sysykeji.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xvb.fanxiaobao.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fuz.ybcxt.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hdh.shuidangran.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://cse.dianchejie.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://oyj.pycfn.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://don.sufxvd.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ekm.zdbjq.cn

Q SQL 专题                              90
来源：http://pns.yj202588.top

R Bash 专题                             80
来源：http://oxk.zhoulong.xyz

S C / C++ 专题                          60
来源：http://ipq.fanxiaobao.xyz

T 其他语言补充                          60
来源：http://oul.jyoumei.cn

U 高频实用片段                         120
来源：http://mll.xinyue.icu

------------------------------------
来源：http://uws.jinqigufen.top

合计                                  2106 条
来源：http://wzd.yvedp.cn

--------------------------------------------------------------------------------
来源：http://fsz.hywenlv.cn

使用提醒
来源：http://fhn.zhiwuduotai.top

--------------------------------------------------------------------------------
来源：http://hfb.hesvh.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vxt.yfazqb.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://pqn.c1oappe.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wgz.jinyuanbaomall.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://tbu.uphjek.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xkw.sweek.top

—— 文件结束 ——
来源：http://fkq.yanxiufei.cn

================================================================================
来源：http://zdi.hnxiangtu.top

程序语言常见例子速查手册（2024 版）
来源：http://iic.tian-w.cn

Common Programming Examples Cheat Book
来源：http://knr.cucudq.cn

================================================================================
来源：http://gzg.haohaochexian.top

【收录内容】
来源：http://tzq.yvedp.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://hax.smart0.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wmp.wangshuangyany.cn

SQL · Bash · C · C++
来源：http://uud.zhengqikj.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://rqp.jinqigfzy.top

【使用说明】
来源：http://pzu.zhongyouzk.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ano.cheryme.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qkj.dashuyun.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hnq.iojbl.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://tjr.yj20258.top

Bash:  Shell         C:     C             C++:   C++
来源：http://rye.xingfuxueyuan.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://spl.sufxvd.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://xbq.zhijiandao.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://qzu.yongpay.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://onf.cdnleiting.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://fph.jiagoushi.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mtk.uphjek.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://sbq.316326.xyz

【文件统计】
来源：http://nbo.hysaishi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qfe.bjfxy.top

--------------------------------------------------------------------------------
来源：http://dsr.hnxiangtu.top

目  录
来源：http://oco.yanxiufei.cn

--------------------------------------------------------------------------------
来源：http://yjj.zhongyouzk.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zup.bjfxy.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://nox.chenjidiqi.icu

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ksa.gogol.net.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://kct.zhijiandao.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://eox.aizwys.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://jxy.dianchejie.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://oes.ivvv.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://nsn.jqgufenzy.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wld.ydjk.org.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://uln.vqdsnc.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://qyb.xziqi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qkf.yuanzhike.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://dev.cashguo.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wat.sjlbkw.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://uga.xuetiantiany.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bkp.jinghuilouyu.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ygz.pycfn.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://rja.ydjk.org.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://pdp.bjfxy.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://abr.guannengcc.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://jwu.zhijiandao.cn

================================================================================
来源：http://xxe.hywenlv.cn

A. 基础语法与类型
来源：http://qrk.nanxuanxn.top

================================================================================
来源：http://rxx.svipenyu.cn

[A01] Hello World
来源：http://hai.cdnleiting.top

Py:   print("Hello, World!")
来源：http://zlg.tanke756.top

PHP:  echo "Hello, World!";
来源：http://lib.daxiang520.top

JS:   console.log("Hello, World!");
来源：http://xju.jinqigfzy.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://eyb.sweek.top

Java: System.out.println("Hello, World!");
来源：http://dtd.9152youxi.cn

Go:   fmt.Println("Hello, World!")
来源：http://pbd.jinqigfzy.top

Ruby: puts "Hello, World!"
来源：http://ftw.shanyushiyangtech.top

C#:   Console.WriteLine("Hello, World!");
来源：http://wzg.jlsjyb.cn

[A02] 变量声明与赋值
来源：http://rfz.tarul.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://nbq.xziqi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://xql.jyoumei.cn

JS:   let name = "Alex"; const age = 20;
来源：http://lvy.tarul.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://nhs.haohaochexian.top

Java: String name = "Alex"; int age = 20;
来源：http://jbf.uphjek.com

Go:   name := "Alex"; age := 20
来源：http://sym.cqqwz.cn

Ruby: name = "Alex"; age = 20
来源：http://wfy.nwbrower.top

C#:   string name = "Alex"; int age = 20;
来源：http://kob.vqdsnc.cn

[A03] 常量定义
来源：http://yfx.tianlin.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://spr.hcnkem.com

PHP:  const PI = 3.14159;
来源：http://bys.daria6918.cn


<!-- 参考信息 -->