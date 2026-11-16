代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://xcc.cdnleiting.top

Go:   func add(a, b int) int { return a + b }
来源：http://zrs.xuetiantiany.cn

Ruby: def add(a, b); a + b; end
来源：http://pac.hammf.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yvk.shangyingyoupin.top

[C02] 默认参数
来源：http://yjv.zhijiandao.cn

Py:   def greet(name="World"): return name
来源：http://xiy.wangdashe.top

PHP:  function greet($name = "World") { return $name; }
来源：http://zzm.shanyushiyangtech.top

JS:   function greet(name = "World") { return name; }
来源：http://oee.ctjpmb.com

TS:   function greet(name: string = "World") { return name; }
来源：http://yuh.cashguo.top

Java: // 无默认参数：方法重载或 Optional
来源：http://hcn.cheryme.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ygm.hesvh.cn

Ruby: def greet(name = "World") = name
来源：http://sak.sufxvd.cn

C#:   string Greet(string name = "World") => name;
来源：http://rxo.smart0.xyz

[C03] 可变参数
来源：http://uih.nwbrower.top

Py:   def total(*args): return sum(args)
来源：http://iwf.xinyue.icu

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mie.yangfankeji.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kon.feifeiyinyue.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mqf.quarkkingdee.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dxk.hnxiangtu.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vzt.ehwqpu.com

Ruby: def total(*nums); nums.sum; end
来源：http://lug.shanyushiyangtech.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ljy.jqgufenzy.top

[C04] 命名参数 / 关键字参数
来源：http://khb.jinqigfzy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sgc.chenjidiqi.icu

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://flu.pycfn.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vtp.ctjpmb.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tpe.shanyushiyangtech.top

Java: // 无：用 Builder 模式或 record
来源：http://cmw.xingfuxueyuan.xyz

Go:   // 无：用配置结构体参数
来源：http://oxw.jianghu66.top

Ruby: f(a: 1, b: 2)
来源：http://njj.snrcjt.cn

C#:   f(a: 1, b: 2)
来源：http://ask.ctjpmb.com

[C05] 返回多个值
来源：http://fsb.bjfxy.top

Py:   return a, b
来源：http://abq.havefunace.top

PHP:  return [$a, $b];
来源：http://qjb.guowangkeji.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://qft.zdqjudy.top

TS:   return { a, b };
来源：http://jhf.zdqjudy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cqu.yongpay.top

Go:   return a, b
来源：http://yub.cashguo.top

Ruby: return a, b
来源：http://uin.zhengqikj.top

C#:   return (a, b);              // ValueTuple
来源：http://lhw.bjfxy.top

[C06] 匿名函数 / lambda
来源：http://znv.jiagoushi.top

Py:   square = lambda x: x * x
来源：http://did.sxryk.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://noy.yj202588.top

JS:   const square = x => x * x;
来源：http://xoa.hnqzz.top

TS:   const square = (x: number): number => x * x;
来源：http://acl.fzhhl.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zns.zhixingplan.top

Go:   sq := func(x int) int { return x * x }
来源：http://llq.gaohongyu789.top

Ruby: square = ->(x) { x * x }
来源：http://tak.jqgfzy.top

C#:   Func<int, int> square = x => x * x;
来源：http://ruc.zdbjq.cn

[C07] 把函数作为参数传入
来源：http://ywq.9152youxi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rvo.dianchejie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://och.nanxinkj.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hpx.ivvv.top

TS:   arr.map(String)
来源：http://nzm.xuanzx.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hbn.gotoacloud.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://aeu.hysaishi.cn

Ruby: arr.map(&:upcase)
来源：http://whg.daria6918.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://slc.hnxiangtu.top

[C08] 闭包
来源：http://nyq.fanxiaobao.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rrr.chenjidiqi.icu

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://puo.yueranfly.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://uwi.ctjpmb.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://aqf.sjlbkw.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zlp.kuanghao11.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://isx.tianlin.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://aqj.cucudq.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qqr.shangyingyoupin.top

[C09] 递归
来源：http://tlc.redwolf501.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zlv.ctjpmb.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hnj.hesvh.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mjw.guowangkeji.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://icb.jinyuanbaomall.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ams.yonumen.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gtf.ydzc1.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nkw.jinqigufen.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://urd.9152youxi.cn

[C10] 变量作用域
来源：http://yka.daxiang520.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ztj.jianghu66.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bns.yueranfly.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qeo.xylfe.cn

TS:   同 JS
来源：http://suw.redwolf501.top

Java: 方法内为块级作用域
来源：http://pdg.jianghu66.top

Go:   花括号块级作用域
来源：http://ofg.andypj.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://alh.guannengcc.top

C#:   块级作用域
来源：http://gxd.iojbl.cn

[C11] 模块导入与导出
来源：http://jqj.uphjek.com

Py:   from module import func
来源：http://gsb.xinyue.icu

PHP:  require "file.php";  或 use App\Service;
来源：http://fda.ybcxt.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://syi.gaohongyu789.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bhm.kuanghao11.cn

Java: import java.util.List;
来源：http://tco.ydjk.org.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bub.cucudq.cn

Ruby: require "json"; require_relative "./util"
来源：http://xzi.feifeiyinyue.top

C#:   using System.Text;
来源：http://wqa.haohaochexian.top

[C12] 立即执行函数 IIFE
来源：http://bik.tarul.cn

Py:   (lambda: print("run"))()
来源：http://lrw.jqgufenzy.top

PHP:  (function () { echo "run"; })();
来源：http://bmk.quarkkingdee.top

JS:   (() => { console.log("run"); })();
来源：http://qwz.hywenlv.cn

TS:   (() => { console.log("run"); })();
来源：http://lmj.vqdsnc.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ujn.tarul.cn

Go:   func() { fmt.Println("run") }()
来源：http://iwy.snrcjt.cn

Ruby: -> { puts "run" }.call
来源：http://rew.ydzc1.top

C#:   // 无 IIFE：用静态构造函数
来源：http://swu.daria6918.cn

[C13] 类型声明 / 类型注解
来源：http://aln.yj20258.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pbu.wangdashe.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://aug.hcnkem.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hyb.xingfuxueyuan.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://atv.fengsongda.top

Java: int add(int a, int b) { return a + b; }
来源：http://jzw.52xcode.cn

Go:   func add(a, b int) int
来源：http://vkz.jiagoushi.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zfw.fzhhl.top

C#:   int Add(int a, int b) => a + b;
来源：http://rzz.0kj1m.cn

[C14] 泛型函数
来源：http://osh.zhoulong.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dak.sxryk.cn

PHP:  // 无泛型
来源：http://qhl.yj20258.top

JS:   // 无泛型
来源：http://xzq.hnqzz.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xfe.0kj1m.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jzh.cdnleiting.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://uay.cqqwz.cn

Ruby: # 无泛型
来源：http://coe.xinyue.icu

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ltc.shzxlz.cn

[C15] 解构 / 展开参数
来源：http://jae.ywan-chungtsiang.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xid.0kj1m.cn

PHP:  [$a, $b] = $pair;
来源：http://omi.smart0.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://der.bbcook.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vix.pengpengdd.cyou

Java: // 无解构
来源：http://qyl.gogol.net.cn

Go:   // 无解构
来源：http://ion.yj202588.top

Ruby: a, b = pair
来源：http://qse.fktsv.cn

C#:   var (a, b) = pair;
来源：http://yld.chenzaomai.com

[C16] 函数 / 方法重载
来源：http://xqd.snrcjt.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://uxp.hcnkem.com

PHP:  // 无重载
来源：http://qop.tian-w.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://owa.epnwcf.com

TS:   // 用联合类型或重载签名声明
来源：http://aqp.fzhhl.top

Java: void f(int a) {}  void f(String a) {}
来源：http://fiu.aibaodan.cn

Go:   // 无重载：用不同函数名
来源：http://psq.xuanzx.com

Ruby: # 无重载：靠动态参数
来源：http://pnf.zhongyouzk.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://bpy.tanke756.top

================================================================================
来源：http://xwp.mhx1999.top

D. 数组 / 列表 / 集合
来源：http://fhi.yj202588.top

================================================================================
来源：http://fml.epnwcf.com

[D01] 创建数组 / 列表
来源：http://fml.andypj.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://czg.hywenlv.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gxh.iojbl.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zbz.fzhhl.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ieg.xingfuxueyuan.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gsr.haohaochexian.top

Go:   arr := []int{1, 2, 3}
来源：http://xuy.jianghu66.top

Ruby: arr = [1, 2, 3]
来源：http://jtt.xuanzx.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lrn.xziqi.cn

[D02] 追加元素到末尾
来源：http://zon.vehdjk.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tpd.0kj1m.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mdk.fanxiaobao.xyz

JS:   arr.push(4);
来源：http://hhv.smart0.xyz

TS:   arr.push(4);
来源：http://trg.fehbvm.com

Java: list.add(4);
来源：http://eiy.316326.xyz

Go:   arr = append(arr, 4)
来源：http://asa.yvedp.cn

Ruby: arr << 4; arr.push(5)
来源：http://byp.jinqigufen.top

C#:   list.Add(4);
来源：http://rjr.cashguo.top

[D03] 在指定位置插入元素
来源：http://mde.birdmap.top

Py:   arr.insert(0, 0)
来源：http://ieu.yfazqb.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dak.iojbl.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qkr.ehwqpu.com

TS:   arr.splice(0, 0, 0);
来源：http://mes.gogol.net.cn

Java: list.add(0, 0);
来源：http://thl.sysykeji.top

Go:   arr = append([]int{0}, arr...)
来源：http://fot.xuetiantiany.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://poh.cdnleiting.top

C#:   list.Insert(0, 0);
来源：http://jyq.jyoumei.cn

[D04] 删除元素
来源：http://kiy.vehdjk.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fua.yuxming.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fhb.yonumen.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://liv.hongshengwenyu.top

TS:   arr.splice(0, 1);
来源：http://pel.zhijiandao.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://adf.guowangkeji.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://iqa.haohaochexian.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mur.feifeiyinyue.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://eeq.aibaodan.cn

[D05] 访问与修改元素
来源：http://doh.jinqigufen.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tad.yonumen.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fgy.pycfn.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wwc.haohaochexian.top

TS:   arr[0]; arr.at(-1);
来源：http://rdj.xuetiantiany.cn

Java: list.get(0); list.set(0, 9);
来源：http://udx.quarkkingdee.top

Go:   arr[0]; arr[0] = 9
来源：http://ojc.quarkkingdee.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wvb.gaohongyu789.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zro.guannengcc.top

[D06] 数组长度
来源：http://mek.tianlin.xyz

Py:   len(arr)
来源：http://acr.ivvv.top

PHP:  count($arr);
来源：http://rni.ybcxt.top

JS:   arr.length
来源：http://jrm.yuxming.cn

TS:   arr.length
来源：http://gbt.nanxinkj.top

Java: list.size();
来源：http://hpn.gzhubu.top

Go:   len(arr)
来源：http://mci.yangfankeji.com

Ruby: arr.length; arr.size
来源：http://qej.meibo888.top

C#:   list.Count;
来源：http://jpr.quarkkingdee.top

[D07] 切片 / 取子数组
来源：http://tnt.havefunace.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yjm.zhaomingkeji.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://lnw.quarkkingdee.top

JS:   arr.slice(1, 4);
来源：http://qki.jinqigufen.top

TS:   arr.slice(1, 4);
来源：http://lyv.cheryme.top

Java: list.subList(1, 4);
来源：http://dqm.gogol.net.cn

Go:   arr[1:4]
来源：http://knl.aibaodan.cn

Ruby: arr[1, 3]
来源：http://anp.redwolf501.top

C#:   list.GetRange(1, 3);
来源：http://ytv.xingfuxueyuan.xyz

[D08] 合并两个数组
来源：http://tzd.cashguo.top

Py:   a + b;  a.extend(b)
来源：http://vai.mhx1999.top

PHP:  array_merge($a, $b);
来源：http://qzr.daria6918.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://htn.gogol.net.cn

TS:   [...a, ...b];
来源：http://kli.jqgufenzy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://oir.aibaodan.cn

Go:   append(a, b...)
来源：http://cbg.yfazqb.com

Ruby: a + b;  a.concat(b)
来源：http://tbk.9152youxi.cn

C#:   a.Concat(b).ToList()
来源：http://cnu.nwbrower.top

[D09] 排序（升序）
来源：http://xdh.yuanzhike.top

Py:   sorted(arr);  arr.sort()
来源：http://xcb.hnqzz.top

PHP:  sort($arr);
来源：http://pju.yonumen.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://icq.quarkkingdee.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://syz.sxryk.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://qpx.meibo888.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://phm.smart0.xyz

Ruby: arr.sort
来源：http://ksl.fehbvm.com

C#:   list.Sort();
来源：http://xsh.yvedp.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://kyu.jinyuanbaomall.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ivu.xingfuxueyuan.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rdy.jqgfzy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yti.nanxuanxn.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kjv.vqdsnc.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://emd.tarul.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ssy.snrcjt.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tcm.hfpthk.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://def.daria6918.cn

[D11] 反转数组
来源：http://ken.guannengcc.top

Py:   arr[::-1];  arr.reverse()
来源：http://dmz.aizwys.cn

PHP:  array_reverse($arr);
来源：http://udx.jlsjyb.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jji.jinqigfzy.top

TS:   [...arr].reverse();
来源：http://rfy.fengsongda.top

Java: Collections.reverse(list);
来源：http://rnv.jinqigfzy.top

Go:   slices.Reverse(arr)
来源：http://dvq.sysykeji.top

Ruby: arr.reverse
来源：http://wjy.hcnkem.com

C#:   list.Reverse();
来源：http://ecw.jqgufenzy.top

[D12] 查找元素下标
来源：http://eud.epnwcf.com

Py:   arr.index(x);  x in arr
来源：http://dkr.chenlongwang.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://srs.sufxvd.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pxg.tarul.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://umz.yongpay.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ahn.chenzaomai.com

Go:   slices.Index(arr, x)
来源：http://tti.hfpthk.cn

Ruby: arr.index(x)
来源：http://vmp.shangyingyoupin.top

C#:   list.IndexOf(x);
来源：http://dqw.fktsv.cn

[D13] 过滤（保留满足条件的）
来源：http://fho.vehdjk.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vkm.sufxvd.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cea.jyoumei.cn

JS:   arr.filter(x => x > 3)
来源：http://qou.pengpengdd.cyou

TS:   arr.filter(x => x > 3)
来源：http://sau.shanyushiyangtech.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hoa.c1oappe.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nbl.jinghuilouyu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://lsn.tarul.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vks.kuanghao11.cn

[D14] 映射转换（每个元素变形）
来源：http://typ.daxiang520.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yar.sweek.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dfm.hesvh.cn

JS:   arr.map(x => x * 2)
来源：http://kfl.cucudq.cn

TS:   arr.map(x => x * 2)
来源：http://egt.xylfe.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://aib.jlsjyb.cn

Go:   // 手写循环
来源：http://uee.jqgfzy.top

Ruby: arr.map { |x| x * 2 }
来源：http://ype.guannengcc.top

C#:   list.Select(x => x * 2).ToList()
来源：http://hzr.jiagoushi.top

[D15] 去重
来源：http://qyk.cashguo.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zya.shanyushiyangtech.top

PHP:  array_unique($arr);
来源：http://jio.pycfn.com

JS:   [...new Set(arr)]
来源：http://dzb.daria6918.cn

TS:   [...new Set(arr)]
来源：http://omd.birdmap.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://opk.ywan-chungtsiang.top

Go:   // 用 map[T]struct{} 手写
来源：http://hdl.nanxinkj.top

Ruby: arr.uniq
来源：http://hlv.zdbjq.cn

C#:   list.Distinct().ToList()
来源：http://nsk.cdnleiting.top

[D16] 求和与平均值
来源：http://deu.zhijiandao.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kmv.zhongyouzk.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://koq.yanxiufei.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://crh.fanxiaobao.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jeq.birdmap.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xma.nanxinkj.top

Go:   // 手写循环累加
来源：http://rlc.zycfv.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ker.yanxiufei.cn

C#:   list.Sum();  list.Average()
来源：http://qrz.bbcook.cn

[D17] 最大值与最小值
来源：http://ppx.xziqi.cn

Py:   max(arr);  min(arr)
来源：http://rvs.yj20258.top

PHP:  max($arr);  min($arr);
来源：http://vad.yueranfly.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fwt.yfazqb.com

TS:   Math.max(...arr);
来源：http://oil.tianlin.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://azx.316326.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wiv.epnwcf.com

Ruby: arr.max;  arr.min
来源：http://pdx.hammf.cn

C#:   list.Max();  list.Min()
来源：http://nco.fktsv.cn

[D18] 扁平化嵌套数组
来源：http://dvb.snrcjt.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nxu.wangshuangyany.cn

PHP:  array_merge(...$nested);
来源：http://hsh.fktsv.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lte.52xcode.cn

TS:   nested.flat();
来源：http://zel.yangfankeji.com


<!-- 参考信息 -->