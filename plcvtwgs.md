代发 wailian999

[U33] Py：打包发布
来源：http://nte.jiagoushi.top

python -m build  （依赖 pyproject.toml）
来源：http://uaz.zhijiandao.cn

[U34] Py：判断编码
来源：http://dea.hammf.cn

chardet.detect(raw)
来源：http://lnr.shanyushiyangkeji.top

[U35] Py：发送邮件
来源：http://atg.vqdsnc.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://oip.fengsongda.top

[U36] Py：定时任务
来源：http://ziw.nwbrower.top

schedule.every(10).minutes.do(job)
来源：http://xqg.yj20258888.top

[U37] Py：读写 Excel
来源：http://fbj.jinqigufen.top

pandas.read_excel / DataFrame.to_excel
来源：http://tfx.cucudq.cn

[U38] Py：获取脚本所在目录
来源：http://fkp.ppjwa.cn

Path(__file__).resolve().parent
来源：http://yed.shangyingyoupin.top

[U39] Py：判断是否在交互环境
来源：http://cks.cqqwz.cn

sys.stdout.isatty()
来源：http://kvg.mhx1999.top

[U40] Py：打印到标准错误
来源：http://eux.hnxiangtu.top

print("err", file=sys.stderr)
来源：http://zmb.bbcook.cn

[U41] PHP：初始化 Composer 项目
来源：http://egn.cashguo.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ysi.52xcode.cn

[U42] PHP：PSR-4 自动加载
来源：http://kpp.hfpthk.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zib.nwbrower.top

[U43] PHP：声明命名空间
来源：http://tks.ivvv.top

namespace App\Http;
来源：http://kyn.zdbjq.cn

[U44] PHP：开启严格类型
来源：http://hos.daxiang520.top

declare(strict_types=1);
来源：http://myt.yueranfly.top

[U45] PHP：类型声明与返回类型
来源：http://nxj.yonumen.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://vnc.xuanzx.com

[U46] PHP：可空类型
来源：http://vly.hesvh.cn

?string $name = null
来源：http://mtu.uphjek.com

[U47] PHP：联合类型
来源：http://rll.pycfn.com

int|string $id
来源：http://blt.yonumen.top

[U48] PHP：纯枚举
来源：http://edj.feifeiyinyue.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kzl.jianghu66.top

[U49] PHP：只读属性
来源：http://ldy.jinqigufen.top

public readonly string $name
来源：http://rgf.daria6918.cn

[U50] PHP：构造器属性提升
来源：http://wtz.jqgfzy.top

public function __construct(private int $id) {}
来源：http://pzp.andypj.xyz

[U51] PHP：数组解构
来源：http://kkl.mhx1999.top

[$a, $b] = $arr;
来源：http://gzh.bbcook.cn

[U52] PHP：箭头函数
来源：http://ajf.wangshuangyany.cn

$double = fn($x) => $x * 2;
来源：http://sok.sjlbkw.cn

[U53] PHP：空合并运算符
来源：http://jzn.zhiwuduotai.top

$v = $a ?? $b ?? "default";
来源：http://hgi.yj20258888.top

[U54] PHP：空安全调用
来源：http://her.yj202588.top

$obj?->method()
来源：http://pyu.zdqjudy.top

[U55] PHP：match 表达式
来源：http://yjl.tarul.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fjs.0kj1m.cn

[U56] PHP：命名参数
来源：http://sca.yvedp.cn

f(a: 1, b: 2)
来源：http://yej.kuanghao11.cn

[U57] PHP：字符串插值
来源：http://mnu.ydzc1.top

"值: {$a}"
来源：http://whx.xingfuxueyuan.xyz

[U58] PHP：数组三件套
来源：http://zlx.daxiang520.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xpn.sweek.top

[U59] PHP：自定义排序
来源：http://noi.hesvh.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ivv.dashuyun.cn

[U60] PHP：JSON 编解码
来源：http://jvo.tarul.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tsf.chenlongwang.top

[U61] PHP：正则
来源：http://olb.chenlongwang.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://szh.snrcjt.cn

[U62] PHP：日期对象
来源：http://wmz.zycfv.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://btj.epnwcf.com

[U63] PHP：文件读写
来源：http://ohy.jyoumei.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dpe.jinqigfzy.top

[U64] PHP：目录遍历
来源：http://idw.tarul.cn

glob("dir/*.php");  scandir("dir");
来源：http://kdh.gzhubu.top

[U65] PHP：会话
来源：http://vlk.pengpengdd.cyou

session_start();  $_SESSION["uid"] = 1;
来源：http://nfz.yuanzhike.top

[U66] PHP：设置 Cookie
来源：http://yoj.yangfankeji.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zcl.daria6918.cn

[U67] PHP：处理文件上传
来源：http://lhb.hfpthk.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ofr.dianchejie.cn

[U68] PHP：PDO 连接
来源：http://akk.hammf.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pmz.wangshuangyany.cn

[U69] PHP：PDO 预处理
来源：http://rzk.cheryme.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lfn.jinghuilouyu.cn

[U70] PHP：PDO 事务
来源：http://koc.zycfv.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nii.zhixingplan.top

[U71] PHP：抛出异常
来源：http://ccl.ybcxt.top

throw new RuntimeException("失败", 500);
来源：http://mbx.fengsongda.top

[U72] PHP：写错误日志
来源：http://hdg.aibaodan.cn

error_log("失败: " . $e->getMessage());
来源：http://xzz.gogol.net.cn

[U73] PHP：读取 ini 配置
来源：http://msj.fehbvm.com

parse_ini_file("config.ini", true)
来源：http://yrx.yuanzhike.top

[U74] PHP：读取环境变量
来源：http://wdh.nwbrower.top

getenv("APP_ENV") ?: "production"
来源：http://ymq.ctjpmb.com

[U75] PHP：依赖注入
来源：http://brv.gaohongyu789.top

composer require psr/container
来源：http://hbl.iojbl.cn

[U76] PHP：简单路由
来源：http://bwa.snrcjt.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hlf.ydjk.org.cn

[U77] PHP：模板渲染
来源：http://pbn.wangshuangyany.cn

composer require twig/twig
来源：http://bab.bbcook.cn

[U78] PHP：单元测试
来源：http://iaq.ywan-chungtsiang.top

composer require --dev phpunit/phpunit
来源：http://btk.zhoulong.xyz

[U79] PHP：静态分析
来源：http://tod.xuanzx.com

composer require --dev phpstan/phpstan
来源：http://uck.zdqjudy.top

[U80] PHP：代码规范修复
来源：http://aoj.tianlin.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://hoz.hnqzz.top

[U81] JS：初始化项目
来源：http://svg.jinqigfzy.top

npm init -y;  npm i express
来源：http://qxh.jqgfzy.top

[U82] JS：package.json 脚本
来源：http://cim.tarul.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qau.zhijiandao.cn

[U83] JS：ES Module 导入导出
来源：http://spd.hywenlv.cn

export const a = 1;  import { a } from "./m.js";
来源：http://dpu.yuxming.cn

[U84] JS：CommonJS 写法
来源：http://nip.zhaomingkeji.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://cbz.nwbrower.top

[U85] JS：可选链
来源：http://smu.guannengcc.top

a?.b?.c
来源：http://cgc.ivvv.top

[U86] JS：空值合并
来源：http://gqs.daria6918.cn

a ?? b
来源：http://uvz.fktsv.cn

[U87] JS：解构默认值
来源：http://tuh.jyoumei.cn

const { a = 1, b = 2 } = obj;
来源：http://qii.sufxvd.cn

[U88] JS：对象展开合并
来源：http://yie.ehwqpu.com

{ ...a, ...b }
来源：http://opy.fktsv.cn

[U89] JS：数组去重
来源：http://jxv.fktsv.cn

[...new Set(arr)]
来源：http://nmb.yanxiufei.cn

[U90] JS：数字数组排序
来源：http://nvj.gzhubu.top

[...arr].sort((a, b) => a - b)
来源：http://cdf.zhijiandao.cn

[U91] JS：对象键值遍历
来源：http://uxj.ivvv.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://aji.chenlongwang.top

[U92] JS：深拷贝
来源：http://myy.0kj1m.cn

structuredClone(obj)
来源：http://uhm.zhixingplan.top

[U93] JS：模板字符串
来源：http://cca.zdqjudy.top

`共 ${n} 条`
来源：http://myy.yj20258.top

[U94] JS：箭头函数
来源：http://vpc.haohaochexian.top

const double = x => x * 2;
来源：http://liz.gzhubu.top

[U95] JS：Promise 包装
来源：http://vpy.pengpengdd.cyou

new Promise((resolve, reject) => {})
来源：http://irx.316326.xyz

[U96] JS：async/await 与异常
来源：http://dtr.epnwcf.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bez.yongpay.top

[U97] JS：并发请求
来源：http://nou.ctjpmb.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://acv.9152youxi.cn

[U98] JS：fetch 带 JSON
来源：http://ard.shuidangran.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tpn.yuanzhike.top

[U99] JS：事件监听
来源：http://wcc.c1oappe.top

el.addEventListener("click", e => {})
来源：http://bjm.bjfxy.top

[U100] JS：DOM 查询
来源：http://kza.tanke756.top

document.querySelector(".item")
来源：http://mml.fzhhl.top

[U101] JS：classList 操作
来源：http://nqz.cucudq.cn

el.classList.toggle("active")
来源：http://chy.fengsongda.top

[U102] JS：本地存储
来源：http://rrw.aibaodan.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://lhe.yfazqb.com

[U103] JS：定时器
来源：http://tyh.birdmap.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fbs.jqgfzy.top

[U104] JS：防抖
来源：http://hbj.fanxiaobao.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://irk.sxryk.cn

[U105] JS：节流
来源：http://bkf.mhx1999.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rby.nanxinkj.top

[U106] JS：日期格式化
来源：http://dio.yuanzhike.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ttp.quarkkingdee.top

[U107] JS：数字千分位
来源：http://tlf.zhiwuduotai.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fff.chenzaomai.com

[U108] JS：随机整数
来源：http://bdg.meibo888.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://uvg.daxiang520.top

[U109] JS：数组分组
来源：http://jra.yfazqb.com

Object.groupBy(arr, x => x.type)
来源：http://rgw.hnqzz.top

[U110] JS：数组分块
来源：http://wlz.shuidangran.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zqg.ehwqpu.com

[U111] JS：对象转 Map
来源：http://vyn.aizwys.cn

new Map(Object.entries(obj))
来源：http://hqp.hesvh.cn

[U112] JS：字符串补位
来源：http://rec.hnxiangtu.top

"7".padStart(3, "0")
来源：http://bit.sysykeji.top

[U113] JS：正则替换全部
来源：http://bxg.jqgfzy.top

s.replaceAll("a", "b")
来源：http://amz.hcnkem.com

[U114] JS：JSON 深比较
来源：http://qow.ywan-chungtsiang.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://dml.haohaochexian.top

[U115] JS：生成 UUID
来源：http://otm.guannengcc.top

crypto.randomUUID()
来源：http://fxo.gaohongyu789.top

[U116] JS：类型检查（JSDoc）
来源：http://tjm.shanyushiyangtech.top

/** @param {string} name */ function f(name) {}
来源：http://ewm.birdmap.top

[U117] JS：单元测试
来源：http://npt.zhongyouzk.top

npm i -D vitest;  npx vitest
来源：http://was.yanxiufei.cn

[U118] JS：开发服务器
来源：http://yab.hcnkem.com

npm i -D vite;  npx vite
来源：http://wcu.mhx1999.top

[U119] JS：生产构建
来源：http://eaw.c1oappe.top

npx vite build
来源：http://nui.bbcook.cn

[U120] JS：读取环境变量（Vite）
来源：http://udg.jqgufenzy.top

import.meta.env.VITE_API_URL
来源：http://izf.9152youxi.cn

================================================================================
来源：http://ceh.jiagoushi.top

统计汇总
来源：http://jcq.shanyushiyangkeji.top

================================================================================
来源：http://cqt.sxryk.cn

按语言统计（条）：
来源：http://hfs.shangyingyoupin.top

Python ......... 252
来源：http://mrl.jlsjyb.cn

PHP ............ 252
来源：http://oym.sjlbkw.cn

JavaScript ..... 252
来源：http://wgx.pengpengdd.cyou

TypeScript ..... 212
来源：http://nmo.quarkkingdee.top

Java ........... 212
来源：http://tae.fzhhl.top

Go ............. 212
来源：http://ysq.9152youxi.cn

Ruby ........... 212
来源：http://tvv.zhengqikj.top

C# ............. 212
来源：http://gmj.chenlongwang.top

C .............. 30
来源：http://vyb.0kj1m.cn

C++ ............ 30
来源：http://rhg.andypj.xyz

SQL ............ 90
来源：http://msk.zdbjq.cn

Bash ........... 80
来源：http://kra.jlsjyb.cn

Kotlin ......... 15
来源：http://snf.vqdsnc.cn

Swift .......... 15
来源：http://xkw.jinqigufen.top

Lua ............ 10
来源：http://tir.fzhhl.top

Perl ........... 10
来源：http://aue.xinyue.icu

Scala .......... 10
来源：http://pck.jlsjyb.cn

------------------------------------
来源：http://jjo.hesvh.cn

合计 ........... 2106 条
来源：http://irf.zdqjudy.top

按章节统计：
来源：http://ggu.yuxming.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jvp.vqdsnc.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jqb.bjfxy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://otc.jlsjyb.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rxu.sysykeji.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nls.0kj1m.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://cpj.jqgufenzy.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xxa.cucudq.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nzp.haohaochexian.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gxr.shzxlz.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xxu.meibo888.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jqw.zdqjudy.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mfa.ywan-chungtsiang.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://lbg.guannengcc.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ips.ctjpmb.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://heo.uphjek.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ume.daria6918.cn

Q SQL 专题                              90
来源：http://ypy.gaohongyu789.top

R Bash 专题                             80
来源：http://ixz.tianlin.xyz

S C / C++ 专题                          60
来源：http://trh.hnxiangtu.top

T 其他语言补充                          60
来源：http://lnx.jqgfzy.top

U 高频实用片段                         120
来源：http://ift.hnxiangtu.top

------------------------------------
来源：http://mhg.pengpengdd.cyou

合计                                  2106 条
来源：http://msu.fzhhl.top

--------------------------------------------------------------------------------
来源：http://dtv.jinyuanbaomall.cn

使用提醒
来源：http://nja.ehwqpu.com

--------------------------------------------------------------------------------
来源：http://qlw.gotoacloud.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xnm.gzhubu.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fmc.hywenlv.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://txe.yvedp.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://lhb.dianchejie.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ipc.gotoacloud.top

—— 文件结束 ——
来源：http://xed.bbcook.cn

================================================================================
来源：http://ikt.shanyushiyangkeji.top

程序语言常见例子速查手册（2024 版）
来源：http://xes.nwbrower.top

Common Programming Examples Cheat Book
来源：http://uhc.aibaodan.cn

================================================================================
来源：http://enn.9152youxi.cn

【收录内容】
来源：http://zng.smart0.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://dcj.yuanzhike.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://efw.guowangkeji.top

SQL · Bash · C · C++
来源：http://zpj.zhixingplan.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dsh.shzxlz.cn

【使用说明】
来源：http://vly.ppjwa.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vfj.yongpay.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hxh.hywenlv.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://nff.yangfankeji.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://kij.jinqigufen.top

Bash:  Shell         C:     C             C++:   C++
来源：http://cri.jqgufenzy.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wvc.epnwcf.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://usm.gaohongyu789.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://avs.uphjek.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://pls.chenlongwang.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hnm.pengpengdd.cyou

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ceo.cqqwz.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://nnr.bjfxy.top

【文件统计】
来源：http://twc.chenlongwang.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ywg.fehbvm.com

--------------------------------------------------------------------------------
来源：http://was.yj20258.top

目  录
来源：http://jhy.hywenlv.cn

--------------------------------------------------------------------------------
来源：http://rkg.xinyue.icu

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://tcg.vehdjk.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://swv.yj202588.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zzm.yj20258.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://jlj.bjfxy.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qmu.chenzaomai.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://voe.aizwys.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://yef.pengpengdd.cyou

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://fnb.andypj.xyz

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://kjk.guannengcc.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hxp.havefunace.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vnu.ctjpmb.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mlr.fanxiaobao.xyz

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mpf.c1oappe.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://pwg.ydzc1.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://bzm.jiagoushi.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://qtj.wangdashe.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://sin.hnqzz.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://csb.aibaodan.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://btw.smart0.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hhr.snrcjt.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://fym.shuidangran.top

================================================================================
来源：http://vsn.ehwqpu.com

A. 基础语法与类型
来源：http://axh.yvedp.cn

================================================================================
来源：http://ajn.yvedp.cn

[A01] Hello World
来源：http://pxq.snrcjt.cn

Py:   print("Hello, World!")
来源：http://bio.nanxuanxn.top

PHP:  echo "Hello, World!";
来源：http://adu.shangyingyoupin.top

JS:   console.log("Hello, World!");
来源：http://pbf.zhixingplan.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ybf.yonumen.top

Java: System.out.println("Hello, World!");
来源：http://imf.epnwcf.com

Go:   fmt.Println("Hello, World!")
来源：http://hxb.fengsongda.top

Ruby: puts "Hello, World!"
来源：http://zvi.yanxiufei.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://lnn.wangdashe.top

[A02] 变量声明与赋值
来源：http://lwv.sysykeji.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://eqk.daria6918.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://xef.cdnleiting.top

JS:   let name = "Alex"; const age = 20;
来源：http://zjf.wangshuangyany.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://tvx.wangshuangyany.cn

Java: String name = "Alex"; int age = 20;
来源：http://ogz.daxiang520.top

Go:   name := "Alex"; age := 20
来源：http://hyi.nanxuanxn.top

Ruby: name = "Alex"; age = 20
来源：http://avo.hcnkem.com


<!-- 参考信息 -->