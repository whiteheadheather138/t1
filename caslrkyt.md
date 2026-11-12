代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://mlu.xziqi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://guc.yongpay.top

Ruby: def add(a, b); a + b; end
来源：http://zow.yuxming.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qmo.c1oappe.top

[C02] 默认参数
来源：http://noh.yangfankeji.com

Py:   def greet(name="World"): return name
来源：http://afa.0kj1m.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://smh.fehbvm.com

JS:   function greet(name = "World") { return name; }
来源：http://scf.zycfv.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qwd.nanxuanxn.top

Java: // 无默认参数：方法重载或 Optional
来源：http://xuc.pengpengdd.cyou

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qey.aizwys.cn

Ruby: def greet(name = "World") = name
来源：http://vqr.shanyushiyangtech.top

C#:   string Greet(string name = "World") => name;
来源：http://mho.zhixingplan.top

[C03] 可变参数
来源：http://rru.yonumen.top

Py:   def total(*args): return sum(args)
来源：http://tlw.dashuyun.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xdy.zdqjudy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bkk.dashuyun.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ccf.vehdjk.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jut.kuanghao11.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://afl.hnxiangtu.top

Ruby: def total(*nums); nums.sum; end
来源：http://mkr.hesvh.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lgf.hcnkem.com

[C04] 命名参数 / 关键字参数
来源：http://pto.vqdsnc.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ane.fktsv.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pxl.guowangkeji.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wdu.yj202588.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ssu.aizwys.cn

Java: // 无：用 Builder 模式或 record
来源：http://ljc.aizwys.cn

Go:   // 无：用配置结构体参数
来源：http://uyo.mhx1999.top

Ruby: f(a: 1, b: 2)
来源：http://spw.hnqzz.top

C#:   f(a: 1, b: 2)
来源：http://cyk.aibaodan.cn

[C05] 返回多个值
来源：http://jsd.cdnleiting.top

Py:   return a, b
来源：http://hmp.guowangkeji.top

PHP:  return [$a, $b];
来源：http://dfn.sysykeji.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://nqo.jiagoushi.top

TS:   return { a, b };
来源：http://bsl.gogol.net.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://alj.havefunace.top

Go:   return a, b
来源：http://urn.xuanzx.com

Ruby: return a, b
来源：http://lhi.hywenlv.cn

C#:   return (a, b);              // ValueTuple
来源：http://bfj.gzhubu.top

[C06] 匿名函数 / lambda
来源：http://pqb.hesvh.cn

Py:   square = lambda x: x * x
来源：http://epm.ivvv.top

PHP:  $square = fn($x) => $x * $x;
来源：http://jco.ydzc1.top

JS:   const square = x => x * x;
来源：http://yig.zdqjudy.top

TS:   const square = (x: number): number => x * x;
来源：http://qcw.jinqigfzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bls.sysykeji.top

Go:   sq := func(x int) int { return x * x }
来源：http://xau.yangfankeji.com

Ruby: square = ->(x) { x * x }
来源：http://hid.nanxuanxn.top

C#:   Func<int, int> square = x => x * x;
来源：http://jvt.ywan-chungtsiang.top

[C07] 把函数作为参数传入
来源：http://snf.ehwqpu.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sqk.fehbvm.com

PHP:  array_map("strtoupper", $arr);
来源：http://kmk.guannengcc.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rmq.fehbvm.com

TS:   arr.map(String)
来源：http://iem.gogol.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xwn.zhoulong.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://twi.zdqjudy.top

Ruby: arr.map(&:upcase)
来源：http://thk.havefunace.top

C#:   arr.Select(s => s.ToUpper())
来源：http://yqw.daxiang520.top

[C08] 闭包
来源：http://llz.yangfankeji.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nhy.gogol.net.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wev.jinqigufen.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sye.dashuyun.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jve.hnxiangtu.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jit.gaohongyu789.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nyj.mhx1999.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://llf.sufxvd.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://woa.cheryme.top

[C09] 递归
来源：http://tdq.snrcjt.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ifq.jiagoushi.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rxe.9152youxi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qph.yuxming.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mxp.mhx1999.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://exv.pengpengdd.cyou

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hzh.aizwys.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ces.cucudq.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://iyq.hnxiangtu.top

[C10] 变量作用域
来源：http://mjp.shanyushiyangkeji.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vph.ctjpmb.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bba.yuxming.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kmi.jiagoushi.top

TS:   同 JS
来源：http://tbh.uphjek.com

Java: 方法内为块级作用域
来源：http://klm.zhijiandao.cn

Go:   花括号块级作用域
来源：http://etm.ywan-chungtsiang.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gzp.dianchejie.cn

C#:   块级作用域
来源：http://mxi.ivvv.top

[C11] 模块导入与导出
来源：http://uuj.tarul.cn

Py:   from module import func
来源：http://ysb.bjfxy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://tjg.52xcode.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://eaf.mhx1999.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://efg.kuanghao11.cn

Java: import java.util.List;
来源：http://pja.hfpthk.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ler.zhaomingkeji.xyz

Ruby: require "json"; require_relative "./util"
来源：http://cwt.zhoulong.xyz

C#:   using System.Text;
来源：http://zza.yuxming.cn

[C12] 立即执行函数 IIFE
来源：http://kgi.xziqi.cn

Py:   (lambda: print("run"))()
来源：http://hzv.xuetiantiany.cn

PHP:  (function () { echo "run"; })();
来源：http://mut.daria6918.cn

JS:   (() => { console.log("run"); })();
来源：http://lai.guowangkeji.top

TS:   (() => { console.log("run"); })();
来源：http://cmh.redwolf501.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dyt.andypj.xyz

Go:   func() { fmt.Println("run") }()
来源：http://bpb.guowangkeji.top

Ruby: -> { puts "run" }.call
来源：http://mft.yj20258.top

C#:   // 无 IIFE：用静态构造函数
来源：http://zxh.yj202588.top

[C13] 类型声明 / 类型注解
来源：http://jwm.quarkkingdee.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jfs.shzxlz.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jqz.ppjwa.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mls.mhx1999.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xul.yj202588.top

Java: int add(int a, int b) { return a + b; }
来源：http://llu.sweek.top

Go:   func add(a, b int) int
来源：http://bvq.dashuyun.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://oet.xuetiantiany.cn

C#:   int Add(int a, int b) => a + b;
来源：http://alj.zdbjq.cn

[C14] 泛型函数
来源：http://thk.jyoumei.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vvl.svipenyu.cn

PHP:  // 无泛型
来源：http://ltb.havefunace.top

JS:   // 无泛型
来源：http://squ.c1oappe.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pqr.yvedp.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jqy.yanxiufei.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qmg.nwbrower.top

Ruby: # 无泛型
来源：http://fpn.xuanzx.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zhe.jinqigfzy.top

[C15] 解构 / 展开参数
来源：http://sam.cashguo.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cjn.fengsongda.top

PHP:  [$a, $b] = $pair;
来源：http://orr.yj20258888.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hem.shangyingyoupin.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://unq.cucudq.cn

Java: // 无解构
来源：http://soe.nanxuanxn.top

Go:   // 无解构
来源：http://vml.tanke756.top

Ruby: a, b = pair
来源：http://bxh.uphjek.com

C#:   var (a, b) = pair;
来源：http://vjl.uphjek.com

[C16] 函数 / 方法重载
来源：http://gty.tian-w.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yws.bjfxy.top

PHP:  // 无重载
来源：http://raz.shuidangran.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ysj.jinyuanbaomall.cn

TS:   // 用联合类型或重载签名声明
来源：http://vgc.sweek.top

Java: void f(int a) {}  void f(String a) {}
来源：http://zzo.vehdjk.com

Go:   // 无重载：用不同函数名
来源：http://gqk.gaohongyu789.top

Ruby: # 无重载：靠动态参数
来源：http://lep.guannengcc.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://lrr.hywenlv.cn

================================================================================
来源：http://itn.c1oappe.top

D. 数组 / 列表 / 集合
来源：http://pyo.jyoumei.cn

================================================================================
来源：http://rmk.hysaishi.cn

[D01] 创建数组 / 列表
来源：http://wyv.zhongyouzk.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://cin.chenjidiqi.icu

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yrb.hnxiangtu.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zjk.yfazqb.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://isc.yuxming.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yaq.fzhhl.top

Go:   arr := []int{1, 2, 3}
来源：http://sld.xziqi.cn

Ruby: arr = [1, 2, 3]
来源：http://nbn.zhixingplan.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://viw.zdbjq.cn

[D02] 追加元素到末尾
来源：http://qkh.vqdsnc.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://iml.zhongyouzk.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ueq.hongshengwenyu.top

JS:   arr.push(4);
来源：http://yod.jinqigufen.top

TS:   arr.push(4);
来源：http://fbv.gzhubu.top

Java: list.add(4);
来源：http://lvu.ivvv.top

Go:   arr = append(arr, 4)
来源：http://gfd.zhixingplan.top

Ruby: arr << 4; arr.push(5)
来源：http://ege.cashguo.top

C#:   list.Add(4);
来源：http://xiz.ydzc1.top

[D03] 在指定位置插入元素
来源：http://itf.fanxiaobao.xyz

Py:   arr.insert(0, 0)
来源：http://wqq.xuanzx.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mmp.yanxiufei.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://npr.jyoumei.cn

TS:   arr.splice(0, 0, 0);
来源：http://mpi.shanyushiyangtech.top

Java: list.add(0, 0);
来源：http://kxi.hammf.cn

Go:   arr = append([]int{0}, arr...)
来源：http://zgz.tanke756.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://aeb.gzhubu.top

C#:   list.Insert(0, 0);
来源：http://nos.tanke756.top

[D04] 删除元素
来源：http://sex.gogol.net.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://oqv.shzxlz.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kru.havefunace.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://emd.bjfxy.top

TS:   arr.splice(0, 1);
来源：http://jqd.fehbvm.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pml.yj20258.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bns.ehwqpu.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qtt.xylfe.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pij.mhx1999.top

[D05] 访问与修改元素
来源：http://gig.zhixingplan.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xcr.cheryme.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ynm.gzhubu.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mgn.9152youxi.cn

TS:   arr[0]; arr.at(-1);
来源：http://pxp.zhongyouzk.top

Java: list.get(0); list.set(0, 9);
来源：http://ezu.chenjidiqi.icu

Go:   arr[0]; arr[0] = 9
来源：http://xgl.ctjpmb.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://atz.cheryme.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xmy.yanxiufei.cn

[D06] 数组长度
来源：http://yxj.wangdashe.top

Py:   len(arr)
来源：http://bqh.redwolf501.top

PHP:  count($arr);
来源：http://eyw.yvedp.cn

JS:   arr.length
来源：http://ceq.shangyingyoupin.top

TS:   arr.length
来源：http://ehn.fzhhl.top

Java: list.size();
来源：http://ukl.smart0.xyz

Go:   len(arr)
来源：http://zdy.hesvh.cn

Ruby: arr.length; arr.size
来源：http://bzu.epnwcf.com

C#:   list.Count;
来源：http://rmu.zhijiandao.cn

[D07] 切片 / 取子数组
来源：http://kyt.redwolf501.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xso.quarkkingdee.top

PHP:  array_slice($arr, 1, 3);
来源：http://yzv.zhiwuduotai.top

JS:   arr.slice(1, 4);
来源：http://zzc.yj20258.top

TS:   arr.slice(1, 4);
来源：http://gze.zhengqikj.top

Java: list.subList(1, 4);
来源：http://ghf.havefunace.top

Go:   arr[1:4]
来源：http://ceq.kuanghao11.cn

Ruby: arr[1, 3]
来源：http://vms.yonumen.top

C#:   list.GetRange(1, 3);
来源：http://ggo.ivvv.top

[D08] 合并两个数组
来源：http://lay.jqgufenzy.top

Py:   a + b;  a.extend(b)
来源：http://itu.pycfn.com

PHP:  array_merge($a, $b);
来源：http://eri.dianchejie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://eki.ehwqpu.com

TS:   [...a, ...b];
来源：http://mxa.jqgfzy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kgu.iojbl.cn

Go:   append(a, b...)
来源：http://bbr.cucudq.cn

Ruby: a + b;  a.concat(b)
来源：http://ssy.hcnkem.com

C#:   a.Concat(b).ToList()
来源：http://qno.cheryme.top

[D09] 排序（升序）
来源：http://hwg.iojbl.cn

Py:   sorted(arr);  arr.sort()
来源：http://sto.jqgfzy.top

PHP:  sort($arr);
来源：http://oul.hywenlv.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rhd.guannengcc.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://pkc.hnxiangtu.top

Java: Collections.sort(list);  list.sort(null);
来源：http://zbi.jqgufenzy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jkj.fehbvm.com

Ruby: arr.sort
来源：http://okg.yongpay.top

C#:   list.Sort();
来源：http://ros.ivvv.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://wei.smart0.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cqu.svipenyu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://izl.bbcook.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ktx.dianchejie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vrf.epnwcf.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vqt.jinyuanbaomall.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ffy.fzhhl.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wtu.gotoacloud.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tnd.hywenlv.cn

[D11] 反转数组
来源：http://cxm.fehbvm.com

Py:   arr[::-1];  arr.reverse()
来源：http://ayj.yuxming.cn

PHP:  array_reverse($arr);
来源：http://hwz.jinqigufen.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://poi.zhiwuduotai.top

TS:   [...arr].reverse();
来源：http://vpk.shzxlz.cn

Java: Collections.reverse(list);
来源：http://bsq.jinqigufen.top

Go:   slices.Reverse(arr)
来源：http://vqh.meibo888.top

Ruby: arr.reverse
来源：http://ojw.xuetiantiany.cn

C#:   list.Reverse();
来源：http://dee.chenjidiqi.icu

[D12] 查找元素下标
来源：http://isz.yonumen.top

Py:   arr.index(x);  x in arr
来源：http://yjq.feifeiyinyue.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://aac.yvedp.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cia.smart0.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sdk.nwbrower.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dkt.yj202588.top

Go:   slices.Index(arr, x)
来源：http://jnw.yj20258.top

Ruby: arr.index(x)
来源：http://bif.hysaishi.cn

C#:   list.IndexOf(x);
来源：http://pqu.ywan-chungtsiang.top

[D13] 过滤（保留满足条件的）
来源：http://ito.316326.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qvl.snrcjt.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vsg.shuidangran.top

JS:   arr.filter(x => x > 3)
来源：http://ocy.fehbvm.com

TS:   arr.filter(x => x > 3)
来源：http://kgf.shanyushiyangtech.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wix.zhengqikj.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ats.meibo888.top

Ruby: arr.select { |x| x > 3 }
来源：http://tug.gogol.net.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://lio.yvedp.cn

[D14] 映射转换（每个元素变形）
来源：http://dxh.xuetiantiany.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rmm.shanyushiyangkeji.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jwq.ybcxt.top

JS:   arr.map(x => x * 2)
来源：http://oyg.yonumen.top

TS:   arr.map(x => x * 2)
来源：http://ylz.quarkkingdee.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://zum.iojbl.cn

Go:   // 手写循环
来源：http://ycp.yonumen.top

Ruby: arr.map { |x| x * 2 }
来源：http://xvo.tanke756.top

C#:   list.Select(x => x * 2).ToList()
来源：http://uja.zhengqikj.top

[D15] 去重
来源：http://tfx.guannengcc.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sfq.snrcjt.cn

PHP:  array_unique($arr);
来源：http://htp.andypj.xyz

JS:   [...new Set(arr)]
来源：http://ism.mhx1999.top

TS:   [...new Set(arr)]
来源：http://xov.c1oappe.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fxu.birdmap.top

Go:   // 用 map[T]struct{} 手写
来源：http://swr.tianlin.xyz

Ruby: arr.uniq
来源：http://gcc.shuidangran.top

C#:   list.Distinct().ToList()
来源：http://qvn.zhoulong.xyz

[D16] 求和与平均值
来源：http://jno.birdmap.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dvu.feifeiyinyue.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hhv.xylfe.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pxj.yuanzhike.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nok.jyoumei.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sjp.meibo888.top

Go:   // 手写循环累加
来源：http://flp.ydjk.org.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hev.iojbl.cn

C#:   list.Sum();  list.Average()
来源：http://ppi.tian-w.cn

[D17] 最大值与最小值
来源：http://gzd.zdqjudy.top

Py:   max(arr);  min(arr)
来源：http://mdc.hywenlv.cn

PHP:  max($arr);  min($arr);
来源：http://nhz.cdnleiting.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rlo.ehwqpu.com

TS:   Math.max(...arr);
来源：http://qlt.aizwys.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://jlx.jinqigfzy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nww.zhixingplan.top

Ruby: arr.max;  arr.min
来源：http://jiu.andypj.xyz

C#:   list.Max();  list.Min()
来源：http://nsx.zhengqikj.top

[D18] 扁平化嵌套数组
来源：http://ust.xinyue.icu

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nvr.bbcook.cn

PHP:  array_merge(...$nested);
来源：http://dxd.xuetiantiany.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fel.xuanzx.com

TS:   nested.flat();
来源：http://cks.feifeiyinyue.top


<!-- 参考信息 -->