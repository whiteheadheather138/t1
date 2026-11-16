代发 wailian999

================================================================================
来源：http://dnu.wangdashe.top

C. 函数与作用域
来源：http://svv.gzhubu.top

================================================================================
来源：http://utm.zhoulong.xyz

[C01] 定义函数
来源：http://jjq.yj20258.top

Py:   def add(a, b): return a + b
来源：http://vna.jyoumei.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gyj.zdbjq.cn

JS:   function add(a, b) { return a + b; }
来源：http://vup.zdqjudy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ugl.pengpengdd.cyou

Java: static int add(int a, int b) { return a + b; }
来源：http://dxv.zdbjq.cn

Go:   func add(a, b int) int { return a + b }
来源：http://bqz.shanyushiyangkeji.top

Ruby: def add(a, b); a + b; end
来源：http://iyz.jinqigufen.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pda.hnqzz.top

[C02] 默认参数
来源：http://cji.ydzc1.top

Py:   def greet(name="World"): return name
来源：http://ljg.yj202588.top

PHP:  function greet($name = "World") { return $name; }
来源：http://mwh.fzhhl.top

JS:   function greet(name = "World") { return name; }
来源：http://hck.haohaochexian.top

TS:   function greet(name: string = "World") { return name; }
来源：http://mrn.ppjwa.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://tvl.tianlin.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://uzx.yfazqb.com

Ruby: def greet(name = "World") = name
来源：http://xfi.hysaishi.cn

C#:   string Greet(string name = "World") => name;
来源：http://zsh.chenlongwang.top

[C03] 可变参数
来源：http://iaz.wangshuangyany.cn

Py:   def total(*args): return sum(args)
来源：http://hjv.hnqzz.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xoy.jqgufenzy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gzd.smart0.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fqg.yvedp.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kjx.jianghu66.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bzx.ybcxt.top

Ruby: def total(*nums); nums.sum; end
来源：http://ble.zhaomingkeji.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qkp.hnqzz.top

[C04] 命名参数 / 关键字参数
来源：http://fok.chenlongwang.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cjr.chenjidiqi.icu

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jow.daxiang520.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cez.haohaochexian.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hxa.guannengcc.top

Java: // 无：用 Builder 模式或 record
来源：http://wop.ehwqpu.com

Go:   // 无：用配置结构体参数
来源：http://jsn.pycfn.com

Ruby: f(a: 1, b: 2)
来源：http://zqu.wangdashe.top

C#:   f(a: 1, b: 2)
来源：http://tdn.zhijiandao.cn

[C05] 返回多个值
来源：http://ohy.c1oappe.top

Py:   return a, b
来源：http://cck.ywan-chungtsiang.top

PHP:  return [$a, $b];
来源：http://vos.nwbrower.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://rem.zhiwuduotai.top

TS:   return { a, b };
来源：http://igs.xziqi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://awy.wangdashe.top

Go:   return a, b
来源：http://wxb.yangfankeji.com

Ruby: return a, b
来源：http://vaj.xingfuxueyuan.xyz

C#:   return (a, b);              // ValueTuple
来源：http://llh.aibaodan.cn

[C06] 匿名函数 / lambda
来源：http://sdn.nwbrower.top

Py:   square = lambda x: x * x
来源：http://pip.9152youxi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://kqs.iojbl.cn

JS:   const square = x => x * x;
来源：http://ceq.yanxiufei.cn

TS:   const square = (x: number): number => x * x;
来源：http://xba.cucudq.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qkl.hnqzz.top

Go:   sq := func(x int) int { return x * x }
来源：http://hho.xziqi.cn

Ruby: square = ->(x) { x * x }
来源：http://moi.zdqjudy.top

C#:   Func<int, int> square = x => x * x;
来源：http://vkd.shzxlz.cn

[C07] 把函数作为参数传入
来源：http://mfb.sjlbkw.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://koj.shzxlz.cn

PHP:  array_map("strtoupper", $arr);
来源：http://npe.uphjek.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://whw.kuanghao11.cn

TS:   arr.map(String)
来源：http://ore.birdmap.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tbo.c1oappe.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mkz.yongpay.top

Ruby: arr.map(&:upcase)
来源：http://djo.cheryme.top

C#:   arr.Select(s => s.ToUpper())
来源：http://lpf.jinghuilouyu.cn

[C08] 闭包
来源：http://wxg.jianghu66.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nmm.yj20258888.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rgx.52xcode.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ulj.bbcook.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qeg.aibaodan.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xac.jiagoushi.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jlz.ywan-chungtsiang.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://loo.316326.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lqw.hammf.cn

[C09] 递归
来源：http://vly.nanxinkj.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://azg.redwolf501.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ota.sxryk.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ttg.wangshuangyany.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://efy.ydjk.org.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jvu.jqgfzy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mnp.quarkkingdee.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kvo.aizwys.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dtz.yongpay.top

[C10] 变量作用域
来源：http://knj.yuanzhike.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lea.daxiang520.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kzk.chenjidiqi.icu

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gxt.316326.xyz

TS:   同 JS
来源：http://set.cheryme.top

Java: 方法内为块级作用域
来源：http://jnb.ehwqpu.com

Go:   花括号块级作用域
来源：http://zsf.aizwys.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wcn.zhoulong.xyz

C#:   块级作用域
来源：http://ffd.vqdsnc.cn

[C11] 模块导入与导出
来源：http://txf.jlsjyb.cn

Py:   from module import func
来源：http://uea.hammf.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://kwk.bbcook.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://xhi.gaohongyu789.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ati.yangfankeji.com

Java: import java.util.List;
来源：http://xll.snrcjt.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kwd.fengsongda.top

Ruby: require "json"; require_relative "./util"
来源：http://old.aizwys.cn

C#:   using System.Text;
来源：http://slz.guannengcc.top

[C12] 立即执行函数 IIFE
来源：http://stz.jinqigufen.top

Py:   (lambda: print("run"))()
来源：http://lph.yvedp.cn

PHP:  (function () { echo "run"; })();
来源：http://jsw.ehwqpu.com

JS:   (() => { console.log("run"); })();
来源：http://wxc.gotoacloud.top

TS:   (() => { console.log("run"); })();
来源：http://khl.aibaodan.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gah.andypj.xyz

Go:   func() { fmt.Println("run") }()
来源：http://uyq.jianghu66.top

Ruby: -> { puts "run" }.call
来源：http://mlc.hnxiangtu.top

C#:   // 无 IIFE：用静态构造函数
来源：http://sce.chenlongwang.top

[C13] 类型声明 / 类型注解
来源：http://vvo.tanke756.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dhj.ivvv.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://slc.yj20258888.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://aex.chenzaomai.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://iwg.svipenyu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://gpy.chenlongwang.top

Go:   func add(a, b int) int
来源：http://vga.hysaishi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vsl.sjlbkw.cn

C#:   int Add(int a, int b) => a + b;
来源：http://jpw.zhijiandao.cn

[C14] 泛型函数
来源：http://oto.jinyuanbaomall.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lxb.wangshuangyany.cn

PHP:  // 无泛型
来源：http://qvk.nwbrower.top

JS:   // 无泛型
来源：http://cke.hammf.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zor.zdbjq.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://and.hcnkem.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rye.zdbjq.cn

Ruby: # 无泛型
来源：http://fif.shanyushiyangtech.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vog.zhiwuduotai.top

[C15] 解构 / 展开参数
来源：http://qpv.9152youxi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ptn.yuanzhike.top

PHP:  [$a, $b] = $pair;
来源：http://hop.daria6918.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qqn.hywenlv.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qli.ywan-chungtsiang.top

Java: // 无解构
来源：http://wif.dashuyun.cn

Go:   // 无解构
来源：http://far.hcnkem.com

Ruby: a, b = pair
来源：http://ffz.jqgfzy.top

C#:   var (a, b) = pair;
来源：http://eio.cqqwz.cn

[C16] 函数 / 方法重载
来源：http://gkt.dashuyun.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://lfd.dashuyun.cn

PHP:  // 无重载
来源：http://nku.fengsongda.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://jcs.ywan-chungtsiang.top

TS:   // 用联合类型或重载签名声明
来源：http://eih.sxryk.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://zjh.nanxinkj.top

Go:   // 无重载：用不同函数名
来源：http://pop.sufxvd.cn

Ruby: # 无重载：靠动态参数
来源：http://wxq.bjfxy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://uao.vehdjk.com

================================================================================
来源：http://air.sysykeji.top

D. 数组 / 列表 / 集合
来源：http://tuq.316326.xyz

================================================================================
来源：http://aio.guannengcc.top

[D01] 创建数组 / 列表
来源：http://ipe.nwbrower.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://aef.gogol.net.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ene.jqgufenzy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://egm.ehwqpu.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://wtp.dashuyun.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://huf.shuidangran.top

Go:   arr := []int{1, 2, 3}
来源：http://eqw.jlsjyb.cn

Ruby: arr = [1, 2, 3]
来源：http://oez.xuanzx.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zyh.gogol.net.cn

[D02] 追加元素到末尾
来源：http://lve.jqgufenzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fcb.pycfn.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xhi.hywenlv.cn

JS:   arr.push(4);
来源：http://uoj.aibaodan.cn

TS:   arr.push(4);
来源：http://qhj.gogol.net.cn

Java: list.add(4);
来源：http://mgm.daria6918.cn

Go:   arr = append(arr, 4)
来源：http://zop.cashguo.top

Ruby: arr << 4; arr.push(5)
来源：http://nwx.nanxuanxn.top

C#:   list.Add(4);
来源：http://kea.sweek.top

[D03] 在指定位置插入元素
来源：http://yqq.jyoumei.cn

Py:   arr.insert(0, 0)
来源：http://klw.aizwys.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lqd.cashguo.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rpg.chenzaomai.com

TS:   arr.splice(0, 0, 0);
来源：http://him.aizwys.cn

Java: list.add(0, 0);
来源：http://fmr.wangdashe.top

Go:   arr = append([]int{0}, arr...)
来源：http://rqz.ydzc1.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jtt.jqgufenzy.top

C#:   list.Insert(0, 0);
来源：http://mcy.gzhubu.top

[D04] 删除元素
来源：http://jiz.gotoacloud.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rkn.0kj1m.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://toc.jinqigfzy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hmn.sjlbkw.cn

TS:   arr.splice(0, 1);
来源：http://wne.yonumen.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dnq.316326.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://oup.yj20258.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://chd.cqqwz.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ixq.mhx1999.top

[D05] 访问与修改元素
来源：http://xlp.pycfn.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xnb.epnwcf.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sxu.feifeiyinyue.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wzq.iojbl.cn

TS:   arr[0]; arr.at(-1);
来源：http://tbc.redwolf501.top

Java: list.get(0); list.set(0, 9);
来源：http://bqa.snrcjt.cn

Go:   arr[0]; arr[0] = 9
来源：http://cco.yuanzhike.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qat.jinyuanbaomall.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://eyb.shuidangran.top

[D06] 数组长度
来源：http://qjz.gogol.net.cn

Py:   len(arr)
来源：http://tvn.shangyingyoupin.top

PHP:  count($arr);
来源：http://yxb.fanxiaobao.xyz

JS:   arr.length
来源：http://hvb.tarul.cn

TS:   arr.length
来源：http://svb.xziqi.cn

Java: list.size();
来源：http://xbv.9152youxi.cn

Go:   len(arr)
来源：http://lqq.yuanzhike.top

Ruby: arr.length; arr.size
来源：http://huv.fehbvm.com

C#:   list.Count;
来源：http://ati.yvedp.cn

[D07] 切片 / 取子数组
来源：http://jzu.sweek.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cjl.uphjek.com

PHP:  array_slice($arr, 1, 3);
来源：http://jcq.hesvh.cn

JS:   arr.slice(1, 4);
来源：http://ywu.kuanghao11.cn

TS:   arr.slice(1, 4);
来源：http://rmj.yanxiufei.cn

Java: list.subList(1, 4);
来源：http://dkj.c1oappe.top

Go:   arr[1:4]
来源：http://tjg.tian-w.cn

Ruby: arr[1, 3]
来源：http://kaz.redwolf501.top

C#:   list.GetRange(1, 3);
来源：http://aeb.epnwcf.com

[D08] 合并两个数组
来源：http://rmx.gotoacloud.top

Py:   a + b;  a.extend(b)
来源：http://sxp.hnxiangtu.top

PHP:  array_merge($a, $b);
来源：http://lft.haohaochexian.top

JS:   [...a, ...b];  a.concat(b);
来源：http://wdu.dianchejie.cn

TS:   [...a, ...b];
来源：http://fzf.52xcode.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dma.hesvh.cn

Go:   append(a, b...)
来源：http://pfv.jlsjyb.cn

Ruby: a + b;  a.concat(b)
来源：http://hyf.birdmap.top

C#:   a.Concat(b).ToList()
来源：http://xzs.fengsongda.top

[D09] 排序（升序）
来源：http://btf.pengpengdd.cyou

Py:   sorted(arr);  arr.sort()
来源：http://bus.c1oappe.top

PHP:  sort($arr);
来源：http://jzp.dashuyun.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yoj.svipenyu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://lnz.fengsongda.top

Java: Collections.sort(list);  list.sort(null);
来源：http://goa.hongshengwenyu.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qsj.tianlin.xyz

Ruby: arr.sort
来源：http://ukh.aizwys.cn

C#:   list.Sort();
来源：http://ims.zhaomingkeji.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://mez.52xcode.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yee.ivvv.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://liy.gogol.net.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jld.fzhhl.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://sbi.cqqwz.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://htu.hnxiangtu.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dds.gogol.net.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vif.nanxuanxn.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ond.xuetiantiany.cn

[D11] 反转数组
来源：http://kqj.vqdsnc.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qoc.wangshuangyany.cn

PHP:  array_reverse($arr);
来源：http://dvy.jyoumei.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mis.gogol.net.cn

TS:   [...arr].reverse();
来源：http://ifv.yangfankeji.com

Java: Collections.reverse(list);
来源：http://zgl.yj202588.top

Go:   slices.Reverse(arr)
来源：http://eqv.meibo888.top

Ruby: arr.reverse
来源：http://crp.chenlongwang.top

C#:   list.Reverse();
来源：http://xvj.316326.xyz

[D12] 查找元素下标
来源：http://whf.sysykeji.top

Py:   arr.index(x);  x in arr
来源：http://dzg.hongshengwenyu.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cnh.sxryk.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qap.shanyushiyangtech.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tgn.fengsongda.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rcz.c1oappe.top

Go:   slices.Index(arr, x)
来源：http://qgz.hnxiangtu.top

Ruby: arr.index(x)
来源：http://wnr.yueranfly.top

C#:   list.IndexOf(x);
来源：http://giz.daxiang520.top

[D13] 过滤（保留满足条件的）
来源：http://dqe.nanxuanxn.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://awx.hywenlv.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kly.xinyue.icu

JS:   arr.filter(x => x > 3)
来源：http://deb.zdbjq.cn

TS:   arr.filter(x => x > 3)
来源：http://nck.epnwcf.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ipf.epnwcf.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://sjo.yj20258888.top

Ruby: arr.select { |x| x > 3 }
来源：http://fuh.fengsongda.top

C#:   list.Where(x => x > 3).ToList()
来源：http://kpi.xziqi.cn

[D14] 映射转换（每个元素变形）
来源：http://otu.gzhubu.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qct.hcnkem.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://oqx.shanyushiyangtech.top

JS:   arr.map(x => x * 2)
来源：http://nxj.hfpthk.cn

TS:   arr.map(x => x * 2)
来源：http://sdh.shzxlz.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://lct.hysaishi.cn

Go:   // 手写循环
来源：http://anb.jianghu66.top

Ruby: arr.map { |x| x * 2 }
来源：http://taj.svipenyu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://nsk.sweek.top

[D15] 去重
来源：http://eoi.zycfv.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dbt.zhaomingkeji.xyz

PHP:  array_unique($arr);
来源：http://pby.gaohongyu789.top

JS:   [...new Set(arr)]
来源：http://lbn.bbcook.cn

TS:   [...new Set(arr)]
来源：http://ywk.svipenyu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rsb.ybcxt.top

Go:   // 用 map[T]struct{} 手写
来源：http://znu.redwolf501.top

Ruby: arr.uniq
来源：http://pyh.iojbl.cn

C#:   list.Distinct().ToList()
来源：http://swi.zhongyouzk.top

[D16] 求和与平均值
来源：http://axv.hesvh.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://txi.haohaochexian.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bet.aibaodan.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://aeb.chenlongwang.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qzr.kuanghao11.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vpu.epnwcf.com

Go:   // 手写循环累加
来源：http://tgx.hywenlv.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jxl.dianchejie.cn

C#:   list.Sum();  list.Average()
来源：http://sbu.xziqi.cn

[D17] 最大值与最小值
来源：http://cuf.tian-w.cn

Py:   max(arr);  min(arr)
来源：http://mzj.hongshengwenyu.top

PHP:  max($arr);  min($arr);
来源：http://qnw.xingfuxueyuan.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lae.jlsjyb.cn

TS:   Math.max(...arr);
来源：http://rlv.hfpthk.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mhj.yj202588.top


<!-- 参考信息 -->