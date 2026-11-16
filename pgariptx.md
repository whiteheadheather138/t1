代发 wailian999

[T37] Lua：字符串拼接
来源：http://efw.zhongyouzk.top

"a" .. "b"
来源：http://oob.nanxinkj.top

[T38] Lua：条件
来源：http://wsm.jyoumei.cn

if x > 0 then print("正") end
来源：http://etg.sysykeji.top

[T39] Lua：模式匹配
来源：http://usi.hysaishi.cn

string.find(s, "%d+")
来源：http://lfc.fanxiaobao.xyz

[T40] Lua：元表
来源：http://zno.jqgufenzy.top

setmetatable({}, { __index = base })
来源：http://xvg.pycfn.com

[T41] Perl：Hello World
来源：http://emp.ctjpmb.com

print "Hello\n";
来源：http://mgx.birdmap.top

[T42] Perl：变量类型
来源：http://upz.hnxiangtu.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pei.316326.xyz

[T43] Perl：字符串插值
来源：http://tgc.ivvv.top

"值: $a"
来源：http://pka.yuxming.cn

[T44] Perl：条件
来源：http://ykj.ydjk.org.cn

if ($a > 0) { print "正"; }
来源：http://nlz.xinyue.icu

[T45] Perl：数组遍历
来源：http://mxb.sweek.top

for my $x (@arr) { print $x; }
来源：http://xcg.birdmap.top

[T46] Perl：哈希操作
来源：http://tsh.zhengqikj.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hqu.hammf.cn

[T47] Perl：正则捕获
来源：http://kdq.sysykeji.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://nnw.xylfe.cn

[T48] Perl：正则替换
来源：http://usy.hammf.cn

$s =~ s/old/new/g;
来源：http://vdz.hesvh.cn

[T49] Perl：函数
来源：http://jwg.nwbrower.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mtj.ctjpmb.com

[T50] Perl：逐行读文件
来源：http://mas.xuanzx.com

open my $fh, "<", "a.txt" or die $!;
来源：http://uxa.xuetiantiany.cn

while (my $line = <$fh>) { print $line; }
来源：http://cih.yj20258.top

[T51] Scala：Hello World
来源：http://ppo.zhengqikj.top

println("Hello")
来源：http://lhs.daria6918.cn

[T52] Scala：变量
来源：http://mjk.yongpay.top

val a = 1;  var b = 2
来源：http://qhp.9152youxi.cn

[T53] Scala：字符串插值
来源：http://kqk.uphjek.com

s"值: $b"
来源：http://ist.jianghu66.top

[T54] Scala：集合映射
来源：http://ewy.nwbrower.top

List(1, 2, 3).map(_ * 2)
来源：http://gmg.zycfv.cn

[T55] Scala：集合过滤
来源：http://zlg.tianlin.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://nua.wangdashe.top

[T56] Scala：样例类
来源：http://hjz.meibo888.top

case class User(name: String, age: Int)
来源：http://adx.0kj1m.cn

[T57] Scala：模式匹配
来源：http://ukd.tianlin.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://odk.yonumen.top

[T58] Scala：函数定义
来源：http://cop.jinghuilouyu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://jvh.0kj1m.cn

[T59] Scala：循环
来源：http://dvu.xuetiantiany.cn

for (i <- 1 to 10) println(i)
来源：http://ndf.wangshuangyany.cn

[T60] Scala：折叠
来源：http://xyi.hongshengwenyu.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gzd.yangfankeji.com

================================================================================
来源：http://axa.hesvh.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rfa.zhixingplan.top

================================================================================
来源：http://whk.ivvv.top

[U01] Py：创建虚拟环境
来源：http://hqb.yj20258888.top

python -m venv .venv && source .venv/bin/activate
来源：http://pdw.jianghu66.top

[U02] Py：导出 / 安装依赖
来源：http://bzq.sufxvd.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vdo.guannengcc.top

[U03] Py：加载 .env 配置
来源：http://wnf.hywenlv.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://whq.yongpay.top

[U04] Py：变量调试打印
来源：http://sup.gogol.net.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://cvz.pycfn.com

[U05] Py：列表去重且保序
来源：http://omr.shanyushiyangkeji.top

list(dict.fromkeys(arr))
来源：http://twj.fehbvm.com

[U06] Py：合并两个字典
来源：http://kcf.yuxming.cn

{**a, **b}
来源：http://dhv.nanxuanxn.top

[U07] Py：反转字典键值
来源：http://pwi.xingfuxueyuan.xyz

{v: k for k, v in d.items()}
来源：http://wkv.andypj.xyz

[U08] Py：展平二维列表
来源：http://hdc.jinqigufen.top

[y for x in nested for y in x]
来源：http://mxk.zhongyouzk.top

[U09] Py：字典取最大值的键
来源：http://ccn.ppjwa.cn

max(d, key=d.get)
来源：http://nqb.chenzaomai.com

[U10] Py：按值排序字典
来源：http://rjx.316326.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nay.cashguo.top

[U11] Py：生成器表达式
来源：http://sfb.wangshuangyany.cn

(x * 2 for x in arr)
来源：http://wif.nanxuanxn.top

[U12] Py：取出现最多的 3 个元素
来源：http://bwr.yvedp.cn

Counter(arr).most_common(3)
来源：http://vvl.hammf.cn

[U13] Py：固定长度队列
来源：http://tul.yj202588.top

deque(maxlen=10)
来源：http://lnz.cucudq.cn

[U14] Py：分组收集到列表
来源：http://hzf.gaohongyu789.top

defaultdict(list)
来源：http://klf.ctjpmb.com

[U15] Py：高精度计时
来源：http://aax.xuanzx.com

t = time.perf_counter()
来源：http://soi.aizwys.cn

[U16] Py：命令行参数解析
来源：http://qch.nwbrower.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lgj.gogol.net.cn

[U17] Py：初始化日志
来源：http://hfy.316326.xyz

logging.basicConfig(level=logging.INFO)
来源：http://lbn.jlsjyb.cn

[U18] Py：预编译正则
来源：http://xnu.yj20258.top

pat = re.compile(r"\d+")
来源：http://tdj.zhijiandao.cn

[U19] Py：正则替换带回调
来源：http://jgp.yj20258888.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ipb.hnxiangtu.top

[U20] Py：缓存函数结果
来源：http://oeg.shzxlz.cn

@functools.lru_cache(maxsize=None)
来源：http://ege.haohaochexian.top

[U21] Py：自定义上下文管理器
来源：http://rxz.haohaochexian.top

@contextlib.contextmanager
来源：http://rlp.zhaomingkeji.xyz

[U22] Py：矩阵转置
来源：http://owv.sufxvd.cn

list(zip(*m))
来源：http://dhx.nanxinkj.top

[U23] Py：分块读取大文件
来源：http://xsz.pycfn.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://has.zhixingplan.top

[U24] Py：路径操作
来源：http://fym.shanyushiyangkeji.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fpt.zhaomingkeji.xyz

[U25] Py：CSV 按字典读
来源：http://fhc.wangdashe.top

csv.DictReader(f)
来源：http://saf.sysykeji.top

[U26] Py：并发下载
来源：http://jks.cheryme.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pmk.sysykeji.top

[U27] Py：异步 HTTP
来源：http://qba.gzhubu.top

aiohttp.ClientSession() 配合 async with
来源：http://gge.c1oappe.top

[U28] Py：类型别名
来源：http://pjb.yangfankeji.com

UserId = int
来源：http://dia.svipenyu.cn

[U29] Py：属性校验
来源：http://iii.havefunace.top

@property 与 @x.setter 配合
来源：http://gzj.mhx1999.top

[U30] Py：数据类
来源：http://byp.guowangkeji.top

@dataclass(slots=True)
来源：http://ocf.0kj1m.cn

[U31] Py：单测
来源：http://hql.nwbrower.top

python -m pytest -q
来源：http://mgy.gaohongyu789.top

[U32] Py：代码格式化
来源：http://hsp.xuetiantiany.cn

ruff format . && ruff check --fix .
来源：http://ghc.yj20258888.top

[U33] Py：打包发布
来源：http://psc.yj20258.top

python -m build  （依赖 pyproject.toml）
来源：http://fts.feifeiyinyue.top

[U34] Py：判断编码
来源：http://xtc.ywan-chungtsiang.top

chardet.detect(raw)
来源：http://kwy.hfpthk.cn

[U35] Py：发送邮件
来源：http://xap.dianchejie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://idj.ybcxt.top

[U36] Py：定时任务
来源：http://sts.ctjpmb.com

schedule.every(10).minutes.do(job)
来源：http://adn.yj202588.top

[U37] Py：读写 Excel
来源：http://tkv.sufxvd.cn

pandas.read_excel / DataFrame.to_excel
来源：http://cxx.xinyue.icu

[U38] Py：获取脚本所在目录
来源：http://itt.jinghuilouyu.cn

Path(__file__).resolve().parent
来源：http://sll.meibo888.top

[U39] Py：判断是否在交互环境
来源：http://mge.c1oappe.top

sys.stdout.isatty()
来源：http://hde.gzhubu.top

[U40] Py：打印到标准错误
来源：http://qbf.yj202588.top

print("err", file=sys.stderr)
来源：http://ffv.kuanghao11.cn

[U41] PHP：初始化 Composer 项目
来源：http://pwz.yuanzhike.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ekh.cqqwz.cn

[U42] PHP：PSR-4 自动加载
来源：http://drx.sxryk.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xvd.quarkkingdee.top

[U43] PHP：声明命名空间
来源：http://uor.sysykeji.top

namespace App\Http;
来源：http://pfl.daria6918.cn

[U44] PHP：开启严格类型
来源：http://auz.wangdashe.top

declare(strict_types=1);
来源：http://pzv.dashuyun.cn

[U45] PHP：类型声明与返回类型
来源：http://yes.316326.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://rga.fktsv.cn

[U46] PHP：可空类型
来源：http://eys.bjfxy.top

?string $name = null
来源：http://jxn.tian-w.cn

[U47] PHP：联合类型
来源：http://jgu.sufxvd.cn

int|string $id
来源：http://zkk.wangdashe.top

[U48] PHP：纯枚举
来源：http://eyp.dianchejie.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://yjk.birdmap.top

[U49] PHP：只读属性
来源：http://xas.andypj.xyz

public readonly string $name
来源：http://mjt.xingfuxueyuan.xyz

[U50] PHP：构造器属性提升
来源：http://dzu.uphjek.com

public function __construct(private int $id) {}
来源：http://bor.yj20258.top

[U51] PHP：数组解构
来源：http://psn.52xcode.cn

[$a, $b] = $arr;
来源：http://cfe.9152youxi.cn

[U52] PHP：箭头函数
来源：http://xei.tarul.cn

$double = fn($x) => $x * 2;
来源：http://mhx.jinqigufen.top

[U53] PHP：空合并运算符
来源：http://dcc.epnwcf.com

$v = $a ?? $b ?? "default";
来源：http://vqj.tianlin.xyz

[U54] PHP：空安全调用
来源：http://eit.sxryk.cn

$obj?->method()
来源：http://gdy.zhijiandao.cn

[U55] PHP：match 表达式
来源：http://sap.hysaishi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mpg.xuanzx.com

[U56] PHP：命名参数
来源：http://yti.fehbvm.com

f(a: 1, b: 2)
来源：http://esu.gogol.net.cn

[U57] PHP：字符串插值
来源：http://rmw.svipenyu.cn

"值: {$a}"
来源：http://tof.yanxiufei.cn

[U58] PHP：数组三件套
来源：http://twk.cdnleiting.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bjt.xziqi.cn

[U59] PHP：自定义排序
来源：http://kll.jyoumei.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cqg.zhongyouzk.top

[U60] PHP：JSON 编解码
来源：http://awi.zdbjq.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://yyo.dianchejie.cn

[U61] PHP：正则
来源：http://xgi.redwolf501.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hkx.nanxinkj.top

[U62] PHP：日期对象
来源：http://hcs.fehbvm.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://tnj.ppjwa.cn

[U63] PHP：文件读写
来源：http://ydt.haohaochexian.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://skk.cashguo.top

[U64] PHP：目录遍历
来源：http://fos.zycfv.cn

glob("dir/*.php");  scandir("dir");
来源：http://yja.guannengcc.top

[U65] PHP：会话
来源：http://oav.cheryme.top

session_start();  $_SESSION["uid"] = 1;
来源：http://mkg.hnxiangtu.top

[U66] PHP：设置 Cookie
来源：http://rwa.jqgufenzy.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://eus.shanyushiyangkeji.top

[U67] PHP：处理文件上传
来源：http://xfs.jinyuanbaomall.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pwe.redwolf501.top

[U68] PHP：PDO 连接
来源：http://kkp.0kj1m.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://adz.meibo888.top

[U69] PHP：PDO 预处理
来源：http://wki.gotoacloud.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fdq.xylfe.cn

[U70] PHP：PDO 事务
来源：http://oqm.yuanzhike.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://yjw.fehbvm.com

[U71] PHP：抛出异常
来源：http://odt.wangshuangyany.cn

throw new RuntimeException("失败", 500);
来源：http://imr.sxryk.cn

[U72] PHP：写错误日志
来源：http://dgf.haohaochexian.top

error_log("失败: " . $e->getMessage());
来源：http://ymq.ivvv.top

[U73] PHP：读取 ini 配置
来源：http://lsn.zhengqikj.top

parse_ini_file("config.ini", true)
来源：http://zql.chenzaomai.com

[U74] PHP：读取环境变量
来源：http://udk.meibo888.top

getenv("APP_ENV") ?: "production"
来源：http://vzv.ivvv.top

[U75] PHP：依赖注入
来源：http://nwo.andypj.xyz

composer require psr/container
来源：http://yam.fanxiaobao.xyz

[U76] PHP：简单路由
来源：http://qen.fehbvm.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lph.jinqigufen.top

[U77] PHP：模板渲染
来源：http://gdx.hnqzz.top

composer require twig/twig
来源：http://dcl.hysaishi.cn

[U78] PHP：单元测试
来源：http://ssc.jyoumei.cn

composer require --dev phpunit/phpunit
来源：http://qbu.zhengqikj.top

[U79] PHP：静态分析
来源：http://yea.quarkkingdee.top

composer require --dev phpstan/phpstan
来源：http://wql.andypj.xyz

[U80] PHP：代码规范修复
来源：http://vgd.bjfxy.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://xhq.hcnkem.com

[U81] JS：初始化项目
来源：http://rgm.yueranfly.top

npm init -y;  npm i express
来源：http://tkg.birdmap.top

[U82] JS：package.json 脚本
来源：http://crx.daria6918.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lym.nwbrower.top

[U83] JS：ES Module 导入导出
来源：http://wmd.cdnleiting.top

export const a = 1;  import { a } from "./m.js";
来源：http://bes.yonumen.top

[U84] JS：CommonJS 写法
来源：http://rya.hnqzz.top

module.exports = { a };  const { a } = require("./m");
来源：http://kki.xuetiantiany.cn

[U85] JS：可选链
来源：http://lhe.havefunace.top

a?.b?.c
来源：http://rrr.aizwys.cn

[U86] JS：空值合并
来源：http://num.ywan-chungtsiang.top

a ?? b
来源：http://npd.shanyushiyangtech.top

[U87] JS：解构默认值
来源：http://kbh.sxryk.cn

const { a = 1, b = 2 } = obj;
来源：http://nlu.haohaochexian.top

[U88] JS：对象展开合并
来源：http://rwj.dashuyun.cn

{ ...a, ...b }
来源：http://fuu.yj202588.top

[U89] JS：数组去重
来源：http://zdp.cdnleiting.top

[...new Set(arr)]
来源：http://rpj.pengpengdd.cyou

[U90] JS：数字数组排序
来源：http://hby.ydzc1.top

[...arr].sort((a, b) => a - b)
来源：http://fqp.ppjwa.cn

[U91] JS：对象键值遍历
来源：http://ipo.zhaomingkeji.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rha.xuanzx.com

[U92] JS：深拷贝
来源：http://jff.sjlbkw.cn

structuredClone(obj)
来源：http://qgk.yangfankeji.com

[U93] JS：模板字符串
来源：http://udn.meibo888.top

`共 ${n} 条`
来源：http://luu.tanke756.top

[U94] JS：箭头函数
来源：http://oyc.wangshuangyany.cn

const double = x => x * 2;
来源：http://llo.yueranfly.top

[U95] JS：Promise 包装
来源：http://fxe.xinyue.icu

new Promise((resolve, reject) => {})
来源：http://rno.gaohongyu789.top

[U96] JS：async/await 与异常
来源：http://rxi.zycfv.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fhv.tanke756.top

[U97] JS：并发请求
来源：http://nvf.sufxvd.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://rhb.dashuyun.cn

[U98] JS：fetch 带 JSON
来源：http://fjn.iojbl.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bax.hongshengwenyu.top

[U99] JS：事件监听
来源：http://zfq.jinghuilouyu.cn

el.addEventListener("click", e => {})
来源：http://gjt.52xcode.cn

[U100] JS：DOM 查询
来源：http://mow.wangdashe.top

document.querySelector(".item")
来源：http://ipp.yfazqb.com

[U101] JS：classList 操作
来源：http://nlr.hfpthk.cn

el.classList.toggle("active")
来源：http://rgl.shangyingyoupin.top

[U102] JS：本地存储
来源：http://uvk.dashuyun.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://mvt.daxiang520.top

[U103] JS：定时器
来源：http://nin.dashuyun.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jqz.aizwys.cn

[U104] JS：防抖
来源：http://twp.jiagoushi.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tlf.jqgufenzy.top

[U105] JS：节流
来源：http://ubi.dianchejie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ilt.ehwqpu.com

[U106] JS：日期格式化
来源：http://acr.zdqjudy.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yhi.daria6918.cn

[U107] JS：数字千分位
来源：http://vgt.wangdashe.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wcv.birdmap.top

[U108] JS：随机整数
来源：http://ycm.jiagoushi.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://end.xinyue.icu

[U109] JS：数组分组
来源：http://hmb.sjlbkw.cn

Object.groupBy(arr, x => x.type)
来源：http://rky.redwolf501.top

[U110] JS：数组分块
来源：http://wbp.sweek.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://crb.cucudq.cn

[U111] JS：对象转 Map
来源：http://ncg.tanke756.top

new Map(Object.entries(obj))
来源：http://fcl.andypj.xyz

[U112] JS：字符串补位
来源：http://vom.gzhubu.top

"7".padStart(3, "0")
来源：http://cpp.haohaochexian.top

[U113] JS：正则替换全部
来源：http://hcf.shzxlz.cn

s.replaceAll("a", "b")
来源：http://adu.dashuyun.cn

[U114] JS：JSON 深比较
来源：http://sdx.hongshengwenyu.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://qbp.fengsongda.top

[U115] JS：生成 UUID
来源：http://ueg.sweek.top

crypto.randomUUID()
来源：http://jkw.zhaomingkeji.xyz

[U116] JS：类型检查（JSDoc）
来源：http://vdo.xuetiantiany.cn

/** @param {string} name */ function f(name) {}
来源：http://crb.zycfv.cn

[U117] JS：单元测试
来源：http://mne.dashuyun.cn

npm i -D vitest;  npx vitest
来源：http://htj.hammf.cn

[U118] JS：开发服务器
来源：http://rmx.bbcook.cn

npm i -D vite;  npx vite
来源：http://eov.9152youxi.cn

[U119] JS：生产构建
来源：http://odi.ydzc1.top

npx vite build
来源：http://eam.jianghu66.top

[U120] JS：读取环境变量（Vite）
来源：http://yko.hfpthk.cn

import.meta.env.VITE_API_URL
来源：http://usq.yj20258888.top

================================================================================
来源：http://dxt.xuanzx.com

统计汇总
来源：http://fla.zycfv.cn

================================================================================
来源：http://jib.chenjidiqi.icu

按语言统计（条）：
来源：http://fur.hysaishi.cn

Python ......... 252
来源：http://spl.gogol.net.cn

PHP ............ 252
来源：http://zws.nwbrower.top

JavaScript ..... 252
来源：http://upp.gaohongyu789.top

TypeScript ..... 212
来源：http://tyd.cucudq.cn


<!-- 参考信息 -->