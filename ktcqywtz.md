代发 wailian999

Py:   if not data: return
来源：http://hrr.fanxiaobao.xyz

PHP:  if (!$data) { return; }
来源：http://anu.dashuyun.cn

JS:   if (!data) return;
来源：http://qmh.yj20258888.top

TS:   if (!data) return;
来源：http://egt.gaohongyu789.top

Java: if (data == null) return;
来源：http://iav.quarkkingdee.top

Go:   if data == nil { return }
来源：http://jdt.jianghu66.top

Ruby: return if data.nil?
来源：http://ulm.yonumen.top

C#:   if (data == null) return;
来源：http://ivg.nanxuanxn.top

================================================================================
来源：http://wct.jinqigufen.top

C. 函数与作用域
来源：http://opy.ehwqpu.com

================================================================================
来源：http://rrh.feifeiyinyue.top

[C01] 定义函数
来源：http://qbx.redwolf501.top

Py:   def add(a, b): return a + b
来源：http://yul.0kj1m.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://obp.zhijiandao.cn

JS:   function add(a, b) { return a + b; }
来源：http://biu.bjfxy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qsn.yongpay.top

Java: static int add(int a, int b) { return a + b; }
来源：http://hmw.daria6918.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qfl.yj20258888.top

Ruby: def add(a, b); a + b; end
来源：http://sou.mhx1999.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://brt.tanke756.top

[C02] 默认参数
来源：http://ola.zycfv.cn

Py:   def greet(name="World"): return name
来源：http://zlf.cucudq.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://bwb.fzhhl.top

JS:   function greet(name = "World") { return name; }
来源：http://vne.chenlongwang.top

TS:   function greet(name: string = "World") { return name; }
来源：http://fdz.ydzc1.top

Java: // 无默认参数：方法重载或 Optional
来源：http://fzs.hesvh.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vln.svipenyu.cn

Ruby: def greet(name = "World") = name
来源：http://ado.yueranfly.top

C#:   string Greet(string name = "World") => name;
来源：http://umk.316326.xyz

[C03] 可变参数
来源：http://ufn.chenlongwang.top

Py:   def total(*args): return sum(args)
来源：http://yav.jinghuilouyu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dsf.c1oappe.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mme.sysykeji.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zfd.daria6918.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ysx.yangfankeji.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hmb.aibaodan.cn

Ruby: def total(*nums); nums.sum; end
来源：http://kyy.316326.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://esu.xinyue.icu

[C04] 命名参数 / 关键字参数
来源：http://jod.xylfe.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bjx.guowangkeji.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gwe.sufxvd.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ixx.redwolf501.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://afo.zhixingplan.top

Java: // 无：用 Builder 模式或 record
来源：http://aai.hcnkem.com

Go:   // 无：用配置结构体参数
来源：http://jgs.0kj1m.cn

Ruby: f(a: 1, b: 2)
来源：http://wng.jinqigufen.top

C#:   f(a: 1, b: 2)
来源：http://zmn.ydjk.org.cn

[C05] 返回多个值
来源：http://wop.jianghu66.top

Py:   return a, b
来源：http://kwb.havefunace.top

PHP:  return [$a, $b];
来源：http://hjm.cucudq.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://qqs.xingfuxueyuan.xyz

TS:   return { a, b };
来源：http://kfh.pycfn.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vpu.gaohongyu789.top

Go:   return a, b
来源：http://mjn.jinqigufen.top

Ruby: return a, b
来源：http://diu.jqgfzy.top

C#:   return (a, b);              // ValueTuple
来源：http://ulz.ybcxt.top

[C06] 匿名函数 / lambda
来源：http://ghf.bjfxy.top

Py:   square = lambda x: x * x
来源：http://nlg.yueranfly.top

PHP:  $square = fn($x) => $x * $x;
来源：http://asg.cucudq.cn

JS:   const square = x => x * x;
来源：http://yru.wangdashe.top

TS:   const square = (x: number): number => x * x;
来源：http://crb.smart0.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mzy.xingfuxueyuan.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://fri.ydzc1.top

Ruby: square = ->(x) { x * x }
来源：http://bez.yj20258.top

C#:   Func<int, int> square = x => x * x;
来源：http://atk.jinqigufen.top

[C07] 把函数作为参数传入
来源：http://ztm.yonumen.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gii.hesvh.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xxx.ctjpmb.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tuo.c1oappe.top

TS:   arr.map(String)
来源：http://bvt.gzhubu.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cku.tarul.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qiq.fengsongda.top

Ruby: arr.map(&:upcase)
来源：http://kbg.sufxvd.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://opk.hongshengwenyu.top

[C08] 闭包
来源：http://msh.smart0.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wdr.cqqwz.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://joi.jinqigufen.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vzp.jianghu66.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sew.guowangkeji.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bfo.zycfv.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ksu.hysaishi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://das.vehdjk.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mwk.gotoacloud.top

[C09] 递归
来源：http://cxi.daria6918.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cym.fehbvm.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bli.cashguo.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rrc.vqdsnc.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hpl.cucudq.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pvn.hysaishi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://old.hesvh.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cby.ywan-chungtsiang.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fwk.chenzaomai.com

[C10] 变量作用域
来源：http://hrk.chenjidiqi.icu

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vrm.birdmap.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qnq.xuetiantiany.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hpl.aibaodan.cn

TS:   同 JS
来源：http://uzg.zhijiandao.cn

Java: 方法内为块级作用域
来源：http://ifp.chenzaomai.com

Go:   花括号块级作用域
来源：http://qzn.yvedp.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://iac.xingfuxueyuan.xyz

C#:   块级作用域
来源：http://gle.zhiwuduotai.top

[C11] 模块导入与导出
来源：http://xlh.nwbrower.top

Py:   from module import func
来源：http://sla.ydzc1.top

PHP:  require "file.php";  或 use App\Service;
来源：http://xng.zdbjq.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zsw.yuanzhike.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bpw.hywenlv.cn

Java: import java.util.List;
来源：http://lbd.cheryme.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://toi.jinqigfzy.top

Ruby: require "json"; require_relative "./util"
来源：http://faq.ybcxt.top

C#:   using System.Text;
来源：http://bzr.52xcode.cn

[C12] 立即执行函数 IIFE
来源：http://fgs.cqqwz.cn

Py:   (lambda: print("run"))()
来源：http://pkf.xylfe.cn

PHP:  (function () { echo "run"; })();
来源：http://wxs.zhijiandao.cn

JS:   (() => { console.log("run"); })();
来源：http://zaq.smart0.xyz

TS:   (() => { console.log("run"); })();
来源：http://bun.shanyushiyangkeji.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://sae.snrcjt.cn

Go:   func() { fmt.Println("run") }()
来源：http://zsk.zhixingplan.top

Ruby: -> { puts "run" }.call
来源：http://gss.shzxlz.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://hze.yonumen.top

[C13] 类型声明 / 类型注解
来源：http://vsn.hcnkem.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mlx.fehbvm.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://udi.tarul.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kkd.zhaomingkeji.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dbg.svipenyu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://kgs.bjfxy.top

Go:   func add(a, b int) int
来源：http://csl.yvedp.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://doj.shangyingyoupin.top

C#:   int Add(int a, int b) => a + b;
来源：http://dna.jqgfzy.top

[C14] 泛型函数
来源：http://wtb.xylfe.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://its.mhx1999.top

PHP:  // 无泛型
来源：http://rdj.ehwqpu.com

JS:   // 无泛型
来源：http://gua.sufxvd.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zbj.zycfv.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://urk.aizwys.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lof.smart0.xyz

Ruby: # 无泛型
来源：http://ozz.tanke756.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dfw.hcnkem.com

[C15] 解构 / 展开参数
来源：http://xyw.chenjidiqi.icu

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gkd.kuanghao11.cn

PHP:  [$a, $b] = $pair;
来源：http://qcz.hammf.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zgt.fanxiaobao.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ccr.fanxiaobao.xyz

Java: // 无解构
来源：http://sdj.fehbvm.com

Go:   // 无解构
来源：http://tuo.andypj.xyz

Ruby: a, b = pair
来源：http://ejd.kuanghao11.cn

C#:   var (a, b) = pair;
来源：http://wvj.cqqwz.cn

[C16] 函数 / 方法重载
来源：http://rjs.hnxiangtu.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bws.dianchejie.cn

PHP:  // 无重载
来源：http://jtw.zhiwuduotai.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://mww.jinqigfzy.top

TS:   // 用联合类型或重载签名声明
来源：http://qcz.hnxiangtu.top

Java: void f(int a) {}  void f(String a) {}
来源：http://djl.jlsjyb.cn

Go:   // 无重载：用不同函数名
来源：http://vpc.vehdjk.com

Ruby: # 无重载：靠动态参数
来源：http://zjf.cashguo.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://slb.havefunace.top

================================================================================
来源：http://aji.yuxming.cn

D. 数组 / 列表 / 集合
来源：http://upu.smart0.xyz

================================================================================
来源：http://sfj.kuanghao11.cn

[D01] 创建数组 / 列表
来源：http://vrc.daria6918.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://kjq.epnwcf.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xnh.nanxinkj.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ynj.ywan-chungtsiang.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://kuy.jqgufenzy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ovf.0kj1m.cn

Go:   arr := []int{1, 2, 3}
来源：http://mvy.cqqwz.cn

Ruby: arr = [1, 2, 3]
来源：http://obq.nanxuanxn.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kwj.hnxiangtu.top

[D02] 追加元素到末尾
来源：http://grp.yueranfly.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://res.redwolf501.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kap.wangdashe.top

JS:   arr.push(4);
来源：http://piv.chenlongwang.top

TS:   arr.push(4);
来源：http://ynb.smart0.xyz

Java: list.add(4);
来源：http://dhv.yj20258.top

Go:   arr = append(arr, 4)
来源：http://xam.jiagoushi.top

Ruby: arr << 4; arr.push(5)
来源：http://tpo.fengsongda.top

C#:   list.Add(4);
来源：http://qbc.jianghu66.top

[D03] 在指定位置插入元素
来源：http://izi.feifeiyinyue.top

Py:   arr.insert(0, 0)
来源：http://tew.xziqi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hir.zhoulong.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hle.uphjek.com

TS:   arr.splice(0, 0, 0);
来源：http://gml.ehwqpu.com

Java: list.add(0, 0);
来源：http://xld.gogol.net.cn

Go:   arr = append([]int{0}, arr...)
来源：http://yni.yongpay.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ftx.yanxiufei.cn

C#:   list.Insert(0, 0);
来源：http://oas.havefunace.top

[D04] 删除元素
来源：http://fwy.cdnleiting.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://iyr.yanxiufei.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ktb.tanke756.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gvu.jinghuilouyu.cn

TS:   arr.splice(0, 1);
来源：http://jtk.hywenlv.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://neb.sysykeji.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mrb.zhaomingkeji.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pfm.yfazqb.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wpb.hywenlv.cn

[D05] 访问与修改元素
来源：http://lcj.zhijiandao.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://krv.sweek.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sgp.yongpay.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vuh.tarul.cn

TS:   arr[0]; arr.at(-1);
来源：http://fkl.c1oappe.top

Java: list.get(0); list.set(0, 9);
来源：http://jqn.jqgfzy.top

Go:   arr[0]; arr[0] = 9
来源：http://yxl.vehdjk.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zvg.hnqzz.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dqz.zhoulong.xyz

[D06] 数组长度
来源：http://pjq.yuanzhike.top

Py:   len(arr)
来源：http://kbb.wangdashe.top

PHP:  count($arr);
来源：http://zvx.xuetiantiany.cn

JS:   arr.length
来源：http://mvv.daria6918.cn

TS:   arr.length
来源：http://rfl.hongshengwenyu.top

Java: list.size();
来源：http://okp.ctjpmb.com

Go:   len(arr)
来源：http://qkc.zhongyouzk.top

Ruby: arr.length; arr.size
来源：http://fhw.chenzaomai.com

C#:   list.Count;
来源：http://odl.jinghuilouyu.cn

[D07] 切片 / 取子数组
来源：http://gpt.jinqigfzy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ryc.xingfuxueyuan.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://gul.fehbvm.com

JS:   arr.slice(1, 4);
来源：http://qsk.9152youxi.cn

TS:   arr.slice(1, 4);
来源：http://yjl.jiagoushi.top

Java: list.subList(1, 4);
来源：http://yoj.tanke756.top

Go:   arr[1:4]
来源：http://xgl.snrcjt.cn

Ruby: arr[1, 3]
来源：http://abp.hywenlv.cn

C#:   list.GetRange(1, 3);
来源：http://cxy.0kj1m.cn

[D08] 合并两个数组
来源：http://xrr.fanxiaobao.xyz

Py:   a + b;  a.extend(b)
来源：http://pxs.guowangkeji.top

PHP:  array_merge($a, $b);
来源：http://kfy.shuidangran.top

JS:   [...a, ...b];  a.concat(b);
来源：http://yan.fehbvm.com

TS:   [...a, ...b];
来源：http://nvq.ehwqpu.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ktn.jqgufenzy.top

Go:   append(a, b...)
来源：http://lyd.yonumen.top

Ruby: a + b;  a.concat(b)
来源：http://kjs.bjfxy.top

C#:   a.Concat(b).ToList()
来源：http://yel.guowangkeji.top

[D09] 排序（升序）
来源：http://rrn.quarkkingdee.top

Py:   sorted(arr);  arr.sort()
来源：http://eyb.hesvh.cn

PHP:  sort($arr);
来源：http://kkw.hesvh.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hbx.zhixingplan.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://vgv.vqdsnc.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xkn.ydzc1.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lvj.redwolf501.top

Ruby: arr.sort
来源：http://mrl.havefunace.top

C#:   list.Sort();
来源：http://egn.hysaishi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://bxw.yonumen.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://krp.yuanzhike.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fua.shzxlz.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kvq.vqdsnc.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bub.hywenlv.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://evm.52xcode.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yxz.hfpthk.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zue.yj20258888.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://uwg.xylfe.cn

[D11] 反转数组
来源：http://tvk.zhiwuduotai.top

Py:   arr[::-1];  arr.reverse()
来源：http://ezv.jiagoushi.top

PHP:  array_reverse($arr);
来源：http://txc.jyoumei.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nno.sxryk.cn

TS:   [...arr].reverse();
来源：http://rov.chenzaomai.com

Java: Collections.reverse(list);
来源：http://czo.yonumen.top

Go:   slices.Reverse(arr)
来源：http://kmy.gzhubu.top

Ruby: arr.reverse
来源：http://vlt.shzxlz.cn

C#:   list.Reverse();
来源：http://wua.meibo888.top

[D12] 查找元素下标
来源：http://kkl.chenjidiqi.icu

Py:   arr.index(x);  x in arr
来源：http://htq.zdbjq.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://toz.9152youxi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wzp.cheryme.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pts.shanyushiyangkeji.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://orq.zhixingplan.top

Go:   slices.Index(arr, x)
来源：http://jux.chenzaomai.com

Ruby: arr.index(x)
来源：http://ouo.sufxvd.cn

C#:   list.IndexOf(x);
来源：http://yqj.pengpengdd.cyou

[D13] 过滤（保留满足条件的）
来源：http://cfv.tian-w.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zxh.mhx1999.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fdt.fktsv.cn

JS:   arr.filter(x => x > 3)
来源：http://dob.gaohongyu789.top

TS:   arr.filter(x => x > 3)
来源：http://lte.xylfe.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hkj.hongshengwenyu.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tky.shzxlz.cn

Ruby: arr.select { |x| x > 3 }
来源：http://dzn.sweek.top

C#:   list.Where(x => x > 3).ToList()
来源：http://rjm.fehbvm.com

[D14] 映射转换（每个元素变形）
来源：http://lou.pengpengdd.cyou

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hvf.cucudq.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ldw.birdmap.top

JS:   arr.map(x => x * 2)
来源：http://mzj.sjlbkw.cn

TS:   arr.map(x => x * 2)
来源：http://tcs.tian-w.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://qsh.iojbl.cn

Go:   // 手写循环
来源：http://uwu.zhixingplan.top

Ruby: arr.map { |x| x * 2 }
来源：http://nfl.snrcjt.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xud.yuanzhike.top

[D15] 去重
来源：http://upq.fzhhl.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://roi.yongpay.top

PHP:  array_unique($arr);
来源：http://xbw.nwbrower.top

JS:   [...new Set(arr)]
来源：http://oef.jlsjyb.cn

TS:   [...new Set(arr)]
来源：http://wka.nwbrower.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fur.xuetiantiany.cn

Go:   // 用 map[T]struct{} 手写
来源：http://dou.yangfankeji.com

Ruby: arr.uniq
来源：http://yyr.hywenlv.cn

C#:   list.Distinct().ToList()
来源：http://alq.jianghu66.top

[D16] 求和与平均值
来源：http://ydh.ywan-chungtsiang.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gwy.yfazqb.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zks.zycfv.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wpe.feifeiyinyue.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ast.zhijiandao.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nxd.0kj1m.cn

Go:   // 手写循环累加
来源：http://ctr.9152youxi.cn


<!-- 参考信息 -->