代发 wailian999

[T41] Perl：Hello World
来源：http://xlv.fktsv.cn

print "Hello\n";
来源：http://uvg.yanxiufei.cn

[T42] Perl：变量类型
来源：http://pkw.shangyingyoupin.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dkl.ywan-chungtsiang.top

[T43] Perl：字符串插值
来源：http://hnn.zhoulong.xyz

"值: $a"
来源：http://ifw.cucudq.cn

[T44] Perl：条件
来源：http://lea.mhx1999.top

if ($a > 0) { print "正"; }
来源：http://ycb.hongshengwenyu.top

[T45] Perl：数组遍历
来源：http://hdr.pengpengdd.cyou

for my $x (@arr) { print $x; }
来源：http://kgw.dianchejie.cn

[T46] Perl：哈希操作
来源：http://oav.zdqjudy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lye.yvedp.cn

[T47] Perl：正则捕获
来源：http://inc.tarul.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://koo.vehdjk.com

[T48] Perl：正则替换
来源：http://vdx.quarkkingdee.top

$s =~ s/old/new/g;
来源：http://ank.chenjidiqi.icu

[T49] Perl：函数
来源：http://uok.zdbjq.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ozy.yangfankeji.com

[T50] Perl：逐行读文件
来源：http://odc.cucudq.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://wsw.jqgfzy.top

while (my $line = <$fh>) { print $line; }
来源：http://gdx.gzhubu.top

[T51] Scala：Hello World
来源：http://oly.ydzc1.top

println("Hello")
来源：http://yuo.svipenyu.cn

[T52] Scala：变量
来源：http://fck.52xcode.cn

val a = 1;  var b = 2
来源：http://pce.fzhhl.top

[T53] Scala：字符串插值
来源：http://tak.jlsjyb.cn

s"值: $b"
来源：http://foo.chenlongwang.top

[T54] Scala：集合映射
来源：http://xmk.dashuyun.cn

List(1, 2, 3).map(_ * 2)
来源：http://jte.ydzc1.top

[T55] Scala：集合过滤
来源：http://naq.redwolf501.top

List(1, 2, 3).filter(_ > 1)
来源：http://vrs.zdqjudy.top

[T56] Scala：样例类
来源：http://fxk.wangshuangyany.cn

case class User(name: String, age: Int)
来源：http://qij.jqgufenzy.top

[T57] Scala：模式匹配
来源：http://tys.yj20258.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://slg.quarkkingdee.top

[T58] Scala：函数定义
来源：http://ptk.daria6918.cn

def add(a: Int, b: Int): Int = a + b
来源：http://srp.tarul.cn

[T59] Scala：循环
来源：http://wcy.jlsjyb.cn

for (i <- 1 to 10) println(i)
来源：http://mzd.xziqi.cn

[T60] Scala：折叠
来源：http://bpk.xylfe.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mru.gzhubu.top

================================================================================
来源：http://cds.guannengcc.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kna.pengpengdd.cyou

================================================================================
来源：http://qag.wangshuangyany.cn

[U01] Py：创建虚拟环境
来源：http://vjs.jqgufenzy.top

python -m venv .venv && source .venv/bin/activate
来源：http://tdv.gogol.net.cn

[U02] Py：导出 / 安装依赖
来源：http://dtk.nanxinkj.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://omd.cdnleiting.top

[U03] Py：加载 .env 配置
来源：http://fak.sweek.top

from dotenv import load_dotenv; load_dotenv()
来源：http://dnc.hysaishi.cn

[U04] Py：变量调试打印
来源：http://iwo.cashguo.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://sqt.zycfv.cn

[U05] Py：列表去重且保序
来源：http://vvg.zycfv.cn

list(dict.fromkeys(arr))
来源：http://dvv.yj20258.top

[U06] Py：合并两个字典
来源：http://oni.ydzc1.top

{**a, **b}
来源：http://khc.hammf.cn

[U07] Py：反转字典键值
来源：http://igf.zhoulong.xyz

{v: k for k, v in d.items()}
来源：http://iuw.fengsongda.top

[U08] Py：展平二维列表
来源：http://eum.daria6918.cn

[y for x in nested for y in x]
来源：http://bcm.nanxuanxn.top

[U09] Py：字典取最大值的键
来源：http://rkj.shangyingyoupin.top

max(d, key=d.get)
来源：http://wlj.jinqigfzy.top

[U10] Py：按值排序字典
来源：http://xad.jinghuilouyu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://piy.zhoulong.xyz

[U11] Py：生成器表达式
来源：http://whl.ybcxt.top

(x * 2 for x in arr)
来源：http://ozp.vqdsnc.cn

[U12] Py：取出现最多的 3 个元素
来源：http://fso.ivvv.top

Counter(arr).most_common(3)
来源：http://cfg.xylfe.cn

[U13] Py：固定长度队列
来源：http://kwn.yvedp.cn

deque(maxlen=10)
来源：http://bnr.hysaishi.cn

[U14] Py：分组收集到列表
来源：http://wyu.yongpay.top

defaultdict(list)
来源：http://xrt.shuidangran.top

[U15] Py：高精度计时
来源：http://fze.snrcjt.cn

t = time.perf_counter()
来源：http://enf.kuanghao11.cn

[U16] Py：命令行参数解析
来源：http://hew.zhoulong.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://urk.kuanghao11.cn

[U17] Py：初始化日志
来源：http://kza.quarkkingdee.top

logging.basicConfig(level=logging.INFO)
来源：http://avr.zhaomingkeji.xyz

[U18] Py：预编译正则
来源：http://apa.zhongyouzk.top

pat = re.compile(r"\d+")
来源：http://rrc.hysaishi.cn

[U19] Py：正则替换带回调
来源：http://rzx.xingfuxueyuan.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://oan.bjfxy.top

[U20] Py：缓存函数结果
来源：http://pnj.iojbl.cn

@functools.lru_cache(maxsize=None)
来源：http://vpx.yj20258888.top

[U21] Py：自定义上下文管理器
来源：http://nip.hysaishi.cn

@contextlib.contextmanager
来源：http://rsc.yfazqb.com

[U22] Py：矩阵转置
来源：http://toi.jlsjyb.cn

list(zip(*m))
来源：http://gzc.yongpay.top

[U23] Py：分块读取大文件
来源：http://mtl.tian-w.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vun.aizwys.cn

[U24] Py：路径操作
来源：http://kig.fzhhl.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tpg.zhijiandao.cn

[U25] Py：CSV 按字典读
来源：http://dap.uphjek.com

csv.DictReader(f)
来源：http://lvq.jinqigfzy.top

[U26] Py：并发下载
来源：http://ewi.cdnleiting.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pks.nanxuanxn.top

[U27] Py：异步 HTTP
来源：http://ohn.yanxiufei.cn

aiohttp.ClientSession() 配合 async with
来源：http://rax.jqgfzy.top

[U28] Py：类型别名
来源：http://cfv.316326.xyz

UserId = int
来源：http://nyu.gaohongyu789.top

[U29] Py：属性校验
来源：http://sbp.pengpengdd.cyou

@property 与 @x.setter 配合
来源：http://ioa.guannengcc.top

[U30] Py：数据类
来源：http://tfu.xuanzx.com

@dataclass(slots=True)
来源：http://zlz.zhixingplan.top

[U31] Py：单测
来源：http://qbb.yanxiufei.cn

python -m pytest -q
来源：http://bdo.tianlin.xyz

[U32] Py：代码格式化
来源：http://xnk.yanxiufei.cn

ruff format . && ruff check --fix .
来源：http://lqd.dianchejie.cn

[U33] Py：打包发布
来源：http://cxs.pengpengdd.cyou

python -m build  （依赖 pyproject.toml）
来源：http://vch.xinyue.icu

[U34] Py：判断编码
来源：http://sfl.hcnkem.com

chardet.detect(raw)
来源：http://lqx.jiagoushi.top

[U35] Py：发送邮件
来源：http://phl.jyoumei.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://sys.cucudq.cn

[U36] Py：定时任务
来源：http://ovd.mhx1999.top

schedule.every(10).minutes.do(job)
来源：http://qnv.sysykeji.top

[U37] Py：读写 Excel
来源：http://zdg.hywenlv.cn

pandas.read_excel / DataFrame.to_excel
来源：http://lqo.bbcook.cn

[U38] Py：获取脚本所在目录
来源：http://urh.nwbrower.top

Path(__file__).resolve().parent
来源：http://nlt.ybcxt.top

[U39] Py：判断是否在交互环境
来源：http://xwk.52xcode.cn

sys.stdout.isatty()
来源：http://ges.fzhhl.top

[U40] Py：打印到标准错误
来源：http://vou.yj20258.top

print("err", file=sys.stderr)
来源：http://blg.tanke756.top

[U41] PHP：初始化 Composer 项目
来源：http://gbp.shangyingyoupin.top

composer init;  composer require guzzlehttp/guzzle
来源：http://zej.zhixingplan.top

[U42] PHP：PSR-4 自动加载
来源：http://ont.yuxming.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://add.tianlin.xyz

[U43] PHP：声明命名空间
来源：http://pvs.xuetiantiany.cn

namespace App\Http;
来源：http://shh.zhongyouzk.top

[U44] PHP：开启严格类型
来源：http://udo.nanxuanxn.top

declare(strict_types=1);
来源：http://xbu.cdnleiting.top

[U45] PHP：类型声明与返回类型
来源：http://ndu.iojbl.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://jml.guannengcc.top

[U46] PHP：可空类型
来源：http://ppj.kuanghao11.cn

?string $name = null
来源：http://tvk.sweek.top

[U47] PHP：联合类型
来源：http://oyr.zhoulong.xyz

int|string $id
来源：http://hjn.kuanghao11.cn

[U48] PHP：纯枚举
来源：http://man.zhaomingkeji.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://yii.fengsongda.top

[U49] PHP：只读属性
来源：http://cfn.shanyushiyangtech.top

public readonly string $name
来源：http://aqw.svipenyu.cn

[U50] PHP：构造器属性提升
来源：http://pqo.zdbjq.cn

public function __construct(private int $id) {}
来源：http://xon.iojbl.cn

[U51] PHP：数组解构
来源：http://tpy.fktsv.cn

[$a, $b] = $arr;
来源：http://rng.cqqwz.cn

[U52] PHP：箭头函数
来源：http://tcq.aibaodan.cn

$double = fn($x) => $x * 2;
来源：http://pat.hysaishi.cn

[U53] PHP：空合并运算符
来源：http://hmt.cqqwz.cn

$v = $a ?? $b ?? "default";
来源：http://fon.yj20258888.top

[U54] PHP：空安全调用
来源：http://emb.52xcode.cn

$obj?->method()
来源：http://nwg.sufxvd.cn

[U55] PHP：match 表达式
来源：http://mye.yj20258888.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kcb.jiagoushi.top

[U56] PHP：命名参数
来源：http://psl.sufxvd.cn

f(a: 1, b: 2)
来源：http://eyx.quarkkingdee.top

[U57] PHP：字符串插值
来源：http://hib.sysykeji.top

"值: {$a}"
来源：http://yfy.meibo888.top

[U58] PHP：数组三件套
来源：http://ztj.aizwys.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wrl.wangdashe.top

[U59] PHP：自定义排序
来源：http://mca.sweek.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bvy.xylfe.cn

[U60] PHP：JSON 编解码
来源：http://olo.daxiang520.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://amt.uphjek.com

[U61] PHP：正则
来源：http://gbz.iojbl.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kkw.fengsongda.top

[U62] PHP：日期对象
来源：http://jdc.jqgfzy.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jqy.ehwqpu.com

[U63] PHP：文件读写
来源：http://kzy.zhaomingkeji.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://sqn.jinqigfzy.top

[U64] PHP：目录遍历
来源：http://dio.ehwqpu.com

glob("dir/*.php");  scandir("dir");
来源：http://jkf.epnwcf.com

[U65] PHP：会话
来源：http://qdg.zhiwuduotai.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ikz.epnwcf.com

[U66] PHP：设置 Cookie
来源：http://fbg.yonumen.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://lel.cashguo.top

[U67] PHP：处理文件上传
来源：http://mws.chenlongwang.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://epc.yuanzhike.top

[U68] PHP：PDO 连接
来源：http://zmx.nanxinkj.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hct.xinyue.icu

[U69] PHP：PDO 预处理
来源：http://ggt.yfazqb.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yqv.zhaomingkeji.xyz

[U70] PHP：PDO 事务
来源：http://yuz.aibaodan.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ddu.yfazqb.com

[U71] PHP：抛出异常
来源：http://ufj.havefunace.top

throw new RuntimeException("失败", 500);
来源：http://oub.hammf.cn

[U72] PHP：写错误日志
来源：http://pvq.yfazqb.com

error_log("失败: " . $e->getMessage());
来源：http://fzn.fktsv.cn

[U73] PHP：读取 ini 配置
来源：http://qsy.fzhhl.top

parse_ini_file("config.ini", true)
来源：http://qbx.smart0.xyz

[U74] PHP：读取环境变量
来源：http://kah.guowangkeji.top

getenv("APP_ENV") ?: "production"
来源：http://wgr.mhx1999.top

[U75] PHP：依赖注入
来源：http://buh.sxryk.cn

composer require psr/container
来源：http://nzv.yonumen.top

[U76] PHP：简单路由
来源：http://srk.cashguo.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lms.xylfe.cn

[U77] PHP：模板渲染
来源：http://gjy.xuetiantiany.cn

composer require twig/twig
来源：http://mbj.shuidangran.top

[U78] PHP：单元测试
来源：http://rqj.iojbl.cn

composer require --dev phpunit/phpunit
来源：http://hxr.sjlbkw.cn

[U79] PHP：静态分析
来源：http://kuh.zycfv.cn

composer require --dev phpstan/phpstan
来源：http://tmr.jianghu66.top

[U80] PHP：代码规范修复
来源：http://sgi.zhoulong.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://vmq.fktsv.cn

[U81] JS：初始化项目
来源：http://wyi.daxiang520.top

npm init -y;  npm i express
来源：http://upo.hnxiangtu.top

[U82] JS：package.json 脚本
来源：http://ddh.meibo888.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vlx.chenlongwang.top

[U83] JS：ES Module 导入导出
来源：http://zvy.hysaishi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://qpn.xingfuxueyuan.xyz

[U84] JS：CommonJS 写法
来源：http://kkb.fktsv.cn

module.exports = { a };  const { a } = require("./m");
来源：http://paj.c1oappe.top

[U85] JS：可选链
来源：http://rki.epnwcf.com

a?.b?.c
来源：http://ctw.ivvv.top

[U86] JS：空值合并
来源：http://soc.fktsv.cn

a ?? b
来源：http://qbc.gogol.net.cn

[U87] JS：解构默认值
来源：http://vkw.uphjek.com

const { a = 1, b = 2 } = obj;
来源：http://olb.quarkkingdee.top

[U88] JS：对象展开合并
来源：http://awv.haohaochexian.top

{ ...a, ...b }
来源：http://fsf.snrcjt.cn

[U89] JS：数组去重
来源：http://hhq.jlsjyb.cn

[...new Set(arr)]
来源：http://eig.svipenyu.cn

[U90] JS：数字数组排序
来源：http://lni.cqqwz.cn

[...arr].sort((a, b) => a - b)
来源：http://zfk.xuetiantiany.cn

[U91] JS：对象键值遍历
来源：http://hjc.yanxiufei.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://thf.epnwcf.com

[U92] JS：深拷贝
来源：http://zsh.52xcode.cn

structuredClone(obj)
来源：http://cui.pengpengdd.cyou

[U93] JS：模板字符串
来源：http://ras.guowangkeji.top

`共 ${n} 条`
来源：http://deg.pycfn.com

[U94] JS：箭头函数
来源：http://hgu.yonumen.top

const double = x => x * 2;
来源：http://gjj.cqqwz.cn

[U95] JS：Promise 包装
来源：http://hag.jinyuanbaomall.cn

new Promise((resolve, reject) => {})
来源：http://czm.jinqigufen.top

[U96] JS：async/await 与异常
来源：http://ivw.feifeiyinyue.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jgr.mhx1999.top

[U97] JS：并发请求
来源：http://did.jiagoushi.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://hjp.zhengqikj.top

[U98] JS：fetch 带 JSON
来源：http://xqu.zycfv.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://iej.meibo888.top

[U99] JS：事件监听
来源：http://flr.sweek.top

el.addEventListener("click", e => {})
来源：http://kxn.guannengcc.top

[U100] JS：DOM 查询
来源：http://skk.316326.xyz

document.querySelector(".item")
来源：http://rkf.gzhubu.top

[U101] JS：classList 操作
来源：http://dxu.xingfuxueyuan.xyz

el.classList.toggle("active")
来源：http://klj.feifeiyinyue.top

[U102] JS：本地存储
来源：http://ynh.yj202588.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://pxm.aibaodan.cn

[U103] JS：定时器
来源：http://scz.hysaishi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qbh.daria6918.cn

[U104] JS：防抖
来源：http://oai.yj20258.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vdq.jqgufenzy.top

[U105] JS：节流
来源：http://cdw.zdqjudy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qgu.fengsongda.top

[U106] JS：日期格式化
来源：http://csr.ybcxt.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bqu.tarul.cn

[U107] JS：数字千分位
来源：http://cug.aizwys.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pqk.shzxlz.cn

[U108] JS：随机整数
来源：http://exl.yanxiufei.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://yos.cucudq.cn

[U109] JS：数组分组
来源：http://zna.ydzc1.top

Object.groupBy(arr, x => x.type)
来源：http://oha.hfpthk.cn

[U110] JS：数组分块
来源：http://prh.sufxvd.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tsj.tianlin.xyz

[U111] JS：对象转 Map
来源：http://zpp.zycfv.cn

new Map(Object.entries(obj))
来源：http://xfk.shanyushiyangtech.top

[U112] JS：字符串补位
来源：http://bob.mhx1999.top

"7".padStart(3, "0")
来源：http://fnu.birdmap.top

[U113] JS：正则替换全部
来源：http://mip.shangyingyoupin.top

s.replaceAll("a", "b")
来源：http://iev.iojbl.cn

[U114] JS：JSON 深比较
来源：http://nwy.iojbl.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://hwh.hfpthk.cn

[U115] JS：生成 UUID
来源：http://yea.hesvh.cn

crypto.randomUUID()
来源：http://zkn.chenjidiqi.icu

[U116] JS：类型检查（JSDoc）
来源：http://dxe.hesvh.cn

/** @param {string} name */ function f(name) {}
来源：http://pll.meibo888.top

[U117] JS：单元测试
来源：http://vgy.wangdashe.top

npm i -D vitest;  npx vitest
来源：http://gmh.fktsv.cn

[U118] JS：开发服务器
来源：http://see.yuanzhike.top

npm i -D vite;  npx vite
来源：http://ekl.guannengcc.top

[U119] JS：生产构建
来源：http://lyh.snrcjt.cn

npx vite build
来源：http://dbd.sxryk.cn

[U120] JS：读取环境变量（Vite）
来源：http://gip.guowangkeji.top

import.meta.env.VITE_API_URL
来源：http://vcs.bbcook.cn

================================================================================
来源：http://fkw.xziqi.cn

统计汇总
来源：http://bcq.yuanzhike.top

================================================================================
来源：http://unm.ydjk.org.cn

按语言统计（条）：
来源：http://uqs.iojbl.cn

Python ......... 252
来源：http://ros.daria6918.cn

PHP ............ 252
来源：http://vhk.jyoumei.cn

JavaScript ..... 252
来源：http://wzb.sufxvd.cn

TypeScript ..... 212
来源：http://wla.sufxvd.cn

Java ........... 212
来源：http://pzu.cashguo.top

Go ............. 212
来源：http://bre.xingfuxueyuan.xyz

Ruby ........... 212
来源：http://uif.fktsv.cn

C# ............. 212
来源：http://fzt.meibo888.top

C .............. 30
来源：http://zgn.vqdsnc.cn

C++ ............ 30
来源：http://lri.meibo888.top

SQL ............ 90
来源：http://fvm.chenzaomai.com

Bash ........... 80
来源：http://fxu.0kj1m.cn


<!-- 参考信息 -->