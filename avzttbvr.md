代发 wailian999

[U33] Py：打包发布
来源：http://hzi.yj20258888.top

python -m build  （依赖 pyproject.toml）
来源：http://xac.gzhubu.top

[U34] Py：判断编码
来源：http://cnu.smart0.xyz

chardet.detect(raw)
来源：http://mdk.sysykeji.top

[U35] Py：发送邮件
来源：http://eam.yuanzhike.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ljg.yj202588.top

[U36] Py：定时任务
来源：http://oyc.meibo888.top

schedule.every(10).minutes.do(job)
来源：http://hnc.havefunace.top

[U37] Py：读写 Excel
来源：http://fdf.cdnleiting.top

pandas.read_excel / DataFrame.to_excel
来源：http://gay.ybcxt.top

[U38] Py：获取脚本所在目录
来源：http://wfl.xingfuxueyuan.xyz

Path(__file__).resolve().parent
来源：http://jch.yanxiufei.cn

[U39] Py：判断是否在交互环境
来源：http://fpb.zhaomingkeji.xyz

sys.stdout.isatty()
来源：http://ned.chenjidiqi.icu

[U40] Py：打印到标准错误
来源：http://lhk.fktsv.cn

print("err", file=sys.stderr)
来源：http://npr.ivvv.top

[U41] PHP：初始化 Composer 项目
来源：http://zcs.xylfe.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ucn.ywan-chungtsiang.top

[U42] PHP：PSR-4 自动加载
来源：http://fub.hesvh.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xpl.zhijiandao.cn

[U43] PHP：声明命名空间
来源：http://tnz.svipenyu.cn

namespace App\Http;
来源：http://frl.yueranfly.top

[U44] PHP：开启严格类型
来源：http://bkc.jyoumei.cn

declare(strict_types=1);
来源：http://oot.guannengcc.top

[U45] PHP：类型声明与返回类型
来源：http://bqw.bjfxy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ted.wangshuangyany.cn

[U46] PHP：可空类型
来源：http://dub.yanxiufei.cn

?string $name = null
来源：http://emx.shuidangran.top

[U47] PHP：联合类型
来源：http://idw.tanke756.top

int|string $id
来源：http://ilt.ppjwa.cn

[U48] PHP：纯枚举
来源：http://bfa.daxiang520.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://izz.ppjwa.cn

[U49] PHP：只读属性
来源：http://ogz.vqdsnc.cn

public readonly string $name
来源：http://ocs.cashguo.top

[U50] PHP：构造器属性提升
来源：http://bpj.c1oappe.top

public function __construct(private int $id) {}
来源：http://cfg.shangyingyoupin.top

[U51] PHP：数组解构
来源：http://zmr.quarkkingdee.top

[$a, $b] = $arr;
来源：http://wnf.nwbrower.top

[U52] PHP：箭头函数
来源：http://hwz.tarul.cn

$double = fn($x) => $x * 2;
来源：http://zwc.dashuyun.cn

[U53] PHP：空合并运算符
来源：http://jcl.yangfankeji.com

$v = $a ?? $b ?? "default";
来源：http://eor.mhx1999.top

[U54] PHP：空安全调用
来源：http://rht.feifeiyinyue.top

$obj?->method()
来源：http://iaf.shanyushiyangtech.top

[U55] PHP：match 表达式
来源：http://fkr.tanke756.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kia.gzhubu.top

[U56] PHP：命名参数
来源：http://jis.feifeiyinyue.top

f(a: 1, b: 2)
来源：http://yzp.ybcxt.top

[U57] PHP：字符串插值
来源：http://oyl.bbcook.cn

"值: {$a}"
来源：http://cxz.iojbl.cn

[U58] PHP：数组三件套
来源：http://tss.svipenyu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cqc.tanke756.top

[U59] PHP：自定义排序
来源：http://ntl.wangshuangyany.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fzf.yongpay.top

[U60] PHP：JSON 编解码
来源：http://chr.jlsjyb.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://azb.birdmap.top

[U61] PHP：正则
来源：http://ssv.jqgufenzy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hwb.epnwcf.com

[U62] PHP：日期对象
来源：http://jrt.aibaodan.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fys.sweek.top

[U63] PHP：文件读写
来源：http://ltz.shanyushiyangtech.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mip.hywenlv.cn

[U64] PHP：目录遍历
来源：http://njp.tianlin.xyz

glob("dir/*.php");  scandir("dir");
来源：http://eae.ywan-chungtsiang.top

[U65] PHP：会话
来源：http://hap.xuanzx.com

session_start();  $_SESSION["uid"] = 1;
来源：http://tyc.ppjwa.cn

[U66] PHP：设置 Cookie
来源：http://hno.hongshengwenyu.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dlz.iojbl.cn

[U67] PHP：处理文件上传
来源：http://cry.smart0.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xim.wangdashe.top

[U68] PHP：PDO 连接
来源：http://iur.mhx1999.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://did.jiagoushi.top

[U69] PHP：PDO 预处理
来源：http://tfc.hnqzz.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nef.yuanzhike.top

[U70] PHP：PDO 事务
来源：http://ytd.zdbjq.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pej.havefunace.top

[U71] PHP：抛出异常
来源：http://ngq.sysykeji.top

throw new RuntimeException("失败", 500);
来源：http://fro.pycfn.com

[U72] PHP：写错误日志
来源：http://zpw.bbcook.cn

error_log("失败: " . $e->getMessage());
来源：http://ngd.andypj.xyz

[U73] PHP：读取 ini 配置
来源：http://plp.chenzaomai.com

parse_ini_file("config.ini", true)
来源：http://mry.hongshengwenyu.top

[U74] PHP：读取环境变量
来源：http://gtn.hnqzz.top

getenv("APP_ENV") ?: "production"
来源：http://bps.shanyushiyangtech.top

[U75] PHP：依赖注入
来源：http://vwf.yonumen.top

composer require psr/container
来源：http://ycb.chenlongwang.top

[U76] PHP：简单路由
来源：http://efi.svipenyu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ihe.hongshengwenyu.top

[U77] PHP：模板渲染
来源：http://ssh.pengpengdd.cyou

composer require twig/twig
来源：http://lcr.tian-w.cn

[U78] PHP：单元测试
来源：http://kgc.fengsongda.top

composer require --dev phpunit/phpunit
来源：http://rbn.birdmap.top

[U79] PHP：静态分析
来源：http://mvr.xziqi.cn

composer require --dev phpstan/phpstan
来源：http://kms.gotoacloud.top

[U80] PHP：代码规范修复
来源：http://dmt.iojbl.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://qzx.yuanzhike.top

[U81] JS：初始化项目
来源：http://myn.haohaochexian.top

npm init -y;  npm i express
来源：http://vhm.316326.xyz

[U82] JS：package.json 脚本
来源：http://cad.jianghu66.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ahj.sufxvd.cn

[U83] JS：ES Module 导入导出
来源：http://hzs.xuanzx.com

export const a = 1;  import { a } from "./m.js";
来源：http://wqz.fzhhl.top

[U84] JS：CommonJS 写法
来源：http://lvg.shzxlz.cn

module.exports = { a };  const { a } = require("./m");
来源：http://uzx.zhijiandao.cn

[U85] JS：可选链
来源：http://cci.yvedp.cn

a?.b?.c
来源：http://tzs.vehdjk.com

[U86] JS：空值合并
来源：http://ivk.yuanzhike.top

a ?? b
来源：http://knd.redwolf501.top

[U87] JS：解构默认值
来源：http://vpb.aibaodan.cn

const { a = 1, b = 2 } = obj;
来源：http://xoy.xinyue.icu

[U88] JS：对象展开合并
来源：http://ldv.ydzc1.top

{ ...a, ...b }
来源：http://xei.mhx1999.top

[U89] JS：数组去重
来源：http://ikw.nanxinkj.top

[...new Set(arr)]
来源：http://jod.jqgfzy.top

[U90] JS：数字数组排序
来源：http://qyc.fzhhl.top

[...arr].sort((a, b) => a - b)
来源：http://rjl.tanke756.top

[U91] JS：对象键值遍历
来源：http://wrg.tianlin.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bqo.birdmap.top

[U92] JS：深拷贝
来源：http://ugj.wangdashe.top

structuredClone(obj)
来源：http://wjx.zhaomingkeji.xyz

[U93] JS：模板字符串
来源：http://yij.bjfxy.top

`共 ${n} 条`
来源：http://ogl.9152youxi.cn

[U94] JS：箭头函数
来源：http://ayo.nanxinkj.top

const double = x => x * 2;
来源：http://juz.c1oappe.top

[U95] JS：Promise 包装
来源：http://six.yj20258.top

new Promise((resolve, reject) => {})
来源：http://fty.zdqjudy.top

[U96] JS：async/await 与异常
来源：http://scm.gzhubu.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xxr.uphjek.com

[U97] JS：并发请求
来源：http://msv.feifeiyinyue.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://pmv.zdqjudy.top

[U98] JS：fetch 带 JSON
来源：http://zco.zhaomingkeji.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vpr.iojbl.cn

[U99] JS：事件监听
来源：http://vqh.tanke756.top

el.addEventListener("click", e => {})
来源：http://vin.zdbjq.cn

[U100] JS：DOM 查询
来源：http://dwk.iojbl.cn

document.querySelector(".item")
来源：http://ynl.dianchejie.cn

[U101] JS：classList 操作
来源：http://iit.zycfv.cn

el.classList.toggle("active")
来源：http://czg.kuanghao11.cn

[U102] JS：本地存储
来源：http://ypv.cqqwz.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://afz.snrcjt.cn

[U103] JS：定时器
来源：http://svq.vehdjk.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zch.ydjk.org.cn

[U104] JS：防抖
来源：http://tvv.cucudq.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rgr.fengsongda.top

[U105] JS：节流
来源：http://ioj.hnxiangtu.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wjf.meibo888.top

[U106] JS：日期格式化
来源：http://lct.ywan-chungtsiang.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://oel.jinqigufen.top

[U107] JS：数字千分位
来源：http://vrv.vehdjk.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mai.jqgfzy.top

[U108] JS：随机整数
来源：http://zmp.tianlin.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://igj.svipenyu.cn

[U109] JS：数组分组
来源：http://gvp.zhaomingkeji.xyz

Object.groupBy(arr, x => x.type)
来源：http://xob.jinqigufen.top

[U110] JS：数组分块
来源：http://gsm.shzxlz.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pww.zdqjudy.top

[U111] JS：对象转 Map
来源：http://gor.cdnleiting.top

new Map(Object.entries(obj))
来源：http://sht.pengpengdd.cyou

[U112] JS：字符串补位
来源：http://bpk.hysaishi.cn

"7".padStart(3, "0")
来源：http://jhp.wangshuangyany.cn

[U113] JS：正则替换全部
来源：http://taw.shuidangran.top

s.replaceAll("a", "b")
来源：http://eui.zhongyouzk.top

[U114] JS：JSON 深比较
来源：http://fdr.yfazqb.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://dnp.wangshuangyany.cn

[U115] JS：生成 UUID
来源：http://tvd.yangfankeji.com

crypto.randomUUID()
来源：http://ozh.yvedp.cn

[U116] JS：类型检查（JSDoc）
来源：http://jjm.hammf.cn

/** @param {string} name */ function f(name) {}
来源：http://nov.jqgfzy.top

[U117] JS：单元测试
来源：http://hoh.zdqjudy.top

npm i -D vitest;  npx vitest
来源：http://pjc.dianchejie.cn

[U118] JS：开发服务器
来源：http://vwb.9152youxi.cn

npm i -D vite;  npx vite
来源：http://itg.yj20258888.top

[U119] JS：生产构建
来源：http://tsq.yj202588.top

npx vite build
来源：http://gkx.yueranfly.top

[U120] JS：读取环境变量（Vite）
来源：http://wvu.52xcode.cn

import.meta.env.VITE_API_URL
来源：http://vmi.vqdsnc.cn

================================================================================
来源：http://aqw.fanxiaobao.xyz

统计汇总
来源：http://yvw.zhoulong.xyz

================================================================================
来源：http://teb.hongshengwenyu.top

按语言统计（条）：
来源：http://xpv.quarkkingdee.top

Python ......... 252
来源：http://zye.iojbl.cn

PHP ............ 252
来源：http://yal.jyoumei.cn

JavaScript ..... 252
来源：http://jzu.epnwcf.com

TypeScript ..... 212
来源：http://etx.nwbrower.top

Java ........... 212
来源：http://now.hywenlv.cn

Go ............. 212
来源：http://yxg.dianchejie.cn

Ruby ........... 212
来源：http://ewr.wangshuangyany.cn

C# ............. 212
来源：http://pvg.ppjwa.cn

C .............. 30
来源：http://vuz.ctjpmb.com

C++ ............ 30
来源：http://uyk.zdbjq.cn

SQL ............ 90
来源：http://mgi.redwolf501.top

Bash ........... 80
来源：http://yjb.bjfxy.top

Kotlin ......... 15
来源：http://jsh.cashguo.top

Swift .......... 15
来源：http://isj.sweek.top

Lua ............ 10
来源：http://fon.9152youxi.cn

Perl ........... 10
来源：http://xff.sysykeji.top

Scala .......... 10
来源：http://wyi.shangyingyoupin.top

------------------------------------
来源：http://jkx.chenzaomai.com

合计 ........... 2106 条
来源：http://nqc.hnxiangtu.top

按章节统计：
来源：http://cqq.shanyushiyangtech.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dne.epnwcf.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://sgo.ywan-chungtsiang.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gru.yvedp.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://bow.zhengqikj.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wyu.c1oappe.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://jxg.hywenlv.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xxl.hammf.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cvv.haohaochexian.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jsn.sweek.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tip.aibaodan.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qvq.shuidangran.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vrt.jqgufenzy.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ugt.ydjk.org.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://fjl.cashguo.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fjo.shzxlz.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xaj.zhengqikj.top

Q SQL 专题                              90
来源：http://avf.svipenyu.cn

R Bash 专题                             80
来源：http://ztl.nanxuanxn.top

S C / C++ 专题                          60
来源：http://nbg.daria6918.cn

T 其他语言补充                          60
来源：http://sjb.jinqigfzy.top

U 高频实用片段                         120
来源：http://hvs.zdqjudy.top

------------------------------------
来源：http://zxz.ctjpmb.com

合计                                  2106 条
来源：http://wrb.sufxvd.cn

--------------------------------------------------------------------------------
来源：http://mqa.yanxiufei.cn

使用提醒
来源：http://iss.svipenyu.cn

--------------------------------------------------------------------------------
来源：http://vdb.jianghu66.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ucc.birdmap.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://eoe.redwolf501.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://sqd.jianghu66.top

在旧版本上使用前请先确认语法支持情况。
来源：http://nuq.jyoumei.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hci.zhongyouzk.top

—— 文件结束 ——
来源：http://nob.sxryk.cn

================================================================================
来源：http://wob.yangfankeji.com

程序语言常见例子速查手册（2024 版）
来源：http://wvg.xingfuxueyuan.xyz

Common Programming Examples Cheat Book
来源：http://yrr.tian-w.cn

================================================================================
来源：http://lmk.zhiwuduotai.top

【收录内容】
来源：http://qhm.haohaochexian.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://bdo.kuanghao11.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://syt.jqgfzy.top

SQL · Bash · C · C++
来源：http://ceq.hnqzz.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://tgj.zhongyouzk.top

【使用说明】
来源：http://ihs.hesvh.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wcd.yonumen.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://gpf.redwolf501.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mgb.shuidangran.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hxf.jinqigufen.top

Bash:  Shell         C:     C             C++:   C++
来源：http://fdb.daria6918.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ril.zhengqikj.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://xxu.zhoulong.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ggq.dashuyun.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://brs.cqqwz.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://uvn.fengsongda.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vke.bjfxy.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kjn.pycfn.com

【文件统计】
来源：http://fpp.cashguo.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ilf.shanyushiyangkeji.top

--------------------------------------------------------------------------------
来源：http://vea.andypj.xyz

目  录
来源：http://wit.yongpay.top

--------------------------------------------------------------------------------
来源：http://apu.ydzc1.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wfy.guowangkeji.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://jsd.hongshengwenyu.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://aav.dianchejie.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zoq.hongshengwenyu.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://gmq.hfpthk.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ubc.guowangkeji.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://bph.shangyingyoupin.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://rnj.fengsongda.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hjw.jinqigufen.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://cbz.jinyuanbaomall.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zln.dashuyun.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://fhv.zhengqikj.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qtv.sysykeji.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://jca.ybcxt.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://bfa.wangdashe.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ydf.cucudq.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://spk.daxiang520.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://ivq.quarkkingdee.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://oxk.jinghuilouyu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://dfs.sweek.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://uwa.ybcxt.top

================================================================================
来源：http://jhx.shzxlz.cn

A. 基础语法与类型
来源：http://npj.chenzaomai.com

================================================================================
来源：http://ygo.yanxiufei.cn

[A01] Hello World
来源：http://vdz.jyoumei.cn

Py:   print("Hello, World!")
来源：http://jdi.gzhubu.top

PHP:  echo "Hello, World!";
来源：http://coh.yuxming.cn

JS:   console.log("Hello, World!");
来源：http://fcr.cheryme.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ssf.hfpthk.cn

Java: System.out.println("Hello, World!");
来源：http://nii.daria6918.cn

Go:   fmt.Println("Hello, World!")
来源：http://jid.jqgfzy.top

Ruby: puts "Hello, World!"
来源：http://kku.jlsjyb.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://zco.nanxuanxn.top

[A02] 变量声明与赋值
来源：http://xjl.hnqzz.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hxg.wangshuangyany.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://xry.haohaochexian.top

JS:   let name = "Alex"; const age = 20;
来源：http://jpr.zdbjq.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://khp.chenzaomai.com

Java: String name = "Alex"; int age = 20;
来源：http://wgd.c1oappe.top

Go:   name := "Alex"; age := 20
来源：http://yoy.aibaodan.cn

Ruby: name = "Alex"; age = 20
来源：http://fdw.pengpengdd.cyou


<!-- 参考信息 -->