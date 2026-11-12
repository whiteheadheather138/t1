代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nww.mhx1999.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jdg.jinqigfzy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nyg.jinqigufen.top

[C09] 递归
来源：http://opb.hnxiangtu.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cor.hysaishi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ccv.zhengqikj.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://inf.feifeiyinyue.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://csq.xuanzx.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bch.daria6918.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vxc.cqqwz.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vnu.ehwqpu.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xyd.yvedp.cn

[C10] 变量作用域
来源：http://qgx.ivvv.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://icd.sjlbkw.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gun.ppjwa.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://whm.sysykeji.top

TS:   同 JS
来源：http://gpi.tianlin.xyz

Java: 方法内为块级作用域
来源：http://mcd.ybcxt.top

Go:   花括号块级作用域
来源：http://hwz.nwbrower.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://iog.jinghuilouyu.cn

C#:   块级作用域
来源：http://gbe.svipenyu.cn

[C11] 模块导入与导出
来源：http://gje.ybcxt.top

Py:   from module import func
来源：http://scm.jyoumei.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://xba.gaohongyu789.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://yzt.iojbl.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jda.svipenyu.cn

Java: import java.util.List;
来源：http://cyv.nwbrower.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kwd.nanxuanxn.top

Ruby: require "json"; require_relative "./util"
来源：http://ocq.zhaomingkeji.xyz

C#:   using System.Text;
来源：http://vzr.birdmap.top

[C12] 立即执行函数 IIFE
来源：http://ybb.daria6918.cn

Py:   (lambda: print("run"))()
来源：http://jvn.jinyuanbaomall.cn

PHP:  (function () { echo "run"; })();
来源：http://lvl.52xcode.cn

JS:   (() => { console.log("run"); })();
来源：http://bid.chenzaomai.com

TS:   (() => { console.log("run"); })();
来源：http://pmi.kuanghao11.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rny.xuanzx.com

Go:   func() { fmt.Println("run") }()
来源：http://dos.xuanzx.com

Ruby: -> { puts "run" }.call
来源：http://rah.jianghu66.top

C#:   // 无 IIFE：用静态构造函数
来源：http://muc.yuxming.cn

[C13] 类型声明 / 类型注解
来源：http://kqn.hfpthk.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xdq.dashuyun.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://myo.gotoacloud.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wcq.daria6918.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yet.hywenlv.cn

Java: int add(int a, int b) { return a + b; }
来源：http://txd.redwolf501.top

Go:   func add(a, b int) int
来源：http://pil.yfazqb.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mpq.cheryme.top

C#:   int Add(int a, int b) => a + b;
来源：http://uni.jinyuanbaomall.cn

[C14] 泛型函数
来源：http://yqs.gaohongyu789.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gse.ydzc1.top

PHP:  // 无泛型
来源：http://bmv.316326.xyz

JS:   // 无泛型
来源：http://jsk.xuanzx.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zll.fehbvm.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ggs.cdnleiting.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wbg.gzhubu.top

Ruby: # 无泛型
来源：http://kuw.tian-w.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lsd.cqqwz.cn

[C15] 解构 / 展开参数
来源：http://erm.fengsongda.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bln.wangshuangyany.cn

PHP:  [$a, $b] = $pair;
来源：http://sup.jinghuilouyu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jwl.zhengqikj.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ebu.ctjpmb.com

Java: // 无解构
来源：http://bvu.ydzc1.top

Go:   // 无解构
来源：http://nsc.smart0.xyz

Ruby: a, b = pair
来源：http://kjq.hesvh.cn

C#:   var (a, b) = pair;
来源：http://hav.hammf.cn

[C16] 函数 / 方法重载
来源：http://xux.meibo888.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tbr.cheryme.top

PHP:  // 无重载
来源：http://zfn.zhaomingkeji.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://xst.fanxiaobao.xyz

TS:   // 用联合类型或重载签名声明
来源：http://uzr.0kj1m.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://jtl.xuetiantiany.cn

Go:   // 无重载：用不同函数名
来源：http://uku.xinyue.icu

Ruby: # 无重载：靠动态参数
来源：http://lgd.yanxiufei.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://vkp.jyoumei.cn

================================================================================
来源：http://dvr.ehwqpu.com

D. 数组 / 列表 / 集合
来源：http://vbg.xuanzx.com

================================================================================
来源：http://azg.zdbjq.cn

[D01] 创建数组 / 列表
来源：http://hnz.shuidangran.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://bjg.mhx1999.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zhh.quarkkingdee.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jlc.zycfv.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ifc.yuanzhike.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xdb.ydzc1.top

Go:   arr := []int{1, 2, 3}
来源：http://omt.yueranfly.top

Ruby: arr = [1, 2, 3]
来源：http://wos.nanxinkj.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tfo.zhongyouzk.top

[D02] 追加元素到末尾
来源：http://wjl.smart0.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ivx.kuanghao11.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tgx.wangdashe.top

JS:   arr.push(4);
来源：http://vcf.zdqjudy.top

TS:   arr.push(4);
来源：http://zjt.pycfn.com

Java: list.add(4);
来源：http://pbu.epnwcf.com

Go:   arr = append(arr, 4)
来源：http://obo.jinghuilouyu.cn

Ruby: arr << 4; arr.push(5)
来源：http://jxf.sjlbkw.cn

C#:   list.Add(4);
来源：http://yco.cashguo.top

[D03] 在指定位置插入元素
来源：http://zwr.tian-w.cn

Py:   arr.insert(0, 0)
来源：http://hai.havefunace.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cff.yj202588.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hif.9152youxi.cn

TS:   arr.splice(0, 0, 0);
来源：http://srz.ehwqpu.com

Java: list.add(0, 0);
来源：http://bij.cashguo.top

Go:   arr = append([]int{0}, arr...)
来源：http://bxe.cdnleiting.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kko.jqgufenzy.top

C#:   list.Insert(0, 0);
来源：http://wyd.yangfankeji.com

[D04] 删除元素
来源：http://efd.c1oappe.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ggo.svipenyu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vjl.yongpay.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rcb.tarul.cn

TS:   arr.splice(0, 1);
来源：http://zre.andypj.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dms.hywenlv.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mhk.daxiang520.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zyo.tianlin.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vec.xylfe.cn

[D05] 访问与修改元素
来源：http://mdo.aibaodan.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vys.haohaochexian.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nky.epnwcf.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nrs.yanxiufei.cn

TS:   arr[0]; arr.at(-1);
来源：http://dpw.9152youxi.cn

Java: list.get(0); list.set(0, 9);
来源：http://fqs.smart0.xyz

Go:   arr[0]; arr[0] = 9
来源：http://dig.vqdsnc.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fsn.sufxvd.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pyh.c1oappe.top

[D06] 数组长度
来源：http://lso.jinyuanbaomall.cn

Py:   len(arr)
来源：http://mko.shzxlz.cn

PHP:  count($arr);
来源：http://xxn.tarul.cn

JS:   arr.length
来源：http://rxx.zhengqikj.top

TS:   arr.length
来源：http://oty.jiagoushi.top

Java: list.size();
来源：http://olk.gogol.net.cn

Go:   len(arr)
来源：http://gex.xinyue.icu

Ruby: arr.length; arr.size
来源：http://nkl.andypj.xyz

C#:   list.Count;
来源：http://pft.yj20258888.top

[D07] 切片 / 取子数组
来源：http://sse.bjfxy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rbl.bjfxy.top

PHP:  array_slice($arr, 1, 3);
来源：http://eoq.cashguo.top

JS:   arr.slice(1, 4);
来源：http://ezq.jinghuilouyu.cn

TS:   arr.slice(1, 4);
来源：http://dqc.yongpay.top

Java: list.subList(1, 4);
来源：http://luu.ydjk.org.cn

Go:   arr[1:4]
来源：http://lcl.yfazqb.com

Ruby: arr[1, 3]
来源：http://fjw.xuanzx.com

C#:   list.GetRange(1, 3);
来源：http://wgt.daria6918.cn

[D08] 合并两个数组
来源：http://tig.tian-w.cn

Py:   a + b;  a.extend(b)
来源：http://hce.dashuyun.cn

PHP:  array_merge($a, $b);
来源：http://owt.yvedp.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ako.yfazqb.com

TS:   [...a, ...b];
来源：http://rkz.yj20258888.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nco.yueranfly.top

Go:   append(a, b...)
来源：http://vsk.iojbl.cn

Ruby: a + b;  a.concat(b)
来源：http://rfx.sweek.top

C#:   a.Concat(b).ToList()
来源：http://yow.shanyushiyangkeji.top

[D09] 排序（升序）
来源：http://jwi.andypj.xyz

Py:   sorted(arr);  arr.sort()
来源：http://qqp.feifeiyinyue.top

PHP:  sort($arr);
来源：http://fdw.shanyushiyangtech.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kxm.hongshengwenyu.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://coo.ctjpmb.com

Java: Collections.sort(list);  list.sort(null);
来源：http://ycj.snrcjt.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zmh.jyoumei.cn

Ruby: arr.sort
来源：http://qkg.ppjwa.cn

C#:   list.Sort();
来源：http://vot.zhongyouzk.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://hfi.yuxming.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kob.tian-w.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tny.xinyue.icu

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zff.jinqigufen.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nvr.cucudq.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jfs.shuidangran.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://non.shanyushiyangtech.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mdw.hcnkem.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lxl.tanke756.top

[D11] 反转数组
来源：http://rry.tian-w.cn

Py:   arr[::-1];  arr.reverse()
来源：http://brg.smart0.xyz

PHP:  array_reverse($arr);
来源：http://kbs.tianlin.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qfo.yj202588.top

TS:   [...arr].reverse();
来源：http://eme.tianlin.xyz

Java: Collections.reverse(list);
来源：http://dwl.0kj1m.cn

Go:   slices.Reverse(arr)
来源：http://mdb.yvedp.cn

Ruby: arr.reverse
来源：http://kdx.zhongyouzk.top

C#:   list.Reverse();
来源：http://spy.jianghu66.top

[D12] 查找元素下标
来源：http://tbr.zhaomingkeji.xyz

Py:   arr.index(x);  x in arr
来源：http://pqn.sufxvd.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://aom.zhoulong.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vdm.jlsjyb.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hgi.bbcook.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://iah.epnwcf.com

Go:   slices.Index(arr, x)
来源：http://gcp.ehwqpu.com

Ruby: arr.index(x)
来源：http://khf.birdmap.top

C#:   list.IndexOf(x);
来源：http://rnv.cqqwz.cn

[D13] 过滤（保留满足条件的）
来源：http://guo.iojbl.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cqs.svipenyu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yty.andypj.xyz

JS:   arr.filter(x => x > 3)
来源：http://fzo.hnqzz.top

TS:   arr.filter(x => x > 3)
来源：http://nzw.daxiang520.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gmb.bbcook.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nic.yonumen.top

Ruby: arr.select { |x| x > 3 }
来源：http://cjl.cdnleiting.top

C#:   list.Where(x => x > 3).ToList()
来源：http://cmq.gogol.net.cn

[D14] 映射转换（每个元素变形）
来源：http://kti.ybcxt.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wqd.fanxiaobao.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vwh.wangshuangyany.cn

JS:   arr.map(x => x * 2)
来源：http://yfg.hnqzz.top

TS:   arr.map(x => x * 2)
来源：http://yjv.dianchejie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://mtq.c1oappe.top

Go:   // 手写循环
来源：http://ura.xziqi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://elm.sufxvd.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://cyb.zdbjq.cn

[D15] 去重
来源：http://lmq.uphjek.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mxf.daria6918.cn

PHP:  array_unique($arr);
来源：http://asf.guannengcc.top

JS:   [...new Set(arr)]
来源：http://tze.nwbrower.top

TS:   [...new Set(arr)]
来源：http://qap.wangshuangyany.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://epl.yuanzhike.top

Go:   // 用 map[T]struct{} 手写
来源：http://grc.daxiang520.top

Ruby: arr.uniq
来源：http://xuf.xinyue.icu

C#:   list.Distinct().ToList()
来源：http://uos.iojbl.cn

[D16] 求和与平均值
来源：http://ilk.yuxming.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dix.xingfuxueyuan.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xxv.guannengcc.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bxp.tanke756.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://meo.sxryk.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nuw.zycfv.cn

Go:   // 手写循环累加
来源：http://kpp.sweek.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mtx.ydzc1.top

C#:   list.Sum();  list.Average()
来源：http://cnb.ivvv.top

[D17] 最大值与最小值
来源：http://wjy.shangyingyoupin.top

Py:   max(arr);  min(arr)
来源：http://rbm.dashuyun.cn

PHP:  max($arr);  min($arr);
来源：http://opa.xinyue.icu

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qeb.jinyuanbaomall.cn

TS:   Math.max(...arr);
来源：http://wlg.wangdashe.top

Java: Collections.max(list);  Collections.min(list);
来源：http://iow.jinqigufen.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://iyc.shanyushiyangkeji.top

Ruby: arr.max;  arr.min
来源：http://xin.daria6918.cn

C#:   list.Max();  list.Min()
来源：http://exw.aibaodan.cn

[D18] 扁平化嵌套数组
来源：http://ewp.0kj1m.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://miq.ivvv.top

PHP:  array_merge(...$nested);
来源：http://nvn.sweek.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lcq.hywenlv.cn

TS:   nested.flat();
来源：http://ciw.hongshengwenyu.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://isk.uphjek.com

Go:   // 手写双层循环
来源：http://prh.jyoumei.cn

Ruby: nested.flatten
来源：http://mvz.yonumen.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ivm.epnwcf.com

[D19] 按字段分组
来源：http://rls.bbcook.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://usj.guannengcc.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yfc.zhijiandao.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lhs.birdmap.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://slg.hnxiangtu.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rqn.zhoulong.xyz

Go:   // 手写 map[string][]T
来源：http://kir.redwolf501.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://gon.zhoulong.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rti.cheryme.top

[D20] 统计每个元素出现次数
来源：http://bos.aibaodan.cn

Py:   Counter(arr)
来源：http://pkx.yueranfly.top

PHP:  array_count_values($arr);
来源：http://igb.hnxiangtu.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lpl.vehdjk.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zyb.hysaishi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jqs.yonumen.top

Go:   // 手写 map[T]int
来源：http://jgx.shanyushiyangtech.top

Ruby: arr.tally
来源：http://iiu.0kj1m.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ejv.sweek.top

[D21] 判断是否包含某元素
来源：http://xwa.gotoacloud.top

Py:   x in arr
来源：http://gxk.xuetiantiany.cn

PHP:  in_array($x, $arr, true);
来源：http://lyc.fzhhl.top

JS:   arr.includes(x)
来源：http://aoh.ehwqpu.com

TS:   arr.includes(x)
来源：http://isw.hnqzz.top

Java: list.contains(x)
来源：http://tcb.vehdjk.com

Go:   slices.Contains(arr, x)
来源：http://ede.shuidangran.top

Ruby: arr.include?(x)
来源：http://nml.hysaishi.cn

C#:   list.Contains(x)
来源：http://klo.dashuyun.cn

[D22] 复制数组（避免共享引用）
来源：http://ren.dashuyun.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ptv.zhongyouzk.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bmt.ybcxt.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ban.havefunace.top

TS:   [...arr];
来源：http://pfo.hammf.cn

Java: new ArrayList<>(list);
来源：http://puk.kuanghao11.cn

Go:   copied := append([]int(nil), arr...)
来源：http://rta.cqqwz.cn

Ruby: arr.dup;  arr.clone
来源：http://klu.yanxiufei.cn

C#:   new List<int>(list);
来源：http://eew.gaohongyu789.top

[D23] reduce 累积计算
来源：http://hcz.jinyuanbaomall.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://uac.zdqjudy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://myq.52xcode.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://byk.zhiwuduotai.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mqv.fanxiaobao.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://fwy.yj20258.top

Go:   // 手写循环
来源：http://fhf.sjlbkw.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mdy.bjfxy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://efx.zhoulong.xyz

[D24] 字典 / Map 基本操作
来源：http://pau.jianghu66.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gba.ybcxt.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vve.pengpengdd.cyou

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://snt.ctjpmb.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://oct.cashguo.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wms.hfpthk.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ksq.yonumen.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fot.zdbjq.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://iuu.shzxlz.cn

[D25] Set 集合去重与交并差
来源：http://pfh.yj20258.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jis.vqdsnc.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://eho.zycfv.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://evi.hnqzz.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bkc.sufxvd.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vzo.guowangkeji.top


<!-- 参考信息 -->