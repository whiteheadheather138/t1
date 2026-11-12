代发 wailian999

[U15] Py：高精度计时
来源：http://cnx.yuanzhike.top

t = time.perf_counter()
来源：http://qmt.uphjek.com

[U16] Py：命令行参数解析
来源：http://ybk.dianchejie.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qtt.chenzaomai.com

[U17] Py：初始化日志
来源：http://koo.0kj1m.cn

logging.basicConfig(level=logging.INFO)
来源：http://ehu.yueranfly.top

[U18] Py：预编译正则
来源：http://vao.zdbjq.cn

pat = re.compile(r"\d+")
来源：http://hbl.gotoacloud.top

[U19] Py：正则替换带回调
来源：http://iqm.9152youxi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xzx.sweek.top

[U20] Py：缓存函数结果
来源：http://wrr.xingfuxueyuan.xyz

@functools.lru_cache(maxsize=None)
来源：http://zwr.hammf.cn

[U21] Py：自定义上下文管理器
来源：http://guo.yuxming.cn

@contextlib.contextmanager
来源：http://iwl.nanxinkj.top

[U22] Py：矩阵转置
来源：http://xcg.quarkkingdee.top

list(zip(*m))
来源：http://tcb.316326.xyz

[U23] Py：分块读取大文件
来源：http://qty.shuidangran.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pqa.sweek.top

[U24] Py：路径操作
来源：http://fpo.xinyue.icu

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qvz.ywan-chungtsiang.top

[U25] Py：CSV 按字典读
来源：http://hcm.birdmap.top

csv.DictReader(f)
来源：http://smb.wangshuangyany.cn

[U26] Py：并发下载
来源：http://ugu.vqdsnc.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://iwz.jqgufenzy.top

[U27] Py：异步 HTTP
来源：http://vkh.xylfe.cn

aiohttp.ClientSession() 配合 async with
来源：http://jyd.zhongyouzk.top

[U28] Py：类型别名
来源：http://htv.smart0.xyz

UserId = int
来源：http://mqu.wangdashe.top

[U29] Py：属性校验
来源：http://uau.jianghu66.top

@property 与 @x.setter 配合
来源：http://wfb.jqgfzy.top

[U30] Py：数据类
来源：http://alc.zhixingplan.top

@dataclass(slots=True)
来源：http://ngf.redwolf501.top

[U31] Py：单测
来源：http://hbw.xuanzx.com

python -m pytest -q
来源：http://iem.bbcook.cn

[U32] Py：代码格式化
来源：http://wsc.cashguo.top

ruff format . && ruff check --fix .
来源：http://rrs.birdmap.top

[U33] Py：打包发布
来源：http://loe.hongshengwenyu.top

python -m build  （依赖 pyproject.toml）
来源：http://dkv.hammf.cn

[U34] Py：判断编码
来源：http://pqb.vehdjk.com

chardet.detect(raw)
来源：http://lpw.gotoacloud.top

[U35] Py：发送邮件
来源：http://klc.jianghu66.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ipj.hnqzz.top

[U36] Py：定时任务
来源：http://fqd.bjfxy.top

schedule.every(10).minutes.do(job)
来源：http://eig.dashuyun.cn

[U37] Py：读写 Excel
来源：http://nkt.epnwcf.com

pandas.read_excel / DataFrame.to_excel
来源：http://hht.hysaishi.cn

[U38] Py：获取脚本所在目录
来源：http://rqb.dianchejie.cn

Path(__file__).resolve().parent
来源：http://tln.fktsv.cn

[U39] Py：判断是否在交互环境
来源：http://rkf.smart0.xyz

sys.stdout.isatty()
来源：http://mmk.bjfxy.top

[U40] Py：打印到标准错误
来源：http://hao.bjfxy.top

print("err", file=sys.stderr)
来源：http://afr.gogol.net.cn

[U41] PHP：初始化 Composer 项目
来源：http://ipv.epnwcf.com

composer init;  composer require guzzlehttp/guzzle
来源：http://jka.sufxvd.cn

[U42] PHP：PSR-4 自动加载
来源：http://rdw.yanxiufei.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://csk.gotoacloud.top

[U43] PHP：声明命名空间
来源：http://gom.chenjidiqi.icu

namespace App\Http;
来源：http://tsa.nanxuanxn.top

[U44] PHP：开启严格类型
来源：http://jjy.yuxming.cn

declare(strict_types=1);
来源：http://yrx.vehdjk.com

[U45] PHP：类型声明与返回类型
来源：http://gnz.yvedp.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://per.ybcxt.top

[U46] PHP：可空类型
来源：http://qkd.jinyuanbaomall.cn

?string $name = null
来源：http://gpn.ybcxt.top

[U47] PHP：联合类型
来源：http://emw.sxryk.cn

int|string $id
来源：http://nyx.ybcxt.top

[U48] PHP：纯枚举
来源：http://fuw.ywan-chungtsiang.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rkl.redwolf501.top

[U49] PHP：只读属性
来源：http://jco.c1oappe.top

public readonly string $name
来源：http://nyh.feifeiyinyue.top

[U50] PHP：构造器属性提升
来源：http://iuy.ehwqpu.com

public function __construct(private int $id) {}
来源：http://mpy.ehwqpu.com

[U51] PHP：数组解构
来源：http://jdc.yongpay.top

[$a, $b] = $arr;
来源：http://toi.kuanghao11.cn

[U52] PHP：箭头函数
来源：http://wtj.pengpengdd.cyou

$double = fn($x) => $x * 2;
来源：http://mit.fktsv.cn

[U53] PHP：空合并运算符
来源：http://zds.cdnleiting.top

$v = $a ?? $b ?? "default";
来源：http://vou.wangshuangyany.cn

[U54] PHP：空安全调用
来源：http://bqc.zhoulong.xyz

$obj?->method()
来源：http://qul.wangdashe.top

[U55] PHP：match 表达式
来源：http://bif.fzhhl.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ggk.yangfankeji.com

[U56] PHP：命名参数
来源：http://mfu.cucudq.cn

f(a: 1, b: 2)
来源：http://sno.ctjpmb.com

[U57] PHP：字符串插值
来源：http://fqd.guannengcc.top

"值: {$a}"
来源：http://ugm.hammf.cn

[U58] PHP：数组三件套
来源：http://enz.pycfn.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gqy.yuxming.cn

[U59] PHP：自定义排序
来源：http://jik.yj20258888.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ksm.feifeiyinyue.top

[U60] PHP：JSON 编解码
来源：http://pei.svipenyu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kow.jyoumei.cn

[U61] PHP：正则
来源：http://qit.jinqigfzy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://sfa.yj20258888.top

[U62] PHP：日期对象
来源：http://byt.uphjek.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gil.zhengqikj.top

[U63] PHP：文件读写
来源：http://dvs.cheryme.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hia.9152youxi.cn

[U64] PHP：目录遍历
来源：http://xlf.jinghuilouyu.cn

glob("dir/*.php");  scandir("dir");
来源：http://ufp.zdbjq.cn

[U65] PHP：会话
来源：http://udo.jyoumei.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://tey.yangfankeji.com

[U66] PHP：设置 Cookie
来源：http://fml.yj20258888.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sdi.sjlbkw.cn

[U67] PHP：处理文件上传
来源：http://wbf.xingfuxueyuan.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mtt.jqgfzy.top

[U68] PHP：PDO 连接
来源：http://ncy.yongpay.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ezg.jinyuanbaomall.cn

[U69] PHP：PDO 预处理
来源：http://phi.guannengcc.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ama.zhoulong.xyz

[U70] PHP：PDO 事务
来源：http://eku.jinqigufen.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mya.ybcxt.top

[U71] PHP：抛出异常
来源：http://ibr.haohaochexian.top

throw new RuntimeException("失败", 500);
来源：http://uje.feifeiyinyue.top

[U72] PHP：写错误日志
来源：http://hyr.chenzaomai.com

error_log("失败: " . $e->getMessage());
来源：http://qsm.gzhubu.top

[U73] PHP：读取 ini 配置
来源：http://yuw.birdmap.top

parse_ini_file("config.ini", true)
来源：http://eds.yueranfly.top

[U74] PHP：读取环境变量
来源：http://bpa.0kj1m.cn

getenv("APP_ENV") ?: "production"
来源：http://ybi.feifeiyinyue.top

[U75] PHP：依赖注入
来源：http://qjj.pengpengdd.cyou

composer require psr/container
来源：http://rvw.gogol.net.cn

[U76] PHP：简单路由
来源：http://lfz.xziqi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jqx.andypj.xyz

[U77] PHP：模板渲染
来源：http://dod.hesvh.cn

composer require twig/twig
来源：http://cgc.bjfxy.top

[U78] PHP：单元测试
来源：http://dbf.sxryk.cn

composer require --dev phpunit/phpunit
来源：http://hrh.gzhubu.top

[U79] PHP：静态分析
来源：http://qgr.zdqjudy.top

composer require --dev phpstan/phpstan
来源：http://hqu.tarul.cn

[U80] PHP：代码规范修复
来源：http://gnu.ctjpmb.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://zkl.jinyuanbaomall.cn

[U81] JS：初始化项目
来源：http://tup.wangshuangyany.cn

npm init -y;  npm i express
来源：http://fwg.jinqigufen.top

[U82] JS：package.json 脚本
来源：http://nrq.bbcook.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://yya.cucudq.cn

[U83] JS：ES Module 导入导出
来源：http://tdc.xuanzx.com

export const a = 1;  import { a } from "./m.js";
来源：http://xas.andypj.xyz

[U84] JS：CommonJS 写法
来源：http://rdz.aibaodan.cn

module.exports = { a };  const { a } = require("./m");
来源：http://epc.mhx1999.top

[U85] JS：可选链
来源：http://jti.hywenlv.cn

a?.b?.c
来源：http://qyr.jinghuilouyu.cn

[U86] JS：空值合并
来源：http://mvg.tianlin.xyz

a ?? b
来源：http://gof.xylfe.cn

[U87] JS：解构默认值
来源：http://kcz.xingfuxueyuan.xyz

const { a = 1, b = 2 } = obj;
来源：http://hdb.dashuyun.cn

[U88] JS：对象展开合并
来源：http://ugp.cheryme.top

{ ...a, ...b }
来源：http://wrr.epnwcf.com

[U89] JS：数组去重
来源：http://sns.yongpay.top

[...new Set(arr)]
来源：http://fnu.zhoulong.xyz

[U90] JS：数字数组排序
来源：http://isa.316326.xyz

[...arr].sort((a, b) => a - b)
来源：http://jsb.ppjwa.cn

[U91] JS：对象键值遍历
来源：http://fff.yangfankeji.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wxa.ivvv.top

[U92] JS：深拷贝
来源：http://dmk.xziqi.cn

structuredClone(obj)
来源：http://xiz.svipenyu.cn

[U93] JS：模板字符串
来源：http://urd.yuanzhike.top

`共 ${n} 条`
来源：http://gqg.yj202588.top

[U94] JS：箭头函数
来源：http://mgr.0kj1m.cn

const double = x => x * 2;
来源：http://mqf.shanyushiyangtech.top

[U95] JS：Promise 包装
来源：http://lnr.cucudq.cn

new Promise((resolve, reject) => {})
来源：http://gws.xinyue.icu

[U96] JS：async/await 与异常
来源：http://gph.yj20258888.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qeo.c1oappe.top

[U97] JS：并发请求
来源：http://nyz.xziqi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://zzv.cheryme.top

[U98] JS：fetch 带 JSON
来源：http://pda.tarul.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://dtj.dashuyun.cn

[U99] JS：事件监听
来源：http://aaq.yvedp.cn

el.addEventListener("click", e => {})
来源：http://vop.havefunace.top

[U100] JS：DOM 查询
来源：http://bge.zhixingplan.top

document.querySelector(".item")
来源：http://dom.meibo888.top

[U101] JS：classList 操作
来源：http://btr.ehwqpu.com

el.classList.toggle("active")
来源：http://kxj.bbcook.cn

[U102] JS：本地存储
来源：http://cmw.ydzc1.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://uaf.xingfuxueyuan.xyz

[U103] JS：定时器
来源：http://jwv.gaohongyu789.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rgk.52xcode.cn

[U104] JS：防抖
来源：http://xac.zhoulong.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nwj.jinyuanbaomall.cn

[U105] JS：节流
来源：http://xte.fzhhl.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ovk.andypj.xyz

[U106] JS：日期格式化
来源：http://whq.hammf.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zuu.bjfxy.top

[U107] JS：数字千分位
来源：http://aup.9152youxi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cgo.chenlongwang.top

[U108] JS：随机整数
来源：http://xpe.yj202588.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bni.52xcode.cn

[U109] JS：数组分组
来源：http://kdj.gotoacloud.top

Object.groupBy(arr, x => x.type)
来源：http://zjl.mhx1999.top

[U110] JS：数组分块
来源：http://jom.jqgfzy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://oxs.jlsjyb.cn

[U111] JS：对象转 Map
来源：http://zia.bjfxy.top

new Map(Object.entries(obj))
来源：http://cug.daria6918.cn

[U112] JS：字符串补位
来源：http://jst.hywenlv.cn

"7".padStart(3, "0")
来源：http://xtn.hnxiangtu.top

[U113] JS：正则替换全部
来源：http://qlf.smart0.xyz

s.replaceAll("a", "b")
来源：http://fhk.fanxiaobao.xyz

[U114] JS：JSON 深比较
来源：http://dnw.shuidangran.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://snt.zycfv.cn

[U115] JS：生成 UUID
来源：http://cyr.chenjidiqi.icu

crypto.randomUUID()
来源：http://fhv.shanyushiyangtech.top

[U116] JS：类型检查（JSDoc）
来源：http://gfw.zhixingplan.top

/** @param {string} name */ function f(name) {}
来源：http://nan.hfpthk.cn

[U117] JS：单元测试
来源：http://bku.yuanzhike.top

npm i -D vitest;  npx vitest
来源：http://ljq.snrcjt.cn

[U118] JS：开发服务器
来源：http://xba.gogol.net.cn

npm i -D vite;  npx vite
来源：http://fgl.nwbrower.top

[U119] JS：生产构建
来源：http://whn.zhiwuduotai.top

npx vite build
来源：http://gqe.cucudq.cn

[U120] JS：读取环境变量（Vite）
来源：http://vyk.yuxming.cn

import.meta.env.VITE_API_URL
来源：http://fss.quarkkingdee.top

================================================================================
来源：http://sjh.tianlin.xyz

统计汇总
来源：http://bcc.zhixingplan.top

================================================================================
来源：http://skm.chenjidiqi.icu

按语言统计（条）：
来源：http://hog.jqgufenzy.top

Python ......... 252
来源：http://cgh.tanke756.top

PHP ............ 252
来源：http://svb.hcnkem.com

JavaScript ..... 252
来源：http://yis.tian-w.cn

TypeScript ..... 212
来源：http://dxh.svipenyu.cn

Java ........... 212
来源：http://lsc.nanxinkj.top

Go ............. 212
来源：http://pme.snrcjt.cn

Ruby ........... 212
来源：http://dco.jqgufenzy.top

C# ............. 212
来源：http://ifx.sjlbkw.cn

C .............. 30
来源：http://yli.shzxlz.cn

C++ ............ 30
来源：http://hnh.uphjek.com

SQL ............ 90
来源：http://foz.zhongyouzk.top

Bash ........... 80
来源：http://fom.zhengqikj.top

Kotlin ......... 15
来源：http://wla.zycfv.cn

Swift .......... 15
来源：http://nwn.ydjk.org.cn

Lua ............ 10
来源：http://dal.hongshengwenyu.top

Perl ........... 10
来源：http://xxc.hnqzz.top

Scala .......... 10
来源：http://azj.yongpay.top

------------------------------------
来源：http://dvs.hysaishi.cn

合计 ........... 2106 条
来源：http://dnl.gaohongyu789.top

按章节统计：
来源：http://aly.tianlin.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://uwq.ppjwa.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hrs.sjlbkw.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ynp.tanke756.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kze.pycfn.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bis.yueranfly.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://cff.ywan-chungtsiang.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hvy.ywan-chungtsiang.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://met.wangdashe.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rto.chenzaomai.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ilo.sufxvd.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://set.shanyushiyangkeji.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lng.yj202588.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://tnn.pengpengdd.cyou

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://man.jqgfzy.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jur.wangshuangyany.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dsf.hnqzz.top

Q SQL 专题                              90
来源：http://qfu.zycfv.cn

R Bash 专题                             80
来源：http://kzb.zhixingplan.top

S C / C++ 专题                          60
来源：http://osp.hnqzz.top

T 其他语言补充                          60
来源：http://toc.yonumen.top

U 高频实用片段                         120
来源：http://kwg.feifeiyinyue.top

------------------------------------
来源：http://gko.zhaomingkeji.xyz

合计                                  2106 条
来源：http://inf.zhaomingkeji.xyz

--------------------------------------------------------------------------------
来源：http://ahf.fktsv.cn

使用提醒
来源：http://jok.ppjwa.cn

--------------------------------------------------------------------------------
来源：http://tfw.shangyingyoupin.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nwf.tian-w.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://eiz.yvedp.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ari.fzhhl.top

在旧版本上使用前请先确认语法支持情况。
来源：http://ttx.meibo888.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://atn.sweek.top

—— 文件结束 ——
来源：http://vzq.hnqzz.top

================================================================================
来源：http://qsl.mhx1999.top

程序语言常见例子速查手册（2024 版）
来源：http://zwy.shzxlz.cn

Common Programming Examples Cheat Book
来源：http://bts.fzhhl.top

================================================================================
来源：http://dug.fktsv.cn

【收录内容】
来源：http://khp.jinqigufen.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://fxh.gotoacloud.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://vtf.pycfn.com

SQL · Bash · C · C++
来源：http://lfc.pycfn.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://kyu.jyoumei.cn

【使用说明】
来源：http://rjo.xinyue.icu

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://zek.cashguo.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mdd.ehwqpu.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://roi.jinqigufen.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://iht.mhx1999.top

Bash:  Shell         C:     C             C++:   C++
来源：http://rcz.aizwys.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://knk.mhx1999.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ili.52xcode.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://uui.cdnleiting.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://arf.sxryk.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ouh.hammf.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://cag.hnxiangtu.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://msc.andypj.xyz

【文件统计】
来源：http://rhy.ivvv.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wxo.bbcook.cn

--------------------------------------------------------------------------------
来源：http://zwd.gaohongyu789.top

目  录
来源：http://zlm.cucudq.cn

--------------------------------------------------------------------------------
来源：http://kva.hfpthk.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://toa.aibaodan.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wif.tarul.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://gpe.hywenlv.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://iaa.hysaishi.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://oef.hammf.cn


<!-- 参考信息 -->