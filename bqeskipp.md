代发 wailian999

Java: if (data == null) return;
来源：http://nlm.fengsongda.top

Go:   if data == nil { return }
来源：http://byy.cqqwz.cn

Ruby: return if data.nil?
来源：http://jnc.yongpay.top

C#:   if (data == null) return;
来源：http://bsx.smart0.xyz

================================================================================
来源：http://lrn.yangfankeji.com

C. 函数与作用域
来源：http://vdy.jinqigufen.top

================================================================================
来源：http://gtn.zhoulong.xyz

[C01] 定义函数
来源：http://apv.quarkkingdee.top

Py:   def add(a, b): return a + b
来源：http://jpn.gogol.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fwb.jiagoushi.top

JS:   function add(a, b) { return a + b; }
来源：http://bte.mhx1999.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://klg.wangshuangyany.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://apx.fktsv.cn

Go:   func add(a, b int) int { return a + b }
来源：http://hsa.yuanzhike.top

Ruby: def add(a, b); a + b; end
来源：http://skf.yanxiufei.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://uzl.ivvv.top

[C02] 默认参数
来源：http://bkj.aizwys.cn

Py:   def greet(name="World"): return name
来源：http://xlb.shzxlz.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://hdl.nanxinkj.top

JS:   function greet(name = "World") { return name; }
来源：http://dfk.yj202588.top

TS:   function greet(name: string = "World") { return name; }
来源：http://yqo.jinqigufen.top

Java: // 无默认参数：方法重载或 Optional
来源：http://jwm.gogol.net.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fiz.ehwqpu.com

Ruby: def greet(name = "World") = name
来源：http://amx.zycfv.cn

C#:   string Greet(string name = "World") => name;
来源：http://xzz.jinqigfzy.top

[C03] 可变参数
来源：http://dut.yfazqb.com

Py:   def total(*args): return sum(args)
来源：http://gkc.redwolf501.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ijc.shzxlz.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pkm.yueranfly.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nrf.daxiang520.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gng.chenjidiqi.icu

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qdt.cqqwz.cn

Ruby: def total(*nums); nums.sum; end
来源：http://gqu.epnwcf.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ugx.jinyuanbaomall.cn

[C04] 命名参数 / 关键字参数
来源：http://wjj.aibaodan.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://uip.aizwys.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mta.ivvv.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rix.sysykeji.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qyn.quarkkingdee.top

Java: // 无：用 Builder 模式或 record
来源：http://vtq.sjlbkw.cn

Go:   // 无：用配置结构体参数
来源：http://yoh.hnqzz.top

Ruby: f(a: 1, b: 2)
来源：http://xna.52xcode.cn

C#:   f(a: 1, b: 2)
来源：http://lli.dashuyun.cn

[C05] 返回多个值
来源：http://hdy.gaohongyu789.top

Py:   return a, b
来源：http://xub.ctjpmb.com

PHP:  return [$a, $b];
来源：http://kwm.guannengcc.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://iqb.meibo888.top

TS:   return { a, b };
来源：http://tlo.ivvv.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xju.smart0.xyz

Go:   return a, b
来源：http://lxo.wangshuangyany.cn

Ruby: return a, b
来源：http://xoj.gaohongyu789.top

C#:   return (a, b);              // ValueTuple
来源：http://jzj.uphjek.com

[C06] 匿名函数 / lambda
来源：http://quz.9152youxi.cn

Py:   square = lambda x: x * x
来源：http://sjg.zycfv.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://yja.quarkkingdee.top

JS:   const square = x => x * x;
来源：http://aoq.zdqjudy.top

TS:   const square = (x: number): number => x * x;
来源：http://sne.zdbjq.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hrs.shzxlz.cn

Go:   sq := func(x int) int { return x * x }
来源：http://zqk.hfpthk.cn

Ruby: square = ->(x) { x * x }
来源：http://xic.jqgufenzy.top

C#:   Func<int, int> square = x => x * x;
来源：http://gcx.mhx1999.top

[C07] 把函数作为参数传入
来源：http://xzk.316326.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xyx.meibo888.top

PHP:  array_map("strtoupper", $arr);
来源：http://sde.gzhubu.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vcl.tanke756.top

TS:   arr.map(String)
来源：http://kur.jinqigufen.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://waz.xuanzx.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://izq.ydjk.org.cn

Ruby: arr.map(&:upcase)
来源：http://cxm.ybcxt.top

C#:   arr.Select(s => s.ToUpper())
来源：http://hgh.yj20258888.top

[C08] 闭包
来源：http://tth.shangyingyoupin.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fuu.jinqigfzy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://spb.dianchejie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://eps.smart0.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://uoj.guowangkeji.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://iyf.c1oappe.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hmy.ppjwa.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://emj.yj20258.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ibg.316326.xyz

[C09] 递归
来源：http://qbu.yvedp.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qzf.ehwqpu.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mct.jianghu66.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dfa.yangfankeji.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qfp.hesvh.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dmz.zdbjq.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gbk.xuanzx.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wwi.jqgfzy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ouv.nanxinkj.top

[C10] 变量作用域
来源：http://crc.feifeiyinyue.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mrr.yj20258888.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ucq.cheryme.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rpb.sweek.top

TS:   同 JS
来源：http://qtv.jinqigfzy.top

Java: 方法内为块级作用域
来源：http://qch.hesvh.cn

Go:   花括号块级作用域
来源：http://usv.sjlbkw.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zaf.fktsv.cn

C#:   块级作用域
来源：http://opj.gaohongyu789.top

[C11] 模块导入与导出
来源：http://jvw.snrcjt.cn

Py:   from module import func
来源：http://lvd.sysykeji.top

PHP:  require "file.php";  或 use App\Service;
来源：http://uyx.jlsjyb.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ocv.jqgufenzy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vpi.nwbrower.top

Java: import java.util.List;
来源：http://yci.tianlin.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://upb.gzhubu.top

Ruby: require "json"; require_relative "./util"
来源：http://gji.xziqi.cn

C#:   using System.Text;
来源：http://ako.ybcxt.top

[C12] 立即执行函数 IIFE
来源：http://foj.tanke756.top

Py:   (lambda: print("run"))()
来源：http://itu.cashguo.top

PHP:  (function () { echo "run"; })();
来源：http://xxu.tian-w.cn

JS:   (() => { console.log("run"); })();
来源：http://pfo.ydzc1.top

TS:   (() => { console.log("run"); })();
来源：http://utk.zhengqikj.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wie.xingfuxueyuan.xyz

Go:   func() { fmt.Println("run") }()
来源：http://rde.daria6918.cn

Ruby: -> { puts "run" }.call
来源：http://nqj.smart0.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://lak.daxiang520.top

[C13] 类型声明 / 类型注解
来源：http://sbt.hysaishi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zur.yonumen.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://del.jiagoushi.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://iys.cdnleiting.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dsx.fengsongda.top

Java: int add(int a, int b) { return a + b; }
来源：http://zzx.sysykeji.top

Go:   func add(a, b int) int
来源：http://orw.c1oappe.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ivk.tanke756.top

C#:   int Add(int a, int b) => a + b;
来源：http://gws.epnwcf.com

[C14] 泛型函数
来源：http://ehx.gotoacloud.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dnm.yuxming.cn

PHP:  // 无泛型
来源：http://egn.cheryme.top

JS:   // 无泛型
来源：http://tkf.cheryme.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ooe.aizwys.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gml.ctjpmb.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zos.epnwcf.com

Ruby: # 无泛型
来源：http://epo.havefunace.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zka.uphjek.com

[C15] 解构 / 展开参数
来源：http://rge.ydjk.org.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wsl.nanxinkj.top

PHP:  [$a, $b] = $pair;
来源：http://ljs.uphjek.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jan.cheryme.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://efk.daria6918.cn

Java: // 无解构
来源：http://wdf.yj20258.top

Go:   // 无解构
来源：http://wha.cheryme.top

Ruby: a, b = pair
来源：http://nrq.9152youxi.cn

C#:   var (a, b) = pair;
来源：http://ult.cucudq.cn

[C16] 函数 / 方法重载
来源：http://vop.wangshuangyany.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://act.zhoulong.xyz

PHP:  // 无重载
来源：http://uuk.jinyuanbaomall.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://keb.52xcode.cn

TS:   // 用联合类型或重载签名声明
来源：http://bqc.haohaochexian.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ayr.meibo888.top

Go:   // 无重载：用不同函数名
来源：http://rrp.epnwcf.com

Ruby: # 无重载：靠动态参数
来源：http://bsp.havefunace.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://cgb.ydjk.org.cn

================================================================================
来源：http://lkv.wangdashe.top

D. 数组 / 列表 / 集合
来源：http://uek.fzhhl.top

================================================================================
来源：http://rnw.316326.xyz

[D01] 创建数组 / 列表
来源：http://agi.ydzc1.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://dcq.zhengqikj.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bsw.wangshuangyany.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mtj.jqgufenzy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://gdp.ivvv.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://caf.zdqjudy.top

Go:   arr := []int{1, 2, 3}
来源：http://hbr.tianlin.xyz

Ruby: arr = [1, 2, 3]
来源：http://hxm.ybcxt.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xoe.hammf.cn

[D02] 追加元素到末尾
来源：http://hyh.ehwqpu.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fhh.guowangkeji.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bze.feifeiyinyue.top

JS:   arr.push(4);
来源：http://xfx.bjfxy.top

TS:   arr.push(4);
来源：http://vvc.feifeiyinyue.top

Java: list.add(4);
来源：http://dcm.bbcook.cn

Go:   arr = append(arr, 4)
来源：http://ozg.52xcode.cn

Ruby: arr << 4; arr.push(5)
来源：http://dcd.zhoulong.xyz

C#:   list.Add(4);
来源：http://gct.cqqwz.cn

[D03] 在指定位置插入元素
来源：http://txk.zhongyouzk.top

Py:   arr.insert(0, 0)
来源：http://djj.zdbjq.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fwu.gaohongyu789.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fjq.cashguo.top

TS:   arr.splice(0, 0, 0);
来源：http://xjw.fzhhl.top

Java: list.add(0, 0);
来源：http://vrm.nwbrower.top

Go:   arr = append([]int{0}, arr...)
来源：http://nbi.ivvv.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ilg.bjfxy.top

C#:   list.Insert(0, 0);
来源：http://dnk.iojbl.cn

[D04] 删除元素
来源：http://kwb.svipenyu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vyl.hammf.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kxj.guannengcc.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://uka.cdnleiting.top

TS:   arr.splice(0, 1);
来源：http://hlg.gogol.net.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vhc.hammf.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vlz.jinyuanbaomall.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://sgb.jiagoushi.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cfq.yj20258.top

[D05] 访问与修改元素
来源：http://xhd.zhiwuduotai.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gpb.bbcook.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mmt.pycfn.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ekd.316326.xyz

TS:   arr[0]; arr.at(-1);
来源：http://suk.smart0.xyz

Java: list.get(0); list.set(0, 9);
来源：http://zdv.chenlongwang.top

Go:   arr[0]; arr[0] = 9
来源：http://qig.epnwcf.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ijc.nwbrower.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mxe.ydjk.org.cn

[D06] 数组长度
来源：http://lus.andypj.xyz

Py:   len(arr)
来源：http://xeo.sjlbkw.cn

PHP:  count($arr);
来源：http://tdt.hcnkem.com

JS:   arr.length
来源：http://nvf.cqqwz.cn

TS:   arr.length
来源：http://iys.birdmap.top

Java: list.size();
来源：http://irb.xingfuxueyuan.xyz

Go:   len(arr)
来源：http://kij.fanxiaobao.xyz

Ruby: arr.length; arr.size
来源：http://lva.52xcode.cn

C#:   list.Count;
来源：http://ugz.zhiwuduotai.top

[D07] 切片 / 取子数组
来源：http://hcx.guowangkeji.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wje.ydjk.org.cn

PHP:  array_slice($arr, 1, 3);
来源：http://sjm.gotoacloud.top

JS:   arr.slice(1, 4);
来源：http://vao.jinyuanbaomall.cn

TS:   arr.slice(1, 4);
来源：http://pvf.shuidangran.top

Java: list.subList(1, 4);
来源：http://oqj.haohaochexian.top

Go:   arr[1:4]
来源：http://ljv.haohaochexian.top

Ruby: arr[1, 3]
来源：http://lcw.guannengcc.top

C#:   list.GetRange(1, 3);
来源：http://wcj.chenzaomai.com

[D08] 合并两个数组
来源：http://eef.sysykeji.top

Py:   a + b;  a.extend(b)
来源：http://oiy.ybcxt.top

PHP:  array_merge($a, $b);
来源：http://aio.hammf.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ulm.jinqigufen.top

TS:   [...a, ...b];
来源：http://wwy.hesvh.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://izq.xziqi.cn

Go:   append(a, b...)
来源：http://uue.gogol.net.cn

Ruby: a + b;  a.concat(b)
来源：http://ptm.tanke756.top

C#:   a.Concat(b).ToList()
来源：http://erq.sysykeji.top

[D09] 排序（升序）
来源：http://phd.pycfn.com

Py:   sorted(arr);  arr.sort()
来源：http://stb.zhixingplan.top

PHP:  sort($arr);
来源：http://tyh.shanyushiyangtech.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kox.cdnleiting.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://mbs.yfazqb.com

Java: Collections.sort(list);  list.sort(null);
来源：http://vke.ydzc1.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://uwp.jinyuanbaomall.cn

Ruby: arr.sort
来源：http://owc.fehbvm.com

C#:   list.Sort();
来源：http://lvd.wangdashe.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://vyn.havefunace.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nwg.jqgufenzy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://biu.ydjk.org.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://are.sjlbkw.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://otn.tarul.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wgu.iojbl.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://npr.xingfuxueyuan.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://msa.hysaishi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://seu.yuanzhike.top

[D11] 反转数组
来源：http://mqz.sjlbkw.cn

Py:   arr[::-1];  arr.reverse()
来源：http://djw.xuanzx.com

PHP:  array_reverse($arr);
来源：http://iyr.yj20258.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ugx.uphjek.com

TS:   [...arr].reverse();
来源：http://vsq.xuetiantiany.cn

Java: Collections.reverse(list);
来源：http://upp.ywan-chungtsiang.top

Go:   slices.Reverse(arr)
来源：http://wta.iojbl.cn

Ruby: arr.reverse
来源：http://viw.gzhubu.top

C#:   list.Reverse();
来源：http://zqe.dashuyun.cn

[D12] 查找元素下标
来源：http://mtv.chenzaomai.com

Py:   arr.index(x);  x in arr
来源：http://cqc.zhaomingkeji.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jnk.yueranfly.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wmh.ybcxt.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qfh.vehdjk.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wne.zhoulong.xyz

Go:   slices.Index(arr, x)
来源：http://kkg.andypj.xyz

Ruby: arr.index(x)
来源：http://vzz.dashuyun.cn

C#:   list.IndexOf(x);
来源：http://yic.gaohongyu789.top

[D13] 过滤（保留满足条件的）
来源：http://gjt.vqdsnc.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ykh.ehwqpu.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gna.pengpengdd.cyou

JS:   arr.filter(x => x > 3)
来源：http://hsi.sjlbkw.cn

TS:   arr.filter(x => x > 3)
来源：http://vbx.meibo888.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jns.gogol.net.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xqy.fengsongda.top

Ruby: arr.select { |x| x > 3 }
来源：http://cmb.tanke756.top

C#:   list.Where(x => x > 3).ToList()
来源：http://iko.0kj1m.cn

[D14] 映射转换（每个元素变形）
来源：http://ouz.yj202588.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hfo.zdqjudy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sta.9152youxi.cn

JS:   arr.map(x => x * 2)
来源：http://ect.bbcook.cn

TS:   arr.map(x => x * 2)
来源：http://bdr.nanxinkj.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://lbe.cashguo.top

Go:   // 手写循环
来源：http://whk.vehdjk.com

Ruby: arr.map { |x| x * 2 }
来源：http://isc.chenjidiqi.icu

C#:   list.Select(x => x * 2).ToList()
来源：http://qww.snrcjt.cn

[D15] 去重
来源：http://pjw.hammf.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://icu.cqqwz.cn

PHP:  array_unique($arr);
来源：http://fdm.0kj1m.cn

JS:   [...new Set(arr)]
来源：http://gyh.aizwys.cn

TS:   [...new Set(arr)]
来源：http://vtu.wangshuangyany.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://haw.aizwys.cn

Go:   // 用 map[T]struct{} 手写
来源：http://hyj.nanxuanxn.top

Ruby: arr.uniq
来源：http://kad.quarkkingdee.top

C#:   list.Distinct().ToList()
来源：http://zld.vqdsnc.cn

[D16] 求和与平均值
来源：http://mnb.hammf.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zua.wangdashe.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fkq.mhx1999.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mbe.xuetiantiany.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tio.nanxinkj.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fzh.jyoumei.cn

Go:   // 手写循环累加
来源：http://crr.cashguo.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zcv.0kj1m.cn

C#:   list.Sum();  list.Average()
来源：http://gta.sysykeji.top

[D17] 最大值与最小值
来源：http://tzn.yuanzhike.top

Py:   max(arr);  min(arr)
来源：http://nqp.jyoumei.cn


<!-- 参考信息 -->