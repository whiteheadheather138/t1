代发 wailian999

================================================================================
来源：http://sig.shanyushiyangtech.top

C. 函数与作用域
来源：http://vpf.jyoumei.cn

================================================================================
来源：http://wbl.shangyingyoupin.top

[C01] 定义函数
来源：http://yad.guowangkeji.top

Py:   def add(a, b): return a + b
来源：http://kud.andypj.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://azu.wangshuangyany.cn

JS:   function add(a, b) { return a + b; }
来源：http://ocp.chenzaomai.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hcq.zhiwuduotai.top

Java: static int add(int a, int b) { return a + b; }
来源：http://cwh.dashuyun.cn

Go:   func add(a, b int) int { return a + b }
来源：http://rbs.ywan-chungtsiang.top

Ruby: def add(a, b); a + b; end
来源：http://zlf.jinghuilouyu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://che.gogol.net.cn

[C02] 默认参数
来源：http://xxn.pengpengdd.cyou

Py:   def greet(name="World"): return name
来源：http://zah.ydjk.org.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://smc.vehdjk.com

JS:   function greet(name = "World") { return name; }
来源：http://mnt.hcnkem.com

TS:   function greet(name: string = "World") { return name; }
来源：http://ymb.wangdashe.top

Java: // 无默认参数：方法重载或 Optional
来源：http://hne.zdbjq.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hvv.hcnkem.com

Ruby: def greet(name = "World") = name
来源：http://ztb.tianlin.xyz

C#:   string Greet(string name = "World") => name;
来源：http://iox.xylfe.cn

[C03] 可变参数
来源：http://hdl.c1oappe.top

Py:   def total(*args): return sum(args)
来源：http://sir.uphjek.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xhs.cqqwz.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://utp.redwolf501.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vvj.vehdjk.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://acg.fanxiaobao.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yfz.yuanzhike.top

Ruby: def total(*nums); nums.sum; end
来源：http://wuq.zhixingplan.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kbl.chenlongwang.top

[C04] 命名参数 / 关键字参数
来源：http://dif.wangshuangyany.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://etp.aizwys.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://frq.guannengcc.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://sjg.yueranfly.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://eol.cashguo.top

Java: // 无：用 Builder 模式或 record
来源：http://hse.ydzc1.top

Go:   // 无：用配置结构体参数
来源：http://npz.fehbvm.com

Ruby: f(a: 1, b: 2)
来源：http://fxd.ivvv.top

C#:   f(a: 1, b: 2)
来源：http://pgp.nanxuanxn.top

[C05] 返回多个值
来源：http://rkm.fktsv.cn

Py:   return a, b
来源：http://hwt.guowangkeji.top

PHP:  return [$a, $b];
来源：http://hmm.cqqwz.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://vvo.epnwcf.com

TS:   return { a, b };
来源：http://qge.yj202588.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lic.hongshengwenyu.top

Go:   return a, b
来源：http://oyh.zhengqikj.top

Ruby: return a, b
来源：http://sjx.yongpay.top

C#:   return (a, b);              // ValueTuple
来源：http://rsr.fengsongda.top

[C06] 匿名函数 / lambda
来源：http://kbs.sxryk.cn

Py:   square = lambda x: x * x
来源：http://bog.redwolf501.top

PHP:  $square = fn($x) => $x * $x;
来源：http://fyu.zycfv.cn

JS:   const square = x => x * x;
来源：http://szb.shanyushiyangtech.top

TS:   const square = (x: number): number => x * x;
来源：http://bep.yonumen.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tdr.shanyushiyangtech.top

Go:   sq := func(x int) int { return x * x }
来源：http://jie.yongpay.top

Ruby: square = ->(x) { x * x }
来源：http://mvr.jinghuilouyu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ckr.hongshengwenyu.top

[C07] 把函数作为参数传入
来源：http://fai.hywenlv.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://teo.cdnleiting.top

PHP:  array_map("strtoupper", $arr);
来源：http://mmm.jiagoushi.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://klz.yongpay.top

TS:   arr.map(String)
来源：http://vel.wangdashe.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://box.chenjidiqi.icu

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tad.jinyuanbaomall.cn

Ruby: arr.map(&:upcase)
来源：http://deo.zhoulong.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://dlw.kuanghao11.cn

[C08] 闭包
来源：http://nhl.hongshengwenyu.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://oez.yj20258888.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ukw.yueranfly.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cir.cheryme.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jbz.zhiwuduotai.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xae.jinyuanbaomall.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://djz.yj20258888.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://obw.gaohongyu789.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dvd.sxryk.cn

[C09] 递归
来源：http://pnb.guannengcc.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wcx.zhongyouzk.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://coj.vqdsnc.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gva.jinghuilouyu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qry.jinqigfzy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://sxl.fehbvm.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zer.bjfxy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://aoh.gzhubu.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ucn.pengpengdd.cyou

[C10] 变量作用域
来源：http://vvx.yj202588.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ldn.birdmap.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dbi.hywenlv.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dkr.gaohongyu789.top

TS:   同 JS
来源：http://kdf.havefunace.top

Java: 方法内为块级作用域
来源：http://tpu.wangdashe.top

Go:   花括号块级作用域
来源：http://rok.vehdjk.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xxy.cucudq.cn

C#:   块级作用域
来源：http://kwh.daria6918.cn

[C11] 模块导入与导出
来源：http://mtk.xinyue.icu

Py:   from module import func
来源：http://vya.jinqigufen.top

PHP:  require "file.php";  或 use App\Service;
来源：http://nne.316326.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://zhv.jianghu66.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nqs.zhijiandao.cn

Java: import java.util.List;
来源：http://nfe.fehbvm.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xry.vqdsnc.cn

Ruby: require "json"; require_relative "./util"
来源：http://tcc.shzxlz.cn

C#:   using System.Text;
来源：http://bjl.zhiwuduotai.top

[C12] 立即执行函数 IIFE
来源：http://vwe.zhixingplan.top

Py:   (lambda: print("run"))()
来源：http://fhg.xziqi.cn

PHP:  (function () { echo "run"; })();
来源：http://ugr.yueranfly.top

JS:   (() => { console.log("run"); })();
来源：http://aio.yj202588.top

TS:   (() => { console.log("run"); })();
来源：http://hce.epnwcf.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lyz.hcnkem.com

Go:   func() { fmt.Println("run") }()
来源：http://fnf.hesvh.cn

Ruby: -> { puts "run" }.call
来源：http://yml.ywan-chungtsiang.top

C#:   // 无 IIFE：用静态构造函数
来源：http://huf.xingfuxueyuan.xyz

[C13] 类型声明 / 类型注解
来源：http://oif.xuetiantiany.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://eud.shanyushiyangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uqy.fengsongda.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kgx.smart0.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yqd.jyoumei.cn

Java: int add(int a, int b) { return a + b; }
来源：http://gfi.cdnleiting.top

Go:   func add(a, b int) int
来源：http://ndl.yj20258.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ibb.guowangkeji.top

C#:   int Add(int a, int b) => a + b;
来源：http://amo.havefunace.top

[C14] 泛型函数
来源：http://lih.bbcook.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://apn.sweek.top

PHP:  // 无泛型
来源：http://sxt.jqgufenzy.top

JS:   // 无泛型
来源：http://ebm.0kj1m.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tmo.dianchejie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://maw.fzhhl.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://byj.sweek.top

Ruby: # 无泛型
来源：http://nyq.ctjpmb.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ycr.quarkkingdee.top

[C15] 解构 / 展开参数
来源：http://crq.svipenyu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jxw.tianlin.xyz

PHP:  [$a, $b] = $pair;
来源：http://aiy.xylfe.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xjo.nwbrower.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sjy.shanyushiyangtech.top

Java: // 无解构
来源：http://csb.aibaodan.cn

Go:   // 无解构
来源：http://bbg.hywenlv.cn

Ruby: a, b = pair
来源：http://rel.gotoacloud.top

C#:   var (a, b) = pair;
来源：http://vzz.yanxiufei.cn

[C16] 函数 / 方法重载
来源：http://and.mhx1999.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tsp.gzhubu.top

PHP:  // 无重载
来源：http://bib.wangshuangyany.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ehn.zhengqikj.top

TS:   // 用联合类型或重载签名声明
来源：http://eoo.zdbjq.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://mns.fzhhl.top

Go:   // 无重载：用不同函数名
来源：http://xic.jinqigufen.top

Ruby: # 无重载：靠动态参数
来源：http://cde.tarul.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://rha.smart0.xyz

================================================================================
来源：http://eal.fzhhl.top

D. 数组 / 列表 / 集合
来源：http://rqt.hcnkem.com

================================================================================
来源：http://hyz.9152youxi.cn

[D01] 创建数组 / 列表
来源：http://pho.sxryk.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://fwe.cashguo.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nfi.shanyushiyangtech.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ugr.jianghu66.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://auv.chenzaomai.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://shj.zhongyouzk.top

Go:   arr := []int{1, 2, 3}
来源：http://lmu.fehbvm.com

Ruby: arr = [1, 2, 3]
来源：http://upv.yj20258.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fgm.guowangkeji.top

[D02] 追加元素到末尾
来源：http://lot.9152youxi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://buh.shangyingyoupin.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vbs.hammf.cn

JS:   arr.push(4);
来源：http://qia.gotoacloud.top

TS:   arr.push(4);
来源：http://jgo.jlsjyb.cn

Java: list.add(4);
来源：http://tyt.cheryme.top

Go:   arr = append(arr, 4)
来源：http://kct.52xcode.cn

Ruby: arr << 4; arr.push(5)
来源：http://fug.yvedp.cn

C#:   list.Add(4);
来源：http://jjv.gzhubu.top

[D03] 在指定位置插入元素
来源：http://mzi.xylfe.cn

Py:   arr.insert(0, 0)
来源：http://pnf.daxiang520.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bar.feifeiyinyue.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fvo.pengpengdd.cyou

TS:   arr.splice(0, 0, 0);
来源：http://vkr.fzhhl.top

Java: list.add(0, 0);
来源：http://sca.jinyuanbaomall.cn

Go:   arr = append([]int{0}, arr...)
来源：http://gev.jinghuilouyu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bme.gaohongyu789.top

C#:   list.Insert(0, 0);
来源：http://ljl.yj202588.top

[D04] 删除元素
来源：http://jsm.iojbl.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ziw.hnxiangtu.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gfd.zhengqikj.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qpk.snrcjt.cn

TS:   arr.splice(0, 1);
来源：http://drx.jqgufenzy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://iri.shangyingyoupin.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dpe.cheryme.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ims.sxryk.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xnd.guannengcc.top

[D05] 访问与修改元素
来源：http://oog.nanxuanxn.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://iws.zhiwuduotai.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://udo.zdqjudy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jcd.fktsv.cn

TS:   arr[0]; arr.at(-1);
来源：http://nto.yj202588.top

Java: list.get(0); list.set(0, 9);
来源：http://knd.jyoumei.cn

Go:   arr[0]; arr[0] = 9
来源：http://vmf.yj202588.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dkc.xinyue.icu

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://imp.zycfv.cn

[D06] 数组长度
来源：http://dxx.hnqzz.top

Py:   len(arr)
来源：http://knc.gaohongyu789.top

PHP:  count($arr);
来源：http://wrl.jinqigufen.top

JS:   arr.length
来源：http://yfx.wangdashe.top

TS:   arr.length
来源：http://njw.jinyuanbaomall.cn

Java: list.size();
来源：http://ayx.yonumen.top

Go:   len(arr)
来源：http://axz.shanyushiyangkeji.top

Ruby: arr.length; arr.size
来源：http://mba.aibaodan.cn

C#:   list.Count;
来源：http://uny.vehdjk.com

[D07] 切片 / 取子数组
来源：http://niu.gogol.net.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://uhq.vqdsnc.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qqa.zdbjq.cn

JS:   arr.slice(1, 4);
来源：http://sxl.shangyingyoupin.top

TS:   arr.slice(1, 4);
来源：http://asn.bjfxy.top

Java: list.subList(1, 4);
来源：http://vrh.nwbrower.top

Go:   arr[1:4]
来源：http://nkt.ybcxt.top

Ruby: arr[1, 3]
来源：http://pss.zdqjudy.top

C#:   list.GetRange(1, 3);
来源：http://efy.yuxming.cn

[D08] 合并两个数组
来源：http://afu.iojbl.cn

Py:   a + b;  a.extend(b)
来源：http://eax.jinghuilouyu.cn

PHP:  array_merge($a, $b);
来源：http://qbr.zhoulong.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://jiv.andypj.xyz

TS:   [...a, ...b];
来源：http://qrg.yueranfly.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wau.cashguo.top

Go:   append(a, b...)
来源：http://wkv.ppjwa.cn

Ruby: a + b;  a.concat(b)
来源：http://kps.hnxiangtu.top

C#:   a.Concat(b).ToList()
来源：http://ypv.fanxiaobao.xyz

[D09] 排序（升序）
来源：http://oxx.chenzaomai.com

Py:   sorted(arr);  arr.sort()
来源：http://qns.jiagoushi.top

PHP:  sort($arr);
来源：http://jhw.xuetiantiany.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://otv.quarkkingdee.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://lpt.kuanghao11.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://bof.jinghuilouyu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mtw.nanxinkj.top

Ruby: arr.sort
来源：http://wac.epnwcf.com

C#:   list.Sort();
来源：http://mbz.ppjwa.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://zlo.jianghu66.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wpv.zhoulong.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://abo.mhx1999.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fgw.gzhubu.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gon.tian-w.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lvc.ppjwa.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gsv.ppjwa.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vyp.ivvv.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dpu.fzhhl.top

[D11] 反转数组
来源：http://dja.yuxming.cn

Py:   arr[::-1];  arr.reverse()
来源：http://rxr.jqgufenzy.top

PHP:  array_reverse($arr);
来源：http://bwj.xuanzx.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tlf.jlsjyb.cn

TS:   [...arr].reverse();
来源：http://npn.hnqzz.top

Java: Collections.reverse(list);
来源：http://zjd.daxiang520.top

Go:   slices.Reverse(arr)
来源：http://qka.zhixingplan.top

Ruby: arr.reverse
来源：http://rcz.ybcxt.top

C#:   list.Reverse();
来源：http://zil.cheryme.top

[D12] 查找元素下标
来源：http://fly.birdmap.top

Py:   arr.index(x);  x in arr
来源：http://gsm.yanxiufei.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://krc.epnwcf.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hkf.jinqigufen.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ize.ivvv.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qey.vehdjk.com

Go:   slices.Index(arr, x)
来源：http://slv.316326.xyz

Ruby: arr.index(x)
来源：http://gqx.pengpengdd.cyou

C#:   list.IndexOf(x);
来源：http://vsj.yuanzhike.top

[D13] 过滤（保留满足条件的）
来源：http://haw.fengsongda.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vyr.fengsongda.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pqg.hammf.cn

JS:   arr.filter(x => x > 3)
来源：http://cve.shanyushiyangtech.top

TS:   arr.filter(x => x > 3)
来源：http://hop.gaohongyu789.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zpn.kuanghao11.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pyf.jinqigufen.top

Ruby: arr.select { |x| x > 3 }
来源：http://roh.ywan-chungtsiang.top

C#:   list.Where(x => x > 3).ToList()
来源：http://qiu.birdmap.top

[D14] 映射转换（每个元素变形）
来源：http://ctj.sjlbkw.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nkw.nwbrower.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ndj.shzxlz.cn

JS:   arr.map(x => x * 2)
来源：http://frg.smart0.xyz

TS:   arr.map(x => x * 2)
来源：http://tng.kuanghao11.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://lne.vqdsnc.cn

Go:   // 手写循环
来源：http://xly.vqdsnc.cn

Ruby: arr.map { |x| x * 2 }
来源：http://rpv.haohaochexian.top

C#:   list.Select(x => x * 2).ToList()
来源：http://uof.uphjek.com

[D15] 去重
来源：http://hgc.pycfn.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ktz.nanxuanxn.top

PHP:  array_unique($arr);
来源：http://fvz.gzhubu.top

JS:   [...new Set(arr)]
来源：http://bsi.zhijiandao.cn

TS:   [...new Set(arr)]
来源：http://daa.dianchejie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mka.cashguo.top

Go:   // 用 map[T]struct{} 手写
来源：http://woe.iojbl.cn

Ruby: arr.uniq
来源：http://vaq.tianlin.xyz

C#:   list.Distinct().ToList()
来源：http://arg.ivvv.top

[D16] 求和与平均值
来源：http://ium.9152youxi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nie.pengpengdd.cyou

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xwh.hcnkem.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wcq.ybcxt.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rra.ybcxt.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rmz.ctjpmb.com

Go:   // 手写循环累加
来源：http://jni.yanxiufei.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qft.0kj1m.cn

C#:   list.Sum();  list.Average()
来源：http://nda.ppjwa.cn

[D17] 最大值与最小值
来源：http://rhx.hfpthk.cn

Py:   max(arr);  min(arr)
来源：http://gmc.yuxming.cn

PHP:  max($arr);  min($arr);
来源：http://xwl.hammf.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rjo.jinqigufen.top

TS:   Math.max(...arr);
来源：http://nro.sxryk.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://nza.wangdashe.top


<!-- 参考信息 -->