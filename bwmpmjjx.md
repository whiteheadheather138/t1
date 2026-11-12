代发 wailian999

[U01] Py：创建虚拟环境
来源：http://hxh.sxryk.cn

python -m venv .venv && source .venv/bin/activate
来源：http://kqk.zhoulong.xyz

[U02] Py：导出 / 安装依赖
来源：http://ypb.vehdjk.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qrl.daria6918.cn

[U03] Py：加载 .env 配置
来源：http://dnx.guowangkeji.top

from dotenv import load_dotenv; load_dotenv()
来源：http://kxd.zhixingplan.top

[U04] Py：变量调试打印
来源：http://wdu.yuanzhike.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://urs.ppjwa.cn

[U05] Py：列表去重且保序
来源：http://ayy.yangfankeji.com

list(dict.fromkeys(arr))
来源：http://ivl.hfpthk.cn

[U06] Py：合并两个字典
来源：http://txj.vehdjk.com

{**a, **b}
来源：http://wlx.cashguo.top

[U07] Py：反转字典键值
来源：http://qhi.9152youxi.cn

{v: k for k, v in d.items()}
来源：http://pio.nanxinkj.top

[U08] Py：展平二维列表
来源：http://gkf.gzhubu.top

[y for x in nested for y in x]
来源：http://ekb.ehwqpu.com

[U09] Py：字典取最大值的键
来源：http://aef.zdqjudy.top

max(d, key=d.get)
来源：http://cie.aibaodan.cn

[U10] Py：按值排序字典
来源：http://mzl.meibo888.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wnp.wangdashe.top

[U11] Py：生成器表达式
来源：http://gjk.cdnleiting.top

(x * 2 for x in arr)
来源：http://pnr.yanxiufei.cn

[U12] Py：取出现最多的 3 个元素
来源：http://pqf.yangfankeji.com

Counter(arr).most_common(3)
来源：http://azu.fzhhl.top

[U13] Py：固定长度队列
来源：http://kon.hammf.cn

deque(maxlen=10)
来源：http://aes.yanxiufei.cn

[U14] Py：分组收集到列表
来源：http://wno.meibo888.top

defaultdict(list)
来源：http://xxm.pycfn.com

[U15] Py：高精度计时
来源：http://jla.uphjek.com

t = time.perf_counter()
来源：http://odf.hnxiangtu.top

[U16] Py：命令行参数解析
来源：http://snh.ywan-chungtsiang.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kpi.yj202588.top

[U17] Py：初始化日志
来源：http://epp.xuetiantiany.cn

logging.basicConfig(level=logging.INFO)
来源：http://okt.hnqzz.top

[U18] Py：预编译正则
来源：http://omm.gogol.net.cn

pat = re.compile(r"\d+")
来源：http://gsm.iojbl.cn

[U19] Py：正则替换带回调
来源：http://jdl.jinqigufen.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qfp.yuanzhike.top

[U20] Py：缓存函数结果
来源：http://lmq.dianchejie.cn

@functools.lru_cache(maxsize=None)
来源：http://mpk.haohaochexian.top

[U21] Py：自定义上下文管理器
来源：http://heq.hesvh.cn

@contextlib.contextmanager
来源：http://pnw.uphjek.com

[U22] Py：矩阵转置
来源：http://wey.pengpengdd.cyou

list(zip(*m))
来源：http://roe.hnqzz.top

[U23] Py：分块读取大文件
来源：http://ckk.hammf.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hvl.ivvv.top

[U24] Py：路径操作
来源：http://zfg.xingfuxueyuan.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://osv.fehbvm.com

[U25] Py：CSV 按字典读
来源：http://aje.ppjwa.cn

csv.DictReader(f)
来源：http://lei.nanxinkj.top

[U26] Py：并发下载
来源：http://xsw.iojbl.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://uza.hesvh.cn

[U27] Py：异步 HTTP
来源：http://xkh.jiagoushi.top

aiohttp.ClientSession() 配合 async with
来源：http://ugw.zycfv.cn

[U28] Py：类型别名
来源：http://xae.zhoulong.xyz

UserId = int
来源：http://ncz.tanke756.top

[U29] Py：属性校验
来源：http://vai.ctjpmb.com

@property 与 @x.setter 配合
来源：http://svz.cucudq.cn

[U30] Py：数据类
来源：http://ewx.fehbvm.com

@dataclass(slots=True)
来源：http://owe.guowangkeji.top

[U31] Py：单测
来源：http://pzl.jianghu66.top

python -m pytest -q
来源：http://dto.gaohongyu789.top

[U32] Py：代码格式化
来源：http://rnn.tanke756.top

ruff format . && ruff check --fix .
来源：http://rca.shanyushiyangtech.top

[U33] Py：打包发布
来源：http://lyg.cqqwz.cn

python -m build  （依赖 pyproject.toml）
来源：http://anq.chenzaomai.com

[U34] Py：判断编码
来源：http://bso.aibaodan.cn

chardet.detect(raw)
来源：http://akf.uphjek.com

[U35] Py：发送邮件
来源：http://rat.nwbrower.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ctd.fengsongda.top

[U36] Py：定时任务
来源：http://kjz.bjfxy.top

schedule.every(10).minutes.do(job)
来源：http://dgu.dashuyun.cn

[U37] Py：读写 Excel
来源：http://osk.yongpay.top

pandas.read_excel / DataFrame.to_excel
来源：http://hpj.ydjk.org.cn

[U38] Py：获取脚本所在目录
来源：http://wwu.yj20258.top

Path(__file__).resolve().parent
来源：http://awh.bjfxy.top

[U39] Py：判断是否在交互环境
来源：http://xgr.jqgfzy.top

sys.stdout.isatty()
来源：http://zye.chenlongwang.top

[U40] Py：打印到标准错误
来源：http://odv.yongpay.top

print("err", file=sys.stderr)
来源：http://mzk.yueranfly.top

[U41] PHP：初始化 Composer 项目
来源：http://nwy.zhongyouzk.top

composer init;  composer require guzzlehttp/guzzle
来源：http://vdb.zhixingplan.top

[U42] PHP：PSR-4 自动加载
来源：http://yik.jyoumei.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://laj.hammf.cn

[U43] PHP：声明命名空间
来源：http://kum.ywan-chungtsiang.top

namespace App\Http;
来源：http://iwv.zdbjq.cn

[U44] PHP：开启严格类型
来源：http://dzr.zhijiandao.cn

declare(strict_types=1);
来源：http://chx.316326.xyz

[U45] PHP：类型声明与返回类型
来源：http://sfo.xylfe.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://hfh.zhijiandao.cn

[U46] PHP：可空类型
来源：http://vsi.gzhubu.top

?string $name = null
来源：http://wbi.iojbl.cn

[U47] PHP：联合类型
来源：http://noj.hysaishi.cn

int|string $id
来源：http://cuu.guowangkeji.top

[U48] PHP：纯枚举
来源：http://vcc.yvedp.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tco.ctjpmb.com

[U49] PHP：只读属性
来源：http://epv.dianchejie.cn

public readonly string $name
来源：http://vve.0kj1m.cn

[U50] PHP：构造器属性提升
来源：http://mfa.zdqjudy.top

public function __construct(private int $id) {}
来源：http://ppt.xylfe.cn

[U51] PHP：数组解构
来源：http://bhi.jiagoushi.top

[$a, $b] = $arr;
来源：http://bzz.andypj.xyz

[U52] PHP：箭头函数
来源：http://ivf.yangfankeji.com

$double = fn($x) => $x * 2;
来源：http://tqz.guannengcc.top

[U53] PHP：空合并运算符
来源：http://pvw.yangfankeji.com

$v = $a ?? $b ?? "default";
来源：http://pgq.shzxlz.cn

[U54] PHP：空安全调用
来源：http://pgz.pengpengdd.cyou

$obj?->method()
来源：http://vej.bjfxy.top

[U55] PHP：match 表达式
来源：http://aqr.xuetiantiany.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ake.dashuyun.cn

[U56] PHP：命名参数
来源：http://qzw.tarul.cn

f(a: 1, b: 2)
来源：http://uei.ehwqpu.com

[U57] PHP：字符串插值
来源：http://ewh.nanxinkj.top

"值: {$a}"
来源：http://kxu.andypj.xyz

[U58] PHP：数组三件套
来源：http://ijd.daxiang520.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ebu.hysaishi.cn

[U59] PHP：自定义排序
来源：http://ijn.pengpengdd.cyou

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tnn.yj20258888.top

[U60] PHP：JSON 编解码
来源：http://ufa.yvedp.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://evg.bbcook.cn

[U61] PHP：正则
来源：http://gta.shuidangran.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nbs.jqgfzy.top

[U62] PHP：日期对象
来源：http://icz.guannengcc.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://sla.tanke756.top

[U63] PHP：文件读写
来源：http://ivr.jiagoushi.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ctb.zdqjudy.top

[U64] PHP：目录遍历
来源：http://eqp.jqgfzy.top

glob("dir/*.php");  scandir("dir");
来源：http://ogo.zhijiandao.cn

[U65] PHP：会话
来源：http://jvj.xuanzx.com

session_start();  $_SESSION["uid"] = 1;
来源：http://gpr.hcnkem.com

[U66] PHP：设置 Cookie
来源：http://mvf.dashuyun.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://klz.ehwqpu.com

[U67] PHP：处理文件上传
来源：http://piw.yonumen.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zij.ydzc1.top

[U68] PHP：PDO 连接
来源：http://nye.gotoacloud.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ikd.meibo888.top

[U69] PHP：PDO 预处理
来源：http://vwe.hywenlv.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://esa.xuetiantiany.cn

[U70] PHP：PDO 事务
来源：http://ens.jinqigufen.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://azp.sjlbkw.cn

[U71] PHP：抛出异常
来源：http://kuq.tarul.cn

throw new RuntimeException("失败", 500);
来源：http://olt.xinyue.icu

[U72] PHP：写错误日志
来源：http://rat.fzhhl.top

error_log("失败: " . $e->getMessage());
来源：http://bbk.zhengqikj.top

[U73] PHP：读取 ini 配置
来源：http://xis.jinyuanbaomall.cn

parse_ini_file("config.ini", true)
来源：http://fbp.tarul.cn

[U74] PHP：读取环境变量
来源：http://sfr.dianchejie.cn

getenv("APP_ENV") ?: "production"
来源：http://pgz.fehbvm.com

[U75] PHP：依赖注入
来源：http://ncw.chenlongwang.top

composer require psr/container
来源：http://sma.hysaishi.cn

[U76] PHP：简单路由
来源：http://pap.yj20258.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fut.nanxinkj.top

[U77] PHP：模板渲染
来源：http://xcb.ehwqpu.com

composer require twig/twig
来源：http://jbz.xingfuxueyuan.xyz

[U78] PHP：单元测试
来源：http://krg.jinqigufen.top

composer require --dev phpunit/phpunit
来源：http://liv.hesvh.cn

[U79] PHP：静态分析
来源：http://lxx.hammf.cn

composer require --dev phpstan/phpstan
来源：http://vbn.pycfn.com

[U80] PHP：代码规范修复
来源：http://wof.bbcook.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://exn.52xcode.cn

[U81] JS：初始化项目
来源：http://jmd.zhoulong.xyz

npm init -y;  npm i express
来源：http://fde.nanxinkj.top

[U82] JS：package.json 脚本
来源：http://mge.havefunace.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://uxh.svipenyu.cn

[U83] JS：ES Module 导入导出
来源：http://msv.smart0.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://iex.jinqigfzy.top

[U84] JS：CommonJS 写法
来源：http://qxv.cheryme.top

module.exports = { a };  const { a } = require("./m");
来源：http://omo.jinyuanbaomall.cn

[U85] JS：可选链
来源：http://nvm.zhixingplan.top

a?.b?.c
来源：http://ilo.fanxiaobao.xyz

[U86] JS：空值合并
来源：http://jhf.0kj1m.cn

a ?? b
来源：http://epe.uphjek.com

[U87] JS：解构默认值
来源：http://pqa.andypj.xyz

const { a = 1, b = 2 } = obj;
来源：http://hii.andypj.xyz

[U88] JS：对象展开合并
来源：http://gdu.dashuyun.cn

{ ...a, ...b }
来源：http://hrs.xylfe.cn

[U89] JS：数组去重
来源：http://kxg.9152youxi.cn

[...new Set(arr)]
来源：http://sld.ybcxt.top

[U90] JS：数字数组排序
来源：http://mau.zhoulong.xyz

[...arr].sort((a, b) => a - b)
来源：http://inu.dianchejie.cn

[U91] JS：对象键值遍历
来源：http://whv.xylfe.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://csy.hysaishi.cn

[U92] JS：深拷贝
来源：http://quh.zdqjudy.top

structuredClone(obj)
来源：http://pxm.nwbrower.top

[U93] JS：模板字符串
来源：http://ouj.shangyingyoupin.top

`共 ${n} 条`
来源：http://vnx.guannengcc.top

[U94] JS：箭头函数
来源：http://dcy.ywan-chungtsiang.top

const double = x => x * 2;
来源：http://sxh.pycfn.com

[U95] JS：Promise 包装
来源：http://gvw.quarkkingdee.top

new Promise((resolve, reject) => {})
来源：http://hye.yuanzhike.top

[U96] JS：async/await 与异常
来源：http://yhx.wangshuangyany.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://tjr.quarkkingdee.top

[U97] JS：并发请求
来源：http://oks.tianlin.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://bfl.cucudq.cn

[U98] JS：fetch 带 JSON
来源：http://lxh.xziqi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nmk.zhiwuduotai.top

[U99] JS：事件监听
来源：http://dhy.gotoacloud.top

el.addEventListener("click", e => {})
来源：http://qbg.ywan-chungtsiang.top

[U100] JS：DOM 查询
来源：http://vcl.yj202588.top

document.querySelector(".item")
来源：http://eaj.ywan-chungtsiang.top

[U101] JS：classList 操作
来源：http://gfd.vehdjk.com

el.classList.toggle("active")
来源：http://xev.jinqigfzy.top

[U102] JS：本地存储
来源：http://yai.feifeiyinyue.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://wwi.zhijiandao.cn

[U103] JS：定时器
来源：http://gin.sysykeji.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rrh.zhijiandao.cn

[U104] JS：防抖
来源：http://ubj.daxiang520.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zxb.vqdsnc.cn

[U105] JS：节流
来源：http://uuk.tarul.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://erh.sxryk.cn

[U106] JS：日期格式化
来源：http://tsr.xylfe.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dtm.chenzaomai.com

[U107] JS：数字千分位
来源：http://ljj.0kj1m.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ldu.daxiang520.top

[U108] JS：随机整数
来源：http://sla.gaohongyu789.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jyp.xylfe.cn

[U109] JS：数组分组
来源：http://eij.yonumen.top

Object.groupBy(arr, x => x.type)
来源：http://fqv.bbcook.cn

[U110] JS：数组分块
来源：http://drn.ppjwa.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ekc.yj20258.top

[U111] JS：对象转 Map
来源：http://pam.smart0.xyz

new Map(Object.entries(obj))
来源：http://dio.ppjwa.cn

[U112] JS：字符串补位
来源：http://ogq.ivvv.top

"7".padStart(3, "0")
来源：http://ibb.zdqjudy.top

[U113] JS：正则替换全部
来源：http://wpx.guannengcc.top

s.replaceAll("a", "b")
来源：http://cvp.yfazqb.com

[U114] JS：JSON 深比较
来源：http://fvc.ivvv.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://gec.chenzaomai.com

[U115] JS：生成 UUID
来源：http://mgt.shanyushiyangkeji.top

crypto.randomUUID()
来源：http://aro.tian-w.cn

[U116] JS：类型检查（JSDoc）
来源：http://pgu.316326.xyz

/** @param {string} name */ function f(name) {}
来源：http://pdw.cheryme.top

[U117] JS：单元测试
来源：http://ryh.bjfxy.top

npm i -D vitest;  npx vitest
来源：http://hxi.xingfuxueyuan.xyz

[U118] JS：开发服务器
来源：http://rae.epnwcf.com

npm i -D vite;  npx vite
来源：http://diz.zhaomingkeji.xyz

[U119] JS：生产构建
来源：http://ian.zhiwuduotai.top

npx vite build
来源：http://ikr.haohaochexian.top

[U120] JS：读取环境变量（Vite）
来源：http://exy.meibo888.top

import.meta.env.VITE_API_URL
来源：http://qxh.vqdsnc.cn

================================================================================
来源：http://kbb.meibo888.top

统计汇总
来源：http://mmp.svipenyu.cn

================================================================================
来源：http://hju.shangyingyoupin.top

按语言统计（条）：
来源：http://tcc.yj20258888.top

Python ......... 252
来源：http://fhx.sysykeji.top

PHP ............ 252
来源：http://hfl.snrcjt.cn

JavaScript ..... 252
来源：http://hnc.pycfn.com

TypeScript ..... 212
来源：http://zoz.fktsv.cn

Java ........... 212
来源：http://nsn.jyoumei.cn

Go ............. 212
来源：http://cjy.cucudq.cn

Ruby ........... 212
来源：http://mlm.chenjidiqi.icu

C# ............. 212
来源：http://dxt.uphjek.com

C .............. 30
来源：http://hmo.jqgufenzy.top

C++ ............ 30
来源：http://icd.tian-w.cn

SQL ............ 90
来源：http://brh.havefunace.top

Bash ........... 80
来源：http://oeq.sweek.top

Kotlin ......... 15
来源：http://phu.ivvv.top

Swift .......... 15
来源：http://zwe.fzhhl.top

Lua ............ 10
来源：http://kpe.hfpthk.cn

Perl ........... 10
来源：http://vqk.meibo888.top

Scala .......... 10
来源：http://lqm.nanxuanxn.top

------------------------------------
来源：http://rvh.nanxinkj.top

合计 ........... 2106 条
来源：http://fqf.cheryme.top

按章节统计：
来源：http://ztr.fengsongda.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dqh.xylfe.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://uzn.iojbl.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hze.sxryk.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://tte.jinqigfzy.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://djp.jiagoushi.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://jax.cheryme.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://gil.sxryk.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://bzc.ctjpmb.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://dbm.hnxiangtu.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ecf.zhixingplan.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xap.zhoulong.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://akh.yuanzhike.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://aup.daxiang520.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://din.zhixingplan.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ehn.aizwys.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://eak.sufxvd.cn

Q SQL 专题                              90
来源：http://qtj.jinyuanbaomall.cn

R Bash 专题                             80
来源：http://abk.quarkkingdee.top

S C / C++ 专题                          60
来源：http://xdy.xuanzx.com

T 其他语言补充                          60
来源：http://qxt.uphjek.com

U 高频实用片段                         120
来源：http://kga.dianchejie.cn

------------------------------------
来源：http://bsx.guowangkeji.top

合计                                  2106 条
来源：http://itf.hesvh.cn

--------------------------------------------------------------------------------
来源：http://tqh.haohaochexian.top

使用提醒
来源：http://iol.ydzc1.top

--------------------------------------------------------------------------------
来源：http://omt.316326.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://gwc.jinqigufen.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://sgc.ivvv.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ynq.bbcook.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://dzb.birdmap.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://utz.jqgufenzy.top

—— 文件结束 ——
来源：http://dsb.uphjek.com

================================================================================
来源：http://imp.gogol.net.cn

程序语言常见例子速查手册（2024 版）
来源：http://bnr.hfpthk.cn

Common Programming Examples Cheat Book
来源：http://wad.yanxiufei.cn

================================================================================
来源：http://sni.ehwqpu.com


<!-- 参考信息 -->