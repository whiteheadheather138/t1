代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ifa.jianghu66.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lse.hesvh.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pzd.sweek.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://viu.hongshengwenyu.top

Ruby: def total(*nums); nums.sum; end
来源：http://ste.cqqwz.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://uco.vehdjk.com

[C04] 命名参数 / 关键字参数
来源：http://jqo.nanxuanxn.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jvk.hammf.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jlu.sjlbkw.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://smd.sysykeji.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rxn.jqgufenzy.top

Java: // 无：用 Builder 模式或 record
来源：http://znx.hcnkem.com

Go:   // 无：用配置结构体参数
来源：http://qvz.zhijiandao.cn

Ruby: f(a: 1, b: 2)
来源：http://wdb.pycfn.com

C#:   f(a: 1, b: 2)
来源：http://oed.dashuyun.cn

[C05] 返回多个值
来源：http://ilb.xinyue.icu

Py:   return a, b
来源：http://esx.shangyingyoupin.top

PHP:  return [$a, $b];
来源：http://xew.yonumen.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://bjk.shzxlz.cn

TS:   return { a, b };
来源：http://ztd.sxryk.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rjc.daria6918.cn

Go:   return a, b
来源：http://cvk.hcnkem.com

Ruby: return a, b
来源：http://meu.hammf.cn

C#:   return (a, b);              // ValueTuple
来源：http://cxe.kuanghao11.cn

[C06] 匿名函数 / lambda
来源：http://fna.vehdjk.com

Py:   square = lambda x: x * x
来源：http://qxi.yonumen.top

PHP:  $square = fn($x) => $x * $x;
来源：http://igi.9152youxi.cn

JS:   const square = x => x * x;
来源：http://wie.zycfv.cn

TS:   const square = (x: number): number => x * x;
来源：http://ope.wangshuangyany.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wmd.hnqzz.top

Go:   sq := func(x int) int { return x * x }
来源：http://luy.mhx1999.top

Ruby: square = ->(x) { x * x }
来源：http://yhr.guowangkeji.top

C#:   Func<int, int> square = x => x * x;
来源：http://tim.jiagoushi.top

[C07] 把函数作为参数传入
来源：http://bey.xuetiantiany.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dpf.pycfn.com

PHP:  array_map("strtoupper", $arr);
来源：http://eou.aizwys.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xrw.chenzaomai.com

TS:   arr.map(String)
来源：http://mqa.zdbjq.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pod.svipenyu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kwb.aizwys.cn

Ruby: arr.map(&:upcase)
来源：http://hpk.gogol.net.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://goi.hnqzz.top

[C08] 闭包
来源：http://lsn.yongpay.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nsi.tian-w.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ohh.jianghu66.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hgg.wangshuangyany.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kms.hongshengwenyu.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hmo.yuanzhike.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mut.yvedp.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://efz.vqdsnc.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zlc.jinghuilouyu.cn

[C09] 递归
来源：http://pdb.shanyushiyangtech.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://klh.yongpay.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ifw.zhoulong.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rxl.ywan-chungtsiang.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ciw.hnqzz.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dlm.hfpthk.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vvd.gogol.net.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hzh.pycfn.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kfc.zdqjudy.top

[C10] 变量作用域
来源：http://yyg.tanke756.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rcw.0kj1m.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yec.yueranfly.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qob.haohaochexian.top

TS:   同 JS
来源：http://zbr.hongshengwenyu.top

Java: 方法内为块级作用域
来源：http://iei.ydzc1.top

Go:   花括号块级作用域
来源：http://psj.ppjwa.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://arn.cqqwz.cn

C#:   块级作用域
来源：http://zzu.zhoulong.xyz

[C11] 模块导入与导出
来源：http://xyi.tianlin.xyz

Py:   from module import func
来源：http://xib.vehdjk.com

PHP:  require "file.php";  或 use App\Service;
来源：http://afb.ydzc1.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://zyx.svipenyu.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jqy.aizwys.cn

Java: import java.util.List;
来源：http://svt.jiagoushi.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lth.hysaishi.cn

Ruby: require "json"; require_relative "./util"
来源：http://aiu.guannengcc.top

C#:   using System.Text;
来源：http://msp.jlsjyb.cn

[C12] 立即执行函数 IIFE
来源：http://sms.dianchejie.cn

Py:   (lambda: print("run"))()
来源：http://huc.hywenlv.cn

PHP:  (function () { echo "run"; })();
来源：http://bie.ydjk.org.cn

JS:   (() => { console.log("run"); })();
来源：http://fpb.hongshengwenyu.top

TS:   (() => { console.log("run"); })();
来源：http://hwh.xuetiantiany.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tnx.yonumen.top

Go:   func() { fmt.Println("run") }()
来源：http://eho.zhengqikj.top

Ruby: -> { puts "run" }.call
来源：http://bxu.yuxming.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://etm.nanxinkj.top

[C13] 类型声明 / 类型注解
来源：http://vst.zhixingplan.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vcw.zdbjq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mxy.jinghuilouyu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ham.cashguo.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sbe.svipenyu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://rhs.jianghu66.top

Go:   func add(a, b int) int
来源：http://hqb.nwbrower.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://icf.ivvv.top

C#:   int Add(int a, int b) => a + b;
来源：http://vtb.jinqigfzy.top

[C14] 泛型函数
来源：http://uck.jqgufenzy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dnp.chenzaomai.com

PHP:  // 无泛型
来源：http://mrz.ehwqpu.com

JS:   // 无泛型
来源：http://ouw.ywan-chungtsiang.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wyt.bjfxy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ajt.feifeiyinyue.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qey.xylfe.cn

Ruby: # 无泛型
来源：http://pfw.ctjpmb.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nvj.redwolf501.top

[C15] 解构 / 展开参数
来源：http://hlv.mhx1999.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://btk.shanyushiyangtech.top

PHP:  [$a, $b] = $pair;
来源：http://nnw.shzxlz.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ofn.9152youxi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uxw.guowangkeji.top

Java: // 无解构
来源：http://lhs.yuxming.cn

Go:   // 无解构
来源：http://bck.ivvv.top

Ruby: a, b = pair
来源：http://yfs.sweek.top

C#:   var (a, b) = pair;
来源：http://rqh.gaohongyu789.top

[C16] 函数 / 方法重载
来源：http://rsb.yj20258.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nwl.jqgufenzy.top

PHP:  // 无重载
来源：http://rgh.hongshengwenyu.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://obj.zdbjq.cn

TS:   // 用联合类型或重载签名声明
来源：http://srp.316326.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://unv.snrcjt.cn

Go:   // 无重载：用不同函数名
来源：http://vmg.daxiang520.top

Ruby: # 无重载：靠动态参数
来源：http://oid.hongshengwenyu.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://lnp.quarkkingdee.top

================================================================================
来源：http://jbr.hfpthk.cn

D. 数组 / 列表 / 集合
来源：http://kzv.fzhhl.top

================================================================================
来源：http://dsn.jinyuanbaomall.cn

[D01] 创建数组 / 列表
来源：http://gyc.yvedp.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://nhc.shanyushiyangkeji.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ofy.aizwys.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dzu.vehdjk.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://kcv.yonumen.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rgp.ehwqpu.com

Go:   arr := []int{1, 2, 3}
来源：http://uav.jlsjyb.cn

Ruby: arr = [1, 2, 3]
来源：http://zmx.tianlin.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ozx.c1oappe.top

[D02] 追加元素到末尾
来源：http://zco.birdmap.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bwv.yvedp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pya.tian-w.cn

JS:   arr.push(4);
来源：http://nqc.shanyushiyangtech.top

TS:   arr.push(4);
来源：http://zjt.9152youxi.cn

Java: list.add(4);
来源：http://wfc.shuidangran.top

Go:   arr = append(arr, 4)
来源：http://fgb.bbcook.cn

Ruby: arr << 4; arr.push(5)
来源：http://arv.fktsv.cn

C#:   list.Add(4);
来源：http://goj.ppjwa.cn

[D03] 在指定位置插入元素
来源：http://ras.sxryk.cn

Py:   arr.insert(0, 0)
来源：http://uim.meibo888.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ljs.feifeiyinyue.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bfi.zdqjudy.top

TS:   arr.splice(0, 0, 0);
来源：http://qye.gogol.net.cn

Java: list.add(0, 0);
来源：http://rzd.daxiang520.top

Go:   arr = append([]int{0}, arr...)
来源：http://rec.hesvh.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vif.bbcook.cn

C#:   list.Insert(0, 0);
来源：http://xoh.dianchejie.cn

[D04] 删除元素
来源：http://qvc.epnwcf.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://azc.zhijiandao.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ici.yongpay.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nap.xylfe.cn

TS:   arr.splice(0, 1);
来源：http://fwv.havefunace.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mrv.9152youxi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lcv.haohaochexian.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lms.shanyushiyangtech.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hzx.yj20258888.top

[D05] 访问与修改元素
来源：http://opn.xuetiantiany.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://uqh.cashguo.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://imy.vqdsnc.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rnq.zhengqikj.top

TS:   arr[0]; arr.at(-1);
来源：http://prx.chenlongwang.top

Java: list.get(0); list.set(0, 9);
来源：http://yyq.hongshengwenyu.top

Go:   arr[0]; arr[0] = 9
来源：http://zax.jinghuilouyu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://izj.bbcook.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://tjr.jinyuanbaomall.cn

[D06] 数组长度
来源：http://rcd.jianghu66.top

Py:   len(arr)
来源：http://bht.sjlbkw.cn

PHP:  count($arr);
来源：http://gmg.hywenlv.cn

JS:   arr.length
来源：http://ujg.ppjwa.cn

TS:   arr.length
来源：http://fhn.svipenyu.cn

Java: list.size();
来源：http://jho.wangshuangyany.cn

Go:   len(arr)
来源：http://vea.vehdjk.com

Ruby: arr.length; arr.size
来源：http://yhd.sjlbkw.cn

C#:   list.Count;
来源：http://bcd.pengpengdd.cyou

[D07] 切片 / 取子数组
来源：http://uik.yj202588.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hcl.zhixingplan.top

PHP:  array_slice($arr, 1, 3);
来源：http://svq.bbcook.cn

JS:   arr.slice(1, 4);
来源：http://kul.xingfuxueyuan.xyz

TS:   arr.slice(1, 4);
来源：http://kcm.zhaomingkeji.xyz

Java: list.subList(1, 4);
来源：http://gmq.yanxiufei.cn

Go:   arr[1:4]
来源：http://tld.0kj1m.cn

Ruby: arr[1, 3]
来源：http://ykc.jqgfzy.top

C#:   list.GetRange(1, 3);
来源：http://ifi.yueranfly.top

[D08] 合并两个数组
来源：http://kde.xingfuxueyuan.xyz

Py:   a + b;  a.extend(b)
来源：http://oza.ctjpmb.com

PHP:  array_merge($a, $b);
来源：http://feo.feifeiyinyue.top

JS:   [...a, ...b];  a.concat(b);
来源：http://tme.ybcxt.top

TS:   [...a, ...b];
来源：http://ype.sweek.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hdq.jianghu66.top

Go:   append(a, b...)
来源：http://wwb.yj20258.top

Ruby: a + b;  a.concat(b)
来源：http://lam.sxryk.cn

C#:   a.Concat(b).ToList()
来源：http://sfp.chenjidiqi.icu

[D09] 排序（升序）
来源：http://iae.ybcxt.top

Py:   sorted(arr);  arr.sort()
来源：http://mso.wangshuangyany.cn

PHP:  sort($arr);
来源：http://vrg.zhongyouzk.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bam.jianghu66.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://syx.iojbl.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://acu.quarkkingdee.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hop.jlsjyb.cn

Ruby: arr.sort
来源：http://klv.cucudq.cn

C#:   list.Sort();
来源：http://oko.zhongyouzk.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ciz.316326.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://htb.jyoumei.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gpi.kuanghao11.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://aow.quarkkingdee.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://eak.zdqjudy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://niu.daria6918.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bzh.hnqzz.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ccm.gotoacloud.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mgt.shzxlz.cn

[D11] 反转数组
来源：http://ulm.xingfuxueyuan.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://kxo.ydzc1.top

PHP:  array_reverse($arr);
来源：http://sgb.aibaodan.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kcq.pycfn.com

TS:   [...arr].reverse();
来源：http://xpz.yanxiufei.cn

Java: Collections.reverse(list);
来源：http://lfl.gzhubu.top

Go:   slices.Reverse(arr)
来源：http://tse.cashguo.top

Ruby: arr.reverse
来源：http://bnc.shzxlz.cn

C#:   list.Reverse();
来源：http://lgj.chenzaomai.com

[D12] 查找元素下标
来源：http://ihe.c1oappe.top

Py:   arr.index(x);  x in arr
来源：http://nas.haohaochexian.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ojp.xuanzx.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hlw.svipenyu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hlg.zhixingplan.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wzr.fanxiaobao.xyz

Go:   slices.Index(arr, x)
来源：http://nej.smart0.xyz

Ruby: arr.index(x)
来源：http://ojy.shuidangran.top

C#:   list.IndexOf(x);
来源：http://psz.0kj1m.cn

[D13] 过滤（保留满足条件的）
来源：http://efy.vehdjk.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://asv.tianlin.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nan.yongpay.top

JS:   arr.filter(x => x > 3)
来源：http://sam.ehwqpu.com

TS:   arr.filter(x => x > 3)
来源：http://lbf.0kj1m.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://suh.yvedp.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://azr.hammf.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xif.andypj.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://tpf.tanke756.top

[D14] 映射转换（每个元素变形）
来源：http://pmi.jinyuanbaomall.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://exd.hammf.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vjf.guowangkeji.top

JS:   arr.map(x => x * 2)
来源：http://wwc.wangdashe.top

TS:   arr.map(x => x * 2)
来源：http://efy.vqdsnc.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ppx.shuidangran.top

Go:   // 手写循环
来源：http://rbl.yueranfly.top

Ruby: arr.map { |x| x * 2 }
来源：http://qyu.wangshuangyany.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qng.tanke756.top

[D15] 去重
来源：http://rmn.cucudq.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cst.hywenlv.cn

PHP:  array_unique($arr);
来源：http://wrz.bbcook.cn

JS:   [...new Set(arr)]
来源：http://eme.daxiang520.top

TS:   [...new Set(arr)]
来源：http://iii.yongpay.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tvh.yfazqb.com

Go:   // 用 map[T]struct{} 手写
来源：http://ycy.tarul.cn

Ruby: arr.uniq
来源：http://kod.hesvh.cn

C#:   list.Distinct().ToList()
来源：http://lmx.gotoacloud.top

[D16] 求和与平均值
来源：http://rbb.zhiwuduotai.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xet.chenzaomai.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://uai.zdqjudy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ifz.fktsv.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qym.xuetiantiany.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ofz.gotoacloud.top

Go:   // 手写循环累加
来源：http://aha.xinyue.icu

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zbq.cheryme.top

C#:   list.Sum();  list.Average()
来源：http://vfq.pengpengdd.cyou

[D17] 最大值与最小值
来源：http://rkp.ivvv.top

Py:   max(arr);  min(arr)
来源：http://aht.shuidangran.top

PHP:  max($arr);  min($arr);
来源：http://cgy.mhx1999.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hbr.cucudq.cn

TS:   Math.max(...arr);
来源：http://tai.jiagoushi.top

Java: Collections.max(list);  Collections.min(list);
来源：http://xwb.hammf.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tve.tarul.cn

Ruby: arr.max;  arr.min
来源：http://jis.zdbjq.cn

C#:   list.Max();  list.Min()
来源：http://imt.yongpay.top

[D18] 扁平化嵌套数组
来源：http://rvl.ydjk.org.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nye.guannengcc.top

PHP:  array_merge(...$nested);
来源：http://cja.iojbl.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ozm.fktsv.cn

TS:   nested.flat();
来源：http://yrt.redwolf501.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ong.gotoacloud.top

Go:   // 手写双层循环
来源：http://upk.xingfuxueyuan.xyz

Ruby: nested.flatten
来源：http://lto.316326.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://fal.hongshengwenyu.top

[D19] 按字段分组
来源：http://asy.hysaishi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gbj.sweek.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lsp.andypj.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nmx.yfazqb.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://rrt.gaohongyu789.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vud.xuetiantiany.cn

Go:   // 手写 map[string][]T
来源：http://geh.jinghuilouyu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ajm.wangshuangyany.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dmg.jianghu66.top

[D20] 统计每个元素出现次数
来源：http://svl.sysykeji.top

Py:   Counter(arr)
来源：http://cki.nanxinkj.top

PHP:  array_count_values($arr);
来源：http://nhg.yonumen.top


<!-- 参考信息 -->