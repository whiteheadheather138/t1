代发 wailian999

[T41] Perl：Hello World
来源：http://nod.aibaodan.cn

print "Hello\n";
来源：http://jeq.gaohongyu789.top

[T42] Perl：变量类型
来源：http://sgc.xuetiantiany.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://iwl.yfazqb.com

[T43] Perl：字符串插值
来源：http://ulu.daria6918.cn

"值: $a"
来源：http://sfc.xziqi.cn

[T44] Perl：条件
来源：http://tub.chenzaomai.com

if ($a > 0) { print "正"; }
来源：http://bji.zhiwuduotai.top

[T45] Perl：数组遍历
来源：http://iiw.wangdashe.top

for my $x (@arr) { print $x; }
来源：http://bok.ctjpmb.com

[T46] Perl：哈希操作
来源：http://zbg.daxiang520.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://svp.ydzc1.top

[T47] Perl：正则捕获
来源：http://obw.xuetiantiany.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://tbf.jinyuanbaomall.cn

[T48] Perl：正则替换
来源：http://vde.birdmap.top

$s =~ s/old/new/g;
来源：http://vjm.gotoacloud.top

[T49] Perl：函数
来源：http://qxj.cheryme.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rel.hysaishi.cn

[T50] Perl：逐行读文件
来源：http://gsp.gaohongyu789.top

open my $fh, "<", "a.txt" or die $!;
来源：http://itl.jiagoushi.top

while (my $line = <$fh>) { print $line; }
来源：http://wxc.chenzaomai.com

[T51] Scala：Hello World
来源：http://xcc.yuxming.cn

println("Hello")
来源：http://vvh.fehbvm.com

[T52] Scala：变量
来源：http://yat.cdnleiting.top

val a = 1;  var b = 2
来源：http://bwy.cheryme.top

[T53] Scala：字符串插值
来源：http://xut.hywenlv.cn

s"值: $b"
来源：http://itj.zdbjq.cn

[T54] Scala：集合映射
来源：http://ffj.sufxvd.cn

List(1, 2, 3).map(_ * 2)
来源：http://yfg.iojbl.cn

[T55] Scala：集合过滤
来源：http://xjb.yfazqb.com

List(1, 2, 3).filter(_ > 1)
来源：http://osp.gogol.net.cn

[T56] Scala：样例类
来源：http://epp.zhixingplan.top

case class User(name: String, age: Int)
来源：http://yka.guannengcc.top

[T57] Scala：模式匹配
来源：http://gyk.zhijiandao.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://yga.cdnleiting.top

[T58] Scala：函数定义
来源：http://srv.dianchejie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zec.xingfuxueyuan.xyz

[T59] Scala：循环
来源：http://voo.bbcook.cn

for (i <- 1 to 10) println(i)
来源：http://elj.jqgufenzy.top

[T60] Scala：折叠
来源：http://niy.jinyuanbaomall.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pst.sweek.top

================================================================================
来源：http://xlt.pengpengdd.cyou

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ibu.shzxlz.cn

================================================================================
来源：http://ffn.fanxiaobao.xyz

[U01] Py：创建虚拟环境
来源：http://iow.zycfv.cn

python -m venv .venv && source .venv/bin/activate
来源：http://doo.haohaochexian.top

[U02] Py：导出 / 安装依赖
来源：http://akz.sxryk.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://omt.andypj.xyz

[U03] Py：加载 .env 配置
来源：http://alh.hywenlv.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://dtn.zdbjq.cn

[U04] Py：变量调试打印
来源：http://lik.shuidangran.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://oym.hongshengwenyu.top

[U05] Py：列表去重且保序
来源：http://zla.zdbjq.cn

list(dict.fromkeys(arr))
来源：http://zjq.meibo888.top

[U06] Py：合并两个字典
来源：http://nhw.aizwys.cn

{**a, **b}
来源：http://rxz.hongshengwenyu.top

[U07] Py：反转字典键值
来源：http://xze.shuidangran.top

{v: k for k, v in d.items()}
来源：http://xeq.ybcxt.top

[U08] Py：展平二维列表
来源：http://tbs.xingfuxueyuan.xyz

[y for x in nested for y in x]
来源：http://mhu.redwolf501.top

[U09] Py：字典取最大值的键
来源：http://gii.dashuyun.cn

max(d, key=d.get)
来源：http://zai.sufxvd.cn

[U10] Py：按值排序字典
来源：http://upe.sysykeji.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lbs.vehdjk.com

[U11] Py：生成器表达式
来源：http://wns.yj20258888.top

(x * 2 for x in arr)
来源：http://pyc.cdnleiting.top

[U12] Py：取出现最多的 3 个元素
来源：http://dsa.0kj1m.cn

Counter(arr).most_common(3)
来源：http://ywy.wangshuangyany.cn

[U13] Py：固定长度队列
来源：http://vvs.xinyue.icu

deque(maxlen=10)
来源：http://mmy.yangfankeji.com

[U14] Py：分组收集到列表
来源：http://hqw.yj20258.top

defaultdict(list)
来源：http://cbf.yanxiufei.cn

[U15] Py：高精度计时
来源：http://fvp.yanxiufei.cn

t = time.perf_counter()
来源：http://ejw.ybcxt.top

[U16] Py：命令行参数解析
来源：http://wux.hongshengwenyu.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lbj.feifeiyinyue.top

[U17] Py：初始化日志
来源：http://mit.svipenyu.cn

logging.basicConfig(level=logging.INFO)
来源：http://ngn.zdqjudy.top

[U18] Py：预编译正则
来源：http://lbg.yj20258888.top

pat = re.compile(r"\d+")
来源：http://asa.wangdashe.top

[U19] Py：正则替换带回调
来源：http://wkv.jlsjyb.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tdp.fengsongda.top

[U20] Py：缓存函数结果
来源：http://cqg.ybcxt.top

@functools.lru_cache(maxsize=None)
来源：http://kvy.hesvh.cn

[U21] Py：自定义上下文管理器
来源：http://chy.hywenlv.cn

@contextlib.contextmanager
来源：http://yzf.nanxuanxn.top

[U22] Py：矩阵转置
来源：http://cyw.chenjidiqi.icu

list(zip(*m))
来源：http://ztd.pycfn.com

[U23] Py：分块读取大文件
来源：http://qmv.sysykeji.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://raj.jinyuanbaomall.cn

[U24] Py：路径操作
来源：http://zzs.snrcjt.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wyo.guowangkeji.top

[U25] Py：CSV 按字典读
来源：http://fkb.guowangkeji.top

csv.DictReader(f)
来源：http://urd.gogol.net.cn

[U26] Py：并发下载
来源：http://knq.jinghuilouyu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qkm.jinyuanbaomall.cn

[U27] Py：异步 HTTP
来源：http://vgu.pycfn.com

aiohttp.ClientSession() 配合 async with
来源：http://ptv.bjfxy.top

[U28] Py：类型别名
来源：http://cus.sufxvd.cn

UserId = int
来源：http://jrs.ybcxt.top

[U29] Py：属性校验
来源：http://lac.jiagoushi.top

@property 与 @x.setter 配合
来源：http://nyy.guannengcc.top

[U30] Py：数据类
来源：http://dfu.c1oappe.top

@dataclass(slots=True)
来源：http://sfl.chenlongwang.top

[U31] Py：单测
来源：http://iea.sjlbkw.cn

python -m pytest -q
来源：http://drk.jinqigfzy.top

[U32] Py：代码格式化
来源：http://gwm.kuanghao11.cn

ruff format . && ruff check --fix .
来源：http://qii.redwolf501.top

[U33] Py：打包发布
来源：http://kyd.shuidangran.top

python -m build  （依赖 pyproject.toml）
来源：http://wmr.chenzaomai.com

[U34] Py：判断编码
来源：http://dky.sjlbkw.cn

chardet.detect(raw)
来源：http://cjh.yonumen.top

[U35] Py：发送邮件
来源：http://yuj.hywenlv.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://orj.hcnkem.com

[U36] Py：定时任务
来源：http://ccc.hywenlv.cn

schedule.every(10).minutes.do(job)
来源：http://msi.xingfuxueyuan.xyz

[U37] Py：读写 Excel
来源：http://nqs.bjfxy.top

pandas.read_excel / DataFrame.to_excel
来源：http://sif.tanke756.top

[U38] Py：获取脚本所在目录
来源：http://wrg.hfpthk.cn

Path(__file__).resolve().parent
来源：http://ujx.tianlin.xyz

[U39] Py：判断是否在交互环境
来源：http://pph.hysaishi.cn

sys.stdout.isatty()
来源：http://jem.jlsjyb.cn

[U40] Py：打印到标准错误
来源：http://vcu.guowangkeji.top

print("err", file=sys.stderr)
来源：http://kbq.guannengcc.top

[U41] PHP：初始化 Composer 项目
来源：http://ieb.havefunace.top

composer init;  composer require guzzlehttp/guzzle
来源：http://uoj.yueranfly.top

[U42] PHP：PSR-4 自动加载
来源：http://paw.yj20258888.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gxx.zhengqikj.top

[U43] PHP：声明命名空间
来源：http://eac.yj202588.top

namespace App\Http;
来源：http://fvn.fktsv.cn

[U44] PHP：开启严格类型
来源：http://tdg.yongpay.top

declare(strict_types=1);
来源：http://bdj.yj202588.top

[U45] PHP：类型声明与返回类型
来源：http://zxk.zhiwuduotai.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://lxj.cucudq.cn

[U46] PHP：可空类型
来源：http://fpb.ydzc1.top

?string $name = null
来源：http://wef.hywenlv.cn

[U47] PHP：联合类型
来源：http://btl.yj20258888.top

int|string $id
来源：http://rof.9152youxi.cn

[U48] PHP：纯枚举
来源：http://xbn.havefunace.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://arh.hysaishi.cn

[U49] PHP：只读属性
来源：http://rme.hongshengwenyu.top

public readonly string $name
来源：http://qud.zhengqikj.top

[U50] PHP：构造器属性提升
来源：http://mfm.aizwys.cn

public function __construct(private int $id) {}
来源：http://pdi.meibo888.top

[U51] PHP：数组解构
来源：http://wgy.uphjek.com

[$a, $b] = $arr;
来源：http://gmh.yuanzhike.top

[U52] PHP：箭头函数
来源：http://ycs.aibaodan.cn

$double = fn($x) => $x * 2;
来源：http://cwo.hnqzz.top

[U53] PHP：空合并运算符
来源：http://tqq.aizwys.cn

$v = $a ?? $b ?? "default";
来源：http://rzr.hongshengwenyu.top

[U54] PHP：空安全调用
来源：http://otf.yueranfly.top

$obj?->method()
来源：http://smd.sxryk.cn

[U55] PHP：match 表达式
来源：http://mdg.yuxming.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wsc.316326.xyz

[U56] PHP：命名参数
来源：http://aij.shangyingyoupin.top

f(a: 1, b: 2)
来源：http://mnj.daxiang520.top

[U57] PHP：字符串插值
来源：http://mnh.jqgfzy.top

"值: {$a}"
来源：http://hbf.shuidangran.top

[U58] PHP：数组三件套
来源：http://ukq.ydjk.org.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hgj.zdqjudy.top

[U59] PHP：自定义排序
来源：http://jjy.daria6918.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ika.fktsv.cn

[U60] PHP：JSON 编解码
来源：http://ewh.hammf.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qwf.ehwqpu.com

[U61] PHP：正则
来源：http://tut.shuidangran.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://oey.jyoumei.cn

[U62] PHP：日期对象
来源：http://dut.fengsongda.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xow.xinyue.icu

[U63] PHP：文件读写
来源：http://vgs.chenjidiqi.icu

file_get_contents($f);  file_put_contents($f, $data);
来源：http://eqp.ehwqpu.com

[U64] PHP：目录遍历
来源：http://tdw.iojbl.cn

glob("dir/*.php");  scandir("dir");
来源：http://aba.shanyushiyangkeji.top

[U65] PHP：会话
来源：http://bzx.smart0.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://qyx.52xcode.cn

[U66] PHP：设置 Cookie
来源：http://hnb.yongpay.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xtx.mhx1999.top

[U67] PHP：处理文件上传
来源：http://rtm.daria6918.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://unl.redwolf501.top

[U68] PHP：PDO 连接
来源：http://szl.redwolf501.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pfp.fehbvm.com

[U69] PHP：PDO 预处理
来源：http://rng.andypj.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qcd.zhiwuduotai.top

[U70] PHP：PDO 事务
来源：http://udh.quarkkingdee.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://omo.fanxiaobao.xyz

[U71] PHP：抛出异常
来源：http://tvp.dashuyun.cn

throw new RuntimeException("失败", 500);
来源：http://fej.ctjpmb.com

[U72] PHP：写错误日志
来源：http://ckd.ehwqpu.com

error_log("失败: " . $e->getMessage());
来源：http://nwe.ppjwa.cn

[U73] PHP：读取 ini 配置
来源：http://yjz.zhiwuduotai.top

parse_ini_file("config.ini", true)
来源：http://tgf.haohaochexian.top

[U74] PHP：读取环境变量
来源：http://nye.xuanzx.com

getenv("APP_ENV") ?: "production"
来源：http://jno.ivvv.top

[U75] PHP：依赖注入
来源：http://czc.jinghuilouyu.cn

composer require psr/container
来源：http://yrw.sufxvd.cn

[U76] PHP：简单路由
来源：http://vzv.yanxiufei.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://nfv.jiagoushi.top

[U77] PHP：模板渲染
来源：http://axx.ybcxt.top

composer require twig/twig
来源：http://dek.ppjwa.cn

[U78] PHP：单元测试
来源：http://rba.nwbrower.top

composer require --dev phpunit/phpunit
来源：http://bxi.svipenyu.cn

[U79] PHP：静态分析
来源：http://oih.zhongyouzk.top

composer require --dev phpstan/phpstan
来源：http://hev.ppjwa.cn

[U80] PHP：代码规范修复
来源：http://skd.dashuyun.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://mol.ydzc1.top

[U81] JS：初始化项目
来源：http://ego.ppjwa.cn

npm init -y;  npm i express
来源：http://grm.nanxinkj.top

[U82] JS：package.json 脚本
来源：http://vae.ybcxt.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nxq.tianlin.xyz

[U83] JS：ES Module 导入导出
来源：http://iuz.jqgufenzy.top

export const a = 1;  import { a } from "./m.js";
来源：http://wfj.epnwcf.com

[U84] JS：CommonJS 写法
来源：http://hwy.zhengqikj.top

module.exports = { a };  const { a } = require("./m");
来源：http://oor.aibaodan.cn

[U85] JS：可选链
来源：http://mqw.hnxiangtu.top

a?.b?.c
来源：http://nff.zhaomingkeji.xyz

[U86] JS：空值合并
来源：http://ypo.shanyushiyangtech.top

a ?? b
来源：http://cll.ehwqpu.com

[U87] JS：解构默认值
来源：http://xgz.fanxiaobao.xyz

const { a = 1, b = 2 } = obj;
来源：http://ugc.sxryk.cn

[U88] JS：对象展开合并
来源：http://tjd.nwbrower.top

{ ...a, ...b }
来源：http://jee.ywan-chungtsiang.top

[U89] JS：数组去重
来源：http://gxu.vqdsnc.cn

[...new Set(arr)]
来源：http://myq.xingfuxueyuan.xyz

[U90] JS：数字数组排序
来源：http://rtw.fengsongda.top

[...arr].sort((a, b) => a - b)
来源：http://grr.zhixingplan.top

[U91] JS：对象键值遍历
来源：http://rty.gotoacloud.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://thd.cdnleiting.top

[U92] JS：深拷贝
来源：http://pgy.xuetiantiany.cn

structuredClone(obj)
来源：http://osu.guannengcc.top

[U93] JS：模板字符串
来源：http://qqp.yvedp.cn

`共 ${n} 条`
来源：http://dyx.daxiang520.top

[U94] JS：箭头函数
来源：http://nrl.hnxiangtu.top

const double = x => x * 2;
来源：http://kam.chenlongwang.top

[U95] JS：Promise 包装
来源：http://dse.pengpengdd.cyou

new Promise((resolve, reject) => {})
来源：http://cyc.c1oappe.top

[U96] JS：async/await 与异常
来源：http://mqj.aizwys.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vgb.meibo888.top

[U97] JS：并发请求
来源：http://unw.andypj.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://rgh.pycfn.com

[U98] JS：fetch 带 JSON
来源：http://qbg.nanxinkj.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://uvo.sweek.top

[U99] JS：事件监听
来源：http://mzd.haohaochexian.top

el.addEventListener("click", e => {})
来源：http://ecg.zdbjq.cn

[U100] JS：DOM 查询
来源：http://zab.fehbvm.com

document.querySelector(".item")
来源：http://ilk.fzhhl.top

[U101] JS：classList 操作
来源：http://kuu.aibaodan.cn

el.classList.toggle("active")
来源：http://vjw.zdbjq.cn

[U102] JS：本地存储
来源：http://dii.bjfxy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://xar.tianlin.xyz

[U103] JS：定时器
来源：http://ilt.mhx1999.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nwq.ydzc1.top

[U104] JS：防抖
来源：http://xqe.nwbrower.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aaj.yanxiufei.cn

[U105] JS：节流
来源：http://bhp.yongpay.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xws.yj20258888.top

[U106] JS：日期格式化
来源：http://cww.hnqzz.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vsc.zhiwuduotai.top

[U107] JS：数字千分位
来源：http://hrz.xuetiantiany.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://twb.epnwcf.com

[U108] JS：随机整数
来源：http://jqy.ivvv.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gxm.yanxiufei.cn

[U109] JS：数组分组
来源：http://jmr.cashguo.top

Object.groupBy(arr, x => x.type)
来源：http://goo.dianchejie.cn

[U110] JS：数组分块
来源：http://kws.zhiwuduotai.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fjt.ehwqpu.com

[U111] JS：对象转 Map
来源：http://ncd.andypj.xyz

new Map(Object.entries(obj))
来源：http://bmg.quarkkingdee.top

[U112] JS：字符串补位
来源：http://cym.zhoulong.xyz

"7".padStart(3, "0")
来源：http://yyn.hfpthk.cn

[U113] JS：正则替换全部
来源：http://baj.sxryk.cn

s.replaceAll("a", "b")
来源：http://bpx.snrcjt.cn

[U114] JS：JSON 深比较
来源：http://jqu.yongpay.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://njk.52xcode.cn

[U115] JS：生成 UUID
来源：http://wwo.fehbvm.com

crypto.randomUUID()
来源：http://sjv.cheryme.top

[U116] JS：类型检查（JSDoc）
来源：http://ogx.jiagoushi.top

/** @param {string} name */ function f(name) {}
来源：http://oib.yanxiufei.cn

[U117] JS：单元测试
来源：http://ueu.shuidangran.top

npm i -D vitest;  npx vitest
来源：http://lui.jiagoushi.top

[U118] JS：开发服务器
来源：http://jnw.ppjwa.cn

npm i -D vite;  npx vite
来源：http://qzo.svipenyu.cn

[U119] JS：生产构建
来源：http://ewl.cqqwz.cn

npx vite build
来源：http://wzz.jinqigfzy.top

[U120] JS：读取环境变量（Vite）
来源：http://sbu.xinyue.icu

import.meta.env.VITE_API_URL
来源：http://dpy.yanxiufei.cn

================================================================================
来源：http://lmu.fehbvm.com

统计汇总
来源：http://rxw.aizwys.cn

================================================================================
来源：http://yoi.sxryk.cn

按语言统计（条）：
来源：http://cdp.feifeiyinyue.top

Python ......... 252
来源：http://pyz.zhengqikj.top

PHP ............ 252
来源：http://zqg.yj202588.top

JavaScript ..... 252
来源：http://hnv.yongpay.top

TypeScript ..... 212
来源：http://nna.yj20258888.top

Java ........... 212
来源：http://ysx.hcnkem.com

Go ............. 212
来源：http://wql.jinqigfzy.top

Ruby ........... 212
来源：http://qfk.hysaishi.cn

C# ............. 212
来源：http://npz.fehbvm.com

C .............. 30
来源：http://thi.kuanghao11.cn

C++ ............ 30
来源：http://qkk.sufxvd.cn

SQL ............ 90
来源：http://rrh.gzhubu.top

Bash ........... 80
来源：http://lev.nanxinkj.top


<!-- 参考信息 -->