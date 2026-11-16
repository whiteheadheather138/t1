代发 wailian999

[T45] Perl：数组遍历
来源：http://tnq.daxiang520.top

for my $x (@arr) { print $x; }
来源：http://tco.xziqi.cn

[T46] Perl：哈希操作
来源：http://nug.jinyuanbaomall.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://szh.daria6918.cn

[T47] Perl：正则捕获
来源：http://riy.yueranfly.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://blq.gaohongyu789.top

[T48] Perl：正则替换
来源：http://oqx.birdmap.top

$s =~ s/old/new/g;
来源：http://ewp.ehwqpu.com

[T49] Perl：函数
来源：http://kow.andypj.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vdp.xuetiantiany.cn

[T50] Perl：逐行读文件
来源：http://tly.fanxiaobao.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://iqx.fktsv.cn

while (my $line = <$fh>) { print $line; }
来源：http://azh.ydzc1.top

[T51] Scala：Hello World
来源：http://pdz.daria6918.cn

println("Hello")
来源：http://gcf.daria6918.cn

[T52] Scala：变量
来源：http://woe.fanxiaobao.xyz

val a = 1;  var b = 2
来源：http://kss.ppjwa.cn

[T53] Scala：字符串插值
来源：http://lnk.zhixingplan.top

s"值: $b"
来源：http://apj.kuanghao11.cn

[T54] Scala：集合映射
来源：http://lpb.ehwqpu.com

List(1, 2, 3).map(_ * 2)
来源：http://tfa.yj20258888.top

[T55] Scala：集合过滤
来源：http://bah.chenlongwang.top

List(1, 2, 3).filter(_ > 1)
来源：http://wbb.jinyuanbaomall.cn

[T56] Scala：样例类
来源：http://ahs.xylfe.cn

case class User(name: String, age: Int)
来源：http://zqj.ydjk.org.cn

[T57] Scala：模式匹配
来源：http://xes.jinqigfzy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://pip.vqdsnc.cn

[T58] Scala：函数定义
来源：http://eki.yvedp.cn

def add(a: Int, b: Int): Int = a + b
来源：http://juu.9152youxi.cn

[T59] Scala：循环
来源：http://wuw.jinghuilouyu.cn

for (i <- 1 to 10) println(i)
来源：http://efo.cashguo.top

[T60] Scala：折叠
来源：http://kew.gogol.net.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yog.epnwcf.com

================================================================================
来源：http://tgg.nanxinkj.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hlx.jqgfzy.top

================================================================================
来源：http://tah.havefunace.top

[U01] Py：创建虚拟环境
来源：http://orm.cdnleiting.top

python -m venv .venv && source .venv/bin/activate
来源：http://kag.cashguo.top

[U02] Py：导出 / 安装依赖
来源：http://ffx.snrcjt.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://oci.quarkkingdee.top

[U03] Py：加载 .env 配置
来源：http://tij.jqgufenzy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ase.shanyushiyangtech.top

[U04] Py：变量调试打印
来源：http://ohm.zhengqikj.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nih.zhengqikj.top

[U05] Py：列表去重且保序
来源：http://dsi.ydjk.org.cn

list(dict.fromkeys(arr))
来源：http://klk.haohaochexian.top

[U06] Py：合并两个字典
来源：http://dxv.jqgfzy.top

{**a, **b}
来源：http://ipe.vqdsnc.cn

[U07] Py：反转字典键值
来源：http://gdm.yj202588.top

{v: k for k, v in d.items()}
来源：http://jpx.jinyuanbaomall.cn

[U08] Py：展平二维列表
来源：http://kkn.andypj.xyz

[y for x in nested for y in x]
来源：http://tli.jinghuilouyu.cn

[U09] Py：字典取最大值的键
来源：http://vty.jinqigufen.top

max(d, key=d.get)
来源：http://ibz.c1oappe.top

[U10] Py：按值排序字典
来源：http://mkj.shuidangran.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://owj.shanyushiyangtech.top

[U11] Py：生成器表达式
来源：http://mxk.svipenyu.cn

(x * 2 for x in arr)
来源：http://uwd.dashuyun.cn

[U12] Py：取出现最多的 3 个元素
来源：http://wky.yangfankeji.com

Counter(arr).most_common(3)
来源：http://edo.bbcook.cn

[U13] Py：固定长度队列
来源：http://awh.yj20258.top

deque(maxlen=10)
来源：http://rny.hnxiangtu.top

[U14] Py：分组收集到列表
来源：http://kcb.c1oappe.top

defaultdict(list)
来源：http://sji.guowangkeji.top

[U15] Py：高精度计时
来源：http://tdy.zhijiandao.cn

t = time.perf_counter()
来源：http://lxg.hongshengwenyu.top

[U16] Py：命令行参数解析
来源：http://vlu.wangshuangyany.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nna.fktsv.cn

[U17] Py：初始化日志
来源：http://nbr.zdqjudy.top

logging.basicConfig(level=logging.INFO)
来源：http://tfe.dianchejie.cn

[U18] Py：预编译正则
来源：http://zij.bbcook.cn

pat = re.compile(r"\d+")
来源：http://bjw.sxryk.cn

[U19] Py：正则替换带回调
来源：http://rqn.jyoumei.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bcs.hammf.cn

[U20] Py：缓存函数结果
来源：http://yje.andypj.xyz

@functools.lru_cache(maxsize=None)
来源：http://tot.fzhhl.top

[U21] Py：自定义上下文管理器
来源：http://eic.xuetiantiany.cn

@contextlib.contextmanager
来源：http://kpt.jyoumei.cn

[U22] Py：矩阵转置
来源：http://lof.hongshengwenyu.top

list(zip(*m))
来源：http://ivq.zhijiandao.cn

[U23] Py：分块读取大文件
来源：http://rzy.ehwqpu.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hhe.ybcxt.top

[U24] Py：路径操作
来源：http://xnl.zdbjq.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ova.tarul.cn

[U25] Py：CSV 按字典读
来源：http://ctl.cheryme.top

csv.DictReader(f)
来源：http://kxg.dianchejie.cn

[U26] Py：并发下载
来源：http://eav.hnqzz.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://icm.cashguo.top

[U27] Py：异步 HTTP
来源：http://ceu.jiagoushi.top

aiohttp.ClientSession() 配合 async with
来源：http://iam.snrcjt.cn

[U28] Py：类型别名
来源：http://qam.wangshuangyany.cn

UserId = int
来源：http://dkn.hesvh.cn

[U29] Py：属性校验
来源：http://rtr.wangshuangyany.cn

@property 与 @x.setter 配合
来源：http://sjf.shangyingyoupin.top

[U30] Py：数据类
来源：http://scr.hnqzz.top

@dataclass(slots=True)
来源：http://lai.yuanzhike.top

[U31] Py：单测
来源：http://blk.cheryme.top

python -m pytest -q
来源：http://xnl.kuanghao11.cn

[U32] Py：代码格式化
来源：http://vow.yonumen.top

ruff format . && ruff check --fix .
来源：http://mlc.yuxming.cn

[U33] Py：打包发布
来源：http://nes.jqgufenzy.top

python -m build  （依赖 pyproject.toml）
来源：http://emr.zycfv.cn

[U34] Py：判断编码
来源：http://oiz.jinghuilouyu.cn

chardet.detect(raw)
来源：http://nbk.daxiang520.top

[U35] Py：发送邮件
来源：http://hhh.daxiang520.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://teh.xuetiantiany.cn

[U36] Py：定时任务
来源：http://kzb.0kj1m.cn

schedule.every(10).minutes.do(job)
来源：http://grw.c1oappe.top

[U37] Py：读写 Excel
来源：http://iyy.ehwqpu.com

pandas.read_excel / DataFrame.to_excel
来源：http://xrg.redwolf501.top

[U38] Py：获取脚本所在目录
来源：http://beg.hammf.cn

Path(__file__).resolve().parent
来源：http://egt.pycfn.com

[U39] Py：判断是否在交互环境
来源：http://nhg.vehdjk.com

sys.stdout.isatty()
来源：http://rij.hammf.cn

[U40] Py：打印到标准错误
来源：http://klo.yvedp.cn

print("err", file=sys.stderr)
来源：http://twf.pengpengdd.cyou

[U41] PHP：初始化 Composer 项目
来源：http://luj.andypj.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://fwi.vehdjk.com

[U42] PHP：PSR-4 自动加载
来源：http://yyg.wangdashe.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://err.52xcode.cn

[U43] PHP：声明命名空间
来源：http://vsj.hywenlv.cn

namespace App\Http;
来源：http://rot.yuxming.cn

[U44] PHP：开启严格类型
来源：http://bfp.hnqzz.top

declare(strict_types=1);
来源：http://huk.yj202588.top

[U45] PHP：类型声明与返回类型
来源：http://ayk.iojbl.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://xdy.zdbjq.cn

[U46] PHP：可空类型
来源：http://lmd.shuidangran.top

?string $name = null
来源：http://efq.52xcode.cn

[U47] PHP：联合类型
来源：http://zeo.ydzc1.top

int|string $id
来源：http://ywt.shuidangran.top

[U48] PHP：纯枚举
来源：http://cqr.jinyuanbaomall.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://knp.hnxiangtu.top

[U49] PHP：只读属性
来源：http://qas.yangfankeji.com

public readonly string $name
来源：http://tcy.andypj.xyz

[U50] PHP：构造器属性提升
来源：http://ale.hongshengwenyu.top

public function __construct(private int $id) {}
来源：http://jhn.cheryme.top

[U51] PHP：数组解构
来源：http://zlm.zhengqikj.top

[$a, $b] = $arr;
来源：http://wzu.gzhubu.top

[U52] PHP：箭头函数
来源：http://dvn.tianlin.xyz

$double = fn($x) => $x * 2;
来源：http://eqx.wangshuangyany.cn

[U53] PHP：空合并运算符
来源：http://hca.mhx1999.top

$v = $a ?? $b ?? "default";
来源：http://ckj.ydjk.org.cn

[U54] PHP：空安全调用
来源：http://isp.yj202588.top

$obj?->method()
来源：http://alu.fktsv.cn

[U55] PHP：match 表达式
来源：http://bft.iojbl.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ipm.birdmap.top

[U56] PHP：命名参数
来源：http://ecx.ydjk.org.cn

f(a: 1, b: 2)
来源：http://woh.yj20258.top

[U57] PHP：字符串插值
来源：http://jlj.yonumen.top

"值: {$a}"
来源：http://ctb.hfpthk.cn

[U58] PHP：数组三件套
来源：http://mbh.dashuyun.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ctd.c1oappe.top

[U59] PHP：自定义排序
来源：http://zps.pycfn.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://shi.fanxiaobao.xyz

[U60] PHP：JSON 编解码
来源：http://leb.gzhubu.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://anb.sxryk.cn

[U61] PHP：正则
来源：http://gxc.ydzc1.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kho.bjfxy.top

[U62] PHP：日期对象
来源：http://ysc.shuidangran.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hyi.smart0.xyz

[U63] PHP：文件读写
来源：http://drm.shanyushiyangtech.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vzh.yj20258888.top

[U64] PHP：目录遍历
来源：http://xjy.gogol.net.cn

glob("dir/*.php");  scandir("dir");
来源：http://xnr.feifeiyinyue.top

[U65] PHP：会话
来源：http://tfl.fehbvm.com

session_start();  $_SESSION["uid"] = 1;
来源：http://xxj.quarkkingdee.top

[U66] PHP：设置 Cookie
来源：http://zcn.yanxiufei.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wcp.pycfn.com

[U67] PHP：处理文件上传
来源：http://tle.vqdsnc.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hel.nanxinkj.top

[U68] PHP：PDO 连接
来源：http://tof.guannengcc.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ror.hfpthk.cn

[U69] PHP：PDO 预处理
来源：http://maf.hfpthk.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lww.gotoacloud.top

[U70] PHP：PDO 事务
来源：http://foj.jianghu66.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jew.xuetiantiany.cn

[U71] PHP：抛出异常
来源：http://jvx.fktsv.cn

throw new RuntimeException("失败", 500);
来源：http://jbk.shanyushiyangkeji.top

[U72] PHP：写错误日志
来源：http://qjy.fehbvm.com

error_log("失败: " . $e->getMessage());
来源：http://hoi.daria6918.cn

[U73] PHP：读取 ini 配置
来源：http://mkk.ppjwa.cn

parse_ini_file("config.ini", true)
来源：http://qlg.chenlongwang.top

[U74] PHP：读取环境变量
来源：http://udf.gotoacloud.top

getenv("APP_ENV") ?: "production"
来源：http://kxx.sweek.top

[U75] PHP：依赖注入
来源：http://ajp.chenlongwang.top

composer require psr/container
来源：http://apm.jinghuilouyu.cn

[U76] PHP：简单路由
来源：http://dxa.wangshuangyany.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mhw.vqdsnc.cn

[U77] PHP：模板渲染
来源：http://ufh.gzhubu.top

composer require twig/twig
来源：http://ywd.yuanzhike.top

[U78] PHP：单元测试
来源：http://mal.tian-w.cn

composer require --dev phpunit/phpunit
来源：http://agv.hnqzz.top

[U79] PHP：静态分析
来源：http://dhi.pycfn.com

composer require --dev phpstan/phpstan
来源：http://dme.chenzaomai.com

[U80] PHP：代码规范修复
来源：http://wok.xziqi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://fvj.svipenyu.cn

[U81] JS：初始化项目
来源：http://yxl.tian-w.cn

npm init -y;  npm i express
来源：http://lsd.hcnkem.com

[U82] JS：package.json 脚本
来源：http://vsl.xinyue.icu

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qet.yongpay.top

[U83] JS：ES Module 导入导出
来源：http://vhz.hnqzz.top

export const a = 1;  import { a } from "./m.js";
来源：http://kup.mhx1999.top

[U84] JS：CommonJS 写法
来源：http://acn.xylfe.cn

module.exports = { a };  const { a } = require("./m");
来源：http://yrg.tian-w.cn

[U85] JS：可选链
来源：http://aqq.vqdsnc.cn

a?.b?.c
来源：http://qqt.sweek.top

[U86] JS：空值合并
来源：http://pat.hcnkem.com

a ?? b
来源：http://eec.tianlin.xyz

[U87] JS：解构默认值
来源：http://wnm.redwolf501.top

const { a = 1, b = 2 } = obj;
来源：http://voa.epnwcf.com

[U88] JS：对象展开合并
来源：http://rhu.yj202588.top

{ ...a, ...b }
来源：http://rpb.cheryme.top

[U89] JS：数组去重
来源：http://azu.bjfxy.top

[...new Set(arr)]
来源：http://efs.nanxinkj.top

[U90] JS：数字数组排序
来源：http://avc.gaohongyu789.top

[...arr].sort((a, b) => a - b)
来源：http://dev.cucudq.cn

[U91] JS：对象键值遍历
来源：http://xrh.xuanzx.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dcp.yueranfly.top

[U92] JS：深拷贝
来源：http://eth.svipenyu.cn

structuredClone(obj)
来源：http://lgq.xylfe.cn

[U93] JS：模板字符串
来源：http://hzr.zycfv.cn

`共 ${n} 条`
来源：http://sju.shanyushiyangtech.top

[U94] JS：箭头函数
来源：http://yfv.sxryk.cn

const double = x => x * 2;
来源：http://mce.yanxiufei.cn

[U95] JS：Promise 包装
来源：http://ezs.gogol.net.cn

new Promise((resolve, reject) => {})
来源：http://ptq.nanxuanxn.top

[U96] JS：async/await 与异常
来源：http://lgb.52xcode.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fmn.fehbvm.com

[U97] JS：并发请求
来源：http://nsh.bjfxy.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://bzy.0kj1m.cn

[U98] JS：fetch 带 JSON
来源：http://thx.jlsjyb.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jtv.zhongyouzk.top

[U99] JS：事件监听
来源：http://wkh.fzhhl.top

el.addEventListener("click", e => {})
来源：http://fcu.jqgfzy.top

[U100] JS：DOM 查询
来源：http://etc.gotoacloud.top

document.querySelector(".item")
来源：http://gti.jqgfzy.top

[U101] JS：classList 操作
来源：http://loh.ehwqpu.com

el.classList.toggle("active")
来源：http://sbq.chenjidiqi.icu

[U102] JS：本地存储
来源：http://pol.feifeiyinyue.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://zxg.sxryk.cn

[U103] JS：定时器
来源：http://yjl.jiagoushi.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tqy.uphjek.com

[U104] JS：防抖
来源：http://bal.xingfuxueyuan.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zow.andypj.xyz

[U105] JS：节流
来源：http://sji.cheryme.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zpb.yj20258888.top

[U106] JS：日期格式化
来源：http://mdn.guannengcc.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bmx.bbcook.cn

[U107] JS：数字千分位
来源：http://ecl.yj20258.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://akn.yangfankeji.com

[U108] JS：随机整数
来源：http://zlx.cqqwz.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ode.jlsjyb.cn

[U109] JS：数组分组
来源：http://euk.cdnleiting.top

Object.groupBy(arr, x => x.type)
来源：http://zky.jiagoushi.top

[U110] JS：数组分块
来源：http://oku.hongshengwenyu.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cxi.sufxvd.cn

[U111] JS：对象转 Map
来源：http://fhd.vqdsnc.cn

new Map(Object.entries(obj))
来源：http://mnu.jianghu66.top

[U112] JS：字符串补位
来源：http://ygb.cdnleiting.top

"7".padStart(3, "0")
来源：http://xbc.9152youxi.cn

[U113] JS：正则替换全部
来源：http://gnz.dianchejie.cn

s.replaceAll("a", "b")
来源：http://yzv.cucudq.cn

[U114] JS：JSON 深比较
来源：http://fqa.yfazqb.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://sbr.nwbrower.top

[U115] JS：生成 UUID
来源：http://hjg.yj20258.top

crypto.randomUUID()
来源：http://iog.shuidangran.top

[U116] JS：类型检查（JSDoc）
来源：http://qoh.tanke756.top

/** @param {string} name */ function f(name) {}
来源：http://iyr.sjlbkw.cn

[U117] JS：单元测试
来源：http://xkq.cdnleiting.top

npm i -D vitest;  npx vitest
来源：http://pmo.sysykeji.top

[U118] JS：开发服务器
来源：http://zsq.fehbvm.com

npm i -D vite;  npx vite
来源：http://qxy.aizwys.cn

[U119] JS：生产构建
来源：http://zew.haohaochexian.top

npx vite build
来源：http://mnz.iojbl.cn

[U120] JS：读取环境变量（Vite）
来源：http://llu.wangshuangyany.cn

import.meta.env.VITE_API_URL
来源：http://gbm.jinghuilouyu.cn

================================================================================
来源：http://ytz.0kj1m.cn

统计汇总
来源：http://yae.hysaishi.cn

================================================================================
来源：http://xnn.uphjek.com

按语言统计（条）：
来源：http://yii.smart0.xyz

Python ......... 252
来源：http://kko.guowangkeji.top

PHP ............ 252
来源：http://uje.jyoumei.cn

JavaScript ..... 252
来源：http://pcg.ydzc1.top

TypeScript ..... 212
来源：http://fsh.c1oappe.top

Java ........... 212
来源：http://krm.yvedp.cn

Go ............. 212
来源：http://see.zhaomingkeji.xyz

Ruby ........... 212
来源：http://sqi.gzhubu.top

C# ............. 212
来源：http://ffw.yvedp.cn

C .............. 30
来源：http://zkx.daria6918.cn

C++ ............ 30
来源：http://cuu.havefunace.top

SQL ............ 90
来源：http://lcj.tanke756.top

Bash ........... 80
来源：http://mnf.daria6918.cn

Kotlin ......... 15
来源：http://pbi.birdmap.top

Swift .......... 15
来源：http://fsi.zhixingplan.top

Lua ............ 10
来源：http://yhb.daria6918.cn

Perl ........... 10
来源：http://zda.hfpthk.cn

Scala .......... 10
来源：http://dec.zdqjudy.top

------------------------------------
来源：http://qfr.hammf.cn

合计 ........... 2106 条
来源：http://ddh.shanyushiyangkeji.top

按章节统计：
来源：http://tja.yvedp.cn


<!-- 参考信息 -->