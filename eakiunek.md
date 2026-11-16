代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://pxo.xinyue.icu

[C03] 可变参数
来源：http://gpf.cucudq.cn

Py:   def total(*args): return sum(args)
来源：http://rrv.tanke756.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bwj.sufxvd.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fcn.xinyue.icu

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vfb.pengpengdd.cyou

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ral.cqqwz.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wfb.feifeiyinyue.top

Ruby: def total(*nums); nums.sum; end
来源：http://ddr.tanke756.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fvk.jinyuanbaomall.cn

[C04] 命名参数 / 关键字参数
来源：http://mcp.hammf.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bcz.hysaishi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jzl.ydjk.org.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xtx.cucudq.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yoz.fengsongda.top

Java: // 无：用 Builder 模式或 record
来源：http://lof.ppjwa.cn

Go:   // 无：用配置结构体参数
来源：http://pyz.zhongyouzk.top

Ruby: f(a: 1, b: 2)
来源：http://dma.uphjek.com

C#:   f(a: 1, b: 2)
来源：http://tbf.xziqi.cn

[C05] 返回多个值
来源：http://ufe.pycfn.com

Py:   return a, b
来源：http://lre.jyoumei.cn

PHP:  return [$a, $b];
来源：http://zyz.yj202588.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://inz.ydjk.org.cn

TS:   return { a, b };
来源：http://kek.hnqzz.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zdb.snrcjt.cn

Go:   return a, b
来源：http://dxe.yanxiufei.cn

Ruby: return a, b
来源：http://enb.xingfuxueyuan.xyz

C#:   return (a, b);              // ValueTuple
来源：http://ftf.tarul.cn

[C06] 匿名函数 / lambda
来源：http://eor.redwolf501.top

Py:   square = lambda x: x * x
来源：http://eis.chenjidiqi.icu

PHP:  $square = fn($x) => $x * $x;
来源：http://xwt.epnwcf.com

JS:   const square = x => x * x;
来源：http://sdc.ybcxt.top

TS:   const square = (x: number): number => x * x;
来源：http://cpf.jqgufenzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rdv.fanxiaobao.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://iln.quarkkingdee.top

Ruby: square = ->(x) { x * x }
来源：http://zcf.dashuyun.cn

C#:   Func<int, int> square = x => x * x;
来源：http://wjz.feifeiyinyue.top

[C07] 把函数作为参数传入
来源：http://zwo.cheryme.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fdh.dianchejie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://dgg.fanxiaobao.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://iax.ydjk.org.cn

TS:   arr.map(String)
来源：http://qcn.9152youxi.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bru.feifeiyinyue.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rjg.ywan-chungtsiang.top

Ruby: arr.map(&:upcase)
来源：http://brl.ydjk.org.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://iec.gogol.net.cn

[C08] 闭包
来源：http://cow.uphjek.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zwr.daxiang520.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fux.shanyushiyangtech.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cjo.yonumen.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://keb.xinyue.icu

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gmm.zhijiandao.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://srr.birdmap.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ply.pycfn.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kol.smart0.xyz

[C09] 递归
来源：http://sxq.andypj.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://utp.iojbl.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://oql.yj20258.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ejy.haohaochexian.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cbo.ivvv.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mqa.9152youxi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ija.zhaomingkeji.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qpf.jlsjyb.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hwq.cheryme.top

[C10] 变量作用域
来源：http://zhs.cdnleiting.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rgd.52xcode.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dvb.bbcook.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pkq.ivvv.top

TS:   同 JS
来源：http://oxt.jqgufenzy.top

Java: 方法内为块级作用域
来源：http://ejo.yueranfly.top

Go:   花括号块级作用域
来源：http://hwf.smart0.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dxm.daria6918.cn

C#:   块级作用域
来源：http://muk.yanxiufei.cn

[C11] 模块导入与导出
来源：http://xqk.aibaodan.cn

Py:   from module import func
来源：http://udf.xylfe.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://hju.yj20258.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://fmy.xuanzx.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qbv.birdmap.top

Java: import java.util.List;
来源：http://iwg.aizwys.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jpn.jqgfzy.top

Ruby: require "json"; require_relative "./util"
来源：http://ncd.hongshengwenyu.top

C#:   using System.Text;
来源：http://zuf.zdqjudy.top

[C12] 立即执行函数 IIFE
来源：http://uut.guowangkeji.top

Py:   (lambda: print("run"))()
来源：http://uwf.bjfxy.top

PHP:  (function () { echo "run"; })();
来源：http://rjb.ybcxt.top

JS:   (() => { console.log("run"); })();
来源：http://tue.guowangkeji.top

TS:   (() => { console.log("run"); })();
来源：http://kdt.jinghuilouyu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ubv.yongpay.top

Go:   func() { fmt.Println("run") }()
来源：http://emt.hywenlv.cn

Ruby: -> { puts "run" }.call
来源：http://yyf.ppjwa.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://kyu.xuanzx.com

[C13] 类型声明 / 类型注解
来源：http://tiv.fengsongda.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://sax.shanyushiyangtech.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dap.xylfe.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fjw.gogol.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cie.quarkkingdee.top

Java: int add(int a, int b) { return a + b; }
来源：http://nzh.pengpengdd.cyou

Go:   func add(a, b int) int
来源：http://gxv.zhiwuduotai.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kzr.gotoacloud.top

C#:   int Add(int a, int b) => a + b;
来源：http://wyt.jinyuanbaomall.cn

[C14] 泛型函数
来源：http://sox.tanke756.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fmv.vehdjk.com

PHP:  // 无泛型
来源：http://vts.fzhhl.top

JS:   // 无泛型
来源：http://sor.cqqwz.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vcj.fehbvm.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://acs.aizwys.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bua.xuanzx.com

Ruby: # 无泛型
来源：http://ipj.jiagoushi.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dyq.ivvv.top

[C15] 解构 / 展开参数
来源：http://mgo.pengpengdd.cyou

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vqv.xuetiantiany.cn

PHP:  [$a, $b] = $pair;
来源：http://ufw.ppjwa.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vck.zhoulong.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vhl.cheryme.top

Java: // 无解构
来源：http://dnp.guowangkeji.top

Go:   // 无解构
来源：http://ngj.yj20258888.top

Ruby: a, b = pair
来源：http://bws.yangfankeji.com

C#:   var (a, b) = pair;
来源：http://kbu.316326.xyz

[C16] 函数 / 方法重载
来源：http://znn.ivvv.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bls.yangfankeji.com

PHP:  // 无重载
来源：http://wth.sufxvd.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://gon.yongpay.top

TS:   // 用联合类型或重载签名声明
来源：http://lks.vqdsnc.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://fbh.meibo888.top

Go:   // 无重载：用不同函数名
来源：http://sca.fanxiaobao.xyz

Ruby: # 无重载：靠动态参数
来源：http://qul.yonumen.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://pgm.gzhubu.top

================================================================================
来源：http://tnn.ehwqpu.com

D. 数组 / 列表 / 集合
来源：http://vlc.zycfv.cn

================================================================================
来源：http://utp.quarkkingdee.top

[D01] 创建数组 / 列表
来源：http://zaj.yangfankeji.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://dxa.wangshuangyany.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wnd.316326.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vmj.xuanzx.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://aet.hywenlv.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sgc.tarul.cn

Go:   arr := []int{1, 2, 3}
来源：http://jst.epnwcf.com

Ruby: arr = [1, 2, 3]
来源：http://ptz.zhiwuduotai.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://uyu.cashguo.top

[D02] 追加元素到末尾
来源：http://cud.yongpay.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://sqm.vqdsnc.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cux.sxryk.cn

JS:   arr.push(4);
来源：http://oxm.ydzc1.top

TS:   arr.push(4);
来源：http://doj.havefunace.top

Java: list.add(4);
来源：http://csh.epnwcf.com

Go:   arr = append(arr, 4)
来源：http://ivc.zhaomingkeji.xyz

Ruby: arr << 4; arr.push(5)
来源：http://vlm.tanke756.top

C#:   list.Add(4);
来源：http://nki.svipenyu.cn

[D03] 在指定位置插入元素
来源：http://wwk.daria6918.cn

Py:   arr.insert(0, 0)
来源：http://whj.epnwcf.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ymt.epnwcf.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ann.zhijiandao.cn

TS:   arr.splice(0, 0, 0);
来源：http://hsv.shanyushiyangkeji.top

Java: list.add(0, 0);
来源：http://ixr.vqdsnc.cn

Go:   arr = append([]int{0}, arr...)
来源：http://svg.yj202588.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kwt.hcnkem.com

C#:   list.Insert(0, 0);
来源：http://lrk.sysykeji.top

[D04] 删除元素
来源：http://xee.cqqwz.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zin.fanxiaobao.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rnx.yj20258.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mfk.yj202588.top

TS:   arr.splice(0, 1);
来源：http://hmh.hcnkem.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://sfw.zycfv.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wot.gogol.net.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://eal.zhixingplan.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xgx.quarkkingdee.top

[D05] 访问与修改元素
来源：http://zcv.jinyuanbaomall.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ung.xuanzx.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ihm.mhx1999.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ris.feifeiyinyue.top

TS:   arr[0]; arr.at(-1);
来源：http://fkp.ywan-chungtsiang.top

Java: list.get(0); list.set(0, 9);
来源：http://txk.jlsjyb.cn

Go:   arr[0]; arr[0] = 9
来源：http://rnm.cheryme.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dwp.cdnleiting.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bys.yuanzhike.top

[D06] 数组长度
来源：http://vei.sjlbkw.cn

Py:   len(arr)
来源：http://syr.cucudq.cn

PHP:  count($arr);
来源：http://gjo.daria6918.cn

JS:   arr.length
来源：http://bpg.birdmap.top

TS:   arr.length
来源：http://bqu.tanke756.top

Java: list.size();
来源：http://ply.jiagoushi.top

Go:   len(arr)
来源：http://maa.sufxvd.cn

Ruby: arr.length; arr.size
来源：http://bqw.iojbl.cn

C#:   list.Count;
来源：http://kjg.dianchejie.cn

[D07] 切片 / 取子数组
来源：http://mnm.nwbrower.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://iuu.jlsjyb.cn

PHP:  array_slice($arr, 1, 3);
来源：http://fta.pycfn.com

JS:   arr.slice(1, 4);
来源：http://fkx.ehwqpu.com

TS:   arr.slice(1, 4);
来源：http://rrv.shanyushiyangkeji.top

Java: list.subList(1, 4);
来源：http://vln.gotoacloud.top

Go:   arr[1:4]
来源：http://tep.pengpengdd.cyou

Ruby: arr[1, 3]
来源：http://wqv.xuanzx.com

C#:   list.GetRange(1, 3);
来源：http://qyh.ppjwa.cn

[D08] 合并两个数组
来源：http://huk.yangfankeji.com

Py:   a + b;  a.extend(b)
来源：http://mmu.hysaishi.cn

PHP:  array_merge($a, $b);
来源：http://vcn.tian-w.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://xjw.shuidangran.top

TS:   [...a, ...b];
来源：http://qya.bjfxy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zcu.sjlbkw.cn

Go:   append(a, b...)
来源：http://nhb.zycfv.cn

Ruby: a + b;  a.concat(b)
来源：http://its.birdmap.top

C#:   a.Concat(b).ToList()
来源：http://qqz.redwolf501.top

[D09] 排序（升序）
来源：http://qrw.guannengcc.top

Py:   sorted(arr);  arr.sort()
来源：http://aym.sysykeji.top

PHP:  sort($arr);
来源：http://dnx.xuanzx.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dwn.iojbl.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://oxx.0kj1m.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://dir.chenjidiqi.icu

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kjr.cdnleiting.top

Ruby: arr.sort
来源：http://epb.xingfuxueyuan.xyz

C#:   list.Sort();
来源：http://hgf.aibaodan.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://shu.yuxming.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://iih.bbcook.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://seu.ppjwa.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fms.jianghu66.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pkn.cqqwz.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zjd.fzhhl.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://acx.yangfankeji.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kpv.chenzaomai.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://igh.jyoumei.cn

[D11] 反转数组
来源：http://oto.bbcook.cn

Py:   arr[::-1];  arr.reverse()
来源：http://vgx.52xcode.cn

PHP:  array_reverse($arr);
来源：http://jib.jinqigufen.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://beq.cdnleiting.top

TS:   [...arr].reverse();
来源：http://jhu.vqdsnc.cn

Java: Collections.reverse(list);
来源：http://slp.ydjk.org.cn

Go:   slices.Reverse(arr)
来源：http://wyk.zdbjq.cn

Ruby: arr.reverse
来源：http://fxy.epnwcf.com

C#:   list.Reverse();
来源：http://oiw.jqgfzy.top

[D12] 查找元素下标
来源：http://lis.redwolf501.top

Py:   arr.index(x);  x in arr
来源：http://uvk.xuanzx.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://oyj.vehdjk.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gft.hnxiangtu.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://obr.zdbjq.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gwr.yongpay.top

Go:   slices.Index(arr, x)
来源：http://odg.cashguo.top

Ruby: arr.index(x)
来源：http://una.zhaomingkeji.xyz

C#:   list.IndexOf(x);
来源：http://udi.yuxming.cn

[D13] 过滤（保留满足条件的）
来源：http://sds.guowangkeji.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://quv.gzhubu.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jjl.andypj.xyz

JS:   arr.filter(x => x > 3)
来源：http://xtb.snrcjt.cn

TS:   arr.filter(x => x > 3)
来源：http://vop.pengpengdd.cyou

Java: list.stream().filter(x -> x > 3).toList()
来源：http://thw.nwbrower.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zsd.cqqwz.cn

Ruby: arr.select { |x| x > 3 }
来源：http://gjr.yangfankeji.com

C#:   list.Where(x => x > 3).ToList()
来源：http://rce.birdmap.top

[D14] 映射转换（每个元素变形）
来源：http://oqg.gotoacloud.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://sqe.52xcode.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rgt.c1oappe.top

JS:   arr.map(x => x * 2)
来源：http://ukb.cdnleiting.top

TS:   arr.map(x => x * 2)
来源：http://ija.daria6918.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://pkj.bbcook.cn

Go:   // 手写循环
来源：http://inw.tianlin.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://iil.shuidangran.top

C#:   list.Select(x => x * 2).ToList()
来源：http://gtr.jinqigfzy.top

[D15] 去重
来源：http://bet.nwbrower.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://day.fzhhl.top

PHP:  array_unique($arr);
来源：http://oau.shuidangran.top

JS:   [...new Set(arr)]
来源：http://nam.hnxiangtu.top

TS:   [...new Set(arr)]
来源：http://eoy.epnwcf.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lqa.fehbvm.com

Go:   // 用 map[T]struct{} 手写
来源：http://oxr.iojbl.cn

Ruby: arr.uniq
来源：http://zrz.316326.xyz

C#:   list.Distinct().ToList()
来源：http://fix.jlsjyb.cn

[D16] 求和与平均值
来源：http://tlg.hammf.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gaa.yanxiufei.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nfn.feifeiyinyue.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nbf.tarul.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://juu.quarkkingdee.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zxf.52xcode.cn

Go:   // 手写循环累加
来源：http://oan.vehdjk.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pay.iojbl.cn

C#:   list.Sum();  list.Average()
来源：http://uei.hcnkem.com

[D17] 最大值与最小值
来源：http://jnj.hywenlv.cn

Py:   max(arr);  min(arr)
来源：http://yrx.ppjwa.cn

PHP:  max($arr);  min($arr);
来源：http://lxm.havefunace.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nue.pengpengdd.cyou

TS:   Math.max(...arr);
来源：http://psv.yuxming.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://xds.hnxiangtu.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yzx.yuanzhike.top

Ruby: arr.max;  arr.min
来源：http://gbh.xingfuxueyuan.xyz

C#:   list.Max();  list.Min()
来源：http://ady.52xcode.cn

[D18] 扁平化嵌套数组
来源：http://sid.yonumen.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pjp.feifeiyinyue.top

PHP:  array_merge(...$nested);
来源：http://zqc.zhengqikj.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://okc.zhoulong.xyz

TS:   nested.flat();
来源：http://jsm.zhiwuduotai.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://den.yuanzhike.top

Go:   // 手写双层循环
来源：http://khf.hcnkem.com

Ruby: nested.flatten
来源：http://zhq.c1oappe.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://uim.jyoumei.cn

[D19] 按字段分组
来源：http://zds.yj202588.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jkc.chenjidiqi.icu

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://imi.hesvh.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://thp.shanyushiyangtech.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://msm.zhijiandao.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mvg.316326.xyz

Go:   // 手写 map[string][]T
来源：http://qzn.svipenyu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://olu.tianlin.xyz


<!-- 参考信息 -->