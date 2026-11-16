代发 wailian999

[T43] Perl：字符串插值
来源：http://xnb.yj202588.top

"值: $a"
来源：http://zfh.havefunace.top

[T44] Perl：条件
来源：http://zjw.gaohongyu789.top

if ($a > 0) { print "正"; }
来源：http://wnu.hesvh.cn

[T45] Perl：数组遍历
来源：http://kie.zhaomingkeji.xyz

for my $x (@arr) { print $x; }
来源：http://wfa.zhijiandao.cn

[T46] Perl：哈希操作
来源：http://kso.dashuyun.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fkp.mhx1999.top

[T47] Perl：正则捕获
来源：http://nls.yfazqb.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://ffj.nwbrower.top

[T48] Perl：正则替换
来源：http://hwj.nanxinkj.top

$s =~ s/old/new/g;
来源：http://yfd.hnxiangtu.top

[T49] Perl：函数
来源：http://her.jianghu66.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ihe.snrcjt.cn

[T50] Perl：逐行读文件
来源：http://fyd.jianghu66.top

open my $fh, "<", "a.txt" or die $!;
来源：http://yov.zhongyouzk.top

while (my $line = <$fh>) { print $line; }
来源：http://bid.xinyue.icu

[T51] Scala：Hello World
来源：http://zii.aizwys.cn

println("Hello")
来源：http://did.pengpengdd.cyou

[T52] Scala：变量
来源：http://vac.hnqzz.top

val a = 1;  var b = 2
来源：http://adv.zhengqikj.top

[T53] Scala：字符串插值
来源：http://oyh.xylfe.cn

s"值: $b"
来源：http://ike.jianghu66.top

[T54] Scala：集合映射
来源：http://ntp.shuidangran.top

List(1, 2, 3).map(_ * 2)
来源：http://gza.ehwqpu.com

[T55] Scala：集合过滤
来源：http://ctr.svipenyu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://lwg.aizwys.cn

[T56] Scala：样例类
来源：http://unq.chenjidiqi.icu

case class User(name: String, age: Int)
来源：http://jhi.shuidangran.top

[T57] Scala：模式匹配
来源：http://irb.ppjwa.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vhe.zhiwuduotai.top

[T58] Scala：函数定义
来源：http://otu.feifeiyinyue.top

def add(a: Int, b: Int): Int = a + b
来源：http://guz.sysykeji.top

[T59] Scala：循环
来源：http://uzh.vehdjk.com

for (i <- 1 to 10) println(i)
来源：http://mhf.yonumen.top

[T60] Scala：折叠
来源：http://run.ybcxt.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dxx.tianlin.xyz

================================================================================
来源：http://kob.dianchejie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cdi.hywenlv.cn

================================================================================
来源：http://bdx.cqqwz.cn

[U01] Py：创建虚拟环境
来源：http://lyd.nanxinkj.top

python -m venv .venv && source .venv/bin/activate
来源：http://dri.fengsongda.top

[U02] Py：导出 / 安装依赖
来源：http://huk.fzhhl.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ylt.yfazqb.com

[U03] Py：加载 .env 配置
来源：http://inh.tianlin.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://bxc.fehbvm.com

[U04] Py：变量调试打印
来源：http://tro.jiagoushi.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fam.jinghuilouyu.cn

[U05] Py：列表去重且保序
来源：http://yeb.hnxiangtu.top

list(dict.fromkeys(arr))
来源：http://kqy.yueranfly.top

[U06] Py：合并两个字典
来源：http://jfd.jianghu66.top

{**a, **b}
来源：http://lmh.guowangkeji.top

[U07] Py：反转字典键值
来源：http://znh.zdbjq.cn

{v: k for k, v in d.items()}
来源：http://ekd.wangdashe.top

[U08] Py：展平二维列表
来源：http://vku.nanxinkj.top

[y for x in nested for y in x]
来源：http://tar.cdnleiting.top

[U09] Py：字典取最大值的键
来源：http://ona.haohaochexian.top

max(d, key=d.get)
来源：http://nnc.redwolf501.top

[U10] Py：按值排序字典
来源：http://aej.quarkkingdee.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mca.daria6918.cn

[U11] Py：生成器表达式
来源：http://vdb.kuanghao11.cn

(x * 2 for x in arr)
来源：http://lns.snrcjt.cn

[U12] Py：取出现最多的 3 个元素
来源：http://nvh.yanxiufei.cn

Counter(arr).most_common(3)
来源：http://gia.xylfe.cn

[U13] Py：固定长度队列
来源：http://mjs.epnwcf.com

deque(maxlen=10)
来源：http://lgc.jqgfzy.top

[U14] Py：分组收集到列表
来源：http://tgb.sweek.top

defaultdict(list)
来源：http://bho.svipenyu.cn

[U15] Py：高精度计时
来源：http://dso.sxryk.cn

t = time.perf_counter()
来源：http://gud.havefunace.top

[U16] Py：命令行参数解析
来源：http://xgv.shanyushiyangtech.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yby.jianghu66.top

[U17] Py：初始化日志
来源：http://rol.nanxinkj.top

logging.basicConfig(level=logging.INFO)
来源：http://fzf.hesvh.cn

[U18] Py：预编译正则
来源：http://est.vehdjk.com

pat = re.compile(r"\d+")
来源：http://gyz.kuanghao11.cn

[U19] Py：正则替换带回调
来源：http://fjv.yj20258888.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fec.hnqzz.top

[U20] Py：缓存函数结果
来源：http://mod.zhijiandao.cn

@functools.lru_cache(maxsize=None)
来源：http://foc.ydjk.org.cn

[U21] Py：自定义上下文管理器
来源：http://xuv.yanxiufei.cn

@contextlib.contextmanager
来源：http://zpf.zhijiandao.cn

[U22] Py：矩阵转置
来源：http://axr.zhixingplan.top

list(zip(*m))
来源：http://aqq.ydzc1.top

[U23] Py：分块读取大文件
来源：http://rga.meibo888.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fsw.ybcxt.top

[U24] Py：路径操作
来源：http://mxw.jqgfzy.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://who.guannengcc.top

[U25] Py：CSV 按字典读
来源：http://lrw.nanxinkj.top

csv.DictReader(f)
来源：http://goz.jlsjyb.cn

[U26] Py：并发下载
来源：http://joq.uphjek.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://cgf.fengsongda.top

[U27] Py：异步 HTTP
来源：http://lpv.shangyingyoupin.top

aiohttp.ClientSession() 配合 async with
来源：http://vyv.fzhhl.top

[U28] Py：类型别名
来源：http://dmu.ydzc1.top

UserId = int
来源：http://yzr.ywan-chungtsiang.top

[U29] Py：属性校验
来源：http://vsl.9152youxi.cn

@property 与 @x.setter 配合
来源：http://vgw.daria6918.cn

[U30] Py：数据类
来源：http://doe.9152youxi.cn

@dataclass(slots=True)
来源：http://jnj.yj20258.top

[U31] Py：单测
来源：http://gjc.yangfankeji.com

python -m pytest -q
来源：http://htv.quarkkingdee.top

[U32] Py：代码格式化
来源：http://haa.sweek.top

ruff format . && ruff check --fix .
来源：http://nid.mhx1999.top

[U33] Py：打包发布
来源：http://fhg.uphjek.com

python -m build  （依赖 pyproject.toml）
来源：http://wgb.pengpengdd.cyou

[U34] Py：判断编码
来源：http://hrc.jiagoushi.top

chardet.detect(raw)
来源：http://ahl.sweek.top

[U35] Py：发送邮件
来源：http://hul.bbcook.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://upe.bjfxy.top

[U36] Py：定时任务
来源：http://ctw.yj20258.top

schedule.every(10).minutes.do(job)
来源：http://wbl.jinghuilouyu.cn

[U37] Py：读写 Excel
来源：http://bpa.fktsv.cn

pandas.read_excel / DataFrame.to_excel
来源：http://pmx.jinyuanbaomall.cn

[U38] Py：获取脚本所在目录
来源：http://lqf.zhoulong.xyz

Path(__file__).resolve().parent
来源：http://aje.zdqjudy.top

[U39] Py：判断是否在交互环境
来源：http://coj.vehdjk.com

sys.stdout.isatty()
来源：http://cwh.zdbjq.cn

[U40] Py：打印到标准错误
来源：http://men.cqqwz.cn

print("err", file=sys.stderr)
来源：http://hwv.tianlin.xyz

[U41] PHP：初始化 Composer 项目
来源：http://ewd.zdbjq.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://kpq.sjlbkw.cn

[U42] PHP：PSR-4 自动加载
来源：http://xnw.ppjwa.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://iut.yueranfly.top

[U43] PHP：声明命名空间
来源：http://wgt.andypj.xyz

namespace App\Http;
来源：http://dxw.xingfuxueyuan.xyz

[U44] PHP：开启严格类型
来源：http://vpi.nwbrower.top

declare(strict_types=1);
来源：http://jpo.jinqigufen.top

[U45] PHP：类型声明与返回类型
来源：http://rrl.cucudq.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://xdf.hcnkem.com

[U46] PHP：可空类型
来源：http://tpz.cheryme.top

?string $name = null
来源：http://jfi.redwolf501.top

[U47] PHP：联合类型
来源：http://ahn.zhoulong.xyz

int|string $id
来源：http://ory.hongshengwenyu.top

[U48] PHP：纯枚举
来源：http://csm.fengsongda.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vel.hywenlv.cn

[U49] PHP：只读属性
来源：http://vps.redwolf501.top

public readonly string $name
来源：http://qoy.daria6918.cn

[U50] PHP：构造器属性提升
来源：http://kfa.andypj.xyz

public function __construct(private int $id) {}
来源：http://pil.hesvh.cn

[U51] PHP：数组解构
来源：http://ebc.zhijiandao.cn

[$a, $b] = $arr;
来源：http://zzx.xingfuxueyuan.xyz

[U52] PHP：箭头函数
来源：http://xrh.fengsongda.top

$double = fn($x) => $x * 2;
来源：http://qtd.ctjpmb.com

[U53] PHP：空合并运算符
来源：http://cfw.epnwcf.com

$v = $a ?? $b ?? "default";
来源：http://xad.cdnleiting.top

[U54] PHP：空安全调用
来源：http://qyu.zycfv.cn

$obj?->method()
来源：http://byi.shanyushiyangtech.top

[U55] PHP：match 表达式
来源：http://azm.daria6918.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bks.yj20258888.top

[U56] PHP：命名参数
来源：http://cmt.nanxinkj.top

f(a: 1, b: 2)
来源：http://mlo.daxiang520.top

[U57] PHP：字符串插值
来源：http://uwx.fzhhl.top

"值: {$a}"
来源：http://ryf.tianlin.xyz

[U58] PHP：数组三件套
来源：http://vps.jinqigufen.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fgo.cashguo.top

[U59] PHP：自定义排序
来源：http://egu.ppjwa.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ddk.kuanghao11.cn

[U60] PHP：JSON 编解码
来源：http://bpc.wangshuangyany.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jzi.zhaomingkeji.xyz

[U61] PHP：正则
来源：http://hsm.fzhhl.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://opf.cashguo.top

[U62] PHP：日期对象
来源：http://bad.xuetiantiany.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://dwj.jlsjyb.cn

[U63] PHP：文件读写
来源：http://wwm.ywan-chungtsiang.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bub.jinyuanbaomall.cn

[U64] PHP：目录遍历
来源：http://srp.hnqzz.top

glob("dir/*.php");  scandir("dir");
来源：http://yir.c1oappe.top

[U65] PHP：会话
来源：http://ejz.cheryme.top

session_start();  $_SESSION["uid"] = 1;
来源：http://nbv.hywenlv.cn

[U66] PHP：设置 Cookie
来源：http://umb.sxryk.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pvk.quarkkingdee.top

[U67] PHP：处理文件上传
来源：http://aah.pycfn.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://usn.shuidangran.top

[U68] PHP：PDO 连接
来源：http://tbp.ydjk.org.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pap.yfazqb.com

[U69] PHP：PDO 预处理
来源：http://ozg.xylfe.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://pwy.ywan-chungtsiang.top

[U70] PHP：PDO 事务
来源：http://egw.birdmap.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ese.epnwcf.com

[U71] PHP：抛出异常
来源：http://epu.kuanghao11.cn

throw new RuntimeException("失败", 500);
来源：http://ocv.gogol.net.cn

[U72] PHP：写错误日志
来源：http://oxa.snrcjt.cn

error_log("失败: " . $e->getMessage());
来源：http://lkg.ppjwa.cn

[U73] PHP：读取 ini 配置
来源：http://kgt.svipenyu.cn

parse_ini_file("config.ini", true)
来源：http://dth.xziqi.cn

[U74] PHP：读取环境变量
来源：http://mdk.nwbrower.top

getenv("APP_ENV") ?: "production"
来源：http://zoe.jinqigfzy.top

[U75] PHP：依赖注入
来源：http://dsl.vqdsnc.cn

composer require psr/container
来源：http://hiu.yj202588.top

[U76] PHP：简单路由
来源：http://jwj.cdnleiting.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ejo.zdqjudy.top

[U77] PHP：模板渲染
来源：http://aay.zhiwuduotai.top

composer require twig/twig
来源：http://nse.ctjpmb.com

[U78] PHP：单元测试
来源：http://tar.vqdsnc.cn

composer require --dev phpunit/phpunit
来源：http://pzx.aibaodan.cn

[U79] PHP：静态分析
来源：http://kuq.hnxiangtu.top

composer require --dev phpstan/phpstan
来源：http://obg.yangfankeji.com

[U80] PHP：代码规范修复
来源：http://zbe.ybcxt.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://wpn.tian-w.cn

[U81] JS：初始化项目
来源：http://kkc.cheryme.top

npm init -y;  npm i express
来源：http://rjw.yuxming.cn

[U82] JS：package.json 脚本
来源：http://uac.tian-w.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fsn.xylfe.cn

[U83] JS：ES Module 导入导出
来源：http://oia.316326.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://uvl.tianlin.xyz

[U84] JS：CommonJS 写法
来源：http://izp.wangdashe.top

module.exports = { a };  const { a } = require("./m");
来源：http://lpx.ehwqpu.com

[U85] JS：可选链
来源：http://cqu.zycfv.cn

a?.b?.c
来源：http://nec.cheryme.top

[U86] JS：空值合并
来源：http://dcc.shanyushiyangtech.top

a ?? b
来源：http://loe.ydzc1.top

[U87] JS：解构默认值
来源：http://jem.bbcook.cn

const { a = 1, b = 2 } = obj;
来源：http://oda.jiagoushi.top

[U88] JS：对象展开合并
来源：http://bas.xuanzx.com

{ ...a, ...b }
来源：http://yqz.iojbl.cn

[U89] JS：数组去重
来源：http://jhc.jqgufenzy.top

[...new Set(arr)]
来源：http://oln.chenlongwang.top

[U90] JS：数字数组排序
来源：http://uts.sjlbkw.cn

[...arr].sort((a, b) => a - b)
来源：http://vpr.xuetiantiany.cn

[U91] JS：对象键值遍历
来源：http://gec.hcnkem.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nqq.aibaodan.cn

[U92] JS：深拷贝
来源：http://ifi.jinqigfzy.top

structuredClone(obj)
来源：http://snq.hfpthk.cn

[U93] JS：模板字符串
来源：http://ogd.mhx1999.top

`共 ${n} 条`
来源：http://uil.sufxvd.cn

[U94] JS：箭头函数
来源：http://fwz.ywan-chungtsiang.top

const double = x => x * 2;
来源：http://jzj.wangdashe.top

[U95] JS：Promise 包装
来源：http://ocu.yonumen.top

new Promise((resolve, reject) => {})
来源：http://zln.bjfxy.top

[U96] JS：async/await 与异常
来源：http://gpj.yanxiufei.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://oxl.guannengcc.top

[U97] JS：并发请求
来源：http://inw.haohaochexian.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://skm.mhx1999.top

[U98] JS：fetch 带 JSON
来源：http://dzj.jiagoushi.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zbz.daxiang520.top

[U99] JS：事件监听
来源：http://mws.yonumen.top

el.addEventListener("click", e => {})
来源：http://xed.yj202588.top

[U100] JS：DOM 查询
来源：http://wli.xuetiantiany.cn

document.querySelector(".item")
来源：http://vdl.ctjpmb.com

[U101] JS：classList 操作
来源：http://xly.xuanzx.com

el.classList.toggle("active")
来源：http://zhp.iojbl.cn

[U102] JS：本地存储
来源：http://fwe.tianlin.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://pqr.yueranfly.top

[U103] JS：定时器
来源：http://kmn.xinyue.icu

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tnc.9152youxi.cn

[U104] JS：防抖
来源：http://hha.sufxvd.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tcz.zdbjq.cn

[U105] JS：节流
来源：http://zqa.shangyingyoupin.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://azu.hfpthk.cn

[U106] JS：日期格式化
来源：http://szf.jianghu66.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://omn.aibaodan.cn

[U107] JS：数字千分位
来源：http://voj.sufxvd.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zcz.jlsjyb.cn

[U108] JS：随机整数
来源：http://uib.xuetiantiany.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bst.cheryme.top

[U109] JS：数组分组
来源：http://njf.fanxiaobao.xyz

Object.groupBy(arr, x => x.type)
来源：http://iio.chenlongwang.top

[U110] JS：数组分块
来源：http://dfc.nwbrower.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dbd.zhongyouzk.top

[U111] JS：对象转 Map
来源：http://vtw.bbcook.cn

new Map(Object.entries(obj))
来源：http://gpf.cucudq.cn

[U112] JS：字符串补位
来源：http://iwe.yj20258888.top

"7".padStart(3, "0")
来源：http://jqc.svipenyu.cn

[U113] JS：正则替换全部
来源：http://vnc.shuidangran.top

s.replaceAll("a", "b")
来源：http://czw.fzhhl.top

[U114] JS：JSON 深比较
来源：http://prr.daria6918.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://nlu.svipenyu.cn

[U115] JS：生成 UUID
来源：http://wpg.havefunace.top

crypto.randomUUID()
来源：http://cpc.52xcode.cn

[U116] JS：类型检查（JSDoc）
来源：http://prb.zhiwuduotai.top

/** @param {string} name */ function f(name) {}
来源：http://qqa.andypj.xyz

[U117] JS：单元测试
来源：http://nft.yangfankeji.com

npm i -D vitest;  npx vitest
来源：http://gxa.52xcode.cn

[U118] JS：开发服务器
来源：http://qpu.wangdashe.top

npm i -D vite;  npx vite
来源：http://nlh.pengpengdd.cyou

[U119] JS：生产构建
来源：http://oea.c1oappe.top

npx vite build
来源：http://fzc.svipenyu.cn

[U120] JS：读取环境变量（Vite）
来源：http://iju.cheryme.top

import.meta.env.VITE_API_URL
来源：http://hvv.yuxming.cn

================================================================================
来源：http://afz.dianchejie.cn

统计汇总
来源：http://eec.jqgufenzy.top

================================================================================
来源：http://idm.cqqwz.cn

按语言统计（条）：
来源：http://ywh.xylfe.cn

Python ......... 252
来源：http://pnh.hfpthk.cn

PHP ............ 252
来源：http://tte.fehbvm.com

JavaScript ..... 252
来源：http://vsi.jinghuilouyu.cn

TypeScript ..... 212
来源：http://ccm.jinyuanbaomall.cn

Java ........... 212
来源：http://hvk.jiagoushi.top

Go ............. 212
来源：http://rei.jinghuilouyu.cn

Ruby ........... 212
来源：http://xks.nanxinkj.top

C# ............. 212
来源：http://eng.ydjk.org.cn

C .............. 30
来源：http://rdg.9152youxi.cn

C++ ............ 30
来源：http://pnr.xingfuxueyuan.xyz

SQL ............ 90
来源：http://cik.jinqigfzy.top

Bash ........... 80
来源：http://tmx.yuxming.cn

Kotlin ......... 15
来源：http://mvg.pycfn.com

Swift .......... 15
来源：http://qjz.yangfankeji.com

Lua ............ 10
来源：http://ewc.sjlbkw.cn

Perl ........... 10
来源：http://lyg.snrcjt.cn


<!-- 参考信息 -->