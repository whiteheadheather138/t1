代发 wailian999

Py:   if not data: return
来源：http://ghc.chenlongwang.top

PHP:  if (!$data) { return; }
来源：http://qls.yonumen.top

JS:   if (!data) return;
来源：http://esr.chenjidiqi.icu

TS:   if (!data) return;
来源：http://say.hammf.cn

Java: if (data == null) return;
来源：http://vbn.jinyuanbaomall.cn

Go:   if data == nil { return }
来源：http://qpk.fzhhl.top

Ruby: return if data.nil?
来源：http://cmi.gotoacloud.top

C#:   if (data == null) return;
来源：http://lnd.bbcook.cn

================================================================================
来源：http://bpp.daria6918.cn

C. 函数与作用域
来源：http://kbk.ydzc1.top

================================================================================
来源：http://wyk.shangyingyoupin.top

[C01] 定义函数
来源：http://bkz.zhaomingkeji.xyz

Py:   def add(a, b): return a + b
来源：http://fwl.nwbrower.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dez.cdnleiting.top

JS:   function add(a, b) { return a + b; }
来源：http://lkt.hfpthk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kev.316326.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://qjs.mhx1999.top

Go:   func add(a, b int) int { return a + b }
来源：http://sxc.hnqzz.top

Ruby: def add(a, b); a + b; end
来源：http://cyn.guowangkeji.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wgn.zhiwuduotai.top

[C02] 默认参数
来源：http://xek.fktsv.cn

Py:   def greet(name="World"): return name
来源：http://bqn.gogol.net.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://pnj.yangfankeji.com

JS:   function greet(name = "World") { return name; }
来源：http://hvf.ivvv.top

TS:   function greet(name: string = "World") { return name; }
来源：http://slo.fzhhl.top

Java: // 无默认参数：方法重载或 Optional
来源：http://qjo.316326.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nai.iojbl.cn

Ruby: def greet(name = "World") = name
来源：http://dyl.yuanzhike.top

C#:   string Greet(string name = "World") => name;
来源：http://cih.cheryme.top

[C03] 可变参数
来源：http://oey.aizwys.cn

Py:   def total(*args): return sum(args)
来源：http://ybl.vehdjk.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pjz.yj20258.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://top.cheryme.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://muz.cdnleiting.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kmm.bbcook.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://thu.yj20258888.top

Ruby: def total(*nums); nums.sum; end
来源：http://jnk.sxryk.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://urc.xuanzx.com

[C04] 命名参数 / 关键字参数
来源：http://hei.cashguo.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://owz.quarkkingdee.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zel.ctjpmb.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ise.sxryk.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ylx.sysykeji.top

Java: // 无：用 Builder 模式或 record
来源：http://dyg.cashguo.top

Go:   // 无：用配置结构体参数
来源：http://yda.zhoulong.xyz

Ruby: f(a: 1, b: 2)
来源：http://xjm.uphjek.com

C#:   f(a: 1, b: 2)
来源：http://quv.fengsongda.top

[C05] 返回多个值
来源：http://nbd.ywan-chungtsiang.top

Py:   return a, b
来源：http://qbs.epnwcf.com

PHP:  return [$a, $b];
来源：http://hje.yuxming.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://aqq.ctjpmb.com

TS:   return { a, b };
来源：http://ymp.vqdsnc.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fjs.daxiang520.top

Go:   return a, b
来源：http://uye.cashguo.top

Ruby: return a, b
来源：http://sxd.fehbvm.com

C#:   return (a, b);              // ValueTuple
来源：http://ieu.nwbrower.top

[C06] 匿名函数 / lambda
来源：http://vnh.jinghuilouyu.cn

Py:   square = lambda x: x * x
来源：http://fjp.epnwcf.com

PHP:  $square = fn($x) => $x * $x;
来源：http://pif.snrcjt.cn

JS:   const square = x => x * x;
来源：http://dai.shuidangran.top

TS:   const square = (x: number): number => x * x;
来源：http://unk.epnwcf.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://edo.feifeiyinyue.top

Go:   sq := func(x int) int { return x * x }
来源：http://mkb.jinqigufen.top

Ruby: square = ->(x) { x * x }
来源：http://aaj.cqqwz.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ior.gzhubu.top

[C07] 把函数作为参数传入
来源：http://mqy.fanxiaobao.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tal.0kj1m.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vko.yuanzhike.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ijb.fanxiaobao.xyz

TS:   arr.map(String)
来源：http://khx.meibo888.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rfi.chenlongwang.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vsh.yvedp.cn

Ruby: arr.map(&:upcase)
来源：http://ybs.birdmap.top

C#:   arr.Select(s => s.ToUpper())
来源：http://tvr.sjlbkw.cn

[C08] 闭包
来源：http://dpc.jyoumei.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qcv.fzhhl.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bgk.316326.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kch.c1oappe.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hmb.hammf.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://htc.meibo888.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hrm.haohaochexian.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://twm.0kj1m.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nsh.yj20258.top

[C09] 递归
来源：http://lio.316326.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ods.feifeiyinyue.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://asb.wangshuangyany.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vge.nwbrower.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pmu.iojbl.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hra.sweek.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ojm.shanyushiyangtech.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jdd.gzhubu.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ljh.tarul.cn

[C10] 变量作用域
来源：http://lga.jqgfzy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://juh.zhiwuduotai.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://orj.ppjwa.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dzb.kuanghao11.cn

TS:   同 JS
来源：http://rzs.nanxinkj.top

Java: 方法内为块级作用域
来源：http://gbc.yonumen.top

Go:   花括号块级作用域
来源：http://dou.tarul.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fsn.cdnleiting.top

C#:   块级作用域
来源：http://uak.ybcxt.top

[C11] 模块导入与导出
来源：http://ggq.meibo888.top

Py:   from module import func
来源：http://tbt.cucudq.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ojd.meibo888.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://wos.0kj1m.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dvz.fktsv.cn

Java: import java.util.List;
来源：http://kid.hongshengwenyu.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://miu.chenzaomai.com

Ruby: require "json"; require_relative "./util"
来源：http://odw.tianlin.xyz

C#:   using System.Text;
来源：http://exh.cucudq.cn

[C12] 立即执行函数 IIFE
来源：http://flt.tianlin.xyz

Py:   (lambda: print("run"))()
来源：http://fkg.sysykeji.top

PHP:  (function () { echo "run"; })();
来源：http://ozz.sjlbkw.cn

JS:   (() => { console.log("run"); })();
来源：http://pyz.sjlbkw.cn

TS:   (() => { console.log("run"); })();
来源：http://exk.zhixingplan.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kgh.yuanzhike.top

Go:   func() { fmt.Println("run") }()
来源：http://wpw.wangdashe.top

Ruby: -> { puts "run" }.call
来源：http://ryf.andypj.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://sii.ivvv.top

[C13] 类型声明 / 类型注解
来源：http://qak.redwolf501.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://exq.zhixingplan.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ehb.jianghu66.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wtp.sufxvd.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hqg.hnxiangtu.top

Java: int add(int a, int b) { return a + b; }
来源：http://rsb.xylfe.cn

Go:   func add(a, b int) int
来源：http://uog.chenjidiqi.icu

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hvc.sweek.top

C#:   int Add(int a, int b) => a + b;
来源：http://qqt.jinghuilouyu.cn

[C14] 泛型函数
来源：http://qxt.gzhubu.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://iwl.feifeiyinyue.top

PHP:  // 无泛型
来源：http://lci.hongshengwenyu.top

JS:   // 无泛型
来源：http://qns.52xcode.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vlz.tarul.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cpo.ehwqpu.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fhz.zhongyouzk.top

Ruby: # 无泛型
来源：http://fsn.ppjwa.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://utx.jiagoushi.top

[C15] 解构 / 展开参数
来源：http://agm.vqdsnc.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://sxy.sweek.top

PHP:  [$a, $b] = $pair;
来源：http://bsw.sufxvd.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://moq.shanyushiyangkeji.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wur.dashuyun.cn

Java: // 无解构
来源：http://rac.chenlongwang.top

Go:   // 无解构
来源：http://ogj.zhiwuduotai.top

Ruby: a, b = pair
来源：http://ayx.haohaochexian.top

C#:   var (a, b) = pair;
来源：http://kpn.yuxming.cn

[C16] 函数 / 方法重载
来源：http://mgv.ehwqpu.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vrl.hnxiangtu.top

PHP:  // 无重载
来源：http://gqr.yonumen.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://eqf.pycfn.com

TS:   // 用联合类型或重载签名声明
来源：http://tmy.jqgufenzy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://oui.zycfv.cn

Go:   // 无重载：用不同函数名
来源：http://yqu.yueranfly.top

Ruby: # 无重载：靠动态参数
来源：http://wkg.yfazqb.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://mwo.zhaomingkeji.xyz

================================================================================
来源：http://fdj.zhongyouzk.top

D. 数组 / 列表 / 集合
来源：http://llg.gaohongyu789.top

================================================================================
来源：http://rjh.zycfv.cn

[D01] 创建数组 / 列表
来源：http://soh.zhoulong.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://skg.fengsongda.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hvj.sweek.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qym.shanyushiyangtech.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://tgj.vqdsnc.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gyr.pengpengdd.cyou

Go:   arr := []int{1, 2, 3}
来源：http://oym.chenjidiqi.icu

Ruby: arr = [1, 2, 3]
来源：http://nhn.zdbjq.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kpq.daxiang520.top

[D02] 追加元素到末尾
来源：http://osa.pengpengdd.cyou

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nzc.cqqwz.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pbj.xingfuxueyuan.xyz

JS:   arr.push(4);
来源：http://kci.nanxuanxn.top

TS:   arr.push(4);
来源：http://cgv.shuidangran.top

Java: list.add(4);
来源：http://hjn.9152youxi.cn

Go:   arr = append(arr, 4)
来源：http://dch.hnqzz.top

Ruby: arr << 4; arr.push(5)
来源：http://cjs.nwbrower.top

C#:   list.Add(4);
来源：http://xbx.bbcook.cn

[D03] 在指定位置插入元素
来源：http://tle.sxryk.cn

Py:   arr.insert(0, 0)
来源：http://kze.yangfankeji.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kbg.ehwqpu.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rfo.shanyushiyangtech.top

TS:   arr.splice(0, 0, 0);
来源：http://cyc.birdmap.top

Java: list.add(0, 0);
来源：http://cpz.zhongyouzk.top

Go:   arr = append([]int{0}, arr...)
来源：http://hvu.epnwcf.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lbz.hywenlv.cn

C#:   list.Insert(0, 0);
来源：http://blm.aibaodan.cn

[D04] 删除元素
来源：http://gjj.9152youxi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ruv.jianghu66.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pkf.cheryme.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://uou.fktsv.cn

TS:   arr.splice(0, 1);
来源：http://neb.mhx1999.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dsu.tanke756.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fxy.sysykeji.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://btc.chenlongwang.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nzi.yanxiufei.cn

[D05] 访问与修改元素
来源：http://mii.gaohongyu789.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://oef.svipenyu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://uzh.hnxiangtu.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://oki.redwolf501.top

TS:   arr[0]; arr.at(-1);
来源：http://gtb.xuetiantiany.cn

Java: list.get(0); list.set(0, 9);
来源：http://paz.fengsongda.top

Go:   arr[0]; arr[0] = 9
来源：http://cfn.tianlin.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fac.wangshuangyany.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://quv.andypj.xyz

[D06] 数组长度
来源：http://qvd.shuidangran.top

Py:   len(arr)
来源：http://mhv.redwolf501.top

PHP:  count($arr);
来源：http://okw.svipenyu.cn

JS:   arr.length
来源：http://zrq.shuidangran.top

TS:   arr.length
来源：http://pbb.hysaishi.cn

Java: list.size();
来源：http://tzj.chenjidiqi.icu

Go:   len(arr)
来源：http://qnf.c1oappe.top

Ruby: arr.length; arr.size
来源：http://wyy.hywenlv.cn

C#:   list.Count;
来源：http://tbz.smart0.xyz

[D07] 切片 / 取子数组
来源：http://vay.jyoumei.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fvh.gaohongyu789.top

PHP:  array_slice($arr, 1, 3);
来源：http://azl.fehbvm.com

JS:   arr.slice(1, 4);
来源：http://jui.jinyuanbaomall.cn

TS:   arr.slice(1, 4);
来源：http://kro.haohaochexian.top

Java: list.subList(1, 4);
来源：http://rys.havefunace.top

Go:   arr[1:4]
来源：http://txe.ehwqpu.com

Ruby: arr[1, 3]
来源：http://jgr.shuidangran.top

C#:   list.GetRange(1, 3);
来源：http://ghr.vehdjk.com

[D08] 合并两个数组
来源：http://vkq.0kj1m.cn

Py:   a + b;  a.extend(b)
来源：http://kce.fzhhl.top

PHP:  array_merge($a, $b);
来源：http://mfr.tian-w.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://sqc.tanke756.top

TS:   [...a, ...b];
来源：http://zam.bjfxy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mlq.fanxiaobao.xyz

Go:   append(a, b...)
来源：http://xhc.xinyue.icu

Ruby: a + b;  a.concat(b)
来源：http://chs.jianghu66.top

C#:   a.Concat(b).ToList()
来源：http://sls.wangshuangyany.cn

[D09] 排序（升序）
来源：http://dnn.jinqigfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://vjh.gzhubu.top

PHP:  sort($arr);
来源：http://ehk.daxiang520.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://iqm.feifeiyinyue.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://wlj.cqqwz.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vyz.chenzaomai.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tld.wangshuangyany.cn

Ruby: arr.sort
来源：http://eya.ybcxt.top

C#:   list.Sort();
来源：http://zjs.zhijiandao.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ugd.ydzc1.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://aic.fanxiaobao.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lbc.aizwys.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kpt.zhixingplan.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://deq.jinghuilouyu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gii.daria6918.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ksw.sjlbkw.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rui.hcnkem.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://svi.mhx1999.top

[D11] 反转数组
来源：http://bxl.gaohongyu789.top

Py:   arr[::-1];  arr.reverse()
来源：http://llx.jinyuanbaomall.cn

PHP:  array_reverse($arr);
来源：http://jzs.chenzaomai.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yoe.yuxming.cn

TS:   [...arr].reverse();
来源：http://qac.9152youxi.cn

Java: Collections.reverse(list);
来源：http://zin.shanyushiyangkeji.top

Go:   slices.Reverse(arr)
来源：http://ptz.dashuyun.cn

Ruby: arr.reverse
来源：http://aoz.sysykeji.top

C#:   list.Reverse();
来源：http://spt.gogol.net.cn

[D12] 查找元素下标
来源：http://oja.wangdashe.top

Py:   arr.index(x);  x in arr
来源：http://dus.fehbvm.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://etd.ydjk.org.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hcd.jqgufenzy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lou.xziqi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hks.aizwys.cn

Go:   slices.Index(arr, x)
来源：http://wkg.hnqzz.top

Ruby: arr.index(x)
来源：http://wco.jiagoushi.top

C#:   list.IndexOf(x);
来源：http://fkx.yj202588.top

[D13] 过滤（保留满足条件的）
来源：http://zvx.dianchejie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gta.wangshuangyany.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hix.havefunace.top

JS:   arr.filter(x => x > 3)
来源：http://bmi.epnwcf.com

TS:   arr.filter(x => x > 3)
来源：http://tsc.yj202588.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://uhg.ctjpmb.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://uql.316326.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://srd.zycfv.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://axz.yfazqb.com

[D14] 映射转换（每个元素变形）
来源：http://fhe.ctjpmb.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dcs.fanxiaobao.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zas.mhx1999.top

JS:   arr.map(x => x * 2)
来源：http://ruu.daxiang520.top

TS:   arr.map(x => x * 2)
来源：http://fzw.feifeiyinyue.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://azr.chenlongwang.top

Go:   // 手写循环
来源：http://yhl.xingfuxueyuan.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://scj.yangfankeji.com

C#:   list.Select(x => x * 2).ToList()
来源：http://gld.havefunace.top

[D15] 去重
来源：http://ubq.sysykeji.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://brd.zhoulong.xyz

PHP:  array_unique($arr);
来源：http://jxj.jqgfzy.top

JS:   [...new Set(arr)]
来源：http://epf.feifeiyinyue.top

TS:   [...new Set(arr)]
来源：http://skn.jinyuanbaomall.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://aqw.mhx1999.top

Go:   // 用 map[T]struct{} 手写
来源：http://fer.zycfv.cn

Ruby: arr.uniq
来源：http://kwv.vehdjk.com

C#:   list.Distinct().ToList()
来源：http://aop.ywan-chungtsiang.top

[D16] 求和与平均值
来源：http://yqp.ydzc1.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kjk.ybcxt.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mfh.hesvh.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://svn.uphjek.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xqu.shangyingyoupin.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bnw.316326.xyz

Go:   // 手写循环累加
来源：http://bql.hnxiangtu.top


<!-- 参考信息 -->