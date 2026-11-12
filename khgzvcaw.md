代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://ggo.aibaodan.cn

[C03] 可变参数
来源：http://qxr.jinqigfzy.top

Py:   def total(*args): return sum(args)
来源：http://kdu.uphjek.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mcu.fktsv.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ylc.zhiwuduotai.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nbm.tianlin.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://iwb.guannengcc.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ucd.vehdjk.com

Ruby: def total(*nums); nums.sum; end
来源：http://pko.ydjk.org.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://woi.shuidangran.top

[C04] 命名参数 / 关键字参数
来源：http://twt.tanke756.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yff.sysykeji.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wia.snrcjt.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://snx.aizwys.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://adf.gaohongyu789.top

Java: // 无：用 Builder 模式或 record
来源：http://jew.yongpay.top

Go:   // 无：用配置结构体参数
来源：http://dtd.gogol.net.cn

Ruby: f(a: 1, b: 2)
来源：http://twm.ydzc1.top

C#:   f(a: 1, b: 2)
来源：http://afk.yangfankeji.com

[C05] 返回多个值
来源：http://vkq.daria6918.cn

Py:   return a, b
来源：http://qax.cucudq.cn

PHP:  return [$a, $b];
来源：http://zae.yangfankeji.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://mqu.zhijiandao.cn

TS:   return { a, b };
来源：http://qxf.c1oappe.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gls.chenzaomai.com

Go:   return a, b
来源：http://kvn.epnwcf.com

Ruby: return a, b
来源：http://lbz.jinyuanbaomall.cn

C#:   return (a, b);              // ValueTuple
来源：http://zma.snrcjt.cn

[C06] 匿名函数 / lambda
来源：http://til.daxiang520.top

Py:   square = lambda x: x * x
来源：http://ujn.jinqigfzy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://unq.shanyushiyangkeji.top

JS:   const square = x => x * x;
来源：http://amy.yongpay.top

TS:   const square = (x: number): number => x * x;
来源：http://ufr.nanxinkj.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vlm.jianghu66.top

Go:   sq := func(x int) int { return x * x }
来源：http://nwm.dashuyun.cn

Ruby: square = ->(x) { x * x }
来源：http://ymd.316326.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://sti.jinqigfzy.top

[C07] 把函数作为参数传入
来源：http://cdh.hywenlv.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://obk.zhixingplan.top

PHP:  array_map("strtoupper", $arr);
来源：http://hkl.bjfxy.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uko.zhongyouzk.top

TS:   arr.map(String)
来源：http://ayc.jinghuilouyu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lau.zdqjudy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sgv.fehbvm.com

Ruby: arr.map(&:upcase)
来源：http://wrk.fengsongda.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ihj.fzhhl.top

[C08] 闭包
来源：http://dcz.hfpthk.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://oqf.zhengqikj.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nfa.cheryme.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vwk.yuxming.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://snc.fengsongda.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zjp.chenjidiqi.icu

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://can.ywan-chungtsiang.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kam.pengpengdd.cyou

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gwx.xinyue.icu

[C09] 递归
来源：http://plz.havefunace.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rju.hesvh.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kec.ivvv.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dkm.jqgfzy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tnz.svipenyu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vqp.jqgfzy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dua.yongpay.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://row.aizwys.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://plw.fehbvm.com

[C10] 变量作用域
来源：http://fli.chenjidiqi.icu

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://prv.jyoumei.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rnt.bjfxy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xkc.jinqigufen.top

TS:   同 JS
来源：http://chb.xylfe.cn

Java: 方法内为块级作用域
来源：http://bxp.cashguo.top

Go:   花括号块级作用域
来源：http://csn.9152youxi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pzy.vehdjk.com

C#:   块级作用域
来源：http://jdm.yj202588.top

[C11] 模块导入与导出
来源：http://ylz.mhx1999.top

Py:   from module import func
来源：http://joy.zhiwuduotai.top

PHP:  require "file.php";  或 use App\Service;
来源：http://fit.andypj.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://rfd.meibo888.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nhh.gotoacloud.top

Java: import java.util.List;
来源：http://tnp.vqdsnc.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://unw.chenjidiqi.icu

Ruby: require "json"; require_relative "./util"
来源：http://ygx.ydjk.org.cn

C#:   using System.Text;
来源：http://jyr.xinyue.icu

[C12] 立即执行函数 IIFE
来源：http://oih.jiagoushi.top

Py:   (lambda: print("run"))()
来源：http://ljv.vqdsnc.cn

PHP:  (function () { echo "run"; })();
来源：http://zjq.ywan-chungtsiang.top

JS:   (() => { console.log("run"); })();
来源：http://mcw.yuanzhike.top

TS:   (() => { console.log("run"); })();
来源：http://dph.cucudq.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://byw.andypj.xyz

Go:   func() { fmt.Println("run") }()
来源：http://hvj.yj20258888.top

Ruby: -> { puts "run" }.call
来源：http://kid.hnqzz.top

C#:   // 无 IIFE：用静态构造函数
来源：http://oqf.haohaochexian.top

[C13] 类型声明 / 类型注解
来源：http://lcv.zhengqikj.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gos.hesvh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xiu.jqgfzy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://dne.0kj1m.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hve.vqdsnc.cn

Java: int add(int a, int b) { return a + b; }
来源：http://szc.ydzc1.top

Go:   func add(a, b int) int
来源：http://cjf.cdnleiting.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://eip.wangdashe.top

C#:   int Add(int a, int b) => a + b;
来源：http://blg.yuxming.cn

[C14] 泛型函数
来源：http://woa.guannengcc.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hmt.yangfankeji.com

PHP:  // 无泛型
来源：http://wwu.fehbvm.com

JS:   // 无泛型
来源：http://rnc.jqgfzy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://itr.daria6918.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vlm.hnxiangtu.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://aas.zhoulong.xyz

Ruby: # 无泛型
来源：http://rsd.xylfe.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vng.zdqjudy.top

[C15] 解构 / 展开参数
来源：http://mkx.cucudq.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://unb.uphjek.com

PHP:  [$a, $b] = $pair;
来源：http://xhj.jiagoushi.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fbt.xziqi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nmg.hesvh.cn

Java: // 无解构
来源：http://vzs.xuanzx.com

Go:   // 无解构
来源：http://atx.yj20258.top

Ruby: a, b = pair
来源：http://cra.wangshuangyany.cn

C#:   var (a, b) = pair;
来源：http://zin.xziqi.cn

[C16] 函数 / 方法重载
来源：http://wlz.hesvh.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zzg.cashguo.top

PHP:  // 无重载
来源：http://xjd.hesvh.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://wvc.vehdjk.com

TS:   // 用联合类型或重载签名声明
来源：http://nlc.wangshuangyany.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://inz.shuidangran.top

Go:   // 无重载：用不同函数名
来源：http://xiy.sweek.top

Ruby: # 无重载：靠动态参数
来源：http://sin.tarul.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://zhd.chenzaomai.com

================================================================================
来源：http://qxo.xinyue.icu

D. 数组 / 列表 / 集合
来源：http://scb.zdbjq.cn

================================================================================
来源：http://vst.iojbl.cn

[D01] 创建数组 / 列表
来源：http://mep.ehwqpu.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://zsl.zdbjq.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yth.yonumen.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jna.jiagoushi.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://fhk.vehdjk.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://chp.yuanzhike.top

Go:   arr := []int{1, 2, 3}
来源：http://fss.bjfxy.top

Ruby: arr = [1, 2, 3]
来源：http://ybw.cdnleiting.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mms.cdnleiting.top

[D02] 追加元素到末尾
来源：http://dcw.zdqjudy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wei.jlsjyb.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xkf.mhx1999.top

JS:   arr.push(4);
来源：http://asu.gzhubu.top

TS:   arr.push(4);
来源：http://zlb.52xcode.cn

Java: list.add(4);
来源：http://sck.yonumen.top

Go:   arr = append(arr, 4)
来源：http://xpp.daxiang520.top

Ruby: arr << 4; arr.push(5)
来源：http://wkw.shangyingyoupin.top

C#:   list.Add(4);
来源：http://dtx.shanyushiyangkeji.top

[D03] 在指定位置插入元素
来源：http://mmp.xinyue.icu

Py:   arr.insert(0, 0)
来源：http://tgo.fengsongda.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dtz.shangyingyoupin.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qdn.ppjwa.cn

TS:   arr.splice(0, 0, 0);
来源：http://cpv.hcnkem.com

Java: list.add(0, 0);
来源：http://tjo.tarul.cn

Go:   arr = append([]int{0}, arr...)
来源：http://dui.cdnleiting.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cxh.aibaodan.cn

C#:   list.Insert(0, 0);
来源：http://okc.jianghu66.top

[D04] 删除元素
来源：http://lcg.sysykeji.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kmf.guannengcc.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lhj.fanxiaobao.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wol.zycfv.cn

TS:   arr.splice(0, 1);
来源：http://kpg.yuxming.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pnf.zhoulong.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jnf.feifeiyinyue.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ibd.aizwys.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ods.jianghu66.top

[D05] 访问与修改元素
来源：http://hpt.andypj.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://uvz.jinqigfzy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yds.nanxinkj.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lyx.shuidangran.top

TS:   arr[0]; arr.at(-1);
来源：http://zsp.jianghu66.top

Java: list.get(0); list.set(0, 9);
来源：http://dce.guowangkeji.top

Go:   arr[0]; arr[0] = 9
来源：http://ste.fzhhl.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mwx.hcnkem.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hgz.wangshuangyany.cn

[D06] 数组长度
来源：http://gtc.9152youxi.cn

Py:   len(arr)
来源：http://see.shanyushiyangtech.top

PHP:  count($arr);
来源：http://cfi.cheryme.top

JS:   arr.length
来源：http://kyz.dianchejie.cn

TS:   arr.length
来源：http://ejk.mhx1999.top

Java: list.size();
来源：http://xcq.ehwqpu.com

Go:   len(arr)
来源：http://yiz.9152youxi.cn

Ruby: arr.length; arr.size
来源：http://xvb.svipenyu.cn

C#:   list.Count;
来源：http://aoh.hywenlv.cn

[D07] 切片 / 取子数组
来源：http://xiv.uphjek.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pgn.yj202588.top

PHP:  array_slice($arr, 1, 3);
来源：http://ihp.ydjk.org.cn

JS:   arr.slice(1, 4);
来源：http://yew.zhengqikj.top

TS:   arr.slice(1, 4);
来源：http://ahq.zdqjudy.top

Java: list.subList(1, 4);
来源：http://coe.hnqzz.top

Go:   arr[1:4]
来源：http://ybx.tianlin.xyz

Ruby: arr[1, 3]
来源：http://xgb.fengsongda.top

C#:   list.GetRange(1, 3);
来源：http://mmc.ybcxt.top

[D08] 合并两个数组
来源：http://qyx.sjlbkw.cn

Py:   a + b;  a.extend(b)
来源：http://zen.guannengcc.top

PHP:  array_merge($a, $b);
来源：http://epa.52xcode.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://hsk.hnxiangtu.top

TS:   [...a, ...b];
来源：http://juf.shzxlz.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ttb.jianghu66.top

Go:   append(a, b...)
来源：http://mpc.shanyushiyangkeji.top

Ruby: a + b;  a.concat(b)
来源：http://kka.chenlongwang.top

C#:   a.Concat(b).ToList()
来源：http://ntl.uphjek.com

[D09] 排序（升序）
来源：http://dqe.0kj1m.cn

Py:   sorted(arr);  arr.sort()
来源：http://uji.wangshuangyany.cn

PHP:  sort($arr);
来源：http://pjf.shanyushiyangkeji.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nbl.yj20258.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://xzp.feifeiyinyue.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ddw.ivvv.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hyq.hysaishi.cn

Ruby: arr.sort
来源：http://xeh.ehwqpu.com

C#:   list.Sort();
来源：http://iqw.yuxming.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://myr.kuanghao11.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hpq.jinghuilouyu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gsg.yueranfly.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://twh.tarul.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ndz.chenlongwang.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://awl.shuidangran.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gpd.xylfe.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rnw.aizwys.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dfr.dianchejie.cn

[D11] 反转数组
来源：http://qtc.gogol.net.cn

Py:   arr[::-1];  arr.reverse()
来源：http://hkd.andypj.xyz

PHP:  array_reverse($arr);
来源：http://vil.sysykeji.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://umh.yvedp.cn

TS:   [...arr].reverse();
来源：http://cvq.meibo888.top

Java: Collections.reverse(list);
来源：http://crp.sxryk.cn

Go:   slices.Reverse(arr)
来源：http://bnd.gzhubu.top

Ruby: arr.reverse
来源：http://iso.jiagoushi.top

C#:   list.Reverse();
来源：http://kzd.fehbvm.com

[D12] 查找元素下标
来源：http://wjl.zhoulong.xyz

Py:   arr.index(x);  x in arr
来源：http://ers.uphjek.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pwl.zhongyouzk.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qqt.hnxiangtu.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://htg.hnqzz.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dod.kuanghao11.cn

Go:   slices.Index(arr, x)
来源：http://gbr.tian-w.cn

Ruby: arr.index(x)
来源：http://ydy.zhengqikj.top

C#:   list.IndexOf(x);
来源：http://cdf.wangshuangyany.cn

[D13] 过滤（保留满足条件的）
来源：http://gbp.andypj.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bps.ydjk.org.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sil.xuetiantiany.cn

JS:   arr.filter(x => x > 3)
来源：http://fsi.yuanzhike.top

TS:   arr.filter(x => x > 3)
来源：http://obo.ywan-chungtsiang.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qgl.hesvh.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tsa.c1oappe.top

Ruby: arr.select { |x| x > 3 }
来源：http://aml.yueranfly.top

C#:   list.Where(x => x > 3).ToList()
来源：http://bxa.aibaodan.cn

[D14] 映射转换（每个元素变形）
来源：http://gem.fanxiaobao.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ryl.andypj.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mck.xuetiantiany.cn

JS:   arr.map(x => x * 2)
来源：http://knx.xinyue.icu

TS:   arr.map(x => x * 2)
来源：http://ooi.chenzaomai.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://qpb.gotoacloud.top

Go:   // 手写循环
来源：http://qst.xziqi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://dtu.aizwys.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://shz.chenzaomai.com

[D15] 去重
来源：http://prm.tianlin.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://spz.zhongyouzk.top

PHP:  array_unique($arr);
来源：http://ana.9152youxi.cn

JS:   [...new Set(arr)]
来源：http://jre.nanxuanxn.top

TS:   [...new Set(arr)]
来源：http://ohu.pengpengdd.cyou

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://swx.zdqjudy.top

Go:   // 用 map[T]struct{} 手写
来源：http://fyd.tian-w.cn

Ruby: arr.uniq
来源：http://hwe.wangshuangyany.cn

C#:   list.Distinct().ToList()
来源：http://lcc.316326.xyz

[D16] 求和与平均值
来源：http://yuq.yangfankeji.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://eub.chenzaomai.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qdo.zhongyouzk.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://eyb.zdqjudy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lii.hongshengwenyu.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://apv.svipenyu.cn

Go:   // 手写循环累加
来源：http://iso.nwbrower.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hof.andypj.xyz

C#:   list.Sum();  list.Average()
来源：http://pbi.jinqigfzy.top

[D17] 最大值与最小值
来源：http://opp.yangfankeji.com

Py:   max(arr);  min(arr)
来源：http://yql.jianghu66.top

PHP:  max($arr);  min($arr);
来源：http://lbu.birdmap.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hqx.ydzc1.top

TS:   Math.max(...arr);
来源：http://ext.dashuyun.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://cjh.pengpengdd.cyou

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cur.jinyuanbaomall.cn

Ruby: arr.max;  arr.min
来源：http://jvw.tianlin.xyz

C#:   list.Max();  list.Min()
来源：http://ngs.ppjwa.cn

[D18] 扁平化嵌套数组
来源：http://lpu.hnqzz.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rce.tian-w.cn

PHP:  array_merge(...$nested);
来源：http://kei.dianchejie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yoe.chenzaomai.com

TS:   nested.flat();
来源：http://mri.hcnkem.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gkf.yj20258.top

Go:   // 手写双层循环
来源：http://fwa.andypj.xyz

Ruby: nested.flatten
来源：http://uuq.vehdjk.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://les.yj20258.top

[D19] 按字段分组
来源：http://lwq.jinghuilouyu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ypo.9152youxi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jtn.xylfe.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gyz.52xcode.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qzt.andypj.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hbq.chenlongwang.top

Go:   // 手写 map[string][]T
来源：http://uiw.yvedp.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://sxr.dianchejie.cn


<!-- 参考信息 -->