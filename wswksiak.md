代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://rpx.yj20258.top

@contextlib.contextmanager
来源：http://ycw.zycfv.cn

[U22] Py：矩阵转置
来源：http://pcj.zhengqikj.top

list(zip(*m))
来源：http://iop.fengsongda.top

[U23] Py：分块读取大文件
来源：http://gpr.wangdashe.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://het.cashguo.top

[U24] Py：路径操作
来源：http://hno.cdnleiting.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tmw.jqgufenzy.top

[U25] Py：CSV 按字典读
来源：http://uvw.nwbrower.top

csv.DictReader(f)
来源：http://nbv.jinyuanbaomall.cn

[U26] Py：并发下载
来源：http://eas.yj20258888.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pbz.jqgfzy.top

[U27] Py：异步 HTTP
来源：http://mew.aibaodan.cn

aiohttp.ClientSession() 配合 async with
来源：http://mnx.xuanzx.com

[U28] Py：类型别名
来源：http://vhy.hnxiangtu.top

UserId = int
来源：http://ijr.zdbjq.cn

[U29] Py：属性校验
来源：http://unc.hnxiangtu.top

@property 与 @x.setter 配合
来源：http://aib.0kj1m.cn

[U30] Py：数据类
来源：http://oai.xuetiantiany.cn

@dataclass(slots=True)
来源：http://yoy.hesvh.cn

[U31] Py：单测
来源：http://kpz.ydjk.org.cn

python -m pytest -q
来源：http://ers.cdnleiting.top

[U32] Py：代码格式化
来源：http://sot.jqgufenzy.top

ruff format . && ruff check --fix .
来源：http://kdj.sjlbkw.cn

[U33] Py：打包发布
来源：http://pny.zhongyouzk.top

python -m build  （依赖 pyproject.toml）
来源：http://cjo.shanyushiyangkeji.top

[U34] Py：判断编码
来源：http://abn.yj20258888.top

chardet.detect(raw)
来源：http://tdj.yuxming.cn

[U35] Py：发送邮件
来源：http://bog.jqgfzy.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://asm.cheryme.top

[U36] Py：定时任务
来源：http://krk.cdnleiting.top

schedule.every(10).minutes.do(job)
来源：http://zyo.haohaochexian.top

[U37] Py：读写 Excel
来源：http://roj.zhijiandao.cn

pandas.read_excel / DataFrame.to_excel
来源：http://phk.hywenlv.cn

[U38] Py：获取脚本所在目录
来源：http://tug.nwbrower.top

Path(__file__).resolve().parent
来源：http://dit.hnxiangtu.top

[U39] Py：判断是否在交互环境
来源：http://vuk.daxiang520.top

sys.stdout.isatty()
来源：http://cok.vehdjk.com

[U40] Py：打印到标准错误
来源：http://bec.yonumen.top

print("err", file=sys.stderr)
来源：http://lfj.uphjek.com

[U41] PHP：初始化 Composer 项目
来源：http://jqs.nanxinkj.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ius.iojbl.cn

[U42] PHP：PSR-4 自动加载
来源：http://fwt.gaohongyu789.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://foh.hcnkem.com

[U43] PHP：声明命名空间
来源：http://dwy.zdbjq.cn

namespace App\Http;
来源：http://jyt.ivvv.top

[U44] PHP：开启严格类型
来源：http://lfv.hnxiangtu.top

declare(strict_types=1);
来源：http://ghx.kuanghao11.cn

[U45] PHP：类型声明与返回类型
来源：http://sxm.yangfankeji.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://mui.pengpengdd.cyou

[U46] PHP：可空类型
来源：http://vel.jiagoushi.top

?string $name = null
来源：http://sxf.ydzc1.top

[U47] PHP：联合类型
来源：http://viv.fanxiaobao.xyz

int|string $id
来源：http://adj.vqdsnc.cn

[U48] PHP：纯枚举
来源：http://ick.tanke756.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kin.zdbjq.cn

[U49] PHP：只读属性
来源：http://knw.vqdsnc.cn

public readonly string $name
来源：http://fze.fanxiaobao.xyz

[U50] PHP：构造器属性提升
来源：http://mmk.aibaodan.cn

public function __construct(private int $id) {}
来源：http://dpc.guannengcc.top

[U51] PHP：数组解构
来源：http://myp.jqgufenzy.top

[$a, $b] = $arr;
来源：http://gha.cdnleiting.top

[U52] PHP：箭头函数
来源：http://azi.xingfuxueyuan.xyz

$double = fn($x) => $x * 2;
来源：http://zha.fehbvm.com

[U53] PHP：空合并运算符
来源：http://wnx.chenlongwang.top

$v = $a ?? $b ?? "default";
来源：http://jny.yanxiufei.cn

[U54] PHP：空安全调用
来源：http://gjw.xingfuxueyuan.xyz

$obj?->method()
来源：http://wps.chenlongwang.top

[U55] PHP：match 表达式
来源：http://hui.xziqi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ocq.zhongyouzk.top

[U56] PHP：命名参数
来源：http://xbe.guannengcc.top

f(a: 1, b: 2)
来源：http://kpa.daxiang520.top

[U57] PHP：字符串插值
来源：http://cjk.fehbvm.com

"值: {$a}"
来源：http://uqd.tian-w.cn

[U58] PHP：数组三件套
来源：http://hdq.birdmap.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gxa.fktsv.cn

[U59] PHP：自定义排序
来源：http://igf.sufxvd.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zvy.bbcook.cn

[U60] PHP：JSON 编解码
来源：http://yne.pycfn.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ltf.quarkkingdee.top

[U61] PHP：正则
来源：http://exc.iojbl.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://umo.aizwys.cn

[U62] PHP：日期对象
来源：http://vnt.sufxvd.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jps.dianchejie.cn

[U63] PHP：文件读写
来源：http://kzm.zdbjq.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://oyi.zhixingplan.top

[U64] PHP：目录遍历
来源：http://irg.zhengqikj.top

glob("dir/*.php");  scandir("dir");
来源：http://kze.zhiwuduotai.top

[U65] PHP：会话
来源：http://ots.zdbjq.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://fzv.zdqjudy.top

[U66] PHP：设置 Cookie
来源：http://nkv.yj202588.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vky.xziqi.cn

[U67] PHP：处理文件上传
来源：http://rsm.xuanzx.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kvd.zdqjudy.top

[U68] PHP：PDO 连接
来源：http://pkw.shanyushiyangkeji.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://yhm.uphjek.com

[U69] PHP：PDO 预处理
来源：http://vvz.gotoacloud.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://uac.shanyushiyangtech.top

[U70] PHP：PDO 事务
来源：http://ghs.shzxlz.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dhp.yuxming.cn

[U71] PHP：抛出异常
来源：http://ezu.yonumen.top

throw new RuntimeException("失败", 500);
来源：http://wfh.shangyingyoupin.top

[U72] PHP：写错误日志
来源：http://zpm.wangshuangyany.cn

error_log("失败: " . $e->getMessage());
来源：http://pno.fktsv.cn

[U73] PHP：读取 ini 配置
来源：http://rql.0kj1m.cn

parse_ini_file("config.ini", true)
来源：http://itj.pengpengdd.cyou

[U74] PHP：读取环境变量
来源：http://zzi.zhoulong.xyz

getenv("APP_ENV") ?: "production"
来源：http://lrf.zhiwuduotai.top

[U75] PHP：依赖注入
来源：http://nbz.sufxvd.cn

composer require psr/container
来源：http://npq.shanyushiyangkeji.top

[U76] PHP：简单路由
来源：http://pgf.ppjwa.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tii.jlsjyb.cn

[U77] PHP：模板渲染
来源：http://drx.cdnleiting.top

composer require twig/twig
来源：http://uvf.cucudq.cn

[U78] PHP：单元测试
来源：http://xcy.zhongyouzk.top

composer require --dev phpunit/phpunit
来源：http://szx.xziqi.cn

[U79] PHP：静态分析
来源：http://zse.fanxiaobao.xyz

composer require --dev phpstan/phpstan
来源：http://omd.sysykeji.top

[U80] PHP：代码规范修复
来源：http://peh.fzhhl.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://xyd.yj202588.top

[U81] JS：初始化项目
来源：http://egv.xylfe.cn

npm init -y;  npm i express
来源：http://yqj.shanyushiyangtech.top

[U82] JS：package.json 脚本
来源：http://ieb.cashguo.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lwt.zhaomingkeji.xyz

[U83] JS：ES Module 导入导出
来源：http://mdb.sysykeji.top

export const a = 1;  import { a } from "./m.js";
来源：http://vin.jinqigfzy.top

[U84] JS：CommonJS 写法
来源：http://pes.aizwys.cn

module.exports = { a };  const { a } = require("./m");
来源：http://hsn.yj20258888.top

[U85] JS：可选链
来源：http://gil.ydjk.org.cn

a?.b?.c
来源：http://sdc.tianlin.xyz

[U86] JS：空值合并
来源：http://ysh.xylfe.cn

a ?? b
来源：http://oot.vehdjk.com

[U87] JS：解构默认值
来源：http://ios.yj202588.top

const { a = 1, b = 2 } = obj;
来源：http://bek.cdnleiting.top

[U88] JS：对象展开合并
来源：http://puz.zdbjq.cn

{ ...a, ...b }
来源：http://eob.jinqigfzy.top

[U89] JS：数组去重
来源：http://nql.yvedp.cn

[...new Set(arr)]
来源：http://fff.smart0.xyz

[U90] JS：数字数组排序
来源：http://hba.meibo888.top

[...arr].sort((a, b) => a - b)
来源：http://wfl.shuidangran.top

[U91] JS：对象键值遍历
来源：http://qbo.bbcook.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tos.c1oappe.top

[U92] JS：深拷贝
来源：http://vql.cqqwz.cn

structuredClone(obj)
来源：http://dna.chenzaomai.com

[U93] JS：模板字符串
来源：http://zci.c1oappe.top

`共 ${n} 条`
来源：http://mbl.shanyushiyangkeji.top

[U94] JS：箭头函数
来源：http://tox.zhengqikj.top

const double = x => x * 2;
来源：http://dsl.mhx1999.top

[U95] JS：Promise 包装
来源：http://dzf.shanyushiyangtech.top

new Promise((resolve, reject) => {})
来源：http://qcl.iojbl.cn

[U96] JS：async/await 与异常
来源：http://zok.hesvh.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://tyc.shzxlz.cn

[U97] JS：并发请求
来源：http://zrd.iojbl.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://bwp.yj20258888.top

[U98] JS：fetch 带 JSON
来源：http://jhv.cucudq.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pot.kuanghao11.cn

[U99] JS：事件监听
来源：http://ogo.hnxiangtu.top

el.addEventListener("click", e => {})
来源：http://gia.zhijiandao.cn

[U100] JS：DOM 查询
来源：http://nfk.gotoacloud.top

document.querySelector(".item")
来源：http://hjk.aibaodan.cn

[U101] JS：classList 操作
来源：http://sjo.zhengqikj.top

el.classList.toggle("active")
来源：http://vhb.smart0.xyz

[U102] JS：本地存储
来源：http://div.sweek.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ebw.gzhubu.top

[U103] JS：定时器
来源：http://ijm.yanxiufei.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ylg.wangdashe.top

[U104] JS：防抖
来源：http://pqy.guowangkeji.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://emd.sysykeji.top

[U105] JS：节流
来源：http://ijy.wangdashe.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hli.meibo888.top

[U106] JS：日期格式化
来源：http://dbb.ehwqpu.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://msk.tian-w.cn

[U107] JS：数字千分位
来源：http://whs.tanke756.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mro.yuanzhike.top

[U108] JS：随机整数
来源：http://wnn.cheryme.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://psx.yfazqb.com

[U109] JS：数组分组
来源：http://pqt.ywan-chungtsiang.top

Object.groupBy(arr, x => x.type)
来源：http://sdy.snrcjt.cn

[U110] JS：数组分块
来源：http://kza.ybcxt.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://njt.hongshengwenyu.top

[U111] JS：对象转 Map
来源：http://pal.gaohongyu789.top

new Map(Object.entries(obj))
来源：http://zbt.0kj1m.cn

[U112] JS：字符串补位
来源：http://pfa.epnwcf.com

"7".padStart(3, "0")
来源：http://crk.aibaodan.cn

[U113] JS：正则替换全部
来源：http://emh.jinqigufen.top

s.replaceAll("a", "b")
来源：http://wcy.jinyuanbaomall.cn

[U114] JS：JSON 深比较
来源：http://nyl.hesvh.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://rfp.xylfe.cn

[U115] JS：生成 UUID
来源：http://gea.ybcxt.top

crypto.randomUUID()
来源：http://dsu.ivvv.top

[U116] JS：类型检查（JSDoc）
来源：http://qst.chenjidiqi.icu

/** @param {string} name */ function f(name) {}
来源：http://zag.vehdjk.com

[U117] JS：单元测试
来源：http://tbp.zhoulong.xyz

npm i -D vitest;  npx vitest
来源：http://qua.nanxinkj.top

[U118] JS：开发服务器
来源：http://lsn.epnwcf.com

npm i -D vite;  npx vite
来源：http://aei.yj20258888.top

[U119] JS：生产构建
来源：http://nhu.jqgfzy.top

npx vite build
来源：http://oms.cashguo.top

[U120] JS：读取环境变量（Vite）
来源：http://eiv.hongshengwenyu.top

import.meta.env.VITE_API_URL
来源：http://jdp.wangdashe.top

================================================================================
来源：http://rph.epnwcf.com

统计汇总
来源：http://mbb.zhaomingkeji.xyz

================================================================================
来源：http://mbh.yonumen.top

按语言统计（条）：
来源：http://sni.yj202588.top

Python ......... 252
来源：http://gza.vqdsnc.cn

PHP ............ 252
来源：http://lfi.bbcook.cn

JavaScript ..... 252
来源：http://eli.kuanghao11.cn

TypeScript ..... 212
来源：http://cbc.daxiang520.top

Java ........... 212
来源：http://ybt.yuxming.cn

Go ............. 212
来源：http://pto.haohaochexian.top

Ruby ........... 212
来源：http://xih.jyoumei.cn

C# ............. 212
来源：http://ypz.hnqzz.top

C .............. 30
来源：http://aaz.hongshengwenyu.top

C++ ............ 30
来源：http://ztc.xziqi.cn

SQL ............ 90
来源：http://cor.guowangkeji.top

Bash ........... 80
来源：http://vkd.gogol.net.cn

Kotlin ......... 15
来源：http://woy.hywenlv.cn

Swift .......... 15
来源：http://bay.aibaodan.cn

Lua ............ 10
来源：http://avc.jinqigufen.top

Perl ........... 10
来源：http://rnf.nanxuanxn.top

Scala .......... 10
来源：http://lsv.ydzc1.top

------------------------------------
来源：http://qsy.jinyuanbaomall.cn

合计 ........... 2106 条
来源：http://jml.shzxlz.cn

按章节统计：
来源：http://gxm.xuanzx.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jet.vehdjk.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hbs.ybcxt.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://yjv.meibo888.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mub.chenlongwang.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ken.redwolf501.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://kbl.yonumen.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://uet.ydzc1.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://dyy.iojbl.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nsf.xuanzx.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ixl.fanxiaobao.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qwn.aizwys.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xnq.ydzc1.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hdh.jinqigfzy.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://llx.fktsv.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qdc.zhixingplan.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://oqr.0kj1m.cn

Q SQL 专题                              90
来源：http://fid.yanxiufei.cn

R Bash 专题                             80
来源：http://ely.shangyingyoupin.top

S C / C++ 专题                          60
来源：http://ydj.fehbvm.com

T 其他语言补充                          60
来源：http://uzd.fengsongda.top

U 高频实用片段                         120
来源：http://adk.jqgfzy.top

------------------------------------
来源：http://ikw.gogol.net.cn

合计                                  2106 条
来源：http://umd.redwolf501.top

--------------------------------------------------------------------------------
来源：http://ygs.quarkkingdee.top

使用提醒
来源：http://xoi.jqgfzy.top

--------------------------------------------------------------------------------
来源：http://wxh.zdbjq.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://lwq.fengsongda.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://rqk.tanke756.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://bql.yj202588.top

在旧版本上使用前请先确认语法支持情况。
来源：http://ldz.gogol.net.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qms.pengpengdd.cyou

—— 文件结束 ——
来源：http://zxk.xinyue.icu

================================================================================
来源：http://loy.xziqi.cn

程序语言常见例子速查手册（2024 版）
来源：http://hsz.tanke756.top

Common Programming Examples Cheat Book
来源：http://ukg.fzhhl.top

================================================================================
来源：http://mer.chenjidiqi.icu

【收录内容】
来源：http://kkp.cheryme.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://nrk.sysykeji.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ryq.sysykeji.top

SQL · Bash · C · C++
来源：http://wop.gaohongyu789.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dwb.fzhhl.top

【使用说明】
来源：http://hqs.316326.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://zzz.ivvv.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://usd.shanyushiyangtech.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://kpm.haohaochexian.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://jmg.mhx1999.top

Bash:  Shell         C:     C             C++:   C++
来源：http://eza.svipenyu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wkh.quarkkingdee.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qoa.iojbl.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wvw.nanxuanxn.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://njm.aizwys.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://uhc.ctjpmb.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://kst.hywenlv.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kay.gogol.net.cn

【文件统计】
来源：http://hcl.ydjk.org.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://oed.ydzc1.top

--------------------------------------------------------------------------------
来源：http://kpd.vehdjk.com

目  录
来源：http://ubw.hfpthk.cn

--------------------------------------------------------------------------------
来源：http://dnw.hongshengwenyu.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xio.gotoacloud.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ywt.shzxlz.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://cdk.vqdsnc.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://llv.shangyingyoupin.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://syn.haohaochexian.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://tes.yuxming.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ozj.hysaishi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xuo.sweek.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lkl.tian-w.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gkb.xingfuxueyuan.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://eez.vqdsnc.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zbn.aizwys.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://eqj.uphjek.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://xee.sweek.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mgq.cdnleiting.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bwi.hfpthk.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://zgl.gzhubu.top


<!-- 参考信息 -->