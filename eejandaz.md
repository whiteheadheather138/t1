代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://wdi.hysaishi.cn

[T55] Scala：集合过滤
来源：http://icy.aibaodan.cn

List(1, 2, 3).filter(_ > 1)
来源：http://cks.sxryk.cn

[T56] Scala：样例类
来源：http://glq.wangdashe.top

case class User(name: String, age: Int)
来源：http://ezh.gzhubu.top

[T57] Scala：模式匹配
来源：http://gib.fehbvm.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://gro.jinghuilouyu.cn

[T58] Scala：函数定义
来源：http://ypr.daxiang520.top

def add(a: Int, b: Int): Int = a + b
来源：http://utq.yanxiufei.cn

[T59] Scala：循环
来源：http://brv.chenlongwang.top

for (i <- 1 to 10) println(i)
来源：http://nwk.feifeiyinyue.top

[T60] Scala：折叠
来源：http://sdl.shanyushiyangkeji.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gmg.yfazqb.com

================================================================================
来源：http://nmv.andypj.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://flt.sysykeji.top

================================================================================
来源：http://rwo.kuanghao11.cn

[U01] Py：创建虚拟环境
来源：http://bkz.yongpay.top

python -m venv .venv && source .venv/bin/activate
来源：http://mgr.cdnleiting.top

[U02] Py：导出 / 安装依赖
来源：http://csg.nanxinkj.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gup.epnwcf.com

[U03] Py：加载 .env 配置
来源：http://kva.yanxiufei.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xyb.ydzc1.top

[U04] Py：变量调试打印
来源：http://pif.epnwcf.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jig.shanyushiyangtech.top

[U05] Py：列表去重且保序
来源：http://env.hnqzz.top

list(dict.fromkeys(arr))
来源：http://qfy.zhaomingkeji.xyz

[U06] Py：合并两个字典
来源：http://viq.dianchejie.cn

{**a, **b}
来源：http://kij.fehbvm.com

[U07] Py：反转字典键值
来源：http://mel.aibaodan.cn

{v: k for k, v in d.items()}
来源：http://ium.dashuyun.cn

[U08] Py：展平二维列表
来源：http://mni.tianlin.xyz

[y for x in nested for y in x]
来源：http://reb.jinyuanbaomall.cn

[U09] Py：字典取最大值的键
来源：http://wpz.hammf.cn

max(d, key=d.get)
来源：http://oei.hongshengwenyu.top

[U10] Py：按值排序字典
来源：http://eax.yangfankeji.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uxb.svipenyu.cn

[U11] Py：生成器表达式
来源：http://pqe.uphjek.com

(x * 2 for x in arr)
来源：http://pfp.vehdjk.com

[U12] Py：取出现最多的 3 个元素
来源：http://dui.aibaodan.cn

Counter(arr).most_common(3)
来源：http://sju.sjlbkw.cn

[U13] Py：固定长度队列
来源：http://cwo.pengpengdd.cyou

deque(maxlen=10)
来源：http://mum.jinqigfzy.top

[U14] Py：分组收集到列表
来源：http://zlu.kuanghao11.cn

defaultdict(list)
来源：http://jda.chenzaomai.com

[U15] Py：高精度计时
来源：http://tgx.nanxinkj.top

t = time.perf_counter()
来源：http://wqk.gogol.net.cn

[U16] Py：命令行参数解析
来源：http://rmf.hysaishi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qul.316326.xyz

[U17] Py：初始化日志
来源：http://vow.jinqigufen.top

logging.basicConfig(level=logging.INFO)
来源：http://iuc.havefunace.top

[U18] Py：预编译正则
来源：http://piz.hongshengwenyu.top

pat = re.compile(r"\d+")
来源：http://drg.shzxlz.cn

[U19] Py：正则替换带回调
来源：http://xcs.ywan-chungtsiang.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vet.yvedp.cn

[U20] Py：缓存函数结果
来源：http://sbi.chenjidiqi.icu

@functools.lru_cache(maxsize=None)
来源：http://pgs.chenjidiqi.icu

[U21] Py：自定义上下文管理器
来源：http://gqx.ybcxt.top

@contextlib.contextmanager
来源：http://cge.ctjpmb.com

[U22] Py：矩阵转置
来源：http://ive.andypj.xyz

list(zip(*m))
来源：http://xmv.yfazqb.com

[U23] Py：分块读取大文件
来源：http://zbz.andypj.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ifj.bbcook.cn

[U24] Py：路径操作
来源：http://zdf.fengsongda.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blh.fktsv.cn

[U25] Py：CSV 按字典读
来源：http://hcu.zycfv.cn

csv.DictReader(f)
来源：http://gjk.fanxiaobao.xyz

[U26] Py：并发下载
来源：http://eix.yuxming.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://obt.yueranfly.top

[U27] Py：异步 HTTP
来源：http://rof.fktsv.cn

aiohttp.ClientSession() 配合 async with
来源：http://qvc.jianghu66.top

[U28] Py：类型别名
来源：http://wvd.xylfe.cn

UserId = int
来源：http://oei.yuxming.cn

[U29] Py：属性校验
来源：http://zlg.jinyuanbaomall.cn

@property 与 @x.setter 配合
来源：http://sjv.yuxming.cn

[U30] Py：数据类
来源：http://yyt.fehbvm.com

@dataclass(slots=True)
来源：http://irm.cheryme.top

[U31] Py：单测
来源：http://mln.zhixingplan.top

python -m pytest -q
来源：http://bmz.tian-w.cn

[U32] Py：代码格式化
来源：http://oru.bbcook.cn

ruff format . && ruff check --fix .
来源：http://tib.cucudq.cn

[U33] Py：打包发布
来源：http://bfv.hongshengwenyu.top

python -m build  （依赖 pyproject.toml）
来源：http://dfu.zdqjudy.top

[U34] Py：判断编码
来源：http://gbj.yanxiufei.cn

chardet.detect(raw)
来源：http://jxd.smart0.xyz

[U35] Py：发送邮件
来源：http://ewd.sjlbkw.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://waa.hcnkem.com

[U36] Py：定时任务
来源：http://urw.yvedp.cn

schedule.every(10).minutes.do(job)
来源：http://dwx.zhixingplan.top

[U37] Py：读写 Excel
来源：http://oce.hnxiangtu.top

pandas.read_excel / DataFrame.to_excel
来源：http://cqr.zhengqikj.top

[U38] Py：获取脚本所在目录
来源：http://bid.pengpengdd.cyou

Path(__file__).resolve().parent
来源：http://pso.jianghu66.top

[U39] Py：判断是否在交互环境
来源：http://ctk.yongpay.top

sys.stdout.isatty()
来源：http://kpw.fktsv.cn

[U40] Py：打印到标准错误
来源：http://ttu.chenzaomai.com

print("err", file=sys.stderr)
来源：http://tio.yonumen.top

[U41] PHP：初始化 Composer 项目
来源：http://gdt.yj202588.top

composer init;  composer require guzzlehttp/guzzle
来源：http://iti.cdnleiting.top

[U42] PHP：PSR-4 自动加载
来源：http://fnu.gotoacloud.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wth.zdbjq.cn

[U43] PHP：声明命名空间
来源：http://emc.uphjek.com

namespace App\Http;
来源：http://ned.zhiwuduotai.top

[U44] PHP：开启严格类型
来源：http://xce.cheryme.top

declare(strict_types=1);
来源：http://ksm.cheryme.top

[U45] PHP：类型声明与返回类型
来源：http://pxv.andypj.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://ubf.chenjidiqi.icu

[U46] PHP：可空类型
来源：http://bqm.gzhubu.top

?string $name = null
来源：http://yxc.zycfv.cn

[U47] PHP：联合类型
来源：http://vax.pengpengdd.cyou

int|string $id
来源：http://uwm.pengpengdd.cyou

[U48] PHP：纯枚举
来源：http://kdy.jianghu66.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://iqz.zhongyouzk.top

[U49] PHP：只读属性
来源：http://ygq.gzhubu.top

public readonly string $name
来源：http://iyx.shanyushiyangtech.top

[U50] PHP：构造器属性提升
来源：http://sgl.jinyuanbaomall.cn

public function __construct(private int $id) {}
来源：http://bll.sweek.top

[U51] PHP：数组解构
来源：http://tzk.aizwys.cn

[$a, $b] = $arr;
来源：http://vzy.cashguo.top

[U52] PHP：箭头函数
来源：http://fzu.yj20258888.top

$double = fn($x) => $x * 2;
来源：http://opf.yj202588.top

[U53] PHP：空合并运算符
来源：http://bkr.aizwys.cn

$v = $a ?? $b ?? "default";
来源：http://mor.yj20258.top

[U54] PHP：空安全调用
来源：http://pye.quarkkingdee.top

$obj?->method()
来源：http://xhe.quarkkingdee.top

[U55] PHP：match 表达式
来源：http://bwe.bbcook.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ppi.aibaodan.cn

[U56] PHP：命名参数
来源：http://jbg.zhongyouzk.top

f(a: 1, b: 2)
来源：http://ldz.svipenyu.cn

[U57] PHP：字符串插值
来源：http://txm.xylfe.cn

"值: {$a}"
来源：http://iqb.nanxinkj.top

[U58] PHP：数组三件套
来源：http://ahm.hnqzz.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://eln.daxiang520.top

[U59] PHP：自定义排序
来源：http://lsz.xylfe.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mgt.andypj.xyz

[U60] PHP：JSON 编解码
来源：http://vbj.shzxlz.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vqi.ybcxt.top

[U61] PHP：正则
来源：http://jgw.pycfn.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pxf.haohaochexian.top

[U62] PHP：日期对象
来源：http://oss.snrcjt.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hhb.hcnkem.com

[U63] PHP：文件读写
来源：http://ejd.sweek.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://raq.snrcjt.cn

[U64] PHP：目录遍历
来源：http://vcp.ctjpmb.com

glob("dir/*.php");  scandir("dir");
来源：http://yst.zhengqikj.top

[U65] PHP：会话
来源：http://soa.ivvv.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ywf.fktsv.cn

[U66] PHP：设置 Cookie
来源：http://tdu.hcnkem.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sws.jqgfzy.top

[U67] PHP：处理文件上传
来源：http://jgo.hfpthk.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://sjm.zhoulong.xyz

[U68] PHP：PDO 连接
来源：http://zrb.sweek.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wrw.yj20258888.top

[U69] PHP：PDO 预处理
来源：http://vhq.hnxiangtu.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yyy.gzhubu.top

[U70] PHP：PDO 事务
来源：http://glj.zhaomingkeji.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rzd.chenjidiqi.icu

[U71] PHP：抛出异常
来源：http://mdt.hongshengwenyu.top

throw new RuntimeException("失败", 500);
来源：http://roh.ybcxt.top

[U72] PHP：写错误日志
来源：http://ikv.xylfe.cn

error_log("失败: " . $e->getMessage());
来源：http://aig.yj20258.top

[U73] PHP：读取 ini 配置
来源：http://rtq.gotoacloud.top

parse_ini_file("config.ini", true)
来源：http://xsx.havefunace.top

[U74] PHP：读取环境变量
来源：http://sos.chenlongwang.top

getenv("APP_ENV") ?: "production"
来源：http://qtc.zhoulong.xyz

[U75] PHP：依赖注入
来源：http://hvy.havefunace.top

composer require psr/container
来源：http://kco.sjlbkw.cn

[U76] PHP：简单路由
来源：http://rhe.nanxinkj.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zdp.hcnkem.com

[U77] PHP：模板渲染
来源：http://lxj.jqgfzy.top

composer require twig/twig
来源：http://wmh.zhijiandao.cn

[U78] PHP：单元测试
来源：http://tjk.ppjwa.cn

composer require --dev phpunit/phpunit
来源：http://dzg.yj202588.top

[U79] PHP：静态分析
来源：http://cww.tanke756.top

composer require --dev phpstan/phpstan
来源：http://uzf.shanyushiyangkeji.top

[U80] PHP：代码规范修复
来源：http://ilv.ydzc1.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ujk.hnqzz.top

[U81] JS：初始化项目
来源：http://ppw.fktsv.cn

npm init -y;  npm i express
来源：http://ssc.fengsongda.top

[U82] JS：package.json 脚本
来源：http://kcb.jqgufenzy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pgq.yuxming.cn

[U83] JS：ES Module 导入导出
来源：http://wrl.zdqjudy.top

export const a = 1;  import { a } from "./m.js";
来源：http://vuk.cashguo.top

[U84] JS：CommonJS 写法
来源：http://ocj.sufxvd.cn

module.exports = { a };  const { a } = require("./m");
来源：http://lmb.yj202588.top

[U85] JS：可选链
来源：http://rff.kuanghao11.cn

a?.b?.c
来源：http://ory.ywan-chungtsiang.top

[U86] JS：空值合并
来源：http://jbn.aizwys.cn

a ?? b
来源：http://ogl.quarkkingdee.top

[U87] JS：解构默认值
来源：http://dcd.jqgufenzy.top

const { a = 1, b = 2 } = obj;
来源：http://ygp.shzxlz.cn

[U88] JS：对象展开合并
来源：http://hcm.hnxiangtu.top

{ ...a, ...b }
来源：http://gni.gogol.net.cn

[U89] JS：数组去重
来源：http://ykj.sjlbkw.cn

[...new Set(arr)]
来源：http://kom.jlsjyb.cn

[U90] JS：数字数组排序
来源：http://dtb.zdqjudy.top

[...arr].sort((a, b) => a - b)
来源：http://csw.fktsv.cn

[U91] JS：对象键值遍历
来源：http://glf.bbcook.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vlr.zhoulong.xyz

[U92] JS：深拷贝
来源：http://lan.0kj1m.cn

structuredClone(obj)
来源：http://uyy.hcnkem.com

[U93] JS：模板字符串
来源：http://pkv.xylfe.cn

`共 ${n} 条`
来源：http://wbn.yfazqb.com

[U94] JS：箭头函数
来源：http://olw.haohaochexian.top

const double = x => x * 2;
来源：http://usx.jinqigufen.top

[U95] JS：Promise 包装
来源：http://tgy.snrcjt.cn

new Promise((resolve, reject) => {})
来源：http://wdc.jiagoushi.top

[U96] JS：async/await 与异常
来源：http://mcb.zdbjq.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://kee.ctjpmb.com

[U97] JS：并发请求
来源：http://mgh.fehbvm.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://cqy.ywan-chungtsiang.top

[U98] JS：fetch 带 JSON
来源：http://hwh.shzxlz.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://axr.ppjwa.cn

[U99] JS：事件监听
来源：http://dhm.smart0.xyz

el.addEventListener("click", e => {})
来源：http://fne.zhongyouzk.top

[U100] JS：DOM 查询
来源：http://wge.sxryk.cn

document.querySelector(".item")
来源：http://kzj.gaohongyu789.top

[U101] JS：classList 操作
来源：http://fsn.snrcjt.cn

el.classList.toggle("active")
来源：http://aps.xinyue.icu

[U102] JS：本地存储
来源：http://los.shuidangran.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://sbi.shzxlz.cn

[U103] JS：定时器
来源：http://cjl.ybcxt.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qeu.guowangkeji.top

[U104] JS：防抖
来源：http://njy.fengsongda.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nrc.jqgfzy.top

[U105] JS：节流
来源：http://wgi.zdqjudy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jaw.xuetiantiany.cn

[U106] JS：日期格式化
来源：http://knt.fehbvm.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jvd.dashuyun.cn

[U107] JS：数字千分位
来源：http://dot.yuanzhike.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://okr.yangfankeji.com

[U108] JS：随机整数
来源：http://lxm.aibaodan.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xwm.sxryk.cn

[U109] JS：数组分组
来源：http://wrh.sysykeji.top

Object.groupBy(arr, x => x.type)
来源：http://qhu.jinqigfzy.top

[U110] JS：数组分块
来源：http://rxp.hnxiangtu.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://iqi.cqqwz.cn

[U111] JS：对象转 Map
来源：http://yeu.chenjidiqi.icu

new Map(Object.entries(obj))
来源：http://jzc.jiagoushi.top

[U112] JS：字符串补位
来源：http://rib.birdmap.top

"7".padStart(3, "0")
来源：http://bgu.epnwcf.com

[U113] JS：正则替换全部
来源：http://xbw.fanxiaobao.xyz

s.replaceAll("a", "b")
来源：http://ynt.wangshuangyany.cn

[U114] JS：JSON 深比较
来源：http://glp.yfazqb.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://qjm.hongshengwenyu.top

[U115] JS：生成 UUID
来源：http://lph.yongpay.top

crypto.randomUUID()
来源：http://ezp.dianchejie.cn

[U116] JS：类型检查（JSDoc）
来源：http://kzc.kuanghao11.cn

/** @param {string} name */ function f(name) {}
来源：http://qij.snrcjt.cn

[U117] JS：单元测试
来源：http://rib.ppjwa.cn

npm i -D vitest;  npx vitest
来源：http://rlg.xylfe.cn

[U118] JS：开发服务器
来源：http://cxb.quarkkingdee.top

npm i -D vite;  npx vite
来源：http://jcn.guannengcc.top

[U119] JS：生产构建
来源：http://cjl.ydjk.org.cn

npx vite build
来源：http://rro.sxryk.cn

[U120] JS：读取环境变量（Vite）
来源：http://bjm.chenlongwang.top

import.meta.env.VITE_API_URL
来源：http://dzq.jinqigufen.top

================================================================================
来源：http://ybp.tanke756.top

统计汇总
来源：http://qrw.ehwqpu.com

================================================================================
来源：http://ins.pycfn.com

按语言统计（条）：
来源：http://rwl.cqqwz.cn

Python ......... 252
来源：http://nnz.epnwcf.com

PHP ............ 252
来源：http://ejk.uphjek.com

JavaScript ..... 252
来源：http://jlo.zhiwuduotai.top

TypeScript ..... 212
来源：http://gab.zdbjq.cn

Java ........... 212
来源：http://jhr.shanyushiyangtech.top

Go ............. 212
来源：http://ngy.pycfn.com

Ruby ........... 212
来源：http://beq.mhx1999.top

C# ............. 212
来源：http://yki.jlsjyb.cn

C .............. 30
来源：http://ccx.hnqzz.top

C++ ............ 30
来源：http://kyq.cheryme.top

SQL ............ 90
来源：http://dvc.birdmap.top

Bash ........... 80
来源：http://dkz.svipenyu.cn

Kotlin ......... 15
来源：http://urk.hywenlv.cn

Swift .......... 15
来源：http://bre.fanxiaobao.xyz

Lua ............ 10
来源：http://wkk.fanxiaobao.xyz

Perl ........... 10
来源：http://zcu.yonumen.top

Scala .......... 10
来源：http://rty.zdqjudy.top

------------------------------------
来源：http://aok.hesvh.cn

合计 ........... 2106 条
来源：http://wng.wangdashe.top

按章节统计：
来源：http://grj.zdbjq.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fhq.epnwcf.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://seq.kuanghao11.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mgu.gzhubu.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://jlv.sjlbkw.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fja.vqdsnc.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qke.yongpay.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://pwd.shanyushiyangtech.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nrw.jinyuanbaomall.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qlm.vqdsnc.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://lmd.snrcjt.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://viz.tanke756.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zef.pycfn.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mhd.zhengqikj.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://lph.sysykeji.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bxe.yfazqb.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bab.uphjek.com

Q SQL 专题                              90
来源：http://iwa.zhongyouzk.top

R Bash 专题                             80
来源：http://pvh.316326.xyz

S C / C++ 专题                          60
来源：http://cxj.hysaishi.cn

T 其他语言补充                          60
来源：http://jgy.shanyushiyangtech.top


<!-- 参考信息 -->