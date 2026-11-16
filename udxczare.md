代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://wyj.zhoulong.xyz

[T55] Scala：集合过滤
来源：http://rgz.iojbl.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ggv.shanyushiyangtech.top

[T56] Scala：样例类
来源：http://acp.havefunace.top

case class User(name: String, age: Int)
来源：http://zwx.smart0.xyz

[T57] Scala：模式匹配
来源：http://nqf.redwolf501.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://zkq.zhongyouzk.top

[T58] Scala：函数定义
来源：http://zjd.dashuyun.cn

def add(a: Int, b: Int): Int = a + b
来源：http://clq.ppjwa.cn

[T59] Scala：循环
来源：http://hrk.zdbjq.cn

for (i <- 1 to 10) println(i)
来源：http://imz.gzhubu.top

[T60] Scala：折叠
来源：http://tln.yanxiufei.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ucr.uphjek.com

================================================================================
来源：http://xuq.fehbvm.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://idh.gaohongyu789.top

================================================================================
来源：http://zae.yangfankeji.com

[U01] Py：创建虚拟环境
来源：http://uxd.daxiang520.top

python -m venv .venv && source .venv/bin/activate
来源：http://gbw.cheryme.top

[U02] Py：导出 / 安装依赖
来源：http://ucx.vqdsnc.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qwj.yj20258888.top

[U03] Py：加载 .env 配置
来源：http://wnf.fzhhl.top

from dotenv import load_dotenv; load_dotenv()
来源：http://wdv.sufxvd.cn

[U04] Py：变量调试打印
来源：http://lkc.meibo888.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rdm.uphjek.com

[U05] Py：列表去重且保序
来源：http://bxn.ywan-chungtsiang.top

list(dict.fromkeys(arr))
来源：http://qww.fehbvm.com

[U06] Py：合并两个字典
来源：http://mtm.feifeiyinyue.top

{**a, **b}
来源：http://weq.c1oappe.top

[U07] Py：反转字典键值
来源：http://dth.9152youxi.cn

{v: k for k, v in d.items()}
来源：http://akw.316326.xyz

[U08] Py：展平二维列表
来源：http://bui.dashuyun.cn

[y for x in nested for y in x]
来源：http://whd.feifeiyinyue.top

[U09] Py：字典取最大值的键
来源：http://cse.gotoacloud.top

max(d, key=d.get)
来源：http://mog.meibo888.top

[U10] Py：按值排序字典
来源：http://zwb.kuanghao11.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uzp.jinyuanbaomall.cn

[U11] Py：生成器表达式
来源：http://csd.aibaodan.cn

(x * 2 for x in arr)
来源：http://idm.shzxlz.cn

[U12] Py：取出现最多的 3 个元素
来源：http://mxn.zhengqikj.top

Counter(arr).most_common(3)
来源：http://hjy.wangdashe.top

[U13] Py：固定长度队列
来源：http://hjb.vqdsnc.cn

deque(maxlen=10)
来源：http://cxo.jinqigfzy.top

[U14] Py：分组收集到列表
来源：http://hpr.yfazqb.com

defaultdict(list)
来源：http://udu.ppjwa.cn

[U15] Py：高精度计时
来源：http://fva.ydzc1.top

t = time.perf_counter()
来源：http://zsl.aibaodan.cn

[U16] Py：命令行参数解析
来源：http://rhg.wangdashe.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pwm.fktsv.cn

[U17] Py：初始化日志
来源：http://kdg.ywan-chungtsiang.top

logging.basicConfig(level=logging.INFO)
来源：http://rad.0kj1m.cn

[U18] Py：预编译正则
来源：http://dxy.hywenlv.cn

pat = re.compile(r"\d+")
来源：http://jeu.hfpthk.cn

[U19] Py：正则替换带回调
来源：http://zfq.yonumen.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rat.sysykeji.top

[U20] Py：缓存函数结果
来源：http://ase.jqgufenzy.top

@functools.lru_cache(maxsize=None)
来源：http://jzu.cqqwz.cn

[U21] Py：自定义上下文管理器
来源：http://rvx.ehwqpu.com

@contextlib.contextmanager
来源：http://tkk.jlsjyb.cn

[U22] Py：矩阵转置
来源：http://edu.snrcjt.cn

list(zip(*m))
来源：http://fye.cheryme.top

[U23] Py：分块读取大文件
来源：http://nsp.zhixingplan.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://eln.xinyue.icu

[U24] Py：路径操作
来源：http://lgv.tarul.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://abs.feifeiyinyue.top

[U25] Py：CSV 按字典读
来源：http://ius.cqqwz.cn

csv.DictReader(f)
来源：http://ufk.mhx1999.top

[U26] Py：并发下载
来源：http://kio.ctjpmb.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://eyv.zycfv.cn

[U27] Py：异步 HTTP
来源：http://ibk.aizwys.cn

aiohttp.ClientSession() 配合 async with
来源：http://mhx.zhiwuduotai.top

[U28] Py：类型别名
来源：http://nxt.svipenyu.cn

UserId = int
来源：http://tbw.bbcook.cn

[U29] Py：属性校验
来源：http://xoe.havefunace.top

@property 与 @x.setter 配合
来源：http://gup.svipenyu.cn

[U30] Py：数据类
来源：http://whm.birdmap.top

@dataclass(slots=True)
来源：http://amw.316326.xyz

[U31] Py：单测
来源：http://dvn.xuetiantiany.cn

python -m pytest -q
来源：http://zos.ppjwa.cn

[U32] Py：代码格式化
来源：http://kvr.yuanzhike.top

ruff format . && ruff check --fix .
来源：http://bqn.gogol.net.cn

[U33] Py：打包发布
来源：http://exd.ydjk.org.cn

python -m build  （依赖 pyproject.toml）
来源：http://llz.tarul.cn

[U34] Py：判断编码
来源：http://arn.xziqi.cn

chardet.detect(raw)
来源：http://wiy.jinyuanbaomall.cn

[U35] Py：发送邮件
来源：http://hoz.jinyuanbaomall.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mcj.zdbjq.cn

[U36] Py：定时任务
来源：http://cyh.zhaomingkeji.xyz

schedule.every(10).minutes.do(job)
来源：http://ltk.cashguo.top

[U37] Py：读写 Excel
来源：http://lrr.sysykeji.top

pandas.read_excel / DataFrame.to_excel
来源：http://gcr.yanxiufei.cn

[U38] Py：获取脚本所在目录
来源：http://hls.jyoumei.cn

Path(__file__).resolve().parent
来源：http://uqc.yfazqb.com

[U39] Py：判断是否在交互环境
来源：http://fdk.gotoacloud.top

sys.stdout.isatty()
来源：http://zpx.yueranfly.top

[U40] Py：打印到标准错误
来源：http://xal.hfpthk.cn

print("err", file=sys.stderr)
来源：http://qwx.tanke756.top

[U41] PHP：初始化 Composer 项目
来源：http://qxg.sjlbkw.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://lbl.yueranfly.top

[U42] PHP：PSR-4 自动加载
来源：http://mnl.hesvh.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zot.vqdsnc.cn

[U43] PHP：声明命名空间
来源：http://wed.cqqwz.cn

namespace App\Http;
来源：http://bap.andypj.xyz

[U44] PHP：开启严格类型
来源：http://hpa.fengsongda.top

declare(strict_types=1);
来源：http://xuu.zdbjq.cn

[U45] PHP：类型声明与返回类型
来源：http://eaa.chenjidiqi.icu

function add(int $a, int $b): int { return $a + $b; }
来源：http://isb.shzxlz.cn

[U46] PHP：可空类型
来源：http://ira.aibaodan.cn

?string $name = null
来源：http://atu.gogol.net.cn

[U47] PHP：联合类型
来源：http://vxl.jiagoushi.top

int|string $id
来源：http://ors.svipenyu.cn

[U48] PHP：纯枚举
来源：http://tvc.sjlbkw.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wwh.ybcxt.top

[U49] PHP：只读属性
来源：http://tuj.tanke756.top

public readonly string $name
来源：http://obl.hcnkem.com

[U50] PHP：构造器属性提升
来源：http://hxh.birdmap.top

public function __construct(private int $id) {}
来源：http://mqk.pycfn.com

[U51] PHP：数组解构
来源：http://eaq.havefunace.top

[$a, $b] = $arr;
来源：http://lvz.vqdsnc.cn

[U52] PHP：箭头函数
来源：http://rqr.xylfe.cn

$double = fn($x) => $x * 2;
来源：http://wvo.hysaishi.cn

[U53] PHP：空合并运算符
来源：http://guc.jlsjyb.cn

$v = $a ?? $b ?? "default";
来源：http://dlg.jinyuanbaomall.cn

[U54] PHP：空安全调用
来源：http://ubz.gogol.net.cn

$obj?->method()
来源：http://eda.jinghuilouyu.cn

[U55] PHP：match 表达式
来源：http://jqf.yuxming.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yny.jinqigfzy.top

[U56] PHP：命名参数
来源：http://rvk.snrcjt.cn

f(a: 1, b: 2)
来源：http://yks.ydjk.org.cn

[U57] PHP：字符串插值
来源：http://xsu.zycfv.cn

"值: {$a}"
来源：http://hzb.zdbjq.cn

[U58] PHP：数组三件套
来源：http://cop.jyoumei.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mgh.haohaochexian.top

[U59] PHP：自定义排序
来源：http://ict.yueranfly.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fui.hesvh.cn

[U60] PHP：JSON 编解码
来源：http://hzd.gotoacloud.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ulx.0kj1m.cn

[U61] PHP：正则
来源：http://bpt.hnqzz.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mso.chenzaomai.com

[U62] PHP：日期对象
来源：http://ucb.cdnleiting.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bzl.jinqigufen.top

[U63] PHP：文件读写
来源：http://dqe.cheryme.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bof.chenlongwang.top

[U64] PHP：目录遍历
来源：http://wil.gzhubu.top

glob("dir/*.php");  scandir("dir");
来源：http://jio.ppjwa.cn

[U65] PHP：会话
来源：http://tab.gogol.net.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://hgw.xuetiantiany.cn

[U66] PHP：设置 Cookie
来源：http://cbh.fengsongda.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://uyz.nwbrower.top

[U67] PHP：处理文件上传
来源：http://lyh.xingfuxueyuan.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://foi.zhiwuduotai.top

[U68] PHP：PDO 连接
来源：http://rnq.cheryme.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jyl.yangfankeji.com

[U69] PHP：PDO 预处理
来源：http://hgz.sweek.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vwi.guowangkeji.top

[U70] PHP：PDO 事务
来源：http://xpq.xylfe.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://uuf.sysykeji.top

[U71] PHP：抛出异常
来源：http://ctx.jqgfzy.top

throw new RuntimeException("失败", 500);
来源：http://jmd.daria6918.cn

[U72] PHP：写错误日志
来源：http://idu.cashguo.top

error_log("失败: " . $e->getMessage());
来源：http://fzq.ybcxt.top

[U73] PHP：读取 ini 配置
来源：http://pqu.iojbl.cn

parse_ini_file("config.ini", true)
来源：http://vfq.ydzc1.top

[U74] PHP：读取环境变量
来源：http://mem.hammf.cn

getenv("APP_ENV") ?: "production"
来源：http://vns.jinqigufen.top

[U75] PHP：依赖注入
来源：http://tum.haohaochexian.top

composer require psr/container
来源：http://eya.iojbl.cn

[U76] PHP：简单路由
来源：http://eeg.jianghu66.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zbt.pengpengdd.cyou

[U77] PHP：模板渲染
来源：http://fbi.iojbl.cn

composer require twig/twig
来源：http://itl.svipenyu.cn

[U78] PHP：单元测试
来源：http://ijc.xinyue.icu

composer require --dev phpunit/phpunit
来源：http://inu.chenjidiqi.icu

[U79] PHP：静态分析
来源：http://osi.yanxiufei.cn

composer require --dev phpstan/phpstan
来源：http://pkv.nanxuanxn.top

[U80] PHP：代码规范修复
来源：http://atl.havefunace.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://nlz.shzxlz.cn

[U81] JS：初始化项目
来源：http://hlt.cucudq.cn

npm init -y;  npm i express
来源：http://bgr.hongshengwenyu.top

[U82] JS：package.json 脚本
来源：http://qgf.aizwys.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gfm.gotoacloud.top

[U83] JS：ES Module 导入导出
来源：http://xls.zhixingplan.top

export const a = 1;  import { a } from "./m.js";
来源：http://wah.yueranfly.top

[U84] JS：CommonJS 写法
来源：http://oju.zhixingplan.top

module.exports = { a };  const { a } = require("./m");
来源：http://qyv.zhaomingkeji.xyz

[U85] JS：可选链
来源：http://pit.ivvv.top

a?.b?.c
来源：http://jyd.0kj1m.cn

[U86] JS：空值合并
来源：http://dcd.zycfv.cn

a ?? b
来源：http://otx.hnqzz.top

[U87] JS：解构默认值
来源：http://xsv.epnwcf.com

const { a = 1, b = 2 } = obj;
来源：http://rmj.jinqigfzy.top

[U88] JS：对象展开合并
来源：http://tnk.fengsongda.top

{ ...a, ...b }
来源：http://pxm.0kj1m.cn

[U89] JS：数组去重
来源：http://pwc.fzhhl.top

[...new Set(arr)]
来源：http://ehl.jinqigfzy.top

[U90] JS：数字数组排序
来源：http://cao.tian-w.cn

[...arr].sort((a, b) => a - b)
来源：http://leg.nwbrower.top

[U91] JS：对象键值遍历
来源：http://juk.snrcjt.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lht.aizwys.cn

[U92] JS：深拷贝
来源：http://qoe.aizwys.cn

structuredClone(obj)
来源：http://yaw.shuidangran.top

[U93] JS：模板字符串
来源：http://slz.gotoacloud.top

`共 ${n} 条`
来源：http://vnq.jqgfzy.top

[U94] JS：箭头函数
来源：http://ngl.cheryme.top

const double = x => x * 2;
来源：http://gpu.shzxlz.cn

[U95] JS：Promise 包装
来源：http://rxq.bjfxy.top

new Promise((resolve, reject) => {})
来源：http://mba.vehdjk.com

[U96] JS：async/await 与异常
来源：http://jxk.cqqwz.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ysa.daxiang520.top

[U97] JS：并发请求
来源：http://xjf.havefunace.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://pop.cashguo.top

[U98] JS：fetch 带 JSON
来源：http://diz.fzhhl.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cka.wangdashe.top

[U99] JS：事件监听
来源：http://ehi.0kj1m.cn

el.addEventListener("click", e => {})
来源：http://ckx.gaohongyu789.top

[U100] JS：DOM 查询
来源：http://wes.svipenyu.cn

document.querySelector(".item")
来源：http://vev.yvedp.cn

[U101] JS：classList 操作
来源：http://gug.zhiwuduotai.top

el.classList.toggle("active")
来源：http://ktr.kuanghao11.cn

[U102] JS：本地存储
来源：http://kzs.birdmap.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://cqs.smart0.xyz

[U103] JS：定时器
来源：http://gpf.sweek.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ftg.xinyue.icu

[U104] JS：防抖
来源：http://ryr.smart0.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dzr.ywan-chungtsiang.top

[U105] JS：节流
来源：http://azs.zdqjudy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://aaw.jinqigufen.top

[U106] JS：日期格式化
来源：http://hpf.sysykeji.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dbh.jyoumei.cn

[U107] JS：数字千分位
来源：http://wqr.svipenyu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mpx.9152youxi.cn

[U108] JS：随机整数
来源：http://msg.vehdjk.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xxe.meibo888.top

[U109] JS：数组分组
来源：http://ysk.ctjpmb.com

Object.groupBy(arr, x => x.type)
来源：http://uzd.hysaishi.cn

[U110] JS：数组分块
来源：http://lqc.yuxming.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://szd.xuanzx.com

[U111] JS：对象转 Map
来源：http://gbq.tianlin.xyz

new Map(Object.entries(obj))
来源：http://yjq.zhaomingkeji.xyz

[U112] JS：字符串补位
来源：http://fxe.sweek.top

"7".padStart(3, "0")
来源：http://ygd.svipenyu.cn

[U113] JS：正则替换全部
来源：http://bdi.chenzaomai.com

s.replaceAll("a", "b")
来源：http://aek.zycfv.cn

[U114] JS：JSON 深比较
来源：http://dma.bbcook.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://pfp.vehdjk.com

[U115] JS：生成 UUID
来源：http://bim.ydjk.org.cn

crypto.randomUUID()
来源：http://rfb.vqdsnc.cn

[U116] JS：类型检查（JSDoc）
来源：http://jjq.ydzc1.top

/** @param {string} name */ function f(name) {}
来源：http://emg.fengsongda.top

[U117] JS：单元测试
来源：http://ujc.shzxlz.cn

npm i -D vitest;  npx vitest
来源：http://ylp.c1oappe.top

[U118] JS：开发服务器
来源：http://wdp.meibo888.top

npm i -D vite;  npx vite
来源：http://fsa.daxiang520.top

[U119] JS：生产构建
来源：http://ozq.fehbvm.com

npx vite build
来源：http://xaa.cqqwz.cn

[U120] JS：读取环境变量（Vite）
来源：http://jhe.zhiwuduotai.top

import.meta.env.VITE_API_URL
来源：http://eoy.sysykeji.top

================================================================================
来源：http://zsz.hammf.cn

统计汇总
来源：http://kwj.bbcook.cn

================================================================================
来源：http://gjy.guannengcc.top

按语言统计（条）：
来源：http://vgz.gzhubu.top

Python ......... 252
来源：http://etr.fanxiaobao.xyz

PHP ............ 252
来源：http://kij.yueranfly.top

JavaScript ..... 252
来源：http://oby.shzxlz.cn

TypeScript ..... 212
来源：http://ujk.quarkkingdee.top

Java ........... 212
来源：http://prh.jiagoushi.top

Go ............. 212
来源：http://acb.xziqi.cn

Ruby ........... 212
来源：http://kjx.hesvh.cn

C# ............. 212
来源：http://wjt.hysaishi.cn

C .............. 30
来源：http://pyx.ydzc1.top

C++ ............ 30
来源：http://qot.zycfv.cn

SQL ............ 90
来源：http://eua.guowangkeji.top

Bash ........... 80
来源：http://ikd.yj20258.top

Kotlin ......... 15
来源：http://pvq.bbcook.cn

Swift .......... 15
来源：http://trp.jiagoushi.top

Lua ............ 10
来源：http://jfy.fengsongda.top

Perl ........... 10
来源：http://pdy.redwolf501.top

Scala .......... 10
来源：http://lzx.gotoacloud.top

------------------------------------
来源：http://tjk.smart0.xyz

合计 ........... 2106 条
来源：http://upj.hnqzz.top

按章节统计：
来源：http://wkq.wangshuangyany.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zrt.xinyue.icu

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tup.shanyushiyangkeji.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ksa.jinghuilouyu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://iap.tian-w.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://axy.sufxvd.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://uoy.shzxlz.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://eaf.fktsv.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jpu.svipenyu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://sqa.hcnkem.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qgh.vehdjk.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kuu.shanyushiyangkeji.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wit.fengsongda.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://uxv.316326.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://bcm.chenjidiqi.icu

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ndb.dashuyun.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://fpk.xingfuxueyuan.xyz

Q SQL 专题                              90
来源：http://ilf.hnqzz.top

R Bash 专题                             80
来源：http://dym.tarul.cn

S C / C++ 专题                          60
来源：http://tls.jlsjyb.cn

T 其他语言补充                          60
来源：http://wih.cdnleiting.top


<!-- 参考信息 -->