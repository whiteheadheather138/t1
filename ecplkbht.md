代发 wailian999

[T47] Perl：正则捕获
来源：http://hpi.feifeiyinyue.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://aud.jqgufenzy.top

[T48] Perl：正则替换
来源：http://jbb.jinqigfzy.top

$s =~ s/old/new/g;
来源：http://tgv.sweek.top

[T49] Perl：函数
来源：http://mah.jyoumei.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://bvv.guowangkeji.top

[T50] Perl：逐行读文件
来源：http://jzf.gogol.net.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://uym.ivvv.top

while (my $line = <$fh>) { print $line; }
来源：http://ahu.316326.xyz

[T51] Scala：Hello World
来源：http://mir.svipenyu.cn

println("Hello")
来源：http://ute.tanke756.top

[T52] Scala：变量
来源：http://lbu.sxryk.cn

val a = 1;  var b = 2
来源：http://zjo.shzxlz.cn

[T53] Scala：字符串插值
来源：http://rwg.xuanzx.com

s"值: $b"
来源：http://jga.yvedp.cn

[T54] Scala：集合映射
来源：http://fwo.guowangkeji.top

List(1, 2, 3).map(_ * 2)
来源：http://fnm.svipenyu.cn

[T55] Scala：集合过滤
来源：http://fxi.zhiwuduotai.top

List(1, 2, 3).filter(_ > 1)
来源：http://iqb.xuanzx.com

[T56] Scala：样例类
来源：http://guc.sysykeji.top

case class User(name: String, age: Int)
来源：http://npl.shanyushiyangtech.top

[T57] Scala：模式匹配
来源：http://auh.nwbrower.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://uck.hesvh.cn

[T58] Scala：函数定义
来源：http://ekz.chenzaomai.com

def add(a: Int, b: Int): Int = a + b
来源：http://ywy.shangyingyoupin.top

[T59] Scala：循环
来源：http://dja.316326.xyz

for (i <- 1 to 10) println(i)
来源：http://xlu.ybcxt.top

[T60] Scala：折叠
来源：http://dvq.vehdjk.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rhp.yj202588.top

================================================================================
来源：http://ijl.gogol.net.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vju.gotoacloud.top

================================================================================
来源：http://izb.snrcjt.cn

[U01] Py：创建虚拟环境
来源：http://gsq.bjfxy.top

python -m venv .venv && source .venv/bin/activate
来源：http://max.epnwcf.com

[U02] Py：导出 / 安装依赖
来源：http://vxt.cucudq.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ksd.uphjek.com

[U03] Py：加载 .env 配置
来源：http://zwm.meibo888.top

from dotenv import load_dotenv; load_dotenv()
来源：http://zcy.wangdashe.top

[U04] Py：变量调试打印
来源：http://msa.chenlongwang.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nen.yj20258888.top

[U05] Py：列表去重且保序
来源：http://qkn.tianlin.xyz

list(dict.fromkeys(arr))
来源：http://rwa.chenjidiqi.icu

[U06] Py：合并两个字典
来源：http://wwf.mhx1999.top

{**a, **b}
来源：http://tmp.smart0.xyz

[U07] Py：反转字典键值
来源：http://bqc.cashguo.top

{v: k for k, v in d.items()}
来源：http://roy.tarul.cn

[U08] Py：展平二维列表
来源：http://jsc.snrcjt.cn

[y for x in nested for y in x]
来源：http://ahu.xinyue.icu

[U09] Py：字典取最大值的键
来源：http://lzs.xinyue.icu

max(d, key=d.get)
来源：http://gqq.zycfv.cn

[U10] Py：按值排序字典
来源：http://efi.vqdsnc.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://klh.zhongyouzk.top

[U11] Py：生成器表达式
来源：http://mde.yfazqb.com

(x * 2 for x in arr)
来源：http://nmn.ywan-chungtsiang.top

[U12] Py：取出现最多的 3 个元素
来源：http://jrq.cashguo.top

Counter(arr).most_common(3)
来源：http://xsb.pycfn.com

[U13] Py：固定长度队列
来源：http://prf.wangshuangyany.cn

deque(maxlen=10)
来源：http://umg.pengpengdd.cyou

[U14] Py：分组收集到列表
来源：http://wnz.aizwys.cn

defaultdict(list)
来源：http://csq.hywenlv.cn

[U15] Py：高精度计时
来源：http://jgn.birdmap.top

t = time.perf_counter()
来源：http://mmd.zhijiandao.cn

[U16] Py：命令行参数解析
来源：http://zyh.jqgufenzy.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ics.ydzc1.top

[U17] Py：初始化日志
来源：http://yue.birdmap.top

logging.basicConfig(level=logging.INFO)
来源：http://phw.pycfn.com

[U18] Py：预编译正则
来源：http://yja.jyoumei.cn

pat = re.compile(r"\d+")
来源：http://ubd.bjfxy.top

[U19] Py：正则替换带回调
来源：http://jap.gogol.net.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://iwx.vqdsnc.cn

[U20] Py：缓存函数结果
来源：http://rrz.jlsjyb.cn

@functools.lru_cache(maxsize=None)
来源：http://yut.havefunace.top

[U21] Py：自定义上下文管理器
来源：http://kiq.jinqigufen.top

@contextlib.contextmanager
来源：http://goj.jinyuanbaomall.cn

[U22] Py：矩阵转置
来源：http://tfd.ehwqpu.com

list(zip(*m))
来源：http://ndo.yuxming.cn

[U23] Py：分块读取大文件
来源：http://ysu.hcnkem.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://onc.ctjpmb.com

[U24] Py：路径操作
来源：http://uhw.jinqigufen.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://avv.zycfv.cn

[U25] Py：CSV 按字典读
来源：http://rhn.nanxinkj.top

csv.DictReader(f)
来源：http://fkr.xingfuxueyuan.xyz

[U26] Py：并发下载
来源：http://mda.jiagoushi.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qkj.aibaodan.cn

[U27] Py：异步 HTTP
来源：http://ztn.andypj.xyz

aiohttp.ClientSession() 配合 async with
来源：http://zlp.fehbvm.com

[U28] Py：类型别名
来源：http://hba.sweek.top

UserId = int
来源：http://ner.hnqzz.top

[U29] Py：属性校验
来源：http://uft.gaohongyu789.top

@property 与 @x.setter 配合
来源：http://esi.snrcjt.cn

[U30] Py：数据类
来源：http://jkv.zhongyouzk.top

@dataclass(slots=True)
来源：http://pcm.ybcxt.top

[U31] Py：单测
来源：http://yge.yongpay.top

python -m pytest -q
来源：http://ouz.bjfxy.top

[U32] Py：代码格式化
来源：http://cvf.zycfv.cn

ruff format . && ruff check --fix .
来源：http://hgh.chenlongwang.top

[U33] Py：打包发布
来源：http://soi.c1oappe.top

python -m build  （依赖 pyproject.toml）
来源：http://lpr.sjlbkw.cn

[U34] Py：判断编码
来源：http://mfu.yuanzhike.top

chardet.detect(raw)
来源：http://xyl.sweek.top

[U35] Py：发送邮件
来源：http://vcx.ctjpmb.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://asm.mhx1999.top

[U36] Py：定时任务
来源：http://bop.smart0.xyz

schedule.every(10).minutes.do(job)
来源：http://nfi.yonumen.top

[U37] Py：读写 Excel
来源：http://fsn.ivvv.top

pandas.read_excel / DataFrame.to_excel
来源：http://vmx.iojbl.cn

[U38] Py：获取脚本所在目录
来源：http://prq.daria6918.cn

Path(__file__).resolve().parent
来源：http://cxg.zhoulong.xyz

[U39] Py：判断是否在交互环境
来源：http://exu.smart0.xyz

sys.stdout.isatty()
来源：http://qmj.sufxvd.cn

[U40] Py：打印到标准错误
来源：http://pjb.xinyue.icu

print("err", file=sys.stderr)
来源：http://udu.bjfxy.top

[U41] PHP：初始化 Composer 项目
来源：http://jtd.smart0.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://qow.tianlin.xyz

[U42] PHP：PSR-4 自动加载
来源：http://vyd.hcnkem.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hpi.9152youxi.cn

[U43] PHP：声明命名空间
来源：http://ohs.aibaodan.cn

namespace App\Http;
来源：http://wmd.chenlongwang.top

[U44] PHP：开启严格类型
来源：http://ddm.zhengqikj.top

declare(strict_types=1);
来源：http://bat.nanxuanxn.top

[U45] PHP：类型声明与返回类型
来源：http://vot.yj202588.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://fmx.jqgufenzy.top

[U46] PHP：可空类型
来源：http://ykg.pengpengdd.cyou

?string $name = null
来源：http://iwr.zycfv.cn

[U47] PHP：联合类型
来源：http://ifo.redwolf501.top

int|string $id
来源：http://ouo.xuetiantiany.cn

[U48] PHP：纯枚举
来源：http://tsf.yongpay.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qbo.jqgufenzy.top

[U49] PHP：只读属性
来源：http://yzf.cashguo.top

public readonly string $name
来源：http://bcc.pycfn.com

[U50] PHP：构造器属性提升
来源：http://gkf.jianghu66.top

public function __construct(private int $id) {}
来源：http://brc.ydzc1.top

[U51] PHP：数组解构
来源：http://wec.ydjk.org.cn

[$a, $b] = $arr;
来源：http://dff.yuanzhike.top

[U52] PHP：箭头函数
来源：http://nik.andypj.xyz

$double = fn($x) => $x * 2;
来源：http://jks.316326.xyz

[U53] PHP：空合并运算符
来源：http://vru.sweek.top

$v = $a ?? $b ?? "default";
来源：http://rsp.vehdjk.com

[U54] PHP：空安全调用
来源：http://xzl.zdbjq.cn

$obj?->method()
来源：http://zna.chenzaomai.com

[U55] PHP：match 表达式
来源：http://fho.zdqjudy.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://sty.sxryk.cn

[U56] PHP：命名参数
来源：http://gxw.yangfankeji.com

f(a: 1, b: 2)
来源：http://aje.guowangkeji.top

[U57] PHP：字符串插值
来源：http://kyu.fktsv.cn

"值: {$a}"
来源：http://jhh.vehdjk.com

[U58] PHP：数组三件套
来源：http://flg.hnqzz.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://htu.yueranfly.top

[U59] PHP：自定义排序
来源：http://dky.shanyushiyangkeji.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://foe.daria6918.cn

[U60] PHP：JSON 编解码
来源：http://qjt.yfazqb.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fqa.cqqwz.cn

[U61] PHP：正则
来源：http://bxy.cheryme.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xcs.andypj.xyz

[U62] PHP：日期对象
来源：http://fet.fehbvm.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://uwx.smart0.xyz

[U63] PHP：文件读写
来源：http://bhp.daria6918.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ugz.haohaochexian.top

[U64] PHP：目录遍历
来源：http://slh.shzxlz.cn

glob("dir/*.php");  scandir("dir");
来源：http://uqa.guowangkeji.top

[U65] PHP：会话
来源：http://fei.yj20258.top

session_start();  $_SESSION["uid"] = 1;
来源：http://kqe.yuxming.cn

[U66] PHP：设置 Cookie
来源：http://lcv.c1oappe.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://boc.kuanghao11.cn

[U67] PHP：处理文件上传
来源：http://okp.vehdjk.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://luf.ivvv.top

[U68] PHP：PDO 连接
来源：http://qgm.jqgufenzy.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rvq.ydzc1.top

[U69] PHP：PDO 预处理
来源：http://cln.kuanghao11.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nvs.xziqi.cn

[U70] PHP：PDO 事务
来源：http://ntv.cashguo.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://msf.hnxiangtu.top

[U71] PHP：抛出异常
来源：http://muj.9152youxi.cn

throw new RuntimeException("失败", 500);
来源：http://epb.pengpengdd.cyou

[U72] PHP：写错误日志
来源：http://obx.feifeiyinyue.top

error_log("失败: " . $e->getMessage());
来源：http://jry.xuanzx.com

[U73] PHP：读取 ini 配置
来源：http://sah.nwbrower.top

parse_ini_file("config.ini", true)
来源：http://tql.jinghuilouyu.cn

[U74] PHP：读取环境变量
来源：http://imu.nwbrower.top

getenv("APP_ENV") ?: "production"
来源：http://vbm.ehwqpu.com

[U75] PHP：依赖注入
来源：http://hzd.yonumen.top

composer require psr/container
来源：http://tdz.svipenyu.cn

[U76] PHP：简单路由
来源：http://lcg.jianghu66.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rht.cashguo.top

[U77] PHP：模板渲染
来源：http://pxs.ywan-chungtsiang.top

composer require twig/twig
来源：http://ivp.zdbjq.cn

[U78] PHP：单元测试
来源：http://cne.yuxming.cn

composer require --dev phpunit/phpunit
来源：http://qfs.andypj.xyz

[U79] PHP：静态分析
来源：http://ccd.yj20258.top

composer require --dev phpstan/phpstan
来源：http://hos.ydzc1.top

[U80] PHP：代码规范修复
来源：http://uhp.0kj1m.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://vvw.daxiang520.top

[U81] JS：初始化项目
来源：http://cig.andypj.xyz

npm init -y;  npm i express
来源：http://mvz.aizwys.cn

[U82] JS：package.json 脚本
来源：http://bnu.jinqigfzy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://luz.zhengqikj.top

[U83] JS：ES Module 导入导出
来源：http://ddp.daria6918.cn

export const a = 1;  import { a } from "./m.js";
来源：http://siu.mhx1999.top

[U84] JS：CommonJS 写法
来源：http://yyu.ybcxt.top

module.exports = { a };  const { a } = require("./m");
来源：http://ziq.jinqigufen.top

[U85] JS：可选链
来源：http://zjm.shzxlz.cn

a?.b?.c
来源：http://owt.hongshengwenyu.top

[U86] JS：空值合并
来源：http://avo.cheryme.top

a ?? b
来源：http://vfr.bjfxy.top

[U87] JS：解构默认值
来源：http://snw.hnxiangtu.top

const { a = 1, b = 2 } = obj;
来源：http://npm.quarkkingdee.top

[U88] JS：对象展开合并
来源：http://ckm.jinqigufen.top

{ ...a, ...b }
来源：http://uge.jianghu66.top

[U89] JS：数组去重
来源：http://bvy.iojbl.cn

[...new Set(arr)]
来源：http://uao.fanxiaobao.xyz

[U90] JS：数字数组排序
来源：http://woi.hysaishi.cn

[...arr].sort((a, b) => a - b)
来源：http://tog.guowangkeji.top

[U91] JS：对象键值遍历
来源：http://tpr.hfpthk.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zuy.hongshengwenyu.top

[U92] JS：深拷贝
来源：http://stt.xylfe.cn

structuredClone(obj)
来源：http://eax.yj202588.top

[U93] JS：模板字符串
来源：http://uwr.xziqi.cn

`共 ${n} 条`
来源：http://xmi.zhaomingkeji.xyz

[U94] JS：箭头函数
来源：http://nwm.cucudq.cn

const double = x => x * 2;
来源：http://pof.zycfv.cn

[U95] JS：Promise 包装
来源：http://gmm.yj20258888.top

new Promise((resolve, reject) => {})
来源：http://pyo.jinqigufen.top

[U96] JS：async/await 与异常
来源：http://otq.jinghuilouyu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xcq.meibo888.top

[U97] JS：并发请求
来源：http://sjd.sxryk.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://edb.zhijiandao.cn

[U98] JS：fetch 带 JSON
来源：http://orb.shangyingyoupin.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://dnr.cucudq.cn

[U99] JS：事件监听
来源：http://yxr.jinyuanbaomall.cn

el.addEventListener("click", e => {})
来源：http://ckr.pengpengdd.cyou

[U100] JS：DOM 查询
来源：http://qlc.hysaishi.cn

document.querySelector(".item")
来源：http://xhd.ppjwa.cn

[U101] JS：classList 操作
来源：http://fpy.chenzaomai.com

el.classList.toggle("active")
来源：http://gkm.xingfuxueyuan.xyz

[U102] JS：本地存储
来源：http://oda.gaohongyu789.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://wod.zycfv.cn

[U103] JS：定时器
来源：http://ltw.cdnleiting.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kdh.kuanghao11.cn

[U104] JS：防抖
来源：http://zci.jyoumei.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ezr.sweek.top

[U105] JS：节流
来源：http://qjz.yongpay.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lpc.yj20258888.top

[U106] JS：日期格式化
来源：http://lbh.yj20258.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lkl.xylfe.cn

[U107] JS：数字千分位
来源：http://gxx.xinyue.icu

new Intl.NumberFormat("en-US").format(1234567)
来源：http://iqf.ivvv.top

[U108] JS：随机整数
来源：http://jra.iojbl.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pgk.xingfuxueyuan.xyz

[U109] JS：数组分组
来源：http://mbj.ivvv.top

Object.groupBy(arr, x => x.type)
来源：http://znc.hnxiangtu.top

[U110] JS：数组分块
来源：http://suc.hcnkem.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jqx.shanyushiyangtech.top

[U111] JS：对象转 Map
来源：http://bfo.sufxvd.cn

new Map(Object.entries(obj))
来源：http://kbf.shangyingyoupin.top

[U112] JS：字符串补位
来源：http://dsu.jyoumei.cn

"7".padStart(3, "0")
来源：http://rqx.0kj1m.cn

[U113] JS：正则替换全部
来源：http://axu.jyoumei.cn

s.replaceAll("a", "b")
来源：http://ffl.ywan-chungtsiang.top

[U114] JS：JSON 深比较
来源：http://ttp.sweek.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://zea.bbcook.cn

[U115] JS：生成 UUID
来源：http://ylx.dianchejie.cn

crypto.randomUUID()
来源：http://lkm.jinyuanbaomall.cn

[U116] JS：类型检查（JSDoc）
来源：http://xvo.zhixingplan.top

/** @param {string} name */ function f(name) {}
来源：http://ijp.yj20258.top

[U117] JS：单元测试
来源：http://zoc.xziqi.cn

npm i -D vitest;  npx vitest
来源：http://wpz.fktsv.cn

[U118] JS：开发服务器
来源：http://brz.chenlongwang.top

npm i -D vite;  npx vite
来源：http://zjn.guannengcc.top

[U119] JS：生产构建
来源：http://vyh.hammf.cn

npx vite build
来源：http://crp.fanxiaobao.xyz

[U120] JS：读取环境变量（Vite）
来源：http://ced.chenlongwang.top

import.meta.env.VITE_API_URL
来源：http://gej.hcnkem.com

================================================================================
来源：http://ufn.zhongyouzk.top

统计汇总
来源：http://dqg.sufxvd.cn

================================================================================
来源：http://xtw.yangfankeji.com

按语言统计（条）：
来源：http://mtq.aizwys.cn

Python ......... 252
来源：http://pwk.yongpay.top

PHP ............ 252
来源：http://gxy.yangfankeji.com

JavaScript ..... 252
来源：http://wjx.wangdashe.top

TypeScript ..... 212
来源：http://txl.hesvh.cn

Java ........... 212
来源：http://kaf.9152youxi.cn

Go ............. 212
来源：http://dkf.hnxiangtu.top

Ruby ........... 212
来源：http://ivq.gaohongyu789.top

C# ............. 212
来源：http://tnq.dianchejie.cn

C .............. 30
来源：http://viy.yangfankeji.com

C++ ............ 30
来源：http://gqn.hnxiangtu.top

SQL ............ 90
来源：http://oan.aizwys.cn

Bash ........... 80
来源：http://itq.quarkkingdee.top

Kotlin ......... 15
来源：http://ipw.yanxiufei.cn

Swift .......... 15
来源：http://fgk.hongshengwenyu.top

Lua ............ 10
来源：http://cmr.sweek.top

Perl ........... 10
来源：http://tkq.shangyingyoupin.top

Scala .......... 10
来源：http://jnk.yuanzhike.top

------------------------------------
来源：http://pfx.zhoulong.xyz

合计 ........... 2106 条
来源：http://pch.yj202588.top

按章节统计：
来源：http://hlg.cucudq.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vce.yuxming.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qjt.meibo888.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ynf.kuanghao11.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ksn.316326.xyz


<!-- 参考信息 -->