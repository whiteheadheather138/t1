代发 wailian999

[U01] Py：创建虚拟环境
来源：http://zca.yangfankeji.com

python -m venv .venv && source .venv/bin/activate
来源：http://neg.xylfe.cn

[U02] Py：导出 / 安装依赖
来源：http://yms.feifeiyinyue.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ajq.tianlin.xyz

[U03] Py：加载 .env 配置
来源：http://oim.ybcxt.top

from dotenv import load_dotenv; load_dotenv()
来源：http://qjg.zhixingplan.top

[U04] Py：变量调试打印
来源：http://isp.52xcode.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lid.shangyingyoupin.top

[U05] Py：列表去重且保序
来源：http://eek.cucudq.cn

list(dict.fromkeys(arr))
来源：http://cbu.sufxvd.cn

[U06] Py：合并两个字典
来源：http://ocy.dianchejie.cn

{**a, **b}
来源：http://wjn.c1oappe.top

[U07] Py：反转字典键值
来源：http://gvl.zhoulong.xyz

{v: k for k, v in d.items()}
来源：http://ins.hysaishi.cn

[U08] Py：展平二维列表
来源：http://yxw.jlsjyb.cn

[y for x in nested for y in x]
来源：http://xpe.yangfankeji.com

[U09] Py：字典取最大值的键
来源：http://ouq.tianlin.xyz

max(d, key=d.get)
来源：http://ltl.yangfankeji.com

[U10] Py：按值排序字典
来源：http://flx.hongshengwenyu.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tbn.316326.xyz

[U11] Py：生成器表达式
来源：http://xkl.ywan-chungtsiang.top

(x * 2 for x in arr)
来源：http://xiv.jinqigufen.top

[U12] Py：取出现最多的 3 个元素
来源：http://tgn.zycfv.cn

Counter(arr).most_common(3)
来源：http://yby.fehbvm.com

[U13] Py：固定长度队列
来源：http://hcy.dianchejie.cn

deque(maxlen=10)
来源：http://zsf.ybcxt.top

[U14] Py：分组收集到列表
来源：http://ams.jlsjyb.cn

defaultdict(list)
来源：http://vgq.ivvv.top

[U15] Py：高精度计时
来源：http://odd.shuidangran.top

t = time.perf_counter()
来源：http://naz.ehwqpu.com

[U16] Py：命令行参数解析
来源：http://awv.gogol.net.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zbs.fengsongda.top

[U17] Py：初始化日志
来源：http://gfr.hysaishi.cn

logging.basicConfig(level=logging.INFO)
来源：http://ynr.fengsongda.top

[U18] Py：预编译正则
来源：http://nme.jinqigufen.top

pat = re.compile(r"\d+")
来源：http://jko.vqdsnc.cn

[U19] Py：正则替换带回调
来源：http://akr.vehdjk.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cwx.ehwqpu.com

[U20] Py：缓存函数结果
来源：http://ufb.fehbvm.com

@functools.lru_cache(maxsize=None)
来源：http://yur.hcnkem.com

[U21] Py：自定义上下文管理器
来源：http://kkb.yonumen.top

@contextlib.contextmanager
来源：http://zcp.dashuyun.cn

[U22] Py：矩阵转置
来源：http://pfs.shanyushiyangkeji.top

list(zip(*m))
来源：http://rvu.zhiwuduotai.top

[U23] Py：分块读取大文件
来源：http://hhq.epnwcf.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://uxc.feifeiyinyue.top

[U24] Py：路径操作
来源：http://kzj.mhx1999.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mgh.fehbvm.com

[U25] Py：CSV 按字典读
来源：http://kmq.pycfn.com

csv.DictReader(f)
来源：http://ksj.hywenlv.cn

[U26] Py：并发下载
来源：http://gzs.shanyushiyangkeji.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://eyq.tanke756.top

[U27] Py：异步 HTTP
来源：http://cqb.bbcook.cn

aiohttp.ClientSession() 配合 async with
来源：http://qki.mhx1999.top

[U28] Py：类型别名
来源：http://pab.snrcjt.cn

UserId = int
来源：http://bjx.52xcode.cn

[U29] Py：属性校验
来源：http://mdm.fengsongda.top

@property 与 @x.setter 配合
来源：http://zob.xuanzx.com

[U30] Py：数据类
来源：http://amv.yangfankeji.com

@dataclass(slots=True)
来源：http://axt.yvedp.cn

[U31] Py：单测
来源：http://usw.zhiwuduotai.top

python -m pytest -q
来源：http://hfd.jianghu66.top

[U32] Py：代码格式化
来源：http://cyh.yanxiufei.cn

ruff format . && ruff check --fix .
来源：http://can.tian-w.cn

[U33] Py：打包发布
来源：http://lgm.hammf.cn

python -m build  （依赖 pyproject.toml）
来源：http://jhf.zdbjq.cn

[U34] Py：判断编码
来源：http://qlh.hammf.cn

chardet.detect(raw)
来源：http://jwk.chenzaomai.com

[U35] Py：发送邮件
来源：http://ydj.pycfn.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wor.tian-w.cn

[U36] Py：定时任务
来源：http://qco.sufxvd.cn

schedule.every(10).minutes.do(job)
来源：http://anr.daria6918.cn

[U37] Py：读写 Excel
来源：http://sct.shanyushiyangkeji.top

pandas.read_excel / DataFrame.to_excel
来源：http://nbv.xylfe.cn

[U38] Py：获取脚本所在目录
来源：http://rpb.guowangkeji.top

Path(__file__).resolve().parent
来源：http://day.xuanzx.com

[U39] Py：判断是否在交互环境
来源：http://dpn.yangfankeji.com

sys.stdout.isatty()
来源：http://wyx.hammf.cn

[U40] Py：打印到标准错误
来源：http://cub.yongpay.top

print("err", file=sys.stderr)
来源：http://jkn.yfazqb.com

[U41] PHP：初始化 Composer 项目
来源：http://gab.ywan-chungtsiang.top

composer init;  composer require guzzlehttp/guzzle
来源：http://biz.yvedp.cn

[U42] PHP：PSR-4 自动加载
来源：http://bne.cashguo.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://clq.hesvh.cn

[U43] PHP：声明命名空间
来源：http://ouc.shanyushiyangtech.top

namespace App\Http;
来源：http://aco.quarkkingdee.top

[U44] PHP：开启严格类型
来源：http://cir.shzxlz.cn

declare(strict_types=1);
来源：http://qxr.uphjek.com

[U45] PHP：类型声明与返回类型
来源：http://brt.cdnleiting.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://zhg.316326.xyz

[U46] PHP：可空类型
来源：http://rtt.guannengcc.top

?string $name = null
来源：http://dsk.havefunace.top

[U47] PHP：联合类型
来源：http://vlx.jyoumei.cn

int|string $id
来源：http://ydz.haohaochexian.top

[U48] PHP：纯枚举
来源：http://dtg.zycfv.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cgj.shangyingyoupin.top

[U49] PHP：只读属性
来源：http://nlf.andypj.xyz

public readonly string $name
来源：http://fir.cashguo.top

[U50] PHP：构造器属性提升
来源：http://njo.nanxinkj.top

public function __construct(private int $id) {}
来源：http://fsy.tanke756.top

[U51] PHP：数组解构
来源：http://ara.jqgfzy.top

[$a, $b] = $arr;
来源：http://nau.zhaomingkeji.xyz

[U52] PHP：箭头函数
来源：http://jkk.shangyingyoupin.top

$double = fn($x) => $x * 2;
来源：http://hnk.jiagoushi.top

[U53] PHP：空合并运算符
来源：http://cmx.dianchejie.cn

$v = $a ?? $b ?? "default";
来源：http://tlw.yueranfly.top

[U54] PHP：空安全调用
来源：http://abe.xylfe.cn

$obj?->method()
来源：http://bhi.ehwqpu.com

[U55] PHP：match 表达式
来源：http://zlu.gotoacloud.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://htc.jinqigufen.top

[U56] PHP：命名参数
来源：http://zow.yj202588.top

f(a: 1, b: 2)
来源：http://gdt.cashguo.top

[U57] PHP：字符串插值
来源：http://npc.yj20258.top

"值: {$a}"
来源：http://nvx.sufxvd.cn

[U58] PHP：数组三件套
来源：http://smp.shanyushiyangkeji.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vmp.zhongyouzk.top

[U59] PHP：自定义排序
来源：http://tzu.mhx1999.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dss.ybcxt.top

[U60] PHP：JSON 编解码
来源：http://iwa.dianchejie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vli.meibo888.top

[U61] PHP：正则
来源：http://hzd.tian-w.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lwk.cashguo.top

[U62] PHP：日期对象
来源：http://trl.chenzaomai.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://oav.xingfuxueyuan.xyz

[U63] PHP：文件读写
来源：http://zck.yj20258888.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gqf.jqgufenzy.top

[U64] PHP：目录遍历
来源：http://oyu.bbcook.cn

glob("dir/*.php");  scandir("dir");
来源：http://mhl.uphjek.com

[U65] PHP：会话
来源：http://gks.shzxlz.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://gev.yj20258888.top

[U66] PHP：设置 Cookie
来源：http://oej.bjfxy.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qkg.wangshuangyany.cn

[U67] PHP：处理文件上传
来源：http://knh.shanyushiyangkeji.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lkg.aizwys.cn

[U68] PHP：PDO 连接
来源：http://tcz.daxiang520.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://cza.dashuyun.cn

[U69] PHP：PDO 预处理
来源：http://vkh.jianghu66.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jgh.gaohongyu789.top

[U70] PHP：PDO 事务
来源：http://nnq.fengsongda.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://yoi.jqgufenzy.top

[U71] PHP：抛出异常
来源：http://eob.zhaomingkeji.xyz

throw new RuntimeException("失败", 500);
来源：http://got.gotoacloud.top

[U72] PHP：写错误日志
来源：http://sbn.feifeiyinyue.top

error_log("失败: " . $e->getMessage());
来源：http://upa.zdbjq.cn

[U73] PHP：读取 ini 配置
来源：http://dgr.hfpthk.cn

parse_ini_file("config.ini", true)
来源：http://jov.yueranfly.top

[U74] PHP：读取环境变量
来源：http://zdd.kuanghao11.cn

getenv("APP_ENV") ?: "production"
来源：http://sum.ybcxt.top

[U75] PHP：依赖注入
来源：http://jiy.ywan-chungtsiang.top

composer require psr/container
来源：http://zob.gaohongyu789.top

[U76] PHP：简单路由
来源：http://xzx.havefunace.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://msl.jinghuilouyu.cn

[U77] PHP：模板渲染
来源：http://kel.0kj1m.cn

composer require twig/twig
来源：http://nej.pycfn.com

[U78] PHP：单元测试
来源：http://zqs.jlsjyb.cn

composer require --dev phpunit/phpunit
来源：http://csr.gaohongyu789.top

[U79] PHP：静态分析
来源：http://und.zdqjudy.top

composer require --dev phpstan/phpstan
来源：http://dvk.chenlongwang.top

[U80] PHP：代码规范修复
来源：http://jnq.gzhubu.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://idt.zdqjudy.top

[U81] JS：初始化项目
来源：http://xqz.zdbjq.cn

npm init -y;  npm i express
来源：http://ylo.nanxuanxn.top

[U82] JS：package.json 脚本
来源：http://zct.bbcook.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://izi.zdqjudy.top

[U83] JS：ES Module 导入导出
来源：http://xei.daxiang520.top

export const a = 1;  import { a } from "./m.js";
来源：http://awp.316326.xyz

[U84] JS：CommonJS 写法
来源：http://zst.hfpthk.cn

module.exports = { a };  const { a } = require("./m");
来源：http://tum.ywan-chungtsiang.top

[U85] JS：可选链
来源：http://hsp.hongshengwenyu.top

a?.b?.c
来源：http://vbd.hongshengwenyu.top

[U86] JS：空值合并
来源：http://wtg.jqgufenzy.top

a ?? b
来源：http://vzz.ctjpmb.com

[U87] JS：解构默认值
来源：http://dfa.gotoacloud.top

const { a = 1, b = 2 } = obj;
来源：http://eph.guowangkeji.top

[U88] JS：对象展开合并
来源：http://eyl.bjfxy.top

{ ...a, ...b }
来源：http://wwk.guannengcc.top

[U89] JS：数组去重
来源：http://und.tian-w.cn

[...new Set(arr)]
来源：http://gdk.aizwys.cn

[U90] JS：数字数组排序
来源：http://xsq.hcnkem.com

[...arr].sort((a, b) => a - b)
来源：http://hch.nanxuanxn.top

[U91] JS：对象键值遍历
来源：http://lpr.shanyushiyangkeji.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rhx.zhiwuduotai.top

[U92] JS：深拷贝
来源：http://dsi.aibaodan.cn

structuredClone(obj)
来源：http://cse.jinyuanbaomall.cn

[U93] JS：模板字符串
来源：http://kgc.nanxuanxn.top

`共 ${n} 条`
来源：http://nha.tarul.cn

[U94] JS：箭头函数
来源：http://qdv.meibo888.top

const double = x => x * 2;
来源：http://zjv.yonumen.top

[U95] JS：Promise 包装
来源：http://rol.quarkkingdee.top

new Promise((resolve, reject) => {})
来源：http://gtx.vehdjk.com

[U96] JS：async/await 与异常
来源：http://nlg.tian-w.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dob.bjfxy.top

[U97] JS：并发请求
来源：http://kgx.jqgfzy.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://eqe.ctjpmb.com

[U98] JS：fetch 带 JSON
来源：http://woh.jinqigfzy.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://diz.yonumen.top

[U99] JS：事件监听
来源：http://czd.guowangkeji.top

el.addEventListener("click", e => {})
来源：http://uff.mhx1999.top

[U100] JS：DOM 查询
来源：http://wpa.vqdsnc.cn

document.querySelector(".item")
来源：http://ccs.wangdashe.top

[U101] JS：classList 操作
来源：http://kba.jinqigfzy.top

el.classList.toggle("active")
来源：http://umd.xingfuxueyuan.xyz

[U102] JS：本地存储
来源：http://tfz.yonumen.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://dcu.ppjwa.cn

[U103] JS：定时器
来源：http://umb.haohaochexian.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://upi.fehbvm.com

[U104] JS：防抖
来源：http://bwl.gzhubu.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jjh.ppjwa.cn

[U105] JS：节流
来源：http://ixf.sxryk.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gpr.bjfxy.top

[U106] JS：日期格式化
来源：http://foo.epnwcf.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cds.aizwys.cn

[U107] JS：数字千分位
来源：http://equ.xziqi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cis.yanxiufei.cn

[U108] JS：随机整数
来源：http://uva.9152youxi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rbi.cdnleiting.top

[U109] JS：数组分组
来源：http://eer.sxryk.cn

Object.groupBy(arr, x => x.type)
来源：http://hnc.fktsv.cn

[U110] JS：数组分块
来源：http://rce.guannengcc.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mkd.tarul.cn

[U111] JS：对象转 Map
来源：http://eez.daria6918.cn

new Map(Object.entries(obj))
来源：http://ntb.shzxlz.cn

[U112] JS：字符串补位
来源：http://sek.c1oappe.top

"7".padStart(3, "0")
来源：http://fvu.jinghuilouyu.cn

[U113] JS：正则替换全部
来源：http://lrv.fktsv.cn

s.replaceAll("a", "b")
来源：http://bep.tanke756.top

[U114] JS：JSON 深比较
来源：http://pff.nwbrower.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://geu.ivvv.top

[U115] JS：生成 UUID
来源：http://khz.jyoumei.cn

crypto.randomUUID()
来源：http://gkk.fengsongda.top

[U116] JS：类型检查（JSDoc）
来源：http://bpf.chenzaomai.com

/** @param {string} name */ function f(name) {}
来源：http://zbh.wangshuangyany.cn

[U117] JS：单元测试
来源：http://jxd.fzhhl.top

npm i -D vitest;  npx vitest
来源：http://dql.sufxvd.cn

[U118] JS：开发服务器
来源：http://tjk.tanke756.top

npm i -D vite;  npx vite
来源：http://fjq.jianghu66.top

[U119] JS：生产构建
来源：http://zay.52xcode.cn

npx vite build
来源：http://jvb.yueranfly.top

[U120] JS：读取环境变量（Vite）
来源：http://jyz.zhijiandao.cn

import.meta.env.VITE_API_URL
来源：http://jqd.jinqigufen.top

================================================================================
来源：http://tjb.cheryme.top

统计汇总
来源：http://dhn.bjfxy.top

================================================================================
来源：http://kdd.jianghu66.top

按语言统计（条）：
来源：http://ioz.chenzaomai.com

Python ......... 252
来源：http://yln.shangyingyoupin.top

PHP ............ 252
来源：http://ihk.quarkkingdee.top

JavaScript ..... 252
来源：http://uei.xuetiantiany.cn

TypeScript ..... 212
来源：http://ldt.ywan-chungtsiang.top

Java ........... 212
来源：http://fns.zhijiandao.cn

Go ............. 212
来源：http://shk.smart0.xyz

Ruby ........... 212
来源：http://tke.hywenlv.cn

C# ............. 212
来源：http://wwq.vehdjk.com

C .............. 30
来源：http://zvw.fktsv.cn

C++ ............ 30
来源：http://gms.jinghuilouyu.cn

SQL ............ 90
来源：http://dxe.gotoacloud.top

Bash ........... 80
来源：http://xth.yonumen.top

Kotlin ......... 15
来源：http://vzq.yuanzhike.top

Swift .......... 15
来源：http://ykr.quarkkingdee.top

Lua ............ 10
来源：http://zvn.gzhubu.top

Perl ........... 10
来源：http://zcl.snrcjt.cn

Scala .......... 10
来源：http://app.nanxinkj.top

------------------------------------
来源：http://opl.smart0.xyz

合计 ........... 2106 条
来源：http://hqz.gotoacloud.top

按章节统计：
来源：http://dgz.yueranfly.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://src.yuanzhike.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rhv.yj20258.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wca.yongpay.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://snp.hesvh.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fap.zhaomingkeji.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vrq.jinyuanbaomall.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://bxr.c1oappe.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://say.yj202588.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lwe.316326.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yin.xinyue.icu

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gxk.c1oappe.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ifi.bjfxy.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://anz.hysaishi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jyu.c1oappe.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://okx.epnwcf.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://gup.chenlongwang.top

Q SQL 专题                              90
来源：http://vwt.xuanzx.com

R Bash 专题                             80
来源：http://nws.cucudq.cn

S C / C++ 专题                          60
来源：http://pim.pycfn.com

T 其他语言补充                          60
来源：http://bgu.zdbjq.cn

U 高频实用片段                         120
来源：http://gkl.9152youxi.cn

------------------------------------
来源：http://nmy.daxiang520.top

合计                                  2106 条
来源：http://bjn.yuxming.cn

--------------------------------------------------------------------------------
来源：http://kjx.zhiwuduotai.top

使用提醒
来源：http://fzs.xuetiantiany.cn

--------------------------------------------------------------------------------
来源：http://fzv.sjlbkw.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wzz.shanyushiyangtech.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://rqv.nwbrower.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://oki.dianchejie.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://yxa.vqdsnc.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rqq.dashuyun.cn

—— 文件结束 ——
来源：http://thh.zdqjudy.top

================================================================================
来源：http://rsq.haohaochexian.top

程序语言常见例子速查手册（2024 版）
来源：http://qah.hnxiangtu.top

Common Programming Examples Cheat Book
来源：http://mpz.ydjk.org.cn

================================================================================
来源：http://xet.iojbl.cn


<!-- 参考信息 -->