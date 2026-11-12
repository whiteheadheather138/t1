代发 wailian999

Py:   if not data: return
来源：http://xsz.xuanzx.com

PHP:  if (!$data) { return; }
来源：http://kiz.zhijiandao.cn

JS:   if (!data) return;
来源：http://nsq.hongshengwenyu.top

TS:   if (!data) return;
来源：http://pzp.316326.xyz

Java: if (data == null) return;
来源：http://bic.guowangkeji.top

Go:   if data == nil { return }
来源：http://czn.hywenlv.cn

Ruby: return if data.nil?
来源：http://dxt.jinqigufen.top

C#:   if (data == null) return;
来源：http://vxg.meibo888.top

================================================================================
来源：http://qxc.birdmap.top

C. 函数与作用域
来源：http://sdm.yangfankeji.com

================================================================================
来源：http://ykb.yj20258888.top

[C01] 定义函数
来源：http://bkf.sxryk.cn

Py:   def add(a, b): return a + b
来源：http://vjb.ppjwa.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wva.xingfuxueyuan.xyz

JS:   function add(a, b) { return a + b; }
来源：http://foc.hesvh.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fdq.feifeiyinyue.top

Java: static int add(int a, int b) { return a + b; }
来源：http://naa.wangdashe.top

Go:   func add(a, b int) int { return a + b }
来源：http://cjz.tian-w.cn

Ruby: def add(a, b); a + b; end
来源：http://qip.hongshengwenyu.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nip.hfpthk.cn

[C02] 默认参数
来源：http://mnm.birdmap.top

Py:   def greet(name="World"): return name
来源：http://wql.redwolf501.top

PHP:  function greet($name = "World") { return $name; }
来源：http://vde.gotoacloud.top

JS:   function greet(name = "World") { return name; }
来源：http://sal.zhixingplan.top

TS:   function greet(name: string = "World") { return name; }
来源：http://cyj.chenzaomai.com

Java: // 无默认参数：方法重载或 Optional
来源：http://zcy.sweek.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://psl.mhx1999.top

Ruby: def greet(name = "World") = name
来源：http://zdm.hywenlv.cn

C#:   string Greet(string name = "World") => name;
来源：http://fpl.zdqjudy.top

[C03] 可变参数
来源：http://efe.c1oappe.top

Py:   def total(*args): return sum(args)
来源：http://rrf.wangshuangyany.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qcy.ydjk.org.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gha.jinyuanbaomall.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mvr.tanke756.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kog.hnxiangtu.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gtb.tarul.cn

Ruby: def total(*nums); nums.sum; end
来源：http://swa.gzhubu.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qwe.gotoacloud.top

[C04] 命名参数 / 关键字参数
来源：http://qjd.zhongyouzk.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fzq.yanxiufei.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mek.meibo888.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jqe.hnqzz.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vpg.fzhhl.top

Java: // 无：用 Builder 模式或 record
来源：http://drb.ppjwa.cn

Go:   // 无：用配置结构体参数
来源：http://zrm.sweek.top

Ruby: f(a: 1, b: 2)
来源：http://ihb.ppjwa.cn

C#:   f(a: 1, b: 2)
来源：http://iab.xziqi.cn

[C05] 返回多个值
来源：http://sap.pycfn.com

Py:   return a, b
来源：http://mkx.mhx1999.top

PHP:  return [$a, $b];
来源：http://mpv.tianlin.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://rxy.hywenlv.cn

TS:   return { a, b };
来源：http://vuc.ppjwa.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nsl.xziqi.cn

Go:   return a, b
来源：http://qwc.cqqwz.cn

Ruby: return a, b
来源：http://pkf.dianchejie.cn

C#:   return (a, b);              // ValueTuple
来源：http://eot.jiagoushi.top

[C06] 匿名函数 / lambda
来源：http://jxo.gzhubu.top

Py:   square = lambda x: x * x
来源：http://cfe.sweek.top

PHP:  $square = fn($x) => $x * $x;
来源：http://pod.c1oappe.top

JS:   const square = x => x * x;
来源：http://phz.haohaochexian.top

TS:   const square = (x: number): number => x * x;
来源：http://hnt.zhixingplan.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vui.shuidangran.top

Go:   sq := func(x int) int { return x * x }
来源：http://bky.haohaochexian.top

Ruby: square = ->(x) { x * x }
来源：http://xjh.yfazqb.com

C#:   Func<int, int> square = x => x * x;
来源：http://mxn.bbcook.cn

[C07] 把函数作为参数传入
来源：http://kay.xylfe.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://abl.wangdashe.top

PHP:  array_map("strtoupper", $arr);
来源：http://epl.zhixingplan.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hsx.zycfv.cn

TS:   arr.map(String)
来源：http://vgk.zhoulong.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://iag.gzhubu.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ngz.gzhubu.top

Ruby: arr.map(&:upcase)
来源：http://ddc.guannengcc.top

C#:   arr.Select(s => s.ToUpper())
来源：http://crg.wangdashe.top

[C08] 闭包
来源：http://mqi.vqdsnc.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://pcq.chenzaomai.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yxa.shzxlz.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kpf.xuanzx.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rbp.jianghu66.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lhd.zdqjudy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dlf.tarul.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fyu.meibo888.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://iew.epnwcf.com

[C09] 递归
来源：http://nwh.sjlbkw.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fts.yanxiufei.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rcf.jinghuilouyu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jno.0kj1m.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zxj.chenzaomai.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ukz.hammf.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cks.xingfuxueyuan.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://elx.ywan-chungtsiang.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xwf.fehbvm.com

[C10] 变量作用域
来源：http://cta.feifeiyinyue.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ucx.guowangkeji.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://piv.uphjek.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://etp.xziqi.cn

TS:   同 JS
来源：http://avh.andypj.xyz

Java: 方法内为块级作用域
来源：http://mvw.chenjidiqi.icu

Go:   花括号块级作用域
来源：http://pus.tianlin.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fuq.xingfuxueyuan.xyz

C#:   块级作用域
来源：http://rph.9152youxi.cn

[C11] 模块导入与导出
来源：http://sku.cucudq.cn

Py:   from module import func
来源：http://sin.shangyingyoupin.top

PHP:  require "file.php";  或 use App\Service;
来源：http://jrt.yj20258.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://xus.haohaochexian.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://izz.zhixingplan.top

Java: import java.util.List;
来源：http://ihs.pengpengdd.cyou

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ead.smart0.xyz

Ruby: require "json"; require_relative "./util"
来源：http://vdx.tarul.cn

C#:   using System.Text;
来源：http://zwl.uphjek.com

[C12] 立即执行函数 IIFE
来源：http://bcn.redwolf501.top

Py:   (lambda: print("run"))()
来源：http://mtf.andypj.xyz

PHP:  (function () { echo "run"; })();
来源：http://ktf.jqgufenzy.top

JS:   (() => { console.log("run"); })();
来源：http://ysb.jianghu66.top

TS:   (() => { console.log("run"); })();
来源：http://bxd.tanke756.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://odo.aibaodan.cn

Go:   func() { fmt.Println("run") }()
来源：http://txm.chenjidiqi.icu

Ruby: -> { puts "run" }.call
来源：http://yrk.hcnkem.com

C#:   // 无 IIFE：用静态构造函数
来源：http://apc.dianchejie.cn

[C13] 类型声明 / 类型注解
来源：http://tfb.zhaomingkeji.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dvd.guowangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ukl.cashguo.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kav.havefunace.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://osj.ehwqpu.com

Java: int add(int a, int b) { return a + b; }
来源：http://ppg.daxiang520.top

Go:   func add(a, b int) int
来源：http://xuy.cucudq.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://eay.xinyue.icu

C#:   int Add(int a, int b) => a + b;
来源：http://akk.chenjidiqi.icu

[C14] 泛型函数
来源：http://eyw.zhijiandao.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xbk.9152youxi.cn

PHP:  // 无泛型
来源：http://nbh.cqqwz.cn

JS:   // 无泛型
来源：http://ehx.xylfe.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://aay.xinyue.icu

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://prj.jinqigfzy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kfm.shzxlz.cn

Ruby: # 无泛型
来源：http://xiy.guowangkeji.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yfe.zhoulong.xyz

[C15] 解构 / 展开参数
来源：http://iuc.zhijiandao.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qgo.zhongyouzk.top

PHP:  [$a, $b] = $pair;
来源：http://pad.aibaodan.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xrb.gotoacloud.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://iql.yongpay.top

Java: // 无解构
来源：http://tej.guannengcc.top

Go:   // 无解构
来源：http://qzm.yongpay.top

Ruby: a, b = pair
来源：http://zza.snrcjt.cn

C#:   var (a, b) = pair;
来源：http://qus.tanke756.top

[C16] 函数 / 方法重载
来源：http://ifx.chenzaomai.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fwv.cashguo.top

PHP:  // 无重载
来源：http://ebn.zhijiandao.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://vgu.bjfxy.top

TS:   // 用联合类型或重载签名声明
来源：http://yss.sufxvd.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ghb.fanxiaobao.xyz

Go:   // 无重载：用不同函数名
来源：http://qut.meibo888.top

Ruby: # 无重载：靠动态参数
来源：http://dmy.sxryk.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://gkv.sysykeji.top

================================================================================
来源：http://xsl.yangfankeji.com

D. 数组 / 列表 / 集合
来源：http://mpf.hesvh.cn

================================================================================
来源：http://qfk.ppjwa.cn

[D01] 创建数组 / 列表
来源：http://zku.sjlbkw.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://bto.zhaomingkeji.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ujm.yvedp.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gqa.zhongyouzk.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://lgq.yj202588.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yrn.zhiwuduotai.top

Go:   arr := []int{1, 2, 3}
来源：http://uvj.aibaodan.cn

Ruby: arr = [1, 2, 3]
来源：http://yix.haohaochexian.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vxk.wangdashe.top

[D02] 追加元素到末尾
来源：http://cse.pycfn.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dom.aibaodan.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://npf.zhijiandao.cn

JS:   arr.push(4);
来源：http://sqq.zdbjq.cn

TS:   arr.push(4);
来源：http://mog.dashuyun.cn

Java: list.add(4);
来源：http://vlb.bbcook.cn

Go:   arr = append(arr, 4)
来源：http://mxz.vqdsnc.cn

Ruby: arr << 4; arr.push(5)
来源：http://yrn.daria6918.cn

C#:   list.Add(4);
来源：http://xha.gaohongyu789.top

[D03] 在指定位置插入元素
来源：http://dul.xziqi.cn

Py:   arr.insert(0, 0)
来源：http://xya.sxryk.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dhw.smart0.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ijz.cashguo.top

TS:   arr.splice(0, 0, 0);
来源：http://uod.snrcjt.cn

Java: list.add(0, 0);
来源：http://ean.9152youxi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://jlf.feifeiyinyue.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://edq.c1oappe.top

C#:   list.Insert(0, 0);
来源：http://mfx.smart0.xyz

[D04] 删除元素
来源：http://iyl.zhijiandao.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ker.guowangkeji.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ftu.yueranfly.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://byb.birdmap.top

TS:   arr.splice(0, 1);
来源：http://pmo.epnwcf.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fph.hammf.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ega.shanyushiyangkeji.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qnd.chenjidiqi.icu

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sls.aibaodan.cn

[D05] 访问与修改元素
来源：http://jcg.zdqjudy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qcn.zhijiandao.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xab.xinyue.icu

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ply.xziqi.cn

TS:   arr[0]; arr.at(-1);
来源：http://iov.c1oappe.top

Java: list.get(0); list.set(0, 9);
来源：http://qes.bbcook.cn

Go:   arr[0]; arr[0] = 9
来源：http://hey.sxryk.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://udn.jlsjyb.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://tlw.cdnleiting.top

[D06] 数组长度
来源：http://oeo.yj20258.top

Py:   len(arr)
来源：http://dgu.ehwqpu.com

PHP:  count($arr);
来源：http://cdz.mhx1999.top

JS:   arr.length
来源：http://fdq.uphjek.com

TS:   arr.length
来源：http://lum.ehwqpu.com

Java: list.size();
来源：http://qfz.xingfuxueyuan.xyz

Go:   len(arr)
来源：http://xby.jiagoushi.top

Ruby: arr.length; arr.size
来源：http://eba.yfazqb.com

C#:   list.Count;
来源：http://xei.zhongyouzk.top

[D07] 切片 / 取子数组
来源：http://lzn.svipenyu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://btn.epnwcf.com

PHP:  array_slice($arr, 1, 3);
来源：http://wnz.nwbrower.top

JS:   arr.slice(1, 4);
来源：http://rco.cashguo.top

TS:   arr.slice(1, 4);
来源：http://mdh.tianlin.xyz

Java: list.subList(1, 4);
来源：http://wbx.hesvh.cn

Go:   arr[1:4]
来源：http://gpa.yj20258888.top

Ruby: arr[1, 3]
来源：http://wwf.tian-w.cn

C#:   list.GetRange(1, 3);
来源：http://aqo.sufxvd.cn

[D08] 合并两个数组
来源：http://jys.havefunace.top

Py:   a + b;  a.extend(b)
来源：http://tcu.yj20258888.top

PHP:  array_merge($a, $b);
来源：http://hjb.jyoumei.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://yme.fengsongda.top

TS:   [...a, ...b];
来源：http://gyr.zhoulong.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://imt.iojbl.cn

Go:   append(a, b...)
来源：http://ggx.cucudq.cn

Ruby: a + b;  a.concat(b)
来源：http://hrg.hfpthk.cn

C#:   a.Concat(b).ToList()
来源：http://pgi.jiagoushi.top

[D09] 排序（升序）
来源：http://vue.tianlin.xyz

Py:   sorted(arr);  arr.sort()
来源：http://sta.aizwys.cn

PHP:  sort($arr);
来源：http://swp.zhengqikj.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sgc.ctjpmb.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://uoa.tianlin.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://ycq.gogol.net.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ksm.wangshuangyany.cn

Ruby: arr.sort
来源：http://fmu.jinqigufen.top

C#:   list.Sort();
来源：http://riq.epnwcf.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://wkp.jyoumei.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jpw.nwbrower.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ntd.xuetiantiany.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bls.jqgufenzy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://inq.nwbrower.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rex.0kj1m.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kky.hammf.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://aut.zhiwuduotai.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wtu.iojbl.cn

[D11] 反转数组
来源：http://hbx.wangdashe.top

Py:   arr[::-1];  arr.reverse()
来源：http://jaq.kuanghao11.cn

PHP:  array_reverse($arr);
来源：http://jbw.nwbrower.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yxn.jqgufenzy.top

TS:   [...arr].reverse();
来源：http://alp.svipenyu.cn

Java: Collections.reverse(list);
来源：http://sfk.gaohongyu789.top

Go:   slices.Reverse(arr)
来源：http://gty.wangshuangyany.cn

Ruby: arr.reverse
来源：http://tqq.dianchejie.cn

C#:   list.Reverse();
来源：http://ajn.ivvv.top

[D12] 查找元素下标
来源：http://gix.jqgufenzy.top

Py:   arr.index(x);  x in arr
来源：http://zie.yanxiufei.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gka.xylfe.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oqh.nanxuanxn.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://led.gaohongyu789.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://psz.uphjek.com

Go:   slices.Index(arr, x)
来源：http://llm.pycfn.com

Ruby: arr.index(x)
来源：http://xcn.sweek.top

C#:   list.IndexOf(x);
来源：http://ube.xuetiantiany.cn

[D13] 过滤（保留满足条件的）
来源：http://lue.chenzaomai.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kod.zhengqikj.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://svf.fehbvm.com

JS:   arr.filter(x => x > 3)
来源：http://rwd.epnwcf.com

TS:   arr.filter(x => x > 3)
来源：http://tjj.ybcxt.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wqz.vehdjk.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://utu.pycfn.com

Ruby: arr.select { |x| x > 3 }
来源：http://jat.yvedp.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qja.shanyushiyangkeji.top

[D14] 映射转换（每个元素变形）
来源：http://rlj.iojbl.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://uys.cucudq.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lpy.yfazqb.com

JS:   arr.map(x => x * 2)
来源：http://ogw.jinghuilouyu.cn

TS:   arr.map(x => x * 2)
来源：http://tog.epnwcf.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://tjg.jianghu66.top

Go:   // 手写循环
来源：http://wup.shangyingyoupin.top

Ruby: arr.map { |x| x * 2 }
来源：http://zbl.yanxiufei.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://bft.fanxiaobao.xyz

[D15] 去重
来源：http://frt.epnwcf.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tbh.yongpay.top

PHP:  array_unique($arr);
来源：http://fmr.daxiang520.top

JS:   [...new Set(arr)]
来源：http://vac.tanke756.top

TS:   [...new Set(arr)]
来源：http://ggc.guannengcc.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pzy.ydzc1.top

Go:   // 用 map[T]struct{} 手写
来源：http://gdo.sxryk.cn

Ruby: arr.uniq
来源：http://kll.zdqjudy.top

C#:   list.Distinct().ToList()
来源：http://nam.yvedp.cn

[D16] 求和与平均值
来源：http://rqr.smart0.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ldg.ehwqpu.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wcf.shangyingyoupin.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://iez.meibo888.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ifa.yvedp.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://abp.vqdsnc.cn

Go:   // 手写循环累加
来源：http://ymm.yongpay.top


<!-- 参考信息 -->