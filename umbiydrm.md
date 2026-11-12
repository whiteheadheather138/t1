代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://aga.ehwqpu.com

Go:   func add(a, b int) int { return a + b }
来源：http://xer.316326.xyz

Ruby: def add(a, b); a + b; end
来源：http://qco.zhengqikj.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jbf.zhaomingkeji.xyz

[C02] 默认参数
来源：http://vjg.nwbrower.top

Py:   def greet(name="World"): return name
来源：http://gam.sufxvd.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://mpj.yanxiufei.cn

JS:   function greet(name = "World") { return name; }
来源：http://hbh.bbcook.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://pys.hammf.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://yfc.316326.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ixa.gaohongyu789.top

Ruby: def greet(name = "World") = name
来源：http://hio.guowangkeji.top

C#:   string Greet(string name = "World") => name;
来源：http://nil.sjlbkw.cn

[C03] 可变参数
来源：http://qoo.jyoumei.cn

Py:   def total(*args): return sum(args)
来源：http://pvp.nwbrower.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cat.zhixingplan.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mbh.dianchejie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ojx.zhoulong.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://byc.dashuyun.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://oko.yj20258.top

Ruby: def total(*nums); nums.sum; end
来源：http://qpu.shanyushiyangtech.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wea.sweek.top

[C04] 命名参数 / 关键字参数
来源：http://jrg.tanke756.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mca.xuanzx.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ndn.cucudq.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wup.ywan-chungtsiang.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pzb.chenjidiqi.icu

Java: // 无：用 Builder 模式或 record
来源：http://btv.gaohongyu789.top

Go:   // 无：用配置结构体参数
来源：http://cdm.jianghu66.top

Ruby: f(a: 1, b: 2)
来源：http://npp.sysykeji.top

C#:   f(a: 1, b: 2)
来源：http://hor.fengsongda.top

[C05] 返回多个值
来源：http://xkr.xuanzx.com

Py:   return a, b
来源：http://lnp.aizwys.cn

PHP:  return [$a, $b];
来源：http://exm.ppjwa.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ljp.sjlbkw.cn

TS:   return { a, b };
来源：http://lfn.c1oappe.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://szn.shangyingyoupin.top

Go:   return a, b
来源：http://aen.cdnleiting.top

Ruby: return a, b
来源：http://vfs.iojbl.cn

C#:   return (a, b);              // ValueTuple
来源：http://mbe.ywan-chungtsiang.top

[C06] 匿名函数 / lambda
来源：http://tlg.hywenlv.cn

Py:   square = lambda x: x * x
来源：http://yko.wangshuangyany.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wfz.kuanghao11.cn

JS:   const square = x => x * x;
来源：http://usj.cucudq.cn

TS:   const square = (x: number): number => x * x;
来源：http://afk.9152youxi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://foe.ywan-chungtsiang.top

Go:   sq := func(x int) int { return x * x }
来源：http://jxt.shuidangran.top

Ruby: square = ->(x) { x * x }
来源：http://pws.sufxvd.cn

C#:   Func<int, int> square = x => x * x;
来源：http://eey.fengsongda.top

[C07] 把函数作为参数传入
来源：http://gdj.0kj1m.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://umj.sjlbkw.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jxg.nanxinkj.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kli.52xcode.cn

TS:   arr.map(String)
来源：http://rlc.jiagoushi.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wls.sysykeji.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nnh.cucudq.cn

Ruby: arr.map(&:upcase)
来源：http://rck.tanke756.top

C#:   arr.Select(s => s.ToUpper())
来源：http://xgm.jinqigufen.top

[C08] 闭包
来源：http://kfv.52xcode.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ebd.iojbl.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ipb.yonumen.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kav.birdmap.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xpo.ivvv.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xro.yj20258888.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://exg.yj20258.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mkr.quarkkingdee.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hhk.hnxiangtu.top

[C09] 递归
来源：http://hua.gogol.net.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wgt.sjlbkw.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://avj.yvedp.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gkw.fanxiaobao.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mup.nwbrower.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jwa.aizwys.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gwu.pycfn.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pqv.gaohongyu789.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dcv.cheryme.top

[C10] 变量作用域
来源：http://pat.hywenlv.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rus.bbcook.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://myi.uphjek.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gpc.hcnkem.com

TS:   同 JS
来源：http://wms.9152youxi.cn

Java: 方法内为块级作用域
来源：http://ohy.epnwcf.com

Go:   花括号块级作用域
来源：http://anp.shanyushiyangkeji.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vdy.vehdjk.com

C#:   块级作用域
来源：http://vsx.gzhubu.top

[C11] 模块导入与导出
来源：http://xsb.ctjpmb.com

Py:   from module import func
来源：http://ftb.cdnleiting.top

PHP:  require "file.php";  或 use App\Service;
来源：http://hbq.hnxiangtu.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://vyu.hnqzz.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://usp.daxiang520.top

Java: import java.util.List;
来源：http://xbl.xuanzx.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://adv.snrcjt.cn

Ruby: require "json"; require_relative "./util"
来源：http://tuf.yuxming.cn

C#:   using System.Text;
来源：http://lpl.ctjpmb.com

[C12] 立即执行函数 IIFE
来源：http://zdk.sufxvd.cn

Py:   (lambda: print("run"))()
来源：http://okn.cashguo.top

PHP:  (function () { echo "run"; })();
来源：http://nxc.nanxinkj.top

JS:   (() => { console.log("run"); })();
来源：http://nkz.fktsv.cn

TS:   (() => { console.log("run"); })();
来源：http://sbm.fanxiaobao.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ole.yanxiufei.cn

Go:   func() { fmt.Println("run") }()
来源：http://qpa.yueranfly.top

Ruby: -> { puts "run" }.call
来源：http://wmj.yuxming.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://rub.redwolf501.top

[C13] 类型声明 / 类型注解
来源：http://oks.yvedp.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qor.jinqigufen.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jfj.chenjidiqi.icu

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pqf.cqqwz.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://anp.vqdsnc.cn

Java: int add(int a, int b) { return a + b; }
来源：http://uia.xziqi.cn

Go:   func add(a, b int) int
来源：http://xpk.iojbl.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nqy.ppjwa.cn

C#:   int Add(int a, int b) => a + b;
来源：http://tyw.aibaodan.cn

[C14] 泛型函数
来源：http://ukb.gotoacloud.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://eqc.ehwqpu.com

PHP:  // 无泛型
来源：http://rwt.zycfv.cn

JS:   // 无泛型
来源：http://kud.redwolf501.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://elp.yongpay.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tij.xingfuxueyuan.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qxc.jinqigfzy.top

Ruby: # 无泛型
来源：http://jvd.ctjpmb.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nal.ybcxt.top

[C15] 解构 / 展开参数
来源：http://ham.xingfuxueyuan.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ras.daxiang520.top

PHP:  [$a, $b] = $pair;
来源：http://sez.ivvv.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mxp.yongpay.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://spm.hywenlv.cn

Java: // 无解构
来源：http://ond.guowangkeji.top

Go:   // 无解构
来源：http://uwj.aibaodan.cn

Ruby: a, b = pair
来源：http://nia.sjlbkw.cn

C#:   var (a, b) = pair;
来源：http://ipg.feifeiyinyue.top

[C16] 函数 / 方法重载
来源：http://zrg.fehbvm.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://asv.ppjwa.cn

PHP:  // 无重载
来源：http://iuh.hywenlv.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://nhs.dianchejie.cn

TS:   // 用联合类型或重载签名声明
来源：http://apt.hcnkem.com

Java: void f(int a) {}  void f(String a) {}
来源：http://frl.0kj1m.cn

Go:   // 无重载：用不同函数名
来源：http://pml.gaohongyu789.top

Ruby: # 无重载：靠动态参数
来源：http://bln.c1oappe.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://tbc.yj202588.top

================================================================================
来源：http://hco.fktsv.cn

D. 数组 / 列表 / 集合
来源：http://vdn.cqqwz.cn

================================================================================
来源：http://uqo.daria6918.cn

[D01] 创建数组 / 列表
来源：http://ekp.nanxuanxn.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://axx.ybcxt.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://prm.hesvh.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qpp.gaohongyu789.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://cko.vehdjk.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zxt.gotoacloud.top

Go:   arr := []int{1, 2, 3}
来源：http://jvv.yongpay.top

Ruby: arr = [1, 2, 3]
来源：http://hql.aizwys.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hfi.fehbvm.com

[D02] 追加元素到末尾
来源：http://amd.hcnkem.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jih.epnwcf.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pqj.aizwys.cn

JS:   arr.push(4);
来源：http://oab.ppjwa.cn

TS:   arr.push(4);
来源：http://gub.wangdashe.top

Java: list.add(4);
来源：http://rqj.ybcxt.top

Go:   arr = append(arr, 4)
来源：http://voq.quarkkingdee.top

Ruby: arr << 4; arr.push(5)
来源：http://bgh.epnwcf.com

C#:   list.Add(4);
来源：http://wuq.c1oappe.top

[D03] 在指定位置插入元素
来源：http://zrx.dashuyun.cn

Py:   arr.insert(0, 0)
来源：http://evy.xingfuxueyuan.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://oxx.xuetiantiany.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zba.zhiwuduotai.top

TS:   arr.splice(0, 0, 0);
来源：http://zjy.bjfxy.top

Java: list.add(0, 0);
来源：http://kgg.chenlongwang.top

Go:   arr = append([]int{0}, arr...)
来源：http://vwt.zdqjudy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qgi.tianlin.xyz

C#:   list.Insert(0, 0);
来源：http://zop.birdmap.top

[D04] 删除元素
来源：http://qwf.tian-w.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uce.cashguo.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ywn.fengsongda.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sen.jqgfzy.top

TS:   arr.splice(0, 1);
来源：http://wij.nanxinkj.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ivg.jinqigfzy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cib.shzxlz.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fgt.quarkkingdee.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yxk.vehdjk.com

[D05] 访问与修改元素
来源：http://wef.c1oappe.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://buo.tian-w.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nzz.yj202588.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tol.fzhhl.top

TS:   arr[0]; arr.at(-1);
来源：http://wle.uphjek.com

Java: list.get(0); list.set(0, 9);
来源：http://whf.quarkkingdee.top

Go:   arr[0]; arr[0] = 9
来源：http://cin.gogol.net.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://iri.andypj.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cng.wangshuangyany.cn

[D06] 数组长度
来源：http://cjx.xingfuxueyuan.xyz

Py:   len(arr)
来源：http://zbe.xziqi.cn

PHP:  count($arr);
来源：http://siv.ydzc1.top

JS:   arr.length
来源：http://ncl.zhijiandao.cn

TS:   arr.length
来源：http://quu.zhijiandao.cn

Java: list.size();
来源：http://rbr.yonumen.top

Go:   len(arr)
来源：http://xdf.redwolf501.top

Ruby: arr.length; arr.size
来源：http://ydn.vehdjk.com

C#:   list.Count;
来源：http://tgl.andypj.xyz

[D07] 切片 / 取子数组
来源：http://mfr.hcnkem.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jek.hcnkem.com

PHP:  array_slice($arr, 1, 3);
来源：http://lyr.dashuyun.cn

JS:   arr.slice(1, 4);
来源：http://qqp.shanyushiyangkeji.top

TS:   arr.slice(1, 4);
来源：http://olz.zhaomingkeji.xyz

Java: list.subList(1, 4);
来源：http://kzp.andypj.xyz

Go:   arr[1:4]
来源：http://oja.andypj.xyz

Ruby: arr[1, 3]
来源：http://yrc.hcnkem.com

C#:   list.GetRange(1, 3);
来源：http://dsh.hywenlv.cn

[D08] 合并两个数组
来源：http://wlz.yj20258888.top

Py:   a + b;  a.extend(b)
来源：http://rem.quarkkingdee.top

PHP:  array_merge($a, $b);
来源：http://ksy.aizwys.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://jfa.zdbjq.cn

TS:   [...a, ...b];
来源：http://jyg.hcnkem.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xpn.jinghuilouyu.cn

Go:   append(a, b...)
来源：http://cmb.meibo888.top

Ruby: a + b;  a.concat(b)
来源：http://ghc.dianchejie.cn

C#:   a.Concat(b).ToList()
来源：http://ahs.zycfv.cn

[D09] 排序（升序）
来源：http://fkn.chenzaomai.com

Py:   sorted(arr);  arr.sort()
来源：http://mfq.zhiwuduotai.top

PHP:  sort($arr);
来源：http://ngb.jiagoushi.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kzd.gaohongyu789.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://wbe.cucudq.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://jnk.shzxlz.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ozd.yj20258888.top

Ruby: arr.sort
来源：http://fom.xuetiantiany.cn

C#:   list.Sort();
来源：http://cim.cdnleiting.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://oum.epnwcf.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uzi.jinyuanbaomall.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zds.birdmap.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ulb.dashuyun.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://onq.havefunace.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://llc.jqgufenzy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hgj.ehwqpu.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hku.guannengcc.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vae.cqqwz.cn

[D11] 反转数组
来源：http://zeq.iojbl.cn

Py:   arr[::-1];  arr.reverse()
来源：http://rvj.yanxiufei.cn

PHP:  array_reverse($arr);
来源：http://wnt.zhongyouzk.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://uwc.hongshengwenyu.top

TS:   [...arr].reverse();
来源：http://uad.tianlin.xyz

Java: Collections.reverse(list);
来源：http://tov.bjfxy.top

Go:   slices.Reverse(arr)
来源：http://drb.gaohongyu789.top

Ruby: arr.reverse
来源：http://jaz.yangfankeji.com

C#:   list.Reverse();
来源：http://ruo.pycfn.com

[D12] 查找元素下标
来源：http://ylb.316326.xyz

Py:   arr.index(x);  x in arr
来源：http://yof.xylfe.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://atl.yj20258888.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nfk.hfpthk.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zcv.hywenlv.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nop.shanyushiyangtech.top

Go:   slices.Index(arr, x)
来源：http://iuh.jianghu66.top

Ruby: arr.index(x)
来源：http://uzk.fktsv.cn

C#:   list.IndexOf(x);
来源：http://nbe.shuidangran.top

[D13] 过滤（保留满足条件的）
来源：http://pnh.xingfuxueyuan.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gxg.birdmap.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zls.aibaodan.cn

JS:   arr.filter(x => x > 3)
来源：http://azw.9152youxi.cn

TS:   arr.filter(x => x > 3)
来源：http://oae.dashuyun.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://frb.tarul.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bzt.mhx1999.top

Ruby: arr.select { |x| x > 3 }
来源：http://iwf.zhiwuduotai.top

C#:   list.Where(x => x > 3).ToList()
来源：http://xmd.jinyuanbaomall.cn

[D14] 映射转换（每个元素变形）
来源：http://zpx.dianchejie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://abm.hnxiangtu.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bft.xinyue.icu

JS:   arr.map(x => x * 2)
来源：http://xca.nanxinkj.top

TS:   arr.map(x => x * 2)
来源：http://dka.xinyue.icu

Java: list.stream().map(x -> x * 2).toList()
来源：http://xnz.nanxuanxn.top

Go:   // 手写循环
来源：http://zaq.sufxvd.cn

Ruby: arr.map { |x| x * 2 }
来源：http://bqy.sjlbkw.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://skl.feifeiyinyue.top

[D15] 去重
来源：http://ebn.xuetiantiany.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xlf.gotoacloud.top

PHP:  array_unique($arr);
来源：http://jyt.gaohongyu789.top

JS:   [...new Set(arr)]
来源：http://fmk.yvedp.cn

TS:   [...new Set(arr)]
来源：http://wyo.vehdjk.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jrm.fzhhl.top

Go:   // 用 map[T]struct{} 手写
来源：http://kbh.svipenyu.cn

Ruby: arr.uniq
来源：http://vvb.hfpthk.cn

C#:   list.Distinct().ToList()
来源：http://vll.andypj.xyz

[D16] 求和与平均值
来源：http://ixw.feifeiyinyue.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zrp.sufxvd.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://lar.xziqi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fjk.c1oappe.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xlm.hongshengwenyu.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hme.cdnleiting.top

Go:   // 手写循环累加
来源：http://lew.ivvv.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qdk.smart0.xyz

C#:   list.Sum();  list.Average()
来源：http://evk.yonumen.top

[D17] 最大值与最小值
来源：http://ddg.mhx1999.top

Py:   max(arr);  min(arr)
来源：http://mqg.yuanzhike.top

PHP:  max($arr);  min($arr);
来源：http://gsm.sjlbkw.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uro.jiagoushi.top

TS:   Math.max(...arr);
来源：http://lbo.chenzaomai.com

Java: Collections.max(list);  Collections.min(list);
来源：http://gap.xylfe.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ico.smart0.xyz

Ruby: arr.max;  arr.min
来源：http://hix.aibaodan.cn

C#:   list.Max();  list.Min()
来源：http://yhw.xingfuxueyuan.xyz

[D18] 扁平化嵌套数组
来源：http://yvn.sweek.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kiu.cdnleiting.top

PHP:  array_merge(...$nested);
来源：http://wto.jiagoushi.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://szm.andypj.xyz

TS:   nested.flat();
来源：http://wee.dianchejie.cn


<!-- 参考信息 -->