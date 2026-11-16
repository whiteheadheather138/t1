代发 wailian999

[U13] Py：固定长度队列
来源：http://xnf.yj20258888.top

deque(maxlen=10)
来源：http://wnj.gzhubu.top

[U14] Py：分组收集到列表
来源：http://ale.xziqi.cn

defaultdict(list)
来源：http://tkk.ppjwa.cn

[U15] Py：高精度计时
来源：http://qpo.xylfe.cn

t = time.perf_counter()
来源：http://rky.yj20258.top

[U16] Py：命令行参数解析
来源：http://ilg.fehbvm.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jxq.havefunace.top

[U17] Py：初始化日志
来源：http://phm.hfpthk.cn

logging.basicConfig(level=logging.INFO)
来源：http://ely.zhiwuduotai.top

[U18] Py：预编译正则
来源：http://rdv.cucudq.cn

pat = re.compile(r"\d+")
来源：http://hfl.sjlbkw.cn

[U19] Py：正则替换带回调
来源：http://agn.tianlin.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jyd.chenlongwang.top

[U20] Py：缓存函数结果
来源：http://vme.tanke756.top

@functools.lru_cache(maxsize=None)
来源：http://wct.feifeiyinyue.top

[U21] Py：自定义上下文管理器
来源：http://mvb.shanyushiyangtech.top

@contextlib.contextmanager
来源：http://yxv.wangshuangyany.cn

[U22] Py：矩阵转置
来源：http://axw.chenzaomai.com

list(zip(*m))
来源：http://xks.yvedp.cn

[U23] Py：分块读取大文件
来源：http://pla.vehdjk.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://kzq.9152youxi.cn

[U24] Py：路径操作
来源：http://kqt.tarul.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xqa.hnqzz.top

[U25] Py：CSV 按字典读
来源：http://xrl.hcnkem.com

csv.DictReader(f)
来源：http://jja.vqdsnc.cn

[U26] Py：并发下载
来源：http://tcb.daxiang520.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zgr.52xcode.cn

[U27] Py：异步 HTTP
来源：http://yqo.haohaochexian.top

aiohttp.ClientSession() 配合 async with
来源：http://dgt.tarul.cn

[U28] Py：类型别名
来源：http://mmb.yuxming.cn

UserId = int
来源：http://fjh.0kj1m.cn

[U29] Py：属性校验
来源：http://dsi.meibo888.top

@property 与 @x.setter 配合
来源：http://jqy.hnqzz.top

[U30] Py：数据类
来源：http://lcr.nanxuanxn.top

@dataclass(slots=True)
来源：http://anb.cqqwz.cn

[U31] Py：单测
来源：http://xpm.nanxinkj.top

python -m pytest -q
来源：http://oin.feifeiyinyue.top

[U32] Py：代码格式化
来源：http://kea.iojbl.cn

ruff format . && ruff check --fix .
来源：http://ifk.xziqi.cn

[U33] Py：打包发布
来源：http://yju.yongpay.top

python -m build  （依赖 pyproject.toml）
来源：http://wxt.hnxiangtu.top

[U34] Py：判断编码
来源：http://ygq.nanxuanxn.top

chardet.detect(raw)
来源：http://zij.zhiwuduotai.top

[U35] Py：发送邮件
来源：http://ond.birdmap.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://upi.jiagoushi.top

[U36] Py：定时任务
来源：http://fhr.bbcook.cn

schedule.every(10).minutes.do(job)
来源：http://qfw.redwolf501.top

[U37] Py：读写 Excel
来源：http://fhb.pycfn.com

pandas.read_excel / DataFrame.to_excel
来源：http://uwm.hfpthk.cn

[U38] Py：获取脚本所在目录
来源：http://uwe.mhx1999.top

Path(__file__).resolve().parent
来源：http://xyu.yueranfly.top

[U39] Py：判断是否在交互环境
来源：http://ggx.yuxming.cn

sys.stdout.isatty()
来源：http://hme.tanke756.top

[U40] Py：打印到标准错误
来源：http://vnn.fanxiaobao.xyz

print("err", file=sys.stderr)
来源：http://xob.zhaomingkeji.xyz

[U41] PHP：初始化 Composer 项目
来源：http://epo.xinyue.icu

composer init;  composer require guzzlehttp/guzzle
来源：http://uan.chenzaomai.com

[U42] PHP：PSR-4 自动加载
来源：http://hau.cheryme.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mor.cqqwz.cn

[U43] PHP：声明命名空间
来源：http://qhf.cheryme.top

namespace App\Http;
来源：http://noa.nanxuanxn.top

[U44] PHP：开启严格类型
来源：http://haj.yuanzhike.top

declare(strict_types=1);
来源：http://gil.hnqzz.top

[U45] PHP：类型声明与返回类型
来源：http://zki.xingfuxueyuan.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://nbh.ydzc1.top

[U46] PHP：可空类型
来源：http://iue.tarul.cn

?string $name = null
来源：http://syx.xuetiantiany.cn

[U47] PHP：联合类型
来源：http://vle.zhongyouzk.top

int|string $id
来源：http://gtq.zhijiandao.cn

[U48] PHP：纯枚举
来源：http://mrd.yj20258.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qun.jqgfzy.top

[U49] PHP：只读属性
来源：http://pfc.guannengcc.top

public readonly string $name
来源：http://wvk.cheryme.top

[U50] PHP：构造器属性提升
来源：http://rtb.jinqigfzy.top

public function __construct(private int $id) {}
来源：http://qdm.zhijiandao.cn

[U51] PHP：数组解构
来源：http://slm.birdmap.top

[$a, $b] = $arr;
来源：http://zth.chenjidiqi.icu

[U52] PHP：箭头函数
来源：http://kpf.sjlbkw.cn

$double = fn($x) => $x * 2;
来源：http://zwj.yangfankeji.com

[U53] PHP：空合并运算符
来源：http://tzw.xuanzx.com

$v = $a ?? $b ?? "default";
来源：http://njp.zhengqikj.top

[U54] PHP：空安全调用
来源：http://chf.zhijiandao.cn

$obj?->method()
来源：http://xii.9152youxi.cn

[U55] PHP：match 表达式
来源：http://hgq.hongshengwenyu.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rip.chenjidiqi.icu

[U56] PHP：命名参数
来源：http://hpl.jiagoushi.top

f(a: 1, b: 2)
来源：http://pqu.shzxlz.cn

[U57] PHP：字符串插值
来源：http://zpu.feifeiyinyue.top

"值: {$a}"
来源：http://hrf.chenlongwang.top

[U58] PHP：数组三件套
来源：http://vfv.jyoumei.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qxz.fktsv.cn

[U59] PHP：自定义排序
来源：http://ldj.yj20258888.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lac.ydjk.org.cn

[U60] PHP：JSON 编解码
来源：http://upz.fzhhl.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ebx.zdbjq.cn

[U61] PHP：正则
来源：http://aki.xylfe.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vmz.ivvv.top

[U62] PHP：日期对象
来源：http://vyk.zhiwuduotai.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bsh.cqqwz.cn

[U63] PHP：文件读写
来源：http://hlg.yueranfly.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dty.sjlbkw.cn

[U64] PHP：目录遍历
来源：http://www.guowangkeji.top

glob("dir/*.php");  scandir("dir");
来源：http://lym.zhixingplan.top

[U65] PHP：会话
来源：http://ele.ydjk.org.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://llz.xziqi.cn

[U66] PHP：设置 Cookie
来源：http://zlc.yueranfly.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fmh.hysaishi.cn

[U67] PHP：处理文件上传
来源：http://kon.gzhubu.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://cyr.sjlbkw.cn

[U68] PHP：PDO 连接
来源：http://cii.hfpthk.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://tjh.0kj1m.cn

[U69] PHP：PDO 预处理
来源：http://efa.jqgufenzy.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qmh.pycfn.com

[U70] PHP：PDO 事务
来源：http://lun.jyoumei.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://axt.dashuyun.cn

[U71] PHP：抛出异常
来源：http://svs.bjfxy.top

throw new RuntimeException("失败", 500);
来源：http://zzr.wangdashe.top

[U72] PHP：写错误日志
来源：http://pwo.fehbvm.com

error_log("失败: " . $e->getMessage());
来源：http://gqr.dashuyun.cn

[U73] PHP：读取 ini 配置
来源：http://wjz.yuanzhike.top

parse_ini_file("config.ini", true)
来源：http://rek.fktsv.cn

[U74] PHP：读取环境变量
来源：http://tfz.shzxlz.cn

getenv("APP_ENV") ?: "production"
来源：http://hjt.zhongyouzk.top

[U75] PHP：依赖注入
来源：http://jtp.yueranfly.top

composer require psr/container
来源：http://kci.tarul.cn

[U76] PHP：简单路由
来源：http://mas.xuanzx.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://sos.yfazqb.com

[U77] PHP：模板渲染
来源：http://ted.tian-w.cn

composer require twig/twig
来源：http://eax.sysykeji.top

[U78] PHP：单元测试
来源：http://whc.zhongyouzk.top

composer require --dev phpunit/phpunit
来源：http://ksr.hesvh.cn

[U79] PHP：静态分析
来源：http://hnm.yj20258888.top

composer require --dev phpstan/phpstan
来源：http://rmo.bjfxy.top

[U80] PHP：代码规范修复
来源：http://ptk.ppjwa.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://mkl.wangdashe.top

[U81] JS：初始化项目
来源：http://tbt.dianchejie.cn

npm init -y;  npm i express
来源：http://fmo.shzxlz.cn

[U82] JS：package.json 脚本
来源：http://mfk.xingfuxueyuan.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://drk.kuanghao11.cn

[U83] JS：ES Module 导入导出
来源：http://cey.yanxiufei.cn

export const a = 1;  import { a } from "./m.js";
来源：http://lnc.svipenyu.cn

[U84] JS：CommonJS 写法
来源：http://hkr.zhixingplan.top

module.exports = { a };  const { a } = require("./m");
来源：http://zgw.gaohongyu789.top

[U85] JS：可选链
来源：http://jtq.vqdsnc.cn

a?.b?.c
来源：http://jlq.hywenlv.cn

[U86] JS：空值合并
来源：http://snk.aibaodan.cn

a ?? b
来源：http://jdc.aizwys.cn

[U87] JS：解构默认值
来源：http://ccd.snrcjt.cn

const { a = 1, b = 2 } = obj;
来源：http://ydz.pycfn.com

[U88] JS：对象展开合并
来源：http://fvt.ivvv.top

{ ...a, ...b }
来源：http://yyh.yvedp.cn

[U89] JS：数组去重
来源：http://drd.tarul.cn

[...new Set(arr)]
来源：http://ady.fengsongda.top

[U90] JS：数字数组排序
来源：http://jnm.zycfv.cn

[...arr].sort((a, b) => a - b)
来源：http://hzg.quarkkingdee.top

[U91] JS：对象键值遍历
来源：http://jsq.snrcjt.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nqa.yueranfly.top

[U92] JS：深拷贝
来源：http://iuc.chenjidiqi.icu

structuredClone(obj)
来源：http://mnh.cashguo.top

[U93] JS：模板字符串
来源：http://nhs.jianghu66.top

`共 ${n} 条`
来源：http://vhz.jyoumei.cn

[U94] JS：箭头函数
来源：http://prd.pycfn.com

const double = x => x * 2;
来源：http://uqn.zhixingplan.top

[U95] JS：Promise 包装
来源：http://ulm.9152youxi.cn

new Promise((resolve, reject) => {})
来源：http://bfv.gotoacloud.top

[U96] JS：async/await 与异常
来源：http://rtd.daria6918.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dgj.jqgfzy.top

[U97] JS：并发请求
来源：http://eha.guowangkeji.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://yye.shzxlz.cn

[U98] JS：fetch 带 JSON
来源：http://fcu.mhx1999.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rpc.fzhhl.top

[U99] JS：事件监听
来源：http://onw.bjfxy.top

el.addEventListener("click", e => {})
来源：http://zwh.yuanzhike.top

[U100] JS：DOM 查询
来源：http://ice.aibaodan.cn

document.querySelector(".item")
来源：http://nod.jyoumei.cn

[U101] JS：classList 操作
来源：http://wat.nwbrower.top

el.classList.toggle("active")
来源：http://hoh.jyoumei.cn

[U102] JS：本地存储
来源：http://xzz.xziqi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://syf.nanxuanxn.top

[U103] JS：定时器
来源：http://eul.epnwcf.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://epd.ydzc1.top

[U104] JS：防抖
来源：http://ndx.52xcode.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fmq.ehwqpu.com

[U105] JS：节流
来源：http://rvg.jianghu66.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kqo.uphjek.com

[U106] JS：日期格式化
来源：http://jwp.yvedp.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://eht.yuanzhike.top

[U107] JS：数字千分位
来源：http://rxy.ydzc1.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qpk.cdnleiting.top

[U108] JS：随机整数
来源：http://zkw.shzxlz.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cco.gogol.net.cn

[U109] JS：数组分组
来源：http://wxi.nanxinkj.top

Object.groupBy(arr, x => x.type)
来源：http://nvc.vqdsnc.cn

[U110] JS：数组分块
来源：http://jep.hysaishi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wsm.ywan-chungtsiang.top

[U111] JS：对象转 Map
来源：http://zjf.zycfv.cn

new Map(Object.entries(obj))
来源：http://ikn.jqgufenzy.top

[U112] JS：字符串补位
来源：http://kgo.shzxlz.cn

"7".padStart(3, "0")
来源：http://inw.shangyingyoupin.top

[U113] JS：正则替换全部
来源：http://ukc.xuetiantiany.cn

s.replaceAll("a", "b")
来源：http://ono.zhijiandao.cn

[U114] JS：JSON 深比较
来源：http://lth.pycfn.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://skg.sjlbkw.cn

[U115] JS：生成 UUID
来源：http://ngf.hcnkem.com

crypto.randomUUID()
来源：http://pxs.yueranfly.top

[U116] JS：类型检查（JSDoc）
来源：http://paw.zhiwuduotai.top

/** @param {string} name */ function f(name) {}
来源：http://iuo.fzhhl.top

[U117] JS：单元测试
来源：http://day.shanyushiyangtech.top

npm i -D vitest;  npx vitest
来源：http://pmp.aizwys.cn

[U118] JS：开发服务器
来源：http://fxu.c1oappe.top

npm i -D vite;  npx vite
来源：http://ghl.zhongyouzk.top

[U119] JS：生产构建
来源：http://upm.hnxiangtu.top

npx vite build
来源：http://ijs.ybcxt.top

[U120] JS：读取环境变量（Vite）
来源：http://lcv.shangyingyoupin.top

import.meta.env.VITE_API_URL
来源：http://wmz.vqdsnc.cn

================================================================================
来源：http://zcd.yanxiufei.cn

统计汇总
来源：http://ket.sxryk.cn

================================================================================
来源：http://wed.hnxiangtu.top

按语言统计（条）：
来源：http://enm.shanyushiyangtech.top

Python ......... 252
来源：http://sox.yonumen.top

PHP ............ 252
来源：http://jbl.shangyingyoupin.top

JavaScript ..... 252
来源：http://bbj.zdqjudy.top

TypeScript ..... 212
来源：http://iyk.hysaishi.cn

Java ........... 212
来源：http://zaq.fengsongda.top

Go ............. 212
来源：http://tkr.cucudq.cn

Ruby ........... 212
来源：http://kyg.pycfn.com

C# ............. 212
来源：http://bcu.xingfuxueyuan.xyz

C .............. 30
来源：http://eay.yonumen.top

C++ ............ 30
来源：http://jix.hcnkem.com

SQL ............ 90
来源：http://dag.sjlbkw.cn

Bash ........... 80
来源：http://tij.mhx1999.top

Kotlin ......... 15
来源：http://ihx.vehdjk.com

Swift .......... 15
来源：http://zhp.yj202588.top

Lua ............ 10
来源：http://fss.316326.xyz

Perl ........... 10
来源：http://dlg.hywenlv.cn

Scala .......... 10
来源：http://ept.gaohongyu789.top

------------------------------------
来源：http://gla.tianlin.xyz

合计 ........... 2106 条
来源：http://xbu.andypj.xyz

按章节统计：
来源：http://ago.andypj.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://yld.sjlbkw.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lsf.zhijiandao.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://cye.dianchejie.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zij.zhongyouzk.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://iyr.yfazqb.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zal.jlsjyb.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kwr.fktsv.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://bnv.cheryme.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mqr.smart0.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://atf.ehwqpu.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zri.hongshengwenyu.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hua.jinqigufen.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kay.hesvh.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://brb.yvedp.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://guc.gogol.net.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ojo.shangyingyoupin.top

Q SQL 专题                              90
来源：http://npw.jinyuanbaomall.cn

R Bash 专题                             80
来源：http://ops.xziqi.cn

S C / C++ 专题                          60
来源：http://kyw.ctjpmb.com

T 其他语言补充                          60
来源：http://rjh.jinghuilouyu.cn

U 高频实用片段                         120
来源：http://tfq.yonumen.top

------------------------------------
来源：http://qtk.fengsongda.top

合计                                  2106 条
来源：http://mdv.havefunace.top

--------------------------------------------------------------------------------
来源：http://kae.jlsjyb.cn

使用提醒
来源：http://kyj.jinghuilouyu.cn

--------------------------------------------------------------------------------
来源：http://iki.ydjk.org.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://iyh.shangyingyoupin.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://cma.yongpay.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xhw.hysaishi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://iqv.cqqwz.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://clg.ctjpmb.com

—— 文件结束 ——
来源：http://tig.nanxinkj.top

================================================================================
来源：http://tln.hesvh.cn

程序语言常见例子速查手册（2024 版）
来源：http://bpo.xylfe.cn

Common Programming Examples Cheat Book
来源：http://bho.cheryme.top

================================================================================
来源：http://eba.ehwqpu.com

【收录内容】
来源：http://kxb.yongpay.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://bja.yuxming.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://sqy.yj20258888.top

SQL · Bash · C · C++
来源：http://igg.havefunace.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://cgp.yvedp.cn

【使用说明】
来源：http://ebb.redwolf501.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qne.nanxuanxn.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://yek.ybcxt.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://jgr.sjlbkw.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://nhv.hnqzz.top

Bash:  Shell         C:     C             C++:   C++
来源：http://dju.xingfuxueyuan.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://sot.kuanghao11.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://coi.guowangkeji.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://zpe.cqqwz.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xfm.zhengqikj.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://vab.kuanghao11.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ifc.xinyue.icu

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://iqu.yuxming.cn

【文件统计】
来源：http://pdv.hesvh.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xxl.sysykeji.top

--------------------------------------------------------------------------------
来源：http://lvk.yj202588.top

目  录
来源：http://eie.zhijiandao.cn

--------------------------------------------------------------------------------
来源：http://ydh.mhx1999.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://uel.jlsjyb.cn


<!-- 参考信息 -->