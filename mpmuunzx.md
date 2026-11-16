代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://zic.hysaishi.cn

[C03] 可变参数
来源：http://isg.fzhhl.top

Py:   def total(*args): return sum(args)
来源：http://lof.fehbvm.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bci.kuanghao11.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pka.quarkkingdee.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uhc.zhengqikj.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ayb.dashuyun.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://raz.guannengcc.top

Ruby: def total(*nums); nums.sum; end
来源：http://vdd.dianchejie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://igl.yj202588.top

[C04] 命名参数 / 关键字参数
来源：http://jqs.wangshuangyany.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pfn.guannengcc.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dst.smart0.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zzz.ydjk.org.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dyv.meibo888.top

Java: // 无：用 Builder 模式或 record
来源：http://qww.andypj.xyz

Go:   // 无：用配置结构体参数
来源：http://ocb.9152youxi.cn

Ruby: f(a: 1, b: 2)
来源：http://ayi.gotoacloud.top

C#:   f(a: 1, b: 2)
来源：http://swz.yfazqb.com

[C05] 返回多个值
来源：http://eph.jqgufenzy.top

Py:   return a, b
来源：http://ehd.uphjek.com

PHP:  return [$a, $b];
来源：http://bhq.chenzaomai.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://glv.sufxvd.cn

TS:   return { a, b };
来源：http://usj.quarkkingdee.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zca.yueranfly.top

Go:   return a, b
来源：http://qbj.jyoumei.cn

Ruby: return a, b
来源：http://nlk.havefunace.top

C#:   return (a, b);              // ValueTuple
来源：http://tzp.dianchejie.cn

[C06] 匿名函数 / lambda
来源：http://tjn.yvedp.cn

Py:   square = lambda x: x * x
来源：http://lqn.svipenyu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xab.iojbl.cn

JS:   const square = x => x * x;
来源：http://wqi.jqgufenzy.top

TS:   const square = (x: number): number => x * x;
来源：http://fgh.zdqjudy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lkq.zhongyouzk.top

Go:   sq := func(x int) int { return x * x }
来源：http://qyu.sweek.top

Ruby: square = ->(x) { x * x }
来源：http://cig.xuanzx.com

C#:   Func<int, int> square = x => x * x;
来源：http://tcf.jqgufenzy.top

[C07] 把函数作为参数传入
来源：http://vvv.52xcode.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gca.aizwys.cn

PHP:  array_map("strtoupper", $arr);
来源：http://wrv.yongpay.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://heu.shanyushiyangkeji.top

TS:   arr.map(String)
来源：http://cdm.gogol.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qeb.zhijiandao.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mub.ivvv.top

Ruby: arr.map(&:upcase)
来源：http://hfm.ehwqpu.com

C#:   arr.Select(s => s.ToUpper())
来源：http://ufl.fzhhl.top

[C08] 闭包
来源：http://giy.yueranfly.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zph.sxryk.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ona.feifeiyinyue.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fwa.vqdsnc.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ygv.uphjek.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://axy.meibo888.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ran.pycfn.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bpo.sxryk.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hex.jinqigufen.top

[C09] 递归
来源：http://cjl.dashuyun.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nne.feifeiyinyue.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cfa.shzxlz.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://msp.xziqi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bro.shuidangran.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://eky.guowangkeji.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dcc.shangyingyoupin.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tvc.sufxvd.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jbc.jianghu66.top

[C10] 变量作用域
来源：http://nsa.jianghu66.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kol.tarul.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fzu.redwolf501.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pal.ywan-chungtsiang.top

TS:   同 JS
来源：http://hit.xingfuxueyuan.xyz

Java: 方法内为块级作用域
来源：http://xpf.zhongyouzk.top

Go:   花括号块级作用域
来源：http://vlf.fanxiaobao.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jhz.tanke756.top

C#:   块级作用域
来源：http://zeg.hongshengwenyu.top

[C11] 模块导入与导出
来源：http://uie.fehbvm.com

Py:   from module import func
来源：http://asb.aibaodan.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://rwr.snrcjt.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://oke.wangdashe.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://eux.shzxlz.cn

Java: import java.util.List;
来源：http://ahz.cheryme.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pgg.tian-w.cn

Ruby: require "json"; require_relative "./util"
来源：http://rjm.xziqi.cn

C#:   using System.Text;
来源：http://fkl.jinghuilouyu.cn

[C12] 立即执行函数 IIFE
来源：http://byi.daxiang520.top

Py:   (lambda: print("run"))()
来源：http://fnn.xingfuxueyuan.xyz

PHP:  (function () { echo "run"; })();
来源：http://xug.tianlin.xyz

JS:   (() => { console.log("run"); })();
来源：http://sdb.ydzc1.top

TS:   (() => { console.log("run"); })();
来源：http://soq.jianghu66.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jxl.cucudq.cn

Go:   func() { fmt.Println("run") }()
来源：http://vuw.yj202588.top

Ruby: -> { puts "run" }.call
来源：http://jzg.yj202588.top

C#:   // 无 IIFE：用静态构造函数
来源：http://vhk.yj202588.top

[C13] 类型声明 / 类型注解
来源：http://exz.jyoumei.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ztx.tarul.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bjd.smart0.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://iof.jinyuanbaomall.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yim.zhongyouzk.top

Java: int add(int a, int b) { return a + b; }
来源：http://ibw.quarkkingdee.top

Go:   func add(a, b int) int
来源：http://ffp.chenjidiqi.icu

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wjk.daria6918.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fwb.ywan-chungtsiang.top

[C14] 泛型函数
来源：http://mvr.xinyue.icu

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dho.xuetiantiany.cn

PHP:  // 无泛型
来源：http://rrt.jyoumei.cn

JS:   // 无泛型
来源：http://ogr.xuetiantiany.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rkd.guowangkeji.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://skp.ydzc1.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://squ.daria6918.cn

Ruby: # 无泛型
来源：http://sfp.hnxiangtu.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dce.jlsjyb.cn

[C15] 解构 / 展开参数
来源：http://mea.mhx1999.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zmo.wangshuangyany.cn

PHP:  [$a, $b] = $pair;
来源：http://otf.tanke756.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nwt.daxiang520.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zgn.sweek.top

Java: // 无解构
来源：http://ksb.jiagoushi.top

Go:   // 无解构
来源：http://dyy.xuetiantiany.cn

Ruby: a, b = pair
来源：http://oaw.gaohongyu789.top

C#:   var (a, b) = pair;
来源：http://age.zdqjudy.top

[C16] 函数 / 方法重载
来源：http://ycv.jianghu66.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://imi.c1oappe.top

PHP:  // 无重载
来源：http://uvt.kuanghao11.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://clk.52xcode.cn

TS:   // 用联合类型或重载签名声明
来源：http://ysn.yonumen.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ugp.bbcook.cn

Go:   // 无重载：用不同函数名
来源：http://afa.52xcode.cn

Ruby: # 无重载：靠动态参数
来源：http://btm.havefunace.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://jhz.quarkkingdee.top

================================================================================
来源：http://zze.zhoulong.xyz

D. 数组 / 列表 / 集合
来源：http://pbo.316326.xyz

================================================================================
来源：http://vez.jinqigufen.top

[D01] 创建数组 / 列表
来源：http://cic.quarkkingdee.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://jpz.tian-w.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sgb.zhoulong.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ygs.yongpay.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://xzw.jqgufenzy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://igp.gotoacloud.top

Go:   arr := []int{1, 2, 3}
来源：http://xpw.yfazqb.com

Ruby: arr = [1, 2, 3]
来源：http://vyh.jyoumei.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cow.uphjek.com

[D02] 追加元素到末尾
来源：http://wki.jqgfzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kmt.jinyuanbaomall.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vtv.yfazqb.com

JS:   arr.push(4);
来源：http://jwd.jinghuilouyu.cn

TS:   arr.push(4);
来源：http://anv.nanxuanxn.top

Java: list.add(4);
来源：http://bwc.vqdsnc.cn

Go:   arr = append(arr, 4)
来源：http://rgn.gaohongyu789.top

Ruby: arr << 4; arr.push(5)
来源：http://nte.andypj.xyz

C#:   list.Add(4);
来源：http://wkm.nwbrower.top

[D03] 在指定位置插入元素
来源：http://tyy.ivvv.top

Py:   arr.insert(0, 0)
来源：http://plp.wangshuangyany.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://amk.yuxming.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fek.fehbvm.com

TS:   arr.splice(0, 0, 0);
来源：http://zxy.snrcjt.cn

Java: list.add(0, 0);
来源：http://out.zhiwuduotai.top

Go:   arr = append([]int{0}, arr...)
来源：http://mrq.c1oappe.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sjy.svipenyu.cn

C#:   list.Insert(0, 0);
来源：http://jec.epnwcf.com

[D04] 删除元素
来源：http://jae.snrcjt.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ejl.wangdashe.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nup.xylfe.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ctr.cdnleiting.top

TS:   arr.splice(0, 1);
来源：http://kzj.yvedp.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jse.zhoulong.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lyg.zdqjudy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qly.chenzaomai.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yhu.zhixingplan.top

[D05] 访问与修改元素
来源：http://qzz.xuanzx.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lcy.cheryme.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qex.zhengqikj.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tgd.xylfe.cn

TS:   arr[0]; arr.at(-1);
来源：http://dfx.jinqigfzy.top

Java: list.get(0); list.set(0, 9);
来源：http://hjb.yanxiufei.cn

Go:   arr[0]; arr[0] = 9
来源：http://ihv.ydjk.org.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wky.jiagoushi.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ftt.daria6918.cn

[D06] 数组长度
来源：http://txk.havefunace.top

Py:   len(arr)
来源：http://fax.yanxiufei.cn

PHP:  count($arr);
来源：http://eds.ywan-chungtsiang.top

JS:   arr.length
来源：http://qoy.yuanzhike.top

TS:   arr.length
来源：http://wkp.yueranfly.top

Java: list.size();
来源：http://toq.yj20258888.top

Go:   len(arr)
来源：http://get.havefunace.top

Ruby: arr.length; arr.size
来源：http://vas.mhx1999.top

C#:   list.Count;
来源：http://jwr.yanxiufei.cn

[D07] 切片 / 取子数组
来源：http://nuz.nwbrower.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qgz.hammf.cn

PHP:  array_slice($arr, 1, 3);
来源：http://pla.andypj.xyz

JS:   arr.slice(1, 4);
来源：http://lcs.zhoulong.xyz

TS:   arr.slice(1, 4);
来源：http://gir.tianlin.xyz

Java: list.subList(1, 4);
来源：http://cck.hcnkem.com

Go:   arr[1:4]
来源：http://rmc.zhongyouzk.top

Ruby: arr[1, 3]
来源：http://blp.gzhubu.top

C#:   list.GetRange(1, 3);
来源：http://npo.fengsongda.top

[D08] 合并两个数组
来源：http://pqy.hnqzz.top

Py:   a + b;  a.extend(b)
来源：http://fiz.epnwcf.com

PHP:  array_merge($a, $b);
来源：http://tql.316326.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://bhn.shanyushiyangkeji.top

TS:   [...a, ...b];
来源：http://pow.ehwqpu.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://noj.hysaishi.cn

Go:   append(a, b...)
来源：http://wrh.jyoumei.cn

Ruby: a + b;  a.concat(b)
来源：http://wsi.jiagoushi.top

C#:   a.Concat(b).ToList()
来源：http://ifi.hywenlv.cn

[D09] 排序（升序）
来源：http://myt.zdqjudy.top

Py:   sorted(arr);  arr.sort()
来源：http://sqj.yvedp.cn

PHP:  sort($arr);
来源：http://acx.tanke756.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wze.hongshengwenyu.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ggq.vqdsnc.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://aws.zhiwuduotai.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vbd.fehbvm.com

Ruby: arr.sort
来源：http://mvf.tanke756.top

C#:   list.Sort();
来源：http://prk.hnqzz.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://vzd.zhoulong.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ztl.mhx1999.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hkw.cqqwz.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hbf.cdnleiting.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qcs.havefunace.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gkm.sweek.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rqk.ydjk.org.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://laa.daria6918.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fos.sjlbkw.cn

[D11] 反转数组
来源：http://iqz.jianghu66.top

Py:   arr[::-1];  arr.reverse()
来源：http://vtu.shuidangran.top

PHP:  array_reverse($arr);
来源：http://hul.jqgfzy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://aeu.jianghu66.top

TS:   [...arr].reverse();
来源：http://upj.cashguo.top

Java: Collections.reverse(list);
来源：http://uuj.redwolf501.top

Go:   slices.Reverse(arr)
来源：http://qvv.havefunace.top

Ruby: arr.reverse
来源：http://cef.vehdjk.com

C#:   list.Reverse();
来源：http://oel.ybcxt.top

[D12] 查找元素下标
来源：http://fyb.vehdjk.com

Py:   arr.index(x);  x in arr
来源：http://uxj.guowangkeji.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dle.yj202588.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rob.zhiwuduotai.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pyw.shangyingyoupin.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jjk.zhoulong.xyz

Go:   slices.Index(arr, x)
来源：http://eip.gzhubu.top

Ruby: arr.index(x)
来源：http://klj.guowangkeji.top

C#:   list.IndexOf(x);
来源：http://dcb.hysaishi.cn

[D13] 过滤（保留满足条件的）
来源：http://gzl.gaohongyu789.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://uur.xinyue.icu

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tye.hywenlv.cn

JS:   arr.filter(x => x > 3)
来源：http://snu.wangdashe.top

TS:   arr.filter(x => x > 3)
来源：http://hmh.nwbrower.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://shd.hywenlv.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cdg.shanyushiyangkeji.top

Ruby: arr.select { |x| x > 3 }
来源：http://zxc.gaohongyu789.top

C#:   list.Where(x => x > 3).ToList()
来源：http://sem.fengsongda.top

[D14] 映射转换（每个元素变形）
来源：http://eya.smart0.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://uhj.wangdashe.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://twr.xingfuxueyuan.xyz

JS:   arr.map(x => x * 2)
来源：http://edj.gotoacloud.top

TS:   arr.map(x => x * 2)
来源：http://klm.c1oappe.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://olx.tian-w.cn

Go:   // 手写循环
来源：http://ynv.gaohongyu789.top

Ruby: arr.map { |x| x * 2 }
来源：http://wxx.xuanzx.com

C#:   list.Select(x => x * 2).ToList()
来源：http://udo.gzhubu.top

[D15] 去重
来源：http://jcp.tianlin.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gnn.316326.xyz

PHP:  array_unique($arr);
来源：http://lkk.gaohongyu789.top

JS:   [...new Set(arr)]
来源：http://goa.daria6918.cn

TS:   [...new Set(arr)]
来源：http://htt.gzhubu.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jnd.sxryk.cn

Go:   // 用 map[T]struct{} 手写
来源：http://pjz.andypj.xyz

Ruby: arr.uniq
来源：http://zeb.tarul.cn

C#:   list.Distinct().ToList()
来源：http://zlz.dashuyun.cn

[D16] 求和与平均值
来源：http://ksc.ybcxt.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ebq.ppjwa.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tyj.tian-w.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hvt.yueranfly.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nyg.shangyingyoupin.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pwq.zhijiandao.cn

Go:   // 手写循环累加
来源：http://sjm.gzhubu.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://smg.0kj1m.cn

C#:   list.Sum();  list.Average()
来源：http://gwp.hesvh.cn

[D17] 最大值与最小值
来源：http://uws.epnwcf.com

Py:   max(arr);  min(arr)
来源：http://pfa.zhijiandao.cn

PHP:  max($arr);  min($arr);
来源：http://hwt.chenzaomai.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://coo.vqdsnc.cn

TS:   Math.max(...arr);
来源：http://ofd.fanxiaobao.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://zmn.vqdsnc.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fsm.zhoulong.xyz

Ruby: arr.max;  arr.min
来源：http://wpr.hfpthk.cn

C#:   list.Max();  list.Min()
来源：http://krh.cucudq.cn

[D18] 扁平化嵌套数组
来源：http://kzb.vehdjk.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cio.shanyushiyangtech.top

PHP:  array_merge(...$nested);
来源：http://lhd.jiagoushi.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xlq.kuanghao11.cn

TS:   nested.flat();
来源：http://mco.sjlbkw.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dye.zhaomingkeji.xyz

Go:   // 手写双层循环
来源：http://dhv.ivvv.top

Ruby: nested.flatten
来源：http://ohe.gotoacloud.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://bcc.yueranfly.top

[D19] 按字段分组
来源：http://ptm.xingfuxueyuan.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ixs.cucudq.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zoc.sjlbkw.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://drl.sxryk.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://yzb.hesvh.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gzr.daria6918.cn

Go:   // 手写 map[string][]T
来源：http://dyg.yj20258.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://vig.yuxming.cn


<!-- 参考信息 -->