代发 wailian999

Py:   def add(a, b): return a + b
来源：http://epn.jqgfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cmb.nwbrower.top

JS:   function add(a, b) { return a + b; }
来源：http://nxt.yanxiufei.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ogr.fengsongda.top

Java: static int add(int a, int b) { return a + b; }
来源：http://bts.zhoulong.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://chl.iojbl.cn

Ruby: def add(a, b); a + b; end
来源：http://fwh.yuanzhike.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://koc.fehbvm.com

[C02] 默认参数
来源：http://wdg.zhengqikj.top

Py:   def greet(name="World"): return name
来源：http://qwu.xingfuxueyuan.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://bsp.sjlbkw.cn

JS:   function greet(name = "World") { return name; }
来源：http://pfe.xylfe.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://iax.hfpthk.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://jnf.cashguo.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gkq.aibaodan.cn

Ruby: def greet(name = "World") = name
来源：http://qap.cdnleiting.top

C#:   string Greet(string name = "World") => name;
来源：http://mbj.xylfe.cn

[C03] 可变参数
来源：http://fxt.sjlbkw.cn

Py:   def total(*args): return sum(args)
来源：http://dsf.zhoulong.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://uvm.andypj.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://byf.ywan-chungtsiang.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ajj.zhiwuduotai.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kur.52xcode.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://uts.pycfn.com

Ruby: def total(*nums); nums.sum; end
来源：http://fey.epnwcf.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hut.jinyuanbaomall.cn

[C04] 命名参数 / 关键字参数
来源：http://pgd.chenjidiqi.icu

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ptv.uphjek.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zhh.uphjek.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bpq.daria6918.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mvk.0kj1m.cn

Java: // 无：用 Builder 模式或 record
来源：http://zok.fzhhl.top

Go:   // 无：用配置结构体参数
来源：http://ihx.epnwcf.com

Ruby: f(a: 1, b: 2)
来源：http://flp.andypj.xyz

C#:   f(a: 1, b: 2)
来源：http://ohe.pycfn.com

[C05] 返回多个值
来源：http://jmv.sjlbkw.cn

Py:   return a, b
来源：http://xou.jiagoushi.top

PHP:  return [$a, $b];
来源：http://bcl.xziqi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://mbh.hywenlv.cn

TS:   return { a, b };
来源：http://mib.wangdashe.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://alu.cheryme.top

Go:   return a, b
来源：http://tbq.dashuyun.cn

Ruby: return a, b
来源：http://des.yuanzhike.top

C#:   return (a, b);              // ValueTuple
来源：http://pfp.ppjwa.cn

[C06] 匿名函数 / lambda
来源：http://jgf.ppjwa.cn

Py:   square = lambda x: x * x
来源：http://ruy.ppjwa.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://yjx.cdnleiting.top

JS:   const square = x => x * x;
来源：http://cgp.yvedp.cn

TS:   const square = (x: number): number => x * x;
来源：http://diw.jinyuanbaomall.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ydk.316326.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://kez.chenlongwang.top

Ruby: square = ->(x) { x * x }
来源：http://fbh.yueranfly.top

C#:   Func<int, int> square = x => x * x;
来源：http://kak.xziqi.cn

[C07] 把函数作为参数传入
来源：http://yty.fanxiaobao.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://joq.nanxinkj.top

PHP:  array_map("strtoupper", $arr);
来源：http://frj.fehbvm.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nik.zhengqikj.top

TS:   arr.map(String)
来源：http://dhd.zhijiandao.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mco.jinyuanbaomall.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://iob.tarul.cn

Ruby: arr.map(&:upcase)
来源：http://xmo.hammf.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wfo.cheryme.top

[C08] 闭包
来源：http://qyp.haohaochexian.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rsd.xinyue.icu

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xpj.yangfankeji.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pih.nanxuanxn.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nqb.ppjwa.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://uno.cheryme.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rjy.guowangkeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hjn.shzxlz.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uil.0kj1m.cn

[C09] 递归
来源：http://kmr.zhijiandao.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lot.vehdjk.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rlh.nanxinkj.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xol.jlsjyb.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bls.zhijiandao.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fjw.chenzaomai.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://out.tian-w.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cws.mhx1999.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qcr.zycfv.cn

[C10] 变量作用域
来源：http://wua.redwolf501.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jql.tianlin.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://khv.jinghuilouyu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xow.hywenlv.cn

TS:   同 JS
来源：http://jog.ivvv.top

Java: 方法内为块级作用域
来源：http://rcj.fengsongda.top

Go:   花括号块级作用域
来源：http://eoe.jinyuanbaomall.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fwi.jyoumei.cn

C#:   块级作用域
来源：http://fla.cqqwz.cn

[C11] 模块导入与导出
来源：http://bsr.ywan-chungtsiang.top

Py:   from module import func
来源：http://jlx.pycfn.com

PHP:  require "file.php";  或 use App\Service;
来源：http://hoo.uphjek.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://bwg.tarul.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yqo.dianchejie.cn

Java: import java.util.List;
来源：http://wmm.zhongyouzk.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tbh.hfpthk.cn

Ruby: require "json"; require_relative "./util"
来源：http://rlu.sweek.top

C#:   using System.Text;
来源：http://mtg.xylfe.cn

[C12] 立即执行函数 IIFE
来源：http://sre.kuanghao11.cn

Py:   (lambda: print("run"))()
来源：http://asx.nwbrower.top

PHP:  (function () { echo "run"; })();
来源：http://abb.yj20258888.top

JS:   (() => { console.log("run"); })();
来源：http://mzf.hywenlv.cn

TS:   (() => { console.log("run"); })();
来源：http://lhn.cqqwz.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dqi.gzhubu.top

Go:   func() { fmt.Println("run") }()
来源：http://izp.zhengqikj.top

Ruby: -> { puts "run" }.call
来源：http://pfs.zhoulong.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://jbe.shuidangran.top

[C13] 类型声明 / 类型注解
来源：http://igf.tianlin.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wcf.dashuyun.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pte.meibo888.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rfk.cdnleiting.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fvl.redwolf501.top

Java: int add(int a, int b) { return a + b; }
来源：http://akc.hcnkem.com

Go:   func add(a, b int) int
来源：http://wac.cheryme.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kzi.feifeiyinyue.top

C#:   int Add(int a, int b) => a + b;
来源：http://jyd.cqqwz.cn

[C14] 泛型函数
来源：http://wiv.yonumen.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zqr.ydzc1.top

PHP:  // 无泛型
来源：http://xfb.cucudq.cn

JS:   // 无泛型
来源：http://bvp.smart0.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://sap.c1oappe.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ohi.ydzc1.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vur.epnwcf.com

Ruby: # 无泛型
来源：http://zmm.0kj1m.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kot.ivvv.top

[C15] 解构 / 展开参数
来源：http://yzn.chenzaomai.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://laq.redwolf501.top

PHP:  [$a, $b] = $pair;
来源：http://dfe.svipenyu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ohw.sjlbkw.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wpt.sysykeji.top

Java: // 无解构
来源：http://stu.yangfankeji.com

Go:   // 无解构
来源：http://cbs.redwolf501.top

Ruby: a, b = pair
来源：http://xie.snrcjt.cn

C#:   var (a, b) = pair;
来源：http://cnu.vqdsnc.cn

[C16] 函数 / 方法重载
来源：http://let.yj20258888.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://oqn.ctjpmb.com

PHP:  // 无重载
来源：http://hzy.yanxiufei.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://cuw.fktsv.cn

TS:   // 用联合类型或重载签名声明
来源：http://zxq.9152youxi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://azi.zhoulong.xyz

Go:   // 无重载：用不同函数名
来源：http://yqm.zycfv.cn

Ruby: # 无重载：靠动态参数
来源：http://jbi.hfpthk.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://pem.chenzaomai.com

================================================================================
来源：http://gyv.zdqjudy.top

D. 数组 / 列表 / 集合
来源：http://srx.xingfuxueyuan.xyz

================================================================================
来源：http://fra.bbcook.cn

[D01] 创建数组 / 列表
来源：http://krl.52xcode.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://dsb.aibaodan.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hnm.zhaomingkeji.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ubn.zhaomingkeji.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://upm.xuetiantiany.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mkr.cqqwz.cn

Go:   arr := []int{1, 2, 3}
来源：http://fti.ivvv.top

Ruby: arr = [1, 2, 3]
来源：http://tea.fanxiaobao.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yeb.xingfuxueyuan.xyz

[D02] 追加元素到末尾
来源：http://aqd.ehwqpu.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mae.hnxiangtu.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://anx.tianlin.xyz

JS:   arr.push(4);
来源：http://ydq.yj20258.top

TS:   arr.push(4);
来源：http://lby.sxryk.cn

Java: list.add(4);
来源：http://rjz.hnxiangtu.top

Go:   arr = append(arr, 4)
来源：http://wbm.yj20258888.top

Ruby: arr << 4; arr.push(5)
来源：http://kxh.zhoulong.xyz

C#:   list.Add(4);
来源：http://xss.jinqigufen.top

[D03] 在指定位置插入元素
来源：http://idm.jiagoushi.top

Py:   arr.insert(0, 0)
来源：http://oot.zdbjq.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://aqw.pycfn.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rnp.daria6918.cn

TS:   arr.splice(0, 0, 0);
来源：http://ngv.xinyue.icu

Java: list.add(0, 0);
来源：http://vuk.ydjk.org.cn

Go:   arr = append([]int{0}, arr...)
来源：http://gtl.zycfv.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://azb.quarkkingdee.top

C#:   list.Insert(0, 0);
来源：http://umo.xziqi.cn

[D04] 删除元素
来源：http://tky.shanyushiyangkeji.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://npk.ydzc1.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ddz.yj202588.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tev.daxiang520.top

TS:   arr.splice(0, 1);
来源：http://fkm.yanxiufei.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ztv.ehwqpu.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rob.aizwys.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bbs.shanyushiyangkeji.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://aec.pycfn.com

[D05] 访问与修改元素
来源：http://oos.bbcook.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yqf.chenjidiqi.icu

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nli.jqgfzy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://duq.zhixingplan.top

TS:   arr[0]; arr.at(-1);
来源：http://whi.uphjek.com

Java: list.get(0); list.set(0, 9);
来源：http://ehe.cqqwz.cn

Go:   arr[0]; arr[0] = 9
来源：http://paz.hongshengwenyu.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hvw.hongshengwenyu.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://skb.jiagoushi.top

[D06] 数组长度
来源：http://zjw.316326.xyz

Py:   len(arr)
来源：http://fcv.yj20258888.top

PHP:  count($arr);
来源：http://hlp.ctjpmb.com

JS:   arr.length
来源：http://bza.gotoacloud.top

TS:   arr.length
来源：http://jev.jinghuilouyu.cn

Java: list.size();
来源：http://emp.chenzaomai.com

Go:   len(arr)
来源：http://jgp.zhiwuduotai.top

Ruby: arr.length; arr.size
来源：http://etk.52xcode.cn

C#:   list.Count;
来源：http://yoz.gzhubu.top

[D07] 切片 / 取子数组
来源：http://fyr.chenlongwang.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pzh.fengsongda.top

PHP:  array_slice($arr, 1, 3);
来源：http://dbu.yj202588.top

JS:   arr.slice(1, 4);
来源：http://oeo.jinqigufen.top

TS:   arr.slice(1, 4);
来源：http://zpx.aizwys.cn

Java: list.subList(1, 4);
来源：http://pca.c1oappe.top

Go:   arr[1:4]
来源：http://ucc.svipenyu.cn

Ruby: arr[1, 3]
来源：http://rqd.nwbrower.top

C#:   list.GetRange(1, 3);
来源：http://ewk.gotoacloud.top

[D08] 合并两个数组
来源：http://zaz.vehdjk.com

Py:   a + b;  a.extend(b)
来源：http://bpf.fktsv.cn

PHP:  array_merge($a, $b);
来源：http://kwm.yangfankeji.com

JS:   [...a, ...b];  a.concat(b);
来源：http://cbw.dashuyun.cn

TS:   [...a, ...b];
来源：http://kjk.snrcjt.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dfk.sweek.top

Go:   append(a, b...)
来源：http://sqr.vehdjk.com

Ruby: a + b;  a.concat(b)
来源：http://nha.sufxvd.cn

C#:   a.Concat(b).ToList()
来源：http://tps.hcnkem.com

[D09] 排序（升序）
来源：http://sro.52xcode.cn

Py:   sorted(arr);  arr.sort()
来源：http://qpy.tanke756.top

PHP:  sort($arr);
来源：http://csn.shanyushiyangkeji.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rhl.yanxiufei.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://frc.zhaomingkeji.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://mtl.zhiwuduotai.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bxl.fzhhl.top

Ruby: arr.sort
来源：http://iav.daxiang520.top

C#:   list.Sort();
来源：http://mjy.bbcook.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://pvz.chenlongwang.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ith.zhengqikj.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://api.xziqi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qql.jqgufenzy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gqg.meibo888.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zqq.ydzc1.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sto.xziqi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://iii.hnqzz.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://smb.ehwqpu.com

[D11] 反转数组
来源：http://sdy.jyoumei.cn

Py:   arr[::-1];  arr.reverse()
来源：http://rte.fzhhl.top

PHP:  array_reverse($arr);
来源：http://heq.ydzc1.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ouz.hywenlv.cn

TS:   [...arr].reverse();
来源：http://uac.yj202588.top

Java: Collections.reverse(list);
来源：http://sns.jiagoushi.top

Go:   slices.Reverse(arr)
来源：http://ull.jqgfzy.top

Ruby: arr.reverse
来源：http://sar.zycfv.cn

C#:   list.Reverse();
来源：http://hul.chenjidiqi.icu

[D12] 查找元素下标
来源：http://uro.yuxming.cn

Py:   arr.index(x);  x in arr
来源：http://ihu.hysaishi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ddj.9152youxi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ivv.ybcxt.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rdd.aibaodan.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ypo.fanxiaobao.xyz

Go:   slices.Index(arr, x)
来源：http://zht.chenzaomai.com

Ruby: arr.index(x)
来源：http://ibo.gaohongyu789.top

C#:   list.IndexOf(x);
来源：http://mne.jlsjyb.cn

[D13] 过滤（保留满足条件的）
来源：http://irp.hfpthk.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tqm.nanxinkj.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yuc.cqqwz.cn

JS:   arr.filter(x => x > 3)
来源：http://xei.zdqjudy.top

TS:   arr.filter(x => x > 3)
来源：http://nvk.fengsongda.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nfq.jinqigfzy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://soo.0kj1m.cn

Ruby: arr.select { |x| x > 3 }
来源：http://kah.yonumen.top

C#:   list.Where(x => x > 3).ToList()
来源：http://pxi.wangshuangyany.cn

[D14] 映射转换（每个元素变形）
来源：http://qlz.yanxiufei.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nbt.shanyushiyangtech.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bhb.yueranfly.top

JS:   arr.map(x => x * 2)
来源：http://bsf.shuidangran.top

TS:   arr.map(x => x * 2)
来源：http://jks.jinyuanbaomall.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://lhr.gzhubu.top

Go:   // 手写循环
来源：http://csk.zycfv.cn

Ruby: arr.map { |x| x * 2 }
来源：http://lef.yueranfly.top

C#:   list.Select(x => x * 2).ToList()
来源：http://yev.andypj.xyz

[D15] 去重
来源：http://zbv.cheryme.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rth.andypj.xyz

PHP:  array_unique($arr);
来源：http://bhl.hfpthk.cn

JS:   [...new Set(arr)]
来源：http://awf.daxiang520.top

TS:   [...new Set(arr)]
来源：http://mef.zdbjq.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yku.zhiwuduotai.top

Go:   // 用 map[T]struct{} 手写
来源：http://cdu.smart0.xyz

Ruby: arr.uniq
来源：http://kih.yvedp.cn

C#:   list.Distinct().ToList()
来源：http://fzh.dashuyun.cn

[D16] 求和与平均值
来源：http://yah.316326.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://erg.jianghu66.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://oyo.sxryk.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://opd.hnxiangtu.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sif.jlsjyb.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://oag.ehwqpu.com

Go:   // 手写循环累加
来源：http://pov.zdqjudy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://drb.svipenyu.cn

C#:   list.Sum();  list.Average()
来源：http://ewc.meibo888.top

[D17] 最大值与最小值
来源：http://fiv.nanxuanxn.top

Py:   max(arr);  min(arr)
来源：http://zra.tanke756.top

PHP:  max($arr);  min($arr);
来源：http://olq.316326.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://niw.pycfn.com

TS:   Math.max(...arr);
来源：http://gvl.bbcook.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://oca.hnxiangtu.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hom.yvedp.cn

Ruby: arr.max;  arr.min
来源：http://gby.jyoumei.cn

C#:   list.Max();  list.Min()
来源：http://gkg.yuanzhike.top

[D18] 扁平化嵌套数组
来源：http://oib.chenlongwang.top


<!-- 参考信息 -->