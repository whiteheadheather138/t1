代发 wailian999

[T39] Lua：模式匹配
来源：http://wir.svipenyu.cn

string.find(s, "%d+")
来源：http://nhr.haohaochexian.top

[T40] Lua：元表
来源：http://bjm.chenjidiqi.icu

setmetatable({}, { __index = base })
来源：http://ntx.xuanzx.com

[T41] Perl：Hello World
来源：http://zlf.xinyue.icu

print "Hello\n";
来源：http://ngx.bjfxy.top

[T42] Perl：变量类型
来源：http://kla.wangshuangyany.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pas.tianlin.xyz

[T43] Perl：字符串插值
来源：http://oir.tarul.cn

"值: $a"
来源：http://ojd.redwolf501.top

[T44] Perl：条件
来源：http://lyq.hysaishi.cn

if ($a > 0) { print "正"; }
来源：http://tkk.birdmap.top

[T45] Perl：数组遍历
来源：http://vbw.ivvv.top

for my $x (@arr) { print $x; }
来源：http://hgd.gzhubu.top

[T46] Perl：哈希操作
来源：http://ejd.andypj.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jwz.zhongyouzk.top

[T47] Perl：正则捕获
来源：http://thr.dianchejie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://fqw.yonumen.top

[T48] Perl：正则替换
来源：http://jws.jianghu66.top

$s =~ s/old/new/g;
来源：http://uux.zhoulong.xyz

[T49] Perl：函数
来源：http://hbt.xuanzx.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ues.fzhhl.top

[T50] Perl：逐行读文件
来源：http://iuv.shzxlz.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://vda.zhijiandao.cn

while (my $line = <$fh>) { print $line; }
来源：http://xgq.gotoacloud.top

[T51] Scala：Hello World
来源：http://mac.cheryme.top

println("Hello")
来源：http://mji.hnxiangtu.top

[T52] Scala：变量
来源：http://cwq.aibaodan.cn

val a = 1;  var b = 2
来源：http://ywl.zhengqikj.top

[T53] Scala：字符串插值
来源：http://edz.jqgfzy.top

s"值: $b"
来源：http://hsf.jianghu66.top

[T54] Scala：集合映射
来源：http://qnx.shanyushiyangtech.top

List(1, 2, 3).map(_ * 2)
来源：http://nfy.xingfuxueyuan.xyz

[T55] Scala：集合过滤
来源：http://vnq.nanxinkj.top

List(1, 2, 3).filter(_ > 1)
来源：http://mzl.xziqi.cn

[T56] Scala：样例类
来源：http://rar.shuidangran.top

case class User(name: String, age: Int)
来源：http://ipo.yj20258888.top

[T57] Scala：模式匹配
来源：http://ngo.nanxinkj.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://jcs.mhx1999.top

[T58] Scala：函数定义
来源：http://wjq.0kj1m.cn

def add(a: Int, b: Int): Int = a + b
来源：http://hom.jinghuilouyu.cn

[T59] Scala：循环
来源：http://ang.tanke756.top

for (i <- 1 to 10) println(i)
来源：http://ofv.jyoumei.cn

[T60] Scala：折叠
来源：http://bmg.zhixingplan.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://oqf.ppjwa.cn

================================================================================
来源：http://sin.jqgufenzy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ubq.snrcjt.cn

================================================================================
来源：http://ngo.cashguo.top

[U01] Py：创建虚拟环境
来源：http://vnx.sjlbkw.cn

python -m venv .venv && source .venv/bin/activate
来源：http://dug.mhx1999.top

[U02] Py：导出 / 安装依赖
来源：http://rtj.yj202588.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nvn.yangfankeji.com

[U03] Py：加载 .env 配置
来源：http://ael.ehwqpu.com

from dotenv import load_dotenv; load_dotenv()
来源：http://cwd.fengsongda.top

[U04] Py：变量调试打印
来源：http://efh.fengsongda.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rzo.ydjk.org.cn

[U05] Py：列表去重且保序
来源：http://wxu.yonumen.top

list(dict.fromkeys(arr))
来源：http://vio.jqgufenzy.top

[U06] Py：合并两个字典
来源：http://own.tian-w.cn

{**a, **b}
来源：http://jnk.zhijiandao.cn

[U07] Py：反转字典键值
来源：http://ybm.tianlin.xyz

{v: k for k, v in d.items()}
来源：http://prm.yangfankeji.com

[U08] Py：展平二维列表
来源：http://tso.redwolf501.top

[y for x in nested for y in x]
来源：http://vef.shzxlz.cn

[U09] Py：字典取最大值的键
来源：http://zgh.xuanzx.com

max(d, key=d.get)
来源：http://tbd.fanxiaobao.xyz

[U10] Py：按值排序字典
来源：http://fwv.hysaishi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://afb.fzhhl.top

[U11] Py：生成器表达式
来源：http://cts.fanxiaobao.xyz

(x * 2 for x in arr)
来源：http://xfx.xuetiantiany.cn

[U12] Py：取出现最多的 3 个元素
来源：http://rvk.fehbvm.com

Counter(arr).most_common(3)
来源：http://xds.gotoacloud.top

[U13] Py：固定长度队列
来源：http://kci.wangdashe.top

deque(maxlen=10)
来源：http://oxq.jinghuilouyu.cn

[U14] Py：分组收集到列表
来源：http://uqc.epnwcf.com

defaultdict(list)
来源：http://fqz.xuanzx.com

[U15] Py：高精度计时
来源：http://pqi.aibaodan.cn

t = time.perf_counter()
来源：http://cia.xuetiantiany.cn

[U16] Py：命令行参数解析
来源：http://hum.zhoulong.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://owd.ybcxt.top

[U17] Py：初始化日志
来源：http://fke.nanxinkj.top

logging.basicConfig(level=logging.INFO)
来源：http://ibo.tarul.cn

[U18] Py：预编译正则
来源：http://gyt.iojbl.cn

pat = re.compile(r"\d+")
来源：http://hne.hcnkem.com

[U19] Py：正则替换带回调
来源：http://rlb.epnwcf.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sjk.ywan-chungtsiang.top

[U20] Py：缓存函数结果
来源：http://orq.tanke756.top

@functools.lru_cache(maxsize=None)
来源：http://ytl.zhongyouzk.top

[U21] Py：自定义上下文管理器
来源：http://eyn.zdqjudy.top

@contextlib.contextmanager
来源：http://ngg.ybcxt.top

[U22] Py：矩阵转置
来源：http://wku.chenjidiqi.icu

list(zip(*m))
来源：http://ecu.zhijiandao.cn

[U23] Py：分块读取大文件
来源：http://els.fengsongda.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://izg.xuanzx.com

[U24] Py：路径操作
来源：http://nwq.ydzc1.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jtu.zhixingplan.top

[U25] Py：CSV 按字典读
来源：http://vgd.shzxlz.cn

csv.DictReader(f)
来源：http://hyg.iojbl.cn

[U26] Py：并发下载
来源：http://tci.fehbvm.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://quv.birdmap.top

[U27] Py：异步 HTTP
来源：http://kep.cashguo.top

aiohttp.ClientSession() 配合 async with
来源：http://xip.ctjpmb.com

[U28] Py：类型别名
来源：http://btw.daxiang520.top

UserId = int
来源：http://ztv.cashguo.top

[U29] Py：属性校验
来源：http://vzx.xingfuxueyuan.xyz

@property 与 @x.setter 配合
来源：http://ylo.ppjwa.cn

[U30] Py：数据类
来源：http://kkh.smart0.xyz

@dataclass(slots=True)
来源：http://iql.ybcxt.top

[U31] Py：单测
来源：http://imh.xuanzx.com

python -m pytest -q
来源：http://ylu.zhongyouzk.top

[U32] Py：代码格式化
来源：http://huy.gotoacloud.top

ruff format . && ruff check --fix .
来源：http://cnm.zycfv.cn

[U33] Py：打包发布
来源：http://paw.hcnkem.com

python -m build  （依赖 pyproject.toml）
来源：http://pgt.gzhubu.top

[U34] Py：判断编码
来源：http://fjy.hesvh.cn

chardet.detect(raw)
来源：http://lxr.zhoulong.xyz

[U35] Py：发送邮件
来源：http://gjo.zdbjq.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tep.xuanzx.com

[U36] Py：定时任务
来源：http://hyf.wangdashe.top

schedule.every(10).minutes.do(job)
来源：http://gmp.tianlin.xyz

[U37] Py：读写 Excel
来源：http://fon.nanxinkj.top

pandas.read_excel / DataFrame.to_excel
来源：http://pby.jlsjyb.cn

[U38] Py：获取脚本所在目录
来源：http://zyd.zhongyouzk.top

Path(__file__).resolve().parent
来源：http://ers.zhijiandao.cn

[U39] Py：判断是否在交互环境
来源：http://zch.guowangkeji.top

sys.stdout.isatty()
来源：http://tww.9152youxi.cn

[U40] Py：打印到标准错误
来源：http://fkp.yj20258.top

print("err", file=sys.stderr)
来源：http://emw.tanke756.top

[U41] PHP：初始化 Composer 项目
来源：http://njq.hammf.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://zjh.nwbrower.top

[U42] PHP：PSR-4 自动加载
来源：http://qdb.sjlbkw.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zwm.guowangkeji.top

[U43] PHP：声明命名空间
来源：http://vtt.tianlin.xyz

namespace App\Http;
来源：http://hgt.ctjpmb.com

[U44] PHP：开启严格类型
来源：http://xwm.daria6918.cn

declare(strict_types=1);
来源：http://unf.jqgufenzy.top

[U45] PHP：类型声明与返回类型
来源：http://ixl.xuanzx.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://jwc.zhoulong.xyz

[U46] PHP：可空类型
来源：http://aoi.xuanzx.com

?string $name = null
来源：http://ubc.nwbrower.top

[U47] PHP：联合类型
来源：http://sie.feifeiyinyue.top

int|string $id
来源：http://jas.wangdashe.top

[U48] PHP：纯枚举
来源：http://jrd.aibaodan.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tye.shanyushiyangtech.top

[U49] PHP：只读属性
来源：http://iwr.cdnleiting.top

public readonly string $name
来源：http://oev.xuanzx.com

[U50] PHP：构造器属性提升
来源：http://tjt.jinqigufen.top

public function __construct(private int $id) {}
来源：http://ixo.tanke756.top

[U51] PHP：数组解构
来源：http://qen.gaohongyu789.top

[$a, $b] = $arr;
来源：http://hhz.ehwqpu.com

[U52] PHP：箭头函数
来源：http://ipf.hammf.cn

$double = fn($x) => $x * 2;
来源：http://rwl.chenlongwang.top

[U53] PHP：空合并运算符
来源：http://gdl.sxryk.cn

$v = $a ?? $b ?? "default";
来源：http://fvq.tian-w.cn

[U54] PHP：空安全调用
来源：http://wlm.xziqi.cn

$obj?->method()
来源：http://asi.fktsv.cn

[U55] PHP：match 表达式
来源：http://elb.shangyingyoupin.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://sfe.sjlbkw.cn

[U56] PHP：命名参数
来源：http://gqr.jinghuilouyu.cn

f(a: 1, b: 2)
来源：http://bxz.tian-w.cn

[U57] PHP：字符串插值
来源：http://byb.hammf.cn

"值: {$a}"
来源：http://zmb.chenzaomai.com

[U58] PHP：数组三件套
来源：http://kft.chenlongwang.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://npf.fengsongda.top

[U59] PHP：自定义排序
来源：http://ywr.sxryk.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bau.xingfuxueyuan.xyz

[U60] PHP：JSON 编解码
来源：http://avj.tianlin.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://psg.chenlongwang.top

[U61] PHP：正则
来源：http://koj.tanke756.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ihc.zhijiandao.cn

[U62] PHP：日期对象
来源：http://hwe.xuanzx.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://oeo.ydzc1.top

[U63] PHP：文件读写
来源：http://rki.epnwcf.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kfr.zhaomingkeji.xyz

[U64] PHP：目录遍历
来源：http://dhb.redwolf501.top

glob("dir/*.php");  scandir("dir");
来源：http://gtw.bjfxy.top

[U65] PHP：会话
来源：http://aba.redwolf501.top

session_start();  $_SESSION["uid"] = 1;
来源：http://yje.tianlin.xyz

[U66] PHP：设置 Cookie
来源：http://jgs.havefunace.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ubf.yj20258888.top

[U67] PHP：处理文件上传
来源：http://emb.zdqjudy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gje.yvedp.cn

[U68] PHP：PDO 连接
来源：http://vvd.dianchejie.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lil.yuxming.cn

[U69] PHP：PDO 预处理
来源：http://etv.nanxinkj.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fxi.daria6918.cn

[U70] PHP：PDO 事务
来源：http://yyq.xingfuxueyuan.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zms.sxryk.cn

[U71] PHP：抛出异常
来源：http://kub.aizwys.cn

throw new RuntimeException("失败", 500);
来源：http://hbt.yj20258.top

[U72] PHP：写错误日志
来源：http://wmg.yonumen.top

error_log("失败: " . $e->getMessage());
来源：http://yrv.jinqigufen.top

[U73] PHP：读取 ini 配置
来源：http://diw.jinyuanbaomall.cn

parse_ini_file("config.ini", true)
来源：http://lsi.zdqjudy.top

[U74] PHP：读取环境变量
来源：http://vkt.svipenyu.cn

getenv("APP_ENV") ?: "production"
来源：http://lpn.zhixingplan.top

[U75] PHP：依赖注入
来源：http://fwj.xingfuxueyuan.xyz

composer require psr/container
来源：http://dbe.jiagoushi.top

[U76] PHP：简单路由
来源：http://vor.yfazqb.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://sid.quarkkingdee.top

[U77] PHP：模板渲染
来源：http://qaa.yvedp.cn

composer require twig/twig
来源：http://nxi.yonumen.top

[U78] PHP：单元测试
来源：http://nuf.jianghu66.top

composer require --dev phpunit/phpunit
来源：http://vzj.ydzc1.top

[U79] PHP：静态分析
来源：http://mbu.cqqwz.cn

composer require --dev phpstan/phpstan
来源：http://fmd.ywan-chungtsiang.top

[U80] PHP：代码规范修复
来源：http://txr.yonumen.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://qvo.hnxiangtu.top

[U81] JS：初始化项目
来源：http://pzp.ydzc1.top

npm init -y;  npm i express
来源：http://bor.yongpay.top

[U82] JS：package.json 脚本
来源：http://hcb.uphjek.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pan.zhaomingkeji.xyz

[U83] JS：ES Module 导入导出
来源：http://vio.ivvv.top

export const a = 1;  import { a } from "./m.js";
来源：http://sac.hcnkem.com

[U84] JS：CommonJS 写法
来源：http://ebl.yueranfly.top

module.exports = { a };  const { a } = require("./m");
来源：http://zkn.guannengcc.top

[U85] JS：可选链
来源：http://faz.sufxvd.cn

a?.b?.c
来源：http://fmf.jinqigfzy.top

[U86] JS：空值合并
来源：http://hro.hywenlv.cn

a ?? b
来源：http://lvo.dianchejie.cn

[U87] JS：解构默认值
来源：http://vmk.jinqigufen.top

const { a = 1, b = 2 } = obj;
来源：http://nfs.chenzaomai.com

[U88] JS：对象展开合并
来源：http://bzi.meibo888.top

{ ...a, ...b }
来源：http://fzs.yj20258888.top

[U89] JS：数组去重
来源：http://anq.xuetiantiany.cn

[...new Set(arr)]
来源：http://lsb.guowangkeji.top

[U90] JS：数字数组排序
来源：http://tsn.guannengcc.top

[...arr].sort((a, b) => a - b)
来源：http://zpw.zhoulong.xyz

[U91] JS：对象键值遍历
来源：http://kgy.dianchejie.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vye.yueranfly.top

[U92] JS：深拷贝
来源：http://wuh.zdbjq.cn

structuredClone(obj)
来源：http://lvo.zdqjudy.top

[U93] JS：模板字符串
来源：http://cqd.ehwqpu.com

`共 ${n} 条`
来源：http://dbb.jinghuilouyu.cn

[U94] JS：箭头函数
来源：http://agc.andypj.xyz

const double = x => x * 2;
来源：http://cjr.pengpengdd.cyou

[U95] JS：Promise 包装
来源：http://spa.ydjk.org.cn

new Promise((resolve, reject) => {})
来源：http://bvl.yvedp.cn

[U96] JS：async/await 与异常
来源：http://fme.shzxlz.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://enh.aizwys.cn

[U97] JS：并发请求
来源：http://flg.chenzaomai.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://ddk.shangyingyoupin.top

[U98] JS：fetch 带 JSON
来源：http://ztr.hesvh.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://uxd.vehdjk.com

[U99] JS：事件监听
来源：http://dfp.iojbl.cn

el.addEventListener("click", e => {})
来源：http://vch.xziqi.cn

[U100] JS：DOM 查询
来源：http://exk.hfpthk.cn

document.querySelector(".item")
来源：http://hif.yuanzhike.top

[U101] JS：classList 操作
来源：http://kkg.fengsongda.top

el.classList.toggle("active")
来源：http://abk.sxryk.cn

[U102] JS：本地存储
来源：http://bdt.zhongyouzk.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://gfz.birdmap.top

[U103] JS：定时器
来源：http://nhp.wangshuangyany.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xqk.redwolf501.top

[U104] JS：防抖
来源：http://pvm.zhengqikj.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dkf.guowangkeji.top

[U105] JS：节流
来源：http://fvz.chenzaomai.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wzr.guowangkeji.top

[U106] JS：日期格式化
来源：http://dqp.nanxuanxn.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://two.yanxiufei.cn

[U107] JS：数字千分位
来源：http://fjl.nanxinkj.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jbs.zhiwuduotai.top

[U108] JS：随机整数
来源：http://ocf.nwbrower.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ypz.zhiwuduotai.top

[U109] JS：数组分组
来源：http://dfj.yj202588.top

Object.groupBy(arr, x => x.type)
来源：http://qkq.gzhubu.top

[U110] JS：数组分块
来源：http://mmq.hongshengwenyu.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gtg.9152youxi.cn

[U111] JS：对象转 Map
来源：http://mld.jianghu66.top

new Map(Object.entries(obj))
来源：http://ocj.cdnleiting.top

[U112] JS：字符串补位
来源：http://pfx.vehdjk.com

"7".padStart(3, "0")
来源：http://yph.ehwqpu.com

[U113] JS：正则替换全部
来源：http://vyu.iojbl.cn

s.replaceAll("a", "b")
来源：http://dbt.tarul.cn

[U114] JS：JSON 深比较
来源：http://awy.gotoacloud.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://pmr.gogol.net.cn

[U115] JS：生成 UUID
来源：http://sor.chenzaomai.com

crypto.randomUUID()
来源：http://wjf.fktsv.cn

[U116] JS：类型检查（JSDoc）
来源：http://rbk.ybcxt.top

/** @param {string} name */ function f(name) {}
来源：http://cbn.zycfv.cn

[U117] JS：单元测试
来源：http://seu.meibo888.top

npm i -D vitest;  npx vitest
来源：http://ujj.havefunace.top

[U118] JS：开发服务器
来源：http://jva.smart0.xyz

npm i -D vite;  npx vite
来源：http://imx.hcnkem.com

[U119] JS：生产构建
来源：http://gze.hnqzz.top

npx vite build
来源：http://cuj.vehdjk.com

[U120] JS：读取环境变量（Vite）
来源：http://muk.shanyushiyangtech.top

import.meta.env.VITE_API_URL
来源：http://dws.jlsjyb.cn

================================================================================
来源：http://gbu.gaohongyu789.top

统计汇总
来源：http://vmc.chenzaomai.com

================================================================================
来源：http://sxi.jinqigfzy.top

按语言统计（条）：
来源：http://skk.tarul.cn

Python ......... 252
来源：http://yuw.yongpay.top

PHP ............ 252
来源：http://tuf.hongshengwenyu.top

JavaScript ..... 252
来源：http://img.wangshuangyany.cn

TypeScript ..... 212
来源：http://ccg.snrcjt.cn

Java ........... 212
来源：http://trj.hnqzz.top

Go ............. 212
来源：http://ebj.quarkkingdee.top

Ruby ........... 212
来源：http://mao.vehdjk.com

C# ............. 212
来源：http://jii.daria6918.cn


<!-- 参考信息 -->