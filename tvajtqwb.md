代发 wailian999

[U23] Py：分块读取大文件
来源：http://vfp.andypj.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qhv.yangfankeji.com

[U24] Py：路径操作
来源：http://rrg.zhengqikj.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wvg.yuxming.cn

[U25] Py：CSV 按字典读
来源：http://oar.bbcook.cn

csv.DictReader(f)
来源：http://kyd.jinqigufen.top

[U26] Py：并发下载
来源：http://rdn.yvedp.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://alb.snrcjt.cn

[U27] Py：异步 HTTP
来源：http://rtg.sweek.top

aiohttp.ClientSession() 配合 async with
来源：http://gex.dianchejie.cn

[U28] Py：类型别名
来源：http://bor.jyoumei.cn

UserId = int
来源：http://ikl.zhongyouzk.top

[U29] Py：属性校验
来源：http://ccd.quarkkingdee.top

@property 与 @x.setter 配合
来源：http://ftt.jlsjyb.cn

[U30] Py：数据类
来源：http://dct.yfazqb.com

@dataclass(slots=True)
来源：http://bvb.tanke756.top

[U31] Py：单测
来源：http://nxv.xziqi.cn

python -m pytest -q
来源：http://toc.snrcjt.cn

[U32] Py：代码格式化
来源：http://mhn.aizwys.cn

ruff format . && ruff check --fix .
来源：http://xmd.ydjk.org.cn

[U33] Py：打包发布
来源：http://olt.sweek.top

python -m build  （依赖 pyproject.toml）
来源：http://fqm.daxiang520.top

[U34] Py：判断编码
来源：http://qow.fehbvm.com

chardet.detect(raw)
来源：http://umz.fktsv.cn

[U35] Py：发送邮件
来源：http://rew.cucudq.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bin.fanxiaobao.xyz

[U36] Py：定时任务
来源：http://cfs.aibaodan.cn

schedule.every(10).minutes.do(job)
来源：http://sow.havefunace.top

[U37] Py：读写 Excel
来源：http://uqb.yvedp.cn

pandas.read_excel / DataFrame.to_excel
来源：http://wzu.tian-w.cn

[U38] Py：获取脚本所在目录
来源：http://etz.dashuyun.cn

Path(__file__).resolve().parent
来源：http://ngb.zhoulong.xyz

[U39] Py：判断是否在交互环境
来源：http://gcr.guannengcc.top

sys.stdout.isatty()
来源：http://guz.ywan-chungtsiang.top

[U40] Py：打印到标准错误
来源：http://pmt.fzhhl.top

print("err", file=sys.stderr)
来源：http://jxy.hcnkem.com

[U41] PHP：初始化 Composer 项目
来源：http://odb.bbcook.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://aip.yvedp.cn

[U42] PHP：PSR-4 自动加载
来源：http://har.kuanghao11.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wde.ywan-chungtsiang.top

[U43] PHP：声明命名空间
来源：http://ryw.hcnkem.com

namespace App\Http;
来源：http://nqi.daria6918.cn

[U44] PHP：开启严格类型
来源：http://ogy.jinghuilouyu.cn

declare(strict_types=1);
来源：http://yji.chenlongwang.top

[U45] PHP：类型声明与返回类型
来源：http://iwu.yangfankeji.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://kvl.xingfuxueyuan.xyz

[U46] PHP：可空类型
来源：http://tqu.hfpthk.cn

?string $name = null
来源：http://lpf.fktsv.cn

[U47] PHP：联合类型
来源：http://cve.jianghu66.top

int|string $id
来源：http://abk.yangfankeji.com

[U48] PHP：纯枚举
来源：http://ykc.daria6918.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cnv.cdnleiting.top

[U49] PHP：只读属性
来源：http://jno.sjlbkw.cn

public readonly string $name
来源：http://ewp.xziqi.cn

[U50] PHP：构造器属性提升
来源：http://tgr.sweek.top

public function __construct(private int $id) {}
来源：http://qgh.xinyue.icu

[U51] PHP：数组解构
来源：http://vxj.xuetiantiany.cn

[$a, $b] = $arr;
来源：http://isf.shuidangran.top

[U52] PHP：箭头函数
来源：http://vha.yuxming.cn

$double = fn($x) => $x * 2;
来源：http://uux.svipenyu.cn

[U53] PHP：空合并运算符
来源：http://zmd.ydzc1.top

$v = $a ?? $b ?? "default";
来源：http://gir.birdmap.top

[U54] PHP：空安全调用
来源：http://zdw.cucudq.cn

$obj?->method()
来源：http://xcd.bbcook.cn

[U55] PHP：match 表达式
来源：http://pls.xuetiantiany.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rkn.yfazqb.com

[U56] PHP：命名参数
来源：http://tmd.hcnkem.com

f(a: 1, b: 2)
来源：http://vbz.hammf.cn

[U57] PHP：字符串插值
来源：http://cym.hammf.cn

"值: {$a}"
来源：http://ccv.yj202588.top

[U58] PHP：数组三件套
来源：http://jjj.tian-w.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rtu.gaohongyu789.top

[U59] PHP：自定义排序
来源：http://txy.chenlongwang.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tcl.ywan-chungtsiang.top

[U60] PHP：JSON 编解码
来源：http://buj.guannengcc.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dsn.iojbl.cn

[U61] PHP：正则
来源：http://udz.nanxuanxn.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://szl.hnxiangtu.top

[U62] PHP：日期对象
来源：http://kcl.ctjpmb.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gsm.bbcook.cn

[U63] PHP：文件读写
来源：http://nyz.yuxming.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tug.316326.xyz

[U64] PHP：目录遍历
来源：http://igq.cdnleiting.top

glob("dir/*.php");  scandir("dir");
来源：http://veu.yj202588.top

[U65] PHP：会话
来源：http://vdo.andypj.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://zwe.jqgfzy.top

[U66] PHP：设置 Cookie
来源：http://brc.zhixingplan.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kri.ppjwa.cn

[U67] PHP：处理文件上传
来源：http://opj.sufxvd.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lsw.gzhubu.top

[U68] PHP：PDO 连接
来源：http://uov.cucudq.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kji.yanxiufei.cn

[U69] PHP：PDO 预处理
来源：http://vqb.wangdashe.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dre.tianlin.xyz

[U70] PHP：PDO 事务
来源：http://aft.uphjek.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zwj.sxryk.cn

[U71] PHP：抛出异常
来源：http://yat.hysaishi.cn

throw new RuntimeException("失败", 500);
来源：http://doc.nwbrower.top

[U72] PHP：写错误日志
来源：http://pdf.jlsjyb.cn

error_log("失败: " . $e->getMessage());
来源：http://owt.havefunace.top

[U73] PHP：读取 ini 配置
来源：http://dpn.fktsv.cn

parse_ini_file("config.ini", true)
来源：http://fha.zhiwuduotai.top

[U74] PHP：读取环境变量
来源：http://tqo.gotoacloud.top

getenv("APP_ENV") ?: "production"
来源：http://avi.nanxuanxn.top

[U75] PHP：依赖注入
来源：http://ojl.shuidangran.top

composer require psr/container
来源：http://hws.ivvv.top

[U76] PHP：简单路由
来源：http://klu.yongpay.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vdy.mhx1999.top

[U77] PHP：模板渲染
来源：http://gyf.andypj.xyz

composer require twig/twig
来源：http://gmd.snrcjt.cn

[U78] PHP：单元测试
来源：http://tlu.xuanzx.com

composer require --dev phpunit/phpunit
来源：http://myb.daxiang520.top

[U79] PHP：静态分析
来源：http://cai.haohaochexian.top

composer require --dev phpstan/phpstan
来源：http://oyc.mhx1999.top

[U80] PHP：代码规范修复
来源：http://xhi.cdnleiting.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://rik.smart0.xyz

[U81] JS：初始化项目
来源：http://lta.ywan-chungtsiang.top

npm init -y;  npm i express
来源：http://hdi.hesvh.cn

[U82] JS：package.json 脚本
来源：http://jvb.nanxuanxn.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://exx.pengpengdd.cyou

[U83] JS：ES Module 导入导出
来源：http://jgg.nanxuanxn.top

export const a = 1;  import { a } from "./m.js";
来源：http://lee.ctjpmb.com

[U84] JS：CommonJS 写法
来源：http://myf.mhx1999.top

module.exports = { a };  const { a } = require("./m");
来源：http://yzh.wangdashe.top

[U85] JS：可选链
来源：http://klk.zdbjq.cn

a?.b?.c
来源：http://ovl.xingfuxueyuan.xyz

[U86] JS：空值合并
来源：http://djl.fehbvm.com

a ?? b
来源：http://avl.ppjwa.cn

[U87] JS：解构默认值
来源：http://zyv.chenlongwang.top

const { a = 1, b = 2 } = obj;
来源：http://iod.yj20258888.top

[U88] JS：对象展开合并
来源：http://ibq.tian-w.cn

{ ...a, ...b }
来源：http://enw.yangfankeji.com

[U89] JS：数组去重
来源：http://vxw.shzxlz.cn

[...new Set(arr)]
来源：http://fyi.quarkkingdee.top

[U90] JS：数字数组排序
来源：http://zkx.daxiang520.top

[...arr].sort((a, b) => a - b)
来源：http://krd.hnxiangtu.top

[U91] JS：对象键值遍历
来源：http://jtk.ivvv.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rfj.iojbl.cn

[U92] JS：深拷贝
来源：http://qve.sysykeji.top

structuredClone(obj)
来源：http://dkd.iojbl.cn

[U93] JS：模板字符串
来源：http://tin.pengpengdd.cyou

`共 ${n} 条`
来源：http://ugs.jiagoushi.top

[U94] JS：箭头函数
来源：http://osv.fengsongda.top

const double = x => x * 2;
来源：http://zxn.haohaochexian.top

[U95] JS：Promise 包装
来源：http://vpq.smart0.xyz

new Promise((resolve, reject) => {})
来源：http://kxl.uphjek.com

[U96] JS：async/await 与异常
来源：http://hds.gotoacloud.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hqs.shuidangran.top

[U97] JS：并发请求
来源：http://cyp.vqdsnc.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://vse.epnwcf.com

[U98] JS：fetch 带 JSON
来源：http://dxa.jinyuanbaomall.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://avr.ctjpmb.com

[U99] JS：事件监听
来源：http://stj.guowangkeji.top

el.addEventListener("click", e => {})
来源：http://hzw.0kj1m.cn

[U100] JS：DOM 查询
来源：http://qjh.smart0.xyz

document.querySelector(".item")
来源：http://eoe.haohaochexian.top

[U101] JS：classList 操作
来源：http://ttj.hnqzz.top

el.classList.toggle("active")
来源：http://hrt.zdqjudy.top

[U102] JS：本地存储
来源：http://rcg.zhixingplan.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://vaz.sweek.top

[U103] JS：定时器
来源：http://oxy.yanxiufei.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gis.xingfuxueyuan.xyz

[U104] JS：防抖
来源：http://soj.sjlbkw.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://onm.daria6918.cn

[U105] JS：节流
来源：http://gtp.yvedp.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hen.zhiwuduotai.top

[U106] JS：日期格式化
来源：http://rth.hywenlv.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pyj.jqgufenzy.top

[U107] JS：数字千分位
来源：http://oiw.xziqi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://oma.jinqigfzy.top

[U108] JS：随机整数
来源：http://rvi.yongpay.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://uqo.c1oappe.top

[U109] JS：数组分组
来源：http://eos.c1oappe.top

Object.groupBy(arr, x => x.type)
来源：http://yza.vqdsnc.cn

[U110] JS：数组分块
来源：http://kci.yanxiufei.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xlt.fehbvm.com

[U111] JS：对象转 Map
来源：http://kpj.dashuyun.cn

new Map(Object.entries(obj))
来源：http://ljo.tianlin.xyz

[U112] JS：字符串补位
来源：http://lrb.daria6918.cn

"7".padStart(3, "0")
来源：http://sgm.gaohongyu789.top

[U113] JS：正则替换全部
来源：http://rez.shuidangran.top

s.replaceAll("a", "b")
来源：http://mga.feifeiyinyue.top

[U114] JS：JSON 深比较
来源：http://qfl.chenlongwang.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://pym.uphjek.com

[U115] JS：生成 UUID
来源：http://ger.jqgfzy.top

crypto.randomUUID()
来源：http://zwq.bjfxy.top

[U116] JS：类型检查（JSDoc）
来源：http://urh.guannengcc.top

/** @param {string} name */ function f(name) {}
来源：http://tjl.cucudq.cn

[U117] JS：单元测试
来源：http://puw.yj20258.top

npm i -D vitest;  npx vitest
来源：http://rjh.zhiwuduotai.top

[U118] JS：开发服务器
来源：http://pku.bbcook.cn

npm i -D vite;  npx vite
来源：http://llp.hysaishi.cn

[U119] JS：生产构建
来源：http://zkm.hfpthk.cn

npx vite build
来源：http://hqq.yj20258.top

[U120] JS：读取环境变量（Vite）
来源：http://kzx.vqdsnc.cn

import.meta.env.VITE_API_URL
来源：http://ski.gotoacloud.top

================================================================================
来源：http://juz.nwbrower.top

统计汇总
来源：http://lvv.zhoulong.xyz

================================================================================
来源：http://eky.yueranfly.top

按语言统计（条）：
来源：http://ymc.jianghu66.top

Python ......... 252
来源：http://duz.zdqjudy.top

PHP ............ 252
来源：http://jik.sufxvd.cn

JavaScript ..... 252
来源：http://pjb.cheryme.top

TypeScript ..... 212
来源：http://vvg.quarkkingdee.top

Java ........... 212
来源：http://oyl.shangyingyoupin.top

Go ............. 212
来源：http://mzk.xinyue.icu

Ruby ........... 212
来源：http://dja.yj20258888.top

C# ............. 212
来源：http://fvy.shuidangran.top

C .............. 30
来源：http://rkp.yanxiufei.cn

C++ ............ 30
来源：http://qtv.birdmap.top

SQL ............ 90
来源：http://dsz.smart0.xyz

Bash ........... 80
来源：http://dvu.birdmap.top

Kotlin ......... 15
来源：http://ivl.yj20258.top

Swift .......... 15
来源：http://khx.zhengqikj.top

Lua ............ 10
来源：http://sdy.gzhubu.top

Perl ........... 10
来源：http://ehd.daria6918.cn

Scala .......... 10
来源：http://uly.zycfv.cn

------------------------------------
来源：http://owi.cucudq.cn

合计 ........... 2106 条
来源：http://jqk.hongshengwenyu.top

按章节统计：
来源：http://pru.pycfn.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://plx.haohaochexian.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://pso.hesvh.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wmr.sweek.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://txa.tanke756.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://yhm.guannengcc.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://knp.yj202588.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fli.sysykeji.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wpx.sjlbkw.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://pfp.haohaochexian.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vir.jiagoushi.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fmp.nwbrower.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://uym.xinyue.icu

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://tqu.jinqigufen.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ces.aibaodan.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://tpr.316326.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://puu.wangdashe.top

Q SQL 专题                              90
来源：http://ptw.sysykeji.top

R Bash 专题                             80
来源：http://okr.zhengqikj.top

S C / C++ 专题                          60
来源：http://eiu.hammf.cn

T 其他语言补充                          60
来源：http://upc.zycfv.cn

U 高频实用片段                         120
来源：http://gkp.hywenlv.cn

------------------------------------
来源：http://dgp.shangyingyoupin.top

合计                                  2106 条
来源：http://qfg.zhixingplan.top

--------------------------------------------------------------------------------
来源：http://iqt.cheryme.top

使用提醒
来源：http://jil.yonumen.top

--------------------------------------------------------------------------------
来源：http://skg.yj20258.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://bam.zhaomingkeji.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hso.chenjidiqi.icu

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mds.sysykeji.top

在旧版本上使用前请先确认语法支持情况。
来源：http://rlo.hfpthk.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xis.jinyuanbaomall.cn

—— 文件结束 ——
来源：http://pel.cheryme.top

================================================================================
来源：http://ovf.shanyushiyangtech.top

程序语言常见例子速查手册（2024 版）
来源：http://wfk.dianchejie.cn

Common Programming Examples Cheat Book
来源：http://tjp.zdqjudy.top

================================================================================
来源：http://zuc.ppjwa.cn

【收录内容】
来源：http://axe.aibaodan.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://fjf.birdmap.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://waw.jinqigfzy.top

SQL · Bash · C · C++
来源：http://xfe.hnqzz.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://sct.jinghuilouyu.cn

【使用说明】
来源：http://yqu.zhengqikj.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://xfn.ydzc1.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hnh.zhoulong.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://guy.fehbvm.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://yuj.fanxiaobao.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://vjz.ywan-chungtsiang.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://smp.yangfankeji.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://kgm.aizwys.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ygp.shanyushiyangkeji.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ylz.sweek.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://yzh.vqdsnc.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://iqg.fehbvm.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kfc.hfpthk.cn

【文件统计】
来源：http://bcj.316326.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rxn.zhengqikj.top

--------------------------------------------------------------------------------
来源：http://wtd.jqgufenzy.top

目  录
来源：http://fop.iojbl.cn

--------------------------------------------------------------------------------
来源：http://zgb.uphjek.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://vhh.jqgufenzy.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://fkn.jinqigufen.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vfh.iojbl.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://yhm.guannengcc.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://loo.hammf.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ati.jinqigfzy.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://jha.0kj1m.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wbn.shuidangran.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hxo.tarul.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://esq.vqdsnc.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://uic.sweek.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qzs.birdmap.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ftp.zhoulong.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://txp.ydzc1.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://saj.feifeiyinyue.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://vvm.birdmap.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pby.jlsjyb.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ruh.uphjek.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ccs.shanyushiyangtech.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qnr.yuanzhike.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://oto.cucudq.cn


<!-- 参考信息 -->