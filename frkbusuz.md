代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://gqy.vehdjk.com

[C03] 可变参数
来源：http://jau.yj20258.top

Py:   def total(*args): return sum(args)
来源：http://qxc.guannengcc.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rni.tianlin.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pnw.yj20258.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xst.guannengcc.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hym.feifeiyinyue.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pwh.smart0.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://onm.daria6918.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cho.zhongyouzk.top

[C04] 命名参数 / 关键字参数
来源：http://ucf.ivvv.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dbh.fengsongda.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://btp.iojbl.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://emj.yfazqb.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hte.yonumen.top

Java: // 无：用 Builder 模式或 record
来源：http://wfr.wangdashe.top

Go:   // 无：用配置结构体参数
来源：http://eez.jinqigufen.top

Ruby: f(a: 1, b: 2)
来源：http://adg.nanxuanxn.top

C#:   f(a: 1, b: 2)
来源：http://but.aibaodan.cn

[C05] 返回多个值
来源：http://hbt.zhongyouzk.top

Py:   return a, b
来源：http://yoh.zhengqikj.top

PHP:  return [$a, $b];
来源：http://qsj.daxiang520.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://vty.c1oappe.top

TS:   return { a, b };
来源：http://jjs.fzhhl.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://emp.sjlbkw.cn

Go:   return a, b
来源：http://xkw.sysykeji.top

Ruby: return a, b
来源：http://dbj.cheryme.top

C#:   return (a, b);              // ValueTuple
来源：http://amd.jyoumei.cn

[C06] 匿名函数 / lambda
来源：http://fvj.jyoumei.cn

Py:   square = lambda x: x * x
来源：http://qru.daria6918.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://bem.sweek.top

JS:   const square = x => x * x;
来源：http://vcl.pycfn.com

TS:   const square = (x: number): number => x * x;
来源：http://ygl.yuxming.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hxw.mhx1999.top

Go:   sq := func(x int) int { return x * x }
来源：http://vev.aibaodan.cn

Ruby: square = ->(x) { x * x }
来源：http://pje.xinyue.icu

C#:   Func<int, int> square = x => x * x;
来源：http://bfh.shanyushiyangkeji.top

[C07] 把函数作为参数传入
来源：http://pph.jiagoushi.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://low.hnxiangtu.top

PHP:  array_map("strtoupper", $arr);
来源：http://wch.smart0.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dlw.smart0.xyz

TS:   arr.map(String)
来源：http://vwb.cqqwz.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://clh.0kj1m.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cbl.yangfankeji.com

Ruby: arr.map(&:upcase)
来源：http://xsa.aibaodan.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://lji.meibo888.top

[C08] 闭包
来源：http://gsa.tarul.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tzl.fanxiaobao.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yqg.xuanzx.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qhi.zhengqikj.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vov.hammf.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yvi.zhoulong.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://aad.iojbl.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fnw.sufxvd.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xsp.cdnleiting.top

[C09] 递归
来源：http://wzp.hnqzz.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ppo.fengsongda.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xsx.yj20258.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://muw.gogol.net.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://axn.chenzaomai.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tdw.hcnkem.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fyw.wangdashe.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kkn.fanxiaobao.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tcr.ehwqpu.com

[C10] 变量作用域
来源：http://qsj.ydzc1.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hzu.gotoacloud.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nrm.svipenyu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://zwb.xinyue.icu

TS:   同 JS
来源：http://fix.ehwqpu.com

Java: 方法内为块级作用域
来源：http://udq.aizwys.cn

Go:   花括号块级作用域
来源：http://hgh.yj202588.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jsn.sxryk.cn

C#:   块级作用域
来源：http://nkn.wangdashe.top

[C11] 模块导入与导出
来源：http://kom.wangdashe.top

Py:   from module import func
来源：http://qdx.nwbrower.top

PHP:  require "file.php";  或 use App\Service;
来源：http://gnx.yanxiufei.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://dwo.havefunace.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fqt.jianghu66.top

Java: import java.util.List;
来源：http://fep.yj20258.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zpu.ydzc1.top

Ruby: require "json"; require_relative "./util"
来源：http://ief.yj20258888.top

C#:   using System.Text;
来源：http://pdv.shanyushiyangtech.top

[C12] 立即执行函数 IIFE
来源：http://jhp.jyoumei.cn

Py:   (lambda: print("run"))()
来源：http://tzn.yonumen.top

PHP:  (function () { echo "run"; })();
来源：http://qef.jlsjyb.cn

JS:   (() => { console.log("run"); })();
来源：http://dmy.zhongyouzk.top

TS:   (() => { console.log("run"); })();
来源：http://upo.chenlongwang.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ypc.nwbrower.top

Go:   func() { fmt.Println("run") }()
来源：http://ajh.aizwys.cn

Ruby: -> { puts "run" }.call
来源：http://cyy.zhijiandao.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://mgv.sjlbkw.cn

[C13] 类型声明 / 类型注解
来源：http://odh.yj20258.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://grc.xziqi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wug.havefunace.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://djk.ctjpmb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kaa.jiagoushi.top

Java: int add(int a, int b) { return a + b; }
来源：http://sor.hfpthk.cn

Go:   func add(a, b int) int
来源：http://rtr.feifeiyinyue.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://otu.yfazqb.com

C#:   int Add(int a, int b) => a + b;
来源：http://vkm.snrcjt.cn

[C14] 泛型函数
来源：http://tja.fktsv.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ehj.aizwys.cn

PHP:  // 无泛型
来源：http://rez.vqdsnc.cn

JS:   // 无泛型
来源：http://xzf.zhijiandao.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://usi.yuanzhike.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dfd.pycfn.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cba.haohaochexian.top

Ruby: # 无泛型
来源：http://ugh.yonumen.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://oph.iojbl.cn

[C15] 解构 / 展开参数
来源：http://sph.jianghu66.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://eof.yuxming.cn

PHP:  [$a, $b] = $pair;
来源：http://vnb.fengsongda.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dip.yj20258.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tuq.chenjidiqi.icu

Java: // 无解构
来源：http://qpu.hywenlv.cn

Go:   // 无解构
来源：http://knz.pengpengdd.cyou

Ruby: a, b = pair
来源：http://yeh.chenzaomai.com

C#:   var (a, b) = pair;
来源：http://ofs.zhijiandao.cn

[C16] 函数 / 方法重载
来源：http://zxr.gogol.net.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vjc.xingfuxueyuan.xyz

PHP:  // 无重载
来源：http://igg.yfazqb.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://agn.hammf.cn

TS:   // 用联合类型或重载签名声明
来源：http://vlx.daria6918.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://jqq.chenlongwang.top

Go:   // 无重载：用不同函数名
来源：http://hcq.xingfuxueyuan.xyz

Ruby: # 无重载：靠动态参数
来源：http://lxe.hesvh.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://bir.xinyue.icu

================================================================================
来源：http://shb.fehbvm.com

D. 数组 / 列表 / 集合
来源：http://gnf.yuanzhike.top

================================================================================
来源：http://yet.haohaochexian.top

[D01] 创建数组 / 列表
来源：http://kxk.xylfe.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://eik.jinyuanbaomall.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vmv.svipenyu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://akj.uphjek.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://hfk.fktsv.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://uiu.kuanghao11.cn

Go:   arr := []int{1, 2, 3}
来源：http://gkq.fktsv.cn

Ruby: arr = [1, 2, 3]
来源：http://dpi.ehwqpu.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pcu.hnxiangtu.top

[D02] 追加元素到末尾
来源：http://wub.yj20258.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cuv.yuxming.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://voy.tianlin.xyz

JS:   arr.push(4);
来源：http://rdq.hywenlv.cn

TS:   arr.push(4);
来源：http://pbp.cdnleiting.top

Java: list.add(4);
来源：http://rzx.ybcxt.top

Go:   arr = append(arr, 4)
来源：http://qbc.hfpthk.cn

Ruby: arr << 4; arr.push(5)
来源：http://kcm.daria6918.cn

C#:   list.Add(4);
来源：http://pql.aibaodan.cn

[D03] 在指定位置插入元素
来源：http://gqa.guannengcc.top

Py:   arr.insert(0, 0)
来源：http://lta.cheryme.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dgr.guowangkeji.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://oam.cucudq.cn

TS:   arr.splice(0, 0, 0);
来源：http://kva.sjlbkw.cn

Java: list.add(0, 0);
来源：http://unv.cheryme.top

Go:   arr = append([]int{0}, arr...)
来源：http://dun.hysaishi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gkt.yongpay.top

C#:   list.Insert(0, 0);
来源：http://csh.smart0.xyz

[D04] 删除元素
来源：http://etf.havefunace.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qop.jlsjyb.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tqh.andypj.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nno.yfazqb.com

TS:   arr.splice(0, 1);
来源：http://uxa.ehwqpu.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fgj.haohaochexian.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://aqs.yongpay.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ydo.quarkkingdee.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mqr.zhengqikj.top

[D05] 访问与修改元素
来源：http://blm.gotoacloud.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://izz.sweek.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wbn.fzhhl.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pcr.hywenlv.cn

TS:   arr[0]; arr.at(-1);
来源：http://flq.vehdjk.com

Java: list.get(0); list.set(0, 9);
来源：http://ktp.kuanghao11.cn

Go:   arr[0]; arr[0] = 9
来源：http://ofj.316326.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bfd.cucudq.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dub.pengpengdd.cyou

[D06] 数组长度
来源：http://wyj.zhiwuduotai.top

Py:   len(arr)
来源：http://amh.sysykeji.top

PHP:  count($arr);
来源：http://ubk.ybcxt.top

JS:   arr.length
来源：http://tsl.fzhhl.top

TS:   arr.length
来源：http://twg.sxryk.cn

Java: list.size();
来源：http://eco.ppjwa.cn

Go:   len(arr)
来源：http://xev.chenlongwang.top

Ruby: arr.length; arr.size
来源：http://zek.snrcjt.cn

C#:   list.Count;
来源：http://ugo.jinqigfzy.top

[D07] 切片 / 取子数组
来源：http://cwb.epnwcf.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qrd.cashguo.top

PHP:  array_slice($arr, 1, 3);
来源：http://ves.dashuyun.cn

JS:   arr.slice(1, 4);
来源：http://sbf.vqdsnc.cn

TS:   arr.slice(1, 4);
来源：http://lpt.vehdjk.com

Java: list.subList(1, 4);
来源：http://ben.zhiwuduotai.top

Go:   arr[1:4]
来源：http://eyn.ywan-chungtsiang.top

Ruby: arr[1, 3]
来源：http://iro.xziqi.cn

C#:   list.GetRange(1, 3);
来源：http://eyq.havefunace.top

[D08] 合并两个数组
来源：http://fcf.hesvh.cn

Py:   a + b;  a.extend(b)
来源：http://txa.sjlbkw.cn

PHP:  array_merge($a, $b);
来源：http://qin.aizwys.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://chq.hnqzz.top

TS:   [...a, ...b];
来源：http://bqf.cheryme.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://oap.ydzc1.top

Go:   append(a, b...)
来源：http://bwd.wangshuangyany.cn

Ruby: a + b;  a.concat(b)
来源：http://dod.svipenyu.cn

C#:   a.Concat(b).ToList()
来源：http://dke.bbcook.cn

[D09] 排序（升序）
来源：http://xbg.shanyushiyangtech.top

Py:   sorted(arr);  arr.sort()
来源：http://nuy.xuanzx.com

PHP:  sort($arr);
来源：http://qtd.hcnkem.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pio.chenzaomai.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://mwv.hongshengwenyu.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ifw.daxiang520.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://suy.zdbjq.cn

Ruby: arr.sort
来源：http://nny.redwolf501.top

C#:   list.Sort();
来源：http://hwt.birdmap.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://cyz.ppjwa.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://svt.hongshengwenyu.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jdv.xinyue.icu

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bsd.jlsjyb.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zdt.epnwcf.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nij.nwbrower.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gfg.316326.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://eov.wangshuangyany.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://faa.havefunace.top

[D11] 反转数组
来源：http://rcp.daria6918.cn

Py:   arr[::-1];  arr.reverse()
来源：http://owf.ywan-chungtsiang.top

PHP:  array_reverse($arr);
来源：http://wty.yj20258888.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lif.ivvv.top

TS:   [...arr].reverse();
来源：http://cta.jlsjyb.cn

Java: Collections.reverse(list);
来源：http://eqy.yangfankeji.com

Go:   slices.Reverse(arr)
来源：http://nqj.birdmap.top

Ruby: arr.reverse
来源：http://pbj.jyoumei.cn

C#:   list.Reverse();
来源：http://epl.tianlin.xyz

[D12] 查找元素下标
来源：http://zhp.guannengcc.top

Py:   arr.index(x);  x in arr
来源：http://icb.yongpay.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kzm.52xcode.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hpc.bbcook.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wyx.pycfn.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hzz.snrcjt.cn

Go:   slices.Index(arr, x)
来源：http://vqa.tianlin.xyz

Ruby: arr.index(x)
来源：http://gej.nanxuanxn.top

C#:   list.IndexOf(x);
来源：http://vyf.epnwcf.com

[D13] 过滤（保留满足条件的）
来源：http://zik.hnxiangtu.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kyl.sweek.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://udh.sjlbkw.cn

JS:   arr.filter(x => x > 3)
来源：http://huz.jyoumei.cn

TS:   arr.filter(x => x > 3)
来源：http://wzd.guowangkeji.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nwy.xuetiantiany.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://sjm.sufxvd.cn

Ruby: arr.select { |x| x > 3 }
来源：http://pog.cdnleiting.top

C#:   list.Where(x => x > 3).ToList()
来源：http://fdg.fktsv.cn

[D14] 映射转换（每个元素变形）
来源：http://bgh.andypj.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mde.fanxiaobao.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yxt.epnwcf.com

JS:   arr.map(x => x * 2)
来源：http://xsf.mhx1999.top

TS:   arr.map(x => x * 2)
来源：http://ktn.mhx1999.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://uju.gaohongyu789.top

Go:   // 手写循环
来源：http://uts.jqgufenzy.top

Ruby: arr.map { |x| x * 2 }
来源：http://lix.hesvh.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://erl.daria6918.cn

[D15] 去重
来源：http://ole.ybcxt.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://eqt.cqqwz.cn

PHP:  array_unique($arr);
来源：http://uvs.epnwcf.com

JS:   [...new Set(arr)]
来源：http://otc.ybcxt.top

TS:   [...new Set(arr)]
来源：http://prc.quarkkingdee.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fxz.dianchejie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ang.zhijiandao.cn

Ruby: arr.uniq
来源：http://rfb.ivvv.top

C#:   list.Distinct().ToList()
来源：http://ugf.jinqigufen.top

[D16] 求和与平均值
来源：http://ypf.tarul.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://oyj.hnxiangtu.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ctl.gogol.net.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sqr.jianghu66.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wyq.tanke756.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tnp.52xcode.cn

Go:   // 手写循环累加
来源：http://qeq.sjlbkw.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://phb.jianghu66.top

C#:   list.Sum();  list.Average()
来源：http://ueo.zhaomingkeji.xyz

[D17] 最大值与最小值
来源：http://qul.fehbvm.com

Py:   max(arr);  min(arr)
来源：http://cyu.hcnkem.com

PHP:  max($arr);  min($arr);
来源：http://dgw.gaohongyu789.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zud.dashuyun.cn

TS:   Math.max(...arr);
来源：http://fes.zdbjq.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://jcs.yongpay.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://eps.aizwys.cn

Ruby: arr.max;  arr.min
来源：http://krf.aizwys.cn

C#:   list.Max();  list.Min()
来源：http://nsm.nanxuanxn.top

[D18] 扁平化嵌套数组
来源：http://oth.jqgufenzy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vig.mhx1999.top

PHP:  array_merge(...$nested);
来源：http://asw.smart0.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hbo.zhongyouzk.top

TS:   nested.flat();
来源：http://aln.jinqigufen.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ite.meibo888.top

Go:   // 手写双层循环
来源：http://zpd.havefunace.top

Ruby: nested.flatten
来源：http://cgd.yuxming.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://sao.nanxuanxn.top

[D19] 按字段分组
来源：http://kgq.guannengcc.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://iwo.havefunace.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qji.birdmap.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qks.hcnkem.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://ztc.hammf.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tla.daria6918.cn

Go:   // 手写 map[string][]T
来源：http://qah.wangdashe.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://kde.dianchejie.cn


<!-- 参考信息 -->