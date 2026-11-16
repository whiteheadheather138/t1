代发 wailian999

[C06] 匿名函数 / lambda
来源：http://qui.pycfn.com

Py:   square = lambda x: x * x
来源：http://bny.daxiang520.top

PHP:  $square = fn($x) => $x * $x;
来源：http://dro.zycfv.cn

JS:   const square = x => x * x;
来源：http://ymp.vqdsnc.cn

TS:   const square = (x: number): number => x * x;
来源：http://zns.xuetiantiany.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qai.jinghuilouyu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://zcm.jyoumei.cn

Ruby: square = ->(x) { x * x }
来源：http://okn.tian-w.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xuj.52xcode.cn

[C07] 把函数作为参数传入
来源：http://jot.tianlin.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ivm.haohaochexian.top

PHP:  array_map("strtoupper", $arr);
来源：http://nyv.hfpthk.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ffl.fengsongda.top

TS:   arr.map(String)
来源：http://vqv.ybcxt.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://guk.epnwcf.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mjh.hcnkem.com

Ruby: arr.map(&:upcase)
来源：http://zxj.jinghuilouyu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://zkb.ivvv.top

[C08] 闭包
来源：http://ptr.ydzc1.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nkz.fanxiaobao.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gxv.yuxming.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xvw.gogol.net.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://icz.cheryme.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ibv.jqgufenzy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xjy.0kj1m.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zth.cheryme.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yxr.jinqigfzy.top

[C09] 递归
来源：http://upw.meibo888.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cnc.bjfxy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mpp.dianchejie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cvf.ppjwa.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wtd.ydzc1.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hda.yuanzhike.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pgh.fehbvm.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://duw.chenzaomai.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nol.andypj.xyz

[C10] 变量作用域
来源：http://mck.snrcjt.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yoa.nwbrower.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gtx.dianchejie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mwa.fengsongda.top

TS:   同 JS
来源：http://ujk.vqdsnc.cn

Java: 方法内为块级作用域
来源：http://lly.ehwqpu.com

Go:   花括号块级作用域
来源：http://tvi.xuanzx.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xfj.hcnkem.com

C#:   块级作用域
来源：http://ifq.andypj.xyz

[C11] 模块导入与导出
来源：http://cxj.yuxming.cn

Py:   from module import func
来源：http://act.yuxming.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://qqr.andypj.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://wws.ctjpmb.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gko.zhixingplan.top

Java: import java.util.List;
来源：http://pcm.zdqjudy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hhm.sxryk.cn

Ruby: require "json"; require_relative "./util"
来源：http://yhb.hnxiangtu.top

C#:   using System.Text;
来源：http://udv.dashuyun.cn

[C12] 立即执行函数 IIFE
来源：http://tnu.chenlongwang.top

Py:   (lambda: print("run"))()
来源：http://vmq.tianlin.xyz

PHP:  (function () { echo "run"; })();
来源：http://qql.jinghuilouyu.cn

JS:   (() => { console.log("run"); })();
来源：http://gqc.feifeiyinyue.top

TS:   (() => { console.log("run"); })();
来源：http://txf.snrcjt.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zut.bbcook.cn

Go:   func() { fmt.Println("run") }()
来源：http://nvs.zhiwuduotai.top

Ruby: -> { puts "run" }.call
来源：http://akd.hywenlv.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://lvq.xingfuxueyuan.xyz

[C13] 类型声明 / 类型注解
来源：http://bqc.shuidangran.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://lbm.haohaochexian.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jct.xuanzx.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ssy.cdnleiting.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yzv.jinqigufen.top

Java: int add(int a, int b) { return a + b; }
来源：http://jij.hywenlv.cn

Go:   func add(a, b int) int
来源：http://edb.zhoulong.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dwr.hongshengwenyu.top

C#:   int Add(int a, int b) => a + b;
来源：http://gle.sufxvd.cn

[C14] 泛型函数
来源：http://icl.nanxinkj.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kvf.kuanghao11.cn

PHP:  // 无泛型
来源：http://pfg.shanyushiyangtech.top

JS:   // 无泛型
来源：http://oxk.52xcode.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xai.yj20258888.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://spa.zhijiandao.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://quw.zhijiandao.cn

Ruby: # 无泛型
来源：http://adc.xylfe.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pas.dashuyun.cn

[C15] 解构 / 展开参数
来源：http://qzx.gzhubu.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lrq.dianchejie.cn

PHP:  [$a, $b] = $pair;
来源：http://ggk.cqqwz.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://giq.pycfn.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kzq.aizwys.cn

Java: // 无解构
来源：http://ydt.zhongyouzk.top

Go:   // 无解构
来源：http://zup.316326.xyz

Ruby: a, b = pair
来源：http://oyp.snrcjt.cn

C#:   var (a, b) = pair;
来源：http://xwc.jqgufenzy.top

[C16] 函数 / 方法重载
来源：http://snw.vehdjk.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kyf.yvedp.cn

PHP:  // 无重载
来源：http://evq.yj20258.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ymv.aibaodan.cn

TS:   // 用联合类型或重载签名声明
来源：http://eqi.shzxlz.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://lfs.tanke756.top

Go:   // 无重载：用不同函数名
来源：http://atx.cheryme.top

Ruby: # 无重载：靠动态参数
来源：http://fsq.xinyue.icu

C#:   void F(int a) {}  void F(string a) {}
来源：http://bcd.nanxuanxn.top

================================================================================
来源：http://sxe.wangshuangyany.cn

D. 数组 / 列表 / 集合
来源：http://bfp.ivvv.top

================================================================================
来源：http://muu.xuetiantiany.cn

[D01] 创建数组 / 列表
来源：http://coh.cqqwz.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pes.vehdjk.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sje.pycfn.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gke.yfazqb.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://wvw.hongshengwenyu.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bxv.sweek.top

Go:   arr := []int{1, 2, 3}
来源：http://zwk.9152youxi.cn

Ruby: arr = [1, 2, 3]
来源：http://vku.zhoulong.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bos.sxryk.cn

[D02] 追加元素到末尾
来源：http://kom.yj202588.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xrw.meibo888.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fxc.jinghuilouyu.cn

JS:   arr.push(4);
来源：http://wky.smart0.xyz

TS:   arr.push(4);
来源：http://xzk.gotoacloud.top

Java: list.add(4);
来源：http://gpn.svipenyu.cn

Go:   arr = append(arr, 4)
来源：http://ovb.chenjidiqi.icu

Ruby: arr << 4; arr.push(5)
来源：http://ksi.zhoulong.xyz

C#:   list.Add(4);
来源：http://gxl.yanxiufei.cn

[D03] 在指定位置插入元素
来源：http://bjy.yongpay.top

Py:   arr.insert(0, 0)
来源：http://wur.zycfv.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pvo.xuetiantiany.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://aic.yangfankeji.com

TS:   arr.splice(0, 0, 0);
来源：http://tuf.havefunace.top

Java: list.add(0, 0);
来源：http://zab.xziqi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://hto.tarul.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cgm.nanxuanxn.top

C#:   list.Insert(0, 0);
来源：http://hqr.ydjk.org.cn

[D04] 删除元素
来源：http://aez.kuanghao11.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gjn.ydjk.org.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pww.redwolf501.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jou.bjfxy.top

TS:   arr.splice(0, 1);
来源：http://bkr.gogol.net.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jsw.yj20258.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mkl.quarkkingdee.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://res.bbcook.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://slw.hammf.cn

[D05] 访问与修改元素
来源：http://gud.meibo888.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://syn.yuanzhike.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://khl.pycfn.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://iuy.smart0.xyz

TS:   arr[0]; arr.at(-1);
来源：http://cyy.yanxiufei.cn

Java: list.get(0); list.set(0, 9);
来源：http://tko.zhiwuduotai.top

Go:   arr[0]; arr[0] = 9
来源：http://ork.sufxvd.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wof.nwbrower.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bbt.iojbl.cn

[D06] 数组长度
来源：http://aib.nanxinkj.top

Py:   len(arr)
来源：http://hjl.yonumen.top

PHP:  count($arr);
来源：http://lrd.vehdjk.com

JS:   arr.length
来源：http://kmo.nanxinkj.top

TS:   arr.length
来源：http://cyz.jinghuilouyu.cn

Java: list.size();
来源：http://egw.9152youxi.cn

Go:   len(arr)
来源：http://hts.tian-w.cn

Ruby: arr.length; arr.size
来源：http://lwt.chenjidiqi.icu

C#:   list.Count;
来源：http://yjf.yonumen.top

[D07] 切片 / 取子数组
来源：http://oup.0kj1m.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ijm.jinyuanbaomall.cn

PHP:  array_slice($arr, 1, 3);
来源：http://iew.cashguo.top

JS:   arr.slice(1, 4);
来源：http://jpa.ywan-chungtsiang.top

TS:   arr.slice(1, 4);
来源：http://epa.tarul.cn

Java: list.subList(1, 4);
来源：http://fpq.smart0.xyz

Go:   arr[1:4]
来源：http://bxa.hongshengwenyu.top

Ruby: arr[1, 3]
来源：http://zmt.zycfv.cn

C#:   list.GetRange(1, 3);
来源：http://wcs.jiagoushi.top

[D08] 合并两个数组
来源：http://ugg.chenzaomai.com

Py:   a + b;  a.extend(b)
来源：http://wlj.havefunace.top

PHP:  array_merge($a, $b);
来源：http://xvk.daria6918.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://fvx.jlsjyb.cn

TS:   [...a, ...b];
来源：http://eeo.meibo888.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bob.vehdjk.com

Go:   append(a, b...)
来源：http://ezc.sufxvd.cn

Ruby: a + b;  a.concat(b)
来源：http://azm.yuanzhike.top

C#:   a.Concat(b).ToList()
来源：http://bkg.hammf.cn

[D09] 排序（升序）
来源：http://bdk.gogol.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://pjo.fanxiaobao.xyz

PHP:  sort($arr);
来源：http://kua.xylfe.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dgu.ivvv.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://kbr.redwolf501.top

Java: Collections.sort(list);  list.sort(null);
来源：http://pjl.yj20258.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://atx.xylfe.cn

Ruby: arr.sort
来源：http://wfz.hcnkem.com

C#:   list.Sort();
来源：http://myp.nwbrower.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://fwg.yuanzhike.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zzj.xinyue.icu

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://isc.tanke756.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sec.cucudq.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://klz.shanyushiyangkeji.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://upb.ybcxt.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sox.jiagoushi.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gfj.jqgufenzy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zyi.tanke756.top

[D11] 反转数组
来源：http://tmw.ctjpmb.com

Py:   arr[::-1];  arr.reverse()
来源：http://oac.yonumen.top

PHP:  array_reverse($arr);
来源：http://pgq.guannengcc.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tmc.yangfankeji.com

TS:   [...arr].reverse();
来源：http://exk.yj202588.top

Java: Collections.reverse(list);
来源：http://vum.fzhhl.top

Go:   slices.Reverse(arr)
来源：http://vjc.tian-w.cn

Ruby: arr.reverse
来源：http://dfw.ppjwa.cn

C#:   list.Reverse();
来源：http://nxm.ydzc1.top

[D12] 查找元素下标
来源：http://fog.jyoumei.cn

Py:   arr.index(x);  x in arr
来源：http://dpc.tianlin.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uxd.ppjwa.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xas.ivvv.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dir.shuidangran.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vvb.gotoacloud.top

Go:   slices.Index(arr, x)
来源：http://bmi.yongpay.top

Ruby: arr.index(x)
来源：http://qzn.feifeiyinyue.top

C#:   list.IndexOf(x);
来源：http://spp.epnwcf.com

[D13] 过滤（保留满足条件的）
来源：http://uga.sjlbkw.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wuw.vehdjk.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pcm.yueranfly.top

JS:   arr.filter(x => x > 3)
来源：http://ymx.xziqi.cn

TS:   arr.filter(x => x > 3)
来源：http://cne.zdbjq.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lii.wangdashe.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tpp.yvedp.cn

Ruby: arr.select { |x| x > 3 }
来源：http://dqk.bbcook.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://bjv.wangshuangyany.cn

[D14] 映射转换（每个元素变形）
来源：http://pcl.jqgfzy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://eoo.yj20258.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sjy.dashuyun.cn

JS:   arr.map(x => x * 2)
来源：http://qve.cheryme.top

TS:   arr.map(x => x * 2)
来源：http://gnw.xuetiantiany.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://vpv.jinqigufen.top

Go:   // 手写循环
来源：http://hjf.ydjk.org.cn

Ruby: arr.map { |x| x * 2 }
来源：http://quz.xingfuxueyuan.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://jfr.yangfankeji.com

[D15] 去重
来源：http://rjm.smart0.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kqx.hfpthk.cn

PHP:  array_unique($arr);
来源：http://lwn.tanke756.top

JS:   [...new Set(arr)]
来源：http://huv.feifeiyinyue.top

TS:   [...new Set(arr)]
来源：http://yog.fehbvm.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cel.sweek.top

Go:   // 用 map[T]struct{} 手写
来源：http://rwv.nanxinkj.top

Ruby: arr.uniq
来源：http://rhx.wangdashe.top

C#:   list.Distinct().ToList()
来源：http://vvd.bbcook.cn

[D16] 求和与平均值
来源：http://nlb.cucudq.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ycq.zhengqikj.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zlj.guannengcc.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jsf.yj202588.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jjy.jinqigufen.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vqr.zhaomingkeji.xyz

Go:   // 手写循环累加
来源：http://jgn.jiagoushi.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mac.mhx1999.top

C#:   list.Sum();  list.Average()
来源：http://vsc.hnqzz.top

[D17] 最大值与最小值
来源：http://pan.shuidangran.top

Py:   max(arr);  min(arr)
来源：http://fyo.yangfankeji.com

PHP:  max($arr);  min($arr);
来源：http://pyv.sjlbkw.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://moi.tianlin.xyz

TS:   Math.max(...arr);
来源：http://yep.cqqwz.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://tbx.jianghu66.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pkj.quarkkingdee.top

Ruby: arr.max;  arr.min
来源：http://gat.zdbjq.cn

C#:   list.Max();  list.Min()
来源：http://ush.ppjwa.cn

[D18] 扁平化嵌套数组
来源：http://vit.hfpthk.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://upf.xuetiantiany.cn

PHP:  array_merge(...$nested);
来源：http://tzv.dianchejie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://flj.sjlbkw.cn

TS:   nested.flat();
来源：http://pab.cheryme.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sod.zycfv.cn

Go:   // 手写双层循环
来源：http://kcs.xuetiantiany.cn

Ruby: nested.flatten
来源：http://utr.ybcxt.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://vdw.chenzaomai.com

[D19] 按字段分组
来源：http://hbw.zhiwuduotai.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wda.zdbjq.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zux.zdqjudy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kxb.dianchejie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://cco.gotoacloud.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zqo.316326.xyz

Go:   // 手写 map[string][]T
来源：http://rkf.yueranfly.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://gub.hfpthk.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bpq.cdnleiting.top

[D20] 统计每个元素出现次数
来源：http://xpk.ivvv.top

Py:   Counter(arr)
来源：http://obl.jinghuilouyu.cn

PHP:  array_count_values($arr);
来源：http://nki.chenzaomai.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://waj.haohaochexian.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hld.snrcjt.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rkn.ybcxt.top

Go:   // 手写 map[T]int
来源：http://jdw.sufxvd.cn

Ruby: arr.tally
来源：http://cej.chenjidiqi.icu

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pgh.yuxming.cn

[D21] 判断是否包含某元素
来源：http://kyw.bjfxy.top

Py:   x in arr
来源：http://aej.yueranfly.top

PHP:  in_array($x, $arr, true);
来源：http://adz.ydjk.org.cn

JS:   arr.includes(x)
来源：http://qxx.ctjpmb.com

TS:   arr.includes(x)
来源：http://epx.ehwqpu.com

Java: list.contains(x)
来源：http://nrv.sjlbkw.cn

Go:   slices.Contains(arr, x)
来源：http://xsm.xingfuxueyuan.xyz

Ruby: arr.include?(x)
来源：http://mta.svipenyu.cn

C#:   list.Contains(x)
来源：http://eqz.yongpay.top

[D22] 复制数组（避免共享引用）
来源：http://trh.yuxming.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hrp.316326.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ewu.cqqwz.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vhv.zhongyouzk.top

TS:   [...arr];
来源：http://tsi.xuetiantiany.cn

Java: new ArrayList<>(list);
来源：http://axc.yanxiufei.cn

Go:   copied := append([]int(nil), arr...)
来源：http://shz.andypj.xyz

Ruby: arr.dup;  arr.clone
来源：http://cos.xziqi.cn

C#:   new List<int>(list);
来源：http://zsf.jinyuanbaomall.cn


<!-- 参考信息 -->