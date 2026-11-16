代发 wailian999

Py:   def add(a, b): return a + b
来源：http://bls.tarul.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://npb.zhiwuduotai.top

JS:   function add(a, b) { return a + b; }
来源：http://ffd.guowangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rpc.shuidangran.top

Java: static int add(int a, int b) { return a + b; }
来源：http://vnc.316326.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://ilf.xylfe.cn

Ruby: def add(a, b); a + b; end
来源：http://zot.birdmap.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yoy.316326.xyz

[C02] 默认参数
来源：http://mka.cqqwz.cn

Py:   def greet(name="World"): return name
来源：http://zxx.hammf.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://kvb.hcnkem.com

JS:   function greet(name = "World") { return name; }
来源：http://eep.52xcode.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hkn.andypj.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://svm.jinqigufen.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fxg.tian-w.cn

Ruby: def greet(name = "World") = name
来源：http://jvt.smart0.xyz

C#:   string Greet(string name = "World") => name;
来源：http://kvn.hongshengwenyu.top

[C03] 可变参数
来源：http://fzk.dashuyun.cn

Py:   def total(*args): return sum(args)
来源：http://dso.yanxiufei.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lem.chenjidiqi.icu

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gsh.aibaodan.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wcd.xziqi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mvj.vqdsnc.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kld.bbcook.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ygw.zhiwuduotai.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wvw.xingfuxueyuan.xyz

[C04] 命名参数 / 关键字参数
来源：http://kgz.ydjk.org.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ffj.sysykeji.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://cwo.daxiang520.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ycr.yj20258888.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://eht.ehwqpu.com

Java: // 无：用 Builder 模式或 record
来源：http://nst.0kj1m.cn

Go:   // 无：用配置结构体参数
来源：http://mog.guowangkeji.top

Ruby: f(a: 1, b: 2)
来源：http://zjs.cucudq.cn

C#:   f(a: 1, b: 2)
来源：http://qol.yj20258888.top

[C05] 返回多个值
来源：http://mfi.fanxiaobao.xyz

Py:   return a, b
来源：http://fmu.ehwqpu.com

PHP:  return [$a, $b];
来源：http://wkx.bjfxy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://dzn.hongshengwenyu.top

TS:   return { a, b };
来源：http://ral.zhiwuduotai.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://uyv.chenlongwang.top

Go:   return a, b
来源：http://enb.fehbvm.com

Ruby: return a, b
来源：http://gub.hfpthk.cn

C#:   return (a, b);              // ValueTuple
来源：http://loj.sweek.top

[C06] 匿名函数 / lambda
来源：http://wmz.yj20258888.top

Py:   square = lambda x: x * x
来源：http://ixr.haohaochexian.top

PHP:  $square = fn($x) => $x * $x;
来源：http://jkf.ctjpmb.com

JS:   const square = x => x * x;
来源：http://bri.tian-w.cn

TS:   const square = (x: number): number => x * x;
来源：http://cyj.yj20258888.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wyo.quarkkingdee.top

Go:   sq := func(x int) int { return x * x }
来源：http://nak.shanyushiyangkeji.top

Ruby: square = ->(x) { x * x }
来源：http://yph.xylfe.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ojm.jyoumei.cn

[C07] 把函数作为参数传入
来源：http://ouq.shangyingyoupin.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bcv.yuanzhike.top

PHP:  array_map("strtoupper", $arr);
来源：http://dij.tianlin.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kji.fktsv.cn

TS:   arr.map(String)
来源：http://ora.316326.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://roo.shanyushiyangkeji.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jba.iojbl.cn

Ruby: arr.map(&:upcase)
来源：http://dky.zdqjudy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://pbr.xuetiantiany.cn

[C08] 闭包
来源：http://icc.daria6918.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://due.cdnleiting.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://los.daria6918.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rld.aibaodan.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fji.hnqzz.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dar.yongpay.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kov.zhiwuduotai.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kne.c1oappe.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ubk.svipenyu.cn

[C09] 递归
来源：http://kcs.gotoacloud.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kol.quarkkingdee.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://joc.chenjidiqi.icu

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://npi.xinyue.icu

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jdm.pengpengdd.cyou

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://abt.birdmap.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://che.fanxiaobao.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hpt.feifeiyinyue.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rvi.yangfankeji.com

[C10] 变量作用域
来源：http://lnv.tianlin.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bhw.shuidangran.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mtu.yanxiufei.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ewy.epnwcf.com

TS:   同 JS
来源：http://jnv.meibo888.top

Java: 方法内为块级作用域
来源：http://kly.zdbjq.cn

Go:   花括号块级作用域
来源：http://qla.iojbl.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://csd.xinyue.icu

C#:   块级作用域
来源：http://ryo.vqdsnc.cn

[C11] 模块导入与导出
来源：http://dyi.xylfe.cn

Py:   from module import func
来源：http://vld.zdqjudy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://knv.gogol.net.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://oli.zdqjudy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fou.fanxiaobao.xyz

Java: import java.util.List;
来源：http://vhb.sufxvd.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://sml.jyoumei.cn

Ruby: require "json"; require_relative "./util"
来源：http://qdt.fktsv.cn

C#:   using System.Text;
来源：http://igt.fktsv.cn

[C12] 立即执行函数 IIFE
来源：http://mck.bjfxy.top

Py:   (lambda: print("run"))()
来源：http://sbg.hywenlv.cn

PHP:  (function () { echo "run"; })();
来源：http://eza.xinyue.icu

JS:   (() => { console.log("run"); })();
来源：http://uzo.zhengqikj.top

TS:   (() => { console.log("run"); })();
来源：http://tvz.quarkkingdee.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ome.fengsongda.top

Go:   func() { fmt.Println("run") }()
来源：http://xsh.52xcode.cn

Ruby: -> { puts "run" }.call
来源：http://pfb.sxryk.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://vvi.bjfxy.top

[C13] 类型声明 / 类型注解
来源：http://ywq.iojbl.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://irh.ybcxt.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://chr.jiagoushi.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sjv.jqgfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lky.ydjk.org.cn

Java: int add(int a, int b) { return a + b; }
来源：http://mmr.jqgufenzy.top

Go:   func add(a, b int) int
来源：http://jhv.zhijiandao.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://oci.ppjwa.cn

C#:   int Add(int a, int b) => a + b;
来源：http://jli.fehbvm.com

[C14] 泛型函数
来源：http://srd.ydjk.org.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xgk.chenjidiqi.icu

PHP:  // 无泛型
来源：http://mwc.yongpay.top

JS:   // 无泛型
来源：http://azk.smart0.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ywa.gaohongyu789.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ntj.ywan-chungtsiang.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lst.wangdashe.top

Ruby: # 无泛型
来源：http://xfi.yueranfly.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jrk.vehdjk.com

[C15] 解构 / 展开参数
来源：http://con.hfpthk.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xha.cqqwz.cn

PHP:  [$a, $b] = $pair;
来源：http://djg.zhixingplan.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://daq.wangshuangyany.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wqc.chenjidiqi.icu

Java: // 无解构
来源：http://sok.yuxming.cn

Go:   // 无解构
来源：http://iqq.yongpay.top

Ruby: a, b = pair
来源：http://xfl.gotoacloud.top

C#:   var (a, b) = pair;
来源：http://uwu.yonumen.top

[C16] 函数 / 方法重载
来源：http://zth.zhaomingkeji.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xky.jinqigufen.top

PHP:  // 无重载
来源：http://pdg.xingfuxueyuan.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://zjm.jyoumei.cn

TS:   // 用联合类型或重载签名声明
来源：http://lpn.vqdsnc.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://fau.guowangkeji.top

Go:   // 无重载：用不同函数名
来源：http://wbu.aibaodan.cn

Ruby: # 无重载：靠动态参数
来源：http://adh.xziqi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qoh.tianlin.xyz

================================================================================
来源：http://aei.birdmap.top

D. 数组 / 列表 / 集合
来源：http://bvb.ivvv.top

================================================================================
来源：http://xpr.gaohongyu789.top

[D01] 创建数组 / 列表
来源：http://lfc.ydzc1.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://yao.haohaochexian.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xdv.zhaomingkeji.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wja.sufxvd.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ret.gotoacloud.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zmh.jinqigfzy.top

Go:   arr := []int{1, 2, 3}
来源：http://tkp.jiagoushi.top

Ruby: arr = [1, 2, 3]
来源：http://vmg.zhengqikj.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mfx.cucudq.cn

[D02] 追加元素到末尾
来源：http://czc.cashguo.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hdy.gaohongyu789.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rrp.xuetiantiany.cn

JS:   arr.push(4);
来源：http://cdg.quarkkingdee.top

TS:   arr.push(4);
来源：http://xnr.zhaomingkeji.xyz

Java: list.add(4);
来源：http://cjv.jinghuilouyu.cn

Go:   arr = append(arr, 4)
来源：http://zkx.fktsv.cn

Ruby: arr << 4; arr.push(5)
来源：http://wqb.guowangkeji.top

C#:   list.Add(4);
来源：http://doo.uphjek.com

[D03] 在指定位置插入元素
来源：http://qms.sweek.top

Py:   arr.insert(0, 0)
来源：http://vgx.snrcjt.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cwf.fktsv.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pze.ydzc1.top

TS:   arr.splice(0, 0, 0);
来源：http://wur.sysykeji.top

Java: list.add(0, 0);
来源：http://mds.cucudq.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ohp.sweek.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fzr.epnwcf.com

C#:   list.Insert(0, 0);
来源：http://gcs.ehwqpu.com

[D04] 删除元素
来源：http://jjx.sufxvd.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://oyg.ctjpmb.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kll.zhengqikj.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jct.aibaodan.cn

TS:   arr.splice(0, 1);
来源：http://onu.c1oappe.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://afm.zhaomingkeji.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hsm.birdmap.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vhi.xziqi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bik.zhixingplan.top

[D05] 访问与修改元素
来源：http://drz.sysykeji.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://evz.hywenlv.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://srn.shzxlz.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ffk.zdbjq.cn

TS:   arr[0]; arr.at(-1);
来源：http://ihd.jinghuilouyu.cn

Java: list.get(0); list.set(0, 9);
来源：http://fje.redwolf501.top

Go:   arr[0]; arr[0] = 9
来源：http://wfy.jinqigufen.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ygb.hongshengwenyu.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://auh.hongshengwenyu.top

[D06] 数组长度
来源：http://fji.tian-w.cn

Py:   len(arr)
来源：http://hrc.hfpthk.cn

PHP:  count($arr);
来源：http://awx.bjfxy.top

JS:   arr.length
来源：http://ahg.zdqjudy.top

TS:   arr.length
来源：http://bgo.fengsongda.top

Java: list.size();
来源：http://eqf.yueranfly.top

Go:   len(arr)
来源：http://dai.bbcook.cn

Ruby: arr.length; arr.size
来源：http://xro.yongpay.top

C#:   list.Count;
来源：http://die.zhiwuduotai.top

[D07] 切片 / 取子数组
来源：http://qnt.yueranfly.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gub.nanxuanxn.top

PHP:  array_slice($arr, 1, 3);
来源：http://rro.ehwqpu.com

JS:   arr.slice(1, 4);
来源：http://gmx.cheryme.top

TS:   arr.slice(1, 4);
来源：http://vgw.vqdsnc.cn

Java: list.subList(1, 4);
来源：http://tqc.jinghuilouyu.cn

Go:   arr[1:4]
来源：http://avi.jinghuilouyu.cn

Ruby: arr[1, 3]
来源：http://qiu.daxiang520.top

C#:   list.GetRange(1, 3);
来源：http://eam.yvedp.cn

[D08] 合并两个数组
来源：http://sya.guowangkeji.top

Py:   a + b;  a.extend(b)
来源：http://nus.aizwys.cn

PHP:  array_merge($a, $b);
来源：http://krp.0kj1m.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://gdp.fktsv.cn

TS:   [...a, ...b];
来源：http://yta.guowangkeji.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ked.ppjwa.cn

Go:   append(a, b...)
来源：http://bil.gogol.net.cn

Ruby: a + b;  a.concat(b)
来源：http://bta.cashguo.top

C#:   a.Concat(b).ToList()
来源：http://csu.cdnleiting.top

[D09] 排序（升序）
来源：http://fps.zhaomingkeji.xyz

Py:   sorted(arr);  arr.sort()
来源：http://pyh.gotoacloud.top

PHP:  sort($arr);
来源：http://mec.sysykeji.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yyq.fktsv.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://jby.52xcode.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://okr.smart0.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ytw.andypj.xyz

Ruby: arr.sort
来源：http://wwx.ehwqpu.com

C#:   list.Sort();
来源：http://qib.quarkkingdee.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://pxp.fzhhl.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kgp.yongpay.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nff.hnqzz.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sqq.smart0.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rib.feifeiyinyue.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ryb.xuetiantiany.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kfh.tianlin.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dve.shanyushiyangkeji.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bou.iojbl.cn

[D11] 反转数组
来源：http://fub.bbcook.cn

Py:   arr[::-1];  arr.reverse()
来源：http://crx.sysykeji.top

PHP:  array_reverse($arr);
来源：http://acc.cheryme.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mgt.shzxlz.cn

TS:   [...arr].reverse();
来源：http://wvq.tarul.cn

Java: Collections.reverse(list);
来源：http://hmc.zdqjudy.top

Go:   slices.Reverse(arr)
来源：http://okd.aibaodan.cn

Ruby: arr.reverse
来源：http://pti.yueranfly.top

C#:   list.Reverse();
来源：http://rsv.sweek.top

[D12] 查找元素下标
来源：http://cvb.yuanzhike.top

Py:   arr.index(x);  x in arr
来源：http://zhl.yuanzhike.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pyo.iojbl.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jlq.jqgufenzy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jag.vqdsnc.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qbg.ppjwa.cn

Go:   slices.Index(arr, x)
来源：http://pgb.yuanzhike.top

Ruby: arr.index(x)
来源：http://kdw.hongshengwenyu.top

C#:   list.IndexOf(x);
来源：http://jnd.sjlbkw.cn

[D13] 过滤（保留满足条件的）
来源：http://pad.xinyue.icu

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://iut.fzhhl.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rbn.hfpthk.cn

JS:   arr.filter(x => x > 3)
来源：http://isq.52xcode.cn

TS:   arr.filter(x => x > 3)
来源：http://rrs.sjlbkw.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://iae.nanxuanxn.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mld.bbcook.cn

Ruby: arr.select { |x| x > 3 }
来源：http://inh.hongshengwenyu.top

C#:   list.Where(x => x > 3).ToList()
来源：http://hxo.guannengcc.top

[D14] 映射转换（每个元素变形）
来源：http://ozx.sjlbkw.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gaf.jinyuanbaomall.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://szl.fehbvm.com

JS:   arr.map(x => x * 2)
来源：http://xwh.chenzaomai.com

TS:   arr.map(x => x * 2)
来源：http://uqu.zhongyouzk.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://duh.zhongyouzk.top

Go:   // 手写循环
来源：http://sbd.jinqigfzy.top

Ruby: arr.map { |x| x * 2 }
来源：http://fqp.tanke756.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ljc.yanxiufei.cn

[D15] 去重
来源：http://tvd.yongpay.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://brf.jinghuilouyu.cn

PHP:  array_unique($arr);
来源：http://zqk.hywenlv.cn

JS:   [...new Set(arr)]
来源：http://oxf.yvedp.cn

TS:   [...new Set(arr)]
来源：http://uji.kuanghao11.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jwx.shanyushiyangtech.top

Go:   // 用 map[T]struct{} 手写
来源：http://xek.aibaodan.cn

Ruby: arr.uniq
来源：http://hjv.gzhubu.top

C#:   list.Distinct().ToList()
来源：http://tgg.jinghuilouyu.cn

[D16] 求和与平均值
来源：http://vqz.jlsjyb.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tuz.mhx1999.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://snn.haohaochexian.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kgj.sufxvd.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://emy.xuetiantiany.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://glo.hysaishi.cn

Go:   // 手写循环累加
来源：http://pre.jinyuanbaomall.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yca.zycfv.cn

C#:   list.Sum();  list.Average()
来源：http://yyt.svipenyu.cn

[D17] 最大值与最小值
来源：http://yan.chenjidiqi.icu

Py:   max(arr);  min(arr)
来源：http://xvf.9152youxi.cn

PHP:  max($arr);  min($arr);
来源：http://mlj.tarul.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rgk.sufxvd.cn

TS:   Math.max(...arr);
来源：http://akp.fzhhl.top

Java: Collections.max(list);  Collections.min(list);
来源：http://piq.zdqjudy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jce.yanxiufei.cn

Ruby: arr.max;  arr.min
来源：http://hvd.wangshuangyany.cn

C#:   list.Max();  list.Min()
来源：http://ndg.zhoulong.xyz

[D18] 扁平化嵌套数组
来源：http://oez.epnwcf.com


<!-- 参考信息 -->