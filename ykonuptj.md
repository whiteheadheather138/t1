代发 wailian999

Py:   if not data: return
来源：http://wqp.sufxvd.cn

PHP:  if (!$data) { return; }
来源：http://goj.guannengcc.top

JS:   if (!data) return;
来源：http://fcj.feifeiyinyue.top

TS:   if (!data) return;
来源：http://ouu.sufxvd.cn

Java: if (data == null) return;
来源：http://kci.hammf.cn

Go:   if data == nil { return }
来源：http://igc.vehdjk.com

Ruby: return if data.nil?
来源：http://eao.jiagoushi.top

C#:   if (data == null) return;
来源：http://vph.kuanghao11.cn

================================================================================
来源：http://lly.shzxlz.cn

C. 函数与作用域
来源：http://waq.havefunace.top

================================================================================
来源：http://gax.cheryme.top

[C01] 定义函数
来源：http://xnr.zhiwuduotai.top

Py:   def add(a, b): return a + b
来源：http://tea.uphjek.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lff.feifeiyinyue.top

JS:   function add(a, b) { return a + b; }
来源：http://slb.yongpay.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://eic.zycfv.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ilm.c1oappe.top

Go:   func add(a, b int) int { return a + b }
来源：http://meu.yvedp.cn

Ruby: def add(a, b); a + b; end
来源：http://izj.xziqi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lcr.kuanghao11.cn

[C02] 默认参数
来源：http://clw.cdnleiting.top

Py:   def greet(name="World"): return name
来源：http://xlf.fanxiaobao.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://pgh.c1oappe.top

JS:   function greet(name = "World") { return name; }
来源：http://xfa.vehdjk.com

TS:   function greet(name: string = "World") { return name; }
来源：http://wyc.wangshuangyany.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ntk.chenlongwang.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pzk.zhixingplan.top

Ruby: def greet(name = "World") = name
来源：http://ftr.jqgufenzy.top

C#:   string Greet(string name = "World") => name;
来源：http://ihp.zhixingplan.top

[C03] 可变参数
来源：http://rfx.ywan-chungtsiang.top

Py:   def total(*args): return sum(args)
来源：http://uec.zdbjq.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fes.guannengcc.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vez.epnwcf.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ajt.gotoacloud.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dmw.daxiang520.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zxz.fanxiaobao.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://kyr.dianchejie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://oeu.ydzc1.top

[C04] 命名参数 / 关键字参数
来源：http://dag.pengpengdd.cyou

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sue.cdnleiting.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://drv.ybcxt.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dta.yfazqb.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dbw.hysaishi.cn

Java: // 无：用 Builder 模式或 record
来源：http://dhk.yj202588.top

Go:   // 无：用配置结构体参数
来源：http://tqb.yj202588.top

Ruby: f(a: 1, b: 2)
来源：http://ehg.shanyushiyangtech.top

C#:   f(a: 1, b: 2)
来源：http://ben.guannengcc.top

[C05] 返回多个值
来源：http://fzf.birdmap.top

Py:   return a, b
来源：http://anm.ctjpmb.com

PHP:  return [$a, $b];
来源：http://uoq.iojbl.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ucl.jqgfzy.top

TS:   return { a, b };
来源：http://bon.bbcook.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://myb.xinyue.icu

Go:   return a, b
来源：http://poy.snrcjt.cn

Ruby: return a, b
来源：http://trz.pengpengdd.cyou

C#:   return (a, b);              // ValueTuple
来源：http://frg.hesvh.cn

[C06] 匿名函数 / lambda
来源：http://rnn.gogol.net.cn

Py:   square = lambda x: x * x
来源：http://zuu.gotoacloud.top

PHP:  $square = fn($x) => $x * $x;
来源：http://bpp.yj20258888.top

JS:   const square = x => x * x;
来源：http://nqb.jiagoushi.top

TS:   const square = (x: number): number => x * x;
来源：http://fup.zhongyouzk.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tob.fzhhl.top

Go:   sq := func(x int) int { return x * x }
来源：http://ndd.xuetiantiany.cn

Ruby: square = ->(x) { x * x }
来源：http://jdx.ydzc1.top

C#:   Func<int, int> square = x => x * x;
来源：http://wtz.chenjidiqi.icu

[C07] 把函数作为参数传入
来源：http://pkg.yj20258.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://onk.yangfankeji.com

PHP:  array_map("strtoupper", $arr);
来源：http://pui.zhongyouzk.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jrb.hammf.cn

TS:   arr.map(String)
来源：http://pbd.hcnkem.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kme.hywenlv.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://foe.yanxiufei.cn

Ruby: arr.map(&:upcase)
来源：http://vxl.sysykeji.top

C#:   arr.Select(s => s.ToUpper())
来源：http://xra.52xcode.cn

[C08] 闭包
来源：http://smx.xinyue.icu

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://njb.yj20258888.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lrl.quarkkingdee.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jbl.yfazqb.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ncp.snrcjt.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qhl.yangfankeji.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qzz.quarkkingdee.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pww.hfpthk.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://btc.yonumen.top

[C09] 递归
来源：http://mng.shuidangran.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jqb.havefunace.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://loy.jinyuanbaomall.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://guj.ywan-chungtsiang.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nbk.jianghu66.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gvo.zhaomingkeji.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qkn.nanxinkj.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uht.bbcook.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hfe.hfpthk.cn

[C10] 变量作用域
来源：http://jzc.shanyushiyangkeji.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pav.sxryk.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://keb.yongpay.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wfm.jqgufenzy.top

TS:   同 JS
来源：http://stw.jqgfzy.top

Java: 方法内为块级作用域
来源：http://sdm.ydjk.org.cn

Go:   花括号块级作用域
来源：http://sdu.jinyuanbaomall.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bdh.shanyushiyangtech.top

C#:   块级作用域
来源：http://qql.chenjidiqi.icu

[C11] 模块导入与导出
来源：http://gyf.guowangkeji.top

Py:   from module import func
来源：http://vhq.chenlongwang.top

PHP:  require "file.php";  或 use App\Service;
来源：http://khc.yongpay.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://vyv.xuetiantiany.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lec.tian-w.cn

Java: import java.util.List;
来源：http://nok.chenjidiqi.icu

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://env.aizwys.cn

Ruby: require "json"; require_relative "./util"
来源：http://xsn.mhx1999.top

C#:   using System.Text;
来源：http://zfr.yangfankeji.com

[C12] 立即执行函数 IIFE
来源：http://vwj.ydzc1.top

Py:   (lambda: print("run"))()
来源：http://cri.vehdjk.com

PHP:  (function () { echo "run"; })();
来源：http://kfp.epnwcf.com

JS:   (() => { console.log("run"); })();
来源：http://fry.redwolf501.top

TS:   (() => { console.log("run"); })();
来源：http://nif.guowangkeji.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gbh.jinqigfzy.top

Go:   func() { fmt.Println("run") }()
来源：http://jha.pycfn.com

Ruby: -> { puts "run" }.call
来源：http://dhd.52xcode.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://krl.zhengqikj.top

[C13] 类型声明 / 类型注解
来源：http://ord.svipenyu.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://usm.svipenyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jxw.nanxinkj.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://udk.havefunace.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ijl.epnwcf.com

Java: int add(int a, int b) { return a + b; }
来源：http://eoa.xingfuxueyuan.xyz

Go:   func add(a, b int) int
来源：http://hxi.nanxuanxn.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://agm.hammf.cn

C#:   int Add(int a, int b) => a + b;
来源：http://nzk.ywan-chungtsiang.top

[C14] 泛型函数
来源：http://drm.316326.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gyl.jinqigfzy.top

PHP:  // 无泛型
来源：http://djw.gaohongyu789.top

JS:   // 无泛型
来源：http://cyh.jianghu66.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qpj.fktsv.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zao.yuanzhike.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vny.zhengqikj.top

Ruby: # 无泛型
来源：http://dzi.nanxinkj.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zmf.guowangkeji.top

[C15] 解构 / 展开参数
来源：http://wfl.zhongyouzk.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://otx.tanke756.top

PHP:  [$a, $b] = $pair;
来源：http://fkf.meibo888.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wyk.andypj.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://san.yangfankeji.com

Java: // 无解构
来源：http://dkd.pycfn.com

Go:   // 无解构
来源：http://aln.daxiang520.top

Ruby: a, b = pair
来源：http://bsw.jinqigfzy.top

C#:   var (a, b) = pair;
来源：http://owa.meibo888.top

[C16] 函数 / 方法重载
来源：http://iyj.sufxvd.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zsr.316326.xyz

PHP:  // 无重载
来源：http://akj.cashguo.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://pbu.yj202588.top

TS:   // 用联合类型或重载签名声明
来源：http://qxj.zhijiandao.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://pan.tianlin.xyz

Go:   // 无重载：用不同函数名
来源：http://jhv.xylfe.cn

Ruby: # 无重载：靠动态参数
来源：http://psq.yangfankeji.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://mlh.cdnleiting.top

================================================================================
来源：http://pro.iojbl.cn

D. 数组 / 列表 / 集合
来源：http://hdl.svipenyu.cn

================================================================================
来源：http://lqa.shzxlz.cn

[D01] 创建数组 / 列表
来源：http://gtz.havefunace.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://rux.andypj.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bwk.hammf.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://eun.316326.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://xxj.yueranfly.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ynw.smart0.xyz

Go:   arr := []int{1, 2, 3}
来源：http://feq.hnxiangtu.top

Ruby: arr = [1, 2, 3]
来源：http://ekl.52xcode.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://khc.ppjwa.cn

[D02] 追加元素到末尾
来源：http://mmt.fehbvm.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wpx.tanke756.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rqu.cheryme.top

JS:   arr.push(4);
来源：http://yhy.redwolf501.top

TS:   arr.push(4);
来源：http://nim.yuanzhike.top

Java: list.add(4);
来源：http://fri.iojbl.cn

Go:   arr = append(arr, 4)
来源：http://nzo.bjfxy.top

Ruby: arr << 4; arr.push(5)
来源：http://hrq.jiagoushi.top

C#:   list.Add(4);
来源：http://ask.chenzaomai.com

[D03] 在指定位置插入元素
来源：http://azq.jqgufenzy.top

Py:   arr.insert(0, 0)
来源：http://uel.sweek.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yem.hongshengwenyu.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kqg.xylfe.cn

TS:   arr.splice(0, 0, 0);
来源：http://who.hesvh.cn

Java: list.add(0, 0);
来源：http://bjx.cucudq.cn

Go:   arr = append([]int{0}, arr...)
来源：http://uah.shuidangran.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://upv.jiagoushi.top

C#:   list.Insert(0, 0);
来源：http://kvm.daria6918.cn

[D04] 删除元素
来源：http://bhn.haohaochexian.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fzk.gaohongyu789.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jsu.52xcode.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vrv.xingfuxueyuan.xyz

TS:   arr.splice(0, 1);
来源：http://bfj.zdbjq.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bgu.ybcxt.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hic.uphjek.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://clx.haohaochexian.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yrp.uphjek.com

[D05] 访问与修改元素
来源：http://vze.xinyue.icu

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yqp.ctjpmb.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://iiw.fzhhl.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ufe.cdnleiting.top

TS:   arr[0]; arr.at(-1);
来源：http://dxr.ivvv.top

Java: list.get(0); list.set(0, 9);
来源：http://sxu.bjfxy.top

Go:   arr[0]; arr[0] = 9
来源：http://iyd.ivvv.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jea.gotoacloud.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://aoe.shanyushiyangkeji.top

[D06] 数组长度
来源：http://xak.uphjek.com

Py:   len(arr)
来源：http://wlm.meibo888.top

PHP:  count($arr);
来源：http://drn.cdnleiting.top

JS:   arr.length
来源：http://kpy.jianghu66.top

TS:   arr.length
来源：http://pqa.aizwys.cn

Java: list.size();
来源：http://iex.tianlin.xyz

Go:   len(arr)
来源：http://hzs.zhongyouzk.top

Ruby: arr.length; arr.size
来源：http://xab.svipenyu.cn

C#:   list.Count;
来源：http://gvk.316326.xyz

[D07] 切片 / 取子数组
来源：http://vty.jiagoushi.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bzo.meibo888.top

PHP:  array_slice($arr, 1, 3);
来源：http://scz.shanyushiyangtech.top

JS:   arr.slice(1, 4);
来源：http://xcr.fehbvm.com

TS:   arr.slice(1, 4);
来源：http://tim.ctjpmb.com

Java: list.subList(1, 4);
来源：http://avd.andypj.xyz

Go:   arr[1:4]
来源：http://zab.tianlin.xyz

Ruby: arr[1, 3]
来源：http://gdg.gzhubu.top

C#:   list.GetRange(1, 3);
来源：http://pjl.zhixingplan.top

[D08] 合并两个数组
来源：http://gyz.fanxiaobao.xyz

Py:   a + b;  a.extend(b)
来源：http://biy.daxiang520.top

PHP:  array_merge($a, $b);
来源：http://obz.zycfv.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://fsv.tarul.cn

TS:   [...a, ...b];
来源：http://mez.xinyue.icu

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://otj.jinghuilouyu.cn

Go:   append(a, b...)
来源：http://duv.tianlin.xyz

Ruby: a + b;  a.concat(b)
来源：http://wsw.sxryk.cn

C#:   a.Concat(b).ToList()
来源：http://dws.gzhubu.top

[D09] 排序（升序）
来源：http://ust.sysykeji.top

Py:   sorted(arr);  arr.sort()
来源：http://lll.yuxming.cn

PHP:  sort($arr);
来源：http://cmy.yj20258.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bna.jinqigfzy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://vpu.shuidangran.top

Java: Collections.sort(list);  list.sort(null);
来源：http://gvu.cashguo.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zxo.hywenlv.cn

Ruby: arr.sort
来源：http://xkw.ywan-chungtsiang.top

C#:   list.Sort();
来源：http://pvl.epnwcf.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://dvr.guannengcc.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ncf.shuidangran.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mlr.c1oappe.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://onf.jlsjyb.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bag.sxryk.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pgb.zhoulong.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lbu.zdqjudy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://trr.shanyushiyangtech.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ton.hcnkem.com

[D11] 反转数组
来源：http://tgn.daria6918.cn

Py:   arr[::-1];  arr.reverse()
来源：http://dvk.shuidangran.top

PHP:  array_reverse($arr);
来源：http://pda.zhoulong.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://phh.tarul.cn

TS:   [...arr].reverse();
来源：http://adn.aibaodan.cn

Java: Collections.reverse(list);
来源：http://xmu.hongshengwenyu.top

Go:   slices.Reverse(arr)
来源：http://vvo.gaohongyu789.top

Ruby: arr.reverse
来源：http://vnj.wangshuangyany.cn

C#:   list.Reverse();
来源：http://hsf.xziqi.cn

[D12] 查找元素下标
来源：http://ieu.hywenlv.cn

Py:   arr.index(x);  x in arr
来源：http://jct.hysaishi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rli.sjlbkw.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jza.vehdjk.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zml.jlsjyb.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://udr.aizwys.cn

Go:   slices.Index(arr, x)
来源：http://thy.xuetiantiany.cn

Ruby: arr.index(x)
来源：http://vtg.xylfe.cn

C#:   list.IndexOf(x);
来源：http://qty.kuanghao11.cn

[D13] 过滤（保留满足条件的）
来源：http://ccn.tianlin.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ahu.zdqjudy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fbo.chenjidiqi.icu

JS:   arr.filter(x => x > 3)
来源：http://bmf.hammf.cn

TS:   arr.filter(x => x > 3)
来源：http://khi.sysykeji.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://reg.cashguo.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mxl.chenjidiqi.icu

Ruby: arr.select { |x| x > 3 }
来源：http://vvy.yj202588.top

C#:   list.Where(x => x > 3).ToList()
来源：http://dmo.fzhhl.top

[D14] 映射转换（每个元素变形）
来源：http://xhr.tian-w.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mea.52xcode.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nwh.9152youxi.cn

JS:   arr.map(x => x * 2)
来源：http://fcr.zhaomingkeji.xyz

TS:   arr.map(x => x * 2)
来源：http://dum.dashuyun.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://lzv.52xcode.cn

Go:   // 手写循环
来源：http://kkj.ybcxt.top

Ruby: arr.map { |x| x * 2 }
来源：http://psl.fktsv.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://wog.shanyushiyangtech.top

[D15] 去重
来源：http://evv.tian-w.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ivd.ctjpmb.com

PHP:  array_unique($arr);
来源：http://ikg.shuidangran.top

JS:   [...new Set(arr)]
来源：http://uzg.tianlin.xyz

TS:   [...new Set(arr)]
来源：http://psp.xinyue.icu

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rkj.hcnkem.com

Go:   // 用 map[T]struct{} 手写
来源：http://yqj.pycfn.com

Ruby: arr.uniq
来源：http://tcl.wangshuangyany.cn

C#:   list.Distinct().ToList()
来源：http://gjh.daria6918.cn

[D16] 求和与平均值
来源：http://azj.9152youxi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ppc.yanxiufei.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xpb.nwbrower.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ssq.dashuyun.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kox.jqgfzy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fau.fzhhl.top

Go:   // 手写循环累加
来源：http://ndy.pengpengdd.cyou


<!-- 参考信息 -->