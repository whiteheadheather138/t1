代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://sys.xingfuxueyuan.xyz

C#:   using System.Text;
来源：http://lyh.hongshengwenyu.top

[C12] 立即执行函数 IIFE
来源：http://bfl.hnxiangtu.top

Py:   (lambda: print("run"))()
来源：http://cbt.yuanzhike.top

PHP:  (function () { echo "run"; })();
来源：http://mfx.ehwqpu.com

JS:   (() => { console.log("run"); })();
来源：http://sec.yuanzhike.top

TS:   (() => { console.log("run"); })();
来源：http://usd.jinyuanbaomall.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://buj.wangdashe.top

Go:   func() { fmt.Println("run") }()
来源：http://buh.zdbjq.cn

Ruby: -> { puts "run" }.call
来源：http://wga.hnqzz.top

C#:   // 无 IIFE：用静态构造函数
来源：http://knc.hnxiangtu.top

[C13] 类型声明 / 类型注解
来源：http://zxh.xuanzx.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vej.ywan-chungtsiang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://edx.hysaishi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rip.daxiang520.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kkm.jinghuilouyu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://nlv.xuetiantiany.cn

Go:   func add(a, b int) int
来源：http://emk.svipenyu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://aht.sufxvd.cn

C#:   int Add(int a, int b) => a + b;
来源：http://uyn.jyoumei.cn

[C14] 泛型函数
来源：http://tzv.hcnkem.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vtd.yfazqb.com

PHP:  // 无泛型
来源：http://ebf.shangyingyoupin.top

JS:   // 无泛型
来源：http://soq.zhaomingkeji.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vxt.zhongyouzk.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ute.fehbvm.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jan.bjfxy.top

Ruby: # 无泛型
来源：http://dyr.xinyue.icu

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qsa.yangfankeji.com

[C15] 解构 / 展开参数
来源：http://hlv.sjlbkw.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://eii.bjfxy.top

PHP:  [$a, $b] = $pair;
来源：http://lkn.xuanzx.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lgm.ppjwa.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uvf.yuanzhike.top

Java: // 无解构
来源：http://nam.yueranfly.top

Go:   // 无解构
来源：http://cgp.jinyuanbaomall.cn

Ruby: a, b = pair
来源：http://baf.sysykeji.top

C#:   var (a, b) = pair;
来源：http://tck.vehdjk.com

[C16] 函数 / 方法重载
来源：http://cgi.gogol.net.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dbi.jianghu66.top

PHP:  // 无重载
来源：http://rfn.ivvv.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://fbr.sjlbkw.cn

TS:   // 用联合类型或重载签名声明
来源：http://zij.jianghu66.top

Java: void f(int a) {}  void f(String a) {}
来源：http://kdh.kuanghao11.cn

Go:   // 无重载：用不同函数名
来源：http://nso.yueranfly.top

Ruby: # 无重载：靠动态参数
来源：http://jdr.hysaishi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://rae.guowangkeji.top

================================================================================
来源：http://xsq.cashguo.top

D. 数组 / 列表 / 集合
来源：http://guk.ydjk.org.cn

================================================================================
来源：http://pdo.yuxming.cn

[D01] 创建数组 / 列表
来源：http://ppq.yanxiufei.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://rgg.pengpengdd.cyou

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dkn.mhx1999.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fvm.jinghuilouyu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ebv.jqgufenzy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mgl.ywan-chungtsiang.top

Go:   arr := []int{1, 2, 3}
来源：http://suo.kuanghao11.cn

Ruby: arr = [1, 2, 3]
来源：http://myp.fengsongda.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ebm.xuetiantiany.cn

[D02] 追加元素到末尾
来源：http://jtt.yanxiufei.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gzf.cqqwz.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jgz.zhaomingkeji.xyz

JS:   arr.push(4);
来源：http://acp.tanke756.top

TS:   arr.push(4);
来源：http://wvv.dashuyun.cn

Java: list.add(4);
来源：http://evk.yanxiufei.cn

Go:   arr = append(arr, 4)
来源：http://wei.ywan-chungtsiang.top

Ruby: arr << 4; arr.push(5)
来源：http://wss.yvedp.cn

C#:   list.Add(4);
来源：http://mzw.shzxlz.cn

[D03] 在指定位置插入元素
来源：http://tdn.aibaodan.cn

Py:   arr.insert(0, 0)
来源：http://jgu.52xcode.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://men.wangshuangyany.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qjb.vqdsnc.cn

TS:   arr.splice(0, 0, 0);
来源：http://hno.ywan-chungtsiang.top

Java: list.add(0, 0);
来源：http://ivb.ybcxt.top

Go:   arr = append([]int{0}, arr...)
来源：http://jnv.tian-w.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uuj.jqgfzy.top

C#:   list.Insert(0, 0);
来源：http://iab.daria6918.cn

[D04] 删除元素
来源：http://imp.0kj1m.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pmm.guannengcc.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baq.cheryme.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ruk.cqqwz.cn

TS:   arr.splice(0, 1);
来源：http://chh.hongshengwenyu.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tka.52xcode.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://laj.ctjpmb.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lit.zhongyouzk.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fhx.sxryk.cn

[D05] 访问与修改元素
来源：http://byo.cdnleiting.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ncp.chenzaomai.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cbk.quarkkingdee.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ocl.xuetiantiany.cn

TS:   arr[0]; arr.at(-1);
来源：http://jbz.smart0.xyz

Java: list.get(0); list.set(0, 9);
来源：http://cmw.jiagoushi.top

Go:   arr[0]; arr[0] = 9
来源：http://mcj.52xcode.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tmh.cheryme.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zuf.yonumen.top

[D06] 数组长度
来源：http://zjz.nwbrower.top

Py:   len(arr)
来源：http://opb.zycfv.cn

PHP:  count($arr);
来源：http://phi.shangyingyoupin.top

JS:   arr.length
来源：http://sla.zycfv.cn

TS:   arr.length
来源：http://ski.yfazqb.com

Java: list.size();
来源：http://omy.yonumen.top

Go:   len(arr)
来源：http://hvg.uphjek.com

Ruby: arr.length; arr.size
来源：http://bls.yanxiufei.cn

C#:   list.Count;
来源：http://jyu.ivvv.top

[D07] 切片 / 取子数组
来源：http://iqu.dashuyun.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mct.gaohongyu789.top

PHP:  array_slice($arr, 1, 3);
来源：http://elm.chenzaomai.com

JS:   arr.slice(1, 4);
来源：http://emx.fzhhl.top

TS:   arr.slice(1, 4);
来源：http://xup.fengsongda.top

Java: list.subList(1, 4);
来源：http://ivt.316326.xyz

Go:   arr[1:4]
来源：http://hwh.dianchejie.cn

Ruby: arr[1, 3]
来源：http://dca.hysaishi.cn

C#:   list.GetRange(1, 3);
来源：http://sck.shzxlz.cn

[D08] 合并两个数组
来源：http://ivc.jqgufenzy.top

Py:   a + b;  a.extend(b)
来源：http://jtu.fengsongda.top

PHP:  array_merge($a, $b);
来源：http://htg.iojbl.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ved.xinyue.icu

TS:   [...a, ...b];
来源：http://fbe.zhiwuduotai.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hmm.ydzc1.top

Go:   append(a, b...)
来源：http://lbt.shanyushiyangkeji.top

Ruby: a + b;  a.concat(b)
来源：http://oyb.yonumen.top

C#:   a.Concat(b).ToList()
来源：http://dhb.gogol.net.cn

[D09] 排序（升序）
来源：http://cyr.yueranfly.top

Py:   sorted(arr);  arr.sort()
来源：http://cgr.andypj.xyz

PHP:  sort($arr);
来源：http://qdt.vehdjk.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rdv.ppjwa.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://yvq.snrcjt.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://kcc.ywan-chungtsiang.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vsv.wangshuangyany.cn

Ruby: arr.sort
来源：http://fpb.jinyuanbaomall.cn

C#:   list.Sort();
来源：http://ige.xuanzx.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://pdg.fktsv.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://usp.zhoulong.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://olt.zhijiandao.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mni.cqqwz.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nlk.yfazqb.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ucs.ydzc1.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qto.zhijiandao.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gzf.shanyushiyangkeji.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tja.yangfankeji.com

[D11] 反转数组
来源：http://jue.jqgufenzy.top

Py:   arr[::-1];  arr.reverse()
来源：http://yyw.iojbl.cn

PHP:  array_reverse($arr);
来源：http://cwi.316326.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yih.gogol.net.cn

TS:   [...arr].reverse();
来源：http://nnq.dianchejie.cn

Java: Collections.reverse(list);
来源：http://flm.0kj1m.cn

Go:   slices.Reverse(arr)
来源：http://zxu.hammf.cn

Ruby: arr.reverse
来源：http://wgx.shzxlz.cn

C#:   list.Reverse();
来源：http://ihi.jiagoushi.top

[D12] 查找元素下标
来源：http://urc.cdnleiting.top

Py:   arr.index(x);  x in arr
来源：http://beb.iojbl.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qap.jianghu66.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://phz.52xcode.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ytg.ehwqpu.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://flp.xuanzx.com

Go:   slices.Index(arr, x)
来源：http://vox.ydzc1.top

Ruby: arr.index(x)
来源：http://kxp.hnqzz.top

C#:   list.IndexOf(x);
来源：http://hja.yuxming.cn

[D13] 过滤（保留满足条件的）
来源：http://xys.jqgfzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://iwj.hongshengwenyu.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qse.iojbl.cn

JS:   arr.filter(x => x > 3)
来源：http://mdl.zhengqikj.top

TS:   arr.filter(x => x > 3)
来源：http://hrx.yuanzhike.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lhg.ppjwa.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ggq.xylfe.cn

Ruby: arr.select { |x| x > 3 }
来源：http://pxv.zdbjq.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://tzm.snrcjt.cn

[D14] 映射转换（每个元素变形）
来源：http://qez.dashuyun.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hyg.svipenyu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://uws.quarkkingdee.top

JS:   arr.map(x => x * 2)
来源：http://fil.shanyushiyangkeji.top

TS:   arr.map(x => x * 2)
来源：http://wfr.fktsv.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://jed.jianghu66.top

Go:   // 手写循环
来源：http://art.sjlbkw.cn

Ruby: arr.map { |x| x * 2 }
来源：http://plz.jqgfzy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://hjc.daria6918.cn

[D15] 去重
来源：http://uik.tanke756.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hsu.gotoacloud.top

PHP:  array_unique($arr);
来源：http://scz.hnqzz.top

JS:   [...new Set(arr)]
来源：http://qcx.wangdashe.top

TS:   [...new Set(arr)]
来源：http://rmo.gotoacloud.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ork.jqgfzy.top

Go:   // 用 map[T]struct{} 手写
来源：http://wvb.jinqigufen.top

Ruby: arr.uniq
来源：http://ddw.havefunace.top

C#:   list.Distinct().ToList()
来源：http://mbr.dianchejie.cn

[D16] 求和与平均值
来源：http://cfv.jinghuilouyu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hsi.zycfv.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zon.haohaochexian.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cuk.ywan-chungtsiang.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://znc.yongpay.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vfk.yueranfly.top

Go:   // 手写循环累加
来源：http://nrg.sysykeji.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nlf.jqgfzy.top

C#:   list.Sum();  list.Average()
来源：http://jiq.fengsongda.top

[D17] 最大值与最小值
来源：http://bzm.wangshuangyany.cn

Py:   max(arr);  min(arr)
来源：http://ouu.gotoacloud.top

PHP:  max($arr);  min($arr);
来源：http://rsy.xinyue.icu

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ppw.uphjek.com

TS:   Math.max(...arr);
来源：http://boy.zhiwuduotai.top

Java: Collections.max(list);  Collections.min(list);
来源：http://qjc.yj20258888.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bwn.c1oappe.top

Ruby: arr.max;  arr.min
来源：http://chw.zhijiandao.cn

C#:   list.Max();  list.Min()
来源：http://bgg.ivvv.top

[D18] 扁平化嵌套数组
来源：http://lji.gzhubu.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ofn.vqdsnc.cn

PHP:  array_merge(...$nested);
来源：http://ujx.yonumen.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://abx.52xcode.cn

TS:   nested.flat();
来源：http://btv.zycfv.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rjb.fehbvm.com

Go:   // 手写双层循环
来源：http://qds.smart0.xyz

Ruby: nested.flatten
来源：http://yrh.sxryk.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xqu.zhaomingkeji.xyz

[D19] 按字段分组
来源：http://fjv.hnqzz.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://aeb.sxryk.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bru.shanyushiyangkeji.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ywe.zhoulong.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://syf.ywan-chungtsiang.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://epe.hywenlv.cn

Go:   // 手写 map[string][]T
来源：http://tdu.sufxvd.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://mim.xuanzx.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://iyi.xuanzx.com

[D20] 统计每个元素出现次数
来源：http://qlv.zhiwuduotai.top

Py:   Counter(arr)
来源：http://btc.svipenyu.cn

PHP:  array_count_values($arr);
来源：http://qim.kuanghao11.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wcb.mhx1999.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uck.zhixingplan.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tqo.shanyushiyangtech.top

Go:   // 手写 map[T]int
来源：http://lol.ehwqpu.com

Ruby: arr.tally
来源：http://qfv.gogol.net.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kyg.c1oappe.top

[D21] 判断是否包含某元素
来源：http://gxw.feifeiyinyue.top

Py:   x in arr
来源：http://vsj.xylfe.cn

PHP:  in_array($x, $arr, true);
来源：http://pxe.yuxming.cn

JS:   arr.includes(x)
来源：http://bgq.vehdjk.com

TS:   arr.includes(x)
来源：http://lpl.cucudq.cn

Java: list.contains(x)
来源：http://ipe.havefunace.top

Go:   slices.Contains(arr, x)
来源：http://mae.dashuyun.cn

Ruby: arr.include?(x)
来源：http://nej.zdqjudy.top

C#:   list.Contains(x)
来源：http://svy.hfpthk.cn

[D22] 复制数组（避免共享引用）
来源：http://fji.pycfn.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rgf.cdnleiting.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qnu.hfpthk.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dnf.nanxuanxn.top

TS:   [...arr];
来源：http://hhl.hammf.cn

Java: new ArrayList<>(list);
来源：http://rhi.uphjek.com

Go:   copied := append([]int(nil), arr...)
来源：http://bng.zhijiandao.cn

Ruby: arr.dup;  arr.clone
来源：http://epn.tianlin.xyz

C#:   new List<int>(list);
来源：http://uzu.jinghuilouyu.cn

[D23] reduce 累积计算
来源：http://xyq.zhoulong.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://eah.xuanzx.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xyw.ctjpmb.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bts.fktsv.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fsx.jqgufenzy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://siw.zhoulong.xyz

Go:   // 手写循环
来源：http://rvz.yanxiufei.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://btm.zdbjq.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://puz.fanxiaobao.xyz

[D24] 字典 / Map 基本操作
来源：http://kte.wangdashe.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wbw.snrcjt.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wnz.yfazqb.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bdu.snrcjt.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jpm.yfazqb.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xkc.feifeiyinyue.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xgt.zhaomingkeji.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bzd.mhx1999.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gov.ctjpmb.com

[D25] Set 集合去重与交并差
来源：http://iec.snrcjt.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://crq.ctjpmb.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sxl.quarkkingdee.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ycb.tian-w.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jhu.ybcxt.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bpd.mhx1999.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qvk.yvedp.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gio.jinyuanbaomall.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cei.andypj.xyz

[D26] 数组转字符串
来源：http://ssr.yj20258888.top

Py:   ", ".join(map(str, arr))
来源：http://lxo.bbcook.cn

PHP:  implode(", ", $arr);
来源：http://vra.yfazqb.com

JS:   arr.join(", ")
来源：http://twg.dashuyun.cn

TS:   arr.join(", ")
来源：http://epf.ybcxt.top

Java: String.join(", ", list)
来源：http://eje.ydzc1.top

Go:   strings.Join(strs, ", ")
来源：http://vrz.jinqigufen.top

Ruby: arr.join(", ")
来源：http://apm.yfazqb.com

C#:   string.Join(", ", list)
来源：http://eik.yj202588.top

================================================================================
来源：http://zgv.tarul.cn

E. 字符串处理
来源：http://ejo.chenjidiqi.icu

================================================================================
来源：http://csm.ivvv.top

[E01] 拼接字符串
来源：http://rrl.guowangkeji.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rph.xylfe.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qtp.chenzaomai.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://sgu.sufxvd.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hwu.hysaishi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ose.zhaomingkeji.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fdw.shangyingyoupin.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sqb.ivvv.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rax.guannengcc.top

[E02] 重复字符串
来源：http://xct.redwolf501.top

Py:   "ab" * 3
来源：http://yse.c1oappe.top

PHP:  str_repeat("ab", 3);
来源：http://fcr.jianghu66.top

JS:   "ab".repeat(3)
来源：http://ybf.haohaochexian.top


<!-- 参考信息 -->