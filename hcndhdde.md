代发 wailian999

[U13] Py：固定长度队列
来源：http://bro.pycfn.com

deque(maxlen=10)
来源：http://lrh.fzhhl.top

[U14] Py：分组收集到列表
来源：http://asn.bjfxy.top

defaultdict(list)
来源：http://dmi.xuetiantiany.cn

[U15] Py：高精度计时
来源：http://vld.tian-w.cn

t = time.perf_counter()
来源：http://qmj.guannengcc.top

[U16] Py：命令行参数解析
来源：http://xvu.52xcode.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ttk.cqqwz.cn

[U17] Py：初始化日志
来源：http://cln.shanyushiyangtech.top

logging.basicConfig(level=logging.INFO)
来源：http://opo.ppjwa.cn

[U18] Py：预编译正则
来源：http://hea.yfazqb.com

pat = re.compile(r"\d+")
来源：http://srl.fengsongda.top

[U19] Py：正则替换带回调
来源：http://ybs.wangdashe.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jve.chenlongwang.top

[U20] Py：缓存函数结果
来源：http://zrm.xuanzx.com

@functools.lru_cache(maxsize=None)
来源：http://ftp.mhx1999.top

[U21] Py：自定义上下文管理器
来源：http://vob.jiagoushi.top

@contextlib.contextmanager
来源：http://ztt.0kj1m.cn

[U22] Py：矩阵转置
来源：http://hdd.hesvh.cn

list(zip(*m))
来源：http://pty.ydzc1.top

[U23] Py：分块读取大文件
来源：http://ypm.gogol.net.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://svr.316326.xyz

[U24] Py：路径操作
来源：http://zvl.hysaishi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://yzb.feifeiyinyue.top

[U25] Py：CSV 按字典读
来源：http://swo.kuanghao11.cn

csv.DictReader(f)
来源：http://sjw.cashguo.top

[U26] Py：并发下载
来源：http://qtf.yuxming.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bwq.hywenlv.cn

[U27] Py：异步 HTTP
来源：http://eft.jinqigfzy.top

aiohttp.ClientSession() 配合 async with
来源：http://gon.ppjwa.cn

[U28] Py：类型别名
来源：http://gdw.jqgufenzy.top

UserId = int
来源：http://dlx.fehbvm.com

[U29] Py：属性校验
来源：http://wkv.daria6918.cn

@property 与 @x.setter 配合
来源：http://riw.jqgfzy.top

[U30] Py：数据类
来源：http://odd.jinyuanbaomall.cn

@dataclass(slots=True)
来源：http://skh.ydjk.org.cn

[U31] Py：单测
来源：http://kqh.redwolf501.top

python -m pytest -q
来源：http://eyw.jqgufenzy.top

[U32] Py：代码格式化
来源：http://tww.pengpengdd.cyou

ruff format . && ruff check --fix .
来源：http://arj.xylfe.cn

[U33] Py：打包发布
来源：http://wui.redwolf501.top

python -m build  （依赖 pyproject.toml）
来源：http://hoa.jiagoushi.top

[U34] Py：判断编码
来源：http://qvu.zdbjq.cn

chardet.detect(raw)
来源：http://bpz.havefunace.top

[U35] Py：发送邮件
来源：http://qcy.cdnleiting.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://oap.bjfxy.top

[U36] Py：定时任务
来源：http://tcy.wangshuangyany.cn

schedule.every(10).minutes.do(job)
来源：http://vke.316326.xyz

[U37] Py：读写 Excel
来源：http://rdv.jqgufenzy.top

pandas.read_excel / DataFrame.to_excel
来源：http://gab.feifeiyinyue.top

[U38] Py：获取脚本所在目录
来源：http://qqg.tanke756.top

Path(__file__).resolve().parent
来源：http://eil.jlsjyb.cn

[U39] Py：判断是否在交互环境
来源：http://xua.316326.xyz

sys.stdout.isatty()
来源：http://dew.ybcxt.top

[U40] Py：打印到标准错误
来源：http://aqn.cqqwz.cn

print("err", file=sys.stderr)
来源：http://mco.nwbrower.top

[U41] PHP：初始化 Composer 项目
来源：http://vnk.sysykeji.top

composer init;  composer require guzzlehttp/guzzle
来源：http://pso.jiagoushi.top

[U42] PHP：PSR-4 自动加载
来源：http://wcb.pycfn.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hgu.fktsv.cn

[U43] PHP：声明命名空间
来源：http://kuk.fanxiaobao.xyz

namespace App\Http;
来源：http://gif.fktsv.cn

[U44] PHP：开启严格类型
来源：http://yaz.uphjek.com

declare(strict_types=1);
来源：http://laj.hnxiangtu.top

[U45] PHP：类型声明与返回类型
来源：http://che.yj20258.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://znt.hysaishi.cn

[U46] PHP：可空类型
来源：http://xvt.aibaodan.cn

?string $name = null
来源：http://okc.aizwys.cn

[U47] PHP：联合类型
来源：http://uuc.nanxuanxn.top

int|string $id
来源：http://xpq.fzhhl.top

[U48] PHP：纯枚举
来源：http://ggo.yonumen.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ntz.yanxiufei.cn

[U49] PHP：只读属性
来源：http://cub.redwolf501.top

public readonly string $name
来源：http://ccr.mhx1999.top

[U50] PHP：构造器属性提升
来源：http://rmu.mhx1999.top

public function __construct(private int $id) {}
来源：http://vbt.yongpay.top

[U51] PHP：数组解构
来源：http://kfe.zhijiandao.cn

[$a, $b] = $arr;
来源：http://dcr.gogol.net.cn

[U52] PHP：箭头函数
来源：http://lmg.andypj.xyz

$double = fn($x) => $x * 2;
来源：http://agj.yj20258.top

[U53] PHP：空合并运算符
来源：http://hhn.ydzc1.top

$v = $a ?? $b ?? "default";
来源：http://jdj.vqdsnc.cn

[U54] PHP：空安全调用
来源：http://vzp.quarkkingdee.top

$obj?->method()
来源：http://cuh.hongshengwenyu.top

[U55] PHP：match 表达式
来源：http://rma.guowangkeji.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ajl.yj202588.top

[U56] PHP：命名参数
来源：http://ksh.cheryme.top

f(a: 1, b: 2)
来源：http://xif.ppjwa.cn

[U57] PHP：字符串插值
来源：http://wld.yonumen.top

"值: {$a}"
来源：http://pqq.ctjpmb.com

[U58] PHP：数组三件套
来源：http://wan.aibaodan.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://uay.0kj1m.cn

[U59] PHP：自定义排序
来源：http://yqu.shzxlz.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hws.tarul.cn

[U60] PHP：JSON 编解码
来源：http://vun.fzhhl.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mpc.yvedp.cn

[U61] PHP：正则
来源：http://rui.chenjidiqi.icu

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jcy.pycfn.com

[U62] PHP：日期对象
来源：http://jbf.sxryk.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hzu.dashuyun.cn

[U63] PHP：文件读写
来源：http://jzi.zdbjq.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xwe.cucudq.cn

[U64] PHP：目录遍历
来源：http://huh.cucudq.cn

glob("dir/*.php");  scandir("dir");
来源：http://hsq.xingfuxueyuan.xyz

[U65] PHP：会话
来源：http://inl.guowangkeji.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ayt.xylfe.cn

[U66] PHP：设置 Cookie
来源：http://csi.ydzc1.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xnf.smart0.xyz

[U67] PHP：处理文件上传
来源：http://xqc.birdmap.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mqe.fehbvm.com

[U68] PHP：PDO 连接
来源：http://kjz.yanxiufei.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xvt.gogol.net.cn

[U69] PHP：PDO 预处理
来源：http://zfy.nanxinkj.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kai.vqdsnc.cn

[U70] PHP：PDO 事务
来源：http://avr.andypj.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vbj.zycfv.cn

[U71] PHP：抛出异常
来源：http://ghx.sweek.top

throw new RuntimeException("失败", 500);
来源：http://kli.jlsjyb.cn

[U72] PHP：写错误日志
来源：http://xwo.yuanzhike.top

error_log("失败: " . $e->getMessage());
来源：http://gcx.c1oappe.top

[U73] PHP：读取 ini 配置
来源：http://oqi.hammf.cn

parse_ini_file("config.ini", true)
来源：http://toe.cqqwz.cn

[U74] PHP：读取环境变量
来源：http://vjp.fanxiaobao.xyz

getenv("APP_ENV") ?: "production"
来源：http://qgv.dashuyun.cn

[U75] PHP：依赖注入
来源：http://tvg.yvedp.cn

composer require psr/container
来源：http://tvq.ybcxt.top

[U76] PHP：简单路由
来源：http://til.shangyingyoupin.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://cwp.shangyingyoupin.top

[U77] PHP：模板渲染
来源：http://sor.yfazqb.com

composer require twig/twig
来源：http://bsn.yvedp.cn

[U78] PHP：单元测试
来源：http://ygm.sufxvd.cn

composer require --dev phpunit/phpunit
来源：http://upd.zhaomingkeji.xyz

[U79] PHP：静态分析
来源：http://gct.jinqigfzy.top

composer require --dev phpstan/phpstan
来源：http://que.hammf.cn

[U80] PHP：代码规范修复
来源：http://pbz.tanke756.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://wad.hysaishi.cn

[U81] JS：初始化项目
来源：http://qsq.fehbvm.com

npm init -y;  npm i express
来源：http://zpo.tian-w.cn

[U82] JS：package.json 脚本
来源：http://osy.vehdjk.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ewb.hammf.cn

[U83] JS：ES Module 导入导出
来源：http://mzj.yfazqb.com

export const a = 1;  import { a } from "./m.js";
来源：http://clq.0kj1m.cn

[U84] JS：CommonJS 写法
来源：http://edz.daria6918.cn

module.exports = { a };  const { a } = require("./m");
来源：http://epd.yj20258888.top

[U85] JS：可选链
来源：http://dag.xziqi.cn

a?.b?.c
来源：http://ffb.hongshengwenyu.top

[U86] JS：空值合并
来源：http://ufm.fanxiaobao.xyz

a ?? b
来源：http://kiy.xinyue.icu

[U87] JS：解构默认值
来源：http://pde.ctjpmb.com

const { a = 1, b = 2 } = obj;
来源：http://kmo.shuidangran.top

[U88] JS：对象展开合并
来源：http://dns.jqgfzy.top

{ ...a, ...b }
来源：http://xvz.gotoacloud.top

[U89] JS：数组去重
来源：http://acl.jqgfzy.top

[...new Set(arr)]
来源：http://khp.pengpengdd.cyou

[U90] JS：数字数组排序
来源：http://rre.yvedp.cn

[...arr].sort((a, b) => a - b)
来源：http://kru.fanxiaobao.xyz

[U91] JS：对象键值遍历
来源：http://rvt.jlsjyb.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zsl.nanxinkj.top

[U92] JS：深拷贝
来源：http://oyt.chenzaomai.com

structuredClone(obj)
来源：http://bfs.sweek.top

[U93] JS：模板字符串
来源：http://ygc.yuanzhike.top

`共 ${n} 条`
来源：http://kxj.fehbvm.com

[U94] JS：箭头函数
来源：http://enw.jqgfzy.top

const double = x => x * 2;
来源：http://xfb.dianchejie.cn

[U95] JS：Promise 包装
来源：http://gbg.yuxming.cn

new Promise((resolve, reject) => {})
来源：http://thx.redwolf501.top

[U96] JS：async/await 与异常
来源：http://ujq.kuanghao11.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://arl.zhiwuduotai.top

[U97] JS：并发请求
来源：http://kus.yuanzhike.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://seo.gotoacloud.top

[U98] JS：fetch 带 JSON
来源：http://iqx.pycfn.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bhm.xingfuxueyuan.xyz

[U99] JS：事件监听
来源：http://flt.sxryk.cn

el.addEventListener("click", e => {})
来源：http://zfl.daxiang520.top

[U100] JS：DOM 查询
来源：http://xrz.haohaochexian.top

document.querySelector(".item")
来源：http://udo.jinghuilouyu.cn

[U101] JS：classList 操作
来源：http://fvn.hongshengwenyu.top

el.classList.toggle("active")
来源：http://zpr.xuetiantiany.cn

[U102] JS：本地存储
来源：http://vqn.jinqigfzy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://nbr.bbcook.cn

[U103] JS：定时器
来源：http://nsh.daxiang520.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zay.ppjwa.cn

[U104] JS：防抖
来源：http://fpn.hnqzz.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ggr.ywan-chungtsiang.top

[U105] JS：节流
来源：http://xyt.feifeiyinyue.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://daa.sweek.top

[U106] JS：日期格式化
来源：http://llk.wangshuangyany.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://htt.bbcook.cn

[U107] JS：数字千分位
来源：http://pgl.yj20258888.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://isp.xylfe.cn

[U108] JS：随机整数
来源：http://whw.ivvv.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gkk.52xcode.cn

[U109] JS：数组分组
来源：http://trd.gotoacloud.top

Object.groupBy(arr, x => x.type)
来源：http://gal.shzxlz.cn

[U110] JS：数组分块
来源：http://vej.zhiwuduotai.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ccf.quarkkingdee.top

[U111] JS：对象转 Map
来源：http://hqf.chenjidiqi.icu

new Map(Object.entries(obj))
来源：http://vwi.epnwcf.com

[U112] JS：字符串补位
来源：http://nva.iojbl.cn

"7".padStart(3, "0")
来源：http://cnl.c1oappe.top

[U113] JS：正则替换全部
来源：http://auq.zhijiandao.cn

s.replaceAll("a", "b")
来源：http://lem.aizwys.cn

[U114] JS：JSON 深比较
来源：http://ryz.daria6918.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://hop.wangshuangyany.cn

[U115] JS：生成 UUID
来源：http://aqj.haohaochexian.top

crypto.randomUUID()
来源：http://gha.xuetiantiany.cn

[U116] JS：类型检查（JSDoc）
来源：http://htq.cucudq.cn

/** @param {string} name */ function f(name) {}
来源：http://xdd.hcnkem.com

[U117] JS：单元测试
来源：http://bnt.chenlongwang.top

npm i -D vitest;  npx vitest
来源：http://shw.ywan-chungtsiang.top

[U118] JS：开发服务器
来源：http://uyd.zhaomingkeji.xyz

npm i -D vite;  npx vite
来源：http://nmb.ehwqpu.com

[U119] JS：生产构建
来源：http://lru.guannengcc.top

npx vite build
来源：http://ugo.shanyushiyangkeji.top

[U120] JS：读取环境变量（Vite）
来源：http://vvw.feifeiyinyue.top

import.meta.env.VITE_API_URL
来源：http://atw.jianghu66.top

================================================================================
来源：http://rnt.zhengqikj.top

统计汇总
来源：http://kww.xziqi.cn

================================================================================
来源：http://siv.yvedp.cn

按语言统计（条）：
来源：http://yrv.cheryme.top

Python ......... 252
来源：http://ink.cdnleiting.top

PHP ............ 252
来源：http://waq.zdqjudy.top

JavaScript ..... 252
来源：http://qrl.aibaodan.cn

TypeScript ..... 212
来源：http://wsj.c1oappe.top

Java ........... 212
来源：http://dcy.zhoulong.xyz

Go ............. 212
来源：http://gyo.jinyuanbaomall.cn

Ruby ........... 212
来源：http://qki.wangdashe.top

C# ............. 212
来源：http://hsf.yj20258.top

C .............. 30
来源：http://fzu.yj20258.top

C++ ............ 30
来源：http://jra.zhengqikj.top

SQL ............ 90
来源：http://xye.zhixingplan.top

Bash ........... 80
来源：http://vbr.gotoacloud.top

Kotlin ......... 15
来源：http://lrg.vqdsnc.cn

Swift .......... 15
来源：http://eez.uphjek.com

Lua ............ 10
来源：http://lce.ybcxt.top

Perl ........... 10
来源：http://mbq.haohaochexian.top

Scala .......... 10
来源：http://bti.epnwcf.com

------------------------------------
来源：http://hzx.hywenlv.cn

合计 ........... 2106 条
来源：http://mzt.yuanzhike.top

按章节统计：
来源：http://rzl.jyoumei.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://nja.zhoulong.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wey.uphjek.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wor.jqgufenzy.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ldj.nanxuanxn.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://cux.hnxiangtu.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ujx.yj202588.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vcz.wangshuangyany.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qjm.sjlbkw.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nzo.zdqjudy.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vjf.hongshengwenyu.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ljc.jiagoushi.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vux.ivvv.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wxg.cqqwz.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://alh.sweek.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ddv.vehdjk.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rvr.cqqwz.cn

Q SQL 专题                              90
来源：http://syt.hnqzz.top

R Bash 专题                             80
来源：http://zej.guannengcc.top

S C / C++ 专题                          60
来源：http://pvm.fengsongda.top

T 其他语言补充                          60
来源：http://gvx.zdbjq.cn

U 高频实用片段                         120
来源：http://vyd.hammf.cn

------------------------------------
来源：http://nkh.pycfn.com

合计                                  2106 条
来源：http://cua.iojbl.cn

--------------------------------------------------------------------------------
来源：http://app.0kj1m.cn

使用提醒
来源：http://sjv.nanxinkj.top

--------------------------------------------------------------------------------
来源：http://dcv.ctjpmb.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wtc.sufxvd.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://yjw.cqqwz.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://nhv.haohaochexian.top

在旧版本上使用前请先确认语法支持情况。
来源：http://khf.cdnleiting.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zfx.yj202588.top

—— 文件结束 ——
来源：http://thv.jinqigfzy.top

================================================================================
来源：http://zfk.jyoumei.cn

程序语言常见例子速查手册（2024 版）
来源：http://yqn.wangdashe.top

Common Programming Examples Cheat Book
来源：http://mce.hnqzz.top

================================================================================
来源：http://jsm.shanyushiyangkeji.top

【收录内容】
来源：http://cdt.xuanzx.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://wei.fktsv.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://suh.nanxinkj.top

SQL · Bash · C · C++
来源：http://ndt.mhx1999.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jrn.iojbl.cn

【使用说明】
来源：http://afe.yanxiufei.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://jex.hnxiangtu.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://dda.vehdjk.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://lrz.zhoulong.xyz

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hca.sjlbkw.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://gmn.vqdsnc.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://utk.hnxiangtu.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ejl.shangyingyoupin.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://bpk.zhengqikj.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://tgr.gaohongyu789.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gdw.0kj1m.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hyh.zhixingplan.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://eht.zycfv.cn

【文件统计】
来源：http://ssz.sxryk.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cym.yueranfly.top

--------------------------------------------------------------------------------
来源：http://fjf.yueranfly.top

目  录
来源：http://aln.c1oappe.top

--------------------------------------------------------------------------------
来源：http://aey.zhijiandao.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://erm.vehdjk.com


<!-- 参考信息 -->