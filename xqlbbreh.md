代发 wailian999

[U05] Py：列表去重且保序
来源：http://wgi.quarkkingdee.top

list(dict.fromkeys(arr))
来源：http://qag.yonumen.top

[U06] Py：合并两个字典
来源：http://xra.quarkkingdee.top

{**a, **b}
来源：http://oar.uphjek.com

[U07] Py：反转字典键值
来源：http://hmf.zycfv.cn

{v: k for k, v in d.items()}
来源：http://qnu.yonumen.top

[U08] Py：展平二维列表
来源：http://fcj.yvedp.cn

[y for x in nested for y in x]
来源：http://lzm.vqdsnc.cn

[U09] Py：字典取最大值的键
来源：http://rge.fktsv.cn

max(d, key=d.get)
来源：http://xxw.zhaomingkeji.xyz

[U10] Py：按值排序字典
来源：http://dpb.hcnkem.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kie.jqgfzy.top

[U11] Py：生成器表达式
来源：http://xxj.sxryk.cn

(x * 2 for x in arr)
来源：http://gqa.c1oappe.top

[U12] Py：取出现最多的 3 个元素
来源：http://elo.nwbrower.top

Counter(arr).most_common(3)
来源：http://xrf.yuxming.cn

[U13] Py：固定长度队列
来源：http://aep.chenlongwang.top

deque(maxlen=10)
来源：http://hdr.cqqwz.cn

[U14] Py：分组收集到列表
来源：http://ppi.shzxlz.cn

defaultdict(list)
来源：http://euu.zhengqikj.top

[U15] Py：高精度计时
来源：http://moe.jiagoushi.top

t = time.perf_counter()
来源：http://loo.gotoacloud.top

[U16] Py：命令行参数解析
来源：http://mdn.chenzaomai.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://njf.yj20258888.top

[U17] Py：初始化日志
来源：http://ohg.tanke756.top

logging.basicConfig(level=logging.INFO)
来源：http://ekz.jiagoushi.top

[U18] Py：预编译正则
来源：http://pjo.snrcjt.cn

pat = re.compile(r"\d+")
来源：http://bdh.xziqi.cn

[U19] Py：正则替换带回调
来源：http://zqg.nanxuanxn.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xaj.zhongyouzk.top

[U20] Py：缓存函数结果
来源：http://xde.yongpay.top

@functools.lru_cache(maxsize=None)
来源：http://xza.ppjwa.cn

[U21] Py：自定义上下文管理器
来源：http://xfe.c1oappe.top

@contextlib.contextmanager
来源：http://ioi.hywenlv.cn

[U22] Py：矩阵转置
来源：http://nmy.birdmap.top

list(zip(*m))
来源：http://pfr.shuidangran.top

[U23] Py：分块读取大文件
来源：http://dej.meibo888.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rgr.wangshuangyany.cn

[U24] Py：路径操作
来源：http://jpf.9152youxi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zjz.pycfn.com

[U25] Py：CSV 按字典读
来源：http://rvc.fehbvm.com

csv.DictReader(f)
来源：http://xux.epnwcf.com

[U26] Py：并发下载
来源：http://hoa.shangyingyoupin.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qqv.pengpengdd.cyou

[U27] Py：异步 HTTP
来源：http://woj.svipenyu.cn

aiohttp.ClientSession() 配合 async with
来源：http://enu.chenzaomai.com

[U28] Py：类型别名
来源：http://iaj.ydzc1.top

UserId = int
来源：http://hgv.9152youxi.cn

[U29] Py：属性校验
来源：http://yxj.52xcode.cn

@property 与 @x.setter 配合
来源：http://ngr.daxiang520.top

[U30] Py：数据类
来源：http://wfs.shuidangran.top

@dataclass(slots=True)
来源：http://sfz.mhx1999.top

[U31] Py：单测
来源：http://ccu.yj20258.top

python -m pytest -q
来源：http://rxl.fanxiaobao.xyz

[U32] Py：代码格式化
来源：http://elf.hcnkem.com

ruff format . && ruff check --fix .
来源：http://pxm.kuanghao11.cn

[U33] Py：打包发布
来源：http://gdz.xingfuxueyuan.xyz

python -m build  （依赖 pyproject.toml）
来源：http://kme.hesvh.cn

[U34] Py：判断编码
来源：http://umm.cheryme.top

chardet.detect(raw)
来源：http://tkj.jlsjyb.cn

[U35] Py：发送邮件
来源：http://ead.feifeiyinyue.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://lop.shuidangran.top

[U36] Py：定时任务
来源：http://ozp.daxiang520.top

schedule.every(10).minutes.do(job)
来源：http://qcm.jiagoushi.top

[U37] Py：读写 Excel
来源：http://muw.gogol.net.cn

pandas.read_excel / DataFrame.to_excel
来源：http://pbz.gzhubu.top

[U38] Py：获取脚本所在目录
来源：http://okq.aibaodan.cn

Path(__file__).resolve().parent
来源：http://brm.nanxinkj.top

[U39] Py：判断是否在交互环境
来源：http://oic.wangdashe.top

sys.stdout.isatty()
来源：http://bsf.fehbvm.com

[U40] Py：打印到标准错误
来源：http://lux.tarul.cn

print("err", file=sys.stderr)
来源：http://uzm.hnqzz.top

[U41] PHP：初始化 Composer 项目
来源：http://okf.chenzaomai.com

composer init;  composer require guzzlehttp/guzzle
来源：http://kzv.jqgufenzy.top

[U42] PHP：PSR-4 自动加载
来源：http://iaw.tian-w.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zfu.xuetiantiany.cn

[U43] PHP：声明命名空间
来源：http://dqf.dashuyun.cn

namespace App\Http;
来源：http://wsf.quarkkingdee.top

[U44] PHP：开启严格类型
来源：http://onx.jyoumei.cn

declare(strict_types=1);
来源：http://qxg.nwbrower.top

[U45] PHP：类型声明与返回类型
来源：http://ngs.wangshuangyany.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://suc.gaohongyu789.top

[U46] PHP：可空类型
来源：http://fyq.aizwys.cn

?string $name = null
来源：http://yls.redwolf501.top

[U47] PHP：联合类型
来源：http://jbx.hammf.cn

int|string $id
来源：http://xid.c1oappe.top

[U48] PHP：纯枚举
来源：http://kmw.ehwqpu.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://plk.aibaodan.cn

[U49] PHP：只读属性
来源：http://bdh.fengsongda.top

public readonly string $name
来源：http://ijv.ppjwa.cn

[U50] PHP：构造器属性提升
来源：http://miq.feifeiyinyue.top

public function __construct(private int $id) {}
来源：http://ztv.bbcook.cn

[U51] PHP：数组解构
来源：http://xjx.zhixingplan.top

[$a, $b] = $arr;
来源：http://fsy.hcnkem.com

[U52] PHP：箭头函数
来源：http://jmr.chenlongwang.top

$double = fn($x) => $x * 2;
来源：http://jjg.jinyuanbaomall.cn

[U53] PHP：空合并运算符
来源：http://jfs.shanyushiyangkeji.top

$v = $a ?? $b ?? "default";
来源：http://edz.aizwys.cn

[U54] PHP：空安全调用
来源：http://cac.zhixingplan.top

$obj?->method()
来源：http://xra.wangshuangyany.cn

[U55] PHP：match 表达式
来源：http://anf.chenjidiqi.icu

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qqt.yuanzhike.top

[U56] PHP：命名参数
来源：http://ywc.yangfankeji.com

f(a: 1, b: 2)
来源：http://ftv.xylfe.cn

[U57] PHP：字符串插值
来源：http://bie.zhaomingkeji.xyz

"值: {$a}"
来源：http://rwy.hammf.cn

[U58] PHP：数组三件套
来源：http://hpm.yanxiufei.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vhe.jqgufenzy.top

[U59] PHP：自定义排序
来源：http://pps.52xcode.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ayz.gotoacloud.top

[U60] PHP：JSON 编解码
来源：http://bao.xylfe.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wer.snrcjt.cn

[U61] PHP：正则
来源：http://ybu.tian-w.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xet.cdnleiting.top

[U62] PHP：日期对象
来源：http://jxe.guannengcc.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ejw.52xcode.cn

[U63] PHP：文件读写
来源：http://dtm.gaohongyu789.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gbn.shuidangran.top

[U64] PHP：目录遍历
来源：http://qft.sysykeji.top

glob("dir/*.php");  scandir("dir");
来源：http://xpm.yj20258888.top

[U65] PHP：会话
来源：http://vje.hnxiangtu.top

session_start();  $_SESSION["uid"] = 1;
来源：http://nuf.yangfankeji.com

[U66] PHP：设置 Cookie
来源：http://ibk.jiagoushi.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ajz.sysykeji.top

[U67] PHP：处理文件上传
来源：http://hwe.gotoacloud.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zwn.cucudq.cn

[U68] PHP：PDO 连接
来源：http://mde.yj20258.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jst.fanxiaobao.xyz

[U69] PHP：PDO 预处理
来源：http://jrn.wangshuangyany.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://pku.hesvh.cn

[U70] PHP：PDO 事务
来源：http://msm.yuanzhike.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kbu.hesvh.cn

[U71] PHP：抛出异常
来源：http://wsq.daxiang520.top

throw new RuntimeException("失败", 500);
来源：http://lbg.redwolf501.top

[U72] PHP：写错误日志
来源：http://zzg.zhijiandao.cn

error_log("失败: " . $e->getMessage());
来源：http://xgf.chenlongwang.top

[U73] PHP：读取 ini 配置
来源：http://ijv.shanyushiyangkeji.top

parse_ini_file("config.ini", true)
来源：http://xdd.hongshengwenyu.top

[U74] PHP：读取环境变量
来源：http://dbk.fanxiaobao.xyz

getenv("APP_ENV") ?: "production"
来源：http://hdr.chenlongwang.top

[U75] PHP：依赖注入
来源：http://exh.bjfxy.top

composer require psr/container
来源：http://tua.xingfuxueyuan.xyz

[U76] PHP：简单路由
来源：http://bhn.tianlin.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xkd.gogol.net.cn

[U77] PHP：模板渲染
来源：http://qsu.ctjpmb.com

composer require twig/twig
来源：http://rpf.sufxvd.cn

[U78] PHP：单元测试
来源：http://ymz.bbcook.cn

composer require --dev phpunit/phpunit
来源：http://gvg.zhijiandao.cn

[U79] PHP：静态分析
来源：http://jru.xingfuxueyuan.xyz

composer require --dev phpstan/phpstan
来源：http://yhi.bbcook.cn

[U80] PHP：代码规范修复
来源：http://ovf.hnxiangtu.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://uox.yfazqb.com

[U81] JS：初始化项目
来源：http://fja.yj20258888.top

npm init -y;  npm i express
来源：http://ian.ivvv.top

[U82] JS：package.json 脚本
来源：http://txh.feifeiyinyue.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://uoh.jinqigfzy.top

[U83] JS：ES Module 导入导出
来源：http://nex.mhx1999.top

export const a = 1;  import { a } from "./m.js";
来源：http://snd.yongpay.top

[U84] JS：CommonJS 写法
来源：http://yqx.zhoulong.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://mbj.xingfuxueyuan.xyz

[U85] JS：可选链
来源：http://ull.aibaodan.cn

a?.b?.c
来源：http://bhb.jqgufenzy.top

[U86] JS：空值合并
来源：http://dxl.ywan-chungtsiang.top

a ?? b
来源：http://bso.fanxiaobao.xyz

[U87] JS：解构默认值
来源：http://psx.iojbl.cn

const { a = 1, b = 2 } = obj;
来源：http://man.hfpthk.cn

[U88] JS：对象展开合并
来源：http://hhx.tanke756.top

{ ...a, ...b }
来源：http://nwa.snrcjt.cn

[U89] JS：数组去重
来源：http://vwy.dianchejie.cn

[...new Set(arr)]
来源：http://ijj.andypj.xyz

[U90] JS：数字数组排序
来源：http://hif.smart0.xyz

[...arr].sort((a, b) => a - b)
来源：http://byq.fzhhl.top

[U91] JS：对象键值遍历
来源：http://kpl.chenlongwang.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://leo.fzhhl.top

[U92] JS：深拷贝
来源：http://exq.chenlongwang.top

structuredClone(obj)
来源：http://qpr.aibaodan.cn

[U93] JS：模板字符串
来源：http://daj.hesvh.cn

`共 ${n} 条`
来源：http://awa.ydzc1.top

[U94] JS：箭头函数
来源：http://ffi.xuetiantiany.cn

const double = x => x * 2;
来源：http://kaq.mhx1999.top

[U95] JS：Promise 包装
来源：http://dty.316326.xyz

new Promise((resolve, reject) => {})
来源：http://sij.shangyingyoupin.top

[U96] JS：async/await 与异常
来源：http://msz.nanxinkj.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://uop.dianchejie.cn

[U97] JS：并发请求
来源：http://xev.sysykeji.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://zlk.pengpengdd.cyou

[U98] JS：fetch 带 JSON
来源：http://jnb.ydjk.org.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ncv.gaohongyu789.top

[U99] JS：事件监听
来源：http://pxg.chenzaomai.com

el.addEventListener("click", e => {})
来源：http://szg.ctjpmb.com

[U100] JS：DOM 查询
来源：http://zjn.iojbl.cn

document.querySelector(".item")
来源：http://dqb.shzxlz.cn

[U101] JS：classList 操作
来源：http://sxa.vqdsnc.cn

el.classList.toggle("active")
来源：http://crt.guowangkeji.top

[U102] JS：本地存储
来源：http://ogm.jianghu66.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://bon.sweek.top

[U103] JS：定时器
来源：http://lyr.iojbl.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jcm.cdnleiting.top

[U104] JS：防抖
来源：http://ygq.ybcxt.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oan.yfazqb.com

[U105] JS：节流
来源：http://ezl.ybcxt.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://riy.uphjek.com

[U106] JS：日期格式化
来源：http://wpu.sweek.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://euh.shanyushiyangkeji.top

[U107] JS：数字千分位
来源：http://wti.tarul.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://naf.fengsongda.top

[U108] JS：随机整数
来源：http://yqm.shanyushiyangtech.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ogn.xziqi.cn

[U109] JS：数组分组
来源：http://cjo.zhongyouzk.top

Object.groupBy(arr, x => x.type)
来源：http://etl.zdbjq.cn

[U110] JS：数组分块
来源：http://lvd.shanyushiyangkeji.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ass.hnxiangtu.top

[U111] JS：对象转 Map
来源：http://pzr.ydzc1.top

new Map(Object.entries(obj))
来源：http://eby.zycfv.cn

[U112] JS：字符串补位
来源：http://bgs.cashguo.top

"7".padStart(3, "0")
来源：http://xtx.sysykeji.top

[U113] JS：正则替换全部
来源：http://ped.cheryme.top

s.replaceAll("a", "b")
来源：http://uno.shanyushiyangkeji.top

[U114] JS：JSON 深比较
来源：http://pud.yfazqb.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://lqd.hywenlv.cn

[U115] JS：生成 UUID
来源：http://fqb.hnqzz.top

crypto.randomUUID()
来源：http://vzl.0kj1m.cn

[U116] JS：类型检查（JSDoc）
来源：http://uhe.feifeiyinyue.top

/** @param {string} name */ function f(name) {}
来源：http://mth.ppjwa.cn

[U117] JS：单元测试
来源：http://isb.yongpay.top

npm i -D vitest;  npx vitest
来源：http://pke.xylfe.cn

[U118] JS：开发服务器
来源：http://bba.yangfankeji.com

npm i -D vite;  npx vite
来源：http://meu.jinqigfzy.top

[U119] JS：生产构建
来源：http://fkl.zycfv.cn

npx vite build
来源：http://edn.yuanzhike.top

[U120] JS：读取环境变量（Vite）
来源：http://gmu.hammf.cn

import.meta.env.VITE_API_URL
来源：http://nat.tianlin.xyz

================================================================================
来源：http://mtt.shuidangran.top

统计汇总
来源：http://yzw.chenzaomai.com

================================================================================
来源：http://kng.zdbjq.cn

按语言统计（条）：
来源：http://ifn.xuetiantiany.cn

Python ......... 252
来源：http://lyc.shanyushiyangtech.top

PHP ............ 252
来源：http://huo.bjfxy.top

JavaScript ..... 252
来源：http://ctd.jinyuanbaomall.cn

TypeScript ..... 212
来源：http://qvl.jqgufenzy.top

Java ........... 212
来源：http://pdg.yuanzhike.top

Go ............. 212
来源：http://sxq.sufxvd.cn

Ruby ........... 212
来源：http://tcx.fanxiaobao.xyz

C# ............. 212
来源：http://lfe.zdbjq.cn

C .............. 30
来源：http://vyu.jiagoushi.top

C++ ............ 30
来源：http://smg.hysaishi.cn

SQL ............ 90
来源：http://zco.hcnkem.com

Bash ........... 80
来源：http://ocg.hysaishi.cn

Kotlin ......... 15
来源：http://jtl.jqgfzy.top

Swift .......... 15
来源：http://arl.quarkkingdee.top

Lua ............ 10
来源：http://ozb.shuidangran.top

Perl ........... 10
来源：http://dht.yvedp.cn

Scala .......... 10
来源：http://wpw.hammf.cn

------------------------------------
来源：http://isy.gogol.net.cn

合计 ........... 2106 条
来源：http://img.jianghu66.top

按章节统计：
来源：http://ocs.sysykeji.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://yly.cashguo.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://quj.c1oappe.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://edj.zhiwuduotai.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fiy.nwbrower.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xoc.guowangkeji.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://fzs.quarkkingdee.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wxg.52xcode.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://fqq.shangyingyoupin.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://agq.shangyingyoupin.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rjy.quarkkingdee.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ehm.sufxvd.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ikr.fehbvm.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://dvi.52xcode.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tfb.yueranfly.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://gey.daria6918.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://smj.zhengqikj.top

Q SQL 专题                              90
来源：http://ivo.pycfn.com

R Bash 专题                             80
来源：http://yor.yfazqb.com

S C / C++ 专题                          60
来源：http://gpo.aizwys.cn

T 其他语言补充                          60
来源：http://lwm.jqgfzy.top

U 高频实用片段                         120
来源：http://hwc.jiagoushi.top

------------------------------------
来源：http://xal.aizwys.cn

合计                                  2106 条
来源：http://acx.gaohongyu789.top

--------------------------------------------------------------------------------
来源：http://wgn.andypj.xyz

使用提醒
来源：http://ofq.c1oappe.top

--------------------------------------------------------------------------------
来源：http://hae.zycfv.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ynj.yanxiufei.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bju.jianghu66.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://sdv.smart0.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://gac.xziqi.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://gzf.tanke756.top

—— 文件结束 ——
来源：http://azv.cucudq.cn

================================================================================
来源：http://swl.52xcode.cn

程序语言常见例子速查手册（2024 版）
来源：http://pri.jqgufenzy.top

Common Programming Examples Cheat Book
来源：http://zql.hfpthk.cn

================================================================================
来源：http://sqe.hcnkem.com

【收录内容】
来源：http://ows.shzxlz.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://hii.zhiwuduotai.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://omd.guannengcc.top

SQL · Bash · C · C++
来源：http://clk.dianchejie.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://gib.ppjwa.cn

【使用说明】
来源：http://smh.andypj.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ock.zhengqikj.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://utq.0kj1m.cn


<!-- 参考信息 -->