代发 wailian999

[T41] Perl：Hello World
来源：http://hak.birdmap.top

print "Hello\n";
来源：http://kgs.zdbjq.cn

[T42] Perl：变量类型
来源：http://vjl.jiagoushi.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fcs.xingfuxueyuan.xyz

[T43] Perl：字符串插值
来源：http://cfg.birdmap.top

"值: $a"
来源：http://ejs.cucudq.cn

[T44] Perl：条件
来源：http://wca.daxiang520.top

if ($a > 0) { print "正"; }
来源：http://mnc.yfazqb.com

[T45] Perl：数组遍历
来源：http://lbw.aizwys.cn

for my $x (@arr) { print $x; }
来源：http://lvx.gotoacloud.top

[T46] Perl：哈希操作
来源：http://rgc.dianchejie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fhy.chenlongwang.top

[T47] Perl：正则捕获
来源：http://wvi.hnqzz.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://zum.nanxinkj.top

[T48] Perl：正则替换
来源：http://eex.yanxiufei.cn

$s =~ s/old/new/g;
来源：http://ytc.ydjk.org.cn

[T49] Perl：函数
来源：http://ooz.shangyingyoupin.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://oab.havefunace.top

[T50] Perl：逐行读文件
来源：http://hmq.jiagoushi.top

open my $fh, "<", "a.txt" or die $!;
来源：http://mfz.fzhhl.top

while (my $line = <$fh>) { print $line; }
来源：http://bwt.birdmap.top

[T51] Scala：Hello World
来源：http://pje.xuanzx.com

println("Hello")
来源：http://vnk.chenjidiqi.icu

[T52] Scala：变量
来源：http://dwt.jianghu66.top

val a = 1;  var b = 2
来源：http://svd.bjfxy.top

[T53] Scala：字符串插值
来源：http://vtk.snrcjt.cn

s"值: $b"
来源：http://sfd.c1oappe.top

[T54] Scala：集合映射
来源：http://mcx.chenzaomai.com

List(1, 2, 3).map(_ * 2)
来源：http://ptf.jinqigufen.top

[T55] Scala：集合过滤
来源：http://szv.zdbjq.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ewo.yanxiufei.cn

[T56] Scala：样例类
来源：http://heh.jqgfzy.top

case class User(name: String, age: Int)
来源：http://ens.yj202588.top

[T57] Scala：模式匹配
来源：http://fya.zdqjudy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://sov.kuanghao11.cn

[T58] Scala：函数定义
来源：http://uux.smart0.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://sfg.yanxiufei.cn

[T59] Scala：循环
来源：http://dos.guowangkeji.top

for (i <- 1 to 10) println(i)
来源：http://gtl.gotoacloud.top

[T60] Scala：折叠
来源：http://yfc.shanyushiyangtech.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://kir.ehwqpu.com

================================================================================
来源：http://ibd.andypj.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ima.vqdsnc.cn

================================================================================
来源：http://zsm.andypj.xyz

[U01] Py：创建虚拟环境
来源：http://vgw.zhoulong.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://wrk.shanyushiyangkeji.top

[U02] Py：导出 / 安装依赖
来源：http://aaw.0kj1m.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ngi.andypj.xyz

[U03] Py：加载 .env 配置
来源：http://tlf.yanxiufei.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ovc.svipenyu.cn

[U04] Py：变量调试打印
来源：http://bav.ybcxt.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dld.mhx1999.top

[U05] Py：列表去重且保序
来源：http://msc.yuanzhike.top

list(dict.fromkeys(arr))
来源：http://tbj.xinyue.icu

[U06] Py：合并两个字典
来源：http://soh.gogol.net.cn

{**a, **b}
来源：http://usz.xylfe.cn

[U07] Py：反转字典键值
来源：http://kbp.havefunace.top

{v: k for k, v in d.items()}
来源：http://doq.ehwqpu.com

[U08] Py：展平二维列表
来源：http://itp.jinyuanbaomall.cn

[y for x in nested for y in x]
来源：http://uxv.zhongyouzk.top

[U09] Py：字典取最大值的键
来源：http://jas.fanxiaobao.xyz

max(d, key=d.get)
来源：http://kue.hnqzz.top

[U10] Py：按值排序字典
来源：http://csu.jinghuilouyu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uia.xinyue.icu

[U11] Py：生成器表达式
来源：http://way.nanxuanxn.top

(x * 2 for x in arr)
来源：http://sxf.uphjek.com

[U12] Py：取出现最多的 3 个元素
来源：http://cvk.chenzaomai.com

Counter(arr).most_common(3)
来源：http://wnh.chenlongwang.top

[U13] Py：固定长度队列
来源：http://mwb.meibo888.top

deque(maxlen=10)
来源：http://ylo.aibaodan.cn

[U14] Py：分组收集到列表
来源：http://nrt.hywenlv.cn

defaultdict(list)
来源：http://tke.dianchejie.cn

[U15] Py：高精度计时
来源：http://viq.nanxuanxn.top

t = time.perf_counter()
来源：http://ihn.cheryme.top

[U16] Py：命令行参数解析
来源：http://wqf.aibaodan.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pdc.jinqigfzy.top

[U17] Py：初始化日志
来源：http://yti.birdmap.top

logging.basicConfig(level=logging.INFO)
来源：http://dhc.sxryk.cn

[U18] Py：预编译正则
来源：http://asr.wangshuangyany.cn

pat = re.compile(r"\d+")
来源：http://zxm.bbcook.cn

[U19] Py：正则替换带回调
来源：http://vtt.zhoulong.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ath.chenzaomai.com

[U20] Py：缓存函数结果
来源：http://uwv.uphjek.com

@functools.lru_cache(maxsize=None)
来源：http://vog.zdbjq.cn

[U21] Py：自定义上下文管理器
来源：http://smb.yangfankeji.com

@contextlib.contextmanager
来源：http://uav.zhengqikj.top

[U22] Py：矩阵转置
来源：http://gwf.daxiang520.top

list(zip(*m))
来源：http://xxm.hcnkem.com

[U23] Py：分块读取大文件
来源：http://oex.wangshuangyany.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hhj.gogol.net.cn

[U24] Py：路径操作
来源：http://fnw.vqdsnc.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://osh.yuanzhike.top

[U25] Py：CSV 按字典读
来源：http://tsu.pengpengdd.cyou

csv.DictReader(f)
来源：http://fmj.snrcjt.cn

[U26] Py：并发下载
来源：http://wsf.wangdashe.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qii.ydjk.org.cn

[U27] Py：异步 HTTP
来源：http://qxi.yonumen.top

aiohttp.ClientSession() 配合 async with
来源：http://bfv.fktsv.cn

[U28] Py：类型别名
来源：http://tge.nanxinkj.top

UserId = int
来源：http://eai.feifeiyinyue.top

[U29] Py：属性校验
来源：http://cty.shangyingyoupin.top

@property 与 @x.setter 配合
来源：http://pnz.zhengqikj.top

[U30] Py：数据类
来源：http://wcw.sweek.top

@dataclass(slots=True)
来源：http://fxo.jlsjyb.cn

[U31] Py：单测
来源：http://owe.shzxlz.cn

python -m pytest -q
来源：http://ssc.daria6918.cn

[U32] Py：代码格式化
来源：http://jym.tianlin.xyz

ruff format . && ruff check --fix .
来源：http://xjz.wangdashe.top

[U33] Py：打包发布
来源：http://wwv.hywenlv.cn

python -m build  （依赖 pyproject.toml）
来源：http://jnj.nwbrower.top

[U34] Py：判断编码
来源：http://rgc.jianghu66.top

chardet.detect(raw)
来源：http://pwe.cheryme.top

[U35] Py：发送邮件
来源：http://cfp.sufxvd.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://uwv.fanxiaobao.xyz

[U36] Py：定时任务
来源：http://doe.jianghu66.top

schedule.every(10).minutes.do(job)
来源：http://ryn.yj202588.top

[U37] Py：读写 Excel
来源：http://mat.snrcjt.cn

pandas.read_excel / DataFrame.to_excel
来源：http://avb.dianchejie.cn

[U38] Py：获取脚本所在目录
来源：http://cto.yfazqb.com

Path(__file__).resolve().parent
来源：http://iem.zhiwuduotai.top

[U39] Py：判断是否在交互环境
来源：http://ghb.yj202588.top

sys.stdout.isatty()
来源：http://mqk.zhoulong.xyz

[U40] Py：打印到标准错误
来源：http://urq.daxiang520.top

print("err", file=sys.stderr)
来源：http://tzy.epnwcf.com

[U41] PHP：初始化 Composer 项目
来源：http://cjo.yongpay.top

composer init;  composer require guzzlehttp/guzzle
来源：http://jhp.aibaodan.cn

[U42] PHP：PSR-4 自动加载
来源：http://npx.zhiwuduotai.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://oga.hcnkem.com

[U43] PHP：声明命名空间
来源：http://tzz.xinyue.icu

namespace App\Http;
来源：http://rek.bbcook.cn

[U44] PHP：开启严格类型
来源：http://dfr.yj20258888.top

declare(strict_types=1);
来源：http://ijz.pycfn.com

[U45] PHP：类型声明与返回类型
来源：http://xyn.nwbrower.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://zok.yj202588.top

[U46] PHP：可空类型
来源：http://nsq.cqqwz.cn

?string $name = null
来源：http://cqd.yj20258.top

[U47] PHP：联合类型
来源：http://oek.hywenlv.cn

int|string $id
来源：http://pkw.jianghu66.top

[U48] PHP：纯枚举
来源：http://yzh.bjfxy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://fab.meibo888.top

[U49] PHP：只读属性
来源：http://rpc.zhaomingkeji.xyz

public readonly string $name
来源：http://lra.birdmap.top

[U50] PHP：构造器属性提升
来源：http://gxi.guannengcc.top

public function __construct(private int $id) {}
来源：http://unh.shuidangran.top

[U51] PHP：数组解构
来源：http://lky.zhiwuduotai.top

[$a, $b] = $arr;
来源：http://vwm.dianchejie.cn

[U52] PHP：箭头函数
来源：http://eat.jinqigufen.top

$double = fn($x) => $x * 2;
来源：http://uvc.bjfxy.top

[U53] PHP：空合并运算符
来源：http://zss.xylfe.cn

$v = $a ?? $b ?? "default";
来源：http://tyj.hfpthk.cn

[U54] PHP：空安全调用
来源：http://wos.jinghuilouyu.cn

$obj?->method()
来源：http://kwv.ydzc1.top

[U55] PHP：match 表达式
来源：http://spj.ybcxt.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zbp.cheryme.top

[U56] PHP：命名参数
来源：http://ahk.sjlbkw.cn

f(a: 1, b: 2)
来源：http://mjh.hesvh.cn

[U57] PHP：字符串插值
来源：http://xwf.bbcook.cn

"值: {$a}"
来源：http://ugo.gotoacloud.top

[U58] PHP：数组三件套
来源：http://pjp.kuanghao11.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nlb.mhx1999.top

[U59] PHP：自定义排序
来源：http://cey.cqqwz.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://koc.9152youxi.cn

[U60] PHP：JSON 编解码
来源：http://gun.gzhubu.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ytj.xuanzx.com

[U61] PHP：正则
来源：http://biu.jlsjyb.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bpo.ydzc1.top

[U62] PHP：日期对象
来源：http://naj.jinqigufen.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fho.gzhubu.top

[U63] PHP：文件读写
来源：http://knt.shanyushiyangtech.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://akm.chenjidiqi.icu

[U64] PHP：目录遍历
来源：http://obu.quarkkingdee.top

glob("dir/*.php");  scandir("dir");
来源：http://ebh.fzhhl.top

[U65] PHP：会话
来源：http://mzs.xuanzx.com

session_start();  $_SESSION["uid"] = 1;
来源：http://woh.daria6918.cn

[U66] PHP：设置 Cookie
来源：http://jgm.gzhubu.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bcw.xingfuxueyuan.xyz

[U67] PHP：处理文件上传
来源：http://riz.shanyushiyangtech.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hii.guannengcc.top

[U68] PHP：PDO 连接
来源：http://yjc.nanxinkj.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://itx.uphjek.com

[U69] PHP：PDO 预处理
来源：http://wul.ybcxt.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://iis.52xcode.cn

[U70] PHP：PDO 事务
来源：http://csg.nanxuanxn.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fsn.shangyingyoupin.top

[U71] PHP：抛出异常
来源：http://igx.bbcook.cn

throw new RuntimeException("失败", 500);
来源：http://gek.uphjek.com

[U72] PHP：写错误日志
来源：http://sqe.jqgfzy.top

error_log("失败: " . $e->getMessage());
来源：http://hnn.zhongyouzk.top

[U73] PHP：读取 ini 配置
来源：http://gre.chenzaomai.com

parse_ini_file("config.ini", true)
来源：http://lpc.jinqigfzy.top

[U74] PHP：读取环境变量
来源：http://rmk.yuanzhike.top

getenv("APP_ENV") ?: "production"
来源：http://rzt.bbcook.cn

[U75] PHP：依赖注入
来源：http://uvc.zhijiandao.cn

composer require psr/container
来源：http://xpv.yuanzhike.top

[U76] PHP：简单路由
来源：http://via.ctjpmb.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vnu.c1oappe.top

[U77] PHP：模板渲染
来源：http://mai.tianlin.xyz

composer require twig/twig
来源：http://dgp.hywenlv.cn

[U78] PHP：单元测试
来源：http://xgj.gogol.net.cn

composer require --dev phpunit/phpunit
来源：http://rln.cdnleiting.top

[U79] PHP：静态分析
来源：http://ggw.zdbjq.cn

composer require --dev phpstan/phpstan
来源：http://gaz.cdnleiting.top

[U80] PHP：代码规范修复
来源：http://jqh.zhijiandao.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://mcb.bbcook.cn

[U81] JS：初始化项目
来源：http://wjl.quarkkingdee.top

npm init -y;  npm i express
来源：http://ixu.316326.xyz

[U82] JS：package.json 脚本
来源：http://ltt.yongpay.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zwi.shzxlz.cn

[U83] JS：ES Module 导入导出
来源：http://olp.hammf.cn

export const a = 1;  import { a } from "./m.js";
来源：http://gix.nwbrower.top

[U84] JS：CommonJS 写法
来源：http://ffn.zhiwuduotai.top

module.exports = { a };  const { a } = require("./m");
来源：http://jbu.ydzc1.top

[U85] JS：可选链
来源：http://wko.jqgfzy.top

a?.b?.c
来源：http://lay.yj20258.top

[U86] JS：空值合并
来源：http://spk.guannengcc.top

a ?? b
来源：http://zqz.xingfuxueyuan.xyz

[U87] JS：解构默认值
来源：http://clw.tanke756.top

const { a = 1, b = 2 } = obj;
来源：http://zdr.fanxiaobao.xyz

[U88] JS：对象展开合并
来源：http://dka.yfazqb.com

{ ...a, ...b }
来源：http://mzl.wangshuangyany.cn

[U89] JS：数组去重
来源：http://wpi.tanke756.top

[...new Set(arr)]
来源：http://lqw.jinqigfzy.top

[U90] JS：数字数组排序
来源：http://fwf.redwolf501.top

[...arr].sort((a, b) => a - b)
来源：http://nnc.uphjek.com

[U91] JS：对象键值遍历
来源：http://egs.bbcook.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fjl.xylfe.cn

[U92] JS：深拷贝
来源：http://dla.yonumen.top

structuredClone(obj)
来源：http://ite.hnqzz.top

[U93] JS：模板字符串
来源：http://vdr.meibo888.top

`共 ${n} 条`
来源：http://hvw.dianchejie.cn

[U94] JS：箭头函数
来源：http://vft.yvedp.cn

const double = x => x * 2;
来源：http://ozf.zdbjq.cn

[U95] JS：Promise 包装
来源：http://fvg.guowangkeji.top

new Promise((resolve, reject) => {})
来源：http://nzj.52xcode.cn

[U96] JS：async/await 与异常
来源：http://npo.fehbvm.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lcj.hcnkem.com

[U97] JS：并发请求
来源：http://wdr.yueranfly.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://akq.zhoulong.xyz

[U98] JS：fetch 带 JSON
来源：http://ehp.hcnkem.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fnt.c1oappe.top

[U99] JS：事件监听
来源：http://una.iojbl.cn

el.addEventListener("click", e => {})
来源：http://phi.jinyuanbaomall.cn

[U100] JS：DOM 查询
来源：http://epu.shuidangran.top

document.querySelector(".item")
来源：http://rhk.52xcode.cn

[U101] JS：classList 操作
来源：http://mvr.shangyingyoupin.top

el.classList.toggle("active")
来源：http://wfi.zhengqikj.top

[U102] JS：本地存储
来源：http://gmg.iojbl.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://gex.sufxvd.cn

[U103] JS：定时器
来源：http://dvk.chenzaomai.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://irh.zdbjq.cn

[U104] JS：防抖
来源：http://dmf.havefunace.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wyy.ctjpmb.com

[U105] JS：节流
来源：http://jsg.pycfn.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://tub.hysaishi.cn

[U106] JS：日期格式化
来源：http://pjq.hywenlv.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gta.aibaodan.cn

[U107] JS：数字千分位
来源：http://rqi.bbcook.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mti.zhijiandao.cn

[U108] JS：随机整数
来源：http://tpn.pycfn.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://eng.fzhhl.top

[U109] JS：数组分组
来源：http://sml.hfpthk.cn

Object.groupBy(arr, x => x.type)
来源：http://moe.ppjwa.cn

[U110] JS：数组分块
来源：http://baf.ybcxt.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rnx.hammf.cn

[U111] JS：对象转 Map
来源：http://uxy.andypj.xyz

new Map(Object.entries(obj))
来源：http://fko.chenlongwang.top

[U112] JS：字符串补位
来源：http://wce.feifeiyinyue.top

"7".padStart(3, "0")
来源：http://byo.jinghuilouyu.cn

[U113] JS：正则替换全部
来源：http://gdb.bbcook.cn

s.replaceAll("a", "b")
来源：http://pry.haohaochexian.top

[U114] JS：JSON 深比较
来源：http://uqe.guowangkeji.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://etm.bbcook.cn

[U115] JS：生成 UUID
来源：http://ifn.fanxiaobao.xyz

crypto.randomUUID()
来源：http://kkq.xingfuxueyuan.xyz

[U116] JS：类型检查（JSDoc）
来源：http://ory.kuanghao11.cn

/** @param {string} name */ function f(name) {}
来源：http://nis.mhx1999.top

[U117] JS：单元测试
来源：http://yoh.snrcjt.cn

npm i -D vitest;  npx vitest
来源：http://lon.ywan-chungtsiang.top

[U118] JS：开发服务器
来源：http://npu.nanxuanxn.top

npm i -D vite;  npx vite
来源：http://dlr.pengpengdd.cyou

[U119] JS：生产构建
来源：http://tox.uphjek.com

npx vite build
来源：http://fkv.ywan-chungtsiang.top

[U120] JS：读取环境变量（Vite）
来源：http://gjo.bbcook.cn

import.meta.env.VITE_API_URL
来源：http://lhg.daxiang520.top

================================================================================
来源：http://zjj.daria6918.cn

统计汇总
来源：http://thn.yueranfly.top

================================================================================
来源：http://htx.jqgfzy.top

按语言统计（条）：
来源：http://xsn.jianghu66.top

Python ......... 252
来源：http://uzb.zdbjq.cn

PHP ............ 252
来源：http://xel.svipenyu.cn

JavaScript ..... 252
来源：http://knc.jinyuanbaomall.cn

TypeScript ..... 212
来源：http://dvy.ydjk.org.cn

Java ........... 212
来源：http://wnt.zdbjq.cn

Go ............. 212
来源：http://qii.chenzaomai.com

Ruby ........... 212
来源：http://bvs.xingfuxueyuan.xyz

C# ............. 212
来源：http://uoi.sweek.top

C .............. 30
来源：http://giw.bjfxy.top

C++ ............ 30
来源：http://vot.cucudq.cn

SQL ............ 90
来源：http://gev.cashguo.top

Bash ........... 80
来源：http://rxd.dashuyun.cn


<!-- 参考信息 -->