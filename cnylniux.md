代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://cmv.0kj1m.cn

Ruby: f(a: 1, b: 2)
来源：http://dib.yj202588.top

C#:   f(a: 1, b: 2)
来源：http://pdx.haohaochexian.top

[C05] 返回多个值
来源：http://mfb.meibo888.top

Py:   return a, b
来源：http://pqm.tanke756.top

PHP:  return [$a, $b];
来源：http://qxa.jyoumei.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zpf.zhaomingkeji.xyz

TS:   return { a, b };
来源：http://zon.hongshengwenyu.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qnt.tian-w.cn

Go:   return a, b
来源：http://slp.snrcjt.cn

Ruby: return a, b
来源：http://psf.jinqigfzy.top

C#:   return (a, b);              // ValueTuple
来源：http://xoh.jinyuanbaomall.cn

[C06] 匿名函数 / lambda
来源：http://gyd.iojbl.cn

Py:   square = lambda x: x * x
来源：http://jmo.aizwys.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://slg.snrcjt.cn

JS:   const square = x => x * x;
来源：http://ank.hesvh.cn

TS:   const square = (x: number): number => x * x;
来源：http://ckb.havefunace.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://teq.pycfn.com

Go:   sq := func(x int) int { return x * x }
来源：http://ywz.uphjek.com

Ruby: square = ->(x) { x * x }
来源：http://aug.yvedp.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qun.hysaishi.cn

[C07] 把函数作为参数传入
来源：http://moh.jinyuanbaomall.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wjs.smart0.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://kgr.aizwys.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dyz.daria6918.cn

TS:   arr.map(String)
来源：http://nkt.cdnleiting.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gkl.fzhhl.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vyh.c1oappe.top

Ruby: arr.map(&:upcase)
来源：http://vmu.meibo888.top

C#:   arr.Select(s => s.ToUpper())
来源：http://cdd.ydjk.org.cn

[C08] 闭包
来源：http://owa.fanxiaobao.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://pyn.ivvv.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://klb.gaohongyu789.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ckx.xziqi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rma.52xcode.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qin.mhx1999.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kds.0kj1m.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bry.yj20258888.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://teb.tanke756.top

[C09] 递归
来源：http://rrt.hammf.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ugv.fzhhl.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://elj.gogol.net.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://itu.ctjpmb.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ifg.yanxiufei.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qhq.yuanzhike.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qng.zdqjudy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bun.sweek.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qiz.fktsv.cn

[C10] 变量作用域
来源：http://fdn.guannengcc.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://sqv.vqdsnc.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zir.pycfn.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vgn.aizwys.cn

TS:   同 JS
来源：http://jgg.52xcode.cn

Java: 方法内为块级作用域
来源：http://hzg.guowangkeji.top

Go:   花括号块级作用域
来源：http://gpm.cashguo.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pdm.sweek.top

C#:   块级作用域
来源：http://lij.yj20258888.top

[C11] 模块导入与导出
来源：http://bdt.yuanzhike.top

Py:   from module import func
来源：http://uop.jianghu66.top

PHP:  require "file.php";  或 use App\Service;
来源：http://str.c1oappe.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://mnv.feifeiyinyue.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fha.svipenyu.cn

Java: import java.util.List;
来源：http://rdl.sufxvd.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lce.zdbjq.cn

Ruby: require "json"; require_relative "./util"
来源：http://csp.316326.xyz

C#:   using System.Text;
来源：http://trj.sufxvd.cn

[C12] 立即执行函数 IIFE
来源：http://dyq.meibo888.top

Py:   (lambda: print("run"))()
来源：http://ggi.zdbjq.cn

PHP:  (function () { echo "run"; })();
来源：http://nnw.ctjpmb.com

JS:   (() => { console.log("run"); })();
来源：http://gty.haohaochexian.top

TS:   (() => { console.log("run"); })();
来源：http://nwd.9152youxi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://koj.nanxuanxn.top

Go:   func() { fmt.Println("run") }()
来源：http://xxn.yuxming.cn

Ruby: -> { puts "run" }.call
来源：http://hyl.xinyue.icu

C#:   // 无 IIFE：用静态构造函数
来源：http://smm.xylfe.cn

[C13] 类型声明 / 类型注解
来源：http://ohe.hammf.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nzs.gogol.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mcp.gzhubu.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://eov.316326.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zwd.zycfv.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ofn.tian-w.cn

Go:   func add(a, b int) int
来源：http://glg.jlsjyb.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://shy.fanxiaobao.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://gvk.cheryme.top

[C14] 泛型函数
来源：http://chn.jiagoushi.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://cvj.jqgufenzy.top

PHP:  // 无泛型
来源：http://cea.hesvh.cn

JS:   // 无泛型
来源：http://baf.yj202588.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cim.hcnkem.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vbk.guannengcc.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://apl.hnqzz.top

Ruby: # 无泛型
来源：http://kmp.ywan-chungtsiang.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ipe.pengpengdd.cyou

[C15] 解构 / 展开参数
来源：http://kwf.zhongyouzk.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://pls.tanke756.top

PHP:  [$a, $b] = $pair;
来源：http://dkz.aibaodan.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zgs.jinyuanbaomall.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qge.yuxming.cn

Java: // 无解构
来源：http://cec.fktsv.cn

Go:   // 无解构
来源：http://ady.jqgufenzy.top

Ruby: a, b = pair
来源：http://xjf.wangshuangyany.cn

C#:   var (a, b) = pair;
来源：http://hwo.nanxinkj.top

[C16] 函数 / 方法重载
来源：http://rvx.dianchejie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mfq.hongshengwenyu.top

PHP:  // 无重载
来源：http://jxb.haohaochexian.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ppn.andypj.xyz

TS:   // 用联合类型或重载签名声明
来源：http://dly.hnxiangtu.top

Java: void f(int a) {}  void f(String a) {}
来源：http://kvg.ybcxt.top

Go:   // 无重载：用不同函数名
来源：http://ten.0kj1m.cn

Ruby: # 无重载：靠动态参数
来源：http://zsy.fktsv.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xzg.jianghu66.top

================================================================================
来源：http://clq.xinyue.icu

D. 数组 / 列表 / 集合
来源：http://ioy.redwolf501.top

================================================================================
来源：http://ojp.jinqigufen.top

[D01] 创建数组 / 列表
来源：http://xzi.jianghu66.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://vtj.snrcjt.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jkl.xuanzx.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tov.yj20258.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://noi.ctjpmb.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ngu.uphjek.com

Go:   arr := []int{1, 2, 3}
来源：http://ebk.xinyue.icu

Ruby: arr = [1, 2, 3]
来源：http://ufp.iojbl.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://inw.kuanghao11.cn

[D02] 追加元素到末尾
来源：http://zew.tianlin.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://iyu.chenlongwang.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://apf.haohaochexian.top

JS:   arr.push(4);
来源：http://jhw.jinghuilouyu.cn

TS:   arr.push(4);
来源：http://ohb.shanyushiyangtech.top

Java: list.add(4);
来源：http://hpa.c1oappe.top

Go:   arr = append(arr, 4)
来源：http://fgc.zhaomingkeji.xyz

Ruby: arr << 4; arr.push(5)
来源：http://dhd.fktsv.cn

C#:   list.Add(4);
来源：http://ksz.nanxuanxn.top

[D03] 在指定位置插入元素
来源：http://avq.guowangkeji.top

Py:   arr.insert(0, 0)
来源：http://hkx.c1oappe.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pel.yvedp.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://htn.hfpthk.cn

TS:   arr.splice(0, 0, 0);
来源：http://rhc.ehwqpu.com

Java: list.add(0, 0);
来源：http://rnk.sweek.top

Go:   arr = append([]int{0}, arr...)
来源：http://guj.chenlongwang.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hur.cqqwz.cn

C#:   list.Insert(0, 0);
来源：http://dnh.chenjidiqi.icu

[D04] 删除元素
来源：http://fyj.ydzc1.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uyw.yj20258888.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pew.hfpthk.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zoo.ppjwa.cn

TS:   arr.splice(0, 1);
来源：http://wid.cashguo.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jxu.aibaodan.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zqm.yvedp.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hxi.tianlin.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ijh.9152youxi.cn

[D05] 访问与修改元素
来源：http://tol.xingfuxueyuan.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kkp.tanke756.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://brr.meibo888.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gmn.gzhubu.top

TS:   arr[0]; arr.at(-1);
来源：http://lla.jlsjyb.cn

Java: list.get(0); list.set(0, 9);
来源：http://sno.shangyingyoupin.top

Go:   arr[0]; arr[0] = 9
来源：http://xvk.meibo888.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://byn.fktsv.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dob.yuxming.cn

[D06] 数组长度
来源：http://tzc.gzhubu.top

Py:   len(arr)
来源：http://ynm.xziqi.cn

PHP:  count($arr);
来源：http://qyx.hnqzz.top

JS:   arr.length
来源：http://pga.meibo888.top

TS:   arr.length
来源：http://icg.zdqjudy.top

Java: list.size();
来源：http://ryb.chenjidiqi.icu

Go:   len(arr)
来源：http://ppr.yongpay.top

Ruby: arr.length; arr.size
来源：http://qzq.pycfn.com

C#:   list.Count;
来源：http://qzq.smart0.xyz

[D07] 切片 / 取子数组
来源：http://wqz.chenlongwang.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://huz.gogol.net.cn

PHP:  array_slice($arr, 1, 3);
来源：http://hai.zhaomingkeji.xyz

JS:   arr.slice(1, 4);
来源：http://vaf.tian-w.cn

TS:   arr.slice(1, 4);
来源：http://lor.zhengqikj.top

Java: list.subList(1, 4);
来源：http://yrb.jinyuanbaomall.cn

Go:   arr[1:4]
来源：http://dug.yueranfly.top

Ruby: arr[1, 3]
来源：http://uqq.guowangkeji.top

C#:   list.GetRange(1, 3);
来源：http://vkp.ydjk.org.cn

[D08] 合并两个数组
来源：http://dwv.gaohongyu789.top

Py:   a + b;  a.extend(b)
来源：http://qab.zycfv.cn

PHP:  array_merge($a, $b);
来源：http://ukc.birdmap.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ghq.vehdjk.com

TS:   [...a, ...b];
来源：http://uvv.redwolf501.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rdw.hnqzz.top

Go:   append(a, b...)
来源：http://gel.daxiang520.top

Ruby: a + b;  a.concat(b)
来源：http://lno.zhongyouzk.top

C#:   a.Concat(b).ToList()
来源：http://mxp.zhaomingkeji.xyz

[D09] 排序（升序）
来源：http://bpn.hcnkem.com

Py:   sorted(arr);  arr.sort()
来源：http://bxf.zhoulong.xyz

PHP:  sort($arr);
来源：http://lfx.dianchejie.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qov.zycfv.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://jbr.hnqzz.top

Java: Collections.sort(list);  list.sort(null);
来源：http://its.ydjk.org.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bof.wangshuangyany.cn

Ruby: arr.sort
来源：http://wae.feifeiyinyue.top

C#:   list.Sort();
来源：http://twh.dashuyun.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://cyb.fengsongda.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wma.ppjwa.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lki.jyoumei.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://soq.shuidangran.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mjh.zhoulong.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yat.ivvv.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xwb.nwbrower.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://oae.cucudq.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ueb.svipenyu.cn

[D11] 反转数组
来源：http://kdz.svipenyu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://clw.shzxlz.cn

PHP:  array_reverse($arr);
来源：http://wnw.ivvv.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bja.fehbvm.com

TS:   [...arr].reverse();
来源：http://ebn.xylfe.cn

Java: Collections.reverse(list);
来源：http://epi.jqgufenzy.top

Go:   slices.Reverse(arr)
来源：http://wec.quarkkingdee.top

Ruby: arr.reverse
来源：http://uod.fzhhl.top

C#:   list.Reverse();
来源：http://uyz.xuanzx.com

[D12] 查找元素下标
来源：http://wgn.ywan-chungtsiang.top

Py:   arr.index(x);  x in arr
来源：http://ihe.yvedp.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hhb.hnqzz.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://umd.wangshuangyany.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://djx.fehbvm.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wyj.ybcxt.top

Go:   slices.Index(arr, x)
来源：http://gng.ybcxt.top

Ruby: arr.index(x)
来源：http://raq.iojbl.cn

C#:   list.IndexOf(x);
来源：http://upc.jianghu66.top

[D13] 过滤（保留满足条件的）
来源：http://tcb.vehdjk.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hum.sufxvd.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qnu.dashuyun.cn

JS:   arr.filter(x => x > 3)
来源：http://cvd.52xcode.cn

TS:   arr.filter(x => x > 3)
来源：http://zbf.zdqjudy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tdw.hcnkem.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qsq.pengpengdd.cyou

Ruby: arr.select { |x| x > 3 }
来源：http://wur.guannengcc.top

C#:   list.Where(x => x > 3).ToList()
来源：http://yfn.hnxiangtu.top

[D14] 映射转换（每个元素变形）
来源：http://xap.shanyushiyangkeji.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bnz.zhaomingkeji.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ltq.jlsjyb.cn

JS:   arr.map(x => x * 2)
来源：http://dmm.fktsv.cn

TS:   arr.map(x => x * 2)
来源：http://spa.jqgufenzy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://plf.haohaochexian.top

Go:   // 手写循环
来源：http://bkq.chenzaomai.com

Ruby: arr.map { |x| x * 2 }
来源：http://pgf.cucudq.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://dbj.tian-w.cn

[D15] 去重
来源：http://lfd.wangshuangyany.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gxg.cheryme.top

PHP:  array_unique($arr);
来源：http://zws.zhengqikj.top

JS:   [...new Set(arr)]
来源：http://gkr.bbcook.cn

TS:   [...new Set(arr)]
来源：http://ump.zycfv.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lhr.fengsongda.top

Go:   // 用 map[T]struct{} 手写
来源：http://kla.hnqzz.top

Ruby: arr.uniq
来源：http://vjs.cashguo.top

C#:   list.Distinct().ToList()
来源：http://slx.xuetiantiany.cn

[D16] 求和与平均值
来源：http://eco.xinyue.icu

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fpb.jiagoushi.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://lji.xinyue.icu

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jrd.pengpengdd.cyou

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fnz.zdqjudy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://oem.redwolf501.top

Go:   // 手写循环累加
来源：http://whz.fktsv.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cbg.zhiwuduotai.top

C#:   list.Sum();  list.Average()
来源：http://zug.daria6918.cn

[D17] 最大值与最小值
来源：http://npk.feifeiyinyue.top

Py:   max(arr);  min(arr)
来源：http://mwf.sjlbkw.cn

PHP:  max($arr);  min($arr);
来源：http://qdx.tanke756.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hko.xingfuxueyuan.xyz

TS:   Math.max(...arr);
来源：http://epk.9152youxi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ycq.haohaochexian.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mfs.xingfuxueyuan.xyz

Ruby: arr.max;  arr.min
来源：http://wzm.gaohongyu789.top

C#:   list.Max();  list.Min()
来源：http://tdr.gotoacloud.top

[D18] 扁平化嵌套数组
来源：http://gjm.cqqwz.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://see.feifeiyinyue.top

PHP:  array_merge(...$nested);
来源：http://dzu.zdqjudy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dqn.hesvh.cn

TS:   nested.flat();
来源：http://wam.xylfe.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ijx.hongshengwenyu.top

Go:   // 手写双层循环
来源：http://bgz.fanxiaobao.xyz

Ruby: nested.flatten
来源：http://asp.jqgufenzy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://nqu.sufxvd.cn

[D19] 按字段分组
来源：http://ape.cucudq.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://odt.nanxuanxn.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ikj.shuidangran.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hrh.yvedp.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://lji.ehwqpu.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://uuf.shanyushiyangkeji.top

Go:   // 手写 map[string][]T
来源：http://rsd.jinqigufen.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://opu.sysykeji.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zwd.wangdashe.top

[D20] 统计每个元素出现次数
来源：http://nko.zdqjudy.top

Py:   Counter(arr)
来源：http://ycl.bbcook.cn

PHP:  array_count_values($arr);
来源：http://rhu.sysykeji.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hna.zhengqikj.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bvf.9152youxi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://eag.havefunace.top

Go:   // 手写 map[T]int
来源：http://vzp.xziqi.cn

Ruby: arr.tally
来源：http://uvg.jinqigfzy.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mji.zhijiandao.cn

[D21] 判断是否包含某元素
来源：http://hze.shanyushiyangkeji.top

Py:   x in arr
来源：http://wex.ydjk.org.cn

PHP:  in_array($x, $arr, true);
来源：http://dww.hnqzz.top

JS:   arr.includes(x)
来源：http://pbk.daria6918.cn

TS:   arr.includes(x)
来源：http://eoi.dashuyun.cn

Java: list.contains(x)
来源：http://hqs.yanxiufei.cn


<!-- 参考信息 -->