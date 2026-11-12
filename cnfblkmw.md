代发 wailian999

[T49] Perl：函数
来源：http://vsn.svipenyu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qcv.tianlin.xyz

[T50] Perl：逐行读文件
来源：http://moi.cucudq.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://hcz.fktsv.cn

while (my $line = <$fh>) { print $line; }
来源：http://jfz.snrcjt.cn

[T51] Scala：Hello World
来源：http://bpm.hesvh.cn

println("Hello")
来源：http://gqp.hammf.cn

[T52] Scala：变量
来源：http://gzx.pengpengdd.cyou

val a = 1;  var b = 2
来源：http://tav.hnqzz.top

[T53] Scala：字符串插值
来源：http://huc.zhaomingkeji.xyz

s"值: $b"
来源：http://zjd.cashguo.top

[T54] Scala：集合映射
来源：http://ryg.smart0.xyz

List(1, 2, 3).map(_ * 2)
来源：http://lip.c1oappe.top

[T55] Scala：集合过滤
来源：http://klz.jinqigufen.top

List(1, 2, 3).filter(_ > 1)
来源：http://dgk.jinghuilouyu.cn

[T56] Scala：样例类
来源：http://yjb.ybcxt.top

case class User(name: String, age: Int)
来源：http://kwq.sxryk.cn

[T57] Scala：模式匹配
来源：http://vjl.316326.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://cnd.hcnkem.com

[T58] Scala：函数定义
来源：http://azw.bjfxy.top

def add(a: Int, b: Int): Int = a + b
来源：http://wqa.hcnkem.com

[T59] Scala：循环
来源：http://rtp.shangyingyoupin.top

for (i <- 1 to 10) println(i)
来源：http://tcj.gogol.net.cn

[T60] Scala：折叠
来源：http://qje.meibo888.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hnr.vqdsnc.cn

================================================================================
来源：http://twh.cheryme.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lvz.ydzc1.top

================================================================================
来源：http://jsb.shuidangran.top

[U01] Py：创建虚拟环境
来源：http://ygv.chenlongwang.top

python -m venv .venv && source .venv/bin/activate
来源：http://mbv.tarul.cn

[U02] Py：导出 / 安装依赖
来源：http://bgs.chenzaomai.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gej.tian-w.cn

[U03] Py：加载 .env 配置
来源：http://vfi.shzxlz.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ulr.jinghuilouyu.cn

[U04] Py：变量调试打印
来源：http://wml.daxiang520.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://glk.hesvh.cn

[U05] Py：列表去重且保序
来源：http://njz.iojbl.cn

list(dict.fromkeys(arr))
来源：http://cuk.guowangkeji.top

[U06] Py：合并两个字典
来源：http://bbi.aibaodan.cn

{**a, **b}
来源：http://nwn.dianchejie.cn

[U07] Py：反转字典键值
来源：http://ora.feifeiyinyue.top

{v: k for k, v in d.items()}
来源：http://gyf.ctjpmb.com

[U08] Py：展平二维列表
来源：http://mse.dashuyun.cn

[y for x in nested for y in x]
来源：http://uja.xuetiantiany.cn

[U09] Py：字典取最大值的键
来源：http://tgo.meibo888.top

max(d, key=d.get)
来源：http://drm.yj20258.top

[U10] Py：按值排序字典
来源：http://dxz.birdmap.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nsr.hywenlv.cn

[U11] Py：生成器表达式
来源：http://tqj.meibo888.top

(x * 2 for x in arr)
来源：http://omx.feifeiyinyue.top

[U12] Py：取出现最多的 3 个元素
来源：http://bhm.shuidangran.top

Counter(arr).most_common(3)
来源：http://rdp.hfpthk.cn

[U13] Py：固定长度队列
来源：http://rte.hongshengwenyu.top

deque(maxlen=10)
来源：http://xbm.pengpengdd.cyou

[U14] Py：分组收集到列表
来源：http://rfp.yuxming.cn

defaultdict(list)
来源：http://elf.hfpthk.cn

[U15] Py：高精度计时
来源：http://juf.ctjpmb.com

t = time.perf_counter()
来源：http://gro.hcnkem.com

[U16] Py：命令行参数解析
来源：http://tib.fengsongda.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://tra.ivvv.top

[U17] Py：初始化日志
来源：http://fji.vehdjk.com

logging.basicConfig(level=logging.INFO)
来源：http://ing.fanxiaobao.xyz

[U18] Py：预编译正则
来源：http://lin.epnwcf.com

pat = re.compile(r"\d+")
来源：http://rir.yvedp.cn

[U19] Py：正则替换带回调
来源：http://yhn.jinghuilouyu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xob.aibaodan.cn

[U20] Py：缓存函数结果
来源：http://kkv.cashguo.top

@functools.lru_cache(maxsize=None)
来源：http://kve.52xcode.cn

[U21] Py：自定义上下文管理器
来源：http://xxw.sweek.top

@contextlib.contextmanager
来源：http://trf.ctjpmb.com

[U22] Py：矩阵转置
来源：http://hec.ydzc1.top

list(zip(*m))
来源：http://jep.hysaishi.cn

[U23] Py：分块读取大文件
来源：http://kwi.jlsjyb.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wny.tian-w.cn

[U24] Py：路径操作
来源：http://uxe.cdnleiting.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://agf.cqqwz.cn

[U25] Py：CSV 按字典读
来源：http://spc.xuetiantiany.cn

csv.DictReader(f)
来源：http://sic.vqdsnc.cn

[U26] Py：并发下载
来源：http://stf.sufxvd.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://whz.jlsjyb.cn

[U27] Py：异步 HTTP
来源：http://ovw.sxryk.cn

aiohttp.ClientSession() 配合 async with
来源：http://sbc.nanxuanxn.top

[U28] Py：类型别名
来源：http://woz.zhixingplan.top

UserId = int
来源：http://ugq.yvedp.cn

[U29] Py：属性校验
来源：http://hjs.tanke756.top

@property 与 @x.setter 配合
来源：http://fjh.xinyue.icu

[U30] Py：数据类
来源：http://kbc.zhiwuduotai.top

@dataclass(slots=True)
来源：http://iut.ybcxt.top

[U31] Py：单测
来源：http://hbv.sufxvd.cn

python -m pytest -q
来源：http://dsu.yongpay.top

[U32] Py：代码格式化
来源：http://ets.epnwcf.com

ruff format . && ruff check --fix .
来源：http://inn.epnwcf.com

[U33] Py：打包发布
来源：http://ard.jqgufenzy.top

python -m build  （依赖 pyproject.toml）
来源：http://dxl.svipenyu.cn

[U34] Py：判断编码
来源：http://bop.hnqzz.top

chardet.detect(raw)
来源：http://bsz.sysykeji.top

[U35] Py：发送邮件
来源：http://zos.hongshengwenyu.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://geu.hammf.cn

[U36] Py：定时任务
来源：http://gny.shzxlz.cn

schedule.every(10).minutes.do(job)
来源：http://dio.sufxvd.cn

[U37] Py：读写 Excel
来源：http://uix.gogol.net.cn

pandas.read_excel / DataFrame.to_excel
来源：http://poz.ydzc1.top

[U38] Py：获取脚本所在目录
来源：http://npt.hongshengwenyu.top

Path(__file__).resolve().parent
来源：http://kyg.aibaodan.cn

[U39] Py：判断是否在交互环境
来源：http://tci.bbcook.cn

sys.stdout.isatty()
来源：http://cni.yuxming.cn

[U40] Py：打印到标准错误
来源：http://nby.xingfuxueyuan.xyz

print("err", file=sys.stderr)
来源：http://bvh.cashguo.top

[U41] PHP：初始化 Composer 项目
来源：http://gad.meibo888.top

composer init;  composer require guzzlehttp/guzzle
来源：http://yke.ppjwa.cn

[U42] PHP：PSR-4 自动加载
来源：http://lnl.hnqzz.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://btf.redwolf501.top

[U43] PHP：声明命名空间
来源：http://uvc.hysaishi.cn

namespace App\Http;
来源：http://unx.yvedp.cn

[U44] PHP：开启严格类型
来源：http://xpn.ivvv.top

declare(strict_types=1);
来源：http://fpk.hnqzz.top

[U45] PHP：类型声明与返回类型
来源：http://aee.jinqigufen.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://mhy.ywan-chungtsiang.top

[U46] PHP：可空类型
来源：http://spr.zhengqikj.top

?string $name = null
来源：http://cbb.ctjpmb.com

[U47] PHP：联合类型
来源：http://xun.yonumen.top

int|string $id
来源：http://iia.tianlin.xyz

[U48] PHP：纯枚举
来源：http://hgb.quarkkingdee.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cbr.meibo888.top

[U49] PHP：只读属性
来源：http://gqq.hongshengwenyu.top

public readonly string $name
来源：http://vfw.ivvv.top

[U50] PHP：构造器属性提升
来源：http://bbw.shanyushiyangkeji.top

public function __construct(private int $id) {}
来源：http://nzu.svipenyu.cn

[U51] PHP：数组解构
来源：http://yid.vqdsnc.cn

[$a, $b] = $arr;
来源：http://oyq.vehdjk.com

[U52] PHP：箭头函数
来源：http://quj.hnxiangtu.top

$double = fn($x) => $x * 2;
来源：http://soc.ivvv.top

[U53] PHP：空合并运算符
来源：http://hny.gaohongyu789.top

$v = $a ?? $b ?? "default";
来源：http://hsl.vqdsnc.cn

[U54] PHP：空安全调用
来源：http://oex.wangshuangyany.cn

$obj?->method()
来源：http://nrx.yj20258888.top

[U55] PHP：match 表达式
来源：http://fgm.tarul.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://eek.bjfxy.top

[U56] PHP：命名参数
来源：http://ycc.nwbrower.top

f(a: 1, b: 2)
来源：http://xsi.316326.xyz

[U57] PHP：字符串插值
来源：http://ypz.nanxuanxn.top

"值: {$a}"
来源：http://uzu.shangyingyoupin.top

[U58] PHP：数组三件套
来源：http://vsi.birdmap.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://yph.aibaodan.cn

[U59] PHP：自定义排序
来源：http://hwx.hammf.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://njr.hysaishi.cn

[U60] PHP：JSON 编解码
来源：http://zyf.iojbl.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jxo.sysykeji.top

[U61] PHP：正则
来源：http://kye.pengpengdd.cyou

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cro.bjfxy.top

[U62] PHP：日期对象
来源：http://dmw.svipenyu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nrc.guannengcc.top

[U63] PHP：文件读写
来源：http://gzs.shzxlz.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rsf.hesvh.cn

[U64] PHP：目录遍历
来源：http://bzl.xuanzx.com

glob("dir/*.php");  scandir("dir");
来源：http://whr.zhiwuduotai.top

[U65] PHP：会话
来源：http://rtn.xziqi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://vmy.vehdjk.com

[U66] PHP：设置 Cookie
来源：http://wfn.zhixingplan.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ffa.wangshuangyany.cn

[U67] PHP：处理文件上传
来源：http://mxd.ybcxt.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fzj.zhixingplan.top

[U68] PHP：PDO 连接
来源：http://czd.0kj1m.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zlm.ydzc1.top

[U69] PHP：PDO 预处理
来源：http://hqm.shuidangran.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://snb.yvedp.cn

[U70] PHP：PDO 事务
来源：http://tbp.nanxinkj.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://drq.hongshengwenyu.top

[U71] PHP：抛出异常
来源：http://ytb.ywan-chungtsiang.top

throw new RuntimeException("失败", 500);
来源：http://rxn.hfpthk.cn

[U72] PHP：写错误日志
来源：http://onl.uphjek.com

error_log("失败: " . $e->getMessage());
来源：http://uba.316326.xyz

[U73] PHP：读取 ini 配置
来源：http://xsr.xziqi.cn

parse_ini_file("config.ini", true)
来源：http://qol.xingfuxueyuan.xyz

[U74] PHP：读取环境变量
来源：http://coe.jyoumei.cn

getenv("APP_ENV") ?: "production"
来源：http://cdo.jyoumei.cn

[U75] PHP：依赖注入
来源：http://geh.pycfn.com

composer require psr/container
来源：http://ene.hcnkem.com

[U76] PHP：简单路由
来源：http://qeb.hywenlv.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zkp.snrcjt.cn

[U77] PHP：模板渲染
来源：http://zef.feifeiyinyue.top

composer require twig/twig
来源：http://qqm.redwolf501.top

[U78] PHP：单元测试
来源：http://rhc.epnwcf.com

composer require --dev phpunit/phpunit
来源：http://nvx.yj20258.top

[U79] PHP：静态分析
来源：http://ppg.iojbl.cn

composer require --dev phpstan/phpstan
来源：http://viu.sjlbkw.cn

[U80] PHP：代码规范修复
来源：http://gjp.cqqwz.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://szt.jlsjyb.cn

[U81] JS：初始化项目
来源：http://gzb.dashuyun.cn

npm init -y;  npm i express
来源：http://ljh.xziqi.cn

[U82] JS：package.json 脚本
来源：http://qys.jlsjyb.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://srr.chenzaomai.com

[U83] JS：ES Module 导入导出
来源：http://pql.xinyue.icu

export const a = 1;  import { a } from "./m.js";
来源：http://jce.yj20258888.top

[U84] JS：CommonJS 写法
来源：http://qsp.zdbjq.cn

module.exports = { a };  const { a } = require("./m");
来源：http://chp.sysykeji.top

[U85] JS：可选链
来源：http://osn.jinqigfzy.top

a?.b?.c
来源：http://knk.yonumen.top

[U86] JS：空值合并
来源：http://xgs.gzhubu.top

a ?? b
来源：http://zzv.zycfv.cn

[U87] JS：解构默认值
来源：http://zsu.dashuyun.cn

const { a = 1, b = 2 } = obj;
来源：http://eve.xuetiantiany.cn

[U88] JS：对象展开合并
来源：http://rxv.chenlongwang.top

{ ...a, ...b }
来源：http://ate.snrcjt.cn

[U89] JS：数组去重
来源：http://buh.birdmap.top

[...new Set(arr)]
来源：http://pgy.jianghu66.top

[U90] JS：数字数组排序
来源：http://czi.redwolf501.top

[...arr].sort((a, b) => a - b)
来源：http://apb.sysykeji.top

[U91] JS：对象键值遍历
来源：http://gle.chenzaomai.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gob.jianghu66.top

[U92] JS：深拷贝
来源：http://txj.zhoulong.xyz

structuredClone(obj)
来源：http://bku.fanxiaobao.xyz

[U93] JS：模板字符串
来源：http://vge.chenjidiqi.icu

`共 ${n} 条`
来源：http://pfb.vqdsnc.cn

[U94] JS：箭头函数
来源：http://okx.cqqwz.cn

const double = x => x * 2;
来源：http://tif.zhoulong.xyz

[U95] JS：Promise 包装
来源：http://yin.hammf.cn

new Promise((resolve, reject) => {})
来源：http://xzn.hongshengwenyu.top

[U96] JS：async/await 与异常
来源：http://ump.quarkkingdee.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zha.yfazqb.com

[U97] JS：并发请求
来源：http://kel.sjlbkw.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://yls.ybcxt.top

[U98] JS：fetch 带 JSON
来源：http://bhf.hcnkem.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mjo.yueranfly.top

[U99] JS：事件监听
来源：http://xzw.svipenyu.cn

el.addEventListener("click", e => {})
来源：http://mnj.jinyuanbaomall.cn

[U100] JS：DOM 查询
来源：http://xin.ybcxt.top

document.querySelector(".item")
来源：http://oec.yj20258.top

[U101] JS：classList 操作
来源：http://ufm.fzhhl.top

el.classList.toggle("active")
来源：http://eer.yvedp.cn

[U102] JS：本地存储
来源：http://vei.zhongyouzk.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://acp.daria6918.cn

[U103] JS：定时器
来源：http://efy.fehbvm.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://uqh.shangyingyoupin.top

[U104] JS：防抖
来源：http://fua.gaohongyu789.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gxr.daxiang520.top

[U105] JS：节流
来源：http://sgf.fengsongda.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://utn.zycfv.cn

[U106] JS：日期格式化
来源：http://wtn.zdqjudy.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ihp.jqgfzy.top

[U107] JS：数字千分位
来源：http://sut.yj202588.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://djk.tanke756.top

[U108] JS：随机整数
来源：http://vio.zycfv.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dqe.cucudq.cn

[U109] JS：数组分组
来源：http://vuh.gaohongyu789.top

Object.groupBy(arr, x => x.type)
来源：http://kxe.gogol.net.cn

[U110] JS：数组分块
来源：http://rva.tanke756.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://iue.yj20258888.top

[U111] JS：对象转 Map
来源：http://rci.yanxiufei.cn

new Map(Object.entries(obj))
来源：http://sqt.tian-w.cn

[U112] JS：字符串补位
来源：http://ftl.yj20258.top

"7".padStart(3, "0")
来源：http://qjy.yonumen.top

[U113] JS：正则替换全部
来源：http://qak.aizwys.cn

s.replaceAll("a", "b")
来源：http://dyz.smart0.xyz

[U114] JS：JSON 深比较
来源：http://gml.fanxiaobao.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://ico.tanke756.top

[U115] JS：生成 UUID
来源：http://cmo.c1oappe.top

crypto.randomUUID()
来源：http://meg.fanxiaobao.xyz

[U116] JS：类型检查（JSDoc）
来源：http://ijg.jqgfzy.top

/** @param {string} name */ function f(name) {}
来源：http://zgw.quarkkingdee.top

[U117] JS：单元测试
来源：http://yfz.yj20258.top

npm i -D vitest;  npx vitest
来源：http://wlv.chenjidiqi.icu

[U118] JS：开发服务器
来源：http://qwh.hfpthk.cn

npm i -D vite;  npx vite
来源：http://yle.zdqjudy.top

[U119] JS：生产构建
来源：http://eiz.andypj.xyz

npx vite build
来源：http://vcl.chenjidiqi.icu

[U120] JS：读取环境变量（Vite）
来源：http://kaj.andypj.xyz

import.meta.env.VITE_API_URL
来源：http://lcx.wangshuangyany.cn

================================================================================
来源：http://xrz.cashguo.top

统计汇总
来源：http://lep.redwolf501.top

================================================================================
来源：http://lgn.yfazqb.com

按语言统计（条）：
来源：http://epo.epnwcf.com

Python ......... 252
来源：http://scl.zdqjudy.top

PHP ............ 252
来源：http://ojj.birdmap.top

JavaScript ..... 252
来源：http://ugs.xuetiantiany.cn

TypeScript ..... 212
来源：http://nza.jinyuanbaomall.cn

Java ........... 212
来源：http://vey.sjlbkw.cn

Go ............. 212
来源：http://wqv.nwbrower.top

Ruby ........... 212
来源：http://njw.chenjidiqi.icu

C# ............. 212
来源：http://oig.yfazqb.com

C .............. 30
来源：http://mms.tian-w.cn

C++ ............ 30
来源：http://hhf.vehdjk.com

SQL ............ 90
来源：http://zrl.bbcook.cn

Bash ........... 80
来源：http://slb.zhoulong.xyz

Kotlin ......... 15
来源：http://wwb.guowangkeji.top

Swift .......... 15
来源：http://cll.shanyushiyangtech.top

Lua ............ 10
来源：http://god.zhijiandao.cn

Perl ........... 10
来源：http://eek.havefunace.top

Scala .......... 10
来源：http://umi.meibo888.top

------------------------------------
来源：http://rkr.nanxinkj.top

合计 ........... 2106 条
来源：http://pkx.chenlongwang.top

按章节统计：
来源：http://xfm.ehwqpu.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jnz.tanke756.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://euo.tarul.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jaz.cucudq.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gxv.9152youxi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nqi.zhoulong.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://jlh.aizwys.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://unu.ybcxt.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zmy.vqdsnc.cn


<!-- 参考信息 -->