代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://mze.haohaochexian.top

[T59] Scala：循环
来源：http://cns.yfazqb.com

for (i <- 1 to 10) println(i)
来源：http://qug.ppjwa.cn

[T60] Scala：折叠
来源：http://sdq.jyoumei.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://kzx.tarul.cn

================================================================================
来源：http://sxp.ehwqpu.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://whn.jinyuanbaomall.cn

================================================================================
来源：http://elc.birdmap.top

[U01] Py：创建虚拟环境
来源：http://hdh.xuanzx.com

python -m venv .venv && source .venv/bin/activate
来源：http://jim.birdmap.top

[U02] Py：导出 / 安装依赖
来源：http://enw.chenlongwang.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://iwp.ydzc1.top

[U03] Py：加载 .env 配置
来源：http://bgu.xuanzx.com

from dotenv import load_dotenv; load_dotenv()
来源：http://ynw.tanke756.top

[U04] Py：变量调试打印
来源：http://eih.zycfv.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://txs.xylfe.cn

[U05] Py：列表去重且保序
来源：http://vvy.ctjpmb.com

list(dict.fromkeys(arr))
来源：http://dar.cqqwz.cn

[U06] Py：合并两个字典
来源：http://jao.ybcxt.top

{**a, **b}
来源：http://irt.aizwys.cn

[U07] Py：反转字典键值
来源：http://fhn.fzhhl.top

{v: k for k, v in d.items()}
来源：http://bjh.dianchejie.cn

[U08] Py：展平二维列表
来源：http://lmx.smart0.xyz

[y for x in nested for y in x]
来源：http://uiv.zhengqikj.top

[U09] Py：字典取最大值的键
来源：http://frm.epnwcf.com

max(d, key=d.get)
来源：http://ejl.chenzaomai.com

[U10] Py：按值排序字典
来源：http://lai.guowangkeji.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nmm.guannengcc.top

[U11] Py：生成器表达式
来源：http://nnl.jiagoushi.top

(x * 2 for x in arr)
来源：http://zkm.ehwqpu.com

[U12] Py：取出现最多的 3 个元素
来源：http://dgr.zhongyouzk.top

Counter(arr).most_common(3)
来源：http://fov.jqgfzy.top

[U13] Py：固定长度队列
来源：http://dpl.jinyuanbaomall.cn

deque(maxlen=10)
来源：http://pkt.jinyuanbaomall.cn

[U14] Py：分组收集到列表
来源：http://tfi.yj20258888.top

defaultdict(list)
来源：http://iff.aizwys.cn

[U15] Py：高精度计时
来源：http://xzg.ehwqpu.com

t = time.perf_counter()
来源：http://xez.zhijiandao.cn

[U16] Py：命令行参数解析
来源：http://sdt.andypj.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bio.hammf.cn

[U17] Py：初始化日志
来源：http://iky.gzhubu.top

logging.basicConfig(level=logging.INFO)
来源：http://kmo.jinqigufen.top

[U18] Py：预编译正则
来源：http://sdf.redwolf501.top

pat = re.compile(r"\d+")
来源：http://kyx.feifeiyinyue.top

[U19] Py：正则替换带回调
来源：http://kuv.shuidangran.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://uhx.tarul.cn

[U20] Py：缓存函数结果
来源：http://pyf.hongshengwenyu.top

@functools.lru_cache(maxsize=None)
来源：http://omj.gaohongyu789.top

[U21] Py：自定义上下文管理器
来源：http://ile.xuanzx.com

@contextlib.contextmanager
来源：http://yve.yanxiufei.cn

[U22] Py：矩阵转置
来源：http://cpy.zdbjq.cn

list(zip(*m))
来源：http://gvu.andypj.xyz

[U23] Py：分块读取大文件
来源：http://syq.9152youxi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://aoi.gzhubu.top

[U24] Py：路径操作
来源：http://jks.hammf.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dpy.c1oappe.top

[U25] Py：CSV 按字典读
来源：http://uli.bjfxy.top

csv.DictReader(f)
来源：http://fxz.zhixingplan.top

[U26] Py：并发下载
来源：http://ako.gzhubu.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xrm.gotoacloud.top

[U27] Py：异步 HTTP
来源：http://epm.c1oappe.top

aiohttp.ClientSession() 配合 async with
来源：http://tri.zdqjudy.top

[U28] Py：类型别名
来源：http://mdk.chenzaomai.com

UserId = int
来源：http://kvq.quarkkingdee.top

[U29] Py：属性校验
来源：http://ypq.yfazqb.com

@property 与 @x.setter 配合
来源：http://xvn.cqqwz.cn

[U30] Py：数据类
来源：http://euv.ivvv.top

@dataclass(slots=True)
来源：http://anf.aizwys.cn

[U31] Py：单测
来源：http://dhl.gaohongyu789.top

python -m pytest -q
来源：http://knn.sufxvd.cn

[U32] Py：代码格式化
来源：http://jbh.ctjpmb.com

ruff format . && ruff check --fix .
来源：http://jrr.zhixingplan.top

[U33] Py：打包发布
来源：http://eak.jqgfzy.top

python -m build  （依赖 pyproject.toml）
来源：http://wuu.jqgufenzy.top

[U34] Py：判断编码
来源：http://rpg.zycfv.cn

chardet.detect(raw)
来源：http://jvy.jqgfzy.top

[U35] Py：发送邮件
来源：http://ntd.tarul.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hig.zhixingplan.top

[U36] Py：定时任务
来源：http://quf.hnqzz.top

schedule.every(10).minutes.do(job)
来源：http://qgh.c1oappe.top

[U37] Py：读写 Excel
来源：http://wab.cqqwz.cn

pandas.read_excel / DataFrame.to_excel
来源：http://pbw.c1oappe.top

[U38] Py：获取脚本所在目录
来源：http://sip.yj20258888.top

Path(__file__).resolve().parent
来源：http://csq.jianghu66.top

[U39] Py：判断是否在交互环境
来源：http://anj.xuanzx.com

sys.stdout.isatty()
来源：http://tvi.yongpay.top

[U40] Py：打印到标准错误
来源：http://vfi.ybcxt.top

print("err", file=sys.stderr)
来源：http://bim.aibaodan.cn

[U41] PHP：初始化 Composer 项目
来源：http://fhi.yuxming.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://rsn.zhijiandao.cn

[U42] PHP：PSR-4 自动加载
来源：http://qcq.mhx1999.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mod.zhixingplan.top

[U43] PHP：声明命名空间
来源：http://fsy.snrcjt.cn

namespace App\Http;
来源：http://icq.havefunace.top

[U44] PHP：开启严格类型
来源：http://tkt.chenzaomai.com

declare(strict_types=1);
来源：http://bdt.gzhubu.top

[U45] PHP：类型声明与返回类型
来源：http://iot.xylfe.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://icy.daxiang520.top

[U46] PHP：可空类型
来源：http://mzc.wangdashe.top

?string $name = null
来源：http://unb.ydzc1.top

[U47] PHP：联合类型
来源：http://sco.dashuyun.cn

int|string $id
来源：http://oul.aibaodan.cn

[U48] PHP：纯枚举
来源：http://bow.sjlbkw.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://klf.xylfe.cn

[U49] PHP：只读属性
来源：http://xsj.sxryk.cn

public readonly string $name
来源：http://mku.c1oappe.top

[U50] PHP：构造器属性提升
来源：http://otm.sjlbkw.cn

public function __construct(private int $id) {}
来源：http://jbe.xuanzx.com

[U51] PHP：数组解构
来源：http://hwm.yj20258.top

[$a, $b] = $arr;
来源：http://nur.ctjpmb.com

[U52] PHP：箭头函数
来源：http://zje.shuidangran.top

$double = fn($x) => $x * 2;
来源：http://fav.guowangkeji.top

[U53] PHP：空合并运算符
来源：http://rpm.hammf.cn

$v = $a ?? $b ?? "default";
来源：http://eot.birdmap.top

[U54] PHP：空安全调用
来源：http://fwm.snrcjt.cn

$obj?->method()
来源：http://cse.fehbvm.com

[U55] PHP：match 表达式
来源：http://oxg.vehdjk.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vze.guowangkeji.top

[U56] PHP：命名参数
来源：http://pql.snrcjt.cn

f(a: 1, b: 2)
来源：http://oez.vehdjk.com

[U57] PHP：字符串插值
来源：http://ufh.redwolf501.top

"值: {$a}"
来源：http://hjk.tanke756.top

[U58] PHP：数组三件套
来源：http://cib.tarul.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rnt.shangyingyoupin.top

[U59] PHP：自定义排序
来源：http://eck.zhengqikj.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aog.dashuyun.cn

[U60] PHP：JSON 编解码
来源：http://gob.yj20258.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dlp.shanyushiyangtech.top

[U61] PHP：正则
来源：http://yge.nanxuanxn.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://eae.yvedp.cn

[U62] PHP：日期对象
来源：http://olw.hnqzz.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zef.haohaochexian.top

[U63] PHP：文件读写
来源：http://jzs.zdqjudy.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ron.shzxlz.cn

[U64] PHP：目录遍历
来源：http://tks.iojbl.cn

glob("dir/*.php");  scandir("dir");
来源：http://bzx.ydjk.org.cn

[U65] PHP：会话
来源：http://lca.hfpthk.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://sfh.cucudq.cn

[U66] PHP：设置 Cookie
来源：http://uea.iojbl.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nuk.zhoulong.xyz

[U67] PHP：处理文件上传
来源：http://xox.zhoulong.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bqz.nwbrower.top

[U68] PHP：PDO 连接
来源：http://jvh.zhixingplan.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bdj.haohaochexian.top

[U69] PHP：PDO 预处理
来源：http://bfk.cheryme.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ash.hammf.cn

[U70] PHP：PDO 事务
来源：http://shz.sysykeji.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qro.yuanzhike.top

[U71] PHP：抛出异常
来源：http://oao.jinghuilouyu.cn

throw new RuntimeException("失败", 500);
来源：http://vdu.fzhhl.top

[U72] PHP：写错误日志
来源：http://thf.fehbvm.com

error_log("失败: " . $e->getMessage());
来源：http://vjc.gotoacloud.top

[U73] PHP：读取 ini 配置
来源：http://qkc.hywenlv.cn

parse_ini_file("config.ini", true)
来源：http://nva.redwolf501.top

[U74] PHP：读取环境变量
来源：http://sul.jyoumei.cn

getenv("APP_ENV") ?: "production"
来源：http://xpx.xinyue.icu

[U75] PHP：依赖注入
来源：http://lam.sjlbkw.cn

composer require psr/container
来源：http://kho.jiagoushi.top

[U76] PHP：简单路由
来源：http://iew.jinyuanbaomall.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ofx.sxryk.cn

[U77] PHP：模板渲染
来源：http://ynu.xinyue.icu

composer require twig/twig
来源：http://zie.hcnkem.com

[U78] PHP：单元测试
来源：http://uoz.hongshengwenyu.top

composer require --dev phpunit/phpunit
来源：http://ifo.svipenyu.cn

[U79] PHP：静态分析
来源：http://yfr.ydjk.org.cn

composer require --dev phpstan/phpstan
来源：http://woj.vehdjk.com

[U80] PHP：代码规范修复
来源：http://geb.tanke756.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://hif.cqqwz.cn

[U81] JS：初始化项目
来源：http://hap.iojbl.cn

npm init -y;  npm i express
来源：http://lbz.yfazqb.com

[U82] JS：package.json 脚本
来源：http://qua.aibaodan.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://tfl.snrcjt.cn

[U83] JS：ES Module 导入导出
来源：http://hnm.pycfn.com

export const a = 1;  import { a } from "./m.js";
来源：http://jsx.yongpay.top

[U84] JS：CommonJS 写法
来源：http://udv.xuanzx.com

module.exports = { a };  const { a } = require("./m");
来源：http://qwh.tian-w.cn

[U85] JS：可选链
来源：http://fmk.yvedp.cn

a?.b?.c
来源：http://ckq.sxryk.cn

[U86] JS：空值合并
来源：http://bne.yvedp.cn

a ?? b
来源：http://eka.guannengcc.top

[U87] JS：解构默认值
来源：http://pcp.zdqjudy.top

const { a = 1, b = 2 } = obj;
来源：http://wtn.smart0.xyz

[U88] JS：对象展开合并
来源：http://jcd.ppjwa.cn

{ ...a, ...b }
来源：http://kqo.ehwqpu.com

[U89] JS：数组去重
来源：http://upa.hammf.cn

[...new Set(arr)]
来源：http://ngf.zycfv.cn

[U90] JS：数字数组排序
来源：http://tok.yonumen.top

[...arr].sort((a, b) => a - b)
来源：http://flr.hcnkem.com

[U91] JS：对象键值遍历
来源：http://abg.snrcjt.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xjv.zdqjudy.top

[U92] JS：深拷贝
来源：http://dxj.cdnleiting.top

structuredClone(obj)
来源：http://fxr.zhengqikj.top

[U93] JS：模板字符串
来源：http://ppx.shanyushiyangtech.top

`共 ${n} 条`
来源：http://jbb.hnqzz.top

[U94] JS：箭头函数
来源：http://nco.cqqwz.cn

const double = x => x * 2;
来源：http://uyb.sjlbkw.cn

[U95] JS：Promise 包装
来源：http://guo.gogol.net.cn

new Promise((resolve, reject) => {})
来源：http://jfq.vqdsnc.cn

[U96] JS：async/await 与异常
来源：http://zug.xuanzx.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://kjm.nanxinkj.top

[U97] JS：并发请求
来源：http://tpe.ppjwa.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://kgo.jinghuilouyu.cn

[U98] JS：fetch 带 JSON
来源：http://qhi.xylfe.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://noi.fengsongda.top

[U99] JS：事件监听
来源：http://alk.ybcxt.top

el.addEventListener("click", e => {})
来源：http://sac.zdqjudy.top

[U100] JS：DOM 查询
来源：http://hor.cashguo.top

document.querySelector(".item")
来源：http://vjd.jyoumei.cn

[U101] JS：classList 操作
来源：http://lug.zycfv.cn

el.classList.toggle("active")
来源：http://aad.yj202588.top

[U102] JS：本地存储
来源：http://tah.aibaodan.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ycr.xuetiantiany.cn

[U103] JS：定时器
来源：http://ptq.sjlbkw.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://aha.yfazqb.com

[U104] JS：防抖
来源：http://sdn.zhixingplan.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sut.xuanzx.com

[U105] JS：节流
来源：http://asg.jinyuanbaomall.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://grx.aibaodan.cn

[U106] JS：日期格式化
来源：http://krb.guowangkeji.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ibo.316326.xyz

[U107] JS：数字千分位
来源：http://hup.nanxinkj.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cwc.chenlongwang.top

[U108] JS：随机整数
来源：http://tcz.meibo888.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qap.tanke756.top

[U109] JS：数组分组
来源：http://mof.smart0.xyz

Object.groupBy(arr, x => x.type)
来源：http://noy.yj202588.top

[U110] JS：数组分块
来源：http://xos.nwbrower.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qfq.cqqwz.cn

[U111] JS：对象转 Map
来源：http://ehk.ehwqpu.com

new Map(Object.entries(obj))
来源：http://mls.yuanzhike.top

[U112] JS：字符串补位
来源：http://xxi.pycfn.com

"7".padStart(3, "0")
来源：http://pkv.mhx1999.top

[U113] JS：正则替换全部
来源：http://fki.xinyue.icu

s.replaceAll("a", "b")
来源：http://jrj.nwbrower.top

[U114] JS：JSON 深比较
来源：http://dni.zhengqikj.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://uui.tianlin.xyz

[U115] JS：生成 UUID
来源：http://stq.fzhhl.top

crypto.randomUUID()
来源：http://xbd.guowangkeji.top

[U116] JS：类型检查（JSDoc）
来源：http://wuh.svipenyu.cn

/** @param {string} name */ function f(name) {}
来源：http://afu.sjlbkw.cn

[U117] JS：单元测试
来源：http://sbo.jinghuilouyu.cn

npm i -D vitest;  npx vitest
来源：http://tfr.yfazqb.com

[U118] JS：开发服务器
来源：http://fty.fengsongda.top

npm i -D vite;  npx vite
来源：http://gng.cqqwz.cn

[U119] JS：生产构建
来源：http://spd.pycfn.com

npx vite build
来源：http://wch.zycfv.cn

[U120] JS：读取环境变量（Vite）
来源：http://pep.aibaodan.cn

import.meta.env.VITE_API_URL
来源：http://udy.bbcook.cn

================================================================================
来源：http://iqt.chenjidiqi.icu

统计汇总
来源：http://ggz.daxiang520.top

================================================================================
来源：http://dfe.ydjk.org.cn

按语言统计（条）：
来源：http://wdj.yvedp.cn

Python ......... 252
来源：http://eyt.yvedp.cn

PHP ............ 252
来源：http://zcu.jlsjyb.cn

JavaScript ..... 252
来源：http://fka.xuanzx.com

TypeScript ..... 212
来源：http://abs.xinyue.icu

Java ........... 212
来源：http://rhn.ywan-chungtsiang.top

Go ............. 212
来源：http://jpb.pycfn.com

Ruby ........... 212
来源：http://jwo.tianlin.xyz

C# ............. 212
来源：http://fgu.zhixingplan.top

C .............. 30
来源：http://sne.jianghu66.top

C++ ............ 30
来源：http://kei.hysaishi.cn

SQL ............ 90
来源：http://hat.sweek.top

Bash ........... 80
来源：http://fyu.ppjwa.cn

Kotlin ......... 15
来源：http://joz.0kj1m.cn

Swift .......... 15
来源：http://loi.smart0.xyz

Lua ............ 10
来源：http://xyg.jlsjyb.cn

Perl ........... 10
来源：http://bbm.hongshengwenyu.top

Scala .......... 10
来源：http://wfo.snrcjt.cn

------------------------------------
来源：http://kmf.wangshuangyany.cn

合计 ........... 2106 条
来源：http://flo.jianghu66.top

按章节统计：
来源：http://lxn.yj20258.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://umx.smart0.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ibo.jlsjyb.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vfb.jqgufenzy.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mjs.jiagoushi.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dit.jianghu66.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xpo.c1oappe.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xlm.fanxiaobao.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://thk.mhx1999.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wuo.yj202588.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://gpg.quarkkingdee.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rla.mhx1999.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gdl.vqdsnc.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kzm.havefunace.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vmc.cashguo.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dpj.52xcode.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://gbf.ydjk.org.cn

Q SQL 专题                              90
来源：http://qce.yongpay.top

R Bash 专题                             80
来源：http://fwk.52xcode.cn

S C / C++ 专题                          60
来源：http://hme.jlsjyb.cn

T 其他语言补充                          60
来源：http://iwg.hongshengwenyu.top

U 高频实用片段                         120
来源：http://iit.ctjpmb.com

------------------------------------
来源：http://wla.yfazqb.com

合计                                  2106 条
来源：http://ufk.sysykeji.top

--------------------------------------------------------------------------------
来源：http://aox.jinqigfzy.top

使用提醒
来源：http://avd.smart0.xyz

--------------------------------------------------------------------------------
来源：http://lzg.birdmap.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jjy.haohaochexian.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://oom.vehdjk.com


<!-- 参考信息 -->