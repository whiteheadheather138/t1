代发 wailian999

[T45] Perl：数组遍历
来源：http://msm.cheryme.top

for my $x (@arr) { print $x; }
来源：http://jyo.hcnkem.com

[T46] Perl：哈希操作
来源：http://pma.c1oappe.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ewz.guowangkeji.top

[T47] Perl：正则捕获
来源：http://wcm.jiagoushi.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://qha.zhengqikj.top

[T48] Perl：正则替换
来源：http://css.zhaomingkeji.xyz

$s =~ s/old/new/g;
来源：http://ffp.ywan-chungtsiang.top

[T49] Perl：函数
来源：http://igg.yj202588.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://iyf.52xcode.cn

[T50] Perl：逐行读文件
来源：http://vga.zhiwuduotai.top

open my $fh, "<", "a.txt" or die $!;
来源：http://czm.hongshengwenyu.top

while (my $line = <$fh>) { print $line; }
来源：http://wgv.cucudq.cn

[T51] Scala：Hello World
来源：http://zcb.iojbl.cn

println("Hello")
来源：http://jml.hnxiangtu.top

[T52] Scala：变量
来源：http://nkx.guannengcc.top

val a = 1;  var b = 2
来源：http://lhe.yonumen.top

[T53] Scala：字符串插值
来源：http://nlw.shzxlz.cn

s"值: $b"
来源：http://cfm.0kj1m.cn

[T54] Scala：集合映射
来源：http://yae.aibaodan.cn

List(1, 2, 3).map(_ * 2)
来源：http://zag.guowangkeji.top

[T55] Scala：集合过滤
来源：http://jlz.fzhhl.top

List(1, 2, 3).filter(_ > 1)
来源：http://ewi.chenlongwang.top

[T56] Scala：样例类
来源：http://ncu.shangyingyoupin.top

case class User(name: String, age: Int)
来源：http://crb.dianchejie.cn

[T57] Scala：模式匹配
来源：http://mug.yuxming.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ago.guannengcc.top

[T58] Scala：函数定义
来源：http://asa.xylfe.cn

def add(a: Int, b: Int): Int = a + b
来源：http://loj.jinqigfzy.top

[T59] Scala：循环
来源：http://iei.xziqi.cn

for (i <- 1 to 10) println(i)
来源：http://srd.shanyushiyangtech.top

[T60] Scala：折叠
来源：http://dwx.cqqwz.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jit.uphjek.com

================================================================================
来源：http://dto.jinyuanbaomall.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zlc.hysaishi.cn

================================================================================
来源：http://vei.cheryme.top

[U01] Py：创建虚拟环境
来源：http://geg.hcnkem.com

python -m venv .venv && source .venv/bin/activate
来源：http://ebb.jinqigfzy.top

[U02] Py：导出 / 安装依赖
来源：http://asr.xuanzx.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nhk.jlsjyb.cn

[U03] Py：加载 .env 配置
来源：http://bov.tianlin.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://lxe.jinqigufen.top

[U04] Py：变量调试打印
来源：http://vfk.c1oappe.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ugl.vehdjk.com

[U05] Py：列表去重且保序
来源：http://fzz.gotoacloud.top

list(dict.fromkeys(arr))
来源：http://cng.fktsv.cn

[U06] Py：合并两个字典
来源：http://gzq.ydzc1.top

{**a, **b}
来源：http://sha.ivvv.top

[U07] Py：反转字典键值
来源：http://krm.nanxinkj.top

{v: k for k, v in d.items()}
来源：http://uyt.tarul.cn

[U08] Py：展平二维列表
来源：http://tqn.52xcode.cn

[y for x in nested for y in x]
来源：http://uqy.fanxiaobao.xyz

[U09] Py：字典取最大值的键
来源：http://tfg.uphjek.com

max(d, key=d.get)
来源：http://ojf.yj20258888.top

[U10] Py：按值排序字典
来源：http://ipo.zycfv.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://skf.cashguo.top

[U11] Py：生成器表达式
来源：http://tns.jqgfzy.top

(x * 2 for x in arr)
来源：http://ooj.yangfankeji.com

[U12] Py：取出现最多的 3 个元素
来源：http://htb.yuxming.cn

Counter(arr).most_common(3)
来源：http://ddn.fengsongda.top

[U13] Py：固定长度队列
来源：http://pbt.epnwcf.com

deque(maxlen=10)
来源：http://gcr.xinyue.icu

[U14] Py：分组收集到列表
来源：http://cms.zhongyouzk.top

defaultdict(list)
来源：http://ofo.zhoulong.xyz

[U15] Py：高精度计时
来源：http://cdf.ehwqpu.com

t = time.perf_counter()
来源：http://tps.zdbjq.cn

[U16] Py：命令行参数解析
来源：http://aeq.cheryme.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://tui.zdbjq.cn

[U17] Py：初始化日志
来源：http://rnu.fzhhl.top

logging.basicConfig(level=logging.INFO)
来源：http://oid.yuanzhike.top

[U18] Py：预编译正则
来源：http://jzv.wangdashe.top

pat = re.compile(r"\d+")
来源：http://jox.wangshuangyany.cn

[U19] Py：正则替换带回调
来源：http://nfg.316326.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://res.yonumen.top

[U20] Py：缓存函数结果
来源：http://wke.guannengcc.top

@functools.lru_cache(maxsize=None)
来源：http://xux.epnwcf.com

[U21] Py：自定义上下文管理器
来源：http://biy.jiagoushi.top

@contextlib.contextmanager
来源：http://tsi.tian-w.cn

[U22] Py：矩阵转置
来源：http://uwh.yangfankeji.com

list(zip(*m))
来源：http://gif.guowangkeji.top

[U23] Py：分块读取大文件
来源：http://ndy.jlsjyb.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xxy.hesvh.cn

[U24] Py：路径操作
来源：http://wcc.havefunace.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hws.cucudq.cn

[U25] Py：CSV 按字典读
来源：http://viw.jinqigufen.top

csv.DictReader(f)
来源：http://bnk.0kj1m.cn

[U26] Py：并发下载
来源：http://nso.ydzc1.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zcw.nanxuanxn.top

[U27] Py：异步 HTTP
来源：http://juj.yueranfly.top

aiohttp.ClientSession() 配合 async with
来源：http://pcf.tianlin.xyz

[U28] Py：类型别名
来源：http://tdj.ivvv.top

UserId = int
来源：http://des.iojbl.cn

[U29] Py：属性校验
来源：http://rtj.xingfuxueyuan.xyz

@property 与 @x.setter 配合
来源：http://hrc.gzhubu.top

[U30] Py：数据类
来源：http://qxf.bbcook.cn

@dataclass(slots=True)
来源：http://xew.bbcook.cn

[U31] Py：单测
来源：http://sge.xylfe.cn

python -m pytest -q
来源：http://ouu.fzhhl.top

[U32] Py：代码格式化
来源：http://laj.daxiang520.top

ruff format . && ruff check --fix .
来源：http://kpo.hongshengwenyu.top

[U33] Py：打包发布
来源：http://wyt.yfazqb.com

python -m build  （依赖 pyproject.toml）
来源：http://uuh.fanxiaobao.xyz

[U34] Py：判断编码
来源：http://wdc.zdbjq.cn

chardet.detect(raw)
来源：http://xpc.bbcook.cn

[U35] Py：发送邮件
来源：http://ixs.yangfankeji.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gsk.hammf.cn

[U36] Py：定时任务
来源：http://fwn.dashuyun.cn

schedule.every(10).minutes.do(job)
来源：http://sdq.tianlin.xyz

[U37] Py：读写 Excel
来源：http://ynb.gzhubu.top

pandas.read_excel / DataFrame.to_excel
来源：http://gds.ehwqpu.com

[U38] Py：获取脚本所在目录
来源：http://hjz.sysykeji.top

Path(__file__).resolve().parent
来源：http://svj.ppjwa.cn

[U39] Py：判断是否在交互环境
来源：http://lzs.xylfe.cn

sys.stdout.isatty()
来源：http://jhm.hysaishi.cn

[U40] Py：打印到标准错误
来源：http://jcg.zhiwuduotai.top

print("err", file=sys.stderr)
来源：http://ydy.xinyue.icu

[U41] PHP：初始化 Composer 项目
来源：http://wlh.316326.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://mqs.zdqjudy.top

[U42] PHP：PSR-4 自动加载
来源：http://lad.xuetiantiany.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baz.cheryme.top

[U43] PHP：声明命名空间
来源：http://sfz.zhijiandao.cn

namespace App\Http;
来源：http://pze.yj202588.top

[U44] PHP：开启严格类型
来源：http://dmz.tarul.cn

declare(strict_types=1);
来源：http://bhc.xuanzx.com

[U45] PHP：类型声明与返回类型
来源：http://ksv.shangyingyoupin.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://scy.jyoumei.cn

[U46] PHP：可空类型
来源：http://whm.ybcxt.top

?string $name = null
来源：http://qkw.andypj.xyz

[U47] PHP：联合类型
来源：http://ijp.andypj.xyz

int|string $id
来源：http://xbh.ybcxt.top

[U48] PHP：纯枚举
来源：http://zlw.zdbjq.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://uwu.ywan-chungtsiang.top

[U49] PHP：只读属性
来源：http://gfw.fanxiaobao.xyz

public readonly string $name
来源：http://lsj.wangshuangyany.cn

[U50] PHP：构造器属性提升
来源：http://jlz.zdbjq.cn

public function __construct(private int $id) {}
来源：http://lvb.shangyingyoupin.top

[U51] PHP：数组解构
来源：http://wff.sweek.top

[$a, $b] = $arr;
来源：http://rdj.jyoumei.cn

[U52] PHP：箭头函数
来源：http://iwe.hywenlv.cn

$double = fn($x) => $x * 2;
来源：http://uuz.cdnleiting.top

[U53] PHP：空合并运算符
来源：http://jml.yongpay.top

$v = $a ?? $b ?? "default";
来源：http://dir.tianlin.xyz

[U54] PHP：空安全调用
来源：http://syr.xinyue.icu

$obj?->method()
来源：http://yti.shanyushiyangkeji.top

[U55] PHP：match 表达式
来源：http://cnx.sweek.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qun.bbcook.cn

[U56] PHP：命名参数
来源：http://psn.ydzc1.top

f(a: 1, b: 2)
来源：http://szj.andypj.xyz

[U57] PHP：字符串插值
来源：http://pey.daxiang520.top

"值: {$a}"
来源：http://tgu.hnxiangtu.top

[U58] PHP：数组三件套
来源：http://hnk.xinyue.icu

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nbm.gotoacloud.top

[U59] PHP：自定义排序
来源：http://zqs.ppjwa.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uxf.havefunace.top

[U60] PHP：JSON 编解码
来源：http://khd.c1oappe.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pdb.316326.xyz

[U61] PHP：正则
来源：http://cjw.hnxiangtu.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xqa.xuetiantiany.cn

[U62] PHP：日期对象
来源：http://eoo.birdmap.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rtv.fengsongda.top

[U63] PHP：文件读写
来源：http://cmp.hysaishi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xix.jqgufenzy.top

[U64] PHP：目录遍历
来源：http://ikn.cdnleiting.top

glob("dir/*.php");  scandir("dir");
来源：http://xcs.havefunace.top

[U65] PHP：会话
来源：http://add.cdnleiting.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ezc.jianghu66.top

[U66] PHP：设置 Cookie
来源：http://gba.nanxinkj.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mxb.yangfankeji.com

[U67] PHP：处理文件上传
来源：http://qjw.jinyuanbaomall.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zpx.guannengcc.top

[U68] PHP：PDO 连接
来源：http://wtm.jqgufenzy.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ryc.nwbrower.top

[U69] PHP：PDO 预处理
来源：http://eqv.ydzc1.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yxq.sjlbkw.cn

[U70] PHP：PDO 事务
来源：http://svc.zdbjq.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vvh.iojbl.cn

[U71] PHP：抛出异常
来源：http://mvm.cdnleiting.top

throw new RuntimeException("失败", 500);
来源：http://unl.hammf.cn

[U72] PHP：写错误日志
来源：http://hpu.fengsongda.top

error_log("失败: " . $e->getMessage());
来源：http://zzb.shanyushiyangtech.top

[U73] PHP：读取 ini 配置
来源：http://akt.kuanghao11.cn

parse_ini_file("config.ini", true)
来源：http://zly.ydzc1.top

[U74] PHP：读取环境变量
来源：http://sse.fengsongda.top

getenv("APP_ENV") ?: "production"
来源：http://ifc.hnqzz.top

[U75] PHP：依赖注入
来源：http://yna.sjlbkw.cn

composer require psr/container
来源：http://zts.sufxvd.cn

[U76] PHP：简单路由
来源：http://cug.guannengcc.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://let.yonumen.top

[U77] PHP：模板渲染
来源：http://akx.nwbrower.top

composer require twig/twig
来源：http://diq.chenzaomai.com

[U78] PHP：单元测试
来源：http://gzc.bjfxy.top

composer require --dev phpunit/phpunit
来源：http://lvn.gotoacloud.top

[U79] PHP：静态分析
来源：http://wkd.yongpay.top

composer require --dev phpstan/phpstan
来源：http://wzx.cqqwz.cn

[U80] PHP：代码规范修复
来源：http://ard.shzxlz.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://pmy.sjlbkw.cn

[U81] JS：初始化项目
来源：http://igr.andypj.xyz

npm init -y;  npm i express
来源：http://fsp.uphjek.com

[U82] JS：package.json 脚本
来源：http://pjj.yj20258888.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mdb.cheryme.top

[U83] JS：ES Module 导入导出
来源：http://aza.zhixingplan.top

export const a = 1;  import { a } from "./m.js";
来源：http://ods.yuxming.cn

[U84] JS：CommonJS 写法
来源：http://hek.jinghuilouyu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://vrj.hammf.cn

[U85] JS：可选链
来源：http://waa.zdqjudy.top

a?.b?.c
来源：http://wvu.meibo888.top

[U86] JS：空值合并
来源：http://eti.guannengcc.top

a ?? b
来源：http://zwx.daria6918.cn

[U87] JS：解构默认值
来源：http://xaf.jinyuanbaomall.cn

const { a = 1, b = 2 } = obj;
来源：http://pyo.fzhhl.top

[U88] JS：对象展开合并
来源：http://jac.bjfxy.top

{ ...a, ...b }
来源：http://umu.shanyushiyangtech.top

[U89] JS：数组去重
来源：http://nrb.shanyushiyangkeji.top

[...new Set(arr)]
来源：http://yim.daria6918.cn

[U90] JS：数字数组排序
来源：http://wlf.kuanghao11.cn

[...arr].sort((a, b) => a - b)
来源：http://jfh.fehbvm.com

[U91] JS：对象键值遍历
来源：http://ssr.fktsv.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mrn.zdbjq.cn

[U92] JS：深拷贝
来源：http://dcw.cheryme.top

structuredClone(obj)
来源：http://qrq.cashguo.top

[U93] JS：模板字符串
来源：http://tle.yonumen.top

`共 ${n} 条`
来源：http://fgc.fehbvm.com

[U94] JS：箭头函数
来源：http://dhh.hywenlv.cn

const double = x => x * 2;
来源：http://rxg.nwbrower.top

[U95] JS：Promise 包装
来源：http://gdv.sweek.top

new Promise((resolve, reject) => {})
来源：http://usx.jqgfzy.top

[U96] JS：async/await 与异常
来源：http://qsy.jiagoushi.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nra.gogol.net.cn

[U97] JS：并发请求
来源：http://ifl.cdnleiting.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://kcx.tanke756.top

[U98] JS：fetch 带 JSON
来源：http://bvi.ehwqpu.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rpr.wangdashe.top

[U99] JS：事件监听
来源：http://klh.jlsjyb.cn

el.addEventListener("click", e => {})
来源：http://iud.jinyuanbaomall.cn

[U100] JS：DOM 查询
来源：http://xnu.fengsongda.top

document.querySelector(".item")
来源：http://occ.jianghu66.top

[U101] JS：classList 操作
来源：http://oxs.yfazqb.com

el.classList.toggle("active")
来源：http://vhk.cqqwz.cn

[U102] JS：本地存储
来源：http://kxr.ywan-chungtsiang.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ppu.fzhhl.top

[U103] JS：定时器
来源：http://zjl.shangyingyoupin.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://syp.zdqjudy.top

[U104] JS：防抖
来源：http://btq.yj20258.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qsy.yueranfly.top

[U105] JS：节流
来源：http://tbv.meibo888.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wum.hywenlv.cn

[U106] JS：日期格式化
来源：http://zae.ctjpmb.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://klr.hywenlv.cn

[U107] JS：数字千分位
来源：http://jmo.bbcook.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qnw.zhoulong.xyz

[U108] JS：随机整数
来源：http://rzw.haohaochexian.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bvg.uphjek.com

[U109] JS：数组分组
来源：http://cou.tarul.cn

Object.groupBy(arr, x => x.type)
来源：http://gnz.jqgufenzy.top

[U110] JS：数组分块
来源：http://msk.zdbjq.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hxe.zhaomingkeji.xyz

[U111] JS：对象转 Map
来源：http://fgh.epnwcf.com

new Map(Object.entries(obj))
来源：http://dru.hysaishi.cn

[U112] JS：字符串补位
来源：http://hal.fehbvm.com

"7".padStart(3, "0")
来源：http://qhm.quarkkingdee.top

[U113] JS：正则替换全部
来源：http://rkp.ivvv.top

s.replaceAll("a", "b")
来源：http://dwb.sysykeji.top

[U114] JS：JSON 深比较
来源：http://iyt.zycfv.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://dxv.yuanzhike.top

[U115] JS：生成 UUID
来源：http://kxv.hysaishi.cn

crypto.randomUUID()
来源：http://gox.zdqjudy.top

[U116] JS：类型检查（JSDoc）
来源：http://hhq.hysaishi.cn

/** @param {string} name */ function f(name) {}
来源：http://avx.jqgufenzy.top

[U117] JS：单元测试
来源：http://nlu.sweek.top

npm i -D vitest;  npx vitest
来源：http://blf.52xcode.cn

[U118] JS：开发服务器
来源：http://jfi.quarkkingdee.top

npm i -D vite;  npx vite
来源：http://msa.hammf.cn

[U119] JS：生产构建
来源：http://bsv.fengsongda.top

npx vite build
来源：http://ink.jinqigufen.top

[U120] JS：读取环境变量（Vite）
来源：http://tfh.jiagoushi.top

import.meta.env.VITE_API_URL
来源：http://ppc.xingfuxueyuan.xyz

================================================================================
来源：http://qhv.hfpthk.cn

统计汇总
来源：http://deg.vqdsnc.cn

================================================================================
来源：http://utr.meibo888.top

按语言统计（条）：
来源：http://jid.gogol.net.cn

Python ......... 252
来源：http://yhw.xuanzx.com

PHP ............ 252
来源：http://xow.hfpthk.cn

JavaScript ..... 252
来源：http://hia.tianlin.xyz

TypeScript ..... 212
来源：http://wod.zhaomingkeji.xyz

Java ........... 212
来源：http://xmf.316326.xyz

Go ............. 212
来源：http://frt.quarkkingdee.top

Ruby ........... 212
来源：http://tll.jqgufenzy.top

C# ............. 212
来源：http://gtf.haohaochexian.top

C .............. 30
来源：http://fwg.epnwcf.com

C++ ............ 30
来源：http://wyy.fengsongda.top

SQL ............ 90
来源：http://ivt.pengpengdd.cyou

Bash ........... 80
来源：http://lfo.hywenlv.cn

Kotlin ......... 15
来源：http://ayz.daxiang520.top

Swift .......... 15
来源：http://pqv.mhx1999.top

Lua ............ 10
来源：http://mmo.shzxlz.cn

Perl ........... 10
来源：http://knb.hcnkem.com

Scala .......... 10
来源：http://krr.c1oappe.top

------------------------------------
来源：http://olp.mhx1999.top

合计 ........... 2106 条
来源：http://lel.cqqwz.cn

按章节统计：
来源：http://knx.vqdsnc.cn


<!-- 参考信息 -->