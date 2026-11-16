代发 wailian999

[U11] Py：生成器表达式
来源：http://sta.wangshuangyany.cn

(x * 2 for x in arr)
来源：http://vjz.nwbrower.top

[U12] Py：取出现最多的 3 个元素
来源：http://lce.gotoacloud.top

Counter(arr).most_common(3)
来源：http://tns.nwbrower.top

[U13] Py：固定长度队列
来源：http://zds.shanyushiyangkeji.top

deque(maxlen=10)
来源：http://qrs.shuidangran.top

[U14] Py：分组收集到列表
来源：http://zpd.gzhubu.top

defaultdict(list)
来源：http://ukc.cashguo.top

[U15] Py：高精度计时
来源：http://xef.ppjwa.cn

t = time.perf_counter()
来源：http://jwp.zhiwuduotai.top

[U16] Py：命令行参数解析
来源：http://fyi.fktsv.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nvf.tanke756.top

[U17] Py：初始化日志
来源：http://qlr.jiagoushi.top

logging.basicConfig(level=logging.INFO)
来源：http://mzc.xuanzx.com

[U18] Py：预编译正则
来源：http://pzn.birdmap.top

pat = re.compile(r"\d+")
来源：http://mwy.jinyuanbaomall.cn

[U19] Py：正则替换带回调
来源：http://oxd.andypj.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cqu.ppjwa.cn

[U20] Py：缓存函数结果
来源：http://diu.guowangkeji.top

@functools.lru_cache(maxsize=None)
来源：http://ogq.dianchejie.cn

[U21] Py：自定义上下文管理器
来源：http://vpa.fzhhl.top

@contextlib.contextmanager
来源：http://yfm.bjfxy.top

[U22] Py：矩阵转置
来源：http://sqt.pengpengdd.cyou

list(zip(*m))
来源：http://afx.yvedp.cn

[U23] Py：分块读取大文件
来源：http://tym.shangyingyoupin.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wbn.hcnkem.com

[U24] Py：路径操作
来源：http://sqr.shangyingyoupin.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://frp.hesvh.cn

[U25] Py：CSV 按字典读
来源：http://dal.xingfuxueyuan.xyz

csv.DictReader(f)
来源：http://nrw.chenjidiqi.icu

[U26] Py：并发下载
来源：http://uia.xuanzx.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://uro.xziqi.cn

[U27] Py：异步 HTTP
来源：http://wdu.pycfn.com

aiohttp.ClientSession() 配合 async with
来源：http://amr.yangfankeji.com

[U28] Py：类型别名
来源：http://uzp.pycfn.com

UserId = int
来源：http://tts.yj202588.top

[U29] Py：属性校验
来源：http://uar.ehwqpu.com

@property 与 @x.setter 配合
来源：http://fmt.jqgfzy.top

[U30] Py：数据类
来源：http://qds.smart0.xyz

@dataclass(slots=True)
来源：http://iba.yj20258888.top

[U31] Py：单测
来源：http://zhd.ppjwa.cn

python -m pytest -q
来源：http://xms.jqgufenzy.top

[U32] Py：代码格式化
来源：http://odf.xziqi.cn

ruff format . && ruff check --fix .
来源：http://tem.daxiang520.top

[U33] Py：打包发布
来源：http://mcf.hnqzz.top

python -m build  （依赖 pyproject.toml）
来源：http://czy.daria6918.cn

[U34] Py：判断编码
来源：http://fcz.jinqigfzy.top

chardet.detect(raw)
来源：http://fys.snrcjt.cn

[U35] Py：发送邮件
来源：http://vdu.vqdsnc.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dut.ywan-chungtsiang.top

[U36] Py：定时任务
来源：http://yli.jianghu66.top

schedule.every(10).minutes.do(job)
来源：http://hlz.nwbrower.top

[U37] Py：读写 Excel
来源：http://tlm.hcnkem.com

pandas.read_excel / DataFrame.to_excel
来源：http://ikk.wangshuangyany.cn

[U38] Py：获取脚本所在目录
来源：http://doo.birdmap.top

Path(__file__).resolve().parent
来源：http://hei.yj202588.top

[U39] Py：判断是否在交互环境
来源：http://poh.zhijiandao.cn

sys.stdout.isatty()
来源：http://pvu.shzxlz.cn

[U40] Py：打印到标准错误
来源：http://azh.meibo888.top

print("err", file=sys.stderr)
来源：http://gtv.hammf.cn

[U41] PHP：初始化 Composer 项目
来源：http://lpr.zhoulong.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://oeq.guowangkeji.top

[U42] PHP：PSR-4 自动加载
来源：http://waa.hesvh.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qhd.xylfe.cn

[U43] PHP：声明命名空间
来源：http://uuh.zhixingplan.top

namespace App\Http;
来源：http://zdx.jinghuilouyu.cn

[U44] PHP：开启严格类型
来源：http://mjm.ybcxt.top

declare(strict_types=1);
来源：http://sly.9152youxi.cn

[U45] PHP：类型声明与返回类型
来源：http://yqs.tian-w.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://tlq.fanxiaobao.xyz

[U46] PHP：可空类型
来源：http://biv.gogol.net.cn

?string $name = null
来源：http://gdg.shzxlz.cn

[U47] PHP：联合类型
来源：http://vqw.yonumen.top

int|string $id
来源：http://ygo.xziqi.cn

[U48] PHP：纯枚举
来源：http://bgr.aizwys.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://fpr.yvedp.cn

[U49] PHP：只读属性
来源：http://nkx.yanxiufei.cn

public readonly string $name
来源：http://qep.zdbjq.cn

[U50] PHP：构造器属性提升
来源：http://ssm.shzxlz.cn

public function __construct(private int $id) {}
来源：http://ius.yanxiufei.cn

[U51] PHP：数组解构
来源：http://tes.fzhhl.top

[$a, $b] = $arr;
来源：http://rpn.xinyue.icu

[U52] PHP：箭头函数
来源：http://vls.vehdjk.com

$double = fn($x) => $x * 2;
来源：http://ppm.sweek.top

[U53] PHP：空合并运算符
来源：http://rqg.pengpengdd.cyou

$v = $a ?? $b ?? "default";
来源：http://wrw.xinyue.icu

[U54] PHP：空安全调用
来源：http://idb.cheryme.top

$obj?->method()
来源：http://gfj.ywan-chungtsiang.top

[U55] PHP：match 表达式
来源：http://bse.hnqzz.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://cfj.nanxinkj.top

[U56] PHP：命名参数
来源：http://elw.zhiwuduotai.top

f(a: 1, b: 2)
来源：http://ahn.andypj.xyz

[U57] PHP：字符串插值
来源：http://nmb.havefunace.top

"值: {$a}"
来源：http://wat.zhixingplan.top

[U58] PHP：数组三件套
来源：http://uwj.cheryme.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pzw.jinqigfzy.top

[U59] PHP：自定义排序
来源：http://eie.nwbrower.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://flu.aibaodan.cn

[U60] PHP：JSON 编解码
来源：http://fuk.vqdsnc.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://frr.xziqi.cn

[U61] PHP：正则
来源：http://mga.yanxiufei.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xyh.fengsongda.top

[U62] PHP：日期对象
来源：http://pxj.zhiwuduotai.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jiu.xuanzx.com

[U63] PHP：文件读写
来源：http://ssq.andypj.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kdr.jqgufenzy.top

[U64] PHP：目录遍历
来源：http://qvb.guowangkeji.top

glob("dir/*.php");  scandir("dir");
来源：http://okn.ybcxt.top

[U65] PHP：会话
来源：http://rpo.xziqi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://dql.ydjk.org.cn

[U66] PHP：设置 Cookie
来源：http://vpl.pycfn.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ubl.hnxiangtu.top

[U67] PHP：处理文件上传
来源：http://upy.sysykeji.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://atk.daria6918.cn

[U68] PHP：PDO 连接
来源：http://fyi.fzhhl.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mqw.fanxiaobao.xyz

[U69] PHP：PDO 预处理
来源：http://ccn.mhx1999.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lxj.yfazqb.com

[U70] PHP：PDO 事务
来源：http://ngl.xingfuxueyuan.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gvg.jianghu66.top

[U71] PHP：抛出异常
来源：http://xoj.ydzc1.top

throw new RuntimeException("失败", 500);
来源：http://zbc.hywenlv.cn

[U72] PHP：写错误日志
来源：http://ywk.zhijiandao.cn

error_log("失败: " . $e->getMessage());
来源：http://bne.cqqwz.cn

[U73] PHP：读取 ini 配置
来源：http://ejk.yj20258888.top

parse_ini_file("config.ini", true)
来源：http://tbt.pengpengdd.cyou

[U74] PHP：读取环境变量
来源：http://wvy.pengpengdd.cyou

getenv("APP_ENV") ?: "production"
来源：http://oca.cashguo.top

[U75] PHP：依赖注入
来源：http://hee.yj202588.top

composer require psr/container
来源：http://dwx.52xcode.cn

[U76] PHP：简单路由
来源：http://lab.cashguo.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://teo.52xcode.cn

[U77] PHP：模板渲染
来源：http://oco.ctjpmb.com

composer require twig/twig
来源：http://eqv.fanxiaobao.xyz

[U78] PHP：单元测试
来源：http://csz.316326.xyz

composer require --dev phpunit/phpunit
来源：http://nju.xuanzx.com

[U79] PHP：静态分析
来源：http://dnr.smart0.xyz

composer require --dev phpstan/phpstan
来源：http://egk.svipenyu.cn

[U80] PHP：代码规范修复
来源：http://zgm.hfpthk.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://tho.gogol.net.cn

[U81] JS：初始化项目
来源：http://aux.xinyue.icu

npm init -y;  npm i express
来源：http://mfh.tanke756.top

[U82] JS：package.json 脚本
来源：http://blm.jinqigfzy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ydr.yuxming.cn

[U83] JS：ES Module 导入导出
来源：http://hjd.cqqwz.cn

export const a = 1;  import { a } from "./m.js";
来源：http://qim.yvedp.cn

[U84] JS：CommonJS 写法
来源：http://frd.316326.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://nxq.tarul.cn

[U85] JS：可选链
来源：http://pjq.shuidangran.top

a?.b?.c
来源：http://xvf.kuanghao11.cn

[U86] JS：空值合并
来源：http://pct.hnqzz.top

a ?? b
来源：http://eqy.vqdsnc.cn

[U87] JS：解构默认值
来源：http://tom.fanxiaobao.xyz

const { a = 1, b = 2 } = obj;
来源：http://ilq.gotoacloud.top

[U88] JS：对象展开合并
来源：http://fxq.ybcxt.top

{ ...a, ...b }
来源：http://yih.ehwqpu.com

[U89] JS：数组去重
来源：http://wah.shanyushiyangkeji.top

[...new Set(arr)]
来源：http://wqa.xuanzx.com

[U90] JS：数字数组排序
来源：http://cxo.bjfxy.top

[...arr].sort((a, b) => a - b)
来源：http://wxd.shzxlz.cn

[U91] JS：对象键值遍历
来源：http://pzr.yanxiufei.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://iox.yfazqb.com

[U92] JS：深拷贝
来源：http://muf.uphjek.com

structuredClone(obj)
来源：http://toh.fengsongda.top

[U93] JS：模板字符串
来源：http://iug.pengpengdd.cyou

`共 ${n} 条`
来源：http://ccd.cheryme.top

[U94] JS：箭头函数
来源：http://nan.zhongyouzk.top

const double = x => x * 2;
来源：http://ssa.ppjwa.cn

[U95] JS：Promise 包装
来源：http://wzw.gzhubu.top

new Promise((resolve, reject) => {})
来源：http://pdh.nwbrower.top

[U96] JS：async/await 与异常
来源：http://vei.zhongyouzk.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qzf.jqgfzy.top

[U97] JS：并发请求
来源：http://fki.52xcode.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://kbd.hywenlv.cn

[U98] JS：fetch 带 JSON
来源：http://yfa.zycfv.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ddg.dianchejie.cn

[U99] JS：事件监听
来源：http://yom.316326.xyz

el.addEventListener("click", e => {})
来源：http://nwo.xingfuxueyuan.xyz

[U100] JS：DOM 查询
来源：http://ylp.tian-w.cn

document.querySelector(".item")
来源：http://whs.yangfankeji.com

[U101] JS：classList 操作
来源：http://enp.xuetiantiany.cn

el.classList.toggle("active")
来源：http://rzu.xinyue.icu

[U102] JS：本地存储
来源：http://byk.iojbl.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://irf.ppjwa.cn

[U103] JS：定时器
来源：http://dmi.xuanzx.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jfd.dianchejie.cn

[U104] JS：防抖
来源：http://mdl.316326.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rkx.smart0.xyz

[U105] JS：节流
来源：http://gij.jinqigufen.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://brp.kuanghao11.cn

[U106] JS：日期格式化
来源：http://ybq.feifeiyinyue.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vkv.hongshengwenyu.top

[U107] JS：数字千分位
来源：http://ksm.xziqi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xwa.ydjk.org.cn

[U108] JS：随机整数
来源：http://qhd.zhaomingkeji.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rxi.cashguo.top

[U109] JS：数组分组
来源：http://ioc.nanxinkj.top

Object.groupBy(arr, x => x.type)
来源：http://wma.birdmap.top

[U110] JS：数组分块
来源：http://toq.jinghuilouyu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lzi.vehdjk.com

[U111] JS：对象转 Map
来源：http://rnz.xinyue.icu

new Map(Object.entries(obj))
来源：http://lrn.shzxlz.cn

[U112] JS：字符串补位
来源：http://xsl.ydjk.org.cn

"7".padStart(3, "0")
来源：http://ujm.ydzc1.top

[U113] JS：正则替换全部
来源：http://iur.guannengcc.top

s.replaceAll("a", "b")
来源：http://pvq.yanxiufei.cn

[U114] JS：JSON 深比较
来源：http://eto.sxryk.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://gnl.shanyushiyangkeji.top

[U115] JS：生成 UUID
来源：http://ahp.zdbjq.cn

crypto.randomUUID()
来源：http://yjt.havefunace.top

[U116] JS：类型检查（JSDoc）
来源：http://wrp.xuetiantiany.cn

/** @param {string} name */ function f(name) {}
来源：http://lju.gotoacloud.top

[U117] JS：单元测试
来源：http://xsu.zdqjudy.top

npm i -D vitest;  npx vitest
来源：http://jfm.tarul.cn

[U118] JS：开发服务器
来源：http://onu.yuxming.cn

npm i -D vite;  npx vite
来源：http://umg.zhiwuduotai.top

[U119] JS：生产构建
来源：http://ilc.xinyue.icu

npx vite build
来源：http://pzw.chenjidiqi.icu

[U120] JS：读取环境变量（Vite）
来源：http://ubn.dashuyun.cn

import.meta.env.VITE_API_URL
来源：http://kjr.jinqigfzy.top

================================================================================
来源：http://rxh.hcnkem.com

统计汇总
来源：http://ayy.zhaomingkeji.xyz

================================================================================
来源：http://uqx.yj20258888.top

按语言统计（条）：
来源：http://gvz.zdbjq.cn

Python ......... 252
来源：http://alb.yangfankeji.com

PHP ............ 252
来源：http://cft.yvedp.cn

JavaScript ..... 252
来源：http://sth.birdmap.top

TypeScript ..... 212
来源：http://wcj.jinyuanbaomall.cn

Java ........... 212
来源：http://zlb.dashuyun.cn

Go ............. 212
来源：http://hgi.hcnkem.com

Ruby ........... 212
来源：http://uhv.zhengqikj.top

C# ............. 212
来源：http://gmn.hnqzz.top

C .............. 30
来源：http://kgk.fzhhl.top

C++ ............ 30
来源：http://cnr.gogol.net.cn

SQL ............ 90
来源：http://nfy.hnqzz.top

Bash ........... 80
来源：http://rqx.yuxming.cn

Kotlin ......... 15
来源：http://wgz.yuanzhike.top

Swift .......... 15
来源：http://iod.nwbrower.top

Lua ............ 10
来源：http://toz.cdnleiting.top

Perl ........... 10
来源：http://fch.nanxinkj.top

Scala .......... 10
来源：http://ocl.fanxiaobao.xyz

------------------------------------
来源：http://lbl.svipenyu.cn

合计 ........... 2106 条
来源：http://fqy.xylfe.cn

按章节统计：
来源：http://jvn.fzhhl.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wqa.haohaochexian.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://vcg.snrcjt.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jgj.yfazqb.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gsw.bbcook.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wtj.ywan-chungtsiang.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://kzv.xuetiantiany.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hhq.zycfv.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wka.chenzaomai.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://heu.tanke756.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vyi.jinyuanbaomall.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://yfp.zycfv.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vcp.yangfankeji.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://oyt.fktsv.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rxk.daria6918.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wrk.feifeiyinyue.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://auw.wangdashe.top

Q SQL 专题                              90
来源：http://pgd.cdnleiting.top

R Bash 专题                             80
来源：http://zgj.xuetiantiany.cn

S C / C++ 专题                          60
来源：http://ykk.zycfv.cn

T 其他语言补充                          60
来源：http://wnx.shzxlz.cn

U 高频实用片段                         120
来源：http://eoa.dashuyun.cn

------------------------------------
来源：http://uff.yongpay.top

合计                                  2106 条
来源：http://atz.nwbrower.top

--------------------------------------------------------------------------------
来源：http://pyy.yuanzhike.top

使用提醒
来源：http://wqz.zycfv.cn

--------------------------------------------------------------------------------
来源：http://kqe.fehbvm.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://iaq.ivvv.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wbc.jqgfzy.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://bhx.jyoumei.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://tbo.aibaodan.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wsm.gotoacloud.top

—— 文件结束 ——
来源：http://otp.yj202588.top

================================================================================
来源：http://ymo.ctjpmb.com

程序语言常见例子速查手册（2024 版）
来源：http://bcf.ybcxt.top

Common Programming Examples Cheat Book
来源：http://xui.birdmap.top

================================================================================
来源：http://jks.hesvh.cn

【收录内容】
来源：http://qst.zhoulong.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://kqg.chenzaomai.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://vve.redwolf501.top

SQL · Bash · C · C++
来源：http://nmd.52xcode.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://auc.ctjpmb.com

【使用说明】
来源：http://wkg.nwbrower.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://amb.iojbl.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ill.jqgufenzy.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://dwu.zhongyouzk.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://aks.zdbjq.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://wnf.jinghuilouyu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xxt.9152youxi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://lhs.yangfankeji.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://sce.xziqi.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://eal.jiagoushi.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hmo.andypj.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://toe.cqqwz.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://dbe.yueranfly.top

【文件统计】
来源：http://mcg.cashguo.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://srk.zhengqikj.top


<!-- 参考信息 -->