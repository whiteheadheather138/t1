代发 wailian999

[U03] Py：加载 .env 配置
来源：http://wtq.jinqigfzy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://tbf.redwolf501.top

[U04] Py：变量调试打印
来源：http://oec.jyoumei.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ujg.guannengcc.top

[U05] Py：列表去重且保序
来源：http://aok.aibaodan.cn

list(dict.fromkeys(arr))
来源：http://srp.epnwcf.com

[U06] Py：合并两个字典
来源：http://jan.dashuyun.cn

{**a, **b}
来源：http://trm.tianlin.xyz

[U07] Py：反转字典键值
来源：http://qgg.jqgufenzy.top

{v: k for k, v in d.items()}
来源：http://frs.pycfn.com

[U08] Py：展平二维列表
来源：http://lsr.jinqigfzy.top

[y for x in nested for y in x]
来源：http://ucg.jqgufenzy.top

[U09] Py：字典取最大值的键
来源：http://tsz.zhongyouzk.top

max(d, key=d.get)
来源：http://ehv.haohaochexian.top

[U10] Py：按值排序字典
来源：http://qeu.hysaishi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ozb.daria6918.cn

[U11] Py：生成器表达式
来源：http://kwf.sjlbkw.cn

(x * 2 for x in arr)
来源：http://clq.fanxiaobao.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://lnx.iojbl.cn

Counter(arr).most_common(3)
来源：http://lwd.meibo888.top

[U13] Py：固定长度队列
来源：http://sce.xuanzx.com

deque(maxlen=10)
来源：http://vay.cashguo.top

[U14] Py：分组收集到列表
来源：http://rut.chenjidiqi.icu

defaultdict(list)
来源：http://jwg.hnqzz.top

[U15] Py：高精度计时
来源：http://dyu.nwbrower.top

t = time.perf_counter()
来源：http://erf.shanyushiyangtech.top

[U16] Py：命令行参数解析
来源：http://vye.jinghuilouyu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wyx.yj20258.top

[U17] Py：初始化日志
来源：http://rsw.dianchejie.cn

logging.basicConfig(level=logging.INFO)
来源：http://etd.pengpengdd.cyou

[U18] Py：预编译正则
来源：http://nth.yangfankeji.com

pat = re.compile(r"\d+")
来源：http://mum.wangdashe.top

[U19] Py：正则替换带回调
来源：http://tgl.hammf.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cck.jinyuanbaomall.cn

[U20] Py：缓存函数结果
来源：http://vqy.shanyushiyangtech.top

@functools.lru_cache(maxsize=None)
来源：http://amg.jinqigfzy.top

[U21] Py：自定义上下文管理器
来源：http://gdv.havefunace.top

@contextlib.contextmanager
来源：http://hmm.yonumen.top

[U22] Py：矩阵转置
来源：http://hiv.hnqzz.top

list(zip(*m))
来源：http://buc.xuanzx.com

[U23] Py：分块读取大文件
来源：http://nkg.yj20258.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://twu.hnxiangtu.top

[U24] Py：路径操作
来源：http://btp.svipenyu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gvb.jinghuilouyu.cn

[U25] Py：CSV 按字典读
来源：http://kvz.gotoacloud.top

csv.DictReader(f)
来源：http://jvf.xinyue.icu

[U26] Py：并发下载
来源：http://uqs.0kj1m.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ihj.jyoumei.cn

[U27] Py：异步 HTTP
来源：http://dap.jinqigufen.top

aiohttp.ClientSession() 配合 async with
来源：http://jdh.vehdjk.com

[U28] Py：类型别名
来源：http://jwp.fehbvm.com

UserId = int
来源：http://qoj.ctjpmb.com

[U29] Py：属性校验
来源：http://yfw.zhaomingkeji.xyz

@property 与 @x.setter 配合
来源：http://iqo.tianlin.xyz

[U30] Py：数据类
来源：http://lay.tian-w.cn

@dataclass(slots=True)
来源：http://ueo.guowangkeji.top

[U31] Py：单测
来源：http://van.jinqigfzy.top

python -m pytest -q
来源：http://uxj.wangshuangyany.cn

[U32] Py：代码格式化
来源：http://qqj.wangdashe.top

ruff format . && ruff check --fix .
来源：http://slh.sufxvd.cn

[U33] Py：打包发布
来源：http://svt.cashguo.top

python -m build  （依赖 pyproject.toml）
来源：http://frc.hysaishi.cn

[U34] Py：判断编码
来源：http://hbu.yuxming.cn

chardet.detect(raw)
来源：http://kho.shuidangran.top

[U35] Py：发送邮件
来源：http://fmf.ydzc1.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vim.bjfxy.top

[U36] Py：定时任务
来源：http://uxx.zhiwuduotai.top

schedule.every(10).minutes.do(job)
来源：http://tjm.ywan-chungtsiang.top

[U37] Py：读写 Excel
来源：http://yym.gaohongyu789.top

pandas.read_excel / DataFrame.to_excel
来源：http://faw.ybcxt.top

[U38] Py：获取脚本所在目录
来源：http://jsu.xziqi.cn

Path(__file__).resolve().parent
来源：http://ldi.hywenlv.cn

[U39] Py：判断是否在交互环境
来源：http://loe.yongpay.top

sys.stdout.isatty()
来源：http://nay.tarul.cn

[U40] Py：打印到标准错误
来源：http://ocn.yvedp.cn

print("err", file=sys.stderr)
来源：http://lfv.meibo888.top

[U41] PHP：初始化 Composer 项目
来源：http://bdr.chenzaomai.com

composer init;  composer require guzzlehttp/guzzle
来源：http://ivc.zhijiandao.cn

[U42] PHP：PSR-4 自动加载
来源：http://ryp.zhijiandao.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://srg.hongshengwenyu.top

[U43] PHP：声明命名空间
来源：http://giw.guowangkeji.top

namespace App\Http;
来源：http://mdn.aizwys.cn

[U44] PHP：开启严格类型
来源：http://dtf.sysykeji.top

declare(strict_types=1);
来源：http://pja.smart0.xyz

[U45] PHP：类型声明与返回类型
来源：http://qzv.ppjwa.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://axk.cashguo.top

[U46] PHP：可空类型
来源：http://bku.zhiwuduotai.top

?string $name = null
来源：http://soj.c1oappe.top

[U47] PHP：联合类型
来源：http://apq.jinyuanbaomall.cn

int|string $id
来源：http://zhw.jlsjyb.cn

[U48] PHP：纯枚举
来源：http://akp.yanxiufei.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ypx.c1oappe.top

[U49] PHP：只读属性
来源：http://fxd.sjlbkw.cn

public readonly string $name
来源：http://phi.yj202588.top

[U50] PHP：构造器属性提升
来源：http://eyh.zhoulong.xyz

public function __construct(private int $id) {}
来源：http://vzv.9152youxi.cn

[U51] PHP：数组解构
来源：http://huh.hywenlv.cn

[$a, $b] = $arr;
来源：http://jqn.jinqigfzy.top

[U52] PHP：箭头函数
来源：http://hkp.chenlongwang.top

$double = fn($x) => $x * 2;
来源：http://cps.meibo888.top

[U53] PHP：空合并运算符
来源：http://pyj.chenzaomai.com

$v = $a ?? $b ?? "default";
来源：http://vpr.wangdashe.top

[U54] PHP：空安全调用
来源：http://jjo.hesvh.cn

$obj?->method()
来源：http://nvg.zdbjq.cn

[U55] PHP：match 表达式
来源：http://elh.gogol.net.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://abs.mhx1999.top

[U56] PHP：命名参数
来源：http://wcp.shzxlz.cn

f(a: 1, b: 2)
来源：http://zwc.yonumen.top

[U57] PHP：字符串插值
来源：http://nus.bbcook.cn

"值: {$a}"
来源：http://leh.yfazqb.com

[U58] PHP：数组三件套
来源：http://twk.dianchejie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://oyq.xylfe.cn

[U59] PHP：自定义排序
来源：http://dmm.jqgufenzy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://umf.yvedp.cn

[U60] PHP：JSON 编解码
来源：http://hdl.yanxiufei.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://puh.kuanghao11.cn

[U61] PHP：正则
来源：http://oxi.smart0.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://czn.cqqwz.cn

[U62] PHP：日期对象
来源：http://mrk.cheryme.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://yup.smart0.xyz

[U63] PHP：文件读写
来源：http://zcm.sjlbkw.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qsl.iojbl.cn

[U64] PHP：目录遍历
来源：http://dtu.svipenyu.cn

glob("dir/*.php");  scandir("dir");
来源：http://pkf.hesvh.cn

[U65] PHP：会话
来源：http://nup.xylfe.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://mrb.yanxiufei.cn

[U66] PHP：设置 Cookie
来源：http://vkk.52xcode.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://upm.yfazqb.com

[U67] PHP：处理文件上传
来源：http://vut.xuanzx.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fhg.52xcode.cn

[U68] PHP：PDO 连接
来源：http://wkr.jinqigfzy.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ubi.sufxvd.cn

[U69] PHP：PDO 预处理
来源：http://yng.yanxiufei.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ncr.gaohongyu789.top

[U70] PHP：PDO 事务
来源：http://eoy.yongpay.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vbb.aizwys.cn

[U71] PHP：抛出异常
来源：http://czw.yangfankeji.com

throw new RuntimeException("失败", 500);
来源：http://whg.tanke756.top

[U72] PHP：写错误日志
来源：http://gtw.wangshuangyany.cn

error_log("失败: " . $e->getMessage());
来源：http://hks.jinqigufen.top

[U73] PHP：读取 ini 配置
来源：http://vgt.fehbvm.com

parse_ini_file("config.ini", true)
来源：http://grw.cheryme.top

[U74] PHP：读取环境变量
来源：http://fzc.jqgfzy.top

getenv("APP_ENV") ?: "production"
来源：http://ydj.cashguo.top

[U75] PHP：依赖注入
来源：http://qnm.birdmap.top

composer require psr/container
来源：http://pte.xuetiantiany.cn

[U76] PHP：简单路由
来源：http://nic.jinqigufen.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://sjy.cashguo.top

[U77] PHP：模板渲染
来源：http://akz.ydzc1.top

composer require twig/twig
来源：http://thm.quarkkingdee.top

[U78] PHP：单元测试
来源：http://fuv.sysykeji.top

composer require --dev phpunit/phpunit
来源：http://cip.havefunace.top

[U79] PHP：静态分析
来源：http://akq.fktsv.cn

composer require --dev phpstan/phpstan
来源：http://yde.zhiwuduotai.top

[U80] PHP：代码规范修复
来源：http://cmx.jinqigfzy.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://twy.jlsjyb.cn

[U81] JS：初始化项目
来源：http://mqt.tarul.cn

npm init -y;  npm i express
来源：http://tzv.vehdjk.com

[U82] JS：package.json 脚本
来源：http://ras.chenlongwang.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gou.yfazqb.com

[U83] JS：ES Module 导入导出
来源：http://jhx.sysykeji.top

export const a = 1;  import { a } from "./m.js";
来源：http://uyo.pengpengdd.cyou

[U84] JS：CommonJS 写法
来源：http://ssp.hesvh.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ndu.yj202588.top

[U85] JS：可选链
来源：http://yas.yonumen.top

a?.b?.c
来源：http://qss.sufxvd.cn

[U86] JS：空值合并
来源：http://qfo.snrcjt.cn

a ?? b
来源：http://icm.fanxiaobao.xyz

[U87] JS：解构默认值
来源：http://bzy.xinyue.icu

const { a = 1, b = 2 } = obj;
来源：http://led.ivvv.top

[U88] JS：对象展开合并
来源：http://wdb.havefunace.top

{ ...a, ...b }
来源：http://srz.ydzc1.top

[U89] JS：数组去重
来源：http://ipl.ywan-chungtsiang.top

[...new Set(arr)]
来源：http://kwq.guannengcc.top

[U90] JS：数字数组排序
来源：http://xcv.shanyushiyangtech.top

[...arr].sort((a, b) => a - b)
来源：http://wnh.andypj.xyz

[U91] JS：对象键值遍历
来源：http://qbo.c1oappe.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dgk.snrcjt.cn

[U92] JS：深拷贝
来源：http://wux.uphjek.com

structuredClone(obj)
来源：http://oig.sjlbkw.cn

[U93] JS：模板字符串
来源：http://fmq.wangshuangyany.cn

`共 ${n} 条`
来源：http://ryi.aibaodan.cn

[U94] JS：箭头函数
来源：http://ynt.zhoulong.xyz

const double = x => x * 2;
来源：http://cez.zhijiandao.cn

[U95] JS：Promise 包装
来源：http://tzu.zhoulong.xyz

new Promise((resolve, reject) => {})
来源：http://qtb.jinyuanbaomall.cn

[U96] JS：async/await 与异常
来源：http://aaa.zdbjq.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nvt.jiagoushi.top

[U97] JS：并发请求
来源：http://aak.zhaomingkeji.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://rkh.daria6918.cn

[U98] JS：fetch 带 JSON
来源：http://bhj.yueranfly.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nxy.hfpthk.cn

[U99] JS：事件监听
来源：http://dwf.smart0.xyz

el.addEventListener("click", e => {})
来源：http://juk.wangshuangyany.cn

[U100] JS：DOM 查询
来源：http://bgs.yj20258.top

document.querySelector(".item")
来源：http://ypd.52xcode.cn

[U101] JS：classList 操作
来源：http://sej.yangfankeji.com

el.classList.toggle("active")
来源：http://xrt.daxiang520.top

[U102] JS：本地存储
来源：http://ahw.smart0.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://axd.sufxvd.cn

[U103] JS：定时器
来源：http://xsc.cashguo.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://auf.bjfxy.top

[U104] JS：防抖
来源：http://dlr.yj20258.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yqx.52xcode.cn

[U105] JS：节流
来源：http://vsr.zhaomingkeji.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://uqi.jiagoushi.top

[U106] JS：日期格式化
来源：http://jww.iojbl.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://uba.jyoumei.cn

[U107] JS：数字千分位
来源：http://bcz.shanyushiyangkeji.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ays.havefunace.top

[U108] JS：随机整数
来源：http://szt.guowangkeji.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://avn.hfpthk.cn

[U109] JS：数组分组
来源：http://dvb.tianlin.xyz

Object.groupBy(arr, x => x.type)
来源：http://fmg.yj202588.top

[U110] JS：数组分块
来源：http://nxu.yj20258.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://csf.ydzc1.top

[U111] JS：对象转 Map
来源：http://rnm.sxryk.cn

new Map(Object.entries(obj))
来源：http://wwt.uphjek.com

[U112] JS：字符串补位
来源：http://hmk.aibaodan.cn

"7".padStart(3, "0")
来源：http://dsu.zhixingplan.top

[U113] JS：正则替换全部
来源：http://zmv.zhijiandao.cn

s.replaceAll("a", "b")
来源：http://wvi.ydzc1.top

[U114] JS：JSON 深比较
来源：http://tnz.fanxiaobao.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://nod.ybcxt.top

[U115] JS：生成 UUID
来源：http://chr.vqdsnc.cn

crypto.randomUUID()
来源：http://ukx.yj20258.top

[U116] JS：类型检查（JSDoc）
来源：http://uop.nanxuanxn.top

/** @param {string} name */ function f(name) {}
来源：http://yhg.fktsv.cn

[U117] JS：单元测试
来源：http://wun.shanyushiyangkeji.top

npm i -D vitest;  npx vitest
来源：http://daf.sweek.top

[U118] JS：开发服务器
来源：http://dul.fanxiaobao.xyz

npm i -D vite;  npx vite
来源：http://qax.quarkkingdee.top

[U119] JS：生产构建
来源：http://gsg.hywenlv.cn

npx vite build
来源：http://hsf.vehdjk.com

[U120] JS：读取环境变量（Vite）
来源：http://nob.cdnleiting.top

import.meta.env.VITE_API_URL
来源：http://zhc.gzhubu.top

================================================================================
来源：http://kjz.cdnleiting.top

统计汇总
来源：http://whg.quarkkingdee.top

================================================================================
来源：http://hra.zhijiandao.cn

按语言统计（条）：
来源：http://wzf.yangfankeji.com

Python ......... 252
来源：http://lgg.jinqigufen.top

PHP ............ 252
来源：http://rzy.tarul.cn

JavaScript ..... 252
来源：http://pqu.xylfe.cn

TypeScript ..... 212
来源：http://jhs.smart0.xyz

Java ........... 212
来源：http://axn.zhengqikj.top

Go ............. 212
来源：http://riv.yonumen.top

Ruby ........... 212
来源：http://qui.shzxlz.cn

C# ............. 212
来源：http://jor.sweek.top

C .............. 30
来源：http://dcm.ehwqpu.com

C++ ............ 30
来源：http://arw.zhixingplan.top

SQL ............ 90
来源：http://ouz.hywenlv.cn

Bash ........... 80
来源：http://dlx.zdbjq.cn

Kotlin ......... 15
来源：http://dox.hywenlv.cn

Swift .......... 15
来源：http://sez.fzhhl.top

Lua ............ 10
来源：http://xqc.zhaomingkeji.xyz

Perl ........... 10
来源：http://egz.zhixingplan.top

Scala .......... 10
来源：http://myw.zhixingplan.top

------------------------------------
来源：http://nzf.yuanzhike.top

合计 ........... 2106 条
来源：http://iqm.ivvv.top

按章节统计：
来源：http://kad.fanxiaobao.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bhr.guowangkeji.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://cyq.redwolf501.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://etn.snrcjt.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://uml.gogol.net.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ekz.jinqigfzy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hli.ppjwa.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mrj.tian-w.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ecy.quarkkingdee.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rwh.yj202588.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://beb.jlsjyb.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jwd.ydzc1.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xyu.hysaishi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://sfs.yongpay.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://nin.tian-w.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bvr.zdbjq.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ufw.zycfv.cn

Q SQL 专题                              90
来源：http://tmt.fzhhl.top

R Bash 专题                             80
来源：http://vnl.jlsjyb.cn

S C / C++ 专题                          60
来源：http://jiy.jinqigufen.top

T 其他语言补充                          60
来源：http://vko.daria6918.cn

U 高频实用片段                         120
来源：http://auy.yj20258.top

------------------------------------
来源：http://qlh.hnqzz.top

合计                                  2106 条
来源：http://quw.hongshengwenyu.top

--------------------------------------------------------------------------------
来源：http://hhx.snrcjt.cn

使用提醒
来源：http://prw.jinghuilouyu.cn

--------------------------------------------------------------------------------
来源：http://tbs.shzxlz.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://cae.ybcxt.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jbu.sjlbkw.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://itf.ehwqpu.com

在旧版本上使用前请先确认语法支持情况。
来源：http://dkd.bbcook.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hcp.tian-w.cn

—— 文件结束 ——
来源：http://oug.ydzc1.top

================================================================================
来源：http://luq.zhixingplan.top

程序语言常见例子速查手册（2024 版）
来源：http://yrj.uphjek.com

Common Programming Examples Cheat Book
来源：http://fwp.xylfe.cn

================================================================================
来源：http://gly.zhongyouzk.top

【收录内容】
来源：http://qnx.birdmap.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ibz.hfpthk.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://scv.pycfn.com

SQL · Bash · C · C++
来源：http://qyp.vqdsnc.cn


<!-- 参考信息 -->