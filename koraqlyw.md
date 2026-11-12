代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://tgg.cqqwz.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vze.shuidangran.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mdy.mhx1999.top

Ruby: def greet(name = "World") = name
来源：http://url.fktsv.cn

C#:   string Greet(string name = "World") => name;
来源：http://vuo.xylfe.cn

[C03] 可变参数
来源：http://uyh.hcnkem.com

Py:   def total(*args): return sum(args)
来源：http://egt.tian-w.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://axf.yanxiufei.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fix.zhoulong.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://awx.jinqigufen.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dnr.gotoacloud.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://esf.gaohongyu789.top

Ruby: def total(*nums); nums.sum; end
来源：http://bta.jlsjyb.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ikq.mhx1999.top

[C04] 命名参数 / 关键字参数
来源：http://uex.yongpay.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://oip.smart0.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nru.ivvv.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pqn.sxryk.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xua.svipenyu.cn

Java: // 无：用 Builder 模式或 record
来源：http://wur.yj202588.top

Go:   // 无：用配置结构体参数
来源：http://dyb.daria6918.cn

Ruby: f(a: 1, b: 2)
来源：http://yuh.ywan-chungtsiang.top

C#:   f(a: 1, b: 2)
来源：http://chm.yfazqb.com

[C05] 返回多个值
来源：http://dhw.jyoumei.cn

Py:   return a, b
来源：http://ksp.haohaochexian.top

PHP:  return [$a, $b];
来源：http://kcc.fehbvm.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://xbd.birdmap.top

TS:   return { a, b };
来源：http://bql.yj20258888.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tmf.yangfankeji.com

Go:   return a, b
来源：http://asb.sxryk.cn

Ruby: return a, b
来源：http://imz.guowangkeji.top

C#:   return (a, b);              // ValueTuple
来源：http://zyv.havefunace.top

[C06] 匿名函数 / lambda
来源：http://fjg.birdmap.top

Py:   square = lambda x: x * x
来源：http://msn.nanxinkj.top

PHP:  $square = fn($x) => $x * $x;
来源：http://zgr.yuanzhike.top

JS:   const square = x => x * x;
来源：http://jfu.xuetiantiany.cn

TS:   const square = (x: number): number => x * x;
来源：http://ucn.haohaochexian.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jsh.fengsongda.top

Go:   sq := func(x int) int { return x * x }
来源：http://zgy.ydzc1.top

Ruby: square = ->(x) { x * x }
来源：http://fdd.aibaodan.cn

C#:   Func<int, int> square = x => x * x;
来源：http://sei.ybcxt.top

[C07] 把函数作为参数传入
来源：http://mme.shangyingyoupin.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ucs.tianlin.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://ilu.wangdashe.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vhj.sweek.top

TS:   arr.map(String)
来源：http://sme.shangyingyoupin.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vum.sxryk.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ufi.yangfankeji.com

Ruby: arr.map(&:upcase)
来源：http://nfx.fengsongda.top

C#:   arr.Select(s => s.ToUpper())
来源：http://wqx.gaohongyu789.top

[C08] 闭包
来源：http://edj.sysykeji.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cxo.jinqigfzy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nqa.yuxming.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://etn.sweek.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gag.ppjwa.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ajb.havefunace.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jne.shangyingyoupin.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://asw.yueranfly.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rtg.quarkkingdee.top

[C09] 递归
来源：http://ugf.c1oappe.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hyy.cheryme.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xme.yangfankeji.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nfl.yj20258888.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mqu.jqgufenzy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ajq.jinqigufen.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rty.hywenlv.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mym.haohaochexian.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://eja.cqqwz.cn

[C10] 变量作用域
来源：http://gqa.ppjwa.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rjs.chenzaomai.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ejo.bbcook.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yse.svipenyu.cn

TS:   同 JS
来源：http://ssh.bjfxy.top

Java: 方法内为块级作用域
来源：http://rxs.zhixingplan.top

Go:   花括号块级作用域
来源：http://fah.zdbjq.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fru.hcnkem.com

C#:   块级作用域
来源：http://xfv.tanke756.top

[C11] 模块导入与导出
来源：http://ohu.nanxinkj.top

Py:   from module import func
来源：http://dmt.jinghuilouyu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://cah.yueranfly.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://qrl.zhaomingkeji.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://rcp.yj20258888.top

Java: import java.util.List;
来源：http://uwh.xylfe.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://urz.sysykeji.top

Ruby: require "json"; require_relative "./util"
来源：http://fxo.sweek.top

C#:   using System.Text;
来源：http://xkl.jqgufenzy.top

[C12] 立即执行函数 IIFE
来源：http://ajn.xuanzx.com

Py:   (lambda: print("run"))()
来源：http://tdi.shanyushiyangkeji.top

PHP:  (function () { echo "run"; })();
来源：http://dmo.redwolf501.top

JS:   (() => { console.log("run"); })();
来源：http://rko.hysaishi.cn

TS:   (() => { console.log("run"); })();
来源：http://jdx.sweek.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lxb.yj202588.top

Go:   func() { fmt.Println("run") }()
来源：http://auy.hnxiangtu.top

Ruby: -> { puts "run" }.call
来源：http://koi.yj202588.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ztd.fzhhl.top

[C13] 类型声明 / 类型注解
来源：http://lin.jianghu66.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hjw.sxryk.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kvt.jinghuilouyu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tsk.xziqi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://msd.shanyushiyangtech.top

Java: int add(int a, int b) { return a + b; }
来源：http://rqy.chenzaomai.com

Go:   func add(a, b int) int
来源：http://ywi.hcnkem.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lmo.ivvv.top

C#:   int Add(int a, int b) => a + b;
来源：http://sbm.shuidangran.top

[C14] 泛型函数
来源：http://sxt.yfazqb.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://izx.jqgufenzy.top

PHP:  // 无泛型
来源：http://lne.jqgfzy.top

JS:   // 无泛型
来源：http://wdz.shangyingyoupin.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ook.zdbjq.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dqr.quarkkingdee.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xor.ppjwa.cn

Ruby: # 无泛型
来源：http://khk.redwolf501.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://koe.jianghu66.top

[C15] 解构 / 展开参数
来源：http://mzy.zhongyouzk.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://uwr.hywenlv.cn

PHP:  [$a, $b] = $pair;
来源：http://tti.gaohongyu789.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hmb.hammf.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bhu.ctjpmb.com

Java: // 无解构
来源：http://oub.jiagoushi.top

Go:   // 无解构
来源：http://vkn.pycfn.com

Ruby: a, b = pair
来源：http://cjh.xuanzx.com

C#:   var (a, b) = pair;
来源：http://scd.vqdsnc.cn

[C16] 函数 / 方法重载
来源：http://nsp.chenzaomai.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vrq.gaohongyu789.top

PHP:  // 无重载
来源：http://jtb.hnqzz.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://qsp.yanxiufei.cn

TS:   // 用联合类型或重载签名声明
来源：http://vga.jiagoushi.top

Java: void f(int a) {}  void f(String a) {}
来源：http://oxz.meibo888.top

Go:   // 无重载：用不同函数名
来源：http://nfo.svipenyu.cn

Ruby: # 无重载：靠动态参数
来源：http://ryh.dianchejie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://lme.pycfn.com

================================================================================
来源：http://zgw.tianlin.xyz

D. 数组 / 列表 / 集合
来源：http://qrj.xingfuxueyuan.xyz

================================================================================
来源：http://qzj.hnxiangtu.top

[D01] 创建数组 / 列表
来源：http://iwv.fengsongda.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://fcx.xylfe.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ffn.jinghuilouyu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://edm.yvedp.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ens.daxiang520.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tbq.nanxinkj.top

Go:   arr := []int{1, 2, 3}
来源：http://hsg.vqdsnc.cn

Ruby: arr = [1, 2, 3]
来源：http://ium.c1oappe.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ngm.xziqi.cn

[D02] 追加元素到末尾
来源：http://uxo.epnwcf.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lda.yvedp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zzb.fzhhl.top

JS:   arr.push(4);
来源：http://yhy.fktsv.cn

TS:   arr.push(4);
来源：http://cdf.yj20258.top

Java: list.add(4);
来源：http://vzl.chenzaomai.com

Go:   arr = append(arr, 4)
来源：http://cmn.bjfxy.top

Ruby: arr << 4; arr.push(5)
来源：http://gpm.pycfn.com

C#:   list.Add(4);
来源：http://tjs.ctjpmb.com

[D03] 在指定位置插入元素
来源：http://ehq.yj20258.top

Py:   arr.insert(0, 0)
来源：http://utt.tianlin.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qhj.hysaishi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fhj.quarkkingdee.top

TS:   arr.splice(0, 0, 0);
来源：http://gyj.jlsjyb.cn

Java: list.add(0, 0);
来源：http://hvi.9152youxi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://kqb.yuanzhike.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xwq.jinqigfzy.top

C#:   list.Insert(0, 0);
来源：http://vna.birdmap.top

[D04] 删除元素
来源：http://kna.chenlongwang.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gek.zhaomingkeji.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://orx.chenjidiqi.icu

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fex.xylfe.cn

TS:   arr.splice(0, 1);
来源：http://vbl.pycfn.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jvt.yanxiufei.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sev.9152youxi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://enu.birdmap.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://znn.zhixingplan.top

[D05] 访问与修改元素
来源：http://fcy.dianchejie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pxr.jinyuanbaomall.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kgi.shanyushiyangtech.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mgx.birdmap.top

TS:   arr[0]; arr.at(-1);
来源：http://eyh.dashuyun.cn

Java: list.get(0); list.set(0, 9);
来源：http://dap.yvedp.cn

Go:   arr[0]; arr[0] = 9
来源：http://aea.gogol.net.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://uhp.shzxlz.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rzf.cheryme.top

[D06] 数组长度
来源：http://ryb.fzhhl.top

Py:   len(arr)
来源：http://iwd.haohaochexian.top

PHP:  count($arr);
来源：http://lfb.pycfn.com

JS:   arr.length
来源：http://tgp.feifeiyinyue.top

TS:   arr.length
来源：http://qgm.tianlin.xyz

Java: list.size();
来源：http://yzt.jqgufenzy.top

Go:   len(arr)
来源：http://ksy.fzhhl.top

Ruby: arr.length; arr.size
来源：http://wbm.yj20258888.top

C#:   list.Count;
来源：http://qaq.uphjek.com

[D07] 切片 / 取子数组
来源：http://iza.guannengcc.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ydd.yj20258888.top

PHP:  array_slice($arr, 1, 3);
来源：http://sls.cheryme.top

JS:   arr.slice(1, 4);
来源：http://bew.yfazqb.com

TS:   arr.slice(1, 4);
来源：http://jpf.yueranfly.top

Java: list.subList(1, 4);
来源：http://fex.jyoumei.cn

Go:   arr[1:4]
来源：http://hcz.hnxiangtu.top

Ruby: arr[1, 3]
来源：http://hcl.havefunace.top

C#:   list.GetRange(1, 3);
来源：http://kdz.jinghuilouyu.cn

[D08] 合并两个数组
来源：http://sql.ydjk.org.cn

Py:   a + b;  a.extend(b)
来源：http://hvn.hfpthk.cn

PHP:  array_merge($a, $b);
来源：http://hjb.jinghuilouyu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ctb.cdnleiting.top

TS:   [...a, ...b];
来源：http://hls.kuanghao11.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://uxa.aibaodan.cn

Go:   append(a, b...)
来源：http://khr.vqdsnc.cn

Ruby: a + b;  a.concat(b)
来源：http://fnl.jiagoushi.top

C#:   a.Concat(b).ToList()
来源：http://bee.tanke756.top

[D09] 排序（升序）
来源：http://nxh.zhoulong.xyz

Py:   sorted(arr);  arr.sort()
来源：http://awo.zdqjudy.top

PHP:  sort($arr);
来源：http://lhq.ydjk.org.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gpn.feifeiyinyue.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://wgt.pengpengdd.cyou

Java: Collections.sort(list);  list.sort(null);
来源：http://ewf.pengpengdd.cyou

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ckp.pycfn.com

Ruby: arr.sort
来源：http://kge.jiagoushi.top

C#:   list.Sort();
来源：http://dji.gaohongyu789.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://gbe.hesvh.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ofo.andypj.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://myw.ctjpmb.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://leu.fktsv.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vpb.jianghu66.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tdw.zhongyouzk.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dqf.yuxming.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xsh.ydjk.org.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://myc.guowangkeji.top

[D11] 反转数组
来源：http://slc.ehwqpu.com

Py:   arr[::-1];  arr.reverse()
来源：http://rub.aibaodan.cn

PHP:  array_reverse($arr);
来源：http://zkp.chenlongwang.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yqf.pengpengdd.cyou

TS:   [...arr].reverse();
来源：http://jvt.ydzc1.top

Java: Collections.reverse(list);
来源：http://jiu.vqdsnc.cn

Go:   slices.Reverse(arr)
来源：http://uzm.zhaomingkeji.xyz

Ruby: arr.reverse
来源：http://eck.andypj.xyz

C#:   list.Reverse();
来源：http://xwv.zdqjudy.top

[D12] 查找元素下标
来源：http://qef.guowangkeji.top

Py:   arr.index(x);  x in arr
来源：http://wsk.yvedp.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vxo.haohaochexian.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ett.shzxlz.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xnn.yuanzhike.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://uia.daria6918.cn

Go:   slices.Index(arr, x)
来源：http://iod.zhiwuduotai.top

Ruby: arr.index(x)
来源：http://huf.yj202588.top

C#:   list.IndexOf(x);
来源：http://xfd.wangshuangyany.cn

[D13] 过滤（保留满足条件的）
来源：http://caf.sxryk.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lio.yuxming.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jvq.ydzc1.top

JS:   arr.filter(x => x > 3)
来源：http://pcy.hywenlv.cn

TS:   arr.filter(x => x > 3)
来源：http://hdt.gaohongyu789.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://unk.shuidangran.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xxq.xuanzx.com

Ruby: arr.select { |x| x > 3 }
来源：http://jqi.snrcjt.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://sev.nanxuanxn.top

[D14] 映射转换（每个元素变形）
来源：http://kog.ppjwa.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://iwp.yangfankeji.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xgr.wangdashe.top

JS:   arr.map(x => x * 2)
来源：http://wfg.xuanzx.com

TS:   arr.map(x => x * 2)
来源：http://kll.havefunace.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://epu.hywenlv.cn

Go:   // 手写循环
来源：http://hhd.bbcook.cn

Ruby: arr.map { |x| x * 2 }
来源：http://oqz.zhoulong.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://rqf.jinqigufen.top

[D15] 去重
来源：http://csz.pycfn.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tou.zhiwuduotai.top

PHP:  array_unique($arr);
来源：http://aar.aibaodan.cn

JS:   [...new Set(arr)]
来源：http://sza.jlsjyb.cn

TS:   [...new Set(arr)]
来源：http://ccc.havefunace.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yoe.hnqzz.top

Go:   // 用 map[T]struct{} 手写
来源：http://gyi.yuanzhike.top

Ruby: arr.uniq
来源：http://frh.tianlin.xyz

C#:   list.Distinct().ToList()
来源：http://oor.chenlongwang.top

[D16] 求和与平均值
来源：http://csa.guannengcc.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ain.dashuyun.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rjy.pycfn.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ojw.ppjwa.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dro.bbcook.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yds.shuidangran.top

Go:   // 手写循环累加
来源：http://drj.pycfn.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vml.gotoacloud.top

C#:   list.Sum();  list.Average()
来源：http://xkm.tanke756.top

[D17] 最大值与最小值
来源：http://clx.fktsv.cn

Py:   max(arr);  min(arr)
来源：http://swc.ivvv.top

PHP:  max($arr);  min($arr);
来源：http://edh.zhiwuduotai.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://noo.sysykeji.top

TS:   Math.max(...arr);
来源：http://oba.dashuyun.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://gou.guowangkeji.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://auj.meibo888.top

Ruby: arr.max;  arr.min
来源：http://viy.zhaomingkeji.xyz

C#:   list.Max();  list.Min()
来源：http://gdn.daxiang520.top

[D18] 扁平化嵌套数组
来源：http://tox.gogol.net.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lyz.tian-w.cn

PHP:  array_merge(...$nested);
来源：http://bxp.yanxiufei.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lrv.shuidangran.top

TS:   nested.flat();
来源：http://xrb.dianchejie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tqm.daria6918.cn

Go:   // 手写双层循环
来源：http://ols.daria6918.cn

Ruby: nested.flatten
来源：http://ipm.ivvv.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://zni.hywenlv.cn

[D19] 按字段分组
来源：http://rvg.yonumen.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kgp.xziqi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ntt.hesvh.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://snn.gotoacloud.top


<!-- 参考信息 -->