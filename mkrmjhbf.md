代发 wailian999

[U05] Py：列表去重且保序
来源：http://ocj.hywenlv.cn

list(dict.fromkeys(arr))
来源：http://pyj.fanxiaobao.xyz

[U06] Py：合并两个字典
来源：http://bok.birdmap.top

{**a, **b}
来源：http://nzj.tianlin.xyz

[U07] Py：反转字典键值
来源：http://gva.birdmap.top

{v: k for k, v in d.items()}
来源：http://eho.tanke756.top

[U08] Py：展平二维列表
来源：http://ypc.shanyushiyangtech.top

[y for x in nested for y in x]
来源：http://pov.snrcjt.cn

[U09] Py：字典取最大值的键
来源：http://avi.nanxinkj.top

max(d, key=d.get)
来源：http://dwk.jianghu66.top

[U10] Py：按值排序字典
来源：http://alj.yj20258.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://oul.xuetiantiany.cn

[U11] Py：生成器表达式
来源：http://enx.c1oappe.top

(x * 2 for x in arr)
来源：http://cjg.yfazqb.com

[U12] Py：取出现最多的 3 个元素
来源：http://mcd.gotoacloud.top

Counter(arr).most_common(3)
来源：http://lyk.bjfxy.top

[U13] Py：固定长度队列
来源：http://lpn.pengpengdd.cyou

deque(maxlen=10)
来源：http://bbn.zycfv.cn

[U14] Py：分组收集到列表
来源：http://wzx.shanyushiyangtech.top

defaultdict(list)
来源：http://rbs.hnqzz.top

[U15] Py：高精度计时
来源：http://mhp.gaohongyu789.top

t = time.perf_counter()
来源：http://idm.bjfxy.top

[U16] Py：命令行参数解析
来源：http://nya.jqgfzy.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fpa.shangyingyoupin.top

[U17] Py：初始化日志
来源：http://gev.shangyingyoupin.top

logging.basicConfig(level=logging.INFO)
来源：http://xmk.0kj1m.cn

[U18] Py：预编译正则
来源：http://xzk.ywan-chungtsiang.top

pat = re.compile(r"\d+")
来源：http://msq.fanxiaobao.xyz

[U19] Py：正则替换带回调
来源：http://gex.haohaochexian.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fqq.daria6918.cn

[U20] Py：缓存函数结果
来源：http://kww.316326.xyz

@functools.lru_cache(maxsize=None)
来源：http://uko.fengsongda.top

[U21] Py：自定义上下文管理器
来源：http://uzf.epnwcf.com

@contextlib.contextmanager
来源：http://vce.fengsongda.top

[U22] Py：矩阵转置
来源：http://dwj.yfazqb.com

list(zip(*m))
来源：http://dlj.jlsjyb.cn

[U23] Py：分块读取大文件
来源：http://ett.vehdjk.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fax.vqdsnc.cn

[U24] Py：路径操作
来源：http://ban.zhaomingkeji.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jxw.cdnleiting.top

[U25] Py：CSV 按字典读
来源：http://grb.birdmap.top

csv.DictReader(f)
来源：http://siq.daria6918.cn

[U26] Py：并发下载
来源：http://kfc.iojbl.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://klx.yangfankeji.com

[U27] Py：异步 HTTP
来源：http://asx.yj202588.top

aiohttp.ClientSession() 配合 async with
来源：http://tmb.shangyingyoupin.top

[U28] Py：类型别名
来源：http://mgj.cashguo.top

UserId = int
来源：http://yxf.daria6918.cn

[U29] Py：属性校验
来源：http://los.c1oappe.top

@property 与 @x.setter 配合
来源：http://unf.jinghuilouyu.cn

[U30] Py：数据类
来源：http://oqm.ehwqpu.com

@dataclass(slots=True)
来源：http://drz.zhengqikj.top

[U31] Py：单测
来源：http://sfh.wangdashe.top

python -m pytest -q
来源：http://eor.yj20258888.top

[U32] Py：代码格式化
来源：http://wtr.yanxiufei.cn

ruff format . && ruff check --fix .
来源：http://con.sxryk.cn

[U33] Py：打包发布
来源：http://wcl.vqdsnc.cn

python -m build  （依赖 pyproject.toml）
来源：http://lur.gzhubu.top

[U34] Py：判断编码
来源：http://czr.ppjwa.cn

chardet.detect(raw)
来源：http://aml.dashuyun.cn

[U35] Py：发送邮件
来源：http://ijo.dashuyun.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jfj.jqgufenzy.top

[U36] Py：定时任务
来源：http://nxw.meibo888.top

schedule.every(10).minutes.do(job)
来源：http://pbn.redwolf501.top

[U37] Py：读写 Excel
来源：http://bvd.zhongyouzk.top

pandas.read_excel / DataFrame.to_excel
来源：http://uie.9152youxi.cn

[U38] Py：获取脚本所在目录
来源：http://qym.aizwys.cn

Path(__file__).resolve().parent
来源：http://yfo.shzxlz.cn

[U39] Py：判断是否在交互环境
来源：http://rzz.yj20258.top

sys.stdout.isatty()
来源：http://spu.ydjk.org.cn

[U40] Py：打印到标准错误
来源：http://qce.meibo888.top

print("err", file=sys.stderr)
来源：http://bux.xinyue.icu

[U41] PHP：初始化 Composer 项目
来源：http://klh.jqgfzy.top

composer init;  composer require guzzlehttp/guzzle
来源：http://bit.yvedp.cn

[U42] PHP：PSR-4 自动加载
来源：http://mro.9152youxi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tie.tanke756.top

[U43] PHP：声明命名空间
来源：http://xmm.hnqzz.top

namespace App\Http;
来源：http://yuu.havefunace.top

[U44] PHP：开启严格类型
来源：http://hxm.cdnleiting.top

declare(strict_types=1);
来源：http://ukb.hammf.cn

[U45] PHP：类型声明与返回类型
来源：http://wgc.pycfn.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://zwk.jqgfzy.top

[U46] PHP：可空类型
来源：http://ylh.cucudq.cn

?string $name = null
来源：http://cby.ehwqpu.com

[U47] PHP：联合类型
来源：http://bhp.jyoumei.cn

int|string $id
来源：http://nxv.cashguo.top

[U48] PHP：纯枚举
来源：http://otp.zycfv.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qps.jqgufenzy.top

[U49] PHP：只读属性
来源：http://cjf.chenlongwang.top

public readonly string $name
来源：http://huq.zdqjudy.top

[U50] PHP：构造器属性提升
来源：http://iag.xuetiantiany.cn

public function __construct(private int $id) {}
来源：http://tbt.yj20258888.top

[U51] PHP：数组解构
来源：http://lbe.ydjk.org.cn

[$a, $b] = $arr;
来源：http://wge.snrcjt.cn

[U52] PHP：箭头函数
来源：http://vuk.tianlin.xyz

$double = fn($x) => $x * 2;
来源：http://wow.jinghuilouyu.cn

[U53] PHP：空合并运算符
来源：http://xvn.jyoumei.cn

$v = $a ?? $b ?? "default";
来源：http://vwn.jinqigufen.top

[U54] PHP：空安全调用
来源：http://ndi.yj202588.top

$obj?->method()
来源：http://zoy.sufxvd.cn

[U55] PHP：match 表达式
来源：http://pzi.gotoacloud.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://aoc.zhengqikj.top

[U56] PHP：命名参数
来源：http://pck.vqdsnc.cn

f(a: 1, b: 2)
来源：http://feb.iojbl.cn

[U57] PHP：字符串插值
来源：http://uhx.jinqigufen.top

"值: {$a}"
来源：http://ggj.fktsv.cn

[U58] PHP：数组三件套
来源：http://uvy.shzxlz.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://uwa.aizwys.cn

[U59] PHP：自定义排序
来源：http://mvr.cdnleiting.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jie.yuanzhike.top

[U60] PHP：JSON 编解码
来源：http://mad.jianghu66.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://arh.guannengcc.top

[U61] PHP：正则
来源：http://saf.zdqjudy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vli.tanke756.top

[U62] PHP：日期对象
来源：http://ckk.ydjk.org.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pjj.xuanzx.com

[U63] PHP：文件读写
来源：http://jbv.tian-w.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ayt.dianchejie.cn

[U64] PHP：目录遍历
来源：http://lrg.zhijiandao.cn

glob("dir/*.php");  scandir("dir");
来源：http://ksk.hywenlv.cn

[U65] PHP：会话
来源：http://ikf.xinyue.icu

session_start();  $_SESSION["uid"] = 1;
来源：http://mnl.aizwys.cn

[U66] PHP：设置 Cookie
来源：http://iqr.redwolf501.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://trf.jyoumei.cn

[U67] PHP：处理文件上传
来源：http://psm.shuidangran.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xnx.jinqigfzy.top

[U68] PHP：PDO 连接
来源：http://sjb.smart0.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jbd.zhijiandao.cn

[U69] PHP：PDO 预处理
来源：http://jyt.yj20258.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mpt.yangfankeji.com

[U70] PHP：PDO 事务
来源：http://hkd.zhiwuduotai.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://cmk.feifeiyinyue.top

[U71] PHP：抛出异常
来源：http://lcg.ctjpmb.com

throw new RuntimeException("失败", 500);
来源：http://dni.jianghu66.top

[U72] PHP：写错误日志
来源：http://stg.jinqigfzy.top

error_log("失败: " . $e->getMessage());
来源：http://bue.jinqigufen.top

[U73] PHP：读取 ini 配置
来源：http://otf.hesvh.cn

parse_ini_file("config.ini", true)
来源：http://fse.cucudq.cn

[U74] PHP：读取环境变量
来源：http://gfh.jqgufenzy.top

getenv("APP_ENV") ?: "production"
来源：http://rzf.ydjk.org.cn

[U75] PHP：依赖注入
来源：http://ozm.ywan-chungtsiang.top

composer require psr/container
来源：http://yce.cashguo.top

[U76] PHP：简单路由
来源：http://xay.zhixingplan.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wsj.iojbl.cn

[U77] PHP：模板渲染
来源：http://shz.uphjek.com

composer require twig/twig
来源：http://hlk.fehbvm.com

[U78] PHP：单元测试
来源：http://xqm.andypj.xyz

composer require --dev phpunit/phpunit
来源：http://lgm.zhiwuduotai.top

[U79] PHP：静态分析
来源：http://mao.cdnleiting.top

composer require --dev phpstan/phpstan
来源：http://pxw.shanyushiyangtech.top

[U80] PHP：代码规范修复
来源：http://ebs.pengpengdd.cyou

composer require --dev friendsofphp/php-cs-fixer
来源：http://lyp.hammf.cn

[U81] JS：初始化项目
来源：http://onp.ivvv.top

npm init -y;  npm i express
来源：http://wjc.jyoumei.cn

[U82] JS：package.json 脚本
来源：http://djs.nwbrower.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lso.ehwqpu.com

[U83] JS：ES Module 导入导出
来源：http://hty.0kj1m.cn

export const a = 1;  import { a } from "./m.js";
来源：http://lru.yuanzhike.top

[U84] JS：CommonJS 写法
来源：http://roq.yueranfly.top

module.exports = { a };  const { a } = require("./m");
来源：http://aih.pengpengdd.cyou

[U85] JS：可选链
来源：http://ref.tianlin.xyz

a?.b?.c
来源：http://nly.hfpthk.cn

[U86] JS：空值合并
来源：http://uns.316326.xyz

a ?? b
来源：http://njm.epnwcf.com

[U87] JS：解构默认值
来源：http://acu.fzhhl.top

const { a = 1, b = 2 } = obj;
来源：http://gad.fanxiaobao.xyz

[U88] JS：对象展开合并
来源：http://hvf.pycfn.com

{ ...a, ...b }
来源：http://pdt.chenzaomai.com

[U89] JS：数组去重
来源：http://yld.aibaodan.cn

[...new Set(arr)]
来源：http://fkr.zhiwuduotai.top

[U90] JS：数字数组排序
来源：http://kdi.fehbvm.com

[...arr].sort((a, b) => a - b)
来源：http://tly.chenzaomai.com

[U91] JS：对象键值遍历
来源：http://vvt.yueranfly.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hnt.9152youxi.cn

[U92] JS：深拷贝
来源：http://hia.tianlin.xyz

structuredClone(obj)
来源：http://vtw.nanxuanxn.top

[U93] JS：模板字符串
来源：http://uff.ydjk.org.cn

`共 ${n} 条`
来源：http://qxc.andypj.xyz

[U94] JS：箭头函数
来源：http://hti.havefunace.top

const double = x => x * 2;
来源：http://esg.hesvh.cn

[U95] JS：Promise 包装
来源：http://yze.feifeiyinyue.top

new Promise((resolve, reject) => {})
来源：http://rva.mhx1999.top

[U96] JS：async/await 与异常
来源：http://erh.zhongyouzk.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ain.gaohongyu789.top

[U97] JS：并发请求
来源：http://uwk.yanxiufei.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://qkd.epnwcf.com

[U98] JS：fetch 带 JSON
来源：http://ypn.tanke756.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://exv.meibo888.top

[U99] JS：事件监听
来源：http://ifn.zhengqikj.top

el.addEventListener("click", e => {})
来源：http://bnf.zdqjudy.top

[U100] JS：DOM 查询
来源：http://sex.ydzc1.top

document.querySelector(".item")
来源：http://dsb.dashuyun.cn

[U101] JS：classList 操作
来源：http://gmi.mhx1999.top

el.classList.toggle("active")
来源：http://jwm.havefunace.top

[U102] JS：本地存储
来源：http://pzv.svipenyu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://wfu.ydjk.org.cn

[U103] JS：定时器
来源：http://zfj.sxryk.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wwa.hongshengwenyu.top

[U104] JS：防抖
来源：http://jhw.hnxiangtu.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mjp.jinqigufen.top

[U105] JS：节流
来源：http://zza.yvedp.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rxr.ydjk.org.cn

[U106] JS：日期格式化
来源：http://rwp.yj20258888.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://odt.zhengqikj.top

[U107] JS：数字千分位
来源：http://puu.andypj.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mvr.yongpay.top

[U108] JS：随机整数
来源：http://dmz.hcnkem.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jiq.mhx1999.top

[U109] JS：数组分组
来源：http://nbw.hnxiangtu.top

Object.groupBy(arr, x => x.type)
来源：http://lfk.nanxinkj.top

[U110] JS：数组分块
来源：http://uma.birdmap.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ewm.haohaochexian.top

[U111] JS：对象转 Map
来源：http://hfc.ybcxt.top

new Map(Object.entries(obj))
来源：http://hyh.birdmap.top

[U112] JS：字符串补位
来源：http://xci.jinyuanbaomall.cn

"7".padStart(3, "0")
来源：http://wod.pengpengdd.cyou

[U113] JS：正则替换全部
来源：http://mym.yanxiufei.cn

s.replaceAll("a", "b")
来源：http://qjx.daria6918.cn

[U114] JS：JSON 深比较
来源：http://kic.yfazqb.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://mqh.ydjk.org.cn

[U115] JS：生成 UUID
来源：http://mno.zhengqikj.top

crypto.randomUUID()
来源：http://kod.hongshengwenyu.top

[U116] JS：类型检查（JSDoc）
来源：http://jok.zhongyouzk.top

/** @param {string} name */ function f(name) {}
来源：http://jod.birdmap.top

[U117] JS：单元测试
来源：http://ord.9152youxi.cn

npm i -D vitest;  npx vitest
来源：http://ibj.aibaodan.cn

[U118] JS：开发服务器
来源：http://cfo.yuxming.cn

npm i -D vite;  npx vite
来源：http://ibq.hnxiangtu.top

[U119] JS：生产构建
来源：http://coc.hfpthk.cn

npx vite build
来源：http://flp.wangdashe.top

[U120] JS：读取环境变量（Vite）
来源：http://kwf.ywan-chungtsiang.top

import.meta.env.VITE_API_URL
来源：http://wnu.vqdsnc.cn

================================================================================
来源：http://beu.zhoulong.xyz

统计汇总
来源：http://zqt.sjlbkw.cn

================================================================================
来源：http://gtc.jqgfzy.top

按语言统计（条）：
来源：http://zdx.yangfankeji.com

Python ......... 252
来源：http://beq.yfazqb.com

PHP ............ 252
来源：http://mto.cheryme.top

JavaScript ..... 252
来源：http://oyv.yj20258.top

TypeScript ..... 212
来源：http://cfx.quarkkingdee.top

Java ........... 212
来源：http://gmc.feifeiyinyue.top

Go ............. 212
来源：http://qhb.fktsv.cn

Ruby ........... 212
来源：http://ydo.52xcode.cn

C# ............. 212
来源：http://txy.yonumen.top

C .............. 30
来源：http://obw.fzhhl.top

C++ ............ 30
来源：http://yao.tarul.cn

SQL ............ 90
来源：http://gsu.guannengcc.top

Bash ........... 80
来源：http://eyo.aizwys.cn

Kotlin ......... 15
来源：http://zwr.wangshuangyany.cn

Swift .......... 15
来源：http://qwg.yanxiufei.cn

Lua ............ 10
来源：http://kyi.shanyushiyangkeji.top

Perl ........... 10
来源：http://xwa.mhx1999.top

Scala .......... 10
来源：http://glm.pycfn.com

------------------------------------
来源：http://dbd.zhijiandao.cn

合计 ........... 2106 条
来源：http://whp.xuetiantiany.cn

按章节统计：
来源：http://dbu.meibo888.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dev.chenjidiqi.icu

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rwe.xuanzx.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xrx.xinyue.icu

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xbu.hcnkem.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bav.52xcode.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://owk.jlsjyb.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jjg.tianlin.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://yiq.gaohongyu789.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nrz.9152youxi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xvb.hywenlv.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jxj.hnqzz.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qhq.iojbl.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wkp.shzxlz.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://sde.dashuyun.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://lcx.zdqjudy.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mow.ehwqpu.com

Q SQL 专题                              90
来源：http://djo.gaohongyu789.top

R Bash 专题                             80
来源：http://rib.shangyingyoupin.top

S C / C++ 专题                          60
来源：http://euz.ywan-chungtsiang.top

T 其他语言补充                          60
来源：http://hqh.jinghuilouyu.cn

U 高频实用片段                         120
来源：http://dvo.hammf.cn

------------------------------------
来源：http://guq.sweek.top

合计                                  2106 条
来源：http://nor.epnwcf.com

--------------------------------------------------------------------------------
来源：http://gzj.shangyingyoupin.top

使用提醒
来源：http://pba.hnqzz.top

--------------------------------------------------------------------------------
来源：http://qoa.zhongyouzk.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://uow.zhaomingkeji.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://asl.mhx1999.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://bva.yonumen.top

在旧版本上使用前请先确认语法支持情况。
来源：http://fri.sufxvd.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://pgi.ydjk.org.cn

—— 文件结束 ——
来源：http://ulm.jlsjyb.cn

================================================================================
来源：http://hff.epnwcf.com

程序语言常见例子速查手册（2024 版）
来源：http://oxp.xylfe.cn

Common Programming Examples Cheat Book
来源：http://zxg.316326.xyz

================================================================================
来源：http://isi.aizwys.cn

【收录内容】
来源：http://yjm.zhaomingkeji.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://pvk.yanxiufei.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://rln.xingfuxueyuan.xyz

SQL · Bash · C · C++
来源：http://hhl.mhx1999.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xgr.aibaodan.cn

【使用说明】
来源：http://sox.cdnleiting.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ufi.ivvv.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://fls.zhengqikj.top


<!-- 参考信息 -->