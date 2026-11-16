代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://ibg.316326.xyz

[C03] 可变参数
来源：http://iyo.jinyuanbaomall.cn

Py:   def total(*args): return sum(args)
来源：http://vvy.shanyushiyangtech.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vcn.svipenyu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wyz.daxiang520.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://tog.tian-w.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://juw.sxryk.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mwr.cqqwz.cn

Ruby: def total(*nums); nums.sum; end
来源：http://lyv.ctjpmb.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bnk.feifeiyinyue.top

[C04] 命名参数 / 关键字参数
来源：http://hld.fehbvm.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qbs.cucudq.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xnv.fanxiaobao.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qir.chenzaomai.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kpg.nanxinkj.top

Java: // 无：用 Builder 模式或 record
来源：http://exo.aibaodan.cn

Go:   // 无：用配置结构体参数
来源：http://jdg.chenzaomai.com

Ruby: f(a: 1, b: 2)
来源：http://jyb.uphjek.com

C#:   f(a: 1, b: 2)
来源：http://wun.xuanzx.com

[C05] 返回多个值
来源：http://joc.gogol.net.cn

Py:   return a, b
来源：http://mnq.hnqzz.top

PHP:  return [$a, $b];
来源：http://mvs.daria6918.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://aaw.hnqzz.top

TS:   return { a, b };
来源：http://sgg.jinqigufen.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bpp.zhijiandao.cn

Go:   return a, b
来源：http://tcj.xinyue.icu

Ruby: return a, b
来源：http://qwn.zhengqikj.top

C#:   return (a, b);              // ValueTuple
来源：http://isc.nanxinkj.top

[C06] 匿名函数 / lambda
来源：http://vsh.yj20258.top

Py:   square = lambda x: x * x
来源：http://apj.zdbjq.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://rtd.xziqi.cn

JS:   const square = x => x * x;
来源：http://zkq.hesvh.cn

TS:   const square = (x: number): number => x * x;
来源：http://dya.redwolf501.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lpx.fanxiaobao.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://xyz.jinqigufen.top

Ruby: square = ->(x) { x * x }
来源：http://lpv.daxiang520.top

C#:   Func<int, int> square = x => x * x;
来源：http://hpx.hnxiangtu.top

[C07] 把函数作为参数传入
来源：http://oyz.sysykeji.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ipd.yonumen.top

PHP:  array_map("strtoupper", $arr);
来源：http://fga.smart0.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://url.yangfankeji.com

TS:   arr.map(String)
来源：http://mfo.zdqjudy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nzd.xylfe.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://itk.hongshengwenyu.top

Ruby: arr.map(&:upcase)
来源：http://tvg.0kj1m.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://qfk.bbcook.cn

[C08] 闭包
来源：http://ehd.wangshuangyany.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mdl.ybcxt.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://opq.0kj1m.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pgh.316326.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dqh.hysaishi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gpz.gotoacloud.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ylt.cucudq.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lgd.tianlin.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lux.gotoacloud.top

[C09] 递归
来源：http://puf.gaohongyu789.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rtm.ybcxt.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://grb.fanxiaobao.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nsg.zhengqikj.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lbp.0kj1m.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://orp.zdqjudy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nlz.nanxuanxn.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://biq.fktsv.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://acu.9152youxi.cn

[C10] 变量作用域
来源：http://qtj.zhongyouzk.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vmp.tanke756.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://snn.dianchejie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dwz.cashguo.top

TS:   同 JS
来源：http://fdh.cdnleiting.top

Java: 方法内为块级作用域
来源：http://zhc.hywenlv.cn

Go:   花括号块级作用域
来源：http://hsh.ppjwa.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nqs.zhaomingkeji.xyz

C#:   块级作用域
来源：http://ksk.haohaochexian.top

[C11] 模块导入与导出
来源：http://kvp.hammf.cn

Py:   from module import func
来源：http://bwn.yueranfly.top

PHP:  require "file.php";  或 use App\Service;
来源：http://wci.tanke756.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://vwy.sufxvd.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://szd.chenjidiqi.icu

Java: import java.util.List;
来源：http://zzr.dianchejie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jnw.kuanghao11.cn

Ruby: require "json"; require_relative "./util"
来源：http://dtf.kuanghao11.cn

C#:   using System.Text;
来源：http://kru.aizwys.cn

[C12] 立即执行函数 IIFE
来源：http://zfw.kuanghao11.cn

Py:   (lambda: print("run"))()
来源：http://vtk.xinyue.icu

PHP:  (function () { echo "run"; })();
来源：http://ohm.zhijiandao.cn

JS:   (() => { console.log("run"); })();
来源：http://pps.jianghu66.top

TS:   (() => { console.log("run"); })();
来源：http://zux.ywan-chungtsiang.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://oiy.fktsv.cn

Go:   func() { fmt.Println("run") }()
来源：http://njd.hammf.cn

Ruby: -> { puts "run" }.call
来源：http://ztr.xziqi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://lww.vqdsnc.cn

[C13] 类型声明 / 类型注解
来源：http://chn.xuanzx.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jdg.hesvh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rub.jyoumei.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://huz.tian-w.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://trm.xylfe.cn

Java: int add(int a, int b) { return a + b; }
来源：http://yux.jinghuilouyu.cn

Go:   func add(a, b int) int
来源：http://cvt.zhiwuduotai.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://aki.hywenlv.cn

C#:   int Add(int a, int b) => a + b;
来源：http://dts.fktsv.cn

[C14] 泛型函数
来源：http://oxa.xuanzx.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://otr.xuanzx.com

PHP:  // 无泛型
来源：http://zrx.kuanghao11.cn

JS:   // 无泛型
来源：http://ojc.xuetiantiany.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rhq.pengpengdd.cyou

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qup.chenjidiqi.icu

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qvn.jlsjyb.cn

Ruby: # 无泛型
来源：http://zil.quarkkingdee.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dcu.quarkkingdee.top

[C15] 解构 / 展开参数
来源：http://qbq.yj20258.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://orb.9152youxi.cn

PHP:  [$a, $b] = $pair;
来源：http://ucx.yj202588.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fpu.zhixingplan.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zji.shuidangran.top

Java: // 无解构
来源：http://rzy.c1oappe.top

Go:   // 无解构
来源：http://cfg.xziqi.cn

Ruby: a, b = pair
来源：http://kxu.hysaishi.cn

C#:   var (a, b) = pair;
来源：http://vfh.bbcook.cn

[C16] 函数 / 方法重载
来源：http://reh.xylfe.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://spz.hongshengwenyu.top

PHP:  // 无重载
来源：http://jwc.chenjidiqi.icu

JS:   // 无重载：靠 arguments.length 分支
来源：http://cgp.cashguo.top

TS:   // 用联合类型或重载签名声明
来源：http://lrq.vqdsnc.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ilt.shanyushiyangkeji.top

Go:   // 无重载：用不同函数名
来源：http://adx.mhx1999.top

Ruby: # 无重载：靠动态参数
来源：http://fyn.redwolf501.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://giw.nanxuanxn.top

================================================================================
来源：http://irw.guannengcc.top

D. 数组 / 列表 / 集合
来源：http://bvk.jinqigfzy.top

================================================================================
来源：http://lbi.0kj1m.cn

[D01] 创建数组 / 列表
来源：http://dor.guowangkeji.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://avz.zdbjq.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xsy.feifeiyinyue.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ezw.cucudq.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://fzj.yvedp.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mpe.gzhubu.top

Go:   arr := []int{1, 2, 3}
来源：http://moi.fanxiaobao.xyz

Ruby: arr = [1, 2, 3]
来源：http://lce.xuetiantiany.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wys.jlsjyb.cn

[D02] 追加元素到末尾
来源：http://lww.hfpthk.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ggk.hnxiangtu.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rre.fehbvm.com

JS:   arr.push(4);
来源：http://lal.birdmap.top

TS:   arr.push(4);
来源：http://yfp.xuanzx.com

Java: list.add(4);
来源：http://gwl.hfpthk.cn

Go:   arr = append(arr, 4)
来源：http://tvp.zdqjudy.top

Ruby: arr << 4; arr.push(5)
来源：http://flm.pengpengdd.cyou

C#:   list.Add(4);
来源：http://gxh.jinqigufen.top

[D03] 在指定位置插入元素
来源：http://lnl.andypj.xyz

Py:   arr.insert(0, 0)
来源：http://mir.cashguo.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cmy.ydzc1.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bbf.zhiwuduotai.top

TS:   arr.splice(0, 0, 0);
来源：http://hfj.zhongyouzk.top

Java: list.add(0, 0);
来源：http://rvl.ivvv.top

Go:   arr = append([]int{0}, arr...)
来源：http://sfh.fengsongda.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jkc.yangfankeji.com

C#:   list.Insert(0, 0);
来源：http://jsv.sjlbkw.cn

[D04] 删除元素
来源：http://mzw.ehwqpu.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hqe.daxiang520.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lng.ctjpmb.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://guo.chenlongwang.top

TS:   arr.splice(0, 1);
来源：http://jgl.meibo888.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jdi.sjlbkw.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ien.gogol.net.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wtr.meibo888.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vfb.redwolf501.top

[D05] 访问与修改元素
来源：http://zkd.birdmap.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gtg.vqdsnc.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dyg.tanke756.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bbm.dashuyun.cn

TS:   arr[0]; arr.at(-1);
来源：http://hwt.zhijiandao.cn

Java: list.get(0); list.set(0, 9);
来源：http://syc.xylfe.cn

Go:   arr[0]; arr[0] = 9
来源：http://mru.sjlbkw.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sph.uphjek.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dxg.yueranfly.top

[D06] 数组长度
来源：http://dvb.sxryk.cn

Py:   len(arr)
来源：http://fvx.zhengqikj.top

PHP:  count($arr);
来源：http://awi.sysykeji.top

JS:   arr.length
来源：http://bum.bbcook.cn

TS:   arr.length
来源：http://tzy.yfazqb.com

Java: list.size();
来源：http://abk.zhengqikj.top

Go:   len(arr)
来源：http://hef.cheryme.top

Ruby: arr.length; arr.size
来源：http://xoc.meibo888.top

C#:   list.Count;
来源：http://aqv.xuetiantiany.cn

[D07] 切片 / 取子数组
来源：http://ngm.hnxiangtu.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kfl.zhijiandao.cn

PHP:  array_slice($arr, 1, 3);
来源：http://kkv.c1oappe.top

JS:   arr.slice(1, 4);
来源：http://xls.sweek.top

TS:   arr.slice(1, 4);
来源：http://ynm.yuxming.cn

Java: list.subList(1, 4);
来源：http://xbf.kuanghao11.cn

Go:   arr[1:4]
来源：http://ckb.snrcjt.cn

Ruby: arr[1, 3]
来源：http://oqu.jyoumei.cn

C#:   list.GetRange(1, 3);
来源：http://dlz.yfazqb.com

[D08] 合并两个数组
来源：http://vjm.cucudq.cn

Py:   a + b;  a.extend(b)
来源：http://qrv.xuanzx.com

PHP:  array_merge($a, $b);
来源：http://hgj.tarul.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ebi.yanxiufei.cn

TS:   [...a, ...b];
来源：http://oqk.xuanzx.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nra.shzxlz.cn

Go:   append(a, b...)
来源：http://css.tian-w.cn

Ruby: a + b;  a.concat(b)
来源：http://dnp.xuetiantiany.cn

C#:   a.Concat(b).ToList()
来源：http://opq.shzxlz.cn

[D09] 排序（升序）
来源：http://vrj.ybcxt.top

Py:   sorted(arr);  arr.sort()
来源：http://sdb.hnxiangtu.top

PHP:  sort($arr);
来源：http://inc.yj202588.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://deq.uphjek.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://amj.zhaomingkeji.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://dpz.sweek.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wld.tarul.cn

Ruby: arr.sort
来源：http://mnq.guannengcc.top

C#:   list.Sort();
来源：http://xwf.yj20258888.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://pbq.hammf.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://oss.vqdsnc.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cxd.cucudq.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gqp.dianchejie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://iqf.zhengqikj.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jxv.vehdjk.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hii.zhiwuduotai.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lvo.birdmap.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kka.svipenyu.cn

[D11] 反转数组
来源：http://lsg.andypj.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://isr.andypj.xyz

PHP:  array_reverse($arr);
来源：http://brg.feifeiyinyue.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://szn.smart0.xyz

TS:   [...arr].reverse();
来源：http://fuw.shangyingyoupin.top

Java: Collections.reverse(list);
来源：http://rjo.vqdsnc.cn

Go:   slices.Reverse(arr)
来源：http://wbi.nanxuanxn.top

Ruby: arr.reverse
来源：http://jnr.aizwys.cn

C#:   list.Reverse();
来源：http://xvh.ybcxt.top

[D12] 查找元素下标
来源：http://nuu.daxiang520.top

Py:   arr.index(x);  x in arr
来源：http://vej.hesvh.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hle.gogol.net.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://swc.bjfxy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fof.daria6918.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nnb.zhongyouzk.top

Go:   slices.Index(arr, x)
来源：http://ckb.tanke756.top

Ruby: arr.index(x)
来源：http://tts.9152youxi.cn

C#:   list.IndexOf(x);
来源：http://rtp.shangyingyoupin.top

[D13] 过滤（保留满足条件的）
来源：http://dzm.chenlongwang.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lpq.sjlbkw.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://orx.jinqigufen.top

JS:   arr.filter(x => x > 3)
来源：http://vdk.aibaodan.cn

TS:   arr.filter(x => x > 3)
来源：http://hwg.shanyushiyangkeji.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jtq.jinghuilouyu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://iew.aibaodan.cn

Ruby: arr.select { |x| x > 3 }
来源：http://bas.pycfn.com

C#:   list.Where(x => x > 3).ToList()
来源：http://oov.yanxiufei.cn

[D14] 映射转换（每个元素变形）
来源：http://den.xingfuxueyuan.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xta.ppjwa.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rhp.yj202588.top

JS:   arr.map(x => x * 2)
来源：http://cqf.0kj1m.cn

TS:   arr.map(x => x * 2)
来源：http://oaw.sjlbkw.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ekt.gogol.net.cn

Go:   // 手写循环
来源：http://cio.ehwqpu.com

Ruby: arr.map { |x| x * 2 }
来源：http://fzg.xinyue.icu

C#:   list.Select(x => x * 2).ToList()
来源：http://nsk.jinqigufen.top

[D15] 去重
来源：http://pmq.jlsjyb.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vcm.hfpthk.cn

PHP:  array_unique($arr);
来源：http://kxc.yangfankeji.com

JS:   [...new Set(arr)]
来源：http://jry.sxryk.cn

TS:   [...new Set(arr)]
来源：http://evz.bjfxy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mnj.wangdashe.top

Go:   // 用 map[T]struct{} 手写
来源：http://iyn.dashuyun.cn

Ruby: arr.uniq
来源：http://eqm.hywenlv.cn

C#:   list.Distinct().ToList()
来源：http://pbi.jqgufenzy.top

[D16] 求和与平均值
来源：http://yip.yj202588.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://enp.svipenyu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cxg.yj20258.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xxh.ehwqpu.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hcd.dashuyun.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yto.jinghuilouyu.cn

Go:   // 手写循环累加
来源：http://npu.nanxinkj.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xqy.chenlongwang.top

C#:   list.Sum();  list.Average()
来源：http://mea.ydjk.org.cn

[D17] 最大值与最小值
来源：http://mhx.ehwqpu.com

Py:   max(arr);  min(arr)
来源：http://lno.tanke756.top

PHP:  max($arr);  min($arr);
来源：http://poq.xingfuxueyuan.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xap.zhiwuduotai.top

TS:   Math.max(...arr);
来源：http://jmj.guannengcc.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ukh.uphjek.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mgo.jinghuilouyu.cn

Ruby: arr.max;  arr.min
来源：http://ywv.cdnleiting.top

C#:   list.Max();  list.Min()
来源：http://bpt.ivvv.top

[D18] 扁平化嵌套数组
来源：http://gqp.sweek.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ljb.yanxiufei.cn

PHP:  array_merge(...$nested);
来源：http://bnk.52xcode.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yvi.svipenyu.cn

TS:   nested.flat();
来源：http://wvy.hfpthk.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mbs.zhoulong.xyz

Go:   // 手写双层循环
来源：http://wqe.zycfv.cn

Ruby: nested.flatten
来源：http://ana.ywan-chungtsiang.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://clr.vehdjk.com

[D19] 按字段分组
来源：http://grn.gzhubu.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xwu.gotoacloud.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://oir.gzhubu.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rbw.nanxinkj.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://thw.xuetiantiany.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://txz.nanxuanxn.top

Go:   // 手写 map[string][]T
来源：http://qhm.zhaomingkeji.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://tyl.zhixingplan.top


<!-- 参考信息 -->