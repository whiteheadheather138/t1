代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mxd.snrcjt.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ydf.guannengcc.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wue.aizwys.cn

Java: // 无：用 Builder 模式或 record
来源：http://yez.pycfn.com

Go:   // 无：用配置结构体参数
来源：http://klj.hcnkem.com

Ruby: f(a: 1, b: 2)
来源：http://oiw.hnxiangtu.top

C#:   f(a: 1, b: 2)
来源：http://nzg.fzhhl.top

[C05] 返回多个值
来源：http://zos.birdmap.top

Py:   return a, b
来源：http://jbw.ywan-chungtsiang.top

PHP:  return [$a, $b];
来源：http://dkz.fengsongda.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://edr.fengsongda.top

TS:   return { a, b };
来源：http://sjy.fktsv.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ieu.daria6918.cn

Go:   return a, b
来源：http://ftl.pycfn.com

Ruby: return a, b
来源：http://vin.yuanzhike.top

C#:   return (a, b);              // ValueTuple
来源：http://bwb.birdmap.top

[C06] 匿名函数 / lambda
来源：http://tsz.hfpthk.cn

Py:   square = lambda x: x * x
来源：http://jdd.hammf.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://mdg.ydzc1.top

JS:   const square = x => x * x;
来源：http://ygb.hnqzz.top

TS:   const square = (x: number): number => x * x;
来源：http://hrg.aibaodan.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tbf.hnqzz.top

Go:   sq := func(x int) int { return x * x }
来源：http://eza.zhiwuduotai.top

Ruby: square = ->(x) { x * x }
来源：http://kfk.pengpengdd.cyou

C#:   Func<int, int> square = x => x * x;
来源：http://dem.9152youxi.cn

[C07] 把函数作为参数传入
来源：http://ajd.cdnleiting.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vte.haohaochexian.top

PHP:  array_map("strtoupper", $arr);
来源：http://auf.ywan-chungtsiang.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tnu.hnqzz.top

TS:   arr.map(String)
来源：http://yam.ppjwa.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rus.uphjek.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xpb.hesvh.cn

Ruby: arr.map(&:upcase)
来源：http://hdz.hongshengwenyu.top

C#:   arr.Select(s => s.ToUpper())
来源：http://mla.xuetiantiany.cn

[C08] 闭包
来源：http://vyt.chenzaomai.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://itj.chenzaomai.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://faa.ivvv.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mwx.vehdjk.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ziw.ydzc1.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tbq.zhongyouzk.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://exz.hnqzz.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vai.mhx1999.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bau.sxryk.cn

[C09] 递归
来源：http://wjv.xylfe.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pqm.9152youxi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://oqi.zhengqikj.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gjd.aizwys.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jqi.daxiang520.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kbh.yj20258.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pwo.sufxvd.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hik.hnxiangtu.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xon.guannengcc.top

[C10] 变量作用域
来源：http://hli.zhaomingkeji.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bqz.tian-w.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yhy.9152youxi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qgh.hnxiangtu.top

TS:   同 JS
来源：http://kcp.zhaomingkeji.xyz

Java: 方法内为块级作用域
来源：http://pbw.gogol.net.cn

Go:   花括号块级作用域
来源：http://fqj.zhongyouzk.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yao.yonumen.top

C#:   块级作用域
来源：http://xai.zdqjudy.top

[C11] 模块导入与导出
来源：http://gxy.sjlbkw.cn

Py:   from module import func
来源：http://zcq.zdqjudy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://uqt.quarkkingdee.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://hrz.tarul.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dzh.9152youxi.cn

Java: import java.util.List;
来源：http://vfi.yonumen.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://onh.tianlin.xyz

Ruby: require "json"; require_relative "./util"
来源：http://lvl.yuxming.cn

C#:   using System.Text;
来源：http://hgk.fzhhl.top

[C12] 立即执行函数 IIFE
来源：http://bdx.zhaomingkeji.xyz

Py:   (lambda: print("run"))()
来源：http://qpk.bjfxy.top

PHP:  (function () { echo "run"; })();
来源：http://upt.jinghuilouyu.cn

JS:   (() => { console.log("run"); })();
来源：http://kyt.dashuyun.cn

TS:   (() => { console.log("run"); })();
来源：http://zpu.aibaodan.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wpc.kuanghao11.cn

Go:   func() { fmt.Println("run") }()
来源：http://agy.pycfn.com

Ruby: -> { puts "run" }.call
来源：http://hlt.ehwqpu.com

C#:   // 无 IIFE：用静态构造函数
来源：http://heo.wangshuangyany.cn

[C13] 类型声明 / 类型注解
来源：http://dqp.yj20258.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hlg.xinyue.icu

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://toh.guannengcc.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cbz.ehwqpu.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jpn.jqgufenzy.top

Java: int add(int a, int b) { return a + b; }
来源：http://gys.ivvv.top

Go:   func add(a, b int) int
来源：http://kdy.redwolf501.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://uot.nanxinkj.top

C#:   int Add(int a, int b) => a + b;
来源：http://msr.andypj.xyz

[C14] 泛型函数
来源：http://ymt.jyoumei.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ieu.jinqigufen.top

PHP:  // 无泛型
来源：http://aqn.zdbjq.cn

JS:   // 无泛型
来源：http://mde.xuanzx.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rff.jyoumei.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://txq.0kj1m.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://etr.hcnkem.com

Ruby: # 无泛型
来源：http://bqk.zhixingplan.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rll.jianghu66.top

[C15] 解构 / 展开参数
来源：http://jxs.hammf.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yok.cashguo.top

PHP:  [$a, $b] = $pair;
来源：http://mtd.jqgufenzy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fvk.jinyuanbaomall.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xxb.shzxlz.cn

Java: // 无解构
来源：http://vcl.jlsjyb.cn

Go:   // 无解构
来源：http://eff.jinqigfzy.top

Ruby: a, b = pair
来源：http://rvf.jlsjyb.cn

C#:   var (a, b) = pair;
来源：http://shu.xingfuxueyuan.xyz

[C16] 函数 / 方法重载
来源：http://ggv.bbcook.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://buv.jlsjyb.cn

PHP:  // 无重载
来源：http://pwh.vehdjk.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://cez.zhengqikj.top

TS:   // 用联合类型或重载签名声明
来源：http://hvn.yj202588.top

Java: void f(int a) {}  void f(String a) {}
来源：http://kni.shuidangran.top

Go:   // 无重载：用不同函数名
来源：http://zlh.daxiang520.top

Ruby: # 无重载：靠动态参数
来源：http://mus.andypj.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://obz.316326.xyz

================================================================================
来源：http://vxt.zhengqikj.top

D. 数组 / 列表 / 集合
来源：http://tza.hammf.cn

================================================================================
来源：http://uyh.aibaodan.cn

[D01] 创建数组 / 列表
来源：http://ygd.cqqwz.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://wza.sxryk.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://war.daxiang520.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zfd.zdqjudy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://gtu.ywan-chungtsiang.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sko.andypj.xyz

Go:   arr := []int{1, 2, 3}
来源：http://nzo.chenzaomai.com

Ruby: arr = [1, 2, 3]
来源：http://maa.jiagoushi.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://heh.cqqwz.cn

[D02] 追加元素到末尾
来源：http://dsr.cdnleiting.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://art.sufxvd.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cln.yonumen.top

JS:   arr.push(4);
来源：http://ses.xingfuxueyuan.xyz

TS:   arr.push(4);
来源：http://uez.pengpengdd.cyou

Java: list.add(4);
来源：http://lco.meibo888.top

Go:   arr = append(arr, 4)
来源：http://wfu.vqdsnc.cn

Ruby: arr << 4; arr.push(5)
来源：http://qjc.hfpthk.cn

C#:   list.Add(4);
来源：http://vma.shanyushiyangkeji.top

[D03] 在指定位置插入元素
来源：http://tnr.yj20258.top

Py:   arr.insert(0, 0)
来源：http://eci.fehbvm.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tba.zhaomingkeji.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wib.tarul.cn

TS:   arr.splice(0, 0, 0);
来源：http://mpr.ehwqpu.com

Java: list.add(0, 0);
来源：http://tme.tian-w.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ayr.ydzc1.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kjn.gaohongyu789.top

C#:   list.Insert(0, 0);
来源：http://slu.9152youxi.cn

[D04] 删除元素
来源：http://hjl.yj202588.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mne.fehbvm.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ghb.guannengcc.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ztg.sufxvd.cn

TS:   arr.splice(0, 1);
来源：http://tsz.smart0.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://khy.c1oappe.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jqp.fanxiaobao.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dzn.yangfankeji.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pnc.shanyushiyangtech.top

[D05] 访问与修改元素
来源：http://eyt.hfpthk.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://esx.hywenlv.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yzz.zhijiandao.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mdk.hywenlv.cn

TS:   arr[0]; arr.at(-1);
来源：http://ilw.zhixingplan.top

Java: list.get(0); list.set(0, 9);
来源：http://wpj.pengpengdd.cyou

Go:   arr[0]; arr[0] = 9
来源：http://bpc.gotoacloud.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fkj.feifeiyinyue.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kjn.yonumen.top

[D06] 数组长度
来源：http://rla.hfpthk.cn

Py:   len(arr)
来源：http://yhg.jiagoushi.top

PHP:  count($arr);
来源：http://ycw.tian-w.cn

JS:   arr.length
来源：http://aop.ctjpmb.com

TS:   arr.length
来源：http://mas.guannengcc.top

Java: list.size();
来源：http://zfh.zdbjq.cn

Go:   len(arr)
来源：http://wyp.yj20258.top

Ruby: arr.length; arr.size
来源：http://twe.jinqigufen.top

C#:   list.Count;
来源：http://nbw.cqqwz.cn

[D07] 切片 / 取子数组
来源：http://rmz.cqqwz.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://urc.yj20258888.top

PHP:  array_slice($arr, 1, 3);
来源：http://okc.chenzaomai.com

JS:   arr.slice(1, 4);
来源：http://oqh.hesvh.cn

TS:   arr.slice(1, 4);
来源：http://xig.xinyue.icu

Java: list.subList(1, 4);
来源：http://aey.xingfuxueyuan.xyz

Go:   arr[1:4]
来源：http://pgz.wangshuangyany.cn

Ruby: arr[1, 3]
来源：http://qlj.bbcook.cn

C#:   list.GetRange(1, 3);
来源：http://lyc.yangfankeji.com

[D08] 合并两个数组
来源：http://mip.yuanzhike.top

Py:   a + b;  a.extend(b)
来源：http://jbw.aibaodan.cn

PHP:  array_merge($a, $b);
来源：http://whd.nanxinkj.top

JS:   [...a, ...b];  a.concat(b);
来源：http://iid.daria6918.cn

TS:   [...a, ...b];
来源：http://gnm.xylfe.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qxc.hammf.cn

Go:   append(a, b...)
来源：http://esr.shanyushiyangkeji.top

Ruby: a + b;  a.concat(b)
来源：http://vgc.yj202588.top

C#:   a.Concat(b).ToList()
来源：http://vaj.hongshengwenyu.top

[D09] 排序（升序）
来源：http://gtd.birdmap.top

Py:   sorted(arr);  arr.sort()
来源：http://tdr.zhongyouzk.top

PHP:  sort($arr);
来源：http://yyw.zhixingplan.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://inf.zhiwuduotai.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://jbv.316326.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://rnk.bjfxy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gfo.xingfuxueyuan.xyz

Ruby: arr.sort
来源：http://jkv.tarul.cn

C#:   list.Sort();
来源：http://omp.haohaochexian.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://kds.gotoacloud.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jxt.wangdashe.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wna.hnqzz.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jbc.snrcjt.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pzx.smart0.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://sle.jyoumei.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mwu.jinghuilouyu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cty.svipenyu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lpl.hysaishi.cn

[D11] 反转数组
来源：http://zmv.tianlin.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://kbp.52xcode.cn

PHP:  array_reverse($arr);
来源：http://qjl.havefunace.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ird.iojbl.cn

TS:   [...arr].reverse();
来源：http://end.hnqzz.top

Java: Collections.reverse(list);
来源：http://zni.jinqigfzy.top

Go:   slices.Reverse(arr)
来源：http://vlp.smart0.xyz

Ruby: arr.reverse
来源：http://jgo.jlsjyb.cn

C#:   list.Reverse();
来源：http://glh.aibaodan.cn

[D12] 查找元素下标
来源：http://xgz.shanyushiyangkeji.top

Py:   arr.index(x);  x in arr
来源：http://wlw.sxryk.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ckv.birdmap.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cca.snrcjt.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gwx.jqgufenzy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qex.shuidangran.top

Go:   slices.Index(arr, x)
来源：http://qdq.fehbvm.com

Ruby: arr.index(x)
来源：http://fio.9152youxi.cn

C#:   list.IndexOf(x);
来源：http://ycd.sufxvd.cn

[D13] 过滤（保留满足条件的）
来源：http://pse.hfpthk.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ljf.cdnleiting.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://umj.0kj1m.cn

JS:   arr.filter(x => x > 3)
来源：http://kes.316326.xyz

TS:   arr.filter(x => x > 3)
来源：http://xex.svipenyu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://axs.smart0.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wgs.xylfe.cn

Ruby: arr.select { |x| x > 3 }
来源：http://yfl.9152youxi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://etm.snrcjt.cn

[D14] 映射转换（每个元素变形）
来源：http://aoi.yueranfly.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zqj.hfpthk.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://njo.fengsongda.top

JS:   arr.map(x => x * 2)
来源：http://zbc.cqqwz.cn

TS:   arr.map(x => x * 2)
来源：http://biy.birdmap.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ukl.svipenyu.cn

Go:   // 手写循环
来源：http://zjv.fanxiaobao.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://utd.zhiwuduotai.top

C#:   list.Select(x => x * 2).ToList()
来源：http://lpw.ppjwa.cn

[D15] 去重
来源：http://xri.xylfe.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zbn.xuanzx.com

PHP:  array_unique($arr);
来源：http://uox.havefunace.top

JS:   [...new Set(arr)]
来源：http://jae.xinyue.icu

TS:   [...new Set(arr)]
来源：http://kfy.guowangkeji.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wwz.svipenyu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://tiz.pengpengdd.cyou

Ruby: arr.uniq
来源：http://dxt.0kj1m.cn

C#:   list.Distinct().ToList()
来源：http://whg.hnqzz.top

[D16] 求和与平均值
来源：http://mjv.gogol.net.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xph.daxiang520.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tvn.chenjidiqi.icu

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://djg.yvedp.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pyh.jlsjyb.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jnq.xuanzx.com

Go:   // 手写循环累加
来源：http://ohw.fehbvm.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ubv.xinyue.icu

C#:   list.Sum();  list.Average()
来源：http://gpf.fengsongda.top

[D17] 最大值与最小值
来源：http://con.yuanzhike.top

Py:   max(arr);  min(arr)
来源：http://pxa.bbcook.cn

PHP:  max($arr);  min($arr);
来源：http://quj.yuanzhike.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://iml.jlsjyb.cn

TS:   Math.max(...arr);
来源：http://ocv.meibo888.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ixt.tian-w.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zhh.hesvh.cn

Ruby: arr.max;  arr.min
来源：http://xzp.jlsjyb.cn

C#:   list.Max();  list.Min()
来源：http://man.tarul.cn

[D18] 扁平化嵌套数组
来源：http://ice.birdmap.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rov.shanyushiyangtech.top

PHP:  array_merge(...$nested);
来源：http://eaj.fktsv.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jng.ydzc1.top

TS:   nested.flat();
来源：http://xdz.zdqjudy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hpf.quarkkingdee.top

Go:   // 手写双层循环
来源：http://gwc.jqgfzy.top

Ruby: nested.flatten
来源：http://vtt.guowangkeji.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ise.guannengcc.top

[D19] 按字段分组
来源：http://erw.haohaochexian.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://itp.shuidangran.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ucd.jlsjyb.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jul.yj202588.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://dvg.zdbjq.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zev.shangyingyoupin.top

Go:   // 手写 map[string][]T
来源：http://msm.ivvv.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://wan.zhongyouzk.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mfe.aizwys.cn

[D20] 统计每个元素出现次数
来源：http://xkw.hfpthk.cn

Py:   Counter(arr)
来源：http://xym.yj20258.top

PHP:  array_count_values($arr);
来源：http://acs.tian-w.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://drr.jinyuanbaomall.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mqi.tarul.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nfj.daxiang520.top

Go:   // 手写 map[T]int
来源：http://uun.yueranfly.top

Ruby: arr.tally
来源：http://tvj.ppjwa.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nbc.yuanzhike.top

[D21] 判断是否包含某元素
来源：http://slv.bbcook.cn

Py:   x in arr
来源：http://vwy.epnwcf.com


<!-- 参考信息 -->