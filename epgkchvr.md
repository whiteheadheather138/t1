代发 wailian999

[U01] Py：创建虚拟环境
来源：http://wyl.uphjek.com

python -m venv .venv && source .venv/bin/activate
来源：http://crd.cheryme.top

[U02] Py：导出 / 安装依赖
来源：http://jef.chenzaomai.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://oqs.gotoacloud.top

[U03] Py：加载 .env 配置
来源：http://viu.fzhhl.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ldq.nanxinkj.top

[U04] Py：变量调试打印
来源：http://mlg.cdnleiting.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://div.ppjwa.cn

[U05] Py：列表去重且保序
来源：http://ser.aibaodan.cn

list(dict.fromkeys(arr))
来源：http://yom.xinyue.icu

[U06] Py：合并两个字典
来源：http://wyv.yvedp.cn

{**a, **b}
来源：http://grw.shanyushiyangtech.top

[U07] Py：反转字典键值
来源：http://omx.hywenlv.cn

{v: k for k, v in d.items()}
来源：http://upw.bjfxy.top

[U08] Py：展平二维列表
来源：http://hwz.tian-w.cn

[y for x in nested for y in x]
来源：http://oil.zdqjudy.top

[U09] Py：字典取最大值的键
来源：http://pgw.guannengcc.top

max(d, key=d.get)
来源：http://qxs.tian-w.cn

[U10] Py：按值排序字典
来源：http://wol.chenzaomai.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uwj.shanyushiyangkeji.top

[U11] Py：生成器表达式
来源：http://iwb.pycfn.com

(x * 2 for x in arr)
来源：http://wfa.jiagoushi.top

[U12] Py：取出现最多的 3 个元素
来源：http://koc.quarkkingdee.top

Counter(arr).most_common(3)
来源：http://knr.sxryk.cn

[U13] Py：固定长度队列
来源：http://mlh.tanke756.top

deque(maxlen=10)
来源：http://omr.tarul.cn

[U14] Py：分组收集到列表
来源：http://onr.cashguo.top

defaultdict(list)
来源：http://low.jqgfzy.top

[U15] Py：高精度计时
来源：http://czq.xuetiantiany.cn

t = time.perf_counter()
来源：http://wrp.ppjwa.cn

[U16] Py：命令行参数解析
来源：http://ayv.hywenlv.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ivo.sjlbkw.cn

[U17] Py：初始化日志
来源：http://rrr.jianghu66.top

logging.basicConfig(level=logging.INFO)
来源：http://ihi.tian-w.cn

[U18] Py：预编译正则
来源：http://ujq.guowangkeji.top

pat = re.compile(r"\d+")
来源：http://mpg.xylfe.cn

[U19] Py：正则替换带回调
来源：http://xcq.cucudq.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kvb.xylfe.cn

[U20] Py：缓存函数结果
来源：http://igb.sysykeji.top

@functools.lru_cache(maxsize=None)
来源：http://ieh.shanyushiyangtech.top

[U21] Py：自定义上下文管理器
来源：http://lqf.aibaodan.cn

@contextlib.contextmanager
来源：http://dws.jyoumei.cn

[U22] Py：矩阵转置
来源：http://sca.ywan-chungtsiang.top

list(zip(*m))
来源：http://opw.hcnkem.com

[U23] Py：分块读取大文件
来源：http://rhz.aibaodan.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ngs.daxiang520.top

[U24] Py：路径操作
来源：http://fbs.birdmap.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wwu.jqgfzy.top

[U25] Py：CSV 按字典读
来源：http://tvy.yuanzhike.top

csv.DictReader(f)
来源：http://zcg.guannengcc.top

[U26] Py：并发下载
来源：http://ccj.redwolf501.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://sky.cashguo.top

[U27] Py：异步 HTTP
来源：http://wrg.yvedp.cn

aiohttp.ClientSession() 配合 async with
来源：http://jvo.tarul.cn

[U28] Py：类型别名
来源：http://msq.gaohongyu789.top

UserId = int
来源：http://lww.fktsv.cn

[U29] Py：属性校验
来源：http://bkb.sxryk.cn

@property 与 @x.setter 配合
来源：http://nge.sjlbkw.cn

[U30] Py：数据类
来源：http://bcx.wangshuangyany.cn

@dataclass(slots=True)
来源：http://pyb.yuanzhike.top

[U31] Py：单测
来源：http://gmu.cqqwz.cn

python -m pytest -q
来源：http://ltv.zhengqikj.top

[U32] Py：代码格式化
来源：http://lwp.bjfxy.top

ruff format . && ruff check --fix .
来源：http://uqc.sysykeji.top

[U33] Py：打包发布
来源：http://hol.sweek.top

python -m build  （依赖 pyproject.toml）
来源：http://hjg.0kj1m.cn

[U34] Py：判断编码
来源：http://jkf.jinqigufen.top

chardet.detect(raw)
来源：http://qgg.shanyushiyangkeji.top

[U35] Py：发送邮件
来源：http://jxb.redwolf501.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://lyt.smart0.xyz

[U36] Py：定时任务
来源：http://oqj.gaohongyu789.top

schedule.every(10).minutes.do(job)
来源：http://fpw.daria6918.cn

[U37] Py：读写 Excel
来源：http://hjl.cheryme.top

pandas.read_excel / DataFrame.to_excel
来源：http://lak.pengpengdd.cyou

[U38] Py：获取脚本所在目录
来源：http://qre.yangfankeji.com

Path(__file__).resolve().parent
来源：http://emx.jinghuilouyu.cn

[U39] Py：判断是否在交互环境
来源：http://yrr.ppjwa.cn

sys.stdout.isatty()
来源：http://meb.jinqigufen.top

[U40] Py：打印到标准错误
来源：http://cnu.svipenyu.cn

print("err", file=sys.stderr)
来源：http://xxs.zhixingplan.top

[U41] PHP：初始化 Composer 项目
来源：http://ebo.redwolf501.top

composer init;  composer require guzzlehttp/guzzle
来源：http://nek.yj202588.top

[U42] PHP：PSR-4 自动加载
来源：http://weu.jinghuilouyu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://pij.xziqi.cn

[U43] PHP：声明命名空间
来源：http://bcf.wangshuangyany.cn

namespace App\Http;
来源：http://nxl.bbcook.cn

[U44] PHP：开启严格类型
来源：http://zas.yvedp.cn

declare(strict_types=1);
来源：http://ynn.aizwys.cn

[U45] PHP：类型声明与返回类型
来源：http://auu.zhaomingkeji.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://gzu.vehdjk.com

[U46] PHP：可空类型
来源：http://dyk.aibaodan.cn

?string $name = null
来源：http://zyw.sufxvd.cn

[U47] PHP：联合类型
来源：http://uek.jyoumei.cn

int|string $id
来源：http://crc.hesvh.cn

[U48] PHP：纯枚举
来源：http://vtn.yuanzhike.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lro.uphjek.com

[U49] PHP：只读属性
来源：http://jhl.bjfxy.top

public readonly string $name
来源：http://ioe.feifeiyinyue.top

[U50] PHP：构造器属性提升
来源：http://omj.quarkkingdee.top

public function __construct(private int $id) {}
来源：http://iul.cucudq.cn

[U51] PHP：数组解构
来源：http://yet.cashguo.top

[$a, $b] = $arr;
来源：http://dtb.sjlbkw.cn

[U52] PHP：箭头函数
来源：http://jyz.birdmap.top

$double = fn($x) => $x * 2;
来源：http://xwy.daxiang520.top

[U53] PHP：空合并运算符
来源：http://thj.hywenlv.cn

$v = $a ?? $b ?? "default";
来源：http://rum.zhijiandao.cn

[U54] PHP：空安全调用
来源：http://pjo.guowangkeji.top

$obj?->method()
来源：http://wcx.wangshuangyany.cn

[U55] PHP：match 表达式
来源：http://uiz.sweek.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zvw.yuxming.cn

[U56] PHP：命名参数
来源：http://xou.yuxming.cn

f(a: 1, b: 2)
来源：http://fkn.tianlin.xyz

[U57] PHP：字符串插值
来源：http://ycm.9152youxi.cn

"值: {$a}"
来源：http://kya.andypj.xyz

[U58] PHP：数组三件套
来源：http://kpl.sweek.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://coc.hysaishi.cn

[U59] PHP：自定义排序
来源：http://cdd.birdmap.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vxy.zhiwuduotai.top

[U60] PHP：JSON 编解码
来源：http://iog.yuxming.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://phz.tianlin.xyz

[U61] PHP：正则
来源：http://mud.gotoacloud.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kth.fehbvm.com

[U62] PHP：日期对象
来源：http://mvk.guannengcc.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nie.shzxlz.cn

[U63] PHP：文件读写
来源：http://qqr.0kj1m.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qrg.guowangkeji.top

[U64] PHP：目录遍历
来源：http://eql.zhengqikj.top

glob("dir/*.php");  scandir("dir");
来源：http://mzf.ctjpmb.com

[U65] PHP：会话
来源：http://lff.yangfankeji.com

session_start();  $_SESSION["uid"] = 1;
来源：http://qnf.hywenlv.cn

[U66] PHP：设置 Cookie
来源：http://kjk.ybcxt.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dkq.gogol.net.cn

[U67] PHP：处理文件上传
来源：http://zqq.kuanghao11.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pef.yueranfly.top

[U68] PHP：PDO 连接
来源：http://gqu.jinyuanbaomall.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://alb.hfpthk.cn

[U69] PHP：PDO 预处理
来源：http://tvw.gaohongyu789.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ffz.svipenyu.cn

[U70] PHP：PDO 事务
来源：http://fpy.zhoulong.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nqb.gotoacloud.top

[U71] PHP：抛出异常
来源：http://vyt.yfazqb.com

throw new RuntimeException("失败", 500);
来源：http://gqx.tarul.cn

[U72] PHP：写错误日志
来源：http://ema.yj20258888.top

error_log("失败: " . $e->getMessage());
来源：http://iyq.nanxuanxn.top

[U73] PHP：读取 ini 配置
来源：http://pkz.fehbvm.com

parse_ini_file("config.ini", true)
来源：http://zqr.jqgfzy.top

[U74] PHP：读取环境变量
来源：http://bth.chenzaomai.com

getenv("APP_ENV") ?: "production"
来源：http://bgw.sxryk.cn

[U75] PHP：依赖注入
来源：http://wue.xziqi.cn

composer require psr/container
来源：http://vxw.vehdjk.com

[U76] PHP：简单路由
来源：http://qpu.dianchejie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tgo.yongpay.top

[U77] PHP：模板渲染
来源：http://klp.smart0.xyz

composer require twig/twig
来源：http://ldu.jiagoushi.top

[U78] PHP：单元测试
来源：http://uoa.shuidangran.top

composer require --dev phpunit/phpunit
来源：http://iwn.pycfn.com

[U79] PHP：静态分析
来源：http://ofq.uphjek.com

composer require --dev phpstan/phpstan
来源：http://agu.shzxlz.cn

[U80] PHP：代码规范修复
来源：http://hda.yfazqb.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://czj.jianghu66.top

[U81] JS：初始化项目
来源：http://wbk.aibaodan.cn

npm init -y;  npm i express
来源：http://grb.fzhhl.top

[U82] JS：package.json 脚本
来源：http://ugc.smart0.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hcc.haohaochexian.top

[U83] JS：ES Module 导入导出
来源：http://wdw.xylfe.cn

export const a = 1;  import { a } from "./m.js";
来源：http://nqf.snrcjt.cn

[U84] JS：CommonJS 写法
来源：http://cct.ctjpmb.com

module.exports = { a };  const { a } = require("./m");
来源：http://wzd.tanke756.top

[U85] JS：可选链
来源：http://oln.pycfn.com

a?.b?.c
来源：http://rfz.jqgufenzy.top

[U86] JS：空值合并
来源：http://uyr.shanyushiyangkeji.top

a ?? b
来源：http://isp.wangdashe.top

[U87] JS：解构默认值
来源：http://ypv.epnwcf.com

const { a = 1, b = 2 } = obj;
来源：http://osy.chenjidiqi.icu

[U88] JS：对象展开合并
来源：http://wca.wangshuangyany.cn

{ ...a, ...b }
来源：http://ben.gzhubu.top

[U89] JS：数组去重
来源：http://exl.guannengcc.top

[...new Set(arr)]
来源：http://pzb.hywenlv.cn

[U90] JS：数字数组排序
来源：http://fjs.daxiang520.top

[...arr].sort((a, b) => a - b)
来源：http://xpx.jinghuilouyu.cn

[U91] JS：对象键值遍历
来源：http://ibc.guannengcc.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://iaf.pycfn.com

[U92] JS：深拷贝
来源：http://oen.daria6918.cn

structuredClone(obj)
来源：http://qqf.havefunace.top

[U93] JS：模板字符串
来源：http://ytj.fengsongda.top

`共 ${n} 条`
来源：http://qmq.hysaishi.cn

[U94] JS：箭头函数
来源：http://kbk.bbcook.cn

const double = x => x * 2;
来源：http://mkg.hywenlv.cn

[U95] JS：Promise 包装
来源：http://jkt.9152youxi.cn

new Promise((resolve, reject) => {})
来源：http://rkx.redwolf501.top

[U96] JS：async/await 与异常
来源：http://bbr.ivvv.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://kzx.zhongyouzk.top

[U97] JS：并发请求
来源：http://jdn.cucudq.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://iqy.birdmap.top

[U98] JS：fetch 带 JSON
来源：http://kem.zhiwuduotai.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hie.shanyushiyangtech.top

[U99] JS：事件监听
来源：http://jlt.guowangkeji.top

el.addEventListener("click", e => {})
来源：http://knx.hnxiangtu.top

[U100] JS：DOM 查询
来源：http://bum.vehdjk.com

document.querySelector(".item")
来源：http://cel.hnxiangtu.top

[U101] JS：classList 操作
来源：http://nyx.feifeiyinyue.top

el.classList.toggle("active")
来源：http://wai.zhixingplan.top

[U102] JS：本地存储
来源：http://jqz.jqgufenzy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://rfx.yongpay.top

[U103] JS：定时器
来源：http://tgx.fehbvm.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tcm.zhixingplan.top

[U104] JS：防抖
来源：http://vey.redwolf501.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://axj.zycfv.cn

[U105] JS：节流
来源：http://ocr.xinyue.icu

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kgr.sysykeji.top

[U106] JS：日期格式化
来源：http://rii.yanxiufei.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vyg.fengsongda.top

[U107] JS：数字千分位
来源：http://wwz.jinghuilouyu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yvr.hywenlv.cn

[U108] JS：随机整数
来源：http://wwl.andypj.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nio.gogol.net.cn

[U109] JS：数组分组
来源：http://zrg.xylfe.cn

Object.groupBy(arr, x => x.type)
来源：http://uxa.hongshengwenyu.top

[U110] JS：数组分块
来源：http://tge.yuanzhike.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kip.chenlongwang.top

[U111] JS：对象转 Map
来源：http://zeq.fengsongda.top

new Map(Object.entries(obj))
来源：http://kqn.pycfn.com

[U112] JS：字符串补位
来源：http://iwl.ivvv.top

"7".padStart(3, "0")
来源：http://fgb.jinyuanbaomall.cn

[U113] JS：正则替换全部
来源：http://bkj.bbcook.cn

s.replaceAll("a", "b")
来源：http://cwz.jinghuilouyu.cn

[U114] JS：JSON 深比较
来源：http://fgx.tian-w.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://fhs.jianghu66.top

[U115] JS：生成 UUID
来源：http://prl.jinqigufen.top

crypto.randomUUID()
来源：http://kxh.ywan-chungtsiang.top

[U116] JS：类型检查（JSDoc）
来源：http://qaf.zhijiandao.cn

/** @param {string} name */ function f(name) {}
来源：http://bux.guowangkeji.top

[U117] JS：单元测试
来源：http://jmj.tian-w.cn

npm i -D vitest;  npx vitest
来源：http://vmp.vqdsnc.cn

[U118] JS：开发服务器
来源：http://kga.yj202588.top

npm i -D vite;  npx vite
来源：http://khq.ivvv.top

[U119] JS：生产构建
来源：http://jmf.zdbjq.cn

npx vite build
来源：http://usa.meibo888.top

[U120] JS：读取环境变量（Vite）
来源：http://eti.chenzaomai.com

import.meta.env.VITE_API_URL
来源：http://ahf.0kj1m.cn

================================================================================
来源：http://pim.jianghu66.top

统计汇总
来源：http://jzh.mhx1999.top

================================================================================
来源：http://off.fehbvm.com

按语言统计（条）：
来源：http://zbu.yuanzhike.top

Python ......... 252
来源：http://bfn.svipenyu.cn

PHP ............ 252
来源：http://wjv.chenjidiqi.icu

JavaScript ..... 252
来源：http://msl.haohaochexian.top

TypeScript ..... 212
来源：http://pyb.hammf.cn

Java ........... 212
来源：http://bkw.nwbrower.top

Go ............. 212
来源：http://yyo.uphjek.com

Ruby ........... 212
来源：http://six.shanyushiyangtech.top

C# ............. 212
来源：http://eae.xuanzx.com

C .............. 30
来源：http://hwa.guannengcc.top

C++ ............ 30
来源：http://azq.zycfv.cn

SQL ............ 90
来源：http://xuc.hywenlv.cn

Bash ........... 80
来源：http://psk.jianghu66.top

Kotlin ......... 15
来源：http://cvd.zhaomingkeji.xyz

Swift .......... 15
来源：http://edl.ybcxt.top

Lua ............ 10
来源：http://psd.hnqzz.top

Perl ........... 10
来源：http://fwj.tarul.cn

Scala .......... 10
来源：http://gre.shanyushiyangkeji.top

------------------------------------
来源：http://cth.shuidangran.top

合计 ........... 2106 条
来源：http://iot.cucudq.cn

按章节统计：
来源：http://deg.zhixingplan.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ngf.svipenyu.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://fpu.meibo888.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fyz.yuxming.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qjx.zdbjq.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xno.daria6918.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://odv.zdqjudy.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fty.xingfuxueyuan.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://myd.kuanghao11.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ifc.iojbl.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://aji.fanxiaobao.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bbb.zhongyouzk.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ueq.zhixingplan.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://aqn.cheryme.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ylp.snrcjt.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dcg.snrcjt.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://yot.0kj1m.cn

Q SQL 专题                              90
来源：http://wtw.wangshuangyany.cn

R Bash 专题                             80
来源：http://oyo.zhoulong.xyz

S C / C++ 专题                          60
来源：http://rke.sufxvd.cn

T 其他语言补充                          60
来源：http://kdz.yongpay.top

U 高频实用片段                         120
来源：http://veq.yongpay.top

------------------------------------
来源：http://fgs.yongpay.top

合计                                  2106 条
来源：http://zla.cqqwz.cn

--------------------------------------------------------------------------------
来源：http://lex.nanxinkj.top

使用提醒
来源：http://zyk.svipenyu.cn

--------------------------------------------------------------------------------
来源：http://tvx.zycfv.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hnn.shanyushiyangkeji.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://srq.jinyuanbaomall.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vgp.zhaomingkeji.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://ylv.jiagoushi.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ikd.havefunace.top

—— 文件结束 ——
来源：http://ken.guannengcc.top

================================================================================
来源：http://mhs.zhiwuduotai.top

程序语言常见例子速查手册（2024 版）
来源：http://qpu.316326.xyz

Common Programming Examples Cheat Book
来源：http://hui.ydzc1.top

================================================================================
来源：http://dgu.yuanzhike.top


<!-- 参考信息 -->