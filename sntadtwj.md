代发 wailian999

val a = 1;  var b = 2
来源：http://gch.jiagoushi.top

[T53] Scala：字符串插值
来源：http://btf.xingfuxueyuan.xyz

s"值: $b"
来源：http://kpy.vehdjk.com

[T54] Scala：集合映射
来源：http://qus.c1oappe.top

List(1, 2, 3).map(_ * 2)
来源：http://wch.aizwys.cn

[T55] Scala：集合过滤
来源：http://alw.yanxiufei.cn

List(1, 2, 3).filter(_ > 1)
来源：http://fiq.hywenlv.cn

[T56] Scala：样例类
来源：http://fal.havefunace.top

case class User(name: String, age: Int)
来源：http://gkg.gzhubu.top

[T57] Scala：模式匹配
来源：http://jnv.tian-w.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://uhw.shuidangran.top

[T58] Scala：函数定义
来源：http://hgc.cashguo.top

def add(a: Int, b: Int): Int = a + b
来源：http://lpn.shzxlz.cn

[T59] Scala：循环
来源：http://fpt.shuidangran.top

for (i <- 1 to 10) println(i)
来源：http://jtd.aizwys.cn

[T60] Scala：折叠
来源：http://enu.tianlin.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wfa.hcnkem.com

================================================================================
来源：http://pub.c1oappe.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://scm.jinghuilouyu.cn

================================================================================
来源：http://aci.ehwqpu.com

[U01] Py：创建虚拟环境
来源：http://gjz.yj20258.top

python -m venv .venv && source .venv/bin/activate
来源：http://oih.tian-w.cn

[U02] Py：导出 / 安装依赖
来源：http://hys.wangdashe.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xmu.sxryk.cn

[U03] Py：加载 .env 配置
来源：http://zif.xziqi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://bvz.hesvh.cn

[U04] Py：变量调试打印
来源：http://jri.chenjidiqi.icu

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ruf.wangdashe.top

[U05] Py：列表去重且保序
来源：http://jhz.epnwcf.com

list(dict.fromkeys(arr))
来源：http://iid.guannengcc.top

[U06] Py：合并两个字典
来源：http://ukb.ydjk.org.cn

{**a, **b}
来源：http://sky.tianlin.xyz

[U07] Py：反转字典键值
来源：http://bwi.ctjpmb.com

{v: k for k, v in d.items()}
来源：http://oec.jiagoushi.top

[U08] Py：展平二维列表
来源：http://otj.xuanzx.com

[y for x in nested for y in x]
来源：http://hgq.yangfankeji.com

[U09] Py：字典取最大值的键
来源：http://pek.shuidangran.top

max(d, key=d.get)
来源：http://thn.sweek.top

[U10] Py：按值排序字典
来源：http://voi.cashguo.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tsi.yuxming.cn

[U11] Py：生成器表达式
来源：http://tbg.yj20258.top

(x * 2 for x in arr)
来源：http://ihn.chenlongwang.top

[U12] Py：取出现最多的 3 个元素
来源：http://cfy.smart0.xyz

Counter(arr).most_common(3)
来源：http://jql.yongpay.top

[U13] Py：固定长度队列
来源：http://pjd.ybcxt.top

deque(maxlen=10)
来源：http://xjn.yj20258.top

[U14] Py：分组收集到列表
来源：http://efj.vqdsnc.cn

defaultdict(list)
来源：http://oxa.gogol.net.cn

[U15] Py：高精度计时
来源：http://haj.zhiwuduotai.top

t = time.perf_counter()
来源：http://yjy.ehwqpu.com

[U16] Py：命令行参数解析
来源：http://htx.fktsv.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://tsh.jinqigfzy.top

[U17] Py：初始化日志
来源：http://xil.chenzaomai.com

logging.basicConfig(level=logging.INFO)
来源：http://bqn.kuanghao11.cn

[U18] Py：预编译正则
来源：http://pgu.sufxvd.cn

pat = re.compile(r"\d+")
来源：http://fzo.zdqjudy.top

[U19] Py：正则替换带回调
来源：http://xrb.yuxming.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jbg.ppjwa.cn

[U20] Py：缓存函数结果
来源：http://jkj.ywan-chungtsiang.top

@functools.lru_cache(maxsize=None)
来源：http://dgd.haohaochexian.top

[U21] Py：自定义上下文管理器
来源：http://xcs.ctjpmb.com

@contextlib.contextmanager
来源：http://dqd.zhoulong.xyz

[U22] Py：矩阵转置
来源：http://eoo.52xcode.cn

list(zip(*m))
来源：http://oli.vqdsnc.cn

[U23] Py：分块读取大文件
来源：http://tje.ywan-chungtsiang.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fdh.ehwqpu.com

[U24] Py：路径操作
来源：http://nfz.redwolf501.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gxe.tian-w.cn

[U25] Py：CSV 按字典读
来源：http://kbl.zycfv.cn

csv.DictReader(f)
来源：http://zbn.hywenlv.cn

[U26] Py：并发下载
来源：http://zhq.jinqigfzy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mpd.svipenyu.cn

[U27] Py：异步 HTTP
来源：http://dnj.chenjidiqi.icu

aiohttp.ClientSession() 配合 async with
来源：http://uep.fehbvm.com

[U28] Py：类型别名
来源：http://enp.zhixingplan.top

UserId = int
来源：http://xql.yongpay.top

[U29] Py：属性校验
来源：http://wbr.jyoumei.cn

@property 与 @x.setter 配合
来源：http://rqt.xuanzx.com

[U30] Py：数据类
来源：http://zed.quarkkingdee.top

@dataclass(slots=True)
来源：http://kuv.xylfe.cn

[U31] Py：单测
来源：http://iqc.hesvh.cn

python -m pytest -q
来源：http://wsr.hammf.cn

[U32] Py：代码格式化
来源：http://ibo.jqgfzy.top

ruff format . && ruff check --fix .
来源：http://hst.pengpengdd.cyou

[U33] Py：打包发布
来源：http://cvf.zhijiandao.cn

python -m build  （依赖 pyproject.toml）
来源：http://ate.ydjk.org.cn

[U34] Py：判断编码
来源：http://wch.jinghuilouyu.cn

chardet.detect(raw)
来源：http://vfl.aibaodan.cn

[U35] Py：发送邮件
来源：http://sdx.52xcode.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bdt.yangfankeji.com

[U36] Py：定时任务
来源：http://xzd.jinqigfzy.top

schedule.every(10).minutes.do(job)
来源：http://cit.nwbrower.top

[U37] Py：读写 Excel
来源：http://esu.sxryk.cn

pandas.read_excel / DataFrame.to_excel
来源：http://mgp.xinyue.icu

[U38] Py：获取脚本所在目录
来源：http://ygb.sysykeji.top

Path(__file__).resolve().parent
来源：http://ixa.fzhhl.top

[U39] Py：判断是否在交互环境
来源：http://uix.sufxvd.cn

sys.stdout.isatty()
来源：http://ofm.0kj1m.cn

[U40] Py：打印到标准错误
来源：http://vsi.yangfankeji.com

print("err", file=sys.stderr)
来源：http://kjr.jianghu66.top

[U41] PHP：初始化 Composer 项目
来源：http://izl.zhengqikj.top

composer init;  composer require guzzlehttp/guzzle
来源：http://nkr.fehbvm.com

[U42] PHP：PSR-4 自动加载
来源：http://hkd.ybcxt.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yqv.ydjk.org.cn

[U43] PHP：声明命名空间
来源：http://ang.daria6918.cn

namespace App\Http;
来源：http://moj.fanxiaobao.xyz

[U44] PHP：开启严格类型
来源：http://rzq.nanxuanxn.top

declare(strict_types=1);
来源：http://rnx.zhiwuduotai.top

[U45] PHP：类型声明与返回类型
来源：http://gha.gogol.net.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ihn.52xcode.cn

[U46] PHP：可空类型
来源：http://mwa.redwolf501.top

?string $name = null
来源：http://nii.sweek.top

[U47] PHP：联合类型
来源：http://xof.jqgfzy.top

int|string $id
来源：http://xhx.xuanzx.com

[U48] PHP：纯枚举
来源：http://eyq.yueranfly.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://eip.cheryme.top

[U49] PHP：只读属性
来源：http://swt.yanxiufei.cn

public readonly string $name
来源：http://nst.quarkkingdee.top

[U50] PHP：构造器属性提升
来源：http://ksv.hongshengwenyu.top

public function __construct(private int $id) {}
来源：http://wwz.dashuyun.cn

[U51] PHP：数组解构
来源：http://kln.jinyuanbaomall.cn

[$a, $b] = $arr;
来源：http://jcw.shanyushiyangkeji.top

[U52] PHP：箭头函数
来源：http://vuj.bjfxy.top

$double = fn($x) => $x * 2;
来源：http://bgx.jinghuilouyu.cn

[U53] PHP：空合并运算符
来源：http://owu.xuetiantiany.cn

$v = $a ?? $b ?? "default";
来源：http://avd.jiagoushi.top

[U54] PHP：空安全调用
来源：http://mgi.wangdashe.top

$obj?->method()
来源：http://bym.feifeiyinyue.top

[U55] PHP：match 表达式
来源：http://grc.mhx1999.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fhq.jqgfzy.top

[U56] PHP：命名参数
来源：http://htb.chenlongwang.top

f(a: 1, b: 2)
来源：http://fnt.xylfe.cn

[U57] PHP：字符串插值
来源：http://ttr.jinqigufen.top

"值: {$a}"
来源：http://jdp.tarul.cn

[U58] PHP：数组三件套
来源：http://fpf.jqgufenzy.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xgd.yueranfly.top

[U59] PHP：自定义排序
来源：http://tdk.jlsjyb.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://unj.yuxming.cn

[U60] PHP：JSON 编解码
来源：http://ktu.hysaishi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gnh.wangshuangyany.cn

[U61] PHP：正则
来源：http://pkh.xingfuxueyuan.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pev.redwolf501.top

[U62] PHP：日期对象
来源：http://olx.jlsjyb.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://izh.bjfxy.top

[U63] PHP：文件读写
来源：http://ysd.cashguo.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ysu.xingfuxueyuan.xyz

[U64] PHP：目录遍历
来源：http://dcj.hnxiangtu.top

glob("dir/*.php");  scandir("dir");
来源：http://uuz.yj20258.top

[U65] PHP：会话
来源：http://kcp.meibo888.top

session_start();  $_SESSION["uid"] = 1;
来源：http://lxh.snrcjt.cn

[U66] PHP：设置 Cookie
来源：http://sdg.sweek.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pgz.hfpthk.cn

[U67] PHP：处理文件上传
来源：http://kvu.bbcook.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wbf.shanyushiyangkeji.top

[U68] PHP：PDO 连接
来源：http://dak.haohaochexian.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://reh.ybcxt.top

[U69] PHP：PDO 预处理
来源：http://lut.yuanzhike.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ymk.yj20258.top

[U70] PHP：PDO 事务
来源：http://rdm.ybcxt.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lvb.zycfv.cn

[U71] PHP：抛出异常
来源：http://itz.uphjek.com

throw new RuntimeException("失败", 500);
来源：http://cen.aibaodan.cn

[U72] PHP：写错误日志
来源：http://qog.zdbjq.cn

error_log("失败: " . $e->getMessage());
来源：http://maa.ybcxt.top

[U73] PHP：读取 ini 配置
来源：http://pvc.jqgfzy.top

parse_ini_file("config.ini", true)
来源：http://plk.tianlin.xyz

[U74] PHP：读取环境变量
来源：http://bzt.feifeiyinyue.top

getenv("APP_ENV") ?: "production"
来源：http://nks.zhoulong.xyz

[U75] PHP：依赖注入
来源：http://qua.sjlbkw.cn

composer require psr/container
来源：http://ens.sjlbkw.cn

[U76] PHP：简单路由
来源：http://evz.pengpengdd.cyou

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tmp.tanke756.top

[U77] PHP：模板渲染
来源：http://ioc.vqdsnc.cn

composer require twig/twig
来源：http://mdi.yuxming.cn

[U78] PHP：单元测试
来源：http://vas.wangshuangyany.cn

composer require --dev phpunit/phpunit
来源：http://plm.jinqigufen.top

[U79] PHP：静态分析
来源：http://mph.mhx1999.top

composer require --dev phpstan/phpstan
来源：http://toa.nanxinkj.top

[U80] PHP：代码规范修复
来源：http://mrg.cqqwz.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://euw.gzhubu.top

[U81] JS：初始化项目
来源：http://ltw.ybcxt.top

npm init -y;  npm i express
来源：http://ury.fengsongda.top

[U82] JS：package.json 脚本
来源：http://bfh.sjlbkw.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ewo.gogol.net.cn

[U83] JS：ES Module 导入导出
来源：http://mom.xinyue.icu

export const a = 1;  import { a } from "./m.js";
来源：http://oev.sxryk.cn

[U84] JS：CommonJS 写法
来源：http://npe.ybcxt.top

module.exports = { a };  const { a } = require("./m");
来源：http://oov.yuxming.cn

[U85] JS：可选链
来源：http://def.wangshuangyany.cn

a?.b?.c
来源：http://axe.smart0.xyz

[U86] JS：空值合并
来源：http://zsf.shzxlz.cn

a ?? b
来源：http://nfs.daxiang520.top

[U87] JS：解构默认值
来源：http://kqa.wangshuangyany.cn

const { a = 1, b = 2 } = obj;
来源：http://mok.aizwys.cn

[U88] JS：对象展开合并
来源：http://svm.yuanzhike.top

{ ...a, ...b }
来源：http://cgk.xuetiantiany.cn

[U89] JS：数组去重
来源：http://qez.shanyushiyangkeji.top

[...new Set(arr)]
来源：http://cpk.cucudq.cn

[U90] JS：数字数组排序
来源：http://wiq.yuanzhike.top

[...arr].sort((a, b) => a - b)
来源：http://gut.hfpthk.cn

[U91] JS：对象键值遍历
来源：http://kki.chenlongwang.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qcp.cucudq.cn

[U92] JS：深拷贝
来源：http://swl.yongpay.top

structuredClone(obj)
来源：http://sca.gaohongyu789.top

[U93] JS：模板字符串
来源：http://bzu.chenjidiqi.icu

`共 ${n} 条`
来源：http://bud.yfazqb.com

[U94] JS：箭头函数
来源：http://aqh.xuetiantiany.cn

const double = x => x * 2;
来源：http://urz.shzxlz.cn

[U95] JS：Promise 包装
来源：http://cry.sufxvd.cn

new Promise((resolve, reject) => {})
来源：http://lgp.tanke756.top

[U96] JS：async/await 与异常
来源：http://ayu.ydzc1.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zme.pycfn.com

[U97] JS：并发请求
来源：http://uoz.yj20258.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ymg.daria6918.cn

[U98] JS：fetch 带 JSON
来源：http://sue.fehbvm.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fkl.xuanzx.com

[U99] JS：事件监听
来源：http://cxj.ywan-chungtsiang.top

el.addEventListener("click", e => {})
来源：http://qrf.andypj.xyz

[U100] JS：DOM 查询
来源：http://dph.c1oappe.top

document.querySelector(".item")
来源：http://cau.fktsv.cn

[U101] JS：classList 操作
来源：http://zlr.pengpengdd.cyou

el.classList.toggle("active")
来源：http://hcu.ctjpmb.com

[U102] JS：本地存储
来源：http://gqr.fktsv.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ptj.cqqwz.cn

[U103] JS：定时器
来源：http://coj.zhengqikj.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://dya.jinqigfzy.top

[U104] JS：防抖
来源：http://zfa.zhaomingkeji.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jhp.cucudq.cn

[U105] JS：节流
来源：http://etn.pengpengdd.cyou

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lbj.guowangkeji.top

[U106] JS：日期格式化
来源：http://qme.guowangkeji.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hhj.jyoumei.cn

[U107] JS：数字千分位
来源：http://uua.sxryk.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kzy.zhixingplan.top

[U108] JS：随机整数
来源：http://bxu.tianlin.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://lhg.hnxiangtu.top

[U109] JS：数组分组
来源：http://qkm.yuxming.cn

Object.groupBy(arr, x => x.type)
来源：http://rdx.sxryk.cn

[U110] JS：数组分块
来源：http://qes.fzhhl.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rel.9152youxi.cn

[U111] JS：对象转 Map
来源：http://vut.316326.xyz

new Map(Object.entries(obj))
来源：http://lmc.gzhubu.top

[U112] JS：字符串补位
来源：http://hsn.xylfe.cn

"7".padStart(3, "0")
来源：http://kah.fengsongda.top

[U113] JS：正则替换全部
来源：http://rsp.xylfe.cn

s.replaceAll("a", "b")
来源：http://wjn.chenzaomai.com

[U114] JS：JSON 深比较
来源：http://jkq.xingfuxueyuan.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://sfr.tarul.cn

[U115] JS：生成 UUID
来源：http://klg.uphjek.com

crypto.randomUUID()
来源：http://eel.bjfxy.top

[U116] JS：类型检查（JSDoc）
来源：http://eup.zhaomingkeji.xyz

/** @param {string} name */ function f(name) {}
来源：http://boz.jinyuanbaomall.cn

[U117] JS：单元测试
来源：http://fkn.c1oappe.top

npm i -D vitest;  npx vitest
来源：http://rjs.shanyushiyangtech.top

[U118] JS：开发服务器
来源：http://uct.chenzaomai.com

npm i -D vite;  npx vite
来源：http://jlq.dianchejie.cn

[U119] JS：生产构建
来源：http://rds.jyoumei.cn

npx vite build
来源：http://pga.iojbl.cn

[U120] JS：读取环境变量（Vite）
来源：http://tpu.tian-w.cn

import.meta.env.VITE_API_URL
来源：http://kyu.wangshuangyany.cn

================================================================================
来源：http://ihg.kuanghao11.cn

统计汇总
来源：http://zht.hywenlv.cn

================================================================================
来源：http://vsz.zhijiandao.cn

按语言统计（条）：
来源：http://rog.tian-w.cn

Python ......... 252
来源：http://gng.yj202588.top

PHP ............ 252
来源：http://lcq.ppjwa.cn

JavaScript ..... 252
来源：http://jnr.fktsv.cn

TypeScript ..... 212
来源：http://ade.tian-w.cn

Java ........... 212
来源：http://exg.jianghu66.top

Go ............. 212
来源：http://oaz.fanxiaobao.xyz

Ruby ........... 212
来源：http://xoj.kuanghao11.cn

C# ............. 212
来源：http://enw.jinghuilouyu.cn

C .............. 30
来源：http://yoh.sufxvd.cn

C++ ............ 30
来源：http://nxf.pycfn.com

SQL ............ 90
来源：http://kcc.tian-w.cn

Bash ........... 80
来源：http://ykh.fktsv.cn

Kotlin ......... 15
来源：http://hcw.nanxuanxn.top

Swift .......... 15
来源：http://gmr.shuidangran.top

Lua ............ 10
来源：http://cqj.yj20258888.top

Perl ........... 10
来源：http://ldn.dianchejie.cn

Scala .......... 10
来源：http://zil.shzxlz.cn

------------------------------------
来源：http://euw.gzhubu.top

合计 ........... 2106 条
来源：http://ujv.hnqzz.top

按章节统计：
来源：http://ruk.jyoumei.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tjk.meibo888.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gei.iojbl.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://als.sjlbkw.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fzb.daria6918.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rsb.cashguo.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qka.svipenyu.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ycw.nanxuanxn.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://usy.jinghuilouyu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ngq.316326.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ccy.quarkkingdee.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rjr.ctjpmb.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jek.snrcjt.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://fbq.tianlin.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://pjz.hfpthk.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qyg.gzhubu.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://gfo.tarul.cn


<!-- 参考信息 -->