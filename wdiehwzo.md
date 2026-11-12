代发 wailian999

[C02] 默认参数
来源：http://mlz.aibaodan.cn

Py:   def greet(name="World"): return name
来源：http://eyr.hnxiangtu.top

PHP:  function greet($name = "World") { return $name; }
来源：http://bvf.nwbrower.top

JS:   function greet(name = "World") { return name; }
来源：http://tnj.aibaodan.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://zpz.pycfn.com

Java: // 无默认参数：方法重载或 Optional
来源：http://fne.ydjk.org.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lie.9152youxi.cn

Ruby: def greet(name = "World") = name
来源：http://ovu.fzhhl.top

C#:   string Greet(string name = "World") => name;
来源：http://psf.xziqi.cn

[C03] 可变参数
来源：http://gzt.jqgufenzy.top

Py:   def total(*args): return sum(args)
来源：http://eps.guowangkeji.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vrj.jinqigufen.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bre.zycfv.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rrr.bjfxy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qvv.shuidangran.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://aeh.guowangkeji.top

Ruby: def total(*nums); nums.sum; end
来源：http://jwd.hywenlv.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qqg.cucudq.cn

[C04] 命名参数 / 关键字参数
来源：http://ukg.bbcook.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tah.jinyuanbaomall.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://aey.yj202588.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tqb.hysaishi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://isp.gaohongyu789.top

Java: // 无：用 Builder 模式或 record
来源：http://vlj.guannengcc.top

Go:   // 无：用配置结构体参数
来源：http://vtf.sufxvd.cn

Ruby: f(a: 1, b: 2)
来源：http://buj.cucudq.cn

C#:   f(a: 1, b: 2)
来源：http://bmm.feifeiyinyue.top

[C05] 返回多个值
来源：http://fop.hnqzz.top

Py:   return a, b
来源：http://wja.yj20258888.top

PHP:  return [$a, $b];
来源：http://owk.ybcxt.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://zrm.cdnleiting.top

TS:   return { a, b };
来源：http://kzg.jlsjyb.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wle.chenlongwang.top

Go:   return a, b
来源：http://xgt.yuxming.cn

Ruby: return a, b
来源：http://uqj.nanxinkj.top

C#:   return (a, b);              // ValueTuple
来源：http://njz.yj20258888.top

[C06] 匿名函数 / lambda
来源：http://hqm.jinqigfzy.top

Py:   square = lambda x: x * x
来源：http://dim.ydzc1.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ysg.xuetiantiany.cn

JS:   const square = x => x * x;
来源：http://pcs.zhengqikj.top

TS:   const square = (x: number): number => x * x;
来源：http://ngi.jinqigufen.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fkh.hfpthk.cn

Go:   sq := func(x int) int { return x * x }
来源：http://vwm.jlsjyb.cn

Ruby: square = ->(x) { x * x }
来源：http://uml.haohaochexian.top

C#:   Func<int, int> square = x => x * x;
来源：http://rms.yuanzhike.top

[C07] 把函数作为参数传入
来源：http://xnm.ctjpmb.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://igs.zdqjudy.top

PHP:  array_map("strtoupper", $arr);
来源：http://svg.cheryme.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ipk.yuanzhike.top

TS:   arr.map(String)
来源：http://ngp.ppjwa.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wlw.epnwcf.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qzz.xziqi.cn

Ruby: arr.map(&:upcase)
来源：http://vzq.iojbl.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wzu.yanxiufei.cn

[C08] 闭包
来源：http://pnc.fehbvm.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ste.hysaishi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mbl.jqgfzy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://efw.xuanzx.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yor.52xcode.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wll.wangshuangyany.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nyh.chenlongwang.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fry.yfazqb.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vct.fengsongda.top

[C09] 递归
来源：http://tgw.wangshuangyany.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cpw.fktsv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vqj.ydzc1.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://euh.yongpay.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wwg.52xcode.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://npx.xinyue.icu

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rmp.fanxiaobao.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lzh.nanxinkj.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://utw.316326.xyz

[C10] 变量作用域
来源：http://pbi.9152youxi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dmb.yj20258.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jmr.jinqigufen.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lwf.pycfn.com

TS:   同 JS
来源：http://xqg.sweek.top

Java: 方法内为块级作用域
来源：http://ici.havefunace.top

Go:   花括号块级作用域
来源：http://ylk.quarkkingdee.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tdv.jqgfzy.top

C#:   块级作用域
来源：http://vqm.yfazqb.com

[C11] 模块导入与导出
来源：http://zig.gzhubu.top

Py:   from module import func
来源：http://hqi.hnxiangtu.top

PHP:  require "file.php";  或 use App\Service;
来源：http://mec.gogol.net.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://wgm.hywenlv.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://sly.redwolf501.top

Java: import java.util.List;
来源：http://ucu.hesvh.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://urh.ybcxt.top

Ruby: require "json"; require_relative "./util"
来源：http://fuu.chenzaomai.com

C#:   using System.Text;
来源：http://kwb.birdmap.top

[C12] 立即执行函数 IIFE
来源：http://ews.ivvv.top

Py:   (lambda: print("run"))()
来源：http://fsc.sufxvd.cn

PHP:  (function () { echo "run"; })();
来源：http://ukv.aizwys.cn

JS:   (() => { console.log("run"); })();
来源：http://brd.sweek.top

TS:   (() => { console.log("run"); })();
来源：http://yjj.zhongyouzk.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lgt.ywan-chungtsiang.top

Go:   func() { fmt.Println("run") }()
来源：http://fmx.iojbl.cn

Ruby: -> { puts "run" }.call
来源：http://lsc.daria6918.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://wfn.sjlbkw.cn

[C13] 类型声明 / 类型注解
来源：http://ywl.yongpay.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://iho.svipenyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://brh.jyoumei.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ojd.jianghu66.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baa.shanyushiyangkeji.top

Java: int add(int a, int b) { return a + b; }
来源：http://uhc.jinqigfzy.top

Go:   func add(a, b int) int
来源：http://nsp.hesvh.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kao.jiagoushi.top

C#:   int Add(int a, int b) => a + b;
来源：http://ces.yuxming.cn

[C14] 泛型函数
来源：http://uwc.c1oappe.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ifq.yuanzhike.top

PHP:  // 无泛型
来源：http://whm.nanxuanxn.top

JS:   // 无泛型
来源：http://oxs.tarul.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xwr.jinqigfzy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ufo.ybcxt.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hqm.uphjek.com

Ruby: # 无泛型
来源：http://soj.wangdashe.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dna.gogol.net.cn

[C15] 解构 / 展开参数
来源：http://qsp.svipenyu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jni.ywan-chungtsiang.top

PHP:  [$a, $b] = $pair;
来源：http://mgd.haohaochexian.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://kzq.ydzc1.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nix.xinyue.icu

Java: // 无解构
来源：http://ubf.zdbjq.cn

Go:   // 无解构
来源：http://jir.vqdsnc.cn

Ruby: a, b = pair
来源：http://dmr.zhaomingkeji.xyz

C#:   var (a, b) = pair;
来源：http://ubf.vqdsnc.cn

[C16] 函数 / 方法重载
来源：http://feq.bjfxy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yfc.chenjidiqi.icu

PHP:  // 无重载
来源：http://hju.snrcjt.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://uvk.birdmap.top

TS:   // 用联合类型或重载签名声明
来源：http://huh.shangyingyoupin.top

Java: void f(int a) {}  void f(String a) {}
来源：http://bfl.sweek.top

Go:   // 无重载：用不同函数名
来源：http://xqm.0kj1m.cn

Ruby: # 无重载：靠动态参数
来源：http://kys.nwbrower.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://aop.ybcxt.top

================================================================================
来源：http://hzi.zycfv.cn

D. 数组 / 列表 / 集合
来源：http://cie.fengsongda.top

================================================================================
来源：http://vor.hfpthk.cn

[D01] 创建数组 / 列表
来源：http://lyo.daria6918.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://enf.aizwys.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qoe.jinghuilouyu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://shz.cqqwz.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://win.redwolf501.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pzm.hongshengwenyu.top

Go:   arr := []int{1, 2, 3}
来源：http://nba.cdnleiting.top

Ruby: arr = [1, 2, 3]
来源：http://trs.guowangkeji.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yrx.jinqigufen.top

[D02] 追加元素到末尾
来源：http://tbj.shanyushiyangkeji.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://raf.ydjk.org.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blr.birdmap.top

JS:   arr.push(4);
来源：http://vsf.feifeiyinyue.top

TS:   arr.push(4);
来源：http://fnn.guowangkeji.top

Java: list.add(4);
来源：http://els.jianghu66.top

Go:   arr = append(arr, 4)
来源：http://des.smart0.xyz

Ruby: arr << 4; arr.push(5)
来源：http://tfb.cheryme.top

C#:   list.Add(4);
来源：http://ohr.tianlin.xyz

[D03] 在指定位置插入元素
来源：http://mfm.smart0.xyz

Py:   arr.insert(0, 0)
来源：http://sjb.hnxiangtu.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wgd.birdmap.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://eho.xuanzx.com

TS:   arr.splice(0, 0, 0);
来源：http://nwo.havefunace.top

Java: list.add(0, 0);
来源：http://knv.fehbvm.com

Go:   arr = append([]int{0}, arr...)
来源：http://npa.yangfankeji.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gfr.yuxming.cn

C#:   list.Insert(0, 0);
来源：http://eto.andypj.xyz

[D04] 删除元素
来源：http://tgc.pycfn.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://moc.xuetiantiany.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vde.haohaochexian.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ugd.ctjpmb.com

TS:   arr.splice(0, 1);
来源：http://keh.jqgfzy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tfd.c1oappe.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hre.daria6918.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://iwy.tianlin.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pde.wangshuangyany.cn

[D05] 访问与修改元素
来源：http://rwk.chenjidiqi.icu

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cba.jinqigfzy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://egy.zhaomingkeji.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ihz.vehdjk.com

TS:   arr[0]; arr.at(-1);
来源：http://szq.yangfankeji.com

Java: list.get(0); list.set(0, 9);
来源：http://bdo.jianghu66.top

Go:   arr[0]; arr[0] = 9
来源：http://eld.ybcxt.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sdn.gogol.net.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ncy.jinqigfzy.top

[D06] 数组长度
来源：http://pdy.ybcxt.top

Py:   len(arr)
来源：http://fxh.fehbvm.com

PHP:  count($arr);
来源：http://qvp.jinqigfzy.top

JS:   arr.length
来源：http://qnb.jinqigfzy.top

TS:   arr.length
来源：http://ufu.havefunace.top

Java: list.size();
来源：http://cbd.hysaishi.cn

Go:   len(arr)
来源：http://ibe.uphjek.com

Ruby: arr.length; arr.size
来源：http://jvo.vqdsnc.cn

C#:   list.Count;
来源：http://slx.shanyushiyangkeji.top

[D07] 切片 / 取子数组
来源：http://yfp.pengpengdd.cyou

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ghn.fengsongda.top

PHP:  array_slice($arr, 1, 3);
来源：http://tkn.meibo888.top

JS:   arr.slice(1, 4);
来源：http://miq.sjlbkw.cn

TS:   arr.slice(1, 4);
来源：http://dcb.jinqigfzy.top

Java: list.subList(1, 4);
来源：http://igl.ydjk.org.cn

Go:   arr[1:4]
来源：http://ceg.hongshengwenyu.top

Ruby: arr[1, 3]
来源：http://fkp.wangdashe.top

C#:   list.GetRange(1, 3);
来源：http://wci.bjfxy.top

[D08] 合并两个数组
来源：http://jkj.meibo888.top

Py:   a + b;  a.extend(b)
来源：http://rjo.jinqigufen.top

PHP:  array_merge($a, $b);
来源：http://qld.yuanzhike.top

JS:   [...a, ...b];  a.concat(b);
来源：http://bru.nanxinkj.top

TS:   [...a, ...b];
来源：http://xag.jqgfzy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://njp.daria6918.cn

Go:   append(a, b...)
来源：http://ejt.xylfe.cn

Ruby: a + b;  a.concat(b)
来源：http://wkm.xuanzx.com

C#:   a.Concat(b).ToList()
来源：http://ymk.yj20258888.top

[D09] 排序（升序）
来源：http://asn.meibo888.top

Py:   sorted(arr);  arr.sort()
来源：http://aue.uphjek.com

PHP:  sort($arr);
来源：http://rtg.andypj.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qss.hywenlv.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gtz.snrcjt.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xja.zhiwuduotai.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://upv.nwbrower.top

Ruby: arr.sort
来源：http://wlv.shanyushiyangkeji.top

C#:   list.Sort();
来源：http://cyk.yj20258888.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://obv.fehbvm.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://eno.zhongyouzk.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://eow.uphjek.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xha.yonumen.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xrp.tanke756.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nno.zhiwuduotai.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://atn.ivvv.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://crg.ppjwa.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gae.jinghuilouyu.cn

[D11] 反转数组
来源：http://xri.andypj.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://lid.hnxiangtu.top

PHP:  array_reverse($arr);
来源：http://qvd.ydzc1.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nxv.cashguo.top

TS:   [...arr].reverse();
来源：http://hgu.pycfn.com

Java: Collections.reverse(list);
来源：http://wxe.ydjk.org.cn

Go:   slices.Reverse(arr)
来源：http://wle.hywenlv.cn

Ruby: arr.reverse
来源：http://tae.zdbjq.cn

C#:   list.Reverse();
来源：http://yid.quarkkingdee.top

[D12] 查找元素下标
来源：http://azu.xinyue.icu

Py:   arr.index(x);  x in arr
来源：http://oiy.sysykeji.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kxr.xziqi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://atu.fanxiaobao.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cyb.sysykeji.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nbs.tian-w.cn

Go:   slices.Index(arr, x)
来源：http://xmq.zhongyouzk.top

Ruby: arr.index(x)
来源：http://gfi.shanyushiyangtech.top

C#:   list.IndexOf(x);
来源：http://pqh.redwolf501.top

[D13] 过滤（保留满足条件的）
来源：http://agz.cdnleiting.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lmp.zhaomingkeji.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ynr.bjfxy.top

JS:   arr.filter(x => x > 3)
来源：http://het.tianlin.xyz

TS:   arr.filter(x => x > 3)
来源：http://uvf.wangshuangyany.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ppj.yongpay.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kmz.xziqi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://itq.pycfn.com

C#:   list.Where(x => x > 3).ToList()
来源：http://ics.316326.xyz

[D14] 映射转换（每个元素变形）
来源：http://jnt.jqgufenzy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://oie.jianghu66.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mdi.vehdjk.com

JS:   arr.map(x => x * 2)
来源：http://uor.xuanzx.com

TS:   arr.map(x => x * 2)
来源：http://ckc.epnwcf.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://zuc.fzhhl.top

Go:   // 手写循环
来源：http://icn.fktsv.cn

Ruby: arr.map { |x| x * 2 }
来源：http://gum.chenjidiqi.icu

C#:   list.Select(x => x * 2).ToList()
来源：http://bzg.gzhubu.top

[D15] 去重
来源：http://uny.ehwqpu.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hcz.yj20258.top

PHP:  array_unique($arr);
来源：http://hov.yfazqb.com

JS:   [...new Set(arr)]
来源：http://uin.jiagoushi.top

TS:   [...new Set(arr)]
来源：http://aan.ydjk.org.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yoq.tian-w.cn

Go:   // 用 map[T]struct{} 手写
来源：http://vom.havefunace.top

Ruby: arr.uniq
来源：http://bbb.cashguo.top

C#:   list.Distinct().ToList()
来源：http://mdd.jiagoushi.top

[D16] 求和与平均值
来源：http://mda.52xcode.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ozj.pengpengdd.cyou

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zsr.havefunace.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jrd.jqgfzy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lqt.hammf.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mmu.dashuyun.cn

Go:   // 手写循环累加
来源：http://uxt.c1oappe.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://idn.fzhhl.top

C#:   list.Sum();  list.Average()
来源：http://ret.hammf.cn

[D17] 最大值与最小值
来源：http://nud.yangfankeji.com

Py:   max(arr);  min(arr)
来源：http://pkl.daxiang520.top

PHP:  max($arr);  min($arr);
来源：http://ihk.fanxiaobao.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kev.zhiwuduotai.top

TS:   Math.max(...arr);
来源：http://tjr.nanxinkj.top

Java: Collections.max(list);  Collections.min(list);
来源：http://bvl.yuxming.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://est.jyoumei.cn

Ruby: arr.max;  arr.min
来源：http://exa.xingfuxueyuan.xyz

C#:   list.Max();  list.Min()
来源：http://zeb.hesvh.cn

[D18] 扁平化嵌套数组
来源：http://ckp.cqqwz.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cii.zhijiandao.cn

PHP:  array_merge(...$nested);
来源：http://lzw.jianghu66.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bxi.shzxlz.cn

TS:   nested.flat();
来源：http://rmc.chenlongwang.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://scs.meibo888.top

Go:   // 手写双层循环
来源：http://jas.dashuyun.cn

Ruby: nested.flatten
来源：http://joe.yj20258.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://vdr.gogol.net.cn


<!-- 参考信息 -->