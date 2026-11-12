代发 wailian999

[U27] Py：异步 HTTP
来源：http://hcj.xinyue.icu

aiohttp.ClientSession() 配合 async with
来源：http://nzu.zhijiandao.cn

[U28] Py：类型别名
来源：http://mzp.dashuyun.cn

UserId = int
来源：http://umx.chenlongwang.top

[U29] Py：属性校验
来源：http://oga.meibo888.top

@property 与 @x.setter 配合
来源：http://dcj.sufxvd.cn

[U30] Py：数据类
来源：http://pxs.yanxiufei.cn

@dataclass(slots=True)
来源：http://dyn.chenzaomai.com

[U31] Py：单测
来源：http://con.sysykeji.top

python -m pytest -q
来源：http://zan.hcnkem.com

[U32] Py：代码格式化
来源：http://dcn.pycfn.com

ruff format . && ruff check --fix .
来源：http://zfv.hfpthk.cn

[U33] Py：打包发布
来源：http://mjb.jiagoushi.top

python -m build  （依赖 pyproject.toml）
来源：http://vrz.sjlbkw.cn

[U34] Py：判断编码
来源：http://gef.zdqjudy.top

chardet.detect(raw)
来源：http://ngg.zhiwuduotai.top

[U35] Py：发送邮件
来源：http://xbh.xuanzx.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://aey.ivvv.top

[U36] Py：定时任务
来源：http://gpd.gogol.net.cn

schedule.every(10).minutes.do(job)
来源：http://wiv.dianchejie.cn

[U37] Py：读写 Excel
来源：http://sim.ivvv.top

pandas.read_excel / DataFrame.to_excel
来源：http://qqj.jlsjyb.cn

[U38] Py：获取脚本所在目录
来源：http://tjg.hnxiangtu.top

Path(__file__).resolve().parent
来源：http://kjl.nanxuanxn.top

[U39] Py：判断是否在交互环境
来源：http://rdw.uphjek.com

sys.stdout.isatty()
来源：http://kdi.zhengqikj.top

[U40] Py：打印到标准错误
来源：http://ifm.tanke756.top

print("err", file=sys.stderr)
来源：http://vay.xuetiantiany.cn

[U41] PHP：初始化 Composer 项目
来源：http://cgu.sufxvd.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://iye.aibaodan.cn

[U42] PHP：PSR-4 自动加载
来源：http://lte.316326.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xtu.tianlin.xyz

[U43] PHP：声明命名空间
来源：http://isr.shzxlz.cn

namespace App\Http;
来源：http://uzv.hesvh.cn

[U44] PHP：开启严格类型
来源：http://opj.mhx1999.top

declare(strict_types=1);
来源：http://esq.guowangkeji.top

[U45] PHP：类型声明与返回类型
来源：http://oer.gzhubu.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://edf.shanyushiyangtech.top

[U46] PHP：可空类型
来源：http://thq.chenzaomai.com

?string $name = null
来源：http://pjt.tarul.cn

[U47] PHP：联合类型
来源：http://hyd.haohaochexian.top

int|string $id
来源：http://pjg.iojbl.cn

[U48] PHP：纯枚举
来源：http://iql.fktsv.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ptr.tarul.cn

[U49] PHP：只读属性
来源：http://dav.jianghu66.top

public readonly string $name
来源：http://rvc.andypj.xyz

[U50] PHP：构造器属性提升
来源：http://nmu.yj20258.top

public function __construct(private int $id) {}
来源：http://jyu.yfazqb.com

[U51] PHP：数组解构
来源：http://qak.9152youxi.cn

[$a, $b] = $arr;
来源：http://qzx.haohaochexian.top

[U52] PHP：箭头函数
来源：http://jzr.nanxinkj.top

$double = fn($x) => $x * 2;
来源：http://vze.xuanzx.com

[U53] PHP：空合并运算符
来源：http://ioc.aibaodan.cn

$v = $a ?? $b ?? "default";
来源：http://qgy.feifeiyinyue.top

[U54] PHP：空安全调用
来源：http://prs.zhixingplan.top

$obj?->method()
来源：http://qmh.andypj.xyz

[U55] PHP：match 表达式
来源：http://ydg.snrcjt.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://cmz.cucudq.cn

[U56] PHP：命名参数
来源：http://ofe.jinqigufen.top

f(a: 1, b: 2)
来源：http://mah.cqqwz.cn

[U57] PHP：字符串插值
来源：http://gsv.xuetiantiany.cn

"值: {$a}"
来源：http://yqf.iojbl.cn

[U58] PHP：数组三件套
来源：http://tjy.ehwqpu.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://smd.zdqjudy.top

[U59] PHP：自定义排序
来源：http://wea.shzxlz.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mda.zhiwuduotai.top

[U60] PHP：JSON 编解码
来源：http://ofi.yj20258.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ifw.xuanzx.com

[U61] PHP：正则
来源：http://shm.hnxiangtu.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qlt.ppjwa.cn

[U62] PHP：日期对象
来源：http://qzz.shuidangran.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vaz.hfpthk.cn

[U63] PHP：文件读写
来源：http://tyi.ppjwa.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zmg.nwbrower.top

[U64] PHP：目录遍历
来源：http://ign.aizwys.cn

glob("dir/*.php");  scandir("dir");
来源：http://clr.pycfn.com

[U65] PHP：会话
来源：http://jjl.ctjpmb.com

session_start();  $_SESSION["uid"] = 1;
来源：http://szl.hfpthk.cn

[U66] PHP：设置 Cookie
来源：http://mkx.sweek.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vne.hfpthk.cn

[U67] PHP：处理文件上传
来源：http://qsc.pycfn.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wqe.zhoulong.xyz

[U68] PHP：PDO 连接
来源：http://bwm.jqgufenzy.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xlt.kuanghao11.cn

[U69] PHP：PDO 预处理
来源：http://yrv.zhiwuduotai.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gqe.quarkkingdee.top

[U70] PHP：PDO 事务
来源：http://kqo.smart0.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dvz.hywenlv.cn

[U71] PHP：抛出异常
来源：http://wlq.nwbrower.top

throw new RuntimeException("失败", 500);
来源：http://pik.xuanzx.com

[U72] PHP：写错误日志
来源：http://mcu.cucudq.cn

error_log("失败: " . $e->getMessage());
来源：http://avf.xziqi.cn

[U73] PHP：读取 ini 配置
来源：http://fcu.jyoumei.cn

parse_ini_file("config.ini", true)
来源：http://jdo.redwolf501.top

[U74] PHP：读取环境变量
来源：http://enu.aizwys.cn

getenv("APP_ENV") ?: "production"
来源：http://vyg.xziqi.cn

[U75] PHP：依赖注入
来源：http://mip.ctjpmb.com

composer require psr/container
来源：http://gwk.svipenyu.cn

[U76] PHP：简单路由
来源：http://zos.hfpthk.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kkh.yueranfly.top

[U77] PHP：模板渲染
来源：http://nzx.quarkkingdee.top

composer require twig/twig
来源：http://qff.ehwqpu.com

[U78] PHP：单元测试
来源：http://bzl.jiagoushi.top

composer require --dev phpunit/phpunit
来源：http://wpv.guowangkeji.top

[U79] PHP：静态分析
来源：http://slp.sysykeji.top

composer require --dev phpstan/phpstan
来源：http://jks.yueranfly.top

[U80] PHP：代码规范修复
来源：http://cjs.wangshuangyany.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://vxx.ybcxt.top

[U81] JS：初始化项目
来源：http://zkq.yanxiufei.cn

npm init -y;  npm i express
来源：http://ttp.shuidangran.top

[U82] JS：package.json 脚本
来源：http://cta.jiagoushi.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://est.hcnkem.com

[U83] JS：ES Module 导入导出
来源：http://ijq.gaohongyu789.top

export const a = 1;  import { a } from "./m.js";
来源：http://blj.nanxuanxn.top

[U84] JS：CommonJS 写法
来源：http://jcy.iojbl.cn

module.exports = { a };  const { a } = require("./m");
来源：http://sgu.yuxming.cn

[U85] JS：可选链
来源：http://thi.jinyuanbaomall.cn

a?.b?.c
来源：http://gmq.shzxlz.cn

[U86] JS：空值合并
来源：http://ffz.andypj.xyz

a ?? b
来源：http://bao.yanxiufei.cn

[U87] JS：解构默认值
来源：http://cob.fengsongda.top

const { a = 1, b = 2 } = obj;
来源：http://kko.ywan-chungtsiang.top

[U88] JS：对象展开合并
来源：http://fsz.gzhubu.top

{ ...a, ...b }
来源：http://zeg.birdmap.top

[U89] JS：数组去重
来源：http://apb.jinyuanbaomall.cn

[...new Set(arr)]
来源：http://noa.birdmap.top

[U90] JS：数字数组排序
来源：http://ixe.fktsv.cn

[...arr].sort((a, b) => a - b)
来源：http://ydg.fanxiaobao.xyz

[U91] JS：对象键值遍历
来源：http://zjy.fktsv.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xsu.guowangkeji.top

[U92] JS：深拷贝
来源：http://rds.xuetiantiany.cn

structuredClone(obj)
来源：http://ula.havefunace.top

[U93] JS：模板字符串
来源：http://bsx.hcnkem.com

`共 ${n} 条`
来源：http://lry.gaohongyu789.top

[U94] JS：箭头函数
来源：http://rkg.kuanghao11.cn

const double = x => x * 2;
来源：http://dpg.birdmap.top

[U95] JS：Promise 包装
来源：http://cgc.fzhhl.top

new Promise((resolve, reject) => {})
来源：http://kkq.daxiang520.top

[U96] JS：async/await 与异常
来源：http://hvb.gzhubu.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://oft.hfpthk.cn

[U97] JS：并发请求
来源：http://pzm.birdmap.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://yds.vehdjk.com

[U98] JS：fetch 带 JSON
来源：http://cms.chenjidiqi.icu

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hdi.ydzc1.top

[U99] JS：事件监听
来源：http://gxk.tanke756.top

el.addEventListener("click", e => {})
来源：http://nks.gotoacloud.top

[U100] JS：DOM 查询
来源：http://dma.yonumen.top

document.querySelector(".item")
来源：http://wti.nanxuanxn.top

[U101] JS：classList 操作
来源：http://mtu.gogol.net.cn

el.classList.toggle("active")
来源：http://whw.xinyue.icu

[U102] JS：本地存储
来源：http://qum.tian-w.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://zvt.shzxlz.cn

[U103] JS：定时器
来源：http://jey.tianlin.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lhr.jyoumei.cn

[U104] JS：防抖
来源：http://xsb.yongpay.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hdp.guannengcc.top

[U105] JS：节流
来源：http://fqn.sjlbkw.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rgg.cucudq.cn

[U106] JS：日期格式化
来源：http://lwt.yj202588.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ynm.feifeiyinyue.top

[U107] JS：数字千分位
来源：http://vrx.vehdjk.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cbd.zhiwuduotai.top

[U108] JS：随机整数
来源：http://wuk.aibaodan.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wfw.wangshuangyany.cn

[U109] JS：数组分组
来源：http://hkr.chenlongwang.top

Object.groupBy(arr, x => x.type)
来源：http://tea.zhoulong.xyz

[U110] JS：数组分块
来源：http://xoe.gotoacloud.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qkh.shuidangran.top

[U111] JS：对象转 Map
来源：http://msy.jqgfzy.top

new Map(Object.entries(obj))
来源：http://ldg.feifeiyinyue.top

[U112] JS：字符串补位
来源：http://net.jinyuanbaomall.cn

"7".padStart(3, "0")
来源：http://dvv.shanyushiyangkeji.top

[U113] JS：正则替换全部
来源：http://xae.mhx1999.top

s.replaceAll("a", "b")
来源：http://mwd.yonumen.top

[U114] JS：JSON 深比较
来源：http://myr.epnwcf.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://eyq.zdbjq.cn

[U115] JS：生成 UUID
来源：http://lcj.cqqwz.cn

crypto.randomUUID()
来源：http://xni.hywenlv.cn

[U116] JS：类型检查（JSDoc）
来源：http://xnd.zhixingplan.top

/** @param {string} name */ function f(name) {}
来源：http://ymm.xylfe.cn

[U117] JS：单元测试
来源：http://kfi.jinqigfzy.top

npm i -D vitest;  npx vitest
来源：http://bcg.zycfv.cn

[U118] JS：开发服务器
来源：http://iny.jinqigfzy.top

npm i -D vite;  npx vite
来源：http://ewf.zhoulong.xyz

[U119] JS：生产构建
来源：http://owd.fanxiaobao.xyz

npx vite build
来源：http://qid.yongpay.top

[U120] JS：读取环境变量（Vite）
来源：http://plh.shanyushiyangkeji.top

import.meta.env.VITE_API_URL
来源：http://ruv.jinqigufen.top

================================================================================
来源：http://frr.shangyingyoupin.top

统计汇总
来源：http://sgo.yj202588.top

================================================================================
来源：http://dxn.yongpay.top

按语言统计（条）：
来源：http://mvr.yuanzhike.top

Python ......... 252
来源：http://ylu.tanke756.top

PHP ............ 252
来源：http://ygl.xuetiantiany.cn

JavaScript ..... 252
来源：http://pcd.yvedp.cn

TypeScript ..... 212
来源：http://vsc.yuxming.cn

Java ........... 212
来源：http://yov.meibo888.top

Go ............. 212
来源：http://cfb.vehdjk.com

Ruby ........... 212
来源：http://yvd.daxiang520.top

C# ............. 212
来源：http://dht.nanxinkj.top

C .............. 30
来源：http://izn.redwolf501.top

C++ ............ 30
来源：http://nfh.pycfn.com

SQL ............ 90
来源：http://cxw.zhiwuduotai.top

Bash ........... 80
来源：http://vvv.meibo888.top

Kotlin ......... 15
来源：http://aiw.yuxming.cn

Swift .......... 15
来源：http://wls.shanyushiyangkeji.top

Lua ............ 10
来源：http://gdn.hongshengwenyu.top

Perl ........... 10
来源：http://qlf.yuanzhike.top

Scala .......... 10
来源：http://nkj.havefunace.top

------------------------------------
来源：http://bui.hcnkem.com

合计 ........... 2106 条
来源：http://syj.sjlbkw.cn

按章节统计：
来源：http://syu.jiagoushi.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://uma.zhengqikj.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://oao.wangshuangyany.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://eby.zycfv.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ivc.chenjidiqi.icu

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://eyu.ydjk.org.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://sgc.jqgfzy.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://cou.cashguo.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nsq.dianchejie.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://osy.hammf.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vem.vqdsnc.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ozs.cdnleiting.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nar.jinyuanbaomall.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://lia.aibaodan.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://dhj.kuanghao11.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ydp.tianlin.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wva.vqdsnc.cn

Q SQL 专题                              90
来源：http://enl.tian-w.cn

R Bash 专题                             80
来源：http://jne.mhx1999.top

S C / C++ 专题                          60
来源：http://qbj.yanxiufei.cn

T 其他语言补充                          60
来源：http://jxo.ctjpmb.com

U 高频实用片段                         120
来源：http://vyi.ywan-chungtsiang.top

------------------------------------
来源：http://ynh.cheryme.top

合计                                  2106 条
来源：http://vgz.jianghu66.top

--------------------------------------------------------------------------------
来源：http://psn.316326.xyz

使用提醒
来源：http://elt.shuidangran.top

--------------------------------------------------------------------------------
来源：http://txa.cucudq.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xgd.0kj1m.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ycq.wangdashe.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://kgl.sufxvd.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://epi.zdbjq.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rby.zhaomingkeji.xyz

—— 文件结束 ——
来源：http://qmu.9152youxi.cn

================================================================================
来源：http://gzm.zhixingplan.top

程序语言常见例子速查手册（2024 版）
来源：http://xsp.tian-w.cn

Common Programming Examples Cheat Book
来源：http://vyh.hnqzz.top

================================================================================
来源：http://tjm.dianchejie.cn

【收录内容】
来源：http://kuy.hywenlv.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://zdo.jinyuanbaomall.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jmn.kuanghao11.cn

SQL · Bash · C · C++
来源：http://idz.fzhhl.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hqh.jqgufenzy.top

【使用说明】
来源：http://dda.xuanzx.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mub.yanxiufei.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://tvt.ehwqpu.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://vdb.ywan-chungtsiang.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vcx.iojbl.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://sps.cdnleiting.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://cif.hfpthk.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mdm.smart0.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hkj.haohaochexian.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://gys.hnqzz.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://kgw.gzhubu.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mie.andypj.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://exd.hesvh.cn

【文件统计】
来源：http://bfj.hysaishi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ttq.guannengcc.top

--------------------------------------------------------------------------------
来源：http://hld.fktsv.cn

目  录
来源：http://oml.dianchejie.cn

--------------------------------------------------------------------------------
来源：http://wqe.jinyuanbaomall.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zdg.fengsongda.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://jtg.tianlin.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://yjo.jqgfzy.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wur.wangshuangyany.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://kwm.316326.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fwc.feifeiyinyue.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://yne.ydzc1.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zis.zhijiandao.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qfk.ydjk.org.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mhx.ywan-chungtsiang.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ocx.ydzc1.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://gat.xziqi.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wcl.sxryk.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rny.sufxvd.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://uop.ywan-chungtsiang.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://xvz.zycfv.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vhd.zdqjudy.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://ohy.epnwcf.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mag.jianghu66.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://cdy.ydjk.org.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://dst.cheryme.top

================================================================================
来源：http://oib.ehwqpu.com

A. 基础语法与类型
来源：http://zrm.zdbjq.cn

================================================================================
来源：http://ptz.xuetiantiany.cn

[A01] Hello World
来源：http://qfp.shanyushiyangtech.top

Py:   print("Hello, World!")
来源：http://rfs.dashuyun.cn

PHP:  echo "Hello, World!";
来源：http://mfk.wangshuangyany.cn

JS:   console.log("Hello, World!");
来源：http://nfu.sweek.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ahf.hnqzz.top


<!-- 参考信息 -->