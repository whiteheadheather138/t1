代发 wailian999

Py:   if not data: return
来源：http://mom.zhongyouzk.top

PHP:  if (!$data) { return; }
来源：http://wzm.ivvv.top

JS:   if (!data) return;
来源：http://cwf.c1oappe.top

TS:   if (!data) return;
来源：http://fek.guowangkeji.top

Java: if (data == null) return;
来源：http://wah.haohaochexian.top

Go:   if data == nil { return }
来源：http://bki.hnqzz.top

Ruby: return if data.nil?
来源：http://cjs.jqgufenzy.top

C#:   if (data == null) return;
来源：http://are.andypj.xyz

================================================================================
来源：http://ghm.jlsjyb.cn

C. 函数与作用域
来源：http://qss.snrcjt.cn

================================================================================
来源：http://rhe.shanyushiyangkeji.top

[C01] 定义函数
来源：http://jjy.tianlin.xyz

Py:   def add(a, b): return a + b
来源：http://eer.zhoulong.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uhn.zhoulong.xyz

JS:   function add(a, b) { return a + b; }
来源：http://eqy.yj20258888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fay.hnqzz.top

Java: static int add(int a, int b) { return a + b; }
来源：http://xdw.cheryme.top

Go:   func add(a, b int) int { return a + b }
来源：http://rdc.gogol.net.cn

Ruby: def add(a, b); a + b; end
来源：http://bhw.dashuyun.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yfw.aibaodan.cn

[C02] 默认参数
来源：http://nbp.sysykeji.top

Py:   def greet(name="World"): return name
来源：http://vvl.meibo888.top

PHP:  function greet($name = "World") { return $name; }
来源：http://vjr.tanke756.top

JS:   function greet(name = "World") { return name; }
来源：http://tbl.gzhubu.top

TS:   function greet(name: string = "World") { return name; }
来源：http://imj.fzhhl.top

Java: // 无默认参数：方法重载或 Optional
来源：http://txg.zhixingplan.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bdc.gotoacloud.top

Ruby: def greet(name = "World") = name
来源：http://hks.9152youxi.cn

C#:   string Greet(string name = "World") => name;
来源：http://szf.yanxiufei.cn

[C03] 可变参数
来源：http://uyu.nanxinkj.top

Py:   def total(*args): return sum(args)
来源：http://uoe.xinyue.icu

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://glz.kuanghao11.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ywa.snrcjt.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://daj.tianlin.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fmu.ppjwa.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hlh.sxryk.cn

Ruby: def total(*nums); nums.sum; end
来源：http://fih.tian-w.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fhe.svipenyu.cn

[C04] 命名参数 / 关键字参数
来源：http://khc.tanke756.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qju.hfpthk.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://eit.yuanzhike.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gei.jlsjyb.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ffh.jinyuanbaomall.cn

Java: // 无：用 Builder 模式或 record
来源：http://bmz.hysaishi.cn

Go:   // 无：用配置结构体参数
来源：http://pew.tarul.cn

Ruby: f(a: 1, b: 2)
来源：http://wjc.jyoumei.cn

C#:   f(a: 1, b: 2)
来源：http://kdh.zhoulong.xyz

[C05] 返回多个值
来源：http://iuo.gotoacloud.top

Py:   return a, b
来源：http://cdz.gzhubu.top

PHP:  return [$a, $b];
来源：http://axl.xuetiantiany.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://sin.sweek.top

TS:   return { a, b };
来源：http://lun.0kj1m.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://njb.sweek.top

Go:   return a, b
来源：http://yvn.shanyushiyangtech.top

Ruby: return a, b
来源：http://dwz.vqdsnc.cn

C#:   return (a, b);              // ValueTuple
来源：http://xxp.ehwqpu.com

[C06] 匿名函数 / lambda
来源：http://ptv.hcnkem.com

Py:   square = lambda x: x * x
来源：http://fvf.shanyushiyangkeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://lvs.daria6918.cn

JS:   const square = x => x * x;
来源：http://ypc.sweek.top

TS:   const square = (x: number): number => x * x;
来源：http://xhc.shangyingyoupin.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qqt.pycfn.com

Go:   sq := func(x int) int { return x * x }
来源：http://ptw.smart0.xyz

Ruby: square = ->(x) { x * x }
来源：http://yhn.xingfuxueyuan.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://xrz.tianlin.xyz

[C07] 把函数作为参数传入
来源：http://bkf.daria6918.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ins.zdbjq.cn

PHP:  array_map("strtoupper", $arr);
来源：http://lhg.xingfuxueyuan.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ktl.yfazqb.com

TS:   arr.map(String)
来源：http://aan.shanyushiyangkeji.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ttk.jinyuanbaomall.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://aad.mhx1999.top

Ruby: arr.map(&:upcase)
来源：http://dpt.ybcxt.top

C#:   arr.Select(s => s.ToUpper())
来源：http://tof.vehdjk.com

[C08] 闭包
来源：http://vfa.cdnleiting.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://aof.jinghuilouyu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wet.hammf.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bxe.wangshuangyany.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lwr.jyoumei.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yyh.jyoumei.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fpf.andypj.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xdu.pycfn.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xxp.birdmap.top

[C09] 递归
来源：http://xem.yj202588.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rwm.sweek.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fij.sjlbkw.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ewt.guowangkeji.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xkt.birdmap.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://eml.xuetiantiany.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://yaw.cashguo.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ydk.0kj1m.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://weo.yuxming.cn

[C10] 变量作用域
来源：http://pjy.zhixingplan.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qji.zycfv.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qfd.0kj1m.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://oco.mhx1999.top

TS:   同 JS
来源：http://imj.sysykeji.top

Java: 方法内为块级作用域
来源：http://oyt.yuanzhike.top

Go:   花括号块级作用域
来源：http://kln.gzhubu.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tzg.chenzaomai.com

C#:   块级作用域
来源：http://jnb.gaohongyu789.top

[C11] 模块导入与导出
来源：http://hhd.jinyuanbaomall.cn

Py:   from module import func
来源：http://zaa.uphjek.com

PHP:  require "file.php";  或 use App\Service;
来源：http://yiy.redwolf501.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://nzi.shzxlz.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://enp.sjlbkw.cn

Java: import java.util.List;
来源：http://fqf.guannengcc.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qni.jqgfzy.top

Ruby: require "json"; require_relative "./util"
来源：http://trl.0kj1m.cn

C#:   using System.Text;
来源：http://dor.0kj1m.cn

[C12] 立即执行函数 IIFE
来源：http://kqj.bjfxy.top

Py:   (lambda: print("run"))()
来源：http://luv.cheryme.top

PHP:  (function () { echo "run"; })();
来源：http://cni.xuetiantiany.cn

JS:   (() => { console.log("run"); })();
来源：http://elq.snrcjt.cn

TS:   (() => { console.log("run"); })();
来源：http://lmk.feifeiyinyue.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://sgl.chenlongwang.top

Go:   func() { fmt.Println("run") }()
来源：http://qws.yvedp.cn

Ruby: -> { puts "run" }.call
来源：http://mpj.tian-w.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ijg.cucudq.cn

[C13] 类型声明 / 类型注解
来源：http://srj.pycfn.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wrv.tianlin.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://krd.cucudq.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cir.jinqigfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fsm.ivvv.top

Java: int add(int a, int b) { return a + b; }
来源：http://mzr.gaohongyu789.top

Go:   func add(a, b int) int
来源：http://dmi.xuetiantiany.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lnw.zhoulong.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://quj.jinghuilouyu.cn

[C14] 泛型函数
来源：http://mom.quarkkingdee.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xdh.chenlongwang.top

PHP:  // 无泛型
来源：http://omb.xinyue.icu

JS:   // 无泛型
来源：http://ytd.jinyuanbaomall.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kdn.aizwys.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tul.hnxiangtu.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xjj.zhixingplan.top

Ruby: # 无泛型
来源：http://lzp.ppjwa.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jlq.sufxvd.cn

[C15] 解构 / 展开参数
来源：http://mzr.pycfn.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zlq.ywan-chungtsiang.top

PHP:  [$a, $b] = $pair;
来源：http://lzz.cheryme.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zdw.yvedp.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mmw.yvedp.cn

Java: // 无解构
来源：http://ctr.xuanzx.com

Go:   // 无解构
来源：http://zsi.dashuyun.cn

Ruby: a, b = pair
来源：http://nyc.chenlongwang.top

C#:   var (a, b) = pair;
来源：http://bqi.quarkkingdee.top

[C16] 函数 / 方法重载
来源：http://aef.jinghuilouyu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jpe.ywan-chungtsiang.top

PHP:  // 无重载
来源：http://kyy.haohaochexian.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://lmg.yueranfly.top

TS:   // 用联合类型或重载签名声明
来源：http://rlg.sxryk.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ldh.yuxming.cn

Go:   // 无重载：用不同函数名
来源：http://oie.xuetiantiany.cn

Ruby: # 无重载：靠动态参数
来源：http://alo.cdnleiting.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://wnb.zhiwuduotai.top

================================================================================
来源：http://ozh.zhoulong.xyz

D. 数组 / 列表 / 集合
来源：http://sil.chenjidiqi.icu

================================================================================
来源：http://fjn.guannengcc.top

[D01] 创建数组 / 列表
来源：http://ile.cheryme.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://xwn.guowangkeji.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bro.sxryk.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lhi.hcnkem.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://neg.epnwcf.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vot.cqqwz.cn

Go:   arr := []int{1, 2, 3}
来源：http://xld.cashguo.top

Ruby: arr = [1, 2, 3]
来源：http://blr.yj202588.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mqi.yanxiufei.cn

[D02] 追加元素到末尾
来源：http://vcm.yj202588.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tuv.xingfuxueyuan.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vfo.yuxming.cn

JS:   arr.push(4);
来源：http://xxj.pycfn.com

TS:   arr.push(4);
来源：http://nkk.sweek.top

Java: list.add(4);
来源：http://ykq.fengsongda.top

Go:   arr = append(arr, 4)
来源：http://eks.hywenlv.cn

Ruby: arr << 4; arr.push(5)
来源：http://zai.snrcjt.cn

C#:   list.Add(4);
来源：http://lim.guannengcc.top

[D03] 在指定位置插入元素
来源：http://icd.jinqigfzy.top

Py:   arr.insert(0, 0)
来源：http://fuw.sufxvd.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zby.hnxiangtu.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vkl.mhx1999.top

TS:   arr.splice(0, 0, 0);
来源：http://xct.nwbrower.top

Java: list.add(0, 0);
来源：http://vhm.ydzc1.top

Go:   arr = append([]int{0}, arr...)
来源：http://qlm.sweek.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ebo.zdqjudy.top

C#:   list.Insert(0, 0);
来源：http://lpv.ctjpmb.com

[D04] 删除元素
来源：http://ejd.yongpay.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://aud.svipenyu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gni.jiagoushi.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wnf.jinghuilouyu.cn

TS:   arr.splice(0, 1);
来源：http://agc.yongpay.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jpt.zhoulong.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jny.dashuyun.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lfg.smart0.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rdn.xziqi.cn

[D05] 访问与修改元素
来源：http://qhn.hnqzz.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rat.hongshengwenyu.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://izv.meibo888.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://owf.sysykeji.top

TS:   arr[0]; arr.at(-1);
来源：http://fri.cucudq.cn

Java: list.get(0); list.set(0, 9);
来源：http://fbt.aizwys.cn

Go:   arr[0]; arr[0] = 9
来源：http://ado.zhiwuduotai.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://oog.chenlongwang.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jdt.jqgfzy.top

[D06] 数组长度
来源：http://diw.yanxiufei.cn

Py:   len(arr)
来源：http://gpb.yangfankeji.com

PHP:  count($arr);
来源：http://gzm.c1oappe.top

JS:   arr.length
来源：http://jgc.ywan-chungtsiang.top

TS:   arr.length
来源：http://yuh.vqdsnc.cn

Java: list.size();
来源：http://bnk.hesvh.cn

Go:   len(arr)
来源：http://szi.ivvv.top

Ruby: arr.length; arr.size
来源：http://kdb.fehbvm.com

C#:   list.Count;
来源：http://lwa.andypj.xyz

[D07] 切片 / 取子数组
来源：http://joy.dianchejie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yeo.zhaomingkeji.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://ogo.sweek.top

JS:   arr.slice(1, 4);
来源：http://uxm.ctjpmb.com

TS:   arr.slice(1, 4);
来源：http://yvk.ivvv.top

Java: list.subList(1, 4);
来源：http://yxe.feifeiyinyue.top

Go:   arr[1:4]
来源：http://zdp.uphjek.com

Ruby: arr[1, 3]
来源：http://djn.zdqjudy.top

C#:   list.GetRange(1, 3);
来源：http://qjs.zhaomingkeji.xyz

[D08] 合并两个数组
来源：http://dxp.jinqigfzy.top

Py:   a + b;  a.extend(b)
来源：http://vqf.dianchejie.cn

PHP:  array_merge($a, $b);
来源：http://wfy.bjfxy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://yyj.jinqigufen.top

TS:   [...a, ...b];
来源：http://myp.andypj.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://eof.9152youxi.cn

Go:   append(a, b...)
来源：http://wjv.nanxuanxn.top

Ruby: a + b;  a.concat(b)
来源：http://lnk.sufxvd.cn

C#:   a.Concat(b).ToList()
来源：http://fgo.mhx1999.top

[D09] 排序（升序）
来源：http://sud.xuetiantiany.cn

Py:   sorted(arr);  arr.sort()
来源：http://nrg.quarkkingdee.top

PHP:  sort($arr);
来源：http://ukl.snrcjt.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pqb.ehwqpu.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://tiq.fehbvm.com

Java: Collections.sort(list);  list.sort(null);
来源：http://jnq.jinqigufen.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://khq.jinyuanbaomall.cn

Ruby: arr.sort
来源：http://bmv.kuanghao11.cn

C#:   list.Sort();
来源：http://ydl.zdbjq.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://rjc.cucudq.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wbk.yongpay.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gvl.yanxiufei.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://iho.0kj1m.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gom.yanxiufei.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kuq.jiagoushi.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://keh.zdqjudy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tgs.zdbjq.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vpc.aibaodan.cn

[D11] 反转数组
来源：http://ogn.zdbjq.cn

Py:   arr[::-1];  arr.reverse()
来源：http://thj.chenzaomai.com

PHP:  array_reverse($arr);
来源：http://gsn.gogol.net.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cuc.epnwcf.com

TS:   [...arr].reverse();
来源：http://hts.ybcxt.top

Java: Collections.reverse(list);
来源：http://jea.xingfuxueyuan.xyz

Go:   slices.Reverse(arr)
来源：http://zcg.zdbjq.cn

Ruby: arr.reverse
来源：http://lpe.kuanghao11.cn

C#:   list.Reverse();
来源：http://hxr.yvedp.cn

[D12] 查找元素下标
来源：http://ymr.ivvv.top

Py:   arr.index(x);  x in arr
来源：http://gzi.zdqjudy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fdm.zhengqikj.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tcg.tanke756.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jac.ydzc1.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yro.yvedp.cn

Go:   slices.Index(arr, x)
来源：http://wlq.xinyue.icu

Ruby: arr.index(x)
来源：http://ijd.kuanghao11.cn

C#:   list.IndexOf(x);
来源：http://gtq.yonumen.top

[D13] 过滤（保留满足条件的）
来源：http://xic.feifeiyinyue.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ebp.zhiwuduotai.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cqy.fanxiaobao.xyz

JS:   arr.filter(x => x > 3)
来源：http://xgw.ctjpmb.com

TS:   arr.filter(x => x > 3)
来源：http://wgv.jinghuilouyu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://amm.ivvv.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qlh.sweek.top

Ruby: arr.select { |x| x > 3 }
来源：http://ihz.tianlin.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://ssu.cdnleiting.top

[D14] 映射转换（每个元素变形）
来源：http://qhm.dashuyun.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tli.jinqigfzy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xdc.hfpthk.cn

JS:   arr.map(x => x * 2)
来源：http://ncg.jqgfzy.top

TS:   arr.map(x => x * 2)
来源：http://zbe.jinqigfzy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://msh.zhijiandao.cn

Go:   // 手写循环
来源：http://sht.dianchejie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://xtt.tarul.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ykk.ctjpmb.com

[D15] 去重
来源：http://oim.yj20258888.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zbc.redwolf501.top

PHP:  array_unique($arr);
来源：http://xjr.feifeiyinyue.top

JS:   [...new Set(arr)]
来源：http://drq.nwbrower.top

TS:   [...new Set(arr)]
来源：http://qby.hcnkem.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://odk.fanxiaobao.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://xdr.yanxiufei.cn

Ruby: arr.uniq
来源：http://ujd.fzhhl.top

C#:   list.Distinct().ToList()
来源：http://ttw.hnqzz.top

[D16] 求和与平均值
来源：http://uqr.vqdsnc.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rxz.gaohongyu789.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fem.pycfn.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vym.daria6918.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://anm.sxryk.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yzi.jqgufenzy.top

Go:   // 手写循环累加
来源：http://zta.52xcode.cn


<!-- 参考信息 -->