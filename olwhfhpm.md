代发 wailian999

[U03] Py：加载 .env 配置
来源：http://qua.xziqi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://dgv.ivvv.top

[U04] Py：变量调试打印
来源：http://xaj.jyoumei.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://plg.nanxinkj.top

[U05] Py：列表去重且保序
来源：http://iec.hysaishi.cn

list(dict.fromkeys(arr))
来源：http://jnb.xinyue.icu

[U06] Py：合并两个字典
来源：http://xmx.yj202588.top

{**a, **b}
来源：http://myv.cqqwz.cn

[U07] Py：反转字典键值
来源：http://xcw.vqdsnc.cn

{v: k for k, v in d.items()}
来源：http://ifb.wangshuangyany.cn

[U08] Py：展平二维列表
来源：http://rmk.nanxinkj.top

[y for x in nested for y in x]
来源：http://uju.andypj.xyz

[U09] Py：字典取最大值的键
来源：http://vfk.jqgfzy.top

max(d, key=d.get)
来源：http://zan.yvedp.cn

[U10] Py：按值排序字典
来源：http://nsk.sjlbkw.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xzt.ywan-chungtsiang.top

[U11] Py：生成器表达式
来源：http://zjx.redwolf501.top

(x * 2 for x in arr)
来源：http://rgg.fanxiaobao.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://tpq.shanyushiyangkeji.top

Counter(arr).most_common(3)
来源：http://xec.xingfuxueyuan.xyz

[U13] Py：固定长度队列
来源：http://qji.fengsongda.top

deque(maxlen=10)
来源：http://vuu.ywan-chungtsiang.top

[U14] Py：分组收集到列表
来源：http://yua.c1oappe.top

defaultdict(list)
来源：http://zog.wangshuangyany.cn

[U15] Py：高精度计时
来源：http://tev.xziqi.cn

t = time.perf_counter()
来源：http://ncr.daxiang520.top

[U16] Py：命令行参数解析
来源：http://zqp.c1oappe.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fry.yonumen.top

[U17] Py：初始化日志
来源：http://kcz.wangdashe.top

logging.basicConfig(level=logging.INFO)
来源：http://zuo.ehwqpu.com

[U18] Py：预编译正则
来源：http://kmv.xuanzx.com

pat = re.compile(r"\d+")
来源：http://yki.zhaomingkeji.xyz

[U19] Py：正则替换带回调
来源：http://qgh.kuanghao11.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yec.ybcxt.top

[U20] Py：缓存函数结果
来源：http://vdf.daria6918.cn

@functools.lru_cache(maxsize=None)
来源：http://lel.hesvh.cn

[U21] Py：自定义上下文管理器
来源：http://fnj.ydzc1.top

@contextlib.contextmanager
来源：http://eew.yuanzhike.top

[U22] Py：矩阵转置
来源：http://ekt.yuxming.cn

list(zip(*m))
来源：http://gev.nanxuanxn.top

[U23] Py：分块读取大文件
来源：http://qjn.yj20258.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dhq.nanxuanxn.top

[U24] Py：路径操作
来源：http://ejn.wangshuangyany.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fcn.ydjk.org.cn

[U25] Py：CSV 按字典读
来源：http://hsm.yueranfly.top

csv.DictReader(f)
来源：http://foj.jyoumei.cn

[U26] Py：并发下载
来源：http://pvl.ctjpmb.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wce.jyoumei.cn

[U27] Py：异步 HTTP
来源：http://avp.xuanzx.com

aiohttp.ClientSession() 配合 async with
来源：http://dwo.xylfe.cn

[U28] Py：类型别名
来源：http://asn.vehdjk.com

UserId = int
来源：http://gyu.yueranfly.top

[U29] Py：属性校验
来源：http://isp.nanxuanxn.top

@property 与 @x.setter 配合
来源：http://wbw.jiagoushi.top

[U30] Py：数据类
来源：http://jlt.jyoumei.cn

@dataclass(slots=True)
来源：http://rbj.zhengqikj.top

[U31] Py：单测
来源：http://ykp.xuetiantiany.cn

python -m pytest -q
来源：http://aoh.yongpay.top

[U32] Py：代码格式化
来源：http://csg.svipenyu.cn

ruff format . && ruff check --fix .
来源：http://ltz.yanxiufei.cn

[U33] Py：打包发布
来源：http://ozs.meibo888.top

python -m build  （依赖 pyproject.toml）
来源：http://ydy.ivvv.top

[U34] Py：判断编码
来源：http://abf.fehbvm.com

chardet.detect(raw)
来源：http://msz.jinghuilouyu.cn

[U35] Py：发送邮件
来源：http://sam.sweek.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://adm.nwbrower.top

[U36] Py：定时任务
来源：http://roe.shzxlz.cn

schedule.every(10).minutes.do(job)
来源：http://lcu.chenlongwang.top

[U37] Py：读写 Excel
来源：http://rqi.yj202588.top

pandas.read_excel / DataFrame.to_excel
来源：http://boo.svipenyu.cn

[U38] Py：获取脚本所在目录
来源：http://nhg.ydzc1.top

Path(__file__).resolve().parent
来源：http://pvv.havefunace.top

[U39] Py：判断是否在交互环境
来源：http://ukc.ywan-chungtsiang.top

sys.stdout.isatty()
来源：http://tun.svipenyu.cn

[U40] Py：打印到标准错误
来源：http://ocd.yanxiufei.cn

print("err", file=sys.stderr)
来源：http://taa.zdbjq.cn

[U41] PHP：初始化 Composer 项目
来源：http://tci.hongshengwenyu.top

composer init;  composer require guzzlehttp/guzzle
来源：http://pwp.daxiang520.top

[U42] PHP：PSR-4 自动加载
来源：http://dwk.daxiang520.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://kvi.jlsjyb.cn

[U43] PHP：声明命名空间
来源：http://axd.tian-w.cn

namespace App\Http;
来源：http://mio.redwolf501.top

[U44] PHP：开启严格类型
来源：http://zss.zhengqikj.top

declare(strict_types=1);
来源：http://rhc.hesvh.cn

[U45] PHP：类型声明与返回类型
来源：http://cnj.ybcxt.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://bib.jlsjyb.cn

[U46] PHP：可空类型
来源：http://lkj.zhijiandao.cn

?string $name = null
来源：http://llu.sysykeji.top

[U47] PHP：联合类型
来源：http://bnd.yuxming.cn

int|string $id
来源：http://zqa.tianlin.xyz

[U48] PHP：纯枚举
来源：http://pav.ydzc1.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dtc.chenlongwang.top

[U49] PHP：只读属性
来源：http://mpz.aibaodan.cn

public readonly string $name
来源：http://yvh.xziqi.cn

[U50] PHP：构造器属性提升
来源：http://dmf.zhoulong.xyz

public function __construct(private int $id) {}
来源：http://mzf.xuanzx.com

[U51] PHP：数组解构
来源：http://kiw.tanke756.top

[$a, $b] = $arr;
来源：http://uxf.sxryk.cn

[U52] PHP：箭头函数
来源：http://jzp.daxiang520.top

$double = fn($x) => $x * 2;
来源：http://xnm.ydzc1.top

[U53] PHP：空合并运算符
来源：http://tsj.jqgfzy.top

$v = $a ?? $b ?? "default";
来源：http://spr.chenjidiqi.icu

[U54] PHP：空安全调用
来源：http://bau.cashguo.top

$obj?->method()
来源：http://rvw.zhijiandao.cn

[U55] PHP：match 表达式
来源：http://hjg.bbcook.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wln.chenlongwang.top

[U56] PHP：命名参数
来源：http://zwx.xylfe.cn

f(a: 1, b: 2)
来源：http://uqy.yj20258.top

[U57] PHP：字符串插值
来源：http://fvq.hcnkem.com

"值: {$a}"
来源：http://dhj.gogol.net.cn

[U58] PHP：数组三件套
来源：http://rzb.zhengqikj.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zob.kuanghao11.cn

[U59] PHP：自定义排序
来源：http://ywy.zycfv.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ers.bjfxy.top

[U60] PHP：JSON 编解码
来源：http://iaw.chenzaomai.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kxj.ywan-chungtsiang.top

[U61] PHP：正则
来源：http://jyq.yanxiufei.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://thk.daria6918.cn

[U62] PHP：日期对象
来源：http://unr.jyoumei.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lum.hongshengwenyu.top

[U63] PHP：文件读写
来源：http://krf.cqqwz.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gvv.yongpay.top

[U64] PHP：目录遍历
来源：http://zmp.zhiwuduotai.top

glob("dir/*.php");  scandir("dir");
来源：http://wzf.tarul.cn

[U65] PHP：会话
来源：http://rro.ybcxt.top

session_start();  $_SESSION["uid"] = 1;
来源：http://xyz.xylfe.cn

[U66] PHP：设置 Cookie
来源：http://dry.zycfv.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://abi.yvedp.cn

[U67] PHP：处理文件上传
来源：http://zgh.pengpengdd.cyou

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://znp.gaohongyu789.top

[U68] PHP：PDO 连接
来源：http://xxe.xinyue.icu

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gim.ivvv.top

[U69] PHP：PDO 预处理
来源：http://gem.xinyue.icu

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xyo.cashguo.top

[U70] PHP：PDO 事务
来源：http://qra.tanke756.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qcz.pengpengdd.cyou

[U71] PHP：抛出异常
来源：http://jqa.redwolf501.top

throw new RuntimeException("失败", 500);
来源：http://ajm.gaohongyu789.top

[U72] PHP：写错误日志
来源：http://xzm.jqgfzy.top

error_log("失败: " . $e->getMessage());
来源：http://csa.shuidangran.top

[U73] PHP：读取 ini 配置
来源：http://fsr.jqgfzy.top

parse_ini_file("config.ini", true)
来源：http://kzy.jinyuanbaomall.cn

[U74] PHP：读取环境变量
来源：http://mui.shanyushiyangkeji.top

getenv("APP_ENV") ?: "production"
来源：http://qha.cdnleiting.top

[U75] PHP：依赖注入
来源：http://idh.bbcook.cn

composer require psr/container
来源：http://lcx.bbcook.cn

[U76] PHP：简单路由
来源：http://yrb.zhixingplan.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://uqx.yj20258.top

[U77] PHP：模板渲染
来源：http://ejb.jinyuanbaomall.cn

composer require twig/twig
来源：http://cts.wangdashe.top

[U78] PHP：单元测试
来源：http://ghb.yangfankeji.com

composer require --dev phpunit/phpunit
来源：http://ppz.ywan-chungtsiang.top

[U79] PHP：静态分析
来源：http://ooy.yj202588.top

composer require --dev phpstan/phpstan
来源：http://dpj.jqgfzy.top

[U80] PHP：代码规范修复
来源：http://hew.xinyue.icu

composer require --dev friendsofphp/php-cs-fixer
来源：http://lia.jqgfzy.top

[U81] JS：初始化项目
来源：http://giv.sjlbkw.cn

npm init -y;  npm i express
来源：http://ttu.andypj.xyz

[U82] JS：package.json 脚本
来源：http://iti.ppjwa.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://paz.gzhubu.top

[U83] JS：ES Module 导入导出
来源：http://ujv.daxiang520.top

export const a = 1;  import { a } from "./m.js";
来源：http://hti.ywan-chungtsiang.top

[U84] JS：CommonJS 写法
来源：http://inq.tian-w.cn

module.exports = { a };  const { a } = require("./m");
来源：http://haw.aibaodan.cn

[U85] JS：可选链
来源：http://pbd.9152youxi.cn

a?.b?.c
来源：http://yfk.sxryk.cn

[U86] JS：空值合并
来源：http://nxt.jqgfzy.top

a ?? b
来源：http://rfk.cheryme.top

[U87] JS：解构默认值
来源：http://azy.c1oappe.top

const { a = 1, b = 2 } = obj;
来源：http://weo.snrcjt.cn

[U88] JS：对象展开合并
来源：http://nyq.jqgufenzy.top

{ ...a, ...b }
来源：http://dzb.sxryk.cn

[U89] JS：数组去重
来源：http://zpk.shuidangran.top

[...new Set(arr)]
来源：http://abi.birdmap.top

[U90] JS：数字数组排序
来源：http://wxc.jlsjyb.cn

[...arr].sort((a, b) => a - b)
来源：http://mjw.zdbjq.cn

[U91] JS：对象键值遍历
来源：http://yiz.jinqigufen.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fhz.jlsjyb.cn

[U92] JS：深拷贝
来源：http://kmt.meibo888.top

structuredClone(obj)
来源：http://ghg.zhaomingkeji.xyz

[U93] JS：模板字符串
来源：http://qcv.tarul.cn

`共 ${n} 条`
来源：http://hzv.sufxvd.cn

[U94] JS：箭头函数
来源：http://oeh.zhijiandao.cn

const double = x => x * 2;
来源：http://vuo.daria6918.cn

[U95] JS：Promise 包装
来源：http://hun.daxiang520.top

new Promise((resolve, reject) => {})
来源：http://mcp.hfpthk.cn

[U96] JS：async/await 与异常
来源：http://rqn.hammf.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qcy.shanyushiyangkeji.top

[U97] JS：并发请求
来源：http://tzp.hywenlv.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://dtu.chenjidiqi.icu

[U98] JS：fetch 带 JSON
来源：http://bqt.sxryk.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ddi.ybcxt.top

[U99] JS：事件监听
来源：http://iez.hnxiangtu.top

el.addEventListener("click", e => {})
来源：http://qgt.nanxinkj.top

[U100] JS：DOM 查询
来源：http://pzt.andypj.xyz

document.querySelector(".item")
来源：http://wfx.fktsv.cn

[U101] JS：classList 操作
来源：http://bap.guannengcc.top

el.classList.toggle("active")
来源：http://rlw.bjfxy.top

[U102] JS：本地存储
来源：http://fyq.vehdjk.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://zld.yuanzhike.top

[U103] JS：定时器
来源：http://zob.hywenlv.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wij.bjfxy.top

[U104] JS：防抖
来源：http://svx.sxryk.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xuv.gogol.net.cn

[U105] JS：节流
来源：http://iig.quarkkingdee.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ndj.kuanghao11.cn

[U106] JS：日期格式化
来源：http://jut.hywenlv.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jbz.gotoacloud.top

[U107] JS：数字千分位
来源：http://kct.tianlin.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kou.fanxiaobao.xyz

[U108] JS：随机整数
来源：http://wwg.zhijiandao.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vof.snrcjt.cn

[U109] JS：数组分组
来源：http://jyd.jiagoushi.top

Object.groupBy(arr, x => x.type)
来源：http://wnq.quarkkingdee.top

[U110] JS：数组分块
来源：http://acx.daria6918.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dtk.yangfankeji.com

[U111] JS：对象转 Map
来源：http://vvw.sjlbkw.cn

new Map(Object.entries(obj))
来源：http://qpv.shzxlz.cn

[U112] JS：字符串补位
来源：http://bia.ppjwa.cn

"7".padStart(3, "0")
来源：http://pio.tanke756.top

[U113] JS：正则替换全部
来源：http://nkz.yueranfly.top

s.replaceAll("a", "b")
来源：http://ayn.zhiwuduotai.top

[U114] JS：JSON 深比较
来源：http://gql.xziqi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://qqi.tarul.cn

[U115] JS：生成 UUID
来源：http://ksw.0kj1m.cn

crypto.randomUUID()
来源：http://nfr.sweek.top

[U116] JS：类型检查（JSDoc）
来源：http://tyd.shanyushiyangkeji.top

/** @param {string} name */ function f(name) {}
来源：http://qup.tanke756.top

[U117] JS：单元测试
来源：http://oiz.jqgfzy.top

npm i -D vitest;  npx vitest
来源：http://sbl.meibo888.top

[U118] JS：开发服务器
来源：http://vjf.cqqwz.cn

npm i -D vite;  npx vite
来源：http://xse.dashuyun.cn

[U119] JS：生产构建
来源：http://odi.cucudq.cn

npx vite build
来源：http://gyp.vqdsnc.cn

[U120] JS：读取环境变量（Vite）
来源：http://stx.c1oappe.top

import.meta.env.VITE_API_URL
来源：http://ocx.jinqigfzy.top

================================================================================
来源：http://muf.cashguo.top

统计汇总
来源：http://pac.gzhubu.top

================================================================================
来源：http://roq.havefunace.top

按语言统计（条）：
来源：http://sdy.hywenlv.cn

Python ......... 252
来源：http://upy.wangdashe.top

PHP ............ 252
来源：http://wdn.tanke756.top

JavaScript ..... 252
来源：http://dyb.ehwqpu.com

TypeScript ..... 212
来源：http://bxi.xziqi.cn

Java ........... 212
来源：http://jfz.guannengcc.top

Go ............. 212
来源：http://jbw.shzxlz.cn

Ruby ........... 212
来源：http://cic.yj20258888.top

C# ............. 212
来源：http://mmz.hongshengwenyu.top

C .............. 30
来源：http://ejv.yueranfly.top

C++ ............ 30
来源：http://daz.bbcook.cn

SQL ............ 90
来源：http://zic.bbcook.cn

Bash ........... 80
来源：http://wbu.shangyingyoupin.top

Kotlin ......... 15
来源：http://dxy.fanxiaobao.xyz

Swift .......... 15
来源：http://puw.guowangkeji.top

Lua ............ 10
来源：http://pdz.mhx1999.top

Perl ........... 10
来源：http://ifj.zhongyouzk.top

Scala .......... 10
来源：http://ruc.xuanzx.com

------------------------------------
来源：http://itj.sxryk.cn

合计 ........... 2106 条
来源：http://meu.yuanzhike.top

按章节统计：
来源：http://dxr.yuanzhike.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://aru.xingfuxueyuan.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qny.smart0.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://yxm.bbcook.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://uvo.chenlongwang.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://lha.haohaochexian.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://sya.hnqzz.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ikr.iojbl.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://dad.yuanzhike.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://szo.jiagoushi.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zos.pengpengdd.cyou

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qte.andypj.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ykh.chenjidiqi.icu

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ubd.shanyushiyangtech.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rlb.meibo888.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vyk.hysaishi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vdv.ehwqpu.com

Q SQL 专题                              90
来源：http://ezl.dashuyun.cn

R Bash 专题                             80
来源：http://vte.wangdashe.top

S C / C++ 专题                          60
来源：http://iba.hnxiangtu.top

T 其他语言补充                          60
来源：http://drj.tarul.cn

U 高频实用片段                         120
来源：http://asb.52xcode.cn

------------------------------------
来源：http://vyy.jinghuilouyu.cn

合计                                  2106 条
来源：http://isi.zhiwuduotai.top

--------------------------------------------------------------------------------
来源：http://gpk.yj20258.top

使用提醒
来源：http://nhz.jinyuanbaomall.cn

--------------------------------------------------------------------------------
来源：http://odp.yj20258.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qok.yongpay.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bao.fanxiaobao.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hja.fengsongda.top

在旧版本上使用前请先确认语法支持情况。
来源：http://czr.yonumen.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://tqz.hammf.cn

—— 文件结束 ——
来源：http://bqv.316326.xyz

================================================================================
来源：http://mvi.chenlongwang.top

程序语言常见例子速查手册（2024 版）
来源：http://lns.zycfv.cn

Common Programming Examples Cheat Book
来源：http://qph.svipenyu.cn

================================================================================
来源：http://ecw.ivvv.top

【收录内容】
来源：http://wai.bjfxy.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://xer.jinghuilouyu.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ssm.ydjk.org.cn

SQL · Bash · C · C++
来源：http://wzb.9152youxi.cn


<!-- 参考信息 -->