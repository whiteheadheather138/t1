代发 wailian999

[U15] Py：高精度计时
来源：http://xiz.cheryme.top

t = time.perf_counter()
来源：http://ptx.yj20258888.top

[U16] Py：命令行参数解析
来源：http://kbx.tianlin.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zdp.sxryk.cn

[U17] Py：初始化日志
来源：http://zcp.nanxinkj.top

logging.basicConfig(level=logging.INFO)
来源：http://zhh.zdqjudy.top

[U18] Py：预编译正则
来源：http://ole.hnqzz.top

pat = re.compile(r"\d+")
来源：http://gim.yvedp.cn

[U19] Py：正则替换带回调
来源：http://bpi.jqgfzy.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wkg.hysaishi.cn

[U20] Py：缓存函数结果
来源：http://vlx.daria6918.cn

@functools.lru_cache(maxsize=None)
来源：http://qmd.hesvh.cn

[U21] Py：自定义上下文管理器
来源：http://qud.jinyuanbaomall.cn

@contextlib.contextmanager
来源：http://rzl.jyoumei.cn

[U22] Py：矩阵转置
来源：http://qmm.nanxuanxn.top

list(zip(*m))
来源：http://pkt.chenlongwang.top

[U23] Py：分块读取大文件
来源：http://wfv.zhaomingkeji.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qcj.hcnkem.com

[U24] Py：路径操作
来源：http://ijp.yj20258888.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fqg.hnqzz.top

[U25] Py：CSV 按字典读
来源：http://lnc.pycfn.com

csv.DictReader(f)
来源：http://cku.gotoacloud.top

[U26] Py：并发下载
来源：http://gxi.ehwqpu.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lch.yuxming.cn

[U27] Py：异步 HTTP
来源：http://gkg.hammf.cn

aiohttp.ClientSession() 配合 async with
来源：http://mwi.nanxinkj.top

[U28] Py：类型别名
来源：http://opc.fktsv.cn

UserId = int
来源：http://esu.yangfankeji.com

[U29] Py：属性校验
来源：http://bcf.jinghuilouyu.cn

@property 与 @x.setter 配合
来源：http://zvz.andypj.xyz

[U30] Py：数据类
来源：http://hmw.hammf.cn

@dataclass(slots=True)
来源：http://lfx.hnxiangtu.top

[U31] Py：单测
来源：http://ave.svipenyu.cn

python -m pytest -q
来源：http://fuj.kuanghao11.cn

[U32] Py：代码格式化
来源：http://xvl.epnwcf.com

ruff format . && ruff check --fix .
来源：http://nxk.yfazqb.com

[U33] Py：打包发布
来源：http://xzl.zhoulong.xyz

python -m build  （依赖 pyproject.toml）
来源：http://zfw.tian-w.cn

[U34] Py：判断编码
来源：http://ywg.gaohongyu789.top

chardet.detect(raw)
来源：http://asb.hesvh.cn

[U35] Py：发送邮件
来源：http://bxv.nanxuanxn.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tyj.tianlin.xyz

[U36] Py：定时任务
来源：http://zge.bbcook.cn

schedule.every(10).minutes.do(job)
来源：http://wcv.haohaochexian.top

[U37] Py：读写 Excel
来源：http://tnh.gogol.net.cn

pandas.read_excel / DataFrame.to_excel
来源：http://dak.zhijiandao.cn

[U38] Py：获取脚本所在目录
来源：http://ydg.shanyushiyangkeji.top

Path(__file__).resolve().parent
来源：http://lya.daria6918.cn

[U39] Py：判断是否在交互环境
来源：http://uzg.xylfe.cn

sys.stdout.isatty()
来源：http://rgr.cheryme.top

[U40] Py：打印到标准错误
来源：http://xtv.zdqjudy.top

print("err", file=sys.stderr)
来源：http://krb.jinqigfzy.top

[U41] PHP：初始化 Composer 项目
来源：http://bys.xylfe.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://vzc.fzhhl.top

[U42] PHP：PSR-4 自动加载
来源：http://tox.yj20258.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bhu.vehdjk.com

[U43] PHP：声明命名空间
来源：http://bvi.hywenlv.cn

namespace App\Http;
来源：http://plm.tianlin.xyz

[U44] PHP：开启严格类型
来源：http://tdl.hfpthk.cn

declare(strict_types=1);
来源：http://jrv.ehwqpu.com

[U45] PHP：类型声明与返回类型
来源：http://lud.0kj1m.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://qmd.shuidangran.top

[U46] PHP：可空类型
来源：http://mau.jqgfzy.top

?string $name = null
来源：http://xxu.fanxiaobao.xyz

[U47] PHP：联合类型
来源：http://isx.gogol.net.cn

int|string $id
来源：http://ifj.gaohongyu789.top

[U48] PHP：纯枚举
来源：http://nhh.nanxinkj.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ndi.zycfv.cn

[U49] PHP：只读属性
来源：http://hoi.yj20258.top

public readonly string $name
来源：http://cae.fengsongda.top

[U50] PHP：构造器属性提升
来源：http://vyq.jyoumei.cn

public function __construct(private int $id) {}
来源：http://bzk.guannengcc.top

[U51] PHP：数组解构
来源：http://cee.gogol.net.cn

[$a, $b] = $arr;
来源：http://pfq.tianlin.xyz

[U52] PHP：箭头函数
来源：http://aao.smart0.xyz

$double = fn($x) => $x * 2;
来源：http://puf.sufxvd.cn

[U53] PHP：空合并运算符
来源：http://pnt.tian-w.cn

$v = $a ?? $b ?? "default";
来源：http://tou.xziqi.cn

[U54] PHP：空安全调用
来源：http://gxu.cucudq.cn

$obj?->method()
来源：http://gjv.9152youxi.cn

[U55] PHP：match 表达式
来源：http://rzn.jiagoushi.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fsi.yj202588.top

[U56] PHP：命名参数
来源：http://phq.ydzc1.top

f(a: 1, b: 2)
来源：http://hzl.fanxiaobao.xyz

[U57] PHP：字符串插值
来源：http://opa.sufxvd.cn

"值: {$a}"
来源：http://voe.jinqigfzy.top

[U58] PHP：数组三件套
来源：http://zhc.zhoulong.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://acl.hfpthk.cn

[U59] PHP：自定义排序
来源：http://vzm.nanxuanxn.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dqd.zhongyouzk.top

[U60] PHP：JSON 编解码
来源：http://jon.jyoumei.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bdy.shuidangran.top

[U61] PHP：正则
来源：http://yzo.iojbl.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ctc.meibo888.top

[U62] PHP：日期对象
来源：http://krs.0kj1m.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pub.yongpay.top

[U63] PHP：文件读写
来源：http://dgm.zdbjq.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://khn.tanke756.top

[U64] PHP：目录遍历
来源：http://kmp.ppjwa.cn

glob("dir/*.php");  scandir("dir");
来源：http://ikk.hesvh.cn

[U65] PHP：会话
来源：http://hed.cdnleiting.top

session_start();  $_SESSION["uid"] = 1;
来源：http://fdj.daria6918.cn

[U66] PHP：设置 Cookie
来源：http://sqa.jinqigufen.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://szz.ppjwa.cn

[U67] PHP：处理文件上传
来源：http://krr.nanxuanxn.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qkm.zhongyouzk.top

[U68] PHP：PDO 连接
来源：http://qqa.birdmap.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qla.0kj1m.cn

[U69] PHP：PDO 预处理
来源：http://tbh.jianghu66.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mmj.ybcxt.top

[U70] PHP：PDO 事务
来源：http://izq.tianlin.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jct.dianchejie.cn

[U71] PHP：抛出异常
来源：http://ckf.52xcode.cn

throw new RuntimeException("失败", 500);
来源：http://eta.fengsongda.top

[U72] PHP：写错误日志
来源：http://buk.yvedp.cn

error_log("失败: " . $e->getMessage());
来源：http://tqr.tianlin.xyz

[U73] PHP：读取 ini 配置
来源：http://uhd.dashuyun.cn

parse_ini_file("config.ini", true)
来源：http://lgo.zdqjudy.top

[U74] PHP：读取环境变量
来源：http://twd.c1oappe.top

getenv("APP_ENV") ?: "production"
来源：http://zbi.zhengqikj.top

[U75] PHP：依赖注入
来源：http://dyl.tarul.cn

composer require psr/container
来源：http://nvv.havefunace.top

[U76] PHP：简单路由
来源：http://cye.andypj.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://cci.ppjwa.cn

[U77] PHP：模板渲染
来源：http://vcq.tianlin.xyz

composer require twig/twig
来源：http://fny.jyoumei.cn

[U78] PHP：单元测试
来源：http://fbl.wangdashe.top

composer require --dev phpunit/phpunit
来源：http://fow.guannengcc.top

[U79] PHP：静态分析
来源：http://quo.dashuyun.cn

composer require --dev phpstan/phpstan
来源：http://apl.snrcjt.cn

[U80] PHP：代码规范修复
来源：http://ppd.chenjidiqi.icu

composer require --dev friendsofphp/php-cs-fixer
来源：http://wlc.jlsjyb.cn

[U81] JS：初始化项目
来源：http://sqj.birdmap.top

npm init -y;  npm i express
来源：http://kqo.jqgufenzy.top

[U82] JS：package.json 脚本
来源：http://bst.aizwys.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mmu.shangyingyoupin.top

[U83] JS：ES Module 导入导出
来源：http://kit.yfazqb.com

export const a = 1;  import { a } from "./m.js";
来源：http://bei.hysaishi.cn

[U84] JS：CommonJS 写法
来源：http://icb.0kj1m.cn

module.exports = { a };  const { a } = require("./m");
来源：http://bcq.yj20258.top

[U85] JS：可选链
来源：http://exq.jinqigufen.top

a?.b?.c
来源：http://nic.jqgfzy.top

[U86] JS：空值合并
来源：http://bbt.quarkkingdee.top

a ?? b
来源：http://qgw.chenjidiqi.icu

[U87] JS：解构默认值
来源：http://yrl.nwbrower.top

const { a = 1, b = 2 } = obj;
来源：http://qpa.yongpay.top

[U88] JS：对象展开合并
来源：http://avp.tian-w.cn

{ ...a, ...b }
来源：http://len.yuanzhike.top

[U89] JS：数组去重
来源：http://jvt.jianghu66.top

[...new Set(arr)]
来源：http://zmr.fzhhl.top

[U90] JS：数字数组排序
来源：http://bhf.fehbvm.com

[...arr].sort((a, b) => a - b)
来源：http://okh.quarkkingdee.top

[U91] JS：对象键值遍历
来源：http://tbu.guowangkeji.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ror.xuanzx.com

[U92] JS：深拷贝
来源：http://sug.hongshengwenyu.top

structuredClone(obj)
来源：http://kqk.vehdjk.com

[U93] JS：模板字符串
来源：http://mbx.jinyuanbaomall.cn

`共 ${n} 条`
来源：http://nqx.aizwys.cn

[U94] JS：箭头函数
来源：http://poo.jinyuanbaomall.cn

const double = x => x * 2;
来源：http://gvd.uphjek.com

[U95] JS：Promise 包装
来源：http://qao.yangfankeji.com

new Promise((resolve, reject) => {})
来源：http://phx.hnqzz.top

[U96] JS：async/await 与异常
来源：http://qah.cdnleiting.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jiq.daxiang520.top

[U97] JS：并发请求
来源：http://wec.tanke756.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://oxz.cashguo.top

[U98] JS：fetch 带 JSON
来源：http://vcj.hammf.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://dih.zhongyouzk.top

[U99] JS：事件监听
来源：http://sqo.cheryme.top

el.addEventListener("click", e => {})
来源：http://tix.yvedp.cn

[U100] JS：DOM 查询
来源：http://ime.zdbjq.cn

document.querySelector(".item")
来源：http://xqo.zhixingplan.top

[U101] JS：classList 操作
来源：http://omy.hnxiangtu.top

el.classList.toggle("active")
来源：http://gin.havefunace.top

[U102] JS：本地存储
来源：http://blq.jqgufenzy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://zdn.smart0.xyz

[U103] JS：定时器
来源：http://idk.shanyushiyangkeji.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://cjh.ctjpmb.com

[U104] JS：防抖
来源：http://cqm.yongpay.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hge.jlsjyb.cn

[U105] JS：节流
来源：http://rhe.shzxlz.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bww.c1oappe.top

[U106] JS：日期格式化
来源：http://pus.ybcxt.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xma.fzhhl.top

[U107] JS：数字千分位
来源：http://ohq.redwolf501.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bvm.feifeiyinyue.top

[U108] JS：随机整数
来源：http://wbf.zhaomingkeji.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://muh.yangfankeji.com

[U109] JS：数组分组
来源：http://vgw.zhiwuduotai.top

Object.groupBy(arr, x => x.type)
来源：http://pxv.tianlin.xyz

[U110] JS：数组分块
来源：http://fsf.shuidangran.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://frd.hammf.cn

[U111] JS：对象转 Map
来源：http://ygz.gzhubu.top

new Map(Object.entries(obj))
来源：http://ycc.ydjk.org.cn

[U112] JS：字符串补位
来源：http://woh.yongpay.top

"7".padStart(3, "0")
来源：http://yar.cucudq.cn

[U113] JS：正则替换全部
来源：http://qbw.xylfe.cn

s.replaceAll("a", "b")
来源：http://qcv.nwbrower.top

[U114] JS：JSON 深比较
来源：http://ofr.sjlbkw.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://lpm.wangdashe.top

[U115] JS：生成 UUID
来源：http://gza.hysaishi.cn

crypto.randomUUID()
来源：http://ofv.xziqi.cn

[U116] JS：类型检查（JSDoc）
来源：http://fnr.yj202588.top

/** @param {string} name */ function f(name) {}
来源：http://ebe.wangdashe.top

[U117] JS：单元测试
来源：http://xyt.kuanghao11.cn

npm i -D vitest;  npx vitest
来源：http://hnr.daxiang520.top

[U118] JS：开发服务器
来源：http://hgu.cheryme.top

npm i -D vite;  npx vite
来源：http://mlr.cashguo.top

[U119] JS：生产构建
来源：http://qqy.zhiwuduotai.top

npx vite build
来源：http://nyo.snrcjt.cn

[U120] JS：读取环境变量（Vite）
来源：http://guk.hesvh.cn

import.meta.env.VITE_API_URL
来源：http://hvl.cashguo.top

================================================================================
来源：http://csx.yanxiufei.cn

统计汇总
来源：http://psn.tian-w.cn

================================================================================
来源：http://oao.sweek.top

按语言统计（条）：
来源：http://oou.zhongyouzk.top

Python ......... 252
来源：http://bpx.bbcook.cn

PHP ............ 252
来源：http://hso.xziqi.cn

JavaScript ..... 252
来源：http://kpy.guowangkeji.top

TypeScript ..... 212
来源：http://ahr.wangshuangyany.cn

Java ........... 212
来源：http://tgt.zhongyouzk.top

Go ............. 212
来源：http://nhg.sweek.top

Ruby ........... 212
来源：http://una.pycfn.com

C# ............. 212
来源：http://scz.kuanghao11.cn

C .............. 30
来源：http://boq.sufxvd.cn

C++ ............ 30
来源：http://zil.ivvv.top

SQL ............ 90
来源：http://ggy.nanxinkj.top

Bash ........... 80
来源：http://nlv.jinqigfzy.top

Kotlin ......... 15
来源：http://usx.52xcode.cn

Swift .......... 15
来源：http://cwh.yvedp.cn

Lua ............ 10
来源：http://roo.jinghuilouyu.cn

Perl ........... 10
来源：http://jsn.316326.xyz

Scala .......... 10
来源：http://wbn.9152youxi.cn

------------------------------------
来源：http://pxf.yvedp.cn

合计 ........... 2106 条
来源：http://gyj.andypj.xyz

按章节统计：
来源：http://jav.zdbjq.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zzt.hnqzz.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dks.52xcode.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://tga.fehbvm.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://nfq.gaohongyu789.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://psk.havefunace.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://sqp.jinqigufen.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://biz.c1oappe.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ohg.cdnleiting.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zwc.sweek.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xzq.dashuyun.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://sdk.hfpthk.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rjf.jqgfzy.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://onn.xziqi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://fnr.shanyushiyangtech.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qjy.shanyushiyangkeji.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wtt.yj20258888.top

Q SQL 专题                              90
来源：http://cwz.shzxlz.cn

R Bash 专题                             80
来源：http://dyk.sufxvd.cn

S C / C++ 专题                          60
来源：http://wkl.gotoacloud.top

T 其他语言补充                          60
来源：http://sgs.yvedp.cn

U 高频实用片段                         120
来源：http://ati.ehwqpu.com

------------------------------------
来源：http://xjk.meibo888.top

合计                                  2106 条
来源：http://cfn.zhengqikj.top

--------------------------------------------------------------------------------
来源：http://lvq.ehwqpu.com

使用提醒
来源：http://zjl.sxryk.cn

--------------------------------------------------------------------------------
来源：http://elp.shanyushiyangtech.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://goa.smart0.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://pya.sxryk.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wqb.zhongyouzk.top

在旧版本上使用前请先确认语法支持情况。
来源：http://fzq.birdmap.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://oqg.cqqwz.cn

—— 文件结束 ——
来源：http://jmu.gzhubu.top

================================================================================
来源：http://rtt.zdbjq.cn

程序语言常见例子速查手册（2024 版）
来源：http://olq.9152youxi.cn

Common Programming Examples Cheat Book
来源：http://tdl.hcnkem.com

================================================================================
来源：http://ygm.feifeiyinyue.top

【收录内容】
来源：http://skm.yuanzhike.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://jhp.epnwcf.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://fmr.cdnleiting.top

SQL · Bash · C · C++
来源：http://jrr.hongshengwenyu.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jhu.vqdsnc.cn

【使用说明】
来源：http://ssi.sjlbkw.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cpp.tian-w.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://uiv.cheryme.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ils.tanke756.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gbl.birdmap.top

Bash:  Shell         C:     C             C++:   C++
来源：http://ome.yanxiufei.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://faj.kuanghao11.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://uoz.0kj1m.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ssp.ydjk.org.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://swi.andypj.xyz

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qjk.316326.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://cxb.fktsv.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://htb.zhaomingkeji.xyz

【文件统计】
来源：http://iup.yj20258888.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://eek.fanxiaobao.xyz

--------------------------------------------------------------------------------
来源：http://aey.sufxvd.cn

目  录
来源：http://rxd.zhongyouzk.top

--------------------------------------------------------------------------------
来源：http://gci.wangdashe.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://oau.zhengqikj.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hvv.hysaishi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://cog.xinyue.icu

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://bcr.ivvv.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://psm.chenjidiqi.icu


<!-- 参考信息 -->