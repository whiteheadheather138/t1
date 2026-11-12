代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ypg.fanxiaobao.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wwn.zdbjq.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bzi.nanxinkj.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ldw.jlsjyb.cn

Ruby: def total(*nums); nums.sum; end
来源：http://pzd.birdmap.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cma.hywenlv.cn

[C04] 命名参数 / 关键字参数
来源：http://phd.sweek.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fco.nwbrower.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nse.guowangkeji.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kxl.hnxiangtu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gjw.dianchejie.cn

Java: // 无：用 Builder 模式或 record
来源：http://ear.shzxlz.cn

Go:   // 无：用配置结构体参数
来源：http://msm.guannengcc.top

Ruby: f(a: 1, b: 2)
来源：http://wmj.wangdashe.top

C#:   f(a: 1, b: 2)
来源：http://htd.chenjidiqi.icu

[C05] 返回多个值
来源：http://ecy.zdbjq.cn

Py:   return a, b
来源：http://xrz.kuanghao11.cn

PHP:  return [$a, $b];
来源：http://wqj.fktsv.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://dmf.yuanzhike.top

TS:   return { a, b };
来源：http://voo.wangshuangyany.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ouq.yvedp.cn

Go:   return a, b
来源：http://kkf.dashuyun.cn

Ruby: return a, b
来源：http://xqs.cucudq.cn

C#:   return (a, b);              // ValueTuple
来源：http://qnu.jinqigfzy.top

[C06] 匿名函数 / lambda
来源：http://kom.0kj1m.cn

Py:   square = lambda x: x * x
来源：http://eym.hcnkem.com

PHP:  $square = fn($x) => $x * $x;
来源：http://rhd.gzhubu.top

JS:   const square = x => x * x;
来源：http://riy.hfpthk.cn

TS:   const square = (x: number): number => x * x;
来源：http://pgg.bjfxy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ldf.hongshengwenyu.top

Go:   sq := func(x int) int { return x * x }
来源：http://tmb.dianchejie.cn

Ruby: square = ->(x) { x * x }
来源：http://rsb.fktsv.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qlg.zhixingplan.top

[C07] 把函数作为参数传入
来源：http://pfe.tianlin.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yba.jiagoushi.top

PHP:  array_map("strtoupper", $arr);
来源：http://qns.quarkkingdee.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://spx.chenlongwang.top

TS:   arr.map(String)
来源：http://zer.aizwys.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://njl.yj20258.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qew.meibo888.top

Ruby: arr.map(&:upcase)
来源：http://xjg.ctjpmb.com

C#:   arr.Select(s => s.ToUpper())
来源：http://ylv.zdqjudy.top

[C08] 闭包
来源：http://evm.ivvv.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dja.cdnleiting.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nkw.jqgufenzy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://eya.andypj.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://iuz.cashguo.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://olh.316326.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jzs.cdnleiting.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://igb.jinyuanbaomall.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://oyb.shanyushiyangtech.top

[C09] 递归
来源：http://abb.hywenlv.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hva.sweek.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mtc.ctjpmb.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://adq.cdnleiting.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ukk.ywan-chungtsiang.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dlj.jinghuilouyu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://yak.hnqzz.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vus.epnwcf.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ujh.ivvv.top

[C10] 变量作用域
来源：http://aem.jiagoushi.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://opt.iojbl.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ukl.jianghu66.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://byz.zdbjq.cn

TS:   同 JS
来源：http://mhs.shuidangran.top

Java: 方法内为块级作用域
来源：http://gwv.fzhhl.top

Go:   花括号块级作用域
来源：http://hsf.hcnkem.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yix.epnwcf.com

C#:   块级作用域
来源：http://glh.ydzc1.top

[C11] 模块导入与导出
来源：http://aap.uphjek.com

Py:   from module import func
来源：http://lyo.sysykeji.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ubl.tarul.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://gut.ehwqpu.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zxx.svipenyu.cn

Java: import java.util.List;
来源：http://ygf.redwolf501.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dfk.guannengcc.top

Ruby: require "json"; require_relative "./util"
来源：http://nol.yongpay.top

C#:   using System.Text;
来源：http://kxh.zhongyouzk.top

[C12] 立即执行函数 IIFE
来源：http://vpg.sjlbkw.cn

Py:   (lambda: print("run"))()
来源：http://crz.cdnleiting.top

PHP:  (function () { echo "run"; })();
来源：http://fio.cdnleiting.top

JS:   (() => { console.log("run"); })();
来源：http://hrp.xingfuxueyuan.xyz

TS:   (() => { console.log("run"); })();
来源：http://xmu.hnxiangtu.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://iqu.ywan-chungtsiang.top

Go:   func() { fmt.Println("run") }()
来源：http://cab.hcnkem.com

Ruby: -> { puts "run" }.call
来源：http://ywh.hfpthk.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://wzu.52xcode.cn

[C13] 类型声明 / 类型注解
来源：http://txd.hammf.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ago.tian-w.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://atx.fanxiaobao.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bdc.havefunace.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://boo.shzxlz.cn

Java: int add(int a, int b) { return a + b; }
来源：http://rrm.vehdjk.com

Go:   func add(a, b int) int
来源：http://hcc.yanxiufei.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ztx.9152youxi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://xsv.zhaomingkeji.xyz

[C14] 泛型函数
来源：http://nwp.zhongyouzk.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wju.zdqjudy.top

PHP:  // 无泛型
来源：http://dpd.yuanzhike.top

JS:   // 无泛型
来源：http://xly.xinyue.icu

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kke.yuanzhike.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://taa.zhixingplan.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hxu.c1oappe.top

Ruby: # 无泛型
来源：http://jrw.0kj1m.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lje.bjfxy.top

[C15] 解构 / 展开参数
来源：http://tri.fanxiaobao.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vqd.shanyushiyangtech.top

PHP:  [$a, $b] = $pair;
来源：http://rrq.ppjwa.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nvt.fehbvm.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bag.nanxuanxn.top

Java: // 无解构
来源：http://ctz.tianlin.xyz

Go:   // 无解构
来源：http://qty.iojbl.cn

Ruby: a, b = pair
来源：http://njs.xinyue.icu

C#:   var (a, b) = pair;
来源：http://tvj.snrcjt.cn

[C16] 函数 / 方法重载
来源：http://gwm.hcnkem.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://aqi.hywenlv.cn

PHP:  // 无重载
来源：http://iqq.snrcjt.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://cjt.0kj1m.cn

TS:   // 用联合类型或重载签名声明
来源：http://ffp.shuidangran.top

Java: void f(int a) {}  void f(String a) {}
来源：http://xxd.hnxiangtu.top

Go:   // 无重载：用不同函数名
来源：http://xvq.zhaomingkeji.xyz

Ruby: # 无重载：靠动态参数
来源：http://vko.shanyushiyangkeji.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://yuu.sufxvd.cn

================================================================================
来源：http://ncw.yvedp.cn

D. 数组 / 列表 / 集合
来源：http://wdq.fengsongda.top

================================================================================
来源：http://oju.chenjidiqi.icu

[D01] 创建数组 / 列表
来源：http://beu.yj202588.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://aoe.daria6918.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sjx.c1oappe.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://kcl.sxryk.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://weh.jlsjyb.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://viu.zhiwuduotai.top

Go:   arr := []int{1, 2, 3}
来源：http://voh.zhixingplan.top

Ruby: arr = [1, 2, 3]
来源：http://lej.cashguo.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vog.jinqigufen.top

[D02] 追加元素到末尾
来源：http://rvx.xuetiantiany.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nmg.yangfankeji.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pka.yj202588.top

JS:   arr.push(4);
来源：http://cjt.tianlin.xyz

TS:   arr.push(4);
来源：http://nha.dashuyun.cn

Java: list.add(4);
来源：http://vxy.tarul.cn

Go:   arr = append(arr, 4)
来源：http://tyi.bbcook.cn

Ruby: arr << 4; arr.push(5)
来源：http://oot.havefunace.top

C#:   list.Add(4);
来源：http://sjq.sufxvd.cn

[D03] 在指定位置插入元素
来源：http://nnb.snrcjt.cn

Py:   arr.insert(0, 0)
来源：http://mpe.jyoumei.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://idf.hnxiangtu.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://lsc.zycfv.cn

TS:   arr.splice(0, 0, 0);
来源：http://rkb.aizwys.cn

Java: list.add(0, 0);
来源：http://xex.bjfxy.top

Go:   arr = append([]int{0}, arr...)
来源：http://aao.jianghu66.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xhr.fanxiaobao.xyz

C#:   list.Insert(0, 0);
来源：http://ycu.tanke756.top

[D04] 删除元素
来源：http://sfk.xingfuxueyuan.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://znv.uphjek.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://iod.sweek.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xuc.bjfxy.top

TS:   arr.splice(0, 1);
来源：http://dnu.zhengqikj.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kkf.xingfuxueyuan.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vue.bjfxy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://uyd.316326.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xmq.smart0.xyz

[D05] 访问与修改元素
来源：http://pkw.yj20258888.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mnz.chenjidiqi.icu

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://uzc.sjlbkw.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yhx.yj20258888.top

TS:   arr[0]; arr.at(-1);
来源：http://ttk.zdbjq.cn

Java: list.get(0); list.set(0, 9);
来源：http://lic.ydzc1.top

Go:   arr[0]; arr[0] = 9
来源：http://kpg.yj20258.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ilk.52xcode.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://afh.mhx1999.top

[D06] 数组长度
来源：http://two.iojbl.cn

Py:   len(arr)
来源：http://mvt.yuxming.cn

PHP:  count($arr);
来源：http://edq.birdmap.top

JS:   arr.length
来源：http://tim.yongpay.top

TS:   arr.length
来源：http://cgu.sweek.top

Java: list.size();
来源：http://exd.zdqjudy.top

Go:   len(arr)
来源：http://fnh.sjlbkw.cn

Ruby: arr.length; arr.size
来源：http://zka.sxryk.cn

C#:   list.Count;
来源：http://cwz.jinqigfzy.top

[D07] 切片 / 取子数组
来源：http://jlj.zhijiandao.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://irc.bjfxy.top

PHP:  array_slice($arr, 1, 3);
来源：http://cei.gotoacloud.top

JS:   arr.slice(1, 4);
来源：http://dkb.epnwcf.com

TS:   arr.slice(1, 4);
来源：http://ciu.ybcxt.top

Java: list.subList(1, 4);
来源：http://loz.xingfuxueyuan.xyz

Go:   arr[1:4]
来源：http://eqd.sjlbkw.cn

Ruby: arr[1, 3]
来源：http://ter.cqqwz.cn

C#:   list.GetRange(1, 3);
来源：http://kkq.bbcook.cn

[D08] 合并两个数组
来源：http://oqf.jqgfzy.top

Py:   a + b;  a.extend(b)
来源：http://bzr.yangfankeji.com

PHP:  array_merge($a, $b);
来源：http://dgm.cdnleiting.top

JS:   [...a, ...b];  a.concat(b);
来源：http://rqf.gzhubu.top

TS:   [...a, ...b];
来源：http://ekx.dianchejie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xnz.jianghu66.top

Go:   append(a, b...)
来源：http://htx.zhoulong.xyz

Ruby: a + b;  a.concat(b)
来源：http://lir.zycfv.cn

C#:   a.Concat(b).ToList()
来源：http://wrt.zhijiandao.cn

[D09] 排序（升序）
来源：http://vvh.zhiwuduotai.top

Py:   sorted(arr);  arr.sort()
来源：http://obq.xziqi.cn

PHP:  sort($arr);
来源：http://qfq.ehwqpu.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://skt.gogol.net.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://mks.hnqzz.top

Java: Collections.sort(list);  list.sort(null);
来源：http://gbo.daria6918.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ehc.cdnleiting.top

Ruby: arr.sort
来源：http://iqu.pycfn.com

C#:   list.Sort();
来源：http://ecw.sxryk.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://iod.andypj.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qol.meibo888.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wdf.tanke756.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wrn.hesvh.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pgy.fktsv.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wjb.hnqzz.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://anv.jyoumei.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://llg.jinyuanbaomall.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cru.feifeiyinyue.top

[D11] 反转数组
来源：http://eqc.daxiang520.top

Py:   arr[::-1];  arr.reverse()
来源：http://bye.zhiwuduotai.top

PHP:  array_reverse($arr);
来源：http://ril.shzxlz.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cnd.xinyue.icu

TS:   [...arr].reverse();
来源：http://zhx.hesvh.cn

Java: Collections.reverse(list);
来源：http://biv.jiagoushi.top

Go:   slices.Reverse(arr)
来源：http://jlr.epnwcf.com

Ruby: arr.reverse
来源：http://rgl.vehdjk.com

C#:   list.Reverse();
来源：http://ezx.aibaodan.cn

[D12] 查找元素下标
来源：http://yfk.jianghu66.top

Py:   arr.index(x);  x in arr
来源：http://uca.gogol.net.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kgs.cheryme.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rbd.sxryk.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://shr.ywan-chungtsiang.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://iaf.52xcode.cn

Go:   slices.Index(arr, x)
来源：http://vdb.bjfxy.top

Ruby: arr.index(x)
来源：http://sjd.daxiang520.top

C#:   list.IndexOf(x);
来源：http://iow.jinqigufen.top

[D13] 过滤（保留满足条件的）
来源：http://lpf.gogol.net.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ime.jianghu66.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pcx.gzhubu.top

JS:   arr.filter(x => x > 3)
来源：http://sop.birdmap.top

TS:   arr.filter(x => x > 3)
来源：http://szd.ybcxt.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ghc.shanyushiyangkeji.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gfs.snrcjt.cn

Ruby: arr.select { |x| x > 3 }
来源：http://yci.xingfuxueyuan.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://wax.gogol.net.cn

[D14] 映射转换（每个元素变形）
来源：http://ael.chenlongwang.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mui.ppjwa.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yve.tianlin.xyz

JS:   arr.map(x => x * 2)
来源：http://cot.316326.xyz

TS:   arr.map(x => x * 2)
来源：http://dmg.meibo888.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ypn.nanxinkj.top

Go:   // 手写循环
来源：http://agi.yj20258.top

Ruby: arr.map { |x| x * 2 }
来源：http://lmu.tarul.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://dgq.jqgfzy.top

[D15] 去重
来源：http://sqf.316326.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xmw.yj20258.top

PHP:  array_unique($arr);
来源：http://dfl.meibo888.top

JS:   [...new Set(arr)]
来源：http://gul.xingfuxueyuan.xyz

TS:   [...new Set(arr)]
来源：http://imn.haohaochexian.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yiy.cdnleiting.top

Go:   // 用 map[T]struct{} 手写
来源：http://xja.yj20258.top

Ruby: arr.uniq
来源：http://ufr.ppjwa.cn

C#:   list.Distinct().ToList()
来源：http://kcp.epnwcf.com

[D16] 求和与平均值
来源：http://lws.sysykeji.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://obs.zdbjq.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ozx.daria6918.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://obj.havefunace.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qmn.hammf.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://oun.aibaodan.cn

Go:   // 手写循环累加
来源：http://xwm.mhx1999.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nmm.svipenyu.cn

C#:   list.Sum();  list.Average()
来源：http://poe.andypj.xyz

[D17] 最大值与最小值
来源：http://nir.yanxiufei.cn

Py:   max(arr);  min(arr)
来源：http://aio.yongpay.top

PHP:  max($arr);  min($arr);
来源：http://okc.xziqi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nue.fktsv.cn

TS:   Math.max(...arr);
来源：http://ahw.hnxiangtu.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ovd.zhijiandao.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ckh.hnxiangtu.top

Ruby: arr.max;  arr.min
来源：http://zly.shuidangran.top

C#:   list.Max();  list.Min()
来源：http://shx.hammf.cn

[D18] 扁平化嵌套数组
来源：http://wtx.yongpay.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://txt.meibo888.top

PHP:  array_merge(...$nested);
来源：http://jzy.svipenyu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yyy.yj20258.top

TS:   nested.flat();
来源：http://jxk.xuanzx.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://eqe.zhoulong.xyz

Go:   // 手写双层循环
来源：http://wqd.yj20258888.top

Ruby: nested.flatten
来源：http://fmh.hammf.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://sjd.sweek.top

[D19] 按字段分组
来源：http://rtd.9152youxi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lzo.hnqzz.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://adl.yanxiufei.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ozh.shangyingyoupin.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ysi.ppjwa.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://puv.hywenlv.cn

Go:   // 手写 map[string][]T
来源：http://jlm.hysaishi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://phw.vehdjk.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tcq.cashguo.top

[D20] 统计每个元素出现次数
来源：http://brz.zhiwuduotai.top

Py:   Counter(arr)
来源：http://sri.guowangkeji.top

PHP:  array_count_values($arr);
来源：http://ghj.shanyushiyangtech.top


<!-- 参考信息 -->