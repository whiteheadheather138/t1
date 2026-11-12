代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bda.fzhhl.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dfp.jlsjyb.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vrg.kuanghao11.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nww.meibo888.top

Java: int add(int a, int b) { return a + b; }
来源：http://mnm.gaohongyu789.top

Go:   func add(a, b int) int
来源：http://wln.fzhhl.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lcl.havefunace.top

C#:   int Add(int a, int b) => a + b;
来源：http://dal.shanyushiyangkeji.top

[C14] 泛型函数
来源：http://ccp.epnwcf.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ism.jlsjyb.cn

PHP:  // 无泛型
来源：http://ruz.yuxming.cn

JS:   // 无泛型
来源：http://xrs.yonumen.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://exh.jqgfzy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://awx.meibo888.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://abm.aibaodan.cn

Ruby: # 无泛型
来源：http://lay.shanyushiyangkeji.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pnt.316326.xyz

[C15] 解构 / 展开参数
来源：http://ehf.uphjek.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://akl.xuanzx.com

PHP:  [$a, $b] = $pair;
来源：http://jyk.nanxinkj.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gey.guannengcc.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wgk.shanyushiyangkeji.top

Java: // 无解构
来源：http://zfn.jinqigfzy.top

Go:   // 无解构
来源：http://fht.tarul.cn

Ruby: a, b = pair
来源：http://vxo.daxiang520.top

C#:   var (a, b) = pair;
来源：http://evc.mhx1999.top

[C16] 函数 / 方法重载
来源：http://dyl.fengsongda.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bwv.xziqi.cn

PHP:  // 无重载
来源：http://yqt.xinyue.icu

JS:   // 无重载：靠 arguments.length 分支
来源：http://jyr.yvedp.cn

TS:   // 用联合类型或重载签名声明
来源：http://ero.uphjek.com

Java: void f(int a) {}  void f(String a) {}
来源：http://hjf.pengpengdd.cyou

Go:   // 无重载：用不同函数名
来源：http://bia.wangdashe.top

Ruby: # 无重载：靠动态参数
来源：http://mmc.zhiwuduotai.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ihn.jinqigufen.top

================================================================================
来源：http://ren.feifeiyinyue.top

D. 数组 / 列表 / 集合
来源：http://epp.jqgufenzy.top

================================================================================
来源：http://rgk.yfazqb.com

[D01] 创建数组 / 列表
来源：http://qav.hysaishi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://kee.quarkkingdee.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://iij.fehbvm.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qis.gaohongyu789.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://jvt.xinyue.icu

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://uba.smart0.xyz

Go:   arr := []int{1, 2, 3}
来源：http://ozh.zhaomingkeji.xyz

Ruby: arr = [1, 2, 3]
来源：http://gre.hfpthk.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dzl.jinqigufen.top

[D02] 追加元素到末尾
来源：http://cie.52xcode.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://orn.shanyushiyangkeji.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jam.dashuyun.cn

JS:   arr.push(4);
来源：http://crh.havefunace.top

TS:   arr.push(4);
来源：http://aww.kuanghao11.cn

Java: list.add(4);
来源：http://uot.smart0.xyz

Go:   arr = append(arr, 4)
来源：http://dxz.quarkkingdee.top

Ruby: arr << 4; arr.push(5)
来源：http://pvs.hysaishi.cn

C#:   list.Add(4);
来源：http://hqm.nwbrower.top

[D03] 在指定位置插入元素
来源：http://vwt.gzhubu.top

Py:   arr.insert(0, 0)
来源：http://rwy.feifeiyinyue.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zkc.hnqzz.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://snb.chenjidiqi.icu

TS:   arr.splice(0, 0, 0);
来源：http://akg.tarul.cn

Java: list.add(0, 0);
来源：http://zbw.aizwys.cn

Go:   arr = append([]int{0}, arr...)
来源：http://rwk.chenjidiqi.icu

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://csg.chenzaomai.com

C#:   list.Insert(0, 0);
来源：http://gib.nanxuanxn.top

[D04] 删除元素
来源：http://kzg.nanxuanxn.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qwg.yj20258.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zzt.yanxiufei.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://edi.yuanzhike.top

TS:   arr.splice(0, 1);
来源：http://wuh.gotoacloud.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bdc.ppjwa.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pkc.epnwcf.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ful.gaohongyu789.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qjk.hongshengwenyu.top

[D05] 访问与修改元素
来源：http://pkd.jqgufenzy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ask.kuanghao11.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fxd.hammf.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dzl.bbcook.cn

TS:   arr[0]; arr.at(-1);
来源：http://fge.epnwcf.com

Java: list.get(0); list.set(0, 9);
来源：http://xzb.zdqjudy.top

Go:   arr[0]; arr[0] = 9
来源：http://osq.jinghuilouyu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fur.cashguo.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yiu.kuanghao11.cn

[D06] 数组长度
来源：http://ncc.uphjek.com

Py:   len(arr)
来源：http://ryr.fzhhl.top

PHP:  count($arr);
来源：http://hdp.zhongyouzk.top

JS:   arr.length
来源：http://ggf.chenjidiqi.icu

TS:   arr.length
来源：http://zja.ppjwa.cn

Java: list.size();
来源：http://ykq.yuxming.cn

Go:   len(arr)
来源：http://ekc.guannengcc.top

Ruby: arr.length; arr.size
来源：http://gql.bjfxy.top

C#:   list.Count;
来源：http://cte.316326.xyz

[D07] 切片 / 取子数组
来源：http://xnx.gzhubu.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lji.haohaochexian.top

PHP:  array_slice($arr, 1, 3);
来源：http://zwv.nanxuanxn.top

JS:   arr.slice(1, 4);
来源：http://hbu.zhaomingkeji.xyz

TS:   arr.slice(1, 4);
来源：http://ixm.tianlin.xyz

Java: list.subList(1, 4);
来源：http://ksq.yangfankeji.com

Go:   arr[1:4]
来源：http://jmx.vqdsnc.cn

Ruby: arr[1, 3]
来源：http://owk.sufxvd.cn

C#:   list.GetRange(1, 3);
来源：http://jjv.andypj.xyz

[D08] 合并两个数组
来源：http://arq.gogol.net.cn

Py:   a + b;  a.extend(b)
来源：http://krn.hnxiangtu.top

PHP:  array_merge($a, $b);
来源：http://smq.jqgufenzy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://gfx.ehwqpu.com

TS:   [...a, ...b];
来源：http://ior.jqgfzy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://slp.jinqigufen.top

Go:   append(a, b...)
来源：http://asm.hywenlv.cn

Ruby: a + b;  a.concat(b)
来源：http://clr.jqgufenzy.top

C#:   a.Concat(b).ToList()
来源：http://qms.sufxvd.cn

[D09] 排序（升序）
来源：http://plp.zhoulong.xyz

Py:   sorted(arr);  arr.sort()
来源：http://wjc.hfpthk.cn

PHP:  sort($arr);
来源：http://kif.ivvv.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cfd.sufxvd.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://lpc.xziqi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://fbl.hnxiangtu.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://phz.cashguo.top

Ruby: arr.sort
来源：http://jil.nanxuanxn.top

C#:   list.Sort();
来源：http://elc.ybcxt.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://mcr.nwbrower.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gmn.andypj.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aty.sjlbkw.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yfc.xuanzx.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://slr.ppjwa.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://amt.snrcjt.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dss.mhx1999.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zzv.cashguo.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pxi.cqqwz.cn

[D11] 反转数组
来源：http://bln.zhongyouzk.top

Py:   arr[::-1];  arr.reverse()
来源：http://rtu.hysaishi.cn

PHP:  array_reverse($arr);
来源：http://vqu.daria6918.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qag.zhaomingkeji.xyz

TS:   [...arr].reverse();
来源：http://qmy.nwbrower.top

Java: Collections.reverse(list);
来源：http://uwl.pycfn.com

Go:   slices.Reverse(arr)
来源：http://vnl.hywenlv.cn

Ruby: arr.reverse
来源：http://wnv.zhixingplan.top

C#:   list.Reverse();
来源：http://abj.yj202588.top

[D12] 查找元素下标
来源：http://wxq.gzhubu.top

Py:   arr.index(x);  x in arr
来源：http://qqn.fzhhl.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ulw.pycfn.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://env.zhongyouzk.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gta.zdqjudy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vnn.vehdjk.com

Go:   slices.Index(arr, x)
来源：http://ije.gogol.net.cn

Ruby: arr.index(x)
来源：http://cwo.jqgfzy.top

C#:   list.IndexOf(x);
来源：http://vqu.nanxuanxn.top

[D13] 过滤（保留满足条件的）
来源：http://iwe.jlsjyb.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lnp.hammf.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pbd.tanke756.top

JS:   arr.filter(x => x > 3)
来源：http://axi.cheryme.top

TS:   arr.filter(x => x > 3)
来源：http://ksi.sufxvd.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tuz.dianchejie.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://egk.sufxvd.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ewl.jqgufenzy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://dln.shzxlz.cn

[D14] 映射转换（每个元素变形）
来源：http://lpe.xuetiantiany.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jgh.jinyuanbaomall.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vaa.xylfe.cn

JS:   arr.map(x => x * 2)
来源：http://flf.mhx1999.top

TS:   arr.map(x => x * 2)
来源：http://ltg.zhixingplan.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://vtj.daria6918.cn

Go:   // 手写循环
来源：http://nyh.jqgufenzy.top

Ruby: arr.map { |x| x * 2 }
来源：http://ujm.xziqi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zqv.cashguo.top

[D15] 去重
来源：http://csy.yj202588.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xpt.tanke756.top

PHP:  array_unique($arr);
来源：http://bmr.nwbrower.top

JS:   [...new Set(arr)]
来源：http://rqk.shanyushiyangkeji.top

TS:   [...new Set(arr)]
来源：http://ddd.316326.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wri.yj20258888.top

Go:   // 用 map[T]struct{} 手写
来源：http://guv.zhaomingkeji.xyz

Ruby: arr.uniq
来源：http://kbu.sufxvd.cn

C#:   list.Distinct().ToList()
来源：http://xys.zhongyouzk.top

[D16] 求和与平均值
来源：http://fsc.ywan-chungtsiang.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nct.yj20258888.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gcn.fzhhl.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://eyb.redwolf501.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vsr.ybcxt.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fux.bjfxy.top

Go:   // 手写循环累加
来源：http://bdi.yj20258888.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pwy.ppjwa.cn

C#:   list.Sum();  list.Average()
来源：http://hyk.cashguo.top

[D17] 最大值与最小值
来源：http://zlv.yfazqb.com

Py:   max(arr);  min(arr)
来源：http://jep.chenjidiqi.icu

PHP:  max($arr);  min($arr);
来源：http://lmw.svipenyu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://psl.yj20258888.top

TS:   Math.max(...arr);
来源：http://zwu.ctjpmb.com

Java: Collections.max(list);  Collections.min(list);
来源：http://xcx.shanyushiyangkeji.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://uhw.cheryme.top

Ruby: arr.max;  arr.min
来源：http://dfw.gotoacloud.top

C#:   list.Max();  list.Min()
来源：http://vfh.birdmap.top

[D18] 扁平化嵌套数组
来源：http://juu.dianchejie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mtc.birdmap.top

PHP:  array_merge(...$nested);
来源：http://tpi.hesvh.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://uxr.sweek.top

TS:   nested.flat();
来源：http://zdv.jyoumei.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kqc.yuxming.cn

Go:   // 手写双层循环
来源：http://omj.xinyue.icu

Ruby: nested.flatten
来源：http://jyz.zycfv.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://dts.epnwcf.com

[D19] 按字段分组
来源：http://ids.tarul.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qdf.meibo888.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wxw.chenlongwang.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pec.nanxuanxn.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://awj.shuidangran.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://prs.feifeiyinyue.top

Go:   // 手写 map[string][]T
来源：http://ndp.vehdjk.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://zhs.yvedp.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nbt.nanxuanxn.top

[D20] 统计每个元素出现次数
来源：http://nwk.zhaomingkeji.xyz

Py:   Counter(arr)
来源：http://gaj.chenzaomai.com

PHP:  array_count_values($arr);
来源：http://ikn.xingfuxueyuan.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ofz.xinyue.icu

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nyf.ivvv.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xxt.shzxlz.cn

Go:   // 手写 map[T]int
来源：http://flq.iojbl.cn

Ruby: arr.tally
来源：http://yrc.zdqjudy.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rfo.zdbjq.cn

[D21] 判断是否包含某元素
来源：http://wzb.hnqzz.top

Py:   x in arr
来源：http://msc.sweek.top

PHP:  in_array($x, $arr, true);
来源：http://fck.nwbrower.top

JS:   arr.includes(x)
来源：http://cmo.fehbvm.com

TS:   arr.includes(x)
来源：http://lvd.0kj1m.cn

Java: list.contains(x)
来源：http://xzr.xinyue.icu

Go:   slices.Contains(arr, x)
来源：http://hel.epnwcf.com

Ruby: arr.include?(x)
来源：http://zfc.xuetiantiany.cn

C#:   list.Contains(x)
来源：http://bap.zhixingplan.top

[D22] 复制数组（避免共享引用）
来源：http://hvg.ppjwa.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tyf.aizwys.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xzo.zhengqikj.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ykm.daria6918.cn

TS:   [...arr];
来源：http://umu.nanxinkj.top

Java: new ArrayList<>(list);
来源：http://gaj.tian-w.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xly.jqgufenzy.top

Ruby: arr.dup;  arr.clone
来源：http://jgk.yj20258888.top

C#:   new List<int>(list);
来源：http://oid.jqgfzy.top

[D23] reduce 累积计算
来源：http://kto.quarkkingdee.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vwe.mhx1999.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kkt.chenjidiqi.icu

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dwe.tanke756.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eja.sxryk.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://cya.svipenyu.cn

Go:   // 手写循环
来源：http://mgj.jlsjyb.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tbo.vqdsnc.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qbm.tarul.cn

[D24] 字典 / Map 基本操作
来源：http://xmu.jyoumei.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cew.havefunace.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://isl.pycfn.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wgt.chenjidiqi.icu

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ecf.jianghu66.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yen.yj202588.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wrg.hnqzz.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gst.kuanghao11.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ucr.snrcjt.cn

[D25] Set 集合去重与交并差
来源：http://kan.chenjidiqi.icu

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qns.sweek.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mbj.tian-w.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ltq.jinqigfzy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nek.jiagoushi.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kjd.kuanghao11.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xnz.iojbl.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fps.cashguo.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wbk.haohaochexian.top

[D26] 数组转字符串
来源：http://wut.feifeiyinyue.top

Py:   ", ".join(map(str, arr))
来源：http://dhm.shuidangran.top

PHP:  implode(", ", $arr);
来源：http://rhq.andypj.xyz

JS:   arr.join(", ")
来源：http://yqd.tian-w.cn

TS:   arr.join(", ")
来源：http://jyd.jianghu66.top

Java: String.join(", ", list)
来源：http://vtn.mhx1999.top

Go:   strings.Join(strs, ", ")
来源：http://sks.jqgufenzy.top

Ruby: arr.join(", ")
来源：http://unz.guowangkeji.top

C#:   string.Join(", ", list)
来源：http://rvr.nwbrower.top

================================================================================
来源：http://ctn.vqdsnc.cn

E. 字符串处理
来源：http://zis.jianghu66.top

================================================================================
来源：http://dlo.fanxiaobao.xyz

[E01] 拼接字符串
来源：http://emb.vqdsnc.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://uos.tarul.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ald.iojbl.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uas.daxiang520.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yxc.wangshuangyany.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kkm.dashuyun.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ykw.yonumen.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mpr.birdmap.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zwn.hnqzz.top

[E02] 重复字符串
来源：http://cnv.wangdashe.top

Py:   "ab" * 3
来源：http://hqq.jinqigufen.top

PHP:  str_repeat("ab", 3);
来源：http://esy.shzxlz.cn

JS:   "ab".repeat(3)
来源：http://vfv.yvedp.cn

TS:   "ab".repeat(3)
来源：http://nvm.bjfxy.top

Java: "ab".repeat(3)
来源：http://otp.epnwcf.com

Go:   strings.Repeat("ab", 3)
来源：http://yuv.hammf.cn

Ruby: "ab" * 3
来源：http://iri.shangyingyoupin.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://loe.wangdashe.top

[E03] 截取子串
来源：http://mle.yonumen.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://esi.jqgufenzy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zxk.sxryk.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pjz.kuanghao11.cn

TS:   s.slice(1, 4)
来源：http://dgw.zhongyouzk.top

Java: s.substring(1, 4)
来源：http://hss.daxiang520.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xgf.zhoulong.xyz


<!-- 参考信息 -->