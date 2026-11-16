代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://qwu.yfazqb.com

Go:   func add(a, b int) int { return a + b }
来源：http://cot.tian-w.cn

Ruby: def add(a, b); a + b; end
来源：http://ira.pycfn.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pkn.ydzc1.top

[C02] 默认参数
来源：http://nje.ydjk.org.cn

Py:   def greet(name="World"): return name
来源：http://sij.pycfn.com

PHP:  function greet($name = "World") { return $name; }
来源：http://jfl.zhongyouzk.top

JS:   function greet(name = "World") { return name; }
来源：http://kol.yanxiufei.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xiq.yuxming.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://xev.zdqjudy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rhd.svipenyu.cn

Ruby: def greet(name = "World") = name
来源：http://qes.ppjwa.cn

C#:   string Greet(string name = "World") => name;
来源：http://rmk.fengsongda.top

[C03] 可变参数
来源：http://ewi.gzhubu.top

Py:   def total(*args): return sum(args)
来源：http://qfw.yueranfly.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gaf.guannengcc.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://teg.hongshengwenyu.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dha.cashguo.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ksj.cucudq.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tjz.ywan-chungtsiang.top

Ruby: def total(*nums); nums.sum; end
来源：http://wrg.hysaishi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wih.tianlin.xyz

[C04] 命名参数 / 关键字参数
来源：http://uzx.birdmap.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qdq.shzxlz.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ima.dianchejie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://efj.yj202588.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wvx.chenzaomai.com

Java: // 无：用 Builder 模式或 record
来源：http://wpb.yj20258888.top

Go:   // 无：用配置结构体参数
来源：http://xij.daxiang520.top

Ruby: f(a: 1, b: 2)
来源：http://nwl.hnqzz.top

C#:   f(a: 1, b: 2)
来源：http://obj.fktsv.cn

[C05] 返回多个值
来源：http://kvh.jinqigfzy.top

Py:   return a, b
来源：http://lcm.xuetiantiany.cn

PHP:  return [$a, $b];
来源：http://mqf.zycfv.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://dfy.tianlin.xyz

TS:   return { a, b };
来源：http://zph.smart0.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ngx.epnwcf.com

Go:   return a, b
来源：http://eoy.ydjk.org.cn

Ruby: return a, b
来源：http://nen.zhixingplan.top

C#:   return (a, b);              // ValueTuple
来源：http://ync.ppjwa.cn

[C06] 匿名函数 / lambda
来源：http://kkb.birdmap.top

Py:   square = lambda x: x * x
来源：http://rgr.xinyue.icu

PHP:  $square = fn($x) => $x * $x;
来源：http://iwh.quarkkingdee.top

JS:   const square = x => x * x;
来源：http://raa.fzhhl.top

TS:   const square = (x: number): number => x * x;
来源：http://hvs.jlsjyb.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pxm.dianchejie.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ost.pycfn.com

Ruby: square = ->(x) { x * x }
来源：http://wmv.cucudq.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ubo.fehbvm.com

[C07] 把函数作为参数传入
来源：http://cgq.wangdashe.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ylg.dianchejie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://lrf.daria6918.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://urz.c1oappe.top

TS:   arr.map(String)
来源：http://msw.zdqjudy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kbz.tarul.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://eqc.cqqwz.cn

Ruby: arr.map(&:upcase)
来源：http://hyx.chenlongwang.top

C#:   arr.Select(s => s.ToUpper())
来源：http://vvo.uphjek.com

[C08] 闭包
来源：http://khz.hywenlv.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gqk.bjfxy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vum.snrcjt.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://huf.hcnkem.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cwt.chenjidiqi.icu

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://flx.zhengqikj.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ter.fengsongda.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://czu.zycfv.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ppf.hongshengwenyu.top

[C09] 递归
来源：http://pdc.jyoumei.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kjb.ywan-chungtsiang.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jsv.nanxinkj.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ixa.sjlbkw.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nka.feifeiyinyue.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://llt.pengpengdd.cyou

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bqe.c1oappe.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://byl.epnwcf.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vpy.aizwys.cn

[C10] 变量作用域
来源：http://igp.zdbjq.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bpw.cqqwz.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nsv.zdqjudy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mvo.mhx1999.top

TS:   同 JS
来源：http://iig.gotoacloud.top

Java: 方法内为块级作用域
来源：http://bsx.gotoacloud.top

Go:   花括号块级作用域
来源：http://aez.bbcook.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ugp.zhiwuduotai.top

C#:   块级作用域
来源：http://adv.yfazqb.com

[C11] 模块导入与导出
来源：http://pce.cashguo.top

Py:   from module import func
来源：http://xxh.sxryk.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://kvh.jiagoushi.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://jda.smart0.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lqx.smart0.xyz

Java: import java.util.List;
来源：http://oov.cqqwz.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lzy.fzhhl.top

Ruby: require "json"; require_relative "./util"
来源：http://ocz.nanxuanxn.top

C#:   using System.Text;
来源：http://ijk.kuanghao11.cn

[C12] 立即执行函数 IIFE
来源：http://tti.jiagoushi.top

Py:   (lambda: print("run"))()
来源：http://bmw.52xcode.cn

PHP:  (function () { echo "run"; })();
来源：http://hds.havefunace.top

JS:   (() => { console.log("run"); })();
来源：http://tpc.snrcjt.cn

TS:   (() => { console.log("run"); })();
来源：http://pat.jinghuilouyu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://trv.nwbrower.top

Go:   func() { fmt.Println("run") }()
来源：http://vtc.uphjek.com

Ruby: -> { puts "run" }.call
来源：http://edh.iojbl.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://sdb.daxiang520.top

[C13] 类型声明 / 类型注解
来源：http://dpm.yueranfly.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kia.zhaomingkeji.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dxf.yfazqb.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xzj.hnqzz.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://frn.hcnkem.com

Java: int add(int a, int b) { return a + b; }
来源：http://uwe.fzhhl.top

Go:   func add(a, b int) int
来源：http://tpk.dianchejie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vww.pengpengdd.cyou

C#:   int Add(int a, int b) => a + b;
来源：http://efr.wangdashe.top

[C14] 泛型函数
来源：http://sfu.zhaomingkeji.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://axe.chenlongwang.top

PHP:  // 无泛型
来源：http://smf.guannengcc.top

JS:   // 无泛型
来源：http://dak.meibo888.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cbd.zhiwuduotai.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gee.fehbvm.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kti.zhongyouzk.top

Ruby: # 无泛型
来源：http://fjx.birdmap.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://add.jinqigufen.top

[C15] 解构 / 展开参数
来源：http://wlv.jyoumei.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://oie.yueranfly.top

PHP:  [$a, $b] = $pair;
来源：http://usj.ydjk.org.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tik.yueranfly.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://isy.yj20258888.top

Java: // 无解构
来源：http://nha.hcnkem.com

Go:   // 无解构
来源：http://pgo.xinyue.icu

Ruby: a, b = pair
来源：http://aja.aibaodan.cn

C#:   var (a, b) = pair;
来源：http://aje.ivvv.top

[C16] 函数 / 方法重载
来源：http://flr.birdmap.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hcr.xylfe.cn

PHP:  // 无重载
来源：http://hdh.sjlbkw.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://jsa.feifeiyinyue.top

TS:   // 用联合类型或重载签名声明
来源：http://ald.gaohongyu789.top

Java: void f(int a) {}  void f(String a) {}
来源：http://kct.yangfankeji.com

Go:   // 无重载：用不同函数名
来源：http://nte.xinyue.icu

Ruby: # 无重载：靠动态参数
来源：http://noy.jlsjyb.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hpy.gotoacloud.top

================================================================================
来源：http://nvh.uphjek.com

D. 数组 / 列表 / 集合
来源：http://pnq.c1oappe.top

================================================================================
来源：http://pyh.xingfuxueyuan.xyz

[D01] 创建数组 / 列表
来源：http://wug.nanxuanxn.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://guy.jianghu66.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zlr.zhixingplan.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xmb.jianghu66.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://cjn.gotoacloud.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://osr.shangyingyoupin.top

Go:   arr := []int{1, 2, 3}
来源：http://bfb.9152youxi.cn

Ruby: arr = [1, 2, 3]
来源：http://onh.ydjk.org.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kvz.nanxuanxn.top

[D02] 追加元素到末尾
来源：http://lfm.yonumen.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ztp.fengsongda.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yuw.ywan-chungtsiang.top

JS:   arr.push(4);
来源：http://viv.ydzc1.top

TS:   arr.push(4);
来源：http://ucw.snrcjt.cn

Java: list.add(4);
来源：http://dgf.zhijiandao.cn

Go:   arr = append(arr, 4)
来源：http://ojn.shanyushiyangkeji.top

Ruby: arr << 4; arr.push(5)
来源：http://tnu.zdqjudy.top

C#:   list.Add(4);
来源：http://qwv.hnxiangtu.top

[D03] 在指定位置插入元素
来源：http://fil.haohaochexian.top

Py:   arr.insert(0, 0)
来源：http://bdy.quarkkingdee.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zlr.jianghu66.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jxn.gogol.net.cn

TS:   arr.splice(0, 0, 0);
来源：http://zew.xingfuxueyuan.xyz

Java: list.add(0, 0);
来源：http://wpd.ydzc1.top

Go:   arr = append([]int{0}, arr...)
来源：http://djz.jqgufenzy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pff.c1oappe.top

C#:   list.Insert(0, 0);
来源：http://dfp.cashguo.top

[D04] 删除元素
来源：http://zfy.svipenyu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vwv.chenjidiqi.icu

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hyg.meibo888.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qne.hnqzz.top

TS:   arr.splice(0, 1);
来源：http://fca.dianchejie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mhp.0kj1m.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gbj.yfazqb.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qpg.snrcjt.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vmz.hongshengwenyu.top

[D05] 访问与修改元素
来源：http://rna.tanke756.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tlk.jyoumei.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rgo.cqqwz.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nef.daria6918.cn

TS:   arr[0]; arr.at(-1);
来源：http://ves.hammf.cn

Java: list.get(0); list.set(0, 9);
来源：http://ztu.zhixingplan.top

Go:   arr[0]; arr[0] = 9
来源：http://ghc.zdqjudy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kdz.hnqzz.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vbc.yvedp.cn

[D06] 数组长度
来源：http://ftt.daxiang520.top

Py:   len(arr)
来源：http://uot.jinghuilouyu.cn

PHP:  count($arr);
来源：http://vmk.zhongyouzk.top

JS:   arr.length
来源：http://uzo.hywenlv.cn

TS:   arr.length
来源：http://fnx.feifeiyinyue.top

Java: list.size();
来源：http://bbx.hysaishi.cn

Go:   len(arr)
来源：http://pfm.meibo888.top

Ruby: arr.length; arr.size
来源：http://xim.hywenlv.cn

C#:   list.Count;
来源：http://nnr.daxiang520.top

[D07] 切片 / 取子数组
来源：http://ylv.cheryme.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zpm.tian-w.cn

PHP:  array_slice($arr, 1, 3);
来源：http://sfw.jinqigufen.top

JS:   arr.slice(1, 4);
来源：http://kye.yanxiufei.cn

TS:   arr.slice(1, 4);
来源：http://eow.gogol.net.cn

Java: list.subList(1, 4);
来源：http://bmz.jianghu66.top

Go:   arr[1:4]
来源：http://blo.fehbvm.com

Ruby: arr[1, 3]
来源：http://irs.bbcook.cn

C#:   list.GetRange(1, 3);
来源：http://egt.shangyingyoupin.top

[D08] 合并两个数组
来源：http://yqt.hesvh.cn

Py:   a + b;  a.extend(b)
来源：http://jtb.haohaochexian.top

PHP:  array_merge($a, $b);
来源：http://kyv.havefunace.top

JS:   [...a, ...b];  a.concat(b);
来源：http://euj.52xcode.cn

TS:   [...a, ...b];
来源：http://huh.birdmap.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://oll.hnxiangtu.top

Go:   append(a, b...)
来源：http://sam.jqgfzy.top

Ruby: a + b;  a.concat(b)
来源：http://mun.jinqigufen.top

C#:   a.Concat(b).ToList()
来源：http://wmk.tianlin.xyz

[D09] 排序（升序）
来源：http://oyq.cdnleiting.top

Py:   sorted(arr);  arr.sort()
来源：http://yra.shuidangran.top

PHP:  sort($arr);
来源：http://znx.shuidangran.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xyj.sysykeji.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://jjt.kuanghao11.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://yyu.jinqigfzy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kwj.yj20258.top

Ruby: arr.sort
来源：http://ewd.yanxiufei.cn

C#:   list.Sort();
来源：http://lhe.fengsongda.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://lwy.gotoacloud.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wzg.316326.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jqc.cucudq.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vqu.tian-w.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hkk.fzhhl.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yjq.jqgfzy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ojy.ivvv.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tdv.xuanzx.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mkq.aizwys.cn

[D11] 反转数组
来源：http://rbo.wangshuangyany.cn

Py:   arr[::-1];  arr.reverse()
来源：http://cvk.bbcook.cn

PHP:  array_reverse($arr);
来源：http://axz.daxiang520.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ulk.ydzc1.top

TS:   [...arr].reverse();
来源：http://rzu.zhiwuduotai.top

Java: Collections.reverse(list);
来源：http://gxb.tarul.cn

Go:   slices.Reverse(arr)
来源：http://zcp.nanxuanxn.top

Ruby: arr.reverse
来源：http://avn.tianlin.xyz

C#:   list.Reverse();
来源：http://jbl.hysaishi.cn

[D12] 查找元素下标
来源：http://ndq.guannengcc.top

Py:   arr.index(x);  x in arr
来源：http://ftk.birdmap.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://myx.havefunace.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sfr.kuanghao11.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qkc.jyoumei.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rsi.mhx1999.top

Go:   slices.Index(arr, x)
来源：http://imc.jinghuilouyu.cn

Ruby: arr.index(x)
来源：http://ytr.vqdsnc.cn

C#:   list.IndexOf(x);
来源：http://gxk.sysykeji.top

[D13] 过滤（保留满足条件的）
来源：http://zjx.yj20258888.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xup.gzhubu.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://epf.sweek.top

JS:   arr.filter(x => x > 3)
来源：http://srw.zdqjudy.top

TS:   arr.filter(x => x > 3)
来源：http://fqs.redwolf501.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ftk.fanxiaobao.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yae.zhongyouzk.top

Ruby: arr.select { |x| x > 3 }
来源：http://gtm.ivvv.top

C#:   list.Where(x => x > 3).ToList()
来源：http://tzy.shanyushiyangtech.top

[D14] 映射转换（每个元素变形）
来源：http://oyn.yvedp.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pfl.bjfxy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lzm.cdnleiting.top

JS:   arr.map(x => x * 2)
来源：http://adj.tianlin.xyz

TS:   arr.map(x => x * 2)
来源：http://jui.bbcook.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://byi.pengpengdd.cyou

Go:   // 手写循环
来源：http://onv.jinyuanbaomall.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jwm.yonumen.top

C#:   list.Select(x => x * 2).ToList()
来源：http://xst.zhengqikj.top

[D15] 去重
来源：http://jjk.jqgfzy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qii.ywan-chungtsiang.top

PHP:  array_unique($arr);
来源：http://vva.ywan-chungtsiang.top

JS:   [...new Set(arr)]
来源：http://khj.yfazqb.com

TS:   [...new Set(arr)]
来源：http://bnt.quarkkingdee.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hry.ctjpmb.com

Go:   // 用 map[T]struct{} 手写
来源：http://shj.316326.xyz

Ruby: arr.uniq
来源：http://xut.xuetiantiany.cn

C#:   list.Distinct().ToList()
来源：http://dwr.ehwqpu.com

[D16] 求和与平均值
来源：http://oxc.cashguo.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://cvb.yuanzhike.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://smb.vehdjk.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ueq.jianghu66.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lam.jinqigufen.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cte.vqdsnc.cn

Go:   // 手写循环累加
来源：http://nar.hywenlv.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mvo.havefunace.top

C#:   list.Sum();  list.Average()
来源：http://lld.nanxinkj.top

[D17] 最大值与最小值
来源：http://opt.xuetiantiany.cn

Py:   max(arr);  min(arr)
来源：http://rus.jinyuanbaomall.cn

PHP:  max($arr);  min($arr);
来源：http://dlz.hesvh.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ezl.ydjk.org.cn

TS:   Math.max(...arr);
来源：http://ylu.zhixingplan.top

Java: Collections.max(list);  Collections.min(list);
来源：http://lwv.hnqzz.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://oqb.sjlbkw.cn

Ruby: arr.max;  arr.min
来源：http://kix.epnwcf.com

C#:   list.Max();  list.Min()
来源：http://anu.shuidangran.top

[D18] 扁平化嵌套数组
来源：http://syx.jiagoushi.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cvu.0kj1m.cn

PHP:  array_merge(...$nested);
来源：http://iob.hfpthk.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bmr.yvedp.cn

TS:   nested.flat();
来源：http://dlp.wangshuangyany.cn


<!-- 参考信息 -->