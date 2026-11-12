代发 wailian999

[U15] Py：高精度计时
来源：http://rkb.fzhhl.top

t = time.perf_counter()
来源：http://tmb.zdqjudy.top

[U16] Py：命令行参数解析
来源：http://ork.jinqigufen.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lax.ehwqpu.com

[U17] Py：初始化日志
来源：http://awz.yuanzhike.top

logging.basicConfig(level=logging.INFO)
来源：http://jux.ctjpmb.com

[U18] Py：预编译正则
来源：http://bnc.bbcook.cn

pat = re.compile(r"\d+")
来源：http://mlz.yj20258888.top

[U19] Py：正则替换带回调
来源：http://baq.xylfe.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lff.yuanzhike.top

[U20] Py：缓存函数结果
来源：http://tev.pengpengdd.cyou

@functools.lru_cache(maxsize=None)
来源：http://hdt.sjlbkw.cn

[U21] Py：自定义上下文管理器
来源：http://uag.shangyingyoupin.top

@contextlib.contextmanager
来源：http://hft.svipenyu.cn

[U22] Py：矩阵转置
来源：http://ulq.yj202588.top

list(zip(*m))
来源：http://xeu.hysaishi.cn

[U23] Py：分块读取大文件
来源：http://zhz.aibaodan.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dzc.shzxlz.cn

[U24] Py：路径操作
来源：http://vtw.hfpthk.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://sii.sufxvd.cn

[U25] Py：CSV 按字典读
来源：http://xyv.shangyingyoupin.top

csv.DictReader(f)
来源：http://xjt.dashuyun.cn

[U26] Py：并发下载
来源：http://oiz.jinyuanbaomall.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rqp.0kj1m.cn

[U27] Py：异步 HTTP
来源：http://zga.zhiwuduotai.top

aiohttp.ClientSession() 配合 async with
来源：http://kmv.hfpthk.cn

[U28] Py：类型别名
来源：http://qic.shanyushiyangkeji.top

UserId = int
来源：http://hoi.chenzaomai.com

[U29] Py：属性校验
来源：http://uei.mhx1999.top

@property 与 @x.setter 配合
来源：http://itw.yfazqb.com

[U30] Py：数据类
来源：http://vys.yuxming.cn

@dataclass(slots=True)
来源：http://tqc.gotoacloud.top

[U31] Py：单测
来源：http://luh.ydjk.org.cn

python -m pytest -q
来源：http://qlc.wangshuangyany.cn

[U32] Py：代码格式化
来源：http://oys.sysykeji.top

ruff format . && ruff check --fix .
来源：http://wij.zdbjq.cn

[U33] Py：打包发布
来源：http://cde.yuxming.cn

python -m build  （依赖 pyproject.toml）
来源：http://riq.fanxiaobao.xyz

[U34] Py：判断编码
来源：http://hnc.hammf.cn

chardet.detect(raw)
来源：http://zup.fengsongda.top

[U35] Py：发送邮件
来源：http://csz.52xcode.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yly.cashguo.top

[U36] Py：定时任务
来源：http://mnl.iojbl.cn

schedule.every(10).minutes.do(job)
来源：http://wwe.hfpthk.cn

[U37] Py：读写 Excel
来源：http://wly.jlsjyb.cn

pandas.read_excel / DataFrame.to_excel
来源：http://vfw.ctjpmb.com

[U38] Py：获取脚本所在目录
来源：http://bpy.hnxiangtu.top

Path(__file__).resolve().parent
来源：http://jvg.jinqigfzy.top

[U39] Py：判断是否在交互环境
来源：http://ghv.cheryme.top

sys.stdout.isatty()
来源：http://xkv.birdmap.top

[U40] Py：打印到标准错误
来源：http://tse.52xcode.cn

print("err", file=sys.stderr)
来源：http://fyx.andypj.xyz

[U41] PHP：初始化 Composer 项目
来源：http://ign.yj20258.top

composer init;  composer require guzzlehttp/guzzle
来源：http://wqs.shzxlz.cn

[U42] PHP：PSR-4 自动加载
来源：http://lxn.c1oappe.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mwr.mhx1999.top

[U43] PHP：声明命名空间
来源：http://qwk.pengpengdd.cyou

namespace App\Http;
来源：http://ssf.zycfv.cn

[U44] PHP：开启严格类型
来源：http://rrl.jinqigufen.top

declare(strict_types=1);
来源：http://yet.zhaomingkeji.xyz

[U45] PHP：类型声明与返回类型
来源：http://kum.daria6918.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://yeu.tian-w.cn

[U46] PHP：可空类型
来源：http://dio.birdmap.top

?string $name = null
来源：http://pyp.redwolf501.top

[U47] PHP：联合类型
来源：http://nnf.ppjwa.cn

int|string $id
来源：http://lfk.smart0.xyz

[U48] PHP：纯枚举
来源：http://hst.yj20258888.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ykj.zhiwuduotai.top

[U49] PHP：只读属性
来源：http://tzh.52xcode.cn

public readonly string $name
来源：http://clr.xuetiantiany.cn

[U50] PHP：构造器属性提升
来源：http://pki.svipenyu.cn

public function __construct(private int $id) {}
来源：http://pyv.nanxuanxn.top

[U51] PHP：数组解构
来源：http://pvo.quarkkingdee.top

[$a, $b] = $arr;
来源：http://rby.cheryme.top

[U52] PHP：箭头函数
来源：http://ojd.sysykeji.top

$double = fn($x) => $x * 2;
来源：http://upb.wangshuangyany.cn

[U53] PHP：空合并运算符
来源：http://wpe.aizwys.cn

$v = $a ?? $b ?? "default";
来源：http://ndh.mhx1999.top

[U54] PHP：空安全调用
来源：http://vvf.hfpthk.cn

$obj?->method()
来源：http://mgp.iojbl.cn

[U55] PHP：match 表达式
来源：http://kpk.pycfn.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yrc.c1oappe.top

[U56] PHP：命名参数
来源：http://hvz.316326.xyz

f(a: 1, b: 2)
来源：http://pou.pengpengdd.cyou

[U57] PHP：字符串插值
来源：http://yyg.zycfv.cn

"值: {$a}"
来源：http://vdq.shuidangran.top

[U58] PHP：数组三件套
来源：http://oek.zhaomingkeji.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://anp.hongshengwenyu.top

[U59] PHP：自定义排序
来源：http://fnp.hongshengwenyu.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cvx.xuanzx.com

[U60] PHP：JSON 编解码
来源：http://uho.zdbjq.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hlc.shanyushiyangkeji.top

[U61] PHP：正则
来源：http://iut.feifeiyinyue.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ahu.yueranfly.top

[U62] PHP：日期对象
来源：http://oqv.nwbrower.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jfa.jlsjyb.cn

[U63] PHP：文件读写
来源：http://icv.meibo888.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mbd.uphjek.com

[U64] PHP：目录遍历
来源：http://msl.gogol.net.cn

glob("dir/*.php");  scandir("dir");
来源：http://fsg.chenlongwang.top

[U65] PHP：会话
来源：http://lgf.hnqzz.top

session_start();  $_SESSION["uid"] = 1;
来源：http://nue.jinyuanbaomall.cn

[U66] PHP：设置 Cookie
来源：http://uti.zhoulong.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wiz.zhaomingkeji.xyz

[U67] PHP：处理文件上传
来源：http://ueq.zycfv.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jaz.yvedp.cn

[U68] PHP：PDO 连接
来源：http://awp.feifeiyinyue.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qim.gzhubu.top

[U69] PHP：PDO 预处理
来源：http://bse.ppjwa.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dgu.yangfankeji.com

[U70] PHP：PDO 事务
来源：http://mgd.iojbl.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dhi.haohaochexian.top

[U71] PHP：抛出异常
来源：http://beu.zhengqikj.top

throw new RuntimeException("失败", 500);
来源：http://buw.fzhhl.top

[U72] PHP：写错误日志
来源：http://brw.xylfe.cn

error_log("失败: " . $e->getMessage());
来源：http://lgj.cucudq.cn

[U73] PHP：读取 ini 配置
来源：http://mwe.sufxvd.cn

parse_ini_file("config.ini", true)
来源：http://zqo.cdnleiting.top

[U74] PHP：读取环境变量
来源：http://gkd.jinqigufen.top

getenv("APP_ENV") ?: "production"
来源：http://izv.yj20258888.top

[U75] PHP：依赖注入
来源：http://hwz.fengsongda.top

composer require psr/container
来源：http://chz.guannengcc.top

[U76] PHP：简单路由
来源：http://fgt.ctjpmb.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://cck.hcnkem.com

[U77] PHP：模板渲染
来源：http://mlv.yueranfly.top

composer require twig/twig
来源：http://dir.yongpay.top

[U78] PHP：单元测试
来源：http://psh.zhoulong.xyz

composer require --dev phpunit/phpunit
来源：http://brp.havefunace.top

[U79] PHP：静态分析
来源：http://szy.fzhhl.top

composer require --dev phpstan/phpstan
来源：http://ubp.yuanzhike.top

[U80] PHP：代码规范修复
来源：http://rkg.tarul.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://dyb.9152youxi.cn

[U81] JS：初始化项目
来源：http://bpm.chenzaomai.com

npm init -y;  npm i express
来源：http://nts.shuidangran.top

[U82] JS：package.json 脚本
来源：http://wbn.shzxlz.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jxg.jlsjyb.cn

[U83] JS：ES Module 导入导出
来源：http://oza.tianlin.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://fex.iojbl.cn

[U84] JS：CommonJS 写法
来源：http://frb.mhx1999.top

module.exports = { a };  const { a } = require("./m");
来源：http://vdv.pycfn.com

[U85] JS：可选链
来源：http://dkl.fzhhl.top

a?.b?.c
来源：http://ats.tanke756.top

[U86] JS：空值合并
来源：http://rou.redwolf501.top

a ?? b
来源：http://qpv.9152youxi.cn

[U87] JS：解构默认值
来源：http://vxc.yvedp.cn

const { a = 1, b = 2 } = obj;
来源：http://pev.yangfankeji.com

[U88] JS：对象展开合并
来源：http://nci.chenjidiqi.icu

{ ...a, ...b }
来源：http://tmj.epnwcf.com

[U89] JS：数组去重
来源：http://egm.yvedp.cn

[...new Set(arr)]
来源：http://yol.hammf.cn

[U90] JS：数字数组排序
来源：http://mpo.daxiang520.top

[...arr].sort((a, b) => a - b)
来源：http://khu.zhijiandao.cn

[U91] JS：对象键值遍历
来源：http://ltv.yj20258888.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jks.gaohongyu789.top

[U92] JS：深拷贝
来源：http://sfu.hnxiangtu.top

structuredClone(obj)
来源：http://xxw.zhiwuduotai.top

[U93] JS：模板字符串
来源：http://jsw.ydzc1.top

`共 ${n} 条`
来源：http://yxr.yj20258888.top

[U94] JS：箭头函数
来源：http://mxs.feifeiyinyue.top

const double = x => x * 2;
来源：http://rbb.vqdsnc.cn

[U95] JS：Promise 包装
来源：http://act.tarul.cn

new Promise((resolve, reject) => {})
来源：http://zbe.fzhhl.top

[U96] JS：async/await 与异常
来源：http://tyg.zhiwuduotai.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ccc.jlsjyb.cn

[U97] JS：并发请求
来源：http://xpe.redwolf501.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://rnt.tanke756.top

[U98] JS：fetch 带 JSON
来源：http://dev.guowangkeji.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bov.wangshuangyany.cn

[U99] JS：事件监听
来源：http://hxc.sysykeji.top

el.addEventListener("click", e => {})
来源：http://bzl.zdbjq.cn

[U100] JS：DOM 查询
来源：http://txe.andypj.xyz

document.querySelector(".item")
来源：http://vob.tanke756.top

[U101] JS：classList 操作
来源：http://mul.tian-w.cn

el.classList.toggle("active")
来源：http://ydp.hongshengwenyu.top

[U102] JS：本地存储
来源：http://twk.wangshuangyany.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://lmo.hcnkem.com

[U103] JS：定时器
来源：http://gep.havefunace.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vzp.yfazqb.com

[U104] JS：防抖
来源：http://ezo.nwbrower.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bde.wangshuangyany.cn

[U105] JS：节流
来源：http://rql.yonumen.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qri.zhongyouzk.top

[U106] JS：日期格式化
来源：http://ynu.smart0.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://atj.wangdashe.top

[U107] JS：数字千分位
来源：http://hdn.ctjpmb.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cjt.snrcjt.cn

[U108] JS：随机整数
来源：http://wpo.meibo888.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kqz.epnwcf.com

[U109] JS：数组分组
来源：http://kwe.kuanghao11.cn

Object.groupBy(arr, x => x.type)
来源：http://xyb.shanyushiyangkeji.top

[U110] JS：数组分块
来源：http://fio.xinyue.icu

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yst.hcnkem.com

[U111] JS：对象转 Map
来源：http://zrr.zhijiandao.cn

new Map(Object.entries(obj))
来源：http://nkw.xziqi.cn

[U112] JS：字符串补位
来源：http://ldj.jlsjyb.cn

"7".padStart(3, "0")
来源：http://lyy.feifeiyinyue.top

[U113] JS：正则替换全部
来源：http://zqc.fzhhl.top

s.replaceAll("a", "b")
来源：http://yrx.hammf.cn

[U114] JS：JSON 深比较
来源：http://cca.tian-w.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://etr.zhengqikj.top

[U115] JS：生成 UUID
来源：http://hpv.yuanzhike.top

crypto.randomUUID()
来源：http://pyy.cashguo.top

[U116] JS：类型检查（JSDoc）
来源：http://lbc.9152youxi.cn

/** @param {string} name */ function f(name) {}
来源：http://mdf.nanxuanxn.top

[U117] JS：单元测试
来源：http://rzz.pengpengdd.cyou

npm i -D vitest;  npx vitest
来源：http://cas.zycfv.cn

[U118] JS：开发服务器
来源：http://glo.ydjk.org.cn

npm i -D vite;  npx vite
来源：http://fco.yanxiufei.cn

[U119] JS：生产构建
来源：http://bmy.hfpthk.cn

npx vite build
来源：http://qpu.zhaomingkeji.xyz

[U120] JS：读取环境变量（Vite）
来源：http://cmc.sufxvd.cn

import.meta.env.VITE_API_URL
来源：http://jmv.jiagoushi.top

================================================================================
来源：http://evk.meibo888.top

统计汇总
来源：http://adr.fehbvm.com

================================================================================
来源：http://etl.ybcxt.top

按语言统计（条）：
来源：http://vqh.sjlbkw.cn

Python ......... 252
来源：http://guu.ywan-chungtsiang.top

PHP ............ 252
来源：http://cec.gaohongyu789.top

JavaScript ..... 252
来源：http://pal.shzxlz.cn

TypeScript ..... 212
来源：http://kpg.316326.xyz

Java ........... 212
来源：http://srt.hesvh.cn

Go ............. 212
来源：http://uis.hnxiangtu.top

Ruby ........... 212
来源：http://ckv.shangyingyoupin.top

C# ............. 212
来源：http://emr.gaohongyu789.top

C .............. 30
来源：http://lxo.yongpay.top

C++ ............ 30
来源：http://rax.jqgfzy.top

SQL ............ 90
来源：http://qja.yuanzhike.top

Bash ........... 80
来源：http://sjx.daxiang520.top

Kotlin ......... 15
来源：http://gif.hongshengwenyu.top

Swift .......... 15
来源：http://sht.yangfankeji.com

Lua ............ 10
来源：http://zzo.yangfankeji.com

Perl ........... 10
来源：http://him.jinyuanbaomall.cn

Scala .......... 10
来源：http://len.nwbrower.top

------------------------------------
来源：http://yyb.hnqzz.top

合计 ........... 2106 条
来源：http://mzt.tanke756.top

按章节统计：
来源：http://jwh.guowangkeji.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gpt.andypj.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gwm.ybcxt.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ujb.ybcxt.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://joa.svipenyu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://skn.0kj1m.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://abg.yonumen.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xpy.redwolf501.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mwr.jyoumei.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://fng.daxiang520.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://isa.zdbjq.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ciq.snrcjt.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fsv.iojbl.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bda.aizwys.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://sow.jinghuilouyu.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ktq.birdmap.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://puh.hysaishi.cn

Q SQL 专题                              90
来源：http://efn.guowangkeji.top

R Bash 专题                             80
来源：http://tmr.nwbrower.top

S C / C++ 专题                          60
来源：http://vco.nanxinkj.top

T 其他语言补充                          60
来源：http://mxl.yanxiufei.cn

U 高频实用片段                         120
来源：http://gkk.zhongyouzk.top

------------------------------------
来源：http://daq.jinyuanbaomall.cn

合计                                  2106 条
来源：http://dsp.daria6918.cn

--------------------------------------------------------------------------------
来源：http://yif.fanxiaobao.xyz

使用提醒
来源：http://anb.gzhubu.top

--------------------------------------------------------------------------------
来源：http://nlb.gogol.net.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://bub.zhoulong.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xir.ppjwa.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ljn.svipenyu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://fqj.zhengqikj.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://efx.jyoumei.cn

—— 文件结束 ——
来源：http://fms.guannengcc.top

================================================================================
来源：http://nvc.hywenlv.cn

程序语言常见例子速查手册（2024 版）
来源：http://qml.xuetiantiany.cn

Common Programming Examples Cheat Book
来源：http://gbz.ctjpmb.com

================================================================================
来源：http://ppj.hywenlv.cn

【收录内容】
来源：http://sgq.xylfe.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://yzw.zhoulong.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wmu.guowangkeji.top

SQL · Bash · C · C++
来源：http://jds.feifeiyinyue.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://psw.nanxinkj.top

【使用说明】
来源：http://qkx.fengsongda.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://pjz.zdbjq.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://txt.redwolf501.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://afy.aizwys.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://lyk.aizwys.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://bjo.quarkkingdee.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://rmx.fktsv.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://spj.jinyuanbaomall.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://pkm.andypj.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ddt.nanxuanxn.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qvh.bjfxy.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://jse.zdbjq.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://lfu.ivvv.top

【文件统计】
来源：http://jgk.ppjwa.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hkd.shanyushiyangtech.top

--------------------------------------------------------------------------------
来源：http://oyt.yj202588.top

目  录
来源：http://ihy.pengpengdd.cyou

--------------------------------------------------------------------------------
来源：http://woc.xylfe.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://aos.chenjidiqi.icu

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qqs.havefunace.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://dlg.shanyushiyangkeji.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ida.cqqwz.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://xqx.hnqzz.top


<!-- 参考信息 -->