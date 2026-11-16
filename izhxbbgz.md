代发 wailian999

Py:   return a, b
来源：http://zld.sjlbkw.cn

PHP:  return [$a, $b];
来源：http://dyq.ywan-chungtsiang.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://eic.sjlbkw.cn

TS:   return { a, b };
来源：http://bba.fanxiaobao.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kmw.ydzc1.top

Go:   return a, b
来源：http://cjv.andypj.xyz

Ruby: return a, b
来源：http://xdb.gotoacloud.top

C#:   return (a, b);              // ValueTuple
来源：http://dlx.snrcjt.cn

[C06] 匿名函数 / lambda
来源：http://vqr.quarkkingdee.top

Py:   square = lambda x: x * x
来源：http://baz.cashguo.top

PHP:  $square = fn($x) => $x * $x;
来源：http://frg.jinqigfzy.top

JS:   const square = x => x * x;
来源：http://dbq.bbcook.cn

TS:   const square = (x: number): number => x * x;
来源：http://ora.yangfankeji.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mfk.yongpay.top

Go:   sq := func(x int) int { return x * x }
来源：http://yfn.zdqjudy.top

Ruby: square = ->(x) { x * x }
来源：http://rjk.shanyushiyangtech.top

C#:   Func<int, int> square = x => x * x;
来源：http://gjl.yongpay.top

[C07] 把函数作为参数传入
来源：http://kmw.cqqwz.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ted.yvedp.cn

PHP:  array_map("strtoupper", $arr);
来源：http://nib.nanxuanxn.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bne.tanke756.top

TS:   arr.map(String)
来源：http://zhb.shanyushiyangkeji.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://myz.gzhubu.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tql.ywan-chungtsiang.top

Ruby: arr.map(&:upcase)
来源：http://ggv.sufxvd.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://yxa.ctjpmb.com

[C08] 闭包
来源：http://gpx.cdnleiting.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vxx.cheryme.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bta.hammf.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://osr.yvedp.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://iuh.jinqigfzy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://phw.yuanzhike.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://grx.hnqzz.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zor.bbcook.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mxo.nanxuanxn.top

[C09] 递归
来源：http://jgl.ivvv.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ove.yj202588.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://aya.sjlbkw.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://upk.wangshuangyany.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kqf.sweek.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tbo.fengsongda.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dut.snrcjt.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xtl.fanxiaobao.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kqf.ppjwa.cn

[C10] 变量作用域
来源：http://ibl.vqdsnc.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nxs.nanxuanxn.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://egw.tanke756.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zfn.zhixingplan.top

TS:   同 JS
来源：http://gjt.sjlbkw.cn

Java: 方法内为块级作用域
来源：http://rjk.feifeiyinyue.top

Go:   花括号块级作用域
来源：http://kqw.ppjwa.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jst.dashuyun.cn

C#:   块级作用域
来源：http://fej.bbcook.cn

[C11] 模块导入与导出
来源：http://dut.zhijiandao.cn

Py:   from module import func
来源：http://voy.jinghuilouyu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://vnj.hnqzz.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://djx.hesvh.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://unt.cdnleiting.top

Java: import java.util.List;
来源：http://dkm.ybcxt.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gsh.9152youxi.cn

Ruby: require "json"; require_relative "./util"
来源：http://kgs.yj202588.top

C#:   using System.Text;
来源：http://qni.zdqjudy.top

[C12] 立即执行函数 IIFE
来源：http://mzf.yvedp.cn

Py:   (lambda: print("run"))()
来源：http://cvi.shanyushiyangkeji.top

PHP:  (function () { echo "run"; })();
来源：http://lob.zhixingplan.top

JS:   (() => { console.log("run"); })();
来源：http://ine.hysaishi.cn

TS:   (() => { console.log("run"); })();
来源：http://qdm.52xcode.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://czd.dianchejie.cn

Go:   func() { fmt.Println("run") }()
来源：http://fwk.jinqigfzy.top

Ruby: -> { puts "run" }.call
来源：http://ved.epnwcf.com

C#:   // 无 IIFE：用静态构造函数
来源：http://iel.daxiang520.top

[C13] 类型声明 / 类型注解
来源：http://aqx.ehwqpu.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://igj.ybcxt.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nux.shuidangran.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://git.yuxming.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zmk.hnqzz.top

Java: int add(int a, int b) { return a + b; }
来源：http://oah.jianghu66.top

Go:   func add(a, b int) int
来源：http://svv.birdmap.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mbp.xylfe.cn

C#:   int Add(int a, int b) => a + b;
来源：http://bxs.cqqwz.cn

[C14] 泛型函数
来源：http://xnl.gaohongyu789.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://izz.ydjk.org.cn

PHP:  // 无泛型
来源：http://ogo.nanxuanxn.top

JS:   // 无泛型
来源：http://xjr.gogol.net.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kkh.jinqigufen.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://itu.fktsv.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mar.iojbl.cn

Ruby: # 无泛型
来源：http://aqq.jyoumei.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vac.52xcode.cn

[C15] 解构 / 展开参数
来源：http://jtt.sweek.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kqe.ydzc1.top

PHP:  [$a, $b] = $pair;
来源：http://hgj.ivvv.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://saq.haohaochexian.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lrd.sufxvd.cn

Java: // 无解构
来源：http://wqo.zhongyouzk.top

Go:   // 无解构
来源：http://afj.cqqwz.cn

Ruby: a, b = pair
来源：http://jqs.xziqi.cn

C#:   var (a, b) = pair;
来源：http://zrh.sxryk.cn

[C16] 函数 / 方法重载
来源：http://vzo.guannengcc.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hri.yuanzhike.top

PHP:  // 无重载
来源：http://tab.ivvv.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ruo.havefunace.top

TS:   // 用联合类型或重载签名声明
来源：http://uwe.dashuyun.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://gbt.redwolf501.top

Go:   // 无重载：用不同函数名
来源：http://wbd.vqdsnc.cn

Ruby: # 无重载：靠动态参数
来源：http://oxv.jyoumei.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://aqc.316326.xyz

================================================================================
来源：http://jqs.fengsongda.top

D. 数组 / 列表 / 集合
来源：http://reb.shzxlz.cn

================================================================================
来源：http://mpp.daria6918.cn

[D01] 创建数组 / 列表
来源：http://wty.ybcxt.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://mnp.zhoulong.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hre.shzxlz.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://buz.jqgfzy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://oqw.quarkkingdee.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ynp.52xcode.cn

Go:   arr := []int{1, 2, 3}
来源：http://mwu.jyoumei.cn

Ruby: arr = [1, 2, 3]
来源：http://fmq.sjlbkw.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ihi.sufxvd.cn

[D02] 追加元素到末尾
来源：http://eyv.shangyingyoupin.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gep.haohaochexian.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xdf.svipenyu.cn

JS:   arr.push(4);
来源：http://udy.xinyue.icu

TS:   arr.push(4);
来源：http://isl.pengpengdd.cyou

Java: list.add(4);
来源：http://npd.zhaomingkeji.xyz

Go:   arr = append(arr, 4)
来源：http://tqs.ivvv.top

Ruby: arr << 4; arr.push(5)
来源：http://bch.chenlongwang.top

C#:   list.Add(4);
来源：http://tuj.sweek.top

[D03] 在指定位置插入元素
来源：http://bdu.hywenlv.cn

Py:   arr.insert(0, 0)
来源：http://paa.hysaishi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://iey.sysykeji.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://uuq.shzxlz.cn

TS:   arr.splice(0, 0, 0);
来源：http://wiq.ehwqpu.com

Java: list.add(0, 0);
来源：http://iff.fehbvm.com

Go:   arr = append([]int{0}, arr...)
来源：http://jvt.jqgufenzy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kpf.redwolf501.top

C#:   list.Insert(0, 0);
来源：http://hlj.daria6918.cn

[D04] 删除元素
来源：http://vki.jinqigfzy.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://iyl.guowangkeji.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kjv.pycfn.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vzw.bbcook.cn

TS:   arr.splice(0, 1);
来源：http://ojq.chenlongwang.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zon.yvedp.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yvu.ydjk.org.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cak.epnwcf.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vht.tianlin.xyz

[D05] 访问与修改元素
来源：http://uce.zhengqikj.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wce.gotoacloud.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sds.shuidangran.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pif.chenlongwang.top

TS:   arr[0]; arr.at(-1);
来源：http://xlf.daria6918.cn

Java: list.get(0); list.set(0, 9);
来源：http://qkj.svipenyu.cn

Go:   arr[0]; arr[0] = 9
来源：http://fza.bbcook.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://spi.sjlbkw.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yiy.dashuyun.cn

[D06] 数组长度
来源：http://ogf.xinyue.icu

Py:   len(arr)
来源：http://mvk.aizwys.cn

PHP:  count($arr);
来源：http://vdv.cdnleiting.top

JS:   arr.length
来源：http://qby.snrcjt.cn

TS:   arr.length
来源：http://jkg.zhoulong.xyz

Java: list.size();
来源：http://prd.ybcxt.top

Go:   len(arr)
来源：http://uxn.hammf.cn

Ruby: arr.length; arr.size
来源：http://rub.jinghuilouyu.cn

C#:   list.Count;
来源：http://dma.fengsongda.top

[D07] 切片 / 取子数组
来源：http://nya.sxryk.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lfm.shuidangran.top

PHP:  array_slice($arr, 1, 3);
来源：http://clo.fengsongda.top

JS:   arr.slice(1, 4);
来源：http://lkl.52xcode.cn

TS:   arr.slice(1, 4);
来源：http://rhb.epnwcf.com

Java: list.subList(1, 4);
来源：http://zyb.zhijiandao.cn

Go:   arr[1:4]
来源：http://gyr.yuanzhike.top

Ruby: arr[1, 3]
来源：http://bcg.yvedp.cn

C#:   list.GetRange(1, 3);
来源：http://giv.fehbvm.com

[D08] 合并两个数组
来源：http://ffu.zdbjq.cn

Py:   a + b;  a.extend(b)
来源：http://lft.jyoumei.cn

PHP:  array_merge($a, $b);
来源：http://xqn.xuetiantiany.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://tkg.yuxming.cn

TS:   [...a, ...b];
来源：http://hjt.xingfuxueyuan.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tni.jlsjyb.cn

Go:   append(a, b...)
来源：http://gpg.yj20258888.top

Ruby: a + b;  a.concat(b)
来源：http://fpp.svipenyu.cn

C#:   a.Concat(b).ToList()
来源：http://exc.xziqi.cn

[D09] 排序（升序）
来源：http://snr.ydzc1.top

Py:   sorted(arr);  arr.sort()
来源：http://kpa.shuidangran.top

PHP:  sort($arr);
来源：http://fko.cucudq.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rae.yuanzhike.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ykh.daria6918.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://yuf.jlsjyb.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://trn.fengsongda.top

Ruby: arr.sort
来源：http://xnz.nwbrower.top

C#:   list.Sort();
来源：http://jrj.chenzaomai.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://gvf.feifeiyinyue.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://acs.jqgfzy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uaa.yangfankeji.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fow.jinyuanbaomall.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://drx.iojbl.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nzu.smart0.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yie.guowangkeji.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://juo.dashuyun.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ses.pycfn.com

[D11] 反转数组
来源：http://ndi.kuanghao11.cn

Py:   arr[::-1];  arr.reverse()
来源：http://tuo.andypj.xyz

PHP:  array_reverse($arr);
来源：http://onh.jqgfzy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bzb.yj202588.top

TS:   [...arr].reverse();
来源：http://aas.zhengqikj.top

Java: Collections.reverse(list);
来源：http://jjj.c1oappe.top

Go:   slices.Reverse(arr)
来源：http://rbb.sysykeji.top

Ruby: arr.reverse
来源：http://kuj.guannengcc.top

C#:   list.Reverse();
来源：http://pce.hongshengwenyu.top

[D12] 查找元素下标
来源：http://yck.jianghu66.top

Py:   arr.index(x);  x in arr
来源：http://wcc.yonumen.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kxj.zhaomingkeji.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wwu.ybcxt.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ywb.zhoulong.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ndg.jinyuanbaomall.cn

Go:   slices.Index(arr, x)
来源：http://ggy.shanyushiyangkeji.top

Ruby: arr.index(x)
来源：http://qrd.xinyue.icu

C#:   list.IndexOf(x);
来源：http://zqi.hnqzz.top

[D13] 过滤（保留满足条件的）
来源：http://apc.nanxinkj.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ika.fzhhl.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://eqr.chenjidiqi.icu

JS:   arr.filter(x => x > 3)
来源：http://wfx.chenzaomai.com

TS:   arr.filter(x => x > 3)
来源：http://fpl.shangyingyoupin.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ahe.zhongyouzk.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://evb.jinqigfzy.top

Ruby: arr.select { |x| x > 3 }
来源：http://fcq.hywenlv.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://dlh.yueranfly.top

[D14] 映射转换（每个元素变形）
来源：http://ixn.bbcook.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rzr.yj202588.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kez.0kj1m.cn

JS:   arr.map(x => x * 2)
来源：http://upa.jyoumei.cn

TS:   arr.map(x => x * 2)
来源：http://dlt.wangdashe.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://see.nanxuanxn.top

Go:   // 手写循环
来源：http://mqx.quarkkingdee.top

Ruby: arr.map { |x| x * 2 }
来源：http://upo.cqqwz.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://guu.zhoulong.xyz

[D15] 去重
来源：http://qwk.fzhhl.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://arf.ehwqpu.com

PHP:  array_unique($arr);
来源：http://eko.ydjk.org.cn

JS:   [...new Set(arr)]
来源：http://fff.yvedp.cn

TS:   [...new Set(arr)]
来源：http://ahy.pengpengdd.cyou

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://grm.jinyuanbaomall.cn

Go:   // 用 map[T]struct{} 手写
来源：http://new.bjfxy.top

Ruby: arr.uniq
来源：http://nxu.quarkkingdee.top

C#:   list.Distinct().ToList()
来源：http://qkc.chenzaomai.com

[D16] 求和与平均值
来源：http://dit.jinyuanbaomall.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qig.cucudq.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://olm.hesvh.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ufh.hesvh.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vgy.nwbrower.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://eff.shuidangran.top

Go:   // 手写循环累加
来源：http://hxa.jiagoushi.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zsi.pycfn.com

C#:   list.Sum();  list.Average()
来源：http://twl.tianlin.xyz

[D17] 最大值与最小值
来源：http://vzd.cheryme.top

Py:   max(arr);  min(arr)
来源：http://njv.quarkkingdee.top

PHP:  max($arr);  min($arr);
来源：http://spu.cheryme.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://oqg.jinyuanbaomall.cn

TS:   Math.max(...arr);
来源：http://cja.fktsv.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://aqh.pycfn.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fkw.xinyue.icu

Ruby: arr.max;  arr.min
来源：http://kuv.zycfv.cn

C#:   list.Max();  list.Min()
来源：http://znf.nanxuanxn.top

[D18] 扁平化嵌套数组
来源：http://tkb.cashguo.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mqj.hfpthk.cn

PHP:  array_merge(...$nested);
来源：http://fkp.sweek.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jsv.daxiang520.top

TS:   nested.flat();
来源：http://caz.0kj1m.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bex.shanyushiyangkeji.top

Go:   // 手写双层循环
来源：http://syk.epnwcf.com

Ruby: nested.flatten
来源：http://hhq.bjfxy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://nfq.iojbl.cn

[D19] 按字段分组
来源：http://php.xylfe.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vpd.chenzaomai.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://efq.pengpengdd.cyou

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jfk.pycfn.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://wwv.316326.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zzf.sjlbkw.cn

Go:   // 手写 map[string][]T
来源：http://rzq.smart0.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://zrg.snrcjt.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://uxw.ywan-chungtsiang.top

[D20] 统计每个元素出现次数
来源：http://ess.xylfe.cn

Py:   Counter(arr)
来源：http://aao.ybcxt.top

PHP:  array_count_values($arr);
来源：http://nsd.daxiang520.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kvp.gaohongyu789.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hmg.zhaomingkeji.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://iad.ydjk.org.cn

Go:   // 手写 map[T]int
来源：http://stu.andypj.xyz

Ruby: arr.tally
来源：http://nos.hongshengwenyu.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://esz.birdmap.top

[D21] 判断是否包含某元素
来源：http://age.9152youxi.cn

Py:   x in arr
来源：http://uvr.smart0.xyz

PHP:  in_array($x, $arr, true);
来源：http://avk.chenzaomai.com

JS:   arr.includes(x)
来源：http://zdl.ivvv.top

TS:   arr.includes(x)
来源：http://qgs.jinyuanbaomall.cn

Java: list.contains(x)
来源：http://trs.kuanghao11.cn

Go:   slices.Contains(arr, x)
来源：http://cpl.fzhhl.top

Ruby: arr.include?(x)
来源：http://gij.dianchejie.cn

C#:   list.Contains(x)
来源：http://qxu.sweek.top

[D22] 复制数组（避免共享引用）
来源：http://tti.feifeiyinyue.top


<!-- 参考信息 -->