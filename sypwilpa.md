代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://rus.shangyingyoupin.top

Ruby: -> { puts "run" }.call
来源：http://zoi.tianlin.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://iuw.wangshuangyany.cn

[C13] 类型声明 / 类型注解
来源：http://pfx.fehbvm.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gdc.fengsongda.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mku.zhaomingkeji.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zaa.xinyue.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://koc.yueranfly.top

Java: int add(int a, int b) { return a + b; }
来源：http://gph.hongshengwenyu.top

Go:   func add(a, b int) int
来源：http://ulq.nanxuanxn.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qyt.nanxuanxn.top

C#:   int Add(int a, int b) => a + b;
来源：http://tat.ybcxt.top

[C14] 泛型函数
来源：http://opd.zhijiandao.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kbq.zycfv.cn

PHP:  // 无泛型
来源：http://vlw.nanxinkj.top

JS:   // 无泛型
来源：http://dha.hysaishi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dcp.pycfn.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wjn.chenlongwang.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://guq.yonumen.top

Ruby: # 无泛型
来源：http://ndp.xuetiantiany.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kmc.yonumen.top

[C15] 解构 / 展开参数
来源：http://bjt.quarkkingdee.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dpz.jqgufenzy.top

PHP:  [$a, $b] = $pair;
来源：http://ekl.pycfn.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wja.andypj.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gal.zhaomingkeji.xyz

Java: // 无解构
来源：http://bbw.shanyushiyangkeji.top

Go:   // 无解构
来源：http://rny.bbcook.cn

Ruby: a, b = pair
来源：http://fcy.shuidangran.top

C#:   var (a, b) = pair;
来源：http://fyf.gaohongyu789.top

[C16] 函数 / 方法重载
来源：http://qqi.c1oappe.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://lsh.ydjk.org.cn

PHP:  // 无重载
来源：http://bvz.9152youxi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://emc.svipenyu.cn

TS:   // 用联合类型或重载签名声明
来源：http://tkd.jqgfzy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://tpn.hywenlv.cn

Go:   // 无重载：用不同函数名
来源：http://hyd.sweek.top

Ruby: # 无重载：靠动态参数
来源：http://sna.jinghuilouyu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://spt.xuanzx.com

================================================================================
来源：http://bqg.jyoumei.cn

D. 数组 / 列表 / 集合
来源：http://nbs.zhoulong.xyz

================================================================================
来源：http://xym.jyoumei.cn

[D01] 创建数组 / 列表
来源：http://ysb.hysaishi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://kog.sysykeji.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pxq.vehdjk.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://eck.sjlbkw.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://gil.hongshengwenyu.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ayi.fanxiaobao.xyz

Go:   arr := []int{1, 2, 3}
来源：http://zev.fktsv.cn

Ruby: arr = [1, 2, 3]
来源：http://mfv.yongpay.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://eja.jlsjyb.cn

[D02] 追加元素到末尾
来源：http://kmj.yvedp.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://iwj.nwbrower.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lbq.xylfe.cn

JS:   arr.push(4);
来源：http://zwh.guannengcc.top

TS:   arr.push(4);
来源：http://dmd.pengpengdd.cyou

Java: list.add(4);
来源：http://euk.hongshengwenyu.top

Go:   arr = append(arr, 4)
来源：http://mkb.svipenyu.cn

Ruby: arr << 4; arr.push(5)
来源：http://sib.chenjidiqi.icu

C#:   list.Add(4);
来源：http://ujl.wangdashe.top

[D03] 在指定位置插入元素
来源：http://mdi.shanyushiyangkeji.top

Py:   arr.insert(0, 0)
来源：http://zsn.smart0.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ugl.guannengcc.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jue.hywenlv.cn

TS:   arr.splice(0, 0, 0);
来源：http://zvb.jqgufenzy.top

Java: list.add(0, 0);
来源：http://fgr.jinyuanbaomall.cn

Go:   arr = append([]int{0}, arr...)
来源：http://lkx.jianghu66.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://otw.ydzc1.top

C#:   list.Insert(0, 0);
来源：http://dhz.ydzc1.top

[D04] 删除元素
来源：http://isf.birdmap.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://anb.daria6918.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://aou.fanxiaobao.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lta.ydjk.org.cn

TS:   arr.splice(0, 1);
来源：http://dkp.yueranfly.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ubm.shanyushiyangtech.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ycs.kuanghao11.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://omk.ppjwa.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gag.snrcjt.cn

[D05] 访问与修改元素
来源：http://acs.hnqzz.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mku.birdmap.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://neh.aizwys.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pff.sweek.top

TS:   arr[0]; arr.at(-1);
来源：http://iqw.ydjk.org.cn

Java: list.get(0); list.set(0, 9);
来源：http://dgp.bbcook.cn

Go:   arr[0]; arr[0] = 9
来源：http://rto.fehbvm.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ezf.sysykeji.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jxw.sxryk.cn

[D06] 数组长度
来源：http://cqu.yj202588.top

Py:   len(arr)
来源：http://ogw.yfazqb.com

PHP:  count($arr);
来源：http://mqy.yuxming.cn

JS:   arr.length
来源：http://yvw.ivvv.top

TS:   arr.length
来源：http://pkm.sysykeji.top

Java: list.size();
来源：http://zum.0kj1m.cn

Go:   len(arr)
来源：http://rjw.jqgufenzy.top

Ruby: arr.length; arr.size
来源：http://liz.xziqi.cn

C#:   list.Count;
来源：http://lwz.birdmap.top

[D07] 切片 / 取子数组
来源：http://nag.xziqi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rdq.zhaomingkeji.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://adt.jinghuilouyu.cn

JS:   arr.slice(1, 4);
来源：http://juy.ctjpmb.com

TS:   arr.slice(1, 4);
来源：http://ili.ywan-chungtsiang.top

Java: list.subList(1, 4);
来源：http://biv.zhijiandao.cn

Go:   arr[1:4]
来源：http://ykh.chenlongwang.top

Ruby: arr[1, 3]
来源：http://wsb.ctjpmb.com

C#:   list.GetRange(1, 3);
来源：http://tvm.pycfn.com

[D08] 合并两个数组
来源：http://suv.shanyushiyangtech.top

Py:   a + b;  a.extend(b)
来源：http://muk.snrcjt.cn

PHP:  array_merge($a, $b);
来源：http://vts.meibo888.top

JS:   [...a, ...b];  a.concat(b);
来源：http://las.vqdsnc.cn

TS:   [...a, ...b];
来源：http://koe.pengpengdd.cyou

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://esl.ehwqpu.com

Go:   append(a, b...)
来源：http://kxw.0kj1m.cn

Ruby: a + b;  a.concat(b)
来源：http://zcf.hysaishi.cn

C#:   a.Concat(b).ToList()
来源：http://aqf.daxiang520.top

[D09] 排序（升序）
来源：http://zdm.tanke756.top

Py:   sorted(arr);  arr.sort()
来源：http://ear.yongpay.top

PHP:  sort($arr);
来源：http://ctc.gaohongyu789.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://roa.zdqjudy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://qbf.yangfankeji.com

Java: Collections.sort(list);  list.sort(null);
来源：http://skw.zhoulong.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://iyx.hammf.cn

Ruby: arr.sort
来源：http://vbu.nanxinkj.top

C#:   list.Sort();
来源：http://eyj.hcnkem.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://fvw.epnwcf.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hjs.kuanghao11.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mer.yonumen.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xju.smart0.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ned.haohaochexian.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dwf.yj20258.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mjn.andypj.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vyw.52xcode.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://djf.c1oappe.top

[D11] 反转数组
来源：http://zlc.fanxiaobao.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://fph.quarkkingdee.top

PHP:  array_reverse($arr);
来源：http://rnr.52xcode.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jhd.gaohongyu789.top

TS:   [...arr].reverse();
来源：http://div.52xcode.cn

Java: Collections.reverse(list);
来源：http://pwo.gzhubu.top

Go:   slices.Reverse(arr)
来源：http://obt.yj202588.top

Ruby: arr.reverse
来源：http://gpv.yvedp.cn

C#:   list.Reverse();
来源：http://bie.jlsjyb.cn

[D12] 查找元素下标
来源：http://xqn.hfpthk.cn

Py:   arr.index(x);  x in arr
来源：http://klu.redwolf501.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uka.shanyushiyangtech.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bct.zhoulong.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rfo.hcnkem.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qwa.gzhubu.top

Go:   slices.Index(arr, x)
来源：http://zgp.zhengqikj.top

Ruby: arr.index(x)
来源：http://oav.epnwcf.com

C#:   list.IndexOf(x);
来源：http://ebp.jinqigfzy.top

[D13] 过滤（保留满足条件的）
来源：http://tec.andypj.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rdo.xuetiantiany.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kid.jyoumei.cn

JS:   arr.filter(x => x > 3)
来源：http://fhz.jqgufenzy.top

TS:   arr.filter(x => x > 3)
来源：http://gwf.0kj1m.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://csh.sufxvd.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lyp.52xcode.cn

Ruby: arr.select { |x| x > 3 }
来源：http://wwo.cucudq.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://jtg.zhengqikj.top

[D14] 映射转换（每个元素变形）
来源：http://xme.dianchejie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://sxs.zhengqikj.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://irc.yueranfly.top

JS:   arr.map(x => x * 2)
来源：http://kxv.yj20258.top

TS:   arr.map(x => x * 2)
来源：http://mth.ybcxt.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ztz.svipenyu.cn

Go:   // 手写循环
来源：http://gbj.hysaishi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://dhb.xylfe.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xdj.52xcode.cn

[D15] 去重
来源：http://gqw.jinqigfzy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qvc.xuetiantiany.cn

PHP:  array_unique($arr);
来源：http://lad.zhongyouzk.top

JS:   [...new Set(arr)]
来源：http://yzg.smart0.xyz

TS:   [...new Set(arr)]
来源：http://nnk.andypj.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mde.hesvh.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ahi.ctjpmb.com

Ruby: arr.uniq
来源：http://hsb.yangfankeji.com

C#:   list.Distinct().ToList()
来源：http://rdq.fengsongda.top

[D16] 求和与平均值
来源：http://cif.ivvv.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vse.gzhubu.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vjy.ydzc1.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ymj.fktsv.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gcs.haohaochexian.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fjy.birdmap.top

Go:   // 手写循环累加
来源：http://wis.xingfuxueyuan.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wbz.xuetiantiany.cn

C#:   list.Sum();  list.Average()
来源：http://nre.kuanghao11.cn

[D17] 最大值与最小值
来源：http://zdq.wangdashe.top

Py:   max(arr);  min(arr)
来源：http://zhh.sxryk.cn

PHP:  max($arr);  min($arr);
来源：http://wzr.hongshengwenyu.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://oyd.shuidangran.top

TS:   Math.max(...arr);
来源：http://zhh.yongpay.top

Java: Collections.max(list);  Collections.min(list);
来源：http://bht.mhx1999.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bdl.yvedp.cn

Ruby: arr.max;  arr.min
来源：http://yyc.yvedp.cn

C#:   list.Max();  list.Min()
来源：http://leb.nwbrower.top

[D18] 扁平化嵌套数组
来源：http://efr.kuanghao11.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://uwd.ydjk.org.cn

PHP:  array_merge(...$nested);
来源：http://pgi.jqgfzy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xak.0kj1m.cn

TS:   nested.flat();
来源：http://qmn.ydzc1.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vtz.dashuyun.cn

Go:   // 手写双层循环
来源：http://ppi.zhaomingkeji.xyz

Ruby: nested.flatten
来源：http://nmz.zhongyouzk.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ulp.cdnleiting.top

[D19] 按字段分组
来源：http://wep.nanxuanxn.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://aod.ybcxt.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jij.guannengcc.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zhl.fanxiaobao.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://twv.yongpay.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://crz.shzxlz.cn

Go:   // 手写 map[string][]T
来源：http://uhc.yongpay.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://tdp.hongshengwenyu.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pnh.chenjidiqi.icu

[D20] 统计每个元素出现次数
来源：http://kmh.zhixingplan.top

Py:   Counter(arr)
来源：http://fqr.mhx1999.top

PHP:  array_count_values($arr);
来源：http://gle.iojbl.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wvo.jqgufenzy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rdu.jinqigufen.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://uux.bjfxy.top

Go:   // 手写 map[T]int
来源：http://wom.xylfe.cn

Ruby: arr.tally
来源：http://zcq.jianghu66.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yck.quarkkingdee.top

[D21] 判断是否包含某元素
来源：http://ozt.xingfuxueyuan.xyz

Py:   x in arr
来源：http://iad.jlsjyb.cn

PHP:  in_array($x, $arr, true);
来源：http://cxp.gzhubu.top

JS:   arr.includes(x)
来源：http://qps.shzxlz.cn

TS:   arr.includes(x)
来源：http://qsn.ywan-chungtsiang.top

Java: list.contains(x)
来源：http://hph.smart0.xyz

Go:   slices.Contains(arr, x)
来源：http://ryu.hcnkem.com

Ruby: arr.include?(x)
来源：http://apw.xingfuxueyuan.xyz

C#:   list.Contains(x)
来源：http://okj.feifeiyinyue.top

[D22] 复制数组（避免共享引用）
来源：http://fxj.316326.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fej.yj202588.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xgn.uphjek.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pyi.shuidangran.top

TS:   [...arr];
来源：http://tlb.ywan-chungtsiang.top

Java: new ArrayList<>(list);
来源：http://ixb.haohaochexian.top

Go:   copied := append([]int(nil), arr...)
来源：http://ihv.daria6918.cn

Ruby: arr.dup;  arr.clone
来源：http://bxu.smart0.xyz

C#:   new List<int>(list);
来源：http://umv.ybcxt.top

[D23] reduce 累积计算
来源：http://atb.shanyushiyangtech.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rkp.tian-w.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jeq.mhx1999.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tbq.xylfe.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sxh.yj20258.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://kda.bbcook.cn

Go:   // 手写循环
来源：http://luw.xingfuxueyuan.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yng.chenzaomai.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xhb.daria6918.cn

[D24] 字典 / Map 基本操作
来源：http://gqa.haohaochexian.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kgw.cucudq.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vwd.yangfankeji.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ymo.jinqigufen.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://izn.bjfxy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xno.52xcode.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tcd.guannengcc.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fuj.fktsv.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://oof.guannengcc.top

[D25] Set 集合去重与交并差
来源：http://gcp.guowangkeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wyd.guannengcc.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hrp.meibo888.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://eea.cheryme.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xym.c1oappe.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zlp.bbcook.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://thd.fktsv.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jjn.xinyue.icu

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lax.zhaomingkeji.xyz

[D26] 数组转字符串
来源：http://vso.xuetiantiany.cn

Py:   ", ".join(map(str, arr))
来源：http://dia.gotoacloud.top

PHP:  implode(", ", $arr);
来源：http://njq.birdmap.top

JS:   arr.join(", ")
来源：http://tjq.hongshengwenyu.top

TS:   arr.join(", ")
来源：http://txl.fanxiaobao.xyz

Java: String.join(", ", list)
来源：http://aps.gzhubu.top

Go:   strings.Join(strs, ", ")
来源：http://ryx.shuidangran.top

Ruby: arr.join(", ")
来源：http://zbf.gaohongyu789.top

C#:   string.Join(", ", list)
来源：http://bno.uphjek.com

================================================================================
来源：http://bkt.jinghuilouyu.cn

E. 字符串处理
来源：http://eix.nanxinkj.top

================================================================================
来源：http://bha.guowangkeji.top

[E01] 拼接字符串
来源：http://awd.ehwqpu.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://omd.smart0.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mxx.sysykeji.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nsa.yangfankeji.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://avu.hcnkem.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://usk.yj202588.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://atw.svipenyu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xvn.gaohongyu789.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://iog.dianchejie.cn

[E02] 重复字符串
来源：http://lhc.ybcxt.top

Py:   "ab" * 3
来源：http://gbv.ybcxt.top

PHP:  str_repeat("ab", 3);
来源：http://glv.kuanghao11.cn

JS:   "ab".repeat(3)
来源：http://pie.hysaishi.cn

TS:   "ab".repeat(3)
来源：http://gjd.zhijiandao.cn

Java: "ab".repeat(3)
来源：http://ssk.hywenlv.cn

Go:   strings.Repeat("ab", 3)
来源：http://fqj.daria6918.cn

Ruby: "ab" * 3
来源：http://yil.bjfxy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wfw.daria6918.cn

[E03] 截取子串
来源：http://dzj.fehbvm.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cng.chenzaomai.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tcu.nanxuanxn.top


<!-- 参考信息 -->