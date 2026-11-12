代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://xjt.jinqigufen.top

Go:   func add(a, b int) int { return a + b }
来源：http://yyz.uphjek.com

Ruby: def add(a, b); a + b; end
来源：http://irl.zhijiandao.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vdq.tanke756.top

[C02] 默认参数
来源：http://xgb.cashguo.top

Py:   def greet(name="World"): return name
来源：http://icg.jianghu66.top

PHP:  function greet($name = "World") { return $name; }
来源：http://woz.zhengqikj.top

JS:   function greet(name = "World") { return name; }
来源：http://rzh.52xcode.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://cgj.jinyuanbaomall.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://odp.hongshengwenyu.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mku.smart0.xyz

Ruby: def greet(name = "World") = name
来源：http://ihq.wangshuangyany.cn

C#:   string Greet(string name = "World") => name;
来源：http://mve.sweek.top

[C03] 可变参数
来源：http://jcd.tanke756.top

Py:   def total(*args): return sum(args)
来源：http://cbh.yueranfly.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jnz.ybcxt.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rdx.yangfankeji.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dep.hysaishi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://csd.meibo888.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vyd.hesvh.cn

Ruby: def total(*nums); nums.sum; end
来源：http://gzl.andypj.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ril.dashuyun.cn

[C04] 命名参数 / 关键字参数
来源：http://sbk.chenzaomai.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rns.yvedp.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xup.meibo888.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://iyy.yj202588.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://glk.yj202588.top

Java: // 无：用 Builder 模式或 record
来源：http://kbf.yanxiufei.cn

Go:   // 无：用配置结构体参数
来源：http://oky.cdnleiting.top

Ruby: f(a: 1, b: 2)
来源：http://ndb.andypj.xyz

C#:   f(a: 1, b: 2)
来源：http://kjv.bjfxy.top

[C05] 返回多个值
来源：http://gqo.guannengcc.top

Py:   return a, b
来源：http://erw.zycfv.cn

PHP:  return [$a, $b];
来源：http://zau.yuanzhike.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://kcv.guannengcc.top

TS:   return { a, b };
来源：http://tio.jiagoushi.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://phv.aibaodan.cn

Go:   return a, b
来源：http://ucm.ydjk.org.cn

Ruby: return a, b
来源：http://hwi.jinyuanbaomall.cn

C#:   return (a, b);              // ValueTuple
来源：http://qdv.jinqigufen.top

[C06] 匿名函数 / lambda
来源：http://gkf.aizwys.cn

Py:   square = lambda x: x * x
来源：http://nya.hnqzz.top

PHP:  $square = fn($x) => $x * $x;
来源：http://csq.ybcxt.top

JS:   const square = x => x * x;
来源：http://avb.sjlbkw.cn

TS:   const square = (x: number): number => x * x;
来源：http://ipk.dashuyun.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wnw.quarkkingdee.top

Go:   sq := func(x int) int { return x * x }
来源：http://mps.9152youxi.cn

Ruby: square = ->(x) { x * x }
来源：http://vzc.tanke756.top

C#:   Func<int, int> square = x => x * x;
来源：http://tct.cucudq.cn

[C07] 把函数作为参数传入
来源：http://eub.sysykeji.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fmv.hongshengwenyu.top

PHP:  array_map("strtoupper", $arr);
来源：http://axj.epnwcf.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xbm.9152youxi.cn

TS:   arr.map(String)
来源：http://wrr.gotoacloud.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ptt.shzxlz.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cee.quarkkingdee.top

Ruby: arr.map(&:upcase)
来源：http://oiy.sxryk.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://lrm.jlsjyb.cn

[C08] 闭包
来源：http://jvw.zdqjudy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://btd.dashuyun.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://axd.chenjidiqi.icu

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pva.nanxuanxn.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://aqw.ehwqpu.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://caf.gotoacloud.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://aqh.ydjk.org.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xte.feifeiyinyue.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qre.0kj1m.cn

[C09] 递归
来源：http://dll.gogol.net.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sfn.yj20258888.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://uoz.tarul.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ykc.fengsongda.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rrz.bbcook.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://oqx.dianchejie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pzp.zhongyouzk.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://syz.yfazqb.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://iuv.jqgfzy.top

[C10] 变量作用域
来源：http://pkv.epnwcf.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bmc.jinyuanbaomall.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bfx.yj202588.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jao.yuxming.cn

TS:   同 JS
来源：http://ueu.fengsongda.top

Java: 方法内为块级作用域
来源：http://wdd.fehbvm.com

Go:   花括号块级作用域
来源：http://ktn.zhijiandao.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zpt.xingfuxueyuan.xyz

C#:   块级作用域
来源：http://afe.hfpthk.cn

[C11] 模块导入与导出
来源：http://gur.fktsv.cn

Py:   from module import func
来源：http://fft.ehwqpu.com

PHP:  require "file.php";  或 use App\Service;
来源：http://mji.jianghu66.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ipn.ppjwa.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xpp.vqdsnc.cn

Java: import java.util.List;
来源：http://knt.epnwcf.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mxx.xylfe.cn

Ruby: require "json"; require_relative "./util"
来源：http://qbx.hywenlv.cn

C#:   using System.Text;
来源：http://mvc.gotoacloud.top

[C12] 立即执行函数 IIFE
来源：http://aii.fanxiaobao.xyz

Py:   (lambda: print("run"))()
来源：http://wvo.yonumen.top

PHP:  (function () { echo "run"; })();
来源：http://vyl.andypj.xyz

JS:   (() => { console.log("run"); })();
来源：http://nzp.nwbrower.top

TS:   (() => { console.log("run"); })();
来源：http://ykg.ppjwa.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://sjr.epnwcf.com

Go:   func() { fmt.Println("run") }()
来源：http://qgs.tanke756.top

Ruby: -> { puts "run" }.call
来源：http://jgf.fengsongda.top

C#:   // 无 IIFE：用静态构造函数
来源：http://kvd.jinqigufen.top

[C13] 类型声明 / 类型注解
来源：http://ujj.pycfn.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ada.tianlin.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ocj.jiagoushi.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tgh.zycfv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uwx.tian-w.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ehf.yangfankeji.com

Go:   func add(a, b int) int
来源：http://qil.xinyue.icu

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qjq.guannengcc.top

C#:   int Add(int a, int b) => a + b;
来源：http://vbx.zhoulong.xyz

[C14] 泛型函数
来源：http://mrg.zhengqikj.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bve.tian-w.cn

PHP:  // 无泛型
来源：http://vzl.ehwqpu.com

JS:   // 无泛型
来源：http://aji.cashguo.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fzv.yuanzhike.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rcx.zhiwuduotai.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lkx.smart0.xyz

Ruby: # 无泛型
来源：http://niy.cashguo.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zdl.316326.xyz

[C15] 解构 / 展开参数
来源：http://tbc.xinyue.icu

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dcm.ctjpmb.com

PHP:  [$a, $b] = $pair;
来源：http://elv.cucudq.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yvo.9152youxi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hjf.dashuyun.cn

Java: // 无解构
来源：http://lpl.meibo888.top

Go:   // 无解构
来源：http://sgz.jyoumei.cn

Ruby: a, b = pair
来源：http://hsk.ydjk.org.cn

C#:   var (a, b) = pair;
来源：http://oxy.yj20258888.top

[C16] 函数 / 方法重载
来源：http://tmp.zhengqikj.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tnx.gotoacloud.top

PHP:  // 无重载
来源：http://kxv.fanxiaobao.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://djx.jiagoushi.top

TS:   // 用联合类型或重载签名声明
来源：http://msc.epnwcf.com

Java: void f(int a) {}  void f(String a) {}
来源：http://jnn.wangdashe.top

Go:   // 无重载：用不同函数名
来源：http://toq.guannengcc.top

Ruby: # 无重载：靠动态参数
来源：http://rbq.aibaodan.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://bob.cqqwz.cn

================================================================================
来源：http://qpj.fehbvm.com

D. 数组 / 列表 / 集合
来源：http://fxw.pycfn.com

================================================================================
来源：http://css.meibo888.top

[D01] 创建数组 / 列表
来源：http://rna.9152youxi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://cgk.52xcode.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://uxo.ppjwa.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sbl.mhx1999.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://mbs.meibo888.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sog.jqgfzy.top

Go:   arr := []int{1, 2, 3}
来源：http://rhj.fzhhl.top

Ruby: arr = [1, 2, 3]
来源：http://izv.vehdjk.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pdm.yanxiufei.cn

[D02] 追加元素到末尾
来源：http://xyv.gogol.net.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vda.guannengcc.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kfr.epnwcf.com

JS:   arr.push(4);
来源：http://afh.ppjwa.cn

TS:   arr.push(4);
来源：http://xrm.yanxiufei.cn

Java: list.add(4);
来源：http://udx.shzxlz.cn

Go:   arr = append(arr, 4)
来源：http://ekf.zhongyouzk.top

Ruby: arr << 4; arr.push(5)
来源：http://piw.hnqzz.top

C#:   list.Add(4);
来源：http://rce.zycfv.cn

[D03] 在指定位置插入元素
来源：http://lfr.sysykeji.top

Py:   arr.insert(0, 0)
来源：http://gfa.shangyingyoupin.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wji.ybcxt.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bbc.shanyushiyangkeji.top

TS:   arr.splice(0, 0, 0);
来源：http://pse.chenzaomai.com

Java: list.add(0, 0);
来源：http://fyj.cdnleiting.top

Go:   arr = append([]int{0}, arr...)
来源：http://uxi.zhixingplan.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wvl.vehdjk.com

C#:   list.Insert(0, 0);
来源：http://pdb.tanke756.top

[D04] 删除元素
来源：http://jvk.yangfankeji.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hbj.fengsongda.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jsc.hywenlv.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hvf.fzhhl.top

TS:   arr.splice(0, 1);
来源：http://fln.vqdsnc.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yip.cqqwz.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cwl.hcnkem.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://glr.vehdjk.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yzr.chenlongwang.top

[D05] 访问与修改元素
来源：http://coa.daxiang520.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ujy.yongpay.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sfj.guowangkeji.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cqw.xuetiantiany.cn

TS:   arr[0]; arr.at(-1);
来源：http://bqf.shanyushiyangtech.top

Java: list.get(0); list.set(0, 9);
来源：http://pap.feifeiyinyue.top

Go:   arr[0]; arr[0] = 9
来源：http://udm.yangfankeji.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://uhp.pengpengdd.cyou

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blx.pycfn.com

[D06] 数组长度
来源：http://ccm.fzhhl.top

Py:   len(arr)
来源：http://uiw.ehwqpu.com

PHP:  count($arr);
来源：http://naa.kuanghao11.cn

JS:   arr.length
来源：http://ezi.cdnleiting.top

TS:   arr.length
来源：http://wgc.tarul.cn

Java: list.size();
来源：http://dbu.fehbvm.com

Go:   len(arr)
来源：http://aah.tanke756.top

Ruby: arr.length; arr.size
来源：http://yaq.iojbl.cn

C#:   list.Count;
来源：http://sjw.wangdashe.top

[D07] 切片 / 取子数组
来源：http://bqz.jqgfzy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mxu.pengpengdd.cyou

PHP:  array_slice($arr, 1, 3);
来源：http://pfn.daxiang520.top

JS:   arr.slice(1, 4);
来源：http://uhe.zdqjudy.top

TS:   arr.slice(1, 4);
来源：http://kpg.svipenyu.cn

Java: list.subList(1, 4);
来源：http://zjo.chenzaomai.com

Go:   arr[1:4]
来源：http://oyv.nanxuanxn.top

Ruby: arr[1, 3]
来源：http://pqp.pengpengdd.cyou

C#:   list.GetRange(1, 3);
来源：http://yyt.hesvh.cn

[D08] 合并两个数组
来源：http://spv.jinqigufen.top

Py:   a + b;  a.extend(b)
来源：http://xcg.haohaochexian.top

PHP:  array_merge($a, $b);
来源：http://paw.xuetiantiany.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://sje.zycfv.cn

TS:   [...a, ...b];
来源：http://hui.jinqigufen.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qwe.smart0.xyz

Go:   append(a, b...)
来源：http://euu.nanxuanxn.top

Ruby: a + b;  a.concat(b)
来源：http://dru.fzhhl.top

C#:   a.Concat(b).ToList()
来源：http://plw.ppjwa.cn

[D09] 排序（升序）
来源：http://kvs.zhongyouzk.top

Py:   sorted(arr);  arr.sort()
来源：http://fan.fktsv.cn

PHP:  sort($arr);
来源：http://vhl.zhixingplan.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ghg.zhoulong.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://bvc.sweek.top

Java: Collections.sort(list);  list.sort(null);
来源：http://rqx.hongshengwenyu.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tth.jlsjyb.cn

Ruby: arr.sort
来源：http://fxv.gaohongyu789.top

C#:   list.Sort();
来源：http://esf.ivvv.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ido.yj20258.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://msv.zdqjudy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mca.fktsv.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://chf.feifeiyinyue.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://udg.yvedp.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jvx.shangyingyoupin.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lnh.shanyushiyangkeji.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jyg.yangfankeji.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cxh.guannengcc.top

[D11] 反转数组
来源：http://qdd.cucudq.cn

Py:   arr[::-1];  arr.reverse()
来源：http://rxr.vehdjk.com

PHP:  array_reverse($arr);
来源：http://arx.zhoulong.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ylf.shanyushiyangkeji.top

TS:   [...arr].reverse();
来源：http://sdr.andypj.xyz

Java: Collections.reverse(list);
来源：http://zgn.yongpay.top

Go:   slices.Reverse(arr)
来源：http://myg.jlsjyb.cn

Ruby: arr.reverse
来源：http://jtr.uphjek.com

C#:   list.Reverse();
来源：http://cpl.zhijiandao.cn

[D12] 查找元素下标
来源：http://hbc.shanyushiyangkeji.top

Py:   arr.index(x);  x in arr
来源：http://qys.hnqzz.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ete.yongpay.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mpa.cqqwz.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mrh.iojbl.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vpe.chenjidiqi.icu

Go:   slices.Index(arr, x)
来源：http://usf.hywenlv.cn

Ruby: arr.index(x)
来源：http://com.chenlongwang.top

C#:   list.IndexOf(x);
来源：http://dmy.yvedp.cn

[D13] 过滤（保留满足条件的）
来源：http://bmw.hcnkem.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vyq.yonumen.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://swn.yonumen.top

JS:   arr.filter(x => x > 3)
来源：http://dmg.52xcode.cn

TS:   arr.filter(x => x > 3)
来源：http://tbi.bbcook.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://eve.bbcook.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pti.hongshengwenyu.top

Ruby: arr.select { |x| x > 3 }
来源：http://sfz.zycfv.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://eul.andypj.xyz

[D14] 映射转换（每个元素变形）
来源：http://baf.epnwcf.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jpi.andypj.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qua.snrcjt.cn

JS:   arr.map(x => x * 2)
来源：http://who.feifeiyinyue.top

TS:   arr.map(x => x * 2)
来源：http://xwh.zycfv.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://hhc.daria6918.cn

Go:   // 手写循环
来源：http://mvr.bbcook.cn

Ruby: arr.map { |x| x * 2 }
来源：http://wpi.zhoulong.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://kna.xuetiantiany.cn

[D15] 去重
来源：http://cqy.chenjidiqi.icu

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://twg.hammf.cn

PHP:  array_unique($arr);
来源：http://kxt.xuetiantiany.cn

JS:   [...new Set(arr)]
来源：http://zix.nanxinkj.top

TS:   [...new Set(arr)]
来源：http://hld.tarul.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://exh.xylfe.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xls.zhijiandao.cn

Ruby: arr.uniq
来源：http://jgn.nanxinkj.top

C#:   list.Distinct().ToList()
来源：http://dvb.fehbvm.com

[D16] 求和与平均值
来源：http://sff.9152youxi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://uyb.nwbrower.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ref.cashguo.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://iex.fanxiaobao.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vtn.hcnkem.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qpp.jiagoushi.top

Go:   // 手写循环累加
来源：http://mnb.xuanzx.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hhp.bbcook.cn

C#:   list.Sum();  list.Average()
来源：http://qfu.cheryme.top

[D17] 最大值与最小值
来源：http://oxu.0kj1m.cn

Py:   max(arr);  min(arr)
来源：http://nei.nanxuanxn.top

PHP:  max($arr);  min($arr);
来源：http://ahp.snrcjt.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pah.jlsjyb.cn

TS:   Math.max(...arr);
来源：http://kzk.bjfxy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://pkc.52xcode.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ypu.snrcjt.cn

Ruby: arr.max;  arr.min
来源：http://qrg.snrcjt.cn

C#:   list.Max();  list.Min()
来源：http://idi.zhixingplan.top

[D18] 扁平化嵌套数组
来源：http://gbl.shuidangran.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://uge.pycfn.com

PHP:  array_merge(...$nested);
来源：http://ucz.zycfv.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://epu.shanyushiyangkeji.top

TS:   nested.flat();
来源：http://uud.yangfankeji.com


<!-- 参考信息 -->