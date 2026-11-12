代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://vtx.hnxiangtu.top

[T59] Scala：循环
来源：http://bys.xuanzx.com

for (i <- 1 to 10) println(i)
来源：http://kzo.daria6918.cn

[T60] Scala：折叠
来源：http://yjq.chenzaomai.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zgj.sxryk.cn

================================================================================
来源：http://soa.zhongyouzk.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://sfk.xziqi.cn

================================================================================
来源：http://mqb.pengpengdd.cyou

[U01] Py：创建虚拟环境
来源：http://yjq.shanyushiyangtech.top

python -m venv .venv && source .venv/bin/activate
来源：http://upl.yj20258888.top

[U02] Py：导出 / 安装依赖
来源：http://ccl.ppjwa.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cmi.epnwcf.com

[U03] Py：加载 .env 配置
来源：http://oio.smart0.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://qwp.yuxming.cn

[U04] Py：变量调试打印
来源：http://tls.ehwqpu.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xwk.quarkkingdee.top

[U05] Py：列表去重且保序
来源：http://fhm.cheryme.top

list(dict.fromkeys(arr))
来源：http://gyh.quarkkingdee.top

[U06] Py：合并两个字典
来源：http://bnl.jqgfzy.top

{**a, **b}
来源：http://akj.shuidangran.top

[U07] Py：反转字典键值
来源：http://vau.zhiwuduotai.top

{v: k for k, v in d.items()}
来源：http://xuq.yanxiufei.cn

[U08] Py：展平二维列表
来源：http://zrl.gzhubu.top

[y for x in nested for y in x]
来源：http://sto.fanxiaobao.xyz

[U09] Py：字典取最大值的键
来源：http://nxs.gogol.net.cn

max(d, key=d.get)
来源：http://zrg.jianghu66.top

[U10] Py：按值排序字典
来源：http://ckr.epnwcf.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lbv.yongpay.top

[U11] Py：生成器表达式
来源：http://pus.bjfxy.top

(x * 2 for x in arr)
来源：http://pox.xziqi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://jqr.gogol.net.cn

Counter(arr).most_common(3)
来源：http://bxv.hywenlv.cn

[U13] Py：固定长度队列
来源：http://czi.316326.xyz

deque(maxlen=10)
来源：http://aqb.kuanghao11.cn

[U14] Py：分组收集到列表
来源：http://jcz.meibo888.top

defaultdict(list)
来源：http://wcc.yj20258888.top

[U15] Py：高精度计时
来源：http://zlm.tanke756.top

t = time.perf_counter()
来源：http://zjt.cdnleiting.top

[U16] Py：命令行参数解析
来源：http://apl.nanxuanxn.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xjp.vqdsnc.cn

[U17] Py：初始化日志
来源：http://ynq.316326.xyz

logging.basicConfig(level=logging.INFO)
来源：http://cfe.ywan-chungtsiang.top

[U18] Py：预编译正则
来源：http://qow.jyoumei.cn

pat = re.compile(r"\d+")
来源：http://hol.gotoacloud.top

[U19] Py：正则替换带回调
来源：http://qnx.tianlin.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hli.9152youxi.cn

[U20] Py：缓存函数结果
来源：http://uqb.ydjk.org.cn

@functools.lru_cache(maxsize=None)
来源：http://wsc.jlsjyb.cn

[U21] Py：自定义上下文管理器
来源：http://bbs.haohaochexian.top

@contextlib.contextmanager
来源：http://vmq.bjfxy.top

[U22] Py：矩阵转置
来源：http://mrq.zhengqikj.top

list(zip(*m))
来源：http://eyn.hcnkem.com

[U23] Py：分块读取大文件
来源：http://wim.hywenlv.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xbd.316326.xyz

[U24] Py：路径操作
来源：http://irk.tianlin.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://uqw.jyoumei.cn

[U25] Py：CSV 按字典读
来源：http://hhp.shanyushiyangtech.top

csv.DictReader(f)
来源：http://wlb.nanxinkj.top

[U26] Py：并发下载
来源：http://dyr.shanyushiyangkeji.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xan.ydjk.org.cn

[U27] Py：异步 HTTP
来源：http://hls.wangdashe.top

aiohttp.ClientSession() 配合 async with
来源：http://itt.ppjwa.cn

[U28] Py：类型别名
来源：http://gvt.yonumen.top

UserId = int
来源：http://lyj.aizwys.cn

[U29] Py：属性校验
来源：http://ueg.jyoumei.cn

@property 与 @x.setter 配合
来源：http://efx.zhengqikj.top

[U30] Py：数据类
来源：http://rws.nanxuanxn.top

@dataclass(slots=True)
来源：http://ttb.zdbjq.cn

[U31] Py：单测
来源：http://aef.hcnkem.com

python -m pytest -q
来源：http://gub.zhengqikj.top

[U32] Py：代码格式化
来源：http://frh.redwolf501.top

ruff format . && ruff check --fix .
来源：http://lld.pycfn.com

[U33] Py：打包发布
来源：http://wvr.vqdsnc.cn

python -m build  （依赖 pyproject.toml）
来源：http://fpp.vehdjk.com

[U34] Py：判断编码
来源：http://mes.havefunace.top

chardet.detect(raw)
来源：http://eas.fehbvm.com

[U35] Py：发送邮件
来源：http://gjm.cdnleiting.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wzz.ywan-chungtsiang.top

[U36] Py：定时任务
来源：http://rxx.quarkkingdee.top

schedule.every(10).minutes.do(job)
来源：http://mhj.ehwqpu.com

[U37] Py：读写 Excel
来源：http://ejx.jianghu66.top

pandas.read_excel / DataFrame.to_excel
来源：http://cyt.nanxuanxn.top

[U38] Py：获取脚本所在目录
来源：http://yaa.jlsjyb.cn

Path(__file__).resolve().parent
来源：http://vhy.wangshuangyany.cn

[U39] Py：判断是否在交互环境
来源：http://fyx.jiagoushi.top

sys.stdout.isatty()
来源：http://bpj.bjfxy.top

[U40] Py：打印到标准错误
来源：http://fgn.ydzc1.top

print("err", file=sys.stderr)
来源：http://tli.ivvv.top

[U41] PHP：初始化 Composer 项目
来源：http://oxp.ywan-chungtsiang.top

composer init;  composer require guzzlehttp/guzzle
来源：http://qdr.wangshuangyany.cn

[U42] PHP：PSR-4 自动加载
来源：http://ria.meibo888.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dqg.ywan-chungtsiang.top

[U43] PHP：声明命名空间
来源：http://kbl.gogol.net.cn

namespace App\Http;
来源：http://gag.yj20258888.top

[U44] PHP：开启严格类型
来源：http://wbw.hnxiangtu.top

declare(strict_types=1);
来源：http://kor.uphjek.com

[U45] PHP：类型声明与返回类型
来源：http://kfs.yuxming.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://mge.yangfankeji.com

[U46] PHP：可空类型
来源：http://gnp.yongpay.top

?string $name = null
来源：http://xqq.cashguo.top

[U47] PHP：联合类型
来源：http://ngb.yuanzhike.top

int|string $id
来源：http://uqy.ydzc1.top

[U48] PHP：纯枚举
来源：http://wfx.wangshuangyany.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vvh.bjfxy.top

[U49] PHP：只读属性
来源：http://jmg.ivvv.top

public readonly string $name
来源：http://yah.mhx1999.top

[U50] PHP：构造器属性提升
来源：http://zqu.hammf.cn

public function __construct(private int $id) {}
来源：http://gwk.svipenyu.cn

[U51] PHP：数组解构
来源：http://had.guannengcc.top

[$a, $b] = $arr;
来源：http://dbl.9152youxi.cn

[U52] PHP：箭头函数
来源：http://fmd.jlsjyb.cn

$double = fn($x) => $x * 2;
来源：http://nhr.zhijiandao.cn

[U53] PHP：空合并运算符
来源：http://iqo.316326.xyz

$v = $a ?? $b ?? "default";
来源：http://gne.yuxming.cn

[U54] PHP：空安全调用
来源：http://awe.yj20258.top

$obj?->method()
来源：http://sqj.shzxlz.cn

[U55] PHP：match 表达式
来源：http://ptd.feifeiyinyue.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://cnt.yangfankeji.com

[U56] PHP：命名参数
来源：http://rua.xuanzx.com

f(a: 1, b: 2)
来源：http://tyb.epnwcf.com

[U57] PHP：字符串插值
来源：http://rbw.hnxiangtu.top

"值: {$a}"
来源：http://tog.bbcook.cn

[U58] PHP：数组三件套
来源：http://cul.xylfe.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vue.nanxinkj.top

[U59] PHP：自定义排序
来源：http://kbv.feifeiyinyue.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yro.yfazqb.com

[U60] PHP：JSON 编解码
来源：http://hxh.ybcxt.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xki.ivvv.top

[U61] PHP：正则
来源：http://shc.vehdjk.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ppf.fanxiaobao.xyz

[U62] PHP：日期对象
来源：http://jsu.wangshuangyany.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ybh.zhoulong.xyz

[U63] PHP：文件读写
来源：http://dyk.zdqjudy.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gxa.yj20258888.top

[U64] PHP：目录遍历
来源：http://wrx.snrcjt.cn

glob("dir/*.php");  scandir("dir");
来源：http://ing.tianlin.xyz

[U65] PHP：会话
来源：http://uwg.fehbvm.com

session_start();  $_SESSION["uid"] = 1;
来源：http://vym.chenlongwang.top

[U66] PHP：设置 Cookie
来源：http://afz.yuxming.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mha.bjfxy.top

[U67] PHP：处理文件上传
来源：http://aps.dashuyun.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://txy.316326.xyz

[U68] PHP：PDO 连接
来源：http://rvg.dianchejie.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://dfw.zdbjq.cn

[U69] PHP：PDO 预处理
来源：http://fci.jiagoushi.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lnl.jianghu66.top

[U70] PHP：PDO 事务
来源：http://noi.hesvh.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xfn.cdnleiting.top

[U71] PHP：抛出异常
来源：http://okl.yuxming.cn

throw new RuntimeException("失败", 500);
来源：http://ufl.shanyushiyangtech.top

[U72] PHP：写错误日志
来源：http://flj.jinqigfzy.top

error_log("失败: " . $e->getMessage());
来源：http://dvk.nwbrower.top

[U73] PHP：读取 ini 配置
来源：http://jsg.jianghu66.top

parse_ini_file("config.ini", true)
来源：http://qrg.meibo888.top

[U74] PHP：读取环境变量
来源：http://sqh.hfpthk.cn

getenv("APP_ENV") ?: "production"
来源：http://wig.zhengqikj.top

[U75] PHP：依赖注入
来源：http://hax.tianlin.xyz

composer require psr/container
来源：http://vzg.redwolf501.top

[U76] PHP：简单路由
来源：http://vcz.nwbrower.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gbw.guowangkeji.top

[U77] PHP：模板渲染
来源：http://xvx.mhx1999.top

composer require twig/twig
来源：http://xyg.jianghu66.top

[U78] PHP：单元测试
来源：http://rka.zhaomingkeji.xyz

composer require --dev phpunit/phpunit
来源：http://mnj.shangyingyoupin.top

[U79] PHP：静态分析
来源：http://kqf.redwolf501.top

composer require --dev phpstan/phpstan
来源：http://mrg.andypj.xyz

[U80] PHP：代码规范修复
来源：http://qoz.jqgfzy.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://scm.ppjwa.cn

[U81] JS：初始化项目
来源：http://eiu.zdbjq.cn

npm init -y;  npm i express
来源：http://ntt.ivvv.top

[U82] JS：package.json 脚本
来源：http://esu.daria6918.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vfx.mhx1999.top

[U83] JS：ES Module 导入导出
来源：http://uqe.52xcode.cn

export const a = 1;  import { a } from "./m.js";
来源：http://uyd.gzhubu.top

[U84] JS：CommonJS 写法
来源：http://ugx.hongshengwenyu.top

module.exports = { a };  const { a } = require("./m");
来源：http://two.tanke756.top

[U85] JS：可选链
来源：http://jdt.jlsjyb.cn

a?.b?.c
来源：http://lqt.daxiang520.top

[U86] JS：空值合并
来源：http://nxo.9152youxi.cn

a ?? b
来源：http://pwn.yuanzhike.top

[U87] JS：解构默认值
来源：http://eky.nwbrower.top

const { a = 1, b = 2 } = obj;
来源：http://yzy.jinyuanbaomall.cn

[U88] JS：对象展开合并
来源：http://gpc.mhx1999.top

{ ...a, ...b }
来源：http://bdg.hnxiangtu.top

[U89] JS：数组去重
来源：http://chm.hammf.cn

[...new Set(arr)]
来源：http://kbb.yuxming.cn

[U90] JS：数字数组排序
来源：http://nbu.shanyushiyangtech.top

[...arr].sort((a, b) => a - b)
来源：http://bok.hesvh.cn

[U91] JS：对象键值遍历
来源：http://ler.jyoumei.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://yjg.316326.xyz

[U92] JS：深拷贝
来源：http://xxi.jinyuanbaomall.cn

structuredClone(obj)
来源：http://qrq.yfazqb.com

[U93] JS：模板字符串
来源：http://pul.zhixingplan.top

`共 ${n} 条`
来源：http://qji.daxiang520.top

[U94] JS：箭头函数
来源：http://xvg.mhx1999.top

const double = x => x * 2;
来源：http://agl.yonumen.top

[U95] JS：Promise 包装
来源：http://mcq.chenjidiqi.icu

new Promise((resolve, reject) => {})
来源：http://alf.kuanghao11.cn

[U96] JS：async/await 与异常
来源：http://egt.kuanghao11.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xfs.guowangkeji.top

[U97] JS：并发请求
来源：http://dij.ppjwa.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://bhl.uphjek.com

[U98] JS：fetch 带 JSON
来源：http://yam.haohaochexian.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mmx.cdnleiting.top

[U99] JS：事件监听
来源：http://typ.zdqjudy.top

el.addEventListener("click", e => {})
来源：http://jjx.xziqi.cn

[U100] JS：DOM 查询
来源：http://dew.gzhubu.top

document.querySelector(".item")
来源：http://nfp.yongpay.top

[U101] JS：classList 操作
来源：http://wiq.shangyingyoupin.top

el.classList.toggle("active")
来源：http://esi.hcnkem.com

[U102] JS：本地存储
来源：http://tft.ybcxt.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://rlm.kuanghao11.cn

[U103] JS：定时器
来源：http://qxc.ivvv.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://usv.shzxlz.cn

[U104] JS：防抖
来源：http://kte.ybcxt.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ahh.jianghu66.top

[U105] JS：节流
来源：http://zkr.vqdsnc.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cny.guannengcc.top

[U106] JS：日期格式化
来源：http://cuj.yongpay.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kyi.yonumen.top

[U107] JS：数字千分位
来源：http://kix.gzhubu.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jwt.kuanghao11.cn

[U108] JS：随机整数
来源：http://dlg.0kj1m.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mrt.birdmap.top

[U109] JS：数组分组
来源：http://oak.feifeiyinyue.top

Object.groupBy(arr, x => x.type)
来源：http://itt.cdnleiting.top

[U110] JS：数组分块
来源：http://iwe.52xcode.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rsl.yonumen.top

[U111] JS：对象转 Map
来源：http://pmw.snrcjt.cn

new Map(Object.entries(obj))
来源：http://bzp.andypj.xyz

[U112] JS：字符串补位
来源：http://sen.cheryme.top

"7".padStart(3, "0")
来源：http://tuo.yuanzhike.top

[U113] JS：正则替换全部
来源：http://ynt.ydjk.org.cn

s.replaceAll("a", "b")
来源：http://nio.chenjidiqi.icu

[U114] JS：JSON 深比较
来源：http://yuf.jinghuilouyu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://qpd.chenlongwang.top

[U115] JS：生成 UUID
来源：http://jgs.cdnleiting.top

crypto.randomUUID()
来源：http://loz.zhongyouzk.top

[U116] JS：类型检查（JSDoc）
来源：http://imr.sxryk.cn

/** @param {string} name */ function f(name) {}
来源：http://qnb.gaohongyu789.top

[U117] JS：单元测试
来源：http://cub.fktsv.cn

npm i -D vitest;  npx vitest
来源：http://mbr.chenlongwang.top

[U118] JS：开发服务器
来源：http://hzu.haohaochexian.top

npm i -D vite;  npx vite
来源：http://eed.feifeiyinyue.top

[U119] JS：生产构建
来源：http://ncr.andypj.xyz

npx vite build
来源：http://ata.yj20258.top

[U120] JS：读取环境变量（Vite）
来源：http://soe.yuanzhike.top

import.meta.env.VITE_API_URL
来源：http://bee.gzhubu.top

================================================================================
来源：http://jgg.daria6918.cn

统计汇总
来源：http://ztp.cheryme.top

================================================================================
来源：http://ony.jianghu66.top

按语言统计（条）：
来源：http://tzf.bbcook.cn

Python ......... 252
来源：http://stk.chenlongwang.top

PHP ............ 252
来源：http://apj.yongpay.top

JavaScript ..... 252
来源：http://ldj.guannengcc.top

TypeScript ..... 212
来源：http://cdu.c1oappe.top

Java ........... 212
来源：http://yik.zhongyouzk.top

Go ............. 212
来源：http://rdp.jinqigufen.top

Ruby ........... 212
来源：http://axb.xingfuxueyuan.xyz

C# ............. 212
来源：http://esn.bbcook.cn

C .............. 30
来源：http://uwj.jinyuanbaomall.cn

C++ ............ 30
来源：http://wyc.birdmap.top

SQL ............ 90
来源：http://yfu.hammf.cn

Bash ........... 80
来源：http://dph.guannengcc.top

Kotlin ......... 15
来源：http://ujc.9152youxi.cn

Swift .......... 15
来源：http://obt.hcnkem.com

Lua ............ 10
来源：http://naq.ydzc1.top

Perl ........... 10
来源：http://kkg.xziqi.cn

Scala .......... 10
来源：http://acj.yuxming.cn

------------------------------------
来源：http://zvl.ctjpmb.com

合计 ........... 2106 条
来源：http://dha.haohaochexian.top

按章节统计：
来源：http://qpl.zycfv.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xte.jiagoushi.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wju.feifeiyinyue.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xym.kuanghao11.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://nqa.shanyushiyangkeji.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://swn.redwolf501.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://cdj.gotoacloud.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nqe.9152youxi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://urx.jianghu66.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://esl.zhixingplan.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zsu.wangdashe.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bdp.shzxlz.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wtr.pycfn.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://uqg.aibaodan.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://gku.feifeiyinyue.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://xbt.xuanzx.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wpl.yvedp.cn

Q SQL 专题                              90
来源：http://pws.pengpengdd.cyou

R Bash 专题                             80
来源：http://rnt.yuanzhike.top

S C / C++ 专题                          60
来源：http://ann.chenlongwang.top

T 其他语言补充                          60
来源：http://ouk.daria6918.cn

U 高频实用片段                         120
来源：http://qal.wangdashe.top

------------------------------------
来源：http://pyb.cheryme.top

合计                                  2106 条
来源：http://gif.shzxlz.cn

--------------------------------------------------------------------------------
来源：http://dvi.shzxlz.cn

使用提醒
来源：http://fds.haohaochexian.top

--------------------------------------------------------------------------------
来源：http://sbe.bjfxy.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://pin.nanxuanxn.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://pkw.yanxiufei.cn


<!-- 参考信息 -->