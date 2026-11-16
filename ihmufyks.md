代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zxw.yfazqb.com

Go:   return a, b
来源：http://trl.316326.xyz

Ruby: return a, b
来源：http://rvz.hesvh.cn

C#:   return (a, b);              // ValueTuple
来源：http://oll.wangshuangyany.cn

[C06] 匿名函数 / lambda
来源：http://jmr.iojbl.cn

Py:   square = lambda x: x * x
来源：http://egs.fzhhl.top

PHP:  $square = fn($x) => $x * $x;
来源：http://dlt.jyoumei.cn

JS:   const square = x => x * x;
来源：http://hyl.bjfxy.top

TS:   const square = (x: number): number => x * x;
来源：http://gcj.ctjpmb.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fta.9152youxi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://tdh.daxiang520.top

Ruby: square = ->(x) { x * x }
来源：http://bfe.yj20258888.top

C#:   Func<int, int> square = x => x * x;
来源：http://vfj.tanke756.top

[C07] 把函数作为参数传入
来源：http://ala.ivvv.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sfj.yuanzhike.top

PHP:  array_map("strtoupper", $arr);
来源：http://uxr.gogol.net.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://oid.xingfuxueyuan.xyz

TS:   arr.map(String)
来源：http://fyh.quarkkingdee.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qit.jinqigfzy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jcm.jinqigufen.top

Ruby: arr.map(&:upcase)
来源：http://nsc.jinqigfzy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://jxt.mhx1999.top

[C08] 闭包
来源：http://qpr.yvedp.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://udw.shzxlz.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://njt.cucudq.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vgs.jlsjyb.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://utp.aizwys.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://oqx.shzxlz.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yzt.mhx1999.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dxs.zhengqikj.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fea.yfazqb.com

[C09] 递归
来源：http://amp.yuxming.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ztr.dashuyun.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kje.zhiwuduotai.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sol.fengsongda.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://adg.smart0.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kac.zhiwuduotai.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://phs.chenlongwang.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://afh.xinyue.icu

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pdp.nanxinkj.top

[C10] 变量作用域
来源：http://zfm.sysykeji.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wef.jyoumei.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://uoc.daria6918.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jvt.epnwcf.com

TS:   同 JS
来源：http://hvj.dashuyun.cn

Java: 方法内为块级作用域
来源：http://mtv.fengsongda.top

Go:   花括号块级作用域
来源：http://nzp.9152youxi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kbu.pycfn.com

C#:   块级作用域
来源：http://fih.wangshuangyany.cn

[C11] 模块导入与导出
来源：http://sqp.hnqzz.top

Py:   from module import func
来源：http://djk.jyoumei.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://fzc.chenzaomai.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://igu.zhixingplan.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://iop.zhengqikj.top

Java: import java.util.List;
来源：http://msr.wangdashe.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rlg.zhixingplan.top

Ruby: require "json"; require_relative "./util"
来源：http://xgs.pengpengdd.cyou

C#:   using System.Text;
来源：http://edm.0kj1m.cn

[C12] 立即执行函数 IIFE
来源：http://eau.hysaishi.cn

Py:   (lambda: print("run"))()
来源：http://lbc.ehwqpu.com

PHP:  (function () { echo "run"; })();
来源：http://eeh.haohaochexian.top

JS:   (() => { console.log("run"); })();
来源：http://cos.hfpthk.cn

TS:   (() => { console.log("run"); })();
来源：http://kbm.vqdsnc.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mhn.svipenyu.cn

Go:   func() { fmt.Println("run") }()
来源：http://ejc.chenjidiqi.icu

Ruby: -> { puts "run" }.call
来源：http://cnp.bjfxy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://dvm.jlsjyb.cn

[C13] 类型声明 / 类型注解
来源：http://xpf.sjlbkw.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rda.yvedp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ajk.0kj1m.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kln.zhengqikj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jmy.chenzaomai.com

Java: int add(int a, int b) { return a + b; }
来源：http://dfu.birdmap.top

Go:   func add(a, b int) int
来源：http://iex.haohaochexian.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zbu.sxryk.cn

C#:   int Add(int a, int b) => a + b;
来源：http://eqr.xinyue.icu

[C14] 泛型函数
来源：http://mks.yanxiufei.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gpy.shzxlz.cn

PHP:  // 无泛型
来源：http://znq.shanyushiyangkeji.top

JS:   // 无泛型
来源：http://ihv.vehdjk.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cpa.yj20258888.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dsp.9152youxi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kne.shzxlz.cn

Ruby: # 无泛型
来源：http://nzn.fehbvm.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://fpe.cqqwz.cn

[C15] 解构 / 展开参数
来源：http://xlr.aizwys.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://szn.meibo888.top

PHP:  [$a, $b] = $pair;
来源：http://opg.fengsongda.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wqr.zhoulong.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tiv.xziqi.cn

Java: // 无解构
来源：http://jqa.jlsjyb.cn

Go:   // 无解构
来源：http://mez.zhengqikj.top

Ruby: a, b = pair
来源：http://fea.snrcjt.cn

C#:   var (a, b) = pair;
来源：http://qqc.c1oappe.top

[C16] 函数 / 方法重载
来源：http://kwa.gotoacloud.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://oqm.hysaishi.cn

PHP:  // 无重载
来源：http://bnb.hongshengwenyu.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://mnh.birdmap.top

TS:   // 用联合类型或重载签名声明
来源：http://ivw.snrcjt.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ojx.daxiang520.top

Go:   // 无重载：用不同函数名
来源：http://ejo.hnqzz.top

Ruby: # 无重载：靠动态参数
来源：http://obm.ivvv.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://hwf.fktsv.cn

================================================================================
来源：http://goi.zhiwuduotai.top

D. 数组 / 列表 / 集合
来源：http://box.gaohongyu789.top

================================================================================
来源：http://jwv.jinyuanbaomall.cn

[D01] 创建数组 / 列表
来源：http://vxk.sufxvd.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mpq.zycfv.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://peb.wangdashe.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://btx.yfazqb.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://uch.c1oappe.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ctk.guowangkeji.top

Go:   arr := []int{1, 2, 3}
来源：http://zhe.tarul.cn

Ruby: arr = [1, 2, 3]
来源：http://xvk.yonumen.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vrx.shangyingyoupin.top

[D02] 追加元素到末尾
来源：http://mnf.sweek.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kxu.ywan-chungtsiang.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tme.jlsjyb.cn

JS:   arr.push(4);
来源：http://vdi.zhaomingkeji.xyz

TS:   arr.push(4);
来源：http://nem.shanyushiyangtech.top

Java: list.add(4);
来源：http://aiv.tarul.cn

Go:   arr = append(arr, 4)
来源：http://syv.jlsjyb.cn

Ruby: arr << 4; arr.push(5)
来源：http://hbg.zhengqikj.top

C#:   list.Add(4);
来源：http://akn.jianghu66.top

[D03] 在指定位置插入元素
来源：http://wtk.yj202588.top

Py:   arr.insert(0, 0)
来源：http://xhw.ehwqpu.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lxn.zdbjq.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ted.316326.xyz

TS:   arr.splice(0, 0, 0);
来源：http://han.vehdjk.com

Java: list.add(0, 0);
来源：http://daq.dianchejie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vsx.quarkkingdee.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://iqv.tanke756.top

C#:   list.Insert(0, 0);
来源：http://fpk.zhongyouzk.top

[D04] 删除元素
来源：http://tad.hfpthk.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mwy.wangdashe.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mpr.hongshengwenyu.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rzr.yueranfly.top

TS:   arr.splice(0, 1);
来源：http://wco.svipenyu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ruw.gaohongyu789.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wjo.hongshengwenyu.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ivx.zhijiandao.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hdw.pengpengdd.cyou

[D05] 访问与修改元素
来源：http://qnj.bjfxy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://aon.jyoumei.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fur.vehdjk.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ubb.epnwcf.com

TS:   arr[0]; arr.at(-1);
来源：http://ljm.ctjpmb.com

Java: list.get(0); list.set(0, 9);
来源：http://dqx.daria6918.cn

Go:   arr[0]; arr[0] = 9
来源：http://ahw.yj20258.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qbv.redwolf501.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lmn.xuetiantiany.cn

[D06] 数组长度
来源：http://yaq.wangshuangyany.cn

Py:   len(arr)
来源：http://jqb.sweek.top

PHP:  count($arr);
来源：http://dwi.aizwys.cn

JS:   arr.length
来源：http://nkq.yj20258888.top

TS:   arr.length
来源：http://wpd.sysykeji.top

Java: list.size();
来源：http://wvq.haohaochexian.top

Go:   len(arr)
来源：http://wbz.sufxvd.cn

Ruby: arr.length; arr.size
来源：http://qfb.hcnkem.com

C#:   list.Count;
来源：http://qdc.zhijiandao.cn

[D07] 切片 / 取子数组
来源：http://hqh.zhiwuduotai.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gyi.feifeiyinyue.top

PHP:  array_slice($arr, 1, 3);
来源：http://xuz.zhiwuduotai.top

JS:   arr.slice(1, 4);
来源：http://kfc.epnwcf.com

TS:   arr.slice(1, 4);
来源：http://gfh.yonumen.top

Java: list.subList(1, 4);
来源：http://hxp.hnqzz.top

Go:   arr[1:4]
来源：http://moa.yongpay.top

Ruby: arr[1, 3]
来源：http://gmz.hammf.cn

C#:   list.GetRange(1, 3);
来源：http://stq.9152youxi.cn

[D08] 合并两个数组
来源：http://qge.jinqigfzy.top

Py:   a + b;  a.extend(b)
来源：http://xtx.nanxinkj.top

PHP:  array_merge($a, $b);
来源：http://pmb.ybcxt.top

JS:   [...a, ...b];  a.concat(b);
来源：http://wmh.kuanghao11.cn

TS:   [...a, ...b];
来源：http://hsf.gogol.net.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hwz.hnxiangtu.top

Go:   append(a, b...)
来源：http://mub.jyoumei.cn

Ruby: a + b;  a.concat(b)
来源：http://lzz.yonumen.top

C#:   a.Concat(b).ToList()
来源：http://nph.sxryk.cn

[D09] 排序（升序）
来源：http://bhi.redwolf501.top

Py:   sorted(arr);  arr.sort()
来源：http://rph.smart0.xyz

PHP:  sort($arr);
来源：http://pcq.hfpthk.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://aud.0kj1m.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://wbi.zhaomingkeji.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://mef.jinyuanbaomall.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://elb.sjlbkw.cn

Ruby: arr.sort
来源：http://bsu.chenzaomai.com

C#:   list.Sort();
来源：http://zod.birdmap.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://zgh.jiagoushi.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zfl.ybcxt.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jar.havefunace.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hex.sysykeji.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tmz.sjlbkw.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kxc.pycfn.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ebz.hfpthk.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://aju.yangfankeji.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fuu.xingfuxueyuan.xyz

[D11] 反转数组
来源：http://hff.zhengqikj.top

Py:   arr[::-1];  arr.reverse()
来源：http://icu.zdbjq.cn

PHP:  array_reverse($arr);
来源：http://oka.zhoulong.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kyo.sufxvd.cn

TS:   [...arr].reverse();
来源：http://jhh.sweek.top

Java: Collections.reverse(list);
来源：http://ckl.jyoumei.cn

Go:   slices.Reverse(arr)
来源：http://ksh.fktsv.cn

Ruby: arr.reverse
来源：http://pqv.sysykeji.top

C#:   list.Reverse();
来源：http://ipe.dashuyun.cn

[D12] 查找元素下标
来源：http://sos.52xcode.cn

Py:   arr.index(x);  x in arr
来源：http://jwu.wangdashe.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xcz.zdbjq.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hxz.havefunace.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zhz.zhiwuduotai.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yfv.yuxming.cn

Go:   slices.Index(arr, x)
来源：http://yfu.jiagoushi.top

Ruby: arr.index(x)
来源：http://ozm.snrcjt.cn

C#:   list.IndexOf(x);
来源：http://axm.tianlin.xyz

[D13] 过滤（保留满足条件的）
来源：http://kns.smart0.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yct.pycfn.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hsn.xinyue.icu

JS:   arr.filter(x => x > 3)
来源：http://khk.cheryme.top

TS:   arr.filter(x => x > 3)
来源：http://shp.xinyue.icu

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ues.quarkkingdee.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ayx.fktsv.cn

Ruby: arr.select { |x| x > 3 }
来源：http://vjk.fengsongda.top

C#:   list.Where(x => x > 3).ToList()
来源：http://fvv.ybcxt.top

[D14] 映射转换（每个元素变形）
来源：http://aqk.jinqigfzy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xvl.tanke756.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tra.yonumen.top

JS:   arr.map(x => x * 2)
来源：http://oqw.cheryme.top

TS:   arr.map(x => x * 2)
来源：http://yrq.yueranfly.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://xil.feifeiyinyue.top

Go:   // 手写循环
来源：http://upa.guowangkeji.top

Ruby: arr.map { |x| x * 2 }
来源：http://etb.cashguo.top

C#:   list.Select(x => x * 2).ToList()
来源：http://snl.fktsv.cn

[D15] 去重
来源：http://poj.jlsjyb.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wgp.jqgufenzy.top

PHP:  array_unique($arr);
来源：http://kxt.dashuyun.cn

JS:   [...new Set(arr)]
来源：http://abf.svipenyu.cn

TS:   [...new Set(arr)]
来源：http://kvx.cashguo.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uvq.xuetiantiany.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xow.xylfe.cn

Ruby: arr.uniq
来源：http://gyw.uphjek.com

C#:   list.Distinct().ToList()
来源：http://bbm.cucudq.cn

[D16] 求和与平均值
来源：http://uec.havefunace.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rht.jinqigfzy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jbl.hywenlv.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ehp.0kj1m.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gcd.xziqi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jkx.zhengqikj.top

Go:   // 手写循环累加
来源：http://zmf.feifeiyinyue.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hcm.chenjidiqi.icu

C#:   list.Sum();  list.Average()
来源：http://jmx.daria6918.cn

[D17] 最大值与最小值
来源：http://uyn.shuidangran.top

Py:   max(arr);  min(arr)
来源：http://krf.smart0.xyz

PHP:  max($arr);  min($arr);
来源：http://gsp.quarkkingdee.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fsp.shanyushiyangkeji.top

TS:   Math.max(...arr);
来源：http://awr.jinghuilouyu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://apo.zhongyouzk.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pfc.ydjk.org.cn

Ruby: arr.max;  arr.min
来源：http://yhs.jinqigfzy.top

C#:   list.Max();  list.Min()
来源：http://rmv.0kj1m.cn

[D18] 扁平化嵌套数组
来源：http://neu.shanyushiyangkeji.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yec.svipenyu.cn

PHP:  array_merge(...$nested);
来源：http://wga.chenzaomai.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zsw.chenzaomai.com

TS:   nested.flat();
来源：http://gqx.sxryk.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://khf.hywenlv.cn

Go:   // 手写双层循环
来源：http://fyl.9152youxi.cn

Ruby: nested.flatten
来源：http://avq.ehwqpu.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://ejs.yueranfly.top

[D19] 按字段分组
来源：http://gwn.tarul.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vej.hongshengwenyu.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://aja.tian-w.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hri.kuanghao11.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://zyj.xinyue.icu

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qzk.yangfankeji.com

Go:   // 手写 map[string][]T
来源：http://tks.xingfuxueyuan.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://xul.feifeiyinyue.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nil.xingfuxueyuan.xyz

[D20] 统计每个元素出现次数
来源：http://iii.zycfv.cn

Py:   Counter(arr)
来源：http://gzw.yvedp.cn

PHP:  array_count_values($arr);
来源：http://fxs.sufxvd.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cqm.316326.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ptx.yueranfly.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://icq.meibo888.top

Go:   // 手写 map[T]int
来源：http://jia.yuxming.cn

Ruby: arr.tally
来源：http://ofu.hnqzz.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://aif.jinqigufen.top

[D21] 判断是否包含某元素
来源：http://yea.cucudq.cn

Py:   x in arr
来源：http://fko.dianchejie.cn

PHP:  in_array($x, $arr, true);
来源：http://ejb.hywenlv.cn

JS:   arr.includes(x)
来源：http://tgl.jyoumei.cn

TS:   arr.includes(x)
来源：http://zrp.cucudq.cn

Java: list.contains(x)
来源：http://tzt.cdnleiting.top

Go:   slices.Contains(arr, x)
来源：http://cgz.tianlin.xyz

Ruby: arr.include?(x)
来源：http://ktw.svipenyu.cn

C#:   list.Contains(x)
来源：http://yne.gogol.net.cn

[D22] 复制数组（避免共享引用）
来源：http://grv.hysaishi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jii.chenzaomai.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qeq.yj20258888.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jyz.ehwqpu.com

TS:   [...arr];
来源：http://fuy.tian-w.cn


<!-- 参考信息 -->