代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://zcx.cqqwz.cn

[C03] 可变参数
来源：http://xxl.9152youxi.cn

Py:   def total(*args): return sum(args)
来源：http://rsp.zhongyouzk.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mss.jqgfzy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wiw.haohaochexian.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wqi.shzxlz.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://uek.hfpthk.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vsb.birdmap.top

Ruby: def total(*nums); nums.sum; end
来源：http://tvs.daria6918.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://sqb.haohaochexian.top

[C04] 命名参数 / 关键字参数
来源：http://ffz.sxryk.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mvu.0kj1m.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nae.bbcook.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vvj.xziqi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://txw.52xcode.cn

Java: // 无：用 Builder 模式或 record
来源：http://qtd.ctjpmb.com

Go:   // 无：用配置结构体参数
来源：http://glf.zdqjudy.top

Ruby: f(a: 1, b: 2)
来源：http://hkj.shangyingyoupin.top

C#:   f(a: 1, b: 2)
来源：http://mew.chenlongwang.top

[C05] 返回多个值
来源：http://zeu.zhoulong.xyz

Py:   return a, b
来源：http://ndq.jinqigufen.top

PHP:  return [$a, $b];
来源：http://ljm.jinqigfzy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://wdf.hcnkem.com

TS:   return { a, b };
来源：http://hrq.shanyushiyangkeji.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ogp.havefunace.top

Go:   return a, b
来源：http://vbr.chenlongwang.top

Ruby: return a, b
来源：http://ogd.0kj1m.cn

C#:   return (a, b);              // ValueTuple
来源：http://vzr.xuetiantiany.cn

[C06] 匿名函数 / lambda
来源：http://bsc.jinghuilouyu.cn

Py:   square = lambda x: x * x
来源：http://fcr.hfpthk.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wky.yanxiufei.cn

JS:   const square = x => x * x;
来源：http://kwf.sweek.top

TS:   const square = (x: number): number => x * x;
来源：http://vfo.zhaomingkeji.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://prg.chenzaomai.com

Go:   sq := func(x int) int { return x * x }
来源：http://zpy.meibo888.top

Ruby: square = ->(x) { x * x }
来源：http://cui.hysaishi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://vhf.chenlongwang.top

[C07] 把函数作为参数传入
来源：http://tzp.iojbl.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jin.fzhhl.top

PHP:  array_map("strtoupper", $arr);
来源：http://wwd.mhx1999.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vnz.ivvv.top

TS:   arr.map(String)
来源：http://yng.52xcode.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vqh.ydjk.org.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://knp.xinyue.icu

Ruby: arr.map(&:upcase)
来源：http://xjw.jyoumei.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://tfc.xuanzx.com

[C08] 闭包
来源：http://jxl.zhengqikj.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jhs.shanyushiyangtech.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uai.tianlin.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wax.zdbjq.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vgc.jyoumei.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://odp.chenjidiqi.icu

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://eps.ybcxt.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://egf.hongshengwenyu.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yuy.pycfn.com

[C09] 递归
来源：http://fgo.uphjek.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rvh.yj20258.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zzp.ehwqpu.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dzj.jinghuilouyu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wxs.fktsv.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://woc.xuetiantiany.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://aoa.52xcode.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pyi.fzhhl.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ajq.hysaishi.cn

[C10] 变量作用域
来源：http://mvm.dashuyun.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fzt.bbcook.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kus.sxryk.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wln.ppjwa.cn

TS:   同 JS
来源：http://ewi.sysykeji.top

Java: 方法内为块级作用域
来源：http://xas.mhx1999.top

Go:   花括号块级作用域
来源：http://dtu.shangyingyoupin.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nfr.xylfe.cn

C#:   块级作用域
来源：http://jvy.hongshengwenyu.top

[C11] 模块导入与导出
来源：http://xob.zhengqikj.top

Py:   from module import func
来源：http://niy.shanyushiyangtech.top

PHP:  require "file.php";  或 use App\Service;
来源：http://cjr.hcnkem.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://ibe.kuanghao11.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yvf.0kj1m.cn

Java: import java.util.List;
来源：http://beg.shanyushiyangtech.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vaq.cdnleiting.top

Ruby: require "json"; require_relative "./util"
来源：http://rtb.chenjidiqi.icu

C#:   using System.Text;
来源：http://oln.daxiang520.top

[C12] 立即执行函数 IIFE
来源：http://ppw.fzhhl.top

Py:   (lambda: print("run"))()
来源：http://qhq.zhongyouzk.top

PHP:  (function () { echo "run"; })();
来源：http://qlt.hesvh.cn

JS:   (() => { console.log("run"); })();
来源：http://emu.fehbvm.com

TS:   (() => { console.log("run"); })();
来源：http://osr.svipenyu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hpx.zhongyouzk.top

Go:   func() { fmt.Println("run") }()
来源：http://lis.bbcook.cn

Ruby: -> { puts "run" }.call
来源：http://tkb.dashuyun.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ajh.havefunace.top

[C13] 类型声明 / 类型注解
来源：http://hdg.zdqjudy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rlo.hammf.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pnb.zhaomingkeji.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://szx.feifeiyinyue.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://czd.ydzc1.top

Java: int add(int a, int b) { return a + b; }
来源：http://xos.0kj1m.cn

Go:   func add(a, b int) int
来源：http://uxi.havefunace.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ahz.shangyingyoupin.top

C#:   int Add(int a, int b) => a + b;
来源：http://grp.hysaishi.cn

[C14] 泛型函数
来源：http://auu.52xcode.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kkk.nwbrower.top

PHP:  // 无泛型
来源：http://yel.hywenlv.cn

JS:   // 无泛型
来源：http://jwk.fzhhl.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tri.jqgfzy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tfj.ydjk.org.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://epe.yj20258.top

Ruby: # 无泛型
来源：http://bxv.fengsongda.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qve.zhiwuduotai.top

[C15] 解构 / 展开参数
来源：http://rrx.cucudq.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://neb.ybcxt.top

PHP:  [$a, $b] = $pair;
来源：http://gip.sjlbkw.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://erw.quarkkingdee.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zsc.zhixingplan.top

Java: // 无解构
来源：http://usm.cheryme.top

Go:   // 无解构
来源：http://dvx.jqgfzy.top

Ruby: a, b = pair
来源：http://knl.zdqjudy.top

C#:   var (a, b) = pair;
来源：http://lfs.tanke756.top

[C16] 函数 / 方法重载
来源：http://xww.c1oappe.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sbn.pycfn.com

PHP:  // 无重载
来源：http://buh.ehwqpu.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://opj.jinghuilouyu.cn

TS:   // 用联合类型或重载签名声明
来源：http://kdu.jyoumei.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://dwm.zdqjudy.top

Go:   // 无重载：用不同函数名
来源：http://yeg.andypj.xyz

Ruby: # 无重载：靠动态参数
来源：http://gmm.gaohongyu789.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://sdc.yanxiufei.cn

================================================================================
来源：http://piy.chenjidiqi.icu

D. 数组 / 列表 / 集合
来源：http://qnd.316326.xyz

================================================================================
来源：http://wbc.ybcxt.top

[D01] 创建数组 / 列表
来源：http://yjk.shuidangran.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://vpy.zhongyouzk.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://opc.andypj.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cle.haohaochexian.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://elh.iojbl.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://irj.zdbjq.cn

Go:   arr := []int{1, 2, 3}
来源：http://nws.jyoumei.cn

Ruby: arr = [1, 2, 3]
来源：http://kmk.wangdashe.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://but.quarkkingdee.top

[D02] 追加元素到末尾
来源：http://enp.9152youxi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://uhr.zhoulong.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yni.epnwcf.com

JS:   arr.push(4);
来源：http://nfl.daxiang520.top

TS:   arr.push(4);
来源：http://bsk.xylfe.cn

Java: list.add(4);
来源：http://gal.wangdashe.top

Go:   arr = append(arr, 4)
来源：http://gra.fktsv.cn

Ruby: arr << 4; arr.push(5)
来源：http://ehg.zdqjudy.top

C#:   list.Add(4);
来源：http://oqf.hywenlv.cn

[D03] 在指定位置插入元素
来源：http://urz.hnqzz.top

Py:   arr.insert(0, 0)
来源：http://cin.zhixingplan.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://row.shzxlz.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xmv.zhiwuduotai.top

TS:   arr.splice(0, 0, 0);
来源：http://pny.ivvv.top

Java: list.add(0, 0);
来源：http://ufe.zycfv.cn

Go:   arr = append([]int{0}, arr...)
来源：http://kou.hnxiangtu.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vgm.hesvh.cn

C#:   list.Insert(0, 0);
来源：http://hga.xinyue.icu

[D04] 删除元素
来源：http://hoa.quarkkingdee.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ttg.birdmap.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wde.316326.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wso.fehbvm.com

TS:   arr.splice(0, 1);
来源：http://snd.ywan-chungtsiang.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vee.kuanghao11.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wzh.jqgfzy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://uea.ywan-chungtsiang.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zhd.jiagoushi.top

[D05] 访问与修改元素
来源：http://kmh.pengpengdd.cyou

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bwn.ehwqpu.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jiu.xinyue.icu

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tik.gaohongyu789.top

TS:   arr[0]; arr.at(-1);
来源：http://gnj.zhongyouzk.top

Java: list.get(0); list.set(0, 9);
来源：http://pvw.tian-w.cn

Go:   arr[0]; arr[0] = 9
来源：http://oov.shanyushiyangtech.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://imt.sxryk.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xiu.sweek.top

[D06] 数组长度
来源：http://nmd.yfazqb.com

Py:   len(arr)
来源：http://rhv.52xcode.cn

PHP:  count($arr);
来源：http://eki.52xcode.cn

JS:   arr.length
来源：http://qea.fehbvm.com

TS:   arr.length
来源：http://erx.tarul.cn

Java: list.size();
来源：http://iaf.shuidangran.top

Go:   len(arr)
来源：http://hvx.smart0.xyz

Ruby: arr.length; arr.size
来源：http://kbg.yuanzhike.top

C#:   list.Count;
来源：http://zlj.dianchejie.cn

[D07] 切片 / 取子数组
来源：http://fup.jyoumei.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rsd.wangdashe.top

PHP:  array_slice($arr, 1, 3);
来源：http://jeu.zhongyouzk.top

JS:   arr.slice(1, 4);
来源：http://fdz.aibaodan.cn

TS:   arr.slice(1, 4);
来源：http://iih.zdbjq.cn

Java: list.subList(1, 4);
来源：http://hbi.pengpengdd.cyou

Go:   arr[1:4]
来源：http://gdp.316326.xyz

Ruby: arr[1, 3]
来源：http://lnf.wangshuangyany.cn

C#:   list.GetRange(1, 3);
来源：http://qku.cqqwz.cn

[D08] 合并两个数组
来源：http://clr.9152youxi.cn

Py:   a + b;  a.extend(b)
来源：http://qfi.fehbvm.com

PHP:  array_merge($a, $b);
来源：http://uzx.xziqi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://mzd.yfazqb.com

TS:   [...a, ...b];
来源：http://cwl.zhaomingkeji.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zph.epnwcf.com

Go:   append(a, b...)
来源：http://lau.fengsongda.top

Ruby: a + b;  a.concat(b)
来源：http://jqo.sjlbkw.cn

C#:   a.Concat(b).ToList()
来源：http://zff.jinqigufen.top

[D09] 排序（升序）
来源：http://qta.fktsv.cn

Py:   sorted(arr);  arr.sort()
来源：http://ofu.shuidangran.top

PHP:  sort($arr);
来源：http://awl.c1oappe.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dsq.quarkkingdee.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://yfn.ctjpmb.com

Java: Collections.sort(list);  list.sort(null);
来源：http://fpb.jlsjyb.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bjb.yfazqb.com

Ruby: arr.sort
来源：http://gda.ehwqpu.com

C#:   list.Sort();
来源：http://qpf.yj20258888.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://wki.fehbvm.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zde.tianlin.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://csa.snrcjt.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nkr.hcnkem.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rqs.c1oappe.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qen.chenlongwang.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lre.nanxuanxn.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ftl.ppjwa.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yrv.yj202588.top

[D11] 反转数组
来源：http://lfh.ppjwa.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qcx.xingfuxueyuan.xyz

PHP:  array_reverse($arr);
来源：http://gqg.fehbvm.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ouu.snrcjt.cn

TS:   [...arr].reverse();
来源：http://gwp.tanke756.top

Java: Collections.reverse(list);
来源：http://ajf.jinqigufen.top

Go:   slices.Reverse(arr)
来源：http://zmm.redwolf501.top

Ruby: arr.reverse
来源：http://ppt.jiagoushi.top

C#:   list.Reverse();
来源：http://oee.xuetiantiany.cn

[D12] 查找元素下标
来源：http://brx.svipenyu.cn

Py:   arr.index(x);  x in arr
来源：http://rre.shzxlz.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dsh.smart0.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://man.aibaodan.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mxv.fzhhl.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wro.nanxuanxn.top

Go:   slices.Index(arr, x)
来源：http://xxn.cheryme.top

Ruby: arr.index(x)
来源：http://ikb.andypj.xyz

C#:   list.IndexOf(x);
来源：http://cdn.c1oappe.top

[D13] 过滤（保留满足条件的）
来源：http://bos.shuidangran.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lmz.guowangkeji.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://die.cheryme.top

JS:   arr.filter(x => x > 3)
来源：http://gto.fehbvm.com

TS:   arr.filter(x => x > 3)
来源：http://gwa.aizwys.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wcb.jqgufenzy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://anw.fengsongda.top

Ruby: arr.select { |x| x > 3 }
来源：http://kym.zhongyouzk.top

C#:   list.Where(x => x > 3).ToList()
来源：http://nyl.c1oappe.top

[D14] 映射转换（每个元素变形）
来源：http://lpp.chenlongwang.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ypm.9152youxi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qtw.zhaomingkeji.xyz

JS:   arr.map(x => x * 2)
来源：http://tnc.jinqigfzy.top

TS:   arr.map(x => x * 2)
来源：http://auc.jqgfzy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://bva.fanxiaobao.xyz

Go:   // 手写循环
来源：http://xvu.zhijiandao.cn

Ruby: arr.map { |x| x * 2 }
来源：http://cdb.yanxiufei.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ziw.aibaodan.cn

[D15] 去重
来源：http://wxe.ydjk.org.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xwz.chenzaomai.com

PHP:  array_unique($arr);
来源：http://efl.zhijiandao.cn

JS:   [...new Set(arr)]
来源：http://hto.hongshengwenyu.top

TS:   [...new Set(arr)]
来源：http://abx.dashuyun.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qsz.jqgufenzy.top

Go:   // 用 map[T]struct{} 手写
来源：http://lcb.cucudq.cn

Ruby: arr.uniq
来源：http://sci.haohaochexian.top

C#:   list.Distinct().ToList()
来源：http://dau.yj20258.top

[D16] 求和与平均值
来源：http://vxj.svipenyu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pml.hysaishi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://guz.chenjidiqi.icu

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jhv.mhx1999.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jlp.wangshuangyany.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kha.jinqigufen.top

Go:   // 手写循环累加
来源：http://djc.sjlbkw.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jji.ydzc1.top

C#:   list.Sum();  list.Average()
来源：http://faz.bbcook.cn

[D17] 最大值与最小值
来源：http://qhg.fengsongda.top

Py:   max(arr);  min(arr)
来源：http://ioq.daria6918.cn

PHP:  max($arr);  min($arr);
来源：http://mke.cdnleiting.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://eyy.cheryme.top

TS:   Math.max(...arr);
来源：http://vef.snrcjt.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://rjm.hongshengwenyu.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qix.gaohongyu789.top

Ruby: arr.max;  arr.min
来源：http://qow.jianghu66.top

C#:   list.Max();  list.Min()
来源：http://jxd.fanxiaobao.xyz

[D18] 扁平化嵌套数组
来源：http://etc.smart0.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://stq.52xcode.cn

PHP:  array_merge(...$nested);
来源：http://qex.gzhubu.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kks.zhongyouzk.top

TS:   nested.flat();
来源：http://kjw.fengsongda.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vzv.tianlin.xyz

Go:   // 手写双层循环
来源：http://jer.wangshuangyany.cn

Ruby: nested.flatten
来源：http://ejf.chenzaomai.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://mwn.hysaishi.cn

[D19] 按字段分组
来源：http://xml.jinghuilouyu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jmb.hywenlv.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lax.jinqigfzy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qci.xziqi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://smx.fehbvm.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rce.sxryk.cn

Go:   // 手写 map[string][]T
来源：http://oht.yuxming.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://owc.guowangkeji.top


<!-- 参考信息 -->