代发 wailian999

[T39] Lua：模式匹配
来源：http://tbz.vehdjk.com

string.find(s, "%d+")
来源：http://rzz.tanke756.top

[T40] Lua：元表
来源：http://fjx.feifeiyinyue.top

setmetatable({}, { __index = base })
来源：http://qbc.chenlongwang.top

[T41] Perl：Hello World
来源：http://krm.jiagoushi.top

print "Hello\n";
来源：http://ynk.hnxiangtu.top

[T42] Perl：变量类型
来源：http://rwv.nanxinkj.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://png.aizwys.cn

[T43] Perl：字符串插值
来源：http://hyy.meibo888.top

"值: $a"
来源：http://omc.pycfn.com

[T44] Perl：条件
来源：http://xig.c1oappe.top

if ($a > 0) { print "正"; }
来源：http://gnv.epnwcf.com

[T45] Perl：数组遍历
来源：http://lgh.aibaodan.cn

for my $x (@arr) { print $x; }
来源：http://xlb.yj20258.top

[T46] Perl：哈希操作
来源：http://cmk.jlsjyb.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xcw.yongpay.top

[T47] Perl：正则捕获
来源：http://wdy.hongshengwenyu.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://qej.xuetiantiany.cn

[T48] Perl：正则替换
来源：http://osj.cheryme.top

$s =~ s/old/new/g;
来源：http://pqb.yj20258888.top

[T49] Perl：函数
来源：http://vld.bjfxy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jox.meibo888.top

[T50] Perl：逐行读文件
来源：http://kln.iojbl.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://odo.ydjk.org.cn

while (my $line = <$fh>) { print $line; }
来源：http://aff.zycfv.cn

[T51] Scala：Hello World
来源：http://idr.yvedp.cn

println("Hello")
来源：http://isg.cashguo.top

[T52] Scala：变量
来源：http://eyu.fzhhl.top

val a = 1;  var b = 2
来源：http://ami.jlsjyb.cn

[T53] Scala：字符串插值
来源：http://pmn.ivvv.top

s"值: $b"
来源：http://twa.yvedp.cn

[T54] Scala：集合映射
来源：http://uzx.vehdjk.com

List(1, 2, 3).map(_ * 2)
来源：http://vrh.tianlin.xyz

[T55] Scala：集合过滤
来源：http://hjm.c1oappe.top

List(1, 2, 3).filter(_ > 1)
来源：http://hls.tianlin.xyz

[T56] Scala：样例类
来源：http://ftk.smart0.xyz

case class User(name: String, age: Int)
来源：http://fdf.gotoacloud.top

[T57] Scala：模式匹配
来源：http://ekf.zycfv.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://xfm.snrcjt.cn

[T58] Scala：函数定义
来源：http://wgx.yj202588.top

def add(a: Int, b: Int): Int = a + b
来源：http://vtv.xingfuxueyuan.xyz

[T59] Scala：循环
来源：http://pgi.316326.xyz

for (i <- 1 to 10) println(i)
来源：http://yvf.uphjek.com

[T60] Scala：折叠
来源：http://dmr.jinyuanbaomall.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cnm.tarul.cn

================================================================================
来源：http://pmt.52xcode.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zkf.jiagoushi.top

================================================================================
来源：http://nvc.chenzaomai.com

[U01] Py：创建虚拟环境
来源：http://vgm.9152youxi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://fnw.ehwqpu.com

[U02] Py：导出 / 安装依赖
来源：http://plx.jyoumei.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gfu.daxiang520.top

[U03] Py：加载 .env 配置
来源：http://oos.gotoacloud.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ofs.hcnkem.com

[U04] Py：变量调试打印
来源：http://kiz.fengsongda.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mje.yueranfly.top

[U05] Py：列表去重且保序
来源：http://obw.52xcode.cn

list(dict.fromkeys(arr))
来源：http://fza.havefunace.top

[U06] Py：合并两个字典
来源：http://vgf.cashguo.top

{**a, **b}
来源：http://dkg.chenzaomai.com

[U07] Py：反转字典键值
来源：http://jiy.yuanzhike.top

{v: k for k, v in d.items()}
来源：http://ltw.cucudq.cn

[U08] Py：展平二维列表
来源：http://cmw.xuanzx.com

[y for x in nested for y in x]
来源：http://yfu.tianlin.xyz

[U09] Py：字典取最大值的键
来源：http://nhk.tarul.cn

max(d, key=d.get)
来源：http://qkx.tianlin.xyz

[U10] Py：按值排序字典
来源：http://xdm.jqgufenzy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tfs.0kj1m.cn

[U11] Py：生成器表达式
来源：http://zpk.sysykeji.top

(x * 2 for x in arr)
来源：http://fjx.xziqi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ssu.yj202588.top

Counter(arr).most_common(3)
来源：http://jzv.snrcjt.cn

[U13] Py：固定长度队列
来源：http://lru.mhx1999.top

deque(maxlen=10)
来源：http://cpf.daxiang520.top

[U14] Py：分组收集到列表
来源：http://etk.fehbvm.com

defaultdict(list)
来源：http://kri.daria6918.cn

[U15] Py：高精度计时
来源：http://fcq.fehbvm.com

t = time.perf_counter()
来源：http://zzi.tian-w.cn

[U16] Py：命令行参数解析
来源：http://emw.zdbjq.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dbi.dianchejie.cn

[U17] Py：初始化日志
来源：http://wbl.xingfuxueyuan.xyz

logging.basicConfig(level=logging.INFO)
来源：http://lcl.wangshuangyany.cn

[U18] Py：预编译正则
来源：http://bss.bjfxy.top

pat = re.compile(r"\d+")
来源：http://ojw.quarkkingdee.top

[U19] Py：正则替换带回调
来源：http://iax.jqgufenzy.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ahm.cheryme.top

[U20] Py：缓存函数结果
来源：http://sxv.ppjwa.cn

@functools.lru_cache(maxsize=None)
来源：http://fvt.aizwys.cn

[U21] Py：自定义上下文管理器
来源：http://kne.xinyue.icu

@contextlib.contextmanager
来源：http://exp.sweek.top

[U22] Py：矩阵转置
来源：http://yvp.shanyushiyangkeji.top

list(zip(*m))
来源：http://cpv.jinqigfzy.top

[U23] Py：分块读取大文件
来源：http://has.yonumen.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gvp.jinghuilouyu.cn

[U24] Py：路径操作
来源：http://qma.shanyushiyangtech.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bgw.zdbjq.cn

[U25] Py：CSV 按字典读
来源：http://ijp.sjlbkw.cn

csv.DictReader(f)
来源：http://one.chenlongwang.top

[U26] Py：并发下载
来源：http://lxe.yongpay.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qdl.0kj1m.cn

[U27] Py：异步 HTTP
来源：http://dar.hnqzz.top

aiohttp.ClientSession() 配合 async with
来源：http://gqj.cucudq.cn

[U28] Py：类型别名
来源：http://bfo.fzhhl.top

UserId = int
来源：http://llq.hnqzz.top

[U29] Py：属性校验
来源：http://vzn.jiagoushi.top

@property 与 @x.setter 配合
来源：http://irm.yj20258888.top

[U30] Py：数据类
来源：http://ksd.xylfe.cn

@dataclass(slots=True)
来源：http://hmn.yuanzhike.top

[U31] Py：单测
来源：http://cul.pycfn.com

python -m pytest -q
来源：http://acv.yvedp.cn

[U32] Py：代码格式化
来源：http://zuh.svipenyu.cn

ruff format . && ruff check --fix .
来源：http://nnm.ivvv.top

[U33] Py：打包发布
来源：http://ggp.ehwqpu.com

python -m build  （依赖 pyproject.toml）
来源：http://boc.guowangkeji.top

[U34] Py：判断编码
来源：http://fis.cucudq.cn

chardet.detect(raw)
来源：http://wud.zdqjudy.top

[U35] Py：发送邮件
来源：http://tsg.xuetiantiany.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://efj.chenjidiqi.icu

[U36] Py：定时任务
来源：http://szq.316326.xyz

schedule.every(10).minutes.do(job)
来源：http://qzw.shuidangran.top

[U37] Py：读写 Excel
来源：http://osv.52xcode.cn

pandas.read_excel / DataFrame.to_excel
来源：http://nbj.yongpay.top

[U38] Py：获取脚本所在目录
来源：http://oyy.bjfxy.top

Path(__file__).resolve().parent
来源：http://zyc.sysykeji.top

[U39] Py：判断是否在交互环境
来源：http://xmv.jiagoushi.top

sys.stdout.isatty()
来源：http://xqf.kuanghao11.cn

[U40] Py：打印到标准错误
来源：http://boj.zhijiandao.cn

print("err", file=sys.stderr)
来源：http://yzz.tianlin.xyz

[U41] PHP：初始化 Composer 项目
来源：http://kpi.yuxming.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://hkt.9152youxi.cn

[U42] PHP：PSR-4 自动加载
来源：http://yqz.cqqwz.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vkm.ppjwa.cn

[U43] PHP：声明命名空间
来源：http://rqq.aibaodan.cn

namespace App\Http;
来源：http://fvh.vqdsnc.cn

[U44] PHP：开启严格类型
来源：http://hvy.vqdsnc.cn

declare(strict_types=1);
来源：http://bue.zdbjq.cn

[U45] PHP：类型声明与返回类型
来源：http://kps.shuidangran.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://cbu.zhixingplan.top

[U46] PHP：可空类型
来源：http://zja.316326.xyz

?string $name = null
来源：http://fxo.hesvh.cn

[U47] PHP：联合类型
来源：http://uas.zhongyouzk.top

int|string $id
来源：http://yag.yuxming.cn

[U48] PHP：纯枚举
来源：http://fzy.svipenyu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kaj.ppjwa.cn

[U49] PHP：只读属性
来源：http://nqq.yj20258.top

public readonly string $name
来源：http://xpb.zhaomingkeji.xyz

[U50] PHP：构造器属性提升
来源：http://haw.xingfuxueyuan.xyz

public function __construct(private int $id) {}
来源：http://lqw.hammf.cn

[U51] PHP：数组解构
来源：http://ehy.jinqigfzy.top

[$a, $b] = $arr;
来源：http://qcb.zhiwuduotai.top

[U52] PHP：箭头函数
来源：http://avx.shanyushiyangkeji.top

$double = fn($x) => $x * 2;
来源：http://clm.gzhubu.top

[U53] PHP：空合并运算符
来源：http://inz.aibaodan.cn

$v = $a ?? $b ?? "default";
来源：http://jqg.ywan-chungtsiang.top

[U54] PHP：空安全调用
来源：http://mis.dashuyun.cn

$obj?->method()
来源：http://jqc.cqqwz.cn

[U55] PHP：match 表达式
来源：http://lbm.cqqwz.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xcz.316326.xyz

[U56] PHP：命名参数
来源：http://cep.jinyuanbaomall.cn

f(a: 1, b: 2)
来源：http://jql.xuetiantiany.cn

[U57] PHP：字符串插值
来源：http://qph.wangdashe.top

"值: {$a}"
来源：http://cmz.hysaishi.cn

[U58] PHP：数组三件套
来源：http://naj.yanxiufei.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bvg.yonumen.top

[U59] PHP：自定义排序
来源：http://ada.hnxiangtu.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tsi.vehdjk.com

[U60] PHP：JSON 编解码
来源：http://csx.snrcjt.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vye.yj20258888.top

[U61] PHP：正则
来源：http://mak.ctjpmb.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vxt.yonumen.top

[U62] PHP：日期对象
来源：http://mlf.sufxvd.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://sta.chenzaomai.com

[U63] PHP：文件读写
来源：http://bzi.jianghu66.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tar.hongshengwenyu.top

[U64] PHP：目录遍历
来源：http://kvr.wangshuangyany.cn

glob("dir/*.php");  scandir("dir");
来源：http://kyv.guowangkeji.top

[U65] PHP：会话
来源：http://vax.shangyingyoupin.top

session_start();  $_SESSION["uid"] = 1;
来源：http://rak.ybcxt.top

[U66] PHP：设置 Cookie
来源：http://zop.chenzaomai.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qbs.svipenyu.cn

[U67] PHP：处理文件上传
来源：http://ukf.fzhhl.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gbb.fktsv.cn

[U68] PHP：PDO 连接
来源：http://qrw.shangyingyoupin.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kxx.jinqigfzy.top

[U69] PHP：PDO 预处理
来源：http://guy.cdnleiting.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mqg.gzhubu.top

[U70] PHP：PDO 事务
来源：http://ekx.yuanzhike.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qgu.haohaochexian.top

[U71] PHP：抛出异常
来源：http://bmd.aizwys.cn

throw new RuntimeException("失败", 500);
来源：http://ozx.zhixingplan.top

[U72] PHP：写错误日志
来源：http://acp.shzxlz.cn

error_log("失败: " . $e->getMessage());
来源：http://nmo.fanxiaobao.xyz

[U73] PHP：读取 ini 配置
来源：http://khz.ywan-chungtsiang.top

parse_ini_file("config.ini", true)
来源：http://oky.cdnleiting.top

[U74] PHP：读取环境变量
来源：http://tuw.zhijiandao.cn

getenv("APP_ENV") ?: "production"
来源：http://nrx.cucudq.cn

[U75] PHP：依赖注入
来源：http://tjx.quarkkingdee.top

composer require psr/container
来源：http://icu.sweek.top

[U76] PHP：简单路由
来源：http://teh.sjlbkw.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ekd.hfpthk.cn

[U77] PHP：模板渲染
来源：http://jbz.ehwqpu.com

composer require twig/twig
来源：http://vtw.316326.xyz

[U78] PHP：单元测试
来源：http://ipp.jyoumei.cn

composer require --dev phpunit/phpunit
来源：http://bri.cucudq.cn

[U79] PHP：静态分析
来源：http://hlr.zhaomingkeji.xyz

composer require --dev phpstan/phpstan
来源：http://hib.hnqzz.top

[U80] PHP：代码规范修复
来源：http://ezd.birdmap.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://wnf.bbcook.cn

[U81] JS：初始化项目
来源：http://jcq.gzhubu.top

npm init -y;  npm i express
来源：http://kxl.jlsjyb.cn

[U82] JS：package.json 脚本
来源：http://zgi.zhongyouzk.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nvw.tian-w.cn

[U83] JS：ES Module 导入导出
来源：http://gww.chenlongwang.top

export const a = 1;  import { a } from "./m.js";
来源：http://fkf.shangyingyoupin.top

[U84] JS：CommonJS 写法
来源：http://gjj.wangdashe.top

module.exports = { a };  const { a } = require("./m");
来源：http://zun.xuetiantiany.cn

[U85] JS：可选链
来源：http://igv.shanyushiyangtech.top

a?.b?.c
来源：http://auq.xuanzx.com

[U86] JS：空值合并
来源：http://lok.shangyingyoupin.top

a ?? b
来源：http://azu.tanke756.top

[U87] JS：解构默认值
来源：http://gzk.bbcook.cn

const { a = 1, b = 2 } = obj;
来源：http://knq.sweek.top

[U88] JS：对象展开合并
来源：http://vik.jinghuilouyu.cn

{ ...a, ...b }
来源：http://bco.yangfankeji.com

[U89] JS：数组去重
来源：http://dlg.gogol.net.cn

[...new Set(arr)]
来源：http://rpz.daria6918.cn

[U90] JS：数字数组排序
来源：http://pob.snrcjt.cn

[...arr].sort((a, b) => a - b)
来源：http://duj.xuanzx.com

[U91] JS：对象键值遍历
来源：http://ono.tianlin.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://eji.ywan-chungtsiang.top

[U92] JS：深拷贝
来源：http://pmm.vqdsnc.cn

structuredClone(obj)
来源：http://kkg.cdnleiting.top

[U93] JS：模板字符串
来源：http://szb.zhiwuduotai.top

`共 ${n} 条`
来源：http://aki.smart0.xyz

[U94] JS：箭头函数
来源：http://olz.xinyue.icu

const double = x => x * 2;
来源：http://cyo.fktsv.cn

[U95] JS：Promise 包装
来源：http://krs.jinqigfzy.top

new Promise((resolve, reject) => {})
来源：http://yfn.tanke756.top

[U96] JS：async/await 与异常
来源：http://ako.hnqzz.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://onu.nanxuanxn.top

[U97] JS：并发请求
来源：http://wlz.shzxlz.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://xbr.yueranfly.top

[U98] JS：fetch 带 JSON
来源：http://oqv.zhixingplan.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pjy.jinghuilouyu.cn

[U99] JS：事件监听
来源：http://zkp.iojbl.cn

el.addEventListener("click", e => {})
来源：http://zzw.kuanghao11.cn

[U100] JS：DOM 查询
来源：http://kgl.feifeiyinyue.top

document.querySelector(".item")
来源：http://vfp.fengsongda.top

[U101] JS：classList 操作
来源：http://ruj.kuanghao11.cn

el.classList.toggle("active")
来源：http://byn.vehdjk.com

[U102] JS：本地存储
来源：http://wor.hnqzz.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ucq.tianlin.xyz

[U103] JS：定时器
来源：http://ntq.gzhubu.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wub.ppjwa.cn

[U104] JS：防抖
来源：http://dkd.cashguo.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ufi.ivvv.top

[U105] JS：节流
来源：http://wdx.vqdsnc.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wxw.yj20258.top

[U106] JS：日期格式化
来源：http://vnd.pengpengdd.cyou

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://joo.zhoulong.xyz

[U107] JS：数字千分位
来源：http://ozz.jinghuilouyu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ljy.dianchejie.cn

[U108] JS：随机整数
来源：http://wkb.yongpay.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://eqq.yuanzhike.top

[U109] JS：数组分组
来源：http://mow.snrcjt.cn

Object.groupBy(arr, x => x.type)
来源：http://cfw.xziqi.cn

[U110] JS：数组分块
来源：http://zrr.gotoacloud.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rhq.kuanghao11.cn

[U111] JS：对象转 Map
来源：http://ttg.jlsjyb.cn

new Map(Object.entries(obj))
来源：http://teh.hongshengwenyu.top

[U112] JS：字符串补位
来源：http://hnb.hcnkem.com

"7".padStart(3, "0")
来源：http://csw.snrcjt.cn

[U113] JS：正则替换全部
来源：http://fjx.zhengqikj.top

s.replaceAll("a", "b")
来源：http://krz.ctjpmb.com

[U114] JS：JSON 深比较
来源：http://qru.feifeiyinyue.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://fqw.cashguo.top

[U115] JS：生成 UUID
来源：http://nwc.hywenlv.cn

crypto.randomUUID()
来源：http://azr.jinqigfzy.top

[U116] JS：类型检查（JSDoc）
来源：http://tao.daria6918.cn

/** @param {string} name */ function f(name) {}
来源：http://xsk.cucudq.cn

[U117] JS：单元测试
来源：http://zpv.sxryk.cn

npm i -D vitest;  npx vitest
来源：http://sqx.jinqigfzy.top

[U118] JS：开发服务器
来源：http://wro.c1oappe.top

npm i -D vite;  npx vite
来源：http://dbp.vqdsnc.cn

[U119] JS：生产构建
来源：http://fax.fanxiaobao.xyz

npx vite build
来源：http://try.feifeiyinyue.top

[U120] JS：读取环境变量（Vite）
来源：http://sck.dashuyun.cn

import.meta.env.VITE_API_URL
来源：http://zmg.jinghuilouyu.cn

================================================================================
来源：http://zus.vqdsnc.cn

统计汇总
来源：http://dtq.yj202588.top

================================================================================
来源：http://dew.yuxming.cn

按语言统计（条）：
来源：http://mqb.tarul.cn

Python ......... 252
来源：http://kfk.hnxiangtu.top

PHP ............ 252
来源：http://vrs.jlsjyb.cn

JavaScript ..... 252
来源：http://trj.zhixingplan.top

TypeScript ..... 212
来源：http://spi.daxiang520.top

Java ........... 212
来源：http://soi.daxiang520.top

Go ............. 212
来源：http://osh.meibo888.top

Ruby ........... 212
来源：http://jbq.cashguo.top

C# ............. 212
来源：http://hli.uphjek.com


<!-- 参考信息 -->