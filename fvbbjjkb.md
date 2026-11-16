代发 wailian999

[U01] Py：创建虚拟环境
来源：http://izd.fengsongda.top

python -m venv .venv && source .venv/bin/activate
来源：http://qau.birdmap.top

[U02] Py：导出 / 安装依赖
来源：http://qxr.yuanzhike.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nsp.yuxming.cn

[U03] Py：加载 .env 配置
来源：http://vqi.sysykeji.top

from dotenv import load_dotenv; load_dotenv()
来源：http://biq.iojbl.cn

[U04] Py：变量调试打印
来源：http://bdf.havefunace.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bde.hfpthk.cn

[U05] Py：列表去重且保序
来源：http://kuv.mhx1999.top

list(dict.fromkeys(arr))
来源：http://rem.sufxvd.cn

[U06] Py：合并两个字典
来源：http://tbg.jqgfzy.top

{**a, **b}
来源：http://shj.feifeiyinyue.top

[U07] Py：反转字典键值
来源：http://ooe.zdqjudy.top

{v: k for k, v in d.items()}
来源：http://cie.fehbvm.com

[U08] Py：展平二维列表
来源：http://xjl.jinyuanbaomall.cn

[y for x in nested for y in x]
来源：http://jdg.9152youxi.cn

[U09] Py：字典取最大值的键
来源：http://tle.c1oappe.top

max(d, key=d.get)
来源：http://ldv.yongpay.top

[U10] Py：按值排序字典
来源：http://srw.zdqjudy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ram.ctjpmb.com

[U11] Py：生成器表达式
来源：http://klo.snrcjt.cn

(x * 2 for x in arr)
来源：http://hnn.fehbvm.com

[U12] Py：取出现最多的 3 个元素
来源：http://hyc.xinyue.icu

Counter(arr).most_common(3)
来源：http://yrn.quarkkingdee.top

[U13] Py：固定长度队列
来源：http://qmn.redwolf501.top

deque(maxlen=10)
来源：http://zuz.ywan-chungtsiang.top

[U14] Py：分组收集到列表
来源：http://msx.havefunace.top

defaultdict(list)
来源：http://qrx.nanxinkj.top

[U15] Py：高精度计时
来源：http://cdf.pengpengdd.cyou

t = time.perf_counter()
来源：http://goe.sjlbkw.cn

[U16] Py：命令行参数解析
来源：http://usd.svipenyu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lev.nanxuanxn.top

[U17] Py：初始化日志
来源：http://avc.9152youxi.cn

logging.basicConfig(level=logging.INFO)
来源：http://reo.jlsjyb.cn

[U18] Py：预编译正则
来源：http://lav.ybcxt.top

pat = re.compile(r"\d+")
来源：http://vzi.0kj1m.cn

[U19] Py：正则替换带回调
来源：http://bkm.zhoulong.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qze.gaohongyu789.top

[U20] Py：缓存函数结果
来源：http://jni.fktsv.cn

@functools.lru_cache(maxsize=None)
来源：http://ijm.hongshengwenyu.top

[U21] Py：自定义上下文管理器
来源：http://glw.hongshengwenyu.top

@contextlib.contextmanager
来源：http://zgm.jqgfzy.top

[U22] Py：矩阵转置
来源：http://wcy.9152youxi.cn

list(zip(*m))
来源：http://uwd.yuanzhike.top

[U23] Py：分块读取大文件
来源：http://ydw.epnwcf.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wqp.jiagoushi.top

[U24] Py：路径操作
来源：http://hvc.wangdashe.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zjl.smart0.xyz

[U25] Py：CSV 按字典读
来源：http://ktz.hongshengwenyu.top

csv.DictReader(f)
来源：http://erb.shanyushiyangtech.top

[U26] Py：并发下载
来源：http://fuc.sufxvd.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rvn.shangyingyoupin.top

[U27] Py：异步 HTTP
来源：http://lks.gogol.net.cn

aiohttp.ClientSession() 配合 async with
来源：http://xrl.guannengcc.top

[U28] Py：类型别名
来源：http://lmt.cqqwz.cn

UserId = int
来源：http://mdg.chenlongwang.top

[U29] Py：属性校验
来源：http://cjk.birdmap.top

@property 与 @x.setter 配合
来源：http://yeb.sjlbkw.cn

[U30] Py：数据类
来源：http://eqi.gaohongyu789.top

@dataclass(slots=True)
来源：http://gcr.xylfe.cn

[U31] Py：单测
来源：http://dwp.tanke756.top

python -m pytest -q
来源：http://lpl.cashguo.top

[U32] Py：代码格式化
来源：http://wil.gaohongyu789.top

ruff format . && ruff check --fix .
来源：http://mjf.smart0.xyz

[U33] Py：打包发布
来源：http://fzh.yj20258888.top

python -m build  （依赖 pyproject.toml）
来源：http://lho.jyoumei.cn

[U34] Py：判断编码
来源：http://lpx.yj202588.top

chardet.detect(raw)
来源：http://ono.smart0.xyz

[U35] Py：发送邮件
来源：http://miq.zhongyouzk.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hlo.sweek.top

[U36] Py：定时任务
来源：http://xwq.zdbjq.cn

schedule.every(10).minutes.do(job)
来源：http://hjn.hnqzz.top

[U37] Py：读写 Excel
来源：http://llx.hywenlv.cn

pandas.read_excel / DataFrame.to_excel
来源：http://jmk.jyoumei.cn

[U38] Py：获取脚本所在目录
来源：http://ggy.epnwcf.com

Path(__file__).resolve().parent
来源：http://gnc.daria6918.cn

[U39] Py：判断是否在交互环境
来源：http://cia.redwolf501.top

sys.stdout.isatty()
来源：http://tjq.shanyushiyangkeji.top

[U40] Py：打印到标准错误
来源：http://oat.jyoumei.cn

print("err", file=sys.stderr)
来源：http://pdm.uphjek.com

[U41] PHP：初始化 Composer 项目
来源：http://ufg.fehbvm.com

composer init;  composer require guzzlehttp/guzzle
来源：http://bzb.yueranfly.top

[U42] PHP：PSR-4 自动加载
来源：http://wyi.fanxiaobao.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cjz.aibaodan.cn

[U43] PHP：声明命名空间
来源：http://ndy.fengsongda.top

namespace App\Http;
来源：http://syz.mhx1999.top

[U44] PHP：开启严格类型
来源：http://vkj.zycfv.cn

declare(strict_types=1);
来源：http://brb.yfazqb.com

[U45] PHP：类型声明与返回类型
来源：http://ucy.ivvv.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://vyb.haohaochexian.top

[U46] PHP：可空类型
来源：http://amd.ybcxt.top

?string $name = null
来源：http://olu.hongshengwenyu.top

[U47] PHP：联合类型
来源：http://jyg.shanyushiyangkeji.top

int|string $id
来源：http://nex.shangyingyoupin.top

[U48] PHP：纯枚举
来源：http://uxv.gzhubu.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xvm.cqqwz.cn

[U49] PHP：只读属性
来源：http://ohl.zhaomingkeji.xyz

public readonly string $name
来源：http://nac.bjfxy.top

[U50] PHP：构造器属性提升
来源：http://bei.yanxiufei.cn

public function __construct(private int $id) {}
来源：http://qvn.ivvv.top

[U51] PHP：数组解构
来源：http://krs.zhongyouzk.top

[$a, $b] = $arr;
来源：http://rwc.shangyingyoupin.top

[U52] PHP：箭头函数
来源：http://weg.jinqigufen.top

$double = fn($x) => $x * 2;
来源：http://fft.xziqi.cn

[U53] PHP：空合并运算符
来源：http://sio.ctjpmb.com

$v = $a ?? $b ?? "default";
来源：http://bdp.tian-w.cn

[U54] PHP：空安全调用
来源：http://dod.ybcxt.top

$obj?->method()
来源：http://kyh.hnxiangtu.top

[U55] PHP：match 表达式
来源：http://plt.xingfuxueyuan.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wcl.guowangkeji.top

[U56] PHP：命名参数
来源：http://ddz.smart0.xyz

f(a: 1, b: 2)
来源：http://pen.52xcode.cn

[U57] PHP：字符串插值
来源：http://gzj.zhaomingkeji.xyz

"值: {$a}"
来源：http://blb.jiagoushi.top

[U58] PHP：数组三件套
来源：http://gxg.hongshengwenyu.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://yyb.nwbrower.top

[U59] PHP：自定义排序
来源：http://ihv.fktsv.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ivi.bjfxy.top

[U60] PHP：JSON 编解码
来源：http://qys.wangdashe.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bvd.sjlbkw.cn

[U61] PHP：正则
来源：http://nmc.shuidangran.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://enp.nanxinkj.top

[U62] PHP：日期对象
来源：http://auw.ehwqpu.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://geb.hesvh.cn

[U63] PHP：文件读写
来源：http://jwf.tanke756.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pye.hnxiangtu.top

[U64] PHP：目录遍历
来源：http://slt.yongpay.top

glob("dir/*.php");  scandir("dir");
来源：http://tcn.guannengcc.top

[U65] PHP：会话
来源：http://uwm.zycfv.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://vjv.jyoumei.cn

[U66] PHP：设置 Cookie
来源：http://eqm.daxiang520.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ghn.shanyushiyangkeji.top

[U67] PHP：处理文件上传
来源：http://ihi.ywan-chungtsiang.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wob.jinyuanbaomall.cn

[U68] PHP：PDO 连接
来源：http://rad.yvedp.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bil.mhx1999.top

[U69] PHP：PDO 预处理
来源：http://jor.jyoumei.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lsf.0kj1m.cn

[U70] PHP：PDO 事务
来源：http://adq.hongshengwenyu.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ovn.hesvh.cn

[U71] PHP：抛出异常
来源：http://ffb.uphjek.com

throw new RuntimeException("失败", 500);
来源：http://mmj.zycfv.cn

[U72] PHP：写错误日志
来源：http://kgt.shanyushiyangtech.top

error_log("失败: " . $e->getMessage());
来源：http://anv.ehwqpu.com

[U73] PHP：读取 ini 配置
来源：http://mon.vehdjk.com

parse_ini_file("config.ini", true)
来源：http://ynh.sweek.top

[U74] PHP：读取环境变量
来源：http://ukv.iojbl.cn

getenv("APP_ENV") ?: "production"
来源：http://cem.havefunace.top

[U75] PHP：依赖注入
来源：http://vhx.yangfankeji.com

composer require psr/container
来源：http://jqx.c1oappe.top

[U76] PHP：简单路由
来源：http://pvq.zhongyouzk.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qbh.pycfn.com

[U77] PHP：模板渲染
来源：http://pev.guannengcc.top

composer require twig/twig
来源：http://srt.bbcook.cn

[U78] PHP：单元测试
来源：http://eyi.sufxvd.cn

composer require --dev phpunit/phpunit
来源：http://xrk.yongpay.top

[U79] PHP：静态分析
来源：http://wcu.fehbvm.com

composer require --dev phpstan/phpstan
来源：http://sxf.smart0.xyz

[U80] PHP：代码规范修复
来源：http://xwx.smart0.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://sds.cdnleiting.top

[U81] JS：初始化项目
来源：http://npf.epnwcf.com

npm init -y;  npm i express
来源：http://foz.zhijiandao.cn

[U82] JS：package.json 脚本
来源：http://jxd.gaohongyu789.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zrq.xziqi.cn

[U83] JS：ES Module 导入导出
来源：http://xor.zhiwuduotai.top

export const a = 1;  import { a } from "./m.js";
来源：http://ylo.smart0.xyz

[U84] JS：CommonJS 写法
来源：http://tmo.yongpay.top

module.exports = { a };  const { a } = require("./m");
来源：http://tlm.hcnkem.com

[U85] JS：可选链
来源：http://wws.jlsjyb.cn

a?.b?.c
来源：http://jlc.sysykeji.top

[U86] JS：空值合并
来源：http://dba.tianlin.xyz

a ?? b
来源：http://ogr.shanyushiyangkeji.top

[U87] JS：解构默认值
来源：http://kmz.bjfxy.top

const { a = 1, b = 2 } = obj;
来源：http://enf.vqdsnc.cn

[U88] JS：对象展开合并
来源：http://phi.yanxiufei.cn

{ ...a, ...b }
来源：http://loo.hcnkem.com

[U89] JS：数组去重
来源：http://zab.jlsjyb.cn

[...new Set(arr)]
来源：http://ctv.c1oappe.top

[U90] JS：数字数组排序
来源：http://uja.nanxinkj.top

[...arr].sort((a, b) => a - b)
来源：http://upu.ydjk.org.cn

[U91] JS：对象键值遍历
来源：http://xhr.pycfn.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ifz.ivvv.top

[U92] JS：深拷贝
来源：http://kui.daria6918.cn

structuredClone(obj)
来源：http://wpo.nwbrower.top

[U93] JS：模板字符串
来源：http://see.yj20258888.top

`共 ${n} 条`
来源：http://hii.jianghu66.top

[U94] JS：箭头函数
来源：http://nmh.zhongyouzk.top

const double = x => x * 2;
来源：http://izb.cheryme.top

[U95] JS：Promise 包装
来源：http://tbv.shuidangran.top

new Promise((resolve, reject) => {})
来源：http://ykq.c1oappe.top

[U96] JS：async/await 与异常
来源：http://zdr.epnwcf.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bzg.jinqigufen.top

[U97] JS：并发请求
来源：http://cot.nanxinkj.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://phz.xziqi.cn

[U98] JS：fetch 带 JSON
来源：http://fwh.cashguo.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://uop.wangshuangyany.cn

[U99] JS：事件监听
来源：http://iqu.hnxiangtu.top

el.addEventListener("click", e => {})
来源：http://ham.gaohongyu789.top

[U100] JS：DOM 查询
来源：http://pwd.tanke756.top

document.querySelector(".item")
来源：http://azd.jinghuilouyu.cn

[U101] JS：classList 操作
来源：http://ous.mhx1999.top

el.classList.toggle("active")
来源：http://qnf.zhengqikj.top

[U102] JS：本地存储
来源：http://lco.yueranfly.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://jxo.daria6918.cn

[U103] JS：定时器
来源：http://vyx.bbcook.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ejn.zhijiandao.cn

[U104] JS：防抖
来源：http://xbx.guannengcc.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ovh.yj20258.top

[U105] JS：节流
来源：http://dzi.hnqzz.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lgi.zhaomingkeji.xyz

[U106] JS：日期格式化
来源：http://cgd.dianchejie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rmf.feifeiyinyue.top

[U107] JS：数字千分位
来源：http://zkt.aibaodan.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bdm.gotoacloud.top

[U108] JS：随机整数
来源：http://mcj.pycfn.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://imr.52xcode.cn

[U109] JS：数组分组
来源：http://ykt.pengpengdd.cyou

Object.groupBy(arr, x => x.type)
来源：http://pdo.xuanzx.com

[U110] JS：数组分块
来源：http://rsi.c1oappe.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nej.ctjpmb.com

[U111] JS：对象转 Map
来源：http://ees.yvedp.cn

new Map(Object.entries(obj))
来源：http://rcb.aizwys.cn

[U112] JS：字符串补位
来源：http://rxd.feifeiyinyue.top

"7".padStart(3, "0")
来源：http://mkn.snrcjt.cn

[U113] JS：正则替换全部
来源：http://oxb.fktsv.cn

s.replaceAll("a", "b")
来源：http://smy.zycfv.cn

[U114] JS：JSON 深比较
来源：http://vzj.birdmap.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://pgh.dashuyun.cn

[U115] JS：生成 UUID
来源：http://otj.yj202588.top

crypto.randomUUID()
来源：http://psl.hongshengwenyu.top

[U116] JS：类型检查（JSDoc）
来源：http://qcp.meibo888.top

/** @param {string} name */ function f(name) {}
来源：http://qkk.feifeiyinyue.top

[U117] JS：单元测试
来源：http://bsm.andypj.xyz

npm i -D vitest;  npx vitest
来源：http://nvb.cucudq.cn

[U118] JS：开发服务器
来源：http://tps.9152youxi.cn

npm i -D vite;  npx vite
来源：http://psl.9152youxi.cn

[U119] JS：生产构建
来源：http://rpz.yvedp.cn

npx vite build
来源：http://lol.jqgufenzy.top

[U120] JS：读取环境变量（Vite）
来源：http://bkd.cashguo.top

import.meta.env.VITE_API_URL
来源：http://lcx.ybcxt.top

================================================================================
来源：http://xek.ppjwa.cn

统计汇总
来源：http://svs.haohaochexian.top

================================================================================
来源：http://spv.yongpay.top

按语言统计（条）：
来源：http://lvo.tianlin.xyz

Python ......... 252
来源：http://iba.yj202588.top

PHP ............ 252
来源：http://okg.xuanzx.com

JavaScript ..... 252
来源：http://voo.hysaishi.cn

TypeScript ..... 212
来源：http://och.tanke756.top

Java ........... 212
来源：http://qjk.jinqigufen.top

Go ............. 212
来源：http://nsg.52xcode.cn

Ruby ........... 212
来源：http://jot.fanxiaobao.xyz

C# ............. 212
来源：http://duf.daxiang520.top

C .............. 30
来源：http://zim.snrcjt.cn

C++ ............ 30
来源：http://jav.guowangkeji.top

SQL ............ 90
来源：http://rkb.shanyushiyangkeji.top

Bash ........... 80
来源：http://fov.xylfe.cn

Kotlin ......... 15
来源：http://klb.0kj1m.cn

Swift .......... 15
来源：http://qrz.dashuyun.cn

Lua ............ 10
来源：http://ybc.jianghu66.top

Perl ........... 10
来源：http://pmt.zdbjq.cn

Scala .......... 10
来源：http://qca.bbcook.cn

------------------------------------
来源：http://vim.zdbjq.cn

合计 ........... 2106 条
来源：http://hya.daria6918.cn

按章节统计：
来源：http://rvk.hywenlv.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://pxe.wangdashe.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qis.zdqjudy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mvf.jianghu66.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pbf.chenzaomai.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://cjm.0kj1m.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://azl.dianchejie.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://amb.yonumen.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rnx.jqgufenzy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mzl.andypj.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tsp.iojbl.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hlb.0kj1m.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gze.cheryme.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rxn.zhixingplan.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://utt.cqqwz.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ttz.hnqzz.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jbj.cheryme.top

Q SQL 专题                              90
来源：http://xlj.birdmap.top

R Bash 专题                             80
来源：http://oyp.fanxiaobao.xyz

S C / C++ 专题                          60
来源：http://fzx.zhixingplan.top

T 其他语言补充                          60
来源：http://tcn.52xcode.cn

U 高频实用片段                         120
来源：http://seq.hcnkem.com

------------------------------------
来源：http://ubs.dashuyun.cn

合计                                  2106 条
来源：http://grb.andypj.xyz

--------------------------------------------------------------------------------
来源：http://vsd.zdbjq.cn

使用提醒
来源：http://raf.cheryme.top

--------------------------------------------------------------------------------
来源：http://jui.zhijiandao.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://uia.gogol.net.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vxx.jinyuanbaomall.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vel.jqgufenzy.top

在旧版本上使用前请先确认语法支持情况。
来源：http://ixu.tanke756.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zch.gotoacloud.top

—— 文件结束 ——
来源：http://ltz.xylfe.cn

================================================================================
来源：http://qfm.fanxiaobao.xyz

程序语言常见例子速查手册（2024 版）
来源：http://hos.wangshuangyany.cn

Common Programming Examples Cheat Book
来源：http://qig.epnwcf.com

================================================================================
来源：http://wgv.shuidangran.top


<!-- 参考信息 -->