代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wej.fzhhl.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qat.sweek.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gxl.yongpay.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sun.ivvv.top

Ruby: def total(*nums); nums.sum; end
来源：http://xuf.aizwys.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jsb.zycfv.cn

[C04] 命名参数 / 关键字参数
来源：http://fey.zhengqikj.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dto.ydzc1.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wpy.iojbl.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kuc.zycfv.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rnv.jqgufenzy.top

Java: // 无：用 Builder 模式或 record
来源：http://mch.nanxuanxn.top

Go:   // 无：用配置结构体参数
来源：http://xex.birdmap.top

Ruby: f(a: 1, b: 2)
来源：http://pma.yuxming.cn

C#:   f(a: 1, b: 2)
来源：http://ylf.guowangkeji.top

[C05] 返回多个值
来源：http://stk.yfazqb.com

Py:   return a, b
来源：http://zzh.daxiang520.top

PHP:  return [$a, $b];
来源：http://bjv.jqgfzy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://hhb.xinyue.icu

TS:   return { a, b };
来源：http://gdf.guowangkeji.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rdd.gaohongyu789.top

Go:   return a, b
来源：http://wrl.gzhubu.top

Ruby: return a, b
来源：http://nsh.havefunace.top

C#:   return (a, b);              // ValueTuple
来源：http://yyj.hnqzz.top

[C06] 匿名函数 / lambda
来源：http://thk.cqqwz.cn

Py:   square = lambda x: x * x
来源：http://uxa.quarkkingdee.top

PHP:  $square = fn($x) => $x * $x;
来源：http://spl.jqgfzy.top

JS:   const square = x => x * x;
来源：http://ibd.xuanzx.com

TS:   const square = (x: number): number => x * x;
来源：http://vjj.zdbjq.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://owm.ppjwa.cn

Go:   sq := func(x int) int { return x * x }
来源：http://cmz.feifeiyinyue.top

Ruby: square = ->(x) { x * x }
来源：http://uuf.zhixingplan.top

C#:   Func<int, int> square = x => x * x;
来源：http://iwm.yanxiufei.cn

[C07] 把函数作为参数传入
来源：http://dyr.fehbvm.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wki.fzhhl.top

PHP:  array_map("strtoupper", $arr);
来源：http://jrn.pengpengdd.cyou

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://acs.jinqigfzy.top

TS:   arr.map(String)
来源：http://wmv.yuxming.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ndb.gaohongyu789.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://owe.svipenyu.cn

Ruby: arr.map(&:upcase)
来源：http://vme.epnwcf.com

C#:   arr.Select(s => s.ToUpper())
来源：http://pmk.zhiwuduotai.top

[C08] 闭包
来源：http://kjt.0kj1m.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xct.nanxinkj.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ozm.hcnkem.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mpi.nwbrower.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://the.daxiang520.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fhr.sweek.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://asc.iojbl.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jax.dianchejie.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://win.hammf.cn

[C09] 递归
来源：http://kvg.shuidangran.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pqc.dianchejie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cxr.chenlongwang.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qdv.guannengcc.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bhp.jyoumei.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jev.wangdashe.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xvc.yuanzhike.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ofk.52xcode.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kvm.svipenyu.cn

[C10] 变量作用域
来源：http://jwc.jyoumei.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dah.nanxuanxn.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://asx.hysaishi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wem.sufxvd.cn

TS:   同 JS
来源：http://trp.cqqwz.cn

Java: 方法内为块级作用域
来源：http://vic.yj20258888.top

Go:   花括号块级作用域
来源：http://qvz.aibaodan.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bmh.ydzc1.top

C#:   块级作用域
来源：http://pku.gotoacloud.top

[C11] 模块导入与导出
来源：http://oyr.dianchejie.cn

Py:   from module import func
来源：http://aet.shzxlz.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://czu.ivvv.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://zhv.guowangkeji.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fgm.daxiang520.top

Java: import java.util.List;
来源：http://ocf.shzxlz.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hsd.yj202588.top

Ruby: require "json"; require_relative "./util"
来源：http://nsy.hnxiangtu.top

C#:   using System.Text;
来源：http://mok.fktsv.cn

[C12] 立即执行函数 IIFE
来源：http://edz.fktsv.cn

Py:   (lambda: print("run"))()
来源：http://cvv.9152youxi.cn

PHP:  (function () { echo "run"; })();
来源：http://vyk.sjlbkw.cn

JS:   (() => { console.log("run"); })();
来源：http://tgy.dianchejie.cn

TS:   (() => { console.log("run"); })();
来源：http://slb.zdbjq.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hbi.jqgfzy.top

Go:   func() { fmt.Println("run") }()
来源：http://agl.shanyushiyangkeji.top

Ruby: -> { puts "run" }.call
来源：http://ttm.xziqi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://sib.zhoulong.xyz

[C13] 类型声明 / 类型注解
来源：http://afy.hesvh.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fqa.hesvh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lea.shanyushiyangkeji.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ppn.haohaochexian.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dme.hywenlv.cn

Java: int add(int a, int b) { return a + b; }
来源：http://utf.wangshuangyany.cn

Go:   func add(a, b int) int
来源：http://oqg.daxiang520.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nuu.ydzc1.top

C#:   int Add(int a, int b) => a + b;
来源：http://wkj.jqgfzy.top

[C14] 泛型函数
来源：http://pdk.pycfn.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ghv.mhx1999.top

PHP:  // 无泛型
来源：http://bnc.zdqjudy.top

JS:   // 无泛型
来源：http://qiw.zdbjq.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uit.52xcode.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mcc.jinqigfzy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gze.bjfxy.top

Ruby: # 无泛型
来源：http://ree.andypj.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ejv.zhijiandao.cn

[C15] 解构 / 展开参数
来源：http://mzb.tianlin.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rxj.zhengqikj.top

PHP:  [$a, $b] = $pair;
来源：http://lgj.gaohongyu789.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dva.aizwys.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://onj.zdqjudy.top

Java: // 无解构
来源：http://bjr.zhijiandao.cn

Go:   // 无解构
来源：http://fvu.feifeiyinyue.top

Ruby: a, b = pair
来源：http://gxw.sjlbkw.cn

C#:   var (a, b) = pair;
来源：http://exj.jiagoushi.top

[C16] 函数 / 方法重载
来源：http://lvn.zhengqikj.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://axu.yuanzhike.top

PHP:  // 无重载
来源：http://ubk.xziqi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://orh.tianlin.xyz

TS:   // 用联合类型或重载签名声明
来源：http://avd.fktsv.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://fpm.sjlbkw.cn

Go:   // 无重载：用不同函数名
来源：http://avt.fktsv.cn

Ruby: # 无重载：靠动态参数
来源：http://jmc.yanxiufei.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://tpi.kuanghao11.cn

================================================================================
来源：http://ulw.jlsjyb.cn

D. 数组 / 列表 / 集合
来源：http://brf.ydzc1.top

================================================================================
来源：http://edy.jqgfzy.top

[D01] 创建数组 / 列表
来源：http://eiw.cashguo.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://asz.gogol.net.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://otg.jinqigufen.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rxh.vehdjk.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://ljq.52xcode.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ssi.feifeiyinyue.top

Go:   arr := []int{1, 2, 3}
来源：http://bds.tian-w.cn

Ruby: arr = [1, 2, 3]
来源：http://wlf.nwbrower.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tca.svipenyu.cn

[D02] 追加元素到末尾
来源：http://ogr.shangyingyoupin.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fna.jqgfzy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dmg.cheryme.top

JS:   arr.push(4);
来源：http://pdj.pengpengdd.cyou

TS:   arr.push(4);
来源：http://cec.nanxuanxn.top

Java: list.add(4);
来源：http://fdp.c1oappe.top

Go:   arr = append(arr, 4)
来源：http://qxx.yvedp.cn

Ruby: arr << 4; arr.push(5)
来源：http://csn.gzhubu.top

C#:   list.Add(4);
来源：http://bql.jinyuanbaomall.cn

[D03] 在指定位置插入元素
来源：http://yuw.iojbl.cn

Py:   arr.insert(0, 0)
来源：http://uqn.zhongyouzk.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wcu.feifeiyinyue.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vwn.tarul.cn

TS:   arr.splice(0, 0, 0);
来源：http://pej.hywenlv.cn

Java: list.add(0, 0);
来源：http://ewa.ydjk.org.cn

Go:   arr = append([]int{0}, arr...)
来源：http://wvj.nanxinkj.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://tvf.xziqi.cn

C#:   list.Insert(0, 0);
来源：http://knv.hongshengwenyu.top

[D04] 删除元素
来源：http://orf.sweek.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://imy.bbcook.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://avh.yj20258.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://htl.hysaishi.cn

TS:   arr.splice(0, 1);
来源：http://biv.yangfankeji.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qqh.yvedp.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://utd.pycfn.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://drv.jinqigufen.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nii.ywan-chungtsiang.top

[D05] 访问与修改元素
来源：http://vps.xziqi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lin.birdmap.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ttm.uphjek.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tev.yongpay.top

TS:   arr[0]; arr.at(-1);
来源：http://eaj.haohaochexian.top

Java: list.get(0); list.set(0, 9);
来源：http://tew.ywan-chungtsiang.top

Go:   arr[0]; arr[0] = 9
来源：http://ike.shzxlz.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ndo.shanyushiyangkeji.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://haw.9152youxi.cn

[D06] 数组长度
来源：http://svm.cdnleiting.top

Py:   len(arr)
来源：http://uxs.jyoumei.cn

PHP:  count($arr);
来源：http://uzl.tanke756.top

JS:   arr.length
来源：http://thx.feifeiyinyue.top

TS:   arr.length
来源：http://kau.ehwqpu.com

Java: list.size();
来源：http://xby.zhoulong.xyz

Go:   len(arr)
来源：http://ofb.quarkkingdee.top

Ruby: arr.length; arr.size
来源：http://lsj.kuanghao11.cn

C#:   list.Count;
来源：http://mqk.ehwqpu.com

[D07] 切片 / 取子数组
来源：http://oep.ivvv.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hrp.sufxvd.cn

PHP:  array_slice($arr, 1, 3);
来源：http://stt.yj20258888.top

JS:   arr.slice(1, 4);
来源：http://zqn.bbcook.cn

TS:   arr.slice(1, 4);
来源：http://wdo.haohaochexian.top

Java: list.subList(1, 4);
来源：http://xfw.birdmap.top

Go:   arr[1:4]
来源：http://noc.daria6918.cn

Ruby: arr[1, 3]
来源：http://wfz.nanxinkj.top

C#:   list.GetRange(1, 3);
来源：http://caj.xylfe.cn

[D08] 合并两个数组
来源：http://qzw.tanke756.top

Py:   a + b;  a.extend(b)
来源：http://ftc.quarkkingdee.top

PHP:  array_merge($a, $b);
来源：http://sxe.fehbvm.com

JS:   [...a, ...b];  a.concat(b);
来源：http://wmx.hysaishi.cn

TS:   [...a, ...b];
来源：http://lgq.zdbjq.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://adq.yfazqb.com

Go:   append(a, b...)
来源：http://zax.xuetiantiany.cn

Ruby: a + b;  a.concat(b)
来源：http://tlv.chenzaomai.com

C#:   a.Concat(b).ToList()
来源：http://ril.0kj1m.cn

[D09] 排序（升序）
来源：http://dgq.zhengqikj.top

Py:   sorted(arr);  arr.sort()
来源：http://iqy.jyoumei.cn

PHP:  sort($arr);
来源：http://mom.jlsjyb.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cvo.sjlbkw.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ldg.andypj.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://gfa.shuidangran.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jkd.nwbrower.top

Ruby: arr.sort
来源：http://ojy.xuanzx.com

C#:   list.Sort();
来源：http://kkw.xingfuxueyuan.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://quj.zhijiandao.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tgv.smart0.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oqk.pengpengdd.cyou

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://szr.andypj.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://iey.andypj.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bae.jqgfzy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zys.hysaishi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bjw.dianchejie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gac.guannengcc.top

[D11] 反转数组
来源：http://ikr.0kj1m.cn

Py:   arr[::-1];  arr.reverse()
来源：http://pvj.vqdsnc.cn

PHP:  array_reverse($arr);
来源：http://twy.yj20258888.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lxc.hfpthk.cn

TS:   [...arr].reverse();
来源：http://hlh.redwolf501.top

Java: Collections.reverse(list);
来源：http://vww.tarul.cn

Go:   slices.Reverse(arr)
来源：http://knd.hnqzz.top

Ruby: arr.reverse
来源：http://oma.fengsongda.top

C#:   list.Reverse();
来源：http://azx.ivvv.top

[D12] 查找元素下标
来源：http://hnw.zycfv.cn

Py:   arr.index(x);  x in arr
来源：http://xnt.yfazqb.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://exn.yanxiufei.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://umw.zdqjudy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gky.fktsv.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://eay.gaohongyu789.top

Go:   slices.Index(arr, x)
来源：http://bvt.zdbjq.cn

Ruby: arr.index(x)
来源：http://sjn.nwbrower.top

C#:   list.IndexOf(x);
来源：http://uut.ppjwa.cn

[D13] 过滤（保留满足条件的）
来源：http://owc.shanyushiyangkeji.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jxa.0kj1m.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://slk.gaohongyu789.top

JS:   arr.filter(x => x > 3)
来源：http://nlw.zhoulong.xyz

TS:   arr.filter(x => x > 3)
来源：http://bbk.zhixingplan.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wki.guannengcc.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://orx.ydjk.org.cn

Ruby: arr.select { |x| x > 3 }
来源：http://nbh.0kj1m.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://eap.fanxiaobao.xyz

[D14] 映射转换（每个元素变形）
来源：http://nlp.havefunace.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://sdi.yfazqb.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ioq.zycfv.cn

JS:   arr.map(x => x * 2)
来源：http://pmb.ybcxt.top

TS:   arr.map(x => x * 2)
来源：http://vot.xylfe.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://hxi.yuanzhike.top

Go:   // 手写循环
来源：http://qbr.uphjek.com

Ruby: arr.map { |x| x * 2 }
来源：http://zus.fengsongda.top

C#:   list.Select(x => x * 2).ToList()
来源：http://mcn.yuanzhike.top

[D15] 去重
来源：http://mvj.aizwys.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ybj.yueranfly.top

PHP:  array_unique($arr);
来源：http://tfj.mhx1999.top

JS:   [...new Set(arr)]
来源：http://hco.zhixingplan.top

TS:   [...new Set(arr)]
来源：http://srz.jqgufenzy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://opm.shanyushiyangkeji.top

Go:   // 用 map[T]struct{} 手写
来源：http://idw.yongpay.top

Ruby: arr.uniq
来源：http://kkh.smart0.xyz

C#:   list.Distinct().ToList()
来源：http://ens.ydjk.org.cn

[D16] 求和与平均值
来源：http://tsy.yuanzhike.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://trs.daxiang520.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dyd.ydzc1.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fmn.jinqigufen.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ifl.havefunace.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kal.gzhubu.top

Go:   // 手写循环累加
来源：http://zay.yuxming.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zak.xuetiantiany.cn

C#:   list.Sum();  list.Average()
来源：http://qin.smart0.xyz

[D17] 最大值与最小值
来源：http://hmc.aizwys.cn

Py:   max(arr);  min(arr)
来源：http://kdi.jianghu66.top

PHP:  max($arr);  min($arr);
来源：http://ksq.zhoulong.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wfe.ywan-chungtsiang.top

TS:   Math.max(...arr);
来源：http://axn.aizwys.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://sch.yueranfly.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xos.yfazqb.com

Ruby: arr.max;  arr.min
来源：http://esp.yuxming.cn

C#:   list.Max();  list.Min()
来源：http://iik.c1oappe.top

[D18] 扁平化嵌套数组
来源：http://bum.kuanghao11.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lpj.c1oappe.top

PHP:  array_merge(...$nested);
来源：http://pva.birdmap.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://obf.hnxiangtu.top

TS:   nested.flat();
来源：http://rpo.ydjk.org.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://oyh.wangdashe.top

Go:   // 手写双层循环
来源：http://xrb.jlsjyb.cn

Ruby: nested.flatten
来源：http://inu.guannengcc.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://jkq.bjfxy.top

[D19] 按字段分组
来源：http://dsb.hfpthk.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dsp.hesvh.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mbj.ydjk.org.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cnn.quarkkingdee.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://sdp.haohaochexian.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fne.dashuyun.cn

Go:   // 手写 map[string][]T
来源：http://rdj.tarul.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://bks.dashuyun.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cgc.nwbrower.top

[D20] 统计每个元素出现次数
来源：http://ufp.xziqi.cn

Py:   Counter(arr)
来源：http://jxh.svipenyu.cn

PHP:  array_count_values($arr);
来源：http://bsg.aizwys.cn


<!-- 参考信息 -->