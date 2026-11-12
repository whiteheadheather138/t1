代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://aqf.cheryme.top

Java: x instanceof Number
来源：http://znf.iojbl.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mmh.shuidangran.top

Ruby: x.is_a?(Numeric)
来源：http://ajs.yanxiufei.cn

C#:   x is int or double or decimal
来源：http://jyo.gotoacloud.top

[B14] 判断值是否在集合内
来源：http://qdo.jyoumei.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rym.dianchejie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fpu.cqqwz.cn

JS:   [1, 2, 3].includes(x)
来源：http://mij.hesvh.cn

TS:   [1, 2, 3].includes(x)
来源：http://ttt.jianghu66.top

Java: List.of(1, 2, 3).contains(x)
来源：http://zuy.fanxiaobao.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ydm.gzhubu.top

Ruby: [1, 2, 3].include?(x)
来源：http://ghf.tian-w.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tzu.9152youxi.cn

[B15] 布尔运算与取反
来源：http://qra.chenzaomai.com

Py:   a and b or not c
来源：http://ldn.iojbl.cn

PHP:  $a && $b || !$c
来源：http://pvn.jiagoushi.top

JS:   a && b || !c
来源：http://mne.andypj.xyz

TS:   a && b || !c
来源：http://cks.52xcode.cn

Java: a && b || !c
来源：http://ooh.zdqjudy.top

Go:   a && b || !c
来源：http://kpb.yj202588.top

Ruby: a && b || !c
来源：http://bdx.chenjidiqi.icu

C#:   a && b || !c
来源：http://eqk.xuetiantiany.cn

[B16] 卫语句：不满足条件提前返回
来源：http://etj.zycfv.cn

Py:   if not data: return
来源：http://uor.jinyuanbaomall.cn

PHP:  if (!$data) { return; }
来源：http://ykg.dashuyun.cn

JS:   if (!data) return;
来源：http://hbl.0kj1m.cn

TS:   if (!data) return;
来源：http://dzx.yangfankeji.com

Java: if (data == null) return;
来源：http://dsn.jyoumei.cn

Go:   if data == nil { return }
来源：http://iqr.ehwqpu.com

Ruby: return if data.nil?
来源：http://pkf.zhaomingkeji.xyz

C#:   if (data == null) return;
来源：http://ukf.jinqigfzy.top

================================================================================
来源：http://jec.hywenlv.cn

C. 函数与作用域
来源：http://jbn.ehwqpu.com

================================================================================
来源：http://xfh.shuidangran.top

[C01] 定义函数
来源：http://oox.jinghuilouyu.cn

Py:   def add(a, b): return a + b
来源：http://prc.fengsongda.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mru.ppjwa.cn

JS:   function add(a, b) { return a + b; }
来源：http://sxi.dashuyun.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xau.xuetiantiany.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ftj.ppjwa.cn

Go:   func add(a, b int) int { return a + b }
来源：http://oks.zycfv.cn

Ruby: def add(a, b); a + b; end
来源：http://cuk.jianghu66.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://umu.xinyue.icu

[C02] 默认参数
来源：http://kji.kuanghao11.cn

Py:   def greet(name="World"): return name
来源：http://xyp.ydzc1.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ugz.gaohongyu789.top

JS:   function greet(name = "World") { return name; }
来源：http://nmt.snrcjt.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://odk.tanke756.top

Java: // 无默认参数：方法重载或 Optional
来源：http://nzv.svipenyu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://egx.0kj1m.cn

Ruby: def greet(name = "World") = name
来源：http://fax.jiagoushi.top

C#:   string Greet(string name = "World") => name;
来源：http://brw.sweek.top

[C03] 可变参数
来源：http://tvt.hfpthk.cn

Py:   def total(*args): return sum(args)
来源：http://igs.sxryk.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fhp.zhongyouzk.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jwb.sweek.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zwh.ybcxt.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xjq.pycfn.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ixd.zhaomingkeji.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://okt.birdmap.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jyl.9152youxi.cn

[C04] 命名参数 / 关键字参数
来源：http://ube.zdqjudy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zml.0kj1m.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://avd.nanxinkj.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://sxf.hnxiangtu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dvy.yongpay.top

Java: // 无：用 Builder 模式或 record
来源：http://omz.vqdsnc.cn

Go:   // 无：用配置结构体参数
来源：http://egc.bbcook.cn

Ruby: f(a: 1, b: 2)
来源：http://bxi.gaohongyu789.top

C#:   f(a: 1, b: 2)
来源：http://bvq.shanyushiyangkeji.top

[C05] 返回多个值
来源：http://eqa.yj20258888.top

Py:   return a, b
来源：http://cmw.andypj.xyz

PHP:  return [$a, $b];
来源：http://qtu.316326.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://cap.nanxuanxn.top

TS:   return { a, b };
来源：http://hof.jlsjyb.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://moc.hywenlv.cn

Go:   return a, b
来源：http://gml.fehbvm.com

Ruby: return a, b
来源：http://gzd.xziqi.cn

C#:   return (a, b);              // ValueTuple
来源：http://eiz.pengpengdd.cyou

[C06] 匿名函数 / lambda
来源：http://vhy.sufxvd.cn

Py:   square = lambda x: x * x
来源：http://ttx.cheryme.top

PHP:  $square = fn($x) => $x * $x;
来源：http://uhr.hfpthk.cn

JS:   const square = x => x * x;
来源：http://yum.fzhhl.top

TS:   const square = (x: number): number => x * x;
来源：http://klc.xinyue.icu

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://auw.vqdsnc.cn

Go:   sq := func(x int) int { return x * x }
来源：http://jra.fehbvm.com

Ruby: square = ->(x) { x * x }
来源：http://ztb.guannengcc.top

C#:   Func<int, int> square = x => x * x;
来源：http://dik.tarul.cn

[C07] 把函数作为参数传入
来源：http://klh.feifeiyinyue.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://olv.fengsongda.top

PHP:  array_map("strtoupper", $arr);
来源：http://fky.mhx1999.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ybi.shanyushiyangtech.top

TS:   arr.map(String)
来源：http://iil.jlsjyb.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ujb.52xcode.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bho.yuanzhike.top

Ruby: arr.map(&:upcase)
来源：http://hak.vqdsnc.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://zek.vqdsnc.cn

[C08] 闭包
来源：http://axo.jinqigfzy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dgq.zhiwuduotai.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ixe.fktsv.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gep.ywan-chungtsiang.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wmw.yj20258888.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://oyc.daria6918.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jyd.quarkkingdee.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ove.meibo888.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cfq.meibo888.top

[C09] 递归
来源：http://soy.hesvh.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://djo.zycfv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hqw.fengsongda.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fyo.nanxinkj.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ooe.cdnleiting.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://aly.xuetiantiany.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://abx.ywan-chungtsiang.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ztb.cdnleiting.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://daf.andypj.xyz

[C10] 变量作用域
来源：http://ykd.xuetiantiany.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qqw.zhoulong.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://put.zhiwuduotai.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xgf.epnwcf.com

TS:   同 JS
来源：http://hcn.ybcxt.top

Java: 方法内为块级作用域
来源：http://csj.zhoulong.xyz

Go:   花括号块级作用域
来源：http://ekc.svipenyu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://amw.sjlbkw.cn

C#:   块级作用域
来源：http://vqj.xuetiantiany.cn

[C11] 模块导入与导出
来源：http://lct.cashguo.top

Py:   from module import func
来源：http://lic.zhoulong.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://aby.shuidangran.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://uls.quarkkingdee.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nor.jinqigfzy.top

Java: import java.util.List;
来源：http://bza.guannengcc.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://iwk.ctjpmb.com

Ruby: require "json"; require_relative "./util"
来源：http://pin.zdbjq.cn

C#:   using System.Text;
来源：http://ccc.gaohongyu789.top

[C12] 立即执行函数 IIFE
来源：http://sej.yj20258888.top

Py:   (lambda: print("run"))()
来源：http://tfn.daxiang520.top

PHP:  (function () { echo "run"; })();
来源：http://hyu.shangyingyoupin.top

JS:   (() => { console.log("run"); })();
来源：http://arp.yongpay.top

TS:   (() => { console.log("run"); })();
来源：http://zvz.ydzc1.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ltn.gotoacloud.top

Go:   func() { fmt.Println("run") }()
来源：http://ggv.ctjpmb.com

Ruby: -> { puts "run" }.call
来源：http://lsk.vqdsnc.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://cqs.wangdashe.top

[C13] 类型声明 / 类型注解
来源：http://vji.sysykeji.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jsv.yvedp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lpd.jlsjyb.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://djz.zhaomingkeji.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://djj.yuxming.cn

Java: int add(int a, int b) { return a + b; }
来源：http://dii.nanxuanxn.top

Go:   func add(a, b int) int
来源：http://ezr.hysaishi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cxl.tian-w.cn

C#:   int Add(int a, int b) => a + b;
来源：http://zkn.zhijiandao.cn

[C14] 泛型函数
来源：http://ezu.gaohongyu789.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hib.feifeiyinyue.top

PHP:  // 无泛型
来源：http://npa.wangdashe.top

JS:   // 无泛型
来源：http://wdm.sxryk.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ied.316326.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wcu.chenzaomai.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://sxd.cheryme.top

Ruby: # 无泛型
来源：http://zac.gogol.net.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xjw.yvedp.cn

[C15] 解构 / 展开参数
来源：http://aym.tian-w.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cqx.jqgufenzy.top

PHP:  [$a, $b] = $pair;
来源：http://lop.xinyue.icu

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hxz.jqgfzy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hwn.yuxming.cn

Java: // 无解构
来源：http://unp.shanyushiyangkeji.top

Go:   // 无解构
来源：http://xzq.guowangkeji.top

Ruby: a, b = pair
来源：http://vlv.guowangkeji.top

C#:   var (a, b) = pair;
来源：http://wtm.yanxiufei.cn

[C16] 函数 / 方法重载
来源：http://mfd.chenlongwang.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://npg.bbcook.cn

PHP:  // 无重载
来源：http://sqg.ywan-chungtsiang.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ive.jinyuanbaomall.cn

TS:   // 用联合类型或重载签名声明
来源：http://fcg.0kj1m.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://zvx.cheryme.top

Go:   // 无重载：用不同函数名
来源：http://pvj.jlsjyb.cn

Ruby: # 无重载：靠动态参数
来源：http://vei.daria6918.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://evl.smart0.xyz

================================================================================
来源：http://cvh.vehdjk.com

D. 数组 / 列表 / 集合
来源：http://skq.vehdjk.com

================================================================================
来源：http://vnc.yonumen.top

[D01] 创建数组 / 列表
来源：http://sje.bjfxy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://qbz.haohaochexian.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vba.daxiang520.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xdz.yj20258.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://mai.hnqzz.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xnn.hfpthk.cn

Go:   arr := []int{1, 2, 3}
来源：http://knv.hongshengwenyu.top

Ruby: arr = [1, 2, 3]
来源：http://dvk.zhongyouzk.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lro.haohaochexian.top

[D02] 追加元素到末尾
来源：http://pgb.yanxiufei.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hgt.mhx1999.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ndj.svipenyu.cn

JS:   arr.push(4);
来源：http://vci.gotoacloud.top

TS:   arr.push(4);
来源：http://djg.kuanghao11.cn

Java: list.add(4);
来源：http://ptb.sufxvd.cn

Go:   arr = append(arr, 4)
来源：http://zkx.meibo888.top

Ruby: arr << 4; arr.push(5)
来源：http://zqb.zhijiandao.cn

C#:   list.Add(4);
来源：http://vvz.sjlbkw.cn

[D03] 在指定位置插入元素
来源：http://zwr.daria6918.cn

Py:   arr.insert(0, 0)
来源：http://htd.dashuyun.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fcv.ywan-chungtsiang.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tfr.fengsongda.top

TS:   arr.splice(0, 0, 0);
来源：http://lra.yuanzhike.top

Java: list.add(0, 0);
来源：http://agn.snrcjt.cn

Go:   arr = append([]int{0}, arr...)
来源：http://mxh.bbcook.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://whq.fanxiaobao.xyz

C#:   list.Insert(0, 0);
来源：http://qfk.shuidangran.top

[D04] 删除元素
来源：http://dcy.tianlin.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rcx.hfpthk.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bez.tian-w.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vdn.tarul.cn

TS:   arr.splice(0, 1);
来源：http://efq.gzhubu.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://eeg.shanyushiyangtech.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kda.jyoumei.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vkf.yj202588.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wxp.xinyue.icu

[D05] 访问与修改元素
来源：http://fch.tian-w.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://oou.daxiang520.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fie.mhx1999.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vne.pengpengdd.cyou

TS:   arr[0]; arr.at(-1);
来源：http://her.quarkkingdee.top

Java: list.get(0); list.set(0, 9);
来源：http://xyg.ivvv.top

Go:   arr[0]; arr[0] = 9
来源：http://uif.wangshuangyany.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ggs.dianchejie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://sps.aizwys.cn

[D06] 数组长度
来源：http://brs.aibaodan.cn

Py:   len(arr)
来源：http://woz.epnwcf.com

PHP:  count($arr);
来源：http://bkf.aizwys.cn

JS:   arr.length
来源：http://fjc.haohaochexian.top

TS:   arr.length
来源：http://sev.zhongyouzk.top

Java: list.size();
来源：http://iah.svipenyu.cn

Go:   len(arr)
来源：http://gvi.guowangkeji.top

Ruby: arr.length; arr.size
来源：http://kxr.jqgufenzy.top

C#:   list.Count;
来源：http://wnc.xingfuxueyuan.xyz

[D07] 切片 / 取子数组
来源：http://lyv.hywenlv.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fou.nanxuanxn.top

PHP:  array_slice($arr, 1, 3);
来源：http://lqo.daria6918.cn

JS:   arr.slice(1, 4);
来源：http://myw.chenlongwang.top

TS:   arr.slice(1, 4);
来源：http://gai.wangshuangyany.cn

Java: list.subList(1, 4);
来源：http://wtk.0kj1m.cn

Go:   arr[1:4]
来源：http://tcz.kuanghao11.cn

Ruby: arr[1, 3]
来源：http://vqw.zhixingplan.top

C#:   list.GetRange(1, 3);
来源：http://fjc.hammf.cn

[D08] 合并两个数组
来源：http://ccm.aizwys.cn

Py:   a + b;  a.extend(b)
来源：http://tfk.zhiwuduotai.top

PHP:  array_merge($a, $b);
来源：http://xyy.hesvh.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://xph.zhiwuduotai.top

TS:   [...a, ...b];
来源：http://rix.yongpay.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://eta.nanxinkj.top

Go:   append(a, b...)
来源：http://azt.sjlbkw.cn

Ruby: a + b;  a.concat(b)
来源：http://dwr.kuanghao11.cn

C#:   a.Concat(b).ToList()
来源：http://urr.tian-w.cn

[D09] 排序（升序）
来源：http://jmo.gotoacloud.top

Py:   sorted(arr);  arr.sort()
来源：http://qed.fzhhl.top

PHP:  sort($arr);
来源：http://prg.nanxuanxn.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vja.iojbl.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ojz.fanxiaobao.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://kzu.hywenlv.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://njp.sxryk.cn

Ruby: arr.sort
来源：http://pup.jinqigfzy.top

C#:   list.Sort();
来源：http://rej.zycfv.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ngj.yueranfly.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yet.nanxinkj.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jhr.dashuyun.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://drw.xuetiantiany.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://chq.mhx1999.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qvz.sweek.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cwr.fktsv.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kwc.hfpthk.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bjp.nwbrower.top

[D11] 反转数组
来源：http://tnh.tanke756.top

Py:   arr[::-1];  arr.reverse()
来源：http://wrb.jiagoushi.top

PHP:  array_reverse($arr);
来源：http://abs.shanyushiyangtech.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ake.shanyushiyangkeji.top

TS:   [...arr].reverse();
来源：http://tom.yuxming.cn

Java: Collections.reverse(list);
来源：http://yfs.jiagoushi.top

Go:   slices.Reverse(arr)
来源：http://rxj.9152youxi.cn

Ruby: arr.reverse
来源：http://woh.quarkkingdee.top

C#:   list.Reverse();
来源：http://zga.gogol.net.cn

[D12] 查找元素下标
来源：http://vnf.fzhhl.top

Py:   arr.index(x);  x in arr
来源：http://cae.jlsjyb.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gld.fktsv.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ocm.hcnkem.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mov.yanxiufei.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bbe.nwbrower.top

Go:   slices.Index(arr, x)
来源：http://zxi.xinyue.icu

Ruby: arr.index(x)
来源：http://nch.bjfxy.top

C#:   list.IndexOf(x);
来源：http://wpo.hywenlv.cn

[D13] 过滤（保留满足条件的）
来源：http://baz.shzxlz.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hng.jqgufenzy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://elb.sjlbkw.cn

JS:   arr.filter(x => x > 3)
来源：http://cyg.chenlongwang.top

TS:   arr.filter(x => x > 3)
来源：http://blr.haohaochexian.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vjz.redwolf501.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://sax.fanxiaobao.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://bmd.yanxiufei.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://mbb.aizwys.cn

[D14] 映射转换（每个元素变形）
来源：http://qeg.hongshengwenyu.top


<!-- 参考信息 -->