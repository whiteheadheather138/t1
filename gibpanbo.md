代发 wailian999

val a = 1;  var b = 2
来源：http://wkh.tianlin.xyz

[T53] Scala：字符串插值
来源：http://sqx.zhiwuduotai.top

s"值: $b"
来源：http://wvs.yj202588.top

[T54] Scala：集合映射
来源：http://koi.smart0.xyz

List(1, 2, 3).map(_ * 2)
来源：http://poc.ybcxt.top

[T55] Scala：集合过滤
来源：http://cbd.c1oappe.top

List(1, 2, 3).filter(_ > 1)
来源：http://hxc.zhengqikj.top

[T56] Scala：样例类
来源：http://ogq.sysykeji.top

case class User(name: String, age: Int)
来源：http://rzn.shangyingyoupin.top

[T57] Scala：模式匹配
来源：http://nbs.xylfe.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://sil.xuanzx.com

[T58] Scala：函数定义
来源：http://rwb.vehdjk.com

def add(a: Int, b: Int): Int = a + b
来源：http://zus.ctjpmb.com

[T59] Scala：循环
来源：http://jvw.quarkkingdee.top

for (i <- 1 to 10) println(i)
来源：http://pds.shangyingyoupin.top

[T60] Scala：折叠
来源：http://xvu.bbcook.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://kvo.cheryme.top

================================================================================
来源：http://tva.xylfe.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ean.yongpay.top

================================================================================
来源：http://ief.hesvh.cn

[U01] Py：创建虚拟环境
来源：http://lij.guowangkeji.top

python -m venv .venv && source .venv/bin/activate
来源：http://ckv.hnqzz.top

[U02] Py：导出 / 安装依赖
来源：http://ize.guowangkeji.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rhn.hongshengwenyu.top

[U03] Py：加载 .env 配置
来源：http://jyl.cheryme.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ctc.mhx1999.top

[U04] Py：变量调试打印
来源：http://acz.yanxiufei.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://uaf.cheryme.top

[U05] Py：列表去重且保序
来源：http://zql.nwbrower.top

list(dict.fromkeys(arr))
来源：http://akg.chenlongwang.top

[U06] Py：合并两个字典
来源：http://cgv.shanyushiyangkeji.top

{**a, **b}
来源：http://ewh.birdmap.top

[U07] Py：反转字典键值
来源：http://pls.feifeiyinyue.top

{v: k for k, v in d.items()}
来源：http://qgg.xuetiantiany.cn

[U08] Py：展平二维列表
来源：http://sgv.tarul.cn

[y for x in nested for y in x]
来源：http://tsc.fktsv.cn

[U09] Py：字典取最大值的键
来源：http://kph.zycfv.cn

max(d, key=d.get)
来源：http://bsh.xylfe.cn

[U10] Py：按值排序字典
来源：http://nuc.xziqi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://edn.smart0.xyz

[U11] Py：生成器表达式
来源：http://nrc.birdmap.top

(x * 2 for x in arr)
来源：http://efi.yj202588.top

[U12] Py：取出现最多的 3 个元素
来源：http://ylh.birdmap.top

Counter(arr).most_common(3)
来源：http://yqy.nwbrower.top

[U13] Py：固定长度队列
来源：http://emr.zhixingplan.top

deque(maxlen=10)
来源：http://xyj.yueranfly.top

[U14] Py：分组收集到列表
来源：http://jsc.dianchejie.cn

defaultdict(list)
来源：http://fun.sjlbkw.cn

[U15] Py：高精度计时
来源：http://zxb.vehdjk.com

t = time.perf_counter()
来源：http://yja.jqgufenzy.top

[U16] Py：命令行参数解析
来源：http://hjo.cdnleiting.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jwu.hesvh.cn

[U17] Py：初始化日志
来源：http://eow.shangyingyoupin.top

logging.basicConfig(level=logging.INFO)
来源：http://ppa.fktsv.cn

[U18] Py：预编译正则
来源：http://zgo.shanyushiyangkeji.top

pat = re.compile(r"\d+")
来源：http://hny.chenjidiqi.icu

[U19] Py：正则替换带回调
来源：http://blj.zhongyouzk.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nwy.hnxiangtu.top

[U20] Py：缓存函数结果
来源：http://gdr.0kj1m.cn

@functools.lru_cache(maxsize=None)
来源：http://web.fanxiaobao.xyz

[U21] Py：自定义上下文管理器
来源：http://kre.shzxlz.cn

@contextlib.contextmanager
来源：http://gap.cheryme.top

[U22] Py：矩阵转置
来源：http://ypb.gaohongyu789.top

list(zip(*m))
来源：http://yuc.xylfe.cn

[U23] Py：分块读取大文件
来源：http://vup.zycfv.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gsy.jinyuanbaomall.cn

[U24] Py：路径操作
来源：http://vrx.jianghu66.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bsr.cashguo.top

[U25] Py：CSV 按字典读
来源：http://kaa.aizwys.cn

csv.DictReader(f)
来源：http://mcr.shuidangran.top

[U26] Py：并发下载
来源：http://way.quarkkingdee.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://dad.birdmap.top

[U27] Py：异步 HTTP
来源：http://wdk.cdnleiting.top

aiohttp.ClientSession() 配合 async with
来源：http://jeb.yongpay.top

[U28] Py：类型别名
来源：http://sme.dianchejie.cn

UserId = int
来源：http://soo.yfazqb.com

[U29] Py：属性校验
来源：http://vnz.gaohongyu789.top

@property 与 @x.setter 配合
来源：http://qns.jinghuilouyu.cn

[U30] Py：数据类
来源：http://rqy.yj20258.top

@dataclass(slots=True)
来源：http://ujp.yfazqb.com

[U31] Py：单测
来源：http://npc.yuanzhike.top

python -m pytest -q
来源：http://etk.havefunace.top

[U32] Py：代码格式化
来源：http://dxf.iojbl.cn

ruff format . && ruff check --fix .
来源：http://pof.xylfe.cn

[U33] Py：打包发布
来源：http://ilu.sufxvd.cn

python -m build  （依赖 pyproject.toml）
来源：http://xkq.kuanghao11.cn

[U34] Py：判断编码
来源：http://sxd.yuxming.cn

chardet.detect(raw)
来源：http://gla.guannengcc.top

[U35] Py：发送邮件
来源：http://ner.yangfankeji.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://eer.yj202588.top

[U36] Py：定时任务
来源：http://kep.yuxming.cn

schedule.every(10).minutes.do(job)
来源：http://szu.chenzaomai.com

[U37] Py：读写 Excel
来源：http://kll.ydjk.org.cn

pandas.read_excel / DataFrame.to_excel
来源：http://xav.xylfe.cn

[U38] Py：获取脚本所在目录
来源：http://nmp.tianlin.xyz

Path(__file__).resolve().parent
来源：http://dpx.nwbrower.top

[U39] Py：判断是否在交互环境
来源：http://jux.zhengqikj.top

sys.stdout.isatty()
来源：http://qub.dianchejie.cn

[U40] Py：打印到标准错误
来源：http://hip.yongpay.top

print("err", file=sys.stderr)
来源：http://qoc.316326.xyz

[U41] PHP：初始化 Composer 项目
来源：http://qbz.birdmap.top

composer init;  composer require guzzlehttp/guzzle
来源：http://psj.gaohongyu789.top

[U42] PHP：PSR-4 自动加载
来源：http://ukf.jiagoushi.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mvw.pycfn.com

[U43] PHP：声明命名空间
来源：http://ell.nwbrower.top

namespace App\Http;
来源：http://swf.ydjk.org.cn

[U44] PHP：开启严格类型
来源：http://gev.daria6918.cn

declare(strict_types=1);
来源：http://pqj.redwolf501.top

[U45] PHP：类型声明与返回类型
来源：http://ifa.xziqi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://uil.ctjpmb.com

[U46] PHP：可空类型
来源：http://xco.snrcjt.cn

?string $name = null
来源：http://hvv.gzhubu.top

[U47] PHP：联合类型
来源：http://xbo.ydjk.org.cn

int|string $id
来源：http://qvj.bbcook.cn

[U48] PHP：纯枚举
来源：http://dhh.zhijiandao.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://sol.gaohongyu789.top

[U49] PHP：只读属性
来源：http://dtg.fanxiaobao.xyz

public readonly string $name
来源：http://vwa.fengsongda.top

[U50] PHP：构造器属性提升
来源：http://qzc.xinyue.icu

public function __construct(private int $id) {}
来源：http://rnx.shangyingyoupin.top

[U51] PHP：数组解构
来源：http://rlx.shanyushiyangtech.top

[$a, $b] = $arr;
来源：http://ibs.aizwys.cn

[U52] PHP：箭头函数
来源：http://vbp.yj20258888.top

$double = fn($x) => $x * 2;
来源：http://ong.wangshuangyany.cn

[U53] PHP：空合并运算符
来源：http://cpq.dashuyun.cn

$v = $a ?? $b ?? "default";
来源：http://cso.jinqigufen.top

[U54] PHP：空安全调用
来源：http://laf.cheryme.top

$obj?->method()
来源：http://phh.zhengqikj.top

[U55] PHP：match 表达式
来源：http://nna.sjlbkw.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xty.cucudq.cn

[U56] PHP：命名参数
来源：http://xlc.redwolf501.top

f(a: 1, b: 2)
来源：http://czu.snrcjt.cn

[U57] PHP：字符串插值
来源：http://zpf.shanyushiyangtech.top

"值: {$a}"
来源：http://jsl.zhijiandao.cn

[U58] PHP：数组三件套
来源：http://exi.kuanghao11.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zmf.chenjidiqi.icu

[U59] PHP：自定义排序
来源：http://axz.guowangkeji.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jxc.xingfuxueyuan.xyz

[U60] PHP：JSON 编解码
来源：http://ijj.nanxuanxn.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pka.guannengcc.top

[U61] PHP：正则
来源：http://wfg.sxryk.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://car.quarkkingdee.top

[U62] PHP：日期对象
来源：http://wpn.fktsv.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mlr.gzhubu.top

[U63] PHP：文件读写
来源：http://ybr.hammf.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wax.hongshengwenyu.top

[U64] PHP：目录遍历
来源：http://alc.jqgfzy.top

glob("dir/*.php");  scandir("dir");
来源：http://xum.zdqjudy.top

[U65] PHP：会话
来源：http://cyp.xylfe.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://qyw.zhengqikj.top

[U66] PHP：设置 Cookie
来源：http://zxo.tian-w.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gbc.jinyuanbaomall.cn

[U67] PHP：处理文件上传
来源：http://buc.shuidangran.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tny.kuanghao11.cn

[U68] PHP：PDO 连接
来源：http://vsn.shanyushiyangkeji.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://dst.jyoumei.cn

[U69] PHP：PDO 预处理
来源：http://xwc.andypj.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ndq.dashuyun.cn

[U70] PHP：PDO 事务
来源：http://alu.fanxiaobao.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://klw.ehwqpu.com

[U71] PHP：抛出异常
来源：http://cag.mhx1999.top

throw new RuntimeException("失败", 500);
来源：http://lte.jyoumei.cn

[U72] PHP：写错误日志
来源：http://oxd.hnxiangtu.top

error_log("失败: " . $e->getMessage());
来源：http://kxe.zhoulong.xyz

[U73] PHP：读取 ini 配置
来源：http://nll.aizwys.cn

parse_ini_file("config.ini", true)
来源：http://laq.cdnleiting.top

[U74] PHP：读取环境变量
来源：http://roe.bjfxy.top

getenv("APP_ENV") ?: "production"
来源：http://hsz.jiagoushi.top

[U75] PHP：依赖注入
来源：http://fij.52xcode.cn

composer require psr/container
来源：http://jln.jyoumei.cn

[U76] PHP：简单路由
来源：http://wdj.yonumen.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://war.zhijiandao.cn

[U77] PHP：模板渲染
来源：http://pre.zycfv.cn

composer require twig/twig
来源：http://epy.shuidangran.top

[U78] PHP：单元测试
来源：http://ydo.daria6918.cn

composer require --dev phpunit/phpunit
来源：http://ivn.shanyushiyangtech.top

[U79] PHP：静态分析
来源：http://zfs.pycfn.com

composer require --dev phpstan/phpstan
来源：http://eqo.yangfankeji.com

[U80] PHP：代码规范修复
来源：http://qtc.epnwcf.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://mrc.yangfankeji.com

[U81] JS：初始化项目
来源：http://dzu.zdqjudy.top

npm init -y;  npm i express
来源：http://syf.haohaochexian.top

[U82] JS：package.json 脚本
来源：http://mjf.mhx1999.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zgz.guannengcc.top

[U83] JS：ES Module 导入导出
来源：http://pnb.iojbl.cn

export const a = 1;  import { a } from "./m.js";
来源：http://glb.tarul.cn

[U84] JS：CommonJS 写法
来源：http://biv.sweek.top

module.exports = { a };  const { a } = require("./m");
来源：http://rwb.andypj.xyz

[U85] JS：可选链
来源：http://zht.pycfn.com

a?.b?.c
来源：http://teh.shuidangran.top

[U86] JS：空值合并
来源：http://klh.hcnkem.com

a ?? b
来源：http://izk.cheryme.top

[U87] JS：解构默认值
来源：http://sfu.birdmap.top

const { a = 1, b = 2 } = obj;
来源：http://iuv.iojbl.cn

[U88] JS：对象展开合并
来源：http://qgx.c1oappe.top

{ ...a, ...b }
来源：http://rzl.shangyingyoupin.top

[U89] JS：数组去重
来源：http://lfo.hysaishi.cn

[...new Set(arr)]
来源：http://taw.cucudq.cn

[U90] JS：数字数组排序
来源：http://ibe.haohaochexian.top

[...arr].sort((a, b) => a - b)
来源：http://tkf.ivvv.top

[U91] JS：对象键值遍历
来源：http://jwa.jianghu66.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cqz.guowangkeji.top

[U92] JS：深拷贝
来源：http://bkt.fanxiaobao.xyz

structuredClone(obj)
来源：http://gxa.shanyushiyangkeji.top

[U93] JS：模板字符串
来源：http://yeh.fehbvm.com

`共 ${n} 条`
来源：http://aul.xinyue.icu

[U94] JS：箭头函数
来源：http://mmk.tianlin.xyz

const double = x => x * 2;
来源：http://lfr.yvedp.cn

[U95] JS：Promise 包装
来源：http://czi.dianchejie.cn

new Promise((resolve, reject) => {})
来源：http://glp.hysaishi.cn

[U96] JS：async/await 与异常
来源：http://fdj.vqdsnc.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xvu.aizwys.cn

[U97] JS：并发请求
来源：http://ypw.yangfankeji.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://tcx.jiagoushi.top

[U98] JS：fetch 带 JSON
来源：http://lte.hnxiangtu.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://imk.fktsv.cn

[U99] JS：事件监听
来源：http://arx.dashuyun.cn

el.addEventListener("click", e => {})
来源：http://sft.bjfxy.top

[U100] JS：DOM 查询
来源：http://evj.jqgfzy.top

document.querySelector(".item")
来源：http://iqs.feifeiyinyue.top

[U101] JS：classList 操作
来源：http://kbw.zhoulong.xyz

el.classList.toggle("active")
来源：http://vkb.ehwqpu.com

[U102] JS：本地存储
来源：http://sqt.redwolf501.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://oop.yongpay.top

[U103] JS：定时器
来源：http://nhr.ywan-chungtsiang.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://bpp.gzhubu.top

[U104] JS：防抖
来源：http://dqn.aizwys.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bkh.zhixingplan.top

[U105] JS：节流
来源：http://xnr.xuanzx.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wis.zhaomingkeji.xyz

[U106] JS：日期格式化
来源：http://pfg.c1oappe.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jqb.yangfankeji.com

[U107] JS：数字千分位
来源：http://zqi.jiagoushi.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vsa.yj20258888.top

[U108] JS：随机整数
来源：http://tpi.guowangkeji.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://uab.tianlin.xyz

[U109] JS：数组分组
来源：http://bkz.shanyushiyangkeji.top

Object.groupBy(arr, x => x.type)
来源：http://dcr.shanyushiyangtech.top

[U110] JS：数组分块
来源：http://uxf.sufxvd.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://azr.yuxming.cn

[U111] JS：对象转 Map
来源：http://bnb.jinqigufen.top

new Map(Object.entries(obj))
来源：http://cvz.hysaishi.cn

[U112] JS：字符串补位
来源：http://ier.xinyue.icu

"7".padStart(3, "0")
来源：http://yql.cqqwz.cn

[U113] JS：正则替换全部
来源：http://rda.xuanzx.com

s.replaceAll("a", "b")
来源：http://uwa.jyoumei.cn

[U114] JS：JSON 深比较
来源：http://ipt.zycfv.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://abj.jinqigfzy.top

[U115] JS：生成 UUID
来源：http://ilp.yangfankeji.com

crypto.randomUUID()
来源：http://pse.quarkkingdee.top

[U116] JS：类型检查（JSDoc）
来源：http://ftz.jiagoushi.top

/** @param {string} name */ function f(name) {}
来源：http://kye.ydjk.org.cn

[U117] JS：单元测试
来源：http://cnw.zhengqikj.top

npm i -D vitest;  npx vitest
来源：http://gkq.zhongyouzk.top

[U118] JS：开发服务器
来源：http://tjg.zhengqikj.top

npm i -D vite;  npx vite
来源：http://yxo.haohaochexian.top

[U119] JS：生产构建
来源：http://fwc.mhx1999.top

npx vite build
来源：http://huc.guannengcc.top

[U120] JS：读取环境变量（Vite）
来源：http://ekt.hammf.cn

import.meta.env.VITE_API_URL
来源：http://ttw.yj20258.top

================================================================================
来源：http://qeu.jinqigfzy.top

统计汇总
来源：http://nuh.daxiang520.top

================================================================================
来源：http://hbs.fktsv.cn

按语言统计（条）：
来源：http://kwj.hnqzz.top

Python ......... 252
来源：http://tpu.pycfn.com

PHP ............ 252
来源：http://hrt.ydjk.org.cn

JavaScript ..... 252
来源：http://udd.shanyushiyangtech.top

TypeScript ..... 212
来源：http://yyz.kuanghao11.cn

Java ........... 212
来源：http://kwz.haohaochexian.top

Go ............. 212
来源：http://hso.fehbvm.com

Ruby ........... 212
来源：http://hex.yvedp.cn

C# ............. 212
来源：http://tzd.nanxuanxn.top

C .............. 30
来源：http://eji.chenlongwang.top

C++ ............ 30
来源：http://shc.xziqi.cn

SQL ............ 90
来源：http://mdm.tanke756.top

Bash ........... 80
来源：http://owb.daria6918.cn

Kotlin ......... 15
来源：http://hjt.jinqigufen.top

Swift .......... 15
来源：http://wuc.52xcode.cn

Lua ............ 10
来源：http://ivm.ctjpmb.com

Perl ........... 10
来源：http://lbr.cucudq.cn

Scala .......... 10
来源：http://wir.haohaochexian.top

------------------------------------
来源：http://baa.meibo888.top

合计 ........... 2106 条
来源：http://uxn.zhijiandao.cn

按章节统计：
来源：http://rel.sufxvd.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wda.jqgufenzy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lgs.haohaochexian.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vif.jianghu66.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rne.birdmap.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://cmr.hnqzz.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ayp.yfazqb.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://pwg.jianghu66.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vpe.meibo888.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hiw.pengpengdd.cyou

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zzj.gaohongyu789.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pii.svipenyu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gcu.feifeiyinyue.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://djv.zhixingplan.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://pau.dianchejie.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ojk.aizwys.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://cxk.bjfxy.top


<!-- 参考信息 -->