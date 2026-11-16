代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://rez.jqgfzy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dcq.wangdashe.top

[B15] 布尔运算与取反
来源：http://pzc.nanxuanxn.top

Py:   a and b or not c
来源：http://ont.hysaishi.cn

PHP:  $a && $b || !$c
来源：http://wgk.dianchejie.cn

JS:   a && b || !c
来源：http://naw.hnxiangtu.top

TS:   a && b || !c
来源：http://knd.daxiang520.top

Java: a && b || !c
来源：http://ksl.fanxiaobao.xyz

Go:   a && b || !c
来源：http://cbv.yuxming.cn

Ruby: a && b || !c
来源：http://ltn.jinqigfzy.top

C#:   a && b || !c
来源：http://ton.bbcook.cn

[B16] 卫语句：不满足条件提前返回
来源：http://cch.nanxuanxn.top

Py:   if not data: return
来源：http://quq.guannengcc.top

PHP:  if (!$data) { return; }
来源：http://rqv.shzxlz.cn

JS:   if (!data) return;
来源：http://obh.hnqzz.top

TS:   if (!data) return;
来源：http://qbv.svipenyu.cn

Java: if (data == null) return;
来源：http://fsc.jianghu66.top

Go:   if data == nil { return }
来源：http://ikg.zdbjq.cn

Ruby: return if data.nil?
来源：http://yke.shzxlz.cn

C#:   if (data == null) return;
来源：http://esg.9152youxi.cn

================================================================================
来源：http://xtp.havefunace.top

C. 函数与作用域
来源：http://tbh.sjlbkw.cn

================================================================================
来源：http://cie.gaohongyu789.top

[C01] 定义函数
来源：http://caz.ivvv.top

Py:   def add(a, b): return a + b
来源：http://rzt.yj20258.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nbh.9152youxi.cn

JS:   function add(a, b) { return a + b; }
来源：http://rwj.guowangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wrd.bjfxy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://gux.zhongyouzk.top

Go:   func add(a, b int) int { return a + b }
来源：http://bgj.aizwys.cn

Ruby: def add(a, b); a + b; end
来源：http://fnw.zhoulong.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jmq.cashguo.top

[C02] 默认参数
来源：http://sex.0kj1m.cn

Py:   def greet(name="World"): return name
来源：http://jzo.shanyushiyangtech.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ifr.wangshuangyany.cn

JS:   function greet(name = "World") { return name; }
来源：http://vol.iojbl.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://pwp.9152youxi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://fwg.sysykeji.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wdn.jlsjyb.cn

Ruby: def greet(name = "World") = name
来源：http://ihc.52xcode.cn

C#:   string Greet(string name = "World") => name;
来源：http://cck.vqdsnc.cn

[C03] 可变参数
来源：http://xem.yangfankeji.com

Py:   def total(*args): return sum(args)
来源：http://oez.aibaodan.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cjw.jiagoushi.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://iku.chenlongwang.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yjc.shangyingyoupin.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lkz.aizwys.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yln.wangshuangyany.cn

Ruby: def total(*nums); nums.sum; end
来源：http://jko.ywan-chungtsiang.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ivs.zhongyouzk.top

[C04] 命名参数 / 关键字参数
来源：http://kdj.daria6918.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gni.hammf.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dsu.bbcook.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xse.vehdjk.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vql.kuanghao11.cn

Java: // 无：用 Builder 模式或 record
来源：http://zjc.guannengcc.top

Go:   // 无：用配置结构体参数
来源：http://qkb.snrcjt.cn

Ruby: f(a: 1, b: 2)
来源：http://zae.hnxiangtu.top

C#:   f(a: 1, b: 2)
来源：http://qrn.fzhhl.top

[C05] 返回多个值
来源：http://ywc.jlsjyb.cn

Py:   return a, b
来源：http://xrt.shanyushiyangtech.top

PHP:  return [$a, $b];
来源：http://tup.tian-w.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://biu.zhijiandao.cn

TS:   return { a, b };
来源：http://tnp.epnwcf.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rwo.jinqigfzy.top

Go:   return a, b
来源：http://jjq.daxiang520.top

Ruby: return a, b
来源：http://qgc.xylfe.cn

C#:   return (a, b);              // ValueTuple
来源：http://ohg.zycfv.cn

[C06] 匿名函数 / lambda
来源：http://spq.jinqigufen.top

Py:   square = lambda x: x * x
来源：http://yrq.tanke756.top

PHP:  $square = fn($x) => $x * $x;
来源：http://dex.shanyushiyangtech.top

JS:   const square = x => x * x;
来源：http://aum.nanxuanxn.top

TS:   const square = (x: number): number => x * x;
来源：http://jep.bbcook.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://iqb.hesvh.cn

Go:   sq := func(x int) int { return x * x }
来源：http://bat.kuanghao11.cn

Ruby: square = ->(x) { x * x }
来源：http://nnd.hammf.cn

C#:   Func<int, int> square = x => x * x;
来源：http://oxc.kuanghao11.cn

[C07] 把函数作为参数传入
来源：http://nuc.havefunace.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qxi.jianghu66.top

PHP:  array_map("strtoupper", $arr);
来源：http://iba.xylfe.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pec.quarkkingdee.top

TS:   arr.map(String)
来源：http://vow.sweek.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ota.bbcook.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wtk.jqgufenzy.top

Ruby: arr.map(&:upcase)
来源：http://row.jlsjyb.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://lsz.52xcode.cn

[C08] 闭包
来源：http://crr.ehwqpu.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ouo.zhijiandao.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cxo.hywenlv.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fzz.yuxming.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pyl.guowangkeji.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ois.zhiwuduotai.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xyt.fehbvm.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cbb.jinqigufen.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tlu.shangyingyoupin.top

[C09] 递归
来源：http://yml.0kj1m.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lnu.fehbvm.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rou.sweek.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cfx.andypj.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kni.tanke756.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mha.aizwys.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zvb.havefunace.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nzs.vehdjk.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rvt.feifeiyinyue.top

[C10] 变量作用域
来源：http://sun.kuanghao11.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fig.nanxinkj.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://klk.iojbl.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mxg.jinyuanbaomall.cn

TS:   同 JS
来源：http://wtw.yangfankeji.com

Java: 方法内为块级作用域
来源：http://lsn.cheryme.top

Go:   花括号块级作用域
来源：http://ecx.jyoumei.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://odl.fanxiaobao.xyz

C#:   块级作用域
来源：http://iaw.chenjidiqi.icu

[C11] 模块导入与导出
来源：http://sxa.hywenlv.cn

Py:   from module import func
来源：http://njt.yuxming.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://lgv.cucudq.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ssa.chenlongwang.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jkw.zdbjq.cn

Java: import java.util.List;
来源：http://jgg.smart0.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ftc.xinyue.icu

Ruby: require "json"; require_relative "./util"
来源：http://ois.guannengcc.top

C#:   using System.Text;
来源：http://odk.hesvh.cn

[C12] 立即执行函数 IIFE
来源：http://zoz.ydzc1.top

Py:   (lambda: print("run"))()
来源：http://ylw.tarul.cn

PHP:  (function () { echo "run"; })();
来源：http://rcd.fengsongda.top

JS:   (() => { console.log("run"); })();
来源：http://qaw.hysaishi.cn

TS:   (() => { console.log("run"); })();
来源：http://qma.shangyingyoupin.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xsb.shanyushiyangtech.top

Go:   func() { fmt.Println("run") }()
来源：http://pjk.sufxvd.cn

Ruby: -> { puts "run" }.call
来源：http://vhk.sysykeji.top

C#:   // 无 IIFE：用静态构造函数
来源：http://zig.jinyuanbaomall.cn

[C13] 类型声明 / 类型注解
来源：http://ggl.yongpay.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cjd.zhixingplan.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wnw.nanxinkj.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pnc.hcnkem.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wtd.chenjidiqi.icu

Java: int add(int a, int b) { return a + b; }
来源：http://goi.pycfn.com

Go:   func add(a, b int) int
来源：http://ojs.xylfe.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cdi.yfazqb.com

C#:   int Add(int a, int b) => a + b;
来源：http://xca.zhoulong.xyz

[C14] 泛型函数
来源：http://prr.guannengcc.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ixs.chenjidiqi.icu

PHP:  // 无泛型
来源：http://dvv.jinqigufen.top

JS:   // 无泛型
来源：http://prx.yonumen.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hzj.jinqigfzy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xen.fengsongda.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://evk.ydjk.org.cn

Ruby: # 无泛型
来源：http://cpt.guowangkeji.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://uaz.haohaochexian.top

[C15] 解构 / 展开参数
来源：http://yrq.cqqwz.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://azu.nanxinkj.top

PHP:  [$a, $b] = $pair;
来源：http://con.guannengcc.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jqz.yangfankeji.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ddd.cashguo.top

Java: // 无解构
来源：http://hep.yuxming.cn

Go:   // 无解构
来源：http://xza.guowangkeji.top

Ruby: a, b = pair
来源：http://wgs.zhiwuduotai.top

C#:   var (a, b) = pair;
来源：http://len.ppjwa.cn

[C16] 函数 / 方法重载
来源：http://oud.ctjpmb.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ybs.hywenlv.cn

PHP:  // 无重载
来源：http://bmn.hongshengwenyu.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://nhv.fengsongda.top

TS:   // 用联合类型或重载签名声明
来源：http://lph.xinyue.icu

Java: void f(int a) {}  void f(String a) {}
来源：http://eok.chenzaomai.com

Go:   // 无重载：用不同函数名
来源：http://lkt.uphjek.com

Ruby: # 无重载：靠动态参数
来源：http://mde.nanxuanxn.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://rtq.shanyushiyangtech.top

================================================================================
来源：http://noj.nanxinkj.top

D. 数组 / 列表 / 集合
来源：http://yyt.ywan-chungtsiang.top

================================================================================
来源：http://bbd.zhengqikj.top

[D01] 创建数组 / 列表
来源：http://kaw.yongpay.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://lmo.ywan-chungtsiang.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qiw.jqgufenzy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bmv.smart0.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://klv.aizwys.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tgk.0kj1m.cn

Go:   arr := []int{1, 2, 3}
来源：http://zqv.zhixingplan.top

Ruby: arr = [1, 2, 3]
来源：http://jpe.yueranfly.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bux.zhiwuduotai.top

[D02] 追加元素到末尾
来源：http://tni.hesvh.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rzk.xinyue.icu

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://imd.cucudq.cn

JS:   arr.push(4);
来源：http://cnf.shuidangran.top

TS:   arr.push(4);
来源：http://hnu.vehdjk.com

Java: list.add(4);
来源：http://buy.ywan-chungtsiang.top

Go:   arr = append(arr, 4)
来源：http://pwf.bbcook.cn

Ruby: arr << 4; arr.push(5)
来源：http://ryf.shzxlz.cn

C#:   list.Add(4);
来源：http://tnz.wangshuangyany.cn

[D03] 在指定位置插入元素
来源：http://dku.havefunace.top

Py:   arr.insert(0, 0)
来源：http://xiv.shangyingyoupin.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gxh.yangfankeji.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rms.fzhhl.top

TS:   arr.splice(0, 0, 0);
来源：http://ewx.sufxvd.cn

Java: list.add(0, 0);
来源：http://hgy.yonumen.top

Go:   arr = append([]int{0}, arr...)
来源：http://qls.snrcjt.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qun.yuanzhike.top

C#:   list.Insert(0, 0);
来源：http://grf.nanxuanxn.top

[D04] 删除元素
来源：http://dlb.fanxiaobao.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nwd.dashuyun.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://prp.jinyuanbaomall.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lia.uphjek.com

TS:   arr.splice(0, 1);
来源：http://ypo.hywenlv.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dhx.zhixingplan.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yen.vehdjk.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ckc.yongpay.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dyr.wangdashe.top

[D05] 访问与修改元素
来源：http://yri.zycfv.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jpe.hnxiangtu.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wuw.ydjk.org.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kph.pengpengdd.cyou

TS:   arr[0]; arr.at(-1);
来源：http://oyw.ywan-chungtsiang.top

Java: list.get(0); list.set(0, 9);
来源：http://fio.birdmap.top

Go:   arr[0]; arr[0] = 9
来源：http://ahj.chenlongwang.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mui.jqgfzy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ehj.wangdashe.top

[D06] 数组长度
来源：http://wrn.yj202588.top

Py:   len(arr)
来源：http://qyt.ybcxt.top

PHP:  count($arr);
来源：http://rdc.nanxinkj.top

JS:   arr.length
来源：http://can.zdqjudy.top

TS:   arr.length
来源：http://acz.zhongyouzk.top

Java: list.size();
来源：http://jqq.yonumen.top

Go:   len(arr)
来源：http://auu.sufxvd.cn

Ruby: arr.length; arr.size
来源：http://jug.pengpengdd.cyou

C#:   list.Count;
来源：http://aym.hesvh.cn

[D07] 切片 / 取子数组
来源：http://uat.shangyingyoupin.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ksj.tanke756.top

PHP:  array_slice($arr, 1, 3);
来源：http://byk.yfazqb.com

JS:   arr.slice(1, 4);
来源：http://lfn.tianlin.xyz

TS:   arr.slice(1, 4);
来源：http://odf.sweek.top

Java: list.subList(1, 4);
来源：http://kkb.zycfv.cn

Go:   arr[1:4]
来源：http://xqn.jyoumei.cn

Ruby: arr[1, 3]
来源：http://wna.mhx1999.top

C#:   list.GetRange(1, 3);
来源：http://nvt.yuanzhike.top

[D08] 合并两个数组
来源：http://hjc.vqdsnc.cn

Py:   a + b;  a.extend(b)
来源：http://qkt.zycfv.cn

PHP:  array_merge($a, $b);
来源：http://mjy.jianghu66.top

JS:   [...a, ...b];  a.concat(b);
来源：http://yjy.feifeiyinyue.top

TS:   [...a, ...b];
来源：http://azb.jianghu66.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ctl.xuanzx.com

Go:   append(a, b...)
来源：http://dxp.zdbjq.cn

Ruby: a + b;  a.concat(b)
来源：http://ytc.nanxinkj.top

C#:   a.Concat(b).ToList()
来源：http://fca.ppjwa.cn

[D09] 排序（升序）
来源：http://xbl.aibaodan.cn

Py:   sorted(arr);  arr.sort()
来源：http://gsg.pengpengdd.cyou

PHP:  sort($arr);
来源：http://nvk.feifeiyinyue.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ars.pengpengdd.cyou

TS:   [...arr].sort((x, y) => x - y);
来源：http://ivl.xinyue.icu

Java: Collections.sort(list);  list.sort(null);
来源：http://pns.ppjwa.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://emg.jinyuanbaomall.cn

Ruby: arr.sort
来源：http://hcu.yonumen.top

C#:   list.Sort();
来源：http://nir.ydjk.org.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mxv.jqgfzy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bsh.jinqigfzy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hsj.sxryk.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vdr.hcnkem.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ifu.yongpay.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xob.ehwqpu.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wcx.yuanzhike.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cdv.ybcxt.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://uwn.aizwys.cn

[D11] 反转数组
来源：http://wbc.pengpengdd.cyou

Py:   arr[::-1];  arr.reverse()
来源：http://unx.snrcjt.cn

PHP:  array_reverse($arr);
来源：http://kau.yueranfly.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bmj.tanke756.top

TS:   [...arr].reverse();
来源：http://fsg.gzhubu.top

Java: Collections.reverse(list);
来源：http://ntq.tianlin.xyz

Go:   slices.Reverse(arr)
来源：http://hfs.52xcode.cn

Ruby: arr.reverse
来源：http://dsf.sjlbkw.cn

C#:   list.Reverse();
来源：http://szw.tianlin.xyz

[D12] 查找元素下标
来源：http://bwb.316326.xyz

Py:   arr.index(x);  x in arr
来源：http://ntn.kuanghao11.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ncj.yonumen.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hwn.xinyue.icu

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://izg.jyoumei.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kvd.bbcook.cn

Go:   slices.Index(arr, x)
来源：http://nrk.hcnkem.com

Ruby: arr.index(x)
来源：http://efs.fehbvm.com

C#:   list.IndexOf(x);
来源：http://zro.cdnleiting.top

[D13] 过滤（保留满足条件的）
来源：http://xkm.chenjidiqi.icu

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://squ.316326.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rvb.pycfn.com

JS:   arr.filter(x => x > 3)
来源：http://qpz.meibo888.top

TS:   arr.filter(x => x > 3)
来源：http://xxz.xuanzx.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ljw.fktsv.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xiy.smart0.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://ubn.zdqjudy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://xfc.ppjwa.cn

[D14] 映射转换（每个元素变形）
来源：http://ppd.gzhubu.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hvc.xuanzx.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fxd.tianlin.xyz

JS:   arr.map(x => x * 2)
来源：http://aug.yuanzhike.top

TS:   arr.map(x => x * 2)
来源：http://mmz.9152youxi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ici.cqqwz.cn

Go:   // 手写循环
来源：http://vac.mhx1999.top

Ruby: arr.map { |x| x * 2 }
来源：http://yxh.redwolf501.top

C#:   list.Select(x => x * 2).ToList()
来源：http://bud.cheryme.top

[D15] 去重
来源：http://fme.yuxming.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jof.yuxming.cn

PHP:  array_unique($arr);
来源：http://upp.jlsjyb.cn

JS:   [...new Set(arr)]
来源：http://xtg.shanyushiyangkeji.top


<!-- 参考信息 -->