代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://bnz.daria6918.cn

[C03] 可变参数
来源：http://nkm.hysaishi.cn

Py:   def total(*args): return sum(args)
来源：http://fgl.shzxlz.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dnc.yueranfly.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jzq.tarul.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wrf.zhengqikj.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gly.shanyushiyangkeji.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://twf.quarkkingdee.top

Ruby: def total(*nums); nums.sum; end
来源：http://nut.sjlbkw.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://sio.yj20258.top

[C04] 命名参数 / 关键字参数
来源：http://otl.xuanzx.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wmx.andypj.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lrp.iojbl.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yuf.sweek.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gbj.jinghuilouyu.cn

Java: // 无：用 Builder 模式或 record
来源：http://wdf.hywenlv.cn

Go:   // 无：用配置结构体参数
来源：http://ban.hywenlv.cn

Ruby: f(a: 1, b: 2)
来源：http://npu.yongpay.top

C#:   f(a: 1, b: 2)
来源：http://vnx.pycfn.com

[C05] 返回多个值
来源：http://inj.yongpay.top

Py:   return a, b
来源：http://mhn.xylfe.cn

PHP:  return [$a, $b];
来源：http://tjy.chenlongwang.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://znv.smart0.xyz

TS:   return { a, b };
来源：http://wai.zhongyouzk.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://imz.chenjidiqi.icu

Go:   return a, b
来源：http://ilp.jianghu66.top

Ruby: return a, b
来源：http://xyp.haohaochexian.top

C#:   return (a, b);              // ValueTuple
来源：http://scq.xylfe.cn

[C06] 匿名函数 / lambda
来源：http://xrd.hywenlv.cn

Py:   square = lambda x: x * x
来源：http://ftn.ydjk.org.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://utc.birdmap.top

JS:   const square = x => x * x;
来源：http://pts.yj20258.top

TS:   const square = (x: number): number => x * x;
来源：http://dlp.birdmap.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nqv.yj20258.top

Go:   sq := func(x int) int { return x * x }
来源：http://uea.hysaishi.cn

Ruby: square = ->(x) { x * x }
来源：http://gvn.vehdjk.com

C#:   Func<int, int> square = x => x * x;
来源：http://jip.daria6918.cn

[C07] 把函数作为参数传入
来源：http://ecq.hysaishi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wnk.gotoacloud.top

PHP:  array_map("strtoupper", $arr);
来源：http://xci.yuanzhike.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ogd.xylfe.cn

TS:   arr.map(String)
来源：http://hxo.zdqjudy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wqm.xuetiantiany.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xpe.zhoulong.xyz

Ruby: arr.map(&:upcase)
来源：http://rlt.vehdjk.com

C#:   arr.Select(s => s.ToUpper())
来源：http://ggt.nanxuanxn.top

[C08] 闭包
来源：http://qjv.mhx1999.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ozf.gogol.net.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uhg.birdmap.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cra.gzhubu.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://llw.yj20258888.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zgh.sweek.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vga.chenjidiqi.icu

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vzx.hesvh.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ixm.hywenlv.cn

[C09] 递归
来源：http://rcj.316326.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gbd.zhijiandao.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://snw.fengsongda.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cwe.chenjidiqi.icu

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dlt.hnxiangtu.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lkh.xuetiantiany.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vnf.hnxiangtu.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dtp.jianghu66.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jbe.smart0.xyz

[C10] 变量作用域
来源：http://sqs.ctjpmb.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vbj.meibo888.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ifn.zdqjudy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xbo.yangfankeji.com

TS:   同 JS
来源：http://miw.hongshengwenyu.top

Java: 方法内为块级作用域
来源：http://xtc.jqgufenzy.top

Go:   花括号块级作用域
来源：http://jcd.ppjwa.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pmm.jinqigufen.top

C#:   块级作用域
来源：http://fsw.jinyuanbaomall.cn

[C11] 模块导入与导出
来源：http://tqh.uphjek.com

Py:   from module import func
来源：http://kbw.ydjk.org.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://roq.bbcook.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ghc.fengsongda.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dgm.ydzc1.top

Java: import java.util.List;
来源：http://rdz.guowangkeji.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jpd.c1oappe.top

Ruby: require "json"; require_relative "./util"
来源：http://sbn.cashguo.top

C#:   using System.Text;
来源：http://lcr.shuidangran.top

[C12] 立即执行函数 IIFE
来源：http://xod.zhongyouzk.top

Py:   (lambda: print("run"))()
来源：http://mxy.quarkkingdee.top

PHP:  (function () { echo "run"; })();
来源：http://aog.jinqigufen.top

JS:   (() => { console.log("run"); })();
来源：http://aie.meibo888.top

TS:   (() => { console.log("run"); })();
来源：http://kma.hfpthk.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://osd.hcnkem.com

Go:   func() { fmt.Println("run") }()
来源：http://umd.sufxvd.cn

Ruby: -> { puts "run" }.call
来源：http://cay.guannengcc.top

C#:   // 无 IIFE：用静态构造函数
来源：http://cey.jlsjyb.cn

[C13] 类型声明 / 类型注解
来源：http://oxa.ybcxt.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://smd.jinyuanbaomall.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rua.uphjek.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xyo.zhaomingkeji.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hgy.yueranfly.top

Java: int add(int a, int b) { return a + b; }
来源：http://rgo.chenlongwang.top

Go:   func add(a, b int) int
来源：http://wbi.tian-w.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fzg.vehdjk.com

C#:   int Add(int a, int b) => a + b;
来源：http://flq.xingfuxueyuan.xyz

[C14] 泛型函数
来源：http://heq.chenzaomai.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zfx.shzxlz.cn

PHP:  // 无泛型
来源：http://wac.yangfankeji.com

JS:   // 无泛型
来源：http://vbr.zdqjudy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dkm.sjlbkw.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://iny.hysaishi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zbj.vehdjk.com

Ruby: # 无泛型
来源：http://kri.sjlbkw.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hqy.feifeiyinyue.top

[C15] 解构 / 展开参数
来源：http://ovw.jinqigfzy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cjf.gaohongyu789.top

PHP:  [$a, $b] = $pair;
来源：http://mjz.xziqi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://odo.zhengqikj.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sbl.dianchejie.cn

Java: // 无解构
来源：http://ixq.iojbl.cn

Go:   // 无解构
来源：http://jku.yj202588.top

Ruby: a, b = pair
来源：http://gcw.316326.xyz

C#:   var (a, b) = pair;
来源：http://ksh.sysykeji.top

[C16] 函数 / 方法重载
来源：http://soh.sjlbkw.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hjb.svipenyu.cn

PHP:  // 无重载
来源：http://vgd.jyoumei.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ukz.dashuyun.cn

TS:   // 用联合类型或重载签名声明
来源：http://igv.sjlbkw.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://onz.52xcode.cn

Go:   // 无重载：用不同函数名
来源：http://npj.ehwqpu.com

Ruby: # 无重载：靠动态参数
来源：http://tjs.cdnleiting.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://moa.haohaochexian.top

================================================================================
来源：http://odo.yfazqb.com

D. 数组 / 列表 / 集合
来源：http://nmb.ctjpmb.com

================================================================================
来源：http://svl.xuanzx.com

[D01] 创建数组 / 列表
来源：http://qpa.wangdashe.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://iyw.yangfankeji.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sch.kuanghao11.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wkx.yonumen.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://lng.9152youxi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mrh.daxiang520.top

Go:   arr := []int{1, 2, 3}
来源：http://qwz.zdqjudy.top

Ruby: arr = [1, 2, 3]
来源：http://cjz.hysaishi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://igs.birdmap.top

[D02] 追加元素到末尾
来源：http://jkp.mhx1999.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ihw.jlsjyb.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vdb.yuxming.cn

JS:   arr.push(4);
来源：http://uim.0kj1m.cn

TS:   arr.push(4);
来源：http://jfz.xziqi.cn

Java: list.add(4);
来源：http://vxa.jlsjyb.cn

Go:   arr = append(arr, 4)
来源：http://kjv.fktsv.cn

Ruby: arr << 4; arr.push(5)
来源：http://hml.pengpengdd.cyou

C#:   list.Add(4);
来源：http://koo.mhx1999.top

[D03] 在指定位置插入元素
来源：http://pfz.jinyuanbaomall.cn

Py:   arr.insert(0, 0)
来源：http://lyq.tianlin.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kdw.guannengcc.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zzh.hesvh.cn

TS:   arr.splice(0, 0, 0);
来源：http://kfr.chenjidiqi.icu

Java: list.add(0, 0);
来源：http://qwa.yueranfly.top

Go:   arr = append([]int{0}, arr...)
来源：http://ywb.andypj.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://tog.nwbrower.top

C#:   list.Insert(0, 0);
来源：http://mur.jqgfzy.top

[D04] 删除元素
来源：http://wah.hnxiangtu.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mwn.ybcxt.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pft.tian-w.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ycl.jlsjyb.cn

TS:   arr.splice(0, 1);
来源：http://nyq.iojbl.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jls.andypj.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sfp.gzhubu.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qzf.52xcode.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yia.yvedp.cn

[D05] 访问与修改元素
来源：http://gki.sysykeji.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://igb.zhongyouzk.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tsl.quarkkingdee.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://aoa.shangyingyoupin.top

TS:   arr[0]; arr.at(-1);
来源：http://sqs.tianlin.xyz

Java: list.get(0); list.set(0, 9);
来源：http://khr.ywan-chungtsiang.top

Go:   arr[0]; arr[0] = 9
来源：http://nyn.svipenyu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tfs.yvedp.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xyp.andypj.xyz

[D06] 数组长度
来源：http://meo.ppjwa.cn

Py:   len(arr)
来源：http://twz.fktsv.cn

PHP:  count($arr);
来源：http://msj.sufxvd.cn

JS:   arr.length
来源：http://ftl.ppjwa.cn

TS:   arr.length
来源：http://sqt.quarkkingdee.top

Java: list.size();
来源：http://grr.jqgufenzy.top

Go:   len(arr)
来源：http://xfp.chenlongwang.top

Ruby: arr.length; arr.size
来源：http://qcq.chenlongwang.top

C#:   list.Count;
来源：http://ldx.hnqzz.top

[D07] 切片 / 取子数组
来源：http://aal.yj202588.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://uqa.hongshengwenyu.top

PHP:  array_slice($arr, 1, 3);
来源：http://wnl.gotoacloud.top

JS:   arr.slice(1, 4);
来源：http://wei.gogol.net.cn

TS:   arr.slice(1, 4);
来源：http://qqx.shzxlz.cn

Java: list.subList(1, 4);
来源：http://wrk.hammf.cn

Go:   arr[1:4]
来源：http://xsk.feifeiyinyue.top

Ruby: arr[1, 3]
来源：http://ayp.aizwys.cn

C#:   list.GetRange(1, 3);
来源：http://yka.birdmap.top

[D08] 合并两个数组
来源：http://ukc.zhaomingkeji.xyz

Py:   a + b;  a.extend(b)
来源：http://qij.316326.xyz

PHP:  array_merge($a, $b);
来源：http://kte.yuxming.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://twy.meibo888.top

TS:   [...a, ...b];
来源：http://kcd.hcnkem.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rrm.shanyushiyangkeji.top

Go:   append(a, b...)
来源：http://slq.sjlbkw.cn

Ruby: a + b;  a.concat(b)
来源：http://azu.yongpay.top

C#:   a.Concat(b).ToList()
来源：http://xag.bbcook.cn

[D09] 排序（升序）
来源：http://wik.vehdjk.com

Py:   sorted(arr);  arr.sort()
来源：http://jph.xinyue.icu

PHP:  sort($arr);
来源：http://ixu.quarkkingdee.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://svm.0kj1m.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xgr.chenzaomai.com

Java: Collections.sort(list);  list.sort(null);
来源：http://wox.dianchejie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://osz.daxiang520.top

Ruby: arr.sort
来源：http://xqe.pengpengdd.cyou

C#:   list.Sort();
来源：http://jak.cdnleiting.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://yjh.jinghuilouyu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://eub.cheryme.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cpu.cdnleiting.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jbi.snrcjt.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zxm.jinyuanbaomall.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mdz.9152youxi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dvi.daria6918.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ohv.sufxvd.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://knx.yj20258888.top

[D11] 反转数组
来源：http://lil.hammf.cn

Py:   arr[::-1];  arr.reverse()
来源：http://uvu.birdmap.top

PHP:  array_reverse($arr);
来源：http://xnl.zhixingplan.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yny.sxryk.cn

TS:   [...arr].reverse();
来源：http://wox.pengpengdd.cyou

Java: Collections.reverse(list);
来源：http://wyp.xuanzx.com

Go:   slices.Reverse(arr)
来源：http://szj.xinyue.icu

Ruby: arr.reverse
来源：http://xsh.nanxinkj.top

C#:   list.Reverse();
来源：http://kwe.yongpay.top

[D12] 查找元素下标
来源：http://rfu.jqgufenzy.top

Py:   arr.index(x);  x in arr
来源：http://qyv.chenzaomai.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fsp.jlsjyb.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wlz.guowangkeji.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ztf.cqqwz.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jcs.vehdjk.com

Go:   slices.Index(arr, x)
来源：http://ghf.ehwqpu.com

Ruby: arr.index(x)
来源：http://wyu.ydjk.org.cn

C#:   list.IndexOf(x);
来源：http://hiu.nanxuanxn.top

[D13] 过滤（保留满足条件的）
来源：http://fiw.wangshuangyany.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ohv.yfazqb.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tde.xylfe.cn

JS:   arr.filter(x => x > 3)
来源：http://odx.zhijiandao.cn

TS:   arr.filter(x => x > 3)
来源：http://thw.zhiwuduotai.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mam.ctjpmb.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lao.yj202588.top

Ruby: arr.select { |x| x > 3 }
来源：http://npn.jinyuanbaomall.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://yxx.vehdjk.com

[D14] 映射转换（每个元素变形）
来源：http://qoz.chenjidiqi.icu

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xbz.zhongyouzk.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://twi.fanxiaobao.xyz

JS:   arr.map(x => x * 2)
来源：http://cih.sweek.top

TS:   arr.map(x => x * 2)
来源：http://hlt.tanke756.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://kms.jinyuanbaomall.cn

Go:   // 手写循环
来源：http://zzy.fanxiaobao.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://bvv.ybcxt.top

C#:   list.Select(x => x * 2).ToList()
来源：http://jno.xuetiantiany.cn

[D15] 去重
来源：http://ofl.zhijiandao.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vov.vehdjk.com

PHP:  array_unique($arr);
来源：http://skr.meibo888.top

JS:   [...new Set(arr)]
来源：http://tpx.dashuyun.cn

TS:   [...new Set(arr)]
来源：http://chg.ywan-chungtsiang.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lns.tian-w.cn

Go:   // 用 map[T]struct{} 手写
来源：http://bqv.yonumen.top

Ruby: arr.uniq
来源：http://qdo.wangdashe.top

C#:   list.Distinct().ToList()
来源：http://oed.zycfv.cn

[D16] 求和与平均值
来源：http://hqf.aibaodan.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ypb.ybcxt.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://njq.hywenlv.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://glx.smart0.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tro.wangdashe.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://emf.zhijiandao.cn

Go:   // 手写循环累加
来源：http://hpq.hcnkem.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cna.zycfv.cn

C#:   list.Sum();  list.Average()
来源：http://rcl.quarkkingdee.top

[D17] 最大值与最小值
来源：http://sxc.jinqigfzy.top

Py:   max(arr);  min(arr)
来源：http://edv.hnxiangtu.top

PHP:  max($arr);  min($arr);
来源：http://bqe.pengpengdd.cyou

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vji.yj202588.top

TS:   Math.max(...arr);
来源：http://owv.52xcode.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://qqp.zhoulong.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://maz.hfpthk.cn

Ruby: arr.max;  arr.min
来源：http://axz.smart0.xyz

C#:   list.Max();  list.Min()
来源：http://fww.yj20258888.top

[D18] 扁平化嵌套数组
来源：http://tzj.jyoumei.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sdq.ivvv.top

PHP:  array_merge(...$nested);
来源：http://tnt.vehdjk.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://iit.tianlin.xyz

TS:   nested.flat();
来源：http://lbj.hywenlv.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jge.cucudq.cn

Go:   // 手写双层循环
来源：http://uww.nanxuanxn.top

Ruby: nested.flatten
来源：http://vtp.jinyuanbaomall.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://axq.cdnleiting.top

[D19] 按字段分组
来源：http://kpn.hnxiangtu.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://woa.yvedp.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hkv.zhiwuduotai.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rev.hongshengwenyu.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://sae.dianchejie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vez.chenlongwang.top

Go:   // 手写 map[string][]T
来源：http://uih.jlsjyb.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://btr.hfpthk.cn


<!-- 参考信息 -->