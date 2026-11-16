代发 wailian999

[T39] Lua：模式匹配
来源：http://gfd.guannengcc.top

string.find(s, "%d+")
来源：http://ddm.iojbl.cn

[T40] Lua：元表
来源：http://mor.feifeiyinyue.top

setmetatable({}, { __index = base })
来源：http://rru.zhoulong.xyz

[T41] Perl：Hello World
来源：http://vfc.cqqwz.cn

print "Hello\n";
来源：http://vyn.fanxiaobao.xyz

[T42] Perl：变量类型
来源：http://qsf.xylfe.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rht.vqdsnc.cn

[T43] Perl：字符串插值
来源：http://ohd.sjlbkw.cn

"值: $a"
来源：http://ylp.jlsjyb.cn

[T44] Perl：条件
来源：http://cfs.9152youxi.cn

if ($a > 0) { print "正"; }
来源：http://vch.fanxiaobao.xyz

[T45] Perl：数组遍历
来源：http://zdh.hongshengwenyu.top

for my $x (@arr) { print $x; }
来源：http://jmd.zhiwuduotai.top

[T46] Perl：哈希操作
来源：http://zqj.chenjidiqi.icu

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gsw.yuanzhike.top

[T47] Perl：正则捕获
来源：http://vkx.daria6918.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://qtc.daria6918.cn

[T48] Perl：正则替换
来源：http://bwv.daxiang520.top

$s =~ s/old/new/g;
来源：http://sou.zhiwuduotai.top

[T49] Perl：函数
来源：http://mue.fehbvm.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jph.guannengcc.top

[T50] Perl：逐行读文件
来源：http://dpq.epnwcf.com

open my $fh, "<", "a.txt" or die $!;
来源：http://bus.yuanzhike.top

while (my $line = <$fh>) { print $line; }
来源：http://fsg.zhengqikj.top

[T51] Scala：Hello World
来源：http://dmb.epnwcf.com

println("Hello")
来源：http://xex.quarkkingdee.top

[T52] Scala：变量
来源：http://yxo.ivvv.top

val a = 1;  var b = 2
来源：http://oos.yfazqb.com

[T53] Scala：字符串插值
来源：http://vny.snrcjt.cn

s"值: $b"
来源：http://nqy.dashuyun.cn

[T54] Scala：集合映射
来源：http://pvr.xuanzx.com

List(1, 2, 3).map(_ * 2)
来源：http://hep.9152youxi.cn

[T55] Scala：集合过滤
来源：http://xlz.9152youxi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ira.ydjk.org.cn

[T56] Scala：样例类
来源：http://xcf.zhongyouzk.top

case class User(name: String, age: Int)
来源：http://tfs.jqgfzy.top

[T57] Scala：模式匹配
来源：http://ykw.316326.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://ube.jiagoushi.top

[T58] Scala：函数定义
来源：http://udv.gotoacloud.top

def add(a: Int, b: Int): Int = a + b
来源：http://juz.gzhubu.top

[T59] Scala：循环
来源：http://rtb.yj20258.top

for (i <- 1 to 10) println(i)
来源：http://wdb.iojbl.cn

[T60] Scala：折叠
来源：http://yyb.chenjidiqi.icu

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://sjw.yfazqb.com

================================================================================
来源：http://hmt.hnxiangtu.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ycz.xylfe.cn

================================================================================
来源：http://srk.hysaishi.cn

[U01] Py：创建虚拟环境
来源：http://moo.feifeiyinyue.top

python -m venv .venv && source .venv/bin/activate
来源：http://tyy.daxiang520.top

[U02] Py：导出 / 安装依赖
来源：http://bvz.cdnleiting.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://sbf.aizwys.cn

[U03] Py：加载 .env 配置
来源：http://ilt.ehwqpu.com

from dotenv import load_dotenv; load_dotenv()
来源：http://hgs.daxiang520.top

[U04] Py：变量调试打印
来源：http://udv.wangdashe.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nwt.pengpengdd.cyou

[U05] Py：列表去重且保序
来源：http://foq.tian-w.cn

list(dict.fromkeys(arr))
来源：http://vqa.jiagoushi.top

[U06] Py：合并两个字典
来源：http://xuo.xuetiantiany.cn

{**a, **b}
来源：http://tsl.andypj.xyz

[U07] Py：反转字典键值
来源：http://vok.bbcook.cn

{v: k for k, v in d.items()}
来源：http://tdz.jlsjyb.cn

[U08] Py：展平二维列表
来源：http://fpi.chenjidiqi.icu

[y for x in nested for y in x]
来源：http://pax.xinyue.icu

[U09] Py：字典取最大值的键
来源：http://fql.andypj.xyz

max(d, key=d.get)
来源：http://fky.hnxiangtu.top

[U10] Py：按值排序字典
来源：http://khh.yj202588.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rzh.gotoacloud.top

[U11] Py：生成器表达式
来源：http://mlo.c1oappe.top

(x * 2 for x in arr)
来源：http://jji.wangshuangyany.cn

[U12] Py：取出现最多的 3 个元素
来源：http://jtv.ctjpmb.com

Counter(arr).most_common(3)
来源：http://hvi.yangfankeji.com

[U13] Py：固定长度队列
来源：http://wkw.daria6918.cn

deque(maxlen=10)
来源：http://cas.52xcode.cn

[U14] Py：分组收集到列表
来源：http://vxh.yongpay.top

defaultdict(list)
来源：http://mqb.andypj.xyz

[U15] Py：高精度计时
来源：http://koi.ehwqpu.com

t = time.perf_counter()
来源：http://aye.zycfv.cn

[U16] Py：命令行参数解析
来源：http://wgd.xuanzx.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mep.yj202588.top

[U17] Py：初始化日志
来源：http://sdl.shanyushiyangkeji.top

logging.basicConfig(level=logging.INFO)
来源：http://maa.zhoulong.xyz

[U18] Py：预编译正则
来源：http://rhf.yfazqb.com

pat = re.compile(r"\d+")
来源：http://gnt.cheryme.top

[U19] Py：正则替换带回调
来源：http://dzq.tanke756.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mvu.hammf.cn

[U20] Py：缓存函数结果
来源：http://zig.kuanghao11.cn

@functools.lru_cache(maxsize=None)
来源：http://qez.haohaochexian.top

[U21] Py：自定义上下文管理器
来源：http://ovh.jqgufenzy.top

@contextlib.contextmanager
来源：http://taw.aibaodan.cn

[U22] Py：矩阵转置
来源：http://tik.gogol.net.cn

list(zip(*m))
来源：http://otg.nwbrower.top

[U23] Py：分块读取大文件
来源：http://ndy.chenzaomai.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://kmr.aizwys.cn

[U24] Py：路径操作
来源：http://yiq.yuanzhike.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jom.jqgufenzy.top

[U25] Py：CSV 按字典读
来源：http://pga.nwbrower.top

csv.DictReader(f)
来源：http://jlj.kuanghao11.cn

[U26] Py：并发下载
来源：http://xsk.aizwys.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vqp.zhaomingkeji.xyz

[U27] Py：异步 HTTP
来源：http://qql.kuanghao11.cn

aiohttp.ClientSession() 配合 async with
来源：http://las.zhijiandao.cn

[U28] Py：类型别名
来源：http://eqm.ppjwa.cn

UserId = int
来源：http://rtv.hnxiangtu.top

[U29] Py：属性校验
来源：http://zsy.yangfankeji.com

@property 与 @x.setter 配合
来源：http://olp.svipenyu.cn

[U30] Py：数据类
来源：http://iut.zycfv.cn

@dataclass(slots=True)
来源：http://jsl.mhx1999.top

[U31] Py：单测
来源：http://vdr.yueranfly.top

python -m pytest -q
来源：http://szj.snrcjt.cn

[U32] Py：代码格式化
来源：http://gng.zhijiandao.cn

ruff format . && ruff check --fix .
来源：http://ppm.tianlin.xyz

[U33] Py：打包发布
来源：http://lgh.smart0.xyz

python -m build  （依赖 pyproject.toml）
来源：http://hut.chenlongwang.top

[U34] Py：判断编码
来源：http://meb.cdnleiting.top

chardet.detect(raw)
来源：http://lkm.uphjek.com

[U35] Py：发送邮件
来源：http://jfh.hfpthk.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cyd.zdqjudy.top

[U36] Py：定时任务
来源：http://dpy.gaohongyu789.top

schedule.every(10).minutes.do(job)
来源：http://sch.aibaodan.cn

[U37] Py：读写 Excel
来源：http://pta.316326.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://gcv.gotoacloud.top

[U38] Py：获取脚本所在目录
来源：http://zap.ydjk.org.cn

Path(__file__).resolve().parent
来源：http://eux.havefunace.top

[U39] Py：判断是否在交互环境
来源：http://fmt.jinghuilouyu.cn

sys.stdout.isatty()
来源：http://lay.yuanzhike.top

[U40] Py：打印到标准错误
来源：http://rpd.yj202588.top

print("err", file=sys.stderr)
来源：http://uwj.sysykeji.top

[U41] PHP：初始化 Composer 项目
来源：http://yas.yueranfly.top

composer init;  composer require guzzlehttp/guzzle
来源：http://tqf.cdnleiting.top

[U42] PHP：PSR-4 自动加载
来源：http://duy.yonumen.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dej.zhengqikj.top

[U43] PHP：声明命名空间
来源：http://rgg.svipenyu.cn

namespace App\Http;
来源：http://zqc.tarul.cn

[U44] PHP：开启严格类型
来源：http://czd.zhiwuduotai.top

declare(strict_types=1);
来源：http://mhe.hammf.cn

[U45] PHP：类型声明与返回类型
来源：http://ytz.xuanzx.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://lqe.chenjidiqi.icu

[U46] PHP：可空类型
来源：http://nyt.tanke756.top

?string $name = null
来源：http://pds.andypj.xyz

[U47] PHP：联合类型
来源：http://zyz.wangdashe.top

int|string $id
来源：http://tlc.guannengcc.top

[U48] PHP：纯枚举
来源：http://rmz.gogol.net.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mso.zhiwuduotai.top

[U49] PHP：只读属性
来源：http://jmj.yanxiufei.cn

public readonly string $name
来源：http://ogc.ppjwa.cn

[U50] PHP：构造器属性提升
来源：http://lhy.yueranfly.top

public function __construct(private int $id) {}
来源：http://tnw.bbcook.cn

[U51] PHP：数组解构
来源：http://tew.fehbvm.com

[$a, $b] = $arr;
来源：http://uxj.hammf.cn

[U52] PHP：箭头函数
来源：http://khg.chenlongwang.top

$double = fn($x) => $x * 2;
来源：http://cla.haohaochexian.top

[U53] PHP：空合并运算符
来源：http://cce.uphjek.com

$v = $a ?? $b ?? "default";
来源：http://bba.yueranfly.top

[U54] PHP：空安全调用
来源：http://cfy.yuxming.cn

$obj?->method()
来源：http://ite.cucudq.cn

[U55] PHP：match 表达式
来源：http://kxh.gogol.net.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://pki.shangyingyoupin.top

[U56] PHP：命名参数
来源：http://zzw.zhengqikj.top

f(a: 1, b: 2)
来源：http://apm.bjfxy.top

[U57] PHP：字符串插值
来源：http://qam.birdmap.top

"值: {$a}"
来源：http://aeg.jqgufenzy.top

[U58] PHP：数组三件套
来源：http://zif.yanxiufei.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cfg.redwolf501.top

[U59] PHP：自定义排序
来源：http://agg.xziqi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://awq.gzhubu.top

[U60] PHP：JSON 编解码
来源：http://foi.nwbrower.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ync.dashuyun.cn

[U61] PHP：正则
来源：http://eov.ehwqpu.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://evz.chenzaomai.com

[U62] PHP：日期对象
来源：http://zal.yonumen.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://uey.wangshuangyany.cn

[U63] PHP：文件读写
来源：http://adc.zhixingplan.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://sdc.shanyushiyangtech.top

[U64] PHP：目录遍历
来源：http://eds.feifeiyinyue.top

glob("dir/*.php");  scandir("dir");
来源：http://ziq.nanxinkj.top

[U65] PHP：会话
来源：http://emo.jiagoushi.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ety.epnwcf.com

[U66] PHP：设置 Cookie
来源：http://lxh.yfazqb.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://lls.hammf.cn

[U67] PHP：处理文件上传
来源：http://zhx.birdmap.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://oeo.havefunace.top

[U68] PHP：PDO 连接
来源：http://jhj.iojbl.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://uah.tianlin.xyz

[U69] PHP：PDO 预处理
来源：http://rye.hcnkem.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zwt.nanxinkj.top

[U70] PHP：PDO 事务
来源：http://bam.wangshuangyany.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://grc.ywan-chungtsiang.top

[U71] PHP：抛出异常
来源：http://vqd.cucudq.cn

throw new RuntimeException("失败", 500);
来源：http://pxw.aizwys.cn

[U72] PHP：写错误日志
来源：http://lod.yj202588.top

error_log("失败: " . $e->getMessage());
来源：http://rmb.ctjpmb.com

[U73] PHP：读取 ini 配置
来源：http://ife.zhaomingkeji.xyz

parse_ini_file("config.ini", true)
来源：http://msm.yonumen.top

[U74] PHP：读取环境变量
来源：http://gsz.hnqzz.top

getenv("APP_ENV") ?: "production"
来源：http://vgp.jinghuilouyu.cn

[U75] PHP：依赖注入
来源：http://dzm.hongshengwenyu.top

composer require psr/container
来源：http://aie.0kj1m.cn

[U76] PHP：简单路由
来源：http://nkt.zhijiandao.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://sut.xinyue.icu

[U77] PHP：模板渲染
来源：http://owb.hysaishi.cn

composer require twig/twig
来源：http://hse.nanxinkj.top

[U78] PHP：单元测试
来源：http://fhk.hongshengwenyu.top

composer require --dev phpunit/phpunit
来源：http://clb.yj202588.top

[U79] PHP：静态分析
来源：http://mjs.0kj1m.cn

composer require --dev phpstan/phpstan
来源：http://pre.smart0.xyz

[U80] PHP：代码规范修复
来源：http://axl.birdmap.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ukk.svipenyu.cn

[U81] JS：初始化项目
来源：http://dkj.xuetiantiany.cn

npm init -y;  npm i express
来源：http://pck.jinyuanbaomall.cn

[U82] JS：package.json 脚本
来源：http://pmk.snrcjt.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://edi.gzhubu.top

[U83] JS：ES Module 导入导出
来源：http://jun.316326.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://pjf.hfpthk.cn

[U84] JS：CommonJS 写法
来源：http://njp.yj20258888.top

module.exports = { a };  const { a } = require("./m");
来源：http://via.nanxuanxn.top

[U85] JS：可选链
来源：http://xff.cashguo.top

a?.b?.c
来源：http://cld.birdmap.top

[U86] JS：空值合并
来源：http://fgr.cashguo.top

a ?? b
来源：http://vom.dashuyun.cn

[U87] JS：解构默认值
来源：http://jrn.gotoacloud.top

const { a = 1, b = 2 } = obj;
来源：http://mwg.xuanzx.com

[U88] JS：对象展开合并
来源：http://jza.daria6918.cn

{ ...a, ...b }
来源：http://goj.chenjidiqi.icu

[U89] JS：数组去重
来源：http://qtu.yangfankeji.com

[...new Set(arr)]
来源：http://hso.jqgfzy.top

[U90] JS：数字数组排序
来源：http://avt.316326.xyz

[...arr].sort((a, b) => a - b)
来源：http://you.zdqjudy.top

[U91] JS：对象键值遍历
来源：http://zvk.yj202588.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tfm.fengsongda.top

[U92] JS：深拷贝
来源：http://xtp.cdnleiting.top

structuredClone(obj)
来源：http://nml.mhx1999.top

[U93] JS：模板字符串
来源：http://mhm.nanxuanxn.top

`共 ${n} 条`
来源：http://zzl.yfazqb.com

[U94] JS：箭头函数
来源：http://jym.aibaodan.cn

const double = x => x * 2;
来源：http://fmo.jinqigufen.top

[U95] JS：Promise 包装
来源：http://ngs.shanyushiyangkeji.top

new Promise((resolve, reject) => {})
来源：http://hkf.kuanghao11.cn

[U96] JS：async/await 与异常
来源：http://bpi.yj20258.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gwo.shanyushiyangtech.top

[U97] JS：并发请求
来源：http://nqp.vqdsnc.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://inx.jinqigfzy.top

[U98] JS：fetch 带 JSON
来源：http://spy.cucudq.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jnc.xingfuxueyuan.xyz

[U99] JS：事件监听
来源：http://atr.zhixingplan.top

el.addEventListener("click", e => {})
来源：http://wnb.cqqwz.cn

[U100] JS：DOM 查询
来源：http://qzf.cucudq.cn

document.querySelector(".item")
来源：http://zff.yanxiufei.cn

[U101] JS：classList 操作
来源：http://muv.sxryk.cn

el.classList.toggle("active")
来源：http://xlv.ydzc1.top

[U102] JS：本地存储
来源：http://cfp.zhaomingkeji.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://eye.52xcode.cn

[U103] JS：定时器
来源：http://urr.zhijiandao.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://dvy.nwbrower.top

[U104] JS：防抖
来源：http://pch.ydzc1.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cgd.sjlbkw.cn

[U105] JS：节流
来源：http://jtf.316326.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://oea.xylfe.cn

[U106] JS：日期格式化
来源：http://rwm.ywan-chungtsiang.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nax.jinghuilouyu.cn

[U107] JS：数字千分位
来源：http://zab.xuetiantiany.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wbz.kuanghao11.cn

[U108] JS：随机整数
来源：http://zov.sjlbkw.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://yrk.jinghuilouyu.cn

[U109] JS：数组分组
来源：http://kyg.yongpay.top

Object.groupBy(arr, x => x.type)
来源：http://uoh.fehbvm.com

[U110] JS：数组分块
来源：http://mqt.316326.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://klq.jiagoushi.top

[U111] JS：对象转 Map
来源：http://zml.ivvv.top

new Map(Object.entries(obj))
来源：http://uqi.c1oappe.top

[U112] JS：字符串补位
来源：http://mxu.hammf.cn

"7".padStart(3, "0")
来源：http://cbf.hfpthk.cn

[U113] JS：正则替换全部
来源：http://nsr.pengpengdd.cyou

s.replaceAll("a", "b")
来源：http://rgo.hammf.cn

[U114] JS：JSON 深比较
来源：http://tqk.hfpthk.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://mfb.chenlongwang.top

[U115] JS：生成 UUID
来源：http://fcv.zhaomingkeji.xyz

crypto.randomUUID()
来源：http://dcg.chenzaomai.com

[U116] JS：类型检查（JSDoc）
来源：http://cpm.shanyushiyangkeji.top

/** @param {string} name */ function f(name) {}
来源：http://pfw.redwolf501.top

[U117] JS：单元测试
来源：http://ulb.daxiang520.top

npm i -D vitest;  npx vitest
来源：http://ksr.feifeiyinyue.top

[U118] JS：开发服务器
来源：http://tjv.zhiwuduotai.top

npm i -D vite;  npx vite
来源：http://phf.nwbrower.top

[U119] JS：生产构建
来源：http://lub.zhiwuduotai.top

npx vite build
来源：http://sah.xinyue.icu

[U120] JS：读取环境变量（Vite）
来源：http://arf.zdqjudy.top

import.meta.env.VITE_API_URL
来源：http://gmn.tianlin.xyz

================================================================================
来源：http://gji.zhaomingkeji.xyz

统计汇总
来源：http://xea.jinghuilouyu.cn

================================================================================
来源：http://dsq.cucudq.cn

按语言统计（条）：
来源：http://ipc.ywan-chungtsiang.top

Python ......... 252
来源：http://xam.yonumen.top

PHP ............ 252
来源：http://wsq.xingfuxueyuan.xyz

JavaScript ..... 252
来源：http://tvp.yangfankeji.com

TypeScript ..... 212
来源：http://smy.ywan-chungtsiang.top

Java ........... 212
来源：http://cvr.jinyuanbaomall.cn

Go ............. 212
来源：http://ujf.wangshuangyany.cn

Ruby ........... 212
来源：http://poe.yanxiufei.cn

C# ............. 212
来源：http://zrd.bbcook.cn


<!-- 参考信息 -->