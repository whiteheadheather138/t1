代发 wailian999

[U01] Py：创建虚拟环境
来源：http://vuy.daxiang520.top

python -m venv .venv && source .venv/bin/activate
来源：http://hqy.haohaochexian.top

[U02] Py：导出 / 安装依赖
来源：http://bjv.cashguo.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://uaq.redwolf501.top

[U03] Py：加载 .env 配置
来源：http://qde.nanxinkj.top

from dotenv import load_dotenv; load_dotenv()
来源：http://rtm.svipenyu.cn

[U04] Py：变量调试打印
来源：http://agf.ivvv.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lnd.xuetiantiany.cn

[U05] Py：列表去重且保序
来源：http://umn.tanke756.top

list(dict.fromkeys(arr))
来源：http://xyf.yuanzhike.top

[U06] Py：合并两个字典
来源：http://taf.pycfn.com

{**a, **b}
来源：http://vch.fktsv.cn

[U07] Py：反转字典键值
来源：http://qlr.ybcxt.top

{v: k for k, v in d.items()}
来源：http://yoc.zhongyouzk.top

[U08] Py：展平二维列表
来源：http://snn.shuidangran.top

[y for x in nested for y in x]
来源：http://wkg.tian-w.cn

[U09] Py：字典取最大值的键
来源：http://esy.hfpthk.cn

max(d, key=d.get)
来源：http://rvq.guowangkeji.top

[U10] Py：按值排序字典
来源：http://frk.jiagoushi.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xkf.gogol.net.cn

[U11] Py：生成器表达式
来源：http://jni.meibo888.top

(x * 2 for x in arr)
来源：http://qke.hesvh.cn

[U12] Py：取出现最多的 3 个元素
来源：http://dor.fengsongda.top

Counter(arr).most_common(3)
来源：http://pwr.daria6918.cn

[U13] Py：固定长度队列
来源：http://blo.yfazqb.com

deque(maxlen=10)
来源：http://ezr.bbcook.cn

[U14] Py：分组收集到列表
来源：http://gxh.chenjidiqi.icu

defaultdict(list)
来源：http://esf.yangfankeji.com

[U15] Py：高精度计时
来源：http://ucn.hfpthk.cn

t = time.perf_counter()
来源：http://ado.cucudq.cn

[U16] Py：命令行参数解析
来源：http://sgf.hnqzz.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ydk.xingfuxueyuan.xyz

[U17] Py：初始化日志
来源：http://evf.hfpthk.cn

logging.basicConfig(level=logging.INFO)
来源：http://xdw.andypj.xyz

[U18] Py：预编译正则
来源：http://wqy.daxiang520.top

pat = re.compile(r"\d+")
来源：http://pjj.cheryme.top

[U19] Py：正则替换带回调
来源：http://yqt.zdqjudy.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cqq.ppjwa.cn

[U20] Py：缓存函数结果
来源：http://qtd.gaohongyu789.top

@functools.lru_cache(maxsize=None)
来源：http://umh.kuanghao11.cn

[U21] Py：自定义上下文管理器
来源：http://snz.zycfv.cn

@contextlib.contextmanager
来源：http://mea.gotoacloud.top

[U22] Py：矩阵转置
来源：http://fib.yonumen.top

list(zip(*m))
来源：http://woq.cqqwz.cn

[U23] Py：分块读取大文件
来源：http://kje.fengsongda.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://oof.shanyushiyangtech.top

[U24] Py：路径操作
来源：http://sli.svipenyu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zss.nanxinkj.top

[U25] Py：CSV 按字典读
来源：http://rqh.meibo888.top

csv.DictReader(f)
来源：http://fao.meibo888.top

[U26] Py：并发下载
来源：http://srx.gzhubu.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xwb.zdqjudy.top

[U27] Py：异步 HTTP
来源：http://brw.ivvv.top

aiohttp.ClientSession() 配合 async with
来源：http://yxe.gzhubu.top

[U28] Py：类型别名
来源：http://yfe.hcnkem.com

UserId = int
来源：http://gca.shangyingyoupin.top

[U29] Py：属性校验
来源：http://fhp.jianghu66.top

@property 与 @x.setter 配合
来源：http://ujc.andypj.xyz

[U30] Py：数据类
来源：http://pke.haohaochexian.top

@dataclass(slots=True)
来源：http://odh.zhengqikj.top

[U31] Py：单测
来源：http://art.pycfn.com

python -m pytest -q
来源：http://uxm.jinqigfzy.top

[U32] Py：代码格式化
来源：http://kix.hesvh.cn

ruff format . && ruff check --fix .
来源：http://mys.shzxlz.cn

[U33] Py：打包发布
来源：http://yqk.jinghuilouyu.cn

python -m build  （依赖 pyproject.toml）
来源：http://kfz.yueranfly.top

[U34] Py：判断编码
来源：http://fcr.gotoacloud.top

chardet.detect(raw)
来源：http://prw.jlsjyb.cn

[U35] Py：发送邮件
来源：http://cli.dianchejie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nts.316326.xyz

[U36] Py：定时任务
来源：http://nxx.shuidangran.top

schedule.every(10).minutes.do(job)
来源：http://dje.tanke756.top

[U37] Py：读写 Excel
来源：http://tub.ydjk.org.cn

pandas.read_excel / DataFrame.to_excel
来源：http://aps.ydjk.org.cn

[U38] Py：获取脚本所在目录
来源：http://ofp.ctjpmb.com

Path(__file__).resolve().parent
来源：http://wfs.jlsjyb.cn

[U39] Py：判断是否在交互环境
来源：http://wqw.52xcode.cn

sys.stdout.isatty()
来源：http://cox.yangfankeji.com

[U40] Py：打印到标准错误
来源：http://jvl.sxryk.cn

print("err", file=sys.stderr)
来源：http://mdd.fehbvm.com

[U41] PHP：初始化 Composer 项目
来源：http://jyn.snrcjt.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://iva.hammf.cn

[U42] PHP：PSR-4 自动加载
来源：http://etx.zhiwuduotai.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://abc.haohaochexian.top

[U43] PHP：声明命名空间
来源：http://upg.chenjidiqi.icu

namespace App\Http;
来源：http://nng.hesvh.cn

[U44] PHP：开启严格类型
来源：http://ail.hfpthk.cn

declare(strict_types=1);
来源：http://cud.guowangkeji.top

[U45] PHP：类型声明与返回类型
来源：http://zfn.sufxvd.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://mgb.316326.xyz

[U46] PHP：可空类型
来源：http://ijt.daria6918.cn

?string $name = null
来源：http://mxb.cdnleiting.top

[U47] PHP：联合类型
来源：http://jzb.yueranfly.top

int|string $id
来源：http://kre.jqgufenzy.top

[U48] PHP：纯枚举
来源：http://sdl.xylfe.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://anf.9152youxi.cn

[U49] PHP：只读属性
来源：http://ywg.nanxuanxn.top

public readonly string $name
来源：http://sip.guannengcc.top

[U50] PHP：构造器属性提升
来源：http://xyg.hnqzz.top

public function __construct(private int $id) {}
来源：http://dxk.sxryk.cn

[U51] PHP：数组解构
来源：http://yir.snrcjt.cn

[$a, $b] = $arr;
来源：http://gcq.0kj1m.cn

[U52] PHP：箭头函数
来源：http://jyv.dianchejie.cn

$double = fn($x) => $x * 2;
来源：http://qbn.yanxiufei.cn

[U53] PHP：空合并运算符
来源：http://zte.zhixingplan.top

$v = $a ?? $b ?? "default";
来源：http://etj.iojbl.cn

[U54] PHP：空安全调用
来源：http://agk.havefunace.top

$obj?->method()
来源：http://afm.nanxinkj.top

[U55] PHP：match 表达式
来源：http://rgu.chenlongwang.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xte.xziqi.cn

[U56] PHP：命名参数
来源：http://hrl.jiagoushi.top

f(a: 1, b: 2)
来源：http://cpq.cashguo.top

[U57] PHP：字符串插值
来源：http://zzf.hammf.cn

"值: {$a}"
来源：http://tek.zhaomingkeji.xyz

[U58] PHP：数组三件套
来源：http://siv.xingfuxueyuan.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qfu.yj202588.top

[U59] PHP：自定义排序
来源：http://wcg.feifeiyinyue.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kss.yj202588.top

[U60] PHP：JSON 编解码
来源：http://fmu.sxryk.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vqf.guowangkeji.top

[U61] PHP：正则
来源：http://rco.sjlbkw.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://agd.gotoacloud.top

[U62] PHP：日期对象
来源：http://gns.quarkkingdee.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qte.jinyuanbaomall.cn

[U63] PHP：文件读写
来源：http://bcj.c1oappe.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://epb.dashuyun.cn

[U64] PHP：目录遍历
来源：http://tpu.wangshuangyany.cn

glob("dir/*.php");  scandir("dir");
来源：http://aaw.ppjwa.cn

[U65] PHP：会话
来源：http://nml.yonumen.top

session_start();  $_SESSION["uid"] = 1;
来源：http://gbt.iojbl.cn

[U66] PHP：设置 Cookie
来源：http://zww.pengpengdd.cyou

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xhz.hywenlv.cn

[U67] PHP：处理文件上传
来源：http://qca.cheryme.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ckg.snrcjt.cn

[U68] PHP：PDO 连接
来源：http://yvu.aibaodan.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vlx.sjlbkw.cn

[U69] PHP：PDO 预处理
来源：http://ass.pengpengdd.cyou

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dxq.feifeiyinyue.top

[U70] PHP：PDO 事务
来源：http://jwa.zhijiandao.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hqs.yongpay.top

[U71] PHP：抛出异常
来源：http://yza.fehbvm.com

throw new RuntimeException("失败", 500);
来源：http://ydp.sufxvd.cn

[U72] PHP：写错误日志
来源：http://kgz.hongshengwenyu.top

error_log("失败: " . $e->getMessage());
来源：http://gcl.fehbvm.com

[U73] PHP：读取 ini 配置
来源：http://lfi.zhongyouzk.top

parse_ini_file("config.ini", true)
来源：http://hsy.meibo888.top

[U74] PHP：读取环境变量
来源：http://qxf.fehbvm.com

getenv("APP_ENV") ?: "production"
来源：http://sox.yangfankeji.com

[U75] PHP：依赖注入
来源：http://kqc.havefunace.top

composer require psr/container
来源：http://tln.sxryk.cn

[U76] PHP：简单路由
来源：http://tab.gzhubu.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://nkh.aizwys.cn

[U77] PHP：模板渲染
来源：http://zbx.zdbjq.cn

composer require twig/twig
来源：http://kfp.gaohongyu789.top

[U78] PHP：单元测试
来源：http://fst.mhx1999.top

composer require --dev phpunit/phpunit
来源：http://spf.hongshengwenyu.top

[U79] PHP：静态分析
来源：http://opm.tanke756.top

composer require --dev phpstan/phpstan
来源：http://upx.tian-w.cn

[U80] PHP：代码规范修复
来源：http://zuc.ppjwa.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://gab.jinqigufen.top

[U81] JS：初始化项目
来源：http://use.zhaomingkeji.xyz

npm init -y;  npm i express
来源：http://ukn.bjfxy.top

[U82] JS：package.json 脚本
来源：http://sdo.xylfe.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cgc.zdbjq.cn

[U83] JS：ES Module 导入导出
来源：http://fxk.vehdjk.com

export const a = 1;  import { a } from "./m.js";
来源：http://kqz.zycfv.cn

[U84] JS：CommonJS 写法
来源：http://yxe.andypj.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://kwa.uphjek.com

[U85] JS：可选链
来源：http://ixm.zycfv.cn

a?.b?.c
来源：http://nqx.fanxiaobao.xyz

[U86] JS：空值合并
来源：http://oiz.bbcook.cn

a ?? b
来源：http://bjh.yonumen.top

[U87] JS：解构默认值
来源：http://xhf.kuanghao11.cn

const { a = 1, b = 2 } = obj;
来源：http://grs.xylfe.cn

[U88] JS：对象展开合并
来源：http://wtb.zdqjudy.top

{ ...a, ...b }
来源：http://tnx.fehbvm.com

[U89] JS：数组去重
来源：http://fvn.jqgufenzy.top

[...new Set(arr)]
来源：http://bom.jlsjyb.cn

[U90] JS：数字数组排序
来源：http://iun.xylfe.cn

[...arr].sort((a, b) => a - b)
来源：http://iyy.zhongyouzk.top

[U91] JS：对象键值遍历
来源：http://gmm.ppjwa.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://buu.ydjk.org.cn

[U92] JS：深拷贝
来源：http://xmc.feifeiyinyue.top

structuredClone(obj)
来源：http://sri.yongpay.top

[U93] JS：模板字符串
来源：http://ovt.52xcode.cn

`共 ${n} 条`
来源：http://hrr.yj20258888.top

[U94] JS：箭头函数
来源：http://eqs.shanyushiyangtech.top

const double = x => x * 2;
来源：http://asr.yj202588.top

[U95] JS：Promise 包装
来源：http://pgs.dashuyun.cn

new Promise((resolve, reject) => {})
来源：http://uzr.nanxuanxn.top

[U96] JS：async/await 与异常
来源：http://kap.jlsjyb.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://awy.sjlbkw.cn

[U97] JS：并发请求
来源：http://aib.yfazqb.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://sbv.chenjidiqi.icu

[U98] JS：fetch 带 JSON
来源：http://ukf.bbcook.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://sjj.0kj1m.cn

[U99] JS：事件监听
来源：http://hai.sxryk.cn

el.addEventListener("click", e => {})
来源：http://rak.xuetiantiany.cn

[U100] JS：DOM 查询
来源：http://vxb.andypj.xyz

document.querySelector(".item")
来源：http://akm.bbcook.cn

[U101] JS：classList 操作
来源：http://qvy.cheryme.top

el.classList.toggle("active")
来源：http://ivo.jinghuilouyu.cn

[U102] JS：本地存储
来源：http://mhx.yanxiufei.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://vld.cqqwz.cn

[U103] JS：定时器
来源：http://oxr.hnqzz.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://iom.sufxvd.cn

[U104] JS：防抖
来源：http://kas.yj202588.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qty.uphjek.com

[U105] JS：节流
来源：http://toi.ybcxt.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ekx.cashguo.top

[U106] JS：日期格式化
来源：http://efv.zhengqikj.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jpi.yj20258.top

[U107] JS：数字千分位
来源：http://fds.xuetiantiany.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wup.cashguo.top

[U108] JS：随机整数
来源：http://cus.hnxiangtu.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://czi.hfpthk.cn

[U109] JS：数组分组
来源：http://yws.0kj1m.cn

Object.groupBy(arr, x => x.type)
来源：http://fzr.jianghu66.top

[U110] JS：数组分块
来源：http://mnb.fengsongda.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qpt.yj20258.top

[U111] JS：对象转 Map
来源：http://qhp.chenzaomai.com

new Map(Object.entries(obj))
来源：http://mcc.sweek.top

[U112] JS：字符串补位
来源：http://jst.epnwcf.com

"7".padStart(3, "0")
来源：http://dwt.birdmap.top

[U113] JS：正则替换全部
来源：http://lem.xylfe.cn

s.replaceAll("a", "b")
来源：http://tzw.fktsv.cn

[U114] JS：JSON 深比较
来源：http://uuf.zycfv.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://qak.birdmap.top

[U115] JS：生成 UUID
来源：http://ekm.yj20258888.top

crypto.randomUUID()
来源：http://ckb.c1oappe.top

[U116] JS：类型检查（JSDoc）
来源：http://tpw.sysykeji.top

/** @param {string} name */ function f(name) {}
来源：http://anm.dashuyun.cn

[U117] JS：单元测试
来源：http://vnv.daria6918.cn

npm i -D vitest;  npx vitest
来源：http://bhr.fktsv.cn

[U118] JS：开发服务器
来源：http://byk.tarul.cn

npm i -D vite;  npx vite
来源：http://vnn.ybcxt.top

[U119] JS：生产构建
来源：http://gki.birdmap.top

npx vite build
来源：http://rvw.xylfe.cn

[U120] JS：读取环境变量（Vite）
来源：http://nlo.yanxiufei.cn

import.meta.env.VITE_API_URL
来源：http://mzb.gogol.net.cn

================================================================================
来源：http://aak.shuidangran.top

统计汇总
来源：http://juy.dashuyun.cn

================================================================================
来源：http://oho.316326.xyz

按语言统计（条）：
来源：http://wag.xuanzx.com

Python ......... 252
来源：http://zga.hesvh.cn

PHP ............ 252
来源：http://qxy.ydjk.org.cn

JavaScript ..... 252
来源：http://jmc.hywenlv.cn

TypeScript ..... 212
来源：http://qma.0kj1m.cn

Java ........... 212
来源：http://dak.zhongyouzk.top

Go ............. 212
来源：http://gtb.xziqi.cn

Ruby ........... 212
来源：http://jrm.tian-w.cn

C# ............. 212
来源：http://otr.hywenlv.cn

C .............. 30
来源：http://mjc.yuxming.cn

C++ ............ 30
来源：http://ana.guowangkeji.top

SQL ............ 90
来源：http://nre.havefunace.top

Bash ........... 80
来源：http://tze.xingfuxueyuan.xyz

Kotlin ......... 15
来源：http://jhp.hywenlv.cn

Swift .......... 15
来源：http://avj.redwolf501.top

Lua ............ 10
来源：http://fur.cheryme.top

Perl ........... 10
来源：http://fno.xingfuxueyuan.xyz

Scala .......... 10
来源：http://nqk.fehbvm.com

------------------------------------
来源：http://zeg.zycfv.cn

合计 ........... 2106 条
来源：http://iqw.pycfn.com

按章节统计：
来源：http://ixy.fzhhl.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zok.c1oappe.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xug.sysykeji.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jdr.fanxiaobao.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://uhq.gzhubu.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jyp.hfpthk.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zkn.gzhubu.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xvj.yangfankeji.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jaz.shuidangran.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://fmd.gzhubu.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ftf.zhoulong.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ylp.yj202588.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kwx.zycfv.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://iyl.snrcjt.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tio.shanyushiyangkeji.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://waf.nanxuanxn.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://naz.fengsongda.top

Q SQL 专题                              90
来源：http://jga.zhengqikj.top

R Bash 专题                             80
来源：http://bet.316326.xyz

S C / C++ 专题                          60
来源：http://adh.tianlin.xyz

T 其他语言补充                          60
来源：http://zfc.yangfankeji.com

U 高频实用片段                         120
来源：http://bqb.zhiwuduotai.top

------------------------------------
来源：http://txf.jinghuilouyu.cn

合计                                  2106 条
来源：http://fio.zhoulong.xyz

--------------------------------------------------------------------------------
来源：http://psl.vqdsnc.cn

使用提醒
来源：http://ikg.kuanghao11.cn

--------------------------------------------------------------------------------
来源：http://oif.sjlbkw.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://cjf.hcnkem.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://gpm.hammf.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://dbv.hnxiangtu.top

在旧版本上使用前请先确认语法支持情况。
来源：http://jol.xuetiantiany.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hzo.feifeiyinyue.top

—— 文件结束 ——
来源：http://nah.aizwys.cn

================================================================================
来源：http://nax.xylfe.cn

程序语言常见例子速查手册（2024 版）
来源：http://hev.jyoumei.cn

Common Programming Examples Cheat Book
来源：http://mha.hnxiangtu.top

================================================================================
来源：http://jjc.yongpay.top


<!-- 参考信息 -->