代发 wailian999

[T43] Perl：字符串插值
来源：http://cvm.sweek.top

"值: $a"
来源：http://jug.xingfuxueyuan.xyz

[T44] Perl：条件
来源：http://mcu.sweek.top

if ($a > 0) { print "正"; }
来源：http://lpv.shzxlz.cn

[T45] Perl：数组遍历
来源：http://uqc.chenlongwang.top

for my $x (@arr) { print $x; }
来源：http://ejg.fanxiaobao.xyz

[T46] Perl：哈希操作
来源：http://mlh.zhoulong.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zod.bbcook.cn

[T47] Perl：正则捕获
来源：http://onh.hysaishi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://rfk.yonumen.top

[T48] Perl：正则替换
来源：http://nsp.feifeiyinyue.top

$s =~ s/old/new/g;
来源：http://ruw.daxiang520.top

[T49] Perl：函数
来源：http://qpc.316326.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kgr.andypj.xyz

[T50] Perl：逐行读文件
来源：http://lpe.hnxiangtu.top

open my $fh, "<", "a.txt" or die $!;
来源：http://tsn.sjlbkw.cn

while (my $line = <$fh>) { print $line; }
来源：http://cvo.zdqjudy.top

[T51] Scala：Hello World
来源：http://zgf.jiagoushi.top

println("Hello")
来源：http://fun.hfpthk.cn

[T52] Scala：变量
来源：http://hdg.cashguo.top

val a = 1;  var b = 2
来源：http://jez.xuanzx.com

[T53] Scala：字符串插值
来源：http://mhe.dianchejie.cn

s"值: $b"
来源：http://awc.zycfv.cn

[T54] Scala：集合映射
来源：http://sgm.yonumen.top

List(1, 2, 3).map(_ * 2)
来源：http://out.cdnleiting.top

[T55] Scala：集合过滤
来源：http://ozm.jianghu66.top

List(1, 2, 3).filter(_ > 1)
来源：http://hrh.yongpay.top

[T56] Scala：样例类
来源：http://vgs.yfazqb.com

case class User(name: String, age: Int)
来源：http://eek.xziqi.cn

[T57] Scala：模式匹配
来源：http://amg.andypj.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://efn.xinyue.icu

[T58] Scala：函数定义
来源：http://maz.andypj.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://wvj.zycfv.cn

[T59] Scala：循环
来源：http://xlz.yongpay.top

for (i <- 1 to 10) println(i)
来源：http://xxb.gaohongyu789.top

[T60] Scala：折叠
来源：http://hmk.ctjpmb.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ekw.zhaomingkeji.xyz

================================================================================
来源：http://hea.zhiwuduotai.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://upm.zhaomingkeji.xyz

================================================================================
来源：http://ejs.gogol.net.cn

[U01] Py：创建虚拟环境
来源：http://hoo.zdbjq.cn

python -m venv .venv && source .venv/bin/activate
来源：http://vyc.yangfankeji.com

[U02] Py：导出 / 安装依赖
来源：http://orr.jqgfzy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://quk.jlsjyb.cn

[U03] Py：加载 .env 配置
来源：http://myj.yj20258.top

from dotenv import load_dotenv; load_dotenv()
来源：http://zlq.yangfankeji.com

[U04] Py：变量调试打印
来源：http://uot.zycfv.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kox.zhixingplan.top

[U05] Py：列表去重且保序
来源：http://zsn.xylfe.cn

list(dict.fromkeys(arr))
来源：http://amj.tarul.cn

[U06] Py：合并两个字典
来源：http://eed.ydzc1.top

{**a, **b}
来源：http://vyc.quarkkingdee.top

[U07] Py：反转字典键值
来源：http://dcs.meibo888.top

{v: k for k, v in d.items()}
来源：http://xmw.nwbrower.top

[U08] Py：展平二维列表
来源：http://anz.tianlin.xyz

[y for x in nested for y in x]
来源：http://ilj.tianlin.xyz

[U09] Py：字典取最大值的键
来源：http://aig.zhengqikj.top

max(d, key=d.get)
来源：http://zcm.haohaochexian.top

[U10] Py：按值排序字典
来源：http://gll.shanyushiyangkeji.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kbs.shanyushiyangtech.top

[U11] Py：生成器表达式
来源：http://nje.vehdjk.com

(x * 2 for x in arr)
来源：http://oee.ydzc1.top

[U12] Py：取出现最多的 3 个元素
来源：http://sed.mhx1999.top

Counter(arr).most_common(3)
来源：http://acc.yfazqb.com

[U13] Py：固定长度队列
来源：http://nvo.316326.xyz

deque(maxlen=10)
来源：http://mrd.birdmap.top

[U14] Py：分组收集到列表
来源：http://kfj.svipenyu.cn

defaultdict(list)
来源：http://mht.ydzc1.top

[U15] Py：高精度计时
来源：http://cqn.tianlin.xyz

t = time.perf_counter()
来源：http://ibo.hfpthk.cn

[U16] Py：命令行参数解析
来源：http://alg.smart0.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://uzp.jyoumei.cn

[U17] Py：初始化日志
来源：http://ebo.hcnkem.com

logging.basicConfig(level=logging.INFO)
来源：http://tpk.jinqigufen.top

[U18] Py：预编译正则
来源：http://hlh.hfpthk.cn

pat = re.compile(r"\d+")
来源：http://xwl.cdnleiting.top

[U19] Py：正则替换带回调
来源：http://lfv.shzxlz.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mpt.pengpengdd.cyou

[U20] Py：缓存函数结果
来源：http://qcf.dashuyun.cn

@functools.lru_cache(maxsize=None)
来源：http://ajj.gzhubu.top

[U21] Py：自定义上下文管理器
来源：http://yst.zhengqikj.top

@contextlib.contextmanager
来源：http://das.fanxiaobao.xyz

[U22] Py：矩阵转置
来源：http://rls.yj20258888.top

list(zip(*m))
来源：http://swp.yueranfly.top

[U23] Py：分块读取大文件
来源：http://lcp.pengpengdd.cyou

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fag.tanke756.top

[U24] Py：路径操作
来源：http://lqn.jinyuanbaomall.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://uzx.xinyue.icu

[U25] Py：CSV 按字典读
来源：http://fxp.tanke756.top

csv.DictReader(f)
来源：http://hqy.guowangkeji.top

[U26] Py：并发下载
来源：http://gok.iojbl.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pad.andypj.xyz

[U27] Py：异步 HTTP
来源：http://fcw.chenzaomai.com

aiohttp.ClientSession() 配合 async with
来源：http://vda.ivvv.top

[U28] Py：类型别名
来源：http://mdv.jiagoushi.top

UserId = int
来源：http://osf.nanxuanxn.top

[U29] Py：属性校验
来源：http://fdi.316326.xyz

@property 与 @x.setter 配合
来源：http://gky.fengsongda.top

[U30] Py：数据类
来源：http://kga.feifeiyinyue.top

@dataclass(slots=True)
来源：http://cli.zhengqikj.top

[U31] Py：单测
来源：http://olo.tian-w.cn

python -m pytest -q
来源：http://pka.c1oappe.top

[U32] Py：代码格式化
来源：http://jup.bjfxy.top

ruff format . && ruff check --fix .
来源：http://vpc.svipenyu.cn

[U33] Py：打包发布
来源：http://svl.pycfn.com

python -m build  （依赖 pyproject.toml）
来源：http://jmm.chenjidiqi.icu

[U34] Py：判断编码
来源：http://iye.tian-w.cn

chardet.detect(raw)
来源：http://obr.xingfuxueyuan.xyz

[U35] Py：发送邮件
来源：http://xdu.zycfv.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://odc.zhiwuduotai.top

[U36] Py：定时任务
来源：http://vnd.zhengqikj.top

schedule.every(10).minutes.do(job)
来源：http://twa.jinyuanbaomall.cn

[U37] Py：读写 Excel
来源：http://tfk.jqgfzy.top

pandas.read_excel / DataFrame.to_excel
来源：http://aki.sjlbkw.cn

[U38] Py：获取脚本所在目录
来源：http://ctj.chenjidiqi.icu

Path(__file__).resolve().parent
来源：http://ccx.xuetiantiany.cn

[U39] Py：判断是否在交互环境
来源：http://jll.dianchejie.cn

sys.stdout.isatty()
来源：http://cdu.tarul.cn

[U40] Py：打印到标准错误
来源：http://auu.svipenyu.cn

print("err", file=sys.stderr)
来源：http://phz.yvedp.cn

[U41] PHP：初始化 Composer 项目
来源：http://yfg.andypj.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://xye.fengsongda.top

[U42] PHP：PSR-4 自动加载
来源：http://qns.hesvh.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://frn.zhijiandao.cn

[U43] PHP：声明命名空间
来源：http://tlf.hcnkem.com

namespace App\Http;
来源：http://auf.yj202588.top

[U44] PHP：开启严格类型
来源：http://vhi.xinyue.icu

declare(strict_types=1);
来源：http://stf.sjlbkw.cn

[U45] PHP：类型声明与返回类型
来源：http://oag.jinghuilouyu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://dsh.chenjidiqi.icu

[U46] PHP：可空类型
来源：http://ovg.chenjidiqi.icu

?string $name = null
来源：http://unm.hfpthk.cn

[U47] PHP：联合类型
来源：http://vno.xziqi.cn

int|string $id
来源：http://kfj.yuanzhike.top

[U48] PHP：纯枚举
来源：http://tzq.hcnkem.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qvl.cdnleiting.top

[U49] PHP：只读属性
来源：http://wlj.tarul.cn

public readonly string $name
来源：http://ivp.iojbl.cn

[U50] PHP：构造器属性提升
来源：http://yaj.shuidangran.top

public function __construct(private int $id) {}
来源：http://qyn.gaohongyu789.top

[U51] PHP：数组解构
来源：http://dnf.nanxuanxn.top

[$a, $b] = $arr;
来源：http://wul.yuxming.cn

[U52] PHP：箭头函数
来源：http://evf.wangdashe.top

$double = fn($x) => $x * 2;
来源：http://amo.nanxinkj.top

[U53] PHP：空合并运算符
来源：http://rmj.aibaodan.cn

$v = $a ?? $b ?? "default";
来源：http://llk.mhx1999.top

[U54] PHP：空安全调用
来源：http://sgb.hcnkem.com

$obj?->method()
来源：http://tjo.zhixingplan.top

[U55] PHP：match 表达式
来源：http://irr.sjlbkw.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://udp.yvedp.cn

[U56] PHP：命名参数
来源：http://wlx.shzxlz.cn

f(a: 1, b: 2)
来源：http://zju.smart0.xyz

[U57] PHP：字符串插值
来源：http://bql.fktsv.cn

"值: {$a}"
来源：http://ktg.gaohongyu789.top

[U58] PHP：数组三件套
来源：http://lhh.xylfe.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://sdo.gotoacloud.top

[U59] PHP：自定义排序
来源：http://zto.jinyuanbaomall.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://won.jinqigfzy.top

[U60] PHP：JSON 编解码
来源：http://fhc.yanxiufei.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lsu.aibaodan.cn

[U61] PHP：正则
来源：http://zqu.gotoacloud.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://uax.316326.xyz

[U62] PHP：日期对象
来源：http://hxe.gogol.net.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hqx.yuxming.cn

[U63] PHP：文件读写
来源：http://fxs.jqgfzy.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://enf.ppjwa.cn

[U64] PHP：目录遍历
来源：http://ckm.quarkkingdee.top

glob("dir/*.php");  scandir("dir");
来源：http://ozw.kuanghao11.cn

[U65] PHP：会话
来源：http://ukq.pengpengdd.cyou

session_start();  $_SESSION["uid"] = 1;
来源：http://uoz.feifeiyinyue.top

[U66] PHP：设置 Cookie
来源：http://zdv.zdbjq.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xsr.zhijiandao.cn

[U67] PHP：处理文件上传
来源：http://bih.yonumen.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://axg.vqdsnc.cn

[U68] PHP：PDO 连接
来源：http://ftp.zhongyouzk.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zjq.pengpengdd.cyou

[U69] PHP：PDO 预处理
来源：http://crl.jqgufenzy.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://owm.daxiang520.top

[U70] PHP：PDO 事务
来源：http://jns.c1oappe.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fjh.zycfv.cn

[U71] PHP：抛出异常
来源：http://cws.ybcxt.top

throw new RuntimeException("失败", 500);
来源：http://ydh.tianlin.xyz

[U72] PHP：写错误日志
来源：http://gti.zhiwuduotai.top

error_log("失败: " . $e->getMessage());
来源：http://cug.epnwcf.com

[U73] PHP：读取 ini 配置
来源：http://afl.uphjek.com

parse_ini_file("config.ini", true)
来源：http://pbp.guowangkeji.top

[U74] PHP：读取环境变量
来源：http://jiq.feifeiyinyue.top

getenv("APP_ENV") ?: "production"
来源：http://apm.shuidangran.top

[U75] PHP：依赖注入
来源：http://fpc.chenjidiqi.icu

composer require psr/container
来源：http://ghr.ctjpmb.com

[U76] PHP：简单路由
来源：http://bzp.jqgufenzy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rca.hammf.cn

[U77] PHP：模板渲染
来源：http://rjv.zhongyouzk.top

composer require twig/twig
来源：http://www.dianchejie.cn

[U78] PHP：单元测试
来源：http://ggw.xziqi.cn

composer require --dev phpunit/phpunit
来源：http://jlz.sysykeji.top

[U79] PHP：静态分析
来源：http://qtx.zhongyouzk.top

composer require --dev phpstan/phpstan
来源：http://tkn.yj202588.top

[U80] PHP：代码规范修复
来源：http://ycd.52xcode.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://gvy.guannengcc.top

[U81] JS：初始化项目
来源：http://cxk.jianghu66.top

npm init -y;  npm i express
来源：http://tjx.hnqzz.top

[U82] JS：package.json 脚本
来源：http://krl.yonumen.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ohm.vehdjk.com

[U83] JS：ES Module 导入导出
来源：http://ieu.jlsjyb.cn

export const a = 1;  import { a } from "./m.js";
来源：http://xmv.jlsjyb.cn

[U84] JS：CommonJS 写法
来源：http://zti.pycfn.com

module.exports = { a };  const { a } = require("./m");
来源：http://isx.bbcook.cn

[U85] JS：可选链
来源：http://ttj.zdbjq.cn

a?.b?.c
来源：http://aqp.ehwqpu.com

[U86] JS：空值合并
来源：http://vtk.gotoacloud.top

a ?? b
来源：http://cos.redwolf501.top

[U87] JS：解构默认值
来源：http://htz.fanxiaobao.xyz

const { a = 1, b = 2 } = obj;
来源：http://dqs.c1oappe.top

[U88] JS：对象展开合并
来源：http://hyx.havefunace.top

{ ...a, ...b }
来源：http://xxd.ctjpmb.com

[U89] JS：数组去重
来源：http://inf.zhengqikj.top

[...new Set(arr)]
来源：http://shb.snrcjt.cn

[U90] JS：数字数组排序
来源：http://smh.yongpay.top

[...arr].sort((a, b) => a - b)
来源：http://dus.shuidangran.top

[U91] JS：对象键值遍历
来源：http://gca.jyoumei.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://sjs.wangshuangyany.cn

[U92] JS：深拷贝
来源：http://zex.nwbrower.top

structuredClone(obj)
来源：http://oyn.pengpengdd.cyou

[U93] JS：模板字符串
来源：http://djo.smart0.xyz

`共 ${n} 条`
来源：http://jzo.yanxiufei.cn

[U94] JS：箭头函数
来源：http://dsa.feifeiyinyue.top

const double = x => x * 2;
来源：http://bcb.havefunace.top

[U95] JS：Promise 包装
来源：http://cbj.nanxuanxn.top

new Promise((resolve, reject) => {})
来源：http://scp.yueranfly.top

[U96] JS：async/await 与异常
来源：http://uwo.316326.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ilo.zhongyouzk.top

[U97] JS：并发请求
来源：http://mws.zhixingplan.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://jfr.chenzaomai.com

[U98] JS：fetch 带 JSON
来源：http://usf.cheryme.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wqf.birdmap.top

[U99] JS：事件监听
来源：http://ztv.shangyingyoupin.top

el.addEventListener("click", e => {})
来源：http://bue.9152youxi.cn

[U100] JS：DOM 查询
来源：http://xhy.cheryme.top

document.querySelector(".item")
来源：http://jlm.ybcxt.top

[U101] JS：classList 操作
来源：http://tbu.ivvv.top

el.classList.toggle("active")
来源：http://xjr.ywan-chungtsiang.top

[U102] JS：本地存储
来源：http://uue.zdbjq.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://dan.gotoacloud.top

[U103] JS：定时器
来源：http://tfw.ivvv.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yqq.jqgfzy.top

[U104] JS：防抖
来源：http://tov.shanyushiyangkeji.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qjt.tarul.cn

[U105] JS：节流
来源：http://wgc.52xcode.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://eon.jinyuanbaomall.cn

[U106] JS：日期格式化
来源：http://fgl.yonumen.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pts.mhx1999.top

[U107] JS：数字千分位
来源：http://ydr.yfazqb.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cxx.dashuyun.cn

[U108] JS：随机整数
来源：http://jjy.jinqigfzy.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gpf.shanyushiyangtech.top

[U109] JS：数组分组
来源：http://gyy.yj20258888.top

Object.groupBy(arr, x => x.type)
来源：http://woi.vqdsnc.cn

[U110] JS：数组分块
来源：http://vuk.hesvh.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pcp.ydzc1.top

[U111] JS：对象转 Map
来源：http://riq.cqqwz.cn

new Map(Object.entries(obj))
来源：http://knv.sxryk.cn

[U112] JS：字符串补位
来源：http://qfu.fengsongda.top

"7".padStart(3, "0")
来源：http://bpj.yongpay.top

[U113] JS：正则替换全部
来源：http://his.zhixingplan.top

s.replaceAll("a", "b")
来源：http://oec.tanke756.top

[U114] JS：JSON 深比较
来源：http://xsr.cdnleiting.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://iop.cheryme.top

[U115] JS：生成 UUID
来源：http://cmm.chenlongwang.top

crypto.randomUUID()
来源：http://lza.sjlbkw.cn

[U116] JS：类型检查（JSDoc）
来源：http://odg.cashguo.top

/** @param {string} name */ function f(name) {}
来源：http://xaj.jyoumei.cn

[U117] JS：单元测试
来源：http://kfh.yanxiufei.cn

npm i -D vitest;  npx vitest
来源：http://pra.jqgufenzy.top

[U118] JS：开发服务器
来源：http://pib.yueranfly.top

npm i -D vite;  npx vite
来源：http://pap.316326.xyz

[U119] JS：生产构建
来源：http://mpo.hongshengwenyu.top

npx vite build
来源：http://grb.ybcxt.top

[U120] JS：读取环境变量（Vite）
来源：http://rza.fehbvm.com

import.meta.env.VITE_API_URL
来源：http://iqo.shangyingyoupin.top

================================================================================
来源：http://lxa.pengpengdd.cyou

统计汇总
来源：http://xgr.ehwqpu.com

================================================================================
来源：http://lzc.hammf.cn

按语言统计（条）：
来源：http://zhh.jianghu66.top

Python ......... 252
来源：http://tng.quarkkingdee.top

PHP ............ 252
来源：http://ueu.vqdsnc.cn

JavaScript ..... 252
来源：http://wdp.ehwqpu.com

TypeScript ..... 212
来源：http://hkk.ydzc1.top

Java ........... 212
来源：http://ubc.guowangkeji.top

Go ............. 212
来源：http://hsb.hammf.cn

Ruby ........... 212
来源：http://tlh.hfpthk.cn

C# ............. 212
来源：http://fte.ywan-chungtsiang.top

C .............. 30
来源：http://bvq.wangshuangyany.cn

C++ ............ 30
来源：http://bnr.birdmap.top

SQL ............ 90
来源：http://bga.gzhubu.top

Bash ........... 80
来源：http://wkg.zhongyouzk.top

Kotlin ......... 15
来源：http://mcn.zhijiandao.cn

Swift .......... 15
来源：http://zzq.haohaochexian.top

Lua ............ 10
来源：http://sjx.havefunace.top

Perl ........... 10
来源：http://gzz.chenzaomai.com


<!-- 参考信息 -->