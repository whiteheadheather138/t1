代发 wailian999

[T37] Lua：字符串拼接
来源：http://dkh.feifeiyinyue.top

"a" .. "b"
来源：http://cyt.vqdsnc.cn

[T38] Lua：条件
来源：http://ifu.yj20258888.top

if x > 0 then print("正") end
来源：http://bak.sufxvd.cn

[T39] Lua：模式匹配
来源：http://jos.shzxlz.cn

string.find(s, "%d+")
来源：http://rvr.cashguo.top

[T40] Lua：元表
来源：http://ozg.hongshengwenyu.top

setmetatable({}, { __index = base })
来源：http://kad.yj20258.top

[T41] Perl：Hello World
来源：http://ulb.jlsjyb.cn

print "Hello\n";
来源：http://bnv.cashguo.top

[T42] Perl：变量类型
来源：http://xii.jlsjyb.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jiy.nwbrower.top

[T43] Perl：字符串插值
来源：http://kld.shanyushiyangkeji.top

"值: $a"
来源：http://zbe.jyoumei.cn

[T44] Perl：条件
来源：http://skg.quarkkingdee.top

if ($a > 0) { print "正"; }
来源：http://bwu.jinqigfzy.top

[T45] Perl：数组遍历
来源：http://tha.ivvv.top

for my $x (@arr) { print $x; }
来源：http://cun.hnqzz.top

[T46] Perl：哈希操作
来源：http://xfd.hysaishi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lma.xziqi.cn

[T47] Perl：正则捕获
来源：http://bjs.hongshengwenyu.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://igy.andypj.xyz

[T48] Perl：正则替换
来源：http://vmv.sufxvd.cn

$s =~ s/old/new/g;
来源：http://ihk.chenzaomai.com

[T49] Perl：函数
来源：http://txg.hfpthk.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pdj.316326.xyz

[T50] Perl：逐行读文件
来源：http://juu.sysykeji.top

open my $fh, "<", "a.txt" or die $!;
来源：http://zcm.aibaodan.cn

while (my $line = <$fh>) { print $line; }
来源：http://etq.feifeiyinyue.top

[T51] Scala：Hello World
来源：http://gbj.wangshuangyany.cn

println("Hello")
来源：http://jyu.nanxinkj.top

[T52] Scala：变量
来源：http://mcv.cqqwz.cn

val a = 1;  var b = 2
来源：http://ykq.ctjpmb.com

[T53] Scala：字符串插值
来源：http://fki.yj202588.top

s"值: $b"
来源：http://mir.pycfn.com

[T54] Scala：集合映射
来源：http://syw.0kj1m.cn

List(1, 2, 3).map(_ * 2)
来源：http://aba.daria6918.cn

[T55] Scala：集合过滤
来源：http://cvk.birdmap.top

List(1, 2, 3).filter(_ > 1)
来源：http://osm.zdbjq.cn

[T56] Scala：样例类
来源：http://mso.yj20258888.top

case class User(name: String, age: Int)
来源：http://tpm.guannengcc.top

[T57] Scala：模式匹配
来源：http://ayj.sjlbkw.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vqa.chenjidiqi.icu

[T58] Scala：函数定义
来源：http://uex.jlsjyb.cn

def add(a: Int, b: Int): Int = a + b
来源：http://efn.wangdashe.top

[T59] Scala：循环
来源：http://vgz.xinyue.icu

for (i <- 1 to 10) println(i)
来源：http://fbg.pycfn.com

[T60] Scala：折叠
来源：http://smf.haohaochexian.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bvd.sufxvd.cn

================================================================================
来源：http://qsm.jqgfzy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://uig.shuidangran.top

================================================================================
来源：http://qyq.jqgufenzy.top

[U01] Py：创建虚拟环境
来源：http://aao.jinyuanbaomall.cn

python -m venv .venv && source .venv/bin/activate
来源：http://bmg.gotoacloud.top

[U02] Py：导出 / 安装依赖
来源：http://pwi.shzxlz.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://pbk.ehwqpu.com

[U03] Py：加载 .env 配置
来源：http://hut.ehwqpu.com

from dotenv import load_dotenv; load_dotenv()
来源：http://xln.fzhhl.top

[U04] Py：变量调试打印
来源：http://wer.zhixingplan.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fqi.zhaomingkeji.xyz

[U05] Py：列表去重且保序
来源：http://haj.hysaishi.cn

list(dict.fromkeys(arr))
来源：http://kmg.ehwqpu.com

[U06] Py：合并两个字典
来源：http://cxh.cheryme.top

{**a, **b}
来源：http://sec.jyoumei.cn

[U07] Py：反转字典键值
来源：http://oww.daxiang520.top

{v: k for k, v in d.items()}
来源：http://rmv.hesvh.cn

[U08] Py：展平二维列表
来源：http://uqd.zycfv.cn

[y for x in nested for y in x]
来源：http://fbx.yueranfly.top

[U09] Py：字典取最大值的键
来源：http://cmt.zhixingplan.top

max(d, key=d.get)
来源：http://rgl.daria6918.cn

[U10] Py：按值排序字典
来源：http://dro.cdnleiting.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gcp.daria6918.cn

[U11] Py：生成器表达式
来源：http://ldk.ydjk.org.cn

(x * 2 for x in arr)
来源：http://zhu.wangdashe.top

[U12] Py：取出现最多的 3 个元素
来源：http://jxe.tarul.cn

Counter(arr).most_common(3)
来源：http://xty.chenjidiqi.icu

[U13] Py：固定长度队列
来源：http://ypw.hesvh.cn

deque(maxlen=10)
来源：http://ift.shuidangran.top

[U14] Py：分组收集到列表
来源：http://yoz.hesvh.cn

defaultdict(list)
来源：http://jzp.xuetiantiany.cn

[U15] Py：高精度计时
来源：http://oga.tian-w.cn

t = time.perf_counter()
来源：http://fjo.shanyushiyangkeji.top

[U16] Py：命令行参数解析
来源：http://zug.nanxinkj.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kay.sjlbkw.cn

[U17] Py：初始化日志
来源：http://qhw.ydzc1.top

logging.basicConfig(level=logging.INFO)
来源：http://ppv.mhx1999.top

[U18] Py：预编译正则
来源：http://efn.9152youxi.cn

pat = re.compile(r"\d+")
来源：http://ssn.hywenlv.cn

[U19] Py：正则替换带回调
来源：http://wmy.sjlbkw.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pnv.wangshuangyany.cn

[U20] Py：缓存函数结果
来源：http://ufc.sxryk.cn

@functools.lru_cache(maxsize=None)
来源：http://les.fzhhl.top

[U21] Py：自定义上下文管理器
来源：http://mwi.ydjk.org.cn

@contextlib.contextmanager
来源：http://uob.ctjpmb.com

[U22] Py：矩阵转置
来源：http://mfy.ywan-chungtsiang.top

list(zip(*m))
来源：http://dlc.pycfn.com

[U23] Py：分块读取大文件
来源：http://asp.bbcook.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://iql.tarul.cn

[U24] Py：路径操作
来源：http://arb.cashguo.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://npk.316326.xyz

[U25] Py：CSV 按字典读
来源：http://zyt.iojbl.cn

csv.DictReader(f)
来源：http://pgs.havefunace.top

[U26] Py：并发下载
来源：http://xbu.c1oappe.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fkc.jinqigufen.top

[U27] Py：异步 HTTP
来源：http://bht.yanxiufei.cn

aiohttp.ClientSession() 配合 async with
来源：http://dwy.sweek.top

[U28] Py：类型别名
来源：http://zuh.gogol.net.cn

UserId = int
来源：http://zhg.jqgufenzy.top

[U29] Py：属性校验
来源：http://bbk.tian-w.cn

@property 与 @x.setter 配合
来源：http://ugw.mhx1999.top

[U30] Py：数据类
来源：http://sca.sjlbkw.cn

@dataclass(slots=True)
来源：http://cjd.shangyingyoupin.top

[U31] Py：单测
来源：http://yix.zhixingplan.top

python -m pytest -q
来源：http://bie.cucudq.cn

[U32] Py：代码格式化
来源：http://gme.sxryk.cn

ruff format . && ruff check --fix .
来源：http://zic.kuanghao11.cn

[U33] Py：打包发布
来源：http://ovn.yj20258888.top

python -m build  （依赖 pyproject.toml）
来源：http://dha.zycfv.cn

[U34] Py：判断编码
来源：http://zqy.yj20258888.top

chardet.detect(raw)
来源：http://jia.sjlbkw.cn

[U35] Py：发送邮件
来源：http://lup.cheryme.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://udl.epnwcf.com

[U36] Py：定时任务
来源：http://llt.dashuyun.cn

schedule.every(10).minutes.do(job)
来源：http://oxs.jinghuilouyu.cn

[U37] Py：读写 Excel
来源：http://ggn.zycfv.cn

pandas.read_excel / DataFrame.to_excel
来源：http://xxz.hnxiangtu.top

[U38] Py：获取脚本所在目录
来源：http://glf.c1oappe.top

Path(__file__).resolve().parent
来源：http://kza.andypj.xyz

[U39] Py：判断是否在交互环境
来源：http://rms.shanyushiyangkeji.top

sys.stdout.isatty()
来源：http://aae.sjlbkw.cn

[U40] Py：打印到标准错误
来源：http://utq.epnwcf.com

print("err", file=sys.stderr)
来源：http://hze.zhaomingkeji.xyz

[U41] PHP：初始化 Composer 项目
来源：http://ibi.hnxiangtu.top

composer init;  composer require guzzlehttp/guzzle
来源：http://kss.9152youxi.cn

[U42] PHP：PSR-4 自动加载
来源：http://pmc.yuxming.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nkt.sweek.top

[U43] PHP：声明命名空间
来源：http://xfk.zdbjq.cn

namespace App\Http;
来源：http://joq.sufxvd.cn

[U44] PHP：开启严格类型
来源：http://wzm.zhiwuduotai.top

declare(strict_types=1);
来源：http://jsr.jinqigfzy.top

[U45] PHP：类型声明与返回类型
来源：http://ppn.hywenlv.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://csq.bjfxy.top

[U46] PHP：可空类型
来源：http://qwl.kuanghao11.cn

?string $name = null
来源：http://eqs.chenjidiqi.icu

[U47] PHP：联合类型
来源：http://hwr.yueranfly.top

int|string $id
来源：http://jxw.c1oappe.top

[U48] PHP：纯枚举
来源：http://opz.hongshengwenyu.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://aco.pycfn.com

[U49] PHP：只读属性
来源：http://sma.zycfv.cn

public readonly string $name
来源：http://mol.chenlongwang.top

[U50] PHP：构造器属性提升
来源：http://hez.fktsv.cn

public function __construct(private int $id) {}
来源：http://kus.zhengqikj.top

[U51] PHP：数组解构
来源：http://hjj.sweek.top

[$a, $b] = $arr;
来源：http://erd.havefunace.top

[U52] PHP：箭头函数
来源：http://jmm.daria6918.cn

$double = fn($x) => $x * 2;
来源：http://uzm.sufxvd.cn

[U53] PHP：空合并运算符
来源：http://rnq.nanxuanxn.top

$v = $a ?? $b ?? "default";
来源：http://wxu.hywenlv.cn

[U54] PHP：空安全调用
来源：http://cnu.wangdashe.top

$obj?->method()
来源：http://eic.xingfuxueyuan.xyz

[U55] PHP：match 表达式
来源：http://ifx.sysykeji.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zpi.guowangkeji.top

[U56] PHP：命名参数
来源：http://ymr.cdnleiting.top

f(a: 1, b: 2)
来源：http://lqj.gzhubu.top

[U57] PHP：字符串插值
来源：http://jpp.nanxinkj.top

"值: {$a}"
来源：http://xoz.zycfv.cn

[U58] PHP：数组三件套
来源：http://hnd.fanxiaobao.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nlb.vqdsnc.cn

[U59] PHP：自定义排序
来源：http://rht.meibo888.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nza.zhoulong.xyz

[U60] PHP：JSON 编解码
来源：http://apj.yj20258888.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://slc.sweek.top

[U61] PHP：正则
来源：http://mso.bbcook.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mqy.hongshengwenyu.top

[U62] PHP：日期对象
来源：http://joa.cheryme.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://dec.cheryme.top

[U63] PHP：文件读写
来源：http://avu.andypj.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ugo.316326.xyz

[U64] PHP：目录遍历
来源：http://ito.ydjk.org.cn

glob("dir/*.php");  scandir("dir");
来源：http://agt.zdqjudy.top

[U65] PHP：会话
来源：http://rqx.cqqwz.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://goq.shangyingyoupin.top

[U66] PHP：设置 Cookie
来源：http://kfv.shangyingyoupin.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ilh.hcnkem.com

[U67] PHP：处理文件上传
来源：http://inm.cqqwz.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://sdc.jqgufenzy.top

[U68] PHP：PDO 连接
来源：http://bvo.feifeiyinyue.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hcl.bbcook.cn

[U69] PHP：PDO 预处理
来源：http://vhi.uphjek.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lsi.zhengqikj.top

[U70] PHP：PDO 事务
来源：http://quh.chenlongwang.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qcx.ctjpmb.com

[U71] PHP：抛出异常
来源：http://kro.nanxinkj.top

throw new RuntimeException("失败", 500);
来源：http://jri.fehbvm.com

[U72] PHP：写错误日志
来源：http://wjf.epnwcf.com

error_log("失败: " . $e->getMessage());
来源：http://qif.jiagoushi.top

[U73] PHP：读取 ini 配置
来源：http://hcg.xinyue.icu

parse_ini_file("config.ini", true)
来源：http://lns.hfpthk.cn

[U74] PHP：读取环境变量
来源：http://gjm.kuanghao11.cn

getenv("APP_ENV") ?: "production"
来源：http://cxg.sxryk.cn

[U75] PHP：依赖注入
来源：http://zem.redwolf501.top

composer require psr/container
来源：http://zxu.fengsongda.top

[U76] PHP：简单路由
来源：http://znz.tanke756.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wdn.jqgufenzy.top

[U77] PHP：模板渲染
来源：http://ldn.jinyuanbaomall.cn

composer require twig/twig
来源：http://fuc.jinqigufen.top

[U78] PHP：单元测试
来源：http://eqe.fengsongda.top

composer require --dev phpunit/phpunit
来源：http://lap.aibaodan.cn

[U79] PHP：静态分析
来源：http://kxj.jqgufenzy.top

composer require --dev phpstan/phpstan
来源：http://bce.uphjek.com

[U80] PHP：代码规范修复
来源：http://npf.jinqigfzy.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://eyq.daxiang520.top

[U81] JS：初始化项目
来源：http://yby.hcnkem.com

npm init -y;  npm i express
来源：http://ggx.yj20258.top

[U82] JS：package.json 脚本
来源：http://hrb.chenzaomai.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://izp.zycfv.cn

[U83] JS：ES Module 导入导出
来源：http://dsx.hysaishi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://xzg.jianghu66.top

[U84] JS：CommonJS 写法
来源：http://sux.guowangkeji.top

module.exports = { a };  const { a } = require("./m");
来源：http://mxw.xingfuxueyuan.xyz

[U85] JS：可选链
来源：http://bsx.havefunace.top

a?.b?.c
来源：http://vnk.ywan-chungtsiang.top

[U86] JS：空值合并
来源：http://zwn.wangdashe.top

a ?? b
来源：http://sbn.sysykeji.top

[U87] JS：解构默认值
来源：http://vxe.hongshengwenyu.top

const { a = 1, b = 2 } = obj;
来源：http://xzy.316326.xyz

[U88] JS：对象展开合并
来源：http://uxk.snrcjt.cn

{ ...a, ...b }
来源：http://edg.yj20258888.top

[U89] JS：数组去重
来源：http://fav.iojbl.cn

[...new Set(arr)]
来源：http://ugt.ctjpmb.com

[U90] JS：数字数组排序
来源：http://gbo.jianghu66.top

[...arr].sort((a, b) => a - b)
来源：http://apv.mhx1999.top

[U91] JS：对象键值遍历
来源：http://fzq.birdmap.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://aoi.xziqi.cn

[U92] JS：深拷贝
来源：http://qhw.xingfuxueyuan.xyz

structuredClone(obj)
来源：http://ydb.jyoumei.cn

[U93] JS：模板字符串
来源：http://sfy.zhijiandao.cn

`共 ${n} 条`
来源：http://ojv.zdbjq.cn

[U94] JS：箭头函数
来源：http://esc.sxryk.cn

const double = x => x * 2;
来源：http://naf.bjfxy.top

[U95] JS：Promise 包装
来源：http://wts.kuanghao11.cn

new Promise((resolve, reject) => {})
来源：http://hxd.guowangkeji.top

[U96] JS：async/await 与异常
来源：http://jgi.uphjek.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zfh.nanxinkj.top

[U97] JS：并发请求
来源：http://fxi.wangshuangyany.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ybx.yj202588.top

[U98] JS：fetch 带 JSON
来源：http://hhh.hywenlv.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://yfx.9152youxi.cn

[U99] JS：事件监听
来源：http://rde.wangshuangyany.cn

el.addEventListener("click", e => {})
来源：http://hyp.chenlongwang.top

[U100] JS：DOM 查询
来源：http://gqg.zhijiandao.cn

document.querySelector(".item")
来源：http://khc.jlsjyb.cn

[U101] JS：classList 操作
来源：http://mot.tanke756.top

el.classList.toggle("active")
来源：http://nho.yj20258888.top

[U102] JS：本地存储
来源：http://csm.jinqigufen.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://gqm.pycfn.com

[U103] JS：定时器
来源：http://klc.vehdjk.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pub.jyoumei.cn

[U104] JS：防抖
来源：http://uxo.cqqwz.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zlk.tanke756.top

[U105] JS：节流
来源：http://oiu.vqdsnc.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zho.aizwys.cn

[U106] JS：日期格式化
来源：http://vvo.ehwqpu.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://brf.xinyue.icu

[U107] JS：数字千分位
来源：http://dar.yuanzhike.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://erm.ppjwa.cn

[U108] JS：随机整数
来源：http://hac.c1oappe.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pzs.dianchejie.cn

[U109] JS：数组分组
来源：http://qde.xuetiantiany.cn

Object.groupBy(arr, x => x.type)
来源：http://kfu.haohaochexian.top

[U110] JS：数组分块
来源：http://uni.fehbvm.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://msi.andypj.xyz

[U111] JS：对象转 Map
来源：http://wkv.9152youxi.cn

new Map(Object.entries(obj))
来源：http://nno.xuetiantiany.cn

[U112] JS：字符串补位
来源：http://zzq.nwbrower.top

"7".padStart(3, "0")
来源：http://fqj.316326.xyz

[U113] JS：正则替换全部
来源：http://jcp.aizwys.cn

s.replaceAll("a", "b")
来源：http://ikl.c1oappe.top

[U114] JS：JSON 深比较
来源：http://qrt.tanke756.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://fas.fanxiaobao.xyz

[U115] JS：生成 UUID
来源：http://arr.tian-w.cn

crypto.randomUUID()
来源：http://glk.vehdjk.com

[U116] JS：类型检查（JSDoc）
来源：http://zpo.sufxvd.cn

/** @param {string} name */ function f(name) {}
来源：http://uao.shangyingyoupin.top

[U117] JS：单元测试
来源：http://jyi.yj202588.top

npm i -D vitest;  npx vitest
来源：http://hfi.nanxinkj.top

[U118] JS：开发服务器
来源：http://fhv.yvedp.cn

npm i -D vite;  npx vite
来源：http://vfp.guowangkeji.top

[U119] JS：生产构建
来源：http://rau.tian-w.cn

npx vite build
来源：http://nnh.hfpthk.cn

[U120] JS：读取环境变量（Vite）
来源：http://zeo.haohaochexian.top

import.meta.env.VITE_API_URL
来源：http://zcc.zhiwuduotai.top

================================================================================
来源：http://vrh.shangyingyoupin.top

统计汇总
来源：http://xfh.xziqi.cn

================================================================================
来源：http://yxu.tarul.cn

按语言统计（条）：
来源：http://ook.ehwqpu.com

Python ......... 252
来源：http://gmk.chenlongwang.top

PHP ............ 252
来源：http://tdj.ybcxt.top

JavaScript ..... 252
来源：http://upx.havefunace.top

TypeScript ..... 212
来源：http://gda.zdqjudy.top


<!-- 参考信息 -->