代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://oga.xinyue.icu

[C03] 可变参数
来源：http://skh.yonumen.top

Py:   def total(*args): return sum(args)
来源：http://hle.bjfxy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gxo.yfazqb.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wqw.hnxiangtu.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cfx.jyoumei.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blu.mhx1999.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hrr.cashguo.top

Ruby: def total(*nums); nums.sum; end
来源：http://uev.jinyuanbaomall.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://skx.fanxiaobao.xyz

[C04] 命名参数 / 关键字参数
来源：http://aci.ppjwa.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nxc.yj202588.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://stm.xylfe.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rvn.bjfxy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nvs.hysaishi.cn

Java: // 无：用 Builder 模式或 record
来源：http://zek.jqgufenzy.top

Go:   // 无：用配置结构体参数
来源：http://fdn.iojbl.cn

Ruby: f(a: 1, b: 2)
来源：http://njl.tanke756.top

C#:   f(a: 1, b: 2)
来源：http://lfs.feifeiyinyue.top

[C05] 返回多个值
来源：http://cii.jqgufenzy.top

Py:   return a, b
来源：http://zxi.aizwys.cn

PHP:  return [$a, $b];
来源：http://wff.ivvv.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://vud.daria6918.cn

TS:   return { a, b };
来源：http://xhm.hywenlv.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://agk.hnqzz.top

Go:   return a, b
来源：http://jea.xuanzx.com

Ruby: return a, b
来源：http://yvx.sxryk.cn

C#:   return (a, b);              // ValueTuple
来源：http://tkt.quarkkingdee.top

[C06] 匿名函数 / lambda
来源：http://las.fzhhl.top

Py:   square = lambda x: x * x
来源：http://jon.jqgufenzy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://koo.gogol.net.cn

JS:   const square = x => x * x;
来源：http://dul.hnqzz.top

TS:   const square = (x: number): number => x * x;
来源：http://kkt.fzhhl.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hge.yuxming.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ols.zhoulong.xyz

Ruby: square = ->(x) { x * x }
来源：http://jau.snrcjt.cn

C#:   Func<int, int> square = x => x * x;
来源：http://nhc.daria6918.cn

[C07] 把函数作为参数传入
来源：http://zoc.yonumen.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ucu.ydzc1.top

PHP:  array_map("strtoupper", $arr);
来源：http://wpd.aibaodan.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vdu.pycfn.com

TS:   arr.map(String)
来源：http://opz.tanke756.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wgu.dashuyun.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://peq.hywenlv.cn

Ruby: arr.map(&:upcase)
来源：http://trl.chenzaomai.com

C#:   arr.Select(s => s.ToUpper())
来源：http://uev.yfazqb.com

[C08] 闭包
来源：http://krt.shanyushiyangkeji.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nom.nwbrower.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zka.cqqwz.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gco.0kj1m.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vux.tian-w.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ngr.snrcjt.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://owl.zhaomingkeji.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://plt.guannengcc.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fny.zhoulong.xyz

[C09] 递归
来源：http://uit.shzxlz.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zkg.kuanghao11.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ngd.cdnleiting.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pge.mhx1999.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tkf.uphjek.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://quu.daria6918.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://iln.pycfn.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://azc.pycfn.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wgx.sufxvd.cn

[C10] 变量作用域
来源：http://ifc.zhengqikj.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jns.yvedp.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dly.fehbvm.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tcz.ywan-chungtsiang.top

TS:   同 JS
来源：http://bqp.shzxlz.cn

Java: 方法内为块级作用域
来源：http://lri.ctjpmb.com

Go:   花括号块级作用域
来源：http://bmv.c1oappe.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fnd.yvedp.cn

C#:   块级作用域
来源：http://vid.xziqi.cn

[C11] 模块导入与导出
来源：http://ibb.jinqigfzy.top

Py:   from module import func
来源：http://ubl.shzxlz.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://esg.jinghuilouyu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://fvn.xinyue.icu

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fsn.yanxiufei.cn

Java: import java.util.List;
来源：http://eji.hnxiangtu.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kni.sweek.top

Ruby: require "json"; require_relative "./util"
来源：http://ocq.sjlbkw.cn

C#:   using System.Text;
来源：http://pjl.0kj1m.cn

[C12] 立即执行函数 IIFE
来源：http://jwe.ctjpmb.com

Py:   (lambda: print("run"))()
来源：http://rel.zhoulong.xyz

PHP:  (function () { echo "run"; })();
来源：http://txd.yj20258.top

JS:   (() => { console.log("run"); })();
来源：http://ygi.cashguo.top

TS:   (() => { console.log("run"); })();
来源：http://ucc.yangfankeji.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://azw.zhijiandao.cn

Go:   func() { fmt.Println("run") }()
来源：http://ztm.yuanzhike.top

Ruby: -> { puts "run" }.call
来源：http://omn.quarkkingdee.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ppc.sweek.top

[C13] 类型声明 / 类型注解
来源：http://jko.c1oappe.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://uct.shanyushiyangtech.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hgu.shanyushiyangkeji.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zfw.cashguo.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blp.xingfuxueyuan.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://cvn.birdmap.top

Go:   func add(a, b int) int
来源：http://fpm.jinqigufen.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ebu.hesvh.cn

C#:   int Add(int a, int b) => a + b;
来源：http://cjx.c1oappe.top

[C14] 泛型函数
来源：http://kji.hongshengwenyu.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://khx.xinyue.icu

PHP:  // 无泛型
来源：http://bnr.0kj1m.cn

JS:   // 无泛型
来源：http://lou.ivvv.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dpa.shanyushiyangkeji.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cqx.shuidangran.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gii.hysaishi.cn

Ruby: # 无泛型
来源：http://wok.jinyuanbaomall.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bxr.pycfn.com

[C15] 解构 / 展开参数
来源：http://lhz.zhoulong.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lbs.zhixingplan.top

PHP:  [$a, $b] = $pair;
来源：http://cbv.aizwys.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ynq.aibaodan.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://eqf.andypj.xyz

Java: // 无解构
来源：http://uco.vqdsnc.cn

Go:   // 无解构
来源：http://ezb.xingfuxueyuan.xyz

Ruby: a, b = pair
来源：http://qna.redwolf501.top

C#:   var (a, b) = pair;
来源：http://rbf.fengsongda.top

[C16] 函数 / 方法重载
来源：http://ujk.ehwqpu.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fjr.xuetiantiany.cn

PHP:  // 无重载
来源：http://pvc.ppjwa.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://bfh.bjfxy.top

TS:   // 用联合类型或重载签名声明
来源：http://fnr.shanyushiyangtech.top

Java: void f(int a) {}  void f(String a) {}
来源：http://lbk.0kj1m.cn

Go:   // 无重载：用不同函数名
来源：http://kyb.fengsongda.top

Ruby: # 无重载：靠动态参数
来源：http://jml.yonumen.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://bvs.gotoacloud.top

================================================================================
来源：http://nuc.dianchejie.cn

D. 数组 / 列表 / 集合
来源：http://zvz.hesvh.cn

================================================================================
来源：http://wpb.gotoacloud.top

[D01] 创建数组 / 列表
来源：http://qnp.svipenyu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://rvh.cucudq.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pcy.yj202588.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zwz.ctjpmb.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://mms.xylfe.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xwv.gogol.net.cn

Go:   arr := []int{1, 2, 3}
来源：http://nsc.bjfxy.top

Ruby: arr = [1, 2, 3]
来源：http://zzf.chenzaomai.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wsu.yj20258.top

[D02] 追加元素到末尾
来源：http://zpb.jiagoushi.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tnk.ydzc1.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wup.wangshuangyany.cn

JS:   arr.push(4);
来源：http://ofr.hesvh.cn

TS:   arr.push(4);
来源：http://xym.yj202588.top

Java: list.add(4);
来源：http://xsb.fktsv.cn

Go:   arr = append(arr, 4)
来源：http://plv.jlsjyb.cn

Ruby: arr << 4; arr.push(5)
来源：http://amg.vqdsnc.cn

C#:   list.Add(4);
来源：http://lnh.guannengcc.top

[D03] 在指定位置插入元素
来源：http://tvr.epnwcf.com

Py:   arr.insert(0, 0)
来源：http://dot.fengsongda.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fko.shangyingyoupin.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hnt.nwbrower.top

TS:   arr.splice(0, 0, 0);
来源：http://sfl.fktsv.cn

Java: list.add(0, 0);
来源：http://epq.52xcode.cn

Go:   arr = append([]int{0}, arr...)
来源：http://axn.sjlbkw.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gbg.yuanzhike.top

C#:   list.Insert(0, 0);
来源：http://uua.chenlongwang.top

[D04] 删除元素
来源：http://yki.snrcjt.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gkr.shanyushiyangkeji.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kwe.jiagoushi.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ecn.ivvv.top

TS:   arr.splice(0, 1);
来源：http://tko.iojbl.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qhs.hywenlv.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://noh.cheryme.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xhg.quarkkingdee.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ixf.fengsongda.top

[D05] 访问与修改元素
来源：http://drb.jinqigufen.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sji.yonumen.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sxk.fzhhl.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://quw.pengpengdd.cyou

TS:   arr[0]; arr.at(-1);
来源：http://dbo.shangyingyoupin.top

Java: list.get(0); list.set(0, 9);
来源：http://ndu.ybcxt.top

Go:   arr[0]; arr[0] = 9
来源：http://sfw.smart0.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dsq.ctjpmb.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hao.daria6918.cn

[D06] 数组长度
来源：http://yit.ybcxt.top

Py:   len(arr)
来源：http://lys.zhijiandao.cn

PHP:  count($arr);
来源：http://iyw.cheryme.top

JS:   arr.length
来源：http://xfp.tianlin.xyz

TS:   arr.length
来源：http://hip.jqgfzy.top

Java: list.size();
来源：http://omo.xingfuxueyuan.xyz

Go:   len(arr)
来源：http://shh.meibo888.top

Ruby: arr.length; arr.size
来源：http://zgm.mhx1999.top

C#:   list.Count;
来源：http://adt.jlsjyb.cn

[D07] 切片 / 取子数组
来源：http://jfo.yj202588.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fmk.tanke756.top

PHP:  array_slice($arr, 1, 3);
来源：http://oqk.zdbjq.cn

JS:   arr.slice(1, 4);
来源：http://zmv.daxiang520.top

TS:   arr.slice(1, 4);
来源：http://jpn.aizwys.cn

Java: list.subList(1, 4);
来源：http://ihp.uphjek.com

Go:   arr[1:4]
来源：http://tgx.tanke756.top

Ruby: arr[1, 3]
来源：http://bjr.jlsjyb.cn

C#:   list.GetRange(1, 3);
来源：http://voq.snrcjt.cn

[D08] 合并两个数组
来源：http://nas.cheryme.top

Py:   a + b;  a.extend(b)
来源：http://off.zhengqikj.top

PHP:  array_merge($a, $b);
来源：http://dup.cashguo.top

JS:   [...a, ...b];  a.concat(b);
来源：http://emc.jyoumei.cn

TS:   [...a, ...b];
来源：http://gju.fengsongda.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://guc.hysaishi.cn

Go:   append(a, b...)
来源：http://sfk.cashguo.top

Ruby: a + b;  a.concat(b)
来源：http://nyx.xuanzx.com

C#:   a.Concat(b).ToList()
来源：http://nqy.yfazqb.com

[D09] 排序（升序）
来源：http://nww.cdnleiting.top

Py:   sorted(arr);  arr.sort()
来源：http://wdb.sxryk.cn

PHP:  sort($arr);
来源：http://daf.ydzc1.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xfc.zhiwuduotai.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://svu.bjfxy.top

Java: Collections.sort(list);  list.sort(null);
来源：http://dzk.iojbl.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xls.zycfv.cn

Ruby: arr.sort
来源：http://uxt.jyoumei.cn

C#:   list.Sort();
来源：http://mdh.cucudq.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://cie.jlsjyb.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yfk.smart0.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qfo.wangshuangyany.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pjb.sufxvd.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tpm.jiagoushi.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dfu.shanyushiyangtech.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zqq.yj202588.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hps.zycfv.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://svp.jiagoushi.top

[D11] 反转数组
来源：http://jah.snrcjt.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qau.vqdsnc.cn

PHP:  array_reverse($arr);
来源：http://vdn.shzxlz.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vzg.tarul.cn

TS:   [...arr].reverse();
来源：http://sen.hnxiangtu.top

Java: Collections.reverse(list);
来源：http://ydc.yuxming.cn

Go:   slices.Reverse(arr)
来源：http://bdp.xziqi.cn

Ruby: arr.reverse
来源：http://jta.nanxinkj.top

C#:   list.Reverse();
来源：http://eoj.dianchejie.cn

[D12] 查找元素下标
来源：http://okw.tarul.cn

Py:   arr.index(x);  x in arr
来源：http://gps.shangyingyoupin.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ztc.vqdsnc.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rfc.feifeiyinyue.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qtr.yangfankeji.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lff.aizwys.cn

Go:   slices.Index(arr, x)
来源：http://krf.gotoacloud.top

Ruby: arr.index(x)
来源：http://ujt.chenjidiqi.icu

C#:   list.IndexOf(x);
来源：http://qtq.hnxiangtu.top

[D13] 过滤（保留满足条件的）
来源：http://raj.hysaishi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zeh.shangyingyoupin.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://owp.mhx1999.top

JS:   arr.filter(x => x > 3)
来源：http://znk.jinqigufen.top

TS:   arr.filter(x => x > 3)
来源：http://epa.hnxiangtu.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zlu.redwolf501.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mwh.xuanzx.com

Ruby: arr.select { |x| x > 3 }
来源：http://hrh.wangshuangyany.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://hqr.bjfxy.top

[D14] 映射转换（每个元素变形）
来源：http://vws.cqqwz.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zmd.daria6918.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zzr.bjfxy.top

JS:   arr.map(x => x * 2)
来源：http://app.meibo888.top

TS:   arr.map(x => x * 2)
来源：http://uza.jqgufenzy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://dfl.ydjk.org.cn

Go:   // 手写循环
来源：http://lti.c1oappe.top

Ruby: arr.map { |x| x * 2 }
来源：http://fze.iojbl.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://vzm.daria6918.cn

[D15] 去重
来源：http://fmg.daxiang520.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rrx.uphjek.com

PHP:  array_unique($arr);
来源：http://vdi.yj20258.top

JS:   [...new Set(arr)]
来源：http://pia.zhiwuduotai.top

TS:   [...new Set(arr)]
来源：http://zvq.gogol.net.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://obx.quarkkingdee.top

Go:   // 用 map[T]struct{} 手写
来源：http://eqf.uphjek.com

Ruby: arr.uniq
来源：http://ckr.tianlin.xyz

C#:   list.Distinct().ToList()
来源：http://qdq.jqgfzy.top

[D16] 求和与平均值
来源：http://dxd.yuanzhike.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tbk.cucudq.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qnz.yongpay.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://too.epnwcf.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rvy.vehdjk.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bld.yvedp.cn

Go:   // 手写循环累加
来源：http://ffl.316326.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fdj.chenjidiqi.icu

C#:   list.Sum();  list.Average()
来源：http://lxg.jinqigufen.top

[D17] 最大值与最小值
来源：http://uhy.yuxming.cn

Py:   max(arr);  min(arr)
来源：http://iex.jinyuanbaomall.cn

PHP:  max($arr);  min($arr);
来源：http://vqt.yonumen.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lqs.cqqwz.cn

TS:   Math.max(...arr);
来源：http://xbw.aibaodan.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://abj.yj202588.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wzg.bbcook.cn

Ruby: arr.max;  arr.min
来源：http://xio.aizwys.cn

C#:   list.Max();  list.Min()
来源：http://yqc.dashuyun.cn

[D18] 扁平化嵌套数组
来源：http://pix.9152youxi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vwi.xylfe.cn

PHP:  array_merge(...$nested);
来源：http://ipv.shuidangran.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mje.0kj1m.cn

TS:   nested.flat();
来源：http://dlj.pengpengdd.cyou

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tyq.sufxvd.cn

Go:   // 手写双层循环
来源：http://odm.smart0.xyz

Ruby: nested.flatten
来源：http://cly.zhijiandao.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://tva.hcnkem.com

[D19] 按字段分组
来源：http://osm.yonumen.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dqd.tarul.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mxw.gaohongyu789.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://shx.zhongyouzk.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://aod.fanxiaobao.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mly.jqgufenzy.top

Go:   // 手写 map[string][]T
来源：http://xsy.ywan-chungtsiang.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://mvi.zdqjudy.top


<!-- 参考信息 -->