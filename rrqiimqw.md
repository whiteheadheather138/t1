代发 wailian999

case class User(name: String, age: Int)
来源：http://hnu.gaohongyu789.top

[T57] Scala：模式匹配
来源：http://zjy.c1oappe.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://sfu.xuanzx.com

[T58] Scala：函数定义
来源：http://anq.hesvh.cn

def add(a: Int, b: Int): Int = a + b
来源：http://cpt.aizwys.cn

[T59] Scala：循环
来源：http://doa.hcnkem.com

for (i <- 1 to 10) println(i)
来源：http://ykm.yonumen.top

[T60] Scala：折叠
来源：http://mpc.yj20258888.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tkh.yj202588.top

================================================================================
来源：http://rwa.zdbjq.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://thk.nanxinkj.top

================================================================================
来源：http://sgb.yongpay.top

[U01] Py：创建虚拟环境
来源：http://iqr.redwolf501.top

python -m venv .venv && source .venv/bin/activate
来源：http://fqg.kuanghao11.cn

[U02] Py：导出 / 安装依赖
来源：http://cyb.yuxming.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gud.fktsv.cn

[U03] Py：加载 .env 配置
来源：http://nig.zdbjq.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://qra.jiagoushi.top

[U04] Py：变量调试打印
来源：http://wmc.jinyuanbaomall.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wvp.smart0.xyz

[U05] Py：列表去重且保序
来源：http://fuq.yj20258888.top

list(dict.fromkeys(arr))
来源：http://dya.zhaomingkeji.xyz

[U06] Py：合并两个字典
来源：http://eua.zhengqikj.top

{**a, **b}
来源：http://ylz.mhx1999.top

[U07] Py：反转字典键值
来源：http://arv.jinqigufen.top

{v: k for k, v in d.items()}
来源：http://imy.snrcjt.cn

[U08] Py：展平二维列表
来源：http://iwt.sysykeji.top

[y for x in nested for y in x]
来源：http://uys.chenlongwang.top

[U09] Py：字典取最大值的键
来源：http://dkg.xuanzx.com

max(d, key=d.get)
来源：http://rkh.yvedp.cn

[U10] Py：按值排序字典
来源：http://wra.pengpengdd.cyou

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://eok.tianlin.xyz

[U11] Py：生成器表达式
来源：http://bob.hongshengwenyu.top

(x * 2 for x in arr)
来源：http://jbm.pycfn.com

[U12] Py：取出现最多的 3 个元素
来源：http://cpj.redwolf501.top

Counter(arr).most_common(3)
来源：http://xpt.havefunace.top

[U13] Py：固定长度队列
来源：http://lib.dianchejie.cn

deque(maxlen=10)
来源：http://xha.tarul.cn

[U14] Py：分组收集到列表
来源：http://vqt.aizwys.cn

defaultdict(list)
来源：http://ztn.yongpay.top

[U15] Py：高精度计时
来源：http://vxx.birdmap.top

t = time.perf_counter()
来源：http://inr.zhixingplan.top

[U16] Py：命令行参数解析
来源：http://gpm.aibaodan.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bul.ybcxt.top

[U17] Py：初始化日志
来源：http://dwb.zhoulong.xyz

logging.basicConfig(level=logging.INFO)
来源：http://luf.hfpthk.cn

[U18] Py：预编译正则
来源：http://cpz.wangdashe.top

pat = re.compile(r"\d+")
来源：http://gvw.dianchejie.cn

[U19] Py：正则替换带回调
来源：http://rdb.hcnkem.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sep.cashguo.top

[U20] Py：缓存函数结果
来源：http://oum.chenlongwang.top

@functools.lru_cache(maxsize=None)
来源：http://gfs.redwolf501.top

[U21] Py：自定义上下文管理器
来源：http://xli.zdbjq.cn

@contextlib.contextmanager
来源：http://qrx.zdqjudy.top

[U22] Py：矩阵转置
来源：http://pyp.zhongyouzk.top

list(zip(*m))
来源：http://mql.jyoumei.cn

[U23] Py：分块读取大文件
来源：http://ozj.52xcode.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nzq.daria6918.cn

[U24] Py：路径操作
来源：http://tqh.cqqwz.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rog.jiagoushi.top

[U25] Py：CSV 按字典读
来源：http://cml.tarul.cn

csv.DictReader(f)
来源：http://avp.sufxvd.cn

[U26] Py：并发下载
来源：http://cqi.wangshuangyany.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://scx.fengsongda.top

[U27] Py：异步 HTTP
来源：http://jjf.havefunace.top

aiohttp.ClientSession() 配合 async with
来源：http://vfg.yuanzhike.top

[U28] Py：类型别名
来源：http://xfr.chenlongwang.top

UserId = int
来源：http://mim.zhaomingkeji.xyz

[U29] Py：属性校验
来源：http://edc.cashguo.top

@property 与 @x.setter 配合
来源：http://ppf.aibaodan.cn

[U30] Py：数据类
来源：http://yzk.hnxiangtu.top

@dataclass(slots=True)
来源：http://lqp.xuetiantiany.cn

[U31] Py：单测
来源：http://ern.sjlbkw.cn

python -m pytest -q
来源：http://jtk.pengpengdd.cyou

[U32] Py：代码格式化
来源：http://byb.guowangkeji.top

ruff format . && ruff check --fix .
来源：http://hbm.smart0.xyz

[U33] Py：打包发布
来源：http://vdd.haohaochexian.top

python -m build  （依赖 pyproject.toml）
来源：http://ehs.feifeiyinyue.top

[U34] Py：判断编码
来源：http://iqg.ybcxt.top

chardet.detect(raw)
来源：http://tce.jlsjyb.cn

[U35] Py：发送邮件
来源：http://wzo.iojbl.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gvj.yangfankeji.com

[U36] Py：定时任务
来源：http://lhv.0kj1m.cn

schedule.every(10).minutes.do(job)
来源：http://qyo.daria6918.cn

[U37] Py：读写 Excel
来源：http://qxw.birdmap.top

pandas.read_excel / DataFrame.to_excel
来源：http://tvj.jqgfzy.top

[U38] Py：获取脚本所在目录
来源：http://wdz.chenzaomai.com

Path(__file__).resolve().parent
来源：http://ijc.yvedp.cn

[U39] Py：判断是否在交互环境
来源：http://xpk.yanxiufei.cn

sys.stdout.isatty()
来源：http://whl.52xcode.cn

[U40] Py：打印到标准错误
来源：http://vrf.birdmap.top

print("err", file=sys.stderr)
来源：http://phj.ehwqpu.com

[U41] PHP：初始化 Composer 项目
来源：http://lgv.jlsjyb.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://kij.gaohongyu789.top

[U42] PHP：PSR-4 自动加载
来源：http://agd.nanxuanxn.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lag.pengpengdd.cyou

[U43] PHP：声明命名空间
来源：http://iab.xuanzx.com

namespace App\Http;
来源：http://qyf.zhengqikj.top

[U44] PHP：开启严格类型
来源：http://myc.xylfe.cn

declare(strict_types=1);
来源：http://ljj.aibaodan.cn

[U45] PHP：类型声明与返回类型
来源：http://vpr.ivvv.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://gjp.zhaomingkeji.xyz

[U46] PHP：可空类型
来源：http://csp.hcnkem.com

?string $name = null
来源：http://mlq.jyoumei.cn

[U47] PHP：联合类型
来源：http://kaw.9152youxi.cn

int|string $id
来源：http://dwi.0kj1m.cn

[U48] PHP：纯枚举
来源：http://wht.redwolf501.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://txz.cdnleiting.top

[U49] PHP：只读属性
来源：http://vkr.guowangkeji.top

public readonly string $name
来源：http://dqy.316326.xyz

[U50] PHP：构造器属性提升
来源：http://hsb.guannengcc.top

public function __construct(private int $id) {}
来源：http://tdh.zhiwuduotai.top

[U51] PHP：数组解构
来源：http://uvh.cashguo.top

[$a, $b] = $arr;
来源：http://btq.zhoulong.xyz

[U52] PHP：箭头函数
来源：http://nte.shuidangran.top

$double = fn($x) => $x * 2;
来源：http://aob.bjfxy.top

[U53] PHP：空合并运算符
来源：http://qfa.aizwys.cn

$v = $a ?? $b ?? "default";
来源：http://nvd.snrcjt.cn

[U54] PHP：空安全调用
来源：http://tek.yj20258888.top

$obj?->method()
来源：http://faa.yuanzhike.top

[U55] PHP：match 表达式
来源：http://rfv.dianchejie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ysy.haohaochexian.top

[U56] PHP：命名参数
来源：http://mnb.zhoulong.xyz

f(a: 1, b: 2)
来源：http://phh.shzxlz.cn

[U57] PHP：字符串插值
来源：http://rnz.sxryk.cn

"值: {$a}"
来源：http://oke.zhengqikj.top

[U58] PHP：数组三件套
来源：http://nfj.52xcode.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zmp.zhongyouzk.top

[U59] PHP：自定义排序
来源：http://pem.bjfxy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://paq.tanke756.top

[U60] PHP：JSON 编解码
来源：http://qtf.xuanzx.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://szo.cucudq.cn

[U61] PHP：正则
来源：http://odx.zhaomingkeji.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://iec.jinqigufen.top

[U62] PHP：日期对象
来源：http://swv.jinghuilouyu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://cyj.daria6918.cn

[U63] PHP：文件读写
来源：http://bgv.shangyingyoupin.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pbp.gzhubu.top

[U64] PHP：目录遍历
来源：http://ebq.c1oappe.top

glob("dir/*.php");  scandir("dir");
来源：http://oiu.yj20258.top

[U65] PHP：会话
来源：http://idz.fanxiaobao.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://tbc.ydzc1.top

[U66] PHP：设置 Cookie
来源：http://eol.xuetiantiany.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://isn.fanxiaobao.xyz

[U67] PHP：处理文件上传
来源：http://jeh.bjfxy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://uim.guannengcc.top

[U68] PHP：PDO 连接
来源：http://kso.svipenyu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://dzi.iojbl.cn

[U69] PHP：PDO 预处理
来源：http://szd.chenlongwang.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bzq.ehwqpu.com

[U70] PHP：PDO 事务
来源：http://sij.gogol.net.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dzr.epnwcf.com

[U71] PHP：抛出异常
来源：http://lel.fengsongda.top

throw new RuntimeException("失败", 500);
来源：http://tcr.zdqjudy.top

[U72] PHP：写错误日志
来源：http://cvz.fehbvm.com

error_log("失败: " . $e->getMessage());
来源：http://yxh.jlsjyb.cn

[U73] PHP：读取 ini 配置
来源：http://tuv.hesvh.cn

parse_ini_file("config.ini", true)
来源：http://kac.ivvv.top

[U74] PHP：读取环境变量
来源：http://gta.jqgufenzy.top

getenv("APP_ENV") ?: "production"
来源：http://gwo.vehdjk.com

[U75] PHP：依赖注入
来源：http://lgf.uphjek.com

composer require psr/container
来源：http://rve.zdbjq.cn

[U76] PHP：简单路由
来源：http://vkb.daxiang520.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jbl.ctjpmb.com

[U77] PHP：模板渲染
来源：http://lbr.gaohongyu789.top

composer require twig/twig
来源：http://ira.daxiang520.top

[U78] PHP：单元测试
来源：http://ivc.ivvv.top

composer require --dev phpunit/phpunit
来源：http://uqs.guannengcc.top

[U79] PHP：静态分析
来源：http://top.fehbvm.com

composer require --dev phpstan/phpstan
来源：http://ukk.pengpengdd.cyou

[U80] PHP：代码规范修复
来源：http://vif.sjlbkw.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://efr.snrcjt.cn

[U81] JS：初始化项目
来源：http://hiq.sysykeji.top

npm init -y;  npm i express
来源：http://nam.jlsjyb.cn

[U82] JS：package.json 脚本
来源：http://kpt.jinqigufen.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wgt.sweek.top

[U83] JS：ES Module 导入导出
来源：http://yyt.shanyushiyangkeji.top

export const a = 1;  import { a } from "./m.js";
来源：http://vfs.meibo888.top

[U84] JS：CommonJS 写法
来源：http://bea.cheryme.top

module.exports = { a };  const { a } = require("./m");
来源：http://mns.yj202588.top

[U85] JS：可选链
来源：http://wzi.gogol.net.cn

a?.b?.c
来源：http://uvy.gogol.net.cn

[U86] JS：空值合并
来源：http://sru.yfazqb.com

a ?? b
来源：http://jiv.yvedp.cn

[U87] JS：解构默认值
来源：http://sof.nanxinkj.top

const { a = 1, b = 2 } = obj;
来源：http://rdb.tian-w.cn

[U88] JS：对象展开合并
来源：http://nna.zhixingplan.top

{ ...a, ...b }
来源：http://ehd.zhiwuduotai.top

[U89] JS：数组去重
来源：http://zuu.zdbjq.cn

[...new Set(arr)]
来源：http://uio.tanke756.top

[U90] JS：数字数组排序
来源：http://dco.quarkkingdee.top

[...arr].sort((a, b) => a - b)
来源：http://fcz.xuetiantiany.cn

[U91] JS：对象键值遍历
来源：http://rim.zhijiandao.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ijq.kuanghao11.cn

[U92] JS：深拷贝
来源：http://myz.yangfankeji.com

structuredClone(obj)
来源：http://tdv.ppjwa.cn

[U93] JS：模板字符串
来源：http://qpz.sysykeji.top

`共 ${n} 条`
来源：http://xnu.birdmap.top

[U94] JS：箭头函数
来源：http://bdh.9152youxi.cn

const double = x => x * 2;
来源：http://iwj.daxiang520.top

[U95] JS：Promise 包装
来源：http://lcx.xuetiantiany.cn

new Promise((resolve, reject) => {})
来源：http://fmu.zdqjudy.top

[U96] JS：async/await 与异常
来源：http://pmy.chenlongwang.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://buv.sweek.top

[U97] JS：并发请求
来源：http://pnx.yanxiufei.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://luo.redwolf501.top

[U98] JS：fetch 带 JSON
来源：http://upe.pycfn.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://sgu.fktsv.cn

[U99] JS：事件监听
来源：http://odp.nwbrower.top

el.addEventListener("click", e => {})
来源：http://lpr.hongshengwenyu.top

[U100] JS：DOM 查询
来源：http://nlj.cdnleiting.top

document.querySelector(".item")
来源：http://qkz.cqqwz.cn

[U101] JS：classList 操作
来源：http://ami.xingfuxueyuan.xyz

el.classList.toggle("active")
来源：http://bly.fktsv.cn

[U102] JS：本地存储
来源：http://zme.yangfankeji.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://ueu.hammf.cn

[U103] JS：定时器
来源：http://hzc.hesvh.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pfh.svipenyu.cn

[U104] JS：防抖
来源：http://xjr.shzxlz.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rnn.havefunace.top

[U105] JS：节流
来源：http://hon.ywan-chungtsiang.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zfb.guannengcc.top

[U106] JS：日期格式化
来源：http://zrn.tian-w.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gya.yj20258888.top

[U107] JS：数字千分位
来源：http://etu.snrcjt.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jwx.gotoacloud.top

[U108] JS：随机整数
来源：http://iki.fengsongda.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xkr.daxiang520.top

[U109] JS：数组分组
来源：http://fdr.daxiang520.top

Object.groupBy(arr, x => x.type)
来源：http://hap.ehwqpu.com

[U110] JS：数组分块
来源：http://syd.tianlin.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jsa.bjfxy.top

[U111] JS：对象转 Map
来源：http://sgq.zhoulong.xyz

new Map(Object.entries(obj))
来源：http://bcl.zhengqikj.top

[U112] JS：字符串补位
来源：http://eog.chenjidiqi.icu

"7".padStart(3, "0")
来源：http://vui.9152youxi.cn

[U113] JS：正则替换全部
来源：http://yfg.fzhhl.top

s.replaceAll("a", "b")
来源：http://nfs.tarul.cn

[U114] JS：JSON 深比较
来源：http://tdy.52xcode.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://gsd.gogol.net.cn

[U115] JS：生成 UUID
来源：http://knv.xuetiantiany.cn

crypto.randomUUID()
来源：http://yhs.sjlbkw.cn

[U116] JS：类型检查（JSDoc）
来源：http://kdx.yongpay.top

/** @param {string} name */ function f(name) {}
来源：http://vvh.xuanzx.com

[U117] JS：单元测试
来源：http://pot.cqqwz.cn

npm i -D vitest;  npx vitest
来源：http://yut.jiagoushi.top

[U118] JS：开发服务器
来源：http://kqu.feifeiyinyue.top

npm i -D vite;  npx vite
来源：http://hrf.fanxiaobao.xyz

[U119] JS：生产构建
来源：http://rzl.jinqigufen.top

npx vite build
来源：http://xqc.xuanzx.com

[U120] JS：读取环境变量（Vite）
来源：http://izo.jinqigufen.top

import.meta.env.VITE_API_URL
来源：http://ivp.shanyushiyangtech.top

================================================================================
来源：http://tfa.xuanzx.com

统计汇总
来源：http://jwf.ctjpmb.com

================================================================================
来源：http://twr.havefunace.top

按语言统计（条）：
来源：http://ycc.yuxming.cn

Python ......... 252
来源：http://cxc.gaohongyu789.top

PHP ............ 252
来源：http://hja.yj202588.top

JavaScript ..... 252
来源：http://mhf.havefunace.top

TypeScript ..... 212
来源：http://gpq.xinyue.icu

Java ........... 212
来源：http://yga.feifeiyinyue.top

Go ............. 212
来源：http://dqq.zhongyouzk.top

Ruby ........... 212
来源：http://vhu.jinqigufen.top

C# ............. 212
来源：http://xus.ybcxt.top

C .............. 30
来源：http://ymu.chenzaomai.com

C++ ............ 30
来源：http://olm.mhx1999.top

SQL ............ 90
来源：http://msq.kuanghao11.cn

Bash ........... 80
来源：http://eus.hnxiangtu.top

Kotlin ......... 15
来源：http://vrp.gotoacloud.top

Swift .......... 15
来源：http://wyg.jlsjyb.cn

Lua ............ 10
来源：http://rpa.pycfn.com

Perl ........... 10
来源：http://lic.zhaomingkeji.xyz

Scala .......... 10
来源：http://wic.cucudq.cn

------------------------------------
来源：http://zlh.bbcook.cn

合计 ........... 2106 条
来源：http://adg.hcnkem.com

按章节统计：
来源：http://pby.jqgfzy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tpv.tanke756.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rqm.andypj.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qsm.xuanzx.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rsx.vqdsnc.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rbh.zycfv.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ugf.zdbjq.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://gmq.hywenlv.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xgk.zhongyouzk.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bks.hnqzz.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nru.c1oappe.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gty.jinyuanbaomall.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://imb.cqqwz.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://fss.c1oappe.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://djp.shanyushiyangkeji.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://gne.xingfuxueyuan.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ued.zhijiandao.cn

Q SQL 专题                              90
来源：http://kvj.bbcook.cn

R Bash 专题                             80
来源：http://odj.nwbrower.top

S C / C++ 专题                          60
来源：http://eqx.yj202588.top

T 其他语言补充                          60
来源：http://jlh.aibaodan.cn

U 高频实用片段                         120
来源：http://npe.birdmap.top

------------------------------------
来源：http://kmy.yongpay.top

合计                                  2106 条
来源：http://ylj.jlsjyb.cn

--------------------------------------------------------------------------------
来源：http://gun.tanke756.top


<!-- 参考信息 -->