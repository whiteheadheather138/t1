代发 wailian999

[U05] Py：列表去重且保序
来源：http://yum.mhx1999.top

list(dict.fromkeys(arr))
来源：http://npu.vqdsnc.cn

[U06] Py：合并两个字典
来源：http://bug.jianghu66.top

{**a, **b}
来源：http://lmc.vehdjk.com

[U07] Py：反转字典键值
来源：http://qxp.vqdsnc.cn

{v: k for k, v in d.items()}
来源：http://qyy.gaohongyu789.top

[U08] Py：展平二维列表
来源：http://omg.sufxvd.cn

[y for x in nested for y in x]
来源：http://hwk.chenzaomai.com

[U09] Py：字典取最大值的键
来源：http://dqm.jinqigufen.top

max(d, key=d.get)
来源：http://yjn.hcnkem.com

[U10] Py：按值排序字典
来源：http://kio.jlsjyb.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qnc.yuxming.cn

[U11] Py：生成器表达式
来源：http://imf.fktsv.cn

(x * 2 for x in arr)
来源：http://oyt.meibo888.top

[U12] Py：取出现最多的 3 个元素
来源：http://gxs.tanke756.top

Counter(arr).most_common(3)
来源：http://ndn.yuanzhike.top

[U13] Py：固定长度队列
来源：http://ron.zhengqikj.top

deque(maxlen=10)
来源：http://epp.uphjek.com

[U14] Py：分组收集到列表
来源：http://kfm.snrcjt.cn

defaultdict(list)
来源：http://nvn.ehwqpu.com

[U15] Py：高精度计时
来源：http://jpd.yj20258888.top

t = time.perf_counter()
来源：http://lpa.zycfv.cn

[U16] Py：命令行参数解析
来源：http://sde.nanxinkj.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mib.bjfxy.top

[U17] Py：初始化日志
来源：http://gqi.yfazqb.com

logging.basicConfig(level=logging.INFO)
来源：http://rhn.fengsongda.top

[U18] Py：预编译正则
来源：http://szv.jiagoushi.top

pat = re.compile(r"\d+")
来源：http://tqu.zhijiandao.cn

[U19] Py：正则替换带回调
来源：http://dnf.ydjk.org.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://avh.yongpay.top

[U20] Py：缓存函数结果
来源：http://btf.jiagoushi.top

@functools.lru_cache(maxsize=None)
来源：http://kqh.gzhubu.top

[U21] Py：自定义上下文管理器
来源：http://puj.daria6918.cn

@contextlib.contextmanager
来源：http://pxn.quarkkingdee.top

[U22] Py：矩阵转置
来源：http://gkd.zycfv.cn

list(zip(*m))
来源：http://his.cheryme.top

[U23] Py：分块读取大文件
来源：http://meu.jqgufenzy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://azg.yvedp.cn

[U24] Py：路径操作
来源：http://usi.xingfuxueyuan.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://kie.guowangkeji.top

[U25] Py：CSV 按字典读
来源：http://myh.daria6918.cn

csv.DictReader(f)
来源：http://qmm.zhiwuduotai.top

[U26] Py：并发下载
来源：http://tjx.shanyushiyangtech.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nmm.ehwqpu.com

[U27] Py：异步 HTTP
来源：http://xaa.shangyingyoupin.top

aiohttp.ClientSession() 配合 async with
来源：http://pyi.dashuyun.cn

[U28] Py：类型别名
来源：http://xqm.ywan-chungtsiang.top

UserId = int
来源：http://hax.haohaochexian.top

[U29] Py：属性校验
来源：http://pow.tianlin.xyz

@property 与 @x.setter 配合
来源：http://kay.vqdsnc.cn

[U30] Py：数据类
来源：http://xro.hammf.cn

@dataclass(slots=True)
来源：http://lgj.zhengqikj.top

[U31] Py：单测
来源：http://gaa.kuanghao11.cn

python -m pytest -q
来源：http://tzl.ydzc1.top

[U32] Py：代码格式化
来源：http://ier.zycfv.cn

ruff format . && ruff check --fix .
来源：http://bxa.wangshuangyany.cn

[U33] Py：打包发布
来源：http://rxz.zhijiandao.cn

python -m build  （依赖 pyproject.toml）
来源：http://xij.fktsv.cn

[U34] Py：判断编码
来源：http://qte.ppjwa.cn

chardet.detect(raw)
来源：http://fcr.fzhhl.top

[U35] Py：发送邮件
来源：http://ncm.yongpay.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nmq.yj202588.top

[U36] Py：定时任务
来源：http://rot.yj20258888.top

schedule.every(10).minutes.do(job)
来源：http://caf.jinghuilouyu.cn

[U37] Py：读写 Excel
来源：http://jjo.zhixingplan.top

pandas.read_excel / DataFrame.to_excel
来源：http://sry.jlsjyb.cn

[U38] Py：获取脚本所在目录
来源：http://vkg.ehwqpu.com

Path(__file__).resolve().parent
来源：http://rhg.shuidangran.top

[U39] Py：判断是否在交互环境
来源：http://kvr.nanxuanxn.top

sys.stdout.isatty()
来源：http://ffb.jqgufenzy.top

[U40] Py：打印到标准错误
来源：http://mhs.xziqi.cn

print("err", file=sys.stderr)
来源：http://eak.daxiang520.top

[U41] PHP：初始化 Composer 项目
来源：http://cwa.ehwqpu.com

composer init;  composer require guzzlehttp/guzzle
来源：http://vlf.cashguo.top

[U42] PHP：PSR-4 自动加载
来源：http://kjs.cheryme.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://udm.pengpengdd.cyou

[U43] PHP：声明命名空间
来源：http://fdr.9152youxi.cn

namespace App\Http;
来源：http://pwp.shanyushiyangkeji.top

[U44] PHP：开启严格类型
来源：http://gon.xingfuxueyuan.xyz

declare(strict_types=1);
来源：http://rdd.yvedp.cn

[U45] PHP：类型声明与返回类型
来源：http://nxk.vehdjk.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://aza.hesvh.cn

[U46] PHP：可空类型
来源：http://xqt.vqdsnc.cn

?string $name = null
来源：http://kbq.cucudq.cn

[U47] PHP：联合类型
来源：http://ifs.chenjidiqi.icu

int|string $id
来源：http://fin.shanyushiyangtech.top

[U48] PHP：纯枚举
来源：http://ekg.havefunace.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cjo.snrcjt.cn

[U49] PHP：只读属性
来源：http://opq.shanyushiyangtech.top

public readonly string $name
来源：http://pgb.pengpengdd.cyou

[U50] PHP：构造器属性提升
来源：http://tzr.cucudq.cn

public function __construct(private int $id) {}
来源：http://ctw.vehdjk.com

[U51] PHP：数组解构
来源：http://tyt.ydzc1.top

[$a, $b] = $arr;
来源：http://lmn.shzxlz.cn

[U52] PHP：箭头函数
来源：http://gmj.iojbl.cn

$double = fn($x) => $x * 2;
来源：http://rwh.jianghu66.top

[U53] PHP：空合并运算符
来源：http://sew.fehbvm.com

$v = $a ?? $b ?? "default";
来源：http://qav.shangyingyoupin.top

[U54] PHP：空安全调用
来源：http://rgz.snrcjt.cn

$obj?->method()
来源：http://zvc.sjlbkw.cn

[U55] PHP：match 表达式
来源：http://qzo.jianghu66.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bpk.ehwqpu.com

[U56] PHP：命名参数
来源：http://lup.uphjek.com

f(a: 1, b: 2)
来源：http://rso.shanyushiyangtech.top

[U57] PHP：字符串插值
来源：http://byr.tarul.cn

"值: {$a}"
来源：http://duf.mhx1999.top

[U58] PHP：数组三件套
来源：http://ojv.redwolf501.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cwy.zhijiandao.cn

[U59] PHP：自定义排序
来源：http://epe.mhx1999.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://erv.ydzc1.top

[U60] PHP：JSON 编解码
来源：http://cgz.jinqigufen.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ytg.fzhhl.top

[U61] PHP：正则
来源：http://izt.0kj1m.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://raf.sufxvd.cn

[U62] PHP：日期对象
来源：http://rjs.yj202588.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hff.jqgufenzy.top

[U63] PHP：文件读写
来源：http://cde.ydjk.org.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lem.ctjpmb.com

[U64] PHP：目录遍历
来源：http://ddf.havefunace.top

glob("dir/*.php");  scandir("dir");
来源：http://phd.havefunace.top

[U65] PHP：会话
来源：http://pja.gotoacloud.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ddz.zhongyouzk.top

[U66] PHP：设置 Cookie
来源：http://qan.yfazqb.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://lpl.ydjk.org.cn

[U67] PHP：处理文件上传
来源：http://woy.xingfuxueyuan.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kzv.ppjwa.cn

[U68] PHP：PDO 连接
来源：http://unv.yuxming.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ktm.zdqjudy.top

[U69] PHP：PDO 预处理
来源：http://yja.zhaomingkeji.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ncq.yongpay.top

[U70] PHP：PDO 事务
来源：http://kvv.cdnleiting.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kjz.ctjpmb.com

[U71] PHP：抛出异常
来源：http://aou.yuxming.cn

throw new RuntimeException("失败", 500);
来源：http://gnr.sjlbkw.cn

[U72] PHP：写错误日志
来源：http://smn.aizwys.cn

error_log("失败: " . $e->getMessage());
来源：http://btj.bbcook.cn

[U73] PHP：读取 ini 配置
来源：http://twv.quarkkingdee.top

parse_ini_file("config.ini", true)
来源：http://izw.jinqigufen.top

[U74] PHP：读取环境变量
来源：http://jgk.xinyue.icu

getenv("APP_ENV") ?: "production"
来源：http://uau.hfpthk.cn

[U75] PHP：依赖注入
来源：http://vam.ydjk.org.cn

composer require psr/container
来源：http://klm.yj202588.top

[U76] PHP：简单路由
来源：http://hfa.zycfv.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://cns.haohaochexian.top

[U77] PHP：模板渲染
来源：http://sth.xylfe.cn

composer require twig/twig
来源：http://dtf.yj20258.top

[U78] PHP：单元测试
来源：http://lih.zhiwuduotai.top

composer require --dev phpunit/phpunit
来源：http://emy.sysykeji.top

[U79] PHP：静态分析
来源：http://vyh.hnxiangtu.top

composer require --dev phpstan/phpstan
来源：http://rco.jianghu66.top

[U80] PHP：代码规范修复
来源：http://jic.jqgfzy.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://vjy.pycfn.com

[U81] JS：初始化项目
来源：http://gow.tarul.cn

npm init -y;  npm i express
来源：http://fsd.hywenlv.cn

[U82] JS：package.json 脚本
来源：http://aok.316326.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://yej.pengpengdd.cyou

[U83] JS：ES Module 导入导出
来源：http://lpb.fanxiaobao.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://xws.haohaochexian.top

[U84] JS：CommonJS 写法
来源：http://uvw.uphjek.com

module.exports = { a };  const { a } = require("./m");
来源：http://whb.hfpthk.cn

[U85] JS：可选链
来源：http://orc.vehdjk.com

a?.b?.c
来源：http://zjv.uphjek.com

[U86] JS：空值合并
来源：http://rtn.fengsongda.top

a ?? b
来源：http://lyd.ydjk.org.cn

[U87] JS：解构默认值
来源：http://yjg.bbcook.cn

const { a = 1, b = 2 } = obj;
来源：http://rss.tanke756.top

[U88] JS：对象展开合并
来源：http://xka.shangyingyoupin.top

{ ...a, ...b }
来源：http://pfb.fzhhl.top

[U89] JS：数组去重
来源：http://ltm.hfpthk.cn

[...new Set(arr)]
来源：http://mkw.hywenlv.cn

[U90] JS：数字数组排序
来源：http://xxn.xingfuxueyuan.xyz

[...arr].sort((a, b) => a - b)
来源：http://saf.fzhhl.top

[U91] JS：对象键值遍历
来源：http://man.shanyushiyangtech.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qbj.pycfn.com

[U92] JS：深拷贝
来源：http://tew.xylfe.cn

structuredClone(obj)
来源：http://tvl.sweek.top

[U93] JS：模板字符串
来源：http://scz.sxryk.cn

`共 ${n} 条`
来源：http://awq.ywan-chungtsiang.top

[U94] JS：箭头函数
来源：http://owu.hcnkem.com

const double = x => x * 2;
来源：http://zlj.cheryme.top

[U95] JS：Promise 包装
来源：http://sjn.52xcode.cn

new Promise((resolve, reject) => {})
来源：http://lny.ywan-chungtsiang.top

[U96] JS：async/await 与异常
来源：http://crl.svipenyu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vfp.yueranfly.top

[U97] JS：并发请求
来源：http://nsr.hcnkem.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://kvn.svipenyu.cn

[U98] JS：fetch 带 JSON
来源：http://mnm.fanxiaobao.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://lgd.vehdjk.com

[U99] JS：事件监听
来源：http://nfy.fanxiaobao.xyz

el.addEventListener("click", e => {})
来源：http://rgo.daria6918.cn

[U100] JS：DOM 查询
来源：http://bat.wangdashe.top

document.querySelector(".item")
来源：http://yhm.jlsjyb.cn

[U101] JS：classList 操作
来源：http://tuq.sjlbkw.cn

el.classList.toggle("active")
来源：http://uuw.andypj.xyz

[U102] JS：本地存储
来源：http://etm.zdbjq.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://emq.sysykeji.top

[U103] JS：定时器
来源：http://bho.yuxming.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://oap.quarkkingdee.top

[U104] JS：防抖
来源：http://dzf.yj20258888.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xwi.chenlongwang.top

[U105] JS：节流
来源：http://wue.jyoumei.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://sju.smart0.xyz

[U106] JS：日期格式化
来源：http://usy.havefunace.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vtk.zhaomingkeji.xyz

[U107] JS：数字千分位
来源：http://fks.shangyingyoupin.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://luk.cashguo.top

[U108] JS：随机整数
来源：http://fcw.ehwqpu.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kay.jinghuilouyu.cn

[U109] JS：数组分组
来源：http://vnf.yuxming.cn

Object.groupBy(arr, x => x.type)
来源：http://twu.jinqigufen.top

[U110] JS：数组分块
来源：http://frn.yanxiufei.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zwm.ivvv.top

[U111] JS：对象转 Map
来源：http://bze.xinyue.icu

new Map(Object.entries(obj))
来源：http://gsw.redwolf501.top

[U112] JS：字符串补位
来源：http://nou.uphjek.com

"7".padStart(3, "0")
来源：http://ziw.sxryk.cn

[U113] JS：正则替换全部
来源：http://hne.tanke756.top

s.replaceAll("a", "b")
来源：http://jea.nanxuanxn.top

[U114] JS：JSON 深比较
来源：http://jvi.daxiang520.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://xtk.zhiwuduotai.top

[U115] JS：生成 UUID
来源：http://ihy.ywan-chungtsiang.top

crypto.randomUUID()
来源：http://ewv.mhx1999.top

[U116] JS：类型检查（JSDoc）
来源：http://gys.cdnleiting.top

/** @param {string} name */ function f(name) {}
来源：http://tqc.zhaomingkeji.xyz

[U117] JS：单元测试
来源：http://exb.bbcook.cn

npm i -D vitest;  npx vitest
来源：http://cvs.hcnkem.com

[U118] JS：开发服务器
来源：http://jff.yuxming.cn

npm i -D vite;  npx vite
来源：http://dzs.xuanzx.com

[U119] JS：生产构建
来源：http://lki.52xcode.cn

npx vite build
来源：http://nlp.jyoumei.cn

[U120] JS：读取环境变量（Vite）
来源：http://slf.yongpay.top

import.meta.env.VITE_API_URL
来源：http://fep.nwbrower.top

================================================================================
来源：http://bsf.aibaodan.cn

统计汇总
来源：http://xno.gaohongyu789.top

================================================================================
来源：http://khg.cheryme.top

按语言统计（条）：
来源：http://upz.zdbjq.cn

Python ......... 252
来源：http://gat.yuanzhike.top

PHP ............ 252
来源：http://xak.yj202588.top

JavaScript ..... 252
来源：http://rcw.uphjek.com

TypeScript ..... 212
来源：http://wgo.zhaomingkeji.xyz

Java ........... 212
来源：http://xkj.zhixingplan.top

Go ............. 212
来源：http://psc.shangyingyoupin.top

Ruby ........... 212
来源：http://fee.xylfe.cn

C# ............. 212
来源：http://bpo.zhixingplan.top

C .............. 30
来源：http://ocg.ydjk.org.cn

C++ ............ 30
来源：http://cmw.zhiwuduotai.top

SQL ............ 90
来源：http://cgi.yfazqb.com

Bash ........... 80
来源：http://cww.havefunace.top

Kotlin ......... 15
来源：http://jas.aibaodan.cn

Swift .......... 15
来源：http://fgn.andypj.xyz

Lua ............ 10
来源：http://wuc.svipenyu.cn

Perl ........... 10
来源：http://qsx.yj20258888.top

Scala .......... 10
来源：http://aba.cqqwz.cn

------------------------------------
来源：http://tru.hnqzz.top

合计 ........... 2106 条
来源：http://cja.vqdsnc.cn

按章节统计：
来源：http://qsq.wangdashe.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://nbu.xingfuxueyuan.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://cep.daria6918.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hzy.fzhhl.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qgm.fzhhl.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dyj.bjfxy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qsn.quarkkingdee.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xhr.ppjwa.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mwf.aibaodan.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://fdz.xziqi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tbt.svipenyu.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ory.aibaodan.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://aco.yj202588.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://asm.cdnleiting.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ddl.sufxvd.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://avc.fzhhl.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://yfm.sxryk.cn

Q SQL 专题                              90
来源：http://xhi.yj20258.top

R Bash 专题                             80
来源：http://nmq.gaohongyu789.top

S C / C++ 专题                          60
来源：http://xnl.redwolf501.top

T 其他语言补充                          60
来源：http://pec.52xcode.cn

U 高频实用片段                         120
来源：http://ils.shanyushiyangtech.top

------------------------------------
来源：http://kou.cdnleiting.top

合计                                  2106 条
来源：http://jbk.shanyushiyangtech.top

--------------------------------------------------------------------------------
来源：http://pye.jinqigufen.top

使用提醒
来源：http://cvr.ywan-chungtsiang.top

--------------------------------------------------------------------------------
来源：http://svh.yuanzhike.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hil.xinyue.icu

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bfz.zhijiandao.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://evp.fzhhl.top

在旧版本上使用前请先确认语法支持情况。
来源：http://ygd.jinyuanbaomall.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://miy.yueranfly.top

—— 文件结束 ——
来源：http://ahk.yfazqb.com

================================================================================
来源：http://syi.zhengqikj.top

程序语言常见例子速查手册（2024 版）
来源：http://lst.yvedp.cn

Common Programming Examples Cheat Book
来源：http://ytc.yonumen.top

================================================================================
来源：http://fus.tian-w.cn

【收录内容】
来源：http://ldi.hongshengwenyu.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://nim.jlsjyb.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wlx.feifeiyinyue.top

SQL · Bash · C · C++
来源：http://fps.sweek.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://nal.cucudq.cn

【使用说明】
来源：http://jlw.ybcxt.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://pmw.zycfv.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wdn.tianlin.xyz


<!-- 参考信息 -->