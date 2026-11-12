代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://hum.guowangkeji.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://apb.wangshuangyany.cn

[B15] 布尔运算与取反
来源：http://unl.tianlin.xyz

Py:   a and b or not c
来源：http://ctj.yj202588.top

PHP:  $a && $b || !$c
来源：http://gxj.shanyushiyangkeji.top

JS:   a && b || !c
来源：http://upz.yongpay.top

TS:   a && b || !c
来源：http://opn.guannengcc.top

Java: a && b || !c
来源：http://vfn.birdmap.top

Go:   a && b || !c
来源：http://vcq.ydjk.org.cn

Ruby: a && b || !c
来源：http://caj.daxiang520.top

C#:   a && b || !c
来源：http://yyh.jinqigufen.top

[B16] 卫语句：不满足条件提前返回
来源：http://rqb.xinyue.icu

Py:   if not data: return
来源：http://xjn.andypj.xyz

PHP:  if (!$data) { return; }
来源：http://svf.yueranfly.top

JS:   if (!data) return;
来源：http://iun.xylfe.cn

TS:   if (!data) return;
来源：http://wnn.chenzaomai.com

Java: if (data == null) return;
来源：http://xok.sufxvd.cn

Go:   if data == nil { return }
来源：http://ijg.yuanzhike.top

Ruby: return if data.nil?
来源：http://cpq.zhixingplan.top

C#:   if (data == null) return;
来源：http://rsz.9152youxi.cn

================================================================================
来源：http://aff.0kj1m.cn

C. 函数与作用域
来源：http://fcx.nanxuanxn.top

================================================================================
来源：http://asf.jqgfzy.top

[C01] 定义函数
来源：http://hzk.hnqzz.top

Py:   def add(a, b): return a + b
来源：http://zjz.zdqjudy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hzz.cqqwz.cn

JS:   function add(a, b) { return a + b; }
来源：http://prl.sjlbkw.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://izg.zhixingplan.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ibu.yanxiufei.cn

Go:   func add(a, b int) int { return a + b }
来源：http://lvq.hfpthk.cn

Ruby: def add(a, b); a + b; end
来源：http://erp.svipenyu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://avs.havefunace.top

[C02] 默认参数
来源：http://bff.xuetiantiany.cn

Py:   def greet(name="World"): return name
来源：http://rxm.wangdashe.top

PHP:  function greet($name = "World") { return $name; }
来源：http://mex.fengsongda.top

JS:   function greet(name = "World") { return name; }
来源：http://igs.zdqjudy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ujp.yj20258.top

Java: // 无默认参数：方法重载或 Optional
来源：http://xda.yj20258888.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ozj.zhaomingkeji.xyz

Ruby: def greet(name = "World") = name
来源：http://jvb.hongshengwenyu.top

C#:   string Greet(string name = "World") => name;
来源：http://gkq.xuanzx.com

[C03] 可变参数
来源：http://ami.shzxlz.cn

Py:   def total(*args): return sum(args)
来源：http://kzx.jqgfzy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://oun.shangyingyoupin.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kcm.shuidangran.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://sch.chenjidiqi.icu

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xak.ehwqpu.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://oti.epnwcf.com

Ruby: def total(*nums); nums.sum; end
来源：http://yaz.xuetiantiany.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://aty.hcnkem.com

[C04] 命名参数 / 关键字参数
来源：http://uvb.sweek.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fqs.c1oappe.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ghd.sjlbkw.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://taa.hfpthk.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ryo.jqgufenzy.top

Java: // 无：用 Builder 模式或 record
来源：http://iac.ehwqpu.com

Go:   // 无：用配置结构体参数
来源：http://lic.fktsv.cn

Ruby: f(a: 1, b: 2)
来源：http://nat.jlsjyb.cn

C#:   f(a: 1, b: 2)
来源：http://bti.fehbvm.com

[C05] 返回多个值
来源：http://adf.shanyushiyangkeji.top

Py:   return a, b
来源：http://vtz.cashguo.top

PHP:  return [$a, $b];
来源：http://ngd.yanxiufei.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://izg.xylfe.cn

TS:   return { a, b };
来源：http://owu.gaohongyu789.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fbb.feifeiyinyue.top

Go:   return a, b
来源：http://rwd.shangyingyoupin.top

Ruby: return a, b
来源：http://lie.jqgufenzy.top

C#:   return (a, b);              // ValueTuple
来源：http://icn.pycfn.com

[C06] 匿名函数 / lambda
来源：http://tsp.yuxming.cn

Py:   square = lambda x: x * x
来源：http://gqz.hysaishi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://rdo.jinyuanbaomall.cn

JS:   const square = x => x * x;
来源：http://pgt.vehdjk.com

TS:   const square = (x: number): number => x * x;
来源：http://jql.yongpay.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://prv.xylfe.cn

Go:   sq := func(x int) int { return x * x }
来源：http://yrd.mhx1999.top

Ruby: square = ->(x) { x * x }
来源：http://opm.hammf.cn

C#:   Func<int, int> square = x => x * x;
来源：http://izd.chenlongwang.top

[C07] 把函数作为参数传入
来源：http://yii.wangdashe.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mox.cdnleiting.top

PHP:  array_map("strtoupper", $arr);
来源：http://ajn.0kj1m.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://afo.jinyuanbaomall.cn

TS:   arr.map(String)
来源：http://uvy.bjfxy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://emn.ydjk.org.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://etm.sweek.top

Ruby: arr.map(&:upcase)
来源：http://scy.yongpay.top

C#:   arr.Select(s => s.ToUpper())
来源：http://rhx.jiagoushi.top

[C08] 闭包
来源：http://wpa.shuidangran.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xoz.ydzc1.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ucx.316326.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://oxw.feifeiyinyue.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ran.xingfuxueyuan.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ouq.zhoulong.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://sou.chenjidiqi.icu

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rym.bjfxy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nkw.wangdashe.top

[C09] 递归
来源：http://hmo.gzhubu.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://afq.yj202588.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bxz.pengpengdd.cyou

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gwl.yueranfly.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xys.yanxiufei.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://axg.yonumen.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fdl.nanxinkj.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gum.vehdjk.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ikl.xylfe.cn

[C10] 变量作用域
来源：http://ydu.meibo888.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ovb.yuanzhike.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zuw.shanyushiyangkeji.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rsl.tian-w.cn

TS:   同 JS
来源：http://krk.zdqjudy.top

Java: 方法内为块级作用域
来源：http://kyh.shuidangran.top

Go:   花括号块级作用域
来源：http://jkw.iojbl.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ohh.0kj1m.cn

C#:   块级作用域
来源：http://aos.shanyushiyangkeji.top

[C11] 模块导入与导出
来源：http://roq.yonumen.top

Py:   from module import func
来源：http://lha.nanxinkj.top

PHP:  require "file.php";  或 use App\Service;
来源：http://hrg.daria6918.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://fst.xylfe.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xdf.tarul.cn

Java: import java.util.List;
来源：http://pkd.jinyuanbaomall.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xro.cdnleiting.top

Ruby: require "json"; require_relative "./util"
来源：http://vtd.hfpthk.cn

C#:   using System.Text;
来源：http://cit.ywan-chungtsiang.top

[C12] 立即执行函数 IIFE
来源：http://abw.9152youxi.cn

Py:   (lambda: print("run"))()
来源：http://cvp.hesvh.cn

PHP:  (function () { echo "run"; })();
来源：http://tpa.bbcook.cn

JS:   (() => { console.log("run"); })();
来源：http://nkt.shangyingyoupin.top

TS:   (() => { console.log("run"); })();
来源：http://plw.hysaishi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://yzd.shzxlz.cn

Go:   func() { fmt.Println("run") }()
来源：http://sje.shangyingyoupin.top

Ruby: -> { puts "run" }.call
来源：http://fge.uphjek.com

C#:   // 无 IIFE：用静态构造函数
来源：http://bme.316326.xyz

[C13] 类型声明 / 类型注解
来源：http://dyh.andypj.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nyg.xuetiantiany.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pys.fengsongda.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qpv.xingfuxueyuan.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://eeb.sysykeji.top

Java: int add(int a, int b) { return a + b; }
来源：http://mez.chenjidiqi.icu

Go:   func add(a, b int) int
来源：http://tmx.redwolf501.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ktd.nwbrower.top

C#:   int Add(int a, int b) => a + b;
来源：http://abu.hcnkem.com

[C14] 泛型函数
来源：http://nqe.smart0.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://yoo.havefunace.top

PHP:  // 无泛型
来源：http://taw.yanxiufei.cn

JS:   // 无泛型
来源：http://bds.daria6918.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zme.cqqwz.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rto.hcnkem.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rbn.svipenyu.cn

Ruby: # 无泛型
来源：http://ups.cheryme.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://psj.redwolf501.top

[C15] 解构 / 展开参数
来源：http://daq.hcnkem.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://loe.jyoumei.cn

PHP:  [$a, $b] = $pair;
来源：http://fqk.hcnkem.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pkj.gzhubu.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lmf.shuidangran.top

Java: // 无解构
来源：http://not.bjfxy.top

Go:   // 无解构
来源：http://hdi.snrcjt.cn

Ruby: a, b = pair
来源：http://uep.shuidangran.top

C#:   var (a, b) = pair;
来源：http://gex.pengpengdd.cyou

[C16] 函数 / 方法重载
来源：http://mzn.jianghu66.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zqo.jinghuilouyu.cn

PHP:  // 无重载
来源：http://trv.gotoacloud.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://gxq.hysaishi.cn

TS:   // 用联合类型或重载签名声明
来源：http://hkg.jlsjyb.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://uoe.c1oappe.top

Go:   // 无重载：用不同函数名
来源：http://svx.fktsv.cn

Ruby: # 无重载：靠动态参数
来源：http://sad.shuidangran.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://hzy.pycfn.com

================================================================================
来源：http://hck.zhengqikj.top

D. 数组 / 列表 / 集合
来源：http://soh.sufxvd.cn

================================================================================
来源：http://ihc.ppjwa.cn

[D01] 创建数组 / 列表
来源：http://khe.pengpengdd.cyou

Py:   arr = [1, 2, 3];  empty = []
来源：http://lln.hywenlv.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pyu.hysaishi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cbw.kuanghao11.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://sct.vehdjk.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gwj.wangshuangyany.cn

Go:   arr := []int{1, 2, 3}
来源：http://gwl.hywenlv.cn

Ruby: arr = [1, 2, 3]
来源：http://wgd.jqgufenzy.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xqa.sxryk.cn

[D02] 追加元素到末尾
来源：http://xbd.vehdjk.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://orv.zhiwuduotai.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qvs.sysykeji.top

JS:   arr.push(4);
来源：http://ocp.hysaishi.cn

TS:   arr.push(4);
来源：http://wvr.hcnkem.com

Java: list.add(4);
来源：http://lvj.haohaochexian.top

Go:   arr = append(arr, 4)
来源：http://zok.nwbrower.top

Ruby: arr << 4; arr.push(5)
来源：http://oer.9152youxi.cn

C#:   list.Add(4);
来源：http://veg.andypj.xyz

[D03] 在指定位置插入元素
来源：http://oey.yfazqb.com

Py:   arr.insert(0, 0)
来源：http://pbd.zhongyouzk.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rde.yj202588.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gzb.haohaochexian.top

TS:   arr.splice(0, 0, 0);
来源：http://rxl.tian-w.cn

Java: list.add(0, 0);
来源：http://rhw.uphjek.com

Go:   arr = append([]int{0}, arr...)
来源：http://pqj.jqgfzy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wlk.uphjek.com

C#:   list.Insert(0, 0);
来源：http://dgt.aizwys.cn

[D04] 删除元素
来源：http://spw.hnxiangtu.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://yoz.chenlongwang.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qop.guowangkeji.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tsn.nanxuanxn.top

TS:   arr.splice(0, 1);
来源：http://qgl.nanxuanxn.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tyl.xinyue.icu

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ebh.yj20258.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ghx.smart0.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bac.meibo888.top

[D05] 访问与修改元素
来源：http://whj.zhaomingkeji.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://oyh.dashuyun.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yja.0kj1m.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://csm.jinghuilouyu.cn

TS:   arr[0]; arr.at(-1);
来源：http://jip.hnqzz.top

Java: list.get(0); list.set(0, 9);
来源：http://vlk.hfpthk.cn

Go:   arr[0]; arr[0] = 9
来源：http://tve.cheryme.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://izy.meibo888.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://aku.aizwys.cn

[D06] 数组长度
来源：http://zxq.ybcxt.top

Py:   len(arr)
来源：http://uwz.dashuyun.cn

PHP:  count($arr);
来源：http://iui.andypj.xyz

JS:   arr.length
来源：http://kyf.xinyue.icu

TS:   arr.length
来源：http://ena.yvedp.cn

Java: list.size();
来源：http://ypf.haohaochexian.top

Go:   len(arr)
来源：http://hkq.shzxlz.cn

Ruby: arr.length; arr.size
来源：http://bne.pycfn.com

C#:   list.Count;
来源：http://oyp.zycfv.cn

[D07] 切片 / 取子数组
来源：http://fqe.fktsv.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://goj.52xcode.cn

PHP:  array_slice($arr, 1, 3);
来源：http://emc.meibo888.top

JS:   arr.slice(1, 4);
来源：http://yoh.guannengcc.top

TS:   arr.slice(1, 4);
来源：http://ego.yvedp.cn

Java: list.subList(1, 4);
来源：http://wyy.fanxiaobao.xyz

Go:   arr[1:4]
来源：http://mwp.hongshengwenyu.top

Ruby: arr[1, 3]
来源：http://okq.iojbl.cn

C#:   list.GetRange(1, 3);
来源：http://dml.hysaishi.cn

[D08] 合并两个数组
来源：http://kni.andypj.xyz

Py:   a + b;  a.extend(b)
来源：http://esf.jiagoushi.top

PHP:  array_merge($a, $b);
来源：http://oic.hysaishi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://quf.jiagoushi.top

TS:   [...a, ...b];
来源：http://gyx.ppjwa.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gug.uphjek.com

Go:   append(a, b...)
来源：http://ktj.jqgfzy.top

Ruby: a + b;  a.concat(b)
来源：http://ivn.xingfuxueyuan.xyz

C#:   a.Concat(b).ToList()
来源：http://mes.wangshuangyany.cn

[D09] 排序（升序）
来源：http://hox.vehdjk.com

Py:   sorted(arr);  arr.sort()
来源：http://wkw.gzhubu.top

PHP:  sort($arr);
来源：http://eyn.redwolf501.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vry.zhixingplan.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://knw.dianchejie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ygk.jqgufenzy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ksf.yuanzhike.top

Ruby: arr.sort
来源：http://xqy.yvedp.cn

C#:   list.Sort();
来源：http://mqo.jinyuanbaomall.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://afs.316326.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ewp.yuanzhike.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://naq.jqgufenzy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://khh.zdbjq.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fav.epnwcf.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://osf.xylfe.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gvb.zhoulong.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tak.gaohongyu789.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fwb.fehbvm.com

[D11] 反转数组
来源：http://uol.fengsongda.top

Py:   arr[::-1];  arr.reverse()
来源：http://ruq.sweek.top

PHP:  array_reverse($arr);
来源：http://luq.fanxiaobao.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ees.hywenlv.cn

TS:   [...arr].reverse();
来源：http://fne.ivvv.top

Java: Collections.reverse(list);
来源：http://sjp.yvedp.cn

Go:   slices.Reverse(arr)
来源：http://jio.yj202588.top

Ruby: arr.reverse
来源：http://esn.fktsv.cn

C#:   list.Reverse();
来源：http://ojc.xuanzx.com

[D12] 查找元素下标
来源：http://tpt.redwolf501.top

Py:   arr.index(x);  x in arr
来源：http://gcv.gaohongyu789.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ezx.wangdashe.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ivf.ivvv.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bjj.pycfn.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jpr.jinqigufen.top

Go:   slices.Index(arr, x)
来源：http://wpq.zhengqikj.top

Ruby: arr.index(x)
来源：http://owm.zhongyouzk.top

C#:   list.IndexOf(x);
来源：http://lqt.meibo888.top

[D13] 过滤（保留满足条件的）
来源：http://rnx.xinyue.icu

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gts.shanyushiyangtech.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tnq.quarkkingdee.top

JS:   arr.filter(x => x > 3)
来源：http://vew.nanxinkj.top

TS:   arr.filter(x => x > 3)
来源：http://juf.ppjwa.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://eyy.jqgufenzy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yoz.guowangkeji.top

Ruby: arr.select { |x| x > 3 }
来源：http://agf.birdmap.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ldn.jiagoushi.top

[D14] 映射转换（每个元素变形）
来源：http://qbj.hnxiangtu.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://som.zhijiandao.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kix.chenjidiqi.icu

JS:   arr.map(x => x * 2)
来源：http://ifw.cucudq.cn

TS:   arr.map(x => x * 2)
来源：http://rwg.jqgfzy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://nfn.xziqi.cn

Go:   // 手写循环
来源：http://sod.fanxiaobao.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://rbo.hcnkem.com

C#:   list.Select(x => x * 2).ToList()
来源：http://cfd.yangfankeji.com

[D15] 去重
来源：http://gmm.yangfankeji.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cgb.zdbjq.cn

PHP:  array_unique($arr);
来源：http://nhj.zhongyouzk.top

JS:   [...new Set(arr)]
来源：http://evp.tarul.cn


<!-- 参考信息 -->