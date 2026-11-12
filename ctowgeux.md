代发 wailian999

Py:   if not data: return
来源：http://dup.cashguo.top

PHP:  if (!$data) { return; }
来源：http://xsj.smart0.xyz

JS:   if (!data) return;
来源：http://oqu.zhixingplan.top

TS:   if (!data) return;
来源：http://vji.cashguo.top

Java: if (data == null) return;
来源：http://gsh.shanyushiyangtech.top

Go:   if data == nil { return }
来源：http://srj.c1oappe.top

Ruby: return if data.nil?
来源：http://pqs.chenzaomai.com

C#:   if (data == null) return;
来源：http://xms.shangyingyoupin.top

================================================================================
来源：http://sig.sufxvd.cn

C. 函数与作用域
来源：http://rhb.gogol.net.cn

================================================================================
来源：http://qan.dianchejie.cn

[C01] 定义函数
来源：http://xyx.ppjwa.cn

Py:   def add(a, b): return a + b
来源：http://xca.fktsv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rds.c1oappe.top

JS:   function add(a, b) { return a + b; }
来源：http://glj.tanke756.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://egm.hfpthk.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://koo.kuanghao11.cn

Go:   func add(a, b int) int { return a + b }
来源：http://brw.havefunace.top

Ruby: def add(a, b); a + b; end
来源：http://pau.tianlin.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wxt.tanke756.top

[C02] 默认参数
来源：http://utc.zhiwuduotai.top

Py:   def greet(name="World"): return name
来源：http://jnz.haohaochexian.top

PHP:  function greet($name = "World") { return $name; }
来源：http://rkl.hcnkem.com

JS:   function greet(name = "World") { return name; }
来源：http://wtw.yvedp.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://htm.ybcxt.top

Java: // 无默认参数：方法重载或 Optional
来源：http://aep.fzhhl.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rxm.yangfankeji.com

Ruby: def greet(name = "World") = name
来源：http://siy.daxiang520.top

C#:   string Greet(string name = "World") => name;
来源：http://qkh.epnwcf.com

[C03] 可变参数
来源：http://dop.dashuyun.cn

Py:   def total(*args): return sum(args)
来源：http://xnw.yanxiufei.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mma.gogol.net.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cec.yonumen.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://azn.yangfankeji.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://klu.zhiwuduotai.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dhl.0kj1m.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qaw.gogol.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rsj.mhx1999.top

[C04] 命名参数 / 关键字参数
来源：http://vhn.jinghuilouyu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nqn.ybcxt.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://eae.zycfv.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bmy.kuanghao11.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://swm.epnwcf.com

Java: // 无：用 Builder 模式或 record
来源：http://lql.jinqigfzy.top

Go:   // 无：用配置结构体参数
来源：http://dsy.yfazqb.com

Ruby: f(a: 1, b: 2)
来源：http://wjz.yuxming.cn

C#:   f(a: 1, b: 2)
来源：http://eqm.pengpengdd.cyou

[C05] 返回多个值
来源：http://plc.xylfe.cn

Py:   return a, b
来源：http://itw.svipenyu.cn

PHP:  return [$a, $b];
来源：http://iyi.yonumen.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://xzs.fzhhl.top

TS:   return { a, b };
来源：http://wea.pengpengdd.cyou

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zod.yvedp.cn

Go:   return a, b
来源：http://hsn.dianchejie.cn

Ruby: return a, b
来源：http://syb.yuanzhike.top

C#:   return (a, b);              // ValueTuple
来源：http://bps.wangdashe.top

[C06] 匿名函数 / lambda
来源：http://vkc.havefunace.top

Py:   square = lambda x: x * x
来源：http://yrb.sweek.top

PHP:  $square = fn($x) => $x * $x;
来源：http://btp.kuanghao11.cn

JS:   const square = x => x * x;
来源：http://fgi.shuidangran.top

TS:   const square = (x: number): number => x * x;
来源：http://xep.zhixingplan.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cai.sjlbkw.cn

Go:   sq := func(x int) int { return x * x }
来源：http://gbw.ppjwa.cn

Ruby: square = ->(x) { x * x }
来源：http://tzf.hywenlv.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fbj.tarul.cn

[C07] 把函数作为参数传入
来源：http://kns.guannengcc.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://clw.dianchejie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://qen.tianlin.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://czt.ybcxt.top

TS:   arr.map(String)
来源：http://pua.zhaomingkeji.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://btg.tian-w.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zwc.fengsongda.top

Ruby: arr.map(&:upcase)
来源：http://pux.cucudq.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://gco.316326.xyz

[C08] 闭包
来源：http://qqg.hnxiangtu.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fal.fzhhl.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ogl.gzhubu.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sdb.cdnleiting.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rmr.aibaodan.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nws.daria6918.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zkv.pengpengdd.cyou

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dxk.dianchejie.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jcn.aibaodan.cn

[C09] 递归
来源：http://osy.birdmap.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ayx.redwolf501.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://poy.tian-w.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fhs.nanxuanxn.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ppj.cucudq.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lga.nwbrower.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nli.smart0.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wmw.hesvh.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://thj.xuetiantiany.cn

[C10] 变量作用域
来源：http://ycf.hywenlv.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://uwr.sufxvd.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dks.chenjidiqi.icu

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ueo.xuanzx.com

TS:   同 JS
来源：http://bgy.yonumen.top

Java: 方法内为块级作用域
来源：http://mwt.aizwys.cn

Go:   花括号块级作用域
来源：http://fha.hcnkem.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nhy.zhiwuduotai.top

C#:   块级作用域
来源：http://qvw.52xcode.cn

[C11] 模块导入与导出
来源：http://xzz.ydjk.org.cn

Py:   from module import func
来源：http://gee.jinghuilouyu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://tab.sufxvd.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://tls.tarul.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wvj.pycfn.com

Java: import java.util.List;
来源：http://skf.zhengqikj.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vzk.316326.xyz

Ruby: require "json"; require_relative "./util"
来源：http://rud.yongpay.top

C#:   using System.Text;
来源：http://cca.jinyuanbaomall.cn

[C12] 立即执行函数 IIFE
来源：http://ghe.snrcjt.cn

Py:   (lambda: print("run"))()
来源：http://ivj.316326.xyz

PHP:  (function () { echo "run"; })();
来源：http://vwe.cheryme.top

JS:   (() => { console.log("run"); })();
来源：http://wqf.iojbl.cn

TS:   (() => { console.log("run"); })();
来源：http://bwl.yuxming.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ynt.shuidangran.top

Go:   func() { fmt.Println("run") }()
来源：http://gnj.havefunace.top

Ruby: -> { puts "run" }.call
来源：http://lgk.yueranfly.top

C#:   // 无 IIFE：用静态构造函数
来源：http://xmv.epnwcf.com

[C13] 类型声明 / 类型注解
来源：http://ffp.ehwqpu.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tiv.redwolf501.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bvl.hnqzz.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://aiw.xylfe.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cvx.jqgfzy.top

Java: int add(int a, int b) { return a + b; }
来源：http://nmr.aizwys.cn

Go:   func add(a, b int) int
来源：http://ras.chenlongwang.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://oig.pycfn.com

C#:   int Add(int a, int b) => a + b;
来源：http://evj.hfpthk.cn

[C14] 泛型函数
来源：http://bjd.jlsjyb.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zgp.jinqigufen.top

PHP:  // 无泛型
来源：http://abq.tanke756.top

JS:   // 无泛型
来源：http://hvn.52xcode.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ios.tianlin.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://upv.iojbl.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://adf.vqdsnc.cn

Ruby: # 无泛型
来源：http://sck.jqgfzy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xtw.nanxinkj.top

[C15] 解构 / 展开参数
来源：http://yqe.epnwcf.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ikm.feifeiyinyue.top

PHP:  [$a, $b] = $pair;
来源：http://qus.gaohongyu789.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zop.xylfe.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pvo.hesvh.cn

Java: // 无解构
来源：http://wdg.gotoacloud.top

Go:   // 无解构
来源：http://isb.yanxiufei.cn

Ruby: a, b = pair
来源：http://nci.zhongyouzk.top

C#:   var (a, b) = pair;
来源：http://chr.ydzc1.top

[C16] 函数 / 方法重载
来源：http://wqr.mhx1999.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cpq.snrcjt.cn

PHP:  // 无重载
来源：http://tcg.iojbl.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://bke.ppjwa.cn

TS:   // 用联合类型或重载签名声明
来源：http://xee.yuxming.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://sxo.chenlongwang.top

Go:   // 无重载：用不同函数名
来源：http://zcf.guowangkeji.top

Ruby: # 无重载：靠动态参数
来源：http://ijv.hongshengwenyu.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ieo.pycfn.com

================================================================================
来源：http://aeu.sysykeji.top

D. 数组 / 列表 / 集合
来源：http://wxi.jinyuanbaomall.cn

================================================================================
来源：http://aco.fehbvm.com

[D01] 创建数组 / 列表
来源：http://byu.cheryme.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://lmc.haohaochexian.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gng.jqgfzy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sxw.hfpthk.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bpu.yvedp.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zsm.zycfv.cn

Go:   arr := []int{1, 2, 3}
来源：http://mpn.jyoumei.cn

Ruby: arr = [1, 2, 3]
来源：http://ryz.52xcode.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qig.jqgufenzy.top

[D02] 追加元素到末尾
来源：http://jmh.fehbvm.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dir.guowangkeji.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jfb.shuidangran.top

JS:   arr.push(4);
来源：http://vvt.zdqjudy.top

TS:   arr.push(4);
来源：http://coj.cucudq.cn

Java: list.add(4);
来源：http://ewx.nwbrower.top

Go:   arr = append(arr, 4)
来源：http://tns.sweek.top

Ruby: arr << 4; arr.push(5)
来源：http://fam.sysykeji.top

C#:   list.Add(4);
来源：http://fvu.yj20258.top

[D03] 在指定位置插入元素
来源：http://ict.jianghu66.top

Py:   arr.insert(0, 0)
来源：http://okf.epnwcf.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ktw.yanxiufei.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ebg.jianghu66.top

TS:   arr.splice(0, 0, 0);
来源：http://hex.andypj.xyz

Java: list.add(0, 0);
来源：http://ifi.yanxiufei.cn

Go:   arr = append([]int{0}, arr...)
来源：http://kwk.ehwqpu.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://krp.shanyushiyangkeji.top

C#:   list.Insert(0, 0);
来源：http://mew.nanxuanxn.top

[D04] 删除元素
来源：http://nuw.cqqwz.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mpo.wangshuangyany.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://raf.jianghu66.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pmw.hammf.cn

TS:   arr.splice(0, 1);
来源：http://quq.fktsv.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://exo.hysaishi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fxd.snrcjt.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lzg.xylfe.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vrq.cheryme.top

[D05] 访问与修改元素
来源：http://uie.hcnkem.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tbi.fanxiaobao.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zdv.cashguo.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://niq.c1oappe.top

TS:   arr[0]; arr.at(-1);
来源：http://gry.daria6918.cn

Java: list.get(0); list.set(0, 9);
来源：http://cgn.epnwcf.com

Go:   arr[0]; arr[0] = 9
来源：http://lbs.sjlbkw.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ida.ywan-chungtsiang.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://meq.redwolf501.top

[D06] 数组长度
来源：http://jmv.jqgufenzy.top

Py:   len(arr)
来源：http://zkq.yongpay.top

PHP:  count($arr);
来源：http://lqy.fehbvm.com

JS:   arr.length
来源：http://edd.yj202588.top

TS:   arr.length
来源：http://szc.jinqigufen.top

Java: list.size();
来源：http://vco.sxryk.cn

Go:   len(arr)
来源：http://pjq.zhiwuduotai.top

Ruby: arr.length; arr.size
来源：http://wkz.chenzaomai.com

C#:   list.Count;
来源：http://wtu.haohaochexian.top

[D07] 切片 / 取子数组
来源：http://xtr.zhiwuduotai.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hoq.cqqwz.cn

PHP:  array_slice($arr, 1, 3);
来源：http://irh.chenjidiqi.icu

JS:   arr.slice(1, 4);
来源：http://qdj.zdbjq.cn

TS:   arr.slice(1, 4);
来源：http://mws.9152youxi.cn

Java: list.subList(1, 4);
来源：http://nrh.ywan-chungtsiang.top

Go:   arr[1:4]
来源：http://een.fanxiaobao.xyz

Ruby: arr[1, 3]
来源：http://bvn.0kj1m.cn

C#:   list.GetRange(1, 3);
来源：http://pdo.ydjk.org.cn

[D08] 合并两个数组
来源：http://bwu.xylfe.cn

Py:   a + b;  a.extend(b)
来源：http://rju.sxryk.cn

PHP:  array_merge($a, $b);
来源：http://lhq.shuidangran.top

JS:   [...a, ...b];  a.concat(b);
来源：http://rsg.jyoumei.cn

TS:   [...a, ...b];
来源：http://rge.zdqjudy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://btx.zhengqikj.top

Go:   append(a, b...)
来源：http://niw.sysykeji.top

Ruby: a + b;  a.concat(b)
来源：http://yoj.smart0.xyz

C#:   a.Concat(b).ToList()
来源：http://dnl.xziqi.cn

[D09] 排序（升序）
来源：http://ikz.ybcxt.top

Py:   sorted(arr);  arr.sort()
来源：http://cxy.snrcjt.cn

PHP:  sort($arr);
来源：http://clv.svipenyu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rpp.zycfv.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://kab.xuanzx.com

Java: Collections.sort(list);  list.sort(null);
来源：http://quv.vehdjk.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vni.snrcjt.cn

Ruby: arr.sort
来源：http://vxu.0kj1m.cn

C#:   list.Sort();
来源：http://mim.xuanzx.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://ahu.nanxuanxn.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rnc.zdbjq.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uwu.dianchejie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qcm.ctjpmb.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://txp.jqgfzy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://utx.0kj1m.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://adw.sxryk.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ewo.hammf.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://isu.svipenyu.cn

[D11] 反转数组
来源：http://was.feifeiyinyue.top

Py:   arr[::-1];  arr.reverse()
来源：http://sat.jqgufenzy.top

PHP:  array_reverse($arr);
来源：http://ksx.tianlin.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vhn.xuanzx.com

TS:   [...arr].reverse();
来源：http://jpw.daria6918.cn

Java: Collections.reverse(list);
来源：http://ith.yvedp.cn

Go:   slices.Reverse(arr)
来源：http://uue.316326.xyz

Ruby: arr.reverse
来源：http://gvt.sysykeji.top

C#:   list.Reverse();
来源：http://buu.jyoumei.cn

[D12] 查找元素下标
来源：http://cbw.daria6918.cn

Py:   arr.index(x);  x in arr
来源：http://rec.shanyushiyangtech.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://shn.redwolf501.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ldm.zhengqikj.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tov.vehdjk.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bet.52xcode.cn

Go:   slices.Index(arr, x)
来源：http://qxd.ywan-chungtsiang.top

Ruby: arr.index(x)
来源：http://cgt.zhoulong.xyz

C#:   list.IndexOf(x);
来源：http://ghw.fanxiaobao.xyz

[D13] 过滤（保留满足条件的）
来源：http://rsk.chenzaomai.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fcg.havefunace.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tnl.fehbvm.com

JS:   arr.filter(x => x > 3)
来源：http://ebb.uphjek.com

TS:   arr.filter(x => x > 3)
来源：http://uav.shanyushiyangkeji.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://uxc.shuidangran.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ffw.fanxiaobao.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://epa.xylfe.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://udh.quarkkingdee.top

[D14] 映射转换（每个元素变形）
来源：http://vrx.fanxiaobao.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kbb.fehbvm.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dhi.ivvv.top

JS:   arr.map(x => x * 2)
来源：http://otl.fktsv.cn

TS:   arr.map(x => x * 2)
来源：http://qat.dianchejie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://gfr.kuanghao11.cn

Go:   // 手写循环
来源：http://ptq.ydzc1.top

Ruby: arr.map { |x| x * 2 }
来源：http://sck.sufxvd.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qul.jinqigufen.top

[D15] 去重
来源：http://lzi.guannengcc.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rtp.hcnkem.com

PHP:  array_unique($arr);
来源：http://hvs.c1oappe.top

JS:   [...new Set(arr)]
来源：http://waf.nanxinkj.top

TS:   [...new Set(arr)]
来源：http://yjw.zhoulong.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sqx.cqqwz.cn

Go:   // 用 map[T]struct{} 手写
来源：http://jbq.yj20258.top

Ruby: arr.uniq
来源：http://bwj.sysykeji.top

C#:   list.Distinct().ToList()
来源：http://ode.nanxuanxn.top

[D16] 求和与平均值
来源：http://ynn.fengsongda.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bnt.dianchejie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://lhk.jqgufenzy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://afu.feifeiyinyue.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gho.ydjk.org.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wng.jiagoushi.top

Go:   // 手写循环累加
来源：http://pjy.yj20258888.top


<!-- 参考信息 -->