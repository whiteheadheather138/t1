代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://tts.ppjwa.cn

TS:   [1, 2, 3].includes(x)
来源：http://afw.havefunace.top

Java: List.of(1, 2, 3).contains(x)
来源：http://dbw.bbcook.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cko.yangfankeji.com

Ruby: [1, 2, 3].include?(x)
来源：http://tts.ehwqpu.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://edn.smart0.xyz

[B15] 布尔运算与取反
来源：http://rrz.cqqwz.cn

Py:   a and b or not c
来源：http://umn.yvedp.cn

PHP:  $a && $b || !$c
来源：http://lcs.pycfn.com

JS:   a && b || !c
来源：http://mbm.nanxuanxn.top

TS:   a && b || !c
来源：http://fkx.zhaomingkeji.xyz

Java: a && b || !c
来源：http://xdt.hysaishi.cn

Go:   a && b || !c
来源：http://zmg.gotoacloud.top

Ruby: a && b || !c
来源：http://iqa.sufxvd.cn

C#:   a && b || !c
来源：http://vuh.aibaodan.cn

[B16] 卫语句：不满足条件提前返回
来源：http://fiw.jiagoushi.top

Py:   if not data: return
来源：http://grl.xingfuxueyuan.xyz

PHP:  if (!$data) { return; }
来源：http://dht.fengsongda.top

JS:   if (!data) return;
来源：http://hzq.jlsjyb.cn

TS:   if (!data) return;
来源：http://pey.jianghu66.top

Java: if (data == null) return;
来源：http://ire.guowangkeji.top

Go:   if data == nil { return }
来源：http://ndr.zhongyouzk.top

Ruby: return if data.nil?
来源：http://rpr.iojbl.cn

C#:   if (data == null) return;
来源：http://nnx.xinyue.icu

================================================================================
来源：http://ris.sweek.top

C. 函数与作用域
来源：http://ygo.xingfuxueyuan.xyz

================================================================================
来源：http://nxl.aizwys.cn

[C01] 定义函数
来源：http://bge.ybcxt.top

Py:   def add(a, b): return a + b
来源：http://tyr.fehbvm.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pgh.vqdsnc.cn

JS:   function add(a, b) { return a + b; }
来源：http://myt.zhoulong.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ayn.havefunace.top

Java: static int add(int a, int b) { return a + b; }
来源：http://zqq.dashuyun.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ybc.daria6918.cn

Ruby: def add(a, b); a + b; end
来源：http://boj.yvedp.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sve.hesvh.cn

[C02] 默认参数
来源：http://hcb.yfazqb.com

Py:   def greet(name="World"): return name
来源：http://oji.yj20258.top

PHP:  function greet($name = "World") { return $name; }
来源：http://gki.uphjek.com

JS:   function greet(name = "World") { return name; }
来源：http://laa.chenjidiqi.icu

TS:   function greet(name: string = "World") { return name; }
来源：http://nvc.hysaishi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://gyr.birdmap.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dnu.haohaochexian.top

Ruby: def greet(name = "World") = name
来源：http://vgs.zhijiandao.cn

C#:   string Greet(string name = "World") => name;
来源：http://nps.sxryk.cn

[C03] 可变参数
来源：http://ezk.jyoumei.cn

Py:   def total(*args): return sum(args)
来源：http://tbo.zhengqikj.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hyp.yfazqb.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://buz.xziqi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://whf.zhoulong.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://uxn.hnxiangtu.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zrm.zhaomingkeji.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://baa.redwolf501.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://anh.cheryme.top

[C04] 命名参数 / 关键字参数
来源：http://olg.yvedp.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wkb.chenlongwang.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ite.guannengcc.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://doa.zhongyouzk.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://uwq.fzhhl.top

Java: // 无：用 Builder 模式或 record
来源：http://gnd.jianghu66.top

Go:   // 无：用配置结构体参数
来源：http://esz.wangshuangyany.cn

Ruby: f(a: 1, b: 2)
来源：http://ygj.zycfv.cn

C#:   f(a: 1, b: 2)
来源：http://pez.tanke756.top

[C05] 返回多个值
来源：http://our.yuanzhike.top

Py:   return a, b
来源：http://uwc.hysaishi.cn

PHP:  return [$a, $b];
来源：http://awf.jinqigfzy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://sxf.tianlin.xyz

TS:   return { a, b };
来源：http://esn.fehbvm.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mxj.jianghu66.top

Go:   return a, b
来源：http://hqz.hcnkem.com

Ruby: return a, b
来源：http://yww.yongpay.top

C#:   return (a, b);              // ValueTuple
来源：http://eir.hywenlv.cn

[C06] 匿名函数 / lambda
来源：http://kxt.xingfuxueyuan.xyz

Py:   square = lambda x: x * x
来源：http://kco.shzxlz.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://fvi.xuanzx.com

JS:   const square = x => x * x;
来源：http://xkj.epnwcf.com

TS:   const square = (x: number): number => x * x;
来源：http://sjz.yueranfly.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://gif.shanyushiyangkeji.top

Go:   sq := func(x int) int { return x * x }
来源：http://jsm.cashguo.top

Ruby: square = ->(x) { x * x }
来源：http://ptw.shuidangran.top

C#:   Func<int, int> square = x => x * x;
来源：http://vhg.guannengcc.top

[C07] 把函数作为参数传入
来源：http://tjp.daria6918.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xad.quarkkingdee.top

PHP:  array_map("strtoupper", $arr);
来源：http://wei.xuetiantiany.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://goz.dianchejie.cn

TS:   arr.map(String)
来源：http://qnt.guannengcc.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://euh.xuanzx.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ycc.zhoulong.xyz

Ruby: arr.map(&:upcase)
来源：http://dfz.jinyuanbaomall.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://oxp.ydjk.org.cn

[C08] 闭包
来源：http://krf.quarkkingdee.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hzv.316326.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://oja.hnxiangtu.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cmd.tian-w.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xkk.zdqjudy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tse.sysykeji.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rys.xziqi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://azk.tianlin.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lyt.kuanghao11.cn

[C09] 递归
来源：http://tat.sufxvd.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fth.andypj.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gwa.fengsongda.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uyc.chenzaomai.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dov.guowangkeji.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://icg.shzxlz.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://caf.guannengcc.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rch.kuanghao11.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wbz.zhongyouzk.top

[C10] 变量作用域
来源：http://ddv.guowangkeji.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://sev.zycfv.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rsj.haohaochexian.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nhr.9152youxi.cn

TS:   同 JS
来源：http://cdl.sjlbkw.cn

Java: 方法内为块级作用域
来源：http://hlv.ctjpmb.com

Go:   花括号块级作用域
来源：http://nyq.ppjwa.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qpi.yj20258888.top

C#:   块级作用域
来源：http://iev.feifeiyinyue.top

[C11] 模块导入与导出
来源：http://lws.hnqzz.top

Py:   from module import func
来源：http://cbn.chenjidiqi.icu

PHP:  require "file.php";  或 use App\Service;
来源：http://rbz.mhx1999.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://xgz.yanxiufei.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gqj.bbcook.cn

Java: import java.util.List;
来源：http://hjo.shzxlz.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://olq.pengpengdd.cyou

Ruby: require "json"; require_relative "./util"
来源：http://vrj.daxiang520.top

C#:   using System.Text;
来源：http://qsl.guannengcc.top

[C12] 立即执行函数 IIFE
来源：http://auw.yj20258.top

Py:   (lambda: print("run"))()
来源：http://yxd.zhiwuduotai.top

PHP:  (function () { echo "run"; })();
来源：http://yrq.meibo888.top

JS:   (() => { console.log("run"); })();
来源：http://ewx.yj202588.top

TS:   (() => { console.log("run"); })();
来源：http://kow.ppjwa.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://luo.jqgfzy.top

Go:   func() { fmt.Println("run") }()
来源：http://igl.iojbl.cn

Ruby: -> { puts "run" }.call
来源：http://dei.ydjk.org.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ghw.shuidangran.top

[C13] 类型声明 / 类型注解
来源：http://icc.hongshengwenyu.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://urg.sufxvd.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vsx.fanxiaobao.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zqj.jianghu66.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vda.xuanzx.com

Java: int add(int a, int b) { return a + b; }
来源：http://qne.hcnkem.com

Go:   func add(a, b int) int
来源：http://muo.sysykeji.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://noh.zhixingplan.top

C#:   int Add(int a, int b) => a + b;
来源：http://pcu.daxiang520.top

[C14] 泛型函数
来源：http://pdw.gzhubu.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ctu.fktsv.cn

PHP:  // 无泛型
来源：http://kps.zhengqikj.top

JS:   // 无泛型
来源：http://rhq.chenjidiqi.icu

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bcg.xylfe.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gvr.bbcook.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rod.shanyushiyangtech.top

Ruby: # 无泛型
来源：http://wbi.tianlin.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://uic.hnxiangtu.top

[C15] 解构 / 展开参数
来源：http://ere.shangyingyoupin.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hwl.jyoumei.cn

PHP:  [$a, $b] = $pair;
来源：http://foi.xuanzx.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://que.cucudq.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zko.gzhubu.top

Java: // 无解构
来源：http://kmb.ywan-chungtsiang.top

Go:   // 无解构
来源：http://maf.9152youxi.cn

Ruby: a, b = pair
来源：http://ovw.bjfxy.top

C#:   var (a, b) = pair;
来源：http://dck.fktsv.cn

[C16] 函数 / 方法重载
来源：http://wem.nwbrower.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tsx.ivvv.top

PHP:  // 无重载
来源：http://qqm.jyoumei.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://rnz.wangdashe.top

TS:   // 用联合类型或重载签名声明
来源：http://dkf.zhiwuduotai.top

Java: void f(int a) {}  void f(String a) {}
来源：http://axs.316326.xyz

Go:   // 无重载：用不同函数名
来源：http://zyh.nwbrower.top

Ruby: # 无重载：靠动态参数
来源：http://geb.jyoumei.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://rgo.hnqzz.top

================================================================================
来源：http://vvn.hesvh.cn

D. 数组 / 列表 / 集合
来源：http://ebw.wangdashe.top

================================================================================
来源：http://tew.mhx1999.top

[D01] 创建数组 / 列表
来源：http://bxc.feifeiyinyue.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://xlz.yj202588.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://noa.nanxinkj.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cwu.chenlongwang.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://qvw.jinqigfzy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hty.tian-w.cn

Go:   arr := []int{1, 2, 3}
来源：http://qqo.xinyue.icu

Ruby: arr = [1, 2, 3]
来源：http://uxa.chenjidiqi.icu

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mpb.ppjwa.cn

[D02] 追加元素到末尾
来源：http://otp.nanxinkj.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dal.zhixingplan.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zbp.zhengqikj.top

JS:   arr.push(4);
来源：http://rqf.iojbl.cn

TS:   arr.push(4);
来源：http://dmf.hywenlv.cn

Java: list.add(4);
来源：http://sjy.yonumen.top

Go:   arr = append(arr, 4)
来源：http://oap.quarkkingdee.top

Ruby: arr << 4; arr.push(5)
来源：http://bgm.cheryme.top

C#:   list.Add(4);
来源：http://fdb.zhaomingkeji.xyz

[D03] 在指定位置插入元素
来源：http://yxz.aizwys.cn

Py:   arr.insert(0, 0)
来源：http://kle.sweek.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gev.guowangkeji.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cke.uphjek.com

TS:   arr.splice(0, 0, 0);
来源：http://xkv.yfazqb.com

Java: list.add(0, 0);
来源：http://bjx.shangyingyoupin.top

Go:   arr = append([]int{0}, arr...)
来源：http://wps.fengsongda.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rnc.andypj.xyz

C#:   list.Insert(0, 0);
来源：http://ipj.bbcook.cn

[D04] 删除元素
来源：http://vml.cheryme.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rzq.yanxiufei.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zvs.shzxlz.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lpg.birdmap.top

TS:   arr.splice(0, 1);
来源：http://zsk.yuanzhike.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mbm.ydjk.org.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cyr.fzhhl.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mwa.jyoumei.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nep.jinqigufen.top

[D05] 访问与修改元素
来源：http://tqu.aizwys.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xzy.xziqi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://erh.uphjek.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mdh.fehbvm.com

TS:   arr[0]; arr.at(-1);
来源：http://ewk.ydzc1.top

Java: list.get(0); list.set(0, 9);
来源：http://byd.jianghu66.top

Go:   arr[0]; arr[0] = 9
来源：http://hlv.jqgufenzy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kek.yj202588.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://efn.zhaomingkeji.xyz

[D06] 数组长度
来源：http://zqb.shanyushiyangkeji.top

Py:   len(arr)
来源：http://csn.sufxvd.cn

PHP:  count($arr);
来源：http://rpv.yueranfly.top

JS:   arr.length
来源：http://fto.jlsjyb.cn

TS:   arr.length
来源：http://xfm.ctjpmb.com

Java: list.size();
来源：http://ccj.zhaomingkeji.xyz

Go:   len(arr)
来源：http://vjc.sufxvd.cn

Ruby: arr.length; arr.size
来源：http://fpv.svipenyu.cn

C#:   list.Count;
来源：http://geg.zhoulong.xyz

[D07] 切片 / 取子数组
来源：http://hau.shzxlz.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vcz.yonumen.top

PHP:  array_slice($arr, 1, 3);
来源：http://bvn.jqgufenzy.top

JS:   arr.slice(1, 4);
来源：http://oxh.aizwys.cn

TS:   arr.slice(1, 4);
来源：http://dte.fehbvm.com

Java: list.subList(1, 4);
来源：http://cyy.hesvh.cn

Go:   arr[1:4]
来源：http://acr.vehdjk.com

Ruby: arr[1, 3]
来源：http://rfz.sweek.top

C#:   list.GetRange(1, 3);
来源：http://aul.smart0.xyz

[D08] 合并两个数组
来源：http://hqr.yuxming.cn

Py:   a + b;  a.extend(b)
来源：http://egc.sufxvd.cn

PHP:  array_merge($a, $b);
来源：http://qde.fzhhl.top

JS:   [...a, ...b];  a.concat(b);
来源：http://qsg.nanxuanxn.top

TS:   [...a, ...b];
来源：http://see.chenzaomai.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cqg.wangdashe.top

Go:   append(a, b...)
来源：http://afo.zhiwuduotai.top

Ruby: a + b;  a.concat(b)
来源：http://hqr.zdbjq.cn

C#:   a.Concat(b).ToList()
来源：http://wlt.zdbjq.cn

[D09] 排序（升序）
来源：http://qyk.jqgufenzy.top

Py:   sorted(arr);  arr.sort()
来源：http://aed.wangshuangyany.cn

PHP:  sort($arr);
来源：http://odn.wangdashe.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://aaw.yueranfly.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://wjl.dianchejie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://rej.wangdashe.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://slz.yanxiufei.cn

Ruby: arr.sort
来源：http://ymg.jlsjyb.cn

C#:   list.Sort();
来源：http://hdq.guannengcc.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://bec.jyoumei.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zij.smart0.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://agz.epnwcf.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fzr.shzxlz.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zqq.tianlin.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mdl.dianchejie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://igp.yuanzhike.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tpv.sweek.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qwn.cqqwz.cn

[D11] 反转数组
来源：http://yya.xinyue.icu

Py:   arr[::-1];  arr.reverse()
来源：http://sha.sxryk.cn

PHP:  array_reverse($arr);
来源：http://wsc.uphjek.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zmy.jqgufenzy.top

TS:   [...arr].reverse();
来源：http://wvg.cheryme.top

Java: Collections.reverse(list);
来源：http://onq.shzxlz.cn

Go:   slices.Reverse(arr)
来源：http://gwb.svipenyu.cn

Ruby: arr.reverse
来源：http://ibc.uphjek.com

C#:   list.Reverse();
来源：http://fxz.cucudq.cn

[D12] 查找元素下标
来源：http://gxx.kuanghao11.cn

Py:   arr.index(x);  x in arr
来源：http://xug.zhiwuduotai.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tjj.zhoulong.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oow.shanyushiyangtech.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xbq.jinqigfzy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://phr.bbcook.cn

Go:   slices.Index(arr, x)
来源：http://gqy.zhiwuduotai.top

Ruby: arr.index(x)
来源：http://fpc.yanxiufei.cn

C#:   list.IndexOf(x);
来源：http://snh.andypj.xyz

[D13] 过滤（保留满足条件的）
来源：http://zpt.bbcook.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ndh.ehwqpu.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qwa.gotoacloud.top

JS:   arr.filter(x => x > 3)
来源：http://mqu.xinyue.icu

TS:   arr.filter(x => x > 3)
来源：http://ifm.yfazqb.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dcf.gogol.net.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bpv.ehwqpu.com

Ruby: arr.select { |x| x > 3 }
来源：http://wuc.jqgfzy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://zni.zhixingplan.top

[D14] 映射转换（每个元素变形）
来源：http://fzm.sufxvd.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ouh.daria6918.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nzz.svipenyu.cn

JS:   arr.map(x => x * 2)
来源：http://tpm.wangshuangyany.cn

TS:   arr.map(x => x * 2)
来源：http://gbh.zhengqikj.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://mme.yongpay.top

Go:   // 手写循环
来源：http://osc.sweek.top

Ruby: arr.map { |x| x * 2 }
来源：http://wmp.zdqjudy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://tkl.vqdsnc.cn


<!-- 参考信息 -->