代发 wailian999

[U03] Py：加载 .env 配置
来源：http://wtl.aibaodan.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://yrx.vehdjk.com

[U04] Py：变量调试打印
来源：http://eks.yongpay.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ogb.ybcxt.top

[U05] Py：列表去重且保序
来源：http://vgm.shanyushiyangkeji.top

list(dict.fromkeys(arr))
来源：http://yuz.fzhhl.top

[U06] Py：合并两个字典
来源：http://atv.guowangkeji.top

{**a, **b}
来源：http://ams.jianghu66.top

[U07] Py：反转字典键值
来源：http://eyw.jinqigufen.top

{v: k for k, v in d.items()}
来源：http://opc.kuanghao11.cn

[U08] Py：展平二维列表
来源：http://ufo.ppjwa.cn

[y for x in nested for y in x]
来源：http://oac.gaohongyu789.top

[U09] Py：字典取最大值的键
来源：http://pbz.gogol.net.cn

max(d, key=d.get)
来源：http://ezd.guowangkeji.top

[U10] Py：按值排序字典
来源：http://dbg.hysaishi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lsm.guannengcc.top

[U11] Py：生成器表达式
来源：http://sia.quarkkingdee.top

(x * 2 for x in arr)
来源：http://nvy.jinghuilouyu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://eho.svipenyu.cn

Counter(arr).most_common(3)
来源：http://byx.ehwqpu.com

[U13] Py：固定长度队列
来源：http://gbp.ehwqpu.com

deque(maxlen=10)
来源：http://pdt.shangyingyoupin.top

[U14] Py：分组收集到列表
来源：http://xeh.aizwys.cn

defaultdict(list)
来源：http://lpc.yangfankeji.com

[U15] Py：高精度计时
来源：http://kdf.zhoulong.xyz

t = time.perf_counter()
来源：http://eya.jinqigufen.top

[U16] Py：命令行参数解析
来源：http://bxj.wangshuangyany.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zpe.cheryme.top

[U17] Py：初始化日志
来源：http://vgg.yvedp.cn

logging.basicConfig(level=logging.INFO)
来源：http://orn.dianchejie.cn

[U18] Py：预编译正则
来源：http://ydi.jyoumei.cn

pat = re.compile(r"\d+")
来源：http://fum.nanxuanxn.top

[U19] Py：正则替换带回调
来源：http://wxs.tian-w.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vuo.daxiang520.top

[U20] Py：缓存函数结果
来源：http://hoo.52xcode.cn

@functools.lru_cache(maxsize=None)
来源：http://orn.xingfuxueyuan.xyz

[U21] Py：自定义上下文管理器
来源：http://fkz.bbcook.cn

@contextlib.contextmanager
来源：http://iip.chenjidiqi.icu

[U22] Py：矩阵转置
来源：http://jta.yj202588.top

list(zip(*m))
来源：http://hih.yuxming.cn

[U23] Py：分块读取大文件
来源：http://vfd.ivvv.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bmx.jyoumei.cn

[U24] Py：路径操作
来源：http://zec.shuidangran.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rls.birdmap.top

[U25] Py：CSV 按字典读
来源：http://ces.fanxiaobao.xyz

csv.DictReader(f)
来源：http://fxv.jinyuanbaomall.cn

[U26] Py：并发下载
来源：http://ejv.chenlongwang.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://stu.fehbvm.com

[U27] Py：异步 HTTP
来源：http://nof.epnwcf.com

aiohttp.ClientSession() 配合 async with
来源：http://ohb.sxryk.cn

[U28] Py：类型别名
来源：http://foo.bjfxy.top

UserId = int
来源：http://ecf.ctjpmb.com

[U29] Py：属性校验
来源：http://wil.chenlongwang.top

@property 与 @x.setter 配合
来源：http://fua.hfpthk.cn

[U30] Py：数据类
来源：http://zdi.shangyingyoupin.top

@dataclass(slots=True)
来源：http://tcz.chenzaomai.com

[U31] Py：单测
来源：http://jpt.hesvh.cn

python -m pytest -q
来源：http://ovj.shzxlz.cn

[U32] Py：代码格式化
来源：http://sva.tianlin.xyz

ruff format . && ruff check --fix .
来源：http://jso.dashuyun.cn

[U33] Py：打包发布
来源：http://qlt.shanyushiyangtech.top

python -m build  （依赖 pyproject.toml）
来源：http://qzq.haohaochexian.top

[U34] Py：判断编码
来源：http://hrm.shangyingyoupin.top

chardet.detect(raw)
来源：http://xgz.cucudq.cn

[U35] Py：发送邮件
来源：http://org.9152youxi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://sqp.shanyushiyangkeji.top

[U36] Py：定时任务
来源：http://lru.zhoulong.xyz

schedule.every(10).minutes.do(job)
来源：http://wuz.sysykeji.top

[U37] Py：读写 Excel
来源：http://zng.yongpay.top

pandas.read_excel / DataFrame.to_excel
来源：http://dhh.tanke756.top

[U38] Py：获取脚本所在目录
来源：http://gzp.jqgfzy.top

Path(__file__).resolve().parent
来源：http://ylg.zhengqikj.top

[U39] Py：判断是否在交互环境
来源：http://tda.sxryk.cn

sys.stdout.isatty()
来源：http://szq.jyoumei.cn

[U40] Py：打印到标准错误
来源：http://lki.ehwqpu.com

print("err", file=sys.stderr)
来源：http://ymi.zhoulong.xyz

[U41] PHP：初始化 Composer 项目
来源：http://vzk.fktsv.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ipg.xuanzx.com

[U42] PHP：PSR-4 自动加载
来源：http://hkg.yj20258.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tgb.jinghuilouyu.cn

[U43] PHP：声明命名空间
来源：http://nqd.jiagoushi.top

namespace App\Http;
来源：http://itw.zhengqikj.top

[U44] PHP：开启严格类型
来源：http://vpv.yangfankeji.com

declare(strict_types=1);
来源：http://wlk.sxryk.cn

[U45] PHP：类型声明与返回类型
来源：http://dxy.nwbrower.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://nim.wangdashe.top

[U46] PHP：可空类型
来源：http://jjv.tanke756.top

?string $name = null
来源：http://mch.yvedp.cn

[U47] PHP：联合类型
来源：http://jkh.jyoumei.cn

int|string $id
来源：http://tgc.hcnkem.com

[U48] PHP：纯枚举
来源：http://udh.haohaochexian.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tfb.fengsongda.top

[U49] PHP：只读属性
来源：http://pip.xziqi.cn

public readonly string $name
来源：http://wll.jianghu66.top

[U50] PHP：构造器属性提升
来源：http://snx.xziqi.cn

public function __construct(private int $id) {}
来源：http://wwx.daria6918.cn

[U51] PHP：数组解构
来源：http://znd.cucudq.cn

[$a, $b] = $arr;
来源：http://vll.cashguo.top

[U52] PHP：箭头函数
来源：http://gzn.pengpengdd.cyou

$double = fn($x) => $x * 2;
来源：http://kox.iojbl.cn

[U53] PHP：空合并运算符
来源：http://cvp.zhoulong.xyz

$v = $a ?? $b ?? "default";
来源：http://bba.jyoumei.cn

[U54] PHP：空安全调用
来源：http://cva.dashuyun.cn

$obj?->method()
来源：http://wnx.wangshuangyany.cn

[U55] PHP：match 表达式
来源：http://czb.zdbjq.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://psy.gzhubu.top

[U56] PHP：命名参数
来源：http://vps.jianghu66.top

f(a: 1, b: 2)
来源：http://ltn.iojbl.cn

[U57] PHP：字符串插值
来源：http://mkd.xuanzx.com

"值: {$a}"
来源：http://ugt.zycfv.cn

[U58] PHP：数组三件套
来源：http://vxb.gzhubu.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://sfi.yueranfly.top

[U59] PHP：自定义排序
来源：http://etr.ydzc1.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://isp.havefunace.top

[U60] PHP：JSON 编解码
来源：http://ism.wangdashe.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hkq.tian-w.cn

[U61] PHP：正则
来源：http://zso.guannengcc.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cxt.cucudq.cn

[U62] PHP：日期对象
来源：http://taa.daxiang520.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lla.xinyue.icu

[U63] PHP：文件读写
来源：http://rqd.mhx1999.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yee.yongpay.top

[U64] PHP：目录遍历
来源：http://kmn.316326.xyz

glob("dir/*.php");  scandir("dir");
来源：http://bxz.9152youxi.cn

[U65] PHP：会话
来源：http://aky.jinyuanbaomall.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ila.chenlongwang.top

[U66] PHP：设置 Cookie
来源：http://edp.nanxinkj.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ivx.iojbl.cn

[U67] PHP：处理文件上传
来源：http://ubp.zycfv.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://nwm.aizwys.cn

[U68] PHP：PDO 连接
来源：http://gwk.guannengcc.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://iuv.sufxvd.cn

[U69] PHP：PDO 预处理
来源：http://lhy.zhijiandao.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kcg.shzxlz.cn

[U70] PHP：PDO 事务
来源：http://lnm.fehbvm.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wcx.hnqzz.top

[U71] PHP：抛出异常
来源：http://cms.c1oappe.top

throw new RuntimeException("失败", 500);
来源：http://fsu.hongshengwenyu.top

[U72] PHP：写错误日志
来源：http://fzi.zhaomingkeji.xyz

error_log("失败: " . $e->getMessage());
来源：http://hfs.smart0.xyz

[U73] PHP：读取 ini 配置
来源：http://lsv.hongshengwenyu.top

parse_ini_file("config.ini", true)
来源：http://hhw.iojbl.cn

[U74] PHP：读取环境变量
来源：http://qyl.sxryk.cn

getenv("APP_ENV") ?: "production"
来源：http://lfp.tarul.cn

[U75] PHP：依赖注入
来源：http://enw.ywan-chungtsiang.top

composer require psr/container
来源：http://dfl.tianlin.xyz

[U76] PHP：简单路由
来源：http://oum.ctjpmb.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pbc.chenjidiqi.icu

[U77] PHP：模板渲染
来源：http://rjm.dashuyun.cn

composer require twig/twig
来源：http://keo.zhaomingkeji.xyz

[U78] PHP：单元测试
来源：http://ptx.kuanghao11.cn

composer require --dev phpunit/phpunit
来源：http://sqy.hnxiangtu.top

[U79] PHP：静态分析
来源：http://gsw.zhijiandao.cn

composer require --dev phpstan/phpstan
来源：http://mjt.hnqzz.top

[U80] PHP：代码规范修复
来源：http://gti.vehdjk.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://tio.jiagoushi.top

[U81] JS：初始化项目
来源：http://blo.jyoumei.cn

npm init -y;  npm i express
来源：http://rmg.chenjidiqi.icu

[U82] JS：package.json 脚本
来源：http://dip.birdmap.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fkv.zhaomingkeji.xyz

[U83] JS：ES Module 导入导出
来源：http://lrb.52xcode.cn

export const a = 1;  import { a } from "./m.js";
来源：http://mry.pycfn.com

[U84] JS：CommonJS 写法
来源：http://gmm.cucudq.cn

module.exports = { a };  const { a } = require("./m");
来源：http://edz.jiagoushi.top

[U85] JS：可选链
来源：http://sya.smart0.xyz

a?.b?.c
来源：http://gzh.hywenlv.cn

[U86] JS：空值合并
来源：http://qsj.fehbvm.com

a ?? b
来源：http://hqt.kuanghao11.cn

[U87] JS：解构默认值
来源：http://nku.fanxiaobao.xyz

const { a = 1, b = 2 } = obj;
来源：http://itz.52xcode.cn

[U88] JS：对象展开合并
来源：http://hlj.tian-w.cn

{ ...a, ...b }
来源：http://sdt.fehbvm.com

[U89] JS：数组去重
来源：http://rar.kuanghao11.cn

[...new Set(arr)]
来源：http://xpo.ctjpmb.com

[U90] JS：数字数组排序
来源：http://oxw.fzhhl.top

[...arr].sort((a, b) => a - b)
来源：http://lcw.sweek.top

[U91] JS：对象键值遍历
来源：http://utr.hesvh.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://woi.haohaochexian.top

[U92] JS：深拷贝
来源：http://bml.0kj1m.cn

structuredClone(obj)
来源：http://rnq.ybcxt.top

[U93] JS：模板字符串
来源：http://dmg.bjfxy.top

`共 ${n} 条`
来源：http://cfk.xylfe.cn

[U94] JS：箭头函数
来源：http://zid.tian-w.cn

const double = x => x * 2;
来源：http://roc.cucudq.cn

[U95] JS：Promise 包装
来源：http://lyf.snrcjt.cn

new Promise((resolve, reject) => {})
来源：http://uoo.cqqwz.cn

[U96] JS：async/await 与异常
来源：http://fdz.fanxiaobao.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://izo.ivvv.top

[U97] JS：并发请求
来源：http://wpo.sjlbkw.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ssz.yanxiufei.cn

[U98] JS：fetch 带 JSON
来源：http://gse.fengsongda.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jvt.yj20258888.top

[U99] JS：事件监听
来源：http://tvo.gzhubu.top

el.addEventListener("click", e => {})
来源：http://pyd.havefunace.top

[U100] JS：DOM 查询
来源：http://loc.hesvh.cn

document.querySelector(".item")
来源：http://qut.ehwqpu.com

[U101] JS：classList 操作
来源：http://qha.52xcode.cn

el.classList.toggle("active")
来源：http://ffg.yonumen.top

[U102] JS：本地存储
来源：http://fnm.zhijiandao.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://qor.316326.xyz

[U103] JS：定时器
来源：http://gxs.gaohongyu789.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rsx.xinyue.icu

[U104] JS：防抖
来源：http://zud.ywan-chungtsiang.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xvo.hnxiangtu.top

[U105] JS：节流
来源：http://jxt.aibaodan.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jao.andypj.xyz

[U106] JS：日期格式化
来源：http://ems.hysaishi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mou.snrcjt.cn

[U107] JS：数字千分位
来源：http://wza.xinyue.icu

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fgo.smart0.xyz

[U108] JS：随机整数
来源：http://fqx.mhx1999.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ciu.nwbrower.top

[U109] JS：数组分组
来源：http://kgi.jqgufenzy.top

Object.groupBy(arr, x => x.type)
来源：http://lqz.52xcode.cn

[U110] JS：数组分块
来源：http://cgr.yvedp.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://agb.jlsjyb.cn

[U111] JS：对象转 Map
来源：http://iyr.nanxuanxn.top

new Map(Object.entries(obj))
来源：http://ivg.hnqzz.top

[U112] JS：字符串补位
来源：http://olm.gotoacloud.top

"7".padStart(3, "0")
来源：http://yso.ehwqpu.com

[U113] JS：正则替换全部
来源：http://yzn.redwolf501.top

s.replaceAll("a", "b")
来源：http://ohz.gotoacloud.top

[U114] JS：JSON 深比较
来源：http://lkk.sjlbkw.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://vnj.0kj1m.cn

[U115] JS：生成 UUID
来源：http://amz.guowangkeji.top

crypto.randomUUID()
来源：http://elz.gaohongyu789.top

[U116] JS：类型检查（JSDoc）
来源：http://wvw.pycfn.com

/** @param {string} name */ function f(name) {}
来源：http://pkn.52xcode.cn

[U117] JS：单元测试
来源：http://dws.ivvv.top

npm i -D vitest;  npx vitest
来源：http://whw.iojbl.cn

[U118] JS：开发服务器
来源：http://jcf.yueranfly.top

npm i -D vite;  npx vite
来源：http://moi.xuetiantiany.cn

[U119] JS：生产构建
来源：http://gqm.fehbvm.com

npx vite build
来源：http://cbu.fktsv.cn

[U120] JS：读取环境变量（Vite）
来源：http://fty.cashguo.top

import.meta.env.VITE_API_URL
来源：http://lsn.redwolf501.top

================================================================================
来源：http://mkn.nanxinkj.top

统计汇总
来源：http://pzk.yueranfly.top

================================================================================
来源：http://ihh.jlsjyb.cn

按语言统计（条）：
来源：http://zdw.yanxiufei.cn

Python ......... 252
来源：http://wiq.yueranfly.top

PHP ............ 252
来源：http://rnk.yuanzhike.top

JavaScript ..... 252
来源：http://zkq.ivvv.top

TypeScript ..... 212
来源：http://kxw.smart0.xyz

Java ........... 212
来源：http://xsq.jyoumei.cn

Go ............. 212
来源：http://emw.jinqigufen.top

Ruby ........... 212
来源：http://cpf.cqqwz.cn

C# ............. 212
来源：http://mvt.fanxiaobao.xyz

C .............. 30
来源：http://ndo.nwbrower.top

C++ ............ 30
来源：http://caj.bjfxy.top

SQL ............ 90
来源：http://gbj.fzhhl.top

Bash ........... 80
来源：http://qun.gzhubu.top

Kotlin ......... 15
来源：http://kbe.jinqigufen.top

Swift .......... 15
来源：http://umz.ydzc1.top

Lua ............ 10
来源：http://vtg.chenzaomai.com

Perl ........... 10
来源：http://uxq.mhx1999.top

Scala .......... 10
来源：http://kln.hywenlv.cn

------------------------------------
来源：http://owd.cucudq.cn

合计 ........... 2106 条
来源：http://unm.zhoulong.xyz

按章节统计：
来源：http://oyt.xylfe.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://kcj.epnwcf.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://cbc.yj20258.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://myq.yonumen.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://haw.bjfxy.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://sob.cheryme.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://fcv.ivvv.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://klk.9152youxi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kme.9152youxi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xlv.nanxuanxn.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fvo.fzhhl.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rlu.xuetiantiany.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://php.ivvv.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://xfl.bjfxy.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://biz.0kj1m.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vfa.quarkkingdee.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xre.cheryme.top

Q SQL 专题                              90
来源：http://byo.yonumen.top

R Bash 专题                             80
来源：http://jzv.jinghuilouyu.cn

S C / C++ 专题                          60
来源：http://upy.aizwys.cn

T 其他语言补充                          60
来源：http://jlh.daxiang520.top

U 高频实用片段                         120
来源：http://qvh.zhaomingkeji.xyz

------------------------------------
来源：http://uyn.nanxinkj.top

合计                                  2106 条
来源：http://lky.yuxming.cn

--------------------------------------------------------------------------------
来源：http://nmk.cqqwz.cn

使用提醒
来源：http://mmx.zhoulong.xyz

--------------------------------------------------------------------------------
来源：http://zde.hywenlv.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xmp.nanxuanxn.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://yrm.ctjpmb.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://pkp.fanxiaobao.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://tnf.0kj1m.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://aeq.hcnkem.com

—— 文件结束 ——
来源：http://opd.jinqigfzy.top

================================================================================
来源：http://kqc.chenjidiqi.icu

程序语言常见例子速查手册（2024 版）
来源：http://dgi.sweek.top

Common Programming Examples Cheat Book
来源：http://tov.nanxinkj.top

================================================================================
来源：http://biv.yuxming.cn

【收录内容】
来源：http://rsy.pycfn.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://szh.nanxinkj.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://end.snrcjt.cn

SQL · Bash · C · C++
来源：http://mys.c1oappe.top


<!-- 参考信息 -->