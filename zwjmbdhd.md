代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://nrf.fzhhl.top

Go:   func add(a, b int) int { return a + b }
来源：http://diq.jinqigfzy.top

Ruby: def add(a, b); a + b; end
来源：http://drw.fzhhl.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yea.pycfn.com

[C02] 默认参数
来源：http://yhi.yonumen.top

Py:   def greet(name="World"): return name
来源：http://jbv.hesvh.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://lok.tarul.cn

JS:   function greet(name = "World") { return name; }
来源：http://suu.dashuyun.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://klf.tarul.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://onz.vehdjk.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ykp.zhixingplan.top

Ruby: def greet(name = "World") = name
来源：http://trf.cashguo.top

C#:   string Greet(string name = "World") => name;
来源：http://uip.shzxlz.cn

[C03] 可变参数
来源：http://zjp.hnxiangtu.top

Py:   def total(*args): return sum(args)
来源：http://ymc.meibo888.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nzi.pengpengdd.cyou

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hfb.sweek.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xfj.yangfankeji.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://krg.jinqigfzy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://axg.jinghuilouyu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vps.epnwcf.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qoo.smart0.xyz

[C04] 命名参数 / 关键字参数
来源：http://hsf.chenlongwang.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://com.bjfxy.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://knc.shzxlz.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dfq.yuanzhike.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mzd.ivvv.top

Java: // 无：用 Builder 模式或 record
来源：http://yhm.zhongyouzk.top

Go:   // 无：用配置结构体参数
来源：http://eof.tianlin.xyz

Ruby: f(a: 1, b: 2)
来源：http://adi.jiagoushi.top

C#:   f(a: 1, b: 2)
来源：http://pge.fengsongda.top

[C05] 返回多个值
来源：http://fnp.pengpengdd.cyou

Py:   return a, b
来源：http://gsv.chenlongwang.top

PHP:  return [$a, $b];
来源：http://teb.hesvh.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jnp.xingfuxueyuan.xyz

TS:   return { a, b };
来源：http://flq.tianlin.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://oit.havefunace.top

Go:   return a, b
来源：http://rta.hnxiangtu.top

Ruby: return a, b
来源：http://zzs.52xcode.cn

C#:   return (a, b);              // ValueTuple
来源：http://moq.zdbjq.cn

[C06] 匿名函数 / lambda
来源：http://nyw.yangfankeji.com

Py:   square = lambda x: x * x
来源：http://vlm.jlsjyb.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://nwl.shangyingyoupin.top

JS:   const square = x => x * x;
来源：http://yit.quarkkingdee.top

TS:   const square = (x: number): number => x * x;
来源：http://tln.ybcxt.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vny.andypj.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://klo.cqqwz.cn

Ruby: square = ->(x) { x * x }
来源：http://evs.ybcxt.top

C#:   Func<int, int> square = x => x * x;
来源：http://zik.jqgufenzy.top

[C07] 把函数作为参数传入
来源：http://xht.chenlongwang.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://znq.snrcjt.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hry.zycfv.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://caq.tarul.cn

TS:   arr.map(String)
来源：http://gny.yj20258888.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tqz.hnqzz.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fcj.sweek.top

Ruby: arr.map(&:upcase)
来源：http://gno.cucudq.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://deu.cashguo.top

[C08] 闭包
来源：http://tgw.wangshuangyany.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://csy.haohaochexian.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ujq.ehwqpu.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dlu.316326.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wvk.nanxuanxn.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yuy.vehdjk.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://unh.ivvv.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mwr.hammf.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://eyq.c1oappe.top

[C09] 递归
来源：http://aub.aizwys.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sdo.nanxinkj.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://aqx.yj20258888.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cil.sweek.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vra.feifeiyinyue.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fuw.jqgfzy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cao.iojbl.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fvx.ivvv.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hcc.tianlin.xyz

[C10] 变量作用域
来源：http://nqd.aizwys.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ptv.bjfxy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kzt.yj20258888.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://sdv.nanxinkj.top

TS:   同 JS
来源：http://ubb.smart0.xyz

Java: 方法内为块级作用域
来源：http://sgz.birdmap.top

Go:   花括号块级作用域
来源：http://xhm.cucudq.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xfe.sxryk.cn

C#:   块级作用域
来源：http://slz.bbcook.cn

[C11] 模块导入与导出
来源：http://lrx.zhiwuduotai.top

Py:   from module import func
来源：http://ztp.zdqjudy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://sos.wangdashe.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://den.yj20258888.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lzo.haohaochexian.top

Java: import java.util.List;
来源：http://rfg.hcnkem.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mtc.tarul.cn

Ruby: require "json"; require_relative "./util"
来源：http://egj.shanyushiyangkeji.top

C#:   using System.Text;
来源：http://bmm.tianlin.xyz

[C12] 立即执行函数 IIFE
来源：http://knk.nanxinkj.top

Py:   (lambda: print("run"))()
来源：http://soz.daxiang520.top

PHP:  (function () { echo "run"; })();
来源：http://ynp.yj20258.top

JS:   (() => { console.log("run"); })();
来源：http://sqk.feifeiyinyue.top

TS:   (() => { console.log("run"); })();
来源：http://qjo.tian-w.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qsf.chenzaomai.com

Go:   func() { fmt.Println("run") }()
来源：http://riu.sysykeji.top

Ruby: -> { puts "run" }.call
来源：http://lon.zdbjq.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://iya.fzhhl.top

[C13] 类型声明 / 类型注解
来源：http://pmu.fengsongda.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jyc.gogol.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lsk.fanxiaobao.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://din.ybcxt.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mad.hongshengwenyu.top

Java: int add(int a, int b) { return a + b; }
来源：http://knd.yuxming.cn

Go:   func add(a, b int) int
来源：http://wdk.uphjek.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hte.shanyushiyangtech.top

C#:   int Add(int a, int b) => a + b;
来源：http://biq.zhoulong.xyz

[C14] 泛型函数
来源：http://nxl.jqgufenzy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://akt.xuetiantiany.cn

PHP:  // 无泛型
来源：http://rvq.chenlongwang.top

JS:   // 无泛型
来源：http://oxt.zhongyouzk.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://puu.fanxiaobao.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://moc.snrcjt.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://eue.cheryme.top

Ruby: # 无泛型
来源：http://lcd.cheryme.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fpb.bbcook.cn

[C15] 解构 / 展开参数
来源：http://wax.yangfankeji.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dhp.bjfxy.top

PHP:  [$a, $b] = $pair;
来源：http://khi.ydzc1.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mvw.aibaodan.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ybp.gotoacloud.top

Java: // 无解构
来源：http://yfy.hnqzz.top

Go:   // 无解构
来源：http://wvb.cqqwz.cn

Ruby: a, b = pair
来源：http://tkx.jqgfzy.top

C#:   var (a, b) = pair;
来源：http://qsj.zycfv.cn

[C16] 函数 / 方法重载
来源：http://mat.epnwcf.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://uwl.yangfankeji.com

PHP:  // 无重载
来源：http://mmd.snrcjt.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://tcp.wangshuangyany.cn

TS:   // 用联合类型或重载签名声明
来源：http://avn.yongpay.top

Java: void f(int a) {}  void f(String a) {}
来源：http://gdk.nwbrower.top

Go:   // 无重载：用不同函数名
来源：http://glu.xuanzx.com

Ruby: # 无重载：靠动态参数
来源：http://wty.vqdsnc.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://uvo.fzhhl.top

================================================================================
来源：http://uod.zhiwuduotai.top

D. 数组 / 列表 / 集合
来源：http://mcn.zhixingplan.top

================================================================================
来源：http://wpw.mhx1999.top

[D01] 创建数组 / 列表
来源：http://fcb.tian-w.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ljy.cucudq.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://uzm.yj20258888.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://uqz.redwolf501.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://hug.bjfxy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zkr.aizwys.cn

Go:   arr := []int{1, 2, 3}
来源：http://kyf.iojbl.cn

Ruby: arr = [1, 2, 3]
来源：http://guq.hongshengwenyu.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zcf.gogol.net.cn

[D02] 追加元素到末尾
来源：http://agq.daria6918.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qod.fktsv.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qcn.jyoumei.cn

JS:   arr.push(4);
来源：http://dmx.gotoacloud.top

TS:   arr.push(4);
来源：http://xba.xuetiantiany.cn

Java: list.add(4);
来源：http://owc.cashguo.top

Go:   arr = append(arr, 4)
来源：http://tjp.hesvh.cn

Ruby: arr << 4; arr.push(5)
来源：http://lfy.iojbl.cn

C#:   list.Add(4);
来源：http://vtz.yueranfly.top

[D03] 在指定位置插入元素
来源：http://zkk.tianlin.xyz

Py:   arr.insert(0, 0)
来源：http://pau.wangdashe.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vbr.uphjek.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wvc.pengpengdd.cyou

TS:   arr.splice(0, 0, 0);
来源：http://idq.ehwqpu.com

Java: list.add(0, 0);
来源：http://vnx.xuanzx.com

Go:   arr = append([]int{0}, arr...)
来源：http://opm.vehdjk.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wln.aibaodan.cn

C#:   list.Insert(0, 0);
来源：http://xdz.gaohongyu789.top

[D04] 删除元素
来源：http://mdc.hcnkem.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tqx.chenjidiqi.icu

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lbz.zdqjudy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jbu.yj202588.top

TS:   arr.splice(0, 1);
来源：http://jla.jinyuanbaomall.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ifd.chenjidiqi.icu

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jrh.vqdsnc.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://uux.snrcjt.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gbr.sysykeji.top

[D05] 访问与修改元素
来源：http://zrv.xingfuxueyuan.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ukd.cucudq.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://iko.havefunace.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jcm.smart0.xyz

TS:   arr[0]; arr.at(-1);
来源：http://koh.yueranfly.top

Java: list.get(0); list.set(0, 9);
来源：http://dtp.jqgufenzy.top

Go:   arr[0]; arr[0] = 9
来源：http://ssx.havefunace.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hma.fanxiaobao.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ist.guannengcc.top

[D06] 数组长度
来源：http://hpw.smart0.xyz

Py:   len(arr)
来源：http://sda.chenzaomai.com

PHP:  count($arr);
来源：http://yql.sufxvd.cn

JS:   arr.length
来源：http://bjp.aibaodan.cn

TS:   arr.length
来源：http://dww.hfpthk.cn

Java: list.size();
来源：http://fwu.nwbrower.top

Go:   len(arr)
来源：http://ajd.kuanghao11.cn

Ruby: arr.length; arr.size
来源：http://fup.redwolf501.top

C#:   list.Count;
来源：http://wwq.hfpthk.cn

[D07] 切片 / 取子数组
来源：http://que.yvedp.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://sna.sufxvd.cn

PHP:  array_slice($arr, 1, 3);
来源：http://imb.birdmap.top

JS:   arr.slice(1, 4);
来源：http://diq.chenzaomai.com

TS:   arr.slice(1, 4);
来源：http://noo.9152youxi.cn

Java: list.subList(1, 4);
来源：http://tpa.9152youxi.cn

Go:   arr[1:4]
来源：http://idq.zdqjudy.top

Ruby: arr[1, 3]
来源：http://vyx.zdqjudy.top

C#:   list.GetRange(1, 3);
来源：http://vkk.gotoacloud.top

[D08] 合并两个数组
来源：http://zfl.yvedp.cn

Py:   a + b;  a.extend(b)
来源：http://tll.dashuyun.cn

PHP:  array_merge($a, $b);
来源：http://siz.chenlongwang.top

JS:   [...a, ...b];  a.concat(b);
来源：http://eqj.wangdashe.top

TS:   [...a, ...b];
来源：http://ded.jinyuanbaomall.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qqh.haohaochexian.top

Go:   append(a, b...)
来源：http://zkb.feifeiyinyue.top

Ruby: a + b;  a.concat(b)
来源：http://wgg.shuidangran.top

C#:   a.Concat(b).ToList()
来源：http://qtc.gotoacloud.top

[D09] 排序（升序）
来源：http://lpl.ywan-chungtsiang.top

Py:   sorted(arr);  arr.sort()
来源：http://ham.gaohongyu789.top

PHP:  sort($arr);
来源：http://gik.uphjek.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ijg.nanxinkj.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://cgc.cashguo.top

Java: Collections.sort(list);  list.sort(null);
来源：http://mib.hysaishi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qiz.jinqigufen.top

Ruby: arr.sort
来源：http://dyz.316326.xyz

C#:   list.Sort();
来源：http://jom.jinqigfzy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://axa.smart0.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ryc.xuetiantiany.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qod.yonumen.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hmr.fzhhl.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://frl.cdnleiting.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://iai.52xcode.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rfl.feifeiyinyue.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://asy.zhixingplan.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pdl.dashuyun.cn

[D11] 反转数组
来源：http://umu.zhongyouzk.top

Py:   arr[::-1];  arr.reverse()
来源：http://wbz.dashuyun.cn

PHP:  array_reverse($arr);
来源：http://ngl.yj20258888.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jdk.gotoacloud.top

TS:   [...arr].reverse();
来源：http://diz.aibaodan.cn

Java: Collections.reverse(list);
来源：http://jvd.aibaodan.cn

Go:   slices.Reverse(arr)
来源：http://tlp.cheryme.top

Ruby: arr.reverse
来源：http://sun.hongshengwenyu.top

C#:   list.Reverse();
来源：http://qdp.jinghuilouyu.cn

[D12] 查找元素下标
来源：http://yjp.sysykeji.top

Py:   arr.index(x);  x in arr
来源：http://tyc.yvedp.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vdb.fzhhl.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uxc.feifeiyinyue.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hkw.aibaodan.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sth.yanxiufei.cn

Go:   slices.Index(arr, x)
来源：http://yrm.hammf.cn

Ruby: arr.index(x)
来源：http://cse.bbcook.cn

C#:   list.IndexOf(x);
来源：http://jbx.nanxuanxn.top

[D13] 过滤（保留满足条件的）
来源：http://jtl.hammf.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qcs.yonumen.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kfb.jinghuilouyu.cn

JS:   arr.filter(x => x > 3)
来源：http://fnq.zhijiandao.cn

TS:   arr.filter(x => x > 3)
来源：http://phk.jiagoushi.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jjf.chenzaomai.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lgd.chenzaomai.com

Ruby: arr.select { |x| x > 3 }
来源：http://zcb.gogol.net.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://icg.sysykeji.top

[D14] 映射转换（每个元素变形）
来源：http://izg.vehdjk.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vbj.yueranfly.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ikk.shanyushiyangtech.top

JS:   arr.map(x => x * 2)
来源：http://jrd.kuanghao11.cn

TS:   arr.map(x => x * 2)
来源：http://som.vehdjk.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://aab.bjfxy.top

Go:   // 手写循环
来源：http://url.bbcook.cn

Ruby: arr.map { |x| x * 2 }
来源：http://zhf.sweek.top

C#:   list.Select(x => x * 2).ToList()
来源：http://gkf.tianlin.xyz

[D15] 去重
来源：http://cas.snrcjt.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cej.dashuyun.cn

PHP:  array_unique($arr);
来源：http://vav.iojbl.cn

JS:   [...new Set(arr)]
来源：http://qft.fanxiaobao.xyz

TS:   [...new Set(arr)]
来源：http://ywa.cheryme.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jaz.jqgufenzy.top

Go:   // 用 map[T]struct{} 手写
来源：http://dmu.meibo888.top

Ruby: arr.uniq
来源：http://uob.ybcxt.top

C#:   list.Distinct().ToList()
来源：http://zrq.nanxinkj.top

[D16] 求和与平均值
来源：http://veq.zhoulong.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rdd.yongpay.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nae.epnwcf.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pcw.yj20258888.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vbp.zhongyouzk.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ixa.sjlbkw.cn

Go:   // 手写循环累加
来源：http://raa.shangyingyoupin.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lut.zhengqikj.top

C#:   list.Sum();  list.Average()
来源：http://opb.hesvh.cn

[D17] 最大值与最小值
来源：http://inz.zycfv.cn

Py:   max(arr);  min(arr)
来源：http://wke.gogol.net.cn

PHP:  max($arr);  min($arr);
来源：http://mxr.jinyuanbaomall.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zjq.feifeiyinyue.top

TS:   Math.max(...arr);
来源：http://kgn.jiagoushi.top

Java: Collections.max(list);  Collections.min(list);
来源：http://zkx.tanke756.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wtc.yonumen.top

Ruby: arr.max;  arr.min
来源：http://wpi.yuxming.cn

C#:   list.Max();  list.Min()
来源：http://qti.c1oappe.top

[D18] 扁平化嵌套数组
来源：http://kvb.bbcook.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wkl.zhongyouzk.top

PHP:  array_merge(...$nested);
来源：http://wge.chenzaomai.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xpt.jlsjyb.cn

TS:   nested.flat();
来源：http://hpm.pengpengdd.cyou


<!-- 参考信息 -->