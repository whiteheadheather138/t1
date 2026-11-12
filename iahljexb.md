代发 wailian999

[U33] Py：打包发布
来源：http://uda.zdqjudy.top

python -m build  （依赖 pyproject.toml）
来源：http://kkx.chenzaomai.com

[U34] Py：判断编码
来源：http://ziy.jinyuanbaomall.cn

chardet.detect(raw)
来源：http://vec.sufxvd.cn

[U35] Py：发送邮件
来源：http://tws.fehbvm.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kqz.mhx1999.top

[U36] Py：定时任务
来源：http://gkj.jiagoushi.top

schedule.every(10).minutes.do(job)
来源：http://gtf.zhixingplan.top

[U37] Py：读写 Excel
来源：http://otl.yvedp.cn

pandas.read_excel / DataFrame.to_excel
来源：http://eiv.jyoumei.cn

[U38] Py：获取脚本所在目录
来源：http://udm.gzhubu.top

Path(__file__).resolve().parent
来源：http://gaa.tianlin.xyz

[U39] Py：判断是否在交互环境
来源：http://xkd.ydjk.org.cn

sys.stdout.isatty()
来源：http://ahz.fanxiaobao.xyz

[U40] Py：打印到标准错误
来源：http://rzc.316326.xyz

print("err", file=sys.stderr)
来源：http://kvw.cheryme.top

[U41] PHP：初始化 Composer 项目
来源：http://asw.pycfn.com

composer init;  composer require guzzlehttp/guzzle
来源：http://ojy.fzhhl.top

[U42] PHP：PSR-4 自动加载
来源：http://kbf.yj202588.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bva.wangshuangyany.cn

[U43] PHP：声明命名空间
来源：http://xce.ehwqpu.com

namespace App\Http;
来源：http://pqp.shuidangran.top

[U44] PHP：开启严格类型
来源：http://efq.fzhhl.top

declare(strict_types=1);
来源：http://yax.xinyue.icu

[U45] PHP：类型声明与返回类型
来源：http://ira.ivvv.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://gqo.yangfankeji.com

[U46] PHP：可空类型
来源：http://wqk.shuidangran.top

?string $name = null
来源：http://lkk.sxryk.cn

[U47] PHP：联合类型
来源：http://srf.sysykeji.top

int|string $id
来源：http://wmy.zhongyouzk.top

[U48] PHP：纯枚举
来源：http://nbz.jinqigufen.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://yra.ydzc1.top

[U49] PHP：只读属性
来源：http://bdl.zdbjq.cn

public readonly string $name
来源：http://pbu.jyoumei.cn

[U50] PHP：构造器属性提升
来源：http://xkl.zycfv.cn

public function __construct(private int $id) {}
来源：http://lvy.jinqigfzy.top

[U51] PHP：数组解构
来源：http://yoz.shanyushiyangtech.top

[$a, $b] = $arr;
来源：http://sux.ivvv.top

[U52] PHP：箭头函数
来源：http://bei.yvedp.cn

$double = fn($x) => $x * 2;
来源：http://qja.cucudq.cn

[U53] PHP：空合并运算符
来源：http://svx.ehwqpu.com

$v = $a ?? $b ?? "default";
来源：http://dhh.yongpay.top

[U54] PHP：空安全调用
来源：http://nje.hywenlv.cn

$obj?->method()
来源：http://vmb.shzxlz.cn

[U55] PHP：match 表达式
来源：http://fbe.sufxvd.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zlu.zhoulong.xyz

[U56] PHP：命名参数
来源：http://vrs.c1oappe.top

f(a: 1, b: 2)
来源：http://kto.vehdjk.com

[U57] PHP：字符串插值
来源：http://she.hnqzz.top

"值: {$a}"
来源：http://amb.yanxiufei.cn

[U58] PHP：数组三件套
来源：http://yah.yj20258888.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nnu.jyoumei.cn

[U59] PHP：自定义排序
来源：http://uma.yanxiufei.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aiv.quarkkingdee.top

[U60] PHP：JSON 编解码
来源：http://lcm.svipenyu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://akm.zhengqikj.top

[U61] PHP：正则
来源：http://bhx.yueranfly.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qws.svipenyu.cn

[U62] PHP：日期对象
来源：http://gvd.dianchejie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://htx.jlsjyb.cn

[U63] PHP：文件读写
来源：http://ujs.zycfv.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mco.ppjwa.cn

[U64] PHP：目录遍历
来源：http://bab.iojbl.cn

glob("dir/*.php");  scandir("dir");
来源：http://zhe.sysykeji.top

[U65] PHP：会话
来源：http://yjl.yuanzhike.top

session_start();  $_SESSION["uid"] = 1;
来源：http://oqv.yj20258.top

[U66] PHP：设置 Cookie
来源：http://lbc.sufxvd.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xya.jyoumei.cn

[U67] PHP：处理文件上传
来源：http://xqt.sxryk.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wri.aizwys.cn

[U68] PHP：PDO 连接
来源：http://iff.fehbvm.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gpy.chenlongwang.top

[U69] PHP：PDO 预处理
来源：http://gpd.52xcode.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://byg.ctjpmb.com

[U70] PHP：PDO 事务
来源：http://lua.zycfv.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pof.xuanzx.com

[U71] PHP：抛出异常
来源：http://feq.sxryk.cn

throw new RuntimeException("失败", 500);
来源：http://yim.ydzc1.top

[U72] PHP：写错误日志
来源：http://vyh.zhiwuduotai.top

error_log("失败: " . $e->getMessage());
来源：http://oll.ivvv.top

[U73] PHP：读取 ini 配置
来源：http://vvb.xinyue.icu

parse_ini_file("config.ini", true)
来源：http://ujr.feifeiyinyue.top

[U74] PHP：读取环境变量
来源：http://jhw.hfpthk.cn

getenv("APP_ENV") ?: "production"
来源：http://ido.c1oappe.top

[U75] PHP：依赖注入
来源：http://uwt.xylfe.cn

composer require psr/container
来源：http://szy.yfazqb.com

[U76] PHP：简单路由
来源：http://btg.tarul.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://oph.xingfuxueyuan.xyz

[U77] PHP：模板渲染
来源：http://vlr.jqgfzy.top

composer require twig/twig
来源：http://zup.fzhhl.top

[U78] PHP：单元测试
来源：http://kbg.sjlbkw.cn

composer require --dev phpunit/phpunit
来源：http://mxc.wangdashe.top

[U79] PHP：静态分析
来源：http://nqp.shanyushiyangtech.top

composer require --dev phpstan/phpstan
来源：http://yps.chenzaomai.com

[U80] PHP：代码规范修复
来源：http://hzl.shzxlz.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://pni.haohaochexian.top

[U81] JS：初始化项目
来源：http://oii.ydzc1.top

npm init -y;  npm i express
来源：http://bip.vehdjk.com

[U82] JS：package.json 脚本
来源：http://qxh.redwolf501.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lmn.nanxinkj.top

[U83] JS：ES Module 导入导出
来源：http://bqv.yuanzhike.top

export const a = 1;  import { a } from "./m.js";
来源：http://zcb.sufxvd.cn

[U84] JS：CommonJS 写法
来源：http://kse.nwbrower.top

module.exports = { a };  const { a } = require("./m");
来源：http://aqg.ehwqpu.com

[U85] JS：可选链
来源：http://cfn.jianghu66.top

a?.b?.c
来源：http://pqs.xuanzx.com

[U86] JS：空值合并
来源：http://pdw.nanxinkj.top

a ?? b
来源：http://yjp.yonumen.top

[U87] JS：解构默认值
来源：http://dsc.zdqjudy.top

const { a = 1, b = 2 } = obj;
来源：http://tnh.yuanzhike.top

[U88] JS：对象展开合并
来源：http://nym.pycfn.com

{ ...a, ...b }
来源：http://qej.zycfv.cn

[U89] JS：数组去重
来源：http://fdf.sxryk.cn

[...new Set(arr)]
来源：http://lbe.sjlbkw.cn

[U90] JS：数字数组排序
来源：http://rps.zdqjudy.top

[...arr].sort((a, b) => a - b)
来源：http://dlm.sweek.top

[U91] JS：对象键值遍历
来源：http://bev.shanyushiyangtech.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://usn.bjfxy.top

[U92] JS：深拷贝
来源：http://ikq.svipenyu.cn

structuredClone(obj)
来源：http://ogk.jinyuanbaomall.cn

[U93] JS：模板字符串
来源：http://wam.zdqjudy.top

`共 ${n} 条`
来源：http://unm.xinyue.icu

[U94] JS：箭头函数
来源：http://wbs.shanyushiyangtech.top

const double = x => x * 2;
来源：http://tlk.sweek.top

[U95] JS：Promise 包装
来源：http://exz.vqdsnc.cn

new Promise((resolve, reject) => {})
来源：http://jtf.chenlongwang.top

[U96] JS：async/await 与异常
来源：http://ykc.gaohongyu789.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bcj.tianlin.xyz

[U97] JS：并发请求
来源：http://hyz.tian-w.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://snl.fengsongda.top

[U98] JS：fetch 带 JSON
来源：http://sny.gogol.net.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xsk.vqdsnc.cn

[U99] JS：事件监听
来源：http://cxm.gzhubu.top

el.addEventListener("click", e => {})
来源：http://tsh.zhongyouzk.top

[U100] JS：DOM 查询
来源：http://mbz.zycfv.cn

document.querySelector(".item")
来源：http://ufc.sufxvd.cn

[U101] JS：classList 操作
来源：http://hjg.bjfxy.top

el.classList.toggle("active")
来源：http://yal.wangdashe.top

[U102] JS：本地存储
来源：http://rom.wangdashe.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://kmx.fzhhl.top

[U103] JS：定时器
来源：http://irv.chenlongwang.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mlx.yj20258.top

[U104] JS：防抖
来源：http://htz.uphjek.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fzr.ydjk.org.cn

[U105] JS：节流
来源：http://mic.xuanzx.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xke.chenjidiqi.icu

[U106] JS：日期格式化
来源：http://dci.ppjwa.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://uhe.yuanzhike.top

[U107] JS：数字千分位
来源：http://tye.meibo888.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zwp.chenjidiqi.icu

[U108] JS：随机整数
来源：http://blv.hnxiangtu.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tiw.hfpthk.cn

[U109] JS：数组分组
来源：http://fno.jqgufenzy.top

Object.groupBy(arr, x => x.type)
来源：http://naj.fzhhl.top

[U110] JS：数组分块
来源：http://tuw.fktsv.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://sfm.mhx1999.top

[U111] JS：对象转 Map
来源：http://ieb.andypj.xyz

new Map(Object.entries(obj))
来源：http://kbu.aizwys.cn

[U112] JS：字符串补位
来源：http://bdz.zhijiandao.cn

"7".padStart(3, "0")
来源：http://ryb.ehwqpu.com

[U113] JS：正则替换全部
来源：http://fky.aizwys.cn

s.replaceAll("a", "b")
来源：http://hvt.fanxiaobao.xyz

[U114] JS：JSON 深比较
来源：http://asj.yuanzhike.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://iue.pengpengdd.cyou

[U115] JS：生成 UUID
来源：http://eaw.epnwcf.com

crypto.randomUUID()
来源：http://ldw.feifeiyinyue.top

[U116] JS：类型检查（JSDoc）
来源：http://shr.guannengcc.top

/** @param {string} name */ function f(name) {}
来源：http://eks.guannengcc.top

[U117] JS：单元测试
来源：http://rqw.hysaishi.cn

npm i -D vitest;  npx vitest
来源：http://cnd.epnwcf.com

[U118] JS：开发服务器
来源：http://oxn.gzhubu.top

npm i -D vite;  npx vite
来源：http://gxv.havefunace.top

[U119] JS：生产构建
来源：http://dgi.zhongyouzk.top

npx vite build
来源：http://wkd.yj20258888.top

[U120] JS：读取环境变量（Vite）
来源：http://kwe.zycfv.cn

import.meta.env.VITE_API_URL
来源：http://npu.guannengcc.top

================================================================================
来源：http://xzd.wangshuangyany.cn

统计汇总
来源：http://thb.52xcode.cn

================================================================================
来源：http://foe.shuidangran.top

按语言统计（条）：
来源：http://csg.yvedp.cn

Python ......... 252
来源：http://zaj.shuidangran.top

PHP ............ 252
来源：http://slz.hfpthk.cn

JavaScript ..... 252
来源：http://uls.yonumen.top

TypeScript ..... 212
来源：http://wlp.shzxlz.cn

Java ........... 212
来源：http://wqd.jqgfzy.top

Go ............. 212
来源：http://uhq.zhijiandao.cn

Ruby ........... 212
来源：http://pse.fehbvm.com

C# ............. 212
来源：http://pwn.fanxiaobao.xyz

C .............. 30
来源：http://djr.dashuyun.cn

C++ ............ 30
来源：http://kga.xuanzx.com

SQL ............ 90
来源：http://qxk.aibaodan.cn

Bash ........... 80
来源：http://ixh.cdnleiting.top

Kotlin ......... 15
来源：http://xov.jiagoushi.top

Swift .......... 15
来源：http://uae.tianlin.xyz

Lua ............ 10
来源：http://ded.guannengcc.top

Perl ........... 10
来源：http://szy.sufxvd.cn

Scala .......... 10
来源：http://lxk.fzhhl.top

------------------------------------
来源：http://ldc.daria6918.cn

合计 ........... 2106 条
来源：http://bnb.fktsv.cn

按章节统计：
来源：http://cyo.shzxlz.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rrk.cdnleiting.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gpt.smart0.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pfs.chenjidiqi.icu

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fpi.tian-w.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://tar.52xcode.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zgo.svipenyu.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ota.chenzaomai.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://bgf.zhiwuduotai.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://etj.jianghu66.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dkj.zycfv.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xfl.meibo888.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wva.bbcook.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zew.hysaishi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jqj.yfazqb.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ckz.gzhubu.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://opq.zycfv.cn

Q SQL 专题                              90
来源：http://csl.yuxming.cn

R Bash 专题                             80
来源：http://qgu.jiagoushi.top

S C / C++ 专题                          60
来源：http://pfs.zhijiandao.cn

T 其他语言补充                          60
来源：http://ntx.zdbjq.cn

U 高频实用片段                         120
来源：http://fdj.yfazqb.com

------------------------------------
来源：http://onf.uphjek.com

合计                                  2106 条
来源：http://wgw.zycfv.cn

--------------------------------------------------------------------------------
来源：http://jhe.yj20258888.top

使用提醒
来源：http://qdt.xylfe.cn

--------------------------------------------------------------------------------
来源：http://iky.jqgfzy.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://pbq.dianchejie.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://cvf.cheryme.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ymb.birdmap.top

在旧版本上使用前请先确认语法支持情况。
来源：http://mqo.c1oappe.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://fyu.sufxvd.cn

—— 文件结束 ——
来源：http://cas.sjlbkw.cn

================================================================================
来源：http://yku.jlsjyb.cn

程序语言常见例子速查手册（2024 版）
来源：http://uaz.gotoacloud.top

Common Programming Examples Cheat Book
来源：http://veq.hammf.cn

================================================================================
来源：http://muv.chenjidiqi.icu

【收录内容】
来源：http://bce.xuetiantiany.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://xji.xylfe.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://yqp.daria6918.cn

SQL · Bash · C · C++
来源：http://xoh.smart0.xyz

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://fwm.fehbvm.com

【使用说明】
来源：http://wof.gzhubu.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://zvs.vehdjk.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xrw.hesvh.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://vsw.jinqigufen.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://bur.gotoacloud.top

Bash:  Shell         C:     C             C++:   C++
来源：http://lkw.hcnkem.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://uwi.havefunace.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://lpb.vqdsnc.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ele.hongshengwenyu.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mvy.hammf.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://brt.yuxming.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://eau.yfazqb.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://soi.nanxuanxn.top

【文件统计】
来源：http://yqf.zycfv.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://afa.fengsongda.top

--------------------------------------------------------------------------------
来源：http://imc.gzhubu.top

目  录
来源：http://ztz.vehdjk.com

--------------------------------------------------------------------------------
来源：http://oai.tanke756.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://vuf.dashuyun.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://bns.zdbjq.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://bwg.svipenyu.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://abn.cheryme.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://gxk.gotoacloud.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wvh.nwbrower.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://lny.yfazqb.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xms.nanxinkj.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tkp.mhx1999.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://roc.kuanghao11.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ulb.hcnkem.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://izl.gotoacloud.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://eiw.jianghu66.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://jhl.xziqi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ggb.zycfv.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ddc.cqqwz.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ipe.sjlbkw.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://bxp.gogol.net.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://bey.shuidangran.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fbk.fzhhl.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hkl.ydzc1.top

================================================================================
来源：http://qyl.daria6918.cn

A. 基础语法与类型
来源：http://mml.jinghuilouyu.cn

================================================================================
来源：http://aps.nanxinkj.top

[A01] Hello World
来源：http://gof.ivvv.top

Py:   print("Hello, World!")
来源：http://bci.yueranfly.top

PHP:  echo "Hello, World!";
来源：http://kko.snrcjt.cn

JS:   console.log("Hello, World!");
来源：http://cjf.jinqigufen.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://vhc.hnqzz.top

Java: System.out.println("Hello, World!");
来源：http://kea.mhx1999.top

Go:   fmt.Println("Hello, World!")
来源：http://lis.dashuyun.cn

Ruby: puts "Hello, World!"
来源：http://sgg.hesvh.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://rhh.sufxvd.cn

[A02] 变量声明与赋值
来源：http://pfv.fengsongda.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://dzt.hfpthk.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ars.jinqigfzy.top

JS:   let name = "Alex"; const age = 20;
来源：http://omz.pengpengdd.cyou

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://qbp.yongpay.top

Java: String name = "Alex"; int age = 20;
来源：http://fmh.vehdjk.com

Go:   name := "Alex"; age := 20
来源：http://rxp.shuidangran.top

Ruby: name = "Alex"; age = 20
来源：http://xvo.sufxvd.cn


<!-- 参考信息 -->