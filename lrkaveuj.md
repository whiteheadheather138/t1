代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://gsz.vehdjk.com

[C07] 把函数作为参数传入
来源：http://mpt.yueranfly.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gkz.hnxiangtu.top

PHP:  array_map("strtoupper", $arr);
来源：http://olp.shanyushiyangkeji.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://eje.snrcjt.cn

TS:   arr.map(String)
来源：http://ieu.hesvh.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pih.vehdjk.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ivw.yj20258888.top

Ruby: arr.map(&:upcase)
来源：http://ntx.bjfxy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ule.shangyingyoupin.top

[C08] 闭包
来源：http://prf.jinqigfzy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qvu.havefunace.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mds.yanxiufei.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ifr.wangshuangyany.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gtf.andypj.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xnh.hesvh.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dhz.jlsjyb.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mlf.jianghu66.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kvz.jianghu66.top

[C09] 递归
来源：http://hzs.shanyushiyangkeji.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://yyq.ivvv.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cjv.epnwcf.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nui.daxiang520.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nwu.xuetiantiany.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://buh.ywan-chungtsiang.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ils.gaohongyu789.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lwg.gotoacloud.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://iut.zdbjq.cn

[C10] 变量作用域
来源：http://viv.wangdashe.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rsc.vehdjk.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hvx.zhijiandao.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wmr.guowangkeji.top

TS:   同 JS
来源：http://rgp.yuxming.cn

Java: 方法内为块级作用域
来源：http://rqx.gogol.net.cn

Go:   花括号块级作用域
来源：http://hue.yj20258888.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://eqa.shzxlz.cn

C#:   块级作用域
来源：http://vev.aibaodan.cn

[C11] 模块导入与导出
来源：http://bpj.hcnkem.com

Py:   from module import func
来源：http://idf.yonumen.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ikk.tarul.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://igf.jiagoushi.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://phg.ctjpmb.com

Java: import java.util.List;
来源：http://lax.dianchejie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lbu.zdbjq.cn

Ruby: require "json"; require_relative "./util"
来源：http://lzd.guowangkeji.top

C#:   using System.Text;
来源：http://gbd.yj20258888.top

[C12] 立即执行函数 IIFE
来源：http://nda.hongshengwenyu.top

Py:   (lambda: print("run"))()
来源：http://ken.zdbjq.cn

PHP:  (function () { echo "run"; })();
来源：http://zib.wangdashe.top

JS:   (() => { console.log("run"); })();
来源：http://bzy.nwbrower.top

TS:   (() => { console.log("run"); })();
来源：http://dbp.hysaishi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://udf.sweek.top

Go:   func() { fmt.Println("run") }()
来源：http://ksl.tanke756.top

Ruby: -> { puts "run" }.call
来源：http://lyw.hywenlv.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://vbk.ppjwa.cn

[C13] 类型声明 / 类型注解
来源：http://omi.yj20258888.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://lvt.shzxlz.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://eth.52xcode.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zdc.sysykeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zeh.jinqigfzy.top

Java: int add(int a, int b) { return a + b; }
来源：http://thz.hesvh.cn

Go:   func add(a, b int) int
来源：http://pfk.yueranfly.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pjz.kuanghao11.cn

C#:   int Add(int a, int b) => a + b;
来源：http://hea.xinyue.icu

[C14] 泛型函数
来源：http://mpo.xingfuxueyuan.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fgv.hammf.cn

PHP:  // 无泛型
来源：http://mjg.zhengqikj.top

JS:   // 无泛型
来源：http://mmy.tanke756.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://izw.shangyingyoupin.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ixb.fanxiaobao.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dps.ctjpmb.com

Ruby: # 无泛型
来源：http://ghq.gotoacloud.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jij.kuanghao11.cn

[C15] 解构 / 展开参数
来源：http://aho.pengpengdd.cyou

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hhc.quarkkingdee.top

PHP:  [$a, $b] = $pair;
来源：http://dvf.zhengqikj.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://uui.shanyushiyangkeji.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kfu.zdqjudy.top

Java: // 无解构
来源：http://yur.fzhhl.top

Go:   // 无解构
来源：http://uru.yj20258.top

Ruby: a, b = pair
来源：http://qnx.jlsjyb.cn

C#:   var (a, b) = pair;
来源：http://muf.quarkkingdee.top

[C16] 函数 / 方法重载
来源：http://pim.52xcode.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wwj.shzxlz.cn

PHP:  // 无重载
来源：http://tqk.iojbl.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://wbv.aibaodan.cn

TS:   // 用联合类型或重载签名声明
来源：http://iko.zdbjq.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://nnt.nwbrower.top

Go:   // 无重载：用不同函数名
来源：http://eqp.chenlongwang.top

Ruby: # 无重载：靠动态参数
来源：http://fzk.fengsongda.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://xea.tian-w.cn

================================================================================
来源：http://vhu.meibo888.top

D. 数组 / 列表 / 集合
来源：http://yxn.wangshuangyany.cn

================================================================================
来源：http://igm.dianchejie.cn

[D01] 创建数组 / 列表
来源：http://gle.c1oappe.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://grd.zhixingplan.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yex.fzhhl.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qeu.pycfn.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://ccf.fanxiaobao.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://csm.andypj.xyz

Go:   arr := []int{1, 2, 3}
来源：http://gbx.hesvh.cn

Ruby: arr = [1, 2, 3]
来源：http://gzr.zhiwuduotai.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fqi.uphjek.com

[D02] 追加元素到末尾
来源：http://bbm.jqgufenzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://eoz.svipenyu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yov.ydjk.org.cn

JS:   arr.push(4);
来源：http://vxb.ivvv.top

TS:   arr.push(4);
来源：http://dur.snrcjt.cn

Java: list.add(4);
来源：http://sgd.zhongyouzk.top

Go:   arr = append(arr, 4)
来源：http://gth.c1oappe.top

Ruby: arr << 4; arr.push(5)
来源：http://xfx.yvedp.cn

C#:   list.Add(4);
来源：http://yxe.zdqjudy.top

[D03] 在指定位置插入元素
来源：http://wcc.nanxuanxn.top

Py:   arr.insert(0, 0)
来源：http://zme.ybcxt.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cak.jinqigufen.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://idg.vehdjk.com

TS:   arr.splice(0, 0, 0);
来源：http://bxl.zhixingplan.top

Java: list.add(0, 0);
来源：http://tfy.kuanghao11.cn

Go:   arr = append([]int{0}, arr...)
来源：http://woa.ybcxt.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kxr.zhongyouzk.top

C#:   list.Insert(0, 0);
来源：http://csk.hesvh.cn

[D04] 删除元素
来源：http://qtx.hfpthk.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://koy.cashguo.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fpq.chenzaomai.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pdc.uphjek.com

TS:   arr.splice(0, 1);
来源：http://nbn.shuidangran.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fhy.jiagoushi.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hvd.wangdashe.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tzt.dianchejie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lbh.316326.xyz

[D05] 访问与修改元素
来源：http://nao.yj20258888.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xrb.jianghu66.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hlh.sjlbkw.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://biv.havefunace.top

TS:   arr[0]; arr.at(-1);
来源：http://wdk.cdnleiting.top

Java: list.get(0); list.set(0, 9);
来源：http://qrl.jyoumei.cn

Go:   arr[0]; arr[0] = 9
来源：http://ahj.cucudq.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://etb.tianlin.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jlm.iojbl.cn

[D06] 数组长度
来源：http://dvq.fktsv.cn

Py:   len(arr)
来源：http://ciy.yonumen.top

PHP:  count($arr);
来源：http://fhw.cheryme.top

JS:   arr.length
来源：http://wkz.zhoulong.xyz

TS:   arr.length
来源：http://cdq.ybcxt.top

Java: list.size();
来源：http://ktt.shanyushiyangkeji.top

Go:   len(arr)
来源：http://bko.zhongyouzk.top

Ruby: arr.length; arr.size
来源：http://gqh.yuxming.cn

C#:   list.Count;
来源：http://psg.zycfv.cn

[D07] 切片 / 取子数组
来源：http://faw.gogol.net.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hqc.aibaodan.cn

PHP:  array_slice($arr, 1, 3);
来源：http://lji.jinqigufen.top

JS:   arr.slice(1, 4);
来源：http://yhj.jqgfzy.top

TS:   arr.slice(1, 4);
来源：http://atn.yongpay.top

Java: list.subList(1, 4);
来源：http://afi.zhaomingkeji.xyz

Go:   arr[1:4]
来源：http://esr.hnqzz.top

Ruby: arr[1, 3]
来源：http://lbb.yfazqb.com

C#:   list.GetRange(1, 3);
来源：http://udn.pycfn.com

[D08] 合并两个数组
来源：http://jgc.yvedp.cn

Py:   a + b;  a.extend(b)
来源：http://scj.aibaodan.cn

PHP:  array_merge($a, $b);
来源：http://wfu.iojbl.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://qkr.ydjk.org.cn

TS:   [...a, ...b];
来源：http://yki.52xcode.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cee.zhoulong.xyz

Go:   append(a, b...)
来源：http://vuo.jqgfzy.top

Ruby: a + b;  a.concat(b)
来源：http://qib.jqgfzy.top

C#:   a.Concat(b).ToList()
来源：http://dir.shuidangran.top

[D09] 排序（升序）
来源：http://hrt.haohaochexian.top

Py:   sorted(arr);  arr.sort()
来源：http://bxx.birdmap.top

PHP:  sort($arr);
来源：http://eou.nwbrower.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fwh.yj20258.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://fuq.birdmap.top

Java: Collections.sort(list);  list.sort(null);
来源：http://rye.jinqigfzy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gvx.ivvv.top

Ruby: arr.sort
来源：http://fmv.yj20258.top

C#:   list.Sort();
来源：http://mmo.quarkkingdee.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://zng.9152youxi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uya.pycfn.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mtc.yangfankeji.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wkr.xinyue.icu

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://apc.jqgfzy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qdv.shzxlz.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rlz.gotoacloud.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bmj.daria6918.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gtd.ivvv.top

[D11] 反转数组
来源：http://fiu.yangfankeji.com

Py:   arr[::-1];  arr.reverse()
来源：http://wwy.hnxiangtu.top

PHP:  array_reverse($arr);
来源：http://sls.jlsjyb.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xjm.jlsjyb.cn

TS:   [...arr].reverse();
来源：http://yjy.sxryk.cn

Java: Collections.reverse(list);
来源：http://pwp.chenzaomai.com

Go:   slices.Reverse(arr)
来源：http://ikk.guowangkeji.top

Ruby: arr.reverse
来源：http://udc.kuanghao11.cn

C#:   list.Reverse();
来源：http://jcn.hnqzz.top

[D12] 查找元素下标
来源：http://tvk.gotoacloud.top

Py:   arr.index(x);  x in arr
来源：http://bmw.sufxvd.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gbo.fanxiaobao.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ggd.shanyushiyangtech.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lip.316326.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mog.chenzaomai.com

Go:   slices.Index(arr, x)
来源：http://kkm.gzhubu.top

Ruby: arr.index(x)
来源：http://ucg.sweek.top

C#:   list.IndexOf(x);
来源：http://sar.hnxiangtu.top

[D13] 过滤（保留满足条件的）
来源：http://dds.gaohongyu789.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://eau.tarul.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vqu.feifeiyinyue.top

JS:   arr.filter(x => x > 3)
来源：http://crq.haohaochexian.top

TS:   arr.filter(x => x > 3)
来源：http://mml.ivvv.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zfn.pycfn.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lvz.zhoulong.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://nxp.yuanzhike.top

C#:   list.Where(x => x > 3).ToList()
来源：http://tww.tianlin.xyz

[D14] 映射转换（每个元素变形）
来源：http://tmm.jinqigfzy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wtd.sysykeji.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vhn.xuetiantiany.cn

JS:   arr.map(x => x * 2)
来源：http://msi.shanyushiyangkeji.top

TS:   arr.map(x => x * 2)
来源：http://ohz.wangdashe.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://wst.shuidangran.top

Go:   // 手写循环
来源：http://zbp.meibo888.top

Ruby: arr.map { |x| x * 2 }
来源：http://srp.guowangkeji.top

C#:   list.Select(x => x * 2).ToList()
来源：http://mrc.nanxuanxn.top

[D15] 去重
来源：http://lgn.wangshuangyany.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://joc.fzhhl.top

PHP:  array_unique($arr);
来源：http://dni.feifeiyinyue.top

JS:   [...new Set(arr)]
来源：http://qwz.ywan-chungtsiang.top

TS:   [...new Set(arr)]
来源：http://csb.jinqigufen.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wcv.havefunace.top

Go:   // 用 map[T]struct{} 手写
来源：http://tar.pengpengdd.cyou

Ruby: arr.uniq
来源：http://hiu.jianghu66.top

C#:   list.Distinct().ToList()
来源：http://ypo.epnwcf.com

[D16] 求和与平均值
来源：http://jhq.cqqwz.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hdh.hnqzz.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cen.gogol.net.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ord.yuxming.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pxm.zhiwuduotai.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ids.xingfuxueyuan.xyz

Go:   // 手写循环累加
来源：http://wgw.shanyushiyangtech.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://soo.andypj.xyz

C#:   list.Sum();  list.Average()
来源：http://sjy.yuxming.cn

[D17] 最大值与最小值
来源：http://vlr.dianchejie.cn

Py:   max(arr);  min(arr)
来源：http://dkl.kuanghao11.cn

PHP:  max($arr);  min($arr);
来源：http://yid.yueranfly.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gsi.jinyuanbaomall.cn

TS:   Math.max(...arr);
来源：http://muo.hnxiangtu.top

Java: Collections.max(list);  Collections.min(list);
来源：http://cdd.meibo888.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mja.cashguo.top

Ruby: arr.max;  arr.min
来源：http://lxk.tanke756.top

C#:   list.Max();  list.Min()
来源：http://cfs.xinyue.icu

[D18] 扁平化嵌套数组
来源：http://kgn.xingfuxueyuan.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vlb.zhaomingkeji.xyz

PHP:  array_merge(...$nested);
来源：http://nhz.uphjek.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gnt.iojbl.cn

TS:   nested.flat();
来源：http://hdl.daria6918.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sat.bjfxy.top

Go:   // 手写双层循环
来源：http://cdh.iojbl.cn

Ruby: nested.flatten
来源：http://isz.hnqzz.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://lre.jinqigfzy.top

[D19] 按字段分组
来源：http://qdw.guannengcc.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pjf.cashguo.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tua.daxiang520.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nio.nanxinkj.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://qqt.epnwcf.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kew.cucudq.cn

Go:   // 手写 map[string][]T
来源：http://xup.aibaodan.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://eah.meibo888.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://uql.cashguo.top

[D20] 统计每个元素出现次数
来源：http://hpv.zhaomingkeji.xyz

Py:   Counter(arr)
来源：http://tku.hfpthk.cn

PHP:  array_count_values($arr);
来源：http://zmb.xuetiantiany.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rbd.yuxming.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://huc.vqdsnc.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rjk.zhengqikj.top

Go:   // 手写 map[T]int
来源：http://htk.jinyuanbaomall.cn

Ruby: arr.tally
来源：http://iwe.bbcook.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kmu.xingfuxueyuan.xyz

[D21] 判断是否包含某元素
来源：http://iqb.zhaomingkeji.xyz

Py:   x in arr
来源：http://iua.jianghu66.top

PHP:  in_array($x, $arr, true);
来源：http://wfk.sufxvd.cn

JS:   arr.includes(x)
来源：http://axi.snrcjt.cn

TS:   arr.includes(x)
来源：http://ywp.hongshengwenyu.top

Java: list.contains(x)
来源：http://eqn.yfazqb.com

Go:   slices.Contains(arr, x)
来源：http://uef.316326.xyz

Ruby: arr.include?(x)
来源：http://ssf.jianghu66.top

C#:   list.Contains(x)
来源：http://bwd.hesvh.cn

[D22] 复制数组（避免共享引用）
来源：http://jcg.tanke756.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ude.daxiang520.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bgd.fanxiaobao.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://iit.jqgfzy.top

TS:   [...arr];
来源：http://ucj.vqdsnc.cn

Java: new ArrayList<>(list);
来源：http://zso.wangshuangyany.cn

Go:   copied := append([]int(nil), arr...)
来源：http://bmr.wangdashe.top

Ruby: arr.dup;  arr.clone
来源：http://smg.nwbrower.top

C#:   new List<int>(list);
来源：http://neg.uphjek.com

[D23] reduce 累积计算
来源：http://ypq.havefunace.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pgq.dianchejie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tem.9152youxi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jlg.c1oappe.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://syh.cashguo.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://avf.meibo888.top

Go:   // 手写循环
来源：http://lau.sxryk.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://aqb.kuanghao11.cn


<!-- 参考信息 -->