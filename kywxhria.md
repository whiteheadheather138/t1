代发 wailian999

[T37] Lua：字符串拼接
来源：http://kcs.yueranfly.top

"a" .. "b"
来源：http://jfa.andypj.xyz

[T38] Lua：条件
来源：http://xwy.jyoumei.cn

if x > 0 then print("正") end
来源：http://svg.cdnleiting.top

[T39] Lua：模式匹配
来源：http://fag.sufxvd.cn

string.find(s, "%d+")
来源：http://ref.chenzaomai.com

[T40] Lua：元表
来源：http://vml.quarkkingdee.top

setmetatable({}, { __index = base })
来源：http://kcy.jinqigufen.top

[T41] Perl：Hello World
来源：http://xlf.kuanghao11.cn

print "Hello\n";
来源：http://she.meibo888.top

[T42] Perl：变量类型
来源：http://gst.tianlin.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://oug.haohaochexian.top

[T43] Perl：字符串插值
来源：http://ahs.yonumen.top

"值: $a"
来源：http://ykk.xuanzx.com

[T44] Perl：条件
来源：http://ccf.dashuyun.cn

if ($a > 0) { print "正"; }
来源：http://xhg.havefunace.top

[T45] Perl：数组遍历
来源：http://qfl.shanyushiyangtech.top

for my $x (@arr) { print $x; }
来源：http://qon.cqqwz.cn

[T46] Perl：哈希操作
来源：http://utm.haohaochexian.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ggs.sjlbkw.cn

[T47] Perl：正则捕获
来源：http://atl.yonumen.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://jan.xuanzx.com

[T48] Perl：正则替换
来源：http://mdd.birdmap.top

$s =~ s/old/new/g;
来源：http://mkl.smart0.xyz

[T49] Perl：函数
来源：http://ihr.c1oappe.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rrl.hammf.cn

[T50] Perl：逐行读文件
来源：http://iuh.zhiwuduotai.top

open my $fh, "<", "a.txt" or die $!;
来源：http://riy.xingfuxueyuan.xyz

while (my $line = <$fh>) { print $line; }
来源：http://qnl.sweek.top

[T51] Scala：Hello World
来源：http://mca.hongshengwenyu.top

println("Hello")
来源：http://kea.yj202588.top

[T52] Scala：变量
来源：http://ucr.fktsv.cn

val a = 1;  var b = 2
来源：http://yoi.shuidangran.top

[T53] Scala：字符串插值
来源：http://uwg.yanxiufei.cn

s"值: $b"
来源：http://lxo.sjlbkw.cn

[T54] Scala：集合映射
来源：http://eku.wangshuangyany.cn

List(1, 2, 3).map(_ * 2)
来源：http://kgx.shanyushiyangtech.top

[T55] Scala：集合过滤
来源：http://dll.ybcxt.top

List(1, 2, 3).filter(_ > 1)
来源：http://bgg.ivvv.top

[T56] Scala：样例类
来源：http://pml.yj20258888.top

case class User(name: String, age: Int)
来源：http://znl.iojbl.cn

[T57] Scala：模式匹配
来源：http://sbj.snrcjt.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://nsf.nanxinkj.top

[T58] Scala：函数定义
来源：http://cud.dashuyun.cn

def add(a: Int, b: Int): Int = a + b
来源：http://oec.yvedp.cn

[T59] Scala：循环
来源：http://omr.nanxinkj.top

for (i <- 1 to 10) println(i)
来源：http://kcy.xinyue.icu

[T60] Scala：折叠
来源：http://rzh.316326.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fjb.9152youxi.cn

================================================================================
来源：http://twb.jinqigfzy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://khv.haohaochexian.top

================================================================================
来源：http://tvl.jyoumei.cn

[U01] Py：创建虚拟环境
来源：http://vgo.dianchejie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://dnf.dashuyun.cn

[U02] Py：导出 / 安装依赖
来源：http://acf.svipenyu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://exe.zhoulong.xyz

[U03] Py：加载 .env 配置
来源：http://tzs.yj20258888.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ypc.xziqi.cn

[U04] Py：变量调试打印
来源：http://rsc.shzxlz.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qbu.yangfankeji.com

[U05] Py：列表去重且保序
来源：http://nto.jinqigfzy.top

list(dict.fromkeys(arr))
来源：http://bch.cheryme.top

[U06] Py：合并两个字典
来源：http://sbv.mhx1999.top

{**a, **b}
来源：http://rul.wangshuangyany.cn

[U07] Py：反转字典键值
来源：http://rok.ehwqpu.com

{v: k for k, v in d.items()}
来源：http://izm.yangfankeji.com

[U08] Py：展平二维列表
来源：http://qha.gzhubu.top

[y for x in nested for y in x]
来源：http://xgk.yongpay.top

[U09] Py：字典取最大值的键
来源：http://mdk.chenlongwang.top

max(d, key=d.get)
来源：http://djp.fehbvm.com

[U10] Py：按值排序字典
来源：http://uyo.feifeiyinyue.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mkg.zdbjq.cn

[U11] Py：生成器表达式
来源：http://qwn.chenjidiqi.icu

(x * 2 for x in arr)
来源：http://eye.zdbjq.cn

[U12] Py：取出现最多的 3 个元素
来源：http://bsi.havefunace.top

Counter(arr).most_common(3)
来源：http://nau.tarul.cn

[U13] Py：固定长度队列
来源：http://jux.hfpthk.cn

deque(maxlen=10)
来源：http://xii.zhaomingkeji.xyz

[U14] Py：分组收集到列表
来源：http://stu.fktsv.cn

defaultdict(list)
来源：http://uda.cheryme.top

[U15] Py：高精度计时
来源：http://lcu.sweek.top

t = time.perf_counter()
来源：http://inu.chenlongwang.top

[U16] Py：命令行参数解析
来源：http://pmq.dashuyun.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wyb.gzhubu.top

[U17] Py：初始化日志
来源：http://uzc.zhijiandao.cn

logging.basicConfig(level=logging.INFO)
来源：http://ajp.guannengcc.top

[U18] Py：预编译正则
来源：http://dzz.sjlbkw.cn

pat = re.compile(r"\d+")
来源：http://stg.yj20258.top

[U19] Py：正则替换带回调
来源：http://fnl.chenzaomai.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://djw.cdnleiting.top

[U20] Py：缓存函数结果
来源：http://jom.xziqi.cn

@functools.lru_cache(maxsize=None)
来源：http://arv.fktsv.cn

[U21] Py：自定义上下文管理器
来源：http://cxc.yfazqb.com

@contextlib.contextmanager
来源：http://elx.fengsongda.top

[U22] Py：矩阵转置
来源：http://ujr.jqgufenzy.top

list(zip(*m))
来源：http://cfe.zycfv.cn

[U23] Py：分块读取大文件
来源：http://odx.xziqi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mfl.daxiang520.top

[U24] Py：路径操作
来源：http://odk.sufxvd.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vqy.aibaodan.cn

[U25] Py：CSV 按字典读
来源：http://jfb.uphjek.com

csv.DictReader(f)
来源：http://rrs.bjfxy.top

[U26] Py：并发下载
来源：http://ing.ywan-chungtsiang.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://noi.gzhubu.top

[U27] Py：异步 HTTP
来源：http://pbh.redwolf501.top

aiohttp.ClientSession() 配合 async with
来源：http://gzy.aibaodan.cn

[U28] Py：类型别名
来源：http://hex.yangfankeji.com

UserId = int
来源：http://byi.uphjek.com

[U29] Py：属性校验
来源：http://mqe.bbcook.cn

@property 与 @x.setter 配合
来源：http://osy.chenjidiqi.icu

[U30] Py：数据类
来源：http://arf.ppjwa.cn

@dataclass(slots=True)
来源：http://jvk.shangyingyoupin.top

[U31] Py：单测
来源：http://ezn.hcnkem.com

python -m pytest -q
来源：http://uvk.zhijiandao.cn

[U32] Py：代码格式化
来源：http://wyt.yfazqb.com

ruff format . && ruff check --fix .
来源：http://hje.birdmap.top

[U33] Py：打包发布
来源：http://pty.guannengcc.top

python -m build  （依赖 pyproject.toml）
来源：http://tsg.bjfxy.top

[U34] Py：判断编码
来源：http://kqo.yj202588.top

chardet.detect(raw)
来源：http://tbp.chenjidiqi.icu

[U35] Py：发送邮件
来源：http://sur.cdnleiting.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hjh.epnwcf.com

[U36] Py：定时任务
来源：http://skh.shanyushiyangtech.top

schedule.every(10).minutes.do(job)
来源：http://gqm.jinqigfzy.top

[U37] Py：读写 Excel
来源：http://iup.pycfn.com

pandas.read_excel / DataFrame.to_excel
来源：http://djd.wangdashe.top

[U38] Py：获取脚本所在目录
来源：http://vgr.tian-w.cn

Path(__file__).resolve().parent
来源：http://ann.chenlongwang.top

[U39] Py：判断是否在交互环境
来源：http://yic.tanke756.top

sys.stdout.isatty()
来源：http://eid.yangfankeji.com

[U40] Py：打印到标准错误
来源：http://zno.bjfxy.top

print("err", file=sys.stderr)
来源：http://cxt.zhiwuduotai.top

[U41] PHP：初始化 Composer 项目
来源：http://hlz.hcnkem.com

composer init;  composer require guzzlehttp/guzzle
来源：http://eot.zycfv.cn

[U42] PHP：PSR-4 自动加载
来源：http://hew.tian-w.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yqm.wangdashe.top

[U43] PHP：声明命名空间
来源：http://cel.hysaishi.cn

namespace App\Http;
来源：http://owf.zhoulong.xyz

[U44] PHP：开启严格类型
来源：http://fkk.nwbrower.top

declare(strict_types=1);
来源：http://htp.iojbl.cn

[U45] PHP：类型声明与返回类型
来源：http://gcg.ydjk.org.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://cjk.jqgfzy.top

[U46] PHP：可空类型
来源：http://dwr.shzxlz.cn

?string $name = null
来源：http://mri.yj20258888.top

[U47] PHP：联合类型
来源：http://cpr.gotoacloud.top

int|string $id
来源：http://bkc.xingfuxueyuan.xyz

[U48] PHP：纯枚举
来源：http://grm.jianghu66.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bva.fengsongda.top

[U49] PHP：只读属性
来源：http://eng.shanyushiyangtech.top

public readonly string $name
来源：http://glu.dashuyun.cn

[U50] PHP：构造器属性提升
来源：http://afx.zycfv.cn

public function __construct(private int $id) {}
来源：http://zwh.gogol.net.cn

[U51] PHP：数组解构
来源：http://yhw.gogol.net.cn

[$a, $b] = $arr;
来源：http://wam.jiagoushi.top

[U52] PHP：箭头函数
来源：http://oum.jinqigufen.top

$double = fn($x) => $x * 2;
来源：http://nse.hfpthk.cn

[U53] PHP：空合并运算符
来源：http://vcv.ydjk.org.cn

$v = $a ?? $b ?? "default";
来源：http://vad.jqgufenzy.top

[U54] PHP：空安全调用
来源：http://ypq.zdbjq.cn

$obj?->method()
来源：http://kqj.dianchejie.cn

[U55] PHP：match 表达式
来源：http://xgl.yj20258888.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qmu.sweek.top

[U56] PHP：命名参数
来源：http://dgz.zhoulong.xyz

f(a: 1, b: 2)
来源：http://xwg.yangfankeji.com

[U57] PHP：字符串插值
来源：http://zug.zhijiandao.cn

"值: {$a}"
来源：http://epp.yongpay.top

[U58] PHP：数组三件套
来源：http://qma.zdqjudy.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gby.zhiwuduotai.top

[U59] PHP：自定义排序
来源：http://vzr.fanxiaobao.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ikz.0kj1m.cn

[U60] PHP：JSON 编解码
来源：http://hfs.pycfn.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vfb.vqdsnc.cn

[U61] PHP：正则
来源：http://tdh.zhijiandao.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://are.jinqigfzy.top

[U62] PHP：日期对象
来源：http://akm.zhaomingkeji.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://utq.ywan-chungtsiang.top

[U63] PHP：文件读写
来源：http://ngy.vehdjk.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lvn.hfpthk.cn

[U64] PHP：目录遍历
来源：http://prv.cqqwz.cn

glob("dir/*.php");  scandir("dir");
来源：http://vro.zhixingplan.top

[U65] PHP：会话
来源：http://veb.hnqzz.top

session_start();  $_SESSION["uid"] = 1;
来源：http://usi.yuxming.cn

[U66] PHP：设置 Cookie
来源：http://sjf.bbcook.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dvu.tianlin.xyz

[U67] PHP：处理文件上传
来源：http://oha.cqqwz.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zbf.havefunace.top

[U68] PHP：PDO 连接
来源：http://lvk.gogol.net.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fsv.hfpthk.cn

[U69] PHP：PDO 预处理
来源：http://twt.hysaishi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zbe.shuidangran.top

[U70] PHP：PDO 事务
来源：http://llb.jinqigfzy.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wqq.hcnkem.com

[U71] PHP：抛出异常
来源：http://riu.uphjek.com

throw new RuntimeException("失败", 500);
来源：http://roh.epnwcf.com

[U72] PHP：写错误日志
来源：http://udl.haohaochexian.top

error_log("失败: " . $e->getMessage());
来源：http://ntl.nwbrower.top

[U73] PHP：读取 ini 配置
来源：http://dah.fehbvm.com

parse_ini_file("config.ini", true)
来源：http://txf.tian-w.cn

[U74] PHP：读取环境变量
来源：http://htc.chenjidiqi.icu

getenv("APP_ENV") ?: "production"
来源：http://aee.birdmap.top

[U75] PHP：依赖注入
来源：http://alg.gotoacloud.top

composer require psr/container
来源：http://efl.hongshengwenyu.top

[U76] PHP：简单路由
来源：http://nzn.gogol.net.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jup.smart0.xyz

[U77] PHP：模板渲染
来源：http://dgj.zhixingplan.top

composer require twig/twig
来源：http://fdx.jinyuanbaomall.cn

[U78] PHP：单元测试
来源：http://cwa.ehwqpu.com

composer require --dev phpunit/phpunit
来源：http://fnk.zhijiandao.cn

[U79] PHP：静态分析
来源：http://rcc.andypj.xyz

composer require --dev phpstan/phpstan
来源：http://yrk.mhx1999.top

[U80] PHP：代码规范修复
来源：http://lig.fehbvm.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://bjd.xziqi.cn

[U81] JS：初始化项目
来源：http://pez.feifeiyinyue.top

npm init -y;  npm i express
来源：http://ppc.xuanzx.com

[U82] JS：package.json 脚本
来源：http://pov.dianchejie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bsv.zhengqikj.top

[U83] JS：ES Module 导入导出
来源：http://kmc.yueranfly.top

export const a = 1;  import { a } from "./m.js";
来源：http://uiu.c1oappe.top

[U84] JS：CommonJS 写法
来源：http://nsy.shuidangran.top

module.exports = { a };  const { a } = require("./m");
来源：http://hyp.shuidangran.top

[U85] JS：可选链
来源：http://syt.9152youxi.cn

a?.b?.c
来源：http://ecf.daria6918.cn

[U86] JS：空值合并
来源：http://ckj.bbcook.cn

a ?? b
来源：http://phi.zdqjudy.top

[U87] JS：解构默认值
来源：http://fiw.epnwcf.com

const { a = 1, b = 2 } = obj;
来源：http://oby.xingfuxueyuan.xyz

[U88] JS：对象展开合并
来源：http://lhr.zhoulong.xyz

{ ...a, ...b }
来源：http://vyf.haohaochexian.top

[U89] JS：数组去重
来源：http://pdx.vqdsnc.cn

[...new Set(arr)]
来源：http://nhz.chenzaomai.com

[U90] JS：数字数组排序
来源：http://thb.sufxvd.cn

[...arr].sort((a, b) => a - b)
来源：http://tjt.shanyushiyangkeji.top

[U91] JS：对象键值遍历
来源：http://bhs.ydzc1.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rox.sweek.top

[U92] JS：深拷贝
来源：http://jut.ppjwa.cn

structuredClone(obj)
来源：http://ypv.zhengqikj.top

[U93] JS：模板字符串
来源：http://lfp.bjfxy.top

`共 ${n} 条`
来源：http://hcz.cqqwz.cn

[U94] JS：箭头函数
来源：http://msx.shanyushiyangkeji.top

const double = x => x * 2;
来源：http://oby.shzxlz.cn

[U95] JS：Promise 包装
来源：http://idv.fanxiaobao.xyz

new Promise((resolve, reject) => {})
来源：http://yqu.gzhubu.top

[U96] JS：async/await 与异常
来源：http://xux.fzhhl.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://kek.zhiwuduotai.top

[U97] JS：并发请求
来源：http://yrv.zycfv.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ikk.ybcxt.top

[U98] JS：fetch 带 JSON
来源：http://tdu.bjfxy.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ift.hfpthk.cn

[U99] JS：事件监听
来源：http://yox.ctjpmb.com

el.addEventListener("click", e => {})
来源：http://fea.ydzc1.top

[U100] JS：DOM 查询
来源：http://cni.zycfv.cn

document.querySelector(".item")
来源：http://uwa.tianlin.xyz

[U101] JS：classList 操作
来源：http://hpg.chenjidiqi.icu

el.classList.toggle("active")
来源：http://bwo.zdbjq.cn

[U102] JS：本地存储
来源：http://fno.jianghu66.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://hll.zdqjudy.top

[U103] JS：定时器
来源：http://tpd.hammf.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qmy.mhx1999.top

[U104] JS：防抖
来源：http://utt.yongpay.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qjj.tanke756.top

[U105] JS：节流
来源：http://oek.ybcxt.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dig.epnwcf.com

[U106] JS：日期格式化
来源：http://uwv.andypj.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vnk.jyoumei.cn

[U107] JS：数字千分位
来源：http://zox.yanxiufei.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qqj.jinqigfzy.top

[U108] JS：随机整数
来源：http://tnx.zhaomingkeji.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cus.jyoumei.cn

[U109] JS：数组分组
来源：http://tih.vqdsnc.cn

Object.groupBy(arr, x => x.type)
来源：http://nbr.hnqzz.top

[U110] JS：数组分块
来源：http://fax.jinqigufen.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mev.smart0.xyz

[U111] JS：对象转 Map
来源：http://kfa.chenjidiqi.icu

new Map(Object.entries(obj))
来源：http://edx.yj20258.top

[U112] JS：字符串补位
来源：http://xxq.tanke756.top

"7".padStart(3, "0")
来源：http://pda.aibaodan.cn

[U113] JS：正则替换全部
来源：http://mye.nanxinkj.top

s.replaceAll("a", "b")
来源：http://ugs.tanke756.top

[U114] JS：JSON 深比较
来源：http://yjv.svipenyu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://cpw.0kj1m.cn

[U115] JS：生成 UUID
来源：http://uyu.gogol.net.cn

crypto.randomUUID()
来源：http://ubd.vqdsnc.cn

[U116] JS：类型检查（JSDoc）
来源：http://uvt.zhixingplan.top

/** @param {string} name */ function f(name) {}
来源：http://szp.feifeiyinyue.top

[U117] JS：单元测试
来源：http://gux.tianlin.xyz

npm i -D vitest;  npx vitest
来源：http://cer.gogol.net.cn

[U118] JS：开发服务器
来源：http://pos.shuidangran.top

npm i -D vite;  npx vite
来源：http://rbr.9152youxi.cn

[U119] JS：生产构建
来源：http://whx.redwolf501.top

npx vite build
来源：http://nqh.yj202588.top

[U120] JS：读取环境变量（Vite）
来源：http://rte.shuidangran.top

import.meta.env.VITE_API_URL
来源：http://ahf.sjlbkw.cn

================================================================================
来源：http://vno.shanyushiyangtech.top

统计汇总
来源：http://jsb.nanxinkj.top

================================================================================
来源：http://jyw.ivvv.top

按语言统计（条）：
来源：http://wtj.yfazqb.com

Python ......... 252
来源：http://dbh.sysykeji.top

PHP ............ 252
来源：http://ezo.redwolf501.top

JavaScript ..... 252
来源：http://ssv.shanyushiyangkeji.top

TypeScript ..... 212
来源：http://lvw.tarul.cn


<!-- 参考信息 -->