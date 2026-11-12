代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://cmb.yangfankeji.com

[T55] Scala：集合过滤
来源：http://pue.pycfn.com

List(1, 2, 3).filter(_ > 1)
来源：http://nph.shanyushiyangtech.top

[T56] Scala：样例类
来源：http://dgj.ybcxt.top

case class User(name: String, age: Int)
来源：http://zdu.dianchejie.cn

[T57] Scala：模式匹配
来源：http://oxe.meibo888.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://kom.pengpengdd.cyou

[T58] Scala：函数定义
来源：http://idx.cqqwz.cn

def add(a: Int, b: Int): Int = a + b
来源：http://twg.hywenlv.cn

[T59] Scala：循环
来源：http://fah.kuanghao11.cn

for (i <- 1 to 10) println(i)
来源：http://nyr.zhixingplan.top

[T60] Scala：折叠
来源：http://eht.gaohongyu789.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mzr.smart0.xyz

================================================================================
来源：http://vlb.tarul.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ckw.hammf.cn

================================================================================
来源：http://noe.tarul.cn

[U01] Py：创建虚拟环境
来源：http://gsk.yanxiufei.cn

python -m venv .venv && source .venv/bin/activate
来源：http://jik.guowangkeji.top

[U02] Py：导出 / 安装依赖
来源：http://tvg.guowangkeji.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qrr.yonumen.top

[U03] Py：加载 .env 配置
来源：http://too.hywenlv.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://iwa.tarul.cn

[U04] Py：变量调试打印
来源：http://ufi.xylfe.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://omt.shanyushiyangkeji.top

[U05] Py：列表去重且保序
来源：http://jto.daxiang520.top

list(dict.fromkeys(arr))
来源：http://uqi.meibo888.top

[U06] Py：合并两个字典
来源：http://lxu.guowangkeji.top

{**a, **b}
来源：http://zgs.xinyue.icu

[U07] Py：反转字典键值
来源：http://hfr.andypj.xyz

{v: k for k, v in d.items()}
来源：http://vep.shanyushiyangtech.top

[U08] Py：展平二维列表
来源：http://sii.cashguo.top

[y for x in nested for y in x]
来源：http://wne.hfpthk.cn

[U09] Py：字典取最大值的键
来源：http://dvq.ppjwa.cn

max(d, key=d.get)
来源：http://anw.aizwys.cn

[U10] Py：按值排序字典
来源：http://xuc.zhaomingkeji.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wqr.jinyuanbaomall.cn

[U11] Py：生成器表达式
来源：http://zfg.fengsongda.top

(x * 2 for x in arr)
来源：http://nav.pengpengdd.cyou

[U12] Py：取出现最多的 3 个元素
来源：http://bdt.xylfe.cn

Counter(arr).most_common(3)
来源：http://xvy.shuidangran.top

[U13] Py：固定长度队列
来源：http://ppj.ydzc1.top

deque(maxlen=10)
来源：http://fec.hywenlv.cn

[U14] Py：分组收集到列表
来源：http://cvw.gogol.net.cn

defaultdict(list)
来源：http://ndg.hcnkem.com

[U15] Py：高精度计时
来源：http://nvm.zhoulong.xyz

t = time.perf_counter()
来源：http://ndn.zhaomingkeji.xyz

[U16] Py：命令行参数解析
来源：http://bnl.zhongyouzk.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vhp.zhixingplan.top

[U17] Py：初始化日志
来源：http://kpx.zhiwuduotai.top

logging.basicConfig(level=logging.INFO)
来源：http://zgw.yueranfly.top

[U18] Py：预编译正则
来源：http://dbb.quarkkingdee.top

pat = re.compile(r"\d+")
来源：http://qsp.52xcode.cn

[U19] Py：正则替换带回调
来源：http://feg.bbcook.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mdn.yj202588.top

[U20] Py：缓存函数结果
来源：http://fsk.0kj1m.cn

@functools.lru_cache(maxsize=None)
来源：http://jnx.jianghu66.top

[U21] Py：自定义上下文管理器
来源：http://fof.uphjek.com

@contextlib.contextmanager
来源：http://ukh.hywenlv.cn

[U22] Py：矩阵转置
来源：http://gji.smart0.xyz

list(zip(*m))
来源：http://pom.fanxiaobao.xyz

[U23] Py：分块读取大文件
来源：http://ywt.bbcook.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qby.sjlbkw.cn

[U24] Py：路径操作
来源：http://gnc.wangdashe.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gdj.zdqjudy.top

[U25] Py：CSV 按字典读
来源：http://vrq.hnqzz.top

csv.DictReader(f)
来源：http://zmz.hfpthk.cn

[U26] Py：并发下载
来源：http://mhp.sxryk.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://oog.tarul.cn

[U27] Py：异步 HTTP
来源：http://bvz.ehwqpu.com

aiohttp.ClientSession() 配合 async with
来源：http://pvw.guowangkeji.top

[U28] Py：类型别名
来源：http://qxf.sweek.top

UserId = int
来源：http://xbn.yj202588.top

[U29] Py：属性校验
来源：http://fja.kuanghao11.cn

@property 与 @x.setter 配合
来源：http://sji.smart0.xyz

[U30] Py：数据类
来源：http://nzu.hnxiangtu.top

@dataclass(slots=True)
来源：http://mra.daria6918.cn

[U31] Py：单测
来源：http://giz.cashguo.top

python -m pytest -q
来源：http://ryf.zhaomingkeji.xyz

[U32] Py：代码格式化
来源：http://avx.shanyushiyangtech.top

ruff format . && ruff check --fix .
来源：http://xuw.gogol.net.cn

[U33] Py：打包发布
来源：http://yue.xylfe.cn

python -m build  （依赖 pyproject.toml）
来源：http://ntv.yueranfly.top

[U34] Py：判断编码
来源：http://ceq.andypj.xyz

chardet.detect(raw)
来源：http://bzj.tian-w.cn

[U35] Py：发送邮件
来源：http://jfw.ybcxt.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tin.fzhhl.top

[U36] Py：定时任务
来源：http://gas.316326.xyz

schedule.every(10).minutes.do(job)
来源：http://sps.sysykeji.top

[U37] Py：读写 Excel
来源：http://ict.yj202588.top

pandas.read_excel / DataFrame.to_excel
来源：http://fij.yuanzhike.top

[U38] Py：获取脚本所在目录
来源：http://xij.dianchejie.cn

Path(__file__).resolve().parent
来源：http://utv.fehbvm.com

[U39] Py：判断是否在交互环境
来源：http://uja.cheryme.top

sys.stdout.isatty()
来源：http://bjj.quarkkingdee.top

[U40] Py：打印到标准错误
来源：http://kvs.yj20258.top

print("err", file=sys.stderr)
来源：http://cqg.hnqzz.top

[U41] PHP：初始化 Composer 项目
来源：http://ude.fktsv.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://pyi.haohaochexian.top

[U42] PHP：PSR-4 自动加载
来源：http://xav.dashuyun.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xyi.guowangkeji.top

[U43] PHP：声明命名空间
来源：http://enz.uphjek.com

namespace App\Http;
来源：http://iff.bbcook.cn

[U44] PHP：开启严格类型
来源：http://fuz.jianghu66.top

declare(strict_types=1);
来源：http://iwq.ywan-chungtsiang.top

[U45] PHP：类型声明与返回类型
来源：http://bxk.yj202588.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ysc.iojbl.cn

[U46] PHP：可空类型
来源：http://oqh.pengpengdd.cyou

?string $name = null
来源：http://vsc.cashguo.top

[U47] PHP：联合类型
来源：http://sds.zdbjq.cn

int|string $id
来源：http://gfi.cdnleiting.top

[U48] PHP：纯枚举
来源：http://lft.vqdsnc.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jrf.hesvh.cn

[U49] PHP：只读属性
来源：http://ugx.uphjek.com

public readonly string $name
来源：http://dcu.xuetiantiany.cn

[U50] PHP：构造器属性提升
来源：http://odn.yfazqb.com

public function __construct(private int $id) {}
来源：http://tnp.nanxinkj.top

[U51] PHP：数组解构
来源：http://qlh.cheryme.top

[$a, $b] = $arr;
来源：http://cgf.zhixingplan.top

[U52] PHP：箭头函数
来源：http://ldf.sweek.top

$double = fn($x) => $x * 2;
来源：http://xmi.yfazqb.com

[U53] PHP：空合并运算符
来源：http://vfr.wangdashe.top

$v = $a ?? $b ?? "default";
来源：http://sol.fanxiaobao.xyz

[U54] PHP：空安全调用
来源：http://ylu.xuanzx.com

$obj?->method()
来源：http://hca.mhx1999.top

[U55] PHP：match 表达式
来源：http://tyn.hcnkem.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yas.cashguo.top

[U56] PHP：命名参数
来源：http://vlj.daxiang520.top

f(a: 1, b: 2)
来源：http://tej.hnqzz.top

[U57] PHP：字符串插值
来源：http://qik.guowangkeji.top

"值: {$a}"
来源：http://jpc.jinqigufen.top

[U58] PHP：数组三件套
来源：http://umf.yueranfly.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://sbx.zhengqikj.top

[U59] PHP：自定义排序
来源：http://zbr.shuidangran.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dou.hammf.cn

[U60] PHP：JSON 编解码
来源：http://fxa.cheryme.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://riz.zhiwuduotai.top

[U61] PHP：正则
来源：http://bbp.yfazqb.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://snf.hnqzz.top

[U62] PHP：日期对象
来源：http://iye.shangyingyoupin.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://yyv.kuanghao11.cn

[U63] PHP：文件读写
来源：http://ntw.vehdjk.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pib.yonumen.top

[U64] PHP：目录遍历
来源：http://rhc.xziqi.cn

glob("dir/*.php");  scandir("dir");
来源：http://rcl.yuanzhike.top

[U65] PHP：会话
来源：http://cqc.zhiwuduotai.top

session_start();  $_SESSION["uid"] = 1;
来源：http://urg.hesvh.cn

[U66] PHP：设置 Cookie
来源：http://pnz.sxryk.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dhz.tarul.cn

[U67] PHP：处理文件上传
来源：http://set.hongshengwenyu.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://abb.epnwcf.com

[U68] PHP：PDO 连接
来源：http://kci.zhiwuduotai.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://sdv.316326.xyz

[U69] PHP：PDO 预处理
来源：http://pan.hywenlv.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://enx.redwolf501.top

[U70] PHP：PDO 事务
来源：http://jof.jiagoushi.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mhn.zhoulong.xyz

[U71] PHP：抛出异常
来源：http://fft.nanxuanxn.top

throw new RuntimeException("失败", 500);
来源：http://xlj.cheryme.top

[U72] PHP：写错误日志
来源：http://hxc.andypj.xyz

error_log("失败: " . $e->getMessage());
来源：http://bla.shuidangran.top

[U73] PHP：读取 ini 配置
来源：http://prx.hongshengwenyu.top

parse_ini_file("config.ini", true)
来源：http://fff.iojbl.cn

[U74] PHP：读取环境变量
来源：http://ciy.tarul.cn

getenv("APP_ENV") ?: "production"
来源：http://znr.hcnkem.com

[U75] PHP：依赖注入
来源：http://lzm.haohaochexian.top

composer require psr/container
来源：http://gug.pycfn.com

[U76] PHP：简单路由
来源：http://bhl.jlsjyb.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pnf.yangfankeji.com

[U77] PHP：模板渲染
来源：http://hgp.jinqigfzy.top

composer require twig/twig
来源：http://nfi.shangyingyoupin.top

[U78] PHP：单元测试
来源：http://nox.yangfankeji.com

composer require --dev phpunit/phpunit
来源：http://udr.shuidangran.top

[U79] PHP：静态分析
来源：http://roy.hywenlv.cn

composer require --dev phpstan/phpstan
来源：http://qvs.sysykeji.top

[U80] PHP：代码规范修复
来源：http://knr.gaohongyu789.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://xgw.hfpthk.cn

[U81] JS：初始化项目
来源：http://hzc.316326.xyz

npm init -y;  npm i express
来源：http://gzc.kuanghao11.cn

[U82] JS：package.json 脚本
来源：http://fba.fehbvm.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wfr.9152youxi.cn

[U83] JS：ES Module 导入导出
来源：http://kqt.pycfn.com

export const a = 1;  import { a } from "./m.js";
来源：http://jyi.xinyue.icu

[U84] JS：CommonJS 写法
来源：http://sue.meibo888.top

module.exports = { a };  const { a } = require("./m");
来源：http://evm.zhiwuduotai.top

[U85] JS：可选链
来源：http://ell.shangyingyoupin.top

a?.b?.c
来源：http://ego.cqqwz.cn

[U86] JS：空值合并
来源：http://fgv.tian-w.cn

a ?? b
来源：http://ebc.jianghu66.top

[U87] JS：解构默认值
来源：http://vpe.cheryme.top

const { a = 1, b = 2 } = obj;
来源：http://nou.yonumen.top

[U88] JS：对象展开合并
来源：http://kee.yangfankeji.com

{ ...a, ...b }
来源：http://jbo.vqdsnc.cn

[U89] JS：数组去重
来源：http://usp.fanxiaobao.xyz

[...new Set(arr)]
来源：http://jdl.xuetiantiany.cn

[U90] JS：数字数组排序
来源：http://fuk.shangyingyoupin.top

[...arr].sort((a, b) => a - b)
来源：http://hep.yonumen.top

[U91] JS：对象键值遍历
来源：http://ngk.uphjek.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gax.smart0.xyz

[U92] JS：深拷贝
来源：http://sjj.sxryk.cn

structuredClone(obj)
来源：http://cvw.cqqwz.cn

[U93] JS：模板字符串
来源：http://xxq.sufxvd.cn

`共 ${n} 条`
来源：http://vtw.wangshuangyany.cn

[U94] JS：箭头函数
来源：http://nhf.zhijiandao.cn

const double = x => x * 2;
来源：http://spt.tian-w.cn

[U95] JS：Promise 包装
来源：http://pcl.sufxvd.cn

new Promise((resolve, reject) => {})
来源：http://avg.ybcxt.top

[U96] JS：async/await 与异常
来源：http://koh.hammf.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vfg.jinyuanbaomall.cn

[U97] JS：并发请求
来源：http://mhs.feifeiyinyue.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://rav.haohaochexian.top

[U98] JS：fetch 带 JSON
来源：http://fmf.sweek.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://lyq.shanyushiyangkeji.top

[U99] JS：事件监听
来源：http://grh.9152youxi.cn

el.addEventListener("click", e => {})
来源：http://oxn.nanxinkj.top

[U100] JS：DOM 查询
来源：http://mnz.cucudq.cn

document.querySelector(".item")
来源：http://peg.jyoumei.cn

[U101] JS：classList 操作
来源：http://qqw.tian-w.cn

el.classList.toggle("active")
来源：http://fgi.yuxming.cn

[U102] JS：本地存储
来源：http://iep.mhx1999.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ayp.jqgufenzy.top

[U103] JS：定时器
来源：http://blt.hcnkem.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vhz.dashuyun.cn

[U104] JS：防抖
来源：http://yhb.ppjwa.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wic.hcnkem.com

[U105] JS：节流
来源：http://tbi.jianghu66.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://iqf.xinyue.icu

[U106] JS：日期格式化
来源：http://hej.fanxiaobao.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rxs.yj202588.top

[U107] JS：数字千分位
来源：http://kvp.yfazqb.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://tez.tanke756.top

[U108] JS：随机整数
来源：http://xze.ybcxt.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ovq.shangyingyoupin.top

[U109] JS：数组分组
来源：http://igc.zhoulong.xyz

Object.groupBy(arr, x => x.type)
来源：http://aik.yj20258888.top

[U110] JS：数组分块
来源：http://nie.shangyingyoupin.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://azv.uphjek.com

[U111] JS：对象转 Map
来源：http://eyx.yj202588.top

new Map(Object.entries(obj))
来源：http://pyk.hfpthk.cn

[U112] JS：字符串补位
来源：http://qya.gogol.net.cn

"7".padStart(3, "0")
来源：http://ywt.redwolf501.top

[U113] JS：正则替换全部
来源：http://vmt.yonumen.top

s.replaceAll("a", "b")
来源：http://uou.kuanghao11.cn

[U114] JS：JSON 深比较
来源：http://pjp.jinghuilouyu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://qyx.meibo888.top

[U115] JS：生成 UUID
来源：http://gjd.pengpengdd.cyou

crypto.randomUUID()
来源：http://jix.dashuyun.cn

[U116] JS：类型检查（JSDoc）
来源：http://stp.316326.xyz

/** @param {string} name */ function f(name) {}
来源：http://jfo.svipenyu.cn

[U117] JS：单元测试
来源：http://hxw.chenzaomai.com

npm i -D vitest;  npx vitest
来源：http://pgi.zhijiandao.cn

[U118] JS：开发服务器
来源：http://efl.tarul.cn

npm i -D vite;  npx vite
来源：http://ush.hesvh.cn

[U119] JS：生产构建
来源：http://uaa.hnqzz.top

npx vite build
来源：http://twl.sjlbkw.cn

[U120] JS：读取环境变量（Vite）
来源：http://kaf.hfpthk.cn

import.meta.env.VITE_API_URL
来源：http://yhp.hcnkem.com

================================================================================
来源：http://nnf.ppjwa.cn

统计汇总
来源：http://jhx.kuanghao11.cn

================================================================================
来源：http://gtl.tanke756.top

按语言统计（条）：
来源：http://tlh.gotoacloud.top

Python ......... 252
来源：http://icr.gzhubu.top

PHP ............ 252
来源：http://lgx.zhijiandao.cn

JavaScript ..... 252
来源：http://bjv.ydzc1.top

TypeScript ..... 212
来源：http://xmu.gotoacloud.top

Java ........... 212
来源：http://wsu.ybcxt.top

Go ............. 212
来源：http://gze.gotoacloud.top

Ruby ........... 212
来源：http://llz.sweek.top

C# ............. 212
来源：http://kqs.birdmap.top

C .............. 30
来源：http://qdk.snrcjt.cn

C++ ............ 30
来源：http://etp.bbcook.cn

SQL ............ 90
来源：http://pyj.vqdsnc.cn

Bash ........... 80
来源：http://rsq.yanxiufei.cn

Kotlin ......... 15
来源：http://kqs.zycfv.cn

Swift .......... 15
来源：http://ulr.snrcjt.cn

Lua ............ 10
来源：http://egm.fktsv.cn

Perl ........... 10
来源：http://vtu.pycfn.com

Scala .......... 10
来源：http://ndt.bjfxy.top

------------------------------------
来源：http://odj.zhongyouzk.top

合计 ........... 2106 条
来源：http://wrd.svipenyu.cn

按章节统计：
来源：http://sxv.shanyushiyangtech.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://coa.bjfxy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://vic.yuxming.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://klx.pycfn.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ugk.9152youxi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rtt.c1oappe.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://llb.zdqjudy.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://haj.svipenyu.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kjg.birdmap.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lgs.ehwqpu.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://viw.pycfn.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://def.hnqzz.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fim.bjfxy.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hky.zhoulong.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://glm.pengpengdd.cyou

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bpf.sjlbkw.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bni.hywenlv.cn

Q SQL 专题                              90
来源：http://qif.nwbrower.top

R Bash 专题                             80
来源：http://jpg.sxryk.cn

S C / C++ 专题                          60
来源：http://nob.yongpay.top

T 其他语言补充                          60
来源：http://frt.hnxiangtu.top


<!-- 参考信息 -->