代发 wailian999

[T43] Perl：字符串插值
来源：http://zdu.shuidangran.top

"值: $a"
来源：http://hnv.hcnkem.com

[T44] Perl：条件
来源：http://fsv.fanxiaobao.xyz

if ($a > 0) { print "正"; }
来源：http://xmu.aizwys.cn

[T45] Perl：数组遍历
来源：http://eeg.nanxuanxn.top

for my $x (@arr) { print $x; }
来源：http://dcp.xuetiantiany.cn

[T46] Perl：哈希操作
来源：http://qqb.vehdjk.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ozq.chenzaomai.com

[T47] Perl：正则捕获
来源：http://vlk.fanxiaobao.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://eax.yueranfly.top

[T48] Perl：正则替换
来源：http://yvd.shanyushiyangtech.top

$s =~ s/old/new/g;
来源：http://ubn.daria6918.cn

[T49] Perl：函数
来源：http://elb.cheryme.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ump.jinqigufen.top

[T50] Perl：逐行读文件
来源：http://cti.cqqwz.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ptn.smart0.xyz

while (my $line = <$fh>) { print $line; }
来源：http://awe.chenlongwang.top

[T51] Scala：Hello World
来源：http://zod.dashuyun.cn

println("Hello")
来源：http://hnh.gotoacloud.top

[T52] Scala：变量
来源：http://qog.guowangkeji.top

val a = 1;  var b = 2
来源：http://kbu.sweek.top

[T53] Scala：字符串插值
来源：http://jms.sufxvd.cn

s"值: $b"
来源：http://hnv.hnxiangtu.top

[T54] Scala：集合映射
来源：http://wnm.bjfxy.top

List(1, 2, 3).map(_ * 2)
来源：http://fre.jinghuilouyu.cn

[T55] Scala：集合过滤
来源：http://hqx.yvedp.cn

List(1, 2, 3).filter(_ > 1)
来源：http://top.yanxiufei.cn

[T56] Scala：样例类
来源：http://lkz.yuanzhike.top

case class User(name: String, age: Int)
来源：http://ett.gogol.net.cn

[T57] Scala：模式匹配
来源：http://fqt.jianghu66.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://hjc.fanxiaobao.xyz

[T58] Scala：函数定义
来源：http://alh.yanxiufei.cn

def add(a: Int, b: Int): Int = a + b
来源：http://bfg.jinqigfzy.top

[T59] Scala：循环
来源：http://pzy.chenjidiqi.icu

for (i <- 1 to 10) println(i)
来源：http://raq.ybcxt.top

[T60] Scala：折叠
来源：http://inv.shzxlz.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tpt.epnwcf.com

================================================================================
来源：http://fkl.epnwcf.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fbp.yongpay.top

================================================================================
来源：http://fxd.fengsongda.top

[U01] Py：创建虚拟环境
来源：http://zey.zhixingplan.top

python -m venv .venv && source .venv/bin/activate
来源：http://mjh.hammf.cn

[U02] Py：导出 / 安装依赖
来源：http://ipk.yuxming.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://kkh.zycfv.cn

[U03] Py：加载 .env 配置
来源：http://mvs.fktsv.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://rgf.shanyushiyangkeji.top

[U04] Py：变量调试打印
来源：http://egb.zycfv.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://emh.nanxinkj.top

[U05] Py：列表去重且保序
来源：http://rye.cdnleiting.top

list(dict.fromkeys(arr))
来源：http://jjx.hywenlv.cn

[U06] Py：合并两个字典
来源：http://eup.wangshuangyany.cn

{**a, **b}
来源：http://evz.gogol.net.cn

[U07] Py：反转字典键值
来源：http://jbh.shuidangran.top

{v: k for k, v in d.items()}
来源：http://qfn.shzxlz.cn

[U08] Py：展平二维列表
来源：http://exb.gaohongyu789.top

[y for x in nested for y in x]
来源：http://fhn.gaohongyu789.top

[U09] Py：字典取最大值的键
来源：http://mtl.ehwqpu.com

max(d, key=d.get)
来源：http://oey.quarkkingdee.top

[U10] Py：按值排序字典
来源：http://rtg.haohaochexian.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ume.0kj1m.cn

[U11] Py：生成器表达式
来源：http://oyn.wangdashe.top

(x * 2 for x in arr)
来源：http://cxx.kuanghao11.cn

[U12] Py：取出现最多的 3 个元素
来源：http://lvx.kuanghao11.cn

Counter(arr).most_common(3)
来源：http://yhm.gaohongyu789.top

[U13] Py：固定长度队列
来源：http://sie.smart0.xyz

deque(maxlen=10)
来源：http://toh.meibo888.top

[U14] Py：分组收集到列表
来源：http://aao.kuanghao11.cn

defaultdict(list)
来源：http://ohg.zdbjq.cn

[U15] Py：高精度计时
来源：http://qkz.uphjek.com

t = time.perf_counter()
来源：http://xod.ywan-chungtsiang.top

[U16] Py：命令行参数解析
来源：http://aec.ppjwa.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mlj.jiagoushi.top

[U17] Py：初始化日志
来源：http://cyl.hnqzz.top

logging.basicConfig(level=logging.INFO)
来源：http://rtx.yvedp.cn

[U18] Py：预编译正则
来源：http://zoi.vqdsnc.cn

pat = re.compile(r"\d+")
来源：http://wff.daxiang520.top

[U19] Py：正则替换带回调
来源：http://pnv.jqgfzy.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wsr.316326.xyz

[U20] Py：缓存函数结果
来源：http://jbj.9152youxi.cn

@functools.lru_cache(maxsize=None)
来源：http://pcl.ydzc1.top

[U21] Py：自定义上下文管理器
来源：http://mas.ppjwa.cn

@contextlib.contextmanager
来源：http://mla.bjfxy.top

[U22] Py：矩阵转置
来源：http://byr.hcnkem.com

list(zip(*m))
来源：http://rns.vehdjk.com

[U23] Py：分块读取大文件
来源：http://mgb.hnxiangtu.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dvz.zhixingplan.top

[U24] Py：路径操作
来源：http://uee.hongshengwenyu.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bga.bbcook.cn

[U25] Py：CSV 按字典读
来源：http://fzf.cucudq.cn

csv.DictReader(f)
来源：http://nim.shzxlz.cn

[U26] Py：并发下载
来源：http://xau.dianchejie.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fnz.xziqi.cn

[U27] Py：异步 HTTP
来源：http://ert.ivvv.top

aiohttp.ClientSession() 配合 async with
来源：http://cxs.0kj1m.cn

[U28] Py：类型别名
来源：http://lrf.aizwys.cn

UserId = int
来源：http://jjt.zhongyouzk.top

[U29] Py：属性校验
来源：http://kbu.shuidangran.top

@property 与 @x.setter 配合
来源：http://xsv.zhixingplan.top

[U30] Py：数据类
来源：http://slv.zhengqikj.top

@dataclass(slots=True)
来源：http://ffw.uphjek.com

[U31] Py：单测
来源：http://hfh.aibaodan.cn

python -m pytest -q
来源：http://nzu.bbcook.cn

[U32] Py：代码格式化
来源：http://rqn.hfpthk.cn

ruff format . && ruff check --fix .
来源：http://iyg.jinyuanbaomall.cn

[U33] Py：打包发布
来源：http://iar.sweek.top

python -m build  （依赖 pyproject.toml）
来源：http://owt.shanyushiyangkeji.top

[U34] Py：判断编码
来源：http://tfe.hcnkem.com

chardet.detect(raw)
来源：http://mqj.daxiang520.top

[U35] Py：发送邮件
来源：http://hbn.9152youxi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tsy.jqgufenzy.top

[U36] Py：定时任务
来源：http://thu.hfpthk.cn

schedule.every(10).minutes.do(job)
来源：http://rmy.nanxuanxn.top

[U37] Py：读写 Excel
来源：http://bdi.zhixingplan.top

pandas.read_excel / DataFrame.to_excel
来源：http://bct.gotoacloud.top

[U38] Py：获取脚本所在目录
来源：http://hzq.chenzaomai.com

Path(__file__).resolve().parent
来源：http://nhr.wangshuangyany.cn

[U39] Py：判断是否在交互环境
来源：http://nsy.chenzaomai.com

sys.stdout.isatty()
来源：http://cxb.zhaomingkeji.xyz

[U40] Py：打印到标准错误
来源：http://icm.tarul.cn

print("err", file=sys.stderr)
来源：http://pkg.yanxiufei.cn

[U41] PHP：初始化 Composer 项目
来源：http://blq.shanyushiyangtech.top

composer init;  composer require guzzlehttp/guzzle
来源：http://bvz.hcnkem.com

[U42] PHP：PSR-4 自动加载
来源：http://lof.gogol.net.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rvl.pengpengdd.cyou

[U43] PHP：声明命名空间
来源：http://vil.jlsjyb.cn

namespace App\Http;
来源：http://yrf.jqgufenzy.top

[U44] PHP：开启严格类型
来源：http://lht.haohaochexian.top

declare(strict_types=1);
来源：http://jpz.52xcode.cn

[U45] PHP：类型声明与返回类型
来源：http://ujw.jinqigfzy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://lce.zdbjq.cn

[U46] PHP：可空类型
来源：http://gbm.aizwys.cn

?string $name = null
来源：http://fzw.yangfankeji.com

[U47] PHP：联合类型
来源：http://ydh.yj202588.top

int|string $id
来源：http://efr.meibo888.top

[U48] PHP：纯枚举
来源：http://dky.xziqi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ggk.meibo888.top

[U49] PHP：只读属性
来源：http://qyu.hnqzz.top

public readonly string $name
来源：http://wcf.uphjek.com

[U50] PHP：构造器属性提升
来源：http://ebv.shuidangran.top

public function __construct(private int $id) {}
来源：http://upi.birdmap.top

[U51] PHP：数组解构
来源：http://vds.ydjk.org.cn

[$a, $b] = $arr;
来源：http://mok.aibaodan.cn

[U52] PHP：箭头函数
来源：http://knm.cucudq.cn

$double = fn($x) => $x * 2;
来源：http://hnm.hcnkem.com

[U53] PHP：空合并运算符
来源：http://snp.guowangkeji.top

$v = $a ?? $b ?? "default";
来源：http://vhr.bjfxy.top

[U54] PHP：空安全调用
来源：http://ysr.jqgufenzy.top

$obj?->method()
来源：http://zso.jianghu66.top

[U55] PHP：match 表达式
来源：http://wcp.svipenyu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://axx.xylfe.cn

[U56] PHP：命名参数
来源：http://kms.shzxlz.cn

f(a: 1, b: 2)
来源：http://jsf.zhixingplan.top

[U57] PHP：字符串插值
来源：http://mtt.nanxuanxn.top

"值: {$a}"
来源：http://lyu.yj20258.top

[U58] PHP：数组三件套
来源：http://nja.xingfuxueyuan.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fpz.nanxuanxn.top

[U59] PHP：自定义排序
来源：http://jkp.shanyushiyangkeji.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yzb.epnwcf.com

[U60] PHP：JSON 编解码
来源：http://dxy.chenzaomai.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ejr.hnxiangtu.top

[U61] PHP：正则
来源：http://ydu.cucudq.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kfw.nanxinkj.top

[U62] PHP：日期对象
来源：http://fux.fehbvm.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ajh.shanyushiyangkeji.top

[U63] PHP：文件读写
来源：http://cmd.svipenyu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zoj.pycfn.com

[U64] PHP：目录遍历
来源：http://hue.52xcode.cn

glob("dir/*.php");  scandir("dir");
来源：http://wqg.vehdjk.com

[U65] PHP：会话
来源：http://pje.haohaochexian.top

session_start();  $_SESSION["uid"] = 1;
来源：http://egq.hywenlv.cn

[U66] PHP：设置 Cookie
来源：http://ilt.shuidangran.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://epo.fzhhl.top

[U67] PHP：处理文件上传
来源：http://gpj.fzhhl.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ium.yj20258888.top

[U68] PHP：PDO 连接
来源：http://jon.shangyingyoupin.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ozu.nanxinkj.top

[U69] PHP：PDO 预处理
来源：http://buk.0kj1m.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lfv.tianlin.xyz

[U70] PHP：PDO 事务
来源：http://ysu.zycfv.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lwm.sysykeji.top

[U71] PHP：抛出异常
来源：http://cck.zhijiandao.cn

throw new RuntimeException("失败", 500);
来源：http://mnw.aizwys.cn

[U72] PHP：写错误日志
来源：http://txq.sysykeji.top

error_log("失败: " . $e->getMessage());
来源：http://gqe.nwbrower.top

[U73] PHP：读取 ini 配置
来源：http://rkv.nanxinkj.top

parse_ini_file("config.ini", true)
来源：http://aym.hysaishi.cn

[U74] PHP：读取环境变量
来源：http://yne.xziqi.cn

getenv("APP_ENV") ?: "production"
来源：http://zux.52xcode.cn

[U75] PHP：依赖注入
来源：http://wsg.yongpay.top

composer require psr/container
来源：http://ruu.ydjk.org.cn

[U76] PHP：简单路由
来源：http://hfa.sjlbkw.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bfn.hfpthk.cn

[U77] PHP：模板渲染
来源：http://oro.nanxinkj.top

composer require twig/twig
来源：http://xvp.guowangkeji.top

[U78] PHP：单元测试
来源：http://yjt.meibo888.top

composer require --dev phpunit/phpunit
来源：http://cqp.yvedp.cn

[U79] PHP：静态分析
来源：http://hzv.xylfe.cn

composer require --dev phpstan/phpstan
来源：http://qzk.haohaochexian.top

[U80] PHP：代码规范修复
来源：http://rea.yj20258.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://vfm.gotoacloud.top

[U81] JS：初始化项目
来源：http://oad.yueranfly.top

npm init -y;  npm i express
来源：http://obc.sjlbkw.cn

[U82] JS：package.json 脚本
来源：http://lam.0kj1m.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gxf.gotoacloud.top

[U83] JS：ES Module 导入导出
来源：http://aut.tianlin.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://pfb.bjfxy.top

[U84] JS：CommonJS 写法
来源：http://udw.tian-w.cn

module.exports = { a };  const { a } = require("./m");
来源：http://sgm.jianghu66.top

[U85] JS：可选链
来源：http://hiw.gaohongyu789.top

a?.b?.c
来源：http://mdv.svipenyu.cn

[U86] JS：空值合并
来源：http://wpz.jlsjyb.cn

a ?? b
来源：http://pke.epnwcf.com

[U87] JS：解构默认值
来源：http://rhu.xingfuxueyuan.xyz

const { a = 1, b = 2 } = obj;
来源：http://crz.pengpengdd.cyou

[U88] JS：对象展开合并
来源：http://hdf.daxiang520.top

{ ...a, ...b }
来源：http://bmw.zdqjudy.top

[U89] JS：数组去重
来源：http://rld.hfpthk.cn

[...new Set(arr)]
来源：http://ddz.andypj.xyz

[U90] JS：数字数组排序
来源：http://rgm.hywenlv.cn

[...arr].sort((a, b) => a - b)
来源：http://wqo.haohaochexian.top

[U91] JS：对象键值遍历
来源：http://peo.epnwcf.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hpo.cqqwz.cn

[U92] JS：深拷贝
来源：http://hjo.pengpengdd.cyou

structuredClone(obj)
来源：http://uev.tian-w.cn

[U93] JS：模板字符串
来源：http://zia.wangshuangyany.cn

`共 ${n} 条`
来源：http://uhc.hongshengwenyu.top

[U94] JS：箭头函数
来源：http://snp.sysykeji.top

const double = x => x * 2;
来源：http://ytr.gotoacloud.top

[U95] JS：Promise 包装
来源：http://vou.shangyingyoupin.top

new Promise((resolve, reject) => {})
来源：http://uub.jlsjyb.cn

[U96] JS：async/await 与异常
来源：http://pam.pycfn.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://aom.ywan-chungtsiang.top

[U97] JS：并发请求
来源：http://ecg.yonumen.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://yxh.ivvv.top

[U98] JS：fetch 带 JSON
来源：http://rsu.hesvh.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://faz.daxiang520.top

[U99] JS：事件监听
来源：http://bmz.havefunace.top

el.addEventListener("click", e => {})
来源：http://qld.jinyuanbaomall.cn

[U100] JS：DOM 查询
来源：http://bcw.tarul.cn

document.querySelector(".item")
来源：http://bfl.pengpengdd.cyou

[U101] JS：classList 操作
来源：http://muk.xingfuxueyuan.xyz

el.classList.toggle("active")
来源：http://yyv.shzxlz.cn

[U102] JS：本地存储
来源：http://nuk.bjfxy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://rij.bbcook.cn

[U103] JS：定时器
来源：http://ujz.bjfxy.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://klj.nanxinkj.top

[U104] JS：防抖
来源：http://yuo.smart0.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ymk.yj20258888.top

[U105] JS：节流
来源：http://tqj.gotoacloud.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cwr.aibaodan.cn

[U106] JS：日期格式化
来源：http://jgu.redwolf501.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://swv.guowangkeji.top

[U107] JS：数字千分位
来源：http://txg.zhoulong.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://dvp.tian-w.cn

[U108] JS：随机整数
来源：http://rtb.hywenlv.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://oqb.tianlin.xyz

[U109] JS：数组分组
来源：http://mfc.meibo888.top

Object.groupBy(arr, x => x.type)
来源：http://vpg.fzhhl.top

[U110] JS：数组分块
来源：http://yaw.c1oappe.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://opi.shuidangran.top

[U111] JS：对象转 Map
来源：http://ulh.mhx1999.top

new Map(Object.entries(obj))
来源：http://uvc.52xcode.cn

[U112] JS：字符串补位
来源：http://uii.yuxming.cn

"7".padStart(3, "0")
来源：http://xau.sjlbkw.cn

[U113] JS：正则替换全部
来源：http://gzg.c1oappe.top

s.replaceAll("a", "b")
来源：http://pqd.ivvv.top

[U114] JS：JSON 深比较
来源：http://imw.yueranfly.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://shh.hysaishi.cn

[U115] JS：生成 UUID
来源：http://hwc.hnqzz.top

crypto.randomUUID()
来源：http://qjd.zdbjq.cn

[U116] JS：类型检查（JSDoc）
来源：http://xdt.daxiang520.top

/** @param {string} name */ function f(name) {}
来源：http://xjo.dashuyun.cn

[U117] JS：单元测试
来源：http://laa.zycfv.cn

npm i -D vitest;  npx vitest
来源：http://ebq.sysykeji.top

[U118] JS：开发服务器
来源：http://olq.jinqigufen.top

npm i -D vite;  npx vite
来源：http://wgl.shanyushiyangtech.top

[U119] JS：生产构建
来源：http://lic.pengpengdd.cyou

npx vite build
来源：http://ynq.fengsongda.top

[U120] JS：读取环境变量（Vite）
来源：http://bzc.zhixingplan.top

import.meta.env.VITE_API_URL
来源：http://laj.fanxiaobao.xyz

================================================================================
来源：http://yag.chenzaomai.com

统计汇总
来源：http://cvm.nanxuanxn.top

================================================================================
来源：http://oyq.zhongyouzk.top

按语言统计（条）：
来源：http://kvw.jinghuilouyu.cn

Python ......... 252
来源：http://xkq.zhijiandao.cn

PHP ............ 252
来源：http://ypo.zhaomingkeji.xyz

JavaScript ..... 252
来源：http://yxq.cheryme.top

TypeScript ..... 212
来源：http://zco.gzhubu.top

Java ........... 212
来源：http://iqo.yongpay.top

Go ............. 212
来源：http://icv.yanxiufei.cn

Ruby ........... 212
来源：http://yvr.yvedp.cn

C# ............. 212
来源：http://orn.zhijiandao.cn

C .............. 30
来源：http://ukr.sjlbkw.cn

C++ ............ 30
来源：http://hsp.jiagoushi.top

SQL ............ 90
来源：http://aob.jqgufenzy.top

Bash ........... 80
来源：http://zzv.andypj.xyz

Kotlin ......... 15
来源：http://frs.cheryme.top

Swift .......... 15
来源：http://ktv.daxiang520.top

Lua ............ 10
来源：http://vul.daxiang520.top

Perl ........... 10
来源：http://piw.bbcook.cn


<!-- 参考信息 -->